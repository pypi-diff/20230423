# Comparing `tmp/metaseg-0.6.1.tar.gz` & `tmp/metaseg-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaseg-0.6.1.tar", last modified: Wed Apr 12 16:55:23 2023, max compression
+gzip compressed data, was "metaseg-0.7.0.tar", last modified: Sun Apr 23 14:53:37 2023, max compression
```

## Comparing `metaseg-0.6.1.tar` & `metaseg-0.7.0.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 16:55:23.451956 metaseg-0.6.1/
--rw-r--r--   0 kadir     (1000) kadir     (1001)    11357 2023-04-12 11:10:24.000000 metaseg-0.6.1/LICENSE
--rw-r--r--   0 kadir     (1000) kadir     (1001)       24 2023-04-12 11:10:24.000000 metaseg-0.6.1/MANIFEST.in
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3531 2023-04-12 16:55:23.451956 metaseg-0.6.1/PKG-INFO
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3257 2023-04-12 16:55:20.000000 metaseg-0.6.1/README.md
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 16:55:23.445290 metaseg-0.6.1/metaseg/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      631 2023-04-12 16:55:20.000000 metaseg-0.6.1/metaseg/__init__.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 16:55:23.448623 metaseg-0.6.1/metaseg/generator/
--rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-12 11:10:24.000000 metaseg-0.6.1/metaseg/generator/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    15127 2023-04-12 11:10:24.000000 metaseg-0.6.1/metaseg/generator/automatic_mask_generator.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2936 2023-04-12 11:10:24.000000 metaseg-0.6.1/metaseg/generator/build_sam.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    11570 2023-04-12 11:10:24.000000 metaseg-0.6.1/metaseg/generator/predictor.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8608 2023-04-12 16:55:20.000000 metaseg-0.6.1/metaseg/mask_predictor.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 16:55:23.448623 metaseg-0.6.1/metaseg/modeling/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      465 2023-04-12 11:10:24.000000 metaseg-0.6.1/metaseg/modeling/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1479 2023-04-12 11:10:24.000000 metaseg-0.6.1/metaseg/modeling/common.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    14341 2023-04-12 11:10:24.000000 metaseg-0.6.1/metaseg/modeling/image_encoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     6540 2023-04-12 11:10:24.000000 metaseg-0.6.1/metaseg/modeling/mask_decoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8596 2023-04-12 11:10:24.000000 metaseg-0.6.1/metaseg/modeling/prompt_encoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     7273 2023-04-12 11:10:24.000000 metaseg-0.6.1/metaseg/modeling/sam.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8332 2023-04-12 11:10:24.000000 metaseg-0.6.1/metaseg/modeling/transformer.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3515 2023-04-12 16:41:21.000000 metaseg-0.6.1/metaseg/sahi_predict.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 16:55:23.448623 metaseg-0.6.1/metaseg/utils/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      276 2023-04-12 11:10:24.000000 metaseg-0.6.1/metaseg/utils/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    12621 2023-04-12 11:10:24.000000 metaseg-0.6.1/metaseg/utils/amg.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2327 2023-04-12 11:10:24.000000 metaseg-0.6.1/metaseg/utils/data_utils.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1231 2023-04-12 11:10:24.000000 metaseg-0.6.1/metaseg/utils/file_utils.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     5743 2023-04-12 11:10:24.000000 metaseg-0.6.1/metaseg/utils/onnx.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3874 2023-04-12 11:10:24.000000 metaseg-0.6.1/metaseg/utils/transforms.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 16:55:23.451956 metaseg-0.6.1/metaseg/webapp/
--rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-12 11:10:24.000000 metaseg-0.6.1/metaseg/webapp/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8416 2023-04-12 16:41:21.000000 metaseg-0.6.1/metaseg/webapp/app.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2470 2023-04-12 16:41:21.000000 metaseg-0.6.1/metaseg/webapp/demo.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 16:55:23.445290 metaseg-0.6.1/metaseg.egg-info/
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3531 2023-04-12 16:55:23.000000 metaseg-0.6.1/metaseg.egg-info/PKG-INFO
--rw-r--r--   0 kadir     (1000) kadir     (1001)      881 2023-04-12 16:55:23.000000 metaseg-0.6.1/metaseg.egg-info/SOURCES.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)        1 2023-04-12 16:55:23.000000 metaseg-0.6.1/metaseg.egg-info/dependency_links.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)      230 2023-04-12 16:55:23.000000 metaseg-0.6.1/metaseg.egg-info/requires.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)        8 2023-04-12 16:55:23.000000 metaseg-0.6.1/metaseg.egg-info/top_level.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)       80 2023-04-12 11:10:24.000000 metaseg-0.6.1/pyproject.toml
--rw-r--r--   0 kadir     (1000) kadir     (1001)      143 2023-04-12 16:41:21.000000 metaseg-0.6.1/requirements.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)      430 2023-04-12 16:55:23.451956 metaseg-0.6.1/setup.cfg
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1529 2023-04-12 11:10:24.000000 metaseg-0.6.1/setup.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-23 14:53:37.570629 metaseg-0.7.0/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    11357 2023-04-20 11:50:36.000000 metaseg-0.7.0/LICENSE
+-rw-r--r--   0 kadir     (1000) kadir     (1001)       24 2023-04-20 11:50:36.000000 metaseg-0.7.0/MANIFEST.in
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     4419 2023-04-23 14:53:37.570629 metaseg-0.7.0/PKG-INFO
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     4145 2023-04-23 14:51:06.000000 metaseg-0.7.0/README.md
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-23 14:53:37.560629 metaseg-0.7.0/metaseg/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      707 2023-04-23 14:53:31.000000 metaseg-0.7.0/metaseg/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2832 2023-04-23 14:53:31.000000 metaseg-0.7.0/metaseg/falai_demo.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-23 14:53:37.567296 metaseg-0.7.0/metaseg/generator/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-20 11:50:36.000000 metaseg-0.7.0/metaseg/generator/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    15127 2023-04-20 11:50:36.000000 metaseg-0.7.0/metaseg/generator/automatic_mask_generator.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2936 2023-04-20 11:50:36.000000 metaseg-0.7.0/metaseg/generator/build_sam.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    11570 2023-04-20 11:50:36.000000 metaseg-0.7.0/metaseg/generator/predictor.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8048 2023-04-23 14:51:06.000000 metaseg-0.7.0/metaseg/mask_predictor.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-23 14:53:37.567296 metaseg-0.7.0/metaseg/modeling/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      465 2023-04-20 11:50:36.000000 metaseg-0.7.0/metaseg/modeling/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1479 2023-04-20 11:50:36.000000 metaseg-0.7.0/metaseg/modeling/common.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    14341 2023-04-20 11:50:36.000000 metaseg-0.7.0/metaseg/modeling/image_encoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     6540 2023-04-20 11:50:36.000000 metaseg-0.7.0/metaseg/modeling/mask_decoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8596 2023-04-20 11:50:36.000000 metaseg-0.7.0/metaseg/modeling/prompt_encoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     7273 2023-04-20 11:50:36.000000 metaseg-0.7.0/metaseg/modeling/sam.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8332 2023-04-20 11:50:36.000000 metaseg-0.7.0/metaseg/modeling/transformer.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3515 2023-04-20 11:50:36.000000 metaseg-0.7.0/metaseg/sahi_predict.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-23 14:53:37.570629 metaseg-0.7.0/metaseg/utils/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      276 2023-04-20 11:50:36.000000 metaseg-0.7.0/metaseg/utils/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    12621 2023-04-20 11:50:36.000000 metaseg-0.7.0/metaseg/utils/amg.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2807 2023-04-23 14:10:49.000000 metaseg-0.7.0/metaseg/utils/data_utils.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1231 2023-04-20 11:50:36.000000 metaseg-0.7.0/metaseg/utils/file_utils.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     5743 2023-04-20 11:50:36.000000 metaseg-0.7.0/metaseg/utils/onnx.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3874 2023-04-20 11:50:36.000000 metaseg-0.7.0/metaseg/utils/transforms.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-23 14:53:37.570629 metaseg-0.7.0/metaseg/webapp/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-20 11:50:36.000000 metaseg-0.7.0/metaseg/webapp/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8416 2023-04-20 11:50:36.000000 metaseg-0.7.0/metaseg/webapp/app.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2470 2023-04-20 11:50:36.000000 metaseg-0.7.0/metaseg/webapp/demo.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-23 14:53:37.563963 metaseg-0.7.0/metaseg.egg-info/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     4419 2023-04-23 14:53:37.000000 metaseg-0.7.0/metaseg.egg-info/PKG-INFO
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      903 2023-04-23 14:53:37.000000 metaseg-0.7.0/metaseg.egg-info/SOURCES.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        1 2023-04-23 14:53:37.000000 metaseg-0.7.0/metaseg.egg-info/dependency_links.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      183 2023-04-23 14:53:37.000000 metaseg-0.7.0/metaseg.egg-info/requires.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        8 2023-04-23 14:53:37.000000 metaseg-0.7.0/metaseg.egg-info/top_level.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)       80 2023-04-20 11:50:36.000000 metaseg-0.7.0/pyproject.toml
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      158 2023-04-23 14:51:06.000000 metaseg-0.7.0/requirements.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      430 2023-04-23 14:53:37.573963 metaseg-0.7.0/setup.cfg
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1529 2023-04-21 13:07:40.000000 metaseg-0.7.0/setup.py
```

### Comparing `metaseg-0.6.1/LICENSE` & `metaseg-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metaseg-0.6.1/PKG-INFO` & `metaseg-0.7.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaseg
-Version: 0.6.1
+Version: 0.7.0
 Home-page: https://github.com/kadirnar/segment-anything-pip
 Author: kadirnar
 License: Apache-2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: dev
