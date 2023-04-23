# Comparing `tmp/nlpie-0.3.tar.gz` & `tmp/nlpie-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlpie-0.3.tar", last modified: Fri Apr 21 21:56:29 2023, max compression
+gzip compressed data, was "nlpie-0.3.1.tar", last modified: Sun Apr 23 19:10:32 2023, max compression
```

## Comparing `nlpie-0.3.tar` & `nlpie-0.3.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 omid       (502) staff       (20)        0 2023-04-21 21:56:29.509795 nlpie-0.3/
--rw-r--r--   0 omid       (502) staff       (20)     2053 2023-04-21 21:56:29.508729 nlpie-0.3/PKG-INFO
--rw-r--r--   0 omid       (502) staff       (20)     1587 2023-04-21 21:19:38.000000 nlpie-0.3/README.md
-drwxr-xr-x   0 omid       (502) staff       (20)        0 2023-04-21 21:56:29.507238 nlpie-0.3/nlpie.egg-info/
--rw-r--r--   0 omid       (502) staff       (20)     2053 2023-04-21 21:56:29.000000 nlpie-0.3/nlpie.egg-info/PKG-INFO
--rw-r--r--   0 omid       (502) staff       (20)      162 2023-04-21 21:56:29.000000 nlpie-0.3/nlpie.egg-info/SOURCES.txt
--rw-r--r--   0 omid       (502) staff       (20)        1 2023-04-21 21:56:29.000000 nlpie-0.3/nlpie.egg-info/dependency_links.txt
--rw-r--r--   0 omid       (502) staff       (20)       50 2023-04-21 21:56:29.000000 nlpie-0.3/nlpie.egg-info/requires.txt
--rw-r--r--   0 omid       (502) staff       (20)        1 2023-04-21 21:56:29.000000 nlpie-0.3/nlpie.egg-info/top_level.txt
--rw-r--r--   0 omid       (502) staff       (20)       38 2023-04-21 21:56:29.510019 nlpie-0.3/setup.cfg
--rw-r--r--   0 omid       (502) staff       (20)      786 2023-04-21 21:56:14.000000 nlpie-0.3/setup.py
+drwxr-xr-x   0 omid       (502) staff       (20)        0 2023-04-23 19:10:32.365249 nlpie-0.3.1/
+-rw-r--r--   0 omid       (502) staff       (20)     2055 2023-04-23 19:10:32.364297 nlpie-0.3.1/PKG-INFO
+-rw-r--r--   0 omid       (502) staff       (20)     1587 2023-04-21 21:19:38.000000 nlpie-0.3.1/README.md
+drwxr-xr-x   0 omid       (502) staff       (20)        0 2023-04-23 19:10:32.362683 nlpie-0.3.1/nlpie.egg-info/
+-rw-r--r--   0 omid       (502) staff       (20)     2055 2023-04-23 19:10:31.000000 nlpie-0.3.1/nlpie.egg-info/PKG-INFO
+-rw-r--r--   0 omid       (502) staff       (20)      162 2023-04-23 19:10:32.000000 nlpie-0.3.1/nlpie.egg-info/SOURCES.txt
+-rw-r--r--   0 omid       (502) staff       (20)        1 2023-04-23 19:10:31.000000 nlpie-0.3.1/nlpie.egg-info/dependency_links.txt
+-rw-r--r--   0 omid       (502) staff       (20)       50 2023-04-23 19:10:31.000000 nlpie-0.3.1/nlpie.egg-info/requires.txt
+-rw-r--r--   0 omid       (502) staff       (20)        1 2023-04-23 19:10:31.000000 nlpie-0.3.1/nlpie.egg-info/top_level.txt
+-rw-r--r--   0 omid       (502) staff       (20)       38 2023-04-23 19:10:32.365350 nlpie-0.3.1/setup.cfg
+-rw-r--r--   0 omid       (502) staff       (20)      816 2023-04-23 19:10:27.000000 nlpie-0.3.1/setup.py
```

### Comparing `nlpie-0.3/PKG-INFO` & `nlpie-0.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpie
-Version: 0.3
+Version: 0.3.1
 Summary: A lightweight clinical entity linking tool using distilled clinical language models from Huggingface and spaCy/ScispaCy
 Home-page: https://github.com/nlpie-research/nlpie
 Author: NLPie Research
 Author-email: info@nlpie.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nlpie-0.3/README.md` & `nlpie-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `nlpie-0.3/nlpie.egg-info/PKG-INFO` & `nlpie-0.3.1/nlpie.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpie
-Version: 0.3
+Version: 0.3.1
 Summary: A lightweight clinical entity linking tool using distilled clinical language models from Huggingface and spaCy/ScispaCy
 Home-page: https://github.com/nlpie-research/nlpie
 Author: NLPie Research
 Author-email: info@nlpie.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nlpie-0.3/setup.py` & `nlpie-0.3.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name='nlpie',
-    version='0.3',
+    version='0.3.1',
     author='NLPie Research',
     author_email='info@nlpie.com',
     description='A lightweight clinical entity linking tool using distilled clinical language models from Huggingface and spaCy/ScispaCy',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/nlpie-research/nlpie',
-    packages=find_packages(),
+    packages=find_packages(include=["nlpie", "nlpie.*"]),
     install_requires=[
         'pandas',
         'scipy',
         'scispacy',
         'negspacy',
         'torch',
         'transformers'
```

