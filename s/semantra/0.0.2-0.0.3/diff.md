# Comparing `tmp/semantra-0.0.2.tar.gz` & `tmp/semantra-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantra-0.0.2.tar", last modified: Sun Apr 23 04:17:17 2023, max compression
+gzip compressed data, was "semantra-0.0.3.tar", last modified: Sun Apr 23 04:21:54 2023, max compression
```

## Comparing `semantra-0.0.2.tar` & `semantra-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,26 @@
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 04:17:17.223431 semantra-0.0.2/
--rw-r--r--   0 freedmand   (501) staff       (20)     1071 2023-03-31 03:28:18.000000 semantra-0.0.2/LICENSE
--rw-r--r--   0 freedmand   (501) staff       (20)       32 2023-04-23 04:14:55.000000 semantra-0.0.2/MANIFEST.in
--rw-r--r--   0 freedmand   (501) staff       (20)     3488 2023-04-23 04:17:17.223287 semantra-0.0.2/PKG-INFO
--rw-r--r--   0 freedmand   (501) staff       (20)     3102 2023-04-16 16:45:22.000000 semantra-0.0.2/README.md
--rw-r--r--   0 freedmand   (501) staff       (20)        5 2023-04-23 04:16:46.000000 semantra-0.0.2/VERSION
--rw-r--r--   0 freedmand   (501) staff       (20)      156 2023-04-23 03:03:00.000000 semantra-0.0.2/requirements.txt
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 04:17:17.223100 semantra-0.0.2/semantra.egg-info/
--rw-r--r--   0 freedmand   (501) staff       (20)     3488 2023-04-23 04:17:17.000000 semantra-0.0.2/semantra.egg-info/PKG-INFO
--rw-r--r--   0 freedmand   (501) staff       (20)      269 2023-04-23 04:17:17.000000 semantra-0.0.2/semantra.egg-info/SOURCES.txt
--rw-r--r--   0 freedmand   (501) staff       (20)        1 2023-04-23 04:17:17.000000 semantra-0.0.2/semantra.egg-info/dependency_links.txt
--rw-r--r--   0 freedmand   (501) staff       (20)       43 2023-04-23 04:17:17.000000 semantra-0.0.2/semantra.egg-info/entry_points.txt
--rw-r--r--   0 freedmand   (501) staff       (20)      156 2023-04-23 04:17:17.000000 semantra-0.0.2/semantra.egg-info/requires.txt
--rw-r--r--   0 freedmand   (501) staff       (20)        9 2023-04-23 04:17:17.000000 semantra-0.0.2/semantra.egg-info/top_level.txt
--rw-r--r--   0 freedmand   (501) staff       (20)    28707 2023-04-23 04:15:34.000000 semantra-0.0.2/semantra.py
--rw-r--r--   0 freedmand   (501) staff       (20)       38 2023-04-23 04:17:17.223478 semantra-0.0.2/setup.cfg
--rw-r--r--   0 freedmand   (501) staff       (20)     1150 2023-04-23 04:15:11.000000 semantra-0.0.2/setup.py
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 04:21:54.341242 semantra-0.0.3/
+-rw-r--r--   0 freedmand   (501) staff       (20)     1071 2023-03-31 03:28:18.000000 semantra-0.0.3/LICENSE
+-rw-r--r--   0 freedmand   (501) staff       (20)       66 2023-04-23 04:21:11.000000 semantra-0.0.3/MANIFEST.in
+-rw-r--r--   0 freedmand   (501) staff       (20)     3488 2023-04-23 04:21:54.341055 semantra-0.0.3/PKG-INFO
+-rw-r--r--   0 freedmand   (501) staff       (20)     3102 2023-04-16 16:45:22.000000 semantra-0.0.3/README.md
+-rw-r--r--   0 freedmand   (501) staff       (20)        5 2023-04-23 04:18:35.000000 semantra-0.0.3/VERSION
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 04:21:54.331371 semantra-0.0.3/client/
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 04:21:54.334231 semantra-0.0.3/client/public/
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 04:21:54.336502 semantra-0.0.3/client/public/build/
+-rw-r--r--   0 freedmand   (501) staff       (20)    14441 2023-04-22 21:42:14.000000 semantra-0.0.3/client/public/build/bundle.css
+-rw-r--r--   0 freedmand   (501) staff       (20)   449074 2023-04-22 21:42:14.000000 semantra-0.0.3/client/public/build/bundle.js
+-rw-r--r--   0 freedmand   (501) staff       (20)  1495716 2023-04-22 21:42:14.000000 semantra-0.0.3/client/public/build/bundle.js.map
+-rw-r--r--   0 freedmand   (501) staff       (20)     3300 2023-04-09 04:23:49.000000 semantra-0.0.3/client/public/favicon.png
+-rw-r--r--   0 freedmand   (501) staff       (20)      890 2023-02-15 22:52:41.000000 semantra-0.0.3/client/public/global.css
+-rw-r--r--   0 freedmand   (501) staff       (20)      434 2023-04-09 20:49:05.000000 semantra-0.0.3/client/public/index.html
+-rw-r--r--   0 freedmand   (501) staff       (20)      156 2023-04-23 03:03:00.000000 semantra-0.0.3/requirements.txt
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 04:21:54.340843 semantra-0.0.3/semantra.egg-info/
+-rw-r--r--   0 freedmand   (501) staff       (20)     3488 2023-04-23 04:21:54.000000 semantra-0.0.3/semantra.egg-info/PKG-INFO
+-rw-r--r--   0 freedmand   (501) staff       (20)      440 2023-04-23 04:21:54.000000 semantra-0.0.3/semantra.egg-info/SOURCES.txt
+-rw-r--r--   0 freedmand   (501) staff       (20)        1 2023-04-23 04:21:54.000000 semantra-0.0.3/semantra.egg-info/dependency_links.txt
+-rw-r--r--   0 freedmand   (501) staff       (20)       43 2023-04-23 04:21:54.000000 semantra-0.0.3/semantra.egg-info/entry_points.txt
+-rw-r--r--   0 freedmand   (501) staff       (20)      156 2023-04-23 04:21:54.000000 semantra-0.0.3/semantra.egg-info/requires.txt
+-rw-r--r--   0 freedmand   (501) staff       (20)        9 2023-04-23 04:21:54.000000 semantra-0.0.3/semantra.egg-info/top_level.txt
+-rw-r--r--   0 freedmand   (501) staff       (20)    28707 2023-04-23 04:15:34.000000 semantra-0.0.3/semantra.py
+-rw-r--r--   0 freedmand   (501) staff       (20)       38 2023-04-23 04:21:54.341287 semantra-0.0.3/setup.cfg
+-rw-r--r--   0 freedmand   (501) staff       (20)     1150 2023-04-23 04:15:11.000000 semantra-0.0.3/setup.py
```

### Comparing `semantra-0.0.2/LICENSE` & `semantra-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `semantra-0.0.2/PKG-INFO` & `semantra-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantra
-Version: 0.0.2
+Version: 0.0.3
 Summary: A semantic search CLI tool
 Home-page: https://github.com/freedmand/semantra
 Author: Dylan Freedman
 Author-email: freedmand@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `semantra-0.0.2/README.md` & `semantra-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `semantra-0.0.2/semantra.egg-info/PKG-INFO` & `semantra-0.0.3/semantra.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantra
-Version: 0.0.2
+Version: 0.0.3
 Summary: A semantic search CLI tool
 Home-page: https://github.com/freedmand/semantra
 Author: Dylan Freedman
 Author-email: freedmand@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `semantra-0.0.2/semantra.py` & `semantra-0.0.3/semantra.py`

 * *Files identical despite different names*

### Comparing `semantra-0.0.2/setup.py` & `semantra-0.0.3/setup.py`

 * *Files identical despite different names*

