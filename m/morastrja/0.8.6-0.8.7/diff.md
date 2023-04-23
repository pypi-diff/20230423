# Comparing `tmp/morastrja-0.8.6.tar.gz` & `tmp/morastrja-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\morastrja-0.8.6.tar", last modified: Sun Apr 23 16:01:33 2023, max compression
+gzip compressed data, was "dist\morastrja-0.8.7.tar", last modified: Sun Apr 23 16:23:19 2023, max compression
```

## Comparing `morastrja-0.8.6.tar` & `morastrja-0.8.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 16:01:33.055795 morastrja-0.8.6/
--rw-rw-rw-   0        0        0      911 2023-04-23 16:01:33.054796 morastrja-0.8.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-23 16:01:33.002949 morastrja-0.8.6/ext/
--rw-rw-rw-   0        0        0   144565 2023-04-23 09:36:42.000000 morastrja-0.8.6/ext/cmorastr.c
--rw-rw-rw-   0        0        0     7449 2023-04-22 08:30:35.000000 morastrja-0.8.6/ext/cmorastr_bitap.h
--rw-rw-rw-   0        0        0     6123 2023-04-22 08:33:16.000000 morastrja-0.8.6/ext/cmorastr_pre.h
--rw-rw-rw-   0        0        0    13611 2023-04-22 08:35:20.000000 morastrja-0.8.6/ext/cmorastr_twoway.c
--rw-rw-rw-   0        0        0      958 2023-04-03 21:48:24.000000 morastrja-0.8.6/ext/cmorastr_twoway.h
-drwxrwxrwx   0        0        0        0 2023-04-23 16:01:33.021814 morastrja-0.8.6/morastrja/
--rw-rw-rw-   0        0        0      851 2023-04-21 04:23:48.000000 morastrja-0.8.6/morastrja/__init__.py
--rw-rw-rw-   0        0        0     6685 2023-04-21 04:24:12.000000 morastrja-0.8.6/morastrja/__init__.pyi
--rw-rw-rw-   0        0        0     1297 2023-04-21 00:44:26.000000 morastrja-0.8.6/morastrja/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 16:01:33.051797 morastrja-0.8.6/morastrja/data/
--rw-rw-rw-   0        0        0        0 2022-12-01 03:09:37.000000 morastrja-0.8.6/morastrja/data/__init__.py
--rw-rw-rw-   0        0        0     1407 2023-01-06 11:34:21.000000 morastrja-0.8.6/morastrja/data/table.bak
--rw-rw-rw-   0        0        0     1407 2023-01-17 12:13:16.000000 morastrja-0.8.6/morastrja/data/table.py
--rw-rw-rw-   0        0        0       54 2023-04-21 04:20:44.000000 morastrja-0.8.6/morastrja/utils.py
--rw-rw-rw-   0        0        0     1058 2023-04-21 04:19:11.000000 morastrja-0.8.6/morastrja/utils.pyi
-drwxrwxrwx   0        0        0        0 2023-04-23 16:01:33.039804 morastrja-0.8.6/morastrja.egg-info/
--rw-rw-rw-   0        0        0      911 2023-04-23 16:01:32.000000 morastrja-0.8.6/morastrja.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      421 2023-04-23 16:01:32.000000 morastrja-0.8.6/morastrja.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 16:01:32.000000 morastrja-0.8.6/morastrja.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-23 16:01:32.000000 morastrja-0.8.6/morastrja.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 16:01:33.055795 morastrja-0.8.6/setup.cfg
--rw-rw-rw-   0        0        0     1529 2023-04-23 16:01:14.000000 morastrja-0.8.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 16:23:19.024389 morastrja-0.8.7/
+-rw-rw-rw-   0        0        0      911 2023-04-23 16:23:19.022389 morastrja-0.8.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-23 16:23:18.963423 morastrja-0.8.7/ext/
+-rw-rw-rw-   0        0        0   144565 2023-04-23 09:36:42.000000 morastrja-0.8.7/ext/cmorastr.c
+-rw-rw-rw-   0        0        0     7449 2023-04-22 08:30:35.000000 morastrja-0.8.7/ext/cmorastr_bitap.h
+-rw-rw-rw-   0        0        0     6123 2023-04-22 08:33:16.000000 morastrja-0.8.7/ext/cmorastr_pre.h
+-rw-rw-rw-   0        0        0    13611 2023-04-22 08:35:20.000000 morastrja-0.8.7/ext/cmorastr_twoway.c
+-rw-rw-rw-   0        0        0      958 2023-04-03 21:48:24.000000 morastrja-0.8.7/ext/cmorastr_twoway.h
+drwxrwxrwx   0        0        0        0 2023-04-23 16:23:18.980414 morastrja-0.8.7/morastrja/
+-rw-rw-rw-   0        0        0      851 2023-04-21 04:23:48.000000 morastrja-0.8.7/morastrja/__init__.py
+-rw-rw-rw-   0        0        0     6685 2023-04-21 04:24:12.000000 morastrja-0.8.7/morastrja/__init__.pyi
+-rw-rw-rw-   0        0        0     1297 2023-04-21 00:44:26.000000 morastrja-0.8.7/morastrja/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 16:23:19.016395 morastrja-0.8.7/morastrja/data/
+-rw-rw-rw-   0        0        0        0 2022-12-01 03:09:37.000000 morastrja-0.8.7/morastrja/data/__init__.py
+-rw-rw-rw-   0        0        0     1407 2023-01-06 11:34:21.000000 morastrja-0.8.7/morastrja/data/table.bak
+-rw-rw-rw-   0        0        0     1407 2023-01-17 12:13:16.000000 morastrja-0.8.7/morastrja/data/table.py
+-rw-rw-rw-   0        0        0       54 2023-04-21 04:20:44.000000 morastrja-0.8.7/morastrja/utils.py
+-rw-rw-rw-   0        0        0     1058 2023-04-21 04:19:11.000000 morastrja-0.8.7/morastrja/utils.pyi
+drwxrwxrwx   0        0        0        0 2023-04-23 16:23:19.006399 morastrja-0.8.7/morastrja.egg-info/
+-rw-rw-rw-   0        0        0      911 2023-04-23 16:23:18.000000 morastrja-0.8.7/morastrja.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      421 2023-04-23 16:23:18.000000 morastrja-0.8.7/morastrja.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 16:23:18.000000 morastrja-0.8.7/morastrja.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-23 16:23:18.000000 morastrja-0.8.7/morastrja.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 16:23:19.025388 morastrja-0.8.7/setup.cfg
+-rw-rw-rw-   0        0        0     1532 2023-04-23 16:22:48.000000 morastrja-0.8.7/setup.py
```

### Comparing `morastrja-0.8.6/PKG-INFO` & `morastrja-0.8.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: morastrja
-Version: 0.8.6
+Version: 0.8.7
 Summary: Mora String for the Japanese Language
 Home-page: https://github.com/Hizuru3/morastrja
 Author: Hizuru
 License: MIT
 Description: 
         This module provides a class that counts morae, based on Japanese syllabaries.
