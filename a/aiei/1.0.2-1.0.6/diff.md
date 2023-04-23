# Comparing `tmp/aiei-1.0.2.tar.gz` & `tmp/aiei-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiei-1.0.2.tar", last modified: Wed Mar  1 12:35:42 2023, max compression
+gzip compressed data, was "aiei-1.0.6.tar", last modified: Sun Apr 23 12:43:25 2023, max compression
```

## Comparing `aiei-1.0.2.tar` & `aiei-1.0.6.tar`

### file list

```diff
@@ -1,124 +1,124 @@
-drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-03-01 12:35:42.874122 aiei-1.0.2/
--rw-rw-r--   0 zl        (1001) zl        (1001)       52 2020-11-09 02:20:47.000000 aiei-1.0.2/MANIFEST.in
--rw-rw-r--   0 zl        (1001) zl        (1001)     1203 2023-03-01 12:35:42.874122 aiei-1.0.2/PKG-INFO
--rw-rw-r--   0 zl        (1001) zl        (1001)      381 2021-09-16 03:57:42.000000 aiei-1.0.2/README.md
-drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-03-01 12:35:42.854122 aiei-1.0.2/aiei/
--rw-rw-r--   0 zl        (1001) zl        (1001)      103 2022-10-08 08:20:10.000000 aiei-1.0.2/aiei/__init__.py
-drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-03-01 12:35:42.854122 aiei-1.0.2/aiei/core/
--rw-rw-r--   0 zl        (1001) zl        (1001)        0 2020-09-30 08:03:24.000000 aiei-1.0.2/aiei/core/__init__.py
--rw-rw-r--   0 zl        (1001) zl        (1001)    20565 2023-03-01 07:38:33.000000 aiei-1.0.2/aiei/core/aiei.py
--rw-rw-r--   0 zl        (1001) zl        (1001)    12504 2023-03-01 12:30:43.000000 aiei-1.0.2/aiei/core/base_config.py
-drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-03-01 12:35:42.854122 aiei-1.0.2/aiei/ctrib/
--rw-rw-r--   0 zl        (1001) zl        (1001)        0 2019-01-22 03:50:05.000000 aiei-1.0.2/aiei/ctrib/__init__.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     8408 2019-03-13 14:17:09.000000 aiei-1.0.2/aiei/ctrib/dsn.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     7142 2022-05-23 14:12:33.000000 aiei-1.0.2/aiei/ctrib/soft_argmax.py
-drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-03-01 12:35:42.858121 aiei-1.0.2/aiei/data/
--rw-rw-r--   0 zl        (1001) zl        (1001)        0 2019-01-22 02:30:50.000000 aiei-1.0.2/aiei/data/__init__.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     1402 2020-01-09 04:09:08.000000 aiei-1.0.2/aiei/data/mixup.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     5522 2021-09-08 08:26:09.000000 aiei-1.0.2/aiei/data/sampler.py
-drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-03-01 12:35:42.858121 aiei-1.0.2/aiei/data/set/
--rw-rw-r--   0 zl        (1001) zl        (1001)        0 2019-01-22 02:30:50.000000 aiei-1.0.2/aiei/data/set/__init__.py
--rw-rw-r--   0 zl        (1001) zl        (1001)    18747 2021-12-16 06:48:44.000000 aiei-1.0.2/aiei/data/set/coco.py
-drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-03-01 12:35:42.858121 aiei-1.0.2/aiei/data/transform/
--rw-rw-r--   0 zl        (1001) zl        (1001)      522 2021-09-08 07:01:47.000000 aiei-1.0.2/aiei/data/transform/__init__.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     3937 2021-09-07 04:19:20.000000 aiei-1.0.2/aiei/data/transform/base_cls.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     6346 2021-09-07 06:35:16.000000 aiei-1.0.2/aiei/data/transform/base_fn.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     4390 2021-09-08 07:06:13.000000 aiei-1.0.2/aiei/data/transform/center_pad.py
--rw-rw-r--   0 zl        (1001) zl        (1001)      325 2021-09-08 07:07:16.000000 aiei-1.0.2/aiei/data/transform/normalize.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     7188 2021-11-07 09:07:41.000000 aiei-1.0.2/aiei/data/transform/random_affine.py
--rw-rw-r--   0 zl        (1001) zl        (1001)      560 2021-09-08 07:07:57.000000 aiei-1.0.2/aiei/data/transform/random_brightness.py
--rw-rw-r--   0 zl        (1001) zl        (1001)      569 2021-09-08 07:08:14.000000 aiei-1.0.2/aiei/data/transform/random_contrast.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     2343 2021-09-08 07:08:30.000000 aiei-1.0.2/aiei/data/transform/random_crop.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     1814 2021-09-08 07:08:43.000000 aiei-1.0.2/aiei/data/transform/random_erase.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     3030 2021-09-08 07:08:56.000000 aiei-1.0.2/aiei/data/transform/random_flip.py
--rw-rw-r--   0 zl        (1001) zl        (1001)      827 2021-09-08 07:09:17.000000 aiei-1.0.2/aiei/data/transform/random_lighting.py
--rw-rw-r--   0 zl        (1001) zl        (1001)      691 2021-09-08 07:09:30.000000 aiei-1.0.2/aiei/data/transform/random_saturation.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     3216 2021-11-07 09:03:15.000000 aiei-1.0.2/aiei/data/transform/resize_edge.py
--rw-rw-r--   0 zl        (1001) zl        (1001)      188 2021-09-08 07:10:01.000000 aiei-1.0.2/aiei/data/transform/to_tensor.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     1635 2020-07-31 01:17:10.000000 aiei-1.0.2/aiei/data/utils.py
--rw-rw-r--   0 zl        (1001) zl        (1001)      580 2023-03-01 12:31:51.000000 aiei-1.0.2/aiei/info.py
-drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-03-01 12:35:42.862122 aiei-1.0.2/aiei/misc/
--rw-rw-r--   0 zl        (1001) zl        (1001)        0 2018-08-15 03:47:04.000000 aiei-1.0.2/aiei/misc/__init__.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     1133 2020-12-16 07:13:35.000000 aiei-1.0.2/aiei/misc/alg.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     3981 2020-05-11 11:28:08.000000 aiei-1.0.2/aiei/misc/dist.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     4920 2023-02-02 10:18:50.000000 aiei-1.0.2/aiei/misc/dotsi.py
--rwxrwxr-x   0 zl        (1001) zl        (1001)     4541 2022-10-08 08:20:10.000000 aiei-1.0.2/aiei/misc/logger.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     7748 2022-10-08 08:20:10.000000 aiei-1.0.2/aiei/misc/mix.py
--rw-rw-r--   0 zl        (1001) zl        (1001)    20361 2021-09-18 03:42:29.000000 aiei-1.0.2/aiei/misc/summary.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     1484 2020-09-14 12:52:11.000000 aiei-1.0.2/aiei/misc/video.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     7633 2022-10-08 08:20:10.000000 aiei-1.0.2/aiei/misc/vis.py
-drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-03-01 12:35:42.862122 aiei-1.0.2/aiei/model/
--rw-rw-r--   0 zl        (1001) zl        (1001)        0 2018-08-15 03:47:04.000000 aiei-1.0.2/aiei/model/__init__.py
-drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-03-01 12:35:42.862122 aiei-1.0.2/aiei/model/backbones/
--rw-rw-r--   0 zl        (1001) zl        (1001)        0 2018-08-15 03:47:04.000000 aiei-1.0.2/aiei/model/backbones/__init__.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     4183 2020-09-28 06:53:33.000000 aiei-1.0.2/aiei/model/backbones/darknet.py
--rw-rw-r--   0 zl        (1001) zl        (1001)    11616 2020-08-15 04:11:50.000000 aiei-1.0.2/aiei/model/backbones/densenet.py
--rw-rw-r--   0 zl        (1001) zl        (1001)    17821 2022-10-08 08:20:10.000000 aiei-1.0.2/aiei/model/backbones/dla.py
--rw-rw-r--   0 zl        (1001) zl        (1001)    10018 2020-06-03 08:41:43.000000 aiei-1.0.2/aiei/model/backbones/efficientnet.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     6777 2020-01-15 15:13:30.000000 aiei-1.0.2/aiei/model/backbones/hgnet.py
--rw-rw-r--   0 zl        (1001) zl        (1001)    22062 2021-12-16 07:05:58.000000 aiei-1.0.2/aiei/model/backbones/highernet.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     7640 2022-10-08 08:20:10.000000 aiei-1.0.2/aiei/model/backbones/resnet.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     8405 2021-12-16 07:06:19.000000 aiei-1.0.2/aiei/model/backbones/shufflenetv2.py
--rw-rw-r--   0 zl        (1001) zl        (1001)    13343 2022-10-10 09:31:16.000000 aiei-1.0.2/aiei/model/backbones/tnet.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     1614 2021-09-09 02:09:26.000000 aiei-1.0.2/aiei/model/function.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     1360 2020-07-13 13:29:37.000000 aiei-1.0.2/aiei/model/init.py
-drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-03-01 12:35:42.862122 aiei-1.0.2/aiei/model/layers/
--rw-rw-r--   0 zl        (1001) zl        (1001)        0 2018-08-15 03:47:04.000000 aiei-1.0.2/aiei/model/layers/__init__.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     2013 2020-08-15 04:11:46.000000 aiei-1.0.2/aiei/model/layers/cbam.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     4330 2020-06-02 02:13:20.000000 aiei-1.0.2/aiei/model/layers/coord_conv.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     5408 2020-08-15 04:11:43.000000 aiei-1.0.2/aiei/model/layers/gau_fpa.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     8888 2020-08-15 04:11:40.000000 aiei-1.0.2/aiei/model/layers/norm.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     1609 2019-03-13 01:37:28.000000 aiei-1.0.2/aiei/model/layers/self_attention.py
--rw-rw-r--   0 zl        (1001) zl        (1001)    13805 2020-08-15 04:11:26.000000 aiei-1.0.2/aiei/model/zlayers.py
-drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-03-01 12:35:42.862122 aiei-1.0.2/aiei/ops/
-drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-03-01 12:35:42.862122 aiei-1.0.2/aiei/ops/FAIR/
-drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-03-01 12:35:42.862122 aiei-1.0.2/aiei/ops/FAIR/ROIAlign/
--rw-rw-r--   0 zl        (1001) zl        (1001)     2883 2020-03-10 04:13:18.000000 aiei-1.0.2/aiei/ops/FAIR/ROIAlign/ROIAlign.h
--rw-rw-r--   0 zl        (1001) zl        (1001)        0 2019-03-01 08:52:42.000000 aiei-1.0.2/aiei/ops/FAIR/__init__.py
--rw-rw-r--   0 zl        (1001) zl        (1001)    16089 2020-03-10 11:15:01.000000 aiei-1.0.2/aiei/ops/FAIR/deform_conv.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     1952 2020-02-27 13:27:36.000000 aiei-1.0.2/aiei/ops/FAIR/deform_conv_with_off.py
-drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-03-01 12:35:42.862122 aiei-1.0.2/aiei/ops/FAIR/deformable/
--rw-rw-r--   0 zl        (1001) zl        (1001)     8235 2020-03-10 04:13:18.000000 aiei-1.0.2/aiei/ops/FAIR/deformable/deform_conv.h
--rw-rw-r--   0 zl        (1001) zl        (1001)     6570 2020-03-10 11:16:09.000000 aiei-1.0.2/aiei/ops/FAIR/nms.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     3994 2020-03-10 11:16:28.000000 aiei-1.0.2/aiei/ops/FAIR/roi_align.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     2766 2022-10-08 08:21:27.000000 aiei-1.0.2/aiei/ops/FAIR/setup.py
--rw-rw-r--   0 zl        (1001) zl        (1001)       69 2021-09-03 17:23:39.000000 aiei-1.0.2/aiei/ops/__init__.py
-drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-03-01 12:35:42.862122 aiei-1.0.2/aiei/ops/dcnv2/
--rw-rw-r--   0 zl        (1001) zl        (1001)      622 2019-05-02 07:07:28.000000 aiei-1.0.2/aiei/ops/dcnv2/__init__.py
-drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-03-01 12:35:42.862122 aiei-1.0.2/aiei/ops/dcnv2/functions/
--rw-rw-r--   0 zl        (1001) zl        (1001)        0 2019-05-02 07:07:28.000000 aiei-1.0.2/aiei/ops/dcnv2/functions/__init__.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     7291 2020-01-19 16:28:33.000000 aiei-1.0.2/aiei/ops/dcnv2/functions/deform_conv.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     2370 2019-05-02 07:07:28.000000 aiei-1.0.2/aiei/ops/dcnv2/functions/deform_pool.py
-drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-03-01 12:35:42.862122 aiei-1.0.2/aiei/ops/dcnv2/modules/
--rw-rw-r--   0 zl        (1001) zl        (1001)        0 2019-05-02 07:07:28.000000 aiei-1.0.2/aiei/ops/dcnv2/modules/__init__.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     4714 2020-01-19 16:30:05.000000 aiei-1.0.2/aiei/ops/dcnv2/modules/deform_conv.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     6313 2019-05-02 07:07:28.000000 aiei-1.0.2/aiei/ops/dcnv2/modules/deform_pool.py
--rw-rw-r--   0 zl        (1001) zl        (1001)      469 2019-05-02 07:07:28.000000 aiei-1.0.2/aiei/ops/dcnv2/setup.py
-drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-03-01 12:35:42.866122 aiei-1.0.2/aiei/ops/nms/
--rw-rw-r--   0 zl        (1001) zl        (1001)       70 2020-03-12 02:14:20.000000 aiei-1.0.2/aiei/ops/nms/__init__.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     6038 2022-10-08 08:21:43.000000 aiei-1.0.2/aiei/ops/nms/nms_wrapper.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     1122 2022-10-08 08:21:47.000000 aiei-1.0.2/aiei/ops/nms/setup.py
-drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-03-01 12:35:42.866122 aiei-1.0.2/aiei/optim/
--rw-rw-r--   0 zl        (1001) zl        (1001)        0 2019-03-01 08:52:42.000000 aiei-1.0.2/aiei/optim/__init__.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     2945 2020-03-08 14:25:31.000000 aiei-1.0.2/aiei/optim/lr_scheduler.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     7906 2019-08-16 05:35:14.000000 aiei-1.0.2/aiei/optim/radam.py
--rw-rw-r--   0 zl        (1001) zl        (1001)      815 2019-08-08 03:56:08.000000 aiei-1.0.2/aiei/optim/swish.py
-drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-03-01 12:35:42.866122 aiei-1.0.2/aiei/spec/
--rw-rw-r--   0 zl        (1001) zl        (1001)        0 2018-08-14 13:29:54.000000 aiei-1.0.2/aiei/spec/__init__.py
-drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-03-01 12:35:42.866122 aiei-1.0.2/aiei/spec/det/
--rw-rw-r--   0 zl        (1001) zl        (1001)        0 2020-07-28 08:43:38.000000 aiei-1.0.2/aiei/spec/det/__init__.py
--rw-rw-r--   0 zl        (1001) zl        (1001)     2422 2020-07-31 10:30:25.000000 aiei-1.0.2/aiei/spec/det/ious.py
-drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-03-01 12:35:42.854122 aiei-1.0.2/aiei.egg-info/
--rw-rw-r--   0 zl        (1001) zl        (1001)     1203 2023-03-01 12:35:42.000000 aiei-1.0.2/aiei.egg-info/PKG-INFO
--rw-rw-r--   0 zl        (1001) zl        (1001)     2618 2023-03-01 12:35:42.000000 aiei-1.0.2/aiei.egg-info/SOURCES.txt
--rw-rw-r--   0 zl        (1001) zl        (1001)        1 2023-03-01 12:35:42.000000 aiei-1.0.2/aiei.egg-info/dependency_links.txt
--rw-rw-r--   0 zl        (1001) zl        (1001)        1 2021-09-16 04:07:06.000000 aiei-1.0.2/aiei.egg-info/not-zip-safe
--rw-rw-r--   0 zl        (1001) zl        (1001)       95 2023-03-01 12:35:42.000000 aiei-1.0.2/aiei.egg-info/requires.txt
--rw-rw-r--   0 zl        (1001) zl        (1001)        5 2023-03-01 12:35:42.000000 aiei-1.0.2/aiei.egg-info/top_level.txt
-drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-03-01 12:35:42.866122 aiei-1.0.2/requirements/
--rw-rw-r--   0 zl        (1001) zl        (1001)        6 2020-11-09 07:51:42.000000 aiei-1.0.2/requirements/develop.txt
--rw-rw-r--   0 zl        (1001) zl        (1001)      218 2021-09-07 03:39:00.000000 aiei-1.0.2/requirements/requirements.txt
--rw-rw-r--   0 zl        (1001) zl        (1001)       38 2023-03-01 12:35:42.874122 aiei-1.0.2/setup.cfg
--rw-rw-r--   0 zl        (1001) zl        (1001)     6010 2023-03-01 12:35:34.000000 aiei-1.0.2/setup.py
-drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-03-01 12:35:42.866122 aiei-1.0.2/tools/
--rw-rw-r--   0 zl        (1001) zl        (1001)     2150 2022-10-08 08:20:10.000000 aiei-1.0.2/tools/aiei
+drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:43:25.845600 aiei-1.0.6/
+-rw-rw-r--   0 zl        (1001) zl        (1001)       52 2020-11-09 02:20:47.000000 aiei-1.0.6/MANIFEST.in
+-rw-rw-r--   0 zl        (1001) zl        (1001)     1203 2023-04-23 12:43:25.845600 aiei-1.0.6/PKG-INFO
+-rw-rw-r--   0 zl        (1001) zl        (1001)      381 2021-09-16 03:57:42.000000 aiei-1.0.6/README.md
+drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:43:25.829600 aiei-1.0.6/aiei/
+-rw-rw-r--   0 zl        (1001) zl        (1001)      103 2022-10-08 08:20:10.000000 aiei-1.0.6/aiei/__init__.py
+drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:43:25.829600 aiei-1.0.6/aiei/core/
+-rw-rw-r--   0 zl        (1001) zl        (1001)        0 2020-09-30 08:03:24.000000 aiei-1.0.6/aiei/core/__init__.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)    20938 2023-04-23 12:42:50.000000 aiei-1.0.6/aiei/core/aiei.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)    12553 2023-04-23 11:53:00.000000 aiei-1.0.6/aiei/core/base_config.py
+drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:43:25.833600 aiei-1.0.6/aiei/ctrib/
+-rw-rw-r--   0 zl        (1001) zl        (1001)        0 2019-01-22 03:50:05.000000 aiei-1.0.6/aiei/ctrib/__init__.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     8408 2019-03-13 14:17:09.000000 aiei-1.0.6/aiei/ctrib/dsn.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     7142 2022-05-23 14:12:33.000000 aiei-1.0.6/aiei/ctrib/soft_argmax.py
+drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:43:25.833600 aiei-1.0.6/aiei/data/
+-rw-rw-r--   0 zl        (1001) zl        (1001)        0 2019-01-22 02:30:50.000000 aiei-1.0.6/aiei/data/__init__.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     1402 2020-01-09 04:09:08.000000 aiei-1.0.6/aiei/data/mixup.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     5522 2021-09-08 08:26:09.000000 aiei-1.0.6/aiei/data/sampler.py
+drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:43:25.833600 aiei-1.0.6/aiei/data/set/
+-rw-rw-r--   0 zl        (1001) zl        (1001)        0 2019-01-22 02:30:50.000000 aiei-1.0.6/aiei/data/set/__init__.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)    18747 2021-12-16 06:48:44.000000 aiei-1.0.6/aiei/data/set/coco.py
+drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:43:25.833600 aiei-1.0.6/aiei/data/transform/
+-rw-rw-r--   0 zl        (1001) zl        (1001)      522 2021-09-08 07:01:47.000000 aiei-1.0.6/aiei/data/transform/__init__.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     3937 2021-09-07 04:19:20.000000 aiei-1.0.6/aiei/data/transform/base_cls.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     6346 2021-09-07 06:35:16.000000 aiei-1.0.6/aiei/data/transform/base_fn.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     4390 2021-09-08 07:06:13.000000 aiei-1.0.6/aiei/data/transform/center_pad.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)      325 2021-09-08 07:07:16.000000 aiei-1.0.6/aiei/data/transform/normalize.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     7188 2021-11-07 09:07:41.000000 aiei-1.0.6/aiei/data/transform/random_affine.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)      560 2021-09-08 07:07:57.000000 aiei-1.0.6/aiei/data/transform/random_brightness.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)      569 2021-09-08 07:08:14.000000 aiei-1.0.6/aiei/data/transform/random_contrast.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     2343 2021-09-08 07:08:30.000000 aiei-1.0.6/aiei/data/transform/random_crop.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     1814 2021-09-08 07:08:43.000000 aiei-1.0.6/aiei/data/transform/random_erase.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     3030 2021-09-08 07:08:56.000000 aiei-1.0.6/aiei/data/transform/random_flip.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)      827 2021-09-08 07:09:17.000000 aiei-1.0.6/aiei/data/transform/random_lighting.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)      691 2021-09-08 07:09:30.000000 aiei-1.0.6/aiei/data/transform/random_saturation.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     3216 2021-11-07 09:03:15.000000 aiei-1.0.6/aiei/data/transform/resize_edge.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)      188 2021-09-08 07:10:01.000000 aiei-1.0.6/aiei/data/transform/to_tensor.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     1635 2020-07-31 01:17:10.000000 aiei-1.0.6/aiei/data/utils.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)      580 2023-04-23 12:43:06.000000 aiei-1.0.6/aiei/info.py
+drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:43:25.837600 aiei-1.0.6/aiei/misc/
+-rw-rw-r--   0 zl        (1001) zl        (1001)        0 2018-08-15 03:47:04.000000 aiei-1.0.6/aiei/misc/__init__.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     1133 2020-12-16 07:13:35.000000 aiei-1.0.6/aiei/misc/alg.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     3981 2020-05-11 11:28:08.000000 aiei-1.0.6/aiei/misc/dist.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     4920 2023-02-02 10:18:50.000000 aiei-1.0.6/aiei/misc/dotsi.py
+-rwxrwxr-x   0 zl        (1001) zl        (1001)     4541 2022-10-08 08:20:10.000000 aiei-1.0.6/aiei/misc/logger.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     7748 2022-10-08 08:20:10.000000 aiei-1.0.6/aiei/misc/mix.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)    20361 2021-09-18 03:42:29.000000 aiei-1.0.6/aiei/misc/summary.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     1484 2020-09-14 12:52:11.000000 aiei-1.0.6/aiei/misc/video.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     7633 2022-10-08 08:20:10.000000 aiei-1.0.6/aiei/misc/vis.py
+drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:43:25.837600 aiei-1.0.6/aiei/model/
+-rw-rw-r--   0 zl        (1001) zl        (1001)        0 2018-08-15 03:47:04.000000 aiei-1.0.6/aiei/model/__init__.py
+drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:43:25.837600 aiei-1.0.6/aiei/model/backbones/
+-rw-rw-r--   0 zl        (1001) zl        (1001)        0 2018-08-15 03:47:04.000000 aiei-1.0.6/aiei/model/backbones/__init__.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     4183 2020-09-28 06:53:33.000000 aiei-1.0.6/aiei/model/backbones/darknet.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)    11616 2020-08-15 04:11:50.000000 aiei-1.0.6/aiei/model/backbones/densenet.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)    17821 2022-10-08 08:20:10.000000 aiei-1.0.6/aiei/model/backbones/dla.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)    10018 2020-06-03 08:41:43.000000 aiei-1.0.6/aiei/model/backbones/efficientnet.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     6777 2020-01-15 15:13:30.000000 aiei-1.0.6/aiei/model/backbones/hgnet.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)    22062 2021-12-16 07:05:58.000000 aiei-1.0.6/aiei/model/backbones/highernet.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     7640 2022-10-08 08:20:10.000000 aiei-1.0.6/aiei/model/backbones/resnet.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     8405 2021-12-16 07:06:19.000000 aiei-1.0.6/aiei/model/backbones/shufflenetv2.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)    13540 2023-04-23 11:27:21.000000 aiei-1.0.6/aiei/model/backbones/tnet.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     1614 2021-09-09 02:09:26.000000 aiei-1.0.6/aiei/model/function.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     1360 2020-07-13 13:29:37.000000 aiei-1.0.6/aiei/model/init.py
+drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:43:25.837600 aiei-1.0.6/aiei/model/layers/
+-rw-rw-r--   0 zl        (1001) zl        (1001)        0 2018-08-15 03:47:04.000000 aiei-1.0.6/aiei/model/layers/__init__.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     2013 2020-08-15 04:11:46.000000 aiei-1.0.6/aiei/model/layers/cbam.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     4330 2020-06-02 02:13:20.000000 aiei-1.0.6/aiei/model/layers/coord_conv.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     5408 2020-08-15 04:11:43.000000 aiei-1.0.6/aiei/model/layers/gau_fpa.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     8888 2020-08-15 04:11:40.000000 aiei-1.0.6/aiei/model/layers/norm.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     1609 2019-03-13 01:37:28.000000 aiei-1.0.6/aiei/model/layers/self_attention.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)    13805 2020-08-15 04:11:26.000000 aiei-1.0.6/aiei/model/zlayers.py
+drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:43:25.841600 aiei-1.0.6/aiei/ops/
+drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:43:25.841600 aiei-1.0.6/aiei/ops/FAIR/
+drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:43:25.841600 aiei-1.0.6/aiei/ops/FAIR/ROIAlign/
+-rw-rw-r--   0 zl        (1001) zl        (1001)     2883 2020-03-10 04:13:18.000000 aiei-1.0.6/aiei/ops/FAIR/ROIAlign/ROIAlign.h
+-rw-rw-r--   0 zl        (1001) zl        (1001)        0 2019-03-01 08:52:42.000000 aiei-1.0.6/aiei/ops/FAIR/__init__.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)    16089 2020-03-10 11:15:01.000000 aiei-1.0.6/aiei/ops/FAIR/deform_conv.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     1952 2020-02-27 13:27:36.000000 aiei-1.0.6/aiei/ops/FAIR/deform_conv_with_off.py
+drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:43:25.841600 aiei-1.0.6/aiei/ops/FAIR/deformable/
+-rw-rw-r--   0 zl        (1001) zl        (1001)     8235 2020-03-10 04:13:18.000000 aiei-1.0.6/aiei/ops/FAIR/deformable/deform_conv.h
+-rw-rw-r--   0 zl        (1001) zl        (1001)     6570 2020-03-10 11:16:09.000000 aiei-1.0.6/aiei/ops/FAIR/nms.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     3994 2020-03-10 11:16:28.000000 aiei-1.0.6/aiei/ops/FAIR/roi_align.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     2766 2022-10-08 08:21:27.000000 aiei-1.0.6/aiei/ops/FAIR/setup.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)       69 2021-09-03 17:23:39.000000 aiei-1.0.6/aiei/ops/__init__.py
+drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:43:25.841600 aiei-1.0.6/aiei/ops/dcnv2/
+-rw-rw-r--   0 zl        (1001) zl        (1001)      622 2019-05-02 07:07:28.000000 aiei-1.0.6/aiei/ops/dcnv2/__init__.py
+drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:43:25.841600 aiei-1.0.6/aiei/ops/dcnv2/functions/
+-rw-rw-r--   0 zl        (1001) zl        (1001)        0 2019-05-02 07:07:28.000000 aiei-1.0.6/aiei/ops/dcnv2/functions/__init__.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     7291 2020-01-19 16:28:33.000000 aiei-1.0.6/aiei/ops/dcnv2/functions/deform_conv.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     2370 2019-05-02 07:07:28.000000 aiei-1.0.6/aiei/ops/dcnv2/functions/deform_pool.py
+drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:43:25.841600 aiei-1.0.6/aiei/ops/dcnv2/modules/
+-rw-rw-r--   0 zl        (1001) zl        (1001)        0 2019-05-02 07:07:28.000000 aiei-1.0.6/aiei/ops/dcnv2/modules/__init__.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     4714 2020-01-19 16:30:05.000000 aiei-1.0.6/aiei/ops/dcnv2/modules/deform_conv.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     6313 2019-05-02 07:07:28.000000 aiei-1.0.6/aiei/ops/dcnv2/modules/deform_pool.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)      469 2019-05-02 07:07:28.000000 aiei-1.0.6/aiei/ops/dcnv2/setup.py
+drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:43:25.841600 aiei-1.0.6/aiei/ops/nms/
+-rw-rw-r--   0 zl        (1001) zl        (1001)       70 2020-03-12 02:14:20.000000 aiei-1.0.6/aiei/ops/nms/__init__.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     6038 2022-10-08 08:21:43.000000 aiei-1.0.6/aiei/ops/nms/nms_wrapper.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     1122 2022-10-08 08:21:47.000000 aiei-1.0.6/aiei/ops/nms/setup.py
+drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:43:25.841600 aiei-1.0.6/aiei/optim/
+-rw-rw-r--   0 zl        (1001) zl        (1001)        0 2019-03-01 08:52:42.000000 aiei-1.0.6/aiei/optim/__init__.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     2945 2020-03-08 14:25:31.000000 aiei-1.0.6/aiei/optim/lr_scheduler.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     7906 2019-08-16 05:35:14.000000 aiei-1.0.6/aiei/optim/radam.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)      815 2019-08-08 03:56:08.000000 aiei-1.0.6/aiei/optim/swish.py
+drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:43:25.841600 aiei-1.0.6/aiei/spec/
+-rw-rw-r--   0 zl        (1001) zl        (1001)        0 2018-08-14 13:29:54.000000 aiei-1.0.6/aiei/spec/__init__.py
+drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:43:25.845600 aiei-1.0.6/aiei/spec/det/
+-rw-rw-r--   0 zl        (1001) zl        (1001)        0 2020-07-28 08:43:38.000000 aiei-1.0.6/aiei/spec/det/__init__.py
+-rw-rw-r--   0 zl        (1001) zl        (1001)     2422 2020-07-31 10:30:25.000000 aiei-1.0.6/aiei/spec/det/ious.py
+drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:43:25.829600 aiei-1.0.6/aiei.egg-info/
+-rw-rw-r--   0 zl        (1001) zl        (1001)     1203 2023-04-23 12:43:25.000000 aiei-1.0.6/aiei.egg-info/PKG-INFO
+-rw-rw-r--   0 zl        (1001) zl        (1001)     2618 2023-04-23 12:43:25.000000 aiei-1.0.6/aiei.egg-info/SOURCES.txt
+-rw-rw-r--   0 zl        (1001) zl        (1001)        1 2023-04-23 12:43:25.000000 aiei-1.0.6/aiei.egg-info/dependency_links.txt
+-rw-rw-r--   0 zl        (1001) zl        (1001)        1 2021-09-16 04:07:06.000000 aiei-1.0.6/aiei.egg-info/not-zip-safe
+-rw-rw-r--   0 zl        (1001) zl        (1001)       95 2023-04-23 12:43:25.000000 aiei-1.0.6/aiei.egg-info/requires.txt
+-rw-rw-r--   0 zl        (1001) zl        (1001)        5 2023-04-23 12:43:25.000000 aiei-1.0.6/aiei.egg-info/top_level.txt
+drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:43:25.845600 aiei-1.0.6/requirements/
+-rw-rw-r--   0 zl        (1001) zl        (1001)        6 2020-11-09 07:51:42.000000 aiei-1.0.6/requirements/develop.txt
+-rw-rw-r--   0 zl        (1001) zl        (1001)      218 2021-09-07 03:39:00.000000 aiei-1.0.6/requirements/requirements.txt
+-rw-rw-r--   0 zl        (1001) zl        (1001)       38 2023-04-23 12:43:25.845600 aiei-1.0.6/setup.cfg
+-rw-rw-r--   0 zl        (1001) zl        (1001)     6010 2023-03-01 12:35:34.000000 aiei-1.0.6/setup.py
+drwxrwxr-x   0 zl        (1001) zl        (1001)        0 2023-04-23 12:43:25.845600 aiei-1.0.6/tools/
+-rw-rw-r--   0 zl        (1001) zl        (1001)     2150 2022-10-08 08:20:10.000000 aiei-1.0.6/tools/aiei
```

### Comparing `aiei-1.0.2/PKG-INFO` & `aiei-1.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiei
-Version: 1.0.2
+Version: 1.0.6
 Summary: A tiny framework for AI.
 Home-page: UNKNOWN
 Author: Lei Zhao
 Author-email: zlchn@qq.com
 License: Apache
 Project-URL: github, https://github.com/
 Description: ### Install AIEI
