# Comparing `tmp/fondat-salesforce-4.0b3.tar.gz` & `tmp/fondat_salesforce-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fondat-salesforce-4.0b3.tar", max compression
+gzip compressed data, was "fondat_salesforce-4.1.0.tar", max compression
```

## Comparing `fondat-salesforce-4.0b3.tar` & `fondat_salesforce-4.1.0.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1065 2022-02-24 07:21:58.358948 fondat-salesforce-4.0b3/LICENSE
--rw-r--r--   0        0        0      848 2021-12-13 07:41:09.813485 fondat-salesforce-4.0b3/README.md
--rw-r--r--   0        0        0       41 2021-12-13 07:39:59.373483 fondat-salesforce-4.0b3/fondat/salesforce/__init__.py
--rw-r--r--   0        0        0     4249 2022-06-29 16:23:43.050900 fondat-salesforce-4.0b3/fondat/salesforce/bulk.py
--rw-r--r--   0        0        0     3924 2022-06-29 16:02:36.017544 fondat-salesforce-4.0b3/fondat/salesforce/client.py
--rw-r--r--   0        0        0     4968 2022-09-30 16:45:55.524115 fondat-salesforce-4.0b3/fondat/salesforce/jobs.py
--rw-r--r--   0        0        0     1294 2022-09-30 16:46:33.100986 fondat-salesforce-4.0b3/fondat/salesforce/limits.py
--rw-r--r--   0        0        0     6118 2022-10-05 22:36:35.642846 fondat-salesforce-4.0b3/fondat/salesforce/oauth.py
--rw-r--r--   0        0        0     1315 2022-09-30 16:47:49.351449 fondat-salesforce-4.0b3/fondat/salesforce/service.py
--rw-r--r--   0        0        0     7098 2022-09-30 16:48:12.481602 fondat-salesforce-4.0b3/fondat/salesforce/sobjects.py
--rw-r--r--   0        0        0     1131 2022-10-05 22:37:56.749819 fondat-salesforce-4.0b3/pyproject.toml
--rw-r--r--   0        0        0     1570 2022-10-05 22:38:11.271817 fondat-salesforce-4.0b3/setup.py
--rw-r--r--   0        0        0     1633 2022-10-05 22:38:11.271988 fondat-salesforce-4.0b3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-02-24 07:21:58.358948 fondat_salesforce-4.1.0/LICENSE
+-rw-r--r--   0        0        0      848 2021-12-13 07:41:09.813485 fondat_salesforce-4.1.0/README.md
+-rw-r--r--   0        0        0       41 2021-12-13 07:39:59.373483 fondat_salesforce-4.1.0/fondat/salesforce/__init__.py
+-rw-r--r--   0        0        0     4773 2023-04-23 15:59:30.418046 fondat_salesforce-4.1.0/fondat/salesforce/bulk.py
+-rw-r--r--   0        0        0     3929 2023-03-23 00:50:08.367095 fondat_salesforce-4.1.0/fondat/salesforce/client.py
+-rw-r--r--   0        0        0     4792 2023-01-30 03:59:41.323045 fondat_salesforce-4.1.0/fondat/salesforce/jobs.py
+-rw-r--r--   0        0        0     1294 2022-09-30 16:46:33.100986 fondat_salesforce-4.1.0/fondat/salesforce/limits.py
+-rw-r--r--   0        0        0     6098 2022-10-09 18:47:21.923140 fondat_salesforce-4.1.0/fondat/salesforce/oauth.py
+-rw-r--r--   0        0        0     1315 2022-09-30 16:47:49.351449 fondat_salesforce-4.1.0/fondat/salesforce/service.py
+-rw-r--r--   0        0        0     7098 2022-09-30 16:48:12.481602 fondat_salesforce-4.1.0/fondat/salesforce/sobjects.py
+-rw-r--r--   0        0        0     1139 2023-04-23 16:01:19.718337 fondat_salesforce-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1695 1970-01-01 00:00:00.000000 fondat_salesforce-4.1.0/PKG-INFO
```

### Comparing `fondat-salesforce-4.0b3/LICENSE` & `fondat_salesforce-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fondat-salesforce-4.0b3/README.md` & `fondat_salesforce-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `fondat-salesforce-4.0b3/fondat/salesforce/bulk.py` & `fondat_salesforce-4.1.0/fondat/salesforce/bulk.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Fondat Salesforce bulk module."""
 
 import asyncio
 
-from collections import deque
+from collections import deque, namedtuple
+from collections.abc import Iterable
 from contextlib import suppress
-from fondat.csv import typeddict_codec
+from fondat.csv import TypedDictCodec
 from fondat.salesforce.client import Client
 from fondat.salesforce.jobs import queries_resource
 from fondat.salesforce.sobjects import SObject, sobject_field_type
 from time import time
 from typing import Any, TypedDict
 
 
@@ -18,48 +19,61 @@
 class SObjectQuery:
     """
     Performs an asynchronous bulk data query.
 
     Parameters:
     • client: client object through which to perform queries
     • sobject: Salesforce object metadata
-    • fields: names of fields to be selected
+    • columns: columns to select  [all fields]
     • where: query conditon expression
     • order_by: order of query results
     • limit: maximum number of rows in query results
     • page_size: number of rows to retrieve per page
     • timeout: seconds to wait for query job to complete
     """
 
+    Column = namedtuple("Column", "name, expression, type")
+
     def __init__(
         self,
         client: Client,
         sobject: SObject,
         *,
-        fields: set[str] | None = None,
+        columns: Iterable[Column | str] | None = None,
         where: str | None = None,
         order_by: str | None = None,
         limit: int | None = None,
         page_size: int | None = None,
         timeout: int | None = None,
     ):
         self.client = client
         self.page_size = page_size
-        indexed = {field.name: field for field in sobject.fields}
-        if fields is None:
-            fields = [f.name for f in sobject.fields if f.type not in _exclude_types]
-        if len(fields) == 0:
-            raise ValueError("you must query at least one field")
-        for name in fields:
-            if not (field := indexed.get(name)):
-                raise ValueError(f"unknown field: {name}")
+        columns = (
+            [f.name for f in sobject.fields if f.type not in _exclude_types]
+            if columns is None
+            else list(columns)
+        )
+        if len(columns) == 0:
+            raise ValueError("must select at least one column")
+        fields = {field.name: field for field in sobject.fields}
+        for n, column in enumerate(columns):
+            if isinstance(column, SObjectQuery.Column):
+                continue
+            field = fields.get(column)
+            if not field:
+                raise ValueError(f"unknown field: {column}")
             if field.type in _exclude_types:
-                raise ValueError(f"cannot query {field.type} type field: {name}")
-        self.td = TypedDict("QueryDict", {f: sobject_field_type(indexed[f]) for f in fields})
-        self.stmt = f"SELECT {', '.join(fields)} FROM {sobject.name}"
+                raise ValueError(f"cannot query {field.type} type field: {column}")
+            columns[n] = SObjectQuery.Column(column, None, sobject_field_type(field))
+        self.td = TypedDict("QueryDict", {column.name: column.type for column in columns})
+        self.stmt = "SELECT "
+        self.stmt += ", ".join(
+            ((c.expression or c.name) + (f" {c.name}" if c.expression else "")) for c in columns
+        )
+        self.stmt += f" FROM {sobject.name}"
         if where:
             self.stmt += f" WHERE {where}"
         if order_by:
             self.stmt += f" ORDER BY {order_by}"
         if limit:
             self.stmt += f" LIMIT {limit}"
         self.timeout = timeout
@@ -103,15 +117,15 @@
             raise RuntimeError("must iterate within async context")
         return self
 
     async def _next_page(self):
         page = await self.query.results(limit=self.page_size or 1000, cursor=self.cursor)
         self.results = deque(page.items)
         self.cursor = page.cursor
-        self.codec = typeddict_codec(self.td, self.results.popleft())
+        self.codec = TypedDictCodec(self.td, self.results.popleft())
 
     async def __anext__(self) -> dict[str, Any]:
         if self.results is None:
             await self._await_complete()
         if self.results is None or (not self.results and self.cursor):
             await self._next_page()
         if not self.results and not self.cursor:
```

