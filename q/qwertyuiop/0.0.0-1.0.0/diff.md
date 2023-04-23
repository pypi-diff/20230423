# Comparing `tmp/qwertyuiop-0.0.0.tar.gz` & `tmp/qwertyuiop-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwertyuiop-0.0.0.tar", last modified: Sun Apr 23 12:22:05 2023, max compression
+gzip compressed data, was "qwertyuiop-1.0.0.tar", last modified: Sun Apr 23 12:26:30 2023, max compression
```

## Comparing `qwertyuiop-0.0.0.tar` & `qwertyuiop-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-23 12:22:05.920590 qwertyuiop-0.0.0/
--rw-r--r--   0 glebmaksimov   (501) staff       (20)     1073 2023-04-21 13:24:22.000000 qwertyuiop-0.0.0/LICENSE
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      600 2023-04-23 12:22:05.920651 qwertyuiop-0.0.0/PKG-INFO
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      268 2023-04-21 15:13:38.000000 qwertyuiop-0.0.0/README.md
-drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-23 12:22:05.919712 qwertyuiop-0.0.0/qwertyuiop/
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      187 2023-04-23 12:21:14.000000 qwertyuiop-0.0.0/qwertyuiop/__init__.py
--rw-r--r--   0 glebmaksimov   (501) staff       (20)    15015 2023-04-22 07:51:57.000000 qwertyuiop-0.0.0/qwertyuiop/classifiers.py
--rw-r--r--   0 glebmaksimov   (501) staff       (20)     4737 2023-04-01 13:58:17.000000 qwertyuiop-0.0.0/qwertyuiop/data_processing.py
--rw-r--r--   0 glebmaksimov   (501) staff       (20)     2118 2023-04-03 14:34:37.000000 qwertyuiop-0.0.0/qwertyuiop/linear_algebra.py
--rw-r--r--   0 glebmaksimov   (501) staff       (20)     2492 2023-04-16 09:06:30.000000 qwertyuiop-0.0.0/qwertyuiop/metrics.py
--rw-r--r--   0 glebmaksimov   (501) staff       (20)    15712 2023-04-21 13:58:28.000000 qwertyuiop-0.0.0/qwertyuiop/regressors.py
-drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-23 12:22:05.920498 qwertyuiop-0.0.0/qwertyuiop.egg-info/
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      600 2023-04-23 12:22:05.000000 qwertyuiop-0.0.0/qwertyuiop.egg-info/PKG-INFO
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      360 2023-04-23 12:22:05.000000 qwertyuiop-0.0.0/qwertyuiop.egg-info/SOURCES.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)        1 2023-04-23 12:22:05.000000 qwertyuiop-0.0.0/qwertyuiop.egg-info/dependency_links.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)       53 2023-04-23 12:22:05.000000 qwertyuiop-0.0.0/qwertyuiop.egg-info/requires.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)       11 2023-04-23 12:22:05.000000 qwertyuiop-0.0.0/qwertyuiop.egg-info/top_level.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)       79 2023-04-23 12:22:05.920885 qwertyuiop-0.0.0/setup.cfg
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      903 2023-04-23 12:21:33.000000 qwertyuiop-0.0.0/setup.py
+drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-23 12:26:30.870058 qwertyuiop-1.0.0/
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)     1073 2023-04-21 13:24:22.000000 qwertyuiop-1.0.0/LICENSE
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      600 2023-04-23 12:26:30.870140 qwertyuiop-1.0.0/PKG-INFO
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      268 2023-04-21 15:13:38.000000 qwertyuiop-1.0.0/README.md
+drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-23 12:26:30.869143 qwertyuiop-1.0.0/qwertyuiop/
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      187 2023-04-23 12:21:14.000000 qwertyuiop-1.0.0/qwertyuiop/__init__.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)    15015 2023-04-22 07:51:57.000000 qwertyuiop-1.0.0/qwertyuiop/classifiers.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)     4737 2023-04-01 13:58:17.000000 qwertyuiop-1.0.0/qwertyuiop/data_processing.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)     2118 2023-04-03 14:34:37.000000 qwertyuiop-1.0.0/qwertyuiop/linear_algebra.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)     2492 2023-04-16 09:06:30.000000 qwertyuiop-1.0.0/qwertyuiop/metrics.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)    15712 2023-04-21 13:58:28.000000 qwertyuiop-1.0.0/qwertyuiop/regressors.py
+drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-23 12:26:30.869929 qwertyuiop-1.0.0/qwertyuiop.egg-info/
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      600 2023-04-23 12:26:30.000000 qwertyuiop-1.0.0/qwertyuiop.egg-info/PKG-INFO
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      360 2023-04-23 12:26:30.000000 qwertyuiop-1.0.0/qwertyuiop.egg-info/SOURCES.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)        1 2023-04-23 12:26:30.000000 qwertyuiop-1.0.0/qwertyuiop.egg-info/dependency_links.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)       53 2023-04-23 12:26:30.000000 qwertyuiop-1.0.0/qwertyuiop.egg-info/requires.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)       11 2023-04-23 12:26:30.000000 qwertyuiop-1.0.0/qwertyuiop.egg-info/top_level.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)       79 2023-04-23 12:26:30.870352 qwertyuiop-1.0.0/setup.cfg
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      903 2023-04-23 12:26:22.000000 qwertyuiop-1.0.0/setup.py
```

### Comparing `qwertyuiop-0.0.0/LICENSE` & `qwertyuiop-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qwertyuiop-0.0.0/PKG-INFO` & `qwertyuiop-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: qwertyuiop
-Version: 0.0.0
+Version: 1.0.0
 Summary: Machine Learning Models
 Home-page: UNKNOWN
 Author: Gleb Maksimov
 Author-email: glebmaksimov092@gmail.com
 License: MIT
