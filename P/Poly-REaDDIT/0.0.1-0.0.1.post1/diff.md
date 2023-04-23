# Comparing `tmp/Poly-REaDDIT-0.0.1.tar.gz` & `tmp/Poly-REaDDIT-0.0.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Poly-REaDDIT-0.0.1.tar", last modified: Sun Apr 23 10:19:05 2023, max compression
+gzip compressed data, was "Poly-REaDDIT-0.0.1.post1.tar", last modified: Sun Apr 23 10:30:02 2023, max compression
```

## Comparing `Poly-REaDDIT-0.0.1.tar` & `Poly-REaDDIT-0.0.1.post1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 giacomo_giallombardo  (1000) giacomo_giallombardo  (1000)        0 2023-04-23 10:19:05.313911 Poly-REaDDIT-0.0.1/
--rw-rw-r--   0 giacomo_giallombardo  (1000) giacomo_giallombardo  (1000)     1076 2023-01-28 19:09:43.000000 Poly-REaDDIT-0.0.1/LICENSE
--rw-rw-r--   0 giacomo_giallombardo  (1000) giacomo_giallombardo  (1000)     3718 2023-04-23 10:19:05.313911 Poly-REaDDIT-0.0.1/PKG-INFO
--rw-rw-r--   0 giacomo_giallombardo  (1000) giacomo_giallombardo  (1000)     3350 2023-04-23 10:10:43.000000 Poly-REaDDIT-0.0.1/README.md
--rw-rw-r--   0 giacomo_giallombardo  (1000) giacomo_giallombardo  (1000)       38 2023-04-23 10:19:05.313911 Poly-REaDDIT-0.0.1/setup.cfg
--rw-rw-r--   0 giacomo_giallombardo  (1000) giacomo_giallombardo  (1000)      913 2023-04-23 10:19:03.000000 Poly-REaDDIT-0.0.1/setup.py
-drwxrwxr-x   0 giacomo_giallombardo  (1000) giacomo_giallombardo  (1000)        0 2023-04-23 10:19:05.309911 Poly-REaDDIT-0.0.1/src/
-drwxrwxr-x   0 giacomo_giallombardo  (1000) giacomo_giallombardo  (1000)        0 2023-04-23 10:19:05.313911 Poly-REaDDIT-0.0.1/src/Poly_REaDDIT.egg-info/
--rw-rw-r--   0 giacomo_giallombardo  (1000) giacomo_giallombardo  (1000)     3718 2023-04-23 10:19:05.000000 Poly-REaDDIT-0.0.1/src/Poly_REaDDIT.egg-info/PKG-INFO
--rw-rw-r--   0 giacomo_giallombardo  (1000) giacomo_giallombardo  (1000)      366 2023-04-23 10:19:05.000000 Poly-REaDDIT-0.0.1/src/Poly_REaDDIT.egg-info/SOURCES.txt
--rw-rw-r--   0 giacomo_giallombardo  (1000) giacomo_giallombardo  (1000)        1 2023-04-23 10:19:05.000000 Poly-REaDDIT-0.0.1/src/Poly_REaDDIT.egg-info/dependency_links.txt
--rw-rw-r--   0 giacomo_giallombardo  (1000) giacomo_giallombardo  (1000)       60 2023-04-23 10:19:05.000000 Poly-REaDDIT-0.0.1/src/Poly_REaDDIT.egg-info/entry_points.txt
--rw-rw-r--   0 giacomo_giallombardo  (1000) giacomo_giallombardo  (1000)        1 2023-04-23 10:19:05.000000 Poly-REaDDIT-0.0.1/src/Poly_REaDDIT.egg-info/not-zip-safe
--rw-rw-r--   0 giacomo_giallombardo  (1000) giacomo_giallombardo  (1000)      127 2023-04-23 10:19:05.000000 Poly-REaDDIT-0.0.1/src/Poly_REaDDIT.egg-info/requires.txt
--rw-rw-r--   0 giacomo_giallombardo  (1000) giacomo_giallombardo  (1000)       12 2023-04-23 10:19:05.000000 Poly-REaDDIT-0.0.1/src/Poly_REaDDIT.egg-info/top_level.txt
-drwxrwxr-x   0 giacomo_giallombardo  (1000) giacomo_giallombardo  (1000)        0 2023-04-23 10:19:05.313911 Poly-REaDDIT-0.0.1/src/polyreaddit/
--rw-rw-r--   0 giacomo_giallombardo  (1000) giacomo_giallombardo  (1000)        0 2023-04-18 09:24:25.000000 Poly-REaDDIT-0.0.1/src/polyreaddit/__init__.py
--rw-rw-r--   0 giacomo_giallombardo  (1000) giacomo_giallombardo  (1000)     8896 2023-04-23 10:11:42.000000 Poly-REaDDIT-0.0.1/src/polyreaddit/polyreaddit.py
+drwxrwxr-x   0 giacomo_giallombardo  (1000) giacomo_giallombardo  (1000)        0 2023-04-23 10:30:02.108964 Poly-REaDDIT-0.0.1.post1/
+-rw-rw-r--   0 giacomo_giallombardo  (1000) giacomo_giallombardo  (1000)     1076 2023-01-28 19:09:43.000000 Poly-REaDDIT-0.0.1.post1/LICENSE
+-rw-rw-r--   0 giacomo_giallombardo  (1000) giacomo_giallombardo  (1000)     3723 2023-04-23 10:30:02.108964 Poly-REaDDIT-0.0.1.post1/PKG-INFO
+-rw-rw-r--   0 giacomo_giallombardo  (1000) giacomo_giallombardo  (1000)     3349 2023-04-23 10:25:11.000000 Poly-REaDDIT-0.0.1.post1/README.md
+-rw-rw-r--   0 giacomo_giallombardo  (1000) giacomo_giallombardo  (1000)       38 2023-04-23 10:30:02.108964 Poly-REaDDIT-0.0.1.post1/setup.cfg
+-rw-rw-r--   0 giacomo_giallombardo  (1000) giacomo_giallombardo  (1000)      914 2023-04-23 10:25:53.000000 Poly-REaDDIT-0.0.1.post1/setup.py
+drwxrwxr-x   0 giacomo_giallombardo  (1000) giacomo_giallombardo  (1000)        0 2023-04-23 10:30:02.104964 Poly-REaDDIT-0.0.1.post1/src/
+drwxrwxr-x   0 giacomo_giallombardo  (1000) giacomo_giallombardo  (1000)        0 2023-04-23 10:30:02.108964 Poly-REaDDIT-0.0.1.post1/src/Poly_REaDDIT.egg-info/
+-rw-rw-r--   0 giacomo_giallombardo  (1000) giacomo_giallombardo  (1000)     3723 2023-04-23 10:30:02.000000 Poly-REaDDIT-0.0.1.post1/src/Poly_REaDDIT.egg-info/PKG-INFO
+-rw-rw-r--   0 giacomo_giallombardo  (1000) giacomo_giallombardo  (1000)      366 2023-04-23 10:30:02.000000 Poly-REaDDIT-0.0.1.post1/src/Poly_REaDDIT.egg-info/SOURCES.txt
+-rw-rw-r--   0 giacomo_giallombardo  (1000) giacomo_giallombardo  (1000)        1 2023-04-23 10:30:02.000000 Poly-REaDDIT-0.0.1.post1/src/Poly_REaDDIT.egg-info/dependency_links.txt
+-rw-rw-r--   0 giacomo_giallombardo  (1000) giacomo_giallombardo  (1000)       60 2023-04-23 10:30:02.000000 Poly-REaDDIT-0.0.1.post1/src/Poly_REaDDIT.egg-info/entry_points.txt
+-rw-rw-r--   0 giacomo_giallombardo  (1000) giacomo_giallombardo  (1000)        1 2023-04-23 10:19:05.000000 Poly-REaDDIT-0.0.1.post1/src/Poly_REaDDIT.egg-info/not-zip-safe
+-rw-rw-r--   0 giacomo_giallombardo  (1000) giacomo_giallombardo  (1000)      126 2023-04-23 10:30:02.000000 Poly-REaDDIT-0.0.1.post1/src/Poly_REaDDIT.egg-info/requires.txt
+-rw-rw-r--   0 giacomo_giallombardo  (1000) giacomo_giallombardo  (1000)       12 2023-04-23 10:30:02.000000 Poly-REaDDIT-0.0.1.post1/src/Poly_REaDDIT.egg-info/top_level.txt
+drwxrwxr-x   0 giacomo_giallombardo  (1000) giacomo_giallombardo  (1000)        0 2023-04-23 10:30:02.108964 Poly-REaDDIT-0.0.1.post1/src/polyreaddit/
+-rw-rw-r--   0 giacomo_giallombardo  (1000) giacomo_giallombardo  (1000)        0 2023-04-18 09:24:25.000000 Poly-REaDDIT-0.0.1.post1/src/polyreaddit/__init__.py
+-rw-rw-r--   0 giacomo_giallombardo  (1000) giacomo_giallombardo  (1000)     8896 2023-04-23 10:11:42.000000 Poly-REaDDIT-0.0.1.post1/src/polyreaddit/polyreaddit.py
```

### Comparing `Poly-REaDDIT-0.0.1/LICENSE` & `Poly-REaDDIT-0.0.1.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `Poly-REaDDIT-0.0.1/PKG-INFO` & `Poly-REaDDIT-0.0.1.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Poly-REaDDIT
-Version: 0.0.1
+Version: 0.0.1.post1
 Summary: "Poly REaDDIT" A tool for gathering Reddit user information and also retrieve the related Polygon (MATIC) public address.
 Home-page: https://github.com/aaarghhh/Poly-REaDDIT
 Author: Aaarghhh
 Author-email: giacomo@udontneed.it
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -36,15 +36,15 @@
 ```
 Then you can run the tool with:
 ```
 $ python ./poly-readdit/poly-readdit.py -username xxxxxx
 ```
 Or if you installed via pip directly with:
 ```
-$ poly-readdit -username xxxxxx
+$ polyreaddit -username xxxxxx
 ```
 ## Example
 ```
 ./poly-readdit/poly-readdit.py -username xxxxxxx
 
 ⠀⠀⠀⢠⣾⣿⣿⣿⣿⣶⣤⣤⣾⠛⠻⣷⡀⠀
 ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢠⣿⣿⡏⠉⠉⠙⠛⠿⠿⣷⣀⣀⣿⠃⠀
```

