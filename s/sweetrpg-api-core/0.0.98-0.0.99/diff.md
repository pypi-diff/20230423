# Comparing `tmp/sweetrpg-api-core-0.0.98.tar.gz` & `tmp/sweetrpg-api-core-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sweetrpg-api-core-0.0.98.tar", last modified: Sun Feb 26 01:41:08 2023, max compression
+gzip compressed data, was "sweetrpg-api-core-0.0.99.tar", last modified: Sun Mar  5 00:30:11 2023, max compression
```

## Comparing `sweetrpg-api-core-0.0.98.tar` & `sweetrpg-api-core-0.0.99.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-26 01:41:08.764382 sweetrpg-api-core-0.0.98/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-02-26 01:41:06.000000 sweetrpg-api-core-0.0.98/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2035 2023-02-26 01:41:08.764382 sweetrpg-api-core-0.0.98/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1403 2023-02-26 01:41:06.000000 sweetrpg-api-core-0.0.98/README.md
--rw-r--r--   0 root         (0) root         (0)     1149 2023-02-26 01:41:08.764382 sweetrpg-api-core-0.0.98/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      334 2023-02-26 01:41:06.000000 sweetrpg-api-core-0.0.98/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-26 01:41:08.760382 sweetrpg-api-core-0.0.98/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-26 01:41:08.760382 sweetrpg-api-core-0.0.98/src/sweetrpg_api_core/
--rw-r--r--   0 root         (0) root         (0)      392 2023-02-26 01:41:06.000000 sweetrpg-api-core-0.0.98/src/sweetrpg_api_core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-26 01:41:08.764382 sweetrpg-api-core-0.0.98/src/sweetrpg_api_core/blueprints/
--rw-r--r--   0 root         (0) root         (0)       81 2023-02-26 01:41:06.000000 sweetrpg-api-core-0.0.98/src/sweetrpg_api_core/blueprints/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-26 01:41:08.764382 sweetrpg-api-core-0.0.98/src/sweetrpg_api_core/blueprints/health/
--rw-r--r--   0 root         (0) root         (0)     1718 2023-02-26 01:41:06.000000 sweetrpg-api-core-0.0.98/src/sweetrpg_api_core/blueprints/health/__init__.py
--rw-r--r--   0 root         (0) root         (0)      129 2023-02-26 01:41:06.000000 sweetrpg-api-core-0.0.98/src/sweetrpg_api_core/constants.py
--rw-r--r--   0 root         (0) root         (0)    29066 2023-02-26 01:41:06.000000 sweetrpg-api-core-0.0.98/src/sweetrpg_api_core/data.py
--rw-r--r--   0 root         (0) root         (0)      798 2023-02-26 01:41:06.000000 sweetrpg-api-core-0.0.98/src/sweetrpg_api_core/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-26 01:41:08.764382 sweetrpg-api-core-0.0.98/src/sweetrpg_api_core/schema/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-26 01:41:06.000000 sweetrpg-api-core-0.0.98/src/sweetrpg_api_core/schema/__init__.py
--rw-r--r--   0 root         (0) root         (0)      841 2023-02-26 01:41:06.000000 sweetrpg-api-core-0.0.98/src/sweetrpg_api_core/schema/base.py
--rw-r--r--   0 root         (0) root         (0)      524 2023-02-26 01:41:06.000000 sweetrpg-api-core-0.0.98/src/sweetrpg_api_core/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-26 01:41:08.764382 sweetrpg-api-core-0.0.98/src/sweetrpg_api_core.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2035 2023-02-26 01:41:08.000000 sweetrpg-api-core-0.0.98/src/sweetrpg_api_core.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      645 2023-02-26 01:41:08.000000 sweetrpg-api-core-0.0.98/src/sweetrpg_api_core.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-26 01:41:08.000000 sweetrpg-api-core-0.0.98/src/sweetrpg_api_core.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-02-26 01:41:08.000000 sweetrpg-api-core-0.0.98/src/sweetrpg_api_core.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       81 2023-02-26 01:41:08.000000 sweetrpg-api-core-0.0.98/src/sweetrpg_api_core.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-02-26 01:41:08.000000 sweetrpg-api-core-0.0.98/src/sweetrpg_api_core.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-05 00:30:11.118792 sweetrpg-api-core-0.0.99/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-03-05 00:30:08.000000 sweetrpg-api-core-0.0.99/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2035 2023-03-05 00:30:11.118792 sweetrpg-api-core-0.0.99/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1403 2023-03-05 00:30:08.000000 sweetrpg-api-core-0.0.99/README.md
+-rw-r--r--   0 root         (0) root         (0)     1149 2023-03-05 00:30:11.118792 sweetrpg-api-core-0.0.99/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      334 2023-03-05 00:30:08.000000 sweetrpg-api-core-0.0.99/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-05 00:30:11.114792 sweetrpg-api-core-0.0.99/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-05 00:30:11.118792 sweetrpg-api-core-0.0.99/src/sweetrpg_api_core/
+-rw-r--r--   0 root         (0) root         (0)      392 2023-03-05 00:30:09.000000 sweetrpg-api-core-0.0.99/src/sweetrpg_api_core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-05 00:30:11.118792 sweetrpg-api-core-0.0.99/src/sweetrpg_api_core/blueprints/
+-rw-r--r--   0 root         (0) root         (0)       81 2023-03-05 00:30:08.000000 sweetrpg-api-core-0.0.99/src/sweetrpg_api_core/blueprints/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-05 00:30:11.118792 sweetrpg-api-core-0.0.99/src/sweetrpg_api_core/blueprints/health/
+-rw-r--r--   0 root         (0) root         (0)     1718 2023-03-05 00:30:08.000000 sweetrpg-api-core-0.0.99/src/sweetrpg_api_core/blueprints/health/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      129 2023-03-05 00:30:08.000000 sweetrpg-api-core-0.0.99/src/sweetrpg_api_core/constants.py
+-rw-r--r--   0 root         (0) root         (0)    29066 2023-03-05 00:30:08.000000 sweetrpg-api-core-0.0.99/src/sweetrpg_api_core/data.py
+-rw-r--r--   0 root         (0) root         (0)      798 2023-03-05 00:30:08.000000 sweetrpg-api-core-0.0.99/src/sweetrpg_api_core/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-05 00:30:11.118792 sweetrpg-api-core-0.0.99/src/sweetrpg_api_core/schema/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-05 00:30:08.000000 sweetrpg-api-core-0.0.99/src/sweetrpg_api_core/schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      841 2023-03-05 00:30:08.000000 sweetrpg-api-core-0.0.99/src/sweetrpg_api_core/schema/base.py
+-rw-r--r--   0 root         (0) root         (0)      524 2023-03-05 00:30:08.000000 sweetrpg-api-core-0.0.99/src/sweetrpg_api_core/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-05 00:30:11.118792 sweetrpg-api-core-0.0.99/src/sweetrpg_api_core.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2035 2023-03-05 00:30:11.000000 sweetrpg-api-core-0.0.99/src/sweetrpg_api_core.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      645 2023-03-05 00:30:11.000000 sweetrpg-api-core-0.0.99/src/sweetrpg_api_core.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-05 00:30:11.000000 sweetrpg-api-core-0.0.99/src/sweetrpg_api_core.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-03-05 00:30:11.000000 sweetrpg-api-core-0.0.99/src/sweetrpg_api_core.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       81 2023-03-05 00:30:11.000000 sweetrpg-api-core-0.0.99/src/sweetrpg_api_core.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-03-05 00:30:11.000000 sweetrpg-api-core-0.0.99/src/sweetrpg_api_core.egg-info/top_level.txt
```

### Comparing `sweetrpg-api-core-0.0.98/LICENSE` & `sweetrpg-api-core-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `sweetrpg-api-core-0.0.98/PKG-INFO` & `sweetrpg-api-core-0.0.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sweetrpg-api-core
-Version: 0.0.98
+Version: 0.0.99
 Home-page: https://sweetrpg.com
 Author: Paul Schifferer
 Author-email: dm@sweetrpg.com
 License: MIT
 Project-URL: Documentation, https://sweetrpg.github.io/api-core
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
```

