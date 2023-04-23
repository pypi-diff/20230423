# Comparing `tmp/codewithgpu-0.2.0-py3-none-any.whl.zip` & `tmp/codewithgpu-0.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,31 @@
-Zip file size: 28291 bytes, number of entries: 22
--rw-r--r--  2.0 unx     1519 b- defN 22-Sep-17 08:06 codewithgpu/__init__.py
--rw-r--r--  2.0 unx      149 b- defN 23-Feb-16 08:28 codewithgpu/version.py
--rw-r--r--  2.0 unx      746 b- defN 22-Sep-14 16:45 codewithgpu/data/__init__.py
--rw-r--r--  2.0 unx     6332 b- defN 22-Sep-17 08:59 codewithgpu/data/dataset.py
--rw-r--r--  2.0 unx     7059 b- defN 22-Sep-14 16:45 codewithgpu/data/reader.py
--rw-r--r--  2.0 unx      608 b- defN 22-Sep-14 16:45 codewithgpu/data/record.proto
--rw-r--r--  2.0 unx     8793 b- defN 22-Sep-17 11:37 codewithgpu/data/record.py
--rw-r--r--  2.0 unx    10202 b- defN 22-Sep-17 09:20 codewithgpu/data/record_pb2.py
--rw-r--r--  2.0 unx      780 b- defN 22-Sep-17 06:35 codewithgpu/data/tf_record.proto
--rw-r--r--  2.0 unx     7024 b- defN 22-Sep-17 11:37 codewithgpu/data/tf_record.py
--rw-r--r--  2.0 unx    11900 b- defN 22-Sep-17 09:20 codewithgpu/data/tf_record_pb2.py
--rw-r--r--  2.0 unx      746 b- defN 22-Sep-14 16:45 codewithgpu/inference/__init__.py
--rw-r--r--  2.0 unx     5969 b- defN 22-Sep-14 16:45 codewithgpu/inference/command.py
--rw-r--r--  2.0 unx     1474 b- defN 22-Sep-14 16:45 codewithgpu/inference/module.py
--rw-r--r--  2.0 unx      746 b- defN 22-Sep-14 16:45 codewithgpu/utils/__init__.py
--rw-r--r--  2.0 unx     3741 b- defN 22-Sep-14 16:45 codewithgpu/utils/logging.py
--rw-r--r--  2.0 unx     1226 b- defN 22-Sep-14 16:45 codewithgpu/utils/unittest_util.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Feb-16 08:28 codewithgpu-0.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     3083 b- defN 23-Feb-16 08:28 codewithgpu-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-16 08:28 codewithgpu-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       69 b- defN 23-Feb-16 08:28 codewithgpu-0.2.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1864 b- defN 23-Feb-16 08:28 codewithgpu-0.2.0.dist-info/RECORD
-22 files, 85479 bytes uncompressed, 25255 bytes compressed:  70.5%
+Zip file size: 35539 bytes, number of entries: 29
+-rw-r--r--  2.0 unx     1519 b- defN 23-Apr-23 11:05 codewithgpu/__init__.py
+-rw-r--r--  2.0 unx     1924 b- defN 23-Apr-23 11:05 codewithgpu/cli.py
+-rw-r--r--  2.0 unx      185 b- defN 23-Apr-23 11:36 codewithgpu/version.py
+-rw-r--r--  2.0 unx      746 b- defN 23-Apr-23 11:05 codewithgpu/data/__init__.py
+-rw-r--r--  2.0 unx     6547 b- defN 23-Apr-23 11:05 codewithgpu/data/dataset.py
+-rw-r--r--  2.0 unx     7177 b- defN 23-Apr-23 11:05 codewithgpu/data/reader.py
+-rw-r--r--  2.0 unx      608 b- defN 23-Apr-23 11:05 codewithgpu/data/record.proto
+-rw-r--r--  2.0 unx     8941 b- defN 23-Apr-23 11:05 codewithgpu/data/record.py
+-rw-r--r--  2.0 unx    10202 b- defN 23-Apr-23 11:05 codewithgpu/data/record_pb2.py
+-rw-r--r--  2.0 unx      780 b- defN 23-Apr-23 11:05 codewithgpu/data/tf_record.proto
+-rw-r--r--  2.0 unx     7299 b- defN 23-Apr-23 11:05 codewithgpu/data/tf_record.py
+-rw-r--r--  2.0 unx    11900 b- defN 23-Apr-23 11:05 codewithgpu/data/tf_record_pb2.py
+-rw-r--r--  2.0 unx      746 b- defN 23-Apr-23 11:05 codewithgpu/inference/__init__.py
+-rw-r--r--  2.0 unx     6128 b- defN 23-Apr-23 11:05 codewithgpu/inference/command.py
+-rw-r--r--  2.0 unx     1474 b- defN 23-Apr-23 11:05 codewithgpu/inference/module.py
+-rw-r--r--  2.0 unx      761 b- defN 23-Apr-23 11:05 codewithgpu/model/__init__.py
+-rw-r--r--  2.0 unx     1418 b- defN 23-Apr-23 11:05 codewithgpu/model/download.py
+-rw-r--r--  2.0 unx      746 b- defN 23-Apr-23 11:05 codewithgpu/utils/__init__.py
+-rw-r--r--  2.0 unx     4076 b- defN 23-Apr-23 11:05 codewithgpu/utils/cg_cli.py
+-rw-r--r--  2.0 unx     3805 b- defN 23-Apr-23 11:05 codewithgpu/utils/decorator.py
+-rw-r--r--  2.0 unx     3629 b- defN 23-Apr-23 11:05 codewithgpu/utils/deprecation.py
+-rw-r--r--  2.0 unx     3741 b- defN 23-Apr-21 09:27 codewithgpu/utils/logging.py
+-rw-r--r--  2.0 unx     1226 b- defN 23-Apr-21 09:27 codewithgpu/utils/unittest_util.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Apr-23 11:36 codewithgpu-0.2.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3033 b- defN 23-Apr-23 11:36 codewithgpu-0.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-23 11:36 codewithgpu-0.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       49 b- defN 23-Apr-23 11:36 codewithgpu-0.2.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       87 b- defN 23-Apr-23 11:36 codewithgpu-0.2.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     2469 b- defN 23-Apr-23 11:36 codewithgpu-0.2.1.dist-info/RECORD
+29 files, 102665 bytes uncompressed, 31553 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -1,10 +1,13 @@
 Filename: codewithgpu/__init__.py
 Comment: 
 
