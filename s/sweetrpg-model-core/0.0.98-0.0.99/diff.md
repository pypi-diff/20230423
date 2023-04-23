# Comparing `tmp/sweetrpg-model-core-0.0.98.tar.gz` & `tmp/sweetrpg-model-core-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sweetrpg-model-core-0.0.98.tar", last modified: Sun Jan 29 21:22:55 2023, max compression
+gzip compressed data, was "sweetrpg-model-core-0.0.99.tar", last modified: Sun Feb  5 01:35:59 2023, max compression
```

## Comparing `sweetrpg-model-core-0.0.98.tar` & `sweetrpg-model-core-0.0.99.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-29 21:22:55.771561 sweetrpg-model-core-0.0.98/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-01-29 21:22:52.000000 sweetrpg-model-core-0.0.98/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2080 2023-01-29 21:22:55.771561 sweetrpg-model-core-0.0.98/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1444 2023-01-29 21:22:52.000000 sweetrpg-model-core-0.0.98/README.md
--rw-r--r--   0 root         (0) root         (0)     1159 2023-01-29 21:22:55.771561 sweetrpg-model-core-0.0.98/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      232 2023-01-29 21:22:52.000000 sweetrpg-model-core-0.0.98/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-29 21:22:55.767562 sweetrpg-model-core-0.0.98/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-29 21:22:55.767562 sweetrpg-model-core-0.0.98/src/sweetrpg_model_core/
--rw-r--r--   0 root         (0) root         (0)      419 2023-01-29 21:22:53.000000 sweetrpg-model-core-0.0.98/src/sweetrpg_model_core/__init__.py
--rw-r--r--   0 root         (0) root         (0)      119 2023-01-29 21:22:52.000000 sweetrpg-model-core-0.0.98/src/sweetrpg_model_core/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-29 21:22:55.767562 sweetrpg-model-core-0.0.98/src/sweetrpg_model_core/convert/
--rw-r--r--   0 root         (0) root         (0)       81 2023-01-29 21:22:52.000000 sweetrpg-model-core-0.0.98/src/sweetrpg_model_core/convert/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2566 2023-01-29 21:22:52.000000 sweetrpg-model-core-0.0.98/src/sweetrpg_model_core/convert/date.py
--rw-r--r--   0 root         (0) root         (0)     1922 2023-01-29 21:22:52.000000 sweetrpg-model-core-0.0.98/src/sweetrpg_model_core/convert/document.py
--rw-r--r--   0 root         (0) root         (0)      891 2023-01-29 21:22:52.000000 sweetrpg-model-core-0.0.98/src/sweetrpg_model_core/convert/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-29 21:22:55.771561 sweetrpg-model-core-0.0.98/src/sweetrpg_model_core/model/
--rw-r--r--   0 root         (0) root         (0)       81 2023-01-29 21:22:52.000000 sweetrpg-model-core-0.0.98/src/sweetrpg_model_core/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2662 2023-01-29 21:22:52.000000 sweetrpg-model-core-0.0.98/src/sweetrpg_model_core/model/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-29 21:22:55.771561 sweetrpg-model-core-0.0.98/src/sweetrpg_model_core/schema/
--rw-r--r--   0 root         (0) root         (0)       89 2023-01-29 21:22:52.000000 sweetrpg-model-core-0.0.98/src/sweetrpg_model_core/schema/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2086 2023-01-29 21:22:52.000000 sweetrpg-model-core-0.0.98/src/sweetrpg_model_core/schema/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-29 21:22:55.767562 sweetrpg-model-core-0.0.98/src/sweetrpg_model_core.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2080 2023-01-29 21:22:55.000000 sweetrpg-model-core-0.0.98/src/sweetrpg_model_core.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      724 2023-01-29 21:22:55.000000 sweetrpg-model-core-0.0.98/src/sweetrpg_model_core.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-29 21:22:55.000000 sweetrpg-model-core-0.0.98/src/sweetrpg_model_core.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-01-29 21:22:55.000000 sweetrpg-model-core-0.0.98/src/sweetrpg_model_core.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       33 2023-01-29 21:22:55.000000 sweetrpg-model-core-0.0.98/src/sweetrpg_model_core.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-01-29 21:22:55.000000 sweetrpg-model-core-0.0.98/src/sweetrpg_model_core.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-05 01:35:59.440001 sweetrpg-model-core-0.0.99/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-02-05 01:35:56.000000 sweetrpg-model-core-0.0.99/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2080 2023-02-05 01:35:59.440001 sweetrpg-model-core-0.0.99/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1444 2023-02-05 01:35:56.000000 sweetrpg-model-core-0.0.99/README.md
+-rw-r--r--   0 root         (0) root         (0)     1159 2023-02-05 01:35:59.440001 sweetrpg-model-core-0.0.99/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      254 2023-02-05 01:35:56.000000 sweetrpg-model-core-0.0.99/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-05 01:35:59.436001 sweetrpg-model-core-0.0.99/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-05 01:35:59.436001 sweetrpg-model-core-0.0.99/src/sweetrpg_model_core/
+-rw-r--r--   0 root         (0) root         (0)      419 2023-02-05 01:35:57.000000 sweetrpg-model-core-0.0.99/src/sweetrpg_model_core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      119 2023-02-05 01:35:56.000000 sweetrpg-model-core-0.0.99/src/sweetrpg_model_core/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-05 01:35:59.436001 sweetrpg-model-core-0.0.99/src/sweetrpg_model_core/convert/
+-rw-r--r--   0 root         (0) root         (0)       81 2023-02-05 01:35:56.000000 sweetrpg-model-core-0.0.99/src/sweetrpg_model_core/convert/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2566 2023-02-05 01:35:56.000000 sweetrpg-model-core-0.0.99/src/sweetrpg_model_core/convert/date.py
+-rw-r--r--   0 root         (0) root         (0)     1922 2023-02-05 01:35:56.000000 sweetrpg-model-core-0.0.99/src/sweetrpg_model_core/convert/document.py
+-rw-r--r--   0 root         (0) root         (0)      891 2023-02-05 01:35:56.000000 sweetrpg-model-core-0.0.99/src/sweetrpg_model_core/convert/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-05 01:35:59.436001 sweetrpg-model-core-0.0.99/src/sweetrpg_model_core/model/
+-rw-r--r--   0 root         (0) root         (0)       81 2023-02-05 01:35:56.000000 sweetrpg-model-core-0.0.99/src/sweetrpg_model_core/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2662 2023-02-05 01:35:56.000000 sweetrpg-model-core-0.0.99/src/sweetrpg_model_core/model/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-05 01:35:59.440001 sweetrpg-model-core-0.0.99/src/sweetrpg_model_core/schema/
+-rw-r--r--   0 root         (0) root         (0)       89 2023-02-05 01:35:56.000000 sweetrpg-model-core-0.0.99/src/sweetrpg_model_core/schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2086 2023-02-05 01:35:56.000000 sweetrpg-model-core-0.0.99/src/sweetrpg_model_core/schema/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-05 01:35:59.436001 sweetrpg-model-core-0.0.99/src/sweetrpg_model_core.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2080 2023-02-05 01:35:59.000000 sweetrpg-model-core-0.0.99/src/sweetrpg_model_core.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      724 2023-02-05 01:35:59.000000 sweetrpg-model-core-0.0.99/src/sweetrpg_model_core.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-02-05 01:35:59.000000 sweetrpg-model-core-0.0.99/src/sweetrpg_model_core.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-02-05 01:35:59.000000 sweetrpg-model-core-0.0.99/src/sweetrpg_model_core.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2023-02-05 01:35:59.000000 sweetrpg-model-core-0.0.99/src/sweetrpg_model_core.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-02-05 01:35:59.000000 sweetrpg-model-core-0.0.99/src/sweetrpg_model_core.egg-info/top_level.txt
```

### Comparing `sweetrpg-model-core-0.0.98/LICENSE` & `sweetrpg-model-core-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `sweetrpg-model-core-0.0.98/PKG-INFO` & `sweetrpg-model-core-0.0.99/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sweetrpg-model-core
-Version: 0.0.98
+Version: 0.0.99
 Home-page: https://sweetrpg.com
 Author: Paul Schifferer
 Author-email: dm@sweetrpg.com
 License: MIT
 Project-URL: Documentation, https://sweetrpg.github.io/model-core
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
```

