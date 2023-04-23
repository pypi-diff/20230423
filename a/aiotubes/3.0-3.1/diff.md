# Comparing `tmp/aiotubes-3.0.tar.gz` & `tmp/aiotubes-3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiotubes-3.0.tar", last modified: Sun Apr 23 14:58:05 2023, max compression
+gzip compressed data, was "aiotubes-3.1.tar", last modified: Sun Apr 23 17:45:02 2023, max compression
```

## Comparing `aiotubes-3.0.tar` & `aiotubes-3.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 14:58:05.477006 aiotubes-3.0/
--rw-rw-rw-   0        0        0     1084 2022-10-11 08:30:57.000000 aiotubes-3.0/LICENSE
--rw-rw-rw-   0        0        0      697 2023-04-23 14:58:05.476009 aiotubes-3.0/PKG-INFO
--rw-rw-rw-   0        0        0      361 2023-04-23 14:57:43.000000 aiotubes-3.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-23 14:58:05.450077 aiotubes-3.0/aiotube/
--rw-rw-rw-   0        0        0       58 2023-04-23 14:53:51.000000 aiotubes-3.0/aiotube/__init__.py
--rw-rw-rw-   0        0        0     1762 2023-04-23 14:53:51.000000 aiotubes-3.0/aiotube/client.py
--rw-rw-rw-   0        0        0      994 2023-04-23 12:02:05.000000 aiotubes-3.0/aiotube/constants.py
--rw-rw-rw-   0        0        0     2511 2023-04-23 14:53:45.000000 aiotubes-3.0/aiotube/exceptions.py
--rw-rw-rw-   0        0        0     5405 2023-04-23 14:53:51.000000 aiotubes-3.0/aiotube/extractors.py
--rw-rw-rw-   0        0        0     1487 2023-02-24 20:59:01.000000 aiotubes-3.0/aiotube/helpers.py
--rw-rw-rw-   0        0        0     4427 2023-02-24 13:57:51.000000 aiotubes-3.0/aiotube/itags.py
--rw-rw-rw-   0        0        0     2226 2023-04-23 14:53:51.000000 aiotubes-3.0/aiotube/playlist.py
--rw-rw-rw-   0        0        0     8021 2023-04-23 14:53:51.000000 aiotubes-3.0/aiotube/streams.py
--rw-rw-rw-   0        0        0     5029 2023-04-23 14:53:51.000000 aiotubes-3.0/aiotube/video.py
-drwxrwxrwx   0        0        0        0 2023-04-23 14:58:05.475035 aiotubes-3.0/aiotubes.egg-info/
--rw-rw-rw-   0        0        0      697 2023-04-23 14:58:05.000000 aiotubes-3.0/aiotubes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-04-23 14:58:05.000000 aiotubes-3.0/aiotubes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 14:58:05.000000 aiotubes-3.0/aiotubes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-23 14:58:05.000000 aiotubes-3.0/aiotubes.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-23 14:58:05.000000 aiotubes-3.0/aiotubes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 14:58:05.477006 aiotubes-3.0/setup.cfg
--rw-rw-rw-   0        0        0      666 2023-04-23 14:51:17.000000 aiotubes-3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 17:45:02.854676 aiotubes-3.1/
+-rw-rw-rw-   0        0        0     1084 2022-10-11 08:30:57.000000 aiotubes-3.1/LICENSE
+-rw-rw-rw-   0        0        0      697 2023-04-23 17:45:02.853677 aiotubes-3.1/PKG-INFO
+-rw-rw-rw-   0        0        0      361 2023-04-23 14:57:43.000000 aiotubes-3.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-23 17:45:02.827747 aiotubes-3.1/aiotube/
+-rw-rw-rw-   0        0        0       58 2023-04-23 14:53:51.000000 aiotubes-3.1/aiotube/__init__.py
+-rw-rw-rw-   0        0        0     1766 2023-04-23 17:42:57.000000 aiotubes-3.1/aiotube/client.py
+-rw-rw-rw-   0        0        0      994 2023-04-23 12:02:05.000000 aiotubes-3.1/aiotube/constants.py
+-rw-rw-rw-   0        0        0     2511 2023-04-23 14:53:45.000000 aiotubes-3.1/aiotube/exceptions.py
+-rw-rw-rw-   0        0        0     5405 2023-04-23 14:53:51.000000 aiotubes-3.1/aiotube/extractors.py
+-rw-rw-rw-   0        0        0     1487 2023-02-24 20:59:01.000000 aiotubes-3.1/aiotube/helpers.py
+-rw-rw-rw-   0        0        0     4427 2023-02-24 13:57:51.000000 aiotubes-3.1/aiotube/itags.py
+-rw-rw-rw-   0        0        0     2226 2023-04-23 14:53:51.000000 aiotubes-3.1/aiotube/playlist.py
+-rw-rw-rw-   0        0        0     8051 2023-04-23 17:42:43.000000 aiotubes-3.1/aiotube/streams.py
+-rw-rw-rw-   0        0        0     5029 2023-04-23 14:53:51.000000 aiotubes-3.1/aiotube/video.py
+drwxrwxrwx   0        0        0        0 2023-04-23 17:45:02.852681 aiotubes-3.1/aiotubes.egg-info/
+-rw-rw-rw-   0        0        0      697 2023-04-23 17:45:02.000000 aiotubes-3.1/aiotubes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-04-23 17:45:02.000000 aiotubes-3.1/aiotubes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 17:45:02.000000 aiotubes-3.1/aiotubes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-23 17:45:02.000000 aiotubes-3.1/aiotubes.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-23 17:45:02.000000 aiotubes-3.1/aiotubes.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 17:45:02.854676 aiotubes-3.1/setup.cfg
+-rw-rw-rw-   0        0        0      666 2023-04-23 17:44:53.000000 aiotubes-3.1/setup.py
```

### Comparing `aiotubes-3.0/LICENSE` & `aiotubes-3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiotubes-3.0/PKG-INFO` & `aiotubes-3.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotubes
-Version: 3.0
+Version: 3.1
 Summary: Asynchronous Youtube API
 Home-page: https://github.com/sheldygg/aiotube
 Author: sheldy
 License: MIT
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

