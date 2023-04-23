# Comparing `tmp/findmyorder-0.0.6.tar.gz` & `tmp/findmyorder-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findmyorder-0.0.6.tar", max compression
+gzip compressed data, was "findmyorder-0.0.7.tar", max compression
```

## Comparing `findmyorder-0.0.6.tar` & `findmyorder-0.0.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-04-23 13:27:46.431849 findmyorder-0.0.6/LICENSE
--rw-r--r--   0        0        0     1426 2023-04-23 13:27:46.431849 findmyorder-0.0.6/README.md
--rw-r--r--   0        0        0      103 2023-04-23 13:27:47.111855 findmyorder-0.0.6/findmyorder/__init__.py
--rw-r--r--   0        0        0      219 2023-04-23 13:27:46.431849 findmyorder-0.0.6/findmyorder/config.py
--rw-r--r--   0        0        0      204 2023-04-23 13:27:46.431849 findmyorder-0.0.6/findmyorder/core.toml
--rw-r--r--   0        0        0     2578 2023-04-23 13:27:46.431849 findmyorder-0.0.6/findmyorder/main.py
--rw-r--r--   0        0        0      962 2023-04-23 13:27:47.111855 findmyorder-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2199 1970-01-01 00:00:00.000000 findmyorder-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-23 13:38:26.794031 findmyorder-0.0.7/LICENSE
+-rw-r--r--   0        0        0     1426 2023-04-23 13:38:26.794031 findmyorder-0.0.7/README.md
+-rw-r--r--   0        0        0      103 2023-04-23 13:38:27.530042 findmyorder-0.0.7/findmyorder/__init__.py
+-rw-r--r--   0        0        0      219 2023-04-23 13:38:26.794031 findmyorder-0.0.7/findmyorder/config.py
+-rw-r--r--   0        0        0      204 2023-04-23 13:38:26.794031 findmyorder-0.0.7/findmyorder/core.toml
+-rw-r--r--   0        0        0     2592 2023-04-23 13:38:26.794031 findmyorder-0.0.7/findmyorder/main.py
+-rw-r--r--   0        0        0      962 2023-04-23 13:38:27.530042 findmyorder-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2199 1970-01-01 00:00:00.000000 findmyorder-0.0.7/PKG-INFO
```

### Comparing `findmyorder-0.0.6/LICENSE` & `findmyorder-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `findmyorder-0.0.6/README.md` & `findmyorder-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `findmyorder-0.0.6/findmyorder/main.py` & `findmyorder-0.0.7/findmyorder/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import asyncio, logging, re
 from datetime import datetime
-from config import settings
+
+
 
 from findmyorder import __version__
+from findmyorder.config import settings
 
 # import pyparsing as pp
 
 # from translate import Translator
 # translator = Translator(to_lang="en")
```

### Comparing `findmyorder-0.0.6/pyproject.toml` & `findmyorder-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "findmyorder"
-version = "0.0.6"
+version = "0.0.7"
 description = "A python package to identify and parse order for trade execution."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["trading", "order", "trade","buy","sell"]
```

### Comparing `findmyorder-0.0.6/PKG-INFO` & `findmyorder-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findmyorder
-Version: 0.0.6
+Version: 0.0.7
 Summary: A python package to identify and parse order for trade execution.
 License: MIT
 Keywords: trading,order,trade,buy,sell
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

