# Comparing `tmp/python_frank_energie-3.1.0.tar.gz` & `tmp/python_frank_energie-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_frank_energie-3.1.0.tar", max compression
+gzip compressed data, was "python_frank_energie-4.0.0.tar", max compression
```

## Comparing `python_frank_energie-3.1.0.tar` & `python_frank_energie-4.0.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11346 2023-04-16 12:06:31.436265 python_frank_energie-3.1.0/LICENSE
--rw-r--r--   0        0        0      325 2023-04-16 12:06:31.436265 python_frank_energie-3.1.0/README.md
--rw-r--r--   0        0        0     2332 2023-04-16 12:06:56.724124 python_frank_energie-3.1.0/pyproject.toml
--rw-r--r--   0        0        0      175 2023-04-16 12:06:31.436265 python_frank_energie-3.1.0/python_frank_energie/__init__.py
--rw-r--r--   0        0        0      332 2023-04-16 12:06:31.440265 python_frank_energie-3.1.0/python_frank_energie/exceptions.py
--rw-r--r--   0        0        0     5975 2023-04-16 12:06:31.440265 python_frank_energie-3.1.0/python_frank_energie/frank_energie.py
--rw-r--r--   0        0        0     6766 2023-04-16 12:06:31.440265 python_frank_energie-3.1.0/python_frank_energie/models.py
--rw-r--r--   0        0        0     1217 1970-01-01 00:00:00.000000 python_frank_energie-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11346 2023-04-23 13:11:10.815568 python_frank_energie-4.0.0/LICENSE
+-rw-r--r--   0        0        0      325 2023-04-23 13:11:10.815568 python_frank_energie-4.0.0/README.md
+-rw-r--r--   0        0        0     2353 2023-04-23 13:11:39.727562 python_frank_energie-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0      175 2023-04-23 13:11:10.815568 python_frank_energie-4.0.0/python_frank_energie/__init__.py
+-rw-r--r--   0        0        0      378 2023-04-23 13:11:10.815568 python_frank_energie-4.0.0/python_frank_energie/exceptions.py
+-rw-r--r--   0        0        0     7195 2023-04-23 13:11:10.815568 python_frank_energie-4.0.0/python_frank_energie/frank_energie.py
+-rw-r--r--   0        0        0     9879 2023-04-23 13:11:10.815568 python_frank_energie-4.0.0/python_frank_energie/models.py
+-rw-r--r--   0        0        0     1217 1970-01-01 00:00:00.000000 python_frank_energie-4.0.0/PKG-INFO
```

### Comparing `python_frank_energie-3.1.0/LICENSE` & `python_frank_energie-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_frank_energie-3.1.0/pyproject.toml` & `python_frank_energie-4.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-frank-energie"
-version = "3.1.0"
+version = "4.0.0"
 description = "Asynchronous Python client for the Frank Energie"
 authors = ["DCSBL"]
 maintainers = ["DCSBL"]
 license = "Apache License 2.0"
 readme = "README.md"
 homepage = "https://github.com/dcsbl/python-frank-energie"
 repository = "https://github.com/dcsbl/python-frank-energie"
@@ -39,14 +39,15 @@
 vulture = "^2.7"
 flake8-bandit = "^3.0.0"
 flake8-bugbear = "^23.3.12"
 flake8-builtins = "^2.1.0"
 flake8-comprehensions = "^3.10.0"
 flake8-eradicate = "^1.2.1"
 flake8-markdown = "^0.3.0"
+freezegun = "^1.2.2"
 darglint = "^1.8.1"
 safety = "^2.3.5"
 codespell = "^2.2.2"
 bandit = "^1.7.3"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/dcsbl/python-frank-energie/issues"
```

### Comparing `python_frank_energie-3.1.0/python_frank_energie/frank_energie.py` & `python_frank_energie-4.0.0/python_frank_energie/frank_energie.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,35 @@
+"""FrankEnergie API implementation."""
+
 from __future__ import annotations
 
 import asyncio
 from datetime import datetime
 from typing import Any
 
 from aiohttp.client import ClientError, ClientSession
 
 from .exceptions import AuthRequiredException
-from .models import Authentication, MonthSummary, PriceData, User
+from .models import Authentication, Invoices, MarketPrices, MonthSummary, User
 
 
 class FrankEnergie:
+    """FrankEnergie API."""
 
     DATA_URL = "https://frank-graphql-prod.graphcdn.app/"
-    _auth: Authentication | None = None
 
     def __init__(
         self,
         clientsession: ClientSession = None,
         auth_token: str | None = None,
         refresh_token: str | None = None,
     ):
+        """Initialize the FrankEnergie client."""
+        self._close_session: bool = False
+        self._auth: Authentication | None = None
         self._session = clientsession
 
         if auth_token is not None or refresh_token is not None:
             self._auth = Authentication(auth_token, refresh_token)
 
     async def _query(self, query):
         if self._session is None:
@@ -42,14 +47,15 @@
 
             return await resp.json()
 
         except (asyncio.TimeoutError, ClientError, KeyError) as error:
             raise ValueError(f"Request failed: {error}") from error
 
     async def login(self, username: str, password: str) -> str:
+        """Login and get the authentication token."""
         query = {
             "query": """
                 mutation Login($email: String!, $password: String!) {
                     login(email: $email, password: $password) {
                         authToken
                         refreshToken
                     }
@@ -59,14 +65,15 @@
             "variables": {"email": username, "password": password},
         }
 
         self._auth = Authentication.from_dict(await self._query(query))
         return self._auth
 
     async def renewToken(self, authToken: str, refreshToken: str) -> str:
+        """Renew the authentication token."""
         query = {
             "query": """
                 mutation RenewToken($authToken: String!, $refreshToken: String!) {
                     renewToken(authToken: $authToken, refreshToken: $refreshToken) {
                         authToken
                         refreshToken
                     }
@@ -79,38 +86,77 @@
         json = await self._query(query)
         print(json)
 
         self._auth = Authentication.from_dict(json)
         return self._auth
 
     async def monthSummary(self) -> MonthSummary:
-
+        """Get month summary data."""
         if self._auth is None:
             raise AuthRequiredException
 
         query = {
             "query": """
                 query MonthSummary {
                     monthSummary {
-                        _id
                         actualCostsUntilLastMeterReadingDate
                         expectedCostsUntilLastMeterReadingDate
+                        expectedCosts
                         lastMeterReadingDate
-                        __typename
                     }
                 }
             """,
             "operationName": "MonthSummary",
             "variables": {},
         }
 
         return MonthSummary.from_dict(await self._query(query))
 
-    async def user(self) -> User:
+    async def invoices(self) -> Invoices:
+        """Get invoices data.
+
+        Returns a Invoices object, containing the previous, current and upcoming invoice.
+        """
+        if self._auth is None:
+            raise AuthRequiredException
+
+        query = {
+            "query": """
+                query Invoices {
+                    invoices {
+                        previousPeriodInvoice {
+                            StartDate
+                            PeriodDescription
+                            TotalAmount
+                        }
+                        currentPeriodInvoice {
+                            StartDate
+                            PeriodDescription
+                            TotalAmount
+                        }
+                        upcomingPeriodInvoice {
+                            StartDate
+                            PeriodDescription
+                            TotalAmount
+                        }
+                    }
+                }
+            """,
+            "operationName": "Invoices",
+            "variables": {},
+        }
+
+        data = await self._query(query)
+        print(data)
+        return Invoices.from_dict(data)
+
+        # return Invoices.from_dict(await self._query(query))
 
+    async def user(self) -> User:
+        """Get user data."""
         if self._auth is None:
             raise AuthRequiredException
 
         query = {
             "query": """
                 query Me {
                     me {
@@ -130,20 +176,16 @@
             "variables": {},
         }
 
         return User.from_dict(await self._query(query))
 
     async def prices(
         self, start_date: datetime, end_date: datetime | None = None
-    ) -> tuple(PriceData, PriceData):
-        """Request to API."""
-        if self._session is None:
-            self._session = ClientSession()
-            self._close_session = True
-
+    ) -> MarketPrices:
+        """Get market prices."""
         query_data = {
             "query": """
                 query MarketPrices($startDate: Date!, $endDate: Date!) {
                     marketPricesElectricity(startDate: $startDate, endDate: $endDate) {
                        from till marketPrice marketPriceTax sourcingMarkupPrice energyTaxPrice
                     }
                     marketPricesGas(startDate: $startDate, endDate: $endDate) {
@@ -151,21 +193,15 @@
                     }
                 }
             """,
             "variables": {"startDate": str(start_date), "endDate": str(end_date)},
             "operationName": "MarketPrices",
         }
 
-        response = await self._query(query_data)
-        return (
-            PriceData(
-                response["data"]["marketPricesElectricity"] if response["data"] else {}
-            ),
-            PriceData(response["data"]["marketPricesGas"] if response["data"] else {}),
-        )
+        return MarketPrices.from_dict(await self._query(query_data))
 
     @property
     def is_authenticated(self) -> bool:
         """Return if client is authenticated.
 
         Does not actually check if the token is valid.
         """
```

### Comparing `python_frank_energie-3.1.0/PKG-INFO` & `python_frank_energie-4.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-frank-energie
-Version: 3.1.0
+Version: 4.0.0
 Summary: Asynchronous Python client for the Frank Energie
 Home-page: https://github.com/dcsbl/python-frank-energie
 License: Apache-2.0
 Author: DCSBL
 Maintainer: DCSBL
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

