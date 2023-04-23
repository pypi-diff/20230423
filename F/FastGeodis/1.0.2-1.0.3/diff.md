# Comparing `tmp/FastGeodis-1.0.2.tar.gz` & `tmp/FastGeodis-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FastGeodis-1.0.2.tar", last modified: Thu Mar  2 12:09:20 2023, max compression
+gzip compressed data, was "FastGeodis-1.0.3.tar", last modified: Sun Apr 23 20:06:37 2023, max compression
```

## Comparing `FastGeodis-1.0.2.tar` & `FastGeodis-1.0.3.tar`

### file list

```diff
@@ -1,25 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-02 12:09:20.741642 FastGeodis-1.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-02 12:09:20.737642 FastGeodis-1.0.2/FastGeodis/
--rw-r--r--   0 runner    (1001) docker     (116)    24610 2023-03-02 12:07:36.000000 FastGeodis-1.0.2/FastGeodis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3927 2023-03-02 12:07:36.000000 FastGeodis-1.0.2/FastGeodis/common.h
--rwxr-xr-x   0 runner    (1001) docker     (116)    17203 2023-03-02 12:07:36.000000 FastGeodis-1.0.2/FastGeodis/fastgeodis.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     7345 2023-03-02 12:07:36.000000 FastGeodis-1.0.2/FastGeodis/fastgeodis.h
--rw-r--r--   0 runner    (1001) docker     (116)    13677 2023-03-02 12:07:36.000000 FastGeodis-1.0.2/FastGeodis/fastgeodis_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (116)    22686 2023-03-02 12:07:36.000000 FastGeodis-1.0.2/FastGeodis/fastgeodis_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (116)    16302 2023-03-02 12:07:36.000000 FastGeodis-1.0.2/FastGeodis/geodis_fastmarch.cpp
--rw-r--r--   0 runner    (1001) docker     (116)    11364 2023-03-02 12:07:36.000000 FastGeodis-1.0.2/FastGeodis/geodis_toivanen.cpp
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-02 12:09:20.741642 FastGeodis-1.0.2/FastGeodis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)    19647 2023-03-02 12:09:20.000000 FastGeodis-1.0.2/FastGeodis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      488 2023-03-02 12:09:20.000000 FastGeodis-1.0.2/FastGeodis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-02 12:09:20.000000 FastGeodis-1.0.2/FastGeodis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-02 12:09:20.000000 FastGeodis-1.0.2/FastGeodis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       13 2023-03-02 12:09:20.000000 FastGeodis-1.0.2/FastGeodis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       25 2023-03-02 12:09:20.000000 FastGeodis-1.0.2/FastGeodis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1540 2023-03-02 12:07:36.000000 FastGeodis-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      116 2023-03-02 12:07:36.000000 FastGeodis-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)    19647 2023-03-02 12:09:20.741642 FastGeodis-1.0.2/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (116)    17521 2023-03-02 12:07:36.000000 FastGeodis-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (116)      117 2023-03-02 12:07:36.000000 FastGeodis-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)       12 2023-03-02 12:07:36.000000 FastGeodis-1.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-03-02 12:09:20.741642 FastGeodis-1.0.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (116)     4553 2023-03-02 12:07:36.000000 FastGeodis-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 20:06:37.701039 FastGeodis-1.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 20:06:37.681038 FastGeodis-1.0.3/FastGeodis/
+-rw-r--r--   0 runner    (1001) docker     (122)    28532 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/FastGeodis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3927 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/FastGeodis/common.h
+-rwxr-xr-x   0 runner    (1001) docker     (122)    20550 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/FastGeodis/fastgeodis.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     8500 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/FastGeodis/fastgeodis.h
+-rw-r--r--   0 runner    (1001) docker     (122)    13677 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/FastGeodis/fastgeodis_cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    22686 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/FastGeodis/fastgeodis_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (122)    13293 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/FastGeodis/geodis_fastmarch.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    16506 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/FastGeodis/geodis_pixelqueue.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    11364 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/FastGeodis/geodis_toivanen.cpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 20:06:37.681038 FastGeodis-1.0.3/FastGeodis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    21675 2023-04-23 20:06:37.000000 FastGeodis-1.0.3/FastGeodis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1613 2023-04-23 20:06:37.000000 FastGeodis-1.0.3/FastGeodis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-23 20:06:37.000000 FastGeodis-1.0.3/FastGeodis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-23 20:06:37.000000 FastGeodis-1.0.3/FastGeodis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-04-23 20:06:37.000000 FastGeodis-1.0.3/FastGeodis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-23 20:06:37.000000 FastGeodis-1.0.3/FastGeodis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1540 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      148 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    21675 2023-04-23 20:06:37.701039 FastGeodis-1.0.3/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (122)    19445 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 20:06:37.673038 FastGeodis-1.0.3/dependency/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 20:06:37.681038 FastGeodis-1.0.3/dependency/fmm/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 20:06:37.673038 FastGeodis-1.0.3/dependency/fmm/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 20:06:37.685038 FastGeodis-1.0.3/dependency/fmm/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     1654 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/dependency/fmm/.github/workflows/cmake.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      397 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/dependency/fmm/.github/workflows/cpplint.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      289 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/dependency/fmm/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1941 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/dependency/fmm/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      206 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/dependency/fmm/CPPLINT.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)    21350 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/dependency/fmm/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 20:06:37.673038 FastGeodis-1.0.3/dependency/fmm/bindings/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 20:06:37.685038 FastGeodis-1.0.3/dependency/fmm/bindings/python/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/dependency/fmm/bindings/python/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     5796 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/dependency/fmm/bindings/python/py-fast-marching-method.cpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 20:06:37.673038 FastGeodis-1.0.3/dependency/fmm/examples/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 20:06:37.685038 FastGeodis-1.0.3/dependency/fmm/examples/cpp/
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/dependency/fmm/examples/cpp/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     4797 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/dependency/fmm/examples/cpp/minimal_example.cpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 20:06:37.685038 FastGeodis-1.0.3/dependency/fmm/examples/python/
+-rw-r--r--   0 runner    (1001) docker     (122)      738 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/dependency/fmm/examples/python/py-fast-marching-minimal-example.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 20:06:37.697039 FastGeodis-1.0.3/dependency/fmm/img/
+-rw-r--r--   0 runner    (1001) docker     (122)  1901907 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/dependency/fmm/img/fmm_readme.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)    23780 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/dependency/fmm/img/fmm_readme_concept.png
+-rw-r--r--   0 runner    (1001) docker     (122)    51743 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/dependency/fmm/img/fmm_readme_dilation_bands.png
+-rw-r--r--   0 runner    (1001) docker     (122)    25143 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/dependency/fmm/img/fmm_readme_eikonal_solvers.png
+-rw-r--r--   0 runner    (1001) docker     (122)    24417 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/dependency/fmm/img/fmm_readme_input_values.png
+-rw-r--r--   0 runner    (1001) docker     (122)    35239 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/dependency/fmm/img/fmm_readme_inside_outside.png
+-rw-r--r--   0 runner    (1001) docker     (122)    56744 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/dependency/fmm/img/fmm_readme_point_source_error.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 20:06:37.673038 FastGeodis-1.0.3/dependency/fmm/include/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 20:06:37.673038 FastGeodis-1.0.3/dependency/fmm/include/thinks/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 20:06:37.697039 FastGeodis-1.0.3/dependency/fmm/include/thinks/fast_marching_method/
+-rw-r--r--   0 runner    (1001) docker     (122)    81519 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/dependency/fmm/include/thinks/fast_marching_method/fast_marching_method.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 20:06:37.701039 FastGeodis-1.0.3/dependency/fmm/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1272 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/dependency/fmm/tests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    22357 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/dependency/fmm/tests/eikonal_solvers_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1238 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/dependency/fmm/tests/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2729 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/dependency/fmm/tests/py-bindings-test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33623 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/dependency/fmm/tests/signed_arrival_time_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    18622 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/dependency/fmm/tests/util.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-23 20:06:37.701039 FastGeodis-1.0.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4666 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/setup.py
```

### Comparing `FastGeodis-1.0.2/FastGeodis/__init__.py` & `FastGeodis-1.0.3/FastGeodis/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -304,151 +304,226 @@
     Returns:
         torch.Tensor with distance transform
     """
     return FastGeodisCpp.signed_generalised_geodesic3d_toivanen(
         image, softmask, spacing, v, lamb, 1 - lamb, iter
     )
 
-def generalised_geodesic2d_fastmarch(
+def geodesic2d_pixelqueue(
     image: torch.Tensor, 
-    softmask: torch.Tensor, 
-    v: float, 
+    seed: torch.Tensor, 
     lamb: float
 ):
-    r"""Computes Generalised Geodesic Distance using Fast Marching method from:
+    r"""Computes Geodesic Distance using Pixel Queue method from:
+    
+    Ikonen, L., & Toivanen, P. (2007). 
+    "Distance and nearest neighbor transforms on gray-level surfaces."
+    Pattern Recognition Letters, 28(5), 604-612.
+    
+    The function expects input as torch.Tensor, which can be run on CPU only using Tensor's device location
 
-    Sethian, James A. 
-    "Fast marching methods." 
-    SIAM review 41.2 (1999): 199-235.
+    Args:
+        image: input image, can be grayscale or multiple channels.
+        seed: seed in {0, 1} with seed information.
+        lamb: weighting factor between 0.0 and 1.0. 0.0 returns euclidean distance, whereas 1.0 returns geodesic distance
+
+    Returns:
+        torch.Tensor with distance transform
+    """
+    return FastGeodisCpp.geodesic2d_pixelqueue(
+        image, seed, lamb, 1 - lamb
+    )
+
+
+def geodesic3d_pixelqueue(
+    image: torch.Tensor,
+    seed: torch.Tensor,
+    spacing: List,
+    lamb: float
+):
+    r"""Computes Geodesic Distance using Pixel Queue method from:
     
-    For more details on generalised geodesic distance, check the following reference:
+    Ikonen, L., & Toivanen, P. (2007). 
+    "Distance and nearest neighbor transforms on gray-level surfaces."
+    Pattern Recognition Letters, 28(5), 604-612.
+    
+    The function expects input as torch.Tensor, which can be run on CPU only using Tensor's device location
 
-    Criminisi, Antonio, Toby Sharp, and Andrew Blake.
-    "Geos: Geodesic image segmentation."
-    European Conference on Computer Vision, Berlin, Heidelberg, 2008.
+    Args:
+        image: input image, can be grayscale or multiple channels.
+        seed: seed in {0, 1} with seed information.
+        spacing: spacing for 3D data
+        lamb: weighting factor between 0.0 and 1.0. 0.0 returns euclidean distance, whereas 1.0 returns geodesic distance
+
+    Returns:
+        torch.Tensor with distance transform
+    """
+    return FastGeodisCpp.geodesic3d_pixelqueue(
+        image, seed, spacing, lamb, 1 - lamb
+    )
 
