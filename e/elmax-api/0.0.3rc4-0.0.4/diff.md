# Comparing `tmp/elmax_api-0.0.3rc4.tar.gz` & `tmp/elmax_api-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elmax_api-0.0.3rc4.tar", last modified: Sun Dec  4 12:05:59 2022, max compression
+gzip compressed data, was "elmax_api-0.0.4.tar", last modified: Sun Apr 23 18:49:43 2023, max compression
```

## Comparing `elmax_api-0.0.3rc4.tar` & `elmax_api-0.0.4.tar`

### file list

```diff
@@ -1,30 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 12:05:59.269538 elmax_api-0.0.3rc4/
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2022-12-04 12:05:59.269538 elmax_api-0.0.3rc4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2022-12-04 12:05:45.000000 elmax_api-0.0.3rc4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 12:05:59.269538 elmax_api-0.0.3rc4/elmax_api/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2022-12-04 12:05:45.000000 elmax_api-0.0.3rc4/elmax_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2022-12-04 12:05:45.000000 elmax_api-0.0.3rc4/elmax_api/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2022-12-04 12:05:45.000000 elmax_api-0.0.3rc4/elmax_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    22309 2022-12-04 12:05:45.000000 elmax_api-0.0.3rc4/elmax_api/http.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 12:05:59.269538 elmax_api-0.0.3rc4/elmax_api/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-04 12:05:45.000000 elmax_api-0.0.3rc4/elmax_api/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2022-12-04 12:05:45.000000 elmax_api-0.0.3rc4/elmax_api/model/actuator.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2022-12-04 12:05:45.000000 elmax_api-0.0.3rc4/elmax_api/model/alarm_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2022-12-04 12:05:45.000000 elmax_api-0.0.3rc4/elmax_api/model/area.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2022-12-04 12:05:45.000000 elmax_api-0.0.3rc4/elmax_api/model/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2022-12-04 12:05:45.000000 elmax_api-0.0.3rc4/elmax_api/model/cover.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2022-12-04 12:05:45.000000 elmax_api-0.0.3rc4/elmax_api/model/cover_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2022-12-04 12:05:45.000000 elmax_api-0.0.3rc4/elmax_api/model/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2022-12-04 12:05:45.000000 elmax_api-0.0.3rc4/elmax_api/model/goup.py
--rw-r--r--   0 runner    (1001) docker     (123)     7539 2022-12-04 12:05:45.000000 elmax_api-0.0.3rc4/elmax_api/model/panel.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2022-12-04 12:05:45.000000 elmax_api-0.0.3rc4/elmax_api/model/scene.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2022-12-04 12:05:45.000000 elmax_api-0.0.3rc4/elmax_api/model/zone.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 12:05:59.269538 elmax_api-0.0.3rc4/elmax_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2022-12-04 12:05:59.000000 elmax_api-0.0.3rc4/elmax_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      608 2022-12-04 12:05:59.000000 elmax_api-0.0.3rc4/elmax_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-04 12:05:59.000000 elmax_api-0.0.3rc4/elmax_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2022-12-04 12:05:59.000000 elmax_api-0.0.3rc4/elmax_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2022-12-04 12:05:59.000000 elmax_api-0.0.3rc4/elmax_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-04 12:05:45.000000 elmax_api-0.0.3rc4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-04 12:05:59.273539 elmax_api-0.0.3rc4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2022-12-04 12:05:45.000000 elmax_api-0.0.3rc4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:49:43.704658 elmax_api-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-04-23 18:49:43.704658 elmax_api-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-23 18:49:28.000000 elmax_api-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:49:43.696658 elmax_api-0.0.4/elmax_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-23 18:49:28.000000 elmax_api-0.0.4/elmax_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-23 18:49:28.000000 elmax_api-0.0.4/elmax_api/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-23 18:49:28.000000 elmax_api-0.0.4/elmax_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23207 2023-04-23 18:49:28.000000 elmax_api-0.0.4/elmax_api/http.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:49:43.700658 elmax_api-0.0.4/elmax_api/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 18:49:28.000000 elmax_api-0.0.4/elmax_api/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-23 18:49:28.000000 elmax_api-0.0.4/elmax_api/model/actuator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-23 18:49:28.000000 elmax_api-0.0.4/elmax_api/model/alarm_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-04-23 18:49:28.000000 elmax_api-0.0.4/elmax_api/model/area.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-23 18:49:28.000000 elmax_api-0.0.4/elmax_api/model/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-23 18:49:28.000000 elmax_api-0.0.4/elmax_api/model/cover.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-23 18:49:28.000000 elmax_api-0.0.4/elmax_api/model/cover_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-23 18:49:28.000000 elmax_api-0.0.4/elmax_api/model/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-23 18:49:28.000000 elmax_api-0.0.4/elmax_api/model/goup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-04-23 18:49:28.000000 elmax_api-0.0.4/elmax_api/model/panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-23 18:49:28.000000 elmax_api-0.0.4/elmax_api/model/scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-23 18:49:28.000000 elmax_api-0.0.4/elmax_api/model/zone.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:49:43.700658 elmax_api-0.0.4/elmax_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-04-23 18:49:43.000000 elmax_api-0.0.4/elmax_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-23 18:49:43.000000 elmax_api-0.0.4/elmax_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 18:49:43.000000 elmax_api-0.0.4/elmax_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-23 18:49:43.000000 elmax_api-0.0.4/elmax_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-23 18:49:43.000000 elmax_api-0.0.4/elmax_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 18:49:28.000000 elmax_api-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 18:49:43.704658 elmax_api-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-23 18:49:28.000000 elmax_api-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:49:43.704658 elmax_api-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-23 18:49:28.000000 elmax_api-0.0.4/tests/test_actuator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-04-23 18:49:28.000000 elmax_api-0.0.4/tests/test_area.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-23 18:49:28.000000 elmax_api-0.0.4/tests/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-04-23 18:49:28.000000 elmax_api-0.0.4/tests/test_control_panels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-04-23 18:49:28.000000 elmax_api-0.0.4/tests/test_cover.py
```

### Comparing `elmax_api-0.0.3rc4/PKG-INFO` & `elmax_api-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elmax_api
-Version: 0.0.3rc4
+Version: 0.0.4
 Summary: Asynchronous API Library to work with Elmax devices
 Home-page: https://github.com/albertogeniola/elmax-api
 Author: Alberto Geniola
 Author-email: albertogeniola@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/albertogeniola/elmax-api
 Project-URL: Source, https://github.com/albertogeniola/elmax-api
