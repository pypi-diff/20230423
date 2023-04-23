# Comparing `tmp/python_ember_mug-0.6.2.tar.gz` & `tmp/python_ember_mug-0.7.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_ember_mug-0.6.2.tar", max compression
+gzip compressed data, was "python_ember_mug-0.7.0b1.tar", max compression
```

## Comparing `python_ember_mug-0.6.2.tar` & `python_ember_mug-0.7.0b1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1069 2023-04-15 03:17:36.080041 python_ember_mug-0.6.2/LICENSE
--rw-r--r--   0        0        0     5219 2023-04-15 03:17:36.080041 python_ember_mug-0.6.2/README.md
--rwxr-xr-x   0        0        0      187 2023-04-15 03:17:36.080041 python_ember_mug-0.6.2/ember_mug/__init__.py
--rw-r--r--   0        0        0      106 2023-04-15 03:17:36.080041 python_ember_mug-0.6.2/ember_mug/__main__.py
--rw-r--r--   0        0        0      296 2023-04-15 03:17:36.080041 python_ember_mug-0.6.2/ember_mug/cli/__init__.py
--rw-r--r--   0        0        0     8471 2023-04-15 03:17:36.080041 python_ember_mug-0.6.2/ember_mug/cli/commands.py
--rw-r--r--   0        0        0     2910 2023-04-15 03:17:36.080041 python_ember_mug-0.6.2/ember_mug/cli/helpers.py
--rw-r--r--   0        0        0     4820 2023-04-15 03:17:36.084041 python_ember_mug-0.6.2/ember_mug/consts.py
--rw-r--r--   0        0        0     7729 2023-04-15 03:17:36.084041 python_ember_mug-0.6.2/ember_mug/data.py
--rw-r--r--   0        0        0      605 2023-04-15 03:17:36.084041 python_ember_mug-0.6.2/ember_mug/formatting.py
--rw-r--r--   0        0        0    16978 2023-04-15 03:17:36.084041 python_ember_mug-0.6.2/ember_mug/mug.py
--rw-r--r--   0        0        0     2112 2023-04-15 03:17:36.084041 python_ember_mug-0.6.2/ember_mug/scanner.py
--rw-r--r--   0        0        0     1963 2023-04-15 03:17:36.084041 python_ember_mug-0.6.2/ember_mug/utils.py
--rw-r--r--   0        0        0     2894 2023-04-15 03:17:36.084041 python_ember_mug-0.6.2/pyproject.toml
--rw-r--r--   0        0        0       46 2023-04-15 03:17:36.084041 python_ember_mug-0.6.2/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-04-15 03:17:36.084041 python_ember_mug-0.6.2/tests/cli/__init__.py
--rw-r--r--   0        0        0     7846 2023-04-15 03:17:36.084041 python_ember_mug-0.6.2/tests/cli/test_commands.py
--rw-r--r--   0        0        0     2663 2023-04-15 03:17:36.084041 python_ember_mug-0.6.2/tests/cli/test_helpers.py
--rw-r--r--   0        0        0     1199 2023-04-15 03:17:36.084041 python_ember_mug-0.6.2/tests/conftest.py
--rw-r--r--   0        0        0    19254 2023-04-15 03:17:36.084041 python_ember_mug-0.6.2/tests/test_connection.py
--rw-r--r--   0        0        0      776 2023-04-15 03:17:36.084041 python_ember_mug-0.6.2/tests/test_consts.py
--rw-r--r--   0        0        0     2343 2023-04-15 03:17:36.084041 python_ember_mug-0.6.2/tests/test_data.py
--rw-r--r--   0        0        0      534 2023-04-15 03:17:36.084041 python_ember_mug-0.6.2/tests/test_formatting.py
--rw-r--r--   0        0        0     3338 2023-04-15 03:17:36.084041 python_ember_mug-0.6.2/tests/test_mug_data.py
--rw-r--r--   0        0        0     2012 2023-04-15 03:17:36.084041 python_ember_mug-0.6.2/tests/test_scanner.py
--rw-r--r--   0        0        0      801 2023-04-15 03:17:36.084041 python_ember_mug-0.6.2/tests/test_utils.py
--rw-r--r--   0        0        0     6425 1970-01-01 00:00:00.000000 python_ember_mug-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-23 18:10:40.292760 python_ember_mug-0.7.0b1/LICENSE
+-rw-r--r--   0        0        0     5219 2023-04-23 18:10:40.292760 python_ember_mug-0.7.0b1/README.md
+-rwxr-xr-x   0        0        0      189 2023-04-23 18:10:40.292760 python_ember_mug-0.7.0b1/ember_mug/__init__.py
+-rw-r--r--   0        0        0      106 2023-04-23 18:10:40.292760 python_ember_mug-0.7.0b1/ember_mug/__main__.py
+-rw-r--r--   0        0        0      296 2023-04-23 18:10:40.292760 python_ember_mug-0.7.0b1/ember_mug/cli/__init__.py
+-rw-r--r--   0        0        0     8471 2023-04-23 18:10:40.292760 python_ember_mug-0.7.0b1/ember_mug/cli/commands.py
+-rw-r--r--   0        0        0     2910 2023-04-23 18:10:40.292760 python_ember_mug-0.7.0b1/ember_mug/cli/helpers.py
+-rw-r--r--   0        0        0     4890 2023-04-23 18:10:40.292760 python_ember_mug-0.7.0b1/ember_mug/consts.py
+-rw-r--r--   0        0        0     7776 2023-04-23 18:10:40.292760 python_ember_mug-0.7.0b1/ember_mug/data.py
+-rw-r--r--   0        0        0      605 2023-04-23 18:10:40.292760 python_ember_mug-0.7.0b1/ember_mug/formatting.py
+-rw-r--r--   0        0        0    16978 2023-04-23 18:10:40.292760 python_ember_mug-0.7.0b1/ember_mug/mug.py
+-rw-r--r--   0        0        0     2112 2023-04-23 18:10:40.292760 python_ember_mug-0.7.0b1/ember_mug/scanner.py
+-rw-r--r--   0        0        0     1963 2023-04-23 18:10:40.292760 python_ember_mug-0.7.0b1/ember_mug/utils.py
+-rw-r--r--   0        0        0     2896 2023-04-23 18:10:40.296760 python_ember_mug-0.7.0b1/pyproject.toml
+-rw-r--r--   0        0        0       46 2023-04-23 18:10:40.296760 python_ember_mug-0.7.0b1/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-23 18:10:40.296760 python_ember_mug-0.7.0b1/tests/cli/__init__.py
+-rw-r--r--   0        0        0     7846 2023-04-23 18:10:40.296760 python_ember_mug-0.7.0b1/tests/cli/test_commands.py
+-rw-r--r--   0        0        0     2663 2023-04-23 18:10:40.296760 python_ember_mug-0.7.0b1/tests/cli/test_helpers.py
+-rw-r--r--   0        0        0     1199 2023-04-23 18:10:40.296760 python_ember_mug-0.7.0b1/tests/conftest.py
+-rw-r--r--   0        0        0    19254 2023-04-23 18:10:40.296760 python_ember_mug-0.7.0b1/tests/test_connection.py
+-rw-r--r--   0        0        0      776 2023-04-23 18:10:40.296760 python_ember_mug-0.7.0b1/tests/test_consts.py
+-rw-r--r--   0        0        0     2343 2023-04-23 18:10:40.296760 python_ember_mug-0.7.0b1/tests/test_data.py
+-rw-r--r--   0        0        0      534 2023-04-23 18:10:40.296760 python_ember_mug-0.7.0b1/tests/test_formatting.py
+-rw-r--r--   0        0        0     3338 2023-04-23 18:10:40.296760 python_ember_mug-0.7.0b1/tests/test_mug_data.py
+-rw-r--r--   0        0        0     2012 2023-04-23 18:10:40.296760 python_ember_mug-0.7.0b1/tests/test_scanner.py
+-rw-r--r--   0        0        0      801 2023-04-23 18:10:40.296760 python_ember_mug-0.7.0b1/tests/test_utils.py
+-rw-r--r--   0        0        0     6427 1970-01-01 00:00:00.000000 python_ember_mug-0.7.0b1/PKG-INFO
```

### Comparing `python_ember_mug-0.6.2/LICENSE` & `python_ember_mug-0.7.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.6.2/README.md` & `python_ember_mug-0.7.0b1/README.md`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.6.2/ember_mug/cli/commands.py` & `python_ember_mug-0.7.0b1/ember_mug/cli/commands.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.6.2/ember_mug/cli/helpers.py` & `python_ember_mug-0.7.0b1/ember_mug/cli/helpers.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.6.2/ember_mug/consts.py` & `python_ember_mug-0.7.0b1/ember_mug/consts.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,21 +8,23 @@
 from typing import Literal
 from uuid import UUID
 
 # Bluetooth names of Ember devices
 EMBER_MUG = "Ember Ceramic Mug"
 EMBER_CUP = "Ember Cup"
 EMBER_CUP_2 = "Ember Cup 2"
+EMBER_TRAVEL_MUG_SHORT = "Ember Travel M"
 EMBER_TRAVEL_MUG = "Ember Travel Mug"
 
 EMBER_BLUETOOTH_NAMES: tuple[str, ...] = (
     EMBER_MUG,
     EMBER_CUP,
     EMBER_CUP_2,
     EMBER_TRAVEL_MUG,
+    EMBER_TRAVEL_MUG_SHORT,
 )
 
 # Format for all the mug's Bluetooth UUIDs
 UUID_TEMPLATE = "fc54{:0>4x}-236c-4c94-8fa9-944a3e5353fa"
 
 
 class TemperatureUnit(str, Enum):
```

