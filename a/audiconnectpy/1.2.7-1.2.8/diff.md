# Comparing `tmp/audiconnectpy-1.2.7.tar.gz` & `tmp/audiconnectpy-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiconnectpy-1.2.7.tar", last modified: Sun Apr 23 17:44:42 2023, max compression
+gzip compressed data, was "audiconnectpy-1.2.8.tar", last modified: Sun Apr 23 17:47:31 2023, max compression
```

## Comparing `audiconnectpy-1.2.7.tar` & `audiconnectpy-1.2.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:44:42.634061 audiconnectpy-1.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-23 17:44:31.000000 audiconnectpy-1.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-23 17:44:31.000000 audiconnectpy-1.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-04-23 17:44:42.634061 audiconnectpy-1.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-04-23 17:44:31.000000 audiconnectpy-1.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:44:42.630061 audiconnectpy-1.2.7/audiconnectpy/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-23 17:44:31.000000 audiconnectpy-1.2.7/audiconnectpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-23 17:44:31.000000 audiconnectpy-1.2.7/audiconnectpy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    22276 2023-04-23 17:44:31.000000 audiconnectpy-1.2.7/audiconnectpy/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-23 17:44:31.000000 audiconnectpy-1.2.7/audiconnectpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    29813 2023-04-23 17:44:31.000000 audiconnectpy-1.2.7/audiconnectpy/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    30341 2023-04-23 17:44:31.000000 audiconnectpy-1.2.7/audiconnectpy/services.py
--rw-r--r--   0 runner    (1001) docker     (123)    19524 2023-04-23 17:44:31.000000 audiconnectpy-1.2.7/audiconnectpy/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:44:42.630061 audiconnectpy-1.2.7/audiconnectpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-04-23 17:44:42.000000 audiconnectpy-1.2.7/audiconnectpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-23 17:44:42.000000 audiconnectpy-1.2.7/audiconnectpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 17:44:42.000000 audiconnectpy-1.2.7/audiconnectpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 17:44:42.000000 audiconnectpy-1.2.7/audiconnectpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-23 17:44:42.000000 audiconnectpy-1.2.7/audiconnectpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-23 17:44:31.000000 audiconnectpy-1.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 17:44:42.634061 audiconnectpy-1.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-23 17:44:40.000000 audiconnectpy-1.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:44:42.630061 audiconnectpy-1.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-23 17:44:31.000000 audiconnectpy-1.2.7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:47:31.480315 audiconnectpy-1.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-23 17:47:19.000000 audiconnectpy-1.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-23 17:47:19.000000 audiconnectpy-1.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-04-23 17:47:31.480315 audiconnectpy-1.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-04-23 17:47:19.000000 audiconnectpy-1.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:47:31.476315 audiconnectpy-1.2.8/audiconnectpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-23 17:47:19.000000 audiconnectpy-1.2.8/audiconnectpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-23 17:47:19.000000 audiconnectpy-1.2.8/audiconnectpy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22276 2023-04-23 17:47:19.000000 audiconnectpy-1.2.8/audiconnectpy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-23 17:47:19.000000 audiconnectpy-1.2.8/audiconnectpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29813 2023-04-23 17:47:19.000000 audiconnectpy-1.2.8/audiconnectpy/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30341 2023-04-23 17:47:19.000000 audiconnectpy-1.2.8/audiconnectpy/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19549 2023-04-23 17:47:19.000000 audiconnectpy-1.2.8/audiconnectpy/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:47:31.480315 audiconnectpy-1.2.8/audiconnectpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-04-23 17:47:31.000000 audiconnectpy-1.2.8/audiconnectpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-23 17:47:31.000000 audiconnectpy-1.2.8/audiconnectpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 17:47:31.000000 audiconnectpy-1.2.8/audiconnectpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 17:47:31.000000 audiconnectpy-1.2.8/audiconnectpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-23 17:47:31.000000 audiconnectpy-1.2.8/audiconnectpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-23 17:47:19.000000 audiconnectpy-1.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 17:47:31.480315 audiconnectpy-1.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-23 17:47:28.000000 audiconnectpy-1.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:47:31.480315 audiconnectpy-1.2.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-23 17:47:19.000000 audiconnectpy-1.2.8/tests/__init__.py
```

### Comparing `audiconnectpy-1.2.7/LICENSE` & `audiconnectpy-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.2.7/PKG-INFO` & `audiconnectpy-1.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 1.2.7
+Version: 1.2.8
 Summary: Provides asynchronous authentication and access to Audi Connect
 Home-page: https://github.com/cyr-ius/audiconnectpy/tree/master/audiconnectpy
 Author: cyr-ius
 Author-email: cyr-ius@ipocus.net
 License: GPL-3
 Keywords: connect,async
 Classifier: Programming Language :: Python
```

### Comparing `audiconnectpy-1.2.7/README.md` & `audiconnectpy-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.2.7/audiconnectpy/api.py` & `audiconnectpy-1.2.8/audiconnectpy/api.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.2.7/audiconnectpy/auth.py` & `audiconnectpy-1.2.8/audiconnectpy/auth.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.2.7/audiconnectpy/models.py` & `audiconnectpy-1.2.8/audiconnectpy/models.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.2.7/audiconnectpy/services.py` & `audiconnectpy-1.2.8/audiconnectpy/services.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.2.7/audiconnectpy/util.py` & `audiconnectpy-1.2.8/audiconnectpy/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -319,14 +319,15 @@
     # Charger
     MAX_CHARGE_CURRENT = FieldType(
         attr="max_charge_current",
         sensor_type="number",
         icon="mdi:current-ac",
         unit_of_measurement="A",
         turn_mode="async_set_charger_max",
+        options=[0, 32],
     )
     CHARGING_STATE = FieldType(
         attr="charging_state",
         sensor_type="sensor",
         icon="mdi:car-battery",
     )
     ACTUAL_CHARGE_RATE = FieldType(
```

### Comparing `audiconnectpy-1.2.7/audiconnectpy.egg-info/PKG-INFO` & `audiconnectpy-1.2.8/audiconnectpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 1.2.7
+Version: 1.2.8
 Summary: Provides asynchronous authentication and access to Audi Connect
 Home-page: https://github.com/cyr-ius/audiconnectpy/tree/master/audiconnectpy
 Author: cyr-ius
 Author-email: cyr-ius@ipocus.net
 License: GPL-3
 Keywords: connect,async
 Classifier: Programming Language :: Python
```

### Comparing `audiconnectpy-1.2.7/pyproject.toml` & `audiconnectpy-1.2.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.2.7/setup.py` & `audiconnectpy-1.2.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Get the long description from the README file
 with open(os.path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name="audiconnectpy",
-    version="1.2.7",
+    version="1.2.8",
     packages=find_packages(),
     author="cyr-ius",
     author_email="cyr-ius@ipocus.net",
     description="Provides asynchronous authentication and access to Audi Connect",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=["aiohttp>=3.8.1", "beautifulsoup4>=4.11.2"],
```

