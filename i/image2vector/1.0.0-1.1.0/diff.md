# Comparing `tmp/image2vector-1.0.0.tar.gz` & `tmp/image2vector-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image2vector-1.0.0.tar", last modified: Sun Apr 23 09:44:01 2023, max compression
+gzip compressed data, was "image2vector-1.1.0.tar", last modified: Mon Apr 10 08:09:07 2023, max compression
```

## Comparing `image2vector-1.0.0.tar` & `image2vector-1.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 ponponon   (501) staff       (20)        0 2023-04-23 09:44:01.453237 image2vector-1.0.0/
--rw-r--r--   0 ponponon   (501) staff       (20)     6521 2023-04-23 09:44:01.453383 image2vector-1.0.0/PKG-INFO
--rw-r--r--   0 ponponon   (501) staff       (20)     5618 2023-04-23 09:41:41.000000 image2vector-1.0.0/README.md
-drwxr-xr-x   0 ponponon   (501) staff       (20)        0 2023-04-23 09:44:01.444576 image2vector-1.0.0/image2vector.egg-info/
--rw-r--r--   0 ponponon   (501) staff       (20)     6521 2023-04-23 09:44:01.000000 image2vector-1.0.0/image2vector.egg-info/PKG-INFO
--rw-r--r--   0 ponponon   (501) staff       (20)      537 2023-04-23 09:44:01.000000 image2vector-1.0.0/image2vector.egg-info/SOURCES.txt
--rw-r--r--   0 ponponon   (501) staff       (20)        1 2023-04-23 09:44:01.000000 image2vector-1.0.0/image2vector.egg-info/dependency_links.txt
--rw-r--r--   0 ponponon   (501) staff       (20)       13 2023-04-23 09:44:01.000000 image2vector-1.0.0/image2vector.egg-info/requires.txt
--rw-r--r--   0 ponponon   (501) staff       (20)        3 2023-04-23 09:44:01.000000 image2vector-1.0.0/image2vector.egg-info/top_level.txt
-drwxr-xr-x   0 ponponon   (501) staff       (20)        0 2023-04-23 09:44:01.446339 image2vector-1.0.0/iv/
--rw-r--r--   0 ponponon   (501) staff       (20)     7651 2023-04-23 09:43:50.000000 image2vector-1.0.0/iv/__init__.py
-drwxr-xr-x   0 ponponon   (501) staff       (20)        0 2023-04-23 09:44:01.446612 image2vector-1.0.0/iv/cirtorch/
--rwxr-xr-x   0 ponponon   (501) staff       (20)        0 2022-12-29 16:28:24.000000 image2vector-1.0.0/iv/cirtorch/__init__.py
-drwxr-xr-x   0 ponponon   (501) staff       (20)        0 2023-04-23 09:44:01.446870 image2vector-1.0.0/iv/cirtorch/datasets/
--rwxr-xr-x   0 ponponon   (501) staff       (20)        0 2022-12-29 16:28:24.000000 image2vector-1.0.0/iv/cirtorch/datasets/__init__.py
--rwxr-xr-x   0 ponponon   (501) staff       (20)     1192 2023-04-23 09:43:50.000000 image2vector-1.0.0/iv/cirtorch/datasets/genericdataset.py
-drwxr-xr-x   0 ponponon   (501) staff       (20)        0 2023-04-23 09:44:01.449648 image2vector-1.0.0/iv/cirtorch/layers/
--rwxr-xr-x   0 ponponon   (501) staff       (20)        0 2022-12-29 16:28:24.000000 image2vector-1.0.0/iv/cirtorch/layers/__init__.py
--rwxr-xr-x   0 ponponon   (501) staff       (20)     2226 2023-04-23 09:41:41.000000 image2vector-1.0.0/iv/cirtorch/layers/functional.py
--rwxr-xr-x   0 ponponon   (501) staff       (20)      350 2022-12-29 16:28:24.000000 image2vector-1.0.0/iv/cirtorch/layers/normalization.py
--rwxr-xr-x   0 ponponon   (501) staff       (20)     3097 2023-04-10 07:57:14.000000 image2vector-1.0.0/iv/cirtorch/layers/pooling.py
-drwxr-xr-x   0 ponponon   (501) staff       (20)        0 2023-04-23 09:44:01.451943 image2vector-1.0.0/iv/cirtorch/networks/
--rwxr-xr-x   0 ponponon   (501) staff       (20)        0 2022-12-29 16:28:24.000000 image2vector-1.0.0/iv/cirtorch/networks/__init__.py
--rwxr-xr-x   0 ponponon   (501) staff       (20)     1288 2023-04-23 09:41:41.000000 image2vector-1.0.0/iv/cirtorch/networks/imageretrievalnet.py
--rw-r--r--   0 ponponon   (501) staff       (20)      361 2023-04-23 09:43:50.000000 image2vector-1.0.0/iv/schemas.py
--rw-r--r--   0 ponponon   (501) staff       (20)       38 2023-04-23 09:44:01.453822 image2vector-1.0.0/setup.cfg
--rw-r--r--   0 ponponon   (501) staff       (20)     1291 2023-04-23 09:41:41.000000 image2vector-1.0.0/setup.py
+drwxr-xr-x   0 ponponon   (501) staff       (20)        0 2023-04-10 08:09:07.796498 image2vector-1.1.0/
+-rw-r--r--   0 ponponon   (501) staff       (20)     6521 2023-04-10 08:09:07.796599 image2vector-1.1.0/PKG-INFO
+-rw-r--r--   0 ponponon   (501) staff       (20)     5618 2023-04-10 07:57:14.000000 image2vector-1.1.0/README.md
+drwxr-xr-x   0 ponponon   (501) staff       (20)        0 2023-04-10 08:09:07.793427 image2vector-1.1.0/image2vector.egg-info/
+-rw-r--r--   0 ponponon   (501) staff       (20)     6521 2023-04-10 08:09:07.000000 image2vector-1.1.0/image2vector.egg-info/PKG-INFO
+-rw-r--r--   0 ponponon   (501) staff       (20)      537 2023-04-10 08:09:07.000000 image2vector-1.1.0/image2vector.egg-info/SOURCES.txt
+-rw-r--r--   0 ponponon   (501) staff       (20)        1 2023-04-10 08:09:07.000000 image2vector-1.1.0/image2vector.egg-info/dependency_links.txt
+-rw-r--r--   0 ponponon   (501) staff       (20)       13 2023-04-10 08:09:07.000000 image2vector-1.1.0/image2vector.egg-info/requires.txt
+-rw-r--r--   0 ponponon   (501) staff       (20)        3 2023-04-10 08:09:07.000000 image2vector-1.1.0/image2vector.egg-info/top_level.txt
+drwxr-xr-x   0 ponponon   (501) staff       (20)        0 2023-04-10 08:09:07.793692 image2vector-1.1.0/iv/
+-rw-r--r--   0 ponponon   (501) staff       (20)     7525 2023-04-10 08:05:05.000000 image2vector-1.1.0/iv/__init__.py
+drwxr-xr-x   0 ponponon   (501) staff       (20)        0 2023-04-10 08:09:07.794051 image2vector-1.1.0/iv/cirtorch/
+-rwxr-xr-x   0 ponponon   (501) staff       (20)        0 2022-12-29 16:28:24.000000 image2vector-1.1.0/iv/cirtorch/__init__.py
+drwxr-xr-x   0 ponponon   (501) staff       (20)        0 2023-04-10 08:09:07.794736 image2vector-1.1.0/iv/cirtorch/datasets/
+-rwxr-xr-x   0 ponponon   (501) staff       (20)        0 2022-12-29 16:28:24.000000 image2vector-1.1.0/iv/cirtorch/datasets/__init__.py
+-rwxr-xr-x   0 ponponon   (501) staff       (20)        0 2023-04-10 07:57:14.000000 image2vector-1.1.0/iv/cirtorch/datasets/genericdataset.py
+drwxr-xr-x   0 ponponon   (501) staff       (20)        0 2023-04-10 08:09:07.795643 image2vector-1.1.0/iv/cirtorch/layers/
+-rwxr-xr-x   0 ponponon   (501) staff       (20)        0 2022-12-29 16:28:24.000000 image2vector-1.1.0/iv/cirtorch/layers/__init__.py
+-rwxr-xr-x   0 ponponon   (501) staff       (20)     2226 2023-04-10 07:57:14.000000 image2vector-1.1.0/iv/cirtorch/layers/functional.py
+-rwxr-xr-x   0 ponponon   (501) staff       (20)      350 2022-12-29 16:28:24.000000 image2vector-1.1.0/iv/cirtorch/layers/normalization.py
+-rwxr-xr-x   0 ponponon   (501) staff       (20)     3097 2023-04-10 07:57:14.000000 image2vector-1.1.0/iv/cirtorch/layers/pooling.py
+drwxr-xr-x   0 ponponon   (501) staff       (20)        0 2023-04-10 08:09:07.796179 image2vector-1.1.0/iv/cirtorch/networks/
+-rwxr-xr-x   0 ponponon   (501) staff       (20)        0 2022-12-29 16:28:24.000000 image2vector-1.1.0/iv/cirtorch/networks/__init__.py
+-rwxr-xr-x   0 ponponon   (501) staff       (20)     1288 2023-04-10 07:57:14.000000 image2vector-1.1.0/iv/cirtorch/networks/imageretrievalnet.py
+-rw-r--r--   0 ponponon   (501) staff       (20)      474 2023-04-10 08:05:05.000000 image2vector-1.1.0/iv/schemas.py
+-rw-r--r--   0 ponponon   (501) staff       (20)       38 2023-04-10 08:09:07.796845 image2vector-1.1.0/setup.cfg
+-rw-r--r--   0 ponponon   (501) staff       (20)     1291 2023-04-10 07:57:14.000000 image2vector-1.1.0/setup.py
```

### Comparing `image2vector-1.0.0/PKG-INFO` & `image2vector-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image2vector
-Version: 1.0.0
+Version: 1.1.0
 Summary: Transforming images into 512-dimensional vectors by residual neural networks
 Home-page: https://github.com/ponponon/image2vector
 Author: ponponon
 Author-email: 1729303158@qq.com
 Maintainer: ponponon
 Maintainer-email: 1729303158@qq.com
 License: MIT License
