# Comparing `tmp/audiconnectpy-1.2.6.tar.gz` & `tmp/audiconnectpy-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiconnectpy-1.2.6.tar", last modified: Sun Apr 23 17:33:41 2023, max compression
+gzip compressed data, was "audiconnectpy-1.2.7.tar", last modified: Sun Apr 23 17:44:42 2023, max compression
```

## Comparing `audiconnectpy-1.2.6.tar` & `audiconnectpy-1.2.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:33:41.453297 audiconnectpy-1.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-23 17:33:30.000000 audiconnectpy-1.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-23 17:33:30.000000 audiconnectpy-1.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-04-23 17:33:41.453297 audiconnectpy-1.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-04-23 17:33:30.000000 audiconnectpy-1.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:33:41.453297 audiconnectpy-1.2.6/audiconnectpy/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-23 17:33:30.000000 audiconnectpy-1.2.6/audiconnectpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-23 17:33:30.000000 audiconnectpy-1.2.6/audiconnectpy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    22276 2023-04-23 17:33:30.000000 audiconnectpy-1.2.6/audiconnectpy/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-23 17:33:30.000000 audiconnectpy-1.2.6/audiconnectpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    29813 2023-04-23 17:33:30.000000 audiconnectpy-1.2.6/audiconnectpy/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    30327 2023-04-23 17:33:30.000000 audiconnectpy-1.2.6/audiconnectpy/services.py
--rw-r--r--   0 runner    (1001) docker     (123)    19481 2023-04-23 17:33:30.000000 audiconnectpy-1.2.6/audiconnectpy/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:33:41.453297 audiconnectpy-1.2.6/audiconnectpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-04-23 17:33:41.000000 audiconnectpy-1.2.6/audiconnectpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-23 17:33:41.000000 audiconnectpy-1.2.6/audiconnectpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 17:33:41.000000 audiconnectpy-1.2.6/audiconnectpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 17:33:41.000000 audiconnectpy-1.2.6/audiconnectpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-23 17:33:41.000000 audiconnectpy-1.2.6/audiconnectpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-23 17:33:30.000000 audiconnectpy-1.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 17:33:41.453297 audiconnectpy-1.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-23 17:33:40.000000 audiconnectpy-1.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:33:41.453297 audiconnectpy-1.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-23 17:33:30.000000 audiconnectpy-1.2.6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:44:42.634061 audiconnectpy-1.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-23 17:44:31.000000 audiconnectpy-1.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-23 17:44:31.000000 audiconnectpy-1.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-04-23 17:44:42.634061 audiconnectpy-1.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-04-23 17:44:31.000000 audiconnectpy-1.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:44:42.630061 audiconnectpy-1.2.7/audiconnectpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-23 17:44:31.000000 audiconnectpy-1.2.7/audiconnectpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-23 17:44:31.000000 audiconnectpy-1.2.7/audiconnectpy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22276 2023-04-23 17:44:31.000000 audiconnectpy-1.2.7/audiconnectpy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-23 17:44:31.000000 audiconnectpy-1.2.7/audiconnectpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29813 2023-04-23 17:44:31.000000 audiconnectpy-1.2.7/audiconnectpy/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30341 2023-04-23 17:44:31.000000 audiconnectpy-1.2.7/audiconnectpy/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19524 2023-04-23 17:44:31.000000 audiconnectpy-1.2.7/audiconnectpy/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:44:42.630061 audiconnectpy-1.2.7/audiconnectpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-04-23 17:44:42.000000 audiconnectpy-1.2.7/audiconnectpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-23 17:44:42.000000 audiconnectpy-1.2.7/audiconnectpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 17:44:42.000000 audiconnectpy-1.2.7/audiconnectpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 17:44:42.000000 audiconnectpy-1.2.7/audiconnectpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-23 17:44:42.000000 audiconnectpy-1.2.7/audiconnectpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-23 17:44:31.000000 audiconnectpy-1.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 17:44:42.634061 audiconnectpy-1.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-23 17:44:40.000000 audiconnectpy-1.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:44:42.630061 audiconnectpy-1.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-23 17:44:31.000000 audiconnectpy-1.2.7/tests/__init__.py
```

### Comparing `audiconnectpy-1.2.6/LICENSE` & `audiconnectpy-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.2.6/PKG-INFO` & `audiconnectpy-1.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 1.2.6
+Version: 1.2.7
 Summary: Provides asynchronous authentication and access to Audi Connect
 Home-page: https://github.com/cyr-ius/audiconnectpy/tree/master/audiconnectpy
 Author: cyr-ius
 Author-email: cyr-ius@ipocus.net
 License: GPL-3
 Keywords: connect,async
 Classifier: Programming Language :: Python
