# Comparing `tmp/tornado-analytics-1.1.2.tar.gz` & `tmp/tornado-analytics-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tornado-analytics-1.1.2.tar", last modified: Fri Apr  7 09:13:28 2023, max compression
+gzip compressed data, was "tornado-analytics-1.1.3.tar", last modified: Sun Apr 23 14:57:10 2023, max compression
```

## Comparing `tornado-analytics-1.1.2.tar` & `tornado-analytics-1.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 09:13:28.622589 tornado-analytics-1.1.2/
--rw-rw-rw-   0        0        0     1086 2023-04-07 09:07:38.000000 tornado-analytics-1.1.2/LICENSE
--rw-rw-rw-   0        0        0     6590 2023-04-07 09:13:28.620593 tornado-analytics-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     4679 2023-04-07 09:13:06.000000 tornado-analytics-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-07 09:13:28.570593 tornado-analytics-1.1.2/api_analytics/
--rw-rw-rw-   0        0        0        0 2022-12-06 23:56:29.000000 tornado-analytics-1.1.2/api_analytics/__init__.py
--rw-rw-rw-   0        0        0      913 2023-04-07 08:45:35.000000 tornado-analytics-1.1.2/api_analytics/core.py
--rw-rw-rw-   0        0        0     1029 2023-04-03 19:32:20.000000 tornado-analytics-1.1.2/api_analytics/tornado.py
--rw-rw-rw-   0        0        0      796 2023-04-07 09:07:43.000000 tornado-analytics-1.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-07 09:13:28.622589 tornado-analytics-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      622 2023-04-07 09:07:53.000000 tornado-analytics-1.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:13:28.616594 tornado-analytics-1.1.2/tornado_analytics.egg-info/
--rw-rw-rw-   0        0        0     6590 2023-04-07 09:13:28.000000 tornado-analytics-1.1.2/tornado_analytics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2023-04-07 09:13:28.000000 tornado-analytics-1.1.2/tornado_analytics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 09:13:28.000000 tornado-analytics-1.1.2/tornado_analytics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-04-07 09:13:28.000000 tornado-analytics-1.1.2/tornado_analytics.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-07 09:13:28.000000 tornado-analytics-1.1.2/tornado_analytics.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 14:57:10.387727 tornado-analytics-1.1.3/
+-rw-rw-rw-   0        0        0     1086 2023-04-07 09:42:03.000000 tornado-analytics-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0     6590 2023-04-23 14:57:10.385696 tornado-analytics-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4679 2023-04-07 09:42:03.000000 tornado-analytics-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 14:57:10.305831 tornado-analytics-1.1.3/api_analytics/
+-rw-rw-rw-   0        0        0        0 2022-12-06 23:56:29.000000 tornado-analytics-1.1.3/api_analytics/__init__.py
+-rw-rw-rw-   0        0        0      944 2023-04-23 14:52:58.000000 tornado-analytics-1.1.3/api_analytics/core.py
+-rw-rw-rw-   0        0        0     1029 2023-04-03 19:32:20.000000 tornado-analytics-1.1.3/api_analytics/tornado.py
+-rw-rw-rw-   0        0        0      796 2023-04-23 14:55:44.000000 tornado-analytics-1.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-23 14:57:10.387727 tornado-analytics-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      622 2023-04-23 14:55:41.000000 tornado-analytics-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 14:57:10.380644 tornado-analytics-1.1.3/tornado_analytics.egg-info/
+-rw-rw-rw-   0        0        0     6590 2023-04-23 14:57:10.000000 tornado-analytics-1.1.3/tornado_analytics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2023-04-23 14:57:10.000000 tornado-analytics-1.1.3/tornado_analytics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 14:57:10.000000 tornado-analytics-1.1.3/tornado_analytics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-04-23 14:57:10.000000 tornado-analytics-1.1.3/tornado_analytics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-23 14:57:10.000000 tornado-analytics-1.1.3/tornado_analytics.egg-info/top_level.txt
```

### Comparing `tornado-analytics-1.1.2/LICENSE` & `tornado-analytics-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tornado-analytics-1.1.2/PKG-INFO` & `tornado-analytics-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tornado-analytics
-Version: 1.1.2
+Version: 1.1.3
 Summary: Monitoring and analytics for Tornado applications.
 Home-page: https://github.com/tom-draper/api-analytics
 Author: Tom Draper
 Author-email: Tom Draper <tomjdraper1@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tom Draper
```

### Comparing `tornado-analytics-1.1.2/README.md` & `tornado-analytics-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `tornado-analytics-1.1.2/api_analytics/core.py` & `tornado-analytics-1.1.3/api_analytics/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-import requests
 import threading
 from datetime import datetime
+from typing import Dict, List
 
+import requests
 
 _requests = []
 _last_posted = datetime.now()
 
 
-def _post_requests(api_key: str, requests_data: list[dict], framework: str):
+def _post_requests(api_key: str, requests_data: List[Dict], framework: str):
     requests.post('https://www.apianalytics-server.com/api/log-request',
                   json={
                       'api_key': api_key,
                       'requests': requests_data,
                       'framework': framework
                   }, timeout=5)
 
 
-def log_request(api_key: str, request_data: dict, framework: str):
+def log_request(api_key: str, request_data: Dict, framework: str):
     if api_key == "" or api_key is None:
         return
     global _requests, _last_posted
     _requests.append(request_data)
     now = datetime.now()
     if (now - _last_posted).total_seconds() > 60.0:
         threading.Thread(target=_post_requests, args=(
```

### Comparing `tornado-analytics-1.1.2/api_analytics/tornado.py` & `tornado-analytics-1.1.3/api_analytics/tornado.py`

 * *Files identical despite different names*

### Comparing `tornado-analytics-1.1.2/pyproject.toml` & `tornado-analytics-1.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 dependencies = ["tornado", "requests"]
 description = "Monitoring and analytics for Tornado applications."
 keywords = ["analytics", "api", "dashboard", "tornado", "middleware"]
 license = {file = "LICENSE"}
 name = "tornado-analytics"
 readme = "README.md"
 requires-python = ">=3.7"
-version = "1.1.2"
+version = "1.1.3"
 
 [project.optional-dependencies]
 build = ["build", "twine"]
 dev = ["pytest"]
 
 [project.urls]
 repository = "https://github.com/tom-draper/api-analytics"
```

### Comparing `tornado-analytics-1.1.2/setup.py` & `tornado-analytics-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 long_description = open("README.md").read()
 
 setup(
     name="tornado-analytics",
-    version="1.1.2",
+    version="1.1.3",
     author="Tom Draper",
     author_email="tomjdraper1@gmail.com",
     license="MIT",
     description="Monitoring and analytics for Tornado applications.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/tom-draper/api-analytics",
```

### Comparing `tornado-analytics-1.1.2/tornado_analytics.egg-info/PKG-INFO` & `tornado-analytics-1.1.3/tornado_analytics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tornado-analytics
-Version: 1.1.2
+Version: 1.1.3
 Summary: Monitoring and analytics for Tornado applications.
 Home-page: https://github.com/tom-draper/api-analytics
 Author: Tom Draper
 Author-email: Tom Draper <tomjdraper1@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tom Draper
```

