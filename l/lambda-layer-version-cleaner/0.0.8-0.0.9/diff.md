# Comparing `tmp/lambda-layer-version-cleaner-0.0.8.tar.gz` & `tmp/lambda-layer-version-cleaner-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lambda-layer-version-cleaner-0.0.8.tar", last modified: Thu Apr 13 13:54:53 2023, max compression
+gzip compressed data, was "lambda-layer-version-cleaner-0.0.9.tar", last modified: Sun Apr 23 14:19:34 2023, max compression
```

## Comparing `lambda-layer-version-cleaner-0.0.8.tar` & `lambda-layer-version-cleaner-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:54:53.905728 lambda-layer-version-cleaner-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-13 13:54:39.000000 lambda-layer-version-cleaner-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-13 13:54:39.000000 lambda-layer-version-cleaner-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-04-13 13:54:53.905728 lambda-layer-version-cleaner-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-04-13 13:54:39.000000 lambda-layer-version-cleaner-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-13 13:54:39.000000 lambda-layer-version-cleaner-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 13:54:53.905728 lambda-layer-version-cleaner-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-13 13:54:39.000000 lambda-layer-version-cleaner-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:54:53.901728 lambda-layer-version-cleaner-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:54:53.901728 lambda-layer-version-cleaner-0.0.8/src/lambda_layer_version_cleaner/
--rw-r--r--   0 runner    (1001) docker     (123)    12107 2023-04-13 13:54:39.000000 lambda-layer-version-cleaner-0.0.8/src/lambda_layer_version_cleaner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:54:53.905728 lambda-layer-version-cleaner-0.0.8/src/lambda_layer_version_cleaner/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-13 13:54:39.000000 lambda-layer-version-cleaner-0.0.8/src/lambda_layer_version_cleaner/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28231 2023-04-13 13:54:39.000000 lambda-layer-version-cleaner-0.0.8/src/lambda_layer_version_cleaner/_jsii/lambda-layer-version-cleaner@0.0.8.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 13:54:39.000000 lambda-layer-version-cleaner-0.0.8/src/lambda_layer_version_cleaner/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:54:53.905728 lambda-layer-version-cleaner-0.0.8/src/lambda_layer_version_cleaner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-04-13 13:54:53.000000 lambda-layer-version-cleaner-0.0.8/src/lambda_layer_version_cleaner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-13 13:54:53.000000 lambda-layer-version-cleaner-0.0.8/src/lambda_layer_version_cleaner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 13:54:53.000000 lambda-layer-version-cleaner-0.0.8/src/lambda_layer_version_cleaner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-13 13:54:53.000000 lambda-layer-version-cleaner-0.0.8/src/lambda_layer_version_cleaner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-13 13:54:53.000000 lambda-layer-version-cleaner-0.0.8/src/lambda_layer_version_cleaner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:19:34.379365 lambda-layer-version-cleaner-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-23 14:19:19.000000 lambda-layer-version-cleaner-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-23 14:19:19.000000 lambda-layer-version-cleaner-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-04-23 14:19:34.379365 lambda-layer-version-cleaner-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-04-23 14:19:19.000000 lambda-layer-version-cleaner-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-23 14:19:19.000000 lambda-layer-version-cleaner-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 14:19:34.379365 lambda-layer-version-cleaner-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-23 14:19:19.000000 lambda-layer-version-cleaner-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:19:34.379365 lambda-layer-version-cleaner-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:19:34.379365 lambda-layer-version-cleaner-0.0.9/src/lambda_layer_version_cleaner/
+-rw-r--r--   0 runner    (1001) docker     (123)    12107 2023-04-23 14:19:19.000000 lambda-layer-version-cleaner-0.0.9/src/lambda_layer_version_cleaner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:19:34.379365 lambda-layer-version-cleaner-0.0.9/src/lambda_layer_version_cleaner/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-23 14:19:19.000000 lambda-layer-version-cleaner-0.0.9/src/lambda_layer_version_cleaner/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28208 2023-04-23 14:19:19.000000 lambda-layer-version-cleaner-0.0.9/src/lambda_layer_version_cleaner/_jsii/lambda-layer-version-cleaner@0.0.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 14:19:19.000000 lambda-layer-version-cleaner-0.0.9/src/lambda_layer_version_cleaner/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:19:34.379365 lambda-layer-version-cleaner-0.0.9/src/lambda_layer_version_cleaner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-04-23 14:19:34.000000 lambda-layer-version-cleaner-0.0.9/src/lambda_layer_version_cleaner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-23 14:19:34.000000 lambda-layer-version-cleaner-0.0.9/src/lambda_layer_version_cleaner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 14:19:34.000000 lambda-layer-version-cleaner-0.0.9/src/lambda_layer_version_cleaner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-23 14:19:34.000000 lambda-layer-version-cleaner-0.0.9/src/lambda_layer_version_cleaner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-23 14:19:34.000000 lambda-layer-version-cleaner-0.0.9/src/lambda_layer_version_cleaner.egg-info/top_level.txt
```

### Comparing `lambda-layer-version-cleaner-0.0.8/LICENSE` & `lambda-layer-version-cleaner-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lambda-layer-version-cleaner-0.0.8/PKG-INFO` & `lambda-layer-version-cleaner-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambda-layer-version-cleaner
-Version: 0.0.8
+Version: 0.0.9
 Summary: lambda-layer-version-cleaner is a CDK Construct that helps you manage and automatically clean up old versions of AWS Lambda Layers.
 Home-page: https://github.com/unirt/lambda-layer-version-cleaner.git
 Author: unirt<lunirtc@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/unirt/lambda-layer-version-cleaner.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `lambda-layer-version-cleaner-0.0.8/README.md` & `lambda-layer-version-cleaner-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `lambda-layer-version-cleaner-0.0.8/setup.py` & `lambda-layer-version-cleaner-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "lambda-layer-version-cleaner",
