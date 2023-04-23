# Comparing `tmp/vnpy_rpcservice-1.0.3.tar.gz` & `tmp/vnpy_rpcservice-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnpy_rpcservice-1.0.3.tar", last modified: Tue Oct 18 12:26:58 2022, max compression
+gzip compressed data, was "vnpy_rpcservice-1.0.4.tar", last modified: Sun Apr 23 04:19:59 2023, max compression
```

## Comparing `vnpy_rpcservice-1.0.3.tar` & `vnpy_rpcservice-1.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2022-10-18 12:26:58.657315 vnpy_rpcservice-1.0.3/
--rw-rw-rw-   0        0        0     1107 2021-12-21 01:00:32.000000 vnpy_rpcservice-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     2009 2022-10-18 12:26:58.658362 vnpy_rpcservice-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1000 2022-10-18 12:26:17.000000 vnpy_rpcservice-1.0.3/README.md
--rw-rw-rw-   0        0        0     1076 2022-10-18 12:26:58.679232 vnpy_rpcservice-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0       43 2021-12-20 13:28:27.000000 vnpy_rpcservice-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2022-10-18 12:26:58.552211 vnpy_rpcservice-1.0.3/vnpy_rpcservice/
--rw-rw-rw-   0        0        0     1404 2021-12-21 01:03:10.000000 vnpy_rpcservice-1.0.3/vnpy_rpcservice/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-18 12:26:58.602949 vnpy_rpcservice-1.0.3/vnpy_rpcservice/rpc_gateway/
--rw-rw-rw-   0        0        0       37 2021-12-20 13:28:27.000000 vnpy_rpcservice-1.0.3/vnpy_rpcservice/rpc_gateway/__init__.py
--rw-rw-rw-   0        0        0     4405 2022-08-01 12:20:06.000000 vnpy_rpcservice-1.0.3/vnpy_rpcservice/rpc_gateway/rpc_gateway.py
-drwxrwxrwx   0        0        0        0 2022-10-18 12:26:58.608748 vnpy_rpcservice-1.0.3/vnpy_rpcservice/rpc_service/
--rw-rw-rw-   0        0        0      440 2022-08-01 12:20:06.000000 vnpy_rpcservice-1.0.3/vnpy_rpcservice/rpc_service/__init__.py
--rw-rw-rw-   0        0        0     4255 2022-10-18 12:25:55.000000 vnpy_rpcservice-1.0.3/vnpy_rpcservice/rpc_service/engine.py
-drwxrwxrwx   0        0        0        0 2022-10-18 12:26:58.655708 vnpy_rpcservice-1.0.3/vnpy_rpcservice/rpc_service/ui/
--rw-rw-rw-   0        0        0       32 2021-12-20 13:28:27.000000 vnpy_rpcservice-1.0.3/vnpy_rpcservice/rpc_service/ui/__init__.py
--rw-rw-rw-   0        0        0    66622 2021-12-20 13:28:27.000000 vnpy_rpcservice-1.0.3/vnpy_rpcservice/rpc_service/ui/rpc.ico
--rw-rw-rw-   0        0        0     3401 2022-08-01 12:20:06.000000 vnpy_rpcservice-1.0.3/vnpy_rpcservice/rpc_service/ui/widget.py
-drwxrwxrwx   0        0        0        0 2022-10-18 12:26:58.596120 vnpy_rpcservice-1.0.3/vnpy_rpcservice.egg-info/
--rw-rw-rw-   0        0        0     2009 2022-10-18 12:26:57.000000 vnpy_rpcservice-1.0.3/vnpy_rpcservice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      580 2022-10-18 12:26:58.000000 vnpy_rpcservice-1.0.3/vnpy_rpcservice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-18 12:26:57.000000 vnpy_rpcservice-1.0.3/vnpy_rpcservice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-10-18 12:26:57.000000 vnpy_rpcservice-1.0.3/vnpy_rpcservice.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       19 2022-10-18 12:26:57.000000 vnpy_rpcservice-1.0.3/vnpy_rpcservice.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2022-10-18 12:26:57.000000 vnpy_rpcservice-1.0.3/vnpy_rpcservice.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 04:19:59.929775 vnpy_rpcservice-1.0.4/
+-rw-rw-rw-   0        0        0     1107 2023-04-22 13:14:11.000000 vnpy_rpcservice-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1986 2023-04-23 04:19:59.929775 vnpy_rpcservice-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1000 2023-04-23 04:19:00.000000 vnpy_rpcservice-1.0.4/README.md
+-rw-rw-rw-   0        0        0     1076 2023-04-23 04:19:59.931837 vnpy_rpcservice-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0       43 2023-04-22 13:14:11.000000 vnpy_rpcservice-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 04:19:59.878998 vnpy_rpcservice-1.0.4/vnpy_rpcservice/
+-rw-rw-rw-   0        0        0     1404 2023-04-22 13:14:11.000000 vnpy_rpcservice-1.0.4/vnpy_rpcservice/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 04:19:59.920012 vnpy_rpcservice-1.0.4/vnpy_rpcservice/rpc_gateway/
+-rw-rw-rw-   0        0        0       37 2023-04-22 13:14:11.000000 vnpy_rpcservice-1.0.4/vnpy_rpcservice/rpc_gateway/__init__.py
+-rw-rw-rw-   0        0        0     4667 2023-04-22 13:23:52.000000 vnpy_rpcservice-1.0.4/vnpy_rpcservice/rpc_gateway/rpc_gateway.py
+drwxrwxrwx   0        0        0        0 2023-04-23 04:19:59.923111 vnpy_rpcservice-1.0.4/vnpy_rpcservice/rpc_service/
+-rw-rw-rw-   0        0        0      440 2023-04-22 13:14:11.000000 vnpy_rpcservice-1.0.4/vnpy_rpcservice/rpc_service/__init__.py
+-rw-rw-rw-   0        0        0     4255 2023-04-22 13:14:11.000000 vnpy_rpcservice-1.0.4/vnpy_rpcservice/rpc_service/engine.py
+drwxrwxrwx   0        0        0        0 2023-04-23 04:19:59.928241 vnpy_rpcservice-1.0.4/vnpy_rpcservice/rpc_service/ui/
+-rw-rw-rw-   0        0        0       32 2023-04-22 13:14:11.000000 vnpy_rpcservice-1.0.4/vnpy_rpcservice/rpc_service/ui/__init__.py
+-rw-rw-rw-   0        0        0    66622 2023-04-22 13:14:11.000000 vnpy_rpcservice-1.0.4/vnpy_rpcservice/rpc_service/ui/rpc.ico
+-rw-rw-rw-   0        0        0     3401 2023-04-22 13:14:11.000000 vnpy_rpcservice-1.0.4/vnpy_rpcservice/rpc_service/ui/widget.py
+drwxrwxrwx   0        0        0        0 2023-04-23 04:19:59.917458 vnpy_rpcservice-1.0.4/vnpy_rpcservice.egg-info/
+-rw-rw-rw-   0        0        0     1986 2023-04-23 04:19:59.000000 vnpy_rpcservice-1.0.4/vnpy_rpcservice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      580 2023-04-23 04:19:59.000000 vnpy_rpcservice-1.0.4/vnpy_rpcservice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 04:19:59.000000 vnpy_rpcservice-1.0.4/vnpy_rpcservice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-23 04:19:59.000000 vnpy_rpcservice-1.0.4/vnpy_rpcservice.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       19 2023-04-23 04:19:59.000000 vnpy_rpcservice-1.0.4/vnpy_rpcservice.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-23 04:19:59.000000 vnpy_rpcservice-1.0.4/vnpy_rpcservice.egg-info/top_level.txt
```

### Comparing `vnpy_rpcservice-1.0.3/LICENSE` & `vnpy_rpcservice-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vnpy_rpcservice-1.0.3/PKG-INFO` & `vnpy_rpcservice-1.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: vnpy_rpcservice
-Version: 1.0.3
+Version: 1.0.4
 Summary: RPC service application and gateway for VeighNa quant trading framework.
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
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -25,15 +24,15 @@
 # VeighNa框架的RPC服务应用
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-1.0.3-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-1.0.4-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-linux|windows|mac-yellow.svg"/>
     <img src ="https://img.shields.io/badge/python-3.7|3.8|3.9|3.10-blue.svg" />
     <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
 </p>
 
 ## 说明
 
