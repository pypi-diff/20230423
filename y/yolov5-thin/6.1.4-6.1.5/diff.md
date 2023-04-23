# Comparing `tmp/yolov5-thin-6.1.4.tar.gz` & `tmp/yolov5-thin-6.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yolov5-thin-6.1.4.tar", last modified: Fri Mar 31 07:52:09 2023, max compression
+gzip compressed data, was "dist/yolov5-thin-6.1.5.tar", last modified: Wed Apr 12 10:17:28 2023, max compression
```

## Comparing `yolov5-thin-6.1.4.tar` & `yolov5-thin-6.1.5.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxrwxr-x   0 shawn     (1000) shawn     (1000)        0 2023-03-31 07:52:09.479021 yolov5-thin-6.1.4/
--rw-rw-r--   0 shawn     (1000) shawn     (1000)    35126 2023-03-28 06:10:25.000000 yolov5-thin-6.1.4/LICENSE
--rw-rw-r--   0 shawn     (1000) shawn     (1000)      249 2023-03-28 06:10:25.000000 yolov5-thin-6.1.4/MANIFEST.in
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     9050 2023-03-31 07:52:09.479021 yolov5-thin-6.1.4/PKG-INFO
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     7848 2023-03-31 07:29:41.000000 yolov5-thin-6.1.4/README.md
--rw-rw-r--   0 shawn     (1000) shawn     (1000)       38 2023-03-31 07:52:09.479021 yolov5-thin-6.1.4/setup.cfg
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     2155 2023-03-31 07:29:41.000000 yolov5-thin-6.1.4/setup.py
-drwxrwxr-x   0 shawn     (1000) shawn     (1000)        0 2023-03-31 07:52:09.471021 yolov5-thin-6.1.4/yolov5/
--rw-rw-r--   0 shawn     (1000) shawn     (1000)      103 2023-03-31 07:47:58.000000 yolov5-thin-6.1.4/yolov5/__init__.py
-drwxrwxr-x   0 shawn     (1000) shawn     (1000)        0 2023-03-31 07:52:09.471021 yolov5-thin-6.1.4/yolov5/data/
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     2768 2023-03-31 07:29:41.000000 yolov5-thin-6.1.4/yolov5/data/Argoverse.yaml
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     1917 2023-03-31 07:29:41.000000 yolov5-thin-6.1.4/yolov5/data/GlobalWheat2020.yaml
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     8108 2023-03-31 07:29:41.000000 yolov5-thin-6.1.4/yolov5/data/Objects365.yaml
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     2372 2023-03-31 07:29:41.000000 yolov5-thin-6.1.4/yolov5/data/SKU-110K.yaml
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     3416 2023-03-31 07:29:41.000000 yolov5-thin-6.1.4/yolov5/data/VOC.yaml
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     2960 2023-03-31 07:29:41.000000 yolov5-thin-6.1.4/yolov5/data/VisDrone.yaml
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     2363 2023-03-31 07:29:41.000000 yolov5-thin-6.1.4/yolov5/data/coco.yaml
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     1723 2023-03-31 07:29:41.000000 yolov5-thin-6.1.4/yolov5/data/coco128.yaml
-drwxrwxr-x   0 shawn     (1000) shawn     (1000)        0 2023-03-31 07:52:09.475021 yolov5-thin-6.1.4/yolov5/data/hyps/
--rw-rw-r--   0 shawn     (1000) shawn     (1000)      673 2023-03-28 06:10:25.000000 yolov5-thin-6.1.4/yolov5/data/hyps/hyp.Objects365.yaml
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     1156 2023-03-28 06:10:25.000000 yolov5-thin-6.1.4/yolov5/data/hyps/hyp.VOC.yaml
--rw-rw-r--   0 shawn     (1000) shawn     (1000)      907 2023-03-31 07:29:41.000000 yolov5-thin-6.1.4/yolov5/data/hyps/hyp.finetune.yaml
--rw-rw-r--   0 shawn     (1000) shawn     (1000)      460 2023-03-31 07:29:41.000000 yolov5-thin-6.1.4/yolov5/data/hyps/hyp.finetune_objects365.yaml
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     1683 2023-03-28 06:10:25.000000 yolov5-thin-6.1.4/yolov5/data/hyps/hyp.scratch-high.yaml
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     1691 2023-03-28 06:10:25.000000 yolov5-thin-6.1.4/yolov5/data/hyps/hyp.scratch-low.yaml
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     1685 2023-03-28 06:10:25.000000 yolov5-thin-6.1.4/yolov5/data/hyps/hyp.scratch-med.yaml
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     1663 2023-03-31 07:29:41.000000 yolov5-thin-6.1.4/yolov5/data/hyps/hyp.scratch.yaml
-drwxrwxr-x   0 shawn     (1000) shawn     (1000)        0 2023-03-31 07:52:09.475021 yolov5-thin-6.1.4/yolov5/data/images/
--rw-rw-r--   0 shawn     (1000) shawn     (1000)   487438 2023-03-28 06:10:25.000000 yolov5-thin-6.1.4/yolov5/data/images/bus.jpg
--rw-rw-r--   0 shawn     (1000) shawn     (1000)   168949 2023-03-28 06:10:25.000000 yolov5-thin-6.1.4/yolov5/data/images/zidane.jpg
-drwxrwxr-x   0 shawn     (1000) shawn     (1000)        0 2023-03-31 07:52:09.475021 yolov5-thin-6.1.4/yolov5/data/scripts/
--rwxrwxr-x   0 shawn     (1000) shawn     (1000)      523 2023-03-31 07:29:41.000000 yolov5-thin-6.1.4/yolov5/data/scripts/download_weights.sh
--rwxrwxr-x   0 shawn     (1000) shawn     (1000)      900 2023-03-31 07:29:41.000000 yolov5-thin-6.1.4/yolov5/data/scripts/get_coco.sh
--rw-rw-r--   0 shawn     (1000) shawn     (1000)      615 2023-03-31 07:29:41.000000 yolov5-thin-6.1.4/yolov5/data/scripts/get_coco128.sh
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     5095 2023-03-31 07:29:41.000000 yolov5-thin-6.1.4/yolov5/data/xView.yaml
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     2476 2023-03-31 07:29:41.000000 yolov5-thin-6.1.4/yolov5/helpers.py
-drwxrwxr-x   0 shawn     (1000) shawn     (1000)        0 2023-03-31 07:52:09.475021 yolov5-thin-6.1.4/yolov5/models/
--rw-rw-r--   0 shawn     (1000) shawn     (1000)        0 2023-03-28 06:10:25.000000 yolov5-thin-6.1.4/yolov5/models/__init__.py
-drwxrwxr-x   0 shawn     (1000) shawn     (1000)        0 2023-03-31 07:52:09.475021 yolov5-thin-6.1.4/yolov5/models/__pycache__/
--rw-rw-r--   0 shawn     (1000) shawn     (1000)      149 2023-03-28 06:19:18.000000 yolov5-thin-6.1.4/yolov5/models/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 shawn     (1000) shawn     (1000)    25027 2023-03-31 04:24:25.000000 yolov5-thin-6.1.4/yolov5/models/__pycache__/common.cpython-38.pyc
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     5383 2023-03-28 07:37:35.000000 yolov5-thin-6.1.4/yolov5/models/__pycache__/experimental.cpython-38.pyc
--rw-rw-r--   0 shawn     (1000) shawn     (1000)    12855 2023-03-31 04:13:46.000000 yolov5-thin-6.1.4/yolov5/models/__pycache__/yolo.cpython-38.pyc
--rw-rw-r--   0 shawn     (1000) shawn     (1000)    25398 2023-03-31 07:47:58.000000 yolov5-thin-6.1.4/yolov5/models/common.py
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     4902 2023-03-31 07:29:41.000000 yolov5-thin-6.1.4/yolov5/models/experimental.py
-drwxrwxr-x   0 shawn     (1000) shawn     (1000)        0 2023-03-31 07:52:09.479021 yolov5-thin-6.1.4/yolov5/models/hub/
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     3335 2023-03-28 06:10:25.000000 yolov5-thin-6.1.4/yolov5/models/hub/anchors.yaml
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     1567 2023-03-28 06:10:25.000000 yolov5-thin-6.1.4/yolov5/models/hub/yolov3-spp.yaml
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     1232 2023-03-28 06:10:25.000000 yolov5-thin-6.1.4/yolov5/models/hub/yolov3-tiny.yaml
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     1558 2023-03-28 06:10:25.000000 yolov5-thin-6.1.4/yolov5/models/hub/yolov3.yaml
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     1423 2023-03-28 06:10:25.000000 yolov5-thin-6.1.4/yolov5/models/hub/yolov5-bifpn.yaml
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     1214 2023-03-28 06:10:25.000000 yolov5-thin-6.1.4/yolov5/models/hub/yolov5-fpn.yaml
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     1687 2023-03-28 06:10:25.000000 yolov5-thin-6.1.4/yolov5/models/hub/yolov5-p2.yaml
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     1349 2023-03-28 06:10:25.000000 yolov5-thin-6.1.4/yolov5/models/hub/yolov5-p34.yaml
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     1741 2023-03-28 06:10:25.000000 yolov5-thin-6.1.4/yolov5/models/hub/yolov5-p6.yaml
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     2122 2023-03-28 06:10:25.000000 yolov5-thin-6.1.4/yolov5/models/hub/yolov5-p7.yaml
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     1407 2023-03-28 06:10:25.000000 yolov5-thin-6.1.4/yolov5/models/hub/yolov5-panet.yaml
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     1820 2023-03-28 06:10:25.000000 yolov5-thin-6.1.4/yolov5/models/hub/yolov5l6.yaml
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     1822 2023-03-28 06:10:25.000000 yolov5-thin-6.1.4/yolov5/models/hub/yolov5m6.yaml
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     1822 2023-03-28 06:10:25.000000 yolov5-thin-6.1.4/yolov5/models/hub/yolov5n6.yaml
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     1483 2023-03-28 06:10:25.000000 yolov5-thin-6.1.4/yolov5/models/hub/yolov5s-ghost.yaml
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     1441 2023-03-28 06:10:25.000000 yolov5-thin-6.1.4/yolov5/models/hub/yolov5s-transformer.yaml
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     1822 2023-03-28 06:10:25.000000 yolov5-thin-6.1.4/yolov5/models/hub/yolov5s6.yaml
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     1822 2023-03-28 06:10:25.000000 yolov5-thin-6.1.4/yolov5/models/hub/yolov5x6.yaml
--rw-rw-r--   0 shawn     (1000) shawn     (1000)    15127 2023-03-31 07:47:58.000000 yolov5-thin-6.1.4/yolov5/models/yolo.py
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     1401 2023-03-28 06:10:25.000000 yolov5-thin-6.1.4/yolov5/models/yolov5l.yaml
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     1403 2023-03-28 06:10:25.000000 yolov5-thin-6.1.4/yolov5/models/yolov5m.yaml
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     1403 2023-03-28 06:10:25.000000 yolov5-thin-6.1.4/yolov5/models/yolov5n.yaml
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     1403 2023-03-28 06:10:25.000000 yolov5-thin-6.1.4/yolov5/models/yolov5s.yaml
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     1403 2023-03-28 06:10:25.000000 yolov5-thin-6.1.4/yolov5/models/yolov5x.yaml
-drwxrwxr-x   0 shawn     (1000) shawn     (1000)        0 2023-03-31 07:52:09.479021 yolov5-thin-6.1.4/yolov5/utils/
--rw-rw-r--   0 shawn     (1000) shawn     (1000)       45 2023-03-31 07:47:58.000000 yolov5-thin-6.1.4/yolov5/utils/__init__.py
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     3449 2023-03-28 06:10:25.000000 yolov5-thin-6.1.4/yolov5/utils/activations.py
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     6094 2023-03-31 07:47:58.000000 yolov5-thin-6.1.4/yolov5/utils/augmentations.py
--rw-rw-r--   0 shawn     (1000) shawn     (1000)      599 2023-03-31 07:47:58.000000 yolov5-thin-6.1.4/yolov5/utils/autoanchor.py
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     2215 2023-03-31 07:29:41.000000 yolov5-thin-6.1.4/yolov5/utils/autobatch.py
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     2402 2023-03-31 07:29:41.000000 yolov5-thin-6.1.4/yolov5/utils/callbacks.py
--rwxrwxr-x   0 shawn     (1000) shawn     (1000)     5492 2023-03-31 07:47:58.000000 yolov5-thin-6.1.4/yolov5/utils/datasets.py
--rwxrwxr-x   0 shawn     (1000) shawn     (1000)    38053 2023-03-31 07:47:58.000000 yolov5-thin-6.1.4/yolov5/utils/general.py
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     8275 2023-03-31 07:47:58.000000 yolov5-thin-6.1.4/yolov5/utils/metrics.py
--rw-rw-r--   0 shawn     (1000) shawn     (1000)    10134 2023-03-31 07:47:58.000000 yolov5-thin-6.1.4/yolov5/utils/plots.py
--rw-rw-r--   0 shawn     (1000) shawn     (1000)    13310 2023-03-31 07:29:41.000000 yolov5-thin-6.1.4/yolov5/utils/torch_utils.py
-drwxrwxr-x   0 shawn     (1000) shawn     (1000)        0 2023-03-31 07:52:09.479021 yolov5-thin-6.1.4/yolov5_thin.egg-info/
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     9050 2023-03-31 07:52:09.000000 yolov5-thin-6.1.4/yolov5_thin.egg-info/PKG-INFO
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     2270 2023-03-31 07:52:09.000000 yolov5-thin-6.1.4/yolov5_thin.egg-info/SOURCES.txt
--rw-rw-r--   0 shawn     (1000) shawn     (1000)        1 2023-03-31 07:52:09.000000 yolov5-thin-6.1.4/yolov5_thin.egg-info/dependency_links.txt
--rw-rw-r--   0 shawn     (1000) shawn     (1000)      111 2023-03-31 07:52:09.000000 yolov5-thin-6.1.4/yolov5_thin.egg-info/requires.txt
--rw-rw-r--   0 shawn     (1000) shawn     (1000)        7 2023-03-31 07:52:09.000000 yolov5-thin-6.1.4/yolov5_thin.egg-info/top_level.txt
+drwxrwxr-x   0 shawn     (1000) shawn     (1000)        0 2023-04-12 10:17:28.989558 yolov5-thin-6.1.5/
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)    35126 2023-03-28 06:10:25.000000 yolov5-thin-6.1.5/LICENSE
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)      249 2023-03-28 06:10:25.000000 yolov5-thin-6.1.5/MANIFEST.in
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     9050 2023-04-12 10:17:28.989558 yolov5-thin-6.1.5/PKG-INFO
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     7848 2023-03-31 07:29:41.000000 yolov5-thin-6.1.5/README.md
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)       38 2023-04-12 10:17:28.989558 yolov5-thin-6.1.5/setup.cfg
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     2155 2023-03-31 07:29:41.000000 yolov5-thin-6.1.5/setup.py
+drwxrwxr-x   0 shawn     (1000) shawn     (1000)        0 2023-04-12 10:17:28.981558 yolov5-thin-6.1.5/yolov5/
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)      103 2023-04-12 10:13:58.000000 yolov5-thin-6.1.5/yolov5/__init__.py
+drwxrwxr-x   0 shawn     (1000) shawn     (1000)        0 2023-04-12 10:17:28.981558 yolov5-thin-6.1.5/yolov5/data/
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     2768 2023-03-31 07:29:41.000000 yolov5-thin-6.1.5/yolov5/data/Argoverse.yaml
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     1917 2023-03-31 07:29:41.000000 yolov5-thin-6.1.5/yolov5/data/GlobalWheat2020.yaml
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     8108 2023-03-31 07:29:41.000000 yolov5-thin-6.1.5/yolov5/data/Objects365.yaml
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     2372 2023-03-31 07:29:41.000000 yolov5-thin-6.1.5/yolov5/data/SKU-110K.yaml
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     3416 2023-03-31 07:29:41.000000 yolov5-thin-6.1.5/yolov5/data/VOC.yaml
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     2960 2023-03-31 07:29:41.000000 yolov5-thin-6.1.5/yolov5/data/VisDrone.yaml
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     2363 2023-03-31 07:29:41.000000 yolov5-thin-6.1.5/yolov5/data/coco.yaml
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     1723 2023-03-31 07:29:41.000000 yolov5-thin-6.1.5/yolov5/data/coco128.yaml
+drwxrwxr-x   0 shawn     (1000) shawn     (1000)        0 2023-04-12 10:17:28.981558 yolov5-thin-6.1.5/yolov5/data/hyps/
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)      673 2023-03-28 06:10:25.000000 yolov5-thin-6.1.5/yolov5/data/hyps/hyp.Objects365.yaml
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     1156 2023-03-28 06:10:25.000000 yolov5-thin-6.1.5/yolov5/data/hyps/hyp.VOC.yaml
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)      907 2023-03-31 07:29:41.000000 yolov5-thin-6.1.5/yolov5/data/hyps/hyp.finetune.yaml
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)      460 2023-03-31 07:29:41.000000 yolov5-thin-6.1.5/yolov5/data/hyps/hyp.finetune_objects365.yaml
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     1683 2023-03-28 06:10:25.000000 yolov5-thin-6.1.5/yolov5/data/hyps/hyp.scratch-high.yaml
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     1691 2023-03-28 06:10:25.000000 yolov5-thin-6.1.5/yolov5/data/hyps/hyp.scratch-low.yaml
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     1685 2023-03-28 06:10:25.000000 yolov5-thin-6.1.5/yolov5/data/hyps/hyp.scratch-med.yaml
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     1663 2023-03-31 07:29:41.000000 yolov5-thin-6.1.5/yolov5/data/hyps/hyp.scratch.yaml
+drwxrwxr-x   0 shawn     (1000) shawn     (1000)        0 2023-04-12 10:17:28.981558 yolov5-thin-6.1.5/yolov5/data/images/
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)   487438 2023-03-28 06:10:25.000000 yolov5-thin-6.1.5/yolov5/data/images/bus.jpg
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)   168949 2023-03-28 06:10:25.000000 yolov5-thin-6.1.5/yolov5/data/images/zidane.jpg
+drwxrwxr-x   0 shawn     (1000) shawn     (1000)        0 2023-04-12 10:17:28.981558 yolov5-thin-6.1.5/yolov5/data/scripts/
+-rwxrwxr-x   0 shawn     (1000) shawn     (1000)      523 2023-03-31 07:29:41.000000 yolov5-thin-6.1.5/yolov5/data/scripts/download_weights.sh
+-rwxrwxr-x   0 shawn     (1000) shawn     (1000)      900 2023-03-31 07:29:41.000000 yolov5-thin-6.1.5/yolov5/data/scripts/get_coco.sh
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)      615 2023-03-31 07:29:41.000000 yolov5-thin-6.1.5/yolov5/data/scripts/get_coco128.sh
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     5095 2023-03-31 07:29:41.000000 yolov5-thin-6.1.5/yolov5/data/xView.yaml
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     2476 2023-03-31 07:29:41.000000 yolov5-thin-6.1.5/yolov5/helpers.py
+drwxrwxr-x   0 shawn     (1000) shawn     (1000)        0 2023-04-12 10:17:28.985558 yolov5-thin-6.1.5/yolov5/models/
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)        0 2023-03-28 06:10:25.000000 yolov5-thin-6.1.5/yolov5/models/__init__.py
+drwxrwxr-x   0 shawn     (1000) shawn     (1000)        0 2023-04-12 10:17:28.985558 yolov5-thin-6.1.5/yolov5/models/__pycache__/
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)      149 2023-03-28 06:19:18.000000 yolov5-thin-6.1.5/yolov5/models/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)    25027 2023-03-31 04:24:25.000000 yolov5-thin-6.1.5/yolov5/models/__pycache__/common.cpython-38.pyc
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     5383 2023-03-28 07:37:35.000000 yolov5-thin-6.1.5/yolov5/models/__pycache__/experimental.cpython-38.pyc
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)    12855 2023-03-31 04:13:46.000000 yolov5-thin-6.1.5/yolov5/models/__pycache__/yolo.cpython-38.pyc
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)    25398 2023-03-31 07:47:58.000000 yolov5-thin-6.1.5/yolov5/models/common.py
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     4902 2023-03-31 07:29:41.000000 yolov5-thin-6.1.5/yolov5/models/experimental.py
+drwxrwxr-x   0 shawn     (1000) shawn     (1000)        0 2023-04-12 10:17:28.985558 yolov5-thin-6.1.5/yolov5/models/hub/
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     3335 2023-03-28 06:10:25.000000 yolov5-thin-6.1.5/yolov5/models/hub/anchors.yaml
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     1567 2023-03-28 06:10:25.000000 yolov5-thin-6.1.5/yolov5/models/hub/yolov3-spp.yaml
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     1232 2023-03-28 06:10:25.000000 yolov5-thin-6.1.5/yolov5/models/hub/yolov3-tiny.yaml
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     1558 2023-03-28 06:10:25.000000 yolov5-thin-6.1.5/yolov5/models/hub/yolov3.yaml
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     1423 2023-03-28 06:10:25.000000 yolov5-thin-6.1.5/yolov5/models/hub/yolov5-bifpn.yaml
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     1214 2023-03-28 06:10:25.000000 yolov5-thin-6.1.5/yolov5/models/hub/yolov5-fpn.yaml
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     1687 2023-03-28 06:10:25.000000 yolov5-thin-6.1.5/yolov5/models/hub/yolov5-p2.yaml
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     1349 2023-03-28 06:10:25.000000 yolov5-thin-6.1.5/yolov5/models/hub/yolov5-p34.yaml
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     1741 2023-03-28 06:10:25.000000 yolov5-thin-6.1.5/yolov5/models/hub/yolov5-p6.yaml
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     2122 2023-03-28 06:10:25.000000 yolov5-thin-6.1.5/yolov5/models/hub/yolov5-p7.yaml
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     1407 2023-03-28 06:10:25.000000 yolov5-thin-6.1.5/yolov5/models/hub/yolov5-panet.yaml
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     1820 2023-03-28 06:10:25.000000 yolov5-thin-6.1.5/yolov5/models/hub/yolov5l6.yaml
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     1822 2023-03-28 06:10:25.000000 yolov5-thin-6.1.5/yolov5/models/hub/yolov5m6.yaml
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     1822 2023-03-28 06:10:25.000000 yolov5-thin-6.1.5/yolov5/models/hub/yolov5n6.yaml
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     1483 2023-03-28 06:10:25.000000 yolov5-thin-6.1.5/yolov5/models/hub/yolov5s-ghost.yaml
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     1441 2023-03-28 06:10:25.000000 yolov5-thin-6.1.5/yolov5/models/hub/yolov5s-transformer.yaml
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     1822 2023-03-28 06:10:25.000000 yolov5-thin-6.1.5/yolov5/models/hub/yolov5s6.yaml
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     1822 2023-03-28 06:10:25.000000 yolov5-thin-6.1.5/yolov5/models/hub/yolov5x6.yaml
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)    14814 2023-04-12 10:16:09.000000 yolov5-thin-6.1.5/yolov5/models/yolo.py
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     1401 2023-03-28 06:10:25.000000 yolov5-thin-6.1.5/yolov5/models/yolov5l.yaml
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     1403 2023-03-28 06:10:25.000000 yolov5-thin-6.1.5/yolov5/models/yolov5m.yaml
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     1403 2023-03-28 06:10:25.000000 yolov5-thin-6.1.5/yolov5/models/yolov5n.yaml
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     1403 2023-03-28 06:10:25.000000 yolov5-thin-6.1.5/yolov5/models/yolov5s.yaml
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     1403 2023-03-28 06:10:25.000000 yolov5-thin-6.1.5/yolov5/models/yolov5x.yaml
+drwxrwxr-x   0 shawn     (1000) shawn     (1000)        0 2023-04-12 10:17:28.985558 yolov5-thin-6.1.5/yolov5/utils/
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)       45 2023-03-31 07:47:58.000000 yolov5-thin-6.1.5/yolov5/utils/__init__.py
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     3449 2023-03-28 06:10:25.000000 yolov5-thin-6.1.5/yolov5/utils/activations.py
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     6094 2023-03-31 07:47:58.000000 yolov5-thin-6.1.5/yolov5/utils/augmentations.py
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)      599 2023-03-31 07:47:58.000000 yolov5-thin-6.1.5/yolov5/utils/autoanchor.py
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     2215 2023-03-31 07:29:41.000000 yolov5-thin-6.1.5/yolov5/utils/autobatch.py
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     2402 2023-03-31 07:29:41.000000 yolov5-thin-6.1.5/yolov5/utils/callbacks.py
+-rwxrwxr-x   0 shawn     (1000) shawn     (1000)     5492 2023-03-31 07:47:58.000000 yolov5-thin-6.1.5/yolov5/utils/datasets.py
+-rwxrwxr-x   0 shawn     (1000) shawn     (1000)    38053 2023-03-31 07:47:58.000000 yolov5-thin-6.1.5/yolov5/utils/general.py
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     8275 2023-03-31 07:47:58.000000 yolov5-thin-6.1.5/yolov5/utils/metrics.py
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)    10134 2023-03-31 07:47:58.000000 yolov5-thin-6.1.5/yolov5/utils/plots.py
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)    13310 2023-03-31 07:29:41.000000 yolov5-thin-6.1.5/yolov5/utils/torch_utils.py
+drwxrwxr-x   0 shawn     (1000) shawn     (1000)        0 2023-04-12 10:17:28.989558 yolov5-thin-6.1.5/yolov5_thin.egg-info/
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     9050 2023-04-12 10:17:28.000000 yolov5-thin-6.1.5/yolov5_thin.egg-info/PKG-INFO
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     2270 2023-04-12 10:17:28.000000 yolov5-thin-6.1.5/yolov5_thin.egg-info/SOURCES.txt
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)        1 2023-04-12 10:17:28.000000 yolov5-thin-6.1.5/yolov5_thin.egg-info/dependency_links.txt
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)      112 2023-04-12 10:17:28.000000 yolov5-thin-6.1.5/yolov5_thin.egg-info/requires.txt
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)        7 2023-04-12 10:17:28.000000 yolov5-thin-6.1.5/yolov5_thin.egg-info/top_level.txt
```

### Comparing `yolov5-thin-6.1.4/LICENSE` & `yolov5-thin-6.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/PKG-INFO` & `yolov5-thin-6.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yolov5-thin
-Version: 6.1.4
+Version: 6.1.5
 Summary: Packaged version of the Yolov5 object detector
 Home-page: https://github.com/SethWen/yolov5-pip.git
 Author: 
 License: GPL
 Keywords: machine-learning,deep-learning,ml,pytorch,YOLO,object-detection,vision,YOLOv3,YOLOv4,YOLOv5
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: yolov5-thin Version: 6.1.4 Summary: Packaged
+Metadata-Version: 2.1 Name: yolov5-thin Version: 6.1.5 Summary: Packaged
 version of the Yolov5 object detector Home-page: https://github.com/SethWen/
 yolov5-pip.git Author: License: GPL Keywords: machine-learning,deep-
 learning,ml,pytorch,YOLO,object-detection,vision,YOLOv3,YOLOv4,YOLOv5
 Classifier: Development Status :: 5 - Production/Stable Classifier: License ::
 OSI Approved :: GNU General Public License (GPL) Classifier: Operating System
 :: OS Independent Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Science/Research Classifier: Programming Language ::