```

### Comparing `aiei-1.0.2/aiei/core/aiei.py` & `aiei-1.0.6/aiei/core/aiei.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 import pprint
 import time
 import socket
 import shutil
 from datetime import datetime
 from tqdm import tqdm
 import cProfile
-import cv2
 import torch
 from torch import nn
 from torch.backends import cudnn
 from torch import distributed as dist
 from torch.cuda import amp
 from torch.utils.data import DataLoader
 from torch.utils.data.distributed import DistributedSampler
@@ -24,16 +23,14 @@
 
 from .base_config import cfg
 from ..data.sampler import GroupSampler, DistributedGroupSampler
 from ..misc import mix, summary
 from ..misc.logger import Logger
 from ..model import function
 
-cv2.setNumThreads(0)
-
 
 def _init_params():
     try:
         cfg._RECORD  # create in cfg.done()
     except Exception as e:
         raise ValueError(f'{e}. You should add "cfg.done()" afetr "cfg = Config()" or import core.aiei shouled be after config')
     # torch.cuda.init()
@@ -132,15 +129,15 @@
         self._start_epoch = 0
         self._best_epoch = 0
         self._best_accuracy = 0.0
         self.writer = _init_params()  # type: SummaryWriter
         self.model, self.optimizer = _init_model(model, optimizer)
         self.criterion = None if criterion is None else criterion.cuda()
         self._scaler = amp.GradScaler(enabled=cfg.FEAT.AMP)
