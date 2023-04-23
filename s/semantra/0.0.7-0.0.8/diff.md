# Comparing `tmp/semantra-0.0.7.tar.gz` & `tmp/semantra-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantra-0.0.7.tar", last modified: Sun Apr 23 12:17:08 2023, max compression
+gzip compressed data, was "semantra-0.0.8.tar", last modified: Sun Apr 23 12:20:30 2023, max compression
```

## Comparing `semantra-0.0.7.tar` & `semantra-0.0.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 12:17:08.388695 semantra-0.0.7/
--rw-r--r--   0 freedmand   (501) staff       (20)     1071 2023-03-31 03:28:18.000000 semantra-0.0.7/LICENSE
--rw-r--r--   0 freedmand   (501) staff       (20)      102 2023-04-23 12:16:47.000000 semantra-0.0.7/MANIFEST.in
--rw-r--r--   0 freedmand   (501) staff       (20)     3488 2023-04-23 12:17:08.388531 semantra-0.0.7/PKG-INFO
--rw-r--r--   0 freedmand   (501) staff       (20)     3102 2023-04-16 16:45:22.000000 semantra-0.0.7/README.md
--rw-r--r--   0 freedmand   (501) staff       (20)        5 2023-04-23 12:15:26.000000 semantra-0.0.7/VERSION
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 12:17:08.378435 semantra-0.0.7/client/
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 12:17:08.380597 semantra-0.0.7/client/public/
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 12:17:08.383045 semantra-0.0.7/client/public/build/
--rw-r--r--   0 freedmand   (501) staff       (20)    14441 2023-04-22 21:42:14.000000 semantra-0.0.7/client/public/build/bundle.css
--rw-r--r--   0 freedmand   (501) staff       (20)   449074 2023-04-22 21:42:14.000000 semantra-0.0.7/client/public/build/bundle.js
--rw-r--r--   0 freedmand   (501) staff       (20)  1495716 2023-04-22 21:42:14.000000 semantra-0.0.7/client/public/build/bundle.js.map
--rw-r--r--   0 freedmand   (501) staff       (20)     3300 2023-04-09 04:23:49.000000 semantra-0.0.7/client/public/favicon.png
--rw-r--r--   0 freedmand   (501) staff       (20)      890 2023-02-15 22:52:41.000000 semantra-0.0.7/client/public/global.css
--rw-r--r--   0 freedmand   (501) staff       (20)      434 2023-04-09 20:49:05.000000 semantra-0.0.7/client/public/index.html
--rw-r--r--   0 freedmand   (501) staff       (20)      156 2023-04-23 03:03:00.000000 semantra-0.0.7/requirements.txt
--rw-r--r--   0 freedmand   (501) staff       (20)       38 2023-04-23 12:17:08.388736 semantra-0.0.7/setup.cfg
--rw-r--r--   0 freedmand   (501) staff       (20)     1194 2023-04-23 12:14:58.000000 semantra-0.0.7/setup.py
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 12:17:08.378723 semantra-0.0.7/src/
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 12:17:08.387286 semantra-0.0.7/src/semantra/
--rw-r--r--   0 freedmand   (501) staff       (20)        0 2023-04-23 04:39:23.000000 semantra-0.0.7/src/semantra/__init__.py
--rw-r--r--   0 freedmand   (501) staff       (20)    11172 2023-04-20 17:02:30.000000 semantra-0.0.7/src/semantra/models.py
--rw-r--r--   0 freedmand   (501) staff       (20)     3118 2023-04-23 04:31:52.000000 semantra-0.0.7/src/semantra/pdf.py
--rw-r--r--   0 freedmand   (501) staff       (20)    28787 2023-04-23 12:15:14.000000 semantra-0.0.7/src/semantra/semantra.py
--rw-r--r--   0 freedmand   (501) staff       (20)     4524 2023-04-22 20:05:23.000000 semantra-0.0.7/src/semantra/util.py
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 12:17:08.388317 semantra-0.0.7/src/semantra.egg-info/
--rw-r--r--   0 freedmand   (501) staff       (20)     3488 2023-04-23 12:17:08.000000 semantra-0.0.7/src/semantra.egg-info/PKG-INFO
--rw-r--r--   0 freedmand   (501) staff       (20)      566 2023-04-23 12:17:08.000000 semantra-0.0.7/src/semantra.egg-info/SOURCES.txt
--rw-r--r--   0 freedmand   (501) staff       (20)        1 2023-04-23 12:17:08.000000 semantra-0.0.7/src/semantra.egg-info/dependency_links.txt
--rw-r--r--   0 freedmand   (501) staff       (20)       52 2023-04-23 12:17:08.000000 semantra-0.0.7/src/semantra.egg-info/entry_points.txt
--rw-r--r--   0 freedmand   (501) staff       (20)      156 2023-04-23 12:17:08.000000 semantra-0.0.7/src/semantra.egg-info/requires.txt
--rw-r--r--   0 freedmand   (501) staff       (20)        1 2023-04-23 12:17:08.000000 semantra-0.0.7/src/semantra.egg-info/top_level.txt
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 12:20:30.733525 semantra-0.0.8/
+-rw-r--r--   0 freedmand   (501) staff       (20)     1071 2023-03-31 03:28:18.000000 semantra-0.0.8/LICENSE
+-rw-r--r--   0 freedmand   (501) staff       (20)      102 2023-04-23 12:16:47.000000 semantra-0.0.8/MANIFEST.in
+-rw-r--r--   0 freedmand   (501) staff       (20)     3488 2023-04-23 12:20:30.733363 semantra-0.0.8/PKG-INFO
+-rw-r--r--   0 freedmand   (501) staff       (20)     3102 2023-04-16 16:45:22.000000 semantra-0.0.8/README.md
+-rw-r--r--   0 freedmand   (501) staff       (20)        5 2023-04-23 12:20:01.000000 semantra-0.0.8/VERSION
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 12:20:30.722785 semantra-0.0.8/client/
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 12:20:30.724829 semantra-0.0.8/client/public/
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 12:20:30.726884 semantra-0.0.8/client/public/build/
+-rw-r--r--   0 freedmand   (501) staff       (20)    14441 2023-04-22 21:42:14.000000 semantra-0.0.8/client/public/build/bundle.css
+-rw-r--r--   0 freedmand   (501) staff       (20)   449074 2023-04-22 21:42:14.000000 semantra-0.0.8/client/public/build/bundle.js
+-rw-r--r--   0 freedmand   (501) staff       (20)  1495716 2023-04-22 21:42:14.000000 semantra-0.0.8/client/public/build/bundle.js.map
+-rw-r--r--   0 freedmand   (501) staff       (20)     3300 2023-04-09 04:23:49.000000 semantra-0.0.8/client/public/favicon.png
+-rw-r--r--   0 freedmand   (501) staff       (20)      890 2023-02-15 22:52:41.000000 semantra-0.0.8/client/public/global.css
+-rw-r--r--   0 freedmand   (501) staff       (20)      434 2023-04-09 20:49:05.000000 semantra-0.0.8/client/public/index.html
+-rw-r--r--   0 freedmand   (501) staff       (20)      156 2023-04-23 03:03:00.000000 semantra-0.0.8/requirements.txt
+-rw-r--r--   0 freedmand   (501) staff       (20)       38 2023-04-23 12:20:30.733568 semantra-0.0.8/setup.cfg
+-rw-r--r--   0 freedmand   (501) staff       (20)     1185 2023-04-23 12:19:56.000000 semantra-0.0.8/setup.py
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 12:20:30.723062 semantra-0.0.8/src/
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 12:20:30.732085 semantra-0.0.8/src/semantra/
+-rw-r--r--   0 freedmand   (501) staff       (20)        0 2023-04-23 04:39:23.000000 semantra-0.0.8/src/semantra/__init__.py
+-rw-r--r--   0 freedmand   (501) staff       (20)    11172 2023-04-20 17:02:30.000000 semantra-0.0.8/src/semantra/models.py
+-rw-r--r--   0 freedmand   (501) staff       (20)     3118 2023-04-23 04:31:52.000000 semantra-0.0.8/src/semantra/pdf.py
+-rw-r--r--   0 freedmand   (501) staff       (20)    28787 2023-04-23 12:15:14.000000 semantra-0.0.8/src/semantra/semantra.py
+-rw-r--r--   0 freedmand   (501) staff       (20)     4524 2023-04-22 20:05:23.000000 semantra-0.0.8/src/semantra/util.py
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 12:20:30.733153 semantra-0.0.8/src/semantra.egg-info/
+-rw-r--r--   0 freedmand   (501) staff       (20)     3488 2023-04-23 12:20:30.000000 semantra-0.0.8/src/semantra.egg-info/PKG-INFO
+-rw-r--r--   0 freedmand   (501) staff       (20)      566 2023-04-23 12:20:30.000000 semantra-0.0.8/src/semantra.egg-info/SOURCES.txt
+-rw-r--r--   0 freedmand   (501) staff       (20)        1 2023-04-23 12:20:30.000000 semantra-0.0.8/src/semantra.egg-info/dependency_links.txt
+-rw-r--r--   0 freedmand   (501) staff       (20)       52 2023-04-23 12:20:30.000000 semantra-0.0.8/src/semantra.egg-info/entry_points.txt
+-rw-r--r--   0 freedmand   (501) staff       (20)      156 2023-04-23 12:20:30.000000 semantra-0.0.8/src/semantra.egg-info/requires.txt
+-rw-r--r--   0 freedmand   (501) staff       (20)        9 2023-04-23 12:20:30.000000 semantra-0.0.8/src/semantra.egg-info/top_level.txt
```

### Comparing `semantra-0.0.7/LICENSE` & `semantra-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `semantra-0.0.7/PKG-INFO` & `semantra-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantra
-Version: 0.0.7
+Version: 0.0.8
 Summary: A semantic search CLI tool
 Home-page: https://github.com/freedmand/semantra
 Author: Dylan Freedman
 Author-email: freedmand@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `semantra-0.0.7/README.md` & `semantra-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `semantra-0.0.7/client/public/build/bundle.css` & `semantra-0.0.8/client/public/build/bundle.css`

 * *Files identical despite different names*

