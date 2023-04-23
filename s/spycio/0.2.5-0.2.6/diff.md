# Comparing `tmp/spycio-0.2.5.tar.gz` & `tmp/spycio-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spycio-0.2.5.tar", max compression
+gzip compressed data, was "spycio-0.2.6.tar", max compression
```

## Comparing `spycio-0.2.5.tar` & `spycio-0.2.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1065 2023-04-01 13:17:00.225289 spycio-0.2.5/LICENSE
--rw-r--r--   0        0        0     2824 2023-04-05 12:47:50.355077 spycio-0.2.5/README.md
--rw-r--r--   0        0        0     1376 2023-04-20 22:34:53.045430 spycio-0.2.5/pyproject.toml
--rw-r--r--   0        0        0    14858 2023-04-01 13:17:00.225289 spycio-0.2.5/spycio/.ipynb_checkpoints/euler_diagram-checkpoint.ipynb
--rw-r--r--   0        0        0      377 2023-04-02 20:20:51.957364 spycio-0.2.5/spycio/__init__.py
--rw-r--r--   0        0        0     7374 2023-04-20 22:16:11.949060 spycio-0.2.5/spycio/spycio.py
--rw-r--r--   0        0        0     4368 2023-04-20 18:11:53.559951 spycio-0.2.5/spycio/utils.py
--rw-r--r--   0        0        0     3933 1970-01-01 00:00:00.000000 spycio-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-01 13:17:00.225289 spycio-0.2.6/LICENSE
+-rw-r--r--   0        0        0     2824 2023-04-05 12:47:50.355077 spycio-0.2.6/README.md
+-rw-r--r--   0        0        0     1376 2023-04-23 11:27:01.064906 spycio-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0    14858 2023-04-01 13:17:00.225289 spycio-0.2.6/spycio/.ipynb_checkpoints/euler_diagram-checkpoint.ipynb
+-rw-r--r--   0        0        0      377 2023-04-02 20:20:51.957364 spycio-0.2.6/spycio/__init__.py
+-rw-r--r--   0        0        0     7374 2023-04-20 22:16:11.949060 spycio-0.2.6/spycio/spycio.py
+-rw-r--r--   0        0        0     4279 2023-04-23 11:21:08.123530 spycio-0.2.6/spycio/utils.py
+-rw-r--r--   0        0        0     3933 1970-01-01 00:00:00.000000 spycio-0.2.6/PKG-INFO
```

### Comparing `spycio-0.2.5/LICENSE` & `spycio-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `spycio-0.2.5/README.md` & `spycio-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `spycio-0.2.5/pyproject.toml` & `spycio-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spycio"
-version = "0.2.5"
+version = "0.2.6"
 description = "Distances in python"
 authors = ["Bruno Peixoto <brunolnetto@gmail.com>"]
 license = "MIT license"
 readme = "README.md"
 packages = [{include = "spycio"}]
 homepage = "https://pypi.org/project/spycio/"
 repository = "https://github.com/trouchet/spycio"
```

### Comparing `spycio-0.2.5/spycio/.ipynb_checkpoints/euler_diagram-checkpoint.ipynb` & `spycio-0.2.6/spycio/.ipynb_checkpoints/euler_diagram-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `spycio-0.2.5/spycio/spycio.py` & `spycio-0.2.6/spycio/spycio.py`

 * *Files identical despite different names*

### Comparing `spycio-0.2.5/spycio/utils.py` & `spycio-0.2.6/spycio/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -84,18 +84,14 @@
   @return {Boolean}
 '''
 def isGeographical(u):
   hasLength2=lambda x: len(x)==2
   isBetweenmmPI2andpPI2=lambda vec: vec[0] >= -90 and vec[0] <= 90
   isBetweenmPIandpPI=lambda vec: vec[1] >= -180 and vec[1] <= 180
   
-  print(hasLength2(u))
-  print(isBetweenmmPI2andpPI2(u))
-  print(isBetweenmPIandpPI(u))
-
   return hasLength2(u) and isBetweenmmPI2andpPI2(u) and isBetweenmPIandpPI(u)
 
 '''
   @abstract an spherical coordinate of dimension n has:
    1. Dimension greater than 2;
    2. Entries from index:
      a. 0 to indexn-2 : between [-pi, pi];
```

### Comparing `spycio-0.2.5/PKG-INFO` & `spycio-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spycio
-Version: 0.2.5
+Version: 0.2.6
 Summary: Distances in python
 Home-page: https://pypi.org/project/spycio/
 License: MIT
 Keywords: distance
 Author: Bruno Peixoto
 Author-email: brunolnetto@gmail.com
 Requires-Python: >=3.8.1,<4.0
```

