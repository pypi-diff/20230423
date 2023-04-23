# Comparing `tmp/klldFN-1.0.4.tar.gz` & `tmp/klldFN-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klldFN-1.0.4.tar", last modified: Thu Mar 23 09:55:50 2023, max compression
+gzip compressed data, was "klldFN-1.0.5.tar", last modified: Sun Apr 23 18:57:45 2023, max compression
```

## Comparing `klldFN-1.0.4.tar` & `klldFN-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-03-23 09:55:50.888578 klldFN-1.0.4/
--rw-r--r--   0 runner    (1000) runner    (1000)     1131 2023-03-23 09:55:50.888578 klldFN-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      670 2023-03-23 09:54:58.000000 klldFN-1.0.4/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-03-23 09:55:50.888578 klldFN-1.0.4/klldFN/
--rw-r--r--   0 runner    (1000) runner    (1000)    75238 2023-03-23 09:50:09.000000 klldFN-1.0.4/klldFN/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-03-23 09:55:50.888578 klldFN-1.0.4/klldFN.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1131 2023-03-23 09:55:50.000000 klldFN-1.0.4/klldFN.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      201 2023-03-23 09:55:50.000000 klldFN-1.0.4/klldFN.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-03-23 09:55:50.000000 klldFN-1.0.4/klldFN.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      127 2023-03-23 09:55:50.000000 klldFN-1.0.4/klldFN.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        7 2023-03-23 09:55:50.000000 klldFN-1.0.4/klldFN.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      393 2023-02-19 12:22:33.000000 klldFN-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-03-23 09:55:50.888578 klldFN-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      806 2023-03-13 17:03:15.000000 klldFN-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-23 18:57:45.027027 klldFN-1.0.5/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1131 2023-04-23 18:57:45.027027 klldFN-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      670 2023-03-23 09:54:58.000000 klldFN-1.0.5/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-23 18:57:45.015027 klldFN-1.0.5/klldFN/
+-rw-r--r--   0 runner    (1000) runner    (1000)    60569 2023-04-23 18:28:00.000000 klldFN-1.0.5/klldFN/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-23 18:57:45.027027 klldFN-1.0.5/klldFN.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1131 2023-04-23 18:57:44.000000 klldFN-1.0.5/klldFN.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      201 2023-04-23 18:57:44.000000 klldFN-1.0.5/klldFN.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-23 18:57:44.000000 klldFN-1.0.5/klldFN.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      127 2023-04-23 18:57:44.000000 klldFN-1.0.5/klldFN.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        7 2023-04-23 18:57:44.000000 klldFN-1.0.5/klldFN.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      393 2023-02-19 12:22:33.000000 klldFN-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-04-23 18:57:45.027027 klldFN-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      806 2023-04-23 18:28:13.000000 klldFN-1.0.5/setup.py
```

### Comparing `klldFN-1.0.4/PKG-INFO` & `klldFN-1.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klldFN
-Version: 1.0.4
+Version: 1.0.5
 Summary: klldFN
 Home-page: https://klld.42web.io
 Author: klld
 License: UNKNOWN
 Description: # klldFN
         Use This To Upload Files To klldFN
```

### Comparing `klldFN-1.0.4/README.md` & `klldFN-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `klldFN-1.0.4/klldFN.egg-info/PKG-INFO` & `klldFN-1.0.5/klldFN.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klldFN
-Version: 1.0.4
+Version: 1.0.5
 Summary: klldFN
 Home-page: https://klld.42web.io
 Author: klld
 License: UNKNOWN
 Description: # klldFN
         Use This To Upload Files To klldFN
```

### Comparing `klldFN-1.0.4/setup.py` & `klldFN-1.0.5/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name="klldFN",
-    version="1.0.4",
+    version="1.0.5",
     author="klld",
     description="klldFN",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://klld.42web.io",
     packages=setuptools.find_packages(),
     classifiers=[
```

