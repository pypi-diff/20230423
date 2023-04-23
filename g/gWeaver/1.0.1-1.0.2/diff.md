# Comparing `tmp/gWeaver-1.0.1.tar.gz` & `tmp/gWeaver-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gWeaver-1.0.1.tar", last modified: Sun Apr 23 18:20:49 2023, max compression
+gzip compressed data, was "gWeaver-1.0.2.tar", last modified: Sun Apr 23 18:28:28 2023, max compression
```

## Comparing `gWeaver-1.0.1.tar` & `gWeaver-1.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:20:49.836255 gWeaver-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-23 18:20:12.000000 gWeaver-1.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-23 18:20:49.836255 gWeaver-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-23 18:20:12.000000 gWeaver-1.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:20:49.836255 gWeaver-1.0.1/dgraph_operations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 18:20:12.000000 gWeaver-1.0.1/dgraph_operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-23 18:20:12.000000 gWeaver-1.0.1/dgraph_operations/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-23 18:20:12.000000 gWeaver-1.0.1/dgraph_operations/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-23 18:20:12.000000 gWeaver-1.0.1/dgraph_operations/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-23 18:20:12.000000 gWeaver-1.0.1/dgraph_operations/graph_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:20:49.836255 gWeaver-1.0.1/dgraph_operations/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 18:20:12.000000 gWeaver-1.0.1/dgraph_operations/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 18:20:12.000000 gWeaver-1.0.1/dgraph_operations/models.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-23 18:20:12.000000 gWeaver-1.0.1/dgraph_operations/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-23 18:20:12.000000 gWeaver-1.0.1/dgraph_operations/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:20:49.836255 gWeaver-1.0.1/gWeaver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-23 18:20:49.000000 gWeaver-1.0.1/gWeaver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-23 18:20:49.000000 gWeaver-1.0.1/gWeaver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 18:20:49.000000 gWeaver-1.0.1/gWeaver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 18:20:48.000000 gWeaver-1.0.1/gWeaver.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-23 18:20:49.000000 gWeaver-1.0.1/gWeaver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-23 18:20:49.000000 gWeaver-1.0.1/gWeaver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-23 18:20:49.836255 gWeaver-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-23 18:20:12.000000 gWeaver-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:28:28.853352 gWeaver-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-23 18:27:54.000000 gWeaver-1.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-23 18:28:28.853352 gWeaver-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-23 18:27:54.000000 gWeaver-1.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:28:28.849352 gWeaver-1.0.2/gWeaver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 18:27:54.000000 gWeaver-1.0.2/gWeaver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-23 18:27:54.000000 gWeaver-1.0.2/gWeaver/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-23 18:27:54.000000 gWeaver-1.0.2/gWeaver/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-23 18:27:54.000000 gWeaver-1.0.2/gWeaver/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-23 18:27:54.000000 gWeaver-1.0.2/gWeaver/graph_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:28:28.853352 gWeaver-1.0.2/gWeaver/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 18:27:54.000000 gWeaver-1.0.2/gWeaver/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 18:27:54.000000 gWeaver-1.0.2/gWeaver/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-23 18:27:54.000000 gWeaver-1.0.2/gWeaver/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-23 18:27:54.000000 gWeaver-1.0.2/gWeaver/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:28:28.853352 gWeaver-1.0.2/gWeaver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-23 18:28:28.000000 gWeaver-1.0.2/gWeaver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-23 18:28:28.000000 gWeaver-1.0.2/gWeaver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 18:28:28.000000 gWeaver-1.0.2/gWeaver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 18:28:27.000000 gWeaver-1.0.2/gWeaver.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-23 18:28:28.000000 gWeaver-1.0.2/gWeaver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-23 18:28:28.000000 gWeaver-1.0.2/gWeaver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-23 18:28:28.853352 gWeaver-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-23 18:27:54.000000 gWeaver-1.0.2/setup.py
```

### Comparing `gWeaver-1.0.1/LICENSE.txt` & `gWeaver-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gWeaver-1.0.1/PKG-INFO` & `gWeaver-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gWeaver
-Version: 1.0.1
+Version: 1.0.2
 Summary: dgraph operation module for Django REST Framework
 Home-page: https://github.com/iamr2k/gWeaver
 Author: Rahul Babu K
 Author-email: rahulbabu101@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `gWeaver-1.0.1/dgraph_operations/actions.py` & `gWeaver-1.0.2/gWeaver/actions.py`

 * *Files identical despite different names*

### Comparing `gWeaver-1.0.1/gWeaver.egg-info/PKG-INFO` & `gWeaver-1.0.2/gWeaver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gWeaver
-Version: 1.0.1
+Version: 1.0.2
 Summary: dgraph operation module for Django REST Framework
 Home-page: https://github.com/iamr2k/gWeaver
 Author: Rahul Babu K
 Author-email: rahulbabu101@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `gWeaver-1.0.1/setup.py` & `gWeaver-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     + extras_require["doc"]
     + extras_require["python-jose"]
 )
 
 
 setup(
     name="gWeaver",
-    version = "1.0.1",
+    version = "1.0.2",
     url="https://github.com/iamr2k/gWeaver",
     license="MIT",
     description="dgraph operation module for Django REST Framework",
     long_description=Path("README.rst").read_text(encoding="utf-8"),
     author="Rahul Babu K",
     author_email="rahulbabu101@gmail.com",
     install_requires=[
```

