# Comparing `tmp/cdk8s-plus-26-2.3.4.tar.gz` & `tmp/cdk8s-plus-26-2.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk8s-plus-26-2.3.4.tar", last modified: Fri Apr 21 02:29:46 2023, max compression
+gzip compressed data, was "cdk8s-plus-26-2.3.5.tar", last modified: Sat Apr 22 02:27:22 2023, max compression
```

## Comparing `cdk8s-plus-26-2.3.4.tar` & `cdk8s-plus-26-2.3.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:29:46.201139 cdk8s-plus-26-2.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-21 02:29:30.000000 cdk8s-plus-26-2.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-21 02:29:30.000000 cdk8s-plus-26-2.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-21 02:29:30.000000 cdk8s-plus-26-2.3.4/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-04-21 02:29:46.201139 cdk8s-plus-26-2.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-04-21 02:29:30.000000 cdk8s-plus-26-2.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-21 02:29:30.000000 cdk8s-plus-26-2.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 02:29:46.201139 cdk8s-plus-26-2.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-21 02:29:30.000000 cdk8s-plus-26-2.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:29:46.193139 cdk8s-plus-26-2.3.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:29:46.197139 cdk8s-plus-26-2.3.4/src/cdk8s_plus_26/
--rw-r--r--   0 runner    (1001) docker     (123)  1130341 2023-04-21 02:29:30.000000 cdk8s-plus-26-2.3.4/src/cdk8s_plus_26/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:29:46.197139 cdk8s-plus-26-2.3.4/src/cdk8s_plus_26/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-21 02:29:30.000000 cdk8s-plus-26-2.3.4/src/cdk8s_plus_26/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1285671 2023-04-21 02:29:30.000000 cdk8s-plus-26-2.3.4/src/cdk8s_plus_26/_jsii/cdk8s-plus-26@2.3.4.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:29:46.197139 cdk8s-plus-26-2.3.4/src/cdk8s_plus_26/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)  2771385 2023-04-21 02:29:30.000000 cdk8s-plus-26-2.3.4/src/cdk8s_plus_26/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 02:29:30.000000 cdk8s-plus-26-2.3.4/src/cdk8s_plus_26/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:29:46.197139 cdk8s-plus-26-2.3.4/src/cdk8s_plus_26.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-04-21 02:29:46.000000 cdk8s-plus-26-2.3.4/src/cdk8s_plus_26.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-21 02:29:46.000000 cdk8s-plus-26-2.3.4/src/cdk8s_plus_26.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 02:29:46.000000 cdk8s-plus-26-2.3.4/src/cdk8s_plus_26.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-21 02:29:46.000000 cdk8s-plus-26-2.3.4/src/cdk8s_plus_26.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-21 02:29:46.000000 cdk8s-plus-26-2.3.4/src/cdk8s_plus_26.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 02:27:22.891605 cdk8s-plus-26-2.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-22 02:27:10.000000 cdk8s-plus-26-2.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-22 02:27:10.000000 cdk8s-plus-26-2.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-22 02:27:10.000000 cdk8s-plus-26-2.3.5/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-04-22 02:27:22.891605 cdk8s-plus-26-2.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-04-22 02:27:10.000000 cdk8s-plus-26-2.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-22 02:27:10.000000 cdk8s-plus-26-2.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 02:27:22.891605 cdk8s-plus-26-2.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-22 02:27:10.000000 cdk8s-plus-26-2.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 02:27:22.883605 cdk8s-plus-26-2.3.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 02:27:22.887605 cdk8s-plus-26-2.3.5/src/cdk8s_plus_26/
+-rw-r--r--   0 runner    (1001) docker     (123)  1130341 2023-04-22 02:27:10.000000 cdk8s-plus-26-2.3.5/src/cdk8s_plus_26/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 02:27:22.887605 cdk8s-plus-26-2.3.5/src/cdk8s_plus_26/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-22 02:27:10.000000 cdk8s-plus-26-2.3.5/src/cdk8s_plus_26/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1285676 2023-04-22 02:27:10.000000 cdk8s-plus-26-2.3.5/src/cdk8s_plus_26/_jsii/cdk8s-plus-26@2.3.5.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 02:27:22.891605 cdk8s-plus-26-2.3.5/src/cdk8s_plus_26/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)  2771385 2023-04-22 02:27:10.000000 cdk8s-plus-26-2.3.5/src/cdk8s_plus_26/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 02:27:10.000000 cdk8s-plus-26-2.3.5/src/cdk8s_plus_26/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 02:27:22.887605 cdk8s-plus-26-2.3.5/src/cdk8s_plus_26.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-04-22 02:27:22.000000 cdk8s-plus-26-2.3.5/src/cdk8s_plus_26.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-22 02:27:22.000000 cdk8s-plus-26-2.3.5/src/cdk8s_plus_26.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 02:27:22.000000 cdk8s-plus-26-2.3.5/src/cdk8s_plus_26.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-22 02:27:22.000000 cdk8s-plus-26-2.3.5/src/cdk8s_plus_26.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-22 02:27:22.000000 cdk8s-plus-26-2.3.5/src/cdk8s_plus_26.egg-info/top_level.txt
```

### Comparing `cdk8s-plus-26-2.3.4/LICENSE` & `cdk8s-plus-26-2.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-26-2.3.4/PKG-INFO` & `cdk8s-plus-26-2.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-plus-26
-Version: 2.3.4
+Version: 2.3.5
 Summary: cdk8s+ is a software development framework that provides high level abstractions for authoring Kubernetes applications. cdk8s-plus-26 synthesizes Kubernetes manifests for Kubernetes 1.26.0
 Home-page: https://github.com/cdk8s-team/cdk8s-plus.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-plus.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk8s-plus-26-2.3.4/README.md` & `cdk8s-plus-26-2.3.5/README.md`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-26-2.3.4/setup.py` & `cdk8s-plus-26-2.3.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk8s-plus-26",
