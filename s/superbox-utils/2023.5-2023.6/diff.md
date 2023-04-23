# Comparing `tmp/superbox-utils-2023.5.tar.gz` & `tmp/superbox-utils-2023.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superbox-utils-2023.5.tar", last modified: Sun Mar 26 05:42:38 2023, max compression
+gzip compressed data, was "superbox-utils-2023.6.tar", last modified: Sun Apr 23 10:39:27 2023, max compression
```

## Comparing `superbox-utils-2023.5.tar` & `superbox-utils-2023.6.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 05:42:38.030403 superbox-utils-2023.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-26 05:42:27.000000 superbox-utils-2023.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-26 05:42:27.000000 superbox-utils-2023.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-03-26 05:42:38.030403 superbox-utils-2023.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-03-26 05:42:27.000000 superbox-utils-2023.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-03-26 05:42:27.000000 superbox-utils-2023.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-03-26 05:42:27.000000 superbox-utils-2023.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-03-26 05:42:38.030403 superbox-utils-2023.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-03-26 05:42:27.000000 superbox-utils-2023.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 05:42:38.022403 superbox-utils-2023.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 05:42:38.026403 superbox-utils-2023.5/src/superbox_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-26 05:42:27.000000 superbox-utils-2023.5/src/superbox_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 05:42:38.026403 superbox-utils-2023.5/src/superbox_utils/argparse/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-26 05:42:27.000000 superbox-utils-2023.5/src/superbox_utils/argparse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-03-26 05:42:27.000000 superbox-utils-2023.5/src/superbox_utils/argparse/argparse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 05:42:38.026403 superbox-utils-2023.5/src/superbox_utils/asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-26 05:42:27.000000 superbox-utils-2023.5/src/superbox_utils/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-26 05:42:27.000000 superbox-utils-2023.5/src/superbox_utils/asyncio/asyncio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 05:42:38.026403 superbox-utils-2023.5/src/superbox_utils/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 05:42:27.000000 superbox-utils-2023.5/src/superbox_utils/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-26 05:42:27.000000 superbox-utils-2023.5/src/superbox_utils/config/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-03-26 05:42:27.000000 superbox-utils-2023.5/src/superbox_utils/config/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 05:42:38.026403 superbox-utils-2023.5/src/superbox_utils/core/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-26 05:42:27.000000 superbox-utils-2023.5/src/superbox_utils/core/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 05:42:38.030403 superbox-utils-2023.5/src/superbox_utils/dict/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 05:42:27.000000 superbox-utils-2023.5/src/superbox_utils/dict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-03-26 05:42:27.000000 superbox-utils-2023.5/src/superbox_utils/dict/data_dict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 05:42:38.030403 superbox-utils-2023.5/src/superbox_utils/hass/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 05:42:27.000000 superbox-utils-2023.5/src/superbox_utils/hass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-03-26 05:42:27.000000 superbox-utils-2023.5/src/superbox_utils/hass/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 05:42:38.030403 superbox-utils-2023.5/src/superbox_utils/logging/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-26 05:42:27.000000 superbox-utils-2023.5/src/superbox_utils/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-03-26 05:42:27.000000 superbox-utils-2023.5/src/superbox_utils/logging/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-03-26 05:42:27.000000 superbox-utils-2023.5/src/superbox_utils/logging/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-03-26 05:42:27.000000 superbox-utils-2023.5/src/superbox_utils/logging/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 05:42:38.030403 superbox-utils-2023.5/src/superbox_utils/mqtt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 05:42:27.000000 superbox-utils-2023.5/src/superbox_utils/mqtt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-26 05:42:27.000000 superbox-utils-2023.5/src/superbox_utils/mqtt/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-03-26 05:42:27.000000 superbox-utils-2023.5/src/superbox_utils/mqtt/connect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 05:42:38.030403 superbox-utils-2023.5/src/superbox_utils/text/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 05:42:27.000000 superbox-utils-2023.5/src/superbox_utils/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-03-26 05:42:27.000000 superbox-utils-2023.5/src/superbox_utils/text/text.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-26 05:42:27.000000 superbox-utils-2023.5/src/superbox_utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 05:42:38.030403 superbox-utils-2023.5/src/superbox_utils/yaml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 05:42:27.000000 superbox-utils-2023.5/src/superbox_utils/yaml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-03-26 05:42:27.000000 superbox-utils-2023.5/src/superbox_utils/yaml/dumper.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-03-26 05:42:27.000000 superbox-utils-2023.5/src/superbox_utils/yaml/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 05:42:38.026403 superbox-utils-2023.5/src/superbox_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-03-26 05:42:38.000000 superbox-utils-2023.5/src/superbox_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-03-26 05:42:38.000000 superbox-utils-2023.5/src/superbox_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 05:42:38.000000 superbox-utils-2023.5/src/superbox_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-26 05:42:38.000000 superbox-utils-2023.5/src/superbox_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-26 05:42:38.000000 superbox-utils-2023.5/src/superbox_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 10:39:27.614685 superbox-utils-2023.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-23 10:39:11.000000 superbox-utils-2023.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-23 10:39:11.000000 superbox-utils-2023.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-23 10:39:27.614685 superbox-utils-2023.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-23 10:39:11.000000 superbox-utils-2023.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-04-23 10:39:11.000000 superbox-utils-2023.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-23 10:39:11.000000 superbox-utils-2023.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-23 10:39:27.614685 superbox-utils-2023.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-23 10:39:11.000000 superbox-utils-2023.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 10:39:27.606685 superbox-utils-2023.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 10:39:27.610685 superbox-utils-2023.6/src/superbox_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-23 10:39:11.000000 superbox-utils-2023.6/src/superbox_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 10:39:27.610685 superbox-utils-2023.6/src/superbox_utils/argparse/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-23 10:39:11.000000 superbox-utils-2023.6/src/superbox_utils/argparse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-23 10:39:11.000000 superbox-utils-2023.6/src/superbox_utils/argparse/argparse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 10:39:27.614685 superbox-utils-2023.6/src/superbox_utils/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-23 10:39:11.000000 superbox-utils-2023.6/src/superbox_utils/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-23 10:39:11.000000 superbox-utils-2023.6/src/superbox_utils/asyncio/asyncio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 10:39:27.614685 superbox-utils-2023.6/src/superbox_utils/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 10:39:11.000000 superbox-utils-2023.6/src/superbox_utils/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-23 10:39:11.000000 superbox-utils-2023.6/src/superbox_utils/config/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-23 10:39:11.000000 superbox-utils-2023.6/src/superbox_utils/config/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 10:39:27.614685 superbox-utils-2023.6/src/superbox_utils/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-23 10:39:11.000000 superbox-utils-2023.6/src/superbox_utils/core/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 10:39:27.614685 superbox-utils-2023.6/src/superbox_utils/dict/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 10:39:11.000000 superbox-utils-2023.6/src/superbox_utils/dict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-23 10:39:11.000000 superbox-utils-2023.6/src/superbox_utils/dict/data_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 10:39:27.614685 superbox-utils-2023.6/src/superbox_utils/hass/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 10:39:11.000000 superbox-utils-2023.6/src/superbox_utils/hass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-23 10:39:11.000000 superbox-utils-2023.6/src/superbox_utils/hass/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 10:39:27.614685 superbox-utils-2023.6/src/superbox_utils/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-23 10:39:11.000000 superbox-utils-2023.6/src/superbox_utils/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-04-23 10:39:11.000000 superbox-utils-2023.6/src/superbox_utils/logging/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-23 10:39:11.000000 superbox-utils-2023.6/src/superbox_utils/logging/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-23 10:39:11.000000 superbox-utils-2023.6/src/superbox_utils/logging/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 10:39:27.614685 superbox-utils-2023.6/src/superbox_utils/mqtt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 10:39:11.000000 superbox-utils-2023.6/src/superbox_utils/mqtt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-23 10:39:11.000000 superbox-utils-2023.6/src/superbox_utils/mqtt/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-04-23 10:39:11.000000 superbox-utils-2023.6/src/superbox_utils/mqtt/connect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 10:39:27.614685 superbox-utils-2023.6/src/superbox_utils/text/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 10:39:11.000000 superbox-utils-2023.6/src/superbox_utils/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-23 10:39:11.000000 superbox-utils-2023.6/src/superbox_utils/text/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-23 10:39:11.000000 superbox-utils-2023.6/src/superbox_utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 10:39:27.614685 superbox-utils-2023.6/src/superbox_utils/yaml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 10:39:11.000000 superbox-utils-2023.6/src/superbox_utils/yaml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-23 10:39:11.000000 superbox-utils-2023.6/src/superbox_utils/yaml/dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-23 10:39:11.000000 superbox-utils-2023.6/src/superbox_utils/yaml/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 10:39:27.610685 superbox-utils-2023.6/src/superbox_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-23 10:39:27.000000 superbox-utils-2023.6/src/superbox_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-23 10:39:27.000000 superbox-utils-2023.6/src/superbox_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 10:39:27.000000 superbox-utils-2023.6/src/superbox_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-23 10:39:27.000000 superbox-utils-2023.6/src/superbox_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-23 10:39:27.000000 superbox-utils-2023.6/src/superbox_utils.egg-info/top_level.txt
```

### Comparing `superbox-utils-2023.5/LICENSE` & `superbox-utils-2023.6/LICENSE`

 * *Files identical despite different names*

### Comparing `superbox-utils-2023.5/pyproject.toml` & `superbox-utils-2023.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ignore_missing_imports = true
 
 [tool.pylint.master]
 # C0114: missing-module-docstring
 # C0115: missing-class-docstring
 # C0116: missing-function-docstring
 # C0301: line-too-long