```

### Comparing `yolov5-thin-6.1.4/README.md` & `yolov5-thin-6.1.5/README.md`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/setup.py` & `yolov5-thin-6.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/data/Argoverse.yaml` & `yolov5-thin-6.1.5/yolov5/data/Argoverse.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/data/GlobalWheat2020.yaml` & `yolov5-thin-6.1.5/yolov5/data/GlobalWheat2020.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/data/Objects365.yaml` & `yolov5-thin-6.1.5/yolov5/data/Objects365.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/data/SKU-110K.yaml` & `yolov5-thin-6.1.5/yolov5/data/SKU-110K.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/data/VOC.yaml` & `yolov5-thin-6.1.5/yolov5/data/VOC.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/data/VisDrone.yaml` & `yolov5-thin-6.1.5/yolov5/data/VisDrone.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/data/coco.yaml` & `yolov5-thin-6.1.5/yolov5/data/coco.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/data/coco128.yaml` & `yolov5-thin-6.1.5/yolov5/data/coco128.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/data/hyps/hyp.Objects365.yaml` & `yolov5-thin-6.1.5/yolov5/data/hyps/hyp.Objects365.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/data/hyps/hyp.VOC.yaml` & `yolov5-thin-6.1.5/yolov5/data/hyps/hyp.VOC.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/data/hyps/hyp.finetune.yaml` & `yolov5-thin-6.1.5/yolov5/data/hyps/hyp.finetune.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/data/hyps/hyp.scratch-high.yaml` & `yolov5-thin-6.1.5/yolov5/data/hyps/hyp.scratch-high.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/data/hyps/hyp.scratch-low.yaml` & `yolov5-thin-6.1.5/yolov5/data/hyps/hyp.scratch-low.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/data/hyps/hyp.scratch-med.yaml` & `yolov5-thin-6.1.5/yolov5/data/hyps/hyp.scratch-med.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/data/hyps/hyp.scratch.yaml` & `yolov5-thin-6.1.5/yolov5/data/hyps/hyp.scratch.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/data/images/bus.jpg` & `yolov5-thin-6.1.5/yolov5/data/images/bus.jpg`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/data/images/zidane.jpg` & `yolov5-thin-6.1.5/yolov5/data/images/zidane.jpg`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/data/scripts/download_weights.sh` & `yolov5-thin-6.1.5/yolov5/data/scripts/download_weights.sh`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/data/scripts/get_coco.sh` & `yolov5-thin-6.1.5/yolov5/data/scripts/get_coco.sh`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/data/scripts/get_coco128.sh` & `yolov5-thin-6.1.5/yolov5/data/scripts/get_coco128.sh`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/data/xView.yaml` & `yolov5-thin-6.1.5/yolov5/data/xView.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/helpers.py` & `yolov5-thin-6.1.5/yolov5/helpers.py`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/models/__pycache__/common.cpython-38.pyc` & `yolov5-thin-6.1.5/yolov5/models/__pycache__/common.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/models/__pycache__/experimental.cpython-38.pyc` & `yolov5-thin-6.1.5/yolov5/models/__pycache__/experimental.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/models/__pycache__/yolo.cpython-38.pyc` & `yolov5-thin-6.1.5/yolov5/models/__pycache__/yolo.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/models/common.py` & `yolov5-thin-6.1.5/yolov5/models/common.py`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/models/experimental.py` & `yolov5-thin-6.1.5/yolov5/models/experimental.py`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/models/hub/anchors.yaml` & `yolov5-thin-6.1.5/yolov5/models/hub/anchors.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/models/hub/yolov3-spp.yaml` & `yolov5-thin-6.1.5/yolov5/models/hub/yolov3-spp.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/models/hub/yolov3-tiny.yaml` & `yolov5-thin-6.1.5/yolov5/models/hub/yolov3-tiny.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/models/hub/yolov3.yaml` & `yolov5-thin-6.1.5/yolov5/models/hub/yolov3.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/models/hub/yolov5-bifpn.yaml` & `yolov5-thin-6.1.5/yolov5/models/hub/yolov5-bifpn.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/models/hub/yolov5-fpn.yaml` & `yolov5-thin-6.1.5/yolov5/models/hub/yolov5-fpn.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/models/hub/yolov5-p2.yaml` & `yolov5-thin-6.1.5/yolov5/models/hub/yolov5-p2.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/models/hub/yolov5-p34.yaml` & `yolov5-thin-6.1.5/yolov5/models/hub/yolov5-p34.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/models/hub/yolov5-p6.yaml` & `yolov5-thin-6.1.5/yolov5/models/hub/yolov5-p6.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/models/hub/yolov5-p7.yaml` & `yolov5-thin-6.1.5/yolov5/models/hub/yolov5-p7.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/models/hub/yolov5-panet.yaml` & `yolov5-thin-6.1.5/yolov5/models/hub/yolov5-panet.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/models/hub/yolov5l6.yaml` & `yolov5-thin-6.1.5/yolov5/models/hub/yolov5l6.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/models/hub/yolov5m6.yaml` & `yolov5-thin-6.1.5/yolov5/models/hub/yolov5m6.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/models/hub/yolov5n6.yaml` & `yolov5-thin-6.1.5/yolov5/models/hub/yolov5n6.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/models/hub/yolov5s-ghost.yaml` & `yolov5-thin-6.1.5/yolov5/models/hub/yolov5s-ghost.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/models/hub/yolov5s-transformer.yaml` & `yolov5-thin-6.1.5/yolov5/models/hub/yolov5s-transformer.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/models/hub/yolov5s6.yaml` & `yolov5-thin-6.1.5/yolov5/models/hub/yolov5s6.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/models/hub/yolov5x6.yaml` & `yolov5-thin-6.1.5/yolov5/models/hub/yolov5x6.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/models/yolo.py` & `yolov5-thin-6.1.5/yolov5/models/yolo.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,39 +54,34 @@
         z = []  # inference output
         for i in range(self.nl):
             x[i] = self.m[i](x[i])  # conv
             bs, _, ny, nx = x[i].shape  # x(bs,255,20,20) to x(bs,3,20,20,85)
             x[i] = x[i].view(bs, self.na, self.no, ny, nx).permute(0, 1, 3, 4, 2).contiguous()
 
             if not self.training:  # inference
-                if self.onnx_dynamic or self.grid[i].shape[2:4] != x[i].shape[2:4]:
-                    self.grid[i], self.anchor_grid[i] = self._make_grid(nx, ny, i)
-
+                grid, anchor_grid = self._make_grid(nx, ny, i)
                 y = x[i].sigmoid()
                 if self.inplace:
-                    y[..., 0:2] = (y[..., 0:2] * 2 + self.grid[i]) * self.stride[i]  # xy
-                    y[..., 2:4] = (y[..., 2:4] * 2) ** 2 * self.anchor_grid[i]  # wh
+                    y[..., 0:2] = (y[..., 0:2] * 2 + grid) * self.stride[i]  # xy
+                    y[..., 2:4] = (y[..., 2:4] * 2) ** 2 * anchor_grid  # wh
                 else:  # for YOLOv5 on AWS Inferentia https://github.com/ultralytics/yolov5/pull/2953
                     xy, wh, conf = y.split((2, 2, self.nc + 1), 4)  # y.tensor_split((2, 4, 5), 4)  # torch 1.8.0
-                    xy = (xy * 2 + self.grid[i]) * self.stride[i]  # xy
-                    wh = (wh * 2) ** 2 * self.anchor_grid[i]  # wh
+                    xy = (xy * 2 + grid) * self.stride[i]  # xy
+                    wh = (wh * 2) ** 2 * anchor_grid       # wh
                     y = torch.cat((xy, wh, conf), 4)
                 z.append(y.view(bs, -1, self.no))
 
         return x if self.training else (torch.cat(z, 1),) if self.export else (torch.cat(z, 1), x)
 
     def _make_grid(self, nx=20, ny=20, i=0):
         d = self.anchors[i].device
         t = self.anchors[i].dtype
         shape = 1, self.na, ny, nx, 2  # grid shape
         y, x = torch.arange(ny, device=d, dtype=t), torch.arange(nx, device=d, dtype=t)
-        if check_version(torch.__version__, '1.10.0'):  # torch>=1.10.0 meshgrid workaround for torch>=0.7 compatibility
-            yv, xv = torch.meshgrid(y, x, indexing='ij')
-        else:
-            yv, xv = torch.meshgrid(y, x)
+        yv, xv = torch.meshgrid(y, x, indexing='ij')
         grid = torch.stack((xv, yv), 2).expand(shape) - 0.5  # add grid offset, i.e. y = 2.0 * x - 0.5
         anchor_grid = (self.anchors[i] * self.stride[i]).view((1, self.na, 1, 1, 2)).expand(shape)
         return grid, anchor_grid
 
 
 class Model(nn.Module):
     # YOLOv5 model
```

