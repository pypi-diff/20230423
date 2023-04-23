# Comparing `tmp/cookiecutter_autodocs-0.0.3.tar.gz` & `tmp/cookiecutter_autodocs-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cookiecutter_autodocs-0.0.3.tar", max compression
+gzip compressed data, was "cookiecutter_autodocs-0.0.4.tar", max compression
```

## Comparing `cookiecutter_autodocs-0.0.3.tar` & `cookiecutter_autodocs-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1063 2023-04-17 02:41:42.888210 cookiecutter_autodocs-0.0.3/LICENSE
--rw-r--r--   0        0        0     2907 2023-04-17 02:41:42.888210 cookiecutter_autodocs-0.0.3/README.md
--rw-r--r--   0        0        0        0 2023-04-17 02:41:42.888210 cookiecutter_autodocs-0.0.3/cookiecutter_autodocs/__init__.py
--rw-r--r--   0        0        0      779 2023-04-17 02:41:42.888210 cookiecutter_autodocs-0.0.3/cookiecutter_autodocs/cli/__init__.py
--rw-r--r--   0        0        0      542 2023-04-17 02:41:42.888210 cookiecutter_autodocs-0.0.3/cookiecutter_autodocs/cli/_async.py
--rw-r--r--   0        0        0      182 2023-04-17 02:41:42.888210 cookiecutter_autodocs-0.0.3/cookiecutter_autodocs/cli/app.py
--rw-r--r--   0        0        0     3829 2023-04-17 02:41:42.888210 cookiecutter_autodocs-0.0.3/cookiecutter_autodocs/cli/generate.py
--rw-r--r--   0        0        0     1844 2023-04-17 02:41:42.888210 cookiecutter_autodocs-0.0.3/cookiecutter_autodocs/cli/gha.py
--rw-r--r--   0        0        0     1135 2023-04-17 02:41:42.888210 cookiecutter_autodocs-0.0.3/cookiecutter_autodocs/cli/validate.py
--rw-r--r--   0        0        0        0 2023-04-17 02:41:42.888210 cookiecutter_autodocs-0.0.3/cookiecutter_autodocs/lib/__init__.py
--rw-r--r--   0        0        0     2015 2023-04-17 02:41:42.888210 cookiecutter_autodocs-0.0.3/cookiecutter_autodocs/lib/files.py
--rw-r--r--   0        0        0      239 2023-04-17 02:41:42.888210 cookiecutter_autodocs-0.0.3/cookiecutter_autodocs/lib/typing.py
--rw-r--r--   0        0        0        0 2023-04-17 02:41:42.888210 cookiecutter_autodocs-0.0.3/cookiecutter_autodocs/py.typed
--rw-r--r--   0        0        0      161 2023-04-17 02:41:42.888210 cookiecutter_autodocs-0.0.3/cookiecutter_autodocs/schemas/__init__.py
--rw-r--r--   0        0        0      502 2023-04-17 02:41:42.888210 cookiecutter_autodocs-0.0.3/cookiecutter_autodocs/schemas/_base.py
--rw-r--r--   0        0        0     5573 2023-04-17 02:41:42.888210 cookiecutter_autodocs-0.0.3/cookiecutter_autodocs/schemas/description.py
--rw-r--r--   0        0        0     1398 2023-04-17 02:41:42.888210 cookiecutter_autodocs-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3730 1970-01-01 00:00:00.000000 cookiecutter_autodocs-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-04-23 04:11:03.060036 cookiecutter_autodocs-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2907 2023-04-23 04:11:03.060036 cookiecutter_autodocs-0.0.4/README.md
+-rw-r--r--   0        0        0        0 2023-04-23 04:11:03.060036 cookiecutter_autodocs-0.0.4/cookiecutter_autodocs/__init__.py
+-rw-r--r--   0        0        0      779 2023-04-23 04:11:03.060036 cookiecutter_autodocs-0.0.4/cookiecutter_autodocs/cli/__init__.py
+-rw-r--r--   0        0        0      542 2023-04-23 04:11:03.060036 cookiecutter_autodocs-0.0.4/cookiecutter_autodocs/cli/_async.py
+-rw-r--r--   0        0        0      182 2023-04-23 04:11:03.060036 cookiecutter_autodocs-0.0.4/cookiecutter_autodocs/cli/app.py
+-rw-r--r--   0        0        0     4244 2023-04-23 04:11:03.060036 cookiecutter_autodocs-0.0.4/cookiecutter_autodocs/cli/generate.py
+-rw-r--r--   0        0        0     1844 2023-04-23 04:11:03.060036 cookiecutter_autodocs-0.0.4/cookiecutter_autodocs/cli/gha.py
+-rw-r--r--   0        0        0     1403 2023-04-23 04:11:03.060036 cookiecutter_autodocs-0.0.4/cookiecutter_autodocs/cli/validate.py
+-rw-r--r--   0        0        0        0 2023-04-23 04:11:03.060036 cookiecutter_autodocs-0.0.4/cookiecutter_autodocs/lib/__init__.py
+-rw-r--r--   0        0        0     2015 2023-04-23 04:11:03.060036 cookiecutter_autodocs-0.0.4/cookiecutter_autodocs/lib/files.py
+-rw-r--r--   0        0        0      239 2023-04-23 04:11:03.060036 cookiecutter_autodocs-0.0.4/cookiecutter_autodocs/lib/typing.py
+-rw-r--r--   0        0        0        0 2023-04-23 04:11:03.060036 cookiecutter_autodocs-0.0.4/cookiecutter_autodocs/py.typed
+-rw-r--r--   0        0        0      161 2023-04-23 04:11:03.060036 cookiecutter_autodocs-0.0.4/cookiecutter_autodocs/schemas/__init__.py
+-rw-r--r--   0        0        0      502 2023-04-23 04:11:03.060036 cookiecutter_autodocs-0.0.4/cookiecutter_autodocs/schemas/_base.py
+-rw-r--r--   0        0        0     5573 2023-04-23 04:11:03.060036 cookiecutter_autodocs-0.0.4/cookiecutter_autodocs/schemas/description.py
+-rw-r--r--   0        0        0     1417 2023-04-23 04:11:03.064036 cookiecutter_autodocs-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3730 1970-01-01 00:00:00.000000 cookiecutter_autodocs-0.0.4/PKG-INFO
```

### Comparing `cookiecutter_autodocs-0.0.3/LICENSE` & `cookiecutter_autodocs-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cookiecutter_autodocs-0.0.3/README.md` & `cookiecutter_autodocs-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `cookiecutter_autodocs-0.0.3/cookiecutter_autodocs/cli/__init__.py` & `cookiecutter_autodocs-0.0.4/cookiecutter_autodocs/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `cookiecutter_autodocs-0.0.3/cookiecutter_autodocs/cli/_async.py` & `cookiecutter_autodocs-0.0.4/cookiecutter_autodocs/cli/_async.py`

 * *Files identical despite different names*

### Comparing `cookiecutter_autodocs-0.0.3/cookiecutter_autodocs/cli/generate.py` & `cookiecutter_autodocs-0.0.4/cookiecutter_autodocs/cli/generate.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,75 +7,77 @@
 from typing import Any
 from typing import Dict
 from typing import Optional
 
 from aiofiles.os import path as aiopath
 from markdownTable import markdownTable
 from rich import print
