# Comparing `tmp/arclet-letoderea-0.4.4.tar.gz` & `tmp/arclet-letoderea-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arclet-letoderea-0.4.4.tar", last modified: Fri Apr  7 07:35:29 2023, max compression
+gzip compressed data, was "arclet-letoderea-0.5.0.tar", last modified: Sun Apr 23 14:05:38 2023, max compression
```

## Comparing `arclet-letoderea-0.4.4.tar` & `arclet-letoderea-0.5.0.tar`

### file list

```diff
@@ -1,30 +1,32 @@
--rw-r--r--   0        0        0      663 2023-04-07 07:31:44.430757 arclet-letoderea-0.4.4/arclet/letoderea/__init__.py
--rw-r--r--   0        0        0     5571 2023-04-07 06:50:56.245034 arclet-letoderea-0.4.4/arclet/letoderea/auxiliary.py
--rw-r--r--   0        0        0        0 2023-03-19 17:38:39.637869 arclet-letoderea-0.4.4/arclet/letoderea/builtin/__init__.py
--rw-r--r--   0        0        0     3400 2023-04-05 12:53:10.839567 arclet-letoderea-0.4.4/arclet/letoderea/builtin/breakpoint.py
--rw-r--r--   0        0        0      820 2023-04-07 06:45:50.811871 arclet-letoderea-0.4.4/arclet/letoderea/builtin/depend.py
--rw-r--r--   0        0        0      197 2023-03-31 18:59:49.623386 arclet-letoderea-0.4.4/arclet/letoderea/context.py
--rw-r--r--   0        0        0     5728 2023-03-31 18:59:49.744750 arclet-letoderea-0.4.4/arclet/letoderea/core.py
--rw-r--r--   0        0        0     1686 2023-04-05 12:57:09.204405 arclet-letoderea-0.4.4/arclet/letoderea/decorate.py
--rw-r--r--   0        0        0     1157 2023-03-23 05:47:21.240677 arclet-letoderea-0.4.4/arclet/letoderea/event.py
--rw-r--r--   0        0        0      304 2023-04-07 06:45:50.801739 arclet-letoderea-0.4.4/arclet/letoderea/exceptions.py
--rw-r--r--   0        0        0     6341 2023-04-07 07:32:34.326656 arclet-letoderea-0.4.4/arclet/letoderea/handler.py
--rw-r--r--   0        0        0     2440 2023-04-05 13:23:24.617902 arclet-letoderea-0.4.4/arclet/letoderea/provider.py
--rw-r--r--   0        0        0     5811 2023-03-23 05:47:21.242677 arclet-letoderea-0.4.4/arclet/letoderea/publisher.py
--rw-r--r--   0        0        0     3157 2023-04-05 12:57:09.191974 arclet-letoderea-0.4.4/arclet/letoderea/subscriber.py
--rw-r--r--   0        0        0      443 2023-03-31 18:57:08.493726 arclet-letoderea-0.4.4/arclet/letoderea/typing.py
--rw-r--r--   0        0        0     1091 2022-01-26 08:43:52.013649 arclet-letoderea-0.4.4/LICENSE
--rw-r--r--   0        0        0      983 2023-04-07 07:34:01.459080 arclet-letoderea-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     1115 2023-03-23 05:47:21.236906 arclet-letoderea-0.4.4/README.md
--rw-r--r--   0        0        0     1502 2023-04-05 13:36:42.941007 arclet-letoderea-0.4.4/tests/breakpoint.py
--rw-r--r--   0        0        0     2282 2023-04-07 06:47:47.105418 arclet-letoderea-0.4.4/tests/combine.py
--rw-r--r--   0        0        0     1900 2023-04-05 13:32:55.790320 arclet-letoderea-0.4.4/tests/condition.py
--rw-r--r--   0        0        0     1468 2023-04-05 13:26:02.431017 arclet-letoderea-0.4.4/tests/decorator.py
--rw-r--r--   0        0        0      757 2023-03-23 05:47:21.275678 arclet-letoderea-0.4.4/tests/depend.py
--rw-r--r--   0        0        0      572 2023-04-05 13:20:19.990233 arclet-letoderea-0.4.4/tests/except.py
--rw-r--r--   0        0        0      922 2023-04-07 07:32:54.555902 arclet-letoderea-0.4.4/tests/nest_except.py
--rw-r--r--   0        0        0      776 2023-03-23 05:47:21.277677 arclet-letoderea-0.4.4/tests/test_handler.py
--rw-r--r--   0        0        0      583 2023-04-05 13:13:59.929688 arclet-letoderea-0.4.4/tests/test_param_parser.py
--rw-r--r--   0        0        0     1898 2023-03-23 05:47:21.285678 arclet-letoderea-0.4.4/tests/test_provider.py
--rw-r--r--   0        0        0      758 2023-04-05 13:13:59.916559 arclet-letoderea-0.4.4/tests/test_publisher.py
--rw-r--r--   0        0        0     1837 1970-01-01 00:00:00.000000 arclet-letoderea-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0      664 2023-04-23 09:37:34.234901 arclet-letoderea-0.5.0/arclet/letoderea/__init__.py
+-rw-r--r--   0        0        0     5634 2023-04-23 12:57:29.709109 arclet-letoderea-0.5.0/arclet/letoderea/auxiliary.py
+-rw-r--r--   0        0        0        0 2023-03-19 17:38:39.637869 arclet-letoderea-0.5.0/arclet/letoderea/builtin/__init__.py
+-rw-r--r--   0        0        0     4126 2023-04-23 13:50:53.063424 arclet-letoderea-0.5.0/arclet/letoderea/builtin/breakpoint.py
+-rw-r--r--   0        0        0      820 2023-04-07 06:45:50.811871 arclet-letoderea-0.5.0/arclet/letoderea/builtin/depend.py
+-rw-r--r--   0        0        0      197 2023-03-31 18:59:49.623386 arclet-letoderea-0.5.0/arclet/letoderea/context.py
+-rw-r--r--   0        0        0     5752 2023-04-23 13:49:49.822125 arclet-letoderea-0.5.0/arclet/letoderea/core.py
+-rw-r--r--   0        0        0     1681 2023-04-23 09:37:34.338972 arclet-letoderea-0.5.0/arclet/letoderea/decorate.py
+-rw-r--r--   0        0        0     1157 2023-03-23 05:47:21.240677 arclet-letoderea-0.5.0/arclet/letoderea/event.py
+-rw-r--r--   0        0        0      304 2023-04-07 06:45:50.801739 arclet-letoderea-0.5.0/arclet/letoderea/exceptions.py
+-rw-r--r--   0        0        0     6341 2023-04-07 07:32:34.326656 arclet-letoderea-0.5.0/arclet/letoderea/handler.py
+-rw-r--r--   0        0        0     2689 2023-04-23 10:05:34.641270 arclet-letoderea-0.5.0/arclet/letoderea/provider.py
+-rw-r--r--   0        0        0     5739 2023-04-23 13:09:19.611255 arclet-letoderea-0.5.0/arclet/letoderea/publisher.py
+-rw-r--r--   0        0        0     3157 2023-04-05 12:57:09.191974 arclet-letoderea-0.5.0/arclet/letoderea/subscriber.py
+-rw-r--r--   0        0        0      438 2023-04-23 12:57:29.695404 arclet-letoderea-0.5.0/arclet/letoderea/typing.py
+-rw-r--r--   0        0        0     1091 2022-01-26 08:43:52.013649 arclet-letoderea-0.5.0/LICENSE
+-rw-r--r--   0        0        0      983 2023-04-23 13:54:09.621159 arclet-letoderea-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1435 2023-04-23 14:03:37.949668 arclet-letoderea-0.5.0/README.md
+-rw-r--r--   0        0        0     1527 2023-04-23 13:07:44.994194 arclet-letoderea-0.5.0/tests/breakpoint.py
+-rw-r--r--   0        0        0     2013 2023-04-23 13:38:01.109308 arclet-letoderea-0.5.0/tests/breakpoint1.py
+-rw-r--r--   0        0        0     2282 2023-04-07 06:47:47.105418 arclet-letoderea-0.5.0/tests/combine.py
+-rw-r--r--   0        0        0     1894 2023-04-23 09:37:34.206903 arclet-letoderea-0.5.0/tests/condition.py
+-rw-r--r--   0        0        0     1462 2023-04-23 09:37:34.153727 arclet-letoderea-0.5.0/tests/decorator.py
+-rw-r--r--   0        0        0      751 2023-04-23 09:37:34.246904 arclet-letoderea-0.5.0/tests/depend.py
+-rw-r--r--   0        0        0      574 2023-04-23 09:37:34.259901 arclet-letoderea-0.5.0/tests/except.py
+-rw-r--r--   0        0        0      918 2023-04-23 09:37:34.217955 arclet-letoderea-0.5.0/tests/nest_except.py
+-rw-r--r--   0        0        0      776 2023-03-23 05:47:21.277677 arclet-letoderea-0.5.0/tests/test_handler.py
+-rw-r--r--   0        0        0      583 2023-04-05 13:13:59.929688 arclet-letoderea-0.5.0/tests/test_param_parser.py
+-rw-r--r--   0        0        0     1892 2023-04-23 09:37:34.294207 arclet-letoderea-0.5.0/tests/test_provider.py
+-rw-r--r--   0        0        0      886 2023-04-23 10:03:48.864079 arclet-letoderea-0.5.0/tests/test_provider_validate.py
+-rw-r--r--   0        0        0      784 2023-04-23 13:11:33.978272 arclet-letoderea-0.5.0/tests/test_publisher.py
+-rw-r--r--   0        0        0     2149 1970-01-01 00:00:00.000000 arclet-letoderea-0.5.0/PKG-INFO
```

### Comparing `arclet-letoderea-0.4.4/arclet/letoderea/__init__.py` & `arclet-letoderea-0.5.0/arclet/letoderea/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,13 +14,13 @@
     SupplyAuxiliary,
     auxilia,
 )
 from .builtin.breakpoint import Breakpoint, StepOut
 from .builtin.depend import Depend, Depends
 from .context import system_ctx
 from .core import EventSystem
