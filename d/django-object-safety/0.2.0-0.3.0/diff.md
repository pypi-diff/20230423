# Comparing `tmp/django_object_safety-0.2.0.tar.gz` & `tmp/django_object_safety-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_object_safety-0.2.0.tar", max compression
+gzip compressed data, was "django_object_safety-0.3.0.tar", max compression
```

## Comparing `django_object_safety-0.2.0.tar` & `django_object_safety-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1081 2023-04-22 17:57:27.834494 django_object_safety-0.2.0/LICENSE
--rw-r--r--   0        0        0      129 2023-04-22 18:09:42.813595 django_object_safety-0.2.0/README.md
--rw-r--r--   0        0        0      688 2023-04-23 14:47:21.436314 django_object_safety-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-16 18:28:46.023260 django_object_safety-0.2.0/safety/__init__.py
--rw-r--r--   0        0        0       63 2023-04-16 18:28:46.023260 django_object_safety-0.2.0/safety/admin.py
--rw-r--r--   0        0        0      144 2023-04-16 18:28:46.023260 django_object_safety-0.2.0/safety/apps.py
--rw-r--r--   0        0        0     1705 2023-04-22 17:57:27.834494 django_object_safety-0.2.0/safety/migrations/0001_initial.py
--rw-r--r--   0        0        0      949 2023-04-22 17:57:27.834494 django_object_safety-0.2.0/safety/migrations/0002_alter_objectpermission_object_ct_and_more.py
--rw-r--r--   0        0        0      445 2023-04-22 17:57:27.834494 django_object_safety-0.2.0/safety/migrations/0003_alter_objectpermission_options.py
--rw-r--r--   0        0        0     2656 2023-04-22 17:57:27.834494 django_object_safety-0.2.0/safety/migrations/0004_alter_objectpermission_unique_together_and_more.py
--rw-r--r--   0        0        0      744 2023-04-22 17:57:27.834494 django_object_safety-0.2.0/safety/migrations/0005_alter_permissiongroup_target_id_and_more.py
--rw-r--r--   0        0        0      444 2023-04-22 17:57:27.834494 django_object_safety-0.2.0/safety/migrations/0006_alter_objectpermission_options.py
--rw-r--r--   0        0        0      434 2023-04-22 17:57:27.834494 django_object_safety-0.2.0/safety/migrations/0007_alter_objectpermission_options.py
--rw-r--r--   0        0        0      571 2023-04-22 17:57:27.834494 django_object_safety-0.2.0/safety/migrations/0008_rename_permissiongroup_objectgroup.py
--rw-r--r--   0        0        0        0 2023-04-16 19:30:41.012284 django_object_safety-0.2.0/safety/migrations/__init__.py
--rw-r--r--   0        0        0     2461 2023-04-22 17:57:27.834494 django_object_safety-0.2.0/safety/models.py
--rw-r--r--   0        0        0    12344 2023-04-23 14:45:56.144510 django_object_safety-0.2.0/safety/shortcuts.py
--rw-r--r--   0        0        0     6153 2023-04-23 14:45:56.136510 django_object_safety-0.2.0/safety/tests.py
--rw-r--r--   0        0        0       63 2023-04-16 18:28:46.023260 django_object_safety-0.2.0/safety/views.py
--rw-r--r--   0        0        0      819 1970-01-01 00:00:00.000000 django_object_safety-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-04-22 17:57:27.834494 django_object_safety-0.3.0/LICENSE
+-rw-r--r--   0        0        0      129 2023-04-22 18:09:42.813595 django_object_safety-0.3.0/README.md
+-rw-r--r--   0        0        0      688 2023-04-23 15:01:36.694395 django_object_safety-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-16 18:28:46.023260 django_object_safety-0.3.0/safety/__init__.py
+-rw-r--r--   0        0        0       63 2023-04-16 18:28:46.023260 django_object_safety-0.3.0/safety/admin.py
+-rw-r--r--   0        0        0      144 2023-04-16 18:28:46.023260 django_object_safety-0.3.0/safety/apps.py
+-rw-r--r--   0        0        0     1705 2023-04-22 17:57:27.834494 django_object_safety-0.3.0/safety/migrations/0001_initial.py
+-rw-r--r--   0        0        0      949 2023-04-22 17:57:27.834494 django_object_safety-0.3.0/safety/migrations/0002_alter_objectpermission_object_ct_and_more.py
+-rw-r--r--   0        0        0      445 2023-04-22 17:57:27.834494 django_object_safety-0.3.0/safety/migrations/0003_alter_objectpermission_options.py
+-rw-r--r--   0        0        0     2656 2023-04-22 17:57:27.834494 django_object_safety-0.3.0/safety/migrations/0004_alter_objectpermission_unique_together_and_more.py
+-rw-r--r--   0        0        0      744 2023-04-22 17:57:27.834494 django_object_safety-0.3.0/safety/migrations/0005_alter_permissiongroup_target_id_and_more.py
+-rw-r--r--   0        0        0      444 2023-04-22 17:57:27.834494 django_object_safety-0.3.0/safety/migrations/0006_alter_objectpermission_options.py
+-rw-r--r--   0        0        0      434 2023-04-22 17:57:27.834494 django_object_safety-0.3.0/safety/migrations/0007_alter_objectpermission_options.py
+-rw-r--r--   0        0        0      571 2023-04-22 17:57:27.834494 django_object_safety-0.3.0/safety/migrations/0008_rename_permissiongroup_objectgroup.py
+-rw-r--r--   0        0        0        0 2023-04-16 19:30:41.012284 django_object_safety-0.3.0/safety/migrations/__init__.py
+-rw-r--r--   0        0        0     2461 2023-04-22 17:57:27.834494 django_object_safety-0.3.0/safety/models.py
+-rw-r--r--   0        0        0    12348 2023-04-23 15:01:19.966432 django_object_safety-0.3.0/safety/shortcuts.py
+-rw-r--r--   0        0        0     6153 2023-04-23 14:45:56.136510 django_object_safety-0.3.0/safety/tests.py
+-rw-r--r--   0        0        0       63 2023-04-16 18:28:46.023260 django_object_safety-0.3.0/safety/views.py
+-rw-r--r--   0        0        0      819 1970-01-01 00:00:00.000000 django_object_safety-0.3.0/PKG-INFO
```

### Comparing `django_object_safety-0.2.0/LICENSE` & `django_object_safety-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_object_safety-0.2.0/pyproject.toml` & `django_object_safety-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-object-safety"
-version = "0.2.0"
+version = "0.3.0"
 description = "Adds object permissions to Django."
 license = "MIT"
 authors = ["William Ferreira"]
 homepage = "https://django-object-safety-docs.readthedocs.io/"
 repository = "https://github.com/williammferreira/django-object-safety/"
 keywords = ["django", "permissions", "object-permissions", "django-permissions", "django-object-permissions"]
 readme = "README.md"
