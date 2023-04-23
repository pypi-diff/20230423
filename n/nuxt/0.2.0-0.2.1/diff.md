# Comparing `tmp/nuxt-0.2.0.tar.gz` & `tmp/nuxt-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nuxt-0.2.0.tar", last modified: Fri Feb 24 08:54:13 2023, max compression
+gzip compressed data, was "nuxt-0.2.1.tar", last modified: Sun Apr 23 11:40:05 2023, max compression
```

## Comparing `nuxt-0.2.0.tar` & `nuxt-0.2.1.tar`

### file list

```diff
@@ -1,30 +1,38 @@
-drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2023-02-24 08:54:13.000000 nuxt-0.2.0/
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      196 2022-10-09 01:47:11.000000 nuxt-0.2.0/MANIFEST.in
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      534 2023-02-24 08:54:13.000000 nuxt-0.2.0/PKG-INFO
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     7147 2023-02-14 03:23:29.000000 nuxt-0.2.0/README.md
-drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2023-02-24 08:54:13.000000 nuxt-0.2.0/nuxt/
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      596 2023-02-24 04:09:14.000000 nuxt-0.2.0/nuxt/__init__.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     6838 2023-02-24 06:43:47.000000 nuxt-0.2.0/nuxt/__main__.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)    15630 2023-02-24 08:39:17.000000 nuxt-0.2.0/nuxt/app.py
-drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2023-02-24 08:54:13.000000 nuxt-0.2.0/nuxt/asyncio/
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      847 2023-02-24 07:48:32.000000 nuxt-0.2.0/nuxt/asyncio/__init__.py
-drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2023-02-24 08:54:13.000000 nuxt-0.2.0/nuxt/asyncio/repositorys/
--rw-rw-r--   0 arvin     (1000) arvin     (1000)        0 2023-02-23 11:20:39.000000 nuxt-0.2.0/nuxt/asyncio/repositorys/__init__.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     4466 2023-02-24 06:47:45.000000 nuxt-0.2.0/nuxt/asyncio/repositorys/validation.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      111 2023-02-24 03:55:25.000000 nuxt-0.2.0/nuxt/datastructures.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      256 2023-02-24 04:03:52.000000 nuxt-0.2.0/nuxt/exceptions.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     6241 2023-02-24 06:26:12.000000 nuxt-0.2.0/nuxt/openapi.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     3848 2022-10-09 01:47:11.000000 nuxt-0.2.0/nuxt/reloader.py
-drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2023-02-24 08:54:13.000000 nuxt-0.2.0/nuxt/repositorys/
--rw-rw-r--   0 arvin     (1000) arvin     (1000)        0 2022-10-09 06:50:24.000000 nuxt-0.2.0/nuxt/repositorys/__init__.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)        0 2023-02-23 02:07:26.000000 nuxt-0.2.0/nuxt/repositorys/empty.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     4456 2023-02-24 06:47:15.000000 nuxt-0.2.0/nuxt/repositorys/validation.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      149 2023-02-24 04:03:11.000000 nuxt-0.2.0/nuxt/requests.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      459 2023-02-24 03:54:00.000000 nuxt-0.2.0/nuxt/responses.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)       54 2023-02-24 03:40:40.000000 nuxt-0.2.0/nuxt/routing.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     4959 2023-02-23 02:58:43.000000 nuxt-0.2.0/nuxt/staticfiles.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     1249 2023-02-22 06:50:07.000000 nuxt-0.2.0/nuxt/templating.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     3692 2023-02-24 07:04:55.000000 nuxt-0.2.0/nuxt/utils.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      217 2023-02-24 04:13:35.000000 nuxt-0.2.0/requirements.txt
--rw-rw-r--   0 arvin     (1000) arvin     (1000)       38 2023-02-24 08:54:13.000000 nuxt-0.2.0/setup.cfg
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     1394 2023-02-21 09:19:47.000000 nuxt-0.2.0/setup.py
+drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2023-04-23 11:40:05.120805 nuxt-0.2.1/
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      196 2022-10-09 01:47:11.000000 nuxt-0.2.1/MANIFEST.in
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      504 2023-04-23 11:40:05.120805 nuxt-0.2.1/PKG-INFO
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     8888 2023-03-23 04:05:59.000000 nuxt-0.2.1/README.md
+drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2023-04-23 11:40:05.116805 nuxt-0.2.1/nuxt/
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      596 2023-02-24 04:09:14.000000 nuxt-0.2.1/nuxt/__init__.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     6838 2023-03-24 06:13:37.000000 nuxt-0.2.1/nuxt/__main__.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)    15630 2023-02-24 08:39:17.000000 nuxt-0.2.1/nuxt/app.py
+drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2023-04-23 11:40:05.116805 nuxt-0.2.1/nuxt/asyncio/
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      847 2023-02-24 07:48:32.000000 nuxt-0.2.1/nuxt/asyncio/__init__.py
+drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2023-04-23 11:40:05.116805 nuxt-0.2.1/nuxt/asyncio/repositorys/
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)        0 2023-02-23 11:20:39.000000 nuxt-0.2.1/nuxt/asyncio/repositorys/__init__.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     4466 2023-02-24 06:47:45.000000 nuxt-0.2.1/nuxt/asyncio/repositorys/validation.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      111 2023-02-24 03:55:25.000000 nuxt-0.2.1/nuxt/datastructures.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      256 2023-02-24 04:03:52.000000 nuxt-0.2.1/nuxt/exceptions.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     6241 2023-02-24 06:26:12.000000 nuxt-0.2.1/nuxt/openapi.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     3848 2022-10-09 01:47:11.000000 nuxt-0.2.1/nuxt/reloader.py
+drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2023-04-23 11:40:05.120805 nuxt-0.2.1/nuxt/repositorys/
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)        0 2022-10-09 06:50:24.000000 nuxt-0.2.1/nuxt/repositorys/__init__.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)        0 2023-02-23 02:07:26.000000 nuxt-0.2.1/nuxt/repositorys/empty.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     4456 2023-02-24 06:47:15.000000 nuxt-0.2.1/nuxt/repositorys/validation.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      149 2023-02-24 04:03:11.000000 nuxt-0.2.1/nuxt/requests.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      459 2023-02-24 03:54:00.000000 nuxt-0.2.1/nuxt/responses.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)       54 2023-02-24 03:40:40.000000 nuxt-0.2.1/nuxt/routing.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     4959 2023-02-23 02:58:43.000000 nuxt-0.2.1/nuxt/staticfiles.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     1249 2023-02-22 06:50:07.000000 nuxt-0.2.1/nuxt/templating.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     3692 2023-02-24 07:04:55.000000 nuxt-0.2.1/nuxt/utils.py
+drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2023-04-23 11:40:05.116805 nuxt-0.2.1/nuxt.egg-info/
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      504 2023-04-23 11:40:05.000000 nuxt-0.2.1/nuxt.egg-info/PKG-INFO
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      656 2023-04-23 11:40:05.000000 nuxt-0.2.1/nuxt.egg-info/SOURCES.txt
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)        1 2023-04-23 11:40:05.000000 nuxt-0.2.1/nuxt.egg-info/dependency_links.txt
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)       43 2023-04-23 11:40:05.000000 nuxt-0.2.1/nuxt.egg-info/entry_points.txt
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)        1 2023-04-23 11:40:04.000000 nuxt-0.2.1/nuxt.egg-info/not-zip-safe
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      218 2023-04-23 11:40:05.000000 nuxt-0.2.1/nuxt.egg-info/requires.txt
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)       11 2023-04-23 11:40:05.000000 nuxt-0.2.1/nuxt.egg-info/top_level.txt
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      217 2023-04-23 11:36:17.000000 nuxt-0.2.1/requirements.txt
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)       38 2023-04-23 11:40:05.120805 nuxt-0.2.1/setup.cfg
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     1394 2023-04-23 11:36:32.000000 nuxt-0.2.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `nuxt-0.2.0/README.md` & `nuxt-0.2.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,56 @@
-# nuxt
+# Nuxt
 
 Nuxt is a integration framework for build web app with python, built on top of [Madara](https://github.com/Arvintian/madara)/[Starlette](https://github.com/encode/starlette)/[Gunicorn](https://github.com/benoitc/gunicorn)/[Uvicorn](https://github.com/encode/uvicorn).
 
+* [Install](#install)
+* [Usage](#usage)
+* [QuickStart](#quickstart)
+* [User’s Guide](#users-guide)
+    * [Routing](#routing)
+    * [Request](#request)
+    * [Response](#response)
+    * [Template](#template)
+    * [Static](#static)
+    * [Blueprint](#blueprint)
+    * [Middleware](#middleware)
+* [AsyncIO](#asyncio)
+* [API Schemas](#api-schemas)
+* [Design](#design)
+
 ## Install
 
 ```
