# Comparing `tmp/spccpkg-0.0.5.tar.gz` & `tmp/spccpkg-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spccpkg-0.0.5.tar", last modified: Sun Apr 23 18:06:31 2023, max compression
+gzip compressed data, was "spccpkg-0.0.6.tar", last modified: Sun Apr 23 18:21:36 2023, max compression
```

## Comparing `spccpkg-0.0.5.tar` & `spccpkg-0.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 18:06:31.523142 spccpkg-0.0.5/
--rw-rw-rw-   0        0        0      451 2023-04-23 18:06:31.522142 spccpkg-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-23 18:06:31.524156 spccpkg-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      698 2023-04-23 18:06:24.000000 spccpkg-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-23 18:06:31.505142 spccpkg-0.0.5/spcc/
--rw-rw-rw-   0        0        0       29 2023-04-23 10:20:37.000000 spccpkg-0.0.5/spcc/__init__.py
--rw-rw-rw-   0        0        0    30418 2023-04-23 17:57:30.000000 spccpkg-0.0.5/spcc/code.py
-drwxrwxrwx   0        0        0        0 2023-04-23 18:06:31.521143 spccpkg-0.0.5/spccpkg.egg-info/
--rw-rw-rw-   0        0        0      451 2023-04-23 18:06:31.000000 spccpkg-0.0.5/spccpkg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      162 2023-04-23 18:06:31.000000 spccpkg-0.0.5/spccpkg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 18:06:31.000000 spccpkg-0.0.5/spccpkg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-04-23 18:06:31.000000 spccpkg-0.0.5/spccpkg.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 18:21:36.818038 spccpkg-0.0.6/
+-rw-rw-rw-   0        0        0      451 2023-04-23 18:21:36.817037 spccpkg-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-23 18:21:36.819039 spccpkg-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      698 2023-04-23 18:21:33.000000 spccpkg-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 18:21:36.793040 spccpkg-0.0.6/spcc/
+-rw-rw-rw-   0        0        0       29 2023-04-23 10:20:37.000000 spccpkg-0.0.6/spcc/__init__.py
+-rw-rw-rw-   0        0        0    30456 2023-04-23 18:20:11.000000 spccpkg-0.0.6/spcc/code.py
+drwxrwxrwx   0        0        0        0 2023-04-23 18:21:36.816038 spccpkg-0.0.6/spccpkg.egg-info/
+-rw-rw-rw-   0        0        0      451 2023-04-23 18:21:36.000000 spccpkg-0.0.6/spccpkg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      162 2023-04-23 18:21:36.000000 spccpkg-0.0.6/spccpkg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 18:21:36.000000 spccpkg-0.0.6/spccpkg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-04-23 18:21:36.000000 spccpkg-0.0.6/spccpkg.egg-info/top_level.txt
```

### Comparing `spccpkg-0.0.5/setup.py` & `spccpkg-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 DESCRIPTION = 'A basic hello package'
 
 # Setting up
 setup(
     name="spccpkg",
     version=VERSION,
     author="yashbrid03",
```

### Comparing `spccpkg-0.0.5/spcc/code.py` & `spccpkg-0.0.6/spcc/code.py`

 * *Files 0% similar despite different names*

```diff
@@ -977,14 +977,16 @@
             yyparse();
             printf("Three Address Code:\n");
             threeAdd();
             printf("Four Address Code:\n");
             fouradd();
             printf("Triple Address Code:\n");
             triple();
+            return 0;
+            }
         '''
 
         print(string)
 
     def main():
         string = '''
         ICG()
```