+def signed_geodesic2d_pixelqueue(
+    image: torch.Tensor, 
+    seed: torch.Tensor, 
+    lamb: float
+):
+    r"""Computes Signed Generalised Geodesic Distance using Pixel Queue method from:
+    
+    Ikonen, L., & Toivanen, P. (2007). 
+    "Distance and nearest neighbor transforms on gray-level surfaces."
+    Pattern Recognition Letters, 28(5), 604-612.
+    
     The function expects input as torch.Tensor, which can be run on CPU only using Tensor's device location
 
     Args:
         image: input image, can be grayscale or multiple channels.
-        softmask: softmask in range [0, 1] with seed information.
-        v: weighting factor for establishing relationship between unary and spatial distances.
+        seed: seed in {0, 1} with seed information.
         lamb: weighting factor between 0.0 and 1.0. 0.0 returns euclidean distance, whereas 1.0 returns geodesic distance
 
     Returns:
         torch.Tensor with distance transform
     """
-    return FastGeodisCpp.generalised_geodesic2d_fastmarch(
-        image, softmask, v, lamb, 1 - lamb
+    return FastGeodisCpp.signed_geodesic2d_pixelqueue(
+        image, seed, lamb, 1 - lamb
     )
 
 
-def generalised_geodesic3d_fastmarch(
+def signed_geodesic3d_pixelqueue(
     image: torch.Tensor,
-    softmask: torch.Tensor,
+    seed: torch.Tensor,
     spacing: List,
-    v: float,
     lamb: float
 ):
-    r"""Computes Generalised Geodesic Distance using Fast Marching method from:
+    r"""Computes Signed Geodesic Distance using Pixel Queue method from:
+    
+    Ikonen, L., & Toivanen, P. (2007). 
+    "Distance and nearest neighbor transforms on gray-level surfaces."
+    Pattern Recognition Letters, 28(5), 604-612.
+    
+    The function expects input as torch.Tensor, which can be run on CPU only using Tensor's device location
 
-    TSethian, James A. 
+    Args:
+        image: input image, can be grayscale or multiple channels.
+        seed: seed in {0, 1} with seed information.
+        spacing: spacing for 3D data
+        lamb: weighting factor between 0.0 and 1.0. 0.0 returns euclidean distance, whereas 1.0 returns geodesic distance
+        iter: number of passes of the iterative distance transform method
+
+    Returns:
+        torch.Tensor with distance transform
+    """
+    return FastGeodisCpp.signed_geodesic3d_pixelqueue(
+        image, seed, spacing, lamb, 1 - lamb
+    )
+
+def geodesic2d_fastmarch(
+    image: torch.Tensor, 
+    seed: torch.Tensor, 
+    lamb: float
+):
+    r"""Computes Geodesic Distance using Fast Marching method from:
+
+    Sethian, James A. 
     "Fast marching methods." 
     SIAM review 41.2 (1999): 199-235.
     
-    For more details on generalised geodesic distance, check the following reference:
+    The function expects input as torch.Tensor, which can be run on CPU only using Tensor's device location
 
-    Criminisi, Antonio, Toby Sharp, and Andrew Blake.
-    "Geos: Geodesic image segmentation."
-    European Conference on Computer Vision, Berlin, Heidelberg, 2008.
+    Args:
+        image: input image, can be grayscale or multiple channels.
+        seed: seed in {0, 1} with seed information.
+        lamb: weighting factor between 0.0 and 1.0. 0.0 returns euclidean distance, whereas 1.0 returns geodesic distance
 
+    Returns:
+        torch.Tensor with distance transform
+    """
+    return FastGeodisCpp.geodesic2d_fastmarch(
+        image, seed, lamb, 1 - lamb
+    )
+
+
+def geodesic3d_fastmarch(
+    image: torch.Tensor,
+    seed: torch.Tensor,
+    spacing: List,
+    lamb: float
+):
+    r"""Computes Geodesic Distance using Fast Marching method from:
+
+    TSethian, James A. 
+    "Fast marching methods." 
+    SIAM review 41.2 (1999): 199-235.
+    
     The function expects input as torch.Tensor, which can be run on CPU only using Tensor's device location
 
     Args:
         image: input image, can be grayscale or multiple channels.
-        softmask: softmask in range [0, 1] with seed information.
+        seed: seed in {0, 1} with seed information.
         spacing: spacing for 3D data
-        v: weighting factor for establishing relationship between unary and spatial distances.
         lamb: weighting factor between 0.0 and 1.0. 0.0 returns euclidean distance, whereas 1.0 returns geodesic distance
 
     Returns:
         torch.Tensor with distance transform
     """
-    return FastGeodisCpp.generalised_geodesic3d_fastmarch(
-        image, softmask, spacing, v, lamb, 1 - lamb
+    return FastGeodisCpp.geodesic3d_fastmarch(
+        image, seed, spacing, lamb, 1 - lamb
     )
 
-def signed_generalised_geodesic2d_fastmarch(
+def signed_geodesic2d_fastmarch(
     image: torch.Tensor, 
-    softmask: torch.Tensor, 
-    v: float, 
+    seed: torch.Tensor, 
     lamb: float
 ):
-    r"""Computes Signed Generalised Geodesic Distance using Fast Marching method from:
+    r"""Computes Signed Geodesic Distance using Fast Marching method from:
 
     Sethian, James A. 
     "Fast marching methods." 
     SIAM review 41.2 (1999): 199-235.
     
-    For more details on generalised geodesic distance, check the following reference:
-
-    Criminisi, Antonio, Toby Sharp, and Andrew Blake.
-    "Geos: Geodesic image segmentation."
-    European Conference on Computer Vision, Berlin, Heidelberg, 2008.
-
     The function expects input as torch.Tensor, which can be run on CPU only using Tensor's device location
 
     Args:
         image: input image, can be grayscale or multiple channels.
-        softmask: softmask in range [0, 1] with seed information.
-        v: weighting factor for establishing relationship between unary and spatial distances.
+        seed: seed in {0, 1} with seed information.
         lamb: weighting factor between 0.0 and 1.0. 0.0 returns euclidean distance, whereas 1.0 returns geodesic distance
 
     Returns:
         torch.Tensor with distance transform
     """
-    return FastGeodisCpp.signed_generalised_geodesic2d_fastmarch(
-        image, softmask, v, lamb, 1 - lamb
+    return FastGeodisCpp.signed_geodesic2d_fastmarch(
+        image, seed, lamb, 1 - lamb
     )
 
 
-def signed_generalised_geodesic3d_fastmarch(
+def signed_geodesic3d_fastmarch(
     image: torch.Tensor,
-    softmask: torch.Tensor,
+    seed: torch.Tensor,
     spacing: List,
-    v: float,
     lamb: float
 ):
-    r"""Computes Signed Generalised Geodesic Distance using Fast Marching method from:
+    r"""Computes Signed Geodesic Distance using Fast Marching method from:
 
     Sethian, James A. 
     "Fast marching methods." 
     SIAM review 41.2 (1999): 199-235.
     
-    For more details on generalised geodesic distance, check the following reference:
-
-    Criminisi, Antonio, Toby Sharp, and Andrew Blake.
-    "Geos: Geodesic image segmentation."
-    European Conference on Computer Vision, Berlin, Heidelberg, 2008.
-
     The function expects input as torch.Tensor, which can be run on CPU only using Tensor's device location
 
     Args:
         image: input image, can be grayscale or multiple channels.
-        softmask: softmask in range [0, 1] with seed information.
+        seed: seed in {0, 1} with seed information.
         spacing: spacing for 3D data
-        v: weighting factor for establishing relationship between unary and spatial distances.
         lamb: weighting factor between 0.0 and 1.0. 0.0 returns euclidean distance, whereas 1.0 returns geodesic distance
         iter: number of passes of the iterative distance transform method
 
     Returns:
         torch.Tensor with distance transform
     """
-    return FastGeodisCpp.signed_generalised_geodesic3d_fastmarch(
-        image, softmask, spacing, v, lamb, 1 - lamb
+    return FastGeodisCpp.signed_geodesic3d_fastmarch(
+        image, seed, spacing, lamb, 1 - lamb
     )
 
 def GSF2d(
     image: torch.Tensor,
     softmask: torch.Tensor,
     theta: float,
     v: float,
@@ -575,19 +650,80 @@
         iter: number of passes of the iterative distance transform method
 
     Returns:
         torch.Tensor with distance transform
     """
     return FastGeodisCpp.GSF3d_toivanen(image, softmask, theta, spacing, v, lamb, iter)
 
+def GSF2d_pixelqueue(
+    image: torch.Tensor,
+    seed: torch.Tensor,
+    theta: float,
+    lamb: float
+):
+    r"""Computes Geodesic Symmetric Filtering (GSF) using Pixel Queue method from:
+
+    Ikonen, L., & Toivanen, P. (2007). 
+    "Distance and nearest neighbor transforms on gray-level surfaces."
+    Pattern Recognition Letters, 28(5), 604-612.
+
+    For more details on GSF, check the following reference:
+
+    Criminisi, Antonio, Toby Sharp, and Andrew Blake.
+    "Geos: Geodesic image segmentation."
+    European Conference on Computer Vision, Berlin, Heidelberg, 2008.
+
+    The function expects input as torch.Tensor, which can be run on CPU only using Tensor's device location
+
+    Args:
+        image: input image, can be grayscale or multiple channels.
+        seed: seed in {0, 1} with seed information.
+        lamb: weighting factor between 0.0 and 1.0. 0.0 returns euclidean distance, whereas 1.0 returns geodesic distance
+
+    Returns:
+        torch.Tensor with distance transform
+    """
+    return FastGeodisCpp.GSF2d_pixelqueue(image, seed, theta, lamb)
+
+def GSF3d_pixelqueue(
+    image: torch.Tensor,
+    seed: torch.Tensor,
+    theta: float,
+    spacing: List,
+    lamb: float,
+):
+    r"""Computes Geodesic Symmetric Filtering (GSF) using Pixel Queue method from:
+
+    Ikonen, L., & Toivanen, P. (2007). 
+    "Distance and nearest neighbor transforms on gray-level surfaces."
+    Pattern Recognition Letters, 28(5), 604-612.
+
+    For more details on GSF, check the following reference:
+
+    Criminisi, Antonio, Toby Sharp, and Andrew Blake.
+    "Geos: Geodesic image segmentation."
+    European Conference on Computer Vision, Berlin, Heidelberg, 2008.
+
+    The function expects input as torch.Tensor, which can be run on CPU only using Tensor's device location
+
+    Args:
+        image: input image, can be grayscale or multiple channels.
+        seed: seed in range {0, 1} with seed information.
+        spacing: spacing for 3D data
+        lamb: weighting factor between 0.0 and 1.0. 0.0 returns euclidean distance, whereas 1.0 returns geodesic distance
+
+    Returns:
+        torch.Tensor with distance transform
+    """
+    return FastGeodisCpp.GSF3d_pixelqueue(image, seed, theta, spacing, lamb)
+
 def GSF2d_fastmarch(
     image: torch.Tensor,
-    softmask: torch.Tensor,
+    seed: torch.Tensor,
     theta: float,
-    v: float,
     lamb: float
 ):
     r"""Computes Geodesic Symmetric Filtering (GSF) using Fast Marching method from:
 
     Sethian, James A. 
     "Fast marching methods." 
     SIAM review 41.2 (1999): 199-235.
@@ -598,30 +734,28 @@
     "Geos: Geodesic image segmentation."
     European Conference on Computer Vision, Berlin, Heidelberg, 2008.
 
     The function expects input as torch.Tensor, which can be run on CPU only using Tensor's device location
 
     Args:
         image: input image, can be grayscale or multiple channels.
-        softmask: softmask in range [0, 1] with seed information.
-        v: weighting factor for establishing relationship between unary and spatial distances.
+        seed: seed in {0, 1} with seed information.
         lamb: weighting factor between 0.0 and 1.0. 0.0 returns euclidean distance, whereas 1.0 returns geodesic distance
 
     Returns:
         torch.Tensor with distance transform
     """
-    return FastGeodisCpp.GSF2d_fastmarch(image, softmask, theta, v, lamb)
+    return FastGeodisCpp.GSF2d_fastmarch(image, seed, theta, lamb)
 
 
 def GSF3d_fastmarch(
     image: torch.Tensor,
-    softmask: torch.Tensor,
+    seed: torch.Tensor,
     theta: float,
     spacing: List,
-    v: float,
     lamb: float,
 ):
     r"""Computes Geodesic Symmetric Filtering (GSF) using Fast Marching method from:
 
     Sethian, James A. 
     "Fast marching methods." 
     SIAM review 41.2 (1999): 199-235.
@@ -632,16 +766,15 @@
     "Geos: Geodesic image segmentation."
     European Conference on Computer Vision, Berlin, Heidelberg, 2008.
 
     The function expects input as torch.Tensor, which can be run on CPU only using Tensor's device location
 
     Args:
         image: input image, can be grayscale or multiple channels.
-        softmask: softmask in range [0, 1] with seed information.
+        seed: seed in {0, 1} with seed information.
         spacing: spacing for 3D data
-        v: weighting factor for establishing relationship between unary and spatial distances.
         lamb: weighting factor between 0.0 and 1.0. 0.0 returns euclidean distance, whereas 1.0 returns geodesic distance
 
     Returns:
         torch.Tensor with distance transform
     """
-    return FastGeodisCpp.GSF3d_fastmarch(image, softmask, theta, spacing, v, lamb)
+    return FastGeodisCpp.GSF3d_fastmarch(image, seed, theta, spacing, lamb)
```

### Comparing `FastGeodis-1.0.2/FastGeodis/common.h` & `FastGeodis-1.0.3/FastGeodis/common.h`

 * *Files identical despite different names*

### Comparing `FastGeodis-1.0.2/FastGeodis/fastgeodis.cpp` & `FastGeodis-1.0.3/FastGeodis/fastgeodis.cpp`

 * *Files 16% similar despite different names*

```diff
@@ -172,43 +172,74 @@
         throw std::invalid_argument(
             "function only supports 3D spacing inputs, received " + std::to_string(spacing.size()));
     }
 
     return generalised_geodesic3d_toivanen_cpu(image, mask, spacing, v, l_grad, l_eucl, iterations);
 }
 
-torch::Tensor generalised_geodesic2d_fastmarch(const torch::Tensor &image, const torch::Tensor &mask, const float &v, const float &l_grad, const float &l_eucl)
+torch::Tensor geodesic2d_pixelqueue(const torch::Tensor &image, const torch::Tensor &mask, const float &l_grad, const float &l_eucl)
+{
+
+    // check input dimensions
+    check_input_dimensions(image, mask, 4);
+
+    // pixelqueue method is only implementable on cpu
+    check_cpu(image);    
+    check_cpu(mask);
+
+    return geodesic2d_pixelqueue_cpu(image, mask, l_grad, l_eucl);
+}
+
+torch::Tensor geodesic3d_pixelqueue(const torch::Tensor &image, const torch::Tensor &mask, const std::vector<float> &spacing, const float &l_grad, const float &l_eucl)
+{
+    // check input dimensions
+    check_input_dimensions(image, mask, 5);
+
+    // pixelqueue method is only implementable on cpu
+    check_cpu(image);    
+    check_cpu(mask);
+
+    if (spacing.size() != 3)
+    {
+        throw std::invalid_argument(
+            "function only supports 3D spacing inputs, received " + std::to_string(spacing.size()));
+    }
+
+    return geodesic3d_pixelqueue_cpu(image, mask, spacing, l_grad, l_eucl);
+}
+
+torch::Tensor geodesic2d_fastmarch(const torch::Tensor &image, const torch::Tensor &mask, const float &l_grad, const float &l_eucl)
 {
 
     // check input dimensions
     check_input_dimensions(image, mask, 4);
 
     // fastmarch method is only implementable on cpu
     check_cpu(image);    
     check_cpu(mask);
 
-    return generalised_geodesic2d_fastmarch_cpu(image, mask, v, l_grad, l_eucl);
+    return geodesic2d_fastmarch_cpu(image, mask, l_grad, l_eucl);
 }
 
-torch::Tensor generalised_geodesic3d_fastmarch(const torch::Tensor &image, const torch::Tensor &mask, const std::vector<float> &spacing, const float &v, const float &l_grad, const float &l_eucl)
+torch::Tensor geodesic3d_fastmarch(const torch::Tensor &image, const torch::Tensor &mask, const std::vector<float> &spacing, const float &l_grad, const float &l_eucl)
 {
     // check input dimensions
     check_input_dimensions(image, mask, 5);
 
     // fastmarch method is only implementable on cpu
     check_cpu(image);    
     check_cpu(mask);
 
     if (spacing.size() != 3)
     {
         throw std::invalid_argument(
             "function only supports 3D spacing inputs, received " + std::to_string(spacing.size()));
     }
 
-    return generalised_geodesic3d_fastmarch_cpu(image, mask, spacing, v, l_grad, l_eucl);
+    return geodesic3d_fastmarch_cpu(image, mask, spacing, l_grad, l_eucl);
 }
 
 torch::Tensor signed_generalised_geodesic2d(const torch::Tensor &image, const torch::Tensor &mask, const float &v, const float &l_grad, const float &l_eucl, const int &iterations)
 {
     auto secondcall = std::async(std::launch::async, generalised_geodesic2d, image, 1 - mask, v, l_grad, l_eucl, iterations);
     torch::Tensor D_M = generalised_geodesic2d(image, mask, v, l_grad, l_eucl, iterations);
     // torch::Tensor D_Mb = generalised_geodesic2d(image, 1 - mask, v, l_grad, l_eucl, iterations);
@@ -241,29 +272,49 @@
     torch::Tensor D_M = generalised_geodesic3d_toivanen(image, mask, spacing, v, l_grad, l_eucl, iterations);
     // torch::Tensor D_Mb = generalised_geodesic3d_toivanen(image, 1 - mask, spacing, v, l_grad, l_eucl, iterations);
     torch::Tensor D_Mb = secondcall.get();
     
     return D_M - D_Mb;
 }
 
-torch::Tensor signed_generalised_geodesic2d_fastmarch(const torch::Tensor &image, const torch::Tensor &mask, const float &v, const float &l_grad, const float &l_eucl)
+torch::Tensor signed_geodesic2d_pixelqueue(const torch::Tensor &image, const torch::Tensor &mask, const float &l_grad, const float &l_eucl)
 {
-    auto secondcall = std::async(std::launch::async, generalised_geodesic2d_fastmarch, image, 1 - mask, v, l_grad, l_eucl);
-    torch::Tensor D_M = generalised_geodesic2d_fastmarch(image, mask, v, l_grad, l_eucl);
-    // torch::Tensor D_Mb = generalised_geodesic2d_fastmarch(image, 1 - mask, v, l_grad, l_eucl);
+    auto secondcall = std::async(std::launch::async, geodesic2d_pixelqueue, image, 1 - mask, l_grad, l_eucl);
+    torch::Tensor D_M = geodesic2d_pixelqueue(image, mask, l_grad, l_eucl);
+    // torch::Tensor D_Mb = geodesic2d_pixelqueue(image, 1 - mask, l_grad, l_eucl);
     torch::Tensor D_Mb = secondcall.get();
 
     return D_M - D_Mb;
 }
 
-torch::Tensor signed_generalised_geodesic3d_fastmarch(const torch::Tensor &image, const torch::Tensor &mask, const std::vector<float> &spacing, const float &v, const float &l_grad, const float &l_eucl)
+torch::Tensor signed_geodesic3d_pixelqueue(const torch::Tensor &image, const torch::Tensor &mask, const std::vector<float> &spacing, const float &l_grad, const float &l_eucl)
 {
-    auto secondcall = std::async(std::launch::async, generalised_geodesic3d_fastmarch, image, 1 - mask, spacing, v, l_grad, l_eucl);
-    torch::Tensor D_M = generalised_geodesic3d_fastmarch(image, mask, spacing, v, l_grad, l_eucl);
-    // torch::Tensor D_Mb = generalised_geodesic3d_fastmarch(image, 1 - mask, spacing, v, l_grad, l_eucl);
+    auto secondcall = std::async(std::launch::async, geodesic3d_pixelqueue, image, 1 - mask, spacing, l_grad, l_eucl);
+    torch::Tensor D_M = geodesic3d_pixelqueue(image, mask, spacing, l_grad, l_eucl);
+    // torch::Tensor D_Mb = geodesic3d_pixelqueue(image, 1 - mask, spacing, l_grad, l_eucl);
+    torch::Tensor D_Mb = secondcall.get();
+
+    return D_M - D_Mb;
+}
+
+torch::Tensor signed_geodesic2d_fastmarch(const torch::Tensor &image, const torch::Tensor &mask, const float &l_grad, const float &l_eucl)
+{
+    auto secondcall = std::async(std::launch::async, geodesic2d_fastmarch, image, 1 - mask, l_grad, l_eucl);
+    torch::Tensor D_M = geodesic2d_fastmarch(image, mask, l_grad, l_eucl);
+    // torch::Tensor D_Mb = geodesic2d_fastmarch(image, 1 - mask, l_grad, l_eucl);
+    torch::Tensor D_Mb = secondcall.get();
+
+    return D_M - D_Mb;
+}
+
+torch::Tensor signed_geodesic3d_fastmarch(const torch::Tensor &image, const torch::Tensor &mask, const std::vector<float> &spacing, const float &l_grad, const float &l_eucl)
+{
+    auto secondcall = std::async(std::launch::async, geodesic3d_fastmarch, image, 1 - mask, spacing, l_grad, l_eucl);
+    torch::Tensor D_M = geodesic3d_fastmarch(image, mask, spacing, l_grad, l_eucl);
+    // torch::Tensor D_Mb = geodesic3d_fastmarch(image, 1 - mask, spacing, l_grad, l_eucl);
     torch::Tensor D_Mb = secondcall.get();
 
     return D_M - D_Mb;
 }
 
 torch::Tensor GSF2d(const torch::Tensor &image, const torch::Tensor &mask, const float &theta, const float &v, const float &lambda, const int &iterations)
 {
@@ -313,57 +364,89 @@
 
     torch::Tensor Dd_Md = -signed_generalised_geodesic3d_toivanen(image, 1 - Md, spacing, v, lambda, 1 - lambda, iterations);
     torch::Tensor De_Me = signed_generalised_geodesic3d_toivanen(image, Me, spacing, v, lambda, 1 - lambda, iterations);
 
     return Dd_Md + De_Me;
 }
 
-torch::Tensor GSF2d_fastmarch(const torch::Tensor &image, const torch::Tensor &mask, const float &theta, const float &v, const float &lambda)
+torch::Tensor GSF2d_pixelqueue(const torch::Tensor &image, const torch::Tensor &mask, const float &theta, const float &lambda)
+{
+    torch::Tensor Ds_M = signed_geodesic2d_pixelqueue(image, mask, lambda, 1 - lambda);
+
+    torch::Tensor Md = (Ds_M > theta).type_as(Ds_M);
+    torch::Tensor Me = (Ds_M > -theta).type_as(Ds_M);
+
+    torch::Tensor Dd_Md = -signed_geodesic2d_pixelqueue(image, 1 - Md, lambda, 1 - lambda);
+    torch::Tensor De_Me = signed_geodesic2d_pixelqueue(image, Me, lambda, 1 - lambda);
+
+    return Dd_Md + De_Me;
+}
+
+torch::Tensor GSF3d_pixelqueue(const torch::Tensor &image, const torch::Tensor &mask, const float &theta, const std::vector<float> &spacing, const float &lambda)
+{
+    torch::Tensor Ds_M = signed_geodesic3d_pixelqueue(image, mask, spacing, lambda, 1 - lambda);
+
+    torch::Tensor Md = (Ds_M > theta).type_as(Ds_M);
+    torch::Tensor Me = (Ds_M > -theta).type_as(Ds_M);
+
+    torch::Tensor Dd_Md = -signed_geodesic3d_pixelqueue(image, 1 - Md, spacing, lambda, 1 - lambda);
+    torch::Tensor De_Me = signed_geodesic3d_pixelqueue(image, Me, spacing, lambda, 1 - lambda);
+
+    return Dd_Md + De_Me;
+}
+
+torch::Tensor GSF2d_fastmarch(const torch::Tensor &image, const torch::Tensor &mask, const float &theta, const float &lambda)
 {
-    torch::Tensor Ds_M = signed_generalised_geodesic2d_fastmarch(image, mask, v, lambda, 1 - lambda);
+    torch::Tensor Ds_M = signed_geodesic2d_fastmarch(image, mask, lambda, 1 - lambda);
 
     torch::Tensor Md = (Ds_M > theta).type_as(Ds_M);
     torch::Tensor Me = (Ds_M > -theta).type_as(Ds_M);
 
-    torch::Tensor Dd_Md = -signed_generalised_geodesic2d_fastmarch(image, 1 - Md, v, lambda, 1 - lambda);
-    torch::Tensor De_Me = signed_generalised_geodesic2d_fastmarch(image, Me, v, lambda, 1 - lambda);
+    torch::Tensor Dd_Md = -signed_geodesic2d_fastmarch(image, 1 - Md, lambda, 1 - lambda);
+    torch::Tensor De_Me = signed_geodesic2d_fastmarch(image, Me, lambda, 1 - lambda);
 
     return Dd_Md + De_Me;
 }
 
-torch::Tensor GSF3d_fastmarch(const torch::Tensor &image, const torch::Tensor &mask, const float &theta, const std::vector<float> &spacing, const float &v, const float &lambda)
+torch::Tensor GSF3d_fastmarch(const torch::Tensor &image, const torch::Tensor &mask, const float &theta, const std::vector<float> &spacing, const float &lambda)
 {
-    torch::Tensor Ds_M = signed_generalised_geodesic3d_fastmarch(image, mask, spacing, v, lambda, 1 - lambda);
+    torch::Tensor Ds_M = signed_geodesic3d_fastmarch(image, mask, spacing, lambda, 1 - lambda);
 
     torch::Tensor Md = (Ds_M > theta).type_as(Ds_M);
     torch::Tensor Me = (Ds_M > -theta).type_as(Ds_M);
 
-    torch::Tensor Dd_Md = -signed_generalised_geodesic3d_fastmarch(image, 1 - Md, spacing, v, lambda, 1 - lambda);
-    torch::Tensor De_Me = signed_generalised_geodesic3d_fastmarch(image, Me, spacing, v, lambda, 1 - lambda);
+    torch::Tensor Dd_Md = -signed_geodesic3d_fastmarch(image, 1 - Md, spacing, lambda, 1 - lambda);
+    torch::Tensor De_Me = signed_geodesic3d_fastmarch(image, Me, spacing, lambda, 1 - lambda);
 
     return Dd_Md + De_Me;
 }
 
 PYBIND11_MODULE(TORCH_EXTENSION_NAME, m)
 {
     m.def("generalised_geodesic2d", &generalised_geodesic2d, "Generalised Geodesic distance 2d");
     m.def("generalised_geodesic3d", &generalised_geodesic3d, "Generalised Geodesic distance 3d");
     m.def("generalised_geodesic2d_toivanen", &generalised_geodesic2d_toivanen, "Generalised Geodesic distance 2d using Toivanen's method");
     m.def("generalised_geodesic3d_toivanen", &generalised_geodesic3d_toivanen, "Generalised Geodesic distance 3d using Toivanen's method");
-    m.def("generalised_geodesic2d_fastmarch", &generalised_geodesic2d_fastmarch, "Generalised Geodesic distance 2d using Fast Marching method");
-    m.def("generalised_geodesic3d_fastmarch", &generalised_geodesic3d_fastmarch, "Generalised Geodesic distance 3d using Fast Marching method");
+    m.def("geodesic2d_pixelqueue", &geodesic2d_pixelqueue, "Geodesic distance 2d using Pixel Queue method");
+    m.def("geodesic3d_pixelqueue", &geodesic3d_pixelqueue, "Geodesic distance 3d using Pixel Queue method");
+    m.def("geodesic2d_fastmarch", &geodesic2d_fastmarch, "Geodesic distance 2d using Fast Marching method");
+    m.def("geodesic3d_fastmarch", &geodesic3d_fastmarch, "Geodesic distance 3d using Fast Marching method");
 
     m.def("signed_generalised_geodesic2d", &signed_generalised_geodesic2d, "Signed Generalised Geodesic distance 2d");
     m.def("signed_generalised_geodesic3d", &signed_generalised_geodesic3d, "Signed Generalised Geodesic distance 3d");
     m.def("signed_generalised_geodesic2d_toivanen", &signed_generalised_geodesic2d_toivanen, "Signed Generalised Geodesic distance 2d using Toivanen's method");
     m.def("signed_generalised_geodesic3d_toivanen", &signed_generalised_geodesic3d_toivanen, "Signed Generalised Geodesic distance 3d using Toivanen's method");
-    m.def("signed_generalised_geodesic2d_fastmarch", &signed_generalised_geodesic2d_fastmarch, "Signed Generalised Geodesic distance 2d using Fast Marching method");
-    m.def("signed_generalised_geodesic3d_fastmarch", &signed_generalised_geodesic3d_fastmarch, "Signed Generalised Geodesic distance 3d using Fast Marching method");
+    m.def("signed_geodesic2d_pixelqueue", &signed_geodesic2d_pixelqueue, "Signed Geodesic distance 2d using Pixel Queue method");
+    m.def("signed_geodesic3d_pixelqueue", &signed_geodesic3d_pixelqueue, "Signed Geodesic distance 3d using Pixel Queue method");
+    m.def("signed_geodesic2d_fastmarch", &signed_geodesic2d_fastmarch, "Signed Geodesic distance 2d using Fast Marching method");
+    m.def("signed_geodesic3d_fastmarch", &signed_geodesic3d_fastmarch, "Signed Geodesic distance 3d using Fast Marching method");
 
     m.def("GSF2d", &GSF2d, "Geodesic Symmetric Filtering 2d");
     m.def("GSF3d", &GSF3d, "Geodesic Symmetric Filtering 3d");
     m.def("GSF2d_toivanen", &GSF2d_toivanen, "Geodesic Symmetric Filtering 2d using Toivanen's method");
     m.def("GSF3d_toivanen", &GSF3d_toivanen, "Geodesic Symmetric Filtering 3d using Toivanen's method");
+    m.def("GSF2d_pixelqueue", &GSF2d_pixelqueue, "Geodesic Symmetric Filtering 2d using Pixel Queue method");
+    m.def("GSF3d_pixelqueue", &GSF3d_pixelqueue, "Geodesic Symmetric Filtering 3d using Pixel Queue method");
     m.def("GSF2d_fastmarch", &GSF2d_fastmarch, "Geodesic Symmetric Filtering 2d using Fast Marching method");
     m.def("GSF3d_fastmarch", &GSF3d_fastmarch, "Geodesic Symmetric Filtering 3d using Fast Marching method");
     
 }
```

### Comparing `FastGeodis-1.0.2/FastGeodis/fastgeodis.h` & `FastGeodis-1.0.3/FastGeodis/fastgeodis.h`

 * *Files 12% similar despite different names*

```diff
@@ -83,26 +83,37 @@
     const torch::Tensor &mask,
     const std::vector<float> &spacing,
     const float &v,
     const float &l_grad,
     const float &l_eucl,
     const int &iterations);
 
-torch::Tensor generalised_geodesic2d_fastmarch_cpu(
+torch::Tensor geodesic2d_pixelqueue_cpu(
     const torch::Tensor &image,
     const torch::Tensor &mask,
-    const float &v,
     const float &l_grad,
     const float &l_eucl);
 
-torch::Tensor generalised_geodesic3d_fastmarch_cpu(
+torch::Tensor geodesic3d_pixelqueue_cpu(
+    const torch::Tensor &image,
+    const torch::Tensor &mask,
+    const std::vector<float> &spacing,
+    const float &l_grad,
+    const float &l_eucl);
+
+torch::Tensor geodesic2d_fastmarch_cpu(
+    const torch::Tensor &image,
+    const torch::Tensor &mask,
+    const float &l_grad,
+    const float &l_eucl);
+
+torch::Tensor geodesic3d_fastmarch_cpu(
     const torch::Tensor &image,
     const torch::Tensor &mask,
     const std::vector<float> &spacing,
-    const float &v,
     const float &l_grad,
     const float &l_eucl);
 
 
 torch::Tensor generalised_geodesic2d(
     const torch::Tensor &image,
     const torch::Tensor &mask,
@@ -133,26 +144,37 @@
     const torch::Tensor &mask,
     const std::vector<float> &spacing,
     const float &v,
     const float &l_grad,
     const float &l_eucl,
     const int &iterations);
 
-torch::Tensor generalised_geodesic2d_fastmarch(
+torch::Tensor geodesic2d_pixelqueue(
     const torch::Tensor &image,
     const torch::Tensor &mask,
-    const float &v,
     const float &l_grad,
     const float &l_eucl);
 
-torch::Tensor generalised_geodesic3d_fastmarch(
+torch::Tensor geodesic3d_pixelqueue(
+    const torch::Tensor &image,
+    const torch::Tensor &mask,
+    const std::vector<float> &spacing,
+    const float &l_grad,
+    const float &l_eucl);
+
+torch::Tensor geodesic2d_fastmarch(
+    const torch::Tensor &image,
+    const torch::Tensor &mask,
+    const float &l_grad,
+    const float &l_eucl);
+
+torch::Tensor geodesic3d_fastmarch(
     const torch::Tensor &image,
     const torch::Tensor &mask,
     const std::vector<float> &spacing,
-    const float &v,
     const float &l_grad,
     const float &l_eucl);
 
 
 torch::Tensor signed_generalised_geodesic2d(
     const torch::Tensor &image,
     const torch::Tensor &mask,
@@ -183,26 +205,37 @@
     const torch::Tensor &mask,
     const std::vector<float> &spacing,
     const float &v,
     const float &l_grad,
     const float &l_eucl,
     const int &iterations);
 
-torch::Tensor signed_generalised_geodesic2d_fastmarch(
+torch::Tensor signed_geodesic2d_pixelqueue(
     const torch::Tensor &image,
     const torch::Tensor &mask,
-    const float &v,
     const float &l_grad,
     const float &l_eucl);
 
-torch::Tensor signed_generalised_geodesic3d_fastmarch(
+torch::Tensor signed_geodesic3d_pixelqueue(
+    const torch::Tensor &image,
+    const torch::Tensor &mask,
+    const std::vector<float> &spacing,
+    const float &l_grad,
+    const float &l_eucl);
+
+torch::Tensor signed_geodesic2d_fastmarch(
+    const torch::Tensor &image,
+    const torch::Tensor &mask,
+    const float &l_grad,
+    const float &l_eucl);
+
+torch::Tensor signed_geodesic3d_fastmarch(
     const torch::Tensor &image,
     const torch::Tensor &mask,
     const std::vector<float> &spacing,
-    const float &v,
     const float &l_grad,
     const float &l_eucl);
 
 torch::Tensor GSF2d(
     const torch::Tensor &image, 
     const torch::Tensor &mask, 
     const float &theta, 
@@ -232,21 +265,32 @@
     const torch::Tensor &mask, 
     const float &theta, 
     const std::vector<float> &spacing, 
     const float &v, 
     const float &lambda, 
     const int &iterations);
 
+torch::Tensor GSF2d_pixelqueue(
+    const torch::Tensor &image, 
+    const torch::Tensor &mask, 
+    const float &theta, 
+    const float &lambda);
+
+torch::Tensor GSF3d_pixelqueue(
+    const torch::Tensor &image, 
+    const torch::Tensor &mask, 
+    const float &theta, 
+    const std::vector<float> &spacing, 
+    const float &lambda);
+
 torch::Tensor GSF2d_fastmarch(
     const torch::Tensor &image, 
     const torch::Tensor &mask, 
     const float &theta, 
-    const float &v, 
     const float &lambda);
 
 torch::Tensor GSF3d_fastmarch(
     const torch::Tensor &image, 
     const torch::Tensor &mask, 
     const float &theta, 
     const std::vector<float> &spacing, 
-    const float &v, 
     const float &lambda);
```

### Comparing `FastGeodis-1.0.2/FastGeodis/fastgeodis_cpu.cpp` & `FastGeodis-1.0.3/FastGeodis/fastgeodis_cpu.cpp`

 * *Files identical despite different names*

### Comparing `FastGeodis-1.0.2/FastGeodis/fastgeodis_cuda.cu` & `FastGeodis-1.0.3/FastGeodis/fastgeodis_cuda.cu`

 * *Files identical despite different names*

### Comparing `FastGeodis-1.0.2/FastGeodis/geodis_fastmarch.cpp` & `FastGeodis-1.0.3/FastGeodis/geodis_pixelqueue.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 // OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 // OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 #include <torch/extension.h>
 #include <vector>
 // #include <iostream>
 
-float l1distance_fastmarch(const float &in1, const float &in2)
+float l1distance_pixelqueue(const float &in1, const float &in2)
 {
     return std::abs(in1 - in2);
 }
 
 struct Point2D
 {
     float distance;
@@ -116,23 +116,23 @@
             {
                 continue;
             }
             
             l_dist = 0.0;
             if (channel == 1)
             {
-                l_dist = l1distance_fastmarch(
+                l_dist = l1distance_pixelqueue(
                     image_ptr[0][0][h][w], 
                     image_ptr[0][0][nh][nw]); 
             }
             else
             {
                 for (int c_i=0; c_i < channel; c_i++)
                 {
-                    l_dist += l1distance_fastmarch(
+                    l_dist += l1distance_pixelqueue(
                         image_ptr[0][c_i][h][w], 
                         image_ptr[0][c_i][nh][nw]);     
                 }       
             }
             delta_dis = l_eucl * space_dis + l_grad * l_dist;
             old_dis   = distance_ptr[0][0][nh][nw];
             new_dis   = distance_ptr[0][0][h][w] + delta_dis;
@@ -155,15 +155,15 @@
                     update_point_in_list(list, new_point);
                 }
             }
         }
     }
 }
 
-void geodesic2d_fastmarch_cpu(
+void geodesic2d_pixelqueue_cpu(
     const torch::Tensor &image,
     torch::Tensor &distance,
     const float &l_grad,
     const float &l_eucl)
 {
     // batch, channel, height, width
     const int channel = image.size(1);
@@ -195,30 +195,33 @@
 
     const float local_dist_f[9] = {
         sqrt(float(2.)), float(1), sqrt(float(2.)), 
         float(1.), float(0.), float(1.), 
         sqrt(float(2.)), float(1.), sqrt(float(2.))};
 
     int init_state;
-    float seed_type;
+    float seed_type, init_dis;
     
     for (int h = 0; h < height; h++)
     {
         for (int w = 0; w < width; w++)
         {
             seed_type = distance_ptr[0][0][h][w];
             if (seed_type > 0)
             {
                 init_state = 2;
+                init_dis = 1.0e10;
             }
             else
             {
                 init_state = 0;
+                init_dis = 0.0;
             }
             state[h][w] = init_state;
+            distance_ptr[0][0][h][w] = init_dis;
         }
     }
 
     // get initial temporary set
     std::vector<Point2D> temporary_list;
     temporary_list.reserve(width * height);
     int temp_state;
@@ -270,24 +273,23 @@
             height,
             width,
             l_grad,
             l_eucl);
     }
 }
 
-torch::Tensor generalised_geodesic2d_fastmarch_cpu(
+torch::Tensor geodesic2d_pixelqueue_cpu(
     const torch::Tensor &image,
     const torch::Tensor &mask,
-    const float &v,
     const float &l_grad,
     const float &l_eucl)
 {
-    torch::Tensor distance = v * mask.clone();
+    torch::Tensor distance = mask.clone();
 
-    geodesic2d_fastmarch_cpu(image, distance, l_grad, l_eucl);
+    geodesic2d_pixelqueue_cpu(image, distance, l_grad, l_eucl);
 
     return distance;
 }
 
 struct Point3D
 {
     float distance;
@@ -374,23 +376,23 @@
             {
                 continue;
             }
 
             l_dist = 0.0;
             if (channel == 1)
             {
-                l_dist = l1distance_fastmarch(
+                l_dist = l1distance_pixelqueue(
                     image_ptr[0][0][d][h][w], 
                     image_ptr[0][0][nd][nh][nw]); 
             }
             else
             {
                 for (int c_i=0; c_i < channel; c_i++)
                 {
-                    l_dist += l1distance_fastmarch(
+                    l_dist += l1distance_pixelqueue(
                         image_ptr[0][c_i][d][h][w], 
                         image_ptr[0][c_i][nd][nh][nw]);     
                 }       
             }                    
             delta_dis = l_eucl * space_dis + l_grad * l_dist;
             old_dis   = distance_ptr[0][0][nd][nh][nw];
             new_dis   = distance_ptr[0][0][d][h][w] + delta_dis;
@@ -416,15 +418,15 @@
                 }
             }
         }
     }
 }
 
 
-void geodesic3d_fastmarch_cpu(
+void geodesic3d_pixelqueue_cpu(
     const torch::Tensor &image,
     torch::Tensor &distance,
     std::vector<float> spacing,
     const float &l_grad,
     const float &l_eucl)
 {
     // batch, channel, depth, height, width
@@ -480,32 +482,35 @@
             ld += spacing[2] * spacing[2];
         }
 
         local_dist_f[ind] = sqrt(ld);
     }
     
     int init_state;
-    float seed_type;
+    float seed_type, init_dis;
 
     for(int d = 0; d < depth; d++)
     {
         for(int h = 0; h < height; h++)
         {
             for (int w = 0; w < width; w++)
             {
                 seed_type = distance_ptr[0][0][d][h][w];
                 if(seed_type > 0)
                 {
                     init_state = 2;
+                    init_dis = 1.0e10;
                 }
                 else
                 {
                     init_state = 0;
+                    init_dis = 0;
                 }
                 state_ptr[d][h][w] = init_state;
+                distance_ptr[0][0][d][h][w] = init_dis;
             }
         }
     }
     
     // get initial temporary set
     std::vector<Point3D> temporary_list;
     temporary_list.reserve(depth * height * width);
@@ -568,21 +573,20 @@
             height, 
             width, 
             l_grad,
             l_eucl);
     }
 }
 
