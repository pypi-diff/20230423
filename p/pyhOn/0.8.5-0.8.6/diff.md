# Comparing `tmp/pyhOn-0.8.5.tar.gz` & `tmp/pyhOn-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhOn-0.8.5.tar", last modified: Sun Apr 23 17:31:53 2023, max compression
+gzip compressed data, was "pyhOn-0.8.6.tar", last modified: Sun Apr 23 18:16:56 2023, max compression
```

## Comparing `pyhOn-0.8.5.tar` & `pyhOn-0.8.6.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:31:53.104823 pyhOn-0.8.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-23 17:31:39.000000 pyhOn-0.8.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-04-23 17:31:53.100823 pyhOn-0.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-04-23 17:31:39.000000 pyhOn-0.8.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:31:53.100823 pyhOn-0.8.5/pyhOn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-04-23 17:31:53.000000 pyhOn-0.8.5/pyhOn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-23 17:31:53.000000 pyhOn-0.8.5/pyhOn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 17:31:53.000000 pyhOn-0.8.5/pyhOn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-23 17:31:53.000000 pyhOn-0.8.5/pyhOn.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-23 17:31:53.000000 pyhOn-0.8.5/pyhOn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 17:31:53.000000 pyhOn-0.8.5/pyhOn.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:31:53.100823 pyhOn-0.8.5/pyhon/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-23 17:31:39.000000 pyhOn-0.8.5/pyhon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-04-23 17:31:39.000000 pyhOn-0.8.5/pyhon/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-04-23 17:31:39.000000 pyhOn-0.8.5/pyhon/appliance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:31:53.100823 pyhOn-0.8.5/pyhon/appliances/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 17:31:39.000000 pyhOn-0.8.5/pyhon/appliances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-23 17:31:39.000000 pyhOn-0.8.5/pyhon/appliances/dw.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-23 17:31:39.000000 pyhOn-0.8.5/pyhon/appliances/ov.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-23 17:31:39.000000 pyhOn-0.8.5/pyhon/appliances/td.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-23 17:31:39.000000 pyhOn-0.8.5/pyhon/appliances/wd.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-23 17:31:39.000000 pyhOn-0.8.5/pyhon/appliances/wm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-04-23 17:31:39.000000 pyhOn-0.8.5/pyhon/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:31:53.100823 pyhOn-0.8.5/pyhon/connection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 17:31:39.000000 pyhOn-0.8.5/pyhon/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7599 2023-04-23 17:31:39.000000 pyhOn-0.8.5/pyhon/connection/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10694 2023-04-23 17:31:39.000000 pyhOn-0.8.5/pyhon/connection/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-23 17:31:39.000000 pyhOn-0.8.5/pyhon/connection/device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:31:53.100823 pyhOn-0.8.5/pyhon/connection/handler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 17:31:39.000000 pyhOn-0.8.5/pyhon/connection/handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-23 17:31:39.000000 pyhOn-0.8.5/pyhon/connection/handler/anonym.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-23 17:31:39.000000 pyhOn-0.8.5/pyhon/connection/handler/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-04-23 17:31:39.000000 pyhOn-0.8.5/pyhon/connection/handler/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-04-23 17:31:39.000000 pyhOn-0.8.5/pyhon/connection/handler/hon.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-23 17:31:39.000000 pyhOn-0.8.5/pyhon/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-23 17:31:39.000000 pyhOn-0.8.5/pyhon/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-04-23 17:31:39.000000 pyhOn-0.8.5/pyhon/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-23 17:31:39.000000 pyhOn-0.8.5/pyhon/hon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:31:53.100823 pyhOn-0.8.5/pyhon/parameter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 17:31:39.000000 pyhOn-0.8.5/pyhon/parameter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-23 17:31:39.000000 pyhOn-0.8.5/pyhon/parameter/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-04-23 17:31:39.000000 pyhOn-0.8.5/pyhon/parameter/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-23 17:31:39.000000 pyhOn-0.8.5/pyhon/parameter/fixed.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-23 17:31:39.000000 pyhOn-0.8.5/pyhon/parameter/program.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-23 17:31:39.000000 pyhOn-0.8.5/pyhon/parameter/range.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 17:31:53.104823 pyhOn-0.8.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-23 17:31:39.000000 pyhOn-0.8.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:16:56.296391 pyhOn-0.8.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-23 18:16:45.000000 pyhOn-0.8.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-04-23 18:16:56.296391 pyhOn-0.8.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-04-23 18:16:45.000000 pyhOn-0.8.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:16:56.296391 pyhOn-0.8.6/pyhOn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-04-23 18:16:56.000000 pyhOn-0.8.6/pyhOn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-23 18:16:56.000000 pyhOn-0.8.6/pyhOn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 18:16:56.000000 pyhOn-0.8.6/pyhOn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-23 18:16:56.000000 pyhOn-0.8.6/pyhOn.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-23 18:16:56.000000 pyhOn-0.8.6/pyhOn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 18:16:56.000000 pyhOn-0.8.6/pyhOn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:16:56.296391 pyhOn-0.8.6/pyhon/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-23 18:16:45.000000 pyhOn-0.8.6/pyhon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-04-23 18:16:45.000000 pyhOn-0.8.6/pyhon/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-04-23 18:16:45.000000 pyhOn-0.8.6/pyhon/appliance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:16:56.296391 pyhOn-0.8.6/pyhon/appliances/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 18:16:45.000000 pyhOn-0.8.6/pyhon/appliances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-23 18:16:45.000000 pyhOn-0.8.6/pyhon/appliances/dw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-23 18:16:45.000000 pyhOn-0.8.6/pyhon/appliances/ov.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-23 18:16:45.000000 pyhOn-0.8.6/pyhon/appliances/td.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-23 18:16:45.000000 pyhOn-0.8.6/pyhon/appliances/wd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-23 18:16:45.000000 pyhOn-0.8.6/pyhon/appliances/wm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-04-23 18:16:45.000000 pyhOn-0.8.6/pyhon/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:16:56.296391 pyhOn-0.8.6/pyhon/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 18:16:45.000000 pyhOn-0.8.6/pyhon/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-04-23 18:16:45.000000 pyhOn-0.8.6/pyhon/connection/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10694 2023-04-23 18:16:45.000000 pyhOn-0.8.6/pyhon/connection/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-23 18:16:45.000000 pyhOn-0.8.6/pyhon/connection/device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:16:56.296391 pyhOn-0.8.6/pyhon/connection/handler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 18:16:45.000000 pyhOn-0.8.6/pyhon/connection/handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-23 18:16:45.000000 pyhOn-0.8.6/pyhon/connection/handler/anonym.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-23 18:16:45.000000 pyhOn-0.8.6/pyhon/connection/handler/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-04-23 18:16:45.000000 pyhOn-0.8.6/pyhon/connection/handler/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-04-23 18:16:45.000000 pyhOn-0.8.6/pyhon/connection/handler/hon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-23 18:16:45.000000 pyhOn-0.8.6/pyhon/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-23 18:16:45.000000 pyhOn-0.8.6/pyhon/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-04-23 18:16:45.000000 pyhOn-0.8.6/pyhon/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-23 18:16:45.000000 pyhOn-0.8.6/pyhon/hon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:16:56.296391 pyhOn-0.8.6/pyhon/parameter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 18:16:45.000000 pyhOn-0.8.6/pyhon/parameter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-23 18:16:45.000000 pyhOn-0.8.6/pyhon/parameter/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-04-23 18:16:45.000000 pyhOn-0.8.6/pyhon/parameter/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-23 18:16:45.000000 pyhOn-0.8.6/pyhon/parameter/fixed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-23 18:16:45.000000 pyhOn-0.8.6/pyhon/parameter/program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-23 18:16:45.000000 pyhOn-0.8.6/pyhon/parameter/range.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 18:16:56.296391 pyhOn-0.8.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-23 18:16:45.000000 pyhOn-0.8.6/setup.py
```

### Comparing `pyhOn-0.8.5/LICENSE` & `pyhOn-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.5/PKG-INFO` & `pyhOn-0.8.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhOn
-Version: 0.8.5
+Version: 0.8.6
 Summary: Control hOn devices with python
 Author: Andre Basche
 License: MIT
 Project-URL: GitHub, https://github.com/Andre0512/pyhOn
 Project-URL: PyPI, https://pypi.org/project/pyhOn
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyhOn-0.8.5/README.md` & `pyhOn-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.5/pyhOn.egg-info/PKG-INFO` & `pyhOn-0.8.6/pyhOn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhOn
-Version: 0.8.5
+Version: 0.8.6
 Summary: Control hOn devices with python
 Author: Andre Basche
 License: MIT
 Project-URL: GitHub, https://github.com/Andre0512/pyhOn
 Project-URL: PyPI, https://pypi.org/project/pyhOn
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyhOn-0.8.5/pyhOn.egg-info/SOURCES.txt` & `pyhOn-0.8.6/pyhOn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.5/pyhon/__main__.py` & `pyhOn-0.8.6/pyhon/__main__.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.5/pyhon/appliance.py` & `pyhOn-0.8.6/pyhon/appliance.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import importlib
+import logging
 from contextlib import suppress
 from typing import Optional, Dict, Any
 from typing import TYPE_CHECKING
 
 from pyhon import helper
 from pyhon.commands import HonCommand
 from pyhon.parameter.fixed import HonParameterFixed
 
 if TYPE_CHECKING:
     from pyhon import HonAPI
 
 
