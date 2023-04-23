# Comparing `tmp/amt-tools-0.3.0.tar.gz` & `tmp/amt-tools-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amt-tools-0.3.0.tar", last modified: Sat Nov  5 13:21:47 2022, max compression
+gzip compressed data, was "amt-tools-0.3.1.tar", last modified: Sun Apr 23 16:44:03 2023, max compression
```

## Comparing `amt-tools-0.3.0.tar` & `amt-tools-0.3.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 rockstar  (1000) rockstar  (1000)        0 2022-11-05 13:21:47.893313 amt-tools-0.3.0/
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     1072 2022-09-14 19:54:16.000000 amt-tools-0.3.0/LICENSE.txt
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     1507 2022-11-05 13:21:47.893313 amt-tools-0.3.0/PKG-INFO
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     1155 2022-11-05 12:25:32.000000 amt-tools-0.3.0/README.md
-drwxrwxr-x   0 rockstar  (1000) rockstar  (1000)        0 2022-11-05 13:21:47.889313 amt-tools-0.3.0/amt_tools/
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)      816 2022-09-14 19:54:16.000000 amt-tools-0.3.0/amt_tools/__init__.py
-drwxrwxr-x   0 rockstar  (1000) rockstar  (1000)        0 2022-11-05 13:21:47.889313 amt-tools-0.3.0/amt_tools/datasets/
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     6397 2022-10-31 01:58:46.000000 amt-tools-0.3.0/amt_tools/datasets/GuitarSet.py
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     8626 2022-09-14 19:54:16.000000 amt-tools-0.3.0/amt_tools/datasets/MAESTRO.py
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     8539 2022-11-02 14:47:45.000000 amt-tools-0.3.0/amt_tools/datasets/MAPS.py
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)      915 2022-09-14 19:54:16.000000 amt-tools-0.3.0/amt_tools/datasets/__init__.py
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     1592 2022-09-14 19:54:16.000000 amt-tools-0.3.0/amt_tools/datasets/combo.py
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)    21147 2022-11-03 01:26:03.000000 amt-tools-0.3.0/amt_tools/datasets/common.py
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)    43876 2022-10-30 23:55:25.000000 amt-tools-0.3.0/amt_tools/evaluate.py
-drwxrwxr-x   0 rockstar  (1000) rockstar  (1000)        0 2022-11-05 13:21:47.893313 amt-tools-0.3.0/amt_tools/features/
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     1052 2022-10-30 15:27:46.000000 amt-tools-0.3.0/amt_tools/features/__init__.py
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     6127 2022-09-14 19:54:16.000000 amt-tools-0.3.0/amt_tools/features/combo.py
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     8022 2022-09-14 19:54:16.000000 amt-tools-0.3.0/amt_tools/features/common.py
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)      613 2022-09-14 19:54:16.000000 amt-tools-0.3.0/amt_tools/features/cqt.py
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)      598 2022-09-14 19:54:16.000000 amt-tools-0.3.0/amt_tools/features/hcqt.py
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     5192 2022-09-15 01:53:17.000000 amt-tools-0.3.0/amt_tools/features/hvqt.py
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     3000 2022-09-15 01:53:17.000000 amt-tools-0.3.0/amt_tools/features/mel.py
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     1843 2022-09-15 01:53:17.000000 amt-tools-0.3.0/amt_tools/features/power.py
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     2447 2022-09-15 01:53:17.000000 amt-tools-0.3.0/amt_tools/features/stft.py
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)    25872 2022-10-30 15:32:39.000000 amt-tools-0.3.0/amt_tools/features/stream.py
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     8063 2022-09-14 19:54:16.000000 amt-tools-0.3.0/amt_tools/features/vqt.py
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     5770 2022-09-15 01:53:17.000000 amt-tools-0.3.0/amt_tools/features/waveform.py
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     4844 2022-09-14 19:54:16.000000 amt-tools-0.3.0/amt_tools/inference.py
-drwxrwxr-x   0 rockstar  (1000) rockstar  (1000)        0 2022-11-05 13:21:47.893313 amt-tools-0.3.0/amt_tools/models/
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)      992 2022-09-14 19:54:16.000000 amt-tools-0.3.0/amt_tools/models/__init__.py
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)    19803 2022-10-11 02:31:35.000000 amt-tools-0.3.0/amt_tools/models/common.py
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)    22019 2022-09-15 01:53:17.000000 amt-tools-0.3.0/amt_tools/models/onsetsframes.py
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     7369 2022-10-06 12:43:33.000000 amt-tools-0.3.0/amt_tools/models/tabcnn.py
-drwxrwxr-x   0 rockstar  (1000) rockstar  (1000)        0 2022-11-05 13:21:47.893313 amt-tools-0.3.0/amt_tools/tools/
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)      946 2022-09-14 19:54:16.000000 amt-tools-0.3.0/amt_tools/tools/__init__.py
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     3843 2022-10-30 22:00:32.000000 amt-tools-0.3.0/amt_tools/tools/constants.py
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     8122 2022-10-30 22:03:23.000000 amt-tools-0.3.0/amt_tools/tools/instrument.py
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)    26499 2022-10-30 22:13:10.000000 amt-tools-0.3.0/amt_tools/tools/io.py
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)   126484 2022-10-31 17:16:58.000000 amt-tools-0.3.0/amt_tools/tools/utils.py
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)    42144 2022-10-30 23:02:53.000000 amt-tools-0.3.0/amt_tools/tools/visualize.py
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     8116 2022-11-02 14:47:31.000000 amt-tools-0.3.0/amt_tools/train.py
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)    44510 2022-10-10 20:48:57.000000 amt-tools-0.3.0/amt_tools/transcribe.py
-drwxrwxr-x   0 rockstar  (1000) rockstar  (1000)        0 2022-11-05 13:21:47.889313 amt-tools-0.3.0/amt_tools.egg-info/
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     1507 2022-11-05 13:21:47.000000 amt-tools-0.3.0/amt_tools.egg-info/PKG-INFO
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     1095 2022-11-05 13:21:47.000000 amt-tools-0.3.0/amt_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)        1 2022-11-05 13:21:47.000000 amt-tools-0.3.0/amt_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)      136 2022-11-05 13:21:47.000000 amt-tools-0.3.0/amt_tools.egg-info/requires.txt
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)       10 2022-11-05 13:21:47.000000 amt-tools-0.3.0/amt_tools.egg-info/top_level.txt
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)       38 2022-11-05 13:21:47.893313 amt-tools-0.3.0/setup.cfg
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     1058 2022-11-02 21:04:13.000000 amt-tools-0.3.0/setup.py
+drwxrwxr-x   0 rockstar  (1000) rockstar  (1000)        0 2023-04-23 16:44:03.893197 amt-tools-0.3.1/
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     1072 2022-09-21 18:10:59.000000 amt-tools-0.3.1/LICENSE.txt
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     1507 2023-04-23 16:44:03.893197 amt-tools-0.3.1/PKG-INFO
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     1155 2022-11-08 18:34:49.000000 amt-tools-0.3.1/README.md
+drwxrwxr-x   0 rockstar  (1000) rockstar  (1000)        0 2023-04-23 16:44:03.889197 amt-tools-0.3.1/amt_tools/
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)      816 2022-09-21 18:10:59.000000 amt-tools-0.3.1/amt_tools/__init__.py
+drwxrwxr-x   0 rockstar  (1000) rockstar  (1000)        0 2023-04-23 16:44:03.889197 amt-tools-0.3.1/amt_tools/datasets/
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     6397 2022-11-08 18:34:49.000000 amt-tools-0.3.1/amt_tools/datasets/GuitarSet.py
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     8626 2022-09-21 18:10:59.000000 amt-tools-0.3.1/amt_tools/datasets/MAESTRO.py
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     8539 2022-11-08 18:34:49.000000 amt-tools-0.3.1/amt_tools/datasets/MAPS.py
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)      915 2022-09-21 18:10:59.000000 amt-tools-0.3.1/amt_tools/datasets/__init__.py
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     1592 2022-09-21 18:10:59.000000 amt-tools-0.3.1/amt_tools/datasets/combo.py
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)    21147 2022-11-08 18:34:49.000000 amt-tools-0.3.1/amt_tools/datasets/common.py
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)    43876 2022-11-08 18:34:49.000000 amt-tools-0.3.1/amt_tools/evaluate.py
+drwxrwxr-x   0 rockstar  (1000) rockstar  (1000)        0 2023-04-23 16:44:03.893197 amt-tools-0.3.1/amt_tools/features/
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     1052 2022-11-08 18:34:49.000000 amt-tools-0.3.1/amt_tools/features/__init__.py
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     6127 2022-09-21 18:10:59.000000 amt-tools-0.3.1/amt_tools/features/combo.py
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     8022 2022-09-21 18:10:59.000000 amt-tools-0.3.1/amt_tools/features/common.py
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)      613 2022-09-21 18:10:59.000000 amt-tools-0.3.1/amt_tools/features/cqt.py
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)      598 2022-09-21 18:10:59.000000 amt-tools-0.3.1/amt_tools/features/hcqt.py
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     5258 2023-04-23 16:40:14.000000 amt-tools-0.3.1/amt_tools/features/hvqt.py
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     3000 2022-11-08 18:34:49.000000 amt-tools-0.3.1/amt_tools/features/mel.py
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     1843 2022-11-08 18:34:49.000000 amt-tools-0.3.1/amt_tools/features/power.py
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     2447 2022-11-08 18:34:49.000000 amt-tools-0.3.1/amt_tools/features/stft.py
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)    25872 2022-11-08 18:34:49.000000 amt-tools-0.3.1/amt_tools/features/stream.py
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     8063 2022-09-21 18:10:59.000000 amt-tools-0.3.1/amt_tools/features/vqt.py
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     5770 2022-11-08 18:34:49.000000 amt-tools-0.3.1/amt_tools/features/waveform.py
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     4844 2022-09-21 18:10:59.000000 amt-tools-0.3.1/amt_tools/inference.py
+drwxrwxr-x   0 rockstar  (1000) rockstar  (1000)        0 2023-04-23 16:44:03.893197 amt-tools-0.3.1/amt_tools/models/
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)      992 2022-09-21 18:10:59.000000 amt-tools-0.3.1/amt_tools/models/__init__.py
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)    19803 2022-11-08 18:34:49.000000 amt-tools-0.3.1/amt_tools/models/common.py
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)    22019 2022-11-08 18:34:49.000000 amt-tools-0.3.1/amt_tools/models/onsetsframes.py
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     7369 2022-11-08 18:34:49.000000 amt-tools-0.3.1/amt_tools/models/tabcnn.py
+drwxrwxr-x   0 rockstar  (1000) rockstar  (1000)        0 2023-04-23 16:44:03.893197 amt-tools-0.3.1/amt_tools/tools/
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)      946 2022-09-21 18:10:59.000000 amt-tools-0.3.1/amt_tools/tools/__init__.py
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     3843 2022-11-08 18:34:49.000000 amt-tools-0.3.1/amt_tools/tools/constants.py
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     8122 2022-11-08 18:34:49.000000 amt-tools-0.3.1/amt_tools/tools/instrument.py
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)    26499 2022-11-08 18:34:49.000000 amt-tools-0.3.1/amt_tools/tools/io.py
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)   126484 2022-11-08 18:34:49.000000 amt-tools-0.3.1/amt_tools/tools/utils.py
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)    42144 2022-11-08 18:34:49.000000 amt-tools-0.3.1/amt_tools/tools/visualize.py
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     8116 2022-09-21 18:10:59.000000 amt-tools-0.3.1/amt_tools/train.py
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)    44510 2022-11-08 18:34:49.000000 amt-tools-0.3.1/amt_tools/transcribe.py
+drwxrwxr-x   0 rockstar  (1000) rockstar  (1000)        0 2023-04-23 16:44:03.889197 amt-tools-0.3.1/amt_tools.egg-info/
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     1507 2023-04-23 16:44:03.000000 amt-tools-0.3.1/amt_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     1095 2023-04-23 16:44:03.000000 amt-tools-0.3.1/amt_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)        1 2023-04-23 16:44:03.000000 amt-tools-0.3.1/amt_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)      136 2023-04-23 16:44:03.000000 amt-tools-0.3.1/amt_tools.egg-info/requires.txt
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)       10 2023-04-23 16:44:03.000000 amt-tools-0.3.1/amt_tools.egg-info/top_level.txt
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)       38 2023-04-23 16:44:03.893197 amt-tools-0.3.1/setup.cfg
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     1058 2023-04-23 16:41:49.000000 amt-tools-0.3.1/setup.py
```

### Comparing `amt-tools-0.3.0/LICENSE.txt` & `amt-tools-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `amt-tools-0.3.0/PKG-INFO` & `amt-tools-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amt-tools
-Version: 0.3.0
+Version: 0.3.1
 Summary: Machine learning tools and framework for automatic music transcription
 Home-page: https://github.com/cwitkowitz/amt-tools
 Author: Frank Cwitkowitz
 Author-email: fcwitkow@ur.rochester.edu
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `amt-tools-0.3.0/README.md` & `amt-tools-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `amt-tools-0.3.0/amt_tools/__init__.py` & `amt-tools-0.3.1/amt_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `amt-tools-0.3.0/amt_tools/datasets/GuitarSet.py` & `amt-tools-0.3.1/amt_tools/datasets/GuitarSet.py`

 * *Files identical despite different names*

### Comparing `amt-tools-0.3.0/amt_tools/datasets/MAESTRO.py` & `amt-tools-0.3.1/amt_tools/datasets/MAESTRO.py`

 * *Files identical despite different names*

### Comparing `amt-tools-0.3.0/amt_tools/datasets/MAPS.py` & `amt-tools-0.3.1/amt_tools/datasets/MAPS.py`

 * *Files identical despite different names*

### Comparing `amt-tools-0.3.0/amt_tools/datasets/__init__.py` & `amt-tools-0.3.1/amt_tools/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `amt-tools-0.3.0/amt_tools/datasets/combo.py` & `amt-tools-0.3.1/amt_tools/datasets/combo.py`

 * *Files identical despite different names*