-        if cfg.TRAIN.RESUME:
+        if cfg.TRAIN.RESUME > 0:
             self._resume()  # before scheduler
         self._lr_scheduler = None if optimizer is None else self.et_scheduler(-1 if self._start_epoch == 0 else self._start_epoch)
         self._train_loader = _init_train_loader(
             train_dataset, kwargs['train_collate_fn'] if
             ('train_collate_fn' in kwargs and kwargs['train_collate_fn'] is not None) else None)
         self._eval_loader = _init_eval_loader(
             eval_dataset, kwargs['eval_collate_fn'] if
@@ -154,27 +151,35 @@
         if cfg.ZL != 0 and cfg.EVAL.USE_BEST_CKPT:
             path_ckpt_file = path_best_ckpt_file
         if os.path.exists(path_ckpt_file):
             # NOTE: map_location equal storage.cuda(local_rank), avoid default all on cuda(0). w/o cuda will be load on CPU
             ckpt = torch.load(path_ckpt_file, map_location=lambda storage, loc: storage)
             # self.model.load_state_dict({f'module.{k}': v for k, v in ckpt['state_dict'].items()})
             # self.model.load_state_dict({k.replace('module.', ''): v for k, v in ckpt['state_dict'].items()})
-            self.model.load_state_dict(ckpt['state_dict'])
+            if cfg.TRAIN.RESUME == 1 or cfg.TRAIN.RESUME is True:
+                self.model.load_state_dict(ckpt['state_dict'])
+            elif cfg.TRAIN.RESUME == 2:
+                m_state_dict = self.model.state_dict()
+                for k, v in ckpt['state_dict'].items():
+                    if k not in m_state_dict:
+                        continue
+                    m_state_dict[k] = v
+                self.model.load_state_dict(m_state_dict)
             if 'extra' not in ckpt.keys() and 'extras' not in ckpt.keys():
                 cfg.LOG.INS.warning(f'Loading third-party model {path_ckpt_file.split("/").pop()}')
                 return  # not zl-ckpt format
             extra = ckpt['extra'] if 'extra' in ckpt else ckpt['extras']
             self._start_epoch = extra['epoch'] + 1
             self.global_step = extra['step'] if 'step' in extra else extra['steps']
             accuracy = extra['accuracy'] if 'accuracy' in extra else extra['perf_AP']
             cfg.LOG.INS.info(f"Loading {len(ckpt['state_dict'].keys())} keys from {path_ckpt_file.split('/').pop()} "
                 f"(epoch {self._start_epoch - 1}, step {self.global_step}, accuracy {accuracy:.5f})")
             if cfg.ZL != 0:
                 return
-            self.optimizer.load_state_dict(ckpt['optimizer'])
+            # self.optimizer.load_state_dict(ckpt['optimizer'])
             if cfg.FEAT.AMP and 'amp' in ckpt.keys():
                 self._scaler.load_state_dict(ckpt['amp'])
             if os.path.exists(path_best_ckpt_file):
                 ckpt = torch.load(path_best_ckpt_file, map_location=lambda storage, loc: storage)
                 extra = ckpt['extra'] if 'extra' in ckpt else ckpt['extras']
                 self._best_accuracy = extra['accuracy'] if 'accuracy' in extra else ['perf_AP']
         else:
@@ -282,17 +287,17 @@
                 if accuracy > self._best_accuracy:
                     self._best_epoch = epoch
                     self._best_accuracy = accuracy
                     is_best_model = True
                 else:
                     is_best_model = False
                 save_ckpt_dict = {
-                    'state_dict': self.model.state_dict(), 'optimizer': self.optimizer.state_dict(), 'extra':
+                    'state_dict': self.model.state_dict(), 'extra':
                     {'epoch': epoch, 'step': self.global_step, 'accuracy': accuracy}
-                }
+                }  # 'optimizer': self.optimizer.state_dict(),
                 if cfg.FEAT.AMP:
                     save_ckpt_dict['amp'] = self._scaler.state_dict()
                 zl_info = {
                     'host_name': socket.gethostname(), 'epoch': epoch, 'accuracy': accuracy, 'best_epoch': self._best_epoch,
                     'best_accuracy': self._best_accuracy, 'others': self.on_saved_info()
                 }
                 mix.save_checkpoint(save_ckpt_dict, is_best_model, f'{cfg.LOG.PATH_ZID}/ckpt', zl_info)
