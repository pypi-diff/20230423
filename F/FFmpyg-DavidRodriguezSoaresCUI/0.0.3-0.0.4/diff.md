# Comparing `tmp/FFmpyg_DavidRodriguezSoaresCUI-0.0.3.tar.gz` & `tmp/FFmpyg_DavidRodriguezSoaresCUI-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FFmpyg_DavidRodriguezSoaresCUI-0.0.3.tar", last modified: Sun Apr 23 13:48:31 2023, max compression
+gzip compressed data, was "FFmpyg_DavidRodriguezSoaresCUI-0.0.4.tar", last modified: Sun Apr 23 15:34:30 2023, max compression
```

## Comparing `FFmpyg_DavidRodriguezSoaresCUI-0.0.3.tar` & `FFmpyg_DavidRodriguezSoaresCUI-0.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 13:48:31.194509 FFmpyg_DavidRodriguezSoaresCUI-0.0.3/
--rw-rw-rw-   0        0        0     6432 2023-04-10 17:40:33.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     9720 2023-04-23 13:48:31.193508 FFmpyg_DavidRodriguezSoaresCUI-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2353 2023-04-16 19:08:19.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.3/README.md
--rw-rw-rw-   0        0        0      814 2023-04-23 13:41:06.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-23 13:48:31.194509 FFmpyg_DavidRodriguezSoaresCUI-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-23 13:48:31.169486 FFmpyg_DavidRodriguezSoaresCUI-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-23 13:48:31.181496 FFmpyg_DavidRodriguezSoaresCUI-0.0.3/src/FFmpyg/
--rw-rw-rw-   0        0        0        0 2023-04-16 17:50:35.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.3/src/FFmpyg/__init__.py
--rw-rw-rw-   0        0        0     2042 2023-04-23 11:58:31.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.3/src/FFmpyg/command.py
--rw-rw-rw-   0        0        0     7167 2023-04-23 13:37:36.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.3/src/FFmpyg/encoder_spec.py
--rw-rw-rw-   0        0        0     1218 2023-04-15 16:47:24.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.3/src/FFmpyg/enums.py
--rw-rw-rw-   0        0        0      296 2023-04-23 11:44:20.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.3/src/FFmpyg/exceptions.py
--rw-rw-rw-   0        0        0     3065 2023-04-16 17:49:59.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.3/src/FFmpyg/ffile.py
--rw-rw-rw-   0        0        0    12453 2023-04-23 13:34:51.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.3/src/FFmpyg/ffmpeg_command.py
--rw-rw-rw-   0        0        0     7606 2023-04-23 11:56:01.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.3/src/FFmpyg/ffmpeg_encoder.py
--rw-rw-rw-   0        0        0     1829 2023-04-23 12:35:50.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.3/src/FFmpyg/ffmpeg_lib.py
--rw-rw-rw-   0        0        0    12019 2023-04-23 13:39:19.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.3/src/FFmpyg/ffmpeg_vmaf.py
--rw-rw-rw-   0        0        0      987 2023-04-16 17:49:28.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.3/src/FFmpyg/ffprobe.py
--rw-rw-rw-   0        0        0     5152 2023-04-16 17:49:21.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.3/src/FFmpyg/stream.py
--rw-rw-rw-   0        0        0     5690 2023-04-23 11:32:06.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.3/src/FFmpyg/utils.py
--rw-rw-rw-   0        0        0     7432 2023-04-23 13:38:43.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.3/src/FFmpyg/virtualfs.py
-drwxrwxrwx   0        0        0        0 2023-04-23 13:48:31.193508 FFmpyg_DavidRodriguezSoaresCUI-0.0.3/src/FFmpyg_DavidRodriguezSoaresCUI.egg-info/
--rw-rw-rw-   0        0        0     9720 2023-04-23 13:48:31.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.3/src/FFmpyg_DavidRodriguezSoaresCUI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      597 2023-04-23 13:48:31.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.3/src/FFmpyg_DavidRodriguezSoaresCUI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 13:48:31.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.3/src/FFmpyg_DavidRodriguezSoaresCUI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-23 13:48:31.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.3/src/FFmpyg_DavidRodriguezSoaresCUI.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 15:34:30.096455 FFmpyg_DavidRodriguezSoaresCUI-0.0.4/
+-rw-rw-rw-   0        0        0     6432 2023-04-10 17:40:33.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     9720 2023-04-23 15:34:30.096455 FFmpyg_DavidRodriguezSoaresCUI-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2353 2023-04-16 19:08:19.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.4/README.md
+-rw-rw-rw-   0        0        0      814 2023-04-23 15:33:18.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-23 15:34:30.096455 FFmpyg_DavidRodriguezSoaresCUI-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-23 15:34:30.074437 FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-04-23 15:34:30.086448 FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg/
+-rw-rw-rw-   0        0        0        0 2023-04-16 17:50:35.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg/__init__.py
+-rw-rw-rw-   0        0        0     2042 2023-04-23 11:58:31.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg/command.py
+-rw-rw-rw-   0        0        0     7167 2023-04-23 13:37:36.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg/encoder_spec.py
+-rw-rw-rw-   0        0        0     1218 2023-04-15 16:47:24.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg/enums.py
+-rw-rw-rw-   0        0        0      296 2023-04-23 11:44:20.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg/exceptions.py
+-rw-rw-rw-   0        0        0     3065 2023-04-16 17:49:59.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg/ffile.py
+-rw-rw-rw-   0        0        0    12453 2023-04-23 13:34:51.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg/ffmpeg_command.py
+-rw-rw-rw-   0        0        0     7606 2023-04-23 11:56:01.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg/ffmpeg_encoder.py
+-rw-rw-rw-   0        0        0     1829 2023-04-23 12:35:50.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg/ffmpeg_lib.py
+-rw-rw-rw-   0        0        0    12018 2023-04-23 15:28:26.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg/ffmpeg_vmaf.py
+-rw-rw-rw-   0        0        0      987 2023-04-16 17:49:28.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg/ffprobe.py
+-rw-rw-rw-   0        0        0     5152 2023-04-16 17:49:21.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg/stream.py
+-rw-rw-rw-   0        0        0     5690 2023-04-23 11:32:06.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg/utils.py
+-rw-rw-rw-   0        0        0     7432 2023-04-23 13:38:43.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg/virtualfs.py
+drwxrwxrwx   0        0        0        0 2023-04-23 15:34:30.095456 FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg_DavidRodriguezSoaresCUI.egg-info/
+-rw-rw-rw-   0        0        0     9720 2023-04-23 15:34:30.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg_DavidRodriguezSoaresCUI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      597 2023-04-23 15:34:30.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg_DavidRodriguezSoaresCUI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 15:34:30.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg_DavidRodriguezSoaresCUI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-23 15:34:30.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg_DavidRodriguezSoaresCUI.egg-info/top_level.txt
```

### Comparing `FFmpyg_DavidRodriguezSoaresCUI-0.0.3/LICENSE` & `FFmpyg_DavidRodriguezSoaresCUI-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `FFmpyg_DavidRodriguezSoaresCUI-0.0.3/PKG-INFO` & `FFmpyg_DavidRodriguezSoaresCUI-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FFmpyg_DavidRodriguezSoaresCUI
-Version: 0.0.3
+Version: 0.0.4
 Summary: A FFMPEG interface for Python by DavidRodriguezSoaresCUI
 Author-email: DavidRodriguezSoaresCUI <fireblaze904+FFmpyg@gmail.com>
 License: CC0 1.0 Universal
         
         Statement of Purpose
         
         The laws of most jurisdictions throughout the world automatically confer exclusive Copyright and Related Rights (defined below) upon the creator and subsequent owner(s) (each and all, an "owner") of an original work of authorship and/or a database (each, a "Work").
```

