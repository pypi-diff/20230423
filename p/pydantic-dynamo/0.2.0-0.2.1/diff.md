# Comparing `tmp/pydantic_dynamo-0.2.0.tar.gz` & `tmp/pydantic_dynamo-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_dynamo-0.2.0.tar", max compression
+gzip compressed data, was "pydantic_dynamo-0.2.1.tar", max compression
```

## Comparing `pydantic_dynamo-0.2.0.tar` & `pydantic_dynamo-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0     1121 2023-03-07 03:45:50.202681 pydantic_dynamo-0.2.0/LICENSE
--rw-r--r--   0        0        0        0 2023-03-07 03:36:36.814175 pydantic_dynamo-0.2.0/pydantic_dynamo/__init__.py
--rw-r--r--   0        0        0      243 2023-04-04 19:40:26.272160 pydantic_dynamo-0.2.0/pydantic_dynamo/constants.py
--rw-r--r--   0        0        0       53 2023-03-07 03:09:09.986643 pydantic_dynamo-0.2.0/pydantic_dynamo/exceptions.py
--rw-r--r--   0        0        0     3294 2023-04-19 02:51:16.873917 pydantic_dynamo-0.2.0/pydantic_dynamo/models.py
--rw-r--r--   0        0        0    14586 2023-04-13 17:24:33.661892 pydantic_dynamo-0.2.0/pydantic_dynamo/repository.py
--rw-r--r--   0        0        0    10579 2023-04-19 02:51:16.873917 pydantic_dynamo-0.2.0/pydantic_dynamo/utils.py
--rw-r--r--   0        0        0        0 2023-04-04 19:23:43.683503 pydantic_dynamo-0.2.0/pydantic_dynamo/v2/__init__.py
--rw-r--r--   0        0        0     4200 2023-04-19 15:32:16.137607 pydantic_dynamo-0.2.0/pydantic_dynamo/v2/models.py
--rw-r--r--   0        0        0    16452 2023-04-19 17:58:49.187593 pydantic_dynamo-0.2.0/pydantic_dynamo/v2/repository.py
--rw-r--r--   0        0        0     3703 2023-04-19 15:48:17.692524 pydantic_dynamo-0.2.0/pydantic_dynamo/v2/sync_repository.py
--rw-r--r--   0        0        0     1190 2023-04-19 17:59:23.770865 pydantic_dynamo-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    15133 2023-04-19 17:57:46.241111 pydantic_dynamo-0.2.0/README.md
--rw-r--r--   0        0        0    15912 1970-01-01 00:00:00.000000 pydantic_dynamo-0.2.0/setup.py
--rw-r--r--   0        0        0    15340 1970-01-01 00:00:00.000000 pydantic_dynamo-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1121 2023-03-07 03:45:50.202681 pydantic_dynamo-0.2.1/LICENSE
+-rw-r--r--   0        0        0        0 2023-03-07 03:36:36.814175 pydantic_dynamo-0.2.1/pydantic_dynamo/__init__.py
+-rw-r--r--   0        0        0      243 2023-04-04 19:40:26.272160 pydantic_dynamo-0.2.1/pydantic_dynamo/constants.py
+-rw-r--r--   0        0        0       53 2023-03-07 03:09:09.986643 pydantic_dynamo-0.2.1/pydantic_dynamo/exceptions.py
+-rw-r--r--   0        0        0     3294 2023-04-19 02:51:16.873917 pydantic_dynamo-0.2.1/pydantic_dynamo/models.py
+-rw-r--r--   0        0        0    14586 2023-04-13 17:24:33.661892 pydantic_dynamo-0.2.1/pydantic_dynamo/repository.py
+-rw-r--r--   0        0        0    10579 2023-04-19 02:51:16.873917 pydantic_dynamo-0.2.1/pydantic_dynamo/utils.py
+-rw-r--r--   0        0        0        0 2023-04-04 19:23:43.683503 pydantic_dynamo-0.2.1/pydantic_dynamo/v2/__init__.py
+-rw-r--r--   0        0        0     4355 2023-04-23 13:36:23.098647 pydantic_dynamo-0.2.1/pydantic_dynamo/v2/models.py
+-rw-r--r--   0        0        0    16611 2023-04-23 13:30:24.492470 pydantic_dynamo-0.2.1/pydantic_dynamo/v2/repository.py
+-rw-r--r--   0        0        0     3781 2023-04-23 13:31:55.765230 pydantic_dynamo-0.2.1/pydantic_dynamo/v2/sync_repository.py
+-rw-r--r--   0        0        0     1190 2023-04-23 13:42:21.894819 pydantic_dynamo-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0    15243 2023-04-20 16:42:35.339053 pydantic_dynamo-0.2.1/README.md
+-rw-r--r--   0        0        0    15448 1970-01-01 00:00:00.000000 pydantic_dynamo-0.2.1/PKG-INFO
```

### Comparing `pydantic_dynamo-0.2.0/LICENSE` & `pydantic_dynamo-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_dynamo-0.2.0/pydantic_dynamo/models.py` & `pydantic_dynamo-0.2.1/pydantic_dynamo/models.py`

 * *Files identical despite different names*

### Comparing `pydantic_dynamo-0.2.0/pydantic_dynamo/repository.py` & `pydantic_dynamo-0.2.1/pydantic_dynamo/repository.py`

 * *Files identical despite different names*

### Comparing `pydantic_dynamo-0.2.0/pydantic_dynamo/utils.py` & `pydantic_dynamo-0.2.1/pydantic_dynamo/utils.py`

 * *Files identical despite different names*

### Comparing `pydantic_dynamo-0.2.0/pydantic_dynamo/v2/models.py` & `pydantic_dynamo-0.2.1/pydantic_dynamo/v2/models.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,62 +1,71 @@
-from abc import abstractmethod, ABC
-from typing import Generic, Optional, Iterable, Sequence, Tuple, AsyncIterable
+from abc import abstractmethod
+from contextlib import AbstractContextManager, AbstractAsyncContextManager
+from typing import (
+    Generic,
+    Optional,
+    Iterable,
+    Sequence,
+    Tuple,
+    AsyncIterator,
+    Iterator,
+)
 
 from pydantic.generics import GenericModel
 
 from pydantic_dynamo.models import ObjT, PartitionedContent, FilterCommand, UpdateCommand
 
 
 class GetResponse(GenericModel, Generic[ObjT]):
     content: Optional[PartitionedContent[ObjT]]
 
 
 class BatchResponse(GenericModel, Generic[ObjT]):
     contents: Iterable[PartitionedContent[ObjT]]
 
 
