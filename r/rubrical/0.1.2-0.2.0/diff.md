# Comparing `tmp/rubrical-0.1.2.tar.gz` & `tmp/rubrical-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubrical-0.1.2.tar", max compression
+gzip compressed data, was "rubrical-0.2.0.tar", max compression
```

## Comparing `rubrical-0.1.2.tar` & `rubrical-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,25 @@
--rw-r--r--   0        0        0    15976 2023-04-06 09:35:32.148463 rubrical-0.1.2/LICENSE
--rw-r--r--   0        0        0     2543 2023-04-06 09:35:32.148463 rubrical-0.1.2/README.md
--rw-r--r--   0        0        0     1866 2023-04-06 09:35:58.760751 rubrical-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-06 09:35:32.148463 rubrical-0.1.2/rubrical/__init__.py
--rw-r--r--   0        0        0      784 2023-04-06 09:35:32.148463 rubrical-0.1.2/rubrical/comparisons/__init__.py
--rw-r--r--   0        0        0     1799 2023-04-06 09:35:32.148463 rubrical-0.1.2/rubrical/comparisons/semversion.py
--rw-r--r--   0        0        0      519 2023-04-06 09:35:32.148463 rubrical-0.1.2/rubrical/comparisons/string.py
--rw-r--r--   0        0        0      295 2023-04-06 09:35:32.148463 rubrical-0.1.2/rubrical/comparisons/utils.py
--rw-r--r--   0        0        0      504 2023-04-06 09:35:32.148463 rubrical-0.1.2/rubrical/enum.py
--rw-r--r--   0        0        0     2623 2023-04-06 09:35:32.148463 rubrical-0.1.2/rubrical/main.py
--rw-r--r--   0        0        0        0 2023-04-06 09:35:32.148463 rubrical-0.1.2/rubrical/package_managers/__init__.py
--rw-r--r--   0        0        0     1670 2023-04-06 09:35:32.148463 rubrical-0.1.2/rubrical/package_managers/base_package_manager.py
--rw-r--r--   0        0        0     1476 2023-04-06 09:35:32.148463 rubrical-0.1.2/rubrical/package_managers/jsonnet.py
--rw-r--r--   0        0        0     1931 2023-04-06 09:35:32.148463 rubrical-0.1.2/rubrical/package_managers/python.py
--rw-r--r--   0        0        0      271 2023-04-06 09:35:32.148463 rubrical-0.1.2/rubrical/package_managers/utilities/git.py
--rw-r--r--   0        0        0     2352 2023-04-06 09:35:32.148463 rubrical-0.1.2/rubrical/reporters/gh.py
--rw-r--r--   0        0        0     1476 2023-04-06 09:35:32.148463 rubrical-0.1.2/rubrical/reporters/terminal.py
--rw-r--r--   0        0        0     4057 2023-04-06 09:35:32.148463 rubrical-0.1.2/rubrical/rubrical.py
--rw-r--r--   0        0        0      467 2023-04-06 09:35:32.148463 rubrical-0.1.2/rubrical/schemas/configuration.py
--rw-r--r--   0        0        0      251 2023-04-06 09:35:32.148463 rubrical-0.1.2/rubrical/schemas/package.py
--rw-r--r--   0        0        0      235 2023-04-06 09:35:32.148463 rubrical-0.1.2/rubrical/schemas/results.py
--rw-r--r--   0        0        0      633 2023-04-06 09:35:32.148463 rubrical-0.1.2/rubrical/utilities/console.py
--rw-r--r--   0        0        0     3514 1970-01-01 00:00:00.000000 rubrical-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    15976 2023-04-23 12:17:43.241480 rubrical-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2782 2023-04-23 12:17:43.241480 rubrical-0.2.0/README.md
+-rw-r--r--   0        0        0     1865 2023-04-23 12:18:06.421523 rubrical-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-23 12:17:43.241480 rubrical-0.2.0/rubrical/__init__.py
+-rw-r--r--   0        0        0      784 2023-04-23 12:17:43.241480 rubrical-0.2.0/rubrical/comparisons/__init__.py
+-rw-r--r--   0        0        0     2255 2023-04-23 12:17:43.241480 rubrical-0.2.0/rubrical/comparisons/semversion.py
+-rw-r--r--   0        0        0      519 2023-04-23 12:17:43.241480 rubrical-0.2.0/rubrical/comparisons/string.py
+-rw-r--r--   0        0        0      295 2023-04-23 12:17:43.241480 rubrical-0.2.0/rubrical/comparisons/utils.py
+-rw-r--r--   0        0        0      568 2023-04-23 12:17:43.241480 rubrical-0.2.0/rubrical/enum.py
+-rw-r--r--   0        0        0     2623 2023-04-23 12:17:43.241480 rubrical-0.2.0/rubrical/main.py
+-rw-r--r--   0        0        0        0 2023-04-23 12:17:43.241480 rubrical-0.2.0/rubrical/package_managers/__init__.py
+-rw-r--r--   0        0        0     2519 2023-04-23 12:17:43.241480 rubrical-0.2.0/rubrical/package_managers/base_package_manager.py
+-rw-r--r--   0        0        0     1242 2023-04-23 12:17:43.241480 rubrical-0.2.0/rubrical/package_managers/go.py
+-rw-r--r--   0        0        0     1479 2023-04-23 12:17:43.241480 rubrical-0.2.0/rubrical/package_managers/jsonnet.py
+-rw-r--r--   0        0        0     4143 2023-04-23 12:17:43.241480 rubrical-0.2.0/rubrical/package_managers/nodejs.py
+-rw-r--r--   0        0        0     1933 2023-04-23 12:17:43.241480 rubrical-0.2.0/rubrical/package_managers/python.py
+-rw-r--r--   0        0        0      271 2023-04-23 12:17:43.241480 rubrical-0.2.0/rubrical/package_managers/utilities/git.py
+-rw-r--r--   0        0        0     2352 2023-04-23 12:17:43.241480 rubrical-0.2.0/rubrical/reporters/gh.py
+-rw-r--r--   0        0        0     1476 2023-04-23 12:17:43.241480 rubrical-0.2.0/rubrical/reporters/terminal.py
+-rw-r--r--   0        0        0     4265 2023-04-23 12:17:43.241480 rubrical-0.2.0/rubrical/rubrical.py
+-rw-r--r--   0        0        0      467 2023-04-23 12:17:43.241480 rubrical-0.2.0/rubrical/schemas/configuration.py
+-rw-r--r--   0        0        0      251 2023-04-23 12:17:43.241480 rubrical-0.2.0/rubrical/schemas/package.py
+-rw-r--r--   0        0        0      235 2023-04-23 12:17:43.241480 rubrical-0.2.0/rubrical/schemas/results.py
+-rw-r--r--   0        0        0      633 2023-04-23 12:17:43.241480 rubrical-0.2.0/rubrical/utilities/console.py
+-rw-r--r--   0        0        0     3752 1970-01-01 00:00:00.000000 rubrical-0.2.0/PKG-INFO
```

### Comparing `rubrical-0.1.2/LICENSE` & `rubrical-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rubrical-0.1.2/README.md` & `rubrical-0.2.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 [![CI](https://github.com/ivanklee86/rubrical/actions/workflows/ci.yaml/badge.svg)](https://github.com/ivanklee86/rubrical/actions/workflows/ci.yaml) [![codecov](https://codecov.io/gh/ivanklee86/rubrical/branch/main/graph/badge.svg?token=9WJM4LBDEX)](https://codecov.io/gh/ivanklee86/rubrical) [![PyPI version](https://badge.fury.io/py/rubrical.svg)](https://badge.fury.io/py/rubrical)
 
 A CLI to encourage (😅) people to update their dependencies!
 
 Supported package managers:
 * Python (requirements.txt)
+* Go (go.mod)
+* Node.js (package.lock)
 * Jsonnet
 * _More coming soon!_
 
 ![rubrical](docs/images/rubrical.png)
 
 ## Installation
 
@@ -49,24 +51,34 @@
 ## Configuration
 
 The `rubrical.yaml` file is used to configure checks for your application.
 
 ```yaml
 version: 1
 package_managers:
+  - name: jsonnet
+    packages:
+      - name: "xunleii/vector_jsonnet" # Name of the dependency
+        block: v0.1.0  # If dependency is older than this, error.
+        warn: v0.1.2  # If dependency is older than this, warn.
   - name: python
     packages:
       - name: Mopidy-Dirble
         block: v1.2.1
         warn: v1.2.2
-  - name: jsonnet
+  - name: go
     packages:
-      - name: "xunleii/vector_jsonnet" # Name of the dependency
-        block: v0.1.0  # If dependency is older than this, error.
-        warn: v0.1.2  # If dependency is older than this, warn.
+      - name: github.com/adrg/xdg
+        block: v0.5.0
+        warn: v0.6.0
+  - name: nodejs
+    packages:
+      - name: react
+        block: v17.0.3
+        warn: v17.0.4
 ```
 
 ## Reporting
 
 ### Terminal
 
 Comes for free!
```

### Comparing `rubrical-0.1.2/pyproject.toml` & `rubrical-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 [tool.isort]
 profile = "black"
 
 [tool.setuptools_scm]
 
 [tool.poetry]
 name = "rubrical"
-version = "0.1.2"
+version = "0.2.0"
 description = "A CLI to encourage (😅) people to update their dependencies!"
 authors = ["Ivan Lee <ivanklee86@gmail.com>"]
 license = "MPL-2.0"
 homepage = "https://github.com/ivanklee86/rubrical"
 repository = "https://github.com/ivanklee86/rubrical"
 readme = "README.md"
 classifiers=[
@@ -45,15 +45,15 @@
 [tool.poetry.scripts]
 rubrical = "rubrical.main:app"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 typer = {extras = ["all"], version = "^0.7.0"}
 pydantic = "^1.10.4"
-semver = "^2.13.0"
+semver = "^3.0.0"
 pygithub = "^1.58.0"
 python-benedict = {extras = ["all"], version = "^0.30.0"}
 pyyaml = "^6.0"
 requirements-parser = "^0.5.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.0.0"
@@ -65,15 +65,15 @@
 pytest-html = "^3.2.0"
 pytest-mock = "^3.10.0"
 pytest-xdist = "^3.0.2"
 setuptools-scm = "^7.0.5"
 twine = "^4.0.2"
 pre-commit = "^3.0.0"
 isort = "^5.10.1"
-ruff = "^0.0.260"
+ruff = "^0.0.262"
 python-dotenv = "^1.0.0"
 typer-cli = "^0.0.13"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "semver"
```

### Comparing `rubrical-0.1.2/rubrical/comparisons/__init__.py` & `rubrical-0.2.0/rubrical/comparisons/__init__.py`

 * *Files identical despite different names*

### Comparing `rubrical-0.1.2/rubrical/comparisons/string.py` & `rubrical-0.2.0/rubrical/comparisons/string.py`

 * *Files identical despite different names*

### Comparing `rubrical-0.1.2/rubrical/main.py` & `rubrical-0.2.0/rubrical/main.py`

 * *Files identical despite different names*

### Comparing `rubrical-0.1.2/rubrical/package_managers/base_package_manager.py` & `rubrical-0.2.0/rubrical/package_managers/python.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,48 +1,53 @@
-import abc
-from pathlib import Path
-from typing import Dict, List
+import requirements
 
-from rubrical.enum import DependencySpecifications
+from rubrical.enum import DependencySpecifications, SupportedPackageManagers
+from rubrical.package_managers.base_package_manager import BasePackageManager
 from rubrical.schemas.package import Package
 
 
-class BasePackageManager(abc.ABC):
-    name: str = ""
-    target_file: str = ""
-    found_files: Dict[str, str]
-    packages: Dict[str, List[Package]]
-    specification_symbols: Dict[str, List[str]] = {
-        DependencySpecifications.EQ.value: ["=="],
-        DependencySpecifications.GT.value: [">"],
-        DependencySpecifications.GTE.value: [">=", "=>"],
-        DependencySpecifications.LT.value: ["<"],
-        DependencySpecifications.LTE.value: ["<=", "=<"],
-        DependencySpecifications.NE.value: ["!="],
-        DependencySpecifications.COMPATIBLE.value: [],
-    }
+class Python(BasePackageManager):
+    target_files = ["requirements.txt"]
 
     def __init__(self) -> None:
         super().__init__()
 
-        self.found_files = {}
-        self.packages = {}
+        self.name = SupportedPackageManagers.PYTHON.value
 
-    def read_package_manager_files(self, current_folder: Path):
-        package_manager_files = current_folder.rglob(self.target_file)
-
-        for package_manager_file in package_manager_files:
-            with open(str(package_manager_file), "r") as file:
-                self.found_files[
-                    str(package_manager_file.relative_to(current_folder))
-                ] = file.read()
-
-    def parse_package_manager_files(self):
-        for file in self.found_files.items():
-            self.parse_package_manager_file(*file)
-
-    def append_package(self, package_file_filename: str, package: Package):
-        self.packages[package_file_filename].append(package)
-
-    @abc.abstractmethod
-    def parse_package_manager_file(self, package_file_filename: str, package_file: str):
-        pass
+        self.specification_symbols = self.specification_symbols | {
+            DependencySpecifications.APPROX_EQ.value: ["~="]
+        }
+
+    def _set_package(self, package_file_filename: str, requirement, spec):
+        for key, value in self.specification_symbols.items():
+            if spec[0] in value:
+                self.append_package(
+                    package_file_filename,
+                    Package(
+                        name=requirement.name,
+                        version=spec[1],
+                        specifier=DependencySpecifications(key),
+                    ),
+                )
+
+    def parse_package_manager_file(
+        self, package_file_filename: str, package_file_contents: str
+    ) -> None:
+        self.packages[package_file_filename] = []
+
+        for req in requirements.parse(package_file_contents):
+            if req.specifier:
+                # Handle cases for single specifiers.
+                if len(req.specs) == 1:
+                    [spec] = req.specs
+                    self._set_package(package_file_filename, req, spec)
+                elif len(req.specs) > 1:
+                    [spec] = [
+                        x
+                        for x in req.specs
+                        if x[0]
+                        in self.specification_symbols["GT"]
+                        + self.specification_symbols["GTE"]
+                    ]
+                    self._set_package(package_file_filename, req, spec)
+                else:
+                    pass
```

### Comparing `rubrical-0.1.2/rubrical/package_managers/jsonnet.py` & `rubrical-0.2.0/rubrical/package_managers/jsonnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 
 class JsonnetFile(BaseModel):
     dependencies: List[JsonnetDependency]
 
 
 class Jsonnet(BasePackageManager):
-    target_file = "jsonnetfile.json"
+    target_files = ["jsonnetfile.json"]
 
     def __init__(self) -> None:
         super().__init__()
 
         self.name = SupportedPackageManagers.JSONNET.value
 
     def parse_package_manager_file(
```

### Comparing `rubrical-0.1.2/rubrical/reporters/gh.py` & `rubrical-0.2.0/rubrical/reporters/gh.py`

 * *Files identical despite different names*

### Comparing `rubrical-0.1.2/rubrical/reporters/terminal.py` & `rubrical-0.2.0/rubrical/reporters/terminal.py`

 * *Files identical despite different names*

### Comparing `rubrical-0.1.2/rubrical/rubrical.py` & `rubrical-0.2.0/rubrical/rubrical.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 from pathlib import Path
 from typing import Dict, List, Tuple
 
 from rubrical.comparisons import check_package
 from rubrical.enum import PackageCheck, SupportedPackageManagers
 from rubrical.package_managers.base_package_manager import BasePackageManager
+from rubrical.package_managers.go import Go
 from rubrical.package_managers.jsonnet import Jsonnet
+from rubrical.package_managers.nodejs import NodeJS
 from rubrical.package_managers.python import Python
 from rubrical.reporters import terminal
 from rubrical.schemas.configuration import RubricalConfig
 from rubrical.schemas.results import PackageCheckResult
 from rubrical.utilities import console
 
 PACKAGE_MANAGER_MAPPING = {
     SupportedPackageManagers.JSONNET.value: Jsonnet,
     SupportedPackageManagers.PYTHON.value: Python,
+    SupportedPackageManagers.GO.value: Go,
+    SupportedPackageManagers.NODEJS.value: NodeJS,
 }
 
 
 class Rubrical:
     configuration: RubricalConfig
     package_managers: List[BasePackageManager]
     repository_path: Path
@@ -29,15 +33,15 @@
         self.configuration = configuration
         self.repository_path = repository_path
         self.debug = debug
         self.package_managers = []
 
         for package_manager in self.configuration.package_managers:
             self.package_managers.append(
-                PACKAGE_MANAGER_MAPPING[package_manager.name]()
+                PACKAGE_MANAGER_MAPPING[package_manager.name]()  #  type:  ignore
             )
 
     def check_package_managers(
         self,
     ) -> Tuple[bool, bool, Dict[str, List[PackageCheckResult]]]:
         warnings_found = False
         blocks_found = False
```

### Comparing `rubrical-0.1.2/rubrical/utilities/console.py` & `rubrical-0.2.0/rubrical/utilities/console.py`

 * *Files identical despite different names*

### Comparing `rubrical-0.1.2/PKG-INFO` & `rubrical-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubrical
-Version: 0.1.2
+Version: 0.2.0
 Summary: A CLI to encourage (😅) people to update their dependencies!
 Home-page: https://github.com/ivanklee86/rubrical
 License: MPL-2.0
 Author: Ivan Lee
 Author-email: ivanklee86@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -14,27 +14,29 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Build Tools
 Requires-Dist: pydantic (>=1.10.4,<2.0.0)
 Requires-Dist: pygithub (>=1.58.0,<2.0.0)
 Requires-Dist: python-benedict[all] (>=0.30.0,<0.31.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requirements-parser (>=0.5.0,<0.6.0)
-Requires-Dist: semver (>=2.13.0,<3.0.0)
+Requires-Dist: semver (>=3.0.0,<4.0.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Project-URL: Repository, https://github.com/ivanklee86/rubrical
 Description-Content-Type: text/markdown
 
 # rubrical
 
 [![CI](https://github.com/ivanklee86/rubrical/actions/workflows/ci.yaml/badge.svg)](https://github.com/ivanklee86/rubrical/actions/workflows/ci.yaml) [![codecov](https://codecov.io/gh/ivanklee86/rubrical/branch/main/graph/badge.svg?token=9WJM4LBDEX)](https://codecov.io/gh/ivanklee86/rubrical) [![PyPI version](https://badge.fury.io/py/rubrical.svg)](https://badge.fury.io/py/rubrical)
 
 A CLI to encourage (😅) people to update their dependencies!
 
 Supported package managers:
 * Python (requirements.txt)
+* Go (go.mod)
+* Node.js (package.lock)
 * Jsonnet
 * _More coming soon!_
 
 ![rubrical](docs/images/rubrical.png)
 
 ## Installation
 
@@ -74,24 +76,34 @@
 ## Configuration
 
 The `rubrical.yaml` file is used to configure checks for your application.
 
 ```yaml
 version: 1
 package_managers:
+  - name: jsonnet
+    packages:
+      - name: "xunleii/vector_jsonnet" # Name of the dependency
+        block: v0.1.0  # If dependency is older than this, error.
+        warn: v0.1.2  # If dependency is older than this, warn.
   - name: python
     packages:
       - name: Mopidy-Dirble
         block: v1.2.1
         warn: v1.2.2
-  - name: jsonnet
+  - name: go
     packages:
-      - name: "xunleii/vector_jsonnet" # Name of the dependency
-        block: v0.1.0  # If dependency is older than this, error.
-        warn: v0.1.2  # If dependency is older than this, warn.
+      - name: github.com/adrg/xdg
+        block: v0.5.0
+        warn: v0.6.0
+  - name: nodejs
+    packages:
+      - name: react
+        block: v17.0.3
+        warn: v17.0.4
 ```
 
 ## Reporting
 
 ### Terminal
 
 Comes for free!
```