```

### Comparing `audiconnectpy-1.2.6/README.md` & `audiconnectpy-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.2.6/audiconnectpy/api.py` & `audiconnectpy-1.2.7/audiconnectpy/api.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.2.6/audiconnectpy/auth.py` & `audiconnectpy-1.2.7/audiconnectpy/auth.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.2.6/audiconnectpy/models.py` & `audiconnectpy-1.2.7/audiconnectpy/models.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.2.6/audiconnectpy/services.py` & `audiconnectpy-1.2.7/audiconnectpy/services.py`

 * *Files 1% similar despite different names*

```diff
@@ -383,15 +383,15 @@
             f"{url}/bs/climatisation/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/climater/actions/{actionid}",
             "start climatisation" if start else "stop climatisation",
             SUCCEEDED,
             FAILED,
             "action.actionState",
         )
 
-    async def async_climater_temp(self, vin: str, temperature: float) -> None:
+    async def async_climater_temp(self, vin: str, temperature: float = 19.5) -> None:
         """Set Climatisation temperature."""
         temperature = int(round(temperature, 1) * 10 + 2731)
         url = await self._async_get_home_region(vin.upper())
         heater_source = self._heater_source.get(vin, "electric")
         data = '<?xml version="1.0" encoding= "UTF-8" ?>'
         data += f"<action><type>setSettings</type><settings><targetTemperature>{temperature}</targetTemperature>"
         data += "<climatisationWithoutHVpower>false</climatisationWithoutHVpower>"
@@ -534,19 +534,19 @@
             f"{url}/bs/batterycharge/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/charger/actions/{actionid}",
             "start charger" if start else "stop charger",
             SUCCEEDED,
             FAILED,
             "action.actionState",
         )
 
-    async def async_set_charger_max(self, vin: str, current: int = 32) -> None:
+    async def async_set_charger_max(self, vin: str, current: float = 32) -> None:
         """Set max current."""
         url = await self._async_get_home_region(vin.upper())
         data = '<?xml version="1.0" encoding= "UTF-8" ?>'
-        data += f"<action><type>setSettings</type><settings><maxChargeCurrent>{current}</maxChargeCurrent></settings></action>"
+        data += f"<action><type>setSettings</type><settings><maxChargeCurrent>{int(current)}</maxChargeCurrent></settings></action>"
         headers = await self._auth.async_get_action_headers(
             "application/vnd.vwg.mbb.ChargerAction_v1_0_0+xml", None
         )
         res = await self._auth.post(
             f"{url}/bs/batterycharge/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/charger/action",
             headers=headers,
             data=data,
```

### Comparing `audiconnectpy-1.2.6/audiconnectpy/util.py` & `audiconnectpy-1.2.7/audiconnectpy/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -315,17 +315,18 @@
         icon="mdi:clock",
         unit_of_measurement="Min",
     )
 
     # Charger
     MAX_CHARGE_CURRENT = FieldType(
         attr="max_charge_current",
-        sensor_type="sensor",
+        sensor_type="number",
         icon="mdi:current-ac",
         unit_of_measurement="A",
+        turn_mode="async_set_charger_max",
     )
     CHARGING_STATE = FieldType(
         attr="charging_state",
         sensor_type="sensor",
         icon="mdi:car-battery",
     )
     ACTUAL_CHARGE_RATE = FieldType(
```

### Comparing `audiconnectpy-1.2.6/audiconnectpy.egg-info/PKG-INFO` & `audiconnectpy-1.2.7/audiconnectpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 1.2.6
+Version: 1.2.7
 Summary: Provides asynchronous authentication and access to Audi Connect
 Home-page: https://github.com/cyr-ius/audiconnectpy/tree/master/audiconnectpy
 Author: cyr-ius
 Author-email: cyr-ius@ipocus.net
 License: GPL-3
 Keywords: connect,async
 Classifier: Programming Language :: Python
```

### Comparing `audiconnectpy-1.2.6/pyproject.toml` & `audiconnectpy-1.2.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.2.6/setup.py` & `audiconnectpy-1.2.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Get the long description from the README file
 with open(os.path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name="audiconnectpy",
-    version="1.2.6",
+    version="1.2.7",
     packages=find_packages(),
     author="cyr-ius",
     author_email="cyr-ius@ipocus.net",
     description="Provides asynchronous authentication and access to Audi Connect",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=["aiohttp>=3.8.1", "beautifulsoup4>=4.11.2"],
```

