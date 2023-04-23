# Comparing `tmp/FFmpyg_DavidRodriguezSoaresCUI-0.0.1.tar.gz` & `tmp/FFmpyg_DavidRodriguezSoaresCUI-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FFmpyg_DavidRodriguezSoaresCUI-0.0.1.tar", last modified: Sun Apr 16 19:40:47 2023, max compression
+gzip compressed data, was "FFmpyg_DavidRodriguezSoaresCUI-0.0.2.tar", last modified: Sun Apr 23 11:49:51 2023, max compression
```

## Comparing `FFmpyg_DavidRodriguezSoaresCUI-0.0.1.tar` & `FFmpyg_DavidRodriguezSoaresCUI-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 19:40:47.782112 FFmpyg_DavidRodriguezSoaresCUI-0.0.1/
--rw-rw-rw-   0        0        0     6432 2023-04-10 17:40:33.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     9720 2023-04-16 19:40:47.782112 FFmpyg_DavidRodriguezSoaresCUI-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2353 2023-04-16 19:08:19.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.1/README.md
--rw-rw-rw-   0        0        0      814 2023-04-16 19:39:22.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-16 19:40:47.782112 FFmpyg_DavidRodriguezSoaresCUI-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-16 19:40:47.766481 FFmpyg_DavidRodriguezSoaresCUI-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-16 19:40:47.782112 FFmpyg_DavidRodriguezSoaresCUI-0.0.1/src/FFmpyg/
--rw-rw-rw-   0        0        0        0 2023-04-16 17:50:35.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.1/src/FFmpyg/__init__.py
--rw-rw-rw-   0        0        0     2048 2023-04-16 17:50:11.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.1/src/FFmpyg/command.py
--rw-rw-rw-   0        0        0     7803 2023-04-16 17:50:07.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.1/src/FFmpyg/encoder_spec.py
--rw-rw-rw-   0        0        0     1218 2023-04-15 16:47:24.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.1/src/FFmpyg/enums.py
--rw-rw-rw-   0        0        0      296 2023-04-13 20:15:22.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.1/src/FFmpyg/exceptions.py
--rw-rw-rw-   0        0        0     3065 2023-04-16 17:49:59.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.1/src/FFmpyg/ffile.py
--rw-rw-rw-   0        0        0    13900 2023-04-16 17:49:49.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.1/src/FFmpyg/ffmpeg_command.py
--rw-rw-rw-   0        0        0     8041 2023-04-16 17:49:38.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.1/src/FFmpyg/ffmpeg_encoder.py
--rw-rw-rw-   0        0        0      987 2023-04-16 17:49:28.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.1/src/FFmpyg/ffprobe.py
--rw-rw-rw-   0        0        0     5152 2023-04-16 17:49:21.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.1/src/FFmpyg/stream.py
--rw-rw-rw-   0        0        0     5633 2023-04-16 12:03:31.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.1/src/FFmpyg/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-16 19:40:47.782112 FFmpyg_DavidRodriguezSoaresCUI-0.0.1/src/FFmpyg_DavidRodriguezSoaresCUI.egg-info/
--rw-rw-rw-   0        0        0     9720 2023-04-16 19:40:47.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.1/src/FFmpyg_DavidRodriguezSoaresCUI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      522 2023-04-16 19:40:47.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.1/src/FFmpyg_DavidRodriguezSoaresCUI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 19:40:47.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.1/src/FFmpyg_DavidRodriguezSoaresCUI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-16 19:40:47.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.1/src/FFmpyg_DavidRodriguezSoaresCUI.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 11:49:51.662006 FFmpyg_DavidRodriguezSoaresCUI-0.0.2/
+-rw-rw-rw-   0        0        0     6432 2023-04-10 17:40:33.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     9720 2023-04-23 11:49:51.662006 FFmpyg_DavidRodriguezSoaresCUI-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2353 2023-04-16 19:08:19.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.2/README.md
+-rw-rw-rw-   0        0        0      814 2023-04-23 11:44:44.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-23 11:49:51.663007 FFmpyg_DavidRodriguezSoaresCUI-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-23 11:49:51.638986 FFmpyg_DavidRodriguezSoaresCUI-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-23 11:49:51.648995 FFmpyg_DavidRodriguezSoaresCUI-0.0.2/src/FFmpyg/
+-rw-rw-rw-   0        0        0        0 2023-04-16 17:50:35.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.2/src/FFmpyg/__init__.py
+-rw-rw-rw-   0        0        0     2048 2023-04-16 17:50:11.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.2/src/FFmpyg/command.py
+-rw-rw-rw-   0        0        0     7803 2023-04-16 17:50:07.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.2/src/FFmpyg/encoder_spec.py
+-rw-rw-rw-   0        0        0     1218 2023-04-15 16:47:24.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.2/src/FFmpyg/enums.py
+-rw-rw-rw-   0        0        0      296 2023-04-23 11:44:20.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.2/src/FFmpyg/exceptions.py
+-rw-rw-rw-   0        0        0     3065 2023-04-16 17:49:59.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.2/src/FFmpyg/ffile.py
+-rw-rw-rw-   0        0        0    13900 2023-04-16 17:49:49.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.2/src/FFmpyg/ffmpeg_command.py
+-rw-rw-rw-   0        0        0     8041 2023-04-16 17:49:38.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.2/src/FFmpyg/ffmpeg_encoder.py
+-rw-rw-rw-   0        0        0     2083 2023-04-23 11:42:21.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.2/src/FFmpyg/ffmpeg_lib.py
+-rw-rw-rw-   0        0        0      987 2023-04-16 17:49:28.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.2/src/FFmpyg/ffprobe.py
+-rw-rw-rw-   0        0        0     5152 2023-04-16 17:49:21.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.2/src/FFmpyg/stream.py
+-rw-rw-rw-   0        0        0     5690 2023-04-23 11:32:06.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.2/src/FFmpyg/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-23 11:49:51.661006 FFmpyg_DavidRodriguezSoaresCUI-0.0.2/src/FFmpyg_DavidRodriguezSoaresCUI.egg-info/
+-rw-rw-rw-   0        0        0     9720 2023-04-23 11:49:51.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.2/src/FFmpyg_DavidRodriguezSoaresCUI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      547 2023-04-23 11:49:51.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.2/src/FFmpyg_DavidRodriguezSoaresCUI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 11:49:51.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.2/src/FFmpyg_DavidRodriguezSoaresCUI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-23 11:49:51.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.2/src/FFmpyg_DavidRodriguezSoaresCUI.egg-info/top_level.txt
```

### Comparing `FFmpyg_DavidRodriguezSoaresCUI-0.0.1/LICENSE` & `FFmpyg_DavidRodriguezSoaresCUI-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `FFmpyg_DavidRodriguezSoaresCUI-0.0.1/PKG-INFO` & `FFmpyg_DavidRodriguezSoaresCUI-0.0.2/src/FFmpyg_DavidRodriguezSoaresCUI.egg-info/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: FFmpyg_DavidRodriguezSoaresCUI
-Version: 0.0.1
+Name: FFmpyg-DavidRodriguezSoaresCUI
+Version: 0.0.2
 Summary: A FFMPEG interface for Python by DavidRodriguezSoaresCUI
 Author-email: DavidRodriguezSoaresCUI <fireblaze904+FFmpyg@gmail.com>
 License: CC0 1.0 Universal
         
         Statement of Purpose
         
         The laws of most jurisdictions throughout the world automatically confer exclusive Copyright and Related Rights (defined below) upon the creator and subsequent owner(s) (each and all, an "owner") of an original work of authorship and/or a database (each, a "Work").
```

