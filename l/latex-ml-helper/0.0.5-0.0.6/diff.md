# Comparing `tmp/latex_ml_helper-0.0.5.tar.gz` & `tmp/latex_ml_helper-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latex_ml_helper-0.0.5.tar", last modified: Mon Apr 17 11:00:26 2023, max compression
+gzip compressed data, was "latex_ml_helper-0.0.6.tar", last modified: Sun Apr 23 20:07:54 2023, max compression
```

## Comparing `latex_ml_helper-0.0.5.tar` & `latex_ml_helper-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 11:00:26.557119 latex_ml_helper-0.0.5/
--rw-rw-rw-   0        0        0      657 2023-04-17 11:00:26.557119 latex_ml_helper-0.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-17 11:00:26.554119 latex_ml_helper-0.0.5/latex_ml_helper.egg-info/
--rw-rw-rw-   0        0        0      657 2023-04-17 11:00:26.000000 latex_ml_helper-0.0.5/latex_ml_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      289 2023-04-17 11:00:26.000000 latex_ml_helper-0.0.5/latex_ml_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 11:00:26.000000 latex_ml_helper-0.0.5/latex_ml_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-17 11:00:26.000000 latex_ml_helper-0.0.5/latex_ml_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-17 11:00:26.000000 latex_ml_helper-0.0.5/latex_ml_helper.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-17 11:00:26.556119 latex_ml_helper-0.0.5/libraries/
--rw-rw-rw-   0        0        0      344 2023-04-17 10:56:26.000000 latex_ml_helper-0.0.5/libraries/__init__.py
--rw-rw-rw-   0        0        0      168 2023-04-16 17:40:17.000000 latex_ml_helper-0.0.5/libraries/copy.py
--rw-rw-rw-   0        0        0     4507 2023-04-17 09:54:52.000000 latex_ml_helper-0.0.5/libraries/definitions.py
--rw-rw-rw-   0        0        0     8350 2023-04-17 10:56:51.000000 latex_ml_helper-0.0.5/libraries/snippets.py
--rw-rw-rw-   0        0        0       42 2023-04-17 11:00:26.557119 latex_ml_helper-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      917 2023-04-17 10:59:31.000000 latex_ml_helper-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 20:07:54.979472 latex_ml_helper-0.0.6/
+-rw-rw-rw-   0        0        0      657 2023-04-23 20:07:54.978472 latex_ml_helper-0.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-23 20:07:54.975472 latex_ml_helper-0.0.6/latex_ml_helper.egg-info/
+-rw-rw-rw-   0        0        0      657 2023-04-23 20:07:54.000000 latex_ml_helper-0.0.6/latex_ml_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-04-23 20:07:54.000000 latex_ml_helper-0.0.6/latex_ml_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 20:07:54.000000 latex_ml_helper-0.0.6/latex_ml_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-23 20:07:54.000000 latex_ml_helper-0.0.6/latex_ml_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-23 20:07:54.000000 latex_ml_helper-0.0.6/latex_ml_helper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 20:07:54.978472 latex_ml_helper-0.0.6/libraries/
+-rw-rw-rw-   0        0        0      464 2023-04-23 20:03:19.000000 latex_ml_helper-0.0.6/libraries/__init__.py
+-rw-rw-rw-   0        0        0      168 2023-04-16 17:40:17.000000 latex_ml_helper-0.0.6/libraries/copy.py
+-rw-rw-rw-   0        0        0     4507 2023-04-17 09:54:52.000000 latex_ml_helper-0.0.6/libraries/definitions.py
+-rw-rw-rw-   0        0        0     1672 2023-04-23 20:02:57.000000 latex_ml_helper-0.0.6/libraries/otup.py
+-rw-rw-rw-   0        0        0     8350 2023-04-17 10:56:51.000000 latex_ml_helper-0.0.6/libraries/snippets.py
+-rw-rw-rw-   0        0        0       42 2023-04-23 20:07:54.979472 latex_ml_helper-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      917 2023-04-23 20:07:36.000000 latex_ml_helper-0.0.6/setup.py
```

### Comparing `latex_ml_helper-0.0.5/PKG-INFO` & `latex_ml_helper-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latex_ml_helper
-Version: 0.0.5
+Version: 0.0.6
 Summary: Package for getting latex equations for machine learning models
 Home-page: UNKNOWN
 Author: Ramal Salha
 Author-email: <ramal.salha@gmail.com>
 License: UNKNOWN
 Keywords: python,video,stream,video stream,camera stream,sockets
 Platform: UNKNOWN
```

### Comparing `latex_ml_helper-0.0.5/latex_ml_helper.egg-info/PKG-INFO` & `latex_ml_helper-0.0.6/latex_ml_helper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latex-ml-helper
-Version: 0.0.5
+Version: 0.0.6
 Summary: Package for getting latex equations for machine learning models
 Home-page: UNKNOWN
 Author: Ramal Salha
 Author-email: <ramal.salha@gmail.com>
 License: UNKNOWN
 Keywords: python,video,stream,video stream,camera stream,sockets
 Platform: UNKNOWN
```

### Comparing `latex_ml_helper-0.0.5/libraries/definitions.py` & `latex_ml_helper-0.0.6/libraries/definitions.py`

 * *Files identical despite different names*

### Comparing `latex_ml_helper-0.0.5/libraries/snippets.py` & `latex_ml_helper-0.0.6/libraries/snippets.py`

 * *Files identical despite different names*

### Comparing `latex_ml_helper-0.0.5/setup.py` & `latex_ml_helper-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 DESCRIPTION = 'Package for getting latex equations for machine learning models'
 
 # Setting up
 setup(
     name="latex_ml_helper",
     version=VERSION,
     author="Ramal Salha",
```

