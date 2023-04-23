# Comparing `tmp/CommonlyTools-1.0.2.tar.gz` & `tmp/CommonlyTools-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CommonlyTools-1.0.2.tar", last modified: Sun Apr 23 03:22:46 2023, max compression
+gzip compressed data, was "CommonlyTools-1.0.3.tar", last modified: Sun Apr 23 04:39:54 2023, max compression
```

## Comparing `CommonlyTools-1.0.2.tar` & `CommonlyTools-1.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-23 03:22:46.776621 CommonlyTools-1.0.2/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-23 03:22:46.772621 CommonlyTools-1.0.2/CommonlyTools.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1581 2023-04-23 03:22:46.000000 CommonlyTools-1.0.2/CommonlyTools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      198 2023-04-23 03:22:46.000000 CommonlyTools-1.0.2/CommonlyTools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-23 03:22:46.000000 CommonlyTools-1.0.2/CommonlyTools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       18 2023-04-23 03:22:46.000000 CommonlyTools-1.0.2/CommonlyTools.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-23 03:22:46.000000 CommonlyTools-1.0.2/CommonlyTools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     1581 2023-04-23 03:22:46.776621 CommonlyTools-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      312 2023-04-23 02:53:39.000000 CommonlyTools-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-04-23 03:22:46.776621 CommonlyTools-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-23 04:39:54.835195 CommonlyTools-1.0.3/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-23 04:39:54.835195 CommonlyTools-1.0.3/CommonlyTools.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1650 2023-04-23 04:39:54.000000 CommonlyTools-1.0.3/CommonlyTools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      198 2023-04-23 04:39:54.000000 CommonlyTools-1.0.3/CommonlyTools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-23 04:39:54.000000 CommonlyTools-1.0.3/CommonlyTools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       18 2023-04-23 04:39:54.000000 CommonlyTools-1.0.3/CommonlyTools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-23 04:39:54.000000 CommonlyTools-1.0.3/CommonlyTools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     1650 2023-04-23 04:39:54.835195 CommonlyTools-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      312 2023-04-23 02:53:39.000000 CommonlyTools-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-04-23 04:39:54.835195 CommonlyTools-1.0.3/setup.cfg
```

### Comparing `CommonlyTools-1.0.2/CommonlyTools.egg-info/PKG-INFO` & `CommonlyTools-1.0.3/CommonlyTools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: CommonlyTools
-Version: 1.0.2
+Version: 1.0.3
 Summary: You will use Python easily!
 Home-page: https://github.com/maxgamil110331/CommonlyTools
 Author: MaxPython110331
+Author-email: dengxiangcheng110331@gmail.com
 License: MIT
 Description: # CommonlyTools
         
         ----------
         
         How to use CommonlyTools?
         >```pip install CommonlyTools```
@@ -32,13 +33,14 @@
         >>>discohook.send(webhook_url="...", username="...", avatar_url="...", content="...", embeds=[...])
         >>>```
         >>
         >>Step 3
         >>>```
         >>>Message was sent!
         >>>```
+Keywords: CommonlyTools
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `CommonlyTools-1.0.2/PKG-INFO` & `CommonlyTools-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: CommonlyTools
-Version: 1.0.2
+Version: 1.0.3
 Summary: You will use Python easily!
 Home-page: https://github.com/maxgamil110331/CommonlyTools
 Author: MaxPython110331
+Author-email: dengxiangcheng110331@gmail.com
 License: MIT
 Description: # CommonlyTools
         
         ----------
         
         How to use CommonlyTools?
         >```pip install CommonlyTools```
@@ -32,13 +33,14 @@
         >>>discohook.send(webhook_url="...", username="...", avatar_url="...", content="...", embeds=[...])
         >>>```
         >>
         >>Step 3
         >>>```
         >>>Message was sent!
         >>>```
+Keywords: CommonlyTools
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

