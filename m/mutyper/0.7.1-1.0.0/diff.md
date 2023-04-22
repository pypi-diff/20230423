# Comparing `tmp/mutyper-0.7.1.tar.gz` & `tmp/mutyper-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mutyper-0.7.1.tar", last modified: Sun Feb 12 01:23:45 2023, max compression
+gzip compressed data, was "mutyper-1.0.0.tar", last modified: Sat Apr 22 21:31:57 2023, max compression
```

## Comparing `mutyper-0.7.1.tar` & `mutyper-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 01:23:45.803299 mutyper-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-02-12 01:23:33.000000 mutyper-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-02-12 01:23:33.000000 mutyper-0.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-02-12 01:23:45.803299 mutyper-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-02-12 01:23:33.000000 mutyper-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 01:23:45.803299 mutyper-0.7.1/mutyper/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-02-12 01:23:33.000000 mutyper-0.7.1/mutyper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-02-12 01:23:45.803299 mutyper-0.7.1/mutyper/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-02-12 01:23:33.000000 mutyper-0.7.1/mutyper/ancestor.py
--rw-r--r--   0 runner    (1001) docker     (123)    16742 2023-02-12 01:23:33.000000 mutyper-0.7.1/mutyper/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 01:23:45.803299 mutyper-0.7.1/mutyper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-02-12 01:23:45.000000 mutyper-0.7.1/mutyper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-02-12 01:23:45.000000 mutyper-0.7.1/mutyper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-12 01:23:45.000000 mutyper-0.7.1/mutyper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-02-12 01:23:45.000000 mutyper-0.7.1/mutyper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-02-12 01:23:45.000000 mutyper-0.7.1/mutyper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-12 01:23:45.000000 mutyper-0.7.1/mutyper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-02-12 01:23:45.803299 mutyper-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-02-12 01:23:33.000000 mutyper-0.7.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-02-12 01:23:33.000000 mutyper-0.7.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 21:31:57.172209 mutyper-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-22 21:31:47.000000 mutyper-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-22 21:31:47.000000 mutyper-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-22 21:31:57.172209 mutyper-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-22 21:31:47.000000 mutyper-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 21:31:57.176209 mutyper-1.0.0/mutyper/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-22 21:31:47.000000 mutyper-1.0.0/mutyper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-22 21:31:57.176209 mutyper-1.0.0/mutyper/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-04-22 21:31:47.000000 mutyper-1.0.0/mutyper/ancestor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16742 2023-04-22 21:31:47.000000 mutyper-1.0.0/mutyper/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 21:31:57.172209 mutyper-1.0.0/mutyper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-22 21:31:57.000000 mutyper-1.0.0/mutyper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-22 21:31:57.000000 mutyper-1.0.0/mutyper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 21:31:57.000000 mutyper-1.0.0/mutyper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-22 21:31:57.000000 mutyper-1.0.0/mutyper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-22 21:31:57.000000 mutyper-1.0.0/mutyper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-22 21:31:57.000000 mutyper-1.0.0/mutyper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-22 21:31:57.172209 mutyper-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-22 21:31:47.000000 mutyper-1.0.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-04-22 21:31:47.000000 mutyper-1.0.0/versioneer.py
```

### Comparing `mutyper-0.7.1/LICENSE` & `mutyper-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mutyper-0.7.1/PKG-INFO` & `mutyper-1.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mutyper
-Version: 0.7.1
+Version: 1.0.0
 Summary: ancestral k-mer mutation types for SNP data
 Home-page: https://github.com/harrispopgen/mutyper
 Author: William DeWitt
 Author-email: wsdewitt@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![](docs/_static/logo.png)
 
 A Python package and command line utility for annotating the local ancestral sequence context of biallelic SNPs
 
