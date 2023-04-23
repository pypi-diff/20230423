# Comparing `tmp/audiconnectpy-1.2.4.tar.gz` & `tmp/audiconnectpy-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiconnectpy-1.2.4.tar", last modified: Sun Apr 23 12:02:48 2023, max compression
+gzip compressed data, was "audiconnectpy-1.2.5.tar", last modified: Sun Apr 23 17:01:17 2023, max compression
```

## Comparing `audiconnectpy-1.2.4.tar` & `audiconnectpy-1.2.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:02:48.825129 audiconnectpy-1.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-23 12:02:35.000000 audiconnectpy-1.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-23 12:02:35.000000 audiconnectpy-1.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-04-23 12:02:48.825129 audiconnectpy-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-04-23 12:02:35.000000 audiconnectpy-1.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:02:48.821129 audiconnectpy-1.2.4/audiconnectpy/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-23 12:02:35.000000 audiconnectpy-1.2.4/audiconnectpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-23 12:02:35.000000 audiconnectpy-1.2.4/audiconnectpy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    22489 2023-04-23 12:02:35.000000 audiconnectpy-1.2.4/audiconnectpy/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-23 12:02:35.000000 audiconnectpy-1.2.4/audiconnectpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    29983 2023-04-23 12:02:35.000000 audiconnectpy-1.2.4/audiconnectpy/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    30211 2023-04-23 12:02:35.000000 audiconnectpy-1.2.4/audiconnectpy/services.py
--rw-r--r--   0 runner    (1001) docker     (123)    19478 2023-04-23 12:02:35.000000 audiconnectpy-1.2.4/audiconnectpy/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:02:48.825129 audiconnectpy-1.2.4/audiconnectpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-04-23 12:02:48.000000 audiconnectpy-1.2.4/audiconnectpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-23 12:02:48.000000 audiconnectpy-1.2.4/audiconnectpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 12:02:48.000000 audiconnectpy-1.2.4/audiconnectpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 12:02:48.000000 audiconnectpy-1.2.4/audiconnectpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-23 12:02:48.000000 audiconnectpy-1.2.4/audiconnectpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-23 12:02:35.000000 audiconnectpy-1.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 12:02:48.825129 audiconnectpy-1.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-23 12:02:46.000000 audiconnectpy-1.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:02:48.825129 audiconnectpy-1.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-23 12:02:35.000000 audiconnectpy-1.2.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:01:17.586630 audiconnectpy-1.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-23 17:01:07.000000 audiconnectpy-1.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-23 17:01:07.000000 audiconnectpy-1.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-04-23 17:01:17.582630 audiconnectpy-1.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-04-23 17:01:07.000000 audiconnectpy-1.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:01:17.582630 audiconnectpy-1.2.5/audiconnectpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-23 17:01:07.000000 audiconnectpy-1.2.5/audiconnectpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-23 17:01:07.000000 audiconnectpy-1.2.5/audiconnectpy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22276 2023-04-23 17:01:07.000000 audiconnectpy-1.2.5/audiconnectpy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-23 17:01:07.000000 audiconnectpy-1.2.5/audiconnectpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29822 2023-04-23 17:01:07.000000 audiconnectpy-1.2.5/audiconnectpy/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30327 2023-04-23 17:01:07.000000 audiconnectpy-1.2.5/audiconnectpy/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19479 2023-04-23 17:01:07.000000 audiconnectpy-1.2.5/audiconnectpy/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:01:17.582630 audiconnectpy-1.2.5/audiconnectpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-04-23 17:01:17.000000 audiconnectpy-1.2.5/audiconnectpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-23 17:01:17.000000 audiconnectpy-1.2.5/audiconnectpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 17:01:17.000000 audiconnectpy-1.2.5/audiconnectpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 17:01:17.000000 audiconnectpy-1.2.5/audiconnectpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-23 17:01:17.000000 audiconnectpy-1.2.5/audiconnectpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-23 17:01:07.000000 audiconnectpy-1.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 17:01:17.586630 audiconnectpy-1.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-23 17:01:16.000000 audiconnectpy-1.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:01:17.582630 audiconnectpy-1.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-23 17:01:07.000000 audiconnectpy-1.2.5/tests/__init__.py
```

### Comparing `audiconnectpy-1.2.4/LICENSE` & `audiconnectpy-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.2.4/PKG-INFO` & `audiconnectpy-1.2.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 1.2.4
+Version: 1.2.5
 Summary: Provides asynchronous authentication and access to Audi Connect
 Home-page: https://github.com/cyr-ius/audiconnectpy/tree/master/audiconnectpy
 Author: cyr-ius
 Author-email: cyr-ius@ipocus.net
 License: GPL-3
 Keywords: connect,async
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # audiconnectpy
```

### Comparing `audiconnectpy-1.2.4/README.md` & `audiconnectpy-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.2.4/audiconnectpy/api.py` & `audiconnectpy-1.2.5/audiconnectpy/api.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.2.4/audiconnectpy/auth.py` & `audiconnectpy-1.2.5/audiconnectpy/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 from .exceptions import (
     AudiException,
     HttpRequestError,
     ServiceNotFoundError,
     TimeoutExceededError,
 )
-from .util import get_attr, jload, json_loads, retry
+from .util import get_attr, jload, json_loads
 
 TIMEOUT = 120
 DELAY = 10
 HDR_XAPP_VERSION = "4.13.0"
 HDR_USER_AGENT = "myAudi-Android/4.13.0 (Build 800238275.2210271555) Android/11"
 MARKET_URL = "https://content.app.my.audi.com/service/mobileapp/configurations"
 CLIENT_ID = "09b6cbec-cd19-4589-82fd-363dfa8c24da@apps_vw-dilab_com"
