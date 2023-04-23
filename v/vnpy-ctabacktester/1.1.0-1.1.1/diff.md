# Comparing `tmp/vnpy_ctabacktester-1.1.0.tar.gz` & `tmp/vnpy_ctabacktester-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnpy_ctabacktester-1.1.0.tar", last modified: Wed Feb 15 14:42:45 2023, max compression
+gzip compressed data, was "vnpy_ctabacktester-1.1.1.tar", last modified: Sun Apr 23 01:56:33 2023, max compression
```

## Comparing `vnpy_ctabacktester-1.1.0.tar` & `vnpy_ctabacktester-1.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-02-15 14:42:45.785557 vnpy_ctabacktester-1.1.0/
--rw-rw-rw-   0        0        0     1107 2023-02-12 12:41:06.000000 vnpy_ctabacktester-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     1967 2023-02-15 14:42:45.785557 vnpy_ctabacktester-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      930 2023-02-15 14:42:21.000000 vnpy_ctabacktester-1.1.0/README.md
--rw-rw-rw-   0        0        0     1103 2023-02-15 14:42:45.793555 vnpy_ctabacktester-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0       43 2023-02-12 12:41:06.000000 vnpy_ctabacktester-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-15 14:42:45.718032 vnpy_ctabacktester-1.1.0/vnpy_ctabacktester/
--rw-rw-rw-   0        0        0     1810 2023-02-12 12:41:06.000000 vnpy_ctabacktester-1.1.0/vnpy_ctabacktester/__init__.py
--rw-rw-rw-   0        0        0    14249 2023-02-13 09:40:22.000000 vnpy_ctabacktester-1.1.0/vnpy_ctabacktester/engine.py
-drwxrwxrwx   0        0        0        0 2023-02-15 14:42:45.776553 vnpy_ctabacktester-1.1.0/vnpy_ctabacktester/ui/
--rw-rw-rw-   0        0        0       39 2023-02-12 12:41:06.000000 vnpy_ctabacktester-1.1.0/vnpy_ctabacktester/ui/__init__.py
--rw-rw-rw-   0        0        0    64478 2023-02-12 12:41:06.000000 vnpy_ctabacktester-1.1.0/vnpy_ctabacktester/ui/backtester.ico
--rw-rw-rw-   0        0        0    50745 2023-02-13 09:38:58.000000 vnpy_ctabacktester-1.1.0/vnpy_ctabacktester/ui/widget.py
-drwxrwxrwx   0        0        0        0 2023-02-15 14:42:45.754545 vnpy_ctabacktester-1.1.0/vnpy_ctabacktester.egg-info/
--rw-rw-rw-   0        0        0     1967 2023-02-15 14:42:45.000000 vnpy_ctabacktester-1.1.0/vnpy_ctabacktester.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      449 2023-02-15 14:42:45.000000 vnpy_ctabacktester-1.1.0/vnpy_ctabacktester.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-15 14:42:45.000000 vnpy_ctabacktester-1.1.0/vnpy_ctabacktester.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-02-15 14:42:45.000000 vnpy_ctabacktester-1.1.0/vnpy_ctabacktester.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       17 2023-02-15 14:42:45.000000 vnpy_ctabacktester-1.1.0/vnpy_ctabacktester.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-02-15 14:42:45.000000 vnpy_ctabacktester-1.1.0/vnpy_ctabacktester.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 01:56:33.429695 vnpy_ctabacktester-1.1.1/
+-rw-rw-rw-   0        0        0     1107 2023-02-12 12:41:06.000000 vnpy_ctabacktester-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1967 2023-04-23 01:56:33.429695 vnpy_ctabacktester-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      930 2023-04-23 01:55:55.000000 vnpy_ctabacktester-1.1.1/README.md
+-rw-rw-rw-   0        0        0     1103 2023-04-23 01:56:33.432700 vnpy_ctabacktester-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0       43 2023-02-12 12:41:06.000000 vnpy_ctabacktester-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 01:56:33.368198 vnpy_ctabacktester-1.1.1/vnpy_ctabacktester/
+-rw-rw-rw-   0        0        0     1810 2023-02-12 12:41:06.000000 vnpy_ctabacktester-1.1.1/vnpy_ctabacktester/__init__.py
+-rw-rw-rw-   0        0        0    14371 2023-04-23 01:52:02.000000 vnpy_ctabacktester-1.1.1/vnpy_ctabacktester/engine.py
+drwxrwxrwx   0        0        0        0 2023-04-23 01:56:33.424692 vnpy_ctabacktester-1.1.1/vnpy_ctabacktester/ui/
+-rw-rw-rw-   0        0        0       39 2023-02-12 12:41:06.000000 vnpy_ctabacktester-1.1.1/vnpy_ctabacktester/ui/__init__.py
+-rw-rw-rw-   0        0        0    64478 2023-02-12 12:41:06.000000 vnpy_ctabacktester-1.1.1/vnpy_ctabacktester/ui/backtester.ico
+-rw-rw-rw-   0        0        0    50745 2023-02-13 09:38:58.000000 vnpy_ctabacktester-1.1.1/vnpy_ctabacktester/ui/widget.py
+drwxrwxrwx   0        0        0        0 2023-04-23 01:56:33.412786 vnpy_ctabacktester-1.1.1/vnpy_ctabacktester.egg-info/
+-rw-rw-rw-   0        0        0     1967 2023-04-23 01:56:33.000000 vnpy_ctabacktester-1.1.1/vnpy_ctabacktester.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      449 2023-04-23 01:56:33.000000 vnpy_ctabacktester-1.1.1/vnpy_ctabacktester.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 01:56:33.000000 vnpy_ctabacktester-1.1.1/vnpy_ctabacktester.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-23 01:56:33.000000 vnpy_ctabacktester-1.1.1/vnpy_ctabacktester.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       17 2023-04-23 01:56:33.000000 vnpy_ctabacktester-1.1.1/vnpy_ctabacktester.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-23 01:56:33.000000 vnpy_ctabacktester-1.1.1/vnpy_ctabacktester.egg-info/top_level.txt
```

### Comparing `vnpy_ctabacktester-1.1.0/LICENSE` & `vnpy_ctabacktester-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vnpy_ctabacktester-1.1.0/PKG-INFO` & `vnpy_ctabacktester-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnpy_ctabacktester
-Version: 1.1.0
+Version: 1.1.1
 Summary: CTA strategy backtesting application for VeighNa quant trading framework.
 Home-page: https://www.vnpy.com
 Author: Xiaoyou Chen
 Author-email: xiaoyou.chen@mail.vnpy.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
 Platform: UNKNOWN
