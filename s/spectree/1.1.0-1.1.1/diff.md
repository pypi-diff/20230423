# Comparing `tmp/spectree-1.1.0.tar.gz` & `tmp/spectree-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectree-1.1.0.tar", last modified: Fri Mar 10 12:50:35 2023, max compression
+gzip compressed data, was "spectree-1.1.1.tar", last modified: Sun Apr 23 04:48:59 2023, max compression
```

## Comparing `spectree-1.1.0.tar` & `spectree-1.1.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:50:35.723417 spectree-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-03-10 12:50:22.000000 spectree-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-10 12:50:22.000000 spectree-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    18765 2023-03-10 12:50:35.723417 spectree-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17412 2023-03-10 12:50:22.000000 spectree-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-03-10 12:50:22.000000 spectree-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-10 12:50:35.723417 spectree-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-03-10 12:50:22.000000 spectree-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:50:35.719417 spectree-1.1.0/spectree/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-03-10 12:50:22.000000 spectree-1.1.0/spectree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-03-10 12:50:22.000000 spectree-1.1.0/spectree/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-03-10 12:50:22.000000 spectree-1.1.0/spectree/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-03-10 12:50:22.000000 spectree-1.1.0/spectree/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-03-10 12:50:22.000000 spectree-1.1.0/spectree/page.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:50:35.723417 spectree-1.1.0/spectree/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-03-10 12:50:22.000000 spectree-1.1.0/spectree/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-03-10 12:50:22.000000 spectree-1.1.0/spectree/plugins/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11761 2023-03-10 12:50:22.000000 spectree-1.1.0/spectree/plugins/falcon_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9960 2023-03-10 12:50:22.000000 spectree-1.1.0/spectree/plugins/flask_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    10359 2023-03-10 12:50:22.000000 spectree-1.1.0/spectree/plugins/quart_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-03-10 12:50:22.000000 spectree-1.1.0/spectree/plugins/starlette_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:50:22.000000 spectree-1.1.0/spectree/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-03-10 12:50:22.000000 spectree-1.1.0/spectree/response.py
--rw-r--r--   0 runner    (1001) docker     (123)    13124 2023-03-10 12:50:22.000000 spectree-1.1.0/spectree/spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     9909 2023-03-10 12:50:22.000000 spectree-1.1.0/spectree/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:50:35.723417 spectree-1.1.0/spectree.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18765 2023-03-10 12:50:35.000000 spectree-1.1.0/spectree.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-03-10 12:50:35.000000 spectree-1.1.0/spectree.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 12:50:35.000000 spectree-1.1.0/spectree.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-03-10 12:50:35.000000 spectree-1.1.0/spectree.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-10 12:50:35.000000 spectree-1.1.0/spectree.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:50:35.723417 spectree-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-03-10 12:50:22.000000 spectree-1.1.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-03-10 12:50:22.000000 spectree-1.1.0/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    11660 2023-03-10 12:50:22.000000 spectree-1.1.0/tests/test_plugin_falcon.py
--rw-r--r--   0 runner    (1001) docker     (123)     8696 2023-03-10 12:50:22.000000 spectree-1.1.0/tests/test_plugin_falcon_asgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     8533 2023-03-10 12:50:22.000000 spectree-1.1.0/tests/test_plugin_flask.py
--rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-03-10 12:50:22.000000 spectree-1.1.0/tests/test_plugin_flask_blueprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-03-10 12:50:22.000000 spectree-1.1.0/tests/test_plugin_flask_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     8219 2023-03-10 12:50:22.000000 spectree-1.1.0/tests/test_plugin_quart.py
--rw-r--r--   0 runner    (1001) docker     (123)    10903 2023-03-10 12:50:22.000000 spectree-1.1.0/tests/test_plugin_starlette.py
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-03-10 12:50:22.000000 spectree-1.1.0/tests/test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-03-10 12:50:22.000000 spectree-1.1.0/tests/test_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-03-10 12:50:22.000000 spectree-1.1.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:48:59.398696 spectree-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-04-23 04:48:45.000000 spectree-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-23 04:48:45.000000 spectree-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    18765 2023-04-23 04:48:59.398696 spectree-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17412 2023-04-23 04:48:45.000000 spectree-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-23 04:48:45.000000 spectree-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 04:48:59.398696 spectree-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-23 04:48:45.000000 spectree-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:48:59.394696 spectree-1.1.1/spectree/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-23 04:48:45.000000 spectree-1.1.1/spectree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-23 04:48:45.000000 spectree-1.1.1/spectree/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-04-23 04:48:45.000000 spectree-1.1.1/spectree/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-04-23 04:48:45.000000 spectree-1.1.1/spectree/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-04-23 04:48:45.000000 spectree-1.1.1/spectree/page.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:48:59.394696 spectree-1.1.1/spectree/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-23 04:48:45.000000 spectree-1.1.1/spectree/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-23 04:48:45.000000 spectree-1.1.1/spectree/plugins/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12063 2023-04-23 04:48:45.000000 spectree-1.1.1/spectree/plugins/falcon_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9960 2023-04-23 04:48:45.000000 spectree-1.1.1/spectree/plugins/flask_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10359 2023-04-23 04:48:45.000000 spectree-1.1.1/spectree/plugins/quart_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-04-23 04:48:45.000000 spectree-1.1.1/spectree/plugins/starlette_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 04:48:45.000000 spectree-1.1.1/spectree/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-04-23 04:48:45.000000 spectree-1.1.1/spectree/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13481 2023-04-23 04:48:45.000000 spectree-1.1.1/spectree/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10040 2023-04-23 04:48:45.000000 spectree-1.1.1/spectree/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:48:59.394696 spectree-1.1.1/spectree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18765 2023-04-23 04:48:59.000000 spectree-1.1.1/spectree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-23 04:48:59.000000 spectree-1.1.1/spectree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 04:48:59.000000 spectree-1.1.1/spectree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-23 04:48:59.000000 spectree-1.1.1/spectree.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-23 04:48:59.000000 spectree-1.1.1/spectree.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:48:59.398696 spectree-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-04-23 04:48:45.000000 spectree-1.1.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-04-23 04:48:45.000000 spectree-1.1.1/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13014 2023-04-23 04:48:45.000000 spectree-1.1.1/tests/test_plugin_falcon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-04-23 04:48:45.000000 spectree-1.1.1/tests/test_plugin_falcon_asgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8663 2023-04-23 04:48:45.000000 spectree-1.1.1/tests/test_plugin_flask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-04-23 04:48:45.000000 spectree-1.1.1/tests/test_plugin_flask_blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-04-23 04:48:45.000000 spectree-1.1.1/tests/test_plugin_flask_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-04-23 04:48:45.000000 spectree-1.1.1/tests/test_plugin_quart.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11246 2023-04-23 04:48:45.000000 spectree-1.1.1/tests/test_plugin_starlette.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-04-23 04:48:45.000000 spectree-1.1.1/tests/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-04-23 04:48:45.000000 spectree-1.1.1/tests/test_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-04-23 04:48:45.000000 spectree-1.1.1/tests/test_utils.py
```

### Comparing `spectree-1.1.0/LICENSE` & `spectree-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spectree-1.1.0/PKG-INFO` & `spectree-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectree
-Version: 1.1.0
+Version: 1.1.1
 Summary: generate OpenAPI document and validate request&response with Python annotations.
 Author-email: Keming Yang <kemingy94@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/0b01001001/spectree
 Project-URL: documentation, https://0b01001001.github.io/spectree/
 Project-URL: repository, https://github.com/0b01001001/spectree
 Project-URL: changelog, https://github.com/0b01001001/spectree/releases