@@ -150,37 +150,34 @@
         if use_json and data:
             data = json.dumps(data)
         response = await self.request(
             METH_POST, url, headers=headers, data=data, **kwargs
         )
         return response
 
-    @retry(exceptions=HttpRequestError, tries=3)
-    async def async_connect(self, username: str, password: str, country: str) -> bool:
+    async def async_connect(
+        self, username: str, password: str, country: str, tries: int = 3
+    ) -> bool:
         """Connect to API."""
         try:
             self._country = country
             await self._async_login(username, password)
-        except TimeoutExceededError as error:
-            _LOGGER.error("Login to Audi service failed: %s ", error)
+        except HttpRequestError as error:  # pylint: disable=broad-except
+            if tries > 1:
+                _LOGGER.warning(
+                    "Login to Audi service failed, trying again in %s seconds [ERROR:%s]",
+                    DELAY,
+                    str(error),
+                )
+                await asyncio.sleep(DELAY)
+                return await self.async_connect(username, password, country, tries - 1)
+            _LOGGER.error("Login to Audi service failed: %s ", str(error))
             return False
-        return True
-        # except HttpRequestError as error:  # pylint: disable=broad-except
-        #     if ntries > 1:
-        #         _LOGGER.error(
-        #             "Login to Audi service failed, trying again in %s seconds [ERROR:%s]",
-        #             DELAY,
-        #             str(error),
-        #         )
-        #         await asyncio.sleep(DELAY)
-        #         return await self.async_connect(username, password, country, ntries - 1)
-        #     _LOGGER.error("Login to Audi service failed: %s ", str(error))
-        #     return False
-        # else:
-        #     return True
+        else:
+            return True
 
     async def _async_login(self, user: str, password: str) -> None:
         """Request login."""
         await self._async_retrieve_url_service()
 
         # Generate code_challenge
         code_verifier = str(base64.urlsafe_b64encode(os.urandom(32)), "utf-8").strip(
```

### Comparing `audiconnectpy-1.2.4/audiconnectpy/models.py` & `audiconnectpy-1.2.5/audiconnectpy/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,15 +110,15 @@
         self.send_time = None
         self.send_time_utc = None
         self.measure_mileage = None
         self.send_mileage = None
         self._vehicle_data = self._get_attributes()
 
     @property
-    def vehicledata_supported(self) -> bool:
+    def is_supported(self) -> bool:
         """Supported status."""
         return self.attributes is not None
 
     @property
     def attributes(self) -> Any:
         """Attributes properties."""
         return self._vehicle_data
@@ -142,14 +142,15 @@
                 unit = raw_field.get("unit")
                 if ids == "0x0101010001":
                     self.measure_time = raw_field.get("tsCarCaptured")
                     self.send_time = raw_field.get("tsCarSent")
                     self.send_time_utc = raw_field.get("tsCarSentUtc")
                     self.measure_mileage = raw_field.get("milCarCaptured")
                     self.send_mileage = raw_field.get("milCarSent")
+                    _attributes.update(set_attr("LAST_UPDATE_TIME", self.send_time_utc))
 
                 if identity := self.IDS.get(ids):
                     _attributes.update(set_attr(identity, value, unit))
                 else:
                     _LOGGER.error("%s not found", ids)
 
         # Append meta sensors
@@ -254,15 +255,15 @@
 @dataclass
 class PreheaterDataResponse:
     """Preheater class."""
 
     data: dict[str, Any]
 
     @property
-    def preheater_supported(self) -> bool:
+    def is_supported(self) -> bool:
         """Supported status."""
         return self.attributes is not None
 
     @property
     def attributes(self) -> dict[Any, dict[str, Any]]:
         """Attributes properties."""
         _attributes = {}
@@ -285,15 +286,15 @@
 @dataclass
 class ChargerDataResponse:
     """Charger class."""
 
     data: dict[str, Any]
 
     @property
-    def charger_supported(self) -> bool:
+    def is_supported(self) -> bool:
         """Supported status."""
         return (
             get_attr(self.data, "charger.settings") is not None
             or get_attr(self.data, "charger.status") is not None
         )
 
     @property
@@ -394,15 +395,15 @@
 @dataclass
 class ClimaterDataResponse:
     """Climater class."""
 
     data: dict[str, Any]
 
     @property
-    def climater_supported(self) -> bool:
+    def is_supported(self) -> bool:
         """Supported status."""
         return self.attributes is not None
 
     @property
     def attributes(self) -> dict[Any, dict[str, Any]]:
         """Attributes properties."""
         _attributes = {}
@@ -464,15 +465,15 @@
 @dataclass
 class HistoryDataResponse:
     """Destination."""
 
     data: dict[str, Any]
 
     @property
-    def history_supported(self) -> bool:
+    def is_supported(self) -> bool:
         """Supported status."""
         return self.attributes is not None
 
     @property
     def attributes(self) -> dict[Any, dict[str, Any]]:
         """Attributes properties."""
         _attributes = {}
@@ -483,15 +484,15 @@
 @dataclass
 class UsersDataResponse:
     """Destination."""
 
     data: dict[str, Any]
 
     @property
-    def users_supported(self) -> bool:
+    def is_supported(self) -> bool:
         """Supported status."""
         return self.attributes is not None
 
     @property
     def attributes(self) -> dict[Any, dict[str, Any]]:
         """Attributes properties."""
         _attributes = {}
@@ -502,15 +503,15 @@
 @dataclass
 class PositionDataResponse:
     """Position class."""
 
     data: dict[str, Any]
 
     @property
-    def position_supported(self) -> bool:
+    def is_supported(self) -> bool:
         """Supported status."""
         return get_attr(self.data, "findCarResponse.Position") is not None
 
     @property
     def attributes(self) -> dict[Any, dict[str, Any]]:
         """Attributes properties."""
         _attributes = {}
@@ -530,14 +531,19 @@
 @dataclass
 class TripDataResponse:
     """Trip class."""
 
     data: dict[str, Any]
 
     @property
+    def is_supported(self) -> bool:
+        """Supported status."""
+        return self.data is not None
+
+    @property
     def attributes(self) -> dict[str, Any]:
         """Attributes properties."""
         trip_id = self.data["tripID"]
         average_electricengine_consumption = (
             (float(self.data["averageElectricEngineConsumption"]) / 10)
             if "averageElectricEngineConsumption" in self.data
             else None
@@ -570,19 +576,14 @@
             "mileage": mileage,
             "startMileage": start_mileage,
             "traveltime": travel_time,
             "timestamp": timestamp,
             "overallMileage": overall_mileage,
         }
 
-    @property
-    def trip_supported(self) -> bool:
-        """Supported status."""
-        return self.data is not None
-
 
 class Vehicle:
     """Vehicle class."""
 
     def __init__(self, data: Any, audi_service: AudiService) -> None:
         """Initialize."""
         self._audi_service = audi_service
@@ -634,18 +635,15 @@
 
     @retry(exceptions=TimeoutExceededError, tries=3, delay=2)
     async def async_update_vehicle(self) -> None:
         """Update vehicle status."""
         if self.support_vehicle is not False:
             try:
                 result = await self._audi_service.async_get_vehicle(self.vin)
-                if result.vehicledata_supported:
-                    self.states.update(
-                        set_attr("LAST_UPDATE_TIME", result.send_time_utc)
-                    )
+                if result.is_supported:
                     self.states.update(result.attributes)
             except ServiceNotFoundError as error:
                 if error.args[0] in (401, 403, 502):
                     self.support_vehicle = False
                 else:
                     _LOGGER.error(
                         "Unable to obtain the vehicle  status report of %s: %s",
@@ -655,23 +653,23 @@
             except HttpRequestError as error:
                 _LOGGER.error(
                     "Unable to obtain the vehicle  status report of %s: %s",
                     self.vin,
                     str(error).rstrip("\n"),
                 )
             else:
-                self.support_vehicle = result.vehicledata_supported
+                self.support_vehicle = result.is_supported
 
     @retry(exceptions=TimeoutExceededError, tries=3, delay=2)
     async def async_update_position(self) -> None:
         """Update vehicle position."""
         if self.support_position is not False:
             try:
                 result = await self._audi_service.async_get_stored_position(self.vin)
-                if result.position_supported:
+                if result.is_supported:
                     self.states.update(result.attributes)
             except ServiceNotFoundError as error:
                 if error.args[0] in (401, 403, 502):
                     self.support_position = False
                 # If error is 204 is returned, the position is currently not available
                 elif error.args[0] != 204:
                     _LOGGER.error(
@@ -682,23 +680,23 @@
             except HttpRequestError as error:
                 _LOGGER.error(
                     "Unable to obtain the vehicle position of %s: %s",
                     self.vin,
                     str(error).rstrip("\n"),
                 )
             else:
-                self.support_position = result.position_supported
+                self.support_position = result.is_supported
 
     @retry(exceptions=TimeoutExceededError, tries=3, delay=2)
     async def async_update_climater(self) -> None:
         """Update vehicle climater."""
         if self.support_climater is not False:
             try:
                 result = await self._audi_service.async_get_climater(self.vin)
-                if result.climater_supported:
+                if result.is_supported:
                     self.states.update(result.attributes)
             except ServiceNotFoundError as error:
                 if error.args[0] in (401, 403, 502):
                     self.support_climater = False
                 else:
                     _LOGGER.error(
                         "Unable to obtain the vehicle climatisation state for %s: %s",
@@ -708,23 +706,23 @@
             except HttpRequestError as error:
                 _LOGGER.error(
                     "Unable to obtain the vehicle climatisation state for %s: %s",
                     self.vin,
                     str(error).rstrip("\n"),
                 )
             else:
-                self.support_climater = result.climater_supported
+                self.support_climater = result.is_supported
 
     @retry(exceptions=TimeoutExceededError, tries=3, delay=2)
     async def async_update_preheater(self) -> None:
         """Update vehicle preheater."""
         if self.support_preheater is not False:
             try:
                 result = await self._audi_service.async_get_preheater(self.vin)
-                if result.preheater_supported:
+                if result.is_supported:
                     self.states.update(result.attributes)
             except ServiceNotFoundError as error:
                 if error.args[0] in (401, 403, 502):
                     self.support_preheater = False
                 else:
                     _LOGGER.error(
                         "Unable to obtain the vehicle preheater state for %s: %s",
@@ -734,23 +732,23 @@
             except HttpRequestError as error:
                 _LOGGER.error(
                     "Unable to obtain the vehicle preheater state for %s: %s",
                     self.vin,
                     str(error).rstrip("\n"),
                 )
             else:
-                self.support_preheater = result.preheater_supported
+                self.support_preheater = result.is_supported
 
     @retry(exceptions=TimeoutExceededError, tries=3, delay=2)
     async def async_update_charger(self) -> None:
         """Update vehicle charger."""
         if self.support_charger is not False:
             try:
                 result = await self._audi_service.async_get_charger(self.vin)
-                if result.charger_supported:
+                if result.is_supported:
                     self.states.update(result.attributes)
             except ServiceNotFoundError as error:
                 if error.args[0] in (401, 403, 502):
                     self.support_charger = False
                 else:
                     _LOGGER.error(
                         "Unable to obtain the vehicle charger state for %s: %s",
@@ -760,32 +758,32 @@
             except HttpRequestError as error:
                 _LOGGER.error(
                     "Unable to obtain the vehicle charger state for %s: %s",
                     self.vin,
                     str(error).rstrip("\n"),
                 )
             else:
-                self.support_charger = result.charger_supported
+                self.support_charger = result.is_supported
 
     @retry(exceptions=TimeoutExceededError, tries=3, delay=2)
     async def async_update_tripdata(
         self, kind: Literal["short", "long", "cyclic"]
     ) -> None:
         """Update vehicle trip."""
         if getattr(self, f"support_trip_{kind}") is not False:
             try:
                 td_cur, td_rst = await self._audi_service.async_get_tripdata(
                     self.vin, kind
                 )
-                if td_cur.trip_supported:
+                if td_cur.is_supported:
                     self.states.update(
                         set_attr(f"trip_{kind}_current", td_cur.attributes)
                     )
 
-                if td_rst.trip_supported:
+                if td_rst.is_supported:
                     self.states.update(
                         set_attr(f"trip_{kind}_reset", td_rst.attributes)
                     )
             except ServiceNotFoundError as error:
                 if error.args[0] in (400, 401, 403, 502):
                     setattr(self, f"support_trip_{kind}", False)
                 else:
```

### Comparing `audiconnectpy-1.2.4/audiconnectpy/services.py` & `audiconnectpy-1.2.5/audiconnectpy/services.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,105 +32,105 @@
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class AudiService:
     """Audi service."""
 
+    brand = "Audi"
+    _home_region: dict[str, str] = {}
+    _home_region_setter: dict[str, str] = {}
+    _heater_source: dict[str, Literal["electric", "auxiliary", "automatic"]] = {}
+    _control_duration: dict[str, int] = {}
+
     def __init__(self, auth: Auth, country: str, spin: int) -> None:
         """Initialize."""
         self._auth = auth
-        self._country: str = "DE" if country is None else country
-        self._type = "Audi"
+        self.country: str = "DE" if country is None else country
         self._spin = spin
-        self._home_region: dict[str, str] = {}
-        self._home_region_setter: dict[str, str] = {}
-        self._target_temp: int = 1950
-        self._heater_source: str = "electric"
-        self._control_duration: int = 60
 
     async def async_get_vehicles(self) -> Any:
         """Get all vehicles."""
         url = await self._async_get_home_region("")
         data = await self._auth.get(
-            f"{url}/usermanagement/users/v1/{self._type}/{self._country}/vehicles"
+            f"{url}/usermanagement/users/v1/{self.brand}/{self.country}/vehicles"
         )
         return data
 
     async def async_get_vehicle_details(self, vin: str) -> Any:
         """Get vehicle data."""
         url = await self._async_get_home_region(vin.upper())
         accept = {
             "Accept": "application/vnd.vwg.mbb.vehicleDataDetail_v2_1_0+json, application/vnd.vwg.mbb.genericError_v1_0_2+json"
         }
         headers = await self._auth.async_get_headers(token_type="mbb", headers=accept)
         data = await self._auth.get(
-            f"{url}/vehicleMgmt/vehicledata/v2/{self._type}/{self._country}/vehicles/{vin.upper()}/",
+            f"{url}/vehicleMgmt/vehicledata/v2/{self.brand}/{self.country}/vehicles/{vin.upper()}/",
             headers=headers,
         )
         return data
 
     async def async_get_vehicle(self, vin: str) -> VehicleDataResponse:
         """Get store data."""
         url = await self._async_get_home_region(vin.upper())
         data = await self._auth.get(
-            f"{url}/bs/vsr/v1/{self._type}/{self._country}/vehicles/{vin.upper()}/status"
+            f"{url}/bs/vsr/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/status"
         )
         return VehicleDataResponse(data, self._spin is not None)
 
     async def async_refresh_vehicle_data(self, vin: str) -> None:
         """Refresh vehicle data."""
         url = await self._async_get_home_region(vin.upper())
         data = await self._auth.post(
-            f"{url}/bs/vsr/v1/{self._type}/{self._country}/vehicles/{vin.upper()}/requests"
+            f"{url}/bs/vsr/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/requests"
         )
         request_id: str = get_attr(data, "CurrentVehicleDataResponse.requestId")
         await self.async_check_request_succeeded(
-            f"{url}/bs/vsr/v1/{self._type}/{self._country}/vehicles/{vin.upper()}/requests/{request_id}/jobstatus",
+            f"{url}/bs/vsr/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/requests/{request_id}/jobstatus",
             "refresh vehicle data",
             REQUEST_SUCCESSFUL,
             REQUEST_FAILED,
             "requestStatusResponse.status",
         )
 
     async def async_get_stored_position(self, vin: str) -> PositionDataResponse:
         """Get position data."""
         url = await self._async_get_home_region(vin.upper())
         data = await self._auth.get(
-            f"{url}/bs/cf/v1/{self._type}/{self._country}/vehicles/{vin.upper()}/position"
+            f"{url}/bs/cf/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/position"
         )
         return PositionDataResponse(data)
 
     async def async_get_destinations(self, vin: str) -> DestinationDataResponse:
         """Get destination data."""
         url = await self._async_get_home_region(vin.upper())
         data = await self._auth.get(
-            f"{url}/destinationfeedservice/mydestinations/v1/{self._type}/{self._country}/vehicles/{vin.upper()}/destinations"
+            f"{url}/destinationfeedservice/mydestinations/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/destinations"
         )
         return DestinationDataResponse(data)
 
     async def async_get_history(self, vin: str) -> HistoryDataResponse:
         """Get history data."""
         url = await self._async_get_home_region(vin.upper())
         data = await self._auth.get(
-            f"{url}/bs/dwap/v1/{self._type}/{self._country}/vehicles/{vin.upper()}/history"
+            f"{url}/bs/dwap/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/history"
         )
         return HistoryDataResponse(data)
 
     async def async_get_vehicule_users(self, vin: str) -> UsersDataResponse:
         """Get ufers of vehicle."""
         url = await self._async_get_home_region(vin.upper())
         data = await self._auth.get(f"{url}/bs/uic/v1/{vin.upper()}/users")
         return UsersDataResponse(data)
 
     async def async_get_charger(self, vin: str) -> ChargerDataResponse:
         """Get charger data."""
         url = await self._async_get_home_region(vin.upper())
         data = await self._auth.get(
-            f"{url}/bs/batterycharge/v1/{self._type}/{self._country}/vehicles/{vin.upper()}/charger"
+            f"{url}/bs/batterycharge/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/charger"
         )
         return ChargerDataResponse(data)
 
     async def async_get_tripdata(
         self, vin: str, kind: Literal["short", "long", "cyclic"]
     ) -> tuple[TripDataResponse, TripDataResponse]:
         """Get trip data."""
@@ -143,15 +143,15 @@
             "from": "1970-01-01T00:00:00Z",
             # "from":(datetime.utcnow() - timedelta(days=365)).strftime("%Y-%m-%dT%H:%M:%SZ"),
             "to": (datetime.utcnow() + timedelta(minutes=90)).strftime(
                 "%Y-%m-%dT%H:%M:%SZ"
             ),
         }
         data = await self._auth.get(
-            f"{url}/bs/tripstatistics/v1/{self._type}/{self._country}/vehicles/{vin.upper()}/tripdata/{kind}",
+            f"{url}/bs/tripstatistics/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/tripdata/{kind}",
             params=params,
         )
         td_sorted = sorted(
             get_attr(data, "tripDataList.tripData"),
             key=lambda k: k["overallMileage"],  # type: ignore[no-any-return]
             reverse=True,
         )
@@ -175,31 +175,31 @@
         )
         return data
 
     async def async_get_climater(self, vin: str) -> ClimaterDataResponse:
         """Get climater data."""
         url = await self._async_get_home_region(vin.upper())
         data = await self._auth.get(
-            f"{url}/bs/climatisation/v1/{self._type}/{self._country}/vehicles/{vin.upper()}/climater"
+            f"{url}/bs/climatisation/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/climater"
         )
         return ClimaterDataResponse(data)
 
     async def async_get_preheater(self, vin: str) -> PreheaterDataResponse:
         """Get Heater/Ventilation data."""
         url = await self._async_get_home_region(vin.upper())
         data = await self._auth.get(
-            f"{url}/bs/rs/v1/{self._type}/{self._country}/vehicles/{vin.upper()}/status"
+            f"{url}/bs/rs/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/status"
         )
         return PreheaterDataResponse(data)
 
     async def async_get_climater_timer(self, vin: str) -> Any:
         """Get timer."""
         url = await self._async_get_home_region(vin.upper())
         data = await self._auth.get(
-            f"{url}/bs/departuretimer/v1/{self._type}/{self._country}/vehicles/{vin.upper()}/timer"
+            f"{url}/bs/departuretimer/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/timer"
         )
         return data
 
     async def async_get_capabilities(self, vin: str) -> VehicleDataResponse:
         """Get capabilities."""
         url = "https://emea.bff.cariad.digital"
         headers = await self._auth.async_get_headers()
@@ -209,17 +209,17 @@
         return VehicleDataResponse(data, self._spin is not None)
 
     async def async_get_vehicle_information(self) -> Any:
         """Get vehicle information."""
         headers = await self._auth.async_get_headers(
             token_type="audi",
             headers={
-                "Accept-Language": f"{self._auth.language}-{self._country.upper()}",
+                "Accept-Language": f"{self._auth.language}-{self.country.upper()}",
                 "Content-Type": "application/json",
-                "X-User-Country": self._country.upper(),
+                "X-User-Country": self.country.upper(),
             },
         )
         data = {
             "query": "query vehicleList {\n userVehicles {\n vin\n mappingVin\n vehicle { core { modelYear\n }\n media { shortName\n longName }\n }\n csid\n commissionNumber\n type\n devicePlatform\n mbbConnect\n userRole {\n role\n }\n vehicle {\n classification {\n driveTrain\n }\n }\n nickname\n }\n}"
         }
         resp = await self._auth.post(
             "https://app-api.live-my.audi.com/vgql/v1/graphql",
@@ -231,15 +231,15 @@
             raise AudiException("Invalid json in vehicle information")
         return resp["data"]
 
     async def async_get_honkflash(self, vin: str) -> Any:
         """Get Honk & Flash status."""
         url = await self._async_get_home_region(vin.upper())
         data = await self._auth.get(
-            f"{url}/bs/rhf/v1/{self._type}/{self._country}/configuration"
+            f"{url}/bs/rhf/v1/{self.brand}/{self.country}/configuration"
         )
         return data
 
     async def async_get_personal_data(self) -> Any:
         """Get Honk & Flash status."""
         url = f"{self._auth.profil_url}/customers/{self._auth.user_id}"
         headers = await self._auth.async_get_headers()
@@ -274,39 +274,39 @@
     #     data = await self._auth.get(f"{url}/uic/v1/vin/{vin.upper()}/users", headers=headers)
     #     return data
 
     async def async_get_fences(self, vin: str) -> Any:
         """Get fences."""
         url = await self._async_get_home_region(vin.upper())
         data = await self._auth.get(
-            f"{url}/bs/geofencing/v1/{self._type}/{self._country}/vehicles/{vin.upper()}/geofencingAlerts"
+            f"{url}/bs/geofencing/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/geofencingAlerts"
         )
         return data
 
     async def async_get_fences_config(self, vin: str) -> Any:
         """Get fences configuration."""
         url = await self._async_get_home_region(vin.upper())
         data = await self._auth.get(
-            f"{url}/bs/geofencing/v1/{self._type}/{self._country}/vehicles/{vin.upper()}/geofencingConfiguration"
+            f"{url}/bs/geofencing/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/geofencingConfiguration"
         )
         return data
 
     async def async_get_speed_alert(self, vin: str) -> Any:
         """Get speed alert."""
         url = await self._async_get_home_region(vin.upper())
         data = await self._auth.get(
-            f"{url}/bs/speedalert/v1/{self._type}/{self._country}/vehicles/{vin.upper()}/speedAlerts"
+            f"{url}/bs/speedalert/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/speedAlerts"
         )
         return data
 
     async def async_get_speed_config(self, vin: str) -> Any:
         """Get speed alert configuration."""
         url = await self._async_get_home_region(vin.upper())
         data = await self._auth.get(
-            f"{url}/bs/speedalert/v1/{self._type}/{self._country}/vehicles/{vin.upper()}/speedAlertConfiguration"
+            f"{url}/bs/speedalert/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/speedAlertConfiguration"
         )
         return data
 
     async def async_lock(self, vin: str, lock: bool) -> None:
         """Set lock."""
         # OpenHab "lock","unlock"
         url = await self._async_get_home_region(vin.upper())
@@ -318,132 +318,131 @@
             },
             security_token=await self._async_get_security_token(
                 vin, "rlu_v1/operations/" + ("LOCK" if lock else "UNLOCK")
             ),
         )
 
         res = await self._auth.post(
-            f"{url}/bs/rlu/v1/{self._type}/{self._country}/vehicles/{vin.upper()}/actions",
+            f"{url}/bs/rlu/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/actions",
             headers=headers,
             data=data,
             use_json=False,
         )
 
         request_id = get_attr(res, "rluActionResponse.requestId")
         await self.async_check_request_succeeded(
-            f"{url}/bs/rlu/v1/{self._type}/{self._country}/vehicles/{vin.upper()}/requests/{request_id}/status",
+            f"{url}/bs/rlu/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/requests/{request_id}/status",
             "lock vehicle" if lock else "unlock vehicle",
             REQUEST_SUCCESSFUL,
             REQUEST_FAILED,
             "requestStatusResponse.status",
         )
 
     async def async_climater(self, vin: str, start: bool) -> None:
         """Set Climatisation."""
         # OpenHab "startClimatisation","stopClimatisation"
         url = await self._async_get_home_region(vin.upper())
+        heater_source = self._heater_source.get(vin, "electric")
         action = (
-            "P_START_CLIMA_EL"
-            if self._heater_source == "electric"
-            else "P_START_CLIMA_AU"
+            "P_START_CLIMA_EL" if heater_source == "electric" else "P_START_CLIMA_AU"
         )
         security_token = await self._async_get_security_token(
             vin, "rclima_v1/operations/" + (action if start else "P_QSTOPACT")
         )
         data = '<?xml version="1.0" encoding= "UTF-8" ?>'
         data += f'<action><type>{"startClimatisation" if start else "stopClimatisation"}</type>'
-        data += f"<settings><heaterSource>{self._heater_source}</heaterSource></settings></action>"
+        data += f"<settings><heaterSource>{heater_source}</heaterSource></settings></action>"
         headers = await self._auth.async_get_action_headers(
             "application/vnd.vwg.mbb.ClimaterAction_v1_0_0+xml", security_token
         )
 
         # headers = await self._auth.async_get_action_headers(
         #     "application/vnd.vwg.mbb.ClimaterAction_v1_0_2+json", security_token
         # )
         # data = (
         #     {
         #         "action": {
         #             "type": "startClimatisation",
         #             "settings": {
         #                 "climatisationWithoutHVpower": "without_hv_power",
-        #                 "heaterSource": self._heater_source,
+        #                 "heaterSource": heater_source,
         #             },
         #         }
         #     }
         #     if start
         #     else {"action": {"type": "stopClimatisation"}}
         # )
 
         res = await self._auth.post(
-            f"{url}/bs/climatisation/v1/{self._type}/{self._country}/vehicles/{vin.upper()}/climater/actions",
+            f"{url}/bs/climatisation/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/climater/actions",
             headers=headers,
             data=data,
             use_json=False,
         )
         actionid = get_attr(res, "action.actionId")
         await self.async_check_request_succeeded(
-            f"{url}/bs/climatisation/v1/{self._type}/{self._country}/vehicles/{vin.upper()}/climater/actions/{actionid}",
+            f"{url}/bs/climatisation/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/climater/actions/{actionid}",
             "start climatisation" if start else "stop climatisation",
             SUCCEEDED,
             FAILED,
             "action.actionState",
         )
 
     async def async_climater_temp(self, vin: str, temperature: float) -> None:
         """Set Climatisation temperature."""
         temperature = int(round(temperature, 1) * 10 + 2731)
         url = await self._async_get_home_region(vin.upper())
+        heater_source = self._heater_source.get(vin, "electric")
         data = '<?xml version="1.0" encoding= "UTF-8" ?>'
         data += f"<action><type>setSettings</type><settings><targetTemperature>{temperature}</targetTemperature>"
         data += "<climatisationWithoutHVpower>false</climatisationWithoutHVpower>"
-        data += (
-            f"<heaterSource>{self._heater_source}</heaterSource></settings></action>"
-        )
+        data += f"<heaterSource>{heater_source}</heaterSource></settings></action>"
         headers = await self._auth.async_get_action_headers(
             "application/vnd.vwg.mbb.ClimaterAction_v1_0_0+xml", None
         )
         # data = json.dumps(
         #     {
         #         "action": {
         #             "type": "setSettings",
         #             "settings": {
         #                 "targetTemperature": temperature,
         #                 "climatisationWithoutHVpower": True,
-        #                 "heaterSource": source,
+        #                 "heaterSource": heater_source,
         #                 "climaterElementSettings": {
         #                     "isClimatisationAtUnlock": False,
         #                     "isMirrorHeatingEnabled": True,
         #                 },
         #             },
         #         }
         #     }
         # )
         # headers = await self._auth.async_get_action_headers("application/json", None)
         res = await self._auth.post(
-            f"{url}/bs/climatisation/v1/{self._type}/{self._country}/vehicles/{vin.upper()}/climater/actions",
+            f"{url}/bs/climatisation/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/climater/actions",
             headers=headers,
             data=data,
             use_json=False,
         )
         actionid = get_attr(res, "action.actionId")
         await self.async_check_request_succeeded(
-            f"{url}/bs/climatisation/v1/{self._type}/{self._country}/vehicles/{vin.upper()}/climater/actions/{actionid}",
+            f"{url}/bs/climatisation/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/climater/actions/{actionid}",
             "set target temperature",
             SUCCEEDED,
             FAILED,
             "action.actionState",
         )
 
     async def async_pre_heating(self, vin: str, start: bool) -> None:
         """Set pre heater."""
         # OpenHab "startPreHeat","stopPreHeat"
         url = await self._async_get_home_region(vin.upper())
         security_token = await self._async_get_security_token(
             vin, "rheating_v1/operations/" + ("P_QSACT" if start else "P_QSTOPACT")
         )
+        # duration = self._control_duration.get(vin, 60)
         data = '<?xml version="1.0" encoding= "UTF-8" ?>'
         data += '<performAction xmlns="http://audi.de/connect/rs">'
         data += f'<quickstart><active>{"true" if start else "false"}</active></quickstart></performAction>'
         headers = await self._auth.async_get_action_headers(
             "application/vnd.vwg.mbb.RemoteStandheizung_v2_0_0+xml", security_token
         )
 
@@ -452,33 +451,34 @@
         # )
         # data = (
         #     {
         #         "performAction": {
         #             "quickstart": {
         #                 "startMode": "heating",
         #                 "active": True,
-        #                 "climatisationDuration": self._control_duration,
+        #                 "climatisationDuration": duration,
         #             }
         #         }
         #     }
         #     if start
         #     else {"performAction": {"quickstop": {"active": False}}}
         # )
 
         await self._auth.post(
-            f"{url}/bs/rs/v1/{self._type}/{self._country}/vehicles/{vin.upper()}/action",
+            f"{url}/bs/rs/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/action",
             headers=headers,
             data=data,
             use_json=False,
         )
 
     async def async_ventilation(self, vin: str, start: bool) -> None:
         """Set ventilation."""
         # OpenHab "startVentilation","stopVentilation"
         url = await self._async_get_home_region(vin.upper())
+        duration = self._control_duration.get(vin, 60)
         security_token = await self._async_get_security_token(
             vin, "rheating_v1/operations/" + ("P_QSACT" if start else "P_QSTOPACT")
         )
         # data = '<?xml version="1.0" encoding= "UTF-8" ?>'
         # data += '<performAction xmlns="http://audi.de/connect/rs">'
         # data += f'<quickstart><active>{"true" if start else "false"}</active>'
         # data += (
@@ -494,24 +494,24 @@
         )
         data = (
             {
                 "performAction": {
                     "quickstart": {
                         "startMode": "ventilation",
                         "active": True,
-                        "climatisationDuration": self._control_duration,
+                        "climatisationDuration": duration,
                     }
                 }
             }
             if start
             else {"performAction": {"quickstop": {"active": False}}}
         )
 
         await self._auth.post(
-            f"{url}/bs/rs/v1/{self._type}/{self._country}/vehicles/{vin.upper()}/action",
+            f"{url}/bs/rs/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/action",
             headers=headers,
             data=data,
             use_json=True,
         )
 
     async def async_charger(self, vin: str, start: bool) -> None:
         """Set charger."""
@@ -519,23 +519,23 @@
         url = await self._async_get_home_region(vin.upper())
         data = '<?xml version="1.0" encoding= "UTF-8" ?>'
         data += f'<action><type>{"true" if start else "false"}</type></action>'
         headers = await self._auth.async_get_action_headers(
             "application/vnd.vwg.mbb.ChargerAction_v1_0_0+xml", None
         )
         res = await self._auth.post(
-            f"{url}/bs/batterycharge/v1/{self._type}/{self._country}/vehicles/{vin.upper()}/charger/actions",
+            f"{url}/bs/batterycharge/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/charger/actions",
             headers=headers,
             data=data,
             use_json=False,
         )
 
         actionid = get_attr(res, "action.actionId")
         await self.async_check_request_succeeded(
-            f"{url}/bs/batterycharge/v1/{self._type}/{self._country}/vehicles/{vin.upper()}/charger/actions/{actionid}",
+            f"{url}/bs/batterycharge/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/charger/actions/{actionid}",
             "start charger" if start else "stop charger",
             SUCCEEDED,
             FAILED,
             "action.actionState",
         )
 
     async def async_set_charger_max(self, vin: str, current: int = 32) -> None:
@@ -543,71 +543,71 @@
         url = await self._async_get_home_region(vin.upper())
         data = '<?xml version="1.0" encoding= "UTF-8" ?>'
         data += f"<action><type>setSettings</type><settings><maxChargeCurrent>{current}</maxChargeCurrent></settings></action>"
         headers = await self._auth.async_get_action_headers(
             "application/vnd.vwg.mbb.ChargerAction_v1_0_0+xml", None
         )
         res = await self._auth.post(
-            f"{url}/bs/batterycharge/v1/{self._type}/{self._country}/vehicles/{vin.upper()}/charger/action",
+            f"{url}/bs/batterycharge/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/charger/action",
             headers=headers,
             data=data,
             use_json=False,
         )
         actionid = get_attr(res, "action.actionId")
         await self.async_check_request_succeeded(
-            f"{url}/bs/batterycharge/v1/{self._type}/{self._country}/vehicles/{vin.upper()}/charger/actions/{actionid}",
+            f"{url}/bs/batterycharge/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/charger/actions/{actionid}",
             "set charger max current",
             SUCCEEDED,
             FAILED,
             "action.actionState",
         )
 
     async def set_heater_source(
-        self, mode: Literal["electric", "auxiliary", "automatic"]
+        self, vin: str, mode: Literal["electric", "auxiliary", "automatic"]
     ) -> None:
         """Set max current."""
         if mode in ["electric", "auxiliary", "automatic"]:
-            self._heater_source = mode
+            self._heater_source[vin] = mode
 
     async def async_window_heating(self, vin: str, start: bool) -> None:
         """Set window heating."""
         # OpenHab "startWindowHeating","stopWindowHeating"
         url = await self._async_get_home_region(vin.upper())
         data = '<?xml version="1.0" encoding= "UTF-8" ?>'
         data += f"<action><type>{'startWindowHeating' if start else 'stopWindowHeating'}</type></action>"
         headers = await self._auth.async_get_action_headers(
             "application/vnd.vwg.mbb.ClimaterAction_v1_0_0+xml", None
         )
         res = await self._auth.post(
-            f"{url}/bs/climatisation/v1/{self._type}/{self._country}/vehicles/{vin.upper()}/climater/actions",
+            f"{url}/bs/climatisation/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/climater/actions",
             headers=headers,
             data=data,
             use_json=False,
         )
         actionid = get_attr(res, "action.actionId")
         await self.async_check_request_succeeded(
-            f"{url}/bs/climatisation/v1/{self._type}/{self._country}/vehicles/{vin.upper()}/climater/actions/{actionid}",
+            f"{url}/bs/climatisation/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/climater/actions/{actionid}",
             "start window heating" if start else "stop window heating",
             SUCCEEDED,
             FAILED,
             "action.actionState",
         )
 
-    async def set_control_duration(self, duration: int) -> None:
+    async def set_control_duration(self, vin: str, duration: int) -> None:
         """Set max current."""
-        self._control_duration = duration
+        self._control_duration[vin] = duration
 
     async def async_set_honkflash(
         self, vin: str, mode: Literal["honk", "flash"], duration: int = 15
     ) -> None:
         """Set honk and flash light."""
         # OpenHab "FLASH_ONLY","HONK_AND_FLASH"
         url = await self._async_get_home_region(vin.upper())
         rsp_position = await self._auth.get(
-            f"{url}/bs/cf/v1/{self._type}/{self._country}/vehicles/{vin.upper()}/position"
+            f"{url}/bs/cf/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/position"
         )
         position = (
             rsp_position.get("findCarResponse", {})
             .get("Position", {})
             .get("carCoordinate")
         )
 
@@ -621,15 +621,15 @@
                 "userPosition": {
                     "latitude": position["latitude"],
                     "longitude": position["longitude"],
                 },
             }
         }
         await self._auth.post(
-            f"{url}/bs/rhf/v1/{self._type}/{self._country}/vehicles/{vin.upper()}/honkAndFlash",
+            f"{url}/bs/rhf/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/honkAndFlash",
             headers=headers,
             data=data,
         )
 
     async def async_check_request_succeeded(
         self, url: str, action: str, success: str, failed: str, path: str
     ) -> None:
```

### Comparing `audiconnectpy-1.2.4/audiconnectpy/util.py` & `audiconnectpy-1.2.5/audiconnectpy/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -603,15 +603,15 @@
                 except exceptions as error:  # pylint: disable=broad-except
                     _tries -= 1
                     if not _tries:
                         logger.error("%s, timeout exceeded", error)
                         raise TimeoutExceededError(error) from error
 
                     if logger is not None:
-                        logger.warning("%s, retrying in %s seconds...", error, _delay)
+                        logger.warning("%s, trying again in %s seconds", error, _delay)
 
                     time.sleep(_delay)
                     _delay *= backoff
 
                     if isinstance(jitter, tuple):
                         _delay += random.uniform(*jitter)
                     else:
```

### Comparing `audiconnectpy-1.2.4/audiconnectpy.egg-info/PKG-INFO` & `audiconnectpy-1.2.5/audiconnectpy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 1.2.4
+Version: 1.2.5
 Summary: Provides asynchronous authentication and access to Audi Connect
 Home-page: https://github.com/cyr-ius/audiconnectpy/tree/master/audiconnectpy
 Author: cyr-ius
 Author-email: cyr-ius@ipocus.net
 License: GPL-3
 Keywords: connect,async
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # audiconnectpy
```

### Comparing `audiconnectpy-1.2.4/pyproject.toml` & `audiconnectpy-1.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.2.4/setup.py` & `audiconnectpy-1.2.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Get the long description from the README file
 with open(os.path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name="audiconnectpy",
-    version="1.2.4",
+    version="1.2.5",
     packages=find_packages(),
     author="cyr-ius",
     author_email="cyr-ius@ipocus.net",
     description="Provides asynchronous authentication and access to Audi Connect",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=["aiohttp>=3.8.1", "beautifulsoup4>=4.11.2"],
@@ -30,12 +30,13 @@
     keywords=["connect", "async"],
     classifiers=[
         "Programming Language :: Python",
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Framework :: AsyncIO",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
 )
```