+_LOGGER = logging.getLogger(__name__)
+
+
 class HonAppliance:
     def __init__(
         self, api: Optional["HonAPI"], info: Dict[str, Any], zone: int = 0
     ) -> None:
         if attributes := info.get("attributes"):
             info["attributes"] = {v["parName"]: v["parValue"] for v in attributes}
         self._info: Dict = info
@@ -179,15 +183,18 @@
                 command.parameters | command.ancillary_parameters
             ).items():
                 result.setdefault(name, {})[key] = parameter.value
         return result
 
     async def load_attributes(self):
         self._attributes = await self._api.load_attributes(self)
-        for name, values in self._attributes.pop("shadow").get("parameters").items():
+        _LOGGER.warning(self._attributes)
+        for name, values in (
+            self._attributes.pop("shadow", {}).get("parameters", {}).items()
+        ):
             self._attributes.setdefault("parameters", {})[name] = values["parNewVal"]
 
     async def load_statistics(self):
         self._statistics = await self._api.load_statistics(self)
 
     async def update(self):
         await self.load_attributes()
```

### Comparing `pyhOn-0.8.5/pyhon/appliances/ov.py` & `pyhOn-0.8.6/pyhon/appliances/ov.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.5/pyhon/appliances/td.py` & `pyhOn-0.8.6/pyhon/appliances/td.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.5/pyhon/commands.py` & `pyhOn-0.8.6/pyhon/commands.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.5/pyhon/connection/api.py` & `pyhOn-0.8.6/pyhon/connection/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from pyhon import const, exceptions
 from pyhon.appliance import HonAppliance
 from pyhon.connection.auth import HonAuth
 from pyhon.connection.handler.anonym import HonAnonymousConnectionHandler
 from pyhon.connection.handler.hon import HonConnectionHandler
 
