# Comparing `tmp/dewloosh.core-1.0.6.tar.gz` & `tmp/dewloosh.core-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dewloosh.core-1.0.6.tar", last modified: Wed Jun 15 08:19:43 2022, max compression
+gzip compressed data, was "dewloosh.core-1.0.9.tar", last modified: Sun Jun 19 18:14:14 2022, max compression
```

## Comparing `dewloosh.core-1.0.6.tar` & `dewloosh.core-1.0.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-15 08:19:43.320460 dewloosh.core-1.0.6/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1065 2022-06-15 08:19:25.000000 dewloosh.core-1.0.6/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)      115 2022-06-15 08:19:25.000000 dewloosh.core-1.0.6/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10334 2022-06-15 08:19:43.320460 dewloosh.core-1.0.6/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9468 2022-06-15 08:19:25.000000 dewloosh.core-1.0.6/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      105 2022-06-15 08:19:25.000000 dewloosh.core-1.0.6/pyproject.toml
--rw-r--r--   0 circleci  (3434) circleci  (3434)       21 2022-06-15 08:19:25.000000 dewloosh.core-1.0.6/requirements.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-06-15 08:19:43.320460 dewloosh.core-1.0.6/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2906 2022-06-15 08:19:25.000000 dewloosh.core-1.0.6/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-15 08:19:43.316460 dewloosh.core-1.0.6/src/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-15 08:19:43.316460 dewloosh.core-1.0.6/src/dewloosh/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-15 08:19:43.320460 dewloosh.core-1.0.6/src/dewloosh/core/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      293 2022-06-15 08:19:25.000000 dewloosh.core-1.0.6/src/dewloosh/core/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      584 2022-06-15 08:19:25.000000 dewloosh.core-1.0.6/src/dewloosh/core/abc.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4920 2022-06-15 08:19:25.000000 dewloosh.core-1.0.6/src/dewloosh/core/acp.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      956 2022-06-15 08:19:25.000000 dewloosh.core-1.0.6/src/dewloosh/core/attr.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9555 2022-06-15 08:19:25.000000 dewloosh.core-1.0.6/src/dewloosh/core/deepdict.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      883 2022-06-15 08:19:25.000000 dewloosh.core-1.0.6/src/dewloosh/core/infix.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4852 2022-06-15 08:19:25.000000 dewloosh.core-1.0.6/src/dewloosh/core/meta.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6567 2022-06-15 08:19:25.000000 dewloosh.core-1.0.6/src/dewloosh/core/signature.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-15 08:19:43.320460 dewloosh.core-1.0.6/src/dewloosh/core/tools/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       89 2022-06-15 08:19:25.000000 dewloosh.core-1.0.6/src/dewloosh/core/tools/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1498 2022-06-15 08:19:25.000000 dewloosh.core-1.0.6/src/dewloosh/core/tools/alphabet.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1800 2022-06-15 08:19:25.000000 dewloosh.core-1.0.6/src/dewloosh/core/tools/dtk.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2114 2022-06-15 08:19:25.000000 dewloosh.core-1.0.6/src/dewloosh/core/tools/kwargtools.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2807 2022-06-15 08:19:25.000000 dewloosh.core-1.0.6/src/dewloosh/core/tools/tools.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      811 2022-06-15 08:19:25.000000 dewloosh.core-1.0.6/src/dewloosh/core/typing.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4438 2022-06-15 08:19:25.000000 dewloosh.core-1.0.6/src/dewloosh/core/wrapping.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-15 08:19:43.316460 dewloosh.core-1.0.6/src/dewloosh.core.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10334 2022-06-15 08:19:43.000000 dewloosh.core-1.0.6/src/dewloosh.core.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      766 2022-06-15 08:19:43.000000 dewloosh.core-1.0.6/src/dewloosh.core.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-06-15 08:19:43.000000 dewloosh.core-1.0.6/src/dewloosh.core.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-06-15 08:19:39.000000 dewloosh.core-1.0.6/src/dewloosh.core.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)       21 2022-06-15 08:19:43.000000 dewloosh.core-1.0.6/src/dewloosh.core.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        9 2022-06-15 08:19:43.000000 dewloosh.core-1.0.6/src/dewloosh.core.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-06-19 18:14:14.370489 dewloosh.core-1.0.9/
+-rw-rw-rw-   0        0        0     1086 2021-11-30 20:14:54.000000 dewloosh.core-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0      125 2022-06-15 08:43:40.000000 dewloosh.core-1.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0    12601 2022-06-19 18:14:14.370489 dewloosh.core-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     9901 2022-06-19 18:09:51.000000 dewloosh.core-1.0.9/README.md
+-rw-rw-rw-   0        0        0      110 2021-11-30 20:14:54.000000 dewloosh.core-1.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       24 2022-02-03 09:49:32.000000 dewloosh.core-1.0.9/requirements.txt
+-rw-rw-rw-   0        0        0       42 2022-06-19 18:14:14.370489 dewloosh.core-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     2994 2022-06-15 07:58:14.000000 dewloosh.core-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2022-06-19 18:14:14.331490 dewloosh.core-1.0.9/src/
+drwxrwxrwx   0        0        0        0 2022-06-19 18:14:14.331490 dewloosh.core-1.0.9/src/dewloosh/
+drwxrwxrwx   0        0        0        0 2022-06-19 18:14:14.363489 dewloosh.core-1.0.9/src/dewloosh/core/
+-rw-rw-rw-   0        0        0      301 2022-06-19 14:00:32.000000 dewloosh.core-1.0.9/src/dewloosh/core/__init__.py
+-rw-rw-rw-   0        0        0      613 2022-06-13 10:36:36.000000 dewloosh.core-1.0.9/src/dewloosh/core/abc.py
+-rw-rw-rw-   0        0        0     5061 2022-06-12 08:52:22.000000 dewloosh.core-1.0.9/src/dewloosh/core/acp.py
+-rw-rw-rw-   0        0        0      993 2022-01-16 10:33:45.000000 dewloosh.core-1.0.9/src/dewloosh/core/attr.py
+-rw-rw-rw-   0        0        0     9935 2022-06-19 13:48:33.000000 dewloosh.core-1.0.9/src/dewloosh/core/deepdict.py
+-rw-rw-rw-   0        0        0      919 2022-06-13 11:56:57.000000 dewloosh.core-1.0.9/src/dewloosh/core/infix.py
+-rw-rw-rw-   0        0        0     4979 2022-06-13 10:37:04.000000 dewloosh.core-1.0.9/src/dewloosh/core/meta.py
+-rw-rw-rw-   0        0        0     6764 2022-06-13 10:41:56.000000 dewloosh.core-1.0.9/src/dewloosh/core/signature.py
+drwxrwxrwx   0        0        0        0 2022-06-19 18:14:14.368490 dewloosh.core-1.0.9/src/dewloosh/core/tools/
+-rw-rw-rw-   0        0        0       92 2022-06-13 10:38:42.000000 dewloosh.core-1.0.9/src/dewloosh/core/tools/__init__.py
+-rw-rw-rw-   0        0        0     1618 2022-06-19 13:48:45.000000 dewloosh.core-1.0.9/src/dewloosh/core/tools/alphabet.py
+-rw-rw-rw-   0        0        0     1863 2022-06-07 14:04:25.000000 dewloosh.core-1.0.9/src/dewloosh/core/tools/dtk.py
+-rw-rw-rw-   0        0        0     2256 2022-06-19 13:48:51.000000 dewloosh.core-1.0.9/src/dewloosh/core/tools/kwargtools.py
+-rw-rw-rw-   0        0        0     2918 2022-06-12 09:22:44.000000 dewloosh.core-1.0.9/src/dewloosh/core/tools/tools.py
+-rw-rw-rw-   0        0        0      917 2022-06-19 13:48:39.000000 dewloosh.core-1.0.9/src/dewloosh/core/typing.py
+-rw-rw-rw-   0        0        0     4570 2022-06-03 18:15:08.000000 dewloosh.core-1.0.9/src/dewloosh/core/wrapping.py
+drwxrwxrwx   0        0        0        0 2022-06-19 18:14:14.354489 dewloosh.core-1.0.9/src/dewloosh.core.egg-info/
+-rw-rw-rw-   0        0        0    12601 2022-06-19 18:14:14.000000 dewloosh.core-1.0.9/src/dewloosh.core.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      766 2022-06-19 18:14:14.000000 dewloosh.core-1.0.9/src/dewloosh.core.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-06-19 18:14:14.000000 dewloosh.core-1.0.9/src/dewloosh.core.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2021-12-13 12:00:10.000000 dewloosh.core-1.0.9/src/dewloosh.core.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       21 2022-06-19 18:14:14.000000 dewloosh.core-1.0.9/src/dewloosh.core.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2022-06-19 18:14:14.000000 dewloosh.core-1.0.9/src/dewloosh.core.egg-info/top_level.txt
```

### Comparing `dewloosh.core-1.0.6/LICENSE` & `dewloosh.core-1.0.9/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2021 dewloosh
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2021 dewloosh
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `dewloosh.core-1.0.6/PKG-INFO` & `dewloosh.core-1.0.9/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,646 +1,619 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 6465 776c  : 2.1.Name: dewl
-00000020: 6f6f 7368 2e63 6f72 650a 5665 7273 696f  oosh.core.Versio
-00000030: 6e3a 2031 2e30 2e36 0a53 756d 6d61 7279  n: 1.0.6.Summary
-00000040: 3a20 436f 6d6d 6f6e 2064 6576 656c 6f70  : Common develop
-00000050: 6572 2075 7469 6c69 7469 6573 2061 6e64  er utilities and
-00000060: 2062 6173 6520 636c 6173 7365 7320 746f   base classes to
-00000070: 2073 7570 706f 7274 206f 7468 6572 2064   support other d
-00000080: 6577 6c6f 6f73 6820 7061 636b 6167 6573  ewloosh packages
-00000090: 2e0a 486f 6d65 2d70 6167 653a 2068 7474  ..Home-page: htt
-000000a0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000000b0: 6465 776c 6f6f 7368 2f64 6577 6c6f 6f73  dewloosh/dewloos
-000000c0: 682d 636f 7265 0a41 7574 686f 723a 2064  h-core.Author: d
-000000d0: 6577 6c6f 6f73 680a 4175 7468 6f72 2d65  ewloosh.Author-e
-000000e0: 6d61 696c 3a20 6465 776c 6f6f 7368 4067  mail: dewloosh@g
-000000f0: 6d61 696c 2e63 6f6d 0a4c 6963 656e 7365  mail.com.License
-00000100: 3a20 554e 4b4e 4f57 4e0a 446f 776e 6c6f  : UNKNOWN.Downlo
-00000110: 6164 2d55 524c 3a20 6874 7470 733a 2f2f  ad-URL: https://
-00000120: 6769 7468 7562 2e63 6f6d 2f64 6577 6c6f  github.com/dewlo
-00000130: 6f73 682f 6465 776c 6f6f 7368 2d63 6f72  osh/dewloosh-cor
-00000140: 652f 6172 6368 6976 652f 7265 6673 2f74  e/archive/refs/t
-00000150: 6167 732f 312e 302e 362e 7a69 700a 506c  ags/1.0.6.zip.Pl
-00000160: 6174 666f 726d 3a20 554e 4b4e 4f57 4e0a  atform: UNKNOWN.
-00000170: 436c 6173 7369 6669 6572 3a20 4465 7665  Classifier: Deve
-00000180: 6c6f 706d 656e 7420 5374 6174 7573 203a  lopment Status :
-00000190: 3a20 3520 2d20 5072 6f64 7563 7469 6f6e  : 5 - Production
-000001a0: 2f53 7461 626c 650a 436c 6173 7369 6669  /Stable.Classifi
-000001b0: 6572 3a20 4c69 6365 6e73 6520 3a3a 204f  er: License :: O
-000001c0: 5349 2041 7070 726f 7665 6420 3a3a 204d  SI Approved :: M
-000001d0: 4954 204c 6963 656e 7365 0a43 6c61 7373  IT License.Class
-000001e0: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
-000001f0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000200: 7974 686f 6e20 3a3a 2033 2e36 0a43 6c61  ython :: 3.6.Cla
-00000210: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
-00000220: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000230: 2050 7974 686f 6e20 3a3a 2033 2e37 0a43   Python :: 3.7.C
-00000240: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
-00000250: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000260: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e38  :: Python :: 3.8
-00000270: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
-00000280: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000290: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-000002a0: 2e39 0a43 6c61 7373 6966 6965 723a 2050  .9.Classifier: P
-000002b0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-000002c0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-000002d0: 2033 203a 3a20 4f6e 6c79 0a43 6c61 7373   3 :: Only.Class
-000002e0: 6966 6965 723a 204f 7065 7261 7469 6e67  ifier: Operating
-000002f0: 2053 7973 7465 6d20 3a3a 204f 5320 496e   System :: OS In
-00000300: 6465 7065 6e64 656e 740a 5265 7175 6972  dependent.Requir
-00000310: 6573 2d50 7974 686f 6e3a 203e 3d33 2e36  es-Python: >=3.6
-00000320: 0a44 6573 6372 6970 7469 6f6e 2d43 6f6e  .Description-Con
-00000330: 7465 6e74 2d54 7970 653a 2074 6578 742f  tent-Type: text/
-00000340: 6d61 726b 646f 776e 0a4c 6963 656e 7365  markdown.License
-00000350: 2d46 696c 653a 204c 4943 454e 5345 0a0a  -File: LICENSE..
-00000360: 2320 2a2a 6465 776c 6f6f 7368 2e63 6f72  # **dewloosh.cor
-00000370: 652a 2a0a 0a3c 6120 6872 6566 3d27 6874  e**..<a href='ht
-00000380: 7470 733a 2f2f 6465 776c 6f6f 7368 2d63  tps://dewloosh-c
-00000390: 6f72 652e 7265 6164 7468 6564 6f63 732e  ore.readthedocs.
-000003a0: 696f 2f65 6e2f 6c61 7465 7374 2f3f 6261  io/en/latest/?ba
-000003b0: 6467 653d 6c61 7465 7374 273e 0a20 2020  dge=latest'>.   
-000003c0: 203c 696d 6720 7372 633d 2768 7474 7073   <img src='https
-000003d0: 3a2f 2f72 6561 6474 6865 646f 6373 2e6f  ://readthedocs.o
-000003e0: 7267 2f70 726f 6a65 6374 732f 6465 776c  rg/projects/dewl
-000003f0: 6f6f 7368 2d63 6f72 652f 6261 6467 652f  oosh-core/badge/
-00000400: 3f76 6572 7369 6f6e 3d6c 6174 6573 7427  ?version=latest'
-00000410: 2061 6c74 3d27 446f 6375 6d65 6e74 6174   alt='Documentat
-00000420: 696f 6e20 5374 6174 7573 2720 2f3e 0a3c  ion Status' />.<
-00000430: 2f61 3e0a 3c61 2068 7265 663d 2268 7474  /a>.<a href="htt
-00000440: 7073 3a2f 2f70 7970 692e 6f72 672f 7072  ps://pypi.org/pr
-00000450: 6f6a 6563 742f 6465 776c 6f6f 7368 2e63  oject/dewloosh.c
-00000460: 6f72 6522 2f3e 0a20 2020 2020 2020 2020  ore"/>.         
-00000470: 2020 203c 696d 6720 7372 633d 2268 7474     <img src="htt
-00000480: 7073 3a2f 2f62 6164 6765 2e66 7572 792e  ps://badge.fury.
-00000490: 696f 2f70 792f 6465 776c 6f6f 7368 2e63  io/py/dewloosh.c
-000004a0: 6f72 652e 7376 6722 2f3e 0a3c 2f61 3e0a  ore.svg"/>.</a>.
-000004b0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-000004c0: 2f6f 7065 6e73 6f75 7263 652e 6f72 672f  /opensource.org/
-000004d0: 6c69 6365 6e73 6573 2f4d 4954 222f 3e0a  licenses/MIT"/>.
-000004e0: 2020 2020 2020 2020 2020 2020 3c69 6d67              <img
-000004f0: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
-00000500: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
-00000510: 6765 2f4c 6963 656e 7365 2d4d 4954 2d79  ge/License-MIT-y
-00000520: 656c 6c6f 772e 7376 6722 2f3e 0a3c 2f61  ellow.svg"/>.</a
-00000530: 3e0a 0a0a 5468 6973 2070 6163 6b61 6765  >...This package
-00000540: 2063 6f6e 7461 696e 7320 636f 6d6d 6f6e   contains common
-00000550: 2064 6576 656c 6f70 6572 2075 7469 6c69   developer utili
-00000560: 7469 6573 2074 6f20 7375 7070 6f72 7420  ties to support 
-00000570: 6f74 6865 7220 6064 6577 6c6f 6f73 6860  other `dewloosh`
-00000580: 2073 6f6c 7574 696f 6e73 2e20 4576 6572   solutions. Ever
-00000590: 7974 6869 6e67 2069 7320 7075 7265 2050  ything is pure P
-000005a0: 7974 686f 6e2c 2074 6865 2070 6163 6b61  ython, the packa
-000005b0: 6765 2072 6571 7569 7265 7320 6e6f 2065  ge requires no e
-000005c0: 7874 7261 2064 6570 656e 6465 6e63 6965  xtra dependencie
-000005d0: 7320 616e 6420 7368 6f75 6c64 2072 756e  s and should run
-000005e0: 206f 6e20 6120 6d69 6e69 6d61 6c20 7365   on a minimal se
-000005f0: 7475 702e 0a0a 5468 6520 6d6f 7374 2069  tup...The most i
-00000600: 6d70 6f72 7461 6e74 2066 6561 7475 7265  mportant feature
-00000610: 733a 0a0a 2a20 5661 7269 6f75 7320 6469  s:..* Various di
-00000620: 6374 696f 6e61 7279 2063 6c61 7373 6573  ctionary classes
-00000630: 2074 6861 7420 656e 6861 6e63 6520 7468   that enhance th
-00000640: 6520 636f 7265 2062 6568 6176 696f 7572  e core behaviour
-00000650: 206f 6620 7468 6520 6275 696c 742d 696e   of the built-in
-00000660: 2060 6469 6374 6020 7479 7065 2e20 5468   `dict` type. Th
-00000670: 6520 746f 7020 6f66 2074 6865 2063 616b  e top of the cak
-00000680: 6520 6973 2074 6865 2060 4465 6570 4469  e is the `DeepDi
-00000690: 6374 6020 636c 6173 732c 2077 6869 6368  ct` class, which
-000006a0: 206f 6666 6572 7320 6120 6469 6666 6572   offers a differ
-000006b0: 656e 7420 6265 6861 7669 6f75 7220 666f  ent behaviour fo
-000006c0: 7220 6e65 7374 6564 2064 6963 7469 6f6e  r nested diction
-000006d0: 6172 6965 7320 6279 2061 7070 6c79 696e  aries by applyin
-000006e0: 6720 6120 7365 6c66 2072 6570 6c69 6361  g a self replica
-000006f0: 7469 6e67 2064 6566 616c 7420 6661 6374  ting defalt fact
-00000700: 6f72 792e 0a0a 2a20 4120 7365 7420 6f66  ory...* A set of
-00000710: 2074 6f6f 6c73 2066 6f72 206d 6574 6170   tools for metap
-00000720: 726f 6772 616d 6d69 6e67 2e20 5468 6520  rogramming. The 
-00000730: 7573 6520 6361 7365 7320 696e 636c 7564  use cases includ
-00000740: 6520 6465 636c 6172 696e 6720 6375 7374  e declaring cust
-00000750: 6f6d 2061 6273 7472 6163 7420 636c 6173  om abstract clas
-00000760: 7320 7072 6f70 6572 7469 6573 2c20 7573  s properties, us
-00000770: 696e 6720 6d65 7461 636c 6173 7365 7320  ing metaclasses 
-00000780: 746f 2061 766f 6964 2075 6e77 616e 7465  to avoid unwante
-00000790: 6420 636f 6465 2063 6f6e 666c 6963 7473  d code conflicts
-000007a0: 2c20 6173 7375 7269 6e67 2074 6865 2069  , assuring the i
-000007b0: 6d70 6c65 6d65 6e74 6174 696f 6e20 6f66  mplementation of
-000007c0: 2061 6273 7472 6163 7420 6d65 7468 6f64   abstract method
-000007d0: 7320 6174 2064 6573 6967 6e20 7469 6d65  s at design time
-000007e0: 2c20 6574 632e 0a0a 2a20 4465 636f 7261  , etc...* Decora
-000007f0: 746f 7273 2c20 7772 6170 7065 7273 2061  tors, wrappers a
-00000800: 6e64 206f 7468 6572 2068 616e 6479 2064  nd other handy d
-00000810: 6576 656c 6f70 6572 2074 6f6f 6c73 2e0a  eveloper tools..
-00000820: 0a23 2320 2a2a 446f 6375 6d65 6e74 6174  .## **Documentat
-00000830: 696f 6e20 616e 6420 4973 7375 6573 2a2a  ion and Issues**
-00000840: 0a0a 436c 6963 6b20 5b68 6572 655d 2868  ..Click [here](h
-00000850: 7474 7073 3a2f 2f64 6577 6c6f 6f73 682d  ttps://dewloosh-
-00000860: 636f 7265 2e72 6561 6474 6865 646f 6373  core.readthedocs
-00000870: 2e69 6f2f 656e 2f6c 6174 6573 742f 2920  .io/en/latest/) 
-00000880: 746f 2072 6561 6420 7468 6520 646f 6375  to read the docu
-00000890: 6d65 6e74 6174 696f 6e2e 0a0a 5468 6572  mentation...Ther
-000008a0: 6520 6172 6520 6e6f 206b 6e6f 776e 2069  e are no known i
-000008b0: 7373 7565 732e 0a0a 2323 202a 2a41 2051  ssues...## **A Q
-000008c0: 7569 636b 2047 7569 6465 2a2a 0a0a 2323  uick Guide**..##
-000008d0: 2323 2044 6963 7469 6f6e 6172 6965 7320  ## Dictionaries 
-000008e0: 6f66 2064 6963 7469 6f6e 6172 6965 7320  of dictionaries 
-000008f0: 6f66 2064 6961 6374 696f 6e61 7269 6573  of diactionaries
-00000900: 206f 6620 2e2e 2e0a 0a49 6e20 6576 6572   of .....In ever
-00000910: 7920 6361 7365 2077 6865 7265 2079 6f75  y case where you
-00000920: 2764 2077 616e 7420 746f 2075 7365 2061  'd want to use a
-00000930: 2060 6469 6374 602c 2079 6f75 2063 616e   `dict`, you can
-00000940: 2075 7365 2061 2060 4465 6570 6469 6374   use a `Deepdict
-00000950: 6020 6173 2061 2064 726f 702d 696e 2072  ` as a drop-in r
-00000960: 6570 6c61 6365 6d65 6e74 2c20 6275 7420  eplacement, but 
-00000970: 6f6e 2074 6f70 206f 6620 7768 6174 2061  on top of what a
-00000980: 2073 696d 706c 6520 6469 6374 696f 6e61   simple dictiona
-00000990: 7279 2070 726f 7669 6465 732c 2061 2060  ry provides, a `
-000009a0: 4465 6570 6469 6374 6020 6973 206d 6f72  Deepdict` is mor
-000009b0: 6520 6361 7061 626c 652c 2061 7320 6974  e capable, as it
-000009c0: 2070 726f 7669 6465 7320 6120 6d61 6368   provides a mach
-000009d0: 696e 6572 7920 746f 2068 616e 646c 6520  inery to handle 
-000009e0: 6e65 7374 6564 206c 6179 6f75 7473 2e20  nested layouts. 
-000009f0: 4974 2069 7320 6261 7369 6361 6c6c 7920  It is basically 
-00000a00: 616e 206f 7264 6572 6564 2060 6465 6661  an ordered `defa
-00000a10: 756c 7464 6963 7460 2077 6974 6820 6120  ultdict` with a 
-00000a20: 7365 6c66 2072 6570 6c69 6361 7469 6e67  self replicating
-00000a30: 2064 6566 6175 6c74 2066 6163 746f 7279   default factory
-00000a40: 2e20 0a0a 6060 6070 7974 686f 6e0a 3e3e  . ..```python.>>
-00000a50: 3e20 6672 6f6d 2064 6577 6c6f 6f73 682e  > from dewloosh.
-00000a60: 636f 7265 2069 6d70 6f72 7420 4465 6570  core import Deep
-00000a70: 6469 6374 0a3e 3e3e 2064 6174 6120 3d20  dict.>>> data = 
-00000a80: 4465 6570 6469 6374 2829 0a60 6060 0a0a  Deepdict().```..
-00000a90: 4120 6044 6565 7064 6963 7460 2069 7320  A `Deepdict` is 
-00000aa0: 6573 7365 6e74 6961 6c6c 7920 6120 6e65  essentially a ne
-00000ab0: 7374 6564 2064 6566 6175 6c74 2064 6963  sted default dic
-00000ac0: 7469 6f6e 6172 792e 2042 6569 6e67 206e  tionary. Being n
-00000ad0: 6573 7465 6420 7265 6665 7273 2074 6f20  ested refers to 
-00000ae0: 7468 6520 6661 6374 2074 6861 7420 796f  the fact that yo
-00000af0: 7520 6361 6e20 646f 2074 6869 733a 0a0a  u can do this:..
-00000b00: 6060 6070 7974 686f 6e0a 3e3e 3e20 6461  ```python.>>> da
-00000b10: 7461 5b27 6127 5d5b 2762 275d 5b27 6327  ta['a']['b']['c'
-00000b20: 5d5b 2765 275d 203d 2031 0a3e 3e3e 2064  ]['e'] = 1.>>> d
-00000b30: 6174 615b 2761 275d 5b27 6227 5d5b 2764  ata['a']['b']['d
-00000b40: 275d 203d 2032 0a60 6060 0a0a 4e6f 7469  '] = 2.```..Noti
-00000b50: 6365 2074 6861 7420 7468 6520 6f62 6a65  ce that the obje
-00000b60: 6374 2063 6172 7665 7320 6120 7761 7920  ct carves a way 
-00000b70: 7570 2075 6e74 696c 2074 6865 206c 6173  up until the las
-00000b80: 7420 6b65 792c 2077 6974 686f 7574 206e  t key, without n
-00000b90: 6565 6469 6e67 2074 6f20 6372 6561 7465  eeding to create
-00000ba0: 2065 6163 6820 6c65 7665 6c20 6578 706c   each level expl
-00000bb0: 6963 6974 6c79 2e20 5768 6174 2068 6170  icitly. What hap
-00000bc0: 7065 6e73 2069 7320 7468 6174 2065 7665  pens is that eve
-00000bd0: 7279 2074 696d 6520 6120 6b65 7920 6973  ry time a key is
-00000be0: 206d 6973 7369 6e67 2069 6e20 6120 6064   missing in a `d
-00000bf0: 6174 6160 2c20 7468 6520 6f62 6a65 6374  ata`, the object
-00000c00: 2063 7265 6174 6573 2061 206e 6577 2069   creates a new i
-00000c10: 6e73 7461 6e63 652c 2077 6869 6368 2074  nstance, which t
-00000c20: 6865 6e20 6973 2061 6c73 6f20 7265 6164  hen is also read
-00000c30: 7920 746f 2068 616e 646c 6520 6d69 7373  y to handle miss
-00000c40: 696e 6720 6b65 7973 206f 7220 6461 7461  ing keys or data
-00000c50: 2e20 4163 6365 7373 696e 6720 6e65 7374  . Accessing nest
-00000c60: 6564 2073 7562 6469 6374 696f 6e61 7269  ed subdictionari
-00000c70: 6573 2077 6f72 6b73 2069 6e20 6120 7369  es works in a si
-00000c80: 6d69 6c61 7220 6661 7368 696f 6e3a 0a0a  milar fashion:..
-00000c90: 6060 6070 7974 686f 6e0a 3e3e 3e20 6461  ```python.>>> da
-00000ca0: 7461 5b27 6127 5d5b 2762 275d 5b27 6327  ta['a']['b']['c'
-00000cb0: 5d5b 2765 275d 0a31 0a60 6060 0a54 6f20  ]['e'].1.```.To 
-00000cc0: 616c 6c6f 7720 666f 7220 6120 6d6f 7265  allow for a more
-00000cd0: 2050 7974 686f 6e69 6320 6665 656c 2c20   Pythonic feel, 
-00000ce0: 6974 2061 6c73 6f20 7375 7070 6f72 7473  it also supports
-00000cf0: 2061 7272 6179 2d6c 696b 6520 696e 6465   array-like inde
-00000d00: 7869 6e67 2c20 736f 2074 6861 7420 7468  xing, so that th
-00000d10: 6520 666f 6c6c 6f77 696e 6720 6f70 6572  e following oper
-00000d20: 6174 696f 6e73 2061 7265 2076 616c 6964  ations are valid
-00000d30: 3a20 0a0a 6060 6070 7974 686f 6e0a 3e3e  : ..```python.>>
-00000d40: 3e20 6461 7461 5b27 6127 2c20 2762 272c  > data['a', 'b',
-00000d50: 2027 6327 2c20 2765 275d 203d 2033 0a3e   'c', 'e'] = 3.>
-00000d60: 3e3e 2064 6174 615b 2761 272c 2027 6227  >> data['a', 'b'
-00000d70: 2c20 2763 272c 2027 6527 5d0a 330a 6060  , 'c', 'e'].3.``
-00000d80: 600a 0a4f 6620 636f 7572 7365 2c20 7468  `..Of course, th
-00000d90: 6973 2069 7320 736f 6d65 7468 696e 6720  is is something 
-00000da0: 7468 6174 2077 6520 6361 6e20 6561 7369  that we can easi
-00000db0: 6c79 2072 6570 6c69 6361 7465 2075 7369  ly replicate usi
-00000dc0: 6e67 2070 7572 6520 5079 7468 6f6e 2069  ng pure Python i
-00000dd0: 6e20 6f6e 6520 6c69 6e65 2c20 7769 7468  n one line, with
-00000de0: 6f75 7420 7468 6520 6e65 6564 2066 6f72  out the need for
-00000df0: 2066 616e 6379 2073 7475 6666 3a0a 0a60   fancy stuff:..`
-00000e00: 6060 7079 7468 6f6e 0a3e 3e3e 2064 6174  ``python.>>> dat
-00000e10: 6120 3d20 7b27 6127 203a 207b 2762 2720  a = {'a' : {'b' 
-00000e20: 3a20 7b27 6327 203a 207b 2765 2720 3a20  : {'c' : {'e' : 
-00000e30: 337d 2c20 2764 2720 3a20 327d 7d7d 2020  3}, 'd' : 2}}}  
-00000e40: 2020 0a60 6060 0a0a 5468 6520 6b65 7920    .```..The key 
-00000e50: 706f 696e 7420 6973 2074 6861 7420 7765  point is that we
-00000e60: 206c 6f6f 7020 6f76 6572 2061 2070 7572   loop over a pur
-00000e70: 6520 6064 6963 7460 2069 6e73 7461 6e63  e `dict` instanc
-00000e80: 652c 2077 6520 6765 740a 0a60 6060 7079  e, we get..```py
-00000e90: 7468 6f6e 0a3e 3e3e 205b 6b20 666f 7220  thon.>>> [k for 
-00000ea0: 6b20 696e 2064 6174 612e 6b65 7973 2829  k in data.keys()
-00000eb0: 5d0a 5b27 6127 5d20 2020 200a 6060 600a  ].['a']    .```.
-00000ec0: 0a42 7574 2069 6620 7765 2075 7365 2061  .But if we use a
-00000ed0: 2060 4465 6570 6469 6374 6020 636c 6173   `Deepdict` clas
-00000ee0: 7320 616e 6420 7468 6520 6f70 7469 6f6e  s and the option
-00000ef0: 2060 6465 6570 3d54 7275 6560 2077 6865   `deep=True` whe
-00000f00: 6e20 6163 6365 7373 696e 670a 6b65 7973  n accessing.keys
-00000f10: 2c20 7661 6c75 6573 206f 7220 6974 656d  , values or item
-00000f20: 7320 6f66 2064 6963 7469 6f6e 6172 6965  s of dictionarie
-00000f30: 732c 2074 6865 2066 6f6c 6c6f 7769 6e67  s, the following
-00000f40: 2068 6170 7065 6e73 3a20 0a0a 6060 6070   happens: ..```p
-00000f50: 7974 686f 6e0a 3e3e 3e20 5b6b 2066 6f72  ython.>>> [k for
-00000f60: 206b 2069 6e20 4465 6570 6469 6374 2864   k in Deepdict(d
-00000f70: 6174 6129 2e6b 6579 7328 6465 6570 3d54  ata).keys(deep=T
-00000f80: 7275 6529 5d0a 5b27 6527 2c20 2764 275d  rue)].['e', 'd']
-00000f90: 2020 2020 0a60 6060 0a0a 5765 2063 616e      .```..We can
-00000fa0: 2073 6565 2c20 7468 6174 2069 6e20 7468   see, that in th
-00000fb0: 6973 2063 6173 652c 2069 7465 7261 7469  is case, iterati
-00000fc0: 6f6e 2067 6f65 7320 6f76 6572 206b 6579  on goes over key
-00000fd0: 732c 2074 6861 7420 6163 7475 616c 6c79  s, that actually
-00000fe0: 2068 6f6c 6420 6f6e 2074 6f20 736f 6d65   hold on to some
-00000ff0: 2064 6174 612c 2061 6e64 2064 6f65 7320   data, and does 
-00001000: 6e6f 7420 7265 7475 726e 2074 6865 2063  not return the c
-00001010: 6f6e 7461 696e 6572 7320 7468 656d 7365  ontainers themse
-00001020: 6c76 6573 2e20 4966 2077 6520 646f 2074  lves. If we do t
-00001030: 6865 2073 616d 6520 6578 7065 7269 6d65  he same experime
-00001040: 6e74 2077 6974 6820 7468 6520 7661 6c75  nt with the valu
-00001050: 6573 2c20 6974 2073 686f 7773 2074 6861  es, it shows tha
-00001060: 7420 7468 6520 6044 6565 7064 6963 7460  t the `Deepdict`
-00001070: 206f 6e6c 7920 7265 7475 726e 7320 7468   only returns th
-00001080: 6520 6c65 6166 7320 6f66 2074 6865 2064  e leafs of the d
-00001090: 6174 612d 7472 6565 2061 6e64 2074 6865  ata-tree and the
-000010a0: 2062 6568 6176 696f 7572 2069 7320 6675   behaviour is fu
-000010b0: 6e64 616d 656e 7461 6c6c 7920 6469 6666  ndamentally diff
-000010c0: 6572 656e 743a 0a0a 6060 6070 7974 686f  erent:..```pytho
-000010d0: 6e0a 3e3e 3e20 5b6b 2066 6f72 206b 2069  n.>>> [k for k i
-000010e0: 6e20 6461 7461 2e76 616c 7565 7328 295d  n data.values()]
-000010f0: 0a5b 7b27 6227 3a20 7b27 6327 3a20 7b27  .[{'b': {'c': {'
-00001100: 6527 3a20 337d 2c20 2764 273a 2032 7d7d  e': 3}, 'd': 2}}
-00001110: 5d20 2020 200a 6060 600a 0a60 6060 7079  ]    .```..```py
-00001120: 7468 6f6e 0a3e 3e3e 205b 6b20 666f 7220  thon.>>> [k for 
-00001130: 6b20 696e 2044 6565 7064 6963 7428 6461  k in Deepdict(da
-00001140: 7461 292e 7661 6c75 6573 2864 6565 703d  ta).values(deep=
-00001150: 5472 7565 295d 0a5b 332c 2032 5d20 2020  True)].[3, 2]   
-00001160: 200a 6060 600a 0a49 7420 6973 2069 6d70   .```..It is imp
-00001170: 6f72 7461 6e74 2c20 7468 6174 2074 6865  ortant, that the
-00001180: 2063 616c 6c20 606f 626a 2e76 616c 7565   call `obj.value
-00001190: 7328 6465 6570 3d54 7275 6529 6020 7374  s(deep=True)` st
-000011a0: 696c 6c20 7265 7475 726e 7320 6120 6765  ill returns a ge
-000011b0: 6e65 7261 746f 7220 6f62 6a65 6374 2c20  nerator object, 
-000011c0: 7768 6963 6820 6d61 6b65 7320 6974 206d  which makes it m
-000011d0: 656d 6f72 7920 6566 6669 6369 656e 7420  emory efficient 
-000011e0: 7768 656e 206c 6f6f 7069 6e67 206f 7665  when looping ove
-000011f0: 7220 6c61 7267 6520 6461 7461 7365 7473  r large datasets
-00001200: 2e0a 0a60 6060 7079 7468 6f6e 0a3e 3e3e  ...```python.>>>
-00001210: 2044 6565 7064 6963 7428 6461 7461 292e   Deepdict(data).
-00001220: 7661 6c75 6573 2864 6565 703d 5472 7565  values(deep=True
-00001230: 290a 3c67 656e 6572 6174 6f72 206f 626a  ).<generator obj
-00001240: 6563 7420 4f72 6465 7265 6444 6566 6175  ect OrderedDefau
-00001250: 6c74 4469 6374 2e76 616c 7565 7320 6174  ltDict.values at
-00001260: 2030 7830 3030 3030 3238 4632 3039 4435   0x0000028F209D5
-00001270: 3441 303e 2020 2020 0a60 6060 0a0a 2323  4A0>    .```..##
-00001280: 2323 2057 7261 7070 696e 670a 0a57 7261  ## Wrapping..Wra
-00001290: 7070 696e 6720 6d61 7920 6e6f 7420 6265  pping may not be
-000012a0: 2074 6865 206d 6f73 7420 656c 6567 616e   the most elegan
-000012b0: 7420 736f 6c75 7469 6f6e 7320 746f 2069  t solutions to i
-000012c0: 6e68 6572 6974 2070 726f 7065 7274 6965  nherit propertie
-000012d0: 7320 6f66 2061 2064 6966 6665 7265 6e74  s of a different
-000012e0: 2063 6c61 7373 2c20 6275 7420 7468 6572   class, but ther
-000012f0: 6520 6172 6520 6365 7274 6169 6e20 7369  e are certain si
-00001300: 7475 6174 696f 6e73 2077 6865 6e20 6974  tuations when it
-00001310: 206d 6967 6874 2073 6176 6520 796f 7572   might save your
-00001320: 206c 6966 652e 204f 6e65 2073 7563 6820   life. One such 
-00001330: 6120 7363 656e 6172 696f 2069 7320 7768  a scenario is wh
-00001340: 656e 2079 6f75 2077 616e 7420 746f 2077  en you want to w
-00001350: 7269 7465 2061 6e20 696e 7465 7266 6163  rite an interfac
-00001360: 6520 746f 2061 2044 6565 7064 6963 7420  e to a Deepdict 
-00001370: 7468 6174 2067 6574 7320 6469 6e61 6d69  that gets dinami
-00001380: 6361 6c6c 7920 6765 6e65 7261 7465 6420  cally generated 
-00001390: 7275 6e74 696d 652c 206d 6561 6e69 6e67  runtime, meaning
-000013a0: 2c20 7468 6174 2074 6865 2063 6c61 7373  , that the class
-000013b0: 6573 2061 7265 2073 696d 706c 7920 6e6f  es are simply no
-000013c0: 7420 7072 6573 656e 7420 6174 2074 6865  t present at the
-000013d0: 2074 696d 6520 6f66 2077 7269 7469 6e67   time of writing
-000013e0: 2079 6f75 7220 6f77 6e20 636f 6465 2e20   your own code. 
-000013f0: 5468 6973 2069 7320 7768 656e 2061 2077  This is when a w
-00001400: 7261 7070 6572 2063 6f6d 6573 2068 616e  rapper comes han
-00001410: 6479 2e20 546f 2077 7261 7020 6120 6469  dy. To wrap a di
-00001420: 6374 696f 6e61 7279 2c20 646f 2074 6865  ctionary, do the
-00001430: 2066 6f6c 6c6f 7769 6e67 3a0a 0a60 6060   following:..```
-00001440: 7079 7468 6f6e 0a3e 3e3e 2066 726f 6d20  python.>>> from 
-00001450: 6465 776c 6f6f 7368 2e63 6f72 6520 696d  dewloosh.core im
-00001460: 706f 7274 2057 7261 7070 6572 0a3e 3e3e  port Wrapper.>>>
-00001470: 2064 6174 6120 3d20 7b27 6127 203a 207b   data = {'a' : {
-00001480: 2762 2720 3a20 7b27 6327 203a 207b 2765  'b' : {'c' : {'e
-00001490: 2720 3a20 337d 2c20 2764 2720 3a20 327d  ' : 3}, 'd' : 2}
-000014a0: 7d7d 0a3e 3e3e 2077 7261 7070 6572 203d  }}.>>> wrapper =
-000014b0: 2057 7261 7070 6572 2877 7261 703d 6461   Wrapper(wrap=da
-000014c0: 7461 2920 2020 0a60 6060 0a0a 5468 6520  ta)   .```..The 
-000014d0: 6057 7261 7070 6572 6020 636c 6173 7320  `Wrapper` class 
-000014e0: 6368 616e 6e65 6c73 2064 6f77 6e20 6576  channels down ev
-000014f0: 6572 7920 6361 6c6c 2074 6f20 7468 6520  ery call to the 
-00001500: 7772 6170 7065 6420 6f62 6a65 6374 2028  wrapped object (
-00001510: 696e 2074 6869 7320 6361 7365 2061 2064  in this case a d
-00001520: 6963 7469 6f6e 6172 7929 2c20 6966 2074  ictionary), if t
-00001530: 6865 206f 626a 6563 7420 7468 6174 2074  he object that t
-00001540: 6865 2063 616c 6c20 6973 206d 6164 6520  he call is made 
-00001550: 7570 6f6e 2069 7320 756e 6162 6c65 2074  upon is unable t
-00001560: 6f20 616e 7377 6572 2074 6865 2063 616c  o answer the cal
-00001570: 6c20 6279 2069 7473 656c 6620 2862 6563  l by itself (bec
-00001580: 6175 7365 2069 7420 6d69 7373 6573 2074  ause it misses t
-00001590: 6865 2077 616e 7465 6420 6174 7472 6962  he wanted attrib
-000015a0: 7574 6520 6f72 206d 6574 686f 6429 2e20  ute or method). 
-000015b0: 5468 6520 7772 6170 7065 6420 6f62 6a65  The wrapped obje
-000015c0: 6374 2069 7320 6163 6365 7373 6962 6c65  ct is accessible
-000015d0: 2074 6872 6f75 6768 2074 6865 2060 7772   through the `wr
-000015e0: 6170 7065 6460 2070 726f 7065 7274 7920  apped` property 
-000015f0: 6f66 2074 6865 2077 7261 7070 6572 2e0a  of the wrapper..
-00001600: 0a60 6060 7079 7468 6f6e 0a3e 3e3e 2077  .```python.>>> w
-00001610: 7261 7070 6572 2e77 7261 7070 6564 0a7b  rapper.wrapped.{
-00001620: 2761 273a 207b 2762 273a 207b 2763 273a  'a': {'b': {'c':
-00001630: 207b 2765 273a 2033 7d2c 2027 6427 3a20   {'e': 3}, 'd': 
-00001640: 327d 7d7d 0a60 6060 0a0a 4e6f 7465 2c20  2}}}.```..Note, 
-00001650: 7468 6174 2069 6620 666f 7220 736f 6d65  that if for some
-00001660: 2072 6561 736f 6e20 7765 2061 6363 6964   reason we accid
-00001670: 656e 7461 6c6c 7920 7368 6164 6f77 2061  entally shadow a
-00001680: 206d 6574 686f 6420 696e 2061 2062 6173   method in a bas
-00001690: 6520 636c 6173 7320 6c69 6b65 2074 6869  e class like thi
-000016a0: 733a 0a0a 6060 6070 7974 686f 6e0a 3e3e  s:..```python.>>
-000016b0: 3e20 636c 6173 7320 4375 7374 6f6d 5772  > class CustomWr
-000016c0: 6170 7065 7228 5772 6170 7065 7229 3a0a  apper(Wrapper):.
-000016d0: 3e3e 3e0a 3e3e 3e20 2020 2064 6566 2076  >>>.>>>    def v
-000016e0: 616c 7565 7328 7365 6c66 2c20 2a61 7267  alues(self, *arg
-000016f0: 732c 202a 2a6b 7761 7267 7329 3a0a 3e3e  s, **kwargs):.>>
-00001700: 3e20 2020 2020 2020 2072 6574 7572 6e20  >        return 
-00001710: 4e6f 6e65 0a60 6060 0a0a 4964 2077 6520  None.```..Id we 
-00001720: 7472 6965 6420 746f 2077 7261 7020 6120  tried to wrap a 
-00001730: 6469 6374 696f 6e61 7279 206e 6f77 2c20  dictionary now, 
-00001740: 7468 6520 696d 706c 656d 656e 7461 7469  the implementati
-00001750: 6f6e 2077 6f75 6c64 2061 6c74 6572 2074  on would alter t
-00001760: 6865 2062 6168 6176 696f 7572 206f 6620  he bahaviour of 
-00001770: 7468 6520 7772 6170 7065 722c 206c 6561  the wrapper, lea
-00001780: 7669 6e67 2074 6865 2062 6568 6176 696f  ving the behavio
-00001790: 7572 206f 6620 7468 6520 7772 6170 7065  ur of the wrappe
-000017a0: 6420 6f62 6a65 6374 2070 7265 7365 7276  d object preserv
-000017b0: 6564 2061 6e64 2073 7469 6c6c 2061 6363  ed and still acc
-000017c0: 6573 7369 626c 6520 6173 2060 6043 7573  essible as ``Cus
-000017d0: 746f 6d57 7261 7070 6572 2877 7261 703d  tomWrapper(wrap=
-000017e0: 6461 7461 292e 7772 6170 7065 642e 7661  data).wrapped.va
-000017f0: 6c75 6573 2829 6060 2e0a 0a60 6060 7079  lues()``...```py
-00001800: 7468 6f6e 0a3e 3e3e 2043 7573 746f 6d57  thon.>>> CustomW
-00001810: 7261 7070 6572 2877 7261 703d 6461 7461  rapper(wrap=data
-00001820: 292e 7772 6170 7065 642e 7661 6c75 6573  ).wrapped.values
-00001830: 2829 0a64 6963 745f 7661 6c75 6573 285b  ().dict_values([
-00001840: 7b27 6227 3a20 7b27 6327 3a20 7b27 6527  {'b': {'c': {'e'
-00001850: 3a20 337d 2c20 2764 273a 2032 7d7d 5d29  : 3}, 'd': 2}}])
-00001860: 0a60 6060 0a0a 2323 2323 2041 6273 7472  .```..#### Abstr
-00001870: 6163 7420 436c 6173 7365 7320 616e 6420  act Classes and 
-00001880: 4d65 7461 7072 6f67 7261 6d6d 696e 670a  Metaprogramming.
-00001890: 0a54 6865 2073 7562 6d6f 6475 6c65 2060  .The submodule `
-000018a0: 6465 776c 6f6f 7368 2e63 6f72 652e 6162  dewloosh.core.ab
-000018b0: 6360 2070 726f 7669 6465 7320 7369 6d70  c` provides simp
-000018c0: 6c65 2063 6c61 7373 6573 2074 6f20 616c  le classes to al
-000018d0: 6c65 7669 6174 6520 736f 6d65 206f 6620  leviate some of 
-000018e0: 7468 6520 756e 7761 6e74 6564 2063 6f6e  the unwanted con
-000018f0: 7365 7175 656e 6365 7320 6f66 2074 6865  sequences of the
-00001900: 2064 796e 616d 6963 616c 6c79 2074 7970   dynamically typ
-00001910: 6564 206e 6174 7572 6520 6f66 2050 7974  ed nature of Pyt
-00001920: 686f 6e2e 204f 6e65 206f 6620 7375 6368  hon. One of such
-00001930: 2061 2073 6365 6e61 7269 6f73 2069 7320   a scenarios is 
-00001940: 7768 656e 2077 6520 7375 6263 6c61 7373  when we subclass
-00001950: 2061 6e6f 7468 6572 2063 6c61 7373 2066   another class f
-00001960: 726f 6d20 6120 7468 6972 642d 7061 7274  rom a third-part
-00001970: 7920 4465 6570 6469 6374 2c20 6265 6361  y Deepdict, beca
-00001980: 7573 6520 7765 2077 616e 7420 746f 2069  use we want to i
-00001990: 6e68 6572 6974 2074 6865 2066 756e 6374  nherit the funct
-000019a0: 696f 6e61 6c69 7479 2074 6865 7265 696e  ionality therein
-000019b0: 2e20 4275 7420 7468 6520 7374 7566 6620  . But the stuff 
-000019c0: 6973 2063 6f6d 706c 6963 6174 6564 2c20  is complicated, 
-000019d0: 616e 6420 7765 2070 726f 6261 626c 7920  and we probably 
-000019e0: 776f 756e 646e 2774 2077 616e 7420 746f  woundn't want to
-000019f0: 2067 6f20 7468 726f 7567 6820 616c 6c20   go through all 
-00001a00: 6f66 2069 742e 204e 6576 6572 7468 656c  of it. Neverthel
-00001a10: 6573 732c 2077 6520 7761 6e74 2074 6f20  ess, we want to 
-00001a20: 6d61 6b65 2073 7572 652c 2074 6861 7420  make sure, that 
-00001a30: 7765 2064 6f6e 2774 2062 7261 6b65 2074  we don't brake t
-00001a40: 6865 2069 6e6e 6572 2066 6c6f 7720 6f66  he inner flow of
-00001a50: 2074 6865 206f 626a 6563 7420 6174 2072   the object at r
-00001a60: 756e 7469 6d65 2c20 6279 206f 7665 7272  untime, by overr
-00001a70: 6964 696e 6720 736f 6d65 2065 7373 656e  iding some essen
-00001a80: 7469 616c 206d 6574 686f 6473 2c20 7368  tial methods, sh
-00001a90: 6164 6f77 696e 6720 7468 6520 6f72 6967  adowing the orig
-00001aa0: 696e 616c 2062 6568 6176 696f 7572 2e20  inal behaviour. 
-00001ab0: 4e6f 7420 6c69 6b65 2069 7420 776f 756c  Not like it woul
-00001ac0: 646e 2774 2073 686f 7720 7570 2072 756e  dn't show up run
-00001ad0: 7469 6d65 2073 6f6f 6e65 7220 6f72 206c  time sooner or l
-00001ae0: 6174 6572 2c20 6275 7420 7468 6973 206c  ater, but this l
-00001af0: 6561 7665 7320 7468 6520 646f 6f72 206f  eaves the door o
-00001b00: 7065 6e65 6420 666f 7220 6261 6420 636f  pened for bad co
-00001b10: 6465 2e20 4c75 636b 696c 792c 2074 6865  de. Luckily, the
-00001b20: 2070 726f 626c 656d 2063 616e 2062 6520   problem can be 
-00001b30: 736f 6c76 6564 2066 6169 726c 7920 6561  solved fairly ea
-00001b40: 7369 6c79 2077 6974 6820 736f 6d65 206d  sily with some m
-00001b50: 6574 6170 726f 6772 616d 6d69 6e67 2c20  etaprogramming, 
-00001b60: 616e 6420 7468 6520 6d65 7461 2073 7562  and the meta sub
-00001b70: 6d6f 6475 6c65 2070 726f 7669 6465 7320  module provides 
-00001b80: 616e 2061 6273 7472 6163 7420 636c 6173  an abstract clas
-00001b90: 7320 6041 4243 5f53 6166 6560 2074 6861  s `ABC_Safe` tha
-00001ba0: 7420 6361 6e20 6265 2075 7365 6420 6173  t can be used as
-00001bb0: 2061 2062 6173 6520 636c 6173 7320 6675   a base class fu
-00001bc0: 7274 6865 7220 646f 776e 2074 6865 206c  rther down the l
-00001bd0: 696e 652e 0a0a 5275 6e6e 696e 6720 7468  ine...Running th
-00001be0: 6520 666f 6c6c 6f77 696e 6720 636f 6465  e following code
-00001bf0: 2074 6872 6f77 7320 616e 2065 7272 6f72   throws an error
-00001c00: 2061 7420 6465 7369 676e 2074 696d 652c   at design time,
-00001c10: 2062 6563 6175 7365 2060 666f 6f60 2069   because `foo` i
-00001c20: 7320 616c 7265 6164 7920 696d 706c 656d  s already implem
-00001c30: 656e 7465 6420 696e 2074 6865 2070 6172  ented in the par
-00001c40: 656e 7420 636c 6173 733a 0a0a 6060 6070  ent class:..```p
-00001c50: 7974 686f 6e0a 3e3e 3e20 6672 6f6d 2064  ython.>>> from d
-00001c60: 6577 6c6f 6f73 682e 636f 7265 2e61 6263  ewloosh.core.abc
-00001c70: 2069 6d70 6f72 7420 4142 435f 5361 6665   import ABC_Safe
-00001c80: 0a3e 3e3e 200a 3e3e 3e20 636c 6173 7320  .>>> .>>> class 
-00001c90: 5061 7265 6e74 2841 4243 5f53 6166 6529  Parent(ABC_Safe)
-00001ca0: 3a0a 3e3e 3e20 2020 2020 6465 6620 666f  :.>>>     def fo
-00001cb0: 6f28 7365 6c66 293a 0a3e 3e3e 2020 2020  o(self):.>>>    
-00001cc0: 2020 2020 2070 6173 730a 3e3e 3e20 0a3e       pass.>>> .>
-00001cd0: 3e3e 2063 6c61 7373 2043 6869 6c64 2850  >> class Child(P
-00001ce0: 6172 656e 7429 3a0a 3e3e 3e20 2020 2020  arent):.>>>     
-00001cf0: 6465 6620 666f 6f28 7365 6c66 293a 0a3e  def foo(self):.>
-00001d00: 3e3e 2020 2020 2020 2020 2070 6173 730a  >>         pass.
-00001d10: 6060 600a 0a41 6e6f 7468 6572 2069 6d70  ```..Another imp
-00001d20: 6f72 7461 6e74 2073 6974 7561 7469 6f6e  ortant situation
-00001d30: 2061 7269 7365 7320 7769 7468 2061 6273   arises with abs
-00001d40: 7472 6163 7420 6d65 7468 6f64 732e 2050  tract methods. P
-00001d50: 7974 686f 6e20 7072 6f76 6964 6573 2061  ython provides a
-00001d60: 2064 6563 6f72 6174 6f72 2066 6f72 2074   decorator for t
-00001d70: 6869 7320 6f75 7420 6f66 2074 6865 2062  his out of the b
-00001d80: 6f78 2c20 6275 7420 6167 6169 6e2c 206e  ox, but again, n
-00001d90: 6f74 2069 6d70 6c65 6d65 6e74 6564 2061  ot implemented a
-00001da0: 6273 7472 6163 7420 6d65 7468 6f64 7320  bstract methods 
-00001db0: 6f6e 6c79 2073 686f 7720 7570 2061 7420  only show up at 
-00001dc0: 7275 6d74 696d 652c 2077 6869 6368 2063  rumtime, which c
-00001dd0: 616e 2065 6173 696c 7920 6265 206e 6f20  an easily be no 
-00001de0: 7469 6d65 2069 6e20 7468 6520 776f 726c  time in the worl
-00001df0: 6420 6f66 2069 6e74 6572 7072 6574 6564  d of interpreted
-00001e00: 206c 616e 6775 6167 6573 2e20 5468 6520   languages. The 
-00001e10: 6d65 7461 2073 7562 6d6f 6475 6c20 6973  meta submodul is
-00001e20: 2065 7175 6970 7065 6420 7769 7468 2061   equipped with a
-00001e30: 6e6f 7468 6572 2061 6273 7472 6163 7420  nother abstract 
-00001e40: 636c 6173 7320 6361 6c6c 6564 2060 4142  class called `AB
-00001e50: 435f 5374 726f 6e67 602c 2074 6861 7420  C_Strong`, that 
-00001e60: 6d61 6b65 7320 796f 7520 6162 6c65 2074  makes you able t
-00001e70: 6f20 6265 2069 6e66 6f72 6d65 6420 6162  o be informed ab
-00001e80: 6f75 7420 6d69 7373 696e 6720 6675 6e63  out missing func
-00001e90: 7469 6f6e 2069 6d70 6c65 6d65 6e74 6174  tion implementat
-00001ea0: 696f 6e73 206f 6620 6120 636c 6173 7320  ions of a class 
-00001eb0: 7269 6768 7420 6174 2064 6573 6967 6e20  right at design 
-00001ec0: 7469 6d65 2e20 4865 7265 2027 5374 726f  time. Here 'Stro
-00001ed0: 6e67 2720 7265 6665 7273 2074 6f20 7468  ng' refers to th
-00001ee0: 6520 7374 726f 6e67 6572 2072 6571 7569  e stronger requi
-00001ef0: 7265 6d65 6e74 2069 6d70 6f73 6564 206f  rement imposed o
-00001f00: 6e20 6162 7374 7261 6374 206d 6574 686f  n abstract metho
-00001f10: 6473 2e20 416e 2061 6273 7472 6163 7420  ds. An abstract 
-00001f20: 6d65 7468 6f64 2069 6e20 6120 6368 696c  method in a chil
-00001f30: 6420 636c 6173 7320 6973 2065 6974 6865  d class is eithe
-00001f40: 7220 696d 706c 656d 656e 7465 642c 206f  r implemented, o
-00001f50: 7220 6465 636f 7261 7465 6420 7769 7468  r decorated with
-00001f60: 2074 6865 2060 6162 7374 7261 6374 6d65   the `abstractme
-00001f70: 7468 6f64 6020 6465 636f 7261 746f 722c  thod` decorator,
-00001f80: 2077 6869 6368 2070 6173 7365 7320 7468   which passes th
-00001f90: 6520 6261 6c6c 2074 6f20 7468 6520 6e65  e ball to the ne
-00001fa0: 7874 2063 6869 6c64 2e20 4f62 7669 6f75  xt child. Obviou
-00001fb0: 736c 792c 2079 6f75 2064 6f6e 2774 2067  sly, you don't g
-00001fc0: 6574 2074 6f20 7275 6e74 696d 652c 2075  et to runtime, u
-00001fd0: 6e6c 6573 7320 796f 7520 696d 706c 656d  nless you implem
-00001fe0: 656e 7420 616c 6c20 7468 6520 7265 7175  ent all the requ
-00001ff0: 6972 6564 2061 6273 7472 6163 7420 636c  ired abstract cl
-00002000: 6173 7365 732e 2054 6869 7320 6973 2061  asses. This is a
-00002010: 6c73 6f20 7573 6566 756c 2069 6620 7765  lso useful if we
-00002020: 2077 616e 7420 746f 2063 7265 6174 6520   want to create 
-00002030: 6120 7465 6d70 6c61 7465 206f 626a 6563  a template objec
-00002040: 742c 2074 6861 7420 7072 6f76 6964 6573  t, that provides
-00002050: 2069 6e73 7472 7563 7469 6f6e 7320 6f6e   instructions on
-00002060: 2068 6f77 2074 6f20 636f 6d70 6c65 7465   how to complete
-00002070: 2061 2073 6b65 6c65 746f 6e20 746f 2068   a skeleton to h
-00002080: 6176 6520 6120 776f 726b 696e 6720 736f  ave a working so
-00002090: 6c75 7469 6f6e 2e20 4120 7369 6d70 6c65  lution. A simple
-000020a0: 2065 7861 6d70 6c65 2074 6f20 696c 6c75   example to illu
-000020b0: 7374 7261 7465 2077 6861 7420 6861 7070  strate what happ
-000020c0: 656e 7320 6966 2079 6f75 2062 7261 6b65  ens if you brake
-000020d0: 2074 6865 2072 756c 6573 2069 7320 7468   the rules is th
-000020e0: 6520 666f 6c6c 6f77 696e 673a 0a0a 6060  e following:..``
-000020f0: 6070 7974 686f 6e0a 3e3e 3e20 6672 6f6d  `python.>>> from
-00002100: 2064 6577 6c6f 6f73 682e 636f 7265 2e61   dewloosh.core.a
-00002110: 6263 2069 6d70 6f72 7420 4142 435f 5374  bc import ABC_St
-00002120: 726f 6e67 0a3e 3e3e 200a 3e3e 3e20 636c  rong.>>> .>>> cl
-00002130: 6173 7320 5061 7265 6e74 2841 4243 5f53  ass Parent(ABC_S
-00002140: 7472 6f6e 6729 3a0a 3e3e 3e20 2020 2020  trong):.>>>     
-00002150: 4061 6273 7472 6163 746d 6574 686f 6420  @abstractmethod 
-00002160: 2020 200a 3e3e 3e20 2020 2020 6465 6620     .>>>     def 
-00002170: 666f 6f28 7365 6c66 293a 0a3e 3e3e 2020  foo(self):.>>>  
-00002180: 2020 2020 2020 2070 6173 730a 3e3e 3e20         pass.>>> 
-00002190: 0a3e 3e3e 2063 6c61 7373 2043 6869 6c64  .>>> class Child
-000021a0: 2850 6172 656e 7429 3a0a 3e3e 3e20 2020  (Parent):.>>>   
-000021b0: 2020 2e2e 2e0a 6060 600a 0a23 2323 2320    ....```..#### 
-000021c0: 4162 7374 7261 6374 2043 6c61 7373 2050  Abstract Class P
-000021d0: 726f 7065 7274 6965 730a 0a41 6c6f 6e67  roperties..Along
-000021e0: 2074 6865 2073 616d 6520 7468 6f75 6768   the same though
-000021f0: 7473 2c20 736f 6d65 7469 6d65 7320 7765  ts, sometimes we
-00002200: 2077 616e 7420 746f 2065 6e73 7572 6520   want to ensure 
-00002210: 7468 6520 6578 6973 7465 6e63 6520 6f66  the existence of
-00002220: 2073 6f6d 6520 636c 6173 730a 7072 6f70   some class.prop
-00002230: 6572 7469 6573 2077 6865 6e20 6275 696c  erties when buil
-00002240: 6469 6e67 2063 6f6d 706c 6578 206f 626a  ding complex obj
-00002250: 6563 7473 2077 6974 6820 6d75 6c74 6970  ects with multip
-00002260: 6c65 2062 6173 6520 636c 6173 7365 732e  le base classes.
-00002270: 2054 6869 7320 6361 6e20 6265 2064 6f6e   This can be don
-00002280: 6520 7573 696e 6720 6120 7370 6563 6961  e using a specia
-00002290: 6c20 6465 636f 7261 746f 723a 0a0a 6060  l decorator:..``
-000022a0: 6070 7974 686f 6e0a 3e3e 3e20 6672 6f6d  `python.>>> from
-000022b0: 2064 6577 6c6f 6f73 682e 636f 7265 2e61   dewloosh.core.a
-000022c0: 6370 2069 6d70 6f72 7420 6162 7374 7261  cp import abstra
-000022d0: 6374 5f63 6c61 7373 5f70 726f 7065 7274  ct_class_propert
-000022e0: 790a 3e3e 3e20 6672 6f6d 2061 6263 2069  y.>>> from abc i
-000022f0: 6d70 6f72 7420 4142 430a 3e3e 3e20 0a3e  mport ABC.>>> .>
-00002300: 3e3e 2040 6162 7374 7261 6374 5f63 6c61  >> @abstract_cla
-00002310: 7373 5f70 726f 7065 7274 7928 7072 6f70  ss_property(prop
-00002320: 313d 696e 742c 2070 726f 7032 3d66 6c6f  1=int, prop2=flo
-00002330: 6174 7d29 0a3e 3e3e 2063 6c61 7373 2042  at}).>>> class B
-00002340: 6173 6543 6c61 7373 4128 4142 4329 3a0a  aseClassA(ABC):.
-00002350: 3e3e 3e20 0a3e 3e3e 2020 2020 2070 726f  >>> .>>>     pro
-00002360: 7031 3a20 696e 740a 3e3e 3e20 2020 2020  p1: int.>>>     
-00002370: 7072 6f70 323a 206c 6973 740a 3e3e 3e20  prop2: list.>>> 
-00002380: 0a3e 3e3e 2020 2020 2064 6566 205f 5f69  .>>>     def __i
-00002390: 6e69 745f 5f28 7365 6c66 293a 0a3e 3e3e  nit__(self):.>>>
-000023a0: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
-000023b0: 6f70 3220 3d20 5b33 2c20 345d 0a3e 3e3e  op2 = [3, 4].>>>
-000023c0: 2020 2020 2020 2020 2073 7570 6572 2829           super()
-000023d0: 2e5f 5f69 6e69 745f 5f28 290a 3e3e 3e20  .__init__().>>> 
-000023e0: 2020 2020 2020 2020 7265 7475 726e 0a60          return.`
-000023f0: 6060 0a0a 2323 2323 2049 6e66 6978 204f  ``..#### Infix O
-00002400: 7065 7261 746f 7273 0a0a 496e 6669 7820  perators..Infix 
-00002410: 6f70 6572 6174 6f72 7320 616c 6c6f 7720  operators allow 
-00002420: 666f 7220 6120 6661 6e63 7920 7761 7920  for a fancy way 
-00002430: 6f66 2064 6566 696e 696e 6720 6269 6e61  of defining bina
-00002440: 7279 206f 7065 7261 7469 6f6e 7320 7573  ry operations us
-00002450: 696e 6720 7468 6520 6f70 6572 6174 6f72  ing the operator
-00002460: 7320 273c 3c27 2c20 273e 3e27 2061 6e64  s '<<', '>>' and
-00002470: 2027 7c27 2e0a 0a60 6060 7079 7468 6f6e   '|'...```python
-00002480: 0a3e 3e3e 2066 726f 6d20 6465 776c 6f6f  .>>> from dewloo
-00002490: 7368 2e63 6f72 652e 696e 6669 7820 696d  sh.core.infix im
-000024a0: 706f 7274 2049 6e66 6978 0a3e 3e3e 200a  port Infix.>>> .
-000024b0: 3e3e 3e20 6d75 6c20 3d20 496e 6669 7828  >>> mul = Infix(
-000024c0: 6c61 6d62 6461 2078 2c20 793a 2078 202a  lambda x, y: x *
-000024d0: 2079 290a 3e3e 3e20 3220 7c20 6d75 6c20   y).>>> 2 | mul 
-000024e0: 7c20 340a 380a 3e3e 3e20 6164 6420 3d20  | 4.8.>>> add = 
-000024f0: 496e 6669 7828 6c61 6d62 6461 2078 2c20  Infix(lambda x, 
-00002500: 793a 2078 202b 2079 290a 3e3e 3e20 3220  y: x + y).>>> 2 
-00002510: 3c3c 2061 6464 203e 3e20 340a 360a 6060  << add >> 4.6.``
-00002520: 600a 0a23 2320 2a2a 496e 7374 616c 6c61  `..## **Installa
-00002530: 7469 6f6e 2a2a 0a54 6869 7320 6973 206f  tion**.This is o
-00002540: 7074 696f 6e61 6c2c 2062 7574 2077 6520  ptional, but we 
-00002550: 7375 6767 6573 7420 796f 7520 746f 2063  suggest you to c
-00002560: 7265 6174 6520 6120 6465 6469 6361 7465  reate a dedicate
-00002570: 6420 7669 7274 7561 6c20 656e 7669 726f  d virtual enviro
-00002580: 6d65 6e74 2061 7420 616c 6c20 7469 6d65  ment at all time
-00002590: 7320 746f 2061 766f 6964 2063 6f6e 666c  s to avoid confl
-000025a0: 6963 7473 2077 6974 6820 796f 7572 206f  icts with your o
-000025b0: 7468 6572 2070 726f 6a65 6374 732e 2043  ther projects. C
-000025c0: 7265 6174 6520 6120 666f 6c64 6572 2c20  reate a folder, 
-000025d0: 6f70 656e 2061 2063 6f6d 6d61 6e64 2073  open a command s
-000025e0: 6865 6c6c 2069 6e20 7468 6174 2066 6f6c  hell in that fol
-000025f0: 6465 7220 616e 6420 7573 6520 7468 6520  der and use the 
-00002600: 666f 6c6c 6f77 696e 6720 636f 6d6d 616e  following comman
-00002610: 640a 0a60 6060 636f 6e73 6f6c 650a 3e3e  d..```console.>>
-00002620: 3e20 7079 7468 6f6e 202d 6d20 7665 6e76  > python -m venv
-00002630: 2076 656e 765f 6e61 6d65 0a60 6060 0a0a   venv_name.```..
-00002640: 4f6e 6365 2074 6865 2065 6e76 6972 6f6d  Once the envirom
-00002650: 656e 7420 6973 2063 7265 6174 6564 2c20  ent is created, 
-00002660: 6163 7469 7661 7465 2069 7420 7669 6120  activate it via 
-00002670: 7479 7069 6e67 0a0a 6060 6063 6f6e 736f  typing..```conso
-00002680: 6c65 0a3e 3e3e 202e 5c76 656e 765f 6e61  le.>>> .\venv_na
-00002690: 6d65 5c53 6372 6970 7473 5c61 6374 6976  me\Scripts\activ
-000026a0: 6174 650a 6060 600a 0a60 6465 776c 6f6f  ate.```..`dewloo
-000026b0: 7368 2e63 6f72 6560 2063 616e 2062 6520  sh.core` can be 
-000026c0: 696e 7374 616c 6c65 6420 2865 6974 6865  installed (eithe
-000026d0: 7220 696e 2061 2076 6972 7475 616c 2065  r in a virtual e
-000026e0: 6e76 6972 6f6d 656e 7420 6f72 2067 6c6f  nviroment or glo
-000026f0: 6261 6c6c 7929 2066 726f 6d20 5079 5049  bally) from PyPI
-00002700: 2075 7369 6e67 2060 7069 7060 206f 6e20   using `pip` on 
-00002710: 5079 7468 6f6e 203e 3d20 332e 363a 0a0a  Python >= 3.6:..
-00002720: 6060 6063 6f6e 736f 6c65 0a3e 3e3e 2070  ```console.>>> p
-00002730: 6970 2069 6e73 7461 6c6c 2064 6577 6c6f  ip install dewlo
-00002740: 6f73 682e 636f 7265 0a60 6060 0a0a 2323  osh.core.```..##
-00002750: 202a 2a54 6573 7469 6e67 2a2a 0a0a 546f   **Testing**..To
-00002760: 2072 756e 2061 6c6c 2074 6573 7473 2c20   run all tests, 
-00002770: 6f70 656e 2075 7020 6120 636f 6e73 6f6c  open up a consol
-00002780: 6520 696e 2074 6865 2072 6f6f 7420 6469  e in the root di
-00002790: 7265 6374 6f72 7920 6f66 2074 6865 2070  rectory of the p
-000027a0: 726f 6a65 6374 2061 6e64 2074 7970 6520  roject and type 
-000027b0: 7468 6520 666f 6c6c 6f77 696e 670a 0a60  the following..`
-000027c0: 6060 636f 6e73 6f6c 650a 3e3e 3e20 7079  ``console.>>> py
-000027d0: 7468 6f6e 202d 6d20 756e 6974 7465 7374  thon -m unittest
-000027e0: 0a60 6060 0a0a 2323 202a 2a44 6570 656e  .```..## **Depen
-000027f0: 6465 6e63 6965 732a 2a0a 0a54 6865 2070  dencies**..The p
-00002800: 6163 6b61 6765 2068 6173 206e 6f20 6465  ackage has no de
-00002810: 7065 6e64 656e 6369 6573 2e0a 0a23 2320  pendencies...## 
-00002820: 2a2a 4c69 6365 6e73 652a 2a0a 0a54 6869  **License**..Thi
-00002830: 7320 7061 636b 6167 6520 6973 206c 6963  s package is lic
-00002840: 656e 7365 6420 756e 6465 7220 7468 6520  ensed under the 
-00002850: 4d49 5420 6c69 6365 6e73 652e 0a0a       MIT license...
+00000000: 5b21 5b42 696e 6465 725d 2868 7474 7073  [![Binder](https
+00000010: 3a2f 2f6d 7962 696e 6465 722e 6f72 672f  ://mybinder.org/
+00000020: 6261 6467 655f 6c6f 676f 2e73 7667 295d  badge_logo.svg)]
+00000030: 2868 7474 7073 3a2f 2f6d 7962 696e 6465  (https://mybinde
+00000040: 722e 6f72 672f 7632 2f67 682f 6465 776c  r.org/v2/gh/dewl
+00000050: 6f6f 7368 2f64 6577 6c6f 6f73 682d 636f  oosh/dewloosh-co
+00000060: 7265 2f6d 6169 6e3f 6c61 6270 6174 683d  re/main?labpath=
+00000070: 6578 616d 706c 6573 2532 4662 6173 6963  examples%2Fbasic
+00000080: 732e 6970 796e 623f 7572 6c70 6174 683d  s.ipynb?urlpath=
+00000090: 6c61 6229 0d0a 5b21 5b43 6972 636c 6543  lab)..[![CircleC
+000000a0: 495d 2868 7474 7073 3a2f 2f63 6972 636c  I](https://circl
+000000b0: 6563 692e 636f 6d2f 6768 2f64 6577 6c6f  eci.com/gh/dewlo
+000000c0: 6f73 682f 6465 776c 6f6f 7368 2d63 6f72  osh/dewloosh-cor
+000000d0: 652e 7376 673f 7374 796c 653d 7368 6965  e.svg?style=shie
+000000e0: 6c64 295d 2868 7474 7073 3a2f 2f63 6972  ld)](https://cir
+000000f0: 636c 6563 692e 636f 6d2f 6768 2f64 6577  cleci.com/gh/dew
+00000100: 6c6f 6f73 682f 6465 776c 6f6f 7368 2d63  loosh/dewloosh-c
+00000110: 6f72 6529 200d 0a5b 215b 446f 6375 6d65  ore) ..[![Docume
+00000120: 6e74 6174 696f 6e20 5374 6174 7573 5d28  ntation Status](
+00000130: 6874 7470 733a 2f2f 7265 6164 7468 6564  https://readthed
+00000140: 6f63 732e 6f72 672f 7072 6f6a 6563 7473  ocs.org/projects
+00000150: 2f64 6577 6c6f 6f73 682d 636f 7265 2f62  /dewloosh-core/b
+00000160: 6164 6765 2f3f 7665 7273 696f 6e3d 6c61  adge/?version=la
+00000170: 7465 7374 295d 2868 7474 7073 3a2f 2f6e  test)](https://n
+00000180: 6464 6963 742e 7265 6164 7468 6564 6f63  ddict.readthedoc
+00000190: 732e 696f 2f65 6e2f 6c61 7465 7374 2f3f  s.io/en/latest/?
+000001a0: 6261 6467 653d 6c61 7465 7374 2920 0d0a  badge=latest) ..
+000001b0: 5b21 5b4c 6963 656e 7365 5d28 6874 7470  [![License](http
+000001c0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+000001d0: 696f 2f62 6164 6765 2f4c 6963 656e 7365  io/badge/License
+000001e0: 2d4d 4954 2d79 656c 6c6f 772e 7376 6729  -MIT-yellow.svg)
+000001f0: 5d28 6874 7470 733a 2f2f 6f70 656e 736f  ](https://openso
+00000200: 7572 6365 2e6f 7267 2f6c 6963 656e 7365  urce.org/license
+00000210: 732f 4d49 5429 0d0a 5b21 5b50 7950 495d  s/MIT)..[![PyPI]
+00000220: 2868 7474 7073 3a2f 2f62 6164 6765 2e66  (https://badge.f
+00000230: 7572 792e 696f 2f70 792f 6465 776c 6f6f  ury.io/py/dewloo
+00000240: 7368 2e63 6f72 652e 7376 6729 5d28 6874  sh.core.svg)](ht
+00000250: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
+00000260: 726f 6a65 6374 2f64 6577 6c6f 6f73 682e  roject/dewloosh.
+00000270: 636f 7265 2920 0d0a 0d0a 2320 2a2a 6465  core) ....# **de
+00000280: 776c 6f6f 7368 2e63 6f72 652a 2a0d 0a0d  wloosh.core**...
+00000290: 0a54 6869 7320 7061 636b 6167 6520 636f  .This package co
+000002a0: 6e74 6169 6e73 2063 6f6d 6d6f 6e20 6465  ntains common de
+000002b0: 7665 6c6f 7065 7220 7574 696c 6974 6965  veloper utilitie
+000002c0: 7320 746f 2073 7570 706f 7274 206f 7468  s to support oth
+000002d0: 6572 2060 6465 776c 6f6f 7368 6020 736f  er `dewloosh` so
+000002e0: 6c75 7469 6f6e 732e 2045 7665 7279 7468  lutions. Everyth
+000002f0: 696e 6720 6973 2070 7572 6520 5079 7468  ing is pure Pyth
+00000300: 6f6e 2c20 7468 6520 7061 636b 6167 6520  on, the package 
+00000310: 7265 7175 6972 6573 206e 6f20 6578 7472  requires no extr
+00000320: 6120 6465 7065 6e64 656e 6369 6573 2061  a dependencies a
+00000330: 6e64 2073 686f 756c 6420 7275 6e20 6f6e  nd should run on
+00000340: 2061 206d 696e 696d 616c 2073 6574 7570   a minimal setup
+00000350: 2e0d 0a0d 0a54 6865 206d 6f73 7420 696d  .....The most im
+00000360: 706f 7274 616e 7420 6665 6174 7572 6573  portant features
+00000370: 3a0d 0a0d 0a2a 2056 6172 696f 7573 2064  :....* Various d
+00000380: 6963 7469 6f6e 6172 7920 636c 6173 7365  ictionary classe
+00000390: 7320 7468 6174 2065 6e68 616e 6365 2074  s that enhance t
+000003a0: 6865 2063 6f72 6520 6265 6861 7669 6f75  he core behaviou
+000003b0: 7220 6f66 2074 6865 2062 7569 6c74 2d69  r of the built-i
+000003c0: 6e20 6064 6963 7460 2074 7970 652e 2054  n `dict` type. T
+000003d0: 6865 2074 6f70 206f 6620 7468 6520 6361  he top of the ca
+000003e0: 6b65 2069 7320 7468 6520 6044 6565 7044  ke is the `DeepD
+000003f0: 6963 7460 2063 6c61 7373 2c20 7768 6963  ict` class, whic
+00000400: 6820 6f66 6665 7273 2061 2064 6966 6665  h offers a diffe
+00000410: 7265 6e74 2062 6568 6176 696f 7572 2066  rent behaviour f
+00000420: 6f72 206e 6573 7465 6420 6469 6374 696f  or nested dictio
+00000430: 6e61 7269 6573 2062 7920 6170 706c 7969  naries by applyi
+00000440: 6e67 2061 2073 656c 6620 7265 706c 6963  ng a self replic
+00000450: 6174 696e 6720 6465 6661 6c74 2066 6163  ating defalt fac
+00000460: 746f 7279 2e0d 0a0d 0a2a 2041 2073 6574  tory.....* A set
+00000470: 206f 6620 746f 6f6c 7320 666f 7220 6d65   of tools for me
+00000480: 7461 7072 6f67 7261 6d6d 696e 672e 2054  taprogramming. T
+00000490: 6865 2075 7365 2063 6173 6573 2069 6e63  he use cases inc
+000004a0: 6c75 6465 2064 6563 6c61 7269 6e67 2063  lude declaring c
+000004b0: 7573 746f 6d20 6162 7374 7261 6374 2063  ustom abstract c
+000004c0: 6c61 7373 2070 726f 7065 7274 6965 732c  lass properties,
+000004d0: 2075 7369 6e67 206d 6574 6163 6c61 7373   using metaclass
+000004e0: 6573 2074 6f20 6176 6f69 6420 756e 7761  es to avoid unwa
+000004f0: 6e74 6564 2063 6f64 6520 636f 6e66 6c69  nted code confli
+00000500: 6374 732c 2061 7373 7572 696e 6720 7468  cts, assuring th
+00000510: 6520 696d 706c 656d 656e 7461 7469 6f6e  e implementation
+00000520: 206f 6620 6162 7374 7261 6374 206d 6574   of abstract met
+00000530: 686f 6473 2061 7420 6465 7369 676e 2074  hods at design t
+00000540: 696d 652c 2065 7463 2e0d 0a0d 0a2a 2044  ime, etc.....* D
+00000550: 6563 6f72 6174 6f72 732c 2077 7261 7070  ecorators, wrapp
+00000560: 6572 7320 616e 6420 6f74 6865 7220 6861  ers and other ha
+00000570: 6e64 7920 6465 7665 6c6f 7065 7220 746f  ndy developer to
+00000580: 6f6c 732e 0d0a 0d0a 2323 202a 2a44 6f63  ols.....## **Doc
+00000590: 756d 656e 7461 7469 6f6e 2a2a 0d0a 0d0a  umentation**....
+000005a0: 436c 6963 6b20 5b68 6572 655d 2868 7474  Click [here](htt
+000005b0: 7073 3a2f 2f64 6577 6c6f 6f73 682d 636f  ps://dewloosh-co
+000005c0: 7265 2e72 6561 6474 6865 646f 6373 2e69  re.readthedocs.i
+000005d0: 6f2f 656e 2f6c 6174 6573 742f 2920 746f  o/en/latest/) to
+000005e0: 2072 6561 6420 7468 6520 646f 6375 6d65   read the docume
+000005f0: 6e74 6174 696f 6e2e 0d0a 0d0a 2323 202a  ntation.....## *
+00000600: 2a49 6e73 7461 6c6c 6174 696f 6e2a 2a0d  *Installation**.
+00000610: 0a54 6869 7320 6973 206f 7074 696f 6e61  .This is optiona
+00000620: 6c2c 2062 7574 2077 6520 7375 6767 6573  l, but we sugges
+00000630: 7420 796f 7520 746f 2063 7265 6174 6520  t you to create 
+00000640: 6120 6465 6469 6361 7465 6420 7669 7274  a dedicated virt
+00000650: 7561 6c20 656e 7669 726f 6d65 6e74 2061  ual enviroment a
+00000660: 7420 616c 6c20 7469 6d65 7320 746f 2061  t all times to a
+00000670: 766f 6964 2063 6f6e 666c 6963 7473 2077  void conflicts w
+00000680: 6974 6820 796f 7572 206f 7468 6572 2070  ith your other p
+00000690: 726f 6a65 6374 732e 2043 7265 6174 6520  rojects. Create 
+000006a0: 6120 666f 6c64 6572 2c20 6f70 656e 2061  a folder, open a
+000006b0: 2063 6f6d 6d61 6e64 2073 6865 6c6c 2069   command shell i
+000006c0: 6e20 7468 6174 2066 6f6c 6465 7220 616e  n that folder an
+000006d0: 6420 7573 6520 7468 6520 666f 6c6c 6f77  d use the follow
+000006e0: 696e 6720 636f 6d6d 616e 640d 0a0d 0a60  ing command....`
+000006f0: 6060 636f 6e73 6f6c 650d 0a3e 3e3e 2070  ``console..>>> p
+00000700: 7974 686f 6e20 2d6d 2076 656e 7620 7665  ython -m venv ve
+00000710: 6e76 5f6e 616d 650d 0a60 6060 0d0a 0d0a  nv_name..```....
+00000720: 4f6e 6365 2074 6865 2065 6e76 6972 6f6d  Once the envirom
+00000730: 656e 7420 6973 2063 7265 6174 6564 2c20  ent is created, 
+00000740: 6163 7469 7661 7465 2069 7420 7669 6120  activate it via 
+00000750: 7479 7069 6e67 0d0a 0d0a 6060 6063 6f6e  typing....```con
+00000760: 736f 6c65 0d0a 3e3e 3e20 2e5c 7665 6e76  sole..>>> .\venv
+00000770: 5f6e 616d 655c 5363 7269 7074 735c 6163  _name\Scripts\ac
+00000780: 7469 7661 7465 0d0a 6060 600d 0a0d 0a60  tivate..```....`
+00000790: 6465 776c 6f6f 7368 2e63 6f72 6560 2063  dewloosh.core` c
+000007a0: 616e 2062 6520 696e 7374 616c 6c65 6420  an be installed 
+000007b0: 2865 6974 6865 7220 696e 2061 2076 6972  (either in a vir
+000007c0: 7475 616c 2065 6e76 6972 6f6d 656e 7420  tual enviroment 
+000007d0: 6f72 2067 6c6f 6261 6c6c 7929 2066 726f  or globally) fro
+000007e0: 6d20 5079 5049 2075 7369 6e67 2060 7069  m PyPI using `pi
+000007f0: 7060 206f 6e20 5079 7468 6f6e 203e 3d20  p` on Python >= 
+00000800: 332e 363a 0d0a 0d0a 6060 6063 6f6e 736f  3.6:....```conso
+00000810: 6c65 0d0a 3e3e 3e20 7069 7020 696e 7374  le..>>> pip inst
+00000820: 616c 6c20 6465 776c 6f6f 7368 2e63 6f72  all dewloosh.cor
+00000830: 650d 0a60 6060 0d0a 0d0a 2323 202a 2a43  e..```....## **C
+00000840: 7261 7368 2043 6f75 7273 652a 2a0d 0a0d  rash Course**...
+00000850: 0a23 2323 2320 4469 6374 696f 6e61 7269  .#### Dictionari
+00000860: 6573 206f 6620 6469 6374 696f 6e61 7269  es of dictionari
+00000870: 6573 206f 6620 6469 6163 7469 6f6e 6172  es of diactionar
+00000880: 6965 7320 6f66 202e 2e2e 0d0a 0d0a 496e  ies of .......In
+00000890: 2065 7665 7279 2063 6173 6520 7768 6572   every case wher
+000008a0: 6520 796f 7527 6420 7761 6e74 2074 6f20  e you'd want to 
+000008b0: 7573 6520 6120 6064 6963 7460 2c20 796f  use a `dict`, yo
+000008c0: 7520 6361 6e20 7573 6520 6120 6044 6565  u can use a `Dee
+000008d0: 7064 6963 7460 2061 7320 6120 6472 6f70  pdict` as a drop
+000008e0: 2d69 6e20 7265 706c 6163 656d 656e 742c  -in replacement,
+000008f0: 2062 7574 206f 6e20 746f 7020 6f66 2077   but on top of w
+00000900: 6861 7420 6120 7369 6d70 6c65 2064 6963  hat a simple dic
+00000910: 7469 6f6e 6172 7920 7072 6f76 6964 6573  tionary provides
+00000920: 2c20 6120 6044 6565 7064 6963 7460 2069  , a `Deepdict` i
+00000930: 7320 6d6f 7265 2063 6170 6162 6c65 2c20  s more capable, 
+00000940: 6173 2069 7420 7072 6f76 6964 6573 2061  as it provides a
+00000950: 206d 6163 6869 6e65 7279 2074 6f20 6861   machinery to ha
+00000960: 6e64 6c65 206e 6573 7465 6420 6c61 796f  ndle nested layo
+00000970: 7574 732e 2049 7420 6973 2062 6173 6963  uts. It is basic
+00000980: 616c 6c79 2061 6e20 6f72 6465 7265 6420  ally an ordered 
+00000990: 6064 6566 6175 6c74 6469 6374 6020 7769  `defaultdict` wi
+000009a0: 7468 2061 2073 656c 6620 7265 706c 6963  th a self replic
+000009b0: 6174 696e 6720 6465 6661 756c 7420 6661  ating default fa
+000009c0: 6374 6f72 792e 200d 0a0d 0a60 6060 7079  ctory. ....```py
+000009d0: 7468 6f6e 0d0a 3e3e 3e20 6672 6f6d 2064  thon..>>> from d
+000009e0: 6577 6c6f 6f73 682e 636f 7265 2069 6d70  ewloosh.core imp
+000009f0: 6f72 7420 4465 6570 6469 6374 0d0a 3e3e  ort Deepdict..>>
+00000a00: 3e20 6461 7461 203d 2044 6565 7064 6963  > data = Deepdic
+00000a10: 7428 290d 0a60 6060 0d0a 0d0a 4120 6044  t()..```....A `D
+00000a20: 6565 7064 6963 7460 2069 7320 6573 7365  eepdict` is esse
+00000a30: 6e74 6961 6c6c 7920 6120 6e65 7374 6564  ntially a nested
+00000a40: 2064 6566 6175 6c74 2064 6963 7469 6f6e   default diction
+00000a50: 6172 792e 2042 6569 6e67 206e 6573 7465  ary. Being neste
+00000a60: 6420 7265 6665 7273 2074 6f20 7468 6520  d refers to the 
+00000a70: 6661 6374 2074 6861 7420 796f 7520 6361  fact that you ca
+00000a80: 6e20 646f 2074 6869 733a 0d0a 0d0a 6060  n do this:....``
+00000a90: 6070 7974 686f 6e0d 0a3e 3e3e 2064 6174  `python..>>> dat
+00000aa0: 615b 2761 275d 5b27 6227 5d5b 2763 275d  a['a']['b']['c']
+00000ab0: 5b27 6527 5d20 3d20 310d 0a3e 3e3e 2064  ['e'] = 1..>>> d
+00000ac0: 6174 615b 2761 275d 5b27 6227 5d5b 2764  ata['a']['b']['d
+00000ad0: 275d 203d 2032 0d0a 6060 600d 0a0d 0a4e  '] = 2..```....N
+00000ae0: 6f74 6963 6520 7468 6174 2074 6865 206f  otice that the o
+00000af0: 626a 6563 7420 6361 7276 6573 2061 2077  bject carves a w
+00000b00: 6179 2075 7020 756e 7469 6c20 7468 6520  ay up until the 
+00000b10: 6c61 7374 206b 6579 2c20 7769 7468 6f75  last key, withou
+00000b20: 7420 6e65 6564 696e 6720 746f 2063 7265  t needing to cre
+00000b30: 6174 6520 6561 6368 206c 6576 656c 2065  ate each level e
+00000b40: 7870 6c69 6369 746c 792e 2057 6861 7420  xplicitly. What 
+00000b50: 6861 7070 656e 7320 6973 2074 6861 7420  happens is that 
+00000b60: 6576 6572 7920 7469 6d65 2061 206b 6579  every time a key
+00000b70: 2069 7320 6d69 7373 696e 6720 696e 2061   is missing in a
+00000b80: 2060 6461 7461 602c 2074 6865 206f 626a   `data`, the obj
+00000b90: 6563 7420 6372 6561 7465 7320 6120 6e65  ect creates a ne
+00000ba0: 7720 696e 7374 616e 6365 2c20 7768 6963  w instance, whic
+00000bb0: 6820 7468 656e 2069 7320 616c 736f 2072  h then is also r
+00000bc0: 6561 6479 2074 6f20 6861 6e64 6c65 206d  eady to handle m
+00000bd0: 6973 7369 6e67 206b 6579 7320 6f72 2064  issing keys or d
+00000be0: 6174 612e 2041 6363 6573 7369 6e67 206e  ata. Accessing n
+00000bf0: 6573 7465 6420 7375 6264 6963 7469 6f6e  ested subdiction
+00000c00: 6172 6965 7320 776f 726b 7320 696e 2061  aries works in a
+00000c10: 2073 696d 696c 6172 2066 6173 6869 6f6e   similar fashion
+00000c20: 3a0d 0a0d 0a60 6060 7079 7468 6f6e 0d0a  :....```python..
+00000c30: 3e3e 3e20 6461 7461 5b27 6127 5d5b 2762  >>> data['a']['b
+00000c40: 275d 5b27 6327 5d5b 2765 275d 0d0a 310d  ']['c']['e']..1.
+00000c50: 0a60 6060 0d0a 546f 2061 6c6c 6f77 2066  .```..To allow f
+00000c60: 6f72 2061 206d 6f72 6520 5079 7468 6f6e  or a more Python
+00000c70: 6963 2066 6565 6c2c 2069 7420 616c 736f  ic feel, it also
+00000c80: 2073 7570 706f 7274 7320 6172 7261 792d   supports array-
+00000c90: 6c69 6b65 2069 6e64 6578 696e 672c 2073  like indexing, s
+00000ca0: 6f20 7468 6174 2074 6865 2066 6f6c 6c6f  o that the follo
+00000cb0: 7769 6e67 206f 7065 7261 7469 6f6e 7320  wing operations 
+00000cc0: 6172 6520 7661 6c69 643a 200d 0a0d 0a60  are valid: ....`
+00000cd0: 6060 7079 7468 6f6e 0d0a 3e3e 3e20 6461  ``python..>>> da
+00000ce0: 7461 5b27 6127 2c20 2762 272c 2027 6327  ta['a', 'b', 'c'
+00000cf0: 2c20 2765 275d 203d 2033 0d0a 3e3e 3e20  , 'e'] = 3..>>> 
+00000d00: 6461 7461 5b27 6127 2c20 2762 272c 2027  data['a', 'b', '
+00000d10: 6327 2c20 2765 275d 0d0a 330d 0a60 6060  c', 'e']..3..```
+00000d20: 0d0a 0d0a 4f66 2063 6f75 7273 652c 2074  ....Of course, t
+00000d30: 6869 7320 6973 2073 6f6d 6574 6869 6e67  his is something
+00000d40: 2074 6861 7420 7765 2063 616e 2065 6173   that we can eas
+00000d50: 696c 7920 7265 706c 6963 6174 6520 7573  ily replicate us
+00000d60: 696e 6720 7075 7265 2050 7974 686f 6e20  ing pure Python 
+00000d70: 696e 206f 6e65 206c 696e 652c 2077 6974  in one line, wit
+00000d80: 686f 7574 2074 6865 206e 6565 6420 666f  hout the need fo
+00000d90: 7220 6661 6e63 7920 7374 7566 663a 0d0a  r fancy stuff:..
+00000da0: 0d0a 6060 6070 7974 686f 6e0d 0a3e 3e3e  ..```python..>>>
+00000db0: 2064 6174 6120 3d20 7b27 6127 203a 207b   data = {'a' : {
+00000dc0: 2762 2720 3a20 7b27 6327 203a 207b 2765  'b' : {'c' : {'e
+00000dd0: 2720 3a20 337d 2c20 2764 2720 3a20 327d  ' : 3}, 'd' : 2}
+00000de0: 7d7d 2020 2020 0d0a 6060 600d 0a0d 0a54  }}    ..```....T
+00000df0: 6865 206b 6579 2070 6f69 6e74 2069 7320  he key point is 
+00000e00: 7468 6174 2077 6520 6c6f 6f70 206f 7665  that we loop ove
+00000e10: 7220 6120 7075 7265 2060 6469 6374 6020  r a pure `dict` 
+00000e20: 696e 7374 616e 6365 2c20 7765 2067 6574  instance, we get
+00000e30: 0d0a 0d0a 6060 6070 7974 686f 6e0d 0a3e  ....```python..>
+00000e40: 3e3e 205b 6b20 666f 7220 6b20 696e 2064  >> [k for k in d
+00000e50: 6174 612e 6b65 7973 2829 5d0d 0a5b 2761  ata.keys()]..['a
+00000e60: 275d 2020 2020 0d0a 6060 600d 0a0d 0a42  ']    ..```....B
+00000e70: 7574 2069 6620 7765 2075 7365 2061 2060  ut if we use a `
+00000e80: 4465 6570 6469 6374 6020 636c 6173 7320  Deepdict` class 
+00000e90: 616e 6420 7468 6520 6f70 7469 6f6e 2060  and the option `
+00000ea0: 6465 6570 3d54 7275 6560 2077 6865 6e20  deep=True` when 
+00000eb0: 6163 6365 7373 696e 670d 0a6b 6579 732c  accessing..keys,
+00000ec0: 2076 616c 7565 7320 6f72 2069 7465 6d73   values or items
+00000ed0: 206f 6620 6469 6374 696f 6e61 7269 6573   of dictionaries
+00000ee0: 2c20 7468 6520 666f 6c6c 6f77 696e 6720  , the following 
+00000ef0: 6861 7070 656e 733a 200d 0a0d 0a60 6060  happens: ....```
+00000f00: 7079 7468 6f6e 0d0a 3e3e 3e20 5b6b 2066  python..>>> [k f
+00000f10: 6f72 206b 2069 6e20 4465 6570 6469 6374  or k in Deepdict
+00000f20: 2864 6174 6129 2e6b 6579 7328 6465 6570  (data).keys(deep
+00000f30: 3d54 7275 6529 5d0d 0a5b 2765 272c 2027  =True)]..['e', '
+00000f40: 6427 5d20 2020 200d 0a60 6060 0d0a 0d0a  d']    ..```....
+00000f50: 5765 2063 616e 2073 6565 2c20 7468 6174  We can see, that
+00000f60: 2069 6e20 7468 6973 2063 6173 652c 2069   in this case, i
+00000f70: 7465 7261 7469 6f6e 2067 6f65 7320 6f76  teration goes ov
+00000f80: 6572 206b 6579 732c 2074 6861 7420 6163  er keys, that ac
+00000f90: 7475 616c 6c79 2068 6f6c 6420 6f6e 2074  tually hold on t
+00000fa0: 6f20 736f 6d65 2064 6174 612c 2061 6e64  o some data, and
+00000fb0: 2064 6f65 7320 6e6f 7420 7265 7475 726e   does not return
+00000fc0: 2074 6865 2063 6f6e 7461 696e 6572 7320   the containers 
+00000fd0: 7468 656d 7365 6c76 6573 2e20 4966 2077  themselves. If w
+00000fe0: 6520 646f 2074 6865 2073 616d 6520 6578  e do the same ex
+00000ff0: 7065 7269 6d65 6e74 2077 6974 6820 7468  periment with th
+00001000: 6520 7661 6c75 6573 2c20 6974 2073 686f  e values, it sho
+00001010: 7773 2074 6861 7420 7468 6520 6044 6565  ws that the `Dee
+00001020: 7064 6963 7460 206f 6e6c 7920 7265 7475  pdict` only retu
+00001030: 726e 7320 7468 6520 6c65 6166 7320 6f66  rns the leafs of
+00001040: 2074 6865 2064 6174 612d 7472 6565 2061   the data-tree a
+00001050: 6e64 2074 6865 2062 6568 6176 696f 7572  nd the behaviour
+00001060: 2069 7320 6675 6e64 616d 656e 7461 6c6c   is fundamentall
+00001070: 7920 6469 6666 6572 656e 743a 0d0a 0d0a  y different:....
+00001080: 6060 6070 7974 686f 6e0d 0a3e 3e3e 205b  ```python..>>> [
+00001090: 6b20 666f 7220 6b20 696e 2064 6174 612e  k for k in data.
+000010a0: 7661 6c75 6573 2829 5d0d 0a5b 7b27 6227  values()]..[{'b'
+000010b0: 3a20 7b27 6327 3a20 7b27 6527 3a20 337d  : {'c': {'e': 3}
+000010c0: 2c20 2764 273a 2032 7d7d 5d20 2020 200d  , 'd': 2}}]    .
+000010d0: 0a60 6060 0d0a 0d0a 6060 6070 7974 686f  .```....```pytho
+000010e0: 6e0d 0a3e 3e3e 205b 6b20 666f 7220 6b20  n..>>> [k for k 
+000010f0: 696e 2044 6565 7064 6963 7428 6461 7461  in Deepdict(data
+00001100: 292e 7661 6c75 6573 2864 6565 703d 5472  ).values(deep=Tr
+00001110: 7565 295d 0d0a 5b33 2c20 325d 2020 2020  ue)]..[3, 2]    
+00001120: 0d0a 6060 600d 0a0d 0a49 7420 6973 2069  ..```....It is i
+00001130: 6d70 6f72 7461 6e74 2c20 7468 6174 2074  mportant, that t
+00001140: 6865 2063 616c 6c20 606f 626a 2e76 616c  he call `obj.val
+00001150: 7565 7328 6465 6570 3d54 7275 6529 6020  ues(deep=True)` 
+00001160: 7374 696c 6c20 7265 7475 726e 7320 6120  still returns a 
+00001170: 6765 6e65 7261 746f 7220 6f62 6a65 6374  generator object
+00001180: 2c20 7768 6963 6820 6d61 6b65 7320 6974  , which makes it
+00001190: 206d 656d 6f72 7920 6566 6669 6369 656e   memory efficien
+000011a0: 7420 7768 656e 206c 6f6f 7069 6e67 206f  t when looping o
+000011b0: 7665 7220 6c61 7267 6520 6461 7461 7365  ver large datase
+000011c0: 7473 2e0d 0a0d 0a60 6060 7079 7468 6f6e  ts.....```python
+000011d0: 0d0a 3e3e 3e20 4465 6570 6469 6374 2864  ..>>> Deepdict(d
+000011e0: 6174 6129 2e76 616c 7565 7328 6465 6570  ata).values(deep
+000011f0: 3d54 7275 6529 0d0a 3c67 656e 6572 6174  =True)..<generat
+00001200: 6f72 206f 626a 6563 7420 4f72 6465 7265  or object Ordere
+00001210: 6444 6566 6175 6c74 4469 6374 2e76 616c  dDefaultDict.val
+00001220: 7565 7320 6174 2030 7830 3030 3030 3238  ues at 0x0000028
+00001230: 4632 3039 4435 3441 303e 2020 2020 0d0a  F209D54A0>    ..
+00001240: 6060 600d 0a0d 0a23 2323 2320 5772 6170  ```....#### Wrap
+00001250: 7069 6e67 0d0a 0d0a 5772 6170 7069 6e67  ping....Wrapping
+00001260: 206d 6179 206e 6f74 2062 6520 7468 6520   may not be the 
+00001270: 6d6f 7374 2065 6c65 6761 6e74 2073 6f6c  most elegant sol
+00001280: 7574 696f 6e73 2074 6f20 696e 6865 7269  utions to inheri
+00001290: 7420 7072 6f70 6572 7469 6573 206f 6620  t properties of 
+000012a0: 6120 6469 6666 6572 656e 7420 636c 6173  a different clas
+000012b0: 732c 2062 7574 2074 6865 7265 2061 7265  s, but there are
+000012c0: 2063 6572 7461 696e 2073 6974 7561 7469   certain situati
+000012d0: 6f6e 7320 7768 656e 2069 7420 6d69 6768  ons when it migh
+000012e0: 7420 7361 7665 2079 6f75 7220 6c69 6665  t save your life
+000012f0: 2e20 4f6e 6520 7375 6368 2061 2073 6365  . One such a sce
+00001300: 6e61 7269 6f20 6973 2077 6865 6e20 796f  nario is when yo
+00001310: 7520 7761 6e74 2074 6f20 7772 6974 6520  u want to write 
+00001320: 616e 2069 6e74 6572 6661 6365 2074 6f20  an interface to 
+00001330: 6120 4465 6570 6469 6374 2074 6861 7420  a Deepdict that 
+00001340: 6765 7473 2064 696e 616d 6963 616c 6c79  gets dinamically
+00001350: 2067 656e 6572 6174 6564 2072 756e 7469   generated runti
+00001360: 6d65 2c20 6d65 616e 696e 672c 2074 6861  me, meaning, tha
+00001370: 7420 7468 6520 636c 6173 7365 7320 6172  t the classes ar
+00001380: 6520 7369 6d70 6c79 206e 6f74 2070 7265  e simply not pre
+00001390: 7365 6e74 2061 7420 7468 6520 7469 6d65  sent at the time
+000013a0: 206f 6620 7772 6974 696e 6720 796f 7572   of writing your
+000013b0: 206f 776e 2063 6f64 652e 2054 6869 7320   own code. This 
+000013c0: 6973 2077 6865 6e20 6120 7772 6170 7065  is when a wrappe
+000013d0: 7220 636f 6d65 7320 6861 6e64 792e 2054  r comes handy. T
+000013e0: 6f20 7772 6170 2061 2064 6963 7469 6f6e  o wrap a diction
+000013f0: 6172 792c 2064 6f20 7468 6520 666f 6c6c  ary, do the foll
+00001400: 6f77 696e 673a 0d0a 0d0a 6060 6070 7974  owing:....```pyt
+00001410: 686f 6e0d 0a3e 3e3e 2066 726f 6d20 6465  hon..>>> from de
+00001420: 776c 6f6f 7368 2e63 6f72 6520 696d 706f  wloosh.core impo
+00001430: 7274 2057 7261 7070 6572 0d0a 3e3e 3e20  rt Wrapper..>>> 
+00001440: 6461 7461 203d 207b 2761 2720 3a20 7b27  data = {'a' : {'
+00001450: 6227 203a 207b 2763 2720 3a20 7b27 6527  b' : {'c' : {'e'
+00001460: 203a 2033 7d2c 2027 6427 203a 2032 7d7d   : 3}, 'd' : 2}}
+00001470: 7d0d 0a3e 3e3e 2077 7261 7070 6572 203d  }..>>> wrapper =
+00001480: 2057 7261 7070 6572 2877 7261 703d 6461   Wrapper(wrap=da
+00001490: 7461 2920 2020 0d0a 6060 600d 0a0d 0a54  ta)   ..```....T
+000014a0: 6865 2060 5772 6170 7065 7260 2063 6c61  he `Wrapper` cla
+000014b0: 7373 2063 6861 6e6e 656c 7320 646f 776e  ss channels down
+000014c0: 2065 7665 7279 2063 616c 6c20 746f 2074   every call to t
+000014d0: 6865 2077 7261 7070 6564 206f 626a 6563  he wrapped objec
+000014e0: 7420 2869 6e20 7468 6973 2063 6173 6520  t (in this case 
+000014f0: 6120 6469 6374 696f 6e61 7279 292c 2069  a dictionary), i
+00001500: 6620 7468 6520 6f62 6a65 6374 2074 6861  f the object tha
+00001510: 7420 7468 6520 6361 6c6c 2069 7320 6d61  t the call is ma
+00001520: 6465 2075 706f 6e20 6973 2075 6e61 626c  de upon is unabl
+00001530: 6520 746f 2061 6e73 7765 7220 7468 6520  e to answer the 
+00001540: 6361 6c6c 2062 7920 6974 7365 6c66 2028  call by itself (
+00001550: 6265 6361 7573 6520 6974 206d 6973 7365  because it misse
+00001560: 7320 7468 6520 7761 6e74 6564 2061 7474  s the wanted att
+00001570: 7269 6275 7465 206f 7220 6d65 7468 6f64  ribute or method
+00001580: 292e 2054 6865 2077 7261 7070 6564 206f  ). The wrapped o
+00001590: 626a 6563 7420 6973 2061 6363 6573 7369  bject is accessi
+000015a0: 626c 6520 7468 726f 7567 6820 7468 6520  ble through the 
+000015b0: 6077 7261 7070 6564 6020 7072 6f70 6572  `wrapped` proper
+000015c0: 7479 206f 6620 7468 6520 7772 6170 7065  ty of the wrappe
+000015d0: 722e 0d0a 0d0a 6060 6070 7974 686f 6e0d  r.....```python.
+000015e0: 0a3e 3e3e 2077 7261 7070 6572 2e77 7261  .>>> wrapper.wra
+000015f0: 7070 6564 0d0a 7b27 6127 3a20 7b27 6227  pped..{'a': {'b'
+00001600: 3a20 7b27 6327 3a20 7b27 6527 3a20 337d  : {'c': {'e': 3}
+00001610: 2c20 2764 273a 2032 7d7d 7d0d 0a60 6060  , 'd': 2}}}..```
+00001620: 0d0a 0d0a 4e6f 7465 2c20 7468 6174 2069  ....Note, that i
+00001630: 6620 666f 7220 736f 6d65 2072 6561 736f  f for some reaso
+00001640: 6e20 7765 2061 6363 6964 656e 7461 6c6c  n we accidentall
+00001650: 7920 7368 6164 6f77 2061 206d 6574 686f  y shadow a metho
+00001660: 6420 696e 2061 2062 6173 6520 636c 6173  d in a base clas
+00001670: 7320 6c69 6b65 2074 6869 733a 0d0a 0d0a  s like this:....
+00001680: 6060 6070 7974 686f 6e0d 0a3e 3e3e 2063  ```python..>>> c
+00001690: 6c61 7373 2043 7573 746f 6d57 7261 7070  lass CustomWrapp
+000016a0: 6572 2857 7261 7070 6572 293a 0d0a 3e3e  er(Wrapper):..>>
+000016b0: 3e0d 0a3e 3e3e 2020 2020 6465 6620 7661  >..>>>    def va
+000016c0: 6c75 6573 2873 656c 662c 202a 6172 6773  lues(self, *args
+000016d0: 2c20 2a2a 6b77 6172 6773 293a 0d0a 3e3e  , **kwargs):..>>
+000016e0: 3e20 2020 2020 2020 2072 6574 7572 6e20  >        return 
+000016f0: 4e6f 6e65 0d0a 6060 600d 0a0d 0a49 6420  None..```....Id 
+00001700: 7765 2074 7269 6564 2074 6f20 7772 6170  we tried to wrap
+00001710: 2061 2064 6963 7469 6f6e 6172 7920 6e6f   a dictionary no
+00001720: 772c 2074 6865 2069 6d70 6c65 6d65 6e74  w, the implement
+00001730: 6174 696f 6e20 776f 756c 6420 616c 7465  ation would alte
+00001740: 7220 7468 6520 6261 6861 7669 6f75 7220  r the bahaviour 
+00001750: 6f66 2074 6865 2077 7261 7070 6572 2c20  of the wrapper, 
+00001760: 6c65 6176 696e 6720 7468 6520 6265 6861  leaving the beha
+00001770: 7669 6f75 7220 6f66 2074 6865 2077 7261  viour of the wra
+00001780: 7070 6564 206f 626a 6563 7420 7072 6573  pped object pres
+00001790: 6572 7665 6420 616e 6420 7374 696c 6c20  erved and still 
+000017a0: 6163 6365 7373 6962 6c65 2061 7320 6060  accessible as ``
+000017b0: 4375 7374 6f6d 5772 6170 7065 7228 7772  CustomWrapper(wr
+000017c0: 6170 3d64 6174 6129 2e77 7261 7070 6564  ap=data).wrapped
+000017d0: 2e76 616c 7565 7328 2960 602e 0d0a 0d0a  .values()``.....
+000017e0: 6060 6070 7974 686f 6e0d 0a3e 3e3e 2043  ```python..>>> C
+000017f0: 7573 746f 6d57 7261 7070 6572 2877 7261  ustomWrapper(wra
+00001800: 703d 6461 7461 292e 7772 6170 7065 642e  p=data).wrapped.
+00001810: 7661 6c75 6573 2829 0d0a 6469 6374 5f76  values()..dict_v
+00001820: 616c 7565 7328 5b7b 2762 273a 207b 2763  alues([{'b': {'c
+00001830: 273a 207b 2765 273a 2033 7d2c 2027 6427  ': {'e': 3}, 'd'
+00001840: 3a20 327d 7d5d 290d 0a60 6060 0d0a 0d0a  : 2}}])..```....
+00001850: 2323 2323 2041 6273 7472 6163 7420 436c  #### Abstract Cl
+00001860: 6173 7365 7320 616e 6420 4d65 7461 7072  asses and Metapr
+00001870: 6f67 7261 6d6d 696e 670d 0a0d 0a54 6865  ogramming....The
+00001880: 2073 7562 6d6f 6475 6c65 2060 6465 776c   submodule `dewl
+00001890: 6f6f 7368 2e63 6f72 652e 6162 6360 2070  oosh.core.abc` p
+000018a0: 726f 7669 6465 7320 7369 6d70 6c65 2063  rovides simple c
+000018b0: 6c61 7373 6573 2074 6f20 616c 6c65 7669  lasses to allevi
+000018c0: 6174 6520 736f 6d65 206f 6620 7468 6520  ate some of the 
+000018d0: 756e 7761 6e74 6564 2063 6f6e 7365 7175  unwanted consequ
+000018e0: 656e 6365 7320 6f66 2074 6865 2064 796e  ences of the dyn
+000018f0: 616d 6963 616c 6c79 2074 7970 6564 206e  amically typed n
+00001900: 6174 7572 6520 6f66 2050 7974 686f 6e2e  ature of Python.
+00001910: 204f 6e65 206f 6620 7375 6368 2061 2073   One of such a s
+00001920: 6365 6e61 7269 6f73 2069 7320 7768 656e  cenarios is when
+00001930: 2077 6520 7375 6263 6c61 7373 2061 6e6f   we subclass ano
+00001940: 7468 6572 2063 6c61 7373 2066 726f 6d20  ther class from 
+00001950: 6120 7468 6972 642d 7061 7274 7920 4465  a third-party De
+00001960: 6570 6469 6374 2c20 6265 6361 7573 6520  epdict, because 
+00001970: 7765 2077 616e 7420 746f 2069 6e68 6572  we want to inher
+00001980: 6974 2074 6865 2066 756e 6374 696f 6e61  it the functiona
+00001990: 6c69 7479 2074 6865 7265 696e 2e20 4275  lity therein. Bu
+000019a0: 7420 7468 6520 7374 7566 6620 6973 2063  t the stuff is c
+000019b0: 6f6d 706c 6963 6174 6564 2c20 616e 6420  omplicated, and 
+000019c0: 7765 2070 726f 6261 626c 7920 776f 756e  we probably woun
+000019d0: 646e 2774 2077 616e 7420 746f 2067 6f20  dn't want to go 
+000019e0: 7468 726f 7567 6820 616c 6c20 6f66 2069  through all of i
+000019f0: 742e 204e 6576 6572 7468 656c 6573 732c  t. Nevertheless,
+00001a00: 2077 6520 7761 6e74 2074 6f20 6d61 6b65   we want to make
+00001a10: 2073 7572 652c 2074 6861 7420 7765 2064   sure, that we d
+00001a20: 6f6e 2774 2062 7261 6b65 2074 6865 2069  on't brake the i
+00001a30: 6e6e 6572 2066 6c6f 7720 6f66 2074 6865  nner flow of the
+00001a40: 206f 626a 6563 7420 6174 2072 756e 7469   object at runti
+00001a50: 6d65 2c20 6279 206f 7665 7272 6964 696e  me, by overridin
+00001a60: 6720 736f 6d65 2065 7373 656e 7469 616c  g some essential
+00001a70: 206d 6574 686f 6473 2c20 7368 6164 6f77   methods, shadow
+00001a80: 696e 6720 7468 6520 6f72 6967 696e 616c  ing the original
+00001a90: 2062 6568 6176 696f 7572 2e20 4e6f 7420   behaviour. Not 
+00001aa0: 6c69 6b65 2069 7420 776f 756c 646e 2774  like it wouldn't
+00001ab0: 2073 686f 7720 7570 2072 756e 7469 6d65   show up runtime
+00001ac0: 2073 6f6f 6e65 7220 6f72 206c 6174 6572   sooner or later
+00001ad0: 2c20 6275 7420 7468 6973 206c 6561 7665  , but this leave
+00001ae0: 7320 7468 6520 646f 6f72 206f 7065 6e65  s the door opene
+00001af0: 6420 666f 7220 6261 6420 636f 6465 2e20  d for bad code. 
+00001b00: 4c75 636b 696c 792c 2074 6865 2070 726f  Luckily, the pro
+00001b10: 626c 656d 2063 616e 2062 6520 736f 6c76  blem can be solv
+00001b20: 6564 2066 6169 726c 7920 6561 7369 6c79  ed fairly easily
+00001b30: 2077 6974 6820 736f 6d65 206d 6574 6170   with some metap
+00001b40: 726f 6772 616d 6d69 6e67 2c20 616e 6420  rogramming, and 
+00001b50: 7468 6520 6d65 7461 2073 7562 6d6f 6475  the meta submodu
+00001b60: 6c65 2070 726f 7669 6465 7320 616e 2061  le provides an a
+00001b70: 6273 7472 6163 7420 636c 6173 7320 6041  bstract class `A
+00001b80: 4243 5f53 6166 6560 2074 6861 7420 6361  BC_Safe` that ca
+00001b90: 6e20 6265 2075 7365 6420 6173 2061 2062  n be used as a b
+00001ba0: 6173 6520 636c 6173 7320 6675 7274 6865  ase class furthe
+00001bb0: 7220 646f 776e 2074 6865 206c 696e 652e  r down the line.
+00001bc0: 0d0a 0d0a 5275 6e6e 696e 6720 7468 6520  ....Running the 
+00001bd0: 666f 6c6c 6f77 696e 6720 636f 6465 2074  following code t
+00001be0: 6872 6f77 7320 616e 2065 7272 6f72 2061  hrows an error a
+00001bf0: 7420 6465 7369 676e 2074 696d 652c 2062  t design time, b
+00001c00: 6563 6175 7365 2060 666f 6f60 2069 7320  ecause `foo` is 
+00001c10: 616c 7265 6164 7920 696d 706c 656d 656e  already implemen
+00001c20: 7465 6420 696e 2074 6865 2070 6172 656e  ted in the paren
+00001c30: 7420 636c 6173 733a 0d0a 0d0a 6060 6070  t class:....```p
+00001c40: 7974 686f 6e0d 0a3e 3e3e 2066 726f 6d20  ython..>>> from 
+00001c50: 6465 776c 6f6f 7368 2e63 6f72 652e 6162  dewloosh.core.ab
+00001c60: 6320 696d 706f 7274 2041 4243 5f53 6166  c import ABC_Saf
+00001c70: 650d 0a3e 3e3e 200d 0a3e 3e3e 2063 6c61  e..>>> ..>>> cla
+00001c80: 7373 2050 6172 656e 7428 4142 435f 5361  ss Parent(ABC_Sa
+00001c90: 6665 293a 0d0a 3e3e 3e20 2020 2020 6465  fe):..>>>     de
+00001ca0: 6620 666f 6f28 7365 6c66 293a 0d0a 3e3e  f foo(self):..>>
+00001cb0: 3e20 2020 2020 2020 2020 7061 7373 0d0a  >         pass..
+00001cc0: 3e3e 3e20 0d0a 3e3e 3e20 636c 6173 7320  >>> ..>>> class 
+00001cd0: 4368 696c 6428 5061 7265 6e74 293a 0d0a  Child(Parent):..
+00001ce0: 3e3e 3e20 2020 2020 6465 6620 666f 6f28  >>>     def foo(
+00001cf0: 7365 6c66 293a 0d0a 3e3e 3e20 2020 2020  self):..>>>     
+00001d00: 2020 2020 7061 7373 0d0a 6060 600d 0a0d      pass..```...
+00001d10: 0a41 6e6f 7468 6572 2069 6d70 6f72 7461  .Another importa
+00001d20: 6e74 2073 6974 7561 7469 6f6e 2061 7269  nt situation ari
+00001d30: 7365 7320 7769 7468 2061 6273 7472 6163  ses with abstrac
+00001d40: 7420 6d65 7468 6f64 732e 2050 7974 686f  t methods. Pytho
+00001d50: 6e20 7072 6f76 6964 6573 2061 2064 6563  n provides a dec
+00001d60: 6f72 6174 6f72 2066 6f72 2074 6869 7320  orator for this 
+00001d70: 6f75 7420 6f66 2074 6865 2062 6f78 2c20  out of the box, 
+00001d80: 6275 7420 6167 6169 6e2c 206e 6f74 2069  but again, not i
+00001d90: 6d70 6c65 6d65 6e74 6564 2061 6273 7472  mplemented abstr
+00001da0: 6163 7420 6d65 7468 6f64 7320 6f6e 6c79  act methods only
+00001db0: 2073 686f 7720 7570 2061 7420 7275 6d74   show up at rumt
+00001dc0: 696d 652c 2077 6869 6368 2063 616e 2065  ime, which can e
+00001dd0: 6173 696c 7920 6265 206e 6f20 7469 6d65  asily be no time
+00001de0: 2069 6e20 7468 6520 776f 726c 6420 6f66   in the world of
+00001df0: 2069 6e74 6572 7072 6574 6564 206c 616e   interpreted lan
+00001e00: 6775 6167 6573 2e20 5468 6520 6d65 7461  guages. The meta
+00001e10: 2073 7562 6d6f 6475 6c20 6973 2065 7175   submodul is equ
+00001e20: 6970 7065 6420 7769 7468 2061 6e6f 7468  ipped with anoth
+00001e30: 6572 2061 6273 7472 6163 7420 636c 6173  er abstract clas
+00001e40: 7320 6361 6c6c 6564 2060 4142 435f 5374  s called `ABC_St
+00001e50: 726f 6e67 602c 2074 6861 7420 6d61 6b65  rong`, that make
+00001e60: 7320 796f 7520 6162 6c65 2074 6f20 6265  s you able to be
+00001e70: 2069 6e66 6f72 6d65 6420 6162 6f75 7420   informed about 
+00001e80: 6d69 7373 696e 6720 6675 6e63 7469 6f6e  missing function
+00001e90: 2069 6d70 6c65 6d65 6e74 6174 696f 6e73   implementations
+00001ea0: 206f 6620 6120 636c 6173 7320 7269 6768   of a class righ
+00001eb0: 7420 6174 2064 6573 6967 6e20 7469 6d65  t at design time
+00001ec0: 2e20 4865 7265 2027 5374 726f 6e67 2720  . Here 'Strong' 
+00001ed0: 7265 6665 7273 2074 6f20 7468 6520 7374  refers to the st
+00001ee0: 726f 6e67 6572 2072 6571 7569 7265 6d65  ronger requireme
+00001ef0: 6e74 2069 6d70 6f73 6564 206f 6e20 6162  nt imposed on ab
+00001f00: 7374 7261 6374 206d 6574 686f 6473 2e20  stract methods. 
+00001f10: 416e 2061 6273 7472 6163 7420 6d65 7468  An abstract meth
+00001f20: 6f64 2069 6e20 6120 6368 696c 6420 636c  od in a child cl
+00001f30: 6173 7320 6973 2065 6974 6865 7220 696d  ass is either im
+00001f40: 706c 656d 656e 7465 642c 206f 7220 6465  plemented, or de
+00001f50: 636f 7261 7465 6420 7769 7468 2074 6865  corated with the
+00001f60: 2060 6162 7374 7261 6374 6d65 7468 6f64   `abstractmethod
+00001f70: 6020 6465 636f 7261 746f 722c 2077 6869  ` decorator, whi
+00001f80: 6368 2070 6173 7365 7320 7468 6520 6261  ch passes the ba
+00001f90: 6c6c 2074 6f20 7468 6520 6e65 7874 2063  ll to the next c
+00001fa0: 6869 6c64 2e20 4f62 7669 6f75 736c 792c  hild. Obviously,
+00001fb0: 2079 6f75 2064 6f6e 2774 2067 6574 2074   you don't get t
+00001fc0: 6f20 7275 6e74 696d 652c 2075 6e6c 6573  o runtime, unles
+00001fd0: 7320 796f 7520 696d 706c 656d 656e 7420  s you implement 
+00001fe0: 616c 6c20 7468 6520 7265 7175 6972 6564  all the required
+00001ff0: 2061 6273 7472 6163 7420 636c 6173 7365   abstract classe
+00002000: 732e 2054 6869 7320 6973 2061 6c73 6f20  s. This is also 
+00002010: 7573 6566 756c 2069 6620 7765 2077 616e  useful if we wan
+00002020: 7420 746f 2063 7265 6174 6520 6120 7465  t to create a te
+00002030: 6d70 6c61 7465 206f 626a 6563 742c 2074  mplate object, t
+00002040: 6861 7420 7072 6f76 6964 6573 2069 6e73  hat provides ins
+00002050: 7472 7563 7469 6f6e 7320 6f6e 2068 6f77  tructions on how
+00002060: 2074 6f20 636f 6d70 6c65 7465 2061 2073   to complete a s
+00002070: 6b65 6c65 746f 6e20 746f 2068 6176 6520  keleton to have 
+00002080: 6120 776f 726b 696e 6720 736f 6c75 7469  a working soluti
+00002090: 6f6e 2e20 4120 7369 6d70 6c65 2065 7861  on. A simple exa
+000020a0: 6d70 6c65 2074 6f20 696c 6c75 7374 7261  mple to illustra
+000020b0: 7465 2077 6861 7420 6861 7070 656e 7320  te what happens 
+000020c0: 6966 2079 6f75 2062 7265 616b 2074 6865  if you break the
+000020d0: 2072 756c 6573 2069 7320 7468 6520 666f   rules is the fo
+000020e0: 6c6c 6f77 696e 673a 0d0a 0d0a 6060 6070  llowing:....```p
+000020f0: 7974 686f 6e0d 0a3e 3e3e 2066 726f 6d20  ython..>>> from 
+00002100: 6465 776c 6f6f 7368 2e63 6f72 652e 6162  dewloosh.core.ab
+00002110: 6320 696d 706f 7274 2041 4243 5f53 7472  c import ABC_Str
+00002120: 6f6e 670d 0a3e 3e3e 200d 0a3e 3e3e 2063  ong..>>> ..>>> c
+00002130: 6c61 7373 2050 6172 656e 7428 4142 435f  lass Parent(ABC_
+00002140: 5374 726f 6e67 293a 0d0a 3e3e 3e20 2020  Strong):..>>>   
+00002150: 2020 4061 6273 7472 6163 746d 6574 686f    @abstractmetho
+00002160: 6420 2020 200d 0a3e 3e3e 2020 2020 2064  d    ..>>>     d
+00002170: 6566 2066 6f6f 2873 656c 6629 3a0d 0a3e  ef foo(self):..>
+00002180: 3e3e 2020 2020 2020 2020 2070 6173 730d  >>         pass.
+00002190: 0a3e 3e3e 200d 0a3e 3e3e 2063 6c61 7373  .>>> ..>>> class
+000021a0: 2043 6869 6c64 2850 6172 656e 7429 3a0d   Child(Parent):.
+000021b0: 0a3e 3e3e 2020 2020 202e 2e2e 0d0a 6060  .>>>     .....``
+000021c0: 600d 0a0d 0a23 2323 2320 4162 7374 7261  `....#### Abstra
+000021d0: 6374 2043 6c61 7373 2050 726f 7065 7274  ct Class Propert
+000021e0: 6965 730d 0a0d 0a41 6c6f 6e67 2074 6865  ies....Along the
+000021f0: 2073 616d 6520 7468 6f75 6768 7473 2c20   same thoughts, 
+00002200: 736f 6d65 7469 6d65 7320 7765 2077 616e  sometimes we wan
+00002210: 7420 746f 2065 6e73 7572 6520 7468 6520  t to ensure the 
+00002220: 6578 6973 7465 6e63 6520 6f66 2073 6f6d  existence of som
+00002230: 6520 636c 6173 730d 0a70 726f 7065 7274  e class..propert
+00002240: 6965 7320 7768 656e 2062 7569 6c64 696e  ies when buildin
+00002250: 6720 636f 6d70 6c65 7820 6f62 6a65 6374  g complex object
+00002260: 7320 7769 7468 206d 756c 7469 706c 6520  s with multiple 
+00002270: 6261 7365 2063 6c61 7373 6573 2e20 5468  base classes. Th
+00002280: 6973 2063 616e 2062 6520 646f 6e65 2075  is can be done u
+00002290: 7369 6e67 2061 2073 7065 6369 616c 2064  sing a special d
+000022a0: 6563 6f72 6174 6f72 3a0d 0a0d 0a60 6060  ecorator:....```
+000022b0: 7079 7468 6f6e 0d0a 3e3e 3e20 6672 6f6d  python..>>> from
+000022c0: 2064 6577 6c6f 6f73 682e 636f 7265 2e61   dewloosh.core.a
+000022d0: 6370 2069 6d70 6f72 7420 6162 7374 7261  cp import abstra
+000022e0: 6374 5f63 6c61 7373 5f70 726f 7065 7274  ct_class_propert
+000022f0: 790d 0a3e 3e3e 2066 726f 6d20 6162 6320  y..>>> from abc 
+00002300: 696d 706f 7274 2041 4243 0d0a 3e3e 3e20  import ABC..>>> 
+00002310: 0d0a 3e3e 3e20 4061 6273 7472 6163 745f  ..>>> @abstract_
+00002320: 636c 6173 735f 7072 6f70 6572 7479 2870  class_property(p
+00002330: 726f 7031 3d69 6e74 2c20 7072 6f70 323d  rop1=int, prop2=
+00002340: 666c 6f61 747d 290d 0a3e 3e3e 2063 6c61  float})..>>> cla
+00002350: 7373 2042 6173 6543 6c61 7373 4128 4142  ss BaseClassA(AB
+00002360: 4329 3a0d 0a3e 3e3e 200d 0a3e 3e3e 2020  C):..>>> ..>>>  
+00002370: 2020 2070 726f 7031 3a20 696e 740d 0a3e     prop1: int..>
+00002380: 3e3e 2020 2020 2070 726f 7032 3a20 6c69  >>     prop2: li
+00002390: 7374 0d0a 3e3e 3e20 0d0a 3e3e 3e20 2020  st..>>> ..>>>   
+000023a0: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+000023b0: 656c 6629 3a0d 0a3e 3e3e 2020 2020 2020  elf):..>>>      
+000023c0: 2020 2073 656c 662e 7072 6f70 3220 3d20     self.prop2 = 
+000023d0: 5b33 2c20 345d 0d0a 3e3e 3e20 2020 2020  [3, 4]..>>>     
+000023e0: 2020 2020 7375 7065 7228 292e 5f5f 696e      super().__in
+000023f0: 6974 5f5f 2829 0d0a 3e3e 3e20 2020 2020  it__()..>>>     
+00002400: 2020 2020 7265 7475 726e 0d0a 6060 600d      return..```.
+00002410: 0a0d 0a23 2323 2320 496e 6669 7820 4f70  ...#### Infix Op
+00002420: 6572 6174 6f72 730d 0a0d 0a49 6e66 6978  erators....Infix
+00002430: 206f 7065 7261 746f 7273 2061 6c6c 6f77   operators allow
+00002440: 2066 6f72 2061 2066 616e 6379 2077 6179   for a fancy way
+00002450: 206f 6620 6465 6669 6e69 6e67 2062 696e   of defining bin
+00002460: 6172 7920 6f70 6572 6174 696f 6e73 2075  ary operations u
+00002470: 7369 6e67 2074 6865 206f 7065 7261 746f  sing the operato
+00002480: 7273 2027 3c3c 272c 2027 3e3e 2720 616e  rs '<<', '>>' an
+00002490: 6420 277c 272e 0d0a 0d0a 6060 6070 7974  d '|'.....```pyt
+000024a0: 686f 6e0d 0a3e 3e3e 2066 726f 6d20 6465  hon..>>> from de
+000024b0: 776c 6f6f 7368 2e63 6f72 652e 696e 6669  wloosh.core.infi
+000024c0: 7820 696d 706f 7274 2049 6e66 6978 0d0a  x import Infix..
+000024d0: 3e3e 3e20 0d0a 3e3e 3e20 6d75 6c20 3d20  >>> ..>>> mul = 
+000024e0: 496e 6669 7828 6c61 6d62 6461 2078 2c20  Infix(lambda x, 
+000024f0: 793a 2078 202a 2079 290d 0a3e 3e3e 2032  y: x * y)..>>> 2
+00002500: 207c 206d 756c 207c 2034 0d0a 380d 0a3e   | mul | 4..8..>
+00002510: 3e3e 2061 6464 203d 2049 6e66 6978 286c  >> add = Infix(l
+00002520: 616d 6264 6120 782c 2079 3a20 7820 2b20  ambda x, y: x + 
+00002530: 7929 0d0a 3e3e 3e20 3220 3c3c 2061 6464  y)..>>> 2 << add
+00002540: 203e 3e20 340d 0a36 0d0a 6060 600d 0a0d   >> 4..6..```...
+00002550: 0a23 2320 2a2a 5465 7374 696e 672a 2a0d  .## **Testing**.
+00002560: 0a0d 0a54 6f20 7275 6e20 616c 6c20 7465  ...To run all te
+00002570: 7374 732c 206f 7065 6e20 7570 2061 2063  sts, open up a c
+00002580: 6f6e 736f 6c65 2069 6e20 7468 6520 726f  onsole in the ro
+00002590: 6f74 2064 6972 6563 746f 7279 206f 6620  ot directory of 
+000025a0: 7468 6520 7072 6f6a 6563 7420 616e 6420  the project and 
+000025b0: 7479 7065 2074 6865 2066 6f6c 6c6f 7769  type the followi
+000025c0: 6e67 0d0a 0d0a 6060 6063 6f6e 736f 6c65  ng....```console
+000025d0: 0d0a 3e3e 3e20 7079 7468 6f6e 202d 6d20  ..>>> python -m 
+000025e0: 756e 6974 7465 7374 0d0a 6060 600d 0a0d  unittest..```...
+000025f0: 0a23 2320 2a2a 4465 7065 6e64 656e 6369  .## **Dependenci
+00002600: 6573 2a2a 0d0a 0d0a 5468 6520 6f6e 6c79  es**....The only
+00002610: 2064 6570 656e 6465 6e63 7920 6973 2060   dependency is `
+00002620: 7369 7860 2c20 746f 2070 726f 7669 6465  six`, to provide
+00002630: 2062 6173 6963 2063 6f6e 7469 6e75 6974   basic continuit
+00002640: 7920 6265 7477 6565 6e20 6d61 6a6f 7220  y between major 
+00002650: 5079 7468 6f6e 2076 6572 7369 6f6e 7320  Python versions 
+00002660: 3220 616e 6420 332e 0d0a 0d0a 2323 202a  2 and 3.....## *
+00002670: 2a4c 6963 656e 7365 2a2a 0d0a 0d0a 5468  *License**....Th
+00002680: 6973 2070 6163 6b61 6765 2069 7320 6c69  is package is li
+00002690: 6365 6e73 6564 2075 6e64 6572 2074 6865  censed under the
+000026a0: 204d 4954 206c 6963 656e 7365 2e          MIT license.
```

### Comparing `dewloosh.core-1.0.6/setup.py` & `dewloosh.core-1.0.9/setup.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-# -*- coding: utf-8 -*-
-import codecs
-import os.path, sys
-from setuptools import find_namespace_packages, setup
-from setuptools.command.install import install
-
-
-def read(rel_path):
-    here = os.path.abspath(os.path.dirname(__file__))
-    with codecs.open(os.path.join(here, rel_path), 'r') as fp:
-        return fp.read()
-
-
-def get_version(rel_path):
-    for line in read(rel_path).splitlines():
-        if line.startswith('__version__'):
-            delim = '"' if '"' in line else "'"
-            return line.split(delim)[1]
-    else:
-        raise RuntimeError("Unable to find version string.")
-    
-    
-def get_description(rel_path):
-    for line in read(rel_path).splitlines():
-        if line.startswith('__description__'):
-            delim = '"' if '"' in line else "'"
-            return line.split(delim)[1]
-    else:
-        raise RuntimeError("Unable to find description string.")
-
-
-with open("README.md", "r") as fh:
-    long_description = fh.read()
-
-
-with open('requirements.txt') as f:
-    required = f.read().splitlines()
-
-
-_module = os.listdir(os.path.join(os.path.dirname(__file__), "src/dewloosh"))[0]
-_init_path = "src/dewloosh/{}/__init__.py".format(_module)
-_version = get_version(_init_path)
-_description = get_description(_init_path)
-_url = 'https://github.com/dewloosh/dewloosh-{}'.format(_module)
-_download_url = _url + '/archive/refs/tags/{}.zip'.format(_version)
-
-
-class VerifyVersionCommand(install):
-    """Custom command to verify that the git tag matches our version"""
-    description = 'verify that the git tag matches our version'
-
-    def run(self):
-        tag = os.getenv('CIRCLE_TAG')
-        v = 'v' + _version
-        if tag != v:
-            info = "Git tag: {0} does not match the version of this app: {1}".format(
-                tag, v
-            )
-            sys.exit(info)
-
-setup(
-	name="dewloosh.{}".format(_module),
-    version=_version,                        
-    author="dewloosh",
-    author_email = 'dewloosh@gmail.com',                   
-    description=_description,
-    long_description=long_description,   
-    long_description_content_type="text/markdown",
-	url = _url, 
-    download_url = _download_url,
-	packages=find_namespace_packages(where='src', include=['dewloosh.*']),
-	classifiers=[
-        'Development Status :: 5 - Production/Stable',     
-        'License :: OSI Approved :: MIT License',
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",   
-        'Programming Language :: Python :: 3 :: Only',
-		'Operating System :: OS Independent'
-    ],                                      
-    python_requires='>=3.6',
-    cmdclass={
-        'verify': VerifyVersionCommand,
-    },                             
-    package_dir={'':'src'},     
-    install_requires=required,
-	zip_safe=False,
+# -*- coding: utf-8 -*-
+import codecs
+import os.path, sys
+from setuptools import find_namespace_packages, setup
+from setuptools.command.install import install
+
+
+def read(rel_path):
+    here = os.path.abspath(os.path.dirname(__file__))
+    with codecs.open(os.path.join(here, rel_path), 'r') as fp:
+        return fp.read()
+
+
+def get_version(rel_path):
+    for line in read(rel_path).splitlines():
+        if line.startswith('__version__'):
+            delim = '"' if '"' in line else "'"
+            return line.split(delim)[1]
+    else:
+        raise RuntimeError("Unable to find version string.")
+    
+    
+def get_description(rel_path):
+    for line in read(rel_path).splitlines():
+        if line.startswith('__description__'):
+            delim = '"' if '"' in line else "'"
+            return line.split(delim)[1]
+    else:
+        raise RuntimeError("Unable to find description string.")
+
+
+with open("README.md", "r") as fh:
+    long_description = fh.read()
+
+
+with open('requirements.txt') as f:
+    required = f.read().splitlines()
+
+
+_module = os.listdir(os.path.join(os.path.dirname(__file__), "src/dewloosh"))[0]
+_init_path = "src/dewloosh/{}/__init__.py".format(_module)
+_version = get_version(_init_path)
+_description = get_description(_init_path)
+_url = 'https://github.com/dewloosh/dewloosh-{}'.format(_module)
+_download_url = _url + '/archive/refs/tags/{}.zip'.format(_version)
+
+
+class VerifyVersionCommand(install):
+    """Custom command to verify that the git tag matches our version"""
+    description = 'verify that the git tag matches our version'
+
+    def run(self):
+        tag = os.getenv('CIRCLE_TAG')
+        v = 'v' + _version
+        if tag != v:
+            info = "Git tag: {0} does not match the version of this app: {1}".format(
+                tag, v
+            )
+            sys.exit(info)
+
+setup(
+	name="dewloosh.{}".format(_module),
+    version=_version,                        
+    author="dewloosh",
+    author_email = 'dewloosh@gmail.com',                   
+    description=_description,
+    long_description=long_description,   
+    long_description_content_type="text/markdown",
+	url = _url, 
+    download_url = _download_url,
+	packages=find_namespace_packages(where='src', include=['dewloosh.*']),
+	classifiers=[
+        'Development Status :: 5 - Production/Stable',     
+        'License :: OSI Approved :: MIT License',
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",   
+        'Programming Language :: Python :: 3 :: Only',
+		'Operating System :: OS Independent'
+    ],                                      
+    python_requires='>=3.6',
+    cmdclass={
+        'verify': VerifyVersionCommand,
+    },                             
+    package_dir={'':'src'},     
+    install_requires=required,
+	zip_safe=False,
 )
```

### Comparing `dewloosh.core-1.0.6/src/dewloosh/core/abc.py` & `dewloosh.core-1.0.9/src/dewloosh/core/abc.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-# -*- coding: utf-8 -*-
-from .meta import *
-
-
-__all__ = ["ABC_Strong", "ABC_Weak", "ABC_Safe"]
-
-
-class ABC_Weak(metaclass=ABCMeta_Weak):
-    """
-    Helper class that provides a standard way to create an ABC using
-    inheritance.
-    """
-    __slots__ = ()
-
-
-class ABC_Strong(metaclass=ABCMeta_Strong):
-    """Helper class that provides a standard way to create an ABC using
-    inheritance.
-    """
-    __slots__ = ()
-
-
-class ABC_Safe(metaclass=ABCMeta_Safe):
-    """
-    Helper class that provides a standard way to create an ABC using
-    inheritance.
-    """
-    __slots__ = ()
-
+# -*- coding: utf-8 -*-
+from .meta import *
+
+
+__all__ = ["ABC_Strong", "ABC_Weak", "ABC_Safe"]
+
+
+class ABC_Weak(metaclass=ABCMeta_Weak):
+    """
+    Helper class that provides a standard way to create an ABC using
+    inheritance.
+    """
+    __slots__ = ()
+
+
+class ABC_Strong(metaclass=ABCMeta_Strong):
+    """Helper class that provides a standard way to create an ABC using
+    inheritance.
+    """
+    __slots__ = ()
+
+
+class ABC_Safe(metaclass=ABCMeta_Safe):
+    """
+    Helper class that provides a standard way to create an ABC using
+    inheritance.
+    """
+    __slots__ = ()
+
```

### Comparing `dewloosh.core-1.0.6/src/dewloosh/core/acp.py` & `dewloosh.core-1.0.9/src/dewloosh/core/acp.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,142 +1,142 @@
-# -*- coding: utf-8 -*-
-"""
-Multiple solutions on how to enforce an abstract class property
-on an object. Generic types like 'List[int]' are not allowed, 
-because the don't work well with the isinstance()-like methods.
-"""
-
-__all__ = ['abstract_class_property', 'setproperty']
-
-
-def abstract_class_property(**kwargs):
-    return abstract_class_property_B(**kwargs)
-
-
-def setproperty(**kwargs):
-    def decorator(cls):
-        for key, value in kwargs.items():
-            setattr(cls, key, value)
-        return cls
-    return decorator
-
-
-"""
-Implementation A : class annotations solution using an object descriptor 
-and a wrapper class with classic pythonic manipulations.
-"""
-
-
-def abstract_class_property_A(**kwargs):
-    """
-    Decorator function to decorate objects with abstract
-    class properties. Leaves behind another decorator 
-    that takes a class as its input.
-    """
-
-    def abstractor(WrappedClass):
-
-        class PropertyWrapper(WrappedClass):
-            """
-            A Wrapper class to decorate objects with abstract class properties.
-            The class has a default dummy annotation, just so that we can append 
-            the items of the input dictionary d to the class definition.
-            The dummy property is deleted at the end.
-            """
-            _dummy_: None
-
-            def __init__(self, *args, **kwargs):
-                WrappedClass.__init__(self)
-                d_ = dict()
-                d_props = PropertyWrapper.__dict__.get('__annotations__', {})
-                for key, value in d_props.items():
-                    d_[key] = value
-                d_self = self.__class__.__dict__.get('__annotations__', {})
-                for key, value in d_self.items():
-                    d_[key] = value
-                for key in d_.keys():
-                    if not hasattr(self, key):
-                        raise AttributeError(f'required attribute {key} not present '
-                                             f'in {self.__class__}')
-                return
-
-        res = PropertyWrapper
-        d_ = res.__dict__['__annotations__']
-        for key, value in kwargs.items():
-            d_[key] = value
-        for key, value in WrappedClass.__dict__.get('__annotations__', {}).items():
-            d_[key] = value
-        del d_['_dummy_']
-        return res
-
-    return abstractor
-
-
-"""
-Implementation B : class annotations solution using an object descriptor and a 
-wrapper class using the __mro__ property of the class.
-This implementation also checks the validity of the declaration.
-"""
-
-
-def abstract_class_property_B(**kwargs):
-    """
-    Decorator function to decorate objects with abstract
-    class properties. Leaves behind another decorator
-    that takes a class as its input.
-    """
-
-    def abstractor(WrappedClass):
-
-        class PropertyWrapper(WrappedClass):
-            """
-            A Wrapper class to decorate objects with abstract class properties.
-            The class has a default dummy annotation, just so that we can append 
-            the items of the input dictionary d to the class definition.
-            The dummy property is deleted at the end.
-            """
-            _dummy_: None
-
-            def __init__(self, *args, **kwargs):
-                WrappedClass.__init__(self)
-                self.__check_absclsprops__()
-                return
-
-            @classmethod
-            def __absclsprops__(cls):
-                """
-                Collects the abstracts class properties and their
-                expected types based on the MRO of the class.
-                """
-                t = cls.__mro__
-                l = [ti.__dict__.get('__annotations__', {}) for ti in t]
-                res = dict()
-                for d in l:
-                    for key, value in d.items():
-                        res[key] = value
-                return res
-
-            def __check_absclsprops__(self):
-                """
-                Checks if the instance has attributes according to
-                the anstract annotations. Returns True if every attribute is
-                a type-correct declaration.
-                """
-                props = self.__class__.__absclsprops__()
-                for key, value in props.items():
-                    if not hasattr(self, key):
-                        raise AttributeError(f'required attribute {key} not present '
-                                             f'in {self.__class__}')
-                    else:
-                        if not isinstance(getattr(self, key), value):
-                            raise TypeError(
-                                'TypeError. key : {}, value = {}'.format(key, value))
-                return True
-
-        res = PropertyWrapper
-        d_ = res.__dict__['__annotations__']
-        for key, value in kwargs.items():
-            d_[key] = value
-        del d_['_dummy_']
-        return res
-
+# -*- coding: utf-8 -*-
+"""
+Multiple solutions on how to enforce an abstract class property
+on an object. Generic types like 'List[int]' are not allowed, 
+because the don't work well with the isinstance()-like methods.
+"""
+
+__all__ = ['abstract_class_property', 'setproperty']
+
+
+def abstract_class_property(**kwargs):
+    return abstract_class_property_B(**kwargs)
+
+
+def setproperty(**kwargs):
+    def decorator(cls):
+        for key, value in kwargs.items():
+            setattr(cls, key, value)
+        return cls
+    return decorator
+
+
+"""
+Implementation A : class annotations solution using an object descriptor 
+and a wrapper class with classic pythonic manipulations.
+"""
+
+
+def abstract_class_property_A(**kwargs):
+    """
+    Decorator function to decorate objects with abstract
+    class properties. Leaves behind another decorator 
+    that takes a class as its input.
+    """
+
+    def abstractor(WrappedClass):
+
+        class PropertyWrapper(WrappedClass):
+            """
+            A Wrapper class to decorate objects with abstract class properties.
+            The class has a default dummy annotation, just so that we can append 
+            the items of the input dictionary d to the class definition.
+            The dummy property is deleted at the end.
+            """
+            _dummy_: None
+
+            def __init__(self, *args, **kwargs):
+                WrappedClass.__init__(self)
+                d_ = dict()
+                d_props = PropertyWrapper.__dict__.get('__annotations__', {})
+                for key, value in d_props.items():
+                    d_[key] = value
+                d_self = self.__class__.__dict__.get('__annotations__', {})
+                for key, value in d_self.items():
+                    d_[key] = value
+                for key in d_.keys():
+                    if not hasattr(self, key):
+                        raise AttributeError(f'required attribute {key} not present '
+                                             f'in {self.__class__}')
+                return
+
+        res = PropertyWrapper
+        d_ = res.__dict__['__annotations__']
+        for key, value in kwargs.items():
+            d_[key] = value
+        for key, value in WrappedClass.__dict__.get('__annotations__', {}).items():
+            d_[key] = value
+        del d_['_dummy_']
+        return res
+
+    return abstractor
+
+
+"""
+Implementation B : class annotations solution using an object descriptor and a 
+wrapper class using the __mro__ property of the class.
+This implementation also checks the validity of the declaration.
+"""
+
+
+def abstract_class_property_B(**kwargs):
+    """
+    Decorator function to decorate objects with abstract
+    class properties. Leaves behind another decorator
+    that takes a class as its input.
+    """
+
+    def abstractor(WrappedClass):
+
+        class PropertyWrapper(WrappedClass):
+            """
+            A Wrapper class to decorate objects with abstract class properties.
+            The class has a default dummy annotation, just so that we can append 
+            the items of the input dictionary d to the class definition.
+            The dummy property is deleted at the end.
+            """
+            _dummy_: None
+
+            def __init__(self, *args, **kwargs):
+                WrappedClass.__init__(self)
+                self.__check_absclsprops__()
+                return
+
+            @classmethod
+            def __absclsprops__(cls):
+                """
+                Collects the abstracts class properties and their
+                expected types based on the MRO of the class.
+                """
+                t = cls.__mro__
+                l = [ti.__dict__.get('__annotations__', {}) for ti in t]
+                res = dict()
+                for d in l:
+                    for key, value in d.items():
+                        res[key] = value
+                return res
+
+            def __check_absclsprops__(self):
+                """
+                Checks if the instance has attributes according to
+                the anstract annotations. Returns True if every attribute is
+                a type-correct declaration.
+                """
+                props = self.__class__.__absclsprops__()
+                for key, value in props.items():
+                    if not hasattr(self, key):
+                        raise AttributeError(f'required attribute {key} not present '
+                                             f'in {self.__class__}')
+                    else:
+                        if not isinstance(getattr(self, key), value):
+                            raise TypeError(
+                                'TypeError. key : {}, value = {}'.format(key, value))
+                return True
+
+        res = PropertyWrapper
+        d_ = res.__dict__['__annotations__']
+        for key, value in kwargs.items():
+            d_[key] = value
+        del d_['_dummy_']
+        return res
+
     return abstractor
```

### Comparing `dewloosh.core-1.0.6/src/dewloosh/core/deepdict.py` & `dewloosh.core-1.0.9/src/dewloosh/core/deepdict.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,311 +1,314 @@
-# -*- coding: utf-8 -*-
-# http://stackoverflow.com/a/6190500/562769
-from typing import Hashable, Union
-from collections.abc import Iterable
-import six
-
-from .tools.dtk import dictparser, parseitems, parseaddress, parsedicts
-
-
-__all__ = ['DeepDict']
-
-
-NoneType = type(None)
-
-
-def issequence(arg) -> bool:
-    """
-    Returns `True` if `arg` is any kind of iterable, but not a string,
-    returns `False` otherwise.
-    
-    Examples
-    --------
-    The formatter to use to print a floating point number with 4 digits:
-    
-    >>> from dewloosh.core.tools import issequence
-    >>> issequence([1, 2])
-    True
-    
-    To print the actual value as a string:
-    
-    >>> issequence('lorem ipsum')
-    False    
-    """
-    return (
-        isinstance(arg, Iterable)
-        and not isinstance(arg, six.string_types)
-    )  
-
-
-class DeepDict(dict):
-    """
-    An nested dictionary class with a self-replicating default factory. 
-    It can be a drop-in replacement for the bulit-in dictionary type, 
-    but it's more capable as it handles nested layouts.
-    
-    Examples
-    --------
-    Basic usage:
-    
-    >>> from nddict import DeepDict
-    >>> d = {'a' : {'aa' : {'aaa' : 0}}, 'b' : 1, 'c' : {'cc' : 2}}
-    >>> dd = DeepDict(d)
-    >>> list(dd.values(deep=True))
-    [0, 1, 2]
-    
-    See the docs for more use cases!
-        
-    """
-    
-    def __init__(self, *args, parent=None, root=None, locked=None, **kwargs):
-        """
-        Returns a `DeepDict` instance.
-
-        Parameters
-        ----------
-        *args : tuple, Optional
-            Extra positional arguments are forwarded to the `dict` class.
-
-        parent : `DeepDict`, Optional
-            Parent `DeepDict` instance. Default is `None`.
-
-        root : `DeepDict`, Optional
-            The top-level object. It is automatically set when creating nested
-            layouts, but may be explicitly provided. Default is `None`. 
-
-        locked : bool or NoneType, Optional
-            If the object is locked, it reacts to missing keys as a regular dictionary would.
-            If it is not, a new level and a new child is created (see the examples in the docs).
-            A `None` value means that in terms of locking, the state of the object 
-            is inherited from its parent. Default is `None`.
-
-        **kwargs : tuple, Optional
-            Extra keyword arguments are forwarded to the `dict` class.
-
-        """
-        super().__init__(*args, **kwargs)
-        self.parent = parent
-        self._root = root
-        self._locked = locked
-        self._key = None
-        
-    @property
-    def key(self) -> Union[Hashable, NoneType]:
-        """
-        Returns the key of the dictionary in its parent, or `None` if the 
-        object is the root.
-        """
-        return self._key
-           
-    @property
-    def locked(self) -> bool:
-        """
-        Returns `True` if the object is locked. The property is equpped with a setter.
-        """
-        if self.parent is None:
-            return self._locked if isinstance(self._locked, bool) else False
-        else:
-            return self._locked if isinstance(self._locked, bool) else self.parent.locked
-
-    @locked.setter
-    def locked(self, value):
-        assert isinstance(value, bool)
-        self._locked = value
-
-    @property
-    def depth(self) -> int:
-        """
-        Retuns the depth of the actual instance in a layout, starting from 0..
-        """
-        if self.parent is None:
-            return 0
-        else:
-            return self.parent.depth + 1
-
-    def lock(self):
-        """
-        Locks the layout of the dictionary. If a `DeepDict` is locked,
-        missing keys are handled the same way as they would've been handled
-        if it was a ´dict´.        
-
-        Equivalent to ``self.locked = True``.
-        """
-        self._locked = True
-
-    def unlock(self):
-        """
-        Releases the layout of the dictionary. If a `DeepDict` is not locked,
-        a missing key creates a new level in the layout.
-
-        Equivalent to ``self.locked = False``.
-        """
-        self._locked = False
-
-    def root(self):
-        """
-        Returns the top-level object in a nested layout.
-        """
-        if self.parent is None:
-            return self
-        else:
-            if self._root is not None:
-                return self._root
-            else:
-                return self.parent.root()
-
-    def is_root(self) -> bool:
-        """
-        Returns `True`, if the object is the root.
-        """
-        return self.parent is None
-
-    def containers(self, *args, inclusive=False, deep=True, dtype=None, **kwargs):
-        """
-        Returns all the containers in a nested layout. A dictionary in a nested layout
-        is called a container, only if it contains other containers (it is a parent). 
-
-        Parameters
-        ----------
-        inclusive : bool, Optional
-            If `True`, the object the call is made upon also gets returned.
-            This can be important if you make the call on the root object, which most
-            of the time does not hold onto relevant data directly.
-            Default is `False`.
-
-        deep : bool, Optional
-            If `True` the parser goes into nested dictionaries.
-            Default is `True`
-
-        dtype : Any, Optional
-            Constrains the type of the returned objects.
-            Default is `None`, which means no restriction.
-
-        Returns
-        -------
-        generator
-            Returns a generator object.
-
-        Examples
-        --------
-        A simple example:
-
-        >>> from nddict import DeepDict
-        >>> data = DeepDict()
-        >>> data['a', 'b', 'c'] = 1
-        >>> [c.key for c in data.containers()]
-        ['a', 'b']
-
-        We can see, that dictionaries 'a' and 'b' are returned as containers, but 'c' 
-        isn't,  because it is not a parent, there are no deeper levels. 
-
-        >>> [c.key for c in data.containers(inclusive=True, deep=True)]
-        [None, 'a', 'b']
-
-        >>> [c.key for c in data.containers(inclusive=True, deep=False)]     
-        [None, 'a']
-
-        >>> [c.key for c in data.containers(inclusive=False, deep=True)]       
-        ['a', 'b']
-
-        >>> [c.key for c in data.containers(inclusive=False, deep=False)]      
-        ['a']
-
-        """
-        dtype = self.__class__ if dtype is None else dtype
-        return parsedicts(self, inclusive=inclusive, dtype=dtype, deep=deep)
-
-    def __getitem__(self, key):
-        try:
-            if issequence(key):
-                return parseaddress(self, key)
-            else:
-                return super().__getitem__(key)
-        except ValueError:
-            return self.__missing__(key)
-        except KeyError:
-            return self.__missing__(key)
-
-    def __setitem__(self, key, value):
-        try:
-            if issequence(key):
-                if not key[0] in self:
-                    d = self.__missing__(key[0])
-                else:
-                    d = self[key[0]]
-                if len(key) > 1:
-                    d.__setitem__(key[1:], value)
-                else:
-                    self[key[0]] = value
-            else:
-                if isinstance(value, DeepDict):
-                    value.__join_parent__(self, key)
-                return super().__setitem__(key, value)
-        except AttributeError:
-            raise RuntimeError(
-                "Target is of type '{}', which is not a container.".format(type(d)))
-        except KeyError:
-            return self.__missing__(key)
-
-    def __missing__(self, key):
-        if self.locked:
-            raise KeyError("Missing key : {}".format(key))
-        if issequence(key):
-            if key[0] not in self:
-                self[key[0]] = value = self.__class__()
-            else:
-                value = self[key[0]]
-            if len(key) > 1:
-                return value.__missing__(key[1:])
-            else:
-                return value
-        else:
-            self[key] = value = self.__class__()
-            return value
-        
-    def __reduce__(self):
-        return self.__class__, tuple(), None, None, self.items()
-    
-    def __repr__(self):
-        frmtstr = self.__class__.__name__ + '(%s)'
-        return frmtstr % (dict.__repr__(self))
-       
-    def __join_parent__(self, parent, key: Hashable = None):
-        self.parent = parent
-        self._root = parent.root()
-        self._key = key
-
-    def items(self, *args, deep=False, return_address=False, **kwargs):
-        if deep:
-            if return_address:
-                for addr, v in dictparser(self):
-                    yield addr, v
-            else:
-                for k, v in parseitems(self):
-                    yield k, v
-        else:
-            for k, v in super().items():
-                yield k, v
-
-    def values(self, *args, deep=False, return_address=False, **kwargs):
-        if deep:
-            if return_address:
-                for addr, v in dictparser(self):
-                    yield addr, v
-            else:
-                for _, v in parseitems(self):
-                    yield v
-        else:
-            for v in super().values():
-                yield v
-
-    def keys(self, *args, deep=False, return_address=False, **kwargs):
-        if deep:
-            if return_address:
-                for addr, _ in dictparser(self):
-                    yield addr
-            else:
-                for k, _ in parseitems(self):
-                    yield k
-        else:
-            for k in super().keys():
-                yield k
+# -*- coding: utf-8 -*-
+# http://stackoverflow.com/a/6190500/562769
+from typing import Hashable, Union
+try:
+    from collections.abc import Iterable
+except ImportError:
+    from collections import Iterable
+import six
+
+from .tools.dtk import dictparser, parseitems, parseaddress, parsedicts
+
+
+__all__ = ['DeepDict']
+
+
+NoneType = type(None)
+
+
+def issequence(arg) -> bool:
+    """
+    Returns `True` if `arg` is any kind of iterable, but not a string,
+    returns `False` otherwise.
+    
+    Examples
+    --------
+    The formatter to use to print a floating point number with 4 digits:
+    
+    >>> from dewloosh.core.tools import issequence
+    >>> issequence([1, 2])
+    True
+    
+    To print the actual value as a string:
+    
+    >>> issequence('lorem ipsum')
+    False    
+    """
+    return (
+        isinstance(arg, Iterable)
+        and not isinstance(arg, six.string_types)
+    )  
+
+
+class DeepDict(dict):
+    """
+    An nested dictionary class with a self-replicating default factory. 
+    It can be a drop-in replacement for the bulit-in dictionary type, 
+    but it's more capable as it handles nested layouts.
+    
+    Examples
+    --------
+    Basic usage:
+    
+    >>> from nddict import DeepDict
+    >>> d = {'a' : {'aa' : {'aaa' : 0}}, 'b' : 1, 'c' : {'cc' : 2}}
+    >>> dd = DeepDict(d)
+    >>> list(dd.values(deep=True))
+    [0, 1, 2]
+    
+    See the docs for more use cases!
+        
+    """
+    
+    def __init__(self, *args, parent=None, root=None, locked=None, **kwargs):
+        """
+        Returns a `DeepDict` instance.
+
+        Parameters
+        ----------
+        *args : tuple, Optional
+            Extra positional arguments are forwarded to the `dict` class.
+
+        parent : `DeepDict`, Optional
+            Parent `DeepDict` instance. Default is `None`.
+
+        root : `DeepDict`, Optional
+            The top-level object. It is automatically set when creating nested
+            layouts, but may be explicitly provided. Default is `None`. 
+
+        locked : bool or NoneType, Optional
+            If the object is locked, it reacts to missing keys as a regular dictionary would.
+            If it is not, a new level and a new child is created (see the examples in the docs).
+            A `None` value means that in terms of locking, the state of the object 
+            is inherited from its parent. Default is `None`.
+
+        **kwargs : tuple, Optional
+            Extra keyword arguments are forwarded to the `dict` class.
+
+        """
+        super().__init__(*args, **kwargs)
+        self.parent = parent
+        self._root = root
+        self._locked = locked
+        self._key = None
+        
+    @property
+    def key(self) -> Union[Hashable, NoneType]:
+        """
+        Returns the key of the dictionary in its parent, or `None` if the 
+        object is the root.
+        """
+        return self._key
+           
+    @property
+    def locked(self) -> bool:
+        """
+        Returns `True` if the object is locked. The property is equpped with a setter.
+        """
+        if self.parent is None:
+            return self._locked if isinstance(self._locked, bool) else False
+        else:
+            return self._locked if isinstance(self._locked, bool) else self.parent.locked
+
+    @locked.setter
+    def locked(self, value):
+        assert isinstance(value, bool)
+        self._locked = value
+
+    @property
+    def depth(self) -> int:
+        """
+        Retuns the depth of the actual instance in a layout, starting from 0..
+        """
+        if self.parent is None:
+            return 0
+        else:
+            return self.parent.depth + 1
+
+    def lock(self):
+        """
+        Locks the layout of the dictionary. If a `DeepDict` is locked,
+        missing keys are handled the same way as they would've been handled
+        if it was a ´dict´.        
+
+        Equivalent to ``self.locked = True``.
+        """
+        self._locked = True
+
+    def unlock(self):
+        """
+        Releases the layout of the dictionary. If a `DeepDict` is not locked,
+        a missing key creates a new level in the layout.
+
+        Equivalent to ``self.locked = False``.
+        """
+        self._locked = False
+
+    def root(self):
+        """
+        Returns the top-level object in a nested layout.
+        """
+        if self.parent is None:
+            return self
+        else:
+            if self._root is not None:
+                return self._root
+            else:
+                return self.parent.root()
+
+    def is_root(self) -> bool:
+        """
+        Returns `True`, if the object is the root.
+        """
+        return self.parent is None
+
+    def containers(self, *args, inclusive=False, deep=True, dtype=None, **kwargs):
+        """
+        Returns all the containers in a nested layout. A dictionary in a nested layout
+        is called a container, only if it contains other containers (it is a parent). 
+
+        Parameters
+        ----------
+        inclusive : bool, Optional
+            If `True`, the object the call is made upon also gets returned.
+            This can be important if you make the call on the root object, which most
+            of the time does not hold onto relevant data directly.
+            Default is `False`.
+
+        deep : bool, Optional
+            If `True` the parser goes into nested dictionaries.
+            Default is `True`
+
+        dtype : Any, Optional
+            Constrains the type of the returned objects.
+            Default is `None`, which means no restriction.
+
+        Returns
+        -------
+        generator
+            Returns a generator object.
+
+        Examples
+        --------
+        A simple example:
+
+        >>> from nddict import DeepDict
+        >>> data = DeepDict()
+        >>> data['a', 'b', 'c'] = 1
+        >>> [c.key for c in data.containers()]
+        ['a', 'b']
+
+        We can see, that dictionaries 'a' and 'b' are returned as containers, but 'c' 
+        isn't,  because it is not a parent, there are no deeper levels. 
+
+        >>> [c.key for c in data.containers(inclusive=True, deep=True)]
+        [None, 'a', 'b']
+
+        >>> [c.key for c in data.containers(inclusive=True, deep=False)]     
+        [None, 'a']
+
+        >>> [c.key for c in data.containers(inclusive=False, deep=True)]       
+        ['a', 'b']
+
+        >>> [c.key for c in data.containers(inclusive=False, deep=False)]      
+        ['a']
+
+        """
+        dtype = self.__class__ if dtype is None else dtype
+        return parsedicts(self, inclusive=inclusive, dtype=dtype, deep=deep)
+
+    def __getitem__(self, key):
+        try:
+            if issequence(key):
+                return parseaddress(self, key)
+            else:
+                return super().__getitem__(key)
+        except ValueError:
+            return self.__missing__(key)
+        except KeyError:
+            return self.__missing__(key)
+
+    def __setitem__(self, key, value):
+        try:
+            if issequence(key):
+                if not key[0] in self:
+                    d = self.__missing__(key[0])
+                else:
+                    d = self[key[0]]
+                if len(key) > 1:
+                    d.__setitem__(key[1:], value)
+                else:
+                    self[key[0]] = value
+            else:
+                if isinstance(value, DeepDict):
+                    value.__join_parent__(self, key)
+                return super().__setitem__(key, value)
+        except AttributeError:
+            raise RuntimeError(
+                "Target is of type '{}', which is not a container.".format(type(d)))
+        except KeyError:
+            return self.__missing__(key)
+
+    def __missing__(self, key):
+        if self.locked:
+            raise KeyError("Missing key : {}".format(key))
+        if issequence(key):
+            if key[0] not in self:
+                self[key[0]] = value = self.__class__()
+            else:
+                value = self[key[0]]
+            if len(key) > 1:
+                return value.__missing__(key[1:])
+            else:
+                return value
+        else:
+            self[key] = value = self.__class__()
+            return value
+        
+    def __reduce__(self):
+        return self.__class__, tuple(), None, None, self.items()
+    
+    def __repr__(self):
+        frmtstr = self.__class__.__name__ + '(%s)'
+        return frmtstr % (dict.__repr__(self))
+       
+    def __join_parent__(self, parent, key: Hashable = None):
+        self.parent = parent
+        self._root = parent.root()
+        self._key = key
+
+    def items(self, *args, deep=False, return_address=False, **kwargs):
+        if deep:
+            if return_address:
+                for addr, v in dictparser(self):
+                    yield addr, v
+            else:
+                for k, v in parseitems(self):
+                    yield k, v
+        else:
+            for k, v in super().items():
+                yield k, v
+
+    def values(self, *args, deep=False, return_address=False, **kwargs):
+        if deep:
+            if return_address:
+                for addr, v in dictparser(self):
+                    yield addr, v
+            else:
+                for _, v in parseitems(self):
+                    yield v
+        else:
+            for v in super().values():
+                yield v
+
+    def keys(self, *args, deep=False, return_address=False, **kwargs):
+        if deep:
+            if return_address:
+                for addr, _ in dictparser(self):
+                    yield addr
+            else:
+                for k, _ in parseitems(self):
+                    yield k
+        else:
+            for k in super().keys():
+                yield k
```

### Comparing `dewloosh.core-1.0.6/src/dewloosh/core/infix.py` & `dewloosh.core-1.0.9/src/dewloosh/core/infix.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-# -*- coding: utf-8 -*-
-from typing import Callable
-
-
-class Infix:
-    """
-    Implements a custom Infix operator using  the 
-    operators '<<', '>>' and '|'.
-
-    Example
-    -------
-        >>> x = Infix(lambda x, y: x * y)
-        >>> print(2 | x | 4)
-        8
-
-        >>> x = Infix(lambda x, y: x + y)
-        >>> print(2 << x >> 4)
-        6
-    """
-
-    def __init__(self, function: Callable):
-        self.function = function
-
-    def __ror__(self, other):
-        return Infix(lambda x, self=self, other=other: self.function(other, x))
-
-    def __or__(self, other):
-        return self.function(other)
-
-    def __rlshift__(self, other):
-        return Infix(lambda x, self=self, other=other: self.function(other, x))
-
-    def __rshift__(self, other):
-        return self.function(other)
-
-    def __call__(self, value1, value2):
+# -*- coding: utf-8 -*-
+from typing import Callable
+
+
+class Infix:
+    """
+    Implements a custom Infix operator using  the 
+    operators '<<', '>>' and '|'.
+
+    Example
+    -------
+        >>> x = Infix(lambda x, y: x * y)
+        >>> print(2 | x | 4)
+        8
+
+        >>> x = Infix(lambda x, y: x + y)
+        >>> print(2 << x >> 4)
+        6
+    """
+
+    def __init__(self, function: Callable):
+        self.function = function
+
+    def __ror__(self, other):
+        return Infix(lambda x, self=self, other=other: self.function(other, x))
+
+    def __or__(self, other):
+        return self.function(other)
+
+    def __rlshift__(self, other):
+        return Infix(lambda x, self=self, other=other: self.function(other, x))
+
+    def __rshift__(self, other):
+        return self.function(other)
+
+    def __call__(self, value1, value2):
         return self.function(value1, value2)
```

### Comparing `dewloosh.core-1.0.6/src/dewloosh/core/meta.py` & `dewloosh.core-1.0.9/src/dewloosh/core/meta.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,128 +1,128 @@
-# -*- coding: utf-8 -*-
-from abc import ABCMeta
-
-
-__all__ = ["ABCMeta_Weak", "ABCMeta_Strong", "ABCMeta_Safe"]
-
-
-def _is_callable(n, v): return callable(v) and ('__' not in n)
-
-
-class ABCMeta_Weak(ABCMeta):
-    """
-    Standard python metaclass. It follows weak abstraction in the meaning, that
-    it is enough to implement the abstarcts in the instance, they impose no
-    restriction on the inherited class itself. Therefore, error only occurs at
-    runtime.
-    """
-
-    @staticmethod
-    def _get_cls_methods(namespace, nomagic=False):
-        """
-        Returns the callable items in the namespace of the class.
-        If `nomagic=False`, magic functions with trailing double 
-        underscores are not returned.
-        """
-        if not nomagic:
-            return {name for name, value in namespace.items()
-                    if callable(value)}
-        else:
-            return {name for name, value in namespace.items()
-                    if _is_callable(name, value)}
-            
-    @staticmethod
-    def _get_cls_abstracts(namespace):
-        """
-        Returns the callable items in the namespace of the class.
-        If `nomagic=False`, magic functions with trailing double 
-        underscores are not returned.
-        """            
-        return getattr(namespace, "__abstractmethods__", set())
-            
-    @staticmethod
-    def _get_base_methods(bases):
-        """
-        Returns the callable items in the namespace of the class.
-        If `nomagic=False`, magic functions with trailing double 
-        underscores are not returned.
-        """
-        base_methods = {}
-        for base in bases:
-            base_methods[base.__name__] = {}
-            for k, v in base.__dict__.items():
-                if _is_callable(k, v):
-                    base_methods[base.__name__][k] = v
-        return base_methods
-                
-    @staticmethod
-    def _get_base_abstracts(bases):
-        """
-        Returns the callable items in the namespace of the class.
-        If `nomagic=False`, magic functions with trailing double 
-        underscores are not returned.
-        """
-        base_abc_methods = {}
-        for base in bases:
-            base_abc_methods[base.__name__] = \
-                getattr(base, "__abstractmethods__", set())
-        return base_abc_methods
-
-
-class ABCMeta_Strong(ABCMeta_Weak):
-    """
-    Strong Python metaclass. It follows strong abstraction in the meaning, that
-    an abstract function of any of the base classes must be implemented or
-    delayed with the use of another @abstractmethod decorator.
-    Error occurs at compilation time.
-    """
-
-    def __init__(self, name, bases, namespace, *args, **kwargs):
-        super().__init__(name, bases, namespace, *args, **kwargs)
-
-    def __new__(metaclass, name, bases, namespace, *args, **kwargs):
-        cls = super().__new__(metaclass, name, bases, namespace, *args,
-                              **kwargs)
-        cls_methods = metaclass._get_cls_methods(namespace)
-        for base in bases:
-            base_abstracts = set()
-            for name in getattr(base, "__abstractmethods__", set()):
-                value = getattr(cls, name, None)
-                if getattr(value, "__isabstractmethod__", False):
-                    base_abstracts.add(name)
-            for abstract in base_abstracts:
-                if abstract not in cls_methods:
-                    err_str = """Can't create abstract class {classname}!
-                    {classname} must implement abstract method {method} of
-                    class {base_class}!""".format(
-                        classname=name,
-                        method=abstract,
-                        base_class=base.__name__)
-                    raise TypeError(err_str)
-        return cls
-
-
-class ABCMeta_Safe(ABCMeta_Weak):
-    """
-    Python metaclass for safe inheritance. Throws a TypeError
-    if a method tries to shadow a definition in any of the base
-    classes.
-    """
-
-    def __init__(self, name, bases, namespace, *args, **kwargs):
-        super().__init__(name, bases, namespace, *args, **kwargs)
-
-    def __new__(metaclass, name, bases, namespace, *args, **kwargs):
-        cls = super().__new__(metaclass, name, bases, namespace, *args,
-                              **kwargs)
-        cls_methods = metaclass._get_cls_methods(namespace, nomagic=True)
-        for base in bases:
-            for method in cls_methods:
-                if hasattr(base, method):
-                    err_str = """Can't create abstract class {classname}!
-                        Method {method} is already implemented in class
-                        {base_class}!""".format(
-                        classname=name,
-                        method=method,
-                        base_class=base.__name__)
-                    raise TypeError(err_str)
+# -*- coding: utf-8 -*-
+from abc import ABCMeta
+
+
+__all__ = ["ABCMeta_Weak", "ABCMeta_Strong", "ABCMeta_Safe"]
+
+
+def _is_callable(n, v): return callable(v) and ('__' not in n)
+
+
+class ABCMeta_Weak(ABCMeta):
+    """
+    Standard python metaclass. It follows weak abstraction in the meaning, that
+    it is enough to implement the abstarcts in the instance, they impose no
+    restriction on the inherited class itself. Therefore, error only occurs at
+    runtime.
+    """
+
+    @staticmethod
+    def _get_cls_methods(namespace, nomagic=False):
+        """
+        Returns the callable items in the namespace of the class.
+        If `nomagic=False`, magic functions with trailing double 
+        underscores are not returned.
+        """
+        if not nomagic:
+            return {name for name, value in namespace.items()
+                    if callable(value)}
+        else:
+            return {name for name, value in namespace.items()
+                    if _is_callable(name, value)}
+            
+    @staticmethod
+    def _get_cls_abstracts(namespace):
+        """
+        Returns the callable items in the namespace of the class.
+        If `nomagic=False`, magic functions with trailing double 
+        underscores are not returned.
+        """            
+        return getattr(namespace, "__abstractmethods__", set())
+            
+    @staticmethod
+    def _get_base_methods(bases):
+        """
+        Returns the callable items in the namespace of the class.
+        If `nomagic=False`, magic functions with trailing double 
+        underscores are not returned.
+        """
+        base_methods = {}
+        for base in bases:
+            base_methods[base.__name__] = {}
+            for k, v in base.__dict__.items():
+                if _is_callable(k, v):
+                    base_methods[base.__name__][k] = v
+        return base_methods
+                
+    @staticmethod
+    def _get_base_abstracts(bases):
+        """
+        Returns the callable items in the namespace of the class.
+        If `nomagic=False`, magic functions with trailing double 
+        underscores are not returned.
+        """
+        base_abc_methods = {}
+        for base in bases:
+            base_abc_methods[base.__name__] = \
+                getattr(base, "__abstractmethods__", set())
+        return base_abc_methods
+
+
+class ABCMeta_Strong(ABCMeta_Weak):
+    """
+    Strong Python metaclass. It follows strong abstraction in the meaning, that
+    an abstract function of any of the base classes must be implemented or
+    delayed with the use of another @abstractmethod decorator.
+    Error occurs at compilation time.
+    """
+
+    def __init__(self, name, bases, namespace, *args, **kwargs):
+        super().__init__(name, bases, namespace, *args, **kwargs)
+
+    def __new__(metaclass, name, bases, namespace, *args, **kwargs):
+        cls = super().__new__(metaclass, name, bases, namespace, *args,
+                              **kwargs)
+        cls_methods = metaclass._get_cls_methods(namespace)
+        for base in bases:
+            base_abstracts = set()
+            for name in getattr(base, "__abstractmethods__", set()):
+                value = getattr(cls, name, None)
+                if getattr(value, "__isabstractmethod__", False):
+                    base_abstracts.add(name)
+            for abstract in base_abstracts:
+                if abstract not in cls_methods:
+                    err_str = """Can't create abstract class {classname}!
+                    {classname} must implement abstract method {method} of
+                    class {base_class}!""".format(
+                        classname=name,
+                        method=abstract,
+                        base_class=base.__name__)
+                    raise TypeError(err_str)
+        return cls
+
+
+class ABCMeta_Safe(ABCMeta_Weak):
+    """
+    Python metaclass for safe inheritance. Throws a TypeError
+    if a method tries to shadow a definition in any of the base
+    classes.
+    """
+
+    def __init__(self, name, bases, namespace, *args, **kwargs):
+        super().__init__(name, bases, namespace, *args, **kwargs)
+
+    def __new__(metaclass, name, bases, namespace, *args, **kwargs):
+        cls = super().__new__(metaclass, name, bases, namespace, *args,
+                              **kwargs)
+        cls_methods = metaclass._get_cls_methods(namespace, nomagic=True)
+        for base in bases:
+            for method in cls_methods:
+                if hasattr(base, method):
+                    err_str = """Can't create abstract class {classname}!
+                        Method {method} is already implemented in class
+                        {base_class}!""".format(
+                        classname=name,
+                        method=method,
+                        base_class=base.__name__)
+                    raise TypeError(err_str)
         return cls
```

### Comparing `dewloosh.core-1.0.6/src/dewloosh/core/signature.py` & `dewloosh.core-1.0.9/src/dewloosh/core/signature.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,197 +1,197 @@
-# -*- coding: utf-8 -*-
-from inspect import signature, Parameter
-from typing import Any
-from typing import Generic as _GenericAlias
-
-
-__all__ = ["Signature"]
-
-
-class Signature(dict):
-    """
-    A class to differentiate between function declarations using their
-    type signatures. It helps to decide if an implementation satisfies
-    some requirements imposed on a class.
-    """
-    
-    __abckey__ = 'isabstractoperation'
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(**kwargs)
-        setattr(self, 'isabstract', 'abstract' in args)
-
-    @classmethod
-    def from_function(cls, funcobj, *attrs, **kwargs):
-
-        if getattr(funcobj, cls.__abckey__, False):
-            sig = Signature('abstract', **kwargs)
-        else:
-            sig = Signature(**kwargs)
-
-        sig['name'] = funcobj.__name__
-        if len(attrs) > 0:
-            sig['attrs'] = frozenset(attrs)
-        else:
-            sig['attrs'] = frozenset()
-
-        params = signature(funcobj).parameters
-        if 'args' in params or 'kwargs' in params:
-            raise TypeError(
-                'Operation can only have a finite number of arguments!')
-        if 'self' in params or 'cls' in params:
-            sig['arity'] = len(params)-1
-        else:
-            sig['arity'] = len(params)
-
-        if sig['arity'] == 0:
-            sig['dtype'] = [Any]
-        else:
-            sig['dtype'] = []
-            for pname, param in params.items():
-                if pname not in ['self', 'cls']:
-                    if param.annotation is not Parameter.empty:
-                        sig['dtype'].append(param.annotation)
-                    else:
-                        sig['dtype'].append(Any)
-
-        annotations = funcobj.__annotations__
-        if 'return' in annotations:
-            sig['rtype'] = annotations['return']
-        else:
-            sig['rtype'] = Any
-
-        return sig
-
-    @classmethod
-    def from_property(cls, funcobj, **kwargs):
-
-        if funcobj.isabstractattribute:
-            sig = Signature('abstract', **kwargs)
-        else:
-            sig = Signature(**kwargs)
-
-        sig['name'] = funcobj.__name__
-
-        annotations = funcobj.__annotations__
-        if 'return' in annotations:
-            sig['rtype'] = annotations['return']
-        else:
-            sig['rtype'] = Any
-
-        return sig
-
-    def compatible_function(self, other: 'Signature') -> bool:
-        """
-        Returns True if two instances are compatible in terms of
-        domain type and result type.
-        """
-        if not isinstance(other, Signature):
-            return False
-
-        # check domain types
-        for type1, type2 in zip(self['dtype'], other['dtype']):
-            if type1 == Any:
-                continue
-            elif isinstance(type1, _GenericAlias):
-                if not isinstance(type2, _GenericAlias):
-                    typeargs = type1.__dict__['__args__']
-                    if type2 not in typeargs:
-                        return False
-                else:
-                    if type1 != type2:
-                        return False
-            else:
-                if type1 != type2:
-                    return False
-
-        # check result type
-        if isinstance(self['rtype'], _GenericAlias):
-            if not isinstance(other['rtype'], _GenericAlias):
-                typeargs = self['rtype'].__dict__['__args__']
-                if not other['rtype'] in typeargs:
-                    return False
-            else:
-                if self['rtype'] != other['rtype']:
-                    return False
-        elif self['rtype'] != Any:
-            if self['rtype'] != other['rtype']:
-                return False
-
-        return True
-
-    def accepts_property(self, other: 'Signature') -> bool:
-        """
-        Returns True if other (implemented operation's signature) is
-        compatible to self (abstract operation's signature).
-        Every value to every key of self must be present in other.
-        For example, here is where axioms are forced to match
-        between two signatures.
-        """
-        if any([not self.isabstract, other.isabstract]):
-            return False
-        if not self.compatible_op(other):
-            return False
-        if not self['name'] == other['name']:
-            return False
-
-        for key, value in self.items():
-            if key not in ['rtype', 'dtype']:
-                if key in other:
-                    if isinstance(value, frozenset) and \
-                            isinstance(other[key], frozenset):
-                        if not value.issubset(other[key]):
-                            return False
-                    else:
-                        if not value == other[key]:
-                            return False
-                else:
-                    return False
-        return True
-
-    def update_function(self, other: 'Signature'):
-        """
-        Updates self with the content of other. Both must be abstracts.
-        """
-        assert isinstance(other, Signature)
-        assert self.isabstract and other.isabstract
-        assert self.compatible_op(other)
-        for key, value in other.items():
-            if key not in ['rtype', 'dtype']:
-                if isinstance(value, frozenset):
-                    if key in self and isinstance(self[key], frozenset):
-                        s = set(self[key])
-                        s.update(set(value))
-                        self[key] = frozenset(s)
-                    else:
-                        self[key] = value
-                else:
-                    self[key] = value
-        return
-
-    def accepts_property(self, value: Any = None) -> bool:
-        """
-        Returns True if other (implemented attribute's signature) is
-        compatible to self (abstract attribute's signature).
-        Name and result type must match.
-        """
-        if not self.isabstract:
-            return False
-        if value is None:
-            return False
-
-        # check result type
-        if isinstance(self['rtype'], _GenericAlias):
-            if not isinstance(type(value), _GenericAlias):
-                typeargs = self['rtype'].__dict__['__args__']
-                if not type(value) in typeargs:
-                    return False
-            else:
-                if self['rtype'] != type(value):
-                    return False
-        elif self['rtype'] != Any:
-            if self['rtype'] != type(value):
-                return False
-        return True
-
-    def accepts_parameters(self, *args):
-        raise NotImplementedError
+# -*- coding: utf-8 -*-
+from inspect import signature, Parameter
+from typing import Any
+from typing import Generic as _GenericAlias
+
+
+__all__ = ["Signature"]
+
+
+class Signature(dict):
+    """
+    A class to differentiate between function declarations using their
+    type signatures. It helps to decide if an implementation satisfies
+    some requirements imposed on a class.
+    """
+    
+    __abckey__ = 'isabstractoperation'
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(**kwargs)
+        setattr(self, 'isabstract', 'abstract' in args)
+
+    @classmethod
+    def from_function(cls, funcobj, *attrs, **kwargs):
+
+        if getattr(funcobj, cls.__abckey__, False):
+            sig = Signature('abstract', **kwargs)
+        else:
+            sig = Signature(**kwargs)
+
+        sig['name'] = funcobj.__name__
+        if len(attrs) > 0:
+            sig['attrs'] = frozenset(attrs)
+        else:
+            sig['attrs'] = frozenset()
+
+        params = signature(funcobj).parameters
+        if 'args' in params or 'kwargs' in params:
+            raise TypeError(
+                'Operation can only have a finite number of arguments!')
+        if 'self' in params or 'cls' in params:
+            sig['arity'] = len(params)-1
+        else:
+            sig['arity'] = len(params)
+
+        if sig['arity'] == 0:
+            sig['dtype'] = [Any]
+        else:
+            sig['dtype'] = []
+            for pname, param in params.items():
+                if pname not in ['self', 'cls']:
+                    if param.annotation is not Parameter.empty:
+                        sig['dtype'].append(param.annotation)
+                    else:
+                        sig['dtype'].append(Any)
+
+        annotations = funcobj.__annotations__
+        if 'return' in annotations:
+            sig['rtype'] = annotations['return']
+        else:
+            sig['rtype'] = Any
+
+        return sig
+
+    @classmethod
+    def from_property(cls, funcobj, **kwargs):
+
+        if funcobj.isabstractattribute:
+            sig = Signature('abstract', **kwargs)
+        else:
+            sig = Signature(**kwargs)
+
+        sig['name'] = funcobj.__name__
+
+        annotations = funcobj.__annotations__
+        if 'return' in annotations:
+            sig['rtype'] = annotations['return']
+        else:
+            sig['rtype'] = Any
+
+        return sig
+
+    def compatible_function(self, other: 'Signature') -> bool:
+        """
+        Returns True if two instances are compatible in terms of
+        domain type and result type.
+        """
+        if not isinstance(other, Signature):
+            return False
+
+        # check domain types
+        for type1, type2 in zip(self['dtype'], other['dtype']):
+            if type1 == Any:
+                continue
+            elif isinstance(type1, _GenericAlias):
+                if not isinstance(type2, _GenericAlias):
+                    typeargs = type1.__dict__['__args__']
+                    if type2 not in typeargs:
+                        return False
+                else:
+                    if type1 != type2:
+                        return False
+            else:
+                if type1 != type2:
+                    return False
+
+        # check result type
+        if isinstance(self['rtype'], _GenericAlias):
+            if not isinstance(other['rtype'], _GenericAlias):
+                typeargs = self['rtype'].__dict__['__args__']
+                if not other['rtype'] in typeargs:
+                    return False
+            else:
+                if self['rtype'] != other['rtype']:
+                    return False
+        elif self['rtype'] != Any:
+            if self['rtype'] != other['rtype']:
+                return False
+
+        return True
+
+    def accepts_property(self, other: 'Signature') -> bool:
+        """
+        Returns True if other (implemented operation's signature) is
+        compatible to self (abstract operation's signature).
+        Every value to every key of self must be present in other.
+        For example, here is where axioms are forced to match
+        between two signatures.
+        """
+        if any([not self.isabstract, other.isabstract]):
+            return False
+        if not self.compatible_op(other):
+            return False
+        if not self['name'] == other['name']:
+            return False
+
+        for key, value in self.items():
+            if key not in ['rtype', 'dtype']:
+                if key in other:
+                    if isinstance(value, frozenset) and \
+                            isinstance(other[key], frozenset):
+                        if not value.issubset(other[key]):
+                            return False
+                    else:
+                        if not value == other[key]:
+                            return False
+                else:
+                    return False
+        return True
+
+    def update_function(self, other: 'Signature'):
+        """
+        Updates self with the content of other. Both must be abstracts.
+        """
+        assert isinstance(other, Signature)
+        assert self.isabstract and other.isabstract
+        assert self.compatible_op(other)
+        for key, value in other.items():
+            if key not in ['rtype', 'dtype']:
+                if isinstance(value, frozenset):
+                    if key in self and isinstance(self[key], frozenset):
+                        s = set(self[key])
+                        s.update(set(value))
+                        self[key] = frozenset(s)
+                    else:
+                        self[key] = value
+                else:
+                    self[key] = value
+        return
+
+    def accepts_property(self, value: Any = None) -> bool:
+        """
+        Returns True if other (implemented attribute's signature) is
+        compatible to self (abstract attribute's signature).
+        Name and result type must match.
+        """
+        if not self.isabstract:
+            return False
+        if value is None:
+            return False
+
+        # check result type
+        if isinstance(self['rtype'], _GenericAlias):
+            if not isinstance(type(value), _GenericAlias):
+                typeargs = self['rtype'].__dict__['__args__']
+                if not type(value) in typeargs:
+                    return False
+            else:
+                if self['rtype'] != type(value):
+                    return False
+        elif self['rtype'] != Any:
+            if self['rtype'] != type(value):
+                return False
+        return True
+
+    def accepts_parameters(self, *args):
+        raise NotImplementedError
```

### Comparing `dewloosh.core-1.0.6/src/dewloosh/core/tools/alphabet.py` & `dewloosh.core-1.0.9/src/dewloosh/core/tools/alphabet.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,52 +1,55 @@
-# -*- coding: utf-8 -*-
-from collections.abc import Iterable
-
-
-def alphabet(abctype: str = 'latin', **kwargs) -> Iterable:
-    if abctype in ('ord', 'o'):
-        start = kwargs.pop('start', 0)
-    elif abctype in ('latin', 'l'):
-        start = ord(kwargs.pop('start', 'a'))
-    elif abctype == 'u':
-        start = ord(kwargs.pop('start', '\u0000'))
-    elif abctype in ('greek', 'g'):
-        start = ord(kwargs.pop('start', '\u03b1'))
-    while True:
-        yield chr(start)
-        start += 1
-
-
-def ordrange(N: int = 1, **kwargs) -> Iterable:
-    start = kwargs.pop('start', 0)
-    if isinstance(start, str):
-        start = ord(start)
-    stop = kwargs.pop('stop', None)
-    if stop is None or stop == start:
-        stop = start + N
-    return [chr(c) for c in range(start, stop)]
-
-
-def latinrange(N: int = 1, **kwargs) -> Iterable:
-    start = kwargs.pop('start', 97)
-    stop = kwargs.pop('stop', None)
-    return ordrange(N, start=start, stop=stop)
-
-
-def urange(N: int = 1, **kwargs) -> Iterable:
-    start = kwargs.pop('start', '\u0000')
-    stop = kwargs.pop('stop', None)
-    if stop is None:
-        stop = start
-    return ordrange(N, start=ord(start), stop=ord(stop))
-
-
-def greekrange(N: int = 1) -> Iterable:
-    return urange(N, start='\u03b1')
-
-
-def arabicrange(N: int = 1, **kwargs) -> Iterable:
-    start = kwargs.pop('start', 0)
-    stop = kwargs.pop('stop', None)
-    if stop is None or stop == start:
-        stop = start + N
+# -*- coding: utf-8 -*-
+try:
+    from collections.abc import Iterable
+except ImportError:
+    from collections import Iterable
+
+
+def alphabet(abctype: str = 'latin', **kwargs) -> Iterable:
+    if abctype in ('ord', 'o'):
+        start = kwargs.pop('start', 0)
+    elif abctype in ('latin', 'l'):
+        start = ord(kwargs.pop('start', 'a'))
+    elif abctype == 'u':
+        start = ord(kwargs.pop('start', '\u0000'))
+    elif abctype in ('greek', 'g'):
+        start = ord(kwargs.pop('start', '\u03b1'))
+    while True:
+        yield chr(start)
+        start += 1
+
+
+def ordrange(N: int = 1, **kwargs) -> Iterable:
+    start = kwargs.pop('start', 0)
+    if isinstance(start, str):
+        start = ord(start)
+    stop = kwargs.pop('stop', None)
+    if stop is None or stop == start:
+        stop = start + N
+    return [chr(c) for c in range(start, stop)]
+
+
+def latinrange(N: int = 1, **kwargs) -> Iterable:
+    start = kwargs.pop('start', 97)
+    stop = kwargs.pop('stop', None)
+    return ordrange(N, start=start, stop=stop)
+
+
+def urange(N: int = 1, **kwargs) -> Iterable:
+    start = kwargs.pop('start', '\u0000')
+    stop = kwargs.pop('stop', None)
+    if stop is None:
+        stop = start
+    return ordrange(N, start=ord(start), stop=ord(stop))
+
+
+def greekrange(N: int = 1) -> Iterable:
+    return urange(N, start='\u03b1')
+
+
+def arabicrange(N: int = 1, **kwargs) -> Iterable:
+    start = kwargs.pop('start', 0)
+    stop = kwargs.pop('stop', None)
+    if stop is None or stop == start:
+        stop = start + N
     return [str(c) for c in range(start, stop)]
```

### Comparing `dewloosh.core-1.0.6/src/dewloosh/core/tools/dtk.py` & `dewloosh.core-1.0.9/src/dewloosh/core/tools/dtk.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-# -*- coding: utf-8 -*-
-from copy import copy
-
-
-def dictparser(d: dict = None, address=None, *args, dtype=dict, **kwargs):
-    """
-    Iterates through all the values of a nested dictionary.
-
-    Notes
-    -----
-        Returns all kinds of items, even nested discionaries themselves,
-        along with their content.
-    """
-    address = [] if address is None else address
-    for key, value in d.items():
-        subaddress = copy(address)
-        subaddress.append(key)
-        if isinstance(value, dtype):
-            for data in dictparser(value, subaddress, dtype=dtype):
-                yield data
-        else:
-            yield subaddress, value
-
-
-def parseaddress(d: dict, a: list):
-    if not isinstance(d, dict):
-        raise ValueError
-    if not a[0] in d:
-        raise KeyError(a[0])
-    if len(a) > 1:
-        return parseaddress(d[a[0]], a[1:])
-    else:
-        return d[a[0]]
-
-
-def parseitems(d: dict = None, *args, dtype=dict, **kwargs):
-    """
-    A generator function that yields all the items of a nested dictionary as
-    (key, value) pairs.
-
-    Notes
-    -----
-        Does not return nested dictionaries themselves, only their content.
-    """
-    for key, value in d.items():
-        if isinstance(value, dtype):
-            for data in parseitems(value, dtype=dtype):
-                yield data
-        else:
-            yield key, value
-
-
-def parsedicts(d: dict = None, *args, inclusive=True, dtype=dict,
-               deep=True, **kwargs):
-    if inclusive:
-        if isinstance(d, dtype):
-            yield d
-    for value in d.values():
-        if isinstance(value, dtype):
-            yield value
-            if deep:
-                for subvalue in \
-                        parsedicts(value, inclusive=False, dtype=dtype):
+# -*- coding: utf-8 -*-
+from copy import copy
+
+
+def dictparser(d: dict = None, address=None, *args, dtype=dict, **kwargs):
+    """
+    Iterates through all the values of a nested dictionary.
+
+    Notes
+    -----
+        Returns all kinds of items, even nested discionaries themselves,
+        along with their content.
+    """
+    address = [] if address is None else address
+    for key, value in d.items():
+        subaddress = copy(address)
+        subaddress.append(key)
+        if isinstance(value, dtype):
+            for data in dictparser(value, subaddress, dtype=dtype):
+                yield data
+        else:
+            yield subaddress, value
+
+
+def parseaddress(d: dict, a: list):
+    if not isinstance(d, dict):
+        raise ValueError
+    if not a[0] in d:
+        raise KeyError(a[0])
+    if len(a) > 1:
+        return parseaddress(d[a[0]], a[1:])
+    else:
+        return d[a[0]]
+
+
+def parseitems(d: dict = None, *args, dtype=dict, **kwargs):
+    """
+    A generator function that yields all the items of a nested dictionary as
+    (key, value) pairs.
+
+    Notes
+    -----
+        Does not return nested dictionaries themselves, only their content.
+    """
+    for key, value in d.items():
+        if isinstance(value, dtype):
+            for data in parseitems(value, dtype=dtype):
+                yield data
+        else:
+            yield key, value
+
+
+def parsedicts(d: dict = None, *args, inclusive=True, dtype=dict,
+               deep=True, **kwargs):
+    if inclusive:
+        if isinstance(d, dtype):
+            yield d
+    for value in d.values():
+        if isinstance(value, dtype):
+            yield value
+            if deep:
+                for subvalue in \
+                        parsedicts(value, inclusive=False, dtype=dtype):
                     yield subvalue
```

### Comparing `dewloosh.core-1.0.6/src/dewloosh/core/tools/kwargtools.py` & `dewloosh.core-1.0.9/src/dewloosh/core/tools/kwargtools.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,73 +1,76 @@
-# -*- coding: utf-8 -*-
-from collections.abc import Iterable
-from typing import Callable
-
-
-def isinkwargs(keys, **kwargs):
-    if isinstance(keys, Iterable) and not isinstance(keys, str):
-        return [key in kwargs for key in keys]
-    else:
-        return keys in kwargs
-
-
-def allinkwargs(keys, **kwargs):
-    if isinstance(keys, Iterable) and not isinstance(keys, str):
-        return all([key in kwargs for key in keys])
-    else:
-        return keys in kwargs
-
-
-def anyinkwargs(keys, **kwargs):
-    if isinstance(keys, Iterable) and not isinstance(keys, str):
-        return any([key in kwargs for key in keys])
-    else:
-        return keys in kwargs
-
-
-def getfromkwargs(keys, default=None, astype=None, **kwargs):
-    res = [kwargs.get(k, default) for k in keys]
-    if astype is None:
-        return res
-    else:
-        return [astype(p) for p in res]
-
-
-def popfromkwargs(keys, d: dict = None, *args, default=None, astype=None,
-                **kwargs):
-    res = [d.pop(k, default) for k in keys]
-    if astype is None:
-        return res
-    else:
-        return [astype(p) for p in res]
-
-
-def getallfromkwargs(keys, default=None, **kwargs):
-    params = getfromkwargs(keys, default=default, **kwargs)
-    if None not in params:
-        return params
-    else:
-        missing = list(filter(lambda p: p == default, params))
-        if len(missing) == 1:
-            key = keys[missing[0]]
-            raise RuntimeError("Parameter {} is missing from the definition!"
-                               .format(key))
-        else:
-            missing_keys = [keys[i] for i in missing]
-            raise RuntimeError("Parameters {} is missing from the definition!"
-                               .format(missing_keys))
-
-
-def getasany(keys, default=None, **kwargs):
-    try:
-        condition = [key in kwargs for key in keys]
-        if not any(condition) == True:
-            return default
-        return kwargs[keys[condition.index(True)]]
-    except Exception:
-        return None
-    
-
-def countkwargs(fnc: Callable, **kwargs):
-    assert callable(fnc)
-    return sum(list(map(fnc, kwargs.keys())))
-
+# -*- coding: utf-8 -*-
+try:
+    from collections.abc import Iterable
+except ImportError:
+    from collections import Iterable
+from typing import Callable
+
+
+def isinkwargs(keys, **kwargs):
+    if isinstance(keys, Iterable) and not isinstance(keys, str):
+        return [key in kwargs for key in keys]
+    else:
+        return keys in kwargs
+
+
+def allinkwargs(keys, **kwargs):
+    if isinstance(keys, Iterable) and not isinstance(keys, str):
+        return all([key in kwargs for key in keys])
+    else:
+        return keys in kwargs
+
+
+def anyinkwargs(keys, **kwargs):
+    if isinstance(keys, Iterable) and not isinstance(keys, str):
+        return any([key in kwargs for key in keys])
+    else:
+        return keys in kwargs
+
+
+def getfromkwargs(keys, default=None, astype=None, **kwargs):
+    res = [kwargs.get(k, default) for k in keys]
+    if astype is None:
+        return res
+    else:
+        return [astype(p) for p in res]
+
+
+def popfromkwargs(keys, d: dict = None, *args, default=None, astype=None,
+                **kwargs):
+    res = [d.pop(k, default) for k in keys]
+    if astype is None:
+        return res
+    else:
+        return [astype(p) for p in res]
+
+
+def getallfromkwargs(keys, default=None, **kwargs):
+    params = getfromkwargs(keys, default=default, **kwargs)
+    if None not in params:
+        return params
+    else:
+        missing = list(filter(lambda p: p == default, params))
+        if len(missing) == 1:
+            key = keys[missing[0]]
+            raise RuntimeError("Parameter {} is missing from the definition!"
+                               .format(key))
+        else:
+            missing_keys = [keys[i] for i in missing]
+            raise RuntimeError("Parameters {} is missing from the definition!"
+                               .format(missing_keys))
+
+
+def getasany(keys, default=None, **kwargs):
+    try:
+        condition = [key in kwargs for key in keys]
+        if not any(condition) == True:
+            return default
+        return kwargs[keys[condition.index(True)]]
+    except Exception:
+        return None
+    
+
+def countkwargs(fnc: Callable, **kwargs):
+    assert callable(fnc)
+    return sum(list(map(fnc, kwargs.keys())))
+
```

### Comparing `dewloosh.core-1.0.6/src/dewloosh/core/tools/tools.py` & `dewloosh.core-1.0.9/src/dewloosh/core/tools/tools.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,112 +1,112 @@
-# -*- coding: utf-8 -*-
-import time
-import sys
-from typing import Callable
-from ..typing import issequence
-
-
-__all__ = ['float_to_str_sig', 'floatformatter', 'issequence']
-
-
-def floatformatter(*args, sig: int=6, **kwargs) -> str:
-    """
-    Returns a formatter, which essantially a string temapate
-    ready to be formatted.
-    
-    Parameters
-    ----------
-    sig : int, Optional
-        Number of significant digits. Default is 6.
-        
-    Returns
-    -------
-    string
-        The string to be formatted.
-    
-    Examples
-    --------    
-    >>> from dewloosh.core import DeepDict
-    >>> data = DeepDict()
-    >>> data['a']['b']['c']['e'] = 1
-    >>> data['a']['b']['d'] = 2
-    >>> data.containers()
-            
-    """
-    return "{" + "0:.{}g".format(sig) + "}"
-
-
-def float_to_str_sig(value, *args, sig: int=6, atol: float=1e-7, 
-                     **kwargs) -> str:
-    """
-    Returns a string representation of a floating point number, with
-    given significant digits.
-
-    Parameters
-    ----------
-    value : float or a sequence of floats
-        A single value, or an iterable.
-
-    sig : int
-        Number of significant digits.
-
-    atol : float
-        Floating point tolerance. Values smaller than this 
-        in the absolute sense are treated as zero.
-
-    Returns
-    -------
-    string or a sequence of strings
-        String representation of the provided input.
-    
-    Example
-    --------
-    Print the value of pi as a string with 4 significant digits:
-    
-    >>> from dewloosh.core.tools import float_to_str_sig
-    >>> import math
-    >>> float_to_str_sig(math.pi, sig=4)
-    '3.142'
-    
-    """
-    if not issequence(value):
-        if atol is not None:
-            if abs(value) < atol:
-                value = 0.0
-        return floatformatter(sig=sig).format(value)
-    else:
-        try:
-            import numpy as np
-        except ImportError:
-            raise ImportError("You need numpy for this.")
-        value = np.array(value)
-        if atol is not None:
-            inds = np.where(np.abs(value) < atol)[0]
-            value[inds] = 0.0
-        formatter = floatformatter(sig=sig)
-        def f(v): return formatter.format(v)
-        return list(map(f, value))
-
-
-def timeit(fnc : Callable) -> float:
-    """
-    A simple decorator to measure execution time of a function.
-    """
-    def inner(*args, **kwargs):
-        t0 = time.time()
-        fnc(*args, **kwargs)
-        t1 = time.time()
-        return t1-t0
-    return inner
-
-
-def suppress(fnc: Callable) -> Callable:
-    """
-    Decorator that wraps a function to suppress it's calls to `print`.
-    """
-    def inner(*arg):
-        original_stdout = sys.stdout
-        sys.stdout = None
-        res = fnc(*arg)
-        sys.stdout = original_stdout
-        return res
+# -*- coding: utf-8 -*-
+import time
+import sys
+from typing import Callable
+from ..typing import issequence
+
+
+__all__ = ['float_to_str_sig', 'floatformatter', 'issequence']
+
+
+def floatformatter(*args, sig: int=6, **kwargs) -> str:
+    """
+    Returns a formatter, which essantially a string temapate
+    ready to be formatted.
+    
+    Parameters
+    ----------
+    sig : int, Optional
+        Number of significant digits. Default is 6.
+        
+    Returns
+    -------
+    string
+        The string to be formatted.
+    
+    Examples
+    --------    
+    >>> from dewloosh.core import DeepDict
+    >>> data = DeepDict()
+    >>> data['a']['b']['c']['e'] = 1
+    >>> data['a']['b']['d'] = 2
+    >>> data.containers()
+            
+    """
+    return "{" + "0:.{}g".format(sig) + "}"
+
+
+def float_to_str_sig(value, *args, sig: int=6, atol: float=1e-7, 
+                     **kwargs) -> str:
+    """
+    Returns a string representation of a floating point number, with
+    given significant digits.
+
+    Parameters
+    ----------
+    value : float or a sequence of floats
+        A single value, or an iterable.
+
+    sig : int
+        Number of significant digits.
+
+    atol : float
+        Floating point tolerance. Values smaller than this 
+        in the absolute sense are treated as zero.
+
+    Returns
+    -------
+    string or a sequence of strings
+        String representation of the provided input.
+    
+    Example
+    --------
+    Print the value of pi as a string with 4 significant digits:
+    
+    >>> from dewloosh.core.tools import float_to_str_sig
+    >>> import math
+    >>> float_to_str_sig(math.pi, sig=4)
+    '3.142'
+    
+    """
+    if not issequence(value):
+        if atol is not None:
+            if abs(value) < atol:
+                value = 0.0
+        return floatformatter(sig=sig).format(value)
+    else:
+        try:
+            import numpy as np
+        except ImportError:
+            raise ImportError("You need numpy for this.")
+        value = np.array(value)
+        if atol is not None:
+            inds = np.where(np.abs(value) < atol)[0]
+            value[inds] = 0.0
+        formatter = floatformatter(sig=sig)
+        def f(v): return formatter.format(v)
+        return list(map(f, value))
+
+
+def timeit(fnc : Callable) -> float:
+    """
+    A simple decorator to measure execution time of a function.
+    """
+    def inner(*args, **kwargs):
+        t0 = time.time()
+        fnc(*args, **kwargs)
+        t1 = time.time()
+        return t1-t0
+    return inner
+
+
+def suppress(fnc: Callable) -> Callable:
+    """
+    Decorator that wraps a function to suppress it's calls to `print`.
+    """
+    def inner(*arg):
+        original_stdout = sys.stdout
+        sys.stdout = None
+        res = fnc(*arg)
+        sys.stdout = original_stdout
+        return res
     return inner
```

### Comparing `dewloosh.core-1.0.6/src/dewloosh.core.egg-info/SOURCES.txt` & `dewloosh.core-1.0.9/src/dewloosh.core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