@@ -26,15 +26,15 @@
 # VeighNa框架的CTA投研模块
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-1.1.0-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-1.1.1-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
     <img src ="https://img.shields.io/badge/python-3.7|3.8|3.9|3.10-blue.svg" />
     <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
 </p>
 
 ## 说明
```

### Comparing `vnpy_ctabacktester-1.1.0/README.md` & `vnpy_ctabacktester-1.1.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # VeighNa框架的CTA投研模块
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-1.1.0-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-1.1.1-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
     <img src ="https://img.shields.io/badge/python-3.7|3.8|3.9|3.10-blue.svg" />
     <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
 </p>
 
 ## 说明
```

### Comparing `vnpy_ctabacktester-1.1.0/setup.cfg` & `vnpy_ctabacktester-1.1.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6e70 795f 6374 6162 6163 6b74   = vnpy_ctabackt
 00000020: 6573 7465 720d 0a76 6572 7369 6f6e 203d  ester..version =
-00000030: 2031 2e31 2e30 0d0a 7572 6c20 3d20 6874   1.1.0..url = ht
+00000030: 2031 2e31 2e31 0d0a 7572 6c20 3d20 6874   1.1.1..url = ht
 00000040: 7470 733a 2f2f 7777 772e 766e 7079 2e63  tps://www.vnpy.c
 00000050: 6f6d 0d0a 6c69 6365 6e73 6520 3d20 4d49  om..license = MI
 00000060: 540d 0a61 7574 686f 7220 3d20 5869 616f  T..author = Xiao
 00000070: 796f 7520 4368 656e 0d0a 6175 7468 6f72  you Chen..author
 00000080: 5f65 6d61 696c 203d 2078 6961 6f79 6f75  _email = xiaoyou
 00000090: 2e63 6865 6e40 6d61 696c 2e76 6e70 792e  .chen@mail.vnpy.
 000000a0: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
