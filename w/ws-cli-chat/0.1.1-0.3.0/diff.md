# Comparing `tmp/ws_cli_chat-0.1.1.tar.gz` & `tmp/ws_cli_chat-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ws_cli_chat-0.1.1.tar", max compression
+gzip compressed data, was "ws_cli_chat-0.3.0.tar", max compression
```

## Comparing `ws_cli_chat-0.1.1.tar` & `ws_cli_chat-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      516 2023-04-22 08:06:37.903046 ws_cli_chat-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1560 2023-04-22 08:02:07.727156 ws_cli_chat-0.1.1/README.md
--rw-r--r--   0        0        0       39 2023-04-22 08:07:02.777152 ws_cli_chat-0.1.1/ws_cli_chat/__init__.py
--rw-r--r--   0        0        0       75 2023-04-22 08:02:07.761667 ws_cli_chat-0.1.1/ws_cli_chat/__main__.py
--rw-r--r--   0        0        0     1223 2023-04-22 08:04:21.778790 ws_cli_chat-0.1.1/ws_cli_chat/cli_chat.py
--rw-r--r--   0        0        0     1364 2023-04-22 06:01:21.192473 ws_cli_chat-0.1.1/ws_cli_chat/console.py
--rw-r--r--   0        0        0     2009 1970-01-01 00:00:00.000000 ws_cli_chat-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      582 2023-04-23 22:33:42.738783 ws_cli_chat-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1560 2023-04-22 08:02:07.727156 ws_cli_chat-0.3.0/README.md
+-rw-r--r--   0        0        0       96 2023-04-23 09:47:35.825879 ws_cli_chat-0.3.0/ws_cli_chat/__init__.py
+-rw-r--r--   0        0        0     3330 2023-04-23 22:16:18.013487 ws_cli_chat-0.3.0/ws_cli_chat/cli_chat.py
+-rw-r--r--   0        0        0     2899 2023-04-23 22:10:57.634176 ws_cli_chat-0.3.0/ws_cli_chat/myconsole.py
+-rw-r--r--   0        0        0      756 2023-04-23 10:55:22.188379 ws_cli_chat-0.3.0/ws_cli_chat/render.py
+-rw-r--r--   0        0        0     2142 1970-01-01 00:00:00.000000 ws_cli_chat-0.3.0/PKG-INFO
```

### Comparing `ws_cli_chat-0.1.1/README.md` & `ws_cli_chat-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ws_cli_chat-0.1.1/PKG-INFO` & `ws_cli_chat-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: ws-cli-chat
-Version: 0.1.1
+Version: 0.3.0
 Summary: simple cli-websocket-ws-cli-chat
 Author: __coelho__
 Author-email: 109885900+MikalROn@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: colorama (>=0.4.6,<0.5.0)
+Requires-Dist: eventsimplegui (>=0.3.0,<0.4.0)
+Requires-Dist: pysimplegui (>=4.60.4,<5.0.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Requires-Dist: websockets (>=11.0.2,<12.0.0)
 Description-Content-Type: text/markdown
 
 # Chat Application
 This is a command-line chat application built with Python that allows users to connect to a websocket server and chat with other users in real-time.
```

