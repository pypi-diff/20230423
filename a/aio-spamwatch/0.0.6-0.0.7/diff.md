# Comparing `tmp/aio_spamwatch-0.0.6.tar.gz` & `tmp/aio_spamwatch-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio_spamwatch-0.0.6.tar", max compression
+gzip compressed data, was "aio_spamwatch-0.0.7.tar", max compression
```

## Comparing `aio_spamwatch-0.0.6.tar` & `aio_spamwatch-0.0.7.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     7652 2023-04-20 23:08:31.066297 aio_spamwatch-0.0.6/LICENSE
--rw-r--r--   0        0        0     1063 2023-04-22 00:13:31.977315 aio_spamwatch-0.0.6/README.md
--rw-r--r--   0        0        0      651 2023-04-22 00:29:35.140658 aio_spamwatch-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      450 2023-04-22 00:29:35.140658 aio_spamwatch-0.0.6/src/aio_spamwatch/__init__.py
--rw-r--r--   0        0        0     5930 2023-04-21 22:38:29.797251 aio_spamwatch-0.0.6/src/aio_spamwatch/client.py
--rw-r--r--   0        0        0     1299 2023-04-21 00:21:40.506347 aio_spamwatch-0.0.6/src/aio_spamwatch/errors.py
--rw-r--r--   0        0        0      526 2023-04-21 21:41:44.300547 aio_spamwatch-0.0.6/src/aio_spamwatch/types.py
--rw-r--r--   0        0        0     1795 1970-01-01 00:00:00.000000 aio_spamwatch-0.0.6/setup.py
--rw-r--r--   0        0        0     1725 1970-01-01 00:00:00.000000 aio_spamwatch-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     7652 2023-04-23 16:37:46.674917 aio_spamwatch-0.0.7/LICENSE
+-rw-r--r--   0        0        0     1063 2023-04-23 16:37:46.674917 aio_spamwatch-0.0.7/README.md
+-rw-r--r--   0        0        0      675 2023-04-23 16:37:46.674917 aio_spamwatch-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      450 2023-04-23 16:37:46.674917 aio_spamwatch-0.0.7/src/aio_spamwatch/__init__.py
+-rw-r--r--   0        0        0     5930 2023-04-23 16:37:46.674917 aio_spamwatch-0.0.7/src/aio_spamwatch/client.py
+-rw-r--r--   0        0        0     1299 2023-04-23 16:37:46.674917 aio_spamwatch-0.0.7/src/aio_spamwatch/errors.py
+-rw-r--r--   0        0        0      526 2023-04-23 16:37:46.674917 aio_spamwatch-0.0.7/src/aio_spamwatch/types.py
+-rw-r--r--   0        0        0     1725 1970-01-01 00:00:00.000000 aio_spamwatch-0.0.7/PKG-INFO
```

### Comparing `aio_spamwatch-0.0.6/LICENSE` & `aio_spamwatch-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aio_spamwatch-0.0.6/README.md` & `aio_spamwatch-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `aio_spamwatch-0.0.6/pyproject.toml` & `aio_spamwatch-0.0.7/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "aio-spamwatch"
-version = "0.0.6"
+version = "0.0.7"
 description = "An asynchronous Python wrapper for the SpamWatch API."
 authors = ["NachABR <nachabr@protonmail.com>"]
 license = "LGPLv3"
 homepage = "https://github.com/NachABR/aio-spamwatch"
 repository = "https://github.com/NachABR/aio-spamwatch.git"
 keywords = ["spamwatch", "asynchronous", "aiohttp", "telegram"]
 readme = "README.md"
 
-packages = [{include = "src"}]
+packages = [{include = "aio_spamwatch", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 aiohttp = ">=3.7"
 
 [tool.poetry.group.dev.dependencies]
 pylint = "^2.17.2"
```

### Comparing `aio_spamwatch-0.0.6/src/aio_spamwatch/client.py` & `aio_spamwatch-0.0.7/src/aio_spamwatch/client.py`

 * *Files identical despite different names*

### Comparing `aio_spamwatch-0.0.6/src/aio_spamwatch/errors.py` & `aio_spamwatch-0.0.7/src/aio_spamwatch/errors.py`

 * *Files identical despite different names*

### Comparing `aio_spamwatch-0.0.6/src/aio_spamwatch/types.py` & `aio_spamwatch-0.0.7/src/aio_spamwatch/types.py`

 * *Files identical despite different names*

### Comparing `aio_spamwatch-0.0.6/PKG-INFO` & `aio_spamwatch-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aio-spamwatch
-Version: 0.0.6
+Version: 0.0.7
 Summary: An asynchronous Python wrapper for the SpamWatch API.
 Home-page: https://github.com/NachABR/aio-spamwatch
 License: LGPLv3
 Keywords: spamwatch,asynchronous,aiohttp,telegram
 Author: NachABR
 Author-email: nachabr@protonmail.com
 Requires-Python: >=3.10,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aio-spamwatch Version: 0.0.6 Summary: An
+Metadata-Version: 2.1 Name: aio-spamwatch Version: 0.0.7 Summary: An
 asynchronous Python wrapper for the SpamWatch API. Home-page: https://
 github.com/NachABR/aio-spamwatch License: LGPLv3 Keywords:
 spamwatch,asynchronous,aiohttp,telegram Author: NachABR Author-email:
 nachabr@protonmail.com Requires-Python: >=3.10,<4.0 Classifier: License ::
 Other/Proprietary License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: aiohttp (>=3.7) Project-URL:
```

