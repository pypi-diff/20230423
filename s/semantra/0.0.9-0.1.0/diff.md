# Comparing `tmp/semantra-0.0.9.tar.gz` & `tmp/semantra-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantra-0.0.9.tar", last modified: Sun Apr 23 12:50:03 2023, max compression
+gzip compressed data, was "semantra-0.1.0.tar", last modified: Sun Apr 23 21:16:04 2023, max compression
```

## Comparing `semantra-0.0.9.tar` & `semantra-0.1.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 12:50:03.430593 semantra-0.0.9/
--rw-r--r--   0 freedmand   (501) staff       (20)     1071 2023-03-31 03:28:18.000000 semantra-0.0.9/LICENSE
--rw-r--r--   0 freedmand   (501) staff       (20)     3645 2023-04-23 12:50:03.430233 semantra-0.0.9/PKG-INFO
--rw-r--r--   0 freedmand   (501) staff       (20)     3102 2023-04-16 16:45:22.000000 semantra-0.0.9/README.md
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 12:50:03.414899 semantra-0.0.9/client/
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 12:50:03.416773 semantra-0.0.9/client/public/
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 12:50:03.418745 semantra-0.0.9/client/public/build/
--rw-r--r--   0 freedmand   (501) staff       (20)    14441 2023-04-22 21:42:14.000000 semantra-0.0.9/client/public/build/bundle.css
--rw-r--r--   0 freedmand   (501) staff       (20)   449074 2023-04-22 21:42:14.000000 semantra-0.0.9/client/public/build/bundle.js
--rw-r--r--   0 freedmand   (501) staff       (20)  1495716 2023-04-22 21:42:14.000000 semantra-0.0.9/client/public/build/bundle.js.map
--rw-r--r--   0 freedmand   (501) staff       (20)     3300 2023-04-09 04:23:49.000000 semantra-0.0.9/client/public/favicon.png
--rw-r--r--   0 freedmand   (501) staff       (20)      890 2023-02-15 22:52:41.000000 semantra-0.0.9/client/public/global.css
--rw-r--r--   0 freedmand   (501) staff       (20)      434 2023-04-09 20:49:05.000000 semantra-0.0.9/client/public/index.html
--rw-r--r--   0 freedmand   (501) staff       (20)      995 2023-04-23 12:48:41.000000 semantra-0.0.9/pyproject.toml
--rw-r--r--   0 freedmand   (501) staff       (20)       38 2023-04-23 12:50:03.430681 semantra-0.0.9/setup.cfg
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 12:50:03.415205 semantra-0.0.9/src/
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 12:50:03.422414 semantra-0.0.9/src/semantra/
--rw-r--r--   0 freedmand   (501) staff       (20)        0 2023-04-23 04:39:23.000000 semantra-0.0.9/src/semantra/__init__.py
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 12:50:03.425724 semantra-0.0.9/src/semantra/__pycache__/
--rw-r--r--   0 freedmand   (501) staff       (20)      148 2023-04-23 04:39:41.000000 semantra-0.0.9/src/semantra/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 freedmand   (501) staff       (20)    10961 2023-04-23 04:37:57.000000 semantra-0.0.9/src/semantra/__pycache__/models.cpython-39.pyc
--rw-r--r--   0 freedmand   (501) staff       (20)     3086 2023-04-23 04:37:58.000000 semantra-0.0.9/src/semantra/__pycache__/pdf.cpython-39.pyc
--rw-r--r--   0 freedmand   (501) staff       (20)    19561 2023-04-23 12:15:19.000000 semantra-0.0.9/src/semantra/__pycache__/semantra.cpython-39.pyc
--rw-r--r--   0 freedmand   (501) staff       (20)     4744 2023-04-23 04:37:58.000000 semantra-0.0.9/src/semantra/__pycache__/util.cpython-39.pyc
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 12:50:03.426299 semantra-0.0.9/src/semantra/client_public/
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 12:50:03.427832 semantra-0.0.9/src/semantra/client_public/build/
--rw-r--r--   0 freedmand   (501) staff       (20)    14441 2023-04-22 21:42:14.000000 semantra-0.0.9/src/semantra/client_public/build/bundle.css
--rw-r--r--   0 freedmand   (501) staff       (20)   449074 2023-04-22 21:42:14.000000 semantra-0.0.9/src/semantra/client_public/build/bundle.js
--rw-r--r--   0 freedmand   (501) staff       (20)  1495716 2023-04-22 21:42:14.000000 semantra-0.0.9/src/semantra/client_public/build/bundle.js.map
--rw-r--r--   0 freedmand   (501) staff       (20)     3300 2023-04-09 04:23:49.000000 semantra-0.0.9/src/semantra/client_public/favicon.png
--rw-r--r--   0 freedmand   (501) staff       (20)      890 2023-02-15 22:52:41.000000 semantra-0.0.9/src/semantra/client_public/global.css
--rw-r--r--   0 freedmand   (501) staff       (20)      434 2023-04-09 20:49:05.000000 semantra-0.0.9/src/semantra/client_public/index.html
--rw-r--r--   0 freedmand   (501) staff       (20)    11172 2023-04-20 17:02:30.000000 semantra-0.0.9/src/semantra/models.py
--rw-r--r--   0 freedmand   (501) staff       (20)     3118 2023-04-23 04:31:52.000000 semantra-0.0.9/src/semantra/pdf.py
--rw-r--r--   0 freedmand   (501) staff       (20)    28701 2023-04-23 12:49:54.000000 semantra-0.0.9/src/semantra/semantra.py
--rw-r--r--   0 freedmand   (501) staff       (20)     4524 2023-04-22 20:05:23.000000 semantra-0.0.9/src/semantra/util.py
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 12:50:03.423626 semantra-0.0.9/src/semantra.egg-info/
--rw-r--r--   0 freedmand   (501) staff       (20)     3645 2023-04-23 12:50:03.000000 semantra-0.0.9/src/semantra.egg-info/PKG-INFO
--rw-r--r--   0 freedmand   (501) staff       (20)     1018 2023-04-23 12:50:03.000000 semantra-0.0.9/src/semantra.egg-info/SOURCES.txt
--rw-r--r--   0 freedmand   (501) staff       (20)        1 2023-04-23 12:50:03.000000 semantra-0.0.9/src/semantra.egg-info/dependency_links.txt
--rw-r--r--   0 freedmand   (501) staff       (20)       52 2023-04-23 12:50:03.000000 semantra-0.0.9/src/semantra.egg-info/entry_points.txt
--rw-r--r--   0 freedmand   (501) staff       (20)      156 2023-04-23 12:50:03.000000 semantra-0.0.9/src/semantra.egg-info/requires.txt
--rw-r--r--   0 freedmand   (501) staff       (20)        9 2023-04-23 12:50:03.000000 semantra-0.0.9/src/semantra.egg-info/top_level.txt
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 21:16:04.492261 semantra-0.1.0/
+-rw-r--r--   0 freedmand   (501) staff       (20)     1071 2023-03-31 03:28:18.000000 semantra-0.1.0/LICENSE
+-rw-r--r--   0 freedmand   (501) staff       (20)     9897 2023-04-23 21:16:04.489555 semantra-0.1.0/PKG-INFO
+-rw-r--r--   0 freedmand   (501) staff       (20)     9354 2023-04-23 21:15:19.000000 semantra-0.1.0/README.md
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 21:16:04.474356 semantra-0.1.0/client/
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 21:16:04.476392 semantra-0.1.0/client/public/
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 21:16:04.478657 semantra-0.1.0/client/public/build/
+-rw-r--r--   0 freedmand   (501) staff       (20)    14441 2023-04-22 21:42:14.000000 semantra-0.1.0/client/public/build/bundle.css
+-rw-r--r--   0 freedmand   (501) staff       (20)   449074 2023-04-22 21:42:14.000000 semantra-0.1.0/client/public/build/bundle.js
+-rw-r--r--   0 freedmand   (501) staff       (20)  1495716 2023-04-22 21:42:14.000000 semantra-0.1.0/client/public/build/bundle.js.map
+-rw-r--r--   0 freedmand   (501) staff       (20)     3300 2023-04-09 04:23:49.000000 semantra-0.1.0/client/public/favicon.png
+-rw-r--r--   0 freedmand   (501) staff       (20)      890 2023-02-15 22:52:41.000000 semantra-0.1.0/client/public/global.css
+-rw-r--r--   0 freedmand   (501) staff       (20)      434 2023-04-09 20:49:05.000000 semantra-0.1.0/client/public/index.html
+-rw-r--r--   0 freedmand   (501) staff       (20)     1020 2023-04-23 21:15:46.000000 semantra-0.1.0/pyproject.toml
+-rw-r--r--   0 freedmand   (501) staff       (20)       38 2023-04-23 21:16:04.492311 semantra-0.1.0/setup.cfg
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 21:16:04.474655 semantra-0.1.0/src/
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 21:16:04.483251 semantra-0.1.0/src/semantra/
+-rw-r--r--   0 freedmand   (501) staff       (20)        0 2023-04-23 04:39:23.000000 semantra-0.1.0/src/semantra/__init__.py
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 21:16:04.486012 semantra-0.1.0/src/semantra/__pycache__/
+-rw-r--r--   0 freedmand   (501) staff       (20)      148 2023-04-23 04:39:41.000000 semantra-0.1.0/src/semantra/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 freedmand   (501) staff       (20)    10961 2023-04-23 04:37:57.000000 semantra-0.1.0/src/semantra/__pycache__/models.cpython-39.pyc
+-rw-r--r--   0 freedmand   (501) staff       (20)     3086 2023-04-23 04:37:58.000000 semantra-0.1.0/src/semantra/__pycache__/pdf.cpython-39.pyc
+-rw-r--r--   0 freedmand   (501) staff       (20)    19561 2023-04-23 12:15:19.000000 semantra-0.1.0/src/semantra/__pycache__/semantra.cpython-39.pyc
+-rw-r--r--   0 freedmand   (501) staff       (20)     4744 2023-04-23 04:37:58.000000 semantra-0.1.0/src/semantra/__pycache__/util.cpython-39.pyc
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 21:16:04.486500 semantra-0.1.0/src/semantra/client_public/
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 21:16:04.487509 semantra-0.1.0/src/semantra/client_public/build/
+-rw-r--r--   0 freedmand   (501) staff       (20)    14441 2023-04-22 21:42:14.000000 semantra-0.1.0/src/semantra/client_public/build/bundle.css
+-rw-r--r--   0 freedmand   (501) staff       (20)   449074 2023-04-22 21:42:14.000000 semantra-0.1.0/src/semantra/client_public/build/bundle.js
+-rw-r--r--   0 freedmand   (501) staff       (20)  1495716 2023-04-22 21:42:14.000000 semantra-0.1.0/src/semantra/client_public/build/bundle.js.map
+-rw-r--r--   0 freedmand   (501) staff       (20)     3300 2023-04-09 04:23:49.000000 semantra-0.1.0/src/semantra/client_public/favicon.png
+-rw-r--r--   0 freedmand   (501) staff       (20)      890 2023-02-15 22:52:41.000000 semantra-0.1.0/src/semantra/client_public/global.css
+-rw-r--r--   0 freedmand   (501) staff       (20)      434 2023-04-09 20:49:05.000000 semantra-0.1.0/src/semantra/client_public/index.html
+-rw-r--r--   0 freedmand   (501) staff       (20)    11501 2023-04-23 13:37:42.000000 semantra-0.1.0/src/semantra/models.py
+-rw-r--r--   0 freedmand   (501) staff       (20)     3118 2023-04-23 04:31:52.000000 semantra-0.1.0/src/semantra/pdf.py
+-rw-r--r--   0 freedmand   (501) staff       (20)    28701 2023-04-23 12:49:54.000000 semantra-0.1.0/src/semantra/semantra.py
+-rw-r--r--   0 freedmand   (501) staff       (20)     4524 2023-04-22 20:05:23.000000 semantra-0.1.0/src/semantra/util.py
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 21:16:04.484574 semantra-0.1.0/src/semantra.egg-info/
+-rw-r--r--   0 freedmand   (501) staff       (20)     9897 2023-04-23 21:16:04.000000 semantra-0.1.0/src/semantra.egg-info/PKG-INFO
+-rw-r--r--   0 freedmand   (501) staff       (20)     1018 2023-04-23 21:16:04.000000 semantra-0.1.0/src/semantra.egg-info/SOURCES.txt
+-rw-r--r--   0 freedmand   (501) staff       (20)        1 2023-04-23 21:16:04.000000 semantra-0.1.0/src/semantra.egg-info/dependency_links.txt
+-rw-r--r--   0 freedmand   (501) staff       (20)       52 2023-04-23 21:16:04.000000 semantra-0.1.0/src/semantra.egg-info/entry_points.txt
+-rw-r--r--   0 freedmand   (501) staff       (20)      176 2023-04-23 21:16:04.000000 semantra-0.1.0/src/semantra.egg-info/requires.txt
+-rw-r--r--   0 freedmand   (501) staff       (20)        9 2023-04-23 21:16:04.000000 semantra-0.1.0/src/semantra.egg-info/top_level.txt
```

### Comparing `semantra-0.0.9/LICENSE` & `semantra-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `semantra-0.0.9/client/public/build/bundle.css` & `semantra-0.1.0/client/public/build/bundle.css`

 * *Files identical despite different names*

