# Comparing `tmp/bittrade_luno_websocket-0.1.2.tar.gz` & `tmp/bittrade_luno_websocket-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bittrade_luno_websocket-0.1.2.tar", max compression
+gzip compressed data, was "bittrade_luno_websocket-0.1.3.tar", max compression
```

## Comparing `bittrade_luno_websocket-0.1.2.tar` & `bittrade_luno_websocket-0.1.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0        0 2023-02-23 05:51:40.566521 bittrade_luno_websocket-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-02-23 05:51:40.566632 bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/__init__.py
--rw-r--r--   0        0        0        0 2023-02-23 05:51:40.566732 bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/channels/__init__.py
--rw-r--r--   0        0        0    12996 2023-03-23 09:09:52.264805 bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/channels/orderbook.py
--rw-r--r--   0        0        0     1838 2023-04-16 10:55:15.725467 bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/channels/user_stream.py
--rw-r--r--   0        0        0        0 2023-03-11 21:05:54.544362 bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/connection/__init__.py
--rw-r--r--   0        0        0     1374 2023-03-11 21:05:54.545267 bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/connection/authenticate.py
--rw-r--r--   0        0        0     3525 2023-03-13 09:43:24.335646 bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/connection/generic.py
--rw-r--r--   0        0        0     2401 2023-03-13 09:43:24.335922 bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/connection/http.py
--rw-r--r--   0        0        0      720 2023-03-13 09:43:24.336282 bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/connection/public.py
--rw-r--r--   0        0        0      102 2023-03-13 09:43:24.336634 bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/models/__init__.py
--rw-r--r--   0        0        0      300 2023-04-16 20:07:19.291721 bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/models/endpoints.py
--rw-r--r--   0        0        0      690 2023-03-11 21:05:54.548298 bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/models/enhanced_websocket.py
--rw-r--r--   0        0        0      203 2023-03-13 09:43:24.337178 bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/models/orderbook.py
--rw-r--r--   0        0        0      398 2023-03-13 09:43:24.337444 bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/models/request.py
--rw-r--r--   0        0        0      847 2023-03-13 09:43:24.337668 bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/models/response_message.py
--rw-r--r--   0        0        0        0 2023-03-13 09:43:24.337809 bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/models/rest/__init__.py
--rw-r--r--   0        0        0      470 2023-04-16 20:12:18.269435 bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/models/rest/balance.py
--rw-r--r--   0        0        0     1100 2023-03-23 09:08:33.509055 bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/models/rest/get_order.py
--rw-r--r--   0        0        0     1236 2023-04-16 20:00:08.620775 bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/models/rest/order.py
--rw-r--r--   0        0        0     1034 2023-04-17 04:25:05.453554 bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/rest/balance.py
--rw-r--r--   0        0        0      580 2023-03-23 09:08:33.509444 bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/rest/get_book.py
--rw-r--r--   0        0        0      621 2023-03-23 09:08:33.509626 bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/rest/get_order.py
--rw-r--r--   0        0        0     1876 2023-04-17 04:24:16.695673 bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/rest/order.py
--rw-r--r--   0        0        0      367 2023-03-13 09:43:24.340924 bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/signing/__init__.py
--rw-r--r--   0        0        0     1070 2023-04-17 04:46:18.032120 bittrade_luno_websocket-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1015 1970-01-01 00:00:00.000000 bittrade_luno_websocket-0.1.2/setup.py
--rw-r--r--   0        0        0      600 1970-01-01 00:00:00.000000 bittrade_luno_websocket-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-02-07 04:39:10.926618 bittrade_luno_websocket-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-02-07 04:39:10.926618 bittrade_luno_websocket-0.1.3/bittrade_luno_websocket/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-13 04:54:38.094803 bittrade_luno_websocket-0.1.3/bittrade_luno_websocket/channels/__init__.py
+-rw-r--r--   0        0        0    12996 2023-04-03 05:19:53.942449 bittrade_luno_websocket-0.1.3/bittrade_luno_websocket/channels/orderbook.py
+-rw-r--r--   0        0        0     1735 2023-04-19 06:22:14.941257 bittrade_luno_websocket-0.1.3/bittrade_luno_websocket/channels/user_stream.py
+-rw-r--r--   0        0        0        0 2023-03-10 01:38:28.536176 bittrade_luno_websocket-0.1.3/bittrade_luno_websocket/connection/__init__.py
+-rw-r--r--   0        0        0     1374 2023-03-12 01:34:13.037369 bittrade_luno_websocket-0.1.3/bittrade_luno_websocket/connection/authenticate.py
+-rw-r--r--   0        0        0     3525 2023-03-12 05:38:45.786365 bittrade_luno_websocket-0.1.3/bittrade_luno_websocket/connection/generic.py
+-rw-r--r--   0        0        0     2296 2023-04-23 05:37:33.190506 bittrade_luno_websocket-0.1.3/bittrade_luno_websocket/connection/http.py
+-rw-r--r--   0        0        0      720 2023-03-12 06:46:01.623584 bittrade_luno_websocket-0.1.3/bittrade_luno_websocket/connection/public.py
+-rw-r--r--   0        0        0      102 2023-03-13 08:27:34.679675 bittrade_luno_websocket-0.1.3/bittrade_luno_websocket/models/__init__.py
+-rw-r--r--   0        0        0      300 2023-04-19 06:19:31.536589 bittrade_luno_websocket-0.1.3/bittrade_luno_websocket/models/endpoints.py
+-rw-r--r--   0        0        0      690 2023-03-10 02:44:12.318417 bittrade_luno_websocket-0.1.3/bittrade_luno_websocket/models/enhanced_websocket.py
+-rw-r--r--   0        0        0      203 2023-03-13 03:15:50.329774 bittrade_luno_websocket-0.1.3/bittrade_luno_websocket/models/orderbook.py
+-rw-r--r--   0        0        0      398 2023-03-13 08:34:59.946557 bittrade_luno_websocket-0.1.3/bittrade_luno_websocket/models/request.py
+-rw-r--r--   0        0        0      847 2023-03-13 08:14:41.380022 bittrade_luno_websocket-0.1.3/bittrade_luno_websocket/models/response_message.py
+-rw-r--r--   0        0        0        0 2023-03-13 08:20:30.323385 bittrade_luno_websocket-0.1.3/bittrade_luno_websocket/models/rest/__init__.py
+-rw-r--r--   0        0        0      470 2023-04-19 06:19:31.546589 bittrade_luno_websocket-0.1.3/bittrade_luno_websocket/models/rest/balance.py
+-rw-r--r--   0        0        0     1100 2023-03-16 08:02:48.834747 bittrade_luno_websocket-0.1.3/bittrade_luno_websocket/models/rest/get_order.py
+-rw-r--r--   0        0        0     1236 2023-04-19 06:19:31.546589 bittrade_luno_websocket-0.1.3/bittrade_luno_websocket/models/rest/order.py
+-rw-r--r--   0        0        0     1034 2023-04-19 06:19:31.546589 bittrade_luno_websocket-0.1.3/bittrade_luno_websocket/rest/balance.py
+-rw-r--r--   0        0        0      580 2023-03-15 08:30:08.583232 bittrade_luno_websocket-0.1.3/bittrade_luno_websocket/rest/get_book.py
+-rw-r--r--   0        0        0      621 2023-03-16 08:05:10.479544 bittrade_luno_websocket-0.1.3/bittrade_luno_websocket/rest/get_order.py
+-rw-r--r--   0        0        0     1876 2023-04-19 06:19:31.546589 bittrade_luno_websocket-0.1.3/bittrade_luno_websocket/rest/order.py
+-rw-r--r--   0        0        0      367 2023-03-13 08:59:54.685549 bittrade_luno_websocket-0.1.3/bittrade_luno_websocket/signing/__init__.py
+-rw-r--r--   0        0        0     1070 2023-04-23 05:41:53.709619 bittrade_luno_websocket-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1015 1970-01-01 00:00:00.000000 bittrade_luno_websocket-0.1.3/setup.py
+-rw-r--r--   0        0        0      600 1970-01-01 00:00:00.000000 bittrade_luno_websocket-0.1.3/PKG-INFO
```

### Comparing `bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/channels/orderbook.py` & `bittrade_luno_websocket-0.1.3/bittrade_luno_websocket/channels/orderbook.py`

 * *Files identical despite different names*

### Comparing `bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/channels/user_stream.py` & `bittrade_luno_websocket-0.1.3/bittrade_luno_websocket/channels/user_stream.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,16 +7,14 @@
     message_types,
     status,
 )
 from elm_framework_helpers.websockets.operators import connection_operators
 from elm_framework_helpers.operators import retry_with_delay
 from typing import Any, Callable, Literal, Optional, TypedDict, cast
 from bittrade_luno_websocket.connection import generic
