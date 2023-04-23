# Comparing `tmp/so_vits_svc_fork-3.9.4.tar.gz` & `tmp/so_vits_svc_fork-3.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "so_vits_svc_fork-3.9.4.tar", max compression
+gzip compressed data, was "so_vits_svc_fork-3.9.5.tar", max compression
```

## Comparing `so_vits_svc_fork-3.9.4.tar` & `so_vits_svc_fork-3.9.5.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0    12463 2023-04-18 09:42:39.840487 so_vits_svc_fork-3.9.4/LICENSE
--rw-r--r--   0        0        0    18160 2023-04-18 09:42:39.840487 so_vits_svc_fork-3.9.4/README.md
--rw-r--r--   0        0        0     3092 2023-04-18 09:42:40.864505 so_vits_svc_fork-3.9.4/pyproject.toml
--rw-r--r--   0        0        0       70 2023-04-18 09:42:40.816504 so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/__init__.py
--rw-r--r--   0        0        0    22740 2023-04-18 09:42:39.844487 so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/__main__.py
--rw-r--r--   0        0        0     1393 2023-04-18 09:42:39.844487 so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/cluster/__init__.py
--rw-r--r--   0        0        0     2844 2023-04-18 09:42:39.844487 so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/cluster/train_cluster.py
--rw-r--r--   0        0        0     2868 2023-04-18 09:42:39.844487 so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/dataset.py
--rw-r--r--   0        0        0     2454 2023-04-18 09:42:39.844487 so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/default_gui_presets.json
--rw-r--r--   0        0        0     7267 2023-04-18 09:42:39.844487 so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/f0.py
--rw-r--r--   0        0        0    25867 2023-04-18 09:42:39.844487 so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/gui.py
--rw-r--r--   0        0        0      864 2023-04-18 09:42:39.844487 so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/hparams.py
--rw-r--r--   0        0        0        0 2023-04-18 09:42:39.844487 so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/inference/__init__.py
--rw-r--r--   0        0        0    24054 2023-04-18 09:42:39.844487 so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/inference/core.py
--rw-r--r--   0        0        0     7485 2023-04-18 09:42:39.844487 so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/inference/main.py
--rw-r--r--   0        0        0     1341 2023-04-18 09:42:39.844487 so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/logger.py
--rw-r--r--   0        0        0        0 2023-04-18 09:42:39.844487 so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/modules/__init__.py
--rw-r--r--   0        0        0    16683 2023-04-18 09:42:39.844487 so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/modules/attentions.py
--rw-r--r--   0        0        0     4620 2023-04-18 09:42:39.844487 so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/modules/commons.py
--rw-r--r--   0        0        0        0 2023-04-18 09:42:39.844487 so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/modules/decoders/__init__.py
--rw-r--r--   0        0        0     1419 2023-04-18 09:42:39.844487 so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/modules/decoders/f0.py
--rw-r--r--   0        0        0       76 2023-04-18 09:42:39.844487 so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/modules/decoders/hifigan/__init__.py
--rw-r--r--   0        0        0    11618 2023-04-18 09:42:39.844487 so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py
--rw-r--r--   0        0        0      340 2023-04-18 09:42:39.844487 so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/modules/decoders/hifigan/_utils.py
--rw-r--r--   0        0        0      318 2023-04-18 09:42:39.844487 so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/modules/decoders/mb_istft/__init__.py
--rw-r--r--   0        0        0    12477 2023-04-18 09:42:39.844487 so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py
--rw-r--r--   0        0        0      419 2023-04-18 09:42:39.844487 so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/modules/decoders/mb_istft/_loss.py
--rw-r--r--   0        0        0     4725 2023-04-18 09:42:39.844487 so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py
--rw-r--r--   0        0        0     8954 2023-04-18 09:42:39.844487 so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py
--rw-r--r--   0        0        0     4879 2023-04-18 09:42:39.844487 so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py
--rw-r--r--   0        0        0     5604 2023-04-18 09:42:39.844487 so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/modules/descriminators.py
--rw-r--r--   0        0        0     4400 2023-04-18 09:42:39.844487 so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/modules/encoders.py
--rw-r--r--   0        0        0     1390 2023-04-18 09:42:39.844487 so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/modules/flows.py
--rw-r--r--   0        0        0     1405 2023-04-18 09:42:39.844487 so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/modules/losses.py
--rw-r--r--   0        0        0     5753 2023-04-18 09:42:39.844487 so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/modules/mel_processing.py
--rw-r--r--   0        0        0    14435 2023-04-18 09:42:39.844487 so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/modules/modules.py
--rw-r--r--   0        0        0     8178 2023-04-18 09:42:39.844487 so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/modules/synthesizers.py
--rw-r--r--   0        0        0        0 2023-04-18 09:42:39.844487 so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/preprocessing/__init__.py
--rw-r--r--   0        0        0     1737 2023-04-18 09:42:39.844487 so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json
--rw-r--r--   0        0        0     1487 2023-04-18 09:42:39.844487 so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json
--rw-r--r--   0        0        0     1548 2023-04-18 09:42:39.844487 so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json
--rw-r--r--   0        0        0     2793 2023-04-18 09:42:39.844487 so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py
--rw-r--r--   0        0        0     4646 2023-04-18 09:42:39.844487 so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py
--rw-r--r--   0        0        0     4382 2023-04-18 09:42:39.844487 so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/preprocessing/preprocess_resample.py
--rw-r--r--   0        0        0     2948 2023-04-18 09:42:39.844487 so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py
--rw-r--r--   0        0        0     1878 2023-04-18 09:42:39.844487 so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/preprocessing/preprocess_split.py
--rw-r--r--   0        0        0      126 2023-04-18 09:42:39.844487 so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/preprocessing/preprocess_utils.py
--rw-r--r--   0        0        0        0 2023-04-18 09:42:39.844487 so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/py.typed
--rw-r--r--   0        0        0    20145 2023-04-18 09:42:39.844487 so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/train.py
--rw-r--r--   0        0        0    13313 2023-04-18 09:42:39.844487 so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/utils.py
--rw-r--r--   0        0        0    20087 1970-01-01 00:00:00.000000 so_vits_svc_fork-3.9.4/PKG-INFO
+-rw-r--r--   0        0        0    12463 2023-04-18 10:19:48.034368 so_vits_svc_fork-3.9.5/LICENSE
+-rw-r--r--   0        0        0    18160 2023-04-18 10:19:48.034368 so_vits_svc_fork-3.9.5/README.md
+-rw-r--r--   0        0        0     3092 2023-04-18 10:19:49.082357 so_vits_svc_fork-3.9.5/pyproject.toml
+-rw-r--r--   0        0        0       70 2023-04-18 10:19:49.034358 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/__init__.py
+-rw-r--r--   0        0        0    22747 2023-04-18 10:19:48.034368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/__main__.py
+-rw-r--r--   0        0        0     1393 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/cluster/__init__.py
+-rw-r--r--   0        0        0     2844 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/cluster/train_cluster.py
+-rw-r--r--   0        0        0     2868 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/dataset.py
+-rw-r--r--   0        0        0     2454 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/default_gui_presets.json
+-rw-r--r--   0        0        0     7267 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/f0.py
+-rw-r--r--   0        0        0    25933 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/gui.py
+-rw-r--r--   0        0        0      864 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/hparams.py
+-rw-r--r--   0        0        0        0 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/inference/__init__.py
+-rw-r--r--   0        0        0    24054 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/inference/core.py
+-rw-r--r--   0        0        0     7485 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/inference/main.py
+-rw-r--r--   0        0        0     1213 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/logger.py
+-rw-r--r--   0        0        0        0 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/__init__.py
+-rw-r--r--   0        0        0    16683 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/attentions.py
+-rw-r--r--   0        0        0     4620 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/commons.py
+-rw-r--r--   0        0        0        0 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/decoders/__init__.py
+-rw-r--r--   0        0        0     1419 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/decoders/f0.py
+-rw-r--r--   0        0        0       76 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/decoders/hifigan/__init__.py
+-rw-r--r--   0        0        0    11618 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py
+-rw-r--r--   0        0        0      340 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/decoders/hifigan/_utils.py
+-rw-r--r--   0        0        0      318 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/decoders/mb_istft/__init__.py
+-rw-r--r--   0        0        0    12477 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py
+-rw-r--r--   0        0        0      419 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/decoders/mb_istft/_loss.py
+-rw-r--r--   0        0        0     4725 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py
+-rw-r--r--   0        0        0     8954 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py
+-rw-r--r--   0        0        0     4879 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py
+-rw-r--r--   0        0        0     5604 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/descriminators.py
+-rw-r--r--   0        0        0     4400 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/encoders.py
+-rw-r--r--   0        0        0     1390 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/flows.py
+-rw-r--r--   0        0        0     1405 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/losses.py
+-rw-r--r--   0        0        0     5753 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/mel_processing.py
+-rw-r--r--   0        0        0    14435 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/modules.py
+-rw-r--r--   0        0        0     8178 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/synthesizers.py
+-rw-r--r--   0        0        0        0 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/preprocessing/__init__.py
+-rw-r--r--   0        0        0     1737 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json
+-rw-r--r--   0        0        0     1487 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json
+-rw-r--r--   0        0        0     1548 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json
+-rw-r--r--   0        0        0     2793 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py
+-rw-r--r--   0        0        0     4646 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py
+-rw-r--r--   0        0        0     4382 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/preprocessing/preprocess_resample.py
+-rw-r--r--   0        0        0     2948 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py
+-rw-r--r--   0        0        0     1878 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/preprocessing/preprocess_split.py
+-rw-r--r--   0        0        0      126 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/preprocessing/preprocess_utils.py
+-rw-r--r--   0        0        0        0 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/py.typed
+-rw-r--r--   0        0        0    20240 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/train.py
+-rw-r--r--   0        0        0    13442 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/utils.py
+-rw-r--r--   0        0        0    20087 1970-01-01 00:00:00.000000 so_vits_svc_fork-3.9.5/PKG-INFO
```

### Comparing `so_vits_svc_fork-3.9.4/LICENSE` & `so_vits_svc_fork-3.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.4/README.md` & `so_vits_svc_fork-3.9.5/README.md`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.4/pyproject.toml` & `so_vits_svc_fork-3.9.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "so-vits-svc-fork"
-version = "3.9.4"
+version = "3.9.5"
 description = "A fork of so-vits-svc."
 authors = ["34j <34j.95a2p@simplelogin.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/34j/so-vits-svc-fork"
 documentation = "https://so-vits-svc-fork.readthedocs.io"
 classifiers = [
```

