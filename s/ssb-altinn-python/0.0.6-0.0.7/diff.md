# Comparing `tmp/ssb_altinn_python-0.0.6.tar.gz` & `tmp/ssb_altinn_python-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssb_altinn_python-0.0.6.tar", max compression
+gzip compressed data, was "ssb_altinn_python-0.0.7.tar", max compression
```

## Comparing `ssb_altinn_python-0.0.6.tar` & `ssb_altinn_python-0.0.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1078 2023-04-23 15:56:36.948973 ssb_altinn_python-0.0.6/LICENSE
--rw-r--r--   0        0        0     3329 2023-04-23 15:56:36.948973 ssb_altinn_python-0.0.6/README.md
--rw-r--r--   0        0        0     1936 2023-04-23 15:56:51.288977 ssb_altinn_python-0.0.6/pyproject.toml
--rw-r--r--   0        0        0       78 2023-04-23 15:56:36.948973 ssb_altinn_python-0.0.6/src/altinn/__init__.py
--rw-r--r--   0        0        0      116 2023-04-23 15:56:36.948973 ssb_altinn_python-0.0.6/src/altinn/__main__.py
--rw-r--r--   0        0        0     2192 2023-04-23 15:56:51.288977 ssb_altinn_python-0.0.6/src/altinn/file.py
--rw-r--r--   0        0        0      419 2023-04-23 15:56:36.948973 ssb_altinn_python-0.0.6/src/altinn/flatten.py
--rw-r--r--   0        0        0       35 2023-04-23 15:56:36.948973 ssb_altinn_python-0.0.6/src/altinn/parser.py
--rw-r--r--   0        0        0        0 2023-04-23 15:56:36.948973 ssb_altinn_python-0.0.6/src/altinn/py.typed
--rw-r--r--   0        0        0       56 2023-04-23 15:56:36.948973 ssb_altinn_python-0.0.6/src/altinn/utils.py
--rw-r--r--   0        0        0     4204 1970-01-01 00:00:00.000000 ssb_altinn_python-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-04-23 16:45:42.679258 ssb_altinn_python-0.0.7/LICENSE
+-rw-r--r--   0        0        0     3329 2023-04-23 16:45:42.679258 ssb_altinn_python-0.0.7/README.md
+-rw-r--r--   0        0        0     1936 2023-04-23 16:45:58.031396 ssb_altinn_python-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0       78 2023-04-23 16:45:42.679258 ssb_altinn_python-0.0.7/src/altinn/__init__.py
+-rw-r--r--   0        0        0      116 2023-04-23 16:45:42.679258 ssb_altinn_python-0.0.7/src/altinn/__main__.py
+-rw-r--r--   0        0        0     2473 2023-04-23 16:45:58.031396 ssb_altinn_python-0.0.7/src/altinn/file.py
+-rw-r--r--   0        0        0      419 2023-04-23 16:45:42.679258 ssb_altinn_python-0.0.7/src/altinn/flatten.py
+-rw-r--r--   0        0        0       35 2023-04-23 16:45:42.679258 ssb_altinn_python-0.0.7/src/altinn/parser.py
+-rw-r--r--   0        0        0        0 2023-04-23 16:45:42.679258 ssb_altinn_python-0.0.7/src/altinn/py.typed
+-rw-r--r--   0        0        0       56 2023-04-23 16:45:42.679258 ssb_altinn_python-0.0.7/src/altinn/utils.py
+-rw-r--r--   0        0        0     4204 1970-01-01 00:00:00.000000 ssb_altinn_python-0.0.7/PKG-INFO
```

### Comparing `ssb_altinn_python-0.0.6/LICENSE` & `ssb_altinn_python-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ssb_altinn_python-0.0.6/README.md` & `ssb_altinn_python-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ssb_altinn_python-0.0.6/pyproject.toml` & `ssb_altinn_python-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ssb-altinn-python"
-version = "0.0.6"
+version = "0.0.7"
 description = "SSB Altinn Python"
 authors = ["Øyvind Bruer-Skarsbø <obr@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/skars82/ssb-altinn-python"
 repository = "https://github.com/skars82/ssb-altinn-python"
 documentation = "https://ssb-altinn-python.readthedocs.io"
```

### Comparing `ssb_altinn_python-0.0.6/src/altinn/file.py` & `ssb_altinn_python-0.0.7/src/altinn/file.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """This module contains the main function for running the Altinn application."""
 
 import os
 from typing import Optional
 
 from dapla import FileClient
+from defusedxml.ElementTree import ParseError
+from defusedxml.ElementTree import parse
 from defusedxml.minidom import parseString
 
 
 def main() -> None:
     """Placeholder function for the main function.
 
     This function is called when the altinn package is run as a script.
@@ -65,7 +67,16 @@
         print(pretty_xml)
 
     def print(self) -> None:
         """Print unformatted version of an XML file."""
         fs = FileClient.get_gcs_file_system()
         file = fs.cat_file(self.file_path)
         print(file.decode())
+
+    def validate(self) -> bool:
+        """Validate the XML file."""
+        try:
+            parse(self.file_path)
+            return True
+
+        except ParseError:
+            return False
```

### Comparing `ssb_altinn_python-0.0.6/PKG-INFO` & `ssb_altinn_python-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssb-altinn-python
-Version: 0.0.6
+Version: 0.0.7
 Summary: SSB Altinn Python
 Home-page: https://github.com/skars82/ssb-altinn-python
 License: MIT
 Author: Øyvind Bruer-Skarsbø
 Author-email: obr@ssb.no
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
```