### Comparing `FFmpyg_DavidRodriguezSoaresCUI-0.0.1/README.md` & `FFmpyg_DavidRodriguezSoaresCUI-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `FFmpyg_DavidRodriguezSoaresCUI-0.0.1/pyproject.toml` & `FFmpyg_DavidRodriguezSoaresCUI-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "FFmpyg_DavidRodriguezSoaresCUI"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="DavidRodriguezSoaresCUI", email="fireblaze904+FFmpyg@gmail.com" },
 ]
 description = "A FFMPEG interface for Python by DavidRodriguezSoaresCUI"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `FFmpyg_DavidRodriguezSoaresCUI-0.0.1/src/FFmpyg/command.py` & `FFmpyg_DavidRodriguezSoaresCUI-0.0.2/src/FFmpyg/command.py`

 * *Files identical despite different names*

### Comparing `FFmpyg_DavidRodriguezSoaresCUI-0.0.1/src/FFmpyg/encoder_spec.py` & `FFmpyg_DavidRodriguezSoaresCUI-0.0.2/src/FFmpyg/encoder_spec.py`

 * *Files identical despite different names*

### Comparing `FFmpyg_DavidRodriguezSoaresCUI-0.0.1/src/FFmpyg/enums.py` & `FFmpyg_DavidRodriguezSoaresCUI-0.0.2/src/FFmpyg/enums.py`

 * *Files identical despite different names*

