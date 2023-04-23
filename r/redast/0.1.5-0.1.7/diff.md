# Comparing `tmp/redast-0.1.5.tar.gz` & `tmp/redast-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redast-0.1.5.tar", last modified: Fri Jun 24 11:14:15 2022, max compression
+gzip compressed data, was "redast-0.1.7.tar", last modified: Sun Apr 23 21:35:52 2023, max compression
```

## Comparing `redast-0.1.5.tar` & `redast-0.1.7.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 rilshok   (1001) office    (1002)        0 2022-06-24 11:14:15.853961 redast-0.1.5/
--rw-r--r--   0 rilshok   (1001) office    (1002)     1088 2022-06-11 15:11:25.000000 redast-0.1.5/LICENSE
--rw-r--r--   0 rilshok   (1001) office    (1002)      148 2022-06-11 15:11:25.000000 redast-0.1.5/MANIFEST.in
--rw-r--r--   0 rilshok   (1001) office    (1002)     7999 2022-06-24 11:14:15.853961 redast-0.1.5/PKG-INFO
--rw-r--r--   0 rilshok   (1001) office    (1002)     7504 2022-06-11 15:11:25.000000 redast-0.1.5/README.md
-drwxr-xr-x   0 rilshok   (1001) office    (1002)        0 2022-06-24 11:14:15.849961 redast-0.1.5/redast/
--rw-r--r--   0 rilshok   (1001) office    (1002)      163 2022-06-23 14:40:02.000000 redast-0.1.5/redast/__init__.py
--rw-r--r--   0 rilshok   (1001) office    (1002)       63 2022-06-24 11:14:14.000000 redast-0.1.5/redast/__init__.pyi
--rw-r--r--   0 rilshok   (1001) office    (1002)      122 2022-06-23 14:42:37.000000 redast-0.1.5/redast/__version__.py
--rw-r--r--   0 rilshok   (1001) office    (1002)        0 2022-06-24 11:14:14.000000 redast-0.1.5/redast/__version__.pyi
-drwxr-xr-x   0 rilshok   (1001) office    (1002)        0 2022-06-24 11:14:15.853961 redast-0.1.5/redast/core/
--rw-r--r--   0 rilshok   (1001) office    (1002)      148 2022-06-23 14:40:02.000000 redast-0.1.5/redast/core/__init__.py
--rw-r--r--   0 rilshok   (1001) office    (1002)       48 2022-06-24 11:14:14.000000 redast-0.1.5/redast/core/__init__.pyi
--rw-r--r--   0 rilshok   (1001) office    (1002)     1488 2022-06-23 14:40:02.000000 redast-0.1.5/redast/core/hash.py
--rw-r--r--   0 rilshok   (1001) office    (1002)      248 2022-06-24 11:14:14.000000 redast-0.1.5/redast/core/hash.pyi
--rw-r--r--   0 rilshok   (1001) office    (1002)     4787 2022-06-23 15:32:43.000000 redast-0.1.5/redast/core/packaging.py
--rw-r--r--   0 rilshok   (1001) office    (1002)     1283 2022-06-24 11:14:14.000000 redast-0.1.5/redast/core/packaging.pyi
--rw-r--r--   0 rilshok   (1001) office    (1002)     6390 2022-06-24 11:13:09.000000 redast-0.1.5/redast/core/storage.py
--rw-r--r--   0 rilshok   (1001) office    (1002)     2070 2022-06-24 11:14:14.000000 redast-0.1.5/redast/core/storage.pyi
-drwxr-xr-x   0 rilshok   (1001) office    (1002)        0 2022-06-24 11:14:15.853961 redast-0.1.5/redast/local/
--rw-r--r--   0 rilshok   (1001) office    (1002)      186 2022-06-23 14:40:02.000000 redast-0.1.5/redast/local/__init__.py
--rw-r--r--   0 rilshok   (1001) office    (1002)       86 2022-06-24 11:14:14.000000 redast-0.1.5/redast/local/__init__.pyi
--rw-r--r--   0 rilshok   (1001) office    (1002)      621 2022-06-23 14:40:02.000000 redast-0.1.5/redast/local/cache.py
--rw-r--r--   0 rilshok   (1001) office    (1002)      281 2022-06-24 11:14:14.000000 redast-0.1.5/redast/local/cache.pyi
--rw-r--r--   0 rilshok   (1001) office    (1002)     2875 2022-06-23 14:40:40.000000 redast-0.1.5/redast/local/drive.py
--rw-r--r--   0 rilshok   (1001) office    (1002)      446 2022-06-24 11:14:14.000000 redast-0.1.5/redast/local/drive.pyi
--rw-r--r--   0 rilshok   (1001) office    (1002)      593 2022-06-23 14:40:02.000000 redast-0.1.5/redast/local/memory.py
--rw-r--r--   0 rilshok   (1001) office    (1002)      231 2022-06-24 11:14:14.000000 redast-0.1.5/redast/local/memory.pyi
--rw-r--r--   0 rilshok   (1001) office    (1002)     1811 2022-06-23 14:40:02.000000 redast-0.1.5/redast/local/sqlite.py
--rw-r--r--   0 rilshok   (1001) office    (1002)      379 2022-06-24 11:14:14.000000 redast-0.1.5/redast/local/sqlite.pyi
--rw-r--r--   0 rilshok   (1001) office    (1002)      225 2022-06-11 15:11:25.000000 redast-0.1.5/redast/py.typed
-drwxr-xr-x   0 rilshok   (1001) office    (1002)        0 2022-06-24 11:14:15.853961 redast-0.1.5/redast/remote/
--rw-r--r--   0 rilshok   (1001) office    (1002)      125 2022-06-23 14:40:02.000000 redast-0.1.5/redast/remote/__init__.py
--rw-r--r--   0 rilshok   (1001) office    (1002)       25 2022-06-24 11:14:14.000000 redast-0.1.5/redast/remote/__init__.pyi
--rw-r--r--   0 rilshok   (1001) office    (1002)     1814 2022-06-23 14:40:02.000000 redast-0.1.5/redast/remote/megacloud.py
--rw-r--r--   0 rilshok   (1001) office    (1002)      273 2022-06-24 11:14:14.000000 redast-0.1.5/redast/remote/megacloud.pyi
-drwxr-xr-x   0 rilshok   (1001) office    (1002)        0 2022-06-24 11:14:15.853961 redast-0.1.5/redast/tool/
--rw-r--r--   0 rilshok   (1001) office    (1002)      118 2022-06-23 14:40:02.000000 redast-0.1.5/redast/tool/__init__.py
--rw-r--r--   0 rilshok   (1001) office    (1002)       18 2022-06-24 11:14:14.000000 redast-0.1.5/redast/tool/__init__.pyi
--rw-r--r--   0 rilshok   (1001) office    (1002)      565 2022-06-23 14:40:02.000000 redast-0.1.5/redast/tool/io.py
--rw-r--r--   0 rilshok   (1001) office    (1002)      113 2022-06-24 11:14:14.000000 redast-0.1.5/redast/tool/io.pyi
-drwxr-xr-x   0 rilshok   (1001) office    (1002)        0 2022-06-24 11:14:15.849961 redast-0.1.5/redast.egg-info/
--rw-r--r--   0 rilshok   (1001) office    (1002)     7999 2022-06-24 11:14:15.000000 redast-0.1.5/redast.egg-info/PKG-INFO
--rw-r--r--   0 rilshok   (1001) office    (1002)      921 2022-06-24 11:14:15.000000 redast-0.1.5/redast.egg-info/SOURCES.txt
--rw-r--r--   0 rilshok   (1001) office    (1002)        1 2022-06-24 11:14:15.000000 redast-0.1.5/redast.egg-info/dependency_links.txt
--rw-r--r--   0 rilshok   (1001) office    (1002)       58 2022-06-24 11:14:15.000000 redast-0.1.5/redast.egg-info/requires.txt
--rw-r--r--   0 rilshok   (1001) office    (1002)        7 2022-06-24 11:14:15.000000 redast-0.1.5/redast.egg-info/top_level.txt
--rw-r--r--   0 rilshok   (1001) office    (1002)       58 2022-06-11 15:11:25.000000 redast-0.1.5/requirements.txt
--rw-r--r--   0 rilshok   (1001) office    (1002)       38 2022-06-24 11:14:15.853961 redast-0.1.5/setup.cfg
--rw-r--r--   0 rilshok   (1001) office    (1002)     1227 2022-06-11 15:11:25.000000 redast-0.1.5/setup.py
+drwxrwxr-x   0 rilshok   (1000) rilshok   (1000)        0 2023-04-23 21:35:52.761614 redast-0.1.7/
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)     1088 2022-04-08 07:02:34.000000 redast-0.1.7/LICENSE
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      148 2022-04-09 19:12:22.000000 redast-0.1.7/MANIFEST.in
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      824 2023-04-23 21:35:52.761614 redast-0.1.7/PKG-INFO
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      292 2023-04-23 21:33:19.000000 redast-0.1.7/README.md
+drwxrwxr-x   0 rilshok   (1000) rilshok   (1000)        0 2023-04-23 21:35:52.757614 redast-0.1.7/redast/
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      349 2023-04-23 21:33:19.000000 redast-0.1.7/redast/__init__.py
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)       63 2023-04-23 21:35:50.000000 redast-0.1.7/redast/__init__.pyi
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      122 2023-04-23 21:35:05.000000 redast-0.1.7/redast/__version__.py
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)        0 2023-04-23 21:35:50.000000 redast-0.1.7/redast/__version__.pyi
+drwxrwxr-x   0 rilshok   (1000) rilshok   (1000)        0 2023-04-23 21:35:52.757614 redast-0.1.7/redast/core/
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      148 2022-06-18 03:47:52.000000 redast-0.1.7/redast/core/__init__.py
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)       48 2023-04-23 21:35:50.000000 redast-0.1.7/redast/core/__init__.pyi
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)     1488 2022-06-18 03:44:49.000000 redast-0.1.7/redast/core/hash.py
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      248 2023-04-23 21:35:50.000000 redast-0.1.7/redast/core/hash.pyi
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)     4787 2022-08-17 19:23:58.000000 redast-0.1.7/redast/core/packaging.py
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)     1283 2023-04-23 21:35:50.000000 redast-0.1.7/redast/core/packaging.pyi
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)     6390 2022-08-17 19:23:58.000000 redast-0.1.7/redast/core/storage.py
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)     2070 2023-04-23 21:35:50.000000 redast-0.1.7/redast/core/storage.pyi
+drwxrwxr-x   0 rilshok   (1000) rilshok   (1000)        0 2023-04-23 21:35:52.757614 redast-0.1.7/redast/local/
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      186 2022-06-18 03:46:20.000000 redast-0.1.7/redast/local/__init__.py
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)       86 2023-04-23 21:35:50.000000 redast-0.1.7/redast/local/__init__.pyi
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      621 2022-06-18 03:45:10.000000 redast-0.1.7/redast/local/cache.py
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      281 2023-04-23 21:35:50.000000 redast-0.1.7/redast/local/cache.pyi
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)     2875 2022-08-17 19:23:58.000000 redast-0.1.7/redast/local/drive.py
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      446 2023-04-23 21:35:50.000000 redast-0.1.7/redast/local/drive.pyi
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      593 2022-06-18 03:45:27.000000 redast-0.1.7/redast/local/memory.py
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      231 2023-04-23 21:35:50.000000 redast-0.1.7/redast/local/memory.pyi
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)     1811 2022-06-18 03:45:37.000000 redast-0.1.7/redast/local/sqlite.py
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      379 2023-04-23 21:35:50.000000 redast-0.1.7/redast/local/sqlite.pyi
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      225 2022-06-18 03:48:02.000000 redast-0.1.7/redast/py.typed
+drwxrwxr-x   0 rilshok   (1000) rilshok   (1000)        0 2023-04-23 21:35:52.757614 redast-0.1.7/redast/remote/
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      125 2022-06-18 03:47:46.000000 redast-0.1.7/redast/remote/__init__.py
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)       25 2023-04-23 21:35:50.000000 redast-0.1.7/redast/remote/__init__.pyi
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)     1814 2022-06-18 03:46:03.000000 redast-0.1.7/redast/remote/megacloud.py
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      273 2023-04-23 21:35:50.000000 redast-0.1.7/redast/remote/megacloud.pyi
+drwxrwxr-x   0 rilshok   (1000) rilshok   (1000)        0 2023-04-23 21:35:52.761614 redast-0.1.7/redast/tool/
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      118 2022-06-18 03:47:14.000000 redast-0.1.7/redast/tool/__init__.py
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)       18 2023-04-23 21:35:50.000000 redast-0.1.7/redast/tool/__init__.pyi
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      565 2022-06-18 03:46:28.000000 redast-0.1.7/redast/tool/io.py
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      113 2023-04-23 21:35:50.000000 redast-0.1.7/redast/tool/io.pyi
+drwxrwxr-x   0 rilshok   (1000) rilshok   (1000)        0 2023-04-23 21:35:52.757614 redast-0.1.7/redast.egg-info/
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      824 2023-04-23 21:35:52.000000 redast-0.1.7/redast.egg-info/PKG-INFO
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      921 2023-04-23 21:35:52.000000 redast-0.1.7/redast.egg-info/SOURCES.txt
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)        1 2023-04-23 21:35:52.000000 redast-0.1.7/redast.egg-info/dependency_links.txt
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)       65 2023-04-23 21:35:52.000000 redast-0.1.7/redast.egg-info/requires.txt
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)        7 2023-04-23 21:35:52.000000 redast-0.1.7/redast.egg-info/top_level.txt
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)       65 2023-04-23 21:33:42.000000 redast-0.1.7/requirements.txt
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)       38 2023-04-23 21:35:52.761614 redast-0.1.7/setup.cfg
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)     1294 2023-04-23 21:33:19.000000 redast-0.1.7/setup.py
```

### Comparing `redast-0.1.5/LICENSE` & `redast-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `redast-0.1.5/redast/core/hash.py` & `redast-0.1.7/redast/core/hash.py`

 * *Files identical despite different names*

