# Comparing `tmp/django_salted_api_tokens-1.0.2.tar.gz` & `tmp/django_salted_api_tokens-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_salted_api_tokens-1.0.2.tar", last modified: Sat Apr  8 23:35:18 2023, max compression
+gzip compressed data, was "django_salted_api_tokens-1.0.3.tar", last modified: Sun Apr 23 03:54:34 2023, max compression
```

## Comparing `django_salted_api_tokens-1.0.2.tar` & `django_salted_api_tokens-1.0.3.tar`

### file list

```diff
@@ -1,49 +1,55 @@
-drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-04-08 23:35:18.155975 django_salted_api_tokens-1.0.2/
--rw-r--r--   0 topcat    (1000) topcat    (1000)    11358 2023-04-03 01:47:41.000000 django_salted_api_tokens-1.0.2/LICENSE
--rw-r--r--   0 topcat    (1000) topcat    (1000)     3250 2023-04-08 23:35:18.155975 django_salted_api_tokens-1.0.2/PKG-INFO
--rw-r--r--   0 topcat    (1000) topcat    (1000)     2708 2023-04-08 07:03:58.000000 django_salted_api_tokens-1.0.2/README.md
--rw-r--r--   0 topcat    (1000) topcat    (1000)      717 2023-04-08 06:59:21.000000 django_salted_api_tokens-1.0.2/pyproject.toml
--rw-r--r--   0 topcat    (1000) topcat    (1000)       38 2023-04-08 23:35:18.155975 django_salted_api_tokens-1.0.2/setup.cfg
-drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-04-08 23:35:18.147975 django_salted_api_tokens-1.0.2/src/
-drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-04-08 23:35:18.151975 django_salted_api_tokens-1.0.2/src/django_salted_api_tokens/
--rw-r--r--   0 topcat    (1000) topcat    (1000)       52 2023-04-08 06:59:21.000000 django_salted_api_tokens-1.0.2/src/django_salted_api_tokens/__init__.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)      766 2023-04-06 07:23:04.000000 django_salted_api_tokens-1.0.2/src/django_salted_api_tokens/admin.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)     1658 2023-04-06 07:23:04.000000 django_salted_api_tokens-1.0.2/src/django_salted_api_tokens/authentication.py
-drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-04-08 23:35:18.151975 django_salted_api_tokens-1.0.2/src/django_salted_api_tokens/migrations/
--rw-r--r--   0 topcat    (1000) topcat    (1000)     1598 2023-04-06 07:23:04.000000 django_salted_api_tokens-1.0.2/src/django_salted_api_tokens/migrations/0001_initial.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)        0 2023-04-06 07:23:04.000000 django_salted_api_tokens-1.0.2/src/django_salted_api_tokens/migrations/__init__.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)      928 2023-04-06 07:23:04.000000 django_salted_api_tokens-1.0.2/src/django_salted_api_tokens/models.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)      484 2023-04-08 06:55:11.000000 django_salted_api_tokens-1.0.2/src/django_salted_api_tokens/serializers.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)      426 2023-04-08 23:24:30.000000 django_salted_api_tokens-1.0.2/src/django_salted_api_tokens/settings.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)      293 2023-04-06 07:23:04.000000 django_salted_api_tokens-1.0.2/src/django_salted_api_tokens/urls.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)      789 2023-04-08 06:55:11.000000 django_salted_api_tokens-1.0.2/src/django_salted_api_tokens/utils.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)     1410 2023-04-08 06:55:11.000000 django_salted_api_tokens-1.0.2/src/django_salted_api_tokens/views.py
-drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-04-08 23:35:18.151975 django_salted_api_tokens-1.0.2/src/django_salted_api_tokens.egg-info/
--rw-r--r--   0 topcat    (1000) topcat    (1000)     3250 2023-04-08 23:35:18.000000 django_salted_api_tokens-1.0.2/src/django_salted_api_tokens.egg-info/PKG-INFO
--rw-r--r--   0 topcat    (1000) topcat    (1000)     1592 2023-04-08 23:35:18.000000 django_salted_api_tokens-1.0.2/src/django_salted_api_tokens.egg-info/SOURCES.txt
--rw-r--r--   0 topcat    (1000) topcat    (1000)        1 2023-04-08 23:35:18.000000 django_salted_api_tokens-1.0.2/src/django_salted_api_tokens.egg-info/dependency_links.txt
--rw-r--r--   0 topcat    (1000) topcat    (1000)       54 2023-04-08 23:35:18.000000 django_salted_api_tokens-1.0.2/src/django_salted_api_tokens.egg-info/requires.txt
--rw-r--r--   0 topcat    (1000) topcat    (1000)       54 2023-04-08 23:35:18.000000 django_salted_api_tokens-1.0.2/src/django_salted_api_tokens.egg-info/top_level.txt
-drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-04-08 23:35:18.151975 django_salted_api_tokens-1.0.2/src/example_django_project/
--rw-r--r--   0 topcat    (1000) topcat    (1000)        0 2023-04-06 07:23:04.000000 django_salted_api_tokens-1.0.2/src/example_django_project/__init__.py
-drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-04-08 23:35:18.155975 django_salted_api_tokens-1.0.2/src/example_django_project/accounts/
--rw-r--r--   0 topcat    (1000) topcat    (1000)        0 2023-04-06 07:23:04.000000 django_salted_api_tokens-1.0.2/src/example_django_project/accounts/__init__.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)       63 2023-04-06 07:23:04.000000 django_salted_api_tokens-1.0.2/src/example_django_project/accounts/admin.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)      148 2023-04-06 07:23:04.000000 django_salted_api_tokens-1.0.2/src/example_django_project/accounts/apps.py
-drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-04-08 23:35:18.155975 django_salted_api_tokens-1.0.2/src/example_django_project/accounts/migrations/
--rw-r--r--   0 topcat    (1000) topcat    (1000)        0 2023-04-06 07:23:04.000000 django_salted_api_tokens-1.0.2/src/example_django_project/accounts/migrations/__init__.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)       57 2023-04-06 07:23:04.000000 django_salted_api_tokens-1.0.2/src/example_django_project/accounts/models.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)       60 2023-04-06 07:23:04.000000 django_salted_api_tokens-1.0.2/src/example_django_project/accounts/tests.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)      266 2023-04-06 07:23:04.000000 django_salted_api_tokens-1.0.2/src/example_django_project/accounts/urls.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)      232 2023-04-06 07:23:04.000000 django_salted_api_tokens-1.0.2/src/example_django_project/accounts/views.py
-drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-04-08 23:35:18.155975 django_salted_api_tokens-1.0.2/src/example_django_project/example_django_project/
--rw-r--r--   0 topcat    (1000) topcat    (1000)        0 2023-04-06 07:23:04.000000 django_salted_api_tokens-1.0.2/src/example_django_project/example_django_project/__init__.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)     3870 2023-04-08 23:33:50.000000 django_salted_api_tokens-1.0.2/src/example_django_project/example_django_project/settings.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)      950 2023-04-06 07:23:04.000000 django_salted_api_tokens-1.0.2/src/example_django_project/example_django_project/urls.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)      421 2023-04-06 07:23:04.000000 django_salted_api_tokens-1.0.2/src/example_django_project/example_django_project/wsgi.py
--rwxr-xr-x   0 topcat    (1000) topcat    (1000)      678 2023-04-06 07:23:04.000000 django_salted_api_tokens-1.0.2/src/example_django_project/manage.py
-drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-04-08 23:35:18.155975 django_salted_api_tokens-1.0.2/src/tests/
--rw-r--r--   0 topcat    (1000) topcat    (1000)        0 2023-04-06 07:23:04.000000 django_salted_api_tokens-1.0.2/src/tests/__init__.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)     1428 2023-04-08 06:55:11.000000 django_salted_api_tokens-1.0.2/src/tests/factories.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)     5113 2023-04-08 06:55:11.000000 django_salted_api_tokens-1.0.2/src/tests/test_authentication_api_key_secret.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)     2083 2023-04-08 06:55:11.000000 django_salted_api_tokens-1.0.2/src/tests/test_view_create_api_key_secret.py
+drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-04-23 03:54:34.467968 django_salted_api_tokens-1.0.3/
+-rw-r--r--   0 topcat    (1000) topcat    (1000)    11358 2023-04-03 01:47:41.000000 django_salted_api_tokens-1.0.3/LICENSE
+-rw-r--r--   0 topcat    (1000) topcat    (1000)     3249 2023-04-23 03:54:34.467968 django_salted_api_tokens-1.0.3/PKG-INFO
+-rw-r--r--   0 topcat    (1000) topcat    (1000)     2707 2023-04-23 03:51:19.000000 django_salted_api_tokens-1.0.3/README.md
+-rw-r--r--   0 topcat    (1000) topcat    (1000)      717 2023-04-23 03:50:17.000000 django_salted_api_tokens-1.0.3/pyproject.toml
+-rw-r--r--   0 topcat    (1000) topcat    (1000)       38 2023-04-23 03:54:34.467968 django_salted_api_tokens-1.0.3/setup.cfg
+drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-04-23 03:54:34.459968 django_salted_api_tokens-1.0.3/src/
+drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-04-23 03:54:34.459968 django_salted_api_tokens-1.0.3/src/django_salted_api_tokens/
+-rw-r--r--   0 topcat    (1000) topcat    (1000)       52 2023-04-23 03:50:17.000000 django_salted_api_tokens-1.0.3/src/django_salted_api_tokens/__init__.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)      766 2023-04-06 07:23:04.000000 django_salted_api_tokens-1.0.3/src/django_salted_api_tokens/admin.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)     1658 2023-04-06 07:23:04.000000 django_salted_api_tokens-1.0.3/src/django_salted_api_tokens/authentication.py
+drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-04-23 03:54:34.463968 django_salted_api_tokens-1.0.3/src/django_salted_api_tokens/management/
+-rw-r--r--   0 topcat    (1000) topcat    (1000)        0 2023-04-23 03:50:17.000000 django_salted_api_tokens-1.0.3/src/django_salted_api_tokens/management/__init__.py
+drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-04-23 03:54:34.463968 django_salted_api_tokens-1.0.3/src/django_salted_api_tokens/management/commands/
+-rw-r--r--   0 topcat    (1000) topcat    (1000)        0 2023-04-23 03:50:17.000000 django_salted_api_tokens-1.0.3/src/django_salted_api_tokens/management/commands/__init__.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)     1255 2023-04-23 03:50:17.000000 django_salted_api_tokens-1.0.3/src/django_salted_api_tokens/management/commands/create_dsat_for_user.py
+drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-04-23 03:54:34.463968 django_salted_api_tokens-1.0.3/src/django_salted_api_tokens/migrations/
+-rw-r--r--   0 topcat    (1000) topcat    (1000)     1598 2023-04-06 07:23:04.000000 django_salted_api_tokens-1.0.3/src/django_salted_api_tokens/migrations/0001_initial.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)        0 2023-04-06 07:23:04.000000 django_salted_api_tokens-1.0.3/src/django_salted_api_tokens/migrations/__init__.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)      928 2023-04-06 07:23:04.000000 django_salted_api_tokens-1.0.3/src/django_salted_api_tokens/models.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)      484 2023-04-23 01:05:32.000000 django_salted_api_tokens-1.0.3/src/django_salted_api_tokens/serializers.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)      426 2023-04-23 01:05:42.000000 django_salted_api_tokens-1.0.3/src/django_salted_api_tokens/settings.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)      293 2023-04-06 07:23:04.000000 django_salted_api_tokens-1.0.3/src/django_salted_api_tokens/urls.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)     1571 2023-04-23 03:50:17.000000 django_salted_api_tokens-1.0.3/src/django_salted_api_tokens/utils.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)      772 2023-04-23 03:50:17.000000 django_salted_api_tokens-1.0.3/src/django_salted_api_tokens/views.py
+drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-04-23 03:54:34.463968 django_salted_api_tokens-1.0.3/src/django_salted_api_tokens.egg-info/
+-rw-r--r--   0 topcat    (1000) topcat    (1000)     3249 2023-04-23 03:54:34.000000 django_salted_api_tokens-1.0.3/src/django_salted_api_tokens.egg-info/PKG-INFO
+-rw-r--r--   0 topcat    (1000) topcat    (1000)     1826 2023-04-23 03:54:34.000000 django_salted_api_tokens-1.0.3/src/django_salted_api_tokens.egg-info/SOURCES.txt
+-rw-r--r--   0 topcat    (1000) topcat    (1000)        1 2023-04-23 03:54:34.000000 django_salted_api_tokens-1.0.3/src/django_salted_api_tokens.egg-info/dependency_links.txt
+-rw-r--r--   0 topcat    (1000) topcat    (1000)       54 2023-04-23 03:54:34.000000 django_salted_api_tokens-1.0.3/src/django_salted_api_tokens.egg-info/requires.txt
+-rw-r--r--   0 topcat    (1000) topcat    (1000)       54 2023-04-23 03:54:34.000000 django_salted_api_tokens-1.0.3/src/django_salted_api_tokens.egg-info/top_level.txt
+drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-04-23 03:54:34.463968 django_salted_api_tokens-1.0.3/src/example_django_project/
+-rw-r--r--   0 topcat    (1000) topcat    (1000)        0 2023-04-06 07:23:04.000000 django_salted_api_tokens-1.0.3/src/example_django_project/__init__.py
+drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-04-23 03:54:34.463968 django_salted_api_tokens-1.0.3/src/example_django_project/accounts/
+-rw-r--r--   0 topcat    (1000) topcat    (1000)        0 2023-04-06 07:23:04.000000 django_salted_api_tokens-1.0.3/src/example_django_project/accounts/__init__.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)       63 2023-04-06 07:23:04.000000 django_salted_api_tokens-1.0.3/src/example_django_project/accounts/admin.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)      148 2023-04-06 07:23:04.000000 django_salted_api_tokens-1.0.3/src/example_django_project/accounts/apps.py
+drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-04-23 03:54:34.463968 django_salted_api_tokens-1.0.3/src/example_django_project/accounts/migrations/
+-rw-r--r--   0 topcat    (1000) topcat    (1000)        0 2023-04-06 07:23:04.000000 django_salted_api_tokens-1.0.3/src/example_django_project/accounts/migrations/__init__.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)       57 2023-04-06 07:23:04.000000 django_salted_api_tokens-1.0.3/src/example_django_project/accounts/models.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)       60 2023-04-06 07:23:04.000000 django_salted_api_tokens-1.0.3/src/example_django_project/accounts/tests.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)      266 2023-04-06 07:23:04.000000 django_salted_api_tokens-1.0.3/src/example_django_project/accounts/urls.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)      232 2023-04-06 07:23:04.000000 django_salted_api_tokens-1.0.3/src/example_django_project/accounts/views.py
+drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-04-23 03:54:34.463968 django_salted_api_tokens-1.0.3/src/example_django_project/example_django_project/
+-rw-r--r--   0 topcat    (1000) topcat    (1000)        0 2023-04-06 07:23:04.000000 django_salted_api_tokens-1.0.3/src/example_django_project/example_django_project/__init__.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)     3870 2023-04-08 23:33:50.000000 django_salted_api_tokens-1.0.3/src/example_django_project/example_django_project/settings.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)      950 2023-04-06 07:23:04.000000 django_salted_api_tokens-1.0.3/src/example_django_project/example_django_project/urls.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)      421 2023-04-06 07:23:04.000000 django_salted_api_tokens-1.0.3/src/example_django_project/example_django_project/wsgi.py
+-rwxr-xr-x   0 topcat    (1000) topcat    (1000)      678 2023-04-06 07:23:04.000000 django_salted_api_tokens-1.0.3/src/example_django_project/manage.py
+drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-04-23 03:54:34.463968 django_salted_api_tokens-1.0.3/src/tests/
+-rw-r--r--   0 topcat    (1000) topcat    (1000)        0 2023-04-06 07:23:04.000000 django_salted_api_tokens-1.0.3/src/tests/__init__.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)     1428 2023-04-08 06:55:11.000000 django_salted_api_tokens-1.0.3/src/tests/factories.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)     5113 2023-04-08 06:55:11.000000 django_salted_api_tokens-1.0.3/src/tests/test_authentication_api_key_secret.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)     1531 2023-04-23 03:50:17.000000 django_salted_api_tokens-1.0.3/src/tests/test_mgmt_cmd_create_dsat_for_user.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)     1931 2023-04-23 03:50:17.000000 django_salted_api_tokens-1.0.3/src/tests/test_view_create_api_key_secret.py
```

### Comparing `django_salted_api_tokens-1.0.2/LICENSE` & `django_salted_api_tokens-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_salted_api_tokens-1.0.2/PKG-INFO` & `django_salted_api_tokens-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_salted_api_tokens
-Version: 1.0.2
+Version: 1.0.3
 Summary: Django token authentication with hashed, salted tokens
 Author-email: Harisankar Krishna Swamy <harisankar.krishna@outlook.com>
 Project-URL: Homepage, https://github.com/harisankar-krishna-swamy/django_salted_api_tokens
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9.2
@@ -26,17 +26,17 @@
 # 3. Configuration
 * Add `DSAT_TOKEN_LENGTH` in `settings.py`  
   Default: `80` Max length: `256`  
 * Add `DSAT_MAX_TOKENS_PER_USER`  in `settings.py`. Maximum number of tokens allowed per user. 
   Subsequent requests for tokens will be rejected.  
   Default: `10`
 * Add `DSAT_HASHLIB_ALGO` in `settings.py`. A string representing the hash algorithm from hashlib.  