### Comparing `python_ember_mug-0.6.2/ember_mug/data.py` & `python_ember_mug-0.7.0b1/ember_mug/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from dataclasses import asdict, dataclass, is_dataclass
 from functools import cached_property
 from typing import Any, NamedTuple
 
 from .consts import (
     ATTR_LABELS,
     EMBER_CUP,
-    EMBER_TRAVEL_MUG,
+    EMBER_TRAVEL_MUG_SHORT,
     EXTRA_ATTRS,
     INITIAL_ATTRS,
     TRAVEL_MUG_ATTRS,
     UPDATE_ATTRS,
     LiquidState,
     TemperatureUnit,
 )
@@ -117,15 +117,15 @@
     def is_cup(self) -> bool:
         """Check if the model is a Cup."""
         return self.name.startswith(EMBER_CUP)
 
     @cached_property
     def is_travel_mug(self) -> bool:
         """Check if the model is a Travel mug."""
-        return self.name.startswith(EMBER_TRAVEL_MUG)
+        return self.name.startswith(EMBER_TRAVEL_MUG_SHORT)
 
     @cached_property
     def attribute_labels(self) -> dict[str, str]:
         """Calculated labels for includes attributes."""
         all_attrs = self.initial_attributes | self.update_attributes | {'use_metric'}
         return {attr: label for attr, label in ATTR_LABELS.items() if attr in all_attrs}
 
