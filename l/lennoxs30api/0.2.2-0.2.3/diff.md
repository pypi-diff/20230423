# Comparing `tmp/lennoxs30api-0.2.2.tar.gz` & `tmp/lennoxs30api-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lennoxs30api-0.2.2.tar", last modified: Fri Apr 14 23:30:21 2023, max compression
+gzip compressed data, was "lennoxs30api-0.2.3.tar", last modified: Sun Apr 23 15:05:41 2023, max compression
```

## Comparing `lennoxs30api-0.2.2.tar` & `lennoxs30api-0.2.3.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxrwxrwx   0 pete      (1000) pete      (1000)        0 2023-04-14 23:30:21.036753 lennoxs30api-0.2.2/
--rwxrwxrwx   0 pete      (1000) pete      (1000)     1092 2021-06-16 19:56:17.000000 lennoxs30api-0.2.2/LICENSE
--rwxrwxrwx   0 pete      (1000) pete      (1000)     2535 2023-04-14 23:30:21.033755 lennoxs30api-0.2.2/PKG-INFO
--rwxrwxrwx   0 pete      (1000) pete      (1000)     2140 2021-07-18 14:46:26.000000 lennoxs30api-0.2.2/README.md
-drwxrwxrwx   0 pete      (1000) pete      (1000)        0 2023-04-14 23:30:20.942763 lennoxs30api-0.2.2/lennoxs30api/
--rwxrwxrwx   0 pete      (1000) pete      (1000)      171 2023-04-14 23:27:17.000000 lennoxs30api-0.2.2/lennoxs30api/__init__.py
--rwxrwxrwx   0 pete      (1000) pete      (1000)     5357 2022-09-03 00:30:25.000000 lennoxs30api-0.2.2/lennoxs30api/lennox_equipment.py
--rwxrwxrwx   0 pete      (1000) pete      (1000)    29143 2022-10-18 13:38:00.000000 lennoxs30api-0.2.2/lennoxs30api/lennox_errors.py
--rwxrwxrwx   0 pete      (1000) pete      (1000)      627 2021-12-24 15:46:31.000000 lennoxs30api-0.2.2/lennoxs30api/lennox_home.py
--rwxrwxrwx   0 pete      (1000) pete      (1000)     1613 2021-06-25 11:10:06.000000 lennoxs30api-0.2.2/lennoxs30api/lennox_period.py
--rwxrwxrwx   0 pete      (1000) pete      (1000)     1118 2021-06-25 11:10:06.000000 lennoxs30api-0.2.2/lennoxs30api/lennox_schedule.py
--rwxrwxrwx   0 pete      (1000) pete      (1000)     2938 2022-05-22 21:24:48.000000 lennoxs30api-0.2.2/lennoxs30api/message_logger.py
--rwxrwxrwx   0 pete      (1000) pete      (1000)     3973 2022-05-22 21:24:48.000000 lennoxs30api-0.2.2/lennoxs30api/metrics.py
--rwxrwxrwx   0 pete      (1000) pete      (1000)   126146 2023-04-14 23:27:17.000000 lennoxs30api-0.2.2/lennoxs30api/s30api_async.py
--rwxrwxrwx   0 pete      (1000) pete      (1000)     2964 2022-12-15 21:56:21.000000 lennoxs30api-0.2.2/lennoxs30api/s30exception.py
-drwxrwxrwx   0 pete      (1000) pete      (1000)        0 2023-04-14 23:30:21.015753 lennoxs30api-0.2.2/lennoxs30api.egg-info/
--rwxrwxrwx   0 pete      (1000) pete      (1000)     2535 2023-04-14 23:30:20.000000 lennoxs30api-0.2.2/lennoxs30api.egg-info/PKG-INFO
--rwxrwxrwx   0 pete      (1000) pete      (1000)      496 2023-04-14 23:30:20.000000 lennoxs30api-0.2.2/lennoxs30api.egg-info/SOURCES.txt
--rwxrwxrwx   0 pete      (1000) pete      (1000)        1 2023-04-14 23:30:20.000000 lennoxs30api-0.2.2/lennoxs30api.egg-info/dependency_links.txt
--rwxrwxrwx   0 pete      (1000) pete      (1000)        8 2023-04-14 23:30:20.000000 lennoxs30api-0.2.2/lennoxs30api.egg-info/requires.txt
--rwxrwxrwx   0 pete      (1000) pete      (1000)       13 2023-04-14 23:30:20.000000 lennoxs30api-0.2.2/lennoxs30api.egg-info/top_level.txt
--rwxrwxrwx   0 pete      (1000) pete      (1000)       38 2023-04-14 23:30:21.038754 lennoxs30api-0.2.2/setup.cfg
--rwxrwxrwx   0 pete      (1000) pete      (1000)      697 2023-04-14 23:27:17.000000 lennoxs30api-0.2.2/setup.py
+drwxrwxrwx   0 pete      (1000) pete      (1000)        0 2023-04-23 15:05:41.034974 lennoxs30api-0.2.3/
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     1092 2021-06-16 19:56:17.000000 lennoxs30api-0.2.3/LICENSE
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     2535 2023-04-23 15:05:41.032972 lennoxs30api-0.2.3/PKG-INFO
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     2140 2021-07-18 14:46:26.000000 lennoxs30api-0.2.3/README.md
+drwxrwxrwx   0 pete      (1000) pete      (1000)        0 2023-04-23 15:05:40.936972 lennoxs30api-0.2.3/lennoxs30api/
+-rwxrwxrwx   0 pete      (1000) pete      (1000)      171 2023-04-23 14:36:07.000000 lennoxs30api-0.2.3/lennoxs30api/__init__.py
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     3188 2023-04-23 14:36:07.000000 lennoxs30api-0.2.3/lennoxs30api/lennox_ble.py
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     5357 2022-09-03 00:30:25.000000 lennoxs30api-0.2.3/lennoxs30api/lennox_equipment.py
+-rwxrwxrwx   0 pete      (1000) pete      (1000)    29143 2022-10-18 13:38:00.000000 lennoxs30api-0.2.3/lennoxs30api/lennox_errors.py
+-rwxrwxrwx   0 pete      (1000) pete      (1000)      627 2021-12-24 15:46:31.000000 lennoxs30api-0.2.3/lennoxs30api/lennox_home.py
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     1613 2021-06-25 11:10:06.000000 lennoxs30api-0.2.3/lennoxs30api/lennox_period.py
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     1118 2021-06-25 11:10:06.000000 lennoxs30api-0.2.3/lennoxs30api/lennox_schedule.py
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     2938 2022-05-22 21:24:48.000000 lennoxs30api-0.2.3/lennoxs30api/message_logger.py
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     3903 2023-04-23 14:36:07.000000 lennoxs30api-0.2.3/lennoxs30api/metrics.py
+-rwxrwxrwx   0 pete      (1000) pete      (1000)   128419 2023-04-23 14:36:07.000000 lennoxs30api-0.2.3/lennoxs30api/s30api_async.py
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     2964 2022-12-15 21:56:21.000000 lennoxs30api-0.2.3/lennoxs30api/s30exception.py
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     2414 2023-04-23 14:36:07.000000 lennoxs30api-0.2.3/lennoxs30api/subscriber_base.py
+drwxrwxrwx   0 pete      (1000) pete      (1000)        0 2023-04-23 15:05:41.015972 lennoxs30api-0.2.3/lennoxs30api.egg-info/
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     2535 2023-04-23 15:05:40.000000 lennoxs30api-0.2.3/lennoxs30api.egg-info/PKG-INFO
+-rwxrwxrwx   0 pete      (1000) pete      (1000)      555 2023-04-23 15:05:40.000000 lennoxs30api-0.2.3/lennoxs30api.egg-info/SOURCES.txt
+-rwxrwxrwx   0 pete      (1000) pete      (1000)        1 2023-04-23 15:05:40.000000 lennoxs30api-0.2.3/lennoxs30api.egg-info/dependency_links.txt
+-rwxrwxrwx   0 pete      (1000) pete      (1000)        8 2023-04-23 15:05:40.000000 lennoxs30api-0.2.3/lennoxs30api.egg-info/requires.txt
+-rwxrwxrwx   0 pete      (1000) pete      (1000)       13 2023-04-23 15:05:40.000000 lennoxs30api-0.2.3/lennoxs30api.egg-info/top_level.txt
+-rwxrwxrwx   0 pete      (1000) pete      (1000)       38 2023-04-23 15:05:41.035977 lennoxs30api-0.2.3/setup.cfg
+-rwxrwxrwx   0 pete      (1000) pete      (1000)      697 2023-04-23 14:36:07.000000 lennoxs30api-0.2.3/setup.py
```

### Comparing `lennoxs30api-0.2.2/LICENSE` & `lennoxs30api-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.2/PKG-INFO` & `lennoxs30api-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lennoxs30api
-Version: 0.2.2
+Version: 0.2.3
 Summary: API Wrapper for Lennox S30 Cloud and LAN API
 Home-page: https://github.com/PeteRager/lennoxs30api
 Author: Pete Rage
 Author-email: pete.rager@x.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lennoxs30api-0.2.2/README.md` & `lennoxs30api-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.2/lennoxs30api/lennox_equipment.py` & `lennoxs30api-0.2.3/lennoxs30api/lennox_equipment.py`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.2/lennoxs30api/lennox_errors.py` & `lennoxs30api-0.2.3/lennoxs30api/lennox_errors.py`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.2/lennoxs30api/lennox_home.py` & `lennoxs30api-0.2.3/lennoxs30api/lennox_home.py`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.2/lennoxs30api/lennox_period.py` & `lennoxs30api-0.2.3/lennoxs30api/lennox_period.py`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.2/lennoxs30api/lennox_schedule.py` & `lennoxs30api-0.2.3/lennoxs30api/lennox_schedule.py`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.2/lennoxs30api/message_logger.py` & `lennoxs30api-0.2.3/lennoxs30api/message_logger.py`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.2/lennoxs30api/metrics.py` & `lennoxs30api-0.2.3/lennoxs30api/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,13 +107,11 @@
         if http_code >= 200 and http_code <= 299:
             self.http_2xx_cnt += 1
             return
 
         self.error_count += 1
         if http_code >= 400 and http_code <= 499:
             self.http_4xx_cnt += 1
-            self.error_count += 1
         elif http_code >= 500 and http_code <= 599:
             self.http_5xx_cnt += 1
-            self.error_count += 1
 
         self.last_error_time = self.now()
```

### Comparing `lennoxs30api-0.2.2/lennoxs30api/s30api_async.py` & `lennoxs30api-0.2.3/lennoxs30api/s30api_async.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# pylint: disable=line-too-long
 """
 Lennox iComfort S30/E30/M30  API.
 
 By Pete Rager
 
 Notes:
   This API currently only supports manual mode (no programs) on the thermostat.
@@ -13,14 +12,43 @@
 
 Ideas/Future:
 
 Change log:
 v0.2.0 - Initial Release
 
 """
+# pylint: disable=line-too-long
+# pylint: disable=logging-fstring-interpolation
+# pylint: disable=logging-not-lazy
+# pylint: disable=invalid-name
+# pylint: disable=broad-exception-caught
+# pylint: disable=protected-access
+# pylint: disable=too-many-lines
+# pylint: disable=missing-function-docstring
+# pylint: disable=consider-using-dict-items
+
+from datetime import datetime
+import logging
+import json
+import uuid
+import ssl
+from typing import Final, List
+from urllib.parse import quote
+
+from aiohttp import ClientTimeout, ClientSession
+
+
+from . import __version__
+from .lennox_ble import LennoxBle
+from .lennox_errors import lennox_error_get_message_from_code, LennoxErrorCodes
+from .lennox_equipment import lennox_equipment, lennox_equipment_diagnostic
+from .lennox_home import lennox_home
+from .lennox_schedule import lennox_schedule
+from .metrics import Metrics
+from .message_logger import MessageLogger
 from .s30exception import (
     EC_AUTHENTICATE,
     EC_BAD_PARAMETERS,
     EC_COMMS_ERROR,
     EC_EQUIPMENT_DNS,
     EC_HTTP_ERR,
     EC_LOGIN,
@@ -31,36 +59,14 @@
     EC_REQUEST_DATA_HELPER,
     EC_SETMODE_HELPER,
     EC_SUBSCRIBE,
     EC_UNAUTHORIZED,
     S30Exception,
     s30exception_from_comm_exception,
 )