```

### Comparing `spectree-1.1.0/README.md` & `spectree-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `spectree-1.1.0/pyproject.toml` & `spectree-1.1.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "spectree"
-version = "1.1.0"
+version = "1.1.1"
 dynamic = []
 description = "generate OpenAPI document and validate request&response with Python annotations."
 readme = "README.md"
 license = {text = "Apache-2.0"}
 requires-python = ">=3.6"
 authors = [
     { name = "Keming Yang", email = "kemingy94@gmail.com" },
@@ -20,24 +20,25 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dependencies = [
-    "pydantic>=1.2",
+    "pydantic>=1.9.1",
 ]
 
 [project.optional-dependencies]
 dev = [
     "autoflake>=1.4,<3.0",
     "black>=22.3,<24.0",
     "flake8>=4,<7",
     "isort~=5.10",
     "mypy>=0.971",
+    "pre-commit",
     "pytest~=7.1",
 ]
 email = [
     "pydantic[email]>=1.2",
 ]
 falcon = [
     "falcon>=3.0.0",
```

### Comparing `spectree-1.1.0/setup.py` & `spectree-1.1.1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -17,10 +17,11 @@
         "dev": [
             "pytest~=7.1",
             "flake8>=4,<7",
             "black>=22.3,<24.0",
             "isort~=5.10",
             "autoflake>=1.4,<3.0",
             "mypy>=0.971",
+            "syrupy>=4.0.0",
         ],
     },
 )