```

### Comparing `elmax_api-0.0.3rc4/README.md` & `elmax_api-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `elmax_api-0.0.3rc4/elmax_api/exceptions.py` & `elmax_api-0.0.4/elmax_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `elmax_api-0.0.3rc4/elmax_api/http.py` & `elmax_api-0.0.4/elmax_api/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 
 def async_auth(func, *method_args, **method_kwargs):
     """
     Asynchronous decorator used to check validity of JWT token.
     It takes care to verify the validity of a JWT token before issuing the method call.
     In case the JWT is expired, or close to expiration date, it tries to renew it.
     """
+
     @functools.wraps(func, *method_args, **method_kwargs)
     async def wrapper(*args, **kwargs):
         # Check whether the client has a valid token to be used. We consider valid tokens with expiration time
         # > 10minutes. If not, try to login first and then proceed with the function call.
         now = time.time()
         _instance = args[0]
         assert isinstance(_instance, GenericElmax)
@@ -69,15 +70,16 @@
 class GenericElmax(ABC):
     """
     Abstract Elmax HTTP client.
     This class takes care of handling API calls against the ELMAX API cloud endpoint.
     It handles data marshalling/unmarshalling, login and token renewal upon expiration.
     """
 
-    def __init__(self,base_url:str=BASE_URL,current_panel_id: str = None, current_panel_pin: str = DEFAULT_PANEL_PIN,
+    def __init__(self, base_url: str = BASE_URL, current_panel_id: str = None,
+                 current_panel_pin: str = DEFAULT_PANEL_PIN,
                  timeout: float = DEFAULT_HTTP_TIMEOUT, ssl_context: Optional[ssl.SSLContext] = None):
         """Base constructor.
 
         Args:
             base_url: API server base-URL
             current_panel_id: Panel id of the preferred panel
             current_panel_pin: Panel PIN of the preferred panel
@@ -92,15 +94,15 @@
         self._base_url = URL(base_url)
 
         # Build the SSL context we trust
         sslcontext = ssl_context if ssl_context is not None else True
         self._http_client = httpx.AsyncClient(timeout=timeout, verify=sslcontext)
 
     @classmethod
-    async def retrieve_server_certificate(cls, hostname:str, port:int):
+    async def retrieve_server_certificate(cls, hostname: str, port: int):
         try:
             pem_server_certificate = ssl.get_server_certificate((hostname, port))
             return pem_server_certificate
         except (socket.gaierror, ConnectionRefusedError) as ex:
             raise ElmaxNetworkError from ex
 
     def set_default_timeout(self, timeout: float):
@@ -109,34 +111,62 @@
 
     async def _request(
             self,
             method: "Elmax.HttpMethod",
             url: str,
             data: Optional[Dict] = None,
             authorized: bool = False,
-            timeout: float = DEFAULT_HTTP_TIMEOUT
+            timeout: float = DEFAULT_HTTP_TIMEOUT,
+            retry_attempts: int = 3
     ) -> Dict:
         """
-        Executes a HTTP API request against a given endpoint, parses the output and returns the
+        Executes an HTTP API request against a given endpoint, parses the output and returns the
         json to the caller. It handles most basic IO exceptions.
         If the API returns a non 200 response, this method raises an `ElmaxApiError`
 
         Args:
             method: HTTP method to use for the HTTP request
             url: Target request URL
             data: Json data/Data to post in POST messages. Ignored when issuing GET requests
             authorized: When set, the request is performed passing the stored authorization token
+            timeout: timeout in seconds for a single attempt
+            retry_attempts: number of retry attempts in case of 422 (panel busy)
 
         Returns:
             Dict: The dictionary object containing authenticated JWT data
 
         Raises:
             ElmaxApiError: Whenever a non 200 return code is returned by the remote server
             ElmaxNetworkError: If the http request could not be completed due to a network error
+            ElmaxPanelBusyError: If the number of retries have been exhausted while the panel returned a busy state (422)
         """
+        retry_attempt = 0
+        while retry_attempt < retry_attempts:
+            try:
+                response_data = await self._internal_request(method=method, url=url, data=data, authorized=authorized,
+                                                             timeout=timeout)
+                _LOGGER.debug(response_data)
+                return response_data
+            except ElmaxApiError as e:
+                if e.status_code == 422:
+                    retry_attempt += 1
+                    _LOGGER.error("Panel is busy. Command will be retried in a moment.")
+                    await asyncio.sleep(BUSY_WAIT_INTERVAL)
+                else:
+                    raise
+        raise ElmaxPanelBusyError()
+
+    async def _internal_request(
+            self,
+            method: "Elmax.HttpMethod",
+            url: str,
+            data: Optional[Dict] = None,
+            authorized: bool = False,
+            timeout: float = DEFAULT_HTTP_TIMEOUT
+    ) -> Dict:
         headers = {
             "User-Agent": USER_AGENT,
             "Accept": "application/json",
             "Content-Type": "application/json",
         }
         if authorized:
             headers["Authorization"] = f"JWT {self._raw_jwt}"
@@ -162,25 +192,25 @@
                     url,
                     str(data),
                     response.status_code,
                     str(response.content),
                 )
                 raise ElmaxApiError(status_code=response.status_code)
 
-            # TODO: the current API version does not return an error description nor an error http
+            # The current API version does not return an error description nor an error http
             #  status code for invalid logins. Instead, an empty body is returned. In that case we
             #  assume the login failed due to invalid user/pass combination
             response_content = response.text
             if response_content == '':
                 raise ElmaxBadLoginError()
 
             return response.json()
 
         # Wrap any other HTTP/NETWORK error
-        except (httpx.ConnectError, httpx.ReadTimeout):
+        except (httpx.ConnectError, httpx.ReadTimeout) as e:
             _LOGGER.exception("An unhandled error occurred while executing API Call.")
             raise ElmaxNetworkError("A network error occurred")
 
     @property
     def current_panel_id(self) -> str:
         return self._current_panel_id
 
@@ -193,15 +223,15 @@
         """
         Specifies whether the client has been granted a JWT which is still valid (not expired)
 
         Returns:
             bool: True if there is a valid JWT token, False if there's no token or if it is expired
         """
         if self._jwt is None:
-            # The user did not login yet
+            # The user did not log in yet
             return False
         if self._jwt.get("exp", 0) <= time.time():
             self._jwt = None
             return False
         return True
 
     @property
@@ -262,18 +292,18 @@
         response_data = await self._request(Elmax.HttpMethod.GET, url=url, authorized=True)
         status = EndpointStatus.from_api_response(response_entry=response_data)
         return status
 
     @async_auth
     @abstractmethod
     async def execute_command(self,
-                               endpoint_id: str,
-                               command: Union[Command, str],
-                               extra_payload: Dict = None,
-                               retry_attempts: int = 3) -> Optional[Dict]:
+                              endpoint_id: str,
+                              command: Union[Command, str],
+                              extra_payload: Dict = None,
+                              retry_attempts: int = 3) -> Optional[Dict]:
         """
         Executes a command against the given endpoint
         Args:
             endpoint_id: EndpointID against which the command should be issued
             command: Command to issue. Can either be a string or a `Command` enum value
             extra_payload: Dictionary of extra payload to be issued to the endpoint
             retry_attempts: Maximum retry attempts in case of 422 error (panel busy)
@@ -287,38 +317,28 @@
                                url: str,
                                extra_payload: Dict = None,
                                retry_attempts: int = 3) -> Optional[Dict]:
 
         if extra_payload is not None and not isinstance(extra_payload, dict):
             raise ValueError("The extra_payload parameter must be a dictionary")
 