-  Supported values are 'sha512', 'sha256', 'sha384'
+  Supported values are 'sha512', 'sha256', 'sha384' 
   Default: `sha512`
-* 
+
 Example
 ```python
 DSAT_TOKEN_LENGTH = 80
 DSAT_MAX_TOKENS_PER_USER = 10
 DSAT_HASHLIB_ALGO = 'sha512'
 ```
```

### Comparing `django_salted_api_tokens-1.0.2/README.md` & `django_salted_api_tokens-1.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 # 3. Configuration
 * Add `DSAT_TOKEN_LENGTH` in `settings.py`  
   Default: `80` Max length: `256`  
 * Add `DSAT_MAX_TOKENS_PER_USER`  in `settings.py`. Maximum number of tokens allowed per user. 
   Subsequent requests for tokens will be rejected.  
   Default: `10`
 * Add `DSAT_HASHLIB_ALGO` in `settings.py`. A string representing the hash algorithm from hashlib.  
-  Supported values are 'sha512', 'sha256', 'sha384'
+  Supported values are 'sha512', 'sha256', 'sha384' 
   Default: `sha512`
-* 
+
 Example
 ```python
 DSAT_TOKEN_LENGTH = 80
 DSAT_MAX_TOKENS_PER_USER = 10
 DSAT_HASHLIB_ALGO = 'sha512'
 ```