### Comparing `amt-tools-0.3.0/amt_tools/datasets/common.py` & `amt-tools-0.3.1/amt_tools/datasets/common.py`

 * *Files identical despite different names*

### Comparing `amt-tools-0.3.0/amt_tools/evaluate.py` & `amt-tools-0.3.1/amt_tools/evaluate.py`

 * *Files identical despite different names*

### Comparing `amt-tools-0.3.0/amt_tools/features/__init__.py` & `amt-tools-0.3.1/amt_tools/features/__init__.py`

 * *Files identical despite different names*

### Comparing `amt-tools-0.3.0/amt_tools/features/combo.py` & `amt-tools-0.3.1/amt_tools/features/combo.py`

 * *Files identical despite different names*

### Comparing `amt-tools-0.3.0/amt_tools/features/common.py` & `amt-tools-0.3.1/amt_tools/features/common.py`

 * *Files identical despite different names*

### Comparing `amt-tools-0.3.0/amt_tools/features/cqt.py` & `amt-tools-0.3.1/amt_tools/features/cqt.py`

 * *Files identical despite different names*

### Comparing `amt-tools-0.3.0/amt_tools/features/hcqt.py` & `amt-tools-0.3.1/amt_tools/features/hcqt.py`

 * *Files identical despite different names*

