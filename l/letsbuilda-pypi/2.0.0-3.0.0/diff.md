# Comparing `tmp/letsbuilda-pypi-2.0.0.tar.gz` & `tmp/letsbuilda-pypi-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "letsbuilda-pypi-2.0.0.tar", last modified: Sat Apr 15 00:40:40 2023, max compression
+gzip compressed data, was "letsbuilda-pypi-3.0.0.tar", last modified: Sun Apr 23 03:08:03 2023, max compression
```

## Comparing `letsbuilda-pypi-2.0.0.tar` & `letsbuilda-pypi-3.0.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:40:40.792339 letsbuilda-pypi-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-15 00:40:26.000000 letsbuilda-pypi-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-15 00:40:40.792339 letsbuilda-pypi-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-15 00:40:26.000000 letsbuilda-pypi-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-15 00:40:26.000000 letsbuilda-pypi-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 00:40:40.792339 letsbuilda-pypi-2.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:40:40.788339 letsbuilda-pypi-2.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:40:40.788339 letsbuilda-pypi-2.0.0/src/letsbuilda/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:40:40.792339 letsbuilda-pypi-2.0.0/src/letsbuilda/pypi/
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-04-15 00:40:26.000000 letsbuilda-pypi-2.0.0/src/letsbuilda/pypi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:40:40.792339 letsbuilda-pypi-2.0.0/src/letsbuilda_pypi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-15 00:40:40.000000 letsbuilda-pypi-2.0.0/src/letsbuilda_pypi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-15 00:40:40.000000 letsbuilda-pypi-2.0.0/src/letsbuilda_pypi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 00:40:40.000000 letsbuilda-pypi-2.0.0/src/letsbuilda_pypi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-15 00:40:40.000000 letsbuilda-pypi-2.0.0/src/letsbuilda_pypi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-15 00:40:40.000000 letsbuilda-pypi-2.0.0/src/letsbuilda_pypi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:40:40.792339 letsbuilda-pypi-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-15 00:40:26.000000 letsbuilda-pypi-2.0.0/tests/test_new_packages_feed.py
+drwxr-xr-x   0 bradleyreynolds  (1000) bradleyreynolds  (1000)        0 2023-04-23 03:08:03.468629 letsbuilda-pypi-3.0.0/
+-rw-r--r--   0 bradleyreynolds  (1000) bradleyreynolds  (1000)     1074 2023-01-24 05:19:25.000000 letsbuilda-pypi-3.0.0/LICENSE
+-rw-r--r--   0 bradleyreynolds  (1000) bradleyreynolds  (1000)      588 2023-04-23 03:08:03.468629 letsbuilda-pypi-3.0.0/PKG-INFO
+-rw-r--r--   0 bradleyreynolds  (1000) bradleyreynolds  (1000)      113 2023-03-29 21:38:26.000000 letsbuilda-pypi-3.0.0/README.md
+-rw-r--r--   0 bradleyreynolds  (1000) bradleyreynolds  (1000)     1035 2023-04-23 03:06:30.000000 letsbuilda-pypi-3.0.0/pyproject.toml
+-rw-r--r--   0 bradleyreynolds  (1000) bradleyreynolds  (1000)       38 2023-04-23 03:08:03.468629 letsbuilda-pypi-3.0.0/setup.cfg
+drwxr-xr-x   0 bradleyreynolds  (1000) bradleyreynolds  (1000)        0 2023-04-23 03:08:03.465296 letsbuilda-pypi-3.0.0/src/
+drwxr-xr-x   0 bradleyreynolds  (1000) bradleyreynolds  (1000)        0 2023-04-23 03:08:03.465296 letsbuilda-pypi-3.0.0/src/letsbuilda/
+drwxr-xr-x   0 bradleyreynolds  (1000) bradleyreynolds  (1000)        0 2023-04-23 03:08:03.465296 letsbuilda-pypi-3.0.0/src/letsbuilda/pypi/
+-rw-r--r--   0 bradleyreynolds  (1000) bradleyreynolds  (1000)      246 2023-04-23 03:06:30.000000 letsbuilda-pypi-3.0.0/src/letsbuilda/pypi/__init__.py
+-rw-r--r--   0 bradleyreynolds  (1000) bradleyreynolds  (1000)     1532 2023-04-23 03:06:30.000000 letsbuilda-pypi-3.0.0/src/letsbuilda/pypi/client.py
+-rw-r--r--   0 bradleyreynolds  (1000) bradleyreynolds  (1000)     4044 2023-04-23 03:06:30.000000 letsbuilda-pypi-3.0.0/src/letsbuilda/pypi/models.py
+drwxr-xr-x   0 bradleyreynolds  (1000) bradleyreynolds  (1000)        0 2023-04-23 03:08:03.468629 letsbuilda-pypi-3.0.0/src/letsbuilda_pypi.egg-info/
+-rw-r--r--   0 bradleyreynolds  (1000) bradleyreynolds  (1000)      588 2023-04-23 03:08:03.000000 letsbuilda-pypi-3.0.0/src/letsbuilda_pypi.egg-info/PKG-INFO
+-rw-r--r--   0 bradleyreynolds  (1000) bradleyreynolds  (1000)      370 2023-04-23 03:08:03.000000 letsbuilda-pypi-3.0.0/src/letsbuilda_pypi.egg-info/SOURCES.txt
+-rw-r--r--   0 bradleyreynolds  (1000) bradleyreynolds  (1000)        1 2023-04-23 03:08:03.000000 letsbuilda-pypi-3.0.0/src/letsbuilda_pypi.egg-info/dependency_links.txt
+-rw-r--r--   0 bradleyreynolds  (1000) bradleyreynolds  (1000)      116 2023-04-23 03:08:03.000000 letsbuilda-pypi-3.0.0/src/letsbuilda_pypi.egg-info/requires.txt
+-rw-r--r--   0 bradleyreynolds  (1000) bradleyreynolds  (1000)       11 2023-04-23 03:08:03.000000 letsbuilda-pypi-3.0.0/src/letsbuilda_pypi.egg-info/top_level.txt
+drwxr-xr-x   0 bradleyreynolds  (1000) bradleyreynolds  (1000)        0 2023-04-23 03:08:03.468629 letsbuilda-pypi-3.0.0/tests/
+-rw-r--r--   0 bradleyreynolds  (1000) bradleyreynolds  (1000)     1611 2023-04-23 03:06:30.000000 letsbuilda-pypi-3.0.0/tests/test_new_packages_feed.py
```

### Comparing `letsbuilda-pypi-2.0.0/LICENSE` & `letsbuilda-pypi-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `letsbuilda-pypi-2.0.0/PKG-INFO` & `letsbuilda-pypi-3.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: letsbuilda-pypi
-Version: 2.0.0
+Version: 3.0.0
 Summary: A wrapper for PyPI's API and RSS feed
 Author-email: Bradley Reynolds <bradley.reynolds@darbia.dev>
 License: MIT
 Project-URL: repository, https://github.com/letsbuilda/letsbuilda-pypi/
 Project-URL: documentation, https://docs.letsbuilda.dev/letsbuilda-pypi/
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `letsbuilda-pypi-2.0.0/pyproject.toml` & `letsbuilda-pypi-3.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [project]
 name = "letsbuilda-pypi"
