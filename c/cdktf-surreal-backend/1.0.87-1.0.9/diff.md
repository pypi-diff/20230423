# Comparing `tmp/cdktf-surreal-backend-1.0.87.tar.gz` & `tmp/cdktf-surreal-backend-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-surreal-backend-1.0.87.tar", last modified: Sat Apr 22 00:18:40 2023, max compression
+gzip compressed data, was "cdktf-surreal-backend-1.0.9.tar", last modified: Tue Jan 31 01:14:28 2023, max compression
```

## Comparing `cdktf-surreal-backend-1.0.87.tar` & `cdktf-surreal-backend-1.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:18:40.403282 cdktf-surreal-backend-1.0.87/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-22 00:18:24.000000 cdktf-surreal-backend-1.0.87/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-22 00:18:24.000000 cdktf-surreal-backend-1.0.87/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-22 00:18:40.403282 cdktf-surreal-backend-1.0.87/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-22 00:18:24.000000 cdktf-surreal-backend-1.0.87/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-22 00:18:24.000000 cdktf-surreal-backend-1.0.87/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 00:18:40.403282 cdktf-surreal-backend-1.0.87/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-04-22 00:18:24.000000 cdktf-surreal-backend-1.0.87/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:18:40.403282 cdktf-surreal-backend-1.0.87/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:18:40.403282 cdktf-surreal-backend-1.0.87/src/cdktf_surreal-backend/
--rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-04-22 00:18:24.000000 cdktf-surreal-backend-1.0.87/src/cdktf_surreal-backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:18:40.403282 cdktf-surreal-backend-1.0.87/src/cdktf_surreal-backend/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-22 00:18:24.000000 cdktf-surreal-backend-1.0.87/src/cdktf_surreal-backend/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10998 2023-04-22 00:18:24.000000 cdktf-surreal-backend-1.0.87/src/cdktf_surreal-backend/_jsii/cdktf-surreal-backend@1.0.87.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 00:18:24.000000 cdktf-surreal-backend-1.0.87/src/cdktf_surreal-backend/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:18:40.403282 cdktf-surreal-backend-1.0.87/src/cdktf_surreal_backend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-22 00:18:40.000000 cdktf-surreal-backend-1.0.87/src/cdktf_surreal_backend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-22 00:18:40.000000 cdktf-surreal-backend-1.0.87/src/cdktf_surreal_backend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 00:18:40.000000 cdktf-surreal-backend-1.0.87/src/cdktf_surreal_backend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-22 00:18:40.000000 cdktf-surreal-backend-1.0.87/src/cdktf_surreal_backend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-22 00:18:40.000000 cdktf-surreal-backend-1.0.87/src/cdktf_surreal_backend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 01:14:28.484941 cdktf-surreal-backend-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-01-31 01:14:09.000000 cdktf-surreal-backend-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-31 01:14:09.000000 cdktf-surreal-backend-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-01-31 01:14:28.484941 cdktf-surreal-backend-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-01-31 01:14:09.000000 cdktf-surreal-backend-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-01-31 01:14:09.000000 cdktf-surreal-backend-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-31 01:14:28.484941 cdktf-surreal-backend-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-01-31 01:14:09.000000 cdktf-surreal-backend-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 01:14:28.484941 cdktf-surreal-backend-1.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 01:14:28.484941 cdktf-surreal-backend-1.0.9/src/cdktf_surreal-backend/
+-rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-01-31 01:14:09.000000 cdktf-surreal-backend-1.0.9/src/cdktf_surreal-backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 01:14:28.484941 cdktf-surreal-backend-1.0.9/src/cdktf_surreal-backend/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-01-31 01:14:09.000000 cdktf-surreal-backend-1.0.9/src/cdktf_surreal-backend/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11054 2023-01-31 01:14:09.000000 cdktf-surreal-backend-1.0.9/src/cdktf_surreal-backend/_jsii/cdktf-surreal-backend@1.0.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 01:14:09.000000 cdktf-surreal-backend-1.0.9/src/cdktf_surreal-backend/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 01:14:28.484941 cdktf-surreal-backend-1.0.9/src/cdktf_surreal_backend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-01-31 01:14:27.000000 cdktf-surreal-backend-1.0.9/src/cdktf_surreal_backend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-01-31 01:14:28.000000 cdktf-surreal-backend-1.0.9/src/cdktf_surreal_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 01:14:27.000000 cdktf-surreal-backend-1.0.9/src/cdktf_surreal_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-01-31 01:14:28.000000 cdktf-surreal-backend-1.0.9/src/cdktf_surreal_backend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-31 01:14:28.000000 cdktf-surreal-backend-1.0.9/src/cdktf_surreal_backend.egg-info/top_level.txt
```

### Comparing `cdktf-surreal-backend-1.0.87/LICENSE` & `cdktf-surreal-backend-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-surreal-backend-1.0.87/PKG-INFO` & `cdktf-surreal-backend-1.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cdktf-surreal-backend
-Version: 1.0.87
+Version: 1.0.9
 Summary: A package that vends a construct to setup the surreal backend in CDKTF
 Home-page: https://github.com/awlsring/cdktf-surreal-backend.git
 Author: awlsring<mattcanemail@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/awlsring/cdktf-surreal-backend.git
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
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -55,7 +55,9 @@
 ### Construct Properties:
 
 * address: The address your backend sever is reachable at.
 * project: The project name to use for this stack.
 * stack: The stack name to use for this stack. stacks names must be unique across a project.
 * username: The username to use for authentication, configured in the server's config.yaml file
 * password: The password to use for authentication, configured in the server's config.yaml file