-from typer import Option
+from typer import Option, Argument
 
 generate_app = AsyncTyper()
 
 
 @generate_app.async_command()
 async def desc(
-    cookiecutter_json: Path = Option(..., "--input", "-i", help="Path to the cookiecutter.json file"),
-    cookiecutter_desc: Path = Option(
-        ...,
+    cookiecutter_json: Path = Argument(..., help="Path to the cookiecutter.json file"),
+    cookiecutter_desc: Optional[Path] = Option(
+        None,
         "--output",
         "-o",
-        help="Path to a cookiecutter.desc file to write. If the file exists, it will be updated in place.",
+        help="Path to a cookiecutter.desc file to write. If the file exists, it will be updated in place. "
+        + "If not specified, the cookiecutter.desc will be written to the same directory as the cookiecutter.json file",
     ),
 ) -> None:
     """Generate a new or update an existing cookiecutter.desc from a cookiecutter.json file."""
+    if cookiecutter_desc is None:
+        cookiecutter_desc = cookiecutter_json.parent / "cookiecutter.desc"
     if await aiopath.exists(str(cookiecutter_desc)):
         print(f"Updating an existing cookiecutter.desc file at {cookiecutter_desc}")
         existing_desc = await CookieCutterDescription.from_cookiecutter_desc(cookiecutter_desc)
     else:
         print(f"Generating a new cookiecutter.desc file at {cookiecutter_desc}")
         existing_desc = CookieCutterDescription(variables={})
     existing_desc.update(await CookieCutterDescription.from_cookiecutter_json(cookiecutter_json))
     await existing_desc.to_cookiecutter_desc(cookiecutter_desc)
     print(f"Generated {cookiecutter_desc} from {cookiecutter_json}")
 
 
 @generate_app.async_command()
 async def cookiecutter(
-    cookiecutter_desc: Path = Option(
+    cookiecutter_desc: Path = Argument(
         ...,
-        "--input",
-        "-i",
         help="Path to a cookiecutter.desc file to read.",
     ),
-    cookiecutter_json: Path = Option(
-        ...,
+    cookiecutter_json: Optional[Path] = Option(
+        None,
         "--output",
         "-o",
-        help="Path to the cookiecutter.json file.  If the file exists, it will be updated in place.",
+        help="Path to the cookiecutter.json file.  If the file exists, it will be updated in place. If not specified, "
+        + "the cookiecutter.json will be written to the same directory as the cookiecutter.json file",
     ),
 ) -> None:
     """Generate a new or update an existing cookiecutter.json file from a cookiecutter.desc."""
+    if cookiecutter_json is None:
+        cookiecutter_json = cookiecutter_desc.parent / "cookiecutter.json"
     if await aiopath.exists(str(cookiecutter_json)):
         print(f"Updating an existing cookiecutter.json file at {cookiecutter_json}")
         existing_json: Dict[str, Any] = await load_cookiecutter_json(cookiecutter_json)
     else:
         print(f"Generating a new cookiecutter.json file at {cookiecutter_json}")
         existing_json = {}
     existing_desc = await CookieCutterDescription.from_cookiecutter_desc(cookiecutter_desc)
     existing_json.update(existing_desc.cookiecutter_json)
     await dump_cookiecutter_json(cookiecutter_json, existing_json)
     print(f"Generated {cookiecutter_json} from {cookiecutter_desc}")
 
 
 @generate_app.async_command()
 async def markdown(
-    cookiecutter_desc: Path = Option(
+    cookiecutter_desc: Path = Argument(
         ...,
-        "--input",
-        "-i",
         help="Path to a cookiecutter.desc file to read.",
     ),
     markdown_file: Optional[Path] = Option(
         None,
         "--outfile",
         "-o",
         help="File to write the markdown table to. If blank, will output to stdout",
```

### Comparing `cookiecutter_autodocs-0.0.3/cookiecutter_autodocs/cli/gha.py` & `cookiecutter_autodocs-0.0.4/cookiecutter_autodocs/cli/gha.py`

 * *Files identical despite different names*

### Comparing `cookiecutter_autodocs-0.0.3/cookiecutter_autodocs/cli/validate.py` & `cookiecutter_autodocs-0.0.4/cookiecutter_autodocs/cli/validate.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 """Code for the validate CLI sub-command"""
 from cookiecutter_autodocs.cli.app import app
 from cookiecutter_autodocs.schemas.description import CookieCutterDescription
 from cookiecutter_autodocs.lib.files import load_cookiecutter_json
 
 from typer import Argument, Option, Exit
 from pathlib import Path
-
+from typing import Optional
 from rich import print
 
 
 @app.async_command()
 async def validate(
     cookiecutter_desc: Path = Argument(
         ...,
         help="Path to the cookiecutter.desc file",
     ),
-    cookiecutter_json: Path = Argument(
-        ...,
-        help="Path to the cookiecutter.json file",
+    cookiecutter_json: Optional[Path] = Argument(
+        None,
+        help="Path to the cookiecutter.json file. If not specified, the cookiecutter.json will be read from the same"
+        + " directory as the cookiecutter.desc file",
     ),
     allow_empty_description: bool = Option(
         False, help="Allow empty descriptions. If not set, an empty description will cause an error."
     ),
 ) -> None:
+    if cookiecutter_json is None:
+        cookiecutter_json = cookiecutter_desc.parent / "cookiecutter.json"
     desc = await CookieCutterDescription.from_cookiecutter_desc(cookiecutter_desc)
     validated, errors = desc.validate_cookiecutter_json(
         await load_cookiecutter_json(cookiecutter_json), allow_empty_desc=allow_empty_description
     )
     if not validated:
         print("Validation failed:")
         print(errors)
```

### Comparing `cookiecutter_autodocs-0.0.3/cookiecutter_autodocs/lib/files.py` & `cookiecutter_autodocs-0.0.4/cookiecutter_autodocs/lib/files.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     """Dump a cookiecutter.json file.
 
     Args:
         cookiecutter_path (StrOrPath): Path to the cookiecutter.json file.
         cookiecutter (dict): The cookiecutter.json file as a dictionary.
     """
     async with aiofiles.open(str(path_or_str), "w") as afh:
-        await afh.write(json.dumps(cookiecutter, indent=4))
+        await afh.write(json.dumps(cookiecutter, indent=2))
 
 
 async def load_cookiecutter_description(path_or_str: StrOrPath) -> Dict[str, Any]:
     """
     Load a cookiecutter.desc file.
 
     Args:
```

### Comparing `cookiecutter_autodocs-0.0.3/cookiecutter_autodocs/schemas/description.py` & `cookiecutter_autodocs-0.0.4/cookiecutter_autodocs/schemas/description.py`

 * *Files identical despite different names*

### Comparing `cookiecutter_autodocs-0.0.3/pyproject.toml` & `cookiecutter_autodocs-0.0.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cookiecutter-autodocs"
-version = "0.0.3"
+version = "0.0.4"
 description = "Generate docs from your cookiecutter template"
 authors = ["Andrew Herrington <andrew.the.techie@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "cookiecutter_autodocs"}]
 
 [tool.poetry.dependencies]
@@ -37,15 +37,15 @@
 pyflakes = "^3.0.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.bandit]
-exclude_dirs = ["tests", "noxfile.py"]
+exclude_dirs = ["tests", "noxfile.py", ".github/scripts"]
 
 
 [tool.black]
 line-length = 120
 
 [tool.ruff]
 line-length = 120
```

### Comparing `cookiecutter_autodocs-0.0.3/PKG-INFO` & `cookiecutter_autodocs-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cookiecutter-autodocs
-Version: 0.0.3
+Version: 0.0.4
 Summary: Generate docs from your cookiecutter template
 License: MIT
 Author: Andrew Herrington
 Author-email: andrew.the.techie@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

