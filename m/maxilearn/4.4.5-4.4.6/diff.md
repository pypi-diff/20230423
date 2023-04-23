# Comparing `tmp/maxilearn-4.4.5.tar.gz` & `tmp/maxilearn-4.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maxilearn-4.4.5.tar", last modified: Sun Apr 23 11:09:13 2023, max compression
+gzip compressed data, was "maxilearn-4.4.6.tar", last modified: Sun Apr 23 11:25:52 2023, max compression
```

## Comparing `maxilearn-4.4.5.tar` & `maxilearn-4.4.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-23 11:09:13.485707 maxilearn-4.4.5/
--rw-r--r--   0 glebmaksimov   (501) staff       (20)     1073 2023-04-21 13:24:22.000000 maxilearn-4.4.5/LICENSE
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      599 2023-04-23 11:09:13.485799 maxilearn-4.4.5/PKG-INFO
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      268 2023-04-21 15:13:38.000000 maxilearn-4.4.5/README.md
-drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-23 11:09:13.484421 maxilearn-4.4.5/maxilearn/
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      182 2023-04-22 17:45:39.000000 maxilearn-4.4.5/maxilearn/__init__.py
--rw-r--r--   0 glebmaksimov   (501) staff       (20)    15015 2023-04-22 07:51:57.000000 maxilearn-4.4.5/maxilearn/classifiers.py
--rw-r--r--   0 glebmaksimov   (501) staff       (20)     4737 2023-04-01 13:58:17.000000 maxilearn-4.4.5/maxilearn/data_processing.py
--rw-r--r--   0 glebmaksimov   (501) staff       (20)     2118 2023-04-03 14:34:37.000000 maxilearn-4.4.5/maxilearn/linear_algebra.py
--rw-r--r--   0 glebmaksimov   (501) staff       (20)     2492 2023-04-16 09:06:30.000000 maxilearn-4.4.5/maxilearn/metrics.py
--rw-r--r--   0 glebmaksimov   (501) staff       (20)    15712 2023-04-21 13:58:28.000000 maxilearn-4.4.5/maxilearn/regressors.py
-drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-23 11:09:13.485553 maxilearn-4.4.5/maxilearn.egg-info/
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      599 2023-04-23 11:09:13.000000 maxilearn-4.4.5/maxilearn.egg-info/PKG-INFO
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      349 2023-04-23 11:09:13.000000 maxilearn-4.4.5/maxilearn.egg-info/SOURCES.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)        1 2023-04-23 11:09:13.000000 maxilearn-4.4.5/maxilearn.egg-info/dependency_links.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)       53 2023-04-23 11:09:13.000000 maxilearn-4.4.5/maxilearn.egg-info/requires.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)       10 2023-04-23 11:09:13.000000 maxilearn-4.4.5/maxilearn.egg-info/top_level.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)       79 2023-04-23 11:09:13.486097 maxilearn-4.4.5/setup.cfg
--rw-r--r--   0 glebmaksimov   (501) staff       (20)     1088 2023-04-23 11:09:01.000000 maxilearn-4.4.5/setup.py
+drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-23 11:25:52.771036 maxilearn-4.4.6/
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)     1073 2023-04-21 13:24:22.000000 maxilearn-4.4.6/LICENSE
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      599 2023-04-23 11:25:52.771161 maxilearn-4.4.6/PKG-INFO
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      268 2023-04-21 15:13:38.000000 maxilearn-4.4.6/README.md
+drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-23 11:25:52.769706 maxilearn-4.4.6/maxilearn/
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      182 2023-04-22 17:45:39.000000 maxilearn-4.4.6/maxilearn/__init__.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)    15015 2023-04-22 07:51:57.000000 maxilearn-4.4.6/maxilearn/classifiers.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)     4737 2023-04-01 13:58:17.000000 maxilearn-4.4.6/maxilearn/data_processing.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)     2118 2023-04-03 14:34:37.000000 maxilearn-4.4.6/maxilearn/linear_algebra.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)     2492 2023-04-16 09:06:30.000000 maxilearn-4.4.6/maxilearn/metrics.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)    15712 2023-04-21 13:58:28.000000 maxilearn-4.4.6/maxilearn/regressors.py
+drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-23 11:25:52.770888 maxilearn-4.4.6/maxilearn.egg-info/
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      599 2023-04-23 11:25:52.000000 maxilearn-4.4.6/maxilearn.egg-info/PKG-INFO
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      349 2023-04-23 11:25:52.000000 maxilearn-4.4.6/maxilearn.egg-info/SOURCES.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)        1 2023-04-23 11:25:52.000000 maxilearn-4.4.6/maxilearn.egg-info/dependency_links.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)       53 2023-04-23 11:25:52.000000 maxilearn-4.4.6/maxilearn.egg-info/requires.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)       10 2023-04-23 11:25:52.000000 maxilearn-4.4.6/maxilearn.egg-info/top_level.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)       79 2023-04-23 11:25:52.771485 maxilearn-4.4.6/setup.cfg
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)     1415 2023-04-23 11:25:52.000000 maxilearn-4.4.6/setup.py
```

### Comparing `maxilearn-4.4.5/LICENSE` & `maxilearn-4.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `maxilearn-4.4.5/PKG-INFO` & `maxilearn-4.4.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: maxilearn
-Version: 4.4.5
+Version: 4.4.6
 Summary: Machine Learning Models
 Home-page: UNKNOWN
 Author: Gleb Maksimov
 Author-email: glebmaksimov092@gmail.com
 License: MIT
-Download-URL: https://github.com/Glebmaksimov/maxilaern/archive/refs/tags/4.4.5.tar.gz
+Download-URL: https://github.com/Glebmaksimov/maxilaern/archive/refs/tags/4.4.6.tar.gz
 Keywords: ML,FROM SWCRATCH,ADVANCED
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `maxilearn-4.4.5/maxilearn/classifiers.py` & `maxilearn-4.4.6/maxilearn/classifiers.py`

 * *Files identical despite different names*

### Comparing `maxilearn-4.4.5/maxilearn/data_processing.py` & `maxilearn-4.4.6/maxilearn/data_processing.py`

 * *Files identical despite different names*

### Comparing `maxilearn-4.4.5/maxilearn/linear_algebra.py` & `maxilearn-4.4.6/maxilearn/linear_algebra.py`

 * *Files identical despite different names*

### Comparing `maxilearn-4.4.5/maxilearn/metrics.py` & `maxilearn-4.4.6/maxilearn/metrics.py`

 * *Files identical despite different names*

### Comparing `maxilearn-4.4.5/maxilearn/regressors.py` & `maxilearn-4.4.6/maxilearn/regressors.py`

 * *Files identical despite different names*

### Comparing `maxilearn-4.4.5/maxilearn.egg-info/PKG-INFO` & `maxilearn-4.4.6/maxilearn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: maxilearn
-Version: 4.4.5
+Version: 4.4.6
 Summary: Machine Learning Models
 Home-page: UNKNOWN
 Author: Gleb Maksimov
 Author-email: glebmaksimov092@gmail.com
 License: MIT
