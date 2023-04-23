# Comparing `tmp/mextractor-2.2.0.tar.gz` & `tmp/mextractor-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mextractor-2.2.0.tar", max compression
+gzip compressed data, was "mextractor-3.0.0.tar", max compression
```

## Comparing `mextractor-2.2.0.tar` & `mextractor-3.0.0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1620 2022-10-25 18:57:56.194390 mextractor-2.2.0/README.md
--rw-r--r--   0        0        0       23 2022-10-25 18:57:56.194390 mextractor-2.2.0/mextractor/__init__.py
--rw-r--r--   0        0        0     2461 2022-10-25 19:12:07.280891 mextractor-2.2.0/mextractor/base.py
--rw-r--r--   0        0        0      794 2022-10-25 19:18:51.462023 mextractor-2.2.0/mextractor/cli.py
--rw-r--r--   0        0        0       67 2022-10-25 18:57:56.195390 mextractor-2.2.0/mextractor/constants.py
--rw-r--r--   0        0        0     2635 2022-10-25 19:07:41.155223 mextractor-2.2.0/mextractor/extractors.py
--rw-r--r--   0        0        0      518 2022-10-25 19:10:42.510421 mextractor-2.2.0/mextractor/utils.py
--rw-r--r--   0        0        0     2351 2022-10-25 19:18:11.282528 mextractor-2.2.0/mextractor/workflow.py
--rw-r--r--   0        0        0     1351 2022-10-25 19:20:25.377890 mextractor-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     2898 1970-01-01 00:00:00.000000 mextractor-2.2.0/setup.py
--rw-r--r--   0        0        0     3045 1970-01-01 00:00:00.000000 mextractor-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1620 2023-04-23 14:38:11.432613 mextractor-3.0.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-23 14:47:49.396153 mextractor-3.0.0/mextractor/__init__.py
+-rw-r--r--   0        0        0     2461 2023-04-23 14:47:43.177188 mextractor-3.0.0/mextractor/base.py
+-rw-r--r--   0        0        0      788 2023-04-23 14:48:01.751085 mextractor-3.0.0/mextractor/cli.py
+-rw-r--r--   0        0        0       67 2023-04-23 14:38:11.432613 mextractor-3.0.0/mextractor/constants.py
+-rw-r--r--   0        0        0     2545 2023-04-23 14:47:29.104265 mextractor-3.0.0/mextractor/extractors.py
+-rw-r--r--   0        0        0      518 2023-04-23 14:38:11.432613 mextractor-3.0.0/mextractor/utils.py
+-rw-r--r--   0        0        0     2351 2023-04-23 14:47:43.185188 mextractor-3.0.0/mextractor/workflow.py
+-rw-r--r--   0        0        0     1247 2023-04-23 14:47:40.535202 mextractor-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2787 1970-01-01 00:00:00.000000 mextractor-3.0.0/PKG-INFO
```

### Comparing `mextractor-2.2.0/README.md` & `mextractor-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `mextractor-2.2.0/mextractor/base.py` & `mextractor-3.0.0/mextractor/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import shutil
 from functools import cached_property
 from typing import Optional
 
 import cv2
-from pydantic import DirectoryPath, BaseModel, FilePath
+from pydantic import BaseModel, DirectoryPath, FilePath
 from pydantic_numpy import NDArrayUint8
 from ruamel.yaml import YAML
 
 from mextractor.constants import DUMP_PATH_SUFFIX
 from mextractor.utils import dump_image
 
 logger = logging.getLogger()
```

### Comparing `mextractor-2.2.0/mextractor/cli.py` & `mextractor-3.0.0/mextractor/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,17 +14,14 @@
 
 @mextractor_cli.command()
 @click.argument("root_dir", required=True, type=str)
 @click.option(
     "-s",
     "--suffix",
     "video_file_suffix",
-    help=f"Suffix of the video files in the sub directories, leaving undefined will fallback to all video suffixes {VIDEO_SUFFIXES}",
+    help=f"Suffix of the video files in the sub directories, leaving undefined will "
+    f"fallback to all video suffixes {VIDEO_SUFFIXES}",
     type=str,
 )
-@click.option(
-    "-f",
-    "--only-frame",
-    is_flag=True
-)
+@click.option("-f", "--only-frame", is_flag=True)
 def video_subdirs(root_dir: DirectoryPath, video_file_suffix: Optional[str] = None, only_frame: bool = False) -> None:
     mextract_videos_in_subdirs(root_dir, video_file_suffix, only_frame=only_frame)