### Comparing `yolov5-thin-6.1.4/yolov5/models/yolov5l.yaml` & `yolov5-thin-6.1.5/yolov5/models/yolov5l.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/models/yolov5m.yaml` & `yolov5-thin-6.1.5/yolov5/models/yolov5m.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/models/yolov5n.yaml` & `yolov5-thin-6.1.5/yolov5/models/yolov5n.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/models/yolov5s.yaml` & `yolov5-thin-6.1.5/yolov5/models/yolov5s.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/models/yolov5x.yaml` & `yolov5-thin-6.1.5/yolov5/models/yolov5x.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/utils/activations.py` & `yolov5-thin-6.1.5/yolov5/utils/activations.py`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/utils/augmentations.py` & `yolov5-thin-6.1.5/yolov5/utils/augmentations.py`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/utils/autoanchor.py` & `yolov5-thin-6.1.5/yolov5/utils/autoanchor.py`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/utils/autobatch.py` & `yolov5-thin-6.1.5/yolov5/utils/autobatch.py`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/utils/callbacks.py` & `yolov5-thin-6.1.5/yolov5/utils/callbacks.py`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/utils/datasets.py` & `yolov5-thin-6.1.5/yolov5/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/utils/general.py` & `yolov5-thin-6.1.5/yolov5/utils/general.py`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/utils/metrics.py` & `yolov5-thin-6.1.5/yolov5/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/utils/plots.py` & `yolov5-thin-6.1.5/yolov5/utils/plots.py`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5/utils/torch_utils.py` & `yolov5-thin-6.1.5/yolov5/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `yolov5-thin-6.1.4/yolov5_thin.egg-info/PKG-INFO` & `yolov5-thin-6.1.5/yolov5_thin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yolov5-thin
-Version: 6.1.4
+Version: 6.1.5
 Summary: Packaged version of the Yolov5 object detector
 Home-page: https://github.com/SethWen/yolov5-pip.git
 Author: 
 License: GPL
 Keywords: machine-learning,deep-learning,ml,pytorch,YOLO,object-detection,vision,YOLOv3,YOLOv4,YOLOv5
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: yolov5-thin Version: 6.1.4 Summary: Packaged
+Metadata-Version: 2.1 Name: yolov5-thin Version: 6.1.5 Summary: Packaged
 version of the Yolov5 object detector Home-page: https://github.com/SethWen/
 yolov5-pip.git Author: License: GPL Keywords: machine-learning,deep-
 learning,ml,pytorch,YOLO,object-detection,vision,YOLOv3,YOLOv4,YOLOv5
 Classifier: Development Status :: 5 - Production/Stable Classifier: License ::
 OSI Approved :: GNU General Public License (GPL) Classifier: Operating System
 :: OS Independent Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Science/Research Classifier: Programming Language ::
```

### Comparing `yolov5-thin-6.1.4/yolov5_thin.egg-info/SOURCES.txt` & `yolov5-thin-6.1.5/yolov5_thin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