-from .decorate import bind, register
+from .decorate import bind, subscribe
 from .event import BaseEvent
 from .exceptions import JudgementError, ParsingStop, PropagationCancelled
 from .provider import Param, Provider, provide
 from .publisher import Publisher
 from .typing import Contexts, Force
```

### Comparing `arclet-letoderea-0.4.4/arclet/letoderea/auxiliary.py` & `arclet-letoderea-0.5.0/arclet/letoderea/auxiliary.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,36 +132,36 @@
             cb.append(aux)
     return res
 
 
 @overload
 def auxilia(
     atype: Literal[AuxType.supply],
-    mode: CombineMode,
+    mode: CombineMode = CombineMode.SINGLE,
     prepare: Callable[[Contexts], Optional[Contexts]] | None = None,
     complete: Callable[[Contexts], Optional[Contexts]] | None = None,
     cleanup: Callable[[Contexts], Optional[Contexts]] | None = None,
 ):
     ...
 
 
 @overload
 def auxilia(
     atype: Literal[AuxType.judge],
-    mode: CombineMode,
+    mode: CombineMode = CombineMode.SINGLE,
     prepare: Callable[[Contexts], Optional[bool]] | None = None,
     complete: Callable[[Contexts], Optional[bool]] | None = None,
     cleanup: Callable[[Contexts], Optional[bool]] | None = None,
 ):
     ...
 
 
 def auxilia(
     atype: AuxType,
-    mode: CombineMode,
+    mode: CombineMode = CombineMode.SINGLE,
     prepare: Callable[[Contexts], Any] | None = None,
     complete: Callable[[Contexts], Any] | None = None,
     cleanup: Callable[[Contexts], Any] | None = None,
 ):
     class _Auxiliary(BaseAuxiliary):
         async def __call__(self, scope: Scope, context: Contexts):
             res = None
