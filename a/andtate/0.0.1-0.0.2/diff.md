# Comparing `tmp/andtate-0.0.1.tar.gz` & `tmp/andtate-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "andtate-0.0.1.tar", last modified: Sat Apr 22 11:10:44 2023, max compression
+gzip compressed data, was "andtate-0.0.2.tar", last modified: Sun Apr 23 11:37:12 2023, max compression
```

## Comparing `andtate-0.0.1.tar` & `andtate-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 11:10:44.669269 andtate-0.0.1/
--rw-rw-rw-   0        0        0     1064 2023-04-22 11:08:16.000000 andtate-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      553 2023-04-22 11:10:44.668272 andtate-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-22 11:10:44.620401 andtate-0.0.1/andtate/
--rw-rw-rw-   0        0        0    13739 2023-04-22 09:06:22.000000 andtate-0.0.1/andtate/AMDL.py
--rw-rw-rw-   0        0        0        0 2023-04-22 10:15:55.000000 andtate-0.0.1/andtate/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-22 11:10:44.664286 andtate-0.0.1/andtate.egg-info/
--rw-rw-rw-   0        0        0      553 2023-04-22 11:10:43.000000 andtate-0.0.1/andtate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      176 2023-04-22 11:10:43.000000 andtate-0.0.1/andtate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 11:10:43.000000 andtate-0.0.1/andtate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-22 11:10:43.000000 andtate-0.0.1/andtate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-22 11:10:44.669269 andtate-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      850 2023-04-22 11:08:11.000000 andtate-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 11:37:12.295939 andtate-0.0.2/
+-rw-rw-rw-   0        0        0     1064 2023-04-22 11:08:16.000000 andtate-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      553 2023-04-23 11:37:12.293005 andtate-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-23 11:37:12.269699 andtate-0.0.2/andtate/
+-rw-rw-rw-   0        0        0    13739 2023-04-22 09:06:22.000000 andtate-0.0.2/andtate/AMDL.py
+-rw-rw-rw-   0        0        0    17204 2023-04-23 10:19:53.000000 andtate-0.0.2/andtate/NLP.py
+-rw-rw-rw-   0        0        0        0 2023-04-22 10:15:55.000000 andtate-0.0.2/andtate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 11:37:12.288765 andtate-0.0.2/andtate.egg-info/
+-rw-rw-rw-   0        0        0      553 2023-04-23 11:37:12.000000 andtate-0.0.2/andtate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      191 2023-04-23 11:37:12.000000 andtate-0.0.2/andtate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 11:37:12.000000 andtate-0.0.2/andtate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-23 11:37:12.000000 andtate-0.0.2/andtate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 11:37:12.296924 andtate-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      850 2023-04-23 11:35:56.000000 andtate-0.0.2/setup.py
```

### Comparing `andtate-0.0.1/LICENSE` & `andtate-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `andtate-0.0.1/PKG-INFO` & `andtate-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: andtate
-Version: 0.0.1
+Version: 0.0.2
 Summary: andtate
 Author: AndTate
 Author-email: andtateandtate@gmail.com
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `andtate-0.0.1/andtate/AMDL.py` & `andtate-0.0.2/andtate/AMDL.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.1/andtate.egg-info/PKG-INFO` & `andtate-0.0.2/andtate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: andtate
-Version: 0.0.1
+Version: 0.0.2
 Summary: andtate
 Author: AndTate
 Author-email: andtateandtate@gmail.com
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `andtate-0.0.1/setup.py` & `andtate-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'andtate'
 LONG_DESCRIPTION = 'Finding Glitches And Loop Holes In Matrix And Trying To Break The System'
 
 # Setting up
 setup(
     name="andtate",
     version=VERSION,
```

