# Comparing `tmp/ox_script-0.3.2.tar.gz` & `tmp/ox_script-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ox_script-0.3.2.tar", last modified: Sat Apr 22 20:00:01 2023, max compression
+gzip compressed data, was "dist/ox_script-0.3.3.tar", last modified: Sat Apr 22 22:36:33 2023, max compression
```

## Comparing `ox_script-0.3.2.tar` & `ox_script-0.3.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jarvislu   (501) staff       (20)        0 2023-04-22 20:00:01.000000 ox_script-0.3.2/
--rw-r--r--   0 jarvislu   (501) staff       (20)      743 2023-04-22 20:00:01.000000 ox_script-0.3.2/PKG-INFO
--rw-r--r--   0 jarvislu   (501) staff       (20)       13 2023-04-22 17:32:02.000000 ox_script-0.3.2/MANIFEST.in
-drwxr-xr-x   0 jarvislu   (501) staff       (20)        0 2023-04-22 20:00:01.000000 ox_script-0.3.2/ox_script/
--rw-------   0 jarvislu   (501) staff       (20)    12092 2023-04-22 19:58:19.000000 ox_script-0.3.2/ox_script/general_purpose_apis.py
--rw-r--r--   0 jarvislu   (501) staff       (20)       72 2023-04-22 19:58:19.000000 ox_script-0.3.2/ox_script/__init__.py
--rw-------   0 jarvislu   (501) staff       (20)    25033 2023-04-22 19:58:19.000000 ox_script-0.3.2/ox_script/printer_specific_apis.py
-drwxr-xr-x   0 jarvislu   (501) staff       (20)        0 2023-04-22 20:00:01.000000 ox_script-0.3.2/ox_script.egg-info/
--rw-r--r--   0 jarvislu   (501) staff       (20)      743 2023-04-22 20:00:01.000000 ox_script-0.3.2/ox_script.egg-info/PKG-INFO
--rw-r--r--   0 jarvislu   (501) staff       (20)      275 2023-04-22 20:00:01.000000 ox_script-0.3.2/ox_script.egg-info/SOURCES.txt
--rw-r--r--   0 jarvislu   (501) staff       (20)       16 2023-04-22 20:00:01.000000 ox_script-0.3.2/ox_script.egg-info/requires.txt
--rw-r--r--   0 jarvislu   (501) staff       (20)       10 2023-04-22 20:00:01.000000 ox_script-0.3.2/ox_script.egg-info/top_level.txt
--rw-r--r--   0 jarvislu   (501) staff       (20)        1 2023-04-22 20:00:01.000000 ox_script-0.3.2/ox_script.egg-info/dependency_links.txt
--rw-r--r--   0 jarvislu   (501) staff       (20)      875 2023-04-22 19:58:29.000000 ox_script-0.3.2/setup.py
--rw-r--r--   0 jarvislu   (501) staff       (20)       38 2023-04-22 20:00:01.000000 ox_script-0.3.2/setup.cfg
+drwxr-xr-x   0 jarvislu   (501) staff       (20)        0 2023-04-22 22:36:33.000000 ox_script-0.3.3/
+-rw-r--r--   0 jarvislu   (501) staff       (20)      743 2023-04-22 22:36:33.000000 ox_script-0.3.3/PKG-INFO
+-rw-r--r--   0 jarvislu   (501) staff       (20)       13 2023-04-22 17:32:02.000000 ox_script-0.3.3/MANIFEST.in
+drwxr-xr-x   0 jarvislu   (501) staff       (20)        0 2023-04-22 22:36:33.000000 ox_script-0.3.3/ox_script/
+-rw-------   0 jarvislu   (501) staff       (20)    12092 2023-04-22 19:58:19.000000 ox_script-0.3.3/ox_script/general_purpose_apis.py
+-rw-r--r--   0 jarvislu   (501) staff       (20)       72 2023-04-22 19:58:19.000000 ox_script-0.3.3/ox_script/__init__.py
+-rw-------   0 jarvislu   (501) staff       (20)    25033 2023-04-22 19:58:19.000000 ox_script-0.3.3/ox_script/printer_specific_apis.py
+drwxr-xr-x   0 jarvislu   (501) staff       (20)        0 2023-04-22 22:36:33.000000 ox_script-0.3.3/ox_script.egg-info/
+-rw-r--r--   0 jarvislu   (501) staff       (20)      743 2023-04-22 22:36:33.000000 ox_script-0.3.3/ox_script.egg-info/PKG-INFO
+-rw-r--r--   0 jarvislu   (501) staff       (20)      275 2023-04-22 22:36:33.000000 ox_script-0.3.3/ox_script.egg-info/SOURCES.txt
+-rw-r--r--   0 jarvislu   (501) staff       (20)       16 2023-04-22 22:36:33.000000 ox_script-0.3.3/ox_script.egg-info/requires.txt
+-rw-r--r--   0 jarvislu   (501) staff       (20)       10 2023-04-22 22:36:33.000000 ox_script-0.3.3/ox_script.egg-info/top_level.txt
+-rw-r--r--   0 jarvislu   (501) staff       (20)        1 2023-04-22 22:36:33.000000 ox_script-0.3.3/ox_script.egg-info/dependency_links.txt
+-rw-r--r--   0 jarvislu   (501) staff       (20)      875 2023-04-22 22:35:25.000000 ox_script-0.3.3/setup.py
+-rw-r--r--   0 jarvislu   (501) staff       (20)       38 2023-04-22 22:36:33.000000 ox_script-0.3.3/setup.cfg
```

### Comparing `ox_script-0.3.2/PKG-INFO` & `ox_script-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: ox_script
-Version: 0.3.2
+Version: 0.3.3
 Summary: The pskfunc.py file details offically supported APIs. The printer have a version of pskfunc.py on the printer with all functions fully implemented.
 Most printer specific functions are left blank intentionally as they are meant to be executed on the printer and will throw an error if called on your devices. This file is provided more so for the beneift of keeping your IDE of choice happy while programming, providing extensive comments on the different functions and allowing for easy install through pip. 
 Home-page: https://github.com/POSTEK-OX-Script
 Author: Postek Electronics Co., Ltd.
 Author-email: support@postek.com.cn
 License: MIT
 Description: UNKNOWN