```

### Comparing `arclet-letoderea-0.4.4/arclet/letoderea/builtin/breakpoint.py` & `arclet-letoderea-0.5.0/arclet/letoderea/builtin/breakpoint.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,90 +1,119 @@
 import asyncio
 from asyncio import Future
-from typing import Any, Callable, List, Optional, Set, Type, Union
+from typing import (
+    AsyncIterator,
+    Awaitable,
+    Callable,
+    Generic,
+    List,
+    Optional,
+    Set,
+    Type,
+    TypeVar,
+    Union,
+)
 
-from ..auxiliary import Scope, AuxType, BaseAuxiliary
-from ..core import BackendPublisher, EventSystem
+from ..auxiliary import AuxType, BaseAuxiliary, Scope
+from ..core import BackendPublisher, EventSystem, system_ctx
 from ..event import BaseEvent
 from ..exceptions import PropagationCancelled
 from ..handler import depend_handler
 from ..provider import Provider
 from ..typing import Contexts, TCallable
 
+_backend = {}
+R = TypeVar("R")
 
-class StepOut(BaseAuxiliary):
+
+class _step_iter(AsyncIterator[R]):
+    def __init__(self, step: "StepOut[R]"):
+        self.step = step
+
+    def __anext__(self) -> Awaitable[R]:
+        bp = _backend.setdefault(0, Breakpoint(system_ctx.get()))
+        return bp(self.step)
+
+
+class StepOut(BaseAuxiliary, Generic[R]):
     target: Set[Type[BaseEvent]]
     providers: List[Union[Provider, Type[Provider]]]
     auxiliaries: List[BaseAuxiliary]
