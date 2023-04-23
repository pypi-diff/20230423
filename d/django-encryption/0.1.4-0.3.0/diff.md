# Comparing `tmp/django_encryption-0.1.4.tar.gz` & `tmp/django_encryption-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_encryption-0.1.4.tar", max compression
+gzip compressed data, was "django_encryption-0.3.0.tar", max compression
```

## Comparing `django_encryption-0.1.4.tar` & `django_encryption-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     5637 2023-04-23 13:03:34.891594 django_encryption-0.1.4/README.md
--rw-r--r--   0        0        0       22 2023-04-23 13:03:34.891594 django_encryption-0.1.4/django_encryption/__init__.py
--rw-r--r--   0        0        0     8175 2023-04-23 13:03:34.891594 django_encryption-0.1.4/django_encryption/fields.py
--rw-r--r--   0        0        0        0 2023-04-23 13:03:34.891594 django_encryption-0.1.4/django_encryption/management/__init__.py
--rw-r--r--   0        0        0        0 2023-04-23 13:03:34.891594 django_encryption-0.1.4/django_encryption/management/commands/__init__.py
--rw-r--r--   0        0        0     3249 2023-04-23 13:03:34.891594 django_encryption-0.1.4/django_encryption/management/commands/generate_vault_migration.py
--rw-r--r--   0        0        0        0 2023-04-23 13:03:34.891594 django_encryption-0.1.4/django_encryption/py.typed
--rw-r--r--   0        0        0    11063 2023-04-23 13:03:34.891594 django_encryption-0.1.4/django_encryption/vault_wrapper.py
--rw-r--r--   0        0        0     2159 2023-04-23 13:04:13.479470 django_encryption-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     7429 1970-01-01 00:00:00.000000 django_encryption-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     6084 2023-04-23 13:47:23.036030 django_encryption-0.3.0/README.md
+-rw-r--r--   0        0        0       22 2023-04-23 13:47:23.036030 django_encryption-0.3.0/django_encryption/__init__.py
+-rw-r--r--   0        0        0    15879 2023-04-23 13:47:23.036030 django_encryption-0.3.0/django_encryption/fields.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:47:23.036030 django_encryption-0.3.0/django_encryption/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:47:23.036030 django_encryption-0.3.0/django_encryption/management/commands/__init__.py
+-rw-r--r--   0        0        0     3278 2023-04-23 13:47:23.036030 django_encryption-0.3.0/django_encryption/management/commands/generate_vault_migration.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:47:23.036030 django_encryption-0.3.0/django_encryption/py.typed
+-rw-r--r--   0        0        0    11063 2023-04-23 13:47:23.036030 django_encryption-0.3.0/django_encryption/vault_wrapper.py
+-rw-r--r--   0        0        0     2159 2023-04-23 13:47:49.040706 django_encryption-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7876 1970-01-01 00:00:00.000000 django_encryption-0.3.0/PKG-INFO
```

### Comparing `django_encryption-0.1.4/README.md` & `django_encryption-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -52,22 +52,24 @@
    You can customize the field by providing additional parameters such as:
 
    - `encryption_type` (**optional**) - Can be `EncryptionType.randomized` or `EncryptionType.deterministic`
    - `expiration_secs` (**optional**) - An integer or None. If an integer, the number of seconds before the encrypted data is expired, and cannot be decrypted anymore. Works only with randomized `encryption_type`
    - `vault_collection` (**optional**) - The name of the vault collection that this field is related to. Defaults to `settings.VAULT_DEFAULT_COLLECTION`
    - `vault_property` (**optional**) - The name of the property in the vault collection that this field is related to. Defaults to the name of the field in django.
    - `data_type_name` (**optional**) - The name of the data type in vault. Defaults to 'string'. This only has impact when generating a vault migration, and does not change the way your django model would behave.
+   - `eager` (default: **true**) - whether or not value will be decrypted (in a batch operation) as soon as it is fetched from the DB. If not, the value will be decrypted the first time it is accessed.
 
    **Note**: use `vault_collection` together with `vault_property` to specify the collection and property in vault that represent this field. This is important for permission control and audit logs. For more advanced use-cases, this would allow you to transition smoothly to using Vault as a secure storage for PII data.
 
-Query your model as usual:
+Query your model as usual, keeping the following in mind:
 
-- Caveat: right now, an API call to vault will be generated for each field in each Model instance you encrypt or decrypt. In the future this will be batched.
+* Read queries are batched. Reading from the Database will generate a single API call per field. Writing to the Database is not batched and will generate an API call for each field in each instance.
+* By default all fields are eagerly fetched - similarly to calling prefetch_related(field_name) on a foreign key.
 
