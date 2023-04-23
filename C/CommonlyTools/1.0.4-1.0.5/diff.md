# Comparing `tmp/CommonlyTools-1.0.4.tar.gz` & `tmp/CommonlyTools-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CommonlyTools-1.0.4.tar", last modified: Sun Apr 23 04:50:45 2023, max compression
+gzip compressed data, was "CommonlyTools-1.0.5.tar", last modified: Sun Apr 23 04:56:28 2023, max compression
```

## Comparing `CommonlyTools-1.0.4.tar` & `CommonlyTools-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-23 04:50:45.034299 CommonlyTools-1.0.4/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-23 04:50:45.030299 CommonlyTools-1.0.4/CommonlyTools.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1650 2023-04-23 04:50:44.000000 CommonlyTools-1.0.4/CommonlyTools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      265 2023-04-23 04:50:44.000000 CommonlyTools-1.0.4/CommonlyTools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-23 04:50:44.000000 CommonlyTools-1.0.4/CommonlyTools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       18 2023-04-23 04:50:44.000000 CommonlyTools-1.0.4/CommonlyTools.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       21 2023-04-23 04:50:44.000000 CommonlyTools-1.0.4/CommonlyTools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-23 04:50:45.030299 CommonlyTools-1.0.4/EasyPY/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-23 04:50:45.030299 CommonlyTools-1.0.4/EasyPY/CommonlyTools/
--rw-------   0 runner    (1000) runner    (1000)       24 2023-04-23 04:34:44.000000 CommonlyTools-1.0.4/EasyPY/CommonlyTools/__init__.py
--rw-------   0 runner    (1000) runner    (1000)     2313 2023-04-23 03:29:39.000000 CommonlyTools-1.0.4/EasyPY/CommonlyTools/discohook.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1650 2023-04-23 04:50:45.030299 CommonlyTools-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      312 2023-04-23 02:53:39.000000 CommonlyTools-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-04-23 04:50:45.034299 CommonlyTools-1.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-23 04:56:28.629826 CommonlyTools-1.0.5/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-23 04:56:28.629826 CommonlyTools-1.0.5/CommonlyTools.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1650 2023-04-23 04:56:28.000000 CommonlyTools-1.0.5/CommonlyTools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      278 2023-04-23 04:56:28.000000 CommonlyTools-1.0.5/CommonlyTools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-23 04:56:28.000000 CommonlyTools-1.0.5/CommonlyTools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       18 2023-04-23 04:56:28.000000 CommonlyTools-1.0.5/CommonlyTools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       14 2023-04-23 04:56:28.000000 CommonlyTools-1.0.5/CommonlyTools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     1062 2023-04-23 04:55:31.000000 CommonlyTools-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     1650 2023-04-23 04:56:28.629826 CommonlyTools-1.0.5/PKG-INFO
+-rw-------   0 runner    (1000) runner    (1000)      910 2023-04-23 04:55:35.000000 CommonlyTools-1.0.5/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-23 04:56:28.629826 CommonlyTools-1.0.5/commonlytools/
+-rw-------   0 runner    (1000) runner    (1000)       24 2023-04-23 04:55:26.000000 CommonlyTools-1.0.5/commonlytools/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)     2313 2023-04-23 04:55:26.000000 CommonlyTools-1.0.5/commonlytools/discohook.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      312 2023-04-23 02:53:39.000000 CommonlyTools-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-04-23 04:56:28.629826 CommonlyTools-1.0.5/setup.cfg
+-rw-------   0 runner    (1000) runner    (1000)      740 2023-04-23 04:56:16.000000 CommonlyTools-1.0.5/setup.py
```

### Comparing `CommonlyTools-1.0.4/CommonlyTools.egg-info/PKG-INFO` & `CommonlyTools-1.0.5/CommonlyTools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CommonlyTools
-Version: 1.0.4
+Version: 1.0.5
 Summary: You will use Python easily!
 Home-page: https://github.com/maxgamil110331/CommonlyTools
 Author: MaxPython110331
 Author-email: dengxiangcheng110331@gmail.com
 License: MIT
 Description: # CommonlyTools
```

### Comparing `CommonlyTools-1.0.4/EasyPY/CommonlyTools/discohook.py` & `CommonlyTools-1.0.5/commonlytools/discohook.py`

 * *Files identical despite different names*

### Comparing `CommonlyTools-1.0.4/PKG-INFO` & `CommonlyTools-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CommonlyTools
-Version: 1.0.4
+Version: 1.0.5
 Summary: You will use Python easily!
 Home-page: https://github.com/maxgamil110331/CommonlyTools
 Author: MaxPython110331
 Author-email: dengxiangcheng110331@gmail.com
 License: MIT
 Description: # CommonlyTools
```

