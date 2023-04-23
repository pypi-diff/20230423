# Comparing `tmp/django_object_safety-0.1.4.tar.gz` & `tmp/django_object_safety-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_object_safety-0.1.4.tar", max compression
+gzip compressed data, was "django_object_safety-0.2.0.tar", max compression
```

## Comparing `django_object_safety-0.1.4.tar` & `django_object_safety-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1081 2023-04-22 17:57:27.834494 django_object_safety-0.1.4/LICENSE
--rw-r--r--   0        0        0      129 2023-04-22 18:09:42.813595 django_object_safety-0.1.4/README.md
--rw-r--r--   0        0        0      688 2023-04-22 18:10:00.117572 django_object_safety-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-16 18:28:46.023260 django_object_safety-0.1.4/safety/__init__.py
--rw-r--r--   0        0        0       63 2023-04-16 18:28:46.023260 django_object_safety-0.1.4/safety/admin.py
--rw-r--r--   0        0        0      144 2023-04-16 18:28:46.023260 django_object_safety-0.1.4/safety/apps.py
--rw-r--r--   0        0        0     1705 2023-04-22 17:57:27.834494 django_object_safety-0.1.4/safety/migrations/0001_initial.py
--rw-r--r--   0        0        0      949 2023-04-22 17:57:27.834494 django_object_safety-0.1.4/safety/migrations/0002_alter_objectpermission_object_ct_and_more.py
--rw-r--r--   0        0        0      445 2023-04-22 17:57:27.834494 django_object_safety-0.1.4/safety/migrations/0003_alter_objectpermission_options.py
--rw-r--r--   0        0        0     2656 2023-04-22 17:57:27.834494 django_object_safety-0.1.4/safety/migrations/0004_alter_objectpermission_unique_together_and_more.py
--rw-r--r--   0        0        0      744 2023-04-22 17:57:27.834494 django_object_safety-0.1.4/safety/migrations/0005_alter_permissiongroup_target_id_and_more.py
--rw-r--r--   0        0        0      444 2023-04-22 17:57:27.834494 django_object_safety-0.1.4/safety/migrations/0006_alter_objectpermission_options.py
--rw-r--r--   0        0        0      434 2023-04-22 17:57:27.834494 django_object_safety-0.1.4/safety/migrations/0007_alter_objectpermission_options.py
--rw-r--r--   0        0        0      571 2023-04-22 17:57:27.834494 django_object_safety-0.1.4/safety/migrations/0008_rename_permissiongroup_objectgroup.py
--rw-r--r--   0        0        0        0 2023-04-16 19:30:41.012284 django_object_safety-0.1.4/safety/migrations/__init__.py
--rw-r--r--   0        0        0     2461 2023-04-22 17:57:27.834494 django_object_safety-0.1.4/safety/models.py
--rw-r--r--   0        0        0    12352 2023-04-22 17:57:27.834494 django_object_safety-0.1.4/safety/shortcuts.py
--rw-r--r--   0        0        0     6111 2023-04-22 17:57:27.834494 django_object_safety-0.1.4/safety/tests.py
--rw-r--r--   0        0        0       63 2023-04-16 18:28:46.023260 django_object_safety-0.1.4/safety/views.py
--rw-r--r--   0        0        0      819 1970-01-01 00:00:00.000000 django_object_safety-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-04-22 17:57:27.834494 django_object_safety-0.2.0/LICENSE
+-rw-r--r--   0        0        0      129 2023-04-22 18:09:42.813595 django_object_safety-0.2.0/README.md
+-rw-r--r--   0        0        0      688 2023-04-23 14:47:21.436314 django_object_safety-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-16 18:28:46.023260 django_object_safety-0.2.0/safety/__init__.py
+-rw-r--r--   0        0        0       63 2023-04-16 18:28:46.023260 django_object_safety-0.2.0/safety/admin.py
+-rw-r--r--   0        0        0      144 2023-04-16 18:28:46.023260 django_object_safety-0.2.0/safety/apps.py
+-rw-r--r--   0        0        0     1705 2023-04-22 17:57:27.834494 django_object_safety-0.2.0/safety/migrations/0001_initial.py
+-rw-r--r--   0        0        0      949 2023-04-22 17:57:27.834494 django_object_safety-0.2.0/safety/migrations/0002_alter_objectpermission_object_ct_and_more.py
+-rw-r--r--   0        0        0      445 2023-04-22 17:57:27.834494 django_object_safety-0.2.0/safety/migrations/0003_alter_objectpermission_options.py
+-rw-r--r--   0        0        0     2656 2023-04-22 17:57:27.834494 django_object_safety-0.2.0/safety/migrations/0004_alter_objectpermission_unique_together_and_more.py
+-rw-r--r--   0        0        0      744 2023-04-22 17:57:27.834494 django_object_safety-0.2.0/safety/migrations/0005_alter_permissiongroup_target_id_and_more.py
+-rw-r--r--   0        0        0      444 2023-04-22 17:57:27.834494 django_object_safety-0.2.0/safety/migrations/0006_alter_objectpermission_options.py
+-rw-r--r--   0        0        0      434 2023-04-22 17:57:27.834494 django_object_safety-0.2.0/safety/migrations/0007_alter_objectpermission_options.py
+-rw-r--r--   0        0        0      571 2023-04-22 17:57:27.834494 django_object_safety-0.2.0/safety/migrations/0008_rename_permissiongroup_objectgroup.py
+-rw-r--r--   0        0        0        0 2023-04-16 19:30:41.012284 django_object_safety-0.2.0/safety/migrations/__init__.py
+-rw-r--r--   0        0        0     2461 2023-04-22 17:57:27.834494 django_object_safety-0.2.0/safety/models.py
+-rw-r--r--   0        0        0    12344 2023-04-23 14:45:56.144510 django_object_safety-0.2.0/safety/shortcuts.py
+-rw-r--r--   0        0        0     6153 2023-04-23 14:45:56.136510 django_object_safety-0.2.0/safety/tests.py
+-rw-r--r--   0        0        0       63 2023-04-16 18:28:46.023260 django_object_safety-0.2.0/safety/views.py
+-rw-r--r--   0        0        0      819 1970-01-01 00:00:00.000000 django_object_safety-0.2.0/PKG-INFO
```

### Comparing `django_object_safety-0.1.4/LICENSE` & `django_object_safety-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_object_safety-0.1.4/pyproject.toml` & `django_object_safety-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-object-safety"
-version = "0.1.4"
+version = "0.2.0"
 description = "Adds object permissions to Django."
 license = "MIT"
 authors = ["William Ferreira"]
 homepage = "https://django-object-safety-docs.readthedocs.io/"
 repository = "https://github.com/williammferreira/django-object-safety/"
 keywords = ["django", "permissions", "object-permissions", "django-permissions", "django-object-permissions"]
 readme = "README.md"
