# Comparing `tmp/aiocache-0.9.0.tar.gz` & `tmp/aiocache-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aiocache-0.9.0.tar", last modified: Tue Apr 24 20:52:29 2018, max compression
+gzip compressed data, was "dist/aiocache-0.9.1.tar", last modified: Thu Apr 26 22:46:11 2018, max compression
```

## Comparing `aiocache-0.9.0.tar` & `aiocache-0.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-04-24 20:52:29.000000 aiocache-0.9.0/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-04-24 20:52:29.000000 aiocache-0.9.0/aiocache/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-04-24 20:52:29.000000 aiocache-0.9.0/aiocache/backends/
--rw-r--r--   0 travis    (2000) travis    (2000)        0 2018-04-24 20:51:30.000000 aiocache-0.9.0/aiocache/backends/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)     5878 2018-04-24 20:51:30.000000 aiocache-0.9.0/aiocache/backends/memcached.py
--rw-r--r--   0 travis    (2000) travis    (2000)     4350 2018-04-24 20:51:30.000000 aiocache-0.9.0/aiocache/backends/memory.py
--rw-r--r--   0 travis    (2000) travis    (2000)     8328 2018-04-24 20:51:30.000000 aiocache-0.9.0/aiocache/backends/redis.py
--rw-r--r--   0 travis    (2000) travis    (2000)      848 2018-04-24 20:51:30.000000 aiocache-0.9.0/aiocache/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)       22 2018-04-24 20:51:30.000000 aiocache-0.9.0/aiocache/_version.py
--rw-r--r--   0 travis    (2000) travis    (2000)    18471 2018-04-24 20:51:30.000000 aiocache-0.9.0/aiocache/base.py
--rw-r--r--   0 travis    (2000) travis    (2000)    12297 2018-04-24 20:51:30.000000 aiocache-0.9.0/aiocache/decorators.py
--rw-r--r--   0 travis    (2000) travis    (2000)     4786 2018-04-24 20:51:30.000000 aiocache-0.9.0/aiocache/factory.py
--rw-r--r--   0 travis    (2000) travis    (2000)     6368 2018-04-24 20:51:30.000000 aiocache-0.9.0/aiocache/lock.py
--rw-r--r--   0 travis    (2000) travis    (2000)     3383 2018-04-24 20:51:30.000000 aiocache-0.9.0/aiocache/plugins.py
--rw-r--r--   0 travis    (2000) travis    (2000)     4879 2018-04-24 20:51:30.000000 aiocache-0.9.0/aiocache/serializers.py
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-04-24 20:52:29.000000 aiocache-0.9.0/aiocache.egg-info/
--rw-r--r--   0 travis    (2000) travis    (2000)      520 2018-04-24 20:52:29.000000 aiocache-0.9.0/aiocache.egg-info/PKG-INFO
--rw-r--r--   0 travis    (2000) travis    (2000)      467 2018-04-24 20:52:29.000000 aiocache-0.9.0/aiocache.egg-info/SOURCES.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        1 2018-04-24 20:52:29.000000 aiocache-0.9.0/aiocache.egg-info/dependency_links.txt
--rw-r--r--   0 travis    (2000) travis    (2000)      215 2018-04-24 20:52:29.000000 aiocache-0.9.0/aiocache.egg-info/requires.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        9 2018-04-24 20:52:29.000000 aiocache-0.9.0/aiocache.egg-info/top_level.txt
--rw-r--r--   0 travis    (2000) travis    (2000)     7446 2018-04-24 20:51:30.000000 aiocache-0.9.0/README.rst
--rw-r--r--   0 travis    (2000) travis    (2000)      252 2018-04-24 20:52:29.000000 aiocache-0.9.0/setup.cfg
--rw-r--r--   0 travis    (2000) travis    (2000)     1340 2018-04-24 20:51:30.000000 aiocache-0.9.0/setup.py
--rw-r--r--   0 travis    (2000) travis    (2000)      520 2018-04-24 20:52:29.000000 aiocache-0.9.0/PKG-INFO
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-04-26 22:46:11.000000 aiocache-0.9.1/
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-04-26 22:46:11.000000 aiocache-0.9.1/aiocache/
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-04-26 22:46:11.000000 aiocache-0.9.1/aiocache/backends/
+-rw-r--r--   0 travis    (2000) travis    (2000)        0 2018-04-26 22:45:26.000000 aiocache-0.9.1/aiocache/backends/__init__.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     5878 2018-04-26 22:45:26.000000 aiocache-0.9.1/aiocache/backends/memcached.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     4350 2018-04-26 22:45:26.000000 aiocache-0.9.1/aiocache/backends/memory.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     8475 2018-04-26 22:45:26.000000 aiocache-0.9.1/aiocache/backends/redis.py
+-rw-r--r--   0 travis    (2000) travis    (2000)      848 2018-04-26 22:45:26.000000 aiocache-0.9.1/aiocache/__init__.py
+-rw-r--r--   0 travis    (2000) travis    (2000)       22 2018-04-26 22:45:26.000000 aiocache-0.9.1/aiocache/_version.py
+-rw-r--r--   0 travis    (2000) travis    (2000)    18471 2018-04-26 22:45:26.000000 aiocache-0.9.1/aiocache/base.py
+-rw-r--r--   0 travis    (2000) travis    (2000)    12297 2018-04-26 22:45:26.000000 aiocache-0.9.1/aiocache/decorators.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     4786 2018-04-26 22:45:26.000000 aiocache-0.9.1/aiocache/factory.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     6368 2018-04-26 22:45:26.000000 aiocache-0.9.1/aiocache/lock.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     3383 2018-04-26 22:45:26.000000 aiocache-0.9.1/aiocache/plugins.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     4984 2018-04-26 22:45:26.000000 aiocache-0.9.1/aiocache/serializers.py
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-04-26 22:46:11.000000 aiocache-0.9.1/aiocache.egg-info/
+-rw-r--r--   0 travis    (2000) travis    (2000)      520 2018-04-26 22:46:11.000000 aiocache-0.9.1/aiocache.egg-info/PKG-INFO
+-rw-r--r--   0 travis    (2000) travis    (2000)      467 2018-04-26 22:46:11.000000 aiocache-0.9.1/aiocache.egg-info/SOURCES.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)        1 2018-04-26 22:46:11.000000 aiocache-0.9.1/aiocache.egg-info/dependency_links.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)      215 2018-04-26 22:46:11.000000 aiocache-0.9.1/aiocache.egg-info/requires.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)        9 2018-04-26 22:46:11.000000 aiocache-0.9.1/aiocache.egg-info/top_level.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)     7446 2018-04-26 22:45:26.000000 aiocache-0.9.1/README.rst
+-rw-r--r--   0 travis    (2000) travis    (2000)      252 2018-04-26 22:46:11.000000 aiocache-0.9.1/setup.cfg
+-rw-r--r--   0 travis    (2000) travis    (2000)     1340 2018-04-26 22:45:26.000000 aiocache-0.9.1/setup.py
+-rw-r--r--   0 travis    (2000) travis    (2000)      520 2018-04-26 22:46:11.000000 aiocache-0.9.1/PKG-INFO
```

### Comparing `aiocache-0.9.0/aiocache/backends/memcached.py` & `aiocache-0.9.1/aiocache/backends/memcached.py`

 * *Files identical despite different names*

### Comparing `aiocache-0.9.0/aiocache/backends/memory.py` & `aiocache-0.9.1/aiocache/backends/memory.py`

 * *Files identical despite different names*

### Comparing `aiocache-0.9.0/aiocache/backends/redis.py` & `aiocache-0.9.1/aiocache/backends/redis.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,18 +58,24 @@
         self.endpoint = endpoint
         self.port = port
         self.db = db
         self.password = password
         self.pool_min_size = pool_min_size
         self.pool_max_size = pool_max_size
         self.create_connection_timeout = create_connection_timeout
