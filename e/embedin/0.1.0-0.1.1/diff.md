# Comparing `tmp/embedin-0.1.0.tar.gz` & `tmp/embedin-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedin-0.1.0.tar", last modified: Sat Apr 22 15:51:24 2023, max compression
+gzip compressed data, was "embedin-0.1.1.tar", last modified: Sat Apr 22 20:07:35 2023, max compression
```

## Comparing `embedin-0.1.0.tar` & `embedin-0.1.1.tar`

### file list

```diff
@@ -1,61 +1,62 @@
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-04-22 15:51:24.272507 embedin-0.1.0/
--rw-r--r--   0 xchen375   (502) staff       (20)    11357 2023-04-10 04:12:37.000000 embedin-0.1.0/LICENSE
--rw-r--r--   0 xchen375   (502) staff       (20)     1570 2023-04-22 15:51:24.272188 embedin-0.1.0/PKG-INFO
--rw-r--r--   0 xchen375   (502) staff       (20)     1133 2023-04-22 15:16:27.000000 embedin-0.1.0/README.md
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-04-22 15:51:24.250422 embedin-0.1.0/embedin.egg-info/
--rw-r--r--   0 xchen375   (502) staff       (20)     1570 2023-04-22 15:51:24.000000 embedin-0.1.0/embedin.egg-info/PKG-INFO
--rw-r--r--   0 xchen375   (502) staff       (20)     1146 2023-04-22 15:51:24.000000 embedin-0.1.0/embedin.egg-info/SOURCES.txt
--rw-r--r--   0 xchen375   (502) staff       (20)        1 2023-04-22 15:51:24.000000 embedin-0.1.0/embedin.egg-info/dependency_links.txt
--rw-r--r--   0 xchen375   (502) staff       (20)       10 2023-04-22 15:51:24.000000 embedin-0.1.0/embedin.egg-info/top_level.txt
--rw-r--r--   0 xchen375   (502) staff       (20)       38 2023-04-22 15:51:24.272591 embedin-0.1.0/setup.cfg
--rw-r--r--   0 xchen375   (502) staff       (20)      652 2023-04-22 15:50:34.000000 embedin-0.1.0/setup.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-04-22 15:51:24.250884 embedin-0.1.0/src/
--rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-09 17:01:17.000000 embedin-0.1.0/src/__init__.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-04-22 15:51:24.251286 embedin-0.1.0/src/client/
--rw-r--r--   0 xchen375   (502) staff       (20)     3166 2023-04-22 15:16:27.000000 embedin-0.1.0/src/client/__init__.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-04-22 15:51:24.253354 embedin-0.1.0/src/embedding/
--rw-r--r--   0 xchen375   (502) staff       (20)      130 2023-04-09 16:47:27.000000 embedin-0.1.0/src/embedding/__init__.py
--rw-r--r--   0 xchen375   (502) staff       (20)      735 2023-04-11 22:28:11.000000 embedin-0.1.0/src/embedding/sentence_transformer.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-04-22 15:51:24.256242 embedin-0.1.0/src/index/
--rw-r--r--   0 xchen375   (502) staff       (20)     1314 2023-04-22 15:16:27.000000 embedin-0.1.0/src/index/__init__.py
--rw-r--r--   0 xchen375   (502) staff       (20)      476 2023-04-22 15:16:27.000000 embedin-0.1.0/src/index/faiss.py
--rw-r--r--   0 xchen375   (502) staff       (20)     1058 2023-04-22 15:16:27.000000 embedin-0.1.0/src/index/hnswlib.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-04-22 15:51:24.258166 embedin-0.1.0/src/model/
--rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-22 15:16:27.000000 embedin-0.1.0/src/model/__init__.py
--rw-r--r--   0 xchen375   (502) staff       (20)      275 2023-04-22 15:16:27.000000 embedin-0.1.0/src/model/collection_model.py
--rw-r--r--   0 xchen375   (502) staff       (20)      610 2023-04-22 15:16:27.000000 embedin-0.1.0/src/model/embedding_model.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-04-22 15:51:24.259996 embedin-0.1.0/src/repository/
--rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-22 15:16:27.000000 embedin-0.1.0/src/repository/__init__.py
--rw-r--r--   0 xchen375   (502) staff       (20)      885 2023-04-22 15:16:27.000000 embedin-0.1.0/src/repository/collection_repository.py
--rw-r--r--   0 xchen375   (502) staff       (20)     1658 2023-04-22 15:16:27.000000 embedin-0.1.0/src/repository/embedding_repository.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-04-22 15:51:24.261572 embedin-0.1.0/src/service/
--rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-22 15:16:27.000000 embedin-0.1.0/src/service/__init__.py
--rw-r--r--   0 xchen375   (502) staff       (20)      440 2023-04-22 15:16:27.000000 embedin-0.1.0/src/service/collection_service.py
--rw-r--r--   0 xchen375   (502) staff       (20)     1645 2023-04-22 15:16:27.000000 embedin-0.1.0/src/service/embedding_service.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-04-22 15:51:24.262213 embedin-0.1.0/src/util/
--rw-r--r--   0 xchen375   (502) staff       (20)      618 2023-04-22 15:16:27.000000 embedin-0.1.0/src/util/__init__.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-04-22 15:51:24.262859 embedin-0.1.0/tests/
--rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-10 19:13:54.000000 embedin-0.1.0/tests/__init__.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-04-22 15:51:24.263287 embedin-0.1.0/tests/client/
--rw-r--r--   0 xchen375   (502) staff       (20)     1785 2023-04-22 15:16:27.000000 embedin-0.1.0/tests/client/__init__.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-04-22 15:51:24.264886 embedin-0.1.0/tests/embedding/
--rw-r--r--   0 xchen375   (502) staff       (20)      318 2023-04-11 02:11:43.000000 embedin-0.1.0/tests/embedding/__init__.py
--rw-r--r--   0 xchen375   (502) staff       (20)     1273 2023-04-09 17:47:30.000000 embedin-0.1.0/tests/embedding/test_embedding.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-04-22 15:51:24.266521 embedin-0.1.0/tests/index/
--rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-22 15:16:27.000000 embedin-0.1.0/tests/index/__init__.py
--rw-r--r--   0 xchen375   (502) staff       (20)      780 2023-04-22 15:16:27.000000 embedin-0.1.0/tests/index/test_faiss.py
--rw-r--r--   0 xchen375   (502) staff       (20)     1631 2023-04-22 15:16:27.000000 embedin-0.1.0/tests/index/test_hnswlib.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-04-22 15:51:24.267866 embedin-0.1.0/tests/model/
--rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-22 15:16:27.000000 embedin-0.1.0/tests/model/__init__.py
--rw-r--r--   0 xchen375   (502) staff       (20)     1889 2023-04-22 15:16:27.000000 embedin-0.1.0/tests/model/test_collection_model.py
--rw-r--r--   0 xchen375   (502) staff       (20)     2039 2023-04-22 15:16:27.000000 embedin-0.1.0/tests/model/test_embedding_model.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-04-22 15:51:24.269268 embedin-0.1.0/tests/repository/
--rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-22 15:16:27.000000 embedin-0.1.0/tests/repository/__init__.py
--rw-r--r--   0 xchen375   (502) staff       (20)     2465 2023-04-22 15:16:27.000000 embedin-0.1.0/tests/repository/test_collection_repository.py
--rw-r--r--   0 xchen375   (502) staff       (20)     5420 2023-04-22 15:16:27.000000 embedin-0.1.0/tests/repository/test_embedding_repository.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-04-22 15:51:24.271082 embedin-0.1.0/tests/service/
--rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-22 15:16:27.000000 embedin-0.1.0/tests/service/__init__.py
--rw-r--r--   0 xchen375   (502) staff       (20)     1326 2023-04-22 15:16:27.000000 embedin-0.1.0/tests/service/test_collection_service.py
--rw-r--r--   0 xchen375   (502) staff       (20)     3640 2023-04-22 15:16:27.000000 embedin-0.1.0/tests/service/test_embedding_service.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-04-22 15:51:24.271607 embedin-0.1.0/tests/util/
--rw-r--r--   0 xchen375   (502) staff       (20)      656 2023-04-22 15:16:27.000000 embedin-0.1.0/tests/util/__init__.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-04-22 20:07:35.006303 embedin-0.1.1/
+-rw-r--r--   0 xchen375   (502) staff       (20)    11357 2023-04-10 04:12:37.000000 embedin-0.1.1/LICENSE
+-rw-r--r--   0 xchen375   (502) staff       (20)     1709 2023-04-22 20:07:35.005808 embedin-0.1.1/PKG-INFO
+-rw-r--r--   0 xchen375   (502) staff       (20)     1272 2023-04-22 15:54:51.000000 embedin-0.1.1/README.md
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-04-22 20:07:34.982881 embedin-0.1.1/embedin/
+-rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-09 17:01:17.000000 embedin-0.1.1/embedin/__init__.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-04-22 20:07:34.986088 embedin-0.1.1/embedin/client/
+-rw-r--r--   0 xchen375   (502) staff       (20)     3182 2023-04-22 17:06:36.000000 embedin-0.1.1/embedin/client/__init__.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-04-22 20:07:34.987284 embedin-0.1.1/embedin/embedding/
+-rw-r--r--   0 xchen375   (502) staff       (20)      130 2023-04-09 16:47:27.000000 embedin-0.1.1/embedin/embedding/__init__.py
+-rw-r--r--   0 xchen375   (502) staff       (20)      739 2023-04-22 17:06:36.000000 embedin-0.1.1/embedin/embedding/sentence_transformer.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-04-22 20:07:34.989077 embedin-0.1.1/embedin/index/
+-rw-r--r--   0 xchen375   (502) staff       (20)     1318 2023-04-22 17:06:36.000000 embedin-0.1.1/embedin/index/__init__.py
+-rw-r--r--   0 xchen375   (502) staff       (20)      480 2023-04-22 17:06:36.000000 embedin-0.1.1/embedin/index/faiss.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     1062 2023-04-22 17:06:36.000000 embedin-0.1.1/embedin/index/hnswlib.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-04-22 20:07:34.990831 embedin-0.1.1/embedin/model/
+-rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-22 15:16:27.000000 embedin-0.1.1/embedin/model/__init__.py
+-rw-r--r--   0 xchen375   (502) staff       (20)      275 2023-04-22 15:16:27.000000 embedin-0.1.1/embedin/model/collection_model.py
+-rw-r--r--   0 xchen375   (502) staff       (20)      610 2023-04-22 15:16:27.000000 embedin-0.1.1/embedin/model/embedding_model.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-04-22 20:07:34.992470 embedin-0.1.1/embedin/repository/
+-rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-22 15:16:27.000000 embedin-0.1.1/embedin/repository/__init__.py
+-rw-r--r--   0 xchen375   (502) staff       (20)      889 2023-04-22 17:06:36.000000 embedin-0.1.1/embedin/repository/collection_repository.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     1662 2023-04-22 17:06:36.000000 embedin-0.1.1/embedin/repository/embedding_repository.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-04-22 20:07:34.994172 embedin-0.1.1/embedin/service/
+-rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-22 15:16:27.000000 embedin-0.1.1/embedin/service/__init__.py
+-rw-r--r--   0 xchen375   (502) staff       (20)      444 2023-04-22 17:06:36.000000 embedin-0.1.1/embedin/service/collection_service.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     1653 2023-04-22 17:06:36.000000 embedin-0.1.1/embedin/service/embedding_service.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-04-22 20:07:34.994758 embedin-0.1.1/embedin/util/
+-rw-r--r--   0 xchen375   (502) staff       (20)      618 2023-04-22 15:16:27.000000 embedin-0.1.1/embedin/util/__init__.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-04-22 20:07:34.985472 embedin-0.1.1/embedin.egg-info/
+-rw-r--r--   0 xchen375   (502) staff       (20)     1709 2023-04-22 20:07:34.000000 embedin-0.1.1/embedin.egg-info/PKG-INFO
+-rw-r--r--   0 xchen375   (502) staff       (20)     1244 2023-04-22 20:07:34.000000 embedin-0.1.1/embedin.egg-info/SOURCES.txt
+-rw-r--r--   0 xchen375   (502) staff       (20)        1 2023-04-22 20:07:34.000000 embedin-0.1.1/embedin.egg-info/dependency_links.txt
+-rw-r--r--   0 xchen375   (502) staff       (20)      166 2023-04-22 20:07:34.000000 embedin-0.1.1/embedin.egg-info/requires.txt
+-rw-r--r--   0 xchen375   (502) staff       (20)       14 2023-04-22 20:07:34.000000 embedin-0.1.1/embedin.egg-info/top_level.txt
+-rw-r--r--   0 xchen375   (502) staff       (20)       38 2023-04-22 20:07:35.006429 embedin-0.1.1/setup.cfg
+-rw-r--r--   0 xchen375   (502) staff       (20)      827 2023-04-22 19:59:15.000000 embedin-0.1.1/setup.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-04-22 20:07:34.995355 embedin-0.1.1/tests/
+-rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-10 19:13:54.000000 embedin-0.1.1/tests/__init__.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-04-22 20:07:34.995826 embedin-0.1.1/tests/client/
+-rw-r--r--   0 xchen375   (502) staff       (20)     1789 2023-04-22 17:06:36.000000 embedin-0.1.1/tests/client/__init__.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-04-22 20:07:34.997197 embedin-0.1.1/tests/embedding/
+-rw-r--r--   0 xchen375   (502) staff       (20)      322 2023-04-22 17:06:36.000000 embedin-0.1.1/tests/embedding/__init__.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     1277 2023-04-22 17:06:36.000000 embedin-0.1.1/tests/embedding/test_embedding.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-04-22 20:07:34.998908 embedin-0.1.1/tests/index/
+-rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-22 15:16:27.000000 embedin-0.1.1/tests/index/__init__.py
+-rw-r--r--   0 xchen375   (502) staff       (20)      784 2023-04-22 17:06:36.000000 embedin-0.1.1/tests/index/test_faiss.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     1635 2023-04-22 17:06:36.000000 embedin-0.1.1/tests/index/test_hnswlib.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-04-22 20:07:35.000908 embedin-0.1.1/tests/model/
+-rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-22 15:16:27.000000 embedin-0.1.1/tests/model/__init__.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     1893 2023-04-22 17:06:36.000000 embedin-0.1.1/tests/model/test_collection_model.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     2043 2023-04-22 17:06:36.000000 embedin-0.1.1/tests/model/test_embedding_model.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-04-22 20:07:35.002691 embedin-0.1.1/tests/repository/
+-rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-22 15:16:27.000000 embedin-0.1.1/tests/repository/__init__.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     2473 2023-04-22 17:06:36.000000 embedin-0.1.1/tests/repository/test_collection_repository.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     5428 2023-04-22 17:06:36.000000 embedin-0.1.1/tests/repository/test_embedding_repository.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-04-22 20:07:35.004499 embedin-0.1.1/tests/service/
+-rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-22 15:16:27.000000 embedin-0.1.1/tests/service/__init__.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     1334 2023-04-22 17:06:36.000000 embedin-0.1.1/tests/service/test_collection_service.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     3656 2023-04-22 17:06:36.000000 embedin-0.1.1/tests/service/test_embedding_service.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-04-22 20:07:35.005144 embedin-0.1.1/tests/util/
+-rw-r--r--   0 xchen375   (502) staff       (20)      660 2023-04-22 17:06:36.000000 embedin-0.1.1/tests/util/__init__.py
```

### Comparing `embedin-0.1.0/LICENSE` & `embedin-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `embedin-0.1.0/PKG-INFO` & `embedin-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: embedin
-Version: 0.1.0
+Version: 0.1.1
 Summary: A lightweight vector database
 Home-page: https://github.com/EmbedInAI/EmbedInDB
 Author: EmbedInAI
 Author-email: EmbedInAI@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# embedin
+# Embedin
 
 ## For development
 
 Clone the repo
 ```bash
 git clone https://github.com/EmbedInAI/embedin.git
 ```
@@ -61,7 +61,16 @@
 ```
 
 Run unit test with coverage report
 ```bash
 coverage run -m unittest discover -s tests -p '*.py'
 coverage report
 ```