### Comparing `semantra-0.0.9/client/public/build/bundle.js` & `semantra-0.1.0/client/public/build/bundle.js`

 * *Files identical despite different names*

### Comparing `semantra-0.0.9/client/public/build/bundle.js.map` & `semantra-0.1.0/client/public/build/bundle.js.map`

 * *Files identical despite different names*

### Comparing `semantra-0.0.9/client/public/favicon.png` & `semantra-0.1.0/client/public/favicon.png`

 * *Files identical despite different names*

### Comparing `semantra-0.0.9/client/public/global.css` & `semantra-0.1.0/client/public/global.css`

 * *Files identical despite different names*

### Comparing `semantra-0.0.9/pyproject.toml` & `semantra-0.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "semantra"
-version = "0.0.9"
+version = "0.1.0"
 description = "A semantic search CLI tool"
 authors = [{name = "Dylan Freedman", email = "freedmand@gmail.com"}]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-  "annoy>=1.17.2",
+  "annoy_fixed>=1.16.3",
   "click>=8.1.3",
   "Flask>=2.2.3",
   "openai>=0.27.2",
+  "Pillow>=9.5.0",
   "pypdfium2>=4.5.0",
   "python-dotenv>=1.0.0",
   "tiktoken>=0.3.3",
   "torch>=2.0.0",
   "tqdm>=4.65.0",
   "transformers>=4.27.4"
 ]
