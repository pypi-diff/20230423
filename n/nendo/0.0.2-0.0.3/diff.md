# Comparing `tmp/nendo-0.0.2.tar.gz` & `tmp/nendo-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nendo-0.0.2.tar", max compression
+gzip compressed data, was "nendo-0.0.3.tar", max compression
```

## Comparing `nendo-0.0.2.tar` & `nendo-0.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1073 2023-03-27 20:51:34.595817 nendo-0.0.2/LICENSE
--rw-r--r--   0        0        0     3160 2023-04-23 00:48:26.855126 nendo-0.0.2/README.md
--rw-r--r--   0        0        0     1319 2023-04-23 10:18:55.315019 nendo-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      465 2023-04-23 00:06:26.661112 nendo-0.0.2/src/nendo/__init__.py
--rw-r--r--   0        0        0      547 2023-04-22 23:11:10.596093 nendo-0.0.2/src/nendo/config.py
--rw-r--r--   0        0        0     2130 2023-04-23 00:05:55.439112 nendo-0.0.2/src/nendo/core.py
--rw-r--r--   0        0        0     6486 2023-04-23 10:05:12.928015 nendo-0.0.2/src/nendo/schema.py
--rw-r--r--   0        0        0      209 2023-04-22 23:57:14.679109 nendo-0.0.2/src/nendo/utils.py
--rw-r--r--   0        0        0     4382 1970-01-01 00:00:00.000000 nendo-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-03-27 20:51:34.595817 nendo-0.0.3/LICENSE
+-rw-r--r--   0        0        0     3160 2023-04-23 00:48:26.855126 nendo-0.0.3/README.md
+-rw-r--r--   0        0        0     1319 2023-04-23 10:34:49.069025 nendo-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      465 2023-04-23 00:06:26.661112 nendo-0.0.3/src/nendo/__init__.py
+-rw-r--r--   0        0        0      547 2023-04-22 23:11:10.596093 nendo-0.0.3/src/nendo/config.py
+-rw-r--r--   0        0        0     2130 2023-04-23 00:05:55.439112 nendo-0.0.3/src/nendo/core.py
+-rw-r--r--   0        0        0     6487 2023-04-23 10:36:49.360026 nendo-0.0.3/src/nendo/schema.py
+-rw-r--r--   0        0        0      209 2023-04-22 23:57:14.679109 nendo-0.0.3/src/nendo/utils.py
+-rw-r--r--   0        0        0     4382 1970-01-01 00:00:00.000000 nendo-0.0.3/PKG-INFO
```

### Comparing `nendo-0.0.2/LICENSE` & `nendo-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nendo-0.0.2/README.md` & `nendo-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `nendo-0.0.2/pyproject.toml` & `nendo-0.0.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nendo"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   "Felix Lorenz <felix@okio.ai>",
   "Samim Winiger <samim@okio.ai>"
 ]
 description = "The nendo generative audio framework."
 license = "MIT"
 readme = "README.md"
```

### Comparing `nendo-0.0.2/src/nendo/config.py` & `nendo-0.0.3/src/nendo/config.py`

 * *Files identical despite different names*

### Comparing `nendo-0.0.2/src/nendo/core.py` & `nendo-0.0.3/src/nendo/core.py`

 * *Files identical despite different names*

### Comparing `nendo-0.0.2/src/nendo/schema.py` & `nendo-0.0.3/src/nendo/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,8 +171,8 @@
     # lifecycle hooks: init, run, destroy
     # 3rd Party API integration
     # compute integration
         
     def __str__(self) -> str:
         """Get a string representation of the object for printing."""
         cls_name = f"\033[1m{self.__class__.__name__}\033[0m"
-        return f"{cls_name}\nType: {self.type}"
+        return f"{cls_name} | type: {self.type}"
```

### Comparing `nendo-0.0.2/PKG-INFO` & `nendo-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nendo
-Version: 0.0.2
+Version: 0.0.3
 Summary: The nendo generative audio framework.
 Home-page: https://nendo.ai
 License: MIT
 Keywords: AI,generative,music,okio,composition,music production,music generation,music information retrieval,MIR,music analysis,song analysis
 Author: Felix Lorenz
 Author-email: felix@okio.ai
 Requires-Python: >=3.8,<3.11
```

