# Comparing `tmp/maxilearn-4.4.9.tar.gz` & `tmp/maxilearn-4.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maxilearn-4.4.9.tar", last modified: Sun Apr 23 11:57:05 2023, max compression
+gzip compressed data, was "maxilearn-4.5.0.tar", last modified: Sun Apr 23 11:57:17 2023, max compression
```

## Comparing `maxilearn-4.4.9.tar` & `maxilearn-4.5.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-23 11:57:05.154538 maxilearn-4.4.9/
--rw-r--r--   0 glebmaksimov   (501) staff       (20)     1073 2023-04-21 13:24:22.000000 maxilearn-4.4.9/LICENSE
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      599 2023-04-23 11:57:05.154649 maxilearn-4.4.9/PKG-INFO
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      268 2023-04-21 15:13:38.000000 maxilearn-4.4.9/README.md
-drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-23 11:57:05.152978 maxilearn-4.4.9/maxilearn/
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      182 2023-04-22 17:45:39.000000 maxilearn-4.4.9/maxilearn/__init__.py
--rw-r--r--   0 glebmaksimov   (501) staff       (20)    15015 2023-04-22 07:51:57.000000 maxilearn-4.4.9/maxilearn/classifiers.py
--rw-r--r--   0 glebmaksimov   (501) staff       (20)     4737 2023-04-01 13:58:17.000000 maxilearn-4.4.9/maxilearn/data_processing.py
--rw-r--r--   0 glebmaksimov   (501) staff       (20)     2118 2023-04-03 14:34:37.000000 maxilearn-4.4.9/maxilearn/linear_algebra.py
--rw-r--r--   0 glebmaksimov   (501) staff       (20)     2492 2023-04-16 09:06:30.000000 maxilearn-4.4.9/maxilearn/metrics.py
--rw-r--r--   0 glebmaksimov   (501) staff       (20)    15712 2023-04-21 13:58:28.000000 maxilearn-4.4.9/maxilearn/regressors.py
-drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-23 11:57:05.154367 maxilearn-4.4.9/maxilearn.egg-info/
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      599 2023-04-23 11:57:05.000000 maxilearn-4.4.9/maxilearn.egg-info/PKG-INFO
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      349 2023-04-23 11:57:05.000000 maxilearn-4.4.9/maxilearn.egg-info/SOURCES.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)        1 2023-04-23 11:57:05.000000 maxilearn-4.4.9/maxilearn.egg-info/dependency_links.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)       53 2023-04-23 11:57:05.000000 maxilearn-4.4.9/maxilearn.egg-info/requires.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)       10 2023-04-23 11:57:05.000000 maxilearn-4.4.9/maxilearn.egg-info/top_level.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)       79 2023-04-23 11:57:05.154964 maxilearn-4.4.9/setup.cfg
--rw-r--r--   0 glebmaksimov   (501) staff       (20)     2048 2023-04-23 11:57:05.000000 maxilearn-4.4.9/setup.py
+drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-23 11:57:17.550143 maxilearn-4.5.0/
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)     1073 2023-04-21 13:24:22.000000 maxilearn-4.5.0/LICENSE
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      599 2023-04-23 11:57:17.550319 maxilearn-4.5.0/PKG-INFO
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      268 2023-04-21 15:13:38.000000 maxilearn-4.5.0/README.md
+drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-23 11:57:17.548725 maxilearn-4.5.0/maxilearn/
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      182 2023-04-22 17:45:39.000000 maxilearn-4.5.0/maxilearn/__init__.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)    15015 2023-04-22 07:51:57.000000 maxilearn-4.5.0/maxilearn/classifiers.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)     4737 2023-04-01 13:58:17.000000 maxilearn-4.5.0/maxilearn/data_processing.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)     2118 2023-04-03 14:34:37.000000 maxilearn-4.5.0/maxilearn/linear_algebra.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)     2492 2023-04-16 09:06:30.000000 maxilearn-4.5.0/maxilearn/metrics.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)    15712 2023-04-21 13:58:28.000000 maxilearn-4.5.0/maxilearn/regressors.py
+drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-23 11:57:17.549963 maxilearn-4.5.0/maxilearn.egg-info/
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      599 2023-04-23 11:57:17.000000 maxilearn-4.5.0/maxilearn.egg-info/PKG-INFO
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      349 2023-04-23 11:57:17.000000 maxilearn-4.5.0/maxilearn.egg-info/SOURCES.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)        1 2023-04-23 11:57:17.000000 maxilearn-4.5.0/maxilearn.egg-info/dependency_links.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)       53 2023-04-23 11:57:17.000000 maxilearn-4.5.0/maxilearn.egg-info/requires.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)       10 2023-04-23 11:57:17.000000 maxilearn-4.5.0/maxilearn.egg-info/top_level.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)       79 2023-04-23 11:57:17.550670 maxilearn-4.5.0/setup.cfg
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)     2048 2023-04-23 11:57:17.000000 maxilearn-4.5.0/setup.py
```

### Comparing `maxilearn-4.4.9/LICENSE` & `maxilearn-4.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `maxilearn-4.4.9/PKG-INFO` & `maxilearn-4.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: maxilearn
-Version: 4.4.9
+Version: 4.5.0
 Summary: Machine Learning Models
 Home-page: UNKNOWN
 Author: Gleb Maksimov
 Author-email: glebmaksimov092@gmail.com
 License: MIT
-Download-URL: https://github.com/Glebmaksimov/maxilaern/archive/refs/tags/4.4.8.tar.gz
+Download-URL: https://github.com/Glebmaksimov/maxilaern/archive/refs/tags/4.4.9.tar.gz
 Keywords: ML,FROM SWCRATCH,ADVANCED
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `maxilearn-4.4.9/maxilearn/classifiers.py` & `maxilearn-4.5.0/maxilearn/classifiers.py`

 * *Files identical despite different names*

### Comparing `maxilearn-4.4.9/maxilearn/data_processing.py` & `maxilearn-4.5.0/maxilearn/data_processing.py`

 * *Files identical despite different names*

### Comparing `maxilearn-4.4.9/maxilearn/linear_algebra.py` & `maxilearn-4.5.0/maxilearn/linear_algebra.py`

 * *Files identical despite different names*

### Comparing `maxilearn-4.4.9/maxilearn/metrics.py` & `maxilearn-4.5.0/maxilearn/metrics.py`

 * *Files identical despite different names*

### Comparing `maxilearn-4.4.9/maxilearn/regressors.py` & `maxilearn-4.5.0/maxilearn/regressors.py`

 * *Files identical despite different names*

### Comparing `maxilearn-4.4.9/maxilearn.egg-info/PKG-INFO` & `maxilearn-4.5.0/maxilearn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: maxilearn
-Version: 4.4.9
+Version: 4.5.0
 Summary: Machine Learning Models
 Home-page: UNKNOWN
 Author: Gleb Maksimov
 Author-email: glebmaksimov092@gmail.com
 License: MIT
-Download-URL: https://github.com/Glebmaksimov/maxilaern/archive/refs/tags/4.4.8.tar.gz
+Download-URL: https://github.com/Glebmaksimov/maxilaern/archive/refs/tags/4.4.9.tar.gz
 Keywords: ML,FROM SWCRATCH,ADVANCED
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `maxilearn-4.4.9/setup.py` & `maxilearn-4.5.0/setup.py`

 * *Files identical despite different names*

