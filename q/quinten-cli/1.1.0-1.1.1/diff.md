# Comparing `tmp/quinten-cli-1.1.0.tar.gz` & `tmp/quinten-cli-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quinten-cli-1.1.0.tar", last modified: Sun Apr 23 18:25:00 2023, max compression
+gzip compressed data, was "quinten-cli-1.1.1.tar", last modified: Sun Apr 23 18:29:54 2023, max compression
```

## Comparing `quinten-cli-1.1.0.tar` & `quinten-cli-1.1.1.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-04-23 18:25:00.848521 quinten-cli-1.1.0/
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     1069 2023-04-23 18:15:22.000000 quinten-cli-1.1.0/LICENSE
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      672 2023-04-23 18:25:00.848521 quinten-cli-1.1.0/PKG-INFO
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      294 2023-04-23 18:15:22.000000 quinten-cli-1.1.0/README.md
-drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-04-23 18:25:00.848521 quinten-cli-1.1.0/cli/
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      925 2023-04-23 18:15:22.000000 quinten-cli-1.1.0/cli/__init__.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      157 2023-04-23 18:15:22.000000 quinten-cli-1.1.0/cli/env.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      625 2023-04-23 18:15:22.000000 quinten-cli-1.1.0/cli/input_interface.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      741 2023-04-23 18:15:22.000000 quinten-cli-1.1.0/cli/install.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     1241 2023-04-23 18:15:22.000000 quinten-cli-1.1.0/cli/output_interface.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     1483 2023-04-23 18:15:22.000000 quinten-cli-1.1.0/cli/progress.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     5139 2023-04-23 18:19:12.000000 quinten-cli-1.1.0/cli/run.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      366 2023-04-23 18:15:22.000000 quinten-cli-1.1.0/cli/status.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      586 2023-04-23 18:23:25.000000 quinten-cli-1.1.0/pyproject.toml
-drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-04-23 18:25:00.848521 quinten-cli-1.1.0/quinten_cli.egg-info/
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      672 2023-04-23 18:25:00.000000 quinten-cli-1.1.0/quinten_cli.egg-info/PKG-INFO
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      453 2023-04-23 18:25:00.000000 quinten-cli-1.1.0/quinten_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 quinten   (1000) quinten   (1000)        1 2023-04-23 18:25:00.000000 quinten-cli-1.1.0/quinten_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 quinten   (1000) quinten   (1000)       44 2023-04-23 18:25:00.000000 quinten-cli-1.1.0/quinten_cli.egg-info/entry_points.txt
--rw-rw-r--   0 quinten   (1000) quinten   (1000)       74 2023-04-23 18:25:00.000000 quinten-cli-1.1.0/quinten_cli.egg-info/requires.txt
--rw-rw-r--   0 quinten   (1000) quinten   (1000)        4 2023-04-23 18:25:00.000000 quinten-cli-1.1.0/quinten_cli.egg-info/top_level.txt
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      553 2023-04-23 18:25:00.848521 quinten-cli-1.1.0/setup.cfg
--rw-rw-r--   0 quinten   (1000) quinten   (1000)       69 2023-04-23 18:24:58.000000 quinten-cli-1.1.0/setup.py
-drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-04-23 18:25:00.848521 quinten-cli-1.1.0/tests/
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      322 2023-04-23 18:15:22.000000 quinten-cli-1.1.0/tests/test_api.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      937 2023-04-23 18:15:22.000000 quinten-cli-1.1.0/tests/test_progress_ui.py
+drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-04-23 18:29:54.818886 quinten-cli-1.1.1/
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     1069 2023-04-23 18:15:22.000000 quinten-cli-1.1.1/LICENSE
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      603 2023-04-23 18:29:54.818886 quinten-cli-1.1.1/PKG-INFO
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      294 2023-04-23 18:15:22.000000 quinten-cli-1.1.1/README.md
+drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-04-23 18:29:54.818886 quinten-cli-1.1.1/cli/
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      925 2023-04-23 18:15:22.000000 quinten-cli-1.1.1/cli/__init__.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      157 2023-04-23 18:15:22.000000 quinten-cli-1.1.1/cli/env.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      625 2023-04-23 18:15:22.000000 quinten-cli-1.1.1/cli/input_interface.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      741 2023-04-23 18:15:22.000000 quinten-cli-1.1.1/cli/install.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     1241 2023-04-23 18:15:22.000000 quinten-cli-1.1.1/cli/output_interface.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     1483 2023-04-23 18:15:22.000000 quinten-cli-1.1.1/cli/progress.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     5139 2023-04-23 18:19:12.000000 quinten-cli-1.1.1/cli/run.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      366 2023-04-23 18:15:22.000000 quinten-cli-1.1.1/cli/status.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      586 2023-04-23 18:25:17.000000 quinten-cli-1.1.1/pyproject.toml
+drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-04-23 18:29:54.818886 quinten-cli-1.1.1/quinten_cli.egg-info/
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      603 2023-04-23 18:29:54.000000 quinten-cli-1.1.1/quinten_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      564 2023-04-23 18:29:54.000000 quinten-cli-1.1.1/quinten_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)        1 2023-04-23 18:29:54.000000 quinten-cli-1.1.1/quinten_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)       44 2023-04-23 18:29:54.000000 quinten-cli-1.1.1/quinten_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)       74 2023-04-23 18:29:54.000000 quinten-cli-1.1.1/quinten_cli.egg-info/requires.txt
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)        4 2023-04-23 18:29:54.000000 quinten-cli-1.1.1/quinten_cli.egg-info/top_level.txt
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)       38 2023-04-23 18:29:54.818886 quinten-cli-1.1.1/setup.cfg
+drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-04-23 18:29:54.818886 quinten-cli-1.1.1/tests/
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      322 2023-04-23 18:15:22.000000 quinten-cli-1.1.1/tests/test_api.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      937 2023-04-23 18:15:22.000000 quinten-cli-1.1.1/tests/test_progress_ui.py
```

### Comparing `quinten-cli-1.1.0/LICENSE` & `quinten-cli-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `quinten-cli-1.1.0/PKG-INFO` & `quinten-cli-1.1.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 Metadata-Version: 2.1
 Name: quinten-cli
-Version: 1.1.0
-Home-page: https://github.com/quintenroets/cli
-Author: Quinten Roets
+Version: 1.1.1
 Author-email: Quinten Roets <qdr2104@columbia.edu>
 License: MIT
 Project-URL: Source Code, https://github.com/quintenroets/cli
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
```

