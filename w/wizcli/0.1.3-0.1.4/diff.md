# Comparing `tmp/wizcli-0.1.3.tar.gz` & `tmp/wizcli-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wizcli-0.1.3.tar", max compression
+gzip compressed data, was "wizcli-0.1.4.tar", max compression
```

## Comparing `wizcli-0.1.3.tar` & `wizcli-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      247 2023-04-22 05:19:10.102030 wizcli-0.1.3/README.md
--rw-r--r--   0        0        0      327 2023-04-23 16:34:27.806299 wizcli-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2156 2023-04-23 16:33:35.335768 wizcli-0.1.3/wizcli/cli.py
--rw-r--r--   0        0        0     2423 2023-04-23 16:31:09.469519 wizcli-0.1.3/wizcli/wiz.py
--rw-r--r--   0        0        0      719 1970-01-01 00:00:00.000000 wizcli-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      247 2023-04-22 05:19:10.102030 wizcli-0.1.4/README.md
+-rw-r--r--   0        0        0      327 2023-04-23 17:21:18.962177 wizcli-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2233 2023-04-23 17:21:08.316888 wizcli-0.1.4/wizcli/cli.py
+-rw-r--r--   0        0        0     2444 2023-04-23 17:17:48.394456 wizcli-0.1.4/wizcli/wiz.py
+-rw-r--r--   0        0        0      719 1970-01-01 00:00:00.000000 wizcli-0.1.4/PKG-INFO
```

### Comparing `wizcli-0.1.3/wizcli/wiz.py` & `wizcli-0.1.4/wizcli/wiz.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,15 @@
-import sys
 import json
 import socket
+import logging
+from pprint import pformat
 from collections import deque
 
+logger = logging.getLogger(__name__)
+
 
 class Wiz:
     STATE_FIELDS = ("r", "g", "b", "c", "w", "dimming", "temp")
 
     def __init__(self, host: str, port: int = 38899, timeout: int = 5):
         self.host = host
         self.port = port
@@ -15,34 +18,34 @@
         self._states = deque()
 
     def __enter__(self):
         self.push_state()
         return self
 
     def __exit__(self, *args, **kwargs):
-        print("Restoring WiZ state...")
+        logger.info("Restoring WiZ state...")
         self.pop_state()
 
     def _send(self, payload: dict) -> dict:
         body = json.dumps(payload)
         addr = (self.host, self.port)
 
+        logger.debug(f" > {pformat(payload)}")
         self.socket.sendto(body.encode("utf8"), addr)
 
         try:
-            resp_content, resp_addr = self.socket.recvfrom(4096)
-        except socket.timeout:
-            print("wiz bulb timeout", file=sys.stderr)
-            return {}
-
-        if not resp_content or addr != resp_addr:
-            print(f"{addr=} != {resp_addr} - {resp_content=}", file=sys.stderr)
-            return {}
+            content, _ = self.socket.recvfrom(4096)
+        except socket.timeout as e:
+            logger.error("wiz bulb timeout")
+            raise e
+
+        response = json.loads(content)
+        logger.debug(f" < {pformat(response)}")
 
-        return json.loads(resp_content)
+        return response
 
     def get_state(self) -> dict:
         return self._send({"method": "getPilot"}).get("result")
 
     def on(self):
         return self._send({"method": "setPilot", "params": {"state": True}})
```

### Comparing `wizcli-0.1.3/PKG-INFO` & `wizcli-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wizcli
-Version: 0.1.3
+Version: 0.1.4
 Summary: wiz cli
 Author: Agustin B
 Author-email: redraw@sdf.org
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

