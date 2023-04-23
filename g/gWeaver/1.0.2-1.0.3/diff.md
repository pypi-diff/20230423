# Comparing `tmp/gWeaver-1.0.2.tar.gz` & `tmp/gWeaver-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gWeaver-1.0.2.tar", last modified: Sun Apr 23 18:28:28 2023, max compression
+gzip compressed data, was "gWeaver-1.0.3.tar", last modified: Sun Apr 23 18:42:20 2023, max compression
```

## Comparing `gWeaver-1.0.2.tar` & `gWeaver-1.0.3.tar`

### file list

```diff
@@ -1,24 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:28:28.853352 gWeaver-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-23 18:27:54.000000 gWeaver-1.0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-23 18:28:28.853352 gWeaver-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-23 18:27:54.000000 gWeaver-1.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:28:28.849352 gWeaver-1.0.2/gWeaver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 18:27:54.000000 gWeaver-1.0.2/gWeaver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-23 18:27:54.000000 gWeaver-1.0.2/gWeaver/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-23 18:27:54.000000 gWeaver-1.0.2/gWeaver/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-23 18:27:54.000000 gWeaver-1.0.2/gWeaver/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-23 18:27:54.000000 gWeaver-1.0.2/gWeaver/graph_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:28:28.853352 gWeaver-1.0.2/gWeaver/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 18:27:54.000000 gWeaver-1.0.2/gWeaver/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 18:27:54.000000 gWeaver-1.0.2/gWeaver/models.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-23 18:27:54.000000 gWeaver-1.0.2/gWeaver/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-23 18:27:54.000000 gWeaver-1.0.2/gWeaver/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:28:28.853352 gWeaver-1.0.2/gWeaver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-23 18:28:28.000000 gWeaver-1.0.2/gWeaver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-23 18:28:28.000000 gWeaver-1.0.2/gWeaver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 18:28:28.000000 gWeaver-1.0.2/gWeaver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 18:28:27.000000 gWeaver-1.0.2/gWeaver.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-23 18:28:28.000000 gWeaver-1.0.2/gWeaver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-23 18:28:28.000000 gWeaver-1.0.2/gWeaver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-23 18:28:28.853352 gWeaver-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-23 18:27:54.000000 gWeaver-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:42:20.664476 gWeaver-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-23 18:41:27.000000 gWeaver-1.0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-23 18:42:20.664476 gWeaver-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-23 18:41:27.000000 gWeaver-1.0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:42:20.660476 gWeaver-1.0.3/gWeaver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 18:41:27.000000 gWeaver-1.0.3/gWeaver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-23 18:41:27.000000 gWeaver-1.0.3/gWeaver/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-23 18:41:27.000000 gWeaver-1.0.3/gWeaver/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-23 18:41:27.000000 gWeaver-1.0.3/gWeaver/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:42:20.660476 gWeaver-1.0.3/gWeaver/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 18:41:27.000000 gWeaver-1.0.3/gWeaver/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-04-23 18:41:27.000000 gWeaver-1.0.3/gWeaver/base/graph_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-23 18:41:27.000000 gWeaver-1.0.3/gWeaver/base/graph_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-23 18:41:27.000000 gWeaver-1.0.3/gWeaver/base/graph_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-04-23 18:41:27.000000 gWeaver-1.0.3/gWeaver/base/node_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-04-23 18:41:27.000000 gWeaver-1.0.3/gWeaver/base/response_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-23 18:41:27.000000 gWeaver-1.0.3/gWeaver/graph_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:42:20.664476 gWeaver-1.0.3/gWeaver/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 18:41:27.000000 gWeaver-1.0.3/gWeaver/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-23 18:41:27.000000 gWeaver-1.0.3/gWeaver/management/graph_migrate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:42:20.664476 gWeaver-1.0.3/gWeaver/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 18:41:27.000000 gWeaver-1.0.3/gWeaver/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-23 18:41:27.000000 gWeaver-1.0.3/gWeaver/managers/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:42:20.664476 gWeaver-1.0.3/gWeaver/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 18:41:27.000000 gWeaver-1.0.3/gWeaver/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 18:41:27.000000 gWeaver-1.0.3/gWeaver/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-23 18:41:27.000000 gWeaver-1.0.3/gWeaver/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-23 18:41:27.000000 gWeaver-1.0.3/gWeaver/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:42:20.660476 gWeaver-1.0.3/gWeaver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-23 18:42:20.000000 gWeaver-1.0.3/gWeaver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-23 18:42:20.000000 gWeaver-1.0.3/gWeaver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 18:42:20.000000 gWeaver-1.0.3/gWeaver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 18:42:19.000000 gWeaver-1.0.3/gWeaver.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-23 18:42:20.000000 gWeaver-1.0.3/gWeaver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-23 18:42:20.000000 gWeaver-1.0.3/gWeaver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-23 18:42:20.664476 gWeaver-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-23 18:41:27.000000 gWeaver-1.0.3/setup.py
```

### Comparing `gWeaver-1.0.2/LICENSE.txt` & `gWeaver-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gWeaver-1.0.2/PKG-INFO` & `gWeaver-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gWeaver
-Version: 1.0.2
+Version: 1.0.3
 Summary: dgraph operation module for Django REST Framework
 Home-page: https://github.com/iamr2k/gWeaver
 Author: Rahul Babu K
 Author-email: rahulbabu101@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `gWeaver-1.0.2/gWeaver/actions.py` & `gWeaver-1.0.3/gWeaver/actions.py`

 * *Files identical despite different names*

### Comparing `gWeaver-1.0.2/gWeaver.egg-info/PKG-INFO` & `gWeaver-1.0.3/gWeaver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gWeaver
-Version: 1.0.2
+Version: 1.0.3
 Summary: dgraph operation module for Django REST Framework
 Home-page: https://github.com/iamr2k/gWeaver
 Author: Rahul Babu K
 Author-email: rahulbabu101@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `gWeaver-1.0.2/setup.py` & `gWeaver-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     + extras_require["doc"]
     + extras_require["python-jose"]
 )
 
 
 setup(
     name="gWeaver",
-    version = "1.0.2",
+    version = "1.0.3",
     url="https://github.com/iamr2k/gWeaver",
     license="MIT",
     description="dgraph operation module for Django REST Framework",
     long_description=Path("README.rst").read_text(encoding="utf-8"),
     author="Rahul Babu K",
     author_email="rahulbabu101@gmail.com",
     install_requires=[
```

