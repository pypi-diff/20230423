# Comparing `tmp/vector_quantize_pytorch-1.2.1.tar.gz` & `tmp/vector_quantize_pytorch-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_quantize_pytorch-1.2.1.tar", last modified: Sat Apr 22 17:00:46 2023, max compression
+gzip compressed data, was "vector_quantize_pytorch-1.2.2.tar", last modified: Sun Apr 23 16:54:32 2023, max compression
```

## Comparing `vector_quantize_pytorch-1.2.1.tar` & `vector_quantize_pytorch-1.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:00:46.481400 vector_quantize_pytorch-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-22 17:00:32.000000 vector_quantize_pytorch-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-22 17:00:46.481400 vector_quantize_pytorch-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14067 2023-04-22 17:00:32.000000 vector_quantize_pytorch-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 17:00:46.481400 vector_quantize_pytorch-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-22 17:00:32.000000 vector_quantize_pytorch-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:00:46.481400 vector_quantize_pytorch-1.2.1/vector_quantize_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-22 17:00:32.000000 vector_quantize_pytorch-1.2.1/vector_quantize_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-22 17:00:32.000000 vector_quantize_pytorch-1.2.1/vector_quantize_pytorch/random_projection_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-04-22 17:00:32.000000 vector_quantize_pytorch-1.2.1/vector_quantize_pytorch/residual_vq.py
--rw-r--r--   0 runner    (1001) docker     (123)    22280 2023-04-22 17:00:32.000000 vector_quantize_pytorch-1.2.1/vector_quantize_pytorch/vector_quantize_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:00:46.481400 vector_quantize_pytorch-1.2.1/vector_quantize_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-22 17:00:46.000000 vector_quantize_pytorch-1.2.1/vector_quantize_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-22 17:00:46.000000 vector_quantize_pytorch-1.2.1/vector_quantize_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 17:00:46.000000 vector_quantize_pytorch-1.2.1/vector_quantize_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-22 17:00:46.000000 vector_quantize_pytorch-1.2.1/vector_quantize_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-22 17:00:46.000000 vector_quantize_pytorch-1.2.1/vector_quantize_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:54:32.642778 vector_quantize_pytorch-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-23 16:54:18.000000 vector_quantize_pytorch-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-23 16:54:32.642778 vector_quantize_pytorch-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14067 2023-04-23 16:54:18.000000 vector_quantize_pytorch-1.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 16:54:32.642778 vector_quantize_pytorch-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-23 16:54:18.000000 vector_quantize_pytorch-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:54:32.638778 vector_quantize_pytorch-1.2.2/vector_quantize_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-23 16:54:18.000000 vector_quantize_pytorch-1.2.2/vector_quantize_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-23 16:54:18.000000 vector_quantize_pytorch-1.2.2/vector_quantize_pytorch/random_projection_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-04-23 16:54:18.000000 vector_quantize_pytorch-1.2.2/vector_quantize_pytorch/residual_vq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22280 2023-04-23 16:54:18.000000 vector_quantize_pytorch-1.2.2/vector_quantize_pytorch/vector_quantize_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:54:32.638778 vector_quantize_pytorch-1.2.2/vector_quantize_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-23 16:54:32.000000 vector_quantize_pytorch-1.2.2/vector_quantize_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-23 16:54:32.000000 vector_quantize_pytorch-1.2.2/vector_quantize_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 16:54:32.000000 vector_quantize_pytorch-1.2.2/vector_quantize_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-23 16:54:32.000000 vector_quantize_pytorch-1.2.2/vector_quantize_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-23 16:54:32.000000 vector_quantize_pytorch-1.2.2/vector_quantize_pytorch.egg-info/top_level.txt
```

### Comparing `vector_quantize_pytorch-1.2.1/LICENSE` & `vector_quantize_pytorch-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.2.1/PKG-INFO` & `vector_quantize_pytorch-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_quantize_pytorch
-Version: 1.2.1
+Version: 1.2.2
 Summary: Vector Quantization - Pytorch
 Home-page: https://github.com/lucidrains/vector-quantizer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,pytorch,quantization
 Classifier: Development Status :: 4 - Beta
```

### Comparing `vector_quantize_pytorch-1.2.1/README.md` & `vector_quantize_pytorch-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.2.1/vector_quantize_pytorch/random_projection_quantizer.py` & `vector_quantize_pytorch-1.2.2/vector_quantize_pytorch/random_projection_quantizer.py`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.2.1/vector_quantize_pytorch/residual_vq.py` & `vector_quantize_pytorch-1.2.2/vector_quantize_pytorch/residual_vq.py`

 * *Files 5% similar despite different names*

```diff
@@ -112,15 +112,18 @@
         assert not (self.accept_image_fmap and exists(indices))
 
         quantized_out = 0.
         residual = x
 
         all_losses = []
         all_indices = []
-        ce_losses = []   # for cross entropy losses across quantizers, if indices are passed in
+
+        if return_loss:
+            assert not torch.any(indices == -1), 'some of the residual vq indices were dropped out. please use indices derived when the module is in eval mode to derive cross entropy loss'
+            ce_losses = []
 
         should_quantize_dropout = self.training and self.quantize_dropout and not return_loss
 
         # sample a layer index at which to dropout further residual quantization
         # also prepare null indices and loss
 
         if should_quantize_dropout:
```

### Comparing `vector_quantize_pytorch-1.2.1/vector_quantize_pytorch/vector_quantize_pytorch.py` & `vector_quantize_pytorch-1.2.2/vector_quantize_pytorch/vector_quantize_pytorch.py`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.2.1/vector_quantize_pytorch.egg-info/PKG-INFO` & `vector_quantize_pytorch-1.2.2/vector_quantize_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-quantize-pytorch
-Version: 1.2.1
+Version: 1.2.2
 Summary: Vector Quantization - Pytorch
 Home-page: https://github.com/lucidrains/vector-quantizer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,pytorch,quantization
 Classifier: Development Status :: 4 - Beta
```