```

### Comparing `aiei-1.0.2/aiei/core/base_config.py` & `aiei-1.0.6/aiei/core/base_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,15 +137,15 @@
 
 
 class TRAIN(Repr):
     BATCH_SIZE = Args.batch_size  # same to imgs_per_gpu
     EPOCHS = Args.epochs
     LR = Args.lr
     LR_SCHEDULER = None
-    RESUME = True
+    RESUME = 1  # 0: not resume, 1: strict resume, 2: loose resume
     EVAL_FREQ = 1  # per n epoch eval model. 0: no EVAL during TRAIN
 
 
 class EVAL(Repr):
     BATCH_SIZE = None  # EVAL_BATCH_SIZE
     USE_BEST_CKPT = False
```

### Comparing `aiei-1.0.2/aiei/ctrib/dsn.py` & `aiei-1.0.6/aiei/ctrib/dsn.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/ctrib/soft_argmax.py` & `aiei-1.0.6/aiei/ctrib/soft_argmax.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/data/mixup.py` & `aiei-1.0.6/aiei/data/mixup.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/data/sampler.py` & `aiei-1.0.6/aiei/data/sampler.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/data/set/coco.py` & `aiei-1.0.6/aiei/data/set/coco.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/data/transform/__init__.py` & `aiei-1.0.6/aiei/data/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/data/transform/base_cls.py` & `aiei-1.0.6/aiei/data/transform/base_cls.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/data/transform/base_fn.py` & `aiei-1.0.6/aiei/data/transform/base_fn.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/data/transform/center_pad.py` & `aiei-1.0.6/aiei/data/transform/center_pad.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/data/transform/random_affine.py` & `aiei-1.0.6/aiei/data/transform/random_affine.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/data/transform/random_brightness.py` & `aiei-1.0.6/aiei/data/transform/random_brightness.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/data/transform/random_contrast.py` & `aiei-1.0.6/aiei/data/transform/random_contrast.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/data/transform/random_crop.py` & `aiei-1.0.6/aiei/data/transform/random_crop.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/data/transform/random_erase.py` & `aiei-1.0.6/aiei/data/transform/random_erase.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/data/transform/random_flip.py` & `aiei-1.0.6/aiei/data/transform/random_flip.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/data/transform/random_lighting.py` & `aiei-1.0.6/aiei/data/transform/random_lighting.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/data/transform/random_saturation.py` & `aiei-1.0.6/aiei/data/transform/random_saturation.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/data/transform/resize_edge.py` & `aiei-1.0.6/aiei/data/transform/resize_edge.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/data/utils.py` & `aiei-1.0.6/aiei/data/utils.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/info.py` & `aiei-1.0.6/aiei/info.py`

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
-    version='1.0.2',
+    version='1.0.6',
     author='Lei Zhao',
     author_email='zlchn@qq.com',
     url='',
     project_urls={
         'github': 'https://github.com/',
     },
     description='A tiny framework for AI.',
```

