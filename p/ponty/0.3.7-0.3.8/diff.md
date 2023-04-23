# Comparing `tmp/ponty-0.3.7.tar.gz` & `tmp/ponty-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ponty-0.3.7.tar", last modified: Wed Apr  5 02:39:31 2023, max compression
+gzip compressed data, was "ponty-0.3.8.tar", last modified: Sun Apr 23 20:18:26 2023, max compression
```

## Comparing `ponty-0.3.7.tar` & `ponty-0.3.8.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-05 02:39:31.171057 ponty-0.3.7/
--rw-r--r--   0 chris      (502) staff       (20)     1015 2023-04-05 02:39:31.170801 ponty-0.3.7/PKG-INFO
--rw-r--r--   0 chris      (502) staff       (20)     1940 2023-04-03 01:28:51.000000 ponty-0.3.7/README.rst
-drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-05 02:39:31.162569 ponty-0.3.7/ponty/
--rw-r--r--   0 chris      (502) staff       (20)     1286 2023-04-01 19:00:59.000000 ponty-0.3.7/ponty/__init__.py
--rw-r--r--   0 chris      (502) staff       (20)     3577 2022-08-25 19:47:44.000000 ponty-0.3.7/ponty/errors.py
-drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-05 02:39:31.165487 ponty-0.3.7/ponty/http/
--rw-r--r--   0 chris      (502) staff       (20)     1177 2023-04-01 18:50:48.000000 ponty-0.3.7/ponty/http/__init__.py
--rw-r--r--   0 chris      (502) staff       (20)     2837 2022-08-16 02:37:27.000000 ponty-0.3.7/ponty/http/client.py
-drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-05 02:39:31.167522 ponty-0.3.7/ponty/http/expect/
--rw-r--r--   0 chris      (502) staff       (20)     1734 2023-04-01 19:01:48.000000 ponty-0.3.7/ponty/http/expect/__init__.py
--rw-r--r--   0 chris      (502) staff       (20)     7733 2023-03-25 04:24:20.000000 ponty-0.3.7/ponty/http/expect/body.py
--rw-r--r--   0 chris      (502) staff       (20)     1097 2023-03-25 04:25:33.000000 ponty-0.3.7/ponty/http/expect/header.py
--rw-r--r--   0 chris      (502) staff       (20)     8854 2023-04-05 02:19:47.000000 ponty-0.3.7/ponty/http/expect/query.py
--rw-r--r--   0 chris      (502) staff       (20)     3453 2023-04-01 15:19:30.000000 ponty-0.3.7/ponty/http/expect/req.py
--rw-r--r--   0 chris      (502) staff       (20)     2586 2023-03-30 20:00:27.000000 ponty-0.3.7/ponty/http/expect/route.py
--rw-r--r--   0 chris      (502) staff       (20)     1129 2022-12-29 15:32:54.000000 ponty-0.3.7/ponty/http/go.py
--rw-r--r--   0 chris      (502) staff       (20)     1379 2023-02-22 03:26:42.000000 ponty-0.3.7/ponty/http/render.py
--rw-r--r--   0 chris      (502) staff       (20)       53 2023-04-02 02:02:29.000000 ponty-0.3.7/ponty/http/response.py
--rw-r--r--   0 chris      (502) staff       (20)     1797 2022-08-16 03:05:39.000000 ponty-0.3.7/ponty/http/routes.py
-drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-05 02:39:31.168198 ponty-0.3.7/ponty/http/schema/
--rw-r--r--   0 chris      (502) staff       (20)      750 2022-08-14 21:35:59.000000 ponty-0.3.7/ponty/http/schema/__init__.py
--rw-r--r--   0 chris      (502) staff       (20)     9102 2023-02-22 03:26:42.000000 ponty-0.3.7/ponty/http/schema/build.py
-drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-05 02:39:31.168482 ponty-0.3.7/ponty/memo/
--rw-r--r--   0 chris      (502) staff       (20)      384 2022-06-15 03:02:09.000000 ponty-0.3.7/ponty/memo/__init__.py
-drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-05 02:39:31.169723 ponty-0.3.7/ponty/memo/cache/
--rw-r--r--   0 chris      (502) staff       (20)        0 2022-06-14 14:23:14.000000 ponty-0.3.7/ponty/memo/cache/__init__.py
--rw-r--r--   0 chris      (502) staff       (20)     4719 2022-09-18 04:30:56.000000 ponty-0.3.7/ponty/memo/cache/base.py
--rw-r--r--   0 chris      (502) staff       (20)     5525 2022-08-26 12:08:34.000000 ponty-0.3.7/ponty/memo/cache/local.py
--rw-r--r--   0 chris      (502) staff       (20)      105 2022-08-04 15:34:08.000000 ponty-0.3.7/ponty/memo/cache/stats.py
-drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-05 02:39:31.170426 ponty-0.3.7/ponty/memo/lock/
--rw-r--r--   0 chris      (502) staff       (20)        0 2022-06-14 14:23:02.000000 ponty-0.3.7/ponty/memo/lock/__init__.py
--rw-r--r--   0 chris      (502) staff       (20)     3178 2022-08-26 11:55:35.000000 ponty-0.3.7/ponty/memo/lock/base.py
--rw-r--r--   0 chris      (502) staff       (20)     3010 2022-08-26 12:11:57.000000 ponty-0.3.7/ponty/memo/lock/local.py
--rw-r--r--   0 chris      (502) staff       (20)        0 2022-07-10 14:41:50.000000 ponty-0.3.7/ponty/py.typed
--rw-r--r--   0 chris      (502) staff       (20)      472 2022-07-08 01:41:18.000000 ponty-0.3.7/ponty/registry.py
--rw-r--r--   0 chris      (502) staff       (20)      269 2023-01-23 03:15:06.000000 ponty-0.3.7/ponty/types_.py
--rw-r--r--   0 chris      (502) staff       (20)     3701 2022-08-23 13:26:59.000000 ponty-0.3.7/ponty/utils.py
-drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-05 02:39:31.163535 ponty-0.3.7/ponty.egg-info/
--rw-r--r--   0 chris      (502) staff       (20)     1015 2023-04-05 02:39:31.000000 ponty-0.3.7/ponty.egg-info/PKG-INFO
--rw-r--r--   0 chris      (502) staff       (20)      828 2023-04-05 02:39:31.000000 ponty-0.3.7/ponty.egg-info/SOURCES.txt
--rw-r--r--   0 chris      (502) staff       (20)        1 2023-04-05 02:39:31.000000 ponty-0.3.7/ponty.egg-info/dependency_links.txt
--rw-r--r--   0 chris      (502) staff       (20)       58 2023-04-05 02:39:31.000000 ponty-0.3.7/ponty.egg-info/requires.txt
--rw-r--r--   0 chris      (502) staff       (20)        6 2023-04-05 02:39:31.000000 ponty-0.3.7/ponty.egg-info/top_level.txt
--rw-r--r--   0 chris      (502) staff       (20)       85 2022-06-13 17:52:03.000000 ponty-0.3.7/pyproject.toml
--rw-r--r--   0 chris      (502) staff       (20)       38 2023-04-05 02:39:31.171121 ponty-0.3.7/setup.cfg
--rw-r--r--   0 chris      (502) staff       (20)     1448 2023-04-05 02:23:17.000000 ponty-0.3.7/setup.py
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-23 20:18:26.200769 ponty-0.3.8/
+-rw-r--r--   0 chris      (502) staff       (20)     1015 2023-04-23 20:18:26.200580 ponty-0.3.8/PKG-INFO
+-rw-r--r--   0 chris      (502) staff       (20)     1940 2023-04-03 01:28:51.000000 ponty-0.3.8/README.rst
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-23 20:18:26.150153 ponty-0.3.8/ponty/
+-rw-r--r--   0 chris      (502) staff       (20)     1286 2023-04-01 19:00:59.000000 ponty-0.3.8/ponty/__init__.py
+-rw-r--r--   0 chris      (502) staff       (20)     3650 2023-04-23 20:09:43.000000 ponty-0.3.8/ponty/errors.py
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-23 20:18:26.162412 ponty-0.3.8/ponty/http/
+-rw-r--r--   0 chris      (502) staff       (20)     1177 2023-04-01 18:50:48.000000 ponty-0.3.8/ponty/http/__init__.py
+-rw-r--r--   0 chris      (502) staff       (20)     2881 2023-04-23 20:09:43.000000 ponty-0.3.8/ponty/http/client.py
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-23 20:18:26.164901 ponty-0.3.8/ponty/http/expect/
+-rw-r--r--   0 chris      (502) staff       (20)     1720 2023-04-23 20:09:43.000000 ponty-0.3.8/ponty/http/expect/__init__.py
+-rw-r--r--   0 chris      (502) staff       (20)     7992 2023-04-23 20:09:43.000000 ponty-0.3.8/ponty/http/expect/body.py
+-rw-r--r--   0 chris      (502) staff       (20)     1097 2023-03-25 04:25:33.000000 ponty-0.3.8/ponty/http/expect/header.py
+-rw-r--r--   0 chris      (502) staff       (20)    10171 2023-04-23 20:09:43.000000 ponty-0.3.8/ponty/http/expect/query.py
+-rw-r--r--   0 chris      (502) staff       (20)     3706 2023-04-23 20:09:43.000000 ponty-0.3.8/ponty/http/expect/req.py
+-rw-r--r--   0 chris      (502) staff       (20)     2604 2023-04-23 20:09:43.000000 ponty-0.3.8/ponty/http/expect/route.py
+-rw-r--r--   0 chris      (502) staff       (20)     1129 2022-12-29 15:32:54.000000 ponty-0.3.8/ponty/http/go.py
+-rw-r--r--   0 chris      (502) staff       (20)     1379 2023-02-22 03:26:42.000000 ponty-0.3.8/ponty/http/render.py
+-rw-r--r--   0 chris      (502) staff       (20)       53 2023-04-02 02:02:29.000000 ponty-0.3.8/ponty/http/response.py
+-rw-r--r--   0 chris      (502) staff       (20)     1797 2022-08-16 03:05:39.000000 ponty-0.3.8/ponty/http/routes.py
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-23 20:18:26.177387 ponty-0.3.8/ponty/http/schema/
+-rw-r--r--   0 chris      (502) staff       (20)      750 2022-08-14 21:35:59.000000 ponty-0.3.8/ponty/http/schema/__init__.py
+-rw-r--r--   0 chris      (502) staff       (20)     9096 2023-04-23 20:09:43.000000 ponty-0.3.8/ponty/http/schema/build.py
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-23 20:18:26.177744 ponty-0.3.8/ponty/memo/
+-rw-r--r--   0 chris      (502) staff       (20)      384 2022-06-15 03:02:09.000000 ponty-0.3.8/ponty/memo/__init__.py
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-23 20:18:26.196641 ponty-0.3.8/ponty/memo/cache/
+-rw-r--r--   0 chris      (502) staff       (20)        0 2022-06-14 14:23:14.000000 ponty-0.3.8/ponty/memo/cache/__init__.py
+-rw-r--r--   0 chris      (502) staff       (20)     4724 2023-04-23 20:09:43.000000 ponty-0.3.8/ponty/memo/cache/base.py
+-rw-r--r--   0 chris      (502) staff       (20)     5531 2023-04-23 20:09:43.000000 ponty-0.3.8/ponty/memo/cache/local.py
+-rw-r--r--   0 chris      (502) staff       (20)      105 2022-08-04 15:34:08.000000 ponty-0.3.8/ponty/memo/cache/stats.py
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-23 20:18:26.200280 ponty-0.3.8/ponty/memo/lock/
+-rw-r--r--   0 chris      (502) staff       (20)        0 2022-06-14 14:23:02.000000 ponty-0.3.8/ponty/memo/lock/__init__.py
+-rw-r--r--   0 chris      (502) staff       (20)     3178 2022-08-26 11:55:35.000000 ponty-0.3.8/ponty/memo/lock/base.py
+-rw-r--r--   0 chris      (502) staff       (20)     3018 2023-04-23 20:09:43.000000 ponty-0.3.8/ponty/memo/lock/local.py
+-rw-r--r--   0 chris      (502) staff       (20)        0 2022-07-10 14:41:50.000000 ponty-0.3.8/ponty/py.typed
+-rw-r--r--   0 chris      (502) staff       (20)      480 2023-04-23 20:09:43.000000 ponty-0.3.8/ponty/registry.py
+-rw-r--r--   0 chris      (502) staff       (20)      269 2023-04-11 04:00:44.000000 ponty-0.3.8/ponty/types_.py
+-rw-r--r--   0 chris      (502) staff       (20)     3701 2022-08-23 13:26:59.000000 ponty-0.3.8/ponty/utils.py
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-23 20:18:26.155509 ponty-0.3.8/ponty.egg-info/
+-rw-r--r--   0 chris      (502) staff       (20)     1015 2023-04-23 20:18:26.000000 ponty-0.3.8/ponty.egg-info/PKG-INFO
+-rw-r--r--   0 chris      (502) staff       (20)      828 2023-04-23 20:18:26.000000 ponty-0.3.8/ponty.egg-info/SOURCES.txt
+-rw-r--r--   0 chris      (502) staff       (20)        1 2023-04-23 20:18:26.000000 ponty-0.3.8/ponty.egg-info/dependency_links.txt
+-rw-r--r--   0 chris      (502) staff       (20)       58 2023-04-23 20:18:26.000000 ponty-0.3.8/ponty.egg-info/requires.txt
+-rw-r--r--   0 chris      (502) staff       (20)        6 2023-04-23 20:18:26.000000 ponty-0.3.8/ponty.egg-info/top_level.txt
+-rw-r--r--   0 chris      (502) staff       (20)       85 2022-06-13 17:52:03.000000 ponty-0.3.8/pyproject.toml
+-rw-r--r--   0 chris      (502) staff       (20)       38 2023-04-23 20:18:26.200822 ponty-0.3.8/setup.cfg
+-rw-r--r--   0 chris      (502) staff       (20)     1448 2023-04-23 20:15:27.000000 ponty-0.3.8/setup.py
```

### Comparing `ponty-0.3.7/PKG-INFO` & `ponty-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ponty
-Version: 0.3.7
+Version: 0.3.8
 Summary: Minimal async web framework, built on aiohttp.
 Home-page: https://github.com/csira/ponty
 License: BSD
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: AsyncIO
 Classifier: Framework :: aiohttp