### Comparing `fondat-salesforce-4.0b3/fondat/salesforce/client.py` & `fondat_salesforce-4.1.0/fondat/salesforce/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
                 _logger.debug("%s %s %d", method, url, response.status)
                 if 200 <= response.status <= 299:
                     yield response
                     return
                 elif response.status == 401 and not auth_error:  # only retry once
                     _logger.debug("retrying authentication")
                     auth_error = True
-                    token = None
+                    self.token = None
                     continue
                 elif 500 <= response.status <= 599 and server_errors < self.retries:
                     _logger.debug(f"retrying server error")
                     await asyncio.sleep(2**server_errors)
                     server_errors += 1
                     continue
                 elif 400 <= response.status <= 599:
```

### Comparing `fondat-salesforce-4.0b3/fondat/salesforce/jobs.py` & `fondat_salesforce-4.1.0/fondat/salesforce/jobs.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import http
 import io
 
 from datetime import datetime
 from fondat.codec import JSONCodec
 from fondat.data import datacls
 from fondat.error import NotFoundError
+from fondat.pagination import Page
 from fondat.resource import mutation, operation, query, resource
 from fondat.salesforce.client import Client
 from typing import Literal
 
 
 Operation = Literal["query", "queryAll"]
 ContentType = Literal["CSV"]
