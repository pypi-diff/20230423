# Comparing `tmp/cppython-cmake-0.1.1.dev15.tar.gz` & `tmp/cppython-cmake-0.1.1.dev16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cppython-cmake-0.1.1.dev15.tar", last modified: Mon Mar 20 22:55:26 2023, max compression
+gzip compressed data, was "cppython-cmake-0.1.1.dev16.tar", last modified: Sun Apr 23 03:14:46 2023, max compression
```

## Comparing `cppython-cmake-0.1.1.dev15.tar` & `cppython-cmake-0.1.1.dev16.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1070 2023-03-20 22:55:05.200986 cppython-cmake-0.1.1.dev15/LICENSE.md
--rw-r--r--   0        0        0       93 2023-03-20 22:55:05.200986 cppython-cmake-0.1.1.dev15/README.md
--rw-r--r--   0        0        0        3 2023-03-20 22:55:05.200986 cppython-cmake-0.1.1.dev15/cppython_cmake/__init__.py
--rw-r--r--   0        0        0     3520 2023-03-20 22:55:05.200986 cppython-cmake-0.1.1.dev15/cppython_cmake/builder.py
--rw-r--r--   0        0        0     2286 2023-03-20 22:55:05.200986 cppython-cmake-0.1.1.dev15/cppython_cmake/plugin.py
--rw-r--r--   0        0        0        0 2023-03-20 22:55:05.200986 cppython-cmake-0.1.1.dev15/cppython_cmake/py.typed
--rw-r--r--   0        0        0      805 2023-03-20 22:55:05.200986 cppython-cmake-0.1.1.dev15/cppython_cmake/resolution.py
--rw-r--r--   0        0        0     3754 2023-03-20 22:55:05.200986 cppython-cmake-0.1.1.dev15/cppython_cmake/schema.py
--rw-r--r--   0        0        0     2406 2023-03-20 22:55:05.200986 cppython-cmake-0.1.1.dev15/pyproject.toml
--rw-r--r--   0        0        0        3 2023-03-20 22:55:05.200986 cppython-cmake-0.1.1.dev15/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-03-20 22:55:05.200986 cppython-cmake-0.1.1.dev15/tests/data/default/CMakePresets.json
--rw-r--r--   0        0        0        3 2023-03-20 22:55:05.200986 cppython-cmake-0.1.1.dev15/tests/integration/__init__.py
--rw-r--r--   0        0        0      849 2023-03-20 22:55:05.200986 cppython-cmake-0.1.1.dev15/tests/integration/test_generator.py
--rw-r--r--   0        0        0        3 2023-03-20 22:55:05.200986 cppython-cmake-0.1.1.dev15/tests/unit/__init__.py
--rw-r--r--   0        0        0     4773 2023-03-20 22:55:05.200986 cppython-cmake-0.1.1.dev15/tests/unit/test_generator.py
--rw-r--r--   0        0        0      523 1970-01-01 00:00:00.000000 cppython-cmake-0.1.1.dev15/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-23 03:14:27.814786 cppython-cmake-0.1.1.dev16/LICENSE.md
+-rw-r--r--   0        0        0       93 2023-04-23 03:14:27.814786 cppython-cmake-0.1.1.dev16/README.md
+-rw-r--r--   0        0        0        3 2023-04-23 03:14:27.814786 cppython-cmake-0.1.1.dev16/cppython_cmake/__init__.py
+-rw-r--r--   0        0        0     3520 2023-04-23 03:14:27.814786 cppython-cmake-0.1.1.dev16/cppython_cmake/builder.py
+-rw-r--r--   0        0        0     2286 2023-04-23 03:14:27.814786 cppython-cmake-0.1.1.dev16/cppython_cmake/plugin.py
+-rw-r--r--   0        0        0        0 2023-04-23 03:14:27.814786 cppython-cmake-0.1.1.dev16/cppython_cmake/py.typed
+-rw-r--r--   0        0        0      805 2023-04-23 03:14:27.814786 cppython-cmake-0.1.1.dev16/cppython_cmake/resolution.py
+-rw-r--r--   0        0        0     3754 2023-04-23 03:14:27.814786 cppython-cmake-0.1.1.dev16/cppython_cmake/schema.py
+-rw-r--r--   0        0        0     2406 2023-04-23 03:14:27.814786 cppython-cmake-0.1.1.dev16/pyproject.toml
+-rw-r--r--   0        0        0        3 2023-04-23 03:14:27.814786 cppython-cmake-0.1.1.dev16/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-23 03:14:27.814786 cppython-cmake-0.1.1.dev16/tests/data/default/CMakePresets.json
+-rw-r--r--   0        0        0        3 2023-04-23 03:14:27.814786 cppython-cmake-0.1.1.dev16/tests/integration/__init__.py
+-rw-r--r--   0        0        0      849 2023-04-23 03:14:27.814786 cppython-cmake-0.1.1.dev16/tests/integration/test_generator.py
+-rw-r--r--   0        0        0        3 2023-04-23 03:14:27.814786 cppython-cmake-0.1.1.dev16/tests/unit/__init__.py
+-rw-r--r--   0        0        0     4773 2023-04-23 03:14:27.814786 cppython-cmake-0.1.1.dev16/tests/unit/test_generator.py
+-rw-r--r--   0        0        0      523 1970-01-01 00:00:00.000000 cppython-cmake-0.1.1.dev16/PKG-INFO
```

### Comparing `cppython-cmake-0.1.1.dev15/LICENSE.md` & `cppython-cmake-0.1.1.dev16/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cppython-cmake-0.1.1.dev15/cppython_cmake/builder.py` & `cppython-cmake-0.1.1.dev16/cppython_cmake/builder.py`

 * *Files identical despite different names*

### Comparing `cppython-cmake-0.1.1.dev15/cppython_cmake/plugin.py` & `cppython-cmake-0.1.1.dev16/cppython_cmake/plugin.py`

 * *Files identical despite different names*

### Comparing `cppython-cmake-0.1.1.dev15/cppython_cmake/resolution.py` & `cppython-cmake-0.1.1.dev16/cppython_cmake/resolution.py`

 * *Files identical despite different names*

### Comparing `cppython-cmake-0.1.1.dev15/cppython_cmake/schema.py` & `cppython-cmake-0.1.1.dev16/cppython_cmake/schema.py`

 * *Files identical despite different names*

### Comparing `cppython-cmake-0.1.1.dev15/pyproject.toml` & `cppython-cmake-0.1.1.dev16/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 readme = "README.md"
 dynamic = []
 requires-python = ">=3.11"
 dependencies = [
     "cppython-core>=0.3.3.dev0",
     "cmake>=3.24.1",
 ]
-version = "0.1.1.dev15"
+version = "0.1.1.dev16"
 
 [project.license-files]
 paths = [
     "LICENSE.md",
 ]
 
 [project.urls]
```

### Comparing `cppython-cmake-0.1.1.dev15/tests/integration/test_generator.py` & `cppython-cmake-0.1.1.dev16/tests/integration/test_generator.py`

 * *Files identical despite different names*

### Comparing `cppython-cmake-0.1.1.dev15/tests/unit/test_generator.py` & `cppython-cmake-0.1.1.dev16/tests/unit/test_generator.py`

 * *Files identical despite different names*

### Comparing `cppython-cmake-0.1.1.dev15/PKG-INFO` & `cppython-cmake-0.1.1.dev16/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cppython-cmake
-Version: 0.1.1.dev15
+Version: 0.1.1.dev16
 Summary: A plugin for CPPython that enables a CMake generator for C++ projects
 License: MIT
 Author-email: Synodic Software <contact@synodic.software>
 Requires-Python: >=3.11
 Project-URL: homepage, https://github.com/Synodic-Software/CPPython-CMake
 Project-URL: repository, https://github.com/Synodic-Software/CPPython-CMake
 Description-Content-Type: text/markdown
```

