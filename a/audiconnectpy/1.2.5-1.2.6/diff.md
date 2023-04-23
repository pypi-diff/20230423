# Comparing `tmp/audiconnectpy-1.2.5.tar.gz` & `tmp/audiconnectpy-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiconnectpy-1.2.5.tar", last modified: Sun Apr 23 17:01:17 2023, max compression
+gzip compressed data, was "audiconnectpy-1.2.6.tar", last modified: Sun Apr 23 17:33:41 2023, max compression
```

## Comparing `audiconnectpy-1.2.5.tar` & `audiconnectpy-1.2.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:01:17.586630 audiconnectpy-1.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-23 17:01:07.000000 audiconnectpy-1.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-23 17:01:07.000000 audiconnectpy-1.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-04-23 17:01:17.582630 audiconnectpy-1.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-04-23 17:01:07.000000 audiconnectpy-1.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:01:17.582630 audiconnectpy-1.2.5/audiconnectpy/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-23 17:01:07.000000 audiconnectpy-1.2.5/audiconnectpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-23 17:01:07.000000 audiconnectpy-1.2.5/audiconnectpy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    22276 2023-04-23 17:01:07.000000 audiconnectpy-1.2.5/audiconnectpy/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-23 17:01:07.000000 audiconnectpy-1.2.5/audiconnectpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    29822 2023-04-23 17:01:07.000000 audiconnectpy-1.2.5/audiconnectpy/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    30327 2023-04-23 17:01:07.000000 audiconnectpy-1.2.5/audiconnectpy/services.py
--rw-r--r--   0 runner    (1001) docker     (123)    19479 2023-04-23 17:01:07.000000 audiconnectpy-1.2.5/audiconnectpy/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:01:17.582630 audiconnectpy-1.2.5/audiconnectpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-04-23 17:01:17.000000 audiconnectpy-1.2.5/audiconnectpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-23 17:01:17.000000 audiconnectpy-1.2.5/audiconnectpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 17:01:17.000000 audiconnectpy-1.2.5/audiconnectpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 17:01:17.000000 audiconnectpy-1.2.5/audiconnectpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-23 17:01:17.000000 audiconnectpy-1.2.5/audiconnectpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-23 17:01:07.000000 audiconnectpy-1.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 17:01:17.586630 audiconnectpy-1.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-23 17:01:16.000000 audiconnectpy-1.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:01:17.582630 audiconnectpy-1.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-23 17:01:07.000000 audiconnectpy-1.2.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:33:41.453297 audiconnectpy-1.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-23 17:33:30.000000 audiconnectpy-1.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-23 17:33:30.000000 audiconnectpy-1.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-04-23 17:33:41.453297 audiconnectpy-1.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-04-23 17:33:30.000000 audiconnectpy-1.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:33:41.453297 audiconnectpy-1.2.6/audiconnectpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-23 17:33:30.000000 audiconnectpy-1.2.6/audiconnectpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-23 17:33:30.000000 audiconnectpy-1.2.6/audiconnectpy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22276 2023-04-23 17:33:30.000000 audiconnectpy-1.2.6/audiconnectpy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-23 17:33:30.000000 audiconnectpy-1.2.6/audiconnectpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29813 2023-04-23 17:33:30.000000 audiconnectpy-1.2.6/audiconnectpy/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30327 2023-04-23 17:33:30.000000 audiconnectpy-1.2.6/audiconnectpy/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19481 2023-04-23 17:33:30.000000 audiconnectpy-1.2.6/audiconnectpy/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:33:41.453297 audiconnectpy-1.2.6/audiconnectpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-04-23 17:33:41.000000 audiconnectpy-1.2.6/audiconnectpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-23 17:33:41.000000 audiconnectpy-1.2.6/audiconnectpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 17:33:41.000000 audiconnectpy-1.2.6/audiconnectpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 17:33:41.000000 audiconnectpy-1.2.6/audiconnectpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-23 17:33:41.000000 audiconnectpy-1.2.6/audiconnectpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-23 17:33:30.000000 audiconnectpy-1.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 17:33:41.453297 audiconnectpy-1.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-23 17:33:40.000000 audiconnectpy-1.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:33:41.453297 audiconnectpy-1.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-23 17:33:30.000000 audiconnectpy-1.2.6/tests/__init__.py
```

### Comparing `audiconnectpy-1.2.5/LICENSE` & `audiconnectpy-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.2.5/PKG-INFO` & `audiconnectpy-1.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 1.2.5
+Version: 1.2.6
 Summary: Provides asynchronous authentication and access to Audi Connect
 Home-page: https://github.com/cyr-ius/audiconnectpy/tree/master/audiconnectpy
 Author: cyr-ius
 Author-email: cyr-ius@ipocus.net
 License: GPL-3
 Keywords: connect,async
 Classifier: Programming Language :: Python
```

### Comparing `audiconnectpy-1.2.5/README.md` & `audiconnectpy-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.2.5/audiconnectpy/api.py` & `audiconnectpy-1.2.6/audiconnectpy/api.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.2.5/audiconnectpy/auth.py` & `audiconnectpy-1.2.6/audiconnectpy/auth.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.2.5/audiconnectpy/models.py` & `audiconnectpy-1.2.6/audiconnectpy/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -446,15 +446,15 @@
 @dataclass
 class DestinationDataResponse:
     """Destination."""
 
     data: dict[str, Any]
 
     @property
-    def destination_supported(self) -> bool:
+    def is_supported(self) -> bool:
         """Supported status."""
         return self.attributes is not None
 
     @property
     def attributes(self) -> dict[Any, dict[str, Any]]:
         """Attributes properties."""
         _attributes = {}
```

### Comparing `audiconnectpy-1.2.5/audiconnectpy/services.py` & `audiconnectpy-1.2.6/audiconnectpy/services.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.2.5/audiconnectpy/util.py` & `audiconnectpy-1.2.6/audiconnectpy/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -414,15 +414,15 @@
         icon="mdi:air-conditioner",
         sensor_type="switch",
         turn_mode="async_climater",
     )
     CLIMATISATION_TARGET_TEMP = FieldType(
         attr="climatisation_target_temperature",
         icon="mdi:temperature-celsius",
-        sensor_type="text",
+        sensor_type="number",
         unit_of_measurement="°C",
         evaluation=lambda x: round((int(x) - 2731) / 10, 1),
         device_class="temperature",
         turn_mode="async_climater_temp",
         options=[7, 40],
     )
     CLIMATISATION_HEATER_SRC = FieldType(
```

### Comparing `audiconnectpy-1.2.5/audiconnectpy.egg-info/PKG-INFO` & `audiconnectpy-1.2.6/audiconnectpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 1.2.5
+Version: 1.2.6
 Summary: Provides asynchronous authentication and access to Audi Connect
 Home-page: https://github.com/cyr-ius/audiconnectpy/tree/master/audiconnectpy
 Author: cyr-ius
 Author-email: cyr-ius@ipocus.net
 License: GPL-3
 Keywords: connect,async
 Classifier: Programming Language :: Python
```

### Comparing `audiconnectpy-1.2.5/pyproject.toml` & `audiconnectpy-1.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.2.5/setup.py` & `audiconnectpy-1.2.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Get the long description from the README file
 with open(os.path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name="audiconnectpy",
-    version="1.2.5",
+    version="1.2.6",
     packages=find_packages(),
     author="cyr-ius",
     author_email="cyr-ius@ipocus.net",
     description="Provides asynchronous authentication and access to Audi Connect",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=["aiohttp>=3.8.1", "beautifulsoup4>=4.11.2"],
```

