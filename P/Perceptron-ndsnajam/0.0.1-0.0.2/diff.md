# Comparing `tmp/Perceptron_ndsnajam-0.0.1.tar.gz` & `tmp/Perceptron_ndsnajam-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/DL_Perceptron/DL_Perceptron/dist/.tmp-smqr9vv7/Perceptron_ndsnajam-0.0.1.tar", last modified: Sun Apr 23 05:26:59 2023, max compression
+gzip compressed data, was "/home/runner/work/DL_Perceptron/DL_Perceptron/dist/.tmp-ix3wuvu1/Perceptron_ndsnajam-0.0.2.tar", last modified: Sun Apr 23 05:35:35 2023, max compression
```

## Comparing `Perceptron_ndsnajam-0.0.1.tar` & `Perceptron_ndsnajam-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 05:26:59.000000 Perceptron_ndsnajam-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-23 05:26:48.000000 Perceptron_ndsnajam-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-23 05:26:59.000000 Perceptron_ndsnajam-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-23 05:26:48.000000 Perceptron_ndsnajam-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-23 05:26:48.000000 Perceptron_ndsnajam-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 05:26:59.000000 Perceptron_ndsnajam-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-23 05:26:48.000000 Perceptron_ndsnajam-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 05:26:59.000000 Perceptron_ndsnajam-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 05:26:59.000000 Perceptron_ndsnajam-0.0.1/src/Perceptron_ndsnajam/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 05:26:48.000000 Perceptron_ndsnajam-0.0.1/src/Perceptron_ndsnajam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-04-23 05:26:48.000000 Perceptron_ndsnajam-0.0.1/src/Perceptron_ndsnajam/perceptron.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 05:26:59.000000 Perceptron_ndsnajam-0.0.1/src/Perceptron_ndsnajam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-23 05:26:59.000000 Perceptron_ndsnajam-0.0.1/src/Perceptron_ndsnajam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-23 05:26:59.000000 Perceptron_ndsnajam-0.0.1/src/Perceptron_ndsnajam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 05:26:59.000000 Perceptron_ndsnajam-0.0.1/src/Perceptron_ndsnajam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-23 05:26:59.000000 Perceptron_ndsnajam-0.0.1/src/Perceptron_ndsnajam.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-23 05:26:59.000000 Perceptron_ndsnajam-0.0.1/src/Perceptron_ndsnajam.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 05:35:35.000000 Perceptron_ndsnajam-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-23 05:35:20.000000 Perceptron_ndsnajam-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-23 05:35:35.000000 Perceptron_ndsnajam-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-23 05:35:20.000000 Perceptron_ndsnajam-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-23 05:35:20.000000 Perceptron_ndsnajam-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 05:35:35.000000 Perceptron_ndsnajam-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-23 05:35:20.000000 Perceptron_ndsnajam-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 05:35:35.000000 Perceptron_ndsnajam-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 05:35:35.000000 Perceptron_ndsnajam-0.0.2/src/Perceptron_ndsnajam/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 05:35:20.000000 Perceptron_ndsnajam-0.0.2/src/Perceptron_ndsnajam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-04-23 05:35:20.000000 Perceptron_ndsnajam-0.0.2/src/Perceptron_ndsnajam/perceptron.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 05:35:35.000000 Perceptron_ndsnajam-0.0.2/src/Perceptron_ndsnajam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-23 05:35:35.000000 Perceptron_ndsnajam-0.0.2/src/Perceptron_ndsnajam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-23 05:35:35.000000 Perceptron_ndsnajam-0.0.2/src/Perceptron_ndsnajam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 05:35:35.000000 Perceptron_ndsnajam-0.0.2/src/Perceptron_ndsnajam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-23 05:35:35.000000 Perceptron_ndsnajam-0.0.2/src/Perceptron_ndsnajam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-23 05:35:35.000000 Perceptron_ndsnajam-0.0.2/src/Perceptron_ndsnajam.egg-info/top_level.txt
```

### Comparing `Perceptron_ndsnajam-0.0.1/LICENSE` & `Perceptron_ndsnajam-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Perceptron_ndsnajam-0.0.1/PKG-INFO` & `Perceptron_ndsnajam-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: Perceptron_ndsnajam
-Version: 0.0.1
+Version: 0.0.2
 Summary: Perceptron or/and/xor gates package
-Home-page: https://github.com/nds-najam/Perceptron_ndsnajam
+Home-page: https://github.com/nds-najam/Perceptron-ndsnajam
 Author: nds-najam
 Author-email: najam.iitm@gmail.com
-Project-URL: Bug Tracker, https://github.com/nds-najam/Perceptron_ndsnajam/issues
+Project-URL: Bug Tracker, https://github.com/nds-najam/Perceptron-ndsnajam/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `Perceptron_ndsnajam-0.0.1/setup.py` & `Perceptron_ndsnajam-0.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-PROJECT_NAME = 'Perceptron_ndsnajam'
+PKG_NAME = 'Perceptron_ndsnajam'
 USER_NAME = 'nds-najam'
+PROJECT_NAME = 'Perceptron-ndsnajam'
 
 setuptools.setup(
     name = "Perceptron_ndsnajam",
-    version = "0.0.1",
+    version = "0.0.2",
     author = USER_NAME,
     author_email="najam.iitm@gmail.com",
     description="Perceptron or/and/xor gates package",
     long_description=long_description,
     long_description_content_type = "text/markdown",
     url = f"https://github.com/{USER_NAME}/{PROJECT_NAME}",
     project_urls = {
```

### Comparing `Perceptron_ndsnajam-0.0.1/src/Perceptron_ndsnajam/perceptron.py` & `Perceptron_ndsnajam-0.0.2/src/Perceptron_ndsnajam/perceptron.py`

 * *Files identical despite different names*

### Comparing `Perceptron_ndsnajam-0.0.1/src/Perceptron_ndsnajam.egg-info/PKG-INFO` & `Perceptron_ndsnajam-0.0.2/src/Perceptron_ndsnajam.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: Perceptron-ndsnajam
-Version: 0.0.1
+Version: 0.0.2
 Summary: Perceptron or/and/xor gates package
-Home-page: https://github.com/nds-najam/Perceptron_ndsnajam
+Home-page: https://github.com/nds-najam/Perceptron-ndsnajam
 Author: nds-najam
 Author-email: najam.iitm@gmail.com
-Project-URL: Bug Tracker, https://github.com/nds-najam/Perceptron_ndsnajam/issues
+Project-URL: Bug Tracker, https://github.com/nds-najam/Perceptron-ndsnajam/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

