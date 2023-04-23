# Comparing `tmp/graph-model-parser-0.1.2.tar.gz` & `tmp/graph-model-parser-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graph-model-parser-0.1.2.tar", last modified: Sun Apr 23 18:54:29 2023, max compression
+gzip compressed data, was "graph-model-parser-0.1.3.tar", last modified: Sun Apr 23 18:56:43 2023, max compression
```

## Comparing `graph-model-parser-0.1.2.tar` & `graph-model-parser-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 albertbuchard   (501) staff       (20)        0 2023-04-23 18:54:29.155475 graph-model-parser-0.1.2/
--rw-r--r--   0 albertbuchard   (501) staff       (20)     2458 2023-04-23 18:54:29.155524 graph-model-parser-0.1.2/PKG-INFO
--rw-r--r--   0 albertbuchard   (501) staff       (20)     1782 2023-04-23 18:52:19.000000 graph-model-parser-0.1.2/README.md
-drwxr-xr-x   0 albertbuchard   (501) staff       (20)        0 2023-04-23 18:54:29.154472 graph-model-parser-0.1.2/graph_model_parser/
--rw-r--r--   0 albertbuchard   (501) staff       (20)       49 2023-04-23 18:52:31.000000 graph-model-parser-0.1.2/graph_model_parser/__init__.py
--rw-r--r--   0 albertbuchard   (501) staff       (20)     8262 2023-04-23 18:03:02.000000 graph-model-parser-0.1.2/graph_model_parser/graph_model_parser.py
-drwxr-xr-x   0 albertbuchard   (501) staff       (20)        0 2023-04-23 18:54:29.155124 graph-model-parser-0.1.2/graph_model_parser.egg-info/
--rw-r--r--   0 albertbuchard   (501) staff       (20)     2458 2023-04-23 18:54:29.000000 graph-model-parser-0.1.2/graph_model_parser.egg-info/PKG-INFO
--rw-r--r--   0 albertbuchard   (501) staff       (20)      366 2023-04-23 18:54:29.000000 graph-model-parser-0.1.2/graph_model_parser.egg-info/SOURCES.txt
--rw-r--r--   0 albertbuchard   (501) staff       (20)        1 2023-04-23 18:54:29.000000 graph-model-parser-0.1.2/graph_model_parser.egg-info/dependency_links.txt
--rw-r--r--   0 albertbuchard   (501) staff       (20)       12 2023-04-23 18:54:29.000000 graph-model-parser-0.1.2/graph_model_parser.egg-info/requires.txt
--rw-r--r--   0 albertbuchard   (501) staff       (20)       25 2023-04-23 18:54:29.000000 graph-model-parser-0.1.2/graph_model_parser.egg-info/top_level.txt
--rw-r--r--   0 albertbuchard   (501) staff       (20)      100 2023-04-23 18:19:22.000000 graph-model-parser-0.1.2/pyproject.toml
--rw-r--r--   0 albertbuchard   (501) staff       (20)      735 2023-04-23 18:54:29.155746 graph-model-parser-0.1.2/setup.cfg
-drwxr-xr-x   0 albertbuchard   (501) staff       (20)        0 2023-04-23 18:54:29.155355 graph-model-parser-0.1.2/tests/
--rw-r--r--   0 albertbuchard   (501) staff       (20)        0 2023-04-23 16:23:02.000000 graph-model-parser-0.1.2/tests/__init__.py
--rw-r--r--   0 albertbuchard   (501) staff       (20)     2262 2023-04-23 18:52:52.000000 graph-model-parser-0.1.2/tests/test_graph_model_parser.py
+drwxr-xr-x   0 albertbuchard   (501) staff       (20)        0 2023-04-23 18:56:43.964506 graph-model-parser-0.1.3/
+-rw-r--r--   0 albertbuchard   (501) staff       (20)     2443 2023-04-23 18:56:43.964576 graph-model-parser-0.1.3/PKG-INFO
+-rw-r--r--   0 albertbuchard   (501) staff       (20)     1767 2023-04-23 18:55:32.000000 graph-model-parser-0.1.3/README.md
+drwxr-xr-x   0 albertbuchard   (501) staff       (20)        0 2023-04-23 18:56:43.963356 graph-model-parser-0.1.3/graph_model_parser/
+-rw-r--r--   0 albertbuchard   (501) staff       (20)       49 2023-04-23 18:52:31.000000 graph-model-parser-0.1.3/graph_model_parser/__init__.py
+-rw-r--r--   0 albertbuchard   (501) staff       (20)     8262 2023-04-23 18:03:02.000000 graph-model-parser-0.1.3/graph_model_parser/graph_model_parser.py
+drwxr-xr-x   0 albertbuchard   (501) staff       (20)        0 2023-04-23 18:56:43.964136 graph-model-parser-0.1.3/graph_model_parser.egg-info/
+-rw-r--r--   0 albertbuchard   (501) staff       (20)     2443 2023-04-23 18:56:43.000000 graph-model-parser-0.1.3/graph_model_parser.egg-info/PKG-INFO
+-rw-r--r--   0 albertbuchard   (501) staff       (20)      366 2023-04-23 18:56:43.000000 graph-model-parser-0.1.3/graph_model_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 albertbuchard   (501) staff       (20)        1 2023-04-23 18:56:43.000000 graph-model-parser-0.1.3/graph_model_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 albertbuchard   (501) staff       (20)       12 2023-04-23 18:56:43.000000 graph-model-parser-0.1.3/graph_model_parser.egg-info/requires.txt
+-rw-r--r--   0 albertbuchard   (501) staff       (20)       25 2023-04-23 18:56:43.000000 graph-model-parser-0.1.3/graph_model_parser.egg-info/top_level.txt
+-rw-r--r--   0 albertbuchard   (501) staff       (20)      100 2023-04-23 18:19:22.000000 graph-model-parser-0.1.3/pyproject.toml
+-rw-r--r--   0 albertbuchard   (501) staff       (20)      735 2023-04-23 18:56:43.964899 graph-model-parser-0.1.3/setup.cfg
+drwxr-xr-x   0 albertbuchard   (501) staff       (20)        0 2023-04-23 18:56:43.964385 graph-model-parser-0.1.3/tests/
+-rw-r--r--   0 albertbuchard   (501) staff       (20)        0 2023-04-23 16:23:02.000000 graph-model-parser-0.1.3/tests/__init__.py
+-rw-r--r--   0 albertbuchard   (501) staff       (20)     2262 2023-04-23 18:52:52.000000 graph-model-parser-0.1.3/tests/test_graph_model_parser.py
```

### Comparing `graph-model-parser-0.1.2/PKG-INFO` & `graph-model-parser-0.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graph-model-parser
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python library for parsing and simulating dynamical graph models from string descriptions
 Home-page: https://github.com/albertbuchard/GraphModelParser
 Author: Albert Buchard
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -16,24 +16,24 @@
 
 # GraphModelParser
 
 GraphModelParser is a Python library for representing and simulating dynamical graph models from a string description. The library supports various probability distributions such as normal, poisson, expon, binom, and uniform from the `scipy.stats` module.
 
 ## Installation
 
