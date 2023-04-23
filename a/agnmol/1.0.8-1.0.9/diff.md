# Comparing `tmp/agnmol-1.0.8.tar.gz` & `tmp/agnmol-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agnmol-1.0.8.tar", last modified: Mon Apr 17 16:34:28 2023, max compression
+gzip compressed data, was "agnmol-1.0.9.tar", last modified: Mon Apr 17 16:39:13 2023, max compression
```

## Comparing `agnmol-1.0.8.tar` & `agnmol-1.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 16:34:28.490082 agnmol-1.0.8/
--rw-rw-rw-   0        0        0     1091 2023-04-15 15:33:58.000000 agnmol-1.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0     2298 2023-04-17 16:34:28.477081 agnmol-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1909 2023-04-17 16:34:05.000000 agnmol-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 16:34:28.448081 agnmol-1.0.8/agnmol/
--rw-rw-rw-   0        0        0        0 2023-04-15 14:55:12.000000 agnmol-1.0.8/agnmol/__init__.py
--rw-rw-rw-   0        0        0      916 2023-04-17 16:10:44.000000 agnmol-1.0.8/agnmol/motion.py
-drwxrwxrwx   0        0        0        0 2023-04-17 16:34:28.475084 agnmol-1.0.8/agnmol.egg-info/
--rw-rw-rw-   0        0        0     2298 2023-04-17 16:34:28.000000 agnmol-1.0.8/agnmol.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-04-17 16:34:28.000000 agnmol-1.0.8/agnmol.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 16:34:28.000000 agnmol-1.0.8/agnmol.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-17 16:34:28.000000 agnmol-1.0.8/agnmol.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      461 2023-04-17 16:34:08.000000 agnmol-1.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-17 16:34:28.491079 agnmol-1.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-17 16:39:13.342443 agnmol-1.0.9/
+-rw-rw-rw-   0        0        0     1080 2023-04-17 16:38:53.000000 agnmol-1.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     2298 2023-04-17 16:39:13.339444 agnmol-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1909 2023-04-17 16:34:05.000000 agnmol-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 16:39:13.323445 agnmol-1.0.9/agnmol/
+-rw-rw-rw-   0        0        0        0 2023-04-15 14:55:12.000000 agnmol-1.0.9/agnmol/__init__.py
+-rw-rw-rw-   0        0        0      916 2023-04-17 16:10:44.000000 agnmol-1.0.9/agnmol/motion.py
+drwxrwxrwx   0        0        0        0 2023-04-17 16:39:13.338444 agnmol-1.0.9/agnmol.egg-info/
+-rw-rw-rw-   0        0        0     2298 2023-04-17 16:39:13.000000 agnmol-1.0.9/agnmol.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-04-17 16:39:13.000000 agnmol-1.0.9/agnmol.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 16:39:13.000000 agnmol-1.0.9/agnmol.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-17 16:39:13.000000 agnmol-1.0.9/agnmol.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      461 2023-04-17 16:38:53.000000 agnmol-1.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-17 16:39:13.342443 agnmol-1.0.9/setup.cfg
```

### Comparing `agnmol-1.0.8/LICENSE.txt` & `agnmol-1.0.9/LICENSE.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2018 The Python Packaging Authority
+Copyright (c) 2023 Agnė Moleikaitytė
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `agnmol-1.0.8/PKG-INFO` & `agnmol-1.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agnmol
-Version: 1.0.8
+Version: 1.0.9
 Summary: A package for physics motion calculations
 Author-email: agnmol <agnmol@ktu.lt>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `agnmol-1.0.8/README.md` & `agnmol-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `agnmol-1.0.8/agnmol/motion.py` & `agnmol-1.0.9/agnmol/motion.py`

 * *Files identical despite different names*

### Comparing `agnmol-1.0.8/agnmol.egg-info/PKG-INFO` & `agnmol-1.0.9/agnmol.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agnmol
-Version: 1.0.8
+Version: 1.0.9
 Summary: A package for physics motion calculations
 Author-email: agnmol <agnmol@ktu.lt>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

