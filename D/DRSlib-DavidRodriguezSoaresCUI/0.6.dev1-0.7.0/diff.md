# Comparing `tmp/DRSlib-DavidRodriguezSoaresCUI-0.6.dev1.tar.gz` & `tmp/DRSlib-DavidRodriguezSoaresCUI-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DRSlib-DavidRodriguezSoaresCUI-0.6.dev1.tar", last modified: Fri Jun 17 11:44:44 2022, max compression
+gzip compressed data, was "DRSlib-DavidRodriguezSoaresCUI-0.7.0.tar", last modified: Sat Apr 22 16:03:05 2023, max compression
```

## Comparing `DRSlib-DavidRodriguezSoaresCUI-0.6.dev1.tar` & `DRSlib-DavidRodriguezSoaresCUI-0.7.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2022-06-17 11:44:44.712023 DRSlib-DavidRodriguezSoaresCUI-0.6.dev1/
--rw-rw-rw-   0        0        0     6432 2021-11-14 15:06:03.000000 DRSlib-DavidRodriguezSoaresCUI-0.6.dev1/LICENSE
--rw-rw-rw-   0        0        0     3547 2022-06-17 11:44:44.712023 DRSlib-DavidRodriguezSoaresCUI-0.6.dev1/PKG-INFO
--rw-rw-rw-   0        0        0     2497 2021-11-28 13:21:49.000000 DRSlib-DavidRodriguezSoaresCUI-0.6.dev1/README.md
--rw-rw-rw-   0        0        0      114 2021-10-31 10:05:27.000000 DRSlib-DavidRodriguezSoaresCUI-0.6.dev1/pyproject.toml
--rw-rw-rw-   0        0        0     1105 2022-06-17 11:44:44.712023 DRSlib-DavidRodriguezSoaresCUI-0.6.dev1/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-06-17 11:44:44.643019 DRSlib-DavidRodriguezSoaresCUI-0.6.dev1/src/
-drwxrwxrwx   0        0        0        0 2022-06-17 11:44:44.680765 DRSlib-DavidRodriguezSoaresCUI-0.6.dev1/src/DRSlib/
--rw-rw-rw-   0        0        0      859 2022-06-17 11:34:50.000000 DRSlib-DavidRodriguezSoaresCUI-0.6.dev1/src/DRSlib/__init__.py
--rw-rw-rw-   0        0        0     5012 2021-11-08 11:11:51.000000 DRSlib-DavidRodriguezSoaresCUI-0.6.dev1/src/DRSlib/banner.py
--rw-rw-rw-   0        0        0     9345 2022-02-06 19:26:19.000000 DRSlib-DavidRodriguezSoaresCUI-0.6.dev1/src/DRSlib/cli_ui.py
--rw-rw-rw-   0        0        0     6156 2021-11-09 12:05:29.000000 DRSlib-DavidRodriguezSoaresCUI-0.6.dev1/src/DRSlib/debug.py
--rw-rw-rw-   0        0        0    10038 2021-12-12 14:31:56.000000 DRSlib-DavidRodriguezSoaresCUI-0.6.dev1/src/DRSlib/decorators.py
--rw-rw-rw-   0        0        0     1188 2021-11-08 10:12:56.000000 DRSlib-DavidRodriguezSoaresCUI-0.6.dev1/src/DRSlib/execute.py
--rw-rw-rw-   0        0        0    12839 2021-11-14 16:07:58.000000 DRSlib-DavidRodriguezSoaresCUI-0.6.dev1/src/DRSlib/fsdb.py
--rw-rw-rw-   0        0        0     4040 2021-11-08 16:02:09.000000 DRSlib-DavidRodriguezSoaresCUI-0.6.dev1/src/DRSlib/hash.py
--rw-rw-rw-   0        0        0     2940 2021-11-08 10:13:12.000000 DRSlib-DavidRodriguezSoaresCUI-0.6.dev1/src/DRSlib/interval.py
--rw-rw-rw-   0        0        0    15407 2021-11-16 13:21:26.000000 DRSlib-DavidRodriguezSoaresCUI-0.6.dev1/src/DRSlib/mediainfo.py
--rw-rw-rw-   0        0        0     1588 2021-11-14 12:29:59.000000 DRSlib-DavidRodriguezSoaresCUI-0.6.dev1/src/DRSlib/os_detect.py
--rw-rw-rw-   0        0        0    14263 2021-11-14 16:11:17.000000 DRSlib-DavidRodriguezSoaresCUI-0.6.dev1/src/DRSlib/path_tools.py
--rw-rw-rw-   0        0        0     2329 2021-11-08 10:13:40.000000 DRSlib-DavidRodriguezSoaresCUI-0.6.dev1/src/DRSlib/spinner.py
--rw-rw-rw-   0        0        0     4133 2021-11-08 10:13:57.000000 DRSlib-DavidRodriguezSoaresCUI-0.6.dev1/src/DRSlib/str_utils.py
--rw-rw-rw-   0        0        0     2891 2021-11-28 12:43:17.000000 DRSlib-DavidRodriguezSoaresCUI-0.6.dev1/src/DRSlib/utils.py
-drwxrwxrwx   0        0        0        0 2022-06-17 11:44:44.712023 DRSlib-DavidRodriguezSoaresCUI-0.6.dev1/src/DRSlib_DavidRodriguezSoaresCUI.egg-info/
--rw-rw-rw-   0        0        0     3547 2022-06-17 11:44:44.000000 DRSlib-DavidRodriguezSoaresCUI-0.6.dev1/src/DRSlib_DavidRodriguezSoaresCUI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      663 2022-06-17 11:44:44.000000 DRSlib-DavidRodriguezSoaresCUI-0.6.dev1/src/DRSlib_DavidRodriguezSoaresCUI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-17 11:44:44.000000 DRSlib-DavidRodriguezSoaresCUI-0.6.dev1/src/DRSlib_DavidRodriguezSoaresCUI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2022-06-17 11:44:44.000000 DRSlib-DavidRodriguezSoaresCUI-0.6.dev1/src/DRSlib_DavidRodriguezSoaresCUI.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-06-17 11:44:44.000000 DRSlib-DavidRodriguezSoaresCUI-0.6.dev1/src/DRSlib_DavidRodriguezSoaresCUI.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-22 16:03:05.910366 DRSlib-DavidRodriguezSoaresCUI-0.7.0/
+-rw-rw-rw-   0        0        0     6432 2021-11-14 15:06:03.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.0/LICENSE
+-rw-rw-rw-   0        0        0     3503 2023-04-22 16:03:05.910366 DRSlib-DavidRodriguezSoaresCUI-0.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2497 2021-11-28 13:21:49.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.0/README.md
+-rw-rw-rw-   0        0        0      114 2021-10-31 10:05:27.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1102 2023-04-22 16:03:05.915371 DRSlib-DavidRodriguezSoaresCUI-0.7.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-22 16:03:05.884484 DRSlib-DavidRodriguezSoaresCUI-0.7.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-22 16:03:05.896353 DRSlib-DavidRodriguezSoaresCUI-0.7.0/src/DRSlib/
+-rw-rw-rw-   0        0        0      697 2023-04-22 15:27:12.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.0/src/DRSlib/__init__.py
+-rw-rw-rw-   0        0        0     5046 2023-04-22 15:27:32.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.0/src/DRSlib/banner.py
+-rw-rw-rw-   0        0        0     9820 2023-04-22 15:27:32.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.0/src/DRSlib/cli_ui.py
+-rw-rw-rw-   0        0        0     6182 2023-04-22 15:27:32.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.0/src/DRSlib/debug.py
+-rw-rw-rw-   0        0        0     9731 2023-04-22 15:27:32.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.0/src/DRSlib/decorators.py
+-rw-rw-rw-   0        0        0     1370 2023-04-22 15:27:32.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.0/src/DRSlib/execute.py
+-rw-rw-rw-   0        0        0    13598 2023-04-22 15:31:18.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.0/src/DRSlib/fsdb.py
+-rw-rw-rw-   0        0        0     3931 2023-04-22 15:27:32.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.0/src/DRSlib/hash.py
+-rw-rw-rw-   0        0        0     3410 2023-04-22 08:30:58.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.0/src/DRSlib/interval.py
+-rw-rw-rw-   0        0        0    15531 2023-04-22 15:27:32.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.0/src/DRSlib/mediainfo.py
+-rw-rw-rw-   0        0        0     1568 2023-04-22 15:27:32.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.0/src/DRSlib/os_detect.py
+-rw-rw-rw-   0        0        0    13957 2023-04-22 15:33:39.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.0/src/DRSlib/path_tools.py
+-rw-rw-rw-   0        0        0     2266 2023-04-22 15:27:32.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.0/src/DRSlib/spinner.py
+-rw-rw-rw-   0        0        0     4188 2023-04-22 15:27:32.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.0/src/DRSlib/str_utils.py
+-rw-rw-rw-   0        0        0     4311 2023-04-22 15:27:32.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.0/src/DRSlib/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-22 16:03:05.910366 DRSlib-DavidRodriguezSoaresCUI-0.7.0/src/DRSlib_DavidRodriguezSoaresCUI.egg-info/
+-rw-rw-rw-   0        0        0     3503 2023-04-22 16:03:05.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.0/src/DRSlib_DavidRodriguezSoaresCUI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      663 2023-04-22 16:03:05.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.0/src/DRSlib_DavidRodriguezSoaresCUI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 16:03:05.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.0/src/DRSlib_DavidRodriguezSoaresCUI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-22 16:03:05.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.0/src/DRSlib_DavidRodriguezSoaresCUI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-22 16:03:05.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.0/src/DRSlib_DavidRodriguezSoaresCUI.egg-info/top_level.txt
```

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.6.dev1/LICENSE` & `DRSlib-DavidRodriguezSoaresCUI-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.6.dev1/PKG-INFO` & `DRSlib-DavidRodriguezSoaresCUI-0.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: DRSlib-DavidRodriguezSoaresCUI
-Version: 0.6.dev1
+Version: 0.7.0
 Summary: DRSlib - a set of utilities by DavidRodriguezSoaresCUI
 Home-page: https://github.com/DavidRodriguezSoaresCUI/DRSlib
 Author: DavidRodriguezSoaresCUI
 Author-email: fireblaze904+DRSlib@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/DavidRodriguezSoaresCUI/DRSlib/issues
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -70,9 +68,7 @@
 ## Warning to users
 
 **DRSlib** is a quickly evolving package, and author doesn't take any responsibility to maintain it or to keep
 its API stable, but will make a good faith effort to do so. Also, some of its code writes to the disk, so its use 
 may lead to data loss.
 
 Use it at your own risk.
-
-
```

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.6.dev1/README.md` & `DRSlib-DavidRodriguezSoaresCUI-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.6.dev1/setup.cfg` & `DRSlib-DavidRodriguezSoaresCUI-0.7.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,70 +1,69 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2044 5253 6c69 622d 4461 7669 6452   = DRSlib-DavidR
 00000020: 6f64 7269 6775 657a 536f 6172 6573 4355  odriguezSoaresCU
