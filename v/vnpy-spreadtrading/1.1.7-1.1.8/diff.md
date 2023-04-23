# Comparing `tmp/vnpy_spreadtrading-1.1.7.tar.gz` & `tmp/vnpy_spreadtrading-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnpy_spreadtrading-1.1.7.tar", last modified: Thu Feb 16 03:16:06 2023, max compression
+gzip compressed data, was "vnpy_spreadtrading-1.1.8.tar", last modified: Sun Apr 23 04:36:18 2023, max compression
```

## Comparing `vnpy_spreadtrading-1.1.7.tar` & `vnpy_spreadtrading-1.1.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-02-16 03:16:06.010125 vnpy_spreadtrading-1.1.7/
--rw-rw-rw-   0        0        0     1107 2023-02-14 07:58:27.000000 vnpy_spreadtrading-1.1.7/LICENSE
--rw-rw-rw-   0        0        0     2020 2023-02-16 03:16:06.010125 vnpy_spreadtrading-1.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     1016 2023-02-16 03:14:41.000000 vnpy_spreadtrading-1.1.7/README.md
--rw-rw-rw-   0        0        0     1100 2023-02-16 03:16:06.012174 vnpy_spreadtrading-1.1.7/setup.cfg
--rw-rw-rw-   0        0        0       43 2023-02-14 07:58:27.000000 vnpy_spreadtrading-1.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-16 03:16:05.731247 vnpy_spreadtrading-1.1.7/vnpy_spreadtrading/
--rw-rw-rw-   0        0        0     1988 2023-02-14 07:58:27.000000 vnpy_spreadtrading-1.1.7/vnpy_spreadtrading/__init__.py
--rw-rw-rw-   0        0        0     5773 2023-02-14 07:58:27.000000 vnpy_spreadtrading-1.1.7/vnpy_spreadtrading/algo.py
--rw-rw-rw-   0        0        0    26280 2023-02-15 01:24:14.000000 vnpy_spreadtrading-1.1.7/vnpy_spreadtrading/backtesting.py
--rw-rw-rw-   0        0        0    16979 2023-02-14 07:59:35.000000 vnpy_spreadtrading-1.1.7/vnpy_spreadtrading/base.py
--rw-rw-rw-   0        0        0    35634 2023-02-16 00:38:43.000000 vnpy_spreadtrading-1.1.7/vnpy_spreadtrading/engine.py
-drwxrwxrwx   0        0        0        0 2023-02-16 03:16:06.005006 vnpy_spreadtrading-1.1.7/vnpy_spreadtrading/strategies/
--rw-rw-rw-   0        0        0        0 2023-02-14 07:58:27.000000 vnpy_spreadtrading-1.1.7/vnpy_spreadtrading/strategies/__init__.py
--rw-rw-rw-   0        0        0     5102 2023-02-14 07:58:27.000000 vnpy_spreadtrading-1.1.7/vnpy_spreadtrading/strategies/basic_spread_strategy.py
--rw-rw-rw-   0        0        0     4556 2023-02-14 07:58:27.000000 vnpy_spreadtrading-1.1.7/vnpy_spreadtrading/strategies/statistical_arbitrage_strategy.py
--rw-rw-rw-   0        0        0    22457 2023-02-14 07:58:27.000000 vnpy_spreadtrading-1.1.7/vnpy_spreadtrading/template.py
-drwxrwxrwx   0        0        0        0 2023-02-16 03:16:06.009083 vnpy_spreadtrading-1.1.7/vnpy_spreadtrading/ui/
--rw-rw-rw-   0        0        0       35 2023-02-14 07:58:27.000000 vnpy_spreadtrading-1.1.7/vnpy_spreadtrading/ui/__init__.py
--rw-rw-rw-   0        0        0    67646 2023-02-14 07:58:27.000000 vnpy_spreadtrading-1.1.7/vnpy_spreadtrading/ui/spread.ico
--rw-rw-rw-   0        0        0    29116 2023-02-14 07:58:27.000000 vnpy_spreadtrading-1.1.7/vnpy_spreadtrading/ui/widget.py
-drwxrwxrwx   0        0        0        0 2023-02-16 03:16:05.939100 vnpy_spreadtrading-1.1.7/vnpy_spreadtrading.egg-info/
--rw-rw-rw-   0        0        0     2020 2023-02-16 03:16:05.000000 vnpy_spreadtrading-1.1.7/vnpy_spreadtrading.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      725 2023-02-16 03:16:05.000000 vnpy_spreadtrading-1.1.7/vnpy_spreadtrading.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-16 03:16:05.000000 vnpy_spreadtrading-1.1.7/vnpy_spreadtrading.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-02-16 03:16:05.000000 vnpy_spreadtrading-1.1.7/vnpy_spreadtrading.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       20 2023-02-16 03:16:05.000000 vnpy_spreadtrading-1.1.7/vnpy_spreadtrading.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-02-16 03:16:05.000000 vnpy_spreadtrading-1.1.7/vnpy_spreadtrading.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 04:36:18.563910 vnpy_spreadtrading-1.1.8/
+-rw-rw-rw-   0        0        0     1107 2023-02-14 07:58:27.000000 vnpy_spreadtrading-1.1.8/LICENSE
+-rw-rw-rw-   0        0        0     2020 2023-04-23 04:36:18.563910 vnpy_spreadtrading-1.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1016 2023-04-23 04:35:29.000000 vnpy_spreadtrading-1.1.8/README.md
+-rw-rw-rw-   0        0        0     1100 2023-04-23 04:36:18.565956 vnpy_spreadtrading-1.1.8/setup.cfg
+-rw-rw-rw-   0        0        0       43 2023-02-14 07:58:27.000000 vnpy_spreadtrading-1.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 04:36:18.496542 vnpy_spreadtrading-1.1.8/vnpy_spreadtrading/
+-rw-rw-rw-   0        0        0     1988 2023-02-14 07:58:27.000000 vnpy_spreadtrading-1.1.8/vnpy_spreadtrading/__init__.py
+-rw-rw-rw-   0        0        0     5773 2023-02-14 07:58:27.000000 vnpy_spreadtrading-1.1.8/vnpy_spreadtrading/algo.py
+-rw-rw-rw-   0        0        0    26351 2023-03-27 06:55:55.000000 vnpy_spreadtrading-1.1.8/vnpy_spreadtrading/backtesting.py
+-rw-rw-rw-   0        0        0    17129 2023-03-27 06:55:11.000000 vnpy_spreadtrading-1.1.8/vnpy_spreadtrading/base.py
+-rw-rw-rw-   0        0        0    35634 2023-02-16 00:38:43.000000 vnpy_spreadtrading-1.1.8/vnpy_spreadtrading/engine.py
+drwxrwxrwx   0        0        0        0 2023-04-23 04:36:18.559289 vnpy_spreadtrading-1.1.8/vnpy_spreadtrading/strategies/
+-rw-rw-rw-   0        0        0        0 2023-02-14 07:58:27.000000 vnpy_spreadtrading-1.1.8/vnpy_spreadtrading/strategies/__init__.py
+-rw-rw-rw-   0        0        0     5102 2023-02-14 07:58:27.000000 vnpy_spreadtrading-1.1.8/vnpy_spreadtrading/strategies/basic_spread_strategy.py
+-rw-rw-rw-   0        0        0     4556 2023-02-14 07:58:27.000000 vnpy_spreadtrading-1.1.8/vnpy_spreadtrading/strategies/statistical_arbitrage_strategy.py
+-rw-rw-rw-   0        0        0    22457 2023-02-14 07:58:27.000000 vnpy_spreadtrading-1.1.8/vnpy_spreadtrading/template.py
+drwxrwxrwx   0        0        0        0 2023-04-23 04:36:18.562889 vnpy_spreadtrading-1.1.8/vnpy_spreadtrading/ui/
+-rw-rw-rw-   0        0        0       35 2023-02-14 07:58:27.000000 vnpy_spreadtrading-1.1.8/vnpy_spreadtrading/ui/__init__.py
+-rw-rw-rw-   0        0        0    67646 2023-02-14 07:58:27.000000 vnpy_spreadtrading-1.1.8/vnpy_spreadtrading/ui/spread.ico
+-rw-rw-rw-   0        0        0    29116 2023-02-14 07:58:27.000000 vnpy_spreadtrading-1.1.8/vnpy_spreadtrading/ui/widget.py
+drwxrwxrwx   0        0        0        0 2023-04-23 04:36:18.553134 vnpy_spreadtrading-1.1.8/vnpy_spreadtrading.egg-info/
+-rw-rw-rw-   0        0        0     2020 2023-04-23 04:36:18.000000 vnpy_spreadtrading-1.1.8/vnpy_spreadtrading.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      725 2023-04-23 04:36:18.000000 vnpy_spreadtrading-1.1.8/vnpy_spreadtrading.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 04:36:18.000000 vnpy_spreadtrading-1.1.8/vnpy_spreadtrading.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-23 04:36:18.000000 vnpy_spreadtrading-1.1.8/vnpy_spreadtrading.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       20 2023-04-23 04:36:18.000000 vnpy_spreadtrading-1.1.8/vnpy_spreadtrading.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-23 04:36:18.000000 vnpy_spreadtrading-1.1.8/vnpy_spreadtrading.egg-info/top_level.txt
```

### Comparing `vnpy_spreadtrading-1.1.7/LICENSE` & `vnpy_spreadtrading-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `vnpy_spreadtrading-1.1.7/PKG-INFO` & `vnpy_spreadtrading-1.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnpy_spreadtrading
-Version: 1.1.7
+Version: 1.1.8
 Summary: Spread trading application for VeighNa quant trading framework.
 Home-page: https://www.vnpy.com
 Author: Xiaoyou Chen
 Author-email: xiaoyou.chen@mail.vnpy.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
 Classifier: Development Status :: 5 - Production/Stable
@@ -25,15 +25,15 @@
 # VeighNa框架的价差交易模块
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-1.1.7-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-1.1.8-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
     <img src ="https://img.shields.io/badge/python-3.7|3.8|3.9|3.10-blue.svg" />
     <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
 </p>
 
 ## 说明
```

