# Comparing `tmp/dknovautils-0.0.30.tar.gz` & `tmp/dknovautils-0.0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dknovautils-0.0.30.tar", last modified: Fri Apr 21 16:13:34 2023, max compression
+gzip compressed data, was "dist/dknovautils-0.0.31.tar", last modified: Sun Apr 23 05:56:10 2023, max compression
```

## Comparing `dknovautils-0.0.30.tar` & `dknovautils-0.0.31.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-04-21 16:13:34.000000 dknovautils-0.0.30/
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-04-21 16:13:34.000000 dknovautils-0.0.30/dknovautils/
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1852 2023-04-21 05:31:21.000000 dknovautils-0.0.30/dknovautils/commons.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     4119 2023-04-21 16:13:33.000000 dknovautils-0.0.30/dknovautils/dkat.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1510 2023-04-13 12:40:40.000000 dknovautils-0.0.30/dknovautils/dkfiles.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1117 2023-04-21 16:13:22.000000 dknovautils-0.0.30/dknovautils/dkipy.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      711 2023-04-21 16:13:33.000000 dknovautils-0.0.30/dknovautils/dk_imports.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      490 2023-04-13 12:40:48.000000 dknovautils-0.0.30/dknovautils/example.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      140 2023-04-13 15:12:06.000000 dknovautils-0.0.30/dknovautils/myadd.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      160 2023-04-13 15:11:54.000000 dknovautils-0.0.30/dknovautils/mysubtract.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      307 2023-04-21 15:52:41.000000 dknovautils-0.0.30/dknovautils/__init__.py
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-04-21 16:13:34.000000 dknovautils-0.0.30/dknovautils.egg-info/
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)        1 2023-04-21 16:13:34.000000 dknovautils-0.0.30/dknovautils.egg-info/dependency_links.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      881 2023-04-21 16:13:34.000000 dknovautils-0.0.30/dknovautils.egg-info/PKG-INFO
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)        6 2023-04-21 16:13:34.000000 dknovautils-0.0.30/dknovautils.egg-info/requires.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      407 2023-04-21 16:13:34.000000 dknovautils-0.0.30/dknovautils.egg-info/SOURCES.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)       12 2023-04-21 16:13:34.000000 dknovautils-0.0.30/dknovautils.egg-info/top_level.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      105 2023-03-09 04:32:08.000000 dknovautils-0.0.30/LICENSE
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      881 2023-04-21 16:13:34.000000 dknovautils-0.0.30/PKG-INFO
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      472 2023-03-09 06:46:27.000000 dknovautils-0.0.30/README.md
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)       38 2023-04-21 16:13:34.000000 dknovautils-0.0.30/setup.cfg
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1140 2023-04-21 16:13:33.000000 dknovautils-0.0.30/setup.py
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-04-23 05:56:10.000000 dknovautils-0.0.31/
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-04-23 05:56:10.000000 dknovautils-0.0.31/dknovautils/
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1881 2023-04-22 16:09:58.000000 dknovautils-0.0.31/dknovautils/commons.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     5432 2023-04-23 05:56:06.000000 dknovautils-0.0.31/dknovautils/dkat.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1510 2023-04-13 12:40:40.000000 dknovautils-0.0.31/dknovautils/dkfiles.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1149 2023-04-22 02:58:52.000000 dknovautils-0.0.31/dknovautils/dkipy.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      711 2023-04-23 05:56:06.000000 dknovautils-0.0.31/dknovautils/dk_imports.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      490 2023-04-13 12:40:48.000000 dknovautils-0.0.31/dknovautils/example.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      140 2023-04-13 15:12:06.000000 dknovautils-0.0.31/dknovautils/myadd.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      160 2023-04-13 15:11:54.000000 dknovautils-0.0.31/dknovautils/mysubtract.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      307 2023-04-21 15:52:41.000000 dknovautils-0.0.31/dknovautils/__init__.py
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-04-23 05:56:10.000000 dknovautils-0.0.31/dknovautils.egg-info/
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)        1 2023-04-23 05:56:09.000000 dknovautils-0.0.31/dknovautils.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      881 2023-04-23 05:56:09.000000 dknovautils-0.0.31/dknovautils.egg-info/PKG-INFO
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)        6 2023-04-23 05:56:09.000000 dknovautils-0.0.31/dknovautils.egg-info/requires.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      407 2023-04-23 05:56:09.000000 dknovautils-0.0.31/dknovautils.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)       12 2023-04-23 05:56:09.000000 dknovautils-0.0.31/dknovautils.egg-info/top_level.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      105 2023-03-09 04:32:08.000000 dknovautils-0.0.31/LICENSE
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      881 2023-04-23 05:56:10.000000 dknovautils-0.0.31/PKG-INFO
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      472 2023-03-09 06:46:27.000000 dknovautils-0.0.31/README.md
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)       38 2023-04-23 05:56:10.000000 dknovautils-0.0.31/setup.cfg
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1140 2023-04-23 05:56:06.000000 dknovautils-0.0.31/setup.py
```

### Comparing `dknovautils-0.0.30/dknovautils/commons.py` & `dknovautils-0.0.31/dknovautils/commons.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 
 from dknovautils.dkat import *
 
 from dknovautils.dkipy import *
 
 