```

### Comparing `vnpy_ctabacktester-1.1.0/vnpy_ctabacktester/__init__.py` & `vnpy_ctabacktester-1.1.1/vnpy_ctabacktester/__init__.py`

 * *Files identical despite different names*

### Comparing `vnpy_ctabacktester-1.1.0/vnpy_ctabacktester/engine.py` & `vnpy_ctabacktester-1.1.1/vnpy_ctabacktester/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from vnpy.trader.constant import Interval
 from vnpy.trader.utility import extract_vt_symbol
 from vnpy.trader.object import HistoryRequest, TickData, ContractData, BarData
 from vnpy.trader.datafeed import BaseDatafeed, get_datafeed
 from vnpy.trader.database import BaseDatabase, get_database
 
 import vnpy_ctastrategy
-from vnpy_ctastrategy import CtaTemplate
+from vnpy_ctastrategy import CtaTemplate, TargetPosTemplate
 from vnpy_ctastrategy.backtesting import (
     BacktestingEngine,
     OptimizationSetting,
     BacktestingMode
 )
 
 
@@ -114,15 +114,19 @@
             module: ModuleType = importlib.import_module(module_name)
 
             # 重载模块，确保如果策略文件中有任何修改，能够立即生效。
             importlib.reload(module)
 
             for name in dir(module):
                 value = getattr(module, name)
-                if (isinstance(value, type) and issubclass(value, CtaTemplate) and value is not CtaTemplate):
+                if (
+                    isinstance(value, type)
+                    and issubclass(value, CtaTemplate)
+                    and value not in {CtaTemplate, TargetPosTemplate}
+                ):
                     self.classes[value.__name__] = value
         except:  # noqa
             msg: str = f"策略文件{module_name}加载失败，触发异常：\n{traceback.format_exc()}"
             self.write_log(msg)
 
     def reload_strategy_class(self) -> None:
         """"""
```

### Comparing `vnpy_ctabacktester-1.1.0/vnpy_ctabacktester/ui/backtester.ico` & `vnpy_ctabacktester-1.1.1/vnpy_ctabacktester/ui/backtester.ico`

 * *Files identical despite different names*

### Comparing `vnpy_ctabacktester-1.1.0/vnpy_ctabacktester/ui/widget.py` & `vnpy_ctabacktester-1.1.1/vnpy_ctabacktester/ui/widget.py`

 * *Files identical despite different names*

### Comparing `vnpy_ctabacktester-1.1.0/vnpy_ctabacktester.egg-info/PKG-INFO` & `vnpy_ctabacktester-1.1.1/vnpy_ctabacktester.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnpy-ctabacktester
-Version: 1.1.0
+Version: 1.1.1
 Summary: CTA strategy backtesting application for VeighNa quant trading framework.
 Home-page: https://www.vnpy.com
 Author: Xiaoyou Chen
 Author-email: xiaoyou.chen@mail.vnpy.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
 Platform: UNKNOWN
@@ -26,15 +26,15 @@
 # VeighNa框架的CTA投研模块
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-1.1.0-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-1.1.1-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
     <img src ="https://img.shields.io/badge/python-3.7|3.8|3.9|3.10-blue.svg" />
     <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
 </p>
 
 ## 说明
```