### Comparing `so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/__main__.py` & `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,26 +15,25 @@
 
 LOG = getLogger(__name__)
 
 IS_TEST = "test" in Path(__file__).parent.stem
 if IS_TEST:
     LOG.debug("Test mode is on.")
 
-LOG.info(f"Version: {__version__}")
-
 
 class RichHelpFormatter(click.HelpFormatter):
     def __init__(
         self,
         indent_increment: int = 2,
         width: int | None = None,
         max_width: int | None = None,
     ) -> None:
         width = 100
         super().__init__(indent_increment, width, max_width)
+        LOG.info(f"Version: {__version__}")
 
 
 def patch_wrap_text():
     orig_wrap_text = click.formatting.wrap_text
 
     def wrap_text(
         text,
```

### Comparing `so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/cluster/__init__.py` & `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/cluster/train_cluster.py` & `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/cluster/train_cluster.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/dataset.py` & `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/dataset.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/default_gui_presets.json` & `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/default_gui_presets.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/f0.py` & `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/gui.py` & `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import PySimpleGUI as sg
 import sounddevice as sd
 import soundfile as sf
 import torch
 from pebble import ProcessFuture, ProcessPool
 from tqdm.tk import tqdm_tk
 
+from . import __version__
 from .utils import ensure_pretrained_model, get_optimal_device
 
 GUI_DEFAULT_PRESETS_PATH = Path(__file__).parent / "default_gui_presets.json"
 GUI_PRESETS_PATH = Path("./user_gui_presets.json").absolute()
 
 LOG = getLogger(__name__)
 
@@ -93,14 +94,15 @@
         if auto_play:
             play_audio(output_path)
     except Exception as e:
         LOG.exception(e)
 
 
 def main():
+    LOG.info(f"version: {__version__}")
     try:
         ensure_pretrained_model(".", "contentvec", tqdm_cls=tqdm_tk)
     except Exception as e:
         LOG.exception(e)
         LOG.info("Trying tqdm.std...")
         try:
             ensure_pretrained_model(".", "contentvec")
```

### Comparing `so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/hparams.py` & `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/hparams.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/inference/core.py` & `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/inference/core.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/inference/main.py` & `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/inference/main.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/logger.py` & `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/logger.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import os
 import sys
-import warnings
 from logging import (
     DEBUG,
     INFO,
     FileHandler,
     StreamHandler,
     basicConfig,
     captureWarnings,
@@ -32,17 +31,14 @@
             StreamHandler() if is_notebook() else RichHandler(),
             FileHandler(f"{package_name}.log"),
         ],
     )
     if IS_TEST:
         getLogger(package_name).setLevel(DEBUG)
     captureWarnings(True)
