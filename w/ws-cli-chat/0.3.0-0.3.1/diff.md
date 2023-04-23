# Comparing `tmp/ws_cli_chat-0.3.0.tar.gz` & `tmp/ws_cli_chat-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ws_cli_chat-0.3.0.tar", max compression
+gzip compressed data, was "ws_cli_chat-0.3.1.tar", max compression
```

## Comparing `ws_cli_chat-0.3.0.tar` & `ws_cli_chat-0.3.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      582 2023-04-23 22:33:42.738783 ws_cli_chat-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1560 2023-04-22 08:02:07.727156 ws_cli_chat-0.3.0/README.md
--rw-r--r--   0        0        0       96 2023-04-23 09:47:35.825879 ws_cli_chat-0.3.0/ws_cli_chat/__init__.py
--rw-r--r--   0        0        0     3330 2023-04-23 22:16:18.013487 ws_cli_chat-0.3.0/ws_cli_chat/cli_chat.py
--rw-r--r--   0        0        0     2899 2023-04-23 22:10:57.634176 ws_cli_chat-0.3.0/ws_cli_chat/myconsole.py
--rw-r--r--   0        0        0      756 2023-04-23 10:55:22.188379 ws_cli_chat-0.3.0/ws_cli_chat/render.py
--rw-r--r--   0        0        0     2142 1970-01-01 00:00:00.000000 ws_cli_chat-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      582 2023-04-23 22:38:57.030007 ws_cli_chat-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1560 2023-04-22 08:02:07.727156 ws_cli_chat-0.3.1/README.md
+-rw-r--r--   0        0        0       43 2023-04-23 22:38:40.233412 ws_cli_chat-0.3.1/ws_cli_chat/__init__.py
+-rw-r--r--   0        0        0     3283 2023-04-23 22:38:40.250507 ws_cli_chat-0.3.1/ws_cli_chat/cli_chat.py
+-rw-r--r--   0        0        0     2901 2023-04-23 22:38:40.280494 ws_cli_chat-0.3.1/ws_cli_chat/myconsole.py
+-rw-r--r--   0        0        0      775 2023-04-23 22:38:40.265970 ws_cli_chat-0.3.1/ws_cli_chat/render.py
+-rw-r--r--   0        0        0     2142 1970-01-01 00:00:00.000000 ws_cli_chat-0.3.1/PKG-INFO
```

### Comparing `ws_cli_chat-0.3.0/pyproject.toml` & `ws_cli_chat-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ws_cli_chat"
-version = "0.3.0"
+version = "0.3.1"
 description = "simple cli-websocket-ws-cli-chat"
 authors = ["__coelho__ <109885900+MikalROn@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "ws_cli_chat"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `ws_cli_chat-0.3.0/README.md` & `ws_cli_chat-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `ws_cli_chat-0.3.0/ws_cli_chat/cli_chat.py` & `ws_cli_chat-0.3.1/ws_cli_chat/cli_chat.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import threading
 import websockets
 import asyncio
 import typer
 import PySimpleGUI as sg
 from pysimpleevent import EventSimpleGUI
-from render import SequestraConsole
 from typing import Optional
-from myconsole import MyConsole
+from ws_cli_chat.myconsole import MyConsole
+
 
-s = SequestraConsole()
 app = typer.Typer()
 MESSAGES: list[str] = []
 
 
 def rederizar_menssagens(lista_menssagens: list) -> None:
     MyConsole.clear()
     [print(menssagen) for menssagen in lista_menssagens]
```

### Comparing `ws_cli_chat-0.3.0/ws_cli_chat/myconsole.py` & `ws_cli_chat-0.3.1/ws_cli_chat/myconsole.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import sys
 import subprocess
 from rich.console import Console
 
+
 console = Console(record=True)
 
 
 
 class MyConsole:
```

### Comparing `ws_cli_chat-0.3.0/ws_cli_chat/render.py` & `ws_cli_chat-0.3.1/ws_cli_chat/render.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import io
 import sys
 
+# Codigo legado
+
 
 class SequestraConsole:
     def __init__(self):
         self.ultima_linha: list = []
 
     def sequestar_console(self):
         def decorator(func):
```

### Comparing `ws_cli_chat-0.3.0/PKG-INFO` & `ws_cli_chat-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ws-cli-chat
-Version: 0.3.0
+Version: 0.3.1
 Summary: simple cli-websocket-ws-cli-chat
 Author: __coelho__
 Author-email: 109885900+MikalROn@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

