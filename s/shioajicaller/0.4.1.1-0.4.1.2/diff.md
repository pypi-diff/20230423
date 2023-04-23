# Comparing `tmp/shioajicaller-0.4.1.1.tar.gz` & `tmp/shioajicaller-0.4.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shioajicaller-0.4.1.1.tar", max compression
+gzip compressed data, was "shioajicaller-0.4.1.2.tar", max compression
```

## Comparing `shioajicaller-0.4.1.1.tar` & `shioajicaller-0.4.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1074 2021-07-18 10:36:07.309953 shioajicaller-0.4.1.1/LICENSE
--rw-r--r--   0        0        0    21151 2023-04-23 03:55:56.545221 shioajicaller-0.4.1.1/README.md
--rw-r--r--   0        0        0      671 2023-04-23 04:19:12.611118 shioajicaller-0.4.1.1/pyproject.toml
--rw-r--r--   0        0        0       64 2023-01-07 06:34:39.824248 shioajicaller-0.4.1.1/shioajicaller/__init__.py
--rw-r--r--   0        0        0    20163 2023-01-07 06:34:39.824583 shioajicaller-0.4.1.1/shioajicaller/caller.py
--rw-r--r--   0        0        0     5631 2023-04-23 03:50:23.401077 shioajicaller-0.4.1.1/shioajicaller/cli/__init__.py
--rw-r--r--   0        0        0       56 2021-07-22 10:56:11.854486 shioajicaller-0.4.1.1/shioajicaller/codes/__init__.py
--rw-r--r--   0        0        0     7573 2022-10-17 17:45:53.550806 shioajicaller-0.4.1.1/shioajicaller/codes/update.py
--rw-r--r--   0        0        0      636 2023-01-07 06:34:39.825269 shioajicaller-0.4.1.1/shioajicaller/config.py
--rw-r--r--   0        0        0       41 2021-10-04 14:25:31.896900 shioajicaller-0.4.1.1/shioajicaller/server/__init__.py
--rw-r--r--   0        0        0    32500 2023-04-23 04:17:11.097236 shioajicaller-0.4.1.1/shioajicaller/server/websocket.py
--rw-r--r--   0        0        0    23180 1970-01-01 00:00:00.000000 shioajicaller-0.4.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2021-07-18 10:36:07.309953 shioajicaller-0.4.1.2/LICENSE
+-rw-r--r--   0        0        0    21151 2023-04-23 03:55:56.545221 shioajicaller-0.4.1.2/README.md
+-rw-r--r--   0        0        0      671 2023-04-23 04:50:16.051088 shioajicaller-0.4.1.2/pyproject.toml
+-rw-r--r--   0        0        0       64 2023-01-07 06:34:39.824248 shioajicaller-0.4.1.2/shioajicaller/__init__.py
+-rw-r--r--   0        0        0    20163 2023-01-07 06:34:39.824583 shioajicaller-0.4.1.2/shioajicaller/caller.py
+-rw-r--r--   0        0        0     5631 2023-04-23 03:50:23.401077 shioajicaller-0.4.1.2/shioajicaller/cli/__init__.py
+-rw-r--r--   0        0        0       56 2021-07-22 10:56:11.854486 shioajicaller-0.4.1.2/shioajicaller/codes/__init__.py
+-rw-r--r--   0        0        0     7573 2022-10-17 17:45:53.550806 shioajicaller-0.4.1.2/shioajicaller/codes/update.py
+-rw-r--r--   0        0        0      636 2023-01-07 06:34:39.825269 shioajicaller-0.4.1.2/shioajicaller/config.py
+-rw-r--r--   0        0        0       41 2021-10-04 14:25:31.896900 shioajicaller-0.4.1.2/shioajicaller/server/__init__.py
+-rw-r--r--   0        0        0    32589 2023-04-23 04:47:27.727156 shioajicaller-0.4.1.2/shioajicaller/server/websocket.py
+-rw-r--r--   0        0        0    23180 1970-01-01 00:00:00.000000 shioajicaller-0.4.1.2/PKG-INFO
```

### Comparing `shioajicaller-0.4.1.1/LICENSE` & `shioajicaller-0.4.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `shioajicaller-0.4.1.1/README.md` & `shioajicaller-0.4.1.2/README.md`

 * *Files identical despite different names*

### Comparing `shioajicaller-0.4.1.1/pyproject.toml` & `shioajicaller-0.4.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shioajicaller"
-version = "0.4.1.1"
+version = "0.4.1.2"
 description = "shioaj warp caller"
 authors = ["Steve Lo <info@sd.idv.tw>"]
 license = "MIT"
 repository = "https://github.com/SDpower/shioajicaller"
 readme = ["README.md", "LICENSE"]
 
 [tool.poetry.dependencies]