-# C0411: rong-import-order
+# C0411: wrong-import-order
 # E0401: import-error
 # R0801: duplicate-code
 # R1732: consider-using-with
 # R6003: consider-alternative-union-syntax (python 3.8 compatibility)
 # W6001: deprecated-typing-alias (python 3.8 compatibility)
 disable = ["C0114", "C0115", "C0116", "C0301", "C0411", "E0401", "R0801", "R1732", "R6003", "W6001"]
 notes = ["FIXME"]
```

### Comparing `superbox-utils-2023.5/setup.cfg` & `superbox-utils-2023.6/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -3,26 +3,28 @@
 
 [metadata]
 name = superbox-utils
 version = attr: superbox_utils.__version__
 description = Utilities for Superbox Python Packages.
 long_description = file: README.md
 long_description_content_type = text/markdown
-url = https://github.com/mh-superbox/superbox-utils
+url = https://github.com/superbox-dev/superbox-utils
 author = Michael Hacker
 author_email = mh@superbox.one
+license = Apache-2.0 license
 license_files = 
 	LICENSE
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3 :: Only
 	Operating System :: POSIX :: Linux
 	Topic :: Utilities
 project_urls = 
 	Source Code = https://github.com/superbox-dev/superbox-utils
 	Bug Reports = https://github.com/superbox-dev/superbox-utils/issues
