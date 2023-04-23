# Comparing `tmp/semantra-0.0.5.tar.gz` & `tmp/semantra-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantra-0.0.5.tar", last modified: Sun Apr 23 04:29:22 2023, max compression
+gzip compressed data, was "semantra-0.0.6.tar", last modified: Sun Apr 23 04:40:52 2023, max compression
```

## Comparing `semantra-0.0.5.tar` & `semantra-0.0.6.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 04:29:22.704917 semantra-0.0.5/
--rw-r--r--   0 freedmand   (501) staff       (20)     1071 2023-03-31 03:28:18.000000 semantra-0.0.5/LICENSE
--rw-r--r--   0 freedmand   (501) staff       (20)       66 2023-04-23 04:21:11.000000 semantra-0.0.5/MANIFEST.in
--rw-r--r--   0 freedmand   (501) staff       (20)     3488 2023-04-23 04:29:22.704731 semantra-0.0.5/PKG-INFO
--rw-r--r--   0 freedmand   (501) staff       (20)     3102 2023-04-16 16:45:22.000000 semantra-0.0.5/README.md
--rw-r--r--   0 freedmand   (501) staff       (20)        5 2023-04-23 04:29:01.000000 semantra-0.0.5/VERSION
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 04:29:22.695520 semantra-0.0.5/client/
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 04:29:22.698120 semantra-0.0.5/client/public/
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 04:29:22.700417 semantra-0.0.5/client/public/build/
--rw-r--r--   0 freedmand   (501) staff       (20)    14441 2023-04-22 21:42:14.000000 semantra-0.0.5/client/public/build/bundle.css
--rw-r--r--   0 freedmand   (501) staff       (20)   449074 2023-04-22 21:42:14.000000 semantra-0.0.5/client/public/build/bundle.js
--rw-r--r--   0 freedmand   (501) staff       (20)  1495716 2023-04-22 21:42:14.000000 semantra-0.0.5/client/public/build/bundle.js.map
--rw-r--r--   0 freedmand   (501) staff       (20)     3300 2023-04-09 04:23:49.000000 semantra-0.0.5/client/public/favicon.png
--rw-r--r--   0 freedmand   (501) staff       (20)      890 2023-02-15 22:52:41.000000 semantra-0.0.5/client/public/global.css
--rw-r--r--   0 freedmand   (501) staff       (20)      434 2023-04-09 20:49:05.000000 semantra-0.0.5/client/public/index.html
--rw-r--r--   0 freedmand   (501) staff       (20)      156 2023-04-23 03:03:00.000000 semantra-0.0.5/requirements.txt
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 04:29:22.704434 semantra-0.0.5/semantra.egg-info/
--rw-r--r--   0 freedmand   (501) staff       (20)     3488 2023-04-23 04:29:22.000000 semantra-0.0.5/semantra.egg-info/PKG-INFO
--rw-r--r--   0 freedmand   (501) staff       (20)      440 2023-04-23 04:29:22.000000 semantra-0.0.5/semantra.egg-info/SOURCES.txt
--rw-r--r--   0 freedmand   (501) staff       (20)        1 2023-04-23 04:29:22.000000 semantra-0.0.5/semantra.egg-info/dependency_links.txt
--rw-r--r--   0 freedmand   (501) staff       (20)       43 2023-04-23 04:29:22.000000 semantra-0.0.5/semantra.egg-info/entry_points.txt
--rw-r--r--   0 freedmand   (501) staff       (20)      156 2023-04-23 04:29:22.000000 semantra-0.0.5/semantra.egg-info/requires.txt
--rw-r--r--   0 freedmand   (501) staff       (20)        9 2023-04-23 04:29:22.000000 semantra-0.0.5/semantra.egg-info/top_level.txt
--rw-r--r--   0 freedmand   (501) staff       (20)    28707 2023-04-23 04:15:34.000000 semantra-0.0.5/semantra.py
--rw-r--r--   0 freedmand   (501) staff       (20)       38 2023-04-23 04:29:22.704980 semantra-0.0.5/setup.cfg
--rw-r--r--   0 freedmand   (501) staff       (20)     1150 2023-04-23 04:15:11.000000 semantra-0.0.5/setup.py
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 04:40:52.431761 semantra-0.0.6/
+-rw-r--r--   0 freedmand   (501) staff       (20)     1071 2023-03-31 03:28:18.000000 semantra-0.0.6/LICENSE
+-rw-r--r--   0 freedmand   (501) staff       (20)       66 2023-04-23 04:21:11.000000 semantra-0.0.6/MANIFEST.in
+-rw-r--r--   0 freedmand   (501) staff       (20)     3488 2023-04-23 04:40:52.431586 semantra-0.0.6/PKG-INFO
+-rw-r--r--   0 freedmand   (501) staff       (20)     3102 2023-04-16 16:45:22.000000 semantra-0.0.6/README.md
+-rw-r--r--   0 freedmand   (501) staff       (20)        5 2023-04-23 04:40:45.000000 semantra-0.0.6/VERSION
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 04:40:52.422944 semantra-0.0.6/client/
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 04:40:52.425306 semantra-0.0.6/client/public/
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 04:40:52.427219 semantra-0.0.6/client/public/build/
+-rw-r--r--   0 freedmand   (501) staff       (20)    14441 2023-04-22 21:42:14.000000 semantra-0.0.6/client/public/build/bundle.css
+-rw-r--r--   0 freedmand   (501) staff       (20)   449074 2023-04-22 21:42:14.000000 semantra-0.0.6/client/public/build/bundle.js
+-rw-r--r--   0 freedmand   (501) staff       (20)  1495716 2023-04-22 21:42:14.000000 semantra-0.0.6/client/public/build/bundle.js.map
+-rw-r--r--   0 freedmand   (501) staff       (20)     3300 2023-04-09 04:23:49.000000 semantra-0.0.6/client/public/favicon.png
+-rw-r--r--   0 freedmand   (501) staff       (20)      890 2023-02-15 22:52:41.000000 semantra-0.0.6/client/public/global.css
+-rw-r--r--   0 freedmand   (501) staff       (20)      434 2023-04-09 20:49:05.000000 semantra-0.0.6/client/public/index.html
+-rw-r--r--   0 freedmand   (501) staff       (20)      156 2023-04-23 03:03:00.000000 semantra-0.0.6/requirements.txt
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 04:40:52.431326 semantra-0.0.6/semantra.egg-info/
+-rw-r--r--   0 freedmand   (501) staff       (20)     3488 2023-04-23 04:40:52.000000 semantra-0.0.6/semantra.egg-info/PKG-INFO
+-rw-r--r--   0 freedmand   (501) staff       (20)      428 2023-04-23 04:40:52.000000 semantra-0.0.6/semantra.egg-info/SOURCES.txt
+-rw-r--r--   0 freedmand   (501) staff       (20)        1 2023-04-23 04:40:52.000000 semantra-0.0.6/semantra.egg-info/dependency_links.txt
+-rw-r--r--   0 freedmand   (501) staff       (20)       56 2023-04-23 04:40:52.000000 semantra-0.0.6/semantra.egg-info/entry_points.txt
+-rw-r--r--   0 freedmand   (501) staff       (20)      156 2023-04-23 04:40:52.000000 semantra-0.0.6/semantra.egg-info/requires.txt
+-rw-r--r--   0 freedmand   (501) staff       (20)        1 2023-04-23 04:40:52.000000 semantra-0.0.6/semantra.egg-info/top_level.txt
+-rw-r--r--   0 freedmand   (501) staff       (20)       38 2023-04-23 04:40:52.431810 semantra-0.0.6/setup.cfg
+-rw-r--r--   0 freedmand   (501) staff       (20)     1169 2023-04-23 04:39:14.000000 semantra-0.0.6/setup.py
```

### Comparing `semantra-0.0.5/LICENSE` & `semantra-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `semantra-0.0.5/PKG-INFO` & `semantra-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantra
-Version: 0.0.5
+Version: 0.0.6
 Summary: A semantic search CLI tool
 Home-page: https://github.com/freedmand/semantra
 Author: Dylan Freedman
 Author-email: freedmand@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `semantra-0.0.5/README.md` & `semantra-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `semantra-0.0.5/client/public/build/bundle.css` & `semantra-0.0.6/client/public/build/bundle.css`

 * *Files identical despite different names*

