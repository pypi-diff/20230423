# Comparing `tmp/superannotate-4.4.9.dev5.tar.gz` & `tmp/superannotate-4.4.9b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/superannotate-python-sdk/superannotate-python-sdk/dist/.tmp-sxnmud2y/superannotate-4.4.9.dev5.tar", last modified: Wed Jan 25 06:33:11 2023, max compression
+gzip compressed data, was "/home/runner/work/superannotate-python-sdk/superannotate-python-sdk/dist/.tmp-5ckskno5/superannotate-4.4.9b1.tar", last modified: Wed Jan 25 14:26:27 2023, max compression
```

## Comparing `superannotate-4.4.9.dev5.tar` & `superannotate-4.4.9b1.tar`

### file list

```diff
@@ -1,174 +1,174 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 06:33:11.000000 superannotate-4.4.9.dev5/
--rw-r--r--   0 runner    (1001) docker     (116)     1073 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      118 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     5425 2023-01-25 06:33:11.000000 superannotate-4.4.9.dev5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     4665 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/README.rst
--rw-r--r--   0 runner    (1001) docker     (116)      424 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-01-25 06:33:11.000000 superannotate-4.4.9.dev5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1651 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 06:33:11.000000 superannotate-4.4.9.dev5/src/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 06:33:11.000000 superannotate-4.4.9.dev5/src/superannotate/
--rw-r--r--   0 runner    (1001) docker     (116)     2847 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 06:33:11.000000 superannotate-4.4.9.dev5/src/superannotate/lib/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 06:33:11.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 06:33:11.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/analytics/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    22449 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/analytics/aggregators.py
--rw-r--r--   0 runner    (1001) docker     (116)     2403 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/analytics/class_analytics.py
--rw-r--r--   0 runner    (1001) docker     (116)    24976 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/analytics/common.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 06:33:11.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/bin/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      251 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/bin/superannotate.py
--rw-r--r--   0 runner    (1001) docker     (116)     2061 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/common.py
--rw-r--r--   0 runner    (1001) docker     (116)      115 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)     4218 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 06:33:11.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/
--rw-r--r--   0 runner    (1001) docker     (116)      296 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    17597 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 06:33:11.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     6956 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/baseStrategy.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 06:33:11.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/coco_converters/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/coco_converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3458 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/coco_converters/coco_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    10430 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/coco_converters/coco_converter.py
--rw-r--r--   0 runner    (1001) docker     (116)     6176 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/coco_converters/coco_strategies.py
--rw-r--r--   0 runner    (1001) docker     (116)     6295 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/coco_converters/coco_to_sa_pixel.py
--rw-r--r--   0 runner    (1001) docker     (116)     8738 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/coco_converters/coco_to_sa_vector.py
--rw-r--r--   0 runner    (1001) docker     (116)     2753 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/coco_converters/sa_pixel_to_coco.py
--rw-r--r--   0 runner    (1001) docker     (116)     7294 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/coco_converters/sa_vector_to_coco.py
--rw-r--r--   0 runner    (1001) docker     (116)     2708 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/converters.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 06:33:11.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/dataloop_converters/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/dataloop_converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      848 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/dataloop_converters/dataloop_helper.py
--rw-r--r--   0 runner    (1001) docker     (116)     1528 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/dataloop_converters/dataloop_strategies.py
--rw-r--r--   0 runner    (1001) docker     (116)     4560 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/dataloop_converters/dataloop_to_sa_vector.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 06:33:11.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/googlecloud_converters/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/googlecloud_converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      965 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/googlecloud_converters/googlecloud_strategies.py
--rw-r--r--   0 runner    (1001) docker     (116)     2087 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/googlecloud_converters/googlecloud_to_sa_vector.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 06:33:11.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/labelbox_converters/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/labelbox_converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4609 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/labelbox_converters/labelbox_helper.py
--rw-r--r--   0 runner    (1001) docker     (116)     1668 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/labelbox_converters/labelbox_strategies.py
--rw-r--r--   0 runner    (1001) docker     (116)     3499 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/labelbox_converters/labelbox_to_sa_pixel.py
--rw-r--r--   0 runner    (1001) docker     (116)     3809 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/labelbox_converters/labelbox_to_sa_vector.py
--rw-r--r--   0 runner    (1001) docker     (116)     2193 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/sa_json_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 06:33:11.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/sagemaker_converters/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/sagemaker_converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1323 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/sagemaker_converters/sagemaker_strategies.py
--rw-r--r--   0 runner    (1001) docker     (116)     4711 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/sagemaker_converters/sagemaker_to_sa_pixel.py
--rw-r--r--   0 runner    (1001) docker     (116)     3027 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/sagemaker_converters/sagemaker_to_sa_vector.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 06:33:11.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/supervisely_converters/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/supervisely_converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      931 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/supervisely_converters/supervisely_helper.py
--rw-r--r--   0 runner    (1001) docker     (116)     2740 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/supervisely_converters/supervisely_strategies.py
--rw-r--r--   0 runner    (1001) docker     (116)     3743 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/supervisely_converters/supervisely_to_sa_pixel.py
--rw-r--r--   0 runner    (1001) docker     (116)     8471 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/supervisely_converters/supervisely_to_sa_vector.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 06:33:11.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/vgg_converters/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/vgg_converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1204 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/vgg_converters/vgg_helper.py
--rw-r--r--   0 runner    (1001) docker     (116)     1449 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/vgg_converters/vgg_strategies.py
--rw-r--r--   0 runner    (1001) docker     (116)     5291 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/vgg_converters/vgg_to_sa_vector.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 06:33:11.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/voc_converters/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/voc_converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1767 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/voc_converters/voc_helper.py
--rw-r--r--   0 runner    (1001) docker     (116)     2210 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/voc_converters/voc_strategies.py
--rw-r--r--   0 runner    (1001) docker     (116)     4610 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/voc_converters/voc_to_sa_pixel.py
--rw-r--r--   0 runner    (1001) docker     (116)     5757 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/voc_converters/voc_to_sa_vector.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 06:33:11.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/vott_converters/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/vott_converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1323 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/vott_converters/vott_strategies.py
--rw-r--r--   0 runner    (1001) docker     (116)     2778 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/vott_converters/vott_to_sa_vector.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 06:33:11.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/yolo_converters/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/yolo_converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      879 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/yolo_converters/yolo_strategies.py
--rw-r--r--   0 runner    (1001) docker     (116)     2815 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/yolo_converters/yolo_to_sa_vector.py
--rw-r--r--   0 runner    (1001) docker     (116)     2690 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/export_from_sa_conversions.py
--rw-r--r--   0 runner    (1001) docker     (116)     1521 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/import_to_sa_conversions.py
--rw-r--r--   0 runner    (1001) docker     (116)    11925 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/sa_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 06:33:11.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/interface/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     6799 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/interface/base_interface.py
--rw-r--r--   0 runner    (1001) docker     (116)    10101 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/interface/cli_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 06:33:11.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/interface/sdk/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/interface/sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/interface/sdk/folders.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/interface/sdk/project.py
--rw-r--r--   0 runner    (1001) docker     (116)   117554 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/interface/sdk_interface.py
--rw-r--r--   0 runner    (1001) docker     (116)     7158 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/interface/types.py
--rw-r--r--   0 runner    (1001) docker     (116)     5872 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 06:33:11.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/server/
--rw-r--r--   0 runner    (1001) docker     (116)      622 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/server/__app.py
--rw-r--r--   0 runner    (1001) docker     (116)      119 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)       77 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/server/__wsgi.py
--rw-r--r--   0 runner    (1001) docker     (116)     8584 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/server/core.py
--rw-r--r--   0 runner    (1001) docker     (116)     1656 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/server/default_app.py
--rw-r--r--   0 runner    (1001) docker     (116)      235 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/app/server/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 06:33:11.000000 superannotate-4.4.9.dev5/src/superannotate/lib/core/
--rw-r--r--   0 runner    (1001) docker     (116)     5389 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      964 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/core/base_usecases.py
--rw-r--r--   0 runner    (1001) docker     (116)     2698 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/core/conditions.py
--rw-r--r--   0 runner    (1001) docker     (116)     1689 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/core/config.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 06:33:11.000000 superannotate-4.4.9.dev5/src/superannotate/lib/core/entities/
--rw-r--r--   0 runner    (1001) docker     (116)     1714 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/core/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    10375 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/core/entities/base.py
--rw-r--r--   0 runner    (1001) docker     (116)     2774 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/core/entities/classes.py
--rw-r--r--   0 runner    (1001) docker     (116)      534 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/core/entities/folder.py
--rw-r--r--   0 runner    (1001) docker     (116)      408 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/core/entities/integrations.py
--rw-r--r--   0 runner    (1001) docker     (116)     1133 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/core/entities/items.py
--rw-r--r--   0 runner    (1001) docker     (116)     4681 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/core/entities/project.py
--rw-r--r--   0 runner    (1001) docker     (116)     1448 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/core/entities/project_entities.py
--rw-r--r--   0 runner    (1001) docker     (116)     4275 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/core/enums.py
--rw-r--r--   0 runner    (1001) docker     (116)      552 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)    10340 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/core/plugin.py
--rw-r--r--   0 runner    (1001) docker     (116)     4142 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/core/reporter.py
--rw-r--r--   0 runner    (1001) docker     (116)     1451 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/core/repositories.py
--rw-r--r--   0 runner    (1001) docker     (116)      988 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/core/response.py
--rw-r--r--   0 runner    (1001) docker     (116)     5161 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/core/service_types.py
--rw-r--r--   0 runner    (1001) docker     (116)    17717 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/core/serviceproviders.py
--rw-r--r--   0 runner    (1001) docker     (116)      697 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/core/types.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 06:33:11.000000 superannotate-4.4.9.dev5/src/superannotate/lib/core/usecases/
--rw-r--r--   0 runner    (1001) docker     (116)      543 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/core/usecases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    66927 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/core/usecases/annotations.py
--rw-r--r--   0 runner    (1001) docker     (116)     1863 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/core/usecases/base.py
--rw-r--r--   0 runner    (1001) docker     (116)     7861 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/core/usecases/classes.py
--rw-r--r--   0 runner    (1001) docker     (116)     5882 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/core/usecases/custom_fields.py
--rw-r--r--   0 runner    (1001) docker     (116)     7503 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/core/usecases/folders.py
--rw-r--r--   0 runner    (1001) docker     (116)    75503 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/core/usecases/images.py
--rw-r--r--   0 runner    (1001) docker     (116)     2951 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/core/usecases/integrations.py
--rw-r--r--   0 runner    (1001) docker     (116)    43309 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/core/usecases/items.py
--rw-r--r--   0 runner    (1001) docker     (116)    24950 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/core/usecases/models.py
--rw-r--r--   0 runner    (1001) docker     (116)    42426 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/core/usecases/projects.py
--rw-r--r--   0 runner    (1001) docker     (116)     9652 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/core/video_convertor.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 06:33:11.000000 superannotate-4.4.9.dev5/src/superannotate/lib/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/infrastructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    42270 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/infrastructure/controller.py
--rw-r--r--   0 runner    (1001) docker     (116)      739 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/infrastructure/helpers.py
--rw-r--r--   0 runner    (1001) docker     (116)     3063 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/infrastructure/repositories.py
--rw-r--r--   0 runner    (1001) docker     (116)     9482 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/infrastructure/serviceprovider.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 06:33:11.000000 superannotate-4.4.9.dev5/src/superannotate/lib/infrastructure/services/
--rw-r--r--   0 runner    (1001) docker     (116)      315 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/infrastructure/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    15430 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/infrastructure/services/annotation.py
--rw-r--r--   0 runner    (1001) docker     (116)     1906 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/infrastructure/services/annotation_class.py
--rw-r--r--   0 runner    (1001) docker     (116)     2002 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/infrastructure/services/custom_field.py
--rw-r--r--   0 runner    (1001) docker     (116)     2953 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/infrastructure/services/folder.py
--rw-r--r--   0 runner    (1001) docker     (116)     6821 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/infrastructure/services/http_client.py
--rw-r--r--   0 runner    (1001) docker     (116)     1074 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/infrastructure/services/integration.py
--rw-r--r--   0 runner    (1001) docker     (116)     7509 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/infrastructure/services/item.py
--rw-r--r--   0 runner    (1001) docker     (116)      808 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/infrastructure/services/models.py
--rw-r--r--   0 runner    (1001) docker     (116)     5511 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/infrastructure/services/project.py
--rw-r--r--   0 runner    (1001) docker     (116)     1994 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/infrastructure/services/subset.py
--rw-r--r--   0 runner    (1001) docker     (116)     5558 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/infrastructure/stream_data_handler.py
--rw-r--r--   0 runner    (1001) docker     (116)      972 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/infrastructure/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     1014 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/lib/infrastructure/validators.py
--rw-r--r--   0 runner    (1001) docker     (116)     2312 2023-01-25 06:32:56.000000 superannotate-4.4.9.dev5/src/superannotate/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 06:33:11.000000 superannotate-4.4.9.dev5/src/superannotate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     5425 2023-01-25 06:33:11.000000 superannotate-4.4.9.dev5/src/superannotate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     8706 2023-01-25 06:33:11.000000 superannotate-4.4.9.dev5/src/superannotate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-01-25 06:33:11.000000 superannotate-4.4.9.dev5/src/superannotate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       82 2023-01-25 06:33:11.000000 superannotate-4.4.9.dev5/src/superannotate.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)      424 2023-01-25 06:33:11.000000 superannotate-4.4.9.dev5/src/superannotate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       14 2023-01-25 06:33:11.000000 superannotate-4.4.9.dev5/src/superannotate.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 14:26:27.000000 superannotate-4.4.9b1/
+-rw-r--r--   0 runner    (1001) docker     (116)     1073 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)      118 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     5422 2023-01-25 14:26:27.000000 superannotate-4.4.9b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     4665 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      424 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2023-01-25 14:26:27.000000 superannotate-4.4.9b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1651 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 14:26:27.000000 superannotate-4.4.9b1/src/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 14:26:27.000000 superannotate-4.4.9b1/src/superannotate/
+-rw-r--r--   0 runner    (1001) docker     (116)     2845 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 14:26:27.000000 superannotate-4.4.9b1/src/superannotate/lib/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 14:26:27.000000 superannotate-4.4.9b1/src/superannotate/lib/app/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 14:26:27.000000 superannotate-4.4.9b1/src/superannotate/lib/app/analytics/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    22449 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/analytics/aggregators.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2403 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/analytics/class_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (116)    24976 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/analytics/common.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 14:26:27.000000 superannotate-4.4.9b1/src/superannotate/lib/app/bin/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      251 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/bin/superannotate.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2061 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/common.py
+-rw-r--r--   0 runner    (1001) docker     (116)      115 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4218 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 14:26:27.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/
+-rw-r--r--   0 runner    (1001) docker     (116)      296 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    17597 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 14:26:27.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6956 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/baseStrategy.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 14:26:27.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/coco_converters/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/coco_converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3458 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/coco_converters/coco_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10430 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/coco_converters/coco_converter.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6176 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/coco_converters/coco_strategies.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6295 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/coco_converters/coco_to_sa_pixel.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8738 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/coco_converters/coco_to_sa_vector.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2753 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/coco_converters/sa_pixel_to_coco.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7294 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/coco_converters/sa_vector_to_coco.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2708 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/converters.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 14:26:27.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/dataloop_converters/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/dataloop_converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      848 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/dataloop_converters/dataloop_helper.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1528 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/dataloop_converters/dataloop_strategies.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4560 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/dataloop_converters/dataloop_to_sa_vector.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 14:26:27.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/googlecloud_converters/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/googlecloud_converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      965 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/googlecloud_converters/googlecloud_strategies.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2087 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/googlecloud_converters/googlecloud_to_sa_vector.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 14:26:27.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/labelbox_converters/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/labelbox_converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4609 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/labelbox_converters/labelbox_helper.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1668 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/labelbox_converters/labelbox_strategies.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3499 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/labelbox_converters/labelbox_to_sa_pixel.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3809 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/labelbox_converters/labelbox_to_sa_vector.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2193 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/sa_json_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 14:26:27.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/sagemaker_converters/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/sagemaker_converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1323 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/sagemaker_converters/sagemaker_strategies.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4711 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/sagemaker_converters/sagemaker_to_sa_pixel.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3027 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/sagemaker_converters/sagemaker_to_sa_vector.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 14:26:27.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/supervisely_converters/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/supervisely_converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      931 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/supervisely_converters/supervisely_helper.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2740 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/supervisely_converters/supervisely_strategies.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3743 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/supervisely_converters/supervisely_to_sa_pixel.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8471 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/supervisely_converters/supervisely_to_sa_vector.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 14:26:27.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/vgg_converters/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/vgg_converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1204 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/vgg_converters/vgg_helper.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1449 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/vgg_converters/vgg_strategies.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5291 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/vgg_converters/vgg_to_sa_vector.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 14:26:27.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/voc_converters/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/voc_converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1767 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/voc_converters/voc_helper.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2210 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/voc_converters/voc_strategies.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4610 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/voc_converters/voc_to_sa_pixel.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5757 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/voc_converters/voc_to_sa_vector.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 14:26:27.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/vott_converters/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/vott_converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1323 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/vott_converters/vott_strategies.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2778 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/vott_converters/vott_to_sa_vector.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 14:26:27.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/yolo_converters/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/yolo_converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      879 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/yolo_converters/yolo_strategies.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2815 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/yolo_converters/yolo_to_sa_vector.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2690 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/export_from_sa_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1521 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/import_to_sa_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11925 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/sa_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 14:26:27.000000 superannotate-4.4.9b1/src/superannotate/lib/app/interface/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6799 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/interface/base_interface.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10101 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/interface/cli_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 14:26:27.000000 superannotate-4.4.9b1/src/superannotate/lib/app/interface/sdk/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/interface/sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/interface/sdk/folders.py
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/interface/sdk/project.py
+-rw-r--r--   0 runner    (1001) docker     (116)   117554 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/interface/sdk_interface.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7158 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/interface/types.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5872 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 14:26:27.000000 superannotate-4.4.9b1/src/superannotate/lib/app/server/
+-rw-r--r--   0 runner    (1001) docker     (116)      622 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/server/__app.py
+-rw-r--r--   0 runner    (1001) docker     (116)      119 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)       77 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/server/__wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8584 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/server/core.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1656 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/server/default_app.py
+-rw-r--r--   0 runner    (1001) docker     (116)      235 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/app/server/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 14:26:27.000000 superannotate-4.4.9b1/src/superannotate/lib/core/
+-rw-r--r--   0 runner    (1001) docker     (116)     5389 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      964 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/core/base_usecases.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2698 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/core/conditions.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1689 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/core/config.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 14:26:27.000000 superannotate-4.4.9b1/src/superannotate/lib/core/entities/
+-rw-r--r--   0 runner    (1001) docker     (116)     1714 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/core/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10375 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/core/entities/base.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2774 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/core/entities/classes.py
+-rw-r--r--   0 runner    (1001) docker     (116)      534 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/core/entities/folder.py
+-rw-r--r--   0 runner    (1001) docker     (116)      408 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/core/entities/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1133 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/core/entities/items.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4681 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/core/entities/project.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1448 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/core/entities/project_entities.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4275 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/core/enums.py
+-rw-r--r--   0 runner    (1001) docker     (116)      552 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10340 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/core/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4142 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/core/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1451 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/core/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (116)      988 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/core/response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5161 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/core/service_types.py
+-rw-r--r--   0 runner    (1001) docker     (116)    17717 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/core/serviceproviders.py
+-rw-r--r--   0 runner    (1001) docker     (116)      697 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/core/types.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 14:26:27.000000 superannotate-4.4.9b1/src/superannotate/lib/core/usecases/
+-rw-r--r--   0 runner    (1001) docker     (116)      543 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/core/usecases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    66927 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/core/usecases/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1863 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/core/usecases/base.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7861 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/core/usecases/classes.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5882 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/core/usecases/custom_fields.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7503 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/core/usecases/folders.py
+-rw-r--r--   0 runner    (1001) docker     (116)    75503 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/core/usecases/images.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2951 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/core/usecases/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (116)    43309 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/core/usecases/items.py
+-rw-r--r--   0 runner    (1001) docker     (116)    24950 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/core/usecases/models.py
+-rw-r--r--   0 runner    (1001) docker     (116)    42426 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/core/usecases/projects.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9652 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/core/video_convertor.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 14:26:27.000000 superannotate-4.4.9b1/src/superannotate/lib/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/infrastructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    42270 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/infrastructure/controller.py
+-rw-r--r--   0 runner    (1001) docker     (116)      739 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/infrastructure/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3063 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/infrastructure/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9482 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/infrastructure/serviceprovider.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 14:26:27.000000 superannotate-4.4.9b1/src/superannotate/lib/infrastructure/services/
+-rw-r--r--   0 runner    (1001) docker     (116)      315 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/infrastructure/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    15430 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/infrastructure/services/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1906 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/infrastructure/services/annotation_class.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2002 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/infrastructure/services/custom_field.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2953 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/infrastructure/services/folder.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6821 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/infrastructure/services/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1074 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/infrastructure/services/integration.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7509 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/infrastructure/services/item.py
+-rw-r--r--   0 runner    (1001) docker     (116)      808 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/infrastructure/services/models.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5511 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/infrastructure/services/project.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1994 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/infrastructure/services/subset.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5558 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/infrastructure/stream_data_handler.py
+-rw-r--r--   0 runner    (1001) docker     (116)      972 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/infrastructure/utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1014 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/lib/infrastructure/validators.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2312 2023-01-25 14:26:13.000000 superannotate-4.4.9b1/src/superannotate/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 14:26:27.000000 superannotate-4.4.9b1/src/superannotate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     5422 2023-01-25 14:26:27.000000 superannotate-4.4.9b1/src/superannotate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     8706 2023-01-25 14:26:27.000000 superannotate-4.4.9b1/src/superannotate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2023-01-25 14:26:27.000000 superannotate-4.4.9b1/src/superannotate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       82 2023-01-25 14:26:27.000000 superannotate-4.4.9b1/src/superannotate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      424 2023-01-25 14:26:27.000000 superannotate-4.4.9b1/src/superannotate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       14 2023-01-25 14:26:27.000000 superannotate-4.4.9b1/src/superannotate.egg-info/top_level.txt
```

### Comparing `superannotate-4.4.9.dev5/LICENSE` & `superannotate-4.4.9b1/LICENSE`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/PKG-INFO` & `superannotate-4.4.9b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superannotate
-Version: 4.4.9.dev5
+Version: 4.4.9b1
 Summary: Python SDK to SuperAnnotate platform
 Home-page: https://github.com/superannotateai/superannotate-python-sdk
 Author: SuperAnnotate AI
 Author-email: suppoort@superannotate.com
 License: MIT
 Project-URL: Documentation, https://superannotate.readthedocs.io/en/stable/
 Classifier: Programming Language :: Python
```

