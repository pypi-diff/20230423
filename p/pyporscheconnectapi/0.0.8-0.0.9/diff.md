# Comparing `tmp/pyporscheconnectapi-0.0.8.tar.gz` & `tmp/pyporscheconnectapi-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyporscheconnectapi-0.0.8.tar", last modified: Thu Feb 18 21:36:05 2021, max compression
+gzip compressed data, was "pyporscheconnectapi-0.0.9.tar", last modified: Sun Jun 20 20:57:47 2021, max compression
```

## Comparing `pyporscheconnectapi-0.0.8.tar` & `pyporscheconnectapi-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-18 21:36:05.149713 pyporscheconnectapi-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (116)      472 2021-02-18 21:36:05.149713 pyporscheconnectapi-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     3139 2021-02-18 21:35:49.000000 pyporscheconnectapi-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-18 21:36:05.145713 pyporscheconnectapi-0.0.8/pyporscheconnectapi/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-18 21:35:49.000000 pyporscheconnectapi-0.0.8/pyporscheconnectapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5571 2021-02-18 21:35:49.000000 pyporscheconnectapi-0.0.8/pyporscheconnectapi/cli.py
--rw-r--r--   0 runner    (1001) docker     (116)     6363 2021-02-18 21:35:49.000000 pyporscheconnectapi-0.0.8/pyporscheconnectapi/client.py
--rw-r--r--   0 runner    (1001) docker     (116)     8414 2021-02-18 21:35:49.000000 pyporscheconnectapi-0.0.8/pyporscheconnectapi/connection.py
--rw-r--r--   0 runner    (1001) docker     (116)     1409 2021-02-18 21:35:49.000000 pyporscheconnectapi-0.0.8/pyporscheconnectapi/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-18 21:36:05.149713 pyporscheconnectapi-0.0.8/pyporscheconnectapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      472 2021-02-18 21:36:04.000000 pyporscheconnectapi-0.0.8/pyporscheconnectapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      445 2021-02-18 21:36:05.000000 pyporscheconnectapi-0.0.8/pyporscheconnectapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-02-18 21:36:04.000000 pyporscheconnectapi-0.0.8/pyporscheconnectapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       60 2021-02-18 21:36:04.000000 pyporscheconnectapi-0.0.8/pyporscheconnectapi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)       10 2021-02-18 21:36:04.000000 pyporscheconnectapi-0.0.8/pyporscheconnectapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       20 2021-02-18 21:36:04.000000 pyporscheconnectapi-0.0.8/pyporscheconnectapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      123 2021-02-18 21:36:05.149713 pyporscheconnectapi-0.0.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (116)      831 2021-02-18 21:35:49.000000 pyporscheconnectapi-0.0.8/setup.py
+drwxr-xr-x   0 johan      (501) staff       (20)        0 2021-06-20 20:57:47.256555 pyporscheconnectapi-0.0.9/
+-rw-r--r--   0 johan      (501) staff       (20)     1071 2021-01-26 22:38:51.000000 pyporscheconnectapi-0.0.9/LICENSE
+-rw-r--r--   0 johan      (501) staff       (20)      472 2021-06-20 20:57:47.256679 pyporscheconnectapi-0.0.9/PKG-INFO
+-rw-r--r--   0 johan      (501) staff       (20)     3678 2021-06-20 20:52:35.000000 pyporscheconnectapi-0.0.9/README.md
+drwxr-xr-x   0 johan      (501) staff       (20)        0 2021-06-20 20:57:47.254428 pyporscheconnectapi-0.0.9/pyporscheconnectapi/
+-rw-r--r--   0 johan      (501) staff       (20)        0 2021-02-01 22:27:05.000000 pyporscheconnectapi-0.0.9/pyporscheconnectapi/__init__.py
+-rw-r--r--   0 johan      (501) staff       (20)     5607 2021-06-20 20:52:35.000000 pyporscheconnectapi-0.0.9/pyporscheconnectapi/cli.py
+-rw-r--r--   0 johan      (501) staff       (20)    12891 2021-06-20 20:52:35.000000 pyporscheconnectapi-0.0.9/pyporscheconnectapi/client.py
+-rw-r--r--   0 johan      (501) staff       (20)     9263 2021-06-20 20:52:35.000000 pyporscheconnectapi-0.0.9/pyporscheconnectapi/connection.py
+-rw-r--r--   0 johan      (501) staff       (20)     1409 2021-02-03 07:49:14.000000 pyporscheconnectapi-0.0.9/pyporscheconnectapi/exceptions.py
+drwxr-xr-x   0 johan      (501) staff       (20)        0 2021-06-20 20:57:47.256338 pyporscheconnectapi-0.0.9/pyporscheconnectapi.egg-info/
+-rw-r--r--   0 johan      (501) staff       (20)      472 2021-06-20 20:57:47.000000 pyporscheconnectapi-0.0.9/pyporscheconnectapi.egg-info/PKG-INFO
+-rw-r--r--   0 johan      (501) staff       (20)      453 2021-06-20 20:57:47.000000 pyporscheconnectapi-0.0.9/pyporscheconnectapi.egg-info/SOURCES.txt
+-rw-r--r--   0 johan      (501) staff       (20)        1 2021-06-20 20:57:47.000000 pyporscheconnectapi-0.0.9/pyporscheconnectapi.egg-info/dependency_links.txt
+-rw-r--r--   0 johan      (501) staff       (20)       60 2021-06-20 20:57:47.000000 pyporscheconnectapi-0.0.9/pyporscheconnectapi.egg-info/entry_points.txt
+-rw-r--r--   0 johan      (501) staff       (20)       10 2021-06-20 20:57:47.000000 pyporscheconnectapi-0.0.9/pyporscheconnectapi.egg-info/requires.txt
+-rw-r--r--   0 johan      (501) staff       (20)       20 2021-06-20 20:57:47.000000 pyporscheconnectapi-0.0.9/pyporscheconnectapi.egg-info/top_level.txt
+-rw-r--r--   0 johan      (501) staff       (20)      123 2021-06-20 20:57:47.257078 pyporscheconnectapi-0.0.9/setup.cfg
+-rwxr-xr-x   0 johan      (501) staff       (20)      831 2021-06-20 20:54:02.000000 pyporscheconnectapi-0.0.9/setup.py
```

### Comparing `pyporscheconnectapi-0.0.8/README.md` & `pyporscheconnectapi-0.0.9/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -19,37 +19,42 @@
 ```
 
 Setup will add a cli under the name porschecli, see below for usage
 
 
 ## CLI usage
 
-A simple cli is provided with this library, it will cache tokens to a file to speed up invocations
+A simple cli is provided with this library, it will cache tokens to a file to speed up invocations. It does not yet support the create/update/delete timer functionality which is present in the library.
 
+If no email or password is supplied as input arguments you will be prompted. Same goes for PIN (used to lock or unlock).
+The --nowait option will just request the action (or stored information) without waiting for confirmation.
 ```
