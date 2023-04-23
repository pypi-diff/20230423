# Comparing `tmp/bevy-2.0.0b2.tar.gz` & `tmp/bevy-2.0.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bevy-2.0.0b2.tar", max compression
+gzip compressed data, was "bevy-2.0.0b4.tar", max compression
```

## Comparing `bevy-2.0.0b2.tar` & `bevy-2.0.0b4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1076 2023-04-17 00:09:47.133909 bevy-2.0.0b2/LICENSE
--rw-r--r--   0        0        0     5859 2023-04-17 00:09:47.133909 bevy-2.0.0b2/README.md
--rw-r--r--   0        0        0      208 2023-04-17 00:09:47.133909 bevy-2.0.0b2/bevy/__init__.py
--rw-r--r--   0        0        0     1463 2023-04-17 00:09:47.133909 bevy-2.0.0b2/bevy/contextvar.py
--rw-r--r--   0        0        0     1692 2023-04-17 00:09:47.133909 bevy-2.0.0b2/bevy/injectors/classes.py
--rw-r--r--   0        0        0     2244 2023-04-17 00:09:47.133909 bevy-2.0.0b2/bevy/injectors/functions.py
--rw-r--r--   0        0        0     2717 2023-04-17 00:09:47.133909 bevy-2.0.0b2/bevy/options.py
--rw-r--r--   0        0        0      164 2023-04-17 00:09:47.133909 bevy-2.0.0b2/bevy/providers/__init__.py
--rw-r--r--   0        0        0     1537 2023-04-17 00:09:47.133909 bevy-2.0.0b2/bevy/providers/annotated_provider.py
--rw-r--r--   0        0        0     3488 2023-04-17 00:09:47.133909 bevy-2.0.0b2/bevy/providers/base.py
--rw-r--r--   0        0        0     1143 2023-04-17 00:09:47.133909 bevy-2.0.0b2/bevy/providers/type_provider.py
--rw-r--r--   0        0        0     5950 2023-04-17 00:09:47.133909 bevy-2.0.0b2/bevy/repository.py
--rw-r--r--   0        0        0      866 2023-04-17 00:09:47.133909 bevy-2.0.0b2/pyproject.toml
--rw-r--r--   0        0        0     6698 1970-01-01 00:00:00.000000 bevy-2.0.0b2/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-04-23 20:31:40.040469 bevy-2.0.0b4/LICENSE
+-rw-r--r--   0        0        0     5859 2023-04-23 20:31:40.040469 bevy-2.0.0b4/README.md
+-rw-r--r--   0        0        0      213 2023-04-23 20:31:40.040469 bevy-2.0.0b4/bevy/__init__.py
+-rw-r--r--   0        0        0     1463 2023-04-23 20:31:40.040469 bevy-2.0.0b4/bevy/contextvar.py
+-rw-r--r--   0        0        0     1692 2023-04-23 20:31:40.040469 bevy-2.0.0b4/bevy/injectors/classes.py
+-rw-r--r--   0        0        0     2244 2023-04-23 20:31:40.040469 bevy-2.0.0b4/bevy/injectors/functions.py
+-rw-r--r--   0        0        0     2717 2023-04-23 20:31:40.040469 bevy-2.0.0b4/bevy/options.py
+-rw-r--r--   0        0        0      164 2023-04-23 20:31:40.040469 bevy-2.0.0b4/bevy/providers/__init__.py
+-rw-r--r--   0        0        0     1537 2023-04-23 20:31:40.040469 bevy-2.0.0b4/bevy/providers/annotated_provider.py
+-rw-r--r--   0        0        0     3488 2023-04-23 20:31:40.040469 bevy-2.0.0b4/bevy/providers/base.py
+-rw-r--r--   0        0        0     1143 2023-04-23 20:31:40.040469 bevy-2.0.0b4/bevy/providers/type_provider.py
+-rw-r--r--   0        0        0     6003 2023-04-23 20:31:40.040469 bevy-2.0.0b4/bevy/repository.py
+-rw-r--r--   0        0        0      866 2023-04-23 20:31:40.044469 bevy-2.0.0b4/pyproject.toml
+-rw-r--r--   0        0        0     6698 1970-01-01 00:00:00.000000 bevy-2.0.0b4/PKG-INFO
```

### Comparing `bevy-2.0.0b2/LICENSE` & `bevy-2.0.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `bevy-2.0.0b2/README.md` & `bevy-2.0.0b4/README.md`

 * *Files identical despite different names*

