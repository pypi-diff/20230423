# Comparing `tmp/tickerdax-0.0.8.tar.gz` & `tmp/tickerdax-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tickerdax-0.0.8.tar", last modified: Mon Nov 14 17:03:03 2022, max compression
+gzip compressed data, was "tickerdax-0.0.9.tar", last modified: Mon Nov 14 19:38:52 2022, max compression
```

## Comparing `tickerdax-0.0.8.tar` & `tickerdax-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 17:03:03.322131 tickerdax-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     5194 2022-11-14 17:03:03.322131 tickerdax-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4673 2022-11-14 17:02:48.000000 tickerdax-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      115 2022-11-14 17:02:48.000000 tickerdax-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      923 2022-11-14 17:03:03.322131 tickerdax-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 17:03:03.318131 tickerdax-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 17:03:03.318131 tickerdax-0.0.8/src/tickerdax/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-14 17:02:48.000000 tickerdax-0.0.8/src/tickerdax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-11-14 17:02:48.000000 tickerdax-0.0.8/src/tickerdax/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2653 2022-11-14 17:02:48.000000 tickerdax-0.0.8/src/tickerdax/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    17767 2022-11-14 17:02:48.000000 tickerdax-0.0.8/src/tickerdax/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     3396 2022-11-14 17:02:48.000000 tickerdax-0.0.8/src/tickerdax/config_base.py
--rw-r--r--   0 runner    (1001) docker     (121)      486 2022-11-14 17:02:48.000000 tickerdax-0.0.8/src/tickerdax/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     2150 2022-11-14 17:02:48.000000 tickerdax-0.0.8/src/tickerdax/downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 17:03:03.322131 tickerdax-0.0.8/src/tickerdax/example_configs/
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-11-14 17:02:48.000000 tickerdax-0.0.8/src/tickerdax/example_configs/config.json
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-11-14 17:02:48.000000 tickerdax-0.0.8/src/tickerdax/example_configs/config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1203 2022-11-14 17:02:48.000000 tickerdax-0.0.8/src/tickerdax/formatting.py
--rw-r--r--   0 runner    (1001) docker     (121)     1761 2022-11-14 17:02:48.000000 tickerdax-0.0.8/src/tickerdax/streamer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 17:03:03.322131 tickerdax-0.0.8/src/tickerdax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5194 2022-11-14 17:03:03.000000 tickerdax-0.0.8/src/tickerdax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      577 2022-11-14 17:03:03.000000 tickerdax-0.0.8/src/tickerdax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-14 17:03:03.000000 tickerdax-0.0.8/src/tickerdax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-11-14 17:03:03.000000 tickerdax-0.0.8/src/tickerdax.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-11-14 17:03:03.000000 tickerdax-0.0.8/src/tickerdax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-11-14 17:03:03.000000 tickerdax-0.0.8/src/tickerdax.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 19:38:52.572804 tickerdax-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     5194 2022-11-14 19:38:52.572804 tickerdax-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4673 2022-11-14 19:38:43.000000 tickerdax-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      115 2022-11-14 19:38:43.000000 tickerdax-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      923 2022-11-14 19:38:52.572804 tickerdax-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 19:38:52.568804 tickerdax-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 19:38:52.572804 tickerdax-0.0.9/src/tickerdax/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-14 19:38:43.000000 tickerdax-0.0.9/src/tickerdax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       90 2022-11-14 19:38:43.000000 tickerdax-0.0.9/src/tickerdax/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2653 2022-11-14 19:38:43.000000 tickerdax-0.0.9/src/tickerdax/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17915 2022-11-14 19:38:43.000000 tickerdax-0.0.9/src/tickerdax/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3396 2022-11-14 19:38:43.000000 tickerdax-0.0.9/src/tickerdax/config_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)      486 2022-11-14 19:38:43.000000 tickerdax-0.0.9/src/tickerdax/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2150 2022-11-14 19:38:43.000000 tickerdax-0.0.9/src/tickerdax/downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 19:38:52.572804 tickerdax-0.0.9/src/tickerdax/example_configs/
+-rw-r--r--   0 runner    (1001) docker     (121)      190 2022-11-14 19:38:43.000000 tickerdax-0.0.9/src/tickerdax/example_configs/config.json
+-rw-r--r--   0 runner    (1001) docker     (121)      112 2022-11-14 19:38:43.000000 tickerdax-0.0.9/src/tickerdax/example_configs/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1203 2022-11-14 19:38:43.000000 tickerdax-0.0.9/src/tickerdax/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1761 2022-11-14 19:38:43.000000 tickerdax-0.0.9/src/tickerdax/streamer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 19:38:52.572804 tickerdax-0.0.9/src/tickerdax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5194 2022-11-14 19:38:52.000000 tickerdax-0.0.9/src/tickerdax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      577 2022-11-14 19:38:52.000000 tickerdax-0.0.9/src/tickerdax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-14 19:38:52.000000 tickerdax-0.0.9/src/tickerdax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-11-14 19:38:52.000000 tickerdax-0.0.9/src/tickerdax.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       98 2022-11-14 19:38:52.000000 tickerdax-0.0.9/src/tickerdax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2022-11-14 19:38:52.000000 tickerdax-0.0.9/src/tickerdax.egg-info/top_level.txt
```

### Comparing `tickerdax-0.0.8/PKG-INFO` & `tickerdax-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tickerdax
-Version: 0.0.8
+Version: 0.0.9
 Summary: A python client for tickerdax.com with a built-in caching system.
 Home-page: https://github.com/tickerdax/tickerdax-python-client
 Author: tickerdax.com
 Author-email: info@tickerdax.com
 Project-URL: Bug Tracker, https://github.com/tickerdax/tickerdax-python-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tickerdax-0.0.8/README.md` & `tickerdax-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `tickerdax-0.0.8/setup.cfg` & `tickerdax-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tickerdax