### Comparing `superannotate-4.4.9.dev5/README.rst` & `superannotate-4.4.9b1/README.rst`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/setup.py` & `superannotate-4.4.9b1/setup.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/__init__.py` & `superannotate-4.4.9b1/src/superannotate/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import sys
 import typing
 
-__version__ = "4.4.9dev5"
+__version__ = "4.4.9b1"
 
 sys.path.append(os.path.split(os.path.realpath(__file__))[0])
 
 import logging.config  # noqa
 import requests  # noqa
 from packaging.version import parse  # noqa
 from superannotate.lib.app.input_converters import convert_json_version  # noqa
```

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/app/analytics/aggregators.py` & `superannotate-4.4.9b1/src/superannotate/lib/app/analytics/aggregators.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/app/analytics/class_analytics.py` & `superannotate-4.4.9b1/src/superannotate/lib/app/analytics/class_analytics.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/app/analytics/common.py` & `superannotate-4.4.9b1/src/superannotate/lib/app/analytics/common.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/app/common.py` & `superannotate-4.4.9b1/src/superannotate/lib/app/common.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/app/helpers.py` & `superannotate-4.4.9b1/src/superannotate/lib/app/helpers.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/conversion.py` & `superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/conversion.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/baseStrategy.py` & `superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/baseStrategy.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/coco_converters/coco_api.py` & `superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/coco_converters/coco_api.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/coco_converters/coco_converter.py` & `superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/coco_converters/coco_converter.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/coco_converters/coco_strategies.py` & `superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/coco_converters/coco_strategies.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/coco_converters/coco_to_sa_pixel.py` & `superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/coco_converters/coco_to_sa_pixel.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/coco_converters/coco_to_sa_vector.py` & `superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/coco_converters/coco_to_sa_vector.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/coco_converters/sa_pixel_to_coco.py` & `superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/coco_converters/sa_pixel_to_coco.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/coco_converters/sa_vector_to_coco.py` & `superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/coco_converters/sa_vector_to_coco.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/converters.py` & `superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/converters.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/dataloop_converters/dataloop_helper.py` & `superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/dataloop_converters/dataloop_helper.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/dataloop_converters/dataloop_strategies.py` & `superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/dataloop_converters/dataloop_strategies.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/dataloop_converters/dataloop_to_sa_vector.py` & `superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/dataloop_converters/dataloop_to_sa_vector.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/googlecloud_converters/googlecloud_strategies.py` & `superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/googlecloud_converters/googlecloud_strategies.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/googlecloud_converters/googlecloud_to_sa_vector.py` & `superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/googlecloud_converters/googlecloud_to_sa_vector.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/labelbox_converters/labelbox_helper.py` & `superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/labelbox_converters/labelbox_helper.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/labelbox_converters/labelbox_strategies.py` & `superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/labelbox_converters/labelbox_strategies.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/labelbox_converters/labelbox_to_sa_pixel.py` & `superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/labelbox_converters/labelbox_to_sa_pixel.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/labelbox_converters/labelbox_to_sa_vector.py` & `superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/labelbox_converters/labelbox_to_sa_vector.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/sa_json_helper.py` & `superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/sa_json_helper.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/sagemaker_converters/sagemaker_strategies.py` & `superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/sagemaker_converters/sagemaker_strategies.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/sagemaker_converters/sagemaker_to_sa_pixel.py` & `superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/sagemaker_converters/sagemaker_to_sa_pixel.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/sagemaker_converters/sagemaker_to_sa_vector.py` & `superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/sagemaker_converters/sagemaker_to_sa_vector.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/supervisely_converters/supervisely_helper.py` & `superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/supervisely_converters/supervisely_helper.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/supervisely_converters/supervisely_strategies.py` & `superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/supervisely_converters/supervisely_strategies.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/supervisely_converters/supervisely_to_sa_pixel.py` & `superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/supervisely_converters/supervisely_to_sa_pixel.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/supervisely_converters/supervisely_to_sa_vector.py` & `superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/supervisely_converters/supervisely_to_sa_vector.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/vgg_converters/vgg_helper.py` & `superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/vgg_converters/vgg_helper.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/vgg_converters/vgg_strategies.py` & `superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/vgg_converters/vgg_strategies.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/vgg_converters/vgg_to_sa_vector.py` & `superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/vgg_converters/vgg_to_sa_vector.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/voc_converters/voc_helper.py` & `superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/voc_converters/voc_helper.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/voc_converters/voc_strategies.py` & `superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/voc_converters/voc_strategies.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/voc_converters/voc_to_sa_pixel.py` & `superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/voc_converters/voc_to_sa_pixel.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/voc_converters/voc_to_sa_vector.py` & `superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/voc_converters/voc_to_sa_vector.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/vott_converters/vott_strategies.py` & `superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/vott_converters/vott_strategies.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/vott_converters/vott_to_sa_vector.py` & `superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/vott_converters/vott_to_sa_vector.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/yolo_converters/yolo_strategies.py` & `superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/yolo_converters/yolo_strategies.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/converters/yolo_converters/yolo_to_sa_vector.py` & `superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/converters/yolo_converters/yolo_to_sa_vector.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/export_from_sa_conversions.py` & `superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/export_from_sa_conversions.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/import_to_sa_conversions.py` & `superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/import_to_sa_conversions.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/app/input_converters/sa_conversion.py` & `superannotate-4.4.9b1/src/superannotate/lib/app/input_converters/sa_conversion.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/app/interface/base_interface.py` & `superannotate-4.4.9b1/src/superannotate/lib/app/interface/base_interface.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/app/interface/cli_interface.py` & `superannotate-4.4.9b1/src/superannotate/lib/app/interface/cli_interface.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/app/interface/sdk_interface.py` & `superannotate-4.4.9b1/src/superannotate/lib/app/interface/sdk_interface.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/app/interface/types.py` & `superannotate-4.4.9b1/src/superannotate/lib/app/interface/types.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/app/serializers.py` & `superannotate-4.4.9b1/src/superannotate/lib/app/serializers.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/app/server/__app.py` & `superannotate-4.4.9b1/src/superannotate/lib/app/server/__app.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/app/server/core.py` & `superannotate-4.4.9b1/src/superannotate/lib/app/server/core.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/app/server/default_app.py` & `superannotate-4.4.9b1/src/superannotate/lib/app/server/default_app.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/core/__init__.py` & `superannotate-4.4.9b1/src/superannotate/lib/core/__init__.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/core/base_usecases.py` & `superannotate-4.4.9b1/src/superannotate/lib/core/base_usecases.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/core/conditions.py` & `superannotate-4.4.9b1/src/superannotate/lib/core/conditions.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/core/config.py` & `superannotate-4.4.9b1/src/superannotate/lib/core/config.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/core/entities/__init__.py` & `superannotate-4.4.9b1/src/superannotate/lib/core/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/core/entities/base.py` & `superannotate-4.4.9b1/src/superannotate/lib/core/entities/base.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/core/entities/classes.py` & `superannotate-4.4.9b1/src/superannotate/lib/core/entities/classes.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/core/entities/folder.py` & `superannotate-4.4.9b1/src/superannotate/lib/core/entities/folder.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/core/entities/items.py` & `superannotate-4.4.9b1/src/superannotate/lib/core/entities/items.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/core/entities/project.py` & `superannotate-4.4.9b1/src/superannotate/lib/core/entities/project.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/core/entities/project_entities.py` & `superannotate-4.4.9b1/src/superannotate/lib/core/entities/project_entities.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/core/enums.py` & `superannotate-4.4.9b1/src/superannotate/lib/core/enums.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/core/exceptions.py` & `superannotate-4.4.9b1/src/superannotate/lib/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/core/plugin.py` & `superannotate-4.4.9b1/src/superannotate/lib/core/plugin.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/core/reporter.py` & `superannotate-4.4.9b1/src/superannotate/lib/core/reporter.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/core/repositories.py` & `superannotate-4.4.9b1/src/superannotate/lib/core/repositories.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/core/response.py` & `superannotate-4.4.9b1/src/superannotate/lib/core/response.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/core/service_types.py` & `superannotate-4.4.9b1/src/superannotate/lib/core/service_types.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/core/serviceproviders.py` & `superannotate-4.4.9b1/src/superannotate/lib/core/serviceproviders.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/core/types.py` & `superannotate-4.4.9b1/src/superannotate/lib/core/types.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/core/usecases/__init__.py` & `superannotate-4.4.9b1/src/superannotate/lib/core/usecases/__init__.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/core/usecases/annotations.py` & `superannotate-4.4.9b1/src/superannotate/lib/core/usecases/annotations.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/core/usecases/base.py` & `superannotate-4.4.9b1/src/superannotate/lib/core/usecases/base.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/core/usecases/classes.py` & `superannotate-4.4.9b1/src/superannotate/lib/core/usecases/classes.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/core/usecases/custom_fields.py` & `superannotate-4.4.9b1/src/superannotate/lib/core/usecases/custom_fields.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/core/usecases/folders.py` & `superannotate-4.4.9b1/src/superannotate/lib/core/usecases/folders.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/core/usecases/images.py` & `superannotate-4.4.9b1/src/superannotate/lib/core/usecases/images.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/core/usecases/integrations.py` & `superannotate-4.4.9b1/src/superannotate/lib/core/usecases/integrations.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/core/usecases/items.py` & `superannotate-4.4.9b1/src/superannotate/lib/core/usecases/items.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/core/usecases/models.py` & `superannotate-4.4.9b1/src/superannotate/lib/core/usecases/models.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/core/usecases/projects.py` & `superannotate-4.4.9b1/src/superannotate/lib/core/usecases/projects.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/core/video_convertor.py` & `superannotate-4.4.9b1/src/superannotate/lib/core/video_convertor.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/infrastructure/controller.py` & `superannotate-4.4.9b1/src/superannotate/lib/infrastructure/controller.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/infrastructure/helpers.py` & `superannotate-4.4.9b1/src/superannotate/lib/infrastructure/helpers.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/infrastructure/repositories.py` & `superannotate-4.4.9b1/src/superannotate/lib/infrastructure/repositories.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/infrastructure/serviceprovider.py` & `superannotate-4.4.9b1/src/superannotate/lib/infrastructure/serviceprovider.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/infrastructure/services/annotation.py` & `superannotate-4.4.9b1/src/superannotate/lib/infrastructure/services/annotation.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/infrastructure/services/annotation_class.py` & `superannotate-4.4.9b1/src/superannotate/lib/infrastructure/services/annotation_class.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/infrastructure/services/custom_field.py` & `superannotate-4.4.9b1/src/superannotate/lib/infrastructure/services/custom_field.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/infrastructure/services/folder.py` & `superannotate-4.4.9b1/src/superannotate/lib/infrastructure/services/folder.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/infrastructure/services/http_client.py` & `superannotate-4.4.9b1/src/superannotate/lib/infrastructure/services/http_client.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/infrastructure/services/integration.py` & `superannotate-4.4.9b1/src/superannotate/lib/infrastructure/services/integration.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/infrastructure/services/item.py` & `superannotate-4.4.9b1/src/superannotate/lib/infrastructure/services/item.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/infrastructure/services/models.py` & `superannotate-4.4.9b1/src/superannotate/lib/infrastructure/services/models.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/infrastructure/services/project.py` & `superannotate-4.4.9b1/src/superannotate/lib/infrastructure/services/project.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/infrastructure/services/subset.py` & `superannotate-4.4.9b1/src/superannotate/lib/infrastructure/services/subset.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/infrastructure/stream_data_handler.py` & `superannotate-4.4.9b1/src/superannotate/lib/infrastructure/stream_data_handler.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/infrastructure/utils.py` & `superannotate-4.4.9b1/src/superannotate/lib/infrastructure/utils.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/lib/infrastructure/validators.py` & `superannotate-4.4.9b1/src/superannotate/lib/infrastructure/validators.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate/logger.py` & `superannotate-4.4.9b1/src/superannotate/logger.py`

 * *Files identical despite different names*

### Comparing `superannotate-4.4.9.dev5/src/superannotate.egg-info/PKG-INFO` & `superannotate-4.4.9b1/src/superannotate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superannotate
-Version: 4.4.9.dev5
+Version: 4.4.9b1
 Summary: Python SDK to SuperAnnotate platform
 Home-page: https://github.com/superannotateai/superannotate-python-sdk
 Author: SuperAnnotate AI
 Author-email: suppoort@superannotate.com
 License: MIT
 Project-URL: Documentation, https://superannotate.readthedocs.io/en/stable/
 Classifier: Programming Language :: Python
```

### Comparing `superannotate-4.4.9.dev5/src/superannotate.egg-info/SOURCES.txt` & `superannotate-4.4.9b1/src/superannotate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

