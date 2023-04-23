# Comparing `tmp/CLUEstering-1.2.0.tar.gz` & `tmp/CLUEstering-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CLUEstering-1.2.0.tar", last modified: Thu Oct 13 06:10:49 2022, max compression
+gzip compressed data, was "CLUEstering-1.3.0.tar", last modified: Sun Apr 23 15:14:25 2023, max compression
```

## Comparing `CLUEstering-1.2.0.tar` & `CLUEstering-1.3.0.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 simone    (1000) simone    (1000)        0 2022-10-13 06:10:49.010830 CLUEstering-1.2.0/
-drwxr-xr-x   0 simone    (1000) simone    (1000)        0 2022-10-13 06:10:49.007497 CLUEstering-1.2.0/CLUEstering/
--rw-r--r--   0 simone    (1000) simone    (1000)     8723 2022-09-26 13:50:03.000000 CLUEstering-1.2.0/CLUEstering/CLUEstering.py
--rw-r--r--   0 simone    (1000) simone    (1000)       93 2022-09-26 13:50:03.000000 CLUEstering-1.2.0/CLUEstering/__init__.py
--rw-r--r--   0 simone    (1000) simone    (1000)    17978 2022-10-13 06:05:47.000000 CLUEstering-1.2.0/CLUEstering/binding.cc
-drwxr-xr-x   0 simone    (1000) simone    (1000)        0 2022-10-13 06:10:49.007497 CLUEstering-1.2.0/CLUEstering.egg-info/
--rw-r--r--   0 simone    (1000) simone    (1000)     3338 2022-10-13 06:10:48.000000 CLUEstering-1.2.0/CLUEstering.egg-info/PKG-INFO
--rw-r--r--   0 simone    (1000) simone    (1000)      289 2022-10-13 06:10:48.000000 CLUEstering-1.2.0/CLUEstering.egg-info/SOURCES.txt
--rw-r--r--   0 simone    (1000) simone    (1000)        1 2022-10-13 06:10:48.000000 CLUEstering-1.2.0/CLUEstering.egg-info/dependency_links.txt
--rw-r--r--   0 simone    (1000) simone    (1000)       32 2022-10-13 06:10:48.000000 CLUEstering-1.2.0/CLUEstering.egg-info/requires.txt
--rw-r--r--   0 simone    (1000) simone    (1000)       27 2022-10-13 06:10:48.000000 CLUEstering-1.2.0/CLUEstering.egg-info/top_level.txt
--rw-r--r--   0 simone    (1000) simone    (1000)    35149 2022-09-26 08:10:11.000000 CLUEstering-1.2.0/LICENSE
--rw-r--r--   0 simone    (1000) simone    (1000)     3338 2022-10-13 06:10:49.007497 CLUEstering-1.2.0/PKG-INFO
--rw-r--r--   0 simone    (1000) simone    (1000)     2772 2022-09-29 11:42:33.000000 CLUEstering-1.2.0/README.md
--rw-r--r--   0 simone    (1000) simone    (1000)      114 2022-09-26 14:23:51.000000 CLUEstering-1.2.0/pyproject.toml
--rw-r--r--   0 simone    (1000) simone    (1000)       38 2022-10-13 06:10:49.010830 CLUEstering-1.2.0/setup.cfg
--rw-r--r--   0 simone    (1000) simone    (1000)     1093 2022-10-13 06:06:17.000000 CLUEstering-1.2.0/setup.py
+drwxr-xr-x   0 simone    (1000) simone    (1000)        0 2023-04-23 15:14:25.834700 CLUEstering-1.3.0/
+drwxr-xr-x   0 simone    (1000) simone    (1000)        0 2023-04-23 15:14:25.834700 CLUEstering-1.3.0/CLUEstering/
+-rw-r--r--   0 simone    (1000) simone    (1000)    16173 2023-04-19 13:58:15.000000 CLUEstering-1.3.0/CLUEstering/CLUEstering.py
+-rw-r--r--   0 simone    (1000) simone    (1000)       92 2023-04-19 13:58:15.000000 CLUEstering-1.3.0/CLUEstering/__init__.py
+-rw-r--r--   0 simone    (1000) simone    (1000)     8452 2023-04-19 13:58:15.000000 CLUEstering-1.3.0/CLUEstering/binding.cc
+drwxr-xr-x   0 simone    (1000) simone    (1000)        0 2023-04-23 15:14:25.834700 CLUEstering-1.3.0/CLUEstering.egg-info/
+-rw-r--r--   0 simone    (1000) simone    (1000)     3338 2023-04-23 15:14:25.000000 CLUEstering-1.3.0/CLUEstering.egg-info/PKG-INFO
+-rw-r--r--   0 simone    (1000) simone    (1000)      331 2023-04-23 15:14:25.000000 CLUEstering-1.3.0/CLUEstering.egg-info/SOURCES.txt
+-rw-r--r--   0 simone    (1000) simone    (1000)        1 2023-04-23 15:14:25.000000 CLUEstering-1.3.0/CLUEstering.egg-info/dependency_links.txt
+-rw-r--r--   0 simone    (1000) simone    (1000)       37 2023-04-23 15:14:25.000000 CLUEstering-1.3.0/CLUEstering.egg-info/requires.txt
+-rw-r--r--   0 simone    (1000) simone    (1000)       27 2023-04-23 15:14:25.000000 CLUEstering-1.3.0/CLUEstering.egg-info/top_level.txt
+-rw-r--r--   0 simone    (1000) simone    (1000)    35149 2023-04-19 13:58:15.000000 CLUEstering-1.3.0/LICENSE
+-rw-r--r--   0 simone    (1000) simone    (1000)     3338 2023-04-23 15:14:25.834700 CLUEstering-1.3.0/PKG-INFO
+-rw-r--r--   0 simone    (1000) simone    (1000)     2772 2023-04-19 13:58:15.000000 CLUEstering-1.3.0/README.md
+-rw-r--r--   0 simone    (1000) simone    (1000)      114 2023-04-19 13:58:15.000000 CLUEstering-1.3.0/pyproject.toml
+-rw-r--r--   0 simone    (1000) simone    (1000)       38 2023-04-23 15:14:25.834700 CLUEstering-1.3.0/setup.cfg
+-rw-r--r--   0 simone    (1000) simone    (1000)     1146 2023-04-19 13:58:15.000000 CLUEstering-1.3.0/setup.py
+drwxr-xr-x   0 simone    (1000) simone    (1000)        0 2023-04-23 15:14:25.834700 CLUEstering-1.3.0/tests/
+-rw-r--r--   0 simone    (1000) simone    (1000)      267 2023-04-19 13:58:15.000000 CLUEstering-1.3.0/tests/test_blob.py
+-rw-r--r--   0 simone    (1000) simone    (1000)      335 2023-04-19 13:58:15.000000 CLUEstering-1.3.0/tests/test_blobtime.py
```

### Comparing `CLUEstering-1.2.0/CLUEstering.egg-info/PKG-INFO` & `CLUEstering-1.3.0/CLUEstering.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CLUEstering
-Version: 1.2.0
+Version: 1.3.0
 Summary: A library that generalizes the original 2-dimensional CLUE algorithm made at CERN.
 Author: Simone Balducci
 Author-email: simone.balducci00@gmail.com
 Keywords: Python,Clustering,Binding
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `CLUEstering-1.2.0/LICENSE` & `CLUEstering-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `CLUEstering-1.2.0/PKG-INFO` & `CLUEstering-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CLUEstering
-Version: 1.2.0
+Version: 1.3.0
 Summary: A library that generalizes the original 2-dimensional CLUE algorithm made at CERN.
 Author: Simone Balducci
 Author-email: simone.balducci00@gmail.com
 Keywords: Python,Clustering,Binding
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `CLUEstering-1.2.0/README.md` & `CLUEstering-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `CLUEstering-1.2.0/setup.py` & `CLUEstering-1.3.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 from setuptools import setup, find_packages
 from pybind11.setup_helpers import Pybind11Extension
 from pathlib import Path
 import codecs
 import os
 
-__version__ = "1.2.0"
+__version__ = "1.3.0"
 this_directory = Path(__file__).parent
 long_description = (this_directory/'README.md').read_text() 
 
 ext_modules = [
 	Pybind11Extension(
 		"CLUEsteringCPP",
 		['CLUEstering/binding.cc'],
+        include_dirs = ['CLUEstering/include/']
 	),
 ]
 
 setup(
     name="CLUEstering",
     version=__version__,
     author="Simone Balducci",
     author_email="simone.balducci00@gmail.com",
     description="A library that generalizes the original 2-dimensional CLUE algorithm made at CERN.",
 	 long_description=long_description,
 	 long_description_content_type='text/markdown',
 	 packages=find_packages(),
-	 install_requires=['sklearn','numpy','matplotlib','pandas'],
+	 install_requires=['scikit-learn','numpy','matplotlib','pandas'],
 	 ext_modules=ext_modules,
 	 keywords=['Python','Clustering','Binding'],
 	 python_requires='>=3.7',
 	 classifiers=[
 		'Intended Audience :: Developers',
 		'Programming Language :: Python :: 3',
 		'Operating System :: Unix',
```