-    warnings.filterwarnings(
-        "ignore", category=UserWarning, message="TypedStorage is deprecated"
-    )
     LOGGER_INIT = True
 
 
 def is_notebook():
     try:
         from IPython import get_ipython
```

### Comparing `so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/modules/attentions.py` & `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/attentions.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/modules/commons.py` & `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/commons.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/modules/decoders/f0.py` & `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/decoders/f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py` & `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py` & `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py` & `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py` & `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py` & `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/modules/descriminators.py` & `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/descriminators.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/modules/encoders.py` & `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/encoders.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/modules/flows.py` & `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/flows.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/modules/losses.py` & `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/losses.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/modules/mel_processing.py` & `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/mel_processing.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/modules/modules.py` & `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/modules.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/modules/synthesizers.py` & `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/synthesizers.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json` & `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json` & `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json` & `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py` & `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py` & `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/preprocessing/preprocess_resample.py` & `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/preprocessing/preprocess_resample.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py` & `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/preprocessing/preprocess_split.py` & `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/preprocessing/preprocess_split.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/train.py` & `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 from .logger import is_notebook
 from .modules.descriminators import MultiPeriodDiscriminator
 from .modules.losses import discriminator_loss, feature_loss, generator_loss, kl_loss
 from .modules.mel_processing import mel_spectrogram_torch
 from .modules.synthesizers import SynthesizerTrn
 
 LOG = getLogger(__name__)