-usage: porschecli [-h] -e EMAIL -p PASSWORD [-s SESSION_FILE] [-v VIN] [-m MODEL]
-              [-a] [-c COUNTRY] [-l LANGUAGE] [-z TIMEZONE]
-              {list,overview,maintenance,summary,capabilities,emobility,position,triplongterm,tripshortterm,speedalerts,theftalerts}
+usage: cli.py [-h] [-e EMAIL] [-p PASSWORD] [-s SESSION_FILE] [-v VIN]
+              [-n PIN] [-m MODEL] [-a] [-c COUNTRY] [-l LANGUAGE]
+              [-z TIMEZONE] [--nowait]
+              {list,overview,maintenance,summary,capabilities,emobility,position,triplongterm,tripshortterm,speedalerts,theftalerts,tokens,lock,unlock,climate-on,climate-off,directcharge-on,directcharge-off}
 
 Porsche Connect CLI.
 
 positional arguments:
-  {list,overview,maintenance,summary,capabilities,emobility,position,triplongterm,tripshortterm,speedalerts,theftalerts}
+  {list,overview,maintenance,summary,capabilities,emobility,position,triplongterm,tripshortterm,speedalerts,theftalerts,tokens,lock,unlock,climate-on,climate-off,directcharge-on,directcharge-off}
 
 optional arguments:
   -h, --help            show this help message and exit
   -e EMAIL, --email EMAIL
   -p PASSWORD, --password PASSWORD
   -s SESSION_FILE, --sessionfile SESSION_FILE
   -v VIN, --vin VIN
+  -n PIN, --pin PIN
   -m MODEL, --model MODEL
   -a, --all
   -c COUNTRY, --country COUNTRY
   -l LANGUAGE, --language LANGUAGE
   -z TIMEZONE, --timezone TIMEZONE