@@ -33,28 +33,26 @@
 ### Usage
 ```python
 from metaseg import SegAutoMaskPredictor, SegManualMaskPredictor
 
 # If gpu memory is not enough, reduce the points_per_side and points_per_batch.
 
 # For image
-
 results = SegAutoMaskPredictor().image_predict(
     source="image.jpg",
     model_type="vit_l", # vit_l, vit_h, vit_b
     points_per_side=16, 
     points_per_batch=64,
     min_area=0,
     output_path="output.jpg",
     show=True,
     save=False,
 )
 
 # For video
-
 results = SegAutoMaskPredictor().video_predict(
     source="video.mp4",
     model_type="vit_l", # vit_l, vit_h, vit_b
     points_per_side=16, 
     points_per_batch=64,
     min_area=1000,
     output_path="output.mp4",
@@ -77,24 +75,23 @@
 
 # For video
 
 results = SegManualMaskPredictor().video_predict(
     source="test.mp4",
     model_type="vit_l", # vit_l, vit_h, vit_b
     input_point=[0, 0, 100, 100]
-    input_label=N
+    input_label=[0, 1],
     input_box=None,
     multimask_output=False,
     random_color=False,
     output_path="output.mp4",
 )
 ```
-```
 
-### SAHI + Segment Anything
+### [SAHI](https://github.com/obss/sahi) + Segment Anything
 
 ```python
 from metaseg import sahi_sliced_predict, SahiAutoSegmentation
 
 image_path = "test.jpg"
 boxes = sahi_sliced_predict(
     image_path=image_path,
@@ -116,14 +113,49 @@
     random_color=False,
     show=True,
     save=False,
 )
 ```
 <img width="700" alt="teaser" src="https://github.com/kadirnar/segment-anything-pip/releases/download/v0.5.0/sahi_autoseg.png">
 
+### [FalAI(Cloud GPU)](https://docs.fal.ai/fal-serverless/quickstart) + Segment Anything
+```bash
+pip install fal_serverless
+```
+
+```python
+# For Auto Mask
+from metaseg import falai_automask_image
+
+image = falai_automask_image(
+    image_path="data.jpg",
+    model_type="vit_b",
+    points_per_side=16,
+    points_per_batch=32,
+    min_area=0,
+)   
+image.show() # Show image
+image.save("output.jpg") # Save image
+
+# For Manual Mask
+from metaseg import falai_manualmask_image
+
+image = falai_manualmask_image(
+    image_path="data.jpg",
+    model_type="vit_b",
+    input_point=[[100, 100], [200, 200]],
+    input_label=[0, 1],
+    input_box=[100, 100, 200, 200], # or [[100, 100, 200, 200], [100, 100, 200, 200]]
+    multimask_output=False,
+    random_color=False,
+)
+image.show() # Show image
+image.save("output.jpg") # Save image
+```
 # Extra Features
 
 - [x] Support for Yolov5/8, Detectron2, Mmdetection, Torchvision models
 - [x] Support for video and web application(Huggingface Spaces)
 - [x] Support for manual single multi box and point selection
 - [x] Support for pip installation
 - [x] Support for SAHI library
+- [x] Support for FalAI
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: metaseg Version: 0.6.1 Home-page: https://
+Metadata-Version: 2.1 Name: metaseg Version: 0.7.0 Home-page: https://
 github.com/kadirnar/segment-anything-pip Author: kadirnar License: Apache-2.0
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 all Provides-Extra: dev License-File: LICENSE
    ***** MetaSeg: Packaged version of the Segment Anything repository *****
                                    [teaser]
                 [downloads] [pypi_version] [HuggingFace_Spaces]
 This repo is a packaged version of the [segment-anything](https://github.com/
@@ -18,21 +18,32 @@
 output_path="output.mp4", ) # For manuel box and point selection # For image
 results = SegManualMaskPredictor().image_predict( source="image.jpg",
 model_type="vit_l", # vit_l, vit_h, vit_b input_point=[[100, 100], [200, 200]],
 input_label=[0, 1], input_box=[100, 100, 200, 200], # or [[100, 100, 200, 200],
 [100, 100, 200, 200]] multimask_output=False, random_color=False, show=True,
 save=False, ) # For video results = SegManualMaskPredictor().video_predict
 ( source="test.mp4", model_type="vit_l", # vit_l, vit_h, vit_b input_point=[0,
-0, 100, 100] input_label=N input_box=None, multimask_output=False,
-random_color=False, output_path="output.mp4", ) ``` ``` ### SAHI + Segment
-Anything ```python from metaseg import sahi_sliced_predict,
-SahiAutoSegmentation image_path = "test.jpg" boxes = sahi_sliced_predict
-( image_path=image_path, detection_model_type="yolov5", #yolov8, detectron2,
-mmdetection, torchvision detection_model_path="yolov5l6.pt", conf_th=0.25,
-image_size=1280, slice_height=256, slice_width=256, overlap_height_ratio=0.2,
+0, 100, 100] input_label=[0, 1], input_box=None, multimask_output=False,
+random_color=False, output_path="output.mp4", ) ``` ### [SAHI](https://
+github.com/obss/sahi) + Segment Anything ```python from metaseg import
+sahi_sliced_predict, SahiAutoSegmentation image_path = "test.jpg" boxes =
+sahi_sliced_predict( image_path=image_path, detection_model_type="yolov5",
+#yolov8, detectron2, mmdetection, torchvision
+detection_model_path="yolov5l6.pt", conf_th=0.25, image_size=1280,
+slice_height=256, slice_width=256, overlap_height_ratio=0.2,
 overlap_width_ratio=0.2, ) SahiAutoSegmentation().predict( source=image_path,
 model_type="vit_b", input_box=boxes, multimask_output=False,
-random_color=False, show=True, save=False, ) ``` [teaser] # Extra Features -
-[x] Support for Yolov5/8, Detectron2, Mmdetection, Torchvision models - [x]
-Support for video and web application(Huggingface Spaces) - [x] Support for
-manual single multi box and point selection - [x] Support for pip installation
-- [x] Support for SAHI library
+random_color=False, show=True, save=False, ) ``` [teaser] ### [FalAI(Cloud
+GPU)](https://docs.fal.ai/fal-serverless/quickstart) + Segment Anything ```bash
+pip install fal_serverless ``` ```python # For Auto Mask from metaseg import
+falai_automask_image image = falai_automask_image( image_path="data.jpg",
+model_type="vit_b", points_per_side=16, points_per_batch=32, min_area=0, )
+image.show() # Show image image.save("output.jpg") # Save image # For Manual
+Mask from metaseg import falai_manualmask_image image = falai_manualmask_image
+( image_path="data.jpg", model_type="vit_b", input_point=[[100, 100], [200,
+200]], input_label=[0, 1], input_box=[100, 100, 200, 200], # or [[100, 100,
+200, 200], [100, 100, 200, 200]] multimask_output=False, random_color=False, )
+image.show() # Show image image.save("output.jpg") # Save image ``` # Extra
+Features - [x] Support for Yolov5/8, Detectron2, Mmdetection, Torchvision
+models - [x] Support for video and web application(Huggingface Spaces) - [x]
+Support for manual single multi box and point selection - [x] Support for pip
+installation - [x] Support for SAHI library - [x] Support for FalAI
```

### Comparing `metaseg-0.6.1/README.md` & `metaseg-0.7.0/metaseg.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: metaseg
+Version: 0.7.0
+Home-page: https://github.com/kadirnar/segment-anything-pip
+Author: kadirnar
+License: Apache-2.0
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: all
+Provides-Extra: dev
+License-File: LICENSE
+
 <div align="center">
 <h2>
      MetaSeg: Packaged version of the Segment Anything repository
 </h2>
 <div>
     <img width="1000" alt="teaser" src="https://github.com/kadirnar/segment-anything-pip/releases/download/v0.2.2/metaseg_demo.gif">
 </div>
