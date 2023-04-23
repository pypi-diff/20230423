# Comparing `tmp/vnpy_dolphindb-1.0.7.tar.gz` & `tmp/vnpy_dolphindb-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnpy_dolphindb-1.0.7.tar", last modified: Thu Mar 23 13:17:16 2023, max compression
+gzip compressed data, was "vnpy_dolphindb-1.0.8.tar", last modified: Sun Apr 23 01:16:32 2023, max compression
```

## Comparing `vnpy_dolphindb-1.0.7.tar` & `vnpy_dolphindb-1.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-03-23 13:17:16.742915 vnpy_dolphindb-1.0.7/
--rw-rw-rw-   0        0        0     1099 2023-03-23 12:55:55.000000 vnpy_dolphindb-1.0.7/LICENSE
--rw-rw-rw-   0        0        0     1962 2023-03-23 13:17:16.742915 vnpy_dolphindb-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      911 2023-03-23 13:15:35.000000 vnpy_dolphindb-1.0.7/README.md
--rw-rw-rw-   0        0        0     1061 2023-03-23 13:17:16.745149 vnpy_dolphindb-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0       43 2023-03-23 12:55:55.000000 vnpy_dolphindb-1.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-23 13:17:16.695141 vnpy_dolphindb-1.0.7/vnpy_dolphindb/
--rw-rw-rw-   0        0        0     1389 2023-03-23 12:55:55.000000 vnpy_dolphindb-1.0.7/vnpy_dolphindb/__init__.py
--rw-rw-rw-   0        0        0    17662 2023-03-23 13:13:42.000000 vnpy_dolphindb-1.0.7/vnpy_dolphindb/dolphindb_database.py
--rw-rw-rw-   0        0        0     3230 2023-03-23 13:13:42.000000 vnpy_dolphindb-1.0.7/vnpy_dolphindb/dolphindb_script.py
-drwxrwxrwx   0        0        0        0 2023-03-23 13:17:16.739901 vnpy_dolphindb-1.0.7/vnpy_dolphindb.egg-info/
--rw-rw-rw-   0        0        0     1962 2023-03-23 13:17:16.000000 vnpy_dolphindb-1.0.7/vnpy_dolphindb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      361 2023-03-23 13:17:16.000000 vnpy_dolphindb-1.0.7/vnpy_dolphindb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-23 13:17:16.000000 vnpy_dolphindb-1.0.7/vnpy_dolphindb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-23 13:17:16.000000 vnpy_dolphindb-1.0.7/vnpy_dolphindb.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       10 2023-03-23 13:17:16.000000 vnpy_dolphindb-1.0.7/vnpy_dolphindb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-03-23 13:17:16.000000 vnpy_dolphindb-1.0.7/vnpy_dolphindb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 01:16:32.673862 vnpy_dolphindb-1.0.8/
+-rw-rw-rw-   0        0        0     1099 2023-04-23 00:47:01.000000 vnpy_dolphindb-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0     1927 2023-04-23 01:16:32.673862 vnpy_dolphindb-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      899 2023-04-23 01:15:59.000000 vnpy_dolphindb-1.0.8/README.md
+-rw-rw-rw-   0        0        0     1061 2023-04-23 01:16:32.676468 vnpy_dolphindb-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0       43 2023-04-23 00:47:01.000000 vnpy_dolphindb-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 01:16:32.646272 vnpy_dolphindb-1.0.8/vnpy_dolphindb/
+-rw-rw-rw-   0        0        0     1389 2023-04-23 00:47:01.000000 vnpy_dolphindb-1.0.8/vnpy_dolphindb/__init__.py
+-rw-rw-rw-   0        0        0    18161 2023-04-23 01:03:17.000000 vnpy_dolphindb-1.0.8/vnpy_dolphindb/dolphindb_database.py
+-rw-rw-rw-   0        0        0     3332 2023-04-23 01:03:49.000000 vnpy_dolphindb-1.0.8/vnpy_dolphindb/dolphindb_script.py
+drwxrwxrwx   0        0        0        0 2023-04-23 01:16:32.671750 vnpy_dolphindb-1.0.8/vnpy_dolphindb.egg-info/
+-rw-rw-rw-   0        0        0     1927 2023-04-23 01:16:32.000000 vnpy_dolphindb-1.0.8/vnpy_dolphindb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      361 2023-04-23 01:16:32.000000 vnpy_dolphindb-1.0.8/vnpy_dolphindb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 01:16:32.000000 vnpy_dolphindb-1.0.8/vnpy_dolphindb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-23 01:10:37.000000 vnpy_dolphindb-1.0.8/vnpy_dolphindb.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       10 2023-04-23 01:16:32.000000 vnpy_dolphindb-1.0.8/vnpy_dolphindb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-23 01:16:32.000000 vnpy_dolphindb-1.0.8/vnpy_dolphindb.egg-info/top_level.txt
```

### Comparing `vnpy_dolphindb-1.0.7/LICENSE` & `vnpy_dolphindb-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `vnpy_dolphindb-1.0.7/PKG-INFO` & `vnpy_dolphindb-1.0.8/vnpy_dolphindb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
-Name: vnpy_dolphindb
-Version: 1.0.7
+Name: vnpy-dolphindb
+Version: 1.0.8
 Summary: DolphinDB database adapter for vn.py quant trading framework.
 Home-page: https://www.vnpy.com
 Author: Xiaoyou Chen
 Author-email: xiaoyou.chen@mail.vnpy.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -26,17 +25,17 @@
 # VeighNa框架的DolphinDB数据库接口
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-1.0.7-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-1.0.8-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-linux|windows-yellow.svg"/>
-    <img src ="https://img.shields.io/badge/python-3.7|3.8|3.9|3.10-blue.svg" />
+    <img src ="https://img.shields.io/badge/python-3.10-blue.svg" />
 </p>
 
 ## 说明
 
 基于dolphindb开发的DolphinDB数据库接口。
 
 **需要使用DolphinDB 2.0以上版本。**
@@ -49,9 +48,7 @@
 |---------|----|---|---|
 |database.name|名称|是|dolphindb|
 |database.host|地址|是|localhost|
 |database.port|端口|是|8848|
 |database.database|实例|是|vnpy|
 |database.user|用户名|是|admin|
 |database.password|密码|是|123456|
-
-
```