```

### Comparing `shioajicaller-0.4.1.1/shioajicaller/caller.py` & `shioajicaller-0.4.1.2/shioajicaller/caller.py`

 * *Files identical despite different names*

### Comparing `shioajicaller-0.4.1.1/shioajicaller/cli/__init__.py` & `shioajicaller-0.4.1.2/shioajicaller/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `shioajicaller-0.4.1.1/shioajicaller/codes/update.py` & `shioajicaller-0.4.1.2/shioajicaller/codes/update.py`

 * *Files identical despite different names*

### Comparing `shioajicaller-0.4.1.1/shioajicaller/config.py` & `shioajicaller-0.4.1.2/shioajicaller/config.py`

 * *Files identical despite different names*

### Comparing `shioajicaller-0.4.1.1/shioajicaller/server/websocket.py` & `shioajicaller-0.4.1.2/shioajicaller/server/websocket.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 import asyncio
-import redis.asyncio.client as redis
+import redis.asyncio as redis
 import os, sys, base64
 import logging
 import orjson
 import time
 import websockets
 from gmqtt import Client as MQTTClient
 import uvloop
@@ -77,17 +77,18 @@
         logging.info(f"SetMqttConnection! {mqttHost} {mqttUser} {mqttPassword}")
 
         self._mqttClient.set_auth_credentials(mqttUser, mqttPassword)
         await self._mqttClient.connect(mqttHost, keepalive=30)
         await STOP.wait()
         await self._mqttClient.disconnect()
 
-    def SetRedisConnection(self,redisHost: str,redisPort: int,redisDb: str):
-        self._redis = redis.Redis(redisHost,redisPort,redisDb)
+    async def SetRedisConnection(self,redisHost: str,redisPort: int,redisDb: str):
+        self._redis = await redis.from_url(f'redis://{redisHost}:{redisPort}/{redisDb}')
         logging.info(f"SetRedisConnections! {redisHost}:{redisPort}:{redisDb}")
+        await self._redis.close()
 
     def OrderCallBack(self,*args):
         loop.call_soon_threadsafe(self._oderQueue.put_nowait, args)
 
     def TradeCallBack(self,**keyword_params):
         loop.call_soon_threadsafe(self._tradeQueue.put_nowait, keyword_params)
 
@@ -591,25 +592,25 @@
     except Exception as ex:
         print('Exception:', ex)
     return None
 
 def __start_wss_server(port:int=6789,callers:Caller=Caller(),pool_size:int=50,debug:int=logging.WARNING,
     with_redis:bool=False,redisHost:str=None,redisPort:int=6379,redisDb:str="0",
     with_mqtt:bool=False,mqttHost:str=None,mqttUser:str="",mqttPassword:str=""):
-    WebsocketsHandler.SetCallers(callers)
-    if with_redis:
-        WebsocketsHandler.SetRedisConnection(redisHost,redisPort,redisDb)
+    WebsocketsHandler.SetCallers(callers)    
     logger = logging.getLogger()
     logger.setLevel(debug)
     if debug == logging.DEBUG:
         loop.set_debug(True)
     task = None
     try:
         if with_mqtt:
             loop.create_task(WebsocketsHandler.SetMqttConnection(mqttHost,mqttUser,mqttPassword))
+        if with_redis:
+            loop.create_task(WebsocketsHandler.SetRedisConnection(redisHost,redisPort,redisDb))
         loop.create_task(WebsocketsHandler.EnevtWorker('EnevtWorker-1'))
         loop.create_task(WebsocketsHandler.OrderWorker('OrderWorker-1'))
         loop.create_task(WebsocketsHandler.TradeWorker('TradeWorker-1'))
         loop.create_task(WebsocketsHandler.CmdWorker('CmdWorker-1'))
         loop.create_task(WebsocketsHandler.SubscribeIndexsTickWorker('SubscribeIndexsTickWorker-1'))
         loop.create_task(WebsocketsHandler.SubscribeIndexsTickWorker('SubscribeIndexsTickWorker-2'))
```

### Comparing `shioajicaller-0.4.1.1/PKG-INFO` & `shioajicaller-0.4.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shioajicaller
-Version: 0.4.1.1
+Version: 0.4.1.2
 Summary: shioaj warp caller
 Home-page: https://github.com/SDpower/shioajicaller
 License: MIT
 Author: Steve Lo
 Author-email: info@sd.idv.tw
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

