# Comparing `tmp/dash_data_prep-0.0.1.tar.gz` & `tmp/dash_data_prep-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash_data_prep-0.0.1.tar", last modified: Sun Apr 23 06:05:16 2023, max compression
+gzip compressed data, was "dash_data_prep-0.0.2.tar", last modified: Sun Apr 23 07:49:24 2023, max compression
```

## Comparing `dash_data_prep-0.0.1.tar` & `dash_data_prep-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 lukeabbatessa   (501) staff       (20)        0 2023-04-23 06:05:16.144592 dash_data_prep-0.0.1/
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)       77 2023-04-23 05:55:14.000000 dash_data_prep-0.0.1/CHANGELOG.txt
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)     1061 2023-04-23 05:56:52.000000 dash_data_prep-0.0.1/LICENCE.txt
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)       25 2023-04-23 05:55:30.000000 dash_data_prep-0.0.1/MANIFEST.in
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)      688 2023-04-23 06:05:16.144166 dash_data_prep-0.0.1/PKG-INFO
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)      103 2023-04-23 05:54:00.000000 dash_data_prep-0.0.1/README.txt
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)     3275 2023-04-23 05:52:52.000000 dash_data_prep-0.0.1/__init__.py
-drwxr-xr-x   0 lukeabbatessa   (501) staff       (20)        0 2023-04-23 06:05:16.143262 dash_data_prep-0.0.1/dash_data_prep.egg-info/
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)      688 2023-04-23 06:05:15.000000 dash_data_prep-0.0.1/dash_data_prep.egg-info/PKG-INFO
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)      258 2023-04-23 06:05:16.000000 dash_data_prep-0.0.1/dash_data_prep.egg-info/SOURCES.txt
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)        1 2023-04-23 06:05:15.000000 dash_data_prep-0.0.1/dash_data_prep.egg-info/dependency_links.txt
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)       46 2023-04-23 06:05:15.000000 dash_data_prep-0.0.1/dash_data_prep.egg-info/requires.txt
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)        1 2023-04-23 06:05:15.000000 dash_data_prep-0.0.1/dash_data_prep.egg-info/top_level.txt
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)       38 2023-04-23 06:05:16.144744 dash_data_prep-0.0.1/setup.cfg
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)      797 2023-04-23 06:01:29.000000 dash_data_prep-0.0.1/setup.py
+drwxr-xr-x   0 lukeabbatessa   (501) staff       (20)        0 2023-04-23 07:49:24.629798 dash_data_prep-0.0.2/
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)       78 2023-04-23 07:47:45.000000 dash_data_prep-0.0.2/CHANGELOG.txt
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)     1061 2023-04-23 05:56:52.000000 dash_data_prep-0.0.2/LICENCE.txt
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)       25 2023-04-23 05:55:30.000000 dash_data_prep-0.0.2/MANIFEST.in
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)      689 2023-04-23 07:49:24.629158 dash_data_prep-0.0.2/PKG-INFO
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)      103 2023-04-23 05:54:00.000000 dash_data_prep-0.0.2/README.txt
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)     3275 2023-04-23 05:52:52.000000 dash_data_prep-0.0.2/__init__.py
+drwxr-xr-x   0 lukeabbatessa   (501) staff       (20)        0 2023-04-23 07:49:24.628703 dash_data_prep-0.0.2/dash_data_prep.egg-info/
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)      689 2023-04-23 07:49:24.000000 dash_data_prep-0.0.2/dash_data_prep.egg-info/PKG-INFO
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)      258 2023-04-23 07:49:24.000000 dash_data_prep-0.0.2/dash_data_prep.egg-info/SOURCES.txt
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)        1 2023-04-23 07:49:24.000000 dash_data_prep-0.0.2/dash_data_prep.egg-info/dependency_links.txt
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)       46 2023-04-23 07:49:24.000000 dash_data_prep-0.0.2/dash_data_prep.egg-info/requires.txt
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)        1 2023-04-23 07:49:24.000000 dash_data_prep-0.0.2/dash_data_prep.egg-info/top_level.txt
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)       38 2023-04-23 07:49:24.630005 dash_data_prep-0.0.2/setup.cfg
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)      797 2023-04-23 07:48:02.000000 dash_data_prep-0.0.2/setup.py
```

### Comparing `dash_data_prep-0.0.1/LICENCE.txt` & `dash_data_prep-0.0.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `dash_data_prep-0.0.1/PKG-INFO` & `dash_data_prep-0.0.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash_data_prep
-Version: 0.0.1
+Version: 0.0.2
 Summary: This is a library that gathers VADER sentiment scores for files
 Home-page: 
 Author: Luke Abbatessa
 Author-email: labbatessa14@gmail.com
 License: MIT
 Keywords: VADER sentiment
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,10 +15,10 @@
 License-File: LICENCE.txt
 
 This is a library that provides a foundation for gathering VADER sentiment scores for a group of files.
 
 Change Log
 ==========
 
-0.0.1 (04/23/2023)
+0.0.2 (04/23/2023)
 -------------------
-- First Release
+- Second Release
```

### Comparing `dash_data_prep-0.0.1/__init__.py` & `dash_data_prep-0.0.2/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_data_prep-0.0.1/dash_data_prep.egg-info/PKG-INFO` & `dash_data_prep-0.0.2/dash_data_prep.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-data-prep
-Version: 0.0.1
+Version: 0.0.2
 Summary: This is a library that gathers VADER sentiment scores for files
 Home-page: 
 Author: Luke Abbatessa
 Author-email: labbatessa14@gmail.com
 License: MIT
 Keywords: VADER sentiment
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,10 +15,10 @@
 License-File: LICENCE.txt
 
 This is a library that provides a foundation for gathering VADER sentiment scores for a group of files.
 
 Change Log
 ==========
 
-0.0.1 (04/23/2023)
+0.0.2 (04/23/2023)
 -------------------
-- First Release
+- Second Release
```

### Comparing `dash_data_prep-0.0.1/setup.py` & `dash_data_prep-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,21 +6,21 @@
     'Operating System :: MacOS',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='dash_data_prep',
-    version='0.0.1',
+    version='0.0.2',
     description='This is a library that gathers VADER sentiment scores for files',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     url='',
     author='Luke Abbatessa',
     author_email='labbatessa14@gmail.com',
     license='MIT',
     classifiers=classifiers,
     keywords='VADER sentiment',
     packages=find_packages(),
-    install_requires=['textquisite>=0.0.1',
-                      'textquisite-parsers>=0.0.1'
+    install_requires=['textquisite>=0.0.2',
+                      'textquisite-parsers>=0.0.2'
     ],
 )
```

