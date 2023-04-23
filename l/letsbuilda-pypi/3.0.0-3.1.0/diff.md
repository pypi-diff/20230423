# Comparing `tmp/letsbuilda-pypi-3.0.0.tar.gz` & `tmp/letsbuilda-pypi-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "letsbuilda-pypi-3.0.0.tar", last modified: Sun Apr 23 03:08:03 2023, max compression
+gzip compressed data, was "letsbuilda-pypi-3.1.0.tar", last modified: Sun Apr 23 07:45:28 2023, max compression
```

## Comparing `letsbuilda-pypi-3.0.0.tar` & `letsbuilda-pypi-3.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 bradleyreynolds  (1000) bradleyreynolds  (1000)        0 2023-04-23 03:08:03.468629 letsbuilda-pypi-3.0.0/
--rw-r--r--   0 bradleyreynolds  (1000) bradleyreynolds  (1000)     1074 2023-01-24 05:19:25.000000 letsbuilda-pypi-3.0.0/LICENSE
--rw-r--r--   0 bradleyreynolds  (1000) bradleyreynolds  (1000)      588 2023-04-23 03:08:03.468629 letsbuilda-pypi-3.0.0/PKG-INFO
--rw-r--r--   0 bradleyreynolds  (1000) bradleyreynolds  (1000)      113 2023-03-29 21:38:26.000000 letsbuilda-pypi-3.0.0/README.md
--rw-r--r--   0 bradleyreynolds  (1000) bradleyreynolds  (1000)     1035 2023-04-23 03:06:30.000000 letsbuilda-pypi-3.0.0/pyproject.toml
--rw-r--r--   0 bradleyreynolds  (1000) bradleyreynolds  (1000)       38 2023-04-23 03:08:03.468629 letsbuilda-pypi-3.0.0/setup.cfg
-drwxr-xr-x   0 bradleyreynolds  (1000) bradleyreynolds  (1000)        0 2023-04-23 03:08:03.465296 letsbuilda-pypi-3.0.0/src/
-drwxr-xr-x   0 bradleyreynolds  (1000) bradleyreynolds  (1000)        0 2023-04-23 03:08:03.465296 letsbuilda-pypi-3.0.0/src/letsbuilda/
-drwxr-xr-x   0 bradleyreynolds  (1000) bradleyreynolds  (1000)        0 2023-04-23 03:08:03.465296 letsbuilda-pypi-3.0.0/src/letsbuilda/pypi/
--rw-r--r--   0 bradleyreynolds  (1000) bradleyreynolds  (1000)      246 2023-04-23 03:06:30.000000 letsbuilda-pypi-3.0.0/src/letsbuilda/pypi/__init__.py
--rw-r--r--   0 bradleyreynolds  (1000) bradleyreynolds  (1000)     1532 2023-04-23 03:06:30.000000 letsbuilda-pypi-3.0.0/src/letsbuilda/pypi/client.py
--rw-r--r--   0 bradleyreynolds  (1000) bradleyreynolds  (1000)     4044 2023-04-23 03:06:30.000000 letsbuilda-pypi-3.0.0/src/letsbuilda/pypi/models.py
-drwxr-xr-x   0 bradleyreynolds  (1000) bradleyreynolds  (1000)        0 2023-04-23 03:08:03.468629 letsbuilda-pypi-3.0.0/src/letsbuilda_pypi.egg-info/
--rw-r--r--   0 bradleyreynolds  (1000) bradleyreynolds  (1000)      588 2023-04-23 03:08:03.000000 letsbuilda-pypi-3.0.0/src/letsbuilda_pypi.egg-info/PKG-INFO
--rw-r--r--   0 bradleyreynolds  (1000) bradleyreynolds  (1000)      370 2023-04-23 03:08:03.000000 letsbuilda-pypi-3.0.0/src/letsbuilda_pypi.egg-info/SOURCES.txt
--rw-r--r--   0 bradleyreynolds  (1000) bradleyreynolds  (1000)        1 2023-04-23 03:08:03.000000 letsbuilda-pypi-3.0.0/src/letsbuilda_pypi.egg-info/dependency_links.txt
--rw-r--r--   0 bradleyreynolds  (1000) bradleyreynolds  (1000)      116 2023-04-23 03:08:03.000000 letsbuilda-pypi-3.0.0/src/letsbuilda_pypi.egg-info/requires.txt
--rw-r--r--   0 bradleyreynolds  (1000) bradleyreynolds  (1000)       11 2023-04-23 03:08:03.000000 letsbuilda-pypi-3.0.0/src/letsbuilda_pypi.egg-info/top_level.txt
-drwxr-xr-x   0 bradleyreynolds  (1000) bradleyreynolds  (1000)        0 2023-04-23 03:08:03.468629 letsbuilda-pypi-3.0.0/tests/
--rw-r--r--   0 bradleyreynolds  (1000) bradleyreynolds  (1000)     1611 2023-04-23 03:06:30.000000 letsbuilda-pypi-3.0.0/tests/test_new_packages_feed.py
+drwxr-xr-x   0 bradleyreynolds  (1000) bradleyreynolds  (1000)        0 2023-04-23 07:45:28.951648 letsbuilda-pypi-3.1.0/
+-rw-r--r--   0 bradleyreynolds  (1000) bradleyreynolds  (1000)     1074 2023-01-24 05:19:25.000000 letsbuilda-pypi-3.1.0/LICENSE
+-rw-r--r--   0 bradleyreynolds  (1000) bradleyreynolds  (1000)      588 2023-04-23 07:45:28.948314 letsbuilda-pypi-3.1.0/PKG-INFO
+-rw-r--r--   0 bradleyreynolds  (1000) bradleyreynolds  (1000)      113 2023-03-29 21:38:26.000000 letsbuilda-pypi-3.1.0/README.md
+-rw-r--r--   0 bradleyreynolds  (1000) bradleyreynolds  (1000)     1035 2023-04-23 07:44:53.000000 letsbuilda-pypi-3.1.0/pyproject.toml
+-rw-r--r--   0 bradleyreynolds  (1000) bradleyreynolds  (1000)       38 2023-04-23 07:45:28.951648 letsbuilda-pypi-3.1.0/setup.cfg
+drwxr-xr-x   0 bradleyreynolds  (1000) bradleyreynolds  (1000)        0 2023-04-23 07:45:28.948314 letsbuilda-pypi-3.1.0/src/
+drwxr-xr-x   0 bradleyreynolds  (1000) bradleyreynolds  (1000)        0 2023-04-23 07:45:28.948314 letsbuilda-pypi-3.1.0/src/letsbuilda/
+drwxr-xr-x   0 bradleyreynolds  (1000) bradleyreynolds  (1000)        0 2023-04-23 07:45:28.948314 letsbuilda-pypi-3.1.0/src/letsbuilda/pypi/
+-rw-r--r--   0 bradleyreynolds  (1000) bradleyreynolds  (1000)      246 2023-04-23 03:06:30.000000 letsbuilda-pypi-3.1.0/src/letsbuilda/pypi/__init__.py
+-rw-r--r--   0 bradleyreynolds  (1000) bradleyreynolds  (1000)     1532 2023-04-23 03:06:30.000000 letsbuilda-pypi-3.1.0/src/letsbuilda/pypi/client.py
+-rw-r--r--   0 bradleyreynolds  (1000) bradleyreynolds  (1000)     4335 2023-04-23 07:44:53.000000 letsbuilda-pypi-3.1.0/src/letsbuilda/pypi/models.py
+drwxr-xr-x   0 bradleyreynolds  (1000) bradleyreynolds  (1000)        0 2023-04-23 07:45:28.948314 letsbuilda-pypi-3.1.0/src/letsbuilda_pypi.egg-info/
+-rw-r--r--   0 bradleyreynolds  (1000) bradleyreynolds  (1000)      588 2023-04-23 07:45:28.000000 letsbuilda-pypi-3.1.0/src/letsbuilda_pypi.egg-info/PKG-INFO
+-rw-r--r--   0 bradleyreynolds  (1000) bradleyreynolds  (1000)      370 2023-04-23 07:45:28.000000 letsbuilda-pypi-3.1.0/src/letsbuilda_pypi.egg-info/SOURCES.txt
+-rw-r--r--   0 bradleyreynolds  (1000) bradleyreynolds  (1000)        1 2023-04-23 07:45:28.000000 letsbuilda-pypi-3.1.0/src/letsbuilda_pypi.egg-info/dependency_links.txt
+-rw-r--r--   0 bradleyreynolds  (1000) bradleyreynolds  (1000)      116 2023-04-23 07:45:28.000000 letsbuilda-pypi-3.1.0/src/letsbuilda_pypi.egg-info/requires.txt
+-rw-r--r--   0 bradleyreynolds  (1000) bradleyreynolds  (1000)       11 2023-04-23 07:45:28.000000 letsbuilda-pypi-3.1.0/src/letsbuilda_pypi.egg-info/top_level.txt
+drwxr-xr-x   0 bradleyreynolds  (1000) bradleyreynolds  (1000)        0 2023-04-23 07:45:28.948314 letsbuilda-pypi-3.1.0/tests/
+-rw-r--r--   0 bradleyreynolds  (1000) bradleyreynolds  (1000)     1611 2023-04-23 03:06:30.000000 letsbuilda-pypi-3.1.0/tests/test_new_packages_feed.py
```

### Comparing `letsbuilda-pypi-3.0.0/LICENSE` & `letsbuilda-pypi-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `letsbuilda-pypi-3.0.0/PKG-INFO` & `letsbuilda-pypi-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: letsbuilda-pypi
-Version: 3.0.0
+Version: 3.1.0
 Summary: A wrapper for PyPI's API and RSS feed
 Author-email: Bradley Reynolds <bradley.reynolds@darbia.dev>
 License: MIT
 Project-URL: repository, https://github.com/letsbuilda/letsbuilda-pypi/
 Project-URL: documentation, https://docs.letsbuilda.dev/letsbuilda-pypi/
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `letsbuilda-pypi-3.0.0/pyproject.toml` & `letsbuilda-pypi-3.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "letsbuilda-pypi"
-version = "3.0.0"
+version = "3.1.0"
 description = "A wrapper for PyPI's API and RSS feed"
 authors = [
     { name = "Bradley Reynolds", email = "bradley.reynolds@darbia.dev" },
 ]
 license = { text = "MIT" }
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `letsbuilda-pypi-3.0.0/src/letsbuilda/pypi/client.py` & `letsbuilda-pypi-3.1.0/src/letsbuilda/pypi/client.py`

 * *Files identical despite different names*

