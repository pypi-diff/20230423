# Comparing `tmp/api-analytics-1.1.3.tar.gz` & `tmp/api-analytics-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "api-analytics-1.1.3.tar", last modified: Sun Apr 23 14:56:55 2023, max compression
+gzip compressed data, was "api-analytics-1.1.4.tar", last modified: Sun Apr 23 16:56:10 2023, max compression
```

## Comparing `api-analytics-1.1.3.tar` & `api-analytics-1.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 14:56:55.498891 api-analytics-1.1.3/
--rw-rw-rw-   0        0        0     1086 2023-04-07 09:42:03.000000 api-analytics-1.1.3/LICENSE
--rw-rw-rw-   0        0        0     7527 2023-04-23 14:56:55.494818 api-analytics-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     5598 2023-04-07 09:42:03.000000 api-analytics-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 14:56:55.427858 api-analytics-1.1.3/api_analytics/
--rw-rw-rw-   0        0        0        0 2022-11-27 20:29:30.000000 api-analytics-1.1.3/api_analytics/__init__.py
--rw-rw-rw-   0        0        0      944 2023-04-23 14:52:42.000000 api-analytics-1.1.3/api_analytics/core.py
--rw-rw-rw-   0        0        0     1125 2023-04-03 19:32:20.000000 api-analytics-1.1.3/api_analytics/django.py
--rw-rw-rw-   0        0        0     1187 2023-04-03 19:32:20.000000 api-analytics-1.1.3/api_analytics/fastapi.py
--rw-rw-rw-   0        0        0     1194 2023-04-03 19:32:20.000000 api-analytics-1.1.3/api_analytics/flask.py
--rw-rw-rw-   0        0        0     1029 2023-04-03 19:32:20.000000 api-analytics-1.1.3/api_analytics/tornado.py
-drwxrwxrwx   0        0        0        0 2023-04-23 14:56:55.489819 api-analytics-1.1.3/api_analytics.egg-info/
--rw-rw-rw-   0        0        0     7527 2023-04-23 14:56:55.000000 api-analytics-1.1.3/api_analytics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      370 2023-04-23 14:56:55.000000 api-analytics-1.1.3/api_analytics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 14:56:55.000000 api-analytics-1.1.3/api_analytics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-04-23 14:56:55.000000 api-analytics-1.1.3/api_analytics.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-23 14:56:55.000000 api-analytics-1.1.3/api_analytics.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      853 2023-04-23 14:55:23.000000 api-analytics-1.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-23 14:56:55.499894 api-analytics-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0      668 2023-04-23 14:55:18.000000 api-analytics-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 16:56:10.363572 api-analytics-1.1.4/
+-rw-rw-rw-   0        0        0     1086 2023-04-07 09:42:03.000000 api-analytics-1.1.4/LICENSE
+-rw-rw-rw-   0        0        0     7535 2023-04-23 16:56:10.362557 api-analytics-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5606 2023-04-23 16:52:47.000000 api-analytics-1.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 16:56:10.318565 api-analytics-1.1.4/api_analytics/
+-rw-rw-rw-   0        0        0        0 2022-11-27 20:29:30.000000 api-analytics-1.1.4/api_analytics/__init__.py
+-rw-rw-rw-   0        0        0      944 2023-04-23 15:33:46.000000 api-analytics-1.1.4/api_analytics/core.py
+-rw-rw-rw-   0        0        0     1125 2023-04-03 19:32:20.000000 api-analytics-1.1.4/api_analytics/django.py
+-rw-rw-rw-   0        0        0     1187 2023-04-03 19:32:20.000000 api-analytics-1.1.4/api_analytics/fastapi.py
+-rw-rw-rw-   0        0        0     1194 2023-04-03 19:32:20.000000 api-analytics-1.1.4/api_analytics/flask.py
+-rw-rw-rw-   0        0        0     1029 2023-04-03 19:32:20.000000 api-analytics-1.1.4/api_analytics/tornado.py
+drwxrwxrwx   0        0        0        0 2023-04-23 16:56:10.358561 api-analytics-1.1.4/api_analytics.egg-info/
+-rw-rw-rw-   0        0        0     7535 2023-04-23 16:56:10.000000 api-analytics-1.1.4/api_analytics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      370 2023-04-23 16:56:10.000000 api-analytics-1.1.4/api_analytics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 16:56:10.000000 api-analytics-1.1.4/api_analytics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-04-23 16:56:10.000000 api-analytics-1.1.4/api_analytics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-23 16:56:10.000000 api-analytics-1.1.4/api_analytics.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      853 2023-04-23 16:55:47.000000 api-analytics-1.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-23 16:56:10.364564 api-analytics-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      668 2023-04-23 16:55:44.000000 api-analytics-1.1.4/setup.py
```

### Comparing `api-analytics-1.1.3/LICENSE` & `api-analytics-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `api-analytics-1.1.3/PKG-INFO` & `api-analytics-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api-analytics
-Version: 1.1.3
+Version: 1.1.4
 Summary: Monitoring and analytics for Python API frameworks.
 Home-page: https://github.com/tom-draper/api-analytics
 Author: Tom Draper
 Author-email: Tom Draper <tomjdraper1@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tom Draper
@@ -72,15 +72,15 @@
 
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

### Comparing `api-analytics-1.1.3/README.md` & `api-analytics-1.1.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
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

### Comparing `api-analytics-1.1.3/api_analytics/core.py` & `api-analytics-1.1.4/api_analytics/core.py`

 * *Files identical despite different names*

### Comparing `api-analytics-1.1.3/api_analytics/django.py` & `api-analytics-1.1.4/api_analytics/django.py`

 * *Files identical despite different names*

### Comparing `api-analytics-1.1.3/api_analytics/fastapi.py` & `api-analytics-1.1.4/api_analytics/fastapi.py`

 * *Files identical despite different names*

### Comparing `api-analytics-1.1.3/api_analytics/flask.py` & `api-analytics-1.1.4/api_analytics/flask.py`

 * *Files identical despite different names*

### Comparing `api-analytics-1.1.3/api_analytics/tornado.py` & `api-analytics-1.1.4/api_analytics/tornado.py`

 * *Files identical despite different names*

### Comparing `api-analytics-1.1.3/api_analytics.egg-info/PKG-INFO` & `api-analytics-1.1.4/api_analytics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api-analytics
-Version: 1.1.3
+Version: 1.1.4
 Summary: Monitoring and analytics for Python API frameworks.
 Home-page: https://github.com/tom-draper/api-analytics
 Author: Tom Draper
 Author-email: Tom Draper <tomjdraper1@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tom Draper
@@ -72,15 +72,15 @@
 
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

### Comparing `api-analytics-1.1.3/pyproject.toml` & `api-analytics-1.1.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 dependencies = ["Django", "fastapi", "Flask", "tornado", "requests"]
 description = "Monitoring and analytics for Python API frameworks."
 keywords = ["analytics", "api", "dashboard", "django", "fastapi", "flask", "tornado", "middleware"]
 license = {file = "LICENSE"}
 name = "api-analytics"
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

### Comparing `api-analytics-1.1.3/setup.py` & `api-analytics-1.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 long_description = open("README.md").read()
 
 setup(
     name="api-analytics",
-    version="1.1.3",
+    version="1.1.4",
     author="Tom Draper",
     author_email="tomjdraper1@gmail.com",
     license="MIT",
     description="Monitoring and analytics for Python API frameworks.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/tom-draper/api-analytics",
```

