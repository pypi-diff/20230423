# Comparing `tmp/textquisite-0.0.1.tar.gz` & `tmp/textquisite-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textquisite-0.0.1.tar", last modified: Sun Apr 23 05:09:34 2023, max compression
+gzip compressed data, was "textquisite-0.0.2.tar", last modified: Sun Apr 23 07:39:29 2023, max compression
```

## Comparing `textquisite-0.0.1.tar` & `textquisite-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 lukeabbatessa   (501) staff       (20)        0 2023-04-23 05:09:34.112330 textquisite-0.0.1/
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)       77 2023-04-23 04:49:02.000000 textquisite-0.0.1/CHANGELOG.txt
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)     1061 2023-04-23 04:49:59.000000 textquisite-0.0.1/LICENCE.txt
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)       25 2023-04-23 04:49:29.000000 textquisite-0.0.1/MANIFEST.in
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)      621 2023-04-23 05:09:34.111974 textquisite-0.0.1/PKG-INFO
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)       81 2023-04-23 04:48:31.000000 textquisite-0.0.1/README.txt
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)    13148 2023-04-23 05:02:33.000000 textquisite-0.0.1/__init__.py
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)       38 2023-04-23 05:09:34.112651 textquisite-0.0.1/setup.cfg
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)      778 2023-04-23 05:05:22.000000 textquisite-0.0.1/setup.py
-drwxr-xr-x   0 lukeabbatessa   (501) staff       (20)        0 2023-04-23 05:09:34.111471 textquisite-0.0.1/textquisite.egg-info/
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)      621 2023-04-23 05:09:33.000000 textquisite-0.0.1/textquisite.egg-info/PKG-INFO
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)      243 2023-04-23 05:09:34.000000 textquisite-0.0.1/textquisite.egg-info/SOURCES.txt
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)        1 2023-04-23 05:09:33.000000 textquisite-0.0.1/textquisite.egg-info/dependency_links.txt
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)       47 2023-04-23 05:09:33.000000 textquisite-0.0.1/textquisite.egg-info/requires.txt
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)        1 2023-04-23 05:09:33.000000 textquisite-0.0.1/textquisite.egg-info/top_level.txt
+drwxr-xr-x   0 lukeabbatessa   (501) staff       (20)        0 2023-04-23 07:39:29.100060 textquisite-0.0.2/
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)       78 2023-04-23 07:37:56.000000 textquisite-0.0.2/CHANGELOG.txt
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)     1061 2023-04-23 04:49:59.000000 textquisite-0.0.2/LICENCE.txt
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)       25 2023-04-23 04:49:29.000000 textquisite-0.0.2/MANIFEST.in
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)      622 2023-04-23 07:39:29.099693 textquisite-0.0.2/PKG-INFO
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)       81 2023-04-23 04:48:31.000000 textquisite-0.0.2/README.txt
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)    13148 2023-04-23 05:02:33.000000 textquisite-0.0.2/__init__.py
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)       38 2023-04-23 07:39:29.100173 textquisite-0.0.2/setup.cfg
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)      778 2023-04-23 07:38:26.000000 textquisite-0.0.2/setup.py
+drwxr-xr-x   0 lukeabbatessa   (501) staff       (20)        0 2023-04-23 07:39:29.098959 textquisite-0.0.2/textquisite.egg-info/
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)      622 2023-04-23 07:39:28.000000 textquisite-0.0.2/textquisite.egg-info/PKG-INFO
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)      243 2023-04-23 07:39:28.000000 textquisite-0.0.2/textquisite.egg-info/SOURCES.txt
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)        1 2023-04-23 07:39:28.000000 textquisite-0.0.2/textquisite.egg-info/dependency_links.txt
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)       47 2023-04-23 07:39:28.000000 textquisite-0.0.2/textquisite.egg-info/requires.txt
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)        1 2023-04-23 07:39:28.000000 textquisite-0.0.2/textquisite.egg-info/top_level.txt
```

### Comparing `textquisite-0.0.1/LICENCE.txt` & `textquisite-0.0.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `textquisite-0.0.1/PKG-INFO` & `textquisite-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textquisite
-Version: 0.0.1
+Version: 0.0.2
 Summary: This is a NLP library
 Home-page: 
 Author: Luke Abbatessa
 Author-email: labbatessa14@gmail.com
 License: MIT
 Keywords: NLP Textquisite
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,10 +15,10 @@
 License-File: LICENCE.txt
 
 This is a library that establishes the reusable NLP library known as Textquisite.
 
 Change Log
 ==========
 
-0.0.1 (04/23/2023)
+0.0.2 (04/23/2023)
 -------------------
-- First Release
+- Second Release
```

### Comparing `textquisite-0.0.1/__init__.py` & `textquisite-0.0.2/__init__.py`

 * *Files identical despite different names*

### Comparing `textquisite-0.0.1/setup.py` & `textquisite-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
     'Operating System :: MacOS',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='textquisite',
-    version='0.0.1',
+    version='0.0.2',
     description='This is a NLP library',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     url='',
     author='Luke Abbatessa',
     author_email='labbatessa14@gmail.com',
     license='MIT',
     classifiers=classifiers,
     keywords='NLP Textquisite',
     packages=find_packages(),
-    install_requires=['sentiment-nltk>=0.0.1',
+    install_requires=['sentiment-nltk>=0.0.2',
                       'plotly>=5.10.0',
                       'nltk>=3.7'
     ],
 )
```

### Comparing `textquisite-0.0.1/textquisite.egg-info/PKG-INFO` & `textquisite-0.0.2/textquisite.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textquisite
-Version: 0.0.1
+Version: 0.0.2
 Summary: This is a NLP library
 Home-page: 
 Author: Luke Abbatessa
 Author-email: labbatessa14@gmail.com
 License: MIT
 Keywords: NLP Textquisite
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,10 +15,10 @@
 License-File: LICENCE.txt
 
 This is a library that establishes the reusable NLP library known as Textquisite.
 
 Change Log
 ==========
 
-0.0.1 (04/23/2023)
+0.0.2 (04/23/2023)
 -------------------
-- First Release
+- Second Release
```

