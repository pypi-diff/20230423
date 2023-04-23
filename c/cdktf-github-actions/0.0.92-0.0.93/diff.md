# Comparing `tmp/cdktf-github-actions-0.0.92.tar.gz` & `tmp/cdktf-github-actions-0.0.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-github-actions-0.0.92.tar", last modified: Fri Apr 21 00:27:44 2023, max compression
+gzip compressed data, was "cdktf-github-actions-0.0.93.tar", last modified: Sat Apr 22 00:28:02 2023, max compression
```

## Comparing `cdktf-github-actions-0.0.92.tar` & `cdktf-github-actions-0.0.93.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:27:44.801852 cdktf-github-actions-0.0.92/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-21 00:27:29.000000 cdktf-github-actions-0.0.92/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-21 00:27:29.000000 cdktf-github-actions-0.0.92/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-04-21 00:27:44.801852 cdktf-github-actions-0.0.92/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-21 00:27:29.000000 cdktf-github-actions-0.0.92/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-21 00:27:29.000000 cdktf-github-actions-0.0.92/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 00:27:44.801852 cdktf-github-actions-0.0.92/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-21 00:27:29.000000 cdktf-github-actions-0.0.92/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:27:44.797852 cdktf-github-actions-0.0.92/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:27:44.801852 cdktf-github-actions-0.0.92/src/cdktf_github-actions/
--rw-r--r--   0 runner    (1001) docker     (123)   190483 2023-04-21 00:27:29.000000 cdktf-github-actions-0.0.92/src/cdktf_github-actions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:27:44.801852 cdktf-github-actions-0.0.92/src/cdktf_github-actions/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-21 00:27:29.000000 cdktf-github-actions-0.0.92/src/cdktf_github-actions/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   189727 2023-04-21 00:27:29.000000 cdktf-github-actions-0.0.92/src/cdktf_github-actions/_jsii/cdktf-github-actions@0.0.92.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 00:27:29.000000 cdktf-github-actions-0.0.92/src/cdktf_github-actions/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:27:44.801852 cdktf-github-actions-0.0.92/src/cdktf_github_actions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-04-21 00:27:44.000000 cdktf-github-actions-0.0.92/src/cdktf_github_actions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-21 00:27:44.000000 cdktf-github-actions-0.0.92/src/cdktf_github_actions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 00:27:44.000000 cdktf-github-actions-0.0.92/src/cdktf_github_actions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-21 00:27:44.000000 cdktf-github-actions-0.0.92/src/cdktf_github_actions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-21 00:27:44.000000 cdktf-github-actions-0.0.92/src/cdktf_github_actions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:28:02.217387 cdktf-github-actions-0.0.93/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-22 00:27:51.000000 cdktf-github-actions-0.0.93/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-22 00:27:51.000000 cdktf-github-actions-0.0.93/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-04-22 00:28:02.217387 cdktf-github-actions-0.0.93/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-22 00:27:51.000000 cdktf-github-actions-0.0.93/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-22 00:27:51.000000 cdktf-github-actions-0.0.93/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 00:28:02.217387 cdktf-github-actions-0.0.93/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-22 00:27:51.000000 cdktf-github-actions-0.0.93/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:28:02.217387 cdktf-github-actions-0.0.93/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:28:02.217387 cdktf-github-actions-0.0.93/src/cdktf_github-actions/
+-rw-r--r--   0 runner    (1001) docker     (123)   190483 2023-04-22 00:27:51.000000 cdktf-github-actions-0.0.93/src/cdktf_github-actions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:28:02.217387 cdktf-github-actions-0.0.93/src/cdktf_github-actions/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-22 00:27:51.000000 cdktf-github-actions-0.0.93/src/cdktf_github-actions/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   189726 2023-04-22 00:27:51.000000 cdktf-github-actions-0.0.93/src/cdktf_github-actions/_jsii/cdktf-github-actions@0.0.93.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 00:27:51.000000 cdktf-github-actions-0.0.93/src/cdktf_github-actions/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:28:02.217387 cdktf-github-actions-0.0.93/src/cdktf_github_actions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-04-22 00:28:02.000000 cdktf-github-actions-0.0.93/src/cdktf_github_actions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-22 00:28:02.000000 cdktf-github-actions-0.0.93/src/cdktf_github_actions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 00:28:02.000000 cdktf-github-actions-0.0.93/src/cdktf_github_actions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-22 00:28:02.000000 cdktf-github-actions-0.0.93/src/cdktf_github_actions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-22 00:28:02.000000 cdktf-github-actions-0.0.93/src/cdktf_github_actions.egg-info/top_level.txt
```

### Comparing `cdktf-github-actions-0.0.92/LICENSE` & `cdktf-github-actions-0.0.93/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-github-actions-0.0.92/PKG-INFO` & `cdktf-github-actions-0.0.93/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-github-actions
-Version: 0.0.92
+Version: 0.0.93
 Summary: @awlsring/cdktf-github-actions
 Home-page: https://github.com/awlsring/cdktf-github-actions.git
 Author: awlsring<mattcanemail@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/awlsring/cdktf-github-actions.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-github-actions-0.0.92/README.md` & `cdktf-github-actions-0.0.93/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-github-actions-0.0.92/setup.py` & `cdktf-github-actions-0.0.93/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-github-actions",
-    "version": "0.0.92",
+    "version": "0.0.93",
     "description": "@awlsring/cdktf-github-actions",
     "license": "Apache-2.0",
     "url": "https://github.com/awlsring/cdktf-github-actions.git",
     "long_description_content_type": "text/markdown",
     "author": "awlsring<mattcanemail@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdktf_github-actions",
         "cdktf_github-actions._jsii"
     ],
     "package_data": {
         "cdktf_github-actions._jsii": [
-            "cdktf-github-actions@0.0.92.jsii.tgz"
+            "cdktf-github-actions@0.0.93.jsii.tgz"
         ],
         "cdktf_github-actions": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdktf-github-actions-0.0.92/src/cdktf_github-actions/__init__.py` & `cdktf-github-actions-0.0.93/src/cdktf_github-actions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-github-actions-0.0.92/src/cdktf_github_actions.egg-info/PKG-INFO` & `cdktf-github-actions-0.0.93/src/cdktf_github_actions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-github-actions
-Version: 0.0.92
+Version: 0.0.93
 Summary: @awlsring/cdktf-github-actions
 Home-page: https://github.com/awlsring/cdktf-github-actions.git
 Author: awlsring<mattcanemail@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/awlsring/cdktf-github-actions.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

