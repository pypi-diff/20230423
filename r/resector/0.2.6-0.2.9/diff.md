# Comparing `tmp/resector-0.2.6.tar.gz` & `tmp/resector-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resector-0.2.6.tar", last modified: Thu Feb  4 19:27:49 2021, max compression
+gzip compressed data, was "resector-0.2.9.tar", last modified: Mon Aug  2 16:07:05 2021, max compression
```

## Comparing `resector-0.2.6.tar` & `resector-0.2.9.tar`

### file list

```diff
@@ -1,49 +1,52 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-04 19:27:49.905140 resector-0.2.6/
--rw-rw-r--   0 travis    (2000) travis    (2000)      180 2021-02-04 19:24:03.000000 resector-0.2.6/AUTHORS.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     3538 2021-02-04 19:24:03.000000 resector-0.2.6/CONTRIBUTING.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       89 2021-02-04 19:24:03.000000 resector-0.2.6/HISTORY.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1080 2021-02-04 19:24:03.000000 resector-0.2.6/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      262 2021-02-04 19:24:03.000000 resector-0.2.6/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     3089 2021-02-04 19:27:49.905140 resector-0.2.6/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1731 2021-02-04 19:24:03.000000 resector-0.2.6/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-04 19:27:49.893140 resector-0.2.6/docs/
--rw-rw-r--   0 travis    (2000) travis    (2000)      609 2021-02-04 19:24:03.000000 resector-0.2.6/docs/Makefile
--rw-rw-r--   0 travis    (2000) travis    (2000)       28 2021-02-04 19:24:03.000000 resector-0.2.6/docs/authors.rst
--rwxrwxr-x   0 travis    (2000) travis    (2000)     4849 2021-02-04 19:24:03.000000 resector-0.2.6/docs/conf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       33 2021-02-04 19:24:03.000000 resector-0.2.6/docs/contributing.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       28 2021-02-04 19:24:03.000000 resector-0.2.6/docs/history.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-04 19:27:49.893140 resector-0.2.6/docs/images/
--rw-rw-r--   0 travis    (2000) travis    (2000)  9372225 2021-02-04 19:24:03.000000 resector-0.2.6/docs/images/60_examples_resized_50.gif
--rw-rw-r--   0 travis    (2000) travis    (2000)      305 2021-02-04 19:24:03.000000 resector-0.2.6/docs/index.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1118 2021-02-04 19:24:03.000000 resector-0.2.6/docs/installation.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      770 2021-02-04 19:24:03.000000 resector-0.2.6/docs/make.bat
--rw-rw-r--   0 travis    (2000) travis    (2000)       27 2021-02-04 19:24:03.000000 resector-0.2.6/docs/readme.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       71 2021-02-04 19:24:03.000000 resector-0.2.6/docs/usage.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-04 19:27:49.905140 resector-0.2.6/resector/
--rw-rw-r--   0 travis    (2000) travis    (2000)      422 2021-02-04 19:24:03.000000 resector-0.2.6/resector/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-04 19:27:49.905140 resector-0.2.6/resector/cli/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-02-04 19:24:03.000000 resector-0.2.6/resector/cli/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2960 2021-02-04 19:24:03.000000 resector-0.2.6/resector/cli/create_noise_volume.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5384 2021-02-04 19:24:03.000000 resector-0.2.6/resector/cli/resect.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3548 2021-02-04 19:24:03.000000 resector-0.2.6/resector/image.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4022 2021-02-04 19:24:03.000000 resector-0.2.6/resector/io.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10556 2021-02-04 19:24:03.000000 resector-0.2.6/resector/mesh.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6436 2021-02-04 19:24:03.000000 resector-0.2.6/resector/parcellation.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10371 2021-02-04 19:24:03.000000 resector-0.2.6/resector/random_resection.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4666 2021-02-04 19:24:03.000000 resector-0.2.6/resector/resector.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-02-04 19:24:03.000000 resector-0.2.6/resector/shape.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8559 2021-02-04 19:24:03.000000 resector-0.2.6/resector/texture.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      296 2021-02-04 19:24:03.000000 resector-0.2.6/resector/timer.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-04 19:27:49.905140 resector-0.2.6/resector.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3089 2021-02-04 19:27:49.000000 resector-0.2.6/resector.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      845 2021-02-04 19:27:49.000000 resector-0.2.6/resector.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-02-04 19:27:49.000000 resector-0.2.6/resector.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      113 2021-02-04 19:27:49.000000 resector-0.2.6/resector.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-02-04 19:27:49.000000 resector-0.2.6/resector.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)       58 2021-02-04 19:27:49.000000 resector-0.2.6/resector.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        9 2021-02-04 19:27:49.000000 resector-0.2.6/resector.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      391 2021-02-04 19:27:49.909140 resector-0.2.6/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1782 2021-02-04 19:24:03.000000 resector-0.2.6/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-04 19:27:49.905140 resector-0.2.6/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)       63 2021-02-04 19:24:03.000000 resector-0.2.6/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      513 2021-02-04 19:24:03.000000 resector-0.2.6/tests/test_resector.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-08-02 16:07:05.176992 resector-0.2.9/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3538 2021-08-02 16:03:05.000000 resector-0.2.9/CONTRIBUTING.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)       89 2021-08-02 16:03:05.000000 resector-0.2.9/HISTORY.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1080 2021-08-02 16:03:05.000000 resector-0.2.9/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)      314 2021-08-02 16:03:05.000000 resector-0.2.9/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5575 2021-08-02 16:07:05.176992 resector-0.2.9/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4646 2021-08-02 16:03:05.000000 resector-0.2.9/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-08-02 16:07:05.160992 resector-0.2.9/docs/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      609 2021-08-02 16:03:05.000000 resector-0.2.9/docs/Makefile
+-rw-rw-r--   0 travis    (2000) travis    (2000)       28 2021-08-02 16:03:05.000000 resector-0.2.9/docs/authors.rst
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     4849 2021-08-02 16:03:05.000000 resector-0.2.9/docs/conf.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       33 2021-08-02 16:03:05.000000 resector-0.2.9/docs/contributing.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)       28 2021-08-02 16:03:05.000000 resector-0.2.9/docs/history.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-08-02 16:07:05.160992 resector-0.2.9/docs/images/
+-rw-rw-r--   0 travis    (2000) travis    (2000)  9372225 2021-08-02 16:03:05.000000 resector-0.2.9/docs/images/60_examples_resized_50.gif
+-rw-rw-r--   0 travis    (2000) travis    (2000)      305 2021-08-02 16:03:05.000000 resector-0.2.9/docs/index.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1118 2021-08-02 16:03:05.000000 resector-0.2.9/docs/installation.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      770 2021-08-02 16:03:05.000000 resector-0.2.9/docs/make.bat
+-rw-rw-r--   0 travis    (2000) travis    (2000)       27 2021-08-02 16:03:05.000000 resector-0.2.9/docs/readme.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)       71 2021-08-02 16:03:05.000000 resector-0.2.9/docs/usage.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-08-02 16:07:05.176992 resector-0.2.9/resector/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7357 2021-08-02 16:03:05.000000 resector-0.2.9/resector/BrainAnatomyLabelsV3_0.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      422 2021-08-02 16:03:05.000000 resector-0.2.9/resector/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-08-02 16:07:05.176992 resector-0.2.9/resector/cli/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-08-02 16:03:05.000000 resector-0.2.9/resector/cli/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2960 2021-08-02 16:03:05.000000 resector-0.2.9/resector/cli/create_noise_volume.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5384 2021-08-02 16:03:05.000000 resector-0.2.9/resector/cli/resect.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3548 2021-08-02 16:03:05.000000 resector-0.2.9/resector/image.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3791 2021-08-02 16:03:05.000000 resector-0.2.9/resector/io.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10556 2021-08-02 16:03:05.000000 resector-0.2.9/resector/mesh.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6429 2021-08-02 16:03:05.000000 resector-0.2.9/resector/parcellation.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10371 2021-08-02 16:03:05.000000 resector-0.2.9/resector/random_resection.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4666 2021-08-02 16:03:05.000000 resector-0.2.9/resector/resector.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-08-02 16:07:05.176992 resector-0.2.9/resector/resources/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    84086 2021-08-02 16:03:05.000000 resector-0.2.9/resector/resources/geodesic_polyhedron.vtp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4469 2021-08-02 16:03:05.000000 resector-0.2.9/resector/resources/volumes.csv
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-08-02 16:03:05.000000 resector-0.2.9/resector/shape.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8559 2021-08-02 16:03:05.000000 resector-0.2.9/resector/texture.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      296 2021-08-02 16:03:05.000000 resector-0.2.9/resector/timer.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-08-02 16:07:05.176992 resector-0.2.9/resector.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5575 2021-08-02 16:07:05.000000 resector-0.2.9/resector.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      943 2021-08-02 16:07:05.000000 resector-0.2.9/resector.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-08-02 16:07:05.000000 resector-0.2.9/resector.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      113 2021-08-02 16:07:05.000000 resector-0.2.9/resector.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-08-02 16:07:05.000000 resector-0.2.9/resector.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)       58 2021-08-02 16:07:05.000000 resector-0.2.9/resector.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        9 2021-08-02 16:07:05.000000 resector-0.2.9/resector.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      391 2021-08-02 16:07:05.180992 resector-0.2.9/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1782 2021-08-02 16:03:05.000000 resector-0.2.9/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-08-02 16:07:05.176992 resector-0.2.9/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       63 2021-08-02 16:03:05.000000 resector-0.2.9/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      513 2021-08-02 16:03:05.000000 resector-0.2.9/tests/test_resector.py
```

### Comparing `resector-0.2.6/CONTRIBUTING.rst` & `resector-0.2.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `resector-0.2.6/LICENSE` & `resector-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `resector-0.2.6/docs/Makefile` & `resector-0.2.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `resector-0.2.6/docs/conf.py` & `resector-0.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `resector-0.2.6/docs/images/60_examples_resized_50.gif` & `resector-0.2.9/docs/images/60_examples_resized_50.gif`

 * *Files identical despite different names*

### Comparing `resector-0.2.6/docs/installation.rst` & `resector-0.2.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `resector-0.2.6/docs/make.bat` & `resector-0.2.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `resector-0.2.6/resector/cli/create_noise_volume.py` & `resector-0.2.9/resector/cli/create_noise_volume.py`

 * *Files identical despite different names*

### Comparing `resector-0.2.6/resector/cli/resect.py` & `resector-0.2.9/resector/cli/resect.py`

 * *Files identical despite different names*

### Comparing `resector-0.2.6/resector/image.py` & `resector-0.2.9/resector/image.py`

 * *Files identical despite different names*

### Comparing `resector-0.2.6/resector/io.py` & `resector-0.2.9/resector/io.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 
 import gzip
 import shutil
 import struct
 from pathlib import Path
 from tempfile import NamedTemporaryFile