+
+To publish to PyPI
+```bash
+pip install twine
+```
+
+```bash
+python setup.py sdist && python setup.py bdist_wheel && twine upload dist/*
+```
```

### Comparing `embedin-0.1.0/README.md` & `embedin-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# embedin
+# Embedin
 
 ## For development
 
 Clone the repo
 ```bash
 git clone https://github.com/EmbedInAI/embedin.git
 ```
@@ -46,8 +46,17 @@
       - "1521:1521"
 ```
 
 Run unit test with coverage report
 ```bash
 coverage run -m unittest discover -s tests -p '*.py'
 coverage report
+```
+
+To publish to PyPI
+```bash
+pip install twine
+```
+
+```bash
+python setup.py sdist && python setup.py bdist_wheel && twine upload dist/*
 ```
```

### Comparing `embedin-0.1.0/embedin.egg-info/PKG-INFO` & `embedin-0.1.1/embedin.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: embedin
-Version: 0.1.0
+Version: 0.1.1
 Summary: A lightweight vector database
 Home-page: https://github.com/EmbedInAI/EmbedInDB
 Author: EmbedInAI
 Author-email: EmbedInAI@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# embedin
+# Embedin
 
 ## For development
 
 Clone the repo
 ```bash
 git clone https://github.com/EmbedInAI/embedin.git
 ```
@@ -61,7 +61,16 @@
 ```
 
 Run unit test with coverage report
 ```bash
 coverage run -m unittest discover -s tests -p '*.py'
 coverage report
 ```
+
+To publish to PyPI
+```bash
+pip install twine
+```
+
+```bash
+python setup.py sdist && python setup.py bdist_wheel && twine upload dist/*
+```
```

### Comparing `embedin-0.1.0/embedin.egg-info/SOURCES.txt` & `embedin-0.1.1/embedin.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 LICENSE
 README.md
 setup.py
+embedin/__init__.py
 embedin.egg-info/PKG-INFO
 embedin.egg-info/SOURCES.txt
 embedin.egg-info/dependency_links.txt
+embedin.egg-info/requires.txt
 embedin.egg-info/top_level.txt
-src/__init__.py
-src/client/__init__.py
-src/embedding/__init__.py
-src/embedding/sentence_transformer.py
-src/index/__init__.py
-src/index/faiss.py
-src/index/hnswlib.py
-src/model/__init__.py
-src/model/collection_model.py
-src/model/embedding_model.py
-src/repository/__init__.py
-src/repository/collection_repository.py
-src/repository/embedding_repository.py
-src/service/__init__.py
-src/service/collection_service.py
-src/service/embedding_service.py
-src/util/__init__.py
+embedin/client/__init__.py
+embedin/embedding/__init__.py
+embedin/embedding/sentence_transformer.py
+embedin/index/__init__.py
+embedin/index/faiss.py
+embedin/index/hnswlib.py
+embedin/model/__init__.py
+embedin/model/collection_model.py
+embedin/model/embedding_model.py
+embedin/repository/__init__.py
+embedin/repository/collection_repository.py
+embedin/repository/embedding_repository.py
+embedin/service/__init__.py
+embedin/service/collection_service.py
+embedin/service/embedding_service.py
+embedin/util/__init__.py
 tests/__init__.py
 tests/client/__init__.py
 tests/embedding/__init__.py
 tests/embedding/test_embedding.py
 tests/index/__init__.py
 tests/index/test_faiss.py
 tests/index/test_hnswlib.py
```

### Comparing `embedin-0.1.0/src/client/__init__.py` & `embedin-0.1.1/embedin/client/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
 
 from sqlalchemy import create_engine
 from sqlalchemy.orm import sessionmaker
 
-from src.embedding.sentence_transformer import SentenceTransformerEmbedding
-from src.index.hnswlib import HNSWNearestNeighbors
-from src.service.collection_service import CollectionService
-from src.service.embedding_service import EmbeddingService
+from embedin.embedding.sentence_transformer import SentenceTransformerEmbedding
+from embedin.index.hnswlib import HNSWNearestNeighbors
+from embedin.service.collection_service import CollectionService
+from embedin.service.embedding_service import EmbeddingService
 
 # Configure the root logger to output to the console
 logging.basicConfig(format='%(asctime)s - %(levelname)s - %(message)s',
                     level=logging.INFO)
 
 logger = logging.getLogger(__name__)
```

### Comparing `embedin-0.1.0/src/embedding/sentence_transformer.py` & `embedin-0.1.1/embedin/embedding/sentence_transformer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from sentence_transformers import SentenceTransformer
 
-from src.embedding import Embedding
+from embedin.embedding import Embedding
 
 
 class SentenceTransformerEmbedding(Embedding):
     def __init__(self, model_name="all-MiniLM-L6-v2"):
         self.model = SentenceTransformer(model_name)
 
     def __call__(self, texts):
```

### Comparing `embedin-0.1.0/src/index/__init__.py` & `embedin-0.1.1/embedin/index/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from abc import ABC, abstractmethod
 
-from src.util import to_np_array
+from embedin.util import to_np_array
 
 
 class NearestNeighbors(ABC):
     def __init__(self, embeddings):
         """
         Args:
             embeddings: A list of embeddings, where each embedding is a list
```

### Comparing `embedin-0.1.0/src/index/hnswlib.py` & `embedin-0.1.1/embedin/index/hnswlib.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 from hnswlib import Index as HNSWIndex
-from src.index import NearestNeighbors, to_np_array
+from embedin.index import NearestNeighbors, to_np_array
 
 
 class HNSWNearestNeighbors(NearestNeighbors):
     # TODO: save index to DB; load index from DB
     def _build_index(self):
         # TODO: double check all those magic numbers
         index = HNSWIndex('cosine', self.embeddings.shape[1])
```

### Comparing `embedin-0.1.0/src/model/embedding_model.py` & `embedin-0.1.1/embedin/model/embedding_model.py`

 * *Files identical despite different names*

### Comparing `embedin-0.1.0/src/repository/collection_repository.py` & `embedin-0.1.1/embedin/repository/collection_repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import uuid
 
-from src.model.collection_model import CollectionModel
+from embedin.model.collection_model import CollectionModel
 
 
 class CollectionRepository:
     def __init__(self, session):
         self.session = session
         self.create_table()
```

### Comparing `embedin-0.1.0/src/repository/embedding_repository.py` & `embedin-0.1.1/embedin/repository/embedding_repository.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from sqlalchemy.exc import IntegrityError
 
-from src.model.embedding_model import EmbeddingModel
+from embedin.model.embedding_model import EmbeddingModel
 
 
 class EmbeddingRepository:
     def __init__(self, session):
         self.session = session
         self.create_table()
```

### Comparing `embedin-0.1.0/src/service/embedding_service.py` & `embedin-0.1.1/embedin/service/embedding_service.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import hashlib
 import json
 import uuid
 from datetime import datetime
 
-from src.model.embedding_model import EmbeddingModel
-from src.repository.embedding_repository import EmbeddingRepository
+from embedin.model.embedding_model import EmbeddingModel
+from embedin.repository.embedding_repository import EmbeddingRepository
 
 
 class EmbeddingService:
     def __init__(self, session):
         self.embedding_repo = EmbeddingRepository(session)
 
     def add_all(self, collection_id, embeddings, texts, metadata_list=None):
```

### Comparing `embedin-0.1.0/src/util/__init__.py` & `embedin-0.1.1/embedin/util/__init__.py`

 * *Files identical despite different names*

### Comparing `embedin-0.1.0/tests/client/__init__.py` & `embedin-0.1.1/tests/client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 from unittest.mock import MagicMock
-from src.client import Client
+from embedin.client import Client
 
 
 class TestClient(unittest.TestCase):
     def setUp(self):
         self.client = Client(collection_name='test_collection',
                              embedding_fn=MagicMock(return_value=[[1, 2, 3], [4, 5, 6]]))
```

### Comparing `embedin-0.1.0/tests/embedding/test_embedding.py` & `embedin-0.1.1/tests/embedding/test_embedding.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 
-from src.embedding.sentence_transformer import SentenceTransformerEmbedding
+from embedin.embedding.sentence_transformer import SentenceTransformerEmbedding
 
 
 class TestSentenceTransformerEmbedding(unittest.TestCase):
     def test_embedding_single_text(self):
         embedding = SentenceTransformerEmbedding()
         text = "This is a test sentence."
         expected_output = embedding.model.encode([text], convert_to_numpy=True)
```

### Comparing `embedin-0.1.0/tests/index/test_faiss.py` & `embedin-0.1.1/tests/index/test_faiss.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
 
 import numpy as np
 
 import faiss
-from src.index.faiss import FaissNearestNeighbors
+from embedin.index.faiss import FaissNearestNeighbors
 
 
 class TestFaissNearestNeighbors(unittest.TestCase):
     def setUp(self):
         self.embeddings = [
             [1, 2, 3],
             [4, 5, 6],
```

### Comparing `embedin-0.1.0/tests/index/test_hnswlib.py` & `embedin-0.1.1/tests/index/test_hnswlib.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
 
 import numpy as np
 
 from hnswlib import Index as HNSWIndex
-from src.index.hnswlib import HNSWNearestNeighbors
+from embedin.index.hnswlib import HNSWNearestNeighbors
 
 
 class TestHNSWNearestNeighbors(unittest.TestCase):
     def setUp(self):
         self.embeddings = [
             [1, 2, 3],
             [4, 5, 6],
```

### Comparing `embedin-0.1.0/tests/model/test_collection_model.py` & `embedin-0.1.1/tests/model/test_collection_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest
 from sqlalchemy import create_engine
 from sqlalchemy.orm import sessionmaker
 
-from src.model.collection_model import CollectionModel, Base
+from embedin.model.collection_model import CollectionModel, Base
 
 engine = create_engine('sqlite:///:memory:', echo=True)
 Session = sessionmaker(bind=engine)
 
 
 class TestCollectionModel(unittest.TestCase):
```

### Comparing `embedin-0.1.0/tests/model/test_embedding_model.py` & `embedin-0.1.1/tests/model/test_embedding_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
 from datetime import datetime
 from sqlalchemy import create_engine
 from sqlalchemy.orm import sessionmaker
 
-from src.model.embedding_model import Base, EmbeddingModel
+from embedin.model.embedding_model import Base, EmbeddingModel
 
 engine = create_engine('sqlite:///:memory:', echo=True)
 Session = sessionmaker(bind=engine)
 
 
 class EmbeddingModelTestCase(unittest.TestCase):
```

### Comparing `embedin-0.1.0/tests/repository/test_collection_repository.py` & `embedin-0.1.1/tests/repository/test_collection_repository.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from unittest import TestCase, mock
 from unittest.mock import Mock, patch
 
-from src.model.collection_model import CollectionModel
-from src.repository.collection_repository import CollectionRepository
+from embedin.model.collection_model import CollectionModel
+from embedin.repository.collection_repository import CollectionRepository
 
 
 class TestCollectionRepository(TestCase):
 
     def setUp(self):
         self.session_mock = Mock()
         self.repo = CollectionRepository(self.session_mock)
```

### Comparing `embedin-0.1.0/tests/repository/test_embedding_repository.py` & `embedin-0.1.1/tests/repository/test_embedding_repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from datetime import datetime
 from unittest import TestCase
 
 from sqlalchemy import create_engine
 from sqlalchemy.orm import sessionmaker
 
-from src.model.embedding_model import EmbeddingModel, Base
-from src.repository.embedding_repository import EmbeddingRepository
+from embedin.model.embedding_model import EmbeddingModel, Base
+from embedin.repository.embedding_repository import EmbeddingRepository
 
 engine = create_engine('sqlite:///:memory:', echo=True)
 Session = sessionmaker(bind=engine)
 
 
 class TestEmbeddingRepository(TestCase):
     def setUp(self):
```

### Comparing `embedin-0.1.0/tests/service/test_collection_service.py` & `embedin-0.1.1/tests/service/test_collection_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 from unittest.mock import Mock
-from src.repository.collection_repository import CollectionRepository
-from src.service.collection_service import CollectionService
+from embedin.repository.collection_repository import CollectionRepository
+from embedin.service.collection_service import CollectionService
 
 
 class TestCollectionService(unittest.TestCase):
 
     def setUp(self):
         self.session = Mock()
         self.collection_repo = CollectionRepository(self.session)
```

### Comparing `embedin-0.1.0/tests/service/test_embedding_service.py` & `embedin-0.1.1/tests/service/test_embedding_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import unittest
 from datetime import datetime
 from unittest.mock import Mock
 
-from src.model.embedding_model import EmbeddingModel
-from src.repository.collection_repository import CollectionRepository
-from src.repository.embedding_repository import EmbeddingRepository
-from src.service.embedding_service import EmbeddingService
+from embedin.model.embedding_model import EmbeddingModel
+from embedin.repository.collection_repository import CollectionRepository
+from embedin.repository.embedding_repository import EmbeddingRepository
+from embedin.service.embedding_service import EmbeddingService
 
 
 class TestEmbeddingService(unittest.TestCase):
 
     def setUp(self):
         self.session = Mock()
         self.embedding_repo = EmbeddingRepository(self.session)
```

### Comparing `embedin-0.1.0/tests/util/__init__.py` & `embedin-0.1.1/tests/util/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 
-from src.index import to_np_array
+from embedin.index import to_np_array
 
 
 class TestToNpArray(unittest.TestCase):
     def test_to_np_array_one_dim(self):
         query_embeddings = [1, 2, 3]
         result = to_np_array(query_embeddings)
         assert result.shape == (1, 3)
```