```

### Comparing `semantra-0.0.9/src/semantra/__pycache__/models.cpython-39.pyc` & `semantra-0.1.0/src/semantra/__pycache__/models.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `semantra-0.0.9/src/semantra/__pycache__/pdf.cpython-39.pyc` & `semantra-0.1.0/src/semantra/__pycache__/pdf.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `semantra-0.0.9/src/semantra/__pycache__/semantra.cpython-39.pyc` & `semantra-0.1.0/src/semantra/__pycache__/semantra.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `semantra-0.0.9/src/semantra/__pycache__/util.cpython-39.pyc` & `semantra-0.1.0/src/semantra/__pycache__/util.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `semantra-0.0.9/src/semantra/client_public/build/bundle.css` & `semantra-0.1.0/src/semantra/client_public/build/bundle.css`

 * *Files identical despite different names*

### Comparing `semantra-0.0.9/src/semantra/client_public/build/bundle.js` & `semantra-0.1.0/src/semantra/client_public/build/bundle.js`

 * *Files identical despite different names*

### Comparing `semantra-0.0.9/src/semantra/client_public/build/bundle.js.map` & `semantra-0.1.0/src/semantra/client_public/build/bundle.js.map`

 * *Files identical despite different names*

### Comparing `semantra-0.0.9/src/semantra/client_public/favicon.png` & `semantra-0.1.0/src/semantra/client_public/favicon.png`

 * *Files identical despite different names*

### Comparing `semantra-0.0.9/src/semantra/client_public/global.css` & `semantra-0.1.0/src/semantra/client_public/global.css`

 * *Files identical despite different names*

### Comparing `semantra-0.0.9/src/semantra/models.py` & `semantra-0.1.0/src/semantra/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from transformers import AutoTokenizer, AutoModel
 import tiktoken
 import numpy as np
 import openai
 from dotenv import load_dotenv
 import os
 
