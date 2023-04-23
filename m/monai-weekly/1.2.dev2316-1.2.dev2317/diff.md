# Comparing `tmp/monai-weekly-1.2.dev2316.tar.gz` & `tmp/monai-weekly-1.2.dev2317.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monai-weekly-1.2.dev2316.tar", last modified: Sun Apr 16 02:21:48 2023, max compression
+gzip compressed data, was "monai-weekly-1.2.dev2317.tar", last modified: Sun Apr 23 02:24:34 2023, max compression
```

## Comparing `monai-weekly-1.2.dev2316.tar` & `monai-weekly-1.2.dev2317.tar`

### file list

```diff
@@ -1,1133 +1,1133 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.476853 monai-weekly-1.2.dev2316/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-04-16 02:21:48.476853 monai-weekly-1.2.dev2316/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.476853 monai-weekly-1.2.dev2316/monai/
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-04-16 02:19:48.000000 monai-weekly-1.2.dev2316/monai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.044857 monai-weekly-1.2.dev2316/monai/_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/_extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.044857 monai-weekly-1.2.dev2316/monai/_extensions/gmm/
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/_extensions/gmm/gmm.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/_extensions/gmm/gmm.h
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/_extensions/gmm/gmm_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16213 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/_extensions/gmm/gmm_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/_extensions/gmm/gmm_cuda_linalg.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/_extensions/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-16 02:21:48.476853 monai-weekly-1.2.dev2316/monai/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.044857 monai-weekly-1.2.dev2316/monai/apps/
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.048857 monai-weekly-1.2.dev2316/monai/apps/auto3dseg/
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/auto3dseg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/auto3dseg/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36754 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/auto3dseg/auto_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    25498 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/auto3dseg/bundle_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)    17319 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/auto3dseg/data_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)    22475 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/auto3dseg/ensemble_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    17523 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/auto3dseg/hpo_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/auto3dseg/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/auto3dseg/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    34560 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.048857 monai-weekly-1.2.dev2316/monai/apps/deepedit/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/deepedit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/deepedit/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    37435 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/deepedit/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.052857 monai-weekly-1.2.dev2316/monai/apps/deepgrow/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/deepgrow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10054 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/deepgrow/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/deepgrow/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    42011 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/deepgrow/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.052857 monai-weekly-1.2.dev2316/monai/apps/detection/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/detection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.052857 monai-weekly-1.2.dev2316/monai/apps/detection/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/detection/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26617 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/detection/metrics/coco.py
--rw-r--r--   0 runner    (1001) docker     (123)    17161 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/detection/metrics/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.056857 monai-weekly-1.2.dev2316/monai/apps/detection/networks/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/detection/networks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51663 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/detection/networks/retinanet_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)    17604 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/detection/networks/retinanet_network.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.056857 monai-weekly-1.2.dev2316/monai/apps/detection/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/detection/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24519 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/detection/transforms/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    17970 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/detection/transforms/box_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    68979 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/detection/transforms/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.060857 monai-weekly-1.2.dev2316/monai/apps/detection/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    13531 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/detection/utils/ATSS_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/detection/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18681 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/detection/utils/anchor_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11120 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/detection/utils/box_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/detection/utils/box_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)    10306 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/detection/utils/detector_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13890 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/detection/utils/hard_negative_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/detection/utils/predict_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.060857 monai-weekly-1.2.dev2316/monai/apps/mmars/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/mmars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13115 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/mmars/mmars.py
--rw-r--r--   0 runner    (1001) docker     (123)     9996 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/mmars/model_desc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.064857 monai-weekly-1.2.dev2316/monai/apps/nnunet/
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/nnunet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/nnunet/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38587 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/nnunet/nnunetv2_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/nnunet/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.064857 monai-weekly-1.2.dev2316/monai/apps/nuclick/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/nuclick/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24948 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/nuclick/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.064857 monai-weekly-1.2.dev2316/monai/apps/pathology/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/pathology/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.064857 monai-weekly-1.2.dev2316/monai/apps/pathology/engines/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/pathology/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/pathology/engines/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.064857 monai-weekly-1.2.dev2316/monai/apps/pathology/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/pathology/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/pathology/handlers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.064857 monai-weekly-1.2.dev2316/monai/apps/pathology/inferers/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/pathology/inferers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9148 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/pathology/inferers/inferer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.068857 monai-weekly-1.2.dev2316/monai/apps/pathology/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/pathology/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7293 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/pathology/losses/hovernet_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.068857 monai-weekly-1.2.dev2316/monai/apps/pathology/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/pathology/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/pathology/metrics/lesion_froc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.068857 monai-weekly-1.2.dev2316/monai/apps/pathology/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/pathology/transforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.068857 monai-weekly-1.2.dev2316/monai/apps/pathology/transforms/post/
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/pathology/transforms/post/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37322 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/pathology/transforms/post/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    25992 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/pathology/transforms/post/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.068857 monai-weekly-1.2.dev2316/monai/apps/pathology/transforms/stain/
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/pathology/transforms/stain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/pathology/transforms/stain/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/pathology/transforms/stain/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/pathology/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.072857 monai-weekly-1.2.dev2316/monai/apps/reconstruction/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/reconstruction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/reconstruction/complex_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/reconstruction/fastmri_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/reconstruction/mri_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.072857 monai-weekly-1.2.dev2316/monai/apps/reconstruction/networks/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/reconstruction/networks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.072857 monai-weekly-1.2.dev2316/monai/apps/reconstruction/networks/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/reconstruction/networks/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/reconstruction/networks/blocks/varnetblock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.072857 monai-weekly-1.2.dev2316/monai/apps/reconstruction/networks/nets/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/reconstruction/networks/nets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/reconstruction/networks/nets/coil_sensitivity_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/reconstruction/networks/nets/complex_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/reconstruction/networks/nets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/reconstruction/networks/nets/varnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.076856 monai-weekly-1.2.dev2316/monai/apps/reconstruction/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/reconstruction/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12240 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/reconstruction/transforms/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    15844 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/reconstruction/transforms/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.076856 monai-weekly-1.2.dev2316/monai/apps/tcia/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/tcia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/tcia/label_desc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/tcia/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13505 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.080856 monai-weekly-1.2.dev2316/monai/auto3dseg/
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/auto3dseg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/auto3dseg/algo_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)    41223 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/auto3dseg/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/auto3dseg/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/auto3dseg/seg_summarizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12193 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/auto3dseg/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.080856 monai-weekly-1.2.dev2316/monai/bundle/
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/bundle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/bundle/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16035 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/bundle/config_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    22410 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/bundle/config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/bundle/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    14353 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/bundle/reference_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    63733 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/bundle/scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/bundle/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16520 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/bundle/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.084856 monai-weekly-1.2.dev2316/monai/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/config/deviceconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/config/type_definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.092856 monai-weekly-1.2.dev2316/monai/data/
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50102 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/data/box_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/data/csv_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/data/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    68927 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/data/dataset_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    10318 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/data/decathlon_datalist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/data/fft_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/data/folder_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)    12484 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/data/grid_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/data/image_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    60619 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/data/image_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    39872 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/data/image_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13309 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/data/iterable_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14097 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/data/itk_torch_bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/data/meta_obj.py
--rw-r--r--   0 runner    (1001) docker     (123)    27321 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/data/meta_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/data/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/data/synthetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/data/test_time_augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8840 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/data/thread_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/data/torchscript_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    64795 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/data/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9059 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/data/video_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    18631 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/data/wsi_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    49442 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/data/wsi_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.096856 monai-weekly-1.2.dev2316/monai/engines/
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24568 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/engines/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/engines/multi_gpu_supervised_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    21347 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/engines/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11631 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/engines/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15250 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/engines/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.096856 monai-weekly-1.2.dev2316/monai/fl/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/fl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.096856 monai-weekly-1.2.dev2316/monai/fl/client/
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/fl/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/fl/client/client_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)    32635 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/fl/client/monai_algo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.096856 monai-weekly-1.2.dev2316/monai/fl/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/fl/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/fl/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/fl/utils/exchange_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/fl/utils/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.112856 monai-weekly-1.2.dev2316/monai/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/checkpoint_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    16071 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/checkpoint_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7606 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/classification_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/clearml_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/decollate_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/earlystop_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/garbage_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/hausdorff_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/ignite_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/logfile_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/lr_schedule_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/mean_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/mean_iou.py
--rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/metric_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/metrics_reloaded_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8560 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/metrics_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)    16326 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/mlflow_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/nvtx_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/panoptic_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/parameter_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/probability_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/regression_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/roc_auc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/smartcache_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    14251 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/stats_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/surface_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)    23325 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/tensorboard_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/validation_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.116856 monai-weekly-1.2.dev2316/monai/inferers/
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/inferers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32038 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/inferers/inferer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/inferers/merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/inferers/splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)    20036 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/inferers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.124856 monai-weekly-1.2.dev2316/monai/losses/
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/losses/contrastive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/losses/deform.py
--rw-r--r--   0 runner    (1001) docker     (123)    46326 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/losses/dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/losses/ds_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/losses/focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/losses/giou_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    15492 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/losses/image_dissimilarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/losses/multi_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/losses/spatial_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/losses/ssim_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/losses/tversky.py
--rw-r--r--   0 runner    (1001) docker     (123)    10224 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/losses/unified_focal_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.136856 monai-weekly-1.2.dev2316/monai/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/metrics/active_learning_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    15101 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/metrics/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/metrics/cumulative_average.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/metrics/f_beta_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/metrics/froc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/metrics/generalized_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)    11470 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/metrics/hausdorff_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/metrics/loss_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    10937 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/metrics/meandice.py
--rw-r--r--   0 runner    (1001) docker     (123)     7209 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/metrics/meaniou.py
--rw-r--r--   0 runner    (1001) docker     (123)    15140 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    13679 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/metrics/panoptic_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)    18235 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/metrics/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/metrics/rocauc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14415 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/metrics/surface_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)    10186 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/metrics/surface_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)    15094 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/metrics/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11772 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/metrics/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.136856 monai-weekly-1.2.dev2316/monai/networks/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.152856 monai-weekly-1.2.dev2316/monai/networks/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/blocks/acti_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/blocks/activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/blocks/aspp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/blocks/backbone_fpn_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11686 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/blocks/convolutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/blocks/crf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/blocks/denseblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/blocks/dints_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/blocks/downsample.py
--rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/blocks/dynunet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/blocks/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/blocks/fcn.py
--rw-r--r--   0 runner    (1001) docker     (123)    10586 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/blocks/feature_pyramid_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/blocks/fft_utils_t.py
--rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/blocks/localnet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/blocks/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/blocks/patchembedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/blocks/regunet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/blocks/segresnet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/blocks/selfattention.py
--rw-r--r--   0 runner    (1001) docker     (123)    12752 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/blocks/squeeze_and_excitation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/blocks/text_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/blocks/transformerblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/blocks/unetr_block.py
--rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/blocks/upsample.py
--rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/blocks/warp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.156856 monai-weekly-1.2.dev2316/monai/networks/layers/
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/layers/convutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/layers/drop_path.py
--rw-r--r--   0 runner    (1001) docker     (123)    12620 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/layers/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)    17992 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/layers/filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/layers/gmm.py
--rw-r--r--   0 runner    (1001) docker     (123)    28470 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/layers/simplelayers.py
--rw-r--r--   0 runner    (1001) docker     (123)    25576 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/layers/spatial_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/layers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/layers/weight_init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.172855 monai-weekly-1.2.dev2316/monai/networks/nets/
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21533 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/ahnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     9202 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/attentionunet.py
--rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    10950 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/basic_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7960 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/basic_unetplusplus.py
--rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    15820 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/densenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    44771 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/dints.py
--rw-r--r--   0 runner    (1001) docker     (123)    18210 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/dynunet.py
--rw-r--r--   0 runner    (1001) docker     (123)    40643 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    14147 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/flexible_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/fullyconnectednet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/highresnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    28678 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/hovernet.py
--rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/milmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/netadapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)    17189 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/regunet.py
--rw-r--r--   0 runner    (1001) docker     (123)    16785 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    13994 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/segresnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    15667 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/segresnet_ds.py
--rw-r--r--   0 runner    (1001) docker     (123)    19289 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/senet.py
--rw-r--r--   0 runner    (1001) docker     (123)    42000 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/swin_unetr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/torchvision_fc.py
--rw-r--r--   0 runner    (1001) docker     (123)    16626 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/transchex.py
--rw-r--r--   0 runner    (1001) docker     (123)    13722 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7943 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/unetr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/varautoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/vitautoenc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/vnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    46286 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.176855 monai-weekly-1.2.dev2316/monai/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21952 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/optimizers/lr_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/optimizers/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/optimizers/novograd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/optimizers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.184856 monai-weekly-1.2.dev2316/monai/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)    15248 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8946 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/adaptors.py
--rw-r--r--   0 runner    (1001) docker     (123)    40532 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/compose.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.188856 monai-weekly-1.2.dev2316/monai/transforms/croppad/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/croppad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    67678 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/croppad/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/croppad/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)    54071 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/croppad/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)    12673 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/croppad/functional.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.188856 monai-weekly-1.2.dev2316/monai/transforms/intensity/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/intensity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    98613 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/intensity/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    76501 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/intensity/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)    17160 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/inverse.py
--rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/inverse_batch_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.188856 monai-weekly-1.2.dev2316/monai/transforms/io/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25430 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/io/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    17821 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/io/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.192855 monai-weekly-1.2.dev2316/monai/transforms/lazy/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/lazy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/lazy/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     9851 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/lazy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.192855 monai-weekly-1.2.dev2316/monai/transforms/meta_utility/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/meta_utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/meta_utility/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/nvtx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.196855 monai-weekly-1.2.dev2316/monai/transforms/post/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/post/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40858 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/post/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    39905 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/post/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.196855 monai-weekly-1.2.dev2316/monai/transforms/signal/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/signal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16378 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/signal/array.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.196855 monai-weekly-1.2.dev2316/monai/transforms/smooth_field/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/smooth_field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17833 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/smooth_field/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/smooth_field/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.200855 monai-weekly-1.2.dev2316/monai/transforms/spatial/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/spatial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   168618 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/spatial/array.py
--rw-r--r--   0 runner    (1001) docker     (123)   107151 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/spatial/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)    31494 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/spatial/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/traits.py
--rw-r--r--   0 runner    (1001) docker     (123)    18234 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.204855 monai-weekly-1.2.dev2316/monai/transforms/utility/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    70325 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/utility/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    75816 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/utility/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)    72516 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    31081 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/utils_create_transform_ims.py
--rw-r--r--   0 runner    (1001) docker     (123)    18397 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/utils_pytorch_numpy_unification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.216855 monai-weekly-1.2.dev2316/monai/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/utils/aliases.py
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    14759 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/utils/deprecate_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8526 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/utils/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)    16807 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/utils/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    15637 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/utils/jupyter_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    27512 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    23631 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/utils/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/utils/nvtx.py
--rw-r--r--   0 runner    (1001) docker     (123)    15936 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/utils/profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/utils/state_cacher.py
--rw-r--r--   0 runner    (1001) docker     (123)    21147 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/utils/type_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.220855 monai-weekly-1.2.dev2316/monai/visualize/
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/visualize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16156 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/visualize/class_activation_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/visualize/gradient_based.py
--rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/visualize/img2tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    18816 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/visualize/occlusion_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     9966 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/visualize/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/visualize/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.220855 monai-weekly-1.2.dev2316/monai_weekly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-04-16 02:21:47.000000 monai-weekly-1.2.dev2316/monai_weekly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    33869 2023-04-16 02:21:48.000000 monai-weekly-1.2.dev2316/monai_weekly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 02:21:47.000000 monai-weekly-1.2.dev2316/monai_weekly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 02:21:47.000000 monai-weekly-1.2.dev2316/monai_weekly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-16 02:21:47.000000 monai-weekly-1.2.dev2316/monai_weekly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-16 02:21:47.000000 monai-weekly-1.2.dev2316/monai_weekly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-04-16 02:21:48.476853 monai-weekly-1.2.dev2316/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.476853 monai-weekly-1.2.dev2316/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_acn_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_activationsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_adaptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_add_channeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_add_coordinate_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_add_coordinate_channelsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_add_extreme_points_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_add_extreme_points_channeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_adjust_contrast.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_adjust_contrastd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_adn.py
--rw-r--r--   0 runner    (1001) docker     (123)     9979 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_affine.py
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_affine_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    19674 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_affine_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_affined.py
--rw-r--r--   0 runner    (1001) docker     (123)     8343 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_ahnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_anchor_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_apply.py
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_apply_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_arraydataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_as_channel_first.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_as_channel_firstd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_as_channel_last.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_as_channel_lastd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_as_discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_as_discreted.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_atss_box_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_attentionunet.py
--rw-r--r--   0 runner    (1001) docker     (123)    21578 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_auto3dseg.py
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_auto3dseg_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_auto3dseg_hpo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_avg_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_basic_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_basic_unetplusplus.py
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_bending_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)    13648 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_bilateral_approx_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    13773 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_bilateral_approx_cuda.py
--rw-r--r--   0 runner    (1001) docker     (123)    15064 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_bilateral_precise.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_blend_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_border_pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_border_padd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_bounding_rect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_bounding_rectd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_box_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)    17289 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_box_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     8925 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_box_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_bundle_ckpt_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     7692 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_bundle_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_bundle_get_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_bundle_init_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_bundle_onnx_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_bundle_trt_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_bundle_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_bundle_verify_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_bundle_verify_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_bundle_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_cachedataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_cachedataset_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_cachedataset_persistent_workers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_cachentransdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_call_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_cast_to_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_cast_to_typed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_center_scale_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_center_scale_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_center_spatial_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_center_spatial_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_channel_pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_check_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_check_missing_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_classes_to_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_classes_to_indicesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_complex_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_component_locator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11371 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_compose.py
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_compose_get_number_conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10091 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_compute_confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_compute_f_beta.py
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_compute_froc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_compute_generalized_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_compute_ho_ver_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_compute_ho_ver_maps_d.py
--rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_compute_meandice.py
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_compute_meaniou.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_compute_panoptic_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_compute_regression_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_compute_roc_auc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_compute_variance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_concat_itemsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_config_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    14667 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_contrastive_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_convert_data_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_convert_to_multi_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_convert_to_multi_channeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_convert_to_onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_convert_to_torchscript.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_convert_to_trt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_convolutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_copy_itemsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_copy_model_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_correct_crop_centers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_create_cross_validation_datalist.py
--rw-r--r--   0 runner    (1001) docker     (123)    10466 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_create_grid_and_affine.py
--rw-r--r--   0 runner    (1001) docker     (123)    18866 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_crf_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    19445 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_crf_cuda.py
--rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_crop_foreground.py
--rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_crop_foregroundd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_cross_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8682 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11089 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_csv_iterable_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_csv_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_cucim_dict_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_cucim_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_cumulative.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_cumulative_average.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_cumulative_average_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_cv2_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_data_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_data_statsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_dataset_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_dataset_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_decathlondataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10357 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_decollate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_deepedit_interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_deepedit_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_deepgrow_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_deepgrow_interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    16313 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_deepgrow_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_delete_itemsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_denseblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_densenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    14747 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_detect_envelope.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_detection_coco_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_detector_boxselector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_detector_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_dev_collate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_dice_ce_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_dice_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_dints_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_dints_mixop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_dints_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_divisible_pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_divisible_padd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_download_and_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_downsample_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_drop_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_ds_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_dvf2ddf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_dynunet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_dynunet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_ensemble_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_ensure_channel_first.py
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_ensure_channel_firstd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_ensure_tuple.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_ensure_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_ensure_typed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_enum_bound_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_eval_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_evenly_divisible_all_gather_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_factorized_increase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_factorized_reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_fastmri_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_fft_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_fg_bg_to_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_fg_bg_to_indicesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_file_basename.py
--rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_fill_holes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_fill_holesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_fl_exchange_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_fl_monai_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_fl_monai_algo_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_fl_monai_algo_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_flatten_sub_keysd.py
--rw-r--r--   0 runner    (1001) docker     (123)    13497 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_flexible_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_flip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_flipd.py
--rw-r--r--   0 runner    (1001) docker     (123)    12045 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_folder_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_foreground_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_foreground_maskd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_fourier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_fpn_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_from_engine_hovernet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_fullyconnectednet.py
--rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     8085 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_gaussian_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_gaussian_sharpen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_gaussian_sharpend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_gaussian_smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_gaussian_smoothd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_generalized_dice_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     8036 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_generalized_dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_generalized_wasserstein_dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_generate_distance_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_generate_distance_mapd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_generate_instance_border.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_generate_instance_borderd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_generate_instance_centroid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_generate_instance_centroidd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_generate_instance_contour.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_generate_instance_contourd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_generate_instance_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_generate_instance_typed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_generate_label_classes_crop_centers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_generate_param_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_generate_pos_neg_label_crop_centers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_generate_spatial_bounding_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_generate_succinct_contour.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_generate_succinct_contourd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_generate_watershed_markers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_generate_watershed_markersd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_generate_watershed_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_generate_watershed_maskd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_get_equivalent_dtype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_get_extreme_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_get_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_get_package_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_get_unique_labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_gibbs_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_gibbs_noised.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_giou_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_global_mutual_information_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_globalnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     9431 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_gmm.py
--rw-r--r--   0 runner    (1001) docker     (123)     8683 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_grid_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_grid_distortion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_grid_distortiond.py
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_grid_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_grid_patchd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_grid_pull.py
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_grid_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_grid_splitd.py
--rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_checkpoint_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_checkpoint_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_classification_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_classification_saver_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_clearml_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_clearml_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_confusion_matrix_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_decollate_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_early_stop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_garbage_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_hausdorff_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_logfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_mean_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_mean_iou.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_metric_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_metrics_reloaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_metrics_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_metrics_saver_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_mlflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_nvtx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_panoptic_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_parameter_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_prob_map_producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_regression_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_regression_metrics_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_rocauc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_rocauc_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_smartcache.py
--rw-r--r--   0 runner    (1001) docker     (123)     9501 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_surface_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_tb_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_tb_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_hardnegsampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_hausdorff_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_header_correct.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_highresnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_hilbert_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_histogram_normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_histogram_normalized.py
--rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_hovernet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_hovernet_instance_map_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_hovernet_instance_map_post_processingd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_hovernet_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_hovernet_nuclear_type_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_hovernet_nuclear_type_post_processingd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_identityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_image_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10444 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_image_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_image_rw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_img2tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_init_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_integration_autorunner.py
--rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_integration_bundle_run.py
--rw-r--r--   0 runner    (1001) docker     (123)    11166 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_integration_classification_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_integration_determinism.py
--rw-r--r--   0 runner    (1001) docker     (123)     9737 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_integration_fast_train.py
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_integration_gpu_customization.py
--rw-r--r--   0 runner    (1001) docker     (123)     8693 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_integration_lazy_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_integration_nnunetv2_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    13199 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_integration_segmentation_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_integration_sliding_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_integration_stn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_integration_unet_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_integration_workers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14035 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_integration_workflows.py
--rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_integration_workflows_gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_intensity_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_intensity_statsd.py
--rw-r--r--   0 runner    (1001) docker     (123)    18873 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_inverse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_inverse_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_inverse_collation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_invert.py
--rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_invertd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_is_supported_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_iterable_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    18618 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_itk_torch_bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_itk_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_k_space_spike_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_k_space_spike_noised.py
--rw-r--r--   0 runner    (1001) docker     (123)    14754 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_keep_largest_connected_component.py
--rw-r--r--   0 runner    (1001) docker     (123)    12548 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_keep_largest_connected_componentd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_kspace_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_label_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_label_filterd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_label_quality_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_label_to_contour.py
--rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_label_to_contourd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_label_to_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_label_to_maskd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_lambda.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_lambdad.py
--rw-r--r--   0 runner    (1001) docker     (123)     9763 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_lesion_froc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_list_data_collate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_list_to_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_lltm.py
--rw-r--r--   0 runner    (1001) docker     (123)    10439 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_lmdbdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_lmdbdataset_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_load_decathlon_datalist.py
--rw-r--r--   0 runner    (1001) docker     (123)    15192 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_load_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     8802 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_load_imaged.py
--rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_load_spacing_orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_loader_semaphore.py
--rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_local_normalized_cross_correlation_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_localnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_localnet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_look_up_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_loss_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_lr_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_make_nifti.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_map_binary_to_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_map_classes_to_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_map_label_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_map_label_valued.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_map_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_mask_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_mask_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_masked_dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_masked_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_masked_patch_wsi_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_matshow3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_mean_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_mean_ensembled.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_median_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_median_smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_median_smoothd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_mednistdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_meta_affine.py
--rw-r--r--   0 runner    (1001) docker     (123)    23490 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_meta_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_metatensor_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_metrics_reloaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_milmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_mmar_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_module_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_monai_env_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_monai_utils_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_mri_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_multi_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_net_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_network_consistency.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_nifti_endianness.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_nifti_header_revise.py
--rw-r--r--   0 runner    (1001) docker     (123)    12065 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_nifti_rw.py
--rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_normalize_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_normalize_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_npzdictitemdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_nrrd_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     9614 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_nuclick_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_numpy_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10734 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_nvtx_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_nvtx_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_occlusion_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_one_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_optim_novograd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_optional_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_ori_ras_lps.py
--rw-r--r--   0 runner    (1001) docker     (123)     8099 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_orientationd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_p3d_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_pad_collation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_pad_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_parallel_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_parallel_execution_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_partition_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_partition_dataset_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_patch_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_patch_inferer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8349 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_patch_wsi_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_patchembedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_pathology_he_stain.py
--rw-r--r--   0 runner    (1001) docker     (123)    10277 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_pathology_he_stain_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_pathology_prob_nms.py
--rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_persistentdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_persistentdataset_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     9041 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_phl_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_phl_cuda.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_pil_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_plot_2d_or_3d_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_png_rw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_polyval.py
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_prepare_batch_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_prepare_batch_default_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_prepare_batch_extra_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_prepare_batch_hovernet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_preset_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_print_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_print_transform_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_probnms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_probnmsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_pytorch_version_after.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_query_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_adjust_contrast.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_adjust_contrastd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_affine.py
--rw-r--r--   0 runner    (1001) docker     (123)     9724 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_affine_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    10960 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_affined.py
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_axis_flip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_axis_flipd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_bias_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_bias_fieldd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_coarse_dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_coarse_dropoutd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_coarse_shuffle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_coarse_shuffled.py
--rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_crop_by_label_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_crop_by_label_classesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_crop_by_pos_neg_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_crop_by_pos_neg_labeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_cucim_dict_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_cucim_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_deform_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_elastic_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_elastic_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_elasticd_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_elasticd_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_flip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_flipd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_gaussian_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_gaussian_noised.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_gaussian_sharpen.py
--rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_gaussian_sharpend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_gaussian_smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_gaussian_smoothd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_gibbs_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_gibbs_noised.py
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_grid_distortion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_grid_distortiond.py
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_grid_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_grid_patchd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_histogram_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_histogram_shiftd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_k_space_spike_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_k_space_spike_noised.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_lambda.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_lambdad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_rician_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_rician_noised.py
--rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_rotate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_rotate90.py
--rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_rotate90d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_rotated.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_scale_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_scale_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_scale_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_scale_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_shift_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_shift_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_spatial_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_spatial_crop_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_spatial_crop_samplesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_spatial_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_std_shift_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_std_shift_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_weighted_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_weighted_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_zoom.py
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_zoomd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_randidentity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_random_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_randomizable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_randomizable_transform_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_randtorchvisiond.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rankfilter_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_recon_net_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_reference_based_normalize_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_reference_based_spatial_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_reference_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_reg_loss_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_regunet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_regunet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_remove_repeated_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_remove_repeated_channeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_remove_small_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_repeat_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_repeat_channeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_replace_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_require_pkg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_resample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_resample_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_resample_datalist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_resample_to_match.py
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_resample_to_matchd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_resampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_resize.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_resize_with_pad_or_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_resize_with_pad_or_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_resized.py
--rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_retinanet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_retinanet_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_retinanet_predict_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rotate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rotate90.py
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rotate90d.py
--rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rotated.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_safe_dtype_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_saliency_inferer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_sample_slices.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_sampler_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_save_classificationd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_save_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_save_imaged.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_save_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_savitzky_golay_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_savitzky_golay_smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_savitzky_golay_smoothd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_scale_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_scale_intensity_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_scale_intensity_range_percentiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_scale_intensity_range_percentilesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_scale_intensity_ranged.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_scale_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_se_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_se_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_seg_loss_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_segresnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_segresnet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_segresnet_ds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_select_cross_validation_folds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_select_itemsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_selfattention.py
--rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_senet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_separable_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_set_determinism.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_set_visible_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_shift_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_shift_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_shuffle_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_signal_continuouswavelet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_signal_fillempty.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_signal_rand_add_gaussiannoise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_signal_rand_add_sine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_signal_rand_add_sine_partial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_signal_rand_add_squarepulse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_signal_rand_add_squarepulse_partial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_signal_rand_drop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_signal_rand_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_signal_rand_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_signal_remove_frequency.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_simple_aspp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_simulatedelay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_simulatedelayd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_skip_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_slice_inferer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10903 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_sliding_patch_wsi_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11961 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_sliding_window_hovernet_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)    15505 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_sliding_window_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_sliding_window_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7514 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_smartcachedataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_smooth_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_sobel_gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_sobel_gradientd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_some_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    14525 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_spacing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_spacingd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7930 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_spatial_combine_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_spatial_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_spatial_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_spatial_pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_spatial_padd.py
--rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_spatial_resample.py
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_spatial_resampled.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_split_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_split_channeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_splitdim.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_splitdimd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_squeezedim.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_squeezedimd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_ssim_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_ssim_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_state_cacher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_std_shift_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_std_shift_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_str2bool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_str2list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_subpixel_upsample.py
--rw-r--r--   0 runner    (1001) docker     (123)    18990 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_surface_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_surface_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_swin_unetr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_synthetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_tciadataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_testtimeaugmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_text_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_thread_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_threadcontainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_threshold_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_threshold_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_timedcall_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_to_contiguous.py
--rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_to_cupy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_to_cupyd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_to_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_to_deviced.py
--rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_to_from_meta_tensord.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_to_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_to_numpyd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_to_onehot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_to_pil.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_to_pild.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_to_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_to_tensord.py
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_torchscript_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_torchvision.py
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_torchvision_fc_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_torchvisiond.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_traceable_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_train_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    16832 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_trainable_bilateral.py
--rw-r--r--   0 runner    (1001) docker     (123)    21398 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_trainable_joint_bilateral.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_transchex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_transformerblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_transpose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_transposed.py
--rw-r--r--   0 runner    (1001) docker     (123)     7738 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_tversky_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_unetr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_unetr_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_unified_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_upsample_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_utils_pytorch_numpy_unification.py
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_varautoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_varnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_version_leq.py
--rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_video_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_vis_cam.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_vis_gradbased.py
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_vis_gradcam.py
--rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_vitautoenc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_vnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_vote_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_vote_ensembled.py
--rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_warp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_watershed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_watershedd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_weight_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_weighted_random_sampler_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_with_allow_missing_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_write_metrics_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)    25914 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_wsireader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_zipdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_zoom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_zoom_affine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_zoomd.py
--rw-r--r--   0 runner    (1001) docker     (123)    81097 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.931623 monai-weekly-1.2.dev2317/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-04-23 02:24:34.931623 monai-weekly-1.2.dev2317/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.935623 monai-weekly-1.2.dev2317/monai/
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-04-23 02:22:48.000000 monai-weekly-1.2.dev2317/monai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.475618 monai-weekly-1.2.dev2317/monai/_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/_extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.475618 monai-weekly-1.2.dev2317/monai/_extensions/gmm/
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/_extensions/gmm/gmm.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/_extensions/gmm/gmm.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/_extensions/gmm/gmm_cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16213 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/_extensions/gmm/gmm_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/_extensions/gmm/gmm_cuda_linalg.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/_extensions/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-23 02:24:34.935623 monai-weekly-1.2.dev2317/monai/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.479619 monai-weekly-1.2.dev2317/monai/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.483619 monai-weekly-1.2.dev2317/monai/apps/auto3dseg/
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/auto3dseg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/auto3dseg/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37105 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/auto3dseg/auto_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26014 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/auto3dseg/bundle_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17319 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/auto3dseg/data_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23351 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/auto3dseg/ensemble_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17523 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/auto3dseg/hpo_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/auto3dseg/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/auto3dseg/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34568 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.487619 monai-weekly-1.2.dev2317/monai/apps/deepedit/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/deepedit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/deepedit/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37435 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/deepedit/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.487619 monai-weekly-1.2.dev2317/monai/apps/deepgrow/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/deepgrow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10054 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/deepgrow/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/deepgrow/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42011 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/deepgrow/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.487619 monai-weekly-1.2.dev2317/monai/apps/detection/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/detection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.491619 monai-weekly-1.2.dev2317/monai/apps/detection/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/detection/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26617 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/detection/metrics/coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17161 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/detection/metrics/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.491619 monai-weekly-1.2.dev2317/monai/apps/detection/networks/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/detection/networks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53221 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/detection/networks/retinanet_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18850 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/detection/networks/retinanet_network.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.495619 monai-weekly-1.2.dev2317/monai/apps/detection/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/detection/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24519 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/detection/transforms/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17916 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/detection/transforms/box_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68979 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/detection/transforms/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.499619 monai-weekly-1.2.dev2317/monai/apps/detection/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    13531 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/detection/utils/ATSS_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/detection/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18681 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/detection/utils/anchor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11120 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/detection/utils/box_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/detection/utils/box_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10306 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/detection/utils/detector_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13890 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/detection/utils/hard_negative_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/detection/utils/predict_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.499619 monai-weekly-1.2.dev2317/monai/apps/mmars/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/mmars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13115 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/mmars/mmars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9996 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/mmars/model_desc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.503619 monai-weekly-1.2.dev2317/monai/apps/nnunet/
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/nnunet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/nnunet/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38587 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/nnunet/nnunetv2_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/nnunet/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.503619 monai-weekly-1.2.dev2317/monai/apps/nuclick/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/nuclick/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24948 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/nuclick/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.503619 monai-weekly-1.2.dev2317/monai/apps/pathology/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/pathology/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.503619 monai-weekly-1.2.dev2317/monai/apps/pathology/engines/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/pathology/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/pathology/engines/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.507619 monai-weekly-1.2.dev2317/monai/apps/pathology/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/pathology/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/pathology/handlers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.507619 monai-weekly-1.2.dev2317/monai/apps/pathology/inferers/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/pathology/inferers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9148 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/pathology/inferers/inferer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.507619 monai-weekly-1.2.dev2317/monai/apps/pathology/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/pathology/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7293 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/pathology/losses/hovernet_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.507619 monai-weekly-1.2.dev2317/monai/apps/pathology/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/pathology/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/pathology/metrics/lesion_froc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.507619 monai-weekly-1.2.dev2317/monai/apps/pathology/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/pathology/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.511619 monai-weekly-1.2.dev2317/monai/apps/pathology/transforms/post/
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/pathology/transforms/post/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37322 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/pathology/transforms/post/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25928 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/pathology/transforms/post/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.511619 monai-weekly-1.2.dev2317/monai/apps/pathology/transforms/stain/
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/pathology/transforms/stain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/pathology/transforms/stain/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/pathology/transforms/stain/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/pathology/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.511619 monai-weekly-1.2.dev2317/monai/apps/reconstruction/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/reconstruction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/reconstruction/complex_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/reconstruction/fastmri_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/reconstruction/mri_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.511619 monai-weekly-1.2.dev2317/monai/apps/reconstruction/networks/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/reconstruction/networks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.515619 monai-weekly-1.2.dev2317/monai/apps/reconstruction/networks/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/reconstruction/networks/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/reconstruction/networks/blocks/varnetblock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.515619 monai-weekly-1.2.dev2317/monai/apps/reconstruction/networks/nets/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/reconstruction/networks/nets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/reconstruction/networks/nets/coil_sensitivity_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/reconstruction/networks/nets/complex_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/reconstruction/networks/nets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/reconstruction/networks/nets/varnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.515619 monai-weekly-1.2.dev2317/monai/apps/reconstruction/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/reconstruction/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12240 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/reconstruction/transforms/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15844 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/reconstruction/transforms/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.519619 monai-weekly-1.2.dev2317/monai/apps/tcia/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/tcia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/tcia/label_desc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/tcia/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13505 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/apps/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.519619 monai-weekly-1.2.dev2317/monai/auto3dseg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/auto3dseg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/auto3dseg/algo_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41223 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/auto3dseg/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/auto3dseg/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/auto3dseg/seg_summarizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12193 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/auto3dseg/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.523619 monai-weekly-1.2.dev2317/monai/bundle/
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/bundle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/bundle/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16035 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/bundle/config_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22410 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/bundle/config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/bundle/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14353 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/bundle/reference_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63940 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/bundle/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/bundle/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17082 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/bundle/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.527619 monai-weekly-1.2.dev2317/monai/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/config/deviceconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/config/type_definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.539619 monai-weekly-1.2.dev2317/monai/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50102 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/data/box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/data/csv_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/data/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68927 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/data/dataset_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10318 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/data/decathlon_datalist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/data/fft_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/data/folder_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12484 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/data/grid_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/data/image_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60619 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/data/image_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39872 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/data/image_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13309 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/data/iterable_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14097 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/data/itk_torch_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/data/meta_obj.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27321 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/data/meta_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/data/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/data/synthetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/data/test_time_augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8840 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/data/thread_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/data/torchscript_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64795 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9059 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/data/video_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18619 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/data/wsi_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49442 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/data/wsi_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.543619 monai-weekly-1.2.dev2317/monai/engines/
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24568 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/engines/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/engines/multi_gpu_supervised_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21347 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/engines/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11631 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/engines/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15250 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/engines/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.543619 monai-weekly-1.2.dev2317/monai/fl/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/fl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.543619 monai-weekly-1.2.dev2317/monai/fl/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/fl/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/fl/client/client_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33232 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/fl/client/monai_algo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.547619 monai-weekly-1.2.dev2317/monai/fl/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/fl/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/fl/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/fl/utils/exchange_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/fl/utils/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.555619 monai-weekly-1.2.dev2317/monai/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/checkpoint_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16071 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/checkpoint_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7606 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/classification_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/clearml_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/decollate_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/earlystop_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/garbage_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/hausdorff_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/ignite_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/logfile_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/lr_schedule_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/mean_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/mean_iou.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/metric_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/metrics_reloaded_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8560 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/metrics_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16326 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/mlflow_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/nvtx_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/panoptic_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/parameter_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/probability_maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/regression_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/roc_auc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/smartcache_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14251 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/stats_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/surface_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23325 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/tensorboard_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/handlers/validation_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.559620 monai-weekly-1.2.dev2317/monai/inferers/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/inferers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32038 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/inferers/inferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/inferers/merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/inferers/splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20017 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/inferers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.563619 monai-weekly-1.2.dev2317/monai/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/losses/contrastive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/losses/deform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46326 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/losses/dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/losses/ds_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/losses/focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/losses/giou_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15492 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/losses/image_dissimilarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/losses/multi_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/losses/spatial_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/losses/ssim_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/losses/tversky.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10224 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/losses/unified_focal_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.571620 monai-weekly-1.2.dev2317/monai/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/metrics/active_learning_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15101 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/metrics/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/metrics/cumulative_average.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/metrics/f_beta_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/metrics/froc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/metrics/generalized_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11470 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/metrics/hausdorff_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/metrics/loss_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/metrics/meandice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7209 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/metrics/meaniou.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15140 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13679 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/metrics/panoptic_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19719 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/metrics/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/metrics/rocauc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14415 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/metrics/surface_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10186 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/metrics/surface_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15094 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/metrics/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11772 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/metrics/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.571620 monai-weekly-1.2.dev2317/monai/networks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.583620 monai-weekly-1.2.dev2317/monai/networks/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/blocks/acti_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/blocks/activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/blocks/aspp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/blocks/backbone_fpn_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11686 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/blocks/convolutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/blocks/crf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/blocks/denseblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/blocks/dints_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/blocks/downsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/blocks/dynunet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/blocks/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/blocks/fcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10586 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/blocks/feature_pyramid_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/blocks/fft_utils_t.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/blocks/localnet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/blocks/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/blocks/patchembedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/blocks/regunet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/blocks/segresnet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/blocks/selfattention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12752 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/blocks/squeeze_and_excitation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/blocks/text_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/blocks/transformerblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/blocks/unetr_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/blocks/upsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/blocks/warp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.587620 monai-weekly-1.2.dev2317/monai/networks/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/layers/convutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/layers/drop_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12638 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/layers/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17992 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/layers/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/layers/gmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28470 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/layers/simplelayers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25576 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/layers/spatial_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/layers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/layers/weight_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.603620 monai-weekly-1.2.dev2317/monai/networks/nets/
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21533 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/ahnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9202 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/attentionunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10950 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/basic_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7960 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/basic_unetplusplus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15820 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44771 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/dints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18210 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/dynunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40643 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14147 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/flexible_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/fullyconnectednet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/highresnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28678 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/hovernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/milmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/netadapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17189 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/regunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16785 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13994 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/segresnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15667 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/segresnet_ds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19289 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/senet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42000 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/swin_unetr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/torchvision_fc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16626 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/transchex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13722 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7943 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/unetr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/varautoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/vitautoenc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/nets/vnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46938 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/networks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.603620 monai-weekly-1.2.dev2317/monai/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21952 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/optimizers/lr_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/optimizers/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/optimizers/novograd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/optimizers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.611620 monai-weekly-1.2.dev2317/monai/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)    15248 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8946 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/adaptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40812 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/compose.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.615620 monai-weekly-1.2.dev2317/monai/transforms/croppad/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/croppad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68231 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/croppad/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/croppad/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54071 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/croppad/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12673 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/croppad/functional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.619620 monai-weekly-1.2.dev2317/monai/transforms/intensity/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/intensity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98613 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/intensity/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76501 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/intensity/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18000 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/inverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/inverse_batch_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.619620 monai-weekly-1.2.dev2317/monai/transforms/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25430 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/io/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17821 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/io/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.623620 monai-weekly-1.2.dev2317/monai/transforms/lazy/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/lazy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/lazy/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9851 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/lazy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.623620 monai-weekly-1.2.dev2317/monai/transforms/meta_utility/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/meta_utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/meta_utility/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/nvtx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.623620 monai-weekly-1.2.dev2317/monai/transforms/post/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/post/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40858 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/post/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39905 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/post/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.627620 monai-weekly-1.2.dev2317/monai/transforms/signal/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/signal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16378 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/signal/array.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.627620 monai-weekly-1.2.dev2317/monai/transforms/smooth_field/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/smooth_field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17833 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/smooth_field/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/smooth_field/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.631620 monai-weekly-1.2.dev2317/monai/transforms/spatial/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/spatial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   168618 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/spatial/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107151 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/spatial/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31494 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/spatial/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18234 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.635620 monai-weekly-1.2.dev2317/monai/transforms/utility/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70839 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/utility/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76330 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/utility/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72516 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31081 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/utils_create_transform_ims.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18397 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/transforms/utils_pytorch_numpy_unification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.639620 monai-weekly-1.2.dev2317/monai/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/utils/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14759 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/utils/deprecate_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8526 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/utils/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16807 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/utils/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15637 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/utils/jupyter_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27512 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23631 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/utils/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/utils/nvtx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15936 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/utils/profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/utils/state_cacher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21147 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/utils/type_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.643620 monai-weekly-1.2.dev2317/monai/visualize/
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/visualize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16156 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/visualize/class_activation_maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/visualize/gradient_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/visualize/img2tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18816 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/visualize/occlusion_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9966 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/visualize/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/monai/visualize/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.647620 monai-weekly-1.2.dev2317/monai_weekly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-04-23 02:24:34.000000 monai-weekly-1.2.dev2317/monai_weekly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    33869 2023-04-23 02:24:34.000000 monai-weekly-1.2.dev2317/monai_weekly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 02:24:34.000000 monai-weekly-1.2.dev2317/monai_weekly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 02:24:34.000000 monai-weekly-1.2.dev2317/monai_weekly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-23 02:24:34.000000 monai-weekly-1.2.dev2317/monai_weekly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 02:24:34.000000 monai-weekly-1.2.dev2317/monai_weekly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-04-23 02:24:34.931623 monai-weekly-1.2.dev2317/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:24:34.931623 monai-weekly-1.2.dev2317/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_acn_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_activationsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_adaptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_add_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_add_coordinate_channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_add_coordinate_channelsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_add_extreme_points_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_add_extreme_points_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_adjust_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_adjust_contrastd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_adn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9979 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_affine_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19674 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_affine_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_affined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8343 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_ahnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_anchor_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_apply_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_arraydataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_as_channel_first.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_as_channel_firstd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_as_channel_last.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_as_channel_lastd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_as_discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_as_discreted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_atss_box_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_attentionunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21578 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_auto3dseg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_auto3dseg_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_auto3dseg_hpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_avg_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_basic_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_basic_unetplusplus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_bending_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13648 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_bilateral_approx_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13773 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_bilateral_approx_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15064 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_bilateral_precise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_blend_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_border_pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_border_padd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_bounding_rect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_bounding_rectd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_box_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17289 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_box_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8925 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_bundle_ckpt_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7692 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_bundle_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_bundle_get_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_bundle_init_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_bundle_onnx_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_bundle_trt_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_bundle_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_bundle_verify_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_bundle_verify_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_bundle_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_cachedataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_cachedataset_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_cachedataset_persistent_workers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_cachentransdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_call_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_cast_to_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_cast_to_typed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_center_scale_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_center_scale_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_center_spatial_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_center_spatial_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_channel_pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_check_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_check_missing_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_classes_to_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_classes_to_indicesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_complex_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_component_locator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11371 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_compose_get_number_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10091 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_compute_confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_compute_f_beta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_compute_froc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_compute_generalized_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_compute_ho_ver_maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_compute_ho_ver_maps_d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_compute_meandice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_compute_meaniou.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_compute_panoptic_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_compute_regression_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_compute_roc_auc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_compute_variance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_concat_itemsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_config_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14667 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_contrastive_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_convert_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_convert_to_multi_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_convert_to_multi_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_convert_to_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_convert_to_torchscript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_convert_to_trt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_convolutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_copy_itemsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_copy_model_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_correct_crop_centers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_create_cross_validation_datalist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10466 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_create_grid_and_affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18866 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_crf_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19445 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_crf_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_crop_foreground.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_crop_foregroundd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_cross_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8682 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11089 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_csv_iterable_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_csv_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_cucim_dict_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_cucim_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_cumulative.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_cumulative_average.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_cumulative_average_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_cv2_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_data_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_data_statsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_dataset_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_dataset_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_decathlondataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10357 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_decollate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_deepedit_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_deepedit_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_deepgrow_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_deepgrow_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16313 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_deepgrow_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_delete_itemsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_denseblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_densenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14747 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_detect_envelope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_detection_coco_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_detector_boxselector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_detector_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_dev_collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_dice_ce_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_dice_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_dints_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_dints_mixop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_dints_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_divisible_pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_divisible_padd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_download_and_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_downsample_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_drop_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_ds_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_dvf2ddf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_dynunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_dynunet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_ensemble_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_ensure_channel_first.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_ensure_channel_firstd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_ensure_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_ensure_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_ensure_typed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_enum_bound_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_eval_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_evenly_divisible_all_gather_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_factorized_increase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_factorized_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_fastmri_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_fft_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_fg_bg_to_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_fg_bg_to_indicesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_file_basename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_fill_holes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_fill_holesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_fl_exchange_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8696 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_fl_monai_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_fl_monai_algo_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_fl_monai_algo_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_flatten_sub_keysd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13497 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_flexible_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_flipd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12045 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_folder_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_foreground_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_foreground_maskd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_fourier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_fpn_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_from_engine_hovernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_fullyconnectednet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8085 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_gaussian_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_gaussian_sharpen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_gaussian_sharpend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_gaussian_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_gaussian_smoothd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_generalized_dice_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8036 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_generalized_dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_generalized_wasserstein_dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_generate_distance_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_generate_distance_mapd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_generate_instance_border.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_generate_instance_borderd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_generate_instance_centroid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_generate_instance_centroidd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_generate_instance_contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_generate_instance_contourd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_generate_instance_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_generate_instance_typed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_generate_label_classes_crop_centers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_generate_param_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_generate_pos_neg_label_crop_centers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_generate_spatial_bounding_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_generate_succinct_contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_generate_succinct_contourd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_generate_watershed_markers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_generate_watershed_markersd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_generate_watershed_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_generate_watershed_maskd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_get_equivalent_dtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_get_extreme_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_get_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_get_package_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_get_unique_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_gibbs_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_gibbs_noised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_giou_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_global_mutual_information_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_globalnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9431 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_gmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8683 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_grid_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_grid_distortion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_grid_distortiond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_grid_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_grid_patchd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_grid_pull.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_grid_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_grid_splitd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_checkpoint_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_checkpoint_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_classification_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_classification_saver_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_clearml_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_clearml_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_confusion_matrix_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_decollate_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_early_stop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_garbage_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_hausdorff_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_logfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_mean_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_mean_iou.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_metric_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_metrics_reloaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_metrics_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_metrics_saver_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_nvtx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_panoptic_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_parameter_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_prob_map_producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_regression_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_regression_metrics_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_rocauc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_rocauc_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_smartcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9501 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_surface_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_tb_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_tb_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_handler_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_hardnegsampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_hausdorff_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_header_correct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_highresnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_hilbert_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_histogram_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_histogram_normalized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_hovernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_hovernet_instance_map_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_hovernet_instance_map_post_processingd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_hovernet_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_hovernet_nuclear_type_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_hovernet_nuclear_type_post_processingd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_identityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_image_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10444 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_image_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_image_rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_img2tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_init_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7555 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_integration_autorunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_integration_bundle_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11166 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_integration_classification_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_integration_determinism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9737 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_integration_fast_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_integration_gpu_customization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_integration_lazy_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_integration_nnunetv2_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13199 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_integration_segmentation_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_integration_sliding_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_integration_stn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_integration_unet_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_integration_workers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14035 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_integration_workflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_integration_workflows_gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_intensity_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_intensity_statsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18873 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_inverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_inverse_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_inverse_collation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_invert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_invertd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_is_supported_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_iterable_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18618 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_itk_torch_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_itk_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_k_space_spike_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_k_space_spike_noised.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14754 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_keep_largest_connected_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12548 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_keep_largest_connected_componentd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_kspace_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_label_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_label_filterd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_label_quality_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_label_to_contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_label_to_contourd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_label_to_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_label_to_maskd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_lambdad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9763 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_lesion_froc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_list_data_collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_list_to_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_lltm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_lmdbdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_lmdbdataset_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_load_decathlon_datalist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15192 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_load_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8802 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_load_imaged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_load_spacing_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_loader_semaphore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_local_normalized_cross_correlation_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_localnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_localnet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_look_up_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_loss_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_lr_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_make_nifti.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_map_binary_to_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_map_classes_to_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_map_label_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_map_label_valued.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_map_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_mask_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_mask_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_masked_dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_masked_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_masked_patch_wsi_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_matshow3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_mean_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_mean_ensembled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_median_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_median_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_median_smoothd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_mednistdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_meta_affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23490 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_meta_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_metatensor_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_metrics_reloaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_milmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_mmar_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_module_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_monai_env_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_monai_utils_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_mri_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_multi_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_net_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_network_consistency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_nifti_endianness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_nifti_header_revise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12065 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_nifti_rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_normalize_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_normalize_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_npzdictitemdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_nrrd_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9614 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_nuclick_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_numpy_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10734 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_nvtx_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_nvtx_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_occlusion_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_one_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_optim_novograd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_optional_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_ori_ras_lps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8099 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_orientationd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_p3d_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_pad_collation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_pad_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_parallel_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_parallel_execution_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_partition_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_partition_dataset_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_patch_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_patch_inferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8349 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_patch_wsi_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_patchembedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_pathology_he_stain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10277 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_pathology_he_stain_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_pathology_prob_nms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_persistentdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_persistentdataset_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9041 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_phl_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_phl_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_pil_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_plot_2d_or_3d_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_png_rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_polyval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_prepare_batch_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_prepare_batch_default_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_prepare_batch_extra_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_prepare_batch_hovernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_preset_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_print_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_print_transform_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_probnms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_probnmsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_pytorch_version_after.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_query_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_adjust_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_adjust_contrastd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9724 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_affine_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10960 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_affined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_axis_flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_axis_flipd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_bias_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_bias_fieldd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_coarse_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_coarse_dropoutd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_coarse_shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_coarse_shuffled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_crop_by_label_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_crop_by_label_classesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_crop_by_pos_neg_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_crop_by_pos_neg_labeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_cucim_dict_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_cucim_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_deform_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_elastic_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_elastic_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_elasticd_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_elasticd_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_flipd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_gaussian_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_gaussian_noised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_gaussian_sharpen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_gaussian_sharpend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_gaussian_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_gaussian_smoothd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_gibbs_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_gibbs_noised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_grid_distortion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_grid_distortiond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_grid_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_grid_patchd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_histogram_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_histogram_shiftd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_k_space_spike_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_k_space_spike_noised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_lambdad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_rician_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_rician_noised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_rotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_rotate90.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_rotate90d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_rotated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_scale_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_scale_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_scale_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_scale_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_shift_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_shift_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_spatial_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_spatial_crop_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_spatial_crop_samplesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_spatial_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_std_shift_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_std_shift_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_weighted_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_weighted_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_zoom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rand_zoomd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_randidentity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_random_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_randomizable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_randomizable_transform_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_randtorchvisiond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rankfilter_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_recon_net_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_reference_based_normalize_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_reference_based_spatial_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_reference_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_reg_loss_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_regunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_regunet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_remove_repeated_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_remove_repeated_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_remove_small_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_repeat_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_repeat_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_replace_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_require_pkg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_resample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_resample_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_resample_datalist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_resample_to_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_resample_to_matchd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_resampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_resize_with_pad_or_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_resize_with_pad_or_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_resized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7382 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_retinanet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_retinanet_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_retinanet_predict_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rotate90.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rotate90d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_rotated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_safe_dtype_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_saliency_inferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_sample_slices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_sampler_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_save_classificationd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_save_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_save_imaged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_save_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_savitzky_golay_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_savitzky_golay_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_savitzky_golay_smoothd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_scale_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_scale_intensity_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_scale_intensity_range_percentiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_scale_intensity_range_percentilesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_scale_intensity_ranged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_scale_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_se_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_se_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_seg_loss_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_segresnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_segresnet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_segresnet_ds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_select_cross_validation_folds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_select_itemsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_selfattention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_senet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_separable_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_set_determinism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_set_visible_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_shift_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_shift_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_shuffle_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_signal_continuouswavelet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_signal_fillempty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_signal_rand_add_gaussiannoise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_signal_rand_add_sine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_signal_rand_add_sine_partial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_signal_rand_add_squarepulse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_signal_rand_add_squarepulse_partial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_signal_rand_drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_signal_rand_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_signal_rand_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_signal_remove_frequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_simple_aspp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_simulatedelay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_simulatedelayd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_skip_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_slice_inferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10903 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_sliding_patch_wsi_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11961 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_sliding_window_hovernet_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15505 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_sliding_window_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_sliding_window_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7514 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_smartcachedataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_smooth_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_sobel_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_sobel_gradientd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_some_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14525 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_spacing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_spacingd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7930 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_spatial_combine_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_spatial_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_spatial_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_spatial_pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_spatial_padd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_spatial_resample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_spatial_resampled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_split_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_split_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_splitdim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_splitdimd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_squeezedim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_squeezedimd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_ssim_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_ssim_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_state_cacher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_std_shift_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_std_shift_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_str2bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_str2list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_subpixel_upsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18990 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_surface_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_surface_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_swin_unetr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_synthetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_tciadataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_testtimeaugmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_text_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_thread_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_threadcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_threshold_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_threshold_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_timedcall_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_to_contiguous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_to_cupy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_to_cupyd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_to_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_to_deviced.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_to_from_meta_tensord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_to_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_to_numpyd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_to_onehot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_to_pil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_to_pild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_to_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_to_tensord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_torchscript_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_torchvision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_torchvision_fc_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_torchvisiond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_traceable_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_train_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16832 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_trainable_bilateral.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21398 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_trainable_joint_bilateral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_transchex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_transformerblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_transposed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7738 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_tversky_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_unetr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_unetr_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_unified_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_upsample_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_utils_pytorch_numpy_unification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_varautoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_varnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_version_leq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_video_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_vis_cam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_vis_gradbased.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_vis_gradcam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_vitautoenc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_vnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_vote_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_vote_ensembled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_warp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_watershed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_watershedd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_weight_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_weighted_random_sampler_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_with_allow_missing_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_write_metrics_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25914 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_wsireader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_zipdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_zoom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_zoom_affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/tests/test_zoomd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81097 2023-04-23 02:22:42.000000 monai-weekly-1.2.dev2317/versioneer.py
```

### Comparing `monai-weekly-1.2.dev2316/LICENSE` & `monai-weekly-1.2.dev2317/LICENSE`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/PKG-INFO` & `monai-weekly-1.2.dev2317/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monai-weekly
-Version: 1.2.dev2316
+Version: 1.2.dev2317
 Summary: AI Toolkit for Healthcare Imaging
 Home-page: https://monai.io/
 Author: MONAI Consortium
 Author-email: monai.contact@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.monai.io/
 Project-URL: Bug Tracker, https://github.com/Project-MONAI/MONAI/issues
```

### Comparing `monai-weekly-1.2.dev2316/README.md` & `monai-weekly-1.2.dev2317/README.md`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/__init__.py` & `monai-weekly-1.2.dev2317/monai/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,8 +74,8 @@
     "metrics",
     "networks",
     "optimizers",
     "transforms",
     "utils",
     "visualize",
 ]
-__commit_id__ = "b356fecdb265ee9af4ce91a0c8238731994b5095"
+__commit_id__ = "43902e3330da8d879222511131e60f40b38d692e"
```

### Comparing `monai-weekly-1.2.dev2316/monai/_extensions/__init__.py` & `monai-weekly-1.2.dev2317/monai/_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/_extensions/gmm/gmm.cpp` & `monai-weekly-1.2.dev2317/monai/_extensions/gmm/gmm.cpp`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/_extensions/gmm/gmm.h` & `monai-weekly-1.2.dev2317/monai/_extensions/gmm/gmm.h`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/_extensions/gmm/gmm_cpu.cpp` & `monai-weekly-1.2.dev2317/monai/_extensions/gmm/gmm_cpu.cpp`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/_extensions/gmm/gmm_cuda.cu` & `monai-weekly-1.2.dev2317/monai/_extensions/gmm/gmm_cuda.cu`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/_extensions/gmm/gmm_cuda_linalg.cuh` & `monai-weekly-1.2.dev2317/monai/_extensions/gmm/gmm_cuda_linalg.cuh`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/_extensions/loader.py` & `monai-weekly-1.2.dev2317/monai/_extensions/loader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/__init__.py` & `monai-weekly-1.2.dev2317/monai/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/auto3dseg/__init__.py` & `monai-weekly-1.2.dev2317/monai/apps/auto3dseg/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/auto3dseg/__main__.py` & `monai-weekly-1.2.dev2317/monai/apps/auto3dseg/__main__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/auto3dseg/auto_runner.py` & `monai-weekly-1.2.dev2317/monai/apps/auto3dseg/auto_runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,14 +76,16 @@
             is supported
         ensemble: on/off switch to run model ensemble and use the ensemble to predict outputs in testing
             datasets.
         not_use_cache: if the value is True, it will ignore all cached results in data analysis,
             algorithm generation, or training, and start the pipeline from scratch.
         templates_path_or_url: the folder with the algorithm templates or a url. If None provided, the default template
             zip url will be downloaded and extracted into the work_dir.
+        allow_skip: a switch passed to BundleGen process which determines if some Algo in the default templates
+            can be skipped based on the analysis on the dataset from Auto3DSeg DataAnalyzer.
         kwargs: image writing parameters for the ensemble inference. The kwargs format follows the SaveImage
             transform. For more information, check https://docs.monai.io/en/stable/transforms.html#saveimage.
 
 
     Examples:
         - User can use the one-liner to start the Auto3Dseg workflow
 
@@ -210,24 +212,26 @@
         algo_gen: bool | None = None,
         train: bool | None = None,
         hpo: bool = False,
         hpo_backend: str = "nni",
         ensemble: bool = True,
         not_use_cache: bool = False,
         templates_path_or_url: str | None = None,
+        allow_skip: bool = True,
         **kwargs: Any,
     ):
         logger.info(f"AutoRunner using work directory {work_dir}")
         os.makedirs(work_dir, exist_ok=True)
 
         self.work_dir = os.path.abspath(work_dir)
         self.data_src_cfg = dict()
         self.data_src_cfg_name = os.path.join(self.work_dir, "input.yaml")
         self.algos = algos
         self.templates_path_or_url = templates_path_or_url
+        self.allow_skip = allow_skip
         self.kwargs = deepcopy(kwargs)
 
         if input is None and os.path.isfile(self.data_src_cfg_name):
             input = self.data_src_cfg_name
             logger.info(f"Input config is not provided, using the default {input}")
 
         if isinstance(input, dict):
@@ -765,17 +769,18 @@
 
             if self.gpu_customization:
                 bundle_generator.generate(
                     self.work_dir,
                     num_fold=self.num_fold,
                     gpu_customization=self.gpu_customization,
                     gpu_customization_specs=self.gpu_customization_specs,
+                    allow_skip=self.allow_skip,
                 )
             else:
-                bundle_generator.generate(self.work_dir, num_fold=self.num_fold)
+                bundle_generator.generate(self.work_dir, num_fold=self.num_fold, allow_skip=self.allow_skip)
             history = bundle_generator.get_history()
             export_bundle_algo_history(history)
             self.export_cache(algo_gen=True)
         else:
             logger.info("Skipping algorithm generation...")
 
         # step 3: algo training
```

### Comparing `monai-weekly-1.2.dev2316/monai/apps/auto3dseg/bundle_gen.py` & `monai-weekly-1.2.dev2317/monai/apps/auto3dseg/bundle_gen.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 from monai.auto3dseg.algo_gen import Algo, AlgoGen
 from monai.auto3dseg.utils import algo_to_pickle
 from monai.bundle.config_parser import ConfigParser
 from monai.utils import ensure_tuple
 from monai.utils.enums import AlgoKeys
 
 logger = get_logger(module_name=__name__)
-ALGO_HASH = os.environ.get("MONAI_ALGO_HASH", "80c832e")
+ALGO_HASH = os.environ.get("MONAI_ALGO_HASH", "23ea143")
 
 __all__ = ["BundleAlgo", "BundleGen"]
 
 
 class BundleAlgo(Algo):
     """
     An algorithm represented by a set of bundle configurations and scripts.
@@ -170,15 +170,15 @@
         params = deepcopy(train_params)
 
         train_py = os.path.join(self.output_path, "scripts", "train.py")
         config_dir = os.path.join(self.output_path, "configs")
 
         if os.path.isdir(config_dir):
             base_cmd = ""
-            for file in os.listdir(config_dir):
+            for file in sorted(os.listdir(config_dir)):
                 if not (file.endswith("yaml") or file.endswith("json")):
                     continue
                 base_cmd += f"{train_py} run --config_file=" if len(base_cmd) == 0 else ","
                 # Python Fire may be confused by single-quoted WindowsPath
                 config_yaml = Path(os.path.join(config_dir, file)).as_posix()
                 base_cmd += f"'{config_yaml}'"
         cmd: str | None = self.device_setting["CMD_PREFIX"]  # type: ignore
@@ -207,31 +207,44 @@
         """
         Execute the training command with target devices information.
 
         """
         if devices_info:
             warnings.warn(f"input devices_info {devices_info} is deprecated and ignored.")
 
-        logger.info(f"Launching: {cmd}")
         ps_environ = os.environ.copy()
         ps_environ["CUDA_VISIBLE_DEVICES"] = str(self.device_setting["CUDA_VISIBLE_DEVICES"])
         if int(self.device_setting["NUM_NODES"]) > 1:
             if self.device_setting["MN_START_METHOD"] == "bcprun":
-                cmd = f"bcprun -n {self.device_setting['NUM_NODES']} -p {self.device_setting['n_devices']} -c {cmd}"
+                cmd_list = [
+                    "bcprun",
+                    "-n",
+                    str(self.device_setting["NUM_NODES"]),
+                    "-p",
+                    str(self.device_setting["n_devices"]),
+                    "-c",
+                    cmd,
+                ]
             else:
                 raise NotImplementedError(
                     f"{self.device_setting['MN_START_METHOD']} is not supported yet. "
                     "Try modify BundleAlgo._run_cmd for your cluster."
                 )
-        cmd_list = cmd.split()
+        else:
+            cmd_list = cmd.split()
+
         _idx = 0
         for _idx, c in enumerate(cmd_list):
             if "=" not in c:  # remove variable assignments before the command such as "OMP_NUM_THREADS=1"
                 break
-        return subprocess.run(cmd_list[_idx:], env=ps_environ, check=True)
+        cmd_list = cmd_list[_idx:]
+
+        logger.info(f"Launching: {' '.join(cmd_list)}")
+
+        return subprocess.run(cmd_list, env=ps_environ, check=True)
 
     def train(
         self, train_params: None | dict = None, device_setting: None | dict = None
     ) -> subprocess.CompletedProcess:
         """
         Load the run function in the training script of each model. Training parameter is predefined by the
         algo_config.yaml file, which is pre-filled by the fill_template_config function in the same instance.
@@ -507,27 +520,30 @@
 
     def generate(
         self,
         output_folder: str = ".",
         num_fold: int = 5,
         gpu_customization: bool = False,
         gpu_customization_specs: dict[str, Any] | None = None,
+        allow_skip: bool = True,
     ) -> None:
         """
         Generate the bundle scripts/configs for each bundleAlgo
 
         Args:
             output_folder: the output folder to save each algorithm.
             num_fold: the number of cross validation fold.
             gpu_customization: the switch to determine automatically customize/optimize bundle script/config
                 parameters for each bundleAlgo based on gpus. Custom parameters are obtained through dummy
                 training to simulate the actual model training process and hyperparameter optimization (HPO)
                 experiments.
             gpu_customization_specs (optinal): the dictionary to enable users overwrite the HPO settings. user can
                 overwrite part of variables as follows or all of them. The structure is as follows.
+            allow_skip: a switch to determine if some Algo in the default templates can be skipped based on the
+                analysis on the dataset from Auto3DSeg DataAnalyzer.
 
                 .. code-block:: python
 
                     gpu_customization_specs = {
                         'ALOG': {
                             'num_trials': 6,
                             'range_num_images_per_batch': [1, 20],
@@ -549,18 +565,21 @@
             for f_id in ensure_tuple(fold_idx):
                 data_stats = self.get_data_stats()
                 data_src_cfg = self.get_data_src()
                 gen_algo = deepcopy(algo)
                 gen_algo.set_data_stats(data_stats)
                 gen_algo.set_data_source(data_src_cfg)
                 name = f"{gen_algo.name}_{f_id}"
-                skip_bundlegen, skip_info = gen_algo.pre_check_skip_algo()
-                if skip_bundlegen:
-                    logger.info(f"{name} is skipped! {skip_info}")
-                    continue
+
+                if allow_skip:
+                    skip_bundlegen, skip_info = gen_algo.pre_check_skip_algo()
+                    if skip_bundlegen:
+                        logger.info(f"{name} is skipped! {skip_info}")
+                        continue
+
                 if gpu_customization:
                     gen_algo.export_to_disk(
                         output_folder,
                         name,
                         fold=f_id,
                         gpu_customization=True,
                         gpu_customization_specs=gpu_customization_specs,
```

### Comparing `monai-weekly-1.2.dev2316/monai/apps/auto3dseg/data_analyzer.py` & `monai-weekly-1.2.dev2317/monai/apps/auto3dseg/data_analyzer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/auto3dseg/ensemble_builder.py` & `monai-weekly-1.2.dev2317/monai/apps/auto3dseg/ensemble_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 
         if isinstance(data_list_or_path, list):
             self.infer_files = data_list_or_path
         elif isinstance(data_list_or_path, str):
             datalist = ConfigParser.load_config_file(data_list_or_path)
             if data_key in datalist:
                 self.infer_files, _ = datafold_read(datalist=datalist, basedir=dataroot, fold=-1, key=data_key)
-            elif hasattr(self, "rank") and self.rank == 0:  # type: ignore
+            elif hasattr(self, "rank") and self.rank == 0:
                 logger.info(f"Datalist file has no testing key - {data_key}. No data for inference is specified")
 
         else:
             raise ValueError("Unsupported parameter type")
 
     def ensemble_pred(self, preds, sigmoid=False):
         """
@@ -171,16 +171,27 @@
         ):
             preds = []
             for algo in self.algo_ensemble:
                 infer_instance = algo[AlgoKeys.ALGO]
                 pred = infer_instance.predict(predict_files=[file], predict_params=param)
                 preds.append(pred[0])
             if "image_save_func" in param:
-                res = img_saver(self.ensemble_pred(preds, sigmoid=sigmoid))
+                try:
+                    ensemble_preds = self.ensemble_pred(preds, sigmoid=sigmoid)
+                except BaseException:
+                    ensemble_preds = self.ensemble_pred([_.to("cpu") for _ in preds], sigmoid=sigmoid)
+                res = img_saver(ensemble_preds)
+                # res is the path to the saved results
+                if hasattr(res, "meta") and "saved_to" in res.meta.keys():
+                    res = res.meta["saved_to"]
+                else:
+                    warn("Image save path not returned.")
+                    res = None
             else:
+                warn("Prediction returned in list instead of disk, provide image_save_func to avoid out of memory.")
                 res = self.ensemble_pred(preds, sigmoid=sigmoid)
             outputs.append(res)
         return outputs
 
     @abstractmethod
     def collect_algos(self, *args, **kwargs):
         raise NotImplementedError
@@ -447,14 +458,15 @@
         self.save_image = {
             "_target_": "SaveImage",
             "output_dir": output_dir,
             "output_postfix": output_postfix,
             "output_dtype": output_dtype,
             "resample": resample,
             "print_log": False,
+            "savepath_in_metadict": True,
         }
         if kwargs:
             self.save_image.update(kwargs)
 
     def set_num_fold(self, num_fold: int = 5) -> None:
         """
         Set the number of cross validation folds for all algos.
@@ -479,29 +491,31 @@
         self.set_ensemble_method(self.ensemble_method_name, **self.kwargs)
 
         history = import_bundle_algo_history(self.work_dir, only_trained=False)
         history_untrained = [h for h in history if not h[AlgoKeys.IS_TRAINED]]
         if history_untrained:
             if self.rank == 0:
                 warn(
-                    f"Ensembling step will skip {[h['name'] for h in history_untrained]} untrained algos."
+                    f"Ensembling step will skip {[h[AlgoKeys.ID] for h in history_untrained]} untrained algos."
                     "Generally it means these algos did not complete training."
                 )
             history = [h for h in history if h[AlgoKeys.IS_TRAINED]]
         if len(history) == 0:
             raise ValueError(
                 f"Could not find the trained results in {self.work_dir}. "
                 "Possibly the required training step was not completed."
             )
 
         builder = AlgoEnsembleBuilder(history, self.data_src_cfg_name)
         builder.set_ensemble_method(self.ensemble_method)
         self.ensembler = builder.get_ensemble()
         infer_files = self.ensembler.infer_files
-        infer_files = partition_dataset(data=infer_files, shuffle=False, num_partitions=self.world_size)[self.rank]
+        infer_files = partition_dataset(
+            data=infer_files, shuffle=False, num_partitions=self.world_size, even_divisible=True
+        )[self.rank]
         # TO DO: Add some function in ensembler for infer_files update?
         self.ensembler.infer_files = infer_files
         # self.kwargs has poped out args for set_image_save_transform
         # add rank to pred_params
         self.kwargs["rank"] = self.rank
         self.kwargs["image_save_func"] = self.save_image
         if self.rank == 0:
@@ -559,15 +573,26 @@
                 raise NotImplementedError(
                     f"{self.device_setting['MN_START_METHOD']} is not supported yet. "
                     "Try modify EnsembleRunner._create_cmd for your cluster."
                 )
             logger.info(f"Ensembling on {self.device_setting['NUM_NODES']} nodes!")
             cmd = "python " if cmd is None else cmd
             cmd = f"{cmd} -m {base_cmd}"
-            cmd = f"bcprun -n {self.device_setting['NUM_NODES']} -p {self.device_setting['n_devices']} -c {cmd}"
+            cmd_list = [
+                "bcprun",
+                "-n",
+                str(self.device_setting["NUM_NODES"]),
+                "-p",
+                str(self.device_setting["n_devices"]),
+                "-c",
+                cmd,
+            ]
+
         else:
             logger.info(f"Ensembling using {self.device_setting['n_devices']} GPU!")
             if cmd is None:
                 cmd = f"torchrun --nnodes={1:d} --nproc_per_node={self.device_setting['n_devices']:d} "
             cmd = f"{cmd} -m {base_cmd}"
-        _ = subprocess.run(cmd.split(), env=ps_environ, check=True)
+            cmd_list = cmd.split()
+
+        _ = subprocess.run(cmd_list, env=ps_environ, check=True)
         return
```

### Comparing `monai-weekly-1.2.dev2316/monai/apps/auto3dseg/hpo_gen.py` & `monai-weekly-1.2.dev2317/monai/apps/auto3dseg/hpo_gen.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/auto3dseg/transforms.py` & `monai-weekly-1.2.dev2317/monai/apps/auto3dseg/transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/auto3dseg/utils.py` & `monai-weekly-1.2.dev2317/monai/apps/auto3dseg/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,14 +46,20 @@
 
         algo, algo_meta_data = algo_from_pickle(obj_filename, template_path=template_path)
 
         if isinstance(algo, BundleAlgo):  # algo's template path needs override
             algo.template_path = algo_meta_data["template_path"]
 
         best_metric = algo_meta_data.get(AlgoKeys.SCORE, None)
+        if best_metric is None:
+            try:
+                best_metric = algo.get_score()
+            except BaseException:
+                pass
+
         is_trained = best_metric is not None
 
         if (only_trained and is_trained) or not only_trained:
             history.append(
                 {AlgoKeys.ID: name, AlgoKeys.ALGO: algo, AlgoKeys.SCORE: best_metric, AlgoKeys.IS_TRAINED: is_trained}
             )
```

### Comparing `monai-weekly-1.2.dev2316/monai/apps/datasets.py` & `monai-weekly-1.2.dev2317/monai/apps/datasets.py`

 * *Files 1% similar despite different names*

```diff
@@ -582,15 +582,15 @@
         First of all, download a series from TCIA according to `series_uid`.
         Then find all referenced series and download.
         """
         seg_first_dir = os.path.join(download_dir, "raw", series_uid)
         download_tcia_series_instance(
             series_uid=series_uid, download_dir=download_dir, output_dir=seg_first_dir, check_md5=False
         )
-        dicom_files = [f for f in os.listdir(seg_first_dir) if f.endswith(".dcm")]
+        dicom_files = [f for f in sorted(os.listdir(seg_first_dir)) if f.endswith(".dcm")]
         # achieve series number and patient id from the first dicom file
         dcm_path = os.path.join(seg_first_dir, dicom_files[0])
         ds = PydicomReader(stop_before_pixels=True, specific_tags=self.load_tags).read(dcm_path)
         # (0x0010,0x0020) and (0x0010,0x0010), better to be contained in `specific_tags`
         patient_id = ds.PatientID if ds.PatientID else ds.PatientName
         if not patient_id:
             warnings.warn(f"unable to find patient name of dicom file: {dcm_path}, use 'patient' instead.")
```

### Comparing `monai-weekly-1.2.dev2316/monai/apps/deepedit/__init__.py` & `monai-weekly-1.2.dev2317/monai/apps/deepedit/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/deepedit/interaction.py` & `monai-weekly-1.2.dev2317/monai/apps/deepedit/interaction.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/deepedit/transforms.py` & `monai-weekly-1.2.dev2317/monai/apps/deepedit/transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/deepgrow/__init__.py` & `monai-weekly-1.2.dev2317/monai/apps/deepgrow/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/deepgrow/dataset.py` & `monai-weekly-1.2.dev2317/monai/apps/deepgrow/dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/deepgrow/interaction.py` & `monai-weekly-1.2.dev2317/monai/apps/deepgrow/interaction.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/deepgrow/transforms.py` & `monai-weekly-1.2.dev2317/monai/apps/deepgrow/transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/detection/__init__.py` & `monai-weekly-1.2.dev2317/monai/apps/detection/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/detection/metrics/__init__.py` & `monai-weekly-1.2.dev2317/monai/apps/detection/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/detection/metrics/coco.py` & `monai-weekly-1.2.dev2317/monai/apps/detection/metrics/coco.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/detection/metrics/matching.py` & `monai-weekly-1.2.dev2317/monai/apps/detection/metrics/matching.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/detection/networks/__init__.py` & `monai-weekly-1.2.dev2317/monai/apps/detection/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/detection/networks/retinanet_detector.py` & `monai-weekly-1.2.dev2317/monai/apps/detection/networks/retinanet_detector.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,27 +118,31 @@
             - size_divisible (int or Sequence[int]) is the expectation on the input image shape.
               The network needs the input spatial_size to be divisible by size_divisible, length should be 2 or 3.
             - cls_key (str) is the key to represent classification in the output dict.
             - box_reg_key (str) is the key to represent box regression in the output dict.
             - num_anchors (int) is the number of anchor shapes at each location. it should equal to
               ``self.anchor_generator.num_anchors_per_location()[0]``.
 
+            If network does not have these attributes, user needs to provide them for the detector.
+
         2. Its input should be an image Tensor sized (B, C, H, W) or (B, C, H, W, D).
 
-        3. About its output ``head_outputs``:
+        3. About its output ``head_outputs``, it should be either a list of tensors or a dictionary of str: List[Tensor]:
 
-            - It should be a dictionary with at least two keys:
-              ``network.cls_key`` and ``network.box_reg_key``.
-            - ``head_outputs[network.cls_key]`` should be List[Tensor] or Tensor. Each Tensor represents
+            - If it is a dictionary, it needs to have at least two keys:
+              ``network.cls_key`` and ``network.box_reg_key``, representing predicted classification maps and box regression maps.
+              ``head_outputs[network.cls_key]`` should be List[Tensor] or Tensor. Each Tensor represents
               classification logits map at one resolution level,
               sized (B, num_classes*num_anchors, H_i, W_i) or (B, num_classes*num_anchors, H_i, W_i, D_i).
-            - ``head_outputs[network.box_reg_key]`` should be List[Tensor] or Tensor. Each Tensor represents
+              ``head_outputs[network.box_reg_key]`` should be List[Tensor] or Tensor. Each Tensor represents
               box regression map at one resolution level,
               sized (B, 2*spatial_dims*num_anchors, H_i, W_i)or (B, 2*spatial_dims*num_anchors, H_i, W_i, D_i).
-            - ``len(head_outputs[network.cls_key]) == len(head_outputs[network.box_reg_key])``.
+              ``len(head_outputs[network.cls_key]) == len(head_outputs[network.box_reg_key])``.
+            - If it is a list of 2N tensors, the first N tensors should be the predicted classification maps,
+              and the second N tensors should be the predicted box regression maps.
 
     Example:
 
         .. code-block:: python
 
             # define a naive network
             import torch
@@ -180,42 +184,41 @@
     """
 
     def __init__(
         self,
         network: nn.Module,
         anchor_generator: AnchorGenerator,
         box_overlap_metric: Callable = box_iou,
+        spatial_dims: int | None = None,  # used only when network.spatial_dims does not exist
+        num_classes: int | None = None,  # used only when network.num_classes does not exist
+        size_divisible: Sequence[int] | int = 1,  # used only when network.size_divisible does not exist
+        cls_key: str = "classification",  # used only when network.cls_key does not exist
+        box_reg_key: str = "box_regression",  # used only when network.box_reg_key does not exist
         debug: bool = False,
     ):
         super().__init__()
 
-        if not all(
-            hasattr(network, attr)
-            for attr in ["spatial_dims", "num_classes", "cls_key", "box_reg_key", "num_anchors", "size_divisible"]
-        ):
-            raise AttributeError(
-                "network should have attributes, including: "
-                "'spatial_dims', 'num_classes', 'cls_key', 'box_reg_key', 'num_anchors', 'size_divisible'."
-            )
-
         self.network = network
-        self.spatial_dims: int = self.network.spatial_dims  # type: ignore[assignment]
-        self.num_classes = self.network.num_classes
-        self.size_divisible = ensure_tuple_rep(self.network.size_divisible, self.spatial_dims)
+        # network attribute
+        self.spatial_dims = self.get_attribute_from_network("spatial_dims", default_value=spatial_dims)
+        self.num_classes = self.get_attribute_from_network("num_classes", default_value=num_classes)
+
+        self.size_divisible = self.get_attribute_from_network("size_divisible", default_value=size_divisible)
+        self.size_divisible = ensure_tuple_rep(self.size_divisible, self.spatial_dims)
         # keys for the network output
-        self.cls_key: str = self.network.cls_key  # type: ignore[assignment]
-        self.box_reg_key: str = self.network.box_reg_key  # type: ignore[assignment]
+        self.cls_key = self.get_attribute_from_network("cls_key", default_value=cls_key)
+        self.box_reg_key = self.get_attribute_from_network("box_reg_key", default_value=box_reg_key)
 
         # check if anchor_generator matches with network
         self.anchor_generator = anchor_generator
-
         self.num_anchors_per_loc = self.anchor_generator.num_anchors_per_location()[0]
-        if self.num_anchors_per_loc != self.network.num_anchors:
+        network_num_anchors = self.get_attribute_from_network("num_anchors", default_value=self.num_anchors_per_loc)
+        if self.num_anchors_per_loc != network_num_anchors:
             raise ValueError(
-                f"Number of feature map channels ({self.network.num_anchors}) "
+                f"Number of feature map channels ({network_num_anchors}) "
                 f"should match with number of anchors at each location ({self.num_anchors_per_loc})."
             )
         # if new coming input images has same shape with
         # self.previous_image_shape, there is no need to generate new anchors.
         self.anchors: list[Tensor] | None = None
         self.previous_image_shape: Any | None = None
 
@@ -248,14 +251,22 @@
             score_thresh=0.05,
             topk_candidates_per_level=1000,
             nms_thresh=0.5,
             detections_per_img=300,
             apply_sigmoid=True,
         )
 
+    def get_attribute_from_network(self, attr_name, default_value=None):
+        if hasattr(self.network, attr_name):
+            return getattr(self.network, attr_name)
+        elif default_value is not None:
+            return default_value
+        else:
+            raise ValueError(f"network does not have attribute {attr_name}, please provide it in the detector.")
+
     def set_box_coder_weights(self, weights: tuple[float]) -> None:
         """
         Set the weights for box coder.
 
         Args:
             weights: a list/tuple with length of 2*self.spatial_dims
 
@@ -493,15 +504,22 @@
         # 2. Pad list of images to a single Tensor `images` with spatial size divisible by self.size_divisible.
         # image_sizes stores the original spatial_size of each image before padding.
         images, image_sizes = preprocess_images(input_images, self.spatial_dims, self.size_divisible)
 
         # 3. Generate network outputs. Use inferer only in evaluation mode.
         if self.training or (not use_inferer):
             head_outputs = self.network(images)
-            ensure_dict_value_to_list_(head_outputs)  # ensure head_outputs is Dict[str, List[Tensor]]
+            if isinstance(head_outputs, (tuple, list)):
+                tmp_dict = {}
+                tmp_dict[self.cls_key] = head_outputs[: len(head_outputs) // 2]
+                tmp_dict[self.box_reg_key] = head_outputs[len(head_outputs) // 2 :]
+                head_outputs = tmp_dict
+            else:
+                # ensure head_outputs is Dict[str, List[Tensor]]
+                ensure_dict_value_to_list_(head_outputs)
         else:
             if self.inferer is None:
                 raise ValueError(
                     "`self.inferer` is not defined." "Please refer to function self.set_sliding_window_inferer(*)."
                 )
             head_outputs = predict_with_inferer(
                 images, self.network, keys=[self.cls_key, self.box_reg_key], inferer=self.inferer
```

### Comparing `monai-weekly-1.2.dev2316/monai/apps/detection/networks/retinanet_network.py` & `monai-weekly-1.2.dev2317/monai/apps/detection/networks/retinanet_network.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 https://github.com/pytorch/vision/blob/main/torchvision/models/detection/retinanet.py
 """
 
 from __future__ import annotations
 
 import math
 from collections.abc import Callable, Sequence
-from typing import Dict
+from typing import Any, Dict
 
 import torch
 from torch import Tensor, nn
 
 from monai.networks.blocks.backbone_fpn_utils import BackboneWithFPN, _resnet_fpn_extractor
 from monai.networks.layers.factories import Conv
 from monai.networks.nets import resnet
@@ -199,28 +199,35 @@
         return box_regression_maps
 
 
 class RetinaNet(nn.Module):
     """
     The network used in RetinaNet.
 
-    It takes an image tensor as inputs, and outputs a dictionary ``head_outputs``.
+    It takes an image tensor as inputs, and outputs either 1) a dictionary ``head_outputs``.
     ``head_outputs[self.cls_key]`` is the predicted classification maps, a list of Tensor.
     ``head_outputs[self.box_reg_key]`` is the predicted box regression maps, a list of Tensor.
+    or 2) a list of 2N tensors ``head_outputs``, with first N tensors being the predicted
+    classification maps and second N tensors being the predicted box regression maps.
 
     Args:
         spatial_dims: number of spatial dimensions of the images. We support both 2D and 3D images.
         num_classes: number of output classes of the model (excluding the background).
         num_anchors: number of anchors at each location.
         feature_extractor: a network that outputs feature maps from the input images,
             each feature map corresponds to a different resolution.
             Its output can have a format of Tensor, Dict[Any, Tensor], or Sequence[Tensor].
             It can be the output of ``resnet_fpn_feature_extractor(*args, **kwargs)``.
         size_divisible: the spatial size of the network input should be divisible by size_divisible,
             decided by the feature_extractor.
+        use_list_output: default False. If False, the network outputs a dictionary ``head_outputs``,
+            ``head_outputs[self.cls_key]`` is the predicted classification maps, a list of Tensor.
+            ``head_outputs[self.box_reg_key]`` is the predicted box regression maps, a list of Tensor.
+            If True, the network outputs a list of 2N tensors ``head_outputs``, with first N tensors being
+            the predicted classification maps and second N tensors being the predicted box regression maps.
 
     Example:
 
         .. code-block:: python
 
             from monai.networks.nets import resnet
             spatial_dims = 3  # 3D network
@@ -251,31 +258,33 @@
                 spatial_dims = spatial_dims,
                 num_classes = 5,
                 num_anchors = 6,
                 feature_extractor=feature_extractor,
                 size_divisible = size_divisible,
             ).to(device)
             result = model(torch.rand(2, 1, 128,128,128))
-            cls_logits_maps = result["cls_logits"]  # a list of len(returned_layers)+1 Tensor
+            cls_logits_maps = result["classification"]  # a list of len(returned_layers)+1 Tensor
             box_regression_maps = result["box_regression"]  # a list of len(returned_layers)+1 Tensor
     """
 
     def __init__(
         self,
         spatial_dims: int,
         num_classes: int,
         num_anchors: int,
         feature_extractor: nn.Module,
         size_divisible: Sequence[int] | int = 1,
+        use_list_output: bool = False,
     ):
         super().__init__()
 
         self.spatial_dims = look_up_option(spatial_dims, supported=[1, 2, 3])
         self.num_classes = num_classes
         self.size_divisible = ensure_tuple_rep(size_divisible, self.spatial_dims)
+        self.use_list_output = use_list_output
 
         if not hasattr(feature_extractor, "out_channels"):
             raise ValueError(
                 "feature_extractor should contain an attribute out_channels "
                 "specifying the number of output channels (assumed to be the "
                 "same for all the levels)"
             )
@@ -289,27 +298,29 @@
         self.regression_head = RetinaNetRegressionHead(
             self.feature_map_channels, self.num_anchors, spatial_dims=self.spatial_dims
         )
 
         self.cls_key: str = "classification"
         self.box_reg_key: str = "box_regression"
 
-    def forward(self, images: Tensor) -> dict[str, list[Tensor]]:
+    def forward(self, images: Tensor) -> Any:
         """
-        It takes an image tensor as inputs, and outputs a dictionary ``head_outputs``.
-        ``head_outputs[self.cls_key]`` is the predicted classification maps, a list of Tensor.
-        ``head_outputs[self.box_reg_key]`` is the predicted box regression maps, a list of Tensor.
+        It takes an image tensor as inputs, and outputs predicted classification maps
+        and predicted box regression maps in ``head_outputs``.
 
         Args:
             images: input images, sized (B, img_channels, H, W) or (B, img_channels, H, W, D).
 
         Return:
-            a dictionary ``head_outputs`` with keys including self.cls_key and self.box_reg_key.
+            1) If self.use_list_output is False, output a dictionary ``head_outputs`` with
+            keys including self.cls_key and self.box_reg_key.
             ``head_outputs[self.cls_key]`` is the predicted classification maps, a list of Tensor.
             ``head_outputs[self.box_reg_key]`` is the predicted box regression maps, a list of Tensor.
+            2) if self.use_list_output is True, outputs a list of 2N tensors ``head_outputs``, with first N tensors being
+            the predicted classification maps and second N tensors being the predicted box regression maps.
 
         """
         # compute features maps list from the input images.
         features = self.feature_extractor(images)
         if isinstance(features, Tensor):
             feature_maps = [features]
         elif torch.jit.isinstance(features, Dict[str, Tensor]):
@@ -319,18 +330,23 @@
 
         if not isinstance(feature_maps[0], Tensor):
             raise ValueError("feature_extractor output format must be Tensor, Dict[str, Tensor], or Sequence[Tensor].")
 
         # compute classification and box regression maps from the feature maps
         # expandable for mask prediction in the future
 
-        head_outputs: dict[str, list[Tensor]] = {self.cls_key: self.classification_head(feature_maps)}
-        head_outputs[self.box_reg_key] = self.regression_head(feature_maps)
-
-        return head_outputs
+        if not self.use_list_output:
+            # output dict
+            head_outputs = {self.cls_key: self.classification_head(feature_maps)}
+            head_outputs[self.box_reg_key] = self.regression_head(feature_maps)
+            return head_outputs
+        else:
+            # output list of tensor, first half is classification, second half is box regression
+            head_outputs_sequence = self.classification_head(feature_maps) + self.regression_head(feature_maps)
+            return head_outputs_sequence
 
 
 def resnet_fpn_feature_extractor(
     backbone: resnet.ResNet,
     spatial_dims: int,
     pretrained_backbone: bool = False,
     returned_layers: Sequence[int] = (1, 2, 3),
```

### Comparing `monai-weekly-1.2.dev2316/monai/apps/detection/transforms/__init__.py` & `monai-weekly-1.2.dev2317/monai/apps/detection/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/detection/transforms/array.py` & `monai-weekly-1.2.dev2317/monai/apps/detection/transforms/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/detection/transforms/box_ops.py` & `monai-weekly-1.2.dev2317/monai/apps/detection/transforms/box_ops.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,20 +17,18 @@
 import numpy as np
 import torch
 
 from monai.config.type_definitions import DtypeLike, NdarrayOrTensor, NdarrayTensor
 from monai.data.box_utils import COMPUTE_DTYPE, TO_REMOVE, get_spatial_dims
 from monai.transforms import Resize
 from monai.transforms.utils import create_scale
-from monai.utils import look_up_option, optional_import
+from monai.utils import look_up_option
 from monai.utils.misc import ensure_tuple, ensure_tuple_rep
 from monai.utils.type_conversion import convert_data_type, convert_to_dst_type
 
-scipy, _ = optional_import("scipy")
-
 
 def _apply_affine_to_points(points: torch.Tensor, affine: torch.Tensor, include_shift: bool = True) -> torch.Tensor:
     """
     This internal function applies affine matrices to the point coordinate
 
     Args:
         points: point coordinates, Nx2 or Nx3 torch tensor or ndarray, representing [x, y] or [x, y, z]
```

### Comparing `monai-weekly-1.2.dev2316/monai/apps/detection/transforms/dictionary.py` & `monai-weekly-1.2.dev2317/monai/apps/detection/transforms/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/detection/utils/ATSS_matcher.py` & `monai-weekly-1.2.dev2317/monai/apps/detection/utils/ATSS_matcher.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/detection/utils/__init__.py` & `monai-weekly-1.2.dev2317/monai/apps/detection/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/detection/utils/anchor_utils.py` & `monai-weekly-1.2.dev2317/monai/apps/detection/utils/anchor_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/detection/utils/box_coder.py` & `monai-weekly-1.2.dev2317/monai/apps/detection/utils/box_coder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/detection/utils/box_selector.py` & `monai-weekly-1.2.dev2317/monai/apps/detection/utils/box_selector.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/detection/utils/detector_utils.py` & `monai-weekly-1.2.dev2317/monai/apps/detection/utils/detector_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/detection/utils/hard_negative_sampler.py` & `monai-weekly-1.2.dev2317/monai/apps/detection/utils/hard_negative_sampler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/detection/utils/predict_utils.py` & `monai-weekly-1.2.dev2317/monai/apps/detection/utils/predict_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,14 +69,20 @@
         keys: the keys in the network output whose values will be output in this func.
             If not provided, will use all keys.
 
     Return:
         network output values concat to a single List[Tensor]
     """
     head_outputs = network(images)
+
+    # if head_outputs is already a sequence of tensors, directly output it
+    if isinstance(head_outputs, (tuple, list)):
+        return list(head_outputs)
+
+    # if head_outputs is a dict
     ensure_dict_value_to_list_(head_outputs, keys)
     if keys is None:
         keys = list(head_outputs.keys())
     check_dict_values_same_length(head_outputs, keys)
     head_outputs_sequence = []
     for k in keys:
         head_outputs_sequence += list(head_outputs[k])
```

### Comparing `monai-weekly-1.2.dev2316/monai/apps/mmars/__init__.py` & `monai-weekly-1.2.dev2317/monai/apps/mmars/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/mmars/mmars.py` & `monai-weekly-1.2.dev2317/monai/apps/mmars/mmars.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/mmars/model_desc.py` & `monai-weekly-1.2.dev2317/monai/apps/mmars/model_desc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/nnunet/__init__.py` & `monai-weekly-1.2.dev2317/monai/apps/nnunet/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/nnunet/__main__.py` & `monai-weekly-1.2.dev2317/monai/apps/nnunet/__main__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/nnunet/nnunetv2_runner.py` & `monai-weekly-1.2.dev2317/monai/apps/nnunet/nnunetv2_runner.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/nnunet/utils.py` & `monai-weekly-1.2.dev2317/monai/apps/nnunet/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/nuclick/__init__.py` & `monai-weekly-1.2.dev2317/monai/apps/nuclick/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/nuclick/transforms.py` & `monai-weekly-1.2.dev2317/monai/apps/nuclick/transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/pathology/__init__.py` & `monai-weekly-1.2.dev2317/monai/apps/pathology/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/pathology/engines/__init__.py` & `monai-weekly-1.2.dev2317/monai/apps/pathology/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/pathology/engines/utils.py` & `monai-weekly-1.2.dev2317/monai/apps/pathology/engines/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/pathology/handlers/__init__.py` & `monai-weekly-1.2.dev2317/monai/apps/pathology/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/pathology/handlers/utils.py` & `monai-weekly-1.2.dev2317/monai/apps/pathology/handlers/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/pathology/inferers/__init__.py` & `monai-weekly-1.2.dev2317/monai/apps/pathology/inferers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/pathology/inferers/inferer.py` & `monai-weekly-1.2.dev2317/monai/apps/pathology/inferers/inferer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/pathology/losses/__init__.py` & `monai-weekly-1.2.dev2317/monai/apps/pathology/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/pathology/losses/hovernet_loss.py` & `monai-weekly-1.2.dev2317/monai/apps/pathology/losses/hovernet_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/pathology/metrics/__init__.py` & `monai-weekly-1.2.dev2317/monai/apps/pathology/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/pathology/metrics/lesion_froc.py` & `monai-weekly-1.2.dev2317/monai/apps/pathology/metrics/lesion_froc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/pathology/transforms/__init__.py` & `monai-weekly-1.2.dev2317/monai/apps/pathology/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/pathology/transforms/post/__init__.py` & `monai-weekly-1.2.dev2317/monai/apps/pathology/transforms/post/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/pathology/transforms/post/array.py` & `monai-weekly-1.2.dev2317/monai/apps/pathology/transforms/post/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/pathology/transforms/post/dictionary.py` & `monai-weekly-1.2.dev2317/monai/apps/pathology/transforms/post/dictionary.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 )
 from monai.config.type_definitions import DtypeLike, KeysCollection, NdarrayOrTensor
 from monai.transforms.transform import MapTransform, Transform
 from monai.utils import optional_import
 from monai.utils.enums import HoVerNetBranch
 
 find_contours, _ = optional_import("skimage.measure", name="find_contours")
-moments, _ = optional_import("skimage.measure", name="moments")
 
 __all__ = [
     "WatershedD",
     "WatershedDict",
     "Watershedd",
     "GenerateWatershedMaskD",
     "GenerateWatershedMaskDict",
```

### Comparing `monai-weekly-1.2.dev2316/monai/apps/pathology/transforms/stain/__init__.py` & `monai-weekly-1.2.dev2317/monai/apps/pathology/transforms/stain/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/pathology/transforms/stain/array.py` & `monai-weekly-1.2.dev2317/monai/apps/pathology/transforms/stain/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/pathology/transforms/stain/dictionary.py` & `monai-weekly-1.2.dev2317/monai/apps/pathology/transforms/stain/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/pathology/utils.py` & `monai-weekly-1.2.dev2317/monai/apps/pathology/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/reconstruction/__init__.py` & `monai-weekly-1.2.dev2317/monai/apps/reconstruction/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/reconstruction/complex_utils.py` & `monai-weekly-1.2.dev2317/monai/apps/reconstruction/complex_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/reconstruction/fastmri_reader.py` & `monai-weekly-1.2.dev2317/monai/apps/reconstruction/fastmri_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/reconstruction/mri_utils.py` & `monai-weekly-1.2.dev2317/monai/apps/reconstruction/mri_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/reconstruction/networks/__init__.py` & `monai-weekly-1.2.dev2317/monai/apps/reconstruction/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/reconstruction/networks/blocks/__init__.py` & `monai-weekly-1.2.dev2317/monai/apps/reconstruction/networks/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/reconstruction/networks/blocks/varnetblock.py` & `monai-weekly-1.2.dev2317/monai/apps/reconstruction/networks/blocks/varnetblock.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/reconstruction/networks/nets/__init__.py` & `monai-weekly-1.2.dev2317/monai/apps/reconstruction/networks/nets/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/reconstruction/networks/nets/coil_sensitivity_model.py` & `monai-weekly-1.2.dev2317/monai/apps/reconstruction/networks/nets/coil_sensitivity_model.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/reconstruction/networks/nets/complex_unet.py` & `monai-weekly-1.2.dev2317/monai/apps/reconstruction/networks/nets/complex_unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/reconstruction/networks/nets/utils.py` & `monai-weekly-1.2.dev2317/monai/apps/reconstruction/networks/nets/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/reconstruction/networks/nets/varnet.py` & `monai-weekly-1.2.dev2317/monai/apps/reconstruction/networks/nets/varnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/reconstruction/transforms/__init__.py` & `monai-weekly-1.2.dev2317/monai/apps/reconstruction/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/reconstruction/transforms/array.py` & `monai-weekly-1.2.dev2317/monai/apps/reconstruction/transforms/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/reconstruction/transforms/dictionary.py` & `monai-weekly-1.2.dev2317/monai/apps/reconstruction/transforms/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/tcia/__init__.py` & `monai-weekly-1.2.dev2317/monai/apps/tcia/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/tcia/label_desc.py` & `monai-weekly-1.2.dev2317/monai/apps/tcia/label_desc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/tcia/utils.py` & `monai-weekly-1.2.dev2317/monai/apps/tcia/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/apps/utils.py` & `monai-weekly-1.2.dev2317/monai/apps/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/auto3dseg/__init__.py` & `monai-weekly-1.2.dev2317/monai/auto3dseg/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/auto3dseg/algo_gen.py` & `monai-weekly-1.2.dev2317/monai/auto3dseg/algo_gen.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/auto3dseg/analyzer.py` & `monai-weekly-1.2.dev2317/monai/auto3dseg/analyzer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/auto3dseg/operations.py` & `monai-weekly-1.2.dev2317/monai/auto3dseg/operations.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/auto3dseg/seg_summarizer.py` & `monai-weekly-1.2.dev2317/monai/auto3dseg/seg_summarizer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/auto3dseg/utils.py` & `monai-weekly-1.2.dev2317/monai/auto3dseg/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/bundle/__init__.py` & `monai-weekly-1.2.dev2317/monai/bundle/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/bundle/__main__.py` & `monai-weekly-1.2.dev2317/monai/bundle/__main__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/bundle/config_item.py` & `monai-weekly-1.2.dev2317/monai/bundle/config_item.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/bundle/config_parser.py` & `monai-weekly-1.2.dev2317/monai/bundle/config_parser.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/bundle/properties.py` & `monai-weekly-1.2.dev2317/monai/bundle/properties.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,14 +155,19 @@
         BundlePropertyConfig.ID: "bundle_root",
     },
     "device": {
         BundleProperty.DESC: "target device to execute the bundle workflow.",
         BundleProperty.REQUIRED: True,
         BundlePropertyConfig.ID: "device",
     },
+    "evaluator": {
+        BundleProperty.DESC: "inference / evaluation workflow engine.",
+        BundleProperty.REQUIRED: True,
+        BundlePropertyConfig.ID: "evaluator",
+    },
     "network_def": {
         BundleProperty.DESC: "network module for the inference.",
         BundleProperty.REQUIRED: True,
         BundlePropertyConfig.ID: "network_def",
     },
     "inferer": {
         BundleProperty.DESC: "MONAI Inferer object to execute the model computation in inference.",
```

### Comparing `monai-weekly-1.2.dev2316/monai/bundle/reference_resolver.py` & `monai-weekly-1.2.dev2317/monai/bundle/reference_resolver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/bundle/scripts.py` & `monai-weekly-1.2.dev2317/monai/bundle/scripts.py`

 * *Files 0% similar despite different names*

```diff
@@ -621,16 +621,19 @@
 
         # Set default args of `run` in a JSON / YAML file, help to record and simplify the command line.
         # Other args still can override the default args at runtime:
         python -m monai.bundle run --args_file "/workspace/data/args.json" --config_file <config path>
 
     Args:
         run_id: ID name of the expected config expression to run, default to "run".
+            to run the config, the target config must contain this ID.
         init_id: ID name of the expected config expression to initialize before running, default to "initialize".
+            it's optional for both configs and this `run` function.
         final_id: ID name of the expected config expression to finalize after running, default to "finalize".
+            it's optional for both configs and this `run` function.
         meta_file: filepath of the metadata file, if it is a list of file paths, the content of them will be merged.
             Default to "configs/metadata.json", which is commonly used for bundles in MONAI model zoo.
         config_file: filepath of the config file, if `None`, must be provided in `args_file`.
             if it is a list of file paths, the content of them will be merged.
         logging_file: config file for `logging` module in the program. for more details:
             https://docs.python.org/3/library/logging.config.html#logging.config.fileConfig.
             Default to "configs/logging.conf", which is commonly used for bundles in MONAI model zoo.
```

### Comparing `monai-weekly-1.2.dev2316/monai/bundle/utils.py` & `monai-weekly-1.2.dev2317/monai/bundle/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/bundle/workflows.py` & `monai-weekly-1.2.dev2317/monai/bundle/workflows.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,23 +40,26 @@
         workflow: specifies the workflow type: "train" or "training" for a training workflow,
             or "infer", "inference", "eval", "evaluation" for a inference workflow,
             other unsupported string will raise a ValueError.
             default to `None` for common workflow.
 
     """
 
+    supported_train_type: tuple = ("train", "training")
+    supported_infer_type: tuple = ("infer", "inference", "eval", "evaluation")
+
     def __init__(self, workflow: str | None = None):
         if workflow is None:
             self.properties = None
             self.workflow = None
             return
-        if workflow.lower() in ("train", "training"):
+        if workflow.lower() in self.supported_train_type:
             self.properties = TrainProperties
             self.workflow = "train"
-        elif workflow.lower() in ("infer", "inference", "eval", "evaluation"):
+        elif workflow.lower() in self.supported_infer_type:
             self.properties = InferProperties
             self.workflow = "infer"
         else:
             raise ValueError(f"Unsupported workflow type: '{workflow}'.")
 
     @abstractmethod
     def initialize(self, *args: Any, **kwargs: Any) -> Any:
@@ -141,16 +144,19 @@
     """
     Specification for the config-based bundle workflow.
     Standardized the `initialize`, `run`, `finalize` behavior in a config-based training, evaluation, or inference.
     For more information: https://docs.monai.io/en/latest/mb_specification.html.
 
     Args:
         run_id: ID name of the expected config expression to run, default to "run".
+            to run the config, the target config must contain this ID.
         init_id: ID name of the expected config expression to initialize before running, default to "initialize".
+            allow a config to have no `initialize` logic and the ID.
         final_id: ID name of the expected config expression to finalize after running, default to "finalize".
+            allow a config to have no `finalize` logic and the ID.
         meta_file: filepath of the metadata file, if it is a list of file paths, the content of them will be merged.
             Default to "configs/metadata.json", which is commonly used for bundles in MONAI model zoo.
         config_file: filepath of the config file, if it is a list of file paths, the content of them will be merged.
         logging_file: config file for `logging` module in the program. for more details:
             https://docs.python.org/3/library/logging.config.html#logging.config.fileConfig.
             Default to "configs/logging.conf", which is commonly used for bundles in MONAI model zoo.
         tracking: if not None, enable the experiment tracking at runtime with optionally configurable and extensible.
@@ -175,15 +181,15 @@
         meta_file: str | Sequence[str] | None = "configs/metadata.json",
         logging_file: str | None = "configs/logging.conf",
         init_id: str = "initialize",
         run_id: str = "run",
         final_id: str = "finalize",
         tracking: str | dict | None = None,
         workflow: str | None = None,
-        **override: dict,
+        **override: Any,
     ) -> None:
         super().__init__(workflow=workflow)
         if logging_file is not None:
             if not os.path.exists(logging_file):
                 if logging_file == "configs/logging.conf":
                     warnings.warn("Default logging file in 'configs/logging.conf' does not exist, skipping logging.")
                 else:
@@ -211,29 +217,33 @@
         # set tracking configs for experiment management
         if tracking is not None:
             if isinstance(tracking, str) and tracking in DEFAULT_EXP_MGMT_SETTINGS:
                 settings_ = DEFAULT_EXP_MGMT_SETTINGS[tracking]
             else:
                 settings_ = ConfigParser.load_config_files(tracking)
             self.patch_bundle_tracking(parser=self.parser, settings=settings_)
+        self._is_initialized: bool = False
 
     def initialize(self) -> Any:
         """
         Initialize the bundle workflow before running.
 
         """
         # reset the "reference_resolver" buffer at initialization stage
         self.parser.parse(reset=True)
+        self._is_initialized = True
         return self._run_expr(id=self.init_id)
 
     def run(self) -> Any:
         """
         Run the bundle workflow, it can be a training, evaluation or inference.
 
         """
+        if self.run_id not in self.parser:
+            raise ValueError(f"run ID '{self.run_id}' doesn't exist in the config file.")
         return self._run_expr(id=self.run_id)
 
     def finalize(self) -> Any:
         """
         Finalize step after the running of bundle workflow.
 
         """
@@ -280,15 +290,15 @@
         With specified property name and information, get the parsed property value from config.
 
         Args:
             name: the name of target property.
             property: other information for the target property, defined in `TrainProperties` or `InferProperties`.
 
         """
-        if not self.parser.ref_resolver.is_resolved():
+        if not self._is_initialized:
             raise RuntimeError("Please execute 'initialize' before getting any parsed content.")
         prop_id = self._get_prop_id(name, property)
         return self.parser.get_parsed_content(id=prop_id) if prop_id is not None else None
 
     def _set_property(self, name: str, property: dict, value: Any) -> None:
         """
         With specified property name and information, set value for the expected property.
@@ -299,14 +309,15 @@
             value: value to set for the property.
 
         """
         prop_id = self._get_prop_id(name, property)
         if prop_id is not None:
             self.parser[prop_id] = value
             # must parse the config again after changing the content
+            self._is_initialized = False
             self.parser.ref_resolver.reset()
 
     def _check_optional_id(self, name: str, property: dict) -> bool:
         """
         If an optional property has reference in the config, check whether the property is existing.
         If `ValidationHandler` is defined for a training workflow, will check whether the optional properties
         "evaluator" and "val_interval" are existing.
```

### Comparing `monai-weekly-1.2.dev2316/monai/config/__init__.py` & `monai-weekly-1.2.dev2317/monai/config/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/config/deviceconfig.py` & `monai-weekly-1.2.dev2317/monai/config/deviceconfig.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/config/type_definitions.py` & `monai-weekly-1.2.dev2317/monai/config/type_definitions.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/data/__init__.py` & `monai-weekly-1.2.dev2317/monai/data/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/data/box_utils.py` & `monai-weekly-1.2.dev2317/monai/data/box_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/data/csv_saver.py` & `monai-weekly-1.2.dev2317/monai/data/csv_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/data/dataloader.py` & `monai-weekly-1.2.dev2317/monai/data/dataloader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/data/dataset.py` & `monai-weekly-1.2.dev2317/monai/data/dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/data/dataset_summary.py` & `monai-weekly-1.2.dev2317/monai/data/dataset_summary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/data/decathlon_datalist.py` & `monai-weekly-1.2.dev2317/monai/data/decathlon_datalist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/data/fft_utils.py` & `monai-weekly-1.2.dev2317/monai/data/fft_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/data/folder_layout.py` & `monai-weekly-1.2.dev2317/monai/data/folder_layout.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/data/grid_dataset.py` & `monai-weekly-1.2.dev2317/monai/data/grid_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/data/image_dataset.py` & `monai-weekly-1.2.dev2317/monai/data/image_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/data/image_reader.py` & `monai-weekly-1.2.dev2317/monai/data/image_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/data/image_writer.py` & `monai-weekly-1.2.dev2317/monai/data/image_writer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/data/iterable_dataset.py` & `monai-weekly-1.2.dev2317/monai/data/iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/data/itk_torch_bridge.py` & `monai-weekly-1.2.dev2317/monai/data/itk_torch_bridge.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/data/meta_obj.py` & `monai-weekly-1.2.dev2317/monai/data/meta_obj.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/data/meta_tensor.py` & `monai-weekly-1.2.dev2317/monai/data/meta_tensor.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/data/samplers.py` & `monai-weekly-1.2.dev2317/monai/data/samplers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/data/synthetic.py` & `monai-weekly-1.2.dev2317/monai/data/synthetic.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/data/test_time_augmentation.py` & `monai-weekly-1.2.dev2317/monai/data/test_time_augmentation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/data/thread_buffer.py` & `monai-weekly-1.2.dev2317/monai/data/thread_buffer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/data/torchscript_utils.py` & `monai-weekly-1.2.dev2317/monai/data/torchscript_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/data/utils.py` & `monai-weekly-1.2.dev2317/monai/data/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/data/video_dataset.py` & `monai-weekly-1.2.dev2317/monai/data/video_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/data/wsi_datasets.py` & `monai-weekly-1.2.dev2317/monai/data/wsi_datasets.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,16 +56,16 @@
 
     Note:
         The input data has the following form as an example:
 
         .. code-block:: python
 
             [
-                {"image": "path/to/image1.tiff", "patch_location": [200, 500], "label": 0},
-                {"image": "path/to/image2.tiff", "patch_location": [100, 700], "patch_size": [20, 20], "patch_level": 2, "label": 1}
+                {"image": "path/to/image1.tiff", "location": [200, 500], "label": 0},
+                {"image": "path/to/image2.tiff", "location": [100, 700], "patch_size": [20, 20], "patch_level": 2, "label": 1}
             ]
 
     """
 
     def __init__(
         self,
         data: Sequence,
```

### Comparing `monai-weekly-1.2.dev2316/monai/data/wsi_reader.py` & `monai-weekly-1.2.dev2317/monai/data/wsi_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/engines/__init__.py` & `monai-weekly-1.2.dev2317/monai/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/engines/evaluator.py` & `monai-weekly-1.2.dev2317/monai/engines/evaluator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/engines/multi_gpu_supervised_trainer.py` & `monai-weekly-1.2.dev2317/monai/engines/multi_gpu_supervised_trainer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/engines/trainer.py` & `monai-weekly-1.2.dev2317/monai/engines/trainer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/engines/utils.py` & `monai-weekly-1.2.dev2317/monai/engines/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/engines/workflow.py` & `monai-weekly-1.2.dev2317/monai/engines/workflow.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/fl/__init__.py` & `monai-weekly-1.2.dev2317/monai/fl/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/fl/client/__init__.py` & `monai-weekly-1.2.dev2317/monai/fl/client/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/fl/client/client_algo.py` & `monai-weekly-1.2.dev2317/monai/fl/client/client_algo.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/fl/client/monai_algo.py` & `monai-weekly-1.2.dev2317/monai/fl/client/monai_algo.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,39 +7,29 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-import logging
 import os
+import time
 from collections.abc import Mapping, MutableMapping
 from typing import Any, cast
 
 import torch
 import torch.distributed as dist
 
-import monai
 from monai.apps.auto3dseg.data_analyzer import DataAnalyzer
 from monai.apps.utils import get_logger
 from monai.auto3dseg import SegSummarizer
-from monai.bundle import DEFAULT_EXP_MGMT_SETTINGS, ConfigComponent, ConfigItem, ConfigParser, ConfigWorkflow
-from monai.engines import SupervisedTrainer, Trainer
+from monai.bundle import BundleWorkflow, ConfigComponent, ConfigItem, ConfigParser, ConfigWorkflow
+from monai.engines import SupervisedEvaluator, SupervisedTrainer, Trainer
 from monai.fl.client import ClientAlgo, ClientAlgoStats
-from monai.fl.utils.constants import (
-    BundleKeys,
-    ExtraItems,
-    FiltersType,
-    FlPhase,
-    FlStatistics,
-    ModelType,
-    RequiredBundleKeys,
-    WeightType,
-)
+from monai.fl.utils.constants import ExtraItems, FiltersType, FlPhase, FlStatistics, ModelType, WeightType
 from monai.fl.utils.exchange_object import ExchangeObject
 from monai.networks.utils import copy_model_state, get_state_dict
 from monai.utils import min_version, require_pkg
 from monai.utils.enums import DataStatsKeys
 
 logger = get_logger(__name__)
 
@@ -66,73 +56,78 @@
 def compute_weight_diff(global_weights, local_var_dict):
     if global_weights is None:
         raise ValueError("Cannot compute weight differences if `global_weights` is None!")
     if local_var_dict is None:
         raise ValueError("Cannot compute weight differences if `local_var_dict` is None!")
     # compute delta model, global model has the primary key set
     weight_diff = {}
+    n_diff = 0
     for name in global_weights:
         if name not in local_var_dict:
             continue
         # returned weight diff will be on the cpu
         weight_diff[name] = local_var_dict[name].cpu() - global_weights[name].cpu()
+        n_diff += 1
         if torch.any(torch.isnan(weight_diff[name])):
             raise ValueError(f"Weights for {name} became NaN...")
+    if n_diff == 0:
+        raise RuntimeError("No weight differences computed!")
     return weight_diff
 
 
-def check_bundle_config(parser):
-    for k in RequiredBundleKeys:
-        if parser.get(k, None) is None:
-            raise KeyError(f"Bundle config misses required key `{k}`")
-
-
-def disable_ckpt_loaders(parser):
-    if BundleKeys.VALIDATE_HANDLERS in parser:
-        for h in parser[BundleKeys.VALIDATE_HANDLERS]:
+def disable_ckpt_loaders(parser: ConfigParser) -> None:
+    if "validate#handlers" in parser:
+        for h in parser["validate#handlers"]:
             if ConfigComponent.is_instantiable(h):
                 if "CheckpointLoader" in h["_target_"]:
                     h["_disabled_"] = True
 
 
 class MonaiAlgoStats(ClientAlgoStats):
     """
     Implementation of ``ClientAlgoStats`` to allow federated learning with MONAI bundle configurations.
 
     Args:
-        bundle_root: path of bundle.
+        bundle_root: directory path of the bundle.
         config_train_filename: bundle training config path relative to bundle_root. Can be a list of files;
-            defaults to "configs/train.json".
+            defaults to "configs/train.json". only useful when `workflow` is None.
         config_filters_filename: filter configuration file. Can be a list of files; defaults to `None`.
+        data_stats_transform_list: transforms to apply for the data stats result.
         histogram_only: whether to only compute histograms. Defaults to False.
+        workflow: the bundle workflow to execute, usually it's training, evaluation or inference.
+            if None, will create an `ConfigWorkflow` internally based on `config_train_filename`.
     """
 
     def __init__(
         self,
         bundle_root: str,
         config_train_filename: str | list | None = "configs/train.json",
         config_filters_filename: str | list | None = None,
-        train_data_key: str | None = BundleKeys.TRAIN_DATA,
-        eval_data_key: str | None = BundleKeys.VALID_DATA,
         data_stats_transform_list: list | None = None,
         histogram_only: bool = False,
+        workflow: BundleWorkflow | None = None,
     ):
         self.logger = logger
         self.bundle_root = bundle_root
         self.config_train_filename = config_train_filename
         self.config_filters_filename = config_filters_filename
-        self.train_data_key = train_data_key
-        self.eval_data_key = eval_data_key
+        self.train_data_key = "train"
+        self.eval_data_key = "eval"
         self.data_stats_transform_list = data_stats_transform_list
         self.histogram_only = histogram_only
+        self.workflow = None
+        if workflow is not None:
+            if not isinstance(workflow, BundleWorkflow):
+                raise ValueError("workflow must be a subclass of BundleWorkflow.")
+            if workflow.get_workflow_type() is None:
+                raise ValueError("workflow doesn't specify the type.")
+            self.workflow = workflow
 
         self.client_name: str | None = None
         self.app_root: str = ""
-        self.train_parser: ConfigParser | None = None
-        self.filter_parser: ConfigParser | None = None
         self.post_statistics_filters: Any = None
         self.phase = FlPhase.IDLE
         self.dataset_root: Any = None
 
     def initialize(self, extra=None):
         """
         Initialize routine to parse configuration files and extract main components such as trainer, evaluator, and filters.
@@ -145,43 +140,34 @@
         if extra is None:
             extra = {}
         self.client_name = extra.get(ExtraItems.CLIENT_NAME, "noname")
         self.logger.info(f"Initializing {self.client_name} ...")
 
         # FL platform needs to provide filepath to configuration files
         self.app_root = extra.get(ExtraItems.APP_ROOT, "")
-
-        # Read bundle config files
         self.bundle_root = os.path.join(self.app_root, self.bundle_root)
 
-        config_train_files = self._add_config_files(self.config_train_filename)
-        config_filter_files = self._add_config_files(self.config_filters_filename)
+        if self.workflow is None:
+            config_train_files = self._add_config_files(self.config_train_filename)
+            self.workflow = ConfigWorkflow(
+                config_file=config_train_files, meta_file=None, logging_file=None, workflow="train"
+            )
+        self.workflow.initialize()
+        self.workflow.bundle_root = self.bundle_root
+        # initialize the workflow as the content changed
+        self.workflow.initialize()
 
-        # Parse
-        self.train_parser = ConfigParser()
-        self.filter_parser = ConfigParser()
-        if len(config_train_files) > 0:
-            self.train_parser.read_config(config_train_files)
-            check_bundle_config(self.train_parser)
+        config_filter_files = self._add_config_files(self.config_filters_filename)
+        filter_parser = ConfigParser()
         if len(config_filter_files) > 0:
-            self.filter_parser.read_config(config_filter_files)
-
-        # override some config items
-        self.train_parser[RequiredBundleKeys.BUNDLE_ROOT] = self.bundle_root
-
-        # Get data location
-        self.dataset_root = self.train_parser.get_parsed_content(
-            BundleKeys.DATASET_DIR, default=ConfigItem(None, BundleKeys.DATASET_DIR)
-        )
-
-        # Get filters
-        self.post_statistics_filters = self.filter_parser.get_parsed_content(
-            FiltersType.POST_STATISTICS_FILTERS, default=ConfigItem(None, FiltersType.POST_STATISTICS_FILTERS)
-        )
-
+            filter_parser.read_config(config_filter_files)
+            # Get filters
+            self.post_statistics_filters = filter_parser.get_parsed_content(
+                FiltersType.POST_STATISTICS_FILTERS, default=ConfigItem(None, FiltersType.POST_STATISTICS_FILTERS)
+            )
         self.logger.info(f"Initialized {self.client_name}.")
 
     def get_data_stats(self, extra: dict | None = None) -> ExchangeObject:
         """
         Returns summary statistics about the local data.
 
         Args:
@@ -191,49 +177,54 @@
         Returns:
             stats: ExchangeObject with summary statistics.
 
         """
         if extra is None:
             raise ValueError("`extra` has to be set")
 
-        if self.dataset_root:
+        if self.workflow.dataset_dir:  # type: ignore
             self.phase = FlPhase.GET_DATA_STATS
-            self.logger.info(f"Computing statistics on {self.dataset_root}")
+            self.logger.info(f"Computing statistics on {self.workflow.dataset_dir}")  # type: ignore
 
             if FlStatistics.HIST_BINS not in extra:
                 raise ValueError("FlStatistics.NUM_OF_BINS not specified in `extra`")
             else:
                 hist_bins = extra[FlStatistics.HIST_BINS]
             if FlStatistics.HIST_RANGE not in extra:
                 raise ValueError("FlStatistics.HIST_RANGE not specified in `extra`")
             else:
                 hist_range = extra[FlStatistics.HIST_RANGE]
 
             stats_dict = {}
 
             # train data stats
             train_summary_stats, train_case_stats = self._get_data_key_stats(
-                parser=self.train_parser,
+                data=self.workflow.train_dataset_data,  # type: ignore
                 data_key=self.train_data_key,
                 hist_bins=hist_bins,
                 hist_range=hist_range,
                 output_path=os.path.join(self.app_root, "train_data_stats.yaml"),
             )
             if train_case_stats:
                 # Only return summary statistics to FL server
                 stats_dict.update({self.train_data_key: train_summary_stats})
 
             # eval data stats
-            eval_summary_stats, eval_case_stats = self._get_data_key_stats(
-                parser=self.train_parser,
-                data_key=self.eval_data_key,
-                hist_bins=hist_bins,
-                hist_range=hist_range,
-                output_path=os.path.join(self.app_root, "eval_data_stats.yaml"),
-            )
+            eval_summary_stats = None
+            eval_case_stats = None
+            if self.workflow.val_dataset_data is not None:  # type: ignore
+                eval_summary_stats, eval_case_stats = self._get_data_key_stats(
+                    data=self.workflow.val_dataset_data,  # type: ignore
+                    data_key=self.eval_data_key,
+                    hist_bins=hist_bins,
+                    hist_range=hist_range,
+                    output_path=os.path.join(self.app_root, "eval_data_stats.yaml"),
+                )
+            else:
+                self.logger.warning("the datalist doesn't contain validation section.")
             if eval_summary_stats:
                 # Only return summary statistics to FL server
                 stats_dict.update({self.eval_data_key: eval_summary_stats})
 
             # total stats
             if train_case_stats and eval_case_stats:
                 # Compute total summary
@@ -248,25 +239,18 @@
                 for _filter in self.post_statistics_filters:
                     stats = _filter(stats, extra)
 
             return stats
         else:
             raise ValueError("data_root not set!")
 
-    def _get_data_key_stats(self, parser, data_key, hist_bins, hist_range, output_path=None):
-        if data_key not in parser:
-            self.logger.warning(f"Data key {data_key} not available in bundle configs.")
-            return None, None
-        data = parser.get_parsed_content(data_key)
-
-        datalist = {data_key: data}
-
+    def _get_data_key_stats(self, data, data_key, hist_bins, hist_range, output_path=None):
         analyzer = DataAnalyzer(
-            datalist=datalist,
-            dataroot=self.dataset_root,
+            datalist={data_key: data},
+            dataroot=self.workflow.dataset_dir,  # type: ignore
             hist_bins=hist_bins,
             hist_range=hist_range,
             output_path=output_path,
             histogram_only=self.histogram_only,
         )
 
         self.logger.info(f"{self.client_name} compute data statistics on {data_key}...")
@@ -321,227 +305,205 @@
         return files
 
 
 @require_pkg(pkg_name="ignite", version="0.4.10", version_checker=min_version)
 class MonaiAlgo(ClientAlgo, MonaiAlgoStats):
     """
     Implementation of ``ClientAlgo`` to allow federated learning with MONAI bundle configurations.
-    FIXME: reimplement this class based on the bundle "ConfigWorkflow".
 
     Args:
-        bundle_root: path of bundle.
+        bundle_root: directory path of the bundle.
         local_epochs: number of local epochs to execute during each round of local training; defaults to 1.
         send_weight_diff: whether to send weight differences rather than full weights; defaults to `True`.
-        config_train_filename: bundle training config path relative to bundle_root. Can be a list of files;
-            defaults to "configs/train.json".
-        config_evaluate_filename: bundle evaluation config path relative to bundle_root. Can be a list of files.
-            If "default", config_evaluate_filename = ["configs/train.json", "configs/evaluate.json"] will be used;
+        config_train_filename: bundle training config path relative to bundle_root. can be a list of files.
+            defaults to "configs/train.json". only useful when `train_workflow` is None.
+        train_kwargs: other args of the `ConfigWorkflow` of train, except for `config_file`, `meta_file`,
+            `logging_file`, `workflow`. only useful when `train_workflow` is None.
+        config_evaluate_filename: bundle evaluation config path relative to bundle_root. can be a list of files.
+            if "default", ["configs/train.json", "configs/evaluate.json"] will be used.
+            this arg is only useful when `eval_workflow` is None.
+        eval_kwargs: other args of the `ConfigWorkflow` of evaluation, except for `config_file`, `meta_file`,
+            `logging_file`, `workflow`. only useful when `eval_workflow` is None.
         config_filters_filename: filter configuration file. Can be a list of files; defaults to `None`.
         disable_ckpt_loading: do not use any CheckpointLoader if defined in train/evaluate configs; defaults to `True`.
         best_model_filepath: location of best model checkpoint; defaults "models/model.pt" relative to `bundle_root`.
         final_model_filepath: location of final model checkpoint; defaults "models/model_final.pt" relative to `bundle_root`.
         save_dict_key: If a model checkpoint contains several state dicts,
             the one defined by `save_dict_key` will be returned by `get_weights`; defaults to "model".
             If all state dicts should be returned, set `save_dict_key` to None.
-        seed: set random seed for modules to enable or disable deterministic training; defaults to `None`,
-            i.e., non-deterministic training.
-        benchmark: set benchmark to `False` for full deterministic behavior in cuDNN components.
-            Note, full determinism in federated learning depends also on deterministic behavior of other FL components,
-            e.g., the aggregator, which is not controlled by this class.
-        multi_gpu: whether to run MonaiAlgo in a multi-GPU setting; defaults to `False`.
-        backend: backend to use for torch.distributed; defaults to "nccl".
-        init_method: init_method for torch.distributed; defaults to "env://".
-        tracking: if not None, enable the experiment tracking at runtime with optionally configurable and extensible.
-            if "mlflow", will add `MLFlowHandler` to the parsed bundle with default tracking settings,
-            if other string, treat it as file path to load the tracking settings.
-            if `dict`, treat it as tracking settings.
-            will patch the target config content with `tracking handlers` and the top-level items of `configs`.
-            for detailed usage examples, plesae check the tutorial:
-            https://github.com/Project-MONAI/tutorials/blob/main/experiment_management/bundle_integrate_mlflow.ipynb.
+        data_stats_transform_list: transforms to apply for the data stats result.
+        eval_workflow_name: the workflow name corresponding to the "config_evaluate_filename", default to "train"
+            as the default "config_evaluate_filename" overrides the train workflow config.
+            this arg is only useful when `eval_workflow` is None.
+        train_workflow: the bundle workflow to execute training, if None, will create a `ConfigWorkflow` internally
+            based on `config_train_filename` and `train_kwargs`.
+        eval_workflow: the bundle workflow to execute evaluation, if None, will create a `ConfigWorkflow` internally
+            based on `config_evaluate_filename`, `eval_kwargs`, `eval_workflow_name`.
 
     """
 
     def __init__(
         self,
         bundle_root: str,
         local_epochs: int = 1,
         send_weight_diff: bool = True,
         config_train_filename: str | list | None = "configs/train.json",
+        train_kwargs: dict | None = None,
         config_evaluate_filename: str | list | None = "default",
+        eval_kwargs: dict | None = None,
         config_filters_filename: str | list | None = None,
         disable_ckpt_loading: bool = True,
         best_model_filepath: str | None = "models/model.pt",
         final_model_filepath: str | None = "models/model_final.pt",
         save_dict_key: str | None = "model",
-        seed: int | None = None,
-        benchmark: bool = True,
-        multi_gpu: bool = False,
-        backend: str = "nccl",
-        init_method: str = "env://",
-        train_data_key: str | None = BundleKeys.TRAIN_DATA,
-        eval_data_key: str | None = BundleKeys.VALID_DATA,
         data_stats_transform_list: list | None = None,
-        tracking: str | dict | None = None,
+        eval_workflow_name: str = "train",
+        train_workflow: BundleWorkflow | None = None,
+        eval_workflow: BundleWorkflow | None = None,
     ):
         self.logger = logger
-        if config_evaluate_filename == "default":
-            # by default, evaluator needs both training and evaluate to be instantiated.
-            config_evaluate_filename = ["configs/train.json", "configs/evaluate.json"]
         self.bundle_root = bundle_root
         self.local_epochs = local_epochs
         self.send_weight_diff = send_weight_diff
         self.config_train_filename = config_train_filename
+        self.train_kwargs = {} if train_kwargs is None else train_kwargs
+        if config_evaluate_filename == "default":
+            # by default, evaluator needs both training and evaluate to be instantiated
+            config_evaluate_filename = ["configs/train.json", "configs/evaluate.json"]
         self.config_evaluate_filename = config_evaluate_filename
+        self.eval_kwargs = {} if eval_kwargs is None else eval_kwargs
         self.config_filters_filename = config_filters_filename
         self.disable_ckpt_loading = disable_ckpt_loading
         self.model_filepaths = {ModelType.BEST_MODEL: best_model_filepath, ModelType.FINAL_MODEL: final_model_filepath}
         self.save_dict_key = save_dict_key
-        self.seed = seed
-        self.benchmark = benchmark
-        self.multi_gpu = multi_gpu
-        self.backend = backend
-        self.init_method = init_method
-        self.train_data_key = train_data_key
-        self.eval_data_key = eval_data_key
         self.data_stats_transform_list = data_stats_transform_list
-        self.tracking = tracking
+        self.eval_workflow_name = eval_workflow_name
+        self.train_workflow = None
+        self.eval_workflow = None
+        if train_workflow is not None:
+            if not isinstance(train_workflow, BundleWorkflow) or train_workflow.get_workflow_type() != "train":
+                raise ValueError(
+                    f"train workflow must be BundleWorkflow and set type in {BundleWorkflow.supported_train_type}."
+                )
+            self.train_workflow = train_workflow
+        if eval_workflow is not None:
+            # evaluation workflow can be "train" type or "infer" type
+            if not isinstance(eval_workflow, BundleWorkflow) or eval_workflow.get_workflow_type() is None:
+                raise ValueError("train workflow must be BundleWorkflow and set type.")
+            self.eval_workflow = eval_workflow
 
         self.app_root = ""
-        self.train_parser: ConfigParser | None = None
-        self.eval_parser: ConfigParser | None = None
         self.filter_parser: ConfigParser | None = None
         self.trainer: SupervisedTrainer | None = None
-        self.evaluator: Any | None = None
+        self.evaluator: SupervisedEvaluator | None = None
         self.pre_filters = None
         self.post_weight_filters = None
         self.post_evaluate_filters = None
         self.iter_of_start_time = 0
         self.global_weights: Mapping | None = None
-        self.rank = 0
 
         self.phase = FlPhase.IDLE
         self.client_name = None
         self.dataset_root = None
 
     def initialize(self, extra=None):
         """
         Initialize routine to parse configuration files and extract main components such as trainer, evaluator, and filters.
 
         Args:
             extra: Dict with additional information that should be provided by FL system,
                 i.e., `ExtraItems.CLIENT_NAME` and `ExtraItems.APP_ROOT`.
 
         """
+        self._set_cuda_device()
         if extra is None:
             extra = {}
         self.client_name = extra.get(ExtraItems.CLIENT_NAME, "noname")
+        timestamp = time.strftime("%Y%m%d_%H%M%S")
         self.logger.info(f"Initializing {self.client_name} ...")
-
-        if self.multi_gpu:
-            dist.init_process_group(backend=self.backend, init_method=self.init_method)
-            self._set_cuda_device()
-            self.logger.info(
-                f"Using multi-gpu training on rank {self.rank} (available devices: {torch.cuda.device_count()})"
-            )
-            if self.rank > 0:
-                self.logger.setLevel(logging.WARNING)
-
-        if self.seed:
-            monai.utils.set_determinism(seed=self.seed)
-        torch.backends.cudnn.benchmark = self.benchmark
-
         # FL platform needs to provide filepath to configuration files
         self.app_root = extra.get(ExtraItems.APP_ROOT, "")
-
-        # Read bundle config files
         self.bundle_root = os.path.join(self.app_root, self.bundle_root)
 
-        config_train_files = self._add_config_files(self.config_train_filename)
-        config_eval_files = self._add_config_files(self.config_evaluate_filename)
-        config_filter_files = self._add_config_files(self.config_filters_filename)
+        if self.train_workflow is None and self.config_train_filename is not None:
+            config_train_files = self._add_config_files(self.config_train_filename)
+            # if enabled experiment tracking, set the run name to the FL client name and timestamp,
+            # expect the tracking settings use "run_name" to define the run name
+            if "run_name" not in self.train_kwargs:
+                self.train_kwargs["run_name"] = f"{self.client_name}_{timestamp}"
+            self.train_workflow = ConfigWorkflow(
+                config_file=config_train_files, meta_file=None, logging_file=None, workflow="train", **self.train_kwargs
+            )
+        if self.train_workflow is not None:
+            self.train_workflow.initialize()
+            self.train_workflow.bundle_root = self.bundle_root
+            self.train_workflow.max_epochs = self.local_epochs
+            if self.disable_ckpt_loading and isinstance(self.train_workflow, ConfigWorkflow):
+                disable_ckpt_loaders(parser=self.train_workflow.parser)
+            # initialize the workflow as the content changed
+            self.train_workflow.initialize()
+            self.trainer = self.train_workflow.trainer
+            if not isinstance(self.trainer, SupervisedTrainer):
+                raise ValueError(f"trainer must be SupervisedTrainer, but got: {type(self.trainer)}.")
+
+        if self.eval_workflow is None and self.config_evaluate_filename is not None:
+            config_eval_files = self._add_config_files(self.config_evaluate_filename)
+            # if enabled experiment tracking, set the run name to the FL client name and timestamp,
+            # expect the tracking settings use "run_name" to define the run name
+            if "run_name" not in self.eval_kwargs:
+                self.eval_kwargs["run_name"] = f"{self.client_name}_{timestamp}"
+            self.eval_workflow = ConfigWorkflow(
+                config_file=config_eval_files,
+                meta_file=None,
+                logging_file=None,
+                workflow=self.eval_workflow_name,
+                **self.eval_kwargs,
+            )
+        if self.eval_workflow is not None:
+            self.eval_workflow.initialize()
+            self.eval_workflow.bundle_root = self.bundle_root
+            if self.disable_ckpt_loading and isinstance(self.eval_workflow, ConfigWorkflow):
+                disable_ckpt_loaders(parser=self.eval_workflow.parser)
+            # initialize the workflow as the content changed
+            self.eval_workflow.initialize()
+            self.evaluator = self.eval_workflow.evaluator
+            if not isinstance(self.evaluator, SupervisedEvaluator):
+                raise ValueError(f"evaluator must be SupervisedEvaluator, but got: {type(self.evaluator)}.")
 
-        # Parse
-        self.train_parser = ConfigParser()
-        self.eval_parser = ConfigParser()
+        config_filter_files = self._add_config_files(self.config_filters_filename)
         self.filter_parser = ConfigParser()
-        if len(config_train_files) > 0:
-            self.train_parser.read_config(config_train_files)
-            check_bundle_config(self.train_parser)
-        if len(config_eval_files) > 0:
-            self.eval_parser.read_config(config_eval_files)
-            check_bundle_config(self.eval_parser)
         if len(config_filter_files) > 0:
             self.filter_parser.read_config(config_filter_files)
 
-        # override some config items
-        self.train_parser[RequiredBundleKeys.BUNDLE_ROOT] = self.bundle_root
-        self.eval_parser[RequiredBundleKeys.BUNDLE_ROOT] = self.bundle_root
-        # number of training epochs for each round
-        if BundleKeys.TRAIN_TRAINER_MAX_EPOCHS in self.train_parser:
-            self.train_parser[BundleKeys.TRAIN_TRAINER_MAX_EPOCHS] = self.local_epochs
-
-        # remove checkpoint loaders
-        if self.disable_ckpt_loading:
-            disable_ckpt_loaders(self.train_parser)
-            disable_ckpt_loaders(self.eval_parser)
-
-        # set tracking configs for experiment management
-        if self.tracking is not None:
-            if isinstance(self.tracking, str) and self.tracking in DEFAULT_EXP_MGMT_SETTINGS:
-                settings_ = DEFAULT_EXP_MGMT_SETTINGS[self.tracking]
-            else:
-                settings_ = ConfigParser.load_config_files(self.tracking)
-            ConfigWorkflow.patch_bundle_tracking(parser=self.train_parser, settings=settings_)
-            ConfigWorkflow.patch_bundle_tracking(parser=self.eval_parser, settings=settings_)
-
-        # Get trainer, evaluator
-        self.trainer = self.train_parser.get_parsed_content(
-            BundleKeys.TRAINER, default=ConfigItem(None, BundleKeys.TRAINER)
-        )
-        self.evaluator = self.eval_parser.get_parsed_content(
-            BundleKeys.EVALUATOR, default=ConfigItem(None, BundleKeys.EVALUATOR)
-        )
-
         # Get filters
         self.pre_filters = self.filter_parser.get_parsed_content(
             FiltersType.PRE_FILTERS, default=ConfigItem(None, FiltersType.PRE_FILTERS)
         )
         self.post_weight_filters = self.filter_parser.get_parsed_content(
             FiltersType.POST_WEIGHT_FILTERS, default=ConfigItem(None, FiltersType.POST_WEIGHT_FILTERS)
         )
         self.post_evaluate_filters = self.filter_parser.get_parsed_content(
             FiltersType.POST_EVALUATE_FILTERS, default=ConfigItem(None, FiltersType.POST_EVALUATE_FILTERS)
         )
         self.post_statistics_filters = self.filter_parser.get_parsed_content(
             FiltersType.POST_STATISTICS_FILTERS, default=ConfigItem(None, FiltersType.POST_STATISTICS_FILTERS)
         )
-
-        # Get data location
-        self.dataset_root = self.train_parser.get_parsed_content(
-            BundleKeys.DATASET_DIR, default=ConfigItem(None, BundleKeys.DATASET_DIR)
-        )
-
-        if self.multi_gpu:
-            if self.rank > 0 and self.trainer:
-                self.trainer.logger.setLevel(logging.WARNING)
-            if self.rank > 0 and self.evaluator:
-                self.evaluator.logger.setLevel(logging.WARNING)
         self.logger.info(f"Initialized {self.client_name}.")
 
     def train(self, data: ExchangeObject, extra: dict | None = None) -> None:
         """
         Train on client's local data.
 
         Args:
             data: `ExchangeObject` containing the current global model weights.
             extra: Dict with additional information that can be provided by the FL system.
 
         """
-        self._set_cuda_device()
 
+        self._set_cuda_device()
         if extra is None:
             extra = {}
         if not isinstance(data, ExchangeObject):
             raise ValueError(f"expected data to be ExchangeObject but received {type(data)}")
 
         if self.trainer is None:
             raise ValueError("self.trainer should not be None.")
@@ -575,16 +537,16 @@
             extra: Dict with additional information that can be provided by the FL system.
 
         Returns:
             return_weights: `ExchangeObject` containing current weights (default)
                 or load requested model type from disk (`ModelType.BEST_MODEL` or `ModelType.FINAL_MODEL`).
 
         """
-        self._set_cuda_device()
 
+        self._set_cuda_device()
         if extra is None:
             extra = {}
 
         # by default return current weights, return best if requested via model type.
         self.phase = FlPhase.GET_WEIGHTS
 
         if ExtraItems.MODEL_TYPE in extra:
@@ -654,16 +616,16 @@
             data: `ExchangeObject` containing the current global model weights.
             extra: Dict with additional information that can be provided by the FL system.
 
         Returns:
             return_metrics: `ExchangeObject` containing evaluation metrics.
 
         """
-        self._set_cuda_device()
 
+        self._set_cuda_device()
         if extra is None:
             extra = {}
         if not isinstance(data, ExchangeObject):
             raise ValueError(f"expected data to be ExchangeObject but received {type(data)}")
 
         if self.evaluator is None:
             raise ValueError("self.evaluator should not be None.")
@@ -717,25 +679,26 @@
         self.logger.info(f"Terminating {self.client_name} during {self.phase} phase.")
         if isinstance(self.trainer, Trainer):
             self.logger.info(f"Terminating {self.client_name} trainer...")
             self.trainer.terminate()
         if isinstance(self.evaluator, Trainer):
             self.logger.info(f"Terminating {self.client_name} evaluator...")
             self.evaluator.terminate()
-
-        if self.multi_gpu:
-            dist.destroy_process_group()
+        if self.train_workflow is not None:
+            self.train_workflow.finalize()
+        if self.eval_workflow is not None:
+            self.eval_workflow.finalize()
 
     def _check_converted(self, global_weights, local_var_dict, n_converted):
         if n_converted == 0:
-            self.logger.warning(
+            raise RuntimeError(
                 f"No global weights converted! Received weight dict keys are {list(global_weights.keys())}"
             )
         else:
             self.logger.info(
                 f"Converted {n_converted} global variables to match {len(local_var_dict)} local variables."
             )
 
     def _set_cuda_device(self):
-        if self.multi_gpu:
+        if dist.is_initialized():
             self.rank = int(os.environ["LOCAL_RANK"])
             torch.cuda.set_device(self.rank)
```

### Comparing `monai-weekly-1.2.dev2316/monai/fl/utils/__init__.py` & `monai-weekly-1.2.dev2317/monai/fl/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/fl/utils/constants.py` & `monai-weekly-1.2.dev2317/monai/fl/utils/constants.py`

 * *Files 11% similar despite different names*

```diff
@@ -47,26 +47,12 @@
     DATA_STATS = "data_stats"
     DATA_COUNT = "data_count"
     FAIL_COUNT = "fail_count"
     TOTAL_DATA = "total_data"
     FEATURE_NAMES = "feature_names"
 
 
-class RequiredBundleKeys(StrEnum):
-    BUNDLE_ROOT = "bundle_root"
-
-
-class BundleKeys(StrEnum):
-    TRAINER = "train#trainer"
-    EVALUATOR = "validate#evaluator"
-    TRAIN_TRAINER_MAX_EPOCHS = "train#trainer#max_epochs"
-    VALIDATE_HANDLERS = "validate#handlers"
-    DATASET_DIR = "dataset_dir"
-    TRAIN_DATA = "train#dataset#data"
-    VALID_DATA = "validate#dataset#data"
-
-
 class FiltersType(StrEnum):
     PRE_FILTERS = "pre_filters"
     POST_WEIGHT_FILTERS = "post_weight_filters"
     POST_EVALUATE_FILTERS = "post_evaluate_filters"
     POST_STATISTICS_FILTERS = "post_statistics_filters"
```

### Comparing `monai-weekly-1.2.dev2316/monai/fl/utils/exchange_object.py` & `monai-weekly-1.2.dev2317/monai/fl/utils/exchange_object.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/fl/utils/filters.py` & `monai-weekly-1.2.dev2317/monai/fl/utils/filters.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         """
 
         raise NotImplementedError
 
 
 class SummaryFilter(Filter):
     """
-    Summary filter to content of ExchangeObject.
+    Summary filter to show content of ExchangeObject.
     """
 
     def __call__(self, data: ExchangeObject, extra: dict | None = None) -> ExchangeObject:
         """
         Example filter that doesn't filter anything but only prints data summary.
 
         Arguments:
```

### Comparing `monai-weekly-1.2.dev2316/monai/handlers/__init__.py` & `monai-weekly-1.2.dev2317/monai/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/handlers/checkpoint_loader.py` & `monai-weekly-1.2.dev2317/monai/handlers/checkpoint_loader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/handlers/checkpoint_saver.py` & `monai-weekly-1.2.dev2317/monai/handlers/checkpoint_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/handlers/classification_saver.py` & `monai-weekly-1.2.dev2317/monai/handlers/classification_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/handlers/clearml_handlers.py` & `monai-weekly-1.2.dev2317/monai/handlers/clearml_handlers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/handlers/confusion_matrix.py` & `monai-weekly-1.2.dev2317/monai/handlers/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/handlers/decollate_batch.py` & `monai-weekly-1.2.dev2317/monai/handlers/decollate_batch.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/handlers/earlystop_handler.py` & `monai-weekly-1.2.dev2317/monai/handlers/earlystop_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/handlers/garbage_collector.py` & `monai-weekly-1.2.dev2317/monai/handlers/garbage_collector.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/handlers/hausdorff_distance.py` & `monai-weekly-1.2.dev2317/monai/handlers/hausdorff_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/handlers/ignite_metric.py` & `monai-weekly-1.2.dev2317/monai/handlers/ignite_metric.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/handlers/logfile_handler.py` & `monai-weekly-1.2.dev2317/monai/handlers/logfile_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/handlers/lr_schedule_handler.py` & `monai-weekly-1.2.dev2317/monai/handlers/lr_schedule_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/handlers/mean_dice.py` & `monai-weekly-1.2.dev2317/monai/handlers/mean_iou.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,45 +10,45 @@
 # limitations under the License.
 
 from __future__ import annotations
 
 from collections.abc import Callable
 
 from monai.handlers.ignite_metric import IgniteMetric
-from monai.metrics import DiceMetric
+from monai.metrics import MeanIoU
 from monai.utils import MetricReduction
 
 
-class MeanDice(IgniteMetric):
+class MeanIoUHandler(IgniteMetric):
     """
-    Computes Dice score metric from full size Tensor and collects average over batch, class-channels, iterations.
+    Computes IoU score metric from full size Tensor and collects average over batch, class-channels, iterations.
     """
 
     def __init__(
         self,
         include_background: bool = True,
         reduction: MetricReduction | str = MetricReduction.MEAN,
         output_transform: Callable = lambda x: x,
         save_details: bool = True,
     ) -> None:
         """
 
         Args:
-            include_background: whether to include dice computation on the first channel of the predicted output.
+            include_background: whether to include iou computation on the first channel of the predicted output.
                 Defaults to True.
             reduction: define the mode to reduce metrics, will only execute reduction on `not-nan` values,
                 available reduction modes: {``"none"``, ``"mean"``, ``"sum"``, ``"mean_batch"``, ``"sum_batch"``,
                 ``"mean_channel"``, ``"sum_channel"``}, default to ``"mean"``. if "none", will not do reduction.
             output_transform: callable to extract `y_pred` and `y` from `ignite.engine.state.output` then
                 construct `(y_pred, y)` pair, where `y_pred` and `y` can be `batch-first` Tensors or
                 lists of `channel-first` Tensors. the form of `(y_pred, y)` is required by the `update()`.
                 `engine.state` and `output_transform` inherit from the ignite concept:
                 https://pytorch.org/ignite/concepts.html#state, explanation and usage example are in the tutorial:
                 https://github.com/Project-MONAI/tutorials/blob/master/modules/batch_output_transform.ipynb.
-            save_details: whether to save metric computation details per image, for example: mean dice of every image.
+            save_details: whether to save metric computation details per image, for example: mean iou of every image.
                 default to True, will save to `engine.state.metric_details` dict with the metric name as key.
 
         See also:
-            :py:meth:`monai.metrics.meandice.compute_dice`
+            :py:meth:`monai.metrics.meaniou.compute_meaniou`
         """
-        metric_fn = DiceMetric(include_background=include_background, reduction=reduction)
+        metric_fn = MeanIoU(include_background=include_background, reduction=reduction)
         super().__init__(metric_fn=metric_fn, output_transform=output_transform, save_details=save_details)
```

### Comparing `monai-weekly-1.2.dev2316/monai/handlers/mean_iou.py` & `monai-weekly-1.2.dev2317/monai/handlers/mean_dice.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,45 +10,49 @@
 # limitations under the License.
 
 from __future__ import annotations
 
 from collections.abc import Callable
 
 from monai.handlers.ignite_metric import IgniteMetric
-from monai.metrics import MeanIoU
+from monai.metrics import DiceMetric
 from monai.utils import MetricReduction
 
 
-class MeanIoUHandler(IgniteMetric):
+class MeanDice(IgniteMetric):
     """
-    Computes IoU score metric from full size Tensor and collects average over batch, class-channels, iterations.
+    Computes Dice score metric from full size Tensor and collects average over batch, class-channels, iterations.
     """
 
     def __init__(
         self,
         include_background: bool = True,
         reduction: MetricReduction | str = MetricReduction.MEAN,
+        num_classes: int | None = None,
         output_transform: Callable = lambda x: x,
         save_details: bool = True,
     ) -> None:
         """
 
         Args:
-            include_background: whether to include iou computation on the first channel of the predicted output.
+            include_background: whether to include dice computation on the first channel of the predicted output.
                 Defaults to True.
             reduction: define the mode to reduce metrics, will only execute reduction on `not-nan` values,
                 available reduction modes: {``"none"``, ``"mean"``, ``"sum"``, ``"mean_batch"``, ``"sum_batch"``,
                 ``"mean_channel"``, ``"sum_channel"``}, default to ``"mean"``. if "none", will not do reduction.
+            num_classes: number of input channels (always including the background). When this is None,
+                ``y_pred.shape[1]`` will be used. This option is useful when both ``y_pred`` and ``y`` are
+                single-channel class indices and the number of classes is not automatically inferred from data.
             output_transform: callable to extract `y_pred` and `y` from `ignite.engine.state.output` then
                 construct `(y_pred, y)` pair, where `y_pred` and `y` can be `batch-first` Tensors or
                 lists of `channel-first` Tensors. the form of `(y_pred, y)` is required by the `update()`.
                 `engine.state` and `output_transform` inherit from the ignite concept:
                 https://pytorch.org/ignite/concepts.html#state, explanation and usage example are in the tutorial:
                 https://github.com/Project-MONAI/tutorials/blob/master/modules/batch_output_transform.ipynb.
-            save_details: whether to save metric computation details per image, for example: mean iou of every image.
+            save_details: whether to save metric computation details per image, for example: mean dice of every image.
                 default to True, will save to `engine.state.metric_details` dict with the metric name as key.
 
         See also:
-            :py:meth:`monai.metrics.meaniou.compute_meaniou`
+            :py:meth:`monai.metrics.meandice.compute_dice`
         """
-        metric_fn = MeanIoU(include_background=include_background, reduction=reduction)
+        metric_fn = DiceMetric(include_background=include_background, reduction=reduction, num_classes=num_classes)
         super().__init__(metric_fn=metric_fn, output_transform=output_transform, save_details=save_details)
```

### Comparing `monai-weekly-1.2.dev2316/monai/handlers/metric_logger.py` & `monai-weekly-1.2.dev2317/monai/handlers/metric_logger.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/handlers/metrics_reloaded_handler.py` & `monai-weekly-1.2.dev2317/monai/handlers/metrics_reloaded_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/handlers/metrics_saver.py` & `monai-weekly-1.2.dev2317/monai/handlers/metrics_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/handlers/mlflow_handler.py` & `monai-weekly-1.2.dev2317/monai/handlers/mlflow_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/handlers/nvtx_handlers.py` & `monai-weekly-1.2.dev2317/monai/handlers/nvtx_handlers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/handlers/panoptic_quality.py` & `monai-weekly-1.2.dev2317/monai/handlers/panoptic_quality.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/handlers/parameter_scheduler.py` & `monai-weekly-1.2.dev2317/monai/handlers/parameter_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/handlers/postprocessing.py` & `monai-weekly-1.2.dev2317/monai/handlers/postprocessing.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/handlers/probability_maps.py` & `monai-weekly-1.2.dev2317/monai/handlers/probability_maps.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/handlers/regression_metrics.py` & `monai-weekly-1.2.dev2317/monai/handlers/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/handlers/roc_auc.py` & `monai-weekly-1.2.dev2317/monai/handlers/roc_auc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/handlers/smartcache_handler.py` & `monai-weekly-1.2.dev2317/monai/handlers/smartcache_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/handlers/stats_handler.py` & `monai-weekly-1.2.dev2317/monai/handlers/stats_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/handlers/surface_distance.py` & `monai-weekly-1.2.dev2317/monai/handlers/surface_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/handlers/tensorboard_handlers.py` & `monai-weekly-1.2.dev2317/monai/handlers/tensorboard_handlers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/handlers/utils.py` & `monai-weekly-1.2.dev2317/monai/handlers/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/handlers/validation_handler.py` & `monai-weekly-1.2.dev2317/monai/handlers/validation_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/inferers/__init__.py` & `monai-weekly-1.2.dev2317/monai/inferers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/inferers/inferer.py` & `monai-weekly-1.2.dev2317/monai/inferers/inferer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/inferers/merger.py` & `monai-weekly-1.2.dev2317/monai/inferers/merger.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/inferers/splitter.py` & `monai-weekly-1.2.dev2317/monai/inferers/splitter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/inferers/utils.py` & `monai-weekly-1.2.dev2317/monai/inferers/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -276,15 +276,15 @@
                 if non_blocking:
                     output_image_list[0][o_slice].copy_(sw_device_buffer[0], non_blocking=non_blocking)
                 else:
                     output_image_list[0][o_slice] += sw_device_buffer[0].to(device=device)
             else:
                 sw_device_buffer[ss] *= w_t
                 sw_device_buffer[ss] = sw_device_buffer[ss].to(device)
-                _compute_coords(sw_batch_size, unravel_slice, z_scale, output_image_list[ss], sw_device_buffer[ss])
+                _compute_coords(unravel_slice, z_scale, output_image_list[ss], sw_device_buffer[ss])
         sw_device_buffer = []
         if buffered:
             b_s += 1
 
     if non_blocking:
         torch.cuda.current_stream().synchronize()
 
@@ -338,15 +338,15 @@
         s_s = slices_np[windows_range[_s - 1].stop % len(slices) if _s > 0 else 0, 0]
         s_e = slices_np[(_r.stop - 1) % len(slices), 1]
         b_slices.append((_r.stop, s_s, s_e))  # buffer index, slice start, slice end
     windows_range = itertools.chain(*windows_range)  # type: ignore
     return slices, n_per_batch, b_slices, windows_range
 
 
-def _compute_coords(sw, coords, z_scale, out, patch):
+def _compute_coords(coords, z_scale, out, patch):
     """sliding window batch spatial scaling indexing for multi-resolution outputs."""
     for original_idx, p in zip(coords, patch):
         idx_zm = list(original_idx)  # 4D for 2D image, 5D for 3D image
         if z_scale:
             for axis in range(2, len(idx_zm)):
                 idx_zm[axis] = slice(
                     int(original_idx[axis].start * z_scale[axis - 2]), int(original_idx[axis].stop * z_scale[axis - 2])
```

### Comparing `monai-weekly-1.2.dev2316/monai/losses/__init__.py` & `monai-weekly-1.2.dev2317/monai/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/losses/contrastive.py` & `monai-weekly-1.2.dev2317/monai/losses/contrastive.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/losses/deform.py` & `monai-weekly-1.2.dev2317/monai/losses/deform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/losses/dice.py` & `monai-weekly-1.2.dev2317/monai/losses/dice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/losses/ds_loss.py` & `monai-weekly-1.2.dev2317/monai/losses/ds_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/losses/focal_loss.py` & `monai-weekly-1.2.dev2317/monai/losses/focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/losses/giou_loss.py` & `monai-weekly-1.2.dev2317/monai/losses/giou_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/losses/image_dissimilarity.py` & `monai-weekly-1.2.dev2317/monai/losses/image_dissimilarity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/losses/multi_scale.py` & `monai-weekly-1.2.dev2317/monai/losses/multi_scale.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/losses/spatial_mask.py` & `monai-weekly-1.2.dev2317/monai/losses/spatial_mask.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/losses/ssim_loss.py` & `monai-weekly-1.2.dev2317/monai/losses/ssim_loss.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,98 +7,119 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
+from collections.abc import Sequence
+
 import torch
 from torch.nn.modules.loss import _Loss
 
-from monai.metrics.regression import SSIMMetric
+from monai.metrics.regression import KernelType, SSIMMetric
+from monai.utils import LossReduction, ensure_tuple_rep
 
 
 class SSIMLoss(_Loss):
     """
-    Build a Pytorch version of the SSIM loss function based on the original formula of SSIM
-
-    Modified and adopted from:
-        https://github.com/facebookresearch/fastMRI/blob/main/banding_removal/fastmri/ssim_loss_mixin.py
+    Compute the loss function based on the Structural Similarity Index Measure (SSIM) Metric.
 
     For more info, visit
         https://vicuesoft.com/glossary/term/ssim-ms-ssim/
 
     SSIM reference paper:
         Wang, Zhou, et al. "Image quality assessment: from error visibility to structural
         similarity." IEEE transactions on image processing 13.4 (2004): 600-612.
     """
 
-    def __init__(self, win_size: int = 7, k1: float = 0.01, k2: float = 0.03, spatial_dims: int = 2):
+    def __init__(
+        self,
+        spatial_dims: int,
+        data_range: float = 1.0,
+        kernel_type: KernelType | str = KernelType.GAUSSIAN,
+        win_size: int | Sequence[int] = 11,
+        kernel_sigma: float | Sequence[float] = 1.5,
+        k1: float = 0.01,
+        k2: float = 0.03,
+        reduction: LossReduction | str = LossReduction.MEAN,
+    ):
         """
         Args:
-            win_size: gaussian weighting window size
+            spatial_dims: number of spatial dimensions of the input images.
+            data_range: value range of input images. (usually 1.0 or 255)
+            kernel_type: type of kernel, can be "gaussian" or "uniform".
+            win_size: window size of kernel
+            kernel_sigma: standard deviation for Gaussian kernel.
             k1: stability constant used in the luminance denominator
             k2: stability constant used in the contrast denominator
-            spatial_dims: if 2, input shape is expected to be (B,C,H,W). if 3, it is expected to be (B,C,H,W,D)
+            reduction: {``"none"``, ``"mean"``, ``"sum"``}
+                Specifies the reduction to apply to the output. Defaults to ``"mean"``.
+                - ``"none"``: no reduction will be applied.
+                - ``"mean"``: the sum of the output will be divided by the number of elements in the output.
+                - ``"sum"``: the output will be summed.
+
         """
-        super().__init__()
-        self.win_size = win_size
-        self.k1, self.k2 = k1, k2
+        super().__init__(reduction=LossReduction(reduction).value)
         self.spatial_dims = spatial_dims
+        self.data_range = data_range
+        self.kernel_type = kernel_type
 
-    def forward(self, x: torch.Tensor, y: torch.Tensor, data_range: torch.Tensor) -> torch.Tensor:
+        if not isinstance(win_size, Sequence):
+            win_size = ensure_tuple_rep(win_size, spatial_dims)
+        self.kernel_size = win_size
+
+        if not isinstance(kernel_sigma, Sequence):
+            kernel_sigma = ensure_tuple_rep(kernel_sigma, spatial_dims)
+        self.kernel_sigma = kernel_sigma
+
+        self.k1 = k1
+        self.k2 = k2
+
+        self.ssim_metric = SSIMMetric(
+            spatial_dims=self.spatial_dims,
+            data_range=self.data_range,
+            kernel_type=self.kernel_type,
+            win_size=self.kernel_size,
+            kernel_sigma=self.kernel_sigma,
+            k1=self.k1,
+            k2=self.k2,
+        )
+
+    def forward(self, input: torch.Tensor, target: torch.Tensor) -> torch.Tensor:
         """
         Args:
-            x: first sample (e.g., the reference image). Its shape is (B,C,W,H) for 2D and pseudo-3D data,
-                and (B,C,W,H,D) for 3D data,
-            y: second sample (e.g., the reconstructed image). It has similar shape as x.
-            data_range: dynamic range of the data
+            input: batch of predicted images with shape (batch_size, channels, spatial_dim1, spatial_dim2[, spatial_dim3])
+            target: batch of target images with shape (batch_size, channels, spatial_dim1, spatial_dim2[, spatial_dim3])
 
         Returns:
-            1-ssim_value (recall this is meant to be a loss function)
+            1 minus the ssim index (recall this is meant to be a loss function)
 
         Example:
             .. code-block:: python
 
                 import torch
 
                 # 2D data
                 x = torch.ones([1,1,10,10])/2
                 y = torch.ones([1,1,10,10])/2
-                data_range = x.max().unsqueeze(0)
-                # the following line should print 1.0 (or 0.9999)
-                print(1-SSIMLoss(spatial_dims=2)(x,y,data_range))
+                print(1-SSIMLoss(spatial_dims=2)(x,y))
 
                 # pseudo-3D data
                 x = torch.ones([1,5,10,10])/2  # 5 could represent number of slices
                 y = torch.ones([1,5,10,10])/2
-                data_range = x.max().unsqueeze(0)
-                # the following line should print 1.0 (or 0.9999)
-                print(1-SSIMLoss(spatial_dims=2)(x,y,data_range))
+                print(1-SSIMLoss(spatial_dims=2)(x,y))
 
                 # 3D data
                 x = torch.ones([1,1,10,10,10])/2
                 y = torch.ones([1,1,10,10,10])/2
-                data_range = x.max().unsqueeze(0)
-                # the following line should print 1.0 (or 0.9999)
-                print(1-SSIMLoss(spatial_dims=3)(x,y,data_range))
+                print(1-SSIMLoss(spatial_dims=3)(x,y))
         """
-        if x.shape[0] == 1:
-            ssim_value: torch.Tensor = SSIMMetric(
-                data_range, self.win_size, self.k1, self.k2, self.spatial_dims
-            )._compute_tensor(x, y)
-        elif x.shape[0] > 1:
-            for i in range(x.shape[0]):
-                ssim_val: torch.Tensor = SSIMMetric(
-                    data_range, self.win_size, self.k1, self.k2, self.spatial_dims
-                )._compute_tensor(x[i : i + 1], y[i : i + 1])
-                if i == 0:
-                    ssim_value = ssim_val
-                else:
-                    ssim_value = torch.cat((ssim_value.view(i), ssim_val.view(1)), dim=0)
-
-        else:
-            raise ValueError("Batch size is not nonnegative integer value")
-        # 1- dimensional tensor is only allowed
-        ssim_value = ssim_value.view(-1, 1)
-        loss: torch.Tensor = 1 - ssim_value.mean()
+        ssim_value = self.ssim_metric._compute_tensor(input, target).view(-1, 1)
+        loss: torch.Tensor = 1 - ssim_value
+
+        if self.reduction == LossReduction.MEAN.value:
+            loss = torch.mean(loss)  # the batch average
+        elif self.reduction == LossReduction.SUM.value:
+            loss = torch.sum(loss)  # sum over the batch
+
         return loss
```

### Comparing `monai-weekly-1.2.dev2316/monai/losses/tversky.py` & `monai-weekly-1.2.dev2317/monai/losses/tversky.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/losses/unified_focal_loss.py` & `monai-weekly-1.2.dev2317/monai/losses/unified_focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/metrics/__init__.py` & `monai-weekly-1.2.dev2317/monai/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/metrics/active_learning_metrics.py` & `monai-weekly-1.2.dev2317/monai/metrics/active_learning_metrics.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/metrics/confusion_matrix.py` & `monai-weekly-1.2.dev2317/monai/metrics/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/metrics/cumulative_average.py` & `monai-weekly-1.2.dev2317/monai/metrics/cumulative_average.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/metrics/f_beta_score.py` & `monai-weekly-1.2.dev2317/monai/metrics/f_beta_score.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/metrics/froc.py` & `monai-weekly-1.2.dev2317/monai/metrics/froc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/metrics/generalized_dice.py` & `monai-weekly-1.2.dev2317/monai/metrics/generalized_dice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/metrics/hausdorff_distance.py` & `monai-weekly-1.2.dev2317/monai/metrics/hausdorff_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/metrics/loss_metric.py` & `monai-weekly-1.2.dev2317/monai/metrics/loss_metric.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/metrics/meandice.py` & `monai-weekly-1.2.dev2317/monai/metrics/meandice.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,35 +43,41 @@
             available reduction modes: {``"none"``, ``"mean"``, ``"sum"``, ``"mean_batch"``, ``"sum_batch"``,
             ``"mean_channel"``, ``"sum_channel"``}, default to ``"mean"``. if "none", will not do reduction.
         get_not_nans: whether to return the `not_nans` count, if True, aggregate() returns (metric, not_nans).
             Here `not_nans` count the number of not nans for the metric, thus its shape equals to the shape of the metric.
         ignore_empty: whether to ignore empty ground truth cases during calculation.
             If `True`, NaN value will be set for empty ground truth cases.
             If `False`, 1 will be set if the predictions of empty ground truth cases are also empty.
+        num_classes: number of input channels (always including the background). When this is None,
+            ``y_pred.shape[1]`` will be used. This option is useful when both ``y_pred`` and ``y`` are
+            single-channel class indices and the number of classes is not automatically inferred from data.
 
     """
 
     def __init__(
         self,
         include_background: bool = True,
         reduction: MetricReduction | str = MetricReduction.MEAN,
         get_not_nans: bool = False,
         ignore_empty: bool = True,
+        num_classes: int | None = None,
     ) -> None:
         super().__init__()
         self.include_background = include_background
         self.reduction = reduction
         self.get_not_nans = get_not_nans
         self.ignore_empty = ignore_empty
+        self.num_classes = num_classes
         self.dice_helper = DiceHelper(
             include_background=self.include_background,
             reduction=MetricReduction.NONE,
             get_not_nans=False,
             softmax=False,
             ignore_empty=self.ignore_empty,
+            num_classes=self.num_classes,
         )
 
     def _compute_tensor(self, y_pred: torch.Tensor, y: torch.Tensor) -> torch.Tensor:  # type: ignore[override]
         """
         Args:
             y_pred: input data to compute, typical segmentation model output.
                 It must be one-hot format and first dim is batch, example shape: [16, 3, 32, 32]. The values
@@ -106,46 +112,53 @@
 
         # do metric reduction
         f, not_nans = do_metric_reduction(data, reduction or self.reduction)
         return (f, not_nans) if self.get_not_nans else f
 
 
 def compute_dice(
-    y_pred: torch.Tensor, y: torch.Tensor, include_background: bool = True, ignore_empty: bool = True
+    y_pred: torch.Tensor,
+    y: torch.Tensor,
+    include_background: bool = True,
+    ignore_empty: bool = True,
+    num_classes: int | None = None,
 ) -> torch.Tensor:
     """Computes Dice score metric for a batch of predictions.
 
     Args:
         y_pred: input data to compute, typical segmentation model output.
-            It must be one-hot format and first dim is batch, example shape: [16, 3, 32, 32]. The values
-            should be binarized.
+            `y_pred` can be single-channel class indices or in the one-hot format.
         y: ground truth to compute mean dice metric. `y` can be single-channel class indices or in the one-hot format.
         include_background: whether to skip Dice computation on the first channel of
             the predicted output. Defaults to True.
         ignore_empty: whether to ignore empty ground truth cases during calculation.
             If `True`, NaN value will be set for empty ground truth cases.
             If `False`, 1 will be set if the predictions of empty ground truth cases are also empty.
+        num_classes: number of input channels (always including the background). When this is None,
+            ``y_pred.shape[1]`` will be used. This option is useful when both ``y_pred`` and ``y`` are
+            single-channel class indices and the number of classes is not automatically inferred from data.
 
     Returns:
         Dice scores per batch and per class, (shape: [batch_size, num_classes]).
 
     """
     return DiceHelper(  # type: ignore
         include_background=include_background,
         reduction=MetricReduction.NONE,
         get_not_nans=False,
         softmax=False,
         ignore_empty=ignore_empty,
+        num_classes=num_classes,
     )(y_pred=y_pred, y=y)
 
 
 class DiceHelper:
     """
     Compute Dice score between two tensors `y_pred` and `y`.
-    `y_pred` must have N channels, `y` can be single-channel class indices or in the one-hot format.
+    `y_pred` and `y` can be single-channel class indices or in the one-hot format.
 
     Example:
 
     .. code-block:: python
 
         import torch
         from monai.metrics import DiceHelper
@@ -166,14 +179,15 @@
         include_background: bool | None = None,
         sigmoid: bool = False,
         softmax: bool | None = None,
         activate: bool = False,
         get_not_nans: bool = True,
         reduction: MetricReduction | str = MetricReduction.MEAN_BATCH,
         ignore_empty: bool = True,
+        num_classes: int | None = None,
     ) -> None:
         """
 
         Args:
             include_background: whether to skip the score on the first channel
                 (default to the value of `sigmoid`, False).
             sigmoid: whether ``y_pred`` are/will be sigmoid activated outputs. If True, thresholding at 0.5
@@ -182,22 +196,26 @@
                 get the discrete prediction. Defaults to the value of ``not sigmoid``.
             activate: whether to apply sigmoid to ``y_pred`` if ``sigmoid`` is True. Defaults to False.
                 This option is only valid when ``sigmoid`` is True.
             get_not_nans: whether to return the number of not-nan values.
             reduction: define mode of reduction to the metrics
             ignore_empty: if `True`, NaN value will be set for empty ground truth cases.
                 If `False`, 1 will be set if the Union of ``y_pred`` and ``y`` is empty.
+            num_classes: number of input channels (always including the background). When this is None,
+                ``y_pred.shape[1]`` will be used. This option is useful when both ``y_pred`` and ``y`` are
+                single-channel class indices and the number of classes is not automatically inferred from data.
         """
         self.sigmoid = sigmoid
         self.reduction = reduction
         self.get_not_nans = get_not_nans
         self.include_background = sigmoid if include_background is None else include_background
         self.softmax = not sigmoid if softmax is None else softmax
         self.activate = activate
         self.ignore_empty = ignore_empty
+        self.num_classes = num_classes
 
     def compute_channel(self, y_pred: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
         """"""
         y_o = torch.sum(y)
         if y_o > 0:
             return (2.0 * torch.sum(torch.masked_select(y, y_pred))) / (y_o + torch.sum(y_pred))
         if self.ignore_empty:
@@ -207,25 +225,31 @@
             return torch.tensor(1.0, device=y_o.device)
         return torch.tensor(0.0, device=y_o.device)
 
     def __call__(self, y_pred: torch.Tensor, y: torch.Tensor) -> torch.Tensor | tuple[torch.Tensor, torch.Tensor]:
         """
 
         Args:
-            y_pred: input predictions with shape (batch_size, num_classes, spatial_dims...).
-                the number of channels is inferred from ``y_pred.shape[1]``.
+            y_pred: input predictions with shape (batch_size, num_classes or 1, spatial_dims...).
+                the number of channels is inferred from ``y_pred.shape[1]`` when ``num_classes is None``.
             y: ground truth with shape (batch_size, num_classes or 1, spatial_dims...).
         """
-        n_pred_ch = y_pred.shape[1]
+        _softmax, _sigmoid = self.softmax, self.sigmoid
+        if self.num_classes is None:
+            n_pred_ch = y_pred.shape[1]  # y_pred is in one-hot format or multi-channel scores
+        else:
+            n_pred_ch = self.num_classes
+            if y_pred.shape[1] == 1 and self.num_classes > 1:  # y_pred is single-channel class indices
+                _softmax = _sigmoid = False
 
-        if self.softmax:
+        if _softmax:
             if n_pred_ch > 1:
                 y_pred = torch.argmax(y_pred, dim=1, keepdim=True)
 
-        elif self.sigmoid:
+        elif _sigmoid:
             if self.activate:
                 y_pred = torch.sigmoid(y_pred)
             y_pred = y_pred > 0.5
 
         first_ch = 0 if self.include_background else 1
         data = []
         for b in range(y_pred.shape[0]):
```

### Comparing `monai-weekly-1.2.dev2316/monai/metrics/meaniou.py` & `monai-weekly-1.2.dev2317/monai/metrics/meaniou.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/metrics/metric.py` & `monai-weekly-1.2.dev2317/monai/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/metrics/panoptic_quality.py` & `monai-weekly-1.2.dev2317/monai/metrics/panoptic_quality.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/metrics/regression.py` & `monai-weekly-1.2.dev2317/monai/metrics/regression.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 import math
 from abc import abstractmethod
-from collections.abc import Callable
+from collections.abc import Callable, Sequence
 from functools import partial
 from typing import Any
 
 import torch
 import torch.nn.functional as F
 
 from monai.metrics.utils import do_metric_reduction
-from monai.utils import MetricReduction
+from monai.utils import MetricReduction, StrEnum, convert_data_type, ensure_tuple_rep
 from monai.utils.type_conversion import convert_to_dst_type
 
 from .metric import CumulativeIterationMetric
 
 
 class RegressionMetric(CumulativeIterationMetric):
     """
@@ -228,162 +228,216 @@
 def compute_mean_error_metrics(y_pred: torch.Tensor, y: torch.Tensor, func: Callable) -> torch.Tensor:
     # reducing in only channel + spatial dimensions (not batch)
     # reduction of batch handled inside __call__() using do_metric_reduction() in respective calling class
     flt = partial(torch.flatten, start_dim=1)
     return torch.mean(flt(func(y - y_pred)), dim=-1, keepdim=True)
 
 
+class KernelType(StrEnum):
+    GAUSSIAN = "gaussian"
+    UNIFORM = "uniform"
+
+
 class SSIMMetric(RegressionMetric):
     r"""
-    Build a Pytorch version of the SSIM metric based on the original formula of SSIM
+    Computes the Structural Similarity Index Measure (SSIM).
 
     .. math::
         \operatorname {SSIM}(x,y) =\frac {(2 \mu_x \mu_y + c_1)(2 \sigma_{xy} + c_2)}{((\mu_x^2 + \
                 \mu_y^2 + c_1)(\sigma_x^2 + \sigma_y^2 + c_2)}
 
     For more info, visit
         https://vicuesoft.com/glossary/term/ssim-ms-ssim/
 
-    Modified and adopted from:
-        https://github.com/facebookresearch/fastMRI/blob/main/banding_removal/fastmri/ssim_loss_mixin.py
-
     SSIM reference paper:
         Wang, Zhou, et al. "Image quality assessment: from error visibility to structural
         similarity." IEEE transactions on image processing 13.4 (2004): 600-612.
 
     Args:
-        data_range: dynamic range of the data
-        win_size: gaussian weighting window size
+        spatial_dims: number of spatial dimensions of the input images.
+        data_range: value range of input images. (usually 1.0 or 255)
+        kernel_type: type of kernel, can be "gaussian" or "uniform".
+        win_size: window size of kernel
+        kernel_sigma: standard deviation for Gaussian kernel.
         k1: stability constant used in the luminance denominator
         k2: stability constant used in the contrast denominator
-        spatial_dims: if 2, input shape is expected to be (B,C,W,H). if 3, it is expected to be (B,C,W,H,D)
         reduction: define the mode to reduce metrics, will only execute reduction on `not-nan` values,
             available reduction modes: {``"none"``, ``"mean"``, ``"sum"``, ``"mean_batch"``, ``"sum_batch"``,
             ``"mean_channel"``, ``"sum_channel"``}, default to ``"mean"``. if "none", will not do reduction
         get_not_nans: whether to return the `not_nans` count, if True, aggregate() returns (metric, not_nans)
     """
 
     def __init__(
         self,
-        data_range: torch.Tensor,
-        win_size: int = 7,
+        spatial_dims: int,
+        data_range: float = 1.0,
+        kernel_type: KernelType | str = KernelType.GAUSSIAN,
+        win_size: int | Sequence[int] = 11,
+        kernel_sigma: float | Sequence[float] = 1.5,
         k1: float = 0.01,
         k2: float = 0.03,
-        spatial_dims: int = 2,
         reduction: MetricReduction | str = MetricReduction.MEAN,
         get_not_nans: bool = False,
-    ):
+    ) -> None:
         super().__init__(reduction=reduction, get_not_nans=get_not_nans)
-        self.data_range = data_range
-        self.win_size = win_size
-        self.k1, self.k2 = k1, k2
+
         self.spatial_dims = spatial_dims
-        self.cov_norm = (win_size**2) / (win_size**2 - 1)
-        self.w = torch.ones([1, 1] + [win_size for _ in range(spatial_dims)]) / win_size**spatial_dims
+        self.data_range = data_range
+        self.kernel_type = kernel_type
 
-    def _compute_intermediate_statistics(self, x: torch.Tensor, y: torch.Tensor) -> tuple[torch.Tensor, ...]:
-        data_range = self.data_range[(None,) * (self.spatial_dims + 2)]
-        # determine whether to work with 2D convolution or 3D
-        conv = getattr(F, f"conv{self.spatial_dims}d")
-        w = convert_to_dst_type(src=self.w, dst=x)[0]
-
-        c1 = (self.k1 * data_range) ** 2  # stability constant for luminance
-        c2 = (self.k2 * data_range) ** 2  # stability constant for contrast
-        ux = conv(x, w)  # mu_x
-        uy = conv(y, w)  # mu_y
-        uxx = conv(x * x, w)  # mu_x^2
-        uyy = conv(y * y, w)  # mu_y^2
-        uxy = conv(x * y, w)  # mu_xy
-        vx = self.cov_norm * (uxx - ux * ux)  # sigma_x
-        vy = self.cov_norm * (uyy - uy * uy)  # sigma_y
-        vxy = self.cov_norm * (uxy - ux * uy)  # sigma_xy
+        if not isinstance(win_size, Sequence):
+            win_size = ensure_tuple_rep(win_size, spatial_dims)
+        self.kernel_size = win_size
+
+        if not isinstance(kernel_sigma, Sequence):
+            kernel_sigma = ensure_tuple_rep(kernel_sigma, spatial_dims)
+        self.kernel_sigma = kernel_sigma
 
-        return c1, c2, ux, uy, vx, vy, vxy
+        self.k1 = k1
+        self.k2 = k2
 
-    def _compute_metric(self, x: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
+    def _compute_metric(self, y_pred: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
         """
         Args:
-            x: first sample (e.g., the reference image). Its shape is (B,C,W,H) for 2D data and (B,C,W,H,D) for 3D.
-                A fastMRI sample should use the 2D format with C being the number of slices.
-            y: second sample (e.g., the reconstructed image). It has similar shape as x
-
-        Returns:
-            ssim_value
-
-        Example:
-            .. code-block:: python
-
-                import torch
-                x = torch.ones([1,1,10,10])/2 # ground truth
-                y = torch.ones([1,1,10,10])/2 # prediction
-                data_range = x.max().unsqueeze(0)
-                # the following line should print 1.0 (or 0.9999)
-                print(SSIMMetric(data_range=data_range,spatial_dims=2)._compute_metric(x,y))
+            y_pred: Predicted image.
+                It must be a 2D or 3D batch-first tensor [B,C,H,W] or [B,C,H,W,D].
+            y: Reference image.
+                It must be a 2D or 3D batch-first tensor [B,C,H,W] or [B,C,H,W,D].
+
+        Raises:
+            ValueError: when `y_pred` is not a 2D or 3D image.
         """
-        if x.shape[1] > 1:  # handling multiple channels (C>1)
-            if x.shape[1] != y.shape[1]:
-                raise ValueError(
-                    f"x and y should have the same number of channels, "
-                    f"but x has {x.shape[1]} channels and y has {y.shape[1]} channels."
-                )
-
-            ssim = torch.stack(
-                [
-                    SSIMMetric(self.data_range, self.win_size, self.k1, self.k2, self.spatial_dims)(  # type: ignore[misc]
-                        x[:, i, ...].unsqueeze(1), y[:, i, ...].unsqueeze(1)
-                    )
-                    for i in range(x.shape[1])
-                ]
+        dims = y_pred.ndimension()
+        if self.spatial_dims == 2 and dims != 4:
+            raise ValueError(
+                f"y_pred should have 4 dimensions (batch, channel, height, width) when using {self.spatial_dims} "
+                f"spatial dimensions, got {dims}."
             )
-            channel_wise_ssim = ssim.mean(1).view(-1, 1)
-            return channel_wise_ssim
 
-        c1, c2, ux, uy, vx, vy, vxy = self._compute_intermediate_statistics(x, y)
+        if self.spatial_dims == 3 and dims != 5:
+            raise ValueError(
+                f"y_pred should have 4 dimensions (batch, channel, height, width, depth) when using {self.spatial_dims}"
+                f" spatial dimensions, got {dims}."
+            )
 
-        numerator = (2 * ux * uy + c1) * (2 * vxy + c2)
-        denom = (ux**2 + uy**2 + c1) * (vx + vy + c2)
-        ssim_value = numerator / denom
-        # [B, 1]
-        ssim_per_batch: torch.Tensor = ssim_value.view(ssim_value.shape[1], -1).mean(1, keepdim=True)
+        ssim_value_full_image, _ = compute_ssim_and_cs(
+            y_pred=y_pred,
+            y=y,
+            spatial_dims=self.spatial_dims,
+            data_range=self.data_range,
+            kernel_type=self.kernel_type,
+            kernel_size=self.kernel_size,
+            kernel_sigma=self.kernel_sigma,
+            k1=self.k1,
+            k2=self.k2,
+        )
+
+        ssim_per_batch: torch.Tensor = ssim_value_full_image.view(ssim_value_full_image.shape[0], -1).mean(
+            1, keepdim=True
+        )
 
         return ssim_per_batch
 
-    def _compute_metric_and_contrast(self, x: torch.Tensor, y: torch.Tensor) -> tuple[torch.Tensor, torch.Tensor]:
-        """
-        Args:
-            x: first sample (e.g., the reference image). Its shape is (B,C,W,H) for 2D data and (B,C,W,H,D) for 3D.
-                A fastMRI sample should use the 2D format with C being the number of slices.
-            y: second sample (e.g., the reconstructed image). It has similar shape as x
 
-        Returns:
-            ssim_value, cs_value
+def _gaussian_kernel(
+    spatial_dims: int, num_channels: int, kernel_size: Sequence[int], kernel_sigma: Sequence[float]
+) -> torch.Tensor:
+    """Computes 2D or 3D gaussian kernel.
+
+    Args:
+        spatial_dims: number of spatial dimensions of the input images.
+        num_channels: number of channels in the image
+        kernel_size: size of kernel
+        kernel_sigma: standard deviation for Gaussian kernel.
+    """
+
+    def gaussian_1d(kernel_size: int, sigma: float) -> torch.Tensor:
+        """Computes 1D gaussian kernel.
+
+        Args:
+            kernel_size: size of the gaussian kernel
+            sigma: Standard deviation of the gaussian kernel
         """
-        if x.shape[1] > 1:  # handling multiple channels (C>1)
-            if x.shape[1] != y.shape[1]:
-                raise ValueError(
-                    f"x and y should have the same number of channels, "
-                    f"but x has {x.shape[1]} channels and y has {y.shape[1]} channels."
-                )
-
-            ssim_ls = []
-            cs_ls = []
-            for i in range(x.shape[1]):
-                ssim_val, cs_val = SSIMMetric(
-                    self.data_range, self.win_size, self.k1, self.k2, self.spatial_dims
-                )._compute_metric_and_contrast(x[:, i, ...].unsqueeze(1), y[:, i, ...].unsqueeze(1))
-                ssim_ls.append(ssim_val)
-                cs_ls.append(cs_val)
-            channel_wise_ssim: torch.Tensor = torch.stack(ssim_ls).mean(1).view(-1, 1)
-            channel_wise_cs: torch.Tensor = torch.stack(cs_ls).mean(1).view(-1, 1)
-            return channel_wise_ssim, channel_wise_cs
-
-        c1, c2, ux, uy, vx, vy, vxy = self._compute_intermediate_statistics(x, y)
-
-        numerator = (2 * ux * uy + c1) * (2 * vxy + c2)
-        denom = (ux**2 + uy**2 + c1) * (vx + vy + c2)
-        ssim_value = numerator / denom
-        # [B, 1]
-        ssim_per_batch: torch.Tensor = ssim_value.view(ssim_value.shape[1], -1).mean(1, keepdim=True)
-
-        cs_per_batch: torch.Tensor = (2 * vxy + c2) / (vx + vy + c2)  # contrast sensitivity function
-        cs_per_batch = cs_per_batch.view(cs_per_batch.shape[0], -1).mean(1, keepdim=True)  # [B, 1]
-        return ssim_per_batch, cs_per_batch
+        dist = torch.arange(start=(1 - kernel_size) / 2, end=(1 + kernel_size) / 2, step=1)
+        gauss = torch.exp(-torch.pow(dist / sigma, 2) / 2)
+        return (gauss / gauss.sum()).unsqueeze(dim=0)
+
+    gaussian_kernel_x = gaussian_1d(kernel_size[0], kernel_sigma[0])
+    gaussian_kernel_y = gaussian_1d(kernel_size[1], kernel_sigma[1])
+    kernel = torch.matmul(gaussian_kernel_x.t(), gaussian_kernel_y)  # (kernel_size, 1) * (1, kernel_size)
+
+    kernel_dimensions: tuple[int, ...] = (num_channels, 1, kernel_size[0], kernel_size[1])
+
+    if spatial_dims == 3:
+        gaussian_kernel_z = gaussian_1d(kernel_size[2], kernel_sigma[2])[None,]
+        kernel = torch.mul(
+            kernel.unsqueeze(-1).repeat(1, 1, kernel_size[2]),
+            gaussian_kernel_z.expand(kernel_size[0], kernel_size[1], kernel_size[2]),
+        )
+        kernel_dimensions = (num_channels, 1, kernel_size[0], kernel_size[1], kernel_size[2])
+
+    return kernel.expand(kernel_dimensions)
+
+
+def compute_ssim_and_cs(
+    y_pred: torch.Tensor,
+    y: torch.Tensor,
+    spatial_dims: int,
+    kernel_size: Sequence[int],
+    kernel_sigma: Sequence[float],
+    data_range: float = 1.0,
+    kernel_type: KernelType | str = KernelType.GAUSSIAN,
+    k1: float = 0.01,
+    k2: float = 0.03,
+) -> tuple[torch.Tensor, torch.Tensor]:
+    """
+    Function to compute the Structural Similarity Index Measure (SSIM) and Contrast Sensitivity (CS) for a batch
+    of images.
+
+    Args:
+        y_pred: batch of predicted images with shape (batch_size, channels, spatial_dim1, spatial_dim2[, spatial_dim3])
+        y: batch of target images with shape (batch_size, channels, spatial_dim1, spatial_dim2[, spatial_dim3])
+        kernel_size: the size of the kernel to use for the SSIM computation.
+        kernel_sigma: the standard deviation of the kernel to use for the SSIM computation.
+        spatial_dims: number of spatial dimensions of the images (2, 3)
+        data_range: the data range of the images.
+        kernel_type: the type of kernel to use for the SSIM computation. Can be either "gaussian" or "uniform".
+        k1: the first stability constant.
+        k2: the second stability constant.
+
+    Returns:
+        ssim: the Structural Similarity Index Measure score for the batch of images.
+        cs: the Contrast Sensitivity for the batch of images.
+    """
+    if y.shape != y_pred.shape:
+        raise ValueError(f"y_pred and y should have same shapes, got {y_pred.shape} and {y.shape}.")
+
+    y_pred = convert_data_type(y_pred, output_type=torch.Tensor, dtype=torch.float)[0]
+    y = convert_data_type(y, output_type=torch.Tensor, dtype=torch.float)[0]
+
+    num_channels = y_pred.size(1)
+
+    if kernel_type == KernelType.GAUSSIAN:
+        kernel = _gaussian_kernel(spatial_dims, num_channels, kernel_size, kernel_sigma)
+    elif kernel_type == KernelType.UNIFORM:
+        kernel = torch.ones((num_channels, 1, *kernel_size)) / torch.prod(torch.tensor(kernel_size))
+
+    kernel = convert_to_dst_type(src=kernel, dst=y_pred)[0]
+
+    c1 = (k1 * data_range) ** 2  # stability constant for luminance
+    c2 = (k2 * data_range) ** 2  # stability constant for contrast
+
+    conv_fn = getattr(F, f"conv{spatial_dims}d")
+    mu_x = conv_fn(y_pred, kernel, groups=num_channels)
+    mu_y = conv_fn(y, kernel, groups=num_channels)
+    mu_xx = conv_fn(y_pred * y_pred, kernel, groups=num_channels)
+    mu_yy = conv_fn(y * y, kernel, groups=num_channels)
+    mu_xy = conv_fn(y_pred * y, kernel, groups=num_channels)
+
+    sigma_x = mu_xx - mu_x * mu_x
+    sigma_y = mu_yy - mu_y * mu_y
+    sigma_xy = mu_xy - mu_x * mu_y
+
+    contrast_sensitivity = (2 * sigma_xy + c2) / (sigma_x + sigma_y + c2)
+    ssim_value_full_image = ((2 * mu_x * mu_y + c1) / (mu_x**2 + mu_y**2 + c1)) * contrast_sensitivity
+
+    return ssim_value_full_image, contrast_sensitivity
```

### Comparing `monai-weekly-1.2.dev2316/monai/metrics/rocauc.py` & `monai-weekly-1.2.dev2317/monai/metrics/rocauc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/metrics/surface_dice.py` & `monai-weekly-1.2.dev2317/monai/metrics/surface_dice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/metrics/surface_distance.py` & `monai-weekly-1.2.dev2317/monai/metrics/surface_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/metrics/utils.py` & `monai-weekly-1.2.dev2317/monai/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/metrics/wrapper.py` & `monai-weekly-1.2.dev2317/monai/metrics/wrapper.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/__init__.py` & `monai-weekly-1.2.dev2317/monai/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/blocks/__init__.py` & `monai-weekly-1.2.dev2317/monai/networks/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/blocks/acti_norm.py` & `monai-weekly-1.2.dev2317/monai/networks/blocks/acti_norm.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/blocks/activation.py` & `monai-weekly-1.2.dev2317/monai/networks/blocks/activation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/blocks/aspp.py` & `monai-weekly-1.2.dev2317/monai/networks/blocks/aspp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/blocks/backbone_fpn_utils.py` & `monai-weekly-1.2.dev2317/monai/networks/blocks/backbone_fpn_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/blocks/convolutions.py` & `monai-weekly-1.2.dev2317/monai/networks/blocks/convolutions.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/blocks/crf.py` & `monai-weekly-1.2.dev2317/monai/networks/blocks/crf.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/blocks/denseblock.py` & `monai-weekly-1.2.dev2317/monai/networks/blocks/denseblock.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/blocks/dints_block.py` & `monai-weekly-1.2.dev2317/monai/networks/blocks/dints_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/blocks/downsample.py` & `monai-weekly-1.2.dev2317/monai/networks/blocks/downsample.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/blocks/dynunet_block.py` & `monai-weekly-1.2.dev2317/monai/networks/blocks/dynunet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/blocks/encoder.py` & `monai-weekly-1.2.dev2317/monai/networks/blocks/encoder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/blocks/fcn.py` & `monai-weekly-1.2.dev2317/monai/networks/blocks/fcn.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/blocks/feature_pyramid_network.py` & `monai-weekly-1.2.dev2317/monai/networks/blocks/feature_pyramid_network.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/blocks/fft_utils_t.py` & `monai-weekly-1.2.dev2317/monai/networks/blocks/fft_utils_t.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/blocks/localnet_block.py` & `monai-weekly-1.2.dev2317/monai/networks/blocks/localnet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/blocks/mlp.py` & `monai-weekly-1.2.dev2317/monai/networks/blocks/mlp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/blocks/patchembedding.py` & `monai-weekly-1.2.dev2317/monai/networks/blocks/patchembedding.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/blocks/regunet_block.py` & `monai-weekly-1.2.dev2317/monai/networks/blocks/regunet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/blocks/segresnet_block.py` & `monai-weekly-1.2.dev2317/monai/networks/blocks/segresnet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/blocks/selfattention.py` & `monai-weekly-1.2.dev2317/monai/networks/blocks/selfattention.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/blocks/squeeze_and_excitation.py` & `monai-weekly-1.2.dev2317/monai/networks/blocks/squeeze_and_excitation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/blocks/text_embedding.py` & `monai-weekly-1.2.dev2317/monai/networks/blocks/text_embedding.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/blocks/transformerblock.py` & `monai-weekly-1.2.dev2317/monai/networks/blocks/transformerblock.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/blocks/unetr_block.py` & `monai-weekly-1.2.dev2317/monai/networks/blocks/unetr_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/blocks/upsample.py` & `monai-weekly-1.2.dev2317/monai/networks/blocks/upsample.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/blocks/warp.py` & `monai-weekly-1.2.dev2317/monai/networks/blocks/warp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/layers/__init__.py` & `monai-weekly-1.2.dev2317/monai/networks/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/layers/convutils.py` & `monai-weekly-1.2.dev2317/monai/networks/layers/convutils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/layers/drop_path.py` & `monai-weekly-1.2.dev2317/monai/networks/layers/drop_path.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/layers/factories.py` & `monai-weekly-1.2.dev2317/monai/networks/layers/factories.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,18 +63,17 @@
 
 import warnings
 from collections.abc import Callable
 from typing import Any
 
 import torch.nn as nn
 
+from monai.networks.utils import has_nvfuser_instance_norm
 from monai.utils import look_up_option, optional_import
 
-InstanceNorm3dNVFuser, has_nvfuser = optional_import("apex.normalization", name="InstanceNorm3dNVFuser")
-
 __all__ = ["LayerFactory", "Dropout", "Norm", "Act", "Conv", "Pool", "Pad", "split_args"]
 
 
 class LayerFactory:
     """
     Factory object for creating layers, this uses given factory functions to actually produce the types or constructing
     callables. These functions are referred to by name and can be added at any time.
@@ -263,20 +262,20 @@
     """
 
     if dim != 3:
         types = (nn.InstanceNorm1d, nn.InstanceNorm2d)
         warnings.warn(f"`InstanceNorm3dNVFuser` only supports 3d cases, use {types[dim - 1]} instead.")
         return types[dim - 1]
 
-    if not has_nvfuser:
+    if not has_nvfuser_instance_norm():
         warnings.warn(
             "`apex.normalization.InstanceNorm3dNVFuser` is not installed properly, use nn.InstanceNorm3d instead."
         )
         return nn.InstanceNorm3d
-    return InstanceNorm3dNVFuser
+    return optional_import("apex.normalization", name="InstanceNorm3dNVFuser")[0]
 
 
 Act.add_factory_callable("elu", lambda: nn.modules.ELU)
 Act.add_factory_callable("relu", lambda: nn.modules.ReLU)
 Act.add_factory_callable("leakyrelu", lambda: nn.modules.LeakyReLU)
 Act.add_factory_callable("prelu", lambda: nn.modules.PReLU)
 Act.add_factory_callable("relu6", lambda: nn.modules.ReLU6)
```

### Comparing `monai-weekly-1.2.dev2316/monai/networks/layers/filtering.py` & `monai-weekly-1.2.dev2317/monai/networks/layers/filtering.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/layers/gmm.py` & `monai-weekly-1.2.dev2317/monai/networks/layers/gmm.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/layers/simplelayers.py` & `monai-weekly-1.2.dev2317/monai/networks/layers/simplelayers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/layers/spatial_transforms.py` & `monai-weekly-1.2.dev2317/monai/networks/layers/spatial_transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/layers/utils.py` & `monai-weekly-1.2.dev2317/monai/networks/layers/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/layers/weight_init.py` & `monai-weekly-1.2.dev2317/monai/networks/layers/weight_init.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/nets/__init__.py` & `monai-weekly-1.2.dev2317/monai/networks/nets/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/nets/ahnet.py` & `monai-weekly-1.2.dev2317/monai/networks/nets/ahnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/nets/attentionunet.py` & `monai-weekly-1.2.dev2317/monai/networks/nets/attentionunet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/nets/autoencoder.py` & `monai-weekly-1.2.dev2317/monai/networks/nets/autoencoder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/nets/basic_unet.py` & `monai-weekly-1.2.dev2317/monai/networks/nets/basic_unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/nets/basic_unetplusplus.py` & `monai-weekly-1.2.dev2317/monai/networks/nets/basic_unetplusplus.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/nets/classifier.py` & `monai-weekly-1.2.dev2317/monai/networks/nets/classifier.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/nets/densenet.py` & `monai-weekly-1.2.dev2317/monai/networks/nets/densenet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/nets/dints.py` & `monai-weekly-1.2.dev2317/monai/networks/nets/dints.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/nets/dynunet.py` & `monai-weekly-1.2.dev2317/monai/networks/nets/dynunet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/nets/efficientnet.py` & `monai-weekly-1.2.dev2317/monai/networks/nets/efficientnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/nets/flexible_unet.py` & `monai-weekly-1.2.dev2317/monai/networks/nets/flexible_unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/nets/fullyconnectednet.py` & `monai-weekly-1.2.dev2317/monai/networks/nets/fullyconnectednet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/nets/generator.py` & `monai-weekly-1.2.dev2317/monai/networks/nets/generator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/nets/highresnet.py` & `monai-weekly-1.2.dev2317/monai/networks/nets/highresnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/nets/hovernet.py` & `monai-weekly-1.2.dev2317/monai/networks/nets/hovernet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/nets/milmodel.py` & `monai-weekly-1.2.dev2317/monai/networks/nets/milmodel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/nets/netadapter.py` & `monai-weekly-1.2.dev2317/monai/networks/nets/netadapter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/nets/regressor.py` & `monai-weekly-1.2.dev2317/monai/networks/nets/regressor.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/nets/regunet.py` & `monai-weekly-1.2.dev2317/monai/networks/nets/regunet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/nets/resnet.py` & `monai-weekly-1.2.dev2317/monai/networks/nets/resnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/nets/segresnet.py` & `monai-weekly-1.2.dev2317/monai/networks/nets/segresnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/nets/segresnet_ds.py` & `monai-weekly-1.2.dev2317/monai/networks/nets/segresnet_ds.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/nets/senet.py` & `monai-weekly-1.2.dev2317/monai/networks/nets/senet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/nets/swin_unetr.py` & `monai-weekly-1.2.dev2317/monai/networks/nets/swin_unetr.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/nets/torchvision_fc.py` & `monai-weekly-1.2.dev2317/monai/networks/nets/torchvision_fc.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,16 +110,18 @@
         fc_name: str = "fc",
         node_name: str = "",
         weights=None,
         **kwargs,
     ):
         if weights is not None:
             model = getattr(models, model_name)(weights=weights, **kwargs)
+        elif pretrained:
+            model = getattr(models, model_name)(weights="DEFAULT", **kwargs)
         else:
-            model = getattr(models, model_name)(pretrained=pretrained, **kwargs)  # 'pretrained' deprecated 0.13
+            model = getattr(models, model_name)(weights=None, **kwargs)
 
         super().__init__(
             model=model,
             num_classes=num_classes,
             dim=dim,
             in_channels=in_channels,
             use_conv=use_conv,
```

### Comparing `monai-weekly-1.2.dev2316/monai/networks/nets/transchex.py` & `monai-weekly-1.2.dev2317/monai/networks/nets/transchex.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/nets/unet.py` & `monai-weekly-1.2.dev2317/monai/networks/nets/unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/nets/unetr.py` & `monai-weekly-1.2.dev2317/monai/networks/nets/unetr.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/nets/varautoencoder.py` & `monai-weekly-1.2.dev2317/monai/networks/nets/varautoencoder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/nets/vit.py` & `monai-weekly-1.2.dev2317/monai/networks/nets/vit.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/nets/vitautoenc.py` & `monai-weekly-1.2.dev2317/monai/networks/nets/vitautoenc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/nets/vnet.py` & `monai-weekly-1.2.dev2317/monai/networks/nets/vnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/networks/utils.py` & `monai-weekly-1.2.dev2317/monai/networks/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,18 +23,18 @@
 from copy import deepcopy
 from typing import Any
 
 import numpy as np
 import torch
 import torch.nn as nn
 
-from monai.apps.utils import get_logger, optional_import
+from monai.apps.utils import get_logger
 from monai.config import PathLike
 from monai.utils.misc import ensure_tuple, save_obj, set_determinism
-from monai.utils.module import look_up_option, pytorch_after
+from monai.utils.module import look_up_option, optional_import, pytorch_after
 from monai.utils.type_conversion import convert_to_dst_type, convert_to_tensor
 
 onnx, _ = optional_import("onnx")
 onnxreference, _ = optional_import("onnx.reference")
 onnxruntime, _ = optional_import("onnxruntime")
 
 __all__ = [
@@ -55,18 +55,41 @@
     "convert_to_trt",
     "meshgrid_ij",
     "meshgrid_xy",
     "replace_modules",
     "replace_modules_temp",
     "look_up_named_module",
     "set_named_module",
+    "has_nvfuser_instance_norm",
 ]
 
 logger = get_logger(module_name=__name__)
 
+_has_nvfuser = None
+
+
+def has_nvfuser_instance_norm():
+    """whether the current environment has InstanceNorm3dNVFuser
+    https://github.com/NVIDIA/apex/blob/23.05-devel/apex/normalization/instance_norm.py#L15-L16
+    """
+    global _has_nvfuser
+    if _has_nvfuser is not None:
+        return _has_nvfuser
+
+    _, _has_nvfuser = optional_import("apex.normalization", name="InstanceNorm3dNVFuser")
+    if not _has_nvfuser:
+        return False
+    try:
+        import importlib
+
+        importlib.import_module("instance_norm_nvfuser_cuda")
+    except ImportError:
+        _has_nvfuser = False
+    return _has_nvfuser
+
 
 def look_up_named_module(name: str, mod, print_all_options=False):
     """
     get the named module in `mod` by the attribute name,
     for example ``look_up_named_module(net, "features.3.1.attn")``
 
     Args:
@@ -886,15 +909,15 @@
 
     if not input_shape:
         raise ValueError("Missing the input shape for model convert.")
 
     if not dynamic_batchsize:
         warnings.warn(f"There is no dynamic batch range. The converted model only takes {input_shape} shape input.")
 
-    if (not (dynamic_batchsize is None)) and (len(dynamic_batchsize) != 3):
+    if (dynamic_batchsize is not None) and (len(dynamic_batchsize) != 3):
         warnings.warn(f"The dynamic batch range sequence should have 3 elements, but got {dynamic_batchsize} elements.")
 
     device = device if device else 0
     target_device = torch.device(f"cuda:{device}") if device else torch.device("cuda:0")
     convert_precision = torch.float32 if precision == "fp32" else torch.half
     inputs = [torch.rand(ensure_tuple(input_shape)).to(target_device)]
```

### Comparing `monai-weekly-1.2.dev2316/monai/optimizers/__init__.py` & `monai-weekly-1.2.dev2317/monai/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/optimizers/lr_finder.py` & `monai-weekly-1.2.dev2317/monai/optimizers/lr_finder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/optimizers/lr_scheduler.py` & `monai-weekly-1.2.dev2317/monai/optimizers/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/optimizers/novograd.py` & `monai-weekly-1.2.dev2317/monai/optimizers/novograd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/optimizers/utils.py` & `monai-weekly-1.2.dev2317/monai/optimizers/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/transforms/__init__.py` & `monai-weekly-1.2.dev2317/monai/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/transforms/adaptors.py` & `monai-weekly-1.2.dev2317/monai/transforms/adaptors.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/transforms/compose.py` & `monai-weekly-1.2.dev2317/monai/transforms/compose.py`

 * *Files 0% similar despite different names*

```diff
@@ -370,15 +370,15 @@
             if not isinstance(_transform, Randomizable):
                 continue
             try:
                 _transform.randomize(data)
             except TypeError as type_error:
                 tfm_name: str = type(_transform).__name__
                 warnings.warn(
-                    f'Transform "{tfm_name}" in Compose not randomized\n{tfm_name}.{type_error}.', RuntimeWarning
+                    f"Transform '{tfm_name}' in Compose not randomized\n{tfm_name}.{type_error}.", RuntimeWarning
                 )
 
     def get_index_of_first(self, predicate):
         """
         get_index_of_first takes a ``predicate`` and returns the index of the first transform that
         satisfies the predicate (ie. makes the predicate return True). If it is unable to find
         a transform that satisfies the ``predicate``, it returns None.
@@ -466,14 +466,19 @@
     def inverse(self, data):
         invertible_transforms = [t for t in self.flatten().transforms if isinstance(t, InvertibleTransform)]
         if not invertible_transforms:
             warnings.warn("inverse has been called but no invertible transforms have been supplied")
 
         # loop backwards over transforms
         for t in reversed(invertible_transforms):
+            if isinstance(t, LazyTransform) and t.lazy_evaluation:
+                warnings.warn(
+                    f"inversing {t.__class__.__name__} lazily may not implemented"
+                    "please set `lazy_evaluation=False` before calling inverse."
+                )
             data = apply_transform(t.inverse, data, self.map_items, self.unpack_items, self.log_stats)
         return data
 
 
 class OneOf(Compose):
     """
     ``OneOf`` provides the ability to randomly choose one transform out of a
```

### Comparing `monai-weekly-1.2.dev2316/monai/transforms/croppad/__init__.py` & `monai-weekly-1.2.dev2317/monai/transforms/croppad/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/transforms/croppad/array.py` & `monai-weekly-1.2.dev2317/monai/transforms/croppad/array.py`

 * *Files 2% similar despite different names*

```diff
@@ -812,14 +812,26 @@
         )
         ret = self.padder.__call__(img=cropped, to_pad=pad_width, mode=mode, **pad_kwargs)
         # combine the traced cropping and padding into one transformation
         # by taking the padded info and placing it in a key inside the crop info.
         if get_track_meta() and isinstance(ret, MetaTensor):
             if not self.lazy_evaluation:
                 ret.applied_operations[-1][TraceKeys.EXTRA_INFO]["pad_info"] = ret.applied_operations.pop()
+            else:
+                pad_info = ret.pending_operations.pop()
+                crop_info = ret.pending_operations.pop()
+                extra = crop_info[TraceKeys.EXTRA_INFO]
+                extra["pad_info"] = pad_info
+                self.push_transform(
+                    ret,
+                    orig_size=crop_info.get(TraceKeys.ORIG_SIZE),
+                    sp_size=pad_info[LazyAttr.SHAPE],
+                    affine=crop_info[LazyAttr.AFFINE] @ pad_info[LazyAttr.AFFINE],
+                    extra_info=extra,
+                )
         return ret
 
     def __call__(  # type: ignore[override]
         self, img: torch.Tensor, mode: str | None = None, **pad_kwargs
     ) -> torch.Tensor:
         """
         Apply the transform to `img`, assuming `img` is channel-first and
```

### Comparing `monai-weekly-1.2.dev2316/monai/transforms/croppad/batch.py` & `monai-weekly-1.2.dev2317/monai/transforms/croppad/batch.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/transforms/croppad/dictionary.py` & `monai-weekly-1.2.dev2317/monai/transforms/croppad/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/transforms/croppad/functional.py` & `monai-weekly-1.2.dev2317/monai/transforms/croppad/functional.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/transforms/intensity/__init__.py` & `monai-weekly-1.2.dev2317/monai/transforms/intensity/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/transforms/intensity/array.py` & `monai-weekly-1.2.dev2317/monai/transforms/intensity/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/transforms/intensity/dictionary.py` & `monai-weekly-1.2.dev2317/monai/transforms/intensity/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/transforms/inverse.py` & `monai-weekly-1.2.dev2317/monai/transforms/inverse.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,17 +119,18 @@
                 xform = self.pop_transform(data, check=False) if do_transform else {}
                 meta_obj = self.push_transform(data, orig_size=xform.get(TraceKeys.ORIG_SIZE), extra_info=xform)
                 return data.copy_meta_from(meta_obj)
             if do_transform:
                 xform = data.pending_operations.pop()
                 extra = xform.copy()
                 xform.update(transform_info)
-                meta_obj = self.push_transform(data, transform_info=xform, lazy_evaluation=lazy_eval, extra_info=extra)
-                return data.copy_meta_from(meta_obj)
-            return data
+            else:  # lazy, replace=True, do_transform=False
+                xform, extra = transform_info, {}
+            meta_obj = self.push_transform(data, transform_info=xform, lazy_evaluation=True, extra_info=extra)
+            return data.copy_meta_from(meta_obj)
         kwargs["lazy_evaluation"] = lazy_eval
         if "transform_info" in kwargs and isinstance(kwargs["transform_info"], dict):
             kwargs["transform_info"].update(transform_info)
         else:
             kwargs["transform_info"] = transform_info
         meta_obj = TraceableTransform.track_transform_meta(data, *args, **kwargs)
         return data.copy_meta_from(meta_obj) if isinstance(data, MetaTensor) else data
@@ -207,24 +208,34 @@
             extra_info.pop(LazyAttr.AFFINE, None)
             info[TraceKeys.EXTRA_INFO] = extra_info
 
         # push the transform info to the applied_operation or pending_operation stack
         if lazy_evaluation:
             if sp_size is None:
                 if LazyAttr.SHAPE not in info:
-                    warnings.warn("spatial size is None in push transform.")
+                    info[LazyAttr.SHAPE] = info.get(TraceKeys.ORIG_SIZE, [])
             else:
-                info[LazyAttr.SHAPE] = tuple(convert_to_numpy(sp_size, wrap_sequence=True).tolist())
+                info[LazyAttr.SHAPE] = sp_size
+            info[LazyAttr.SHAPE] = tuple(convert_to_numpy(info[LazyAttr.SHAPE], wrap_sequence=True).tolist())
             if affine is None:
                 if LazyAttr.AFFINE not in info:
-                    warnings.warn("affine is None in push transform.")
+                    info[LazyAttr.AFFINE] = MetaTensor.get_default_affine()
             else:
-                info[LazyAttr.AFFINE] = convert_to_tensor(affine, device=torch.device("cpu"))
+                info[LazyAttr.AFFINE] = affine
+            info[LazyAttr.AFFINE] = convert_to_tensor(info[LazyAttr.AFFINE], device=torch.device("cpu"))
             out_obj.push_pending_operation(info)
         else:
+            if out_obj.pending_operations:
+                transform_name = info.get(TraceKeys.CLASS_NAME, "") if isinstance(info, dict) else ""
+                warnings.warn(
+                    f"Applying transform {transform_name} to a MetaTensor with pending operations "
+                    "is not supported (as this eventually changes the ordering of applied_operations when the pending "
+                    f"operations are executed). Please clear the pending operations before transform {transform_name}."
+                    f"\nPending operations: {[x.get(TraceKeys.CLASS_NAME) for x in out_obj.pending_operations]}."
+                )
             out_obj.push_applied_operation(info)
         if isinstance(data, Mapping):
             if not isinstance(data, dict):
                 data = dict(data)
             if isinstance(data_t, MetaTensor):
                 data[key] = data_t.copy_meta_from(out_obj)
             else:
```

### Comparing `monai-weekly-1.2.dev2316/monai/transforms/inverse_batch_transform.py` & `monai-weekly-1.2.dev2317/monai/transforms/inverse_batch_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/transforms/io/__init__.py` & `monai-weekly-1.2.dev2317/monai/transforms/io/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/transforms/io/array.py` & `monai-weekly-1.2.dev2317/monai/transforms/io/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/transforms/io/dictionary.py` & `monai-weekly-1.2.dev2317/monai/transforms/io/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/transforms/lazy/__init__.py` & `monai-weekly-1.2.dev2317/monai/transforms/lazy/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/transforms/lazy/functional.py` & `monai-weekly-1.2.dev2317/monai/transforms/lazy/functional.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/transforms/lazy/utils.py` & `monai-weekly-1.2.dev2317/monai/transforms/lazy/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/transforms/meta_utility/__init__.py` & `monai-weekly-1.2.dev2317/monai/transforms/meta_utility/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/transforms/meta_utility/dictionary.py` & `monai-weekly-1.2.dev2317/monai/transforms/meta_utility/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/transforms/nvtx.py` & `monai-weekly-1.2.dev2317/monai/transforms/nvtx.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/transforms/post/__init__.py` & `monai-weekly-1.2.dev2317/monai/transforms/post/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/transforms/post/array.py` & `monai-weekly-1.2.dev2317/monai/transforms/post/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/transforms/post/dictionary.py` & `monai-weekly-1.2.dev2317/monai/transforms/post/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/transforms/signal/__init__.py` & `monai-weekly-1.2.dev2317/monai/transforms/signal/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/transforms/signal/array.py` & `monai-weekly-1.2.dev2317/monai/transforms/signal/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/transforms/smooth_field/__init__.py` & `monai-weekly-1.2.dev2317/monai/transforms/smooth_field/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/transforms/smooth_field/array.py` & `monai-weekly-1.2.dev2317/monai/transforms/smooth_field/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/transforms/smooth_field/dictionary.py` & `monai-weekly-1.2.dev2317/monai/transforms/smooth_field/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/transforms/spatial/__init__.py` & `monai-weekly-1.2.dev2317/monai/transforms/spatial/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/transforms/spatial/array.py` & `monai-weekly-1.2.dev2317/monai/transforms/spatial/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/transforms/spatial/dictionary.py` & `monai-weekly-1.2.dev2317/monai/transforms/spatial/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/transforms/spatial/functional.py` & `monai-weekly-1.2.dev2317/monai/transforms/spatial/functional.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/transforms/traits.py` & `monai-weekly-1.2.dev2317/monai/transforms/traits.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/transforms/transform.py` & `monai-weekly-1.2.dev2317/monai/transforms/transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/transforms/utility/__init__.py` & `monai-weekly-1.2.dev2317/monai/transforms/utility/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/transforms/utility/array.py` & `monai-weekly-1.2.dev2317/monai/transforms/utility/array.py`

 * *Files 2% similar despite different names*

```diff
@@ -826,27 +826,32 @@
         lambd = Lambda(func=lambda x: x[:4, :, :])
         print(lambd(image).shape)
         (4, 2, 2)
 
     Args:
         func: Lambda/function to be applied.
         inv_func: Lambda/function of inverse operation, default to `lambda x: x`.
+        track_meta:  If `False`, then standard data objects will be returned (e.g., torch.Tensor` and `np.ndarray`)
+            as opposed to MONAI's enhanced objects. By default, this is `True`.
 
     Raises:
         TypeError: When ``func`` is not an ``Optional[Callable]``.
 
     """
 
     backend = [TransformBackends.TORCH, TransformBackends.NUMPY]
 
-    def __init__(self, func: Callable | None = None, inv_func: Callable = no_collation) -> None:
+    def __init__(
+        self, func: Callable | None = None, inv_func: Callable = no_collation, track_meta: bool = True
+    ) -> None:
         if func is not None and not callable(func):
             raise TypeError(f"func must be None or callable but is {type(func).__name__}.")
         self.func = func
         self.inv_func = inv_func
+        self.track_meta = track_meta
 
     def __call__(self, img: NdarrayOrTensor, func: Callable | None = None):
         """
         Apply `self.func` to `img`.
 
         Args:
             func: Lambda/function to be applied. Defaults to `self.func`.
@@ -856,15 +861,15 @@
 
         """
         fn = func if func is not None else self.func
         if not callable(fn):
             raise TypeError(f"func must be None or callable but is {type(fn).__name__}.")
         out = fn(img)
         # convert to MetaTensor if necessary
-        if isinstance(out, (np.ndarray, torch.Tensor)) and not isinstance(out, MetaTensor) and get_track_meta():
+        if isinstance(out, (np.ndarray, torch.Tensor)) and not isinstance(out, MetaTensor) and self.track_meta:
             out = MetaTensor(out)
         if isinstance(out, MetaTensor):
             self.push_transform(out)
         return out
 
     def inverse(self, data: torch.Tensor):
         if isinstance(data, MetaTensor):
@@ -877,29 +882,37 @@
     Randomizable version :py:class:`monai.transforms.Lambda`, the input `func` may contain random logic,
     or randomly execute the function based on `prob`.
 
     Args:
         func: Lambda/function to be applied.
         prob: probability of executing the random function, default to 1.0, with 100% probability to execute.
         inv_func: Lambda/function of inverse operation, default to `lambda x: x`.
+        track_meta:  If `False`, then standard data objects will be returned (e.g., torch.Tensor` and `np.ndarray`)
+            as opposed to MONAI's enhanced objects. By default, this is `True`.
 
     For more details, please check :py:class:`monai.transforms.Lambda`.
     """
 
     backend = Lambda.backend
 
-    def __init__(self, func: Callable | None = None, prob: float = 1.0, inv_func: Callable = no_collation) -> None:
-        Lambda.__init__(self=self, func=func, inv_func=inv_func)
+    def __init__(
+        self,
+        func: Callable | None = None,
+        prob: float = 1.0,
+        inv_func: Callable = no_collation,
+        track_meta: bool = True,
+    ) -> None:
+        Lambda.__init__(self=self, func=func, inv_func=inv_func, track_meta=track_meta)
         RandomizableTransform.__init__(self=self, prob=prob)
 
     def __call__(self, img: NdarrayOrTensor, func: Callable | None = None):
         self.randomize(img)
         out = deepcopy(super().__call__(img, func) if self._do_transform else img)
         # convert to MetaTensor if necessary
-        if not isinstance(out, MetaTensor) and get_track_meta():
+        if not isinstance(out, MetaTensor) and self.track_meta:
             out = MetaTensor(out)
         if isinstance(out, MetaTensor):
             lambda_info = self.pop_transform(out) if self._do_transform else {}
             self.push_transform(out, extra_info=lambda_info)
         return out
 
     def inverse(self, data: torch.Tensor):
@@ -1623,21 +1636,19 @@
         if isinstance(filter, str):
             if not filter_size:
                 raise ValueError("`filter_size` must be specified when specifying filters by string.")
             if filter_size % 2 == 0:
                 raise ValueError("`filter_size` should be a single uneven integer.")
             if filter not in self.supported_filters:
                 raise NotImplementedError(f"{filter}. Supported filters are {self.supported_filters}.")
-        elif isinstance(filter, torch.Tensor) or isinstance(filter, np.ndarray):
+        elif isinstance(filter, (torch.Tensor, np.ndarray)):
             if filter.ndim not in [1, 2, 3]:
                 raise ValueError("Only 1D, 2D, and 3D filters are supported.")
             self._check_all_values_uneven(filter.shape)
-        elif isinstance(filter, (nn.Module, Transform)):
-            pass
-        else:
+        elif not isinstance(filter, (nn.Module, Transform)):
             raise TypeError(
                 f"{type(filter)} is not supported."
                 "Supported types are `class 'str'`, `class 'torch.Tensor'`, `class 'np.ndarray'`, "
                 "`class 'torch.nn.modules.module.Module'`, `class 'monai.transforms.Transform'`"
             )
 
     def _check_kwargs_are_present(self, filter, **kwargs):
```

### Comparing `monai-weekly-1.2.dev2316/monai/transforms/utility/dictionary.py` & `monai-weekly-1.2.dev2317/monai/transforms/utility/dictionary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1084,14 +1084,16 @@
     Args:
         keys: keys of the corresponding items to be transformed.
             See also: :py:class:`monai.transforms.compose.MapTransform`
         func: Lambda/function to be applied. It also can be a sequence of Callable,
             each element corresponds to a key in ``keys``.
         inv_func: Lambda/function of inverse operation if want to invert transforms, default to `lambda x: x`.
             It also can be a sequence of Callable, each element corresponds to a key in ``keys``.
+        track_meta:  If `False`, then standard data objects will be returned (e.g., torch.Tensor` and `np.ndarray`)
+            as opposed to MONAI's enhanced objects. By default, this is `True`.
         overwrite: whether to overwrite the original data in the input dictionary with lambda function output. it
             can be bool or str, when setting to str, it will create a new key for the output and keep the value of
             key intact. default to True. it also can be a sequence of bool or str, each element corresponds to a key
             in ``keys``.
         allow_missing_keys: don't raise exception if key is missing.
 
     Note: The inverse operation doesn't allow to define `extra_info` or access other information, such as the
@@ -1102,22 +1104,23 @@
     backend = Lambda.backend
 
     def __init__(
         self,
         keys: KeysCollection,
         func: Sequence[Callable] | Callable,
         inv_func: Sequence[Callable] | Callable = no_collation,
+        track_meta: bool = True,
         overwrite: Sequence[bool] | bool | Sequence[str] | str = True,
         allow_missing_keys: bool = False,
     ) -> None:
         super().__init__(keys, allow_missing_keys)
         self.func = ensure_tuple_rep(func, len(self.keys))
         self.inv_func = ensure_tuple_rep(inv_func, len(self.keys))
         self.overwrite = ensure_tuple_rep(overwrite, len(self.keys))
-        self._lambd = Lambda()
+        self._lambd = Lambda(track_meta=track_meta)
 
     def __call__(self, data: Mapping[Hashable, torch.Tensor]) -> dict[Hashable, torch.Tensor]:
         d = dict(data)
         for key, func, overwrite in self.key_iterator(d, self.func, self.overwrite):
             ret = self._lambd(img=d[key], func=func)
             if overwrite and isinstance(overwrite, bool):
                 d[key] = ret
@@ -1142,14 +1145,16 @@
     Args:
         keys: keys of the corresponding items to be transformed.
             See also: :py:class:`monai.transforms.compose.MapTransform`
         func: Lambda/function to be applied. It also can be a sequence of Callable,
             each element corresponds to a key in ``keys``.
         inv_func: Lambda/function of inverse operation if want to invert transforms, default to `lambda x: x`.
             It also can be a sequence of Callable, each element corresponds to a key in ``keys``.
+        track_meta:  If `False`, then standard data objects will be returned (e.g., torch.Tensor` and `np.ndarray`)
+            as opposed to MONAI's enhanced objects. By default, this is `True`.
         overwrite: whether to overwrite the original data in the input dictionary with lambda function output.
             default to True. it also can be a sequence of bool, each element corresponds to a key in ``keys``.
         prob: probability of executing the random function, default to 1.0, with 100% probability to execute.
             note that all the data specified by `keys` will share the same random probability to execute or not.
         allow_missing_keys: don't raise exception if key is missing.
 
     For more details, please check :py:class:`monai.transforms.Lambdad`.
@@ -1161,23 +1166,25 @@
     backend = Lambda.backend
 
     def __init__(
         self,
         keys: KeysCollection,
         func: Sequence[Callable] | Callable,
         inv_func: Sequence[Callable] | Callable = no_collation,
+        track_meta: bool = True,
         overwrite: Sequence[bool] | bool = True,
         prob: float = 1.0,
         allow_missing_keys: bool = False,
     ) -> None:
         Lambdad.__init__(
             self=self,
             keys=keys,
             func=func,
             inv_func=inv_func,
+            track_meta=track_meta,
             overwrite=overwrite,
             allow_missing_keys=allow_missing_keys,
         )
         RandomizableTransform.__init__(self=self, prob=prob, do_transform=True)
 
     def __call__(self, data):
         self.randomize(data)
```

### Comparing `monai-weekly-1.2.dev2316/monai/transforms/utils.py` & `monai-weekly-1.2.dev2317/monai/transforms/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/transforms/utils_create_transform_ims.py` & `monai-weekly-1.2.dev2317/monai/transforms/utils_create_transform_ims.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/transforms/utils_pytorch_numpy_unification.py` & `monai-weekly-1.2.dev2317/monai/transforms/utils_pytorch_numpy_unification.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/utils/__init__.py` & `monai-weekly-1.2.dev2317/monai/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/utils/aliases.py` & `monai-weekly-1.2.dev2317/monai/utils/aliases.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,16 @@
         if obj is None:
             raise ValueError(f"Module {modname!r} does not have member {declname!r}.")
 
     # attempt to resolve a simple name
     if obj is None:
         # Get all modules having the declaration/import, need to check here that getattr returns something which doesn't
         # equate to False since in places __getattr__ returns 0 incorrectly:
-        # https://github.com/tensorflow/tensorboard/blob/a22566561d2b4fea408755a951ac9eaf3a156f8e/tensorboard/compat/tensorflow_stub/pywrap_tensorflow.py#L35  # noqa: B950
+        # https://github.com/tensorflow/tensorboard/blob/a22566561d2b4fea408755a951ac9eaf3a156f8e/
+        # tensorboard/compat/tensorflow_stub/pywrap_tensorflow.py#L35
         mods = [m for m in list(sys.modules.values()) if getattr(m, name, None)]
 
         if len(mods) > 0:  # found modules with this declaration or import
             if len(mods) > 1:  # found multiple modules, need to determine if ambiguous or just multiple imports
                 foundmods = set(filter(None, {inspect.getmodule(getattr(m, name)) for m in mods}))  # resolve imports
 
                 if len(foundmods) > 1:  # found multiple declarations with the same name
```

### Comparing `monai-weekly-1.2.dev2316/monai/utils/decorators.py` & `monai-weekly-1.2.dev2317/monai/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/utils/deprecate_utils.py` & `monai-weekly-1.2.dev2317/monai/utils/deprecate_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/utils/dist.py` & `monai-weekly-1.2.dev2317/monai/utils/dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/utils/enums.py` & `monai-weekly-1.2.dev2317/monai/utils/enums.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/utils/jupyter_utils.py` & `monai-weekly-1.2.dev2317/monai/utils/jupyter_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/utils/misc.py` & `monai-weekly-1.2.dev2317/monai/utils/misc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/utils/module.py` & `monai-weekly-1.2.dev2317/monai/utils/module.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/utils/nvtx.py` & `monai-weekly-1.2.dev2317/monai/utils/nvtx.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/utils/profiling.py` & `monai-weekly-1.2.dev2317/monai/utils/profiling.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/utils/state_cacher.py` & `monai-weekly-1.2.dev2317/monai/utils/state_cacher.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/utils/type_conversion.py` & `monai-weekly-1.2.dev2317/monai/utils/type_conversion.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/visualize/__init__.py` & `monai-weekly-1.2.dev2317/monai/visualize/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/visualize/class_activation_maps.py` & `monai-weekly-1.2.dev2317/monai/visualize/class_activation_maps.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/visualize/gradient_based.py` & `monai-weekly-1.2.dev2317/monai/visualize/gradient_based.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/visualize/img2tensorboard.py` & `monai-weekly-1.2.dev2317/monai/visualize/img2tensorboard.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/visualize/occlusion_sensitivity.py` & `monai-weekly-1.2.dev2317/monai/visualize/occlusion_sensitivity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/visualize/utils.py` & `monai-weekly-1.2.dev2317/monai/visualize/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai/visualize/visualizer.py` & `monai-weekly-1.2.dev2317/monai/visualize/visualizer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai_weekly.egg-info/PKG-INFO` & `monai-weekly-1.2.dev2317/monai_weekly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monai-weekly
-Version: 1.2.dev2316
+Version: 1.2.dev2317
 Summary: AI Toolkit for Healthcare Imaging
 Home-page: https://monai.io/
 Author: MONAI Consortium
 Author-email: monai.contact@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.monai.io/
 Project-URL: Bug Tracker, https://github.com/Project-MONAI/MONAI/issues
```

### Comparing `monai-weekly-1.2.dev2316/monai_weekly.egg-info/SOURCES.txt` & `monai-weekly-1.2.dev2317/monai_weekly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/monai_weekly.egg-info/requires.txt` & `monai-weekly-1.2.dev2317/monai_weekly.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/pyproject.toml` & `monai-weekly-1.2.dev2317/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -32,14 +32,19 @@
 )
 '''
 
 [tool.pycln]
 all = true
 exclude = "monai/bundle/__main__.py"
 
+[tool.ruff]
+line-length = 133
+ignore-init-module-imports = true
+ignore = ["F401", "E741"]
+
 [tool.pytype]
 # Space-separated list of files or directories to exclude.
 exclude = ["versioneer.py", "_version.py"]
 # Space-separated list of files or directories to process.
 inputs = ["monai"]
 # Keep going past errors to analyze as many files as possible.
 keep_going = true
```

### Comparing `monai-weekly-1.2.dev2316/setup.cfg` & `monai-weekly-1.2.dev2317/setup.cfg`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/setup.py` & `monai-weekly-1.2.dev2317/setup.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_acn_block.py` & `monai-weekly-1.2.dev2317/tests/test_acn_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_activations.py` & `monai-weekly-1.2.dev2317/tests/test_activations.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_activationsd.py` & `monai-weekly-1.2.dev2317/tests/test_activationsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_adaptors.py` & `monai-weekly-1.2.dev2317/tests/test_adaptors.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_add_channeld.py` & `monai-weekly-1.2.dev2317/tests/test_add_channeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_add_coordinate_channels.py` & `monai-weekly-1.2.dev2317/tests/test_add_coordinate_channels.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_add_coordinate_channelsd.py` & `monai-weekly-1.2.dev2317/tests/test_add_coordinate_channelsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_add_extreme_points_channel.py` & `monai-weekly-1.2.dev2317/tests/test_add_extreme_points_channel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_add_extreme_points_channeld.py` & `monai-weekly-1.2.dev2317/tests/test_add_extreme_points_channeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_adjust_contrast.py` & `monai-weekly-1.2.dev2317/tests/test_adjust_contrast.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_adjust_contrastd.py` & `monai-weekly-1.2.dev2317/tests/test_adjust_contrastd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_adn.py` & `monai-weekly-1.2.dev2317/tests/test_adn.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_affine.py` & `monai-weekly-1.2.dev2317/tests/test_affine.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_affine_grid.py` & `monai-weekly-1.2.dev2317/tests/test_affine_grid.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_affine_transform.py` & `monai-weekly-1.2.dev2317/tests/test_affine_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_affined.py` & `monai-weekly-1.2.dev2317/tests/test_affined.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_ahnet.py` & `monai-weekly-1.2.dev2317/tests/test_ahnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_alias.py` & `monai-weekly-1.2.dev2317/tests/test_alias.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_anchor_box.py` & `monai-weekly-1.2.dev2317/tests/test_anchor_box.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_apply.py` & `monai-weekly-1.2.dev2317/tests/test_apply.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_apply_filter.py` & `monai-weekly-1.2.dev2317/tests/test_apply_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_arraydataset.py` & `monai-weekly-1.2.dev2317/tests/test_arraydataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_as_channel_first.py` & `monai-weekly-1.2.dev2317/tests/test_as_channel_first.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_as_channel_firstd.py` & `monai-weekly-1.2.dev2317/tests/test_as_channel_firstd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_as_channel_last.py` & `monai-weekly-1.2.dev2317/tests/test_as_channel_last.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_as_channel_lastd.py` & `monai-weekly-1.2.dev2317/tests/test_as_channel_lastd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_as_discrete.py` & `monai-weekly-1.2.dev2317/tests/test_as_discrete.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_as_discreted.py` & `monai-weekly-1.2.dev2317/tests/test_as_discreted.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_atss_box_matcher.py` & `monai-weekly-1.2.dev2317/tests/test_atss_box_matcher.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_attentionunet.py` & `monai-weekly-1.2.dev2317/tests/test_attentionunet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_auto3dseg.py` & `monai-weekly-1.2.dev2317/tests/test_auto3dseg.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_auto3dseg_ensemble.py` & `monai-weekly-1.2.dev2317/tests/test_auto3dseg_ensemble.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     else {}
 )
 
 pred_param = {"files_slices": slice(0, 1), "mode": "mean", "sigmoid": True}
 
 
 @skip_if_quick
-@SkipIfBeforePyTorchVersion((1, 9, 1))
+@SkipIfBeforePyTorchVersion((1, 11, 1))
 @unittest.skipIf(not has_tb, "no tensorboard summary writer")
 class TestEnsembleBuilder(unittest.TestCase):
     def setUp(self) -> None:
         set_determinism(0)
         self.test_dir = tempfile.TemporaryDirectory()
 
     @skip_if_no_cuda
```

### Comparing `monai-weekly-1.2.dev2316/tests/test_auto3dseg_hpo.py` & `monai-weekly-1.2.dev2317/tests/test_auto3dseg_hpo.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         {"fold": 2, "image": "tr_image_010.fake.nii.gz", "label": "tr_label_010.fake.nii.gz"},
         {"fold": 2, "image": "tr_image_011.fake.nii.gz", "label": "tr_label_011.fake.nii.gz"},
         {"fold": 2, "image": "tr_image_012.fake.nii.gz", "label": "tr_label_012.fake.nii.gz"},
     ],
 }
 
 
-@SkipIfBeforePyTorchVersion((1, 9, 1))
+@SkipIfBeforePyTorchVersion((1, 11, 1))
 @unittest.skipIf(not has_tb, "no tensorboard summary writer")
 class TestHPO(unittest.TestCase):
     def setUp(self) -> None:
         self.test_dir = tempfile.TemporaryDirectory()
         test_path = self.test_dir.name
 
         work_dir = os.path.abspath(os.path.join(test_path, "workdir"))
@@ -173,17 +173,16 @@
     def test_get_history(self) -> None:
         algo_dict = self.history[-1]
         algo = algo_dict[AlgoKeys.ALGO]
         nni_gen = NNIGen(algo=algo, params=override_param)
         obj_filename = nni_gen.get_obj_filename()
 
         NNIGen().run_algo(obj_filename, self.work_dir)
-
         history = import_bundle_algo_history(self.work_dir, only_trained=True)
-        assert len(history) == 1
+        assert len(history) == 3
 
     def tearDown(self) -> None:
         self.test_dir.cleanup()
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai-weekly-1.2.dev2316/tests/test_autoencoder.py` & `monai-weekly-1.2.dev2317/tests/test_autoencoder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_avg_merger.py` & `monai-weekly-1.2.dev2317/tests/test_avg_merger.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_basic_unet.py` & `monai-weekly-1.2.dev2317/tests/test_basic_unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_basic_unetplusplus.py` & `monai-weekly-1.2.dev2317/tests/test_basic_unetplusplus.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_bending_energy.py` & `monai-weekly-1.2.dev2317/tests/test_bending_energy.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_bilateral_approx_cpu.py` & `monai-weekly-1.2.dev2317/tests/test_bilateral_approx_cpu.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_bilateral_approx_cuda.py` & `monai-weekly-1.2.dev2317/tests/test_bilateral_approx_cuda.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_bilateral_precise.py` & `monai-weekly-1.2.dev2317/tests/test_bilateral_precise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_blend_images.py` & `monai-weekly-1.2.dev2317/tests/test_blend_images.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_border_pad.py` & `monai-weekly-1.2.dev2317/tests/test_border_pad.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_border_padd.py` & `monai-weekly-1.2.dev2317/tests/test_border_padd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_bounding_rect.py` & `monai-weekly-1.2.dev2317/tests/test_bounding_rect.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_bounding_rectd.py` & `monai-weekly-1.2.dev2317/tests/test_bounding_rectd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_box_coder.py` & `monai-weekly-1.2.dev2317/tests/test_box_coder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_box_transform.py` & `monai-weekly-1.2.dev2317/tests/test_box_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_box_utils.py` & `monai-weekly-1.2.dev2317/tests/test_box_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_bundle_ckpt_export.py` & `monai-weekly-1.2.dev2317/tests/test_bundle_ckpt_export.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_bundle_download.py` & `monai-weekly-1.2.dev2317/tests/test_bundle_download.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_bundle_get_data.py` & `monai-weekly-1.2.dev2317/tests/test_bundle_get_data.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_bundle_init_bundle.py` & `monai-weekly-1.2.dev2317/tests/test_bundle_init_bundle.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_bundle_onnx_export.py` & `monai-weekly-1.2.dev2317/tests/test_bundle_onnx_export.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_bundle_trt_export.py` & `monai-weekly-1.2.dev2317/tests/test_bundle_trt_export.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_bundle_utils.py` & `monai-weekly-1.2.dev2317/tests/test_bundle_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_bundle_verify_metadata.py` & `monai-weekly-1.2.dev2317/tests/test_bundle_verify_metadata.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_bundle_verify_net.py` & `monai-weekly-1.2.dev2317/tests/test_bundle_verify_net.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_bundle_workflow.py` & `monai-weekly-1.2.dev2317/tests/test_bundle_workflow.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_cachedataset.py` & `monai-weekly-1.2.dev2317/tests/test_cachedataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_cachedataset_parallel.py` & `monai-weekly-1.2.dev2317/tests/test_cachedataset_parallel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_cachedataset_persistent_workers.py` & `monai-weekly-1.2.dev2317/tests/test_cachedataset_persistent_workers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_cachentransdataset.py` & `monai-weekly-1.2.dev2317/tests/test_cachentransdataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_call_dist.py` & `monai-weekly-1.2.dev2317/tests/test_call_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_cast_to_type.py` & `monai-weekly-1.2.dev2317/tests/test_cast_to_type.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_cast_to_typed.py` & `monai-weekly-1.2.dev2317/tests/test_cast_to_typed.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_center_scale_crop.py` & `monai-weekly-1.2.dev2317/tests/test_center_scale_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_center_scale_cropd.py` & `monai-weekly-1.2.dev2317/tests/test_center_scale_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_center_spatial_crop.py` & `monai-weekly-1.2.dev2317/tests/test_center_spatial_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_center_spatial_cropd.py` & `monai-weekly-1.2.dev2317/tests/test_center_spatial_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_channel_pad.py` & `monai-weekly-1.2.dev2317/tests/test_channel_pad.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_check_hash.py` & `monai-weekly-1.2.dev2317/tests/test_check_hash.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_check_missing_files.py` & `monai-weekly-1.2.dev2317/tests/test_check_missing_files.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_classes_to_indices.py` & `monai-weekly-1.2.dev2317/tests/test_classes_to_indices.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_classes_to_indicesd.py` & `monai-weekly-1.2.dev2317/tests/test_classes_to_indicesd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_complex_utils.py` & `monai-weekly-1.2.dev2317/tests/test_complex_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_component_locator.py` & `monai-weekly-1.2.dev2317/tests/test_component_locator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_compose.py` & `monai-weekly-1.2.dev2317/tests/test_compose.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_compose_get_number_conversions.py` & `monai-weekly-1.2.dev2317/tests/test_compose_get_number_conversions.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_compute_confusion_matrix.py` & `monai-weekly-1.2.dev2317/tests/test_compute_confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_compute_f_beta.py` & `monai-weekly-1.2.dev2317/tests/test_compute_f_beta.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_compute_froc.py` & `monai-weekly-1.2.dev2317/tests/test_compute_froc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_compute_generalized_dice.py` & `monai-weekly-1.2.dev2317/tests/test_compute_generalized_dice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_compute_ho_ver_maps.py` & `monai-weekly-1.2.dev2317/tests/test_compute_ho_ver_maps.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_compute_ho_ver_maps_d.py` & `monai-weekly-1.2.dev2317/tests/test_compute_ho_ver_maps_d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_compute_meandice.py` & `monai-weekly-1.2.dev2317/tests/test_compute_meandice.py`

 * *Files 5% similar despite different names*

```diff
@@ -203,20 +203,24 @@
         vals = {"y_pred": dict(input_data).pop("y_pred"), "y": dict(input_data).pop("y")}
         result = DiceHelper(sigmoid=True)(**vals)
         np.testing.assert_allclose(result[0].cpu().numpy(), [0.0, 0.0, 0.0], atol=1e-4)
         np.testing.assert_allclose(sorted(result[1].cpu().numpy()), [0.0, 1.0, 2.0], atol=1e-4)
         result = DiceHelper(softmax=True, get_not_nans=False)(**vals)
         np.testing.assert_allclose(result[0].cpu().numpy(), [0.0, 0.0], atol=1e-4)
 
+        num_classes = vals["y_pred"].shape[1]
+        vals["y_pred"] = torch.argmax(vals["y_pred"], dim=1, keepdim=True)
+        result = DiceHelper(sigmoid=True, num_classes=num_classes)(**vals)
+        np.testing.assert_allclose(result[0].cpu().numpy(), [0.0, 0.0, 0.0], atol=1e-4)
+
     # DiceMetric class tests
     @parameterized.expand([TEST_CASE_1, TEST_CASE_2, TEST_CASE_10])
     def test_value_class(self, input_data, expected_value):
         # same test as for compute_dice
-        vals = {}
-        vals["y_pred"] = input_data.pop("y_pred")
+        vals = {"y_pred": input_data.pop("y_pred")}
         vals["y"] = input_data.pop("y")
         dice_metric = DiceMetric(**input_data)
         dice_metric(**vals)
         result = dice_metric.aggregate(reduction="none")
         np.testing.assert_allclose(result.cpu().numpy(), expected_value, atol=1e-4)
 
     @parameterized.expand([TEST_CASE_4, TEST_CASE_5, TEST_CASE_6, TEST_CASE_7, TEST_CASE_8])
```

### Comparing `monai-weekly-1.2.dev2316/tests/test_compute_meaniou.py` & `monai-weekly-1.2.dev2317/tests/test_compute_meaniou.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_compute_panoptic_quality.py` & `monai-weekly-1.2.dev2317/tests/test_compute_panoptic_quality.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_compute_regression_metrics.py` & `monai-weekly-1.2.dev2317/tests/test_compute_regression_metrics.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_compute_roc_auc.py` & `monai-weekly-1.2.dev2317/tests/test_compute_roc_auc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_compute_variance.py` & `monai-weekly-1.2.dev2317/tests/test_compute_variance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_concat_itemsd.py` & `monai-weekly-1.2.dev2317/tests/test_concat_itemsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_config_item.py` & `monai-weekly-1.2.dev2317/tests/test_config_item.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_config_parser.py` & `monai-weekly-1.2.dev2317/tests/test_config_parser.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_contrastive_loss.py` & `monai-weekly-1.2.dev2317/tests/test_contrastive_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_convert_data_type.py` & `monai-weekly-1.2.dev2317/tests/test_convert_data_type.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_convert_to_multi_channel.py` & `monai-weekly-1.2.dev2317/tests/test_convert_to_multi_channel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_convert_to_multi_channeld.py` & `monai-weekly-1.2.dev2317/tests/test_convert_to_multi_channeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_convert_to_onnx.py` & `monai-weekly-1.2.dev2317/tests/test_convert_to_onnx.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_convert_to_torchscript.py` & `monai-weekly-1.2.dev2317/tests/test_convert_to_torchscript.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_convert_to_trt.py` & `monai-weekly-1.2.dev2317/tests/test_convert_to_trt.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_convolutions.py` & `monai-weekly-1.2.dev2317/tests/test_convolutions.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_copy_itemsd.py` & `monai-weekly-1.2.dev2317/tests/test_copy_itemsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_copy_model_state.py` & `monai-weekly-1.2.dev2317/tests/test_copy_model_state.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_correct_crop_centers.py` & `monai-weekly-1.2.dev2317/tests/test_correct_crop_centers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_create_cross_validation_datalist.py` & `monai-weekly-1.2.dev2317/tests/test_create_cross_validation_datalist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_create_grid_and_affine.py` & `monai-weekly-1.2.dev2317/tests/test_create_grid_and_affine.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_crf_cpu.py` & `monai-weekly-1.2.dev2317/tests/test_crf_cpu.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_crf_cuda.py` & `monai-weekly-1.2.dev2317/tests/test_crf_cuda.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_crop_foreground.py` & `monai-weekly-1.2.dev2317/tests/test_crop_foreground.py`

 * *Files 20% similar despite different names*

```diff
@@ -142,10 +142,21 @@
         with self.assertRaises(ValueError):
             crop_fn = CropForeground(**input_param)
             # lazy
             crop_fn.lazy_evaluation = True
             pending_result = crop_fn(image)
             return apply_transforms(pending_result, mode="nearest", align_corners=align_corners)[0]
 
+    @parameterized.expand(TEST_COORDS + TESTS)
+    def test_inverse_pending_ops(self, input_param, image, _expected_data, align_corners):
+        crop_fn = CropForeground(**input_param)
+        crop_fn.lazy_evaluation = True
+        pending_result = crop_fn(image)
+        self.assertIsInstance(pending_result, MetaTensor)
+        result = apply_transforms(pending_result, mode="nearest", align_corners=align_corners)[0]
+        inverted = crop_fn.inverse(result)
+        self.assertEqual(image.shape, inverted.shape)
+        self.assertTrue((not inverted.applied_operations) and (not inverted.pending_operations))
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai-weekly-1.2.dev2316/tests/test_crop_foregroundd.py` & `monai-weekly-1.2.dev2317/tests/test_crop_foregroundd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_cross_validation.py` & `monai-weekly-1.2.dev2317/tests/test_cross_validation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_csv_dataset.py` & `monai-weekly-1.2.dev2317/tests/test_csv_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_csv_iterable_dataset.py` & `monai-weekly-1.2.dev2317/tests/test_csv_iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_csv_saver.py` & `monai-weekly-1.2.dev2317/tests/test_csv_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_cucim_dict_transform.py` & `monai-weekly-1.2.dev2317/tests/test_cucim_dict_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_cucim_transform.py` & `monai-weekly-1.2.dev2317/tests/test_cucim_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_cumulative.py` & `monai-weekly-1.2.dev2317/tests/test_cumulative.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_cumulative_average.py` & `monai-weekly-1.2.dev2317/tests/test_cumulative_average.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_cumulative_average_dist.py` & `monai-weekly-1.2.dev2317/tests/test_cumulative_average_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_cv2_dist.py` & `monai-weekly-1.2.dev2317/tests/test_cv2_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_data_stats.py` & `monai-weekly-1.2.dev2317/tests/test_data_stats.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_data_statsd.py` & `monai-weekly-1.2.dev2317/tests/test_data_statsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_dataloader.py` & `monai-weekly-1.2.dev2317/tests/test_dataloader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_dataset.py` & `monai-weekly-1.2.dev2317/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_dataset_func.py` & `monai-weekly-1.2.dev2317/tests/test_dataset_func.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_dataset_summary.py` & `monai-weekly-1.2.dev2317/tests/test_dataset_summary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_decathlondataset.py` & `monai-weekly-1.2.dev2317/tests/test_decathlondataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_decollate.py` & `monai-weekly-1.2.dev2317/tests/test_decollate.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_deepedit_interaction.py` & `monai-weekly-1.2.dev2317/tests/test_deepedit_interaction.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_deepedit_transforms.py` & `monai-weekly-1.2.dev2317/tests/test_deepedit_transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_deepgrow_dataset.py` & `monai-weekly-1.2.dev2317/tests/test_deepgrow_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_deepgrow_interaction.py` & `monai-weekly-1.2.dev2317/tests/test_deepgrow_interaction.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_deepgrow_transforms.py` & `monai-weekly-1.2.dev2317/tests/test_deepgrow_transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_delete_itemsd.py` & `monai-weekly-1.2.dev2317/tests/test_delete_itemsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_denseblock.py` & `monai-weekly-1.2.dev2317/tests/test_denseblock.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_densenet.py` & `monai-weekly-1.2.dev2317/tests/test_densenet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_deprecated.py` & `monai-weekly-1.2.dev2317/tests/test_deprecated.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_detect_envelope.py` & `monai-weekly-1.2.dev2317/tests/test_detect_envelope.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_detection_coco_metrics.py` & `monai-weekly-1.2.dev2317/tests/test_detection_coco_metrics.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_detector_boxselector.py` & `monai-weekly-1.2.dev2317/tests/test_detector_boxselector.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_detector_utils.py` & `monai-weekly-1.2.dev2317/tests/test_detector_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_dev_collate.py` & `monai-weekly-1.2.dev2317/tests/test_dev_collate.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_dice_ce_loss.py` & `monai-weekly-1.2.dev2317/tests/test_dice_ce_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_dice_focal_loss.py` & `monai-weekly-1.2.dev2317/tests/test_dice_focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_dice_loss.py` & `monai-weekly-1.2.dev2317/tests/test_dice_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_dints_cell.py` & `monai-weekly-1.2.dev2317/tests/test_dints_cell.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_dints_mixop.py` & `monai-weekly-1.2.dev2317/tests/test_dints_mixop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_dints_network.py` & `monai-weekly-1.2.dev2317/tests/test_dints_network.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_discriminator.py` & `monai-weekly-1.2.dev2317/tests/test_discriminator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_divisible_pad.py` & `monai-weekly-1.2.dev2317/tests/test_divisible_pad.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_divisible_padd.py` & `monai-weekly-1.2.dev2317/tests/test_divisible_padd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_download_and_extract.py` & `monai-weekly-1.2.dev2317/tests/test_download_and_extract.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_downsample_block.py` & `monai-weekly-1.2.dev2317/tests/test_downsample_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_drop_path.py` & `monai-weekly-1.2.dev2317/tests/test_drop_path.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_ds_loss.py` & `monai-weekly-1.2.dev2317/tests/test_ds_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_dvf2ddf.py` & `monai-weekly-1.2.dev2317/tests/test_dvf2ddf.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_dynunet.py` & `monai-weekly-1.2.dev2317/tests/test_dynunet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_dynunet_block.py` & `monai-weekly-1.2.dev2317/tests/test_dynunet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_efficientnet.py` & `monai-weekly-1.2.dev2317/tests/test_efficientnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_ensemble_evaluator.py` & `monai-weekly-1.2.dev2317/tests/test_ensemble_evaluator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_ensure_channel_first.py` & `monai-weekly-1.2.dev2317/tests/test_ensure_channel_first.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_ensure_channel_firstd.py` & `monai-weekly-1.2.dev2317/tests/test_ensure_channel_firstd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_ensure_tuple.py` & `monai-weekly-1.2.dev2317/tests/test_ensure_tuple.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_ensure_type.py` & `monai-weekly-1.2.dev2317/tests/test_ensure_type.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_ensure_typed.py` & `monai-weekly-1.2.dev2317/tests/test_ensure_typed.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_enum_bound_interp.py` & `monai-weekly-1.2.dev2317/tests/test_enum_bound_interp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_eval_mode.py` & `monai-weekly-1.2.dev2317/tests/test_eval_mode.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_evenly_divisible_all_gather_dist.py` & `monai-weekly-1.2.dev2317/tests/test_evenly_divisible_all_gather_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_factorized_increase.py` & `monai-weekly-1.2.dev2317/tests/test_factorized_increase.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_factorized_reduce.py` & `monai-weekly-1.2.dev2317/tests/test_factorized_reduce.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_fastmri_reader.py` & `monai-weekly-1.2.dev2317/tests/test_fastmri_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_fft_utils.py` & `monai-weekly-1.2.dev2317/tests/test_fft_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_fg_bg_to_indices.py` & `monai-weekly-1.2.dev2317/tests/test_fg_bg_to_indices.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_fg_bg_to_indicesd.py` & `monai-weekly-1.2.dev2317/tests/test_fg_bg_to_indicesd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_file_basename.py` & `monai-weekly-1.2.dev2317/tests/test_file_basename.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_fill_holes.py` & `monai-weekly-1.2.dev2317/tests/test_fill_holes.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_fill_holesd.py` & `monai-weekly-1.2.dev2317/tests/test_fill_holesd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_fl_exchange_object.py` & `monai-weekly-1.2.dev2317/tests/test_fl_exchange_object.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_fl_monai_algo.py` & `monai-weekly-1.2.dev2317/tests/test_fl_monai_algo.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,36 +7,41 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
+import glob
 import os
 import shutil
-import tempfile
 import unittest
+from copy import deepcopy
+from os.path import join as pathjoin
 
 from parameterized import parameterized
 
-from monai.bundle import ConfigParser
+from monai.bundle import ConfigParser, ConfigWorkflow
 from monai.bundle.utils import DEFAULT_HANDLERS_ID
 from monai.fl.client.monai_algo import MonaiAlgo
 from monai.fl.utils.constants import ExtraItems
 from monai.fl.utils.exchange_object import ExchangeObject
 from monai.utils import path_to_uri
 from tests.utils import SkipIfNoModule
 
 _root_dir = os.path.abspath(os.path.join(os.path.dirname(__file__)))
 _data_dir = os.path.join(_root_dir, "testing_data")
+_logging_file = pathjoin(_data_dir, "logging.conf")
 
 TEST_TRAIN_1 = [
     {
         "bundle_root": _data_dir,
-        "config_train_filename": os.path.join(_data_dir, "config_fl_train.json"),
+        "train_workflow": ConfigWorkflow(
+            config_file=os.path.join(_data_dir, "config_fl_train.json"), workflow="train", logging_file=_logging_file
+        ),
         "config_evaluate_filename": None,
         "config_filters_filename": os.path.join(_data_dir, "config_fl_filters.json"),
     }
 ]
 TEST_TRAIN_2 = [
     {
         "bundle_root": _data_dir,
@@ -44,175 +49,185 @@
         "config_evaluate_filename": None,
         "config_filters_filename": None,
     }
 ]
 TEST_TRAIN_3 = [
     {
         "bundle_root": _data_dir,
-        "config_train_filename": [
-            os.path.join(_data_dir, "config_fl_train.json"),
-            os.path.join(_data_dir, "config_fl_train.json"),
-        ],
+        "train_workflow": ConfigWorkflow(
+            config_file=os.path.join(_data_dir, "config_fl_train.json"), workflow="train", logging_file=_logging_file
+        ),
         "config_evaluate_filename": None,
-        "config_filters_filename": [
-            os.path.join(_data_dir, "config_fl_filters.json"),
-            os.path.join(_data_dir, "config_fl_filters.json"),
-        ],
+        "config_filters_filename": os.path.join(_data_dir, "config_fl_filters.json"),
+    }
+]
+
+TEST_TRAIN_4 = [
+    {
+        "bundle_root": _data_dir,
+        "train_workflow": ConfigWorkflow(
+            config_file=os.path.join(_data_dir, "config_fl_train.json"),
+            workflow="train",
+            logging_file=_logging_file,
+            tracking={
+                "handlers_id": DEFAULT_HANDLERS_ID,
+                "configs": {
+                    "execute_config": f"{_data_dir}/config_executed.json",
+                    "trainer": {
+                        "_target_": "MLFlowHandler",
+                        "tracking_uri": path_to_uri(_data_dir) + "/mlflow_override",
+                        "output_transform": "$monai.handlers.from_engine(['loss'], first=True)",
+                        "close_on_complete": True,
+                    },
+                },
+            },
+        ),
+        "config_evaluate_filename": None,
+        "config_filters_filename": None,
     }
 ]
 
 TEST_EVALUATE_1 = [
     {
         "bundle_root": _data_dir,
         "config_train_filename": None,
-        "config_evaluate_filename": os.path.join(_data_dir, "config_fl_evaluate.json"),
+        "eval_workflow": ConfigWorkflow(
+            config_file=[
+                os.path.join(_data_dir, "config_fl_train.json"),
+                os.path.join(_data_dir, "config_fl_evaluate.json"),
+            ],
+            workflow="train",
+            logging_file=_logging_file,
+            tracking="mlflow",
+            tracking_uri=path_to_uri(_data_dir) + "/mlflow_1",
+            experiment_name="monai_eval1",
+        ),
         "config_filters_filename": os.path.join(_data_dir, "config_fl_filters.json"),
     }
 ]
 TEST_EVALUATE_2 = [
     {
         "bundle_root": _data_dir,
         "config_train_filename": None,
-        "config_evaluate_filename": os.path.join(_data_dir, "config_fl_evaluate.json"),
+        "config_evaluate_filename": [
+            os.path.join(_data_dir, "config_fl_train.json"),
+            os.path.join(_data_dir, "config_fl_evaluate.json"),
+        ],
+        "eval_kwargs": {
+            "tracking": "mlflow",
+            "tracking_uri": path_to_uri(_data_dir) + "/mlflow_2",
+            "experiment_name": "monai_eval2",
+        },
+        "eval_workflow_name": "training",
         "config_filters_filename": None,
     }
 ]
 TEST_EVALUATE_3 = [
     {
         "bundle_root": _data_dir,
         "config_train_filename": None,
-        "config_evaluate_filename": [
-            os.path.join(_data_dir, "config_fl_evaluate.json"),
-            os.path.join(_data_dir, "config_fl_evaluate.json"),
-        ],
-        "config_filters_filename": [
-            os.path.join(_data_dir, "config_fl_filters.json"),
-            os.path.join(_data_dir, "config_fl_filters.json"),
-        ],
+        "eval_workflow": ConfigWorkflow(
+            config_file=[
+                os.path.join(_data_dir, "config_fl_train.json"),
+                os.path.join(_data_dir, "config_fl_evaluate.json"),
+            ],
+            workflow="train",
+            logging_file=_logging_file,
+        ),
+        "config_filters_filename": os.path.join(_data_dir, "config_fl_filters.json"),
     }
 ]
 
 TEST_GET_WEIGHTS_1 = [
     {
         "bundle_root": _data_dir,
-        "config_train_filename": os.path.join(_data_dir, "config_fl_train.json"),
+        "train_workflow": ConfigWorkflow(
+            config_file=os.path.join(_data_dir, "config_fl_train.json"), workflow="train", logging_file=_logging_file
+        ),
         "config_evaluate_filename": None,
         "send_weight_diff": False,
         "config_filters_filename": os.path.join(_data_dir, "config_fl_filters.json"),
     }
 ]
 TEST_GET_WEIGHTS_2 = [
     {
         "bundle_root": _data_dir,
-        "config_train_filename": None,
-        "config_evaluate_filename": None,
-        "send_weight_diff": False,
-        "config_filters_filename": os.path.join(_data_dir, "config_fl_filters.json"),
-    }
-]
-TEST_GET_WEIGHTS_3 = [
-    {
-        "bundle_root": _data_dir,
         "config_train_filename": os.path.join(_data_dir, "config_fl_train.json"),
         "config_evaluate_filename": None,
         "send_weight_diff": True,
         "config_filters_filename": os.path.join(_data_dir, "config_fl_filters.json"),
     }
 ]
-TEST_GET_WEIGHTS_4 = [
+TEST_GET_WEIGHTS_3 = [
     {
         "bundle_root": _data_dir,
-        "config_train_filename": [
-            os.path.join(_data_dir, "config_fl_train.json"),
-            os.path.join(_data_dir, "config_fl_train.json"),
-        ],
+        "train_workflow": ConfigWorkflow(
+            config_file=os.path.join(_data_dir, "config_fl_train.json"), workflow="train", logging_file=_logging_file
+        ),
         "config_evaluate_filename": None,
         "send_weight_diff": True,
-        "config_filters_filename": [
-            os.path.join(_data_dir, "config_fl_filters.json"),
-            os.path.join(_data_dir, "config_fl_filters.json"),
-        ],
+        "config_filters_filename": os.path.join(_data_dir, "config_fl_filters.json"),
     }
 ]
 
 
 @SkipIfNoModule("ignite")
 @SkipIfNoModule("mlflow")
 class TestFLMonaiAlgo(unittest.TestCase):
-    @parameterized.expand([TEST_TRAIN_1, TEST_TRAIN_2, TEST_TRAIN_3])
+    @parameterized.expand([TEST_TRAIN_1, TEST_TRAIN_2, TEST_TRAIN_3, TEST_TRAIN_4])
     def test_train(self, input_params):
-        # get testing data dir and update train config; using the first to define data dir
-        if isinstance(input_params["config_train_filename"], list):
-            config_train_filename = [
-                os.path.join(input_params["bundle_root"], x) for x in input_params["config_train_filename"]
-            ]
-        else:
-            config_train_filename = os.path.join(input_params["bundle_root"], input_params["config_train_filename"])
-
-        data_dir = tempfile.mkdtemp()
-        # test experiment management
-        input_params["tracking"] = {
-            "handlers_id": DEFAULT_HANDLERS_ID,
-            "configs": {
-                "execute_config": f"{data_dir}/config_executed.json",
-                "trainer": {
-                    "_target_": "MLFlowHandler",
-                    "tracking_uri": path_to_uri(data_dir) + "/mlflow_override",
-                    "output_transform": "$monai.handlers.from_engine(['loss'], first=True)",
-                    "close_on_complete": True,
-                },
-            },
-        }
-
         # initialize algo
         algo = MonaiAlgo(**input_params)
         algo.initialize(extra={ExtraItems.CLIENT_NAME: "test_fl"})
         algo.abort()
 
         # initialize model
-        parser = ConfigParser()
-        parser.read_config(config_train_filename)
+        parser = ConfigParser(config=deepcopy(algo.train_workflow.parser.get()))
         parser.parse()
         network = parser.get_parsed_content("network")
 
         data = ExchangeObject(weights=network.state_dict())
 
         # test train
         algo.train(data=data, extra={})
         algo.finalize()
-        self.assertTrue(os.path.exists(f"{data_dir}/mlflow_override"))
-        self.assertTrue(os.path.exists(f"{data_dir}/config_executed.json"))
-        shutil.rmtree(data_dir)
+
+        # test experiment management
+        if "execute_config" in algo.train_workflow.parser:
+            self.assertTrue(os.path.exists(f"{_data_dir}/mlflow_override"))
+            shutil.rmtree(f"{_data_dir}/mlflow_override")
+            self.assertTrue(os.path.exists(f"{_data_dir}/config_executed.json"))
+            os.remove(f"{_data_dir}/config_executed.json")
 
     @parameterized.expand([TEST_EVALUATE_1, TEST_EVALUATE_2, TEST_EVALUATE_3])
     def test_evaluate(self, input_params):
-        # get testing data dir and update train config; using the first to define data dir
-        if isinstance(input_params["config_evaluate_filename"], list):
-            config_eval_filename = [
-                os.path.join(input_params["bundle_root"], x) for x in input_params["config_evaluate_filename"]
-            ]
-        else:
-            config_eval_filename = os.path.join(input_params["bundle_root"], input_params["config_evaluate_filename"])
-
         # initialize algo
         algo = MonaiAlgo(**input_params)
         algo.initialize(extra={ExtraItems.CLIENT_NAME: "test_fl"})
 
         # initialize model
-        parser = ConfigParser()
-        parser.read_config(config_eval_filename)
+        parser = ConfigParser(config=deepcopy(algo.eval_workflow.parser.get()))
         parser.parse()
         network = parser.get_parsed_content("network")
 
         data = ExchangeObject(weights=network.state_dict())
 
         # test evaluate
         algo.evaluate(data=data, extra={})
 
-    @parameterized.expand([TEST_GET_WEIGHTS_1, TEST_GET_WEIGHTS_2, TEST_GET_WEIGHTS_3, TEST_GET_WEIGHTS_4])
+        # test experiment management
+        if "execute_config" in algo.eval_workflow.parser:
+            self.assertGreater(len(list(glob.glob(f"{_data_dir}/mlflow_*"))), 0)
+            for f in list(glob.glob(f"{_data_dir}/mlflow_*")):
+                shutil.rmtree(f)
+            self.assertGreater(len(list(glob.glob(f"{_data_dir}/eval/config_*"))), 0)
+            for f in list(glob.glob(f"{_data_dir}/eval/config_*")):
+                os.remove(f)
+
+    @parameterized.expand([TEST_GET_WEIGHTS_1, TEST_GET_WEIGHTS_2, TEST_GET_WEIGHTS_3])
     def test_get_weights(self, input_params):
         # initialize algo
         algo = MonaiAlgo(**input_params)
         algo.initialize(extra={ExtraItems.CLIENT_NAME: "test_fl"})
 
         # test train
         if input_params["send_weight_diff"]:  # should not work as test doesn't receive a global model
```

### Comparing `monai-weekly-1.2.dev2316/tests/test_fl_monai_algo_stats.py` & `monai-weekly-1.2.dev2317/tests/test_fl_monai_algo_stats.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,47 +12,56 @@
 from __future__ import annotations
 
 import os
 import unittest
 
 from parameterized import parameterized
 
+from monai.bundle import ConfigWorkflow
 from monai.fl.client import MonaiAlgoStats
 from monai.fl.utils.constants import ExtraItems, FlStatistics
 from monai.fl.utils.exchange_object import ExchangeObject
 from tests.utils import SkipIfNoModule
 
 _root_dir = os.path.abspath(os.path.join(os.path.dirname(__file__)))
 _data_dir = os.path.join(_root_dir, "testing_data")
+_logging_file = os.path.join(_data_dir, "logging.conf")
 
 TEST_GET_DATA_STATS_1 = [
     {
         "bundle_root": _data_dir,
-        "config_train_filename": os.path.join(_data_dir, "config_fl_stats_1.json"),
+        "workflow": ConfigWorkflow(
+            workflow="train",
+            config_file=os.path.join(_data_dir, "config_fl_stats_1.json"),
+            logging_file=_logging_file,
+            meta_file=None,
+        ),
         "config_filters_filename": os.path.join(_data_dir, "config_fl_filters.json"),
     }
 ]
 TEST_GET_DATA_STATS_2 = [
     {
         "bundle_root": _data_dir,
         "config_train_filename": os.path.join(_data_dir, "config_fl_stats_2.json"),
         "config_filters_filename": os.path.join(_data_dir, "config_fl_filters.json"),
     }
 ]
 TEST_GET_DATA_STATS_3 = [
     {
         "bundle_root": _data_dir,
-        "config_train_filename": [
-            os.path.join(_data_dir, "config_fl_stats_1.json"),
-            os.path.join(_data_dir, "config_fl_stats_2.json"),
-        ],
-        "config_filters_filename": [
-            os.path.join(_data_dir, "config_fl_filters.json"),
-            os.path.join(_data_dir, "config_fl_filters.json"),
-        ],
+        "workflow": ConfigWorkflow(
+            workflow="train",
+            config_file=[
+                os.path.join(_data_dir, "config_fl_stats_1.json"),
+                os.path.join(_data_dir, "config_fl_stats_2.json"),
+            ],
+            logging_file=_logging_file,
+            meta_file=None,
+        ),
+        "config_filters_filename": os.path.join(_data_dir, "config_fl_filters.json"),
     }
 ]
 
 
 @SkipIfNoModule("ignite")
 class TestFLMonaiAlgo(unittest.TestCase):
     @parameterized.expand([TEST_GET_DATA_STATS_1, TEST_GET_DATA_STATS_2, TEST_GET_DATA_STATS_3])
```

### Comparing `monai-weekly-1.2.dev2316/tests/test_flatten_sub_keysd.py` & `monai-weekly-1.2.dev2317/tests/test_flatten_sub_keysd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_flexible_unet.py` & `monai-weekly-1.2.dev2317/tests/test_flexible_unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_flip.py` & `monai-weekly-1.2.dev2317/tests/test_flip.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_flipd.py` & `monai-weekly-1.2.dev2317/tests/test_flipd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_focal_loss.py` & `monai-weekly-1.2.dev2317/tests/test_focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_folder_layout.py` & `monai-weekly-1.2.dev2317/tests/test_folder_layout.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_foreground_mask.py` & `monai-weekly-1.2.dev2317/tests/test_foreground_mask.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_foreground_maskd.py` & `monai-weekly-1.2.dev2317/tests/test_foreground_maskd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_fourier.py` & `monai-weekly-1.2.dev2317/tests/test_fourier.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_fpn_block.py` & `monai-weekly-1.2.dev2317/tests/test_fpn_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_from_engine_hovernet.py` & `monai-weekly-1.2.dev2317/tests/test_from_engine_hovernet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_fullyconnectednet.py` & `monai-weekly-1.2.dev2317/tests/test_fullyconnectednet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_gaussian.py` & `monai-weekly-1.2.dev2317/tests/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_gaussian_filter.py` & `monai-weekly-1.2.dev2317/tests/test_gaussian_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_gaussian_sharpen.py` & `monai-weekly-1.2.dev2317/tests/test_gaussian_sharpen.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_gaussian_sharpend.py` & `monai-weekly-1.2.dev2317/tests/test_gaussian_sharpend.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_gaussian_smooth.py` & `monai-weekly-1.2.dev2317/tests/test_gaussian_smooth.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_gaussian_smoothd.py` & `monai-weekly-1.2.dev2317/tests/test_gaussian_smoothd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_generalized_dice_focal_loss.py` & `monai-weekly-1.2.dev2317/tests/test_generalized_dice_focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_generalized_dice_loss.py` & `monai-weekly-1.2.dev2317/tests/test_generalized_dice_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_generalized_wasserstein_dice_loss.py` & `monai-weekly-1.2.dev2317/tests/test_generalized_wasserstein_dice_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_generate_distance_map.py` & `monai-weekly-1.2.dev2317/tests/test_generate_distance_map.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_generate_distance_mapd.py` & `monai-weekly-1.2.dev2317/tests/test_generate_distance_mapd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_generate_instance_border.py` & `monai-weekly-1.2.dev2317/tests/test_generate_instance_border.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_generate_instance_borderd.py` & `monai-weekly-1.2.dev2317/tests/test_generate_instance_borderd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_generate_instance_centroid.py` & `monai-weekly-1.2.dev2317/tests/test_generate_instance_centroid.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_generate_instance_centroidd.py` & `monai-weekly-1.2.dev2317/tests/test_generate_instance_centroidd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_generate_instance_contour.py` & `monai-weekly-1.2.dev2317/tests/test_generate_instance_contour.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_generate_instance_contourd.py` & `monai-weekly-1.2.dev2317/tests/test_generate_instance_contourd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_generate_instance_type.py` & `monai-weekly-1.2.dev2317/tests/test_generate_instance_type.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_generate_instance_typed.py` & `monai-weekly-1.2.dev2317/tests/test_generate_instance_typed.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_generate_label_classes_crop_centers.py` & `monai-weekly-1.2.dev2317/tests/test_generate_label_classes_crop_centers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_generate_param_groups.py` & `monai-weekly-1.2.dev2317/tests/test_generate_param_groups.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_generate_pos_neg_label_crop_centers.py` & `monai-weekly-1.2.dev2317/tests/test_generate_pos_neg_label_crop_centers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_generate_spatial_bounding_box.py` & `monai-weekly-1.2.dev2317/tests/test_generate_spatial_bounding_box.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_generate_succinct_contour.py` & `monai-weekly-1.2.dev2317/tests/test_generate_succinct_contour.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_generate_succinct_contourd.py` & `monai-weekly-1.2.dev2317/tests/test_generate_succinct_contourd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_generate_watershed_markers.py` & `monai-weekly-1.2.dev2317/tests/test_generate_watershed_markers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_generate_watershed_markersd.py` & `monai-weekly-1.2.dev2317/tests/test_generate_watershed_markersd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_generate_watershed_mask.py` & `monai-weekly-1.2.dev2317/tests/test_generate_watershed_mask.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_generate_watershed_maskd.py` & `monai-weekly-1.2.dev2317/tests/test_generate_watershed_maskd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_generator.py` & `monai-weekly-1.2.dev2317/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_get_equivalent_dtype.py` & `monai-weekly-1.2.dev2317/tests/test_get_equivalent_dtype.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_get_extreme_points.py` & `monai-weekly-1.2.dev2317/tests/test_get_extreme_points.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_get_layers.py` & `monai-weekly-1.2.dev2317/tests/test_get_layers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_get_package_version.py` & `monai-weekly-1.2.dev2317/tests/test_get_package_version.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_get_unique_labels.py` & `monai-weekly-1.2.dev2317/tests/test_get_unique_labels.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_gibbs_noise.py` & `monai-weekly-1.2.dev2317/tests/test_gibbs_noise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_gibbs_noised.py` & `monai-weekly-1.2.dev2317/tests/test_gibbs_noised.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_giou_loss.py` & `monai-weekly-1.2.dev2317/tests/test_giou_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_global_mutual_information_loss.py` & `monai-weekly-1.2.dev2317/tests/test_global_mutual_information_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_globalnet.py` & `monai-weekly-1.2.dev2317/tests/test_globalnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_gmm.py` & `monai-weekly-1.2.dev2317/tests/test_gmm.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_grid_dataset.py` & `monai-weekly-1.2.dev2317/tests/test_grid_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_grid_distortion.py` & `monai-weekly-1.2.dev2317/tests/test_grid_distortion.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_grid_distortiond.py` & `monai-weekly-1.2.dev2317/tests/test_grid_distortiond.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_grid_patch.py` & `monai-weekly-1.2.dev2317/tests/test_grid_patch.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_grid_patchd.py` & `monai-weekly-1.2.dev2317/tests/test_grid_patchd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_grid_pull.py` & `monai-weekly-1.2.dev2317/tests/test_grid_pull.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_grid_split.py` & `monai-weekly-1.2.dev2317/tests/test_grid_split.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_grid_splitd.py` & `monai-weekly-1.2.dev2317/tests/test_grid_splitd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_handler_checkpoint_loader.py` & `monai-weekly-1.2.dev2317/tests/test_handler_checkpoint_loader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_handler_checkpoint_saver.py` & `monai-weekly-1.2.dev2317/tests/test_handler_checkpoint_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_handler_classification_saver.py` & `monai-weekly-1.2.dev2317/tests/test_handler_classification_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_handler_classification_saver_dist.py` & `monai-weekly-1.2.dev2317/tests/test_handler_classification_saver_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_handler_clearml_image.py` & `monai-weekly-1.2.dev2317/tests/test_handler_clearml_image.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_handler_clearml_stats.py` & `monai-weekly-1.2.dev2317/tests/test_handler_clearml_stats.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_handler_confusion_matrix.py` & `monai-weekly-1.2.dev2317/tests/test_handler_confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_handler_confusion_matrix_dist.py` & `monai-weekly-1.2.dev2317/tests/test_handler_confusion_matrix_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_handler_decollate_batch.py` & `monai-weekly-1.2.dev2317/tests/test_handler_decollate_batch.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_handler_early_stop.py` & `monai-weekly-1.2.dev2317/tests/test_handler_early_stop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_handler_garbage_collector.py` & `monai-weekly-1.2.dev2317/tests/test_handler_garbage_collector.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_handler_hausdorff_distance.py` & `monai-weekly-1.2.dev2317/tests/test_handler_hausdorff_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_handler_logfile.py` & `monai-weekly-1.2.dev2317/tests/test_handler_logfile.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_handler_lr_scheduler.py` & `monai-weekly-1.2.dev2317/tests/test_handler_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_handler_mean_dice.py` & `monai-weekly-1.2.dev2317/tests/test_handler_mean_iou.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,64 +13,64 @@
 
 import unittest
 
 import torch
 from ignite.engine import Engine, Events
 from parameterized import parameterized
 
-from monai.handlers import MeanDice, from_engine
+from monai.handlers import MeanIoUHandler, from_engine
 from tests.utils import assert_allclose
 
 TEST_CASE_1 = [{"include_background": True, "output_transform": from_engine(["pred", "label"])}, 0.75, (4, 2)]
-TEST_CASE_2 = [{"include_background": False, "output_transform": from_engine(["pred", "label"])}, 0.66666, (4, 1)]
+TEST_CASE_2 = [{"include_background": False, "output_transform": from_engine(["pred", "label"])}, 2 / 3, (4, 1)]
 TEST_CASE_3 = [
     {"reduction": "mean_channel", "output_transform": from_engine(["pred", "label"])},
     torch.Tensor([1.0, 0.0, 1.0, 1.0]),
     (4, 2),
 ]
 
 
-class TestHandlerMeanDice(unittest.TestCase):
-    # TODO test multi node averaged dice
+class TestHandlerMeanIoU(unittest.TestCase):
+    # TODO test multi node averaged iou
 
     @parameterized.expand([TEST_CASE_1, TEST_CASE_2, TEST_CASE_3])
     def test_compute(self, input_params, expected_avg, details_shape):
-        dice_metric = MeanDice(**input_params)
+        iou_metric = MeanIoUHandler(**input_params)
 
         # set up engine
 
         def _val_func(engine, batch):
             pass
 
         engine = Engine(_val_func)
-        dice_metric.attach(engine=engine, name="mean_dice")
+        iou_metric.attach(engine=engine, name="mean_iou")
         # test input a list of channel-first tensor
         y_pred = [torch.Tensor([[0], [1]]), torch.Tensor([[1], [0]])]
         y = torch.Tensor([[[0], [1]], [[0], [1]]])
         engine.state.output = {"pred": y_pred, "label": y}
         engine.fire_event(Events.ITERATION_COMPLETED)
 
         y_pred = [torch.Tensor([[0], [1]]), torch.Tensor([[1], [0]])]
         y = torch.Tensor([[[0], [1]], [[1], [0]]])
         engine.state.output = {"pred": y_pred, "label": y}
         engine.fire_event(Events.ITERATION_COMPLETED)
 
         engine.fire_event(Events.EPOCH_COMPLETED)
-        assert_allclose(engine.state.metrics["mean_dice"], expected_avg, atol=1e-4, rtol=1e-4, type_test=False)
-        self.assertTupleEqual(tuple(engine.state.metric_details["mean_dice"].shape), details_shape)
+        assert_allclose(engine.state.metrics["mean_iou"], expected_avg)
+        self.assertTupleEqual(tuple(engine.state.metric_details["mean_iou"].shape), details_shape)
 
     @parameterized.expand([TEST_CASE_1, TEST_CASE_2])
     def test_shape_mismatch(self, input_params, _expected_avg, _details_shape):
-        dice_metric = MeanDice(**input_params)
+        iou_metric = MeanIoUHandler(**input_params)
         with self.assertRaises((AssertionError, ValueError)):
             y_pred = torch.Tensor([[0, 1], [1, 0]])
-            y = torch.ones((2, 3))
-            dice_metric.update([y_pred, y])
+            y = torch.ones((3, 30))
+            iou_metric.update([y_pred, y])
 
         with self.assertRaises((AssertionError, ValueError)):
             y_pred = torch.Tensor([[0, 1], [1, 0]])
-            y = torch.ones((3, 2))
-            dice_metric.update([y_pred, y])
+            y = torch.ones((8, 30))
+            iou_metric.update([y_pred, y])
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai-weekly-1.2.dev2316/tests/test_handler_mean_iou.py` & `monai-weekly-1.2.dev2317/tests/test_handler_metric_logger.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,67 +10,53 @@
 # limitations under the License.
 
 from __future__ import annotations
 
 import unittest
 
 import torch
-from ignite.engine import Engine, Events
-from parameterized import parameterized
 
-from monai.handlers import MeanIoUHandler, from_engine
-from tests.utils import assert_allclose
+from monai.utils import optional_import
+from tests.utils import SkipIfNoModule
 
-TEST_CASE_1 = [{"include_background": True, "output_transform": from_engine(["pred", "label"])}, 0.75, (4, 2)]
-TEST_CASE_2 = [{"include_background": False, "output_transform": from_engine(["pred", "label"])}, 2 / 3, (4, 1)]
-TEST_CASE_3 = [
-    {"reduction": "mean_channel", "output_transform": from_engine(["pred", "label"])},
-    torch.Tensor([1.0, 0.0, 1.0, 1.0]),
-    (4, 2),
-]
-
-
-class TestHandlerMeanIoU(unittest.TestCase):
-    # TODO test multi node averaged iou
-
-    @parameterized.expand([TEST_CASE_1, TEST_CASE_2, TEST_CASE_3])
-    def test_compute(self, input_params, expected_avg, details_shape):
-        iou_metric = MeanIoUHandler(**input_params)
+try:
+    _, has_ignite = optional_import("ignite")
+    from ignite.engine import Engine, Events
+
+    from monai.handlers import MetricLogger
+except ImportError:
+    has_ignite = False
+
+
+class TestHandlerMetricLogger(unittest.TestCase):
+    @SkipIfNoModule("ignite")
+    def test_metric_logging(self):
+        dummy_name = "dummy"
 
         # set up engine
+        def _train_func(engine, batch):
+            return torch.tensor(0.0)
 
-        def _val_func(engine, batch):
-            pass
+        engine = Engine(_train_func)
 
-        engine = Engine(_val_func)
-        iou_metric.attach(engine=engine, name="mean_iou")
-        # test input a list of channel-first tensor
-        y_pred = [torch.Tensor([[0], [1]]), torch.Tensor([[1], [0]])]
-        y = torch.Tensor([[[0], [1]], [[0], [1]]])
-        engine.state.output = {"pred": y_pred, "label": y}
-        engine.fire_event(Events.ITERATION_COMPLETED)
-
-        y_pred = [torch.Tensor([[0], [1]]), torch.Tensor([[1], [0]])]
-        y = torch.Tensor([[[0], [1]], [[1], [0]]])
-        engine.state.output = {"pred": y_pred, "label": y}
-        engine.fire_event(Events.ITERATION_COMPLETED)
-
-        engine.fire_event(Events.EPOCH_COMPLETED)
-        assert_allclose(engine.state.metrics["mean_iou"], expected_avg)
-        self.assertTupleEqual(tuple(engine.state.metric_details["mean_iou"].shape), details_shape)
-
-    @parameterized.expand([TEST_CASE_1, TEST_CASE_2])
-    def test_shape_mismatch(self, input_params, _expected_avg, _details_shape):
-        iou_metric = MeanIoUHandler(**input_params)
-        with self.assertRaises((AssertionError, ValueError)):
-            y_pred = torch.Tensor([[0, 1], [1, 0]])
-            y = torch.ones((3, 30))
-            iou_metric.update([y_pred, y])
-
-        with self.assertRaises((AssertionError, ValueError)):
-            y_pred = torch.Tensor([[0, 1], [1, 0]])
-            y = torch.ones((8, 30))
-            iou_metric.update([y_pred, y])
+        # set up dummy metric
+        @engine.on(Events.EPOCH_COMPLETED)
+        def _update_metric(engine):
+            engine.state.metrics[dummy_name] = 1
+
+        # set up testing handler
+        handler = MetricLogger(loss_transform=lambda output: output.item())
+        handler.attach(engine)
+
+        engine.run(range(3), max_epochs=2)
+
+        expected_loss = [(1, 0.0), (2, 0.0), (3, 0.0), (4, 0.0), (5, 0.0), (6, 0.0)]
+        expected_metric = [(4, 1), (5, 1), (6, 1)]
+
+        self.assertSetEqual({dummy_name}, set(handler.metrics))
+
+        self.assertListEqual(expected_loss, handler.loss)
+        self.assertListEqual(expected_metric, handler.metrics[dummy_name])
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai-weekly-1.2.dev2316/tests/test_handler_metric_logger.py` & `monai-weekly-1.2.dev2317/tests/test_integration_determinism.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,54 +9,82 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 import unittest
 
+import numpy as np
 import torch
+from torch.utils.data import DataLoader, Dataset
 
-from monai.utils import optional_import
-from tests.utils import SkipIfNoModule
-
-try:
-    _, has_ignite = optional_import("ignite")
-    from ignite.engine import Engine, Events
-
-    from monai.handlers import MetricLogger
-except ImportError:
-    has_ignite = False
-
-
-class TestHandlerMetricLogger(unittest.TestCase):
-    @SkipIfNoModule("ignite")
-    def test_metric_logging(self):
-        dummy_name = "dummy"
-
-        # set up engine
-        def _train_func(engine, batch):
-            return torch.tensor(0.0)
-
-        engine = Engine(_train_func)
-
-        # set up dummy metric
-        @engine.on(Events.EPOCH_COMPLETED)
-        def _update_metric(engine):
-            engine.state.metrics[dummy_name] = 1
-
-        # set up testing handler
-        handler = MetricLogger(loss_transform=lambda output: output.item())
-        handler.attach(engine)
-
-        engine.run(range(3), max_epochs=2)
-
-        expected_loss = [(1, 0.0), (2, 0.0), (3, 0.0), (4, 0.0), (5, 0.0), (6, 0.0)]
-        expected_metric = [(4, 1), (5, 1), (6, 1)]
-
-        self.assertSetEqual({dummy_name}, set(handler.metrics))
-
-        self.assertListEqual(expected_loss, handler.loss)
-        self.assertListEqual(expected_metric, handler.metrics[dummy_name])
+from monai.data import create_test_image_2d
+from monai.losses import DiceLoss
+from monai.networks.nets import UNet
+from monai.transforms import AddChannel, Compose, RandRotate90, RandSpatialCrop, ScaleIntensity
+from monai.utils import set_determinism
+from tests.utils import DistTestCase, TimedCall
+
+
+def run_test(batch_size=64, train_steps=200, device="cuda:0"):
+    class _TestBatch(Dataset):
+        def __init__(self, transforms):
+            self.transforms = transforms
+
+        def __getitem__(self, _unused_id):
+            im, seg = create_test_image_2d(128, 128, noise_max=1, num_objs=4, num_seg_classes=1)
+            seed = np.random.randint(2147483647)
+            self.transforms.set_random_state(seed=seed)
+            im = self.transforms(im)
+            self.transforms.set_random_state(seed=seed)
+            seg = self.transforms(seg)
+            return im, seg
+
+        def __len__(self):
+            return train_steps
+
+    net = UNet(
+        spatial_dims=2, in_channels=1, out_channels=1, channels=(4, 8, 16, 32), strides=(2, 2, 2), num_res_units=2
+    ).to(device)
+
+    loss = DiceLoss(sigmoid=True)
+    opt = torch.optim.Adam(net.parameters(), 1e-2)
+    train_transforms = Compose(
+        [AddChannel(), ScaleIntensity(), RandSpatialCrop((96, 96), random_size=False), RandRotate90()]
+    )
+
+    src = DataLoader(_TestBatch(train_transforms), batch_size=batch_size, shuffle=True)
+
+    net.train()
+    epoch_loss = 0
+    step = 0
+    for img, seg in src:
+        step += 1
+        opt.zero_grad()
+        output = net(img.to(device))
+        step_loss = loss(output, seg.to(device))
+        step_loss.backward()
+        opt.step()
+        epoch_loss += step_loss.item()
+    epoch_loss /= step
+
+    return epoch_loss, step
+
+
+class TestDeterminism(DistTestCase):
+    def setUp(self):
+        self.device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu:0")
+
+    def tearDown(self):
+        set_determinism(seed=None)
+
+    @TimedCall(seconds=150, skip_timing=not torch.cuda.is_available())
+    def test_training(self):
+        set_determinism(seed=0)
+        loss, step = run_test(device=self.device)
+        print(f"Deterministic loss {loss} at training step {step}")
+        np.testing.assert_allclose(step, 4)
+        np.testing.assert_allclose(loss, 0.536134, rtol=1e-4)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai-weekly-1.2.dev2316/tests/test_handler_metrics_reloaded.py` & `monai-weekly-1.2.dev2317/tests/test_handler_metrics_reloaded.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_handler_metrics_saver.py` & `monai-weekly-1.2.dev2317/tests/test_handler_metrics_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_handler_metrics_saver_dist.py` & `monai-weekly-1.2.dev2317/tests/test_handler_metrics_saver_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_handler_mlflow.py` & `monai-weekly-1.2.dev2317/tests/test_handler_mlflow.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_handler_nvtx.py` & `monai-weekly-1.2.dev2317/tests/test_handler_nvtx.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_handler_panoptic_quality.py` & `monai-weekly-1.2.dev2317/tests/test_handler_panoptic_quality.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_handler_parameter_scheduler.py` & `monai-weekly-1.2.dev2317/tests/test_handler_parameter_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_handler_post_processing.py` & `monai-weekly-1.2.dev2317/tests/test_handler_post_processing.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_handler_prob_map_producer.py` & `monai-weekly-1.2.dev2317/tests/test_handler_prob_map_producer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_handler_regression_metrics.py` & `monai-weekly-1.2.dev2317/tests/test_handler_regression_metrics.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_handler_regression_metrics_dist.py` & `monai-weekly-1.2.dev2317/tests/test_handler_regression_metrics_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_handler_rocauc.py` & `monai-weekly-1.2.dev2317/tests/test_handler_rocauc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_handler_rocauc_dist.py` & `monai-weekly-1.2.dev2317/tests/test_handler_rocauc_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_handler_smartcache.py` & `monai-weekly-1.2.dev2317/tests/test_handler_smartcache.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_handler_stats.py` & `monai-weekly-1.2.dev2317/tests/test_handler_stats.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_handler_surface_distance.py` & `monai-weekly-1.2.dev2317/tests/test_handler_surface_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_handler_tb_image.py` & `monai-weekly-1.2.dev2317/tests/test_handler_tb_image.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_handler_tb_stats.py` & `monai-weekly-1.2.dev2317/tests/test_handler_tb_stats.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_handler_validation.py` & `monai-weekly-1.2.dev2317/tests/test_handler_validation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_hardnegsampler.py` & `monai-weekly-1.2.dev2317/tests/test_hardnegsampler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_hashing.py` & `monai-weekly-1.2.dev2317/tests/test_hashing.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_hausdorff_distance.py` & `monai-weekly-1.2.dev2317/tests/test_hausdorff_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_header_correct.py` & `monai-weekly-1.2.dev2317/tests/test_header_correct.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_highresnet.py` & `monai-weekly-1.2.dev2317/tests/test_highresnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_hilbert_transform.py` & `monai-weekly-1.2.dev2317/tests/test_hilbert_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_histogram_normalize.py` & `monai-weekly-1.2.dev2317/tests/test_histogram_normalize.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_histogram_normalized.py` & `monai-weekly-1.2.dev2317/tests/test_histogram_normalized.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_hovernet.py` & `monai-weekly-1.2.dev2317/tests/test_hovernet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_hovernet_instance_map_post_processing.py` & `monai-weekly-1.2.dev2317/tests/test_hovernet_instance_map_post_processing.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_hovernet_instance_map_post_processingd.py` & `monai-weekly-1.2.dev2317/tests/test_hovernet_instance_map_post_processingd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_hovernet_loss.py` & `monai-weekly-1.2.dev2317/tests/test_hovernet_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_hovernet_nuclear_type_post_processing.py` & `monai-weekly-1.2.dev2317/tests/test_hovernet_nuclear_type_post_processing.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_hovernet_nuclear_type_post_processingd.py` & `monai-weekly-1.2.dev2317/tests/test_hovernet_nuclear_type_post_processingd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_identity.py` & `monai-weekly-1.2.dev2317/tests/test_identity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_identityd.py` & `monai-weekly-1.2.dev2317/tests/test_identityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_image_dataset.py` & `monai-weekly-1.2.dev2317/tests/test_image_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_image_filter.py` & `monai-weekly-1.2.dev2317/tests/test_image_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_image_rw.py` & `monai-weekly-1.2.dev2317/tests/test_image_rw.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_img2tensorboard.py` & `monai-weekly-1.2.dev2317/tests/test_img2tensorboard.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_init_reader.py` & `monai-weekly-1.2.dev2317/tests/test_init_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_integration_autorunner.py` & `monai-weekly-1.2.dev2317/tests/test_integration_autorunner.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,14 +54,15 @@
     {
         "num_images_per_batch": num_images_per_batch,
         "num_epochs": 2,
         "num_epochs_per_validation": 1,
         "num_warmup_epochs": 1,
         "use_pretrain": False,
         "pretrained_path": "",
+        "num_steps_per_image": 1,
     }
     if torch.cuda.is_available()
     else {}
 )
 
 pred_param = {"files_slices": slice(0, 1), "mode": "mean", "sigmoid": True}
 
@@ -108,38 +109,47 @@
         self.data_src_cfg = data_src_cfg
         self.test_path = test_path
 
     @skip_if_no_cuda
     def test_autorunner(self) -> None:
         work_dir = os.path.join(self.test_path, "work_dir")
         runner = AutoRunner(
-            work_dir=work_dir, input=self.data_src_cfg, templates_path_or_url=get_testing_algo_template_path()
+            work_dir=work_dir,
+            input=self.data_src_cfg,
+            templates_path_or_url=get_testing_algo_template_path(),
+            allow_skip=False,
         )
         runner.set_training_params(train_param)  # 2 epochs
         runner.set_num_fold(1)
         with skip_if_downloading_fails():
             runner.run()
 
     @skip_if_no_cuda
     def test_autorunner_ensemble(self) -> None:
         work_dir = os.path.join(self.test_path, "work_dir")
         runner = AutoRunner(
-            work_dir=work_dir, input=self.data_src_cfg, templates_path_or_url=get_testing_algo_template_path()
+            work_dir=work_dir,
+            input=self.data_src_cfg,
+            templates_path_or_url=get_testing_algo_template_path(),
+            allow_skip=False,
         )
         runner.set_training_params(train_param)  # 2 epochs
         runner.set_ensemble_method("AlgoEnsembleBestByFold")
         runner.set_num_fold(1)
         with skip_if_downloading_fails():
             runner.run()
 
     @skip_if_no_cuda
     def test_autorunner_gpu_customization(self) -> None:
         work_dir = os.path.join(self.test_path, "work_dir")
         runner = AutoRunner(
-            work_dir=work_dir, input=self.data_src_cfg, templates_path_or_url=get_testing_algo_template_path()
+            work_dir=work_dir,
+            input=self.data_src_cfg,
+            templates_path_or_url=get_testing_algo_template_path(),
+            allow_skip=False,
         )
         gpu_customization_specs = {
             "universal": {"num_trials": 1, "range_num_images_per_batch": [1, 2], "range_num_sw_batch_size": [1, 2]}
         }
         runner.set_gpu_customization(gpu_customization=True, gpu_customization_specs=gpu_customization_specs)
         runner.set_training_params(train_param)  # 2 epochs
         runner.set_num_fold(1)
@@ -152,14 +162,15 @@
         work_dir = os.path.join(self.test_path, "work_dir")
         runner = AutoRunner(
             work_dir=work_dir,
             input=self.data_src_cfg,
             hpo=True,
             ensemble=False,
             templates_path_or_url=get_testing_algo_template_path(),
+            allow_skip=False,
         )
         hpo_param = {
             "num_epochs_per_validation": train_param["num_epochs_per_validation"],
             "num_images_per_batch": train_param["num_images_per_batch"],
             "num_epochs": train_param["num_epochs"],
             "num_warmup_epochs": train_param["num_warmup_epochs"],
             "use_pretrain": train_param["use_pretrain"],
```

### Comparing `monai-weekly-1.2.dev2316/tests/test_integration_bundle_run.py` & `monai-weekly-1.2.dev2317/tests/test_integration_bundle_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,17 @@
                 },
                 f,
             )
         cmd = ["coverage", "run", "-m", "monai.bundle"]
         # test both CLI entry "run" and "run_workflow"
         command_line_tests(cmd + ["run", "training", "--config_file", config_file])
         command_line_tests(cmd + ["run_workflow", "--run_id", "training", "--config_file", config_file])
+        with self.assertRaises(RuntimeError):
+            # test wrong run_id="run"
+            command_line_tests(cmd + ["run", "run", "--config_file", config_file])
 
     @parameterized.expand([TEST_CASE_1, TEST_CASE_2])
     def test_shape(self, config_file, expected_shape):
         test_image = np.random.rand(*expected_shape)
         tempdir = self.data_dir
         filename = os.path.join(tempdir, "image.nii")
         nib.save(nib.Nifti1Image(test_image, np.eye(4)), filename)
```

### Comparing `monai-weekly-1.2.dev2316/tests/test_integration_classification_2d.py` & `monai-weekly-1.2.dev2317/tests/test_integration_classification_2d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_integration_determinism.py` & `monai-weekly-1.2.dev2317/tests/test_integration_unet_2d.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,80 +11,56 @@
 
 from __future__ import annotations
 
 import unittest
 
 import numpy as np
 import torch
+from ignite.engine import create_supervised_trainer
 from torch.utils.data import DataLoader, Dataset
 
 from monai.data import create_test_image_2d
 from monai.losses import DiceLoss
-from monai.networks.nets import UNet
-from monai.transforms import AddChannel, Compose, RandRotate90, RandSpatialCrop, ScaleIntensity
-from monai.utils import set_determinism
-from tests.utils import DistTestCase, TimedCall
+from monai.networks.nets import BasicUNet, UNet
+from tests.utils import DistTestCase, TimedCall, skip_if_quick
 
 
-def run_test(batch_size=64, train_steps=200, device="cuda:0"):
+def run_test(net_name="basicunet", batch_size=64, train_steps=100, device="cuda:0"):
     class _TestBatch(Dataset):
-        def __init__(self, transforms):
-            self.transforms = transforms
-
         def __getitem__(self, _unused_id):
             im, seg = create_test_image_2d(128, 128, noise_max=1, num_objs=4, num_seg_classes=1)
-            seed = np.random.randint(2147483647)
-            self.transforms.set_random_state(seed=seed)
-            im = self.transforms(im)
-            self.transforms.set_random_state(seed=seed)
-            seg = self.transforms(seg)
-            return im, seg
+            return im[None], seg[None].astype(np.float32)
 
         def __len__(self):
             return train_steps
 
-    net = UNet(
-        spatial_dims=2, in_channels=1, out_channels=1, channels=(4, 8, 16, 32), strides=(2, 2, 2), num_res_units=2
-    ).to(device)
+    if net_name == "basicunet":
+        net = BasicUNet(spatial_dims=2, in_channels=1, out_channels=1, features=(4, 8, 8, 16, 16, 32))
+    elif net_name == "unet":
+        net = UNet(
+            spatial_dims=2, in_channels=1, out_channels=1, channels=(4, 8, 16, 32), strides=(2, 2, 2), num_res_units=2
+        )
+    net.to(device)
 
     loss = DiceLoss(sigmoid=True)
-    opt = torch.optim.Adam(net.parameters(), 1e-2)
-    train_transforms = Compose(
-        [AddChannel(), ScaleIntensity(), RandSpatialCrop((96, 96), random_size=False), RandRotate90()]
-    )
-
-    src = DataLoader(_TestBatch(train_transforms), batch_size=batch_size, shuffle=True)
-
-    net.train()
-    epoch_loss = 0
-    step = 0
-    for img, seg in src:
-        step += 1
-        opt.zero_grad()
-        output = net(img.to(device))
-        step_loss = loss(output, seg.to(device))
-        step_loss.backward()
-        opt.step()
-        epoch_loss += step_loss.item()
-    epoch_loss /= step
-
-    return epoch_loss, step
-
-
-class TestDeterminism(DistTestCase):
-    def setUp(self):
-        self.device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu:0")
-
-    def tearDown(self):
-        set_determinism(seed=None)
-
-    @TimedCall(seconds=150, skip_timing=not torch.cuda.is_available())
-    def test_training(self):
-        set_determinism(seed=0)
-        loss, step = run_test(device=self.device)
-        print(f"Deterministic loss {loss} at training step {step}")
-        np.testing.assert_allclose(step, 4)
-        np.testing.assert_allclose(loss, 0.536134, rtol=1e-4)
+    opt = torch.optim.Adam(net.parameters(), 1e-4)
+    src = DataLoader(_TestBatch(), batch_size=batch_size)
+
+    trainer = create_supervised_trainer(net, opt, loss, device, False)
+
+    trainer.run(src, 1)
+    loss = trainer.state.output
+    return loss
+
+
+@skip_if_quick
+class TestIntegrationUnet2D(DistTestCase):
+    @TimedCall(seconds=20, daemon=False)
+    def test_unet_training(self):
+        for n in ["basicunet", "unet"]:
+            loss = run_test(net_name=n, device=torch.device("cuda:0" if torch.cuda.is_available() else "cpu:0"))
+            print(loss)
+            self.assertGreaterEqual(0.85, loss)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai-weekly-1.2.dev2316/tests/test_integration_fast_train.py` & `monai-weekly-1.2.dev2317/tests/test_integration_fast_train.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_integration_gpu_customization.py` & `monai-weekly-1.2.dev2317/tests/test_integration_gpu_customization.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_integration_lazy_samples.py` & `monai-weekly-1.2.dev2317/tests/test_integration_lazy_samples.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,19 +19,23 @@
 
 import nibabel as nib
 import numpy as np
 import torch
 
 import monai
 import monai.transforms as mt
-from monai.data import create_test_image_3d
+from monai.data import create_test_image_3d, decollate_batch
 from monai.utils import set_determinism
 from tests.utils import HAS_CUPY, DistTestCase, SkipIfBeforePyTorchVersion, skip_if_quick
 
 
+def _no_op(x):
+    return x
+
+
 def run_training_test(root_dir, device="cuda:0", cachedataset=0, readers=(None, None), num_workers=4, lazy=True):
     print(f"test case: {locals()}")
     images = sorted(glob(os.path.join(root_dir, "img*.nii.gz")))
     segs = sorted(glob(os.path.join(root_dir, "seg*.nii.gz")))
     train_files = [{"img": img, "seg": seg} for img, seg in zip(images[:20], segs[:20])]
     device = "cuda:0" if HAS_CUPY and torch.cuda.is_available() else "cpu"  # mode 0 and cuda requires CUPY
     num_workers = 0 if torch.cuda.is_available() else num_workers
@@ -60,14 +64,15 @@
             ),
             mt.RandRotate90d(keys=["img", "seg"], prob=0.8, spatial_axes=(0, 2)),
             mt.RandZoomd(
                 keys=["img", "seg"], prob=1.0, min_zoom=1.0, max_zoom=1.0, mode=("trilinear", 0), keep_size=True
             ),
             mt.ResizeWithPadOrCropD(keys=["img", "seg"], spatial_size=[80, 72, 80]),
             mt.Rotated(keys=["img", "seg"], angle=[np.pi / 2, np.pi / 2, 0], mode="nearest", keep_size=False),
+            mt.Lambdad(keys=["img"], func=_no_op),
         ],
         lazy_evaluation=lazy,
         overrides=lazy_kwargs,
         override_keys=("img", "seg"),
         verbose=num_workers > 0,  # testing both flags
     )
 
@@ -94,29 +99,30 @@
         output_ext=".nii.gz",
         output_postfix=f"seg_{lazy}_{num_workers}",
         mode="bilinear",
         resample=False,
         separate_folder=False,
         print_log=False,
     )
+    inverter = mt.Invertd(
+        keys="seg", orig_keys="img", transform=mt.Compose(train_transforms.transforms[-5:]), to_tensor=True
+    )
 
     # use batch_size=2 to load images and use RandCropByPosNegLabeld to generate 2 x 4 images for network training
     _g = torch.Generator()
     _g.manual_seed(0)
     set_determinism(0)
     train_loader = monai.data.DataLoader(
         train_ds, batch_size=1, shuffle=True, num_workers=num_workers, generator=_g, persistent_workers=num_workers > 0
     )
     all_coords = set()
     for epoch in range(5):
         print("-" * 10)
         print(f"Epoch {epoch + 1}/5")
-        step = 0
-        for batch_data in train_loader:
-            step += 1
+        for step, batch_data in enumerate(train_loader, start=1):
             inputs, labels = batch_data["img"].to(device), batch_data["seg"].to(device)
             optimizer.zero_grad()
             outputs = model(inputs)
             loss = loss_function(outputs, labels)
             loss.backward()
             optimizer.step()
             epoch_len = len(train_ds) // train_loader.batch_size
@@ -139,14 +145,24 @@
                 coords = f"{img_name} - {ops}"
                 print(coords)
                 # np.testing.assert_allclose(coords in all_coords, False)
                 all_coords.add(coords)
                 saver(item)  # just testing the saving
                 saver(in_img)
                 saver(in_seg)
+    if lazy:
+        inverted = 0
+        try:
+            inverted = [inverter(b_data) for b_data in decollate_batch(batch_data)]
+        except RuntimeError as e:
+            if "Lambda" in str(e):
+                inverted = None
+        assert inverted is None, "invert LambdaD + lazy is not supported"
+    else:
+        [inverter(b_data) for b_data in decollate_batch(batch_data)]  # expecting no error
     return ops
 
 
 @skip_if_quick
 @SkipIfBeforePyTorchVersion((1, 11))
 class IntegrationLazyResampling(DistTestCase):
     def setUp(self):
```

### Comparing `monai-weekly-1.2.dev2316/tests/test_integration_nnunetv2_runner.py` & `monai-weekly-1.2.dev2317/tests/test_integration_nnunetv2_runner.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_integration_segmentation_3d.py` & `monai-weekly-1.2.dev2317/tests/test_integration_segmentation_3d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_integration_sliding_window.py` & `monai-weekly-1.2.dev2317/tests/test_integration_sliding_window.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_integration_stn.py` & `monai-weekly-1.2.dev2317/tests/test_integration_stn.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_integration_unet_2d.py` & `monai-weekly-1.2.dev2317/tests/test_integration_workers.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,56 +11,51 @@
 
 from __future__ import annotations
 
 import unittest
 
 import numpy as np
 import torch
-from ignite.engine import create_supervised_trainer
-from torch.utils.data import DataLoader, Dataset
 
-from monai.data import create_test_image_2d
-from monai.losses import DiceLoss
-from monai.networks.nets import BasicUNet, UNet
-from tests.utils import DistTestCase, TimedCall, skip_if_quick
-
-
-def run_test(net_name="basicunet", batch_size=64, train_steps=100, device="cuda:0"):
-    class _TestBatch(Dataset):
-        def __getitem__(self, _unused_id):
-            im, seg = create_test_image_2d(128, 128, noise_max=1, num_objs=4, num_seg_classes=1)
-            return im[None], seg[None].astype(np.float32)
-
-        def __len__(self):
-            return train_steps
-
-    if net_name == "basicunet":
-        net = BasicUNet(spatial_dims=2, in_channels=1, out_channels=1, features=(4, 8, 8, 16, 16, 32))
-    elif net_name == "unet":
-        net = UNet(
-            spatial_dims=2, in_channels=1, out_channels=1, channels=(4, 8, 16, 32), strides=(2, 2, 2), num_res_units=2
-        )
-    net.to(device)
-
-    loss = DiceLoss(sigmoid=True)
-    opt = torch.optim.Adam(net.parameters(), 1e-4)
-    src = DataLoader(_TestBatch(), batch_size=batch_size)
-
-    trainer = create_supervised_trainer(net, opt, loss, device, False)
-
-    trainer.run(src, 1)
-    loss = trainer.state.output
-    return loss
+from monai.data import DataLoader
+from monai.utils import set_determinism
+from tests.utils import DistTestCase, SkipIfBeforePyTorchVersion, TimedCall, skip_if_no_cuda, skip_if_quick
+
+
+def run_loading_test(num_workers=50, device=None, pw=False):
+    """multi workers stress tests"""
+    set_determinism(seed=0)
+    if device is None:
+        device = "cuda:0" if torch.cuda.is_available() else "cpu"
+    train_ds = list(range(10000))
+    train_loader = DataLoader(train_ds, batch_size=300, shuffle=True, num_workers=num_workers, persistent_workers=pw)
+    answer = []
+    for _ in range(2):
+        np.testing.assert_equal(torch.cuda.memory_allocated(), 0)
+        for batch_data in train_loader:
+            x = batch_data.to(device)
+            mem = torch.cuda.memory_allocated()
+            np.testing.assert_equal(mem > 0 and mem < 5000, True)
+        answer.append(x[-1].item())
+        del x
+    return answer
 
 
 @skip_if_quick
-class TestIntegrationUnet2D(DistTestCase):
-    @TimedCall(seconds=20, daemon=False)
-    def test_unet_training(self):
-        for n in ["basicunet", "unet"]:
-            loss = run_test(net_name=n, device=torch.device("cuda:0" if torch.cuda.is_available() else "cpu:0"))
-            print(loss)
-            self.assertGreaterEqual(0.85, loss)
+@skip_if_no_cuda
+@SkipIfBeforePyTorchVersion((1, 9))
+class IntegrationLoading(DistTestCase):
+    def tearDown(self):
+        set_determinism(seed=None)
+
+    @TimedCall(seconds=5000, skip_timing=not torch.cuda.is_available(), daemon=False)
+    def test_timing(self):
+        expected = None
+        for pw in (False, True):
+            result = run_loading_test(pw=pw)
+            if expected is None:
+                expected = result[0]
+        np.testing.assert_allclose(result[0], expected)  # test for deterministic first epoch in two settings
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai-weekly-1.2.dev2316/tests/test_integration_workers.py` & `monai-weekly-1.2.dev2317/tests/test_rand_gaussian_noised.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,51 +11,40 @@
 
 from __future__ import annotations
 
 import unittest
 
 import numpy as np
 import torch
+from parameterized import parameterized
 
-from monai.data import DataLoader
-from monai.utils import set_determinism
-from tests.utils import DistTestCase, SkipIfBeforePyTorchVersion, TimedCall, skip_if_no_cuda, skip_if_quick
-
-
-def run_loading_test(num_workers=50, device=None, pw=False):
-    """multi workers stress tests"""
-    set_determinism(seed=0)
-    if device is None:
-        device = "cuda:0" if torch.cuda.is_available() else "cpu"
-    train_ds = list(range(10000))
-    train_loader = DataLoader(train_ds, batch_size=300, shuffle=True, num_workers=num_workers, persistent_workers=pw)
-    answer = []
-    for _ in range(2):
-        np.testing.assert_equal(torch.cuda.memory_allocated(), 0)
-        for batch_data in train_loader:
-            x = batch_data.to(device)
-            mem = torch.cuda.memory_allocated()
-            np.testing.assert_equal(mem > 0 and mem < 5000, True)
-        answer.append(x[-1].item())
-        del x
-    return answer
-
-
-@skip_if_quick
-@skip_if_no_cuda
-@SkipIfBeforePyTorchVersion((1, 9))
-class IntegrationLoading(DistTestCase):
-    def tearDown(self):
-        set_determinism(seed=None)
-
-    @TimedCall(seconds=5000, skip_timing=not torch.cuda.is_available(), daemon=False)
-    def test_timing(self):
-        expected = None
-        for pw in (False, True):
-            result = run_loading_test(pw=pw)
-            if expected is None:
-                expected = result[0]
-        np.testing.assert_allclose(result[0], expected)  # test for deterministic first epoch in two settings
+from monai.transforms import RandGaussianNoised
+from tests.utils import TEST_NDARRAYS, NumpyImageTestCase2D
+
+TESTS = []
+for p in TEST_NDARRAYS:
+    TESTS.append(["test_zero_mean", p, ["img1", "img2"], 0, 0.1])
+    TESTS.append(["test_non_zero_mean", p, ["img1", "img2"], 1, 0.5])
+
+seed = 0
+
+
+class TestRandGaussianNoised(NumpyImageTestCase2D):
+    @parameterized.expand(TESTS)
+    def test_correct_results(self, _, im_type, keys, mean, std):
+        gaussian_fn = RandGaussianNoised(keys=keys, prob=1.0, mean=mean, std=std, dtype=np.float64)
+        gaussian_fn.set_random_state(seed)
+        im = im_type(self.imt)
+        noised = gaussian_fn({k: im for k in keys})
+        np.random.seed(seed)
+        # simulate the randomize() of transform
+        np.random.random()
+        noise = np.random.normal(mean, np.random.uniform(0, std), size=self.imt.shape)
+        for k in keys:
+            expected = self.imt + noise
+            if isinstance(noised[k], torch.Tensor):
+                noised[k] = noised[k].cpu()
+            np.testing.assert_allclose(expected, noised[k], atol=1e-5, rtol=1e-5)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai-weekly-1.2.dev2316/tests/test_integration_workflows.py` & `monai-weekly-1.2.dev2317/tests/test_integration_workflows.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_integration_workflows_gan.py` & `monai-weekly-1.2.dev2317/tests/test_integration_workflows_gan.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_intensity_stats.py` & `monai-weekly-1.2.dev2317/tests/test_intensity_stats.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_intensity_statsd.py` & `monai-weekly-1.2.dev2317/tests/test_intensity_statsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_inverse.py` & `monai-weekly-1.2.dev2317/tests/test_inverse.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_inverse_array.py` & `monai-weekly-1.2.dev2317/tests/test_inverse_array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_inverse_collation.py` & `monai-weekly-1.2.dev2317/tests/test_inverse_collation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_invert.py` & `monai-weekly-1.2.dev2317/tests/test_invert.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_invertd.py` & `monai-weekly-1.2.dev2317/tests/test_invertd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_is_supported_format.py` & `monai-weekly-1.2.dev2317/tests/test_is_supported_format.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_iterable_dataset.py` & `monai-weekly-1.2.dev2317/tests/test_iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_itk_torch_bridge.py` & `monai-weekly-1.2.dev2317/tests/test_itk_torch_bridge.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_itk_writer.py` & `monai-weekly-1.2.dev2317/tests/test_itk_writer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_k_space_spike_noise.py` & `monai-weekly-1.2.dev2317/tests/test_k_space_spike_noise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_k_space_spike_noised.py` & `monai-weekly-1.2.dev2317/tests/test_k_space_spike_noised.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_keep_largest_connected_component.py` & `monai-weekly-1.2.dev2317/tests/test_keep_largest_connected_component.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_keep_largest_connected_componentd.py` & `monai-weekly-1.2.dev2317/tests/test_keep_largest_connected_componentd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_kspace_mask.py` & `monai-weekly-1.2.dev2317/tests/test_kspace_mask.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_label_filter.py` & `monai-weekly-1.2.dev2317/tests/test_label_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_label_filterd.py` & `monai-weekly-1.2.dev2317/tests/test_label_filterd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_label_quality_score.py` & `monai-weekly-1.2.dev2317/tests/test_label_quality_score.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_label_to_contour.py` & `monai-weekly-1.2.dev2317/tests/test_label_to_contour.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_label_to_contourd.py` & `monai-weekly-1.2.dev2317/tests/test_label_to_contourd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_label_to_mask.py` & `monai-weekly-1.2.dev2317/tests/test_label_to_mask.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_label_to_maskd.py` & `monai-weekly-1.2.dev2317/tests/test_label_to_maskd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_lambda.py` & `monai-weekly-1.2.dev2317/tests/test_lambda.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,16 +9,20 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 import unittest
 
+from numpy import ndarray
+from torch import Tensor
+
 from monai.data.meta_tensor import MetaTensor
 from monai.transforms.utility.array import Lambda
+from monai.utils.type_conversion import convert_to_numpy, convert_to_tensor
 from tests.utils import TEST_NDARRAYS, NumpyImageTestCase2D, assert_allclose
 
 
 class TestLambda(NumpyImageTestCase2D):
     def test_lambda_identity(self):
         for p in TEST_NDARRAYS:
             img = p(self.imt)
@@ -40,10 +44,28 @@
             out = lambd(img)
             assert_allclose(slice_func(img), out, type_test=False)
             self.assertIsInstance(out, MetaTensor)
             self.assertEqual(len(out.applied_operations), 1)
             out = lambd.inverse(out)
             self.assertEqual(len(out.applied_operations), 0)
 
+    def test_lambda_track_meta_false(self):
+        for p in TEST_NDARRAYS:
+            img = p(self.imt)
+
+            def to_numpy(x):
+                return convert_to_numpy(x)
+
+            lambd = Lambda(func=to_numpy, track_meta=False)
+            out = lambd(img)
+            self.assertIsInstance(out, ndarray)
+
+            def to_tensor(x):
+                return convert_to_tensor(x)
+
+            lambd = Lambda(func=to_tensor, track_meta=False)
+            out = lambd(img)
+            self.assertIsInstance(out, Tensor)
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai-weekly-1.2.dev2316/tests/test_lambdad.py` & `monai-weekly-1.2.dev2317/tests/test_lambdad.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,16 +9,20 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 import unittest
 
+from numpy import ndarray
+from torch import Tensor
+
 from monai.data.meta_tensor import MetaTensor
 from monai.transforms.utility.dictionary import Lambdad
+from monai.utils.type_conversion import convert_to_numpy, convert_to_tensor
 from tests.utils import TEST_NDARRAYS, NumpyImageTestCase2D, assert_allclose
 
 
 class TestLambdad(NumpyImageTestCase2D):
     def test_lambdad_identity(self):
         for p in TEST_NDARRAYS:
             img = p(self.imt)
@@ -49,10 +53,31 @@
             assert_allclose(expected, out_img, type_test=False)
             self.assertIsInstance(out_img, MetaTensor)
             self.assertEqual(len(out_img.applied_operations), 1)
             inv_img = lambd.inverse(out)["img"]
             self.assertIsInstance(inv_img, MetaTensor)
             self.assertEqual(len(inv_img.applied_operations), 0)
 
+    def test_lambdad_track_meta_false(self):
+        for p in TEST_NDARRAYS:
+            img = p(self.imt)
+            data = {"img": img}
+
+            def to_numpy(x):
+                return convert_to_numpy(x)
+
+            lambd = Lambdad(keys=data.keys(), func=to_numpy, track_meta=False)
+            out = lambd(data)
+            out_img = out["img"]
+            self.assertIsInstance(out_img, ndarray)
+
+            def to_tensor(x):
+                return convert_to_tensor(x)
+
+            lambd = Lambdad(keys=data.keys(), func=to_tensor, track_meta=False)
+            out = lambd(data)
+            out_img = out["img"]
+            self.assertIsInstance(out_img, Tensor)
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai-weekly-1.2.dev2316/tests/test_lesion_froc.py` & `monai-weekly-1.2.dev2317/tests/test_lesion_froc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_list_data_collate.py` & `monai-weekly-1.2.dev2317/tests/test_list_data_collate.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_list_to_dict.py` & `monai-weekly-1.2.dev2317/tests/test_list_to_dict.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_lltm.py` & `monai-weekly-1.2.dev2317/tests/test_lltm.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_lmdbdataset.py` & `monai-weekly-1.2.dev2317/tests/test_lmdbdataset.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,25 +8,24 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 import os
-import shutil
 import tempfile
 import unittest
 
 import nibabel as nib
 import numpy as np
 from parameterized import parameterized
 
 from monai.data import LMDBDataset, json_hashing
 from monai.transforms import Compose, LoadImaged, SimulateDelayd, Transform
-from tests.utils import DistCall, DistTestCase, skip_if_windows
+from tests.utils import skip_if_windows
 
 TEST_CASE_1 = [
     Compose(
         [
             LoadImaged(keys=["image", "label", "extra"]),
             SimulateDelayd(keys=["image", "label", "extra"], delay_time=[1e-7, 1e-6, 1e-5]),
         ]
@@ -200,48 +199,9 @@
                 self.assertEqual(dataset_postcached[0]["label"], os.path.join(tempdir, "test_label1_new.nii.gz"))
                 self.assertEqual(dataset_postcached[1]["extra"], os.path.join(tempdir, "test_extra2_new.nii.gz"))
             else:
                 with self.assertRaises(RuntimeError):
                     dataset_postcached.set_data(data=test_data_new)  # filename list updated, files do not exist
 
 
-@skip_if_windows
-class TestMPLMDBDataset(DistTestCase):
-    def setUp(self):
-        self.tempdir = tempfile.mkdtemp()
-
-    def tearDown(self):
-        shutil.rmtree(self.tempdir)
-
-    @DistCall(nnodes=1, nproc_per_node=1)
-    def test_mp_cache(self):
-        items = [[list(range(i))] for i in range(5)]
-
-        ds = LMDBDataset(items, transform=_InplaceXform(), cache_dir=self.tempdir, lmdb_kwargs={"map_size": 10 * 1024})
-        self.assertEqual(items, [[[]], [[0]], [[0, 1]], [[0, 1, 2]], [[0, 1, 2, 3]]])
-        ds1 = LMDBDataset(items, transform=_InplaceXform(), cache_dir=self.tempdir, lmdb_kwargs={"map_size": 10 * 1024})
-        self.assertEqual(list(ds1), list(ds))
-        self.assertEqual(items, [[[]], [[0]], [[0, 1]], [[0, 1, 2]], [[0, 1, 2, 3]]])
-
-        ds = LMDBDataset(
-            items,
-            transform=_InplaceXform(),
-            cache_dir=self.tempdir,
-            lmdb_kwargs={"map_size": 10 * 1024},
-            hash_func=json_hashing,
-        )
-        self.assertEqual(items, [[[]], [[0]], [[0, 1]], [[0, 1, 2]], [[0, 1, 2, 3]]])
-        ds1 = LMDBDataset(
-            items,
-            transform=_InplaceXform(),
-            cache_dir=self.tempdir,
-            lmdb_kwargs={"map_size": 10 * 1024},
-            hash_func=json_hashing,
-        )
-        self.assertEqual(list(ds1), list(ds))
-        self.assertEqual(items, [[[]], [[0]], [[0, 1]], [[0, 1, 2]], [[0, 1, 2, 3]]])
-
-        self.assertTrue(isinstance(ds1.info(), dict))
-
-
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai-weekly-1.2.dev2316/tests/test_lmdbdataset_dist.py` & `monai-weekly-1.2.dev2317/tests/test_lmdbdataset_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_load_decathlon_datalist.py` & `monai-weekly-1.2.dev2317/tests/test_load_decathlon_datalist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_load_image.py` & `monai-weekly-1.2.dev2317/tests/test_load_image.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_load_imaged.py` & `monai-weekly-1.2.dev2317/tests/test_load_imaged.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_load_spacing_orientation.py` & `monai-weekly-1.2.dev2317/tests/test_load_spacing_orientation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_loader_semaphore.py` & `monai-weekly-1.2.dev2317/tests/test_loader_semaphore.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_local_normalized_cross_correlation_loss.py` & `monai-weekly-1.2.dev2317/tests/test_local_normalized_cross_correlation_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_localnet.py` & `monai-weekly-1.2.dev2317/tests/test_localnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_localnet_block.py` & `monai-weekly-1.2.dev2317/tests/test_localnet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_look_up_option.py` & `monai-weekly-1.2.dev2317/tests/test_look_up_option.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_loss_metric.py` & `monai-weekly-1.2.dev2317/tests/test_loss_metric.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_lr_finder.py` & `monai-weekly-1.2.dev2317/tests/test_lr_finder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_lr_scheduler.py` & `monai-weekly-1.2.dev2317/tests/test_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_make_nifti.py` & `monai-weekly-1.2.dev2317/tests/test_make_nifti.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_map_binary_to_indices.py` & `monai-weekly-1.2.dev2317/tests/test_map_binary_to_indices.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_map_classes_to_indices.py` & `monai-weekly-1.2.dev2317/tests/test_map_classes_to_indices.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_map_label_value.py` & `monai-weekly-1.2.dev2317/tests/test_map_label_value.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_map_label_valued.py` & `monai-weekly-1.2.dev2317/tests/test_map_label_valued.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_map_transform.py` & `monai-weekly-1.2.dev2317/tests/test_map_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_mask_intensity.py` & `monai-weekly-1.2.dev2317/tests/test_mask_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_mask_intensityd.py` & `monai-weekly-1.2.dev2317/tests/test_mask_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_masked_dice_loss.py` & `monai-weekly-1.2.dev2317/tests/test_masked_dice_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_masked_loss.py` & `monai-weekly-1.2.dev2317/tests/test_masked_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_masked_patch_wsi_dataset.py` & `monai-weekly-1.2.dev2317/tests/test_masked_patch_wsi_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_matshow3d.py` & `monai-weekly-1.2.dev2317/tests/test_matshow3d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_mean_ensemble.py` & `monai-weekly-1.2.dev2317/tests/test_mean_ensemble.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_mean_ensembled.py` & `monai-weekly-1.2.dev2317/tests/test_mean_ensembled.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_median_filter.py` & `monai-weekly-1.2.dev2317/tests/test_median_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_median_smooth.py` & `monai-weekly-1.2.dev2317/tests/test_median_smooth.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_median_smoothd.py` & `monai-weekly-1.2.dev2317/tests/test_median_smoothd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_mednistdataset.py` & `monai-weekly-1.2.dev2317/tests/test_mednistdataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_meta_affine.py` & `monai-weekly-1.2.dev2317/tests/test_meta_affine.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_meta_tensor.py` & `monai-weekly-1.2.dev2317/tests/test_meta_tensor.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_metatensor_integration.py` & `monai-weekly-1.2.dev2317/tests/test_metatensor_integration.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_metrics_reloaded.py` & `monai-weekly-1.2.dev2317/tests/test_metrics_reloaded.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_milmodel.py` & `monai-weekly-1.2.dev2317/tests/test_milmodel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_mlp.py` & `monai-weekly-1.2.dev2317/tests/test_mlp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_mmar_download.py` & `monai-weekly-1.2.dev2317/tests/test_mmar_download.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_module_list.py` & `monai-weekly-1.2.dev2317/tests/test_module_list.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_monai_env_vars.py` & `monai-weekly-1.2.dev2317/tests/test_monai_env_vars.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_monai_utils_misc.py` & `monai-weekly-1.2.dev2317/tests/test_monai_utils_misc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_mri_utils.py` & `monai-weekly-1.2.dev2317/tests/test_mri_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_multi_scale.py` & `monai-weekly-1.2.dev2317/tests/test_multi_scale.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_net_adapter.py` & `monai-weekly-1.2.dev2317/tests/test_net_adapter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_network_consistency.py` & `monai-weekly-1.2.dev2317/tests/test_network_consistency.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_nifti_endianness.py` & `monai-weekly-1.2.dev2317/tests/test_nifti_endianness.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_nifti_header_revise.py` & `monai-weekly-1.2.dev2317/tests/test_nifti_header_revise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_nifti_rw.py` & `monai-weekly-1.2.dev2317/tests/test_nifti_rw.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_normalize_intensity.py` & `monai-weekly-1.2.dev2317/tests/test_normalize_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_normalize_intensityd.py` & `monai-weekly-1.2.dev2317/tests/test_normalize_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_npzdictitemdataset.py` & `monai-weekly-1.2.dev2317/tests/test_npzdictitemdataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_nrrd_reader.py` & `monai-weekly-1.2.dev2317/tests/test_nrrd_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_nuclick_transforms.py` & `monai-weekly-1.2.dev2317/tests/test_nuclick_transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_numpy_reader.py` & `monai-weekly-1.2.dev2317/tests/test_numpy_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_nvtx_decorator.py` & `monai-weekly-1.2.dev2317/tests/test_nvtx_decorator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_nvtx_transform.py` & `monai-weekly-1.2.dev2317/tests/test_nvtx_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_occlusion_sensitivity.py` & `monai-weekly-1.2.dev2317/tests/test_occlusion_sensitivity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_one_of.py` & `monai-weekly-1.2.dev2317/tests/test_one_of.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_optim_novograd.py` & `monai-weekly-1.2.dev2317/tests/test_optim_novograd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_optional_import.py` & `monai-weekly-1.2.dev2317/tests/test_optional_import.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_ori_ras_lps.py` & `monai-weekly-1.2.dev2317/tests/test_ori_ras_lps.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_orientation.py` & `monai-weekly-1.2.dev2317/tests/test_orientation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_orientationd.py` & `monai-weekly-1.2.dev2317/tests/test_orientationd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_p3d_block.py` & `monai-weekly-1.2.dev2317/tests/test_p3d_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_pad_collation.py` & `monai-weekly-1.2.dev2317/tests/test_pad_collation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_pad_mode.py` & `monai-weekly-1.2.dev2317/tests/test_pad_mode.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_parallel_execution.py` & `monai-weekly-1.2.dev2317/tests/test_parallel_execution.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_parallel_execution_dist.py` & `monai-weekly-1.2.dev2317/tests/test_parallel_execution_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_partition_dataset.py` & `monai-weekly-1.2.dev2317/tests/test_partition_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_partition_dataset_classes.py` & `monai-weekly-1.2.dev2317/tests/test_partition_dataset_classes.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_patch_dataset.py` & `monai-weekly-1.2.dev2317/tests/test_patch_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_patch_inferer.py` & `monai-weekly-1.2.dev2317/tests/test_patch_inferer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_patch_wsi_dataset.py` & `monai-weekly-1.2.dev2317/tests/test_patch_wsi_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_patchembedding.py` & `monai-weekly-1.2.dev2317/tests/test_patchembedding.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_pathology_he_stain.py` & `monai-weekly-1.2.dev2317/tests/test_pathology_he_stain.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_pathology_he_stain_dict.py` & `monai-weekly-1.2.dev2317/tests/test_pathology_he_stain_dict.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_pathology_prob_nms.py` & `monai-weekly-1.2.dev2317/tests/test_pathology_prob_nms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_persistentdataset.py` & `monai-weekly-1.2.dev2317/tests/test_persistentdataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_persistentdataset_dist.py` & `monai-weekly-1.2.dev2317/tests/test_persistentdataset_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_phl_cpu.py` & `monai-weekly-1.2.dev2317/tests/test_phl_cpu.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_phl_cuda.py` & `monai-weekly-1.2.dev2317/tests/test_phl_cuda.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_pil_reader.py` & `monai-weekly-1.2.dev2317/tests/test_pil_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_plot_2d_or_3d_image.py` & `monai-weekly-1.2.dev2317/tests/test_plot_2d_or_3d_image.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_png_rw.py` & `monai-weekly-1.2.dev2317/tests/test_png_rw.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_polyval.py` & `monai-weekly-1.2.dev2317/tests/test_polyval.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_prepare_batch_default.py` & `monai-weekly-1.2.dev2317/tests/test_prepare_batch_default.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_prepare_batch_default_dist.py` & `monai-weekly-1.2.dev2317/tests/test_prepare_batch_default_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_prepare_batch_extra_input.py` & `monai-weekly-1.2.dev2317/tests/test_prepare_batch_extra_input.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_prepare_batch_hovernet.py` & `monai-weekly-1.2.dev2317/tests/test_prepare_batch_hovernet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_preset_filters.py` & `monai-weekly-1.2.dev2317/tests/test_preset_filters.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_print_info.py` & `monai-weekly-1.2.dev2317/tests/test_print_info.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_print_transform_backends.py` & `monai-weekly-1.2.dev2317/tests/test_print_transform_backends.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_probnms.py` & `monai-weekly-1.2.dev2317/tests/test_probnms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_probnmsd.py` & `monai-weekly-1.2.dev2317/tests/test_probnmsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_profiling.py` & `monai-weekly-1.2.dev2317/tests/test_profiling.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_pytorch_version_after.py` & `monai-weekly-1.2.dev2317/tests/test_pytorch_version_after.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_query_memory.py` & `monai-weekly-1.2.dev2317/tests/test_query_memory.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_adjust_contrast.py` & `monai-weekly-1.2.dev2317/tests/test_rand_adjust_contrast.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_adjust_contrastd.py` & `monai-weekly-1.2.dev2317/tests/test_rand_adjust_contrastd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_affine.py` & `monai-weekly-1.2.dev2317/tests/test_rand_affine.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_affine_grid.py` & `monai-weekly-1.2.dev2317/tests/test_rand_affine_grid.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_affined.py` & `monai-weekly-1.2.dev2317/tests/test_rand_affined.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_axis_flip.py` & `monai-weekly-1.2.dev2317/tests/test_rand_axis_flip.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_axis_flipd.py` & `monai-weekly-1.2.dev2317/tests/test_rand_axis_flipd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_bias_field.py` & `monai-weekly-1.2.dev2317/tests/test_rand_bias_field.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_bias_fieldd.py` & `monai-weekly-1.2.dev2317/tests/test_rand_bias_fieldd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_coarse_dropout.py` & `monai-weekly-1.2.dev2317/tests/test_rand_coarse_dropout.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_coarse_dropoutd.py` & `monai-weekly-1.2.dev2317/tests/test_rand_coarse_dropoutd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_coarse_shuffle.py` & `monai-weekly-1.2.dev2317/tests/test_rand_coarse_shuffle.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_coarse_shuffled.py` & `monai-weekly-1.2.dev2317/tests/test_rand_coarse_shuffled.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_crop_by_label_classes.py` & `monai-weekly-1.2.dev2317/tests/test_rand_crop_by_label_classes.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_crop_by_label_classesd.py` & `monai-weekly-1.2.dev2317/tests/test_rand_crop_by_label_classesd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_crop_by_pos_neg_label.py` & `monai-weekly-1.2.dev2317/tests/test_rand_crop_by_pos_neg_label.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_crop_by_pos_neg_labeld.py` & `monai-weekly-1.2.dev2317/tests/test_rand_crop_by_pos_neg_labeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_cucim_dict_transform.py` & `monai-weekly-1.2.dev2317/tests/test_rand_cucim_dict_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_cucim_transform.py` & `monai-weekly-1.2.dev2317/tests/test_rand_cucim_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_deform_grid.py` & `monai-weekly-1.2.dev2317/tests/test_rand_deform_grid.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_elastic_2d.py` & `monai-weekly-1.2.dev2317/tests/test_rand_elastic_2d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_elastic_3d.py` & `monai-weekly-1.2.dev2317/tests/test_rand_elastic_3d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_elasticd_2d.py` & `monai-weekly-1.2.dev2317/tests/test_rand_elasticd_2d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_elasticd_3d.py` & `monai-weekly-1.2.dev2317/tests/test_rand_elasticd_3d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_flip.py` & `monai-weekly-1.2.dev2317/tests/test_rand_flip.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_flipd.py` & `monai-weekly-1.2.dev2317/tests/test_rand_flipd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_gaussian_noise.py` & `monai-weekly-1.2.dev2317/tests/test_rand_gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_gaussian_noised.py` & `monai-weekly-1.2.dev2317/tests/test_rand_rician_noised.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,38 +13,40 @@
 
 import unittest
 
 import numpy as np
 import torch
 from parameterized import parameterized
 
-from monai.transforms import RandGaussianNoised
+from monai.transforms import RandRicianNoised
 from tests.utils import TEST_NDARRAYS, NumpyImageTestCase2D
 
 TESTS = []
 for p in TEST_NDARRAYS:
     TESTS.append(["test_zero_mean", p, ["img1", "img2"], 0, 0.1])
     TESTS.append(["test_non_zero_mean", p, ["img1", "img2"], 1, 0.5])
 
 seed = 0
 
 
-class TestRandGaussianNoised(NumpyImageTestCase2D):
+class TestRandRicianNoisedNumpy(NumpyImageTestCase2D):
     @parameterized.expand(TESTS)
-    def test_correct_results(self, _, im_type, keys, mean, std):
-        gaussian_fn = RandGaussianNoised(keys=keys, prob=1.0, mean=mean, std=std, dtype=np.float64)
-        gaussian_fn.set_random_state(seed)
-        im = im_type(self.imt)
-        noised = gaussian_fn({k: im for k in keys})
+    def test_correct_results(self, _, in_type, keys, mean, std):
+        rician_fn = RandRicianNoised(keys=keys, prob=1.0, mean=mean, std=std, dtype=np.float64)
+        rician_fn.set_random_state(seed)
+        noised = rician_fn({k: in_type(self.imt) for k in keys})
         np.random.seed(seed)
-        # simulate the randomize() of transform
-        np.random.random()
-        noise = np.random.normal(mean, np.random.uniform(0, std), size=self.imt.shape)
         for k in keys:
-            expected = self.imt + noise
+            # simulate the `randomize` function of transform
+            np.random.random()
+            _std = np.random.uniform(0, std)
+            expected = np.sqrt(
+                (self.imt + np.random.normal(mean, _std, size=self.imt.shape)) ** 2
+                + np.random.normal(mean, _std, size=self.imt.shape) ** 2
+            )
             if isinstance(noised[k], torch.Tensor):
                 noised[k] = noised[k].cpu()
             np.testing.assert_allclose(expected, noised[k], atol=1e-5, rtol=1e-5)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_gaussian_sharpen.py` & `monai-weekly-1.2.dev2317/tests/test_rand_gaussian_sharpen.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_gaussian_sharpend.py` & `monai-weekly-1.2.dev2317/tests/test_rand_gaussian_sharpend.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_gaussian_smooth.py` & `monai-weekly-1.2.dev2317/tests/test_rand_gaussian_smooth.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_gaussian_smoothd.py` & `monai-weekly-1.2.dev2317/tests/test_rand_gaussian_smoothd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_gibbs_noise.py` & `monai-weekly-1.2.dev2317/tests/test_rand_gibbs_noise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_gibbs_noised.py` & `monai-weekly-1.2.dev2317/tests/test_rand_gibbs_noised.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_grid_distortion.py` & `monai-weekly-1.2.dev2317/tests/test_rand_grid_distortion.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_grid_distortiond.py` & `monai-weekly-1.2.dev2317/tests/test_rand_grid_distortiond.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_grid_patch.py` & `monai-weekly-1.2.dev2317/tests/test_rand_grid_patch.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_grid_patchd.py` & `monai-weekly-1.2.dev2317/tests/test_rand_grid_patchd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_histogram_shift.py` & `monai-weekly-1.2.dev2317/tests/test_rand_histogram_shift.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_histogram_shiftd.py` & `monai-weekly-1.2.dev2317/tests/test_rand_histogram_shiftd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_k_space_spike_noise.py` & `monai-weekly-1.2.dev2317/tests/test_rand_k_space_spike_noise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_k_space_spike_noised.py` & `monai-weekly-1.2.dev2317/tests/test_rand_k_space_spike_noised.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_lambda.py` & `monai-weekly-1.2.dev2317/tests/test_rand_lambda.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_lambdad.py` & `monai-weekly-1.2.dev2317/tests/test_rand_lambdad.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_rician_noise.py` & `monai-weekly-1.2.dev2317/tests/test_rand_rician_noise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_rician_noised.py` & `monai-weekly-1.2.dev2317/tests/test_reference_based_spatial_cropd.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,43 +10,48 @@
 # limitations under the License.
 
 from __future__ import annotations
 
 import unittest
 
 import numpy as np
-import torch
 from parameterized import parameterized
 
-from monai.transforms import RandRicianNoised
-from tests.utils import TEST_NDARRAYS, NumpyImageTestCase2D
+from monai.apps.reconstruction.transforms.dictionary import ReferenceBasedSpatialCropd
+from tests.utils import TEST_NDARRAYS
+
+# see test_spatial_cropd for typical tests (like roi_start,
+# roi_slices, etc.)
+# here, we test TargetBasedSpatialCropd's functionality
+# which focuses on automatic input crop based on target image's shape.
 
 TESTS = []
 for p in TEST_NDARRAYS:
-    TESTS.append(["test_zero_mean", p, ["img1", "img2"], 0, 0.1])
-    TESTS.append(["test_non_zero_mean", p, ["img1", "img2"], 1, 0.5])
-
-seed = 0
+    # 2D
+    TESTS.append(
+        [
+            {"keys": ["kspace_masked_ifft"], "ref_key": "target"},
+            {"kspace_masked_ifft": p(np.ones([10, 20, 20])), "target": p(np.ones([5, 8, 8]))},
+            (8, 8),  # expected shape
+        ]
+    )
+
+    # 3D
+    TESTS.append(
+        [
+            {"keys": ["kspace_masked_ifft"], "ref_key": "target"},
+            {"kspace_masked_ifft": p(np.ones([10, 20, 20, 16])), "target": p(np.ones([5, 8, 8, 6]))},
+            (8, 8, 6),  # expected shape
+        ]
+    )
 
 
-class TestRandRicianNoisedNumpy(NumpyImageTestCase2D):
+class TestTargetBasedSpatialCropd(unittest.TestCase):
     @parameterized.expand(TESTS)
-    def test_correct_results(self, _, in_type, keys, mean, std):
-        rician_fn = RandRicianNoised(keys=keys, prob=1.0, mean=mean, std=std, dtype=np.float64)
-        rician_fn.set_random_state(seed)
-        noised = rician_fn({k: in_type(self.imt) for k in keys})
-        np.random.seed(seed)
-        for k in keys:
-            # simulate the `randomize` function of transform
-            np.random.random()
-            _std = np.random.uniform(0, std)
-            expected = np.sqrt(
-                (self.imt + np.random.normal(mean, _std, size=self.imt.shape)) ** 2
-                + np.random.normal(mean, _std, size=self.imt.shape) ** 2
-            )
-            if isinstance(noised[k], torch.Tensor):
-                noised[k] = noised[k].cpu()
-            np.testing.assert_allclose(expected, noised[k], atol=1e-5, rtol=1e-5)
+    def test_shape(self, args, data, expected_shape):
+        cropper = ReferenceBasedSpatialCropd(keys=args["keys"], ref_key=args["ref_key"])
+        res_data = cropper(data)
+        self.assertTupleEqual(res_data[args["keys"][0]].shape[1:], expected_shape)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_rotate.py` & `monai-weekly-1.2.dev2317/tests/test_rand_rotate.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_rotate90.py` & `monai-weekly-1.2.dev2317/tests/test_rand_rotate90.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_rotate90d.py` & `monai-weekly-1.2.dev2317/tests/test_rand_rotate90d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_rotated.py` & `monai-weekly-1.2.dev2317/tests/test_rand_rotated.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_scale_crop.py` & `monai-weekly-1.2.dev2317/tests/test_rand_scale_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_scale_cropd.py` & `monai-weekly-1.2.dev2317/tests/test_rand_scale_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_scale_intensity.py` & `monai-weekly-1.2.dev2317/tests/test_rand_scale_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_scale_intensityd.py` & `monai-weekly-1.2.dev2317/tests/test_rand_scale_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_shift_intensity.py` & `monai-weekly-1.2.dev2317/tests/test_rand_shift_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_shift_intensityd.py` & `monai-weekly-1.2.dev2317/tests/test_rand_shift_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_spatial_crop.py` & `monai-weekly-1.2.dev2317/tests/test_rand_spatial_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_spatial_crop_samples.py` & `monai-weekly-1.2.dev2317/tests/test_rand_spatial_crop_samples.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_spatial_crop_samplesd.py` & `monai-weekly-1.2.dev2317/tests/test_rand_spatial_crop_samplesd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_spatial_cropd.py` & `monai-weekly-1.2.dev2317/tests/test_rand_spatial_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_std_shift_intensity.py` & `monai-weekly-1.2.dev2317/tests/test_rand_std_shift_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_std_shift_intensityd.py` & `monai-weekly-1.2.dev2317/tests/test_rand_std_shift_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_weighted_crop.py` & `monai-weekly-1.2.dev2317/tests/test_rand_weighted_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_weighted_cropd.py` & `monai-weekly-1.2.dev2317/tests/test_rand_weighted_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_zoom.py` & `monai-weekly-1.2.dev2317/tests/test_rand_zoom.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rand_zoomd.py` & `monai-weekly-1.2.dev2317/tests/test_rand_zoomd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_randidentity.py` & `monai-weekly-1.2.dev2317/tests/test_randidentity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_random_order.py` & `monai-weekly-1.2.dev2317/tests/test_random_order.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_randomizable.py` & `monai-weekly-1.2.dev2317/tests/test_randomizable.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_randomizable_transform_type.py` & `monai-weekly-1.2.dev2317/tests/test_randomizable_transform_type.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_randtorchvisiond.py` & `monai-weekly-1.2.dev2317/tests/test_randtorchvisiond.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rankfilter_dist.py` & `monai-weekly-1.2.dev2317/tests/test_rankfilter_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_recon_net_utils.py` & `monai-weekly-1.2.dev2317/tests/test_recon_net_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_reference_based_normalize_intensity.py` & `monai-weekly-1.2.dev2317/tests/test_reference_based_normalize_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_reference_resolver.py` & `monai-weekly-1.2.dev2317/tests/test_reference_resolver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_reg_loss_integration.py` & `monai-weekly-1.2.dev2317/tests/test_reg_loss_integration.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_regunet.py` & `monai-weekly-1.2.dev2317/tests/test_regunet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_regunet_block.py` & `monai-weekly-1.2.dev2317/tests/test_regunet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_remove_repeated_channel.py` & `monai-weekly-1.2.dev2317/tests/test_remove_repeated_channel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_remove_repeated_channeld.py` & `monai-weekly-1.2.dev2317/tests/test_remove_repeated_channeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_remove_small_objects.py` & `monai-weekly-1.2.dev2317/tests/test_remove_small_objects.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_repeat_channel.py` & `monai-weekly-1.2.dev2317/tests/test_repeat_channel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_repeat_channeld.py` & `monai-weekly-1.2.dev2317/tests/test_repeat_channeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_replace_module.py` & `monai-weekly-1.2.dev2317/tests/test_replace_module.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_require_pkg.py` & `monai-weekly-1.2.dev2317/tests/test_require_pkg.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_resample.py` & `monai-weekly-1.2.dev2317/tests/test_resample.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_resample_backends.py` & `monai-weekly-1.2.dev2317/tests/test_resample_backends.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_resample_datalist.py` & `monai-weekly-1.2.dev2317/tests/test_resample_datalist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_resample_to_match.py` & `monai-weekly-1.2.dev2317/tests/test_resample_to_match.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,30 +68,29 @@
     def test_correct(self, reader, writer):
         loader = Compose([LoadImaged(("im1", "im2"), reader=reader), EnsureChannelFirstd(("im1", "im2"))])
         data = loader({"im1": self.fnames[0], "im2": self.fnames[1]})
         tr = ResampleToMatch()
         im_mod = tr(data["im2"], data["im1"])
 
         # check lazy resample
-        tr_lazy = ResampleToMatch()
         call_param = {"img": data["im2"], "img_dst": data["im1"]}
-        test_resampler_lazy(tr_lazy, im_mod, init_param={}, call_param=call_param)
+        test_resampler_lazy(tr, im_mod, init_param={}, call_param=call_param)
 
         saver = SaveImaged(
             "im3", output_dir=self.tmpdir, output_postfix="", separate_folder=False, writer=writer, resample=False
         )
         im_mod.meta["filename_or_obj"] = get_rand_fname()
         saver({"im3": im_mod})
 
         saved = nib.load(os.path.join(self.tmpdir, im_mod.meta["filename_or_obj"]))
         assert_allclose(data["im1"].shape[1:], saved.shape)
         assert_allclose(saved.header["dim"][:4], np.array([3, 384, 384, 19]))
 
     def test_inverse(self):
-        loader = Compose([LoadImaged(("im1", "im2")), EnsureChannelFirstd(("im1", "im2"))])
+        loader = Compose([LoadImaged(("im1", "im2"), image_only=True), EnsureChannelFirstd(("im1", "im2"))])
         data = loader({"im1": self.fnames[0], "im2": self.fnames[1]})
         tr = ResampleToMatch()
         im_mod = tr(data["im2"], data["im1"])
         self.assertNotEqual(im_mod.shape, data["im2"].shape)
         self.assertGreater(((im_mod.affine - data["im2"].affine) ** 2).sum() ** 0.5, 1e-2)
         # inverse
         im_mod2 = tr.inverse(im_mod)
```

### Comparing `monai-weekly-1.2.dev2316/tests/test_resample_to_matchd.py` & `monai-weekly-1.2.dev2317/tests/test_resample_to_matchd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_resampler.py` & `monai-weekly-1.2.dev2317/tests/test_resampler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_resize.py` & `monai-weekly-1.2.dev2317/tests/test_resize.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_resize_with_pad_or_crop.py` & `monai-weekly-1.2.dev2317/tests/test_resize_with_pad_or_crop.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,11 +89,13 @@
                 pending_result,
                 mode="nearest",
                 padding_mode=TESTS_PENDING_MODE[input_param["mode"]],
                 align_corners=align_corners,
             )[0]
             # compare
             assert_allclose(result, expected, rtol=1e-5)
+            inverted = padcropper.inverse(result)
+            self.assertEqual(inverted.shape, image.shape)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai-weekly-1.2.dev2316/tests/test_resize_with_pad_or_cropd.py` & `monai-weekly-1.2.dev2317/tests/test_resize_with_pad_or_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_resized.py` & `monai-weekly-1.2.dev2317/tests/test_resized.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_resnet.py` & `monai-weekly-1.2.dev2317/tests/test_resnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_retinanet.py` & `monai-weekly-1.2.dev2317/tests/test_retinanet.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,32 +179,32 @@
         except BaseException:
             idx = 0
         idx %= 3
         # test whether support torchscript
         data = torch.randn(input_shape)
         backbone = model(**input_param)
         if idx == 0:
-            test_onnx_save(backbone, data, rtol=1e-3, atol=0.1)
+            test_onnx_save(backbone, data, rtol=2e-3)
             return
         feature_extractor = resnet_fpn_feature_extractor(
             backbone=backbone,
             spatial_dims=input_param["spatial_dims"],
             pretrained_backbone=input_param["pretrained"],
             trainable_backbone_layers=None,
             returned_layers=[1, 2],
         )
         if idx == 1:
-            test_onnx_save(feature_extractor, data, rtol=1e-3)
+            test_onnx_save(feature_extractor, data, rtol=2e-3)
             return
         net = RetinaNet(
             spatial_dims=input_param["spatial_dims"],
             num_classes=input_param["num_classes"],
             num_anchors=num_anchors,
             feature_extractor=feature_extractor,
             size_divisible=32,
         )
         if idx == 2:
-            test_onnx_save(net, data, rtol=1e-3)
+            test_onnx_save(net, data, rtol=2e-3)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai-weekly-1.2.dev2316/tests/test_retinanet_detector.py` & `monai-weekly-1.2.dev2317/tests/test_retinanet_detector.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_retinanet_predict_utils.py` & `monai-weekly-1.2.dev2317/tests/test_retinanet_predict_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rotate.py` & `monai-weekly-1.2.dev2317/tests/test_rotate.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rotate90.py` & `monai-weekly-1.2.dev2317/tests/test_rotate90.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rotate90d.py` & `monai-weekly-1.2.dev2317/tests/test_rotate90d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_rotated.py` & `monai-weekly-1.2.dev2317/tests/test_rotated.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_safe_dtype_range.py` & `monai-weekly-1.2.dev2317/tests/test_safe_dtype_range.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_saliency_inferer.py` & `monai-weekly-1.2.dev2317/tests/test_saliency_inferer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_sample_slices.py` & `monai-weekly-1.2.dev2317/tests/test_sample_slices.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_sampler_dist.py` & `monai-weekly-1.2.dev2317/tests/test_sampler_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_save_classificationd.py` & `monai-weekly-1.2.dev2317/tests/test_save_classificationd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_save_image.py` & `monai-weekly-1.2.dev2317/tests/test_save_image.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_save_imaged.py` & `monai-weekly-1.2.dev2317/tests/test_save_imaged.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_save_state.py` & `monai-weekly-1.2.dev2317/tests/test_save_state.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_savitzky_golay_filter.py` & `monai-weekly-1.2.dev2317/tests/test_savitzky_golay_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_savitzky_golay_smooth.py` & `monai-weekly-1.2.dev2317/tests/test_savitzky_golay_smooth.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_savitzky_golay_smoothd.py` & `monai-weekly-1.2.dev2317/tests/test_savitzky_golay_smoothd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_scale_intensity.py` & `monai-weekly-1.2.dev2317/tests/test_scale_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_scale_intensity_range.py` & `monai-weekly-1.2.dev2317/tests/test_scale_intensity_range.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_scale_intensity_range_percentiles.py` & `monai-weekly-1.2.dev2317/tests/test_scale_intensity_range_percentiles.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_scale_intensity_range_percentilesd.py` & `monai-weekly-1.2.dev2317/tests/test_scale_intensity_range_percentilesd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_scale_intensity_ranged.py` & `monai-weekly-1.2.dev2317/tests/test_scale_intensity_ranged.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_scale_intensityd.py` & `monai-weekly-1.2.dev2317/tests/test_scale_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_se_block.py` & `monai-weekly-1.2.dev2317/tests/test_se_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_se_blocks.py` & `monai-weekly-1.2.dev2317/tests/test_se_blocks.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_seg_loss_integration.py` & `monai-weekly-1.2.dev2317/tests/test_seg_loss_integration.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_segresnet.py` & `monai-weekly-1.2.dev2317/tests/test_segresnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_segresnet_block.py` & `monai-weekly-1.2.dev2317/tests/test_segresnet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_segresnet_ds.py` & `monai-weekly-1.2.dev2317/tests/test_segresnet_ds.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_select_cross_validation_folds.py` & `monai-weekly-1.2.dev2317/tests/test_select_cross_validation_folds.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_select_itemsd.py` & `monai-weekly-1.2.dev2317/tests/test_select_itemsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_selfattention.py` & `monai-weekly-1.2.dev2317/tests/test_selfattention.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_senet.py` & `monai-weekly-1.2.dev2317/tests/test_senet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_separable_filter.py` & `monai-weekly-1.2.dev2317/tests/test_separable_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_set_determinism.py` & `monai-weekly-1.2.dev2317/tests/test_set_determinism.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_set_visible_devices.py` & `monai-weekly-1.2.dev2317/tests/test_set_visible_devices.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_shift_intensity.py` & `monai-weekly-1.2.dev2317/tests/test_shift_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_shift_intensityd.py` & `monai-weekly-1.2.dev2317/tests/test_shift_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_shuffle_buffer.py` & `monai-weekly-1.2.dev2317/tests/test_shuffle_buffer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_signal_continuouswavelet.py` & `monai-weekly-1.2.dev2317/tests/test_signal_continuouswavelet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_signal_fillempty.py` & `monai-weekly-1.2.dev2317/tests/test_signal_fillempty.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_signal_rand_add_gaussiannoise.py` & `monai-weekly-1.2.dev2317/tests/test_signal_rand_add_gaussiannoise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_signal_rand_add_sine.py` & `monai-weekly-1.2.dev2317/tests/test_signal_rand_add_sine.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_signal_rand_add_sine_partial.py` & `monai-weekly-1.2.dev2317/tests/test_signal_rand_add_sine_partial.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_signal_rand_add_squarepulse.py` & `monai-weekly-1.2.dev2317/tests/test_signal_rand_add_squarepulse.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_signal_rand_add_squarepulse_partial.py` & `monai-weekly-1.2.dev2317/tests/test_signal_rand_add_squarepulse_partial.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_signal_rand_drop.py` & `monai-weekly-1.2.dev2317/tests/test_signal_rand_drop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_signal_rand_scale.py` & `monai-weekly-1.2.dev2317/tests/test_signal_rand_scale.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_signal_rand_shift.py` & `monai-weekly-1.2.dev2317/tests/test_signal_rand_shift.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_signal_remove_frequency.py` & `monai-weekly-1.2.dev2317/tests/test_signal_remove_frequency.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_simple_aspp.py` & `monai-weekly-1.2.dev2317/tests/test_simple_aspp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_simulatedelay.py` & `monai-weekly-1.2.dev2317/tests/test_simulatedelay.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_simulatedelayd.py` & `monai-weekly-1.2.dev2317/tests/test_simulatedelayd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_skip_connection.py` & `monai-weekly-1.2.dev2317/tests/test_skip_connection.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_slice_inferer.py` & `monai-weekly-1.2.dev2317/tests/test_slice_inferer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_sliding_patch_wsi_dataset.py` & `monai-weekly-1.2.dev2317/tests/test_sliding_patch_wsi_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_sliding_window_hovernet_inference.py` & `monai-weekly-1.2.dev2317/tests/test_sliding_window_hovernet_inference.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_sliding_window_inference.py` & `monai-weekly-1.2.dev2317/tests/test_sliding_window_inference.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_sliding_window_splitter.py` & `monai-weekly-1.2.dev2317/tests/test_sliding_window_splitter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_smartcachedataset.py` & `monai-weekly-1.2.dev2317/tests/test_smartcachedataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_smooth_field.py` & `monai-weekly-1.2.dev2317/tests/test_smooth_field.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_sobel_gradient.py` & `monai-weekly-1.2.dev2317/tests/test_sobel_gradient.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_sobel_gradientd.py` & `monai-weekly-1.2.dev2317/tests/test_sobel_gradientd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_some_of.py` & `monai-weekly-1.2.dev2317/tests/test_some_of.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_spacing.py` & `monai-weekly-1.2.dev2317/tests/test_spacing.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_spacingd.py` & `monai-weekly-1.2.dev2317/tests/test_spacingd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_spatial_combine_transforms.py` & `monai-weekly-1.2.dev2317/tests/test_spatial_combine_transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_spatial_crop.py` & `monai-weekly-1.2.dev2317/tests/test_spatial_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_spatial_cropd.py` & `monai-weekly-1.2.dev2317/tests/test_spatial_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_spatial_pad.py` & `monai-weekly-1.2.dev2317/tests/test_spatial_pad.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_spatial_padd.py` & `monai-weekly-1.2.dev2317/tests/test_spatial_padd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_spatial_resample.py` & `monai-weekly-1.2.dev2317/tests/test_spatial_resample.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_spatial_resampled.py` & `monai-weekly-1.2.dev2317/tests/test_spatial_resampled.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_split_channel.py` & `monai-weekly-1.2.dev2317/tests/test_split_channel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_split_channeld.py` & `monai-weekly-1.2.dev2317/tests/test_split_channeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_splitdim.py` & `monai-weekly-1.2.dev2317/tests/test_splitdim.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_splitdimd.py` & `monai-weekly-1.2.dev2317/tests/test_splitdimd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_squeezedim.py` & `monai-weekly-1.2.dev2317/tests/test_squeezedim.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_squeezedimd.py` & `monai-weekly-1.2.dev2317/tests/test_squeezedimd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_state_cacher.py` & `monai-weekly-1.2.dev2317/tests/test_state_cacher.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_std_shift_intensity.py` & `monai-weekly-1.2.dev2317/tests/test_std_shift_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_std_shift_intensityd.py` & `monai-weekly-1.2.dev2317/tests/test_std_shift_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_str2bool.py` & `monai-weekly-1.2.dev2317/tests/test_str2bool.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_str2list.py` & `monai-weekly-1.2.dev2317/tests/test_str2list.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_subpixel_upsample.py` & `monai-weekly-1.2.dev2317/tests/test_subpixel_upsample.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_surface_dice.py` & `monai-weekly-1.2.dev2317/tests/test_surface_dice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_surface_distance.py` & `monai-weekly-1.2.dev2317/tests/test_surface_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_swin_unetr.py` & `monai-weekly-1.2.dev2317/tests/test_swin_unetr.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_synthetic.py` & `monai-weekly-1.2.dev2317/tests/test_synthetic.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_tciadataset.py` & `monai-weekly-1.2.dev2317/tests/test_tciadataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_testtimeaugmentation.py` & `monai-weekly-1.2.dev2317/tests/test_testtimeaugmentation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_text_encoding.py` & `monai-weekly-1.2.dev2317/tests/test_text_encoding.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_thread_buffer.py` & `monai-weekly-1.2.dev2317/tests/test_thread_buffer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_threadcontainer.py` & `monai-weekly-1.2.dev2317/tests/test_threadcontainer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_threshold_intensity.py` & `monai-weekly-1.2.dev2317/tests/test_threshold_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_threshold_intensityd.py` & `monai-weekly-1.2.dev2317/tests/test_threshold_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_timedcall_dist.py` & `monai-weekly-1.2.dev2317/tests/test_timedcall_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_to_contiguous.py` & `monai-weekly-1.2.dev2317/tests/test_to_contiguous.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_to_cupy.py` & `monai-weekly-1.2.dev2317/tests/test_to_cupy.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_to_cupyd.py` & `monai-weekly-1.2.dev2317/tests/test_to_cupyd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_to_device.py` & `monai-weekly-1.2.dev2317/tests/test_to_device.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_to_deviced.py` & `monai-weekly-1.2.dev2317/tests/test_to_deviced.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_to_from_meta_tensord.py` & `monai-weekly-1.2.dev2317/tests/test_to_from_meta_tensord.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_to_numpy.py` & `monai-weekly-1.2.dev2317/tests/test_to_numpy.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_to_numpyd.py` & `monai-weekly-1.2.dev2317/tests/test_to_numpyd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_to_onehot.py` & `monai-weekly-1.2.dev2317/tests/test_to_onehot.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_to_pil.py` & `monai-weekly-1.2.dev2317/tests/test_to_pil.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_to_pild.py` & `monai-weekly-1.2.dev2317/tests/test_to_pild.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_to_tensor.py` & `monai-weekly-1.2.dev2317/tests/test_to_tensor.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_to_tensord.py` & `monai-weekly-1.2.dev2317/tests/test_to_tensord.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_torchscript_utils.py` & `monai-weekly-1.2.dev2317/tests/test_torchscript_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_torchvision.py` & `monai-weekly-1.2.dev2317/tests/test_torchvision.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_torchvision_fc_model.py` & `monai-weekly-1.2.dev2317/tests/test_torchvision_fc_model.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_torchvisiond.py` & `monai-weekly-1.2.dev2317/tests/test_torchvisiond.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_traceable_transform.py` & `monai-weekly-1.2.dev2317/tests/test_traceable_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_train_mode.py` & `monai-weekly-1.2.dev2317/tests/test_train_mode.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_trainable_bilateral.py` & `monai-weekly-1.2.dev2317/tests/test_trainable_bilateral.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_trainable_joint_bilateral.py` & `monai-weekly-1.2.dev2317/tests/test_trainable_joint_bilateral.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_transchex.py` & `monai-weekly-1.2.dev2317/tests/test_transchex.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_transform.py` & `monai-weekly-1.2.dev2317/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_transformerblock.py` & `monai-weekly-1.2.dev2317/tests/test_transformerblock.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_transpose.py` & `monai-weekly-1.2.dev2317/tests/test_transpose.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_transposed.py` & `monai-weekly-1.2.dev2317/tests/test_transposed.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_tversky_loss.py` & `monai-weekly-1.2.dev2317/tests/test_tversky_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_unet.py` & `monai-weekly-1.2.dev2317/tests/test_unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_unetr.py` & `monai-weekly-1.2.dev2317/tests/test_unetr.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_unetr_block.py` & `monai-weekly-1.2.dev2317/tests/test_unetr_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_unified_focal_loss.py` & `monai-weekly-1.2.dev2317/tests/test_unified_focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_upsample_block.py` & `monai-weekly-1.2.dev2317/tests/test_upsample_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_utils_pytorch_numpy_unification.py` & `monai-weekly-1.2.dev2317/tests/test_utils_pytorch_numpy_unification.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_varautoencoder.py` & `monai-weekly-1.2.dev2317/tests/test_varautoencoder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_varnet.py` & `monai-weekly-1.2.dev2317/tests/test_varnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_version_leq.py` & `monai-weekly-1.2.dev2317/tests/test_version_leq.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_video_datasets.py` & `monai-weekly-1.2.dev2317/tests/test_video_datasets.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_vis_cam.py` & `monai-weekly-1.2.dev2317/tests/test_vis_cam.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_vis_gradbased.py` & `monai-weekly-1.2.dev2317/tests/test_vis_gradbased.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_vis_gradcam.py` & `monai-weekly-1.2.dev2317/tests/test_vis_gradcam.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_vit.py` & `monai-weekly-1.2.dev2317/tests/test_vit.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_vitautoenc.py` & `monai-weekly-1.2.dev2317/tests/test_vitautoenc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_vnet.py` & `monai-weekly-1.2.dev2317/tests/test_vnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_vote_ensemble.py` & `monai-weekly-1.2.dev2317/tests/test_vote_ensemble.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_vote_ensembled.py` & `monai-weekly-1.2.dev2317/tests/test_vote_ensembled.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_warp.py` & `monai-weekly-1.2.dev2317/tests/test_warp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_watershed.py` & `monai-weekly-1.2.dev2317/tests/test_watershed.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_watershedd.py` & `monai-weekly-1.2.dev2317/tests/test_watershedd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_weight_init.py` & `monai-weekly-1.2.dev2317/tests/test_weight_init.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_weighted_random_sampler_dist.py` & `monai-weekly-1.2.dev2317/tests/test_weighted_random_sampler_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_with_allow_missing_keys.py` & `monai-weekly-1.2.dev2317/tests/test_with_allow_missing_keys.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_write_metrics_reports.py` & `monai-weekly-1.2.dev2317/tests/test_write_metrics_reports.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_wsireader.py` & `monai-weekly-1.2.dev2317/tests/test_wsireader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_zipdataset.py` & `monai-weekly-1.2.dev2317/tests/test_zipdataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_zoom.py` & `monai-weekly-1.2.dev2317/tests/test_zoom.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_zoom_affine.py` & `monai-weekly-1.2.dev2317/tests/test_zoom_affine.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/tests/test_zoomd.py` & `monai-weekly-1.2.dev2317/tests/test_zoomd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2316/versioneer.py` & `monai-weekly-1.2.dev2317/versioneer.py`

 * *Files identical despite different names*

