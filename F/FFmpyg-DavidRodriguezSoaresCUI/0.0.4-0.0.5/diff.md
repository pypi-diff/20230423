# Comparing `tmp/FFmpyg_DavidRodriguezSoaresCUI-0.0.4.tar.gz` & `tmp/FFmpyg_DavidRodriguezSoaresCUI-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FFmpyg_DavidRodriguezSoaresCUI-0.0.4.tar", last modified: Sun Apr 23 15:34:30 2023, max compression
+gzip compressed data, was "FFmpyg_DavidRodriguezSoaresCUI-0.0.5.tar", last modified: Sun Apr 23 16:14:54 2023, max compression
```

## Comparing `FFmpyg_DavidRodriguezSoaresCUI-0.0.4.tar` & `FFmpyg_DavidRodriguezSoaresCUI-0.0.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 15:34:30.096455 FFmpyg_DavidRodriguezSoaresCUI-0.0.4/
--rw-rw-rw-   0        0        0     6432 2023-04-10 17:40:33.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     9720 2023-04-23 15:34:30.096455 FFmpyg_DavidRodriguezSoaresCUI-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2353 2023-04-16 19:08:19.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.4/README.md
--rw-rw-rw-   0        0        0      814 2023-04-23 15:33:18.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-23 15:34:30.096455 FFmpyg_DavidRodriguezSoaresCUI-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-23 15:34:30.074437 FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-04-23 15:34:30.086448 FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg/
--rw-rw-rw-   0        0        0        0 2023-04-16 17:50:35.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg/__init__.py
--rw-rw-rw-   0        0        0     2042 2023-04-23 11:58:31.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg/command.py
--rw-rw-rw-   0        0        0     7167 2023-04-23 13:37:36.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg/encoder_spec.py
--rw-rw-rw-   0        0        0     1218 2023-04-15 16:47:24.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg/enums.py
--rw-rw-rw-   0        0        0      296 2023-04-23 11:44:20.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg/exceptions.py
--rw-rw-rw-   0        0        0     3065 2023-04-16 17:49:59.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg/ffile.py
--rw-rw-rw-   0        0        0    12453 2023-04-23 13:34:51.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg/ffmpeg_command.py
--rw-rw-rw-   0        0        0     7606 2023-04-23 11:56:01.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg/ffmpeg_encoder.py
--rw-rw-rw-   0        0        0     1829 2023-04-23 12:35:50.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg/ffmpeg_lib.py
--rw-rw-rw-   0        0        0    12018 2023-04-23 15:28:26.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg/ffmpeg_vmaf.py
--rw-rw-rw-   0        0        0      987 2023-04-16 17:49:28.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg/ffprobe.py
--rw-rw-rw-   0        0        0     5152 2023-04-16 17:49:21.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg/stream.py
--rw-rw-rw-   0        0        0     5690 2023-04-23 11:32:06.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg/utils.py
--rw-rw-rw-   0        0        0     7432 2023-04-23 13:38:43.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg/virtualfs.py
-drwxrwxrwx   0        0        0        0 2023-04-23 15:34:30.095456 FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg_DavidRodriguezSoaresCUI.egg-info/
--rw-rw-rw-   0        0        0     9720 2023-04-23 15:34:30.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg_DavidRodriguezSoaresCUI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      597 2023-04-23 15:34:30.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg_DavidRodriguezSoaresCUI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 15:34:30.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg_DavidRodriguezSoaresCUI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-23 15:34:30.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg_DavidRodriguezSoaresCUI.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 16:14:54.965484 FFmpyg_DavidRodriguezSoaresCUI-0.0.5/
+-rw-rw-rw-   0        0        0     6432 2023-04-10 17:40:33.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     9720 2023-04-23 16:14:54.965484 FFmpyg_DavidRodriguezSoaresCUI-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2353 2023-04-16 19:08:19.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.5/README.md
+-rw-rw-rw-   0        0        0      814 2023-04-23 16:11:13.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-23 16:14:54.966486 FFmpyg_DavidRodriguezSoaresCUI-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-23 16:14:54.944466 FFmpyg_DavidRodriguezSoaresCUI-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-04-23 16:14:54.956477 FFmpyg_DavidRodriguezSoaresCUI-0.0.5/src/FFmpyg/
+-rw-rw-rw-   0        0        0        0 2023-04-16 17:50:35.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.5/src/FFmpyg/__init__.py
+-rw-rw-rw-   0        0        0     2069 2023-04-23 16:10:08.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.5/src/FFmpyg/command.py
+-rw-rw-rw-   0        0        0     7175 2023-04-23 16:09:55.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.5/src/FFmpyg/encoder_spec.py
+-rw-rw-rw-   0        0        0     1218 2023-04-15 16:47:24.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.5/src/FFmpyg/enums.py
+-rw-rw-rw-   0        0        0      296 2023-04-23 11:44:20.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.5/src/FFmpyg/exceptions.py
+-rw-rw-rw-   0        0        0     3073 2023-04-23 16:10:18.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.5/src/FFmpyg/ffile.py
+-rw-rw-rw-   0        0        0    12480 2023-04-23 16:10:26.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.5/src/FFmpyg/ffmpeg_command.py
+-rw-rw-rw-   0        0        0     7638 2023-04-23 16:08:14.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.5/src/FFmpyg/ffmpeg_encoder.py
+-rw-rw-rw-   0        0        0     1837 2023-04-23 16:10:49.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.5/src/FFmpyg/ffmpeg_lib.py
+-rw-rw-rw-   0        0        0    12024 2023-04-23 16:10:45.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.5/src/FFmpyg/ffmpeg_vmaf.py
+-rw-rw-rw-   0        0        0      987 2023-04-16 17:49:28.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.5/src/FFmpyg/ffprobe.py
+-rw-rw-rw-   0        0        0     5188 2023-04-23 16:09:25.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.5/src/FFmpyg/stream.py
+-rw-rw-rw-   0        0        0     1177 2023-04-23 16:09:37.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.5/src/FFmpyg/utils.py
+-rw-rw-rw-   0        0        0     7436 2023-04-23 16:11:01.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.5/src/FFmpyg/virtualfs.py
+drwxrwxrwx   0        0        0        0 2023-04-23 16:14:54.964484 FFmpyg_DavidRodriguezSoaresCUI-0.0.5/src/FFmpyg_DavidRodriguezSoaresCUI.egg-info/
+-rw-rw-rw-   0        0        0     9720 2023-04-23 16:14:54.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.5/src/FFmpyg_DavidRodriguezSoaresCUI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      597 2023-04-23 16:14:54.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.5/src/FFmpyg_DavidRodriguezSoaresCUI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 16:14:54.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.5/src/FFmpyg_DavidRodriguezSoaresCUI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-23 16:14:54.000000 FFmpyg_DavidRodriguezSoaresCUI-0.0.5/src/FFmpyg_DavidRodriguezSoaresCUI.egg-info/top_level.txt
```

### Comparing `FFmpyg_DavidRodriguezSoaresCUI-0.0.4/LICENSE` & `FFmpyg_DavidRodriguezSoaresCUI-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `FFmpyg_DavidRodriguezSoaresCUI-0.0.4/PKG-INFO` & `FFmpyg_DavidRodriguezSoaresCUI-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FFmpyg_DavidRodriguezSoaresCUI
-Version: 0.0.4
+Version: 0.0.5
 Summary: A FFMPEG interface for Python by DavidRodriguezSoaresCUI
 Author-email: DavidRodriguezSoaresCUI <fireblaze904+FFmpyg@gmail.com>
 License: CC0 1.0 Universal
         
         Statement of Purpose
         
         The laws of most jurisdictions throughout the world automatically confer exclusive Copyright and Related Rights (defined below) upon the creator and subsequent owner(s) (each and all, an "owner") of an original work of authorship and/or a database (each, a "Work").
```

