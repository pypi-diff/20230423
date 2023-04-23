# Comparing `tmp/ml_pckg-1.1.0.tar.gz` & `tmp/ml_pckg-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml_pckg-1.1.0.tar", last modified: Sun Apr 23 13:42:41 2023, max compression
+gzip compressed data, was "ml_pckg-1.1.1.tar", last modified: Sun Apr 23 13:48:01 2023, max compression
```

## Comparing `ml_pckg-1.1.0.tar` & `ml_pckg-1.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-23 13:42:41.702522 ml_pckg-1.1.0/
--rw-r--r--   0 glebmaksimov   (501) staff       (20)     1073 2023-04-21 13:24:22.000000 ml_pckg-1.1.0/LICENSE
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      595 2023-04-23 13:42:41.702632 ml_pckg-1.1.0/PKG-INFO
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      268 2023-04-21 15:13:38.000000 ml_pckg-1.1.0/README.md
-drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-23 13:42:41.701139 ml_pckg-1.1.0/ml_pckg/
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      212 2023-04-23 13:28:28.000000 ml_pckg-1.1.0/ml_pckg/__init__.py
--rw-r--r--   0 glebmaksimov   (501) staff       (20)    14978 2023-04-23 13:30:48.000000 ml_pckg-1.1.0/ml_pckg/classifiers.py
--rw-r--r--   0 glebmaksimov   (501) staff       (20)     4737 2023-04-01 13:58:17.000000 ml_pckg-1.1.0/ml_pckg/data_processing.py
--rw-r--r--   0 glebmaksimov   (501) staff       (20)     2118 2023-04-03 14:34:37.000000 ml_pckg-1.1.0/ml_pckg/linear_algebra.py
--rw-r--r--   0 glebmaksimov   (501) staff       (20)     2932 2023-04-23 13:19:13.000000 ml_pckg-1.1.0/ml_pckg/metrics.py
--rw-r--r--   0 glebmaksimov   (501) staff       (20)    15712 2023-04-21 13:58:28.000000 ml_pckg-1.1.0/ml_pckg/regressors.py
-drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-23 13:42:41.702324 ml_pckg-1.1.0/ml_pckg.egg-info/
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      595 2023-04-23 13:42:41.000000 ml_pckg-1.1.0/ml_pckg.egg-info/PKG-INFO
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      327 2023-04-23 13:42:41.000000 ml_pckg-1.1.0/ml_pckg.egg-info/SOURCES.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)        1 2023-04-23 13:42:41.000000 ml_pckg-1.1.0/ml_pckg.egg-info/dependency_links.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)       53 2023-04-23 13:42:41.000000 ml_pckg-1.1.0/ml_pckg.egg-info/requires.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)        8 2023-04-23 13:42:41.000000 ml_pckg-1.1.0/ml_pckg.egg-info/top_level.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)       79 2023-04-23 13:42:41.702942 ml_pckg-1.1.0/setup.cfg
--rw-r--r--   0 glebmaksimov   (501) staff       (20)     1597 2023-04-23 13:42:22.000000 ml_pckg-1.1.0/setup.py
+drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-23 13:48:01.699053 ml_pckg-1.1.1/
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)     1073 2023-04-21 13:24:22.000000 ml_pckg-1.1.1/LICENSE
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      595 2023-04-23 13:48:01.699171 ml_pckg-1.1.1/PKG-INFO
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      268 2023-04-21 15:13:38.000000 ml_pckg-1.1.1/README.md
+drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-23 13:48:01.697737 ml_pckg-1.1.1/ml_pckg/
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      212 2023-04-23 13:28:28.000000 ml_pckg-1.1.1/ml_pckg/__init__.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)    14978 2023-04-23 13:30:48.000000 ml_pckg-1.1.1/ml_pckg/classifiers.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)     4737 2023-04-01 13:58:17.000000 ml_pckg-1.1.1/ml_pckg/data_processing.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)     2118 2023-04-03 14:34:37.000000 ml_pckg-1.1.1/ml_pckg/linear_algebra.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)     2932 2023-04-23 13:19:13.000000 ml_pckg-1.1.1/ml_pckg/metrics.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)    15712 2023-04-21 13:58:28.000000 ml_pckg-1.1.1/ml_pckg/regressors.py
+drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-23 13:48:01.698893 ml_pckg-1.1.1/ml_pckg.egg-info/
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      595 2023-04-23 13:48:01.000000 ml_pckg-1.1.1/ml_pckg.egg-info/PKG-INFO
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      327 2023-04-23 13:48:01.000000 ml_pckg-1.1.1/ml_pckg.egg-info/SOURCES.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)        1 2023-04-23 13:48:01.000000 ml_pckg-1.1.1/ml_pckg.egg-info/dependency_links.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)       53 2023-04-23 13:48:01.000000 ml_pckg-1.1.1/ml_pckg.egg-info/requires.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)        8 2023-04-23 13:48:01.000000 ml_pckg-1.1.1/ml_pckg.egg-info/top_level.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)       79 2023-04-23 13:48:01.699471 ml_pckg-1.1.1/setup.cfg
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)     1585 2023-04-23 13:42:41.000000 ml_pckg-1.1.1/setup.py
```

### Comparing `ml_pckg-1.1.0/LICENSE` & `ml_pckg-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ml_pckg-1.1.0/PKG-INFO` & `ml_pckg-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ml_pckg
-Version: 1.1.0
+Version: 1.1.1
 Summary: Machine Learning Models
 Home-page: UNKNOWN
 Author: Gleb Maksimov
 Author-email: glebmaksimov092@gmail.com
 License: MIT