+Filename: codewithgpu/cli.py
+Comment: 
+
 Filename: codewithgpu/version.py
 Comment: 
 
 Filename: codewithgpu/data/__init__.py
 Comment: 
 
 Filename: codewithgpu/data/dataset.py
@@ -36,32 +39,50 @@
 
 Filename: codewithgpu/inference/command.py
 Comment: 
 
 Filename: codewithgpu/inference/module.py
 Comment: 
 
+Filename: codewithgpu/model/__init__.py
+Comment: 
+
+Filename: codewithgpu/model/download.py
+Comment: 
+
 Filename: codewithgpu/utils/__init__.py
 Comment: 
 
+Filename: codewithgpu/utils/cg_cli.py
+Comment: 
+
+Filename: codewithgpu/utils/decorator.py
+Comment: 
+
+Filename: codewithgpu/utils/deprecation.py
+Comment: 
+
 Filename: codewithgpu/utils/logging.py
 Comment: 
 
 Filename: codewithgpu/utils/unittest_util.py
 Comment: 
 
-Filename: codewithgpu-0.2.0.dist-info/LICENSE
+Filename: codewithgpu-0.2.1.dist-info/LICENSE
+Comment: 
+
+Filename: codewithgpu-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: codewithgpu-0.2.0.dist-info/METADATA
+Filename: codewithgpu-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: codewithgpu-0.2.0.dist-info/WHEEL
+Filename: codewithgpu-0.2.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: codewithgpu-0.2.0.dist-info/top_level.txt
+Filename: codewithgpu-0.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: codewithgpu-0.2.0.dist-info/RECORD
+Filename: codewithgpu-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## codewithgpu/version.py

```diff
@@ -1,6 +1,6 @@
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
-version = '0.2.0'
-git_version = 'None'
+version = '0.2.1'
+git_version = '9ec37e2480a68e67e04cba90c5d6f7e0921f14ba'
```

## codewithgpu/data/dataset.py

```diff
@@ -19,16 +19,21 @@
 from __future__ import division
 from __future__ import print_function
 
 import json
 import os
 import struct
 
-from codewithgpu.data import record_pb2
-from codewithgpu.data import tf_record_pb2
+try:
+    from codewithgpu.data import record_pb2
+    from codewithgpu.data import tf_record_pb2
+except (ImportError, TypeError):
+    from codewithgpu.utils import deprecation
+    record_pb2 = deprecation.NotInstalled('protobuf<4.0.0')
+    tf_record_pb2 = deprecation.NotInstalled('protobuf<4.0.0')
 from codewithgpu.data.record import RecordDecoder
 from codewithgpu.data.tf_record import TFRecordDecoder
 
 
 class RecordDataset(object):
     """Dataset to load data from the record files."""
```

## codewithgpu/data/reader.py

```diff
@@ -17,15 +17,19 @@
 
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
 import multiprocessing
 
-import numpy as np
+try:
+    import numpy as np
+except ImportError:
+    from codewithgpu.utils import deprecation
+    np = deprecation.NotInstalled('numpy')
 
 from codewithgpu.data.dataset import RecordDataset
 
 
 class DatasetReader(multiprocessing.Process):
     """Read examples from a dataset.
```

## codewithgpu/data/record.py

```diff
@@ -18,15 +18,19 @@
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
 import json
 import os
 
-from codewithgpu.data import record_pb2
+try:
+    from codewithgpu.data import record_pb2
+except (ImportError, TypeError):
+    from codewithgpu.utils import deprecation
+    record_pb2 = deprecation.NotInstalled('protobuf<4.0.0')
 
 
 class FeatureType(object):
     """Record feature type."""
 
     BYTES = 'BYTES'
     STRING = 'STRING'
```

## codewithgpu/data/tf_record.py

```diff
@@ -18,17 +18,25 @@
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
 import struct
 import zlib
 
-import numpy
-
-from codewithgpu.data import tf_record_pb2
+try:
+    import numpy as np
+except ImportError:
+    from codewithgpu.utils import deprecation
+    np = deprecation.NotInstalled('numpy')
+
+try:
+    from codewithgpu.data import tf_record_pb2
+except (ImportError, TypeError):
+    from codewithgpu.utils import deprecation
+    tf_record_pb2 = deprecation.NotInstalled('protobuf<4.0.0')
 from codewithgpu.data.record import RecordWriter
 
 
 class FeatureType(object):
     """Record feature type."""
 
     BYTES = 'bytes'
```

## codewithgpu/inference/command.py

```diff
@@ -24,15 +24,18 @@
 import multiprocessing
 
 try:
     import cv2
     import flask
     import numpy as np
 except ImportError:
-    cv2 = flask = np = None
+    from codewithgpu.utils import deprecation
+    cv2 = deprecation.NotInstalled('opencv-python')
+    flask = deprecation.NotInstalled('flask')
+    np = deprecation.NotInstalled('numpy')
 
 from codewithgpu.inference.module import InferenceModule
 
 
 class ServingCommand(object):
     """Command to run serving."""
```

## Comparing `codewithgpu-0.2.0.dist-info/LICENSE` & `codewithgpu-0.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `codewithgpu-0.2.0.dist-info/METADATA` & `codewithgpu-0.2.1.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 636f 6465  : 2.1.Name: code
 00000020: 7769 7468 6770 750a 5665 7273 696f 6e3a  withgpu.Version:
