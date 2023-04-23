# Comparing `tmp/embedbase-1.0.4.tar.gz` & `tmp/embedbase-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedbase-1.0.4.tar", max compression
+gzip compressed data, was "embedbase-1.0.5.tar", max compression
```

## Comparing `embedbase-1.0.4.tar` & `embedbase-1.0.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1069 2023-04-20 14:25:59.598282 embedbase-1.0.4/LICENSE
--rw-r--r--   0        0        0     5879 2023-04-20 14:25:59.598282 embedbase-1.0.4/README.md
--rw-r--r--   0        0        0      121 2023-04-20 14:25:59.666282 embedbase-1.0.4/embedbase/__init__.py
--rw-r--r--   0        0        0     3388 2023-04-20 14:25:59.666282 embedbase-1.0.4/embedbase/__main__.py
--rw-r--r--   0        0        0      976 2023-04-20 14:25:59.666282 embedbase-1.0.4/embedbase/api.py
--rw-r--r--   0        0        0    16171 2023-04-20 14:25:59.666282 embedbase-1.0.4/embedbase/app.py
--rw-r--r--   0        0        0       88 2023-04-20 14:25:59.666282 embedbase-1.0.4/embedbase/database/__init__.py
--rw-r--r--   0        0        0     2398 2023-04-20 14:25:59.666282 embedbase-1.0.4/embedbase/database/base.py
--rw-r--r--   0        0        0     1164 2023-04-20 14:25:59.666282 embedbase-1.0.4/embedbase/database/db_utils.py
--rw-r--r--   0        0        0     4701 2023-04-20 14:25:59.666282 embedbase-1.0.4/embedbase/database/memory_db.py
--rw-r--r--   0        0        0      504 2023-04-20 14:25:59.666282 embedbase-1.0.4/embedbase/database/pinecone_db.py
--rw-r--r--   0        0        0     7938 2023-04-20 14:25:59.666282 embedbase-1.0.4/embedbase/database/postgres_db.py
--rw-r--r--   0        0        0     4084 2023-04-20 14:25:59.666282 embedbase-1.0.4/embedbase/database/supabase_db.py
--rw-r--r--   0        0        0      411 2023-04-20 14:25:59.666282 embedbase-1.0.4/embedbase/database/weaviate_db.py
--rw-r--r--   0        0        0       77 2023-04-20 14:25:59.666282 embedbase-1.0.4/embedbase/embedding/__init__.py
--rw-r--r--   0        0        0      858 2023-04-20 14:25:59.666282 embedbase-1.0.4/embedbase/embedding/base.py
--rw-r--r--   0        0        0     1237 2023-04-20 14:25:59.666282 embedbase-1.0.4/embedbase/embedding/cohere.py
--rw-r--r--   0        0        0     2059 2023-04-20 14:25:59.666282 embedbase-1.0.4/embedbase/embedding/openai.py
--rw-r--r--   0        0        0     1551 2023-04-20 14:25:59.666282 embedbase-1.0.4/embedbase/firebase_auth.py
--rw-r--r--   0        0        0      575 2023-04-20 14:25:59.666282 embedbase-1.0.4/embedbase/logging_utils.py
--rw-r--r--   0        0        0      661 2023-04-20 14:25:59.666282 embedbase-1.0.4/embedbase/models.py
--rw-r--r--   0        0        0     1285 2023-04-20 14:25:59.666282 embedbase-1.0.4/embedbase/settings.py
--rw-r--r--   0        0        0     3208 2023-04-20 14:25:59.666282 embedbase-1.0.4/embedbase/strings.py
--rw-r--r--   0        0        0      301 2023-04-20 14:25:59.666282 embedbase-1.0.4/embedbase/supabase_auth.py
--rw-r--r--   0        0        0     2101 2023-04-20 14:25:59.666282 embedbase-1.0.4/embedbase/utils.py
--rw-r--r--   0        0        0     3585 2023-04-20 14:25:59.670282 embedbase-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     7360 1970-01-01 00:00:00.000000 embedbase-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-23 15:50:48.608243 embedbase-1.0.5/LICENSE
+-rw-r--r--   0        0        0     6105 2023-04-23 15:50:48.608243 embedbase-1.0.5/README.md
+-rw-r--r--   0        0        0      121 2023-04-23 15:50:48.660244 embedbase-1.0.5/embedbase/__init__.py
+-rw-r--r--   0        0        0     3447 2023-04-23 15:50:48.660244 embedbase-1.0.5/embedbase/__main__.py
+-rw-r--r--   0        0        0      976 2023-04-23 15:50:48.660244 embedbase-1.0.5/embedbase/api.py
+-rw-r--r--   0        0        0    16171 2023-04-23 15:50:48.660244 embedbase-1.0.5/embedbase/app.py
+-rw-r--r--   0        0        0       88 2023-04-23 15:50:48.664244 embedbase-1.0.5/embedbase/database/__init__.py
+-rw-r--r--   0        0        0     2398 2023-04-23 15:50:48.664244 embedbase-1.0.5/embedbase/database/base.py
+-rw-r--r--   0        0        0     1164 2023-04-23 15:50:48.664244 embedbase-1.0.5/embedbase/database/db_utils.py
+-rw-r--r--   0        0        0     4701 2023-04-23 15:50:48.664244 embedbase-1.0.5/embedbase/database/memory_db.py
+-rw-r--r--   0        0        0      504 2023-04-23 15:50:48.664244 embedbase-1.0.5/embedbase/database/pinecone_db.py
+-rw-r--r--   0        0        0     7938 2023-04-23 15:50:48.664244 embedbase-1.0.5/embedbase/database/postgres_db.py
+-rw-r--r--   0        0        0     4084 2023-04-23 15:50:48.664244 embedbase-1.0.5/embedbase/database/supabase_db.py
+-rw-r--r--   0        0        0      411 2023-04-23 15:50:48.664244 embedbase-1.0.5/embedbase/database/weaviate_db.py
+-rw-r--r--   0        0        0       77 2023-04-23 15:50:48.664244 embedbase-1.0.5/embedbase/embedding/__init__.py
+-rw-r--r--   0        0        0      858 2023-04-23 15:50:48.664244 embedbase-1.0.5/embedbase/embedding/base.py
+-rw-r--r--   0        0        0     1237 2023-04-23 15:50:48.664244 embedbase-1.0.5/embedbase/embedding/cohere.py
+-rw-r--r--   0        0        0     2059 2023-04-23 15:50:48.664244 embedbase-1.0.5/embedbase/embedding/openai.py
+-rw-r--r--   0        0        0     1551 2023-04-23 15:50:48.664244 embedbase-1.0.5/embedbase/firebase_auth.py
+-rw-r--r--   0        0        0      690 2023-04-23 15:50:48.664244 embedbase-1.0.5/embedbase/logging_utils.py
+-rw-r--r--   0        0        0      661 2023-04-23 15:50:48.664244 embedbase-1.0.5/embedbase/models.py
+-rw-r--r--   0        0        0     1285 2023-04-23 15:50:48.664244 embedbase-1.0.5/embedbase/settings.py
+-rw-r--r--   0        0        0     3208 2023-04-23 15:50:48.664244 embedbase-1.0.5/embedbase/strings.py
+-rw-r--r--   0        0        0      301 2023-04-23 15:50:48.664244 embedbase-1.0.5/embedbase/supabase_auth.py
+-rw-r--r--   0        0        0     2101 2023-04-23 15:50:48.664244 embedbase-1.0.5/embedbase/utils.py
+-rw-r--r--   0        0        0     3585 2023-04-23 15:50:48.664244 embedbase-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     7586 1970-01-01 00:00:00.000000 embedbase-1.0.5/PKG-INFO
```

### Comparing `embedbase-1.0.4/LICENSE` & `embedbase-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.4/README.md` & `embedbase-1.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,28 @@
 
 
 <p align="center">
 <img width="150" alt="embedbasevector" src="https://user-images.githubusercontent.com/11430621/223136025-14572cac-f2aa-455c-936b-a48cb35a0c57.png">
   <h1 align="center">Embedbase</h1>
 
 
