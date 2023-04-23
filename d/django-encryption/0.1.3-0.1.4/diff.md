# Comparing `tmp/django_encryption-0.1.3.tar.gz` & `tmp/django_encryption-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_encryption-0.1.3.tar", max compression
+gzip compressed data, was "django_encryption-0.1.4.tar", max compression
```

## Comparing `django_encryption-0.1.3.tar` & `django_encryption-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     5637 2023-03-30 06:23:36.786198 django_encryption-0.1.3/README.md
--rw-r--r--   0        0        0       22 2023-03-30 06:23:36.786198 django_encryption-0.1.3/django_encryption/__init__.py
--rw-r--r--   0        0        0     8175 2023-03-30 06:23:36.790199 django_encryption-0.1.3/django_encryption/fields.py
--rw-r--r--   0        0        0        0 2023-03-30 06:23:36.790199 django_encryption-0.1.3/django_encryption/management/__init__.py
--rw-r--r--   0        0        0        0 2023-03-30 06:23:36.790199 django_encryption-0.1.3/django_encryption/management/commands/__init__.py
--rw-r--r--   0        0        0     3249 2023-03-30 06:23:36.790199 django_encryption-0.1.3/django_encryption/management/commands/generate_vault_migration.py
--rw-r--r--   0        0        0        0 2023-03-30 06:23:36.790199 django_encryption-0.1.3/django_encryption/py.typed
--rw-r--r--   0        0        0    11063 2023-03-30 06:23:36.790199 django_encryption-0.1.3/django_encryption/vault_wrapper.py
--rw-r--r--   0        0        0     2159 2023-03-30 06:23:50.386397 django_encryption-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     7429 1970-01-01 00:00:00.000000 django_encryption-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     5637 2023-04-23 13:03:34.891594 django_encryption-0.1.4/README.md
+-rw-r--r--   0        0        0       22 2023-04-23 13:03:34.891594 django_encryption-0.1.4/django_encryption/__init__.py
+-rw-r--r--   0        0        0     8175 2023-04-23 13:03:34.891594 django_encryption-0.1.4/django_encryption/fields.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:03:34.891594 django_encryption-0.1.4/django_encryption/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:03:34.891594 django_encryption-0.1.4/django_encryption/management/commands/__init__.py
+-rw-r--r--   0        0        0     3249 2023-04-23 13:03:34.891594 django_encryption-0.1.4/django_encryption/management/commands/generate_vault_migration.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:03:34.891594 django_encryption-0.1.4/django_encryption/py.typed
+-rw-r--r--   0        0        0    11063 2023-04-23 13:03:34.891594 django_encryption-0.1.4/django_encryption/vault_wrapper.py
+-rw-r--r--   0        0        0     2159 2023-04-23 13:04:13.479470 django_encryption-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     7429 1970-01-01 00:00:00.000000 django_encryption-0.1.4/PKG-INFO
```

### Comparing `django_encryption-0.1.3/README.md` & `django_encryption-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `django_encryption-0.1.3/django_encryption/fields.py` & `django_encryption-0.1.4/django_encryption/fields.py`

 * *Files identical despite different names*

### Comparing `django_encryption-0.1.3/django_encryption/management/commands/generate_vault_migration.py` & `django_encryption-0.1.4/django_encryption/management/commands/generate_vault_migration.py`

 * *Files identical despite different names*

### Comparing `django_encryption-0.1.3/django_encryption/vault_wrapper.py` & `django_encryption-0.1.4/django_encryption/vault_wrapper.py`

 * *Files identical despite different names*

### Comparing `django_encryption-0.1.3/pyproject.toml` & `django_encryption-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-encryption"
-version = "0.1.3"
+version = "0.1.4"
 description = "A set of fields that wrap standard Django fields with encryption provided Piiano Vault."
 authors = ["Imri Goldberg <imri.goldberg@piiano.com>"]
 license = "MIT"
 packages = [ { include = "django_encryption" } ]
 readme = "README.md"
 repository = "https://github.com/piiano/vault-python"
 keywords = [ "encryption", "django", "fields" ]
```

### Comparing `django_encryption-0.1.3/PKG-INFO` & `django_encryption-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-encryption
-Version: 0.1.3
+Version: 0.1.4
 Summary: A set of fields that wrap standard Django fields with encryption provided Piiano Vault.
 Home-page: https://github.com/piiano/vault-python
 License: MIT
 Keywords: encryption,django,fields
 Author: Imri Goldberg
 Author-email: imri.goldberg@piiano.com
 Requires-Python: >=3.8,<4.0
```

