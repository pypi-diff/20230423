# Comparing `tmp/findmyorder-0.0.1.tar.gz` & `tmp/findmyorder-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findmyorder-0.0.1.tar", max compression
+gzip compressed data, was "findmyorder-0.0.2.tar", max compression
```

## Comparing `findmyorder-0.0.1.tar` & `findmyorder-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-04-22 17:19:50.513890 findmyorder-0.0.1/LICENSE
--rw-r--r--   0        0        0     1372 2023-04-22 17:19:50.513890 findmyorder-0.0.1/README.md
--rw-r--r--   0        0        0       97 2023-04-22 17:19:51.417882 findmyorder-0.0.1/findmyorder/__init__.py
--rw-r--r--   0        0        0      147 2023-04-22 17:19:50.513890 findmyorder-0.0.1/findmyorder/config.py
--rw-r--r--   0        0        0       79 2023-04-22 17:19:50.513890 findmyorder-0.0.1/findmyorder/core.toml
--rw-r--r--   0        0        0      781 2023-04-22 17:19:50.513890 findmyorder-0.0.1/findmyorder/main.py
--rw-r--r--   0        0        0      908 2023-04-22 17:19:51.417882 findmyorder-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2115 1970-01-01 00:00:00.000000 findmyorder-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-23 06:34:46.562026 findmyorder-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1372 2023-04-23 06:34:46.562026 findmyorder-0.0.2/README.md
+-rw-r--r--   0        0        0      103 2023-04-23 06:34:47.326040 findmyorder-0.0.2/findmyorder/__init__.py
+-rw-r--r--   0        0        0      146 2023-04-23 06:34:46.562026 findmyorder-0.0.2/findmyorder/config.py
+-rw-r--r--   0        0        0     2106 2023-04-23 06:34:46.562026 findmyorder-0.0.2/findmyorder/main.py
+-rw-r--r--   0        0        0       77 2023-04-23 06:34:46.562026 findmyorder-0.0.2/findmyorder/settings.toml
+-rw-r--r--   0        0        0      925 2023-04-23 06:34:47.326040 findmyorder-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2140 1970-01-01 00:00:00.000000 findmyorder-0.0.2/PKG-INFO
```

### Comparing `findmyorder-0.0.1/LICENSE` & `findmyorder-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `findmyorder-0.0.1/README.md` & `findmyorder-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `findmyorder-0.0.1/pyproject.toml` & `findmyorder-0.0.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "findmyorder"
-version = "0.0.1"
+version = "0.0.2"
 description = "A python package to identify order and parse data"
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 
 [tool.poetry.urls]
@@ -12,14 +12,16 @@
 "Support" =  "https://github.com/mraniki/findmyorder/discussions"
 "Issues" =  "https://github.com/mraniki/findmyorder/issues"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.11"
 asyncio = "*"
 pyparsing = "*"
+translate = "*"
+
 
 [tool.poetry.dev-dependencies]
 python-semantic-release = "*"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `findmyorder-0.0.1/PKG-INFO` & `findmyorder-0.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: findmyorder
-Version: 0.0.1
+Version: 0.0.2
 Summary: A python package to identify order and parse data
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: asyncio
 Requires-Dist: pyparsing
+Requires-Dist: translate
 Project-URL: Changelog, https://github.com/mraniki/findmyorder/blob/dev/CHANGELOG.rst
 Project-URL: Issues, https://github.com/mraniki/findmyorder/issues
 Project-URL: Support, https://github.com/mraniki/findmyorder/discussions
 Description-Content-Type: text/markdown
 
 # Find my order.
```