### Comparing `FFmpyg_DavidRodriguezSoaresCUI-0.0.4/README.md` & `FFmpyg_DavidRodriguezSoaresCUI-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `FFmpyg_DavidRodriguezSoaresCUI-0.0.4/pyproject.toml` & `FFmpyg_DavidRodriguezSoaresCUI-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "FFmpyg_DavidRodriguezSoaresCUI"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="DavidRodriguezSoaresCUI", email="fireblaze904+FFmpyg@gmail.com" },
 ]
 description = "A FFMPEG interface for Python by DavidRodriguezSoaresCUI"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg/command.py` & `FFmpyg_DavidRodriguezSoaresCUI-0.0.5/src/FFmpyg/command.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """ Contains class Command, used to execute external programs
 """
 import logging
 from os import PathLike
 from subprocess import PIPE, Popen
 from typing import Any, Dict, List
 
-from .utils import ensureQuoted, assertTrue
+from DRSlib.utils import assertTrue
+
+from .utils import ensureQuoted
 
 
 LOG = logging.getLogger(__file__)
 
 
 class Command:
     """Represents a shell command as a list of parts, and
```

### Comparing `FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg/encoder_spec.py` & `FFmpyg_DavidRodriguezSoaresCUI-0.0.5/src/FFmpyg/encoder_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,17 +13,18 @@
 """
 
 import re
 from collections import defaultdict
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Union
 