```

### Comparing `mextractor-2.2.0/mextractor/extractors.py` & `mextractor-3.0.0/mextractor/extractors.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,12 +68,10 @@
         average_fps = int(numerator) / int(denominator)
     else:
         average_fps = float(ffmpeg_metadata["avg_frame_rate"])
 
     return MextractorMetadata(
         name=path_to_video.stem,
         resolution=(ffmpeg_metadata["width"], ffmpeg_metadata["height"]),
-        frames=ffmpeg_metadata["nb_frames"],
         average_fps=average_fps,
-        seconds=ffmpeg_metadata["duration"],
         image=extract_video_frame(path_to_video, frame_to_extract_time) if include_image else None,
     )
```

### Comparing `mextractor-2.2.0/mextractor/utils.py` & `mextractor-3.0.0/mextractor/utils.py`

 * *Files identical despite different names*

### Comparing `mextractor-2.2.0/mextractor/workflow.py` & `mextractor-3.0.0/mextractor/workflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import shutil
 from concurrent.futures import ThreadPoolExecutor
 from shutil import rmtree
 from typing import Optional
 
-from pydantic import FilePath, DirectoryPath, validate_arguments
+from pydantic import DirectoryPath, FilePath, validate_arguments
 
 from mextractor.base import MextractorMetadata
 from mextractor.constants import VIDEO_SUFFIXES
 from mextractor.extractors import extract_image, extract_video, extract_video_frame
 from mextractor.utils import dump_image
```

### Comparing `mextractor-2.2.0/pyproject.toml` & `mextractor-3.0.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,35 @@
 [tool.poetry]
 name = "mextractor"
-version = "2.2.0"
+version = "3.0.0"
 description = "mextractor can extract media metadata to YAML and read them"
 readme = "README.md"
 repository = "https://github.com/caniko/media-metadata-extractor"
 homepage = "https://pypi.org/project/mextractor/"
 authors = ["Can H. Tartanoglu <canhtart@gmail.com>"]
 license = "Apache-2.0"
 keywords = ["pydantic", "metadata", "video", "image", "bigdata"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.7, <3.11"
-setuptools = "*"
+python = ">=3.9, <3.12"
 
-numpy = [
-    {version = "*", python = ">=3.8, <3.11"},
-    {version = "^1.21.0", python = "~3.7"}
-]
+numpy = "*"
 
 pydantic = "^1.9.2"
-pydantic-numpy = "^1.3.0"
+pydantic-numpy = "^2.2.1"
 
 "ruamel.yaml" = "^0.17.21"
 opencv-python = "^4.6.0"
 
 ffmpeg-python = {version = "^0.2.0", optional = true}
 
-numba = {version = "^0.56.0", optional = true}
 click = "^8.1.3"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 
 [tool.poetry.extras]
 video-extract = ["ffmpeg-python"]
@@ -44,15 +39,19 @@
 
 [tool.mypy]
 python_version = "3.10"
 plugins = "numpy.typing.mypy_plugin"
 
 [tool.isort]
 profile = "black"
+line_length = 120
 
 [tool.black]
 line-length = 120
 target-version = ["py310"]
 
+[tool.ruff]
+line-length = 120
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `mextractor-2.2.0/PKG-INFO` & `mextractor-3.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 Metadata-Version: 2.1
 Name: mextractor
-Version: 2.2.0
+Version: 3.0.0
 Summary: mextractor can extract media metadata to YAML and read them
 Home-page: https://pypi.org/project/mextractor/
 License: Apache-2.0
 Keywords: pydantic,metadata,video,image,bigdata
 Author: Can H. Tartanoglu
 Author-email: canhtart@gmail.com
-Requires-Python: >=3.7,<3.11
+Requires-Python: >=3.9,<3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: video-extract
 Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: ffmpeg-python (>=0.2.0,<0.3.0); extra == "video-extract"
-Requires-Dist: numba (>=0.56.0,<0.57.0)
-Requires-Dist: numpy (>=1.21.0,<2.0.0); python_version >= "3.7" and python_version < "3.8"
-Requires-Dist: numpy; python_version >= "3.8" and python_version < "3.11"
+Requires-Dist: ffmpeg-python (>=0.2.0,<0.3.0) ; extra == "video-extract"
+Requires-Dist: numpy
 Requires-Dist: opencv-python (>=4.6.0,<5.0.0)
 Requires-Dist: pydantic (>=1.9.2,<2.0.0)
-Requires-Dist: pydantic-numpy (>=1.3.0,<2.0.0)
+Requires-Dist: pydantic-numpy (>=2.2.1,<3.0.0)
 Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0)
-Requires-Dist: setuptools
 Project-URL: Repository, https://github.com/caniko/media-metadata-extractor
 Description-Content-Type: text/markdown
 
 # mextractor: media metadata extractor
 
 Videos and images can be large.
```

