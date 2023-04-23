# Comparing `tmp/tastytrade-api-0.8.0.tar.gz` & `tmp/tastytrade-api-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tastytrade-api-0.8.0.tar", last modified: Sun Apr 23 08:22:49 2023, max compression
+gzip compressed data, was "tastytrade-api-0.8.2.tar", last modified: Sun Apr 23 08:32:40 2023, max compression
```

## Comparing `tastytrade-api-0.8.0.tar` & `tastytrade-api-0.8.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 08:22:49.418609 tastytrade-api-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 08:22:28.000000 tastytrade-api-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-23 08:22:49.418609 tastytrade-api-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-23 08:22:28.000000 tastytrade-api-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 08:22:49.418609 tastytrade-api-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-23 08:22:28.000000 tastytrade-api-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 08:22:49.414609 tastytrade-api-0.8.0/tastytrade_api/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 08:22:28.000000 tastytrade-api-0.8.0/tastytrade_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 08:22:49.418609 tastytrade-api-0.8.0/tastytrade_api/account/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 08:22:28.000000 tastytrade-api-0.8.0/tastytrade_api/account/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-04-23 08:22:28.000000 tastytrade-api-0.8.0/tastytrade_api/account/account_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-04-23 08:22:28.000000 tastytrade-api-0.8.0/tastytrade_api/account/balances_positions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-04-23 08:22:28.000000 tastytrade-api-0.8.0/tastytrade_api/authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 08:22:49.418609 tastytrade-api-0.8.0/tastytrade_api/market_data/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 08:22:28.000000 tastytrade-api-0.8.0/tastytrade_api/market_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16855 2023-04-23 08:22:28.000000 tastytrade-api-0.8.0/tastytrade_api/market_data/instruments.py
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-04-23 08:22:28.000000 tastytrade-api-0.8.0/tastytrade_api/market_data/market_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 08:22:49.418609 tastytrade-api-0.8.0/tastytrade_api/streamer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 08:22:28.000000 tastytrade-api-0.8.0/tastytrade_api/streamer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-04-23 08:22:28.000000 tastytrade-api-0.8.0/tastytrade_api/streamer/dx_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-04-23 08:22:28.000000 tastytrade-api-0.8.0/tastytrade_api/streamer/dxfeed_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-04-23 08:22:28.000000 tastytrade-api-0.8.0/tastytrade_api/streamer/streamer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-04-23 08:22:28.000000 tastytrade-api-0.8.0/tastytrade_api/symbology.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 08:22:49.418609 tastytrade-api-0.8.0/tastytrade_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-23 08:22:49.000000 tastytrade-api-0.8.0/tastytrade_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-23 08:22:49.000000 tastytrade-api-0.8.0/tastytrade_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 08:22:49.000000 tastytrade-api-0.8.0/tastytrade_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-23 08:22:49.000000 tastytrade-api-0.8.0/tastytrade_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-23 08:22:49.000000 tastytrade-api-0.8.0/tastytrade_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 08:22:49.418609 tastytrade-api-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 08:22:28.000000 tastytrade-api-0.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-04-23 08:22:28.000000 tastytrade-api-0.8.0/tests/test_authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 08:32:40.026306 tastytrade-api-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 08:32:20.000000 tastytrade-api-0.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-23 08:32:40.026306 tastytrade-api-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-23 08:32:20.000000 tastytrade-api-0.8.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 08:32:40.026306 tastytrade-api-0.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-23 08:32:20.000000 tastytrade-api-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 08:32:40.022306 tastytrade-api-0.8.2/tastytrade_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 08:32:20.000000 tastytrade-api-0.8.2/tastytrade_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 08:32:40.022306 tastytrade-api-0.8.2/tastytrade_api/account/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 08:32:20.000000 tastytrade-api-0.8.2/tastytrade_api/account/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9051 2023-04-23 08:32:20.000000 tastytrade-api-0.8.2/tastytrade_api/account/account_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-04-23 08:32:20.000000 tastytrade-api-0.8.2/tastytrade_api/account/balances_positions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-04-23 08:32:20.000000 tastytrade-api-0.8.2/tastytrade_api/authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 08:32:40.022306 tastytrade-api-0.8.2/tastytrade_api/market_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 08:32:20.000000 tastytrade-api-0.8.2/tastytrade_api/market_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16855 2023-04-23 08:32:20.000000 tastytrade-api-0.8.2/tastytrade_api/market_data/instruments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-04-23 08:32:20.000000 tastytrade-api-0.8.2/tastytrade_api/market_data/market_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 08:32:40.026306 tastytrade-api-0.8.2/tastytrade_api/streamer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 08:32:20.000000 tastytrade-api-0.8.2/tastytrade_api/streamer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-04-23 08:32:20.000000 tastytrade-api-0.8.2/tastytrade_api/streamer/dx_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-04-23 08:32:20.000000 tastytrade-api-0.8.2/tastytrade_api/streamer/dxfeed_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-04-23 08:32:20.000000 tastytrade-api-0.8.2/tastytrade_api/streamer/streamer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-04-23 08:32:20.000000 tastytrade-api-0.8.2/tastytrade_api/symbology.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 08:32:40.022306 tastytrade-api-0.8.2/tastytrade_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-23 08:32:40.000000 tastytrade-api-0.8.2/tastytrade_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-23 08:32:40.000000 tastytrade-api-0.8.2/tastytrade_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 08:32:40.000000 tastytrade-api-0.8.2/tastytrade_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-23 08:32:40.000000 tastytrade-api-0.8.2/tastytrade_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-23 08:32:40.000000 tastytrade-api-0.8.2/tastytrade_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 08:32:40.026306 tastytrade-api-0.8.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 08:32:20.000000 tastytrade-api-0.8.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-04-23 08:32:20.000000 tastytrade-api-0.8.2/tests/test_authentication.py
```

### Comparing `tastytrade-api-0.8.0/PKG-INFO` & `tastytrade-api-0.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tastytrade-api
-Version: 0.8.0
+Version: 0.8.2
 Summary: A Python client and SDK for the Tastytrade API
 Home-page: https://github.com/peter-oroszvari/tastytrade-api
 Author: Peter Oroszvari
 Author-email: peter@oroszvari.hu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tastytrade-api-0.8.0/README.md` & `tastytrade-api-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `tastytrade-api-0.8.0/setup.py` & `tastytrade-api-0.8.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="tastytrade-api",
-    version="0.8.0",
+    version="0.8.2",
     author="Peter Oroszvari",
     author_email="peter@oroszvari.hu",
     description="A Python client and SDK for the Tastytrade API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/peter-oroszvari/tastytrade-api",
     packages=find_packages(),
```