+from DRSlib.utils import assertTrue
+
 from .command import Command
 from .enums import StreamType
-from .utils import assertTrue
 
 ENCODER_LINE = re.compile(r"\s+([AVS])[ADEILSV\.]{5} (\S+).*")
 ENCODER_GENERAL_CAPABILITIES = re.compile(r"General capabilities: (.*)")
 FFMPEG_CODEC = re.compile(r"\s*[ADEILSV\.]{6} (\S+).*")
 FFMPEG_DESCRIPTION_VALUE_DEFAULT = re.compile(r"\(default (.+?)\)")
 FFMPEG_DESCRIPTION_VALUE_RANGE = re.compile(r"\(from (.+?) to (.+?)\)")
 FFMPEG_FLAGS = re.compile(r"[ADEILSV\.]{10}")
```

### Comparing `FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg/enums.py` & `FFmpyg_DavidRodriguezSoaresCUI-0.0.5/src/FFmpyg/enums.py`

 * *Files identical despite different names*

### Comparing `FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg/ffile.py` & `FFmpyg_DavidRodriguezSoaresCUI-0.0.5/src/FFmpyg/ffile.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,18 +5,19 @@
 """
 
 
 from collections import namedtuple
 from pathlib import Path
 from typing import List
 
+from DRSlib.utils import assertTrue
+
 from .enums import FfprobeInfoKey, StreamType
 from .ffprobe import file_stream_info
 from .stream import FutureStream, Stream
-from .utils import assertTrue
 
 StreamCriteria = namedtuple("StreamCriteria", "codec_type codec")
 
 
 class MediaFile:
     """FFMPEG-focused media file representation; views a media file as a
     container for streams."""
```

### Comparing `FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg/ffmpeg_command.py` & `FFmpyg_DavidRodriguezSoaresCUI-0.0.5/src/FFmpyg/ffmpeg_command.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,27 +3,29 @@
 encoders and more
 """
 import logging
 import sys
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Set, Tuple, Union
 
+from DRSlib.utils import assertTrue
+
 from .command import Command
 from .exceptions import FilterComputationFailed
 from .ffile import (
     FfprobeInfoKey,
     FutureMediaFile,
     FutureStream,
     MediaFile,
     Stream,
     StreamCriteria,
     StreamType,
 )
 from .ffmpeg_encoder import Encoder
-from .utils import assertTrue, random_words
+from .utils import random_words
 
 LOG = logging.getLogger(__file__)
 
 
 class FfmpegOptions:
     """Represents FFMPEG global options"""
```

### Comparing `FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg/ffmpeg_encoder.py` & `FFmpyg_DavidRodriguezSoaresCUI-0.0.5/src/FFmpyg/ffmpeg_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """Defines FFMPEG-compliant encoder abstraction and manipulation facilities
 """
 import logging
-from pathlib import Path
 import re
+from pathlib import Path
 
 # import re
 from typing import Any, Callable, Dict, List, Optional, Union
 
 import yaml
+from DRSlib.cli_ui import choose_from_list, user_input
+from DRSlib.utils import assertTrue
 
 from .encoder_spec import (
     ffmpeg_supported_encoders,
     get_codec_from_encoder,
     read_encoder_parameters,
 )
-from .utils import assertTrue, user_input, choose_from_list
 from .enums import StreamType
 
 LOG = logging.getLogger(__file__)
 AVAILABLE_ENCODERS: Dict[Union[str, Path], List[str]] = {}
 
 
 def is_available_encoder(encoder: str, ffmpeg: Union[str, Path]) -> bool:
