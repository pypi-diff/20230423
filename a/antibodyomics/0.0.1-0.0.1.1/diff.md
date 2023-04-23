# Comparing `tmp/antibodyomics-0.0.1.tar.gz` & `tmp/antibodyomics-0.0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antibodyomics-0.0.1.tar", last modified: Sun Apr 23 20:56:20 2023, max compression
+gzip compressed data, was "antibodyomics-0.0.1.1.tar", last modified: Sun Apr 23 21:07:35 2023, max compression
```

## Comparing `antibodyomics-0.0.1.tar` & `antibodyomics-0.0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 schaubaj (755442540) NIH\Domain Users (1360859114)        0 2023-04-23 20:56:20.064036 antibodyomics-0.0.1/
--rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)     1070 2023-04-23 19:59:15.000000 antibodyomics-0.0.1/LICENSE
--rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)      773 2023-04-23 20:56:20.063869 antibodyomics-0.0.1/PKG-INFO
--rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)      247 2023-04-23 20:10:41.000000 antibodyomics-0.0.1/README.md
--rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)      599 2023-04-23 20:55:57.000000 antibodyomics-0.0.1/pyproject.toml
--rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)       38 2023-04-23 20:56:20.064084 antibodyomics-0.0.1/setup.cfg
-drwxrwxr-x   0 schaubaj (755442540) NIH\Domain Users (1360859114)        0 2023-04-23 20:56:20.046632 antibodyomics-0.0.1/src/
-drwxrwxr-x   0 schaubaj (755442540) NIH\Domain Users (1360859114)        0 2023-04-23 20:56:20.054938 antibodyomics-0.0.1/src/antibodyomics/
--rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)        0 2023-04-23 20:12:12.000000 antibodyomics-0.0.1/src/antibodyomics/__init__.py
--rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)       43 2023-04-23 20:12:59.000000 antibodyomics-0.0.1/src/antibodyomics/example.py
-drwxrwxr-x   0 schaubaj (755442540) NIH\Domain Users (1360859114)        0 2023-04-23 20:56:20.062305 antibodyomics-0.0.1/src/antibodyomics.egg-info/
--rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)      773 2023-04-23 20:56:20.000000 antibodyomics-0.0.1/src/antibodyomics.egg-info/PKG-INFO
--rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)      324 2023-04-23 20:56:20.000000 antibodyomics-0.0.1/src/antibodyomics.egg-info/SOURCES.txt
--rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)        1 2023-04-23 20:56:20.000000 antibodyomics-0.0.1/src/antibodyomics.egg-info/dependency_links.txt
--rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)       33 2023-04-23 20:56:20.000000 antibodyomics-0.0.1/src/antibodyomics.egg-info/top_level.txt
-drwxrwxr-x   0 schaubaj (755442540) NIH\Domain Users (1360859114)        0 2023-04-23 20:56:20.063628 antibodyomics-0.0.1/src/antibodyomics_test/
--rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)        0 2023-04-23 20:12:12.000000 antibodyomics-0.0.1/src/antibodyomics_test/__init__.py
--rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)       43 2023-04-23 20:12:59.000000 antibodyomics-0.0.1/src/antibodyomics_test/example.py
+drwxrwxr-x   0 schaubaj (755442540) NIH\Domain Users (1360859114)        0 2023-04-23 21:07:35.215928 antibodyomics-0.0.1.1/
+-rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)     1070 2023-04-23 19:59:15.000000 antibodyomics-0.0.1.1/LICENSE
+-rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)     1100 2023-04-23 21:07:35.215787 antibodyomics-0.0.1.1/PKG-INFO
+-rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)      571 2023-04-23 21:05:01.000000 antibodyomics-0.0.1.1/README.md
+-rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)      601 2023-04-23 21:06:35.000000 antibodyomics-0.0.1.1/pyproject.toml
+-rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)       38 2023-04-23 21:07:35.215968 antibodyomics-0.0.1.1/setup.cfg
+drwxrwxr-x   0 schaubaj (755442540) NIH\Domain Users (1360859114)        0 2023-04-23 21:07:35.212854 antibodyomics-0.0.1.1/src/
+drwxrwxr-x   0 schaubaj (755442540) NIH\Domain Users (1360859114)        0 2023-04-23 21:07:35.214361 antibodyomics-0.0.1.1/src/antibodyomics/
+-rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)        0 2023-04-23 20:12:12.000000 antibodyomics-0.0.1.1/src/antibodyomics/__init__.py
+-rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)       43 2023-04-23 20:12:59.000000 antibodyomics-0.0.1.1/src/antibodyomics/example.py
+drwxrwxr-x   0 schaubaj (755442540) NIH\Domain Users (1360859114)        0 2023-04-23 21:07:35.215190 antibodyomics-0.0.1.1/src/antibodyomics.egg-info/
+-rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)     1100 2023-04-23 21:07:35.000000 antibodyomics-0.0.1.1/src/antibodyomics.egg-info/PKG-INFO
+-rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)      324 2023-04-23 21:07:35.000000 antibodyomics-0.0.1.1/src/antibodyomics.egg-info/SOURCES.txt
+-rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)        1 2023-04-23 21:07:35.000000 antibodyomics-0.0.1.1/src/antibodyomics.egg-info/dependency_links.txt
+-rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)       33 2023-04-23 21:07:35.000000 antibodyomics-0.0.1.1/src/antibodyomics.egg-info/top_level.txt
+drwxrwxr-x   0 schaubaj (755442540) NIH\Domain Users (1360859114)        0 2023-04-23 21:07:35.215602 antibodyomics-0.0.1.1/src/antibodyomics_test/
+-rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)        0 2023-04-23 20:12:12.000000 antibodyomics-0.0.1.1/src/antibodyomics_test/__init__.py
+-rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)       43 2023-04-23 20:12:59.000000 antibodyomics-0.0.1.1/src/antibodyomics_test/example.py
```

### Comparing `antibodyomics-0.0.1/LICENSE` & `antibodyomics-0.0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `antibodyomics-0.0.1/PKG-INFO` & `antibodyomics-0.0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,69 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 616e 7469  : 2.1.Name: anti
 00000020: 626f 6479 6f6d 6963 730a 5665 7273 696f  bodyomics.Versio
-00000030: 6e3a 2030 2e30 2e31 0a53 756d 6d61 7279  n: 0.0.1.Summary
-00000040: 3a20 416e 2061 6e74 6962 6f64 796f 6d69  : An antibodyomi
-00000050: 6373 206c 6962 7261 7279 0a41 7574 686f  cs library.Autho
-00000060: 722d 656d 6169 6c3a 2041 6e64 7265 7720  r-email: Andrew 
-00000070: 5363 6861 7562 203c 616e 6472 6577 2e73  Schaub <andrew.s
-00000080: 6368 6175 6240 7072 6f74 6f6e 6d61 696c  chaub@protonmail
-00000090: 2e63 6f6d 3e0a 5072 6f6a 6563 742d 5552  .com>.Project-UR
-000000a0: 4c3a 2048 6f6d 6570 6167 652c 2068 7474  L: Homepage, htt
-000000b0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000000c0: 6472 6577 7363 6861 7562 2f61 6e74 6962  drewschaub/antib
-000000d0: 6f64 796f 6d69 6373 0a50 726f 6a65 6374  odyomics.Project
-000000e0: 2d55 524c 3a20 4275 6720 5472 6163 6b65  -URL: Bug Tracke
-000000f0: 722c 2068 7474 7073 3a2f 2f67 6974 6875  r, https://githu
-00000100: 622e 636f 6d2f 6472 6577 7363 6861 7562  b.com/drewschaub
-00000110: 2f61 6e74 6962 6f64 796f 6d69 6373 2f69  /antibodyomics/i
-00000120: 7373 7565 730a 436c 6173 7369 6669 6572  ssues.Classifier
-00000130: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
-00000140: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000150: 203a 3a20 330a 436c 6173 7369 6669 6572   :: 3.Classifier
-00000160: 3a20 4c69 6365 6e73 6520 3a3a 204f 5349  : License :: OSI
-00000170: 2041 7070 726f 7665 6420 3a3a 204d 4954   Approved :: MIT
-00000180: 204c 6963 656e 7365 0a43 6c61 7373 6966   License.Classif
-00000190: 6965 723a 204f 7065 7261 7469 6e67 2053  ier: Operating S
-000001a0: 7973 7465 6d20 3a3a 204f 5320 496e 6465  ystem :: OS Inde
-000001b0: 7065 6e64 656e 740a 5265 7175 6972 6573  pendent.Requires
-000001c0: 2d50 7974 686f 6e3a 203e 3d33 2e37 0a44  -Python: >=3.7.D
-000001d0: 6573 6372 6970 7469 6f6e 2d43 6f6e 7465  escription-Conte
-000001e0: 6e74 2d54 7970 653a 2074 6578 742f 6d61  nt-Type: text/ma
-000001f0: 726b 646f 776e 0a4c 6963 656e 7365 2d46  rkdown.License-F
-00000200: 696c 653a 204c 4943 454e 5345 0a0a 2320  ile: LICENSE..# 
-00000210: 616e 7469 626f 6479 6f6d 6963 730a 0a23  antibodyomics..#
-00000220: 2320 4261 636b 656e 640a 0a49 276d 2075  # Backend..I'm u
-00000230: 7369 6e67 2073 6574 7570 746f 6f6c 732c  sing setuptools,
-00000240: 2062 7574 206f 7468 6572 206f 7074 696f   but other optio
-00000250: 6e73 2077 6572 6520 4861 7463 686c 696e  ns were Hatchlin
-00000260: 672c 2046 6c69 7420 616e 6420 5044 4d0a  g, Flit and PDM.
-00000270: 0a68 7474 7073 3a2f 2f70 6163 6b61 6769  .https://packagi
-00000280: 6e67 2e70 7974 686f 6e2e 6f72 672f 656e  ng.python.org/en
-00000290: 2f6c 6174 6573 742f 7475 746f 7269 616c  /latest/tutorial
-000002a0: 732f 7061 636b 6167 696e 672d 7072 6f6a  s/packaging-proj
-000002b0: 6563 7473 2f0a 0a0a 2323 2041 6374 696f  ects/...## Actio
-000002c0: 6e20 4974 656d 730a 0a31 2e20 4920 6e65  n Items..1. I ne
-000002d0: 6564 2074 6f20 6164 6420 7468 6520 7265  ed to add the re
-000002e0: 7175 6972 6564 2070 6163 6b61 6765 7320  quired packages 
-000002f0: 746f 2060 7079 7072 6f6a 6563 742e 746f  to `pyproject.to
-00000300: 6d6c 6020 0a                             ml` .
+00000030: 6e3a 2030 2e30 2e31 2e31 0a53 756d 6d61  n: 0.0.1.1.Summa
+00000040: 7279 3a20 416e 2061 6e74 6962 6f64 796f  ry: An antibodyo
+00000050: 6d69 6373 206c 6962 7261 7279 0a41 7574  mics library.Aut
+00000060: 686f 722d 656d 6169 6c3a 2041 6e64 7265  hor-email: Andre
+00000070: 7720 5363 6861 7562 203c 616e 6472 6577  w Schaub <andrew
+00000080: 2e73 6368 6175 6240 7072 6f74 6f6e 6d61  .schaub@protonma
+00000090: 696c 2e63 6f6d 3e0a 5072 6f6a 6563 742d  il.com>.Project-
+000000a0: 5552 4c3a 2048 6f6d 6570 6167 652c 2068  URL: Homepage, h
+000000b0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000000c0: 6d2f 6472 6577 7363 6861 7562 2f61 6e74  m/drewschaub/ant
+000000d0: 6962 6f64 796f 6d69 6373 0a50 726f 6a65  ibodyomics.Proje
+000000e0: 6374 2d55 524c 3a20 4275 6720 5472 6163  ct-URL: Bug Trac
+000000f0: 6b65 722c 2068 7474 7073 3a2f 2f67 6974  ker, https://git
+00000100: 6875 622e 636f 6d2f 6472 6577 7363 6861  hub.com/drewscha
+00000110: 7562 2f61 6e74 6962 6f64 796f 6d69 6373  ub/antibodyomics
+00000120: 2f69 7373 7565 730a 436c 6173 7369 6669  /issues.Classifi
+00000130: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
+00000140: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000150: 6f6e 203a 3a20 330a 436c 6173 7369 6669  on :: 3.Classifi
+00000160: 6572 3a20 4c69 6365 6e73 6520 3a3a 204f  er: License :: O
+00000170: 5349 2041 7070 726f 7665 6420 3a3a 204d  SI Approved :: M
+00000180: 4954 204c 6963 656e 7365 0a43 6c61 7373  IT License.Class
+00000190: 6966 6965 723a 204f 7065 7261 7469 6e67  ifier: Operating
+000001a0: 2053 7973 7465 6d20 3a3a 204f 5320 496e   System :: OS In
+000001b0: 6465 7065 6e64 656e 740a 5265 7175 6972  dependent.Requir
+000001c0: 6573 2d50 7974 686f 6e3a 203e 3d33 2e37  es-Python: >=3.7
+000001d0: 0a44 6573 6372 6970 7469 6f6e 2d43 6f6e  .Description-Con
+000001e0: 7465 6e74 2d54 7970 653a 2074 6578 742f  tent-Type: text/
+000001f0: 6d61 726b 646f 776e 0a4c 6963 656e 7365  markdown.License
+00000200: 2d46 696c 653a 204c 4943 454e 5345 0a0a  -File: LICENSE..
+00000210: 2323 2041 626f 7574 0a0a 2d2d 2d0a 0a2a  ## About..---..*
+00000220: 2a53 6f75 7263 6520 436f 6465 2a2a 3a20  *Source Code**: 
+00000230: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00000240: 2f68 7474 7073 3a2f 2f67 6974 6875 622e  /https://github.
+00000250: 636f 6d2f 6472 6577 7363 6861 7562 2f61  com/drewschaub/a
+00000260: 6e74 6962 6f64 796f 6d69 6373 2220 7461  ntibodyomics" ta
+00000270: 7267 6574 3d22 5f62 6c61 6e6b 223e 6874  rget="_blank">ht
+00000280: 7470 733a 2f2f 6874 7470 733a 2f2f 6769  tps://https://gi
+00000290: 7468 7562 2e63 6f6d 2f64 7265 7773 6368  thub.com/drewsch
+000002a0: 6175 622f 616e 7469 626f 6479 6f6d 6963  aub/antibodyomic
+000002b0: 733c 2f61 3e0a 0a2d 2d2d 0a0a 416e 7469  s</a>..---..Anti
+000002c0: 626f 6479 6f6d 6963 7320 6973 2061 2070  bodyomics is a p
+000002d0: 7974 686f 6e20 6c69 6272 6172 7920 666f  ython library fo
+000002e0: 7220 7065 7266 6f72 6d69 6e67 2073 7472  r performing str
+000002f0: 7563 7475 7261 6c20 616e 6420 6765 6e65  uctural and gene
+00000300: 7469 6320 2062 696f 696e 666f 726d 6174  tic  bioinformat
+00000310: 6963 2061 6e61 6c79 7369 7320 696e 2070  ic analysis in p
+00000320: 7974 686f 6e2e 200a 0a23 2320 496e 7374  ython. ..## Inst
+00000330: 616c 6c61 7469 6f6e 0a0a 2d2d 2d0a 0a49  allation..---..I
+00000340: 6e73 7461 6c6c 6174 696f 6e20 6973 2068  nstallation is h
+00000350: 616e 646c 6564 2075 7369 6e67 2074 6865  andled using the
+00000360: 2070 7974 686f 6e20 7061 636b 6167 6520   python package 
+00000370: 696e 7374 616c 6c65 7220 6070 6970 600a  installer `pip`.
+00000380: 0a60 6060 636f 6e73 6f6c 650a 2420 7069  .```console.$ pi
+00000390: 7020 696e 7374 616c 6c20 616e 7469 626f  p install antibo
+000003a0: 6479 6f6d 6963 730a 6060 600a 0a23 2320  dyomics.```..## 
+000003b0: 4c69 6365 6e73 650a 0a5b 215b 4c69 6365  License..[![Lice
+000003c0: 6e73 655d 2868 7474 7073 3a2f 2f69 6d67  nse](https://img
+000003d0: 2e73 6869 656c 6473 2e69 6f2f 6769 7468  .shields.io/gith
+000003e0: 7562 2f6c 6963 656e 7365 2f64 7265 7773  ub/license/drews
+000003f0: 6368 6175 622f 616e 7469 626f 6479 6f6d  chaub/antibodyom
+00000400: 6963 7329 5d28 6874 7470 733a 2f2f 6f70  ics)](https://op
+00000410: 656e 736f 7572 6365 2e6f 7267 2f6c 6963  ensource.org/lic
+00000420: 656e 7365 732f 4d49 5429 0a0a 2d20 436f  enses/MIT)..- Co
+00000430: 7079 7269 6768 7420 c2a9 2041 6e64 7265  pyright .. Andre
+00000440: 7720 4a2e 2053 6368 6175 620a            w J. Schaub.
```