-    handler: Callable[..., Any]
+    handler: Union[Callable[..., Awaitable[R]], Callable[..., R]]
     priority: int
 
     def __init__(
         self,
         events: List[Type[BaseEvent]],
+        handler: Optional[Union[Callable[..., Awaitable[R]], Callable[..., R]]] = None,
         providers: Optional[List[Union[Provider, Type[Provider]]]] = None,
         auxiliaries: Optional[List[BaseAuxiliary]] = None,
         priority: int = 15,
-        handler: Optional[Callable[..., Any]] = None,
+        block: bool = False,
     ):
         self.target = set(events)
         super().__init__(AuxType.judge)
         self.providers = providers or []
         self.auxiliaries = auxiliaries or []
         self.priority = priority
         self.handler = handler or (lambda: None)
+        self.block = block
 
     @property
     def scopes(self) -> Set[Scope]:
         return {Scope.prepare}
 
     async def __call__(self, scope: Scope, context: Contexts):
         return type(context["event"]) in self.target
 
     def use(self, func: TCallable) -> TCallable:
         self.handler = func
         return func
 
+    def __aiter__(self) -> _step_iter[R]:
+        return _step_iter(self)
+
 
 class Breakpoint:
     es: EventSystem
     publisher: BackendPublisher
 
     def __init__(self, event_system: EventSystem):
         self.es = event_system
         self.publisher = BackendPublisher("builtin.breakpoint")
-        self.es.add_publisher(self.publisher)
 
     async def wait(
         self,
-        condition: StepOut,
+        condition: StepOut[R],
         timeout: float = 0.0,
-    ):
+    ) -> R:
         fut = self.es.loop.create_future()
 
         for et in condition.target:
             callable_target = self.new_target(et, condition, fut)  # type: ignore