@@ -38,26 +39,14 @@
     columnDelimiter: ColumnDelimiter
     numberRecordsProcessed: int | None
     retries: int | None
     totalProcessingTime: int | None
 
 
 @datacls
-class QueryResultsPage:
-    items: list[list[str]]
-    cursor: bytes | None
-
-
-@datacls
-class QueriesPage:
-    items: list[Query]
-    cursor: bytes | None
-
-
-@datacls
 class _QueriesResponse:
     done: bool
     records: list[Query]
     nextRecordsUrl: str | None
 
 
 @datacls
@@ -80,36 +69,33 @@
 
         def __init__(self, id: str):
             self.path = f"{path}/{id}"
 
         @operation
         async def get(self) -> Query:
             """Get information about a query job."""
-
             async with client.request("GET", self.path) as response:
                 return JSONCodec.get(Query).decode(await response.json())
 
         @operation
         async def delete(self):
             """Delete a query job."""
-
             async with client.request("DELETE", self.path):
                 pass
 
         @mutation
         async def abort(self):
             """Abort a query job."""
-
             async with client.request("PATCH", self.path, json={"state": "Aborted"}):
                 pass
 
         @query
         async def results(
             self, limit: int = 1000, cursor: bytes | None = None
-        ) -> QueryResultsPage:
+        ) -> Page[list[str]]:
             """
             Get results for a query job as CSV rows.
 
             The returned page items contain CSV-decoded rows. The first row is the CSV header,
             which contains the names of the columns.
             """
 
@@ -120,35 +106,33 @@
                 method="GET",
                 path=f"{self.path}/results",
                 headers={"Accept": "text/csv"},
                 params=params,
             ) as response:
                 if response.status == http.HTTPStatus.NO_CONTENT.value:
                     raise NotFoundError  # no results yet
-                with io.StringIO(await response.text()) as sio:
+                with io.StringIO(await response.text("utf-8")) as sio:
                     items = [row for row in csv.reader(sio)]
                 locator = response.headers.get("Sforce-Locator")
-            return QueryResultsPage(
-                items=items, cursor=locator.encode() if locator != "null" else None
-            )
+            return Page(items=items, cursor=locator.encode() if locator != "null" else None)
 
     @resource
     class QueriesResource:
         """Asynchronous query jobs."""
 
         @operation
-        async def get(self, cursor: bytes | None = None) -> QueriesPage:
+        async def get(self, cursor: bytes | None = None) -> Page[Query]:
             """Get information about all query jobs."""
 
             params = {"jobType": "V2Query"}
             async with client.request(
                 method="GET", path=cursor.decode() if cursor else path, params=params
             ) as response:
                 json = JSONCodec.get(_QueriesResponse).decode(await response.json())
