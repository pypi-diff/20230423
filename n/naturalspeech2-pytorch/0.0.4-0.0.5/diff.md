# Comparing `tmp/naturalspeech2-pytorch-0.0.4.tar.gz` & `tmp/naturalspeech2-pytorch-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naturalspeech2-pytorch-0.0.4.tar", last modified: Sun Apr 23 16:10:58 2023, max compression
+gzip compressed data, was "naturalspeech2-pytorch-0.0.5.tar", last modified: Sun Apr 23 16:12:28 2023, max compression
```

## Comparing `naturalspeech2-pytorch-0.0.4.tar` & `naturalspeech2-pytorch-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:10:58.682590 naturalspeech2-pytorch-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-23 16:10:47.000000 naturalspeech2-pytorch-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-23 16:10:58.682590 naturalspeech2-pytorch-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-23 16:10:47.000000 naturalspeech2-pytorch-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:10:58.682590 naturalspeech2-pytorch-0.0.4/naturalspeech2_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-23 16:10:47.000000 naturalspeech2-pytorch-0.0.4/naturalspeech2_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25501 2023-04-23 16:10:47.000000 naturalspeech2-pytorch-0.0.4/naturalspeech2_pytorch/naturalspeech2_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:10:58.682590 naturalspeech2-pytorch-0.0.4/naturalspeech2_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-23 16:10:58.000000 naturalspeech2-pytorch-0.0.4/naturalspeech2_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-23 16:10:58.000000 naturalspeech2-pytorch-0.0.4/naturalspeech2_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 16:10:58.000000 naturalspeech2-pytorch-0.0.4/naturalspeech2_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-23 16:10:58.000000 naturalspeech2-pytorch-0.0.4/naturalspeech2_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-23 16:10:58.000000 naturalspeech2-pytorch-0.0.4/naturalspeech2_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 16:10:58.682590 naturalspeech2-pytorch-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-23 16:10:47.000000 naturalspeech2-pytorch-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:12:28.535666 naturalspeech2-pytorch-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-23 16:12:14.000000 naturalspeech2-pytorch-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-23 16:12:28.535666 naturalspeech2-pytorch-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-23 16:12:14.000000 naturalspeech2-pytorch-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:12:28.535666 naturalspeech2-pytorch-0.0.5/naturalspeech2_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-23 16:12:14.000000 naturalspeech2-pytorch-0.0.5/naturalspeech2_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25501 2023-04-23 16:12:14.000000 naturalspeech2-pytorch-0.0.5/naturalspeech2_pytorch/naturalspeech2_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:12:28.535666 naturalspeech2-pytorch-0.0.5/naturalspeech2_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-23 16:12:28.000000 naturalspeech2-pytorch-0.0.5/naturalspeech2_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-23 16:12:28.000000 naturalspeech2-pytorch-0.0.5/naturalspeech2_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 16:12:28.000000 naturalspeech2-pytorch-0.0.5/naturalspeech2_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-23 16:12:28.000000 naturalspeech2-pytorch-0.0.5/naturalspeech2_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-23 16:12:28.000000 naturalspeech2-pytorch-0.0.5/naturalspeech2_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 16:12:28.535666 naturalspeech2-pytorch-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-23 16:12:14.000000 naturalspeech2-pytorch-0.0.5/setup.py
```

### Comparing `naturalspeech2-pytorch-0.0.4/LICENSE` & `naturalspeech2-pytorch-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `naturalspeech2-pytorch-0.0.4/PKG-INFO` & `naturalspeech2-pytorch-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naturalspeech2-pytorch
-Version: 0.0.4
+Version: 0.0.5
 Summary: Natural Speech 2 - Pytorch
 Home-page: https://github.com/lucidrains/naturalspeech2-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,latent diffusion,speech synthesis
 Classifier: Development Status :: 4 - Beta
```

### Comparing `naturalspeech2-pytorch-0.0.4/README.md` & `naturalspeech2-pytorch-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `naturalspeech2-pytorch-0.0.4/naturalspeech2_pytorch/naturalspeech2_pytorch.py` & `naturalspeech2-pytorch-0.0.5/naturalspeech2_pytorch/naturalspeech2_pytorch.py`

 * *Files identical despite different names*

### Comparing `naturalspeech2-pytorch-0.0.4/naturalspeech2_pytorch.egg-info/PKG-INFO` & `naturalspeech2-pytorch-0.0.5/naturalspeech2_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naturalspeech2-pytorch
-Version: 0.0.4
+Version: 0.0.5
 Summary: Natural Speech 2 - Pytorch
 Home-page: https://github.com/lucidrains/naturalspeech2-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,latent diffusion,speech synthesis
 Classifier: Development Status :: 4 - Beta
```

### Comparing `naturalspeech2-pytorch-0.0.4/setup.py` & `naturalspeech2-pytorch-0.0.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'naturalspeech2-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.0.4',
+  version = '0.0.5',
   license='MIT',
   description = 'Natural Speech 2 - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/naturalspeech2-pytorch',
   keywords = [
@@ -16,15 +16,15 @@
     'latent diffusion',
     'speech synthesis'
   ],
   install_requires=[
     'accelerate',
     'audiolm-pytorch>=0.27.2',
     'beartype',
-    'einops>=0.4',
+    'einops>=0.6.1',
     'ema-pytorch',
     'torch>=1.6',
     'tqdm',
     'vector-quantize-pytorch>=1.1.6'
   ],
   classifiers=[
     'Development Status :: 4 - Beta',
```

