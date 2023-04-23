# Comparing `tmp/cdk-stacksets-0.0.83.tar.gz` & `tmp/cdk-stacksets-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-stacksets-0.0.83.tar", last modified: Sun Apr 23 00:15:23 2023, max compression
+gzip compressed data, was "cdk-stacksets-0.0.9.tar", last modified: Mon Jan 23 00:16:09 2023, max compression
```

## Comparing `cdk-stacksets-0.0.83.tar` & `cdk-stacksets-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:15:23.023755 cdk-stacksets-0.0.83/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-23 00:15:09.000000 cdk-stacksets-0.0.83/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-23 00:15:09.000000 cdk-stacksets-0.0.83/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12163 2023-04-23 00:15:23.023755 cdk-stacksets-0.0.83/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11249 2023-04-23 00:15:09.000000 cdk-stacksets-0.0.83/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-23 00:15:09.000000 cdk-stacksets-0.0.83/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 00:15:23.023755 cdk-stacksets-0.0.83/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-23 00:15:09.000000 cdk-stacksets-0.0.83/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:15:23.023755 cdk-stacksets-0.0.83/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:15:23.023755 cdk-stacksets-0.0.83/src/cdk_stacksets/
--rw-r--r--   0 runner    (1001) docker     (123)    83981 2023-04-23 00:15:09.000000 cdk-stacksets-0.0.83/src/cdk_stacksets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:15:23.023755 cdk-stacksets-0.0.83/src/cdk_stacksets/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-23 00:15:09.000000 cdk-stacksets-0.0.83/src/cdk_stacksets/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    71051 2023-04-23 00:15:09.000000 cdk-stacksets-0.0.83/src/cdk_stacksets/_jsii/cdk-stacksets@0.0.83.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 00:15:09.000000 cdk-stacksets-0.0.83/src/cdk_stacksets/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:15:23.023755 cdk-stacksets-0.0.83/src/cdk_stacksets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12163 2023-04-23 00:15:22.000000 cdk-stacksets-0.0.83/src/cdk_stacksets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-23 00:15:22.000000 cdk-stacksets-0.0.83/src/cdk_stacksets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 00:15:22.000000 cdk-stacksets-0.0.83/src/cdk_stacksets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-23 00:15:22.000000 cdk-stacksets-0.0.83/src/cdk_stacksets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-23 00:15:22.000000 cdk-stacksets-0.0.83/src/cdk_stacksets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 00:16:09.494084 cdk-stacksets-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-01-23 00:15:55.000000 cdk-stacksets-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-23 00:15:55.000000 cdk-stacksets-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12131 2023-01-23 00:16:09.494084 cdk-stacksets-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11249 2023-01-23 00:15:55.000000 cdk-stacksets-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-01-23 00:15:55.000000 cdk-stacksets-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-23 00:16:09.494084 cdk-stacksets-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-01-23 00:15:55.000000 cdk-stacksets-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 00:16:09.494084 cdk-stacksets-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 00:16:09.494084 cdk-stacksets-0.0.9/src/cdk_stacksets/
+-rw-r--r--   0 runner    (1001) docker     (123)    83981 2023-01-23 00:15:55.000000 cdk-stacksets-0.0.9/src/cdk_stacksets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 00:16:09.494084 cdk-stacksets-0.0.9/src/cdk_stacksets/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-01-23 00:15:55.000000 cdk-stacksets-0.0.9/src/cdk_stacksets/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68654 2023-01-23 00:15:55.000000 cdk-stacksets-0.0.9/src/cdk_stacksets/_jsii/cdk-stacksets@0.0.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-23 00:15:55.000000 cdk-stacksets-0.0.9/src/cdk_stacksets/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 00:16:09.494084 cdk-stacksets-0.0.9/src/cdk_stacksets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12131 2023-01-23 00:16:08.000000 cdk-stacksets-0.0.9/src/cdk_stacksets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-01-23 00:16:09.000000 cdk-stacksets-0.0.9/src/cdk_stacksets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-23 00:16:09.000000 cdk-stacksets-0.0.9/src/cdk_stacksets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-01-23 00:16:09.000000 cdk-stacksets-0.0.9/src/cdk_stacksets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-23 00:16:09.000000 cdk-stacksets-0.0.9/src/cdk_stacksets.egg-info/top_level.txt
```

### Comparing `cdk-stacksets-0.0.83/LICENSE` & `cdk-stacksets-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-stacksets-0.0.83/PKG-INFO` & `cdk-stacksets-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cdk-stacksets
-Version: 0.0.83
+Version: 0.0.9
 Summary: cdk-stacksets
 Home-page: https://github.com/cdklabs/cdk-stacksets.git
 Author: Amazon Web Services<aws-cdk-dev@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-stacksets.git
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -354,7 +354,9 @@
         stackset_name="CDKToolkit-prd",
         initial_bootstrap_target=StackSetTarget.from_organizational_units(
             regions=regions,
             organizational_units=["ou-hrza-bb999427", "ou-hraa-ar111127"]
         )
     ))
 ```
+
+
```

### Comparing `cdk-stacksets-0.0.83/README.md` & `cdk-stacksets-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cdk-stacksets-0.0.83/setup.py` & `cdk-stacksets-0.0.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-stacksets",
-    "version": "0.0.83",
+    "version": "0.0.9",
     "description": "cdk-stacksets",
     "license": "Apache-2.0",
     "url": "https://github.com/cdklabs/cdk-stacksets.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services<aws-cdk-dev@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,38 +22,37 @@
     },
     "packages": [
         "cdk_stacksets",
         "cdk_stacksets._jsii"
     ],
     "package_data": {
         "cdk_stacksets._jsii": [
-            "cdk-stacksets@0.0.83.jsii.tgz"
+            "cdk-stacksets@0.0.9.jsii.tgz"
         ],
         "cdk_stacksets": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "aws-cdk-lib>=2.45.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.80.0, <2.0.0",
+        "jsii>=1.73.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "Development Status :: 4 - Beta",
         "License :: OSI Approved"
     ],
     "scripts": []
 }
 """
```

### Comparing `cdk-stacksets-0.0.83/src/cdk_stacksets/__init__.py` & `cdk-stacksets-0.0.9/src/cdk_stacksets/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-stacksets-0.0.83/src/cdk_stacksets.egg-info/PKG-INFO` & `cdk-stacksets-0.0.9/src/cdk_stacksets.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cdk-stacksets
-Version: 0.0.83
+Version: 0.0.9
 Summary: cdk-stacksets
 Home-page: https://github.com/cdklabs/cdk-stacksets.git
 Author: Amazon Web Services<aws-cdk-dev@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-stacksets.git
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -354,7 +354,9 @@
         stackset_name="CDKToolkit-prd",
         initial_bootstrap_target=StackSetTarget.from_organizational_units(
             regions=regions,
             organizational_units=["ou-hrza-bb999427", "ou-hraa-ar111127"]
         )
     ))
 ```
+
+
```