-00000030: 2030 2e32 2e30 0a53 756d 6d61 7279 3a20   0.2.0.Summary: 
+00000030: 2030 2e32 2e31 0a53 756d 6d61 7279 3a20   0.2.1.Summary: 
 00000040: 436f 6465 5769 7468 4750 5520 5079 7468  CodeWithGPU Pyth
 00000050: 6f6e 2043 6c69 656e 740a 486f 6d65 2d70  on Client.Home-p
 00000060: 6167 653a 2068 7474 7073 3a2f 2f67 6974  age: https://git
 00000070: 6875 622e 636f 6d2f 7365 6574 6163 6c6f  hub.com/seetaclo
 00000080: 7564 2f63 6f64 6577 6974 6867 7075 0a41  ud/codewithgpu.A
 00000090: 7574 686f 723a 2053 6565 7461 436c 6f75  uthor: SeetaClou
 000000a0: 640a 4c69 6365 6e73 653a 2041 7061 6368  d.License: Apach
@@ -45,149 +45,146 @@
 000002c0: 6373 0a43 6c61 7373 6966 6965 723a 2054  cs.Classifier: T
 000002d0: 6f70 6963 203a 3a20 5363 6965 6e74 6966  opic :: Scientif
 000002e0: 6963 2f45 6e67 696e 6565 7269 6e67 203a  ic/Engineering :
 000002f0: 3a20 4172 7469 6669 6369 616c 2049 6e74  : Artificial Int
 00000300: 656c 6c69 6765 6e63 650a 4465 7363 7269  elligence.Descri
 00000310: 7074 696f 6e2d 436f 6e74 656e 742d 5479  ption-Content-Ty
 00000320: 7065 3a20 7465 7874 2f6d 6172 6b64 6f77  pe: text/markdow