### Comparing `sweetrpg-model-core-0.0.98/README.md` & `sweetrpg-model-core-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `sweetrpg-model-core-0.0.98/setup.cfg` & `sweetrpg-model-core-0.0.99/setup.cfg`

 * *Files identical despite different names*

### Comparing `sweetrpg-model-core-0.0.98/src/sweetrpg_model_core/convert/date.py` & `sweetrpg-model-core-0.0.99/src/sweetrpg_model_core/convert/date.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-model-core-0.0.98/src/sweetrpg_model_core/convert/document.py` & `sweetrpg-model-core-0.0.99/src/sweetrpg_model_core/convert/document.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-model-core-0.0.98/src/sweetrpg_model_core/convert/model.py` & `sweetrpg-model-core-0.0.99/src/sweetrpg_model_core/convert/model.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-model-core-0.0.98/src/sweetrpg_model_core/model/base.py` & `sweetrpg-model-core-0.0.99/src/sweetrpg_model_core/model/base.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-model-core-0.0.98/src/sweetrpg_model_core/schema/base.py` & `sweetrpg-model-core-0.0.99/src/sweetrpg_model_core/schema/base.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-model-core-0.0.98/src/sweetrpg_model_core.egg-info/PKG-INFO` & `sweetrpg-model-core-0.0.99/src/sweetrpg_model_core.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sweetrpg-model-core
-Version: 0.0.98
+Version: 0.0.99
 Home-page: https://sweetrpg.com
 Author: Paul Schifferer
 Author-email: dm@sweetrpg.com
 License: MIT
 Project-URL: Documentation, https://sweetrpg.github.io/model-core
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
```

### Comparing `sweetrpg-model-core-0.0.98/src/sweetrpg_model_core.egg-info/SOURCES.txt` & `sweetrpg-model-core-0.0.99/src/sweetrpg_model_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

