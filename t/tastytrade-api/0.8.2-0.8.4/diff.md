# Comparing `tmp/tastytrade-api-0.8.2.tar.gz` & `tmp/tastytrade-api-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tastytrade-api-0.8.2.tar", last modified: Sun Apr 23 08:32:40 2023, max compression
+gzip compressed data, was "tastytrade-api-0.8.4.tar", last modified: Sun Apr 23 08:45:12 2023, max compression
```

## Comparing `tastytrade-api-0.8.2.tar` & `tastytrade-api-0.8.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 08:32:40.026306 tastytrade-api-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 08:32:20.000000 tastytrade-api-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-23 08:32:40.026306 tastytrade-api-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-23 08:32:20.000000 tastytrade-api-0.8.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 08:32:40.026306 tastytrade-api-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-23 08:32:20.000000 tastytrade-api-0.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 08:32:40.022306 tastytrade-api-0.8.2/tastytrade_api/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 08:32:20.000000 tastytrade-api-0.8.2/tastytrade_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 08:32:40.022306 tastytrade-api-0.8.2/tastytrade_api/account/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 08:32:20.000000 tastytrade-api-0.8.2/tastytrade_api/account/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9051 2023-04-23 08:32:20.000000 tastytrade-api-0.8.2/tastytrade_api/account/account_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-04-23 08:32:20.000000 tastytrade-api-0.8.2/tastytrade_api/account/balances_positions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-04-23 08:32:20.000000 tastytrade-api-0.8.2/tastytrade_api/authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 08:32:40.022306 tastytrade-api-0.8.2/tastytrade_api/market_data/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 08:32:20.000000 tastytrade-api-0.8.2/tastytrade_api/market_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16855 2023-04-23 08:32:20.000000 tastytrade-api-0.8.2/tastytrade_api/market_data/instruments.py
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-04-23 08:32:20.000000 tastytrade-api-0.8.2/tastytrade_api/market_data/market_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 08:32:40.026306 tastytrade-api-0.8.2/tastytrade_api/streamer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 08:32:20.000000 tastytrade-api-0.8.2/tastytrade_api/streamer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-04-23 08:32:20.000000 tastytrade-api-0.8.2/tastytrade_api/streamer/dx_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-04-23 08:32:20.000000 tastytrade-api-0.8.2/tastytrade_api/streamer/dxfeed_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-04-23 08:32:20.000000 tastytrade-api-0.8.2/tastytrade_api/streamer/streamer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-04-23 08:32:20.000000 tastytrade-api-0.8.2/tastytrade_api/symbology.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 08:32:40.022306 tastytrade-api-0.8.2/tastytrade_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-23 08:32:40.000000 tastytrade-api-0.8.2/tastytrade_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-23 08:32:40.000000 tastytrade-api-0.8.2/tastytrade_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 08:32:40.000000 tastytrade-api-0.8.2/tastytrade_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-23 08:32:40.000000 tastytrade-api-0.8.2/tastytrade_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-23 08:32:40.000000 tastytrade-api-0.8.2/tastytrade_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 08:32:40.026306 tastytrade-api-0.8.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 08:32:20.000000 tastytrade-api-0.8.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-04-23 08:32:20.000000 tastytrade-api-0.8.2/tests/test_authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 08:45:12.549508 tastytrade-api-0.8.4/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 08:44:46.000000 tastytrade-api-0.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-23 08:45:12.549508 tastytrade-api-0.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-23 08:44:46.000000 tastytrade-api-0.8.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 08:45:12.549508 tastytrade-api-0.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-23 08:44:46.000000 tastytrade-api-0.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 08:45:12.545508 tastytrade-api-0.8.4/tastytrade_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 08:44:46.000000 tastytrade-api-0.8.4/tastytrade_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 08:45:12.549508 tastytrade-api-0.8.4/tastytrade_api/account/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 08:44:46.000000 tastytrade-api-0.8.4/tastytrade_api/account/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9051 2023-04-23 08:44:46.000000 tastytrade-api-0.8.4/tastytrade_api/account/account_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-04-23 08:44:46.000000 tastytrade-api-0.8.4/tastytrade_api/account/balances_positions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-04-23 08:44:46.000000 tastytrade-api-0.8.4/tastytrade_api/authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 08:45:12.549508 tastytrade-api-0.8.4/tastytrade_api/market_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 08:44:46.000000 tastytrade-api-0.8.4/tastytrade_api/market_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17818 2023-04-23 08:44:46.000000 tastytrade-api-0.8.4/tastytrade_api/market_data/instruments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-04-23 08:44:46.000000 tastytrade-api-0.8.4/tastytrade_api/market_data/market_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 08:45:12.549508 tastytrade-api-0.8.4/tastytrade_api/streamer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 08:44:46.000000 tastytrade-api-0.8.4/tastytrade_api/streamer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-04-23 08:44:46.000000 tastytrade-api-0.8.4/tastytrade_api/streamer/dx_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-04-23 08:44:46.000000 tastytrade-api-0.8.4/tastytrade_api/streamer/dxfeed_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-04-23 08:44:46.000000 tastytrade-api-0.8.4/tastytrade_api/streamer/streamer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-04-23 08:44:46.000000 tastytrade-api-0.8.4/tastytrade_api/symbology.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 08:45:12.545508 tastytrade-api-0.8.4/tastytrade_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-23 08:45:12.000000 tastytrade-api-0.8.4/tastytrade_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-23 08:45:12.000000 tastytrade-api-0.8.4/tastytrade_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 08:45:12.000000 tastytrade-api-0.8.4/tastytrade_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-23 08:45:12.000000 tastytrade-api-0.8.4/tastytrade_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-23 08:45:12.000000 tastytrade-api-0.8.4/tastytrade_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 08:45:12.549508 tastytrade-api-0.8.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 08:44:46.000000 tastytrade-api-0.8.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-04-23 08:44:46.000000 tastytrade-api-0.8.4/tests/test_authentication.py
```

### Comparing `tastytrade-api-0.8.2/PKG-INFO` & `tastytrade-api-0.8.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tastytrade-api
-Version: 0.8.2
+Version: 0.8.4
 Summary: A Python client and SDK for the Tastytrade API
 Home-page: https://github.com/peter-oroszvari/tastytrade-api
 Author: Peter Oroszvari
 Author-email: peter@oroszvari.hu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tastytrade-api-0.8.2/README.md` & `tastytrade-api-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `tastytrade-api-0.8.2/setup.py` & `tastytrade-api-0.8.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="tastytrade-api",
-    version="0.8.2",
+    version="0.8.4",
     author="Peter Oroszvari",
     author_email="peter@oroszvari.hu",
     description="A Python client and SDK for the Tastytrade API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/peter-oroszvari/tastytrade-api",
     packages=find_packages(),
```

