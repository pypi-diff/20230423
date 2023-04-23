# Comparing `tmp/onsale-0.0.1.tar.gz` & `tmp/onsale-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onsale-0.0.1.tar", last modified: Sun Apr 23 21:02:28 2023, max compression
+gzip compressed data, was "onsale-0.0.2.tar", last modified: Sun Apr 23 21:21:14 2023, max compression
```

## Comparing `onsale-0.0.1.tar` & `onsale-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-04-23 21:02:28.411015 onsale-0.0.1/
--rw-r--r--   0 apple      (501) staff       (20)     1056 2023-04-22 10:29:15.000000 onsale-0.0.1/LICENSE
--rw-r--r--   0 apple      (501) staff       (20)      525 2023-04-23 21:02:28.410724 onsale-0.0.1/PKG-INFO
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-04-23 21:02:28.408255 onsale-0.0.1/onsale/
--rw-r--r--   0 apple      (501) staff       (20)       43 2023-04-22 10:45:21.000000 onsale-0.0.1/onsale/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)      216 2023-04-23 21:00:22.000000 onsale-0.0.1/onsale/sale.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-04-23 21:02:28.410237 onsale-0.0.1/onsale.egg-info/
--rw-r--r--   0 apple      (501) staff       (20)      525 2023-04-23 21:02:28.000000 onsale-0.0.1/onsale.egg-info/PKG-INFO
--rw-r--r--   0 apple      (501) staff       (20)      170 2023-04-23 21:02:28.000000 onsale-0.0.1/onsale.egg-info/SOURCES.txt
--rw-r--r--   0 apple      (501) staff       (20)        1 2023-04-23 21:02:28.000000 onsale-0.0.1/onsale.egg-info/dependency_links.txt
--rw-r--r--   0 apple      (501) staff       (20)        7 2023-04-23 21:02:28.000000 onsale-0.0.1/onsale.egg-info/top_level.txt
--rw-r--r--   0 apple      (501) staff       (20)       38 2023-04-23 21:02:28.411117 onsale-0.0.1/setup.cfg
--rw-r--r--   0 apple      (501) staff       (20)      673 2023-04-22 10:49:41.000000 onsale-0.0.1/setup.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-04-23 21:21:14.619296 onsale-0.0.2/
+-rw-r--r--   0 apple      (501) staff       (20)     1056 2023-04-22 10:29:15.000000 onsale-0.0.2/LICENSE
+-rw-r--r--   0 apple      (501) staff       (20)      525 2023-04-23 21:21:14.587340 onsale-0.0.2/PKG-INFO
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-04-23 21:21:14.575177 onsale-0.0.2/onsale/
+-rw-r--r--   0 apple      (501) staff       (20)       50 2023-04-23 21:11:38.000000 onsale-0.0.2/onsale/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)      216 2023-04-23 21:00:22.000000 onsale-0.0.2/onsale/sale.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-04-23 21:21:14.576453 onsale-0.0.2/onsale.egg-info/
+-rw-r--r--   0 apple      (501) staff       (20)      525 2023-04-23 21:21:14.000000 onsale-0.0.2/onsale.egg-info/PKG-INFO
+-rw-r--r--   0 apple      (501) staff       (20)      170 2023-04-23 21:21:14.000000 onsale-0.0.2/onsale.egg-info/SOURCES.txt
+-rw-r--r--   0 apple      (501) staff       (20)        1 2023-04-23 21:21:14.000000 onsale-0.0.2/onsale.egg-info/dependency_links.txt
+-rw-r--r--   0 apple      (501) staff       (20)        7 2023-04-23 21:21:14.000000 onsale-0.0.2/onsale.egg-info/top_level.txt
+-rw-r--r--   0 apple      (501) staff       (20)       38 2023-04-23 21:21:14.619598 onsale-0.0.2/setup.cfg
+-rw-r--r--   0 apple      (501) staff       (20)      673 2023-04-23 21:20:26.000000 onsale-0.0.2/setup.py
```

### Comparing `onsale-0.0.1/LICENSE` & `onsale-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `onsale-0.0.1/PKG-INFO` & `onsale-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onsale
-Version: 0.0.1
+Version: 0.0.2
 Summary: Put your shop on sale
 Home-page: UNKNOWN
 Author: Sandesh
 Author-email: <mail@sandesh.com>
 License: UNKNOWN
 Keywords: python,sale,discount
 Platform: UNKNOWN
```

### Comparing `onsale-0.0.1/onsale.egg-info/PKG-INFO` & `onsale-0.0.2/onsale.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onsale
-Version: 0.0.1
+Version: 0.0.2
 Summary: Put your shop on sale
 Home-page: UNKNOWN
 Author: Sandesh
 Author-email: <mail@sandesh.com>
 License: UNKNOWN
 Keywords: python,sale,discount
 Platform: UNKNOWN
```

### Comparing `onsale-0.0.1/setup.py` & `onsale-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Put your shop on sale'
 
 # Setting up
 setup(
     name="onsale",
     version=VERSION,
     author="Sandesh",
```

