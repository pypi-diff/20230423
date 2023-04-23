# Comparing `tmp/spccpkg-0.0.3.tar.gz` & `tmp/spccpkg-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spccpkg-0.0.3.tar", last modified: Sun Apr 23 10:31:13 2023, max compression
+gzip compressed data, was "spccpkg-0.0.4.tar", last modified: Sun Apr 23 17:48:43 2023, max compression
```

## Comparing `spccpkg-0.0.3.tar` & `spccpkg-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 10:31:13.829591 spccpkg-0.0.3/
--rw-rw-rw-   0        0        0      451 2023-04-23 10:31:13.829591 spccpkg-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-23 10:31:13.830593 spccpkg-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      698 2023-04-23 10:30:14.000000 spccpkg-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-23 10:31:13.814886 spccpkg-0.0.3/spcc/
--rw-rw-rw-   0        0        0       29 2023-04-23 10:20:37.000000 spccpkg-0.0.3/spcc/__init__.py
--rw-rw-rw-   0        0        0     5236 2023-04-23 10:29:39.000000 spccpkg-0.0.3/spcc/code.py
-drwxrwxrwx   0        0        0        0 2023-04-23 10:31:13.827594 spccpkg-0.0.3/spccpkg.egg-info/
--rw-rw-rw-   0        0        0      451 2023-04-23 10:31:13.000000 spccpkg-0.0.3/spccpkg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      162 2023-04-23 10:31:13.000000 spccpkg-0.0.3/spccpkg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 10:31:13.000000 spccpkg-0.0.3/spccpkg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-04-23 10:31:13.000000 spccpkg-0.0.3/spccpkg.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 17:48:43.175546 spccpkg-0.0.4/
+-rw-rw-rw-   0        0        0      451 2023-04-23 17:48:43.174546 spccpkg-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-23 17:48:43.175546 spccpkg-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      698 2023-04-23 17:48:15.000000 spccpkg-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 17:48:43.151545 spccpkg-0.0.4/spcc/
+-rw-rw-rw-   0        0        0       29 2023-04-23 10:20:37.000000 spccpkg-0.0.4/spcc/__init__.py
+-rw-rw-rw-   0        0        0    30490 2023-04-23 17:26:06.000000 spccpkg-0.0.4/spcc/code.py
+drwxrwxrwx   0        0        0        0 2023-04-23 17:48:43.172545 spccpkg-0.0.4/spccpkg.egg-info/
+-rw-rw-rw-   0        0        0      451 2023-04-23 17:48:42.000000 spccpkg-0.0.4/spccpkg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      162 2023-04-23 17:48:43.000000 spccpkg-0.0.4/spccpkg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 17:48:42.000000 spccpkg-0.0.4/spccpkg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-04-23 17:48:42.000000 spccpkg-0.0.4/spccpkg.egg-info/top_level.txt
```

### Comparing `spccpkg-0.0.3/setup.py` & `spccpkg-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'A basic hello package'
 
 # Setting up
 setup(
     name="spccpkg",
     version=VERSION,
     author="yashbrid03",
```

