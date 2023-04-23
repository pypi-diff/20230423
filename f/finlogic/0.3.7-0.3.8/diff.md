# Comparing `tmp/FinLogic-0.3.7.tar.gz` & `tmp/finlogic-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FinLogic-0.3.7.tar", last modified: Sat Apr 22 03:14:58 2023, max compression
+gzip compressed data, was "finlogic-0.3.8.tar", last modified: Sun Apr 23 12:24:42 2023, max compression
```

## Comparing `FinLogic-0.3.7.tar` & `finlogic-0.3.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1072 2023-03-19 09:29:48.277335 FinLogic-0.3.7/LICENSE
--rw-r--r--   0        0        0    10060 2023-04-22 03:12:14.634867 FinLogic-0.3.7/README.md
--rw-r--r--   0        0        0      423 2023-04-22 03:12:14.634867 FinLogic-0.3.7/finlogic/__init__.py
--rw-r--r--   0        0        0    22078 2023-04-22 03:12:14.634867 FinLogic-0.3.7/finlogic/company.py
--rw-r--r--   0        0        0     1024 2023-04-22 03:12:14.634867 FinLogic-0.3.7/finlogic/config.py
--rw-r--r--   0        0        0     9283 2023-04-22 03:12:14.634867 FinLogic-0.3.7/finlogic/cvm.py
--rw-r--r--   0        0        0     6806 2023-04-22 03:12:14.634867 FinLogic-0.3.7/finlogic/database.py
--rw-r--r--   0        0        0      996 2023-04-02 12:44:27.971854 FinLogic-0.3.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-19 09:29:48.278335 FinLogic-0.3.7/tests/__init__.py
--rw-r--r--   0        0        0     2125 2023-04-14 09:12:15.664615 FinLogic-0.3.7/tests/test_company.py
--rw-r--r--   0        0        0      598 2023-04-22 03:12:14.635867 FinLogic-0.3.7/tests/test_database.py
--rw-r--r--   0        0        0    10700 1970-01-01 00:00:00.000000 FinLogic-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-03-19 09:29:48.277335 finlogic-0.3.8/LICENSE
+-rw-r--r--   0        0        0    10060 2023-04-22 03:12:14.634867 finlogic-0.3.8/README.md
+-rw-r--r--   0        0        0      423 2023-04-22 17:40:14.252933 finlogic-0.3.8/finlogic/__init__.py
+-rw-r--r--   0        0        0    22078 2023-04-22 03:12:14.634867 finlogic-0.3.8/finlogic/company.py
+-rw-r--r--   0        0        0     1024 2023-04-22 03:12:14.634867 finlogic-0.3.8/finlogic/config.py
+-rw-r--r--   0        0        0     9283 2023-04-22 03:12:14.634867 finlogic-0.3.8/finlogic/cvm.py
+-rw-r--r--   0        0        0     6806 2023-04-22 03:12:14.634867 finlogic-0.3.8/finlogic/database.py
+-rw-r--r--   0        0        0      989 2023-04-23 12:24:42.046992 finlogic-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-19 09:29:48.278335 finlogic-0.3.8/tests/__init__.py
+-rw-r--r--   0        0        0     2125 2023-04-14 09:12:15.664615 finlogic-0.3.8/tests/test_company.py
+-rw-r--r--   0        0        0      598 2023-04-22 03:12:14.635867 finlogic-0.3.8/tests/test_database.py
+-rw-r--r--   0        0        0    12080 1970-01-01 00:00:00.000000 finlogic-0.3.8/PKG-INFO
```

### Comparing `FinLogic-0.3.7/LICENSE` & `finlogic-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `FinLogic-0.3.7/README.md` & `finlogic-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `FinLogic-0.3.7/finlogic/company.py` & `finlogic-0.3.8/finlogic/company.py`

 * *Files identical despite different names*

### Comparing `FinLogic-0.3.7/finlogic/config.py` & `finlogic-0.3.8/finlogic/config.py`

 * *Files identical despite different names*

### Comparing `FinLogic-0.3.7/finlogic/cvm.py` & `finlogic-0.3.8/finlogic/cvm.py`

 * *Files identical despite different names*

### Comparing `FinLogic-0.3.7/finlogic/database.py` & `finlogic-0.3.8/finlogic/database.py`

 * *Files identical despite different names*

### Comparing `FinLogic-0.3.7/pyproject.toml` & `finlogic-0.3.8/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+[build-system]
+requires = [
+    "pdm-backend",
+]
+build-backend = "pdm.backend"
+
 [project]
 name = "FinLogic"
 dynamic = []
 description = "Finance toolkit for listed Brazilian companies"
 requires-python = ">=3.10"
 readme = "README.md"
 keywords = [
@@ -18,29 +24,23 @@
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
     "pandas>=1.4.0",
     "requests>=2.27.0",
     "zstandard>=0.17.0",
 ]
-version = "0.3.7"
+version = "0.3.8"
 
 [project.license]
 file = "LICENSE"
 
 [project.optional-dependencies]
 test = [
     "pytest>=7.0.0",
 ]
 
 [project.urls]
 repository = "https://github.com/crdcj/FinLogic"
 