### Comparing `aiotubes-3.0/aiotube/client.py` & `aiotubes-3.1/aiotube/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 
 
 class HttpMethod(Enum):
     GET = "GET"
     POST = "POST"
     PUT = "PUT"
     DELETE = "DELETE"
+    HEAD = "HEAD"
 
 
 class RequestClient:
     def __init__(self, client: str):
         self.context = default_clients[client]["context"]
         self.api_key = default_clients[client]["api_key"]
-        self.base_headers = {"User-Agent": "Mozilla/5.0", "accept-language": "en-US,en"}
 
     @property
     def base_params(self) -> dict:
         return {"key": self.api_key, "contentCheckOk": True, "racyCheckOk": True}
 
     @property
     def base_data(self) -> dict:
@@ -33,25 +33,26 @@
         self,
         method: HttpMethod,
         url: str,
         headers: dict = None,
         params: dict = None,
         data: dict = None,
     ):
+        base_headers = {"User-Agent": "Mozilla/5.0", "accept-language": "en-US,en"}
         if params:
             params = urlencode(params)
         if headers:
-            self.base_headers.update(headers)
+            base_headers.update(headers)
         if data:
             data = json.dumps(data)
         async with ClientSession() as session:
             async with session.request(
                 method=method.value,
                 url=url,
-                headers=self.base_headers,
+                headers=base_headers,
                 params=params,
                 data=data,
             ) as response:
                 headers = response.headers
                 try:
                     response_data = await response.json()
                 except ContentTypeError:
```

### Comparing `aiotubes-3.0/aiotube/constants.py` & `aiotubes-3.1/aiotube/constants.py`

 * *Files identical despite different names*

### Comparing `aiotubes-3.0/aiotube/exceptions.py` & `aiotubes-3.1/aiotube/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiotubes-3.0/aiotube/extractors.py` & `aiotubes-3.1/aiotube/extractors.py`

 * *Files identical despite different names*

### Comparing `aiotubes-3.0/aiotube/helpers.py` & `aiotubes-3.1/aiotube/helpers.py`

 * *Files identical despite different names*

### Comparing `aiotubes-3.0/aiotube/itags.py` & `aiotubes-3.1/aiotube/itags.py`

 * *Files identical despite different names*

### Comparing `aiotubes-3.0/aiotube/playlist.py` & `aiotubes-3.1/aiotube/playlist.py`

 * *Files identical despite different names*

### Comparing `aiotubes-3.0/aiotube/streams.py` & `aiotubes-3.1/aiotube/streams.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from datetime import datetime
 from io import BytesIO
 from typing import AsyncGenerator, Callable, List, Optional
 
 from pydantic import BaseModel, HttpUrl
 
-from .client import RequestClient
+from .client import RequestClient, HttpMethod
 from .extractors import mime_type_codec
 from .helpers import safe_filename, target_directory
 from .itags import get_format_profile
 
 
 class Stream(BaseModel, RequestClient):
     title: str
@@ -92,26 +92,26 @@
         """Whether the stream only contains video.
 
         :rtype: bool
         """
         return self.is_progressive or self.type == "video"
 
     async def filesize(self) -> int:
-        response = await self.request(method="HEAD", url=self.url)
+        response = await self.request(method=HttpMethod.HEAD, url=self.url)
         return int(response.get("headers", {}).get("Content-Length"))
 
     async def _download(self) -> AsyncGenerator[bytes, None]:
         default_range_size = 9437184
         file_size: int = default_range_size
         downloaded = 0
         while downloaded < file_size:
             stop_pos = min(downloaded + default_range_size, file_size) - 1
             range_header = f"bytes={downloaded}-{stop_pos}"
             request = await self.request(
-                method="GET", url=self.url, headers={"Range": range_header}
+                method=HttpMethod.GET, url=self.url, headers={"Range": range_header}
             )
             headers = request.get("headers")
             chunk = request.get("response")
             if file_size == default_range_size:
                 content_range = headers.get("Content-Range")
                 file_size = int(content_range.split("/")[1])
             downloaded += len(chunk)
```

### Comparing `aiotubes-3.0/aiotube/video.py` & `aiotubes-3.1/aiotube/video.py`

 * *Files identical despite different names*

### Comparing `aiotubes-3.0/aiotubes.egg-info/PKG-INFO` & `aiotubes-3.1/aiotubes.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotubes
-Version: 3.0
+Version: 3.1
 Summary: Asynchronous Youtube API
 Home-page: https://github.com/sheldygg/aiotube
 Author: sheldy
 License: MIT
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

### Comparing `aiotubes-3.0/setup.py` & `aiotubes-3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def get_description():
     with open('README.rst', 'r', encoding='utf-8') as f:
         return f.read()
 
 
 setuptools.setup(
     name="aiotubes",
-    version="3.0",
+    version="3.1",
     license='MIT',
     author="sheldy",
     description="Asynchronous Youtube API",
     url="https://github.com/sheldygg/aiotube",
     packages=setuptools.find_packages(),
     long_description_content_type='text/markdown',
     long_description=get_description(),
```

