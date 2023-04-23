# Comparing `tmp/crunch-cli-0.8.1.tar.gz` & `tmp/crunch-cli-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crunch-cli-0.8.1.tar", last modified: Wed Mar 29 00:22:39 2023, max compression
+gzip compressed data, was "crunch-cli-0.9.0.tar", last modified: Mon Apr  3 12:45:02 2023, max compression
```

## Comparing `crunch-cli-0.8.1.tar` & `crunch-cli-0.9.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 00:22:39.016446 crunch-cli-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-03-29 00:22:39.016446 crunch-cli-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-29 00:22:31.000000 crunch-cli-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 00:22:39.016446 crunch-cli-0.8.1/crunch_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-03-29 00:22:31.000000 crunch-cli-0.8.1/crunch_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-29 00:22:31.000000 crunch-cli-0.8.1/crunch_cli/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 00:22:39.016446 crunch-cli-0.8.1/crunch_cli/command/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-29 00:22:31.000000 crunch-cli-0.8.1/crunch_cli/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-03-29 00:22:31.000000 crunch-cli-0.8.1/crunch_cli/command/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-03-29 00:22:31.000000 crunch-cli-0.8.1/crunch_cli/command/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-03-29 00:22:31.000000 crunch-cli-0.8.1/crunch_cli/command/push.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-03-29 00:22:31.000000 crunch-cli-0.8.1/crunch_cli/command/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-03-29 00:22:31.000000 crunch-cli-0.8.1/crunch_cli/command/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-03-29 00:22:31.000000 crunch-cli-0.8.1/crunch_cli/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-03-29 00:22:31.000000 crunch-cli-0.8.1/crunch_cli/ensure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-03-29 00:22:31.000000 crunch-cli-0.8.1/crunch_cli/inline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-03-29 00:22:31.000000 crunch-cli-0.8.1/crunch_cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-03-29 00:22:31.000000 crunch-cli-0.8.1/crunch_cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 00:22:39.016446 crunch-cli-0.8.1/crunch_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-03-29 00:22:39.000000 crunch-cli-0.8.1/crunch_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-03-29 00:22:39.000000 crunch-cli-0.8.1/crunch_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 00:22:39.000000 crunch-cli-0.8.1/crunch_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-29 00:22:39.000000 crunch-cli-0.8.1/crunch_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 00:22:39.000000 crunch-cli-0.8.1/crunch_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-29 00:22:39.000000 crunch-cli-0.8.1/crunch_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-29 00:22:39.000000 crunch-cli-0.8.1/crunch_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 00:22:39.016446 crunch-cli-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-03-29 00:22:31.000000 crunch-cli-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:45:02.956189 crunch-cli-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-03 12:45:02.956189 crunch-cli-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-03 12:44:58.000000 crunch-cli-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:45:02.952189 crunch-cli-0.9.0/crunch_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-03 12:44:58.000000 crunch-cli-0.9.0/crunch_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-03 12:44:58.000000 crunch-cli-0.9.0/crunch_cli/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:45:02.956189 crunch-cli-0.9.0/crunch_cli/command/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-03 12:44:58.000000 crunch-cli-0.9.0/crunch_cli/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-03 12:44:58.000000 crunch-cli-0.9.0/crunch_cli/command/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-04-03 12:44:58.000000 crunch-cli-0.9.0/crunch_cli/command/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-03 12:44:58.000000 crunch-cli-0.9.0/crunch_cli/command/push.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-03 12:44:58.000000 crunch-cli-0.9.0/crunch_cli/command/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-04-03 12:44:58.000000 crunch-cli-0.9.0/crunch_cli/command/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-03 12:44:58.000000 crunch-cli-0.9.0/crunch_cli/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-03 12:44:58.000000 crunch-cli-0.9.0/crunch_cli/ensure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-04-03 12:44:58.000000 crunch-cli-0.9.0/crunch_cli/inline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-04-03 12:44:58.000000 crunch-cli-0.9.0/crunch_cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-04-03 12:44:58.000000 crunch-cli-0.9.0/crunch_cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:45:02.956189 crunch-cli-0.9.0/crunch_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-03 12:45:02.000000 crunch-cli-0.9.0/crunch_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-03 12:45:02.000000 crunch-cli-0.9.0/crunch_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 12:45:02.000000 crunch-cli-0.9.0/crunch_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-03 12:45:02.000000 crunch-cli-0.9.0/crunch_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 12:45:02.000000 crunch-cli-0.9.0/crunch_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-03 12:45:02.000000 crunch-cli-0.9.0/crunch_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-03 12:45:02.000000 crunch-cli-0.9.0/crunch_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 12:45:02.956189 crunch-cli-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-03 12:44:58.000000 crunch-cli-0.9.0/setup.py
```

### Comparing `crunch-cli-0.8.1/crunch_cli/command/convert.py` & `crunch-cli-0.9.0/crunch_cli/command/convert.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,34 @@
 import os
 import json
 import ast
 import astor
 import re
 import click