```

### Comparing `image2vector-1.0.0/README.md` & `image2vector-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `image2vector-1.0.0/image2vector.egg-info/PKG-INFO` & `image2vector-1.1.0/image2vector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image2vector
-Version: 1.0.0
+Version: 1.1.0
 Summary: Transforming images into 512-dimensional vectors by residual neural networks
 Home-page: https://github.com/ponponon/image2vector
 Author: ponponon
 Author-email: 1729303158@qq.com
 Maintainer: ponponon
 Maintainer-email: 1729303158@qq.com
 License: MIT License
```

### Comparing `image2vector-1.0.0/image2vector.egg-info/SOURCES.txt` & `image2vector-1.1.0/image2vector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `image2vector-1.0.0/iv/__init__.py` & `image2vector-1.1.0/iv/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-from typing import List, Union
+from typing import List, Union, Optional, Callable
 from pathlib import Path
 from io import BytesIO
 import torch
 import numpy
 from PIL import Image
 from numpy import ndarray
 from torch import Tensor
 from torch import device as TorchDevice
 from torchvision import transforms
-from torchvision.transforms.functional import InterpolationMode
 from iv.cirtorch.networks.imageretrievalnet import ImageRetrievalNet
-from iv.schemas import Device, Runtime
+from iv.schemas import Device, Runtime, PilMode
 
 
-__version__ = '1.0.0'
+__version__ = '1.1.0'
 VERSION = __version__
 
 preprocess = transforms.Compose([
     transforms.Resize(224),
     transforms.CenterCrop(224),
     transforms.ToTensor(),
     transforms.Normalize(
@@ -95,119 +94,115 @@
             self.network = trt_ts_module
 
         else:
             raise Exception(f'Unsupported runtime: {self.runtime}')
 
     def images_to_vectors(self, images: Tensor) -> Tensor:
         if self.runtime == Runtime.PYTORCH.value:
+            import torch
             with torch.no_grad():
                 _img_tensor = images.to(self.device)
                 features = self.network(_img_tensor)
                 vectors = torch.transpose(features, 0, 1)
                 return vectors
         elif self.runtime == Runtime.ONNXRUNTIME.value:
             ort_inputs = {
                 self.network.get_inputs()[0].name:
                     images.cpu().numpy()
             }
             ort_outputs: list[numpy.ndarray] = self.network.run(
                 None, ort_inputs)
             _ort_output = ort_outputs[0]
             _ort_output: ndarray
-            _t = torch.from_numpy(_ort_output)
-            t = torch.transpose(_t, 0, 1)
+            t = _ort_output.transpose((1, 0))
             return t
 
         elif self.runtime == Runtime.PYTORCH_SCRIPT.value:
+            import torch
             with torch.no_grad():
                 _img_tensor = images.to(self.device)
                 features = self.network(_img_tensor)
                 vectors = torch.transpose(features, 0, 1)
                 return vectors
         elif self.runtime == Runtime.PYTORCH_TENSORRT.value:
+            import torch
             _img_tensor = images.to(self.device)
             features = self.network(_img_tensor)
             vectors = torch.transpose(features, 0, 1)
             return vectors
         else:
             raise Exception('not support runtime')
 
     def gen_vector(
         self,
         image: Union[Image.Image, ndarray, Path, str, bytes],
-        batch_size: int = 1,
-        num_workers: int = 0
+        convert_mode: Optional[PilMode] = None,
+        preprocess_func: Optional[Callable[[Image.Image], Image.Image]] = None
     ) -> List[float]:
         if isinstance(image, bytes):
             image_file_like = BytesIO(image)
-            image = Image.open(image_file_like).convert('RGB')
-
-        if isinstance(image, Image.Image):
-            image = image.convert('RGB')
-
-        if isinstance(image, Path) or isinstance(image, str):
-            image = Image.open(str(image)).convert('RGB')
-
-        if isinstance(image, ndarray):
-            image = Image.fromarray(image).convert('RGB')
-
-        assert isinstance(image, Image.Image)
+            image = Image.open(image_file_like)
+        elif isinstance(image, Image.Image):
+            pass
+        elif isinstance(image, Path) or isinstance(image, str):
+            image = Image.open(str(image))
+        elif isinstance(image, ndarray):
+            image = Image.fromarray(image)
+        else:
+            raise Exception(f'Unsupported type: {type(image)}')
+        if convert_mode:
+            image = image.convert(convert_mode.value)
 
         batch_size = 1
 
+        if preprocess_func:
+            image = preprocess_func(image)
+
         preprocessed_image: torch.Tensor = preprocess(image)
         unsqueezed_image = preprocessed_image.unsqueeze(0)
 
         _images = torch.cat([unsqueezed_image]*batch_size, dim=0)
 
         vectors = self.images_to_vectors(_images)
 
         return vectors.squeeze(0).tolist()
 
     def gen_vectors(
         self,
         images: List[Union[Image.Image, ndarray, Path, str, bytes]],
-        batch_size: int = 1,
-        num_workers: int = 0
+        convert_mode: Optional[PilMode] = None,
+        preprocess_func: Optional[Callable[[Image.Image], Image.Image]] = None
     ) -> List[List[float]]:
 
-        _images = []
+        _images: list[Image.Image] = []
 
         assert isinstance(images, List)
         assert len(images) > 0
 
         for index, image in enumerate(images):
             if isinstance(image, bytes):
                 image_file_like = BytesIO(image)
-                image = Image.open(image_file_like).convert('RGB')
-                # _images[index] = image
-                _images.append(image)
-                assert isinstance(image, Image.Image)
-
+                image = Image.open(image_file_like)
             elif isinstance(image, Image.Image):
-                if image.mode != 'RGB':
-                    image = image.convert('RGB')
-                # _images[index] = image
-                _images.append(image)
-                assert isinstance(image, Image.Image)
-
+                pass
             elif isinstance(image, Path) or isinstance(image, str):
-                image = Image.open(str(image)).convert('RGB')
-                # _images[index] = image
-                _images.append(image)
-                assert isinstance(image, Image.Image)
-
+                image = Image.open(str(image))
             elif isinstance(image, ndarray):
-                image = Image.fromarray(image).convert('RGB')
-                # _images[index] = image
-                _images.append(image)
-                assert isinstance(image, Image.Image)
+                image = Image.fromarray(image)
             else:
                 raise Exception(f'Unsupported type: {type(image)}')
 
+            if preprocess_func:
+                image = preprocess_func(image)
+
+            if convert_mode:
+                image = image.convert(convert_mode.value)
+            assert isinstance(image, Image.Image)
+            _images.append(image)
+
         assert isinstance(
             _images[0], Image.Image), f'images[0] type: {type(_images[0])}'
 
         for index, image in enumerate(_images):
             preprocessed_image: torch.Tensor = preprocess(image)
             unsqueezed_image = preprocessed_image.unsqueeze(0)
             _images[index] = unsqueezed_image
```

### Comparing `image2vector-1.0.0/iv/cirtorch/layers/functional.py` & `image2vector-1.1.0/iv/cirtorch/layers/functional.py`

 * *Files identical despite different names*

### Comparing `image2vector-1.0.0/iv/cirtorch/layers/pooling.py` & `image2vector-1.1.0/iv/cirtorch/layers/pooling.py`

 * *Files identical despite different names*

### Comparing `image2vector-1.0.0/iv/cirtorch/networks/imageretrievalnet.py` & `image2vector-1.1.0/iv/cirtorch/networks/imageretrievalnet.py`

 * *Files identical despite different names*

### Comparing `image2vector-1.0.0/setup.py` & `image2vector-1.1.0/setup.py`

 * *Files identical despite different names*

