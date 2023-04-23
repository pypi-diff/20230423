# Comparing `tmp/html2info-0.1.4.tar.gz` & `tmp/html2info-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "html2info-0.1.4.tar", last modified: Sun Apr 23 00:29:52 2023, max compression
+gzip compressed data, was "html2info-0.1.5.tar", last modified: Sun Apr 23 00:43:56 2023, max compression
```

## Comparing `html2info-0.1.4.tar` & `html2info-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-04-23 00:29:52.377436 html2info-0.1.4/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     6013 2023-04-23 00:29:52.377436 html2info-0.1.4/PKG-INFO
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     5278 2023-04-20 20:54:37.000000 html2info-0.1.4/README.md
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-04-23 00:29:52.377436 html2info-0.1.4/html2info/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)        0 2023-04-19 18:56:39.000000 html2info-0.1.4/html2info/__init__.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     5002 2023-04-23 00:28:59.000000 html2info-0.1.4/html2info/linkedin.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      396 2023-04-23 00:22:17.000000 html2info-0.1.4/html2info/types.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      190 2023-04-19 19:16:29.000000 html2info-0.1.4/html2info/utils.py
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-04-23 00:29:52.377436 html2info-0.1.4/html2info.egg-info/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     6013 2023-04-23 00:29:52.000000 html2info-0.1.4/html2info.egg-info/PKG-INFO
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      279 2023-04-23 00:29:52.000000 html2info-0.1.4/html2info.egg-info/SOURCES.txt
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)        1 2023-04-23 00:29:52.000000 html2info-0.1.4/html2info.egg-info/dependency_links.txt
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       23 2023-04-23 00:29:52.000000 html2info-0.1.4/html2info.egg-info/requires.txt
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       10 2023-04-23 00:29:52.000000 html2info-0.1.4/html2info.egg-info/top_level.txt
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1478 2023-04-19 22:54:36.000000 html2info-0.1.4/pyproject.toml
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       38 2023-04-23 00:29:52.377436 html2info-0.1.4/setup.cfg
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1360 2023-04-23 00:29:15.000000 html2info-0.1.4/setup.py
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-04-23 00:43:56.810199 html2info-0.1.5/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     6013 2023-04-23 00:43:56.810199 html2info-0.1.5/PKG-INFO
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     5278 2023-04-20 20:54:37.000000 html2info-0.1.5/README.md
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-04-23 00:43:56.810199 html2info-0.1.5/html2info/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)        0 2023-04-19 18:56:39.000000 html2info-0.1.5/html2info/__init__.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     5002 2023-04-23 00:28:59.000000 html2info-0.1.5/html2info/linkedin.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      439 2023-04-23 00:43:09.000000 html2info-0.1.5/html2info/types.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      190 2023-04-19 19:16:29.000000 html2info-0.1.5/html2info/utils.py
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-04-23 00:43:56.810199 html2info-0.1.5/html2info.egg-info/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     6013 2023-04-23 00:43:56.000000 html2info-0.1.5/html2info.egg-info/PKG-INFO
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      279 2023-04-23 00:43:56.000000 html2info-0.1.5/html2info.egg-info/SOURCES.txt
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)        1 2023-04-23 00:43:56.000000 html2info-0.1.5/html2info.egg-info/dependency_links.txt
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       23 2023-04-23 00:43:56.000000 html2info-0.1.5/html2info.egg-info/requires.txt
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       10 2023-04-23 00:43:56.000000 html2info-0.1.5/html2info.egg-info/top_level.txt
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1475 2023-04-23 00:41:00.000000 html2info-0.1.5/pyproject.toml
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       38 2023-04-23 00:43:56.810199 html2info-0.1.5/setup.cfg
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1360 2023-04-23 00:43:25.000000 html2info-0.1.5/setup.py
```

### Comparing `html2info-0.1.4/PKG-INFO` & `html2info-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html2info
-Version: 0.1.4
+Version: 0.1.5
 Summary: A package to parse raw HTML and return structured information.
 Author: Vladimir Iglovikov
 Author-email: iglovikov@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `html2info-0.1.4/README.md` & `html2info-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `html2info-0.1.4/html2info/linkedin.py` & `html2info-0.1.5/html2info/linkedin.py`

 * *Files identical despite different names*

### Comparing `html2info-0.1.4/html2info.egg-info/PKG-INFO` & `html2info-0.1.5/html2info.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html2info
-Version: 0.1.4
+Version: 0.1.5
 Summary: A package to parse raw HTML and return structured information.
 Author: Vladimir Iglovikov
 Author-email: iglovikov@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `html2info-0.1.4/pyproject.toml` & `html2info-0.1.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # NOTE: you have to use single-quoted strings in TOML for regular expressions.
 # It's the equivalent of r-strings in Python.  Multiline strings are treated as
 # verbose regular expressions by Black.  Use [ ] to denote a significant space
 # character.
 
 [tool.black]
 line-length = 120
-target-version = ['py310']
+target-version = ['py39']
 include = '\.pyi?$'
 exclude = '''
 /(
     \.eggs
   | \.git
   | \.hg
   | \.mypy_cache
@@ -59,11 +59,11 @@
 
 extend-exclude = ["tests", "setup.py"]
 per-file-ignores = { }
 
 # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 
-# Assume Python 3.10
-target-version = "py310"
+# Assume Python 3.9
+target-version = "py39"
 
 fix = true
```

### Comparing `html2info-0.1.4/setup.py` & `html2info-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="html2info",  # Replace with your package name
-    version="0.1.4",  # Replace with your package version
+    version="0.1.5",  # Replace with your package version
     author="Vladimir Iglovikov",  # Replace with your name
     author_email="iglovikov@gmail.com",  # Replace with your email
     description="A package to parse raw HTML and return structured information.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(exclude=["tests"]),
     classifiers=[
```

