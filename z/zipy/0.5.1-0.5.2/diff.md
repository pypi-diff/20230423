# Comparing `tmp/zipy-0.5.1.tar.gz` & `tmp/zipy-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zipy-0.5.1.tar", max compression
+gzip compressed data, was "zipy-0.5.2.tar", max compression
```

## Comparing `zipy-0.5.1.tar` & `zipy-0.5.2.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0      221 2023-03-01 05:49:23.475612 zipy-0.5.1/README.md
--rw-r--r--   0        0        0      689 2023-03-14 02:45:32.841056 zipy-0.5.1/pyproject.toml
--rw-r--r--   0        0        0        0 2022-12-02 06:04:03.457276 zipy-0.5.1/zipy/__init__.py
--rw-r--r--   0        0        0     2847 2022-12-12 04:52:25.251775 zipy-0.5.1/zipy/cache.py
--rw-r--r--   0        0        0        0 2023-03-01 08:48:41.314138 zipy-0.5.1/zipy/cmdline/__init__.py
--rw-r--r--   0        0        0      498 2023-03-13 14:26:17.339747 zipy-0.5.1/zipy/cmdline/string.py
--rw-r--r--   0        0        0      545 2023-03-13 14:26:17.339675 zipy-0.5.1/zipy/cmdline/web3.py
--rw-r--r--   0        0        0      577 2023-03-14 02:42:29.138225 zipy-0.5.1/zipy/data.py
--rw-r--r--   0        0        0      162 2022-12-06 03:16:01.905306 zipy-0.5.1/zipy/inspect.py
--rw-r--r--   0        0        0     2482 2022-12-21 04:45:29.904965 zipy-0.5.1/zipy/retry.py
--rw-r--r--   0        0        0     2153 2022-12-09 07:04:47.730978 zipy-0.5.1/zipy/time.py
--rw-r--r--   0        0        0     9769 2023-03-13 14:26:17.295318 zipy-0.5.1/zipy/web3.py
--rw-r--r--   0        0        0      955 1970-01-01 00:00:00.000000 zipy-0.5.1/setup.py
--rw-r--r--   0        0        0      793 1970-01-01 00:00:00.000000 zipy-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0      221 2023-03-01 05:49:23.475612 zipy-0.5.2/README.md
+-rw-r--r--   0        0        0      689 2023-04-23 11:16:23.087279 zipy-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-12-02 06:04:03.457276 zipy-0.5.2/zipy/__init__.py
+-rw-r--r--   0        0        0     2847 2022-12-12 04:52:25.251775 zipy-0.5.2/zipy/cache.py
+-rw-r--r--   0        0        0        0 2023-03-01 08:48:41.314138 zipy-0.5.2/zipy/cmdline/__init__.py
+-rw-r--r--   0        0        0      498 2023-03-13 14:26:17.339747 zipy-0.5.2/zipy/cmdline/string.py
+-rw-r--r--   0        0        0      545 2023-03-13 14:26:17.339675 zipy-0.5.2/zipy/cmdline/web3.py
+-rw-r--r--   0        0        0      577 2023-03-14 02:42:29.138225 zipy-0.5.2/zipy/data.py
+-rw-r--r--   0        0        0      162 2022-12-06 03:16:01.905306 zipy-0.5.2/zipy/inspect.py
+-rw-r--r--   0        0        0     2563 2023-04-23 11:13:41.578203 zipy-0.5.2/zipy/retry.py
+-rw-r--r--   0        0        0     2153 2022-12-09 07:04:47.730978 zipy-0.5.2/zipy/time.py
+-rw-r--r--   0        0        0     9769 2023-03-13 14:26:17.295318 zipy-0.5.2/zipy/web3.py
+-rw-r--r--   0        0        0      793 1970-01-01 00:00:00.000000 zipy-0.5.2/PKG-INFO
```

### Comparing `zipy-0.5.1/pyproject.toml` & `zipy-0.5.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zipy"
-version = "0.5.1"
+version = "0.5.2"
 description = "Zipy is a toolbox containing a set of convenient python function"
 authors = ["冒险岛真好玩 <17826800084g@gmail.com>"]
 readme = "README.md"
 packages = [{include = "zipy"}]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4"
```

### Comparing `zipy-0.5.1/zipy/cache.py` & `zipy-0.5.2/zipy/cache.py`

 * *Files identical despite different names*

### Comparing `zipy-0.5.1/zipy/cmdline/web3.py` & `zipy-0.5.2/zipy/cmdline/web3.py`

 * *Files identical despite different names*

### Comparing `zipy-0.5.1/zipy/data.py` & `zipy-0.5.2/zipy/data.py`

 * *Files identical despite different names*

### Comparing `zipy-0.5.1/zipy/retry.py` & `zipy-0.5.2/zipy/retry.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import asyncio
 import time
 import itertools
 from typing import Iterable
+from functools import update_wrapper
 from zipy import inspect
 
 
 __all__ = ["retry"]
 
 
 def retry(*, times: int = 1, wait: float = 0, exceptions: Iterable = [Exception]):
@@ -39,15 +40,15 @@
                         if any(
                             map(lambda c: isinstance(exc, c), exceptions)  # noqa: F821
                         ):
                             await asyncio.sleep(wait)
                         else:
                             raise exc
 
-            return wrapper
+            return update_wrapper(wrapper, func)
         elif inspect.isnormalfunc(func):
 
             def wrapper(*args, **kwargs):
                 for ntry in range(times) if times > 0 else itertools.count(0):
                     try:
                         return func(*args, **kwargs)
                     except Exception as exc:
@@ -56,12 +57,12 @@
                         if any(
                             map(lambda c: isinstance(exc, c), exceptions)  # noqa: F821
                         ):
                             time.sleep(wait)
                         else:
                             raise exc
 
-            return wrapper
+            return update_wrapper(wrapper, func)
         else:
             raise ValueError(f"{func} is neither coroutine nor normal function")
 
     return decorator
```

### Comparing `zipy-0.5.1/zipy/time.py` & `zipy-0.5.2/zipy/time.py`

 * *Files identical despite different names*

### Comparing `zipy-0.5.1/zipy/web3.py` & `zipy-0.5.2/zipy/web3.py`

 * *Files identical despite different names*

### Comparing `zipy-0.5.1/PKG-INFO` & `zipy-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zipy
-Version: 0.5.1
+Version: 0.5.2
 Summary: Zipy is a toolbox containing a set of convenient python function
 Author: 冒险岛真好玩
 Author-email: 17826800084g@gmail.com
 Requires-Python: >=3.9,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