@@ -21,28 +33,26 @@
 ### Usage
 ```python
 from metaseg import SegAutoMaskPredictor, SegManualMaskPredictor
 
 # If gpu memory is not enough, reduce the points_per_side and points_per_batch.
 
 # For image
-
 results = SegAutoMaskPredictor().image_predict(
     source="image.jpg",
     model_type="vit_l", # vit_l, vit_h, vit_b
     points_per_side=16, 
     points_per_batch=64,
     min_area=0,
     output_path="output.jpg",
     show=True,
     save=False,
 )
 
 # For video
-
 results = SegAutoMaskPredictor().video_predict(
     source="video.mp4",
     model_type="vit_l", # vit_l, vit_h, vit_b
     points_per_side=16, 
     points_per_batch=64,
     min_area=1000,
     output_path="output.mp4",
@@ -65,24 +75,23 @@
 
 # For video
 
 results = SegManualMaskPredictor().video_predict(
     source="test.mp4",
     model_type="vit_l", # vit_l, vit_h, vit_b
     input_point=[0, 0, 100, 100]
-    input_label=N
+    input_label=[0, 1],
     input_box=None,
     multimask_output=False,
     random_color=False,
     output_path="output.mp4",
 )
 ```
-```
 
-### SAHI + Segment Anything
+### [SAHI](https://github.com/obss/sahi) + Segment Anything
 
 ```python
 from metaseg import sahi_sliced_predict, SahiAutoSegmentation
 
 image_path = "test.jpg"
 boxes = sahi_sliced_predict(
     image_path=image_path,
@@ -104,14 +113,49 @@
     random_color=False,
     show=True,
     save=False,
 )
 ```
 <img width="700" alt="teaser" src="https://github.com/kadirnar/segment-anything-pip/releases/download/v0.5.0/sahi_autoseg.png">
 
+### [FalAI(Cloud GPU)](https://docs.fal.ai/fal-serverless/quickstart) + Segment Anything
+```bash
+pip install fal_serverless
+```
+
+```python
+# For Auto Mask
+from metaseg import falai_automask_image
+
+image = falai_automask_image(
+    image_path="data.jpg",
+    model_type="vit_b",
+    points_per_side=16,
+    points_per_batch=32,
+    min_area=0,
+)   
+image.show() # Show image
+image.save("output.jpg") # Save image
+
+# For Manual Mask
+from metaseg import falai_manualmask_image
+
+image = falai_manualmask_image(
+    image_path="data.jpg",
+    model_type="vit_b",
+    input_point=[[100, 100], [200, 200]],
+    input_label=[0, 1],
+    input_box=[100, 100, 200, 200], # or [[100, 100, 200, 200], [100, 100, 200, 200]]
+    multimask_output=False,
+    random_color=False,
+)
+image.show() # Show image
+image.save("output.jpg") # Save image
+```
 # Extra Features
 
 - [x] Support for Yolov5/8, Detectron2, Mmdetection, Torchvision models
 - [x] Support for video and web application(Huggingface Spaces)
 - [x] Support for manual single multi box and point selection
 - [x] Support for pip installation
 - [x] Support for SAHI library
+- [x] Support for FalAI
```

