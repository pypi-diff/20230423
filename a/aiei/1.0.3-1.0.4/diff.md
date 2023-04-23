# Comparing `tmp/aiei-1.0.3.tar.gz` & `tmp/aiei-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiei-1.0.3.tar", last modified: Sun Apr 23 12:11:48 2023, max compression
+gzip compressed data, was "aiei-1.0.4.tar", last modified: Sun Apr 23 12:24:59 2023, max compression
```

## Comparing `aiei-1.0.3.tar` & `aiei-1.0.4.tar`

### file list

```diff
@@ -1,124 +1,124 @@
-drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:11:48.499378 aiei-1.0.3/
--rw-rw-r--   0 zl        (1001) zl        (1001)       52 2020-11-09 02:20:47.000000 aiei-1.0.3/MANIFEST.in
--rw-rw-r--   0 zl        (1001) zl        (1001)     1203 2023-04-23 12:11:48.499378 aiei-1.0.3/PKG-INFO
--rw-rw-r--   0 zl        (1001) zl        (1001)      381 2021-09-16 03:57:42.000000 aiei-1.0.3/README.md
-drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:11:48.479378 aiei-1.0.3/aiei/
--rw-rw-r--   0 zl        (1001) zl        (1001)      103 2022-10-08 08:20:10.000000 aiei-1.0.3/aiei/__init__.py
-drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:11:48.479378 aiei-1.0.3/aiei/core/
--rw-rw-r--   0 zl        (1001) zl        (1001)        0 2020-09-30 08:03:24.000000 aiei-1.0.3/aiei/core/__init__.py
--rw-rw-r--   0 zl        (1001) zl        (1001)    20925 2023-04-23 12:02:54.000000 aiei-1.0.3/aiei/core/aiei.py
--rw-rw-r--   0 zl        (1001) zl        (1001)    12553 2023-04-23 11:53:00.000000 aiei-1.0.3/aiei/core/base_config.py
-drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:11:48.479378 aiei-1.0.3/aiei/ctrib/
--rw-rw-r--   0 zl        (1001) zl        (1001)        0 2019-01-22 03:50:05.000000 aiei-1.0.3/aiei/ctrib/__init__.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     8408 2019-03-13 14:17:09.000000 aiei-1.0.3/aiei/ctrib/dsn.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     7142 2022-05-23 14:12:33.000000 aiei-1.0.3/aiei/ctrib/soft_argmax.py
-drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:11:48.479378 aiei-1.0.3/aiei/data/
--rw-rw-r--   0 zl        (1001) zl        (1001)        0 2019-01-22 02:30:50.000000 aiei-1.0.3/aiei/data/__init__.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     1402 2020-01-09 04:09:08.000000 aiei-1.0.3/aiei/data/mixup.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     5522 2021-09-08 08:26:09.000000 aiei-1.0.3/aiei/data/sampler.py
-drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:11:48.479378 aiei-1.0.3/aiei/data/set/
--rw-rw-r--   0 zl        (1001) zl        (1001)        0 2019-01-22 02:30:50.000000 aiei-1.0.3/aiei/data/set/__init__.py
--rw-rw-r--   0 zl        (1001) zl        (1001)    18747 2021-12-16 06:48:44.000000 aiei-1.0.3/aiei/data/set/coco.py
-drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:11:48.483378 aiei-1.0.3/aiei/data/transform/
--rw-rw-r--   0 zl        (1001) zl        (1001)      522 2021-09-08 07:01:47.000000 aiei-1.0.3/aiei/data/transform/__init__.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     3937 2021-09-07 04:19:20.000000 aiei-1.0.3/aiei/data/transform/base_cls.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     6346 2021-09-07 06:35:16.000000 aiei-1.0.3/aiei/data/transform/base_fn.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     4390 2021-09-08 07:06:13.000000 aiei-1.0.3/aiei/data/transform/center_pad.py
--rw-rw-r--   0 zl        (1001) zl        (1001)      325 2021-09-08 07:07:16.000000 aiei-1.0.3/aiei/data/transform/normalize.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     7188 2021-11-07 09:07:41.000000 aiei-1.0.3/aiei/data/transform/random_affine.py
--rw-rw-r--   0 zl        (1001) zl        (1001)      560 2021-09-08 07:07:57.000000 aiei-1.0.3/aiei/data/transform/random_brightness.py
--rw-rw-r--   0 zl        (1001) zl        (1001)      569 2021-09-08 07:08:14.000000 aiei-1.0.3/aiei/data/transform/random_contrast.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     2343 2021-09-08 07:08:30.000000 aiei-1.0.3/aiei/data/transform/random_crop.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     1814 2021-09-08 07:08:43.000000 aiei-1.0.3/aiei/data/transform/random_erase.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     3030 2021-09-08 07:08:56.000000 aiei-1.0.3/aiei/data/transform/random_flip.py
--rw-rw-r--   0 zl        (1001) zl        (1001)      827 2021-09-08 07:09:17.000000 aiei-1.0.3/aiei/data/transform/random_lighting.py
--rw-rw-r--   0 zl        (1001) zl        (1001)      691 2021-09-08 07:09:30.000000 aiei-1.0.3/aiei/data/transform/random_saturation.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     3216 2021-11-07 09:03:15.000000 aiei-1.0.3/aiei/data/transform/resize_edge.py
--rw-rw-r--   0 zl        (1001) zl        (1001)      188 2021-09-08 07:10:01.000000 aiei-1.0.3/aiei/data/transform/to_tensor.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     1635 2020-07-31 01:17:10.000000 aiei-1.0.3/aiei/data/utils.py
--rw-rw-r--   0 zl        (1001) zl        (1001)      580 2023-04-23 12:11:04.000000 aiei-1.0.3/aiei/info.py
-drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:11:48.483378 aiei-1.0.3/aiei/misc/
--rw-rw-r--   0 zl        (1001) zl        (1001)        0 2018-08-15 03:47:04.000000 aiei-1.0.3/aiei/misc/__init__.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     1133 2020-12-16 07:13:35.000000 aiei-1.0.3/aiei/misc/alg.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     3981 2020-05-11 11:28:08.000000 aiei-1.0.3/aiei/misc/dist.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     4920 2023-02-02 10:18:50.000000 aiei-1.0.3/aiei/misc/dotsi.py
--rwxrwxr-x   0 zl        (1001) zl        (1001)     4541 2022-10-08 08:20:10.000000 aiei-1.0.3/aiei/misc/logger.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     7748 2022-10-08 08:20:10.000000 aiei-1.0.3/aiei/misc/mix.py
--rw-rw-r--   0 zl        (1001) zl        (1001)    20361 2021-09-18 03:42:29.000000 aiei-1.0.3/aiei/misc/summary.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     1484 2020-09-14 12:52:11.000000 aiei-1.0.3/aiei/misc/video.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     7633 2022-10-08 08:20:10.000000 aiei-1.0.3/aiei/misc/vis.py
-drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:11:48.487378 aiei-1.0.3/aiei/model/
--rw-rw-r--   0 zl        (1001) zl        (1001)        0 2018-08-15 03:47:04.000000 aiei-1.0.3/aiei/model/__init__.py
-drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:11:48.487378 aiei-1.0.3/aiei/model/backbones/
--rw-rw-r--   0 zl        (1001) zl        (1001)        0 2018-08-15 03:47:04.000000 aiei-1.0.3/aiei/model/backbones/__init__.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     4183 2020-09-28 06:53:33.000000 aiei-1.0.3/aiei/model/backbones/darknet.py
--rw-rw-r--   0 zl        (1001) zl        (1001)    11616 2020-08-15 04:11:50.000000 aiei-1.0.3/aiei/model/backbones/densenet.py
--rw-rw-r--   0 zl        (1001) zl        (1001)    17821 2022-10-08 08:20:10.000000 aiei-1.0.3/aiei/model/backbones/dla.py
--rw-rw-r--   0 zl        (1001) zl        (1001)    10018 2020-06-03 08:41:43.000000 aiei-1.0.3/aiei/model/backbones/efficientnet.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     6777 2020-01-15 15:13:30.000000 aiei-1.0.3/aiei/model/backbones/hgnet.py
--rw-rw-r--   0 zl        (1001) zl        (1001)    22062 2021-12-16 07:05:58.000000 aiei-1.0.3/aiei/model/backbones/highernet.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     7640 2022-10-08 08:20:10.000000 aiei-1.0.3/aiei/model/backbones/resnet.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     8405 2021-12-16 07:06:19.000000 aiei-1.0.3/aiei/model/backbones/shufflenetv2.py
--rw-rw-r--   0 zl        (1001) zl        (1001)    13540 2023-04-23 11:27:21.000000 aiei-1.0.3/aiei/model/backbones/tnet.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     1614 2021-09-09 02:09:26.000000 aiei-1.0.3/aiei/model/function.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     1360 2020-07-13 13:29:37.000000 aiei-1.0.3/aiei/model/init.py
-drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:11:48.487378 aiei-1.0.3/aiei/model/layers/
--rw-rw-r--   0 zl        (1001) zl        (1001)        0 2018-08-15 03:47:04.000000 aiei-1.0.3/aiei/model/layers/__init__.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     2013 2020-08-15 04:11:46.000000 aiei-1.0.3/aiei/model/layers/cbam.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     4330 2020-06-02 02:13:20.000000 aiei-1.0.3/aiei/model/layers/coord_conv.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     5408 2020-08-15 04:11:43.000000 aiei-1.0.3/aiei/model/layers/gau_fpa.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     8888 2020-08-15 04:11:40.000000 aiei-1.0.3/aiei/model/layers/norm.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     1609 2019-03-13 01:37:28.000000 aiei-1.0.3/aiei/model/layers/self_attention.py
--rw-rw-r--   0 zl        (1001) zl        (1001)    13805 2020-08-15 04:11:26.000000 aiei-1.0.3/aiei/model/zlayers.py
-drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:11:48.487378 aiei-1.0.3/aiei/ops/
-drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:11:48.491378 aiei-1.0.3/aiei/ops/FAIR/
-drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:11:48.491378 aiei-1.0.3/aiei/ops/FAIR/ROIAlign/
--rw-rw-r--   0 zl        (1001) zl        (1001)     2883 2020-03-10 04:13:18.000000 aiei-1.0.3/aiei/ops/FAIR/ROIAlign/ROIAlign.h
--rw-rw-r--   0 zl        (1001) zl        (1001)        0 2019-03-01 08:52:42.000000 aiei-1.0.3/aiei/ops/FAIR/__init__.py
--rw-rw-r--   0 zl        (1001) zl        (1001)    16089 2020-03-10 11:15:01.000000 aiei-1.0.3/aiei/ops/FAIR/deform_conv.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     1952 2020-02-27 13:27:36.000000 aiei-1.0.3/aiei/ops/FAIR/deform_conv_with_off.py
-drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:11:48.491378 aiei-1.0.3/aiei/ops/FAIR/deformable/
--rw-rw-r--   0 zl        (1001) zl        (1001)     8235 2020-03-10 04:13:18.000000 aiei-1.0.3/aiei/ops/FAIR/deformable/deform_conv.h
--rw-rw-r--   0 zl        (1001) zl        (1001)     6570 2020-03-10 11:16:09.000000 aiei-1.0.3/aiei/ops/FAIR/nms.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     3994 2020-03-10 11:16:28.000000 aiei-1.0.3/aiei/ops/FAIR/roi_align.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     2766 2022-10-08 08:21:27.000000 aiei-1.0.3/aiei/ops/FAIR/setup.py
--rw-rw-r--   0 zl        (1001) zl        (1001)       69 2021-09-03 17:23:39.000000 aiei-1.0.3/aiei/ops/__init__.py
-drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:11:48.491378 aiei-1.0.3/aiei/ops/dcnv2/
--rw-rw-r--   0 zl        (1001) zl        (1001)      622 2019-05-02 07:07:28.000000 aiei-1.0.3/aiei/ops/dcnv2/__init__.py
-drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:11:48.491378 aiei-1.0.3/aiei/ops/dcnv2/functions/
--rw-rw-r--   0 zl        (1001) zl        (1001)        0 2019-05-02 07:07:28.000000 aiei-1.0.3/aiei/ops/dcnv2/functions/__init__.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     7291 2020-01-19 16:28:33.000000 aiei-1.0.3/aiei/ops/dcnv2/functions/deform_conv.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     2370 2019-05-02 07:07:28.000000 aiei-1.0.3/aiei/ops/dcnv2/functions/deform_pool.py
-drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:11:48.491378 aiei-1.0.3/aiei/ops/dcnv2/modules/
--rw-rw-r--   0 zl        (1001) zl        (1001)        0 2019-05-02 07:07:28.000000 aiei-1.0.3/aiei/ops/dcnv2/modules/__init__.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     4714 2020-01-19 16:30:05.000000 aiei-1.0.3/aiei/ops/dcnv2/modules/deform_conv.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     6313 2019-05-02 07:07:28.000000 aiei-1.0.3/aiei/ops/dcnv2/modules/deform_pool.py
--rw-rw-r--   0 zl        (1001) zl        (1001)      469 2019-05-02 07:07:28.000000 aiei-1.0.3/aiei/ops/dcnv2/setup.py
-drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:11:48.491378 aiei-1.0.3/aiei/ops/nms/
--rw-rw-r--   0 zl        (1001) zl        (1001)       70 2020-03-12 02:14:20.000000 aiei-1.0.3/aiei/ops/nms/__init__.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     6038 2022-10-08 08:21:43.000000 aiei-1.0.3/aiei/ops/nms/nms_wrapper.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     1122 2022-10-08 08:21:47.000000 aiei-1.0.3/aiei/ops/nms/setup.py
-drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:11:48.491378 aiei-1.0.3/aiei/optim/
--rw-rw-r--   0 zl        (1001) zl        (1001)        0 2019-03-01 08:52:42.000000 aiei-1.0.3/aiei/optim/__init__.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     2945 2020-03-08 14:25:31.000000 aiei-1.0.3/aiei/optim/lr_scheduler.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     7906 2019-08-16 05:35:14.000000 aiei-1.0.3/aiei/optim/radam.py
--rw-rw-r--   0 zl        (1001) zl        (1001)      815 2019-08-08 03:56:08.000000 aiei-1.0.3/aiei/optim/swish.py
-drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:11:48.491378 aiei-1.0.3/aiei/spec/
--rw-rw-r--   0 zl        (1001) zl        (1001)        0 2018-08-14 13:29:54.000000 aiei-1.0.3/aiei/spec/__init__.py
-drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:11:48.495378 aiei-1.0.3/aiei/spec/det/
--rw-rw-r--   0 zl        (1001) zl        (1001)        0 2020-07-28 08:43:38.000000 aiei-1.0.3/aiei/spec/det/__init__.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     2422 2020-07-31 10:30:25.000000 aiei-1.0.3/aiei/spec/det/ious.py
-drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:11:48.479378 aiei-1.0.3/aiei.egg-info/
--rw-rw-r--   0 zl        (1001) zl        (1001)     1203 2023-04-23 12:11:48.000000 aiei-1.0.3/aiei.egg-info/PKG-INFO
--rw-rw-r--   0 zl        (1001) zl        (1001)     2618 2023-04-23 12:11:48.000000 aiei-1.0.3/aiei.egg-info/SOURCES.txt
--rw-rw-r--   0 zl        (1001) zl        (1001)        1 2023-04-23 12:11:48.000000 aiei-1.0.3/aiei.egg-info/dependency_links.txt
--rw-rw-r--   0 zl        (1001) zl        (1001)        1 2021-09-16 04:07:06.000000 aiei-1.0.3/aiei.egg-info/not-zip-safe
--rw-rw-r--   0 zl        (1001) zl        (1001)       95 2023-04-23 12:11:48.000000 aiei-1.0.3/aiei.egg-info/requires.txt
--rw-rw-r--   0 zl        (1001) zl        (1001)        5 2023-04-23 12:11:48.000000 aiei-1.0.3/aiei.egg-info/top_level.txt
-drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:11:48.495378 aiei-1.0.3/requirements/
--rw-rw-r--   0 zl        (1001) zl        (1001)        6 2020-11-09 07:51:42.000000 aiei-1.0.3/requirements/develop.txt
--rw-rw-r--   0 zl        (1001) zl        (1001)      218 2021-09-07 03:39:00.000000 aiei-1.0.3/requirements/requirements.txt
--rw-rw-r--   0 zl        (1001) zl        (1001)       38 2023-04-23 12:11:48.499378 aiei-1.0.3/setup.cfg
--rw-rw-r--   0 zl        (1001) zl        (1001)     6010 2023-03-01 12:35:34.000000 aiei-1.0.3/setup.py
-drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:11:48.495378 aiei-1.0.3/tools/
--rw-rw-r--   0 zl        (1001) zl        (1001)     2150 2022-10-08 08:20:10.000000 aiei-1.0.3/tools/aiei
+drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:24:59.151449 aiei-1.0.4/
+-rw-rw-r--   0 zl        (1001) zl        (1001)       52 2020-11-09 02:20:47.000000 aiei-1.0.4/MANIFEST.in
+-rw-rw-r--   0 zl        (1001) zl        (1001)     1203 2023-04-23 12:24:59.151449 aiei-1.0.4/PKG-INFO
+-rw-rw-r--   0 zl        (1001) zl        (1001)      381 2021-09-16 03:57:42.000000 aiei-1.0.4/README.md
+drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:24:59.131449 aiei-1.0.4/aiei/
+-rw-rw-r--   0 zl        (1001) zl        (1001)      103 2022-10-08 08:20:10.000000 aiei-1.0.4/aiei/__init__.py
+drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:24:59.135449 aiei-1.0.4/aiei/core/
+-rw-rw-r--   0 zl        (1001) zl        (1001)        0 2020-09-30 08:03:24.000000 aiei-1.0.4/aiei/core/__init__.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)    20954 2023-04-23 12:22:23.000000 aiei-1.0.4/aiei/core/aiei.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)    12553 2023-04-23 11:53:00.000000 aiei-1.0.4/aiei/core/base_config.py
+drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:24:59.135449 aiei-1.0.4/aiei/ctrib/
+-rw-rw-r--   0 zl        (1001) zl        (1001)        0 2019-01-22 03:50:05.000000 aiei-1.0.4/aiei/ctrib/__init__.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     8408 2019-03-13 14:17:09.000000 aiei-1.0.4/aiei/ctrib/dsn.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     7142 2022-05-23 14:12:33.000000 aiei-1.0.4/aiei/ctrib/soft_argmax.py
+drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:24:59.135449 aiei-1.0.4/aiei/data/
+-rw-rw-r--   0 zl        (1001) zl        (1001)        0 2019-01-22 02:30:50.000000 aiei-1.0.4/aiei/data/__init__.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     1402 2020-01-09 04:09:08.000000 aiei-1.0.4/aiei/data/mixup.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     5522 2021-09-08 08:26:09.000000 aiei-1.0.4/aiei/data/sampler.py
+drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:24:59.135449 aiei-1.0.4/aiei/data/set/
+-rw-rw-r--   0 zl        (1001) zl        (1001)        0 2019-01-22 02:30:50.000000 aiei-1.0.4/aiei/data/set/__init__.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)    18747 2021-12-16 06:48:44.000000 aiei-1.0.4/aiei/data/set/coco.py
+drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:24:59.139449 aiei-1.0.4/aiei/data/transform/
+-rw-rw-r--   0 zl        (1001) zl        (1001)      522 2021-09-08 07:01:47.000000 aiei-1.0.4/aiei/data/transform/__init__.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     3937 2021-09-07 04:19:20.000000 aiei-1.0.4/aiei/data/transform/base_cls.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     6346 2021-09-07 06:35:16.000000 aiei-1.0.4/aiei/data/transform/base_fn.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     4390 2021-09-08 07:06:13.000000 aiei-1.0.4/aiei/data/transform/center_pad.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)      325 2021-09-08 07:07:16.000000 aiei-1.0.4/aiei/data/transform/normalize.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     7188 2021-11-07 09:07:41.000000 aiei-1.0.4/aiei/data/transform/random_affine.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)      560 2021-09-08 07:07:57.000000 aiei-1.0.4/aiei/data/transform/random_brightness.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)      569 2021-09-08 07:08:14.000000 aiei-1.0.4/aiei/data/transform/random_contrast.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     2343 2021-09-08 07:08:30.000000 aiei-1.0.4/aiei/data/transform/random_crop.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     1814 2021-09-08 07:08:43.000000 aiei-1.0.4/aiei/data/transform/random_erase.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     3030 2021-09-08 07:08:56.000000 aiei-1.0.4/aiei/data/transform/random_flip.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)      827 2021-09-08 07:09:17.000000 aiei-1.0.4/aiei/data/transform/random_lighting.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)      691 2021-09-08 07:09:30.000000 aiei-1.0.4/aiei/data/transform/random_saturation.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     3216 2021-11-07 09:03:15.000000 aiei-1.0.4/aiei/data/transform/resize_edge.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)      188 2021-09-08 07:10:01.000000 aiei-1.0.4/aiei/data/transform/to_tensor.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     1635 2020-07-31 01:17:10.000000 aiei-1.0.4/aiei/data/utils.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)      580 2023-04-23 12:24:51.000000 aiei-1.0.4/aiei/info.py
+drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:24:59.139449 aiei-1.0.4/aiei/misc/
+-rw-rw-r--   0 zl        (1001) zl        (1001)        0 2018-08-15 03:47:04.000000 aiei-1.0.4/aiei/misc/__init__.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     1133 2020-12-16 07:13:35.000000 aiei-1.0.4/aiei/misc/alg.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     3981 2020-05-11 11:28:08.000000 aiei-1.0.4/aiei/misc/dist.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     4920 2023-02-02 10:18:50.000000 aiei-1.0.4/aiei/misc/dotsi.py
+-rwxrwxr-x   0 zl        (1001) zl        (1001)     4541 2022-10-08 08:20:10.000000 aiei-1.0.4/aiei/misc/logger.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     7748 2022-10-08 08:20:10.000000 aiei-1.0.4/aiei/misc/mix.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)    20361 2021-09-18 03:42:29.000000 aiei-1.0.4/aiei/misc/summary.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     1484 2020-09-14 12:52:11.000000 aiei-1.0.4/aiei/misc/video.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     7633 2022-10-08 08:20:10.000000 aiei-1.0.4/aiei/misc/vis.py
+drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:24:59.139449 aiei-1.0.4/aiei/model/
+-rw-rw-r--   0 zl        (1001) zl        (1001)        0 2018-08-15 03:47:04.000000 aiei-1.0.4/aiei/model/__init__.py
+drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:24:59.143449 aiei-1.0.4/aiei/model/backbones/
+-rw-rw-r--   0 zl        (1001) zl        (1001)        0 2018-08-15 03:47:04.000000 aiei-1.0.4/aiei/model/backbones/__init__.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     4183 2020-09-28 06:53:33.000000 aiei-1.0.4/aiei/model/backbones/darknet.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)    11616 2020-08-15 04:11:50.000000 aiei-1.0.4/aiei/model/backbones/densenet.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)    17821 2022-10-08 08:20:10.000000 aiei-1.0.4/aiei/model/backbones/dla.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)    10018 2020-06-03 08:41:43.000000 aiei-1.0.4/aiei/model/backbones/efficientnet.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     6777 2020-01-15 15:13:30.000000 aiei-1.0.4/aiei/model/backbones/hgnet.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)    22062 2021-12-16 07:05:58.000000 aiei-1.0.4/aiei/model/backbones/highernet.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     7640 2022-10-08 08:20:10.000000 aiei-1.0.4/aiei/model/backbones/resnet.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     8405 2021-12-16 07:06:19.000000 aiei-1.0.4/aiei/model/backbones/shufflenetv2.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)    13540 2023-04-23 11:27:21.000000 aiei-1.0.4/aiei/model/backbones/tnet.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     1614 2021-09-09 02:09:26.000000 aiei-1.0.4/aiei/model/function.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     1360 2020-07-13 13:29:37.000000 aiei-1.0.4/aiei/model/init.py
+drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:24:59.143449 aiei-1.0.4/aiei/model/layers/
+-rw-rw-r--   0 zl        (1001) zl        (1001)        0 2018-08-15 03:47:04.000000 aiei-1.0.4/aiei/model/layers/__init__.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     2013 2020-08-15 04:11:46.000000 aiei-1.0.4/aiei/model/layers/cbam.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     4330 2020-06-02 02:13:20.000000 aiei-1.0.4/aiei/model/layers/coord_conv.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     5408 2020-08-15 04:11:43.000000 aiei-1.0.4/aiei/model/layers/gau_fpa.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     8888 2020-08-15 04:11:40.000000 aiei-1.0.4/aiei/model/layers/norm.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     1609 2019-03-13 01:37:28.000000 aiei-1.0.4/aiei/model/layers/self_attention.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)    13805 2020-08-15 04:11:26.000000 aiei-1.0.4/aiei/model/zlayers.py
+drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:24:59.143449 aiei-1.0.4/aiei/ops/
+drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:24:59.147449 aiei-1.0.4/aiei/ops/FAIR/
+drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:24:59.147449 aiei-1.0.4/aiei/ops/FAIR/ROIAlign/
+-rw-rw-r--   0 zl        (1001) zl        (1001)     2883 2020-03-10 04:13:18.000000 aiei-1.0.4/aiei/ops/FAIR/ROIAlign/ROIAlign.h
+-rw-rw-r--   0 zl        (1001) zl        (1001)        0 2019-03-01 08:52:42.000000 aiei-1.0.4/aiei/ops/FAIR/__init__.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)    16089 2020-03-10 11:15:01.000000 aiei-1.0.4/aiei/ops/FAIR/deform_conv.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     1952 2020-02-27 13:27:36.000000 aiei-1.0.4/aiei/ops/FAIR/deform_conv_with_off.py
+drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:24:59.147449 aiei-1.0.4/aiei/ops/FAIR/deformable/
+-rw-rw-r--   0 zl        (1001) zl        (1001)     8235 2020-03-10 04:13:18.000000 aiei-1.0.4/aiei/ops/FAIR/deformable/deform_conv.h
+-rw-rw-r--   0 zl        (1001) zl        (1001)     6570 2020-03-10 11:16:09.000000 aiei-1.0.4/aiei/ops/FAIR/nms.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     3994 2020-03-10 11:16:28.000000 aiei-1.0.4/aiei/ops/FAIR/roi_align.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     2766 2022-10-08 08:21:27.000000 aiei-1.0.4/aiei/ops/FAIR/setup.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)       69 2021-09-03 17:23:39.000000 aiei-1.0.4/aiei/ops/__init__.py
+drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:24:59.147449 aiei-1.0.4/aiei/ops/dcnv2/
+-rw-rw-r--   0 zl        (1001) zl        (1001)      622 2019-05-02 07:07:28.000000 aiei-1.0.4/aiei/ops/dcnv2/__init__.py
+drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:24:59.147449 aiei-1.0.4/aiei/ops/dcnv2/functions/
+-rw-rw-r--   0 zl        (1001) zl        (1001)        0 2019-05-02 07:07:28.000000 aiei-1.0.4/aiei/ops/dcnv2/functions/__init__.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     7291 2020-01-19 16:28:33.000000 aiei-1.0.4/aiei/ops/dcnv2/functions/deform_conv.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     2370 2019-05-02 07:07:28.000000 aiei-1.0.4/aiei/ops/dcnv2/functions/deform_pool.py
+drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:24:59.147449 aiei-1.0.4/aiei/ops/dcnv2/modules/
+-rw-rw-r--   0 zl        (1001) zl        (1001)        0 2019-05-02 07:07:28.000000 aiei-1.0.4/aiei/ops/dcnv2/modules/__init__.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     4714 2020-01-19 16:30:05.000000 aiei-1.0.4/aiei/ops/dcnv2/modules/deform_conv.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     6313 2019-05-02 07:07:28.000000 aiei-1.0.4/aiei/ops/dcnv2/modules/deform_pool.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)      469 2019-05-02 07:07:28.000000 aiei-1.0.4/aiei/ops/dcnv2/setup.py
+drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:24:59.147449 aiei-1.0.4/aiei/ops/nms/
+-rw-rw-r--   0 zl        (1001) zl        (1001)       70 2020-03-12 02:14:20.000000 aiei-1.0.4/aiei/ops/nms/__init__.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     6038 2022-10-08 08:21:43.000000 aiei-1.0.4/aiei/ops/nms/nms_wrapper.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     1122 2022-10-08 08:21:47.000000 aiei-1.0.4/aiei/ops/nms/setup.py
+drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:24:59.147449 aiei-1.0.4/aiei/optim/
+-rw-rw-r--   0 zl        (1001) zl        (1001)        0 2019-03-01 08:52:42.000000 aiei-1.0.4/aiei/optim/__init__.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     2945 2020-03-08 14:25:31.000000 aiei-1.0.4/aiei/optim/lr_scheduler.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     7906 2019-08-16 05:35:14.000000 aiei-1.0.4/aiei/optim/radam.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)      815 2019-08-08 03:56:08.000000 aiei-1.0.4/aiei/optim/swish.py
+drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:24:59.147449 aiei-1.0.4/aiei/spec/
+-rw-rw-r--   0 zl        (1001) zl        (1001)        0 2018-08-14 13:29:54.000000 aiei-1.0.4/aiei/spec/__init__.py
+drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:24:59.151449 aiei-1.0.4/aiei/spec/det/
+-rw-rw-r--   0 zl        (1001) zl        (1001)        0 2020-07-28 08:43:38.000000 aiei-1.0.4/aiei/spec/det/__init__.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     2422 2020-07-31 10:30:25.000000 aiei-1.0.4/aiei/spec/det/ious.py
+drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:24:59.135449 aiei-1.0.4/aiei.egg-info/
+-rw-rw-r--   0 zl        (1001) zl        (1001)     1203 2023-04-23 12:24:58.000000 aiei-1.0.4/aiei.egg-info/PKG-INFO
+-rw-rw-r--   0 zl        (1001) zl        (1001)     2618 2023-04-23 12:24:58.000000 aiei-1.0.4/aiei.egg-info/SOURCES.txt
+-rw-rw-r--   0 zl        (1001) zl        (1001)        1 2023-04-23 12:24:58.000000 aiei-1.0.4/aiei.egg-info/dependency_links.txt
+-rw-rw-r--   0 zl        (1001) zl        (1001)        1 2021-09-16 04:07:06.000000 aiei-1.0.4/aiei.egg-info/not-zip-safe
+-rw-rw-r--   0 zl        (1001) zl        (1001)       95 2023-04-23 12:24:58.000000 aiei-1.0.4/aiei.egg-info/requires.txt
+-rw-rw-r--   0 zl        (1001) zl        (1001)        5 2023-04-23 12:24:58.000000 aiei-1.0.4/aiei.egg-info/top_level.txt
+drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:24:59.151449 aiei-1.0.4/requirements/
+-rw-rw-r--   0 zl        (1001) zl        (1001)        6 2020-11-09 07:51:42.000000 aiei-1.0.4/requirements/develop.txt
+-rw-rw-r--   0 zl        (1001) zl        (1001)      218 2021-09-07 03:39:00.000000 aiei-1.0.4/requirements/requirements.txt
+-rw-rw-r--   0 zl        (1001) zl        (1001)       38 2023-04-23 12:24:59.151449 aiei-1.0.4/setup.cfg
+-rw-rw-r--   0 zl        (1001) zl        (1001)     6010 2023-03-01 12:35:34.000000 aiei-1.0.4/setup.py
+drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:24:59.151449 aiei-1.0.4/tools/
+-rw-rw-r--   0 zl        (1001) zl        (1001)     2150 2022-10-08 08:20:10.000000 aiei-1.0.4/tools/aiei
```

### Comparing `aiei-1.0.3/PKG-INFO` & `aiei-1.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiei
-Version: 1.0.3
+Version: 1.0.4
 Summary: A tiny framework for AI.
 Home-page: UNKNOWN
 Author: Lei Zhao
 Author-email: zlchn@qq.com
 License: Apache
 Project-URL: github, https://github.com/
 Description: ### Install AIEI
