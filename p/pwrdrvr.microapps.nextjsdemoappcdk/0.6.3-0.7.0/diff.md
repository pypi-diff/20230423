# Comparing `tmp/pwrdrvr.microapps.nextjsdemoappcdk-0.6.3.tar.gz` & `tmp/pwrdrvr.microapps.nextjsdemoappcdk-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/__w/microapps-app-nextjs-demo/microapps-app-nextjs-demo/packages/cdk-construct/dist/python/pwrdrvr.microapps.nextjsdemoappcdk-", last modified: Tue Feb 21 01:43:43 2023, max compression
+gzip compressed data, was "/__w/microapps-app-nextjs-demo/microapps-app-nextjs-demo/packages/cdk-construct/dist/python/pwrdrvr.microapps.nextjsdemoappcdk-", last modified: Sun Apr 23 13:50:33 2023, max compression
```

## Comparing `pwrdrvr.microapps.nextjsdemoappcdk-0.6.3.tar` & `pwrdrvr.microapps.nextjsdemoappcdk-0.7.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-02-21 01:43:43.000000 pwrdrvr.microapps.nextjsdemoappcdk-0.6.3/
--rw-r--r--   0 superchain  (1001) superchain  (1001)     1067 2023-02-21 01:43:36.000000 pwrdrvr.microapps.nextjsdemoappcdk-0.6.3/LICENSE
--rw-r--r--   0 superchain  (1001) superchain  (1001)       23 2023-02-21 01:43:36.000000 pwrdrvr.microapps.nextjsdemoappcdk-0.6.3/MANIFEST.in
--rw-r--r--   0 superchain  (1001) superchain  (1001)     1664 2023-02-21 01:43:43.000000 pwrdrvr.microapps.nextjsdemoappcdk-0.6.3/PKG-INFO
--rw-r--r--   0 superchain  (1001) superchain  (1001)      660 2023-02-21 01:43:36.000000 pwrdrvr.microapps.nextjsdemoappcdk-0.6.3/README.md
--rw-r--r--   0 superchain  (1001) superchain  (1001)      106 2023-02-21 01:43:36.000000 pwrdrvr.microapps.nextjsdemoappcdk-0.6.3/pyproject.toml
--rw-r--r--   0 superchain  (1001) superchain  (1001)       38 2023-02-21 01:43:43.000000 pwrdrvr.microapps.nextjsdemoappcdk-0.6.3/setup.cfg
--rw-r--r--   0 superchain  (1001) superchain  (1001)     1894 2023-02-21 01:43:36.000000 pwrdrvr.microapps.nextjsdemoappcdk-0.6.3/setup.py
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-02-21 01:43:43.000000 pwrdrvr.microapps.nextjsdemoappcdk-0.6.3/src/
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-02-21 01:43:43.000000 pwrdrvr.microapps.nextjsdemoappcdk-0.6.3/src/pwrdrvr/
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-02-21 01:43:43.000000 pwrdrvr.microapps.nextjsdemoappcdk-0.6.3/src/pwrdrvr/microapps/
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-02-21 01:43:43.000000 pwrdrvr.microapps.nextjsdemoappcdk-0.6.3/src/pwrdrvr/microapps/nextjsdemoappcdk/
--rw-r--r--   0 superchain  (1001) superchain  (1001)     6300 2023-02-21 01:43:36.000000 pwrdrvr.microapps.nextjsdemoappcdk-0.6.3/src/pwrdrvr/microapps/nextjsdemoappcdk/__init__.py
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-02-21 01:43:43.000000 pwrdrvr.microapps.nextjsdemoappcdk-0.6.3/src/pwrdrvr/microapps/nextjsdemoappcdk/_jsii/
--rw-r--r--   0 superchain  (1001) superchain  (1001)      413 2023-02-21 01:43:36.000000 pwrdrvr.microapps.nextjsdemoappcdk-0.6.3/src/pwrdrvr/microapps/nextjsdemoappcdk/_jsii/__init__.py
--rw-r--r--   0 superchain  (1001) superchain  (1001)  3008037 2023-02-21 01:43:36.000000 pwrdrvr.microapps.nextjsdemoappcdk-0.6.3/src/pwrdrvr/microapps/nextjsdemoappcdk/_jsii/microapps-app-nextjs-demo-cdk@0.6.3.jsii.tgz
--rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-02-21 01:43:36.000000 pwrdrvr.microapps.nextjsdemoappcdk-0.6.3/src/pwrdrvr/microapps/nextjsdemoappcdk/py.typed
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-02-21 01:43:43.000000 pwrdrvr.microapps.nextjsdemoappcdk-0.6.3/src/pwrdrvr.microapps.nextjsdemoappcdk.egg-info/
--rw-r--r--   0 superchain  (1001) superchain  (1001)     1664 2023-02-21 01:43:42.000000 pwrdrvr.microapps.nextjsdemoappcdk-0.6.3/src/pwrdrvr.microapps.nextjsdemoappcdk.egg-info/PKG-INFO
--rw-r--r--   0 superchain  (1001) superchain  (1001)      608 2023-02-21 01:43:42.000000 pwrdrvr.microapps.nextjsdemoappcdk-0.6.3/src/pwrdrvr.microapps.nextjsdemoappcdk.egg-info/SOURCES.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-02-21 01:43:42.000000 pwrdrvr.microapps.nextjsdemoappcdk-0.6.3/src/pwrdrvr.microapps.nextjsdemoappcdk.egg-info/dependency_links.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)       93 2023-02-21 01:43:42.000000 pwrdrvr.microapps.nextjsdemoappcdk-0.6.3/src/pwrdrvr.microapps.nextjsdemoappcdk.egg-info/requires.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)        8 2023-02-21 01:43:42.000000 pwrdrvr.microapps.nextjsdemoappcdk-0.6.3/src/pwrdrvr.microapps.nextjsdemoappcdk.egg-info/top_level.txt
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-04-23 13:50:33.000000 pwrdrvr.microapps.nextjsdemoappcdk-0.7.0/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     1067 2023-04-23 13:50:25.000000 pwrdrvr.microapps.nextjsdemoappcdk-0.7.0/LICENSE
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       23 2023-04-23 13:50:25.000000 pwrdrvr.microapps.nextjsdemoappcdk-0.7.0/MANIFEST.in
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     1664 2023-04-23 13:50:33.000000 pwrdrvr.microapps.nextjsdemoappcdk-0.7.0/PKG-INFO
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      660 2023-04-23 13:50:25.000000 pwrdrvr.microapps.nextjsdemoappcdk-0.7.0/README.md
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      106 2023-04-23 13:50:25.000000 pwrdrvr.microapps.nextjsdemoappcdk-0.7.0/pyproject.toml
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       38 2023-04-23 13:50:33.000000 pwrdrvr.microapps.nextjsdemoappcdk-0.7.0/setup.cfg
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     1894 2023-04-23 13:50:25.000000 pwrdrvr.microapps.nextjsdemoappcdk-0.7.0/setup.py
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-04-23 13:50:33.000000 pwrdrvr.microapps.nextjsdemoappcdk-0.7.0/src/
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-04-23 13:50:33.000000 pwrdrvr.microapps.nextjsdemoappcdk-0.7.0/src/pwrdrvr/
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-04-23 13:50:33.000000 pwrdrvr.microapps.nextjsdemoappcdk-0.7.0/src/pwrdrvr/microapps/
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-04-23 13:50:33.000000 pwrdrvr.microapps.nextjsdemoappcdk-0.7.0/src/pwrdrvr/microapps/nextjsdemoappcdk/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     6300 2023-04-23 13:50:25.000000 pwrdrvr.microapps.nextjsdemoappcdk-0.7.0/src/pwrdrvr/microapps/nextjsdemoappcdk/__init__.py
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-04-23 13:50:33.000000 pwrdrvr.microapps.nextjsdemoappcdk-0.7.0/src/pwrdrvr/microapps/nextjsdemoappcdk/_jsii/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      413 2023-04-23 13:50:25.000000 pwrdrvr.microapps.nextjsdemoappcdk-0.7.0/src/pwrdrvr/microapps/nextjsdemoappcdk/_jsii/__init__.py
+-rw-r--r--   0 superchain  (1001) superchain  (1001)  5644036 2023-04-23 13:50:25.000000 pwrdrvr.microapps.nextjsdemoappcdk-0.7.0/src/pwrdrvr/microapps/nextjsdemoappcdk/_jsii/microapps-app-nextjs-demo-cdk@0.7.0.jsii.tgz
+-rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-04-23 13:50:25.000000 pwrdrvr.microapps.nextjsdemoappcdk-0.7.0/src/pwrdrvr/microapps/nextjsdemoappcdk/py.typed
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-04-23 13:50:33.000000 pwrdrvr.microapps.nextjsdemoappcdk-0.7.0/src/pwrdrvr.microapps.nextjsdemoappcdk.egg-info/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     1664 2023-04-23 13:50:33.000000 pwrdrvr.microapps.nextjsdemoappcdk-0.7.0/src/pwrdrvr.microapps.nextjsdemoappcdk.egg-info/PKG-INFO
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      608 2023-04-23 13:50:33.000000 pwrdrvr.microapps.nextjsdemoappcdk-0.7.0/src/pwrdrvr.microapps.nextjsdemoappcdk.egg-info/SOURCES.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-04-23 13:50:33.000000 pwrdrvr.microapps.nextjsdemoappcdk-0.7.0/src/pwrdrvr.microapps.nextjsdemoappcdk.egg-info/dependency_links.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       93 2023-04-23 13:50:33.000000 pwrdrvr.microapps.nextjsdemoappcdk-0.7.0/src/pwrdrvr.microapps.nextjsdemoappcdk.egg-info/requires.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)        8 2023-04-23 13:50:33.000000 pwrdrvr.microapps.nextjsdemoappcdk-0.7.0/src/pwrdrvr.microapps.nextjsdemoappcdk.egg-info/top_level.txt
```

### Comparing `pwrdrvr.microapps.nextjsdemoappcdk-0.6.3/LICENSE` & `pwrdrvr.microapps.nextjsdemoappcdk-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pwrdrvr.microapps.nextjsdemoappcdk-0.6.3/PKG-INFO` & `pwrdrvr.microapps.nextjsdemoappcdk-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwrdrvr.microapps.nextjsdemoappcdk
-Version: 0.6.3
+Version: 0.7.0
 Summary: Release app for the MicroApps framework, by PwrDrvr LLC. Provides the ability to control which version of an app is launched.
 Home-page: https://github.com/pwrdrvr/microapps-app-nextjs-demo
 Author: PwrDrvr LLC
 License: MIT
 Project-URL: Source, https://github.com/pwrdrvr/microapps-app-nextjs-demo
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `pwrdrvr.microapps.nextjsdemoappcdk-0.6.3/README.md` & `pwrdrvr.microapps.nextjsdemoappcdk-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pwrdrvr.microapps.nextjsdemoappcdk-0.6.3/setup.py` & `pwrdrvr.microapps.nextjsdemoappcdk-0.7.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "pwrdrvr.microapps.nextjsdemoappcdk",
-    "version": "0.6.3",
+    "version": "0.7.0",
     "description": "Release app for the MicroApps framework, by PwrDrvr LLC. Provides the ability to control which version of an app is launched.",
     "license": "MIT",
     "url": "https://github.com/pwrdrvr/microapps-app-nextjs-demo",
     "long_description_content_type": "text/markdown",
     "author": "PwrDrvr LLC",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "pwrdrvr.microapps.nextjsdemoappcdk",
         "pwrdrvr.microapps.nextjsdemoappcdk._jsii"
     ],
     "package_data": {
         "pwrdrvr.microapps.nextjsdemoappcdk._jsii": [
-            "microapps-app-nextjs-demo-cdk@0.6.3.jsii.tgz"
+            "microapps-app-nextjs-demo-cdk@0.7.0.jsii.tgz"
         ],
         "pwrdrvr.microapps.nextjsdemoappcdk": [
             "py.typed"
         ]
     },
     "python_requires": ">=3.6",
     "install_requires": [
```