-Download-URL: https://github.com/Glebmaksimov/maxilaern/archive/refs/tags/0.0.0.tar.gz
+Download-URL: https://github.com/Glebmaksimov/maxilaern/archive/refs/tags/1.0.0.tar.gz
 Keywords: ML,FROM SWCRATCH,ADVANCED
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `qwertyuiop-0.0.0/qwertyuiop/classifiers.py` & `qwertyuiop-1.0.0/qwertyuiop/classifiers.py`

 * *Files identical despite different names*

### Comparing `qwertyuiop-0.0.0/qwertyuiop/data_processing.py` & `qwertyuiop-1.0.0/qwertyuiop/data_processing.py`

 * *Files identical despite different names*

### Comparing `qwertyuiop-0.0.0/qwertyuiop/linear_algebra.py` & `qwertyuiop-1.0.0/qwertyuiop/linear_algebra.py`

 * *Files identical despite different names*

### Comparing `qwertyuiop-0.0.0/qwertyuiop/metrics.py` & `qwertyuiop-1.0.0/qwertyuiop/metrics.py`

 * *Files identical despite different names*

### Comparing `qwertyuiop-0.0.0/qwertyuiop/regressors.py` & `qwertyuiop-1.0.0/qwertyuiop/regressors.py`

 * *Files identical despite different names*

### Comparing `qwertyuiop-0.0.0/qwertyuiop.egg-info/PKG-INFO` & `qwertyuiop-1.0.0/qwertyuiop.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: qwertyuiop
-Version: 0.0.0
+Version: 1.0.0
 Summary: Machine Learning Models
 Home-page: UNKNOWN
 Author: Gleb Maksimov
 Author-email: glebmaksimov092@gmail.com
 License: MIT
-Download-URL: https://github.com/Glebmaksimov/maxilaern/archive/refs/tags/0.0.0.tar.gz
+Download-URL: https://github.com/Glebmaksimov/maxilaern/archive/refs/tags/1.0.0.tar.gz
 Keywords: ML,FROM SWCRATCH,ADVANCED
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `qwertyuiop-0.0.0/setup.py` & `qwertyuiop-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from distutils.core import setup
 from update import update_version
 
-current_version = '0.0.0'
+current_version = '1.0.0'
 
 setup(
     name='qwertyuiop',
     packages=['qwertyuiop'],
     version=current_version,
     license='MIT',
     description='Machine Learning Models',
```