### Comparing `vnpy_dolphindb-1.0.7/README.md` & `vnpy_dolphindb-1.0.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # VeighNa框架的DolphinDB数据库接口
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-1.0.7-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-1.0.8-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-linux|windows-yellow.svg"/>
-    <img src ="https://img.shields.io/badge/python-3.7|3.8|3.9|3.10-blue.svg" />
+    <img src ="https://img.shields.io/badge/python-3.10-blue.svg" />
 </p>
 
 ## 说明
 
 基于dolphindb开发的DolphinDB数据库接口。
 
 **需要使用DolphinDB 2.0以上版本。**
```

### Comparing `vnpy_dolphindb-1.0.7/setup.cfg` & `vnpy_dolphindb-1.0.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6e70 795f 646f 6c70 6869 6e64   = vnpy_dolphind
 00000020: 620d 0a76 6572 7369 6f6e 203d 2031 2e30  b..version = 1.0
-00000030: 2e37 0d0a 7572 6c20 3d20 6874 7470 733a  .7..url = https:
+00000030: 2e38 0d0a 7572 6c20 3d20 6874 7470 733a  .8..url = https:
 00000040: 2f2f 7777 772e 766e 7079 2e63 6f6d 0d0a  //www.vnpy.com..
 00000050: 6c69 6365 6e73 6520 3d20 4d49 540d 0a61  license = MIT..a
 00000060: 7574 686f 7220 3d20 5869 616f 796f 7520  uthor = Xiaoyou 
 00000070: 4368 656e 0d0a 6175 7468 6f72 5f65 6d61  Chen..author_ema
 00000080: 696c 203d 2078 6961 6f79 6f75 2e63 6865  il = xiaoyou.che
 00000090: 6e40 6d61 696c 2e76 6e70 792e 636f 6d0d  n@mail.vnpy.com.
 000000a0: 0a64 6573 6372 6970 7469 6f6e 203d 2044  .description = D
