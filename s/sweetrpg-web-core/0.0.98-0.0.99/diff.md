# Comparing `tmp/sweetrpg-web-core-0.0.98.tar.gz` & `tmp/sweetrpg-web-core-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sweetrpg-web-core-0.0.98.tar", last modified: Sat Jan  8 14:39:03 2022, max compression
+gzip compressed data, was "dist/sweetrpg-web-core-0.0.99.tar", last modified: Sat Jan  8 14:41:55 2022, max compression
```

## Comparing `sweetrpg-web-core-0.0.98.tar` & `sweetrpg-web-core-0.0.99.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-08 14:39:03.000000 sweetrpg-web-core-0.0.98/
--rw-r--r--   0 root         (0) root         (0)     1065 2022-01-08 14:39:00.000000 sweetrpg-web-core-0.0.98/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2072 2022-01-08 14:39:03.000000 sweetrpg-web-core-0.0.98/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1403 2022-01-08 14:39:00.000000 sweetrpg-web-core-0.0.98/README.md
--rw-r--r--   0 root         (0) root         (0)     1148 2022-01-08 14:39:03.000000 sweetrpg-web-core-0.0.98/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      220 2022-01-08 14:39:00.000000 sweetrpg-web-core-0.0.98/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-08 14:39:03.000000 sweetrpg-web-core-0.0.98/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-08 14:39:03.000000 sweetrpg-web-core-0.0.98/src/sweetrpg_web_core/
--rw-r--r--   0 root         (0) root         (0)      401 2022-01-08 14:39:01.000000 sweetrpg-web-core-0.0.98/src/sweetrpg_web_core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-08 14:39:03.000000 sweetrpg-web-core-0.0.98/src/sweetrpg_web_core/blueprints/
--rw-r--r--   0 root         (0) root         (0)       81 2022-01-08 14:39:00.000000 sweetrpg-web-core-0.0.98/src/sweetrpg_web_core/blueprints/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-08 14:39:03.000000 sweetrpg-web-core-0.0.98/src/sweetrpg_web_core/blueprints/health/
--rw-r--r--   0 root         (0) root         (0)     1361 2022-01-08 14:39:00.000000 sweetrpg-web-core-0.0.98/src/sweetrpg_web_core/blueprints/health/__init__.py
--rw-r--r--   0 root         (0) root         (0)      525 2022-01-08 14:39:00.000000 sweetrpg-web-core-0.0.98/src/sweetrpg_web_core/constants.py
--rw-r--r--   0 root         (0) root         (0)      798 2022-01-08 14:39:00.000000 sweetrpg-web-core-0.0.98/src/sweetrpg_web_core/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-08 14:39:03.000000 sweetrpg-web-core-0.0.98/src/sweetrpg_web_core/helpers/
--rw-r--r--   0 root         (0) root         (0)       98 2022-01-08 14:39:00.000000 sweetrpg-web-core-0.0.98/src/sweetrpg_web_core/helpers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4207 2022-01-08 14:39:00.000000 sweetrpg-web-core-0.0.98/src/sweetrpg_web_core/helpers/context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-08 14:39:03.000000 sweetrpg-web-core-0.0.98/src/sweetrpg_web_core.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2072 2022-01-08 14:39:03.000000 sweetrpg-web-core-0.0.98/src/sweetrpg_web_core.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      589 2022-01-08 14:39:03.000000 sweetrpg-web-core-0.0.98/src/sweetrpg_web_core.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-01-08 14:39:03.000000 sweetrpg-web-core-0.0.98/src/sweetrpg_web_core.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2022-01-08 14:39:03.000000 sweetrpg-web-core-0.0.98/src/sweetrpg_web_core.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       11 2022-01-08 14:39:03.000000 sweetrpg-web-core-0.0.98/src/sweetrpg_web_core.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2022-01-08 14:39:03.000000 sweetrpg-web-core-0.0.98/src/sweetrpg_web_core.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-08 14:41:55.000000 sweetrpg-web-core-0.0.99/
+-rw-r--r--   0 root         (0) root         (0)     1065 2022-01-08 14:41:53.000000 sweetrpg-web-core-0.0.99/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2072 2022-01-08 14:41:55.000000 sweetrpg-web-core-0.0.99/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1403 2022-01-08 14:41:53.000000 sweetrpg-web-core-0.0.99/README.md
+-rw-r--r--   0 root         (0) root         (0)     1148 2022-01-08 14:41:55.000000 sweetrpg-web-core-0.0.99/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      220 2022-01-08 14:41:53.000000 sweetrpg-web-core-0.0.99/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-08 14:41:55.000000 sweetrpg-web-core-0.0.99/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-08 14:41:55.000000 sweetrpg-web-core-0.0.99/src/sweetrpg_web_core/
+-rw-r--r--   0 root         (0) root         (0)      401 2022-01-08 14:41:53.000000 sweetrpg-web-core-0.0.99/src/sweetrpg_web_core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-08 14:41:55.000000 sweetrpg-web-core-0.0.99/src/sweetrpg_web_core/blueprints/
+-rw-r--r--   0 root         (0) root         (0)       81 2022-01-08 14:41:53.000000 sweetrpg-web-core-0.0.99/src/sweetrpg_web_core/blueprints/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-08 14:41:55.000000 sweetrpg-web-core-0.0.99/src/sweetrpg_web_core/blueprints/health/
+-rw-r--r--   0 root         (0) root         (0)     1361 2022-01-08 14:41:53.000000 sweetrpg-web-core-0.0.99/src/sweetrpg_web_core/blueprints/health/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      525 2022-01-08 14:41:53.000000 sweetrpg-web-core-0.0.99/src/sweetrpg_web_core/constants.py
+-rw-r--r--   0 root         (0) root         (0)      798 2022-01-08 14:41:53.000000 sweetrpg-web-core-0.0.99/src/sweetrpg_web_core/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-08 14:41:55.000000 sweetrpg-web-core-0.0.99/src/sweetrpg_web_core/helpers/
+-rw-r--r--   0 root         (0) root         (0)       98 2022-01-08 14:41:53.000000 sweetrpg-web-core-0.0.99/src/sweetrpg_web_core/helpers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4207 2022-01-08 14:41:53.000000 sweetrpg-web-core-0.0.99/src/sweetrpg_web_core/helpers/context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-08 14:41:55.000000 sweetrpg-web-core-0.0.99/src/sweetrpg_web_core.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2072 2022-01-08 14:41:55.000000 sweetrpg-web-core-0.0.99/src/sweetrpg_web_core.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      589 2022-01-08 14:41:55.000000 sweetrpg-web-core-0.0.99/src/sweetrpg_web_core.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-08 14:41:55.000000 sweetrpg-web-core-0.0.99/src/sweetrpg_web_core.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2022-01-08 14:41:55.000000 sweetrpg-web-core-0.0.99/src/sweetrpg_web_core.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2022-01-08 14:41:55.000000 sweetrpg-web-core-0.0.99/src/sweetrpg_web_core.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2022-01-08 14:41:55.000000 sweetrpg-web-core-0.0.99/src/sweetrpg_web_core.egg-info/top_level.txt
```

### Comparing `sweetrpg-web-core-0.0.98/LICENSE` & `sweetrpg-web-core-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `sweetrpg-web-core-0.0.98/PKG-INFO` & `sweetrpg-web-core-0.0.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sweetrpg-web-core
-Version: 0.0.98
+Version: 0.0.99
 Summary: UNKNOWN
 Home-page: https://sweetrpg.com
 Author: Paul Schifferer
 Author-email: dm@sweetrpg.com
 License: MIT
 Project-URL: Documentation, https://sweetrpg.github.io/web-core
 Platform: UNKNOWN
```

