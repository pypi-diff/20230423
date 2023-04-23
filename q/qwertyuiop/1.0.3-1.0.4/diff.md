# Comparing `tmp/qwertyuiop-1.0.3.tar.gz` & `tmp/qwertyuiop-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwertyuiop-1.0.3.tar", last modified: Sun Apr 23 12:37:14 2023, max compression
+gzip compressed data, was "qwertyuiop-1.0.4.tar", last modified: Sun Apr 23 12:37:34 2023, max compression
```

## Comparing `qwertyuiop-1.0.3.tar` & `qwertyuiop-1.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-23 12:37:14.993252 qwertyuiop-1.0.3/
--rw-r--r--   0 glebmaksimov   (501) staff       (20)     1073 2023-04-21 13:24:22.000000 qwertyuiop-1.0.3/LICENSE
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      600 2023-04-23 12:37:14.993324 qwertyuiop-1.0.3/PKG-INFO
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      268 2023-04-21 15:13:38.000000 qwertyuiop-1.0.3/README.md
-drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-23 12:37:14.992418 qwertyuiop-1.0.3/qwertyuiop/
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      187 2023-04-23 12:21:14.000000 qwertyuiop-1.0.3/qwertyuiop/__init__.py
--rw-r--r--   0 glebmaksimov   (501) staff       (20)    15015 2023-04-22 07:51:57.000000 qwertyuiop-1.0.3/qwertyuiop/classifiers.py
--rw-r--r--   0 glebmaksimov   (501) staff       (20)     4737 2023-04-01 13:58:17.000000 qwertyuiop-1.0.3/qwertyuiop/data_processing.py
--rw-r--r--   0 glebmaksimov   (501) staff       (20)     2118 2023-04-03 14:34:37.000000 qwertyuiop-1.0.3/qwertyuiop/linear_algebra.py
--rw-r--r--   0 glebmaksimov   (501) staff       (20)     2492 2023-04-16 09:06:30.000000 qwertyuiop-1.0.3/qwertyuiop/metrics.py
--rw-r--r--   0 glebmaksimov   (501) staff       (20)    15712 2023-04-21 13:58:28.000000 qwertyuiop-1.0.3/qwertyuiop/regressors.py
-drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-23 12:37:14.993132 qwertyuiop-1.0.3/qwertyuiop.egg-info/
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      600 2023-04-23 12:37:14.000000 qwertyuiop-1.0.3/qwertyuiop.egg-info/PKG-INFO
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      360 2023-04-23 12:37:14.000000 qwertyuiop-1.0.3/qwertyuiop.egg-info/SOURCES.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)        1 2023-04-23 12:37:14.000000 qwertyuiop-1.0.3/qwertyuiop.egg-info/dependency_links.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)       53 2023-04-23 12:37:14.000000 qwertyuiop-1.0.3/qwertyuiop.egg-info/requires.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)       11 2023-04-23 12:37:14.000000 qwertyuiop-1.0.3/qwertyuiop.egg-info/top_level.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)       79 2023-04-23 12:37:14.993530 qwertyuiop-1.0.3/setup.cfg
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      904 2023-04-23 12:37:04.000000 qwertyuiop-1.0.3/setup.py
+drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-23 12:37:34.869881 qwertyuiop-1.0.4/
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)     1073 2023-04-21 13:24:22.000000 qwertyuiop-1.0.4/LICENSE
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      600 2023-04-23 12:37:34.869960 qwertyuiop-1.0.4/PKG-INFO
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      268 2023-04-21 15:13:38.000000 qwertyuiop-1.0.4/README.md
+drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-23 12:37:34.869024 qwertyuiop-1.0.4/qwertyuiop/
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      187 2023-04-23 12:21:14.000000 qwertyuiop-1.0.4/qwertyuiop/__init__.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)    15015 2023-04-22 07:51:57.000000 qwertyuiop-1.0.4/qwertyuiop/classifiers.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)     4737 2023-04-01 13:58:17.000000 qwertyuiop-1.0.4/qwertyuiop/data_processing.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)     2118 2023-04-03 14:34:37.000000 qwertyuiop-1.0.4/qwertyuiop/linear_algebra.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)     2492 2023-04-16 09:06:30.000000 qwertyuiop-1.0.4/qwertyuiop/metrics.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)    15712 2023-04-21 13:58:28.000000 qwertyuiop-1.0.4/qwertyuiop/regressors.py
+drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-23 12:37:34.869760 qwertyuiop-1.0.4/qwertyuiop.egg-info/
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      600 2023-04-23 12:37:34.000000 qwertyuiop-1.0.4/qwertyuiop.egg-info/PKG-INFO
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      360 2023-04-23 12:37:34.000000 qwertyuiop-1.0.4/qwertyuiop.egg-info/SOURCES.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)        1 2023-04-23 12:37:34.000000 qwertyuiop-1.0.4/qwertyuiop.egg-info/dependency_links.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)       53 2023-04-23 12:37:34.000000 qwertyuiop-1.0.4/qwertyuiop.egg-info/requires.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)       11 2023-04-23 12:37:34.000000 qwertyuiop-1.0.4/qwertyuiop.egg-info/top_level.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)       79 2023-04-23 12:37:34.870210 qwertyuiop-1.0.4/setup.cfg
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      904 2023-04-23 12:37:15.000000 qwertyuiop-1.0.4/setup.py
```

### Comparing `qwertyuiop-1.0.3/LICENSE` & `qwertyuiop-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qwertyuiop-1.0.3/PKG-INFO` & `qwertyuiop-1.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: qwertyuiop
-Version: 1.0.3
+Version: 1.0.4
 Summary: Machine Learning Models
 Home-page: UNKNOWN
 Author: Gleb Maksimov
 Author-email: glebmaksimov092@gmail.com
 License: MIT