```

### Comparing `spectree-1.1.0/spectree/config.py` & `spectree-1.1.1/spectree/config.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.0/spectree/models.py` & `spectree-1.1.1/spectree/models.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.0/spectree/page.py` & `spectree-1.1.1/spectree/page.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.0/spectree/plugins/__init__.py` & `spectree-1.1.1/spectree/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.0/spectree/plugins/base.py` & `spectree-1.1.1/spectree/plugins/base.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.0/spectree/plugins/falcon_plugin.py` & `spectree-1.1.1/spectree/plugins/falcon_plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -228,24 +228,30 @@
 
         if resp and resp.has_model():
             model = resp.find_model(_resp.status[:3])
             if model and isinstance(_resp.media, model):
                 _resp.media = _resp.media.dict()
                 skip_validation = True
 
+            if self._data_set_manually(_resp):
+                skip_validation = True
+
             if model and not skip_validation:
                 try:
                     model.parse_obj(_resp.media)
                 except ValidationError as err:
                     resp_validation_error = err
                     _resp.status = HTTP_500
                     _resp.media = err.errors()
 
         after(_req, _resp, resp_validation_error, _self)
 
+    def _data_set_manually(self, resp):
+        return (resp.text is not None or resp.data is not None) and resp.media is None
+
     def bypass(self, func, method):
         if isinstance(func, partial):
             return True
         return inspect.isfunction(func)
 
 
 class FalconAsgiPlugin(FalconPlugin):
@@ -324,14 +330,17 @@
 
         if resp and resp.has_model():
             model = resp.find_model(_resp.status[:3])
             if model and isinstance(_resp.media, model):
                 _resp.media = _resp.media.dict()
                 skip_validation = True
 
+            if self._data_set_manually(_resp):
+                skip_validation = True
+
             model = resp.find_model(_resp.status[:3])
             if model and not skip_validation:
                 try:
                     model.parse_obj(_resp.media)
                 except ValidationError as err:
                     resp_validation_error = err
                     _resp.status = HTTP_500
```

### Comparing `spectree-1.1.0/spectree/plugins/flask_plugin.py` & `spectree-1.1.1/spectree/plugins/flask_plugin.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.0/spectree/plugins/quart_plugin.py` & `spectree-1.1.1/spectree/plugins/quart_plugin.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.0/spectree/plugins/starlette_plugin.py` & `spectree-1.1.1/spectree/plugins/starlette_plugin.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.0/spectree/spec.py` & `spectree-1.1.1/spectree/spec.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Mapping,
     Optional,
     Sequence,
     Type,
     get_type_hints,
 )
 