-from bittrade_luno_websocket.models.orderbook import RawOrderBook, RawOrder
-from bittrade_luno_websocket.rest.get_book import load_order_book_http
 from bittrade_luno_websocket.connection.authenticate import send_credentials_operator
 
 import reactivex
 from reactivex import (
     Observable,
     observable,
     abc,
@@ -34,15 +32,17 @@
 class UserStreamMessage(TypedDict):
     type: Literal["order_status", "order_fill", "balance_update"]
     order_status_update: dict
     order_fill_update: dict
     balance_update: dict
 
 
-def user_stream_connection(key: str, secret: str, stable_delay: int = 10):
+def user_stream_connection(
+    key: str, secret: str, stable_delay: int = 10
+) -> Observable[bundle.WebsocketBundle]:
     def subscribe(observer, scheduler=None):
         bundles = generic.raw_websocket_connection(
             "wss://ws.luno.com/api/1/userstream"
         ).pipe(
             retry_with_delay.retry_with_delay(
                 retry_with_delay.luno_delay(), reactivex.timer(stable_delay)
             ),
```

### Comparing `bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/connection/authenticate.py` & `bittrade_luno_websocket-0.1.3/bittrade_luno_websocket/connection/authenticate.py`

 * *Files identical despite different names*

### Comparing `bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/connection/generic.py` & `bittrade_luno_websocket-0.1.3/bittrade_luno_websocket/connection/generic.py`

 * *Files identical despite different names*

### Comparing `bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/connection/http.py` & `bittrade_luno_websocket-0.1.3/bittrade_luno_websocket/connection/http.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,34 +14,32 @@
 
 logger = getLogger(__name__)
 
 
 def prepare_request(message: models.RequestMessage) -> requests.models.Request:
     http_method = message.method
     kwargs = {}
-    if http_method == "GET":
-        kwargs["params"] = message.params
-    if http_method == "POST":
-        kwargs["json"] = message.params
+    kwargs["params"] = message.params
 
     endpoint = message.endpoint.value
     if message.url_format_arguments:
         endpoint = endpoint.format(**message.url_format_arguments)
-    
+
     return requests.Request(http_method, f"{MARKET_URL}{endpoint}", **kwargs)
 
 
 def send_request(request: requests.models.Request) -> reactivex.Observable:
     def subscribe(
         observer: reactivex.abc.ObserverBase,
         scheduler: reactivex.abc.SchedulerBase | None = None,
     ) -> reactivex.abc.DisposableBase:
         scheduler_ = scheduler or CurrentThreadScheduler()
+
         def act(s, state):
-            del state, s # Unused
+            del state, s  # Unused
             response = session.send(request.prepare())
             if response.ok:
                 body = response.json()
                 if "error_code" in body:
                     observer.on_error(body["error_code"])
                 else:
                     observer.on_next(body)
@@ -56,10 +54,11 @@
                         response.request.body
                         if request.method == "POST"
                         else response.request.headers,
                     )
                     observer.on_error(str(response.status_code))
                 except Exception as exc:
                     observer.on_error(exc)
+
         return scheduler_.schedule(act)
 
     return reactivex.Observable(subscribe)
```

### Comparing `bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/connection/public.py` & `bittrade_luno_websocket-0.1.3/bittrade_luno_websocket/connection/public.py`

 * *Files identical despite different names*

### Comparing `bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/models/enhanced_websocket.py` & `bittrade_luno_websocket-0.1.3/bittrade_luno_websocket/models/enhanced_websocket.py`

 * *Files identical despite different names*

### Comparing `bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/models/response_message.py` & `bittrade_luno_websocket-0.1.3/bittrade_luno_websocket/models/response_message.py`

 * *Files identical despite different names*

### Comparing `bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/models/rest/get_order.py` & `bittrade_luno_websocket-0.1.3/bittrade_luno_websocket/models/rest/get_order.py`

 * *Files identical despite different names*

### Comparing `bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/models/rest/order.py` & `bittrade_luno_websocket-0.1.3/bittrade_luno_websocket/models/rest/order.py`

 * *Files identical despite different names*

### Comparing `bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/rest/balance.py` & `bittrade_luno_websocket-0.1.3/bittrade_luno_websocket/rest/balance.py`

 * *Files identical despite different names*

### Comparing `bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/rest/get_book.py` & `bittrade_luno_websocket-0.1.3/bittrade_luno_websocket/rest/get_book.py`

 * *Files identical despite different names*

### Comparing `bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/rest/get_order.py` & `bittrade_luno_websocket-0.1.3/bittrade_luno_websocket/rest/get_order.py`

 * *Files identical despite different names*

### Comparing `bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/rest/order.py` & `bittrade_luno_websocket-0.1.3/bittrade_luno_websocket/rest/order.py`

 * *Files identical despite different names*

### Comparing `bittrade_luno_websocket-0.1.2/pyproject.toml` & `bittrade_luno_websocket-0.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bittrade-luno-websocket"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["Matt <matt@techspace.asia>"]
 readme = "README.md"
 packages = [{ include = "bittrade_luno_websocket" }]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `bittrade_luno_websocket-0.1.2/setup.py` & `bittrade_luno_websocket-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'reactivex>=4.0.4,<5.0.0',
  'requests>=2.28.2,<3.0.0',
  'returns>=0.19.0,<0.20.0',
  'websocket-client>=1.5.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'bittrade-luno-websocket',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': '',
     'long_description': '',
     'author': 'Matt',
     'author_email': 'matt@techspace.asia',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `bittrade_luno_websocket-0.1.2/PKG-INFO` & `bittrade_luno_websocket-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bittrade-luno-websocket
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Matt
 Author-email: matt@techspace.asia
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ccxt (>=2.7.91,<3.0.0)
```