### Comparing `semantra-0.0.5/client/public/build/bundle.js` & `semantra-0.0.6/client/public/build/bundle.js`

 * *Files identical despite different names*

### Comparing `semantra-0.0.5/client/public/build/bundle.js.map` & `semantra-0.0.6/client/public/build/bundle.js.map`

 * *Files identical despite different names*

### Comparing `semantra-0.0.5/client/public/favicon.png` & `semantra-0.0.6/client/public/favicon.png`

 * *Files identical despite different names*

### Comparing `semantra-0.0.5/client/public/global.css` & `semantra-0.0.6/client/public/global.css`

 * *Files identical despite different names*

### Comparing `semantra-0.0.5/semantra.egg-info/PKG-INFO` & `semantra-0.0.6/semantra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantra
-Version: 0.0.5
+Version: 0.0.6
 Summary: A semantic search CLI tool
 Home-page: https://github.com/freedmand/semantra
 Author: Dylan Freedman
 Author-email: freedmand@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `semantra-0.0.5/setup.py` & `semantra-0.0.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,24 +18,25 @@
     name="semantra",
     version=version,
     description="A semantic search CLI tool",
     long_description=long_description,
     url="https://github.com/freedmand/semantra",
     author="Dylan Freedman",
     author_email="freedmand@gmail.com",
-    py_modules=["semantra"],
-    packages=find_packages(),
+    packages=find_packages(
+        where="src/semantra",
+    ),
     install_requires=requirements,
     python_requires=">=3.9",
     include_package_data=True,
     package_data={"": ["client/public", "VERSION"]},
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     entry_points={
         "console_scripts": [
-            "semantra = semantra:main",
+            "semantra = src.semantra.semantra:main",
         ]
     },
 )
```

