# Comparing `tmp/ml_pckg-1.1.6.tar.gz` & `tmp/ml_pckg-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml_pckg-1.1.6.tar", last modified: Sun Apr 23 13:59:55 2023, max compression
+gzip compressed data, was "ml_pckg-1.1.7.tar", last modified: Sun Apr 23 14:01:24 2023, max compression
```

## Comparing `ml_pckg-1.1.6.tar` & `ml_pckg-1.1.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-23 13:59:55.146433 ml_pckg-1.1.6/
--rw-r--r--   0 glebmaksimov   (501) staff       (20)     1073 2023-04-21 13:24:22.000000 ml_pckg-1.1.6/LICENSE
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      595 2023-04-23 13:59:55.146564 ml_pckg-1.1.6/PKG-INFO
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      268 2023-04-21 15:13:38.000000 ml_pckg-1.1.6/README.md
-drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-23 13:59:55.145088 ml_pckg-1.1.6/ml_pckg/
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      212 2023-04-23 13:28:28.000000 ml_pckg-1.1.6/ml_pckg/__init__.py
--rw-r--r--   0 glebmaksimov   (501) staff       (20)    14978 2023-04-23 13:30:48.000000 ml_pckg-1.1.6/ml_pckg/classifiers.py
--rw-r--r--   0 glebmaksimov   (501) staff       (20)     4737 2023-04-01 13:58:17.000000 ml_pckg-1.1.6/ml_pckg/data_processing.py
--rw-r--r--   0 glebmaksimov   (501) staff       (20)     2118 2023-04-03 14:34:37.000000 ml_pckg-1.1.6/ml_pckg/linear_algebra.py
--rw-r--r--   0 glebmaksimov   (501) staff       (20)     2932 2023-04-23 13:19:13.000000 ml_pckg-1.1.6/ml_pckg/metrics.py
--rw-r--r--   0 glebmaksimov   (501) staff       (20)    15712 2023-04-21 13:58:28.000000 ml_pckg-1.1.6/ml_pckg/regressors.py
-drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-23 13:59:55.146250 ml_pckg-1.1.6/ml_pckg.egg-info/
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      595 2023-04-23 13:59:55.000000 ml_pckg-1.1.6/ml_pckg.egg-info/PKG-INFO
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      327 2023-04-23 13:59:55.000000 ml_pckg-1.1.6/ml_pckg.egg-info/SOURCES.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)        1 2023-04-23 13:59:55.000000 ml_pckg-1.1.6/ml_pckg.egg-info/dependency_links.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)       53 2023-04-23 13:59:55.000000 ml_pckg-1.1.6/ml_pckg.egg-info/requires.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)        8 2023-04-23 13:59:55.000000 ml_pckg-1.1.6/ml_pckg.egg-info/top_level.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)       79 2023-04-23 13:59:55.146987 ml_pckg-1.1.6/setup.cfg
--rw-r--r--   0 glebmaksimov   (501) staff       (20)     1589 2023-04-23 13:59:39.000000 ml_pckg-1.1.6/setup.py
+drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-23 14:01:24.453515 ml_pckg-1.1.7/
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)     1073 2023-04-21 13:24:22.000000 ml_pckg-1.1.7/LICENSE
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      595 2023-04-23 14:01:24.453606 ml_pckg-1.1.7/PKG-INFO
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      268 2023-04-21 15:13:38.000000 ml_pckg-1.1.7/README.md
+drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-23 14:01:24.452305 ml_pckg-1.1.7/ml_pckg/
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      212 2023-04-23 13:28:28.000000 ml_pckg-1.1.7/ml_pckg/__init__.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)    14978 2023-04-23 13:30:48.000000 ml_pckg-1.1.7/ml_pckg/classifiers.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)     4737 2023-04-01 13:58:17.000000 ml_pckg-1.1.7/ml_pckg/data_processing.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)     2118 2023-04-03 14:34:37.000000 ml_pckg-1.1.7/ml_pckg/linear_algebra.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)     2932 2023-04-23 13:19:13.000000 ml_pckg-1.1.7/ml_pckg/metrics.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)    15712 2023-04-21 13:58:28.000000 ml_pckg-1.1.7/ml_pckg/regressors.py
+drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-23 14:01:24.453344 ml_pckg-1.1.7/ml_pckg.egg-info/
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      595 2023-04-23 14:01:24.000000 ml_pckg-1.1.7/ml_pckg.egg-info/PKG-INFO
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      327 2023-04-23 14:01:24.000000 ml_pckg-1.1.7/ml_pckg.egg-info/SOURCES.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)        1 2023-04-23 14:01:24.000000 ml_pckg-1.1.7/ml_pckg.egg-info/dependency_links.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)       53 2023-04-23 14:01:24.000000 ml_pckg-1.1.7/ml_pckg.egg-info/requires.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)        8 2023-04-23 14:01:24.000000 ml_pckg-1.1.7/ml_pckg.egg-info/top_level.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)       79 2023-04-23 14:01:24.453906 ml_pckg-1.1.7/setup.cfg
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)     1588 2023-04-23 14:01:10.000000 ml_pckg-1.1.7/setup.py
```

### Comparing `ml_pckg-1.1.6/LICENSE` & `ml_pckg-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ml_pckg-1.1.6/PKG-INFO` & `ml_pckg-1.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ml_pckg
-Version: 1.1.6
+Version: 1.1.7
 Summary: Machine Learning Models
 Home-page: UNKNOWN
 Author: Gleb Maksimov
 Author-email: glebmaksimov092@gmail.com
 License: MIT