-from ._types import FunctionDecorator, ModelType
+from ._types import FunctionDecorator, ModelType, NamingStrategy
 from .config import Configuration, ModeEnum
 from .models import Tag, ValidationError
 from .plugins import PLUGINS, BasePlugin
 from .response import Response
 from .utils import (
     default_after_handler,
     default_before_handler,
@@ -33,41 +33,45 @@
 
 
 class SpecTree:
     """
     Interface
 
     :param str backend_name: choose from ('flask', 'falcon', 'falcon-asgi', 'starlette')
-    :param backend: a backend that inherit `SpecTree.plugins.base.BasePlugin`
+    :param backend: a backend that inherit `SpecTree.plugins.base.BasePlugin`, this will
+        override the `backend_name` if provided
     :param app: backend framework application instance (can be registered later)
     :param before: a callback function of the form
         :meth:`spectree.utils.default_before_handler`
         ``func(req, resp, req_validation_error, instance)``
         that will be called after the request validation before the endpoint function
     :param after: a callback function of the form
         :meth:`spectree.utils.default_after_handler`
         ``func(req, resp, resp_validation_error, instance)``
         that will be called after the response validation
     :param validation_error_status: The default response status code to use in the
         event of a validation error. This value can be overridden for specific endpoints
         if needed.
-    :param kwargs: init :class:`spectree.config.Configuration`
+    :param kwargs: init :class:`spectree.config.Configuration`, they can also be
+        configured through the environment variables with prefix `spectree_`
     """
 
     def __init__(
         self,
         backend_name: str = "base",
         backend: Optional[Type[BasePlugin]] = None,
         app: Any = None,
         before: Callable = default_before_handler,
         after: Callable = default_after_handler,
         validation_error_status: int = 422,
         validation_error_model: Optional[ModelType] = None,
+        naming_strategy: NamingStrategy = get_model_key,
         **kwargs: Any,
     ):
+        self.naming_strategy = naming_strategy
         self.before = before
         self.after = after
         self.validation_error_status = validation_error_status
         self.validation_error_model = validation_error_model or ValidationError
         self.config: Configuration = Configuration.parse_obj(kwargs)
         self.backend_name = backend_name
         if backend:
@@ -251,16 +255,18 @@
         return decorate_validation
 
     def _add_model(self, model: ModelType) -> str:
         """
         unified model processing
         """
 
-        model_key = get_model_key(model=model)
-        self.models[model_key] = deepcopy(get_model_schema(model=model))
+        model_key = self.naming_strategy(model)
+        self.models[model_key] = deepcopy(
+            get_model_schema(model=model, naming_strategy=self.naming_strategy)
+        )
 
         return model_key
 
     def _generate_spec(self) -> Dict[str, Any]:
         """
         generate OpenAPI spec according to routes and decorators
         """
@@ -293,15 +299,15 @@
 
                 routes[path][method.lower()] = {
                     "summary": summary or f"{name} <{method}>",
                     "operationId": operation_id,
                     "description": desc or "",
                     "tags": [str(x) for x in getattr(func, "tags", ())],
                     "parameters": parse_params(func, parameters[:], self.models),
-                    "responses": parse_resp(func),
+                    "responses": parse_resp(func, self.naming_strategy),
                 }
 
                 security = getattr(func, "security", None)
                 if security is not None:
                     routes[path][method.lower()]["security"] = get_security(security)
 
                 deprecated = getattr(func, "deprecated", False)
```

### Comparing `spectree-1.1.0/spectree/utils.py` & `spectree-1.1.1/spectree/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     Tuple,
     Type,
     Union,
 )
 
 from pydantic import BaseModel, ValidationError
 