### Comparing `pwrdrvr.microapps.nextjsdemoappcdk-0.6.3/src/pwrdrvr/microapps/nextjsdemoappcdk/__init__.py` & `pwrdrvr.microapps.nextjsdemoappcdk-0.7.0/src/pwrdrvr/microapps/nextjsdemoappcdk/__init__.py`

 * *Files identical despite different names*

### Comparing `pwrdrvr.microapps.nextjsdemoappcdk-0.6.3/src/pwrdrvr.microapps.nextjsdemoappcdk.egg-info/PKG-INFO` & `pwrdrvr.microapps.nextjsdemoappcdk-0.7.0/src/pwrdrvr.microapps.nextjsdemoappcdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwrdrvr.microapps.nextjsdemoappcdk
-Version: 0.6.3
+Version: 0.7.0
 Summary: Release app for the MicroApps framework, by PwrDrvr LLC. Provides the ability to control which version of an app is launched.
 Home-page: https://github.com/pwrdrvr/microapps-app-nextjs-demo
 Author: PwrDrvr LLC
 License: MIT
 Project-URL: Source, https://github.com/pwrdrvr/microapps-app-nextjs-demo
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `pwrdrvr.microapps.nextjsdemoappcdk-0.6.3/src/pwrdrvr.microapps.nextjsdemoappcdk.egg-info/SOURCES.txt` & `pwrdrvr.microapps.nextjsdemoappcdk-0.7.0/src/pwrdrvr.microapps.nextjsdemoappcdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/pwrdrvr.microapps.nextjsdemoappcdk.egg-info/SOURCES.txt
 src/pwrdrvr.microapps.nextjsdemoappcdk.egg-info/dependency_links.txt
 src/pwrdrvr.microapps.nextjsdemoappcdk.egg-info/requires.txt
 src/pwrdrvr.microapps.nextjsdemoappcdk.egg-info/top_level.txt
 src/pwrdrvr/microapps/nextjsdemoappcdk/__init__.py
 src/pwrdrvr/microapps/nextjsdemoappcdk/py.typed
 src/pwrdrvr/microapps/nextjsdemoappcdk/_jsii/__init__.py
-src/pwrdrvr/microapps/nextjsdemoappcdk/_jsii/microapps-app-nextjs-demo-cdk@0.6.3.jsii.tgz
+src/pwrdrvr/microapps/nextjsdemoappcdk/_jsii/microapps-app-nextjs-demo-cdk@0.7.0.jsii.tgz
```

