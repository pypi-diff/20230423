# Comparing `tmp/anyioc-0.9.0.tar.gz` & `tmp/anyioc-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/anyioc-0.9.0.tar", last modified: Wed Jul  1 06:14:17 2020, max compression
+gzip compressed data, was "dist/anyioc-0.9.1.tar", last modified: Sat Jul  4 07:34:14 2020, max compression
```

## Comparing `anyioc-0.9.0.tar` & `anyioc-0.9.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-01 06:14:17.000000 anyioc-0.9.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4697 2020-07-01 06:14:17.000000 anyioc-0.9.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     3269 2020-07-01 06:13:53.000000 anyioc-0.9.0/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-01 06:14:17.000000 anyioc-0.9.0/anyioc/
--rw-rw-r--   0 travis    (2000) travis    (2000)      185 2020-07-01 06:13:53.000000 anyioc-0.9.0/anyioc/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6507 2020-07-01 06:13:53.000000 anyioc-0.9.0/anyioc/builder.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      558 2020-07-01 06:13:53.000000 anyioc-0.9.0/anyioc/err.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2669 2020-07-01 06:13:53.000000 anyioc-0.9.0/anyioc/g.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7767 2020-07-01 06:13:53.000000 anyioc-0.9.0/anyioc/ioc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5782 2020-07-01 06:13:53.000000 anyioc-0.9.0/anyioc/ioc_resolver.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4150 2020-07-01 06:13:53.000000 anyioc-0.9.0/anyioc/ioc_service_info.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1064 2020-07-01 06:13:53.000000 anyioc-0.9.0/anyioc/ioc_services.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1406 2020-07-01 06:13:53.000000 anyioc-0.9.0/anyioc/symbols.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6760 2020-07-01 06:13:53.000000 anyioc-0.9.0/anyioc/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-01 06:14:17.000000 anyioc-0.9.0/anyioc.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4697 2020-07-01 06:14:17.000000 anyioc-0.9.0/anyioc.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      351 2020-07-01 06:14:17.000000 anyioc-0.9.0/anyioc.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-07-01 06:14:17.000000 anyioc-0.9.0/anyioc.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-07-01 06:14:17.000000 anyioc-0.9.0/anyioc.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)        7 2020-07-01 06:14:17.000000 anyioc-0.9.0/anyioc.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2020-07-01 06:14:17.000000 anyioc-0.9.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      180 2020-07-01 06:13:53.000000 anyioc-0.9.0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-04 07:34:14.000000 anyioc-0.9.1/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4697 2020-07-04 07:34:14.000000 anyioc-0.9.1/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3269 2020-07-04 07:33:50.000000 anyioc-0.9.1/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-04 07:34:14.000000 anyioc-0.9.1/anyioc/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      185 2020-07-04 07:33:50.000000 anyioc-0.9.1/anyioc/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6227 2020-07-04 07:33:50.000000 anyioc-0.9.1/anyioc/builder.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      558 2020-07-04 07:33:50.000000 anyioc-0.9.1/anyioc/err.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2669 2020-07-04 07:33:50.000000 anyioc-0.9.1/anyioc/g.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7731 2020-07-04 07:33:50.000000 anyioc-0.9.1/anyioc/ioc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5782 2020-07-04 07:33:50.000000 anyioc-0.9.1/anyioc/ioc_resolver.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4462 2020-07-04 07:33:50.000000 anyioc-0.9.1/anyioc/ioc_service_info.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1064 2020-07-04 07:33:50.000000 anyioc-0.9.1/anyioc/ioc_services.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1049 2020-07-04 07:33:50.000000 anyioc-0.9.1/anyioc/symbols.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6852 2020-07-04 07:33:50.000000 anyioc-0.9.1/anyioc/utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-04 07:34:14.000000 anyioc-0.9.1/anyioc.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4697 2020-07-04 07:34:14.000000 anyioc-0.9.1/anyioc.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      351 2020-07-04 07:34:14.000000 anyioc-0.9.1/anyioc.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-07-04 07:34:14.000000 anyioc-0.9.1/anyioc.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-07-04 07:34:14.000000 anyioc-0.9.1/anyioc.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)        7 2020-07-04 07:34:14.000000 anyioc-0.9.1/anyioc.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2020-07-04 07:34:14.000000 anyioc-0.9.1/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)      180 2020-07-04 07:33:50.000000 anyioc-0.9.1/setup.py
```

### Comparing `anyioc-0.9.0/PKG-INFO` & `anyioc-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anyioc
-Version: 0.9.0
+Version: 0.9.1
 Summary: UNKNOWN
 Home-page: https://github.com/Cologler/anyioc-python
 License: MIT License
 Description: # anyioc
         
         ![GitHub](https://img.shields.io/github/license/Cologler/anyioc-python.svg)
         [![Build Status](https://travis-ci.com/Cologler/anyioc-python.svg?branch=master)](https://travis-ci.com/Cologler/anyioc-python)
```

### Comparing `anyioc-0.9.0/README.md` & `anyioc-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `anyioc-0.9.0/anyioc/builder.py` & `anyioc-0.9.1/anyioc/builder.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,31 +3,34 @@
 # Copyright (c) 2019~2999 - Cologler <skyoflw@gmail.com>
 # ----------
 #
 # ----------
 
 from .ioc import ScopedServiceProvider, LifeTime
 from .symbols import Symbols, _Symbol
+from .utils import inject_by_anno, inject_by_name
+
+inject_by_table = {
+    'anno': inject_by_anno,
+    'inject_by_anno': inject_by_anno,
+    'name': inject_by_name,
+    'inject_by_name': inject_by_name
+}
 
 class ServiceProviderBuilder:
     '''
-    the high level register API for `ServiceProvider`.
+    provide decorator api for `ServiceProvider`.
     '''
-    __slots__ = ('_provider', '_last_added_key')
+    __slots__ = ('_provider')
 
     def __init__(self, provider: ScopedServiceProvider):
         self._provider = provider
-        self._last_added_key = None
-
-    @property
-    def last_added_key(self):
-        return self._last_added_key
 
     def _on_key_added(self, key):
-        self._last_added_key = key
+        pass
 
     def register(self, lifetime: LifeTime, key=None, factory=None, *, inject_by=None):
         '''
         register a service factory by key.
 
         `factory` accept a function which require one or zero parameter.
         if the count of parameter is 1, pass a `IServiceProvider` as the argument.
@@ -42,14 +45,20 @@
 
         returns:
 
         - decorator return the factory.
         - non-decorator always return None
         '''
 
+        if isinstance(inject_by, str):
+            if inject_by in inject_by_table:
+                inject_by = inject_by_table[inject_by]
+            else:
+                raise ValueError(f'{inject_by} is not one of known `inject by` action.')
+
         def decorator(func):
             aliases = ()
             if key is None:
                 safe_key = func
             elif isinstance(key, list):
                 if not key:
                     raise ValueError('cannot use empty list as key list')
@@ -132,53 +141,40 @@
         returns:
 
         - decorator return the factory.
         - non-decorator always return None
         '''
         return self.register(LifeTime.transient, key, factory, inject_by=inject_by)
 
-    def value(self, key, *value):
+    def value(self, key):
         '''
-        register a value by key.
-
-        this function can use like a decorator if only have 1 arguments.
-
-        if `key` is `None`, use a new `object()` as key.
-        you can get the generated new key by access `ServiceProviderBuilder.last_added_key`.
-
-        return the value.
+        get a decorator that use to register a singleton value by key.
         '''
-        if len(value) > 1:
-            raise TypeError(f'takes 1 or 2 arguments but {len(value)+1} was given')
 
         def decorator(value):
-            safe_key = key if key is not None else object()
-            self._provider.register_value(safe_key, value)
-            self._on_key_added(safe_key)
+            self._provider.register_value(key, value)
+            self._on_key_added(key)
             return value
 
-        return decorator(value[0]) if value else decorator
+        return decorator
 
-    def group(self, group_key=None):
+    def group(self, *keys):
         '''
-        add a new group into `ServiceProvider` by key `group_key`.
-
-        if `group_key` is `None`, use return value as key.
+        add a new group into `ServiceProvider` by keys,
+        return a group scoped `ServiceProviderBuilder` to build sub services.
 
-        return a `Group` instance as the unique key.
+        the return instance can also use like a unique key.
         '''
         from .utils import make_group
 
         group = Group(self._provider)
         self._provider.register_group(group, group)
         self._on_key_added(group)
-        if group_key is not None:
-            self._provider.register_bind(group_key, group)
-            sym = Symbols.get_symbol_for_group_src(group_key)
-            self._provider.register_value(sym, group)
+        for k in keys:
+            self._provider.register_bind(k, group)
         return group
 
 
 class Group(ServiceProviderBuilder):
     '''
     a `Group` class use for build `ServiceProvider` and use as unique group key.
     '''
```

### Comparing `anyioc-0.9.0/anyioc/err.py` & `anyioc-0.9.1/anyioc/err.py`

 * *Files identical despite different names*

### Comparing `anyioc-0.9.0/anyioc/g.py` & `anyioc-0.9.1/anyioc/g.py`

 * *Files identical despite different names*

### Comparing `anyioc-0.9.0/anyioc/ioc.py` & `anyioc-0.9.1/anyioc/ioc.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from .ioc_services import ServicesMap
 from .ioc_resolver import IServiceInfoResolver, ServiceInfoChainResolver
 from .ioc_service_info import (
     LifeTime,
     IServiceInfo,
     ServiceInfo,
     ProviderServiceInfo,
+    GetAttrServiceInfo,
     ValueServiceInfo,
     GroupedServiceInfo,
     BindedServiceInfo,
     CallerFrameServiceInfo
 )
 
 
@@ -47,19 +48,20 @@
         create a scoped service provider for get scoped services.
         '''
         raise NotImplementedError
 
 
 class ScopedServiceProvider(IServiceProvider):
 
-    def __init__(self, services: ServicesMap):
+    def __init__(self, services: ServicesMap, parent=None):
         super().__init__()
         self._services = services
         self._exit_stack = None
-        self._services[Symbols.cache] = ValueServiceInfo({})
+        self._scoped_cache = {}
+        self._parent = parent
         self.__class__ = ServiceProvider # hack
 
     def _get_service_info(self, key) -> IServiceInfo:
         try:
             return self._services[key]
         except KeyError:
             pass
@@ -191,16 +193,14 @@
         provider.register_value('int', 1)
         provider.register_group('any', ['str', 'int'])
         assert provider['any'] == ('name', 1)
         ```
 
         equals `register_transient(key, lambda ioc: tuple(ioc[k] for k in keys))`
         '''
-        sym = Symbols.get_symbol_for_group_src(key)
-        self.register_value(sym, keys)
         return self.register_service_info(key, GroupedServiceInfo(keys))
 
     def register_bind(self, new_key, target_key):
         '''
         bind `new_key` to `target_key` so
         you can use `new_key` as key to get value from service provider.
 
@@ -208,23 +208,22 @@
         '''
         return self.register_service_info(new_key, BindedServiceInfo(target_key))
 
     def scope(self):
         '''
         create a scoped service provider.
         '''
-        sp = ScopedServiceProvider(self._services.scope())
+        sp = ScopedServiceProvider(self._services.scope(), self)
         self.enter(sp)
-        sp.register_value(Symbols.provider_parent, self)
         return sp
 
     @property
     def builder(self):
         '''
-        get a new `ServiceProviderBuilder` for use high level api for this `ServiceProvider`.
+        get a new `ServiceProviderBuilder` wrapper for this `ServiceProvider`.
         '''
         from .builder import ServiceProviderBuilder
         return ServiceProviderBuilder(self)
 
 
 class ServiceProvider(ScopedServiceProvider):
     '''
@@ -232,15 +231,16 @@
     '''
 
     def __init__(self):
         super().__init__(ServicesMap())
         provider_service_info = ProviderServiceInfo()
         self._services[Symbols.provider] = provider_service_info
         self._services[Symbols.provider_root] = ValueServiceInfo(self)
-        self._services[Symbols.provider_parent] = ValueServiceInfo(None)
+        self._services[Symbols.provider_parent] = GetAttrServiceInfo('_parent')
+        self._services[Symbols.cache] = GetAttrServiceInfo('_scoped_cache')
         self._services[Symbols.missing_resolver] = ValueServiceInfo(ServiceInfoChainResolver())
         self._services[Symbols.caller_frame] = CallerFrameServiceInfo()
         # service alias
         self._services['ioc'] = provider_service_info
         self._services['provider'] = provider_service_info
         self._services['service_provider'] = provider_service_info
         self._services[ServiceProvider] = provider_service_info
```

### Comparing `anyioc-0.9.0/anyioc/ioc_resolver.py` & `anyioc-0.9.1/anyioc/ioc_resolver.py`

 * *Files identical despite different names*

### Comparing `anyioc-0.9.0/anyioc/ioc_service_info.py` & `anyioc-0.9.1/anyioc/ioc_service_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -106,14 +106,27 @@
 
     __slots__ = ()
 
     def get(self, provider):
         return provider
 
 
+class GetAttrServiceInfo(IServiceInfo):
+    '''getattr from current `ServiceProvider`.'''
+
+    __slots__ = ('_attr_info')
+
+    def __init__(self, *attr_info: tuple):
+        super().__init__()
+        self._attr_info = attr_info
+
+    def get(self, provider):
+        return getattr(provider, *self._attr_info)
+
+
 class ValueServiceInfo(IServiceInfo):
     '''a `IServiceInfo` use for get fixed value.'''
 
     __slots__ = ('_value')
 
     def __init__(self, value):
         self._value = value
```

### Comparing `anyioc-0.9.0/anyioc/ioc_services.py` & `anyioc-0.9.1/anyioc/ioc_services.py`

 * *Files identical despite different names*

### Comparing `anyioc-0.9.0/anyioc/symbols.py` & `anyioc-0.9.1/anyioc/symbols.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,19 +42,7 @@
     cache = _Symbol('cache')
 
     # the missing resolver from `IServiceProvider`
     missing_resolver = _Symbol('missing_resolver')
 
     # get frame info of caller
     caller_frame = _Symbol('caller_frame')
-
-    # the named group tag for builder
-    _group_src_tag = _Symbol('_group_src_tag')
-
-    @classmethod
-    def get_symbol_for_group_src(cls, group):
-        '''
-        get a symbol for get group source from `ServiceProvider`.
-
-        this may change after anyioc update (include return value type).
-        '''
-        return (cls._group_src_tag, group)
```

### Comparing `anyioc-0.9.0/anyioc/utils.py` & `anyioc-0.9.1/anyioc/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -225,13 +225,17 @@
     ```
     '''
     import logging
     import inspect
     from .symbols import Symbols
 
     fr = ioc[Symbols.caller_frame]
-    mo = inspect.getmodule(fr.frame)
-    return logging.getLogger(mo.__name__)
+    if fr.filename == '<stdin>':
+        name = '<stdin>'
+    else:
+        mo = inspect.getmodule(fr.frame)
+        name = mo.__name__
+    return logging.getLogger(name)
 
 # keep old func names:
 
 auto_inject = inject_by_name
```

### Comparing `anyioc-0.9.0/anyioc.egg-info/PKG-INFO` & `anyioc-0.9.1/anyioc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anyioc
-Version: 0.9.0
+Version: 0.9.1
 Summary: UNKNOWN
 Home-page: https://github.com/Cologler/anyioc-python
 License: MIT License
 Description: # anyioc
         
         ![GitHub](https://img.shields.io/github/license/Cologler/anyioc-python.svg)
         [![Build Status](https://travis-ci.com/Cologler/anyioc-python.svg?branch=master)](https://travis-ci.com/Cologler/anyioc-python)
```