@@ -51,9 +50,7 @@
 
 
 或者下载源代码后，解压后在cmd中运行：
 
 ```
 pip install .
 ```
-
-
```

### Comparing `vnpy_rpcservice-1.0.3/README.md` & `vnpy_rpcservice-1.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # VeighNa框架的RPC服务应用
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-1.0.3-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-1.0.4-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-linux|windows|mac-yellow.svg"/>
     <img src ="https://img.shields.io/badge/python-3.7|3.8|3.9|3.10-blue.svg" />
     <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
 </p>
 
 ## 说明
```

### Comparing `vnpy_rpcservice-1.0.3/setup.cfg` & `vnpy_rpcservice-1.0.4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6e70 795f 7270 6373 6572 7669   = vnpy_rpcservi
 00000020: 6365 0d0a 7665 7273 696f 6e20 3d20 312e  ce..version = 1.
-00000030: 302e 330d 0a75 726c 203d 2068 7474 7073  0.3..url = https
+00000030: 302e 340d 0a75 726c 203d 2068 7474 7073  0.4..url = https
 00000040: 3a2f 2f77 7777 2e76 6e70 792e 636f 6d0d  ://www.vnpy.com.
 00000050: 0a6c 6963 656e 7365 203d 204d 4954 0d0a  .license = MIT..
 00000060: 6175 7468 6f72 203d 2058 6961 6f79 6f75  author = Xiaoyou
 00000070: 2043 6865 6e0d 0a61 7574 686f 725f 656d   Chen..author_em
 00000080: 6169 6c20 3d20 7869 616f 796f 752e 6368  ail = xiaoyou.ch
 00000090: 656e 406d 6169 6c2e 766e 7079 2e63 6f6d  en@mail.vnpy.com
 000000a0: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description =
