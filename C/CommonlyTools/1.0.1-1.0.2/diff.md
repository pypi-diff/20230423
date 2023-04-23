# Comparing `tmp/CommonlyTools-1.0.1.tar.gz` & `tmp/CommonlyTools-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CommonlyTools-1.0.1.tar", last modified: Sun Apr 23 02:28:53 2023, max compression
+gzip compressed data, was "CommonlyTools-1.0.2.tar", last modified: Sun Apr 23 03:22:46 2023, max compression
```

## Comparing `CommonlyTools-1.0.1.tar` & `CommonlyTools-1.0.2.tar`

### file list

```diff
@@ -1,9 +1,10 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-23 02:28:53.397718 CommonlyTools-1.0.1/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-23 02:28:53.397718 CommonlyTools-1.0.1/CommonlyTools.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1626 2023-04-23 02:28:53.000000 CommonlyTools-1.0.1/CommonlyTools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      183 2023-04-23 02:28:53.000000 CommonlyTools-1.0.1/CommonlyTools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-23 02:28:53.000000 CommonlyTools-1.0.1/CommonlyTools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       18 2023-04-23 02:28:53.000000 CommonlyTools-1.0.1/CommonlyTools.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-23 02:28:53.000000 CommonlyTools-1.0.1/CommonlyTools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     1626 2023-04-23 02:28:53.397718 CommonlyTools-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-04-23 02:28:53.397718 CommonlyTools-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-23 03:22:46.776621 CommonlyTools-1.0.2/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-23 03:22:46.772621 CommonlyTools-1.0.2/CommonlyTools.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1581 2023-04-23 03:22:46.000000 CommonlyTools-1.0.2/CommonlyTools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      198 2023-04-23 03:22:46.000000 CommonlyTools-1.0.2/CommonlyTools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-23 03:22:46.000000 CommonlyTools-1.0.2/CommonlyTools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       18 2023-04-23 03:22:46.000000 CommonlyTools-1.0.2/CommonlyTools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-23 03:22:46.000000 CommonlyTools-1.0.2/CommonlyTools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     1581 2023-04-23 03:22:46.776621 CommonlyTools-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      312 2023-04-23 02:53:39.000000 CommonlyTools-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-04-23 03:22:46.776621 CommonlyTools-1.0.2/setup.cfg
```

### Comparing `CommonlyTools-1.0.1/CommonlyTools.egg-info/PKG-INFO` & `CommonlyTools-1.0.2/CommonlyTools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: CommonlyTools
-Version: 1.0.1
+Version: 1.0.2
 Summary: You will use Python easily!
 Home-page: https://github.com/maxgamil110331/CommonlyTools
 Author: MaxPython110331
-Author-email: dengxiangcheng110331@gmail.com
 License: MIT
 Description: # CommonlyTools
         
         ----------
         
         How to use CommonlyTools?
         >```pip install CommonlyTools```
```

### Comparing `CommonlyTools-1.0.1/PKG-INFO` & `CommonlyTools-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: CommonlyTools
-Version: 1.0.1
+Version: 1.0.2
 Summary: You will use Python easily!
 Home-page: https://github.com/maxgamil110331/CommonlyTools
 Author: MaxPython110331
-Author-email: dengxiangcheng110331@gmail.com
 License: MIT
 Description: # CommonlyTools
         
         ----------
         
         How to use CommonlyTools?
         >```pip install CommonlyTools```
```