-load_dotenv()
+load_dotenv(dotenv_path=os.path.join(os.getcwd(), ".env"))
 
 if "OPENAI_API_KEY" in os.environ:
     openai.api_key = os.getenv("OPENAI_API_KEY")
 
 
 minilm_model_name = "sentence-transformers/all-MiniLM-L6-v2"
 mpnet_model_name = "sentence-transformers/all-mpnet-base-v2"
@@ -107,14 +107,19 @@
 class OpenAIModel(BaseModel):
     def __init__(
         self,
         model_name="text-embedding-ada-002",
         num_dimensions=1536,
         tokenizer_name="cl100k_base",
     ):
+        # Check if OpenAI API key is set
+        if "OPENAI_API_KEY" not in os.environ:
+            raise Exception(
+                "OpenAI API key not set. Please set the OPENAI_API_KEY environment variable or create a `.env` file with the key in the same directory."
+            )
         self.model_name = model_name
         self.num_dimensions = num_dimensions
         self.tokenizer = tiktoken.get_encoding(tokenizer_name)
 
     def get_config(self):
         return {
             "model_type": "openai",
```

### Comparing `semantra-0.0.9/src/semantra/pdf.py` & `semantra-0.1.0/src/semantra/pdf.py`

 * *Files identical despite different names*

### Comparing `semantra-0.0.9/src/semantra/semantra.py` & `semantra-0.1.0/src/semantra/semantra.py`

 * *Files identical despite different names*

### Comparing `semantra-0.0.9/src/semantra/util.py` & `semantra-0.1.0/src/semantra/util.py`

 * *Files identical despite different names*

### Comparing `semantra-0.0.9/src/semantra.egg-info/SOURCES.txt` & `semantra-0.1.0/src/semantra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