### Comparing `sweetrpg-web-core-0.0.98/README.md` & `sweetrpg-web-core-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `sweetrpg-web-core-0.0.98/setup.cfg` & `sweetrpg-web-core-0.0.99/setup.cfg`

 * *Files identical despite different names*

### Comparing `sweetrpg-web-core-0.0.98/src/sweetrpg_web_core/blueprints/health/__init__.py` & `sweetrpg-web-core-0.0.99/src/sweetrpg_web_core/blueprints/health/__init__.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-web-core-0.0.98/src/sweetrpg_web_core/constants.py` & `sweetrpg-web-core-0.0.99/src/sweetrpg_web_core/constants.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-web-core-0.0.98/src/sweetrpg_web_core/errors.py` & `sweetrpg-web-core-0.0.99/src/sweetrpg_web_core/errors.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-web-core-0.0.98/src/sweetrpg_web_core/helpers/context.py` & `sweetrpg-web-core-0.0.99/src/sweetrpg_web_core/helpers/context.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-web-core-0.0.98/src/sweetrpg_web_core.egg-info/PKG-INFO` & `sweetrpg-web-core-0.0.99/src/sweetrpg_web_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sweetrpg-web-core
-Version: 0.0.98
+Version: 0.0.99
 Summary: UNKNOWN
 Home-page: https://sweetrpg.com
 Author: Paul Schifferer
 Author-email: dm@sweetrpg.com
 License: MIT
 Project-URL: Documentation, https://sweetrpg.github.io/web-core
 Platform: UNKNOWN
```

### Comparing `sweetrpg-web-core-0.0.98/src/sweetrpg_web_core.egg-info/SOURCES.txt` & `sweetrpg-web-core-0.0.99/src/sweetrpg_web_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

