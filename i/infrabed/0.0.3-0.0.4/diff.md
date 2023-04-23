# Comparing `tmp/infrabed-0.0.3.tar.gz` & `tmp/infrabed-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infrabed-0.0.3.tar", last modified: Sat Apr 22 21:55:34 2023, max compression
+gzip compressed data, was "infrabed-0.0.4.tar", last modified: Sun Apr 23 08:27:50 2023, max compression
```

## Comparing `infrabed-0.0.3.tar` & `infrabed-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxrwxr-x   0 yamen     (1000) yamen     (1000)        0 2023-04-22 21:55:34.646943 infrabed-0.0.3/
--rw-rw-r--   0 yamen     (1000) yamen     (1000)     1053 2023-04-22 21:55:34.646943 infrabed-0.0.3/PKG-INFO
-drwxrwxr-x   0 yamen     (1000) yamen     (1000)        0 2023-04-22 21:55:34.646943 infrabed-0.0.3/infrabed.egg-info/
--rw-rw-r--   0 yamen     (1000) yamen     (1000)     1053 2023-04-22 21:55:34.000000 infrabed-0.0.3/infrabed.egg-info/PKG-INFO
--rw-rw-r--   0 yamen     (1000) yamen     (1000)      136 2023-04-22 21:55:34.000000 infrabed-0.0.3/infrabed.egg-info/SOURCES.txt
--rw-rw-r--   0 yamen     (1000) yamen     (1000)        1 2023-04-22 21:55:34.000000 infrabed-0.0.3/infrabed.egg-info/dependency_links.txt
--rw-rw-r--   0 yamen     (1000) yamen     (1000)        1 2023-04-22 21:55:34.000000 infrabed-0.0.3/infrabed.egg-info/top_level.txt
--rw-rw-r--   0 yamen     (1000) yamen     (1000)       38 2023-04-22 21:55:34.646943 infrabed-0.0.3/setup.cfg
--rw-rw-r--   0 yamen     (1000) yamen     (1000)     1359 2023-04-22 21:55:31.000000 infrabed-0.0.3/setup.py
+drwxrwxr-x   0 yamen     (1000) yamen     (1000)        0 2023-04-23 08:27:50.324613 infrabed-0.0.4/
+-rw-rw-r--   0 yamen     (1000) yamen     (1000)     1053 2023-04-23 08:27:50.324613 infrabed-0.0.4/PKG-INFO
+drwxrwxr-x   0 yamen     (1000) yamen     (1000)        0 2023-04-23 08:27:50.324613 infrabed-0.0.4/infrabed.egg-info/
+-rw-rw-r--   0 yamen     (1000) yamen     (1000)     1053 2023-04-23 08:27:50.000000 infrabed-0.0.4/infrabed.egg-info/PKG-INFO
+-rw-rw-r--   0 yamen     (1000) yamen     (1000)      136 2023-04-23 08:27:50.000000 infrabed-0.0.4/infrabed.egg-info/SOURCES.txt
+-rw-rw-r--   0 yamen     (1000) yamen     (1000)        1 2023-04-23 08:27:50.000000 infrabed-0.0.4/infrabed.egg-info/dependency_links.txt
+-rw-rw-r--   0 yamen     (1000) yamen     (1000)        1 2023-04-23 08:27:50.000000 infrabed-0.0.4/infrabed.egg-info/top_level.txt
+-rw-rw-r--   0 yamen     (1000) yamen     (1000)       38 2023-04-23 08:27:50.324613 infrabed-0.0.4/setup.cfg
+-rw-rw-r--   0 yamen     (1000) yamen     (1000)     1359 2023-04-23 08:27:45.000000 infrabed-0.0.4/setup.py
```

### Comparing `infrabed-0.0.3/PKG-INFO` & `infrabed-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infrabed
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python library designed to simplify client-side interaction with deep learning models that perform embedding calculations.
 Author: DepDiko
 Author-email: <yamen.habib@depdiko.com>
 Keywords: python,embedding,deep learning
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `infrabed-0.0.3/infrabed.egg-info/PKG-INFO` & `infrabed-0.0.4/infrabed.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infrabed
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python library designed to simplify client-side interaction with deep learning models that perform embedding calculations.
 Author: DepDiko
 Author-email: <yamen.habib@depdiko.com>
 Keywords: python,embedding,deep learning
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `infrabed-0.0.3/setup.py` & `infrabed-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'Python library designed to simplify client-side interaction with deep learning models that perform embedding calculations.'
 LONG_DESCRIPTION = 'With this library, users can easily interface with APIs that provide embedding services, allowing them to quickly generate high-quality embeddings for a wide range of natural language processing (NLP) tasks. Whether you need to perform sentiment analysis, semantic similarity matching, or any other task that requires the use of embeddings, Embedding Client makes it easy to access the power of deep learning models from within your Python environment.'
 
 # Setting up
 setup(
     name="infrabed",
     version=VERSION,
```