### Comparing `quinten-cli-1.1.0/cli/__init__.py` & `quinten-cli-1.1.1/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `quinten-cli-1.1.0/cli/input_interface.py` & `quinten-cli-1.1.1/cli/input_interface.py`

 * *Files identical despite different names*

### Comparing `quinten-cli-1.1.0/cli/install.py` & `quinten-cli-1.1.1/cli/install.py`

 * *Files identical despite different names*

### Comparing `quinten-cli-1.1.0/cli/output_interface.py` & `quinten-cli-1.1.1/cli/output_interface.py`

 * *Files identical despite different names*

### Comparing `quinten-cli-1.1.0/cli/progress.py` & `quinten-cli-1.1.1/cli/progress.py`

 * *Files identical despite different names*

### Comparing `quinten-cli-1.1.0/cli/run.py` & `quinten-cli-1.1.1/cli/run.py`

 * *Files identical despite different names*

### Comparing `quinten-cli-1.1.0/pyproject.toml` & `quinten-cli-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "quinten-cli"
-version = "1.1.0"
+version = "1.1.1"
 description = ""
 authors = [{name = "Quinten Roets", email = "qdr2104@columbia.edu"}]
 license = {text = "MIT"}
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
     "python-dotenv",
```

### Comparing `quinten-cli-1.1.0/quinten_cli.egg-info/PKG-INFO` & `quinten-cli-1.1.1/quinten_cli.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 Metadata-Version: 2.1
 Name: quinten-cli
-Version: 1.1.0
-Home-page: https://github.com/quintenroets/cli
-Author: Quinten Roets
+Version: 1.1.1
 Author-email: Quinten Roets <qdr2104@columbia.edu>
 License: MIT
 Project-URL: Source Code, https://github.com/quintenroets/cli
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
```

### Comparing `quinten-cli-1.1.0/tests/test_progress_ui.py` & `quinten-cli-1.1.1/tests/test_progress_ui.py`

 * *Files identical despite different names*