```

### Comparing `aiei-1.0.3/aiei/core/aiei.py` & `aiei-1.0.4/aiei/core/aiei.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,23 +151,25 @@
         if cfg.ZL != 0 and cfg.EVAL.USE_BEST_CKPT:
             path_ckpt_file = path_best_ckpt_file
         if os.path.exists(path_ckpt_file):
             # NOTE: map_location equal storage.cuda(local_rank), avoid default all on cuda(0). w/o cuda will be load on CPU
             ckpt = torch.load(path_ckpt_file, map_location=lambda storage, loc: storage)
             # self.model.load_state_dict({f'module.{k}': v for k, v in ckpt['state_dict'].items()})
             # self.model.load_state_dict({k.replace('module.', ''): v for k, v in ckpt['state_dict'].items()})
-            if cfg.TRAIN.RESUME == 1 or cfg.TRAIN.RESUME:
+            if cfg.TRAIN.RESUME == 1 or cfg.TRAIN.RESUME is True:
                 self.model.load_state_dict(ckpt['state_dict'])
             elif cfg.TRAIN.RESUME == 2:
                 m_state_dict = self.model.state_dict()
                 for k, v in ckpt['state_dict'].items():
                     if k not in m_state_dict:
                         continue
                     m_state_dict[k] = v
                 self.model.load_state_dict(m_state_dict)
