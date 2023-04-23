# Comparing `tmp/lets_debug_helper-1.5.3.tar.gz` & `tmp/lets_debug_helper-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lets_debug_helper-1.5.3.tar", max compression
+gzip compressed data, was "lets_debug_helper-1.5.4.tar", max compression
```

## Comparing `lets_debug_helper-1.5.3.tar` & `lets_debug_helper-1.5.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1070 2020-12-30 17:36:35.000000 lets_debug_helper-1.5.3/LICENSE
--rw-r--r--   0        0        0      602 2022-11-09 23:11:52.000026 lets_debug_helper-1.5.3/README.md
--rw-r--r--   0        0        0        0 2022-05-21 18:48:28.935073 lets_debug_helper-1.5.3/letsdebughelper/__init__.py
--rw-r--r--   0        0        0      833 2022-11-09 21:26:35.530699 lets_debug_helper-1.5.3/letsdebughelper/helpers.py
--rwxr-xr-x   0        0        0     3691 2022-11-09 23:01:49.551755 lets_debug_helper-1.5.3/letsdebughelper/letsdebug.py
--rw-r--r--   0        0        0        0 2022-05-21 18:48:28.936018 lets_debug_helper-1.5.3/letsdebughelper/tests/__init__.py
--rw-r--r--   0        0        0     1161 2022-11-09 21:30:15.848526 lets_debug_helper-1.5.3/letsdebughelper/tests/test_helpers.py
--rw-r--r--   0        0        0     9710 2022-11-09 23:08:21.750119 lets_debug_helper-1.5.3/letsdebughelper/tests/test_letsdebug.py
--rw-r--r--   0        0        0      900 2023-03-23 16:09:00.519087 lets_debug_helper-1.5.3/pyproject.toml
--rw-r--r--   0        0        0      898 1970-01-01 00:00:00.000000 lets_debug_helper-1.5.3/setup.py
--rw-r--r--   0        0        0      675 1970-01-01 00:00:00.000000 lets_debug_helper-1.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2020-12-30 17:36:35.000000 lets_debug_helper-1.5.4/LICENSE
+-rw-r--r--   0        0        0      602 2022-11-09 23:11:52.000026 lets_debug_helper-1.5.4/README.md
+-rw-r--r--   0        0        0        0 2022-05-21 18:48:28.935073 lets_debug_helper-1.5.4/letsdebughelper/__init__.py
+-rw-r--r--   0        0        0      833 2022-11-09 21:26:35.530699 lets_debug_helper-1.5.4/letsdebughelper/helpers.py
+-rwxr-xr-x   0        0        0     3691 2022-11-09 23:01:49.551755 lets_debug_helper-1.5.4/letsdebughelper/letsdebug.py
+-rw-r--r--   0        0        0        0 2022-05-21 18:48:28.936018 lets_debug_helper-1.5.4/letsdebughelper/tests/__init__.py
+-rw-r--r--   0        0        0     1161 2022-11-09 21:30:15.848526 lets_debug_helper-1.5.4/letsdebughelper/tests/test_helpers.py
+-rw-r--r--   0        0        0     9710 2022-11-09 23:08:21.750119 lets_debug_helper-1.5.4/letsdebughelper/tests/test_letsdebug.py
+-rw-r--r--   0        0        0      900 2023-04-23 07:43:29.706583 lets_debug_helper-1.5.4/pyproject.toml
+-rw-r--r--   0        0        0      898 1970-01-01 00:00:00.000000 lets_debug_helper-1.5.4/setup.py
+-rw-r--r--   0        0        0      675 1970-01-01 00:00:00.000000 lets_debug_helper-1.5.4/PKG-INFO
```

### Comparing `lets_debug_helper-1.5.3/LICENSE` & `lets_debug_helper-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lets_debug_helper-1.5.3/README.md` & `lets_debug_helper-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `lets_debug_helper-1.5.3/letsdebughelper/helpers.py` & `lets_debug_helper-1.5.4/letsdebughelper/helpers.py`

 * *Files identical despite different names*

### Comparing `lets_debug_helper-1.5.3/letsdebughelper/letsdebug.py` & `lets_debug_helper-1.5.4/letsdebughelper/letsdebug.py`

 * *Files identical despite different names*

### Comparing `lets_debug_helper-1.5.3/letsdebughelper/tests/test_helpers.py` & `lets_debug_helper-1.5.4/letsdebughelper/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `lets_debug_helper-1.5.3/letsdebughelper/tests/test_letsdebug.py` & `lets_debug_helper-1.5.4/letsdebughelper/tests/test_letsdebug.py`

 * *Files identical despite different names*

### Comparing `lets_debug_helper-1.5.3/pyproject.toml` & `lets_debug_helper-1.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lets-debug-helper"
-version = "1.5.3"
+version = "1.5.4"
 description = "This is a cli tool that interacts with the Let's Debug API"
 authors = ["Jeffrey Crane <jediknight11206@gmail.com>"]
 license = "License :: OSI Approved :: MIT License"
 include = ["README.md"]
 packages = [
     { include = "letsdebughelper" },
 ]
```

### Comparing `lets_debug_helper-1.5.3/setup.py` & `lets_debug_helper-1.5.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'six>=1.16.0,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['lets-debug = letsdebughelper.letsdebug:main']}
 
 setup_kwargs = {
     'name': 'lets-debug-helper',
-    'version': '1.5.3',
+    'version': '1.5.4',
     'description': "This is a cli tool that interacts with the Let's Debug API",
     'long_description': 'None',
     'author': 'Jeffrey Crane',
     'author_email': 'jediknight11206@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `lets_debug_helper-1.5.3/PKG-INFO` & `lets_debug_helper-1.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lets-debug-helper
-Version: 1.5.3
+Version: 1.5.4
 Summary: This is a cli tool that interacts with the Let's Debug API
 License: License :: OSI Approved :: MIT License
 Author: Jeffrey Crane
 Author-email: jediknight11206@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