### Comparing `vnpy_spreadtrading-1.1.7/README.md` & `vnpy_spreadtrading-1.1.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # VeighNa框架的价差交易模块
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-1.1.7-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-1.1.8-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
     <img src ="https://img.shields.io/badge/python-3.7|3.8|3.9|3.10-blue.svg" />
     <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
 </p>
 
 ## 说明
```

### Comparing `vnpy_spreadtrading-1.1.7/setup.cfg` & `vnpy_spreadtrading-1.1.8/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6e70 795f 7370 7265 6164 7472   = vnpy_spreadtr
 00000020: 6164 696e 670d 0a76 6572 7369 6f6e 203d  ading..version =
-00000030: 2031 2e31 2e37 0d0a 7572 6c20 3d20 6874   1.1.7..url = ht
+00000030: 2031 2e31 2e38 0d0a 7572 6c20 3d20 6874   1.1.8..url = ht
 00000040: 7470 733a 2f2f 7777 772e 766e 7079 2e63  tps://www.vnpy.c
 00000050: 6f6d 0d0a 6c69 6365 6e73 6520 3d20 4d49  om..license = MI
 00000060: 540d 0a61 7574 686f 7220 3d20 5869 616f  T..author = Xiao
 00000070: 796f 7520 4368 656e 0d0a 6175 7468 6f72  you Chen..author
 00000080: 5f65 6d61 696c 203d 2078 6961 6f79 6f75  _email = xiaoyou
 00000090: 2e63 6865 6e40 6d61 696c 2e76 6e70 792e  .chen@mail.vnpy.
 000000a0: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