+  --nowait
 ```
 
 ## Library usage
 
 Install pyporscheconnectapi using pip (requires python > 3.6)
 
 
@@ -71,40 +76,35 @@
 
     await conn.close()
 
 loop = asyncio.get_event_loop()
 loop.run_until_complete(vehicles())
 ```
 
-### Example connection usage for custom requests 
+### Example connection usage for custom requests
 ```
 import asyncio
 from pyporscheconnectapi.connection import Connection
 from pyporscheconnectapi.client import Client
 email = ..your porsche connect email...
 password = ...your porsche connect password...
 
 async def vehicles() -> None:
     conn = Connection(email, password)
     client = Client(conn)
 
     vehicles = await client.getVehicles()
     for vehicle in vehicles:
         print(f"VIN: {vehicle['vin']} Model: {vehicle['modelDescription']} Year: {vehicle['modelYear']}")
-        # Using connection.get will automatically add auth headers 
+        # Using connection.get will automatically add auth headers
         data = await conn.get(f"https://api.porsche.com/core/api/v3/se/sv_SE/vehicles/{vehicle['vin']}")
         print(f"Battery at {data['carControlData']['batteryLevel']['value']}%")
 
     await conn.close()
 
 loop = asyncio.get_event_loop()
 loop.run_until_complete(vehicles())
 ```
 
 