### Comparing `amt-tools-0.3.0/amt_tools/features/hvqt.py` & `amt-tools-0.3.1/amt_tools/features/hvqt.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,16 +158,16 @@
 
         Returns
         ----------
         times : ndarray
           Time in seconds of each frame
         """
 
-        # Use the times of the lowest harmonic's transform
-        times = self.modules[0].get_times(audio, at_start)
+        # Use the times of the lowest harmonic's transform, trimmed to the expected frames
+        times = self.modules[0].get_times(audio, at_start)[:self.get_expected_frames(audio)]
 
         return times
 
     def get_feature_size(self):
         """
         Helper function to access dimensionality of features.
```

### Comparing `amt-tools-0.3.0/amt_tools/features/mel.py` & `amt-tools-0.3.1/amt_tools/features/mel.py`

 * *Files identical despite different names*

### Comparing `amt-tools-0.3.0/amt_tools/features/power.py` & `amt-tools-0.3.1/amt_tools/features/power.py`

 * *Files identical despite different names*

### Comparing `amt-tools-0.3.0/amt_tools/features/stft.py` & `amt-tools-0.3.1/amt_tools/features/stft.py`

 * *Files identical despite different names*

### Comparing `amt-tools-0.3.0/amt_tools/features/stream.py` & `amt-tools-0.3.1/amt_tools/features/stream.py`

 * *Files identical despite different names*

### Comparing `amt-tools-0.3.0/amt_tools/features/vqt.py` & `amt-tools-0.3.1/amt_tools/features/vqt.py`

 * *Files identical despite different names*

### Comparing `amt-tools-0.3.0/amt_tools/features/waveform.py` & `amt-tools-0.3.1/amt_tools/features/waveform.py`

 * *Files identical despite different names*

### Comparing `amt-tools-0.3.0/amt_tools/inference.py` & `amt-tools-0.3.1/amt_tools/inference.py`

 * *Files identical despite different names*

### Comparing `amt-tools-0.3.0/amt_tools/models/__init__.py` & `amt-tools-0.3.1/amt_tools/models/__init__.py`

 * *Files identical despite different names*

### Comparing `amt-tools-0.3.0/amt_tools/models/common.py` & `amt-tools-0.3.1/amt_tools/models/common.py`

 * *Files identical despite different names*

### Comparing `amt-tools-0.3.0/amt_tools/models/onsetsframes.py` & `amt-tools-0.3.1/amt_tools/models/onsetsframes.py`

 * *Files identical despite different names*

### Comparing `amt-tools-0.3.0/amt_tools/models/tabcnn.py` & `amt-tools-0.3.1/amt_tools/models/tabcnn.py`

 * *Files identical despite different names*

### Comparing `amt-tools-0.3.0/amt_tools/tools/__init__.py` & `amt-tools-0.3.1/amt_tools/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `amt-tools-0.3.0/amt_tools/tools/constants.py` & `amt-tools-0.3.1/amt_tools/tools/constants.py`

 * *Files identical despite different names*

