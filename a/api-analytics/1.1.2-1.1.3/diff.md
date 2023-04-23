# Comparing `tmp/api-analytics-1.1.2.tar.gz` & `tmp/api-analytics-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "api-analytics-1.1.2.tar", last modified: Fri Apr  7 09:10:38 2023, max compression
+gzip compressed data, was "api-analytics-1.1.3.tar", last modified: Sun Apr 23 14:56:55 2023, max compression
```

## Comparing `api-analytics-1.1.2.tar` & `api-analytics-1.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 09:10:38.426901 api-analytics-1.1.2/
--rw-rw-rw-   0        0        0     1086 2023-04-07 09:07:28.000000 api-analytics-1.1.2/LICENSE
--rw-rw-rw-   0        0        0     7534 2023-04-07 09:10:38.425783 api-analytics-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     5605 2023-04-07 09:06:53.000000 api-analytics-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-07 09:10:38.368781 api-analytics-1.1.2/api_analytics/
--rw-rw-rw-   0        0        0        0 2022-11-27 20:29:30.000000 api-analytics-1.1.2/api_analytics/__init__.py
--rw-rw-rw-   0        0        0      913 2023-04-07 08:45:34.000000 api-analytics-1.1.2/api_analytics/core.py
--rw-rw-rw-   0        0        0     1125 2023-04-03 19:32:20.000000 api-analytics-1.1.2/api_analytics/django.py
--rw-rw-rw-   0        0        0     1187 2023-04-03 19:32:20.000000 api-analytics-1.1.2/api_analytics/fastapi.py
--rw-rw-rw-   0        0        0     1194 2023-04-03 19:32:20.000000 api-analytics-1.1.2/api_analytics/flask.py
--rw-rw-rw-   0        0        0     1029 2023-04-03 19:32:20.000000 api-analytics-1.1.2/api_analytics/tornado.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:10:38.421767 api-analytics-1.1.2/api_analytics.egg-info/
--rw-rw-rw-   0        0        0     7534 2023-04-07 09:10:38.000000 api-analytics-1.1.2/api_analytics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      370 2023-04-07 09:10:38.000000 api-analytics-1.1.2/api_analytics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 09:10:38.000000 api-analytics-1.1.2/api_analytics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-04-07 09:10:38.000000 api-analytics-1.1.2/api_analytics.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-07 09:10:38.000000 api-analytics-1.1.2/api_analytics.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      853 2023-04-07 09:06:44.000000 api-analytics-1.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-07 09:10:38.426901 api-analytics-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      668 2023-04-07 09:06:41.000000 api-analytics-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 14:56:55.498891 api-analytics-1.1.3/
+-rw-rw-rw-   0        0        0     1086 2023-04-07 09:42:03.000000 api-analytics-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0     7527 2023-04-23 14:56:55.494818 api-analytics-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5598 2023-04-07 09:42:03.000000 api-analytics-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 14:56:55.427858 api-analytics-1.1.3/api_analytics/
+-rw-rw-rw-   0        0        0        0 2022-11-27 20:29:30.000000 api-analytics-1.1.3/api_analytics/__init__.py
+-rw-rw-rw-   0        0        0      944 2023-04-23 14:52:42.000000 api-analytics-1.1.3/api_analytics/core.py
+-rw-rw-rw-   0        0        0     1125 2023-04-03 19:32:20.000000 api-analytics-1.1.3/api_analytics/django.py
+-rw-rw-rw-   0        0        0     1187 2023-04-03 19:32:20.000000 api-analytics-1.1.3/api_analytics/fastapi.py
+-rw-rw-rw-   0        0        0     1194 2023-04-03 19:32:20.000000 api-analytics-1.1.3/api_analytics/flask.py
+-rw-rw-rw-   0        0        0     1029 2023-04-03 19:32:20.000000 api-analytics-1.1.3/api_analytics/tornado.py
+drwxrwxrwx   0        0        0        0 2023-04-23 14:56:55.489819 api-analytics-1.1.3/api_analytics.egg-info/
+-rw-rw-rw-   0        0        0     7527 2023-04-23 14:56:55.000000 api-analytics-1.1.3/api_analytics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      370 2023-04-23 14:56:55.000000 api-analytics-1.1.3/api_analytics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 14:56:55.000000 api-analytics-1.1.3/api_analytics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-04-23 14:56:55.000000 api-analytics-1.1.3/api_analytics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-23 14:56:55.000000 api-analytics-1.1.3/api_analytics.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      853 2023-04-23 14:55:23.000000 api-analytics-1.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-23 14:56:55.499894 api-analytics-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      668 2023-04-23 14:55:18.000000 api-analytics-1.1.3/setup.py
```

### Comparing `api-analytics-1.1.2/LICENSE` & `api-analytics-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `api-analytics-1.1.2/PKG-INFO` & `api-analytics-1.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api-analytics
-Version: 1.1.2
+Version: 1.1.3
 Summary: Monitoring and analytics for Python API frameworks.
 Home-page: https://github.com/tom-draper/api-analytics
 Author: Tom Draper
 Author-email: Tom Draper <tomjdraper1@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tom Draper
@@ -33,15 +33,15 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: build
 Provides-Extra: dev
 License-File: LICENSE
 
-# Python API Analytics
+# API Analytics
 
 A lightweight API analytics solution, complete with a dashboard.
 
 ## Getting Started
 
 ### 1. Generate an API key
```