-    "version": "2.3.4",
+    "version": "2.3.5",
     "description": "cdk8s+ is a software development framework that provides high level abstractions for authoring Kubernetes applications. cdk8s-plus-26 synthesizes Kubernetes manifests for Kubernetes 1.26.0",
     "license": "Apache-2.0",
     "url": "https://github.com/cdk8s-team/cdk8s-plus.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -23,24 +23,24 @@
     "packages": [
         "cdk8s_plus_26",
         "cdk8s_plus_26._jsii",
         "cdk8s_plus_26.k8s"
     ],
     "package_data": {
         "cdk8s_plus_26._jsii": [
-            "cdk8s-plus-26@2.3.4.jsii.tgz"
+            "cdk8s-plus-26@2.3.5.jsii.tgz"
         ],
         "cdk8s_plus_26": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "cdk8s>=2.7.56, <3.0.0",
-        "constructs>=10.2.2, <11.0.0",
+        "constructs>=10.2.3, <11.0.0",
         "jsii>=1.80.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
```

### Comparing `cdk8s-plus-26-2.3.4/src/cdk8s_plus_26/__init__.py` & `cdk8s-plus-26-2.3.5/src/cdk8s_plus_26/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-26-2.3.4/src/cdk8s_plus_26/k8s/__init__.py` & `cdk8s-plus-26-2.3.5/src/cdk8s_plus_26/k8s/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-26-2.3.4/src/cdk8s_plus_26.egg-info/PKG-INFO` & `cdk8s-plus-26-2.3.5/src/cdk8s_plus_26.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-plus-26
-Version: 2.3.4
+Version: 2.3.5
 Summary: cdk8s+ is a software development framework that provides high level abstractions for authoring Kubernetes applications. cdk8s-plus-26 synthesizes Kubernetes manifests for Kubernetes 1.26.0
 Home-page: https://github.com/cdk8s-team/cdk8s-plus.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-plus.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