-
 pip install nuxt
-
 ```
 
 ## Usage
 
 ```
-
 Usage: nuxt [OPTIONS]
 
 Options:
-  --module TEXT           Your python module.
-  --config TEXT           Your nuxt app config json file path.
-  --static TEXT           Your static file directory path.
-  --static-url-path TEXT  Your static url path.
-  --debug BOOLEAN         Enable nuxt app debug mode.
-  --address TEXT          Listen and serve address.
-  --port INTEGER          Listen and serve port.
-  --workers INTEGER       Prefork work count, default is cpu core count.
-  --help                  Show this message and exit.
-
+  --module TEXT            Your python module.
+  --config TEXT            Your nuxt app config json file path.
+  --openapi BOOLEAN        Enable openapi schema and swagger ui.
+  --openapi-url-path TEXT  Openapi schema and ui path, default is /docs
+  --static TEXT            Your static file directory path.
+  --static-index BOOLEAN   Display the index page if path in static is dir.
+  --static-url-path TEXT   Your static url path, default is static directory path basename.
+  --debug BOOLEAN          Enable nuxt app debug mode.
+  --address TEXT           Listen and serve address.
+  --port INTEGER           Listen and serve port.
+  --workers INTEGER        Prefork work count, default is cpu core count.
+  --help                   Show this message and exit.
 ```
 
 
 ## QuickStart
 
 ```