-
 def write_async():
     pass
 
 
 def dtprint(s: str):
     print(s)
 
@@ -47,20 +46,22 @@
         AT._innerLoggerFun_(obj, level)
         return
     else:
         pass
 
     now = datetime.now()
     # dts = now.strftime("%d/%m/%Y %H:%M:%S")
-    otstr = now.isoformat()[:(10 + 1 + 8)]
+    otstr = now.isoformat()[:(10 + 1 + 8+4)]
+
+    if False:
 
-    otstr2 = datetime.fromtimestamp(time.time()).strftime(
-        "%Y-%m-%dT%H:%M:%S.%f")[0:23]
+        otstr2 = datetime.fromtimestamp(time.time()).strftime(
+            "%Y-%m-%dT%H:%M:%S.%f")[0:23]
 
-    msg = f'[{otstr}]{obj}'
+        msg = f'[{otstr}]{obj}'
 
     print(f"[{otstr}][{level.name.lower()}]{obj}")
 
 # _myCntInfos = {}
 
 
 '''
```

### Comparing `dknovautils-0.0.30/dknovautils/dkfiles.py` & `dknovautils-0.0.31/dknovautils/dkfiles.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.0.30/dknovautils/dkipy.py` & `dknovautils-0.0.31/dknovautils/dkipy.py`

 * *Files 22% similar despite different names*

```diff
@@ -29,18 +29,18 @@
         if logcmd:
             commons.iprint_info(f'begin run cmd: {cmd}')
 
         r = get_ipython().getoutput(cmd)
         return r
 
 
-def dk_mfc(cmd): DkIpyUtils.mfc(cmd)
+def dk_mfc(cmd, logcmd): DkIpyUtils.mfc(cmd, logcmd)
 
 
-def dk_mfr(cmd): return DkIpyUtils.mfr(cmd)
+def dk_mfr(cmd, logcmd): return DkIpyUtils.mfr(cmd, logcmd)
 
 
 '''
 
 !{cmd}
 
 r=get_ipython().getoutput('{cmd}')
```

### Comparing `dknovautils-0.0.30/dknovautils/dk_imports.py` & `dknovautils-0.0.31/dknovautils/dk_imports.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.0.30/dknovautils.egg-info/PKG-INFO` & `dknovautils-0.0.31/dknovautils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dknovautils
-Version: 0.0.30
+Version: 0.0.31
 Summary: This is the tools for dknova.
 Home-page: http://example.com
 Author: dknova
 Author-email: dknova@example.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dknovautils-0.0.30/PKG-INFO` & `dknovautils-0.0.31/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dknovautils
-Version: 0.0.30
+Version: 0.0.31
 Summary: This is the tools for dknova.
 Home-page: http://example.com
 Author: dknova
 Author-email: dknova@example.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dknovautils-0.0.30/setup.py` & `dknovautils-0.0.31/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import re
 import setuptools
 
 from distutils.core import setup
 from setuptools import find_packages
 
-DkAppVer = '0.0.30'
+DkAppVer = '0.0.31'
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="dknovautils",
     version=DkAppVer,
```