```

### Comparing `django_salted_api_tokens-1.0.2/pyproject.toml` & `django_salted_api_tokens-1.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "django_salted_api_tokens"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="Harisankar Krishna Swamy", email="harisankar.krishna@outlook.com" },
 ]
 description = "Django token authentication with hashed, salted tokens"
 readme = "README.md"
 requires-python = ">=3.9.2"
 dependencies = [
```

### Comparing `django_salted_api_tokens-1.0.2/src/django_salted_api_tokens/admin.py` & `django_salted_api_tokens-1.0.3/src/django_salted_api_tokens/admin.py`

 * *Files identical despite different names*

### Comparing `django_salted_api_tokens-1.0.2/src/django_salted_api_tokens/authentication.py` & `django_salted_api_tokens-1.0.3/src/django_salted_api_tokens/authentication.py`

 * *Files identical despite different names*

### Comparing `django_salted_api_tokens-1.0.2/src/django_salted_api_tokens/migrations/0001_initial.py` & `django_salted_api_tokens-1.0.3/src/django_salted_api_tokens/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_salted_api_tokens-1.0.2/src/django_salted_api_tokens/models.py` & `django_salted_api_tokens-1.0.3/src/django_salted_api_tokens/models.py`

 * *Files identical despite different names*

### Comparing `django_salted_api_tokens-1.0.2/src/django_salted_api_tokens/views.py` & `django_salted_api_tokens-1.0.3/src/django_salted_api_tokens/views.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,23 @@
-from ksuid import ksuid
 from rest_framework.authtoken.views import ObtainAuthToken
-from rest_framework.exceptions import ValidationError
 from rest_framework.response import Response
 
-from .models import ApiToken
 from .serializers import TokenResponseSerializer
-from .settings import (DSAT_HASHLIB_ALGO, DSAT_MAX_TOKENS_PER_USER,
-                       DSAT_TOKEN_LENGTH)
-from .utils import gen_token, hashed_secret
+from .utils import create_dsat_token_for_user
 
 
 class CreateApiToken(ObtainAuthToken):
     """
     Create API access token for user.
     """
 
     def post(self, request, *args, **kwargs):
         serializer = self.serializer_class(
             data=request.data, context={'request': request}
         )
         serializer.is_valid(raise_exception=True)
         user = serializer.validated_data['user']
-        n_user_tokens = ApiToken.objects.filter(user=user).count()
-        if n_user_tokens >= DSAT_MAX_TOKENS_PER_USER:
-            raise ValidationError('Maximum tokens limit reached for user')
-        token_id, user_token = f'{ksuid()}', gen_token(n_chars=DSAT_TOKEN_LENGTH)
-        db_token, created = ApiToken.objects.get_or_create(
-            user=user,
-            token_id=token_id,
-            token=hashed_secret(secret=user_token, algo=DSAT_HASHLIB_ALGO),
-        )
+        token_id, user_token = create_dsat_token_for_user(user)
         token_resp = TokenResponseSerializer(
-            {'token_id': db_token.token_id, 'token': user_token}
+            {'token_id': token_id, 'token': user_token}
         ).data
         return Response(token_resp)
```

### Comparing `django_salted_api_tokens-1.0.2/src/django_salted_api_tokens.egg-info/PKG-INFO` & `django_salted_api_tokens-1.0.3/src/django_salted_api_tokens.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-salted-api-tokens
-Version: 1.0.2
+Version: 1.0.3
 Summary: Django token authentication with hashed, salted tokens
 Author-email: Harisankar Krishna Swamy <harisankar.krishna@outlook.com>
 Project-URL: Homepage, https://github.com/harisankar-krishna-swamy/django_salted_api_tokens
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9.2
@@ -26,17 +26,17 @@
 # 3. Configuration
 * Add `DSAT_TOKEN_LENGTH` in `settings.py`  
   Default: `80` Max length: `256`  
 * Add `DSAT_MAX_TOKENS_PER_USER`  in `settings.py`. Maximum number of tokens allowed per user. 
   Subsequent requests for tokens will be rejected.  
   Default: `10`
 * Add `DSAT_HASHLIB_ALGO` in `settings.py`. A string representing the hash algorithm from hashlib.  
-  Supported values are 'sha512', 'sha256', 'sha384'
+  Supported values are 'sha512', 'sha256', 'sha384' 
   Default: `sha512`
-* 
+
 Example
 ```python
 DSAT_TOKEN_LENGTH = 80
 DSAT_MAX_TOKENS_PER_USER = 10
 DSAT_HASHLIB_ALGO = 'sha512'
 ```
```

### Comparing `django_salted_api_tokens-1.0.2/src/django_salted_api_tokens.egg-info/SOURCES.txt` & `django_salted_api_tokens-1.0.3/src/django_salted_api_tokens.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 src/django_salted_api_tokens/utils.py
 src/django_salted_api_tokens/views.py
 src/django_salted_api_tokens.egg-info/PKG-INFO
 src/django_salted_api_tokens.egg-info/SOURCES.txt
 src/django_salted_api_tokens.egg-info/dependency_links.txt
 src/django_salted_api_tokens.egg-info/requires.txt
 src/django_salted_api_tokens.egg-info/top_level.txt
+src/django_salted_api_tokens/management/__init__.py
+src/django_salted_api_tokens/management/commands/__init__.py
+src/django_salted_api_tokens/management/commands/create_dsat_for_user.py
 src/django_salted_api_tokens/migrations/0001_initial.py
 src/django_salted_api_tokens/migrations/__init__.py
 src/example_django_project/__init__.py
 src/example_django_project/manage.py
 src/example_django_project/accounts/__init__.py
 src/example_django_project/accounts/admin.py
 src/example_django_project/accounts/apps.py
@@ -30,8 +33,9 @@
 src/example_django_project/example_django_project/__init__.py
 src/example_django_project/example_django_project/settings.py
 src/example_django_project/example_django_project/urls.py
 src/example_django_project/example_django_project/wsgi.py
 src/tests/__init__.py
 src/tests/factories.py
 src/tests/test_authentication_api_key_secret.py
+src/tests/test_mgmt_cmd_create_dsat_for_user.py
 src/tests/test_view_create_api_key_secret.py
```

### Comparing `django_salted_api_tokens-1.0.2/src/example_django_project/example_django_project/settings.py` & `django_salted_api_tokens-1.0.3/src/example_django_project/example_django_project/settings.py`

 * *Files identical despite different names*

### Comparing `django_salted_api_tokens-1.0.2/src/example_django_project/example_django_project/urls.py` & `django_salted_api_tokens-1.0.3/src/example_django_project/example_django_project/urls.py`

 * *Files identical despite different names*

### Comparing `django_salted_api_tokens-1.0.2/src/example_django_project/manage.py` & `django_salted_api_tokens-1.0.3/src/example_django_project/manage.py`

 * *Files identical despite different names*

### Comparing `django_salted_api_tokens-1.0.2/src/tests/factories.py` & `django_salted_api_tokens-1.0.3/src/tests/factories.py`

 * *Files identical despite different names*

### Comparing `django_salted_api_tokens-1.0.2/src/tests/test_authentication_api_key_secret.py` & `django_salted_api_tokens-1.0.3/src/tests/test_authentication_api_key_secret.py`

 * *Files identical despite different names*

### Comparing `django_salted_api_tokens-1.0.2/src/tests/test_view_create_api_key_secret.py` & `django_salted_api_tokens-1.0.3/src/tests/test_view_create_api_key_secret.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from http import HTTPStatus
 
-from django.test import TestCase, override_settings
+from django.test import TestCase
 from rest_framework.exceptions import ValidationError
 from rest_framework.test import APIClient
 
 from tests.factories import ApiTokenUserFactory, test_password
 
 
 class TestViewCreateApiToken(TestCase):
@@ -27,26 +27,24 @@
     def test_view__create_api_token(self):
         client = APIClient(enforce_csrf_checks=True)
         ep = self.url_dsat
         data = {'username': self.user.username, 'password': test_password}
         response = client.post(path=ep, data=data)
         self._assert_http_ok_token_reponse(response)
 
-    @override_settings(DSAT_MAX_TOKENS_PER_USER=2)
     def test_view__max_tokens_per_user(self):
         from django.conf import settings
 
-        for i in range(1, settings.DSAT_MAX_TOKENS_PER_USER + 1):
+        for i in range(0, settings.DSAT_MAX_TOKENS_PER_USER + 1):
             client = APIClient(enforce_csrf_checks=True)
             ep = self.url_dsat
             data = {'username': self.user.username, 'password': test_password}
-            if i <= settings.DSAT_MAX_TOKENS_PER_USER:
+            if i < settings.DSAT_MAX_TOKENS_PER_USER:
                 response = client.post(path=ep, data=data)
                 self._assert_http_ok_token_reponse(response)
             else:
-                with self.assertRaises(ValidationError):
-                    response = client.post(path=ep, data=data)
-                    self.assertEqual(
-                        HTTPStatus.BAD_REQUEST,
-                        response.status_code,
-                        'Validation error must be raised on reaching DSAT_MAX_TOKENS_PER_USER',
-                    )
+                response = client.post(path=ep, data=data)
+                self.assertEqual(
+                    HTTPStatus.BAD_REQUEST,
+                    response.status_code,
+                    'Validation error must be raised on reaching DSAT_MAX_TOKENS_PER_USER',
+                )
```

