# Comparing `tmp/vnpy_tqsdk-3.2.11.tar.gz` & `tmp/vnpy_tqsdk-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnpy_tqsdk-3.2.11.tar", last modified: Fri Aug  5 14:22:05 2022, max compression
+gzip compressed data, was "vnpy_tqsdk-3.4.0.tar", last modified: Sun Apr 23 01:09:50 2023, max compression
```

## Comparing `vnpy_tqsdk-3.2.11.tar` & `vnpy_tqsdk-3.4.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-08-05 14:22:05.669411 vnpy_tqsdk-3.2.11/
--rw-rw-rw-   0        0        0     1109 2021-09-24 04:39:57.000000 vnpy_tqsdk-3.2.11/LICENSE
--rw-rw-rw-   0        0        0     2419 2022-08-05 14:22:05.670463 vnpy_tqsdk-3.2.11/PKG-INFO
--rw-rw-rw-   0        0        0     1589 2022-08-05 14:20:37.000000 vnpy_tqsdk-3.2.11/README.md
--rw-rw-rw-   0        0        0      909 2022-08-05 14:22:05.712227 vnpy_tqsdk-3.2.11/setup.cfg
--rw-rw-rw-   0        0        0       43 2021-09-24 04:39:57.000000 vnpy_tqsdk-3.2.11/setup.py
-drwxrwxrwx   0        0        0        0 2022-08-05 14:22:05.595150 vnpy_tqsdk-3.2.11/vnpy_tqsdk/
--rw-rw-rw-   0        0        0     1379 2021-09-24 04:39:57.000000 vnpy_tqsdk-3.2.11/vnpy_tqsdk/__init__.py
--rw-rw-rw-   0        0        0     2442 2022-08-05 14:18:39.000000 vnpy_tqsdk-3.2.11/vnpy_tqsdk/tqsdk_datafeed.py
-drwxrwxrwx   0        0        0        0 2022-08-05 14:22:05.667365 vnpy_tqsdk-3.2.11/vnpy_tqsdk.egg-info/
--rw-rw-rw-   0        0        0     2419 2022-08-05 14:22:04.000000 vnpy_tqsdk-3.2.11/vnpy_tqsdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2022-08-05 14:22:05.000000 vnpy_tqsdk-3.2.11/vnpy_tqsdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-05 14:22:04.000000 vnpy_tqsdk-3.2.11/vnpy_tqsdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-08-05 14:22:04.000000 vnpy_tqsdk-3.2.11/vnpy_tqsdk.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        6 2022-08-05 14:22:04.000000 vnpy_tqsdk-3.2.11/vnpy_tqsdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2022-08-05 14:22:04.000000 vnpy_tqsdk-3.2.11/vnpy_tqsdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 01:09:50.907667 vnpy_tqsdk-3.4.0/
+-rw-rw-rw-   0        0        0     1109 2023-04-23 00:32:53.000000 vnpy_tqsdk-3.4.0/LICENSE
+-rw-rw-rw-   0        0        0     2407 2023-04-23 01:09:50.907667 vnpy_tqsdk-3.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1601 2023-04-23 00:36:21.000000 vnpy_tqsdk-3.4.0/README.md
+-rw-rw-rw-   0        0        0      908 2023-04-23 01:09:50.909743 vnpy_tqsdk-3.4.0/setup.cfg
+-rw-rw-rw-   0        0        0       43 2023-04-23 00:32:53.000000 vnpy_tqsdk-3.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 01:09:50.856476 vnpy_tqsdk-3.4.0/vnpy_tqsdk/
+-rw-rw-rw-   0        0        0     1379 2023-04-23 00:32:53.000000 vnpy_tqsdk-3.4.0/vnpy_tqsdk/__init__.py
+-rw-rw-rw-   0        0        0     2487 2023-04-23 00:33:35.000000 vnpy_tqsdk-3.4.0/vnpy_tqsdk/tqsdk_datafeed.py
+drwxrwxrwx   0        0        0        0 2023-04-23 01:09:50.906648 vnpy_tqsdk-3.4.0/vnpy_tqsdk.egg-info/
+-rw-rw-rw-   0        0        0     2407 2023-04-23 01:09:50.000000 vnpy_tqsdk-3.4.0/vnpy_tqsdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2023-04-23 01:09:50.000000 vnpy_tqsdk-3.4.0/vnpy_tqsdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 01:09:50.000000 vnpy_tqsdk-3.4.0/vnpy_tqsdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-23 01:09:50.000000 vnpy_tqsdk-3.4.0/vnpy_tqsdk.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        6 2023-04-23 01:09:50.000000 vnpy_tqsdk-3.4.0/vnpy_tqsdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-23 01:09:50.000000 vnpy_tqsdk-3.4.0/vnpy_tqsdk.egg-info/top_level.txt
```

### Comparing `vnpy_tqsdk-3.2.11/LICENSE` & `vnpy_tqsdk-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vnpy_tqsdk-3.2.11/PKG-INFO` & `vnpy_tqsdk-3.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: vnpy_tqsdk
-Version: 3.2.11
+Version: 3.4.0
 Summary: TQsdk datafeed for VeighNa quant trading framework.
 Home-page: https://www.vnpy.com
 Author: Xiaoyou Chen
 Author-email: xiaoyou.chen@mail.vnpy.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: License :: OSI Approved :: MIT License