+            # else:
+
             if 'extra' not in ckpt.keys() and 'extras' not in ckpt.keys():
                 cfg.LOG.INS.warning(f'Loading third-party model {path_ckpt_file.split("/").pop()}')
                 return  # not zl-ckpt format
             extra = ckpt['extra'] if 'extra' in ckpt else ckpt['extras']
             self._start_epoch = extra['epoch'] + 1
             self.global_step = extra['step'] if 'step' in extra else extra['steps']
             accuracy = extra['accuracy'] if 'accuracy' in extra else extra['perf_AP']
```

### Comparing `aiei-1.0.3/aiei/core/base_config.py` & `aiei-1.0.4/aiei/core/base_config.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/ctrib/dsn.py` & `aiei-1.0.4/aiei/ctrib/dsn.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/ctrib/soft_argmax.py` & `aiei-1.0.4/aiei/ctrib/soft_argmax.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/data/mixup.py` & `aiei-1.0.4/aiei/data/mixup.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/data/sampler.py` & `aiei-1.0.4/aiei/data/sampler.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/data/set/coco.py` & `aiei-1.0.4/aiei/data/set/coco.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/data/transform/__init__.py` & `aiei-1.0.4/aiei/data/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/data/transform/base_cls.py` & `aiei-1.0.4/aiei/data/transform/base_cls.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/data/transform/base_fn.py` & `aiei-1.0.4/aiei/data/transform/base_fn.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/data/transform/center_pad.py` & `aiei-1.0.4/aiei/data/transform/center_pad.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/data/transform/random_affine.py` & `aiei-1.0.4/aiei/data/transform/random_affine.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/data/transform/random_brightness.py` & `aiei-1.0.4/aiei/data/transform/random_brightness.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/data/transform/random_contrast.py` & `aiei-1.0.4/aiei/data/transform/random_contrast.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/data/transform/random_crop.py` & `aiei-1.0.4/aiei/data/transform/random_crop.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/data/transform/random_erase.py` & `aiei-1.0.4/aiei/data/transform/random_erase.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/data/transform/random_flip.py` & `aiei-1.0.4/aiei/data/transform/random_flip.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/data/transform/random_lighting.py` & `aiei-1.0.4/aiei/data/transform/random_lighting.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/data/transform/random_saturation.py` & `aiei-1.0.4/aiei/data/transform/random_saturation.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/data/transform/resize_edge.py` & `aiei-1.0.4/aiei/data/transform/resize_edge.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/data/utils.py` & `aiei-1.0.4/aiei/data/utils.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/info.py` & `aiei-1.0.4/aiei/info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 (c) ZL-2020.
 @author ZhaoLei
 @since 2020.10.29 22:20
 """
 INFO = dict(
     name='aiei',
-    version='1.0.3',
+    version='1.0.4',
     author='Lei Zhao',
     author_email='zlchn@qq.com',
     url='',
     project_urls={
         'github': 'https://github.com/',
     },
     description='A tiny framework for AI.',
```

### Comparing `aiei-1.0.3/aiei/misc/alg.py` & `aiei-1.0.4/aiei/misc/alg.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/misc/dist.py` & `aiei-1.0.4/aiei/misc/dist.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/misc/dotsi.py` & `aiei-1.0.4/aiei/misc/dotsi.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/misc/logger.py` & `aiei-1.0.4/aiei/misc/logger.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/misc/mix.py` & `aiei-1.0.4/aiei/misc/mix.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/misc/summary.py` & `aiei-1.0.4/aiei/misc/summary.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/misc/video.py` & `aiei-1.0.4/aiei/misc/video.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/misc/vis.py` & `aiei-1.0.4/aiei/misc/vis.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/model/backbones/darknet.py` & `aiei-1.0.4/aiei/model/backbones/darknet.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/model/backbones/densenet.py` & `aiei-1.0.4/aiei/model/backbones/densenet.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/model/backbones/dla.py` & `aiei-1.0.4/aiei/model/backbones/dla.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/model/backbones/efficientnet.py` & `aiei-1.0.4/aiei/model/backbones/efficientnet.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/model/backbones/hgnet.py` & `aiei-1.0.4/aiei/model/backbones/hgnet.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/model/backbones/highernet.py` & `aiei-1.0.4/aiei/model/backbones/highernet.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/model/backbones/resnet.py` & `aiei-1.0.4/aiei/model/backbones/resnet.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/model/backbones/shufflenetv2.py` & `aiei-1.0.4/aiei/model/backbones/shufflenetv2.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/model/backbones/tnet.py` & `aiei-1.0.4/aiei/model/backbones/tnet.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/model/function.py` & `aiei-1.0.4/aiei/model/function.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/model/init.py` & `aiei-1.0.4/aiei/model/init.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/model/layers/cbam.py` & `aiei-1.0.4/aiei/model/layers/cbam.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/model/layers/coord_conv.py` & `aiei-1.0.4/aiei/model/layers/coord_conv.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/model/layers/gau_fpa.py` & `aiei-1.0.4/aiei/model/layers/gau_fpa.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/model/layers/norm.py` & `aiei-1.0.4/aiei/model/layers/norm.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/model/layers/self_attention.py` & `aiei-1.0.4/aiei/model/layers/self_attention.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/model/zlayers.py` & `aiei-1.0.4/aiei/model/zlayers.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/ops/FAIR/ROIAlign/ROIAlign.h` & `aiei-1.0.4/aiei/ops/FAIR/ROIAlign/ROIAlign.h`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/ops/FAIR/deform_conv.py` & `aiei-1.0.4/aiei/ops/FAIR/deform_conv.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/ops/FAIR/deform_conv_with_off.py` & `aiei-1.0.4/aiei/ops/FAIR/deform_conv_with_off.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/ops/FAIR/deformable/deform_conv.h` & `aiei-1.0.4/aiei/ops/FAIR/deformable/deform_conv.h`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/ops/FAIR/nms.py` & `aiei-1.0.4/aiei/ops/FAIR/nms.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/ops/FAIR/roi_align.py` & `aiei-1.0.4/aiei/ops/FAIR/roi_align.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/ops/FAIR/setup.py` & `aiei-1.0.4/aiei/ops/FAIR/setup.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/ops/dcnv2/__init__.py` & `aiei-1.0.4/aiei/ops/dcnv2/__init__.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/ops/dcnv2/functions/deform_conv.py` & `aiei-1.0.4/aiei/ops/dcnv2/functions/deform_conv.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/ops/dcnv2/functions/deform_pool.py` & `aiei-1.0.4/aiei/ops/dcnv2/functions/deform_pool.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/ops/dcnv2/modules/deform_conv.py` & `aiei-1.0.4/aiei/ops/dcnv2/modules/deform_conv.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/ops/dcnv2/modules/deform_pool.py` & `aiei-1.0.4/aiei/ops/dcnv2/modules/deform_pool.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/ops/nms/nms_wrapper.py` & `aiei-1.0.4/aiei/ops/nms/nms_wrapper.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/ops/nms/setup.py` & `aiei-1.0.4/aiei/ops/nms/setup.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/optim/lr_scheduler.py` & `aiei-1.0.4/aiei/optim/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/optim/radam.py` & `aiei-1.0.4/aiei/optim/radam.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/optim/swish.py` & `aiei-1.0.4/aiei/optim/swish.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei/spec/det/ious.py` & `aiei-1.0.4/aiei/spec/det/ious.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/aiei.egg-info/PKG-INFO` & `aiei-1.0.4/aiei.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiei
-Version: 1.0.3
+Version: 1.0.4
 Summary: A tiny framework for AI.
 Home-page: UNKNOWN
 Author: Lei Zhao
 Author-email: zlchn@qq.com
 License: Apache
 Project-URL: github, https://github.com/
 Description: ### Install AIEI
```

### Comparing `aiei-1.0.3/aiei.egg-info/SOURCES.txt` & `aiei-1.0.4/aiei.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/setup.py` & `aiei-1.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.3/tools/aiei` & `aiei-1.0.4/tools/aiei`

 * *Files identical despite different names*