```

### Comparing `ponty-0.3.7/README.rst` & `ponty-0.3.8/README.rst`

 * *Files identical despite different names*

### Comparing `ponty-0.3.7/ponty/__init__.py` & `ponty-0.3.8/ponty/__init__.py`

 * *Files identical despite different names*

### Comparing `ponty-0.3.7/ponty/errors.py` & `ponty-0.3.8/ponty/errors.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     """
     status_code: int = 500  #: HTTP status code for the response. See the official IANA registry `here <https://www.iana.org/assignments/http-status-codes/http-status-codes.xhtml>`__
 
     def __init__(
         self,
         *,
-        text: str = None,
+        text: typing.Union[str, None] = None,
         body: typing.Any = None,
         **kw
     ):
         if text is not None and body is not None:
             raise ValueError
 
         super().__init__()
@@ -47,39 +47,41 @@
     """Returns a 400. Inherits :class:`PontyError`."""
 
     status_code = 400
 
 
 
 
-P = ParamSpec("P")
-R = TypeVar("R")
+_P = ParamSpec("_P")
+_R = TypeVar("_R")
 
 
-def error_trap(f: Callable[P, Awaitable[R]]) -> Callable[P, Awaitable[R]]:
+def error_trap(f: Callable[_P, Awaitable[_R]]) -> Callable[_P, Awaitable[_R]]:
     @functools.wraps(f)
-    async def wrapper(*a: P.args, **kw: P.kwargs) -> R:
+    async def wrapper(*a: _P.args, **kw: _P.kwargs) -> _R:
         try:
             return await f(*a, **kw)
         except PontyError as e:
             raise_status(
                 e.status_code,
                 text=e.text,
                 body=e.body,
                 **e.kw
             )
     return wrapper
 
 
+
+
 def raise_status(
     status: int,
     *,
-    text: str = None,
+    text: typing.Union[str, None] = None,
     body: typing.Any = None,
-    content_type: str = None,
+    content_type: typing.Union[str, None] = None,
     **kw
 ) -> typing.NoReturn:
     """
     Raise an `aiohttp.web.HTTPException <https://docs.aiohttp.org/en/stable/web_reference.html#aiohttp.web.HTTPException>`_
     for the given status code.
 
     :param status: HTTP status code