-class ReadOnlyAbstractRepository(ABC, Generic[ObjT]):
+class ReadOnlyAbstractRepository(AbstractAsyncContextManager, Generic[ObjT]):
     @abstractmethod
     async def get(
         self, partition_id: Optional[Sequence[str]], content_id: Optional[Sequence[str]]
     ) -> GetResponse:
         pass
 
     @abstractmethod
     def get_batch(
         self,
         request_ids: Sequence[Tuple[Optional[Sequence[str]], Optional[Sequence[str]]]],
-    ) -> AsyncIterable[BatchResponse]:
+    ) -> AsyncIterator[BatchResponse]:
         pass
 
     @abstractmethod
     def list(
         self,
         partition_id: Optional[Sequence[str]],
         content_prefix: Optional[Sequence[str]],
         sort_ascending: bool = True,
         limit: Optional[int] = None,
         filters: Optional[FilterCommand] = None,
-    ) -> AsyncIterable[BatchResponse]:
+    ) -> AsyncIterator[BatchResponse]:
         pass
 
     @abstractmethod
     def list_between(
         self,
         partition_id: Optional[Sequence[str]],
         content_start: Optional[Sequence[str]],
         content_end: Optional[Sequence[str]],
         sort_ascending: bool = True,
         limit: Optional[int] = None,
         filters: Optional[FilterCommand] = None,
-    ) -> AsyncIterable[BatchResponse]:
+    ) -> AsyncIterator[BatchResponse]:
         pass
 
 
