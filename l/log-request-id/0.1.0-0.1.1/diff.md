# Comparing `tmp/log_request_id-0.1.0.tar.gz` & `tmp/log_request_id-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "log_request_id-0.1.0.tar", max compression
+gzip compressed data, was "log_request_id-0.1.1.tar", max compression
```

## Comparing `log_request_id-0.1.0.tar` & `log_request_id-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1075 2023-04-01 20:44:23.120296 log_request_id-0.1.0/LICENSE
--rw-r--r--   0        0        0     1468 2023-04-02 18:57:57.700124 log_request_id-0.1.0/README.rst
--rw-r--r--   0        0        0       24 2023-04-02 18:57:57.700866 log_request_id-0.1.0/log_request_id/__init__.py
--rw-r--r--   0        0        0     1553 2023-04-02 18:57:57.701106 log_request_id-0.1.0/log_request_id/flask.py
--rw-r--r--   0        0        0     1155 2023-04-01 19:57:10.419717 log_request_id-0.1.0/log_request_id/logging.py
--rw-r--r--   0        0        0      695 2023-04-01 20:42:51.994153 log_request_id-0.1.0/log_request_id/request_id.py
--rw-r--r--   0        0        0      662 2023-04-02 18:57:57.701302 log_request_id-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2138 1970-01-01 00:00:00.000000 log_request_id-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-04-02 10:32:16.842007 log_request_id-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1468 2023-04-02 12:02:10.180489 log_request_id-0.1.1/README.rst
+-rw-r--r--   0        0        0       24 2023-04-02 12:02:11.744521 log_request_id-0.1.1/log_request_id/__init__.py
+-rw-r--r--   0        0        0     2017 2023-04-23 13:07:37.558137 log_request_id-0.1.1/log_request_id/flask.py
+-rw-r--r--   0        0        0     1155 2023-04-01 14:41:31.633053 log_request_id-0.1.1/log_request_id/logging.py
+-rw-r--r--   0        0        0      772 2023-04-23 12:32:48.158879 log_request_id-0.1.1/log_request_id/request_id.py
+-rw-r--r--   0        0        0      662 2023-04-23 12:42:18.655677 log_request_id-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2107 1970-01-01 00:00:00.000000 log_request_id-0.1.1/setup.py
+-rw-r--r--   0        0        0     2138 1970-01-01 00:00:00.000000 log_request_id-0.1.1/PKG-INFO
```

### Comparing `log_request_id-0.1.0/LICENSE` & `log_request_id-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `log_request_id-0.1.0/README.rst` & `log_request_id-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `log_request_id-0.1.0/log_request_id/flask.py` & `log_request_id-0.1.1/log_request_id/flask.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,60 @@
 import os
+from collections.abc import Callable
 from typing import Optional
-from .request_id import DEFAULT_REQUEST_ID_OBJECT_NAME, default_request_id_generator, register_context_getter
 
+from .request_id import (DEFAULT_REQUEST_ID_OBJECT_NAME,
+                         default_request_id_generator, register_context_getter)
 
-@register_context_getter(skip=os.getenv('LOG_REQUEST_ID_FRAMEWORK_SUPPORT') == 'flask')
-def get_flask_context_request_id(request_id_object_name=None):
+
+@register_context_getter(skip=os.getenv("LOG_REQUEST_ID_FRAMEWORK_SUPPORT") == "flask")
+def get_flask_context_request_id(request_id_object_name=DEFAULT_REQUEST_ID_OBJECT_NAME):
     from flask import g, has_request_context
 
-    request_id_object_name = request_id_object_name or DEFAULT_REQUEST_ID_OBJECT_NAME
     return g.get(request_id_object_name, None) if has_request_context() else None
 
 
-def init_flask_request_id_handler(app, request_id_object_name: Optional[str] = None, request_id_generator=None):
-    app.before_request(lambda : propagate_flask_request_id(request_id_object_name, request_id_generator))
+def init_flask_request_id_handler(
+    app,
+    request_id_object_name: str = DEFAULT_REQUEST_ID_OBJECT_NAME,
+    request_id_generator: Callable = default_request_id_generator,
+):
+    app.before_request(
+        lambda: _init_request_id(
+            request_id_object_name=request_id_object_name, request_id_generator=request_id_generator
+        )
+    )
+    app.after_request(lambda response: _set_response_header(response, request_id_object_name=request_id_object_name))
+
+
+def _init_request_id(
+    request_id_object_name: str = DEFAULT_REQUEST_ID_OBJECT_NAME,
+    request_id_generator: Callable = default_request_id_generator,
+):
+    from flask import g, has_request_context, request
+
+    request_id = request.headers.get("X-Request-ID", request_id_generator())
+
+    if has_request_context() and g.get(request_id_object_name) is None:
+        setattr(g, request_id_object_name, request_id)
 
 
-def propagate_flask_request_id(request_id = None, request_id_object_name: Optional[str] = None, request_id_generator=None):
+def _set_response_header(
+    response,
+    request_id_object_name: str = DEFAULT_REQUEST_ID_OBJECT_NAME,
+):
     from flask import g, has_request_context
 
-    request_id_generator = request_id_generator or default_request_id_generator
-    request_id_object_name = request_id_object_name or DEFAULT_REQUEST_ID_OBJECT_NAME
-    request_id = request_id or request_id_generator()
+    if has_request_context():
+        request_id = g.get(request_id_object_name)
+        response.headers.add("X-Request-ID", request_id)
 
-    if has_request_context() and g.get(request_id_object_name) is None:
-        setattr(g, request_id_object_name, request_id_generator())
+    return response
 
 
 def suppress_flask_request_id(request_id_object_name: Optional[str] = None):
     from flask import g, has_request_context
+
     request_id_object_name = request_id_object_name or DEFAULT_REQUEST_ID_OBJECT_NAME
 
     if has_request_context():
         g.pop(request_id_object_name, None)
```

### Comparing `log_request_id-0.1.0/log_request_id/logging.py` & `log_request_id-0.1.1/log_request_id/logging.py`

 * *Files identical despite different names*

### Comparing `log_request_id-0.1.0/log_request_id/request_id.py` & `log_request_id-0.1.1/log_request_id/request_id.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+from collections.abc import Callable
+from typing import List
 import uuid
 import functools
 import os
 
 DEFAULT_REQUEST_ID_OBJECT_NAME: str = os.getenv('DEFAULT_REQUEST_ID_OBJECT_NAME', default='request_id')
-REQUEST_ID_CONTEXT_GETTERS = []
+REQUEST_ID_CONTEXT_GETTERS: List[Callable] = []
 
 
 def current_request_id():
     for request_id_context_getter in REQUEST_ID_CONTEXT_GETTERS:
         request_id = request_id_context_getter()
 
         if request_id is not None:
```

### Comparing `log_request_id-0.1.0/pyproject.toml` & `log_request_id-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 | docs
 | \.github
 )/
 '''
 
 [tool.poetry]
 name = "log-request-id"
-version = "0.1.0"
+version = "0.1.1"
 description = "Log-Request-ID is extension for handling request-ID in logging."
 authors = ["kuzxnia <kacper.kuzniarski@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 packages = [{include = "log_request_id"}]
 
 [tool.poetry.dependencies]
```

### Comparing `log_request_id-0.1.0/PKG-INFO` & `log_request_id-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: log-request-id
-Version: 0.1.0
+Version: 0.1.1
 Summary: Log-Request-ID is extension for handling request-ID in logging.
 License: MIT
 Author: kuzxnia
 Author-email: kacper.kuzniarski@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

