# Comparing `tmp/fastapi-analytics-1.1.3.tar.gz` & `tmp/fastapi-analytics-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-analytics-1.1.3.tar", last modified: Sun Apr 23 14:55:32 2023, max compression
+gzip compressed data, was "fastapi-analytics-1.1.4.tar", last modified: Sun Apr 23 16:54:58 2023, max compression
```

## Comparing `fastapi-analytics-1.1.3.tar` & `fastapi-analytics-1.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 14:55:32.356880 fastapi-analytics-1.1.3/
--rw-rw-rw-   0        0        0     1086 2023-04-07 09:42:03.000000 fastapi-analytics-1.1.3/LICENSE
--rw-rw-rw-   0        0        0     6182 2023-04-23 14:55:32.354875 fastapi-analytics-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     4271 2023-04-07 09:42:03.000000 fastapi-analytics-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 14:55:32.296881 fastapi-analytics-1.1.3/api_analytics/
--rw-rw-rw-   0        0        0        0 2022-11-27 20:29:30.000000 fastapi-analytics-1.1.3/api_analytics/__init__.py
--rw-rw-rw-   0        0        0      944 2023-04-23 14:52:30.000000 fastapi-analytics-1.1.3/api_analytics/core.py
--rw-rw-rw-   0        0        0     1187 2023-04-03 19:32:20.000000 fastapi-analytics-1.1.3/api_analytics/fastapi.py
-drwxrwxrwx   0        0        0        0 2023-04-23 14:55:32.352885 fastapi-analytics-1.1.3/fastapi_analytics.egg-info/
--rw-rw-rw-   0        0        0     6182 2023-04-23 14:55:32.000000 fastapi-analytics-1.1.3/fastapi_analytics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2023-04-23 14:55:32.000000 fastapi-analytics-1.1.3/fastapi_analytics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 14:55:32.000000 fastapi-analytics-1.1.3/fastapi_analytics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-04-23 14:55:32.000000 fastapi-analytics-1.1.3/fastapi_analytics.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-23 14:55:32.000000 fastapi-analytics-1.1.3/fastapi_analytics.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      796 2023-04-23 14:54:35.000000 fastapi-analytics-1.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-23 14:55:32.356880 fastapi-analytics-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0      622 2023-04-23 14:54:31.000000 fastapi-analytics-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 16:54:58.287361 fastapi-analytics-1.1.4/
+-rw-rw-rw-   0        0        0     1086 2023-04-07 09:42:03.000000 fastapi-analytics-1.1.4/LICENSE
+-rw-rw-rw-   0        0        0     6190 2023-04-23 16:54:58.285359 fastapi-analytics-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4279 2023-04-23 16:52:31.000000 fastapi-analytics-1.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 16:54:58.236355 fastapi-analytics-1.1.4/api_analytics/
+-rw-rw-rw-   0        0        0        0 2022-11-27 20:29:30.000000 fastapi-analytics-1.1.4/api_analytics/__init__.py
+-rw-rw-rw-   0        0        0      944 2023-04-23 15:33:46.000000 fastapi-analytics-1.1.4/api_analytics/core.py
+-rw-rw-rw-   0        0        0     1187 2023-04-03 19:32:20.000000 fastapi-analytics-1.1.4/api_analytics/fastapi.py
+drwxrwxrwx   0        0        0        0 2023-04-23 16:54:58.283395 fastapi-analytics-1.1.4/fastapi_analytics.egg-info/
+-rw-rw-rw-   0        0        0     6190 2023-04-23 16:54:58.000000 fastapi-analytics-1.1.4/fastapi_analytics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2023-04-23 16:54:58.000000 fastapi-analytics-1.1.4/fastapi_analytics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 16:54:58.000000 fastapi-analytics-1.1.4/fastapi_analytics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-04-23 16:54:58.000000 fastapi-analytics-1.1.4/fastapi_analytics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-23 16:54:58.000000 fastapi-analytics-1.1.4/fastapi_analytics.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      796 2023-04-23 16:54:35.000000 fastapi-analytics-1.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-23 16:54:58.287361 fastapi-analytics-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      622 2023-04-23 16:54:33.000000 fastapi-analytics-1.1.4/setup.py
```

### Comparing `fastapi-analytics-1.1.3/LICENSE` & `fastapi-analytics-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-analytics-1.1.3/PKG-INFO` & `fastapi-analytics-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-analytics
-Version: 1.1.3
+Version: 1.1.4
 Summary: Monitoring and analytics for FastAPI applications.
 Home-page: https://github.com/tom-draper/api-analytics
 Author: Tom Draper
 Author-email: Tom Draper <tomjdraper1@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tom Draper
