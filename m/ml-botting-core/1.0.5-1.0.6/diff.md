# Comparing `tmp/ml_botting_core-1.0.5.tar.gz` & `tmp/ml_botting_core-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml_botting_core-1.0.5.tar", last modified: Sun Apr 23 16:16:24 2023, max compression
+gzip compressed data, was "ml_botting_core-1.0.6.tar", last modified: Sun Apr 23 16:28:27 2023, max compression
```

## Comparing `ml_botting_core-1.0.5.tar` & `ml_botting_core-1.0.6.tar`

### file list

```diff
@@ -1,31 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:16:23.998342 ml_botting_core-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-23 16:15:03.000000 ml_botting_core-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-04-23 16:16:23.998342 ml_botting_core-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-04-23 16:15:03.000000 ml_botting_core-1.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-23 16:15:03.000000 ml_botting_core-1.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-23 16:16:23.998342 ml_botting_core-1.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:16:23.990342 ml_botting_core-1.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:16:23.994342 ml_botting_core-1.0.5/src/ml_botting_core/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-23 16:15:03.000000 ml_botting_core-1.0.5/src/ml_botting_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-04-23 16:15:03.000000 ml_botting_core-1.0.5/src/ml_botting_core/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:16:23.994342 ml_botting_core-1.0.5/src/ml_botting_core/classification/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 16:15:03.000000 ml_botting_core-1.0.5/src/ml_botting_core/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-04-23 16:15:03.000000 ml_botting_core-1.0.5/src/ml_botting_core/classification/universal_classifier_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:16:23.994342 ml_botting_core-1.0.5/src/ml_botting_core/model_management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 16:15:03.000000 ml_botting_core-1.0.5/src/ml_botting_core/model_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-23 16:15:03.000000 ml_botting_core-1.0.5/src/ml_botting_core/model_management/download_models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 16:15:03.000000 ml_botting_core-1.0.5/src/ml_botting_core/model_management/load_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-04-23 16:15:03.000000 ml_botting_core-1.0.5/src/ml_botting_core/model_management/model_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:16:23.994342 ml_botting_core-1.0.5/src/ml_botting_core/prediction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 16:15:03.000000 ml_botting_core-1.0.5/src/ml_botting_core/prediction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-04-23 16:15:03.000000 ml_botting_core-1.0.5/src/ml_botting_core/prediction/prediction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:16:23.994342 ml_botting_core-1.0.5/src/ml_botting_core/regression/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 16:15:03.000000 ml_botting_core-1.0.5/src/ml_botting_core/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 16:15:03.000000 ml_botting_core-1.0.5/src/ml_botting_core/regression/universal_regressor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:16:23.994342 ml_botting_core-1.0.5/src/ml_botting_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-04-23 16:16:23.000000 ml_botting_core-1.0.5/src/ml_botting_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-23 16:16:23.000000 ml_botting_core-1.0.5/src/ml_botting_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 16:16:23.000000 ml_botting_core-1.0.5/src/ml_botting_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-23 16:16:23.000000 ml_botting_core-1.0.5/src/ml_botting_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:16:23.998342 ml_botting_core-1.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-23 16:15:03.000000 ml_botting_core-1.0.5/tests/test_universal_predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:28:27.522061 ml_botting_core-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-23 16:26:56.000000 ml_botting_core-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-04-23 16:28:27.522061 ml_botting_core-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-04-23 16:26:56.000000 ml_botting_core-1.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-23 16:26:56.000000 ml_botting_core-1.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-23 16:28:27.522061 ml_botting_core-1.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:28:27.514060 ml_botting_core-1.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:28:27.518060 ml_botting_core-1.0.6/src/ml_botting_core/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-23 16:26:56.000000 ml_botting_core-1.0.6/src/ml_botting_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-04-23 16:26:56.000000 ml_botting_core-1.0.6/src/ml_botting_core/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:28:27.518060 ml_botting_core-1.0.6/src/ml_botting_core/classification/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 16:26:56.000000 ml_botting_core-1.0.6/src/ml_botting_core/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-04-23 16:26:56.000000 ml_botting_core-1.0.6/src/ml_botting_core/classification/universal_classifier_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:28:27.518060 ml_botting_core-1.0.6/src/ml_botting_core/general/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 16:26:56.000000 ml_botting_core-1.0.6/src/ml_botting_core/general/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-23 16:26:56.000000 ml_botting_core-1.0.6/src/ml_botting_core/general/general.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:28:27.518060 ml_botting_core-1.0.6/src/ml_botting_core/model_management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 16:26:56.000000 ml_botting_core-1.0.6/src/ml_botting_core/model_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-23 16:26:56.000000 ml_botting_core-1.0.6/src/ml_botting_core/model_management/download_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 16:26:56.000000 ml_botting_core-1.0.6/src/ml_botting_core/model_management/load_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-04-23 16:26:56.000000 ml_botting_core-1.0.6/src/ml_botting_core/model_management/model_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:28:27.522061 ml_botting_core-1.0.6/src/ml_botting_core/prediction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 16:26:56.000000 ml_botting_core-1.0.6/src/ml_botting_core/prediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-23 16:26:56.000000 ml_botting_core-1.0.6/src/ml_botting_core/prediction/prediction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:28:27.522061 ml_botting_core-1.0.6/src/ml_botting_core/regression/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 16:26:56.000000 ml_botting_core-1.0.6/src/ml_botting_core/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 16:26:56.000000 ml_botting_core-1.0.6/src/ml_botting_core/regression/universal_regressor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:28:27.518060 ml_botting_core-1.0.6/src/ml_botting_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-04-23 16:28:27.000000 ml_botting_core-1.0.6/src/ml_botting_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-23 16:28:27.000000 ml_botting_core-1.0.6/src/ml_botting_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 16:28:27.000000 ml_botting_core-1.0.6/src/ml_botting_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-23 16:28:27.000000 ml_botting_core-1.0.6/src/ml_botting_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:28:27.522061 ml_botting_core-1.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-23 16:26:56.000000 ml_botting_core-1.0.6/tests/test_universal_predictor.py
```

### Comparing `ml_botting_core-1.0.5/LICENSE` & `ml_botting_core-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ml_botting_core-1.0.5/PKG-INFO` & `ml_botting_core-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml_botting_core
-Version: 1.0.5
+Version: 1.0.6
 Summary: Making ML more accessible to botting apps. Solving Complex UI Challenges w/ ML.
 Home-page: https://github.com/darkmatter2222/ml_botting_core
 Author: Ryan Susman
 Author-email: ryansusman@gmail.com
 Project-URL: Bug Tracker, https://github.com/darkmatter2222/ml_botting_core/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml_botting_core-1.0.5/README.md` & `ml_botting_core-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ml_botting_core-1.0.5/setup.cfg` & `ml_botting_core-1.0.6/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ml_botting_core