```

### Comparing `ox_script-0.3.2/ox_script/general_purpose_apis.py` & `ox_script-0.3.3/ox_script/general_purpose_apis.py`

 * *Files identical despite different names*

### Comparing `ox_script-0.3.2/ox_script/printer_specific_apis.py` & `ox_script-0.3.3/ox_script/printer_specific_apis.py`

 * *Files identical despite different names*

### Comparing `ox_script-0.3.2/ox_script.egg-info/PKG-INFO` & `ox_script-0.3.3/ox_script.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: ox-script
-Version: 0.3.2
+Version: 0.3.3
 Summary: The pskfunc.py file details offically supported APIs. The printer have a version of pskfunc.py on the printer with all functions fully implemented.
 Most printer specific functions are left blank intentionally as they are meant to be executed on the printer and will throw an error if called on your devices. This file is provided more so for the beneift of keeping your IDE of choice happy while programming, providing extensive comments on the different functions and allowing for easy install through pip. 
 Home-page: https://github.com/POSTEK-OX-Script
 Author: Postek Electronics Co., Ltd.
 Author-email: support@postek.com.cn
 License: MIT
 Description: UNKNOWN
```

### Comparing `ox_script-0.3.2/setup.py` & `ox_script-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ox_script',
-    version='0.3.2',
+    version='0.3.3',
     author='Postek Electronics Co., Ltd.',
     author_email='support@postek.com.cn',
     packages=find_packages(),
     license="MIT",
     description="The pskfunc.py file details offically supported APIs. The printer have a version of pskfunc.py on the printer with all functions fully implemented.\nMost printer specific functions are left blank intentionally as they are meant to be executed on the printer and will throw an error if called on your devices. This file is provided more so for the beneift of keeping your IDE of choice happy while programming, providing extensive comments on the different functions and allowing for easy install through pip. ",
     url="https://github.com/POSTEK-OX-Script",
     install_requires=[
```

