# Comparing `tmp/aws-solutions-constructs.aws-fargate-opensearch-2.38.0.tar.gz` & `tmp/aws-solutions-constructs.aws-fargate-opensearch-2.39.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src158235709/src/source/patterns/@aws-solutions-constructs/aws-fargate-opensearch/dist/python/aws-solutions-c", last modified: Sun Apr 16 12:19:30 2023, max compression
+gzip compressed data, was "/codebuild/output/src259931730/src/source/patterns/@aws-solutions-constructs/aws-fargate-opensearch/dist/python/aws-solutions-c", last modified: Sun Apr 23 17:27:38 2023, max compression
```

## Comparing `aws-solutions-constructs.aws-fargate-opensearch-2.38.0.tar` & `aws-solutions-constructs.aws-fargate-opensearch-2.39.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 12:19:30.000000 aws-solutions-constructs.aws-fargate-opensearch-2.38.0/
--rw-r--r--   0 root         (0) root         (0)    10279 2023-04-16 12:19:17.000000 aws-solutions-constructs.aws-fargate-opensearch-2.38.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-04-16 12:19:17.000000 aws-solutions-constructs.aws-fargate-opensearch-2.38.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    11468 2023-04-16 12:19:30.000000 aws-solutions-constructs.aws-fargate-opensearch-2.38.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10519 2023-04-16 12:19:17.000000 aws-solutions-constructs.aws-fargate-opensearch-2.38.0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-04-16 12:19:17.000000 aws-solutions-constructs.aws-fargate-opensearch-2.38.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-16 12:19:30.000000 aws-solutions-constructs.aws-fargate-opensearch-2.38.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1983 2023-04-16 12:19:17.000000 aws-solutions-constructs.aws-fargate-opensearch-2.38.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 12:19:30.000000 aws-solutions-constructs.aws-fargate-opensearch-2.38.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 12:19:30.000000 aws-solutions-constructs.aws-fargate-opensearch-2.38.0/src/aws_solutions_constructs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 12:19:30.000000 aws-solutions-constructs.aws-fargate-opensearch-2.38.0/src/aws_solutions_constructs/aws_fargate_opensearch/
--rw-r--r--   0 root         (0) root         (0)    39513 2023-04-16 12:19:17.000000 aws-solutions-constructs.aws-fargate-opensearch-2.38.0/src/aws_solutions_constructs/aws_fargate_opensearch/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 12:19:30.000000 aws-solutions-constructs.aws-fargate-opensearch-2.38.0/src/aws_solutions_constructs/aws_fargate_opensearch/_jsii/
--rw-r--r--   0 root         (0) root         (0)      495 2023-04-16 12:19:17.000000 aws-solutions-constructs.aws-fargate-opensearch-2.38.0/src/aws_solutions_constructs/aws_fargate_opensearch/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)   106375 2023-04-16 12:19:17.000000 aws-solutions-constructs.aws-fargate-opensearch-2.38.0/src/aws_solutions_constructs/aws_fargate_opensearch/_jsii/aws-fargate-opensearch@2.38.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 12:19:17.000000 aws-solutions-constructs.aws-fargate-opensearch-2.38.0/src/aws_solutions_constructs/aws_fargate_opensearch/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 12:19:30.000000 aws-solutions-constructs.aws-fargate-opensearch-2.38.0/src/aws_solutions_constructs.aws_fargate_opensearch.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11468 2023-04-16 12:19:29.000000 aws-solutions-constructs.aws-fargate-opensearch-2.38.0/src/aws_solutions_constructs.aws_fargate_opensearch.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      719 2023-04-16 12:19:30.000000 aws-solutions-constructs.aws-fargate-opensearch-2.38.0/src/aws_solutions_constructs.aws_fargate_opensearch.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 12:19:29.000000 aws-solutions-constructs.aws-fargate-opensearch-2.38.0/src/aws_solutions_constructs.aws_fargate_opensearch.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      149 2023-04-16 12:19:29.000000 aws-solutions-constructs.aws-fargate-opensearch-2.38.0/src/aws_solutions_constructs.aws_fargate_opensearch.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-04-16 12:19:29.000000 aws-solutions-constructs.aws-fargate-opensearch-2.38.0/src/aws_solutions_constructs.aws_fargate_opensearch.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 17:27:38.000000 aws-solutions-constructs.aws-fargate-opensearch-2.39.0/
+-rw-r--r--   0 root         (0) root         (0)    10279 2023-04-23 17:27:25.000000 aws-solutions-constructs.aws-fargate-opensearch-2.39.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-23 17:27:25.000000 aws-solutions-constructs.aws-fargate-opensearch-2.39.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    11468 2023-04-23 17:27:38.000000 aws-solutions-constructs.aws-fargate-opensearch-2.39.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10519 2023-04-23 17:27:25.000000 aws-solutions-constructs.aws-fargate-opensearch-2.39.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2023-04-23 17:27:25.000000 aws-solutions-constructs.aws-fargate-opensearch-2.39.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-23 17:27:38.000000 aws-solutions-constructs.aws-fargate-opensearch-2.39.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1983 2023-04-23 17:27:25.000000 aws-solutions-constructs.aws-fargate-opensearch-2.39.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 17:27:38.000000 aws-solutions-constructs.aws-fargate-opensearch-2.39.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 17:27:38.000000 aws-solutions-constructs.aws-fargate-opensearch-2.39.0/src/aws_solutions_constructs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 17:27:38.000000 aws-solutions-constructs.aws-fargate-opensearch-2.39.0/src/aws_solutions_constructs/aws_fargate_opensearch/
+-rw-r--r--   0 root         (0) root         (0)    39513 2023-04-23 17:27:25.000000 aws-solutions-constructs.aws-fargate-opensearch-2.39.0/src/aws_solutions_constructs/aws_fargate_opensearch/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 17:27:38.000000 aws-solutions-constructs.aws-fargate-opensearch-2.39.0/src/aws_solutions_constructs/aws_fargate_opensearch/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      495 2023-04-23 17:27:25.000000 aws-solutions-constructs.aws-fargate-opensearch-2.39.0/src/aws_solutions_constructs/aws_fargate_opensearch/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   106374 2023-04-23 17:27:25.000000 aws-solutions-constructs.aws-fargate-opensearch-2.39.0/src/aws_solutions_constructs/aws_fargate_opensearch/_jsii/aws-fargate-opensearch@2.39.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 17:27:25.000000 aws-solutions-constructs.aws-fargate-opensearch-2.39.0/src/aws_solutions_constructs/aws_fargate_opensearch/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 17:27:38.000000 aws-solutions-constructs.aws-fargate-opensearch-2.39.0/src/aws_solutions_constructs.aws_fargate_opensearch.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11468 2023-04-23 17:27:37.000000 aws-solutions-constructs.aws-fargate-opensearch-2.39.0/src/aws_solutions_constructs.aws_fargate_opensearch.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      719 2023-04-23 17:27:37.000000 aws-solutions-constructs.aws-fargate-opensearch-2.39.0/src/aws_solutions_constructs.aws_fargate_opensearch.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 17:27:37.000000 aws-solutions-constructs.aws-fargate-opensearch-2.39.0/src/aws_solutions_constructs.aws_fargate_opensearch.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      149 2023-04-23 17:27:37.000000 aws-solutions-constructs.aws-fargate-opensearch-2.39.0/src/aws_solutions_constructs.aws_fargate_opensearch.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-04-23 17:27:37.000000 aws-solutions-constructs.aws-fargate-opensearch-2.39.0/src/aws_solutions_constructs.aws_fargate_opensearch.egg-info/top_level.txt
```

### Comparing `aws-solutions-constructs.aws-fargate-opensearch-2.38.0/LICENSE` & `aws-solutions-constructs.aws-fargate-opensearch-2.39.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-solutions-constructs.aws-fargate-opensearch-2.38.0/PKG-INFO` & `aws-solutions-constructs.aws-fargate-opensearch-2.39.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-solutions-constructs.aws-fargate-opensearch
-Version: 2.38.0
+Version: 2.39.0
 Summary: CDK Constructs for AWS Fargate to Amazon OpenSearch Service
 Home-page: https://github.com/awslabs/aws-solutions-constructs.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/awslabs/aws-solutions-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-solutions-constructs.aws-fargate-opensearch-2.38.0/README.md` & `aws-solutions-constructs.aws-fargate-opensearch-2.39.0/README.md`

 * *Files identical despite different names*