-<h3 align="center">The end to end platform to help you ship embeddings-powered apps.</h3>
+<h3 align="center">Add memory to AI with embeddings</h3>
 
   <p align="center">
     <br />
     <a href="https://discord.gg/pMNeuGrDky"><img alt="Discord" src="https://img.shields.io/discord/1066022656845025310?color=black&style=for-the-badge"></a>
     <a href="https://badge.fury.io/py/embedbase"><img alt="PyPI" src="https://img.shields.io/pypi/v/embedbase?color=black&style=for-the-badge"></a>
-    <!--<a href="https://render.com/deploy?repo=https://github.com/different-ai/embedbase">
+    <a href="https://render.com/deploy?repo=https://github.com/different-ai/embedbase">
+    <br />
     <img src="https://render.com/images/deploy-to-render-button.svg" alt="Deploy to Render">
-  </a>-->
+  </a>
+  <br />
+  <a target="_blank" href="https://colab.research.google.com/github/different-ai/embedbase/blob/main/notebooks/Embedbase_Getting_started.ipynb">
+    <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
+  </a>
     <p align="center">Open-source API, SDK & dashboard to easily create, store, and retrieve machine learning embeddings</p>
     <p align="center">Used by <a href="https://github.com/louis030195/obsidian-ava">AVA</a> and serving 100k request a day</p>
     <div align="center">
       <a href="https://app.embedbase.xyz/signup">Try Embedbase Cloud now</a>
       ·
       <a href="https://github.com/different-ai/embedbase/issues/new?assignees=&labels=enhancement">Request Feature</a>
       ·