```

### Comparing `vnpy_dolphindb-1.0.7/vnpy_dolphindb/__init__.py` & `vnpy_dolphindb-1.0.8/vnpy_dolphindb/__init__.py`

 * *Files identical despite different names*

### Comparing `vnpy_dolphindb-1.0.7/vnpy_dolphindb/dolphindb_database.py` & `vnpy_dolphindb-1.0.8/vnpy_dolphindb/dolphindb_database.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from typing import Dict, List
 from datetime import datetime
 
 import numpy as np
 import pandas as pd
 import dolphindb as ddb
 
 from vnpy.trader.constant import Exchange, Interval
@@ -25,51 +24,56 @@
 )
 
 
 class DolphindbDatabase(BaseDatabase):
     """DolphinDB数据库接口"""
 
     def __init__(self) -> None:
-        """"""
+        """构造函数"""
         self.user: str = SETTINGS["database.user"]
         self.password: str = SETTINGS["database.password"]
         self.host: str = SETTINGS["database.host"]
         self.port: int = SETTINGS["database.port"]
-        self.db_path: str = "dfs://vnpy"
+        self.db_path: str = "dfs://" + SETTINGS["database.database"]
 
         # 连接数据库
-        self.session = ddb.session()
+        self.session: ddb.session = ddb.session()
         self.session.connect(self.host, self.port, self.user, self.password)
 
         # 创建连接池（用于数据写入）
-        self.pool = ddb.DBConnectionPool(self.host, self.port, 1, self.user, self.password)
+        self.pool: ddb.DBConnectionPool = ddb.DBConnectionPool(self.host, self.port, 1, self.user, self.password)
 
         # 初始化数据库和数据表
         if not self.session.existsDatabase(self.db_path):
             self.session.run(CREATE_DATABASE_SCRIPT)
             self.session.run(CREATE_BAR_TABLE_SCRIPT)
             self.session.run(CREATE_TICK_TABLE_SCRIPT)
             self.session.run(CREATE_BAROVERVIEW_TABLE_SCRIPT)
             self.session.run(CREATE_TICKOVERVIEW_TABLE_SCRIPT)
 
-    def save_bar_data(self, bars: List[BarData], stream: bool = False) -> bool:
+    def __del__(self) -> None:
+        """析构函数"""
+        if not self.session.isClosed():
+            self.session.close()
+
+    def save_bar_data(self, bars: list[BarData], stream: bool = False) -> bool:
         """保存k线数据"""
         # 读取主键参数
         bar: BarData = bars[0]
         symbol: str = bar.symbol
         exchange: Exchange = bar.exchange
         interval: Interval = bar.interval
 
         # 转换为DatFrame写入数据库
-        data: List[dict] = []
+        data: list[dict] = []
 
         for bar in bars:
-            dt = np.datetime64(convert_tz(bar.datetime))
+            dt: np.datetime64 = np.datetime64(convert_tz(bar.datetime))
 
