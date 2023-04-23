# Comparing `tmp/parasect-1.1.0.tar.gz` & `tmp/parasect-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parasect-1.1.0.tar", max compression
+gzip compressed data, was "parasect-1.1.1.tar", max compression
```

## Comparing `parasect-1.1.0.tar` & `parasect-1.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1080 2023-01-10 23:29:57.702714 parasect-1.1.0/LICENSE.rst
--rw-r--r--   0        0        0     4351 2023-01-10 23:29:57.702714 parasect-1.1.0/README.rst
--rw-r--r--   0        0        0     2196 2023-01-10 23:30:12.258722 parasect-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      193 2023-01-10 23:29:57.706714 parasect-1.1.0/src/parasect/__init__.py
--rw-r--r--   0        0        0     3502 2023-01-10 23:29:57.706714 parasect-1.1.0/src/parasect/__main__.py
--rw-r--r--   0        0        0    26127 2023-01-10 23:29:57.706714 parasect-1.1.0/src/parasect/_helpers.py
--rwxr-xr-x   0        0        0    28007 2023-01-10 23:29:57.706714 parasect-1.1.0/src/parasect/build_lib.py
--rwxr-xr-x   0        0        0    15184 2023-01-10 23:29:57.706714 parasect-1.1.0/src/parasect/compare_lib.py
--rw-r--r--   0        0        0        0 2023-01-10 23:29:57.706714 parasect-1.1.0/src/parasect/py.typed
--rw-r--r--   0        0        0     5463 1970-01-01 00:00:00.000000 parasect-1.1.0/setup.py
--rw-r--r--   0        0        0     5409 1970-01-01 00:00:00.000000 parasect-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-04-23 17:58:42.205257 parasect-1.1.1/LICENSE.rst
+-rw-r--r--   0        0        0     4351 2023-04-23 17:58:42.205257 parasect-1.1.1/README.rst
+-rw-r--r--   0        0        0     2234 2023-04-23 17:58:59.229601 parasect-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      193 2023-04-23 17:58:42.213257 parasect-1.1.1/src/parasect/__init__.py
+-rw-r--r--   0        0        0     3502 2023-04-23 17:58:42.213257 parasect-1.1.1/src/parasect/__main__.py
+-rw-r--r--   0        0        0    27529 2023-04-23 17:58:59.233601 parasect-1.1.1/src/parasect/_helpers.py
+-rwxr-xr-x   0        0        0    28187 2023-04-23 17:58:42.213257 parasect-1.1.1/src/parasect/build_lib.py
+-rwxr-xr-x   0        0        0    15184 2023-04-23 17:58:42.213257 parasect-1.1.1/src/parasect/compare_lib.py
+-rw-r--r--   0        0        0        0 2023-04-23 17:58:42.213257 parasect-1.1.1/src/parasect/py.typed
+-rw-r--r--   0        0        0     5430 1970-01-01 00:00:00.000000 parasect-1.1.1/setup.py
+-rw-r--r--   0        0        0     5362 1970-01-01 00:00:00.000000 parasect-1.1.1/PKG-INFO
```

### Comparing `parasect-1.1.0/LICENSE.rst` & `parasect-1.1.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `parasect-1.1.0/README.rst` & `parasect-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `parasect-1.1.0/pyproject.toml` & `parasect-1.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "parasect"
-version = "1.1.0"
+version = "1.1.1"
 description = "Utility for manipulating parameter sets for autopilots."
 authors = ["George Zogopoulos <geo.zogop.papal@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/AvyFly/parasect"
 repository = "https://github.com/AvyFly/parasect"
 documentation = "https://parasect.readthedocs.io"
@@ -17,44 +17,46 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 click = "^8.0.1"
 PyYAML = "^6.0"
 defusedxml = "^0.7.1"
 pydantic = "^1.9.1"
-directory-tree = "^0.0.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
-coverage = {extras = ["toml"], version = "^6.4"}
+coverage = {extras = ["toml"], version = "^7.2"}
 safety = "^2.2.0"
-mypy = "^0.961"
+mypy = "^1.0.1"
 typeguard = "^2.13.2"
 xdoctest = {extras = ["colors"], version = "^1.0.0"}
-sphinx = "^5.0.1"
+sphinx = "^6.1.3"
 sphinx-autobuild = ">=2021.3.14"
 pre-commit = "^2.15.0"
 flake8 = "^4.0.1"
 black = ">=21.10b0"
 flake8-bandit = "^3.0.0"
 flake8-bugbear = "^22.4.25"
 flake8-docstrings = "^1.6.0"
-flake8-rst-docstrings = "^0.2.6"
+flake8-rst-docstrings = "^0.3.0"
 pep8-naming = "^0.13.0"
 darglint = "^1.8.1"
 reorder-python-imports = "^3.1.0"
 pre-commit-hooks = "^4.3.0"
-sphinx-click = "^4.1.0"
+sphinx-click = "^4.4.0"
 Pygments = "^2.10.0"
-pyupgrade = "^2.34.0"
-furo = ">=2021.11.12"
+pyupgrade = "^3.3.1"
+furo = ">=2022.12.7"
 
 [tool.poetry.scripts]
 parasect = "parasect.__main__:cli"
 
+[tool.poetry.group.dev.dependencies]
+directory-tree = "^0.0.3.1"
+
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
 tests = ["tests", "*/tests"]
 
 [tool.coverage.run]
 branch = true
 source = ["parasect", "tests"]
```

### Comparing `parasect-1.1.0/src/parasect/__main__.py` & `parasect-1.1.1/src/parasect/__main__.py`

 * *Files identical despite different names*

### Comparing `parasect-1.1.0/src/parasect/_helpers.py` & `parasect-1.1.1/src/parasect/_helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -230,16 +230,16 @@
     substances: Optional[Substances]
     groups: Optional[Substances]
 
 
 class Recipe(BaseModel, extra="forbid"):
     """A set of ingredients and allergens."""
 
-    ingredients: Optional[Substances]
-    allergens: Optional[Allergens]
+    ingredients: Optional[Substances] = None
+    allergens: Optional[Allergens] = None
 
 
 class DishModel(BaseModel, extra="forbid"):
     """A complete dish."""
 
     common: Optional[Recipe]
     variants: Optional[Dict[str, "DishModel"]]
@@ -458,15 +458,15 @@
     max_value = float("inf")
     increment = None  # Instruction for increments for UIs
     unit = None
     decimal = None  # Suggested increment by the parameter documentation
     reboot_required = False
     group = None
     vid: int  # Vehicle ID, default 1
-    cid: int  # Componenet ID, default 1
+    cid: int  # Component ID, default 1
 
     def __init__(
         self,
         name: str,
         value: Union[int, float],
         param_type: Optional[str] = None,
         vid: int = 1,
@@ -544,50 +544,82 @@
     params: Dict[str, Parameter]
 
     def __init__(self, original: Optional["ParameterList"] = None):
         """Class constructor."""
         if not original:
             self.params = dict()
         else:
-            self.params = original.params
+            self.params = dict(original.params)
+
+    @classmethod
+    def build_param_hash_from_param(cls, p: Parameter) -> str:
+        """Build the params dictionary hash from a Parameter entry."""
+        return cls.build_param_hash(p.name, p.cid)
+
+    @staticmethod
+    def build_param_hash(name: str, cid: int) -> str:
+        """Build the params dictionary."""
+        return f"{name}:{cid}"
+
+    @staticmethod
+    def decode_parameter_hash(hash: str) -> Tuple[str, int]:
+        """Deduce parameter details from the hash."""
+        parts = hash.split(":")
+        name = parts[0]
+        if len(parts) == 1:
+            cid = 1
+        else:
+            cid = int(parts[1])
+        return name, cid
 
     def __iter__(self) -> Generator[Parameter, None, None]:
         """__iter__ dunder method."""
         for param_name in sorted(self.params.keys()):
             yield self.params[param_name]
 
     def __sub__(self, other: "ParameterList") -> "ParameterList":
         """Subtract a ParameterList from another ParameterList."""
         param_list = ParameterList(self)
         for param in param_list:
-            if param.name in other.keys():
+            param_hash = self.build_param_hash_from_param(param)
+            if param_hash in other.keys():
                 param_list.remove_param(param)
         return param_list
 
     def __str__(self) -> str:
         """__str__ dunder method."""
         param_strings = []
         for param_name in sorted(self.params.keys()):
             param_strings.append(self.params[param_name].__str__())
         return "\n".join(param_strings)
 
     def __len__(self) -> int:
         """__len__ dunder method."""
         return len(self.params)
 
-    def __getitem__(self, key: str) -> Parameter:
+    def __getitem__(self, key: Union[str, Tuple[str, int]]) -> Parameter:
         """__getitem__ dunder method."""
-        return self.params[key]
+        if isinstance(key, str):
+            # The key is only a parameter name. Assume cid == 1.
+            name, cid = self.decode_parameter_hash(key)
+        else:
+            # The cid is provided.
+            name, cid = key
+        param_hash = self.build_param_hash(name, cid)
+        return self.params[param_hash]
 
     def __contains__(self, item: Union[str, Parameter]) -> bool:
         """Answer if the parameter list contains a parameter."""
         if isinstance(item, str):
-            return item in self.params.keys()
+            # Assume cid == 1.
+            param_hash = self.build_param_hash(item, 1)
+            return param_hash in self.params.keys()
         else:  # item is Parameter
-            return item.name in self.params.keys()
+            param_hash = self.build_param_hash_from_param(item)
+            return param_hash in self.params.keys()
 
     def keys(self) -> KeysView:
         """__keys__ dunder method.
 
         It returns the names of the parameters it contains.
         """
         return self.params.keys()
@@ -596,43 +628,45 @@
         self, param: Parameter, safe: bool = False, overwrite: bool = True
     ) -> None:
         """Add a Parameter to the list."""
         # param: The parameter object
         # safe: allow adding new parameters
         # overwrite: allow overwriting existing parameters
         get_logger().debug(f"Attempting to add {param} to list")
-        if safe and param.name not in self.params.keys():
-            raise KeyError(f"{param.name} is not an existing key")
-        if not overwrite and param.name in self.params.keys():
-            raise KeyError(f"Tried to overwrite key {param.name}")
+        param_hash = self.build_param_hash_from_param(param)
+        if safe and param_hash not in self.params.keys():
+            raise KeyError(f"{param.name} with cid={param.cid} is not an existing key")
+        if not overwrite and param_hash in self.params.keys():
+            raise KeyError(f"Tried to overwrite key {param.name} with cid={param.cid}")
         # If parameter doesn't exist, create it
-        if param.name not in self.params:
-            self.params[param.name] = param
+        if param_hash not in self.params:
+            self.params[param_hash] = param
         # otherwise copy only the value
         else:
             # Try to deduce parameter type
             if param.param_type is not None:
                 # If we know the new parameter type
                 new_value = param.value
-            elif self.params[param.name].param_type is None:
+            elif self.params[param_hash].param_type is None:
                 # If we don't know the existing parameter type
                 new_value = param.value
             else:
                 # We know the target type, cast the new parameter value
-                param_type = self.params[param.name].param_type
+                param_type = self.params[param_hash].param_type
                 new_value = cast_param_value(param.value, param_type)
-            self.params[param.name].value = new_value
+            self.params[param_hash].value = new_value
 
     def remove_param(self, param: Parameter, safe: bool = True) -> None:
         """Remove a Parameter from the list."""
         # param: The parameter object
         # safe: don't try to remove not existing parameters
-        if safe and param.name not in self.params.keys():
-            raise KeyError(f"{param.name} is not an existing key")
-        self.params.pop(param.name, None)
+        param_hash = self.build_param_hash_from_param(param)
+        if safe and param_hash not in self.params.keys():
+            raise KeyError(f"{param.name} with cid={param.cid} is not an existing key")
+        self.params.pop(param_hash, None)
 
 
 # Construct parameters from structured input
 ############################################
 
 
 def build_param_from_xml(parameter: XmlElement) -> Parameter:
```

### Comparing `parasect-1.1.0/src/parasect/build_lib.py` & `parasect-1.1.1/src/parasect/build_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -511,29 +511,30 @@
     def export_to_px4(self) -> Generator[str, None, None]:
         """Export as PX4 parameter file."""
         # Read header
         get_logger().debug("Loading parameter header")
         header_model = get_boilerplate(ConfigPaths().staple_dishes, "header")
         yield from self.build_header_footer(header_model, self.header, "px4")
 
-        param_names = sorted(self.param_list.keys())
-        for param_name in param_names:
-            param_value = self.param_list[param_name].get_pretty_value()
-            internal_type = self.param_list[param_name].param_type
+        param_hashes = sorted(self.param_list.keys())
+        for param_hash in param_hashes:
+            param_name = self.param_list[param_hash].name
+            param_value = self.param_list[param_hash].get_pretty_value()
+            internal_type = self.param_list[param_hash].param_type
             if internal_type == "FLOAT":
                 param_type = 9
             elif internal_type == "INT32":
                 param_type = 6
             else:
                 raise TypeError(
                     f"Unknown parameter type {internal_type} for parameter {param_name}"
                 )
 
-            vid = self.param_list[param_name].vid
-            cid = self.param_list[param_name].cid
+            vid = self.param_list[param_hash].vid
+            cid = self.param_list[param_hash].cid
             yield f"{vid}\t{cid}\t{param_name}\t{param_value}\t{param_type}\n"
 
     def export_to_px4af(self, version: int) -> Generator[str, None, None]:
         """PX4 airframe file build helper."""
         # Diversivy versions
         if version == 1:
             directive = "set"
@@ -550,17 +551,18 @@
         yield from self.build_header_footer(header_dish, self.header, dish)
 
         if not self.is_sitl:
             indentation = "\t"
         else:
             indentation = ""
 
-        param_names = sorted(self.param_list.keys())
-        for param_name in param_names:
-            param_value = self.param_list[param_name].get_pretty_value()
+        param_hashes = sorted(self.param_list.keys())
+        for param_hash in param_hashes:
+            param_name = self.param_list[param_hash].name
+            param_value = self.param_list[param_hash].get_pretty_value()
 
             yield f"{indentation}param {directive} {param_name} {param_value}\n"
 
         # Read footer
         get_logger().debug("Loading parameter footer.")
         footer_dict = get_boilerplate(ConfigPaths().staple_dishes, "footer")
         yield from self.build_header_footer(footer_dict, self.footer, dish)
@@ -584,16 +586,17 @@
         # Read header
         get_logger().debug("Loading parameter header.")
         header_dish = get_boilerplate(ConfigPaths().staple_dishes, "header")
         yield from self.build_header_footer(header_dish, self.header, "csv")
 
         indentation = ""
 
-        param_names = sorted(self.param_list.keys())
-        for param_name in param_names:
+        param_hashes = sorted(self.param_list.keys())
+        for param_name in param_hashes:
+            param_name = self.param_list[param_name].name
             param_value = self.param_list[param_name].get_pretty_value()
 
             yield f"{indentation}{param_name},{param_value}\n"
 
         # Read footer
         get_logger().debug("Loading parameter footer.")
         footer_dict = get_boilerplate(ConfigPaths().staple_dishes, "footer")
```

### Comparing `parasect-1.1.0/src/parasect/compare_lib.py` & `parasect-1.1.1/src/parasect/compare_lib.py`

 * *Files identical despite different names*

### Comparing `parasect-1.1.0/setup.py` & `parasect-1.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,23 +10,22 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['PyYAML>=6.0,<7.0',
  'click>=8.0.1,<9.0.0',
  'defusedxml>=0.7.1,<0.8.0',
- 'directory-tree>=0.0.2,<0.0.3',
  'pydantic>=1.9.1,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['parasect = parasect.__main__:cli']}
 
 setup_kwargs = {
     'name': 'parasect',
-    'version': '1.1.0',
+    'version': '1.1.1',
     'description': 'Utility for manipulating parameter sets for autopilots.',
     'long_description': "Parasect\n========\n\n.. badges-begin\n\n|PyPI| |Status| |Python Version| |License|\n\n|Read the Docs| |Tests| |Codecov|\n\n|pre-commit| |Black|\n\n.. |PyPI| image:: https://img.shields.io/pypi/v/parasect.svg\n   :target: https://pypi.org/project/parasect/\n   :alt: PyPI\n.. |Status| image:: https://img.shields.io/pypi/status/parasect.svg\n   :target: https://pypi.org/project/parasect/\n   :alt: Status\n.. |Python Version| image:: https://img.shields.io/pypi/pyversions/parasect\n   :target: https://pypi.org/project/parasect\n   :alt: Python Version\n.. |License| image:: https://img.shields.io/github/license/AvyFly/parasect\n   :target: https://opensource.org/licenses/MIT\n   :alt: License\n.. |Read the Docs| image:: https://img.shields.io/readthedocs/parasect/latest.svg?label=Read%20the%20Docs\n   :target: https://parasect.readthedocs.io/\n   :alt: Read the documentation at https://parasect.readthedocs.io/\n.. |Tests| image:: https://github.com/AvyFly/parasect/workflows/Tests/badge.svg\n   :target: https://github.com/AvyFly/parasect/actions?workflow=Tests\n   :alt: Tests\n.. |Codecov| image:: https://codecov.io/gh/AvyFly/parasect/branch/master/graph/badge.svg\n   :target: https://codecov.io/gh/AvyFly/parasect\n   :alt: Codecov\n.. |pre-commit| image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white\n   :target: https://github.com/pre-commit/pre-commit\n   :alt: pre-commit\n.. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg\n   :target: https://github.com/psf/black\n   :alt: Black\n\n.. badges-end\n\n.. image:: docs/_static/logo.svg\n   :alt: parasect logo\n   :width: 320\n   :align: center\n\n.. logo-end\n\n\nWelcome to *Parasect*, a utility for manipulating parameter sets for autopilots!\n\nFeatures\n--------\n\n*Parasect* has two-fold capabilities:\n\n1. Compare two parameter sets and highlighting their differences.\n2. Parsing from user-defined content and generating new parameter sets, ready for loading into an autopilot.\n\nList of currently supported autopilots:\n\n* PX4_\n\nRequirements\n------------\n\n*Parasect* is a pure-Python project. Its requirements are managed by the Poetry_ dependency manager.\nWhen you install *Parasect* via pip_ its requirements will also be installed automatically.\n\nCurrently *Parasect* has been tested:\n\n* in Continuous Integration servers for **Ubuntu Linux**, **Windows**\n* manually in **Ubuntu Linux**.\n\n\nInstallation\n------------\n\nYou can install *Parasect* via pip_ from PyPI_:\n\n.. code:: console\n\n   $ pip install parasect\n\n\nUsage\n-----\n\n*Parasect* is primarily used as a command-line program.\nIn its simplest form, two parameter files can be compared via:\n\n.. code:: console\n\n   $ parasect compare <FILE_1> <FILE_2>\n\nThe usage for building parameter sets is more involved.\nPlease see the `Command-line Reference <CLI usage_>`_ for details.\n\nAdditionally, it exposes a minimal API, enabling automated operations.\nThis is described in the `API Reference <API usage_>`_.\n\nIt is strongly recommended that you read the Concepts_ that *Parasect* employs, if you plan to make full use of it.\n\n\nContributing\n------------\n\nContributions are very welcome.\nTo learn more, see the `Contributor Guide`_.\n\n\nLicense\n-------\n\nDistributed under the terms of the `MIT license`_,\n*Parasect* is free and open source software.\n\n\nIssues\n------\n\nIf you encounter any problems,\nplease `file an issue`_ along with a detailed description.\n\n\nCredits\n-------\n\nThis project was sponsored by `Avy B.V. <Avy_>`_, a UAV company in Amsterdam.\n\nThis project was generated from `@cjolowicz`_'s `Hypermodern Python Cookiecutter`_ template.\n\n.. _@cjolowicz: https://github.com/cjolowicz\n.. _Cookiecutter: https://github.com/audreyr/cookiecutter\n.. _MIT license: https://opensource.org/licenses/MIT\n.. _PyPI: https://pypi.org/\n.. _Hypermodern Python Cookiecutter: https://github.com/cjolowicz/cookiecutter-hypermodern-python\n.. _file an issue: https://github.com/AvyFly/parasect/issues\n.. _pip: https://pip.pypa.io/\n.. _CLI usage: https://parasect.readthedocs.io/en/latest/reference.html#cli-reference\n.. _API usage: https://parasect.readthedocs.io/en/latest/reference.html#api-reference\n.. _Concepts: https://parasect.readthedocs.io/en/latest/concepts.html\n.. _PX4: https://px4.io/\n.. _Poetry: https://python-poetry.org/\n.. _Avy: https://avy.eu\n.. github-only\n.. _Contributor Guide: CONTRIBUTING.rst\n",
     'author': 'George Zogopoulos',
     'author_email': 'geo.zogop.papal@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/AvyFly/parasect',
```

### Comparing `parasect-1.1.0/PKG-INFO` & `parasect-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parasect
-Version: 1.1.0
+Version: 1.1.1
 Summary: Utility for manipulating parameter sets for autopilots.
 Home-page: https://github.com/AvyFly/parasect
 License: MIT
 Author: George Zogopoulos
 Author-email: geo.zogop.papal@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,15 +13,14 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: click (>=8.0.1,<9.0.0)
 Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
-Requires-Dist: directory-tree (>=0.0.2,<0.0.3)
 Requires-Dist: pydantic (>=1.9.1,<2.0.0)
 Project-URL: Changelog, https://github.com/AvyFly/parasect/releases
 Project-URL: Documentation, https://parasect.readthedocs.io
 Project-URL: Repository, https://github.com/AvyFly/parasect
 Description-Content-Type: text/x-rst
 
 Parasect
```