-torch.backends.cudnn.benchmark = True
 torch.set_float32_matmul_precision("high")
 
 
 class VCDataModule(pl.LightningDataModule):
     batch_size: int
 
     def __init__(self, hparams: Any):
@@ -47,24 +46,23 @@
         # these should be called in setup(), but we need to calculate check_val_every_n_epoch
         self.train_dataset = TextAudioDataset(self.__hparams, is_validation=False)
         self.val_dataset = TextAudioDataset(self.__hparams, is_validation=True)
 
     def train_dataloader(self):
         return DataLoader(
             self.train_dataset,
-            # pin_memory=False,
-            num_workers=min(cpu_count(), self.__hparams.train.get("num_workers", 4)),
+            num_workers=min(cpu_count(), self.__hparams.train.get("num_workers", 8)),
             batch_size=self.batch_size,
             collate_fn=self.collate_fn,
+            persistent_workers=True,
         )
 
     def val_dataloader(self):
         return DataLoader(
             self.val_dataset,
-            # pin_memory=False,
             batch_size=1,
             collate_fn=self.collate_fn,
         )
 
 
 def train(
     config_path: Path | str, model_path: Path | str, reset_optimizer: bool = False
@@ -91,14 +89,16 @@
         precision="16-mixed"
         if hparams.train.fp16_run
         else "bf16-mixed"
         if hparams.train.get("bf16_run", False)
         else 32,
         strategy=strategy,
         callbacks=[pl.callbacks.RichProgressBar()] if not is_notebook() else None,
+        benchmark=True,
+        enable_checkpointing=False,
     )
     tuner = Tuner(trainer)
     model = VitsLightning(reset_optimizer=reset_optimizer, **hparams)
 
     # automatic batch size scaling
     batch_size = hparams.train.batch_size
     batch_split = str(batch_size).split("-")