### Comparing `tastytrade-api-0.8.0/tastytrade_api/account/account_handler.py` & `tastytrade-api-0.8.2/tastytrade_api/account/account_handler.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import requests
 import json
-
 class TastytradeAccount:
     """
     Initializes a new instance of the API client with the given session token and API URL.
 
     Args:
         session_token (str): The session token used to authenticate API requests.
         api_url (str): The base URL of the API.
@@ -143,8 +142,64 @@
         response = requests.get(f"{self.api_url}/accounts/{account_number}/net-liq/history", headers=headers, params=params)
         if response.status_code == 200:
             response_data = response.json()
             return response_data
         else:
             raise Exception(f"Error getting account net liq history: {response.status_code} - {response.content}")
 
+    def get_effective_margin_requirements(self, account_number, underlying_symbol):
+        """
+        This method is similar to the get_margin_requirements method, except that it retrieves the effective margin 
+        requirements for a specific underlying symbol rather than the overall margin/capital requirements report.
+        
+        Makes a GET request to the /accounts/{account_number}/margin-requirements/{underlying_symbol}/effective endpoint
+        for the specified account's effective margin requirements for the given underlying symbol, and returns the response
+        as a JSON object.
+
+        Args:
+            account_number (str): The account number for the account to retrieve effective margin requirements for.
+            underlying_symbol (str): The underlying symbol for which to retrieve effective margin requirements.
+
+        Returns:
+            dict: Dictionary containing the effective margin requirements, as returned by the API.
+
+        Raises:
+            Exception: If there was an error in the GET request or if the status code is not 200 OK.
+        """
+        headers = {
+            "Authorization": f"{self.session_token}"
+        }
+        response = requests.get(
+            f"{self.api_url}/accounts/{account_number}/margin-requirements/{underlying_symbol}/effective",
+            headers=headers
+        )
+        if response.status_code == 200:
+            response_data = response.json()
+            return response_data
+        else:
+            raise Exception(f"Error getting effective margin requirements for account {account_number}: "
+                            f"{response.status_code} - {response.content}")
+
+    def get_position_limit(self, account_number):
+        """
+        Makes a GET request to the /accounts/{account_number}/position-limit API endpoint for the specified account's
+        position limit, and returns the position limit.
 
