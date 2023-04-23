# Comparing `tmp/cppython-vcpkg-0.4.1.dev8.tar.gz` & `tmp/cppython-vcpkg-0.4.1.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cppython-vcpkg-0.4.1.dev8.tar", last modified: Sun Oct 16 12:54:31 2022, max compression
+gzip compressed data, was "cppython-vcpkg-0.4.1.dev9.tar", last modified: Sun Oct 16 17:00:12 2022, max compression
```

## Comparing `cppython-vcpkg-0.4.1.dev8.tar` & `cppython-vcpkg-0.4.1.dev9.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-10-16 12:54:14.977336 cppython-vcpkg-0.4.1.dev8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-10-16 12:54:14.977336 cppython-vcpkg-0.4.1.dev8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)        3 2022-10-16 12:54:14.977336 cppython-vcpkg-0.4.1.dev8/cppython_vcpkg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8969 2022-10-16 12:54:14.977336 cppython-vcpkg-0.4.1.dev8/cppython_vcpkg/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-16 12:54:14.977336 cppython-vcpkg-0.4.1.dev8/cppython_vcpkg/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-10-16 12:54:14.977336 cppython-vcpkg-0.4.1.dev8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)        3 2022-10-16 12:54:14.977336 cppython-vcpkg-0.4.1.dev8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        3 2022-10-16 12:54:14.977336 cppython-vcpkg-0.4.1.dev8/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      841 2022-10-16 12:54:14.977336 cppython-vcpkg-0.4.1.dev8/tests/integration/test_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)        3 2022-10-16 12:54:14.977336 cppython-vcpkg-0.4.1.dev8/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      822 2022-10-16 12:54:14.977336 cppython-vcpkg-0.4.1.dev8/tests/unit/test_provider.py
--rw-------   0 runner    (1001) docker     (121)      519 2022-10-16 12:54:31.497410 cppython-vcpkg-0.4.1.dev8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-10-16 17:00:00.978758 cppython-vcpkg-0.4.1.dev9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (121)       92 2022-10-16 17:00:00.978758 cppython-vcpkg-0.4.1.dev9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)        3 2022-10-16 17:00:00.978758 cppython-vcpkg-0.4.1.dev9/cppython_vcpkg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6441 2022-10-16 17:00:00.978758 cppython-vcpkg-0.4.1.dev9/cppython_vcpkg/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-16 17:00:00.978758 cppython-vcpkg-0.4.1.dev9/cppython_vcpkg/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)     1883 2022-10-16 17:00:00.978758 cppython-vcpkg-0.4.1.dev9/cppython_vcpkg/resolution.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1031 2022-10-16 17:00:00.978758 cppython-vcpkg-0.4.1.dev9/cppython_vcpkg/schema.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-10-16 17:00:00.978758 cppython-vcpkg-0.4.1.dev9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)        3 2022-10-16 17:00:00.982758 cppython-vcpkg-0.4.1.dev9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)        3 2022-10-16 17:00:00.982758 cppython-vcpkg-0.4.1.dev9/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      841 2022-10-16 17:00:00.982758 cppython-vcpkg-0.4.1.dev9/tests/integration/test_provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)        3 2022-10-16 17:00:00.982758 cppython-vcpkg-0.4.1.dev9/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1198 2022-10-16 17:00:00.982758 cppython-vcpkg-0.4.1.dev9/tests/unit/test_provider.py
+-rw-------   0 runner    (1001) docker     (121)      519 2022-10-16 17:00:12.414902 cppython-vcpkg-0.4.1.dev9/PKG-INFO
```

### Comparing `cppython-vcpkg-0.4.1.dev8/LICENSE.md` & `cppython-vcpkg-0.4.1.dev9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cppython-vcpkg-0.4.1.dev8/cppython_vcpkg/plugin.py` & `cppython-vcpkg-0.4.1.dev9/cppython_vcpkg/plugin.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,93 +4,28 @@
 import json
 from os import name as system_name
 from pathlib import Path, PosixPath, WindowsPath
 from typing import Any
 
 from cppython_core.exceptions import ProcessError
 from cppython_core.plugin_schema.provider import Provider, ProviderData