### Comparing `FFmpyg_DavidRodriguezSoaresCUI-0.0.3/README.md` & `FFmpyg_DavidRodriguezSoaresCUI-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `FFmpyg_DavidRodriguezSoaresCUI-0.0.3/pyproject.toml` & `FFmpyg_DavidRodriguezSoaresCUI-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "FFmpyg_DavidRodriguezSoaresCUI"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="DavidRodriguezSoaresCUI", email="fireblaze904+FFmpyg@gmail.com" },
 ]
 description = "A FFMPEG interface for Python by DavidRodriguezSoaresCUI"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `FFmpyg_DavidRodriguezSoaresCUI-0.0.3/src/FFmpyg/command.py` & `FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg/command.py`

 * *Files identical despite different names*

### Comparing `FFmpyg_DavidRodriguezSoaresCUI-0.0.3/src/FFmpyg/encoder_spec.py` & `FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg/encoder_spec.py`

 * *Files identical despite different names*

### Comparing `FFmpyg_DavidRodriguezSoaresCUI-0.0.3/src/FFmpyg/enums.py` & `FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg/enums.py`

 * *Files identical despite different names*

### Comparing `FFmpyg_DavidRodriguezSoaresCUI-0.0.3/src/FFmpyg/ffile.py` & `FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg/ffile.py`

 * *Files identical despite different names*