+import typing
 
 from .. import constants
 
-def convert(
-    notebook_file_path: str,
-    python_file_path: str,
-    override: bool = False,
-):
-    with open(notebook_file_path) as fd:
-        notebook = json.load(fd)
 
+def convert_cells(cells: typing.List[typing.Any]):
     module = ast.Module()
     module.body = []
 
-    for cell in notebook.get("cells", []):
-        cell_id = cell["metadata"]["id"]
+    for index, cell in enumerate(cells):
+        cell_id = cell["metadata"].get("id") or f"cell_{index}"
 
         def log(message):
             print(f"convert {cell_id} {message}")
 
         cell_type = cell["cell_type"]
         if cell_type != "code":
             log(f"skip since not code: {cell_type}")
             continue
 
-        source = "".join(
+        source = "\n".join(
             line
             for line in cell["source"]
             if not re.match(r"^\s*?(!|%|#)", line)
         )
 
         if not len(source):
             log(f"skip since empty (without !bash, %magic and #comment)")
@@ -48,22 +43,45 @@
                 module.body.append(node)
 
         if valid == 0:
             log(f"skip since no valid node")
         else:
             log(f"used {valid}/{len(tree.body)} node(s)")
 
-    source = astor.to_source(module)
+    return astor.to_source(module)
+
+
+def convert_cells_to_file(
+    cells: typing.List[typing.Any],
+    python_file_path: str,
+    override: bool = False,
+):
+    source = convert_cells(cells)
 
     if python_file_path != constants.CONVERTED_MAIN_PY and not override and os.path.exists(python_file_path):
         override = click.prompt(
             f"file {python_file_path} already exists, override?",
             type=bool,
             default=False,
             prompt_suffix=" "
         )
 
         if not override:
             raise click.Abort()
 
     with open(python_file_path, "w") as fd:
         fd.write(source)
+
+
+def convert(
+    notebook_file_path: str,
+    python_file_path: str,
+    override: bool = False,
+):
+    with open(notebook_file_path) as fd:
+        notebook = json.load(fd)
+
+    convert_cells_to_file(
+        notebook.get("cells", []),
+        python_file_path,
+        override
+    )
```

### Comparing `crunch-cli-0.8.1/crunch_cli/command/download.py` & `crunch-cli-0.9.0/crunch_cli/command/download.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-0.8.1/crunch_cli/command/push.py` & `crunch-cli-0.9.0/crunch_cli/command/push.py`

 * *Files 21% similar despite different names*

```diff
@@ -43,14 +43,23 @@
         with open(tmp.name, "rb") as fd:
             version = session.post(
                 f"/v1/projects/{project_name}/versions",
                 data={
                     "message": message,
                     "mainFilePath": main_file_path,
                     "pushToken": push_token,
+                    "notebook": False
                 },
                 files={
-                    "tarFile": ('code.tar', fd, "application/x-tar")
+                    "file": ('code.tar', fd, "application/x-tar")
                 }
             ).json()
 
     return version
+
+
+def push_summary(version, session: utils.CustomSession):
+    print("\n---")
+    print(f"Version #{version['number']} succesfully uploaded!")
+
+    url = session.format_web_url(f"/project/versions/{version['number']}")
+    print(f"Find it on your dashboard: {url}")
```

### Comparing `crunch-cli-0.8.1/crunch_cli/command/setup.py` & `crunch-cli-0.9.0/crunch_cli/command/setup.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-0.8.1/crunch_cli/command/test.py` & `crunch-cli-0.9.0/crunch_cli/command/test.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-0.8.1/crunch_cli/ensure.py` & `crunch-cli-0.9.0/crunch_cli/ensure.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-0.8.1/crunch_cli/inline.py` & `crunch-cli-0.9.0/crunch_cli/inline.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import typing
 import pandas
 import os
 import click
 
-from . import utils, ensure
+from . import utils, ensure, constants
 from . import command
 
 
 class _Inline:
 
     def __init__(self, module: typing.Any):
         self.module = module
@@ -23,14 +23,18 @@
             os.environ["API_BASE_URL"],
             bool(os.environ.get("DEBUG", "False")),
         )
 
         print(f"loaded inline runner with module: {module}")
 
     def call_process_data(self) -> typing.Union[pandas.DataFrame, pandas.DataFrame, pandas.DataFrame]:
+        print("call_process_data() is deprecated, use call call_data_process() instead")
+        return self.call_data_process()
+
+    def call_data_process(self) -> typing.Union[pandas.DataFrame, pandas.DataFrame, pandas.DataFrame]:
         handler = ensure.is_function(self.module, "data_process")
 
         (
             x_train_path,
             y_train_path,
             x_test_path
         ) = command.download(self.session)
@@ -71,10 +75,47 @@
 
         handler = ensure.is_function(self.module, "infer")
         prediction = handler(self.model, self.x_test)
         self.prediction = ensure.return_infer(prediction)
 
         return self.prediction
 
+    def push(self) -> pandas.DataFrame:
+        codes = self.module.In
+
+        before = os.getcwd()
+        try:
+            utils.change_root()
+
+            main_file_path = constants.CONVERTED_MAIN_PY
+            command.convert_cells_to_file(
+                [
+                    {
+                        "metadata": {
+                            "id": f"cell_{index}"
+                        },
+                        "cell_type": "code",
+                        "source": code.split("\n")
+                    }
+                    for index, code in enumerate(codes)
+                ],
+                main_file_path
+            )
+
+            version = command.push(
+                self.session,
+                click.prompt("Message", default="", show_default=False),
+                main_file_path
+            )
+
+            command.push_summary(version, self.session)
+        finally:
+            now = os.getcwd()
+            if before != now:
+                try:
+                    os.chdir(before)
+                except:
+                    print(f"chdir could not go back to {before}")
+
 
 def load(module: typing.Any):
     return _Inline(module)
```

### Comparing `crunch-cli-0.8.1/crunch_cli/main.py` & `crunch-cli-0.9.0/crunch_cli/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,19 +91,15 @@
     try:
         version = command.push(
             session,
             message=message,
             main_file_path=main_file_path
         )
 
-        print("\n---")
-        print(f"Version #{version['number']} succesfully uploaded!")
-
-        url = session.format_web_url(f"/project/versions/{version['number']}")
-        print(f"Find it on your dashboard: {url}")
+        command.push_summary(version, session)
     finally:
         if converted:
             os.unlink(main_file_path)
 
 
 @cli.command(help="Test your code locally.")
 @click.option("-m", "--main-file", "main_file_path", default="main.py", show_default=True, help="Entrypoint of your code.")
```

### Comparing `crunch-cli-0.8.1/crunch_cli/utils.py` & `crunch-cli-0.9.0/crunch_cli/utils.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-0.8.1/crunch_cli.egg-info/SOURCES.txt` & `crunch-cli-0.9.0/crunch_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crunch-cli-0.8.1/setup.py` & `crunch-cli-0.9.0/setup.py`

 * *Files identical despite different names*

