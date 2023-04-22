# Comparing `tmp/infrabed-0.0.1.tar.gz` & `tmp/infrabed-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infrabed-0.0.1.tar", last modified: Sat Apr 22 21:10:51 2023, max compression
+gzip compressed data, was "infrabed-0.0.2.tar", last modified: Sat Apr 22 21:14:11 2023, max compression
```

## Comparing `infrabed-0.0.1.tar` & `infrabed-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,9 @@
-drwxrwxr-x   0 yamen     (1000) yamen     (1000)        0 2023-04-22 21:10:51.881182 infrabed-0.0.1/
--rw-rw-r--   0 yamen     (1000) yamen     (1000)     1053 2023-04-22 21:10:51.881182 infrabed-0.0.1/PKG-INFO
-drwxrwxr-x   0 yamen     (1000) yamen     (1000)        0 2023-04-22 21:10:51.881182 infrabed-0.0.1/infrabed.egg-info/
--rw-rw-r--   0 yamen     (1000) yamen     (1000)     1053 2023-04-22 21:10:51.000000 infrabed-0.0.1/infrabed.egg-info/PKG-INFO
--rw-rw-r--   0 yamen     (1000) yamen     (1000)      167 2023-04-22 21:10:51.000000 infrabed-0.0.1/infrabed.egg-info/SOURCES.txt
--rw-rw-r--   0 yamen     (1000) yamen     (1000)        1 2023-04-22 21:10:51.000000 infrabed-0.0.1/infrabed.egg-info/dependency_links.txt
--rw-rw-r--   0 yamen     (1000) yamen     (1000)       29 2023-04-22 21:10:51.000000 infrabed-0.0.1/infrabed.egg-info/requires.txt
--rw-rw-r--   0 yamen     (1000) yamen     (1000)        1 2023-04-22 21:10:51.000000 infrabed-0.0.1/infrabed.egg-info/top_level.txt
--rw-rw-r--   0 yamen     (1000) yamen     (1000)       38 2023-04-22 21:10:51.881182 infrabed-0.0.1/setup.cfg
--rw-rw-r--   0 yamen     (1000) yamen     (1000)     1399 2023-04-22 21:10:08.000000 infrabed-0.0.1/setup.py
+drwxrwxr-x   0 yamen     (1000) yamen     (1000)        0 2023-04-22 21:14:11.319175 infrabed-0.0.2/
+-rw-rw-r--   0 yamen     (1000) yamen     (1000)     1053 2023-04-22 21:14:11.319175 infrabed-0.0.2/PKG-INFO
+drwxrwxr-x   0 yamen     (1000) yamen     (1000)        0 2023-04-22 21:14:11.319175 infrabed-0.0.2/infrabed.egg-info/
+-rw-rw-r--   0 yamen     (1000) yamen     (1000)     1053 2023-04-22 21:14:11.000000 infrabed-0.0.2/infrabed.egg-info/PKG-INFO
+-rw-rw-r--   0 yamen     (1000) yamen     (1000)      136 2023-04-22 21:14:11.000000 infrabed-0.0.2/infrabed.egg-info/SOURCES.txt
+-rw-rw-r--   0 yamen     (1000) yamen     (1000)        1 2023-04-22 21:14:11.000000 infrabed-0.0.2/infrabed.egg-info/dependency_links.txt
+-rw-rw-r--   0 yamen     (1000) yamen     (1000)        1 2023-04-22 21:14:11.000000 infrabed-0.0.2/infrabed.egg-info/top_level.txt
+-rw-rw-r--   0 yamen     (1000) yamen     (1000)       38 2023-04-22 21:14:11.319175 infrabed-0.0.2/setup.cfg
+-rw-rw-r--   0 yamen     (1000) yamen     (1000)     1359 2023-04-22 21:13:55.000000 infrabed-0.0.2/setup.py
```

### Comparing `infrabed-0.0.1/PKG-INFO` & `infrabed-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infrabed
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python library designed to simplify client-side interaction with deep learning models that perform embedding calculations.
 Author: DepDiko
 Author-email: <yamen.habib@depdiko.com>
 Keywords: python,embedding,deep learning
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `infrabed-0.0.1/infrabed.egg-info/PKG-INFO` & `infrabed-0.0.2/infrabed.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infrabed
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python library designed to simplify client-side interaction with deep learning models that perform embedding calculations.
 Author: DepDiko
 Author-email: <yamen.habib@depdiko.com>
 Keywords: python,embedding,deep learning
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `infrabed-0.0.1/setup.py` & `infrabed-0.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Python library designed to simplify client-side interaction with deep learning models that perform embedding calculations.'
 LONG_DESCRIPTION = 'With this library, users can easily interface with APIs that provide embedding services, allowing them to quickly generate high-quality embeddings for a wide range of natural language processing (NLP) tasks. Whether you need to perform sentiment analysis, semantic similarity matching, or any other task that requires the use of embeddings, Embedding Client makes it easy to access the power of deep learning models from within your Python environment.'
 
 # Setting up
 setup(
     name="infrabed",
     version=VERSION,
     author="DepDiko",
     author_email="<yamen.habib@depdiko.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
-    install_requires=['requests', 'base64',  'hashlib', 'hmac'],
+    install_requires=[],
     keywords=['python', 'embedding', 'deep learning'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