-from ._types import ModelType, MultiDict
+from ._types import ModelType, MultiDict, NamingStrategy
 
 # parse HTTP status code to get the code
 HTTP_CODE = re.compile(r"^HTTP_(?P<code>\d{3})$")
 
 RE_FLASK_RULE = re.compile(
     r"""
     (?P<static>[^<]*)                           # static rule data
@@ -127,29 +127,14 @@
                         **extra,
                     }
                 )
 
     return params
 
 
-def parse_resp(func: Any):
-    """
-    get the response spec
-
-    If this function does not have explicit ``resp`` but have other models,
-    a ``422 Validation Error`` will be appended to the response spec, since
-    this may be triggered in the validation step.
-    """
-    responses = {}
-    if hasattr(func, "resp"):
-        responses = func.resp.generate_spec()
-
-    return responses
-
-
 def has_model(func: Any) -> bool:
     """
     return True if this function have ``pydantic.BaseModel``
     """
     if any(hasattr(func, x) for x in ("query", "json", "headers")):
         return True
 
@@ -240,26 +225,26 @@
     :param model: `pydantic.BaseModel` query, json, headers or cookies from
         request or response
     """
 
     return f"{model.__name__}.{hash_module_path(module_path=model.__module__)}"
 
 
-def get_model_schema(model: ModelType):
+def get_model_schema(model: ModelType, naming_strategy: NamingStrategy = get_model_key):
     """
     return a dictionary representing the model as JSON Schema with a hashed
     infix in ref to ensure name uniqueness
 
     :param model: `pydantic.BaseModel` query, json, headers or cookies from
         request or response
     """
     assert issubclass(model, BaseModel)
 
     return model.schema(
-        ref_template=f"#/components/schemas/{get_model_key(model)}.{{model}}"
+        ref_template=f"#/components/schemas/{naming_strategy(model)}.{{model}}"
     )
 
 
 def get_security(security: Union[None, Mapping, Sequence[Any]]) -> List[Any]:
     """
     return the correct format of security
     """
@@ -330,7 +315,22 @@
         yield converter, data["args"] or None, variable
         pos = m.end()
     if pos < end:
         remaining = rule[pos:]
         if ">" in remaining or "<" in remaining:
             raise ValueError(f"malformed url rule: {rule!r}")
         yield None, None, remaining
+
+
+def parse_resp(func: Any, naming_strategy: NamingStrategy = get_model_key):
+    """
+    get the response spec
+
+    If this function does not have explicit ``resp`` but have other models,
+    a ``422 Validation Error`` will be appended to the response spec, since
+    this may be triggered in the validation step.
+    """
+    responses = {}
+    if hasattr(func, "resp"):
+        responses = func.resp.generate_spec(naming_strategy)
+
+    return responses
```

### Comparing `spectree-1.1.0/spectree.egg-info/PKG-INFO` & `spectree-1.1.1/spectree.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectree
-Version: 1.1.0
+Version: 1.1.1
 Summary: generate OpenAPI document and validate request&response with Python annotations.
 Author-email: Keming Yang <kemingy94@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/0b01001001/spectree
 Project-URL: documentation, https://0b01001001.github.io/spectree/
 Project-URL: repository, https://github.com/0b01001001/spectree
 Project-URL: changelog, https://github.com/0b01001001/spectree/releases
```

### Comparing `spectree-1.1.0/spectree.egg-info/SOURCES.txt` & `spectree-1.1.1/spectree.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spectree-1.1.0/tests/test_config.py` & `spectree-1.1.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.0/tests/test_plugin_falcon.py` & `spectree-1.1.1/tests/test_plugin_falcon.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from spectree import Response, SpecTree
 
 from .common import (
     JSON,
     Cookies,
     FormFileUpload,
     Headers,
+    ListJSON,
     Query,
     Resp,
     StrDict,
     api_tag,
 )
 
 
@@ -181,23 +182,51 @@
     )
     def on_post(self, req, resp, form: FormFileUpload):
         assert form.file
         file_content = form.file
         resp.media = {"file": file_content.decode("utf-8")}
 
 
+class ListJsonView:
+    name = "json list request view"
+
+    @api.validate(
+        json=ListJSON,
+    )
+    def on_post(self, req, resp, json: ListJSON):
+        pass
+
+
+class ViewWithCustomSerializer:
+    name = "view with custom serializer"
+
+    @api.validate(
+        resp=Response(HTTP_200=Resp),
+    )
+    def on_get(self, req, resp):
+        resp.data = Resp(name="falcon", score=[1, 2, 3]).json().encode("utf-8")
+
+    @api.validate(
+        resp=Response(HTTP_200=Resp),
+    )
+    def on_post(self, req, resp):
+        resp.text = Resp(name="falcon", score=[1, 2, 3]).json()
+
+
 app = App()
 app.add_route("/ping", Ping())
 app.add_route("/api/user/{name}", UserScore())
 app.add_route("/api/user_annotated/{name}", UserScoreAnnotated())
 app.add_route("/api/user/{name}/address/{address_id}", UserAddress())
 app.add_route("/api/user_skip/{name}", UserScoreSkip())
 app.add_route("/api/user_model/{name}", UserScoreModel())
 app.add_route("/api/no_response", NoResponseView())
 app.add_route("/api/file_upload", FileUploadView())