-from cppython_core.schema import CorePluginData, CPPythonModel
+from cppython_core.schema import CorePluginData
 from cppython_core.utility import subprocess_call
-from pydantic import Field, HttpUrl
-from pydantic.types import DirectoryPath
 
-
-class VcpkgDataResolved(CPPythonModel):
-    """Resolved vcpkg data"""
-
-    install_path: DirectoryPath
-    manifest_path: DirectoryPath
-
-
-class VcpkgData(CPPythonModel):
-    """vcpkg provider data"""
-
-    install_path: Path = Field(
-        default=Path("build"),
-        alias="install-path",
-        description="The referenced dependencies defined by the local vcpkg.json manifest file",
-    )
-
-    manifest_path: Path = Field(
-        default=Path(), alias="manifest-path", description="The directory to store the manifest file, vcpkg.json"
-    )
-
-
-class VcpkgDependency(CPPythonModel):
-    """Vcpkg dependency type"""
-
-    name: str
-
-
-class Manifest(CPPythonModel):
-    """The manifest schema"""
-
-    name: str
-
-    version: str
-    homepage: HttpUrl | None = Field(default=None)
-    dependencies: list[VcpkgDependency] = Field(default=[])
+from cppython_vcpkg.resolution import generate_manifest, resolve_vcpkg_data
 
 
 class VcpkgProvider(Provider):
     """vcpkg Provider"""
 
     def __init__(self, group_data: ProviderData, core_data: CorePluginData) -> None:
         super().__init__(group_data, core_data)
 
         # Default the provider data
-        self.data = self._resolve_data(VcpkgData())
-
-    def _resolve_data(self, data: VcpkgData) -> VcpkgDataResolved:
-        """_summary_
-
-        Args:
-            data: _description_
-
-        Returns:
-            _description_
-        """
-
-        root_directory = self.core_data.project_data.pyproject_file.parent.absolute()
-
-        modified_install_path = data.install_path
-        modified_manifest_path = data.manifest_path
-
-        # Add the project location to all relative paths
-        if not modified_install_path.is_absolute():
-            modified_install_path = root_directory / modified_install_path
-
-        if not modified_manifest_path.is_absolute():
-            modified_manifest_path = root_directory / modified_manifest_path
-
-        # Create directories
-        modified_install_path.mkdir(parents=True, exist_ok=True)
-        modified_manifest_path.mkdir(parents=True, exist_ok=True)
-
-        return VcpkgDataResolved(install_path=modified_install_path, manifest_path=modified_manifest_path)
+        self.data = resolve_vcpkg_data({}, core_data)
 
     @classmethod
     def _update_provider(cls, path: Path) -> None:
         """Calls the vcpkg tool install script
 
         Args:
             path: The path where the script is located
@@ -103,33 +38,14 @@
                 subprocess_call(
                     ["./" + str(PosixPath("bootstrap-vcpkg.sh"))], logger=cls.logger(), cwd=path, shell=True
                 )
         except ProcessError:
             cls.logger().error("Unable to bootstrap the vcpkg repository", exc_info=True)
             raise
 
-    def _extract_manifest(self) -> Manifest:
-        """From the input configuration data, construct a Vcpkg specific Manifest type
-
-        Returns:
-            The manifest
-        """
-        base_dependencies = self.core_data.cppython_data.dependencies
-
-        vcpkg_dependencies: list[VcpkgDependency] = []
-        for dependency in base_dependencies:
-            vcpkg_dependency = VcpkgDependency(name=dependency.name)
-            vcpkg_dependencies.append(vcpkg_dependency)
-
-        return Manifest(
-            name=self.core_data.pep621_data.name,
-            version=self.core_data.pep621_data.version,
-            dependencies=vcpkg_dependencies,
-        )
-
     @staticmethod
     def name() -> str:
         """The string that is matched with the [tool.cppython.provider] string
 
         Returns:
             Plugin name
         """
@@ -138,17 +54,15 @@
     def activate(self, data: dict[str, Any]) -> None:
         """_summary_
 
         Args:
             data: _description_
         """
 
-        input_data = VcpkgData(**data)
-
-        self.data = self._resolve_data(input_data)
+        self.data = resolve_vcpkg_data(data, self.core_data)
 
     def supports_generator(self, name: str) -> bool:
         """_summary_
 
         Args:
             name: _description_
 