```

### Comparing `django_object_safety-0.1.4/safety/migrations/0001_initial.py` & `django_object_safety-0.2.0/safety/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-0.1.4/safety/migrations/0002_alter_objectpermission_object_ct_and_more.py` & `django_object_safety-0.2.0/safety/migrations/0002_alter_objectpermission_object_ct_and_more.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-0.1.4/safety/migrations/0004_alter_objectpermission_unique_together_and_more.py` & `django_object_safety-0.2.0/safety/migrations/0004_alter_objectpermission_unique_together_and_more.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-0.1.4/safety/migrations/0005_alter_permissiongroup_target_id_and_more.py` & `django_object_safety-0.2.0/safety/migrations/0005_alter_permissiongroup_target_id_and_more.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-0.1.4/safety/migrations/0008_rename_permissiongroup_objectgroup.py` & `django_object_safety-0.2.0/safety/migrations/0008_rename_permissiongroup_objectgroup.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-0.1.4/safety/models.py` & `django_object_safety-0.2.0/safety/models.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-0.1.4/safety/shortcuts.py` & `django_object_safety-0.2.0/safety/shortcuts.py`

 * *Files 4% similar despite different names*

```diff
@@ -236,17 +236,17 @@
         Group: The group object.
     """
 
     return get_object_group_model().objects.get(name=name, target_id=obj.id,
                                                 target_ct=ContentType.objects.get_for_model(obj))
 
 
-def create_perm_group(name: str, permissions: list[str], obj) -> ObjectGroup:
+def create_object_group(name: str, permissions: list[str], obj) -> ObjectGroup:
     """
-    Create a permission group.
+    Create a object group.
 
     Args:
         name (string): The name of the group.
         permissions: The permissions to add to the group.
         obj: The object to add the group to.
 
     Returns:
@@ -258,17 +258,17 @@
 
     for permission in permissions:
         perm_group.permissions.add(Permission.objects.get(codename=permission))
 
     return perm_group
 
 
-def delete_perm_group(name: str, obj) -> bool:
+def delete_object_group(name: str, obj) -> bool:
     """
-    Remove a permission group.
+    Remove a object group.
 
     Args:
         name (string): The name of the group.
         obj: The object to remove the group from.
 
     Returns:
         bool: True if the group was removed, otherwise False.
@@ -279,17 +279,17 @@
     if not group.exists():
         return False
 
     group.delete()
     return True
 
 
-def add_user_to_perm_group(user: get_user_model(), name: str, obj) -> bool:
+def add_user_to_object_group(user: get_user_model(), name: str, obj) -> bool:
     """