-            self.es.register(
+            self.es.on(
                 et,  # type: ignore
                 priority=condition.priority,
                 auxiliaries=[condition],
                 publisher=self.publisher,
             )(callable_target)
 
         try:
+            self.es.add_publisher(self.publisher)
             return await asyncio.wait_for(fut, timeout) if timeout else await fut
         except asyncio.TimeoutError:
             return None
         finally:
             if not fut.done():
                 self.publisher.subscribers.clear()
+            self.es.publishers.pop(self.publisher.id)
 
     def new_target(self, event_t: Type[BaseEvent], condition: StepOut, fut: Future):
 
-        sub = self.es.register(
+        sub = self.es.on(
             event_t,  # type: ignore
             priority=condition.priority,
             auxiliaries=condition.auxiliaries,
             providers=condition.providers,
             publisher=self.publisher,
         )(condition.handler)
         self.publisher.remove_subscriber(event_t, sub)  # type: ignore
@@ -92,13 +121,14 @@
         async def inner(event: event_t):
             if fut.done():
                 return False
 
             result = await depend_handler(sub, event)
             if result is not None and not fut.done():
                 fut.set_result(result)
-                raise PropagationCancelled()
+                if condition.block:
+                    raise PropagationCancelled()
 
         return inner
 
-    def __call__(self, condition: StepOut, timeout: float = 0.0):
+    def __call__(self, condition: StepOut[R], timeout: float = 0.0) -> Awaitable[R]:
         return self.wait(condition, timeout)
```

### Comparing `arclet-letoderea-0.4.4/arclet/letoderea/builtin/depend.py` & `arclet-letoderea-0.5.0/arclet/letoderea/builtin/depend.py`

 * *Files identical despite different names*

### Comparing `arclet-letoderea-0.4.4/arclet/letoderea/core.py` & `arclet-letoderea-0.5.0/arclet/letoderea/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,26 @@
 
 
 class BackendPublisher(Publisher):
     def validate(self, event: type[BaseEvent]):
         return True
 
 
+async def dispatch(subscribers: list[Subscriber], event: BaseEvent):
+    if not subscribers:
+        return
+    grouped: dict[int, list[Subscriber]] = group_dict(subscribers, lambda x: x.priority)
+    for _, current_subs in sorted(grouped.items(), key=lambda x: x[0]):
+        tasks = [depend_handler(subscriber, event) for subscriber in current_subs]
+        results = await asyncio.gather(*tasks, return_exceptions=True)
+        for result in results:
+            if result.__class__ is PropagationCancelled:
+                return
+
+
 class EventSystem:
     _ref_tasks = set()
     _backend_publisher: Publisher = BackendPublisher("__backend__publisher__")
     loop: asyncio.AbstractEventLoop
     publishers: dict[str, Publisher]
     global_providers: list[Provider]
 
@@ -83,35 +95,23 @@
             pubs.append(pub)
         elif not publisher:
             pubs.extend(
                 pub
                 for pub in self.publishers.values()
                 if pub.validate(event.__class__)  # type: ignore
             )
-            if not pubs:
-                pubs.append(self._backend_publisher)
         else:
             pubs.append(publisher)
-        subscribers = sum((pub.subscribers[event.__class__] for pub in pubs), [])
-        task = self.loop.create_task(self.dispatch(subscribers, event))
+        pubs.append(self._backend_publisher)
+        subscribers = sum((pub.subscribers.get(event.__class__, []) for pub in pubs), [])
+        task = self.loop.create_task(dispatch(subscribers, event))
         task.add_done_callback(self._ref_tasks.discard)
         return task
 
-    async def dispatch(self, subscribers: list[Subscriber], event: BaseEvent):
-        grouped: dict[int, list[Subscriber]] = group_dict(
-            subscribers, lambda x: x.priority
-        )
-        for _, current_subs in sorted(grouped.items(), key=lambda x: x[0]):
-            tasks = [depend_handler(subscriber, event) for subscriber in current_subs]
-            results = await asyncio.gather(*tasks, return_exceptions=True)
-            for result in results:
-                if result is PropagationCancelled:
-                    return
-
-    def register(
+    def on(
         self,
         *events: type[BaseEvent],
         priority: int = 16,
         auxiliaries: list[BaseAuxiliary] | None = None,
         providers: list[Provider | type[Provider]] | None = None,
         publisher: Publisher | None = None,
     ):
@@ -131,23 +131,26 @@
                         ]
                         or [self._backend_publisher]
                     )
                 )
                 for pub in select_pubs:
                     _providers = [
                         *self.global_providers,
-                        *get_providers(event),  # type: ignore
+                        *get_providers(event),
                         *pub.providers.get(event, []),
                         *providers,
                     ]
-                    auxiliaries.extend(get_auxiliaries(event))
+                    _auxiliaries = [
+                        *auxiliaries,
+                        *get_auxiliaries(event)
+                    ]
                     exec_target = Subscriber(
                         exec_target,
                         priority=priority,
-                        auxiliaries=auxiliaries,
+                        auxiliaries=_auxiliaries,
                         providers=_providers,
                     )
                     pub.add_subscriber(event, exec_target)  # type: ignore
 
             return exec_target
 
         return register_wrapper
```

### Comparing `arclet-letoderea-0.4.4/arclet/letoderea/decorate.py` & `arclet-letoderea-0.5.0/arclet/letoderea/decorate.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,20 +28,20 @@
             else:
                 getattr(target, "__auxiliaries__").extend(auxiliaries)
         return target
 
     return wrapper
 
 
