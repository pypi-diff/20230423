# Comparing `tmp/locusdb-0.1.0.tar.gz` & `tmp/locusdb-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "locusdb-0.1.0.tar", max compression
+gzip compressed data, was "locusdb-0.2.0.tar", max compression
```

## Comparing `locusdb-0.1.0.tar` & `locusdb-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-04-15 17:42:49.338898 locusdb-0.1.0/LICENSE
--rw-r--r--   0        0        0     1161 2023-04-20 17:22:18.616256 locusdb-0.1.0/README.md
--rw-r--r--   0        0        0      529 2023-04-20 17:21:15.594477 locusdb-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       91 2023-04-17 16:49:29.119238 locusdb-0.1.0/src/locusdb/__init__.py
--rw-r--r--   0        0        0      913 2023-04-16 18:14:59.138499 locusdb-0.1.0/src/locusdb/config.py
--rw-r--r--   0        0        0     3295 2023-04-20 17:21:04.132094 locusdb-0.1.0/src/locusdb/index.py
--rw-r--r--   0        0        0      619 2023-04-16 18:14:57.658451 locusdb-0.1.0/src/locusdb/vector.py
--rw-r--r--   0        0        0     1866 1970-01-01 00:00:00.000000 locusdb-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-23 18:03:54.915691 locusdb-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1188 2023-04-23 18:03:54.915691 locusdb-0.2.0/README.md
+-rw-r--r--   0        0        0      592 2023-04-23 18:04:07.240211 locusdb-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       91 2023-04-23 18:03:54.915691 locusdb-0.2.0/src/locusdb/__init__.py
+-rw-r--r--   0        0        0      913 2023-04-23 18:03:54.915691 locusdb-0.2.0/src/locusdb/config.py
+-rw-r--r--   0        0        0     3247 2023-04-23 18:03:54.915691 locusdb-0.2.0/src/locusdb/index.py
+-rw-r--r--   0        0        0      619 2023-04-23 18:03:54.915691 locusdb-0.2.0/src/locusdb/vector.py
+-rw-r--r--   0        0        0     1992 1970-01-01 00:00:00.000000 locusdb-0.2.0/setup.py
+-rw-r--r--   0        0        0     1893 1970-01-01 00:00:00.000000 locusdb-0.2.0/PKG-INFO
```

### Comparing `locusdb-0.1.0/LICENSE` & `locusdb-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `locusdb-0.1.0/README.md` & `locusdb-0.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 Why Locus?
 * Easy to use
 * 2 dependencies
 * Store database locally
 
 
 ## Installation
-Soon
-
+``` bash
+pip install locusdb
+```
 ## Example Code
 Some example code to illustrate Locus' functionality.
 
 ``` python
 import numpy as np
 from locusdb import Config, Vector, Index
```

### Comparing `locusdb-0.1.0/pyproject.toml` & `locusdb-0.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "locusdb"
-version = "0.1.0"
+version = "v0.2.0"
 license="Apache-2.0"
 description = "Local, in-memory vector database"
 authors = ["Alex <46456279+the-alex-b@users.noreply.github.com>"]
 readme = "README.md"
 repository="https://github.com/the-alex-b/Locus"
 
 [tool.poetry.dependencies]
@@ -13,11 +13,14 @@
 numpy = "^1.24.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 mypy = "^1.2.0"
 bandit = "^1.7.5"
 isort = "^5.12.0"
+pytest-cov = "^4.0.0"
+pylint = "^2.17.2"
+autoflake = "^2.1.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `locusdb-0.1.0/src/locusdb/config.py` & `locusdb-0.2.0/src/locusdb/config.py`

 * *Files identical despite different names*

### Comparing `locusdb-0.1.0/src/locusdb/index.py` & `locusdb-0.2.0/src/locusdb/index.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,17 +75,14 @@
 
         if persist_on_disk:
             self._store_on_disk()
 
     def retrieve(self, embedding: np.array, number_of_results: int = 3) -> list[dict]:
         labels, distances = self.hnsw_index.knn_query(embedding, k=number_of_results)
 
-        print(labels)
-        print(distances)
-
         return [
             {"element": self.structured_memory[id], "distance": distances[0][i]}
             for i, id in enumerate(labels[0])
         ]
 
     def _store_on_disk(self) -> None:
         with open(
```

### Comparing `locusdb-0.1.0/src/locusdb/vector.py` & `locusdb-0.2.0/src/locusdb/vector.py`

 * *Files identical despite different names*

### Comparing `locusdb-0.1.0/PKG-INFO` & `locusdb-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: locusdb
-Version: 0.1.0
+Version: 0.2.0
 Summary: Local, in-memory vector database
 Home-page: https://github.com/the-alex-b/Locus
 License: Apache-2.0
 Author: Alex
 Author-email: 46456279+the-alex-b@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -23,16 +23,17 @@
 Why Locus?
 * Easy to use
 * 2 dependencies
 * Store database locally
 
 
 ## Installation
-Soon
-
+``` bash
+pip install locusdb
+```
 ## Example Code
 Some example code to illustrate Locus' functionality.
 
 ``` python
 import numpy as np
 from locusdb import Config, Vector, Index
```

