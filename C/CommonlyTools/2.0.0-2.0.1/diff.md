# Comparing `tmp/CommonlyTools-2.0.0.tar.gz` & `tmp/CommonlyTools-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CommonlyTools-2.0.0.tar", last modified: Sun Apr 23 06:41:52 2023, max compression
+gzip compressed data, was "CommonlyTools-2.0.1.tar", last modified: Sun Apr 23 14:25:28 2023, max compression
```

## Comparing `CommonlyTools-2.0.0.tar` & `CommonlyTools-2.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-23 06:41:52.390236 CommonlyTools-2.0.0/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-23 06:41:52.390236 CommonlyTools-2.0.0/CommonlyTools.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1650 2023-04-23 06:41:52.000000 CommonlyTools-2.0.0/CommonlyTools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      278 2023-04-23 06:41:52.000000 CommonlyTools-2.0.0/CommonlyTools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-23 06:41:52.000000 CommonlyTools-2.0.0/CommonlyTools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       18 2023-04-23 06:41:52.000000 CommonlyTools-2.0.0/CommonlyTools.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       14 2023-04-23 06:41:52.000000 CommonlyTools-2.0.0/CommonlyTools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     1062 2023-04-23 04:55:31.000000 CommonlyTools-2.0.0/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     1650 2023-04-23 06:41:52.390236 CommonlyTools-2.0.0/PKG-INFO
--rw-------   0 runner    (1000) runner    (1000)      910 2023-04-23 06:38:57.000000 CommonlyTools-2.0.0/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-23 06:41:52.390236 CommonlyTools-2.0.0/commonlytools/
--rw-------   0 runner    (1000) runner    (1000)       24 2023-04-23 04:55:26.000000 CommonlyTools-2.0.0/commonlytools/__init__.py
--rw-------   0 runner    (1000) runner    (1000)     2313 2023-04-23 04:55:26.000000 CommonlyTools-2.0.0/commonlytools/discohook.py
--rw-r--r--   0 runner    (1000) runner    (1000)      312 2023-04-23 02:53:39.000000 CommonlyTools-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-04-23 06:41:52.394236 CommonlyTools-2.0.0/setup.cfg
--rw-------   0 runner    (1000) runner    (1000)      740 2023-04-23 06:40:28.000000 CommonlyTools-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-23 14:25:28.270012 CommonlyTools-2.0.1/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-23 14:25:28.266012 CommonlyTools-2.0.1/CommonlyTools.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1650 2023-04-23 14:25:27.000000 CommonlyTools-2.0.1/CommonlyTools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      278 2023-04-23 14:25:28.000000 CommonlyTools-2.0.1/CommonlyTools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-23 14:25:27.000000 CommonlyTools-2.0.1/CommonlyTools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       18 2023-04-23 14:25:27.000000 CommonlyTools-2.0.1/CommonlyTools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       14 2023-04-23 14:25:27.000000 CommonlyTools-2.0.1/CommonlyTools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     1062 2023-04-23 04:55:31.000000 CommonlyTools-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     1650 2023-04-23 14:25:28.266012 CommonlyTools-2.0.1/PKG-INFO
+-rw-------   0 runner    (1000) runner    (1000)      910 2023-04-23 06:38:57.000000 CommonlyTools-2.0.1/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-23 14:25:28.266012 CommonlyTools-2.0.1/commonlytools/
+-rw-------   0 runner    (1000) runner    (1000)       24 2023-04-23 04:55:26.000000 CommonlyTools-2.0.1/commonlytools/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)     2313 2023-04-23 14:24:09.000000 CommonlyTools-2.0.1/commonlytools/discohook.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      312 2023-04-23 02:53:39.000000 CommonlyTools-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-04-23 14:25:28.270012 CommonlyTools-2.0.1/setup.cfg
+-rw-------   0 runner    (1000) runner    (1000)      740 2023-04-23 14:24:20.000000 CommonlyTools-2.0.1/setup.py
```

### Comparing `CommonlyTools-2.0.0/CommonlyTools.egg-info/PKG-INFO` & `CommonlyTools-2.0.1/CommonlyTools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CommonlyTools
-Version: 2.0.0
+Version: 2.0.1
 Summary: You will use Python easily!
 Home-page: https://github.com/maxgamil110331/CommonlyTools
 Author: MaxPython110331
 Author-email: dengxiangcheng110331@gmail.com
 License: MIT
 Description: # CommonlyTools
```

### Comparing `CommonlyTools-2.0.0/LICENSE` & `CommonlyTools-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `CommonlyTools-2.0.0/PKG-INFO` & `CommonlyTools-2.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CommonlyTools
-Version: 2.0.0
+Version: 2.0.1
 Summary: You will use Python easily!
 Home-page: https://github.com/maxgamil110331/CommonlyTools
 Author: MaxPython110331
 Author-email: dengxiangcheng110331@gmail.com
 License: MIT
 Description: # CommonlyTools
```

### Comparing `CommonlyTools-2.0.0/README.md` & `CommonlyTools-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `CommonlyTools-2.0.0/commonlytools/discohook.py` & `CommonlyTools-2.0.1/commonlytools/discohook.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import requests
 import datetime
 
 
 def Colour(colour:int=0):
-    colour=int(str(colour), 10)
+    colour=int(f"{colour}", 10)
     return colour
 
 
 def Timestamp(timestamp:datetime.datetime):
     return f"{timestamp.year}-{timestamp.month}-{timestamp.day}T{timestamp.hour}:{timestamp.minute}:{timestamp.second}.{timestamp.microsecond}Z"
```

### Comparing `CommonlyTools-2.0.0/setup.py` & `CommonlyTools-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="CommonlyTools",
-    version="2.0.0",
+    version="2.0.1",
     author="MaxPython110331",
     author_email="dengxiangcheng110331@gmail.com",
     description="You will use Python easily!",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://github.com/maxgamil110331/CommonlyTools",
```

