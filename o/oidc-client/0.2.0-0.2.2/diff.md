# Comparing `tmp/oidc_client-0.2.0.tar.gz` & `tmp/oidc_client-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oidc_client-0.2.0.tar", max compression
+gzip compressed data, was "oidc_client-0.2.2.tar", max compression
```

## Comparing `oidc_client-0.2.0.tar` & `oidc_client-0.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1085 2023-04-21 15:13:40.948593 oidc_client-0.2.0/LICENSE.md
--rw-r--r--   0        0        0     1069 2023-04-21 15:13:40.948593 oidc_client-0.2.0/README.md
--rw-r--r--   0        0        0      541 2023-04-21 15:13:40.948593 oidc_client-0.2.0/oidc_client/__init__.py
--rw-r--r--   0        0        0       30 2023-04-21 15:13:40.948593 oidc_client-0.2.0/oidc_client/__main__.py
--rw-r--r--   0        0        0     4925 2023-04-21 15:13:40.948593 oidc_client-0.2.0/oidc_client/cli.py
--rw-r--r--   0        0        0     3697 2023-04-21 15:13:40.948593 oidc_client-0.2.0/oidc_client/config.py
--rw-r--r--   0        0        0      925 2023-04-21 15:13:40.948593 oidc_client-0.2.0/oidc_client/discovery.py
--rw-r--r--   0        0        0      488 2023-04-21 15:13:40.948593 oidc_client-0.2.0/oidc_client/error.py
--rw-r--r--   0        0        0      215 2023-04-21 15:13:40.949594 oidc_client-0.2.0/oidc_client/index.html
--rw-r--r--   0        0        0     1882 2023-04-21 15:13:40.949594 oidc_client-0.2.0/oidc_client/lib.py
--rw-r--r--   0        0        0     1123 2023-04-21 15:13:40.949594 oidc_client-0.2.0/oidc_client/localhost.crt
--rw-r--r--   0        0        0     1704 2023-04-21 15:13:40.949594 oidc_client-0.2.0/oidc_client/localhost.key
--rw-r--r--   0        0        0     7656 2023-04-21 15:13:40.949594 oidc_client-0.2.0/oidc_client/oauth.py
--rw-r--r--   0        0        0      807 2023-04-21 15:13:40.949594 oidc_client-0.2.0/oidc_client/pkce.py
--rw-r--r--   0        0        0      556 2023-04-21 15:13:40.949594 oidc_client-0.2.0/oidc_client/tls.py
--rw-r--r--   0        0        0     1320 2023-04-21 15:13:40.949594 oidc_client-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1946 1970-01-01 00:00:00.000000 oidc_client-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-04-23 20:54:47.993720 oidc_client-0.2.2/LICENSE.md
+-rw-r--r--   0        0        0     1069 2023-04-23 20:54:47.993720 oidc_client-0.2.2/README.md
+-rw-r--r--   0        0        0      541 2023-04-23 20:54:47.993720 oidc_client-0.2.2/oidc_client/__init__.py
+-rw-r--r--   0        0        0       30 2023-04-23 20:54:47.993720 oidc_client-0.2.2/oidc_client/__main__.py
+-rw-r--r--   0        0        0     4925 2023-04-23 20:54:47.993720 oidc_client-0.2.2/oidc_client/cli.py
+-rw-r--r--   0        0        0     3717 2023-04-23 20:54:47.993720 oidc_client-0.2.2/oidc_client/config.py
+-rw-r--r--   0        0        0      925 2023-04-23 20:54:47.993720 oidc_client-0.2.2/oidc_client/discovery.py
+-rw-r--r--   0        0        0      488 2023-04-23 20:54:47.993720 oidc_client-0.2.2/oidc_client/error.py
+-rw-r--r--   0        0        0      215 2023-04-23 20:54:47.993720 oidc_client-0.2.2/oidc_client/index.html
+-rw-r--r--   0        0        0     1748 2023-04-23 20:54:47.993720 oidc_client-0.2.2/oidc_client/lib.py
+-rw-r--r--   0        0        0     1123 2023-04-23 20:54:47.993720 oidc_client-0.2.2/oidc_client/localhost.crt
+-rw-r--r--   0        0        0     1704 2023-04-23 20:54:47.994720 oidc_client-0.2.2/oidc_client/localhost.key
+-rw-r--r--   0        0        0     8471 2023-04-23 20:54:47.994720 oidc_client-0.2.2/oidc_client/oauth.py
+-rw-r--r--   0        0        0      807 2023-04-23 20:54:47.994720 oidc_client-0.2.2/oidc_client/pkce.py
+-rw-r--r--   0        0        0      556 2023-04-23 20:54:47.994720 oidc_client-0.2.2/oidc_client/tls.py
+-rw-r--r--   0        0        0     1320 2023-04-23 20:54:47.994720 oidc_client-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1946 1970-01-01 00:00:00.000000 oidc_client-0.2.2/PKG-INFO
```

### Comparing `oidc_client-0.2.0/LICENSE.md` & `oidc_client-0.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `oidc_client-0.2.0/README.md` & `oidc_client-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `oidc_client-0.2.0/oidc_client/__init__.py` & `oidc_client-0.2.2/oidc_client/__init__.py`

 * *Files identical despite different names*

### Comparing `oidc_client-0.2.0/oidc_client/cli.py` & `oidc_client-0.2.2/oidc_client/cli.py`

 * *Files identical despite different names*

### Comparing `oidc_client-0.2.0/oidc_client/config.py` & `oidc_client-0.2.2/oidc_client/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from urllib.parse import urlparse
 
 from .error import ProviderConfigError
 
 # FIXME: type-check when we drop support for Python 3.10
 try:
     import tomllib
