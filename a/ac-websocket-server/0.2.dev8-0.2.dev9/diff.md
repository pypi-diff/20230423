# Comparing `tmp/ac-websocket-server-0.2.dev8.tar.gz` & `tmp/ac-websocket-server-0.2.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ac-websocket-server-0.2.dev8.tar", last modified: Thu Mar  9 22:55:54 2023, max compression
+gzip compressed data, was "ac-websocket-server-0.2.dev9.tar", last modified: Mon Mar 20 03:06:26 2023, max compression
```

## Comparing `ac-websocket-server-0.2.dev8.tar` & `ac-websocket-server-0.2.dev9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-03-09 22:55:54.352716 ac-websocket-server-0.2.dev8/
--rw-r--r--   0 mark       (501) staff       (20)     4939 2023-03-09 22:55:54.352509 ac-websocket-server-0.2.dev8/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)     4672 2022-11-14 11:13:56.000000 ac-websocket-server-0.2.dev8/README.md
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-03-09 22:55:54.334519 ac-websocket-server-0.2.dev8/ac_websocket_client/
--rw-r--r--   0 mark       (501) staff       (20)       51 2022-12-22 06:43:00.000000 ac-websocket-server-0.2.dev8/ac_websocket_client/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)     1467 2022-12-22 06:43:00.000000 ac-websocket-server-0.2.dev8/ac_websocket_client/__main__.py
--rw-r--r--   0 mark       (501) staff       (20)    21465 2023-03-05 22:27:25.000000 ac-websocket-server-0.2.dev8/ac_websocket_client/app.py
--rw-r--r--   0 mark       (501) staff       (20)     4350 2022-12-21 22:24:54.000000 ac-websocket-server-0.2.dev8/ac_websocket_client/objects.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-03-09 22:55:54.343654 ac-websocket-server-0.2.dev8/ac_websocket_server/
--rw-r--r--   0 mark       (501) staff       (20)      264 2022-09-02 03:43:49.000000 ac-websocket-server-0.2.dev8/ac_websocket_server/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)     1701 2022-11-14 11:13:56.000000 ac-websocket-server-0.2.dev8/ac_websocket_server/__main__.py
--rw-r--r--   0 mark       (501) staff       (20)    10231 2023-02-12 22:42:19.000000 ac-websocket-server-0.2.dev8/ac_websocket_server/child.py
--rw-r--r--   0 mark       (501) staff       (20)     2684 2022-11-15 11:34:40.000000 ac-websocket-server-0.2.dev8/ac_websocket_server/connection.py
--rw-r--r--   0 mark       (501) staff       (20)      132 2023-03-09 22:55:39.000000 ac-websocket-server-0.2.dev8/ac_websocket_server/constants.py
--rw-r--r--   0 mark       (501) staff       (20)      530 2022-09-02 03:43:49.000000 ac-websocket-server-0.2.dev8/ac_websocket_server/debug.py
--rw-r--r--   0 mark       (501) staff       (20)     7594 2023-03-09 22:54:14.000000 ac-websocket-server-0.2.dev8/ac_websocket_server/entries.py
--rw-r--r--   0 mark       (501) staff       (20)      148 2022-09-02 03:43:49.000000 ac-websocket-server-0.2.dev8/ac_websocket_server/error.py
--rw-r--r--   0 mark       (501) staff       (20)     9242 2023-02-19 02:33:16.000000 ac-websocket-server-0.2.dev8/ac_websocket_server/game.py
--rw-r--r--   0 mark       (501) staff       (20)     3640 2022-11-15 11:34:40.000000 ac-websocket-server-0.2.dev8/ac_websocket_server/grid.py
--rw-r--r--   0 mark       (501) staff       (20)     1441 2023-03-05 22:27:25.000000 ac-websocket-server-0.2.dev8/ac_websocket_server/handlers.py
--rw-r--r--   0 mark       (501) staff       (20)     2480 2022-11-15 11:34:40.000000 ac-websocket-server-0.2.dev8/ac_websocket_server/lobby.py
--rw-r--r--   0 mark       (501) staff       (20)     2939 2023-02-13 04:44:51.000000 ac-websocket-server-0.2.dev8/ac_websocket_server/objects.py
--rw-r--r--   0 mark       (501) staff       (20)     3389 2022-10-14 06:35:28.000000 ac-websocket-server-0.2.dev8/ac_websocket_server/observer.py
--rw-r--r--   0 mark       (501) staff       (20)      957 2022-09-04 08:46:38.000000 ac-websocket-server-0.2.dev8/ac_websocket_server/protocol.py
--rw-r--r--   0 mark       (501) staff       (20)     4399 2023-03-05 22:28:02.000000 ac-websocket-server-0.2.dev8/ac_websocket_server/server.py
--rw-r--r--   0 mark       (501) staff       (20)     1777 2022-09-02 03:38:58.000000 ac-websocket-server-0.2.dev8/ac_websocket_server/task_logger.py
--rw-r--r--   0 mark       (501) staff       (20)     2694 2023-03-05 22:28:02.000000 ac-websocket-server-0.2.dev8/ac_websocket_server/tracker.py
--rw-r--r--   0 mark       (501) staff       (20)     8063 2023-01-08 22:03:02.000000 ac-websocket-server-0.2.dev8/ac_websocket_server/watcher.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-03-09 22:55:54.347681 ac-websocket-server-0.2.dev8/ac_websocket_server.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)     4939 2023-03-09 22:55:54.000000 ac-websocket-server-0.2.dev8/ac_websocket_server.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      942 2023-03-09 22:55:54.000000 ac-websocket-server-0.2.dev8/ac_websocket_server.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-03-09 22:55:54.000000 ac-websocket-server-0.2.dev8/ac_websocket_server.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)       35 2023-03-09 22:55:54.000000 ac-websocket-server-0.2.dev8/ac_websocket_server.egg-info/requires.txt
--rw-r--r--   0 mark       (501) staff       (20)       40 2023-03-09 22:55:54.000000 ac-websocket-server-0.2.dev8/ac_websocket_server.egg-info/top_level.txt
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-03-09 22:55:54.352766 ac-websocket-server-0.2.dev8/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)      729 2022-11-06 00:50:25.000000 ac-websocket-server-0.2.dev8/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-03-20 03:06:26.513317 ac-websocket-server-0.2.dev9/
+-rw-r--r--   0 mark       (501) staff       (20)     4939 2023-03-20 03:06:26.513094 ac-websocket-server-0.2.dev9/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)     4672 2022-11-14 11:13:56.000000 ac-websocket-server-0.2.dev9/README.md
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-03-20 03:06:26.500850 ac-websocket-server-0.2.dev9/ac_websocket_client/
+-rw-r--r--   0 mark       (501) staff       (20)       51 2022-12-22 06:43:00.000000 ac-websocket-server-0.2.dev9/ac_websocket_client/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)     1467 2022-12-22 06:43:00.000000 ac-websocket-server-0.2.dev9/ac_websocket_client/__main__.py
+-rw-r--r--   0 mark       (501) staff       (20)    21465 2023-03-05 22:27:25.000000 ac-websocket-server-0.2.dev9/ac_websocket_client/app.py
+-rw-r--r--   0 mark       (501) staff       (20)     4350 2022-12-21 22:24:54.000000 ac-websocket-server-0.2.dev9/ac_websocket_client/objects.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-03-20 03:06:26.510138 ac-websocket-server-0.2.dev9/ac_websocket_server/
+-rw-r--r--   0 mark       (501) staff       (20)      264 2022-09-02 03:43:49.000000 ac-websocket-server-0.2.dev9/ac_websocket_server/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)     1701 2022-11-14 11:13:56.000000 ac-websocket-server-0.2.dev9/ac_websocket_server/__main__.py
+-rw-r--r--   0 mark       (501) staff       (20)    10231 2023-02-12 22:42:19.000000 ac-websocket-server-0.2.dev9/ac_websocket_server/child.py
+-rw-r--r--   0 mark       (501) staff       (20)     2684 2022-11-15 11:34:40.000000 ac-websocket-server-0.2.dev9/ac_websocket_server/connection.py
+-rw-r--r--   0 mark       (501) staff       (20)      132 2023-03-17 05:54:12.000000 ac-websocket-server-0.2.dev9/ac_websocket_server/constants.py
+-rw-r--r--   0 mark       (501) staff       (20)      530 2022-09-02 03:43:49.000000 ac-websocket-server-0.2.dev9/ac_websocket_server/debug.py
+-rw-r--r--   0 mark       (501) staff       (20)     7594 2023-03-10 21:12:13.000000 ac-websocket-server-0.2.dev9/ac_websocket_server/entries.py
+-rw-r--r--   0 mark       (501) staff       (20)      148 2022-09-02 03:43:49.000000 ac-websocket-server-0.2.dev9/ac_websocket_server/error.py
+-rw-r--r--   0 mark       (501) staff       (20)     9242 2023-02-19 02:33:16.000000 ac-websocket-server-0.2.dev9/ac_websocket_server/game.py
+-rw-r--r--   0 mark       (501) staff       (20)     4804 2023-03-20 02:59:48.000000 ac-websocket-server-0.2.dev9/ac_websocket_server/grid.py
+-rw-r--r--   0 mark       (501) staff       (20)     1441 2023-03-05 22:27:25.000000 ac-websocket-server-0.2.dev9/ac_websocket_server/handlers.py
+-rw-r--r--   0 mark       (501) staff       (20)     2480 2022-11-15 11:34:40.000000 ac-websocket-server-0.2.dev9/ac_websocket_server/lobby.py
+-rw-r--r--   0 mark       (501) staff       (20)     2939 2023-02-13 04:44:51.000000 ac-websocket-server-0.2.dev9/ac_websocket_server/objects.py
+-rw-r--r--   0 mark       (501) staff       (20)     3389 2022-10-14 06:35:28.000000 ac-websocket-server-0.2.dev9/ac_websocket_server/observer.py
+-rw-r--r--   0 mark       (501) staff       (20)      957 2022-09-04 08:46:38.000000 ac-websocket-server-0.2.dev9/ac_websocket_server/protocol.py
+-rw-r--r--   0 mark       (501) staff       (20)     4582 2023-03-19 23:43:44.000000 ac-websocket-server-0.2.dev9/ac_websocket_server/server.py
+-rw-r--r--   0 mark       (501) staff       (20)     1777 2022-09-02 03:38:58.000000 ac-websocket-server-0.2.dev9/ac_websocket_server/task_logger.py
+-rw-r--r--   0 mark       (501) staff       (20)     2694 2023-03-05 22:28:02.000000 ac-websocket-server-0.2.dev9/ac_websocket_server/tracker.py
+-rw-r--r--   0 mark       (501) staff       (20)     8063 2023-01-08 22:03:02.000000 ac-websocket-server-0.2.dev9/ac_websocket_server/watcher.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-03-20 03:06:26.512676 ac-websocket-server-0.2.dev9/ac_websocket_server.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)     4939 2023-03-20 03:06:26.000000 ac-websocket-server-0.2.dev9/ac_websocket_server.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      942 2023-03-20 03:06:26.000000 ac-websocket-server-0.2.dev9/ac_websocket_server.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-03-20 03:06:26.000000 ac-websocket-server-0.2.dev9/ac_websocket_server.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)       35 2023-03-20 03:06:26.000000 ac-websocket-server-0.2.dev9/ac_websocket_server.egg-info/requires.txt
+-rw-r--r--   0 mark       (501) staff       (20)       40 2023-03-20 03:06:26.000000 ac-websocket-server-0.2.dev9/ac_websocket_server.egg-info/top_level.txt
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-03-20 03:06:26.513374 ac-websocket-server-0.2.dev9/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)      729 2022-11-06 00:50:25.000000 ac-websocket-server-0.2.dev9/setup.py
```

### Comparing `ac-websocket-server-0.2.dev8/PKG-INFO` & `ac-websocket-server-0.2.dev9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ac-websocket-server
-Version: 0.2.dev8
+Version: 0.2.dev9
 Summary: Assetto Corsa Websockets Server
 Author: Mark Hannon
 Author-email: mark.hannon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