-from .lennox_errors import (
-    lennox_error_get_message_from_code,
-    LennoxErrorCodes,
-)
-from datetime import datetime
-import logging
-import json
-import uuid
-import ssl
-from aiohttp import ClientTimeout, ClientSession
-
-from urllib.parse import quote
-from typing import Final, List
-from .lennox_schedule import lennox_schedule
-from .lennox_home import lennox_home
-from .metrics import Metrics
-from .message_logger import MessageLogger
-from .lennox_equipment import (
-    lennox_equipment,
-    lennox_equipment_diagnostic,
-    lennox_equipment_parameter,
-)
 
 
 _LOGGER = logging.getLogger(__name__)
 
 CLOUD_AUTHENTICATE_URL = "https://ic3messaging.myicomfort.com/v1/mobile/authenticate"
 CLOUD_LOGIN_URL = "https://ic3messaging.myicomfort.com/v2/user/login"
 CLOUD_NEGOTIATE_URL = "https://icnotificationservice.myicomfort.com/LennoxNotificationServer/negotiate"
@@ -186,14 +192,18 @@
 # Parameter range for zoneTestControl
 PID_ZONE_1_BLOWER_CFM = 256
 PID_ZONE_8_HEATING_CFM = 279
 
 # String in lennox JSON representing no value.
 LENNOX_NONE_STR: Final = "none"
 
+# BLE Sensor
+LENNOX_BLE_COMMSTATUS_AVAILABLE: Final = "active"
+LENNOX_BLE_STATUS_INPUT_AVAILABLE: Final = "0"
+
 # NOTE:  This application id is super important and a point of brittleness.  You can find this in the burp logs between the mobile app and the Lennox server.
 # If we start getting reports of missesd message, this is the place to look....
 # Here is what I do know
 #
 #  The application id is unique to the mobile app install, so if you install the app on your iphone and ipad you will have two different ids.
 #  Uninstalling app on ipad and re-installing created the same app_id; which is also referenced as the device_id in some api calls
 #
