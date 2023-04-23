# Comparing `tmp/maxilearn-4.2.tar.gz` & `tmp/maxilearn-4.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maxilearn-4.2.tar", last modified: Sat Apr 22 17:41:40 2023, max compression
+gzip compressed data, was "maxilearn-4.4.4.tar", last modified: Sun Apr 23 10:59:19 2023, max compression
```

## Comparing `maxilearn-4.2.tar` & `maxilearn-4.4.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-22 17:41:40.202887 maxilearn-4.2/
--rw-r--r--   0 glebmaksimov   (501) staff       (20)     1073 2023-04-21 13:24:22.000000 maxilearn-4.2/LICENSE
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      595 2023-04-22 17:41:40.202988 maxilearn-4.2/PKG-INFO
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      268 2023-04-21 15:13:38.000000 maxilearn-4.2/README.md
-drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-22 17:41:40.201360 maxilearn-4.2/maxilearn/
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      182 2023-04-22 17:30:22.000000 maxilearn-4.2/maxilearn/__init__.py
--rw-r--r--   0 glebmaksimov   (501) staff       (20)    15015 2023-04-22 07:51:57.000000 maxilearn-4.2/maxilearn/classifiers.py
--rw-r--r--   0 glebmaksimov   (501) staff       (20)     4737 2023-04-01 13:58:17.000000 maxilearn-4.2/maxilearn/data_processing.py
--rw-r--r--   0 glebmaksimov   (501) staff       (20)     2118 2023-04-03 14:34:37.000000 maxilearn-4.2/maxilearn/linear_algebra.py
--rw-r--r--   0 glebmaksimov   (501) staff       (20)     2492 2023-04-16 09:06:30.000000 maxilearn-4.2/maxilearn/metrics.py
--rw-r--r--   0 glebmaksimov   (501) staff       (20)    15712 2023-04-21 13:58:28.000000 maxilearn-4.2/maxilearn/regressors.py
-drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-22 17:41:40.202708 maxilearn-4.2/maxilearn.egg-info/
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      595 2023-04-22 17:41:40.000000 maxilearn-4.2/maxilearn.egg-info/PKG-INFO
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      349 2023-04-22 17:41:40.000000 maxilearn-4.2/maxilearn.egg-info/SOURCES.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)        1 2023-04-22 17:41:40.000000 maxilearn-4.2/maxilearn.egg-info/dependency_links.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)       51 2023-04-22 17:41:40.000000 maxilearn-4.2/maxilearn.egg-info/requires.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)       10 2023-04-22 17:41:40.000000 maxilearn-4.2/maxilearn.egg-info/top_level.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)       79 2023-04-22 17:41:40.203390 maxilearn-4.2/setup.cfg
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      795 2023-04-22 17:39:32.000000 maxilearn-4.2/setup.py
+drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-23 10:59:19.651188 maxilearn-4.4.4/
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)     1073 2023-04-21 13:24:22.000000 maxilearn-4.4.4/LICENSE
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      599 2023-04-23 10:59:19.651299 maxilearn-4.4.4/PKG-INFO
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      268 2023-04-21 15:13:38.000000 maxilearn-4.4.4/README.md
+drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-23 10:59:19.649893 maxilearn-4.4.4/maxilearn/
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      182 2023-04-22 17:45:39.000000 maxilearn-4.4.4/maxilearn/__init__.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)    15015 2023-04-22 07:51:57.000000 maxilearn-4.4.4/maxilearn/classifiers.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)     4737 2023-04-01 13:58:17.000000 maxilearn-4.4.4/maxilearn/data_processing.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)     2118 2023-04-03 14:34:37.000000 maxilearn-4.4.4/maxilearn/linear_algebra.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)     2492 2023-04-16 09:06:30.000000 maxilearn-4.4.4/maxilearn/metrics.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)    15712 2023-04-21 13:58:28.000000 maxilearn-4.4.4/maxilearn/regressors.py
+drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-23 10:59:19.651017 maxilearn-4.4.4/maxilearn.egg-info/
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      599 2023-04-23 10:59:19.000000 maxilearn-4.4.4/maxilearn.egg-info/PKG-INFO
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      349 2023-04-23 10:59:19.000000 maxilearn-4.4.4/maxilearn.egg-info/SOURCES.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)        1 2023-04-23 10:59:19.000000 maxilearn-4.4.4/maxilearn.egg-info/dependency_links.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)       53 2023-04-23 10:59:19.000000 maxilearn-4.4.4/maxilearn.egg-info/requires.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)       10 2023-04-23 10:59:19.000000 maxilearn-4.4.4/maxilearn.egg-info/top_level.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)       79 2023-04-23 10:59:19.651596 maxilearn-4.4.4/setup.cfg
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)     1056 2023-04-23 10:58:14.000000 maxilearn-4.4.4/setup.py
```

### Comparing `maxilearn-4.2/LICENSE` & `maxilearn-4.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `maxilearn-4.2/PKG-INFO` & `maxilearn-4.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: maxilearn
-Version: 4.2
+Version: 4.4.4
 Summary: Machine Learning Models
 Home-page: UNKNOWN
 Author: Gleb Maksimov
 Author-email: glebmaksimov092@gmail.com
 License: MIT
-Download-URL: https://github.com/Glebmaksimov/maxilaern/archive/refs/tags/4.2.tar.gz
+Download-URL: https://github.com/Glebmaksimov/maxilaern/archive/refs/tags/4.4.4.tar.gz
 Keywords: ML,FROM SWCRATCH,ADVANCED
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `maxilearn-4.2/maxilearn/classifiers.py` & `maxilearn-4.4.4/maxilearn/classifiers.py`

 * *Files identical despite different names*

### Comparing `maxilearn-4.2/maxilearn/data_processing.py` & `maxilearn-4.4.4/maxilearn/data_processing.py`

 * *Files identical despite different names*

### Comparing `maxilearn-4.2/maxilearn/linear_algebra.py` & `maxilearn-4.4.4/maxilearn/linear_algebra.py`

 * *Files identical despite different names*

### Comparing `maxilearn-4.2/maxilearn/metrics.py` & `maxilearn-4.4.4/maxilearn/metrics.py`

 * *Files identical despite different names*

### Comparing `maxilearn-4.2/maxilearn/regressors.py` & `maxilearn-4.4.4/maxilearn/regressors.py`

 * *Files identical despite different names*

### Comparing `maxilearn-4.2/maxilearn.egg-info/PKG-INFO` & `maxilearn-4.4.4/maxilearn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: maxilearn
-Version: 4.2
+Version: 4.4.4
 Summary: Machine Learning Models
 Home-page: UNKNOWN
 Author: Gleb Maksimov
 Author-email: glebmaksimov092@gmail.com
 License: MIT
-Download-URL: https://github.com/Glebmaksimov/maxilaern/archive/refs/tags/4.2.tar.gz
+Download-URL: https://github.com/Glebmaksimov/maxilaern/archive/refs/tags/4.4.4.tar.gz
 Keywords: ML,FROM SWCRATCH,ADVANCED
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

