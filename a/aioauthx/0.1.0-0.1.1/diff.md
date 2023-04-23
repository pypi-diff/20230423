# Comparing `tmp/aioauthx-0.1.0.tar.gz` & `tmp/aioauthx-0.1.1.tar.gz`

## Comparing `aioauthx-0.1.0.tar` & `aioauthx-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 aioauthx-0.1.0/README.md
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 aioauthx-0.1.0/aioauthx/__init__.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 aioauthx-0.1.0/aioauthx/__version__.py
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 aioauthx-0.1.0/aioauthx/auth.py
--rw-r--r--   0        0        0     5202 2020-02-02 00:00:00.000000 aioauthx-0.1.0/aioauthx/client_reqrep.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aioauthx-0.1.0/aioauthx/flows/__init__.py
--rw-r--r--   0        0        0     8050 2020-02-02 00:00:00.000000 aioauthx-0.1.0/aioauthx/flows/negotiate.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 aioauthx-0.1.0/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 aioauthx-0.1.0/LICENSE
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 aioauthx-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 aioauthx-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 aioauthx-0.1.1/README.md
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 aioauthx-0.1.1/aioauthx/__init__.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 aioauthx-0.1.1/aioauthx/__version__.py
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 aioauthx-0.1.1/aioauthx/auth.py
+-rw-r--r--   0        0        0     5202 2020-02-02 00:00:00.000000 aioauthx-0.1.1/aioauthx/client_reqrep.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aioauthx-0.1.1/aioauthx/flows/__init__.py
+-rw-r--r--   0        0        0     8045 2020-02-02 00:00:00.000000 aioauthx-0.1.1/aioauthx/flows/negotiate.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 aioauthx-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 aioauthx-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 aioauthx-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 aioauthx-0.1.1/PKG-INFO
```

### Comparing `aioauthx-0.1.0/README.md` & `aioauthx-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `aioauthx-0.1.0/aioauthx/auth.py` & `aioauthx-0.1.1/aioauthx/auth.py`

 * *Files identical despite different names*

### Comparing `aioauthx-0.1.0/aioauthx/client_reqrep.py` & `aioauthx-0.1.1/aioauthx/client_reqrep.py`

 * *Files identical despite different names*

### Comparing `aioauthx-0.1.0/aioauthx/flows/negotiate.py` & `aioauthx-0.1.1/aioauthx/flows/negotiate.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         if username is not None:
             auth_info = (username, domain, password)
         self._auth_info = auth_info
         self._service = service
         self._delegate = delegate
         self._opportunistic_auth = opportunistic_auth
 
-    async def auth_flow(
+    async def flow(
         self,
         request: ClientRequest,
         connection: Connection
     ) -> AsyncGenerator[None, ClientResponse]:
         """Implementation of the Negotiate/NTLM challenge-response authentication
         protocol.
         """
```

### Comparing `aioauthx-0.1.0/.gitignore` & `aioauthx-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `aioauthx-0.1.0/LICENSE` & `aioauthx-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aioauthx-0.1.0/pyproject.toml` & `aioauthx-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aioauthx-0.1.0/PKG-INFO` & `aioauthx-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioauthx
-Version: 0.1.0
+Version: 0.1.1
 Summary: HTTPX-style authorization schemes for aiohttp.
 Project-URL: Changelog, https://github.com/newvicx/aioauthx/blob/master/CHANGELOG.md
 Project-URL: Homepage, https://github.com/newvicx/aioauthx
 Project-URL: Source, https://github.com/newvicx/aioauthx
 Author-email: Chris Newville <chrisnewville1396@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
```