#### html2text {}

```diff
@@ -1,7 +1,11 @@
+Metadata-Version: 2.1 Name: metaseg Version: 0.7.0 Home-page: https://
+github.com/kadirnar/segment-anything-pip Author: kadirnar License: Apache-2.0
+Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
+all Provides-Extra: dev License-File: LICENSE
    ***** MetaSeg: Packaged version of the Segment Anything repository *****
                                    [teaser]
                 [downloads] [pypi_version] [HuggingFace_Spaces]
 This repo is a packaged version of the [segment-anything](https://github.com/
 facebookresearch/segment-anything) model. ### Installation ```bash pip install
 metaseg ``` ### Usage ```python from metaseg import SegAutoMaskPredictor,
 SegManualMaskPredictor # If gpu memory is not enough, reduce the
@@ -14,21 +18,32 @@
 output_path="output.mp4", ) # For manuel box and point selection # For image
 results = SegManualMaskPredictor().image_predict( source="image.jpg",
 model_type="vit_l", # vit_l, vit_h, vit_b input_point=[[100, 100], [200, 200]],
 input_label=[0, 1], input_box=[100, 100, 200, 200], # or [[100, 100, 200, 200],
 [100, 100, 200, 200]] multimask_output=False, random_color=False, show=True,
 save=False, ) # For video results = SegManualMaskPredictor().video_predict
 ( source="test.mp4", model_type="vit_l", # vit_l, vit_h, vit_b input_point=[0,
-0, 100, 100] input_label=N input_box=None, multimask_output=False,
-random_color=False, output_path="output.mp4", ) ``` ``` ### SAHI + Segment
-Anything ```python from metaseg import sahi_sliced_predict,
-SahiAutoSegmentation image_path = "test.jpg" boxes = sahi_sliced_predict
-( image_path=image_path, detection_model_type="yolov5", #yolov8, detectron2,
-mmdetection, torchvision detection_model_path="yolov5l6.pt", conf_th=0.25,
-image_size=1280, slice_height=256, slice_width=256, overlap_height_ratio=0.2,
+0, 100, 100] input_label=[0, 1], input_box=None, multimask_output=False,
+random_color=False, output_path="output.mp4", ) ``` ### [SAHI](https://
+github.com/obss/sahi) + Segment Anything ```python from metaseg import
+sahi_sliced_predict, SahiAutoSegmentation image_path = "test.jpg" boxes =
+sahi_sliced_predict( image_path=image_path, detection_model_type="yolov5",
+#yolov8, detectron2, mmdetection, torchvision
+detection_model_path="yolov5l6.pt", conf_th=0.25, image_size=1280,
+slice_height=256, slice_width=256, overlap_height_ratio=0.2,
 overlap_width_ratio=0.2, ) SahiAutoSegmentation().predict( source=image_path,
 model_type="vit_b", input_box=boxes, multimask_output=False,
-random_color=False, show=True, save=False, ) ``` [teaser] # Extra Features -
-[x] Support for Yolov5/8, Detectron2, Mmdetection, Torchvision models - [x]
-Support for video and web application(Huggingface Spaces) - [x] Support for
-manual single multi box and point selection - [x] Support for pip installation
-- [x] Support for SAHI library
+random_color=False, show=True, save=False, ) ``` [teaser] ### [FalAI(Cloud
+GPU)](https://docs.fal.ai/fal-serverless/quickstart) + Segment Anything ```bash
+pip install fal_serverless ``` ```python # For Auto Mask from metaseg import
+falai_automask_image image = falai_automask_image( image_path="data.jpg",
+model_type="vit_b", points_per_side=16, points_per_batch=32, min_area=0, )
+image.show() # Show image image.save("output.jpg") # Save image # For Manual
+Mask from metaseg import falai_manualmask_image image = falai_manualmask_image
+( image_path="data.jpg", model_type="vit_b", input_point=[[100, 100], [200,
+200]], input_label=[0, 1], input_box=[100, 100, 200, 200], # or [[100, 100,
+200, 200], [100, 100, 200, 200]] multimask_output=False, random_color=False, )
+image.show() # Show image image.save("output.jpg") # Save image ``` # Extra
+Features - [x] Support for Yolov5/8, Detectron2, Mmdetection, Torchvision
+models - [x] Support for video and web application(Huggingface Spaces) - [x]
+Support for manual single multi box and point selection - [x] Support for pip
+installation - [x] Support for SAHI library - [x] Support for FalAI
```

### Comparing `metaseg-0.6.1/metaseg/__init__.py` & `metaseg-0.7.0/metaseg/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 
 # This source code is licensed under the license found in the
 # LICENSE file in the root directory of this source tree.
 
