# Comparing `tmp/lg_april_permissions-0.1.7.tar.gz` & `tmp/lg_april_permissions-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lg_april_permissions-0.1.7.tar", max compression
+gzip compressed data, was "lg_april_permissions-0.1.8.tar", max compression
```

## Comparing `lg_april_permissions-0.1.7.tar` & `lg_april_permissions-0.1.8.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     6891 2023-04-05 13:50:30.283574 lg_april_permissions-0.1.7/README.md
--rw-r--r--   0        0        0     8044 2023-04-06 09:57:54.237981 lg_april_permissions-0.1.7/lg_april_permissions/__init__.py
--rw-r--r--   0        0        0      753 2023-04-06 09:58:49.374643 lg_april_permissions-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     7442 1970-01-01 00:00:00.000000 lg_april_permissions-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     7230 2023-04-08 21:31:25.553760 lg_april_permissions-0.1.8/README.md
+-rw-r--r--   0        0        0     9746 2023-04-23 09:06:42.532808 lg_april_permissions-0.1.8/lg_april_permissions/__init__.py
+-rw-r--r--   0        0        0      753 2023-04-23 09:10:32.089976 lg_april_permissions-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     7781 1970-01-01 00:00:00.000000 lg_april_permissions-0.1.8/PKG-INFO
```

### Comparing `lg_april_permissions-0.1.7/README.md` & `lg_april_permissions-0.1.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # buditool
-Das Tool dient hauptsächlich zum synchronisieren von Berechtigungen: es schaut in die Postgres-DB (April_Permissions) und schickt API calls an Budibase, um die Berechtigungen zu setzten. Bitte auch die KNOWN ISSUES in tests/bb_test.py lesen!
+Das Tool dient hauptsächlich zum synchronisieren von Berechtigungen: es schaut in die Postgres-DB (April_Permissions) und schickt API calls an Budibase, um die Berechtigungen zu setzten. Bitte auch die KNOWN ISSUES in tests/bb_test.py lesen! Die entsprechenden Images werden über die CI gebaut und können einfach von unserer Registry gepullt werden:
+- buditool --serve: https://git.itsnow.biz/LG-IT/docker-lg-april-permissions
+- Postgres mit curl: https://git.itsnow.biz/LG-IT/docker-lg-postgres
+- all unsere Images (heißt hier Packges): https://git.itsnow.biz/LG-IT/-/packages
 
 ### Features 
 ```bash
 kmille@linbox:lg-april-permissions ~/.local/bin/buditool -h
 usage: buditool [-h] [-u USER] [--list-apps] [--list-users] [-a ADD_PERMISSIONS] [-r REMOVE_PERMISSIONS] [-s] [-c CONFIG] [--version]
 
 options:
```

### Comparing `lg_april_permissions-0.1.7/lg_april_permissions/__init__.py` & `lg_april_permissions-0.1.8/lg_april_permissions/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -106,26 +106,66 @@
             fail(f"Status code: {resp.status_code}\n{resp.text}")
         j = resp.json()
     except Exception as e:
         fail(e)
     return j
 
 
-def show_users() -> None:
+def get_users() -> dict:
     try:
         resp = session.post(BB_BASE_API_URL + "users/search")
         if resp.status_code != 200:
             fail(f"Status code: {resp.status_code}\n{resp.text}")
         j = resp.json()
     except Exception as e:
         fail(e)
     users = j['data']
+    return users
+
+
+def show_users() -> None:
+    users = get_users()
     print(json.dumps(users, indent=4))
 
 
