# Comparing `tmp/wizcli-0.1.2.tar.gz` & `tmp/wizcli-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wizcli-0.1.2.tar", max compression
+gzip compressed data, was "wizcli-0.1.3.tar", max compression
```

## Comparing `wizcli-0.1.2.tar` & `wizcli-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      247 2023-04-22 05:19:10.102030 wizcli-0.1.2/README.md
--rw-r--r--   0        0        0      327 2023-04-22 05:36:55.487794 wizcli-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1479 2023-04-22 05:36:26.730516 wizcli-0.1.2/wizcli/cli.py
--rw-r--r--   0        0        0     2187 2023-04-22 04:37:46.764498 wizcli-0.1.2/wizcli/wiz.py
--rw-r--r--   0        0        0      719 1970-01-01 00:00:00.000000 wizcli-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      247 2023-04-22 05:19:10.102030 wizcli-0.1.3/README.md
+-rw-r--r--   0        0        0      327 2023-04-23 16:34:27.806299 wizcli-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2156 2023-04-23 16:33:35.335768 wizcli-0.1.3/wizcli/cli.py
+-rw-r--r--   0        0        0     2423 2023-04-23 16:31:09.469519 wizcli-0.1.3/wizcli/wiz.py
+-rw-r--r--   0        0        0      719 1970-01-01 00:00:00.000000 wizcli-0.1.3/PKG-INFO
```

### Comparing `wizcli-0.1.2/wizcli/cli.py` & `wizcli-0.1.3/wizcli/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,38 @@
+import math
 from dataclasses import dataclass
+
 import typer
 from .wiz import Wiz
 
 run = typer.Typer()
 
 @dataclass
 class State:
     wiz: Wiz
     verbose: bool
 
 
 @run.callback()
 def common(
     ctx: typer.Context,
-    host: str = typer.Option(None, "--host", "-h", envvar="WIZ_HOST"),
-    port: int = 38899,
+    host: str = typer.Option(None, "--host", "-h", envvar="WIZ_HOST", help="WiZ bulb host"),
+    port: int = typer.Option(38899, "--port", "-p", envvar="WIZ_PORT", help="WiZ bulb port"),
+    timeout: int = typer.Option(5, "--timeout", "-t", envvar="WIZ_TIMEOUT", help="Timeout in seconds"),
     verbose: bool = typer.Option(False, "--verbose", "-v"),
 ):
     if not host:
         print("Missing host.")
         raise typer.Abort()
 
     if verbose:
         typer.echo(f"WiZ {host=} {port=}")
 
     ctx.obj = State(
-        wiz=Wiz(host, port),
+        wiz=Wiz(host, port, timeout=timeout),
         verbose=verbose
     )
 
 
 @run.command()
 def on(ctx: typer.Context):
     ctx.obj.wiz.on()
@@ -37,45 +40,63 @@
 
 @run.command()
 def off(ctx: typer.Context):
     ctx.obj.wiz.off()
 
 
 @run.command()
+def switch(ctx: typer.Context):
+    state = ctx.obj.wiz.get_state()
+    if state["state"]:
+        ctx.obj.wiz.off()
+    else:
+        ctx.obj.wiz.on()
+
+
+@run.command()
 def dim(
     ctx: typer.Context,
-    value: int = typer.Argument(50, min=0, max=100),
+    value: int = typer.Argument(50, min=0, max=100, help="%"),
 ):
+    value = math.floor(value / 100 * 255)
     ctx.obj.wiz.set_brightness(value)
 
 
 @run.command()
 def temp(
     ctx: typer.Context,
-    value: int = typer.Argument(None, min=0, max=100),
+    value: int = typer.Argument(50, min=0, max=100, help="%"),
 ):
-    kelvin = value * (6500 - 2200) // 100 + 2200
-    ctx.obj.wiz.set_temp(kelvin)
+    k = math.floor(value * (6500 - 2200) / 100 + 2200)
+    ctx.obj.wiz.set_temp(k)
 
 
 @run.command()
-def hot(ctx: typer.Context):
-    ctx.obj.wiz.set_temp(2200)
+def warm(
+    ctx: typer.Context,
+    value: int = typer.Argument(100, min=0, max=100, help="%"),
+):
+    value = math.floor(value / 100 * 255)
+    ctx.obj.wiz.set_warm(value)
 
 
 @run.command()
-def cold(ctx: typer.Context):
-    ctx.obj.wiz.set_temp(6500)
+def cold(
+    ctx: typer.Context,
+    value: int = typer.Argument(100, min=0, max=100, help="%"),
+):
+    value = math.floor(value / 100 * 255)
+    ctx.obj.wiz.set_cold(value)
 
 
 @run.command()
 def rgb(
     ctx: typer.Context,
-    r: int = typer.Argument(None, min=0, max=255),
-    g: int = typer.Argument(None, min=0, max=255),
-    b: int = typer.Argument(None, min=0, max=255),
+    r: int = typer.Argument(0, min=0, max=255),
+    g: int = typer.Argument(0, min=0, max=255),
+    b: int = typer.Argument(0, min=0, max=255),
 ):
     ctx.obj.wiz.set_color((r, g, b))
 
 
 if __name__ == "__main__":
     run()
```

### Comparing `wizcli-0.1.2/wizcli/wiz.py` & `wizcli-0.1.3/wizcli/wiz.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 import socket
 from collections import deque
 
 
 class Wiz:
     STATE_FIELDS = ("r", "g", "b", "c", "w", "dimming", "temp")
 
-    def __init__(self, host: str, port: int = 38899):
+    def __init__(self, host: str, port: int = 38899, timeout: int = 5):
         self.host = host
         self.port = port
         self.socket = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
-        self.socket.settimeout(2)
+        self.socket.settimeout(timeout)
         self._states = deque()
 
     def __enter__(self):
         self.push_state()
         return self
 
     def __exit__(self, *args, **kwargs):
@@ -55,14 +55,20 @@
 
     def set_brightness(self, value):
         return self._send({"method": "setPilot", "params": {"dimming": value}})
 
     def set_temp(self, value):
         return self._send({"method": "setPilot", "params": {"temp": value}})
 
+    def set_warm(self, value):
+        return self._send({"method": "setPilot", "params": {"w": value}})
+
+    def set_cold(self, value):
+        return self._send({"method": "setPilot", "params": {"c": value}})
+
     def push_state(self):
         """push state to the queue"""
         state = self.get_state()
         self._states.append(state)
 
     def pop_state(self):
         try:
```

### Comparing `wizcli-0.1.2/PKG-INFO` & `wizcli-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wizcli
-Version: 0.1.2
+Version: 0.1.3
 Summary: wiz cli
 Author: Agustin B
 Author-email: redraw@sdf.org
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