@@ -478,14 +478,17 @@
 
         # end of epoch
         if self.trainer.is_last_batch:
             self.scheduler_g.step()
             self.scheduler_d.step()
 
     def validation_step(self, batch, batch_idx):
+        # avoid logging with wrong global step
+        if self.global_step == 0:
+            return
         with torch.no_grad():
             self.net_g.eval()
             c, f0, _, mel, y, g, _, uv = batch
             y_hat = self.net_g.infer(c, f0, uv, g=g)
             y_hat_mel = mel_spectrogram_torch(y_hat.squeeze(1).float(), self.hparams)
             self.log_audio_dict(
                 {f"gen/audio_{batch_idx}": y_hat[0], f"gt/audio_{batch_idx}": y[0]}
```

### Comparing `so_vits_svc_fork-3.9.4/src/so_vits_svc_fork/utils.py` & `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -187,15 +187,15 @@
     if not_in_to:
         warnings.warn(f"Keys not found in model state dict:" f"{not_in_to}")
     if not_in_from:
         warnings.warn(f"Keys not found in checkpoint state dict:" f"{not_in_from}")
     shape_missmatch = []
     for k, v in from_.items():
         if k not in to_:
-            warnings.warn(f"Key {k} not found in model state dict")
+            pass
         elif hasattr(v, "shape"):
             if not hasattr(to_[k], "shape"):
                 raise ValueError(f"Key {k} is not a tensor")
             if to_[k].shape == v.shape:
                 to_[k] = v
             else:
                 shape_missmatch.append((k, to_[k].shape, v.shape))
@@ -221,15 +221,19 @@
     model: torch.nn.Module,
     optimizer: torch.optim.Optimizer | None = None,
     skip_optimizer: bool = False,
 ) -> tuple[torch.nn.Module, torch.optim.Optimizer | None, float, int]:
     if not Path(checkpoint_path).is_file():
         raise FileNotFoundError(f"File {checkpoint_path} not found")
     with Path(checkpoint_path).open("rb") as f:
-        checkpoint_dict = torch.load(f, map_location="cpu", weights_only=True)
+        with warnings.catch_warnings():
+            warnings.filterwarnings(
+                "ignore", category=UserWarning, message="TypedStorage is deprecated"
+            )
+            checkpoint_dict = torch.load(f, map_location="cpu", weights_only=True)
     iteration = checkpoint_dict["iteration"]
     learning_rate = checkpoint_dict["learning_rate"]
 
     # safe load module
     if hasattr(model, "module"):
         safe_load(model.module, checkpoint_dict["model"])
     else:
```

### Comparing `so_vits_svc_fork-3.9.4/PKG-INFO` & `so_vits_svc_fork-3.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: so-vits-svc-fork
-Version: 3.9.4
+Version: 3.9.5
 Summary: A fork of so-vits-svc.
 Home-page: https://github.com/34j/so-vits-svc-fork
 License: MIT
 Author: 34j
 Author-email: 34j.95a2p@simplelogin.com
 Requires-Python: >=3.8,<3.11
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: so-vits-svc-fork Version: 3.9.4 Summary: A fork of
+Metadata-Version: 2.1 Name: so-vits-svc-fork Version: 3.9.5 Summary: A fork of
 so-vits-svc. Home-page: https://github.com/34j/so-vits-svc-fork License: MIT
 Author: 34j Author-email: 34j.95a2p@simplelogin.com Requires-Python:
 >=3.8,<3.11 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