+app.add_route("/api/list_json", ListJsonView())
+app.add_route("/api/custom_serializer", ViewWithCustomSerializer())
 api.register(app)
 
 
 @pytest.fixture
 def client():
     return testing.TestClient(app)
 
@@ -282,14 +311,23 @@
     resp = client.simulate_request(
         "GET",
         "/api/no_response",
     )
     assert resp.status_code == 200
 
 
+def test_falcon_list_json_request_sync(client):
+    resp = client.simulate_request(
+        "POST",
+        "/api/list_json",
+        json=[dict(name="foo", limit=1)],
+    )
+    assert resp.status_code == 200
+
+
 @pytest.fixture
 def test_client_and_api(request):
     api_args = ["falcon"]
     api_kwargs = {}
     endpoint_kwargs = {
         "headers": Headers,
         "resp": Response(HTTP_200=StrDict),
@@ -401,7 +439,23 @@
             "Content-Type": "multipart/form-data; boundary=%s" % boundary,
         },
         body=body.encode("utf-8"),
     )
     assert resp.status_code == 200, resp.text
     assert resp.headers["content-type"] == "application/json"
     assert resp.json["file"] == file_content
+
+
+def test_falcon_custom_serializer(client):
+    resp = client.simulate_get(
+        "/api/custom_serializer",
+    )
+    assert resp.status_code == 200
+    assert resp.json["name"] == "falcon"
+    assert resp.json["score"] == [1, 2, 3]
+
+    resp = client.simulate_post(
+        "/api/custom_serializer",
+    )
+    assert resp.status_code == 200
+    assert resp.json["name"] == "falcon"
+    assert resp.json["score"] == [1, 2, 3]
```

### Comparing `spectree-1.1.0/tests/test_plugin_falcon_asgi.py` & `spectree-1.1.1/tests/test_plugin_falcon_asgi.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from spectree import Response, SpecTree
 
 from .common import (
     JSON,
     Cookies,
     FormFileUpload,
     Headers,
+    ListJSON,
     Query,
     Resp,
     StrDict,
     api_tag,
 )
 
 
@@ -106,32 +107,60 @@
     @api.validate(
         json=StrDict,  # resp is missing completely
     )
     async def on_post(self, req, resp, json: JSON):
         pass
 
 
+class ListJsonView:
+    name = "json list request view"
+
+    @api.validate(
+        json=ListJSON,
+    )
+    async def on_post(self, req, resp, json: ListJSON):
+        pass
+
+
 class FileUploadView:
     name = "file upload view"
 
     @api.validate(
         form=FormFileUpload,
     )
     async def on_post(self, req, resp, form: FormFileUpload):
         assert form.file
         file_content = await form.file.get_data()
         resp.media = {"file": file_content.decode("utf-8")}
 
 
+class ViewWithCustomSerializer:
+    name = "view with custom serializer"
+
+    @api.validate(
+        resp=Response(HTTP_200=Resp),
+    )
+    async def on_get(self, req, resp):
+        resp.data = Resp(name="falcon", score=[1, 2, 3]).json().encode("utf-8")
+
+    @api.validate(
+        resp=Response(HTTP_200=Resp),
+    )
+    async def on_post(self, req, resp):
+        resp.text = Resp(name="falcon", score=[1, 2, 3]).json()
+
+
 app = App()
 app.add_route("/ping", Ping())
 app.add_route("/api/user/{name}", UserScore())
 app.add_route("/api/user_annotated/{name}", UserScoreAnnotated())
 app.add_route("/api/no_response", NoResponseView())
 app.add_route("/api/file_upload", FileUploadView())