### Comparing `tastytrade-api-0.8.2/tastytrade_api/account/account_handler.py` & `tastytrade-api-0.8.4/tastytrade_api/account/account_handler.py`

 * *Files identical despite different names*

### Comparing `tastytrade-api-0.8.2/tastytrade_api/account/balances_positions.py` & `tastytrade-api-0.8.4/tastytrade_api/account/balances_positions.py`

 * *Files identical despite different names*

### Comparing `tastytrade-api-0.8.2/tastytrade_api/authentication.py` & `tastytrade-api-0.8.4/tastytrade_api/authentication.py`

 * *Files 18% similar despite different names*

```diff
@@ -105,7 +105,40 @@
             if response.status_code == 200:
                 data = response.json()
                 return data
             else:
                 print(f"Error: {response.status_code}")
                 print("Response text:", response.text)
                 return None
+    def create_session(self, username: str, password: str, remember_me: bool = False, remember_token: str = None) -> Optional[Dict[str, str]]:
+        """
+        Creates a new user session with the Tastytrade API, using the specified username and password.
+
+        Args:
+            username (str): The username or email of the user.
+            password (str): The password for the user's account.
+            remember_me (bool): Whether the session should be extended for longer than normal via remember token. Defaults to False.
+            remember_token (str): The remember token. Allows skipping for 2 factor within its window.
+
+        Returns:
+            Optional[Dict[str, str]]: A dictionary containing the user's session token and other related data. Returns None if there's an error.
+        """
+        payload = {
+            "login": username,
+            "password": password,
+            "remember-me": remember_me,
+            "remember-token": remember_token
+        }
+
+        headers = {}
+        response = requests.post(self.url, headers=headers, json=payload)
+
+        if response.status_code == 201:
+            data = response.json()
+            self.session_token = data['data']['session-token']
+            self.remember_token = data['data']['remember-token']
+            self.user_data = data['data']['user']
+            self.token_timestamp = time.time()
+            return data
+        else:
+            print(f"Error: {response.status_code}")
+            return None
```