-00000330: 6e0a 4c69 6365 6e73 652d 4669 6c65 3a20  n.License-File: 
-00000340: 4c49 4345 4e53 450a 5265 7175 6972 6573  LICENSE.Requires
-00000350: 2d44 6973 743a 206e 756d 7079 0a52 6571  -Dist: numpy.Req
-00000360: 7569 7265 732d 4469 7374 3a20 7072 6f74  uires-Dist: prot
-00000370: 6f62 7566 2028 3c3d 332e 3230 2e31 2c3e  obuf (<=3.20.1,>
-00000380: 3d33 2e39 2e31 290a 5265 7175 6972 6573  =3.9.1).Requires
-00000390: 2d44 6973 743a 206f 7065 6e63 762d 7079  -Dist: opencv-py
-000003a0: 7468 6f6e 0a52 6571 7569 7265 732d 4469  thon.Requires-Di
-000003b0: 7374 3a20 666c 6173 6b0a 5265 7175 6972  st: flask.Requir
-000003c0: 6573 2d44 6973 743a 2067 7261 6469 6f0a  es-Dist: gradio.
-000003d0: 0a23 2043 6f64 6557 6974 6847 5055 0a0a  .# CodeWithGPU..
-000003e0: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-000003f0: 2f2f 6472 6167 6f6e 2e73 6565 7461 7465  //dragon.seetate
-00000400: 6368 2e63 6f6d 2f64 6f77 6e6c 6f61 642f  ch.com/download/
-00000410: 636f 6465 7769 7468 6770 752f 6173 7365  codewithgpu/asse
-00000420: 7473 2f62 616e 6e65 722e 706e 6722 2f3e  ts/banner.png"/>
-00000430: 0a0a 5b43 6f64 6557 6974 6847 5055 5d28  ..[CodeWithGPU](
-00000440: 6874 7470 733a 2f2f 7777 772e 636f 6465  https://www.code
-00000450: 7769 7468 6770 752e 636f 6d29 2069 7320  withgpu.com) is 
-00000460: 6120 636f 6d6d 756e 6974 7920 7468 6174  a community that
-00000470: 2066 6f63 7573 6573 206f 6e20 7468 6520   focuses on the 
-00000480: 7265 7072 6f64 7563 6962 6c65 2041 4920  reproducible AI 
-00000490: 616c 676f 7269 7468 6d73 2e20 4974 2068  algorithms. It h
-000004a0: 6173 2063 6c6f 7365 206c 696e 6b73 2077  as close links w
-000004b0: 6974 6820 5b47 6974 6875 625d 2868 7474  ith [Github](htt
-000004c0: 7073 3a2f 2f77 7777 2e67 6974 6875 622e  ps://www.github.
-000004d0: 636f 6d29 2062 7920 6c65 7665 7261 6769  com) by leveragi
-000004e0: 6e67 2074 6865 206d 616e 6167 6564 2063  ng the managed c
-000004f0: 6f64 652c 2061 6e64 2064 6973 7472 6962  ode, and distrib
-00000500: 7574 6573 2063 6f72 7265 7370 6f6e 6469  utes correspondi
-00000510: 6e67 2064 6f63 6b65 7220 696d 6167 6573  ng docker images
-00000520: 2c20 6d6f 6465 6c73 2061 6e64 206c 6f67  , models and log
-00000530: 7320 666f 7220 6672 6965 6e64 6c79 2072  s for friendly r
-00000540: 6570 726f 6475 6374 696f 6e2e 0a0a 5468  eproduction...Th
-00000550: 6973 2072 6570 6f73 6974 6f72 7920 7072  is repository pr
-00000560: 6f76 6964 6573 2061 206e 6f76 656c 2064  ovides a novel d
-00000570: 6174 6120 6c6f 6164 696e 6720 736f 6c75  ata loading solu
-00000580: 7469 6f6e 2074 6861 7420 6d61 7073 2064  tion that maps d
-00000590: 6174 6120 6265 7477 6565 6e20 5079 7468  ata between Pyth
-000005a0: 6f6e 206f 626a 6563 7420 616e 6420 7365  on object and se
-000005b0: 7269 616c 697a 6564 2062 7974 6573 2061  rialized bytes a
-000005c0: 7574 6f6d 6174 6963 616c 6c79 2e20 5468  utomatically. Th
-000005d0: 6973 2073 6f6c 7574 696f 6e20 656e 636f  is solution enco
-000005e0: 7572 6167 6573 2064 6576 656c 6f70 6572  urages developer
-000005f0: 7320 746f 2062 7569 6c64 2061 2068 6965  s to build a hie
-00000600: 7261 7263 6869 6361 6c20 6461 7461 206c  rarchical data l
-00000610: 6f61 6469 6e67 2070 6970 656c 696e 652c  oading pipeline,
-00000620: 2077 6869 6368 2064 6563 6f75 706c 6573   which decouples
-00000630: 2074 6865 2072 6561 6469 6e67 2c20 7472   the reading, tr
-00000640: 616e 7366 6f72 6d69 6e67 2061 6e64 2062  ansforming and b
-00000650: 6174 6368 696e 672e 2053 696d 696c 6172  atching. Similar
-00000660: 2073 6f6c 7574 696f 6e2c 2073 7563 6820   solution, such 
-00000670: 6173 205b 4e56 4944 4941 2044 414c 495d  as [NVIDIA DALI]
-00000680: 2868 7474 7073 3a2f 2f64 6576 656c 6f70  (https://develop
-00000690: 6572 2e6e 7669 6469 612e 636f 6d2f 6461  er.nvidia.com/da
-000006a0: 6c69 292c 2069 7320 7769 6465 6c79 2064  li), is widely d
-000006b0: 6570 6c6f 7965 6420 696e 206d 616e 7920  eployed in many 
-000006c0: 4850 4320 7379 7374 656d 7320 616e 6420  HPC systems and 
-000006d0: 4d4c 2062 656e 6368 6d61 726b 732e 0a0a  ML benchmarks...
-000006e0: 4265 7369 6465 732c 2069 7420 636f 6e73  Besides, it cons
-000006f0: 6964 6572 7320 6120 6d6f 6475 6c61 7220  iders a modular 
-00000700: 616e 6420 6173 796e 6368 726f 6e6f 7573  and asynchronous
-00000710: 2064 6573 6967 6e20 666f 7220 7468 6520   design for the 
-00000720: 696e 6665 7265 6e63 6520 6f66 2041 4920  inference of AI 
-00000730: 6d6f 6465 6c73 2e20 4465 7665 6c6f 7065  models. Develope
-00000740: 7273 2063 616e 2065 6173 696c 7920 7365  rs can easily se
-00000750: 7276 6520 7468 6569 7220 6d6f 6465 6c73  rve their models
-00000760: 206f 6e20 6469 7374 7269 6275 7465 6420   on distributed 
-00000770: 6465 7669 6365 7320 6279 2063 7265 6174  devices by creat
-00000780: 696e 6720 6120 6d61 6e79 2d74 6f2d 6d61  ing a many-to-ma
-00000790: 6e79 2022 5072 6f64 7563 6572 2d43 6f6e  ny "Producer-Con
-000007a0: 7375 6d65 7222 2064 6174 6166 6c6f 772c  sumer" dataflow,
-000007b0: 2061 6e64 2074 6865 2066 6c6f 7720 636f   and the flow co
-000007c0: 6e74 726f 6c20 6973 2064 6561 6c74 2062  ntrol is dealt b
-000007d0: 7920 7468 6520 7379 6e63 6872 6f6e 6f75  y the synchronou
-000007e0: 7320 7175 6575 6573 2e20 4279 2074 6869  s queues. By thi
-000007f0: 7320 7761 792c 206d 6f64 656c 2073 6572  s way, model ser
-00000800: 7669 6e67 2072 6573 656d 626c 6573 2074  ving resembles t
-00000810: 7261 696e 696e 6720 616e 6420 6361 6e20  raining and can 
-00000820: 616c 736f 2067 6574 2067 7265 6174 2062  also get great b
-00000830: 656e 6566 6974 2066 726f 6d20 7468 6520  enefit from the 
-00000840: 6566 6669 6369 656e 7420 6461 7461 206c  efficient data l
-00000850: 6f61 6465 722e 0a0a 416c 736f 2c20 6974  oader...Also, it
-00000860: 2064 6576 656c 6f70 7320 7468 6520 6265   develops the be
-00000870: 6e63 686d 6172 6b73 206f 6620 6d6f 6465  nchmarks of mode
-00000880: 726e 2041 4920 6d6f 6465 6c73 206f 6e20  rn AI models on 
-00000890: 6469 7665 7273 6520 6163 6365 6c65 7261  diverse accelera
-000008a0: 746f 7273 2c20 696e 636c 7564 696e 6720  tors, including 
-000008b0: 7468 6520 6e65 7765 7374 204e 5649 4449  the newest NVIDI
-000008c0: 4120 4750 5573 2061 6e64 2041 7070 6c65  A GPUs and Apple
-000008d0: 2053 696c 6963 6f6e 2070 726f 6365 7373   Silicon process
-000008e0: 6f72 732e 2049 7420 7769 6c6c 2068 656c  ors. It will hel
-000008f0: 7020 7573 6572 7320 746f 206d 6174 6368  p users to match
-00000900: 2074 6865 6972 2064 656d 616e 6420 6f6e   their demand on
-00000910: 2070 6963 6b69 6e67 2074 6865 2062 6573   picking the bes
-00000920: 7420 7375 6974 6162 6c65 2064 6576 6963  t suitable devic
-00000930: 6573 2e20 2a2a 2ae2 809c 5468 6520 6d6f  es. ***...The mo
-00000940: 7265 2072 6561 736f 6e61 626c 6520 4750  re reasonable GP
-00000950: 5573 2079 6f75 2062 7579 2c20 7468 6520  Us you buy, the 
-00000960: 6d6f 7265 206d 6f6e 6579 2079 6f75 2073  more money you s
-00000970: 6176 652e e280 9d2a 2a2a 0a0a 2323 2049  ave....***..## I
-00000980: 6e73 7461 6c6c 6174 696f 6e0a 0a49 6e73  nstallation..Ins
-00000990: 7461 6c6c 2066 726f 6d20 5079 5049 3a0a  tall from PyPI:.
-000009a0: 0a60 6060 6261 7368 0a70 6970 2069 6e73  .```bash.pip ins
-000009b0: 7461 6c6c 2063 6f64 6577 6974 6867 7075  tall codewithgpu
-000009c0: 0a60 6060 0a0a 4f72 2c20 636c 6f6e 6520  .```..Or, clone 
-000009d0: 7468 6973 2072 6570 6f73 6974 6f72 7920  this repository 
-000009e0: 746f 206c 6f63 616c 2064 6973 6b20 616e  to local disk an
-000009f0: 6420 696e 7374 616c 6c3a 0a0a 6060 6062  d install:..```b
-00000a00: 6173 680a 6364 2063 6f64 6577 6974 6867  ash.cd codewithg
-00000a10: 7075 2026 2620 7069 7020 696e 7374 7361  pu && pip instsa
-00000a20: 6c6c 202e 0a60 6060 0a0a 596f 7520 6361  ll ..```..You ca
-00000a30: 6e20 616c 736f 2069 6e73 7461 6c6c 2066  n also install f
-00000a40: 726f 6d20 7468 6520 7265 6d6f 7465 2072  rom the remote r
-00000a50: 6570 6f73 6974 6f72 793a 200a 0a60 6060  epository: ..```
-00000a60: 6261 7368 0a70 6970 2069 6e73 7461 6c6c  bash.pip install
-00000a70: 2067 6974 2b73 7368 3a2f 2f67 6974 4067   git+ssh://git@g
-00000a80: 6974 6875 622e 636f 6d2f 7365 6574 6163  ithub.com/seetac
-00000a90: 6c6f 7564 2f63 6f64 6577 6974 6867 7075  loud/codewithgpu
-00000aa0: 2e67 6974 0a60 6060 0a0a 2323 2051 7569  .git.```..## Qui
-00000ab0: 636b 2053 7461 7274 0a0a 2323 2320 4465  ck Start..### De
-00000ac0: 706c 6f79 2049 6d61 6765 2049 6e66 6572  ploy Image Infer
-00000ad0: 656e 6365 2041 7070 6c69 6361 7469 6f6e  ence Application
-00000ae0: 0a0a 5365 6520 5b45 7861 6d70 6c65 3a20  ..See [Example: 
-00000af0: 496d 6167 6520 496e 6665 7265 6e63 655d  Image Inference]
-00000b00: 2865 7861 6d70 6c65 732f 696d 6167 655f  (examples/image_
-00000b10: 696e 6665 7265 6e63 652e 7079 292e 0a0a  inference.py)...
-00000b20: 2323 2320 5573 6520 5265 636f 7264 2044  ### Use Record D
-00000b30: 6174 6173 6574 2054 6f20 4163 6365 6c65  ataset To Accele
-00000b40: 7261 7465 2044 6174 6120 4c6f 6164 696e  rate Data Loadin
-00000b50: 670a 0a53 6565 205b 4578 616d 706c 653a  g..See [Example:
-00000b60: 2052 6563 6f72 6420 4461 7461 7365 745d   Record Dataset]
-00000b70: 2865 7861 6d70 6c65 732f 7265 636f 7264  (examples/record
-00000b80: 5f64 6174 6173 6574 2e70 7929 2e0a 0a23  _dataset.py)...#
-00000b90: 2323 204d 6f64 656c 2042 656e 6368 6d61  ## Model Benchma
-00000ba0: 726b 730a 0a53 6565 205b 446f 633a 204d  rks..See [Doc: M
-00000bb0: 6f64 656c 2042 656e 6368 6d61 726b 735d  odel Benchmarks]
-00000bc0: 2862 656e 6368 6d61 726b 732f 6d6f 6465  (benchmarks/mode
-00000bd0: 6c73 2f52 4541 444d 452e 6d64 292e 0a0a  ls/README.md)...
-00000be0: 2323 204c 6963 656e 7365 0a5b 4170 6163  ## License.[Apac
-00000bf0: 6865 204c 6963 656e 7365 2032 2e30 5d28  he License 2.0](
-00000c00: 4c49 4345 4e53 4529 0a0a 0a              LICENSE)...
+00000330: 6e0a 0a3c 6831 2061 6c69 676e 3d22 6365  n..<h1 align="ce
+00000340: 6e74 6572 223e 0a20 203c 6120 6872 6566  nter">.  <a href
+00000350: 3d22 6874 7470 733a 2f2f 7777 772e 636f  ="https://www.co
+00000360: 6465 7769 7468 6770 752e 636f 6d22 3e0a  dewithgpu.com">.
+00000370: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
+00000380: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
+00000390: 6565 7461 636c 6f75 642f 636f 6465 7769  eetacloud/codewi
+000003a0: 7468 6770 752f 626c 6f62 2f6d 6169 6e2f  thgpu/blob/main/
+000003b0: 646f 6373 2f69 6d61 6765 732f 6261 6e6e  docs/images/bann
+000003c0: 6572 5f72 6570 6f73 6974 6f72 792e 706e  er_repository.pn
+000003d0: 6722 2061 6c74 3d22 636f 6465 7769 7468  g" alt="codewith
+000003e0: 6770 7522 2077 6964 7468 3d22 3735 2522  gpu" width="75%"
+000003f0: 3e0a 2020 3c2f 613e 0a3c 2f68 313e 0a0a  >.  </a>.</h1>..
+00000400: 5b43 6f64 6557 6974 6847 5055 5d28 6874  [CodeWithGPU](ht
+00000410: 7470 733a 2f2f 7777 772e 636f 6465 7769  tps://www.codewi
+00000420: 7468 6770 752e 636f 6d29 2069 7320 6120  thgpu.com) is a 
+00000430: 636f 6d6d 756e 6974 7920 7468 6174 2066  community that f
+00000440: 6f63 7573 6573 206f 6e20 7468 6520 7265  ocuses on the re
+00000450: 7072 6f64 7563 6962 6c65 2041 4920 616c  producible AI al
+00000460: 676f 7269 7468 6d73 2e20 4974 2068 6173  gorithms. It has
+00000470: 2063 6c6f 7365 206c 696e 6b73 2077 6974   close links wit
+00000480: 6820 5b47 6974 6875 625d 2868 7474 7073  h [Github](https
+00000490: 3a2f 2f77 7777 2e67 6974 6875 622e 636f  ://www.github.co
+000004a0: 6d29 2062 7920 6c65 7665 7261 6769 6e67  m) by leveraging
+000004b0: 2074 6865 206d 616e 6167 6564 2063 6f64   the managed cod
+000004c0: 652c 2061 6e64 2064 6973 7472 6962 7574  e, and distribut
+000004d0: 6573 2063 6f72 7265 7370 6f6e 6469 6e67  es corresponding
+000004e0: 2064 6f63 6b65 7220 696d 6167 6573 2c20   docker images, 
+000004f0: 6d6f 6465 6c73 2061 6e64 206c 6f67 7320  models and logs 
+00000500: 666f 7220 6672 6965 6e64 6c79 2072 6570  for friendly rep
+00000510: 726f 6475 6374 696f 6e2e 0a0a 5468 6973  roduction...This
+00000520: 2072 6570 6f73 6974 6f72 7920 7072 6f76   repository prov
+00000530: 6964 6573 2061 206e 6f76 656c 2064 6174  ides a novel dat
+00000540: 6120 6c6f 6164 696e 6720 736f 6c75 7469  a loading soluti
+00000550: 6f6e 2074 6861 7420 6d61 7073 2064 6174  on that maps dat
+00000560: 6120 6265 7477 6565 6e20 5079 7468 6f6e  a between Python
+00000570: 206f 626a 6563 7420 616e 6420 7365 7269   object and seri
+00000580: 616c 697a 6564 2062 7974 6573 2061 7574  alized bytes aut
+00000590: 6f6d 6174 6963 616c 6c79 2e20 5468 6973  omatically. This
+000005a0: 2073 6f6c 7574 696f 6e20 656e 636f 7572   solution encour
+000005b0: 6167 6573 2064 6576 656c 6f70 6572 7320  ages developers 
+000005c0: 746f 2062 7569 6c64 2061 2068 6965 7261  to build a hiera
+000005d0: 7263 6869 6361 6c20 6461 7461 206c 6f61  rchical data loa
+000005e0: 6469 6e67 2070 6970 656c 696e 652c 2077  ding pipeline, w
+000005f0: 6869 6368 2064 6563 6f75 706c 6573 2074  hich decouples t
+00000600: 6865 2072 6561 6469 6e67 2c20 7472 616e  he reading, tran
+00000610: 7366 6f72 6d69 6e67 2061 6e64 2062 6174  sforming and bat
+00000620: 6368 696e 672e 2053 696d 696c 6172 2073  ching. Similar s
+00000630: 6f6c 7574 696f 6e2c 2073 7563 6820 6173  olution, such as
+00000640: 205b 4e56 4944 4941 2044 414c 495d 2868   [NVIDIA DALI](h
+00000650: 7474 7073 3a2f 2f64 6576 656c 6f70 6572  ttps://developer
+00000660: 2e6e 7669 6469 612e 636f 6d2f 6461 6c69  .nvidia.com/dali
+00000670: 292c 2069 7320 7769 6465 6c79 2064 6570  ), is widely dep
+00000680: 6c6f 7965 6420 696e 206d 616e 7920 4850  loyed in many HP
+00000690: 4320 7379 7374 656d 7320 616e 6420 4d4c  C systems and ML
+000006a0: 2062 656e 6368 6d61 726b 732e 0a0a 4265   benchmarks...Be
+000006b0: 7369 6465 732c 2069 7420 636f 6e73 6964  sides, it consid
+000006c0: 6572 7320 6120 6d6f 6475 6c61 7220 616e  ers a modular an
+000006d0: 6420 6173 796e 6368 726f 6e6f 7573 2064  d asynchronous d
+000006e0: 6573 6967 6e20 666f 7220 7468 6520 696e  esign for the in
+000006f0: 6665 7265 6e63 6520 6f66 2041 4920 6d6f  ference of AI mo
+00000700: 6465 6c73 2e20 4465 7665 6c6f 7065 7273  dels. Developers
+00000710: 2063 616e 2065 6173 696c 7920 7365 7276   can easily serv
+00000720: 6520 7468 6569 7220 6d6f 6465 6c73 206f  e their models o
+00000730: 6e20 6469 7374 7269 6275 7465 6420 6465  n distributed de
+00000740: 7669 6365 7320 6279 2063 7265 6174 696e  vices by creatin
+00000750: 6720 6120 6d61 6e79 2d74 6f2d 6d61 6e79  g a many-to-many
+00000760: 2022 5072 6f64 7563 6572 2d43 6f6e 7375   "Producer-Consu
+00000770: 6d65 7222 2064 6174 6166 6c6f 772c 2061  mer" dataflow, a
+00000780: 6e64 2074 6865 2066 6c6f 7720 636f 6e74  nd the flow cont
+00000790: 726f 6c20 6973 2064 6561 6c74 2062 7920  rol is dealt by 
+000007a0: 7468 6520 7379 6e63 6872 6f6e 6f75 7320  the synchronous 
+000007b0: 7175 6575 6573 2e20 4279 2074 6869 7320  queues. By this 
+000007c0: 7761 792c 206d 6f64 656c 2073 6572 7669  way, model servi
+000007d0: 6e67 2072 6573 656d 626c 6573 2074 7261  ng resembles tra
+000007e0: 696e 696e 6720 616e 6420 6361 6e20 616c  ining and can al
+000007f0: 736f 2067 6574 2067 7265 6174 2062 656e  so get great ben
+00000800: 6566 6974 2066 726f 6d20 7468 6520 6566  efit from the ef
+00000810: 6669 6369 656e 7420 6461 7461 206c 6f61  ficient data loa
+00000820: 6465 722e 0a0a 416c 736f 2c20 6974 2064  der...Also, it d
+00000830: 6576 656c 6f70 7320 7468 6520 6265 6e63  evelops the benc
+00000840: 686d 6172 6b73 206f 6620 6d6f 6465 726e  hmarks of modern
+00000850: 2041 4920 6d6f 6465 6c73 206f 6e20 6469   AI models on di
+00000860: 7665 7273 6520 6163 6365 6c65 7261 746f  verse accelerato
+00000870: 7273 2c20 696e 636c 7564 696e 6720 7468  rs, including th
+00000880: 6520 6e65 7765 7374 204e 5649 4449 4120  e newest NVIDIA 
+00000890: 4750 5573 2061 6e64 2041 7070 6c65 2053  GPUs and Apple S
+000008a0: 696c 6963 6f6e 2070 726f 6365 7373 6f72  ilicon processor
+000008b0: 732e 2049 7420 7769 6c6c 2068 656c 7020  s. It will help 
+000008c0: 7573 6572 7320 746f 206d 6174 6368 2074  users to match t
+000008d0: 6865 6972 2064 656d 616e 6420 6f6e 2070  heir demand on p
+000008e0: 6963 6b69 6e67 2074 6865 2062 6573 7420  icking the best 
+000008f0: 7375 6974 6162 6c65 2064 6576 6963 6573  suitable devices
+00000900: 2e20 2a2a 2ae2 809c 5468 6520 6d6f 7265  . ***...The more
+00000910: 2072 6561 736f 6e61 626c 6520 4750 5573   reasonable GPUs
+00000920: 2079 6f75 2062 7579 2c20 7468 6520 6d6f   you buy, the mo
+00000930: 7265 206d 6f6e 6579 2079 6f75 2073 6176  re money you sav
+00000940: 652e e280 9d2a 2a2a 0a0a 2323 2049 6e73  e....***..## Ins
+00000950: 7461 6c6c 6174 696f 6e0a 0a49 6e73 7461  tallation..Insta
+00000960: 6c6c 2066 726f 6d20 5079 5049 3a0a 0a60  ll from PyPI:..`
+00000970: 6060 6261 7368 0a70 6970 2069 6e73 7461  ``bash.pip insta
+00000980: 6c6c 2063 6f64 6577 6974 6867 7075 0a60  ll codewithgpu.`
+00000990: 6060 0a0a 4f72 2c20 636c 6f6e 6520 7468  ``..Or, clone th
+000009a0: 6973 2072 6570 6f73 6974 6f72 7920 746f  is repository to
+000009b0: 206c 6f63 616c 2064 6973 6b20 616e 6420   local disk and 
+000009c0: 696e 7374 616c 6c3a 0a0a 6060 6062 6173  install:..```bas
+000009d0: 680a 6364 2063 6f64 6577 6974 6867 7075  h.cd codewithgpu
+000009e0: 2026 2620 7069 7020 696e 7374 7361 6c6c   && pip instsall
+000009f0: 202e 0a60 6060 0a0a 596f 7520 6361 6e20   ..```..You can 
+00000a00: 616c 736f 2069 6e73 7461 6c6c 2066 726f  also install fro
+00000a10: 6d20 7468 6520 7265 6d6f 7465 2072 6570  m the remote rep
+00000a20: 6f73 6974 6f72 793a 200a 0a60 6060 6261  ository: ..```ba
+00000a30: 7368 0a70 6970 2069 6e73 7461 6c6c 2067  sh.pip install g
+00000a40: 6974 2b73 7368 3a2f 2f67 6974 4067 6974  it+ssh://git@git
+00000a50: 6875 622e 636f 6d2f 7365 6574 6163 6c6f  hub.com/seetaclo
+00000a60: 7564 2f63 6f64 6577 6974 6867 7075 2e67  ud/codewithgpu.g
+00000a70: 6974 0a60 6060 0a0a 2323 2051 7569 636b  it.```..## Quick
+00000a80: 2053 7461 7274 0a0a 2323 2320 4465 706c   Start..### Depl
+00000a90: 6f79 2049 6d61 6765 2049 6e66 6572 656e  oy Image Inferen
+00000aa0: 6365 2041 7070 6c69 6361 7469 6f6e 0a0a  ce Application..
+00000ab0: 5365 6520 5b45 7861 6d70 6c65 3a20 496d  See [Example: Im
+00000ac0: 6167 6520 496e 6665 7265 6e63 655d 2865  age Inference](e
+00000ad0: 7861 6d70 6c65 732f 696d 6167 655f 696e  xamples/image_in
+00000ae0: 6665 7265 6e63 652e 7079 292e 0a0a 2323  ference.py)...##
+00000af0: 2320 5573 6520 5265 636f 7264 2044 6174  # Use Record Dat
+00000b00: 6173 6574 2054 6f20 4163 6365 6c65 7261  aset To Accelera
+00000b10: 7465 2044 6174 6120 4c6f 6164 696e 670a  te Data Loading.
+00000b20: 0a53 6565 205b 4578 616d 706c 653a 2052  .See [Example: R
+00000b30: 6563 6f72 6420 4461 7461 7365 745d 2865  ecord Dataset](e
+00000b40: 7861 6d70 6c65 732f 7265 636f 7264 5f64  xamples/record_d
+00000b50: 6174 6173 6574 2e70 7929 2e0a 0a23 2323  ataset.py)...###
+00000b60: 204d 6f64 656c 2042 656e 6368 6d61 726b   Model Benchmark
+00000b70: 730a 0a53 6565 205b 446f 633a 204d 6f64  s..See [Doc: Mod
+00000b80: 656c 2042 656e 6368 6d61 726b 735d 2862  el Benchmarks](b
+00000b90: 656e 6368 6d61 726b 732f 6d6f 6465 6c73  enchmarks/models
+00000ba0: 2f52 4541 444d 452e 6d64 292e 0a0a 2323  /README.md)...##
+00000bb0: 204c 6963 656e 7365 0a5b 4170 6163 6865   License.[Apache
+00000bc0: 204c 6963 656e 7365 2032 2e30 5d28 4c49   License 2.0](LI
+00000bd0: 4345 4e53 4529 0a0a 0a                   CENSE)...
```

## Comparing `codewithgpu-0.2.0.dist-info/RECORD` & `codewithgpu-0.2.1.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 codewithgpu/__init__.py,sha256=w9fTbSSotrutAL0-GdHHJYfXsOk50rADpKRMjWIHTaU,1519
-codewithgpu/version.py,sha256=zy05-sq4BU4KdgAMGRCWTB_DGljq_-FMCOnawK1Bzm0,149
+codewithgpu/cli.py,sha256=OGi5C1KheYHv_4vL-_kzsep87W5WnbgesqZT96UMFw4,1924
+codewithgpu/version.py,sha256=sqrBJvf0ZjTdX9xaFHpv4JGAv-a8ITnbcY44gc9RIjU,185
 codewithgpu/data/__init__.py,sha256=BS1ku8WVrSQXgBXqv0day5ZxbstsOQbW5bWQjyVjoOs,746