-class AbstractRepository(ReadOnlyAbstractRepository[ObjT], ABC):
+class AbstractRepository(ReadOnlyAbstractRepository[ObjT]):
     @abstractmethod
     async def put(self, content: PartitionedContent[ObjT]) -> None:
         pass
 
     @abstractmethod
     async def put_batch(self, content: Iterable[PartitionedContent[ObjT]]) -> None:
         pass
@@ -76,53 +85,53 @@
         self,
         partition_id: Optional[Sequence[str]],
         content_prefix: Optional[Sequence[str]],
     ) -> None:
         pass
 
 
-class SyncReadOnlyAbstractRepository(ABC, Generic[ObjT]):
+class SyncReadOnlyAbstractRepository(AbstractContextManager, Generic[ObjT]):
     @abstractmethod
     def get(
         self, partition_id: Optional[Sequence[str]], content_id: Optional[Sequence[str]]
     ) -> GetResponse:
         pass
 
     @abstractmethod
     def get_batch(
         self,
         request_ids: Sequence[Tuple[Optional[Sequence[str]], Optional[Sequence[str]]]],
-    ) -> Iterable[BatchResponse]:
+    ) -> Iterator[BatchResponse]:
         pass
 
     @abstractmethod
     def list(
         self,
         partition_id: Optional[Sequence[str]],
         content_prefix: Optional[Sequence[str]],
         sort_ascending: bool = True,
         limit: Optional[int] = None,
         filters: Optional[FilterCommand] = None,
-    ) -> Iterable[BatchResponse]:
+    ) -> Iterator[BatchResponse]:
         pass
 
     @abstractmethod
     def list_between(
         self,
         partition_id: Optional[Sequence[str]],
         content_start: Optional[Sequence[str]],
         content_end: Optional[Sequence[str]],
         sort_ascending: bool = True,
         limit: Optional[int] = None,
         filters: Optional[FilterCommand] = None,
-    ) -> Iterable[BatchResponse]:
+    ) -> Iterator[BatchResponse]:
         pass
 
 
-class SyncAbstractRepository(SyncReadOnlyAbstractRepository[ObjT], ABC):
+class SyncAbstractRepository(SyncReadOnlyAbstractRepository[ObjT]):
     @abstractmethod
     def put(self, content: PartitionedContent[ObjT]) -> None:
         pass
 
     @abstractmethod
     def put_batch(self, content: Iterable[PartitionedContent[ObjT]]) -> None:
         pass
```

### Comparing `pydantic_dynamo-0.2.0/pydantic_dynamo/v2/repository.py` & `pydantic_dynamo-0.2.1/pydantic_dynamo/v2/repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,24 @@
 from __future__ import annotations
 
 import logging
 from datetime import datetime, timezone