```

### Comparing `FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg/ffmpeg_lib.py` & `FFmpyg_DavidRodriguezSoaresCUI-0.0.5/src/FFmpyg/ffmpeg_lib.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 Some convenient methods to retrieve simple info about FFmpeg
 """
 import logging
 import re
 from pathlib import Path
 from typing import Dict, List, Union
 
+from DRSlib.utils import assertTrue
+
 from .command import Command
-from .utils import assertTrue
 
 FFMPEG_VERSION = re.compile(r"ffmpeg version (\S+) Copyright \(c\) \d{4}\-(\d{4})")
 FFMPEG_FEATURE = re.compile(r"--enable-(\S+)")
 LOG = logging.getLogger(__file__)
 
 
 def get_ffmpeg_info(ffmpeg: Union[str, Path]) -> Dict[str, Union[List[str], str]]:
```

### Comparing `FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg/ffmpeg_vmaf.py` & `FFmpyg_DavidRodriguezSoaresCUI-0.0.5/src/FFmpyg/ffmpeg_vmaf.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,26 +10,26 @@
 import logging
 import math
 from pathlib import Path
 from typing import Dict, List, Union
 
 import numpy as np
 from DRSlib.hash import get_temporary_dir_name
+from DRSlib.utils import assertTrue
 from matplotlib import pyplot as plt
 
 from .enums import FfprobeInfoKey, StreamType
 from .ffile import MediaFile, StreamCriteria
 from .ffmpeg_command import (
     FfmpegInput,
     FfmpegOptions,
     FilterComplexNode,
     build_ffmpeg_command,
 )
 from .ffmpeg_lib import assert_ffmpeg_supports_feature
-from .utils import assertTrue
 from .virtualfs import WorkingDirectory
 
 LOG = logging.getLogger(__file__)
 FFMPEG_FEATURE_VMAF = "libvmaf"
 
 
 def assert_ffmpeg_supports_vmaf(ffmpeg: Union[str, Path]) -> None:
```

### Comparing `FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg/ffprobe.py` & `FFmpyg_DavidRodriguezSoaresCUI-0.0.5/src/FFmpyg/ffprobe.py`

 * *Files identical despite different names*

### Comparing `FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg/stream.py` & `FFmpyg_DavidRodriguezSoaresCUI-0.0.5/src/FFmpyg/stream.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """ Streams are the elementary components of a media file
 """
 from typing import Any, Optional, Union
 
-from .ffmpeg_encoder import Encoder
-from .enums import FfprobeInfoKey, StreamType
-from .utils import assertTrue, dict_difference, flatten_dict_join
+from DRSlib.dict_utils import dict_difference, flatten_dict_join
+from DRSlib.utils import assertTrue
 
+from .enums import FfprobeInfoKey, StreamType
+from .ffmpeg_encoder import Encoder
 
 StreamKeyType = Union[FfprobeInfoKey, StreamType, str]
 
 
 class Stream:
     """Multimedia stream"""
```

### Comparing `FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg/virtualfs.py` & `FFmpyg_DavidRodriguezSoaresCUI-0.0.5/src/FFmpyg/virtualfs.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 """
 import json
 import uuid
 from pathlib import Path
 from typing import Generator, List, Optional, Union
 
 from DRSlib.hash import get_temporary_dir_name
-
-from .utils import assertTrue
+from DRSlib.utils import assertTrue
 
 
 class Node:
     """Data structure used to implement tree. It's serializable and has search functionnality"""
 
     def __init__(
         self,
```

### Comparing `FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg_DavidRodriguezSoaresCUI.egg-info/PKG-INFO` & `FFmpyg_DavidRodriguezSoaresCUI-0.0.5/src/FFmpyg_DavidRodriguezSoaresCUI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FFmpyg-DavidRodriguezSoaresCUI
-Version: 0.0.4
+Version: 0.0.5
 Summary: A FFMPEG interface for Python by DavidRodriguezSoaresCUI
 Author-email: DavidRodriguezSoaresCUI <fireblaze904+FFmpyg@gmail.com>
 License: CC0 1.0 Universal
         
         Statement of Purpose
         
         The laws of most jurisdictions throughout the world automatically confer exclusive Copyright and Related Rights (defined below) upon the creator and subsequent owner(s) (each and all, an "owner") of an original work of authorship and/or a database (each, a "Work").
```

### Comparing `FFmpyg_DavidRodriguezSoaresCUI-0.0.4/src/FFmpyg_DavidRodriguezSoaresCUI.egg-info/SOURCES.txt` & `FFmpyg_DavidRodriguezSoaresCUI-0.0.5/src/FFmpyg_DavidRodriguezSoaresCUI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