-
-
 ## Credits
 [evcc](https://github.com/andig/evcc) was a good resource for figuring out the Authentication flow
-
-
-
```

### Comparing `pyporscheconnectapi-0.0.8/pyporscheconnectapi/cli.py` & `pyporscheconnectapi-0.0.9/pyporscheconnectapi/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         with open(args.session_file) as json_file:
             tokens = json.load(json_file)
     except FileNotFoundError:
         tokens = {}
     except json.decoder.JSONDecodeError:
         tokens = {}
 
-    email = args.email or input("Please enter porsche connect email: ")
+    email = args.email or input("Please enter Porsche Connect email: ")
     password = args.password or getpass()
     conn = Connection(email, password, tokens=tokens, country=args.country, language=args.language)
 
     client = Client(conn)
 
     try:
         if args.command == "list":
@@ -68,17 +68,17 @@
                 elif args.command == "theftalerts":
                     data = await client.getTheftAlerts(vin)
                 elif args.command == "climate-on":
                     data = await client.climateOn(vin, waitForConfirmation = not args.nowait)
                 elif args.command == "climate-off":
                     data = await client.climateOff(vin, waitForConfirmation = not args.nowait)
                 elif args.command == "directcharge-on":
-                    data = await client.directChargeOn(vin, waitForConfirmation = not args.nowait)
+                    data = await client.directChargeOn(vin, model=args.model, waitForConfirmation = not args.nowait)
                 elif args.command == "directcharge-off":
-                    data = await client.directChargeOff(vin, waitForConfirmation = not args.nowait)
+                    data = await client.directChargeOff(vin, model=args.model, waitForConfirmation = not args.nowait)
                 elif args.command == 'lock' or args.command == 'unlock':
                     pin = args.pin
                     if pin is None:
                         pin = getpass("PIN code: ")
                     if(args.command == 'lock'):
                         data = await client.lock(vin, pin, waitForConfirmation = not args.nowait)
                     else:
```

### Comparing `pyporscheconnectapi-0.0.8/pyporscheconnectapi/connection.py` & `pyporscheconnectapi-0.0.9/pyporscheconnectapi/connection.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,45 +30,45 @@
     def __init__(
         self,
         email: Text = None,
         password: Text = None,
         websession: aiohttp.ClientSession = None,
         language: Text = 'de',
         country: Text = 'DE',
-        tokens = None 
+        tokens = None
     ) -> None:
         """Initialize connection object."""
         self.porscheCookiedomain: Text = "https://login.porsche.com"
         self.porscheLogin: Text = "https://login.porsche.com/auth/de/de_DE"
         self.porscheLoginAuth: Text = "https://login.porsche.com/auth/api/v1/de/de_DE/public/login"
         self.porscheAPIAuth: Text = "https://login.porsche.com/as/authorization.oauth2"
         self.porscheAPIToken: Text = "https://login.porsche.com/as/token.oauth2"
         self.porscheAPI: Text = "https://connect-portal.porsche.com/core/api/v3/de/de_DE"
         self.porscheApplications = {
                 'portal': {
-                    'client_id': 'TZ4Vf5wnKeipJxvatJ60lPHYEzqZ4WNp', 
+                    'client_id': 'TZ4Vf5wnKeipJxvatJ60lPHYEzqZ4WNp',
                     'redirect_uri': 'https://my-static02.porsche.com/static/cms/auth.html',
                     'prefix': 'https://connect-portal.porsche.com/core/api/v3/'
                     },
-                'carcontrol': { 
+                'carcontrol': {
                     'client_id': 'gZLSI7ThXFB4d2ld9t8Cx2DBRvGr1zN2',
                     'redirect_uri':  'https://connect-portal.porsche.com/myservices/auth/auth.html',
                     'prefix': 'https://api.porsche.com/'
                     }
                 }
 
         self.isTokenRefreshed = False
         self.tokens = tokens or {}
         self.email = email
         self.password = password
         self.websession = websession
         self._isLoggedIn = False
         self.country = country
         self.language = language
-        
+
         if self.websession == None:
             self.websession = aiohttp.ClientSession()
         _LOGGER.debug("New connection created")
 
 
     async def _login(self):
         _LOGGER.debug("Start authentication, get initial state from login page....")
@@ -108,15 +108,15 @@
         code_verifier = base64.urlsafe_b64encode(os.urandom(40)).decode('utf-8')
         code_verifier = re.sub('[^a-zA-Z0-9]+', '', code_verifier)
 
         code_challenge = hashlib.sha256(code_verifier.encode('utf-8')).digest()
         code_challenge = base64.urlsafe_b64encode(code_challenge).decode('utf-8')
         code_challenge = code_challenge.replace('=', '')
 
-        auth_data = { 
+        auth_data = {
                 'scope': 'openid',
                 'response_type': 'code',
                 'access_type': 'offline',
                 'prompt': 'none',
                 'client_id': application['client_id'],
                 'redirect_uri': application['redirect_uri'],
                 'code_challenge': code_challenge,
@@ -127,15 +127,15 @@
             last_location = resp.history[len(resp.history) - 1].headers['Location']
             query = urllib.parse.urlparse(last_location).query
             redirect_params = urllib.parse.parse_qs(query)
             auth_code = redirect_params['code'][0]
             _LOGGER.debug("Code %s", auth_code)
 
         auth_token_data = {
-                'grant_type': 'authorization_code', 
+                'grant_type': 'authorization_code',
                 'client_id': application['client_id'],
                 'redirect_uri': application['redirect_uri'],
                 'code': auth_code,
                 'prompt': 'none',
                 'code_verifier': code_verifier
                 }
         _LOGGER.debug("Data %s", auth_token_data)
@@ -166,14 +166,32 @@
             application = self._applicationForURL(url)
             headers = await self._createhead(application)
             async with self.websession.post(url, data=data, json=json, headers=headers) as resp:
                 return await resp.json()
         except aiohttp.ClientResponseError as exception_:
             raise PorscheException(exception_.status)
 
+    async def put(self, url, data=None, json=None):
+        try:
+            application = self._applicationForURL(url)
+            headers = await self._createhead(application)
+            async with self.websession.put(url, data=data, json=json, headers=headers) as resp:
+                return await resp.json()
+        except aiohttp.ClientResponseError as exception_:
+            raise PorscheException(exception_.status)
+
+    async def delete(self, url, data=None, json=None):
+        try:
+            application = self._applicationForURL(url)
+            headers = await self._createhead(application)
+            async with self.websession.delete(url, data=data, json=json, headers=headers) as resp:
+                return await resp.json()
+        except aiohttp.ClientResponseError as exception_:
+            raise PorscheException(exception_.status)
+
     def _applicationForURL(self, url):
        for key in self.porscheApplications:
            app = self.porscheApplications[key]
            if url.startswith(app['prefix']):
                return app
        # else return None
        return None
```

### Comparing `pyporscheconnectapi-0.0.8/pyporscheconnectapi/exceptions.py` & `pyporscheconnectapi-0.0.9/pyporscheconnectapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyporscheconnectapi-0.0.8/setup.py` & `pyporscheconnectapi-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 
 setup(
     name="pyporscheconnectapi",
-    version="0.0.8",
+    version="0.0.9",
     author="Johan Isaksson",
     author_email="johan@generatorhallen.se",
     description="Python library and CLI for communicating with Porsche Connect API.",
     include_package_data=True,
     url="https://github.com/cjne/pyporscheconnectapi",
     license="MIT",
     packages=["pyporscheconnectapi"],
```