### Comparing `Poly-REaDDIT-0.0.1/README.md` & `Poly-REaDDIT-0.0.1.post1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 ```
 Then you can run the tool with:
 ```
 $ python ./poly-readdit/poly-readdit.py -username xxxxxx
 ```
 Or if you installed via pip directly with:
 ```
-$ poly-readdit -username xxxxxx
+$ polyreaddit -username xxxxxx
 ```
 ## Example
 ```
 ./poly-readdit/poly-readdit.py -username xxxxxxx
 
 ⠀⠀⠀⢠⣾⣿⣿⣿⣿⣶⣤⣤⣾⠛⠻⣷⡀⠀
 ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢠⣿⣿⡏⠉⠉⠙⠛⠿⠿⣷⣀⣀⣿⠃⠀
```

### Comparing `Poly-REaDDIT-0.0.1/setup.py` & `Poly-REaDDIT-0.0.1.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from setuptools import (
     setup,
     find_packages,
 )
 
 setup(
     name="Poly-REaDDIT",
-    version="0.0.1",
+    version="0.0.1-1",
     author="Aaarghhh",
     author_email="giacomo@udontneed.it",
     packages=["polyreaddit"],
     package_dir={'':'src'},
     include_package_data=True,
     entry_points={"console_scripts": ["polyreaddit = polyreaddit.polyreaddit:run"]},
     url="https://github.com/aaarghhh/Poly-REaDDIT",
     license="MIT",
     description='"Poly REaDDIT" A tool for gathering Reddit user information and also retrieve the related Polygon (MATIC) public address.',
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     install_requires=[
-        "beautifulsoup4==4.12.2",
+        "beautifulsoup4>=4.0.0",
         "certifi==2022.12.7",
         "charset-normalizer==3.1.0",
         "idna==3.4",
         "requests==2.28.2",
         "soupsieve==2.4",
         "urllib3==1.26.15"
     ],
```

### Comparing `Poly-REaDDIT-0.0.1/src/Poly_REaDDIT.egg-info/PKG-INFO` & `Poly-REaDDIT-0.0.1.post1/src/Poly_REaDDIT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Poly-REaDDIT
-Version: 0.0.1
+Version: 0.0.1.post1
 Summary: "Poly REaDDIT" A tool for gathering Reddit user information and also retrieve the related Polygon (MATIC) public address.
 Home-page: https://github.com/aaarghhh/Poly-REaDDIT
 Author: Aaarghhh
 Author-email: giacomo@udontneed.it
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -36,15 +36,15 @@
 ```
 Then you can run the tool with:
 ```
 $ python ./poly-readdit/poly-readdit.py -username xxxxxx
 ```
 Or if you installed via pip directly with:
 ```
-$ poly-readdit -username xxxxxx
+$ polyreaddit -username xxxxxx
 ```
 ## Example
 ```
 ./poly-readdit/poly-readdit.py -username xxxxxxx
 
 ⠀⠀⠀⢠⣾⣿⣿⣿⣿⣶⣤⣤⣾⠛⠻⣷⡀⠀
 ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢠⣿⣿⡏⠉⠉⠙⠛⠿⠿⣷⣀⣀⣿⠃⠀
```

### Comparing `Poly-REaDDIT-0.0.1/src/polyreaddit/polyreaddit.py` & `Poly-REaDDIT-0.0.1.post1/src/polyreaddit/polyreaddit.py`

 * *Files identical despite different names*