### Comparing `amt-tools-0.3.0/amt_tools/tools/instrument.py` & `amt-tools-0.3.1/amt_tools/tools/instrument.py`

 * *Files identical despite different names*

### Comparing `amt-tools-0.3.0/amt_tools/tools/io.py` & `amt-tools-0.3.1/amt_tools/tools/io.py`

 * *Files identical despite different names*

### Comparing `amt-tools-0.3.0/amt_tools/tools/utils.py` & `amt-tools-0.3.1/amt_tools/tools/utils.py`

 * *Files identical despite different names*

### Comparing `amt-tools-0.3.0/amt_tools/tools/visualize.py` & `amt-tools-0.3.1/amt_tools/tools/visualize.py`

 * *Files identical despite different names*

### Comparing `amt-tools-0.3.0/amt_tools/train.py` & `amt-tools-0.3.1/amt_tools/train.py`

 * *Files identical despite different names*

### Comparing `amt-tools-0.3.0/amt_tools/transcribe.py` & `amt-tools-0.3.1/amt_tools/transcribe.py`

 * *Files identical despite different names*

### Comparing `amt-tools-0.3.0/amt_tools.egg-info/PKG-INFO` & `amt-tools-0.3.1/amt_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amt-tools
-Version: 0.3.0
+Version: 0.3.1
 Summary: Machine learning tools and framework for automatic music transcription
 Home-page: https://github.com/cwitkowitz/amt-tools
 Author: Frank Cwitkowitz
 Author-email: fcwitkow@ur.rochester.edu
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `amt-tools-0.3.0/amt_tools.egg-info/SOURCES.txt` & `amt-tools-0.3.1/amt_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amt-tools-0.3.0/setup.py` & `amt-tools-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,13 +11,13 @@
     # TODO - why does 'pip install -e' consider generated/examples as packages?
     packages=find_packages(),
     python_requires='>=3.8',
     install_requires=['numpy', 'librosa', 'torch', 'matplotlib', 'sacred', 'mir_eval',
                       'jams', 'mido', 'requests', 'tqdm', 'tensorboard', 'tensorboardX',
                       'scipy', 'pandas', 'mirdata', 'sounddevice', 'pynput'],
     #scripts=['examples/of_1.py', 'examples/of_2.py', 'examples/tabcnn.py'],
-    version='0.3.0',
+    version='0.3.1',
     license='MIT',
     description='Machine learning tools and framework for automatic music transcription',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown'
 )
```