@@ -22,17 +21,17 @@
 # VeighNa框架的天勤TQSDK数据服务接口
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-3.2.11-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-3.4.0-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
-    <img src ="https://img.shields.io/badge/python-3.7-blue.svg"/>
+    <img src ="https://img.shields.io/badge/python-3.7|3.8|3.9|3.10-blue.svg"/>
     <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
 </p>
 
 ## 说明
 
 基于天勤TQSDK模块的3.2.11版本开发，支持以下中国金融市场的K线数据：
 
@@ -72,9 +71,7 @@
 在VeighNa中使用天勤TQSDK时，需要在全局配置中填写以下字段信息：
 
 |名称|含义|必填|举例|
 |---------|----|---|---|
 |datafeed.name|名称|是|tqsdk|
 |datafeed.username|用户名|是|test|
 |datafeed.password|密码|是|12345678|
-
-
```

### Comparing `vnpy_tqsdk-3.2.11/README.md` & `vnpy_tqsdk-3.4.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # VeighNa框架的天勤TQSDK数据服务接口
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-3.2.11-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-3.4.0-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
-    <img src ="https://img.shields.io/badge/python-3.7-blue.svg"/>
+    <img src ="https://img.shields.io/badge/python-3.7|3.8|3.9|3.10-blue.svg"/>
     <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
 </p>
 
 ## 说明
 
 基于天勤TQSDK模块的3.2.11版本开发，支持以下中国金融市场的K线数据：