-from typing import Type, Dict, List, Any, Iterable, Union, Optional, Sequence, Tuple, AsyncIterable
+from typing import (
+    Type,
+    Dict,
+    List,
+    Any,
+    Iterable,
+    Union,
+    Optional,
+    Sequence,
+    Tuple,
+    AsyncGenerator,
+    AsyncIterator,
+)
 
 from boto3.dynamodb.conditions import Key
 
 from pydantic_dynamo.constants import (
     EMPTY_LIST,
     INTERNAL_OBJECT_VERSION,
     INTERNAL_TTL,
@@ -70,14 +82,17 @@
         self._content_type = content_type
         self._table_name = table_name
         self._partition_key = partition_key
         self._sort_key = sort_key
         self._table = table
         self._resource = resource
 
+    async def __aexit__(self, exc_type, exc_val, exc_tb):
+        pass
+
     @property
     def context(self) -> Dict[str, str]:
         return {
             "item_class": self._item_class.__name__,
             "partition_prefix": self._partition_id(EMPTY_LIST),
             "content_prefix": self._content_id(EMPTY_LIST),
         }
@@ -161,15 +176,15 @@
             logger.info("No item found in table by key", extra=log_context)
             content = None
         return GetResponse(content=content)
 
     async def get_batch(
         self,
         request_ids: Sequence[Tuple[Optional[Sequence[str]], Optional[Sequence[str]]]],
-    ) -> AsyncIterable[BatchResponse]:
+    ) -> AsyncIterator[BatchResponse]:
         batch_number = 0
         for request_id_batch in chunks(request_ids, size=100):
             batch_number += 1
             logger.info(
                 "Starting batch get items request",
                 extra={
                     "batch_number": batch_number,
@@ -213,15 +228,15 @@
     async def list(
         self,
         partition_id: Optional[Sequence[str]],
         content_prefix: Optional[Sequence[str]],
         sort_ascending: bool = True,
         limit: Optional[int] = None,
         filters: Optional[FilterCommand] = None,
-    ) -> AsyncIterable[BatchResponse]:
+    ) -> AsyncIterator[BatchResponse]:
         if partition_id is None:
             partition_id = EMPTY_LIST
         if content_prefix is None:
             content_prefix = EMPTY_LIST
 
         condition = Key(self._partition_key).eq(self._partition_id(partition_id)) & Key(
             self._sort_key
@@ -238,15 +253,15 @@
         self,
         partition_id: Optional[Sequence[str]],
         content_start: Optional[Sequence[str]],
         content_end: Optional[Sequence[str]],
         sort_ascending: bool = True,
         limit: Optional[int] = None,
         filters: Optional[FilterCommand] = None,
-    ) -> AsyncIterable[BatchResponse]:
+    ) -> AsyncIterator[BatchResponse]:
         log_context = {
             "partition_id": partition_id,
             "content_start": content_start,
             "content_end": content_end,
             **self.context,
         }
         if partition_id is None:
@@ -354,15 +369,15 @@
     async def _query_all_data(
         self,
         key_condition_expression: Key,
         sort_ascending: bool = True,
         limit: Optional[int] = None,
         filters: Optional[FilterCommand] = None,
         select_fields: Optional[Sequence[str]] = None,
-    ) -> AsyncIterable[List[Dict]]:
+    ) -> AsyncGenerator[List[Dict], None]:
         query_kwargs = {
             "KeyConditionExpression": key_condition_expression,
             "ScanIndexForward": sort_ascending,
         }
         if filters:
             validate_filters_for_schema(self._item_schema, filters)
             if filter_expression := build_filter_expression(filters):
```

### Comparing `pydantic_dynamo-0.2.0/pydantic_dynamo/v2/sync_repository.py` & `pydantic_dynamo-0.2.1/pydantic_dynamo/v2/sync_repository.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import asyncio
 from asyncio import AbstractEventLoop