### Comparing `tastytrade-api-0.8.2/tastytrade_api/market_data/instruments.py` & `tastytrade-api-0.8.4/tastytrade_api/market_data/instruments.py`

 * *Files 2% similar despite different names*

```diff
@@ -383,8 +383,33 @@
     Returns a set of warrant definitions that can be filtered by parameters
     """
     
     """
     TBD: Future options chanins and option chains implementation
     """
 
+    def get_symbol_data(self, symbol: str) -> List[Dict[str, Any]]:
+        """
+        Makes a GET request to the /symbols/search/{symbol} API endpoint and returns an array of symbol data.
+
+        Args:
+            symbol (str): The symbol to search for.
+
+        Returns:
+            list: List of symbol objects, as returned by the API.
+
+        Raises:
+            Exception: If there was an error in the GET request or if the status code is not 200 OK.
+        """
+        headers = {
+            "Authorization": f"{self.session_token}"
+        }
+
+        response = requests.get(f"{self.api_url}/symbols/search/{symbol}", headers=headers)
+
+        if response.status_code == 200:
+            response_data = json.loads(response.content)
+            symbol_data = response_data["data"]["items"]
+            return symbol_data
+        else:
+            raise Exception(f"Error getting symbol data for {symbol}: {response.status_code} - {response.content}")
```

### Comparing `tastytrade-api-0.8.2/tastytrade_api/market_data/market_metrics.py` & `tastytrade-api-0.8.4/tastytrade_api/market_data/market_metrics.py`

 * *Files identical despite different names*

### Comparing `tastytrade-api-0.8.2/tastytrade_api/streamer/dx_mapping.py` & `tastytrade-api-0.8.4/tastytrade_api/streamer/dx_mapping.py`

 * *Files identical despite different names*

### Comparing `tastytrade-api-0.8.2/tastytrade_api/streamer/dxfeed_handler.py` & `tastytrade-api-0.8.4/tastytrade_api/streamer/dxfeed_handler.py`

 * *Files identical despite different names*

### Comparing `tastytrade-api-0.8.2/tastytrade_api/streamer/streamer.py` & `tastytrade-api-0.8.4/tastytrade_api/streamer/streamer.py`

 * *Files identical despite different names*

### Comparing `tastytrade-api-0.8.2/tastytrade_api/symbology.py` & `tastytrade-api-0.8.4/tastytrade_api/symbology.py`

 * *Files identical despite different names*

### Comparing `tastytrade-api-0.8.2/tastytrade_api.egg-info/PKG-INFO` & `tastytrade-api-0.8.4/tastytrade_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tastytrade-api
-Version: 0.8.2
+Version: 0.8.4
 Summary: A Python client and SDK for the Tastytrade API
 Home-page: https://github.com/peter-oroszvari/tastytrade-api
 Author: Peter Oroszvari
 Author-email: peter@oroszvari.hu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tastytrade-api-0.8.2/tastytrade_api.egg-info/SOURCES.txt` & `tastytrade-api-0.8.4/tastytrade_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tastytrade-api-0.8.2/tests/test_authentication.py` & `tastytrade-api-0.8.4/tests/test_authentication.py`

 * *Files identical despite different names*