-_LOGGER = logging.getLogger()
+_LOGGER = logging.getLogger(__name__)
 
 
 class HonAPI:
     def __init__(
         self,
         email: str = "",
         password: str = "",
```

### Comparing `pyhOn-0.8.5/pyhon/connection/auth.py` & `pyhOn-0.8.6/pyhon/connection/auth.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.5/pyhon/connection/device.py` & `pyhOn-0.8.6/pyhon/connection/device.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.5/pyhon/connection/handler/anonym.py` & `pyhOn-0.8.6/pyhon/connection/handler/anonym.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.5/pyhon/connection/handler/auth.py` & `pyhOn-0.8.6/pyhon/connection/handler/auth.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.5/pyhon/connection/handler/base.py` & `pyhOn-0.8.6/pyhon/connection/handler/base.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.5/pyhon/connection/handler/hon.py` & `pyhOn-0.8.6/pyhon/connection/handler/hon.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.5/pyhon/helper.py` & `pyhOn-0.8.6/pyhon/helper.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.5/pyhon/hon.py` & `pyhOn-0.8.6/pyhon/hon.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.5/pyhon/parameter/base.py` & `pyhOn-0.8.6/pyhon/parameter/base.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.5/pyhon/parameter/enum.py` & `pyhOn-0.8.6/pyhon/parameter/enum.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.5/pyhon/parameter/fixed.py` & `pyhOn-0.8.6/pyhon/parameter/fixed.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.5/pyhon/parameter/program.py` & `pyhOn-0.8.6/pyhon/parameter/program.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.5/pyhon/parameter/range.py` & `pyhOn-0.8.6/pyhon/parameter/range.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.5/setup.py` & `pyhOn-0.8.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="pyhOn",
-    version="0.8.5",
+    version="0.8.6",
     author="Andre Basche",
     description="Control hOn devices with python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     project_urls={
         "GitHub": "https://github.com/Andre0512/pyhOn",
         "PyPI": "https://pypi.org/project/pyhOn",
```