```

### Comparing `ponty-0.3.7/ponty/http/__init__.py` & `ponty-0.3.8/ponty/http/__init__.py`

 * *Files identical despite different names*

### Comparing `ponty-0.3.7/ponty/http/client.py` & `ponty-0.3.8/ponty/http/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 
 
 def http_client_provider(
     *,
     name: str = _defaultname,
     timeout: int = 5,
     concurrency: int = 100,
-    headers: dict[str, typing.Any] = None,
-    cookies: dict[str, typing.Any] = None,
+    headers: typing.Union[ dict[str, typing.Any], None ] = None,
+    cookies: typing.Union[ dict[str, typing.Any], None ] = None,
     **kw
 ) -> Provider:
     """Builds an HTTP Client Session provider.
 
     Wraps `aiohttp.ClientSession <https://docs.aiohttp.org/en/stable/client_reference.html#aiohttp.ClientSession>`_.
 
     :param name: unique name, used by :func:`lease_http_client`
```

### Comparing `ponty-0.3.7/ponty/http/expect/__init__.py` & `ponty-0.3.8/ponty/http/expect/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 
 class AIOHttpReq:
     """Forwards along the
     `aiohttp.web.Request <https://docs.aiohttp.org/en/latest/web_reference.html#aiohttp.web.Request>`__.
 
     """
-    def __get__(self, obj: Request, objtype: type[Request] = None) -> aiohttp.web.Request:
+    def __get__(self, obj: Request, objtype: type[Request]) -> aiohttp.web.Request:
         return obj.req
 
 
 class Cookie:
     """Extracts request cookie `name`.
 
     :param str name: cookie name