-            d = {
+            d: dict = {
                 "symbol": symbol,
                 "exchange": exchange.value,
                 "datetime": dt,
                 "interval": interval.value,
                 "volume": float(bar.volume),
                 "turnover": float(bar.turnover),
                 "open_interest": float(bar.open_interest),
@@ -79,15 +83,15 @@
                 "close_price": float(bar.close_price)
             }
 
             data.append(d)
 
         df: pd.DataFrame = pd.DataFrame.from_records(data)
 
-        appender = ddb.PartitionedTableAppender(self.db_path, "bar", "datetime", self.pool)
+        appender: ddb.PartitionedTableAppender = ddb.PartitionedTableAppender(self.db_path, "bar", "datetime", self.pool)
         appender.append(df)
 
         # 计算已有K线数据的汇总
         overview_table = self.session.loadTable(tableName="baroverview", dbPath=self.db_path)
         overview: pd.DataFrame = (
             overview_table.select('*')
             .where(f'symbol="{symbol}"')
@@ -117,49 +121,49 @@
                 .where(f'interval="{interval.value}"')
                 .toDF()
             )
 
             count: int = df_count["count"][0]
 
         # 更新K线汇总数据
-        data: List[dict] = []
+        data: list[dict] = []
 
-        dt = np.datetime64(datetime(2022, 1, 1))    # 该时间戳仅用于分区
+        dt: np.datetime64 = np.datetime64(datetime(2022, 1, 1))    # 该时间戳仅用于分区
 
-        d: Dict = {
+        d: dict = {
             "symbol": symbol,
             "exchange": exchange.value,
             "interval": interval.value,
             "count": count,
             "start": start,
             "end": end,
             "datetime": dt,
         }
         data.append(d)
 
         df: pd.DataFrame = pd.DataFrame.from_records(data)
 
-        appender = ddb.PartitionedTableAppender(self.db_path, "baroverview", "datetime", self.pool)
+        appender: ddb.PartitionedTableAppender = ddb.PartitionedTableAppender(self.db_path, "baroverview", "datetime", self.pool)
         appender.append(df)
 
         return True
 
-    def save_tick_data(self, ticks: List[TickData], stream: bool = False) -> bool:
+    def save_tick_data(self, ticks: list[TickData], stream: bool = False) -> bool:
         """保存TICK数据"""
         # 读取主键参数
         tick: BarData = ticks[0]
         symbol: str = tick.symbol
         exchange: Exchange = tick.exchange
 
-        data: List[dict] = []
+        data: list[dict] = []
 
         for tick in ticks:
-            dt = np.datetime64(convert_tz(tick.datetime))
+            dt: np.datetime64 = np.datetime64(convert_tz(tick.datetime))
 
-            d: Dict = {
+            d: dict = {
                 "symbol": tick.symbol,
                 "exchange": tick.exchange.value,
                 "datetime": dt,
 
                 "name": tick.name,
                 "volume": float(tick.volume),
                 "turnover": float(tick.turnover),
@@ -201,15 +205,15 @@
                 "localtime": np.datetime64(tick.localtime),
             }
 
             data.append(d)
 
         df: pd.DataFrame = pd.DataFrame.from_records(data)
 
-        appender = ddb.PartitionedTableAppender(self.db_path, "tick", "datetime", self.pool)
+        appender: ddb.PartitionedTableAppender = ddb.PartitionedTableAppender(self.db_path, "tick", "datetime", self.pool)
         appender.append(df)
 
         # 计算已有Tick数据的汇总
         overview_table = self.session.loadTable(tableName="tickoverview", dbPath=self.db_path)
         overview: pd.DataFrame = (
             overview_table.select('*')
             .where(f'symbol="{symbol}"')
@@ -237,52 +241,52 @@
                 .where(f'exchange="{exchange.value}"')
                 .toDF()
             )
 
             count: int = df_count["count"][0]
 
         # 更新Tick汇总数据
-        data: List[dict] = []
+        data: list[dict] = []
 
-        dt = np.datetime64(datetime(2022, 1, 1))    # 该时间戳仅用于分区
+        dt: np.datetime64 = np.datetime64(datetime(2022, 1, 1))    # 该时间戳仅用于分区
 
-        d: Dict = {
+        d: dict = {
             "symbol": symbol,
             "exchange": exchange.value,
             "count": count,
             "start": start,
             "end": end,
             "datetime": dt,
         }
         data.append(d)
 
         df: pd.DataFrame = pd.DataFrame.from_records(data)
 
-        appender = ddb.PartitionedTableAppender(self.db_path, "tickoverview", "datetime", self.pool)
+        appender: ddb.PartitionedTableAppender = ddb.PartitionedTableAppender(self.db_path, "tickoverview", "datetime", self.pool)
         appender.append(df)
 
         return True
 
     def load_bar_data(
         self,
         symbol: str,
         exchange: Exchange,
         interval: Interval,
         start: datetime,
         end: datetime
-    ) -> List[BarData]:
+    ) -> list[BarData]:
         """读取K线数据"""
         # 转换时间格式
         start = np.datetime64(start)
         start: str = str(start).replace("-", ".")
 
         end = np.datetime64(end)
         end: str = str(end).replace("-", ".")
 
-        table = self.session.loadTable(tableName="bar", dbPath=self.db_path)
+        table: ddb.Table = self.session.loadTable(tableName="bar", dbPath=self.db_path)
 
         df: pd.DataFrame = (
             table.select('*')
             .where(f'symbol="{symbol}"')
             .where(f'exchange="{exchange.value}"')
             .where(f'interval="{interval.value}"')
             .where(f'datetime>={start}')
@@ -293,15 +297,15 @@
         if df.empty:
             return []
 
         df.set_index("datetime", inplace=True)
         df = df.tz_localize(DB_TZ.key)
 
         # 转换为BarData格式
-        bars: List[BarData] = []
+        bars: list[BarData] = []
 
         for tp in df.itertuples():
             bar = BarData(
                 symbol=symbol,
                 exchange=exchange,
                 datetime=tp.Index.to_pydatetime(),
                 interval=interval,
@@ -320,25 +324,25 @@
 
     def load_tick_data(
         self,
         symbol: str,
         exchange: Exchange,
         start: datetime,
         end: datetime
-    ) -> List[TickData]:
+    ) -> list[TickData]:
         """读取Tick数据"""
         # 转换时间格式
         start = np.datetime64(start)
         start: str = str(start).replace("-", ".")
 
         end = np.datetime64(end)
         end: str = str(end).replace("-", ".")
 
         # 读取数据DataFrame
-        table = self.session.loadTable(tableName="tick", dbPath=self.db_path)
+        table: ddb.Table = self.session.loadTable(tableName="tick", dbPath=self.db_path)
 
         df: pd.DataFrame = (
             table.select('*')
             .where(f'symbol="{symbol}"')
             .where(f'exchange="{exchange.value}"')
             .where(f'datetime>={start}')
             .where(f'datetime<={end}')
@@ -348,18 +352,18 @@
         if df.empty:
             return []
 
         df.set_index("datetime", inplace=True)
         df = df.tz_localize(DB_TZ.key)
 
         # 转换为TickData格式
-        ticks: List[TickData] = []
+        ticks: list[TickData] = []
 
         for tp in df.itertuples():
-            tick = TickData(
+            tick: TickData = TickData(
                 symbol=symbol,
                 exchange=exchange,
                 datetime=tp.Index.to_pydatetime(),
                 name=tp.name,
                 volume=tp.volume,
                 turnover=tp.turnover,
                 open_interest=tp.open_interest,
@@ -402,37 +406,37 @@
         self,
         symbol: str,
         exchange: Exchange,
         interval: Interval
     ) -> int:
         """删除K线数据"""
         # 加载数据表
-        table = self.session.loadTable(tableName="bar", dbPath=self.db_path)
+        table: ddb.Table = self.session.loadTable(tableName="bar", dbPath=self.db_path)
 
         # 统计数据量
         df: pd.DataFrame = (
             table.select('count(*)')
             .where(f'symbol="{symbol}"')
             .where(f'exchange="{exchange.value}"')
             .where(f'interval="{interval.value}"')
             .toDF()
         )
-        count = df["count"][0]
+        count: int = df["count"][0]
 
         # 删除K线数据
         (
             table.delete()
             .where(f'symbol="{symbol}"')
             .where(f'exchange="{exchange.value}"')
             .where(f'interval="{interval.value}"')
             .execute()
         )
 
         # 删除K线汇总
-        table = self.session.loadTable(tableName="baroverview", dbPath=self.db_path)
+        table: ddb.Table = self.session.loadTable(tableName="baroverview", dbPath=self.db_path)
         (
             table.delete()
             .where(f'symbol="{symbol}"')
             .where(f'exchange="{exchange.value}"')
             .where(f'interval="{interval.value}"')
             .execute()
         )
@@ -442,15 +446,15 @@
     def delete_tick_data(
         self,
         symbol: str,
         exchange: Exchange
     ) -> int:
         """删除Tick数据"""
         # 加载数据表
-        table = self.session.loadTable(tableName="tick", dbPath=self.db_path)
+        table: ddb.Table = self.session.loadTable(tableName="tick", dbPath=self.db_path)
 
         # 统计数据量
         df: pd.DataFrame = (
             table.select('count(*)')
             .where(f'symbol="{symbol}"')
             .where(f'exchange="{exchange.value}"')
             .toDF()
@@ -462,55 +466,55 @@
             table.delete()
             .where(f'symbol="{symbol}"')
             .where(f'exchange="{exchange.value}"')
             .execute()
         )
 
         # 删除Tick汇总
-        table = self.session.loadTable(tableName="tickoverview", dbPath=self.db_path)
+        table: ddb.Table = self.session.loadTable(tableName="tickoverview", dbPath=self.db_path)
         (
             table.delete()
             .where(f'symbol="{symbol}"')
             .where(f'exchange="{exchange.value}"')
             .execute()
         )
 
         return count
 
-    def get_bar_overview(self) -> List[BarOverview]:
+    def get_bar_overview(self) -> list[BarOverview]:
         """"查询数据库中的K线汇总信息"""
-        table = self.session.loadTable(tableName="baroverview", dbPath=self.db_path)
+        table: ddb.Table = self.session.loadTable(tableName="baroverview", dbPath=self.db_path)
         df: pd.DataFrame = table.select('*').toDF()
 
-        overviews: List[BarOverview] = []
+        overviews: list[BarOverview] = []
 
         for tp in df.itertuples():
-            overview = BarOverview(
+            overview: BarOverview = BarOverview(
                 symbol=tp.symbol,
                 exchange=Exchange(tp.exchange),
                 interval=Interval(tp.interval),
                 count=tp.count,
                 start=datetime.fromtimestamp(tp.start.to_pydatetime().timestamp(), DB_TZ),
                 end=datetime.fromtimestamp(tp.end.to_pydatetime().timestamp(), DB_TZ),
             )
             overviews.append(overview)
 
         return overviews
 
-    def get_tick_overview(self) -> List[TickOverview]:
+    def get_tick_overview(self) -> list[TickOverview]:
         """"查询数据库中的K线汇总信息"""
-        table = self.session.loadTable(tableName="tickoverview", dbPath=self.db_path)
+        table: ddb.Table = self.session.loadTable(tableName="tickoverview", dbPath=self.db_path)
         df: pd.DataFrame = table.select('*').toDF()
 
-        overviews: List[TickOverview] = []
+        overviews: list[TickOverview] = []
 
         for tp in df.itertuples():
-            overview = TickOverview(
+            overview: TickOverview = TickOverview(
                 symbol=tp.symbol,
                 exchange=Exchange(tp.exchange),
                 count=tp.count,
                 start=datetime.fromtimestamp(tp.start.to_pydatetime().timestamp(), DB_TZ),
                 end=datetime.fromtimestamp(tp.end.to_pydatetime().timestamp(), DB_TZ),
             )
             overviews.append(overview)
 
-        return overviews
+        return overviews
```

### Comparing `vnpy_dolphindb-1.0.7/vnpy_dolphindb/dolphindb_script.py` & `vnpy_dolphindb-1.0.8/vnpy_dolphindb/dolphindb_script.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 """
 DolphinDB脚本，用于在DolphinDB中创建数据库和数据表。
 """
 
+from vnpy.trader.setting import SETTINGS
+
+
+DB_PATH = "dfs://" + SETTINGS["database.database"]
+
+
 # 创建数据库
-CREATE_DATABASE_SCRIPT = """
-dataPath = "dfs://vnpy"
+CREATE_DATABASE_SCRIPT = f"""
+dataPath = "{DB_PATH}"
 db = database(dataPath, VALUE, 2000.01M..2030.12M, engine=`TSDB)
 """
 
 # 创建bar表
-CREATE_BAR_TABLE_SCRIPT = """
-dataPath = "dfs://vnpy"
+CREATE_BAR_TABLE_SCRIPT = f"""
+dataPath = "{DB_PATH}"
 db = database(dataPath)
 
 bar_columns = ["symbol", "exchange", "datetime", "interval", "volume", "turnover", "open_interest", "open_price", "high_price", "low_price", "close_price"]
 bar_type = [SYMBOL, SYMBOL, NANOTIMESTAMP, SYMBOL, DOUBLE, DOUBLE, DOUBLE, DOUBLE, DOUBLE, DOUBLE, DOUBLE]
 bar = table(1:0, bar_columns, bar_type)
 
 db.createPartitionedTable(
@@ -22,16 +28,16 @@
     "bar",
     partitionColumns=["datetime"],
     sortColumns=["symbol", "exchange", "interval", "datetime"],
     keepDuplicates=LAST)
 """
 
 # 创建tick表
-CREATE_TICK_TABLE_SCRIPT = """
-dataPath = "dfs://vnpy"
+CREATE_TICK_TABLE_SCRIPT = f"""
+dataPath = "{DB_PATH}"
 db = database(dataPath)
 
 tick_columns = ["symbol", "exchange", "datetime", "name", "volume", "turnover", "open_interest", "last_price", "last_volume", "limit_up", "limit_down",
                 "open_price", "high_price", "low_price", "pre_close",
                 "bid_price_1", "bid_price_2", "bid_price_3", "bid_price_4", "bid_price_5",
                 "ask_price_1", "ask_price_2", "ask_price_3", "ask_price_4", "ask_price_5",
                 "bid_volume_1", "bid_volume_2", "bid_volume_3", "bid_volume_4", "bid_volume_5",
@@ -49,32 +55,32 @@
     "tick",
     partitionColumns=["datetime"],
     sortColumns=["symbol", "exchange", "datetime"],
     keepDuplicates=LAST)
 """
 
 # 创建bar_overview表
-CREATE_BAROVERVIEW_TABLE_SCRIPT = """
-dataPath = "dfs://vnpy"
+CREATE_BAROVERVIEW_TABLE_SCRIPT = f"""
+dataPath = "{DB_PATH}"
 db = database(dataPath)
 
 overview_columns = ["symbol", "exchange", "interval", "count", "start", "end", "datetime"]
 overview_type = [SYMBOL, SYMBOL, SYMBOL, INT, NANOTIMESTAMP, NANOTIMESTAMP, NANOTIMESTAMP]
 baroverview = table(1:0, overview_columns, overview_type)
 db.createPartitionedTable(
     baroverview,
     "baroverview",
     partitionColumns=["datetime"],
     sortColumns=["symbol", "exchange", "interval", "datetime"],
     keepDuplicates=LAST)
 """
 
 # 创建tick_overview表
-CREATE_TICKOVERVIEW_TABLE_SCRIPT = """
-dataPath = "dfs://vnpy"
+CREATE_TICKOVERVIEW_TABLE_SCRIPT = f"""
+dataPath = "{DB_PATH}"
 db = database(dataPath)
 overview_columns = ["symbol", "exchange", "count", "start", "end", "datetime"]
 overview_type = [SYMBOL, SYMBOL, INT, NANOTIMESTAMP, NANOTIMESTAMP, NANOTIMESTAMP]
 tickoverview = table(1:0, overview_columns, overview_type)
 db.createPartitionedTable(
     tickoverview,
     "tickoverview",
```

### Comparing `vnpy_dolphindb-1.0.7/vnpy_dolphindb.egg-info/PKG-INFO` & `vnpy_dolphindb-1.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
-Name: vnpy-dolphindb
-Version: 1.0.7
+Name: vnpy_dolphindb
+Version: 1.0.8
 Summary: DolphinDB database adapter for vn.py quant trading framework.
 Home-page: https://www.vnpy.com
 Author: Xiaoyou Chen
 Author-email: xiaoyou.chen@mail.vnpy.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -26,17 +25,17 @@
 # VeighNa框架的DolphinDB数据库接口
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-1.0.7-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-1.0.8-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-linux|windows-yellow.svg"/>
-    <img src ="https://img.shields.io/badge/python-3.7|3.8|3.9|3.10-blue.svg" />
+    <img src ="https://img.shields.io/badge/python-3.10-blue.svg" />
 </p>
 
 ## 说明
 
 基于dolphindb开发的DolphinDB数据库接口。
 
 **需要使用DolphinDB 2.0以上版本。**
@@ -49,9 +48,7 @@
 |---------|----|---|---|
 |database.name|名称|是|dolphindb|
 |database.host|地址|是|localhost|
 |database.port|端口|是|8848|
 |database.database|实例|是|vnpy|
 |database.user|用户名|是|admin|
 |database.password|密码|是|123456|
-
-
```

