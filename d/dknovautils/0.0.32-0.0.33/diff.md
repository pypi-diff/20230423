# Comparing `tmp/dknovautils-0.0.32.tar.gz` & `tmp/dknovautils-0.0.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dknovautils-0.0.32.tar", last modified: Sun Apr 23 08:36:11 2023, max compression
+gzip compressed data, was "dist/dknovautils-0.0.33.tar", last modified: Sun Apr 23 14:12:42 2023, max compression
```

## Comparing `dknovautils-0.0.32.tar` & `dknovautils-0.0.33.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-04-23 08:36:11.000000 dknovautils-0.0.32/
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-04-23 08:36:11.000000 dknovautils-0.0.32/dknovautils/
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1881 2023-04-22 16:09:58.000000 dknovautils-0.0.32/dknovautils/commons.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     5428 2023-04-23 08:36:10.000000 dknovautils-0.0.32/dknovautils/dkat.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1510 2023-04-13 12:40:40.000000 dknovautils-0.0.32/dknovautils/dkfiles.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1149 2023-04-22 02:58:52.000000 dknovautils-0.0.32/dknovautils/dkipy.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      711 2023-04-23 08:36:10.000000 dknovautils-0.0.32/dknovautils/dk_imports.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      490 2023-04-13 12:40:48.000000 dknovautils-0.0.32/dknovautils/example.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      140 2023-04-13 15:12:06.000000 dknovautils-0.0.32/dknovautils/myadd.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      160 2023-04-13 15:11:54.000000 dknovautils-0.0.32/dknovautils/mysubtract.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      307 2023-04-21 15:52:41.000000 dknovautils-0.0.32/dknovautils/__init__.py
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-04-23 08:36:11.000000 dknovautils-0.0.32/dknovautils.egg-info/
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)        1 2023-04-23 08:36:10.000000 dknovautils-0.0.32/dknovautils.egg-info/dependency_links.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      881 2023-04-23 08:36:10.000000 dknovautils-0.0.32/dknovautils.egg-info/PKG-INFO
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)        6 2023-04-23 08:36:10.000000 dknovautils-0.0.32/dknovautils.egg-info/requires.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      407 2023-04-23 08:36:10.000000 dknovautils-0.0.32/dknovautils.egg-info/SOURCES.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)       12 2023-04-23 08:36:10.000000 dknovautils-0.0.32/dknovautils.egg-info/top_level.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      105 2023-03-09 04:32:08.000000 dknovautils-0.0.32/LICENSE
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      881 2023-04-23 08:36:11.000000 dknovautils-0.0.32/PKG-INFO
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      472 2023-03-09 06:46:27.000000 dknovautils-0.0.32/README.md
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)       38 2023-04-23 08:36:11.000000 dknovautils-0.0.32/setup.cfg
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1140 2023-04-23 08:36:10.000000 dknovautils-0.0.32/setup.py
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-04-23 14:12:42.000000 dknovautils-0.0.33/
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-04-23 14:12:42.000000 dknovautils-0.0.33/dknovautils/
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1881 2023-04-22 16:09:58.000000 dknovautils-0.0.33/dknovautils/commons.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     5513 2023-04-23 14:12:41.000000 dknovautils-0.0.33/dknovautils/dkat.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1510 2023-04-13 12:40:40.000000 dknovautils-0.0.33/dknovautils/dkfiles.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1149 2023-04-22 02:58:52.000000 dknovautils-0.0.33/dknovautils/dkipy.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      711 2023-04-23 14:12:41.000000 dknovautils-0.0.33/dknovautils/dk_imports.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      490 2023-04-13 12:40:48.000000 dknovautils-0.0.33/dknovautils/example.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      140 2023-04-13 15:12:06.000000 dknovautils-0.0.33/dknovautils/myadd.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      160 2023-04-13 15:11:54.000000 dknovautils-0.0.33/dknovautils/mysubtract.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      307 2023-04-21 15:52:41.000000 dknovautils-0.0.33/dknovautils/__init__.py
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-04-23 14:12:42.000000 dknovautils-0.0.33/dknovautils.egg-info/
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)        1 2023-04-23 14:12:42.000000 dknovautils-0.0.33/dknovautils.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      881 2023-04-23 14:12:42.000000 dknovautils-0.0.33/dknovautils.egg-info/PKG-INFO
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)        6 2023-04-23 14:12:42.000000 dknovautils-0.0.33/dknovautils.egg-info/requires.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      407 2023-04-23 14:12:42.000000 dknovautils-0.0.33/dknovautils.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)       12 2023-04-23 14:12:42.000000 dknovautils-0.0.33/dknovautils.egg-info/top_level.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      105 2023-03-09 04:32:08.000000 dknovautils-0.0.33/LICENSE
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      881 2023-04-23 14:12:42.000000 dknovautils-0.0.33/PKG-INFO
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      472 2023-03-09 06:46:27.000000 dknovautils-0.0.33/README.md
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)       38 2023-04-23 14:12:42.000000 dknovautils-0.0.33/setup.cfg
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1140 2023-04-23 14:12:41.000000 dknovautils-0.0.33/setup.py
```

### Comparing `dknovautils-0.0.32/dknovautils/commons.py` & `dknovautils-0.0.33/dknovautils/commons.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.0.32/dknovautils/dkat.py` & `dknovautils-0.0.33/dknovautils/dkat.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 import dknovautils
 from dknovautils.commons import *
 
 import beepy
 
 