-[![build and test](https://github.com/harrispopgen/mutyper/actions/workflows/build-and-test.yml/badge.svg)](https://github.com/harrispopgen/mutyper/actions/workflows/build-and-test.yml)
+[![Build and test](https://github.com/harrispopgen/mutyper/actions/workflows/build-and-test.yml/badge.svg)](https://github.com/harrispopgen/mutyper/actions/workflows/build-and-test.yml)
 [![Docs build and deploy](https://github.com/harrispopgen/mutyper/actions/workflows/docs-build-and-deploy.yml/badge.svg)](https://github.com/harrispopgen/mutyper/actions/workflows/docs-build-and-deploy.yml)
 [![Python package](https://github.com/harrispopgen/mutyper/actions/workflows/python-publish.yml/badge.svg)](https://github.com/harrispopgen/mutyper/actions/workflows/python-publish.yml)
 [![status](https://joss.theoj.org/papers/db2fb9b0e9fa1b380ff75655796e7bf1/status.svg)](https://joss.theoj.org/papers/db2fb9b0e9fa1b380ff75655796e7bf1)
 
 #### See [documentation](https://harrispopgen.github.io/mutyper) for install and usage information.
 
 Pairs well with the package [`mushi`](https://github.com/harrispopgen/mushi), which performs mutation spectrum history inference.
```

### Comparing `mutyper-0.7.1/README.md` & `mutyper-1.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ![](docs/_static/logo.png)
 
 A Python package and command line utility for annotating the local ancestral sequence context of biallelic SNPs
 
-[![build and test](https://github.com/harrispopgen/mutyper/actions/workflows/build-and-test.yml/badge.svg)](https://github.com/harrispopgen/mutyper/actions/workflows/build-and-test.yml)
+[![Build and test](https://github.com/harrispopgen/mutyper/actions/workflows/build-and-test.yml/badge.svg)](https://github.com/harrispopgen/mutyper/actions/workflows/build-and-test.yml)
 [![Docs build and deploy](https://github.com/harrispopgen/mutyper/actions/workflows/docs-build-and-deploy.yml/badge.svg)](https://github.com/harrispopgen/mutyper/actions/workflows/docs-build-and-deploy.yml)
 [![Python package](https://github.com/harrispopgen/mutyper/actions/workflows/python-publish.yml/badge.svg)](https://github.com/harrispopgen/mutyper/actions/workflows/python-publish.yml)
 [![status](https://joss.theoj.org/papers/db2fb9b0e9fa1b380ff75655796e7bf1/status.svg)](https://joss.theoj.org/papers/db2fb9b0e9fa1b380ff75655796e7bf1)
 
 #### See [documentation](https://harrispopgen.github.io/mutyper) for install and usage information.
 
 Pairs well with the package [`mushi`](https://github.com/harrispopgen/mushi), which performs mutation spectrum history inference.
```

### Comparing `mutyper-0.7.1/mutyper/ancestor.py` & `mutyper-1.0.0/mutyper/ancestor.py`

 * *Files identical despite different names*

### Comparing `mutyper-0.7.1/mutyper/cli.py` & `mutyper-1.0.0/mutyper/cli.py`

 * *Files identical despite different names*

### Comparing `mutyper-0.7.1/mutyper.egg-info/PKG-INFO` & `mutyper-1.0.0/mutyper.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mutyper
-Version: 0.7.1
+Version: 1.0.0
 Summary: ancestral k-mer mutation types for SNP data
 Home-page: https://github.com/harrispopgen/mutyper
 Author: William DeWitt
 Author-email: wsdewitt@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![](docs/_static/logo.png)
 
 A Python package and command line utility for annotating the local ancestral sequence context of biallelic SNPs
 
-[![build and test](https://github.com/harrispopgen/mutyper/actions/workflows/build-and-test.yml/badge.svg)](https://github.com/harrispopgen/mutyper/actions/workflows/build-and-test.yml)
+[![Build and test](https://github.com/harrispopgen/mutyper/actions/workflows/build-and-test.yml/badge.svg)](https://github.com/harrispopgen/mutyper/actions/workflows/build-and-test.yml)
 [![Docs build and deploy](https://github.com/harrispopgen/mutyper/actions/workflows/docs-build-and-deploy.yml/badge.svg)](https://github.com/harrispopgen/mutyper/actions/workflows/docs-build-and-deploy.yml)
 [![Python package](https://github.com/harrispopgen/mutyper/actions/workflows/python-publish.yml/badge.svg)](https://github.com/harrispopgen/mutyper/actions/workflows/python-publish.yml)
 [![status](https://joss.theoj.org/papers/db2fb9b0e9fa1b380ff75655796e7bf1/status.svg)](https://joss.theoj.org/papers/db2fb9b0e9fa1b380ff75655796e7bf1)
 
 #### See [documentation](https://harrispopgen.github.io/mutyper) for install and usage information.
 
 Pairs well with the package [`mushi`](https://github.com/harrispopgen/mushi), which performs mutation spectrum history inference.
```

### Comparing `mutyper-0.7.1/setup.py` & `mutyper-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `mutyper-0.7.1/versioneer.py` & `mutyper-1.0.0/versioneer.py`

 * *Files identical despite different names*

