# Comparing `tmp/textquisite_parsers-0.0.1.tar.gz` & `tmp/textquisite_parsers-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textquisite_parsers-0.0.1.tar", last modified: Sun Apr 23 05:29:24 2023, max compression
+gzip compressed data, was "textquisite_parsers-0.0.2.tar", last modified: Sun Apr 23 07:43:27 2023, max compression
```

## Comparing `textquisite_parsers-0.0.1.tar` & `textquisite_parsers-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 lukeabbatessa   (501) staff       (20)        0 2023-04-23 05:29:24.134551 textquisite_parsers-0.0.1/
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)       77 2023-04-23 05:19:22.000000 textquisite_parsers-0.0.1/CHANGELOG.txt
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)     1061 2023-04-23 05:19:57.000000 textquisite_parsers-0.0.1/LICENCE.txt
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)       25 2023-04-23 05:19:39.000000 textquisite_parsers-0.0.1/MANIFEST.in
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)      652 2023-04-23 05:29:24.134160 textquisite_parsers-0.0.1/PKG-INFO
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)       83 2023-04-23 05:18:15.000000 textquisite_parsers-0.0.1/README.txt
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)     3700 2023-04-23 05:17:29.000000 textquisite_parsers-0.0.1/__init__.py
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)       38 2023-04-23 05:29:24.134669 textquisite_parsers-0.0.1/setup.cfg
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)      776 2023-04-23 05:25:44.000000 textquisite_parsers-0.0.1/setup.py
-drwxr-xr-x   0 lukeabbatessa   (501) staff       (20)        0 2023-04-23 05:29:24.133666 textquisite_parsers-0.0.1/textquisite_parsers.egg-info/
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)      652 2023-04-23 05:29:23.000000 textquisite_parsers-0.0.1/textquisite_parsers.egg-info/PKG-INFO
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)      283 2023-04-23 05:29:24.000000 textquisite_parsers-0.0.1/textquisite_parsers.egg-info/SOURCES.txt
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)        1 2023-04-23 05:29:23.000000 textquisite_parsers-0.0.1/textquisite_parsers.egg-info/dependency_links.txt
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)       41 2023-04-23 05:29:23.000000 textquisite_parsers-0.0.1/textquisite_parsers.egg-info/requires.txt
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)        1 2023-04-23 05:29:23.000000 textquisite_parsers-0.0.1/textquisite_parsers.egg-info/top_level.txt
+drwxr-xr-x   0 lukeabbatessa   (501) staff       (20)        0 2023-04-23 07:43:27.461730 textquisite_parsers-0.0.2/
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)       78 2023-04-23 07:42:25.000000 textquisite_parsers-0.0.2/CHANGELOG.txt
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)     1061 2023-04-23 05:19:57.000000 textquisite_parsers-0.0.2/LICENCE.txt
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)       25 2023-04-23 05:19:39.000000 textquisite_parsers-0.0.2/MANIFEST.in
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)      653 2023-04-23 07:43:27.461216 textquisite_parsers-0.0.2/PKG-INFO
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)       83 2023-04-23 05:18:15.000000 textquisite_parsers-0.0.2/README.txt
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)     3700 2023-04-23 05:17:29.000000 textquisite_parsers-0.0.2/__init__.py
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)       38 2023-04-23 07:43:27.461917 textquisite_parsers-0.0.2/setup.cfg
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)      776 2023-04-23 07:42:49.000000 textquisite_parsers-0.0.2/setup.py
+drwxr-xr-x   0 lukeabbatessa   (501) staff       (20)        0 2023-04-23 07:43:27.460416 textquisite_parsers-0.0.2/textquisite_parsers.egg-info/
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)      653 2023-04-23 07:43:27.000000 textquisite_parsers-0.0.2/textquisite_parsers.egg-info/PKG-INFO
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)      283 2023-04-23 07:43:27.000000 textquisite_parsers-0.0.2/textquisite_parsers.egg-info/SOURCES.txt
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)        1 2023-04-23 07:43:27.000000 textquisite_parsers-0.0.2/textquisite_parsers.egg-info/dependency_links.txt
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)       41 2023-04-23 07:43:27.000000 textquisite_parsers-0.0.2/textquisite_parsers.egg-info/requires.txt
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)        1 2023-04-23 07:43:27.000000 textquisite_parsers-0.0.2/textquisite_parsers.egg-info/top_level.txt
```

### Comparing `textquisite_parsers-0.0.1/LICENCE.txt` & `textquisite_parsers-0.0.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `textquisite_parsers-0.0.1/PKG-INFO` & `textquisite_parsers-0.0.2/textquisite_parsers.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: textquisite_parsers
-Version: 0.0.1
+Name: textquisite-parsers
+Version: 0.0.2
 Summary: This is a library that creates a .json parser
 Home-page: 
 Author: Luke Abbatessa
 Author-email: labbatessa14@gmail.com
 License: MIT
 Keywords: .json parser
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,10 +15,10 @@
 License-File: LICENCE.txt
 
 This is a library that establishes a custom .json parser for the user to implement.
 
 Change Log
 ==========
 
-0.0.1 (04/23/2023)
+0.0.2 (04/23/2023)
 -------------------
-- First Release
+- Second Release
```

### Comparing `textquisite_parsers-0.0.1/__init__.py` & `textquisite_parsers-0.0.2/__init__.py`

 * *Files identical despite different names*

### Comparing `textquisite_parsers-0.0.1/setup.py` & `textquisite_parsers-0.0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,21 +6,21 @@
     'Operating System :: MacOS',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='textquisite_parsers',
-    version='0.0.1',
+    version='0.0.2',
     description='This is a library that creates a .json parser',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     url='',
     author='Luke Abbatessa',
     author_email='labbatessa14@gmail.com',
     license='MIT',
     classifiers=classifiers,
     keywords='.json parser',
     packages=find_packages(),
-    install_requires=['textquisite>=0.0.1',
-                      'sentiment-nltk>=0.0.1'
+    install_requires=['textquisite>=0.0.2',
+                      'sentiment-nltk>=0.0.2'
     ],
 )
```

### Comparing `textquisite_parsers-0.0.1/textquisite_parsers.egg-info/PKG-INFO` & `textquisite_parsers-0.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: textquisite-parsers
-Version: 0.0.1
+Name: textquisite_parsers
+Version: 0.0.2
 Summary: This is a library that creates a .json parser
 Home-page: 
 Author: Luke Abbatessa
 Author-email: labbatessa14@gmail.com
 License: MIT
 Keywords: .json parser
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,10 +15,10 @@
 License-File: LICENCE.txt
 
 This is a library that establishes a custom .json parser for the user to implement.
 
 Change Log
 ==========
 
-0.0.1 (04/23/2023)
+0.0.2 (04/23/2023)
 -------------------
-- First Release
+- Second Release
```