-        retry_attempt = 0
-        while retry_attempt < retry_attempts:
-            try:
-                response_data = await self._request(Elmax.HttpMethod.POST, url=url, authorized=True, data=extra_payload)
-                _LOGGER.debug(response_data)
-                return response_data
-            except ElmaxApiError as e:
-                if e.status_code == 422:
-                    retry_attempt += 1
-                    _LOGGER.error("Panel is busy. Command will be retried in a moment.")
-                    await asyncio.sleep(BUSY_WAIT_INTERVAL)
-                else:
-                    raise
-        raise ElmaxPanelBusyError()
+        response_data = await self._request(Elmax.HttpMethod.POST, url=url, authorized=True, data=extra_payload,
+                                            retry_attempts=retry_attempts)
+        _LOGGER.debug(response_data)
+        return response_data
 
     def get_authenticated_username(self) -> Optional[str]:
         """
         Returns the username associated to the current JWT token, if any.
         In case the user is not authenticated, returns None
         """
         if self._jwt is None:
             return None
         return self._jwt.get("email")
-                
+
     class HttpMethod(Enum):
         """Enumerative helper for supported HTTP methods of the Elmax API"""
 
         GET = "get"
         POST = "post"
 
 
@@ -460,23 +480,24 @@
         return await self.get_panel_status(control_panel_id=self._current_panel_id, pin=self._current_panel_pin)
 
 
 class ElmaxLocal(GenericElmax):
     """
     Class implementing the Local HTTP API client.
     """