@@ -234,14 +244,15 @@
         app_id: The unique application id to use to create a message subscription
         ip_address: The ip_address to connect to when using Local Connection.  None if using a Cloud Connection
         protocol: The protocol to use.  Set to http when using the simulator, else should be https
         pii_message_logs: Indicates if personal information should be redacted from the message logs.
         message_debug_logging:  Indicates if messages should be include when debug logging
         message_logging_file:  When specified messages will be logged to this file only.
         """
+        _LOGGER.info("s30api_async init version %s", __version__)
         self._username = username
         self._password = password
         self._protocol = protocol
         self._pii_message_logs = pii_message_logs
         self.message_log = MessageLogger(_LOGGER, message_debug_logging, message_logging_file)
         self.timeout: int = 300 if timeout is None else timeout
         # Generate a unique app id, following the existing formatting
@@ -251,15 +262,15 @@
             appPrefix = APPLICATION_ID[: len(APPLICATION_ID) - len(epoch_time)]
             app_id = appPrefix + epoch_time
             self._applicationid: str = app_id
             _LOGGER.info(f"__init__  generating unique applicationId [{self._applicationid}]")
         else:
             self._applicationid: str = app_id
             _LOGGER.info(f"__init__ using provided applicationId [{self._applicationid}]")
-        if ip_address == None:
+        if ip_address is None:
             self.isLANConnection = False
             self.ssl = True
             self.initialize_urls_cloud()
         else:
             self.ip = ip_address
             self.isLANConnection = True
             # The certificate on the S30 cannot be validated.  It is self issued by Lennox
@@ -275,14 +286,19 @@
         self._session: ClientSession = None
         self.metrics: Metrics = Metrics()
         self.loginBearerToken = None
         self.authBearerToken = None
         self._homeList: List[lennox_home] = []
         self.system_list: List["lennox_system"] = []
         self._badSenderDict: dict = {}
+        self.loginToken: str = None
+        self._connectionId = None
+        self._connectionToken: str = None
+        self._tryWebsockets = None
+        self._streamURL: str = None
 
     def initialize_urls_cloud(self):
         self.url_authenticate: str = CLOUD_AUTHENTICATE_URL
         self.url_login: str = CLOUD_LOGIN_URL
         self.url_negotiate: str = CLOUD_NEGOTIATE_URL
         self.url_retrieve: str = CLOUD_RETRIEVE_URL
         self.url_requestdata: str = CLOUD_REQUESTDATA_URL
@@ -303,21 +319,21 @@
         self.url_negotiate: str = None
         self.url_retrieve: str = self.set_url_protocol(f"https://{self.ip}/Messages/{self._applicationid}/Retrieve")
         self.url_requestdata: str = self.set_url_protocol(f"https://{self.ip}/Messages/RequestData")
         self.url_publish: str = self.set_url_protocol(f"https://{self.ip}/Messages/Publish")
         self.url_logout: str = self.set_url_protocol(f"https://{self.ip}/Endpoints/{self._applicationid}/Disconnect")
 
     def getClientId(self) -> str:
-        if self.isLANConnection == True:
+        if self.isLANConnection is True:
             return self._applicationid
         # Cloud appends email address for uniqueness
         return self._applicationid + "_" + self._username
 
     async def shutdown(self) -> None:
-        if self.isLANConnection == True or self.loginBearerToken != None:
+        if self.isLANConnection is True or self.loginBearerToken is not None:
             await self.logout()
         await self._close_session()
 
     async def logout(self) -> None:
         _LOGGER.info(f"logout - Entering - [{self.url_logout}]")
         url: str = self.url_logout
         headers = {
@@ -331,54 +347,55 @@
         try:
             resp = await self.post(url, headers=headers, data=None)
             if resp.status != 200 and resp.status != 204:
                 errmsg = f"logout failed response code [{resp.status}] url [{url}]"
                 _LOGGER.error(errmsg)
                 raise S30Exception(errmsg, EC_LOGOUT, 1)
         except S30Exception as e:
-            raise e
+            raise e from e
         except Exception as e:
             s30e = s30exception_from_comm_exception(e, operation="logout", url=url, metrics=self.metrics)
-            if s30e != None:
-                raise s30e
-            _LOGGER.exception("logout exception - please raise as issue")
-            raise S30Exception("logout failed", EC_AUTHENTICATE, 2)
+            if s30e is not None:
+                raise s30e from e
+            _LOGGER.exception("logout exception - please raise an issue")
+            raise S30Exception(f"logout failed [{e}]", EC_AUTHENTICATE, 2) from e
 
     async def _close_session(self) -> None:
         _LOGGER.debug("Closing Session")
-        if self._session != None:
+        if self._session is not None:
             try:
                 await self._session.close()
                 self._session = None
             except Exception as e:
-                _LOGGER.exception("serverConnect - failed to close session")
+                _LOGGER.exception("_close_session - failed to close session [%s]", str(e))
+                self._session = None
 
     def _create_session(self) -> None:
         _LOGGER.debug("Creating Session")
         to = ClientTimeout(total=self.timeout)
         self._session = ClientSession(timeout=to)
 
     async def serverConnect(self) -> None:
         # On a reconnect we will close down the old session and get a new one
-        _LOGGER.debug("serverLogin - Entering")
+        _LOGGER.debug("serverConnect - Entering")
         await self._close_session()
         self._create_session()
         await self.authenticate()
         await self.login()
         await self.negotiate()
         self.metrics.last_reconnect_time = self.metrics.now()
-        _LOGGER.debug("serverLogin - Complete")
+        _LOGGER.debug("serverConnect - Complete")
 
     AUTHENTICATE_RETRIES: int = 5
 
     async def authenticate(self) -> None:
         """Authenticate with Lennox Server by presenting a certificate.  Throws S30Exception on failure"""
         # The only reason this function would fail is if the certificate is no longer valid or the URL is not longer valid.
         _LOGGER.debug("authenticate - Enter")
-        if self.isLANConnection == True:
+        if self.isLANConnection is True:
             return
         url = self.url_authenticate
         body = CERTIFICATE
         err_msg: str = None
         try:
             # I did see this fail due to an active directory error on Lennox side.  I saw the same failure in the Burp log for the App and saw that it repeatedly retried
             # until success, so this must be a known / re-occuring issue that they have solved via retries.  When this occurred the call hung for a while, hence there
@@ -401,50 +418,50 @@
         except S30Exception as e:
             raise e
         except KeyError as e:
             raise S30Exception(
                 f"authenticate failed - unexpected response - unable to find [{e}] in msg [{resp_json}]",
                 EC_AUTHENTICATE,
                 2,
-            )
+            ) from e
         except Exception as e:
             s30e = s30exception_from_comm_exception(e, operation="authenticate", url=url, metrics=self.metrics)
-            if s30e != None:
-                raise s30e
-            _LOGGER.exception("authenticate exception - please raise as issue ")
-            raise S30Exception("authenticate failed", EC_AUTHENTICATE, 2)
+            if s30e is not None:
+                raise s30e from e
+            _LOGGER.exception("authenticate exception - please raise as issue")
+            raise S30Exception("authenticate failed", EC_AUTHENTICATE, 2) from e
 
     def getHomeByHomeId(self, homeId) -> lennox_home:
         for home in self._homeList:
             if str(home.id) == str(homeId):
                 return home
         return None
 
     def getOrCreateHome(self, homeId) -> lennox_home:
         home = self.getHomeByHomeId(homeId)
-        if home != None:
+        if home is not None:
             return home
         home = lennox_home(homeId)
         self._homeList.append(home)
         return home
 
-    def getHomeByIdx(self, id) -> lennox_home:
+    def getHomeByIdx(self, home_id: int) -> lennox_home:
         for home in self._homeList:
-            if str(home.idx) == str(id):
+            if str(home.idx) == str(home_id):
                 return home
         return None
 
     def getHomes(self) -> List[lennox_home]:
         return self._homeList
 
     async def post(self, url, headers=None, data=None):
         # LAN Connections do not send headers
         if self.isLANConnection:
             headers = None
-        if data != None:
+        if data is not None:
             self.metrics.inc_send_count(len(data))
         resp = await self._session.post(url, headers=headers, data=data, ssl=self.ssl)
         self.metrics.inc_receive_count()
         self.metrics.process_http_code(resp.status)
         return resp
 
     async def get(self, url, headers=None, params=None):
@@ -457,15 +474,15 @@
         return resp
 
     async def login(self) -> None:
         """Login to Lennox Server using provided email and password.  Throws S30Exception on failure"""
         _LOGGER.debug("login - Enter")
         url: str = self.url_login
         try:
-            if self.isLANConnection == True:
+            if self.isLANConnection is True:
                 resp = await self.post(url)
                 if resp.status != 200 and resp.status != 204:
                     raise S30Exception(
                         f"login local connection failed url [{url}] response code [{resp.status}]",
                         EC_LOGIN,
                         2,
                     )
@@ -484,15 +501,14 @@
                     "Authorization": self.authBearerToken,
                     "Content-Type": "text/plain",
                     "User-Agent": USER_AGENT,
                 }
                 resp = await self.post(url, headers=headers, data=body)
                 if resp.status != 200:
                     txt = await resp.text()
-                    errmsg = f"login failed response code [{resp.status}] text [{txt}]"
                     raise S30Exception(
                         f"login failed response code [{resp.status}] url [{url}] text [{txt}]",
                         EC_LOGIN,
                         1,
                     )
                 resp_json = await resp.json()
                 self.message_logger(resp_json)
@@ -501,27 +517,27 @@
             _LOGGER.error(e.message)
             raise e
         except json.JSONDecodeError as e:
             raise S30Exception(
                 f"login - JSONDecodeError unable to decode json response [{e}]",
                 EC_LOGIN,
                 3,
-            )
+            ) from e
         except KeyError as e:
             raise S30Exception(
                 f"login failed - unexpected response - unable to find [{e}] in msg [{resp_json}]",
                 EC_LOGIN,
                 2,
-            )
+            ) from e
         except Exception as e:
             s30e = s30exception_from_comm_exception(e, operation="login", url=url, metrics=self.metrics)
-            if s30e != None:
-                raise s30e
+            if s30e is not None:
+                raise s30e from e
             _LOGGER.exception(f"login - unexpected exception - please raise an issue to track [{e}]")
-            raise S30Exception(f"login failed due to unexpected exception [{e}]", EC_LOGIN, 7)
+            raise S30Exception(f"login failed due to unexpected exception [{e}]", EC_LOGIN, 7) from e
         _LOGGER.info(f"login Success homes [{len(self._homeList)}] systems [{len(self.system_list)}]")
 
     def process_login_response(self, resp_json: json):
         # Grab the bearer token
         self.loginBearerToken = resp_json["ServerAssignedRoot"]["serverAssigned"]["security"]["userToken"]["encoded"]
         # Split off the "bearer" part of the token, as we need to use just the token part later in the URL.  Format is "Bearer <token>"
         split = self.loginBearerToken.split(" ")
@@ -542,15 +558,15 @@
         lhome.update("0", "local", "")
         lsystem = self.getOrCreateSystem("LCC")
         lsystem.update(self, lhome, 0)
 
     async def negotiate(self) -> None:
         _LOGGER.debug("Negotiate - Enter")
         try:
-            if self.isLANConnection == True:
+            if self.isLANConnection is True:
                 return
             url = self.url_negotiate
             # This sets the version of the client protocol, at some point Lenox could obsolete this version
             url += "?clientProtocol=1.3.0.0"
             # Since these may have special characters, they need to be URI encoded
             url += "&clientId=" + quote(self.getClientId())
             url += "&Authorization=" + quote(self.loginToken)
@@ -575,27 +591,26 @@
         except S30Exception as e:
             raise e
         except KeyError as e:
             raise S30Exception(
                 f"negotiate failed - unexpected response - unable to find [{e}] in msg [{resp_json}]",
                 EC_NEGOTIATE,
                 2,
-            )
+            ) from e
         except Exception as e:
             s30e = s30exception_from_comm_exception(e, operation="negotiate", url=url, metrics=self.metrics)
-            if s30e != None:
-                raise s30e
+            if s30e is not None:
+                raise s30e from e
             _LOGGER.exception("negotiate - unexpected exception - please raise an issue to track")
-            raise S30Exception("negotiate failed due to unexpected exception", EC_COMMS_ERROR, 7)
+            raise S30Exception("negotiate failed due to unexpected exception", EC_COMMS_ERROR, 7) from e
 
     # The topics subscribed to here are based on the topics that the WebApp subscribes to.  We likely don't need to subscribe to all of them
     # These appear to be JSON topics that correspond to the returned JSON.  For now we will do what the web app does.
     async def subscribe(self, lennoxSystem: "lennox_system") -> None:
-
-        if self.isLANConnection == True:
+        if self.isLANConnection is True:
             ref: int = 1
             try:
                 await self.requestDataHelper(
                     lennoxSystem.sysId,
                     '"AdditionalParameters":{"JSONPath":"1;/systemControl;/systemController;/reminderSensors;/reminders;/alerts/active;/alerts/meta;/bleProvisionDB;/ble;/indoorAirQuality;/fwm;/rgw;/devices;/zones;/equipments;/schedules;/occupancy;/system"}',
                 )
                 ref = 2
@@ -603,19 +618,19 @@
                     lennoxSystem.sysId,
                     '"AdditionalParameters":{"JSONPath":"1;/automatedTest;/zoneTestControl;/homes;/reminders;/algorithm;/historyReportFileDetails;/interfaces;/logs"}',
                 )
 
             except S30Exception as e:
                 err_msg = f"subscribe fail loca [{ref}] sysId [{lennoxSystem.sysId}] {e.as_string()}"
                 _LOGGER.error(err_msg)
-                raise e
+                raise e from e
             except Exception as e:
                 err_msg = f"subscribe fail locb [{ref}] sysId [{lennoxSystem.sysId}] [{e}] "
                 _LOGGER.exception(err_msg)
-                raise S30Exception(err_msg, EC_SUBSCRIBE, 3)
+                raise S30Exception(err_msg, EC_SUBSCRIBE, 3) from e
 
         else:
             ref: int = 1
             try:
                 await lennoxSystem.update_system_online_cloud()
                 ref = 2
                 await self.requestDataHelper(
@@ -630,20 +645,20 @@
             except S30Exception as e:
                 err_msg = f"subscribe fail locc [{ref}] sysId [{lennoxSystem.sysId}] {e.as_string()}"
                 _LOGGER.error(err_msg)
                 raise e
             except Exception as e:
                 err_msg = f"subscribe fail locd [{ref}] sysId [{lennoxSystem.sysId}] [{e}]"
                 _LOGGER.exception(err_msg)
-                raise S30Exception(err_msg, EC_SUBSCRIBE, 3)
+                raise S30Exception(err_msg, EC_SUBSCRIBE, 3) from e
 
     async def messagePump(self) -> None:
         # This method reads off the queue.
         # Observations:  the clientId is not passed in, they must be mapping the token to the clientId as part of negotiate
-        # TODO: The long polling is not working for cloud connections, I have tried adjusting the long polling delay.  Long polling seems to work from the IOS App, not sure
+        # The long polling is not working for cloud connections, I have tried adjusting the long polling delay.  Long polling seems to work from the IOS App, not sure
         # what the difference is.   https://gist.github.com/rcarmo/3f0772f2cbe0612b699dcbb839edabeb
         # Returns True if messages were received, False if no messages were found, and throws S30Exception for errors
         #        _LOGGER.debug("Request Data - Enter")
         try:
             url = self.url_retrieve
             headers = {
                 "Authorization": self.loginBearerToken,
@@ -686,33 +701,33 @@
             return True
         except S30Exception as e:
             self.metrics.inc_receive_message_error()
             raise e
         except Exception as e:
             self.metrics.inc_receive_message_error()
             s30e = s30exception_from_comm_exception(e, operation="messagePump", url=url, metrics=self.metrics)
-            if s30e != None:
-                raise s30e
+            if s30e is not None:
+                raise s30e from e
             # should not be here, these are unexpected exceptions that should be handled better
             _LOGGER.exception("messagePump - unexpected exception - please raise an issue to track")
-            raise S30Exception("messagePump failed due to unexpected exception", EC_COMMS_ERROR, 7)
+            raise S30Exception("messagePump failed due to unexpected exception", EC_COMMS_ERROR, 7) from e
 
     def processMessage(self, message):
         self.metrics.inc_message_count()
         # LAN message and cloud message uses different capitalization.
         if "SenderID" in message:
             sysId = message["SenderID"]
         else:
             sysId = message["SenderId"]
         system = self.getSystem(sysId)
-        if system != None:
+        if system is not None:
             system.processMessage(message)
         else:
             system: lennox_system = self.getSystemSibling(sysId)
-            if system == None:
+            if system is None:
                 self.metrics.inc_sender_message_drop()
                 if sysId in self._badSenderDict:
                     _LOGGER.debug(f"processMessage dropping messages from unknown SenderId/SystemId [{sysId}]")
                 else:
                     _LOGGER.error(
                         f"processMessage dropping message from unknown SenderId/SystemId [{sysId}] - please consult https://github.com/PeteRager/lennoxs30/blob/master/docs/sibling.md for configuration assistance"
                     )
@@ -752,15 +767,15 @@
             body += "}"
 
             jsbody = json.loads(body)
             self.message_logger(jsbody)
             resp = await self.post(url, headers=headers, data=body)
             if resp.status == 200:
                 # TODO we should be inspecting the return body?
-                if self.isLANConnection == True:
+                if self.isLANConnection is True:
                     txt = await resp.text()
                     _LOGGER.debug(txt)
                     return txt
                 else:
                     txt = await resp.json()
                     self.message_logger(txt)
                     return txt
@@ -772,25 +787,25 @@
         except S30Exception as e:
             raise e
         except json.JSONDecodeError as e:
             raise S30Exception(
                 f"requestDataHelper failed - JSONDecodeError [{e}] in msg",
                 EC_REQUEST_DATA_HELPER,
                 3,
-            )
+            ) from e
         except Exception as e:
             s30e = s30exception_from_comm_exception(e, operation="requestDataHelper", url=url, metrics=self.metrics)
-            if s30e != None:
-                raise s30e
+            if s30e is not None:
+                raise s30e from e
             _LOGGER.exception("requestDataHelper - unexpected exception - please raise an issue to track")
             raise S30Exception(
                 "requestDataHelper failed due to unexpected exception",
                 EC_COMMS_ERROR,
                 7,
-            )
+            ) from e
 
     def getSystem(self, sysId) -> "lennox_system":
         for system in self.system_list:
             if system.sysId == sysId:
                 return system
         return None
 
@@ -798,15 +813,15 @@
         for system in self.system_list:
             if system.sibling_identifier == sysId:
                 return system
         return None
 
     def getOrCreateSystem(self, sysId: str) -> "lennox_system":
         system = self.getSystem(sysId)
-        if system != None:
+        if system is not None:
             return system
         system = lennox_system(sysId)
         self.system_list.append(system)
         return system
 
     # When publishing data, app uses a GUID that counts up from 1.
     def getNextMessageId(self):
@@ -834,15 +849,15 @@
             _LOGGER.debug("setmode message [" + data + "]")
             await self.publishMessageHelper(sysId, data)
         except S30Exception as e:
             _LOGGER.error(f"setmode - S30Exception {e.as_string()}")
             raise e
         except Exception as e:
             _LOGGER.exception("setmode - Exception ")
-            raise S30Exception(str(e), EC_SETMODE_HELPER, 1)
+            raise S30Exception(str(e), EC_SETMODE_HELPER, 1) from e
         _LOGGER.info(f"setModeHelper success[{mode}] scheduleId [{scheduleId}] sysId [{sysId}]")
 
     async def publish_message_helper_dict(self, sysId: str, message: dict, additional_parameters=None):
         data = '"Data":' + json.dumps(message)
         await self.publishMessageHelper(sysId, data, additional_parameters=additional_parameters)
 
     async def publishMessageHelper(self, sysId: str, data: str, additional_parameters=None) -> None:
@@ -859,15 +874,15 @@
             }
 
             body = "{"
             body += '"MessageType":"Command",'
             body += '"SenderID":"' + self.getClientId() + '",'
             body += '"MessageID":"' + self.getNextMessageId() + '",'
             body += '"TargetID":"' + sysId + '",'
-            if additional_parameters != None:
+            if additional_parameters is not None:
                 body += '"AdditionalParameters":"' + additional_parameters + '",'
             body += data
             body += "}"
 
             # See if we can parse the JSON, if we can't error will be thrown, no point in sending lennox bad data
             jsbody = json.loads(body)
             self.message_logger(jsbody)
@@ -889,34 +904,34 @@
                     2,
                 )
         except json.JSONDecodeError as e:
             raise S30Exception(
                 f"publishMessageHelper failed - JSONDecodeError [{e}] in msg [{resp_txt}]",
                 EC_PUBLISH_MESSAGE,
                 3,
-            )
+            ) from e
         except KeyError as e:
             raise S30Exception(
                 f"publishMessageHelper failed - unexpected response - unable to find [{e}] in msg [{resp_txt}]",
                 EC_PUBLISH_MESSAGE,
                 4,
-            )
+            ) from e
         except S30Exception as e:
             _LOGGER.error(e.message)
             raise e
         except Exception as e:
             s30e = s30exception_from_comm_exception(e, operation="publishMessageHelper", url=url, metrics=self.metrics)
-            if s30e != None:
-                raise s30e
+            if s30e is not None:
+                raise s30e from e
             _LOGGER.exception("publishMessageHelper - unexpected exception - please raise an issue to track")
             raise S30Exception(
                 "publishMessageHelper failed due to unexpected exception",
                 EC_COMMS_ERROR,
                 5,
-            )
+            ) from e
         _LOGGER.info("publishMessageHelper success sysId [" + str(sysId) + "]")
 
     async def setHVACMode(self, sysId: str, mode: str, scheduleId: int) -> None:
         _LOGGER.info(f"setHVACMode mode [{mode}] scheduleId [{scheduleId}] sysId [{sysId}]")
         if mode not in HVAC_MODES:
             err_msg = f"setHVACMode - invalide mode [{mode}] requested, must be in [{HVAC_MODES}]"
             raise S30Exception(err_msg, EC_BAD_PARAMETERS, 1)
@@ -934,42 +949,44 @@
         if mode not in FAN_MODES:
             err_msg = f"setFanMode - invalide mode [{mode}] requested, must be in [{FAN_MODES}]"
             raise S30Exception(err_msg, EC_BAD_PARAMETERS, 1)
         await self.setModeHelper(sysId, "fanMode", mode, scheduleId)
 
     async def setManualAwayMode(self, sysId: str, mode: bool) -> None:
         _LOGGER.info(f"setManualAwayMode mode [{mode}] sysId [{sysId}]")
-        str = None
-        if mode == True:
-            str = "true"
-        if mode == False:
-            str = "false"
-        if str is None:
+        mode_str = None
+        if mode is True:
+            mode_str = "true"
+        if mode is False:
+            mode_str = "false"
+        if mode_str is None:
             err_msg = f"setManualAwayMode - invalid mode [{mode}] requested, must be True or False"
             raise S30Exception(err_msg, EC_BAD_PARAMETERS, 1)
-        data = '"Data":{"occupancy":{"manualAway":' + str + "}" + "}"
+        data = '"Data":{"occupancy":{"manualAway":' + mode_str + "}" + "}"
         await self.publishMessageHelper(sysId, data)
 
     async def cancel_smart_away(self, sysId: str) -> None:
         _LOGGER.info(f"cancel_smart_away sysId [{sysId}]")
         command = {"occupancy": {"smartAway": {"config": {"cancel": True}}}}
         data = '"Data":' + json.dumps(command).replace(" ", "")
         await self.publishMessageHelper(sysId, data)
 
     async def enable_smart_away(self, sysId: str, mode: bool) -> None:
         _LOGGER.info(f"enable_smart_away mode [{mode}] sysId [{sysId}]")
-        if mode != True and mode != False:
+        if mode is not True and mode is not False:
             err_msg = f"enable_smart_away - invalid mode [{mode}] requested, must be True or False"
             raise S30Exception(err_msg, EC_BAD_PARAMETERS, 1)
         command = {"occupancy": {"smartAway": {"config": {"enabled": mode}}}}
         data = '"Data":' + json.dumps(command).replace(" ", "")
         await self.publishMessageHelper(sysId, data)
 
 
 class lennox_system(object):
+    """Represents a Lennox Control System"""
+
     def __init__(self, sysId: str):
         self.sysId: str = sysId
         self.api: s30api_async = None
         self.idx: int = None
         self.home: lennox_home = None
         self.zone_list: List["lennox_zone"] = []
         self._schedules: List[lennox_schedule] = []
@@ -1065,132 +1082,134 @@
             "occupancy": self._processOccupancy,
             "devices": self._processDevices,
             "equipments": self._processEquipments,
             "systemControl": self._processSystemControl,
             "siblings": self._processSiblings,
             "rgw": self._process_rgw,
             "alerts": self._process_alerts,
+            "ble": self._process_ble,
         }
 
         self.equipment: dict[int, lennox_equipment] = {}
+        self.ble_devices: dict[int, LennoxBle] = {}
         _LOGGER.info(f"Creating lennox_system sysId [{self.sysId}]")
 
     async def update_system_online_cloud(self):
         response = await self.api.requestDataHelper(
             "ic3server",
             '"AdditionalParameters":{"publisherpresence":"true"},"Data":{"presence":[{"id":0,"endpointId":"'
             + self.sysId
             + '"}]}',
         )
-        if response != None:
+        if response is not None:
             message_txt = response.get("message")
-            if message_txt != None:
+            if message_txt is not None:
                 try:
                     message = json.loads(message_txt)
                 except Exception as e:
                     _LOGGER.warning(
-                        f"update_system_online_cloud - Failed to obtain presence status from cloud message [{message}] exception [{e}]"
+                        f"update_system_online_cloud - Failed to obtain presence status from cloud message [{message_txt}] exception [{e}]"
                     )
                     return
                 presence = message.get("presence")
-                if presence != None:
+                if presence is not None:
                     sysId = presence[0].get("endpointId")
                     if sysId != self.sysId:
                         _LOGGER.error(
                             f"update_system_online_cloud - get_system_online_cloud sysId [{self.sysId}] received unexpected sysId [{sysId}]"
                         )
                     else:
                         self.attr_updater(presence[0], "status", "cloud_status")
                         self.executeOnUpdateCallbacks()
                 else:
                     _LOGGER.warning(f"update_system_online_cloud - No presense element in response [{response}]")
             else:
                 _LOGGER.warning(f"update_system_online_cloud - No message element in response [{response}]")
         else:
-            _LOGGER.warning(f"update_system_online_cloud - No Response Received")
+            _LOGGER.warning("update_system_online_cloud - No Response Received")
 
     def update(self, api: s30api_async, home: lennox_home, idx: int):
         self.api = api
         self.idx = idx
         self.home = home
         _LOGGER.info(f"Update lennox_system idx [{self.idx}] sysId [{self.sysId}]")
 
     def processMessage(self, message) -> None:
         try:
             if "Data" in message:
                 # By definition if we receive a message for a cloud connected system, it is online.
-                if self.api.isLANConnection == False:
+                if self.api.isLANConnection is False:
                     self.attr_updater({"status": "online"}, "status", "cloud_status")
                 data = message["Data"]
                 for key in self.message_processing_list:
                     try:
                         if key in data:
                             self.message_processing_list[key](data[key])
-                    except Exception as e:
+                    except Exception:
                         _LOGGER.exception(f"processMessage key [{key}] Exception - Failed Message to Follow")
                         _LOGGER.error(
                             json.dumps(
                                 self.api.message_log.remove_redacted_fields(message),
                                 indent=4,
                             )
                         )
                 _LOGGER.debug(
                     f"processMessage complete system id [{self.sysId}] dirty [{self._dirty}] dirtyList [{self._dirtyList}]"
                 )
                 self.executeOnUpdateCallbacks()
-        except Exception as e:
+        except Exception:
             _LOGGER.exception("processMessage - unexpected exception - Failed Message to Follow")
             _LOGGER.error(json.dumps(self.api.message_log.remove_redacted_fields(message), indent=4))
 
-    def getOrCreateSchedule(self, id):
-        schedule = self.getSchedule(id)
-        if schedule != None:
+    def getOrCreateSchedule(self, schedule_id):
+        schedule = self.getSchedule(schedule_id)
+        if schedule is not None:
             return schedule
-        schedule = lennox_schedule(id)
+        schedule = lennox_schedule(schedule_id)
         self._schedules.append(schedule)
         return schedule
 
-    def getSchedule(self, id):
+    def getSchedule(self, schedule_id):
         for schedule in self._schedules:
-            if schedule.id == id:
+            if schedule.id == schedule_id:
                 return schedule
         return None
 
     def getSchedules(self):
         return self._schedules
 
     def getOrCreateEquipment(self, equipment_id: int) -> lennox_equipment:
         if equipment_id not in self.equipment:
             self.equipment[equipment_id] = lennox_equipment(equipment_id)
         return self.equipment[equipment_id]
 
     def get_indoor_unit_equipment(self) -> lennox_equipment:
-        if self.has_indoor_unit == False:
+        if self.has_indoor_unit is False:
             return None
         eq: lennox_equipment = None
         # Try to match on the type
-        for k, eq in self.equipment.items():
+        for _, eq in self.equipment.items():
             if (
-                eq.equipment_name != None
-                and self.indoorUnitType != None
+                eq.equipment_name is not None
+                and self.indoorUnitType is not None
                 and eq.equipment_type_name.casefold() == self.indoorUnitType.casefold()
             ):
                 return eq
         # Otherwise return Eq 2 as this is typically the indoor unit
         return self.equipment.get(2)
 
     def get_outdoor_unit_equipment(self) -> lennox_equipment:
-        if self.has_outdoor_unit == False:
+        if self.has_outdoor_unit is False:
             return None
         eq: lennox_equipment = None
         # Try to match on the type
-        for k, eq in self.equipment.items():
+        for _, eq in self.equipment.items():
             if (
-                eq.equipment_name != None
-                and self.outdoorUnitType != None
+                eq.equipment_name is not None
+                and self.outdoorUnitType is not None
                 and eq.equipment_type_name.casefold() == self.outdoorUnitType.casefold()
             ):
                 return eq
         # Otherwise return Eq 1 as this is typically the indoor unit
         return self.equipment.get(1)
 
     def _processSystemControl(self, systemControl):
@@ -1219,151 +1238,165 @@
             self.attr_updater(status, "relayServerConnected")
             self.attr_updater(status, "internetStatus")
 
     def _process_alerts(self, alerts):
         if "active" in alerts:
             self.active_alerts = []
             for alert in alerts["active"]:
-                if (alert1 := alert.get("alert", None)) != None:
+                if (alert1 := alert.get("alert", None)) is not None:
                     t_alert = alert1.copy()
                     # A code of zero indicates a non-alert, lennox seems to put one of these in by default.
-                    if (code := t_alert.get("code", None)) != None and code != 0:
+                    if (code := t_alert.get("code", None)) is not None and code != 0:
                         t_alert["message"] = lennox_error_get_message_from_code(code)
                         if code == LennoxErrorCodes.lx_alarm_id_Low_Ambient_HP_Heat_Lockout.value:
                             self.attr_updater(t_alert, "isStillActive", "heatpump_low_ambient_lockout")
                         elif code == LennoxErrorCodes.lx_alarm_id_High_Ambient_Auxiliary_Heat_Lockout.value:
                             self.attr_updater(
                                 t_alert,
                                 "isStillActive",
                                 "aux_heat_high_ambient_lockout",
                             )
-                        if t_alert.get("isStillActive", True) != False:
+                        if t_alert.get("isStillActive", True) is not False:
                             self.active_alerts.append(t_alert)
             self._dirty = True
             self._dirtyList.append("active_alerts")
         if "meta" in alerts:
             meta = alerts["meta"]
             self.attr_updater(meta, "numClearedAlerts", "alerts_num_cleared")
             self.attr_updater(meta, "numActiveAlerts", "alerts_num_active")
             self.attr_updater(meta, "lastClearedAlertId", "alerts_last_cleared_id")
             self.attr_updater(meta, "numAlertsInActiveArray", "alerts_num_in_active_array")
             if "numAlertsInActiveArray" in meta and self.alerts_num_in_active_array == 0:
                 self.active_alerts = []
                 self._dirty = True
                 self._dirtyList.append("active_alerts")
 
+    def get_or_create_ble_device(self, ble_id: int) -> LennoxBle:
+        if ble_id not in self.ble_devices:
+            self.ble_devices[ble_id] = LennoxBle(ble_id)
+        return self.ble_devices[ble_id]
+
+    def _process_ble(self, ble):
+        for devices in ble.get("devices", {}):
+            if "device" in devices:
+                device = devices["device"]
+                if "wdn" in device and device["wdn"] != 0:
+                    ble_device = self.get_or_create_ble_device(device["wdn"])
+                    ble_device.update_from_json(device)
+                    ble_device.execute_on_update_callbacks()
+
     def _processSchedules(self, schedules):
         """Processes the schedule messages, throws base exceptions if a problem is encoutered"""
         for schedule in schedules:
             self._dirty = True
-            if "schedules" in self._dirtyList == False:
+            if "schedules" in self._dirtyList is False:
                 self._dirtyList.append("schedules")
-            id = schedule["id"]
+            schedule_id = schedule["id"]
             if "schedule" in schedule:
-                lschedule = self.getSchedule(id)
+                lschedule = self.getSchedule(schedule_id)
                 if lschedule is None and "name" in schedule["schedule"]:
-                    lschedule = self.getOrCreateSchedule(id)
-                if lschedule != None:
+                    lschedule = self.getOrCreateSchedule(schedule_id)
+                if lschedule is not None:
                     lschedule.update(schedule)
                     # In manual mode, the updates only hit the schedulde rather than the period within the status.
                     # So here, we look for changes to these schedules and route them to the zone but only
                     # if it is in manual mode.
                     if schedule["id"] in (
                         16,
                         17,
                         18,
                         19,
                     ):  # Manual Mode Zones 1 .. 4
-                        zone_id = id - LENNOX_MANUAL_MODE_SCHEDULE_START_INDEX
+                        zone_id = schedule_id - LENNOX_MANUAL_MODE_SCHEDULE_START_INDEX
                         period = schedule["schedule"]["periods"][0]["period"]
                         zone: lennox_zone = self.getZone(zone_id)
                         if zone.isZoneManualMode():
                             zone._processPeriodMessage(period)
                             zone.executeOnUpdateCallbacks()
 
     def registerOnUpdateCallback(self, callbackfunc, match=None):
         self._callbacks.append({"func": callbackfunc, "match": match})
 
     def executeOnUpdateCallbacks(self):
-        if self._dirty == True:
+        if self._dirty is True:
             for callback in self._callbacks:
                 callbackfunc = callback["func"]
                 match = callback["match"]
                 matches = False
                 if match is None:
                     matches = True
                 else:
                     for m in match:
                         if m in self._dirtyList:
                             matches = True
                             break
                 try:
-                    if matches == True:
+                    if matches is True:
                         callbackfunc()
-                except Exception as e:
+                except Exception:
                     # Log and eat this exception so we can process other callbacks
                     _LOGGER.exception("executeOnUpdateCallback - failed ")
         self._dirty = False
         self._dirtyList = []
 
     def registerOnUpdateCallbackEqParameters(self, callbackfunc, match=None):
         # match is f'{eid}_{pid}'
         self._eqParametersCallbacks.append({"func": callbackfunc, "match": match})
 
-    def executeOnUpdateCallbacksEqParameters(self, id):
+    def executeOnUpdateCallbacksEqParameters(self, pid):
         for callback in self._eqParametersCallbacks:
             callbackfunc = callback["func"]
             match = callback["match"]
             matches = False
             if match is None:
                 matches = True
             else:
                 for m in match:
-                    if m == id:
+                    if m == pid:
                         matches = True
                         break
             try:
-                if matches == True:
+                if matches is True:
                     # Adding ID to the callback, since you can pass in an array
                     # of IDs to register for the callback, the callback needs to
                     # know which id the value belongs to.
-                    callbackfunc(id)
-            except Exception as e:
+                    callbackfunc(pid)
+            except Exception:
                 # Log and eat this exception so we can process other callbacks
                 _LOGGER.exception("executeOnUpdateCallbacksEqParameters - failed ")
 
     def registerOnUpdateCallbackDiag(self, callbackfunc, match=None):
         # match is f'{eid}_{did}'
         self._diagcallbacks.append({"func": callbackfunc, "match": match})
 
-    def executeOnUpdateCallbacksDiag(self, id, newval):
+    def executeOnUpdateCallbacksDiag(self, diag_id, newval):
         for callback in self._diagcallbacks:
             callbackfunc = callback["func"]
             match = callback["match"]
             matches = False
             if match is None:
                 matches = True
             else:
                 for m in match:
-                    if m == id:
+                    if m == diag_id:
                         matches = True
                         break
             try:
-                if matches == True:
+                if matches is True:
                     # Adding ID to the callback, since you can pass in an array
                     # of IDs to register for the callback, the callback needs to
                     # know which id the value belongs to.
-                    callbackfunc(id, newval)
-            except Exception as e:
+                    callbackfunc(diag_id, newval)
+            except Exception:
                 # Log and eat this exception so we can process other callbacks
                 _LOGGER.exception("executeOnUpdateCallbacksDiag - failed")
 
-    def attr_updater(self, set, attr: str, propertyName: str = None) -> bool:
-        if attr in set:
-            attr_val = set[attr]
+    def attr_updater(self, input_set, attr: str, propertyName: str = None) -> bool:
+        if attr in input_set:
+            attr_val = input_set[attr]
             if propertyName is None:
                 propertyName = attr
             if getattr(self, propertyName) != attr_val:
                 setattr(self, propertyName, attr_val)
                 self._dirty = True
                 if propertyName not in self._dirtyList:
                     self._dirtyList.append(propertyName)
@@ -1394,33 +1427,33 @@
                 if "ventilation" in options:
                     ventilation = options["ventilation"]
                     self.attr_updater(ventilation, "unitType", "ventilationUnitType")
                     self.attr_updater(ventilation, "controlMode", "ventilationControlMode")
                 if "enhancedDehumidificationOvercoolingF" in options:
                     eoc = options["enhancedDehumidificationOvercoolingF"]
                     if "range" in eoc:
-                        range = eoc["range"]
-                        self.attr_updater(range, "min", "enhancedDehumidificationOvercoolingF_min")
-                        self.attr_updater(range, "max", "enhancedDehumidificationOvercoolingF_max")
-                        self.attr_updater(range, "inc", "enhancedDehumidificationOvercoolingF_inc")
+                        dehumid_range = eoc["range"]
+                        self.attr_updater(dehumid_range, "min", "enhancedDehumidificationOvercoolingF_min")
+                        self.attr_updater(dehumid_range, "max", "enhancedDehumidificationOvercoolingF_max")
+                        self.attr_updater(dehumid_range, "inc", "enhancedDehumidificationOvercoolingF_inc")
                         self.attr_updater(
-                            range,
+                            dehumid_range,
                             "enable",
                             "enhancedDehumidificationOvercoolingF_enable",
                         )
 
                 if "enhancedDehumidificationOvercoolingC" in options:
                     eoc = options["enhancedDehumidificationOvercoolingC"]
                     if "range" in eoc:
-                        range = eoc["range"]
-                        self.attr_updater(range, "min", "enhancedDehumidificationOvercoolingC_min")
-                        self.attr_updater(range, "max", "enhancedDehumidificationOvercoolingC_max")
-                        self.attr_updater(range, "inc", "enhancedDehumidificationOvercoolingC_inc")
+                        dehumid_range = eoc["range"]
+                        self.attr_updater(dehumid_range, "min", "enhancedDehumidificationOvercoolingC_min")
+                        self.attr_updater(dehumid_range, "max", "enhancedDehumidificationOvercoolingC_max")
+                        self.attr_updater(dehumid_range, "inc", "enhancedDehumidificationOvercoolingC_inc")
                         self.attr_updater(
-                            range,
+                            dehumid_range,
                             "enable",
                             "enhancedDehumidificationOvercoolingC_enable",
                         )
 
         if "status" in message:
             status = message["status"]
             self.attr_updater(status, "outdoorTemperature")
@@ -1571,67 +1604,67 @@
                 self.attr_updater(smart_away_status, "state", "sa_state")
                 self.attr_updater(smart_away_status, "setpointState", "sa_setpointState")
 
     def get_manual_away_mode(self) -> bool:
         return self.manualAwayMode
 
     def get_smart_away_mode(self) -> bool:
-        if self.sa_enabled == True and (
+        if self.sa_enabled is True and (
             self.sa_setpointState == LENNOX_SA_SETPOINT_STATE_TRANSITION
             or self.sa_setpointState == LENNOX_SA_SETPOINT_STATE_AWAY
         ):
             return True
         return False
 
     def get_away_mode(self) -> bool:
-        if self.get_manual_away_mode() == True or self.get_smart_away_mode() == True:
+        if self.get_manual_away_mode() is True or self.get_smart_away_mode() is True:
             return True
         return False
 
     async def set_manual_away_mode(self, mode: bool) -> None:
         await self.api.setManualAwayMode(self.sysId, mode)
 
     async def cancel_smart_away(self) -> None:
-        if self.sa_enabled != True:
+        if self.sa_enabled is not True:
             raise S30Exception(
                 f"Unable to cancel smart away, system [{self.sysId}] smart away not enabled [{self.sa_enabled}]",
                 EC_BAD_PARAMETERS,
                 1,
             )
         await self.api.cancel_smart_away(self.sysId)
 
     async def enable_smart_away(self, mode: bool) -> None:
         await self.api.enable_smart_away(self.sysId, mode)
 
-    def getZone(self, id):
+    def getZone(self, zone_id):
         for zone in self.zone_list:
-            if zone.id == id:
+            if zone.id == zone_id:
                 return zone
         return None
 
     async def setHVACMode(self, mode, scheduleId):
         return await self.api.setHVACMode(self.sysId, mode, scheduleId)
 
     async def setHumidityMode(self, mode, scheduleId):
         return await self.api.setHumidityMode(self.sysId, mode, scheduleId)
 
     async def setFanMode(self, mode, scheduleId):
         return await self.api.setFanMode(self.sysId, mode, scheduleId)
 
     def convertFtoC(self, tempF: float, noOffset=False) -> float:
         # Lennox allows Celsius to be specified only in 0.5 degree increments
-        if noOffset == False:
+        if noOffset is False:
             float_TempC = (float(tempF) - 32.0) * (5.0 / 9.0)
         else:
             float_TempC = (float(tempF)) * (5.0 / 9.0)
         return self.celsius_round(float_TempC)
 
     def convertCtoF(self, tempC: float, noOffset=False) -> int:
         # Lennox allows Faren to be specified only in 1 degree increments
-        if noOffset == False:
+        if noOffset is False:
             float_TempF = (float(tempC) * (9.0 / 5.0)) + 32.0
         else:
             float_TempF = float(tempC) * (9.0 / 5.0)
         return self.faren_round(float_TempF)
 
     def celsius_round(self, c: float) -> float:
         ### Round to nearest 0.5
@@ -1658,95 +1691,95 @@
         husp=None,
         desp=None,
     ) -> None:
         _LOGGER.debug(
             f"lennox_system:perform_schedule_setpoint  sysid [{self.sysId}] zoneid [{zoneId}] schedule_id [{scheduleId}] hsp [{hsp}] hspC [{hspC}] csp [{csp}] cspC [{cspC}] sp [{sp}] spC [{spC}] single_setpoint_mode [{self.single_setpoint_mode}] husp [{husp}] desp [{desp}]"
         )
         if (
-            hsp == None
-            and hspC == None
-            and csp == None
-            and cspC == None
-            and sp == None
-            and spC == None
-            and husp == None
-            and desp == None
+            hsp is None
+            and hspC is None
+            and csp is None
+            and cspC is None
+            and sp is None
+            and spC is None
+            and husp is None
+            and desp is None
         ):
             raise S30Exception(
                 f"lennox_system:perform_schedule_setpoint  sysid [{self.sysId}] no setpoints provided - must specify one or more setpoints",
                 EC_BAD_PARAMETERS,
                 1,
             )
 
         ### No data validation in this routine, make sure you know what you are setting.
         ### Use the zone.perform_setpoint for error checking
         command = {"schedules": [{"schedule": {"periods": [{"id": 0, "period": {}}]}, "id": scheduleId}]}
 
         period = command["schedules"][0]["schedule"]["periods"][0]["period"]
-        if hsp != None:
+        if hsp is not None:
             period["hsp"] = int(hsp)
-        if cspC != None:
+        if cspC is not None:
             period["cspC"] = float(cspC)
-        if hspC != None:
+        if hspC is not None:
             period["hspC"] = float(hspC)
-        if csp != None:
+        if csp is not None:
             period["csp"] = int(csp)
-        if sp != None:
+        if sp is not None:
             period["sp"] = int(sp)
-        if spC != None:
+        if spC is not None:
             period["spC"] = float(spC)
-        if husp != None:
+        if husp is not None:
             period["husp"] = int(husp)
-        if desp != None:
+        if desp is not None:
             period["desp"] = int(desp)
 
         data = '"Data":' + json.dumps(command).replace(" ", "")
         await self.api.publishMessageHelper(self.sysId, data)
 
-    def getOrCreateZone(self, id):
-        zone = self.getZone(id)
-        if zone != None:
+    def getOrCreateZone(self, zone_id):
+        zone = self.getZone(zone_id)
+        if zone is not None:
             return zone
-        zone = lennox_zone(self, id)
+        zone = lennox_zone(self, zone_id)
         self.zone_list.append(zone)
         return zone
 
     def _processZonesMessage(self, message):
         for zone in message:
-            id = zone["id"]
-            lzone = self.getOrCreateZone(id)
+            zone_id = zone["id"]
+            lzone = self.getOrCreateZone(zone_id)
             lzone.processMessage(zone)
 
     def supports_ventilation(self) -> bool:
-        return self.is_none(self.ventilationUnitType) == False
+        return self.is_none(self.ventilationUnitType) is False
 
     async def ventilation_on(self) -> None:
         _LOGGER.debug(f"ventilation_on sysid [{self.sysId}]")
-        if self.supports_ventilation() == False:
+        if self.supports_ventilation() is False:
             err_msg = f"ventilation_on - attempting to turn ventilation on for non-supported equipment ventilatorUnitType [{self.ventilationUnitType}]"
             raise S30Exception(err_msg, EC_EQUIPMENT_DNS, 1)
         command = {"system": {"config": {"ventilationMode": "on"}}}
         await self.api.publish_message_helper_dict(self.sysId, command)
 
     async def ventilation_off(self) -> None:
         _LOGGER.debug(f"ventilation_off sysid [{self.sysId}] ")
-        if self.supports_ventilation() == False:
+        if self.supports_ventilation() is False:
             err_msg = f"ventilation_off - attempting to turn ventilation off for non-supported equipment ventilatorUnitType [{self.ventilationUnitType}]"
             raise S30Exception(err_msg, EC_EQUIPMENT_DNS, 1)
         command = {"system": {"config": {"ventilationMode": "off"}}}
         await self.api.publish_message_helper_dict(self.sysId, command)
 
     async def ventilation_timed(self, durationSecs: int) -> None:
         _LOGGER.debug(f"ventilation_timed sysid [{self.sysId}] durationSecs [{durationSecs}] ")
         try:
             duration_i = int(durationSecs)
         except ValueError as v:
             err_msg = f"ventilation_timed - invalid duration specified must be a positive integer durationSecs [{durationSecs}] valueError [{v}]"
-            raise S30Exception(err_msg, EC_BAD_PARAMETERS, 1)
-        if self.supports_ventilation() == False:
+            raise S30Exception(err_msg, EC_BAD_PARAMETERS, 1) from v
+        if self.supports_ventilation() is False:
             err_msg = f"ventilation_timed - attempting to set timed ventilation for non-supported equipment ventilatorUnitType [{self.ventilationUnitType}]"
             raise S30Exception(err_msg, EC_EQUIPMENT_DNS, 1)
         if duration_i < 0:
             err_msg = f"ventilation_timed - invalid duration specified must be a positive integer durationSecs [{durationSecs}]"
             raise S30Exception(err_msg, EC_BAD_PARAMETERS, 2)
         command = {"systemController": {"command": f"ventilateNow {duration_i}"}}
         await self.api.publish_message_helper_dict(self.sysId, command)
@@ -1761,46 +1794,46 @@
         data = '"Data":{"system":{"config":{"allergenDefender":false} } }'
         await self.api.publishMessageHelper(self.sysId, data)
 
     async def centralMode_on(self) -> None:
         _LOGGER.debug(f"centralMode_on sysid [{self.sysId}] ")
         if self.numberOfZones == 1:
             raise S30Exception(
-                f"Central Mode is not configurable for a system with only one zone",
+                "Central Mode is not configurable for a system with only one zone",
                 EC_BAD_PARAMETERS,
                 1,
             )
         data = '"Data":{"system":{"config":{"centralMode":true} } }'
         await self.api.publishMessageHelper(self.sysId, data)
 
     async def centralMode_off(self) -> None:
         _LOGGER.debug(f"centralMode_off sysid [{self.sysId}] ")
         if self.numberOfZones == 1:
             raise S30Exception(
-                f"Central Mode is not configurable for a system with only one zone",
+                "Central Mode is not configurable for a system with only one zone",
                 EC_BAD_PARAMETERS,
                 1,
             )
         data = '"Data":{"system":{"config":{"centralMode":false} } }'
         await self.api.publishMessageHelper(self.sysId, data)
 
-    async def set_circulateTime(self, min: int) -> None:
-        _LOGGER.debug(f"set_circulateTime sysid [{self.sysId}] min [{min}]")
+    async def set_circulateTime(self, minutes: int) -> None:
+        _LOGGER.debug(f"set_circulateTime sysid [{self.sysId}] min [{minutes}]")
         try:
-            r_min = int(min)
+            r_min = int(minutes)
         except ValueError as e:
             raise S30Exception(
-                f"Circulate Time [{min}] must be an integer between [{LENNOX_CIRCULATE_TIME_MIN}] and [{LENNOX_CIRCULATE_TIME_MAX}]",
+                f"Circulate Time [{minutes}] must be an integer between [{LENNOX_CIRCULATE_TIME_MIN}] and [{LENNOX_CIRCULATE_TIME_MAX}]",
                 EC_BAD_PARAMETERS,
                 1,
-            )
+            ) from e
 
         if r_min < LENNOX_CIRCULATE_TIME_MIN or r_min > LENNOX_CIRCULATE_TIME_MAX:
             raise S30Exception(
-                f"Circulate Time [{min}] must be between [{LENNOX_CIRCULATE_TIME_MIN}] and [{LENNOX_CIRCULATE_TIME_MAX}]",
+                f"Circulate Time [{minutes}] must be between [{LENNOX_CIRCULATE_TIME_MIN}] and [{LENNOX_CIRCULATE_TIME_MAX}]",
                 EC_BAD_PARAMETERS,
                 2,
             )
         data = '"Data":{"system":{"config":{"circulateTime":' + str(r_min) + " } } }"
         await self.api.publishMessageHelper(self.sysId, data)
 
     def is_none(self, s: str) -> bool:
@@ -1830,52 +1863,52 @@
         if self.is_none(self.dehumidifierType):
             raise S30Exception(
                 f"System does not have a dehumidifier, cannot set enhancedDehumidificationOvercooling r_f [{r_f}] r_c [{r_c}]",
                 EC_EQUIPMENT_DNS,
                 1,
             )
         if (
-            self.enhancedDehumidificationOvercoolingF_enable != True
-            or self.enhancedDehumidificationOvercoolingC_enable != True
+            self.enhancedDehumidificationOvercoolingF_enable is not True
+            or self.enhancedDehumidificationOvercoolingC_enable is not True
         ):
             raise S30Exception(
                 f"System does not allow enhancedDehumidificationOvercooling enhancedDehumidificationOvercoolingF_enable [{self.enhancedDehumidificationOvercoolingF_enable}] enhancedDehumidificationOvercoolingC_enable [{self.enhancedDehumidificationOvercoolingC_enable}]",
                 EC_EQUIPMENT_DNS,
                 2,
             )
-        if r_f == None and r_c == None:
+        if r_f is None and r_c is None:
             raise S30Exception(
-                f"enhancedDehumidificationOvercooling must specifcy r_f, r_c or both",
+                "enhancedDehumidificationOvercooling must specifcy r_f, r_c or both",
                 EC_BAD_PARAMETERS,
                 3,
             )
-        if r_f != None:
+        if r_f is not None:
             try:
                 f = int(r_f)
             except ValueError as e:
                 raise S30Exception(
                     f"enhancedDehumidificationOvercooling r_f [{r_f}] must be an integer",
                     EC_BAD_PARAMETERS,
                     4,
-                )
+                ) from e
             if f < self.enhancedDehumidificationOvercoolingF_min or f > self.enhancedDehumidificationOvercoolingF_max:
                 raise S30Exception(
                     f"enhancedDehumidificationOvercooling r_f [{r_f}] must be an integer between [{self.enhancedDehumidificationOvercoolingF_min}] and [{self.enhancedDehumidificationOvercoolingF_max}]",
                     EC_BAD_PARAMETERS,
                     5,
                 )
-        if r_c != None:
+        if r_c is not None:
             try:
                 c = float(r_c)
             except ValueError as e:
                 raise S30Exception(
                     f"enhancedDehumidificationOvercooling r_f [{r_c}] must be an float",
                     EC_BAD_PARAMETERS,
                     6,
-                )
+                ) from e
             if c < self.enhancedDehumidificationOvercoolingC_min or c > self.enhancedDehumidificationOvercoolingC_max:
                 raise S30Exception(
                     f"enhancedDehumidificationOvercooling r_c [{r_c}] must be an floating point between [{self.enhancedDehumidificationOvercoolingC_min}] and [{self.enhancedDehumidificationOvercoolingC_max}]",
                     EC_BAD_PARAMETERS,
                     7,
                 )
 
@@ -1944,15 +1977,15 @@
         if parameter is None:
             raise S30Exception(
                 f"set_equipment_parameter_value cannot find parameter with equipment_id [{equipment_id}] pid [{pid}] value [{value}]",
                 EC_BAD_PARAMETERS,
                 2,
             )
 
-        if parameter.enabled != True:
+        if parameter.enabled is not True:
             raise S30Exception(
                 f"set_equipment_parameter_value cannot set disabled parameter equipment_id [{equipment_id}] pid [{pid}] value [{value}]",
                 EC_BAD_PARAMETERS,
                 3,
             )
 
         call_value = parameter.validate_and_translate(value)
@@ -1996,39 +2029,41 @@
         if parameter is None:
             raise S30Exception(
                 f"set_zone_test_parameter_value cannot find parameter with equipment_id 0 pid [{pid}] value [{value}]",
                 EC_BAD_PARAMETERS,
                 3,
             )
 
-        if parameter.enabled != True:
+        if parameter.enabled is not True:
             raise S30Exception(
                 f"set_zone_test_parameter_value cannot set disabled parameter equipment_id 0 pid [{pid}] value [{value}]",
                 EC_BAD_PARAMETERS,
                 4,
             )
 
         call_value = parameter.validate_and_translate(value)
         await self._internal_set_zone_test_parameter_value(pid, call_value, enabled)
 
     @property
     def has_indoor_unit(self) -> bool:
-        if self.indoorUnitType != None and self.indoorUnitType != LENNOX_NONE_STR:
+        if self.indoorUnitType is not None and self.indoorUnitType != LENNOX_NONE_STR:
             return True
         return False
 
     @property
     def has_outdoor_unit(self) -> bool:
-        if self.outdoorUnitType != None and self.outdoorUnitType != LENNOX_NONE_STR:
+        if self.outdoorUnitType is not None and self.outdoorUnitType != LENNOX_NONE_STR:
             return True
         return False
 
 
 class lennox_zone(object):
-    def __init__(self, system, id):
+    """Represents a lennox zone"""
+
+    def __init__(self, system, zone_id):
         self._callbacks = []
 
         self.temperature = None
         self.temperatureC = None
         self.temperatureStatus = None
         self.humidity = None
         self.humidityStatus = None
@@ -2089,15 +2124,15 @@
         self.desp = None  # Dehumidify Setpoint %
         self.sp = None  # Perfect Mode Setpoint F
         self.spC = None  # Perfect Mode Setpoint C
         self.husp = None  # Humidity Setpoint
         self.startTime = None
         self.overrideActive = None
 
-        self.id: int = id
+        self.id: int = zone_id
         self.name: str = None
         self.system: lennox_system = system
         self._dirty = False
         self._dirtyList = []
 
         _LOGGER.info(f"Creating lennox_zone id [{self.id}]")
 
@@ -2105,38 +2140,38 @@
     def unique_id(self) -> str:
         return (self.system.unique_id + "_" + str(self.id)).replace("-", "") + "_T"
 
     def registerOnUpdateCallback(self, callbackfunc, match=None):
         self._callbacks.append({"func": callbackfunc, "match": match})
 
     def executeOnUpdateCallbacks(self):
-        if self._dirty == True:
+        if self._dirty is True:
             for callback in self._callbacks:
                 callbackfunc = callback["func"]
                 match = callback["match"]
                 matches = False
                 if match is None:
                     matches = True
                 else:
                     for m in match:
                         if m in self._dirtyList:
                             matches = True
                             break
                 try:
-                    if matches == True:
+                    if matches is True:
                         callbackfunc()
-                except Exception as e:
+                except Exception:
                     # Log and eat this exception so we can process other callbacks
                     _LOGGER.exception("executeOnUpdateCallback - failed")
         self._dirty = False
         self._dirtyList = []
 
-    def attr_updater(self, set, attr: str) -> bool:
-        if attr in set:
-            attr_val = set[attr]
+    def attr_updater(self, input_set, attr: str) -> bool:
+        if attr in input_set:
+            attr_val = input_set[attr]
             if getattr(self, attr) != attr_val:
                 setattr(self, attr, attr_val)
                 self._dirty = True
                 if attr not in self._dirtyList:
                     self._dirtyList.append(attr)
                 _LOGGER.debug(f"update_attr: zone Id [{self.id}] attr [{attr}] value [{attr_val}]")
                 return True
@@ -2174,15 +2209,15 @@
             self.attr_updater(config, "scheduleId")
             self.attr_updater(config, "scheduleHold")
             if "scheduleHold" in config:
                 scheduleHold = config["scheduleHold"]
                 found = False
                 if "scheduleId" in scheduleHold:
                     if scheduleHold["scheduleId"] == self.getOverrideScheduleId():
-                        if scheduleHold["enabled"] == True:
+                        if scheduleHold["enabled"] is True:
                             self.overrideActive = True
                             found = True
                 if found is False:
                     self.overrideActive = False
                 self._dirty = True
                 self._dirtyList.append("scheduleHold")
 
@@ -2229,15 +2264,15 @@
         self.attr_updater(period, "husp")
         self.attr_updater(period, "startTime")
 
     def getTemperature(self):
         return self.temperature
 
     def is_zone_active(self) -> bool:
-        return self.temperature != None
+        return self.temperature is not None
 
     def getTemperatureC(self):
         return self.temperatureC
 
     def getHumidity(self):
         return self.humidity
 
@@ -2256,15 +2291,15 @@
     def getHeatSP(self):
         return self.hsp
 
     def getTargetTemperatureF(self):
         if self.systemMode == LENNOX_HVAC_OFF:
             return None
         # In single setpoint mode there is only one target.
-        if self.system.single_setpoint_mode == True:
+        if self.system.single_setpoint_mode is True:
             return self.sp
 
         if self.systemMode == LENNOX_HVAC_COOL:
             return self.csp
 
         if self.systemMode == LENNOX_HVAC_HEAT or self.systemMode == LENNOX_HVAC_EMERGENCY_HEAT:
             return self.hsp
@@ -2273,25 +2308,25 @@
             return None
         return None
 
     def getTargetTemperatureC(self):
         if self.systemMode == LENNOX_HVAC_OFF:
             return None
         # In single setpoint mode there is only one target.
-        if self.system.single_setpoint_mode == True:
+        if self.system.single_setpoint_mode is True:
             return self.spC
 
-        if self.heatingOption == True and self.coolingOption == True:
+        if self.heatingOption is True and self.coolingOption is True:
             if self.systemMode == "cool":
                 return self.cspC
             if self.systemMode == "heat":
                 return self.hspC
-        elif self.heatingOption == True:
+        elif self.heatingOption is True:
             return self.hspC
-        elif self.coolingOption == True:
+        elif self.coolingOption is True:
             return self.cspC
         else:
             return None
 
     def getHumidifySetpoint(self):
         return self.husp
 
@@ -2308,109 +2343,108 @@
 
     def isZoneOveride(self) -> bool:
         if self.scheduleId == self.getOverrideScheduleId():
             return True
         return False
 
     def validate_setpoints(self, r_hsp=None, r_hspC=None, r_csp=None, r_cspC=None, r_sp=None, r_spC=None):
-
-        if (r_sp != None or r_spC != None) and self.system.single_setpoint_mode == False:
+        if (r_sp is not None or r_spC is not None) and self.system.single_setpoint_mode is False:
             raise S30Exception(
-                f"validate_setpoints: r_sp or r_spC can only be specified when system is in single setpoint mode",
+                "validate_setpoints: r_sp or r_spC can only be specified when system is in single setpoint mode",
                 EC_BAD_PARAMETERS,
                 2,
             )
 
-        if r_sp == None and r_spC == None and self.system.single_setpoint_mode == True:
+        if r_sp is None and r_spC is None and self.system.single_setpoint_mode is True:
             raise S30Exception(
-                f"validate_setpoints: r_sp or r_spC must be specified when system is in single setpoint mode",
+                "validate_setpoints: r_sp or r_spC must be specified when system is in single setpoint mode",
                 EC_BAD_PARAMETERS,
                 2,
             )
 
         if (
-            r_hsp != None or r_hspC != None or r_csp != None or r_cspC != None
-        ) and self.system.single_setpoint_mode == True:
+            r_hsp is not None or r_hspC is not None or r_csp is not None or r_cspC is not None
+        ) and self.system.single_setpoint_mode is True:
             raise S30Exception(
-                f"validate_setpoints: r_hsp, r_hspC, r_csp and r_cspC must not be specified when system is in single setpoint mode",
+                "validate_setpoints: r_hsp, r_hspC, r_csp and r_cspC must not be specified when system is in single setpoint mode",
                 EC_BAD_PARAMETERS,
                 2,
             )
 
         if (
-            r_hsp == None
-            and r_hspC == None
-            and r_csp == None
-            and r_cspC == None
-            and self.system.single_setpoint_mode == False
+            r_hsp is None
+            and r_hspC is None
+            and r_csp is None
+            and r_cspC is None
+            and self.system.single_setpoint_mode is False
         ):
             raise S30Exception(
-                f"validate_setpoints: r_hsp, r_hspC, r_csp or r_cspC must be specified when system is in single setpoint mode",
+                "validate_setpoints: r_hsp, r_hspC, r_csp or r_cspC must be specified when system is in single setpoint mode",
                 EC_BAD_PARAMETERS,
                 2,
             )
 
-        if r_csp != None and r_csp < self.minCsp:
+        if r_csp is not None and r_csp < self.minCsp:
             raise S30Exception(
                 f"setHeatCoolSPF r_csp [{r_csp}] must be greater than minCsp [{self.minCsp}]",
                 EC_BAD_PARAMETERS,
                 1,
             )
-        if r_csp != None and r_csp > self.maxCsp:
+        if r_csp is not None and r_csp > self.maxCsp:
             raise S30Exception(
                 f"setHeatCoolSPF r_csp [{r_csp}] must be less than maxCsp [{self.maxCsp}]",
                 EC_BAD_PARAMETERS,
                 2,
             )
-        if r_hsp != None and r_hsp < self.minHsp:
+        if r_hsp is not None and r_hsp < self.minHsp:
             raise S30Exception(
                 f"setHeatCoolSPF r_hsp [{r_hsp}] must be greater than minCsp [{self.minHsp}]",
                 EC_BAD_PARAMETERS,
                 3,
             )
-        if r_hsp != None and r_hsp > self.maxHsp:
+        if r_hsp is not None and r_hsp > self.maxHsp:
             raise S30Exception(
                 f"setHeatCoolSPF r_hsp [{r_hsp}] must be less than maxHsp [{self.maxHsp}]",
                 EC_BAD_PARAMETERS,
                 2,
             )
 
-        if r_cspC != None and r_cspC < self.minCspC:
+        if r_cspC is not None and r_cspC < self.minCspC:
             raise S30Exception(
                 f"setHeatCoolSPC r_cspC [{r_cspC}] must be greater than minCspC [{self.minCspC}]",
                 EC_BAD_PARAMETERS,
                 1,
             )
-        if r_cspC != None and r_cspC > self.maxCspC:
+        if r_cspC is not None and r_cspC > self.maxCspC:
             raise S30Exception(
                 f"setHeatCoolSPC r_cspC [{r_cspC}] must be less than maxCspC [{self.maxCspC}]",
                 EC_BAD_PARAMETERS,
                 2,
             )
-        if r_hspC != None and r_hspC < self.minHspC:
+        if r_hspC is not None and r_hspC < self.minHspC:
             raise S30Exception(
                 f"setHeatCoolSPC r_hspC [{r_hspC}] must be greater than minCspC [{self.minHspC}]",
                 EC_BAD_PARAMETERS,
                 3,
             )
-        if r_hspC != None and r_hspC > self.maxHspC:
+        if r_hspC is not None and r_hspC > self.maxHspC:
             raise S30Exception(
                 f"setHeatCoolSPC r_hspC [{r_hspC}] must be less than maxHspC [{self.maxHspC}]",
                 EC_BAD_PARAMETERS,
                 2,
             )
 
-        if r_sp != None and (r_sp > self.maxCsp or r_sp < self.minHsp):
+        if r_sp is not None and (r_sp > self.maxCsp or r_sp < self.minHsp):
             raise S30Exception(
                 f"setHeatCoolSPC r_sp [{r_sp}] must be between [{self.minHsp}] and [{self.maxHsp}]",
                 EC_BAD_PARAMETERS,
                 2,
             )
 
-        if r_spC != None and (r_spC > self.maxCspC or r_spC < self.minHspC):
+        if r_spC is not None and (r_spC > self.maxCspC or r_spC < self.minHspC):
             raise S30Exception(
                 f"setHeatCoolSPC r_spC [{r_spC}] must be between [{self.minHspC}] and [{self.maxHspC}]",
                 EC_BAD_PARAMETERS,
                 2,
             )
 
     async def perform_setpoint(self, r_hsp=None, r_hspC=None, r_csp=None, r_cspC=None, r_sp=None, r_spC=None):
@@ -2427,55 +2461,55 @@
             r_spC=r_spC,
         )
 
         hsp = hspC = csp = cspC = sp = spC = None
 
         # When in this mode, the lennox app always sends hsp,hspC,csp and cspC in the message.  The code fills
         # in the parameters by either converting faren to celsius or by copying the current setpoint value from the zone
-        if self.system.single_setpoint_mode == False:
-            if r_hsp != None:
+        if self.system.single_setpoint_mode is False:
+            if r_hsp is not None:
                 hsp = self.system.faren_round(r_hsp)
             else:
-                if r_hspC != None:
+                if r_hspC is not None:
                     hsp = self.system.convertCtoF(r_hspC)
                 else:
                     hsp = self.hsp
 
-            if r_hspC != None:
+            if r_hspC is not None:
                 hspC = self.system.celsius_round(r_hspC)
             else:
-                if r_hsp != None:
+                if r_hsp is not None:
                     hspC = self.system.convertFtoC(r_hsp)
                 else:
                     hspC = self.hspC
 
-            if r_csp != None:
+            if r_csp is not None:
                 csp = self.system.faren_round(r_csp)
             else:
-                if r_cspC != None:
+                if r_cspC is not None:
                     csp = self.system.convertCtoF(r_cspC)
                 else:
                     csp = self.csp
 
-            if r_cspC != None:
+            if r_cspC is not None:
                 cspC = self.system.celsius_round(r_cspC)
             else:
-                if r_csp != None:
+                if r_csp is not None:
                     cspC = self.system.convertFtoC(r_csp)
                 else:
                     cspC = self.cspC
         else:
-            if r_sp != None:
+            if r_sp is not None:
                 sp = self.system.faren_round(r_sp)
-            elif r_spC != None:
+            elif r_spC is not None:
                 sp = self.system.convertCtoF(r_spC)
 
-            if r_spC != None:
+            if r_spC is not None:
                 spC = self.system.celsius_round(r_spC)
-            elif r_sp != None:
+            elif r_sp is not None:
                 spC = self.system.convertFtoC(r_sp)
 
         await self._execute_setpoints(hsp=hsp, hspC=hspC, csp=csp, cspC=cspC, sp=sp, spC=spC)
 
     async def _execute_setpoints(
         self,
         hsp=None,
@@ -2486,15 +2520,15 @@
         spC=None,
         husp: int = None,
         desp: int = None,
     ):
         info_str = f"zone [{self.id}] hsp [{hsp}] hspC [{hspC}] csp [{csp}] cspC [{cspC}] sp [{sp}] spC [{spC}] husp [{husp}] desp [{desp}]"
         _LOGGER.info(f"_execute_setpoints {info_str}")
         # If the zone is in manual mode, the temperature can just be set.
-        if self.isZoneManualMode() == True:
+        if self.isZoneManualMode() is True:
             _LOGGER.info(f"lennox_zone:_execute_setpoints zone already in manual mode id [{self.id}]")
             await self.system.perform_schedule_setpoint(
                 zoneId=self.id,
                 scheduleId=self.getManualModeScheduleId(),
                 hsp=hsp,
                 hspC=hspC,
                 csp=csp,
@@ -2504,15 +2538,15 @@
                 husp=husp,
                 desp=desp,
             )
             return
 
         # The zone is following a schedule.  So first check if it's already running
         # the override schedule and we can just set the temperature
-        if self.isZoneOveride() == True:
+        if self.isZoneOveride() is True:
             _LOGGER.info(f"lennox_zone:_execute_setpoints zone already in overridemode id [{self.id}]")
             await self.system.perform_schedule_setpoint(
                 zoneId=self.id,
                 scheduleId=self.getOverrideScheduleId(),
                 hsp=hsp,
                 hspC=hspC,
                 csp=csp,
@@ -2583,35 +2617,35 @@
         if r_husp is None and r_desp is None:
             raise S30Exception(
                 f"perform_humidify_setpoint: r_husp or r_desp must be specified - values [{r_husp}] [{r_desp}]",
                 EC_BAD_PARAMETERS,
                 1,
             )
 
-        if r_husp != None:
+        if r_husp is not None:
             husp = int(r_husp)
             if husp > self.maxHumSp or husp < self.minHumSp:
                 raise S30Exception(
                     f"perform_humidify_setpoint: r_husp invalid value [{r_husp}] must be between [{self.minHumSp}] and [{self.maxHumSp}]",
                     EC_BAD_PARAMETERS,
                     2,
                 )
 
-        if r_desp != None:
+        if r_desp is not None:
             desp = int(r_desp)
             if desp > self.maxDehumSp or desp < self.minDehumSp:
                 raise S30Exception(
                     f"perform_humidify_setpoint: r_desp invalid value [{r_desp}] must be between [{self.minDehumSp}] and [{self.maxDehumSp}]",
                     EC_BAD_PARAMETERS,
                     2,
                 )
         await self._execute_setpoints(husp=husp, desp=desp)
 
     async def setScheduleHold(self, hold: bool) -> bool:
-        if hold == True:
+        if hold is True:
             strHold = "true"
         else:
             strHold = "false"
 
         _LOGGER.info("lennox_zone:setScheduleHold zone [" + str(self.id) + "] hold [" + str(strHold) + "]")
         # Add a schedule hold to the zone, for now all hold will expire on next period
         data = '"Data":{"zones":[{"config":{"scheduleHold":'
@@ -2631,26 +2665,26 @@
     async def setSchedule(self, scheduleName: str) -> None:
         scheduleId = None
         for schedule in self.system.getSchedules():
             if schedule.name == scheduleName:
                 scheduleId = schedule.id
                 break
 
-        if scheduleId == None:
+        if scheduleId is None:
             err_msg = f"setSchedule - unknown schedule [{scheduleName}] zone [{self.name}]"
             raise S30Exception(err_msg, EC_NO_SCHEDULE, 1)
 
         await self.system.setSchedule(self.id, scheduleId)
 
     async def setFanMode(self, fan_mode: str) -> None:
-        if self.isZoneManualMode() == True:
+        if self.isZoneManualMode() is True:
             await self.system.setFanMode(fan_mode, self.getManualModeScheduleId())
             return
 
-        if self.isZoneOveride() == False:
+        if self.isZoneOveride() is False:
             data = '"Data":{"schedules":[{"schedule":{"periods":[{"id":0,"period":'
             data += '{"desp":' + str(self.desp) + ","
             data += '"hsp":' + str(self.hsp) + ","
             data += '"cspC":' + str(self.cspC) + ","
             data += '"sp":' + str(self.sp) + ","
             data += '"husp":' + str(self.husp) + ","
             data += '"humidityMode":"' + str(self.humidityMode) + '",'
@@ -2665,75 +2699,75 @@
             await self.system.api.publishMessageHelper(self.system.sysId, data)
             await self.setScheduleHold(True)
         await self.system.setFanMode(fan_mode, self.getOverrideScheduleId())
 
     async def setHVACMode(self, hvac_mode: str) -> None:
         # We want to be careful passing modes to the controller that it does not support.  We don't want to brick the controller.
         if hvac_mode == LENNOX_HVAC_COOL:
-            if self.coolingOption == False:
+            if self.coolingOption is False:
                 raise S30Exception(
                     f"setHvacMode - invalid hvac mode - zone [{self.id}]  does not support [{hvac_mode}]",
                     EC_BAD_PARAMETERS,
                     1,
                 )
         elif hvac_mode == LENNOX_HVAC_HEAT:
-            if self.heatingOption == False:
+            if self.heatingOption is False:
                 raise S30Exception(
                     f"setHvacMode - invalid hvac mode - zone [{self.id}]  does not support [{hvac_mode}]",
                     EC_BAD_PARAMETERS,
                     2,
                 )
         elif hvac_mode == LENNOX_HVAC_HEAT_COOL:
-            if self.heatingOption == False or self.coolingOption == False:
+            if self.heatingOption is False or self.coolingOption is False:
                 raise S30Exception(
                     f"setHvacMode - invalid hvac mode - zone [{self.id}]  does not support [{hvac_mode}]",
                     EC_BAD_PARAMETERS,
                     3,
                 )
         elif hvac_mode == LENNOX_HVAC_EMERGENCY_HEAT:
-            if self.heatingOption == False or self.system.has_emergency_heat() == False:
+            if self.heatingOption is False or self.system.has_emergency_heat() is False:
                 raise S30Exception(
                     f"setHvacMode - invalid hvac mode - zone [{self.id}]  does not support [{hvac_mode}]",
                     EC_BAD_PARAMETERS,
                     4,
                 )
         elif hvac_mode == LENNOX_HVAC_OFF:
             pass
         else:
             raise S30Exception(
                 f"setHvacMode - invalidate hvac mode - zone [{self.id}]  does not recognize [{hvac_mode}]",
                 EC_BAD_PARAMETERS,
                 4,
             )
 
-        if self.isZoneManualMode() == False:
+        if self.isZoneManualMode() is False:
             await self.system.setSchedule(self.id, self.getManualModeScheduleId())
         await self.system.setHVACMode(hvac_mode, self.getManualModeScheduleId())
 
     async def setHumidityMode(self, mode: str) -> None:
         # We want to be careful passing modes to the controller that it does not support.  We don't want to brick the controller.
         if mode == LENNOX_HUMIDITY_MODE_HUMIDIFY:
-            if self.humidificationOption == False:
+            if self.humidificationOption is False:
                 raise S30Exception(
                     f"setHumidityMode - invalid mode - zone [{self.id}]  does not support [{mode}]",
                     EC_BAD_PARAMETERS,
                     1,
                 )
         elif mode == LENNOX_HUMIDITY_MODE_DEHUMIDIFY:
-            if self.dehumidificationOption == False:
+            if self.dehumidificationOption is False:
                 raise S30Exception(
                     f"setHumidityMode - invalid mode - zone [{self.id}]  does not support [{mode}]",
                     EC_BAD_PARAMETERS,
                     2,
                 )
         elif mode == LENNOX_HUMIDITY_MODE_OFF:
             pass
         else:
             raise S30Exception(
                 f"setHumidityMode - invalidate mode - zone [{self.id}]  does not recognize [{mode}]",
                 EC_BAD_PARAMETERS,
                 4,
             )
 
-        if self.isZoneManualMode() == False:
+        if self.isZoneManualMode() is False:
             await self.system.setSchedule(self.id, self.getManualModeScheduleId())
         await self.system.setHumidityMode(mode, self.getManualModeScheduleId())
```

### Comparing `lennoxs30api-0.2.2/lennoxs30api/s30exception.py` & `lennoxs30api-0.2.3/lennoxs30api/s30exception.py`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.2/lennoxs30api.egg-info/PKG-INFO` & `lennoxs30api-0.2.3/lennoxs30api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lennoxs30api
-Version: 0.2.2
+Version: 0.2.3
 Summary: API Wrapper for Lennox S30 Cloud and LAN API
 Home-page: https://github.com/PeteRager/lennoxs30api
 Author: Pete Rage
 Author-email: pete.rager@x.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lennoxs30api-0.2.2/setup.py` & `lennoxs30api-0.2.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lennoxs30api",
-    version="0.2.2",
+    version="0.2.3",
     description="API Wrapper for Lennox S30 Cloud and LAN API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/PeteRager/lennoxs30api",
     author="Pete Rage",
     author_email="pete.rager@x.com",
     license="MIT",
```