-except ImportError:
+except ImportError:  # pragma: no cover
     import toml as tomllib  # type: ignore
 
 DEFAULT_CONFIG_FILE = "pyproject.toml"
 
 DEFAULT_OIDC_SCOPE = "openid profile email"
 DEFAULT_REDIRECT_URI = "http://127.0.0.1:39303/oauth2/callback"
```

### Comparing `oidc_client-0.2.0/oidc_client/discovery.py` & `oidc_client-0.2.2/oidc_client/discovery.py`

 * *Files identical despite different names*

### Comparing `oidc_client-0.2.0/oidc_client/lib.py` & `oidc_client-0.2.2/oidc_client/lib.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,11 @@
 """High level OpenID Connect login helper."""
 from .config import DEFAULT_OIDC_SCOPE, ProviderConfig
 from .error import TokenRequestParamError
-from .oauth import (
-    GrantType,
-    TokenResponse,
-    fetch_token,
-    handle_authorization_code,
-    start_authorization_code_flow,
-)
+from .oauth import GrantType, TokenResponse, fetch_token, start_authorization_code_flow
 from .pkce import PKCESecret
 
 
 def login(
     provider_config: ProviderConfig,
     client_id: str,
     client_secret: str | None = None,
@@ -27,22 +21,21 @@
     if interactive:
         if not redirect_uri:
             raise TokenRequestParamError(
                 "redirect_uri must be provided for interactive login."
             )
 
         pkce_secret = PKCESecret()
-        state = start_authorization_code_flow(
+        code = start_authorization_code_flow(
             provider_config.authorization_endpoint,
             client_id=client_id,
             redirect_uri=redirect_uri,
             scope=scope,
             pkce_secret=pkce_secret,
         )
-        code = handle_authorization_code(state=state, redirect_uri=redirect_uri)
         return fetch_token(
             provider_config.token_endpoint,
             grant_type=GrantType.AUTHORIZATION_CODE,
             client_id=client_id,
             redirect_uri=redirect_uri,
             code=code,
             pkce_secret=pkce_secret,
```

### Comparing `oidc_client-0.2.0/oidc_client/localhost.crt` & `oidc_client-0.2.2/oidc_client/localhost.crt`

 * *Files identical despite different names*

### Comparing `oidc_client-0.2.0/oidc_client/localhost.key` & `oidc_client-0.2.2/oidc_client/localhost.key`

 * *Files identical despite different names*

### Comparing `oidc_client-0.2.0/oidc_client/oauth.py` & `oidc_client-0.2.2/oidc_client/oauth.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,34 +6,38 @@
 import random
 import string
 import webbrowser
 from dataclasses import dataclass, fields
 from http import HTTPStatus
 from http.server import BaseHTTPRequestHandler, HTTPServer
 from importlib.resources import files
+from socket import socket
 from typing import cast
 from urllib.error import HTTPError
 from urllib.parse import parse_qs, urlencode, urlparse
 from urllib.request import Request, urlopen
 
 from .error import AuthorizationError, RedirectionError
 from .pkce import PKCESecret
 from .tls import setup_tls
 
 try:
     from enum import StrEnum
-except ImportError:
+except ImportError:  # pragma: no cover
     from strenum import StrEnum  # type: ignore
 
 
 class AuthorizationCodeHandler(BaseHTTPRequestHandler):
     """OAuth 2.1 authorization code flow (with PKCE) HTTP handler."""
 
     def __init__(
-        self, request: bytes, client_address: tuple[str, int], server: RedirectionServer
+        self,
+        request: socket | tuple[bytes, socket],
+        client_address: tuple[str, int],
+        server: RedirectionServer,
     ):
         # Required for type-checking the server object
         super().__init__(request, client_address, server)
 
     def log_message(self, *_: str) -> None:
         # Silence HTTP server logging to *stdout* and *stderr*
         pass
@@ -88,73 +92,94 @@
     """OAuth 2.1 authorization code flow (with PKCE) HTTP server."""
 
     def __init__(
         self,
         server_address: tuple[str, int],
         handler_class: type[AuthorizationCodeHandler],
         redirection_path: str,
-        state: str,
         tls: bool = False,
     ):
         super().__init__(server_address, handler_class)
 
-        self.redirection_path = redirection_path or "/"
-        self.state = state
-
         if tls:
             self.socket = setup_tls(self.socket)
 
+        self.redirection_path = redirection_path or "/"
+        self.state = base64.urlsafe_b64encode(
+            "".join(
+                random.choices(string.ascii_letters + string.digits + "-._~", k=32)
+            ).encode()
+        ).decode()
+
         self.code: str | None = None
         self.error: AuthorizationError | None = None
 
 
-def start_authorization_code_flow(
+def redirection_server(redirect_uri: str) -> RedirectionServer:
+    """Create a local HTTP server to handle an OAuth 2.1 authorization code redirect.
+
+    This factory allows us to create the server from just the redirect URI.
+    """
+    server_conf = urlparse(redirect_uri)
+
+    if not server_conf.hostname or not server_conf.port:
+        raise ValueError("cannot start redirection server without hostname and port.")
+
+    return RedirectionServer(
+        (server_conf.hostname, server_conf.port),
+        AuthorizationCodeHandler,
+        redirection_path=server_conf.path,
+        tls=server_conf.scheme == "https",
+    )
+
+
+def open_authorization_endpoint(
     endpoint: str,
     client_id: str,
     redirect_uri: str,
+    state: str,
     scope: str,
     pkce_secret: PKCESecret,
-) -> str:
-    """Start OAuth 2.1 authorization code flow (with PKCE).
-
-    Authorization code flow is interactive, this opens a web browser allowing a user to
-    log in.
-    """
-    state = base64.urlsafe_b64encode(
-        "".join(
-            random.choices(string.ascii_letters + string.digits + "-._~", k=32)
-        ).encode()
-    )
+) -> None:
+    """Direct the user agent to an OAuth 2.1 authorization server."""
     params = {
         "client_id": client_id,
         "redirect_uri": redirect_uri,
         "response_type": "code",
         "state": state,
         "scope": scope,
         "code_challenge": pkce_secret.challenge,
         "code_challenge_method": pkce_secret.challenge_method,
     }
     webbrowser.open(f"{endpoint}?{urlencode(params)}")
-    return state.decode()
-
 
-def handle_authorization_code(state: str, redirect_uri: str) -> str:
-    """Serve local HTTP server to handle the OAuth 2.1 authorization code redirect."""
-    server_conf = urlparse(redirect_uri)
 
-    if not server_conf.hostname or not server_conf.port:
-        raise ValueError("cannot start redirection server without hostname and port.")
+def start_authorization_code_flow(
+    endpoint: str,
+    client_id: str,
+    redirect_uri: str,
+    scope: str,
+    pkce_secret: PKCESecret,
+) -> str:
+    """Start OAuth 2.1 authorization code flow (with PKCE).
 
-    with RedirectionServer(
-        (server_conf.hostname, server_conf.port),
-        AuthorizationCodeHandler,
-        redirection_path=server_conf.path,
-        state=state,
-        tls=server_conf.scheme == "https",
-    ) as httpd:
+    Authorization code flow is interactive, this:
+    1. opens a web browser allowing a user to log in;
+    2. a local HTTP server handles the redirection from the authorization server and
+       accepts the authorization code (a temporary credential used to obtain tokens).
+    """
+    with redirection_server(redirect_uri) as httpd:
+        open_authorization_endpoint(
+            endpoint=endpoint,
+            client_id=client_id,
+            redirect_uri=redirect_uri,
+            state=httpd.state,
+            scope=scope,
+            pkce_secret=pkce_secret,
+        )
         while not httpd.code and not httpd.error:
             httpd.handle_request()
         if httpd.error:
             raise httpd.error
         if not httpd.code:
             # This should not ever be reached.
             raise AuthorizationError(  # pragma: no cover
```

### Comparing `oidc_client-0.2.0/oidc_client/pkce.py` & `oidc_client-0.2.2/oidc_client/pkce.py`

 * *Files identical despite different names*

### Comparing `oidc_client-0.2.0/oidc_client/tls.py` & `oidc_client-0.2.2/oidc_client/tls.py`

 * *Files identical despite different names*

### Comparing `oidc_client-0.2.0/pyproject.toml` & `oidc_client-0.2.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oidc-client"
-version = "0.2.0"
+version = "0.2.2"
 description = "A pure-Python OpenID Connect client"
 readme = "README.md"
 keywords = ["openid", "oidc", "oauth", "oauth2"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Topic :: Internet :: WWW/HTTP",
@@ -19,22 +19,22 @@
 
 [tool.poetry.dependencies]
 python = "^3.10"
 toml = { version = "^0.10.2", allow-prereleases = true, python = "<3.11" }
 StrEnum = { version = "^0.4.10", allow-prereleases = true, python = "<3.11" }
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.1.3"
-flake8 = "^5.0.4"
-mypy = "^0.971"
-isort = "^5.10.1"
-black = "^22.6.0"
+pytest = "^7.3.1"
+flake8 = "^6.0.0"
+mypy = "^1.2.0"
+isort = "^5.12.0"
+black = "^23.3.0"
 types-toml = "^0.10.8"
-pytest-cov = "^3.0.0"
-pytest-asyncio = "^0.19.0"
+pytest-cov = "^4.0.0"
+pytest-asyncio = "^0.21.0"
 pytest-timeout = "^2.1.0"
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `oidc_client-0.2.0/PKG-INFO` & `oidc_client-0.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oidc-client
-Version: 0.2.0
+Version: 0.2.2
 Summary: A pure-Python OpenID Connect client
 Home-page: https://gitlab.com/lzinsou/oidc-client
 Keywords: openid,oidc,oauth,oauth2
 Author: Loris Zinsou
 Author-email: lzinsou@proton.me
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