-You can wrap your queries with: `with fields.mask_field(MyModel.my_field):` (or `transform` or `with_reason`):
+The SDK also supports masking and other vault transformations by using mask(MyModel.my_field) or transform('transformation-name', MyModel.my_field) as part of the query.
 
 - This tells the encryption SDK to mask the values of MyModel.my_field. So for example, for an SSN you would get "**\*-**-6789".
 - All vault's supported transformations are also supported using the `transform` context manager. See [Built-in transformations](https://piiano.com/docs/guides/manage-transformations/built-in-transformations) in Vault's API documentation for a list of Vault's supported transformations.
 
 ## Sample code
 
 ```
```

### Comparing `django_encryption-0.1.4/django_encryption/management/commands/generate_vault_migration.py` & `django_encryption-0.3.0/django_encryption/management/commands/generate_vault_migration.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,16 @@
 
 
 TEMPLATE = """
 import os
 from typing import Dict, List
 
 os.environ.setdefault("DJANGO_SETTINGS_MODULE", "__PROJECT_NAME__.settings")
+import django
+django.setup()
 
 from django_encryption.fields import VaultException, get_vault # noqa
 
 
 COLLECTION_TO_FIELDS: Dict[str, List[str]] = __COLLECTION_TO_FIELDS__
```

### Comparing `django_encryption-0.1.4/django_encryption/vault_wrapper.py` & `django_encryption-0.3.0/django_encryption/vault_wrapper.py`

 * *Files identical despite different names*

### Comparing `django_encryption-0.1.4/pyproject.toml` & `django_encryption-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-encryption"
-version = "0.1.4"
+version = "0.3.0"
 description = "A set of fields that wrap standard Django fields with encryption provided Piiano Vault."
 authors = ["Imri Goldberg <imri.goldberg@piiano.com>"]
 license = "MIT"
 packages = [ { include = "django_encryption" } ]
 readme = "README.md"
 repository = "https://github.com/piiano/vault-python"
 keywords = [ "encryption", "django", "fields" ]
@@ -51,16 +51,16 @@
 pytest = "^7.2.2"
 mock = "^4.0.3"
 pycodestyle = "^2.8.0"
 types-mock = "^5.0.0.5"
 ipython = "^8.11.0"
 isort = "^5.12.0"
 black = "^23.1.0"
-django-coverage = "^1.2.4"
 tox = "^4.4.7"
+django-coverage = "^1.2.4"
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.tox]
```

### Comparing `django_encryption-0.1.4/PKG-INFO` & `django_encryption-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-encryption
-Version: 0.1.4
+Version: 0.3.0
 Summary: A set of fields that wrap standard Django fields with encryption provided Piiano Vault.
 Home-page: https://github.com/piiano/vault-python
 License: MIT
 Keywords: encryption,django,fields
 Author: Imri Goldberg
 Author-email: imri.goldberg@piiano.com
 Requires-Python: >=3.8,<4.0
@@ -95,22 +95,24 @@
    You can customize the field by providing additional parameters such as:
 
    - `encryption_type` (**optional**) - Can be `EncryptionType.randomized` or `EncryptionType.deterministic`
    - `expiration_secs` (**optional**) - An integer or None. If an integer, the number of seconds before the encrypted data is expired, and cannot be decrypted anymore. Works only with randomized `encryption_type`
    - `vault_collection` (**optional**) - The name of the vault collection that this field is related to. Defaults to `settings.VAULT_DEFAULT_COLLECTION`
    - `vault_property` (**optional**) - The name of the property in the vault collection that this field is related to. Defaults to the name of the field in django.
    - `data_type_name` (**optional**) - The name of the data type in vault. Defaults to 'string'. This only has impact when generating a vault migration, and does not change the way your django model would behave.
+   - `eager` (default: **true**) - whether or not value will be decrypted (in a batch operation) as soon as it is fetched from the DB. If not, the value will be decrypted the first time it is accessed.
 
    **Note**: use `vault_collection` together with `vault_property` to specify the collection and property in vault that represent this field. This is important for permission control and audit logs. For more advanced use-cases, this would allow you to transition smoothly to using Vault as a secure storage for PII data.
 
-Query your model as usual:
+Query your model as usual, keeping the following in mind:
 
-- Caveat: right now, an API call to vault will be generated for each field in each Model instance you encrypt or decrypt. In the future this will be batched.
+* Read queries are batched. Reading from the Database will generate a single API call per field. Writing to the Database is not batched and will generate an API call for each field in each instance.
+* By default all fields are eagerly fetched - similarly to calling prefetch_related(field_name) on a foreign key.
 
-You can wrap your queries with: `with fields.mask_field(MyModel.my_field):` (or `transform` or `with_reason`):
+The SDK also supports masking and other vault transformations by using mask(MyModel.my_field) or transform('transformation-name', MyModel.my_field) as part of the query.
 
 - This tells the encryption SDK to mask the values of MyModel.my_field. So for example, for an SSN you would get "**\*-**-6789".
 - All vault's supported transformations are also supported using the `transform` context manager. See [Built-in transformations](https://piiano.com/docs/guides/manage-transformations/built-in-transformations) in Vault's API documentation for a list of Vault's supported transformations.
 
 ## Sample code
 
 ```
```