-def register(*event: Type[BaseEvent]):
+def subscribe(*event: Type[BaseEvent]):
     es = system_ctx.get()
 
     def wrapper(target: TWrap) -> TWrap:
         if not es:
             return target
         if isinstance(target, Subscriber):
             for e in event:
                 es._backend_publisher.add_subscriber(e, target)  # noqa
             return target
-        return es.register(*event)(target)
+        return es.on(*event)(target)
 
     return wrapper
```

### Comparing `arclet-letoderea-0.4.4/arclet/letoderea/event.py` & `arclet-letoderea-0.5.0/arclet/letoderea/event.py`

 * *Files identical despite different names*

### Comparing `arclet-letoderea-0.4.4/arclet/letoderea/handler.py` & `arclet-letoderea-0.5.0/arclet/letoderea/handler.py`

 * *Files identical despite different names*

### Comparing `arclet-letoderea-0.4.4/arclet/letoderea/provider.py` & `arclet-letoderea-0.5.0/arclet/letoderea/provider.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from __future__ import annotations
 
 from abc import ABCMeta, abstractmethod
 from dataclasses import dataclass
-from typing import Any, Awaitable, Callable, Generic, NamedTuple, TypeVar, get_origin
-from tarina import run_always_await
+from typing import Any, Awaitable, Callable, Generic, NamedTuple, TypeVar, get_args
 
-from .typing import Contexts
+from tarina import generic_issubclass, run_always_await
+from tarina.generic import Unions, get_origin
 
+from .typing import Contexts
 
 T = TypeVar("T")
 
 
 class Param(NamedTuple):
     name: str
     annotation: Any
@@ -32,17 +33,24 @@
         _local_storage[cls] = cls.__orig_bases__[0].__args__[0]  # type: ignore
         if _local_storage[cls] is T:
             raise TypeError(
                 "Subclass of Provider must be generic. If you need a wildcard, please using `typing.Any`"
             )
 
     def validate(self, param: Param):