+
     def __init__(self, panel_api_url: str, panel_code: str, ssl_context: ssl.SSLContext = None):
         """Client constructor.
 
         Args:
             panel_api_url: API address of the Elmax Panel
             panel_code: authentication code to be used with the panel
             ssl_context: SSLContext object to use for SSL verification
         """
-        super(ElmaxLocal, self).__init__(base_url=panel_api_url,ssl_context=ssl_context)
+        super(ElmaxLocal, self).__init__(base_url=panel_api_url, ssl_context=ssl_context)
         # The current version of the local API does not expose the panel ID attribute,
         # so we use the panel IP as ID
         self.set_current_panel(panel_id=panel_api_url, panel_pin=panel_code)
 
     async def login(self, *args, **kwargs) -> Dict:
         """
         Connects to the Local ENDPOINT and returns the access token to be used within the client
@@ -561,8 +582,8 @@
         except ElmaxApiError as e:
             if e.status_code == 403:
                 raise ElmaxBadPinError() from e
             else:
                 raise
 
         panel_status = PanelStatus.from_api_response(response_entry=response_data)
-        return panel_status
+        return panel_status
```

### Comparing `elmax_api-0.0.3rc4/elmax_api/model/actuator.py` & `elmax_api-0.0.4/elmax_api/model/actuator.py`

 * *Files identical despite different names*

### Comparing `elmax_api-0.0.3rc4/elmax_api/model/area.py` & `elmax_api-0.0.4/elmax_api/model/area.py`

 * *Files identical despite different names*

### Comparing `elmax_api-0.0.3rc4/elmax_api/model/cover.py` & `elmax_api-0.0.4/elmax_api/model/cover.py`

 * *Files identical despite different names*

### Comparing `elmax_api-0.0.3rc4/elmax_api/model/endpoint.py` & `elmax_api-0.0.4/elmax_api/model/endpoint.py`

 * *Files identical despite different names*

### Comparing `elmax_api-0.0.3rc4/elmax_api/model/goup.py` & `elmax_api-0.0.4/elmax_api/model/goup.py`

 * *Files identical despite different names*

### Comparing `elmax_api-0.0.3rc4/elmax_api/model/panel.py` & `elmax_api-0.0.4/elmax_api/model/panel.py`

 * *Files identical despite different names*

### Comparing `elmax_api-0.0.3rc4/elmax_api/model/scene.py` & `elmax_api-0.0.4/elmax_api/model/scene.py`

 * *Files identical despite different names*

### Comparing `elmax_api-0.0.3rc4/elmax_api/model/zone.py` & `elmax_api-0.0.4/elmax_api/model/zone.py`

 * *Files identical despite different names*

### Comparing `elmax_api-0.0.3rc4/elmax_api.egg-info/PKG-INFO` & `elmax_api-0.0.4/elmax_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elmax-api
-Version: 0.0.3rc4
+Version: 0.0.4
 Summary: Asynchronous API Library to work with Elmax devices
 Home-page: https://github.com/albertogeniola/elmax-api
 Author: Alberto Geniola
 Author-email: albertogeniola@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/albertogeniola/elmax-api
 Project-URL: Source, https://github.com/albertogeniola/elmax-api
```

### Comparing `elmax_api-0.0.3rc4/elmax_api.egg-info/SOURCES.txt` & `elmax_api-0.0.4/elmax_api.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -17,8 +17,13 @@
 elmax_api/model/command.py
 elmax_api/model/cover.py
 elmax_api/model/cover_status.py
 elmax_api/model/endpoint.py
 elmax_api/model/goup.py
 elmax_api/model/panel.py
 elmax_api/model/scene.py
-elmax_api/model/zone.py
+elmax_api/model/zone.py
+tests/test_actuator.py
+tests/test_area.py
+tests/test_authentication.py
+tests/test_control_panels.py
+tests/test_cover.py
```

### Comparing `elmax_api-0.0.3rc4/setup.py` & `elmax_api-0.0.4/setup.py`

 * *Files identical despite different names*

