# Comparing `tmp/qcloud-python-sts-3.1.3.tar.gz` & `tmp/qcloud-python-sts-3.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/qcloud-python-sts-3.1.3.tar", last modified: Wed Jan  4 05:14:14 2023, max compression
+gzip compressed data, was "dist/qcloud-python-sts-3.1.4.tar", last modified: Sun Apr 23 07:37:37 2023, max compression
```

## Comparing `qcloud-python-sts-3.1.3.tar` & `qcloud-python-sts-3.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 libertyzhu   (501) staff       (20)        0 2023-01-04 05:14:14.000000 qcloud-python-sts-3.1.3/
--rw-r--r--   0 libertyzhu   (501) staff       (20)       42 2022-07-25 12:45:04.000000 qcloud-python-sts-3.1.3/MANIFEST.in
--rw-r--r--   0 libertyzhu   (501) staff       (20)     4922 2023-01-04 05:14:14.000000 qcloud-python-sts-3.1.3/PKG-INFO
--rw-r--r--   0 libertyzhu   (501) staff       (20)     3856 2022-09-16 06:34:39.000000 qcloud-python-sts-3.1.3/README.md
-drwxr-xr-x   0 libertyzhu   (501) staff       (20)        0 2023-01-04 05:14:14.000000 qcloud-python-sts-3.1.3/qcloud_python_sts.egg-info/
--rw-r--r--   0 libertyzhu   (501) staff       (20)     4922 2023-01-04 05:14:14.000000 qcloud-python-sts-3.1.3/qcloud_python_sts.egg-info/PKG-INFO
--rw-r--r--   0 libertyzhu   (501) staff       (20)      261 2023-01-04 05:14:14.000000 qcloud-python-sts-3.1.3/qcloud_python_sts.egg-info/SOURCES.txt
--rw-r--r--   0 libertyzhu   (501) staff       (20)        1 2023-01-04 05:14:14.000000 qcloud-python-sts-3.1.3/qcloud_python_sts.egg-info/dependency_links.txt
--rw-r--r--   0 libertyzhu   (501) staff       (20)        9 2023-01-04 05:14:14.000000 qcloud-python-sts-3.1.3/qcloud_python_sts.egg-info/requires.txt
--rw-r--r--   0 libertyzhu   (501) staff       (20)        4 2023-01-04 05:14:14.000000 qcloud-python-sts-3.1.3/qcloud_python_sts.egg-info/top_level.txt
--rw-r--r--   0 libertyzhu   (501) staff       (20)       38 2023-01-04 05:14:14.000000 qcloud-python-sts-3.1.3/setup.cfg
--rw-r--r--   0 libertyzhu   (501) staff       (20)      536 2023-01-04 05:12:08.000000 qcloud-python-sts-3.1.3/setup.py
-drwxr-xr-x   0 libertyzhu   (501) staff       (20)        0 2023-01-04 05:14:14.000000 qcloud-python-sts-3.1.3/sts/
--rw-r--r--   0 libertyzhu   (501) staff       (20)        0 2022-07-25 12:45:04.000000 qcloud-python-sts-3.1.3/sts/__init__.py
--rw-r--r--   0 libertyzhu   (501) staff       (20)    12155 2022-12-26 05:48:21.000000 qcloud-python-sts-3.1.3/sts/sts.py
+drwxr-xr-x   0 libertyzhu   (501) staff       (20)        0 2023-04-23 07:37:37.000000 qcloud-python-sts-3.1.4/
+-rw-r--r--   0 libertyzhu   (501) staff       (20)       42 2022-07-25 12:45:04.000000 qcloud-python-sts-3.1.4/MANIFEST.in
+-rw-r--r--   0 libertyzhu   (501) staff       (20)     4922 2023-04-23 07:37:37.000000 qcloud-python-sts-3.1.4/PKG-INFO
+-rw-r--r--   0 libertyzhu   (501) staff       (20)     3856 2022-09-16 06:34:39.000000 qcloud-python-sts-3.1.4/README.md
+drwxr-xr-x   0 libertyzhu   (501) staff       (20)        0 2023-04-23 07:37:37.000000 qcloud-python-sts-3.1.4/qcloud_python_sts.egg-info/
+-rw-r--r--   0 libertyzhu   (501) staff       (20)     4922 2023-04-23 07:37:37.000000 qcloud-python-sts-3.1.4/qcloud_python_sts.egg-info/PKG-INFO
+-rw-r--r--   0 libertyzhu   (501) staff       (20)      261 2023-04-23 07:37:37.000000 qcloud-python-sts-3.1.4/qcloud_python_sts.egg-info/SOURCES.txt
+-rw-r--r--   0 libertyzhu   (501) staff       (20)        1 2023-04-23 07:37:37.000000 qcloud-python-sts-3.1.4/qcloud_python_sts.egg-info/dependency_links.txt
+-rw-r--r--   0 libertyzhu   (501) staff       (20)        9 2023-04-23 07:37:37.000000 qcloud-python-sts-3.1.4/qcloud_python_sts.egg-info/requires.txt
+-rw-r--r--   0 libertyzhu   (501) staff       (20)        4 2023-04-23 07:37:37.000000 qcloud-python-sts-3.1.4/qcloud_python_sts.egg-info/top_level.txt
+-rw-r--r--   0 libertyzhu   (501) staff       (20)       38 2023-04-23 07:37:37.000000 qcloud-python-sts-3.1.4/setup.cfg
+-rw-r--r--   0 libertyzhu   (501) staff       (20)      553 2023-04-23 07:33:36.000000 qcloud-python-sts-3.1.4/setup.py
+drwxr-xr-x   0 libertyzhu   (501) staff       (20)        0 2023-04-23 07:37:37.000000 qcloud-python-sts-3.1.4/sts/
+-rw-r--r--   0 libertyzhu   (501) staff       (20)        0 2022-07-25 12:45:04.000000 qcloud-python-sts-3.1.4/sts/__init__.py
+-rw-r--r--   0 libertyzhu   (501) staff       (20)    12155 2022-12-26 05:48:21.000000 qcloud-python-sts-3.1.4/sts/sts.py
```

### Comparing `qcloud-python-sts-3.1.3/PKG-INFO` & `qcloud-python-sts-3.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcloud-python-sts
-Version: 3.1.3
+Version: 3.1.4
 Summary: this is sts for python on v3
 Home-page: https://github.com/tencentyun/qcloud-cos-sts-sdk
 Author: qcloudterminal
 Author-email: qcloudterminal@gmail.com
 License: MIT
 Description: ## 获取 SDK
