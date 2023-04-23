# Comparing `tmp/ssb_altinn_python-0.0.5.tar.gz` & `tmp/ssb_altinn_python-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssb_altinn_python-0.0.5.tar", max compression
+gzip compressed data, was "ssb_altinn_python-0.0.6.tar", max compression
```

## Comparing `ssb_altinn_python-0.0.5.tar` & `ssb_altinn_python-0.0.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1078 2023-04-16 19:33:04.808758 ssb_altinn_python-0.0.5/LICENSE
--rw-r--r--   0        0        0     2844 2023-04-16 19:33:17.780731 ssb_altinn_python-0.0.5/README.md
--rw-r--r--   0        0        0     1954 2023-04-16 19:33:17.784731 ssb_altinn_python-0.0.5/pyproject.toml
--rw-r--r--   0        0        0       78 2023-04-16 19:33:17.784731 ssb_altinn_python-0.0.5/src/altinn/__init__.py
--rw-r--r--   0        0        0      116 2023-04-16 19:33:17.784731 ssb_altinn_python-0.0.5/src/altinn/__main__.py
--rw-r--r--   0        0        0     1988 2023-04-16 19:33:17.784731 ssb_altinn_python-0.0.5/src/altinn/file.py
--rw-r--r--   0        0        0      419 2023-04-16 19:33:17.784731 ssb_altinn_python-0.0.5/src/altinn/flatten.py
--rw-r--r--   0        0        0       35 2023-04-16 19:33:17.784731 ssb_altinn_python-0.0.5/src/altinn/parser.py
--rw-r--r--   0        0        0        0 2023-04-16 19:33:04.808758 ssb_altinn_python-0.0.5/src/altinn/py.typed
--rw-r--r--   0        0        0       56 2023-04-16 19:33:17.784731 ssb_altinn_python-0.0.5/src/altinn/utils.py
--rw-r--r--   0        0        0     3750 1970-01-01 00:00:00.000000 ssb_altinn_python-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-04-23 15:56:36.948973 ssb_altinn_python-0.0.6/LICENSE
+-rw-r--r--   0        0        0     3329 2023-04-23 15:56:36.948973 ssb_altinn_python-0.0.6/README.md
+-rw-r--r--   0        0        0     1936 2023-04-23 15:56:51.288977 ssb_altinn_python-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0       78 2023-04-23 15:56:36.948973 ssb_altinn_python-0.0.6/src/altinn/__init__.py
+-rw-r--r--   0        0        0      116 2023-04-23 15:56:36.948973 ssb_altinn_python-0.0.6/src/altinn/__main__.py
+-rw-r--r--   0        0        0     2192 2023-04-23 15:56:51.288977 ssb_altinn_python-0.0.6/src/altinn/file.py
+-rw-r--r--   0        0        0      419 2023-04-23 15:56:36.948973 ssb_altinn_python-0.0.6/src/altinn/flatten.py
+-rw-r--r--   0        0        0       35 2023-04-23 15:56:36.948973 ssb_altinn_python-0.0.6/src/altinn/parser.py
+-rw-r--r--   0        0        0        0 2023-04-23 15:56:36.948973 ssb_altinn_python-0.0.6/src/altinn/py.typed
+-rw-r--r--   0        0        0       56 2023-04-23 15:56:36.948973 ssb_altinn_python-0.0.6/src/altinn/utils.py
+-rw-r--r--   0        0        0     4204 1970-01-01 00:00:00.000000 ssb_altinn_python-0.0.6/PKG-INFO
```

### Comparing `ssb_altinn_python-0.0.5/LICENSE` & `ssb_altinn_python-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ssb_altinn_python-0.0.5/README.md` & `ssb_altinn_python-0.0.6/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -24,36 +24,42 @@
 ## Features
 
 This is work-in-progress Python-package for dealing with xml-data from Altinn3.
 
 ```python
 from altinn import FileInfo
 
-x = FileInfo(
+form = FileInfo(
     "gs://ssb-prod-dapla-felles-data-delt/altinn3/form_dc551844cd74.xml"
 )
 
-x.filename()
-# Returns the filename: form_dc551844cd74
+# Get file filename without '.xml'-postfix
+form.filename()
+# Returns: 'form_dc551844cd74'
+
+# Print a nicely formatted version of the file
+form.pretty_print()
 ```
 
 ## Requirements
 
-s
-
-- TODO
+- dapla-toolbelt >=1.6.2,<2.0.0
+- defusedxml >=0.7.1,<0.8.0
+- pytest >=7.2.2,<8.0.0
 
 ## Installation
 