+
 import vtk
 import numpy as np
+import torchio as tio
 import nibabel as nib
 import SimpleITK as sitk
 
 
 CHECK_QFAC = False
 debug_dir = None
 debug_num_files = 0
@@ -57,29 +59,16 @@
         nii.header['qform_code'] = 1
         nii.header['sform_code'] = 0
         nii.to_filename(image_path)
     if CHECK_QFAC:
         check_qfac(image_path)
 
 
-def nib_to_sitk(array, affine):
-    """
-    This actually seems faster than .parcellation.get_image_from_reference
-    """
-    array = array if isinstance(array, np.ndarray) else array.numpy()
-    with NamedTemporaryFile(suffix='.nii') as f:
-        nib.Nifti1Image(array, affine).to_filename(f.name)
-        if CHECK_QFAC:
-            check_qfac(f.name)
-        image = read_itk(f.name)
-    return image
-
-
 def get_sphere_poly_data():
-    resources_dir = Path(__file__).parent.parent / 'resources'
+    resources_dir = Path(__file__).parent / 'resources'
     mesh_path = resources_dir / 'geodesic_polyhedron.vtp'
     if not mesh_path.is_file():
         raise FileNotFoundError(f'{mesh_path} does not exist')
     poly_data = read_poly_data(mesh_path)
     if poly_data.GetNumberOfPoints() == 0:
         message = (
             f'Error reading sphere poly data from {mesh_path}. Contents:'
@@ -128,7 +117,13 @@
         write_poly_data(x, path, flip=True)
     elif isinstance(x, sitk.Image):
         path = debug_dir / f'{out_stem}.nii.gz'
         write(x, path)
     else:
         raise TypeError(f'Type not understood: {type(x)}')
     debug_num_files += 1
+
+
+def nib_to_sitk(array: np.ndarray, affine: np.ndarray):
+    assert array.ndim == 3
+    array = array[np.newaxis]
+    return tio.io.nib_to_sitk(array, affine)
```

### Comparing `resector-0.2.6/resector/mesh.py` & `resector-0.2.9/resector/mesh.py`

 * *Files identical despite different names*

### Comparing `resector-0.2.6/resector/parcellation.py` & `resector-0.2.9/resector/parcellation.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,15 +122,15 @@
             label, name = line.split()[:2]
             label = int(label)
             progress.set_description(f'Removing {name}')
             array[array == label] = 0
 
 
 def get_color_table():
-    labels_path = Path(__file__).parent.parent / 'BrainAnatomyLabelsV3_0.txt'
+    labels_path = Path(__file__).parent / 'BrainAnatomyLabelsV3_0.txt'
     lines = labels_path.read_text().splitlines()
     return lines
 
 
 def get_image_from_reference(array, reference):
     if array.dtype == np.bool:
         array = array.astype(np.uint8)
```

### Comparing `resector-0.2.6/resector/random_resection.py` & `resector-0.2.9/resector/random_resection.py`

 * *Files identical despite different names*

### Comparing `resector-0.2.6/resector/resector.py` & `resector-0.2.9/resector/resector.py`

 * *Files identical despite different names*

### Comparing `resector-0.2.6/resector/texture.py` & `resector-0.2.9/resector/texture.py`

 * *Files identical despite different names*

### Comparing `resector-0.2.6/resector.egg-info/SOURCES.txt` & `resector-0.2.9/resector.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-AUTHORS.rst
 CONTRIBUTING.rst
 HISTORY.rst
 LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
@@ -13,14 +12,15 @@
 docs/history.rst
 docs/index.rst
 docs/installation.rst
 docs/make.bat
 docs/readme.rst
 docs/usage.rst
 docs/images/60_examples_resized_50.gif
+resector/BrainAnatomyLabelsV3_0.txt
 resector/__init__.py
 resector/image.py
 resector/io.py
 resector/mesh.py
 resector/parcellation.py
 resector/random_resection.py
 resector/resector.py
@@ -33,9 +33,11 @@
 resector.egg-info/entry_points.txt
 resector.egg-info/not-zip-safe
 resector.egg-info/requires.txt
 resector.egg-info/top_level.txt
 resector/cli/__init__.py
 resector/cli/create_noise_volume.py
 resector/cli/resect.py
+resector/resources/geodesic_polyhedron.vtp
+resector/resources/volumes.csv
 tests/__init__.py
 tests/test_resector.py
```

### Comparing `resector-0.2.6/setup.py` & `resector-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,10 +54,10 @@
     keywords='resector',
     name='resector',
     packages=find_packages(include=['resector', 'resector.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/fepegar/resector',
-    version='0.2.6',
+    version='0.2.9',
     zip_safe=False,
 )
```

### Comparing `resector-0.2.6/tests/test_resector.py` & `resector-0.2.9/tests/test_resector.py`

 * *Files identical despite different names*