```

### Comparing `vnpy_tqsdk-3.2.11/setup.cfg` & `vnpy_tqsdk-3.4.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6e70 795f 7471 7364 6b0d 0a76   = vnpy_tqsdk..v
-00000020: 6572 7369 6f6e 203d 2033 2e32 2e31 310d  ersion = 3.2.11.
-00000030: 0a75 726c 203d 2068 7474 7073 3a2f 2f77  .url = https://w
-00000040: 7777 2e76 6e70 792e 636f 6d0d 0a6c 6963  ww.vnpy.com..lic
-00000050: 656e 7365 203d 204d 4954 0d0a 6175 7468  ense = MIT..auth
-00000060: 6f72 203d 2058 6961 6f79 6f75 2043 6865  or = Xiaoyou Che
-00000070: 6e0d 0a61 7574 686f 725f 656d 6169 6c20  n..author_email 
-00000080: 3d20 7869 616f 796f 752e 6368 656e 406d  = xiaoyou.chen@m
-00000090: 6169 6c2e 766e 7079 2e63 6f6d 0d0a 6465  ail.vnpy.com..de
-000000a0: 7363 7269 7074 696f 6e20 3d20 5451 7364  scription = TQsd
-000000b0: 6b20 6461 7461 6665 6564 2066 6f72 2056  k datafeed for V
-000000c0: 6569 6768 4e61 2071 7561 6e74 2074 7261  eighNa quant tra
-000000d0: 6469 6e67 2066 7261 6d65 776f 726b 2e0d  ding framework..
-000000e0: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
-000000f0: 6e20 3d20 6669 6c65 3a20 5245 4144 4d45  n = file: README
-00000100: 2e6d 640d 0a6c 6f6e 675f 6465 7363 7269  .md..long_descri
-00000110: 7074 696f 6e5f 636f 6e74 656e 745f 7479  ption_content_ty
-00000120: 7065 203d 2074 6578 742f 6d61 726b 646f  pe = text/markdo
-00000130: 776e 0d0a 6b65 7977 6f72 6473 203d 200d  wn..keywords = .
-00000140: 0a09 7175 616e 740d 0a09 7175 616e 7469  ..quant...quanti
-00000150: 7461 7469 7665 0d0a 0969 6e76 6573 746d  tative...investm
-00000160: 656e 740d 0a09 7472 6164 696e 670d 0a09  ent...trading...
-00000170: 616c 676f 7472 6164 696e 670d 0a63 6c61  algotrading..cla
-00000180: 7373 6966 6965 7273 203d 200d 0a09 4465  ssifiers = ...De
-00000190: 7665 6c6f 706d 656e 7420 5374 6174 7573  velopment Status
-000001a0: 203a 3a20 3520 2d20 5072 6f64 7563 7469   :: 5 - Producti
-000001b0: 6f6e 2f53 7461 626c 650d 0a09 4f70 6572  on/Stable...Oper
-000001c0: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
-000001d0: 4f53 2049 6e64 6570 656e 6465 6e74 0d0a  OS Independent..
-000001e0: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
-000001f0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-00000200: 3a3a 2033 0d0a 0950 726f 6772 616d 6d69  :: 3...Programmi
-00000210: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000220: 7974 686f 6e20 3a3a 2033 2e37 0d0a 0954  ython :: 3.7...T
-00000230: 6f70 6963 203a 3a20 4f66 6669 6365 2f42  opic :: Office/B
-00000240: 7573 696e 6573 7320 3a3a 2046 696e 616e  usiness :: Finan
-00000250: 6369 616c 203a 3a20 496e 7665 7374 6d65  cial :: Investme
-00000260: 6e74 0d0a 0950 726f 6772 616d 6d69 6e67  nt...Programming
-00000270: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000280: 686f 6e20 3a3a 2049 6d70 6c65 6d65 6e74  hon :: Implement
-00000290: 6174 696f 6e20 3a3a 2043 5079 7468 6f6e  ation :: CPython
-000002a0: 0d0a 094c 6963 656e 7365 203a 3a20 4f53  ...License :: OS
-000002b0: 4920 4170 7072 6f76 6564 203a 3a20 4d49  I Approved :: MI
-000002c0: 5420 4c69 6365 6e73 650d 0a09 4e61 7475  T License...Natu
-000002d0: 7261 6c20 4c61 6e67 7561 6765 203a 3a20  ral Language :: 
-000002e0: 4368 696e 6573 6520 2853 696d 706c 6966  Chinese (Simplif
-000002f0: 6965 6429 0d0a 0d0a 5b6f 7074 696f 6e73  ied)....[options
-00000300: 5d0d 0a70 6163 6b61 6765 7320 3d20 6669  ]..packages = fi
-00000310: 6e64 3a0d 0a69 6e63 6c75 6465 5f70 6163  nd:..include_pac
-00000320: 6b61 6765 5f64 6174 6120 3d20 5472 7565  kage_data = True
-00000330: 0d0a 7a69 705f 7361 6665 203d 2046 616c  ..zip_safe = Fal
-00000340: 7365 0d0a 696e 7374 616c 6c5f 7265 7175  se..install_requ
-00000350: 6972 6573 203d 200d 0a09 7471 7364 6b0d  ires = ...tqsdk.
-00000360: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
-00000370: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
-00000380: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
+00000020: 6572 7369 6f6e 203d 2033 2e34 2e30 0d0a  ersion = 3.4.0..
+00000030: 7572 6c20 3d20 6874 7470 733a 2f2f 7777  url = https://ww
+00000040: 772e 766e 7079 2e63 6f6d 0d0a 6c69 6365  w.vnpy.com..lice
+00000050: 6e73 6520 3d20 4d49 540d 0a61 7574 686f  nse = MIT..autho
+00000060: 7220 3d20 5869 616f 796f 7520 4368 656e  r = Xiaoyou Chen
+00000070: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
+00000080: 2078 6961 6f79 6f75 2e63 6865 6e40 6d61   xiaoyou.chen@ma
+00000090: 696c 2e76 6e70 792e 636f 6d0d 0a64 6573  il.vnpy.com..des
+000000a0: 6372 6970 7469 6f6e 203d 2054 5173 646b  cription = TQsdk
+000000b0: 2064 6174 6166 6565 6420 666f 7220 5665   datafeed for Ve
+000000c0: 6967 684e 6120 7175 616e 7420 7472 6164  ighNa quant trad
+000000d0: 696e 6720 6672 616d 6577 6f72 6b2e 0d0a  ing framework...
+000000e0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
+000000f0: 203d 2066 696c 653a 2052 4541 444d 452e   = file: README.
+00000100: 6d64 0d0a 6c6f 6e67 5f64 6573 6372 6970  md..long_descrip
+00000110: 7469 6f6e 5f63 6f6e 7465 6e74 5f74 7970  tion_content_typ
+00000120: 6520 3d20 7465 7874 2f6d 6172 6b64 6f77  e = text/markdow
+00000130: 6e0d 0a6b 6579 776f 7264 7320 3d20 0d0a  n..keywords = ..
+00000140: 0971 7561 6e74 0d0a 0971 7561 6e74 6974  .quant...quantit
+00000150: 6174 6976 650d 0a09 696e 7665 7374 6d65  ative...investme
+00000160: 6e74 0d0a 0974 7261 6469 6e67 0d0a 0961  nt...trading...a
+00000170: 6c67 6f74 7261 6469 6e67 0d0a 636c 6173  lgotrading..clas
+00000180: 7369 6669 6572 7320 3d20 0d0a 0944 6576  sifiers = ...Dev
+00000190: 656c 6f70 6d65 6e74 2053 7461 7475 7320  elopment Status 
+000001a0: 3a3a 2035 202d 2050 726f 6475 6374 696f  :: 5 - Productio
+000001b0: 6e2f 5374 6162 6c65 0d0a 094f 7065 7261  n/Stable...Opera
+000001c0: 7469 6e67 2053 7973 7465 6d20 3a3a 204f  ting System :: O
+000001d0: 5320 496e 6465 7065 6e64 656e 740d 0a09  S Independent...
+000001e0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+000001f0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000200: 3a20 330d 0a09 5072 6f67 7261 6d6d 696e  : 3...Programmin
+00000210: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000220: 7468 6f6e 203a 3a20 332e 370d 0a09 546f  thon :: 3.7...To
+00000230: 7069 6320 3a3a 204f 6666 6963 652f 4275  pic :: Office/Bu
+00000240: 7369 6e65 7373 203a 3a20 4669 6e61 6e63  siness :: Financ
+00000250: 6961 6c20 3a3a 2049 6e76 6573 746d 656e  ial :: Investmen
+00000260: 740d 0a09 5072 6f67 7261 6d6d 696e 6720  t...Programming 
+00000270: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000280: 6f6e 203a 3a20 496d 706c 656d 656e 7461  on :: Implementa
+00000290: 7469 6f6e 203a 3a20 4350 7974 686f 6e0d  tion :: CPython.
+000002a0: 0a09 4c69 6365 6e73 6520 3a3a 204f 5349  ..License :: OSI
+000002b0: 2041 7070 726f 7665 6420 3a3a 204d 4954   Approved :: MIT
+000002c0: 204c 6963 656e 7365 0d0a 094e 6174 7572   License...Natur
+000002d0: 616c 204c 616e 6775 6167 6520 3a3a 2043  al Language :: C
+000002e0: 6869 6e65 7365 2028 5369 6d70 6c69 6669  hinese (Simplifi
+000002f0: 6564 290d 0a0d 0a5b 6f70 7469 6f6e 735d  ed)....[options]
+00000300: 0d0a 7061 636b 6167 6573 203d 2066 696e  ..packages = fin
+00000310: 643a 0d0a 696e 636c 7564 655f 7061 636b  d:..include_pack
+00000320: 6167 655f 6461 7461 203d 2054 7275 650d  age_data = True.
+00000330: 0a7a 6970 5f73 6166 6520 3d20 4661 6c73  .zip_safe = Fals
+00000340: 650d 0a69 6e73 7461 6c6c 5f72 6571 7569  e..install_requi
+00000350: 7265 7320 3d20 0d0a 0974 7173 646b 0d0a  res = ...tqsdk..
+00000360: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
+00000370: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
+00000380: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
```

### Comparing `vnpy_tqsdk-3.2.11/vnpy_tqsdk/__init__.py` & `vnpy_tqsdk-3.4.0/vnpy_tqsdk/__init__.py`

 * *Files identical despite different names*

### Comparing `vnpy_tqsdk-3.2.11/vnpy_tqsdk/tqsdk_datafeed.py` & `vnpy_tqsdk-3.4.0/vnpy_tqsdk/tqsdk_datafeed.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import timedelta
-from typing import Dict, List, Optional
+from typing import Dict, List, Optional, Callable
 import traceback
 
 from pandas import DataFrame, Timestamp
 from tqsdk import TqApi, TqAuth
 
 from vnpy.trader.datafeed import BaseDatafeed
 from vnpy.trader.setting import SETTINGS