-[build-system]
-requires = [
-    "pdm-pep517>=1.0",
-]
-build-backend = "pdm.pep517.api"
-
 [tool.pdm.version]
 source = "file"
 path = "finlogic/__init__.py"
```

### Comparing `FinLogic-0.3.7/tests/test_company.py` & `finlogic-0.3.8/tests/test_company.py`

 * *Files identical despite different names*

### Comparing `FinLogic-0.3.7/tests/test_database.py` & `finlogic-0.3.8/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `FinLogic-0.3.7/PKG-INFO` & `finlogic-0.3.8/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,46 @@
 Metadata-Version: 2.1
-Name: FinLogic
-Version: 0.3.7
+Name: finlogic
+Version: 0.3.8
 Summary: Finance toolkit for listed Brazilian companies
 Keywords: pandas, cvm, finance, investment, accounting
-Author-email: Carlos Carvalho <cr.cj@outlook.com>
-Requires-Python: >=3.10
+Author-Email: Carlos Carvalho <cr.cj@outlook.com>
+License: MIT License
+        
+        Copyright (c) 2022 Carlos Carvalho
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
+Classifier: Topic :: Office/Business :: Financial :: Accounting
+Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Classifier: Topic :: Office/Business :: Financial :: Accounting
-Classifier: Topic :: Office/Business :: Financial :: Investment
+Project-URL: Repository, https://github.com/crdcj/FinLogic
+Requires-Python: >=3.10
+Requires-Dist: pandas>=1.4.0
+Requires-Dist: requests>=2.27.0
+Requires-Dist: zstandard>=0.17.0
+Requires-Dist: pytest>=7.0.0; extra == "test"
 Provides-Extra: test
-Project-URL: repository, https://github.com/crdcj/FinLogic
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://img.shields.io/pypi/v/finlogic.svg)](https://pypi.python.org/pypi/finlogic)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/finlogic/badges/version.svg)](https://anaconda.org/conda-forge/finlogic)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/finlogic.svg)](https://pypi.python.org/pypi/finlogic)
 [![Python Version](https://img.shields.io/pypi/pyversions/finlogic)](https://www.python.org/)
 [![Anaconda License](https://anaconda.org/conda-forge/finlogic/badges/license.svg)](https://anaconda.org/conda-forge/finlogic)
@@ -215,8 +240,7 @@
 | net_margin                   |      0.135 |      0.022 |      0.236 |
 
 ---
 
 P.S.: All contributors are welcome, from beginner to advanced.
 
 **Felipe Costa and Carlos Carvalho**
-
```

#### html2text {}

```diff
@@ -1,17 +1,33 @@
-Metadata-Version: 2.1 Name: FinLogic Version: 0.3.7 Summary: Finance toolkit
+Metadata-Version: 2.1 Name: finlogic Version: 0.3.8 Summary: Finance toolkit
 for listed Brazilian companies Keywords: pandas, cvm, finance, investment,
-accounting Author-email: Carlos Carvalho
-cj@outlook.com> Requires-Python: >=3.10 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3.12 Classifier: Topic :: Office/Business ::
-Financial :: Accounting Classifier: Topic :: Office/Business :: Financial ::
-Investment Provides-Extra: test Project-URL: repository, https://github.com/
-crdcj/FinLogic Description-Content-Type: text/markdown [![PyPI version](https:/
-/img.shields.io/pypi/v/finlogic.svg)](https://pypi.python.org/pypi/finlogic) [!
+accounting Author-Email: Carlos Carvalho
+cj@outlook.com> License: MIT License Copyright (c) 2022 Carlos Carvalho
+Permission is hereby granted, free of charge, to any person obtaining a copy of
+this software and associated documentation files (the "Software"), to deal in
+the Software without restriction, including without limitation the rights to
+use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
+of the Software, and to permit persons to whom the Software is furnished to do
+so, subject to the following conditions: The above copyright notice and this
+permission notice shall be included in all copies or substantial portions of
+the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO
+EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
+OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
+ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE. Classifier: Topic :: Office/Business :: Financial ::
+Accounting Classifier: Topic :: Office/Business :: Financial :: Investment
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
+Project-URL: Repository, https://github.com/crdcj/FinLogic Requires-Python:
+>=3.10 Requires-Dist: pandas>=1.4.0 Requires-Dist: requests>=2.27.0 Requires-
+Dist: zstandard>=0.17.0 Requires-Dist: pytest>=7.0.0; extra == "test" Provides-
+Extra: test Description-Content-Type: text/markdown [![PyPI version](https://
+img.shields.io/pypi/v/finlogic.svg)](https://pypi.python.org/pypi/finlogic) [!
 [Anaconda-Server Badge](https://anaconda.org/conda-forge/finlogic/badges/
 version.svg)](https://anaconda.org/conda-forge/finlogic) [![PyPI Downloads]
 (https://img.shields.io/pypi/dm/finlogic.svg)](https://pypi.python.org/pypi/
 finlogic) [![Python Version](https://img.shields.io/pypi/pyversions/finlogic)]
 (https://www.python.org/) [![Anaconda License](https://anaconda.org/conda-
 forge/finlogic/badges/license.svg)](https://anaconda.org/conda-forge/finlogic)
 [![Code Style: black](https://img.shields.io/badge/code%20style-black-
```

