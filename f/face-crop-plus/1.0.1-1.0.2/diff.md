# Comparing `tmp/face-crop-plus-1.0.1.tar.gz` & `tmp/face-crop-plus-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "face-crop-plus-1.0.1.tar", last modified: Sun Apr 23 12:51:30 2023, max compression
+gzip compressed data, was "face-crop-plus-1.0.2.tar", last modified: Sun Apr 23 13:55:38 2023, max compression
```

## Comparing `face-crop-plus-1.0.1.tar` & `face-crop-plus-1.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:51:30.255117 face-crop-plus-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-23 12:51:16.000000 face-crop-plus-1.0.1/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)    20817 2023-04-23 12:51:30.255117 face-crop-plus-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19800 2023-04-23 12:51:16.000000 face-crop-plus-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 12:51:30.255117 face-crop-plus-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-04-23 12:51:16.000000 face-crop-plus-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:51:30.251117 face-crop-plus-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:51:30.251117 face-crop-plus-1.0.1/src/face_crop_plus/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-23 12:51:16.000000 face-crop-plus-1.0.1/src/face_crop_plus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10366 2023-04-23 12:51:16.000000 face-crop-plus-1.0.1/src/face_crop_plus/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42905 2023-04-23 12:51:16.000000 face-crop-plus-1.0.1/src/face_crop_plus/cropper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:51:30.251117 face-crop-plus-1.0.1/src/face_crop_plus/models/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-23 12:51:16.000000 face-crop-plus-1.0.1/src/face_crop_plus/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13019 2023-04-23 12:51:16.000000 face-crop-plus-1.0.1/src/face_crop_plus/models/_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    19842 2023-04-23 12:51:16.000000 face-crop-plus-1.0.1/src/face_crop_plus/models/bise.py
--rw-r--r--   0 runner    (1001) docker     (123)    21126 2023-04-23 12:51:16.000000 face-crop-plus-1.0.1/src/face_crop_plus/models/retinaface.py
--rw-r--r--   0 runner    (1001) docker     (123)     6289 2023-04-23 12:51:16.000000 face-crop-plus-1.0.1/src/face_crop_plus/models/rrdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    11459 2023-04-23 12:51:16.000000 face-crop-plus-1.0.1/src/face_crop_plus/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:51:30.251117 face-crop-plus-1.0.1/src/face_crop_plus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20817 2023-04-23 12:51:30.000000 face-crop-plus-1.0.1/src/face_crop_plus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-23 12:51:30.000000 face-crop-plus-1.0.1/src/face_crop_plus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 12:51:30.000000 face-crop-plus-1.0.1/src/face_crop_plus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-23 12:51:30.000000 face-crop-plus-1.0.1/src/face_crop_plus.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-23 12:51:30.000000 face-crop-plus-1.0.1/src/face_crop_plus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-23 12:51:30.000000 face-crop-plus-1.0.1/src/face_crop_plus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:55:38.096177 face-crop-plus-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-23 13:55:27.000000 face-crop-plus-1.0.2/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)    23703 2023-04-23 13:55:38.096177 face-crop-plus-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22696 2023-04-23 13:55:27.000000 face-crop-plus-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 13:55:38.096177 face-crop-plus-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-23 13:55:27.000000 face-crop-plus-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:55:38.092177 face-crop-plus-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:55:38.092177 face-crop-plus-1.0.2/src/face_crop_plus/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-23 13:55:27.000000 face-crop-plus-1.0.2/src/face_crop_plus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10366 2023-04-23 13:55:27.000000 face-crop-plus-1.0.2/src/face_crop_plus/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42905 2023-04-23 13:55:27.000000 face-crop-plus-1.0.2/src/face_crop_plus/cropper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:55:38.096177 face-crop-plus-1.0.2/src/face_crop_plus/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-23 13:55:27.000000 face-crop-plus-1.0.2/src/face_crop_plus/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13019 2023-04-23 13:55:27.000000 face-crop-plus-1.0.2/src/face_crop_plus/models/_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19842 2023-04-23 13:55:27.000000 face-crop-plus-1.0.2/src/face_crop_plus/models/bise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21126 2023-04-23 13:55:27.000000 face-crop-plus-1.0.2/src/face_crop_plus/models/retinaface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6289 2023-04-23 13:55:27.000000 face-crop-plus-1.0.2/src/face_crop_plus/models/rrdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11459 2023-04-23 13:55:27.000000 face-crop-plus-1.0.2/src/face_crop_plus/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:55:38.092177 face-crop-plus-1.0.2/src/face_crop_plus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23703 2023-04-23 13:55:38.000000 face-crop-plus-1.0.2/src/face_crop_plus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-23 13:55:38.000000 face-crop-plus-1.0.2/src/face_crop_plus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 13:55:38.000000 face-crop-plus-1.0.2/src/face_crop_plus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-23 13:55:38.000000 face-crop-plus-1.0.2/src/face_crop_plus.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-23 13:55:38.000000 face-crop-plus-1.0.2/src/face_crop_plus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-23 13:55:38.000000 face-crop-plus-1.0.2/src/face_crop_plus.egg-info/top_level.txt
```

### Comparing `face-crop-plus-1.0.1/LICENCE` & `face-crop-plus-1.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `face-crop-plus-1.0.1/PKG-INFO` & `face-crop-plus-1.0.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,18 @@
-Metadata-Version: 2.1
-Name: face-crop-plus
-Version: 1.0.1
-Summary: Automatic face aligner and cropper with quality enhancement and attribute parsing.
-Home-page: https://github.com/mantasu/face-crop-plus
-Author: mantasu (Mantas Birškus)
-Author-email: mantix7@gmail.com
-License: MIT
-Project-URL: Documentation, https://mantasu.github.io/face-crop-plus
-Project-URL: Bug Tracker, https://github.com/mantasu/face-crop-plus/issues
-Keywords: face,python,pytorch,alignment,cropping,super resolution,quality enhancement,parsing,grouping,attributes,mask,segmentation,celeba
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENCE
-
 # Face Crop Plus
 
 [![DOI](https://zenodo.org/badge/621262834.svg)](https://zenodo.org/badge/latestdoi/621262834)
 [![PyPI](https://img.shields.io/pypi/v/face-crop-plus?color=orange)](https://pypi.org/project/face-crop-plus/)
 [![Python: 3.10](https://img.shields.io/badge/python-3.10-brightgreen)](https://www.python.org/downloads/release/python-3100/)
 [![CUDA: yes](https://img.shields.io/badge/cuda-yes-green)](https://developer.nvidia.com/cuda-toolkit)
 [![License: MIT](https://img.shields.io/badge/license-MIT-lightgrey.svg)](https://opensource.org/licenses/MIT)
 
 <p align="center" width="100%">
 
-![Banner](assets/banner.png)
+![Banner](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/banner.png)
 
 </p>
 
 ## About
 
 Image preprocessing package for automatic face alignment and cropping with additional features. It provides the following functionality:
 1. **Face cropping** - face alignment and center-cropping using facial landmarks. Landmarks can be automatically predicted or, if they are already know, can be supplied through a separate file. It is possible to specify face factor, i.e., face area relative to the cropped image, and face extraction strategy, e.g., all faces or largest face per image.
@@ -72,15 +50,15 @@
 ```python
 from face_crop_plus import Cropper
 
 cropper = Cropper(face_factor=0.7, strategy="largest")
 cropper.process_dir(input_dir="path/to/images")
 ```
 
-For a quick demo, you can experiment with [demo.py](demo/demo.py) file:
+For a quick demo, you can experiment with [demo.py](https://github.com/mantasu/face-crop-plus/blob/main/demo/demo.py) file:
 ```bash
 git clone https://github.com/mantasu/face-crop-plus
 cd face-crop-plus/demo
 python demo.py
 ```
 
 For more examples, see _Examples_ section.
@@ -95,69 +73,69 @@
 
 * `landmarks` - if you don't want automatic landmark prediction and already have face landmark coordinates in a separate file, you can specify the path to it. See the table below for the expected file formats.
 
     | File format      | Description                                                                                                                                                                          |
     | :--------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
     | `.json`          | Expects a dictionary with the following example entries: `'image.jpg': [x1, y1, ...]`. I.e., keys are image file names and values are flattened arrays of face landmark coordinates. |
     | `.csv`           | Expects comma-separated values of where each line is of the form `image.jpg,x1,y1,...`. Note that it also expects the first line to be a header.                                     |
-    | `.txt` and other | Similar to CSV file, but each line is expected to have space-separated values of the form `image.jpg x1 y1 ...`. No header is expected.                                             |
+    | `.txt` and other | Similar to CSV file, but each line is expected to have space-separated values of the form `image.jpg x1 y1 ...`. No header is expected.                                              |
 
 * `output_size` - the output size of the cropped face images. Can be either a tuple of 2 values (weight, height) or a single value indicating square dimensions
 
     | 200 × 200                           | 300 × 300                           | 300 × 200                           | 200 × 300                           |
     | :---------------------------------: | :---------------------------------: | :---------------------------------: | :---------------------------------: |
-    | ![200x200](assets/size_200x200.jpg) | ![300x300](assets/size_300x300.jpg) | ![300x200](assets/size_300x200.jpg) | ![200x300](assets/size_200x300.jpg) |
+    | ![200x200](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/size_200x200.jpg) | ![300x300](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/size_300x300.jpg) | ![300x200](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/size_300x200.jpg) | ![200x300](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/size_200x300.jpg) |
 
 * `face_factor` - the fraction of the face area relative to the output image. The value is between 0 and 1 and, the larger the value, the larger the face is in the output image.
 
     | 0.4                           | 0.55                            | 0.7                            | 0.85                            |
     | :---------------------------: | :-----------------------------: | :----------------------------: | :-----------------------------: |
-    | ![0.4](assets/factor_0.4.jpg) | ![0.55](assets/factor_0.55.jpg) | ![0.55](assets/factor_0.7.jpg) | ![0.55](assets/factor_0.85.jpg) |
+    | ![0.4](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/factor_0.4.jpg) | ![0.55](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/factor_0.55.jpg) | ![0.55](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/factor_0.7.jpg) | ![0.55](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/factor_0.85.jpg) |
 
 * `padding` - the type of padding (border mode) to apply after cropping the images. If faces are near edges, the empty areas after aligning those faces will be filled with some values. This could be _constant_ (leave black), _replicate_ (repeat the last value of the edge in the original image), _reflect_ (mirror the values before the edge).
 
-    | Constant                                 | Replicate                                  | Reflect                                | Wrap                             |
-    | :--------------------------------------: | :----------------------------------------: | :------------------------------------: | :------------------------------: |
-    | ![constant](assets/padding_constant.jpg) | ![replicate](assets/padding_replicate.jpg) | ![reflect](assets/padding_reflect.jpg) | ![wrap](assets/padding_wrap.jpg) |
+    | Constant                                                                                               | Replicate                                                                                                | Reflect                                                                                              | Wrap                                                                                           |
+    | :----------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------: | :--------------------------------------------------------------------------------------------------: | :--------------------------------------------------------------------------------------------: |
+    | ![constant](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/padding_constant.jpg) | ![replicate](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/padding_replicate.jpg) | ![reflect](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/padding_reflect.jpg) | ![wrap](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/padding_wrap.jpg) |
 
 * `det_threshold` - if automatic detection is desired, then detection threshold, which is a value between 0 and 1, can be specified to indicate when the detected face should be considered an actual face. Lower values allow more faces to be extracted, however they can be blurry and not non-primary, e.g., the ones in the background. Higher values only alow clear faces to be considered. It only makes sense to play around with this parameter when `strategy` is specified to return more than one face, e.g., _all_. For example, if it is `0.999`, the blurry face in the background in the examples above is not detected, however if the threshold `0.998`, the face is still detected. For blurrier images, thresholds may differ.
 
 * `strategy` - the strategy to apply for cropping out images. This can be set to _all_, if all faces should be extracted from each image (suffixes will be added to each file name), _largest_, if only the largest faces should be considered (slowest), _best_ if only the first face (which has the best confidence score) per image should be considered.
 
 ### Quality Enhancement
 
 Quality enhancement feature allows to restore blurry faces. It has one main argument:
 
 * `enh_threshold` - quality enhancement threshold that tells when the image quality should be enhanced. It is the minimum average face factor, i.e., face area relative to the image, below which the whole image is enhanced. Note that quality enhancement is an expensive operation, thus set this to a low value, like `0.01` to only enhance images where faces are actually small. If your images are of reasonable quality and don't contain many tiny faces, you may want to set this to _None_ (or to a negative value if using command-line) to disable the model. Here are some of the examples of the extracted faces before and after enhancing the image:
 
     | Face 1                 | Face 2                 | Face 3                 | Face 4                 |
     | :--------------------: | :--------------------: | :--------------------: | :--------------------: |
-    | ![b1](assets/f1_b.jpg) | ![b2](assets/f2_b.jpg) | ![b3](assets/f3_b.jpg) | ![b6](assets/f4_b.jpg) |
-    | ![a1](assets/f1_a.jpg) | ![a2](assets/f2_a.jpg) | ![a3](assets/f3_a.jpg) | ![a6](assets/f4_a.jpg) |
+    | ![b1](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/f1_b.jpg) | ![b2](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/f2_b.jpg) | ![b3](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/f3_b.jpg) | ![b6](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/f4_b.jpg) |
+    | ![a1](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/f1_a.jpg) | ![a2](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/f2_a.jpg) | ![a3](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/f3_a.jpg) | ![a6](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/f4_a.jpg) |
 
 
 > Quality enhancement can be used as a separate feature to enhance images that contain faces. For an end user, it is a useful feature to boost the quality of photos. It is not suggested to enhance ultra high resolution images (>2000) because your GPU will explode. See _Pure Enhancement/Parsing_ section on how to run it as a stand-alone.
 
 
 ### Attribute Parsing
 
 Face parsing to attributes allows to group output images by category and generate attribute masks for that category. Categorized images are put to their corresponding sub-folders in the output directory.
 * `attr_groups` - dictionary specifying attribute groups, based on which the face images should be grouped. Each key represents an attribute group name, e.g., _glasses_, _earings and neckless_, _no accessories_, and each value represents attribute indices, e.g., `[6]`, `[9, 15]`, `[-6, -9, -15, -18]`, each index mapping to some attribute. Since this model labels face image pixels, if there is enough pixels with the specified values in the list, the whole face image will be put into that attribute category. For negative values, it will be checked that the labeled face image does not contain those (absolute) values. If it is None, then there will be no grouping according to attributes. Here are some group examples with 2 sample images per group:
 
     | Glasses <br/> `[6]`           | Earrings and neckless <br/> `[9, 15]`       | Hats, no glasses <br/> `[18, -6]`     | No accessories <br/> `[-6, -9, -15, -18]` |
     | :---------------------------: | :-----------------------------------------: | :-----------------------------------: | :---------------------------------------: |
-    | ![ag11](assets/glasses_1.jpg) | ![ag21](assets/earrings_and_neckless_1.jpg) | ![ag31](assets/hats_no_glasses_1.jpg) | ![ag31](assets/no_accessories_1.jpg)      |
-    | ![ag12](assets/glasses_2.jpg) | ![ag21](assets/earrings_and_neckless_2.jpg) | ![ag31](assets/hats_no_glasses_2.jpg) | ![ag31](assets/no_accessories_2.jpg)      |
+    | ![ag11](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/glasses_1.jpg) | ![ag21](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/earrings_and_neckless_1.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/hats_no_glasses_1.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/no_accessories_1.jpg)      |
+    | ![ag12](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/glasses_2.jpg) | ![ag21](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/earrings_and_neckless_2.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/hats_no_glasses_2.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/no_accessories_2.jpg)      |
 
 * `mask_groups` - Dictionary specifying mask groups, based on which the face images and their masks should be grouped. Each key represents a mask group name, e.g., _nose_, _eyes and eyebrows_, and each value represents attribute indices, e.g., `[10]`, `[2, 3, 4, 5]`, each index mapping to some attribute. Since this model labels face image pixels, a mask will be created with 255 (white) at pixels that match the specified attributes and zeros (black) elsewhere. Note that negative values would make no sense here and having them would cause an error. Images are saved to sub-directories named by the mask group and masks are saved to sub-directories under the same name, except with `_mask` suffix. If it is None, then there will be no grouping according to mask groups. Here are some group examples with 1 sample image and its mask per group (for consistency, same images as before):
 
     | Glasses <br/> `[6]`           | Earrings and neckless <br/> `[9, 15]`       | Nose <br/> `[10]`                     | Eyes and eyebrows <br/> `[2, 3, 4, 5]` |
     | :---------------------------: | :-----------------------------------------: | :-----------------------------------: | :------------------------------------: |
-    | ![ag11](assets/glasses_1.jpg) | ![ag21](assets/earrings_and_neckless_1.jpg) | ![ag31](assets/hats_no_glasses_1.jpg) | ![ag31](assets/no_accessories_1.jpg)   |
-    | ![ag11](assets/glasses_m.jpg) | ![ag21](assets/earrings_and_neckless_m.jpg) | ![ag31](assets/hats_no_glasses_m.jpg) | ![ag31](assets/no_accessories_m.jpg)   |
+    | ![ag11](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/glasses_1.jpg) | ![ag21](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/earrings_and_neckless_1.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/hats_no_glasses_1.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/no_accessories_1.jpg)   |
+    | ![ag11](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/glasses_m.jpg ) | ![ag21](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/earrings_and_neckless_m.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/hats_no_glasses_m.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/no_accessories_m.jpg)   |
 
 > If both `attr_groups` and `mask_groups` are specified, first images are grouped according to face attributes, then images in each groups are further sub-grouped to different mask groups (along with their masks).
 
 
 Here are the 19 possible face attributes (with `0` representing the neutral category):
 
 <p align="center" width="100%">
@@ -183,15 +161,15 @@
 ```
 
 You can specify the command-line arguments via JSON config file and provide the path to it. Further command-line arguments would overwrite the values taken from the JSON file.
 ```bash
 face-crop-plus --config path/to/json --attr-groups '{"glasses": [6]}'
 ```
 
