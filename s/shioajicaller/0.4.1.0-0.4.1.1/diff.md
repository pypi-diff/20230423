# Comparing `tmp/shioajicaller-0.4.1.0.tar.gz` & `tmp/shioajicaller-0.4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shioajicaller-0.4.1.0.tar", max compression
+gzip compressed data, was "shioajicaller-0.4.1.1.tar", max compression
```

## Comparing `shioajicaller-0.4.1.0.tar` & `shioajicaller-0.4.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1074 2021-07-18 10:36:07.309953 shioajicaller-0.4.1.0/LICENSE
--rw-r--r--   0        0        0    21151 2023-04-23 03:55:56.545221 shioajicaller-0.4.1.0/README.md
--rw-r--r--   0        0        0      671 2023-04-23 04:03:17.620627 shioajicaller-0.4.1.0/pyproject.toml
--rw-r--r--   0        0        0       64 2023-01-07 06:34:39.824248 shioajicaller-0.4.1.0/shioajicaller/__init__.py
--rw-r--r--   0        0        0    20163 2023-01-07 06:34:39.824583 shioajicaller-0.4.1.0/shioajicaller/caller.py
--rw-r--r--   0        0        0     5631 2023-04-23 03:50:23.401077 shioajicaller-0.4.1.0/shioajicaller/cli/__init__.py
--rw-r--r--   0        0        0       56 2021-07-22 10:56:11.854486 shioajicaller-0.4.1.0/shioajicaller/codes/__init__.py
--rw-r--r--   0        0        0     7573 2022-10-17 17:45:53.550806 shioajicaller-0.4.1.0/shioajicaller/codes/update.py
--rw-r--r--   0        0        0      636 2023-01-07 06:34:39.825269 shioajicaller-0.4.1.0/shioajicaller/config.py
--rw-r--r--   0        0        0       41 2021-10-04 14:25:31.896900 shioajicaller-0.4.1.0/shioajicaller/server/__init__.py
--rw-r--r--   0        0        0    32499 2023-04-23 04:06:14.056190 shioajicaller-0.4.1.0/shioajicaller/server/websocket.py
--rw-r--r--   0        0        0    23180 1970-01-01 00:00:00.000000 shioajicaller-0.4.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2021-07-18 10:36:07.309953 shioajicaller-0.4.1.1/LICENSE
+-rw-r--r--   0        0        0    21151 2023-04-23 03:55:56.545221 shioajicaller-0.4.1.1/README.md
+-rw-r--r--   0        0        0      671 2023-04-23 04:19:12.611118 shioajicaller-0.4.1.1/pyproject.toml
+-rw-r--r--   0        0        0       64 2023-01-07 06:34:39.824248 shioajicaller-0.4.1.1/shioajicaller/__init__.py
+-rw-r--r--   0        0        0    20163 2023-01-07 06:34:39.824583 shioajicaller-0.4.1.1/shioajicaller/caller.py
+-rw-r--r--   0        0        0     5631 2023-04-23 03:50:23.401077 shioajicaller-0.4.1.1/shioajicaller/cli/__init__.py
+-rw-r--r--   0        0        0       56 2021-07-22 10:56:11.854486 shioajicaller-0.4.1.1/shioajicaller/codes/__init__.py
+-rw-r--r--   0        0        0     7573 2022-10-17 17:45:53.550806 shioajicaller-0.4.1.1/shioajicaller/codes/update.py
+-rw-r--r--   0        0        0      636 2023-01-07 06:34:39.825269 shioajicaller-0.4.1.1/shioajicaller/config.py
+-rw-r--r--   0        0        0       41 2021-10-04 14:25:31.896900 shioajicaller-0.4.1.1/shioajicaller/server/__init__.py
+-rw-r--r--   0        0        0    32500 2023-04-23 04:17:11.097236 shioajicaller-0.4.1.1/shioajicaller/server/websocket.py
+-rw-r--r--   0        0        0    23180 1970-01-01 00:00:00.000000 shioajicaller-0.4.1.1/PKG-INFO
```

### Comparing `shioajicaller-0.4.1.0/LICENSE` & `shioajicaller-0.4.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shioajicaller-0.4.1.0/README.md` & `shioajicaller-0.4.1.1/README.md`

 * *Files identical despite different names*

### Comparing `shioajicaller-0.4.1.0/pyproject.toml` & `shioajicaller-0.4.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "shioajicaller"
-version = "0.4.1.0"
+version = "0.4.1.1"
 description = "shioaj warp caller"
 authors = ["Steve Lo <info@sd.idv.tw>"]
 license = "MIT"
 repository = "https://github.com/SDpower/shioajicaller"
 readme = ["README.md", "LICENSE"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 shioaji = {extras = ["speed"], version = "^1.1.0"}
 python-dotenv = "^0.19.0"
-redis = "^3.5.3"
+redis = "^4.5.4"
 websockets = "^10.0"
 gmqtt = "^0.6.10"
 orjson = "^3.8.0"
 uvloop = {version = "^0.17.0", platform = "linux"}
 
 [tool.poetry.dev-dependencies]
```

### Comparing `shioajicaller-0.4.1.0/shioajicaller/caller.py` & `shioajicaller-0.4.1.1/shioajicaller/caller.py`

 * *Files identical despite different names*

### Comparing `shioajicaller-0.4.1.0/shioajicaller/cli/__init__.py` & `shioajicaller-0.4.1.1/shioajicaller/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `shioajicaller-0.4.1.0/shioajicaller/codes/update.py` & `shioajicaller-0.4.1.1/shioajicaller/codes/update.py`

 * *Files identical despite different names*

### Comparing `shioajicaller-0.4.1.0/shioajicaller/config.py` & `shioajicaller-0.4.1.1/shioajicaller/config.py`

 * *Files identical despite different names*

### Comparing `shioajicaller-0.4.1.0/shioajicaller/server/websocket.py` & `shioajicaller-0.4.1.1/shioajicaller/server/websocket.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 import asyncio
-import redis.asyncio as redis
+import redis.asyncio.client as redis
 import os, sys, base64
 import logging
 import orjson
 import time
 import websockets
 from gmqtt import Client as MQTTClient
 import uvloop
@@ -78,15 +78,15 @@
 
         self._mqttClient.set_auth_credentials(mqttUser, mqttPassword)
         await self._mqttClient.connect(mqttHost, keepalive=30)
         await STOP.wait()
         await self._mqttClient.disconnect()
 
     def SetRedisConnection(self,redisHost: str,redisPort: int,redisDb: str):
-        self._redis = redis.StrictRedis(redisHost,redisPort,redisDb)
+        self._redis = redis.Redis(redisHost,redisPort,redisDb)
         logging.info(f"SetRedisConnections! {redisHost}:{redisPort}:{redisDb}")
 
     def OrderCallBack(self,*args):
         loop.call_soon_threadsafe(self._oderQueue.put_nowait, args)
 
     def TradeCallBack(self,**keyword_params):
         loop.call_soon_threadsafe(self._tradeQueue.put_nowait, keyword_params)
```

### Comparing `shioajicaller-0.4.1.0/PKG-INFO` & `shioajicaller-0.4.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shioajicaller
-Version: 0.4.1.0
+Version: 0.4.1.1
 Summary: shioaj warp caller
 Home-page: https://github.com/SDpower/shioajicaller
 License: MIT
 Author: Steve Lo
 Author-email: info@sd.idv.tw
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: gmqtt (>=0.6.10,<0.7.0)
 Requires-Dist: orjson (>=3.8.0,<4.0.0)
 Requires-Dist: python-dotenv (>=0.19.0,<0.20.0)
-Requires-Dist: redis (>=3.5.3,<4.0.0)
+Requires-Dist: redis (>=4.5.4,<5.0.0)
 Requires-Dist: shioaji[speed] (>=1.1.0,<2.0.0)
 Requires-Dist: uvloop (>=0.17.0,<0.18.0) ; sys_platform == "linux"
 Requires-Dist: websockets (>=10.0,<11.0)
 Project-URL: Repository, https://github.com/SDpower/shioajicaller
 Description-Content-Type: text/markdown
 
 Shioaji Warp Caller P.O.C project.
```