### Comparing `redast-0.1.5/redast/core/packaging.py` & `redast-0.1.7/redast/core/packaging.py`

 * *Files identical despite different names*

### Comparing `redast-0.1.5/redast/core/packaging.pyi` & `redast-0.1.7/redast/core/packaging.pyi`

 * *Files identical despite different names*

### Comparing `redast-0.1.5/redast/core/storage.py` & `redast-0.1.7/redast/core/storage.py`

 * *Files identical despite different names*

### Comparing `redast-0.1.5/redast/core/storage.pyi` & `redast-0.1.7/redast/core/storage.pyi`

 * *Files identical despite different names*

### Comparing `redast-0.1.5/redast/local/cache.py` & `redast-0.1.7/redast/local/cache.py`

 * *Files identical despite different names*

### Comparing `redast-0.1.5/redast/local/drive.py` & `redast-0.1.7/redast/local/drive.py`

 * *Files identical despite different names*

### Comparing `redast-0.1.5/redast/local/memory.py` & `redast-0.1.7/redast/local/memory.py`

 * *Files identical despite different names*

### Comparing `redast-0.1.5/redast/local/sqlite.py` & `redast-0.1.7/redast/local/sqlite.py`

 * *Files identical despite different names*

### Comparing `redast-0.1.5/redast/remote/megacloud.py` & `redast-0.1.7/redast/remote/megacloud.py`

 * *Files identical despite different names*