### Comparing `aiei-1.0.2/aiei/misc/alg.py` & `aiei-1.0.6/aiei/misc/alg.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/misc/dist.py` & `aiei-1.0.6/aiei/misc/dist.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/misc/dotsi.py` & `aiei-1.0.6/aiei/misc/dotsi.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/misc/logger.py` & `aiei-1.0.6/aiei/misc/logger.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/misc/mix.py` & `aiei-1.0.6/aiei/misc/mix.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/misc/summary.py` & `aiei-1.0.6/aiei/misc/summary.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/misc/video.py` & `aiei-1.0.6/aiei/misc/video.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/misc/vis.py` & `aiei-1.0.6/aiei/misc/vis.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/model/backbones/darknet.py` & `aiei-1.0.6/aiei/model/backbones/darknet.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/model/backbones/densenet.py` & `aiei-1.0.6/aiei/model/backbones/densenet.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/model/backbones/dla.py` & `aiei-1.0.6/aiei/model/backbones/dla.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/model/backbones/efficientnet.py` & `aiei-1.0.6/aiei/model/backbones/efficientnet.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/model/backbones/hgnet.py` & `aiei-1.0.6/aiei/model/backbones/hgnet.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/model/backbones/highernet.py` & `aiei-1.0.6/aiei/model/backbones/highernet.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/model/backbones/resnet.py` & `aiei-1.0.6/aiei/model/backbones/resnet.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/model/backbones/shufflenetv2.py` & `aiei-1.0.6/aiei/model/backbones/shufflenetv2.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/model/backbones/tnet.py` & `aiei-1.0.6/aiei/model/backbones/tnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,32 +186,34 @@
         mul1 = torch.mul(inputs_lateral, igud1)
         return mul1 + inputs_lateral
 
 
 class UpLayer(nn.Module):
     def __init__(self, in_cs, out_cs):
         super(UpLayer, self).__init__()
