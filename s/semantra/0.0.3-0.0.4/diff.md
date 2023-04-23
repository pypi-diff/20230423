# Comparing `tmp/semantra-0.0.3.tar.gz` & `tmp/semantra-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantra-0.0.3.tar", last modified: Sun Apr 23 04:21:54 2023, max compression
+gzip compressed data, was "semantra-0.0.4.tar", last modified: Sun Apr 23 04:25:40 2023, max compression
```

## Comparing `semantra-0.0.3.tar` & `semantra-0.0.4.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 04:21:54.341242 semantra-0.0.3/
--rw-r--r--   0 freedmand   (501) staff       (20)     1071 2023-03-31 03:28:18.000000 semantra-0.0.3/LICENSE
--rw-r--r--   0 freedmand   (501) staff       (20)       66 2023-04-23 04:21:11.000000 semantra-0.0.3/MANIFEST.in
--rw-r--r--   0 freedmand   (501) staff       (20)     3488 2023-04-23 04:21:54.341055 semantra-0.0.3/PKG-INFO
--rw-r--r--   0 freedmand   (501) staff       (20)     3102 2023-04-16 16:45:22.000000 semantra-0.0.3/README.md
--rw-r--r--   0 freedmand   (501) staff       (20)        5 2023-04-23 04:18:35.000000 semantra-0.0.3/VERSION
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 04:21:54.331371 semantra-0.0.3/client/
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 04:21:54.334231 semantra-0.0.3/client/public/
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 04:21:54.336502 semantra-0.0.3/client/public/build/
--rw-r--r--   0 freedmand   (501) staff       (20)    14441 2023-04-22 21:42:14.000000 semantra-0.0.3/client/public/build/bundle.css
--rw-r--r--   0 freedmand   (501) staff       (20)   449074 2023-04-22 21:42:14.000000 semantra-0.0.3/client/public/build/bundle.js
--rw-r--r--   0 freedmand   (501) staff       (20)  1495716 2023-04-22 21:42:14.000000 semantra-0.0.3/client/public/build/bundle.js.map
--rw-r--r--   0 freedmand   (501) staff       (20)     3300 2023-04-09 04:23:49.000000 semantra-0.0.3/client/public/favicon.png
--rw-r--r--   0 freedmand   (501) staff       (20)      890 2023-02-15 22:52:41.000000 semantra-0.0.3/client/public/global.css
--rw-r--r--   0 freedmand   (501) staff       (20)      434 2023-04-09 20:49:05.000000 semantra-0.0.3/client/public/index.html
--rw-r--r--   0 freedmand   (501) staff       (20)      156 2023-04-23 03:03:00.000000 semantra-0.0.3/requirements.txt
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 04:21:54.340843 semantra-0.0.3/semantra.egg-info/
--rw-r--r--   0 freedmand   (501) staff       (20)     3488 2023-04-23 04:21:54.000000 semantra-0.0.3/semantra.egg-info/PKG-INFO
--rw-r--r--   0 freedmand   (501) staff       (20)      440 2023-04-23 04:21:54.000000 semantra-0.0.3/semantra.egg-info/SOURCES.txt
--rw-r--r--   0 freedmand   (501) staff       (20)        1 2023-04-23 04:21:54.000000 semantra-0.0.3/semantra.egg-info/dependency_links.txt
--rw-r--r--   0 freedmand   (501) staff       (20)       43 2023-04-23 04:21:54.000000 semantra-0.0.3/semantra.egg-info/entry_points.txt
--rw-r--r--   0 freedmand   (501) staff       (20)      156 2023-04-23 04:21:54.000000 semantra-0.0.3/semantra.egg-info/requires.txt
--rw-r--r--   0 freedmand   (501) staff       (20)        9 2023-04-23 04:21:54.000000 semantra-0.0.3/semantra.egg-info/top_level.txt
--rw-r--r--   0 freedmand   (501) staff       (20)    28707 2023-04-23 04:15:34.000000 semantra-0.0.3/semantra.py
--rw-r--r--   0 freedmand   (501) staff       (20)       38 2023-04-23 04:21:54.341287 semantra-0.0.3/setup.cfg
--rw-r--r--   0 freedmand   (501) staff       (20)     1150 2023-04-23 04:15:11.000000 semantra-0.0.3/setup.py
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 04:25:40.322369 semantra-0.0.4/
+-rw-r--r--   0 freedmand   (501) staff       (20)     1071 2023-03-31 03:28:18.000000 semantra-0.0.4/LICENSE
+-rw-r--r--   0 freedmand   (501) staff       (20)       66 2023-04-23 04:21:11.000000 semantra-0.0.4/MANIFEST.in
+-rw-r--r--   0 freedmand   (501) staff       (20)     3488 2023-04-23 04:25:40.322196 semantra-0.0.4/PKG-INFO
+-rw-r--r--   0 freedmand   (501) staff       (20)     3102 2023-04-16 16:45:22.000000 semantra-0.0.4/README.md
+-rw-r--r--   0 freedmand   (501) staff       (20)        5 2023-04-23 04:24:53.000000 semantra-0.0.4/VERSION
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 04:25:40.314727 semantra-0.0.4/client/
+-rw-r--r--   0 freedmand   (501) staff       (20)        0 2023-04-23 04:23:41.000000 semantra-0.0.4/client/__init__.py
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 04:25:40.315447 semantra-0.0.4/client/public/
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 04:25:40.317427 semantra-0.0.4/client/public/build/
+-rw-r--r--   0 freedmand   (501) staff       (20)    14441 2023-04-22 21:42:14.000000 semantra-0.0.4/client/public/build/bundle.css
+-rw-r--r--   0 freedmand   (501) staff       (20)   449074 2023-04-22 21:42:14.000000 semantra-0.0.4/client/public/build/bundle.js
+-rw-r--r--   0 freedmand   (501) staff       (20)  1495716 2023-04-22 21:42:14.000000 semantra-0.0.4/client/public/build/bundle.js.map
+-rw-r--r--   0 freedmand   (501) staff       (20)     3300 2023-04-09 04:23:49.000000 semantra-0.0.4/client/public/favicon.png
+-rw-r--r--   0 freedmand   (501) staff       (20)      890 2023-02-15 22:52:41.000000 semantra-0.0.4/client/public/global.css
+-rw-r--r--   0 freedmand   (501) staff       (20)      434 2023-04-09 20:49:05.000000 semantra-0.0.4/client/public/index.html
+-rw-r--r--   0 freedmand   (501) staff       (20)      156 2023-04-23 03:03:00.000000 semantra-0.0.4/requirements.txt
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 04:25:40.321987 semantra-0.0.4/semantra.egg-info/
+-rw-r--r--   0 freedmand   (501) staff       (20)     3488 2023-04-23 04:25:40.000000 semantra-0.0.4/semantra.egg-info/PKG-INFO
+-rw-r--r--   0 freedmand   (501) staff       (20)      459 2023-04-23 04:25:40.000000 semantra-0.0.4/semantra.egg-info/SOURCES.txt
+-rw-r--r--   0 freedmand   (501) staff       (20)        1 2023-04-23 04:25:40.000000 semantra-0.0.4/semantra.egg-info/dependency_links.txt
+-rw-r--r--   0 freedmand   (501) staff       (20)       43 2023-04-23 04:25:40.000000 semantra-0.0.4/semantra.egg-info/entry_points.txt
+-rw-r--r--   0 freedmand   (501) staff       (20)      156 2023-04-23 04:25:40.000000 semantra-0.0.4/semantra.egg-info/requires.txt
+-rw-r--r--   0 freedmand   (501) staff       (20)       16 2023-04-23 04:25:40.000000 semantra-0.0.4/semantra.egg-info/top_level.txt
+-rw-r--r--   0 freedmand   (501) staff       (20)    28707 2023-04-23 04:15:34.000000 semantra-0.0.4/semantra.py
+-rw-r--r--   0 freedmand   (501) staff       (20)       38 2023-04-23 04:25:40.322417 semantra-0.0.4/setup.cfg
+-rw-r--r--   0 freedmand   (501) staff       (20)     1150 2023-04-23 04:15:11.000000 semantra-0.0.4/setup.py
```

### Comparing `semantra-0.0.3/LICENSE` & `semantra-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `semantra-0.0.3/PKG-INFO` & `semantra-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantra
-Version: 0.0.3
+Version: 0.0.4
 Summary: A semantic search CLI tool
 Home-page: https://github.com/freedmand/semantra
 Author: Dylan Freedman
 Author-email: freedmand@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `semantra-0.0.3/README.md` & `semantra-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `semantra-0.0.3/client/public/build/bundle.css` & `semantra-0.0.4/client/public/build/bundle.css`

 * *Files identical despite different names*

### Comparing `semantra-0.0.3/client/public/build/bundle.js` & `semantra-0.0.4/client/public/build/bundle.js`

 * *Files identical despite different names*

### Comparing `semantra-0.0.3/client/public/build/bundle.js.map` & `semantra-0.0.4/client/public/build/bundle.js.map`

 * *Files identical despite different names*

### Comparing `semantra-0.0.3/client/public/favicon.png` & `semantra-0.0.4/client/public/favicon.png`

 * *Files identical despite different names*

### Comparing `semantra-0.0.3/client/public/global.css` & `semantra-0.0.4/client/public/global.css`

 * *Files identical despite different names*

### Comparing `semantra-0.0.3/semantra.egg-info/PKG-INFO` & `semantra-0.0.4/semantra.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantra
-Version: 0.0.3
+Version: 0.0.4
 Summary: A semantic search CLI tool
 Home-page: https://github.com/freedmand/semantra
 Author: Dylan Freedman
 Author-email: freedmand@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `semantra-0.0.3/semantra.py` & `semantra-0.0.4/semantra.py`

 * *Files identical despite different names*

### Comparing `semantra-0.0.3/setup.py` & `semantra-0.0.4/setup.py`

 * *Files identical despite different names*