### Comparing `letsbuilda-pypi-3.0.0/src/letsbuilda/pypi/models.py` & `letsbuilda-pypi-3.1.0/src/letsbuilda/pypi/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,21 +71,28 @@
     packagetype: str
     python_version: str
     requires_python: str | None
     size: int
     upload_time: DateTime
     upload_time_iso_8601: DateTime
     url: str
+    inspector_url: str
     yanked: bool
     yanked_reason: None
 
     @classmethod
-    def from_dict(cls, data: dict) -> "URL":
+    def from_dict(cls, data: dict, package_name: str, package_version: str) -> "URL":
         data["upload_time"]: DateTime = pendulum.parse(data["upload_time"])
         data["upload_time_iso_8601"]: DateTime = pendulum.parse(data["upload_time_iso_8601"])
+
+        data["inspector_url"] = data["url"].replace(
+            "https://files.pythonhosted.org/",
+            f"https://inspector.pypi.io/project/{package_name}/{package_version}/",
+        )
+
         return cls(**data)
 
 
 @dataclass(frozen=True, slots=True)
 class Info:
     """Package metadata internal info block"""
 
@@ -131,15 +138,15 @@
     vulnerabilities: list["Vulnerability"]
 
     @classmethod
     def from_dict(cls, data: dict) -> "PackageMetadata":
         return cls(
             info=Info.from_dict(data["info"]),
             last_serial=data["last_serial"],
-            urls=[URL.from_dict(url_data) for url_data in data["urls"]],
+            urls=[URL.from_dict(url_data, data["name"], data["version"]) for url_data in data["urls"]],
             vulnerabilities=[Vulnerability.from_dict(vuln_data) for vuln_data in data["vulnerabilities"]],
         )
 
 
 @dataclass(frozen=True, slots=True)
 class RSSPackageMetadata:
     """RSS Package metadata"""
```

### Comparing `letsbuilda-pypi-3.0.0/src/letsbuilda_pypi.egg-info/PKG-INFO` & `letsbuilda-pypi-3.1.0/src/letsbuilda_pypi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: letsbuilda-pypi
-Version: 3.0.0
+Version: 3.1.0
 Summary: A wrapper for PyPI's API and RSS feed
 Author-email: Bradley Reynolds <bradley.reynolds@darbia.dev>
 License: MIT
 Project-URL: repository, https://github.com/letsbuilda/letsbuilda-pypi/
 Project-URL: documentation, https://docs.letsbuilda.dev/letsbuilda-pypi/
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `letsbuilda-pypi-3.0.0/tests/test_new_packages_feed.py` & `letsbuilda-pypi-3.1.0/tests/test_new_packages_feed.py`

 * *Files identical despite different names*