-version = "2.0.0"
+version = "3.0.0"
 description = "A wrapper for PyPI's API and RSS feed"
 authors = [
     { name = "Bradley Reynolds", email = "bradley.reynolds@darbia.dev" },
 ]
 license = { text = "MIT" }
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
     "aiohttp",
     "xmltodict",
+    "pendulum",
 ]
 
 [project.urls]
 repository = "https://github.com/letsbuilda/letsbuilda-pypi/"
 documentation = "https://docs.letsbuilda.dev/letsbuilda-pypi/"
 
 [project.optional-dependencies]
```

### Comparing `letsbuilda-pypi-2.0.0/src/letsbuilda_pypi.egg-info/PKG-INFO` & `letsbuilda-pypi-3.0.0/src/letsbuilda_pypi.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: letsbuilda-pypi
-Version: 2.0.0
+Version: 3.0.0
 Summary: A wrapper for PyPI's API and RSS feed
 Author-email: Bradley Reynolds <bradley.reynolds@darbia.dev>
 License: MIT
 Project-URL: repository, https://github.com/letsbuilda/letsbuilda-pypi/
 Project-URL: documentation, https://docs.letsbuilda.dev/letsbuilda-pypi/
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `letsbuilda-pypi-2.0.0/tests/test_new_packages_feed.py` & `letsbuilda-pypi-3.0.0/tests/test_new_packages_feed.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 """Test parsing metadata from the new packages RSS feed"""
 
 from datetime import datetime
 
-from letsbuilda.pypi import PackageMetadata
+from letsbuilda.pypi import RSSPackageMetadata
 
 
 def test_parse_publication_date() -> None:
     """Confirm publication date gets parsed correctly"""
     data = {
         "title": "test-package added to PyPI",
         "link": "https://pypi.org/project/test-package",
         "guid": "https://pypi.org/project/test-package",
         "description": "a test package",
         "author": "test-author@example.com",
         "pubDate": "Wed, 29 Mar 2023 21:30:05 GMT",
     }
-    parsed_data = PackageMetadata.build_from(data)
+    parsed_data = RSSPackageMetadata.build_from(data)
     assert parsed_data.publication_date == datetime(2023, 3, 29, 21, 30, 5)
 
 
 def test_author_missing() -> None:
     """Confirm missing author gets set to None"""
     data = {
         "title": "test-package added to PyPI",
         "link": "https://pypi.org/project/test-package",
         "guid": "https://pypi.org/project/test-package",
         "description": "a test package",
         "pubDate": "Wed, 29 Mar 2023 21:30:05 GMT",
     }
-    parsed_data = PackageMetadata.build_from(data)
+    parsed_data = RSSPackageMetadata.build_from(data)
     assert parsed_data.author is None
 
 
 def test_description_missing() -> None:
     """Confirm missing description gets set to None"""
     data = {
         "title": "test-package added to PyPI",
         "link": "https://pypi.org/project/test-package",
         "guid": "https://pypi.org/project/test-package",
         "author": "test-author@example.com",
         "pubDate": "Wed, 29 Mar 2023 21:30:05 GMT",
     }
-    parsed_data = PackageMetadata.build_from(data)
+    parsed_data = RSSPackageMetadata.build_from(data)
     assert parsed_data.description is None
```

