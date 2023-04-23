# Comparing `tmp/nanoatp-0.3.1.tar.gz` & `tmp/nanoatp-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanoatp-0.3.1.tar", max compression
+gzip compressed data, was "nanoatp-0.3.2.tar", max compression
```

## Comparing `nanoatp-0.3.1.tar` & `nanoatp-0.3.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1067 2023-02-24 19:04:39.038224 nanoatp-0.3.1/LICENSE
--rw-r--r--   0        0        0     3417 2023-04-17 14:29:54.818051 nanoatp-0.3.1/README.md
--rw-r--r--   0        0        0      277 2023-04-17 14:16:19.116394 nanoatp-0.3.1/nanoatp/__init__.py
--rw-r--r--   0        0        0     8200 2023-04-17 10:53:06.448130 nanoatp-0.3.1/nanoatp/nanoatp.py
--rw-r--r--   0        0        0     3034 2023-04-16 15:21:42.774112 nanoatp-0.3.1/nanoatp/richtext.py
--rw-r--r--   0        0        0      922 2023-04-17 14:29:54.818439 nanoatp-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     4297 1970-01-01 00:00:00.000000 nanoatp-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-02-24 19:04:39.038224 nanoatp-0.3.2/LICENSE
+-rw-r--r--   0        0        0     4182 2023-04-23 09:33:59.603773 nanoatp-0.3.2/README.md
+-rw-r--r--   0        0        0      283 2023-04-23 09:33:59.605564 nanoatp-0.3.2/nanoatp/__init__.py
+-rw-r--r--   0        0        0     8539 2023-04-23 09:33:59.606360 nanoatp-0.3.2/nanoatp/bskyagent.py
+-rw-r--r--   0        0        0     3034 2023-04-23 09:09:57.876090 nanoatp-0.3.2/nanoatp/richtext.py
+-rw-r--r--   0        0        0      922 2023-04-23 09:33:59.607197 nanoatp-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     5062 1970-01-01 00:00:00.000000 nanoatp-0.3.2/PKG-INFO
```

### Comparing `nanoatp-0.3.1/LICENSE` & `nanoatp-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nanoatp-0.3.1/README.md` & `nanoatp-0.3.2/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,18 @@
 # nanoatp
 
