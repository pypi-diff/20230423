# Comparing `tmp/vnpy_ctastrategy-1.1.3.tar.gz` & `tmp/vnpy_ctastrategy-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnpy_ctastrategy-1.1.3.tar", last modified: Wed Feb 15 14:36:06 2023, max compression
+gzip compressed data, was "vnpy_ctastrategy-1.1.4.tar", last modified: Sun Apr 23 03:38:22 2023, max compression
```

## Comparing `vnpy_ctastrategy-1.1.3.tar` & `vnpy_ctastrategy-1.1.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-02-15 14:36:06.950927 vnpy_ctastrategy-1.1.3/
--rw-rw-rw-   0        0        0     1107 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.3/LICENSE
--rw-rw-rw-   0        0        0     1969 2023-02-15 14:36:06.951933 vnpy_ctastrategy-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      946 2023-02-15 14:35:06.000000 vnpy_ctastrategy-1.1.3/README.md
--rw-rw-rw-   0        0        0     1088 2023-02-15 14:36:06.955927 vnpy_ctastrategy-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0       43 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-15 14:36:06.819334 vnpy_ctastrategy-1.1.3/vnpy_ctastrategy/
--rw-rw-rw-   0        0        0     2041 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.3/vnpy_ctastrategy/__init__.py
--rw-rw-rw-   0        0        0    37582 2023-02-13 09:22:23.000000 vnpy_ctastrategy-1.1.3/vnpy_ctastrategy/backtesting.py
--rw-rw-rw-   0        0        0     1274 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.3/vnpy_ctastrategy/base.py
--rw-rw-rw-   0        0        0    32542 2023-02-12 12:59:25.000000 vnpy_ctastrategy-1.1.3/vnpy_ctastrategy/engine.py
-drwxrwxrwx   0        0        0        0 2023-02-15 14:36:06.910934 vnpy_ctastrategy-1.1.3/vnpy_ctastrategy/strategies/
--rw-rw-rw-   0        0        0        0 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.3/vnpy_ctastrategy/strategies/__init__.py
--rw-rw-rw-   0        0        0     3764 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.3/vnpy_ctastrategy/strategies/atr_rsi_strategy.py
--rw-rw-rw-   0        0        0     3701 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.3/vnpy_ctastrategy/strategies/boll_channel_strategy.py
--rw-rw-rw-   0        0        0     2919 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.3/vnpy_ctastrategy/strategies/double_ma_strategy.py
--rw-rw-rw-   0        0        0     4192 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.3/vnpy_ctastrategy/strategies/dual_thrust_strategy.py
--rw-rw-rw-   0        0        0     4185 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.3/vnpy_ctastrategy/strategies/king_keltner_strategy.py
--rw-rw-rw-   0        0        0     6118 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.3/vnpy_ctastrategy/strategies/multi_signal_strategy.py
--rw-rw-rw-   0        0        0     3667 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.3/vnpy_ctastrategy/strategies/multi_timeframe_strategy.py
--rw-rw-rw-   0        0        0     3044 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.3/vnpy_ctastrategy/strategies/test_strategy.py
--rw-rw-rw-   0        0        0     4381 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.3/vnpy_ctastrategy/strategies/turtle_signal_strategy.py
--rw-rw-rw-   0        0        0    13503 2023-01-06 11:08:07.000000 vnpy_ctastrategy-1.1.3/vnpy_ctastrategy/template.py
-drwxrwxrwx   0        0        0        0 2023-02-15 14:36:06.940933 vnpy_ctastrategy-1.1.3/vnpy_ctastrategy/ui/
--rw-rw-rw-   0        0        0       32 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.3/vnpy_ctastrategy/ui/__init__.py
--rw-rw-rw-   0        0        0    67646 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.3/vnpy_ctastrategy/ui/cta.ico
--rw-rw-rw-   0        0        0     9024 2023-02-10 06:05:33.000000 vnpy_ctastrategy-1.1.3/vnpy_ctastrategy/ui/rollover.py
--rw-rw-rw-   0        0        0    17453 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.3/vnpy_ctastrategy/ui/widget.py
-drwxrwxrwx   0        0        0        0 2023-02-15 14:36:06.851333 vnpy_ctastrategy-1.1.3/vnpy_ctastrategy.egg-info/
--rw-rw-rw-   0        0        0     1969 2023-02-15 14:36:06.000000 vnpy_ctastrategy-1.1.3/vnpy_ctastrategy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1042 2023-02-15 14:36:06.000000 vnpy_ctastrategy-1.1.3/vnpy_ctastrategy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-15 14:36:06.000000 vnpy_ctastrategy-1.1.3/vnpy_ctastrategy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-02-15 14:36:06.000000 vnpy_ctastrategy-1.1.3/vnpy_ctastrategy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       14 2023-02-15 14:36:06.000000 vnpy_ctastrategy-1.1.3/vnpy_ctastrategy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-02-15 14:36:06.000000 vnpy_ctastrategy-1.1.3/vnpy_ctastrategy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 03:38:22.392650 vnpy_ctastrategy-1.1.4/
+-rw-rw-rw-   0        0        0     1107 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.4/LICENSE
+-rw-rw-rw-   0        0        0     1969 2023-04-23 03:38:22.392650 vnpy_ctastrategy-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      946 2023-04-23 03:37:50.000000 vnpy_ctastrategy-1.1.4/README.md
+-rw-rw-rw-   0        0        0     1088 2023-04-23 03:38:22.395653 vnpy_ctastrategy-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0       43 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:38:22.296113 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/
+-rw-rw-rw-   0        0        0     2072 2023-04-23 02:03:30.000000 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/__init__.py
+-rw-rw-rw-   0        0        0    37582 2023-02-13 09:22:23.000000 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/backtesting.py
+-rw-rw-rw-   0        0        0     1274 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/base.py
+-rw-rw-rw-   0        0        0    32778 2023-04-23 02:01:58.000000 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/engine.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:38:22.375373 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/strategies/
+-rw-rw-rw-   0        0        0        0 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/strategies/__init__.py
+-rw-rw-rw-   0        0        0     3764 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/strategies/atr_rsi_strategy.py
+-rw-rw-rw-   0        0        0     3701 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/strategies/boll_channel_strategy.py
+-rw-rw-rw-   0        0        0     2919 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/strategies/double_ma_strategy.py
+-rw-rw-rw-   0        0        0     4192 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/strategies/dual_thrust_strategy.py
+-rw-rw-rw-   0        0        0     4185 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/strategies/king_keltner_strategy.py
+-rw-rw-rw-   0        0        0     6118 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/strategies/multi_signal_strategy.py
+-rw-rw-rw-   0        0        0     3667 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/strategies/multi_timeframe_strategy.py
+-rw-rw-rw-   0        0        0     3044 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/strategies/test_strategy.py
+-rw-rw-rw-   0        0        0     4381 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/strategies/turtle_signal_strategy.py
+-rw-rw-rw-   0        0        0    13503 2023-01-06 11:08:07.000000 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/template.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:38:22.389650 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/ui/
+-rw-rw-rw-   0        0        0       32 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/ui/__init__.py
+-rw-rw-rw-   0        0        0    67646 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/ui/cta.ico
+-rw-rw-rw-   0        0        0     9024 2023-03-08 14:40:08.000000 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/ui/rollover.py
+-rw-rw-rw-   0        0        0    17453 2023-03-09 07:35:44.000000 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/ui/widget.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:38:22.338937 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy.egg-info/
+-rw-rw-rw-   0        0        0     1969 2023-04-23 03:38:22.000000 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1042 2023-04-23 03:38:22.000000 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 03:38:22.000000 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-23 03:38:22.000000 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       14 2023-04-23 03:38:22.000000 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-04-23 03:38:22.000000 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy.egg-info/top_level.txt
```

### Comparing `vnpy_ctastrategy-1.1.3/LICENSE` & `vnpy_ctastrategy-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vnpy_ctastrategy-1.1.3/PKG-INFO` & `vnpy_ctastrategy-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnpy_ctastrategy
-Version: 1.1.3
+Version: 1.1.4
 Summary: CTA strategy application for VeighNa quant trading framework.
 Home-page: https://www.vnpy.com
 Author: Xiaoyou Chen
 Author-email: xiaoyou.chen@mail.vnpy.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
 Platform: UNKNOWN