+app.add_route("/api/list_json", ListJsonView())
+app.add_route("/api/custom_serializer", ViewWithCustomSerializer())
 api.register(app)
 
 
 @pytest.fixture
 def client():
     return testing.TestClient(app)
 
@@ -147,14 +176,23 @@
         "POST",
         "/api/no_response",
         json=dict(name="foo", limit=1),
     )
     assert resp.status_code == 200
 
 
+def test_falcon_list_json_request_async(client):
+    resp = client.simulate_request(
+        "POST",
+        "/api/list_json",
+        json=[dict(name="foo", limit=1)],
+    )
+    assert resp.status_code == 200
+
+
 def test_falcon_validate(client):
     resp = client.simulate_request(
         "GET", "/ping", headers={"Content-Type": "text/plain"}
     )
     assert resp.status_code == 422
     assert resp.headers.get("X-Error") == "Validation Error", resp.headers
 
@@ -310,7 +348,23 @@
         headers={
             "Content-Type": "multipart/form-data; boundary=%s" % boundary,
         },
         body=body.encode("utf-8"),
     )
     assert resp.status_code == 200, resp.text
     assert resp.json["file"] == file_content
+
+
+def test_falcon_custom_serializer(client):
+    resp = client.simulate_get(
+        "/api/custom_serializer",
+    )
+    assert resp.status_code == 200
+    assert resp.json["name"] == "falcon"
+    assert resp.json["score"] == [1, 2, 3]
+
+    resp = client.simulate_post(
+        "/api/custom_serializer",
+    )
+    assert resp.status_code == 200
+    assert resp.json["name"] == "falcon"
+    assert resp.json["score"] == [1, 2, 3]
```

### Comparing `spectree-1.1.0/tests/test_plugin_flask.py` & `spectree-1.1.1/tests/test_plugin_flask.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from .common import (
     JSON,
     SECURITY_SCHEMAS,
     Cookies,
     Form,
     FormFileUpload,
     Headers,
+    ListJSON,
     Order,
     Query,
     Resp,
     StrDict,
     api_tag,
 )
 
@@ -155,14 +156,22 @@
 @api.validate(
     json=StrDict,
 )
 def no_response():
     return {}
 
 
+@app.route("/api/list_json", methods=["POST"])
+@api.validate(
+    json=ListJSON,
+)
+def json_list():
+    return {}
+
+
 # INFO: ensures that spec is calculated and cached _after_ registering
 # view functions for validations. This enables tests to access `api.spec`
 # without app_context.
 with app.app_context():
     api.spec
 api.register(app)
```

### Comparing `spectree-1.1.0/tests/test_plugin_flask_blueprint.py` & `spectree-1.1.1/tests/test_plugin_flask_blueprint.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from .common import (
     JSON,
     Cookies,
     Form,
     FormFileUpload,
     Headers,
+    ListJSON,
     Order,
     Query,
     Resp,
     StrDict,
     api_tag,
     get_paths,
 )
@@ -144,14 +145,22 @@
 @api.validate(
     json=StrDict,
 )
 def no_response():
     return {}
 
 
+@app.route("/api/list_json", methods=["POST"])
+@api.validate(
+    json=ListJSON,
+)
+def list_json():
+    return {}
+
+
 api.register(app)
 
 flask_app = Flask(__name__)
 flask_app.register_blueprint(app)
 with flask_app.app_context():
     api.spec
```

### Comparing `spectree-1.1.0/tests/test_plugin_flask_view.py` & `spectree-1.1.1/tests/test_plugin_flask_view.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 from .common import (
     JSON,
     Cookies,
     Form,
     FormFileUpload,
     Headers,
+    ListJSON,
     Order,
     Query,
     Resp,
     StrDict,
     api_tag,
 )
 
@@ -155,14 +156,22 @@
     @api.validate(
         json=StrDict,  # resp is missing completely
     )
     def post(self, json: JSON):
         return {}
 
 