```

### Comparing `vnpy_rpcservice-1.0.3/vnpy_rpcservice/__init__.py` & `vnpy_rpcservice-1.0.4/vnpy_rpcservice/__init__.py`

 * *Files identical despite different names*

### Comparing `vnpy_rpcservice-1.0.3/vnpy_rpcservice/rpc_gateway/rpc_gateway.py` & `vnpy_rpcservice-1.0.4/vnpy_rpcservice/rpc_gateway/rpc_gateway.py`

 * *Files 6% similar despite different names*

```diff
@@ -91,32 +91,36 @@
             contract.gateway_name = self.gateway_name
             self.on_contract(contract)
         self.write_log("合约信息查询成功")
 
         accounts: List[AccountData] = self.client.get_all_accounts()
         for account in accounts:
             account.gateway_name = self.gateway_name
+            account.__post_init__()
             self.on_account(account)
         self.write_log("资金信息查询成功")
 
         positions: List[PositionData] = self.client.get_all_positions()
         for position in positions:
             position.gateway_name = self.gateway_name
+            position.__post_init__()
             self.on_position(position)
         self.write_log("持仓信息查询成功")
 
         orders: List[OrderData] = self.client.get_all_orders()
         for order in orders:
             order.gateway_name = self.gateway_name
+            order.__post_init__()
             self.on_order(order)
         self.write_log("委托信息查询成功")
 
         trades: List[TradeData] = self.client.get_all_trades()
         for trade in trades:
             trade.gateway_name = self.gateway_name
+            trade.__post_init__()
             self.on_trade(trade)
         self.write_log("成交信息查询成功")
 
     def close(self) -> None:
         """关闭连接"""
         self.client.stop()
         self.client.join()
@@ -128,8 +132,11 @@
             return
 
         data: Any = event.data
 
         if hasattr(data, "gateway_name"):
             data.gateway_name = self.gateway_name
 
+        if isinstance(data, (PositionData, AccountData, OrderData, TradeData)):
+            data.__post_init__()
+
         self.event_engine.put(event)
```

### Comparing `vnpy_rpcservice-1.0.3/vnpy_rpcservice/rpc_service/engine.py` & `vnpy_rpcservice-1.0.4/vnpy_rpcservice/rpc_service/engine.py`

 * *Files identical despite different names*

### Comparing `vnpy_rpcservice-1.0.3/vnpy_rpcservice/rpc_service/ui/rpc.ico` & `vnpy_rpcservice-1.0.4/vnpy_rpcservice/rpc_service/ui/rpc.ico`

 * *Files identical despite different names*

### Comparing `vnpy_rpcservice-1.0.3/vnpy_rpcservice/rpc_service/ui/widget.py` & `vnpy_rpcservice-1.0.4/vnpy_rpcservice/rpc_service/ui/widget.py`

 * *Files identical despite different names*

### Comparing `vnpy_rpcservice-1.0.3/vnpy_rpcservice.egg-info/PKG-INFO` & `vnpy_rpcservice-1.0.4/vnpy_rpcservice.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: vnpy-rpcservice
-Version: 1.0.3
+Version: 1.0.4
 Summary: RPC service application and gateway for VeighNa quant trading framework.
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
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -25,15 +24,15 @@
 # VeighNa框架的RPC服务应用
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-1.0.3-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-1.0.4-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-linux|windows|mac-yellow.svg"/>
     <img src ="https://img.shields.io/badge/python-3.7|3.8|3.9|3.10-blue.svg" />
     <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
 </p>
 
 ## 说明
 
@@ -51,9 +50,7 @@
 
 
 或者下载源代码后，解压后在cmd中运行：
 
 ```
 pip install .
 ```
-
-
```

### Comparing `vnpy_rpcservice-1.0.3/vnpy_rpcservice.egg-info/SOURCES.txt` & `vnpy_rpcservice-1.0.4/vnpy_rpcservice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