-        return self.origin == param.annotation or (
-            isinstance(param.annotation, type)
-            and issubclass(param.annotation, get_origin(self.origin) or self.origin)
+        return (
+            self.origin == param.annotation
+            or (
+                isinstance(param.annotation, type)
+                and generic_issubclass(param.annotation, self.origin)
+            )
+            or (
+                get_origin(param.annotation) in Unions
+                and self.origin in get_args(param.annotation)
+            )
         )
 
     @abstractmethod
     async def __call__(self, context: Contexts) -> T | None:
         """
         依据提供模式，从集合中提供一个对象
         """
```

### Comparing `arclet-letoderea-0.4.4/arclet/letoderea/publisher.py` & `arclet-letoderea-0.5.0/arclet/letoderea/publisher.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,16 +68,14 @@
     providers: dict[type[BaseEvent], list[Provider]]
 
     def __init__(self, id_: str, queue_size: int = -1):
         self.id = id_
         self.event_queue = Queue(queue_size)
         self.subscribers = {}
         self.providers = {}
-        if es := system_ctx.get():
-            es.add_publisher(self)
 
     def __repr__(self):
         return f"Publisher::{self.id}"
 
     @abstractmethod
     def validate(self, event: type[BaseEvent]):
         """验证该事件类型是否符合该发布者"""
```

### Comparing `arclet-letoderea-0.4.4/arclet/letoderea/subscriber.py` & `arclet-letoderea-0.5.0/arclet/letoderea/subscriber.py`

 * *Files identical despite different names*

### Comparing `arclet-letoderea-0.4.4/LICENSE` & `arclet-letoderea-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arclet-letoderea-0.4.4/pyproject.toml` & `arclet-letoderea-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "arclet-letoderea"
-version = "0.4.4"
+version = "0.5.0"
 description = "A high-performance, simple-structured event system, relies on asyncio"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
-    "tarina>=0.1.0",
+    "tarina>=0.3.0",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 keywords = [
     "asyncio",
     "event-system",
     "dispatch",
```

### Comparing `arclet-letoderea-0.4.4/README.md` & `arclet-letoderea-0.5.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -23,17 +23,25 @@
 
 class TestEvent:
 
     async def gather(self, context: Contexts):
         context["name"] = "Letoderea"
 
 
-@es.register(TestEvent)
+@es.on(TestEvent)
 async def test_subscriber(name: str):
     print(name)
 
 
 es.loop.run_until_complete(es.publish(TestEvent()))
 ```
 
+## 特性
+
+- 任何实现了 `gather` 方法的类都可以作为事件
+- 通过 `Provider` 实现依赖注入的静态绑定，提高性能
+- 通过 `Contexts` 增强事件传递的灵活性
+- 通过 `Publisher` 实现事件响应的隔离
+- 通过 `Auxiliary` 提供了一系列辅助方法，方便事件的处理
+
 ## 开源协议
 本实现以 MIT 为开源协议。
```

### Comparing `arclet-letoderea-0.4.4/tests/breakpoint.py` & `arclet-letoderea-0.5.0/tests/breakpoint.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,33 +5,32 @@
 
 
 loop = asyncio.get_event_loop()
 es = EventSystem(loop=loop)
 break_point = Breakpoint(es)
 
 
-def handler(msg: str):
+async def handler(msg: str):
     if msg == "continue!":
         print("[breakpoint] <<< receive in handler:", f'"{msg}"')
         return "world!"
 
 
 class ExampleEvent:
     msg: str
 
     async def gather(self, ctx: Contexts):
         ctx['msg'] = self.msg
 
 
-@es.register(ExampleEvent)
+@es.on(ExampleEvent)
 async def test(msg: str):
     if msg == 'hello':
         print("[subscriber] >>> wait for msg: \"continue!\" ")
-        out = StepOut([ExampleEvent])
-        out.use(handler)
+        out = StepOut([ExampleEvent], handler)
         print("[subscriber] >>> current out:", out)
         res = await break_point(out)
         print("[subscriber] >>> wait result:", f'"{res}"')
         print("[subscriber] >>> finish!")
 
 
 a = ExampleEvent()
@@ -52,8 +51,9 @@
             es.publish(c)
         else:
             print(i+1, 'event posted with msg: "continue!"')
             es.publish(b)
         await asyncio.sleep(1)
 
 
+print(es._backend_publisher.subscribers)
 loop.run_until_complete(main())
```

### Comparing `arclet-letoderea-0.4.4/tests/combine.py` & `arclet-letoderea-0.5.0/tests/combine.py`

 * *Files identical despite different names*

### Comparing `arclet-letoderea-0.4.4/tests/condition.py` & `arclet-letoderea-0.5.0/tests/condition.py`

 * *Files 14% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     type: str = "ExampleEvent"
     msg: int = 0
 
     async def gather(self, context: dict):
         context['index'] = self.msg
 
 
-@es.register(ExampleEvent, auxiliaries=[TestTimeLimit(0, 0), Interval(0.2)])
+@es.on(ExampleEvent, auxiliaries=[TestTimeLimit(0, 0), Interval(0.2)])
 async def test(index: int, a: str = "hello", ):
     gc.collect()
     print(index, a)
 
 
 b = ExampleEvent()
```

### Comparing `arclet-letoderea-0.4.4/tests/decorator.py` & `arclet-letoderea-0.5.0/tests/decorator.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     msg: str
 
     async def gather(self, context: dict):
         context['m'] = self.num
         context['a'] = self.msg
 
 
-@es.register(ExampleEvent)
+@es.on(ExampleEvent)
 @bind(TestDecorate())
 async def test(m: int, a: str = TestDecorate()):
     print(m, type(m), end=' ')
     print(a, type(a))
 
 
 async def main():
```

### Comparing `arclet-letoderea-0.4.4/tests/depend.py` & `arclet-letoderea-0.5.0/tests/depend.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     raise ParsingStop
 
 
 def TestDepend() -> bool:
     return Depends(test_depend)
 
 
-@es.register(ExampleEvent)
+@es.on(ExampleEvent)
 def test(m: bool = TestDepend()):
     print(m)
 
 
 async def main():
     try:
         a = ExampleEvent()
```

### Comparing `arclet-letoderea-0.4.4/tests/except.py` & `arclet-letoderea-0.5.0/tests/except.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from __future__ import annotations
 
-from arclet.letoderea import EventSystem, BaseEvent, provide, Contexts, bind, register
+from arclet.letoderea import EventSystem, BaseEvent, provide, Contexts, bind, subscribe
 
 es = EventSystem()
 
 
 class TestEvent(BaseEvent):
     async def gather(self, context: Contexts):
         context["name"] = "Letoderea"
 
 
-@register(TestEvent)
+@subscribe(TestEvent)
 @bind(provide(int, "foo", lambda x: x.get('a')))
 @bind(provide(int, "bar", lambda x: x.get('b')))
 @bind(provide(int, "baz", lambda x: x.get('c')))
 async def test_subscriber(name: str, age: int):
     print(name, age)
```

### Comparing `arclet-letoderea-0.4.4/tests/nest_except.py` & `arclet-letoderea-0.5.0/tests/nest_except.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,19 +17,20 @@
         async def __call__(self, context: Contexts):
             return context.get('a')
 
 
 def wrapper(a: int):  # sourcery skip: raise-specific-error
     return int(a)
 
+
 def wrapper1(a: int = Depend(wrapper)):  # sourcery skip: raise-specific-error
     return int(a)
 
 
-@es.register(ExampleEvent, auxiliaries=[Depend(wrapper)])
+@es.on(ExampleEvent, auxiliaries=[Depend(wrapper)])
 async def handler(a: int = Depend(wrapper1)):
     print(a)
 
 
 async def main():
     await es.publish(ExampleEvent())
```

### Comparing `arclet-letoderea-0.4.4/tests/test_handler.py` & `arclet-letoderea-0.5.0/tests/test_handler.py`

 * *Files identical despite different names*

### Comparing `arclet-letoderea-0.4.4/tests/test_param_parser.py` & `arclet-letoderea-0.5.0/tests/test_param_parser.py`

 * *Files identical despite different names*

### Comparing `arclet-letoderea-0.4.4/tests/test_provider.py` & `arclet-letoderea-0.5.0/tests/test_provider.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         context["name"] = "Letoderea"
 
     class TestProvider(Provider[str]):
         async def __call__(self, context: Contexts) -> str | None:
             return context['name']
 
 
-@es.register(TestEvent)
+@es.on(TestEvent)
 @bind(IntProvider, BoolProvider, FloatProvider)
 async def test_subscriber(
     name0: str,
     age0: int,
     is_true0: bool,
     num0: float,
     name1: str,
```

### Comparing `arclet-letoderea-0.4.4/tests/test_publisher.py` & `arclet-letoderea-0.5.0/tests/test_publisher.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,17 +18,18 @@
 
     def validate(self, event: type[BaseEvent]):
         return event == TestEvent
 
 
 test = provide(str, call=lambda x: x.get("name"))
 my_publisher = MyPublisher("test")
+es.add_publisher(my_publisher)
 my_publisher.unsafe_push(TestEvent("hello world"))
 my_publisher[TestEvent] += test()
 
 
-@es.register(TestEvent)
+@es.on(TestEvent)
 async def test_subscriber(a: str):
     print(a)
 
 
 loop.run_until_complete(asyncio.sleep(0.1))
```

### Comparing `arclet-letoderea-0.4.4/PKG-INFO` & `arclet-letoderea-0.5.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arclet-letoderea
-Version: 0.4.4
+Version: 0.5.0
 Summary: A high-performance, simple-structured event system, relies on asyncio
 License: MIT
 Keywords: asyncio,event-system,dispatch,dependency-injection
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -41,18 +41,26 @@
 
 class TestEvent:
 
     async def gather(self, context: Contexts):
         context["name"] = "Letoderea"
 
 
-@es.register(TestEvent)
+@es.on(TestEvent)
 async def test_subscriber(name: str):
     print(name)
 
 
 es.loop.run_until_complete(es.publish(TestEvent()))
 ```
 
+## 特性
+
+- 任何实现了 `gather` 方法的类都可以作为事件
+- 通过 `Provider` 实现依赖注入的静态绑定，提高性能
+- 通过 `Contexts` 增强事件传递的灵活性
+- 通过 `Publisher` 实现事件响应的隔离
+- 通过 `Auxiliary` 提供了一系列辅助方法，方便事件的处理
+
 ## 开源协议
 本实现以 MIT 为开源协议。
```

