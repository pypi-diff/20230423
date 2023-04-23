# Comparing `tmp/cleez-0.1.2.tar.gz` & `tmp/cleez-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleez-0.1.2.tar", max compression
+gzip compressed data, was "cleez-0.1.3.tar", max compression
```

## Comparing `cleez-0.1.2.tar` & `cleez-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0      583 2023-04-17 08:35:32.159563 cleez-0.1.2/LICENSE
--rw-r--r--   0        0        0      896 2023-04-17 09:52:54.513608 cleez-0.1.2/README.rst
--rw-r--r--   0        0        0     3102 2023-04-18 16:41:05.082118 cleez-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      340 2023-04-17 16:19:10.886202 cleez-0.1.2/src/cleez/__init__.py
--rw-r--r--   0        0        0     4598 2023-04-17 18:29:05.545545 cleez-0.1.2/src/cleez/cleez.py
--rw-r--r--   0        0        0      371 2023-04-16 21:08:33.001276 cleez-0.1.2/src/cleez/colors.py
--rw-r--r--   0        0        0     1237 2023-04-18 13:52:32.245318 cleez-0.1.2/src/cleez/command.py
--rw-r--r--   0        0        0      268 2023-04-17 18:11:58.414950 cleez-0.1.2/src/cleez/exceptions.py
--rw-r--r--   0        0        0     2692 2023-04-17 19:57:10.619068 cleez-0.1.2/src/cleez/help.py
--rw-r--r--   0        0        0     1758 1970-01-01 00:00:00.000000 cleez-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      583 2023-04-17 08:35:32.159563 cleez-0.1.3/LICENSE
+-rw-r--r--   0        0        0      896 2023-04-17 09:52:54.513608 cleez-0.1.3/README.rst
+-rw-r--r--   0        0        0     3364 2023-04-23 09:08:34.038374 cleez-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      340 2023-04-17 16:19:10.886202 cleez-0.1.3/src/cleez/__init__.py
+-rw-r--r--   0        0        0      553 2023-04-23 08:31:27.115897 cleez-0.1.3/src/cleez/actions.py
+-rw-r--r--   0        0        0     4666 2023-04-23 08:52:49.436377 cleez-0.1.3/src/cleez/cleez.py
+-rw-r--r--   0        0        0      371 2023-04-16 21:08:33.001276 cleez-0.1.3/src/cleez/colors.py
+-rw-r--r--   0        0        0     1237 2023-04-18 13:52:32.245318 cleez-0.1.3/src/cleez/command.py
+-rw-r--r--   0        0        0      268 2023-04-17 18:11:58.414950 cleez-0.1.3/src/cleez/exceptions.py
+-rw-r--r--   0        0        0     2692 2023-04-17 19:57:10.619068 cleez-0.1.3/src/cleez/help.py
+-rw-r--r--   0        0        0    16860 2023-04-23 09:07:58.541193 cleez-0.1.3/src/cleez/testing.py
+-rw-r--r--   0        0        0     1796 1970-01-01 00:00:00.000000 cleez-0.1.3/PKG-INFO
```

### Comparing `cleez-0.1.2/LICENSE` & `cleez-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cleez-0.1.2/README.rst` & `cleez-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `cleez-0.1.2/pyproject.toml` & `cleez-0.1.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "cleez"
-version = "0.1.2"
+version = "0.1.3"
 homepage = "https://github.com/abilian/cleez"
 description = "Simple class-based CLI framework."
 authors = ["Abilian SAS <sf@abilian.com>"]
 readme = "README.rst"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
     'Intended Audience :: Developers',
@@ -23,14 +23,15 @@
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4"
 termcolor = "^2.2.0"
 
 # Temp (for debugging)
 snoop = "^0.4.3"
+click = "^8.1.3"
 
 [tool.poetry.group.dev.dependencies]
 ## Standard cruft
 abilian-devtools = "*"
 
 # Cruft (project templates management)
 cruft = "*"
@@ -83,18 +84,31 @@
     "SIM",
     "TID",
     "RUF",
     "PLC", "PLE", "PLR", "PLW",
 ]
 # Add later: "ANN", "ERA"...
 
+exclude = [
+    "src/cleez/testing.py",
+#    ".tox",
+#    ".nox",
+#    "tests",
+#    "sandbox",
+#    "doc",
+#    "scripts",
+#    "tmp",
+]
+
 ignore = [
     "S101",  # Use of `assert` detected
     "SIM108", # Use ternary operator
     "A001",  # Shadowing of built-in
+    "A002",  # Argument `input` is shadowing a python builtin
+    "I001",  # Ruff not agreeing with isort
 ]
 
 # ---
 
 [tool.bandit]
 skips = [
   "B404", # blacklist
```

### Comparing `cleez-0.1.2/src/cleez/cleez.py` & `cleez-0.1.3/src/cleez/cleez.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,17 @@
         # self.common_options(args)
         if "_command" not in args:
             self.help_maker.print_help(self)
             sys.exit()  # exit 0 or exit 1 ?
 
         self.call_command(args._command, args)
 
+    def main(self, args, prog_name):
+        return self.run(args)
+
     def scan(self, module_name: str):
         root_module = importlib.import_module(module_name)
         root_module_name = root_module.__name__
         root_path = Path(root_module.__file__).parent  # type: ignore
         for _, module_name, _ in iter_modules([str(root_path)]):
             module = importlib.import_module(f"{root_module_name}.{module_name}")
             for attribute_name in dir(module):
```

### Comparing `cleez-0.1.2/src/cleez/command.py` & `cleez-0.1.3/src/cleez/command.py`

 * *Files identical despite different names*

### Comparing `cleez-0.1.2/src/cleez/help.py` & `cleez-0.1.3/src/cleez/help.py`

 * *Files identical despite different names*

### Comparing `cleez-0.1.2/PKG-INFO` & `cleez-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleez
-Version: 0.1.2
+Version: 0.1.3
 Summary: Simple class-based CLI framework.
 Home-page: https://github.com/abilian/cleez
 Author: Abilian SAS
 Author-email: sf@abilian.com
 Requires-Python: >=3.9,<4
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: snoop (>=0.4.3,<0.5.0)
 Requires-Dist: termcolor (>=2.2.0,<3.0.0)
 Description-Content-Type: text/x-rst
 
 =====
 Cleez
 =====
```