### Comparing `antibodyomics-0.0.1/pyproject.toml` & `antibodyomics-0.0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "antibodyomics"
-version = "0.0.1"
+version = "0.0.1.1"
 authors = [
   { name="Andrew Schaub", email="andrew.schaub@protonmail.com" },
 ]
 description = "An antibodyomics library"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `antibodyomics-0.0.1/src/antibodyomics.egg-info/PKG-INFO` & `antibodyomics-0.0.1.1/src/antibodyomics.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,69 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 616e 7469  : 2.1.Name: anti
 00000020: 626f 6479 6f6d 6963 730a 5665 7273 696f  bodyomics.Versio
-00000030: 6e3a 2030 2e30 2e31 0a53 756d 6d61 7279  n: 0.0.1.Summary
-00000040: 3a20 416e 2061 6e74 6962 6f64 796f 6d69  : An antibodyomi
-00000050: 6373 206c 6962 7261 7279 0a41 7574 686f  cs library.Autho
-00000060: 722d 656d 6169 6c3a 2041 6e64 7265 7720  r-email: Andrew 
-00000070: 5363 6861 7562 203c 616e 6472 6577 2e73  Schaub <andrew.s
-00000080: 6368 6175 6240 7072 6f74 6f6e 6d61 696c  chaub@protonmail
-00000090: 2e63 6f6d 3e0a 5072 6f6a 6563 742d 5552  .com>.Project-UR
-000000a0: 4c3a 2048 6f6d 6570 6167 652c 2068 7474  L: Homepage, htt
-000000b0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000000c0: 6472 6577 7363 6861 7562 2f61 6e74 6962  drewschaub/antib
-000000d0: 6f64 796f 6d69 6373 0a50 726f 6a65 6374  odyomics.Project
-000000e0: 2d55 524c 3a20 4275 6720 5472 6163 6b65  -URL: Bug Tracke
-000000f0: 722c 2068 7474 7073 3a2f 2f67 6974 6875  r, https://githu
-00000100: 622e 636f 6d2f 6472 6577 7363 6861 7562  b.com/drewschaub
-00000110: 2f61 6e74 6962 6f64 796f 6d69 6373 2f69  /antibodyomics/i
-00000120: 7373 7565 730a 436c 6173 7369 6669 6572  ssues.Classifier
-00000130: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
-00000140: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000150: 203a 3a20 330a 436c 6173 7369 6669 6572   :: 3.Classifier
-00000160: 3a20 4c69 6365 6e73 6520 3a3a 204f 5349  : License :: OSI
-00000170: 2041 7070 726f 7665 6420 3a3a 204d 4954   Approved :: MIT
-00000180: 204c 6963 656e 7365 0a43 6c61 7373 6966   License.Classif
-00000190: 6965 723a 204f 7065 7261 7469 6e67 2053  ier: Operating S
-000001a0: 7973 7465 6d20 3a3a 204f 5320 496e 6465  ystem :: OS Inde
-000001b0: 7065 6e64 656e 740a 5265 7175 6972 6573  pendent.Requires
-000001c0: 2d50 7974 686f 6e3a 203e 3d33 2e37 0a44  -Python: >=3.7.D
-000001d0: 6573 6372 6970 7469 6f6e 2d43 6f6e 7465  escription-Conte
-000001e0: 6e74 2d54 7970 653a 2074 6578 742f 6d61  nt-Type: text/ma
-000001f0: 726b 646f 776e 0a4c 6963 656e 7365 2d46  rkdown.License-F
-00000200: 696c 653a 204c 4943 454e 5345 0a0a 2320  ile: LICENSE..# 
-00000210: 616e 7469 626f 6479 6f6d 6963 730a 0a23  antibodyomics..#
-00000220: 2320 4261 636b 656e 640a 0a49 276d 2075  # Backend..I'm u
-00000230: 7369 6e67 2073 6574 7570 746f 6f6c 732c  sing setuptools,
-00000240: 2062 7574 206f 7468 6572 206f 7074 696f   but other optio
-00000250: 6e73 2077 6572 6520 4861 7463 686c 696e  ns were Hatchlin
-00000260: 672c 2046 6c69 7420 616e 6420 5044 4d0a  g, Flit and PDM.
-00000270: 0a68 7474 7073 3a2f 2f70 6163 6b61 6769  .https://packagi
-00000280: 6e67 2e70 7974 686f 6e2e 6f72 672f 656e  ng.python.org/en
-00000290: 2f6c 6174 6573 742f 7475 746f 7269 616c  /latest/tutorial
-000002a0: 732f 7061 636b 6167 696e 672d 7072 6f6a  s/packaging-proj
-000002b0: 6563 7473 2f0a 0a0a 2323 2041 6374 696f  ects/...## Actio
-000002c0: 6e20 4974 656d 730a 0a31 2e20 4920 6e65  n Items..1. I ne
-000002d0: 6564 2074 6f20 6164 6420 7468 6520 7265  ed to add the re
-000002e0: 7175 6972 6564 2070 6163 6b61 6765 7320  quired packages 
-000002f0: 746f 2060 7079 7072 6f6a 6563 742e 746f  to `pyproject.to
-00000300: 6d6c 6020 0a                             ml` .
+00000030: 6e3a 2030 2e30 2e31 2e31 0a53 756d 6d61  n: 0.0.1.1.Summa
+00000040: 7279 3a20 416e 2061 6e74 6962 6f64 796f  ry: An antibodyo
+00000050: 6d69 6373 206c 6962 7261 7279 0a41 7574  mics library.Aut
+00000060: 686f 722d 656d 6169 6c3a 2041 6e64 7265  hor-email: Andre
+00000070: 7720 5363 6861 7562 203c 616e 6472 6577  w Schaub <andrew
+00000080: 2e73 6368 6175 6240 7072 6f74 6f6e 6d61  .schaub@protonma
+00000090: 696c 2e63 6f6d 3e0a 5072 6f6a 6563 742d  il.com>.Project-
+000000a0: 5552 4c3a 2048 6f6d 6570 6167 652c 2068  URL: Homepage, h
+000000b0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000000c0: 6d2f 6472 6577 7363 6861 7562 2f61 6e74  m/drewschaub/ant
+000000d0: 6962 6f64 796f 6d69 6373 0a50 726f 6a65  ibodyomics.Proje
+000000e0: 6374 2d55 524c 3a20 4275 6720 5472 6163  ct-URL: Bug Trac
+000000f0: 6b65 722c 2068 7474 7073 3a2f 2f67 6974  ker, https://git
+00000100: 6875 622e 636f 6d2f 6472 6577 7363 6861  hub.com/drewscha
+00000110: 7562 2f61 6e74 6962 6f64 796f 6d69 6373  ub/antibodyomics
+00000120: 2f69 7373 7565 730a 436c 6173 7369 6669  /issues.Classifi
+00000130: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
+00000140: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000150: 6f6e 203a 3a20 330a 436c 6173 7369 6669  on :: 3.Classifi
+00000160: 6572 3a20 4c69 6365 6e73 6520 3a3a 204f  er: License :: O
+00000170: 5349 2041 7070 726f 7665 6420 3a3a 204d  SI Approved :: M
+00000180: 4954 204c 6963 656e 7365 0a43 6c61 7373  IT License.Class
+00000190: 6966 6965 723a 204f 7065 7261 7469 6e67  ifier: Operating
+000001a0: 2053 7973 7465 6d20 3a3a 204f 5320 496e   System :: OS In
+000001b0: 6465 7065 6e64 656e 740a 5265 7175 6972  dependent.Requir
+000001c0: 6573 2d50 7974 686f 6e3a 203e 3d33 2e37  es-Python: >=3.7
+000001d0: 0a44 6573 6372 6970 7469 6f6e 2d43 6f6e  .Description-Con
+000001e0: 7465 6e74 2d54 7970 653a 2074 6578 742f  tent-Type: text/
+000001f0: 6d61 726b 646f 776e 0a4c 6963 656e 7365  markdown.License
+00000200: 2d46 696c 653a 204c 4943 454e 5345 0a0a  -File: LICENSE..
+00000210: 2323 2041 626f 7574 0a0a 2d2d 2d0a 0a2a  ## About..---..*
+00000220: 2a53 6f75 7263 6520 436f 6465 2a2a 3a20  *Source Code**: 
+00000230: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00000240: 2f68 7474 7073 3a2f 2f67 6974 6875 622e  /https://github.
+00000250: 636f 6d2f 6472 6577 7363 6861 7562 2f61  com/drewschaub/a
+00000260: 6e74 6962 6f64 796f 6d69 6373 2220 7461  ntibodyomics" ta
+00000270: 7267 6574 3d22 5f62 6c61 6e6b 223e 6874  rget="_blank">ht
+00000280: 7470 733a 2f2f 6874 7470 733a 2f2f 6769  tps://https://gi
+00000290: 7468 7562 2e63 6f6d 2f64 7265 7773 6368  thub.com/drewsch
+000002a0: 6175 622f 616e 7469 626f 6479 6f6d 6963  aub/antibodyomic
+000002b0: 733c 2f61 3e0a 0a2d 2d2d 0a0a 416e 7469  s</a>..---..Anti
+000002c0: 626f 6479 6f6d 6963 7320 6973 2061 2070  bodyomics is a p
+000002d0: 7974 686f 6e20 6c69 6272 6172 7920 666f  ython library fo
+000002e0: 7220 7065 7266 6f72 6d69 6e67 2073 7472  r performing str
+000002f0: 7563 7475 7261 6c20 616e 6420 6765 6e65  uctural and gene
+00000300: 7469 6320 2062 696f 696e 666f 726d 6174  tic  bioinformat
+00000310: 6963 2061 6e61 6c79 7369 7320 696e 2070  ic analysis in p
+00000320: 7974 686f 6e2e 200a 0a23 2320 496e 7374  ython. ..## Inst
+00000330: 616c 6c61 7469 6f6e 0a0a 2d2d 2d0a 0a49  allation..---..I
+00000340: 6e73 7461 6c6c 6174 696f 6e20 6973 2068  nstallation is h
+00000350: 616e 646c 6564 2075 7369 6e67 2074 6865  andled using the
+00000360: 2070 7974 686f 6e20 7061 636b 6167 6520   python package 
+00000370: 696e 7374 616c 6c65 7220 6070 6970 600a  installer `pip`.
+00000380: 0a60 6060 636f 6e73 6f6c 650a 2420 7069  .```console.$ pi
+00000390: 7020 696e 7374 616c 6c20 616e 7469 626f  p install antibo
+000003a0: 6479 6f6d 6963 730a 6060 600a 0a23 2320  dyomics.```..## 
+000003b0: 4c69 6365 6e73 650a 0a5b 215b 4c69 6365  License..[![Lice
+000003c0: 6e73 655d 2868 7474 7073 3a2f 2f69 6d67  nse](https://img
+000003d0: 2e73 6869 656c 6473 2e69 6f2f 6769 7468  .shields.io/gith
+000003e0: 7562 2f6c 6963 656e 7365 2f64 7265 7773  ub/license/drews
+000003f0: 6368 6175 622f 616e 7469 626f 6479 6f6d  chaub/antibodyom
+00000400: 6963 7329 5d28 6874 7470 733a 2f2f 6f70  ics)](https://op
+00000410: 656e 736f 7572 6365 2e6f 7267 2f6c 6963  ensource.org/lic
+00000420: 656e 7365 732f 4d49 5429 0a0a 2d20 436f  enses/MIT)..- Co
+00000430: 7079 7269 6768 7420 c2a9 2041 6e64 7265  pyright .. Andre
+00000440: 7720 4a2e 2053 6368 6175 620a            w J. Schaub.
```