```

### Comparing `superbox-utils-2023.5/setup.py` & `superbox-utils-2023.6/setup.py`

 * *Files identical despite different names*

### Comparing `superbox-utils-2023.5/src/superbox_utils/argparse/argparse.py` & `superbox-utils-2023.6/src/superbox_utils/argparse/argparse.py`

 * *Files identical despite different names*

### Comparing `superbox-utils-2023.5/src/superbox_utils/config/loader.py` & `superbox-utils-2023.6/src/superbox_utils/config/loader.py`

 * *Files identical despite different names*

### Comparing `superbox-utils-2023.5/src/superbox_utils/dict/data_dict.py` & `superbox-utils-2023.6/src/superbox_utils/dict/data_dict.py`

 * *Files identical despite different names*

### Comparing `superbox-utils-2023.5/src/superbox_utils/hass/config.py` & `superbox-utils-2023.6/src/superbox_utils/hass/config.py`

 * *Files identical despite different names*

### Comparing `superbox-utils-2023.5/src/superbox_utils/logging/config.py` & `superbox-utils-2023.6/src/superbox_utils/logging/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,22 +20,24 @@
     level: str = field(default="error")
 
     @property
     def verbose(self) -> int:
         """Get logging verbose level as integer."""
         return list(LOG_LEVEL).index(self.level)
 
-    def init(self, log: Optional[str], log_path: Path, name: Optional[str] = None, verbose: int = 0) -> None:
+    def init(
+        self, log: Optional[str], log_path: Optional[Path] = None, name: Optional[str] = None, verbose: int = 0
+    ) -> None:
         """Initialize logger handler and formatter.
 
         Parameters
         ----------
         log: str
             set log handler to systemd, stdout or file.
-        log_path: Path
+        log_path: Path, optional
             custom log path.
         name: str, optional
             The logger name.
         verbose: int
             Logging verbose level as integer.
         """
         logger: logging.Logger = logging.getLogger(name)
@@ -45,15 +47,15 @@
             systemd_handler = handler.SystemdHandler()
             systemd_handler.setFormatter(logging.Formatter(SYSTEMD_LOG_FORMAT))
             logger.addHandler(systemd_handler)
         elif log == "stdout":
             stdout_handler: logging.Handler = logging.StreamHandler()
             stdout_handler.setFormatter(logging.Formatter(STDOUT_LOG_FORMAT))
             logger.addHandler(stdout_handler)
-        elif log == "file":
+        elif log == "file" and log_path:
             log_path.mkdir(exist_ok=True, parents=True)
 
             file_handler = logging.FileHandler(log_path / f"{name}.log")
             file_handler.setFormatter(logging.Formatter(FILE_LOG_FORMAT, datefmt="%Y-%m-%d %H:%M:%S"))
             logger.addHandler(file_handler)
         else:
             default_handler: logging.Handler = logging.StreamHandler()
```

### Comparing `superbox-utils-2023.5/src/superbox_utils/logging/handler.py` & `superbox-utils-2023.6/src/superbox_utils/logging/handler.py`

 * *Files identical despite different names*

### Comparing `superbox-utils-2023.5/src/superbox_utils/mqtt/connect.py` & `superbox-utils-2023.6/src/superbox_utils/mqtt/connect.py`

 * *Files identical despite different names*

### Comparing `superbox-utils-2023.5/src/superbox_utils/text/text.py` & `superbox-utils-2023.6/src/superbox_utils/text/text.py`

 * *Files identical despite different names*

### Comparing `superbox-utils-2023.5/src/superbox_utils/yaml/dumper.py` & `superbox-utils-2023.6/src/superbox_utils/yaml/dumper.py`

 * *Files identical despite different names*

### Comparing `superbox-utils-2023.5/src/superbox_utils/yaml/loader.py` & `superbox-utils-2023.6/src/superbox_utils/yaml/loader.py`

 * *Files identical despite different names*

### Comparing `superbox-utils-2023.5/src/superbox_utils.egg-info/SOURCES.txt` & `superbox-utils-2023.6/src/superbox_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