@@ -26,15 +26,15 @@
 # VeighNa框架的CTA策略模块
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-1.1.3-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-1.1.4-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
     <img src ="https://img.shields.io/badge/python-3.7|3.8|3.9|3.10-blue.svg" />
     <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
 </p>
 
 ## 说明
```

### Comparing `vnpy_ctastrategy-1.1.3/README.md` & `vnpy_ctastrategy-1.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # VeighNa框架的CTA策略模块
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-1.1.3-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-1.1.4-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
     <img src ="https://img.shields.io/badge/python-3.7|3.8|3.9|3.10-blue.svg" />
     <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
 </p>
 
 ## 说明
```

### Comparing `vnpy_ctastrategy-1.1.3/setup.cfg` & `vnpy_ctastrategy-1.1.4/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6e70 795f 6374 6173 7472 6174   = vnpy_ctastrat
 00000020: 6567 790d 0a76 6572 7369 6f6e 203d 2031  egy..version = 1
-00000030: 2e31 2e33 0d0a 7572 6c20 3d20 6874 7470  .1.3..url = http
+00000030: 2e31 2e34 0d0a 7572 6c20 3d20 6874 7470  .1.4..url = http
 00000040: 733a 2f2f 7777 772e 766e 7079 2e63 6f6d  s://www.vnpy.com
 00000050: 0d0a 6c69 6365 6e73 6520 3d20 4d49 540d  ..license = MIT.
 00000060: 0a61 7574 686f 7220 3d20 5869 616f 796f  .author = Xiaoyo
 00000070: 7520 4368 656e 0d0a 6175 7468 6f72 5f65  u Chen..author_e
 00000080: 6d61 696c 203d 2078 6961 6f79 6f75 2e63  mail = xiaoyou.c
 00000090: 6865 6e40 6d61 696c 2e76 6e70 792e 636f  hen@mail.vnpy.co
 000000a0: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
