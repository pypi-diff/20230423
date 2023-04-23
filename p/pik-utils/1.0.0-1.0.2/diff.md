# Comparing `tmp/pik_utils-1.0.0.tar.gz` & `tmp/pik-utils-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pik_utils-1.0.0.tar", last modified: Fri Apr 21 13:16:40 2023, max compression
+gzip compressed data, was "pik-utils-1.0.2.tar", last modified: Sun Apr 23 12:57:13 2023, max compression
```

## Comparing `pik_utils-1.0.0.tar` & `pik-utils-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 13:16:40.191700 pik_utils-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      322 2023-04-21 13:16:40.191700 pik_utils-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 13:16:40.191700 pik_utils-1.0.0/pik_utils/
--rw-r--r--   0 root         (0) root         (0)       69 2023-04-21 13:16:39.000000 pik_utils-1.0.0/pik_utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 13:16:40.191700 pik_utils-1.0.0/pik_utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)      322 2023-04-21 13:16:40.000000 pik_utils-1.0.0/pik_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      162 2023-04-21 13:16:40.000000 pik_utils-1.0.0/pik_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 13:16:40.000000 pik_utils-1.0.0/pik_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-04-21 13:16:40.000000 pik_utils-1.0.0/pik_utils.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-21 13:16:40.191700 pik_utils-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      535 2023-04-21 13:16:39.000000 pik_utils-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 12:57:13.784638 pik-utils-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)      322 2023-04-23 12:57:13.784638 pik-utils-1.0.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 12:57:13.784638 pik-utils-1.0.2/pik-utils/
+-rw-r--r--   0 root         (0) root         (0)    82161 2023-04-23 12:57:13.000000 pik-utils-1.0.2/pik-utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 12:57:13.784638 pik-utils-1.0.2/pik_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      322 2023-04-23 12:57:13.000000 pik-utils-1.0.2/pik_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      162 2023-04-23 12:57:13.000000 pik-utils-1.0.2/pik_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 12:57:13.000000 pik-utils-1.0.2/pik_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-04-23 12:57:13.000000 pik-utils-1.0.2/pik_utils.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-23 12:57:13.784638 pik-utils-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      535 2023-04-23 12:57:12.000000 pik-utils-1.0.2/setup.py
```

### Comparing `pik_utils-1.0.0/setup.py` & `pik-utils-1.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.0.2'
 DESCRIPTION = "Utils ofr pik"
 LONG_DESCRIPTION = "Utils ofr pik"
 
 # Setting up
 setup(
-    name="pik_utils",
+    name="pik-utils",
     version=VERSION,
     author="GigaAlex",
     author_email="nick.faltermeier@gmx.de",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
```