### Comparing `semantra-0.0.7/client/public/build/bundle.js` & `semantra-0.0.8/client/public/build/bundle.js`

 * *Files identical despite different names*

### Comparing `semantra-0.0.7/client/public/build/bundle.js.map` & `semantra-0.0.8/client/public/build/bundle.js.map`

 * *Files identical despite different names*

### Comparing `semantra-0.0.7/client/public/favicon.png` & `semantra-0.0.8/client/public/favicon.png`

 * *Files identical despite different names*

### Comparing `semantra-0.0.7/client/public/global.css` & `semantra-0.0.8/client/public/global.css`

 * *Files identical despite different names*

### Comparing `semantra-0.0.7/setup.py` & `semantra-0.0.8/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     version=version,
     description="A semantic search CLI tool",
     long_description=long_description,
     url="https://github.com/freedmand/semantra",
     author="Dylan Freedman",
     author_email="freedmand@gmail.com",
     packages=find_packages(
-        where="src/semantra",
+        where="src",
     ),
     install_requires=requirements,
     python_requires=">=3.9",
     include_package_data=True,
     package_data={"": ["client/public", "VERSION"]},
     package_dir={"": "src"},
     classifiers=[
```

### Comparing `semantra-0.0.7/src/semantra/models.py` & `semantra-0.0.8/src/semantra/models.py`

 * *Files identical despite different names*

### Comparing `semantra-0.0.7/src/semantra/pdf.py` & `semantra-0.0.8/src/semantra/pdf.py`

 * *Files identical despite different names*

### Comparing `semantra-0.0.7/src/semantra/semantra.py` & `semantra-0.0.8/src/semantra/semantra.py`

 * *Files identical despite different names*

### Comparing `semantra-0.0.7/src/semantra/util.py` & `semantra-0.0.8/src/semantra/util.py`

 * *Files identical despite different names*

### Comparing `semantra-0.0.7/src/semantra.egg-info/PKG-INFO` & `semantra-0.0.8/src/semantra.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantra
-Version: 0.0.7
+Version: 0.0.8
 Summary: A semantic search CLI tool
 Home-page: https://github.com/freedmand/semantra
 Author: Dylan Freedman
 Author-email: freedmand@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `semantra-0.0.7/src/semantra.egg-info/SOURCES.txt` & `semantra-0.0.8/src/semantra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