@@ -26,21 +26,21 @@
     """天勤TQsdk数据服务接口"""
 
     def __init__(self):
         """"""
         self.username: str = SETTINGS["datafeed.username"]
         self.password: str = SETTINGS["datafeed.password"]
 
-    def query_bar_history(self, req: HistoryRequest) -> Optional[List[BarData]]:
+    def query_bar_history(self, req: HistoryRequest, output: Callable = print) -> Optional[List[BarData]]:
         """查询k线数据"""
         # 初始化API
         try:
             api: TqApi = TqApi(auth=TqAuth(self.username, self.password))
         except Exception:
-            traceback.print_exc()
+            output(traceback.format_exc())
             return None
 
         # 查询数据
         tq_symbol: str = f"{req.exchange.value}.{req.symbol}"
 
         df: DataFrame = api.get_kline_data_series(
             symbol=tq_symbol,
```

### Comparing `vnpy_tqsdk-3.2.11/vnpy_tqsdk.egg-info/PKG-INFO` & `vnpy_tqsdk-3.4.0/vnpy_tqsdk.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: vnpy-tqsdk
-Version: 3.2.11
+Version: 3.4.0
 Summary: TQsdk datafeed for VeighNa quant trading framework.
 Home-page: https://www.vnpy.com
 Author: Xiaoyou Chen
 Author-email: xiaoyou.chen@mail.vnpy.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: License :: OSI Approved :: MIT License
@@ -22,17 +21,17 @@
 # VeighNa框架的天勤TQSDK数据服务接口
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-3.2.11-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-3.4.0-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
-    <img src ="https://img.shields.io/badge/python-3.7-blue.svg"/>
+    <img src ="https://img.shields.io/badge/python-3.7|3.8|3.9|3.10-blue.svg"/>
     <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
 </p>
 
 ## 说明
 
 基于天勤TQSDK模块的3.2.11版本开发，支持以下中国金融市场的K线数据：
 
@@ -72,9 +71,7 @@
 在VeighNa中使用天勤TQSDK时，需要在全局配置中填写以下字段信息：
 
 |名称|含义|必填|举例|
 |---------|----|---|---|
 |datafeed.name|名称|是|tqsdk|
 |datafeed.username|用户名|是|test|
 |datafeed.password|密码|是|12345678|
-
-
```