-Download-URL: https://github.com/Glebmaksimov/ml_pckg/archive/refs/tags/1.1.6.tar.gz
+Download-URL: https://github.com/Glebmaksimov/ml_pckg/archive/refs/tags/1.1.7.tar.gz
 Keywords: ML,FROM SWCRATCH,ADVANCED
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ml_pckg-1.1.6/ml_pckg/classifiers.py` & `ml_pckg-1.1.7/ml_pckg/classifiers.py`

 * *Files identical despite different names*

### Comparing `ml_pckg-1.1.6/ml_pckg/data_processing.py` & `ml_pckg-1.1.7/ml_pckg/data_processing.py`

 * *Files identical despite different names*

### Comparing `ml_pckg-1.1.6/ml_pckg/linear_algebra.py` & `ml_pckg-1.1.7/ml_pckg/linear_algebra.py`

 * *Files identical despite different names*

### Comparing `ml_pckg-1.1.6/ml_pckg/metrics.py` & `ml_pckg-1.1.7/ml_pckg/metrics.py`

 * *Files identical despite different names*

### Comparing `ml_pckg-1.1.6/ml_pckg/regressors.py` & `ml_pckg-1.1.7/ml_pckg/regressors.py`

 * *Files identical despite different names*

### Comparing `ml_pckg-1.1.6/ml_pckg.egg-info/PKG-INFO` & `ml_pckg-1.1.7/ml_pckg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ml-pckg
-Version: 1.1.6
+Version: 1.1.7
 Summary: Machine Learning Models
 Home-page: UNKNOWN
 Author: Gleb Maksimov
 Author-email: glebmaksimov092@gmail.com
 License: MIT
-Download-URL: https://github.com/Glebmaksimov/ml_pckg/archive/refs/tags/1.1.6.tar.gz
+Download-URL: https://github.com/Glebmaksimov/ml_pckg/archive/refs/tags/1.1.7.tar.gz
 Keywords: ML,FROM SWCRATCH,ADVANCED
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ml_pckg-1.1.6/setup.py` & `ml_pckg-1.1.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 import re
 with open('setup.py', 'r') as f:
     setup_file = f.read()
 
-current_version = f'1.1.6'
+current_version = f'1.1.7'
 
 setup(
     name='ml_pckg',
     packages=['ml_pckg'],
     version=current_version,
     license='MIT',
     description='Machine Learning Models',
@@ -33,15 +33,15 @@
 
 major, minor, patch = current_version.split('.')
 
 new_version = int(major)*100 + int(minor)*10 + int(patch)
 new_version = str(new_version + 1)
 with open('setup.py', 'w') as f:
     f.write(re.sub(r"current_version\s*=\s*'(.*?)'",
-            f"current_version = f'{new_version[0]}.{new_version[1]}.{new_version[2]}'", setup_file))
+            f"current_version = '{new_version[0]}.{new_version[1]}.{new_version[2]}'", setup_file))
 
 # with open("run_to_update.txt", "r") as f:
 #     contents = f.read()
 
 # contents = contents.replace("<commit_message>", current_version + 'commit')
 # contents = contents.replace("<tag_name>", current_version)
 # contents = contents.replace("<tag_message>", current_version)
```