-codewithgpu/data/dataset.py,sha256=OJFLndwsKA5sjUd0p7BpMgonCKYCQyMSH0fcXO25HLw,6332
-codewithgpu/data/reader.py,sha256=7G6hW7RN9ZbOObOe87_kb4tcj1q9fHGbtknma-c9pEA,7059
+codewithgpu/data/dataset.py,sha256=lhm1KAR12xb3-AUtHWvYjhPEytL3ozpIY6RDVdsr_Wc,6547
+codewithgpu/data/reader.py,sha256=obDLYyFvZf0WxXdeDMYwqsS14vgXPKvvIxRv7vfA-HE,7177
 codewithgpu/data/record.proto,sha256=mToQiLJ9idcmEoaKwEbCNffe1Cv4ZcNoUhyW2oTvw-Y,608
-codewithgpu/data/record.py,sha256=SPcSXxnk6BoV-hzaDKtOJZicdWjLtdFUI0kZ7dzHRpw,8793
+codewithgpu/data/record.py,sha256=xD53qMX1UWAXrOemlhXuiYZfHxbw0lXGUDof9IsRbfM,8941
 codewithgpu/data/record_pb2.py,sha256=0eygLJUOK3KKsQXBOBbwB-wh-kMQW5Z35ZMAVs0vlsA,10202
 codewithgpu/data/tf_record.proto,sha256=iA-8rb9uDY6g-FFcpAsHW3He1Djc_pRzKXjtk2V3UlI,780
