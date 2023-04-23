# Comparing `tmp/funcs-0.4.0.tar.gz` & `tmp/funcs-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcs-0.4.0.tar", max compression
+gzip compressed data, was "funcs-0.5.0.tar", max compression
```

## Comparing `funcs-0.4.0.tar` & `funcs-0.5.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1092 2023-04-21 07:57:44.740132 funcs-0.4.0/LICENSE
--rw-r--r--   0        0        0     2872 2023-04-21 07:57:44.740132 funcs-0.4.0/README.md
--rw-r--r--   0        0        0     1690 2023-04-21 07:57:44.740132 funcs-0.4.0/funcs/__init__.py
--rw-r--r--   0        0        0      883 2023-04-21 07:57:44.740132 funcs-0.4.0/funcs/application.py
--rw-r--r--   0        0        0      856 2023-04-21 07:57:44.740132 funcs-0.4.0/funcs/callers.py
--rw-r--r--   0        0        0     5467 2023-04-21 07:57:44.740132 funcs-0.4.0/funcs/composition.py
--rw-r--r--   0        0        0      830 2023-04-21 07:57:44.740132 funcs-0.4.0/funcs/debug.py
--rw-r--r--   0        0        0      166 2023-04-21 07:57:44.740132 funcs-0.4.0/funcs/decorators.py
--rw-r--r--   0        0        0     6337 2023-04-21 07:57:44.740132 funcs-0.4.0/funcs/flow.py
--rw-r--r--   0        0        0     2259 2023-04-21 07:57:44.740132 funcs-0.4.0/funcs/functions.py
--rw-r--r--   0        0        0      418 2023-04-21 07:57:44.740132 funcs-0.4.0/funcs/getters.py
--rw-r--r--   0        0        0      782 2023-04-21 07:57:44.740132 funcs-0.4.0/funcs/primitives.py
--rw-r--r--   0        0        0        0 2023-04-21 07:57:44.740132 funcs-0.4.0/funcs/py.typed
--rw-r--r--   0        0        0     1111 2023-04-21 07:57:44.740132 funcs-0.4.0/funcs/reduction.py
--rw-r--r--   0        0        0     1031 2023-04-21 07:57:44.740132 funcs-0.4.0/funcs/types.py
--rw-r--r--   0        0        0     6579 2023-04-21 07:57:44.740132 funcs-0.4.0/funcs/typing.py
--rw-r--r--   0        0        0     2344 2023-04-21 07:57:44.740132 funcs-0.4.0/funcs/unpacking.py
--rw-r--r--   0        0        0     3022 2023-04-21 07:57:44.740132 funcs-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     4062 1970-01-01 00:00:00.000000 funcs-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-04-23 13:41:20.086921 funcs-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2872 2023-04-23 13:41:20.086921 funcs-0.5.0/README.md
+-rw-r--r--   0        0        0     1690 2023-04-23 13:41:20.086921 funcs-0.5.0/funcs/__init__.py
+-rw-r--r--   0        0        0      883 2023-04-23 13:41:20.086921 funcs-0.5.0/funcs/application.py
+-rw-r--r--   0        0        0      856 2023-04-23 13:41:20.086921 funcs-0.5.0/funcs/callers.py
+-rw-r--r--   0        0        0     5467 2023-04-23 13:41:20.086921 funcs-0.5.0/funcs/composition.py
+-rw-r--r--   0        0        0      830 2023-04-23 13:41:20.086921 funcs-0.5.0/funcs/debug.py
+-rw-r--r--   0        0        0      166 2023-04-23 13:41:20.086921 funcs-0.5.0/funcs/decorators.py
+-rw-r--r--   0        0        0     6337 2023-04-23 13:41:20.086921 funcs-0.5.0/funcs/flow.py
+-rw-r--r--   0        0        0     2259 2023-04-23 13:41:20.086921 funcs-0.5.0/funcs/functions.py
+-rw-r--r--   0        0        0      418 2023-04-23 13:41:20.086921 funcs-0.5.0/funcs/getters.py
+-rw-r--r--   0        0        0      782 2023-04-23 13:41:20.086921 funcs-0.5.0/funcs/primitives.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:41:20.086921 funcs-0.5.0/funcs/py.typed
+-rw-r--r--   0        0        0     1111 2023-04-23 13:41:20.086921 funcs-0.5.0/funcs/reduction.py
+-rw-r--r--   0        0        0     1031 2023-04-23 13:41:20.086921 funcs-0.5.0/funcs/types.py
+-rw-r--r--   0        0        0     6633 2023-04-23 13:41:20.086921 funcs-0.5.0/funcs/typing.py
+-rw-r--r--   0        0        0     2344 2023-04-23 13:41:20.086921 funcs-0.5.0/funcs/unpacking.py
+-rw-r--r--   0        0        0     3022 2023-04-23 13:41:20.086921 funcs-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4062 1970-01-01 00:00:00.000000 funcs-0.5.0/PKG-INFO
```

### Comparing `funcs-0.4.0/LICENSE` & `funcs-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `funcs-0.4.0/README.md` & `funcs-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 $ poetry add funcs
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-funcs = "^0.4.0"
+funcs = "^0.5.0"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.funcs]
 git = "https://github.com/nekitdev/funcs.git"
```

### Comparing `funcs-0.4.0/funcs/__init__.py` & `funcs-0.5.0/funcs/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 __description__ = "Functional programming in Python."
 __url__ = "https://github.com/nekitdev/funcs"
 
 __title__ = "funcs"
 __author__ = "nekitdev"
 __license__ = "MIT"