+from metaseg.falai_demo import falai_automask_image, falai_manuelmask_image
 from metaseg.generator.automatic_mask_generator import SamAutomaticMaskGenerator
 from metaseg.generator.build_sam import build_sam, build_sam_vit_b, build_sam_vit_h, build_sam_vit_l, sam_model_registry
 from metaseg.generator.predictor import SamPredictor
 from metaseg.mask_predictor import SegAutoMaskPredictor, SegManualMaskPredictor
 from metaseg.sahi_predict import SahiAutoSegmentation, sahi_sliced_predict
 
-__version__ = "0.6.1"
+__version__ = "0.7.0"
```

### Comparing `metaseg-0.6.1/metaseg/generator/automatic_mask_generator.py` & `metaseg-0.7.0/metaseg/generator/automatic_mask_generator.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.6.1/metaseg/generator/build_sam.py` & `metaseg-0.7.0/metaseg/generator/build_sam.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.6.1/metaseg/generator/predictor.py` & `metaseg-0.7.0/metaseg/generator/predictor.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.6.1/metaseg/mask_predictor.py` & `metaseg-0.7.0/metaseg/mask_predictor.py`

 * *Files 2% similar despite different names*

```diff
@@ -240,33 +240,7 @@
             combined_mask = cv2.add(frame, mask_image)
             out.write(combined_mask)
 
         out.release()
         cap.release()
         cv2.destroyAllWindows()
         return output_path
