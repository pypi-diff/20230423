# Comparing `tmp/aiointeractions-1.1.1.tar.gz` & `tmp/aiointeractions-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiointeractions-1.1.1.tar", last modified: Sat Feb 11 18:08:35 2023, max compression
+gzip compressed data, was "aiointeractions-1.2.0.tar", last modified: Sun Apr 23 17:53:25 2023, max compression
```

## Comparing `aiointeractions-1.1.1.tar` & `aiointeractions-1.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-02-11 18:08:35.396196 aiointeractions-1.1.1/
--rw-rw-rw-   0        0        0     1104 2023-02-11 18:07:32.000000 aiointeractions-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     2229 2023-02-11 18:08:35.393165 aiointeractions-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1154 2023-02-11 18:07:32.000000 aiointeractions-1.1.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-02-11 18:08:35.356410 aiointeractions-1.1.1/aiointeractions/
--rw-rw-rw-   0        0        0      228 2023-02-11 18:07:32.000000 aiointeractions-1.1.1/aiointeractions/__init__.py
--rw-rw-rw-   0        0        0     6991 2023-02-11 18:07:32.000000 aiointeractions-1.1.1/aiointeractions/app.py
-drwxrwxrwx   0        0        0        0 2023-02-11 18:08:35.389292 aiointeractions-1.1.1/aiointeractions.egg-info/
--rw-rw-rw-   0        0        0     2229 2023-02-11 18:08:35.000000 aiointeractions-1.1.1/aiointeractions.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      322 2023-02-11 18:08:35.000000 aiointeractions-1.1.1/aiointeractions.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-11 18:08:35.000000 aiointeractions-1.1.1/aiointeractions.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2023-02-11 18:08:35.000000 aiointeractions-1.1.1/aiointeractions.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-02-11 18:08:35.000000 aiointeractions-1.1.1/aiointeractions.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1580 2023-02-11 18:07:32.000000 aiointeractions-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-11 18:08:35.397154 aiointeractions-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0       75 2023-02-11 18:07:32.000000 aiointeractions-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-11 18:08:35.391235 aiointeractions-1.1.1/tests/
--rw-rw-rw-   0        0        0     1351 2023-02-11 18:07:32.000000 aiointeractions-1.1.1/tests/test_interactions_handler.py
+drwxrwxrwx   0        0        0        0 2023-04-23 17:53:25.333061 aiointeractions-1.2.0/
+-rw-rw-rw-   0        0        0     1104 2023-04-23 17:18:17.000000 aiointeractions-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     2229 2023-04-23 17:53:25.332069 aiointeractions-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1154 2023-04-23 17:18:17.000000 aiointeractions-1.2.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-23 17:53:25.290075 aiointeractions-1.2.0/aiointeractions/
+-rw-rw-rw-   0        0        0      226 2023-04-23 17:34:33.000000 aiointeractions-1.2.0/aiointeractions/__init__.py
+-rw-rw-rw-   0        0        0     7738 2023-04-23 17:45:12.000000 aiointeractions-1.2.0/aiointeractions/app.py
+drwxrwxrwx   0        0        0        0 2023-04-23 17:53:25.326094 aiointeractions-1.2.0/aiointeractions.egg-info/
+-rw-rw-rw-   0        0        0     2229 2023-04-23 17:53:25.000000 aiointeractions-1.2.0/aiointeractions.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      322 2023-04-23 17:53:25.000000 aiointeractions-1.2.0/aiointeractions.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 17:53:25.000000 aiointeractions-1.2.0/aiointeractions.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       91 2023-04-23 17:53:25.000000 aiointeractions-1.2.0/aiointeractions.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-23 17:53:25.000000 aiointeractions-1.2.0/aiointeractions.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1580 2023-04-23 17:18:17.000000 aiointeractions-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-23 17:53:25.333061 aiointeractions-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0       73 2023-04-23 17:30:18.000000 aiointeractions-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 17:53:25.329062 aiointeractions-1.2.0/tests/
+-rw-rw-rw-   0        0        0     1351 2023-04-23 17:30:18.000000 aiointeractions-1.2.0/tests/test_interactions_handler.py
```

### Comparing `aiointeractions-1.1.1/LICENSE` & `aiointeractions-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiointeractions-1.1.1/PKG-INFO` & `aiointeractions-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiointeractions
-Version: 1.1.1
+Version: 1.2.0
 Summary: An async Discord HTTP Interactions wrapper for discord.py.
 Author: The Master
 License: MIT
 Project-URL: Homepage, http://github.com/TheMaster3558/aiointeractions
 Project-URL: Documentation, http://aiointeractions.readthedocs.io/
 Keywords: discord
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `aiointeractions-1.1.1/README.rst` & `aiointeractions-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `aiointeractions-1.1.1/aiointeractions/app.py` & `aiointeractions-1.2.0/aiointeractions/app.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,31 +24,31 @@
 from __future__ import annotations
 
 import asyncio
 from typing import Any, Callable, Dict, Mapping, Optional, Set
 
 import discord
 from aiohttp import web
-from nacl.signing import VerifyKey
 from nacl.exceptions import BadSignatureError