### Comparing `FFmpyg_DavidRodriguezSoaresCUI-0.0.3/src/FFmpyg/ffmpeg_command.py` & `FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg/ffmpeg_command.py`

 * *Files identical despite different names*

### Comparing `FFmpyg_DavidRodriguezSoaresCUI-0.0.3/src/FFmpyg/ffmpeg_encoder.py` & `FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg/ffmpeg_encoder.py`

 * *Files identical despite different names*

### Comparing `FFmpyg_DavidRodriguezSoaresCUI-0.0.3/src/FFmpyg/ffmpeg_lib.py` & `FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg/ffmpeg_lib.py`

 * *Files identical despite different names*

### Comparing `FFmpyg_DavidRodriguezSoaresCUI-0.0.3/src/FFmpyg/ffmpeg_vmaf.py` & `FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg/ffmpeg_vmaf.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import json
 import logging
 import math
 from pathlib import Path
 from typing import Dict, List, Union
 
 import numpy as np
-from DRSlib.utils import get_temporary_dir_name
+from DRSlib.hash import get_temporary_dir_name
 from matplotlib import pyplot as plt
 
 from .enums import FfprobeInfoKey, StreamType
 from .ffile import MediaFile, StreamCriteria
 from .ffmpeg_command import (
     FfmpegInput,
     FfmpegOptions,
```

### Comparing `FFmpyg_DavidRodriguezSoaresCUI-0.0.3/src/FFmpyg/ffprobe.py` & `FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg/ffprobe.py`

 * *Files identical despite different names*

### Comparing `FFmpyg_DavidRodriguezSoaresCUI-0.0.3/src/FFmpyg/stream.py` & `FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg/stream.py`

 * *Files identical despite different names*

### Comparing `FFmpyg_DavidRodriguezSoaresCUI-0.0.3/src/FFmpyg/utils.py` & `FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg/utils.py`

 * *Files identical despite different names*

### Comparing `FFmpyg_DavidRodriguezSoaresCUI-0.0.3/src/FFmpyg/virtualfs.py` & `FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg/virtualfs.py`

 * *Files identical despite different names*

### Comparing `FFmpyg_DavidRodriguezSoaresCUI-0.0.3/src/FFmpyg_DavidRodriguezSoaresCUI.egg-info/PKG-INFO` & `FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg_DavidRodriguezSoaresCUI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FFmpyg-DavidRodriguezSoaresCUI
-Version: 0.0.3
+Version: 0.0.4
 Summary: A FFMPEG interface for Python by DavidRodriguezSoaresCUI
 Author-email: DavidRodriguezSoaresCUI <fireblaze904+FFmpyg@gmail.com>
 License: CC0 1.0 Universal
         
         Statement of Purpose
         
         The laws of most jurisdictions throughout the world automatically confer exclusive Copyright and Related Rights (defined below) upon the creator and subsequent owner(s) (each and all, an "owner") of an original work of authorship and/or a database (each, a "Work").
```

### Comparing `FFmpyg_DavidRodriguezSoaresCUI-0.0.3/src/FFmpyg_DavidRodriguezSoaresCUI.egg-info/SOURCES.txt` & `FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg_DavidRodriguezSoaresCUI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