-Download-URL: https://github.com/Glebmaksimov/ml_pckg/archive/refs/tags/1.1.0.tar.gz
+Download-URL: https://github.com/Glebmaksimov/ml_pckg/archive/refs/tags/1.1.1.tar.gz
 Keywords: ML,FROM SWCRATCH,ADVANCED
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ml_pckg-1.1.0/ml_pckg/classifiers.py` & `ml_pckg-1.1.1/ml_pckg/classifiers.py`

 * *Files identical despite different names*

### Comparing `ml_pckg-1.1.0/ml_pckg/data_processing.py` & `ml_pckg-1.1.1/ml_pckg/data_processing.py`

 * *Files identical despite different names*

### Comparing `ml_pckg-1.1.0/ml_pckg/linear_algebra.py` & `ml_pckg-1.1.1/ml_pckg/linear_algebra.py`

 * *Files identical despite different names*

### Comparing `ml_pckg-1.1.0/ml_pckg/metrics.py` & `ml_pckg-1.1.1/ml_pckg/metrics.py`

 * *Files identical despite different names*

### Comparing `ml_pckg-1.1.0/ml_pckg/regressors.py` & `ml_pckg-1.1.1/ml_pckg/regressors.py`

 * *Files identical despite different names*

### Comparing `ml_pckg-1.1.0/ml_pckg.egg-info/PKG-INFO` & `ml_pckg-1.1.1/ml_pckg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ml-pckg
-Version: 1.1.0
+Version: 1.1.1
 Summary: Machine Learning Models
 Home-page: UNKNOWN
 Author: Gleb Maksimov
 Author-email: glebmaksimov092@gmail.com
 License: MIT
-Download-URL: https://github.com/Glebmaksimov/ml_pckg/archive/refs/tags/1.1.0.tar.gz
+Download-URL: https://github.com/Glebmaksimov/ml_pckg/archive/refs/tags/1.1.1.tar.gz
 Keywords: ML,FROM SWCRATCH,ADVANCED
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ml_pckg-1.1.0/setup.py` & `ml_pckg-1.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 import re
 with open('setup.py', 'r') as f:
     setup_file = f.read()
 
-current_version = '1.1.0'
+current_version = '1.1.1'
 
 setup(
     name='ml_pckg',
     packages=['ml_pckg'],
     version=current_version,
     license='MIT',
     description='Machine Learning Models',
@@ -34,15 +34,15 @@
 major, minor, patch = current_version.split('.')
 
 new_version = int(major)*100 + int(minor)*10 + int(patch)
 new_version = str(new_version + 1)
 current_version = f'{new_version[0]}.{new_version[1]}.{new_version[2]}'
 with open('setup.py', 'w') as f:
     f.write(re.sub(r"current_version\s*=\s*'(.*?)'",
-            f"current_version = '{current_version}'", setup_file))
+            f"current_version = '1.1.1'", setup_file))
 with open("update.txt", "r") as f:
     contents = f.read()
 
 contents = contents.replace("<commit_message>", current_version + 'commit')
 contents = contents.replace("<tag_name>", current_version)
 contents = contents.replace("<tag_message>", current_version)
```