-Download-URL: https://github.com/Glebmaksimov/maxilaern/archive/refs/tags/1.0.3.tar.gz
+Download-URL: https://github.com/Glebmaksimov/maxilaern/archive/refs/tags/1.0.4.tar.gz
 Keywords: ML,FROM SWCRATCH,ADVANCED
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `qwertyuiop-1.0.3/qwertyuiop/classifiers.py` & `qwertyuiop-1.0.4/qwertyuiop/classifiers.py`

 * *Files identical despite different names*

### Comparing `qwertyuiop-1.0.3/qwertyuiop/data_processing.py` & `qwertyuiop-1.0.4/qwertyuiop/data_processing.py`

 * *Files identical despite different names*

### Comparing `qwertyuiop-1.0.3/qwertyuiop/linear_algebra.py` & `qwertyuiop-1.0.4/qwertyuiop/linear_algebra.py`

 * *Files identical despite different names*

### Comparing `qwertyuiop-1.0.3/qwertyuiop/metrics.py` & `qwertyuiop-1.0.4/qwertyuiop/metrics.py`

 * *Files identical despite different names*

### Comparing `qwertyuiop-1.0.3/qwertyuiop/regressors.py` & `qwertyuiop-1.0.4/qwertyuiop/regressors.py`

 * *Files identical despite different names*

### Comparing `qwertyuiop-1.0.3/qwertyuiop.egg-info/PKG-INFO` & `qwertyuiop-1.0.4/qwertyuiop.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: qwertyuiop
-Version: 1.0.3
+Version: 1.0.4
 Summary: Machine Learning Models
 Home-page: UNKNOWN
 Author: Gleb Maksimov
 Author-email: glebmaksimov092@gmail.com
 License: MIT
-Download-URL: https://github.com/Glebmaksimov/maxilaern/archive/refs/tags/1.0.3.tar.gz
+Download-URL: https://github.com/Glebmaksimov/maxilaern/archive/refs/tags/1.0.4.tar.gz
 Keywords: ML,FROM SWCRATCH,ADVANCED
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `qwertyuiop-1.0.3/setup.py` & `qwertyuiop-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 from update import update_version
 
 
-current_version = '1.0.3'
+current_version = '1.0.4'
 
 setup(
     name='qwertyuiop',
     packages=['qwertyuiop'],
     version=current_version,
     license='MIT',
     description='Machine Learning Models',
```