```

### Comparing `vnpy_spreadtrading-1.1.7/vnpy_spreadtrading/__init__.py` & `vnpy_spreadtrading-1.1.8/vnpy_spreadtrading/__init__.py`

 * *Files identical despite different names*

### Comparing `vnpy_spreadtrading-1.1.7/vnpy_spreadtrading/algo.py` & `vnpy_spreadtrading-1.1.8/vnpy_spreadtrading/algo.py`

 * *Files identical despite different names*

### Comparing `vnpy_spreadtrading-1.1.7/vnpy_spreadtrading/backtesting.py` & `vnpy_spreadtrading-1.1.8/vnpy_spreadtrading/backtesting.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,19 +138,20 @@
 
         if self.start >= self.end:
             self.output("起始日期必须小于结束日期")
             return
 
         if self.mode == BacktestingMode.BAR:
             self.history_data = load_bar_data(
-                self.spread,
-                self.interval,
-                self.start,
-                self.end,
-                self.pricetick
+                spread=self.spread,
+                interval=self.interval,
+                start=self.start,
+                end=self.end,
+                pricetick=self.pricetick,
+                backtesting=True
             )
         else:
             self.history_data = load_tick_data(
                 self.spread,
                 self.start,
                 self.end
             )
```

### Comparing `vnpy_spreadtrading-1.1.7/vnpy_spreadtrading/base.py` & `vnpy_spreadtrading-1.1.8/vnpy_spreadtrading/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -394,31 +394,36 @@
 
 def load_bar_data(
     spread: SpreadData,
     interval: Interval,
     start: datetime,
     end: datetime,
     pricetick: float = 0,
-    output: Callable = print
+    output: Callable = print,
+    backtesting: bool = False
 ) -> List[BarData]:
     """"""
     database: BaseDatabase = get_database()
 
     # Load bar data of each spread leg
     leg_bars: Dict[str, Dict] = {}
 
     for vt_symbol in spread.legs.keys():
         symbol, exchange = extract_vt_symbol(vt_symbol)
 