@@ -61,14 +61,14 @@
         errorcode: int = 400,
     ):
         self._name = name
         self._required = required
         self._default = default
         self._errorcode = errorcode
 
-    def __get__(self, obj: Request, objtype: type[Request] = None) -> str:
+    def __get__(self, obj: Request, objtype: type[Request]) -> str:
         try:
             return obj.req.cookies[self._name]
         except KeyError:
             if self._required:
                 raise_status(self._errorcode)
             return self._default
```

### Comparing `ponty-0.3.7/ponty/http/expect/body.py` & `ponty-0.3.8/ponty/http/expect/body.py`

 * *Files 10% similar despite different names*

```diff
@@ -88,19 +88,26 @@
         ...
         < HTTP/1.1 400 Bad Request
         < Content-Type: text/plain; charset=utf-8
         ...
         'last_name' is a required property
 
     """
+
+    @typing.overload
+    def __init__(self, *, filepath: str, schema: None = None): ...
+
+    @typing.overload
+    def __init__(self, *, filepath: None = None, schema: dict[str, typing.Any]): ...
+
     def __init__(
         self,
         *,
-        filepath: str = None,
-        schema: dict[str, typing.Any] = None,
+        filepath: typing.Union[str, None] = None,
+        schema: typing.Union[ dict[str, typing.Any], None ] = None,
     ):
         super().__init__()
 
         if not logical_xor(filepath, schema):
             raise RuntimeError("only one of filepath, schema may be specified")
 
         if filepath:
@@ -274,15 +281,15 @@
             -v
         ...
         < HTTP/1.1 400 Bad Request
         ...
         'abc' is not of type 'integer'
 
     """
