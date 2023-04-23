# Comparing `tmp/enrRiceTrait-1.2.1.tar.gz` & `tmp/enrRiceTrait-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enrRiceTrait-1.2.1.tar", last modified: Sun Apr 23 14:57:49 2023, max compression
+gzip compressed data, was "enrRiceTrait-1.3.0.tar", last modified: Sun Apr 23 15:01:41 2023, max compression
```

## Comparing `enrRiceTrait-1.2.1.tar` & `enrRiceTrait-1.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 yao        (501) staff       (20)        0 2023-04-23 14:57:49.383813 enrRiceTrait-1.2.1/
--rw-rw-r--   0 yao        (501) staff       (20)       53 2021-03-29 13:55:50.000000 enrRiceTrait-1.2.1/MANIFEST.in
--rw-r--r--   0 yao        (501) staff       (20)      599 2023-04-23 14:57:49.383499 enrRiceTrait-1.2.1/PKG-INFO
--rw-rw-r--   0 yao        (501) staff       (20)       92 2020-07-13 13:31:42.000000 enrRiceTrait-1.2.1/README.md
-drwxr-xr-x   0 yao        (501) staff       (20)        0 2023-04-23 14:57:49.351439 enrRiceTrait-1.2.1/enrRiceTrait/
--rw-r--r--   0 yao        (501) staff       (20)    28228 2023-04-23 14:14:51.000000 enrRiceTrait-1.2.1/enrRiceTrait/Enrichment.py
--rw-rw-r--   0 yao        (501) staff       (20)      478 2021-03-29 14:59:32.000000 enrRiceTrait-1.2.1/enrRiceTrait/PTE_config.py
--rw-rw-r--   0 yao        (501) staff       (20)      222 2023-04-23 14:57:32.000000 enrRiceTrait-1.2.1/enrRiceTrait/__init__.py
-drwxr-xr-x   0 yao        (501) staff       (20)        0 2023-04-23 14:57:49.376342 enrRiceTrait-1.2.1/enrRiceTrait/data/
--rw-rw-r--   0 yao        (501) staff       (20)  9834834 2021-03-27 15:22:16.000000 enrRiceTrait-1.2.1/enrRiceTrait/data/Total_Association.txt
--rw-rw-r--   0 yao        (501) staff       (20)  1090456 2021-03-25 12:59:06.000000 enrRiceTrait-1.2.1/enrRiceTrait/data/to.wto.ro.funRiceGene.obo
-drwxr-xr-x   0 yao        (501) staff       (20)        0 2023-04-23 14:57:49.353908 enrRiceTrait-1.2.1/enrRiceTrait.egg-info/
--rw-rw-r--   0 yao        (501) staff       (20)      599 2023-04-23 14:57:49.000000 enrRiceTrait-1.2.1/enrRiceTrait.egg-info/PKG-INFO
--rw-rw-r--   0 yao        (501) staff       (20)      337 2023-04-23 14:57:49.000000 enrRiceTrait-1.2.1/enrRiceTrait.egg-info/SOURCES.txt
--rw-rw-r--   0 yao        (501) staff       (20)        1 2023-04-23 14:57:49.000000 enrRiceTrait-1.2.1/enrRiceTrait.egg-info/dependency_links.txt
--rw-rw-r--   0 yao        (501) staff       (20)       13 2023-04-23 14:57:49.000000 enrRiceTrait-1.2.1/enrRiceTrait.egg-info/top_level.txt
--rw-r--r--   0 yao        (501) staff       (20)       38 2023-04-23 14:57:49.384014 enrRiceTrait-1.2.1/setup.cfg
--rw-rw-r--   0 yao        (501) staff       (20)     1085 2023-04-23 14:57:32.000000 enrRiceTrait-1.2.1/setup.py
+drwxr-xr-x   0 yao        (501) staff       (20)        0 2023-04-23 15:01:41.224342 enrRiceTrait-1.3.0/
+-rw-rw-r--   0 yao        (501) staff       (20)       53 2021-03-29 13:55:50.000000 enrRiceTrait-1.3.0/MANIFEST.in
+-rw-r--r--   0 yao        (501) staff       (20)      599 2023-04-23 15:01:41.224070 enrRiceTrait-1.3.0/PKG-INFO
+-rw-rw-r--   0 yao        (501) staff       (20)       92 2020-07-13 13:31:42.000000 enrRiceTrait-1.3.0/README.md
+drwxr-xr-x   0 yao        (501) staff       (20)        0 2023-04-23 15:01:41.204536 enrRiceTrait-1.3.0/enrRiceTrait/
+-rw-r--r--   0 yao        (501) staff       (20)    28228 2023-04-23 14:14:51.000000 enrRiceTrait-1.3.0/enrRiceTrait/Enrichment.py
+-rw-rw-r--   0 yao        (501) staff       (20)      478 2021-03-29 14:59:32.000000 enrRiceTrait-1.3.0/enrRiceTrait/PTE_config.py
+-rw-rw-r--   0 yao        (501) staff       (20)      222 2023-04-23 15:01:01.000000 enrRiceTrait-1.3.0/enrRiceTrait/__init__.py
+drwxr-xr-x   0 yao        (501) staff       (20)        0 2023-04-23 15:01:41.217676 enrRiceTrait-1.3.0/enrRiceTrait/data/
+-rw-rw-r--   0 yao        (501) staff       (20)  9834834 2021-03-27 15:22:16.000000 enrRiceTrait-1.3.0/enrRiceTrait/data/Total_Association.txt
+-rw-rw-r--   0 yao        (501) staff       (20)  1090456 2021-03-25 12:59:06.000000 enrRiceTrait-1.3.0/enrRiceTrait/data/to.wto.ro.funRiceGene.obo
+drwxr-xr-x   0 yao        (501) staff       (20)        0 2023-04-23 15:01:41.205458 enrRiceTrait-1.3.0/enrRiceTrait.egg-info/
+-rw-rw-r--   0 yao        (501) staff       (20)      599 2023-04-23 15:01:41.000000 enrRiceTrait-1.3.0/enrRiceTrait.egg-info/PKG-INFO
+-rw-rw-r--   0 yao        (501) staff       (20)      337 2023-04-23 15:01:41.000000 enrRiceTrait-1.3.0/enrRiceTrait.egg-info/SOURCES.txt
+-rw-rw-r--   0 yao        (501) staff       (20)        1 2023-04-23 15:01:41.000000 enrRiceTrait-1.3.0/enrRiceTrait.egg-info/dependency_links.txt
+-rw-rw-r--   0 yao        (501) staff       (20)       13 2023-04-23 15:01:41.000000 enrRiceTrait-1.3.0/enrRiceTrait.egg-info/top_level.txt
+-rw-r--r--   0 yao        (501) staff       (20)       38 2023-04-23 15:01:41.224423 enrRiceTrait-1.3.0/setup.cfg
+-rw-rw-r--   0 yao        (501) staff       (20)     1085 2023-04-23 15:01:01.000000 enrRiceTrait-1.3.0/setup.py
```

### Comparing `enrRiceTrait-1.2.1/PKG-INFO` & `enrRiceTrait-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enrRiceTrait
-Version: 1.2.1
+Version: 1.3.0
 Summary: A python package for Rice Trait Enrichment.
 Home-page: https://github.com/YaoXinZhi/enrRiceTrait
 Author: xinzhi_yao
 Author-email: xinzhi_bioinfo@163.com
 License: UNKNOWN
 Description: # Plant Trait Enrichment Package  
         This is a python package for plant trait enrichment.