+[![PyPI](https://img.shields.io/pypi/v/nanoatp?color=blue)](https://pypi.org/project/nanoatp/)
+[![GitHub License](https://img.shields.io/github/license/susumuota/nanoatp)](https://github.com/susumuota/nanoatp/blob/main/LICENSE)
+[![GitHub last commit](https://img.shields.io/github/last-commit/susumuota/nanoatp)](https://github.com/susumuota/nanoatp/commits)
+&emsp;
+EN |
+[JA](https://github-com.translate.goog/susumuota/nanoatp/blob/main/README.md?_x_tr_sl=en&_x_tr_tl=ja&_x_tr_hl=ja&_x_tr_pto=wapp) |
+[ES](https://github-com.translate.goog/susumuota/nanoatp/blob/main/README.md?_x_tr_sl=en&_x_tr_tl=es&_x_tr_hl=es&_x_tr_pto=wapp) |
+[ZH](https://github-com.translate.goog/susumuota/nanoatp/blob/main/README.md?_x_tr_sl=en&_x_tr_tl=zh-CN&_x_tr_hl=zh-CN&_x_tr_pto=wapp)
+
 A nano implementation of the AT Protocol (Authenticated Transfer Protocol) for Python.
 
 ## Getting started
 
 - First, install the package.
 
 ```bash
@@ -33,18 +42,18 @@
 # create a RichText
 rt = RichText("Hello @ota.bsky.social, check out this link: https://example.com")
 rt.detectFacets(agent)
 print(rt.facets)
 
 # upload an image
 image = agent.uploadImage("example.png")
-embed = {"$type": "app.bsky.embed.images#main", "images": [image]}
-record = {"text": rt.text, "facets": rt.facets, "embed": embed}
 
 # post it
+embed = {"$type": "app.bsky.embed.images#main", "images": [image]}
+record = {"text": rt.text, "facets": rt.facets, "embed": embed}
 response = agent.post(record)
 print(response)
 ```
 
 See [examples](https://github.com/susumuota/nanoatp/tree/main/examples) for more.
 
 ## Usage
@@ -140,8 +149,8 @@
 
 ## License
 
 MIT License. See [LICENSE](LICENSE) for details.
 
 ## Author
 
-Susumu Ota
+S. Ota
```

### Comparing `nanoatp-0.3.1/nanoatp/nanoatp.py` & `nanoatp-0.3.2/nanoatp/bskyagent.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # SPDX-FileCopyrightText: 2023 Susumu OTA <1632335+susumuota@users.noreply.github.com>
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
-import datetime
-import os
+from datetime import datetime, timezone
 from mimetypes import guess_type
+from os import getenv
 from typing import Any
 from urllib.parse import urlparse
 
 import requests
 
 
 # TODO: replace Any
@@ -19,59 +19,69 @@
         self.service = service
         self.requests = requests.Session()
         self.session: dict[str, str] = {}
         self.headers: dict[str, str] = {}
 
     def login(self, identifier: str = "", password: str = ""):
         """https://github.com/bluesky-social/atproto/blob/main/packages/api/src/agent.ts"""
-        id = identifier or os.getenv("ATP_IDENTIFIER") or ""
-        pw = password or os.getenv("ATP_PASSWORD") or ""
-        session = self.createSession(id, pw)
-        if not verifySession(session):
+        id = identifier or getenv("ATP_IDENTIFIER") or ""
+        pw = password or getenv("ATP_PASSWORD") or ""
+        session = self._server_createSession(id, pw)
+        if session.get("error") or not session.get("accessJwt"):
             self.session = {}
             self.headers = {}
             raise Exception(str(session))
         self.session = session
         accessJwt = self.session.get("accessJwt")
         self.headers = {"Authorization": f"Bearer {accessJwt}"}
         return self.session
 
     def getPost(self, repo: str, rkey: str, cid: str = "") -> dict[str, Any]:
         """https://github.com/bluesky-social/atproto/blob/main/packages/api/src/bsky-agent.ts"""
-        return self.getRecord(repo, "app.bsky.feed.post", rkey, cid)
+        return self._repo_getRecord(repo, "app.bsky.feed.post", rkey, cid)
 
     def post(self, record: dict[str, Any]):
         """https://github.com/bluesky-social/atproto/blob/main/packages/api/src/bsky-agent.ts"""
         if not self.session:
             raise Exception("Not logged in")
         if not record.get("createdAt"):
-            record.update({"createdAt": now()})
+            record.update({"createdAt": datetime.now(timezone.utc).isoformat().replace("+00:00", "Z")})
         if not record.get("$type"):
             record.update({"$type": "app.bsky.feed.post"})
         repo = self.session.get("did") or self.session.get("handle") or ""
-        return self.createRecord(repo, "app.bsky.feed.post", record)
+        return self._repo_createRecord(repo, "app.bsky.feed.post", record)
 
     def deletePost(self, postUri: str):
         """https://github.com/bluesky-social/atproto/blob/main/packages/api/src/bsky-agent.ts"""
         if not self.session:
             raise Exception("Not logged in")
-        repo, collection, rkey = parseUri(postUri)
+        repo, collection, rkey = parseAtUri(postUri)
         if not (repo and collection and rkey):
             raise Exception(f"Invalid postUrl format: {postUri}")
-        return self.deleteRecord(repo, collection, rkey)
+        return self._repo_deleteRecord(repo, collection, rkey)
+
+    def uploadBlob(self, data: bytes, encoding: str) -> dict[str, Any]:
+        """https://github.com/bluesky-social/atproto/blob/main/packages/api/src/agent.ts"""
+        if not self.session:
+            raise Exception("Not logged in")
+        return self._repo_uploadBlob(data, encoding)
+
+    def resolveHandle(self, handle: str):
+        """https://github.com/bluesky-social/atproto/blob/main/packages/api/src/agent.ts"""
+        return self._identity_resolveHandle(handle)
 
     def uploadImage(self, path: str, alt: str = "", encoding: str = ""):
         """https://github.com/bluesky-social/atproto/blob/main/lexicons/app/bsky/embed/images.json"""
         if not self.session:
             raise Exception("Not logged in")
         encoding = encoding or guess_type(path)[0] or "application/octet-stream"
         data = b""
         with open(path, "rb") as f:
             data = f.read()
-        response = self.uploadBlob(data, encoding)
+        response = self._repo_uploadBlob(data, encoding)
         blob: dict[str, str] = response.get("blob") or {}
         if blob is {}:
             raise Exception(str(response))
         image: dict[str, Any] = {
             "$type": "app.bsky.embed.images#image",
             "alt": alt,
             "image": {
@@ -79,21 +89,21 @@
                 "ref": blob.get("ref"),
                 "mimeType": blob.get("mimeType"),
                 "size": blob.get("size"),
             },
         }
         return image
 
-    def createSession(self, identifier: str, password: str) -> dict[str, Any]:
+    def _server_createSession(self, identifier: str, password: str) -> dict[str, Any]:
         """https://github.com/bluesky-social/atproto/blob/main/lexicons/com/atproto/server/createSession.json"""
         json = {"identifier": identifier, "password": password}
         response = self.requests.post(f"{self.service}/xrpc/com.atproto.server.createSession", json=json)
         return response.json()
 
-    def createRecord(
+    def _repo_createRecord(
         self,
         repo: str,
         collection: str,
         record: dict[str, Any],
         rkey: str = "",
         validate: bool = True,
         swapCommit: str = "",
@@ -104,36 +114,36 @@
         json.update({"validate": validate}) if not validate else None  # default is True
         json.update({"swapCommit": swapCommit}) if swapCommit != "" else None
         response = self.requests.post(
             f"{self.service}/xrpc/com.atproto.repo.createRecord", headers=self.headers, json=json
         )
         return response.json()
 
-    def getRecord(self, repo: str, collection: str, rkey: str, cid: str = "") -> dict[str, Any]:
+    def _repo_getRecord(self, repo: str, collection: str, rkey: str, cid: str = "") -> dict[str, Any]:
         """https://github.com/bluesky-social/atproto/blob/main/lexicons/com/atproto/repo/getRecord.json"""
         params = {"repo": repo, "collection": collection, "rkey": rkey}
         params.update({"cid": cid}) if cid != "" else None
         response = self.requests.get(
             f"{self.service}/xrpc/com.atproto.repo.getRecord", headers=self.headers, params=params
         )
         return response.json()
 
-    def deleteRecord(
+    def _repo_deleteRecord(
         self, repo: str, collection: str, rkey: str, swapRecord: str = "", swapCommit: str = ""
     ) -> requests.Response:
         """https://github.com/bluesky-social/atproto/blob/main/lexicons/com/atproto/repo/deleteRecord.json"""
         json = {"repo": repo, "collection": collection, "rkey": rkey}
         json.update({"swapRecord": swapRecord}) if swapRecord != "" else None
         json.update({"swapCommit": swapCommit}) if swapCommit != "" else None
         response = self.requests.post(
             f"{self.service}/xrpc/com.atproto.repo.deleteRecord", headers=self.headers, json=json
         )
         return response  # TODO
 
-    def listRecords(
+    def _repo_listRecords(
         self,
         repo: str,
         collection: str,
         limit: int = 50,
         cursor: str = "",
         rkeyStart: str = "",
         rkeyEnd: str = "",
@@ -147,39 +157,29 @@
         params.update({"rkeyEnd": rkeyEnd}) if rkeyEnd != "" else None
         params.update({"reverse": reverse}) if reverse else None  # default is False
         response = self.requests.get(
             f"{self.service}/xrpc/com.atproto.repo.listRecords", headers=self.headers, params=params
         )
         return response.json()
 
-    def uploadBlob(self, data: bytes, encoding: str) -> dict[str, Any]:
+    def _repo_uploadBlob(self, data: bytes, encoding: str) -> dict[str, Any]:
         """https://github.com/bluesky-social/atproto/blob/main/lexicons/com/atproto/repo/uploadBlob.json"""
         headers = {"Content-Type": encoding, "Content-Length": str(len(data))}
         headers.update(self.headers)
         response = self.requests.post(f"{self.service}/xrpc/com.atproto.repo.uploadBlob", headers=headers, data=data)
         return response.json()
 
-    def resolveHandle(self, handle: str):
+    def _identity_resolveHandle(self, handle: str):
         """https://github.com/bluesky-social/atproto/blob/main/lexicons/com/atproto/identity/resolveHandle.json"""
         params = {"handle": handle}
         response = self.requests.get(
             f"{self.service}/xrpc/com.atproto.identity.resolveHandle", headers=self.headers, params=params
         )
         return response.json()
 
 
-# TODO: create util.py?
-def verifySession(session: dict[str, str]):
-    """https://github.com/bluesky-social/atproto/blob/main/lexicons/com/atproto/server/createSession.json"""
-    # email is optional
-    return not session.get("error") and set(session.keys()).issuperset({"did", "handle", "accessJwt", "refreshJwt"})
-
-
-def now():
-    return datetime.datetime.now(datetime.timezone.utc).isoformat().replace("+00:00", "Z")
-
-
-def parseUri(uri: str):
+def parseAtUri(uri: str):
+    """https://github.com/bluesky-social/atproto/blob/main/packages/uri/src/index.ts"""
     u = urlparse(uri)
     repo = u.netloc
     _, collection, rkey = u.path.split("/")
     return repo, collection, rkey
```

### Comparing `nanoatp-0.3.1/nanoatp/richtext.py` & `nanoatp-0.3.2/nanoatp/richtext.py`

 * *Files identical despite different names*

### Comparing `nanoatp-0.3.1/pyproject.toml` & `nanoatp-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nanoatp"
-version = "0.3.1"
+version = "0.3.2"
 description = "A nano implementation of the AT Protocol (Authenticated Transfer Protocol) for Python."
 license = "MIT"
 authors = ["Susumu OTA <1632335+susumuota@users.noreply.github.com>"]
 readme = "README.md"
 homepage = "https://github.com/susumuota/nanoatp"
 repository = "https://github.com/susumuota/nanoatp"
 documentation = "https://github.com/susumuota/nanoatp#readme"
```

### Comparing `nanoatp-0.3.1/PKG-INFO` & `nanoatp-0.3.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanoatp
-Version: 0.3.1
+Version: 0.3.2
 Summary: A nano implementation of the AT Protocol (Authenticated Transfer Protocol) for Python.
 Home-page: https://github.com/susumuota/nanoatp
 License: MIT
 Keywords: atprotocol,atproto,bluesky
 Author: Susumu OTA
 Author-email: 1632335+susumuota@users.noreply.github.com
 Requires-Python: >=3.9.16,<4.0.0
@@ -17,14 +17,23 @@
 Requires-Dist: tld (>=0.13,<0.14)
 Project-URL: Documentation, https://github.com/susumuota/nanoatp#readme
 Project-URL: Repository, https://github.com/susumuota/nanoatp
 Description-Content-Type: text/markdown
 
 # nanoatp
 
+[![PyPI](https://img.shields.io/pypi/v/nanoatp?color=blue)](https://pypi.org/project/nanoatp/)
+[![GitHub License](https://img.shields.io/github/license/susumuota/nanoatp)](https://github.com/susumuota/nanoatp/blob/main/LICENSE)
+[![GitHub last commit](https://img.shields.io/github/last-commit/susumuota/nanoatp)](https://github.com/susumuota/nanoatp/commits)
+&emsp;
+EN |
+[JA](https://github-com.translate.goog/susumuota/nanoatp/blob/main/README.md?_x_tr_sl=en&_x_tr_tl=ja&_x_tr_hl=ja&_x_tr_pto=wapp) |
+[ES](https://github-com.translate.goog/susumuota/nanoatp/blob/main/README.md?_x_tr_sl=en&_x_tr_tl=es&_x_tr_hl=es&_x_tr_pto=wapp) |
+[ZH](https://github-com.translate.goog/susumuota/nanoatp/blob/main/README.md?_x_tr_sl=en&_x_tr_tl=zh-CN&_x_tr_hl=zh-CN&_x_tr_pto=wapp)
+
 A nano implementation of the AT Protocol (Authenticated Transfer Protocol) for Python.
 
 ## Getting started
 
 - First, install the package.
 
 ```bash
@@ -54,18 +63,18 @@
 # create a RichText
 rt = RichText("Hello @ota.bsky.social, check out this link: https://example.com")
 rt.detectFacets(agent)
 print(rt.facets)
 
 # upload an image
 image = agent.uploadImage("example.png")
-embed = {"$type": "app.bsky.embed.images#main", "images": [image]}
-record = {"text": rt.text, "facets": rt.facets, "embed": embed}
 
 # post it
+embed = {"$type": "app.bsky.embed.images#main", "images": [image]}
+record = {"text": rt.text, "facets": rt.facets, "embed": embed}
 response = agent.post(record)
 print(response)
 ```
 
 See [examples](https://github.com/susumuota/nanoatp/tree/main/examples) for more.
 
 ## Usage
@@ -161,9 +170,9 @@
 
 ## License
 
 MIT License. See [LICENSE](LICENSE) for details.
 
 ## Author
 
-Susumu Ota
+S. Ota
```