+        Args:
+            account_number (str): The account number for the account to retrieve.
+
+        Returns:
+            int: The position limit for the account, as returned by the API.
+
+        Raises:
+            Exception: If there was an error in the GET request or if the status code is not 200 OK.
+        """
+        headers = {
+            "Authorization": f"{self.session_token}"
+        }
+        response = requests.get(f"{self.api_url}/accounts/{account_number}/position-limit", headers=headers)
+        if response.status_code == 200:
+            response_data = json.loads(response.content)
+            position_limit = response_data["data"]["positionLimit"]
+            return position_limit
+        else:
+            raise Exception(f"Error getting position limit for account {account_number}: {response.status_code} - {response.content}")
```

### Comparing `tastytrade-api-0.8.0/tastytrade_api/account/balances_positions.py` & `tastytrade-api-0.8.2/tastytrade_api/account/balances_positions.py`

 * *Files identical despite different names*

### Comparing `tastytrade-api-0.8.0/tastytrade_api/authentication.py` & `tastytrade-api-0.8.2/tastytrade_api/authentication.py`

 * *Files identical despite different names*

### Comparing `tastytrade-api-0.8.0/tastytrade_api/market_data/instruments.py` & `tastytrade-api-0.8.2/tastytrade_api/market_data/instruments.py`

 * *Files identical despite different names*

### Comparing `tastytrade-api-0.8.0/tastytrade_api/market_data/market_metrics.py` & `tastytrade-api-0.8.2/tastytrade_api/market_data/market_metrics.py`

 * *Files identical despite different names*

### Comparing `tastytrade-api-0.8.0/tastytrade_api/streamer/dx_mapping.py` & `tastytrade-api-0.8.2/tastytrade_api/streamer/dx_mapping.py`

 * *Files identical despite different names*

### Comparing `tastytrade-api-0.8.0/tastytrade_api/streamer/dxfeed_handler.py` & `tastytrade-api-0.8.2/tastytrade_api/streamer/dxfeed_handler.py`

 * *Files identical despite different names*

### Comparing `tastytrade-api-0.8.0/tastytrade_api/streamer/streamer.py` & `tastytrade-api-0.8.2/tastytrade_api/streamer/streamer.py`

 * *Files identical despite different names*

### Comparing `tastytrade-api-0.8.0/tastytrade_api/symbology.py` & `tastytrade-api-0.8.2/tastytrade_api/symbology.py`

 * *Files identical despite different names*

### Comparing `tastytrade-api-0.8.0/tastytrade_api.egg-info/PKG-INFO` & `tastytrade-api-0.8.2/tastytrade_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tastytrade-api
-Version: 0.8.0
+Version: 0.8.2
 Summary: A Python client and SDK for the Tastytrade API
 Home-page: https://github.com/peter-oroszvari/tastytrade-api
 Author: Peter Oroszvari
 Author-email: peter@oroszvari.hu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tastytrade-api-0.8.0/tastytrade_api.egg-info/SOURCES.txt` & `tastytrade-api-0.8.2/tastytrade_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tastytrade-api-0.8.0/tests/test_authentication.py` & `tastytrade-api-0.8.2/tests/test_authentication.py`

 * *Files identical despite different names*

