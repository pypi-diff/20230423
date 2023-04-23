# Comparing `tmp/audiconnectpy-1.2.8.tar.gz` & `tmp/audiconnectpy-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiconnectpy-1.2.8.tar", last modified: Sun Apr 23 17:47:31 2023, max compression
+gzip compressed data, was "audiconnectpy-1.2.9.tar", last modified: Sun Apr 23 17:55:18 2023, max compression
```

## Comparing `audiconnectpy-1.2.8.tar` & `audiconnectpy-1.2.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:47:31.480315 audiconnectpy-1.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-23 17:47:19.000000 audiconnectpy-1.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-23 17:47:19.000000 audiconnectpy-1.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-04-23 17:47:31.480315 audiconnectpy-1.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-04-23 17:47:19.000000 audiconnectpy-1.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:47:31.476315 audiconnectpy-1.2.8/audiconnectpy/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-23 17:47:19.000000 audiconnectpy-1.2.8/audiconnectpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-23 17:47:19.000000 audiconnectpy-1.2.8/audiconnectpy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    22276 2023-04-23 17:47:19.000000 audiconnectpy-1.2.8/audiconnectpy/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-23 17:47:19.000000 audiconnectpy-1.2.8/audiconnectpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    29813 2023-04-23 17:47:19.000000 audiconnectpy-1.2.8/audiconnectpy/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    30341 2023-04-23 17:47:19.000000 audiconnectpy-1.2.8/audiconnectpy/services.py
--rw-r--r--   0 runner    (1001) docker     (123)    19549 2023-04-23 17:47:19.000000 audiconnectpy-1.2.8/audiconnectpy/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:47:31.480315 audiconnectpy-1.2.8/audiconnectpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-04-23 17:47:31.000000 audiconnectpy-1.2.8/audiconnectpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-23 17:47:31.000000 audiconnectpy-1.2.8/audiconnectpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 17:47:31.000000 audiconnectpy-1.2.8/audiconnectpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 17:47:31.000000 audiconnectpy-1.2.8/audiconnectpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-23 17:47:31.000000 audiconnectpy-1.2.8/audiconnectpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-23 17:47:19.000000 audiconnectpy-1.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 17:47:31.480315 audiconnectpy-1.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-23 17:47:28.000000 audiconnectpy-1.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:47:31.480315 audiconnectpy-1.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-23 17:47:19.000000 audiconnectpy-1.2.8/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:55:18.922106 audiconnectpy-1.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-23 17:55:08.000000 audiconnectpy-1.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-23 17:55:08.000000 audiconnectpy-1.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-04-23 17:55:18.922106 audiconnectpy-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-04-23 17:55:08.000000 audiconnectpy-1.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:55:18.922106 audiconnectpy-1.2.9/audiconnectpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-23 17:55:08.000000 audiconnectpy-1.2.9/audiconnectpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-23 17:55:08.000000 audiconnectpy-1.2.9/audiconnectpy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22276 2023-04-23 17:55:08.000000 audiconnectpy-1.2.9/audiconnectpy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-23 17:55:08.000000 audiconnectpy-1.2.9/audiconnectpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29813 2023-04-23 17:55:08.000000 audiconnectpy-1.2.9/audiconnectpy/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30342 2023-04-23 17:55:08.000000 audiconnectpy-1.2.9/audiconnectpy/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19549 2023-04-23 17:55:08.000000 audiconnectpy-1.2.9/audiconnectpy/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:55:18.922106 audiconnectpy-1.2.9/audiconnectpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-04-23 17:55:18.000000 audiconnectpy-1.2.9/audiconnectpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-23 17:55:18.000000 audiconnectpy-1.2.9/audiconnectpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 17:55:18.000000 audiconnectpy-1.2.9/audiconnectpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 17:55:18.000000 audiconnectpy-1.2.9/audiconnectpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-23 17:55:18.000000 audiconnectpy-1.2.9/audiconnectpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-23 17:55:08.000000 audiconnectpy-1.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 17:55:18.922106 audiconnectpy-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-23 17:55:18.000000 audiconnectpy-1.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:55:18.922106 audiconnectpy-1.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-23 17:55:08.000000 audiconnectpy-1.2.9/tests/__init__.py
```

### Comparing `audiconnectpy-1.2.8/LICENSE` & `audiconnectpy-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.2.8/PKG-INFO` & `audiconnectpy-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 1.2.8
+Version: 1.2.9
 Summary: Provides asynchronous authentication and access to Audi Connect
 Home-page: https://github.com/cyr-ius/audiconnectpy/tree/master/audiconnectpy
 Author: cyr-ius
 Author-email: cyr-ius@ipocus.net
 License: GPL-3
 Keywords: connect,async
 Classifier: Programming Language :: Python
```

### Comparing `audiconnectpy-1.2.8/README.md` & `audiconnectpy-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.2.8/audiconnectpy/api.py` & `audiconnectpy-1.2.9/audiconnectpy/api.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.2.8/audiconnectpy/auth.py` & `audiconnectpy-1.2.9/audiconnectpy/auth.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.2.8/audiconnectpy/models.py` & `audiconnectpy-1.2.9/audiconnectpy/models.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.2.8/audiconnectpy/services.py` & `audiconnectpy-1.2.9/audiconnectpy/services.py`

 * *Files 0% similar despite different names*

```diff
@@ -543,15 +543,15 @@
         url = await self._async_get_home_region(vin.upper())
         data = '<?xml version="1.0" encoding= "UTF-8" ?>'
         data += f"<action><type>setSettings</type><settings><maxChargeCurrent>{int(current)}</maxChargeCurrent></settings></action>"
         headers = await self._auth.async_get_action_headers(
             "application/vnd.vwg.mbb.ChargerAction_v1_0_0+xml", None
         )
         res = await self._auth.post(
-            f"{url}/bs/batterycharge/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/charger/action",
+            f"{url}/bs/batterycharge/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/charger/actions",
             headers=headers,
             data=data,
             use_json=False,
         )
         actionid = get_attr(res, "action.actionId")
         await self.async_check_request_succeeded(
             f"{url}/bs/batterycharge/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/charger/actions/{actionid}",
```

### Comparing `audiconnectpy-1.2.8/audiconnectpy/util.py` & `audiconnectpy-1.2.9/audiconnectpy/util.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.2.8/audiconnectpy.egg-info/PKG-INFO` & `audiconnectpy-1.2.9/audiconnectpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 1.2.8
+Version: 1.2.9
 Summary: Provides asynchronous authentication and access to Audi Connect
 Home-page: https://github.com/cyr-ius/audiconnectpy/tree/master/audiconnectpy
 Author: cyr-ius
 Author-email: cyr-ius@ipocus.net
 License: GPL-3
 Keywords: connect,async
 Classifier: Programming Language :: Python
```

### Comparing `audiconnectpy-1.2.8/pyproject.toml` & `audiconnectpy-1.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.2.8/setup.py` & `audiconnectpy-1.2.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Get the long description from the README file
 with open(os.path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name="audiconnectpy",
-    version="1.2.8",
+    version="1.2.9",
     packages=find_packages(),
     author="cyr-ius",
     author_email="cyr-ius@ipocus.net",
     description="Provides asynchronous authentication and access to Audi Connect",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=["aiohttp>=3.8.1", "beautifulsoup4>=4.11.2"],
```