### Comparing `api-analytics-1.1.2/README.md` & `api-analytics-1.1.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Python API Analytics
+# API Analytics
 
 A lightweight API analytics solution, complete with a dashboard.
 
 ## Getting Started
 
 ### 1. Generate an API key
```

### Comparing `api-analytics-1.1.2/api_analytics/core.py` & `api-analytics-1.1.3/api_analytics/core.py`

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

### Comparing `api-analytics-1.1.2/api_analytics/django.py` & `api-analytics-1.1.3/api_analytics/django.py`

 * *Files identical despite different names*

### Comparing `api-analytics-1.1.2/api_analytics/fastapi.py` & `api-analytics-1.1.3/api_analytics/fastapi.py`

 * *Files identical despite different names*

### Comparing `api-analytics-1.1.2/api_analytics/flask.py` & `api-analytics-1.1.3/api_analytics/flask.py`

 * *Files identical despite different names*

### Comparing `api-analytics-1.1.2/api_analytics/tornado.py` & `api-analytics-1.1.3/api_analytics/tornado.py`

 * *Files identical despite different names*

### Comparing `api-analytics-1.1.2/api_analytics.egg-info/PKG-INFO` & `api-analytics-1.1.3/api_analytics.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api-analytics
-Version: 1.1.2
+Version: 1.1.3
 Summary: Monitoring and analytics for Python API frameworks.
 Home-page: https://github.com/tom-draper/api-analytics
 Author: Tom Draper
 Author-email: Tom Draper <tomjdraper1@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tom Draper
@@ -33,15 +33,15 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: build
 Provides-Extra: dev
 License-File: LICENSE
 
-# Python API Analytics
+# API Analytics
 
 A lightweight API analytics solution, complete with a dashboard.
 
 ## Getting Started
 
 ### 1. Generate an API key
```

### Comparing `api-analytics-1.1.2/pyproject.toml` & `api-analytics-1.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 dependencies = ["Django", "fastapi", "Flask", "tornado", "requests"]
 description = "Monitoring and analytics for Python API frameworks."
 keywords = ["analytics", "api", "dashboard", "django", "fastapi", "flask", "tornado", "middleware"]
 license = {file = "LICENSE"}
 name = "api-analytics"
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

### Comparing `api-analytics-1.1.2/setup.py` & `api-analytics-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 long_description = open("README.md").read()
 
 setup(
     name="api-analytics",
-    version="1.1.2",
+    version="1.1.3",
     author="Tom Draper",
     author_email="tomjdraper1@gmail.com",
     license="MIT",
     description="Monitoring and analytics for Python API frameworks.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/tom-draper/api-analytics",
```

