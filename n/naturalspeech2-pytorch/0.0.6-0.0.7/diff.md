# Comparing `tmp/naturalspeech2-pytorch-0.0.6.tar.gz` & `tmp/naturalspeech2-pytorch-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naturalspeech2-pytorch-0.0.6.tar", last modified: Sun Apr 23 16:26:25 2023, max compression
+gzip compressed data, was "naturalspeech2-pytorch-0.0.7.tar", last modified: Sun Apr 23 16:27:14 2023, max compression
```

## Comparing `naturalspeech2-pytorch-0.0.6.tar` & `naturalspeech2-pytorch-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:26:25.059831 naturalspeech2-pytorch-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-23 16:26:13.000000 naturalspeech2-pytorch-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-23 16:26:25.059831 naturalspeech2-pytorch-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-23 16:26:13.000000 naturalspeech2-pytorch-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:26:25.055831 naturalspeech2-pytorch-0.0.6/naturalspeech2_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-23 16:26:13.000000 naturalspeech2-pytorch-0.0.6/naturalspeech2_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25834 2023-04-23 16:26:13.000000 naturalspeech2-pytorch-0.0.6/naturalspeech2_pytorch/naturalspeech2_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:26:25.059831 naturalspeech2-pytorch-0.0.6/naturalspeech2_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-23 16:26:25.000000 naturalspeech2-pytorch-0.0.6/naturalspeech2_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-23 16:26:25.000000 naturalspeech2-pytorch-0.0.6/naturalspeech2_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 16:26:25.000000 naturalspeech2-pytorch-0.0.6/naturalspeech2_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-23 16:26:25.000000 naturalspeech2-pytorch-0.0.6/naturalspeech2_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-23 16:26:25.000000 naturalspeech2-pytorch-0.0.6/naturalspeech2_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 16:26:25.059831 naturalspeech2-pytorch-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-23 16:26:13.000000 naturalspeech2-pytorch-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:27:14.259597 naturalspeech2-pytorch-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-23 16:27:00.000000 naturalspeech2-pytorch-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-23 16:27:14.259597 naturalspeech2-pytorch-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-23 16:27:00.000000 naturalspeech2-pytorch-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:27:14.259597 naturalspeech2-pytorch-0.0.7/naturalspeech2_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-23 16:27:00.000000 naturalspeech2-pytorch-0.0.7/naturalspeech2_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-04-23 16:27:00.000000 naturalspeech2-pytorch-0.0.7/naturalspeech2_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25834 2023-04-23 16:27:00.000000 naturalspeech2-pytorch-0.0.7/naturalspeech2_pytorch/naturalspeech2_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:27:14.259597 naturalspeech2-pytorch-0.0.7/naturalspeech2_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-23 16:27:14.000000 naturalspeech2-pytorch-0.0.7/naturalspeech2_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-23 16:27:14.000000 naturalspeech2-pytorch-0.0.7/naturalspeech2_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 16:27:14.000000 naturalspeech2-pytorch-0.0.7/naturalspeech2_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-23 16:27:14.000000 naturalspeech2-pytorch-0.0.7/naturalspeech2_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-23 16:27:14.000000 naturalspeech2-pytorch-0.0.7/naturalspeech2_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 16:27:14.259597 naturalspeech2-pytorch-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-23 16:27:00.000000 naturalspeech2-pytorch-0.0.7/setup.py
```

### Comparing `naturalspeech2-pytorch-0.0.6/LICENSE` & `naturalspeech2-pytorch-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `naturalspeech2-pytorch-0.0.6/PKG-INFO` & `naturalspeech2-pytorch-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naturalspeech2-pytorch
-Version: 0.0.6
+Version: 0.0.7
 Summary: Natural Speech 2 - Pytorch
 Home-page: https://github.com/lucidrains/naturalspeech2-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,latent diffusion,speech synthesis
 Classifier: Development Status :: 4 - Beta
```

### Comparing `naturalspeech2-pytorch-0.0.6/README.md` & `naturalspeech2-pytorch-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `naturalspeech2-pytorch-0.0.6/naturalspeech2_pytorch/naturalspeech2_pytorch.py` & `naturalspeech2-pytorch-0.0.7/naturalspeech2_pytorch/naturalspeech2_pytorch.py`

 * *Files identical despite different names*

### Comparing `naturalspeech2-pytorch-0.0.6/naturalspeech2_pytorch.egg-info/PKG-INFO` & `naturalspeech2-pytorch-0.0.7/naturalspeech2_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naturalspeech2-pytorch
-Version: 0.0.6
+Version: 0.0.7
 Summary: Natural Speech 2 - Pytorch
 Home-page: https://github.com/lucidrains/naturalspeech2-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,latent diffusion,speech synthesis
 Classifier: Development Status :: 4 - Beta
```

### Comparing `naturalspeech2-pytorch-0.0.6/setup.py` & `naturalspeech2-pytorch-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'naturalspeech2-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.0.6',
+  version = '0.0.7',
   license='MIT',
   description = 'Natural Speech 2 - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/naturalspeech2-pytorch',
   keywords = [
```

