# Comparing `tmp/pytest_hot_reloading-0.1.0a1.tar.gz` & `tmp/pytest_hot_reloading-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_hot_reloading-0.1.0a1.tar", max compression
+gzip compressed data, was "pytest_hot_reloading-0.1.0a2.tar", max compression
```

## Comparing `pytest_hot_reloading-0.1.0a1.tar` & `pytest_hot_reloading-0.1.0a2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1072 2023-04-07 00:33:48.326861 pytest_hot_reloading-0.1.0a1/LICENSE
--rw-r--r--   0        0        0     2402 2023-04-21 20:07:47.475596 pytest_hot_reloading-0.1.0a1/README.md
--rw-r--r--   0        0        0      655 2023-04-23 17:18:42.973057 pytest_hot_reloading-0.1.0a1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-07 00:39:23.095602 pytest_hot_reloading-0.1.0a1/pytest_hot_reloading/__init__.py
--rw-r--r--   0        0        0     1716 2023-04-21 18:53:22.219113 pytest_hot_reloading-0.1.0a1/pytest_hot_reloading/client.py
--rw-r--r--   0        0        0     4557 2023-04-21 19:45:15.205903 pytest_hot_reloading-0.1.0a1/pytest_hot_reloading/daemon.py
--rw-r--r--   0        0        0     6013 2023-04-21 19:51:49.361239 pytest_hot_reloading-0.1.0a1/pytest_hot_reloading/plugin.py
--rw-r--r--   0        0        0     2803 1970-01-01 00:00:00.000000 pytest_hot_reloading-0.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-07 00:33:48.326861 pytest_hot_reloading-0.1.0a2/LICENSE
+-rw-r--r--   0        0        0     2402 2023-04-21 20:07:47.475596 pytest_hot_reloading-0.1.0a2/README.md
+-rw-r--r--   0        0        0      655 2023-04-23 17:25:52.941402 pytest_hot_reloading-0.1.0a2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-07 00:39:23.095602 pytest_hot_reloading-0.1.0a2/pytest_hot_reloading/__init__.py
+-rw-r--r--   0        0        0     1716 2023-04-21 18:53:22.219113 pytest_hot_reloading-0.1.0a2/pytest_hot_reloading/client.py
+-rw-r--r--   0        0        0     4557 2023-04-21 19:45:15.205903 pytest_hot_reloading-0.1.0a2/pytest_hot_reloading/daemon.py
+-rw-r--r--   0        0        0     6013 2023-04-21 19:51:49.361239 pytest_hot_reloading-0.1.0a2/pytest_hot_reloading/plugin.py
+-rw-r--r--   0        0        0     2848 1970-01-01 00:00:00.000000 pytest_hot_reloading-0.1.0a2/PKG-INFO
```

### Comparing `pytest_hot_reloading-0.1.0a1/LICENSE` & `pytest_hot_reloading-0.1.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_hot_reloading-0.1.0a1/README.md` & `pytest_hot_reloading-0.1.0a2/README.md`

 * *Files identical despite different names*

### Comparing `pytest_hot_reloading-0.1.0a1/pyproject.toml` & `pytest_hot_reloading-0.1.0a2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,24 +2,23 @@
 line-length = 98
 
 [tool.black]
 line-length = 98
 
 [tool.poetry]
 name = "pytest-hot-reloading"
-version = "0.1.0-alpha.1"
+version = "0.1.0-alpha.2"
 description = "A pytest plugin to enable a hot reloading daemon."
 authors = ["James Hutchison <jamesghutchison@proton.me>"]
 readme = "README.md"
 packages = [{ include = "pytest_hot_reloading" }]
 
 [tool.poetry.dependencies]
-python = "~3.11"
-jurigged = "^0.5.5"
-
+python = ">=3.10"
+jurigged = "~0.5.5"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.2.0"
 ruff = "^0.0.261"
 black = "^23.3.0"
 pytest = "^7.2.2"
```

### Comparing `pytest_hot_reloading-0.1.0a1/pytest_hot_reloading/client.py` & `pytest_hot_reloading-0.1.0a2/pytest_hot_reloading/client.py`

 * *Files identical despite different names*

### Comparing `pytest_hot_reloading-0.1.0a1/pytest_hot_reloading/daemon.py` & `pytest_hot_reloading-0.1.0a2/pytest_hot_reloading/daemon.py`

 * *Files identical despite different names*

### Comparing `pytest_hot_reloading-0.1.0a1/pytest_hot_reloading/plugin.py` & `pytest_hot_reloading-0.1.0a2/pytest_hot_reloading/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_hot_reloading-0.1.0a1/PKG-INFO` & `pytest_hot_reloading-0.1.0a2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: pytest-hot-reloading
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: A pytest plugin to enable a hot reloading daemon.
 Author: James Hutchison
 Author-email: jamesghutchison@proton.me
-Requires-Python: >=3.11,<3.12
+Requires-Python: >=3.10
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: jurigged (>=0.5.5,<0.6.0)
 Description-Content-Type: text/markdown
 
 # A PyTest Hot Reloading Plugin
 A hot reloading pytest daemon, implemented as a plugin.
```