-You can install _SSB Altinn Python_ via [pip] from [PyPI]:
+You can install _SSB Altinn Python_ via [poetry] from [PyPI]:
 
 ```console
-pip install ssb-altinn-python
+poetry add ssb-altinn-python
 ```
 
+To install this in the Jupyter-environment on Dapla, where it is ment to be used, it is required to install it in an virtual environment. It is recommended to do this in an [ssb-project](https://manual.dapla.ssb.no/jobbe-med-kode.html) where the preferred tool is [poetry](https://python-poetry.org/).
+
 ## Usage
 
 Please see the [Command-line Reference] for details.
 
 ## Contributing
 
 Contributions are very welcome.
```

### Comparing `ssb_altinn_python-0.0.5/pyproject.toml` & `ssb_altinn_python-0.0.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ssb-altinn-python"
-version = "0.0.5"
+version = "0.0.6"
 description = "SSB Altinn Python"
 authors = ["Øyvind Bruer-Skarsbø <obr@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/skars82/ssb-altinn-python"
 repository = "https://github.com/skars82/ssb-altinn-python"
 documentation = "https://ssb-altinn-python.readthedocs.io"
@@ -16,15 +16,14 @@
 ]
 
 [tool.poetry.urls]
 Changelog = "https://github.com/skars82/ssb-altinn-python/releases"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-click = ">=8.0.1"
 pytest = "^7.2.2"
 dapla-toolbelt = "^1.6.2"
 defusedxml = "^0.7.1"
 
 [tool.poetry.dev-dependencies]
 Pygments = ">=2.10.0"
 black = ">=21.10b0"
```

### Comparing `ssb_altinn_python-0.0.5/src/altinn/file.py` & `ssb_altinn_python-0.0.6/src/altinn/file.py`

 * *Files 10% similar despite different names*

```diff
@@ -59,7 +59,13 @@
 
     def pretty_print(self) -> None:
         """Print formatted version of an xml-file."""
         fs = FileClient.get_gcs_file_system()
         dom = parseString(fs.cat_file(self.file_path))
         pretty_xml = dom.toprettyxml(indent="  ")
         print(pretty_xml)
+
+    def print(self) -> None:
+        """Print unformatted version of an XML file."""
+        fs = FileClient.get_gcs_file_system()
+        file = fs.cat_file(self.file_path)
+        print(file.decode())
```

### Comparing `ssb_altinn_python-0.0.5/PKG-INFO` & `ssb_altinn_python-0.0.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: ssb-altinn-python
-Version: 0.0.5
+Version: 0.0.6
 Summary: SSB Altinn Python
 Home-page: https://github.com/skars82/ssb-altinn-python
 License: MIT
 Author: Øyvind Bruer-Skarsbø
 Author-email: obr@ssb.no
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: click (>=8.0.1)
 Requires-Dist: dapla-toolbelt (>=1.6.2,<2.0.0)
 Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
 Requires-Dist: pytest (>=7.2.2,<8.0.0)
 Project-URL: Changelog, https://github.com/skars82/ssb-altinn-python/releases
 Project-URL: Documentation, https://ssb-altinn-python.readthedocs.io
 Project-URL: Repository, https://github.com/skars82/ssb-altinn-python
 Description-Content-Type: text/markdown
@@ -47,36 +46,42 @@
 ## Features
 
 This is work-in-progress Python-package for dealing with xml-data from Altinn3.
 
 ```python
 from altinn import FileInfo
 
-x = FileInfo(
+form = FileInfo(
     "gs://ssb-prod-dapla-felles-data-delt/altinn3/form_dc551844cd74.xml"
 )
 
-x.filename()
-# Returns the filename: form_dc551844cd74
+# Get file filename without '.xml'-postfix
+form.filename()
+# Returns: 'form_dc551844cd74'
+
+# Print a nicely formatted version of the file
+form.pretty_print()
 ```
 
 ## Requirements
 
-s
-
-- TODO
+- dapla-toolbelt >=1.6.2,<2.0.0
+- defusedxml >=0.7.1,<0.8.0
+- pytest >=7.2.2,<8.0.0
 
 ## Installation
 
-You can install _SSB Altinn Python_ via [pip] from [PyPI]:
+You can install _SSB Altinn Python_ via [poetry] from [PyPI]:
 
 ```console
-pip install ssb-altinn-python
+poetry add ssb-altinn-python
 ```
 
+To install this in the Jupyter-environment on Dapla, where it is ment to be used, it is required to install it in an virtual environment. It is recommended to do this in an [ssb-project](https://manual.dapla.ssb.no/jobbe-med-kode.html) where the preferred tool is [poetry](https://python-poetry.org/).
+
 ## Usage
 
 Please see the [Command-line Reference] for details.
 
 ## Contributing
 
 Contributions are very welcome.
```

