# Comparing `tmp/onvif_gui-1.0.2.tar.gz` & `tmp/onvif-gui-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onvif_gui-1.0.2.tar", last modified: Sun Apr 23 02:52:22 2023, max compression
+gzip compressed data, was "onvif-gui-1.0.3.tar", last modified: Sun Apr 23 02:57:19 2023, max compression
```

## Comparing `onvif_gui-1.0.2.tar` & `onvif-gui-1.0.3.tar`

### file list

```diff
@@ -1,271 +1,271 @@
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:52:22.335854 onvif_gui-1.0.2/
--rw-r--r--   0 stephen   (1000) stephen   (1000)    11357 2023-04-21 03:11:06.000000 onvif_gui-1.0.2/LICENSE
--rw-r--r--   0 stephen   (1000) stephen   (1000)       65 2023-04-22 12:44:29.000000 onvif_gui-1.0.2/MANIFEST.in
--rw-r--r--   0 stephen   (1000) stephen   (1000)     8711 2023-04-23 02:52:22.335854 onvif_gui-1.0.2/PKG-INFO
--rw-r--r--   0 stephen   (1000) stephen   (1000)     8171 2023-04-23 02:28:18.000000 onvif_gui-1.0.2/README.md
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:52:22.307854 onvif_gui-1.0.2/onvif_gui/
--rw-r--r--   0 stephen   (1000) stephen   (1000)       28 2023-04-21 01:55:37.000000 onvif_gui-1.0.2/onvif_gui/__init__.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:52:22.311854 onvif_gui-1.0.2/onvif_gui/components/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      196 2023-04-21 00:50:17.000000 onvif_gui-1.0.2/onvif_gui/components/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1743 2023-04-21 18:19:18.000000 onvif_gui-1.0.2/onvif_gui/components/comboselector.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2236 2023-04-21 18:19:18.000000 onvif_gui-1.0.2/onvif_gui/components/fileselector.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5320 2023-04-21 18:19:18.000000 onvif_gui-1.0.2/onvif_gui/components/labelselector.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4073 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/components/progress.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1143 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/components/thresholdslider.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:52:22.311854 onvif_gui-1.0.2/onvif_gui/detectron2/
--rw-r--r--   0 stephen   (1000) stephen   (1000)       67 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/__init__.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:52:22.311854 onvif_gui-1.0.2/onvif_gui/detectron2/checkpoint/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      347 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/checkpoint/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    17770 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/checkpoint/c2_model_loading.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5685 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/checkpoint/catalog.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5258 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/checkpoint/detection_checkpoint.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:52:22.311854 onvif_gui-1.0.2/onvif_gui/detectron2/config/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      599 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/config/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     7890 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/config/compat.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     9211 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/config/config.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    29512 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/config/defaults.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3015 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/config/instantiate.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    15378 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/config/lazy.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:52:22.311854 onvif_gui-1.0.2/onvif_gui/detectron2/configs/
--rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-04-20 14:25:53.000000 onvif_gui-1.0.2/onvif_gui/detectron2/configs/__init__.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:52:22.311854 onvif_gui-1.0.2/onvif_gui/detectron2/data/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      644 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/data/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     7378 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/data/benchmark.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    21231 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/data/build.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     7224 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/data/catalog.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     9162 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/data/common.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     8169 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/data/dataset_mapper.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:52:22.315854 onvif_gui-1.0.2/onvif_gui/detectron2/data/datasets/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      523 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/data/datasets/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    10174 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/data/datasets/builtin.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    21841 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/data/datasets/builtin_meta.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    13167 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/data/datasets/cityscapes.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     7821 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/data/datasets/cityscapes_panoptic.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    23465 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/data/datasets/coco.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     8977 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/data/datasets/coco_panoptic.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     9623 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/data/datasets/lvis.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)   223757 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/data/datasets/lvis_v0_5_categories.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)   219177 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/data/datasets/lvis_v1_categories.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    39414 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/data/datasets/lvis_v1_category_image_count.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3128 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/data/datasets/pascal_voc.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)      169 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/data/datasets/register_coco.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    22841 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/data/detection_utils.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:52:22.315854 onvif_gui-1.0.2/onvif_gui/detectron2/data/samplers/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      412 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/data/samplers/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    11789 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/data/samplers/distributed_sampler.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1944 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/data/samplers/grouped_batch_sampler.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:52:22.315854 onvif_gui-1.0.2/onvif_gui/detectron2/data/transforms/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      466 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/data/transforms/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    14112 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/data/transforms/augmentation.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    23069 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/data/transforms/augmentation_impl.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    12629 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/data/transforms/transform.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:52:22.315854 onvif_gui-1.0.2/onvif_gui/detectron2/layers/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      874 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/layers/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5764 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/layers/aspp.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    12131 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/layers/batch_norm.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3024 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/layers/blocks.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    16978 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/layers/deform_conv.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4202 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/layers/losses.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    10879 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/layers/mask_ops.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6490 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/layers/nms.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3098 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/layers/roi_align.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3302 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/layers/roi_align_rotated.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)      652 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/layers/rotated_boxes.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)      537 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/layers/shape_spec.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5123 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/layers/wrappers.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:52:22.319854 onvif_gui-1.0.2/onvif_gui/detectron2/modeling/
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1568 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/modeling/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    15439 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/modeling/anchor_generator.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:52:22.319854 onvif_gui-1.0.2/onvif_gui/detectron2/modeling/backbone/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      598 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/modeling/backbone/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2512 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/modeling/backbone/backbone.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1015 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/modeling/backbone/build.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    10360 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/modeling/backbone/fpn.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    15988 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/modeling/backbone/mvit.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    16656 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/modeling/backbone/regnet.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    23658 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/modeling/backbone/resnet.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    25095 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/modeling/backbone/swin.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6360 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/modeling/backbone/utils.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    19338 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/modeling/backbone/vit.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    15123 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/modeling/box_regression.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6264 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/modeling/matcher.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:52:22.319854 onvif_gui-1.0.2/onvif_gui/detectron2/modeling/meta_arch/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      508 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/modeling/meta_arch/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)      814 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/modeling/meta_arch/build.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    11651 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/modeling/meta_arch/dense_detector.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    13213 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/modeling/meta_arch/fcos.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    10407 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/modeling/meta_arch/panoptic_fpn.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    13896 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/modeling/meta_arch/rcnn.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    18265 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/modeling/meta_arch/retinanet.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     9906 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/modeling/meta_arch/semantic_seg.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    10832 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/modeling/mmdet_wrapper.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    11316 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/modeling/poolers.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4045 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/modeling/postprocessing.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:52:22.319854 onvif_gui-1.0.2/onvif_gui/detectron2/modeling/proposal_generator/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      231 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/modeling/proposal_generator/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)      836 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/modeling/proposal_generator/build.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     8128 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/modeling/proposal_generator/proposal_utils.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    23814 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/modeling/proposal_generator/rpn.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     8807 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/modeling/proposal_generator/rrpn.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:52:22.319854 onvif_gui-1.0.2/onvif_gui/detectron2/modeling/roi_heads/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      768 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/modeling/roi_heads/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4077 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/modeling/roi_heads/box_head.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    12990 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/modeling/roi_heads/cascade_rcnn.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    25390 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/modeling/roi_heads/fast_rcnn.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    11156 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/modeling/roi_heads/keypoint_head.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    12169 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/modeling/roi_heads/mask_head.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    37701 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/modeling/roi_heads/roi_heads.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    11175 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/modeling/roi_heads/rotated_fast_rcnn.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2334 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/modeling/sampling.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    12416 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/modeling/test_time_augmentation.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1780 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/predictor.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:52:22.323854 onvif_gui-1.0.2/onvif_gui/detectron2/structures/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      645 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/structures/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    14429 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/structures/boxes.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5520 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/structures/image_list.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6613 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/structures/instances.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     9030 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/structures/keypoints.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    19802 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/structures/masks.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    18853 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/structures/rotated_boxes.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2707 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/tracker.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:52:22.323854 onvif_gui-1.0.2/onvif_gui/detectron2/utils/
--rw-r--r--   0 stephen   (1000) stephen   (1000)       51 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/utils/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6017 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/utils/analysis.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     8391 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/utils/collect_env.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4096 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/utils/colormap.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5608 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/utils/comm.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1852 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/utils/develop.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5644 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/utils/env.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    17022 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/utils/events.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1189 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/utils/file_io.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     7807 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/utils/logger.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2583 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/utils/memory.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1874 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/utils/registry.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1064 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/utils/serialize.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    18113 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/utils/testing.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    11319 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/utils/video_visualizer.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    51159 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/detectron2/utils/visualizer.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1996 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/glwidget.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    11956 2023-04-23 02:50:48.000000 onvif_gui-1.0.2/onvif_gui/main.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:52:22.323854 onvif_gui-1.0.2/onvif_gui/modules/
--rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-04-20 01:38:46.000000 onvif_gui-1.0.2/onvif_gui/modules/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5981 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/modules/keypoint.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4215 2023-04-21 18:19:18.000000 onvif_gui-1.0.2/onvif_gui/modules/retinanet.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3006 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/modules/sample.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6542 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/modules/segment.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    10603 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/modules/yolox.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:52:22.323854 onvif_gui-1.0.2/onvif_gui/onvif/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      191 2023-04-21 00:45:40.000000 onvif_gui-1.0.2/onvif_gui/onvif/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5739 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/onvif/admintab.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3955 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/onvif/imagetab.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2421 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/onvif/logindialog.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5243 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/onvif/networktab.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5114 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/onvif/ptztab.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4523 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/onvif/videotab.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:52:22.323854 onvif_gui-1.0.2/onvif_gui/panels/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      147 2023-04-21 01:42:06.000000 onvif_gui-1.0.2/onvif_gui/panels/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    13464 2023-04-21 18:25:08.000000 onvif_gui-1.0.2/onvif_gui/panels/camerapanel.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    14489 2023-04-22 12:51:02.000000 onvif_gui-1.0.2/onvif_gui/panels/filepanel.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2737 2023-04-21 03:48:23.000000 onvif_gui-1.0.2/onvif_gui/panels/modulepanel.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    13192 2023-04-21 18:19:18.000000 onvif_gui-1.0.2/onvif_gui/panels/settingspanel.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:52:22.331854 onvif_gui-1.0.2/onvif_gui/resources/
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1126 2023-04-21 18:19:18.000000 onvif_gui-1.0.2/onvif_gui/resources/LICENSE
--rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-04-20 14:25:24.000000 onvif_gui-1.0.2/onvif_gui/resources/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)      252 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/apply.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      245 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/apply_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      244 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/apply_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      911 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/audio.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      536 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/audio_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      920 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/audio_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      203 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/branch_closed.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      219 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/branch_closed_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      211 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/branch_closed_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      199 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/branch_open.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      168 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/branch_open_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      172 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/branch_open_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      267 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/checked.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      235 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/checked_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      246 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/checked_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)    11948 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/darkstyle.qss
--rw-r--r--   0 stephen   (1000) stephen   (1000)      910 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/discover.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      849 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/discover_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      937 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/discover_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      425 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/fast-forward.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      253 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/fast-forward_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      433 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/fast-forward_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      641 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/mute.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      346 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/mute_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      618 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/mute_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      347 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/next.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      225 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/next_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      348 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/next_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)    46084 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/onvif_gui.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      172 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/pause.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      144 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/pause_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      149 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/pause_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      321 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/play.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      209 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/play_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      316 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/play_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      349 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/previous.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      232 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/previous_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      348 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/previous_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      324 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/radio-off.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      250 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/radio-off_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      324 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/radio-off_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      350 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/radio-on.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      263 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/radio-on_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      343 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/radio-on_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      395 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/record.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      394 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/record_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      425 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/record_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      408 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/recording.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      435 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/recording_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      532 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/recording_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2005 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/resources.qrc
--rw-r--r--   0 stephen   (1000) stephen   (1000)   120051 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/resources.rcc
--rw-r--r--   0 stephen   (1000) stephen   (1000)      454 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/rewind.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      250 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/rewind_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      457 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/rewind_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      187 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/small_arrow_left.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      183 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/small_arrow_left_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      189 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/small_arrow_left_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      162 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/small_arrow_up.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      160 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/small_arrow_up_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      161 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/small_arrow_up_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      158 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/stop.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      140 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/stop_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      151 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/stop_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      143 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/unchecked.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      142 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/unchecked_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      143 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/resources/unchecked_lo.png
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:52:22.331854 onvif_gui-1.0.2/onvif_gui/yolox/
--rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-04-20 01:35:42.000000 onvif_gui-1.0.2/onvif_gui/yolox/__init__.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:52:22.335854 onvif_gui-1.0.2/onvif_gui/yolox/models/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      936 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/yolox/models/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4894 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/yolox/models/build.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6647 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/yolox/models/darknet.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2305 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/yolox/models/losses.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6720 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/yolox/models/network_blocks.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3104 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/yolox/models/yolo_fpn.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    25526 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/yolox/models/yolo_head.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4158 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/yolox/models/yolo_pafpn.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1992 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/yolox/models/yolox.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:52:22.335854 onvif_gui-1.0.2/onvif_gui/yolox/tracker/
--rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-04-20 14:24:51.000000 onvif_gui-1.0.2/onvif_gui/yolox/tracker/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)      951 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/yolox/tracker/basetrack.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    12172 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/yolox/tracker/byte_tracker.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     9547 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/yolox/tracker/kalman_filter.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6158 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/yolox/tracker/matching.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:52:22.335854 onvif_gui-1.0.2/onvif_gui/yolox/utils/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      126 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/yolox/utils/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1580 2023-04-18 23:02:56.000000 onvif_gui-1.0.2/onvif_gui/yolox/utils/utils.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:52:22.311854 onvif_gui-1.0.2/onvif_gui.egg-info/
--rw-r--r--   0 stephen   (1000) stephen   (1000)     8711 2023-04-23 02:52:22.000000 onvif_gui-1.0.2/onvif_gui.egg-info/PKG-INFO
--rw-r--r--   0 stephen   (1000) stephen   (1000)     9466 2023-04-23 02:52:22.000000 onvif_gui-1.0.2/onvif_gui.egg-info/SOURCES.txt
--rw-r--r--   0 stephen   (1000) stephen   (1000)        1 2023-04-23 02:52:22.000000 onvif_gui-1.0.2/onvif_gui.egg-info/dependency_links.txt
--rw-r--r--   0 stephen   (1000) stephen   (1000)       45 2023-04-23 02:52:22.000000 onvif_gui-1.0.2/onvif_gui.egg-info/entry_points.txt
--rw-r--r--   0 stephen   (1000) stephen   (1000)       47 2023-04-23 02:52:22.000000 onvif_gui-1.0.2/onvif_gui.egg-info/requires.txt
--rw-r--r--   0 stephen   (1000) stephen   (1000)       10 2023-04-23 02:52:22.000000 onvif_gui-1.0.2/onvif_gui.egg-info/top_level.txt
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1524 2023-04-23 02:52:00.000000 onvif_gui-1.0.2/pyproject.toml
--rw-r--r--   0 stephen   (1000) stephen   (1000)       38 2023-04-23 02:52:22.335854 onvif_gui-1.0.2/setup.cfg
--rw-r--r--   0 stephen   (1000) stephen   (1000)      740 2023-04-23 02:52:07.000000 onvif_gui-1.0.2/setup.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.759837 onvif-gui-1.0.3/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    11357 2023-04-21 03:11:06.000000 onvif-gui-1.0.3/LICENSE
+-rw-r--r--   0 stephen   (1000) stephen   (1000)       65 2023-04-22 12:44:29.000000 onvif-gui-1.0.3/MANIFEST.in
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     8710 2023-04-23 02:57:19.759837 onvif-gui-1.0.3/PKG-INFO
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     8171 2023-04-23 02:28:18.000000 onvif-gui-1.0.3/README.md
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.723837 onvif-gui-1.0.3/onvif_gui/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)       28 2023-04-21 01:55:37.000000 onvif-gui-1.0.3/onvif_gui/__init__.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.723837 onvif-gui-1.0.3/onvif_gui/components/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      196 2023-04-21 00:50:17.000000 onvif-gui-1.0.3/onvif_gui/components/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1743 2023-04-21 18:19:18.000000 onvif-gui-1.0.3/onvif_gui/components/comboselector.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2236 2023-04-21 18:19:18.000000 onvif-gui-1.0.3/onvif_gui/components/fileselector.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5320 2023-04-21 18:19:18.000000 onvif-gui-1.0.3/onvif_gui/components/labelselector.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4073 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/components/progress.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1143 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/components/thresholdslider.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.723837 onvif-gui-1.0.3/onvif_gui/detectron2/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)       67 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/__init__.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.727837 onvif-gui-1.0.3/onvif_gui/detectron2/checkpoint/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      347 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/checkpoint/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    17770 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/checkpoint/c2_model_loading.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5685 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/checkpoint/catalog.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5258 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/checkpoint/detection_checkpoint.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.727837 onvif-gui-1.0.3/onvif_gui/detectron2/config/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      599 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/config/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     7890 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/config/compat.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     9211 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/config/config.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    29512 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/config/defaults.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3015 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/config/instantiate.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    15378 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/config/lazy.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.727837 onvif-gui-1.0.3/onvif_gui/detectron2/configs/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-04-20 14:25:53.000000 onvif-gui-1.0.3/onvif_gui/detectron2/configs/__init__.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.727837 onvif-gui-1.0.3/onvif_gui/detectron2/data/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      644 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/data/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     7378 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/data/benchmark.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    21231 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/data/build.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     7224 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/data/catalog.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     9162 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/data/common.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     8169 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/data/dataset_mapper.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.731837 onvif-gui-1.0.3/onvif_gui/detectron2/data/datasets/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      523 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/data/datasets/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    10174 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/data/datasets/builtin.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    21841 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/data/datasets/builtin_meta.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    13167 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/data/datasets/cityscapes.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     7821 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/data/datasets/cityscapes_panoptic.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    23465 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/data/datasets/coco.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     8977 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/data/datasets/coco_panoptic.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     9623 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/data/datasets/lvis.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)   223757 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/data/datasets/lvis_v0_5_categories.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)   219177 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/data/datasets/lvis_v1_categories.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    39414 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/data/datasets/lvis_v1_category_image_count.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3128 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/data/datasets/pascal_voc.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      169 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/data/datasets/register_coco.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    22841 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/data/detection_utils.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.731837 onvif-gui-1.0.3/onvif_gui/detectron2/data/samplers/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      412 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/data/samplers/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    11789 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/data/samplers/distributed_sampler.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1944 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/data/samplers/grouped_batch_sampler.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.731837 onvif-gui-1.0.3/onvif_gui/detectron2/data/transforms/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      466 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/data/transforms/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    14112 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/data/transforms/augmentation.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    23069 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/data/transforms/augmentation_impl.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    12629 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/data/transforms/transform.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.735837 onvif-gui-1.0.3/onvif_gui/detectron2/layers/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      874 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/layers/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5764 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/layers/aspp.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    12131 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/layers/batch_norm.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3024 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/layers/blocks.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    16978 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/layers/deform_conv.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4202 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/layers/losses.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    10879 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/layers/mask_ops.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     6490 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/layers/nms.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3098 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/layers/roi_align.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3302 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/layers/roi_align_rotated.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      652 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/layers/rotated_boxes.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      537 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/layers/shape_spec.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5123 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/layers/wrappers.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.735837 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1568 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    15439 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/anchor_generator.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.735837 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/backbone/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      598 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/backbone/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2512 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/backbone/backbone.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1015 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/backbone/build.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    10360 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/backbone/fpn.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    15988 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/backbone/mvit.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    16656 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/backbone/regnet.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    23658 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/backbone/resnet.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    25095 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/backbone/swin.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     6360 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/backbone/utils.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    19338 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/backbone/vit.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    15123 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/box_regression.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     6264 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/matcher.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.739837 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/meta_arch/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      508 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/meta_arch/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      814 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/meta_arch/build.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    11651 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/meta_arch/dense_detector.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    13213 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/meta_arch/fcos.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    10407 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/meta_arch/panoptic_fpn.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    13896 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/meta_arch/rcnn.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    18265 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/meta_arch/retinanet.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     9906 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/meta_arch/semantic_seg.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    10832 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/mmdet_wrapper.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    11316 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/poolers.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4045 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/postprocessing.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.739837 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/proposal_generator/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      231 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/proposal_generator/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      836 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/proposal_generator/build.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     8128 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/proposal_generator/proposal_utils.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    23814 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/proposal_generator/rpn.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     8807 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/proposal_generator/rrpn.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.739837 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/roi_heads/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      768 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/roi_heads/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4077 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/roi_heads/box_head.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    12990 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/roi_heads/cascade_rcnn.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    25390 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/roi_heads/fast_rcnn.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    11156 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/roi_heads/keypoint_head.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    12169 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/roi_heads/mask_head.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    37701 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/roi_heads/roi_heads.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    11175 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/roi_heads/rotated_fast_rcnn.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2334 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/sampling.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    12416 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/modeling/test_time_augmentation.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1780 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/predictor.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.739837 onvif-gui-1.0.3/onvif_gui/detectron2/structures/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      645 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/structures/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    14429 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/structures/boxes.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5520 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/structures/image_list.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     6613 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/structures/instances.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     9030 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/structures/keypoints.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    19802 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/structures/masks.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    18853 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/structures/rotated_boxes.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2707 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/tracker.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.743837 onvif-gui-1.0.3/onvif_gui/detectron2/utils/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)       51 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/utils/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     6017 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/utils/analysis.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     8391 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/utils/collect_env.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4096 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/utils/colormap.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5608 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/utils/comm.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1852 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/utils/develop.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5644 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/utils/env.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    17022 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/utils/events.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1189 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/utils/file_io.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     7807 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/utils/logger.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2583 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/utils/memory.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1874 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/utils/registry.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1064 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/utils/serialize.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    18113 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/utils/testing.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    11319 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/utils/video_visualizer.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    51159 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/detectron2/utils/visualizer.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1996 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/glwidget.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    11956 2023-04-23 02:50:48.000000 onvif-gui-1.0.3/onvif_gui/main.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.743837 onvif-gui-1.0.3/onvif_gui/modules/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-04-20 01:38:46.000000 onvif-gui-1.0.3/onvif_gui/modules/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5981 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/modules/keypoint.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4215 2023-04-21 18:19:18.000000 onvif-gui-1.0.3/onvif_gui/modules/retinanet.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3006 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/modules/sample.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     6542 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/modules/segment.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    10603 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/modules/yolox.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.747837 onvif-gui-1.0.3/onvif_gui/onvif/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      191 2023-04-21 00:45:40.000000 onvif-gui-1.0.3/onvif_gui/onvif/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5739 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/onvif/admintab.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3955 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/onvif/imagetab.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2421 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/onvif/logindialog.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5243 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/onvif/networktab.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5114 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/onvif/ptztab.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4523 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/onvif/videotab.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.747837 onvif-gui-1.0.3/onvif_gui/panels/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      147 2023-04-21 01:42:06.000000 onvif-gui-1.0.3/onvif_gui/panels/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    13464 2023-04-21 18:25:08.000000 onvif-gui-1.0.3/onvif_gui/panels/camerapanel.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    14489 2023-04-22 12:51:02.000000 onvif-gui-1.0.3/onvif_gui/panels/filepanel.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2737 2023-04-21 03:48:23.000000 onvif-gui-1.0.3/onvif_gui/panels/modulepanel.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    13192 2023-04-21 18:19:18.000000 onvif-gui-1.0.3/onvif_gui/panels/settingspanel.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.759837 onvif-gui-1.0.3/onvif_gui/resources/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1126 2023-04-21 18:19:18.000000 onvif-gui-1.0.3/onvif_gui/resources/LICENSE
+-rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-04-20 14:25:24.000000 onvif-gui-1.0.3/onvif_gui/resources/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      252 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/apply.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      245 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/apply_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      244 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/apply_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      911 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/audio.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      536 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/audio_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      920 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/audio_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      203 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/branch_closed.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      219 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/branch_closed_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      211 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/branch_closed_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      199 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/branch_open.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      168 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/branch_open_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      172 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/branch_open_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      267 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/checked.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      235 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/checked_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      246 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/checked_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    11948 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/darkstyle.qss
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      910 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/discover.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      849 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/discover_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      937 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/discover_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      425 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/fast-forward.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      253 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/fast-forward_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      433 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/fast-forward_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      641 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/mute.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      346 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/mute_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      618 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/mute_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      347 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/next.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      225 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/next_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      348 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/next_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    46084 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/onvif_gui.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      172 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/pause.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      144 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/pause_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      149 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/pause_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      321 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/play.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      209 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/play_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      316 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/play_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      349 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/previous.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      232 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/previous_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      348 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/previous_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      324 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/radio-off.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      250 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/radio-off_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      324 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/radio-off_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      350 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/radio-on.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      263 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/radio-on_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      343 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/radio-on_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      395 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/record.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      394 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/record_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      425 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/record_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      408 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/recording.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      435 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/recording_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      532 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/recording_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2005 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/resources.qrc
+-rw-r--r--   0 stephen   (1000) stephen   (1000)   120051 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/resources.rcc
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      454 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/rewind.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      250 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/rewind_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      457 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/rewind_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      187 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/small_arrow_left.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      183 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/small_arrow_left_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      189 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/small_arrow_left_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      162 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/small_arrow_up.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      160 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/small_arrow_up_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      161 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/small_arrow_up_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      158 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/stop.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      140 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/stop_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      151 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/stop_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      143 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/unchecked.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      142 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/unchecked_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      143 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/resources/unchecked_lo.png
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.759837 onvif-gui-1.0.3/onvif_gui/yolox/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-04-20 01:35:42.000000 onvif-gui-1.0.3/onvif_gui/yolox/__init__.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.759837 onvif-gui-1.0.3/onvif_gui/yolox/models/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      936 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/yolox/models/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4894 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/yolox/models/build.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     6647 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/yolox/models/darknet.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2305 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/yolox/models/losses.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     6720 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/yolox/models/network_blocks.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3104 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/yolox/models/yolo_fpn.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    25526 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/yolox/models/yolo_head.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4158 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/yolox/models/yolo_pafpn.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1992 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/yolox/models/yolox.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.759837 onvif-gui-1.0.3/onvif_gui/yolox/tracker/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-04-20 14:24:51.000000 onvif-gui-1.0.3/onvif_gui/yolox/tracker/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      951 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/yolox/tracker/basetrack.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    12172 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/yolox/tracker/byte_tracker.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     9547 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/yolox/tracker/kalman_filter.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     6158 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/yolox/tracker/matching.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.759837 onvif-gui-1.0.3/onvif_gui/yolox/utils/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      126 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/yolox/utils/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1580 2023-04-18 23:02:56.000000 onvif-gui-1.0.3/onvif_gui/yolox/utils/utils.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-23 02:57:19.723837 onvif-gui-1.0.3/onvif_gui.egg-info/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     8710 2023-04-23 02:57:19.000000 onvif-gui-1.0.3/onvif_gui.egg-info/PKG-INFO
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     9466 2023-04-23 02:57:19.000000 onvif-gui-1.0.3/onvif_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 stephen   (1000) stephen   (1000)        1 2023-04-23 02:57:19.000000 onvif-gui-1.0.3/onvif_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 stephen   (1000) stephen   (1000)       45 2023-04-23 02:57:19.000000 onvif-gui-1.0.3/onvif_gui.egg-info/entry_points.txt
+-rw-r--r--   0 stephen   (1000) stephen   (1000)       47 2023-04-23 02:57:19.000000 onvif-gui-1.0.3/onvif_gui.egg-info/requires.txt
+-rw-r--r--   0 stephen   (1000) stephen   (1000)       10 2023-04-23 02:57:19.000000 onvif-gui-1.0.3/onvif_gui.egg-info/top_level.txt
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1523 2023-04-23 02:56:42.000000 onvif-gui-1.0.3/pyproject.toml
+-rw-r--r--   0 stephen   (1000) stephen   (1000)       38 2023-04-23 02:57:19.759837 onvif-gui-1.0.3/setup.cfg
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      740 2023-04-23 02:56:51.000000 onvif-gui-1.0.3/setup.py
```

### Comparing `onvif_gui-1.0.2/LICENSE` & `onvif-gui-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/PKG-INFO` & `onvif-gui-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: onvif_gui
-Version: 1.0.2
-Summary: A sample Python project
+Name: onvif-gui
+Version: 1.0.3
+Summary: A client gui for Onvif
 Author: Stephen Rhodes
 Author-email: Stephen Rhodes <sr99622@gmail.com>
 Keywords: sample,setuptools,development
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `onvif_gui-1.0.2/README.md` & `onvif-gui-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/components/comboselector.py` & `onvif-gui-1.0.3/onvif_gui/components/comboselector.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/components/fileselector.py` & `onvif-gui-1.0.3/onvif_gui/components/fileselector.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/components/labelselector.py` & `onvif-gui-1.0.3/onvif_gui/components/labelselector.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/components/progress.py` & `onvif-gui-1.0.3/onvif_gui/components/progress.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/components/thresholdslider.py` & `onvif-gui-1.0.3/onvif_gui/components/thresholdslider.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/checkpoint/c2_model_loading.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/checkpoint/c2_model_loading.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/checkpoint/catalog.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/checkpoint/catalog.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/checkpoint/detection_checkpoint.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/checkpoint/detection_checkpoint.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/config/__init__.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/config/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/config/compat.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/config/compat.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/config/config.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/config/config.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/config/defaults.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/config/defaults.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/config/instantiate.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/config/instantiate.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/config/lazy.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/config/lazy.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/data/__init__.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/data/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/data/benchmark.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/data/benchmark.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/data/build.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/data/build.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/data/catalog.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/data/catalog.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/data/common.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/data/common.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/data/dataset_mapper.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/data/dataset_mapper.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/data/datasets/__init__.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/data/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/data/datasets/builtin.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/data/datasets/builtin.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/data/datasets/builtin_meta.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/data/datasets/builtin_meta.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/data/datasets/cityscapes.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/data/datasets/cityscapes.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/data/datasets/cityscapes_panoptic.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/data/datasets/cityscapes_panoptic.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/data/datasets/coco.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/data/datasets/coco.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/data/datasets/coco_panoptic.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/data/datasets/coco_panoptic.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/data/datasets/lvis.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/data/datasets/lvis.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/data/datasets/lvis_v0_5_categories.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/data/datasets/lvis_v0_5_categories.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/data/datasets/lvis_v1_categories.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/data/datasets/lvis_v1_categories.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/data/datasets/lvis_v1_category_image_count.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/data/datasets/lvis_v1_category_image_count.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/data/datasets/pascal_voc.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/data/datasets/pascal_voc.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/data/detection_utils.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/data/detection_utils.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/data/samplers/distributed_sampler.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/data/samplers/distributed_sampler.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/data/samplers/grouped_batch_sampler.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/data/samplers/grouped_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/data/transforms/augmentation.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/data/transforms/augmentation.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/data/transforms/augmentation_impl.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/data/transforms/augmentation_impl.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/data/transforms/transform.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/data/transforms/transform.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/layers/__init__.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/layers/aspp.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/layers/aspp.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/layers/batch_norm.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/layers/batch_norm.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/layers/blocks.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/layers/blocks.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/layers/deform_conv.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/layers/deform_conv.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/layers/losses.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/layers/losses.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/layers/mask_ops.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/layers/mask_ops.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/layers/nms.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/layers/nms.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/layers/roi_align.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/layers/roi_align.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/layers/roi_align_rotated.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/layers/roi_align_rotated.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/layers/rotated_boxes.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/layers/rotated_boxes.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/layers/shape_spec.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/layers/shape_spec.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/layers/wrappers.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/layers/wrappers.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/modeling/__init__.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/modeling/anchor_generator.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/anchor_generator.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/modeling/backbone/__init__.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/backbone/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/modeling/backbone/backbone.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/backbone/backbone.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/modeling/backbone/build.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/backbone/build.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/modeling/backbone/fpn.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/backbone/fpn.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/modeling/backbone/mvit.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/backbone/mvit.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/modeling/backbone/regnet.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/backbone/regnet.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/modeling/backbone/resnet.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/backbone/resnet.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/modeling/backbone/swin.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/backbone/swin.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/modeling/backbone/utils.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/backbone/utils.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/modeling/backbone/vit.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/backbone/vit.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/modeling/box_regression.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/box_regression.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/modeling/matcher.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/matcher.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/modeling/meta_arch/build.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/meta_arch/build.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/modeling/meta_arch/dense_detector.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/meta_arch/dense_detector.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/modeling/meta_arch/fcos.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/meta_arch/fcos.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/modeling/meta_arch/panoptic_fpn.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/meta_arch/panoptic_fpn.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/modeling/meta_arch/rcnn.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/meta_arch/rcnn.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/modeling/meta_arch/retinanet.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/meta_arch/retinanet.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/modeling/meta_arch/semantic_seg.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/meta_arch/semantic_seg.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/modeling/mmdet_wrapper.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/mmdet_wrapper.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/modeling/poolers.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/poolers.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/modeling/postprocessing.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/postprocessing.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/modeling/proposal_generator/build.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/proposal_generator/build.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/modeling/proposal_generator/proposal_utils.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/proposal_generator/proposal_utils.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/modeling/proposal_generator/rpn.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/proposal_generator/rpn.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/modeling/proposal_generator/rrpn.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/proposal_generator/rrpn.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/modeling/roi_heads/__init__.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/roi_heads/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/modeling/roi_heads/box_head.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/roi_heads/box_head.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/modeling/roi_heads/cascade_rcnn.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/roi_heads/cascade_rcnn.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/modeling/roi_heads/fast_rcnn.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/roi_heads/fast_rcnn.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/modeling/roi_heads/keypoint_head.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/roi_heads/keypoint_head.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/modeling/roi_heads/mask_head.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/roi_heads/mask_head.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/modeling/roi_heads/roi_heads.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/roi_heads/roi_heads.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/modeling/roi_heads/rotated_fast_rcnn.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/roi_heads/rotated_fast_rcnn.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/modeling/sampling.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/sampling.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/modeling/test_time_augmentation.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/modeling/test_time_augmentation.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/predictor.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/predictor.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/structures/__init__.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/structures/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/structures/boxes.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/structures/boxes.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/structures/image_list.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/structures/image_list.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/structures/instances.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/structures/instances.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/structures/keypoints.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/structures/keypoints.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/structures/masks.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/structures/masks.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/structures/rotated_boxes.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/structures/rotated_boxes.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/tracker.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/tracker.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/utils/analysis.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/utils/analysis.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/utils/collect_env.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/utils/colormap.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/utils/colormap.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/utils/comm.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/utils/comm.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/utils/develop.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/utils/develop.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/utils/env.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/utils/env.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/utils/events.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/utils/events.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/utils/file_io.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/utils/file_io.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/utils/logger.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/utils/logger.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/utils/memory.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/utils/memory.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/utils/registry.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/utils/registry.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/utils/serialize.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/utils/serialize.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/utils/testing.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/utils/testing.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/utils/video_visualizer.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/utils/video_visualizer.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/detectron2/utils/visualizer.py` & `onvif-gui-1.0.3/onvif_gui/detectron2/utils/visualizer.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/glwidget.py` & `onvif-gui-1.0.3/onvif_gui/glwidget.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/main.py` & `onvif-gui-1.0.3/onvif_gui/main.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/modules/keypoint.py` & `onvif-gui-1.0.3/onvif_gui/modules/keypoint.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/modules/retinanet.py` & `onvif-gui-1.0.3/onvif_gui/modules/retinanet.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/modules/sample.py` & `onvif-gui-1.0.3/onvif_gui/modules/sample.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/modules/segment.py` & `onvif-gui-1.0.3/onvif_gui/modules/segment.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/modules/yolox.py` & `onvif-gui-1.0.3/onvif_gui/modules/yolox.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/onvif/admintab.py` & `onvif-gui-1.0.3/onvif_gui/onvif/admintab.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/onvif/imagetab.py` & `onvif-gui-1.0.3/onvif_gui/onvif/imagetab.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/onvif/logindialog.py` & `onvif-gui-1.0.3/onvif_gui/onvif/logindialog.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/onvif/networktab.py` & `onvif-gui-1.0.3/onvif_gui/onvif/networktab.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/onvif/ptztab.py` & `onvif-gui-1.0.3/onvif_gui/onvif/ptztab.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/onvif/videotab.py` & `onvif-gui-1.0.3/onvif_gui/onvif/videotab.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/panels/camerapanel.py` & `onvif-gui-1.0.3/onvif_gui/panels/camerapanel.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/panels/filepanel.py` & `onvif-gui-1.0.3/onvif_gui/panels/filepanel.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/panels/modulepanel.py` & `onvif-gui-1.0.3/onvif_gui/panels/modulepanel.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/panels/settingspanel.py` & `onvif-gui-1.0.3/onvif_gui/panels/settingspanel.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/resources/LICENSE` & `onvif-gui-1.0.3/onvif_gui/resources/LICENSE`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/resources/audio.png` & `onvif-gui-1.0.3/onvif_gui/resources/audio.png`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/resources/audio_hi.png` & `onvif-gui-1.0.3/onvif_gui/resources/audio_hi.png`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/resources/audio_lo.png` & `onvif-gui-1.0.3/onvif_gui/resources/audio_lo.png`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/resources/darkstyle.qss` & `onvif-gui-1.0.3/onvif_gui/resources/darkstyle.qss`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/resources/discover.png` & `onvif-gui-1.0.3/onvif_gui/resources/discover.png`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/resources/discover_hi.png` & `onvif-gui-1.0.3/onvif_gui/resources/discover_hi.png`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/resources/discover_lo.png` & `onvif-gui-1.0.3/onvif_gui/resources/discover_lo.png`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/resources/mute.png` & `onvif-gui-1.0.3/onvif_gui/resources/mute.png`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/resources/mute_lo.png` & `onvif-gui-1.0.3/onvif_gui/resources/mute_lo.png`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/resources/onvif_gui.png` & `onvif-gui-1.0.3/onvif_gui/resources/onvif_gui.png`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/resources/recording_lo.png` & `onvif-gui-1.0.3/onvif_gui/resources/recording_lo.png`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/resources/resources.qrc` & `onvif-gui-1.0.3/onvif_gui/resources/resources.qrc`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/resources/resources.rcc` & `onvif-gui-1.0.3/onvif_gui/resources/resources.rcc`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/yolox/models/__init__.py` & `onvif-gui-1.0.3/onvif_gui/yolox/models/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/yolox/models/build.py` & `onvif-gui-1.0.3/onvif_gui/yolox/models/build.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/yolox/models/darknet.py` & `onvif-gui-1.0.3/onvif_gui/yolox/models/darknet.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/yolox/models/losses.py` & `onvif-gui-1.0.3/onvif_gui/yolox/models/losses.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/yolox/models/network_blocks.py` & `onvif-gui-1.0.3/onvif_gui/yolox/models/network_blocks.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/yolox/models/yolo_fpn.py` & `onvif-gui-1.0.3/onvif_gui/yolox/models/yolo_fpn.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/yolox/models/yolo_head.py` & `onvif-gui-1.0.3/onvif_gui/yolox/models/yolo_head.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/yolox/models/yolo_pafpn.py` & `onvif-gui-1.0.3/onvif_gui/yolox/models/yolo_pafpn.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/yolox/models/yolox.py` & `onvif-gui-1.0.3/onvif_gui/yolox/models/yolox.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/yolox/tracker/basetrack.py` & `onvif-gui-1.0.3/onvif_gui/yolox/tracker/basetrack.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/yolox/tracker/byte_tracker.py` & `onvif-gui-1.0.3/onvif_gui/yolox/tracker/byte_tracker.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/yolox/tracker/kalman_filter.py` & `onvif-gui-1.0.3/onvif_gui/yolox/tracker/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/yolox/tracker/matching.py` & `onvif-gui-1.0.3/onvif_gui/yolox/tracker/matching.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui/yolox/utils/utils.py` & `onvif-gui-1.0.3/onvif_gui/yolox/utils/utils.py`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/onvif_gui.egg-info/PKG-INFO` & `onvif-gui-1.0.3/onvif_gui.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: onvif-gui
-Version: 1.0.2
-Summary: A sample Python project
+Version: 1.0.3
+Summary: A client gui for Onvif
 Author: Stephen Rhodes
 Author-email: Stephen Rhodes <sr99622@gmail.com>
 Keywords: sample,setuptools,development
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `onvif_gui-1.0.2/onvif_gui.egg-info/SOURCES.txt` & `onvif-gui-1.0.3/onvif_gui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onvif_gui-1.0.2/pyproject.toml` & `onvif-gui-1.0.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
-name = "onvif_gui"  # Required
-version = "1.0.2"  # Required
-description = "A sample Python project"  # Optional
+name = "onvif-gui"  # Required
+version = "1.0.3"  # Required
+description = "A client gui for Onvif"  # Optional
 readme = "README.md" # Optional
 requires-python = ">=3.7"
 license = {file = "LICENSE.txt"}
 keywords = ["sample", "setuptools", "development"]  # Optional
 authors = [
   {name = "Stephen Rhodes", email = "sr99622@gmail.com" } # Optional
 ]
```

### Comparing `onvif_gui-1.0.2/setup.py` & `onvif-gui-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools.command.install import install
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="onvif_gui",
-    version="1.0.2",
+    version="1.0.3",
     author="Stephen Rhodes",
     author_email="sr99622@gmail.com",
     description="GUI program for onvif",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     classifiers=[
```