```

### Comparing `embedbase-1.0.4/embedbase/__main__.py` & `embedbase-1.0.5/embedbase/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,52 +1,54 @@
 from typing import List, Union
 import uvicorn
 from embedbase import get_app
 from embedbase.database.memory_db import MemoryDatabase
 from embedbase.embedding.base import Embedder
 from sentence_transformers import SentenceTransformer
 
+
 # pylint: disable=missing-class-docstring
 class LocalEmbedder(Embedder):
     EMBEDDING_MODEL = "all-MiniLM-L6-v2"
- 
-    def __init__(
-        self, model: str = EMBEDDING_MODEL, **kwargs
-    ):
+
+    def __init__(self, model: str = EMBEDDING_MODEL, **kwargs):
         super().__init__(**kwargs)
         self.model = SentenceTransformer(model)
- 
+        self._dimensions = self.model.get_sentence_embedding_dimension()
+
     @property
     def dimensions(self) -> int:
         """
         Return the dimensions of the embeddings
         :return: dimensions of the embeddings
         """
         return self._dimensions
- 
+
     def is_too_big(self, text: str) -> bool:
         """
         Check if text is too big to be embedded,
         delegating the splitting UX to the caller
         :param text: text to check
         :return: True if text is too big, False otherwise
         """
         return len(text) > self.model.get_max_seq_length()
- 
+
     async def embed(self, data: Union[List[str], str]) -> List[List[float]]:
         """
         Embed a list of texts
         :param texts: list of texts
         :return: list of embeddings
         """
         embeddings = self.model.encode(data)
         return embeddings.tolist() if isinstance(data, list) else [embeddings.tolist()]
 
+
 app = get_app().use_db(MemoryDatabase()).use_embedder(LocalEmbedder()).run()
 
+
 # pylint: disable=missing-function-docstring
 def run_app():
     print(
         # pylint: disable=anomalous-backslash-in-string
         """
                  _           _   _         _               _          _         
         /\ \        /\_\/\_\ _    / /\            /\ \       /\ \       
@@ -71,9 +73,10 @@
      \/_____________/\_\___\     /____/_/ \_____\/   \/__________/      
                                                                                                 
                  [-0.005, 0.012, -0.008, ..., -0.010]
         """
     )
     uvicorn.run("embedbase:app", host="0.0.0.0")
 
+
 if __name__ == "__main__":
     run_app()
```

### Comparing `embedbase-1.0.4/embedbase/api.py` & `embedbase-1.0.5/embedbase/api.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.4/embedbase/app.py` & `embedbase-1.0.5/embedbase/app.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.4/embedbase/database/base.py` & `embedbase-1.0.5/embedbase/database/base.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.4/embedbase/database/db_utils.py` & `embedbase-1.0.5/embedbase/database/db_utils.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.4/embedbase/database/memory_db.py` & `embedbase-1.0.5/embedbase/database/memory_db.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.4/embedbase/database/postgres_db.py` & `embedbase-1.0.5/embedbase/database/postgres_db.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.4/embedbase/database/supabase_db.py` & `embedbase-1.0.5/embedbase/database/supabase_db.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.4/embedbase/embedding/base.py` & `embedbase-1.0.5/embedbase/embedding/base.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.4/embedbase/embedding/cohere.py` & `embedbase-1.0.5/embedbase/embedding/cohere.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.4/embedbase/embedding/openai.py` & `embedbase-1.0.5/embedbase/embedding/openai.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.4/embedbase/firebase_auth.py` & `embedbase-1.0.5/embedbase/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.4/embedbase/logging_utils.py` & `embedbase-1.0.5/embedbase/logging_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 import logging
 from typing import Optional
 
 from embedbase.settings import Settings
 from logging import Logger
 