```

### Comparing `vnpy_ctastrategy-1.1.3/vnpy_ctastrategy/__init__.py` & `vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 
 from pathlib import Path
+from typing import Type
 
 import importlib_metadata
 from vnpy.trader.app import BaseApp
 from vnpy.trader.constant import Direction
 from vnpy.trader.object import TickData, BarData, TradeData, OrderData
 from vnpy.trader.utility import BarGenerator, ArrayManager
 
@@ -43,10 +44,10 @@
 class CtaStrategyApp(BaseApp):
     """"""
 
     app_name: str = APP_NAME
     app_module: str = __module__
     app_path: Path = Path(__file__).parent
     display_name: str = "CTA策略"
-    engine_class: CtaEngine = CtaEngine
+    engine_class: Type[CtaEngine] = CtaEngine
     widget_name: str = "CtaManager"
     icon_name: str = str(app_path.joinpath("ui", "cta.ico"))
```

### Comparing `vnpy_ctastrategy-1.1.3/vnpy_ctastrategy/backtesting.py` & `vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/backtesting.py`

 * *Files identical despite different names*

### Comparing `vnpy_ctastrategy-1.1.3/vnpy_ctastrategy/base.py` & `vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/base.py`

 * *Files identical despite different names*

### Comparing `vnpy_ctastrategy-1.1.3/vnpy_ctastrategy/engine.py` & `vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     EVENT_CTA_STRATEGY,
     EVENT_CTA_STOPORDER,
     EngineType,
     StopOrder,
     StopOrderStatus,
     STOPORDER_PREFIX
 )