```

### Comparing `ac-websocket-server-0.2.dev8/README.md` & `ac-websocket-server-0.2.dev9/README.md`

 * *Files identical despite different names*

### Comparing `ac-websocket-server-0.2.dev8/ac_websocket_client/__main__.py` & `ac-websocket-server-0.2.dev9/ac_websocket_client/__main__.py`

 * *Files identical despite different names*

### Comparing `ac-websocket-server-0.2.dev8/ac_websocket_client/app.py` & `ac-websocket-server-0.2.dev9/ac_websocket_client/app.py`

 * *Files identical despite different names*

### Comparing `ac-websocket-server-0.2.dev8/ac_websocket_client/objects.py` & `ac-websocket-server-0.2.dev9/ac_websocket_client/objects.py`

 * *Files identical despite different names*

### Comparing `ac-websocket-server-0.2.dev8/ac_websocket_server/__main__.py` & `ac-websocket-server-0.2.dev9/ac_websocket_server/__main__.py`

 * *Files identical despite different names*

### Comparing `ac-websocket-server-0.2.dev8/ac_websocket_server/child.py` & `ac-websocket-server-0.2.dev9/ac_websocket_server/child.py`

 * *Files identical despite different names*

### Comparing `ac-websocket-server-0.2.dev8/ac_websocket_server/connection.py` & `ac-websocket-server-0.2.dev9/ac_websocket_server/connection.py`

 * *Files identical despite different names*

### Comparing `ac-websocket-server-0.2.dev8/ac_websocket_server/debug.py` & `ac-websocket-server-0.2.dev9/ac_websocket_server/debug.py`

 * *Files identical despite different names*

### Comparing `ac-websocket-server-0.2.dev8/ac_websocket_server/entries.py` & `ac-websocket-server-0.2.dev9/ac_websocket_server/entries.py`

 * *Files identical despite different names*

### Comparing `ac-websocket-server-0.2.dev8/ac_websocket_server/game.py` & `ac-websocket-server-0.2.dev9/ac_websocket_server/game.py`

 * *Files identical despite different names*

### Comparing `ac-websocket-server-0.2.dev8/ac_websocket_server/handlers.py` & `ac-websocket-server-0.2.dev9/ac_websocket_server/handlers.py`

 * *Files identical despite different names*

### Comparing `ac-websocket-server-0.2.dev8/ac_websocket_server/lobby.py` & `ac-websocket-server-0.2.dev9/ac_websocket_server/lobby.py`

 * *Files identical despite different names*

### Comparing `ac-websocket-server-0.2.dev8/ac_websocket_server/objects.py` & `ac-websocket-server-0.2.dev9/ac_websocket_server/objects.py`

 * *Files identical despite different names*

### Comparing `ac-websocket-server-0.2.dev8/ac_websocket_server/observer.py` & `ac-websocket-server-0.2.dev9/ac_websocket_server/observer.py`

 * *Files identical despite different names*

### Comparing `ac-websocket-server-0.2.dev8/ac_websocket_server/protocol.py` & `ac-websocket-server-0.2.dev9/ac_websocket_server/protocol.py`

 * *Files identical despite different names*

### Comparing `ac-websocket-server-0.2.dev8/ac_websocket_server/server.py` & `ac-websocket-server-0.2.dev9/ac_websocket_server/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,19 @@
         self.port = port
 
         if not server_directory:
             self.server_directory = os.getcwd()
         else:
             self.server_directory = server_directory
 