-    "version": "0.0.8",
+    "version": "0.0.9",
     "description": "lambda-layer-version-cleaner is a CDK Construct that helps you manage and automatically clean up old versions of AWS Lambda Layers.",
     "license": "Apache-2.0",
     "url": "https://github.com/unirt/lambda-layer-version-cleaner.git",
     "long_description_content_type": "text/markdown",
     "author": "unirt<lunirtc@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "lambda_layer_version_cleaner",
         "lambda_layer_version_cleaner._jsii"
     ],
     "package_data": {
         "lambda_layer_version_cleaner._jsii": [
-            "lambda-layer-version-cleaner@0.0.8.jsii.tgz"
+            "lambda-layer-version-cleaner@0.0.9.jsii.tgz"
         ],
         "lambda_layer_version_cleaner": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `lambda-layer-version-cleaner-0.0.8/src/lambda_layer_version_cleaner/__init__.py` & `lambda-layer-version-cleaner-0.0.9/src/lambda_layer_version_cleaner/__init__.py`

 * *Files identical despite different names*

### Comparing `lambda-layer-version-cleaner-0.0.8/src/lambda_layer_version_cleaner.egg-info/PKG-INFO` & `lambda-layer-version-cleaner-0.0.9/src/lambda_layer_version_cleaner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambda-layer-version-cleaner
-Version: 0.0.8
+Version: 0.0.9
 Summary: lambda-layer-version-cleaner is a CDK Construct that helps you manage and automatically clean up old versions of AWS Lambda Layers.
 Home-page: https://github.com/unirt/lambda-layer-version-cleaner.git
 Author: unirt<lunirtc@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/unirt/lambda-layer-version-cleaner.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `lambda-layer-version-cleaner-0.0.8/src/lambda_layer_version_cleaner.egg-info/SOURCES.txt` & `lambda-layer-version-cleaner-0.0.9/src/lambda_layer_version_cleaner.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/lambda_layer_version_cleaner/py.typed
 src/lambda_layer_version_cleaner.egg-info/PKG-INFO
 src/lambda_layer_version_cleaner.egg-info/SOURCES.txt
 src/lambda_layer_version_cleaner.egg-info/dependency_links.txt
 src/lambda_layer_version_cleaner.egg-info/requires.txt
 src/lambda_layer_version_cleaner.egg-info/top_level.txt
 src/lambda_layer_version_cleaner/_jsii/__init__.py
-src/lambda_layer_version_cleaner/_jsii/lambda-layer-version-cleaner@0.0.8.jsii.tgz
+src/lambda_layer_version_cleaner/_jsii/lambda-layer-version-cleaner@0.0.9.jsii.tgz
```