-        # First, try to query history from datafeed
-        bar_data: List[BarData] = query_bar_from_datafeed(
-            symbol, exchange, interval, start, end, output
-        )
+        # 初始化K线列表
+        bar_data: List[BarData] = [] 
 
-        # If failed, query history from database
+        # 只有实盘才优先尝试从数据服务查询
+        if not backtesting:
+            bar_data = query_bar_from_datafeed(
+                symbol, exchange, interval, start, end, output
+            )
+
+        # 如果查询失败，则尝试从数据库中读取
         if not bar_data:
             bar_data = database.load_bar_data(
                 symbol, exchange, interval, start, end
             )
 
         bars: Dict[datetime, BarData] = {bar.datetime: bar for bar in bar_data}
         leg_bars[vt_symbol] = bars
```

### Comparing `vnpy_spreadtrading-1.1.7/vnpy_spreadtrading/engine.py` & `vnpy_spreadtrading-1.1.8/vnpy_spreadtrading/engine.py`

 * *Files identical despite different names*

### Comparing `vnpy_spreadtrading-1.1.7/vnpy_spreadtrading/strategies/basic_spread_strategy.py` & `vnpy_spreadtrading-1.1.8/vnpy_spreadtrading/strategies/basic_spread_strategy.py`

 * *Files identical despite different names*

### Comparing `vnpy_spreadtrading-1.1.7/vnpy_spreadtrading/strategies/statistical_arbitrage_strategy.py` & `vnpy_spreadtrading-1.1.8/vnpy_spreadtrading/strategies/statistical_arbitrage_strategy.py`

 * *Files identical despite different names*

### Comparing `vnpy_spreadtrading-1.1.7/vnpy_spreadtrading/template.py` & `vnpy_spreadtrading-1.1.8/vnpy_spreadtrading/template.py`

 * *Files identical despite different names*

### Comparing `vnpy_spreadtrading-1.1.7/vnpy_spreadtrading/ui/spread.ico` & `vnpy_spreadtrading-1.1.8/vnpy_spreadtrading/ui/spread.ico`

 * *Files identical despite different names*

### Comparing `vnpy_spreadtrading-1.1.7/vnpy_spreadtrading/ui/widget.py` & `vnpy_spreadtrading-1.1.8/vnpy_spreadtrading/ui/widget.py`

 * *Files identical despite different names*

### Comparing `vnpy_spreadtrading-1.1.7/vnpy_spreadtrading.egg-info/PKG-INFO` & `vnpy_spreadtrading-1.1.8/vnpy_spreadtrading.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnpy-spreadtrading
-Version: 1.1.7
+Version: 1.1.8
 Summary: Spread trading application for VeighNa quant trading framework.
 Home-page: https://www.vnpy.com
 Author: Xiaoyou Chen
 Author-email: xiaoyou.chen@mail.vnpy.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
 Classifier: Development Status :: 5 - Production/Stable
@@ -25,15 +25,15 @@
 # VeighNa框架的价差交易模块
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-1.1.7-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-1.1.8-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
     <img src ="https://img.shields.io/badge/python-3.7|3.8|3.9|3.10-blue.svg" />
     <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
 </p>
 
 ## 说明
```

### Comparing `vnpy_spreadtrading-1.1.7/vnpy_spreadtrading.egg-info/SOURCES.txt` & `vnpy_spreadtrading-1.1.8/vnpy_spreadtrading.egg-info/SOURCES.txt`

 * *Files identical despite different names*