+
+
```

### Comparing `cdktf-surreal-backend-1.0.87/README.md` & `cdktf-surreal-backend-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-surreal-backend-1.0.87/setup.py` & `cdktf-surreal-backend-1.0.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-surreal-backend",
-    "version": "1.0.87",
+    "version": "1.0.9",
     "description": "A package that vends a construct to setup the surreal backend in CDKTF",
     "license": "Apache-2.0",
     "url": "https://github.com/awlsring/cdktf-surreal-backend.git",
     "long_description_content_type": "text/markdown",
     "author": "awlsring<mattcanemail@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,38 +22,37 @@
     },
     "packages": [
         "cdktf_surreal-backend",
         "cdktf_surreal-backend._jsii"
     ],
     "package_data": {
         "cdktf_surreal-backend._jsii": [
-            "cdktf-surreal-backend@1.0.87.jsii.tgz"
+            "cdktf-surreal-backend@1.0.9.jsii.tgz"
         ],
         "cdktf_surreal-backend": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "cdktf>=0.14.3, <0.15.0",
         "constructs>=10.1.52, <11.0.0",
-        "jsii>=1.80.0, <2.0.0",
+        "jsii>=1.74.0, <2.0.0",
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
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved"
     ],
     "scripts": []
 }
 """
```

### Comparing `cdktf-surreal-backend-1.0.87/src/cdktf_surreal-backend/__init__.py` & `cdktf-surreal-backend-1.0.9/src/cdktf_surreal-backend/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-surreal-backend-1.0.87/src/cdktf_surreal_backend.egg-info/PKG-INFO` & `cdktf-surreal-backend-1.0.9/src/cdktf_surreal_backend.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cdktf-surreal-backend
-Version: 1.0.87
+Version: 1.0.9
 Summary: A package that vends a construct to setup the surreal backend in CDKTF
 Home-page: https://github.com/awlsring/cdktf-surreal-backend.git
 Author: awlsring<mattcanemail@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/awlsring/cdktf-surreal-backend.git
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
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -55,7 +55,9 @@
 ### Construct Properties:
 
 * address: The address your backend sever is reachable at.
 * project: The project name to use for this stack.
 * stack: The stack name to use for this stack. stacks names must be unique across a project.
 * username: The username to use for authentication, configured in the server's config.yaml file
 * password: The password to use for authentication, configured in the server's config.yaml file
+
+
```