```

### Comparing `enrRiceTrait-1.2.1/enrRiceTrait/Enrichment.py` & `enrRiceTrait-1.3.0/enrRiceTrait/Enrichment.py`

 * *Files identical despite different names*

### Comparing `enrRiceTrait-1.2.1/enrRiceTrait/data/Total_Association.txt` & `enrRiceTrait-1.3.0/enrRiceTrait/data/Total_Association.txt`

 * *Files identical despite different names*

### Comparing `enrRiceTrait-1.2.1/enrRiceTrait/data/to.wto.ro.funRiceGene.obo` & `enrRiceTrait-1.3.0/enrRiceTrait/data/to.wto.ro.funRiceGene.obo`

 * *Files identical despite different names*

### Comparing `enrRiceTrait-1.2.1/enrRiceTrait.egg-info/PKG-INFO` & `enrRiceTrait-1.3.0/enrRiceTrait.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enrRiceTrait
-Version: 1.2.1
+Version: 1.3.0
 Summary: A python package for Rice Trait Enrichment.
 Home-page: https://github.com/YaoXinZhi/enrRiceTrait
 Author: xinzhi_yao
 Author-email: xinzhi_bioinfo@163.com
 License: UNKNOWN
 Description: # Plant Trait Enrichment Package  
         This is a python package for plant trait enrichment.
```

### Comparing `enrRiceTrait-1.2.1/setup.py` & `enrRiceTrait-1.3.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setup(
   name='enrRiceTrait',
-  version='1.2.1',
+  version='1.3.0',
   author='xinzhi_yao',
   author_email='xinzhi_bioinfo@163.com',
   description="A python package for Rice Trait Enrichment.",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/YaoXinZhi/enrRiceTrait",
```

