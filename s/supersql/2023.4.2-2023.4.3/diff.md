# Comparing `tmp/supersql-2023.4.2.tar.gz` & `tmp/supersql-2023.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "supersql-2023.4.2.tar", max compression
+gzip compressed data, was "supersql-2023.4.3.tar", max compression
```

## Comparing `supersql-2023.4.2.tar` & `supersql-2023.4.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rwxr-xr-x   0        0        0     1048 2023-01-20 23:27:04.000000 supersql-2023.4.2/LICENSE.md
--rwxr-xr-x   0        0        0     3014 2023-01-20 23:22:54.000000 supersql-2023.4.2/README.md
--rwxr-xr-x   0        0        0      861 2023-04-23 10:59:43.342383 supersql-2023.4.2/pyproject.toml
--rwxr-xr-x   0        0        0      269 2023-04-22 21:33:45.498403 supersql-2023.4.2/supersql/__init__.py
--rwxr-xr-x   0        0        0        0 2023-01-21 17:07:28.000000 supersql-2023.4.2/supersql/alternate.py
--rwxr-xr-x   0        0        0     3823 2023-04-22 19:22:20.869838 supersql-2023.4.2/supersql/column.py
--rwxr-xr-x   0        0        0      357 2023-04-22 21:47:06.761429 supersql-2023.4.2/supersql/constants.py
--rwxr-xr-x   0        0        0     1178 2023-01-23 01:14:26.000000 supersql-2023.4.2/supersql/core.py
--rwxr-xr-x   0        0        0     8626 2023-04-22 19:04:57.992610 supersql-2023.4.2/supersql/dquery.py
--rwxr-xr-x   0        0        0      518 2023-01-24 18:41:24.000000 supersql-2023.4.2/supersql/helpers.py
--rwxr-xr-x   0        0        0     8593 2023-04-22 19:50:07.215779 supersql-2023.4.2/supersql/query.py
--rwxr-xr-x   0        0        0     1133 2023-04-22 21:31:41.349988 supersql-2023.4.2/supersql/results.py
--rwxr-xr-x   0        0        0     1894 2023-04-22 11:20:09.187343 supersql-2023.4.2/supersql/table.py
--rw-r--r--   0        0        0     3764 1970-01-01 00:00:00.000000 supersql-2023.4.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1048 2023-01-20 23:27:04.000000 supersql-2023.4.3/LICENSE.md
+-rwxr-xr-x   0        0        0     3014 2023-01-20 23:22:54.000000 supersql-2023.4.3/README.md
+-rwxr-xr-x   0        0        0      861 2023-04-23 11:06:22.920837 supersql-2023.4.3/pyproject.toml
+-rwxr-xr-x   0        0        0      269 2023-04-22 21:33:45.498403 supersql-2023.4.3/supersql/__init__.py
+-rwxr-xr-x   0        0        0        0 2023-01-21 17:07:28.000000 supersql-2023.4.3/supersql/alternate.py
+-rwxr-xr-x   0        0        0     3823 2023-04-22 19:22:20.869838 supersql-2023.4.3/supersql/column.py
+-rwxr-xr-x   0        0        0      357 2023-04-22 21:47:06.761429 supersql-2023.4.3/supersql/constants.py
+-rwxr-xr-x   0        0        0     1178 2023-01-23 01:14:26.000000 supersql-2023.4.3/supersql/core.py
+-rwxr-xr-x   0        0        0     8626 2023-04-22 19:04:57.992610 supersql-2023.4.3/supersql/dquery.py
+-rwxr-xr-x   0        0        0      518 2023-01-24 18:41:24.000000 supersql-2023.4.3/supersql/helpers.py
+-rwxr-xr-x   0        0        0     8593 2023-04-22 19:50:07.215779 supersql-2023.4.3/supersql/query.py
+-rwxr-xr-x   0        0        0     1133 2023-04-22 21:31:41.349988 supersql-2023.4.3/supersql/results.py
+-rwxr-xr-x   0        0        0     1894 2023-04-22 11:20:09.187343 supersql-2023.4.3/supersql/table.py
+-rw-r--r--   0        0        0     3714 1970-01-01 00:00:00.000000 supersql-2023.4.3/PKG-INFO
```

### Comparing `supersql-2023.4.2/LICENSE.md` & `supersql-2023.4.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `supersql-2023.4.2/README.md` & `supersql-2023.4.3/README.md`

 * *Files identical despite different names*

### Comparing `supersql-2023.4.2/pyproject.toml` & `supersql-2023.4.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "supersql"
-version = "2023.4.2"
+version = "2023.4.3"
 description = "Thin wrapper on top of SQL that enables you write SQL code in python easily"
 authors = ["Tersoo Ortserga <codesage@live.com>"]
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
-python = "^3.6"
+python = "^3.7"
 asyncpg = "^0.27.0"
 
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.1"
 pytest-asyncio = "^0.21.0"
 aiosqlite = "^0.19.0"
```

### Comparing `supersql-2023.4.2/supersql/column.py` & `supersql-2023.4.3/supersql/column.py`

 * *Files identical despite different names*

### Comparing `supersql-2023.4.2/supersql/core.py` & `supersql-2023.4.3/supersql/core.py`

 * *Files identical despite different names*

### Comparing `supersql-2023.4.2/supersql/dquery.py` & `supersql-2023.4.3/supersql/dquery.py`

 * *Files identical despite different names*

### Comparing `supersql-2023.4.2/supersql/helpers.py` & `supersql-2023.4.3/supersql/helpers.py`

 * *Files identical despite different names*

### Comparing `supersql-2023.4.2/supersql/query.py` & `supersql-2023.4.3/supersql/query.py`

 * *Files identical despite different names*

### Comparing `supersql-2023.4.2/supersql/results.py` & `supersql-2023.4.3/supersql/results.py`

 * *Files identical despite different names*

### Comparing `supersql-2023.4.2/supersql/table.py` & `supersql-2023.4.3/supersql/table.py`

 * *Files identical despite different names*

### Comparing `supersql-2023.4.2/PKG-INFO` & `supersql-2023.4.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: supersql
-Version: 2023.4.2
+Version: 2023.4.3
 Summary: Thin wrapper on top of SQL that enables you write SQL code in python easily
 Author: Tersoo Ortserga
 Author-email: codesage@live.com
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: mysql
 Provides-Extra: postgres
```