-from .template import CtaTemplate
+from .template import CtaTemplate, TargetPosTemplate
 
 
 # 停止单状态映射
 STOP_STATUS_MAP: Dict[Status, StopOrderStatus] = {
     Status.SUBMITTING: StopOrderStatus.WAITING,
     Status.NOTTRADED: StopOrderStatus.WAITING,
     Status.PARTTRADED: StopOrderStatus.TRIGGERED,
@@ -810,15 +810,19 @@
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
 
     def load_strategy_data(self) -> None:
         """
@@ -915,14 +919,17 @@
         """
         if strategy_name not in self.strategy_setting:
             return
 
         self.strategy_setting.pop(strategy_name)
         save_json(self.setting_filename, self.strategy_setting)
 
+        self.strategy_data.pop(strategy_name, None)
+        save_json(self.data_filename, self.strategy_data)
+
     def put_stop_order_event(self, stop_order: StopOrder) -> None:
         """
         Put an event to update stop order status.
         """
         event: Event = Event(EVENT_CTA_STOPORDER, stop_order)
         self.event_engine.put(event)
```

### Comparing `vnpy_ctastrategy-1.1.3/vnpy_ctastrategy/strategies/atr_rsi_strategy.py` & `vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/strategies/atr_rsi_strategy.py`

 * *Files identical despite different names*

### Comparing `vnpy_ctastrategy-1.1.3/vnpy_ctastrategy/strategies/boll_channel_strategy.py` & `vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/strategies/boll_channel_strategy.py`

 * *Files identical despite different names*

### Comparing `vnpy_ctastrategy-1.1.3/vnpy_ctastrategy/strategies/double_ma_strategy.py` & `vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/strategies/double_ma_strategy.py`

 * *Files identical despite different names*

### Comparing `vnpy_ctastrategy-1.1.3/vnpy_ctastrategy/strategies/dual_thrust_strategy.py` & `vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/strategies/dual_thrust_strategy.py`

 * *Files identical despite different names*

### Comparing `vnpy_ctastrategy-1.1.3/vnpy_ctastrategy/strategies/king_keltner_strategy.py` & `vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/strategies/king_keltner_strategy.py`

 * *Files identical despite different names*

### Comparing `vnpy_ctastrategy-1.1.3/vnpy_ctastrategy/strategies/multi_signal_strategy.py` & `vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/strategies/multi_signal_strategy.py`

 * *Files identical despite different names*

### Comparing `vnpy_ctastrategy-1.1.3/vnpy_ctastrategy/strategies/multi_timeframe_strategy.py` & `vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/strategies/multi_timeframe_strategy.py`

 * *Files identical despite different names*

### Comparing `vnpy_ctastrategy-1.1.3/vnpy_ctastrategy/strategies/test_strategy.py` & `vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/strategies/test_strategy.py`

 * *Files identical despite different names*

### Comparing `vnpy_ctastrategy-1.1.3/vnpy_ctastrategy/strategies/turtle_signal_strategy.py` & `vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/strategies/turtle_signal_strategy.py`

 * *Files identical despite different names*

### Comparing `vnpy_ctastrategy-1.1.3/vnpy_ctastrategy/template.py` & `vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/template.py`

 * *Files identical despite different names*

### Comparing `vnpy_ctastrategy-1.1.3/vnpy_ctastrategy/ui/cta.ico` & `vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/ui/cta.ico`

 * *Files identical despite different names*

### Comparing `vnpy_ctastrategy-1.1.3/vnpy_ctastrategy/ui/rollover.py` & `vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/ui/rollover.py`

 * *Files identical despite different names*

### Comparing `vnpy_ctastrategy-1.1.3/vnpy_ctastrategy/ui/widget.py` & `vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/ui/widget.py`

 * *Files identical despite different names*

### Comparing `vnpy_ctastrategy-1.1.3/vnpy_ctastrategy.egg-info/PKG-INFO` & `vnpy_ctastrategy-1.1.4/vnpy_ctastrategy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnpy-ctastrategy
-Version: 1.1.3
+Version: 1.1.4
 Summary: CTA strategy application for VeighNa quant trading framework.
 Home-page: https://www.vnpy.com
 Author: Xiaoyou Chen
 Author-email: xiaoyou.chen@mail.vnpy.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
 Platform: UNKNOWN
@@ -26,15 +26,15 @@
 # VeighNa框架的CTA策略模块
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-1.1.3-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-1.1.4-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
     <img src ="https://img.shields.io/badge/python-3.7|3.8|3.9|3.10-blue.svg" />
     <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
 </p>
 
 ## 说明
```

### Comparing `vnpy_ctastrategy-1.1.3/vnpy_ctastrategy.egg-info/SOURCES.txt` & `vnpy_ctastrategy-1.1.4/vnpy_ctastrategy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