-torch::Tensor generalised_geodesic3d_fastmarch_cpu(
+torch::Tensor geodesic3d_pixelqueue_cpu(
     const torch::Tensor &image,
     const torch::Tensor &mask,
     const std::vector<float> &spacing,
-    const float &v,
     const float &l_grad,
     const float &l_eucl)
 {
-    torch::Tensor distance = v * mask.clone();
+    torch::Tensor distance = mask.clone();
 
-    geodesic3d_fastmarch_cpu(image, distance, spacing, l_grad, l_eucl);
+    geodesic3d_pixelqueue_cpu(image, distance, spacing, l_grad, l_eucl);
 
     return distance;
 }
```

### Comparing `FastGeodis-1.0.2/FastGeodis/geodis_toivanen.cpp` & `FastGeodis-1.0.3/FastGeodis/geodis_toivanen.cpp`

 * *Files identical despite different names*

### Comparing `FastGeodis-1.0.2/FastGeodis.egg-info/PKG-INFO` & `FastGeodis-1.0.3/FastGeodis.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: FastGeodis
-Version: 1.0.2
+Version: 1.0.3
 Summary: Fast Implementation of Generalised Geodesic Distance Transform for CPU (OpenMP) and GPU (CUDA)
 Home-page: https://github.com/masadcv/FastGeodis
 Author: Muhammad Asad
 Author-email: masadcv@gmail.com
 License: BSD-3-Clause License
 Description: # FastGeodis: Fast Generalised Geodesic Distance Transform
         [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
-        <img src="https://img.shields.io/pypi/dm/fastgeodis.svg?label=PyPI%20downloads&logo=python&logoColor=green"/>
+        [![Downloads](https://static.pepy.tech/personalized-badge/fastgeodis?period=total&units=international_system&left_color=grey&right_color=green&left_text=Total%20Downloads)](https://pepy.tech/project/fastgeodis)
         [![status](https://joss.theoj.org/papers/d0b6e3daa4b22fec471691c6f1c60e2a/status.svg)](https://joss.theoj.org/papers/d0b6e3daa4b22fec471691c6f1c60e2a)
         [![CI Build](https://github.com/masadcv/FastGeodis/actions/workflows/build.yml/badge.svg)](https://github.com/masadcv/FastGeodis/actions/workflows/build.yml)
         [![PyPI version](https://badge.fury.io/py/FastGeodis.svg)](https://badge.fury.io/py/FastGeodis)
-        <img src="https://img.shields.io/badge/Python-3.6%20|%203.7%20|%203.8%20|%203.9-3776ab.svg"/>
+        <img src="https://img.shields.io/badge/Python-3.6%20|%203.7%20|%203.8%20|%203.9%20|%203.10%20-3776ab.svg"/>
         <img src="https://img.shields.io/badge/PyTorch-%3E%3D%201.5.0-brightgreen.svg"/>
-        
+        <!--<img src="https://img.shields.io/pypi/dm/fastgeodis.svg?label=PyPI%20downloads&logo=python&logoColor=green"/>-->
         This repository provides CPU (OpenMP) and GPU (CUDA) implementations of Generalised Geodesic Distance Transform in PyTorch for 2D and 3D input data based on parallelisable raster scan ideas from [1]. It includes methods for computing Geodesic, Euclidean distance transform and mixture of both. 
         
         | 2D images, 1 of 4 passes | 3D volumes, 1 of 6 passes  |
         |-------------------|-------------------------|
         | <img src="https://raw.githubusercontent.com/masadcv/FastGeodis/master/figures/FastGeodis2D.png?raw=true" width="300" /> | <img src="https://raw.githubusercontent.com/masadcv/FastGeodis/master/figures/FastGeodis3D.png?raw=true" width="300" /> |
         
         
@@ -83,22 +83,33 @@
         | Toivanen's Generalised Geodesic Distance 2D   |  Toivanen's generalised geodesic distance transform for CPU [9]          |      [FastGeodis.generalised_geodesic2d_toivanen](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.generalised_geodesic2d_toivanen)         |
         | Toivanen's Generalised Geodesic Distance 3D   |  Toivanen's generalised geodesic distance transform for CPU [9]          |      [FastGeodis.generalised_geodesic3d_toivanen](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.generalised_geodesic3d_toivanen)         |
         | Toivanen's Signed Generalised Geodesic Distance 2D   |  Toivanen's signed generalised geodesic distance transform for CPU [9]          |      [FastGeodis.signed_generalised_geodesic2d_toivanen](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.signed_generalised_geodesic2d_toivanen)         |
         | Toivanen's Signed Generalised Geodesic Distance 3D   |  Toivanen's signed generalised geodesic distance transform for CPU [9]          |      [FastGeodis.signed_generalised_geodesic3d_toivanen](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.signed_generalised_geodesic3d_toivanen)         |
         | Toivanen's Geodesic Symmetric Filtering 2D   |  Toivanen's geodesic symmetric filtering for CPU [2, 9]          |      [FastGeodis.GSF2d_toivanen](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.GSF2d_toivanen)         |
         | Toivanen's Geodesic Symmetric Filtering 3D   |  Toivanen's geodesic symmetric filtering for CPU [2, 9]          |      [FastGeodis.GSF3d_toivanen](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.GSF3d_toivanen)         |
         
+        ## Pixel Queue Implementations for CPU based on [11]
+        
+        | Method | Description | Documentation |
+        |--------|-------------|---------------|
+        | Pixel Queue Geodesic Distance 2D   |  Pixel Queue geodesic distance transform for CPU [11]          |      [FastGeodis.geodesic2d_fastmarch](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.geodesic2d_pixelqueue)         |
+        | Pixel Queue Geodesic Distance 3D   |  Pixel Queue geodesic distance transform for CPU [11]          |      [FastGeodis.geodesic3d_pixelqueue](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.geodesic3d_pixelqueue)         |
+        | Pixel Queue Signed Geodesic Distance 2D   |  Pixel Queue signed geodesic distance transform for CPU [11]          |      [FastGeodis.signed_geodesic2d_pixelqueue](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.signed_geodesic2d_pixelqueue)         |
+        | Pixel Queue Signed Geodesic Distance 3D   |  Pixel Queue signed geodesic distance transform for CPU [11]          |      [FastGeodis.signed_geodesic3d_pixelqueue](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.signed_geodesic3d_pixelqueue)         |
+        | Pixel Queue Geodesic Symmetric Filtering 2D   |  Pixel Queue geodesic symmetric filtering for CPU [2, 11]          |      [FastGeodis.GSF2d_pixelqueue](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.GSF2d_pixelqueue)         |
+        | Pixel Queue Geodesic Symmetric Filtering 3D   |  Pixel Queue geodesic symmetric filtering for CPU [2, 11]          |      [FastGeodis.GSF3d_pixelqueue](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.GSF3d_pixelqueue)         |
+        
         ## Fast Marching Implementations for CPU based on [4, 10]
         
         | Method | Description | Documentation |
         |--------|-------------|---------------|
-        | Fast Marching Generalised Geodesic Distance 2D   |  Fast Marching generalised geodesic distance transform for CPU [9]          |      [FastGeodis.generalised_geodesic2d_fastmarch](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.generalised_geodesic2d_fastmarch)         |
-        | Fast Marching Generalised Geodesic Distance 3D   |  Fast Marching generalised geodesic distance transform for CPU [9]          |      [FastGeodis.generalised_geodesic3d_fastmarch](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.generalised_geodesic3d_fastmarch)         |
-        | Fast Marching Signed Generalised Geodesic Distance 2D   |  Fast Marching signed generalised geodesic distance transform for CPU [9]          |      [FastGeodis.signed_generalised_geodesic2d_fastmarch](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.signed_generalised_geodesic2d_fastmarch)         |
-        | Fast Marching Signed Generalised Geodesic Distance 3D   |  Fast Marching signed generalised geodesic distance transform for CPU [9]          |      [FastGeodis.signed_generalised_geodesic3d_fastmarch](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.signed_generalised_geodesic3d_fastmarch)         |
+        | Fast Marching Geodesic Distance 2D   |  Fast Marching geodesic distance transform for CPU [9]          |      [FastGeodis.geodesic2d_fastmarch](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.geodesic2d_fastmarch)         |
+        | Fast Marching Geodesic Distance 3D   |  Fast Marching geodesic distance transform for CPU [9]          |      [FastGeodis.geodesic3d_fastmarch](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.geodesic3d_fastmarch)         |
+        | Fast Marching Signed Geodesic Distance 2D   |  Fast Marching signed geodesic distance transform for CPU [9]          |      [FastGeodis.signed_geodesic2d_fastmarch](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.signed_geodesic2d_fastmarch)         |
+        | Fast Marching Signed Geodesic Distance 3D   |  Fast Marching signed geodesic distance transform for CPU [9]          |      [FastGeodis.signed_geodesic3d_fastmarch](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.signed_geodesic3d_fastmarch)         |
         | Fast Marching Geodesic Symmetric Filtering 2D   |  Fast Marching geodesic symmetric filtering for CPU [2, 9]          |      [FastGeodis.GSF2d_fastmarch](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.GSF2d_fastmarch)         |
         | Fast Marching Geodesic Symmetric Filtering 3D   |  Fast Marching geodesic symmetric filtering for CPU [2, 9]          |      [FastGeodis.GSF3d_fastmarch](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.GSF3d_fastmarch)         |
         
         # Example usage
         
         ### Fast Geodesic Distance Transform
         The following demonstrates a simple example showing FastGeodis usage:
@@ -211,11 +222,13 @@
         
         - [8] [https://www.tensorflow.org/addons/api_docs/python/tfa/image/euclidean_dist_transform](https://www.tensorflow.org/addons/api_docs/python/tfa/image/euclidean_dist_transform)
         
         - [9] Toivanen, Pekka J. "New geodosic distance transforms for gray-scale images." Pattern Recognition Letters 17.5 (1996): 437-450.
         
         - [10] Sethian, James A. "Fast marching methods." SIAM review 41.2 (1999): 199-235.
         
+        - [11] Ikonen, L., & Toivanen, P. (2007). Distance and nearest neighbor transforms on gray-level surfaces. Pattern Recognition Letters, 28(5), 604-612. [[doi](https://doi.org/10.1016/j.patrec.2006.10.010)]
+        
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `FastGeodis-1.0.2/LICENSE` & `FastGeodis-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `FastGeodis-1.0.2/PKG-INFO` & `FastGeodis-1.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: FastGeodis
-Version: 1.0.2
+Version: 1.0.3
 Summary: Fast Implementation of Generalised Geodesic Distance Transform for CPU (OpenMP) and GPU (CUDA)
 Home-page: https://github.com/masadcv/FastGeodis
 Author: Muhammad Asad
 Author-email: masadcv@gmail.com
 License: BSD-3-Clause License
 Description: # FastGeodis: Fast Generalised Geodesic Distance Transform
         [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
-        <img src="https://img.shields.io/pypi/dm/fastgeodis.svg?label=PyPI%20downloads&logo=python&logoColor=green"/>
+        [![Downloads](https://static.pepy.tech/personalized-badge/fastgeodis?period=total&units=international_system&left_color=grey&right_color=green&left_text=Total%20Downloads)](https://pepy.tech/project/fastgeodis)
         [![status](https://joss.theoj.org/papers/d0b6e3daa4b22fec471691c6f1c60e2a/status.svg)](https://joss.theoj.org/papers/d0b6e3daa4b22fec471691c6f1c60e2a)
         [![CI Build](https://github.com/masadcv/FastGeodis/actions/workflows/build.yml/badge.svg)](https://github.com/masadcv/FastGeodis/actions/workflows/build.yml)
         [![PyPI version](https://badge.fury.io/py/FastGeodis.svg)](https://badge.fury.io/py/FastGeodis)
-        <img src="https://img.shields.io/badge/Python-3.6%20|%203.7%20|%203.8%20|%203.9-3776ab.svg"/>
+        <img src="https://img.shields.io/badge/Python-3.6%20|%203.7%20|%203.8%20|%203.9%20|%203.10%20-3776ab.svg"/>
         <img src="https://img.shields.io/badge/PyTorch-%3E%3D%201.5.0-brightgreen.svg"/>
-        
+        <!--<img src="https://img.shields.io/pypi/dm/fastgeodis.svg?label=PyPI%20downloads&logo=python&logoColor=green"/>-->
         This repository provides CPU (OpenMP) and GPU (CUDA) implementations of Generalised Geodesic Distance Transform in PyTorch for 2D and 3D input data based on parallelisable raster scan ideas from [1]. It includes methods for computing Geodesic, Euclidean distance transform and mixture of both. 
         
         | 2D images, 1 of 4 passes | 3D volumes, 1 of 6 passes  |
         |-------------------|-------------------------|
         | <img src="https://raw.githubusercontent.com/masadcv/FastGeodis/master/figures/FastGeodis2D.png?raw=true" width="300" /> | <img src="https://raw.githubusercontent.com/masadcv/FastGeodis/master/figures/FastGeodis3D.png?raw=true" width="300" /> |
         
         
@@ -83,22 +83,33 @@
         | Toivanen's Generalised Geodesic Distance 2D   |  Toivanen's generalised geodesic distance transform for CPU [9]          |      [FastGeodis.generalised_geodesic2d_toivanen](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.generalised_geodesic2d_toivanen)         |
         | Toivanen's Generalised Geodesic Distance 3D   |  Toivanen's generalised geodesic distance transform for CPU [9]          |      [FastGeodis.generalised_geodesic3d_toivanen](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.generalised_geodesic3d_toivanen)         |
         | Toivanen's Signed Generalised Geodesic Distance 2D   |  Toivanen's signed generalised geodesic distance transform for CPU [9]          |      [FastGeodis.signed_generalised_geodesic2d_toivanen](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.signed_generalised_geodesic2d_toivanen)         |
         | Toivanen's Signed Generalised Geodesic Distance 3D   |  Toivanen's signed generalised geodesic distance transform for CPU [9]          |      [FastGeodis.signed_generalised_geodesic3d_toivanen](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.signed_generalised_geodesic3d_toivanen)         |
         | Toivanen's Geodesic Symmetric Filtering 2D   |  Toivanen's geodesic symmetric filtering for CPU [2, 9]          |      [FastGeodis.GSF2d_toivanen](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.GSF2d_toivanen)         |
         | Toivanen's Geodesic Symmetric Filtering 3D   |  Toivanen's geodesic symmetric filtering for CPU [2, 9]          |      [FastGeodis.GSF3d_toivanen](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.GSF3d_toivanen)         |
         
+        ## Pixel Queue Implementations for CPU based on [11]
+        
+        | Method | Description | Documentation |
+        |--------|-------------|---------------|
+        | Pixel Queue Geodesic Distance 2D   |  Pixel Queue geodesic distance transform for CPU [11]          |      [FastGeodis.geodesic2d_fastmarch](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.geodesic2d_pixelqueue)         |
+        | Pixel Queue Geodesic Distance 3D   |  Pixel Queue geodesic distance transform for CPU [11]          |      [FastGeodis.geodesic3d_pixelqueue](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.geodesic3d_pixelqueue)         |
+        | Pixel Queue Signed Geodesic Distance 2D   |  Pixel Queue signed geodesic distance transform for CPU [11]          |      [FastGeodis.signed_geodesic2d_pixelqueue](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.signed_geodesic2d_pixelqueue)         |
+        | Pixel Queue Signed Geodesic Distance 3D   |  Pixel Queue signed geodesic distance transform for CPU [11]          |      [FastGeodis.signed_geodesic3d_pixelqueue](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.signed_geodesic3d_pixelqueue)         |
+        | Pixel Queue Geodesic Symmetric Filtering 2D   |  Pixel Queue geodesic symmetric filtering for CPU [2, 11]          |      [FastGeodis.GSF2d_pixelqueue](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.GSF2d_pixelqueue)         |
+        | Pixel Queue Geodesic Symmetric Filtering 3D   |  Pixel Queue geodesic symmetric filtering for CPU [2, 11]          |      [FastGeodis.GSF3d_pixelqueue](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.GSF3d_pixelqueue)         |
+        
         ## Fast Marching Implementations for CPU based on [4, 10]
         
         | Method | Description | Documentation |
         |--------|-------------|---------------|
-        | Fast Marching Generalised Geodesic Distance 2D   |  Fast Marching generalised geodesic distance transform for CPU [9]          |      [FastGeodis.generalised_geodesic2d_fastmarch](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.generalised_geodesic2d_fastmarch)         |
-        | Fast Marching Generalised Geodesic Distance 3D   |  Fast Marching generalised geodesic distance transform for CPU [9]          |      [FastGeodis.generalised_geodesic3d_fastmarch](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.generalised_geodesic3d_fastmarch)         |
-        | Fast Marching Signed Generalised Geodesic Distance 2D   |  Fast Marching signed generalised geodesic distance transform for CPU [9]          |      [FastGeodis.signed_generalised_geodesic2d_fastmarch](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.signed_generalised_geodesic2d_fastmarch)         |
-        | Fast Marching Signed Generalised Geodesic Distance 3D   |  Fast Marching signed generalised geodesic distance transform for CPU [9]          |      [FastGeodis.signed_generalised_geodesic3d_fastmarch](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.signed_generalised_geodesic3d_fastmarch)         |
+        | Fast Marching Geodesic Distance 2D   |  Fast Marching geodesic distance transform for CPU [9]          |      [FastGeodis.geodesic2d_fastmarch](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.geodesic2d_fastmarch)         |
+        | Fast Marching Geodesic Distance 3D   |  Fast Marching geodesic distance transform for CPU [9]          |      [FastGeodis.geodesic3d_fastmarch](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.geodesic3d_fastmarch)         |
+        | Fast Marching Signed Geodesic Distance 2D   |  Fast Marching signed geodesic distance transform for CPU [9]          |      [FastGeodis.signed_geodesic2d_fastmarch](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.signed_geodesic2d_fastmarch)         |
+        | Fast Marching Signed Geodesic Distance 3D   |  Fast Marching signed geodesic distance transform for CPU [9]          |      [FastGeodis.signed_geodesic3d_fastmarch](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.signed_geodesic3d_fastmarch)         |
         | Fast Marching Geodesic Symmetric Filtering 2D   |  Fast Marching geodesic symmetric filtering for CPU [2, 9]          |      [FastGeodis.GSF2d_fastmarch](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.GSF2d_fastmarch)         |
         | Fast Marching Geodesic Symmetric Filtering 3D   |  Fast Marching geodesic symmetric filtering for CPU [2, 9]          |      [FastGeodis.GSF3d_fastmarch](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.GSF3d_fastmarch)         |
         
         # Example usage
         
         ### Fast Geodesic Distance Transform
         The following demonstrates a simple example showing FastGeodis usage:
@@ -211,11 +222,13 @@
         
         - [8] [https://www.tensorflow.org/addons/api_docs/python/tfa/image/euclidean_dist_transform](https://www.tensorflow.org/addons/api_docs/python/tfa/image/euclidean_dist_transform)
         
         - [9] Toivanen, Pekka J. "New geodosic distance transforms for gray-scale images." Pattern Recognition Letters 17.5 (1996): 437-450.
         
         - [10] Sethian, James A. "Fast marching methods." SIAM review 41.2 (1999): 199-235.
         
+        - [11] Ikonen, L., & Toivanen, P. (2007). Distance and nearest neighbor transforms on gray-level surfaces. Pattern Recognition Letters, 28(5), 604-612. [[doi](https://doi.org/10.1016/j.patrec.2006.10.010)]
+        
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `FastGeodis-1.0.2/README.md` & `FastGeodis-1.0.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # FastGeodis: Fast Generalised Geodesic Distance Transform
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
-<img src="https://img.shields.io/pypi/dm/fastgeodis.svg?label=PyPI%20downloads&logo=python&logoColor=green"/>
+[![Downloads](https://static.pepy.tech/personalized-badge/fastgeodis?period=total&units=international_system&left_color=grey&right_color=green&left_text=Total%20Downloads)](https://pepy.tech/project/fastgeodis)
 [![status](https://joss.theoj.org/papers/d0b6e3daa4b22fec471691c6f1c60e2a/status.svg)](https://joss.theoj.org/papers/d0b6e3daa4b22fec471691c6f1c60e2a)
 [![CI Build](https://github.com/masadcv/FastGeodis/actions/workflows/build.yml/badge.svg)](https://github.com/masadcv/FastGeodis/actions/workflows/build.yml)
 [![PyPI version](https://badge.fury.io/py/FastGeodis.svg)](https://badge.fury.io/py/FastGeodis)
-<img src="https://img.shields.io/badge/Python-3.6%20|%203.7%20|%203.8%20|%203.9-3776ab.svg"/>
+<img src="https://img.shields.io/badge/Python-3.6%20|%203.7%20|%203.8%20|%203.9%20|%203.10%20-3776ab.svg"/>
 <img src="https://img.shields.io/badge/PyTorch-%3E%3D%201.5.0-brightgreen.svg"/>
-
+<!--<img src="https://img.shields.io/pypi/dm/fastgeodis.svg?label=PyPI%20downloads&logo=python&logoColor=green"/>-->
 This repository provides CPU (OpenMP) and GPU (CUDA) implementations of Generalised Geodesic Distance Transform in PyTorch for 2D and 3D input data based on parallelisable raster scan ideas from [1]. It includes methods for computing Geodesic, Euclidean distance transform and mixture of both. 
 
 | 2D images, 1 of 4 passes | 3D volumes, 1 of 6 passes  |
 |-------------------|-------------------------|
 | <img src="https://raw.githubusercontent.com/masadcv/FastGeodis/master/figures/FastGeodis2D.png?raw=true" width="300" /> | <img src="https://raw.githubusercontent.com/masadcv/FastGeodis/master/figures/FastGeodis3D.png?raw=true" width="300" /> |
 
 
@@ -75,22 +75,33 @@
 | Toivanen's Generalised Geodesic Distance 2D   |  Toivanen's generalised geodesic distance transform for CPU [9]          |      [FastGeodis.generalised_geodesic2d_toivanen](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.generalised_geodesic2d_toivanen)         |
 | Toivanen's Generalised Geodesic Distance 3D   |  Toivanen's generalised geodesic distance transform for CPU [9]          |      [FastGeodis.generalised_geodesic3d_toivanen](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.generalised_geodesic3d_toivanen)         |
 | Toivanen's Signed Generalised Geodesic Distance 2D   |  Toivanen's signed generalised geodesic distance transform for CPU [9]          |      [FastGeodis.signed_generalised_geodesic2d_toivanen](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.signed_generalised_geodesic2d_toivanen)         |
 | Toivanen's Signed Generalised Geodesic Distance 3D   |  Toivanen's signed generalised geodesic distance transform for CPU [9]          |      [FastGeodis.signed_generalised_geodesic3d_toivanen](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.signed_generalised_geodesic3d_toivanen)         |
 | Toivanen's Geodesic Symmetric Filtering 2D   |  Toivanen's geodesic symmetric filtering for CPU [2, 9]          |      [FastGeodis.GSF2d_toivanen](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.GSF2d_toivanen)         |
 | Toivanen's Geodesic Symmetric Filtering 3D   |  Toivanen's geodesic symmetric filtering for CPU [2, 9]          |      [FastGeodis.GSF3d_toivanen](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.GSF3d_toivanen)         |
 
+## Pixel Queue Implementations for CPU based on [11]
+
+| Method | Description | Documentation |
+|--------|-------------|---------------|
+| Pixel Queue Geodesic Distance 2D   |  Pixel Queue geodesic distance transform for CPU [11]          |      [FastGeodis.geodesic2d_fastmarch](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.geodesic2d_pixelqueue)         |
+| Pixel Queue Geodesic Distance 3D   |  Pixel Queue geodesic distance transform for CPU [11]          |      [FastGeodis.geodesic3d_pixelqueue](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.geodesic3d_pixelqueue)         |
+| Pixel Queue Signed Geodesic Distance 2D   |  Pixel Queue signed geodesic distance transform for CPU [11]          |      [FastGeodis.signed_geodesic2d_pixelqueue](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.signed_geodesic2d_pixelqueue)         |
+| Pixel Queue Signed Geodesic Distance 3D   |  Pixel Queue signed geodesic distance transform for CPU [11]          |      [FastGeodis.signed_geodesic3d_pixelqueue](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.signed_geodesic3d_pixelqueue)         |
+| Pixel Queue Geodesic Symmetric Filtering 2D   |  Pixel Queue geodesic symmetric filtering for CPU [2, 11]          |      [FastGeodis.GSF2d_pixelqueue](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.GSF2d_pixelqueue)         |
+| Pixel Queue Geodesic Symmetric Filtering 3D   |  Pixel Queue geodesic symmetric filtering for CPU [2, 11]          |      [FastGeodis.GSF3d_pixelqueue](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.GSF3d_pixelqueue)         |
+
 ## Fast Marching Implementations for CPU based on [4, 10]
 
 | Method | Description | Documentation |
 |--------|-------------|---------------|
-| Fast Marching Generalised Geodesic Distance 2D   |  Fast Marching generalised geodesic distance transform for CPU [9]          |      [FastGeodis.generalised_geodesic2d_fastmarch](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.generalised_geodesic2d_fastmarch)         |
-| Fast Marching Generalised Geodesic Distance 3D   |  Fast Marching generalised geodesic distance transform for CPU [9]          |      [FastGeodis.generalised_geodesic3d_fastmarch](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.generalised_geodesic3d_fastmarch)         |
-| Fast Marching Signed Generalised Geodesic Distance 2D   |  Fast Marching signed generalised geodesic distance transform for CPU [9]          |      [FastGeodis.signed_generalised_geodesic2d_fastmarch](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.signed_generalised_geodesic2d_fastmarch)         |
-| Fast Marching Signed Generalised Geodesic Distance 3D   |  Fast Marching signed generalised geodesic distance transform for CPU [9]          |      [FastGeodis.signed_generalised_geodesic3d_fastmarch](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.signed_generalised_geodesic3d_fastmarch)         |
+| Fast Marching Geodesic Distance 2D   |  Fast Marching geodesic distance transform for CPU [9]          |      [FastGeodis.geodesic2d_fastmarch](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.geodesic2d_fastmarch)         |
+| Fast Marching Geodesic Distance 3D   |  Fast Marching geodesic distance transform for CPU [9]          |      [FastGeodis.geodesic3d_fastmarch](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.geodesic3d_fastmarch)         |
+| Fast Marching Signed Geodesic Distance 2D   |  Fast Marching signed geodesic distance transform for CPU [9]          |      [FastGeodis.signed_geodesic2d_fastmarch](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.signed_geodesic2d_fastmarch)         |
+| Fast Marching Signed Geodesic Distance 3D   |  Fast Marching signed geodesic distance transform for CPU [9]          |      [FastGeodis.signed_geodesic3d_fastmarch](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.signed_geodesic3d_fastmarch)         |
 | Fast Marching Geodesic Symmetric Filtering 2D   |  Fast Marching geodesic symmetric filtering for CPU [2, 9]          |      [FastGeodis.GSF2d_fastmarch](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.GSF2d_fastmarch)         |
 | Fast Marching Geodesic Symmetric Filtering 3D   |  Fast Marching geodesic symmetric filtering for CPU [2, 9]          |      [FastGeodis.GSF3d_fastmarch](https://fastgeodis.readthedocs.io/en/latest/api_docs.html#FastGeodis.GSF3d_fastmarch)         |
 
 # Example usage
 
 ### Fast Geodesic Distance Transform
 The following demonstrates a simple example showing FastGeodis usage:
@@ -202,7 +213,9 @@
 - [7] [https://docs.scipy.org/doc/scipy/reference/generated/scipy.ndimage.distance_transform_edt.html](https://docs.scipy.org/doc/scipy/reference/generated/scipy.ndimage.distance_transform_edt.html)
 
 - [8] [https://www.tensorflow.org/addons/api_docs/python/tfa/image/euclidean_dist_transform](https://www.tensorflow.org/addons/api_docs/python/tfa/image/euclidean_dist_transform)
 
 - [9] Toivanen, Pekka J. "New geodosic distance transforms for gray-scale images." Pattern Recognition Letters 17.5 (1996): 437-450.
 
 - [10] Sethian, James A. "Fast marching methods." SIAM review 41.2 (1999): 199-235.
+
+- [11] Ikonen, L., & Toivanen, P. (2007). Distance and nearest neighbor transforms on gray-level surfaces. Pattern Recognition Letters, 28(5), 604-612. [[doi](https://doi.org/10.1016/j.patrec.2006.10.010)]
```

### Comparing `FastGeodis-1.0.2/setup.py` & `FastGeodis-1.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -116,17 +116,20 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 with open("requirements.txt", "r") as fp:
     install_requires = fp.read().splitlines()
 
+# add dependencies folder in include path
+dep_dir = os.path.join(".", "dependency")
+
 setup(
     name="FastGeodis",
-    version="1.0.2",
+    version="1.0.3",
     description="Fast Implementation of Generalised Geodesic Distance Transform for CPU (OpenMP) and GPU (CUDA)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/masadcv/FastGeodis",
     author="Muhammad Asad",
     author_email="masadcv@gmail.com",
     license="BSD-3-Clause License",
@@ -137,8 +140,9 @@
     install_requires=install_requires,
     cmdclass={
         "build_ext": BuildExtension
     },  # .with_options(no_python_abi_suffix=True)},
     packages=find_packages(exclude=("data", "docs", "examples", "scripts", "tests")),
     zip_safe=False,
     ext_modules=get_extensions(),
+    include_dirs=[dep_dir],
 )
```