-codewithgpu/data/tf_record.py,sha256=0P9V771ITweo555d6IGgakroQFg1RRLf_BlAYWydgtg,7024
+codewithgpu/data/tf_record.py,sha256=VTfBgEpuvsrSH42irj8Q8DySrJQQet29tLc7hrOk6rk,7299
 codewithgpu/data/tf_record_pb2.py,sha256=OMgulDnqXpDArdyHnI32yy_EOvNggWcOl779grQJ838,11900
 codewithgpu/inference/__init__.py,sha256=BS1ku8WVrSQXgBXqv0day5ZxbstsOQbW5bWQjyVjoOs,746
-codewithgpu/inference/command.py,sha256=ppaALwnMvGW_If4vmipAiXmv4argtgJapHv9QlRcU9k,5969
+codewithgpu/inference/command.py,sha256=7RUMuMQqGLZXc398OtmZmuSuUuc4bfF_uO1cEblNyf0,6128
 codewithgpu/inference/module.py,sha256=59dLqKDfK5D5a3CyvtpKy1X9Osp4F0Bxg7WyVU_0bgw,1474
+codewithgpu/model/__init__.py,sha256=FZ70jzGC0ZCYWDVI54RlrBU2cDSVgoOzZ7uaSChTKOw,761
+codewithgpu/model/download.py,sha256=-SJ7EPqkKYEQTmIQCezDfLgx6YKtPoWuoxbfyTCu89A,1418
 codewithgpu/utils/__init__.py,sha256=BS1ku8WVrSQXgBXqv0day5ZxbstsOQbW5bWQjyVjoOs,746