-    Add a user to a permission group.
+    Add a user to a object group.
 
     Args:
         user: The user to add to the group.
         name: The name of the perm group.
         obj: The object for the perm group.
 
     Returns:
@@ -297,17 +297,17 @@
     """
 
     get_object_group_model().objects.get(name=name, target_id=obj.id,
                                          target_ct=ContentType.objects.get_for_model(obj)).users.add(user)
     return True
 
 
-def remove_user_from_perm_group(user: get_user_model(), name: str, obj) -> bool:
+def remove_user_from_object_group(user: get_user_model(), name: str, obj) -> bool:
     """
-    Remove a user from a permission group.
+    Remove a user from a object group.
 
     Args:
         user: The user to remove from the group.
         name: The name of the perm group.
         obj: The object of the perm group.
 
     Returns:
```

### Comparing `django_object_safety-0.1.4/safety/tests.py` & `django_object_safety-0.2.0/safety/tests.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from django.contrib.auth import get_user_model
 from django.contrib.auth.models import Group, Permission
 from django.contrib.contenttypes.models import ContentType
 from django.db import models
 from django.test import TransactionTestCase
 from django_fake_model import models as f
 
-from safety.shortcuts import set_perm, has_perm, lift_perm, create_perm_group, delete_perm_group, \
-    add_user_to_perm_group, remove_user_from_perm_group
+from safety.shortcuts import set_perm, has_perm, lift_perm, create_object_group, delete_object_group, \
+    add_user_to_object_group, remove_user_from_object_group
 
 
 class FakePost(f.FakeModel):
     title = models.CharField(max_length=100)
     content = models.TextField()
 
     class Meta:
@@ -101,46 +101,46 @@
         self.posts.append(FakePost.objects.create(title="TestPost2", content="TestContent2"))
 
         FakePost.set_django_objects()
 
         self.fake_post_ct = ContentType.objects.get_for_model(FakePost)
 
     def test_create_permission_group(self):
-        create_perm_group("editors",
-                          ["view_fakepost", "change_fakepost", "delete_fakepost"],
-                          self.posts[0])
-        add_user_to_perm_group(self.users[0], "editors", self.posts[0])
+        create_object_group("editors",
+                            ["view_fakepost", "change_fakepost", "delete_fakepost"],
+                            self.posts[0])
+        add_user_to_object_group(self.users[0], "editors", self.posts[0])
 
         self.assertTrue(has_perm([self.users[0]], "change_fakepost", self.posts[0]))
 
     def test_delete_permission_group(self):
-        create_perm_group("editors",
-                          ["view_fakepost", "change_fakepost", "delete_fakepost"],
-                          self.posts[0])
+        create_object_group("editors",
+                            ["view_fakepost", "change_fakepost", "delete_fakepost"],
+                            self.posts[0])
 
-        delete_perm_group("editors", self.posts[0])
+        delete_object_group("editors", self.posts[0])
 
         self.assertFalse(has_perm([self.users[0]], "change_fakepost", self.posts[0]))
 
     def test_remove_user_from_permission_group(self):
-        create_perm_group("editors",
-                          ["view_fakepost", "change_fakepost", "delete_fakepost"],
-                          self.posts[0])
+        create_object_group("editors",
+                            ["view_fakepost", "change_fakepost", "delete_fakepost"],
+                            self.posts[0])
 
-        add_user_to_perm_group(self.users[0], "editors", self.posts[0])
+        add_user_to_object_group(self.users[0], "editors", self.posts[0])
 
-        remove_user_from_perm_group(self.users[0], "editors", self.posts[0])
+        remove_user_from_object_group(self.users[0], "editors", self.posts[0])
 
         self.assertFalse(has_perm([self.users[0]], "change_fakepost", self.posts[0]))
 
     def test_remove_permission_on_delete(self):
-        create_perm_group("editors",
-                          ["view_fakepost", "change_fakepost", "delete_fakepost"],
-                          self.posts[0])
+        create_object_group("editors",
+                            ["view_fakepost", "change_fakepost", "delete_fakepost"],
+                            self.posts[0])
 
-        add_user_to_perm_group(self.users[0], "editors", self.posts[0])
+        add_user_to_object_group(self.users[0], "editors", self.posts[0])
 
         post = self.posts[0]
 
         self.posts[0].delete()
 
         self.assertFalse(has_perm([self.users[0]], "change_fakepost", post))
```

### Comparing `django_object_safety-0.1.4/PKG-INFO` & `django_object_safety-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-object-safety
-Version: 0.1.4
+Version: 0.2.0
 Summary: Adds object permissions to Django.
 Home-page: https://django-object-safety-docs.readthedocs.io/
 License: MIT
 Keywords: django,permissions,object-permissions,django-permissions,django-object-permissions
 Author: William Ferreira
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

