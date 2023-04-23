# Comparing `tmp/ospyata-3.1.0.tar.gz` & `tmp/ospyata-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ospyata-3.1.0.tar", last modified: Sat Apr 15 08:14:05 2023, max compression
+gzip compressed data, was "ospyata-3.1.1.tar", last modified: Sun Apr 23 13:28:16 2023, max compression
```

## Comparing `ospyata-3.1.0.tar` & `ospyata-3.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:14:05.045255 ospyata-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-15 08:13:55.000000 ospyata-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-15 08:14:05.045255 ospyata-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-15 08:13:55.000000 ospyata-3.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-15 08:14:05.045255 ospyata-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-15 08:13:55.000000 ospyata-3.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:14:05.045255 ospyata-3.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:14:05.045255 ospyata-3.1.0/src/ospyata/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-15 08:13:55.000000 ospyata-3.1.0/src/ospyata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-15 08:13:55.000000 ospyata-3.1.0/src/ospyata/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-04-15 08:13:55.000000 ospyata-3.1.0/src/ospyata/osmata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:14:05.045255 ospyata-3.1.0/src/ospyata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-15 08:14:05.000000 ospyata-3.1.0/src/ospyata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-15 08:14:05.000000 ospyata-3.1.0/src/ospyata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 08:14:05.000000 ospyata-3.1.0/src/ospyata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-15 08:14:05.000000 ospyata-3.1.0/src/ospyata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-15 08:14:05.000000 ospyata-3.1.0/src/ospyata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:28:16.665884 ospyata-3.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-23 13:28:05.000000 ospyata-3.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-23 13:28:16.665884 ospyata-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-23 13:28:05.000000 ospyata-3.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-23 13:28:16.665884 ospyata-3.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-23 13:28:05.000000 ospyata-3.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:28:16.661884 ospyata-3.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:28:16.661884 ospyata-3.1.1/src/ospyata/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-23 13:28:05.000000 ospyata-3.1.1/src/ospyata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-23 13:28:05.000000 ospyata-3.1.1/src/ospyata/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5982 2023-04-23 13:28:05.000000 ospyata-3.1.1/src/ospyata/osmata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:28:16.665884 ospyata-3.1.1/src/ospyata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-23 13:28:16.000000 ospyata-3.1.1/src/ospyata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-23 13:28:16.000000 ospyata-3.1.1/src/ospyata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 13:28:16.000000 ospyata-3.1.1/src/ospyata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-23 13:28:16.000000 ospyata-3.1.1/src/ospyata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-23 13:28:16.000000 ospyata-3.1.1/src/ospyata.egg-info/top_level.txt
```

### Comparing `ospyata-3.1.0/LICENSE` & `ospyata-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ospyata-3.1.0/PKG-INFO` & `ospyata-3.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ospyata
-Version: 3.1.0
+Version: 3.1.1
 Summary: Python library for the open source bookmark app Osmata.
 Home-page: https://github.com/aerocyber/ospyata
 Author: aerocyber
 License: MIT License
 Project-URL: Bug Reports, https://github.com/aerocyber/ospyata/issues
 Project-URL: Source, https://github.com/aerocyber/ospyata/
 Keywords: osmata,development,osmata-bindings,osmata-python-bindings,bookmarks,ospyata
```

### Comparing `ospyata-3.1.0/README.md` & `ospyata-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ospyata-3.1.0/setup.py` & `ospyata-3.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # Get the long description from the README file
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 
 setup(
     name='ospyata',
     license="MIT License",
-    version='3.1.0',
+    version='3.1.1',
     description='Python library for the open source bookmark app Osmata.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/aerocyber/ospyata',
     author='aerocyber',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
```

### Comparing `ospyata-3.1.0/src/ospyata/osmata.py` & `ospyata-3.1.1/src/ospyata/osmata.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # This software is released under the MIT License.
 # https://opensource.org/licenses/MIT
 
 import json
 import validators
 from typing import List
 import pathlib
-from jsonschema import validate
 
 
 class OspyataException(Exception):
     pass
 
 
 class Osmata:
@@ -64,45 +63,72 @@
 
     def validate_omio(self, dat: str):
         """Validate an omio file
 
         Args:
             dat (str): The omio string.
         """
-        schema = {
-            "$schema": "https://json-schema.org/draft/2020-12/schema",
-            "$id": "https://example.com/product.schema.json",
-            "title": "Osmations",
-            "description": "A record of all bookmarks.",
-            "type": "object",
-            "properties": {
-                "Name": {
-                    "description": "The unique identifier for a record.",
-                    "type": "string"
-                },
-                "URL": {
-                    "description": "URL associated with the Name.",
-                    "type": "string"
-                },
-                "Categories": {
-                    "description": "Tags for the Record",
-                    "type": "array",
-                    "items": {
-                        "type": "string"
-                    }
-                }
-            },
-            "required": ["Name", "URL"]
-        }
-        try:
-            validate(instance=dat, schema=schema)
-        except Exception as e:
-            return False
-        else:
-            return True
+        # schema = {
+        #     "$schema": "https://json-schema.org/draft/2020-12/schema",
+        #     "$id": "https://example.com/product.schema.json",
+        #     "title": "Osmations",
+        #     "description": "A record of all bookmarks.",
+        #     "type": "object",
+        #     "properties": {
+        #         "Name": {
+        #             "description": "The unique identifier for a record.",
+        #             "type": "string"
+        #         },
+        #         "URL": {
+        #             "description": "URL associated with the Name.",
+        #             "type": "string"
+        #         },
+        #         "Categories": {
+        #             "description": "Tags for the Record",
+        #             "type": "array",
+        #             "items": {
+        #                 "type": "string"
+        #             }
+        #         }
+        #     },
+        #     "required": ["Name", "URL"]
+        # }
+        # try:
+        #     validate(instance=dat, schema=schema)
+        # except Exception as e:
+        #     return False
+        # else:
+        #     return True
+        data = json.loads(dat)
+        _keys = data.keys()
+        _urls = []
+        _is_cat_list = True
+        for record in data:
+            if isinstance(record, str):
+                if isinstance(data[record], dict):
+                    if "URL" in data[record].keys():
+                        if "Categories" in data[record].keys():
+                            if not isinstance(data[record]["Categories"], list):
+                                return False
+                            else:
+                                try:
+                                    _is_url = self.validate_url(data[record]["URL"])
+                                except Exception:
+                                    return False
+                        else:
+                            return False
+                    else:
+                        return False
+                else:
+                    return False
+            else:
+                return False
+        return True
+
+
 
     def dumpOmio(self):
         return json.dumps(self.db)
 
     def loadOmio(self, omio_path):
         if pathlib.Path(omio_path).exists():
             f = open(omio_path, 'r')
```

### Comparing `ospyata-3.1.0/src/ospyata.egg-info/PKG-INFO` & `ospyata-3.1.1/src/ospyata.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ospyata
-Version: 3.1.0
+Version: 3.1.1
 Summary: Python library for the open source bookmark app Osmata.
 Home-page: https://github.com/aerocyber/ospyata
 Author: aerocyber
 License: MIT License
 Project-URL: Bug Reports, https://github.com/aerocyber/ospyata/issues
 Project-URL: Source, https://github.com/aerocyber/ospyata/
 Keywords: osmata,development,osmata-bindings,osmata-python-bindings,bookmarks,ospyata
```