+codewithgpu/utils/cg_cli.py,sha256=3Urv0uigHTPjfRF4EdSrk1hQbloCIUlgahe3ymL0pdo,4076
+codewithgpu/utils/decorator.py,sha256=eavLk-cu8K9kiTNquJjAwVIziQ2-dG23aFTe3i_1Vkk,3805
+codewithgpu/utils/deprecation.py,sha256=JNzJijpwuXdu9nf4pOzlLqmFvrCM__JZRy5zVU_Xkk8,3629
 codewithgpu/utils/logging.py,sha256=psQyhYN4RRfhcohMvOMIRb2SEsfsRzk3rQzhelhGjgI,3741
 codewithgpu/utils/unittest_util.py,sha256=jz2HVLIHe_TlrQ9QJ-HOg0Erf-QEVmfuQDo0Q4BkfDw,1226
-codewithgpu-0.2.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-codewithgpu-0.2.0.dist-info/METADATA,sha256=SsHVrAANW2LWOPxk2xB01iWAceTb2F7U3-V4yFvhzjQ,3083
-codewithgpu-0.2.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-codewithgpu-0.2.0.dist-info/top_level.txt,sha256=LVhDOD16UsfedWNFxURSX5yK45Izqnt5w3znfgB3zS0,69
-codewithgpu-0.2.0.dist-info/RECORD,,
+codewithgpu-0.2.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+codewithgpu-0.2.1.dist-info/METADATA,sha256=3pnqGYjGTwIFwGq0RpHo8ONEog-Ia6-HHBqGJqjjSfU,3033
+codewithgpu-0.2.1.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+codewithgpu-0.2.1.dist-info/entry_points.txt,sha256=uIKsOHrbYlsA2As8st4u2hBbCA5pGUjKwJuRJUpK0MQ,49
+codewithgpu-0.2.1.dist-info/top_level.txt,sha256=orLQMHWZMLDPkZO_r-8233w9F1YzYk6xqY7Oti5-P4s,87
+codewithgpu-0.2.1.dist-info/RECORD,,
```

