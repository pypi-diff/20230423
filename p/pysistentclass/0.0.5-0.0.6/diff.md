# Comparing `tmp/pysistentclass-0.0.5.tar.gz` & `tmp/pysistentclass-0.0.6.tar.gz`

## Comparing `pysistentclass-0.0.5.tar` & `pysistentclass-0.0.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pysistentclass-0.0.5/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     8031 2020-02-02 00:00:00.000000 pysistentclass-0.0.5/src/pysistentclass/__init__.py
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 pysistentclass-0.0.5/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 pysistentclass-0.0.5/LICENSE
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 pysistentclass-0.0.5/README.md
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 pysistentclass-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 pysistentclass-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pysistentclass-0.0.6/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     8051 2020-02-02 00:00:00.000000 pysistentclass-0.0.6/src/pysistentclass/__init__.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pysistentclass-0.0.6/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 pysistentclass-0.0.6/LICENSE
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 pysistentclass-0.0.6/README.md
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 pysistentclass-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 pysistentclass-0.0.6/PKG-INFO
```

### Comparing `pysistentclass-0.0.5/.github/workflows/python-publish.yml` & `pysistentclass-0.0.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pysistentclass-0.0.5/src/pysistentclass/__init__.py` & `pysistentclass-0.0.6/src/pysistentclass/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,51 +1,59 @@
 from __future__ import annotations
 from pathlib import Path
-from dataclasses import dataclass, field, make_dataclass
+from dataclasses import dataclass, field
 from enum import Enum
-from typing import Dict, List, Union, Any, Type
+from typing import Dict, List, Union, Any, dataclass_transform, Type, TypeVar
 
 from importlib import import_module
 
 import json
 import yaml
 import toml
 
 import inspect
 import hashlib
 
 import colorlog
 import logging
 
+T = TypeVar("T")
+
 
 def logger(name: str) -> logging.Logger:
     logger = colorlog.getLogger(name)
-    myFormatter = colorlog.ColoredFormatter(log_colors={
-        'DEBUG': 'cyan', 'INFO': 'reset', 'ERROR': 'bold_red', 'WARNING': 'yellow'}, fmt="%(log_color)s%(levelname)s %(asctime)s " + name + " > %(message)s")
+    myFormatter = colorlog.ColoredFormatter(
+        log_colors={
+            "DEBUG": "cyan",
+            "INFO": "reset",
+            "ERROR": "bold_red",
+            "WARNING": "yellow",
+        },
+        fmt="%(log_color)s%(levelname)s %(asctime)s " + name + " > %(message)s",
+    )
     handler = colorlog.StreamHandler()
     handler.setFormatter(myFormatter)
     logger.addHandler(handler)
 
     return logger
 
 
 LOGGER = logger(__name__ + ".py")
 
 
 class SettingsAttributeError(Exception):
     pass
 
 
-def skip_underscore_keys(obj): return {
-    k: v for k, v in vars(obj).items() if not k.startswith("_")
-}
+def skip_underscore_keys(obj):
+    return {k: v for k, v in vars(obj).items() if not k.startswith("_")}
 
 
-def json_pretty(obj): return json.dumps(
-    obj, indent=4, sort_keys=True, default=vars)
+def json_pretty(obj):
+    return json.dumps(obj, indent=4, sort_keys=True, default=vars)
 
 
 class Format(str, Enum):
     deserializer: callable
     serializer: callable
 
     def __new__(
@@ -71,30 +79,31 @@
     PRIVATE = "private"
 
     class _ScopeRepr:
         def __repr__(self) -> str:
             pass
 
 
-def pysistentclass(cls=None, /, *, init=True) -> Type[_T@dataclass]:
+@dataclass_transform()
+def pysistentclass(cls: Type[T]) -> Type[T]:
     """
     pysistentclass decorator
 
     This decorator can be used to mark a class as a pysistentclass.
     """
     # return make_dataclass(cls.__name__)
+    cls._scope = getattr(cls, "_scope", Scope.PUBLIC)
+    cls._class_key = None
     datacls = dataclass(cls)
-    setattr(datacls, "_scope", getattr(datacls, "_scope", Scope.PUBLIC))
-    setattr(datacls, "_class_key", None)
     return datacls
 
 
 @dataclass
 class Settings(dict):
-    """ Settings class
+    """Settings class
 
     This is a dataclass that holds the settings for the application. It
     is a subclass of dict, so it can be used as a dict.
 
     It can be used in two ways:
 
     1. If you don't need to store any data in your settings, you can use
@@ -105,32 +114,31 @@
 
     2. If you need to store data in your settings, you can create a
     subclass of Settings and add data fields to it. In that case, you
     need to pass a settings_dir parameter to the constructor. This
     parameter should be the path to the directory where the settings
     file will be stored.
     """
+
     settings_dir: Union[Path, str]
 
-    _classes: Dict[str, Dict[str, str]] = field(
-        default_factory=dict, init=False)
+    _classes: Dict[str, Dict[str, str]] = field(default_factory=dict, init=False)
     _settings: Dict[str, object] = field(default_factory=dict, init=False)
 
     module_names: List[str] = field(default_factory=list)
     format: Format = Format.JSON
     logging_level: int = logging.DEBUG
 
     def json_object_hook(self, obj: dict) -> object:
         if "_class_key" in obj:
             class_key = obj["_class_key"]
             module = import_module(self._classes[class_key]["module"])
             class_name = self._classes[class_key]["class_name"]
             if not hasattr(module, class_name):
-                raise SettingsAttributeError(
-                    f"{module} does not have {class_name}")
+                raise SettingsAttributeError(f"{module} does not have {class_name}")
             class_obj = getattr(module, class_name)
             return class_obj(**obj)
         return obj
 
     def __post_init__(self):
         LOGGER.setLevel(self.logging_level)
         LOGGER.debug(f"__post_init__()")
@@ -212,16 +220,15 @@
                     serialized, self.json_object_hook
                 )
         except SettingsAttributeError as e:
             LOGGER.debug(e)
         if serialized != default_serialized:
             LOGGER.debug("serialized != default_serialized")
         if not deserialized:
-            LOGGER.debug(
-                "deserialized is None or empty using default settings!")
+            LOGGER.debug("deserialized is None or empty using default settings!")
             deserialized = self._settings
         self._settings = deserialized
         self.public = {}
         self.private = {}
         for k, v in self._settings.items():
             if v._scope == Scope.PUBLIC:
                 self.public[k] = v
```

### Comparing `pysistentclass-0.0.5/LICENSE` & `pysistentclass-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pysistentclass-0.0.5/pyproject.toml` & `pysistentclass-0.0.6/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pysistentclass"
-version = "0.0.5"
+version = "0.0.6"
 authors = [{ name = "manjaroman2", email = "manjaroman2@protonmail.com" }]
 description = "A small settings module for python"
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
 dependencies = ["colorlog", "PyYAML", "toml"]
```

### Comparing `pysistentclass-0.0.5/PKG-INFO` & `pysistentclass-0.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pysistentclass
-Version: 0.0.5
+Version: 0.0.6
 Summary: A small settings module for python
 Project-URL: Homepage, https://github.com/manjaroman2/pysistentclass
 Project-URL: Bug Tracker, https://github.com/manjaroman2/pysistentclass/issues
 Author-email: manjaroman2 <manjaroman2@protonmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
+Requires-Python: >=3.11
 Requires-Dist: colorlog
 Requires-Dist: pyyaml
 Requires-Dist: toml
 Description-Content-Type: text/markdown
 
 # pysistentclass
```

