# Comparing `tmp/lg_april_permissions-0.1.8.tar.gz` & `tmp/lg_april_permissions-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lg_april_permissions-0.1.8.tar", max compression
+gzip compressed data, was "lg_april_permissions-0.1.9.tar", max compression
```

## Comparing `lg_april_permissions-0.1.8.tar` & `lg_april_permissions-0.1.9.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     7230 2023-04-08 21:31:25.553760 lg_april_permissions-0.1.8/README.md
--rw-r--r--   0        0        0     9746 2023-04-23 09:06:42.532808 lg_april_permissions-0.1.8/lg_april_permissions/__init__.py
--rw-r--r--   0        0        0      753 2023-04-23 09:10:32.089976 lg_april_permissions-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     7781 1970-01-01 00:00:00.000000 lg_april_permissions-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     7230 2023-04-08 21:31:25.553760 lg_april_permissions-0.1.9/README.md
+-rw-r--r--   0        0        0     9960 2023-04-23 19:19:54.402891 lg_april_permissions-0.1.9/lg_april_permissions/__init__.py
+-rw-r--r--   0        0        0      753 2023-04-23 19:20:23.199571 lg_april_permissions-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     7781 1970-01-01 00:00:00.000000 lg_april_permissions-0.1.9/PKG-INFO
```

### Comparing `lg_april_permissions-0.1.8/README.md` & `lg_april_permissions-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `lg_april_permissions-0.1.8/lg_april_permissions/__init__.py` & `lg_april_permissions-0.1.9/lg_april_permissions/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import os
 import json
 from pathlib import Path
 import yaml
 import psycopg2
 import importlib.metadata
 import waitress
+from datetime import datetime
+
 
 BB_BASE_API_URL = None
 BB_API_KEY = None
 PERMISSIONS = None
 DB_CONNECTION = None
 LISTEN_PORT = None
 
@@ -76,15 +78,15 @@
         #Thread(target=sync_db_permissions).start()
         err, err_msg = sync_db_permissions()
         if err:
             return jsonify(error=str(err_msg)), 500
         else:
             return jsonify(status="ok"), 200
 
-    print(f"Starting webhook backend on port {LISTEN_PORT} (version {__version__}")
+    print(f"Starting webhook backend on port {LISTEN_PORT} (version {__version__})")
     # run debug server if started with poetry run python lg_april_permissions/__init__.py -c settings.yaml --serve
     if __name__ == '__main__':
         app.run(debug=True, port=LISTEN_PORT)
     else:
         waitress.serve(app, port=LISTEN_PORT)
 
 
@@ -180,16 +182,19 @@
 
 
 def add_permissions(userid: str):
     print(f"Adding permissions for user {userid}")
     u = get_user(userid)
     roles = u['data']['roles']
     print(f"Rollen vorher:\n{json.dumps(roles, indent=4)}")
-    roles.update(PERMISSIONS)
+    if PERMISSIONS.items() <= roles.items():
+        print(f"User {userid} already has the valid permissions. Skipping ...")
+        return
 
+    roles.update(PERMISSIONS)
     u = update_user_roles(userid, roles)
     roles = u['data']['roles']
     print(f"Rollen danach:\n{json.dumps(roles, indent=4)}")
 
 
 def remove_permissions(userid: str):
     print(f"Removing permissions for user {userid}")
@@ -207,15 +212,15 @@
     roles = u['data']['roles']
     u = update_user_roles(userid, roles)
     roles = u['data']['roles']
     print(f"Rollen danach:\n{json.dumps(roles, indent=4)}")
 
 
 def sync_db_permissions() -> (bool, str):
-    print("Syncing permissions with database")
+    print(f"Syncing permissions with database at {datetime.now().strftime('%H:%M:%S')}")
     try:
         conn = psycopg2.connect(DB_CONNECTION)
         cur = conn.cursor()
         cur.execute('SELECT fk_bikoe FROM "April_Permissions"')
         permissions = cur.fetchall()
         for permission in permissions:
             fk_bikoe = int(permission[0])
```

### Comparing `lg_april_permissions-0.1.8/pyproject.toml` & `lg_april_permissions-0.1.9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lg-april-permissions"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["kmille <github@androidloves.me>"]
 readme = "README.md"
 packages = [{include = "lg_april_permissions"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `lg_april_permissions-0.1.8/PKG-INFO` & `lg_april_permissions-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lg-april-permissions
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: kmille
 Author-email: github@androidloves.me
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

