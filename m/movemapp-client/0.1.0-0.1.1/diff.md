# Comparing `tmp/movemapp_client-0.1.0.tar.gz` & `tmp/movemapp_client-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "movemapp_client-0.1.0.tar", last modified: Sun Apr 23 17:43:30 2023, max compression
+gzip compressed data, was "movemapp_client-0.1.1.tar", last modified: Sun Apr 23 17:49:31 2023, max compression
```

## Comparing `movemapp_client-0.1.0.tar` & `movemapp_client-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 shoaib     (501) staff       (20)        0 2023-04-23 17:43:30.785354 movemapp_client-0.1.0/
--rw-r--r--   0 shoaib     (501) staff       (20)     1096 2023-04-23 11:12:32.000000 movemapp_client-0.1.0/LICENSE
--rw-r--r--   0 shoaib     (501) staff       (20)      555 2023-04-23 17:43:30.785188 movemapp_client-0.1.0/PKG-INFO
--rw-r--r--   0 shoaib     (501) staff       (20)     2554 2023-04-23 17:37:56.000000 movemapp_client-0.1.0/README.md
-drwxr-xr-x   0 shoaib     (501) staff       (20)        0 2023-04-23 17:43:30.784045 movemapp_client-0.1.0/movemapp_client/
--rw-r--r--   0 shoaib     (501) staff       (20)       94 2023-04-23 11:08:23.000000 movemapp_client-0.1.0/movemapp_client/__init__.py
--rw-r--r--   0 shoaib     (501) staff       (20)     3376 2023-04-23 15:12:03.000000 movemapp_client-0.1.0/movemapp_client/client.py
-drwxr-xr-x   0 shoaib     (501) staff       (20)        0 2023-04-23 17:43:30.784893 movemapp_client-0.1.0/movemapp_client.egg-info/
--rw-r--r--   0 shoaib     (501) staff       (20)      555 2023-04-23 17:43:30.000000 movemapp_client-0.1.0/movemapp_client.egg-info/PKG-INFO
--rw-r--r--   0 shoaib     (501) staff       (20)      274 2023-04-23 17:43:30.000000 movemapp_client-0.1.0/movemapp_client.egg-info/SOURCES.txt
--rw-r--r--   0 shoaib     (501) staff       (20)        1 2023-04-23 17:43:30.000000 movemapp_client-0.1.0/movemapp_client.egg-info/dependency_links.txt
--rw-r--r--   0 shoaib     (501) staff       (20)       56 2023-04-23 17:43:30.000000 movemapp_client-0.1.0/movemapp_client.egg-info/requires.txt
--rw-r--r--   0 shoaib     (501) staff       (20)       16 2023-04-23 17:43:30.000000 movemapp_client-0.1.0/movemapp_client.egg-info/top_level.txt
--rw-r--r--   0 shoaib     (501) staff       (20)       38 2023-04-23 17:43:30.785414 movemapp_client-0.1.0/setup.cfg
--rw-r--r--   0 shoaib     (501) staff       (20)      852 2023-04-23 17:43:20.000000 movemapp_client-0.1.0/setup.py
+drwxr-xr-x   0 shoaib     (501) staff       (20)        0 2023-04-23 17:49:31.796062 movemapp_client-0.1.1/
+-rw-r--r--   0 shoaib     (501) staff       (20)     1096 2023-04-23 11:12:32.000000 movemapp_client-0.1.1/LICENSE
+-rw-r--r--   0 shoaib     (501) staff       (20)      450 2023-04-23 17:49:31.795910 movemapp_client-0.1.1/PKG-INFO
+-rw-r--r--   0 shoaib     (501) staff       (20)     2554 2023-04-23 17:37:56.000000 movemapp_client-0.1.1/README.md
+drwxr-xr-x   0 shoaib     (501) staff       (20)        0 2023-04-23 17:49:31.794775 movemapp_client-0.1.1/movemapp_client/
+-rw-r--r--   0 shoaib     (501) staff       (20)       94 2023-04-23 11:08:23.000000 movemapp_client-0.1.1/movemapp_client/__init__.py
+-rw-r--r--   0 shoaib     (501) staff       (20)     3376 2023-04-23 15:12:03.000000 movemapp_client-0.1.1/movemapp_client/client.py
+drwxr-xr-x   0 shoaib     (501) staff       (20)        0 2023-04-23 17:49:31.795693 movemapp_client-0.1.1/movemapp_client.egg-info/
+-rw-r--r--   0 shoaib     (501) staff       (20)      450 2023-04-23 17:49:31.000000 movemapp_client-0.1.1/movemapp_client.egg-info/PKG-INFO
+-rw-r--r--   0 shoaib     (501) staff       (20)      274 2023-04-23 17:49:31.000000 movemapp_client-0.1.1/movemapp_client.egg-info/SOURCES.txt
+-rw-r--r--   0 shoaib     (501) staff       (20)        1 2023-04-23 17:49:31.000000 movemapp_client-0.1.1/movemapp_client.egg-info/dependency_links.txt
+-rw-r--r--   0 shoaib     (501) staff       (20)       56 2023-04-23 17:49:31.000000 movemapp_client-0.1.1/movemapp_client.egg-info/requires.txt
+-rw-r--r--   0 shoaib     (501) staff       (20)       16 2023-04-23 17:49:31.000000 movemapp_client-0.1.1/movemapp_client.egg-info/top_level.txt
+-rw-r--r--   0 shoaib     (501) staff       (20)       38 2023-04-23 17:49:31.796115 movemapp_client-0.1.1/setup.cfg
+-rw-r--r--   0 shoaib     (501) staff       (20)      749 2023-04-23 17:48:53.000000 movemapp_client-0.1.1/setup.py
```

### Comparing `movemapp_client-0.1.0/LICENSE` & `movemapp_client-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `movemapp_client-0.1.0/README.md` & `movemapp_client-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `movemapp_client-0.1.0/movemapp_client/client.py` & `movemapp_client-0.1.1/movemapp_client/client.py`

 * *Files identical despite different names*

### Comparing `movemapp_client-0.1.0/setup.py` & `movemapp_client-0.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="movemapp_client",
-    version="0.1.0",
+    version="0.1.1",
     packages=find_packages(),
     install_requires=[
          "carto",
          "python-dotenv"
     ],
     # dev dependencies
     extras_require={
@@ -19,13 +19,11 @@
     description="A Python package for Movemapp client",
     author="Shoaib Burq",
     author_email="shoaib@geografia.com.au",
     url="https://github.com/geografia-au/movemapp_client",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
-        "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11"
+        "Operating System :: OS Independent",
+        "License :: OSI Approved :: MIT License"
     ],
 )
```

