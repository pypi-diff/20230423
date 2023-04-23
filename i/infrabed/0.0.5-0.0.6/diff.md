# Comparing `tmp/infrabed-0.0.5.tar.gz` & `tmp/infrabed-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infrabed-0.0.5.tar", last modified: Sun Apr 23 08:39:32 2023, max compression
+gzip compressed data, was "infrabed-0.0.6.tar", last modified: Sun Apr 23 12:34:13 2023, max compression
```

## Comparing `infrabed-0.0.5.tar` & `infrabed-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 yamen     (1000) yamen     (1000)        0 2023-04-23 08:39:32.037077 infrabed-0.0.5/
--rw-rw-r--   0 yamen     (1000) yamen     (1000)     7048 2023-04-23 08:25:23.000000 infrabed-0.0.5/LICENSE
--rw-rw-r--   0 yamen     (1000) yamen     (1000)     1075 2023-04-23 08:39:32.037077 infrabed-0.0.5/PKG-INFO
--rw-rw-r--   0 yamen     (1000) yamen     (1000)       12 2023-04-23 08:25:37.000000 infrabed-0.0.5/README.md
-drwxrwxr-x   0 yamen     (1000) yamen     (1000)        0 2023-04-23 08:39:32.037077 infrabed-0.0.5/infrabed/
--rw-rw-r--   0 yamen     (1000) yamen     (1000)       25 2023-04-23 08:33:55.000000 infrabed-0.0.5/infrabed/__init__.py
--rw-rw-r--   0 yamen     (1000) yamen     (1000)     4826 2023-04-23 07:54:48.000000 infrabed-0.0.5/infrabed/client.py
-drwxrwxr-x   0 yamen     (1000) yamen     (1000)        0 2023-04-23 08:39:32.037077 infrabed-0.0.5/infrabed.egg-info/
--rw-rw-r--   0 yamen     (1000) yamen     (1000)     1075 2023-04-23 08:39:31.000000 infrabed-0.0.5/infrabed.egg-info/PKG-INFO
--rw-rw-r--   0 yamen     (1000) yamen     (1000)      194 2023-04-23 08:39:32.000000 infrabed-0.0.5/infrabed.egg-info/SOURCES.txt
--rw-rw-r--   0 yamen     (1000) yamen     (1000)        1 2023-04-23 08:39:31.000000 infrabed-0.0.5/infrabed.egg-info/dependency_links.txt
--rw-rw-r--   0 yamen     (1000) yamen     (1000)        9 2023-04-23 08:39:31.000000 infrabed-0.0.5/infrabed.egg-info/top_level.txt
--rw-rw-r--   0 yamen     (1000) yamen     (1000)       38 2023-04-23 08:39:32.037077 infrabed-0.0.5/setup.cfg
--rw-rw-r--   0 yamen     (1000) yamen     (1000)     1359 2023-04-23 08:39:26.000000 infrabed-0.0.5/setup.py
+drwxrwxr-x   0 yamen     (1000) yamen     (1000)        0 2023-04-23 12:34:13.863787 infrabed-0.0.6/
+-rw-rw-r--   0 yamen     (1000) yamen     (1000)     7048 2023-04-23 08:25:23.000000 infrabed-0.0.6/LICENSE
+-rw-rw-r--   0 yamen     (1000) yamen     (1000)     1075 2023-04-23 12:34:13.863787 infrabed-0.0.6/PKG-INFO
+-rw-rw-r--   0 yamen     (1000) yamen     (1000)       12 2023-04-23 08:25:37.000000 infrabed-0.0.6/README.md
+drwxrwxr-x   0 yamen     (1000) yamen     (1000)        0 2023-04-23 12:34:13.863787 infrabed-0.0.6/infrabed/
+-rw-rw-r--   0 yamen     (1000) yamen     (1000)       27 2023-04-23 12:30:27.000000 infrabed-0.0.6/infrabed/__init__.py
+-rw-rw-r--   0 yamen     (1000) yamen     (1000)     4826 2023-04-23 12:23:14.000000 infrabed-0.0.6/infrabed/client.py
+drwxrwxr-x   0 yamen     (1000) yamen     (1000)        0 2023-04-23 12:34:13.863787 infrabed-0.0.6/infrabed.egg-info/
+-rw-rw-r--   0 yamen     (1000) yamen     (1000)     1075 2023-04-23 12:34:13.000000 infrabed-0.0.6/infrabed.egg-info/PKG-INFO
+-rw-rw-r--   0 yamen     (1000) yamen     (1000)      194 2023-04-23 12:34:13.000000 infrabed-0.0.6/infrabed.egg-info/SOURCES.txt
+-rw-rw-r--   0 yamen     (1000) yamen     (1000)        1 2023-04-23 12:34:13.000000 infrabed-0.0.6/infrabed.egg-info/dependency_links.txt
+-rw-rw-r--   0 yamen     (1000) yamen     (1000)        9 2023-04-23 12:34:13.000000 infrabed-0.0.6/infrabed.egg-info/top_level.txt
+-rw-rw-r--   0 yamen     (1000) yamen     (1000)       38 2023-04-23 12:34:13.863787 infrabed-0.0.6/setup.cfg
+-rw-rw-r--   0 yamen     (1000) yamen     (1000)     1359 2023-04-23 12:33:46.000000 infrabed-0.0.6/setup.py
```

### Comparing `infrabed-0.0.5/LICENSE` & `infrabed-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `infrabed-0.0.5/PKG-INFO` & `infrabed-0.0.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infrabed
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python library designed to simplify client-side interaction with deep learning models that perform embedding calculations.
 Author: DepDiko
 Author-email: <yamen.habib@depdiko.com>
 Keywords: python,embedding,deep learning
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `infrabed-0.0.5/infrabed/client.py` & `infrabed-0.0.6/infrabed/client.py`

 * *Files identical despite different names*

### Comparing `infrabed-0.0.5/infrabed.egg-info/PKG-INFO` & `infrabed-0.0.6/infrabed.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infrabed
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python library designed to simplify client-side interaction with deep learning models that perform embedding calculations.
 Author: DepDiko
 Author-email: <yamen.habib@depdiko.com>
 Keywords: python,embedding,deep learning
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `infrabed-0.0.5/setup.py` & `infrabed-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 
 
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 DESCRIPTION = 'Python library designed to simplify client-side interaction with deep learning models that perform embedding calculations.'
 LONG_DESCRIPTION = 'With this library, users can easily interface with APIs that provide embedding services, allowing them to quickly generate high-quality embeddings for a wide range of natural language processing (NLP) tasks. Whether you need to perform sentiment analysis, semantic similarity matching, or any other task that requires the use of embeddings, Embedding Client makes it easy to access the power of deep learning models from within your Python environment.'
 
 # Setting up
 setup(
     name="infrabed",
     version=VERSION,
```