@@ -57,15 +57,15 @@
 
 ```py
 import uvicorn
 from fastapi import FastAPI
 from api_analytics.fastapi import Analytics
 
 app = FastAPI()
-app.add_middleware(Analytics, <API-KEY>)  # Add middleware
+app.add_middleware(Analytics, api_key=<API-KEY>)  # Add middleware
 
 @app.get("/")
 async def root():
     return {"message": "Hello World"}
 
 if __name__ == "__main__":
     uvicorn.run("app:app", reload=True)
```

### Comparing `fastapi-analytics-1.1.3/README.md` & `fastapi-analytics-1.1.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 ```py
 import uvicorn
 from fastapi import FastAPI
 from api_analytics.fastapi import Analytics
 
 app = FastAPI()
-app.add_middleware(Analytics, <API-KEY>)  # Add middleware
+app.add_middleware(Analytics, api_key=<API-KEY>)  # Add middleware
 
 @app.get("/")
 async def root():
     return {"message": "Hello World"}
 
 if __name__ == "__main__":
     uvicorn.run("app:app", reload=True)
```

### Comparing `fastapi-analytics-1.1.3/api_analytics/core.py` & `fastapi-analytics-1.1.4/api_analytics/core.py`

 * *Files identical despite different names*

### Comparing `fastapi-analytics-1.1.3/api_analytics/fastapi.py` & `fastapi-analytics-1.1.4/api_analytics/fastapi.py`

 * *Files identical despite different names*

### Comparing `fastapi-analytics-1.1.3/fastapi_analytics.egg-info/PKG-INFO` & `fastapi-analytics-1.1.4/fastapi_analytics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-analytics
-Version: 1.1.3
+Version: 1.1.4
 Summary: Monitoring and analytics for FastAPI applications.
 Home-page: https://github.com/tom-draper/api-analytics
 Author: Tom Draper
 Author-email: Tom Draper <tomjdraper1@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tom Draper
@@ -57,15 +57,15 @@
 
 ```py
 import uvicorn
 from fastapi import FastAPI
 from api_analytics.fastapi import Analytics
 
 app = FastAPI()
-app.add_middleware(Analytics, <API-KEY>)  # Add middleware
+app.add_middleware(Analytics, api_key=<API-KEY>)  # Add middleware
 
 @app.get("/")
 async def root():
     return {"message": "Hello World"}
 
 if __name__ == "__main__":
     uvicorn.run("app:app", reload=True)
```

### Comparing `fastapi-analytics-1.1.3/pyproject.toml` & `fastapi-analytics-1.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 dependencies = ["fastapi", "requests"]
 description = "Monitoring and analytics for FastAPI applications."
 keywords = ["analytics", "api", "dashboard", "fastapi", "middleware"]
 license = {file = "LICENSE"}
 name = "fastapi-analytics"
 readme = "README.md"
 requires-python = ">=3.7"
-version = "1.1.3"
+version = "1.1.4"
 
 [project.optional-dependencies]
 build = ["build", "twine"]
 dev = ["pytest"]
 
 [project.urls]
 repository = "https://github.com/tom-draper/api-analytics"
```

### Comparing `fastapi-analytics-1.1.3/setup.py` & `fastapi-analytics-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 long_description = open("README.md").read()
 
 setup(
     name="fastapi-analytics",
-    version="1.1.3",
+    version="1.1.4",
     author="Tom Draper",
     author_email="tomjdraper1@gmail.com",
     license="MIT",
     description="Monitoring and analytics for FastAPI applications.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/tom-draper/api-analytics",
```