-00000030: 490d 0a76 6572 7369 6f6e 203d 2030 2e36  I..version = 0.6
-00000040: 2e64 6576 310d 0a61 7574 686f 7220 3d20  .dev1..author = 
-00000050: 4461 7669 6452 6f64 7269 6775 657a 536f  DavidRodriguezSo
-00000060: 6172 6573 4355 490d 0a61 7574 686f 725f  aresCUI..author_
-00000070: 656d 6169 6c20 3d20 6669 7265 626c 617a  email = fireblaz
-00000080: 6539 3034 2b44 5253 6c69 6240 676d 6169  e904+DRSlib@gmai
-00000090: 6c2e 636f 6d0d 0a64 6573 6372 6970 7469  l.com..descripti
-000000a0: 6f6e 203d 2044 5253 6c69 6220 2d20 6120  on = DRSlib - a 
-000000b0: 7365 7420 6f66 2075 7469 6c69 7469 6573  set of utilities
-000000c0: 2062 7920 4461 7669 6452 6f64 7269 6775   by DavidRodrigu
-000000d0: 657a 536f 6172 6573 4355 490d 0a6c 6f6e  ezSoaresCUI..lon
-000000e0: 675f 6465 7363 7269 7074 696f 6e20 3d20  g_description = 
-000000f0: 6669 6c65 3a20 5245 4144 4d45 2e6d 640d  file: README.md.
-00000100: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
-00000110: 6e5f 636f 6e74 656e 745f 7479 7065 203d  n_content_type =
-00000120: 2074 6578 742f 6d61 726b 646f 776e 0d0a   text/markdown..
-00000130: 7572 6c20 3d20 6874 7470 733a 2f2f 6769  url = https://gi
-00000140: 7468 7562 2e63 6f6d 2f44 6176 6964 526f  thub.com/DavidRo
-00000150: 6472 6967 7565 7a53 6f61 7265 7343 5549  driguezSoaresCUI
-00000160: 2f44 5253 6c69 620d 0a70 726f 6a65 6374  /DRSlib..project
-00000170: 5f75 726c 7320 3d20 0d0a 0942 7567 2054  _urls = ...Bug T
-00000180: 7261 636b 6572 203d 2068 7474 7073 3a2f  racker = https:/
-00000190: 2f67 6974 6875 622e 636f 6d2f 4461 7669  /github.com/Davi
-000001a0: 6452 6f64 7269 6775 657a 536f 6172 6573  dRodriguezSoares
-000001b0: 4355 492f 4452 536c 6962 2f69 7373 7565  CUI/DRSlib/issue
-000001c0: 730d 0a63 6c61 7373 6966 6965 7273 203d  s..classifiers =
-000001d0: 200d 0a09 4465 7665 6c6f 706d 656e 7420   ...Development 
-000001e0: 5374 6174 7573 203a 3a20 3320 2d20 416c  Status :: 3 - Al
-000001f0: 7068 610d 0a09 496e 7465 6e64 6564 2041  pha...Intended A
-00000200: 7564 6965 6e63 6520 3a3a 2044 6576 656c  udience :: Devel
-00000210: 6f70 6572 730d 0a09 4c69 6365 6e73 6520  opers...License 
-00000220: 3a3a 2043 4330 2031 2e30 2055 6e69 7665  :: CC0 1.0 Unive
-00000230: 7273 616c 2028 4343 3020 312e 3029 2050  rsal (CC0 1.0) P
-00000240: 7562 6c69 6320 446f 6d61 696e 2044 6564  ublic Domain Ded
-00000250: 6963 6174 696f 6e0d 0a09 4f70 6572 6174  ication...Operat
-00000260: 696e 6720 5379 7374 656d 203a 3a20 4f53  ing System :: OS
-00000270: 2049 6e64 6570 656e 6465 6e74 0d0a 0950   Independent...P
-00000280: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000290: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-000002a0: 2033 203a 3a20 4f6e 6c79 0d0a 0950 726f   3 :: Only...Pro
-000002b0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-000002c0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-000002d0: 2e36 0d0a 0950 726f 6772 616d 6d69 6e67  .6...Programming
-000002e0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-000002f0: 686f 6e20 3a3a 2033 2e37 0d0a 0950 726f  hon :: 3.7...Pro
-00000300: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000310: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000320: 2e38 0d0a 0950 726f 6772 616d 6d69 6e67  .8...Programming
-00000330: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000340: 686f 6e20 3a3a 2033 2e39 0d0a 0954 6f70  hon :: 3.9...Top
-00000350: 6963 203a 3a20 536f 6674 7761 7265 2044  ic :: Software D
-00000360: 6576 656c 6f70 6d65 6e74 203a 3a20 4c69  evelopment :: Li
-00000370: 6272 6172 6965 7320 3a3a 2050 7974 686f  braries :: Pytho
-00000380: 6e20 4d6f 6475 6c65 730d 0a0d 0a5b 6f70  n Modules....[op
-00000390: 7469 6f6e 735d 0d0a 7061 636b 6167 655f  tions]..package_
-000003a0: 6469 7220 3d20 0d0a 093d 2073 7263 0d0a  dir = ...= src..
-000003b0: 7061 636b 6167 6573 203d 2066 696e 643a  packages = find:
-000003c0: 0d0a 7079 7468 6f6e 5f72 6571 7569 7265  ..python_require
-000003d0: 7320 3d20 3e3d 332e 360d 0a69 6e73 7461  s = >=3.6..insta
-000003e0: 6c6c 5f72 6571 7569 7265 7320 3d20 0d0a  ll_requires = ..
-000003f0: 0973 656e 6432 7472 6173 680d 0a0d 0a5b  .send2trash....[
-00000400: 6f70 7469 6f6e 732e 7061 636b 6167 6573  options.packages
-00000410: 2e66 696e 645d 0d0a 7768 6572 6520 3d20  .find]..where = 
-00000420: 7372 630d 0a0d 0a5b 6567 675f 696e 666f  src....[egg_info
-00000430: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
-00000440: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
-00000450: 0a                                       .
+00000030: 490d 0a76 6572 7369 6f6e 203d 2030 2e37  I..version = 0.7
+00000040: 2e30 0d0a 6175 7468 6f72 203d 2044 6176  .0..author = Dav
+00000050: 6964 526f 6472 6967 7565 7a53 6f61 7265  idRodriguezSoare
+00000060: 7343 5549 0d0a 6175 7468 6f72 5f65 6d61  sCUI..author_ema
+00000070: 696c 203d 2066 6972 6562 6c61 7a65 3930  il = fireblaze90
+00000080: 342b 4452 536c 6962 4067 6d61 696c 2e63  4+DRSlib@gmail.c
+00000090: 6f6d 0d0a 6465 7363 7269 7074 696f 6e20  om..description 
+000000a0: 3d20 4452 536c 6962 202d 2061 2073 6574  = DRSlib - a set
+000000b0: 206f 6620 7574 696c 6974 6965 7320 6279   of utilities by
+000000c0: 2044 6176 6964 526f 6472 6967 7565 7a53   DavidRodriguezS
+000000d0: 6f61 7265 7343 5549 0d0a 6c6f 6e67 5f64  oaresCUI..long_d
+000000e0: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
+000000f0: 653a 2052 4541 444d 452e 6d64 0d0a 6c6f  e: README.md..lo
+00000100: 6e67 5f64 6573 6372 6970 7469 6f6e 5f63  ng_description_c
+00000110: 6f6e 7465 6e74 5f74 7970 6520 3d20 7465  ontent_type = te
+00000120: 7874 2f6d 6172 6b64 6f77 6e0d 0a75 726c  xt/markdown..url
+00000130: 203d 2068 7474 7073 3a2f 2f67 6974 6875   = https://githu
+00000140: 622e 636f 6d2f 4461 7669 6452 6f64 7269  b.com/DavidRodri
+00000150: 6775 657a 536f 6172 6573 4355 492f 4452  guezSoaresCUI/DR
+00000160: 536c 6962 0d0a 7072 6f6a 6563 745f 7572  Slib..project_ur
+00000170: 6c73 203d 200d 0a09 4275 6720 5472 6163  ls = ...Bug Trac
+00000180: 6b65 7220 3d20 6874 7470 733a 2f2f 6769  ker = https://gi
+00000190: 7468 7562 2e63 6f6d 2f44 6176 6964 526f  thub.com/DavidRo
+000001a0: 6472 6967 7565 7a53 6f61 7265 7343 5549  driguezSoaresCUI
+000001b0: 2f44 5253 6c69 622f 6973 7375 6573 0d0a  /DRSlib/issues..
+000001c0: 636c 6173 7369 6669 6572 7320 3d20 0d0a  classifiers = ..
+000001d0: 0944 6576 656c 6f70 6d65 6e74 2053 7461  .Development Sta
+000001e0: 7475 7320 3a3a 2033 202d 2041 6c70 6861  tus :: 3 - Alpha
+000001f0: 0d0a 0949 6e74 656e 6465 6420 4175 6469  ...Intended Audi
+00000200: 656e 6365 203a 3a20 4465 7665 6c6f 7065  ence :: Develope
+00000210: 7273 0d0a 094c 6963 656e 7365 203a 3a20  rs...License :: 
+00000220: 4343 3020 312e 3020 556e 6976 6572 7361  CC0 1.0 Universa
+00000230: 6c20 2843 4330 2031 2e30 2920 5075 626c  l (CC0 1.0) Publ
+00000240: 6963 2044 6f6d 6169 6e20 4465 6469 6361  ic Domain Dedica
+00000250: 7469 6f6e 0d0a 094f 7065 7261 7469 6e67  tion...Operating
+00000260: 2053 7973 7465 6d20 3a3a 204f 5320 496e   System :: OS In
+00000270: 6465 7065 6e64 656e 740d 0a09 5072 6f67  dependent...Prog
+00000280: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000290: 203a 3a20 5079 7468 6f6e 203a 3a20 3320   :: Python :: 3 
+000002a0: 3a3a 204f 6e6c 790d 0a09 5072 6f67 7261  :: Only...Progra
+000002b0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+000002c0: 3a20 5079 7468 6f6e 203a 3a20 332e 360d  : Python :: 3.6.
+000002d0: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
+000002e0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+000002f0: 203a 3a20 332e 370d 0a09 5072 6f67 7261   :: 3.7...Progra
+00000300: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000310: 3a20 5079 7468 6f6e 203a 3a20 332e 380d  : Python :: 3.8.
+00000320: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
+00000330: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000340: 203a 3a20 332e 390d 0a09 546f 7069 6320   :: 3.9...Topic 
+00000350: 3a3a 2053 6f66 7477 6172 6520 4465 7665  :: Software Deve
+00000360: 6c6f 706d 656e 7420 3a3a 204c 6962 7261  lopment :: Libra
+00000370: 7269 6573 203a 3a20 5079 7468 6f6e 204d  ries :: Python M
+00000380: 6f64 756c 6573 0d0a 0d0a 5b6f 7074 696f  odules....[optio
+00000390: 6e73 5d0d 0a70 6163 6b61 6765 5f64 6972  ns]..package_dir
+000003a0: 203d 200d 0a09 3d20 7372 630d 0a70 6163   = ...= src..pac
+000003b0: 6b61 6765 7320 3d20 6669 6e64 3a0d 0a70  kages = find:..p
+000003c0: 7974 686f 6e5f 7265 7175 6972 6573 203d  ython_requires =
+000003d0: 203e 3d33 2e36 0d0a 696e 7374 616c 6c5f   >=3.6..install_
+000003e0: 7265 7175 6972 6573 203d 200d 0a09 7365  requires = ...se
+000003f0: 6e64 3274 7261 7368 0d0a 0d0a 5b6f 7074  nd2trash....[opt
+00000400: 696f 6e73 2e70 6163 6b61 6765 732e 6669  ions.packages.fi
+00000410: 6e64 5d0d 0a77 6865 7265 203d 2073 7263  nd]..where = src
+00000420: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
+00000430: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
+00000440: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
```

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.6.dev1/src/DRSlib/__init__.py` & `DRSlib-DavidRodriguezSoaresCUI-0.7.0/src/DRSlib/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # package-level docstring
-__doc__ = '''
+"""
 DRSlib - a set of utilities by DavidRodriguezSoaresCUI
 ======================================================
 
 **DRSlib** is a Python package that provides a wide range of small
 yet powerful set of highly-reusable functions, classes,
 decorators, etc. Its main purpose is to provide high-level
 "building blocks" that accomplish simple tasks, facilitating
 the writing of elaborate scripts with limited code.
 
 License: see *LICENSE file*
 
 Author: **DavidRodriguezSoaresCUI**
 
 Check its `Github repository <https://github.com/DavidRodriguezSoaresCUI/DRSlib>`_ and its `Pypi project page <https://pypi.org/project/DRSlib-DavidRodriguezSoaresCUI/>`_ .
-'''
-__all__=['banner','cli_ui','debug','decorators','execute','fsdb','hash','interval','mediainfo','os_detect','path_tools','spinner','str_utils','utils']
+"""
```

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.6.dev1/src/DRSlib/banner.py` & `DRSlib-DavidRodriguezSoaresCUI-0.7.0/src/DRSlib/banner.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,133 +1,143 @@
-# module-level docstring
-__doc__='''
+"""
 Banner module
 =============
 
 Banners are text elements used in CLI interfaces. They use is
-mostly for easthetic purposes. This module provides banner 
+mostly for easthetic purposes. This module provides banner
 generators and a wrapper (to bannerize functions/classes)
 
 On formatters: two are provided
-All formatters should have signature `( title: str, width: int = DEFAULT_BANNER_WIDTH, one_line: bool = False ) -> str`
+All formatters should have signature `(title: str, width: int = DEFAULT_BANNER_WIDTH, one_line: bool = False) -> str`
 (or compatible) and (for formatters in banner.py) have an entry in global dictionnary `style_switch`.
-'''
- 
+"""
+
 from typing import Callable, Any, Union
 import functools
 import shutil
 from pathlib import Path
 
-DEFAULT_BANNER_WIDTH = min( shutil.get_terminal_size().columns, 40 )
+DEFAULT_BANNER_WIDTH = min(shutil.get_terminal_size().columns, 40)
+
 
-def full_style_formatter( title: str, width: int = DEFAULT_BANNER_WIDTH, one_line: bool = False ) -> str:
-    ''' Returns a "full style" banner in string representation '''
+def full_style_formatter(
+    title: str, width: int = DEFAULT_BANNER_WIDTH, one_line: bool = False
+) -> str:
+    """Returns a "full style" banner in string representation"""
     title_len = len(title)
-    d = int((width-title_len-2)/2) # number of # symbols on either side of the banner title
-    second_line = "{} {}{} {}".format(
-        '#'*d,
-        title,
-        ' ' if title_len%2==1 else '', # padding
-        '#'*d
+    padding = int((width - title_len - 2) / 2) * "#"
+    title_spacing = " " if title_len % 2 == 1 else ""
+    second_line = f"{padding} {title}{title_spacing} {padding}"
+
+    return (
+        second_line
+        if one_line
+        else "\n".join(["#" * width, second_line, "#" * width + "\n"])
     )
-    
-    return second_line if one_line else "\n".join([ 
-        '#' * width,
-        second_line,
-        '#' * width + '\n'
-    ])
 
-def lean_style_formatter( title: str, width: int = DEFAULT_BANNER_WIDTH, one_line: bool = False ) -> str:
-    ''' Returns a "lean style" banner in string representation '''
+
+def lean_style_formatter(
+    title: str, width: int = DEFAULT_BANNER_WIDTH, one_line: bool = False
+) -> str:
+    """Returns a "lean style" banner in string representation"""
     title_len = len(title)
-    d = int((width-title_len-2)/2) # number of space symbols on either side of the banner title
-    second_line = "#{}{}{}{}#".format(
-        ' '*d,
-        title,
-        ' ' if title_len%2==1 else '', # padding
-        ' '*d
+    padding = int((width - title_len - 2) / 2) * " "
+    title_spacing = " " if title_len % 2 == 1 else ""
+    second_line = f"#{padding}{title}{title_spacing}{padding}#"
+
+    return (
+        second_line
+        if one_line
+        else "\n".join(["#" * width, second_line, "#" * width + "\n"])
     )
-    
-    return second_line if one_line else "\n".join([ 
-        '#' * width,
-        second_line,
-        '#' * width + '\n'
-    ])
-
-
-style_switch = {
-    'full': full_style_formatter,
-    'lean': lean_style_formatter
-}
 
 
-def one_line_banner( title: str, style: Union[str,Callable] = 'full', width:int = DEFAULT_BANNER_WIDTH ) -> str:
-    ''' Returns a string containing a one-line banner
+style_switch = {"full": full_style_formatter, "lean": lean_style_formatter}
+
+
+def one_line_banner(
+    title: str, style: Union[str, Callable] = "full", width: int = DEFAULT_BANNER_WIDTH
+) -> str:
+    """Returns a string containing a one-line banner
     Available styles : 'full', 'lean'
-    External formatters: If style is Callable, it is assumed to be a formatter following 
+    External formatters: If style is Callable, it is assumed to be a formatter following
     signature norm (see module docstring)
-    '''
-    
-    style_formatter = style if callable(style) else style_switch[style]
-    banner = style_formatter( title=title, width=width, one_line=True )
-    return banner + '\n'
+    """
 
+    style_formatter: Callable = style if callable(style) else style_switch[style]  # type: ignore[assignment]
+    banner = style_formatter(title=title, width=width, one_line=True)
+    return banner + "\n"
 
-def multi_line_banner( title: str, style: Union[str,Callable] = 'full', width:int = DEFAULT_BANNER_WIDTH ) -> str:
-    ''' Returns a string containing a multi-line banner
+
+def multi_line_banner(
+    title: str, style: Union[str, Callable] = "full", width: int = DEFAULT_BANNER_WIDTH
+) -> str:
+    """Returns a string containing a multi-line banner
     Available styles : 'full', 'lean'
-    External formatters: If style is Callable, it is assumed to be a formatter following 
+    External formatters: If style is Callable, it is assumed to be a formatter following
     signature norm (see module docstring)
-    '''
-    
-    style_formatter = style if callable(style) else style_switch[style]
-    banner = style_formatter( title=title, width=width )
-    return banner + '\n'
+    """
+
+    style_formatter: Callable = style if callable(style) else style_switch[style]  # type: ignore[assignment]
+    banner = style_formatter(title=title, width=width)
+    return banner + "\n"
+
 
+def bannerize(
+    style: Union[Callable, str],
+    width: int = DEFAULT_BANNER_WIDTH,
+    one_line: bool = False,
+) -> Callable:
+    """Decorator. Adds a banner before function's execution. Not intended nor tested for decorating classes.
 
-def bannerize( style: Union[Callable,str], width: int = DEFAULT_BANNER_WIDTH, one_line: bool = False ) -> Callable:
-    ''' Decorator. Adds a banner before function's execution. Not intended nor tested for decorating classes.
-    
     When `style` is given and is a callable formatter, it will be used to produce banner, otherwise `style`
     must be a string equal to a key in `style_switch`, which defines the formatter to use.
-    
+
     Available styles : see style_switch
-    '''
+    """
 
-    def actual_decorator( user_funtion: Callable ) -> Callable:
-        ''' Sets up the banner to be displayed for user_function '''
-        nonlocal style_formatter, width, one_line
+    def actual_decorator(user_funtion: Callable) -> Callable:
+        """Sets up the banner to be displayed for user_function"""
+        nonlocal style_formatter, width, one_line  # type: ignore[misc]
 
         # Get name of the file containing `user_function`
-        file_path = user_funtion.__getattribute__('__globals__').get('__file__')
+        file_path = getattr(user_funtion.__globals__, "__file__")
         file_name = Path(file_path).stem
         # Setting the banner title
-        _banner = style_formatter( 
-            title=file_name if user_funtion.__name__=='main' else f"{file_name}.{user_funtion.__name__}",
+        _banner = style_formatter(
+            title=file_name
+            if user_funtion.__name__ == "main"
+            else f"{file_name}.{user_funtion.__name__}",
             width=width,
-            one_line=one_line
+            one_line=one_line,
         )
 
         @functools.wraps(user_funtion)
-        def wrapper( *args, **kwargs ) -> Any:
-            ''' Prints the banner for user_function and executes it '''
+        def wrapper(*args, **kwargs) -> Any:
+            """Prints the banner for user_function and executes it"""
             nonlocal _banner
 
             # Printing banner
-            print( _banner )
+            print(_banner)
 
-            return user_funtion( *args, **kwargs )
+            return user_funtion(*args, **kwargs)
 
         return wrapper
 
+    style_formatter: Callable
     if callable(style):
         # formatter passed
-        style_formatter = style 
+        style_formatter = style
     elif isinstance(style, str):
         # `style` argument passed => validation
-        style_formatter = style_switch.get( style )
-        if not style_formatter:
-            raise ValueError(f"bannerize: value for argument 'style' not recorgized: '{style}' not in {list(style_switch.keys())} !")
+        try:
+            style_formatter = style_switch[style]
+        except KeyError as e:
+            raise ValueError(
+                f"bannerize: value for argument 'style' not recorgized: '{style}' not in {list(style_switch.keys())} !"
+            ) from e
     else:
-        raise ValueError("bannerize: required value for 'style' is neither a formatter (Callable) nor a string.")
+        raise ValueError(
+            "bannerize: required value for 'style' is neither a formatter (Callable) nor a string."
+        )
 
     return actual_decorator
```

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.6.dev1/src/DRSlib/cli_ui.py` & `DRSlib-DavidRodriguezSoaresCUI-0.7.0/src/DRSlib/cli_ui.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,262 +1,299 @@
 # pylint: disable=eval-used, broad-except
 
-# module-level docstring
-__doc__='''
+
+"""
 Command line user interface
 ===========================
 
 Implements convenience function for CLI user interaction.
 Useful when you need to ask the user what to do, or select one
 of many options.
-'''
+"""
 
-from typing import Iterable, Union, Any, Callable, Dict, Optional
-from pathlib import Path
-import sys
+import ast
 import os
+import sys
+from pathlib import Path
+from typing import Any, Callable, Dict, Iterable, Optional, Union
 
 from .banner import one_line_banner
 from .os_detect import Os
-from .path_tools import folder_get_subdirs, windows_list_logical_drives, make_FS_safe
+from .path_tools import folder_get_subdirs, make_FS_safe, windows_list_logical_drives
+from .utils import assertTrue
 
 KBI_msg = "A KEYBOARDINTERRUPT WAS RAISED. THE PROGRAM WILL EXIT NOW."
 
-def __input_KBI( message: str, exit_on_KBI: bool = True ) -> str:
-    ''' Handles `KeyboardInterrupts` on `input` calls, used by other more complex functions.
+
+def __input_KBI(message: str, exit_on_KBI: bool = True) -> str:
+    """Handles `KeyboardInterrupts` on `input` calls, used by other more complex functions.
     `exit_on_KBI`: If True, user can exit the program. If False, handling
     of KeyboardInterrupt is delegated to calling code.
-    '''
+    """
     if exit_on_KBI:
         try:
-            return input( message )
+            return input(message)
         except KeyboardInterrupt:
-            print( KBI_msg )
+            print(KBI_msg)
             end_of_program()
-    return input( message )
+    return input(message)
 
 
 def pause() -> None:
-    ''' Implements a 'pause' feature. Press ENTER to continue. If 'Ctrl+C' is pressed, 
-    it exits the program '''
+    """Implements a 'pause' feature. Press ENTER to continue. If 'Ctrl+C' is pressed,
+    it exits the program"""
 
-    __input_KBI( "Press the <ENTER> key to continue...", exit_on_KBI=False )
+    __input_KBI("Press the <ENTER> key to continue...", exit_on_KBI=False)
 
 
-def end_of_program( exit_code: int = 0, halt: bool = False ) -> None:
-    ''' Standardized way of ending programs '''
+def end_of_program(exit_code: int = 0, halt: bool = False) -> None:
+    """Standardized way of ending programs"""
     print("\nEND OF PROGRAM\n")
     if halt:
         pause()
     sys.exit(exit_code)
 
 
-def yes_or_no( message: str, retry: bool = True, default: bool = None, exit_on_KBI: bool = True ) -> bool:
-    ''' User input fiels optimized for obtaining y/n answer.
+def yes_or_no(
+    message: str,
+    retry: bool = True,
+    default: Optional[bool] = None,
+    exit_on_KBI: bool = True,
+) -> bool:
+    """User input fiels optimized for obtaining y/n answer.
     Loops user input until `KeyboardInterrupt` is raised (hard exit) or user types correct answer.
     `default` is returned if user input is inconclusive and `retry` is False.
 
     eg::
 
-        >>> continue = yes_or_no( "Continue ?", retry=False, defalut=False )
+        >>> continue = yes_or_no("Continue ?", retry=False, defalut=False)
         'Continue ? (y/n): '
-        >>> confirm_date = yes_or_no( "Is the date correct ?" )
+        >>> confirm_date = yes_or_no("Is the date correct ?")
         'Is the date correct ? (y/n): '
-        
-    '''
-    if not retry:
-        assert default is not None and isinstance( default, bool )
+
+    """
+    if not retry and default is None:
+        raise ValueError("Can't have retry=False and default=None")
+
+    default_txt = "" if default is None else f" [default:{'y' if default else 'n'}]"
+    message_txt = f"{message} (y/n){default_txt}: "
 
     while True:
-        default_txt = ' [default:y]' if default is True else ( ' [default:n]' if default is False else '' )
-        raw_input = __input_KBI( 
-            f"{message} (y/n){default_txt}: ",
-            exit_on_KBI=exit_on_KBI
-        ).lower()
+        raw_input = __input_KBI(message_txt, exit_on_KBI=exit_on_KBI).lower()
 
-        if raw_input=='' and default is not None:
-            return default
-        if raw_input[0] == 'y':
+        if raw_input[0].lower() == "y":
             return True
-        if raw_input[0] == 'n':
+        if raw_input[0].lower() == "n":
             return False
         if retry:
             print("Invalid answer, try again")
             continue
-        return default
+        return default  # type: ignore[return-value]
 
 
-def user_input( prompt: str, accepted: Union[Iterable[Union[str,int]],Callable], default: Any = None ) -> str:
-    ''' Asks user for input, with restrictions on accpetable values.
+def user_input(
+    prompt: str,
+    accepted: Union[Iterable[Union[str, int]], Callable],
+    default: Optional[Any] = None,
+) -> str:
+    """Asks user for input, with restrictions on accpetable values.
     `prompt`: appropriate text asking the user for input. Should be straightforward and informative about the kind of data that is asked
     `accepted`: either a function testing if the user input is acceptable, or an iterable containing all acceptable values
     `default`: When given, if the user input is not acceptes, default is returned. When abscent, the user will be prompted again until either
     an accepted value is entered or a KeyboardInterrupt is raised.
     Note: this is only designed to retrieve values of the following types: str, int, float
-    '''
-    
+    """
+
     # Smart prompt reformat
     if default is not None:
         prompt += f"[default:{default}] "
-    if prompt[-1] == ':':
-        prompt += ' '
-    elif prompt[-2:]!=': ':
-        prompt += ': '
+    if prompt[-1] == ":":
+        prompt += " "
+    elif prompt[-2:] != ": ":
+        prompt += ": "
+
+    def acceptable_UI(ui: str) -> bool:
+        return accepted(ui) if callable(accepted) else (ui in accepted)
 
-    acceptable_UI = lambda ui: accepted(ui) if callable(accepted) else (ui in accepted)
-        
     while True:
         # main loop: ask user until an acceptable input is received, or a KeyboradInterrupt ends the program
-        _user_input = __input_KBI( prompt )
-        
+        _user_input = __input_KBI(prompt)
+
         # case: raw user input is accepted
-        if acceptable_UI( _user_input ):
+        if acceptable_UI(_user_input):
             return _user_input
-        
+
         # case: processed user input is accepted
-        variations = [ 'int(_user_input)', 'float(_user_input)', '_user_input.lower()' ]
+        variations = ["int(_user_input)", "float(_user_input)", "_user_input.lower()"]
         for variation in variations:
             try:
-                __user_input = eval( variation )
-                if acceptable_UI( __user_input ):
+                __user_input = ast.literal_eval(variation)
+                if acceptable_UI(__user_input):
                     return __user_input
             except (ValueError, AttributeError):
                 pass
-        
+
         # case: user input is not accepted AND there is a default
         if default is not None:
             return default
-        
+
         # case: user input is not accepted AND there is no default => notify user, ask again
-        print("Input '%s' is not a valid input. %s", _user_input, (f"Please choose one of : {accepted}" if not callable(accepted) else "") )
+        print(
+            "Input '%s' is not a valid input. %s",
+            _user_input,
+            (f"Please choose one of : {accepted}" if not callable(accepted) else ""),
+        )
 
 
-def choose_from_list( choices: list, default: int ) -> Any:
-    ''' Prints then asks the user to choose an item from a list
+def choose_from_list(choices: list, default: Optional[int]) -> Any:
+    """Prints then asks the user to choose an item from a list
     `default`
-    '''
+    """
     # Print choices
-    print( "Choices:\n  " + '\n  '.join([
-        f"[{idx}] {choice}"
-        for idx, choice in enumerate(choices)
-    ]) + '\n' )
+    print(
+        "Choices:\n  "
+        + "\n  ".join([f"[{idx}] {choice}" for idx, choice in enumerate(choices)])
+        + "\n"
+    )
 
     # Get user selection
-    idx = user_input( "Selection : ", accepted=list(range(len(choices))), default=default )
+    idx = int(
+        user_input("Selection : ", accepted=list(range(len(choices))), default=default)
+    )
 
     # Return choice
     return choices[idx]
 
 
-def select_action( choices: Dict[str,Callable], no_banner: bool = False, default: str = None, execute: bool = False ) -> Optional[Callable]:
-    ''' Asks the user to choose an action amongst a list of labeled actions. Returns a callable
+def select_action(
+    choices: Dict[str, dict[str, Union[str, Callable]]],
+    no_banner: bool = False,
+    default: Optional[str] = None,
+    execute: bool = False,
+) -> Optional[Callable]:
+    """Asks the user to choose an action amongst a list of labeled actions. Returns a callable
     corresponding to the chosen action if `execute` is False, executes it otherwise.
-    
+
     Example of `choices`::
 
         choices = {
             'q': {
                 'explanation': 'quit the program',
                 'action': <function that exits the program:Callable>
             },
             ...
         }
-    ''' 
+    """
 
     # Print banner
     if not no_banner:
-        banner = one_line_banner( "Selection menu" )
+        banner = one_line_banner("Selection menu")
         print(banner)
 
     accepted_inputs = choices.keys()
 
     # Print choices
-    choice_formatter = lambda choice: choice + ( f" - {choices[choice]['explanation']}" if 'explanation' in choices[choice] else '' )
-    print( "Choices:\n  " + '\n  '.join([
-        choice_formatter( choice )
-        for choice in accepted_inputs
-    ]) + '\n' )
-    
+    def choice_formatter(choice) -> str:
+        return choice + (
+            f" - {choices[choice]['explanation']}"
+            if "explanation" in choices[choice]
+            else ""
+        )
+
+    print(
+        "Choices:\n  "
+        + "\n  ".join([choice_formatter(choice) for choice in accepted_inputs])
+        + "\n"
+    )
+
     # Get user choice
-    _user_input = user_input( "Selection : ", accepted=accepted_inputs, default=default )
+    _user_input = user_input("Selection : ", accepted=accepted_inputs, default=default)
 
     # Return or execute corresponding callable
+    action: Callable = choices[_user_input]["action"]  # type: ignore[assignment]
+    assertTrue(
+        callable(action), "Expected action to be callable, found {}", type(action)
+    )
+
     if execute:
-        choices[_user_input]['action']()
+        action()
         return None
-    
-    return choices[_user_input]['action']
+
+    return action
 
 
-def cli_explorer( root_dir: Path = None, allow_mkdir: bool = True ) -> Path:
-    ''' Allows for the user to explore directories to select one.
-    '''
+def cli_explorer(root_dir: Optional[Path] = None, allow_mkdir: bool = True) -> Path:
+    """Allows for the user to explore directories to select one."""
 
-    sub_dirs = folder_get_subdirs( root_dir ) if root_dir else windows_list_logical_drives()
+    sub_dirs = (
+        folder_get_subdirs(root_dir) if root_dir else windows_list_logical_drives()
+    )
     cwd = root_dir
-    
+
     def get_parent():
         try:
             return cwd.parent
         except Exception:
             return None
 
     while True:
         print(f"cwd : {cwd}")
+        cwd_exists = cwd is not None and cwd.exists()
 
         # Craft selection list
-        selection_list = [ d.name if 0<len(d.name) else str(d) for d in sub_dirs ]
-        extra_options = list()
+        selection_list = [d.name if 0 < len(d.name) else str(d) for d in sub_dirs]
+        extra_options = []
         cwd_parent = get_parent()
         if cwd_parent:
-            extra_options.append('..')
-        if cwd:
-            extra_options.append('.')
+            extra_options.append("..")
+        if cwd_exists:
+            extra_options.append(".")
             if allow_mkdir:
-                extra_options.append('<Make new folder here>')
+                extra_options.append("<Make new folder here>")
 
         # ask user
-        next_dir = choose_from_list( 
+        next_dir = choose_from_list(
             choices=extra_options + selection_list,
-            default=extra_options.index('.') if '.' in extra_options else None 
+            default=extra_options.index(".") if "." in extra_options else None,
         )
-        
-        if next_dir=='..':
-            if cwd==cwd_parent:
+
+        if next_dir == "..":
+            if cwd == cwd_parent:
                 # happens when at the root of a drive on windows
                 sub_dirs = windows_list_logical_drives()
                 cwd = None
                 continue
             cwd = cwd_parent
-        elif next_dir=='.':
-            return cwd
-        elif next_dir=='<Make new folder here>':
+        elif next_dir == ".":
+            return cwd  # type: ignore[return-value]
+        elif next_dir == "<Make new folder here>":
             while True:
                 new_dir_name = user_input(
-                    prompt="New folder name",
-                    accepted=lambda x: isinstance(x, str)
+                    prompt="New folder name", accepted=lambda x: isinstance(x, str)
                 )
-                new_dir = cwd / make_FS_safe(new_dir_name.replace('.',''))
+                new_dir = cwd / make_FS_safe(new_dir_name.replace(".", ""))  # type: ignore[operator]
                 if new_dir.is_dir():
                     print(f"'{new_dir_name}' already exists !")
                     continue
                 new_dir.mkdir()
                 cwd = new_dir
                 break
         else:
-            cwd = sub_dirs[ selection_list.index( next_dir ) ]
-        sub_dirs = folder_get_subdirs( cwd )
+            cwd = sub_dirs[selection_list.index(next_dir)]
+
+        if cwd_exists:
+            sub_dirs = folder_get_subdirs(cwd)  # type: ignore[arg-type]
 
 
 def clear_screen() -> None:
-    ''' Clears the terminal screen, multi-platform '''
+    """Clears the terminal screen, multi-platform"""
     _os = Os()
     if _os.windows or _os.cygwin:
-        os.system( 'CLS' )
+        os.system("CLS")  # nosec
     elif _os.linux or _os.wsl:
-        os.system( 'clear' )
+        os.system("clear")  # nosec
 
 
-def skipNlines( n: int ) -> None:
-    ''' Skips n lines in the terminal; used for vertical whitespace '''
-    assert n>0, "drslib::skipNlines: Invalid number of lines entered : '{}'".format(n)
-    print('{}'.format('\n'*(n-1)))
+def skipNlines(n: int) -> None:
+    """Skips n lines in the terminal; used for vertical whitespace"""
+    assertTrue(n > 0, "Invalid number of lines entered : '{}'", n)
+    print("{}".format("\n" * (n - 1)))
```

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.6.dev1/src/DRSlib/debug.py` & `DRSlib-DavidRodriguezSoaresCUI-0.7.0/src/DRSlib/debug.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,168 +1,173 @@
-# module-level docstring
-__doc__='''
+"""
 Debugging utils
 ===============
 
 Deubgging is made easier with these convenience functions.
-'''
+"""
 
-from typing import Callable, Any, Union
+from typing import Callable, Any, Optional, Union
 import functools
 import re
 import shutil
 import traceback
 
-FUNC_RELEVANT_ATTR={
-    '__annotations__',
-    '__class__',
-    '__defaults__',
-    '__dict__',
-    '__doc__',
-    '__kwdefaults__',
-    '__module__',
-    '__name__',
-    '__qualname__'
+FUNC_RELEVANT_ATTR = {
+    "__annotations__",
+    "__class__",
+    "__defaults__",
+    "__dict__",
+    "__doc__",
+    "__kwdefaults__",
+    "__module__",
+    "__name__",
+    "__qualname__",
 }
 
-def func_attribute_printout( user_funtion: Callable ) -> None:
-    ''' Prints relevant attributes of `user_function`, with attribute name, value and type.
+
+def func_attribute_printout(user_funtion: Callable) -> None:
+    """Prints relevant attributes of `user_function`, with attribute name, value and type.
     Relevant attributes are in `FUNC_RELEVANT_ATTR`.
 
     Usage example: reviewing an unfamiliar imported function::
-    
+
         from some.module import foo
-        func_attribute_printout( foo )
-    
+        func_attribute_printout(foo)
+
     Output::
 
         foo.__annotations__ = ...
         [...]
         foo.__qualname__ = foo, type=str
-        
-    '''
+
+    """
     f_name = user_funtion.__name__
     for attr in dir(user_funtion):
         if attr in FUNC_RELEVANT_ATTR:
-            attr_val = user_funtion.__getattribute__(attr)
+            attr_val = getattr(user_funtion, attr)
             print(f"{f_name}.{attr} = {attr_val}, type={type(attr_val)}")
 
 
-regex_var_name_from_call = re.compile(r'\(\s*(?:var\s*=\s*)?([^,\ ]+).*\).*$')
+REGEX_VAR_NAME_FROM_CALL = re.compile(r"\(\s*(?:var\s*=\s*)?([^,\ ]+).*\).*$")
 
-def debug_var( var: Any, var_name: str = None ) -> None:
-    ''' Prints the name, value and type of a variable, typically used during development
+
+def debug_var(var: Any, var_name: Optional[str] = None) -> None:
+    """Prints the name, value and type of a variable, typically used during development
     for quick and easy type/value sanity checks.
 
     Warning: if debug_var is decorated, automatic variable name retrieval doesn't work !
              You will need to specify var_name.
 
-    Automatic variable name retrieval : in most situations `debug_var` should be able to 
+    Automatic variable name retrieval : in most situations `debug_var` should be able to
     retrieve the name of the variable using the `traceback` module. If it fails, simply
-    add it manually. This feature was inspired by code snippets from 
+    add it manually. This feature was inspired by code snippets from
     https://stackoverflow.com/questions/2749796/how-to-get-the-original-variable-name-of-variable-passed-to-a-function
 
     Usage example : you want to add a sanity check to a received value::
-    
+
         ...
         res = do_something()
-        debug_var( res )
+        debug_var(res)
         ...
 
     Output::
-    
+
         >>> DEBUG VAR: res=[1999, 2011] (list)
 
     Note : during development a different method for retrieving var_name automatically
     was found. It used the stack module. Unfortunately it was found to be
     significantly slower and to not have any significant advantage so it was removed.
     You can find the implementation here below::
-    
+
         # inspect method : similar but extract locals from frame(s) and try to find
         stack = inspect.stack()[2:]
         for frameinfos in stack:
             lcls = frameinfos.frame.f_locals
             for name in lcls:
                 if id(var) == id(lcls[name]):
                     var_name = name
                     break
             if var_name:
                 break
-    
+
 
     Performance : tested on a AMD 1700 using the standard Python 3.9 interpreter,
     which used only 1 execution thread. Executed 10 iteration in ~2ms and 100'000
     iterations in ~11.8s (~9 iter/ms). Figures for indicative purposes only.
-    '''
+    """
 
     # If `var_name` isn't specified, we try to retrieve this information
     if var_name is None:
         # traceback method : extract stack frame to retrieve call code ..
-        raw_call_traceback = traceback.extract_stack( limit=2 )[0]
+        raw_call_traceback = traceback.extract_stack(limit=2)[0]
         call_code_line = raw_call_traceback.line
         # .. then extract variable name from call to `debug_var` using regular expression (handles both args and kwargs)
-        var_name = regex_var_name_from_call.search(call_code_line).groups()[0]
+        if call_code_line:
+            var_name_match = REGEX_VAR_NAME_FROM_CALL.search(call_code_line)
+            if var_name_match:
+                var_name = var_name_match.groups()[0]
 
     if not var_name:
         var_name = "error:Couldn't determine variable name automatically. Pleasy try to pass variable name as argument."
-    print( f"DEBUG VAR: {var_name}={var} ({type(var)})")
+    print(f"DEBUG VAR: {var_name}={var} ({type(var)})")
 
 
-def call_progress( expected_argument: Union[Callable,str] ) -> Callable:
-    ''' Decorator. Typically used to make the execution status of 
+def call_progress(expected_argument: Union[Callable, str]) -> Callable:
+    """Decorator. Typically used to make the execution status of
     a function verbose when developping.
     The decorated function's execution is enclosed in a text-based
-    box, with pre/post-execution message. 
+    box, with pre/post-execution message.
 
     `expected_argument`: Optional string argument, replaces the default
     message (user_function.__name__).
 
     Usage example: decorating debug_var (see warning in debug_var's docstring)::
-    
+
         decorated_debug_var = call_progress("debug_var debugs a variable")(debug_var)
         hello='world'
-        decorated_debug_var( var=hello, var_name='hello' )
+        decorated_debug_var(var=hello, var_name='hello')
 
     Output::
 
         ----------------------------------------
         debug_var debugs a variable ..
         DEBUG VAR: hello=world (<class 'str'>)
         debug_var debugs a variable done
         ----------------------------------------
-    
-    
+
+
     Note: this example is not great: decorating manually (not with @call_progress syntax)
     and decorating a function that specifically advises against decoration. But this showcases
     an actual use case that works.
-    '''
-
-    def actual_decorator( user_function: Callable ) -> Callable:
+    """
 
-        @functools.wraps( user_function )
-        def wrapper( *args, **kwargs ) -> Any:
+    def actual_decorator(user_function: Callable) -> Callable:
+        @functools.wraps(user_function)
+        def wrapper(*args, **kwargs) -> Any:
             nonlocal user_function
 
-            box_W = min( shutil.get_terminal_size().columns, 40 )
-            
-            print( '-' * box_W )
-            print( printout_text + ' ..' )
-            res = user_function( *args, **kwargs )
-            print( printout_text + ' done' )
-            print( '-' * box_W )
+            box_width = min(shutil.get_terminal_size().columns, 40)
+
+            print("-" * box_width)
+            print(printout_text + " ..")
+            res = user_function(*args, **kwargs)
+            print(printout_text + " done")
+            print("-" * box_width)
 
             return res
 
         return wrapper
 
-    if callable( expected_argument ):
-        # decorator_with_arguments was run without argument => use 
+    if callable(expected_argument):
+        # decorator_with_arguments was run without argument => use
         # default values for expected arguments or raise error
         user_function = expected_argument
         printout_text = user_function.__name__
         return actual_decorator(user_function)
 
     if isinstance(expected_argument, str):
         printout_text = expected_argument
         return actual_decorator
 
-    raise ValueError(f"call_progress: `expected_argument` of type {type(expected_argument)} is not in Union[Callable,str] !")
+    raise ValueError(
+        f"call_progress: `expected_argument` of type {type(expected_argument)} is not in Union[Callable,str] !"
+    )
```

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.6.dev1/src/DRSlib/decorators.py` & `DRSlib-DavidRodriguezSoaresCUI-0.7.0/src/DRSlib/decorators.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,364 +1,358 @@
-# module-level docstring
-__doc__='''
+"""
 General-purpose decorators
 ==========================
 
 This file contains useful (function) decorators !
 
 Also, you can find :
  - a structure convention for all function decorators
  - tests for each decorator (see at the bottom of the file; run the file to execute them)
 
-'''
+"""
 
-from typing import Any, Callable, Union
-import time
+import cProfile
 import datetime
+import functools
 import logging
-from pathlib import Path
 import pickle
+import pstats
+import time
+from pathlib import Path
+from typing import Any, Callable, Union
 
-# functool.wraps is a decorator for wrappers that copies informations from 
-# the original function to the wrapper, allowing for transparently chaining decorators
-import functools
-# for profiling
-import cProfile
-import pstats 
-
+from .utils import assertTrue
 
 ########### CONVENTION ###########
-# Any decorator in this file must 
+# Any decorator in this file must
 # follow this format; please use it
 # as a template :
 ########### CONVENTION ###########
 
-def decorator_without_argument( user_function: Callable ) -> Callable:
-    '''
+
+def decorator_without_argument(user_function: Callable) -> Callable:
+    """
     DOCSTRING
-    '''
+    """
 
     # maybe do something here
 
-    @functools.wraps( user_function )
-    def wrapper( *args, **kwargs ) -> Any:
+    @functools.wraps(user_function)
+    def wrapper(*args, **kwargs) -> Any:
         nonlocal user_function
 
         # maybe do something before calling f
-        res = user_function( *args, **kwargs )
+        res = user_function(*args, **kwargs)
         # maybe do something after calling f
         return res
 
     return wrapper
-    
 
-def decorator_with_arguments( expected_argument: Any ) -> Callable:
-    '''
-    DOCSTRING
-    '''
 
-    def actual_decorator( user_function: Callable ) -> Callable:
+def decorator_with_arguments(expected_argument: Any) -> Callable:
+    """
+    DOCSTRING
+    """
 
+    def actual_decorator(user_function: Callable) -> Callable:
         # maybe do something here
 
-        @functools.wraps( user_function )
-        def wrapper( *args, **kwargs ) -> Any:
+        @functools.wraps(user_function)
+        def wrapper(*args, **kwargs) -> Any:
             nonlocal user_function
-            
+
             # maybe do something before calling f
-            res = user_function( *args, **kwargs )
+            res = user_function(*args, **kwargs)
             # maybe do something after calling f
 
             return res
 
         return wrapper
 
-    if callable( expected_argument ):
-        # decorator_with_arguments was run without argument => use 
+    if callable(expected_argument):
+        # decorator_with_arguments was run without argument => use
         # default values for expected arguments or raise error
         user_function = expected_argument
         return actual_decorator(user_function)
 
     # decorator_with_arguments was run with argument (maybe do something here)
 
     return actual_decorator
 
 
 ########### progress tracking ###########
 
-def call_progress( message: str ) -> Callable:
-    ''' Prints progress of a callable to stdout
-    '''
 
-    def actual_decorator( user_function: Callable ) -> Callable:
+def call_progress(message: str) -> Callable:
+    """Prints progress of a callable to stdout"""
 
+    def actual_decorator(user_function: Callable) -> Callable:
         # maybe do something here
 
-        @functools.wraps( user_function )
-        def wrapper( *args, **kwargs ) -> Any:
+        @functools.wraps(user_function)
+        def wrapper(*args, **kwargs) -> Any:
             nonlocal user_function, message
-            
-            print("-"*40)
-            print( message + ' ..' )
-            res = user_function( *args, **kwargs )
-            print( message + ' OK!' )
-            print("-"*40)
+
+            print("-" * 40)
+            print(message + " ..")
+            res = user_function(*args, **kwargs)
+            print(message + " OK!")
+            print("-" * 40)
 
             return res
 
         return wrapper
 
-    assert isinstance( message, str ), "message must be a string"
+    assertTrue(isinstance(message, str), "message must be a string")
 
     return actual_decorator
 
 
 ########### timing ###########
 
-def timer( user_function: Callable ) -> Callable:
-    '''
+
+def timer(user_function: Callable) -> Callable:
+    """
     Prints how much time user function took to run
-    '''
+    """
 
-    @functools.wraps( user_function )
-    def wrapper( *args, **kwargs ) -> Any:
+    @functools.wraps(user_function)
+    def wrapper(*args, **kwargs) -> Any:
         nonlocal user_function
 
         t_start = time.time()
-        res = user_function( *args, **kwargs )
-        elapsed_ms = int( 1000 * (time.time() - t_start) )
+        res = user_function(*args, **kwargs)
+        elapsed_ms = int(1000 * (time.time() - t_start))
         print(f"Function {user_function.__name__} ran for {elapsed_ms}ms.")
         return res
 
     return wrapper
 
 
-def profile( user_function: Callable ) -> Callable:
-    ''' Profiling is an advanced technique to measure
-    code execution time. 
+def profile(user_function: Callable) -> Callable:
+    """Profiling is an advanced technique to measure
+    code execution time.
 
     This decorator was heavily inspired from mCoding's video:
     https://www.youtube.com/watch?v=m_a0fN48Alw
 
     Using PROF output file : you need the `snakeviz` package
     installed (`pip install snakeviz`). Simply type
     `snakeviz <profile file>`
-    in a terminal and you should see a web browser window with 
+    in a terminal and you should see a web browser window with
     visualizations of the profile.
-    '''
+    """
 
-    @functools.wraps( user_function )
-    def wrapper( *args, **kwargs ) -> Any:
+    @functools.wraps(user_function)
+    def wrapper(*args, **kwargs) -> Any:
         nonlocal user_function
 
         # Create profiler and run user function
         with cProfile.Profile() as _profile:
-            res = user_function( *args, **kwargs )
-        
+            res = user_function(*args, **kwargs)
+
             # Store results
-            stats = pstats.Stats( _profile )
-            stats.sort_stats( pstats.SortKey.TIME )
-            stats.dump_stats(filename=f'profile_{user_function.__name__}.prof')
+            stats = pstats.Stats(_profile)
+            stats.sort_stats(pstats.SortKey.TIME)
+            stats.dump_stats(filename=f"profile_{user_function.__name__}.prof")
 
         return res
 
     return wrapper
 
 
-def minimum_duration( min_duration_s: Union[float,int] ) -> Callable:
-    ''' Makes sure the callable's execution takes no less than
+def minimum_duration(min_duration_s: Union[float, int]) -> Callable:
+    """Makes sure the callable's execution takes no less than
     ``min_duration_s`` seconds to execute, using the ``time``
     library's functions.
 
     Usage example: Avoid getting banned for spamming requests::
 
-        ban_safe_urlopen = minimum_duration( min_duration_s=0.5 )( urllib.request.urlopen )
+        ban_safe_urlopen = minimum_duration(min_duration_s=0.5)(urllib.request.urlopen)
         for url in URLs:
             with ban_safe_urlopen(url) as f:
                 ...
-        
-    '''
 
-    def actual_decorator( user_function: Callable ) -> Callable:
+    """
 
-        @functools.wraps( user_function )
-        def wrapper( *args, **kwargs ) -> Any:
+    def actual_decorator(user_function: Callable) -> Callable:
+        @functools.wraps(user_function)
+        def wrapper(*args, **kwargs) -> Any:
             nonlocal user_function, min_duration_s
-            
+
             start_time = time.time()
-            res = user_function( *args, **kwargs )
+            res = user_function(*args, **kwargs)
             time_to_skip = min_duration_s - (time.time() - start_time)
             if time_to_skip > 0:
-                time.sleep( time_to_skip )
+                time.sleep(time_to_skip)
 
             return res
 
         return wrapper
 
-    assert isinstance( min_duration_s, (float,int) ), "minimum_duration: Omitted parameter `min_duration_s`."
+    assertTrue(
+        isinstance(min_duration_s, (float, int)),
+        "minimum_duration: Omitted parameter `min_duration_s`.",
+    )
 
     return actual_decorator
 
 
 ########### logging ###########
 
 
-def log_to_file( user_function: Callable ) -> Callable:
-    '''
+def log_to_file(user_function: Callable) -> Callable:
+    """
     Logs function call to file
-    '''
-    
-    logging.basicConfig( 
-        filename=f"{user_function.__name__}.log",
-        level=logging.INFO
-    )
-    _log = logging.getLogger( user_function.__name__ )
+    """
+
+    logging.basicConfig(filename=f"{user_function.__name__}.log", level=logging.INFO)
+    _log = logging.getLogger(user_function.__name__)
 
-    @functools.wraps( user_function )
-    def wrapper( *args, **kwargs ) -> Any:
+    @functools.wraps(user_function)
+    def wrapper(*args, **kwargs) -> Any:
         nonlocal user_function
 
-        str_args = ', '.join([
-            str(arg) 
-            for arg in args
-        ])
+        str_args = ", ".join([str(arg) for arg in args])
         _now = datetime.datetime.now()
-        res = user_function( *args, **kwargs )
+        res = user_function(*args, **kwargs)
 
         _log.info(
-            "Called function %s with args=[%s] and kwargs=%s at %s, with return value %s.", 
+            "Called function %s with args=[%s] and kwargs=%s at %s, with return value %s.",
             user_function.__name__,
             str_args,
             kwargs,
             _now,
-            res
+            res,
         )
-        
+
         return res
 
     return wrapper
 
 
 ########### caching ###########
 
 
-def cacheFS( cache_file: Path ) -> Callable:
-    '''
+def cacheFS(cache_file_or_args: Union[Path, Any]) -> Callable:
+    """
     Returns a decorator that caches the returned value of user function using a cache file.
-    '''
+    """
+
+    def actual_decorator(user_function: Callable) -> Callable:
+        """Caches the returned value of user function using a cache file."""
 
-    def actual_decorator( user_function: Callable ) -> Callable:
-        ''' Caches the returned value of user function using a cache file. '''
+        @functools.wraps(user_function)
+        def wrapper(*args, **kwargs) -> Any:
+            nonlocal user_function, cache_file, cached_data  # type: ignore[misc]
 
-        @functools.wraps( user_function )
-        def wrapper( *args, **kwargs ) -> Any:
-            nonlocal user_function, cache_file, cached_data
-            
             k = (args, frozenset(kwargs.items()))
             if k in cached_data:
                 # cache hit
-                print(f"Cache hit for {user_function.__name__} with args={args} and kwargs={kwargs}.")
+                print(
+                    f"Cache hit for {user_function.__name__} with args={args} and kwargs={kwargs}."
+                )
                 return cached_data[k]
-            
+
             # else: cache miss
-            res = user_function( *args, **kwargs )
+            res = user_function(*args, **kwargs)
             cached_data[k] = res
-            with cache_file.open( mode='wb' ) as f:
-                pickle.dump( cached_data, f ) # update cache
-            
+            with cache_file.open(mode="wb") as f:
+                pickle.dump(cached_data, f)  # update cache
+
             print(f"Written cache to file '{cache_file}'.")
 
             return res
 
         return wrapper
 
-
-    def load_cached_data( cache_file: Path ) -> dict:
+    def load_cached_data(cache_file: Path) -> dict:
         if cache_file.is_file():
             try:
-                with cache_file.open( mode='rb' ) as f:
-                    cached_data = pickle.load( f )
+                with cache_file.open(mode="rb") as f:
+                    cached_data = pickle.load(f)
             except EOFError:
-                pass # cache file exists but doesn't contain anything/valid data
+                pass  # cache file exists but doesn't contain anything/valid data
             else:
                 return cached_data
-        return dict()
+        return {}
 
+    cached_data: dict
+    cached_file: Path
 
-    if callable( cache_file ):
+    if callable(cache_file_or_args):
         # cacheFS was run without argument => default filename
-        user_function = cache_file
-        cache_file = Path( f"{user_function.__name__}.cacheFS" )
-        cached_data = load_cached_data( cache_file )
-        return actual_decorator(user_function)
+        cache_file = Path(f"{cache_file_or_args.__name__}.cacheFS")
+        cached_data = load_cached_data(cache_file)
+        return actual_decorator(cache_file_or_args)
 
     # else: cacheFS was run with argument
     # File Extension enforcement
-    if cache_file.suffix != '.cacheFS':
-        cache_file = Path( f'{cache_file}.cacheFS' )
+    if cache_file_or_args.suffix != ".cacheFS":
+        cache_file = Path(f"{cache_file}.cacheFS")
 
-    cached_data = load_cached_data( cache_file )
+    cached_data = load_cached_data(cache_file)
 
     return actual_decorator
 
 
 ########### end of decorators ###########
 
 
-if __name__=="__main__":
+if __name__ == "__main__":
 
     def vspace():
-        ''' just prints newlines '''
-        print( '\n' * 2 )
+        """just prints newlines"""
+        print("\n" * 2)
 
     # Tests
 
     # Test 01
     vspace()
     print("Test 01 : decorator 'timer'")
 
     @timer
     def wait2s() -> None:
-        ''' Just wait 2s '''
+        """Just wait 2s"""
         time.sleep(2)
 
     print(wait2s)
     print(wait2s.__doc__)
     wait2s()
 
     # Test 02
     vspace()
     print("Test 02 : decorator 'log_to_file'")
 
     @log_to_file
-    def add( a: int, b: int ) -> int:
-        ''' Add a and b '''
+    def add(a: int, b: int) -> int:
+        """Add a and b"""
         return a + b
 
     print(add)
     print(add.__doc__)
-    add( 7, 13 )
-    logfile = Path('add.log')
-    assert logfile.is_file()
+    add(7, 13)
+    logfile = Path("add.log")
+    assertTrue(logfile.is_file(), "logfile must exist: '{}'", logfile)
 
     # Test 03
     vspace()
     print("Test 03 : decorator 'cacheFS'")
 
-    # @cacheFS( Path('slow_mult') )
+    # @cacheFS(Path('slow_mult'))
     @cacheFS
-    def slow_mult( a: int, b: int ) -> int:
-        ''' Multiply a and b '''
+    def slow_mult(a: int, b: int) -> int:
+        """Multiply a and b"""
         time.sleep(1)
         return a * b
 
     print(slow_mult)
     print(slow_mult.__doc__)
 
-    @timer 
+    @timer
     def test03():
-        ''' tests timer decorator '''
+        """tests timer decorator"""
         for i in range(4):
-            res = slow_mult( 111, 10*i )
+            res = slow_mult(111, 10 * i)
             print(f"111 * {i} = {res}")
 
-    test03() # runs in 2ms-4s depending on cache hits/misses
+    test03()  # runs in 2ms-4s depending on cache hits/misses
```

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.6.dev1/src/DRSlib/execute.py` & `DRSlib-DavidRodriguezSoaresCUI-0.7.0/src/DRSlib/execute.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,40 @@
 # pylint: disable=broad-except
 
-# module-level docstring
-__doc__='''
+
+"""
 Shell command execution
 =======================
 
 Sometimes we just want to execute a shell command and possibly
 retrieve stdout/stderr, without hassle.
-'''
+"""
+
+from os import PathLike
+from typing import Dict, Sequence, Union
+from subprocess import Popen, PIPE  # nosec
+
+
+COMMAND_TYPE = Union[
+    Union[str, bytes, PathLike[str], PathLike[bytes]],
+    Sequence[Union[str, bytes, PathLike[str], PathLike[bytes]]],
+]
 
-from typing import Iterable, Dict, Union
-from subprocess import Popen, PIPE
 
-def execute( command: Union[str,Iterable[str]], shell: bool = True ) -> Dict[str,str]:
-    ''' Passes command to subprocess.Popen, retrieves stdout/stderr and performs
+def execute(command: COMMAND_TYPE, shell: bool = False) -> Dict[str, str]:
+    """Passes command to subprocess.Popen, retrieves stdout/stderr and performs
     error management.
     Returns a dictionnary containing stdX.
-    Upon command failure, prints exception and returns empty dict. '''
+    Upon command failure, prints exception and returns empty dict."""
 
     try:
-        with Popen( command, stdout=PIPE, stderr=PIPE, shell=shell ) as process:
+        with Popen(command, stdout=PIPE, stderr=PIPE, shell=shell) as process:  # nosec
             # wait and retrieve stdout/err
             _stdout, _stderr = process.communicate()
             # handle text encoding issues and return stdX
             return {
-                'stdout': _stdout.decode('utf8', errors='backslashreplace'),
-                'stderr': _stderr.decode('utf8', errors='backslashreplace')
+                "stdout": _stdout.decode("utf8", errors="backslashreplace"),
+                "stderr": _stderr.decode("utf8", errors="backslashreplace"),
             }
     except Exception as e:
-        print(f"execute: Error while executing command '{command}' : {e}")
+        print(f"execute: Error while executing command '{command}' : {e}")  # type: ignore[str-bytes-safe]
         raise
```

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.6.dev1/src/DRSlib/fsdb.py` & `DRSlib-DavidRodriguezSoaresCUI-0.7.0/src/DRSlib/fsdb.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,287 +1,330 @@
-# pylint: disable=broad-except, eval-used
+# pylint: disable=broad-except, unnecessary-lambda-assignment
 
-# module-level docstring
-__doc__='''
+
+"""
 FileSystemDataBase
 ==================
 
 A collection of tools for having a cached representation of
 a file system.
-'''
+"""
 
-from pathlib import Path
-import re
+import ast
 import json
-from typing import Callable, Union, List, Dict, Iterable
 import logging
+import re
+from pathlib import Path
+from typing import Any, Callable, Dict, Iterable, List, Optional, Union
+
 from .decorators import timer
-from .path_tools import ensure_dir_exists, make_FS_safe, folder_get_file_count
+from .path_tools import ensure_dir_exists, folder_get_file_count, make_FS_safe
 from .str_utils import truncate_str
-from .utils import pickle_this, unpickle_this
-log = logging.getLogger( __file__ )
+from .utils import assertTrue, pickle_this, unpickle_this
 
+LOG = logging.getLogger(__file__)
 
-def FSindex( root: Path, condition: Callable = lambda x: True ) -> Dict[str,dict]:
-    ''' Returns a dictionnary such as
+
+def FSindex(root: Path, condition: Callable = lambda x: True) -> Dict[str, dict]:
+    """Returns a dictionnary such as
     - Contains <root_path:str> as only key
     - Recursively represents contained files and subdirectories, with each their subdirectories, etc
-    '''
-    assert root.is_dir()
+    """
+    assertTrue(root.is_dir(), "Root dir must exist: '{}'", root)
     _root = root.resolve()
 
-    def recursive_collection( _dir: Path ):
-        def try_recursion( location: Path ):
+    def recursive_collection(_dir: Path):
+        def try_recursion(location: Path):
             try:
-                return recursive_collection( location ) if location.is_dir() else None
+                return recursive_collection(location) if location.is_dir() else None
             except Exception as e:
-                print(f"FSindex: something went wrong at '{root}'. Error:\n{e}")
+                print(f"FSindex: something went wrong at '{_root}'. Error:\n{e}")
                 return None
 
         return {
-            str(child.name): try_recursion( child )
+            str(child.name): try_recursion(child)
             for child in _dir.iterdir()
-            if condition( child )
+            if condition(child)
         }
 
-    root_s = root.as_posix()
-    if root_s[-1] == '/':
+    root_s = _root.as_posix()
+    if root_s[-1] == "/":
         root_s = root_s[:-1]
 
-    return {
-        root_s: recursive_collection( root )
-    }
+    return {root_s: recursive_collection(root)}
 
 
 class CachedFS:
-    ''' Caching a filesystem tree can be useful for applications
+    """Caching a filesystem tree can be useful for applications
     with frequent file system lookups.
-    
+
     Features :
      - Possiblity to backup to/load from JSON file
      - cache directories, files, or both
-    '''
-
-    def __init__( self, root: Path, directories: bool = True, files: bool = True, backup_fs: dict = None ) -> None:
+    """
 
+    def __init__(
+        self,
+        root: Path,
+        directories: bool = True,
+        files: bool = True,
+        backup_fs: Optional[dict] = None,
+    ) -> None:
         if backup_fs:
-            self.root = Path( backup_fs['root'] )
-            assert root.samefile(self.root), f"ERROR: given root path '{root}' is different from backup root path '{self.root}' !"
-            assert self.root.is_dir(), f"It seems root='{self.root}' is no longer a valid directory !"
-            self.filter_text = backup_fs['filter']
-            self.filter = eval( backup_fs['filter'] )
-            self.fs = backup_fs['fs']
+            self.root = Path(backup_fs["root"])
+            assertTrue(
+                root.samefile(self.root),
+                "ERROR: given root path '{}' is different from backup root path '{}' !",
+                root,
+                self.root,
+            )
+            assertTrue(
+                self.root.is_dir(),
+                "It seems root='{}' is no longer a valid directory !",
+                self.root,
+            )
+            self.filter_text = backup_fs["filter"]
+            self.filter = ast.literal_eval(backup_fs["filter"])
+            self.fs = backup_fs["fs"]
 
         else:
-            assert files or directories, "CachedFS cannot be instantiated with directories=files=False."
-            assert root.is_dir(), f"root='{root}' is not a valid directory"
+            assertTrue(
+                files or directories,
+                "CachedFS cannot be instantiated with directories=files=False.",
+            )
+            assertTrue(root.is_dir(), "root='{}' is not a valid directory", root)
             self.root = root.resolve()
-            condition = ' or '.join( [
-                x
-                for x in [
-                    'x.is_dir()' if directories else None,
-                    'x.is_file()' if files else None
+            condition = " or ".join(
+                [
+                    x
+                    for x in [
+                        "x.is_dir()" if directories else None,
+                        "x.is_file()" if files else None,
+                    ]
+                    if x is not None
                 ]
-                if x is not None 
-            ] )
-            self.filter_text = f'lambda x: {condition}'
-            self.filter = eval( self.filter_text )
+            )
+            self.filter_text = f"lambda x: {condition}"
+            self.filter = ast.literal_eval(self.filter_text)
             self.update()
-        
-        
-    @timer
-    def update( self ) -> None:
-        ''' Updates internal DB '''
-        self.fs = FSindex( self.root, self.filter )
-
 
-    def __contains__( self, pattern: str ) -> bool:
-        ''' Implements `<pattern:str> in <_:CachedFS>` operation
-        '''
-        _pattern = re.compile(pattern, flags=re.IGNORECASE )
-
-        return 0 < len( self.search( 
-            search_for=_pattern,
-            stop_at_first=True
-        ) )
+    @timer
+    def update(self) -> None:
+        """Updates internal DB"""
+        self.fs = FSindex(self.root, self.filter)
+
+    def __contains__(self, pattern: str) -> bool:
+        """Implements `<pattern:str> in <_:CachedFS>` operation"""
+        _pattern = re.compile(pattern, flags=re.IGNORECASE)
 
+        return 0 < len(self.search(search_for=_pattern, stop_at_first=True))
 
     @timer
-    def search( self, search_for: Union[str,re.Pattern,Callable], stop_at_first: bool = False ) -> List[str]:
-        ''' Performs a search on internal FileSystem representation.
+    def search(
+        self, search_for: Union[str, re.Pattern, Callable], stop_at_first: bool = False
+    ) -> List[str]:
+        """Performs a search on internal FileSystem representation.
 
         `search_for`: Match criterion. Can be a string (matches file/directory name; case insensitive),
         a re.Pattern (matches with re.Pattern.match()) or a callable (must return boolean values; match
         on True).
 
         `stop_at_first`: returns at most one matching item.
-        '''
+        """
 
         if callable(search_for):
             _search_for = search_for
         if isinstance(search_for, re.Pattern):
-            _search_for = lambda x: bool(search_for.match(x))
+            _search_for = lambda x: bool(search_for.match(x))  # type: ignore[union-attr]
         if isinstance(search_for, str):
             search_for_lower = search_for.lower()
-            _search_for = lambda x: search_for_lower in x.lower()
+            _search_for = lambda x: search_for_lower in x.lower()  # type: ignore[union-attr]
 
-        combine_paths = lambda x,y: f"{x}/{y}" if x else y
+        def combine_paths(x: Optional[str], y: str) -> str:
+            return f"{x}/{y}" if x else y
 
-        def search_recursive( FSDB: dict, path_prefix: str = '' ):
-            matches = list()
-            #print(f"search_recursive: from '{path_prefix}'")
+        def search_recursive(FSDB: dict, path_prefix: str = ""):
+            matches = []
+            # print(f"search_recursive: from '{path_prefix}'")
             try:
                 for item, children in FSDB.items():
-                    if _search_for( item ):
-                        #print(f"Positive: '{item}'")
-                        matches.append( combine_paths( path_prefix, item ) )
+                    if _search_for(item):
+                        # print(f"Positive: '{item}'")
+                        matches.append(combine_paths(path_prefix, item))
                         if stop_at_first:
                             return matches
                     if children:
-                        matches.extend( 
-                            search_recursive( children, combine_paths( path_prefix, item ) )
+                        matches.extend(
+                            search_recursive(children, combine_paths(path_prefix, item))
                         )
                     if stop_at_first and matches:
                         return matches
             except Exception as e:
-                print(f"search_recursive: something went wrong at '{path_prefix}'. Error:\n{e}")
+                print(
+                    f"search_recursive: something went wrong at '{path_prefix}'. Error:\n{e}"
+                )
                 raise
-            
-            return matches
-        
-        return search_recursive( self.fs )
-
 
-    def as_json( self ) -> str:
-        ''' Dumps CachedFS as json-formatted string '''
-        data = {
-            'root': str(self.root),
-            'fs': self.fs,
-            'filter': self.filter_text
-        }
-        return json.dumps( data, indent=2 )
+            return matches
 
-    
-    def backup_to_file( self, backup_file: Path ) -> None:
-        ''' Dumps CachedFS to json-formatted file '''
-        assert backup_file.suffix.lower() == '.json'
-        backup_file.write_text( self.as_json(), encoding='utf8' )
+        return search_recursive(self.fs)
 
+    def as_json(self) -> str:
+        """Dumps CachedFS as json-formatted string"""
+        data = {"root": str(self.root), "fs": self.fs, "filter": self.filter_text}
+        return json.dumps(data, indent=2)
+
+    def backup_to_file(self, backup_file: Path) -> None:
+        """Dumps CachedFS to json-formatted file"""
+        assertTrue(
+            backup_file.suffix.lower() == ".json",
+            "Unexpected suffix '{}'",
+            backup_file.suffix.lower(),
+        )
+        backup_file.write_text(self.as_json(), encoding="utf8")
 
     @classmethod
-    def from_file( cls, backup_file: Path, root: Path ):
-        ''' Loads CachedFS from json-formatted string produced by CachedFS.backup_to_file() function.
+    def from_file(cls, backup_file: Path, root: Path):
+        """Loads CachedFS from json-formatted string produced by CachedFS.backup_to_file() function.
         Note: `root` is required to verify the intended root matches root in cache file.
-        '''
-        assert backup_file.suffix.lower() == '.json'
-        backup = json.loads( backup_file.read_text( encoding='utf8' ) )
-        return CachedFS( root=root, backup_fs=backup )
-    
+        """
+        assertTrue(
+            backup_file.suffix.lower() == ".json",
+            "Unexpected suffix '{}'",
+            backup_file.suffix.lower(),
+        )
+        backup = json.loads(backup_file.read_text(encoding="utf8"))
+        return CachedFS(root=root, backup_fs=backup)
+
 
-def get_snapshot_file( snapshot_folder: Path, snapshot_filename: str ) -> Path:
-    ''' Returns a snapshot file path, given snapshot folder path and a filename 
+def get_snapshot_file(snapshot_folder: Path, snapshot_filename: str) -> Path:
+    """Returns a snapshot file path, given snapshot folder path and a filename
     (which passes through a sanitization process).
-    '''
-    
-    ensure_dir_exists( snapshot_folder )
-    FS_safe_snapshot_filename = make_FS_safe( snapshot_filename + '.snapshot' )
+    """
+
+    ensure_dir_exists(snapshot_folder)
+    FS_safe_snapshot_filename = make_FS_safe(snapshot_filename + ".snapshot")
     snapshot_file = snapshot_folder / FS_safe_snapshot_filename
 
     # Multiple reasons may lead to OSErrors for a given path
     try:
         snapshot_file.is_file()
     except OSError as e:
-        try: # Correction: trucnating file name to 240 characters
-            snapshot_file = snapshot_folder / truncate_str( 
-                FS_safe_snapshot_filename, 
-                output_length=240
+        try:  # Correction: trucnating file name to 240 characters
+            snapshot_file = snapshot_folder / truncate_str(
+                FS_safe_snapshot_filename, output_length=240
             )
             snapshot_file.is_file()
         except OSError:
-            raise OSError("get_snapshot_file: Snapshot file inaccessible for unforeseen reasons (FIXME!).") from e
+            raise OSError(
+                "get_snapshot_file: Snapshot file inaccessible for unforeseen reasons (FIXME!)."
+            ) from e
 
     return snapshot_file
 
 
-def get_folder_snapshot_h( _root: Path, extentions: Iterable[str], snapshot_folder: Path, recursive: bool = True, simplified: bool = False, rec: bool = False ) -> dict:
-    ''' Recursive helper function to `get_folder_snapshot`.
+def get_folder_snapshot_h(
+    _root: Path,
+    extentions: Iterable[str],
+    snapshot_folder: Path,
+    recursive: bool = True,
+    simplified: bool = False,
+    rec: bool = False,
+) -> dict:
+    """Recursive helper function to `get_folder_snapshot`.
     For more information see its docstring.
-    '''
+    """
 
     # '*.txt' -> 'txt' extension conversion
-    extentions = [ e.replace('*.','.') for e in extentions ]
+    extentions = [e.replace("*.", ".") for e in extentions]
 
     # Check for cached results
-    cache_file_name = str(_root) + ('.S' if simplified else '.C')
-    cache_file = get_snapshot_file( snapshot_folder, cache_file_name )
+    cache_file_name = str(_root) + (".S" if simplified else ".C")
+    cache_file = get_snapshot_file(snapshot_folder, cache_file_name)
     try:
-        res = unpickle_this( cache_file )
+        res = unpickle_this(cache_file)
     except Exception:
         res = None
     if res:
         if simplified:
-            log.info( "get_folder_snapshot: loaded from cache" )
+            LOG.info("get_folder_snapshot: loaded from cache")
             return res
         # Check for discrepancy in file number, as indicator something changed and snapshot should be rebuilt
-        nbfiles1, nbfiles2 = res['__nbfiles__'], folder_get_file_count( _root )
-        if nbfiles1==nbfiles2:
-            log.info( "get_folder_snapshot: loaded from cache" )
+        nbfiles1, nbfiles2 = res["__nbfiles__"], folder_get_file_count(_root)
+        if nbfiles1 == nbfiles2:
+            LOG.info("get_folder_snapshot: loaded from cache")
             return res
-        log.debug("get_folder_snapshot: number of files changes (%s != %s) -> updating snapshot", nbfiles1, nbfiles2)
+        LOG.debug(
+            "get_folder_snapshot: number of files changes (%s != %s) -> updating snapshot",
+            nbfiles1,
+            nbfiles2,
+        )
 
     # Build from scratch
-    log.info("get_folder_snapshot: from '%s' ..", _root)
-    content = dict()
+    LOG.info("get_folder_snapshot: from '%s' ..", _root)
+    content: Dict[str, Any] = {}
 
-    if simplified: # "simplified" version
+    if simplified:  # "simplified" version
         for item in _root.iterdir():
             if item.is_file():
                 (name, ext) = (item.stem, item.suffix)
                 if ext not in extentions:
                     continue
                 content[name] = item.resolve()
             elif item.is_dir():
                 if not recursive:
                     continue
-                content_rec = get_folder_snapshot_h( item, extentions, snapshot_folder, recursive, simplified, rec=True )
-                content.update( content_rec )
+                content_rec = get_folder_snapshot_h(
+                    item, extentions, snapshot_folder, recursive, simplified, rec=True
+                )
+                content.update(content_rec)
             else:
-                raise ValueError("get_folder_snapshot::Not file or folder : {}".format(item))
-                
-    else: # "complex" version
+                raise ValueError(f"get_folder_snapshot::Not file or folder : {item}")
+
+    else:  # "complex" version
         file_count = 0
         for item in _root.iterdir():
             if item.is_file():
                 (name, ext) = (item.stem, item.suffix)
                 if ext not in extentions:
                     continue
                 content[name] = item.resolve()
                 file_count += 1
             elif item.is_dir():
                 if not recursive:
                     continue
-                content_rec = get_folder_snapshot_h( item, extentions, snapshot_folder, recursive, simplified, rec=True )
+                content_rec = get_folder_snapshot_h(
+                    item, extentions, snapshot_folder, recursive, simplified, rec=True
+                )
                 content[item.name] = content_rec
-                file_count += content_rec['__nbfiles__']
+                file_count += content_rec["__nbfiles__"]
             else:
-                raise ValueError("get_folder_snapshot::Not file or folder : {}".format(item))
+                raise ValueError(f"get_folder_snapshot::Not file or folder : {item}")
 
         # Add file count
-        content['__nbfiles__'] = file_count
-        log.debug("get_folder_snapshot: from '%s' : found %s files !", _root, file_count)
+        content["__nbfiles__"] = file_count
+        LOG.debug(
+            "get_folder_snapshot: from '%s' : found %s files !", _root, file_count
+        )
 
     # Caching for later use
     if not (simplified and rec):
-        pickle_this( content, cache_file )
+        pickle_this(content, cache_file)
 
     return content
 
 
-def get_folder_snapshot( _root: Path, extentions: Iterable[str], snapshot_folder: Path, recursive: bool = True, simplified: bool = False ) -> dict:
-    ''' Recursively builds a dictionnary representation of a directory tree. Only listed file extensions are considered.
+def get_folder_snapshot(
+    _root: Path,
+    extentions: Iterable[str],
+    snapshot_folder: Path,
+    recursive: bool = True,
+    simplified: bool = False,
+) -> dict:
+    """Recursively builds a dictionnary representation of a directory tree. Only listed file extensions are considered.
 
     `extensions` : iterable of ``'*.ext'`` or ``'.ext'``
 
     Rules ("complex") :
      - The returned dictionnary has one entry : 'root'
      - An entry E can have one of three values according to  :
        > E is a directory : its value is a dictionnary with name of contained items as keys
@@ -333,10 +376,12 @@
         {
             'file3': '<root>/file3.log',
             'file4': '<root>/A/file4.jpg',
             'file5': '<root>/A/file5.git',
             'file7': '<root>/A/file7.txt',
             'file8': '<root>/A/T/file8.png'
         }
-    '''
-    ensure_dir_exists( snapshot_folder )
-    return get_folder_snapshot_h( _root, extentions, snapshot_folder, recursive, simplified )
+    """
+    ensure_dir_exists(snapshot_folder)
+    return get_folder_snapshot_h(
+        _root, extentions, snapshot_folder, recursive, simplified
+    )
```

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.6.dev1/src/DRSlib/hash.py` & `DRSlib-DavidRodriguezSoaresCUI-0.7.0/src/DRSlib/hash.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,138 +1,142 @@
-﻿# module-level docstring
-__doc__='''
+﻿"""
 Hash-related tools
 ==================
 
 Useful tools for easily hashing files.
-'''
+"""
 
 import hashlib
-from pathlib import Path
 import logging
-from typing import Union, Optional, Dict, Iterable
+from pathlib import Path
+from typing import Dict, Optional
 
-from .utils import pickle_this, unpickle_this
-from .spinner import MySpinner
 from .os_detect import Os
 from .path_tools import ensure_dir_exists, file_collector
+from .spinner import MySpinner
+from .utils import assertTrue, pickle_this, unpickle_this
 
-BLOCKSIZE = 65_536 # 2 ** 16
-log = logging.getLogger( __file__ )
+BLOCKSIZE = 65_536  # 2 ** 16
+log = logging.getLogger(__file__)
 spinner = MySpinner()
 current_os = Os()
 
-def file_hash( file: Path ) -> str:
-    ''' Returns the md5 hash of the corresponding file
+
+def file_hash(file: Path) -> str:
+    """Returns the md5 hash of the corresponding file
     Reads the file in 2^16 bytes (~65Ko) chunks
-    '''
+    """
 
-    hasher = hashlib.md5()
-    with file.open(mode='rb') as f:
+    hasher = hashlib.md5()  # nosec B324
+    with file.open(mode="rb") as f:
         chunk = f.read(BLOCKSIZE)
         while 0 < len(chunk):
             hasher.update(chunk)
             chunk = f.read(BLOCKSIZE)
 
     hash_s = hasher.hexdigest()
 
-    log.debug( "File %s has md5 hash %s.", file, hash_s )
+    log.debug("File %s has md5 hash %s.", file, hash_s)
     return hash_s
 
 
-def partial_MD5( file: Path ) -> str:
-    ''' Reads up to 10MB of the given file and returns MD5 (partial) checksum. Borrowing code from : https://stackoverflow.com/a/1131238
+def partial_MD5(file: Path) -> str:
+    """Reads up to 10MB of the given file and returns MD5 (partial) checksum. Borrowing code from : https://stackoverflow.com/a/1131238
     This is achieved by reading 10 times ~1MB, thus reducing RAM usage.
-    '''
-    hasher = hashlib.md5()
-    with file.open(mode='rb') as f:
+    """
+    hasher = hashlib.md5()  # nosec B324
+    with file.open(mode="rb") as f:
         for _ in range(10):
             chunk = f.read(1_048_576)
             if not chunk:
                 break
             hasher.update(chunk)
-            
+
     return hasher.hexdigest()
 
 
-def path_to_id( _path: Path, limit_id_len: bool = True ) -> str:
-    ''' Returns a string identifier for any given file/directory path.
+def path_to_id(_path: Path, limit_id_len: bool = True) -> str:
+    """Returns a string identifier for any given file/directory path.
 
     `limit_id_len`: If True, keeps id length below 190 characters
-    '''
+    """
     path = _path.resolve()
 
     anchor_len = 3 if current_os.wsl else len(path.anchor)
 
     _id = str(path)[anchor_len:]
     if limit_id_len and 190 < len(_id):
-        _id = _id[:160] + ' [...] ' + _id[-20:]
+        _id = _id[:160] + " [...] " + _id[-20:]
 
     return _id
 
 
-def directory_hash( directory: Path, pattern: Union[str,Iterable[str]] = '*.*', old_hashes: Optional[dict] = None ) -> Dict[str,str]:
-    ''' Returns a dictionnary of md5 hash of all the files in the directory
+def directory_hash(
+    directory: Path,
+    pattern: str = "*.*",
+    old_hashes: Optional[dict] = None,
+) -> Dict[str, str]:
+    """Returns a dictionnary of md5 hash of all the files in the directory
     corresponding to path 'directory'.
-    
-    Returns: Dict[ <file_name:str>, <file_hash:str> ]
-    '''
-
-    files = file_collector(
-        root = directory,
-        pattern=pattern
-    )
 
-    hashes = dict()
+    Returns: Dict[<file_name:str>, <file_hash:str>]
+    """
+
+    files = file_collector(root=directory, pattern=pattern)
+    if old_hashes is None:
+        old_hashes = {}
+
+    hashes = {}
     for file in files:
         key = file.name
         if key in old_hashes:
-            log.debug('Cache hit')
+            log.debug("Cache hit")
             hashes[key] = old_hashes[key]
             continue
-            
-        hashes[key] = file_hash( file )        
+
+        hashes[key] = file_hash(file)
 
     return hashes
 
 
-def tree_hash( root: Path, hash_location: Path, pattern: Union[str,Iterable[str]] = '*.*', fastload: bool = False ) -> None:
-    ''' Explores the directory structure recursively from 'root', computing their hash.
+def tree_hash(
+    root: Path,
+    hash_location: Path,
+    pattern: str = "*.*",
+    fastload: bool = False,
+) -> None:
+    """Explores the directory structure recursively from 'root', computing their hash.
     For each directory explored, saves hashes found to a file.
 
     `fastload`: If True and the corresponding hash file is found, hashes are not re-checked. This
     is used for performance reasons. Do not use if changes are likely.
 
-    '''
+    """
 
     root = root.resolve()
     hash_location = hash_location.resolve()
-    assert root.is_dir()
-    ensure_dir_exists( hash_location )
+    assertTrue(root.is_dir(), "Root dir must exist: '{}'", root)
+    ensure_dir_exists(hash_location)
 
-    subdirectories = [x for x in root.iterdir() if x.is_dir() and x!=hash_location]
+    subdirectories = [x for x in root.iterdir() if x.is_dir() and x != hash_location]
     for sub_dir in subdirectories:
-        savefile = hash_location / path_to_id( sub_dir )
+        savefile = hash_location / path_to_id(sub_dir)
 
         if not (fastload and savefile.is_file()):
-            old_hashes = unpickle_this( savefile )
+            old_hashes = unpickle_this(savefile)
             spinner.animation()
-            hashes = directory_hash( 
-                directory=sub_dir,
-                pattern=pattern,
-                old_hashes=old_hashes
+            hashes = directory_hash(
+                directory=sub_dir, pattern=pattern, old_hashes=old_hashes
             )
-            data = dict()
-            data['folder'] = sub_dir
-            data['hashes'] = hashes
-            
+            data = {"folder": sub_dir, "hashes": hashes}
+
             pickle_this(data, savefile)
         else:
-            spinner.animation(text='cache hit')
-        
+            spinner.animation(text="cache hit")
+
         # Recursion
         tree_hash(
             root=sub_dir,
             hash_location=hash_location,
             pattern=pattern,
-            fastload=fastload
+            fastload=fastload,
         )
```

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.6.dev1/src/DRSlib/interval.py` & `DRSlib-DavidRodriguezSoaresCUI-0.7.0/src/DRSlib/interval.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,73 +1,96 @@
-# module-level docstring
-__doc__='''
+"""
 Interval representation implementation
 ======================================
 
 A simple implementation for generic intervals.
-'''
+"""
+from typing import Optional, Tuple, Union
 
+from .utils import assertTrue
 
-from typing import NewType, Union, Optional, Tuple
+Numerical = Union[float, int]
+
+
+class InvalidInterval(Exception):
+    """Trivial exception for invalid interval"""
 
-Numerical = NewType( 'Numerical', Union[float,int] )
 
 class Interval:
-    ''' Represents an interval [a,b] of real (numerical) values
+    """Represents an interval [a,b] of real (numerical) values
     Note : the interval [a,b] must be strictly positive (a<b)
-    '''
+    """
 
-    class InvalidInterval(Exception):
-        ''' Trivial exception for invalid interval '''
-        
     # Needed for visibility
-    InvalidInterval=InvalidInterval
+    # InvalidInterval = InvalidInterval
 
-    def __init__( self, a: Numerical, b: Numerical, boundary: Optional['Interval'] = None ) -> None:
-        assert a<b, f"Interval.__init__: invalid arguments : a={a}, b={b} do not respect rule a<b"
-        self.a = a
-        self.b = b
+    def __init__(
+        self, left: Numerical, right: Numerical, boundary: Optional["Interval"] = None
+    ) -> None:
+        assertTrue(
+            left < right,
+            "left={}, right={} do not respect rule: left < right",
+            left,
+            right,
+        )
+        self.left = left
+        self.right = right
         if isinstance(boundary, Interval):
-            self.a, self.b = self.intersection( boundary )      
+            res = self.intersection(boundary)
+            if res is not None:
+                self.left, self.right = res
 
     @property
     def len(self) -> Numerical:
-        ''' Property. Represents the length of the interval '''
-        return self.b - self.a
+        """Property. Represents the length of the interval"""
+        return self.right - self.left
+
+    def __str__(self):
+        return f"<Interval {self.left:.2f}-{self.right:.2f} [{self.len:.2f}]>"
 
-    def __str__( self ):
-        return f"<Interval {self.a:.2f}-{self.b:.2f} [{self.len:.2f}]>"
+    def __iter__(self):
+        return iter([self.left, self.right])
 
-    def intersection( self, other: 'Interval', return_obj: bool = False, raise_exception: bool = True ) -> Union['Interval',Tuple[Numerical,Numerical], None]:
-        ''' Computes the intersection between two Interval objects.
+    def intersection(
+        self, other: "Interval", return_obj: bool = False, raise_exception: bool = True
+    ) -> Union["Interval", Tuple[Numerical, Numerical], None]:
+        """Computes the intersection between two Interval objects.
         Let [x,y] be the valid strictly interval representing the intersection (only exists on
         strictly overlapping intervals).
-        
+
         Returns : either an Interval object representing the [x,y] interval (if `return_obj`),
-        or the (x,y) tuple (if not `return_obj`), or nothing if [x,y] doesn't exist 
+        or the (x,y) tuple (if not `return_obj`), or nothing if [x,y] doesn't exist
         (see `raise_exception` below).
-        
+
         `raise_exception` : allows to disable raising exception, returning None instead.
-        '''
-        assert isinstance( other, Interval )
-        a = self.a if other.a < self.a else other.a
-        b = self.b if self.b < other.b else other.b
-        if b <= a and raise_exception:
-            # non-strictly overlapping intervals 
-            raise self.InvalidInterval()
-        else:
-            # valid intersection exists 
-            return Interval(a,b) if return_obj else (a, b)
+        """
+        assertTrue(
+            isinstance(other, Interval), "Expected Interval, found {}", type(other)
+        )
+        left = self.left if other.left < self.left else other.left
+        right = self.right if self.right < other.right else other.right
+        if right <= left and raise_exception:
+            # non-strictly overlapping intervals
+            raise InvalidInterval()
+        # valid intersection exists
+        return Interval(left, right) if return_obj else (left, right)
 
     @classmethod
-    def from_length( cls, length: Numerical, start: Optional[Numerical] = None, end: Optional[Numerical] = None ) -> 'Interval':
-        ''' Creates an Interval from 2 (or more) of an interval's properties : start point, end point, length '''
-        assert 0 < length
-        if start:
-            if end:
-                assert abs((end - start) - length) < (end - start) * 0.01, "Interval.from_length: argument mismatch"
+    def from_length(
+        cls,
+        length: Numerical,
+        start: Optional[Numerical] = None,
+        end: Optional[Numerical] = None,
+    ) -> "Interval":
+        """Creates an Interval from 2 (or more) of an interval's properties : start point, end point, length"""
+        assertTrue(0 < length, "Interval must have non-zero lenth")
+        if start is not None:
+            if end is not None:
+                assertTrue(
+                    abs((end - start) - length) < (end - start) * 0.01,
+                    "argument mismatch",
+                )
             else:
                 end = start + length
-        elif end:
+        elif end is not None:
             start = end - length
-        return Interval( start, end )
-        
+        return Interval(start, end)  # type: ignore[arg-type]
```

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.6.dev1/src/DRSlib/mediainfo.py` & `DRSlib-DavidRodriguezSoaresCUI-0.7.0/src/DRSlib/mediainfo.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,424 +1,421 @@
-# module-level docstring
-__doc__='''
+"""
 MediaInfo interface
 ===================
 
 An interface to software `MediaInfo <https://mediaarea.net/fr/MediaInfo>`_
 
 Note: For it to work, MediaInfo needs to be installed on the system AND be
 callable from a terminal.
-'''
-
+"""
 import logging
 import re
 from pathlib import Path
 from typing import List, Dict, Union, Iterable
 
-from .utils import type_assert
+from .utils import type_assert, flatten_list
 from .execute import execute
 
-MEDIAINFO_POSSIBLE_RETURN_VALUES = Union[int,float,str,type(None)]
+
+MEDIAINFO_POSSIBLE_RETURN_VALUES = Union[int, float, str, None]
+
 
 class Datapoint:
-    ''' In this context, a Datapoint represents a multimedia parameter
+    """In this context, a Datapoint represents a multimedia parameter
     in a format compatible with MediaInfo's cli interface.
-    
+
     Advantages:
 
     - systematic solution
-    
+
     - integrates cli<->shorthand format conversion
-    
+
     - ability to combine commands
-    
+
     - shifts complexity from MediaInfo's class
-    '''
+    """
 
-    SEPARATOR = '\\n'
+    SEPARATOR = "\\n"
 
-    def __init__( self, category: str, parameter: Union[str,List[str]] ):
+    def __init__(self, category: str, parameter: Union[str, List[str]]):
         self.category = category
         self.parameter = parameter
 
     def __str__(self):
-        parameter_s = Datapoint.SEPARATOR.join( self.parameter ) \
-            if isinstance( self.parameter, list ) \
+        parameter_s = (
+            Datapoint.SEPARATOR.join(self.parameter)
+            if isinstance(self.parameter, list)
             else self.parameter
+        )
         return f"--Inform={self.category};" + parameter_s
 
     def __repr__(self):
         return f"< Datapoint : '{str(self)}' >"
 
-    def __parameter_shorthand(self, p: str ):
-        ''' Tries to convert parameter to its equivalent shorthand.
+    def __parameter_shorthand(self, p: str):
+        """Tries to convert parameter to its equivalent shorthand.
         Helper function for `parameter_shorthand`
-        '''        
-        for k,v in MediaInfo.DATAPOINTS.items():
+        """
+        for k, v in MediaInfo.DATAPOINTS.items():
             dp = Datapoint.from_string(v)
-            if dp.parameter==p:
+            if dp.parameter == p:
                 return k
-        return p 
+        return p
 
     @property
     def parameter_shorthand(self):
-        ''' Tries to convert parameter to its equivalent shorthand '''
-        return self.__parameter_shorthand( self.parameter ) \
-            if isinstance( self.parameter, str ) \
-            else [
-                self.__parameter_shorthand( p )
-                for p in self.parameter
-            ]
-
+        """Tries to convert parameter to its equivalent shorthand"""
+        return (
+            self.__parameter_shorthand(self.parameter)
+            if isinstance(self.parameter, str)
+            else [self.__parameter_shorthand(p) for p in self.parameter]
+        )
 
     @classmethod
-    def from_string( cls, datapoint: str ) -> 'Datapoint':
-        ''' Converts datapoint from '--Inform=<category>;%parameter%'-formatted
+    def from_string(cls, datapoint: str) -> "Datapoint":
+        """Converts datapoint from '--Inform=<category>;%parameter%'-formatted
         string to Datapoint instance
-        '''
-        datapoint = MediaInfo.DATAPOINTS.get( datapoint, datapoint ) # Handle shorthands
+        """
+        datapoint = MediaInfo.DATAPOINTS.get(datapoint, datapoint)  # Handle shorthands
         try:
-            res = re.match( r"^\-\-Inform=(.+?);(.+)$", datapoint ).groups(0)
-            assert len(res)==2
-            return Datapoint( *res )
-        except AttributeError as e:
-            raise ValueError(f"Datapoint.from_string : could not find category from datapoint string '{datapoint}'") from e
-
+            match = re.match(r"^\-\-Inform=(.+?);(.+)$", datapoint)
+            if not match:
+                raise ValueError("String does not match regex")
+            res = match.groups()
+            return Datapoint(res[0], res[1])
+        except (AttributeError, ValueError) as e:
+            raise ValueError(
+                f"Datapoint.from_string : could not find category from datapoint string '{datapoint}'"
+            ) from e
 
     @classmethod
-    def from_strings( cls, datapoints: Iterable[str] ) -> List['Datapoint']:
-        ''' Converts datapoint from '--Inform=<category>;%parameter%'-formatted
+    def from_strings(cls, datapoints: Iterable[str]) -> List["Datapoint"]:
+        """Converts datapoint from '--Inform=<category>;%parameter%'-formatted
         string to Datapoint instance
-        '''
-        return [
-            Datapoint.from_string(dp)
-            for dp in datapoints
-        ]
-
+        """
+        return [Datapoint.from_string(dp) for dp in datapoints]
 
     @classmethod
-    def group_by_category( cls, datapoints: Iterable['Datapoint'] ) -> Dict[str,List['Datapoint']]:
-        ''' Group datapoints by category
-        '''
+    def group_by_category(
+        cls, datapoints: Iterable["Datapoint"]
+    ) -> Dict[str, List["Datapoint"]]:
+        """Group datapoints by category"""
         return {
-            cat: [ 
-                d
-                for d in datapoints
-                if d.category == cat
-            ]
-            for cat in { d.category for d in datapoints }
+            cat: [d for d in datapoints if d.category == cat]
+            for cat in {d.category for d in datapoints}
         }
 
-
-    @classmethod 
-    def combine( cls, datapoints: Iterable['Datapoint'] ) -> List['Datapoint']:
-        ''' From an arbitrary amount of datapoints, combines them into
+    @classmethod
+    def combine(cls, datapoints: Iterable["Datapoint"]) -> List["Datapoint"]:
+        """From an arbitrary amount of datapoints, combines them into
         Datapoints (one per category).
-        '''
+        """
         categorized_datapoints = Datapoint.group_by_category(datapoints)
-        
+
         return [
-            Datapoint( 
-                category=cat, 
-                parameter=[
-                    cat_dp.parameter
-                    for cat_dp in cat_datapoints
-                ]
+            Datapoint(
+                category=cat,
+                parameter=flatten_list([cat_dp.parameter for cat_dp in cat_datapoints]),
             )
-            for cat,cat_datapoints in categorized_datapoints.items()
+            for cat, cat_datapoints in categorized_datapoints.items()
         ]
 
 
 class MediaInfo:
-    ''' Interface for MediaInfo, useful for retrieving info about
+    """Interface for MediaInfo, useful for retrieving info about
     video/audio/image files.
 
     example : retrieving info for file 'v.mp4'::
 
-        >>> MI = MediaInfo()                        # MediaInfo interface setup 
+        >>> MI = MediaInfo()                        # MediaInfo interface setup
         >>> f = Path('v.mp4')                       # File path
-        >>> MI.get_base_stats( f )                  # Returns dict with basic stats
-        >>> MI.get_datapoint( f, 'V_FrameCount' )   # Returns specific stat (uses shorthand)
-        >>> MI.get_datapoint( f, '--Inform=Video;%FrameCount%' )   # Equivalent to previous line
+        >>> MI.get_base_stats(f)                  # Returns dict with basic stats
+        >>> MI.get_datapoint(f, 'V_FrameCount')   # Returns specific stat (uses shorthand)
+        >>> MI.get_datapoint(f, '--Inform=Video;%FrameCount%')   # Equivalent to previous line
 
     example 2 : retrieving basic and advanced info about 'v.mp4'::
 
-        >>> MI = MediaInfo()                        # MediaInfo interface setup 
+        >>> MI = MediaInfo()                        # MediaInfo interface setup
         >>> f = Path('v.mp4')                       # File path
-        >>> stats = MI.get_base_stats( f )                  # Returns dict with basic stats
-        >>> stats = MI.get_datapoints( f, ['V_StreamSize','V_FrameCount','V_UniqueID'], existing_stats=stats ) # Returns specific stats (uses shorthand; update `stats`)
-    
-    '''
+        >>> stats = MI.get_base_stats(f)                  # Returns dict with basic stats
+        >>> stats = MI.get_datapoints(f, ['V_StreamSize','V_FrameCount','V_UniqueID'], existing_stats=stats) # Returns specific stats (uses shorthand; update `stats`)
+
+    """
 
     # collection of shorthand and their MediaInfo-understandable CLI argument counterpart
     # Naming convention : '<category_name_initial>_<parameter_name>'
     DATAPOINTS = {
-        'V_StreamSize' : '--Inform=Video;%StreamSize%',
-        'V_FrameCount' : '--Inform=Video;%FrameCount%',
-        'V_UniqueID'   : '--Inform=Video;%UniqueID%',
-        'V_Duration'   : '--Inform=Video;%Duration%',
-        'V_FrameRate'  : '--Inform=Video;%FrameRate%'
+        "V_StreamSize": "--Inform=Video;%StreamSize%",
+        "V_FrameCount": "--Inform=Video;%FrameCount%",
+        "V_UniqueID": "--Inform=Video;%UniqueID%",
+        "V_Duration": "--Inform=Video;%Duration%",
+        "V_FrameRate": "--Inform=Video;%FrameRate%",
     }
 
     UNIT_FACTOR = {
-        'Mb/s'    : 1_000_000,
-        'kb/s'    : 1000,
-        'b/s'     : 1,
-        'bits'    : 1,
-        'GiB'     : 1_000_000_000,
-        'MiB'     : 1_000_000,
-        'KiB'     : 1_000,
-        'pixels'  : 1,
-        'FPS'     : 1,
-        'ms'      : 0.001,
-        'kHz'     : 1_000,
-        'channels': 1
+        "Mb/s": 1_000_000,
+        "kb/s": 1000,
+        "b/s": 1,
+        "bits": 1,
+        "GiB": 1_000_000_000,
+        "MiB": 1_000_000,
+        "KiB": 1_000,
+        "pixels": 1,
+        "FPS": 1,
+        "ms": 0.001,
+        "kHz": 1_000,
+        "channels": 1,
     }
 
-    def __init__( self, executable: str = 'MediaInfo', logLevel: int = logging.WARNING ) -> None:
-        ''' `executable` : if typing 'MediaInfo' on a shell doesn't call mediainfo, specify using this argument a valid string that does.
-                           It can be a variant (eg. 'mediainfo.exe') or a path (eg. '~/tmp/mediainfo/mediainfo').
-        '''
-        self.log = logging.getLogger('MediaInfo')
-        self.log.setLevel( logLevel )
+    def __init__(
+        self, executable: str = "MediaInfo", logLevel: int = logging.WARNING
+    ) -> None:
+        """`executable` : if typing 'MediaInfo' on a shell doesn't call mediainfo, specify using this argument a valid string that does.
+        It can be a variant (eg. 'mediainfo.exe') or a path (eg. '~/tmp/mediainfo/mediainfo').
+        """
+        self.log = logging.getLogger("MediaInfo")
+        self.log.setLevel(logLevel)
         self.executable = executable
-        type_assert( executable, 'executable', str, 'MediaInfo: ' )
-        self.version = None 
+        type_assert(executable, "executable", str, "MediaInfo: ")
+        self.version = None
         self.get_MI_version()
 
-        self.log.debug("Successfully initialized object : %s" , str(self))
-
+        self.log.debug("Successfully initialized object : %s", str(self))
 
-    def get_MI_version( self ) -> None:
-        ''' Tries to obtain callable MediaInfo version
-        '''
+    def get_MI_version(self) -> None:
+        """Tries to obtain callable MediaInfo version"""
         try:
-            stdout = execute(
-                command=[self.executable,'--Version']
-            )['stdout'].replace('\n', '')
-            self.version = re.search( r"(v[\.0-9]+)", stdout ).group(0)
+            stdout = execute(command=[self.executable, "--Version"])["stdout"].replace(
+                "\n", ""
+            )
+            version_match = re.search(r"(v[\.0-9]+)", stdout)
+            if not version_match:
+                raise ValueError(f"version text doesnt match regex: '{stdout}'")
+            self.version = version_match.group(0)  # type: ignore
         except AttributeError as e:
-            raise ValueError(f"MediaInfo : could not find a version number from string '{stdout}'") from e
-
+            raise ValueError(
+                f"MediaInfo : could not find a version number from string '{stdout}'"
+            ) from e
 
     def __str__(self) -> str:
-        return f"< Mediainfo : executable '{self.executable}' version '{self.version}' >"
-
+        return f"<Mediainfo : executable:'{self.executable}' version:'{self.version}'>"
 
     def __repr__(self) -> str:
         return str(self)
 
-
     @classmethod
-    def __try_casting_numbers( cls, s: str ) -> MEDIAINFO_POSSIBLE_RETURN_VALUES:
-        ''' Simple helper function; tries to cast str -> int/float
+    def __try_casting_numbers(cls, s: str) -> MEDIAINFO_POSSIBLE_RETURN_VALUES:
+        """Simple helper function; tries to cast str -> int/float
         returns argument when fails
-        '''
-        
+        """
+
         try:
             return int(s)
         except ValueError:
             try:
                 return float(s)
             except ValueError:
                 return s
 
-
     @classmethod
-    def __filter_data( cls, s: str ) -> MEDIAINFO_POSSIBLE_RETURN_VALUES:
-        ''' MediaInfo typically returns a number. This function handles the conversion 
+    def __filter_data(cls, s: str) -> MEDIAINFO_POSSIBLE_RETURN_VALUES:
+        """MediaInfo typically returns a number. This function handles the conversion
         process in the case this number includes a unit and a "simple"/"raw" value is
-        desired. 
-        
-        Note that after the conversion the value is passed to `MediaInfo.__try_casting_numbers` 
+        desired.
+
+        Note that after the conversion the value is passed to `MediaInfo.__try_casting_numbers`
         for basic int/float conversion.
-        '''
-        if s in ['','\r\n','\n', None]:
+        """
+        if s in ["", "\r\n", "\n", None]:
             return None
-            
-        for unit,mult in cls.UNIT_FACTOR.items():
-            pos = s.find( unit )                
+
+        for unit, mult in cls.UNIT_FACTOR.items():
+            pos = s.find(unit)
             if pos != -1:
-                s_ok = re.sub( r'(\d) (\d)', r'\1\2', s[:pos] ) # remove unit and spaces between numbers
-                val = MediaInfo.__try_casting_numbers( s_ok )
+                s_ok = re.sub(
+                    r"(\d) (\d)", r"\1\2", s[:pos]
+                )  # remove unit and spaces between numbers
+                val = MediaInfo.__try_casting_numbers(s_ok)
 
-                if type(val) in [int,float]:
+                if isinstance(val, (int, float)):
                     # successful cast
                     return val * mult
-        
-        return MediaInfo.__try_casting_numbers(s)
 
+        return MediaInfo.__try_casting_numbers(s)
 
-    def get_base_stats( self, media_file: Path ) -> Dict[str,Dict[str,MEDIAINFO_POSSIBLE_RETURN_VALUES]]:
-        ''' Convenience function : retrieves the stats returned by MediaInfo 
+    def get_base_stats(
+        self, media_file: Path
+    ) -> Dict[str, Dict[str, MEDIAINFO_POSSIBLE_RETURN_VALUES]]:
+        """Convenience function : retrieves the stats returned by MediaInfo
         when ran without specific arguments
 
-        WARNING: Some values returned by default by MediaInfo are imprecise 
+        WARNING: Some values returned by default by MediaInfo are imprecise
         or rounded, typically because they are expressed in user-friendly
         units like 'Mb/s', 'GiB', etc
 
         Returns : <dict[<category_name:str>,<dict[<datapoint_name:str>,<MediaInfo_value>]>]>
-        '''
-        type_assert( media_file, 'media_file', Path, 'MediaInfo::get_base_stats: ' )
+        """
+        type_assert(media_file, "media_file", Path, "MediaInfo::get_base_stats: ")
         _file = media_file.resolve()
-        stdout = execute( [self.executable, str(_file)] )['stdout']
+        stdout = execute([self.executable, str(_file)])["stdout"]
 
-        if stdout.strip()=='':
-            self.log.warning("Could not retrieve data from file %s. Name too long ?", media_file)
+        if stdout.strip() == "":
+            self.log.warning(
+                "Could not retrieve data from file %s. Name too long ?", media_file
+            )
             return {}
 
         # Preprocessing : decoding, splitting lines, regrouping datapoints
-        category = 'Uncategorized'
-        lines = { category : list() }
+        category = "Uncategorized"
+        lines: Dict[str, list] = {category: []}
         for line in stdout.splitlines():
-            
             # Discard empty lines
             if not line:
                 continue
-                
+
             # Data lines have ':'
-            if ':' in line:
-                lines[category].append( line.split(':') )
+            if ":" in line:
+                lines[category].append(line.split(":"))
                 continue
 
             # Category line (?)
             category = line
-            lines[category] = list()
+            lines[category] = []
 
         # Return actual data, nicely formatted
         res = {
             category: {
-                s_data[0].strip():MediaInfo.__filter_data(s_data[1].strip())
-                for s_data in lines[category]
+                s_data[0].strip(): MediaInfo.__filter_data(s_data[1].strip())
+                for s_data in category_lines
             }
-            for category in lines
-            if lines[category]
+            for category, category_lines in lines.items()
+            if category_lines
         }
 
         # cleanup
-        cleanup = {
-            'Video': {
-                'Frame rate': r'([\.0-9]+) \([0-9/]+\) FPS'
-            }
-        }
-        for _category,_cat_rules in cleanup.items():
+        cleanup = {"Video": {"Frame rate": r"([\.0-9]+) \([0-9/]+\) FPS"}}
+        for _category, _cat_rules in cleanup.items():
             if _category not in res:
                 continue
 
             for _datapoint, _datapoint_rule in _cat_rules.items():
                 if _datapoint not in res[_category]:
                     continue
-                if not isinstance( res[_category][_datapoint], str ):
+                if not isinstance(res[_category][_datapoint], str):
                     continue
 
                 # apply cleanup regex
                 regex_res = re.search(
-                    pattern=_datapoint_rule,
-                    string=res[_category][_datapoint]
+                    pattern=_datapoint_rule, string=str(res[_category][_datapoint])
                 )
                 if regex_res:
                     res[_category][_datapoint] = self.__try_casting_numbers(
                         regex_res[1]
                     )
 
         return res
 
-
-    def __get_datapoint( self, media_file: Path, datapoint: Datapoint ) -> MEDIAINFO_POSSIBLE_RETURN_VALUES:
-        ''' Calls MediaInfo to get a datapoint value.
+    def __get_datapoint(
+        self, media_file: Path, datapoint: Datapoint
+    ) -> MEDIAINFO_POSSIBLE_RETURN_VALUES:
+        """Calls MediaInfo to get a datapoint value.
         `datapoint` must be in a form understandable by MediaInfo, like '--Inform=Video;%UniqueID%'
-        '''
+        """
 
-        data = execute( 
-            [ 
-                self.executable,
-                str(datapoint),
-                str(media_file)
-            ]
-        )['stdout']
+        data = execute([self.executable, str(datapoint), str(media_file)])["stdout"]
 
-        if data.strip()=='':
-            self.log.warning("Could not retrieve data from file %s. Name too long ?", media_file)
+        if data.strip() == "":
+            self.log.warning(
+                "Could not retrieve data from file %s. Name too long ?", media_file
+            )
             return None
-        
-        return data
 
+        return data
 
-    def get_datapoint( self, media_file: Path, datapoint: str ) -> MEDIAINFO_POSSIBLE_RETURN_VALUES:
-        ''' Gets one datapoint's value
+    def get_datapoint(
+        self, media_file: Path, datapoint: str
+    ) -> MEDIAINFO_POSSIBLE_RETURN_VALUES:
+        """Gets one datapoint's value
         For multiple datapoints, use `MediaInfo.get_datapoints`
 
         `datapoint` can be in a shorthand format
 
         Returns : <dict[<datapoint_name:str>,<MediaInfo_value>]>
-        '''
-        type_assert( media_file, 'media_file', Path, 'MediaInfo::get_base_stats: ' )
+        """
+        type_assert(media_file, "media_file", Path, "MediaInfo::get_base_stats: ")
         _file = media_file.resolve()
 
         # `datapoint` may be a shorthand datapoint reference. ex : 'V_UniqueID' is shorthand for '--Inform=Video;%UniqueID%'
-        dp = Datapoint.from_string( self.DATAPOINTS.get( datapoint, datapoint ) )
-        return MediaInfo.__filter_data(self.__get_datapoint( _file, dp ))
-
+        dp = Datapoint.from_string(self.DATAPOINTS.get(datapoint, datapoint))
+        dp_value = self.__get_datapoint(_file, dp)
+        return (
+            MediaInfo.__filter_data(dp_value) if isinstance(dp_value, str) else dp_value
+        )
 
-    def get_datapoints( self, media_file: Path, datapoints: List[str], existing_stats=None ) -> Dict[str,MEDIAINFO_POSSIBLE_RETURN_VALUES]:
-        ''' Gets multiple datapoints with as few calls as possible.
+    def get_datapoints(
+        self, media_file: Path, datapoints: List[str], existing_stats=None
+    ) -> Dict[str, MEDIAINFO_POSSIBLE_RETURN_VALUES]:
+        """Gets multiple datapoints with as few calls as possible.
         This is done by grouping them by category
 
         `datapoint` can be in a shorthand format
 
         `existing_stats`: to update existing stats
 
-        Technical note : MediaInfo supports returning multiple values per call, 
+        Technical note : MediaInfo supports returning multiple values per call,
         but this is limited to parameters of the same category.
 
         Performance note : Internal testing shows that execution time grows linearly
         with the number of calls to `MediaInfo.exec`, therefore using `MediaInfo.get_datapoints`
         is recommended over `MediaInfo.get_datapoints` when more than one datapoint is needed. (TODO: correct note)
 
         Returns : <dict[<datapoint_name:str>,<MediaInfo_value>]>
-        '''
-        type_assert( media_file, 'media_file', Path, 'MediaInfo::get_base_stats: ' )
+        """
+        type_assert(media_file, "media_file", Path, "MediaInfo::get_base_stats: ")
         _file = media_file.resolve()
 
         # Combine datapoints
-        combined_datapoints = Datapoint.combine( 
-            Datapoint.from_strings(
-                [
-                    self.DATAPOINTS.get( dp, dp )
-                    for dp in datapoints
-                ]
-            )
+        combined_datapoints = Datapoint.combine(
+            Datapoint.from_strings([self.DATAPOINTS.get(dp, dp) for dp in datapoints])
         )
-        
+
         # Issue calls for each combined datapoint, store their result
-        res = dict() if existing_stats is None else existing_stats
+        def cleanup_name(name: str) -> str:
+            return (name[2:] if name.startswith("V_") else name).replace("%", "")
+
+        res = {} if existing_stats is None else existing_stats
         for dp in combined_datapoints:
-            answer = [
-                MediaInfo.__filter_data( dataline )
-                for dataline in self.__get_datapoint( _file, dp ).splitlines()
-            ]
+            data = self.__get_datapoint(_file, dp)
+            answer = (
+                [MediaInfo.__filter_data(dataline) for dataline in data.splitlines()]
+                if isinstance(data, str)
+                else [data]
+            )
+
             nb_answer = len(answer)
 
             cat = dp.category
 
             # storing results
-            if not cat in res:
-                res[cat] = dict()
-                
-            if isinstance(dp.parameter, str) and nb_answer==1:
+            if cat not in res:
+                res[cat] = {}
+
+            if isinstance(dp.parameter, str) and nb_answer == 1:
                 # Datapoint with 1 parameter
-                res[cat].update({
-                    dp.parameter_shorthand[2:]:answer
-                })
+                res[cat].update({cleanup_name(dp.parameter_shorthand): answer})
                 continue
 
-            if nb_answer==len(dp.parameter):
+            if nb_answer == len(dp.parameter):
                 # Datapoint with N>1 parameters
-                res[cat].update({
-                    p[2:]:a
-                    for p,a in zip( dp.parameter_shorthand, answer )
-                })
+                res[cat].update(
+                    {cleanup_name(p): a for p, a in zip(dp.parameter_shorthand, answer)}
+                )
                 continue
 
-            self.log.warning("Illegal state induced by faulty values : datapoint=%s, answer='%s' for file '%s'", dp, answer, media_file)
+            self.log.warning(
+                "Illegal state induced by faulty values : datapoint=%s, answer='%s' for file '%s'",
+                dp,
+                answer,
+                media_file,
+            )
 
         return res
```

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.6.dev1/src/DRSlib/os_detect.py` & `DRSlib-DavidRodriguezSoaresCUI-0.7.0/src/DRSlib/os_detect.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 ﻿# pylint: disable=too-few-public-methods
 
-# module-level docstring
-__doc__='''
+
+__doc__ = """
 OS detection module
 ===================
 
 Straightforward OS detection, for when platform-specific code must
 be written.
 
 I am not the original author of this class. It was downloaded from:
 https://github.com/scivision/pybashutils/blob/master/pybashutils/os_detect.py
 
-'''
+"""
 
 from platform import system, uname
 
+
 class Os:
     """
     returns class with properties:
     .cygwin   Cygwin detected
     .wsl      Windows Subsystem for Linux (WSL) detected
     .mac      Mac OS detected
     .linux    Linux detected
@@ -33,29 +34,29 @@
         self.cygwin = False
         self.wsl = False
         self.mac = False
         self.linux = False
         self.windows = False
         self.bsd = False
 
-        if 'cygwin' in syst:
+        if "cygwin" in syst:
             self.cygwin = True
-            self.os = 'cygwin'
-        elif 'darwin' in syst:
+            self.os = "cygwin"
+        elif "darwin" in syst:
             self.mac = True
-            self.os = 'mac'
-        elif 'linux' in syst:
-            if 'Microsoft' in uname().release:
+            self.os = "mac"
+        elif "linux" in syst:
+            if "Microsoft" in uname().release:
                 self.wsl = True
-                self.os = 'wsl'
+                self.os = "wsl"
             else:
                 self.linux = True
-                self.os = 'linux'
-        elif 'windows' in syst:
+                self.os = "linux"
+        elif "windows" in syst:
             self.windows = True
-            self.os = 'windows'
-        elif 'bsd' in syst:
+            self.os = "windows"
+        elif "bsd" in syst:
             self.bsd = True
-            self.os = 'bsd'
+            self.os = "bsd"
 
     def __str__(self):
         return self.os
```

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.6.dev1/src/DRSlib/spinner.py` & `DRSlib-DavidRodriguezSoaresCUI-0.7.0/src/DRSlib/spinner.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,68 +1,67 @@
 ﻿# pylint: disable=broad-except
 
-# module-level docstring
-__doc__='''
+
+__doc__ = """
 CLI text-based spinning animation
 =================================
 
 An exceedingly simplistic progress animation library.
-'''
+"""
 
 import itertools
 import os
 import sys
 from .str_utils import truncate_str
 
+
 class MySpinner:
-    ''' My simple spinner, one-function, easy to use and supports text
+    """My simple spinner, one-function, easy to use and supports text
     on the left of the spinning wheel !
-    
+
     Usage example::
 
         spinner = MySpinner()
         nb_items = len(items_to_process)
         for idx, item in enumerate(items_to_process):
             if idx%10==0:
-                spinner.animation( text=f"Progress: {100*idx/nb_items:.1f}%" ) 
-            process_item( item )
-            
-    '''
+                spinner.animation(text=f"Progress: {100*idx/nb_items:.1f}%")
+            process_item(item)
 
-    def __init__( self ) -> None:
+    """
+
+    def __init__(self) -> None:
         self.last_txt_len = 0
-        self.spinner = itertools.cycle(['-', '\\', '|', '/'])
+        self.spinner = itertools.cycle(["-", "\\", "|", "/"])
         try:
             self.terminal_width = os.get_terminal_size().columns
         except Exception as e:
-            print(f"MySpinner: Could not get terminal width, defaulting to 40 columns. Got error {e}")
+            print(
+                f"MySpinner: Could not get terminal width, defaulting to 40 columns. Got error {e}"
+            )
             self.terminal_width = 40
         # print(f"MySpinner: terminal width is {self.terminal_width}")
 
-
-    def animation( self, text: str = '', no_spinner: bool = False ):
-        ''' update animation, with the option to print text on the left of the
+    def animation(self, text: str = "", no_spinner: bool = False):
+        """update animation, with the option to print text on the left of the
         spinner character
-        '''
-        tmplen = (self.last_txt_len + 1)
+        """
+        tmplen = self.last_txt_len + 1
         # erase previous message
         # why do backspaces, then whitespace, then backspaces again :
         # because backspace alone didn't consistently erase previous text
-        sys.stdout.write( '\b' * tmplen + ' ' * tmplen + '\b' * tmplen ) 
+        sys.stdout.write("\b" * tmplen + " " * tmplen + "\b" * tmplen)
 
         # write new message, truncated to not overflow terminal width (necessary for best results)
-        spinner_symbol = '' if no_spinner else next(self.spinner)
+        spinner_symbol = "" if no_spinner else next(self.spinner)
         message = truncate_str(
             text + spinner_symbol,
-            output_length=self.terminal_width-1, 
-            cut_location='center'
+            output_length=self.terminal_width - 1,
+            cut_location="center",
         )
-        sys.stdout.write( 
-            message
-        ) 
+        sys.stdout.write(message)
         sys.stdout.flush()
-        self.last_txt_len = len( message ) - (0 if no_spinner else 1)
+        self.last_txt_len = len(message) - (0 if no_spinner else 1)
 
-    def clear( self ):
-        ''' erase spinner character (and accompanying text)
-        '''
-        self.animation( no_spinner=True )
+    def clear(self):
+        """erase spinner character (and accompanying text)"""
+        self.animation(no_spinner=True)
```

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.6.dev1/src/DRSlib/str_utils.py` & `DRSlib-DavidRodriguezSoaresCUI-0.7.0/src/DRSlib/str_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,104 +1,114 @@
 # pylint: disable=too-many-return-statements
 
-# module-level docstring
-__doc__='''
+
+__doc__ = """
 String-focused utils
 ====================
 
 Simple utils that accomplish one task well, specifically string operations.
 
-'''
- 
+"""
+
 import re
 
-def ensure_double_quotes( s: str ) -> str:
-    ''' Ensures s is double quoted in a particular way :
+
+def ensure_double_quotes(s: str) -> str:
+    """Ensures s is double quoted in a particular way :
      - returned string must begin and end with a double quote character `"`
      - any double quote that isn't at the beginning or end must be escaped `\\"`
 
     Examples :
      - `` (empty string) -> `""`
      - `.` -> `"."`
      - `hello` -> `"hello"`
      - `"hello` -> `"hello"`
      - `hello"` -> `"hello"`
      - `"hello"` -> `"hello"` (unchanged)
      - `"he"llo` -> `"he\\"llo"`
      - `"he\\"llo"` -> `"he\\"llo"` (unchanged)
 
-    '''
+    """
 
     if not s:
         return '""'
-    if len(s)==1:
-        if s[0]=='"':
+    if len(s) == 1:
+        if s[0] == '"':
             return '"\\""'
         return '"' + s + '"'
     # else
     if s[0] != '"':
-        return ensure_double_quotes( '"' + s )
+        return ensure_double_quotes('"' + s)
     if s[-1] != '"':
-        return ensure_double_quotes( s + '"' )
+        return ensure_double_quotes(s + '"')
 
     # past this point, 2 <= len(s) and there are double quotes at the beginning and end of s.
-    
-    double_quote_locations = set( m.start() for m in re.finditer(r'"', s) )
-    escaped_double_quote_locations = set( m.start()+1 for m in re.finditer(r'\\"', s) )
-    double_quote_locations.difference_update( escaped_double_quote_locations )
+
+    double_quote_locations = set(m.start() for m in re.finditer(r'"', s))
+    escaped_double_quote_locations = set(m.start() + 1 for m in re.finditer(r'\\"', s))
+    double_quote_locations.difference_update(escaped_double_quote_locations)
 
     # s lacks any double quotes
     if not double_quote_locations:
         return '"' + s + '"'
 
     # detection of double quotes to escape
-    proper_double_quote_location = set( [0, len(s)-1] )
-    misplaced_double_quotes = set(double_quote_locations).difference( proper_double_quote_location )
+    proper_double_quote_location = set([0, len(s) - 1])
+    misplaced_double_quotes = set(double_quote_locations).difference(
+        proper_double_quote_location
+    )
     # print(f"proper_double_quote_location={proper_double_quote_location}")
     # print(f"double_quote_locations={double_quote_locations}")
     # print(f"misplaced_double_quotes={misplaced_double_quotes}")
-    
+
     # s is already properly double quoted
     if not misplaced_double_quotes:
         return s
 
     # escaping double quotes plus recursion
     s_characters = list(s)
     misplaced_DQ_idx = misplaced_double_quotes.pop()
-    _s = ''.join( s_characters[:misplaced_DQ_idx] + [ '\\', '"' ] + s_characters[misplaced_DQ_idx+1:] )
-    return ensure_double_quotes( _s )
+    _s = "".join(
+        s_characters[:misplaced_DQ_idx]
+        + ["\\", '"']
+        + s_characters[misplaced_DQ_idx + 1 :]
+    )
+    return ensure_double_quotes(_s)
 
 
-def truncate_str( s: str, output_length: int, cut_location: str = 'center' ) -> str:
-    ''' Truncates string to a new length
-    
+def truncate_str(s: str, output_length: int, cut_location: str = "center") -> str:
+    """Truncates string to a new length
+
     `cut_location` : (default:'center') in ['left','center','right']
-    ''' 
+    """
     s_len = len(s)
     if s_len <= output_length:
-        return s 
+        return s
     if output_length <= 7:
-        print(f"Warning: used truncate_str with 'output_length'={output_length}<=7, which is too low and would probably result in undesired results, so 's' was returned unchanged !")
+        print(
+            f"Warning: used truncate_str with 'output_length'={output_length}<=7, which is too low and would probably result in undesired results, so 's' was returned unchanged !"
+        )
         return s
 
-    #len_diff = s_len-output_length
-    if cut_location=='left':
-        return f"{ s[:output_length-6] } [...]"
-    if cut_location=='center':
+    # len_diff = s_len-output_length
+    if cut_location == "left":
+        return f"{s[:output_length-6]} [...]"
+    if cut_location == "center":
         offset = (output_length // 2) - 3
-        return f"{ s[:offset] } [...] { s[-(offset - (1 if output_length%2==0 else 0)):] }"
+        return f"{s[:offset]} [...] {s[-(offset - (1 if output_length%2==0 else 0)):]}"
 
-    if cut_location=='right':
-        return f"[...] { s[-(output_length-6):] }"
+    if cut_location == "right":
+        return f"[...] {s[-(output_length-6):]}"
     # else
-    raise ValueError(f"truncate_str: given parameter 'cut_location'={cut_location} is not in ['left','center','right'] !")
+    raise ValueError(
+        f"truncate_str: given parameter 'cut_location'={cut_location} is not in ['left','center','right'] !"
+    )
 
 
-if __name__=='__main__':
-
+if __name__ == "__main__":
     # ensure_double_quotes tests
 
     # tests = [
     #     '',
     #     '.',
     #     '"',
     #     '"hello',
@@ -108,19 +118,17 @@
     #     'he\\"llo'
     # ]
 
     # for test_s in tests:
     #     res = ensure_double_quotes(test_s)
     #     print(f"test_s={test_s}={list(test_s)} -> {list(res)} = {res}")
 
-
     # truncate_str tests
 
-    tests = [
-        'h'* 20,
-        'h' * 21
-    ]
-    for new_len in [10,15]:
-        for cut in ['left','center','right']:
+    tests = ["h" * 20, "h" * 21]
+    for new_len in [10, 15]:
+        for cut in ["left", "center", "right"]:
             for test_s in tests:
-                res = truncate_str( test_s, new_len, cut)
-                print(f"new_len={new_len}, cut={cut} : test_s='{test_s}' (len={len(test_s)}) -> '{res}' (len={len(res)})")
+                res = truncate_str(test_s, new_len, cut)
+                print(
+                    f"new_len={new_len}, cut={cut} : test_s='{test_s}' (len={len(test_s)}) -> '{res}' (len={len(res)})"
+                )
```

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.6.dev1/src/DRSlib_DavidRodriguezSoaresCUI.egg-info/PKG-INFO` & `DRSlib-DavidRodriguezSoaresCUI-0.7.0/src/DRSlib_DavidRodriguezSoaresCUI.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: DRSlib-DavidRodriguezSoaresCUI
-Version: 0.6.dev1
+Version: 0.7.0
 Summary: DRSlib - a set of utilities by DavidRodriguezSoaresCUI
 Home-page: https://github.com/DavidRodriguezSoaresCUI/DRSlib
 Author: DavidRodriguezSoaresCUI
 Author-email: fireblaze904+DRSlib@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/DavidRodriguezSoaresCUI/DRSlib/issues
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -70,9 +68,7 @@
 ## Warning to users
 
 **DRSlib** is a quickly evolving package, and author doesn't take any responsibility to maintain it or to keep
 its API stable, but will make a good faith effort to do so. Also, some of its code writes to the disk, so its use 
 may lead to data loss.
 
 Use it at your own risk.
-
-
```

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.6.dev1/src/DRSlib_DavidRodriguezSoaresCUI.egg-info/SOURCES.txt` & `DRSlib-DavidRodriguezSoaresCUI-0.7.0/src/DRSlib_DavidRodriguezSoaresCUI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