-version = 1.0.5
+version = 1.0.6
 author = Ryan Susman
 author_email = ryansusman@gmail.com
 description = Making ML more accessible to botting apps. Solving Complex UI Challenges w/ ML.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/darkmatter2222/ml_botting_core
 project_urls =
```

### Comparing `ml_botting_core-1.0.5/src/ml_botting_core/base.py` & `ml_botting_core-1.0.6/src/ml_botting_core/base.py`

 * *Files identical despite different names*

### Comparing `ml_botting_core-1.0.5/src/ml_botting_core/classification/universal_classifier_trainer.py` & `ml_botting_core-1.0.6/src/ml_botting_core/classification/universal_classifier_trainer.py`

 * *Files identical despite different names*

### Comparing `ml_botting_core-1.0.5/src/ml_botting_core/model_management/download_models.py` & `ml_botting_core-1.0.6/src/ml_botting_core/model_management/download_models.py`

 * *Files identical despite different names*

### Comparing `ml_botting_core-1.0.5/src/ml_botting_core/model_management/model_manager.py` & `ml_botting_core-1.0.6/src/ml_botting_core/model_management/model_manager.py`

 * *Files identical despite different names*

### Comparing `ml_botting_core-1.0.5/src/ml_botting_core/prediction/prediction.py` & `ml_botting_core-1.0.6/src/ml_botting_core/prediction/prediction.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import json
 import datetime
 import os
 import time
 
 from ..general.general import mkdir_p
 
-
 def write_json(new_data, filename):
     if not os.path.isfile(filename):
         file = open(filename, 'w+')
         file.write(json.dumps({"results": []}, indent=1))
         file.close()
         time.sleep(0.1)
```

### Comparing `ml_botting_core-1.0.5/src/ml_botting_core.egg-info/PKG-INFO` & `ml_botting_core-1.0.6/src/ml_botting_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-botting-core
-Version: 1.0.5
+Version: 1.0.6
 Summary: Making ML more accessible to botting apps. Solving Complex UI Challenges w/ ML.
 Home-page: https://github.com/darkmatter2222/ml_botting_core
 Author: Ryan Susman
 Author-email: ryansusman@gmail.com
 Project-URL: Bug Tracker, https://github.com/darkmatter2222/ml_botting_core/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml_botting_core-1.0.5/src/ml_botting_core.egg-info/SOURCES.txt` & `ml_botting_core-1.0.6/src/ml_botting_core.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 src/ml_botting_core/base.py
 src/ml_botting_core.egg-info/PKG-INFO
 src/ml_botting_core.egg-info/SOURCES.txt
 src/ml_botting_core.egg-info/dependency_links.txt
 src/ml_botting_core.egg-info/top_level.txt
 src/ml_botting_core/classification/__init__.py
 src/ml_botting_core/classification/universal_classifier_trainer.py
+src/ml_botting_core/general/__init__.py
+src/ml_botting_core/general/general.py
 src/ml_botting_core/model_management/__init__.py
 src/ml_botting_core/model_management/download_models.py
 src/ml_botting_core/model_management/load_models.py
 src/ml_botting_core/model_management/model_manager.py
 src/ml_botting_core/prediction/__init__.py
 src/ml_botting_core/prediction/prediction.py
 src/ml_botting_core/regression/__init__.py
```