+from nacl.signing import VerifyKey
 
 if discord.utils.HAS_ORJSON:
     from orjson import dumps, loads
 else:
     from json import dumps, loads
 
 
 __all__ = ('InteractionsApp',)
 
 
 none_function: Callable[[Any], None] = lambda r: None
 PONG: Dict[str, int] = {'type': 1}  # pong response
 
 
-def get_latest_task(before_tasks: Set[asyncio.Task[Any]]) -> asyncio.Task[None]:
+def get_latest_task(before_tasks: Set[asyncio.Task[Any]]) -> asyncio.Task[Any]:
     return (asyncio.all_tasks() - before_tasks).pop()
     # guaranteed to be expected task because there are no awaits
     # inbetween calling this function and the all tasks get
 
 
 class InteractionsApp:
     """A web application made with `aiohttp` for receiving interactions from Discord.
@@ -66,14 +66,20 @@
         A function (synchronous or asynchronous) that accepts 1 argument,
         `request <https://docs.aiohttp.org/en/stable/web_reference.html#aiohttp.web.Request>`_
         that would return the body for the response.
     forbidden_response: Callable[[web.Request], Any]
         A function (synchronous or asynchronous) that accepts 1 argument,
         `request <https://docs.aiohttp.org/en/stable/web_reference.html#aiohttp.web.Request>`_
         that would return the body for the response.
+    raise_for_bad_response: :class:`bool`
+        Raises `aiohttp.web.HTTPException <https://docs.aiohttp.org/en/stable/web_reference.html#aiohttp.web.HTTPException>`_
+        on a bad request, otherwise returns `aiohttp.web.Response <https://docs.aiohttp.org/en/stable/web_reference.html#aiohttp.web.Response>`_
+        This parameter will always be ``True`` starting from v2.
+
+        .. versionadded:: 1.2
 
 
     .. warning::
 
         If the return value of `success_response` or `forbidden_response` are meant to be a JSON response, make sure to
         serialize the object to JSON format with `json.dumps <https://docs.python.org/3/library/json.html#json.dumps>`_.
 
@@ -88,28 +94,30 @@
         self,
         client: discord.Client,
         *,
         app: Optional[web.Application] = None,
         route: str = '/interactions',
         success_response: Callable[[web.Request], Any] = none_function,
         forbidden_response: Callable[[web.Request], Any] = none_function,
+        raise_for_bad_response: bool = False,
     ) -> None:
         self.client: discord.Client = client
         self.verify_key: VerifyKey = discord.utils.MISSING
 
         if app is None:
             app = web.Application()
 
         app.add_routes([web.post(route, self.interactions_handler)])
         app.on_startup.append(self._set_running)
         app.on_shutdown.append(self._set_running)
         self.app: web.Application = app
 
         self.success_response: Callable[[web.Request], Any] = success_response
         self.forbidden_response: Callable[[web.Request], Any] = forbidden_response
+        self.raise_for_bad_response: bool = raise_for_bad_response
 
         self._running: bool = False
 
     async def _set_running(self, _: Any) -> None:
         self._running = not self._running
 
     def _verify_request(self, headers: Mapping[str, Any], body: str) -> bool:
@@ -131,21 +139,26 @@
         ``True`` if the app is running, otherwise ``False``.
 
 
         .. versionadded:: 1.1
         """
         return self._running
 
+    def _handle_unauthorized_request(self, body: Any) -> web.Response:
+        if self.raise_for_bad_response:
+            raise web.HTTPUnauthorized(body=body)
+        return web.Response(status=401, body=body)
+
     async def interactions_handler(self, request: web.Request) -> web.Response:
         self.client.dispatch('interaction_request', request)
         body = await request.text()
 
         if not self._verify_request(request.headers, body):
             response = await discord.utils.maybe_coroutine(self.forbidden_response, request)
-            return web.Response(status=401, body=response)
+            return self._handle_unauthorized_request(body)
 
         self.client.dispatch('verified_interaction_request', request)
         data = loads(body)
         if data['type'] == 1:  # ping
             return web.Response(body=dumps(PONG))
 
         tasks = asyncio.all_tasks()
```

### Comparing `aiointeractions-1.1.1/aiointeractions.egg-info/PKG-INFO` & `aiointeractions-1.2.0/aiointeractions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiointeractions
-Version: 1.1.1
+Version: 1.2.0
 Summary: An async Discord HTTP Interactions wrapper for discord.py.
 Author: The Master
 License: MIT
 Project-URL: Homepage, http://github.com/TheMaster3558/aiointeractions
 Project-URL: Documentation, http://aiointeractions.readthedocs.io/
 Keywords: discord
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `aiointeractions-1.1.1/pyproject.toml` & `aiointeractions-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiointeractions-1.1.1/tests/test_interactions_handler.py` & `aiointeractions-1.2.0/tests/test_interactions_handler.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Any, Mapping
 
+import discord
 import pytest
 
 import aiointeractions
-import discord
 
 
 class MockRequest:
     def __init__(self, headers: Mapping[str, Any], data: Any):
         self.headers = headers
         self._data = data
```