-__version__ = "0.4.0"
+__version__ = "0.5.0"
 
 from funcs.application import apply, partial
 from funcs.callers import caller, method_caller
 from funcs.composition import compose, compose_once, pipe, pipe_once
 from funcs.debug import tap
 from funcs.decorators import wraps
 from funcs.flow import once, post_processing, reraise, reraise_with, suppress, wrap_with
```

### Comparing `funcs-0.4.0/funcs/application.py` & `funcs-0.5.0/funcs/application.py`

 * *Files identical despite different names*

### Comparing `funcs-0.4.0/funcs/callers.py` & `funcs-0.5.0/funcs/callers.py`

 * *Files identical despite different names*

### Comparing `funcs-0.4.0/funcs/composition.py` & `funcs-0.5.0/funcs/composition.py`

 * *Files identical despite different names*

### Comparing `funcs-0.4.0/funcs/debug.py` & `funcs-0.5.0/funcs/debug.py`

 * *Files identical despite different names*

### Comparing `funcs-0.4.0/funcs/flow.py` & `funcs-0.5.0/funcs/flow.py`

 * *Files identical despite different names*

### Comparing `funcs-0.4.0/funcs/functions.py` & `funcs-0.5.0/funcs/functions.py`

 * *Files identical despite different names*

### Comparing `funcs-0.4.0/funcs/primitives.py` & `funcs-0.5.0/funcs/primitives.py`

 * *Files identical despite different names*

### Comparing `funcs-0.4.0/funcs/reduction.py` & `funcs-0.5.0/funcs/reduction.py`

 * *Files identical despite different names*

### Comparing `funcs-0.4.0/funcs/types.py` & `funcs-0.5.0/funcs/types.py`

 * *Files identical despite different names*

### Comparing `funcs-0.4.0/funcs/typing.py` & `funcs-0.5.0/funcs/typing.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,31 +5,31 @@
 
 from typing_extensions import ParamSpec, TypeAlias, TypeGuard
 
 __all__ = (
     "Traceback",
     "AnyError",
     "AnyErrorType",
-    "Error",
-    "ErrorType",
+    "NormalError",
+    "NormalErrorType",
     "AnyContextManager",
     "SimpleContextManager",
     "EmptyTuple",
     "Tuple1",
     "Tuple2",
     "Tuple3",
     "Tuple4",
     "Tuple5",
     "Tuple6",
     "Tuple7",
     "Tuple8",
     "DynamicTuple",
     "AnyTuple",
     "AnyErrorTypes",
-    "ErrorTypes",
+    "NormalErrorTypes",
     "DynamicCallable",
     "AnyCallable",
     "Nullary",
     "Unary",
     "Binary",
     "Ternary",
     "Quaternary",
@@ -65,17 +65,17 @@
 )
 
 AnyError: TypeAlias = BaseException
 """Represents any errors."""
 AnyErrorType = Type[AnyError]
 """Represents any error types."""
 
-Error: TypeAlias = Exception
+NormalError: TypeAlias = Exception
 """Represents normal errors."""
-ErrorType = Type[Error]
+NormalErrorType = Type[NormalError]
 """Represents normal error types."""
 
 AnyContextManager = ContextManager[Any]
 """Represents any context managers."""
 SimpleContextManager = ContextManager[None]
 """Represents simple context managers that don't return anything on enter."""
 
@@ -111,16 +111,16 @@
 DynamicTuple = Tuple[T, ...]
 """Represents homogeneous tuples of any length `(T, ...)`."""
 AnyTuple = DynamicTuple[Any]
 """Represents any tuples `(Any, ...)`."""
 
 AnyErrorTypes = DynamicTuple[AnyErrorType]
 """Represents tuples of any error types `(AnyErrorType, ...)`."""
-ErrorTypes = DynamicTuple[ErrorType]
-"""Represents tuples of normal error types `(ErrorType, ...)`."""
+NormalErrorTypes = DynamicTuple[NormalErrorType]
+"""Represents tuples of normal error types `(NormalErrorType, ...)`."""
 
 DynamicCallable = Callable[..., R]
 """Represents dynamic callables `(...) -> R`."""
 AnyCallable = DynamicCallable[Any]
 """Represents any callables `(...) -> Any`."""
 
 F = TypeVar("F", bound=AnyCallable)
```

### Comparing `funcs-0.4.0/funcs/unpacking.py` & `funcs-0.5.0/funcs/unpacking.py`

 * *Files identical despite different names*

### Comparing `funcs-0.4.0/pyproject.toml` & `funcs-0.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "funcs"
-version = "0.4.0"
+version = "0.5.0"
 description = "Functional programming in Python."
 authors = ["nekitdev"]
 license = "MIT"
 
 readme = "README.md"
 
 homepage = "https://github.com/nekitdev/funcs"
@@ -126,15 +126,15 @@
 warn_unreachable = true
 
 warn_redundant_casts = true
 warn_unused_ignores = false  # compatibility
 
 [tool.changelogging]
 name = "funcs"
-version = "0.4.0"
+version = "0.5.0"
 url = "https://github.com/nekitdev/funcs"
 directory = "changes"
 output = "CHANGELOG.md"
 
 start_string = "<!-- changelogging: start -->"
 
 title_format = "{version} ({date})"
```

### Comparing `funcs-0.4.0/PKG-INFO` & `funcs-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcs
-Version: 0.4.0
+Version: 0.5.0
 Summary: Functional programming in Python.
 Home-page: https://github.com/nekitdev/funcs
 License: MIT
 Keywords: python,function,functional,paradigm
 Author: nekitdev
 Requires-Python: >=3.7
 Classifier: Development Status :: 5 - Production/Stable
@@ -70,15 +70,15 @@
 $ poetry add funcs
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-funcs = "^0.4.0"
+funcs = "^0.5.0"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.funcs]
 git = "https://github.com/nekitdev/funcs.git"
```