-Download-URL: https://github.com/Glebmaksimov/maxilaern/archive/refs/tags/4.4.5.tar.gz
+Download-URL: https://github.com/Glebmaksimov/maxilaern/archive/refs/tags/4.4.6.tar.gz
 Keywords: ML,FROM SWCRATCH,ADVANCED
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `maxilearn-4.4.5/setup.py` & `maxilearn-4.4.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,29 @@
 from distutils.core import setup
 import re
 
+with open('setup.py', 'r') as f:
+    setup_file = f.read()
 
-current_version = '4.4.4'
+current_version = re.search(
+    r"current_version\s*=\s*'(.*?)'", setup_file).group(1)
+
+current_version = '4.4.6'
 major, minor, patch = current_version.split('.')
 new_version = int(major)*100 + int(minor)*10 + int(patch)
 new_version += 1
 new_version = str(new_version)
 current_version = f'{new_version[0]}.{new_version[1]}.{new_version[2]}'
 
+# Write the new version to setup.py
+with open('setup.py', 'w') as f:
+    f.write(re.sub(r"current_version\s*=\s*'(.*?)'",
+            f"current_version = '4.4.6'", setup_file))
+
+
 setup(
     name='maxilearn',
     packages=['maxilearn'],
     version=current_version,
     license='MIT',
     description='Machine Learning Models',
     author='Gleb Maksimov',
```