-    
-if __name__ == "__main__":
-    # video
-    source = "test.mp4"
-    model_type = "sam_resnet50d_ade20k"
-    input_box = [0, 0, 100, 100]
-    input_point = None
-    input_label = None
-    multimask_output = False
-    output_path = "output.mp4"
-    random_color = False
-    show = False
-    save = True
-
-    # video
-    predictor = SegManualMaskPredictor()
-    predictor.video_predict(
-        source,
-        model_type,
-        input_box,
-        input_point,
-        input_label,
-        multimask_output,
-        output_path,
-        random_color,
-    )
```

### Comparing `metaseg-0.6.1/metaseg/modeling/common.py` & `metaseg-0.7.0/metaseg/modeling/common.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.6.1/metaseg/modeling/image_encoder.py` & `metaseg-0.7.0/metaseg/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.6.1/metaseg/modeling/mask_decoder.py` & `metaseg-0.7.0/metaseg/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.6.1/metaseg/modeling/prompt_encoder.py` & `metaseg-0.7.0/metaseg/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.6.1/metaseg/modeling/sam.py` & `metaseg-0.7.0/metaseg/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.6.1/metaseg/modeling/transformer.py` & `metaseg-0.7.0/metaseg/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.6.1/metaseg/sahi_predict.py` & `metaseg-0.7.0/metaseg/sahi_predict.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.6.1/metaseg/utils/amg.py` & `metaseg-0.7.0/metaseg/utils/amg.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.6.1/metaseg/utils/data_utils.py` & `metaseg-0.7.0/metaseg/utils/data_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,33 @@
     import cv2
 
     image = cv2.imread(image_path)
     image = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
     return image
 
 
+def load_server_image(image_path):
+    import os
+    from io import BytesIO
+    from uuid import uuid4
+
+    from PIL import Image
+
+    imagedir = str(uuid4())
+    os.system(f"mkdir -p {imagedir}")
+    image = Image.open(BytesIO(image_path))
+    if image.mode != "RGB":
+        image = image.convert("RGB")
+
+    image_path = f"{imagedir}/base_image_v0.png"
+    output_path = f"{imagedir}/output_v0.png"
+    image.save(image_path, format="PNG")
+    return image_path, output_path
+
+
 def load_video(video_path, output_path="output.mp4"):
     import cv2
 
     cap = cv2.VideoCapture(video_path)
     frame_width = int(cap.get(cv2.CAP_PROP_FRAME_WIDTH))
     frame_height = int(cap.get(cv2.CAP_PROP_FRAME_HEIGHT))
     fourcc = cv2.VideoWriter_fourcc(*"XVID")