+        if os.path.isdir(f'{self.server_directory}/debug'):
+            self.debug_directory = f'{self.server_directory}/debug'
+        else:
+            self.debug_directory = None
+
         try:
             self.game = GameServer(directory=self.server_directory)
             s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
             result = s.connect_ex((self.host, int(self.game.http_port)))
             s.close()
             if result == 0:
                 msg = f'Fatal error - Existing ACS process running on {self.host}:{self.game.http_port}'
```

### Comparing `ac-websocket-server-0.2.dev8/ac_websocket_server/task_logger.py` & `ac-websocket-server-0.2.dev9/ac_websocket_server/task_logger.py`

 * *Files identical despite different names*

### Comparing `ac-websocket-server-0.2.dev8/ac_websocket_server/tracker.py` & `ac-websocket-server-0.2.dev9/ac_websocket_server/tracker.py`

 * *Files identical despite different names*

### Comparing `ac-websocket-server-0.2.dev8/ac_websocket_server/watcher.py` & `ac-websocket-server-0.2.dev9/ac_websocket_server/watcher.py`

 * *Files identical despite different names*

### Comparing `ac-websocket-server-0.2.dev8/ac_websocket_server.egg-info/PKG-INFO` & `ac-websocket-server-0.2.dev9/ac_websocket_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ac-websocket-server
-Version: 0.2.dev8
+Version: 0.2.dev9
 Summary: Assetto Corsa Websockets Server
 Author: Mark Hannon
 Author-email: mark.hannon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
```

### Comparing `ac-websocket-server-0.2.dev8/ac_websocket_server.egg-info/SOURCES.txt` & `ac-websocket-server-0.2.dev9/ac_websocket_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ac-websocket-server-0.2.dev8/setup.py` & `ac-websocket-server-0.2.dev9/setup.py`

 * *Files identical despite different names*

