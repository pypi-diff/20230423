# Comparing `tmp/langcorn-0.0.5.tar.gz` & `tmp/langcorn-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langcorn-0.0.5.tar", max compression
+gzip compressed data, was "langcorn-0.0.6.tar", max compression
```

## Comparing `langcorn-0.0.5.tar` & `langcorn-0.0.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1088 2023-04-18 11:39:47.784152 langcorn-0.0.5/LICENSE
--rw-r--r--   0        0        0     4847 2023-04-18 11:39:47.784152 langcorn-0.0.5/Readme.md
--rw-r--r--   0        0        0       77 2023-04-18 11:39:47.784152 langcorn-0.0.5/langcorn/__init__.py
--rw-r--r--   0        0        0      417 2023-04-18 11:39:47.784152 langcorn-0.0.5/langcorn/__main__.py
--rw-r--r--   0        0        0        0 2023-04-18 11:39:47.784152 langcorn-0.0.5/langcorn/server/__init__.py
--rw-r--r--   0        0        0     3156 2023-04-18 11:39:47.784152 langcorn-0.0.5/langcorn/server/api.py
--rw-r--r--   0        0        0      825 2023-04-18 11:39:47.784152 langcorn-0.0.5/langcorn/server/test_api.py
--rw-r--r--   0        0        0      944 2023-04-18 11:39:47.784152 langcorn-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     5829 1970-01-01 00:00:00.000000 langcorn-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-04-23 12:09:58.514611 langcorn-0.0.6/LICENSE
+-rw-r--r--   0        0        0     4936 2023-04-23 12:09:58.514611 langcorn-0.0.6/Readme.md
+-rw-r--r--   0        0        0       77 2023-04-23 12:09:58.514611 langcorn-0.0.6/langcorn/__init__.py
+-rw-r--r--   0        0        0      417 2023-04-23 12:09:58.514611 langcorn-0.0.6/langcorn/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-23 12:09:58.514611 langcorn-0.0.6/langcorn/server/__init__.py
+-rw-r--r--   0        0        0     3156 2023-04-23 12:09:58.514611 langcorn-0.0.6/langcorn/server/api.py
+-rw-r--r--   0        0        0      825 2023-04-23 12:09:58.514611 langcorn-0.0.6/langcorn/server/test_api.py
+-rw-r--r--   0        0        0      944 2023-04-23 12:09:58.514611 langcorn-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     5918 1970-01-01 00:00:00.000000 langcorn-0.0.6/PKG-INFO
```

### Comparing `langcorn-0.0.5/LICENSE` & `langcorn-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `langcorn-0.0.5/Readme.md` & `langcorn-0.0.6/Readme.md`

 * *Files 4% similar despite different names*

```diff
@@ -117,16 +117,19 @@
 ```
 
 Now, your LangChain models and pipelines are accessible via the LangCorn API server.
 
 ## Docs
 
 Automatically served FastAPI doc
+[Live example](https://langcorn-ift9ub8zg-msoedov.vercel.app/docs#/) hosted on vercel.
+
 ![](https://res.cloudinary.com/dq0w2rtm9/image/upload/c_pad,b_auto:predominant,fl_preserve_transparency/v1681817836/Screen_Shot_2023-04-18_at_14.36.00_ms2thb.jpg?_s=public-apps)
 
+
 ## Auth
 
 It possible to add a static api token auth by specifying `auth_token`
 
 ```shell
 python langcorn server examples.ex1:chain examples.ex2:chain --auth_token=api-secret-value
 ```
```

### Comparing `langcorn-0.0.5/langcorn/server/api.py` & `langcorn-0.0.6/langcorn/server/api.py`

 * *Files identical despite different names*

### Comparing `langcorn-0.0.5/langcorn/server/test_api.py` & `langcorn-0.0.6/langcorn/server/test_api.py`

 * *Files identical despite different names*

### Comparing `langcorn-0.0.5/pyproject.toml` & `langcorn-0.0.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langcorn"
-version = "0.0.5"
+version = "0.0.6"
 description = "A Python package creating rest api interface for LangChain"
 authors = ["Alexander Miasoiedov <msoedov@gmail.com>"]
 maintainers = [
     "Alexander Miasoiedov <msoedov@gmail.com>",
 ]
 repository = "https://github.com/msoedov/langcorn"
 license = "MIT"
@@ -14,16 +14,16 @@
 
 
 [tool.poetry.scripts]
 langcorn = "langcorn.__main__:entrypoint"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-fastapi = "^0.92.0"
-uvicorn = "^0.20.0"
+fastapi = "^0.95.0"
+uvicorn = "^0.21.1"
 langchain = "^0.0.139"
 openai = "^0.27.2"
 fire = "^0.5.0"
 loguru = "^0.7.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
```

### Comparing `langcorn-0.0.5/PKG-INFO` & `langcorn-0.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: langcorn
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Python package creating rest api interface for LangChain
 Home-page: https://github.com/msoedov/langcorn
 License: MIT
 Keywords: nlp,langchain,openai,gpt,fastapi
 Author: Alexander Miasoiedov
 Author-email: msoedov@gmail.com
 Maintainer: Alexander Miasoiedov
 Maintainer-email: msoedov@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: fastapi (>=0.92.0,<0.93.0)
+Requires-Dist: fastapi (>=0.95.0,<0.96.0)
 Requires-Dist: fire (>=0.5.0,<0.6.0)
 Requires-Dist: langchain (>=0.0.139,<0.0.140)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: openai (>=0.27.2,<0.28.0)
-Requires-Dist: uvicorn (>=0.20.0,<0.21.0)
+Requires-Dist: uvicorn (>=0.21.1,<0.22.0)
 Project-URL: Repository, https://github.com/msoedov/langcorn
 Description-Content-Type: text/markdown
 
 # Langcorn
 
 LangCorn is an API server that enables you to serve LangChain models and pipelines with ease, leveraging the power of FastAPI for a robust and efficient experience.
 
@@ -143,16 +143,19 @@
 ```
 
 Now, your LangChain models and pipelines are accessible via the LangCorn API server.
 
 ## Docs
 
 Automatically served FastAPI doc
+[Live example](https://langcorn-ift9ub8zg-msoedov.vercel.app/docs#/) hosted on vercel.
+
 ![](https://res.cloudinary.com/dq0w2rtm9/image/upload/c_pad,b_auto:predominant,fl_preserve_transparency/v1681817836/Screen_Shot_2023-04-18_at_14.36.00_ms2thb.jpg?_s=public-apps)
 
+
 ## Auth
 
 It possible to add a static api token auth by specifying `auth_token`
 
 ```shell
 python langcorn server examples.ex1:chain examples.ex2:chain --auth_token=api-secret-value
 ```
```

