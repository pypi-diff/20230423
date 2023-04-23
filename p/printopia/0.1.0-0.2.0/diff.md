# Comparing `tmp/printopia-0.1.0.tar.gz` & `tmp/printopia-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "printopia-0.1.0.tar", max compression
+gzip compressed data, was "printopia-0.2.0.tar", max compression
```

## Comparing `printopia-0.1.0.tar` & `printopia-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      443 2023-04-23 13:41:09.885544 printopia-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1555 2023-04-21 18:12:12.063824 printopia-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-04-23 13:37:52.857957 printopia-0.1.0/src/printopia/__init__.py
--rw-r--r--   0        0        0     4008 2023-04-21 13:38:43.419184 printopia-0.1.0/src/printopia/printopia.py
--rw-r--r--   0        0        0     1996 1970-01-01 00:00:00.000000 printopia-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      488 2023-04-23 20:35:13.946210 printopia-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1555 2023-04-21 18:12:12.063824 printopia-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-23 13:37:52.857957 printopia-0.2.0/src/printopia/__init__.py
+-rw-r--r--   0        0        0     4008 2023-04-21 13:38:43.419184 printopia-0.2.0/src/printopia/printopia.py
+-rw-r--r--   0        0        0     1831 1970-01-01 00:00:00.000000 printopia-0.2.0/PKG-INFO
```

### Comparing `printopia-0.1.0/README.md` & `printopia-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `printopia-0.1.0/src/printopia/printopia.py` & `printopia-0.2.0/src/printopia/printopia.py`

 * *Files identical despite different names*

### Comparing `printopia-0.1.0/PKG-INFO` & `printopia-0.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 Metadata-Version: 2.1
 Name: printopia
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 Author: akshat
 Author-email: akshat1997tamrakar@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
-Requires-Dist: pytest (>=7.3.1,<8.0.0)
-Requires-Dist: pytest-cov (>=4.0.0,<5.0.0)
-Requires-Dist: pytest-sugar (>=0.9.7,<0.10.0)
-Requires-Dist: tox (>=4.4.12,<5.0.0)
 Description-Content-Type: text/markdown
 
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg?&style=for-the-badge&logo=python&logoColor=blue"></a>
 
 
 Introduction
 ------------------------------------------------
```