+class ListJsonView(MethodView):
+    @api.validate(
+        json=ListJSON,
+    )
+    def post(self):
+        return {}
+
+
 app.add_url_rule("/ping", view_func=Ping.as_view("ping"))
 app.add_url_rule("/api/user/<name>", view_func=User.as_view("user"), methods=["POST"])
 app.add_url_rule(
     "/api/user_annotated/<name>",
     view_func=UserAnnotated.as_view("user_annotated"),
     methods=["POST"],
 )
@@ -185,14 +194,18 @@
     "/api/no_response",
     view_func=NoResponseView.as_view("no_response_view"),
 )
 app.add_url_rule(
     "/api/file_upload",
     view_func=FileUploadView.as_view("file_upload_view"),
 )
+app.add_url_rule(
+    "/api/list_json",
+    view_func=ListJsonView.as_view("list_json_view"),
+)
 
 # INFO: ensures that spec is calculated and cached _after_ registering
 # view functions for validations. This enables tests to access `api.spec`
 # without app_context.
 with app.app_context():
     api.spec
```

### Comparing `spectree-1.1.0/tests/test_plugin_quart.py` & `spectree-1.1.1/tests/test_plugin_quart.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from spectree import Response, SpecTree
 
 from .common import (
     JSON,
     SECURITY_SCHEMAS,
     Cookies,
     Headers,
+    ListJSON,
     Order,
     Query,
     Resp,
     StrDict,
     api_tag,
 )
 
@@ -137,14 +138,22 @@
 @api.validate(
     json=JSON,
 )
 async def no_response():
     return {}
 
 
+@app.route("/api/list_json", methods=["POST"])
+@api.validate(
+    json=ListJSON,
+)
+async def list_json():
+    return {}
+
+
 # INFO: ensures that spec is calculated and cached _after_ registering
 # view functions for validations. This enables tests to access `api.spec`
 # without app_context.
 # with app.app_context():
 #     api.spec
 api.register(app)
```

### Comparing `spectree-1.1.0/tests/test_plugin_starlette.py` & `spectree-1.1.1/tests/test_plugin_starlette.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from spectree.plugins.starlette_plugin import PydanticResponse
 
 from .common import (
     JSON,
     Cookies,
     FormFileUpload,
     Headers,
+    ListJSON,
     Order,
     Query,
     Resp,
     StrDict,
     api_tag,
 )
 
@@ -130,14 +131,21 @@
     json=StrDict,
     resp=Response(HTTP_200=None),
 )
 async def no_response(request):
     return JSONResponse({})
 
 
+@api.validate(
+    json=ListJSON,
+)
+async def list_json(request):
+    return JSONResponse({})
+
+
 app = Starlette(
     routes=[
         Route("/ping", Ping),
         Mount(
             "/api",
             routes=[
                 Mount(
@@ -162,14 +170,15 @@
                     "/user_model",
                     routes=[
                         Route("/{name}", user_score_model, methods=["POST"]),
                     ],
                 ),
                 Route("/no_response", no_response, methods=["POST", "GET"]),
                 Route("/file_upload", file_upload, methods=["POST"]),
+                Route("/list_json", list_json, methods=["POST"]),
             ],
         ),
         Mount("/static", app=StaticFiles(directory="docs"), name="static"),
     ]
 )
 
 
@@ -355,14 +364,19 @@
     resp = client.get("/api/no_response")
     assert resp.status_code == 200, resp.text
 
     resp = client.post("/api/no_response", json={"name": "starlette", "limit": 1})
     assert resp.status_code == 200, resp.text
 
 
+def test_json_list_request(client):
+    resp = client.post("/api/list_json", json=[{"name": "starlette", "limit": 1}])
+    assert resp.status_code == 200, resp.text
+
+
 def test_starlette_upload_file(client):
     file_content = "abcdef"
     file_io = io.BytesIO(file_content.encode("utf-8"))
     resp = client.post(
         "/api/file_upload",
         files={"file": ("test.txt", file_io, "text/plain")},
     )
```

### Comparing `spectree-1.1.0/tests/test_response.py` & `spectree-1.1.1/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.0/tests/test_spec.py` & `spectree-1.1.1/tests/test_spec.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.0/tests/test_utils.py` & `spectree-1.1.1/tests/test_utils.py`

 * *Files identical despite different names*