-        list_smooth = []
-        list_gau = []
+        list_smooth, list_gau, list_lat_smooth = [], [], []
         self.last_smooth = smooth(in_cs[-1], out_cs[-1])
         for i in range(len(in_cs) - 1):
             # up_channel = in_cs[i + 1] if i == 0 else out_cs[i + 1]  # initial is from in_cs
+            # list_lat_smooth.append(smooth(out_cs[i + 1], out_cs[i + 1]))
             list_gau.append(GAU(out_cs[i + 1], out_cs[i + 1] // 4 + in_cs[i]))
             list_smooth.append(smooth(out_cs[i + 1] // 4 + in_cs[i], out_cs[i]))
         self.list_smooth = nn.ModuleList(list_smooth)
         self.list_gau = nn.ModuleList(list_gau)
+        # self.list_lat_smooth = nn.ModuleList(list_lat_smooth)
         self.shuffle = nn.PixelShuffle(2)
 
     def forward(self, list_input):
         assert len(list_input) == len(self.list_smooth) + 1
         outs = []
         x = self.last_smooth(list_input[-1])
         outs.append(x)
         for i in range(len(list_input) - 2, -1, -1):
             x_lateral = list_input[i]
+            # x = self.list_lat_smooth[i](x)
             x_up = self.shuffle(x)
             cat_cs = torch.cat([x_lateral, x_up], dim=1)
             cat_cs = self.list_gau[i](x, cat_cs)
             x = self.list_smooth[i](cat_cs)
             outs.append(x)
         return outs[::-1]
```

### Comparing `aiei-1.0.2/aiei/model/function.py` & `aiei-1.0.6/aiei/model/function.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/model/init.py` & `aiei-1.0.6/aiei/model/init.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/model/layers/cbam.py` & `aiei-1.0.6/aiei/model/layers/cbam.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/model/layers/coord_conv.py` & `aiei-1.0.6/aiei/model/layers/coord_conv.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/model/layers/gau_fpa.py` & `aiei-1.0.6/aiei/model/layers/gau_fpa.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/model/layers/norm.py` & `aiei-1.0.6/aiei/model/layers/norm.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/model/layers/self_attention.py` & `aiei-1.0.6/aiei/model/layers/self_attention.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/model/zlayers.py` & `aiei-1.0.6/aiei/model/zlayers.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/ops/FAIR/ROIAlign/ROIAlign.h` & `aiei-1.0.6/aiei/ops/FAIR/ROIAlign/ROIAlign.h`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/ops/FAIR/deform_conv.py` & `aiei-1.0.6/aiei/ops/FAIR/deform_conv.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/ops/FAIR/deform_conv_with_off.py` & `aiei-1.0.6/aiei/ops/FAIR/deform_conv_with_off.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/ops/FAIR/deformable/deform_conv.h` & `aiei-1.0.6/aiei/ops/FAIR/deformable/deform_conv.h`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/ops/FAIR/nms.py` & `aiei-1.0.6/aiei/ops/FAIR/nms.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/ops/FAIR/roi_align.py` & `aiei-1.0.6/aiei/ops/FAIR/roi_align.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/ops/FAIR/setup.py` & `aiei-1.0.6/aiei/ops/FAIR/setup.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/ops/dcnv2/__init__.py` & `aiei-1.0.6/aiei/ops/dcnv2/__init__.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/ops/dcnv2/functions/deform_conv.py` & `aiei-1.0.6/aiei/ops/dcnv2/functions/deform_conv.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/ops/dcnv2/functions/deform_pool.py` & `aiei-1.0.6/aiei/ops/dcnv2/functions/deform_pool.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/ops/dcnv2/modules/deform_conv.py` & `aiei-1.0.6/aiei/ops/dcnv2/modules/deform_conv.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/ops/dcnv2/modules/deform_pool.py` & `aiei-1.0.6/aiei/ops/dcnv2/modules/deform_pool.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/ops/nms/nms_wrapper.py` & `aiei-1.0.6/aiei/ops/nms/nms_wrapper.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/ops/nms/setup.py` & `aiei-1.0.6/aiei/ops/nms/setup.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/optim/lr_scheduler.py` & `aiei-1.0.6/aiei/optim/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/optim/radam.py` & `aiei-1.0.6/aiei/optim/radam.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/optim/swish.py` & `aiei-1.0.6/aiei/optim/swish.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei/spec/det/ious.py` & `aiei-1.0.6/aiei/spec/det/ious.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/aiei.egg-info/PKG-INFO` & `aiei-1.0.6/aiei.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiei
-Version: 1.0.2
+Version: 1.0.6
 Summary: A tiny framework for AI.
 Home-page: UNKNOWN
 Author: Lei Zhao
 Author-email: zlchn@qq.com
 License: Apache
 Project-URL: github, https://github.com/
 Description: ### Install AIEI
```

### Comparing `aiei-1.0.2/aiei.egg-info/SOURCES.txt` & `aiei-1.0.6/aiei.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/setup.py` & `aiei-1.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `aiei-1.0.2/tools/aiei` & `aiei-1.0.6/tools/aiei`

 * *Files identical despite different names*