@@ -161,15 +75,15 @@
 
         return False
 
     def gather_input(self, name: str) -> Any:
         return None
 
     @classmethod
-    def tooling_downloaded(cls, path: DirectoryPath) -> bool:
+    def tooling_downloaded(cls, path: Path) -> bool:
         """Returns whether the provider tooling needs to be downloaded
 
         Args:
             path: The directory to check for downloaded tooling
 
         Raises:
             ProcessError: Failed vcpkg calls
@@ -189,15 +103,15 @@
 
         except ProcessError:
             return False
 
         return True
 
     @classmethod
-    async def download_tooling(cls, path: DirectoryPath) -> None:
+    async def download_tooling(cls, path: Path) -> None:
         """Installs the external tooling required by the provider
 
         Args:
             path: The directory to download any extra tooling to
 
         Raises:
             ProcessError: Failed vcpkg calls
@@ -230,15 +144,15 @@
     def install(self) -> None:
         """Called when dependencies need to be installed from a lock file.
 
         Raises:
             ProcessError: Failed vcpkg calls
         """
         manifest_path = self.data.manifest_path
-        manifest = self._extract_manifest()
+        manifest = generate_manifest(self.core_data)
 
         # Write out the manifest
         serialized = json.loads(manifest.json(exclude_none=True))
         with open(manifest_path / "vcpkg.json", "w", encoding="utf8") as file:
             json.dump(serialized, file, ensure_ascii=False, indent=4)
 
         executable = self.core_data.cppython_data.install_path / "vcpkg"
@@ -261,15 +175,15 @@
     def update(self) -> None:
         """Called when dependencies need to be updated and written to the lock file.
 
         Raises:
             ProcessError: Failed vcpkg calls
         """
         manifest_path = self.data.manifest_path
-        manifest = self._extract_manifest()
+        manifest = generate_manifest(self.core_data)
 
         # Write out the manifest
         serialized = json.loads(manifest.json(exclude_none=True))
         with open(manifest_path / "vcpkg.json", "w", encoding="utf8") as file:
             json.dump(serialized, file, ensure_ascii=False, indent=4)
 
         executable = self.core_data.cppython_data.install_path / "vcpkg"
```

### Comparing `cppython-vcpkg-0.4.1.dev8/pyproject.toml` & `cppython-vcpkg-0.4.1.dev9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ]
 readme = "README.md"
 dynamic = []
 requires-python = ">=3.10"
 dependencies = [
     "cppython-core>=0.3.3.dev0",
 ]
-version = "0.4.1.dev8"
+version = "0.4.1.dev9"
 
 [project.license-files]
 paths = [
     "LICENSE.md",
 ]
 
 [project.urls]
```

### Comparing `cppython-vcpkg-0.4.1.dev8/tests/integration/test_provider.py` & `cppython-vcpkg-0.4.1.dev9/tests/integration/test_provider.py`

 * *Files identical despite different names*

### Comparing `cppython-vcpkg-0.4.1.dev8/PKG-INFO` & `cppython-vcpkg-0.4.1.dev9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cppython-vcpkg
-Version: 0.4.1.dev8
+Version: 0.4.1.dev9
 Summary: A plugin for CPPython that enables vcpkg support for CMake projects
 License: MIT
 Author-email: Synodic Software <contact@synodic.software>
 Requires-Python: >=3.10
 Project-URL: homepage, https://github.com/Synodic-Software/CPPython-Vcpkg
 Project-URL: repository, https://github.com/Synodic-Software/CPPython-Vcpkg
 Description-Content-Type: text/markdown
```

