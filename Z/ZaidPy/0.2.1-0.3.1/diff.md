# Comparing `tmp/ZaidPy-0.2.1.tar.gz` & `tmp/ZaidPy-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ZaidPy-0.2.1.tar", last modified: Sat Apr 22 21:24:53 2023, max compression
+gzip compressed data, was "ZaidPy-0.3.1.tar", last modified: Sat Apr 22 21:46:35 2023, max compression
```

## Comparing `ZaidPy-0.2.1.tar` & `ZaidPy-0.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 21:24:53.516752 ZaidPy-0.2.1/
--rw-rw-rw-   0        0        0       32 2023-04-19 17:51:40.000000 ZaidPy-0.2.1/LICENSE.txt
--rw-rw-rw-   0        0        0      842 2023-04-22 21:24:53.515750 ZaidPy-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      328 2023-04-21 20:51:26.000000 ZaidPy-0.2.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-22 21:24:53.517751 ZaidPy-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      950 2023-04-22 21:22:03.000000 ZaidPy-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-22 21:24:53.484805 ZaidPy-0.2.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-22 21:24:53.495772 ZaidPy-0.2.1/src/ZaidPy/
--rw-rw-rw-   0        0        0     3292 2023-04-22 21:20:49.000000 ZaidPy-0.2.1/src/ZaidPy/ZaidPy.py
--rw-rw-rw-   0        0        0       24 2023-04-21 19:58:55.000000 ZaidPy-0.2.1/src/ZaidPy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-22 21:24:53.513751 ZaidPy-0.2.1/src/ZaidPy.egg-info/
--rw-rw-rw-   0        0        0      842 2023-04-22 21:24:53.000000 ZaidPy-0.2.1/src/ZaidPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2023-04-22 21:24:53.000000 ZaidPy-0.2.1/src/ZaidPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 21:24:53.000000 ZaidPy-0.2.1/src/ZaidPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-22 21:24:53.000000 ZaidPy-0.2.1/src/ZaidPy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-22 21:46:35.713174 ZaidPy-0.3.1/
+-rw-rw-rw-   0        0        0       32 2023-04-19 17:51:40.000000 ZaidPy-0.3.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      842 2023-04-22 21:46:35.712173 ZaidPy-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2023-04-21 20:51:26.000000 ZaidPy-0.3.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-22 21:46:35.713174 ZaidPy-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      950 2023-04-22 21:42:59.000000 ZaidPy-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 21:46:35.689301 ZaidPy-0.3.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-22 21:46:35.696297 ZaidPy-0.3.1/src/ZaidPy/
+-rw-rw-rw-   0        0        0     4276 2023-04-22 21:41:27.000000 ZaidPy-0.3.1/src/ZaidPy/ZaidPy.py
+-rw-rw-rw-   0        0        0       24 2023-04-21 19:58:55.000000 ZaidPy-0.3.1/src/ZaidPy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-22 21:46:35.710174 ZaidPy-0.3.1/src/ZaidPy.egg-info/
+-rw-rw-rw-   0        0        0      842 2023-04-22 21:46:35.000000 ZaidPy-0.3.1/src/ZaidPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2023-04-22 21:46:35.000000 ZaidPy-0.3.1/src/ZaidPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 21:46:35.000000 ZaidPy-0.3.1/src/ZaidPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-22 21:46:35.000000 ZaidPy-0.3.1/src/ZaidPy.egg-info/top_level.txt
```

### Comparing `ZaidPy-0.2.1/PKG-INFO` & `ZaidPy-0.3.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ZaidPy
-Version: 0.2.1
+Version: 0.3.1
 Summary: • Scrape Instagram Profile and login Instagram
 Home-page: 
 Author: Zaid
 Author-email: www710700@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ZaidPy-0.2.1/setup.py` & `ZaidPy-0.3.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 f.write('instaloder\nuser_agent\nrequests')
 
 fr = open("requirements.txt",'r')
 requires = fr.read().split('\n')
     
 setuptools.setup(
     name="ZaidPy",
-    version="0.2.1",
+    version="0.3.1",
     author="Zaid",
     author_email="www710700@gmail.com",
     description="• Scrape Instagram Profile and login Instagram",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     project_urls={
```

### Comparing `ZaidPy-0.2.1/src/ZaidPy.egg-info/PKG-INFO` & `ZaidPy-0.3.1/src/ZaidPy.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ZaidPy
-Version: 0.2.1
+Version: 0.3.1
 Summary: • Scrape Instagram Profile and login Instagram
 Home-page: 
 Author: Zaid
 Author-email: www710700@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