-from typing import Optional, Sequence, Iterable, Tuple, AsyncIterable, TypeVar
+from typing import Optional, Sequence, Iterable, Tuple, AsyncIterable, TypeVar, Iterator
 
 from pydantic_dynamo.models import ObjT, FilterCommand, UpdateCommand, PartitionedContent
 from pydantic_dynamo.v2.models import (
     SyncAbstractRepository,
     BatchResponse,
     GetResponse,
     AbstractRepository,
@@ -14,14 +14,17 @@
 Output = TypeVar("Output")
 
 
 class SyncDynamoRepository(SyncAbstractRepository[ObjT]):
     def __init__(self, async_repo: AbstractRepository[ObjT]):
         self._async_repo = async_repo
 
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        pass
+
     def put(self, content: PartitionedContent[ObjT]) -> None:
         loop = asyncio.get_event_loop()
         loop.run_until_complete(self._async_repo.put(content))
 
     def put_batch(self, content: Iterable[PartitionedContent[ObjT]]) -> None:
         loop = asyncio.get_event_loop()
         loop.run_until_complete(self._async_repo.put_batch(content))
@@ -48,53 +51,53 @@
         self, partition_id: Optional[Sequence[str]], content_id: Optional[Sequence[str]]
     ) -> GetResponse:
         loop = asyncio.get_event_loop()
         return loop.run_until_complete(self._async_repo.get(partition_id, content_id))
 
     def get_batch(
         self, request_ids: Sequence[Tuple[Optional[Sequence[str]], Optional[Sequence[str]]]]
-    ) -> Iterable[BatchResponse]:
+    ) -> Iterator[BatchResponse]:
         loop = asyncio.get_event_loop()
         return iter_over_async(self._async_repo.get_batch(request_ids), loop)
 
     def list(
         self,
         partition_id: Optional[Sequence[str]],
         content_prefix: Optional[Sequence[str]],
         sort_ascending: bool = True,
         limit: Optional[int] = None,
         filters: Optional[FilterCommand] = None,
-    ) -> Iterable[BatchResponse]:
+    ) -> Iterator[BatchResponse]:
         loop = asyncio.get_event_loop()
         return iter_over_async(
             self._async_repo.list(partition_id, content_prefix, sort_ascending, limit, filters),
             loop,
         )
 
     def list_between(
         self,
         partition_id: Optional[Sequence[str]],
         content_start: Optional[Sequence[str]],
         content_end: Optional[Sequence[str]],
         sort_ascending: bool = True,
         limit: Optional[int] = None,
         filters: Optional[FilterCommand] = None,
-    ) -> Iterable[BatchResponse]:
+    ) -> Iterator[BatchResponse]:
         loop = asyncio.get_event_loop()
         return iter_over_async(
             self._async_repo.list_between(
                 partition_id, content_start, content_end, sort_ascending, limit, filters
             ),
             loop,
         )
 
 
 def iter_over_async(
     async_iterable: AsyncIterable[Output], loop: AbstractEventLoop
-) -> Iterable[Output]:
+) -> Iterator[Output]:
     async_iterator = async_iterable.__aiter__()
 
     async def get_next():
         try:
             next_obj = await async_iterator.__anext__()
             return False, next_obj
         except StopAsyncIteration:
```

### Comparing `pydantic_dynamo-0.2.0/pyproject.toml` & `pydantic_dynamo-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-dynamo"
-version = "0.2.0"
+version = "0.2.1"
 description = ""
 authors = ["David Jetter <davidajetter@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pydantic_dynamo"}]
 homepage = "https://github.com/david-a-jetter/pydantic-dynamo"
 
 [tool.poetry.dependencies]
```

### Comparing `pydantic_dynamo-0.2.0/README.md` & `pydantic_dynamo-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,17 @@
 Or even better, use [Poetry](https://python-poetry.org/docs/):
 ```
 poetry add pydantic-dynamo
 ```
 
 ## Usage
 
-The ideal consumer a developer of a low-to-medium complexity application. You will lose
+All of the goodness of pydantic data modeling, pointed at your DynamoDB table instead of your REST API.
+
+The ideal consumer is a developer of a low-to-medium complexity application. You will lose
 some benefits of the single-table pattern, specifically the ability to query
 and retrieve objects of different types in a single connection. Except the most complex single-table examples, 
 access patterns can be implemented to utilize the `list`/`list_between`
 and `get_batch` functions, documented below, to prevent N+1 queries and provide sufficient performance.
 
 
 ### Table Creation
```

### Comparing `pydantic_dynamo-0.2.0/PKG-INFO` & `pydantic_dynamo-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-dynamo
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Home-page: https://github.com/david-a-jetter/pydantic-dynamo
 Author: David Jetter
 Author-email: davidajetter@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -35,15 +35,17 @@
 Or even better, use [Poetry](https://python-poetry.org/docs/):
 ```
 poetry add pydantic-dynamo
 ```
 
 ## Usage
 
-The ideal consumer a developer of a low-to-medium complexity application. You will lose
+All of the goodness of pydantic data modeling, pointed at your DynamoDB table instead of your REST API.
+
+The ideal consumer is a developer of a low-to-medium complexity application. You will lose
 some benefits of the single-table pattern, specifically the ability to query
 and retrieve objects of different types in a single connection. Except the most complex single-table examples, 
 access patterns can be implemented to utilize the `list`/`list_between`
 and `get_batch` functions, documented below, to prevent N+1 queries and provide sufficient performance.
 
 
 ### Table Creation
```