-To install the required dependencies, simply run:
+You can install GraphModelParser from PyPI by running:
 
 ```bash
-pip install -r requirements.txt
+pip install graph-model-parser
 ```
 
 ## Usage
 
 ```python
-from graph_model_parser.graph_model_parser import GraphModelParser
+from graph_model_parser import GraphModelParser
 import numpy as np
 
 # Set seed for reproducibility
 np.random.seed(42)
 
 model_description = '''
             a_{t} = a_{t-1} + 1
```

### Comparing `graph-model-parser-0.1.2/README.md` & `graph-model-parser-0.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # GraphModelParser
 
 GraphModelParser is a Python library for representing and simulating dynamical graph models from a string description. The library supports various probability distributions such as normal, poisson, expon, binom, and uniform from the `scipy.stats` module.
 
 ## Installation
 
-To install the required dependencies, simply run:
+You can install GraphModelParser from PyPI by running:
 
 ```bash
-pip install -r requirements.txt
+pip install graph-model-parser
 ```
 
 ## Usage
 
 ```python
-from graph_model_parser.graph_model_parser import GraphModelParser
+from graph_model_parser import GraphModelParser
 import numpy as np
 
 # Set seed for reproducibility
 np.random.seed(42)
 
 model_description = '''
             a_{t} = a_{t-1} + 1
```

### Comparing `graph-model-parser-0.1.2/graph_model_parser/graph_model_parser.py` & `graph-model-parser-0.1.3/graph_model_parser/graph_model_parser.py`

 * *Files identical despite different names*

### Comparing `graph-model-parser-0.1.2/graph_model_parser.egg-info/PKG-INFO` & `graph-model-parser-0.1.3/graph_model_parser.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graph-model-parser
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python library for parsing and simulating dynamical graph models from string descriptions
 Home-page: https://github.com/albertbuchard/GraphModelParser
 Author: Albert Buchard
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -16,24 +16,24 @@
 
 # GraphModelParser
 
 GraphModelParser is a Python library for representing and simulating dynamical graph models from a string description. The library supports various probability distributions such as normal, poisson, expon, binom, and uniform from the `scipy.stats` module.
 
 ## Installation
 
-To install the required dependencies, simply run:
+You can install GraphModelParser from PyPI by running:
 
 ```bash
-pip install -r requirements.txt
+pip install graph-model-parser
 ```
 
 ## Usage
 
 ```python
-from graph_model_parser.graph_model_parser import GraphModelParser
+from graph_model_parser import GraphModelParser
 import numpy as np
 
 # Set seed for reproducibility
 np.random.seed(42)
 
 model_description = '''
             a_{t} = a_{t-1} + 1
```

### Comparing `graph-model-parser-0.1.2/setup.cfg` & `graph-model-parser-0.1.3/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = graph-model-parser
-version = 0.1.2
+version = 0.1.3
 author = Albert Buchard
 description = A Python library for parsing and simulating dynamical graph models from string descriptions
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/albertbuchard/GraphModelParser
 classifiers = 
 	Development Status :: 3 - Alpha
```

### Comparing `graph-model-parser-0.1.2/tests/test_graph_model_parser.py` & `graph-model-parser-0.1.3/tests/test_graph_model_parser.py`

 * *Files identical despite different names*