-    def __init__(self, cls: type[D], *, filepath: str = None):
+    def __init__(self, cls: type[D], *, filepath: typing.Union[str, None] = None):
         self._cls = cls
 
         if filepath:
             super().__init__(filepath=filepath)
         else:
             super().__init__(schema=dataclass_to_jsonschema(cls))
```

### Comparing `ponty-0.3.7/ponty/http/expect/header.py` & `ponty-0.3.8/ponty/http/expect/header.py`

 * *Files identical despite different names*

### Comparing `ponty-0.3.7/ponty/http/expect/query.py` & `ponty-0.3.8/ponty/http/expect/query.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     :param bool required:
       if True, the query parameter will be treated as a mandatory
       component of the request;
       an HTTP 400 will be raised in the event no value is supplied.
       Default `False`
 
     :param _T default:
-      default value, returned if the query param is not provided.
+      default value, returned if the query param has not been provided.
       Set `required=True` instead if this should be treated as an error condition.
       One of `required` or `default` must be provided
 
     :param cast_func:
       function to convert the string value provided to type `T`.
       If the function raises a `ValueError` when it fails,
       the error will be trapped and reraised as an HTTP 400
@@ -40,14 +40,15 @@
     :param Iterable[str] values:
       if supplied, validates the captured query parameter against these
       legal values.
       Throws a 400 in the event of a mismatch
 
     It's easiest to use :class:`StringQueryParameter` or
     :class:`PosIntQueryParameter` for simple cases in practice.
+
     Use the :class:`QueryParameter` base class to create new custom parsers,
     in the same way as :class:`RouteParameter`:
 
 
     .. code-block:: python
         :emphasize-lines: 22,34,40
 
@@ -180,15 +181,15 @@
 
         self._key = key
         self._required = required
         self._default = default
         self._cast_func = cast_func
         self._values = values
 
-    def __set_name__(self, obj: Request, name: str) -> None:
+    def __set_name__(self, obj: type[Request], name: str) -> None:
         if not self._key:
             self._key = name
 
     def __get__(self, obj: Request, objtype: type[Request]) -> _T:
         if obj is None:
             raise TypeError
 
@@ -205,19 +206,17 @@
             vals = (str(v) for v in self._values)
             msg = f"{self._key} must be one of {{{','.join(vals)}}}"
             raise ValidationError(text=msg)
 
         try:
             return self._cast_func(val)
         except ValueError:
-            msg = f"{val} could not be cast"
+            msg = f"'{val}' could not be cast"
             raise ValidationError(text=msg)
 
-        return val
-
 
 class StringQueryParameter(QueryParameter[str]):
     """
     Inherits :class:`QueryParameter`.
     Treats the captured query param as a string.
 
     .. code-block:: python
@@ -330,14 +329,69 @@
 
 
 class PosIntQueryParameter(QueryParameter[int]):
     """
     Inherits :class:`QueryParameter`.
     Casts the captured query param to an integer, and validates it is non-negative.
 
+    .. code-block:: python
+        :emphasize-lines: 12
+
+        from ponty import (
+            expect,
+            get,
+            render_json,
+            Request,
+            PosIntQueryParameter,
+        )
+
+
+        class HelloReq(Request):
+
+            num_exclamations = PosIntQueryParameter(key="bangs", default=1)
+
+
+        @get("/hello")
+        @expect(HelloReq)
+        @render_json
+        async def greet(num_exclamations: int):
+            return {"greeting": f"hello world{'!' * num_exclamations}"}
+
+
+    .. code-block:: bash
+        :emphasize-lines: 4
+
+        $ curl localhost:8080/hello?bangs=7 | python -m json.tool
+        {
+            "data": {
+                "greeting": "hello world!!!!!!!"
+            },
+            "elapsed": 0
+            "now": 1681345852404,
+        }
+
+
+    .. code-block:: bash
+        :caption: not an int
+        :emphasize-lines: 2,7,13
+
+        $ curl localhost:8080/hello?bangs=abc
+        > GET /hello?bangs=abc HTTP/1.1
+        > Host: localhost:8008
+        > User-Agent: curl/7.79.1
+        > Accept: */*
+        >
+        < HTTP/1.1 400 Bad Request
+        < Content-Type: text/plain; charset=utf-8
+        < Content-Length: 21
+        < Date: Thu, 13 Apr 2023 00:31:40 GMT
+        < Server: Python/3.9 aiohttp/3.7.3
+        <
+        'abc' could not be cast
+
     """
     def __init__(self, **kw):
         super().__init__(cast_func=int, **kw)
 
     def __get__(self, obj: Request, objtype: type[Request]) -> int:
         val = super().__get__(obj, objtype)
         if val < 0:
```

### Comparing `ponty-0.3.7/ponty/http/expect/req.py` & `ponty-0.3.8/ponty/http/expect/req.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import functools
 import inspect
 import typing
+from typing import Awaitable, Callable, TypeVar
+from typing_extensions import ParamSpec
 import warnings
 
 import aiohttp.web
 
 from ponty.errors import raise_status
 
 
@@ -20,15 +22,15 @@
 
     def __get__(self, obj: "Request", objtype: type["Request"]):
         return obj._text
 
 
 
 
-_T = typing.TypeVar("_T", covariant=True)
+_T = TypeVar("_T", covariant=True)
 
 
 @typing.runtime_checkable
 class _Descriptor(typing.Protocol[_T]):
     def __get__(self, obj, objtype=None) -> _T: ...
 
 
@@ -67,15 +69,15 @@
     _fieldnames: tuple[str, ...] = ()
     _extract_json: bool = False
     _extract_text: bool = False
 
     def __init__(self, req: aiohttp.web.Request):
         self.req = req
         self._json = None
-        self._text: typing.Optional[str] = None
+        self._text: typing.Union[str, None] = None
 
     @property
     def _fields(self) -> dict[str, typing.Any]:
         return {name: getattr(self, name) for name in self._fieldnames}
 
     async def _prepare(self) -> None:
         if self._extract_json:
@@ -83,41 +85,48 @@
 
         if self._extract_text:
             self._text = await self.req.text()
 
 
 
 
-def expect(cls: type[Request], *, mimetype: str = None):
+_P = ParamSpec("_P")
+_R = TypeVar("_R")
+
+
+def expect(cls: type[Request], *, mimetype: typing.Union[str, None] = None):
     """
     Preprocess the HTTP request, according to the rules configured in the
     :class:`Request` subclass.
 
     :param type[Request] cls: subclass of :class:`Request`,
       with rules for processing the HTTP request attached as descriptors
 
     :param str mimetype: expected IANA media type.
       If provided and the specified type does not match the media type
       found in the content-type header, throws a 415
 
     """
-    def wraps(f):
+    def wraps(
+        f: Callable[_P, Awaitable[_R]]
+    ) -> Callable[[aiohttp.web.Request], Awaitable[_R]]:
+
         sig = inspect.signature(f)
         argnames = sig.parameters.keys()
 
         symdiff = set(cls._fieldnames) ^ set(argnames)
         if symdiff:
             raise TypeError(f"Parameter mismatch in '{f.__name__}': {', '.join(symdiff)}")
 
         if cls._extract_json:
             if mimetype is not None and mimetype != "application/json":
-                warnings.warn(f"handler '{f.__name__}' expects a json payload but mimetype '{mimetype}' is expected")
+                warnings.warn(f"handler '{f.__name__}' expects a json payload but mimetype '{mimetype}' has been specified")
 
         @functools.wraps(f)
-        async def wrapper(req: aiohttp.web.Request):
+        async def wrapper(req: aiohttp.web.Request) -> _R:
             if mimetype:
                 if mimetype not in req.headers["content-type"]:
                     raise_status(415)
 
             inst = cls(req)
             await inst._prepare()
             return await f(**inst._fields)
```

### Comparing `ponty-0.3.7/ponty/http/expect/route.py` & `ponty-0.3.8/ponty/http/expect/route.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,15 +52,15 @@
             ...
 
     """
     def __init__(
         self,
         *,
         pattern: str,
-        cast_func: typing.Callable[[str], _T] = None,
+        cast_func: typing.Union[ typing.Callable[[str], _T], None ] = None,
     ):
         self._pattern = pattern
         self._cast_func = cast_func
 
     def __set_name__(self, owner: type[Request], name: str):
         self._key = name
 
@@ -68,16 +68,16 @@
     def __get__(self, obj: None, objtype: type[Request]) -> str: ...
 
     @typing.overload
     def __get__(self, obj: Request, objtype: type[Request]) -> _T: ...
 
     def __get__(
         self,
-        obj: typing.Optional[Request],
-        objtype: type[Request] = None,
+        obj: typing.Union[Request, None],
+        objtype: type[Request],
     ) -> typing.Union[_T, str]:
 
         if obj is None:
             return f"{{{self._key}:{self._pattern}}}"
 
         val = obj.req.match_info[self._key]
         if self._cast_func:
```

### Comparing `ponty-0.3.7/ponty/http/go.py` & `ponty-0.3.8/ponty/http/go.py`

 * *Files identical despite different names*

### Comparing `ponty-0.3.7/ponty/http/render.py` & `ponty-0.3.8/ponty/http/render.py`

 * *Files identical despite different names*

### Comparing `ponty-0.3.7/ponty/http/routes.py` & `ponty-0.3.8/ponty/http/routes.py`

 * *Files identical despite different names*

### Comparing `ponty-0.3.7/ponty/http/schema/__init__.py` & `ponty-0.3.8/ponty/http/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `ponty-0.3.7/ponty/http/schema/build.py` & `ponty-0.3.8/ponty/http/schema/build.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,15 +231,15 @@
             anno = {}
 
         return _lookup(args[0], primary, defs, **anno)
 
     if unscripted_type is typing.Literal:
         return {"enum": list(args), **kw}
 
-    is_uniontype: bool = unscripted_type is typing.Union
+    is_uniontype = unscripted_type is typing.Union
     if sys.version_info >= (3, 10):
         is_uniontype = is_uniontype or (unscripted_type is types.UnionType)
     if is_uniontype:  # also catches Optional
         return {
             "anyOf": [_lookup(arg, primary, defs) for arg in args],
             **kw
         }
```

### Comparing `ponty-0.3.7/ponty/memo/cache/base.py` & `ponty-0.3.8/ponty/memo/cache/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,46 +24,46 @@
     Returned by subclasses of :class:`CacheStore`.
 
     """
 
 
 
 
-T = typing.TypeVar("T")
+_T = typing.TypeVar("_T")
 
 
-class CacheStore(abc.ABC, typing.Generic[T]):
+class CacheStore(abc.ABC, typing.Generic[_T]):
     """Abstract Base Class. Container for cached items.
 
     :func:`cache` expects two abstract methods,
     :meth:`get <ponty.memo.CacheStore.get>` and
     :meth:`set <ponty.memo.CacheStore.set>`, and
     :func:`invalidate` expects one,
     :meth:`remove <ponty.memo.CacheStore.remove>`.
     All three must return awaitables.
 
     Generic on one variable, the type T of the cached item.
 
     """
 
     @abc.abstractmethod
-    async def get(self, key: str) -> typing.Union[T, type[cachemiss]]:
+    async def get(self, key: str) -> typing.Union[_T, type[cachemiss]]:
         """Fetch the cached value.
 
         Errors are not captured.
 
         :param key: unique id for the cached item
         :returns: the cached item,
           or the :class:`cachemiss` sentinel if it does not exist
         :rtype: Union[T, type[:class:`cachemiss`]]
 
         """
 
     @abc.abstractmethod
-    async def set(self, key: str, data: T) -> None:
+    async def set(self, key: str, data: _T) -> None:
         """Add an item to the cache.
 
         :param key: unique id for the item
         :param data: the item to be cached
 
         """
```

### Comparing `ponty-0.3.7/ponty/memo/cache/local.py` & `ponty-0.3.8/ponty/memo/cache/local.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,36 +3,36 @@
 import warnings
 
 from ponty.memo.cache.base import CacheStore, cache, cachemiss, Stampede
 from ponty.memo.lock.local import locallock
 from ponty.utils import now_millis
 
 
-T = typing.TypeVar("T")
+_T = typing.TypeVar("_T")
 
 
-class _LRUStore(CacheStore[T]):
+class _LRUStore(CacheStore[_T]):
 
     def __init__(self, ttl_ms: int, maxsize: int):
         super().__init__()
 
         if ttl_ms < 0:
             raise ValueError("negative ttl is nonsense")
         self._ttl_ms: typing.Final[int] = ttl_ms
 
         if maxsize < 0:
             raise ValueError("negative maxsize is nonsense")
         if maxsize == 0:
             warnings.warn("Cache without maxsize may grow endlessly, beware.")
         self._maxsize: typing.Final[int] = maxsize
 
-        self._cache: dict[str, tuple[typing.Union[int, None], T]] = dict()
+        self._cache: dict[str, tuple[typing.Union[int, None], _T]] = dict()
         self._lru: deque[str] = deque()
 
-    async def get(self, key: str) -> typing.Union[T, type[cachemiss]]:
+    async def get(self, key: str) -> typing.Union[_T, type[cachemiss]]:
         try:
             expiry, data = self._cache[key]
         except KeyError:
             return cachemiss
 
         if expiry is not None and expiry < now_millis():
             await self.remove(key)
@@ -40,15 +40,15 @@
 
         # rotate key to the end of the LRU queue
         self._lru.remove(key)
         self._lru.append(key)
 
         return data
 
-    async def set(self, key: str, data: T) -> None:
+    async def set(self, key: str, data: _T) -> None:
         if self._ttl_ms == 0:
             expiry = None
         else:
             expiry = now_millis() + self._ttl_ms
 
         self._cache[key] = (expiry, data)
         self._lru.append(key)
```

### Comparing `ponty-0.3.7/ponty/memo/lock/base.py` & `ponty-0.3.8/ponty/memo/lock/base.py`

 * *Files identical despite different names*

### Comparing `ponty-0.3.7/ponty/memo/lock/local.py` & `ponty-0.3.8/ponty/memo/lock/local.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from ponty.memo.lock.base import SentinelStore, Lock
 
 
 class _Sentinels(SentinelStore):
 
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__()
         self._sentinels: set[str] = set()
 
     async def exists(self, key: str) -> bool:
         return key in self._sentinels
 
     async def add(self, key: str) -> None:
```

### Comparing `ponty-0.3.7/ponty/utils.py` & `ponty-0.3.8/ponty/utils.py`

 * *Files identical despite different names*

### Comparing `ponty-0.3.7/ponty.egg-info/PKG-INFO` & `ponty-0.3.8/ponty.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ponty
-Version: 0.3.7
+Version: 0.3.8
 Summary: Minimal async web framework, built on aiohttp.
 Home-page: https://github.com/csira/ponty
 License: BSD
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: AsyncIO
 Classifier: Framework :: aiohttp
```

### Comparing `ponty-0.3.7/ponty.egg-info/SOURCES.txt` & `ponty-0.3.8/ponty.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ponty-0.3.7/setup.py` & `ponty-0.3.8/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 if __name__ == "__main__":
     setup(
         packages=find_packages(),
         package_data={"ponty": ["py.typed"]},
         name="ponty",
-        version="0.3.7",
+        version="0.3.8",
         license="BSD",
         url="https://github.com/csira/ponty",
         description="Minimal async web framework, built on aiohttp.",
         install_requires=[
             "aiohttp>=3.7.3",
             "jsonschema==3.2.0",
             "typing-extensions>=4.2.0",
```