-version = 0.0.8
+version = 0.0.9
 author = tickerdax.com
 author_email = info@tickerdax.com
 description = A python client for tickerdax.com with a built-in caching system.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tickerdax/tickerdax-python-client
 project_urls =
```

### Comparing `tickerdax-0.0.8/src/tickerdax/cli.py` & `tickerdax-0.0.9/src/tickerdax/cli.py`

 * *Files identical despite different names*

### Comparing `tickerdax-0.0.8/src/tickerdax/client.py` & `tickerdax-0.0.9/src/tickerdax/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -254,21 +254,24 @@
         try:
             async with websockets.connect(
                     uri,
                     extra_headers={'email': self._email, 'token': self._websocket_api_key}
             ) as connected_socket:
                 self._logger.info(f"> Connected to {uri}")
                 while True:
-                    data = json.loads(await connected_socket.recv())
-                    symbol = data.get('symbol')
-                    timestamp = data.get('id')
-                    if symbol and timestamp:
-                        for key in self._get_cache_keys(client._format_route(route), [symbol], [timestamp]):
-                            self._redis_client.set(key, json.dumps(data))
-                            self._logger.info(f'Cached: {pformat(data)}')
+                    try:
+                        data = json.loads(await connected_socket.recv())
+                        symbol = data.get('symbol')
+                        timestamp = data.get('id')
+                        if symbol and timestamp:
+                            for key in self._get_cache_keys(self._format_route(route), [symbol], [timestamp]):
+                                self._redis_client.set(key, json.dumps(data))
+                                self._logger.info(f'Cached: {pformat(data)}')
+                    except Exception as error:
+                        self._logger.error(error)
 
         except InvalidStatusCode as error:
             if error.status_code == 401:
                 self.report_error(
                     'This email and API key combination are not authorized to connect to '
                     'the https://tickerdax.com websocket API. Please check you credentials.'
                 )
```

### Comparing `tickerdax-0.0.8/src/tickerdax/config_base.py` & `tickerdax-0.0.9/src/tickerdax/config_base.py`

 * *Files identical despite different names*

### Comparing `tickerdax-0.0.8/src/tickerdax/downloader.py` & `tickerdax-0.0.9/src/tickerdax/downloader.py`

 * *Files identical despite different names*

### Comparing `tickerdax-0.0.8/src/tickerdax/formatting.py` & `tickerdax-0.0.9/src/tickerdax/formatting.py`

 * *Files identical despite different names*

### Comparing `tickerdax-0.0.8/src/tickerdax/streamer.py` & `tickerdax-0.0.9/src/tickerdax/streamer.py`

 * *Files identical despite different names*

### Comparing `tickerdax-0.0.8/src/tickerdax.egg-info/PKG-INFO` & `tickerdax-0.0.9/src/tickerdax.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tickerdax
-Version: 0.0.8
+Version: 0.0.9
 Summary: A python client for tickerdax.com with a built-in caching system.
 Home-page: https://github.com/tickerdax/tickerdax-python-client
 Author: tickerdax.com
 Author-email: info@tickerdax.com
 Project-URL: Bug Tracker, https://github.com/tickerdax/tickerdax-python-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tickerdax-0.0.8/src/tickerdax.egg-info/SOURCES.txt` & `tickerdax-0.0.9/src/tickerdax.egg-info/SOURCES.txt`

 * *Files identical despite different names*