+def show_users_by_app(filter_app_id: str) -> None:
+    users = get_users()
+    for user in users:
+        for app_id, permission in user['roles'].items():
+            if app_id == filter_app_id:
+                name = f"{user['firstName']} {user['lastName']}"
+                print(f"{user['_id']} | {name:<35} | {user['email']:<40} | {permission}")
+
+
+def bikoe_migration():
+    """Jede, die Zugriff auf die Protest-Buffet App hat, bekommt BASIC Rechte für die Bikö-Krönung App - wird nur einmal benötigt"""
+    buffet_app_id = "app_6bb0b333c2fd43fb98f4b54a67e17c14"
+    biko_kroenung_id = "app_f06982298ecc47b7b5ab9019c7fbd1a8"
+
+    def add_bikeo_permissions(userid: str):
+        print(f"Adding BikÖ permissions for user {userid}")
+        u = get_user(userid)
+        roles = u['data']['roles']
+        print(f"Rollen vorher:\n{json.dumps(roles, indent=4)}")
+        perm = {biko_kroenung_id: "BASIC"}
+        roles.update(perm)
+
+        u = update_user_roles(userid, roles)
+        roles = u['data']['roles']
+        print(f"Rollen danach:\n{json.dumps(roles, indent=4)}")
+
+    users = get_users()
+    for user in users:
+        for app_id, permission in user['roles'].items():
+            if app_id == buffet_app_id:
+                name = f"{user['firstName']} {user['lastName']}"
+                print(f"{user['_id']} | {name:<35} | {user['email']:<40} | {permission}")
+                add_bikeo_permissions(user['_id'])
+
+
 def show_user(userid: str) -> None:
     u = get_user(userid)
     print(json.dumps(u, indent=4))
 
 
 def update_user_roles(userid: str, roles: dict) -> None:
     try:
@@ -202,14 +242,15 @@
 
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument("-u", "--user", help="show user (needs bb user id)")
     parser.add_argument("--list-apps", action="store_true", help="list all bb apps")
     parser.add_argument("--list-users", action="store_true", help="list all bb users")
+    parser.add_argument("--show-users-by-app", help="list all users and their permissions for a specific <app id>")
     parser.add_argument("-a", "--add-permissions", help="add permissions for user (needs bb user id)")
     parser.add_argument("-r", "--remove-permissions", help="remove permissions for user (needs bb user id)")
     parser.add_argument("-s", "--sync", action="store_true", help="synchronize permissions with db")
     parser.add_argument("-c", "--config", help="config file")
     parser.add_argument("--serve", action="store_true", help="run backend with /sync to run --sync by webhook")
     parser.add_argument("--version", action="store_true", help="show version")
 
@@ -229,14 +270,16 @@
         show_apps()
     elif args.list_users:
         show_users()
     elif args.add_permissions:
         add_permissions(args.add_permissions)
     elif args.remove_permissions:
         remove_permissions(args.remove_permissions)
+    elif args.show_users_by_app:
+        show_users_by_app(args.show_users_by_app)
     elif args.sync:
         err, err_msg = sync_db_permissions()
         if err:
             print(err_msg)
             sys.exit(1)
     elif args.serve:
         run_backend()
```

### Comparing `lg_april_permissions-0.1.7/pyproject.toml` & `lg_april_permissions-0.1.8/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lg-april-permissions"
-version = "0.1.7"
+version = "0.1.8"
 description = ""
 authors = ["kmille <github@androidloves.me>"]
 readme = "README.md"
 packages = [{include = "lg_april_permissions"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `lg_april_permissions-0.1.7/PKG-INFO` & `lg_april_permissions-0.1.8/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lg-april-permissions
-Version: 0.1.7
+Version: 0.1.8
 Summary: 
 Author: kmille
 Author-email: github@androidloves.me
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -12,15 +12,18 @@
 Requires-Dist: psycopg2-binary (>=2.9.6,<3.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: waitress (>=2.1.2,<3.0.0)
 Description-Content-Type: text/markdown
 
 # buditool
-Das Tool dient hauptsächlich zum synchronisieren von Berechtigungen: es schaut in die Postgres-DB (April_Permissions) und schickt API calls an Budibase, um die Berechtigungen zu setzten. Bitte auch die KNOWN ISSUES in tests/bb_test.py lesen!
+Das Tool dient hauptsächlich zum synchronisieren von Berechtigungen: es schaut in die Postgres-DB (April_Permissions) und schickt API calls an Budibase, um die Berechtigungen zu setzten. Bitte auch die KNOWN ISSUES in tests/bb_test.py lesen! Die entsprechenden Images werden über die CI gebaut und können einfach von unserer Registry gepullt werden:
+- buditool --serve: https://git.itsnow.biz/LG-IT/docker-lg-april-permissions
+- Postgres mit curl: https://git.itsnow.biz/LG-IT/docker-lg-postgres
+- all unsere Images (heißt hier Packges): https://git.itsnow.biz/LG-IT/-/packages
 
 ### Features 
 ```bash
 kmille@linbox:lg-april-permissions ~/.local/bin/buditool -h
 usage: buditool [-h] [-u USER] [--list-apps] [--list-users] [-a ADD_PERMISSIONS] [-r REMOVE_PERMISSIONS] [-s] [-c CONFIG] [--version]
 
 options:
```