### Comparing `aws-solutions-constructs.aws-fargate-opensearch-2.38.0/setup.py` & `aws-solutions-constructs.aws-fargate-opensearch-2.39.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-solutions-constructs.aws-fargate-opensearch",
-    "version": "2.38.0",
+    "version": "2.39.0",
     "description": "CDK Constructs for AWS Fargate to Amazon OpenSearch Service",
     "license": "Apache-2.0",
     "url": "https://github.com/awslabs/aws-solutions-constructs.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,24 +22,24 @@
     },
     "packages": [
         "aws_solutions_constructs.aws_fargate_opensearch",
         "aws_solutions_constructs.aws_fargate_opensearch._jsii"
     ],
     "package_data": {
         "aws_solutions_constructs.aws_fargate_opensearch._jsii": [
-            "aws-fargate-opensearch@2.38.0.jsii.tgz"
+            "aws-fargate-opensearch@2.39.0.jsii.tgz"
         ],
         "aws_solutions_constructs.aws_fargate_opensearch": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib>=2.74.0, <3.0.0",
-        "aws-solutions-constructs.core==2.38.0",
+        "aws-cdk-lib>=2.76.0, <3.0.0",
+        "aws-solutions-constructs.core==2.39.0",
         "constructs>=10.0.0, <11.0.0",
         "jsii>=1.80.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
```

### Comparing `aws-solutions-constructs.aws-fargate-opensearch-2.38.0/src/aws_solutions_constructs/aws_fargate_opensearch/__init__.py` & `aws-solutions-constructs.aws-fargate-opensearch-2.39.0/src/aws_solutions_constructs/aws_fargate_opensearch/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-solutions-constructs.aws-fargate-opensearch-2.38.0/src/aws_solutions_constructs.aws_fargate_opensearch.egg-info/PKG-INFO` & `aws-solutions-constructs.aws-fargate-opensearch-2.39.0/src/aws_solutions_constructs.aws_fargate_opensearch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-solutions-constructs.aws-fargate-opensearch
-Version: 2.38.0
+Version: 2.39.0
 Summary: CDK Constructs for AWS Fargate to Amazon OpenSearch Service
 Home-page: https://github.com/awslabs/aws-solutions-constructs.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/awslabs/aws-solutions-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-solutions-constructs.aws-fargate-opensearch-2.38.0/src/aws_solutions_constructs.aws_fargate_opensearch.egg-info/SOURCES.txt` & `aws-solutions-constructs.aws-fargate-opensearch-2.39.0/src/aws_solutions_constructs.aws_fargate_opensearch.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/aws_solutions_constructs.aws_fargate_opensearch.egg-info/SOURCES.txt
 src/aws_solutions_constructs.aws_fargate_opensearch.egg-info/dependency_links.txt
 src/aws_solutions_constructs.aws_fargate_opensearch.egg-info/requires.txt
 src/aws_solutions_constructs.aws_fargate_opensearch.egg-info/top_level.txt
 src/aws_solutions_constructs/aws_fargate_opensearch/__init__.py
 src/aws_solutions_constructs/aws_fargate_opensearch/py.typed
 src/aws_solutions_constructs/aws_fargate_opensearch/_jsii/__init__.py
-src/aws_solutions_constructs/aws_fargate_opensearch/_jsii/aws-fargate-opensearch@2.38.0.jsii.tgz
+src/aws_solutions_constructs/aws_fargate_opensearch/_jsii/aws-fargate-opensearch@2.39.0.jsii.tgz
```

