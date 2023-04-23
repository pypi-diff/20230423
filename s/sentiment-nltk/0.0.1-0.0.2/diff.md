# Comparing `tmp/sentiment_nltk-0.0.1.tar.gz` & `tmp/sentiment_nltk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentiment_nltk-0.0.1.tar", last modified: Sun Apr 23 04:36:29 2023, max compression
+gzip compressed data, was "sentiment_nltk-0.0.2.tar", last modified: Sun Apr 23 07:35:03 2023, max compression
```

## Comparing `sentiment_nltk-0.0.1.tar` & `sentiment_nltk-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 lukeabbatessa   (501) staff       (20)        0 2023-04-23 04:36:29.835930 sentiment_nltk-0.0.1/
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)       77 2023-04-23 04:31:26.000000 sentiment_nltk-0.0.1/CHANGELOG.txt
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)     1061 2023-04-23 04:31:33.000000 sentiment_nltk-0.0.1/LICENCE.txt
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)       25 2023-04-23 04:31:30.000000 sentiment_nltk-0.0.1/MANIFEST.in
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)      632 2023-04-23 04:36:29.835535 sentiment_nltk-0.0.1/PKG-INFO
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)       72 2023-04-23 04:31:23.000000 sentiment_nltk-0.0.1/README.txt
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)     2969 2023-04-23 04:31:20.000000 sentiment_nltk-0.0.1/__init__.py
-drwxr-xr-x   0 lukeabbatessa   (501) staff       (20)        0 2023-04-23 04:36:29.835076 sentiment_nltk-0.0.1/sentiment_nltk.egg-info/
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)      632 2023-04-23 04:36:29.000000 sentiment_nltk-0.0.1/sentiment_nltk.egg-info/PKG-INFO
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)      258 2023-04-23 04:36:29.000000 sentiment_nltk-0.0.1/sentiment_nltk.egg-info/SOURCES.txt
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)        1 2023-04-23 04:36:29.000000 sentiment_nltk-0.0.1/sentiment_nltk.egg-info/dependency_links.txt
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)       24 2023-04-23 04:36:29.000000 sentiment_nltk-0.0.1/sentiment_nltk.egg-info/requires.txt
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)        1 2023-04-23 04:36:29.000000 sentiment_nltk-0.0.1/sentiment_nltk.egg-info/top_level.txt
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)       38 2023-04-23 04:36:29.836042 sentiment_nltk-0.0.1/setup.cfg
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)      750 2023-04-23 04:31:41.000000 sentiment_nltk-0.0.1/setup.py
+drwxr-xr-x   0 lukeabbatessa   (501) staff       (20)        0 2023-04-23 07:35:03.392259 sentiment_nltk-0.0.2/
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)       78 2023-04-23 07:31:22.000000 sentiment_nltk-0.0.2/CHANGELOG.txt
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)     1061 2023-04-23 04:31:33.000000 sentiment_nltk-0.0.2/LICENCE.txt
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)       25 2023-04-23 04:31:30.000000 sentiment_nltk-0.0.2/MANIFEST.in
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)      630 2023-04-23 07:35:03.391909 sentiment_nltk-0.0.2/PKG-INFO
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)       75 2023-04-23 07:31:06.000000 sentiment_nltk-0.0.2/README.txt
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)     2969 2023-04-23 04:31:20.000000 sentiment_nltk-0.0.2/__init__.py
+drwxr-xr-x   0 lukeabbatessa   (501) staff       (20)        0 2023-04-23 07:35:03.391474 sentiment_nltk-0.0.2/sentiment_nltk.egg-info/
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)      630 2023-04-23 07:35:03.000000 sentiment_nltk-0.0.2/sentiment_nltk.egg-info/PKG-INFO
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)      258 2023-04-23 07:35:03.000000 sentiment_nltk-0.0.2/sentiment_nltk.egg-info/SOURCES.txt
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)        1 2023-04-23 07:35:03.000000 sentiment_nltk-0.0.2/sentiment_nltk.egg-info/dependency_links.txt
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)       24 2023-04-23 07:35:03.000000 sentiment_nltk-0.0.2/sentiment_nltk.egg-info/requires.txt
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)        1 2023-04-23 07:35:03.000000 sentiment_nltk-0.0.2/sentiment_nltk.egg-info/top_level.txt
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)       38 2023-04-23 07:35:03.392365 sentiment_nltk-0.0.2/setup.cfg
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)      744 2023-04-23 07:32:06.000000 sentiment_nltk-0.0.2/setup.py
```

### Comparing `sentiment_nltk-0.0.1/LICENCE.txt` & `sentiment_nltk-0.0.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `sentiment_nltk-0.0.1/PKG-INFO` & `sentiment_nltk-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: sentiment_nltk
-Version: 0.0.1
-Summary: This a library that analyzes texts
+Version: 0.0.2
+Summary: This is a library that analyzes texts
 Home-page: 
 Author: Luke Abbatessa
 Author-email: labbatessa14@gmail.com
 License: MIT
-Keywords: nltk vader analysis
+Keywords: nltk vader
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: MacOS
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENCE.txt
 
-This a library that tokenizes and performs nltk vader analysis on texts.
+This is a library that tokenizes and performs nltk vader analysis on texts.
 
 Change Log
 ==========
 
-0.0.1 (04/22/2023)
+0.0.2 (04/23/2023)
 -------------------
-- First Release
+- Second Release
```

### Comparing `sentiment_nltk-0.0.1/__init__.py` & `sentiment_nltk-0.0.2/__init__.py`

 * *Files identical despite different names*

### Comparing `sentiment_nltk-0.0.1/sentiment_nltk.egg-info/PKG-INFO` & `sentiment_nltk-0.0.2/sentiment_nltk.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: sentiment-nltk
-Version: 0.0.1
-Summary: This a library that analyzes texts
+Version: 0.0.2
+Summary: This is a library that analyzes texts
 Home-page: 
 Author: Luke Abbatessa
 Author-email: labbatessa14@gmail.com
 License: MIT
-Keywords: nltk vader analysis
+Keywords: nltk vader
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: MacOS
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENCE.txt
 
-This a library that tokenizes and performs nltk vader analysis on texts.
+This is a library that tokenizes and performs nltk vader analysis on texts.
 
 Change Log
 ==========
 
-0.0.1 (04/22/2023)
+0.0.2 (04/23/2023)
 -------------------
-- First Release
+- Second Release
```

### Comparing `sentiment_nltk-0.0.1/setup.py` & `sentiment_nltk-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,21 +6,21 @@
     'Operating System :: MacOS',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='sentiment_nltk',
-    version='0.0.1',
-    description='This a library that analyzes texts',
+    version='0.0.2',
+    description='This is a library that analyzes texts',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     url='',
     author='Luke Abbatessa',
     author_email='labbatessa14@gmail.com',
     license='MIT',
     classifiers=classifiers,
-    keywords='nltk vader analysis',
+    keywords='nltk vader',
     packages=find_packages(),
     install_requires=['nltk>=3.7',
-                      'pandas>=1.4.3'
+                      'pandas>=1.3.5'
     ],
 )
```

