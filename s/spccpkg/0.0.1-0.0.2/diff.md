# Comparing `tmp/spccpkg-0.0.1.tar.gz` & `tmp/spccpkg-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spccpkg-0.0.1.tar", last modified: Sun Apr 23 10:10:09 2023, max compression
+gzip compressed data, was "spccpkg-0.0.2.tar", last modified: Sun Apr 23 10:21:37 2023, max compression
```

## Comparing `spccpkg-0.0.1.tar` & `spccpkg-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 10:10:09.273008 spccpkg-0.0.1/
--rw-rw-rw-   0        0        0      451 2023-04-23 10:10:09.272008 spccpkg-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-23 10:10:09.273008 spccpkg-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      698 2023-04-23 10:08:45.000000 spccpkg-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-23 10:10:09.247010 spccpkg-0.0.1/spcc/
--rw-rw-rw-   0        0        0       24 2023-04-23 10:02:01.000000 spccpkg-0.0.1/spcc/__init__.py
--rw-rw-rw-   0        0        0       34 2023-04-23 10:01:04.000000 spccpkg-0.0.1/spcc/code.py
-drwxrwxrwx   0        0        0        0 2023-04-23 10:10:09.270023 spccpkg-0.0.1/spccpkg.egg-info/
--rw-rw-rw-   0        0        0      451 2023-04-23 10:10:08.000000 spccpkg-0.0.1/spccpkg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      162 2023-04-23 10:10:09.000000 spccpkg-0.0.1/spccpkg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 10:10:08.000000 spccpkg-0.0.1/spccpkg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-04-23 10:10:08.000000 spccpkg-0.0.1/spccpkg.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 10:21:37.463420 spccpkg-0.0.2/
+-rw-rw-rw-   0        0        0      451 2023-04-23 10:21:37.462399 spccpkg-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-23 10:21:37.463420 spccpkg-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      698 2023-04-23 10:21:33.000000 spccpkg-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 10:21:37.447399 spccpkg-0.0.2/spcc/
+-rw-rw-rw-   0        0        0       29 2023-04-23 10:20:37.000000 spccpkg-0.0.2/spcc/__init__.py
+-rw-rw-rw-   0        0        0       64 2023-04-23 10:20:17.000000 spccpkg-0.0.2/spcc/code.py
+drwxrwxrwx   0        0        0        0 2023-04-23 10:21:37.460401 spccpkg-0.0.2/spccpkg.egg-info/
+-rw-rw-rw-   0        0        0      451 2023-04-23 10:21:37.000000 spccpkg-0.0.2/spccpkg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      162 2023-04-23 10:21:37.000000 spccpkg-0.0.2/spccpkg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 10:21:37.000000 spccpkg-0.0.2/spccpkg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-04-23 10:21:37.000000 spccpkg-0.0.2/spccpkg.egg-info/top_level.txt
```

### Comparing `spccpkg-0.0.1/setup.py` & `spccpkg-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'A basic hello package'
 
 # Setting up
 setup(
     name="spccpkg",
     version=VERSION,
     author="yashbrid03",
```