```

### Comparing `django_object_safety-0.2.0/safety/migrations/0001_initial.py` & `django_object_safety-0.3.0/safety/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-0.2.0/safety/migrations/0002_alter_objectpermission_object_ct_and_more.py` & `django_object_safety-0.3.0/safety/migrations/0002_alter_objectpermission_object_ct_and_more.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-0.2.0/safety/migrations/0004_alter_objectpermission_unique_together_and_more.py` & `django_object_safety-0.3.0/safety/migrations/0004_alter_objectpermission_unique_together_and_more.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-0.2.0/safety/migrations/0005_alter_permissiongroup_target_id_and_more.py` & `django_object_safety-0.3.0/safety/migrations/0005_alter_permissiongroup_target_id_and_more.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-0.2.0/safety/migrations/0008_rename_permissiongroup_objectgroup.py` & `django_object_safety-0.3.0/safety/migrations/0008_rename_permissiongroup_objectgroup.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-0.2.0/safety/models.py` & `django_object_safety-0.3.0/safety/models.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-0.2.0/safety/shortcuts.py` & `django_object_safety-0.3.0/safety/shortcuts.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,17 +220,17 @@
     if not group_obj_perm.exists():
         return False
 
     group_obj_perm.delete()
     return True
 
 
-def get_perm_group(name: str, obj) -> ObjectGroup:
+def retrieve_object_group(name: str, obj) -> ObjectGroup:
     """
-    Get a permission group.
+    Get an object group.
 
     Args:
         name (string): The name of the group.
         obj: The object to get the group from.
 
     Returns:
         Group: The group object.
```

### Comparing `django_object_safety-0.2.0/safety/tests.py` & `django_object_safety-0.3.0/safety/tests.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-0.2.0/PKG-INFO` & `django_object_safety-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-object-safety
-Version: 0.2.0
+Version: 0.3.0
 Summary: Adds object permissions to Django.
 Home-page: https://django-object-safety-docs.readthedocs.io/
 License: MIT
 Keywords: django,permissions,object-permissions,django-permissions,django-object-permissions
 Author: William Ferreira
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