```

### Comparing `qcloud-python-sts-3.1.3/README.md` & `qcloud-python-sts-3.1.4/README.md`

 * *Files identical despite different names*

### Comparing `qcloud-python-sts-3.1.3/qcloud_python_sts.egg-info/PKG-INFO` & `qcloud-python-sts-3.1.4/qcloud_python_sts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcloud-python-sts
-Version: 3.1.3
+Version: 3.1.4
 Summary: this is sts for python on v3
 Home-page: https://github.com/tencentyun/qcloud-cos-sts-sdk
 Author: qcloudterminal
 Author-email: qcloudterminal@gmail.com
 License: MIT
 Description: ## 获取 SDK
```

### Comparing `qcloud-python-sts-3.1.3/setup.py` & `qcloud-python-sts-3.1.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding=utf-8
 from setuptools import setup, find_packages
 
-with open("README.md", "r") as fh:
+with open("README.md", "r", encoding='utf8') as fh:
     long_description = fh.read()
 
 setup(
     name='qcloud-python-sts',
-    version='3.1.3',
+    version='3.1.4',
     description='this is sts for python on v3',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/tencentyun/qcloud-cos-sts-sdk',
     author='qcloudterminal',
     author_email='qcloudterminal@gmail.com',
     license='MIT',
```

### Comparing `qcloud-python-sts-3.1.3/sts/sts.py` & `qcloud-python-sts-3.1.4/sts/sts.py`

 * *Files identical despite different names*

