# Comparing `tmp/discoger-1.0.0.tar.gz` & `tmp/discoger-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discoger-1.0.0.tar", last modified: Sun Apr 23 12:26:26 2023, max compression
+gzip compressed data, was "discoger-1.0.1.tar", last modified: Sun Apr 23 12:40:17 2023, max compression
```

## Comparing `discoger-1.0.0.tar` & `discoger-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:26:26.448911 discoger-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-23 12:26:13.000000 discoger-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-23 12:26:26.448911 discoger-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-23 12:26:13.000000 discoger-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:26:26.448911 discoger-1.0.0/discoger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:26:13.000000 discoger-1.0.0/discoger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-23 12:26:13.000000 discoger-1.0.0/discoger/_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-04-23 12:26:13.000000 discoger-1.0.0/discoger/discoger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:26:26.448911 discoger-1.0.0/discoger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-23 12:26:26.000000 discoger-1.0.0/discoger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-23 12:26:26.000000 discoger-1.0.0/discoger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 12:26:26.000000 discoger-1.0.0/discoger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-23 12:26:26.000000 discoger-1.0.0/discoger.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-23 12:26:26.000000 discoger-1.0.0/discoger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-23 12:26:26.000000 discoger-1.0.0/discoger.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-23 12:26:26.448911 discoger-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-04-23 12:26:13.000000 discoger-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:40:17.751697 discoger-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-23 12:40:03.000000 discoger-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-23 12:40:17.751697 discoger-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-23 12:40:03.000000 discoger-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:40:17.747697 discoger-1.0.1/discoger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:40:03.000000 discoger-1.0.1/discoger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-23 12:40:03.000000 discoger-1.0.1/discoger/_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-04-23 12:40:03.000000 discoger-1.0.1/discoger/discoger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:40:17.751697 discoger-1.0.1/discoger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-23 12:40:17.000000 discoger-1.0.1/discoger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-23 12:40:17.000000 discoger-1.0.1/discoger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 12:40:17.000000 discoger-1.0.1/discoger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-23 12:40:17.000000 discoger-1.0.1/discoger.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-23 12:40:17.000000 discoger-1.0.1/discoger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-23 12:40:17.000000 discoger-1.0.1/discoger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-23 12:40:17.751697 discoger-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-04-23 12:40:03.000000 discoger-1.0.1/setup.py
```

### Comparing `discoger-1.0.0/LICENSE` & `discoger-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `discoger-1.0.0/PKG-INFO` & `discoger-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: discoger
-Version: 1.0.0
+Version: 1.0.1
 Summary: Get notification from Discogs
 Home-page: https://github.com/beudbeud/discoger
 Author: Beudbeud
 Author-email: beudbeud@gmail.com
 License: GNU General Public License v3 (GPLv3)
-Download-URL: https://github.com/beudbeud/discoger/archive/1.0.0.tar.gz
+Download-URL: https://github.com/beudbeud/discoger/archive/1.0.1.tar.gz
 Description: # Discoger
         
         Telegram bot for checking if there are new sell in one specific list on Discogs
         
         ## How to use it
         
         ### Installation
```

### Comparing `discoger-1.0.0/README.md` & `discoger-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `discoger-1.0.0/discoger/discoger.py` & `discoger-1.0.1/discoger/discoger.py`

 * *Files identical despite different names*

### Comparing `discoger-1.0.0/discoger.egg-info/PKG-INFO` & `discoger-1.0.1/discoger.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: discoger
-Version: 1.0.0
+Version: 1.0.1
 Summary: Get notification from Discogs
 Home-page: https://github.com/beudbeud/discoger
 Author: Beudbeud
 Author-email: beudbeud@gmail.com
 License: GNU General Public License v3 (GPLv3)
-Download-URL: https://github.com/beudbeud/discoger/archive/1.0.0.tar.gz
+Download-URL: https://github.com/beudbeud/discoger/archive/1.0.1.tar.gz
 Description: # Discoger
         
         Telegram bot for checking if there are new sell in one specific list on Discogs
         
         ## How to use it
         
         ### Installation
```

### Comparing `discoger-1.0.0/setup.py` & `discoger-1.0.1/setup.py`

 * *Files identical despite different names*