@@ -141,15 +141,15 @@
         """Attributes to update based on model and extra."""
         attributes = UPDATE_ATTRS
         if self.include_extra is False:
             attributes = attributes - EXTRA_ATTRS
         if self.is_cup:
             attributes = attributes - {'name'}
         elif self.is_travel_mug:
-            attributes = attributes | TRAVEL_MUG_ATTRS
+            attributes = (attributes - {'led_colour', 'liquid_level'}) | TRAVEL_MUG_ATTRS
         return attributes
 
 
 @dataclass
 class MugMeta:
     """Meta data for mug."""
```

### Comparing `python_ember_mug-0.6.2/ember_mug/formatting.py` & `python_ember_mug-0.7.0b1/ember_mug/formatting.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.6.2/ember_mug/mug.py` & `python_ember_mug-0.7.0b1/ember_mug/mug.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.6.2/ember_mug/scanner.py` & `python_ember_mug-0.7.0b1/ember_mug/scanner.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.6.2/ember_mug/utils.py` & `python_ember_mug-0.7.0b1/ember_mug/utils.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.6.2/pyproject.toml` & `python_ember_mug-0.7.0b1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "python-ember-mug"
-version = "0.6.2"
+version = "0.7.0b1"
 homepage = "https://github.com/sopelj/python-ember-mug"
 description = "Python Library for Ember Mugs."
 authors = ["Jesse Sopel <jesse.sopel@gmail.com>"]
 readme = "README.md"
 license =  "MIT"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
@@ -32,15 +32,15 @@
 bleak = ">=0.19.5"
 
 [tool.poetry.group.dev.dependencies]
 black  = { version = ">=22.6,<24.0" }
 isort  = { version = "^5.8.0" }
 flake8  = { version = ">=5,<7" }
 flake8-docstrings = { version = "^1.6.0" }
-mypy = { version = ">=0.971,<1.2" }
+mypy = { version = ">=0.971,<1.3" }
 pytest  = { version = "^7.2.1" }
 pytest-cov  = { version = ">=3,<5" }
 pytest-asyncio =  { version = ">=0.19,<0.22" }
 tox  = { version = "^3.20.1" }
 virtualenv  = { version = "^20.2.2" }
 mkdocs  = { version = "^1.1.2" }
 mkdocs-include-markdown-plugin  = { version = ">=3.6.1,<5.0.0" }
```

### Comparing `python_ember_mug-0.6.2/tests/cli/test_commands.py` & `python_ember_mug-0.7.0b1/tests/cli/test_commands.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.6.2/tests/cli/test_helpers.py` & `python_ember_mug-0.7.0b1/tests/cli/test_helpers.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.6.2/tests/conftest.py` & `python_ember_mug-0.7.0b1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.6.2/tests/test_connection.py` & `python_ember_mug-0.7.0b1/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.6.2/tests/test_consts.py` & `python_ember_mug-0.7.0b1/tests/test_consts.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.6.2/tests/test_data.py` & `python_ember_mug-0.7.0b1/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.6.2/tests/test_formatting.py` & `python_ember_mug-0.7.0b1/tests/test_formatting.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.6.2/tests/test_mug_data.py` & `python_ember_mug-0.7.0b1/tests/test_mug_data.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.6.2/tests/test_scanner.py` & `python_ember_mug-0.7.0b1/tests/test_scanner.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.6.2/tests/test_utils.py` & `python_ember_mug-0.7.0b1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.6.2/PKG-INFO` & `python_ember_mug-0.7.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-ember-mug
-Version: 0.6.2
+Version: 0.7.0b1
 Summary: Python Library for Ember Mugs.
 Home-page: https://github.com/sopelj/python-ember-mug
 License: MIT
 Author: Jesse Sopel
 Author-email: jesse.sopel@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Development Status :: 2 - Pre-Alpha
```