+
 def get_logger(settings: Optional[Settings] = None) -> Logger:
     logger = logging.getLogger("embedbase")
     logger.setLevel(settings.log_level if settings else "INFO")
+
+    # Clear the existing handlers
+    for handler in logger.handlers[:]:
+        logger.removeHandler(handler)
+
     handler = logging.StreamHandler()
     handler.setLevel(settings.log_level if settings else "INFO")
     formatter = logging.Formatter(
         "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
     )
     handler.setFormatter(formatter)
     logger.addHandler(handler)
+
     return logger
```

### Comparing `embedbase-1.0.4/embedbase/models.py` & `embedbase-1.0.5/embedbase/models.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.4/embedbase/settings.py` & `embedbase-1.0.5/embedbase/settings.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.4/embedbase/strings.py` & `embedbase-1.0.5/embedbase/strings.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.4/embedbase/utils.py` & `embedbase-1.0.5/embedbase/utils.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.4/pyproject.toml` & `embedbase-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "embedbase"
-version = "1.0.4"
+version = "1.0.5"
 description = "API, SDK & dashboard to easily create, store, and retrieve machine learning embeddings."
 readme = "README.md"
 authors = ["Different AI <louis@embedbase.xyz>"]
 license = "MIT"
 repository = "https://github.com/different-ai/embedbase"
 homepage = "https://github.com/different-ai/embedbase"
 
@@ -53,15 +53,15 @@
 pylint = "^2.11.1"
 pytest = "^7.3.1"
 pyupgrade = "^2.29.1"
 safety = "^1.10.3"
 coverage = "^6.1.2"
 coverage-badge = "^1.1.0"
 pytest-html = "^3.1.1"
-pytest-cov = "^3.0.0"
+pytest-cov = "^4.0.0"
 httpx = "^0.24.0"
 pytest-asyncio = "^0.21.0"
 
 [project.optional-dependencies]
 minimal = []
 firebase = ["firebase_admin"]
 observability = ["sentry-sdk[fastapi]"]
```

### Comparing `embedbase-1.0.4/PKG-INFO` & `embedbase-1.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedbase
-Version: 1.0.4
+Version: 1.0.5
 Summary: API, SDK & dashboard to easily create, store, and retrieve machine learning embeddings.
 Home-page: https://github.com/different-ai/embedbase
 License: MIT
 Keywords: embeddings,machine learning,artificial intelligence
 Author: Different AI
 Author-email: louis@embedbase.xyz
 Requires-Python: >=3.8,<4.0
@@ -36,23 +36,28 @@
 
 
 <p align="center">
 <img width="150" alt="embedbasevector" src="https://user-images.githubusercontent.com/11430621/223136025-14572cac-f2aa-455c-936b-a48cb35a0c57.png">
   <h1 align="center">Embedbase</h1>
 
 
-<h3 align="center">The end to end platform to help you ship embeddings-powered apps.</h3>
+<h3 align="center">Add memory to AI with embeddings</h3>
 
   <p align="center">
     <br />
     <a href="https://discord.gg/pMNeuGrDky"><img alt="Discord" src="https://img.shields.io/discord/1066022656845025310?color=black&style=for-the-badge"></a>
     <a href="https://badge.fury.io/py/embedbase"><img alt="PyPI" src="https://img.shields.io/pypi/v/embedbase?color=black&style=for-the-badge"></a>
-    <!--<a href="https://render.com/deploy?repo=https://github.com/different-ai/embedbase">
+    <a href="https://render.com/deploy?repo=https://github.com/different-ai/embedbase">
+    <br />
     <img src="https://render.com/images/deploy-to-render-button.svg" alt="Deploy to Render">
-  </a>-->
+  </a>
+  <br />
+  <a target="_blank" href="https://colab.research.google.com/github/different-ai/embedbase/blob/main/notebooks/Embedbase_Getting_started.ipynb">
+    <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
+  </a>
     <p align="center">Open-source API, SDK & dashboard to easily create, store, and retrieve machine learning embeddings</p>
     <p align="center">Used by <a href="https://github.com/louis030195/obsidian-ava">AVA</a> and serving 100k request a day</p>
     <div align="center">
       <a href="https://app.embedbase.xyz/signup">Try Embedbase Cloud now</a>
       ·
       <a href="https://github.com/different-ai/embedbase/issues/new?assignees=&labels=enhancement">Request Feature</a>
       ·
```

