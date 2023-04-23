# Comparing `tmp/secapi-tl-1.1.6.tar.gz` & `tmp/secapi-tl-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secapi-tl-1.1.6.tar", last modified: Fri Apr 21 14:39:16 2023, max compression
+gzip compressed data, was "secapi-tl-1.1.7.tar", last modified: Sun Apr 23 16:01:59 2023, max compression
```

## Comparing `secapi-tl-1.1.6.tar` & `secapi-tl-1.1.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-21 14:39:16.898633 secapi-tl-1.1.6/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1063 2022-10-14 12:06:38.000000 secapi-tl-1.1.6/LICENSE
--rw-rw-r--   0 tom       (1000) tom       (1000)     5137 2023-04-21 14:39:16.898633 secapi-tl-1.1.6/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)     3698 2023-04-09 10:03:28.000000 secapi-tl-1.1.6/README.md
--rw-rw-r--   0 tom       (1000) tom       (1000)      391 2023-04-21 14:37:12.000000 secapi-tl-1.1.6/pyproject.toml
--rw-rw-r--   0 tom       (1000) tom       (1000)       38 2023-04-21 14:39:16.898633 secapi-tl-1.1.6/setup.cfg
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-21 14:39:16.898633 secapi-tl-1.1.6/src/
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-21 14:39:16.898633 secapi-tl-1.1.6/src/secapi_tl/
--rw-rw-r--   0 tom       (1000) tom       (1000)      299 2023-04-08 12:35:48.000000 secapi-tl-1.1.6/src/secapi_tl/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     6136 2023-04-15 21:09:49.000000 secapi-tl-1.1.6/src/secapi_tl/filing.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4053 2023-04-15 16:38:29.000000 secapi-tl-1.1.6/src/secapi_tl/filing_query.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      989 2022-10-14 21:27:13.000000 secapi-tl-1.1.6/src/secapi_tl/key_mapper.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1377 2023-04-21 14:28:20.000000 secapi-tl-1.1.6/src/secapi_tl/request.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-21 14:39:16.898633 secapi-tl-1.1.6/src/secapi_tl.egg-info/
--rw-rw-r--   0 tom       (1000) tom       (1000)     5137 2023-04-21 14:39:16.000000 secapi-tl-1.1.6/src/secapi_tl.egg-info/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)      349 2023-04-21 14:39:16.000000 secapi-tl-1.1.6/src/secapi_tl.egg-info/SOURCES.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        1 2023-04-21 14:39:16.000000 secapi-tl-1.1.6/src/secapi_tl.egg-info/dependency_links.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       42 2023-04-21 14:39:16.000000 secapi-tl-1.1.6/src/secapi_tl.egg-info/requires.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       10 2023-04-21 14:39:16.000000 secapi-tl-1.1.6/src/secapi_tl.egg-info/top_level.txt
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-23 16:01:59.165676 secapi-tl-1.1.7/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1063 2022-10-14 12:06:38.000000 secapi-tl-1.1.7/LICENSE
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5137 2023-04-23 16:01:59.165676 secapi-tl-1.1.7/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3698 2023-04-09 10:03:28.000000 secapi-tl-1.1.7/README.md
+-rw-rw-r--   0 tom       (1000) tom       (1000)      391 2023-04-23 16:01:08.000000 secapi-tl-1.1.7/pyproject.toml
+-rw-rw-r--   0 tom       (1000) tom       (1000)       38 2023-04-23 16:01:59.165676 secapi-tl-1.1.7/setup.cfg
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-23 16:01:59.161676 secapi-tl-1.1.7/src/
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-23 16:01:59.165676 secapi-tl-1.1.7/src/secapi_tl/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      299 2023-04-08 12:35:48.000000 secapi-tl-1.1.7/src/secapi_tl/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     6136 2023-04-15 21:09:49.000000 secapi-tl-1.1.7/src/secapi_tl/filing.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4053 2023-04-15 16:38:29.000000 secapi-tl-1.1.7/src/secapi_tl/filing_query.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      989 2022-10-14 21:27:13.000000 secapi-tl-1.1.7/src/secapi_tl/key_mapper.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1175 2023-04-23 15:57:28.000000 secapi-tl-1.1.7/src/secapi_tl/request.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-23 16:01:59.165676 secapi-tl-1.1.7/src/secapi_tl.egg-info/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5137 2023-04-23 16:01:59.000000 secapi-tl-1.1.7/src/secapi_tl.egg-info/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)      349 2023-04-23 16:01:59.000000 secapi-tl-1.1.7/src/secapi_tl.egg-info/SOURCES.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)        1 2023-04-23 16:01:59.000000 secapi-tl-1.1.7/src/secapi_tl.egg-info/dependency_links.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       42 2023-04-23 16:01:59.000000 secapi-tl-1.1.7/src/secapi_tl.egg-info/requires.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       10 2023-04-23 16:01:59.000000 secapi-tl-1.1.7/src/secapi_tl.egg-info/top_level.txt
```

### Comparing `secapi-tl-1.1.6/LICENSE` & `secapi-tl-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `secapi-tl-1.1.6/PKG-INFO` & `secapi-tl-1.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secapi-tl
-Version: 1.1.6
+Version: 1.1.7
 License: MIT License
         
         Copyright (c) 2022 tlie03
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `secapi-tl-1.1.6/README.md` & `secapi-tl-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `secapi-tl-1.1.6/src/secapi_tl/filing.py` & `secapi-tl-1.1.7/src/secapi_tl/filing.py`

 * *Files identical despite different names*