### Comparing `sweetrpg-api-core-0.0.98/README.md` & `sweetrpg-api-core-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `sweetrpg-api-core-0.0.98/setup.cfg` & `sweetrpg-api-core-0.0.99/setup.cfg`

 * *Files identical despite different names*

### Comparing `sweetrpg-api-core-0.0.98/src/sweetrpg_api_core/blueprints/health/__init__.py` & `sweetrpg-api-core-0.0.99/src/sweetrpg_api_core/blueprints/health/__init__.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-api-core-0.0.98/src/sweetrpg_api_core/data.py` & `sweetrpg-api-core-0.0.99/src/sweetrpg_api_core/data.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-api-core-0.0.98/src/sweetrpg_api_core/errors.py` & `sweetrpg-api-core-0.0.99/src/sweetrpg_api_core/errors.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-api-core-0.0.98/src/sweetrpg_api_core/schema/base.py` & `sweetrpg-api-core-0.0.99/src/sweetrpg_api_core/schema/base.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-api-core-0.0.98/src/sweetrpg_api_core/utils.py` & `sweetrpg-api-core-0.0.99/src/sweetrpg_api_core/utils.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-api-core-0.0.98/src/sweetrpg_api_core.egg-info/PKG-INFO` & `sweetrpg-api-core-0.0.99/src/sweetrpg_api_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sweetrpg-api-core
-Version: 0.0.98
+Version: 0.0.99
 Home-page: https://sweetrpg.com
 Author: Paul Schifferer
 Author-email: dm@sweetrpg.com
 License: MIT
 Project-URL: Documentation, https://sweetrpg.github.io/api-core
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
```

### Comparing `sweetrpg-api-core-0.0.98/src/sweetrpg_api_core.egg-info/SOURCES.txt` & `sweetrpg-api-core-0.0.99/src/sweetrpg_api_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

