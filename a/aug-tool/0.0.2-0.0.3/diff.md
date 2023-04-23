# Comparing `tmp/aug-tool-0.0.2.tar.gz` & `tmp/aug-tool-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aug-tool-0.0.2.tar", last modified: Sun Apr 23 15:47:50 2023, max compression
+gzip compressed data, was "aug-tool-0.0.3.tar", last modified: Sun Apr 23 16:33:57 2023, max compression
```

## Comparing `aug-tool-0.0.2.tar` & `aug-tool-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 15:47:50.519628 aug-tool-0.0.2/
--rw-rw-rw-   0        0        0     1089 2023-04-14 20:14:24.000000 aug-tool-0.0.2/LICENCE
--rw-rw-rw-   0        0        0       20 2023-04-14 20:14:30.000000 aug-tool-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2725 2023-04-23 15:47:50.519628 aug-tool-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2059 2023-04-15 13:31:22.000000 aug-tool-0.0.2/README.md
--rw-rw-rw-   0        0        0      108 2023-04-14 20:14:26.000000 aug-tool-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      805 2023-04-23 15:47:50.521622 aug-tool-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-23 15:47:50.479320 aug-tool-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-23 15:47:50.511683 aug-tool-0.0.2/src/aug-tool/
--rw-rw-rw-   0        0        0     6540 2023-04-23 15:20:48.000000 aug-tool-0.0.2/src/aug-tool/Augmentation.py
--rw-rw-rw-   0        0        0        0 2023-04-14 18:48:21.000000 aug-tool-0.0.2/src/aug-tool/__init__.py
--rw-rw-rw-   0        0        0     3832 2023-04-23 15:46:09.000000 aug-tool-0.0.2/src/aug-tool/aug_tool.py
--rw-rw-rw-   0        0        0      617 2023-04-23 15:47:09.000000 aug-tool-0.0.2/src/aug-tool/deneme.py
-drwxrwxrwx   0        0        0        0 2023-04-23 15:47:50.518632 aug-tool-0.0.2/src/aug_tool.egg-info/
--rw-rw-rw-   0        0        0     2725 2023-04-23 15:47:50.000000 aug-tool-0.0.2/src/aug_tool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      300 2023-04-23 15:47:50.000000 aug-tool-0.0.2/src/aug_tool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 15:47:50.000000 aug-tool-0.0.2/src/aug_tool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-23 15:47:50.000000 aug-tool-0.0.2/src/aug_tool.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 16:33:57.699164 aug-tool-0.0.3/
+-rw-rw-rw-   0        0        0     1089 2023-04-14 20:14:24.000000 aug-tool-0.0.3/LICENCE
+-rw-rw-rw-   0        0        0       26 2023-04-23 16:29:48.000000 aug-tool-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2725 2023-04-23 16:33:57.700160 aug-tool-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2059 2023-04-15 13:31:22.000000 aug-tool-0.0.3/README.md
+-rw-rw-rw-   0        0        0      108 2023-04-14 20:14:26.000000 aug-tool-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      805 2023-04-23 16:33:57.701158 aug-tool-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-23 16:33:57.673072 aug-tool-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-23 16:33:57.692191 aug-tool-0.0.3/src/aug_tool/
+-rw-rw-rw-   0        0        0     6540 2023-04-23 15:20:48.000000 aug-tool-0.0.3/src/aug_tool/Augmentation.py
+-rw-rw-rw-   0        0        0        0 2023-04-14 18:48:21.000000 aug-tool-0.0.3/src/aug_tool/__init__.py
+-rw-rw-rw-   0        0        0     3832 2023-04-23 15:46:09.000000 aug-tool-0.0.3/src/aug_tool/aug_tool.py
+-rw-rw-rw-   0        0        0   142539 2023-01-17 19:52:24.000000 aug-tool-0.0.3/src/aug_tool/effect_1.png
+-rw-rw-rw-   0        0        0    62735 2023-01-17 19:56:01.000000 aug-tool-0.0.3/src/aug_tool/effect_2.png
+-rw-rw-rw-   0        0        0      617 2023-04-23 15:47:09.000000 aug-tool-0.0.3/src/aug_tool/example.py
+-rw-rw-rw-   0        0        0   182306 2023-02-05 15:48:52.000000 aug-tool-0.0.3/src/aug_tool/logo.png
+-rw-rw-rw-   0        0        0    20616 2023-04-15 10:14:20.000000 aug-tool-0.0.3/src/aug_tool/logo2.png
+drwxrwxrwx   0        0        0        0 2023-04-23 16:33:57.698171 aug-tool-0.0.3/src/aug_tool.egg-info/
+-rw-rw-rw-   0        0        0     2725 2023-04-23 16:33:57.000000 aug-tool-0.0.3/src/aug_tool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      398 2023-04-23 16:33:57.000000 aug-tool-0.0.3/src/aug_tool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 16:33:57.000000 aug-tool-0.0.3/src/aug_tool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-23 16:33:57.000000 aug-tool-0.0.3/src/aug_tool.egg-info/top_level.txt
```

### Comparing `aug-tool-0.0.2/LICENCE` & `aug-tool-0.0.3/LICENCE`

 * *Files identical despite different names*

### Comparing `aug-tool-0.0.2/PKG-INFO` & `aug-tool-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aug-tool
-Version: 0.0.2
+Version: 0.0.3
 Summary: Our library is now available on PyPI for easy installation and integration. Don t settle for limited training data - try our library today and take your ML projects to new heights!
 Home-page: https://github.com/hakanaktas1/aug-tool
 Author: Hakan Aktaş
 Author-email: hakanaktas4541@gmail.com
 Project-URL: Bug Tracker, https://github.com/hakanaktas1/aug-tool
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aug-tool-0.0.2/README.md` & `aug-tool-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `aug-tool-0.0.2/setup.cfg` & `aug-tool-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 7567 2d74 6f6f 6c0d 0a76 6572   = aug-tool..ver
-00000020: 7369 6f6e 203d 2030 2e30 2e32 0d0a 6175  sion = 0.0.2..au
+00000020: 7369 6f6e 203d 2030 2e30 2e33 0d0a 6175  sion = 0.0.3..au
 00000030: 7468 6f72 203d 2048 616b 616e 2041 6b74  thor = Hakan Akt
 00000040: 61c5 9f0d 0a61 7574 686f 725f 656d 6169  a....author_emai
 00000050: 6c20 3d20 6861 6b61 6e61 6b74 6173 3435  l = hakanaktas45
 00000060: 3431 4067 6d61 696c 2e63 6f6d 0d0a 6465  41@gmail.com..de
 00000070: 7363 7269 7074 696f 6e20 3d20 4f75 7220  scription = Our 
 00000080: 6c69 6272 6172 7920 6973 206e 6f77 2061  library is now a
 00000090: 7661 696c 6162 6c65 206f 6e20 5079 5049  vailable on PyPI
```

### Comparing `aug-tool-0.0.2/src/aug-tool/Augmentation.py` & `aug-tool-0.0.3/src/aug_tool/Augmentation.py`

 * *Files identical despite different names*

### Comparing `aug-tool-0.0.2/src/aug-tool/aug_tool.py` & `aug-tool-0.0.3/src/aug_tool/aug_tool.py`

 * *Files identical despite different names*

### Comparing `aug-tool-0.0.2/src/aug-tool/deneme.py` & `aug-tool-0.0.3/src/aug_tool/example.py`

 * *Files identical despite different names*

### Comparing `aug-tool-0.0.2/src/aug_tool.egg-info/PKG-INFO` & `aug-tool-0.0.3/src/aug_tool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aug-tool
-Version: 0.0.2
+Version: 0.0.3
 Summary: Our library is now available on PyPI for easy installation and integration. Don t settle for limited training data - try our library today and take your ML projects to new heights!
 Home-page: https://github.com/hakanaktas1/aug-tool
 Author: Hakan Aktaş
 Author-email: hakanaktas4541@gmail.com
 Project-URL: Bug Tracker, https://github.com/hakanaktas1/aug-tool
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