### Comparing `secapi-tl-1.1.6/src/secapi_tl/filing_query.py` & `secapi-tl-1.1.7/src/secapi_tl/filing_query.py`

 * *Files identical despite different names*

### Comparing `secapi-tl-1.1.6/src/secapi_tl/key_mapper.py` & `secapi-tl-1.1.7/src/secapi_tl/key_mapper.py`

 * *Files identical despite different names*

### Comparing `secapi-tl-1.1.6/src/secapi_tl/request.py` & `secapi-tl-1.1.7/src/secapi_tl/request.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,34 +4,33 @@
 of requests stays in the boundaries set by the sec.
 
 The method was implemented as a static method of a class because
 an implementation as a normal function caused some issues
 by exceeding the request limits when used with threading.
 These issues disappeared with the implementation as a static method.
 """
-import time
-import math
 import requests
 from requests_random_user_agent import USER_AGENTS
 from random import choice
 from ratelimit import limits, sleep_and_retry
+from threading import Lock
 
 SEC_REQUEST_COUNT = 1
-SEC_PERIOD = 0.1
+SEC_PERIOD = 0.11
 
 
 class Request:
+    sec_request_lock = Lock()
 
     @staticmethod
     @sleep_and_retry
     @limits(calls=SEC_REQUEST_COUNT, period=SEC_PERIOD)
-    def sec_request(url: str, retries: int=5):
+    def sec_request(url: str):
         header = {"User-Agent": choice(USER_AGENTS)}
+
+        Request.sec_request_lock.acquire()
         response = requests.get(url=url, headers=header)
-        if response.status_code != 200 and retries > 0:
-            time.sleep(20 * (1 / math.exp(retries-1)))
-            response = Request.sec_request(url=url, retries=retries-1)
-
-        # raise Connection error on deepest function call if there was no successful response for all tries
-        if response.status_code != 200 and retries == 0:
-            raise ConnectionError(f"invalid response statuscode: {response.status_code}")
+        Request.sec_request_lock.release()
+
+        if response.status_code != 200:
+            raise ConnectionError(f"invalid response status code {response.status_code}")
         return response
```

### Comparing `secapi-tl-1.1.6/src/secapi_tl.egg-info/PKG-INFO` & `secapi-tl-1.1.7/src/secapi_tl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secapi-tl
-Version: 1.1.6
+Version: 1.1.7
 License: MIT License
         
         Copyright (c) 2022 tlie03
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