```

### Comparing `morastrja-0.8.6/ext/cmorastr.c` & `morastrja-0.8.7/ext/cmorastr.c`

 * *Files identical despite different names*

### Comparing `morastrja-0.8.6/ext/cmorastr_bitap.h` & `morastrja-0.8.7/ext/cmorastr_bitap.h`

 * *Files identical despite different names*

### Comparing `morastrja-0.8.6/ext/cmorastr_pre.h` & `morastrja-0.8.7/ext/cmorastr_pre.h`

 * *Files identical despite different names*

### Comparing `morastrja-0.8.6/ext/cmorastr_twoway.c` & `morastrja-0.8.7/ext/cmorastr_twoway.c`

 * *Files identical despite different names*

### Comparing `morastrja-0.8.6/ext/cmorastr_twoway.h` & `morastrja-0.8.7/ext/cmorastr_twoway.h`

 * *Files identical despite different names*

### Comparing `morastrja-0.8.6/morastrja/__init__.py` & `morastrja-0.8.7/morastrja/__init__.py`

 * *Files identical despite different names*

### Comparing `morastrja-0.8.6/morastrja/__init__.pyi` & `morastrja-0.8.7/morastrja/__init__.pyi`

 * *Files identical despite different names*

### Comparing `morastrja-0.8.6/morastrja/__main__.py` & `morastrja-0.8.7/morastrja/__main__.py`

 * *Files identical despite different names*

### Comparing `morastrja-0.8.6/morastrja/data/table.bak` & `morastrja-0.8.7/morastrja/data/table.bak`

 * *Files identical despite different names*

### Comparing `morastrja-0.8.6/morastrja/data/table.py` & `morastrja-0.8.7/morastrja/data/table.py`

 * *Files identical despite different names*

### Comparing `morastrja-0.8.6/morastrja/utils.pyi` & `morastrja-0.8.7/morastrja/utils.pyi`

 * *Files identical despite different names*

### Comparing `morastrja-0.8.6/morastrja.egg-info/PKG-INFO` & `morastrja-0.8.7/morastrja.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: morastrja
-Version: 0.8.6
+Version: 0.8.7
 Summary: Mora String for the Japanese Language
 Home-page: https://github.com/Hizuru3/morastrja
 Author: Hizuru
 License: MIT
 Description: 
         This module provides a class that counts morae, based on Japanese syllabaries.
```

### Comparing `morastrja-0.8.6/setup.py` & `morastrja-0.8.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup, Extension
 
 
 ext = Extension('morastrja._morastr',
                 sources = ['ext/cmorastr.c'],
+                depends = ['*.h', 'cmorastr_twoway.c'],
                 extra_compile_args=['-O2'])
 
 setup (name = 'morastrja',
-       version = '0.8.6',
+       version = '0.8.7',
        description = 'Mora String for the Japanese Language',
        author = 'Hizuru',
        url = 'https://github.com/Hizuru3/morastrja',
        license = 'MIT',
        long_description = '''
 This module provides a class that counts morae, based on Japanese syllabaries.
 ''',
-       packages = ['morastrja', 'morastrja.data', 'ext'],
+       packages = ['morastrja', 'morastrja.data'],
        package_data = {'morastrja': ['__init__.pyi', 'utils.pyi'],
-                       'morastrja.data': ['table.bak'],
-                       'ext': ['*.c', '*.h']},
+                       'morastrja.data': ['table.bak']},
        ext_modules = [ext],
        classifiers = ['Intended Audience :: Science/Research',
                       'Intended Audience :: Developers',
                       'License :: OSI Approved :: MIT License',
                       'Natural Language :: Japanese',
                       'Programming Language :: Python :: 3.7',
                       'Programming Language :: Python :: 3.8',
```