### Comparing `bevy-2.0.0b2/bevy/contextvar.py` & `bevy-2.0.0b4/bevy/contextvar.py`

 * *Files identical despite different names*

### Comparing `bevy-2.0.0b2/bevy/injectors/classes.py` & `bevy-2.0.0b4/bevy/injectors/classes.py`

 * *Files identical despite different names*

### Comparing `bevy-2.0.0b2/bevy/injectors/functions.py` & `bevy-2.0.0b4/bevy/injectors/functions.py`

 * *Files identical despite different names*

### Comparing `bevy-2.0.0b2/bevy/options.py` & `bevy-2.0.0b4/bevy/options.py`

 * *Files identical despite different names*

### Comparing `bevy-2.0.0b2/bevy/providers/annotated_provider.py` & `bevy-2.0.0b4/bevy/providers/annotated_provider.py`

 * *Files identical despite different names*

### Comparing `bevy-2.0.0b2/bevy/providers/base.py` & `bevy-2.0.0b4/bevy/providers/base.py`

 * *Files identical despite different names*

### Comparing `bevy-2.0.0b2/bevy/providers/type_provider.py` & `bevy-2.0.0b4/bevy/providers/type_provider.py`

 * *Files identical despite different names*

### Comparing `bevy-2.0.0b2/bevy/repository.py` & `bevy-2.0.0b4/bevy/repository.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,20 +39,23 @@
 
     _bevy_repository: "_ContextVarDefaultFactory[Repository[_K, _V]]" = (
         _ContextVarDefaultFactory("bevy_context", default=lambda: Repository.factory())
     )
 
     def __init__(self, parent: "Repository | None" = None):
         self._parent = parent or _NullRepository()
-        self._providers: list[Provider[_K, _V]] = []
+        self._providers: tuple[Provider[_K, _V]] = []
 
     def add_providers(self, *providers: Type[Provider[_K, _V]]):
         """Creates providers and adds them to the repository. These providers will be used to lookup and create
         instances that will be stored and returned by the repository."""
-        self._providers.extend(provider(self) for provider in providers)
+        self._providers = (
+            *(provider(self) for provider in providers),
+            *self._providers,
+        )
 
     def branch(self) -> "Repository[_K, _V]":
         branch = type(self)(self)
 
         providers = (provider.get_clone_factory() for provider in self._providers)
         branch.add_providers(*providers)
```

### Comparing `bevy-2.0.0b2/pyproject.toml` & `bevy-2.0.0b4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Bevy"
-version = "2.0.0b2"
+version = "2.0.0b4"
 description = "Python Dependency Inversion made simple so you can focus on creating amazing code."
 authors = ["Zech Zimmerman <hi@zech.codes>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/ZechCodes/Bevy"
 repository = "https://github.com/ZechCodes/Bevy"
 documentation = "https://github.com/ZechCodes/Bevy/blob/master/README.md"
```

### Comparing `bevy-2.0.0b2/PKG-INFO` & `bevy-2.0.0b4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bevy
-Version: 2.0.0b2
+Version: 2.0.0b4
 Summary: Python Dependency Inversion made simple so you can focus on creating amazing code.
 Home-page: https://github.com/ZechCodes/Bevy
 License: MIT
 Keywords: dependency,injection,annotations,types
 Author: Zech Zimmerman
 Author-email: hi@zech.codes
 Requires-Python: >=3.10,<4.0
```

