# Comparing `tmp/nlpie-0.3.1.tar.gz` & `tmp/nlpie-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlpie-0.3.1.tar", last modified: Sun Apr 23 19:10:32 2023, max compression
+gzip compressed data, was "nlpie-0.3.2.tar", last modified: Sun Apr 23 19:30:02 2023, max compression
```

## Comparing `nlpie-0.3.1.tar` & `nlpie-0.3.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 omid       (502) staff       (20)        0 2023-04-23 19:10:32.365249 nlpie-0.3.1/
--rw-r--r--   0 omid       (502) staff       (20)     2055 2023-04-23 19:10:32.364297 nlpie-0.3.1/PKG-INFO
--rw-r--r--   0 omid       (502) staff       (20)     1587 2023-04-21 21:19:38.000000 nlpie-0.3.1/README.md
-drwxr-xr-x   0 omid       (502) staff       (20)        0 2023-04-23 19:10:32.362683 nlpie-0.3.1/nlpie.egg-info/
--rw-r--r--   0 omid       (502) staff       (20)     2055 2023-04-23 19:10:31.000000 nlpie-0.3.1/nlpie.egg-info/PKG-INFO
--rw-r--r--   0 omid       (502) staff       (20)      162 2023-04-23 19:10:32.000000 nlpie-0.3.1/nlpie.egg-info/SOURCES.txt
--rw-r--r--   0 omid       (502) staff       (20)        1 2023-04-23 19:10:31.000000 nlpie-0.3.1/nlpie.egg-info/dependency_links.txt
--rw-r--r--   0 omid       (502) staff       (20)       50 2023-04-23 19:10:31.000000 nlpie-0.3.1/nlpie.egg-info/requires.txt
--rw-r--r--   0 omid       (502) staff       (20)        1 2023-04-23 19:10:31.000000 nlpie-0.3.1/nlpie.egg-info/top_level.txt
--rw-r--r--   0 omid       (502) staff       (20)       38 2023-04-23 19:10:32.365350 nlpie-0.3.1/setup.cfg
--rw-r--r--   0 omid       (502) staff       (20)      816 2023-04-23 19:10:27.000000 nlpie-0.3.1/setup.py
+drwxr-xr-x   0 omid       (502) staff       (20)        0 2023-04-23 19:30:02.544170 nlpie-0.3.2/
+-rw-r--r--   0 omid       (502) staff       (20)     2041 2023-04-23 19:30:02.542946 nlpie-0.3.2/PKG-INFO
+-rw-r--r--   0 omid       (502) staff       (20)     1573 2023-04-23 19:22:32.000000 nlpie-0.3.2/README.md
+drwxr-xr-x   0 omid       (502) staff       (20)        0 2023-04-23 19:30:02.541253 nlpie-0.3.2/nlpie.egg-info/
+-rw-r--r--   0 omid       (502) staff       (20)     2041 2023-04-23 19:30:02.000000 nlpie-0.3.2/nlpie.egg-info/PKG-INFO
+-rw-r--r--   0 omid       (502) staff       (20)      162 2023-04-23 19:30:02.000000 nlpie-0.3.2/nlpie.egg-info/SOURCES.txt
+-rw-r--r--   0 omid       (502) staff       (20)        1 2023-04-23 19:30:02.000000 nlpie-0.3.2/nlpie.egg-info/dependency_links.txt
+-rw-r--r--   0 omid       (502) staff       (20)       79 2023-04-23 19:30:02.000000 nlpie-0.3.2/nlpie.egg-info/requires.txt
+-rw-r--r--   0 omid       (502) staff       (20)        1 2023-04-23 19:30:02.000000 nlpie-0.3.2/nlpie.egg-info/top_level.txt
+-rw-r--r--   0 omid       (502) staff       (20)       38 2023-04-23 19:30:02.544426 nlpie-0.3.2/setup.cfg
+-rw-r--r--   0 omid       (502) staff       (20)      821 2023-04-23 19:20:07.000000 nlpie-0.3.2/setup.py
```

### Comparing `nlpie-0.3.1/PKG-INFO` & `nlpie-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpie
-Version: 0.3.1
+Version: 0.3.2
 Summary: A lightweight clinical entity linking tool using distilled clinical language models from Huggingface and spaCy/ScispaCy
 Home-page: https://github.com/nlpie-research/nlpie
 Author: NLPie Research
 Author-email: info@nlpie.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -33,15 +33,15 @@
 
 ## Installation
 
 Install the required packages by running:
 
  
 ```bash
-pip install -r requirements.txt
+pip install nlpie
 ```
 
 ## Usage
 ### Preprocessor
 
 Use the `InputPreprocessor` class in `preprocessor.py` to preprocess an input CSV file:
```

### Comparing `nlpie-0.3.1/README.md` & `nlpie-0.3.2/nlpie.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: nlpie
+Version: 0.3.2
+Summary: A lightweight clinical entity linking tool using distilled clinical language models from Huggingface and spaCy/ScispaCy
+Home-page: https://github.com/nlpie-research/nlpie
+Author: NLPie Research
+Author-email: info@nlpie.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+
 # NLPIE: A Lightweight Entity Linker
 
 A lightweight entity linking tool using distilled clinical language models from Huggingface and spaCy/ScispaCy intended to connect clinical notes to UMLS codes. Additional mapping is available for ICD-10 and SNOMED CT entries. 
 
 ## Repository Structure
 
 ```
@@ -21,15 +33,15 @@
 
 ## Installation
 
 Install the required packages by running:
 
  
 ```bash
-pip install -r requirements.txt
+pip install nlpie
 ```
 
 ## Usage
 ### Preprocessor
 
 Use the `InputPreprocessor` class in `preprocessor.py` to preprocess an input CSV file:
```

### Comparing `nlpie-0.3.1/nlpie.egg-info/PKG-INFO` & `nlpie-0.3.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: nlpie
-Version: 0.3.1
-Summary: A lightweight clinical entity linking tool using distilled clinical language models from Huggingface and spaCy/ScispaCy
-Home-page: https://github.com/nlpie-research/nlpie
-Author: NLPie Research
-Author-email: info@nlpie.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-
 # NLPIE: A Lightweight Entity Linker
 
 A lightweight entity linking tool using distilled clinical language models from Huggingface and spaCy/ScispaCy intended to connect clinical notes to UMLS codes. Additional mapping is available for ICD-10 and SNOMED CT entries. 
 
 ## Repository Structure
 
 ```
@@ -33,15 +21,15 @@
 
 ## Installation
 
 Install the required packages by running:
 
  
 ```bash
-pip install -r requirements.txt
+pip install nlpie
 ```
 
 ## Usage
 ### Preprocessor
 
 Use the `InputPreprocessor` class in `preprocessor.py` to preprocess an input CSV file:
```

### Comparing `nlpie-0.3.1/setup.py` & `nlpie-0.3.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 
 setup(
     name='nlpie',
-    version='0.3.1',
+    version='0.3.2',
     author='NLPie Research',
     author_email='info@nlpie.com',
     description='A lightweight clinical entity linking tool using distilled clinical language models from Huggingface and spaCy/ScispaCy',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/nlpie-research/nlpie',
     packages=find_packages(include=["nlpie", "nlpie.*"]),
     install_requires=[
-        'pandas',
-        'scipy',
-        'scispacy',
-        'negspacy',
-        'torch',
-        'transformers'
+    'pandas==1.5.3',
+    'scipy',
+    'scispacy==0.5.1',
+    'negspacy==1.0.3',
+    'torch',
+    'transformers==4.28.1'
     ],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
 )
```