### Comparing `FFmpyg_DavidRodriguezSoaresCUI-0.0.1/src/FFmpyg/ffile.py` & `FFmpyg_DavidRodriguezSoaresCUI-0.0.2/src/FFmpyg/ffile.py`

 * *Files identical despite different names*

### Comparing `FFmpyg_DavidRodriguezSoaresCUI-0.0.1/src/FFmpyg/ffmpeg_command.py` & `FFmpyg_DavidRodriguezSoaresCUI-0.0.2/src/FFmpyg/ffmpeg_command.py`

 * *Files identical despite different names*

### Comparing `FFmpyg_DavidRodriguezSoaresCUI-0.0.1/src/FFmpyg/ffmpeg_encoder.py` & `FFmpyg_DavidRodriguezSoaresCUI-0.0.2/src/FFmpyg/ffmpeg_encoder.py`

 * *Files identical despite different names*

### Comparing `FFmpyg_DavidRodriguezSoaresCUI-0.0.1/src/FFmpyg/ffprobe.py` & `FFmpyg_DavidRodriguezSoaresCUI-0.0.2/src/FFmpyg/ffprobe.py`

 * *Files identical despite different names*

### Comparing `FFmpyg_DavidRodriguezSoaresCUI-0.0.1/src/FFmpyg/stream.py` & `FFmpyg_DavidRodriguezSoaresCUI-0.0.2/src/FFmpyg/stream.py`

 * *Files identical despite different names*

### Comparing `FFmpyg_DavidRodriguezSoaresCUI-0.0.1/src/FFmpyg/utils.py` & `FFmpyg_DavidRodriguezSoaresCUI-0.0.2/src/FFmpyg/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import ast
 import random
 import string
 from typing import Any, Callable, Iterable, List, Optional, Set, Union
 
 
 DOUBLE_QUOTE = '"'
+LOG_FORMAT = "[%(levelname)s:%(funcName)s] %(message)s"
 
 
 def ensureQuoted(s: str) -> str:
     """Ensures a string containing spaces is fully enclosed
     between double quotes
     """
     if " " not in s:
```

### Comparing `FFmpyg_DavidRodriguezSoaresCUI-0.0.1/src/FFmpyg_DavidRodriguezSoaresCUI.egg-info/PKG-INFO` & `FFmpyg_DavidRodriguezSoaresCUI-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: FFmpyg-DavidRodriguezSoaresCUI
-Version: 0.0.1
+Name: FFmpyg_DavidRodriguezSoaresCUI
+Version: 0.0.2
 Summary: A FFMPEG interface for Python by DavidRodriguezSoaresCUI
 Author-email: DavidRodriguezSoaresCUI <fireblaze904+FFmpyg@gmail.com>
 License: CC0 1.0 Universal
         
         Statement of Purpose
         
         The laws of most jurisdictions throughout the world automatically confer exclusive Copyright and Related Rights (defined below) upon the creator and subsequent owner(s) (each and all, an "owner") of an original work of authorship and/or a database (each, a "Work").
```

### Comparing `FFmpyg_DavidRodriguezSoaresCUI-0.0.1/src/FFmpyg_DavidRodriguezSoaresCUI.egg-info/SOURCES.txt` & `FFmpyg_DavidRodriguezSoaresCUI-0.0.2/src/FFmpyg_DavidRodriguezSoaresCUI.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 src/FFmpyg/command.py
 src/FFmpyg/encoder_spec.py
 src/FFmpyg/enums.py
 src/FFmpyg/exceptions.py
 src/FFmpyg/ffile.py
 src/FFmpyg/ffmpeg_command.py
 src/FFmpyg/ffmpeg_encoder.py
+src/FFmpyg/ffmpeg_lib.py
 src/FFmpyg/ffprobe.py
 src/FFmpyg/stream.py
 src/FFmpyg/utils.py
 src/FFmpyg_DavidRodriguezSoaresCUI.egg-info/PKG-INFO
 src/FFmpyg_DavidRodriguezSoaresCUI.egg-info/SOURCES.txt
 src/FFmpyg_DavidRodriguezSoaresCUI.egg-info/dependency_links.txt
 src/FFmpyg_DavidRodriguezSoaresCUI.egg-info/top_level.txt
```

