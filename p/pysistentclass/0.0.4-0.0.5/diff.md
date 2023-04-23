# Comparing `tmp/pysistentclass-0.0.4.tar.gz` & `tmp/pysistentclass-0.0.5.tar.gz`

## Comparing `pysistentclass-0.0.4.tar` & `pysistentclass-0.0.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pysistentclass-0.0.4/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     7979 2020-02-02 00:00:00.000000 pysistentclass-0.0.4/src/pysistentclass/__init__.py
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 pysistentclass-0.0.4/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 pysistentclass-0.0.4/LICENSE
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 pysistentclass-0.0.4/README.md
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 pysistentclass-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 pysistentclass-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pysistentclass-0.0.5/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     8031 2020-02-02 00:00:00.000000 pysistentclass-0.0.5/src/pysistentclass/__init__.py
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 pysistentclass-0.0.5/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 pysistentclass-0.0.5/LICENSE
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 pysistentclass-0.0.5/README.md
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 pysistentclass-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 pysistentclass-0.0.5/PKG-INFO
```

### Comparing `pysistentclass-0.0.4/.github/workflows/python-publish.yml` & `pysistentclass-0.0.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pysistentclass-0.0.4/src/pysistentclass/__init__.py` & `pysistentclass-0.0.5/src/pysistentclass/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 from pathlib import Path
-from dataclasses import dataclass, field
+from dataclasses import dataclass, field, make_dataclass
 from enum import Enum
-from typing import Dict, List, Union, Any
+from typing import Dict, List, Union, Any, Type
 
 from importlib import import_module
 
 import json
 import yaml
 import toml
 
@@ -71,24 +71,25 @@
     PRIVATE = "private"
 
     class _ScopeRepr:
         def __repr__(self) -> str:
             pass
 
 
-def pysistentclass(wrapped_class: type):
+def pysistentclass(cls=None, /, *, init=True) -> Type[_T@dataclass]:
     """
     pysistentclass decorator
 
     This decorator can be used to mark a class as a pysistentclass.
     """
-    setattr(wrapped_class, "_scope", getattr(wrapped_class, "_scope", Scope.PUBLIC))
-    setattr(wrapped_class, "_class_key", None)
-    wrapped_class = dataclass(wrapped_class)
-    return wrapped_class
+    # return make_dataclass(cls.__name__)
+    datacls = dataclass(cls)
+    setattr(datacls, "_scope", getattr(datacls, "_scope", Scope.PUBLIC))
+    setattr(datacls, "_class_key", None)
+    return datacls
 
 
 @dataclass
 class Settings(dict):
     """ Settings class
 
     This is a dataclass that holds the settings for the application. It
```

### Comparing `pysistentclass-0.0.4/LICENSE` & `pysistentclass-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pysistentclass-0.0.4/pyproject.toml` & `pysistentclass-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pysistentclass"
-version = "0.0.4"
+version = "0.0.5"
 authors = [{ name = "manjaroman2", email = "manjaroman2@protonmail.com" }]
 description = "A small settings module for python"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

### Comparing `pysistentclass-0.0.4/PKG-INFO` & `pysistentclass-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysistentclass
-Version: 0.0.4
+Version: 0.0.5
 Summary: A small settings module for python
 Project-URL: Homepage, https://github.com/manjaroman2/pysistentclass
 Project-URL: Bug Tracker, https://github.com/manjaroman2/pysistentclass/issues
 Author-email: manjaroman2 <manjaroman2@protonmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

