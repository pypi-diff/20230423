# Comparing `tmp/async_fm-0.0.1.tar.gz` & `tmp/async_fm-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_fm-0.0.1.tar", max compression
+gzip compressed data, was "async_fm-0.0.2.tar", max compression
```

## Comparing `async_fm-0.0.1.tar` & `async_fm-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1069 2023-04-23 05:05:10.759636 async_fm-0.0.1/LICENSE
--rw-r--r--   0        0        0     1590 2023-04-23 05:05:10.759636 async_fm-0.0.1/README.md
--rw-r--r--   0        0        0      665 2023-04-23 05:05:10.759636 async_fm-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       76 2023-04-23 05:05:10.763636 async_fm-0.0.1/src/asyncfm/__init__.py
--rw-r--r--   0        0        0     1296 2023-04-23 05:05:10.763636 async_fm-0.0.1/src/asyncfm/api/__init__.py
--rw-r--r--   0        0        0    14947 2023-04-23 05:05:10.763636 async_fm-0.0.1/src/asyncfm/api/user.py
--rw-r--r--   0        0        0     2424 2023-04-23 05:05:10.763636 async_fm-0.0.1/src/asyncfm/exceptions.py
--rw-r--r--   0        0        0     1235 2023-04-23 05:05:10.763636 async_fm-0.0.1/src/asyncfm/types.py
--rw-r--r--   0        0        0      206 2023-04-23 05:05:10.763636 async_fm-0.0.1/src/asyncfm/utils.py
--rw-r--r--   0        0        0     2273 1970-01-01 00:00:00.000000 async_fm-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-23 06:34:10.655999 async_fm-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1590 2023-04-23 06:34:10.655999 async_fm-0.0.2/README.md
+-rw-r--r--   0        0        0      683 2023-04-23 06:34:10.655999 async_fm-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       76 2023-04-23 06:34:10.655999 async_fm-0.0.2/src/asyncfm/__init__.py
+-rw-r--r--   0        0        0     1296 2023-04-23 06:34:10.655999 async_fm-0.0.2/src/asyncfm/api/__init__.py
+-rw-r--r--   0        0        0    14947 2023-04-23 06:34:10.655999 async_fm-0.0.2/src/asyncfm/api/user.py
+-rw-r--r--   0        0        0     2424 2023-04-23 06:34:10.655999 async_fm-0.0.2/src/asyncfm/exceptions.py
+-rw-r--r--   0        0        0     1235 2023-04-23 06:34:10.655999 async_fm-0.0.2/src/asyncfm/types.py
+-rw-r--r--   0        0        0      206 2023-04-23 06:34:10.655999 async_fm-0.0.2/src/asyncfm/utils.py
+-rw-r--r--   0        0        0     2273 1970-01-01 00:00:00.000000 async_fm-0.0.2/PKG-INFO
```

### Comparing `async_fm-0.0.1/LICENSE` & `async_fm-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `async_fm-0.0.1/README.md` & `async_fm-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `async_fm-0.0.1/pyproject.toml` & `async_fm-0.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "Async-FM"
-version = "0.0.1"
+version = "0.0.2"
 description = "Python library for interacting with the Last.fm API asynchronously."
 authors = ["NachABR <nachabr@protonmail.com>"]
 license = "MIT"
 readme = "README.md"
-packages = [{include = "src"}]
+packages = [{include = "asyncfm", from = "src"}]
 homepage = "https://github.com/NachABR/async-fm"
 repository = "https://github.com/NachABR/async-fm.git"
 keywords = ["python", "lastfm", "aiohttp", "async"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 aiohttp = ">=3.7"
```

### Comparing `async_fm-0.0.1/src/asyncfm/api/__init__.py` & `async_fm-0.0.2/src/asyncfm/api/__init__.py`

 * *Files identical despite different names*

### Comparing `async_fm-0.0.1/src/asyncfm/api/user.py` & `async_fm-0.0.2/src/asyncfm/api/user.py`

 * *Files identical despite different names*

### Comparing `async_fm-0.0.1/src/asyncfm/exceptions.py` & `async_fm-0.0.2/src/asyncfm/exceptions.py`

 * *Files identical despite different names*

### Comparing `async_fm-0.0.1/src/asyncfm/types.py` & `async_fm-0.0.2/src/asyncfm/types.py`

 * *Files identical despite different names*

### Comparing `async_fm-0.0.1/PKG-INFO` & `async_fm-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-fm
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python library for interacting with the Last.fm API asynchronously.
 Home-page: https://github.com/NachABR/async-fm
 License: MIT
 Keywords: python,lastfm,aiohttp,async
 Author: NachABR
 Author-email: nachabr@protonmail.com
 Requires-Python: >=3.10,<4.0
```