-DkAppVer = '0.0.32'
+DkAppVer = '0.0.33'
 _unknown_err = '_unknown_err4035'
 
 
 class AT(object):
 
     _innerLoggerFun_ = None
 
@@ -28,21 +28,21 @@
                 # 也用debug级别。只是在prod模式下可以关闭。
                 logger.debug(obj)
             elif llevel == LLevel.Debug:
                 logger.debug(obj)
             elif llevel == LLevel.Info:
                 logger.info(obj)
             elif llevel == LLevel.Warn:
+                logger.warning(obj)
                 if beepWarn:
                     AT.beep_error_buffered()
-                logger.warning(obj)
             elif llevel == LLevel.Error:
+                logger.error(obj)
                 if beepError:
                     AT.beep_error_buffered()
-                logger.error(obj)
             else:
                 assert False, f"bad {llevel}"
 
             pass
 
         if initInnerLoggerFun:
             AT._innerLoggerFun_ = mloggerFun
@@ -169,14 +169,16 @@
             return
 
         AT._AstErrorCnt_ += 1
         msg = _unknown_err if s is None else s
 
         dknovautils.commons.iprint_error(msg)
 
+        raise DkAstException(msg)
+
         # assert b,
         pass
 
     @staticmethod
     def mychdir(s):
         assert isinstance(s, str) and len(s) > 0
         iprint_debug(f'chdir: {s}')
@@ -198,14 +200,18 @@
     @staticmethod
     def unimplemented(s: str = None):
         AT.assert_(False, s if s is not None else 'err4823 unimplemented 未实现的功能')
 
     VERSION = DkAppVer
 
 
+class DkAstException(Exception):
+    pass
+
+
 '''
 
 LOG_FORMAT = "%(asctime)s - %(levelname)s - %(message)s"
 DATE_FORMAT = "%m/%d/%Y %H:%M:%S %p"
 
 logging.basicConfig(filename='/mnt/d/tmp/demo0726.log', level=logging.DEBUG, format=LOG_FORMAT, datefmt=DATE_FORMAT)
```

### Comparing `dknovautils-0.0.32/dknovautils/dkfiles.py` & `dknovautils-0.0.33/dknovautils/dkfiles.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.0.32/dknovautils/dkipy.py` & `dknovautils-0.0.33/dknovautils/dkipy.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.0.32/dknovautils/dk_imports.py` & `dknovautils-0.0.33/dknovautils/dk_imports.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.0.32/dknovautils.egg-info/PKG-INFO` & `dknovautils-0.0.33/dknovautils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dknovautils
-Version: 0.0.32
+Version: 0.0.33
 Summary: This is the tools for dknova.
 Home-page: http://example.com
 Author: dknova
 Author-email: dknova@example.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dknovautils-0.0.32/PKG-INFO` & `dknovautils-0.0.33/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dknovautils
-Version: 0.0.32
+Version: 0.0.33
 Summary: This is the tools for dknova.
 Home-page: http://example.com
 Author: dknova
 Author-email: dknova@example.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dknovautils-0.0.32/setup.py` & `dknovautils-0.0.33/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import re
 import setuptools
 
 from distutils.core import setup
 from setuptools import find_packages
 
-DkAppVer = '0.0.32'
+DkAppVer = '0.0.33'
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="dknovautils",
     version=DkAppVer,
```

