# Comparing `tmp/yuanfen-1.0.0.tar.gz` & `tmp/yuanfen-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yuanfen-1.0.0.tar", last modified: Sun Apr 23 06:27:59 2023, max compression
+gzip compressed data, was "yuanfen-1.0.1.tar", last modified: Sun Apr 23 06:47:14 2023, max compression
```

## Comparing `yuanfen-1.0.0.tar` & `yuanfen-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxr-xr-x   0 bean       (501) staff       (20)        0 2023-04-23 06:27:59.447583 yuanfen-1.0.0/
--rw-r--r--   0 bean       (501) staff       (20)      962 2023-04-23 06:27:59.447429 yuanfen-1.0.0/PKG-INFO
--rw-r--r--   0 bean       (501) staff       (20)      635 2023-04-23 06:23:40.000000 yuanfen-1.0.0/README.md
--rw-r--r--   0 bean       (501) staff       (20)       38 2023-04-23 06:27:59.447625 yuanfen-1.0.0/setup.cfg
--rw-r--r--   0 bean       (501) staff       (20)      515 2023-04-23 06:18:12.000000 yuanfen-1.0.0/setup.py
-drwxr-xr-x   0 bean       (501) staff       (20)        0 2023-04-23 06:27:59.446503 yuanfen-1.0.0/utils/
--rw-r--r--   0 bean       (501) staff       (20)        0 2023-04-23 05:49:11.000000 yuanfen-1.0.0/utils/__init__.py
--rw-r--r--   0 bean       (501) staff       (20)     1791 2023-04-23 05:50:05.000000 yuanfen-1.0.0/utils/config.py
--rw-r--r--   0 bean       (501) staff       (20)      804 2023-04-23 06:18:49.000000 yuanfen-1.0.0/utils/logger.py
-drwxr-xr-x   0 bean       (501) staff       (20)        0 2023-04-23 06:27:59.447215 yuanfen-1.0.0/yuanfen.egg-info/
--rw-r--r--   0 bean       (501) staff       (20)      962 2023-04-23 06:27:59.000000 yuanfen-1.0.0/yuanfen.egg-info/PKG-INFO
--rw-r--r--   0 bean       (501) staff       (20)      192 2023-04-23 06:27:59.000000 yuanfen-1.0.0/yuanfen.egg-info/SOURCES.txt
--rw-r--r--   0 bean       (501) staff       (20)        1 2023-04-23 06:27:59.000000 yuanfen-1.0.0/yuanfen.egg-info/dependency_links.txt
--rw-r--r--   0 bean       (501) staff       (20)        6 2023-04-23 06:27:59.000000 yuanfen-1.0.0/yuanfen.egg-info/top_level.txt
+drwxr-xr-x   0 bean       (501) staff       (20)        0 2023-04-23 06:47:14.865203 yuanfen-1.0.1/
+-rw-r--r--   0 bean       (501) staff       (20)      962 2023-04-23 06:47:14.865017 yuanfen-1.0.1/PKG-INFO
+-rw-r--r--   0 bean       (501) staff       (20)      635 2023-04-23 06:23:40.000000 yuanfen-1.0.1/README.md
+-rw-r--r--   0 bean       (501) staff       (20)       38 2023-04-23 06:47:14.865248 yuanfen-1.0.1/setup.cfg
+-rw-r--r--   0 bean       (501) staff       (20)      515 2023-04-23 06:46:50.000000 yuanfen-1.0.1/setup.py
+drwxr-xr-x   0 bean       (501) staff       (20)        0 2023-04-23 06:47:14.863922 yuanfen-1.0.1/utils/
+-rw-r--r--   0 bean       (501) staff       (20)     1791 2023-04-23 05:50:05.000000 yuanfen-1.0.1/utils/config.py
+-rw-r--r--   0 bean       (501) staff       (20)      804 2023-04-23 06:18:49.000000 yuanfen-1.0.1/utils/logger.py
+drwxr-xr-x   0 bean       (501) staff       (20)        0 2023-04-23 06:47:14.864750 yuanfen-1.0.1/yuanfen.egg-info/
+-rw-r--r--   0 bean       (501) staff       (20)      962 2023-04-23 06:47:14.000000 yuanfen-1.0.1/yuanfen.egg-info/PKG-INFO
+-rw-r--r--   0 bean       (501) staff       (20)      174 2023-04-23 06:47:14.000000 yuanfen-1.0.1/yuanfen.egg-info/SOURCES.txt
+-rw-r--r--   0 bean       (501) staff       (20)        1 2023-04-23 06:47:14.000000 yuanfen-1.0.1/yuanfen.egg-info/dependency_links.txt
+-rw-r--r--   0 bean       (501) staff       (20)        1 2023-04-23 06:47:14.000000 yuanfen-1.0.1/yuanfen.egg-info/top_level.txt
```

### Comparing `yuanfen-1.0.0/PKG-INFO` & `yuanfen-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yuanfen
-Version: 1.0.0
+Version: 1.0.1
 Summary: Yuanfen Python Library
 Home-page: 
 Author: Bean
 Author-email: bean@yuanfen.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yuanfen-1.0.0/README.md` & `yuanfen-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `yuanfen-1.0.0/setup.py` & `yuanfen-1.0.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yuanfen",
-  version="1.0.0",
+  version="1.0.1",
   author="Bean",
   author_email="bean@yuanfen.net",
   description="Yuanfen Python Library",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="",
   packages=setuptools.find_packages(),
```

### Comparing `yuanfen-1.0.0/utils/config.py` & `yuanfen-1.0.1/utils/config.py`

 * *Files identical despite different names*

### Comparing `yuanfen-1.0.0/utils/logger.py` & `yuanfen-1.0.1/utils/logger.py`

 * *Files identical despite different names*

### Comparing `yuanfen-1.0.0/yuanfen.egg-info/PKG-INFO` & `yuanfen-1.0.1/yuanfen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yuanfen
-Version: 1.0.0
+Version: 1.0.1
 Summary: Yuanfen Python Library
 Home-page: 
 Author: Bean
 Author-email: bean@yuanfen.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