```

### Comparing `metaseg-0.6.1/metaseg/utils/file_utils.py` & `metaseg-0.7.0/metaseg/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.6.1/metaseg/utils/onnx.py` & `metaseg-0.7.0/metaseg/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.6.1/metaseg/utils/transforms.py` & `metaseg-0.7.0/metaseg/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.6.1/metaseg/webapp/app.py` & `metaseg-0.7.0/metaseg/webapp/app.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.6.1/metaseg/webapp/demo.py` & `metaseg-0.7.0/metaseg/webapp/demo.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.6.1/metaseg.egg-info/PKG-INFO` & `metaseg-0.7.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: metaseg
-Version: 0.6.1
-Home-page: https://github.com/kadirnar/segment-anything-pip
-Author: kadirnar
-License: Apache-2.0
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: all
-Provides-Extra: dev
-License-File: LICENSE
-
 <div align="center">
 <h2>
      MetaSeg: Packaged version of the Segment Anything repository
 </h2>
 <div>
     <img width="1000" alt="teaser" src="https://github.com/kadirnar/segment-anything-pip/releases/download/v0.2.2/metaseg_demo.gif">
 </div>
@@ -33,28 +21,26 @@
 ### Usage
 ```python
 from metaseg import SegAutoMaskPredictor, SegManualMaskPredictor
 
 # If gpu memory is not enough, reduce the points_per_side and points_per_batch.
 
 # For image
-
 results = SegAutoMaskPredictor().image_predict(
     source="image.jpg",
     model_type="vit_l", # vit_l, vit_h, vit_b
     points_per_side=16, 
     points_per_batch=64,
     min_area=0,
     output_path="output.jpg",
     show=True,
     save=False,
 )
 
 # For video
-
 results = SegAutoMaskPredictor().video_predict(
     source="video.mp4",
     model_type="vit_l", # vit_l, vit_h, vit_b
     points_per_side=16, 
     points_per_batch=64,
     min_area=1000,
     output_path="output.mp4",
@@ -77,24 +63,23 @@
 
 # For video
 
 results = SegManualMaskPredictor().video_predict(
     source="test.mp4",
     model_type="vit_l", # vit_l, vit_h, vit_b
     input_point=[0, 0, 100, 100]
-    input_label=N
+    input_label=[0, 1],
     input_box=None,
     multimask_output=False,
     random_color=False,
     output_path="output.mp4",
 )
 ```
-```
 
-### SAHI + Segment Anything
+### [SAHI](https://github.com/obss/sahi) + Segment Anything
 
 ```python
 from metaseg import sahi_sliced_predict, SahiAutoSegmentation
 
 image_path = "test.jpg"
 boxes = sahi_sliced_predict(
     image_path=image_path,
@@ -116,14 +101,49 @@
     random_color=False,
     show=True,
     save=False,
 )
 ```
 <img width="700" alt="teaser" src="https://github.com/kadirnar/segment-anything-pip/releases/download/v0.5.0/sahi_autoseg.png">
 
+### [FalAI(Cloud GPU)](https://docs.fal.ai/fal-serverless/quickstart) + Segment Anything
+```bash
+pip install fal_serverless
+```
+
+```python
+# For Auto Mask
+from metaseg import falai_automask_image
+
+image = falai_automask_image(
+    image_path="data.jpg",
+    model_type="vit_b",
+    points_per_side=16,
+    points_per_batch=32,
+    min_area=0,
+)   
+image.show() # Show image
+image.save("output.jpg") # Save image
+
+# For Manual Mask
+from metaseg import falai_manualmask_image
+
+image = falai_manualmask_image(
+    image_path="data.jpg",
+    model_type="vit_b",
+    input_point=[[100, 100], [200, 200]],
+    input_label=[0, 1],
+    input_box=[100, 100, 200, 200], # or [[100, 100, 200, 200], [100, 100, 200, 200]]
+    multimask_output=False,
+    random_color=False,
+)
+image.show() # Show image
+image.save("output.jpg") # Save image
+```
 # Extra Features
 
 - [x] Support for Yolov5/8, Detectron2, Mmdetection, Torchvision models
 - [x] Support for video and web application(Huggingface Spaces)
 - [x] Support for manual single multi box and point selection
 - [x] Support for pip installation
 - [x] Support for SAHI library
+- [x] Support for FalAI
```

#### html2text {}