-        self._pool_lock = asyncio.Lock()
+        self.__pool_lock = None
         self._loop = loop
         self._pool = None
 
+    @property
+    def _pool_lock(self):
+        if self.__pool_lock is None:
+            self.__pool_lock = asyncio.Lock()
+        return self.__pool_lock
+
     async def acquire_conn(self):
         await self._get_pool()
         conn = await self._pool.acquire()
         if not AIOREDIS_BEFORE_ONE:
             conn = aioredis.Redis(conn)
         return conn
```

### Comparing `aiocache-0.9.0/aiocache/__init__.py` & `aiocache-0.9.1/aiocache/__init__.py`

 * *Files identical despite different names*

### Comparing `aiocache-0.9.0/aiocache/base.py` & `aiocache-0.9.1/aiocache/base.py`

 * *Files identical despite different names*

### Comparing `aiocache-0.9.0/aiocache/decorators.py` & `aiocache-0.9.1/aiocache/decorators.py`

 * *Files identical despite different names*

### Comparing `aiocache-0.9.0/aiocache/factory.py` & `aiocache-0.9.1/aiocache/factory.py`

 * *Files identical despite different names*

### Comparing `aiocache-0.9.0/aiocache/lock.py` & `aiocache-0.9.1/aiocache/lock.py`

 * *Files identical despite different names*

### Comparing `aiocache-0.9.0/aiocache/plugins.py` & `aiocache-0.9.1/aiocache/plugins.py`

 * *Files identical despite different names*

### Comparing `aiocache-0.9.0/aiocache/serializers.py` & `aiocache-0.9.1/aiocache/serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 import logging
 import pickle
-import msgpack
 
 logger = logging.getLogger(__file__)
 
 try:
     import ujson as json
 except ImportError:
     logger.warning("ujson module not found, using json")
     import json
 
+try:
+    import msgpack
+except ImportError:
+    logger.warning("msgpack not installed, MsgPackSerializer unavailable")
+
 
 _NOT_SET = object()
 
 
 class BaseSerializer:
 
     DEFAULT_ENCODING = 'utf-8'
```

### Comparing `aiocache-0.9.0/aiocache.egg-info/PKG-INFO` & `aiocache-0.9.1/aiocache.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: aiocache
-Version: 0.9.0
+Version: 0.9.1
 Summary: multi backend asyncio cache
 Home-page: https://github.com/argaen/aiocache
 Author: Manuel Miranda
 Author-email: manu.mirandad@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Framework :: AsyncIO
-Provides-Extra: memcached
+Provides-Extra: dev
 Provides-Extra: redis
+Provides-Extra: memcached
 Provides-Extra: msgpack
-Provides-Extra: dev
```

### Comparing `aiocache-0.9.0/README.rst` & `aiocache-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `aiocache-0.9.0/setup.py` & `aiocache-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `aiocache-0.9.0/PKG-INFO` & `aiocache-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: aiocache
-Version: 0.9.0
+Version: 0.9.1
 Summary: multi backend asyncio cache
 Home-page: https://github.com/argaen/aiocache
 Author: Manuel Miranda
 Author-email: manu.mirandad@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Framework :: AsyncIO
-Provides-Extra: memcached
+Provides-Extra: dev
 Provides-Extra: redis
+Provides-Extra: memcached
 Provides-Extra: msgpack
-Provides-Extra: dev
```

