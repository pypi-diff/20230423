# Comparing `tmp/dknovautils-0.0.31.tar.gz` & `tmp/dknovautils-0.0.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dknovautils-0.0.31.tar", last modified: Sun Apr 23 05:56:10 2023, max compression
+gzip compressed data, was "dist/dknovautils-0.0.32.tar", last modified: Sun Apr 23 08:36:11 2023, max compression
```

## Comparing `dknovautils-0.0.31.tar` & `dknovautils-0.0.32.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-04-23 05:56:10.000000 dknovautils-0.0.31/
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-04-23 05:56:10.000000 dknovautils-0.0.31/dknovautils/
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1881 2023-04-22 16:09:58.000000 dknovautils-0.0.31/dknovautils/commons.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     5432 2023-04-23 05:56:06.000000 dknovautils-0.0.31/dknovautils/dkat.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1510 2023-04-13 12:40:40.000000 dknovautils-0.0.31/dknovautils/dkfiles.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1149 2023-04-22 02:58:52.000000 dknovautils-0.0.31/dknovautils/dkipy.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      711 2023-04-23 05:56:06.000000 dknovautils-0.0.31/dknovautils/dk_imports.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      490 2023-04-13 12:40:48.000000 dknovautils-0.0.31/dknovautils/example.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      140 2023-04-13 15:12:06.000000 dknovautils-0.0.31/dknovautils/myadd.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      160 2023-04-13 15:11:54.000000 dknovautils-0.0.31/dknovautils/mysubtract.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      307 2023-04-21 15:52:41.000000 dknovautils-0.0.31/dknovautils/__init__.py
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-04-23 05:56:10.000000 dknovautils-0.0.31/dknovautils.egg-info/
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)        1 2023-04-23 05:56:09.000000 dknovautils-0.0.31/dknovautils.egg-info/dependency_links.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      881 2023-04-23 05:56:09.000000 dknovautils-0.0.31/dknovautils.egg-info/PKG-INFO
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)        6 2023-04-23 05:56:09.000000 dknovautils-0.0.31/dknovautils.egg-info/requires.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      407 2023-04-23 05:56:09.000000 dknovautils-0.0.31/dknovautils.egg-info/SOURCES.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)       12 2023-04-23 05:56:09.000000 dknovautils-0.0.31/dknovautils.egg-info/top_level.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      105 2023-03-09 04:32:08.000000 dknovautils-0.0.31/LICENSE
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      881 2023-04-23 05:56:10.000000 dknovautils-0.0.31/PKG-INFO
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      472 2023-03-09 06:46:27.000000 dknovautils-0.0.31/README.md
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)       38 2023-04-23 05:56:10.000000 dknovautils-0.0.31/setup.cfg
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1140 2023-04-23 05:56:06.000000 dknovautils-0.0.31/setup.py
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-04-23 08:36:11.000000 dknovautils-0.0.32/
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-04-23 08:36:11.000000 dknovautils-0.0.32/dknovautils/
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1881 2023-04-22 16:09:58.000000 dknovautils-0.0.32/dknovautils/commons.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     5428 2023-04-23 08:36:10.000000 dknovautils-0.0.32/dknovautils/dkat.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1510 2023-04-13 12:40:40.000000 dknovautils-0.0.32/dknovautils/dkfiles.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1149 2023-04-22 02:58:52.000000 dknovautils-0.0.32/dknovautils/dkipy.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      711 2023-04-23 08:36:10.000000 dknovautils-0.0.32/dknovautils/dk_imports.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      490 2023-04-13 12:40:48.000000 dknovautils-0.0.32/dknovautils/example.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      140 2023-04-13 15:12:06.000000 dknovautils-0.0.32/dknovautils/myadd.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      160 2023-04-13 15:11:54.000000 dknovautils-0.0.32/dknovautils/mysubtract.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      307 2023-04-21 15:52:41.000000 dknovautils-0.0.32/dknovautils/__init__.py
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-04-23 08:36:11.000000 dknovautils-0.0.32/dknovautils.egg-info/
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)        1 2023-04-23 08:36:10.000000 dknovautils-0.0.32/dknovautils.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      881 2023-04-23 08:36:10.000000 dknovautils-0.0.32/dknovautils.egg-info/PKG-INFO
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)        6 2023-04-23 08:36:10.000000 dknovautils-0.0.32/dknovautils.egg-info/requires.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      407 2023-04-23 08:36:10.000000 dknovautils-0.0.32/dknovautils.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)       12 2023-04-23 08:36:10.000000 dknovautils-0.0.32/dknovautils.egg-info/top_level.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      105 2023-03-09 04:32:08.000000 dknovautils-0.0.32/LICENSE
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      881 2023-04-23 08:36:11.000000 dknovautils-0.0.32/PKG-INFO
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      472 2023-03-09 06:46:27.000000 dknovautils-0.0.32/README.md
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)       38 2023-04-23 08:36:11.000000 dknovautils-0.0.32/setup.cfg
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1140 2023-04-23 08:36:10.000000 dknovautils-0.0.32/setup.py
```

### Comparing `dknovautils-0.0.31/dknovautils/commons.py` & `dknovautils-0.0.32/dknovautils/commons.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.0.31/dknovautils/dkat.py` & `dknovautils-0.0.32/dknovautils/dkat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 import dknovautils
 from dknovautils.commons import *
 
 import beepy
 
 
-DkAppVer = '0.0.31'
+DkAppVer = '0.0.32'
 _unknown_err = '_unknown_err4035'
 
 
 class AT(object):
 
     _innerLoggerFun_ = None
 
@@ -161,15 +161,15 @@
 
     @staticmethod
     def assert_(b: bool, s: str = None):
         # 改成完善的形式
 
         assert isinstance(b, bool)
 
-        if not b:
+        if b:
             return
 
         AT._AstErrorCnt_ += 1
         msg = _unknown_err if s is None else s
 
         dknovautils.commons.iprint_error(msg)
```

### Comparing `dknovautils-0.0.31/dknovautils/dkfiles.py` & `dknovautils-0.0.32/dknovautils/dkfiles.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.0.31/dknovautils/dkipy.py` & `dknovautils-0.0.32/dknovautils/dkipy.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.0.31/dknovautils/dk_imports.py` & `dknovautils-0.0.32/dknovautils/dk_imports.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.0.31/dknovautils.egg-info/PKG-INFO` & `dknovautils-0.0.32/dknovautils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dknovautils
-Version: 0.0.31
+Version: 0.0.32
 Summary: This is the tools for dknova.
 Home-page: http://example.com
 Author: dknova
 Author-email: dknova@example.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dknovautils-0.0.31/PKG-INFO` & `dknovautils-0.0.32/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dknovautils
-Version: 0.0.31
+Version: 0.0.32
 Summary: This is the tools for dknova.
 Home-page: http://example.com
 Author: dknova
 Author-email: dknova@example.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dknovautils-0.0.31/setup.py` & `dknovautils-0.0.32/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import re
 import setuptools
 
 from distutils.core import setup
 from setuptools import find_packages
 
-DkAppVer = '0.0.31'
+DkAppVer = '0.0.32'
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="dknovautils",
     version=DkAppVer,
```