```diff
@@ -1,11 +1,7 @@
-Metadata-Version: 2.1 Name: metaseg Version: 0.6.1 Home-page: https://
-github.com/kadirnar/segment-anything-pip Author: kadirnar License: Apache-2.0
-Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
-all Provides-Extra: dev License-File: LICENSE
    ***** MetaSeg: Packaged version of the Segment Anything repository *****
                                    [teaser]
                 [downloads] [pypi_version] [HuggingFace_Spaces]
 This repo is a packaged version of the [segment-anything](https://github.com/
 facebookresearch/segment-anything) model. ### Installation ```bash pip install
 metaseg ``` ### Usage ```python from metaseg import SegAutoMaskPredictor,
 SegManualMaskPredictor # If gpu memory is not enough, reduce the
@@ -18,21 +14,32 @@
 output_path="output.mp4", ) # For manuel box and point selection # For image
 results = SegManualMaskPredictor().image_predict( source="image.jpg",
 model_type="vit_l", # vit_l, vit_h, vit_b input_point=[[100, 100], [200, 200]],
 input_label=[0, 1], input_box=[100, 100, 200, 200], # or [[100, 100, 200, 200],
 [100, 100, 200, 200]] multimask_output=False, random_color=False, show=True,
 save=False, ) # For video results = SegManualMaskPredictor().video_predict
 ( source="test.mp4", model_type="vit_l", # vit_l, vit_h, vit_b input_point=[0,
-0, 100, 100] input_label=N input_box=None, multimask_output=False,
-random_color=False, output_path="output.mp4", ) ``` ``` ### SAHI + Segment
-Anything ```python from metaseg import sahi_sliced_predict,
-SahiAutoSegmentation image_path = "test.jpg" boxes = sahi_sliced_predict
-( image_path=image_path, detection_model_type="yolov5", #yolov8, detectron2,
-mmdetection, torchvision detection_model_path="yolov5l6.pt", conf_th=0.25,
-image_size=1280, slice_height=256, slice_width=256, overlap_height_ratio=0.2,
+0, 100, 100] input_label=[0, 1], input_box=None, multimask_output=False,
+random_color=False, output_path="output.mp4", ) ``` ### [SAHI](https://
+github.com/obss/sahi) + Segment Anything ```python from metaseg import
+sahi_sliced_predict, SahiAutoSegmentation image_path = "test.jpg" boxes =
+sahi_sliced_predict( image_path=image_path, detection_model_type="yolov5",
+#yolov8, detectron2, mmdetection, torchvision
+detection_model_path="yolov5l6.pt", conf_th=0.25, image_size=1280,
+slice_height=256, slice_width=256, overlap_height_ratio=0.2,
 overlap_width_ratio=0.2, ) SahiAutoSegmentation().predict( source=image_path,
 model_type="vit_b", input_box=boxes, multimask_output=False,
-random_color=False, show=True, save=False, ) ``` [teaser] # Extra Features -
-[x] Support for Yolov5/8, Detectron2, Mmdetection, Torchvision models - [x]
-Support for video and web application(Huggingface Spaces) - [x] Support for
-manual single multi box and point selection - [x] Support for pip installation
-- [x] Support for SAHI library
+random_color=False, show=True, save=False, ) ``` [teaser] ### [FalAI(Cloud
+GPU)](https://docs.fal.ai/fal-serverless/quickstart) + Segment Anything ```bash
+pip install fal_serverless ``` ```python # For Auto Mask from metaseg import
+falai_automask_image image = falai_automask_image( image_path="data.jpg",
+model_type="vit_b", points_per_side=16, points_per_batch=32, min_area=0, )
+image.show() # Show image image.save("output.jpg") # Save image # For Manual
+Mask from metaseg import falai_manualmask_image image = falai_manualmask_image
+( image_path="data.jpg", model_type="vit_b", input_point=[[100, 100], [200,
+200]], input_label=[0, 1], input_box=[100, 100, 200, 200], # or [[100, 100,
+200, 200], [100, 100, 200, 200]] multimask_output=False, random_color=False, )
+image.show() # Show image image.save("output.jpg") # Save image ``` # Extra
+Features - [x] Support for Yolov5/8, Detectron2, Mmdetection, Torchvision
+models - [x] Support for video and web application(Huggingface Spaces) - [x]
+Support for manual single multi box and point selection - [x] Support for pip
+installation - [x] Support for SAHI library - [x] Support for FalAI
```

### Comparing `metaseg-0.6.1/metaseg.egg-info/SOURCES.txt` & `metaseg-0.7.0/metaseg.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 MANIFEST.in
 README.md
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 metaseg/__init__.py
+metaseg/falai_demo.py
 metaseg/mask_predictor.py
 metaseg/sahi_predict.py
 metaseg.egg-info/PKG-INFO
 metaseg.egg-info/SOURCES.txt
 metaseg.egg-info/dependency_links.txt
 metaseg.egg-info/requires.txt
 metaseg.egg-info/top_level.txt
```

### Comparing `metaseg-0.6.1/setup.py` & `metaseg-0.7.0/setup.py`

 * *Files identical despite different names*

