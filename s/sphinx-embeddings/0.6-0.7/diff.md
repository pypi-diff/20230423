# Comparing `tmp/sphinx-embeddings-0.6.tar.gz` & `tmp/sphinx-embeddings-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-embeddings-0.6.tar", last modified: Sun Apr 23 17:45:40 2023, max compression
+gzip compressed data, was "sphinx-embeddings-0.7.tar", last modified: Sun Apr 23 17:50:59 2023, max compression
```

## Comparing `sphinx-embeddings-0.6.tar` & `sphinx-embeddings-0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-04-23 17:45:40.814081 sphinx-embeddings-0.6/
--rw-r--r--   0 kayce    (319046) primarygroup (89939)       59 2023-04-23 17:45:40.814081 sphinx-embeddings-0.6/PKG-INFO
--rw-r--r--   0 kayce    (319046) primarygroup (89939)       19 2023-04-19 18:13:27.000000 sphinx-embeddings-0.6/README.md
--rw-r--r--   0 kayce    (319046) primarygroup (89939)       38 2023-04-23 17:45:40.814081 sphinx-embeddings-0.6/setup.cfg
--rw-r--r--   0 kayce    (319046) primarygroup (89939)      320 2023-04-23 17:45:19.000000 sphinx-embeddings-0.6/setup.py
-drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-04-23 17:45:40.814081 sphinx-embeddings-0.6/sphinx-embeddings/
--rw-r--r--   0 kayce    (319046) primarygroup (89939)     1549 2023-04-23 17:45:07.000000 sphinx-embeddings-0.6/sphinx-embeddings/__init__.py
-drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-04-23 17:45:40.814081 sphinx-embeddings-0.6/sphinx_embeddings.egg-info/
--rw-r--r--   0 kayce    (319046) primarygroup (89939)       59 2023-04-23 17:45:40.000000 sphinx-embeddings-0.6/sphinx_embeddings.egg-info/PKG-INFO
--rw-r--r--   0 kayce    (319046) primarygroup (89939)      252 2023-04-23 17:45:40.000000 sphinx-embeddings-0.6/sphinx_embeddings.egg-info/SOURCES.txt
--rw-r--r--   0 kayce    (319046) primarygroup (89939)        1 2023-04-23 17:45:40.000000 sphinx-embeddings-0.6/sphinx_embeddings.egg-info/dependency_links.txt
--rw-r--r--   0 kayce    (319046) primarygroup (89939)      842 2023-04-23 17:45:40.000000 sphinx-embeddings-0.6/sphinx_embeddings.egg-info/requires.txt
--rw-r--r--   0 kayce    (319046) primarygroup (89939)       18 2023-04-23 17:45:40.000000 sphinx-embeddings-0.6/sphinx_embeddings.egg-info/top_level.txt
+drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-04-23 17:50:59.728156 sphinx-embeddings-0.7/
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)       59 2023-04-23 17:50:59.728156 sphinx-embeddings-0.7/PKG-INFO
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)       19 2023-04-19 18:13:27.000000 sphinx-embeddings-0.7/README.md
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)       38 2023-04-23 17:50:59.728156 sphinx-embeddings-0.7/setup.cfg
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)      320 2023-04-23 17:46:55.000000 sphinx-embeddings-0.7/setup.py
+drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-04-23 17:50:59.728156 sphinx-embeddings-0.7/sphinx-embeddings/
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)     1601 2023-04-23 17:46:49.000000 sphinx-embeddings-0.7/sphinx-embeddings/__init__.py
+drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-04-23 17:50:59.728156 sphinx-embeddings-0.7/sphinx_embeddings.egg-info/
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)       59 2023-04-23 17:50:59.000000 sphinx-embeddings-0.7/sphinx_embeddings.egg-info/PKG-INFO
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)      252 2023-04-23 17:50:59.000000 sphinx-embeddings-0.7/sphinx_embeddings.egg-info/SOURCES.txt
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)        1 2023-04-23 17:50:59.000000 sphinx-embeddings-0.7/sphinx_embeddings.egg-info/dependency_links.txt
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)      842 2023-04-23 17:50:59.000000 sphinx-embeddings-0.7/sphinx_embeddings.egg-info/requires.txt
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)       18 2023-04-23 17:50:59.000000 sphinx-embeddings-0.7/sphinx_embeddings.egg-info/top_level.txt
```

### Comparing `sphinx-embeddings-0.6/sphinx-embeddings/__init__.py` & `sphinx-embeddings-0.7/sphinx-embeddings/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from hashlib import md5
 from json import dump, load
 import tiktoken
 from os import environ, path
 from copy import deepcopy
 
 def estimate_token_count(text):
+    encoding = tiktoken.get_encoding('cl100k_base')
     return len(encoding.encode(text))
 
 def generate_embeddings(app, doctree, docname):
     data = read_data()
     encoding = tiktoken.get_encoding('cl100k_base')
     clone = deepcopy(doctree)
     # Remove code blocks
```

### Comparing `sphinx-embeddings-0.6/sphinx_embeddings.egg-info/requires.txt` & `sphinx-embeddings-0.7/sphinx_embeddings.egg-info/requires.txt`

 * *Files identical despite different names*