### Comparing `redast-0.1.5/redast/tool/io.py` & `redast-0.1.7/redast/tool/io.py`

 * *Files identical despite different names*

### Comparing `redast-0.1.5/redast.egg-info/SOURCES.txt` & `redast-0.1.7/redast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `redast-0.1.5/setup.py` & `redast-0.1.7/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,47 @@
+"""redast installation script"""
+
 import runpy
 from pathlib import Path
 
-from setuptools import find_packages, setup
+from setuptools import find_packages, setup  # type: ignore
 
-name = "redast"
-short_descriprion = "remote data storage"
-author = "Vladislav A. Proskurov"
-author_email = "rilshok@pm.me"
-url = "https://github.com/rilshok/redast"
-license = "MIT"
-classifiers = [
+NAME = "redast"
+DESCRIPTION = "remote data storage"
+LICENSE = "MIT"
+AUTHOR = "Vladislav A. Proskurov"
+AUTHOR_EMAIL = "rilshok@pm.me"
+URL = "https://github.com/rilshok/redast"
+CLASSIFIERS = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
-version_path = Path(__file__).resolve().parent / name / "__version__.py"
-version = runpy.run_path(version_path)["__version__"]
+VERSION_PATH = str(Path(__file__).resolve().parent / NAME / "__version__.py")
+VERSION = runpy.run_path(VERSION_PATH)["__version__"]
+
+with open("README.md", "r", encoding="utf-8") as file:
+    LONG_DESCRIPTION = file.read()
 
-with open("README.md", "r") as file:
-    long_description = file.read()
+with open("requirements.txt", "r", encoding="utf-8") as file:
+    REQUIREMENTS = file.read().splitlines()
 
-with open("requirements.txt", encoding="utf-8") as file:
-    requirements = file.read().splitlines()
 
 setup(
-    name=name,
-    author=author,
-    author_email=author_email,
-    descriprion=short_descriprion,
-    long_description=long_description,
+    name=NAME,
+    descriprion=DESCRIPTION,
+    long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    license=license,
-    url=url,
-    packages=find_packages(include=(name,)),
+    license=LICENSE,
+    author=AUTHOR,
+    author_email=AUTHOR_EMAIL,
+    version=VERSION,
+    url=URL,
+    packages=find_packages(include=(NAME,)),
     include_package_data=True,
-    version=version,
-    install_requires=requirements,
-    classifiers=classifiers,
+    install_requires=REQUIREMENTS,
+    classifiers=CLASSIFIERS,
     python_requires=">=3.8",
 )
```

