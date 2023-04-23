# Comparing `tmp/shioajicaller-0.4.0.0.tar.gz` & `tmp/shioajicaller-0.4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shioajicaller-0.4.0.0.tar", max compression
+gzip compressed data, was "shioajicaller-0.4.1.0.tar", max compression
```

## Comparing `shioajicaller-0.4.0.0.tar` & `shioajicaller-0.4.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1074 2021-07-18 10:36:07.309953 shioajicaller-0.4.0.0/LICENSE
--rw-r--r--   0        0        0      600 2023-01-07 06:34:39.823964 shioajicaller-0.4.0.0/pyproject.toml
--rw-r--r--   0        0        0       64 2023-01-07 06:34:39.824248 shioajicaller-0.4.0.0/shioajicaller/__init__.py
--rw-r--r--   0        0        0    20163 2023-01-07 06:34:39.824583 shioajicaller-0.4.0.0/shioajicaller/caller.py
--rw-r--r--   0        0        0     5631 2023-01-07 06:34:39.824896 shioajicaller-0.4.0.0/shioajicaller/cli/__init__.py
--rw-r--r--   0        0        0       56 2021-07-22 10:56:11.854486 shioajicaller-0.4.0.0/shioajicaller/codes/__init__.py
--rw-r--r--   0        0        0     7573 2022-10-17 17:45:53.550806 shioajicaller-0.4.0.0/shioajicaller/codes/update.py
--rw-r--r--   0        0        0      636 2023-01-07 06:34:39.825269 shioajicaller-0.4.0.0/shioajicaller/config.py
--rw-r--r--   0        0        0       41 2021-10-04 14:25:31.896900 shioajicaller-0.4.0.0/shioajicaller/server/__init__.py
--rw-r--r--   0        0        0    32644 2023-01-04 16:26:39.812163 shioajicaller-0.4.0.0/shioajicaller/server/websocket.py
--rw-r--r--   0        0        0     1078 1970-01-01 00:00:00.000000 shioajicaller-0.4.0.0/setup.py
--rw-r--r--   0        0        0      828 1970-01-01 00:00:00.000000 shioajicaller-0.4.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2021-07-18 10:36:07.309953 shioajicaller-0.4.1.0/LICENSE
+-rw-r--r--   0        0        0    21151 2023-04-23 03:55:56.545221 shioajicaller-0.4.1.0/README.md
+-rw-r--r--   0        0        0      671 2023-04-23 04:03:17.620627 shioajicaller-0.4.1.0/pyproject.toml
+-rw-r--r--   0        0        0       64 2023-01-07 06:34:39.824248 shioajicaller-0.4.1.0/shioajicaller/__init__.py
+-rw-r--r--   0        0        0    20163 2023-01-07 06:34:39.824583 shioajicaller-0.4.1.0/shioajicaller/caller.py
+-rw-r--r--   0        0        0     5631 2023-04-23 03:50:23.401077 shioajicaller-0.4.1.0/shioajicaller/cli/__init__.py
+-rw-r--r--   0        0        0       56 2021-07-22 10:56:11.854486 shioajicaller-0.4.1.0/shioajicaller/codes/__init__.py
+-rw-r--r--   0        0        0     7573 2022-10-17 17:45:53.550806 shioajicaller-0.4.1.0/shioajicaller/codes/update.py
+-rw-r--r--   0        0        0      636 2023-01-07 06:34:39.825269 shioajicaller-0.4.1.0/shioajicaller/config.py
+-rw-r--r--   0        0        0       41 2021-10-04 14:25:31.896900 shioajicaller-0.4.1.0/shioajicaller/server/__init__.py
+-rw-r--r--   0        0        0    32499 2023-04-23 04:06:14.056190 shioajicaller-0.4.1.0/shioajicaller/server/websocket.py
+-rw-r--r--   0        0        0    23180 1970-01-01 00:00:00.000000 shioajicaller-0.4.1.0/PKG-INFO
```

### Comparing `shioajicaller-0.4.0.0/LICENSE` & `shioajicaller-0.4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shioajicaller-0.4.0.0/shioajicaller/caller.py` & `shioajicaller-0.4.1.0/shioajicaller/caller.py`

 * *Files identical despite different names*

### Comparing `shioajicaller-0.4.0.0/shioajicaller/cli/__init__.py` & `shioajicaller-0.4.1.0/shioajicaller/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `shioajicaller-0.4.0.0/shioajicaller/codes/update.py` & `shioajicaller-0.4.1.0/shioajicaller/codes/update.py`

 * *Files identical despite different names*

### Comparing `shioajicaller-0.4.0.0/shioajicaller/config.py` & `shioajicaller-0.4.1.0/shioajicaller/config.py`

 * *Files identical despite different names*

### Comparing `shioajicaller-0.4.0.0/shioajicaller/server/websocket.py` & `shioajicaller-0.4.1.0/shioajicaller/server/websocket.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 import asyncio
-import aioredis
+import redis.asyncio as redis
 import os, sys, base64
 import logging
 import orjson
 import time
 import websockets
 from gmqtt import Client as MQTTClient
 import uvloop
@@ -78,22 +78,15 @@
 
         self._mqttClient.set_auth_credentials(mqttUser, mqttPassword)
         await self._mqttClient.connect(mqttHost, keepalive=30)
         await STOP.wait()
         await self._mqttClient.disconnect()
 
     def SetRedisConnection(self,redisHost: str,redisPort: int,redisDb: str):
-        self._redis = aioredis.Redis(
-            host=redisHost,
-            port=redisPort,
-            db=redisDb,
-            encoding="utf-8",
-            decode_responses=True,
-            socket_keepalive=True,
-        )
+        self._redis = redis.StrictRedis(redisHost,redisPort,redisDb)
         logging.info(f"SetRedisConnections! {redisHost}:{redisPort}:{redisDb}")
 
     def OrderCallBack(self,*args):
         loop.call_soon_threadsafe(self._oderQueue.put_nowait, args)
 
     def TradeCallBack(self,**keyword_params):
         loop.call_soon_threadsafe(self._tradeQueue.put_nowait, keyword_params)
```

