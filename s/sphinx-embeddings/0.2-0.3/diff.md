# Comparing `tmp/sphinx-embeddings-0.2.tar.gz` & `tmp/sphinx-embeddings-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-embeddings-0.2.tar", last modified: Sun Apr 23 17:22:25 2023, max compression
+gzip compressed data, was "sphinx-embeddings-0.3.tar", last modified: Sun Apr 23 17:32:26 2023, max compression
```

## Comparing `sphinx-embeddings-0.2.tar` & `sphinx-embeddings-0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-04-23 17:22:25.562544 sphinx-embeddings-0.2/
--rw-r--r--   0 kayce    (319046) primarygroup (89939)       59 2023-04-23 17:22:25.562544 sphinx-embeddings-0.2/PKG-INFO
--rw-r--r--   0 kayce    (319046) primarygroup (89939)       19 2023-04-19 18:13:27.000000 sphinx-embeddings-0.2/README.md
--rw-r--r--   0 kayce    (319046) primarygroup (89939)       38 2023-04-23 17:22:25.562544 sphinx-embeddings-0.2/setup.cfg
--rw-r--r--   0 kayce    (319046) primarygroup (89939)      320 2023-04-23 17:21:45.000000 sphinx-embeddings-0.2/setup.py
-drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-04-23 17:22:25.562544 sphinx-embeddings-0.2/sphinx-embeddings/
--rw-r--r--   0 kayce    (319046) primarygroup (89939)     1472 2023-04-23 17:15:53.000000 sphinx-embeddings-0.2/sphinx-embeddings/__init__.py
-drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-04-23 17:22:25.562544 sphinx-embeddings-0.2/sphinx_embeddings.egg-info/
--rw-r--r--   0 kayce    (319046) primarygroup (89939)       59 2023-04-23 17:22:25.000000 sphinx-embeddings-0.2/sphinx_embeddings.egg-info/PKG-INFO
--rw-r--r--   0 kayce    (319046) primarygroup (89939)      252 2023-04-23 17:22:25.000000 sphinx-embeddings-0.2/sphinx_embeddings.egg-info/SOURCES.txt
--rw-r--r--   0 kayce    (319046) primarygroup (89939)        1 2023-04-23 17:22:25.000000 sphinx-embeddings-0.2/sphinx_embeddings.egg-info/dependency_links.txt
--rw-r--r--   0 kayce    (319046) primarygroup (89939)      842 2023-04-23 17:22:25.000000 sphinx-embeddings-0.2/sphinx_embeddings.egg-info/requires.txt
--rw-r--r--   0 kayce    (319046) primarygroup (89939)       18 2023-04-23 17:22:25.000000 sphinx-embeddings-0.2/sphinx_embeddings.egg-info/top_level.txt
+drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-04-23 17:32:26.389909 sphinx-embeddings-0.3/
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)       59 2023-04-23 17:32:26.389909 sphinx-embeddings-0.3/PKG-INFO
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)       19 2023-04-19 18:13:27.000000 sphinx-embeddings-0.3/README.md
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)       38 2023-04-23 17:32:26.389909 sphinx-embeddings-0.3/setup.cfg
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)      320 2023-04-23 17:31:41.000000 sphinx-embeddings-0.3/setup.py
+drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-04-23 17:32:26.389909 sphinx-embeddings-0.3/sphinx-embeddings/
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)     1471 2023-04-23 17:31:33.000000 sphinx-embeddings-0.3/sphinx-embeddings/__init__.py
+drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-04-23 17:32:26.389909 sphinx-embeddings-0.3/sphinx_embeddings.egg-info/
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)       59 2023-04-23 17:32:26.000000 sphinx-embeddings-0.3/sphinx_embeddings.egg-info/PKG-INFO
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)      252 2023-04-23 17:32:26.000000 sphinx-embeddings-0.3/sphinx_embeddings.egg-info/SOURCES.txt
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)        1 2023-04-23 17:32:26.000000 sphinx-embeddings-0.3/sphinx_embeddings.egg-info/dependency_links.txt
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)      842 2023-04-23 17:32:26.000000 sphinx-embeddings-0.3/sphinx_embeddings.egg-info/requires.txt
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)       18 2023-04-23 17:32:26.000000 sphinx-embeddings-0.3/sphinx_embeddings.egg-info/top_level.txt
```

### Comparing `sphinx-embeddings-0.2/sphinx-embeddings/__init__.py` & `sphinx-embeddings-0.3/sphinx-embeddings/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from docutils import nodes
 from hashlib import md5
 from json import dump, load
-import tiktokenA
+import tiktoken
 from os import environ
 
 def estimate_token_count(text):
     return len(encoding.encode(text))
 
 def generate_embeddings(app, doctree, docname):
     encoding = tiktoken.get_encoding('cl100k_base')
```

### Comparing `sphinx-embeddings-0.2/sphinx_embeddings.egg-info/requires.txt` & `sphinx-embeddings-0.3/sphinx_embeddings.egg-info/requires.txt`

 * *Files identical despite different names*

