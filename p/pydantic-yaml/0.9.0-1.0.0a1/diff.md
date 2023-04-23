# Comparing `tmp/pydantic_yaml-0.9.0.tar.gz` & `tmp/pydantic_yaml-1.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_yaml-0.9.0.tar", last modified: Wed Jan  4 20:56:30 2023, max compression
+gzip compressed data, was "pydantic_yaml-1.0.0a1.tar", last modified: Sun Apr 23 21:25:57 2023, max compression
```

## Comparing `pydantic_yaml-0.9.0.tar` & `pydantic_yaml-1.0.0a1.tar`

### file list

```diff
@@ -1,44 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 20:56:30.442383 pydantic_yaml-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-01-04 20:56:10.000000 pydantic_yaml-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-01-04 20:56:30.442383 pydantic_yaml-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-01-04 20:56:10.000000 pydantic_yaml-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 20:56:30.438383 pydantic_yaml-0.9.0/pydantic_yaml/
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-01-04 20:56:10.000000 pydantic_yaml-0.9.0/pydantic_yaml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 20:56:30.442383 pydantic_yaml-0.9.0/pydantic_yaml/compat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-04 20:56:10.000000 pydantic_yaml-0.9.0/pydantic_yaml/compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-01-04 20:56:10.000000 pydantic_yaml-0.9.0/pydantic_yaml/compat/hacks.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-01-04 20:56:10.000000 pydantic_yaml-0.9.0/pydantic_yaml/compat/old_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-01-04 20:56:10.000000 pydantic_yaml-0.9.0/pydantic_yaml/compat/representers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-01-04 20:56:10.000000 pydantic_yaml-0.9.0/pydantic_yaml/compat/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-01-04 20:56:10.000000 pydantic_yaml-0.9.0/pydantic_yaml/compat/yaml_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 20:56:30.442383 pydantic_yaml-0.9.0/pydantic_yaml/ext/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-01-04 20:56:10.000000 pydantic_yaml-0.9.0/pydantic_yaml/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-01-04 20:56:10.000000 pydantic_yaml-0.9.0/pydantic_yaml/ext/semver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-01-04 20:56:10.000000 pydantic_yaml-0.9.0/pydantic_yaml/ext/versioned_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-01-04 20:56:10.000000 pydantic_yaml-0.9.0/pydantic_yaml/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     9174 2023-01-04 20:56:10.000000 pydantic_yaml-0.9.0/pydantic_yaml/mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-01-04 20:56:10.000000 pydantic_yaml-0.9.0/pydantic_yaml/model.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-01-04 20:56:10.000000 pydantic_yaml-0.9.0/pydantic_yaml/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 20:56:30.442383 pydantic_yaml-0.9.0/pydantic_yaml/test/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-01-04 20:56:10.000000 pydantic_yaml-0.9.0/pydantic_yaml/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-01-04 20:56:10.000000 pydantic_yaml-0.9.0/pydantic_yaml/test/recursive.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-01-04 20:56:10.000000 pydantic_yaml-0.9.0/pydantic_yaml/test/test_advanced_yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-01-04 20:56:10.000000 pydantic_yaml-0.9.0/pydantic_yaml/test/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-01-04 20:56:10.000000 pydantic_yaml-0.9.0/pydantic_yaml/test/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-01-04 20:56:10.000000 pydantic_yaml-0.9.0/pydantic_yaml/test/test_resursive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-01-04 20:56:10.000000 pydantic_yaml-0.9.0/pydantic_yaml/test/test_secret_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-01-04 20:56:10.000000 pydantic_yaml-0.9.0/pydantic_yaml/test/test_sorting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-01-04 20:56:10.000000 pydantic_yaml-0.9.0/pydantic_yaml/test/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-01-04 20:56:10.000000 pydantic_yaml-0.9.0/pydantic_yaml/test/test_versioned.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-01-04 20:56:10.000000 pydantic_yaml-0.9.0/pydantic_yaml/test/versioned.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-04 20:56:10.000000 pydantic_yaml-0.9.0/pydantic_yaml/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 20:56:30.442383 pydantic_yaml-0.9.0/pydantic_yaml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-01-04 20:56:30.000000 pydantic_yaml-0.9.0/pydantic_yaml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-01-04 20:56:30.000000 pydantic_yaml-0.9.0/pydantic_yaml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-04 20:56:30.000000 pydantic_yaml-0.9.0/pydantic_yaml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-04 20:56:22.000000 pydantic_yaml-0.9.0/pydantic_yaml.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-01-04 20:56:30.000000 pydantic_yaml-0.9.0/pydantic_yaml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-01-04 20:56:30.000000 pydantic_yaml-0.9.0/pydantic_yaml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-01-04 20:56:10.000000 pydantic_yaml-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-01-04 20:56:30.442383 pydantic_yaml-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-01-04 20:56:10.000000 pydantic_yaml-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:25:57.226184 pydantic_yaml-1.0.0a1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:25:57.222184 pydantic_yaml-1.0.0a1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:25:57.222184 pydantic_yaml-1.0.0a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/.github/workflows/python-testing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-04-23 21:25:57.226184 pydantic_yaml-1.0.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:25:57.222184 pydantic_yaml-1.0.0a1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/docs/installing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/docs/versioned.md
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 21:25:57.226184 pydantic_yaml-1.0.0a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:25:57.222184 pydantic_yaml-1.0.0a1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:25:57.222184 pydantic_yaml-1.0.0a1/src/pydantic_yaml/
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/src/pydantic_yaml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:25:57.226184 pydantic_yaml-1.0.0a1/src/pydantic_yaml/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/src/pydantic_yaml/deprecated/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/src/pydantic_yaml/dumper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:25:57.226184 pydantic_yaml-1.0.0a1/src/pydantic_yaml/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:25:57.226184 pydantic_yaml-1.0.0a1/src/pydantic_yaml/examples/base_models/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/src/pydantic_yaml/examples/base_models/a-1.1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/src/pydantic_yaml/examples/base_models/a-1.2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/src/pydantic_yaml/examples/base_models/a.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/src/pydantic_yaml/examples/base_models/b.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/src/pydantic_yaml/examples/base_models/has_enums.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/src/pydantic_yaml/examples/base_models/recursive.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/src/pydantic_yaml/examples/base_models/root_list_obj.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/src/pydantic_yaml/examples/base_models/root_list_str.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/src/pydantic_yaml/examples/base_models/uses_refs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/src/pydantic_yaml/examples/base_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/src/pydantic_yaml/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/src/pydantic_yaml/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/src/pydantic_yaml/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:25:57.226184 pydantic_yaml-1.0.0a1/src/pydantic_yaml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-04-23 21:25:57.000000 pydantic_yaml-1.0.0a1/src/pydantic_yaml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-23 21:25:57.000000 pydantic_yaml-1.0.0a1/src/pydantic_yaml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 21:25:57.000000 pydantic_yaml-1.0.0a1/src/pydantic_yaml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 21:25:40.000000 pydantic_yaml-1.0.0a1/src/pydantic_yaml.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-23 21:25:57.000000 pydantic_yaml-1.0.0a1/src/pydantic_yaml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-23 21:25:57.000000 pydantic_yaml-1.0.0a1/src/pydantic_yaml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:25:57.226184 pydantic_yaml-1.0.0a1/src/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/src/test/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/src/test/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/src/test/test_failures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/src/test/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/src/test/test_readme.py
```

### Comparing `pydantic_yaml-0.9.0/LICENSE` & `pydantic_yaml-1.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_yaml-0.9.0/README.md` & `pydantic_yaml-1.0.0a1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,163 +1,142 @@
-# pydantic-yaml
+Metadata-Version: 2.1
+Name: pydantic_yaml
+Version: 1.0.0a1
+Summary: Adds some YAML functionality to the excellent `pydantic` library.
+Author-email: NowanIlfideme <git@nowan.dev>
+License: MIT License
+        
+        Copyright (c) 2020 Anatoly Makarevich
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: github, https://github.com/NowanIlfideme/pydantic-yaml
+Project-URL: docs, https://pydantic-yaml.readthedocs.io/en/latest/
+Keywords: pydantic,yaml
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: Software Development
+Classifier: Typing :: Typed
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: docs
+License-File: LICENSE
+
+# Pydantic-YAML
 
 [![PyPI version](https://badge.fury.io/py/pydantic-yaml.svg)](https://badge.fury.io/py/pydantic-yaml) [![Documentation Status](https://readthedocs.org/projects/pydantic-yaml/badge/?version=latest)](https://pydantic-yaml.readthedocs.io/en/latest/?badge=latest)
  [![Unit Tests](https://github.com/NowanIlfideme/pydantic-yaml/actions/workflows/python-testing.yml/badge.svg)](https://github.com/NowanIlfideme/pydantic-yaml/actions/workflows/python-testing.yml)
 
-This is a small helper library that adds some YAML capabilities to [pydantic](https://github.com/samuelcolvin/pydantic), namely dumping to yaml via the `yaml_model.yaml()` function, and parsing from strings/files using `YamlModel.parse_raw()` and `YamlModel.parse_file()`. It also adds `Enum` subclasses that get dumped to YAML as strings or integers, and fixes dumping of some typical types.
+Pydantic-YAML adds YAML capabilities to [Pydantic](https://pydantic-docs.helpmanual.io/),
+which is an _excellent_ Python library for data validation and settings management.
+If you aren't familiar with Pydantic, I would suggest you first check out their
+[docs](https://pydantic-docs.helpmanual.io/).
 
 [Documentation on ReadTheDocs.org](https://pydantic-yaml.readthedocs.io/en/latest/)
 
 ## Basic Usage
 
-Typical usage is seen below. See the [pydantic docs](https://pydantic-docs.helpmanual.io/)
-for more usage examples.
-
 ```python
+from enum import Enum
 from pydantic import BaseModel, validator
-from pydantic_yaml import YamlStrEnum, YamlModel
+from pydantic_yaml import parse_yaml_raw_as, to_yaml_str
 
+class MyEnum(str, Enum):
+    """A custom enumeration that is YAML-safe."""
 
-class MyEnum(YamlStrEnum):
-    """This is a custom enumeration that is YAML-safe."""
-    
     a = "a"
     b = "b"
 
 class InnerModel(BaseModel):
-    """This is a normal pydantic model that can be used as an inner class."""
-    
+    """A normal pydantic model that can be used as an inner class."""
+
     fld: float = 1.0
 
-class MyModel(YamlModel):
-    """This is our custom class, with a `.yaml()` method.
-    
-    The `parse_raw()` and `parse_file()` methods are also updated to be able to
-    handle `content_type='application/yaml'`, `protocol="yaml"` and file names
-    ending with `.yml`/`.yaml`
-    """
+class MyModel(BaseModel):
+    """Our custom Pydantic model."""
 
     x: int = 1
     e: MyEnum = MyEnum.a
     m: InnerModel = InnerModel()
 
-    @validator('x')
+    @validator("x")
     def _chk_x(cls, v: int) -> int:  # noqa
         """You can add your normal pydantic validators, like this one."""
         assert v > 0
         return v
 
 m1 = MyModel(x=2, e="b", m=InnerModel(fld=1.5))
 
 # This dumps to YAML and JSON respectively
-yml = m1.yaml()
+yml = to_yaml_str(m1)
 jsn = m1.json()
 
-m2 = MyModel.parse_raw(yml)  # This automatically assumes YAML
+# This parses YAML as the MyModel type
+m2 = parse_yaml_raw_as(MyModel, yml)
 assert m1 == m2
 
-m3 = MyModel.parse_raw(jsn)  # This will fallback to JSON
+# JSON is also valid YAML, so this works too
+m3 = parse_yaml_raw_as(MyModel, jsn)
 assert m1 == m3
 
-m4 = MyModel.parse_raw(yml, proto="yaml")
-assert m1 == m4
-
-m5 = MyModel.parse_raw(yml, content_type="application/yaml")
-assert m1 == m5
-```
-
-## Installation
-
-`pip install pydantic_yaml`
-
-Make sure to install `ruamel.yaml` or `pyyaml` as well. These are optional dependencies:
-
-`pip install pydantic_yaml[ruamel]`
-
-`pip install pydantic_yaml[pyyaml]`
-
-## Mixin Class
-
-Version 0.5.0 adds a `YamlModelMixin` which can be used to add YAML functionality on
-top of, or alongside, other base classes:
-
-```python
-from typing import List
-
-from pydantic import BaseModel
-from pydantic_yaml import YamlModelMixin
-
-
-class MyBase(BaseModel):
-    """This is a normal."""
-    x: str = "x"
-
-class ExtModel(YamlModelMixin, MyBase):
-    """This model can be sent to/read from YAML."""
-    y: List[int] = [1, 2, 3]  # and you can define additional fields, if you want
 ```
 
-Note that this `YamlModelMixin` must be **before** any `BaseModel`-derived classes.
-This will hopefully be resolved in Pydantic 2.0
-(see [this discussion](https://github.com/samuelcolvin/pydantic/discussions/3025)
-for more details). If you know a better way of implementing this, please make raise
-an issue or create a PR!
-
 ## Configuration
 
-You can configure the function used to dump and load the YAML by using the `Config`
-inner class, [as in Pydantic](https://pydantic-docs.helpmanual.io/usage/model_config/):
+Currently we use the JSON dumping of Pydantic to perform most of the magic.
+
+This uses the `Config` inner class,
+[as in Pydantic](https://pydantic-docs.helpmanual.io/usage/model_config/):
 
 ```python
-class MyModel(YamlModel):
+class MyModel(BaseModel):
     # ...
     class Config:
-        # You can override these fields:
-        yaml_dumps = my_custom_dumper
-        yaml_loads = lambda x: MyModel()
+        # You can override these fields, which affect JSON and YAML:
+        json_dumps = my_custom_dumper
+        json_loads = lambda x: MyModel()
         # As well as other Pydantic configuration:
         allow_mutation = False
 ```
 
-## Versioned Models
-
-Since YAML is often used for config files, there is also a `SemVer` str-like class and `VersionedYamlModel` base class.
-
-The `version` attribute is parsed according to the SemVer
-([Semantic Versioning](https://semver.org/)) specification.
-It's constrained between the `min_version` and `max_version` specified by your models'
-`Config` inner class (similar to regular `pydantic` models).
-
-### Usage example
+A separate configuration for YAML specifically will be added later.
 
 ```python
-from pydantic import ValidationError
-from pydantic_yaml import SemVer, VersionedYamlModel
+# TODO
+```
 
-class A(VersionedYamlModel):
-    """Model with min, max constraints as None."""
+## Breaking Changes for `pydantic-yaml` V1
 
-    foo: str = "bar"
+The API for `pydantic-yaml` version 1.0.0 has been greatly simplified!
 
+### Mixin Class
 
-class B(VersionedYamlModel):
-    """Model with a maximum version set."""
-    
-    foo: str = "bar"
+This functionality has currently been removed!
+`YamlModel` and `YamlModelMixin` base classes are no longer needed.
+The plan is to re-add it before v1 fully releases,
+to allow the `.yaml()` or `.parse_*()` methods.
+However, this will be availble only for `pydantic<2`.
 
-    class Config:
-        min_version = "2.0.0"
+### Versioned Models
 
-ex_yml = """
-version: 1.0.0
-foo: baz
-"""
-
-a = A.parse_raw(ex_yml)
-assert a.version == SemVer("1.0.0")
-assert a.foo == "baz"
-
-try:
-    B.parse_raw(ex_yml)
-except ValidationError as e:
-    print("Correctly got ValidationError:", e, sep="\n")
-```
+This functionality has been removed, as it's questionably useful for most users.
+There is an [example in the docs](docs/versioned.md) that's available.
```

### Comparing `pydantic_yaml-0.9.0/pydantic_yaml/ext/versioned_model.py` & `pydantic_yaml-1.0.0a1/docs/versioned.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,113 +1,145 @@
-from typing import Optional, Tuple, Type
-import warnings
+# Versioned Models
+
+Versioned models were removed from `pydantic-yaml` as their usefulness for most
+users was questionable, and it added the `semver` dependency.
+
+If you need to recover functionality, below is an alternative you should use
+that is almost pure Pydantic v1.
 
-from pydantic import validator
+## Custom VersionedModel in Pydantic v1
 
-from pydantic_yaml.model import YamlModel
-from .semver import SemVer
+```python
+"""Versioned model example.
+
+Library versions:
+
+    pydantic<2
+    semver~=3.0.0  # additional
+"""
+
+import warnings
+from typing import Optional, Tuple, Type
 
-__all__ = ["VersionedYamlModel"]
+from pydantic import BaseModel, validator
+from semver import Version  # type: ignore
 
 
 def _chk_between(v, lo=None, hi=None):
     if v is None:
         return
     if (hi is not None) and (v > hi):
         raise ValueError(f"Default version higher than maximum: {v} > {hi}")
     if (lo is not None) and (v < lo):
         raise ValueError(f"Default version lower than minimum: {v} < {lo}")
 
 
 def _get_minmax_robust(
-    cls: Type["VersionedYamlModel"],
-) -> Tuple[Optional[SemVer], Optional[SemVer]]:
+    cls: Type["VersionedModel"],
+) -> Tuple[Optional[Version], Optional[Version]]:
     min_, max_ = None, None
     for supcls in cls.mro():
         Config = getattr(supcls, "Config", None)
         if Config is not None:
             if min_ is None:
                 min_ = getattr(Config, "min_version", None)
             if max_ is None:
                 max_ = getattr(Config, "max_version", None)
     return min_, max_
 
 
-class VersionedYamlModel(YamlModel):
-    """YAML model with versioning support.
-
-    Usage
-    -----
-    Inherit from this class, and set a Config class with attributes 
-    `min_version` and/or `max_version`:
+class VersionedModel(BaseModel):
+    """Versioned model behavior."""
 
-    ```python
-    class MyModel(VersionedYamlModel):
-        class Config:
-            min_version = "1.0.0"
+    version: Version
 
-        foo: str = "bar"
-    ```
+    class Config:
+        """Pydantic configuration."""
 
-    By default, the minimum version is "0.0.0" and the maximum is unset.
-    This pattern enables you to more easily version your YAML files and
-    protect against accidentally using older (or newer) configuration file formats.
+        # Allow SemVer
+        arbitrary_types_allowed = True
+        json_encoders = {Version: lambda x: str(x)}
 
-    Notes
-    -----
-    By default, a validator checks that the "version" field is between 
-    `Config.min_version` and `Config.max_version`, if those are not None.
+        # Version limits
+        min_version = Version(0, 0, 0)
+        max_version = None
 
-    It's probably best not to even set the `version` field by hand, but rather
-    in your configuration.
-    """
+    @validator("version", pre=True)
+    def _check_version(cls: Type["VersionedModel"], v) -> Version:  # type: ignore
+        """Set version from a string, then check within the limits."""
+        if not isinstance(v, Version):
+            v = Version.parse(v)
 
-    version: SemVer
+        min_, max_ = _get_minmax_robust(cls)
+        _chk_between(v, lo=min_, hi=max_)
+        return v
 
     def __init_subclass__(cls) -> None:
+        """Set config values."""
         # Check Config class types
         Config = getattr(cls, "Config", None)
         if Config is not None:
             # check one field
             minv = getattr(Config, "min_version", None)
             if minv is not None:
-                if not isinstance(minv, SemVer):
-                    setattr(Config, "min_version", SemVer(minv))
+                if not isinstance(minv, Version):
+                    setattr(Config, "min_version", Version.parse(minv))
             # check other field
             maxv = getattr(Config, "max_version", None)
             if maxv is not None:
-                if not isinstance(maxv, SemVer):
-                    setattr(Config, "max_version", SemVer(maxv))
+                if not isinstance(maxv, Version):
+                    setattr(Config, "max_version", Version.parse(maxv))
 
         # Check ranges
         min_, max_ = _get_minmax_robust(cls)
         if (min_ is not None) and (max_ is not None) and (min_ > max_):
-            raise ValueError(
-                f"Minimum version higher than maximum: {min_!r} > {max_!r}"
-            )
+            raise ValueError(f"Minimum version higher than maximum: {min_!r} > {max_!r}")
 
         # Check the default value of the "version" field
         fld = cls.__fields__["version"]
         d = fld.default
         if d is None:
             pass
         else:
             _chk_between(d, lo=min_, hi=max_)
             warnings.warn(
                 f"Recommended to have `version` be required, but set default {d!r}",
                 UserWarning,
             )
 
-        if not issubclass(fld.type_, SemVer):
-            raise TypeError(
-                f"Field type for `version` must be SemVer, got {fld.type_!r}"
-            )
+        if not issubclass(fld.type_, Version):
+            raise TypeError(f"Field type for `version` must be Version, got {fld.type_!r}")
 
-    @validator("version", always=True)
-    def _check_semver(cls, v):
-        min_, max_ = _get_minmax_robust(cls)
-        _chk_between(v, lo=min_, hi=max_)
-        return v
 
-    class Config:
-        min_version = SemVer("0.0.0")
-        max_version = None
+if __name__ == "__main__":
+    from pydantic_yaml import parse_yaml_raw_as
+
+    class FooBar(VersionedModel):
+        """Foobar model."""
+
+        foo: str
+
+        class Config:
+            """Pydantic configuration."""
+
+            max_version = Version(1)
+
+    fb = parse_yaml_raw_as(
+        FooBar,
+        """
+        version: 0.2.0
+        foo: bar
+        """,
+    )
+    try:
+        parse_yaml_raw_as(
+            FooBar,
+            """
+            version: 1.2.0  # higher than v1!
+            foo: bar
+            """,
+        )
+    except Exception as e:
+        print(e)
+
+
+```
```

### Comparing `pydantic_yaml-0.9.0/pydantic_yaml/main.py` & `pydantic_yaml-1.0.0a1/src/pydantic_yaml/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,23 @@
 """YAML-enabled Pydantic models."""
 
 __all__ = [
+    # New API
     "__version__",
-    "yaml",
-    "yaml_safe_dump",
-    "yaml_safe_load",
-    "YamlEnum",
+    "parse_yaml_file_as",
+    "parse_yaml_raw_as",
+    "to_yaml_file",
+    "to_yaml_str",
+    # TODO: Re-add
+    # YamlModelMixin ?
+    # YamlModel ?
+    # Deprecated classes
     "YamlInt",
     "YamlIntEnum",
     "YamlStr",
     "YamlStrEnum",
-    "YamlModel",
-    "YamlModelMixin",
-    "YamlModelMixinConfig",
-    "SemVer",
-    "VersionedYamlModel",
 ]
 
-from .compat.old_enums import YamlEnum
-from .compat.hacks import inject_all as _inject_yaml_hacks
-from .compat.types import YamlInt, YamlIntEnum, YamlStr, YamlStrEnum
-from .compat.yaml_lib import yaml, yaml_safe_dump, yaml_safe_load
-from .ext.semver import SemVer
-from .ext.versioned_model import VersionedYamlModel
-from .mixin import YamlModelMixin, YamlModelMixinConfig
-from .model import YamlModel
+from .deprecated.types import YamlInt, YamlIntEnum, YamlStr, YamlStrEnum
+from .dumper import to_yaml_file, to_yaml_str
+from .loader import parse_yaml_file_as, parse_yaml_raw_as
 from .version import __version__
-
-_inject_yaml_hacks()
```

