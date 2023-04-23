# Comparing `tmp/micropython-async_websocket_client-0.1.9.tar.gz` & `tmp/micropython-async_websocket_client-0.2.0.tar.gz`

## Comparing `micropython-async_websocket_client-0.1.9.tar` & `micropython-async_websocket_client-0.2.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-rw-r--   0 vovaman   (1000) vovaman   (1000)       36 2022-02-17 19:11:37.000000 micropython-async_websocket_client-0.1.9/async_websocket_client/__init__.py
--rw-rw-r--   0 vovaman   (1000) vovaman   (1000)     7822 2023-03-05 17:19:34.000000 micropython-async_websocket_client-0.1.9/async_websocket_client/ws.py
--rw-rw-r--   0 vovaman   (1000) vovaman   (1000)     2867 2023-03-05 18:31:24.000000 micropython-async_websocket_client-0.1.9/micropython_async_websocket_client.egg-info/PKG-INFO
--rw-rw-r--   0 vovaman   (1000) vovaman   (1000)        9 2023-03-05 18:31:24.000000 micropython-async_websocket_client-0.1.9/micropython_async_websocket_client.egg-info/requires.txt
+-rw-rw-r--   0 vovaman   (1000) vovaman   (1000)       36 2022-02-17 19:11:37.000000 micropython-async_websocket_client-0.2.0/async_websocket_client/__init__.py
+-rw-rw-r--   0 vovaman   (1000) vovaman   (1000)     8041 2023-04-23 17:18:35.000000 micropython-async_websocket_client-0.2.0/async_websocket_client/ws.py
+-rw-rw-r--   0 vovaman   (1000) vovaman   (1000)     2953 2023-04-23 17:25:39.000000 micropython-async_websocket_client-0.2.0/micropython_async_websocket_client.egg-info/PKG-INFO
+-rw-rw-r--   0 vovaman   (1000) vovaman   (1000)        9 2023-04-23 17:25:39.000000 micropython-async_websocket_client-0.2.0/micropython_async_websocket_client.egg-info/requires.txt
```

### Comparing `micropython-async_websocket_client-0.1.9/async_websocket_client/ws.py` & `micropython-async_websocket_client-0.2.0/async_websocket_client/ws.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,19 +70,25 @@
         while line is None:
             line = self.sock.readline()
             await a.sleep_ms(self.delay_read)
 
         return line
 
     async def a_read(self, size: int = None):
-        b = None
-        while b is None:
+        chunks = []
+        while True:
             b = self.sock.read(size)
             await a.sleep_ms(self.delay_read)
-        return b
+            if b:
+                if (size is None or len(b) == size):
+                    return b
+                chunks.append(b)
+                size -= len(b)
+                if size == 0:
+                    return b''.join(chunks)
 
     async def handshake(self, uri, headers=[]):
         if self.sock:
             self.close()
 
         self.sock = socket.socket()
         self.uri = self.urlparse(uri)
```

### Comparing `micropython-async_websocket_client-0.1.9/micropython_async_websocket_client.egg-info/PKG-INFO` & `micropython-async_websocket_client-0.2.0/micropython_async_websocket_client.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython-async-websocket-client
-Version: 0.1.9
+Version: 0.2.0
 Summary: Asynchronous websocket client for ESP32 controller.
 Home-page: https://github.com/Vovaman/micropython_async_websocket_client
 Download-URL: https://github.com/Vovaman/micropython_async_websocket_client/releases
 Author: Vladimir Badashkin
 Author-email: bd_postbox1@mail.ru
 License: Apache License 2.0
 Keywords: ESP32,micropython,websocket,asynchronous,client
@@ -50,14 +50,19 @@
 ```
 
 All needed dependencies are in esp32-20220618-v1.19.1.bin.
 # example
 Sample using of this module is in https://github.com/Vovaman/example_async_websocket.
 
 
+0.2.0
+-----
+Fix for big data packet.
+Author: [mutatrum](https://github.com/mutatrum)
+
 0.1.9
 -----
 Method `close()` is added and example project (see link above) is changed
 to demonstrate it.
 
 0.1.8
 -----
```