-An example JSON config file is [demo.json](demo/demo.json). If you've cloned the repository, you can run from it:
+An example JSON config file is [demo.json](https://github.com/mantasu/face-crop-plus/blob/main/demo/demo.json). If you've cloned the repository, you can run from it:
 ```bash
 face-crop-plus --config demo/demo.json --device cuda:0 # overwrite device
 ```
 
 For all the available command line arguments, just type (although refer to documentation for more details):
 ```bash
 face-crop-plus -h
@@ -305,10 +283,10 @@
 @misc{face-crop-plus,
   author = {Mantas Birškus},
   title = {Face Crop Plus},
   year = {2023},
   publisher = {GitHub},
   journal = {GitHub repository},
   howpublished = {\url{https://github.com/mantasu/face-crop-plus}},
-  doi = {10.5281/zenodo.7856750}
+  doi = {10.5281/zenodo.7856908}
 }
-```
+```
```

### Comparing `face-crop-plus-1.0.1/setup.py` & `face-crop-plus-1.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,16 @@
-import subprocess
 import setuptools
 
-version = (
-    subprocess.run(["git", "describe", "--tags"], stdout=subprocess.PIPE)
-    .stdout.decode("utf-8")
-    .strip()[1:]
-)
-
 with open("README.md", "r", encoding = "utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name = "face-crop-plus",
-    version = version,
-    author = "mantasu (Mantas Birškus)",
+    version = "1.0.2",
+    author = "Mantas Birškus",
     author_email = "mantix7@gmail.com",
     license = "MIT",
     description = f"Automatic face aligner and cropper with quality "
                   f"enhancement and attribute parsing.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/mantasu/face-crop-plus",
```

### Comparing `face-crop-plus-1.0.1/src/face_crop_plus/__main__.py` & `face-crop-plus-1.0.2/src/face_crop_plus/__main__.py`

 * *Files identical despite different names*

### Comparing `face-crop-plus-1.0.1/src/face_crop_plus/cropper.py` & `face-crop-plus-1.0.2/src/face_crop_plus/cropper.py`

 * *Files identical despite different names*

### Comparing `face-crop-plus-1.0.1/src/face_crop_plus/models/_layers.py` & `face-crop-plus-1.0.2/src/face_crop_plus/models/_layers.py`

 * *Files identical despite different names*

### Comparing `face-crop-plus-1.0.1/src/face_crop_plus/models/bise.py` & `face-crop-plus-1.0.2/src/face_crop_plus/models/bise.py`

 * *Files identical despite different names*

### Comparing `face-crop-plus-1.0.1/src/face_crop_plus/models/retinaface.py` & `face-crop-plus-1.0.2/src/face_crop_plus/models/retinaface.py`

 * *Files identical despite different names*

### Comparing `face-crop-plus-1.0.1/src/face_crop_plus/models/rrdb.py` & `face-crop-plus-1.0.2/src/face_crop_plus/models/rrdb.py`

 * *Files identical despite different names*

### Comparing `face-crop-plus-1.0.1/src/face_crop_plus/utils.py` & `face-crop-plus-1.0.2/src/face_crop_plus/utils.py`

 * *Files identical despite different names*

### Comparing `face-crop-plus-1.0.1/src/face_crop_plus.egg-info/SOURCES.txt` & `face-crop-plus-1.0.2/src/face_crop_plus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