-            return QueriesPage(
+            return Page(
                 items=json.records,
                 cursor=json.nextRecordsUrl.encode() if json.nextRecordsUrl else None,
             )
 
         @operation
         async def post(self, operation: Operation, query: str) -> Query:
             """Create a query job."""
```

### Comparing `fondat-salesforce-4.0b3/fondat/salesforce/limits.py` & `fondat_salesforce-4.1.0/fondat/salesforce/limits.py`

 * *Files identical despite different names*

### Comparing `fondat-salesforce-4.0b3/fondat/salesforce/oauth.py` & `fondat_salesforce-4.1.0/fondat/salesforce/oauth.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Fondat Salesforce OAuth module."""
 
 import aiohttp
-import fondat.codec
 
 from fondat.codec import JSONCodec
 from fondat.data import datacls
 from fondat.error import UnauthorizedError
 from typing import Literal, Optional
 from urllib.parse import urlencode
```

### Comparing `fondat-salesforce-4.0b3/fondat/salesforce/service.py` & `fondat_salesforce-4.1.0/fondat/salesforce/service.py`

 * *Files identical despite different names*

### Comparing `fondat-salesforce-4.0b3/fondat/salesforce/sobjects.py` & `fondat_salesforce-4.1.0/fondat/salesforce/sobjects.py`

 * *Files identical despite different names*

### Comparing `fondat-salesforce-4.0b3/pyproject.toml` & `fondat_salesforce-4.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -4,43 +4,43 @@
 
 [tool.black]
 line-length = 96
 target-version = ['py310']
 
 [tool.poetry]
 name = "fondat-salesforce"
-version = "4.0b3"
+version = "4.1.0"
 description = "Fondat package for Salesforce."
 readme = "README.md"
 authors = ["fondat-salesforce authors"]
 homepage = "https://github.com/fondat/fondat-salesforce/"
 documentation = "https://github.com/fondat/fondat-salesforce/wiki"
 license = "MIT"
 keywords = ["asgi", "framework", "resource", "openapi"]
 classifiers = [
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries :: Application Frameworks",
 ]
 packages = [
     { include = "fondat" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 aiohttp = "^3.8"
-fondat = "^4.0b4"
+fondat = "^4.1"
 
 [tool.poetry.dev-dependencies]
-black = "^22.6"
-isort = "^5.10.1"
-pre-commit = "^2.20"
-pytest = "^7.1"
-pytest-asyncio = "^0.18"
-pytest-cov = "^3.0"
+black = "^23.3"
+isort = "^5.12"
+pre-commit = "^3.2"
+pytest = "^7.3"
+pytest-asyncio = "^0.21"
+pytest-cov = "^4.0"
 
 [tool.isort]
 profile = "black"
 lexicographical = true
 lines_after_imports = 2
 lines_between_types = 1
 line_length = 96
```

### Comparing `fondat-salesforce-4.0b3/PKG-INFO` & `fondat_salesforce-4.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: fondat-salesforce
-Version: 4.0b3
+Version: 4.1.0
 Summary: Fondat package for Salesforce.
 Home-page: https://github.com/fondat/fondat-salesforce/
 License: MIT
 Keywords: asgi,framework,resource,openapi
 Author: fondat-salesforce authors
 Requires-Python: >=3.10,<4.0
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Dist: aiohttp (>=3.8,<4.0)
-Requires-Dist: fondat (>=4.0b4,<5.0)
+Requires-Dist: fondat (>=4.1,<5.0)
 Project-URL: Documentation, https://github.com/fondat/fondat-salesforce/wiki
 Description-Content-Type: text/markdown
 
 # fondat-salesforce
 
 [![PyPI](https://badge.fury.io/py/fondat-salesforce.svg)](https://badge.fury.io/py/fondat-salesforce)
 [![Python](https://img.shields.io/pypi/pyversions/fondat-core)](https://python.org/)
```