-
 > cat example.py
 
 from nuxt import route
 
 @route("/demo", methods=["GET"])
 def demo(request):
     return {
@@ -50,15 +63,14 @@
 [2021-04-27 12:07:56 +0800] [4284] [INFO] Starting gunicorn 20.1.0
 [2021-04-27 12:07:56 +0800] [4284] [INFO] Listening at: http://0.0.0.0:5000 (4284)
 [2021-04-27 12:07:56 +0800] [4284] [INFO] Using worker: uvicorn.workers.UvicornWorker
 [2021-04-27 12:07:56 +0800] [4287] [INFO] Booting worker with pid: 4287
 [2021-04-27 12:07:56 +0800] [4288] [INFO] Booting worker with pid: 4288
 
 > curl -v http://127.0.0.1:5000/demo
-
 ```
 
 ## User’s Guide
 
 ### Routing
 
 Use the route() decorator to bind a function to a URL.
@@ -116,85 +128,61 @@
 
 The nuxt request object just a warp of [werkzeug request](https://werkzeug.palletsprojects.com/en/1.0.x/wrappers/#werkzeug.wrappers.Request), so your can access request data by werkzeug's methods.
 
 ### Response
 
 The return value from a view function is automatically converted into a [werkzeug response](https://werkzeug.palletsprojects.com/en/1.0.x/wrappers/#werkzeug.wrappers.Response) for you. If the return value is a dict, which will serialize any supported JSON data type and set mimetype to application/json.
 
-### Websocket
-
-Nuxt's websocket route implemented by [starlette](https://www.starlette.io/websockets/). The handler function is a [ASGI](https://asgi.readthedocs.io/en/latest/) application, so you should write the handler function with python's [asyncio](https://docs.python.org/3/library/asyncio.html).
-
-```
-from nuxt import websocket_route,WebSocket
-
-@websocket_route("/ws/echo")
-async def ws_echo(socket: WebSocket):
-    await socket.accept()
-    try:
-        while True:
-            text = await socket.receive_text()
-            await socket.send_text(text)
-    except WebSocketDisconnect as e:
-        pass
-```
 
 ### Template
 
 Nuxt's template engine powered by [jinja](https://jinja.palletsprojects.com/en/3.1.x/).
 
 ```
-
 from nuxt import render_template
 from nuxt import route
 
 @route("/", methods=["GET"])
 def index(request):
     return render_template(request, "index.html", user="Arvin"), {"content-type": "text/html"}
-
 ```
 
 ### Static
 
-Nuxt can be convenient serve static files, internally based on [starlette](https://www.starlette.io/staticfiles/) and [asyncio](https://docs.python.org/3/library/asyncio.html).
+Nuxt can be convenient serve static files.
 
 ```
-
 nuxt --static <directory path> --static-url-path  <request base url path>
-
 ```
 
 ### Blueprint
 
 A Blueprint is a way to organize a group of related views and other code. Rather than registering views and other code directly with an application, they are registered with a blueprint.
 
 ```
-
 from nuxt import Blueprint,register_blueprint
 
 bp_example = Blueprint("bp_example")
 
 @bp_example.route("/item", methods=["POST"])
 def blueprint_route(request: Request):
     data = request.get_json()
     return {
         "code": 0,
         "result": data,
     }
 
 register_blueprint(bp_example, url_prefix="/blueprint")
-
 ```
 
 ### Middleware
 
 Middleware is a framework of hooks into Nuxt’s request/response processing. It’s a light, low-level “plugin” system for globally altering input or output.
 
 ```
-
 class SimpleMiddleware:
 
     def __init__(self, get_response):
         self.get_response = get_response
         # One-time configuration and initialization.
 
     def __call__(self, request):
@@ -209,19 +197,81 @@
         return response
 
     def process_view(self, request, callback, callback_kwargs):
         return None
 
     def process_exception(self, request, exception):
         return None
-
 ```
 
 The `get_response` callable provided by Nuxt might be the actual view (if this is the last listed middleware) or it might be the next middleware in the chain.
 
 `process_view()` is called just before Nuxt calls the view. It should return either None or an response object. If it returns None, Nuxt will continue processing this request, executing any other `process_view()` middleware and, then, the appropriate view. If it returns an response object, Nuxt won’t bother calling the appropriate view; it’ll apply response middleware to that response and return the result.
 
 Nuxt calls `process_exception()` when a view raises an exception. process_exception() should return either None or an response object.
 
-### Design
+
+## AsyncIO
+
+The AsyncIO submodule of Nuxt supports Python's asyncio, allowing Request and Response objects to work in asynchronous mode. Additionally, it enables the implementation of Websockets. Route and Blueprint in an asynchronous manner while maintaining consistency with synchronous mode.
+
+```
+from nuxt.asyncio import Blueprint, register_blueprint
+from nuxt.asyncio import Request, WebSocket, WebSocketDisconnect
+from nuxt.asyncio import route, websocket_route
+
+
+@websocket_route("/ws/echo")
+async def ws_echo(socket: WebSocket):
+    await socket.accept()
+    try:
+        while True:
+            text = await socket.receive_text()
+            recv = "echo:{}".format(text)
+            await socket.send_text(recv)
+    except WebSocketDisconnect as e:
+        pass
+
+
+@route("/user/<string:name>", methods=["GET"])
+async def user_info(request: Request, name):
+    return "hello,{}".format(name)
+
+
+bp_async = Blueprint("bp_async")
+
+
+@bp_async.websocket_route("/ws/echo")
+async def bp_ws_echo(socket: WebSocket):
+    await socket.accept()
+    try:
+        while True:
+            text = await socket.receive_text()
+            recv = "echo:{}".format(text)
+            await socket.send_text(recv)
+    except WebSocketDisconnect as e:
+        pass
+
+
+@bp_async.route("/user/<string:name>", methods=["GET"])
+async def bp_user_info(request, name):
+    return "hello,{}".format(name)
+
+register_blueprint(bp_async, url_prefix="/asyncbp")
+```
+
+In asynchronous mode, nuxt's objects is warp of starlette's [request](https://www.starlette.io/requests/) and [response](https://www.starlette.io/responses/) and [websocket](https://www.starlette.io/websockets/).
+
+
+## API Schemas
+
+Nuxt supports automatically generating API schemas and provides web documentation pages based on Swagger.
+
+```
+nuxt --module example --openapi true
+
+> schemas page on: http://127.0.0.1:5000/docs
+```
+
+## Design
 
 Nuxt use uvicorn web server as the frontend, dispatch http request to wsgi/madara handlers or static file handlers, dispatch websocket request to asgi/starlette handlers.
```

### Comparing `nuxt-0.2.0/nuxt/__init__.py` & `nuxt-0.2.1/nuxt/__init__.py`

 * *Files identical despite different names*

### Comparing `nuxt-0.2.0/nuxt/__main__.py` & `nuxt-0.2.1/nuxt/__main__.py`

 * *Files identical despite different names*

### Comparing `nuxt-0.2.0/nuxt/app.py` & `nuxt-0.2.1/nuxt/app.py`

 * *Files identical despite different names*

### Comparing `nuxt-0.2.0/nuxt/asyncio/__init__.py` & `nuxt-0.2.1/nuxt/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `nuxt-0.2.0/nuxt/asyncio/repositorys/validation.py` & `nuxt-0.2.1/nuxt/asyncio/repositorys/validation.py`

 * *Files identical despite different names*

### Comparing `nuxt-0.2.0/nuxt/openapi.py` & `nuxt-0.2.1/nuxt/openapi.py`

 * *Files identical despite different names*

### Comparing `nuxt-0.2.0/nuxt/reloader.py` & `nuxt-0.2.1/nuxt/reloader.py`

 * *Files identical despite different names*

### Comparing `nuxt-0.2.0/nuxt/repositorys/validation.py` & `nuxt-0.2.1/nuxt/repositorys/validation.py`

 * *Files identical despite different names*

### Comparing `nuxt-0.2.0/nuxt/staticfiles.py` & `nuxt-0.2.1/nuxt/staticfiles.py`

 * *Files identical despite different names*

### Comparing `nuxt-0.2.0/nuxt/templating.py` & `nuxt-0.2.1/nuxt/templating.py`

 * *Files identical despite different names*

### Comparing `nuxt-0.2.0/nuxt/utils.py` & `nuxt-0.2.1/nuxt/utils.py`

 * *Files identical despite different names*

### Comparing `nuxt-0.2.0/setup.py` & `nuxt-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import find_packages
 
 os.chdir(os.path.dirname(sys.argv[0]) or ".")
 here = os.path.abspath(os.path.dirname(__file__))
 
 setup_args = dict(
     name='nuxt',
-    version='0.2.0',
+    version='0.2.1',
     description='A integration framework for build web app.',
     long_description="Nuxt is a integration framework for build web app, built on top of [Madara](https://github.com/Arvintian/madara)/[Starlette](https://github.com/encode/starlette)/[Gunicorn](https://github.com/benoitc/gunicorn)/[Uvicorn](https://github.com/encode/uvicorn).",
     long_description_content_type="text/markdown",
     author='arvin',
     license='MIT',
     url='https://github.com/Arvintian/nuxt',
     author_email='arvintian8@gamil.com',
```

