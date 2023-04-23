# Comparing `tmp/sphinx-embeddings-0.1.tar.gz` & `tmp/sphinx-embeddings-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-embeddings-0.1.tar", last modified: Wed Apr 19 18:35:11 2023, max compression
+gzip compressed data, was "sphinx-embeddings-0.2.tar", last modified: Sun Apr 23 17:22:25 2023, max compression
```

## Comparing `sphinx-embeddings-0.1.tar` & `sphinx-embeddings-0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-04-19 18:35:11.554390 sphinx-embeddings-0.1/
--rw-r--r--   0 kayce    (319046) primarygroup (89939)       59 2023-04-19 18:35:11.554390 sphinx-embeddings-0.1/PKG-INFO
--rw-r--r--   0 kayce    (319046) primarygroup (89939)       19 2023-04-19 18:13:27.000000 sphinx-embeddings-0.1/README.md
--rw-r--r--   0 kayce    (319046) primarygroup (89939)       38 2023-04-19 18:35:11.554390 sphinx-embeddings-0.1/setup.cfg
--rw-r--r--   0 kayce    (319046) primarygroup (89939)      320 2023-04-19 18:16:00.000000 sphinx-embeddings-0.1/setup.py
-drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-04-19 18:35:11.554390 sphinx-embeddings-0.1/sphinx-embeddings/
--rw-r--r--   0 kayce    (319046) primarygroup (89939)      762 2023-04-19 18:33:20.000000 sphinx-embeddings-0.1/sphinx-embeddings/__init__.py
-drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-04-19 18:35:11.554390 sphinx-embeddings-0.1/sphinx_embeddings.egg-info/
--rw-r--r--   0 kayce    (319046) primarygroup (89939)       59 2023-04-19 18:35:11.000000 sphinx-embeddings-0.1/sphinx_embeddings.egg-info/PKG-INFO
--rw-r--r--   0 kayce    (319046) primarygroup (89939)      252 2023-04-19 18:35:11.000000 sphinx-embeddings-0.1/sphinx_embeddings.egg-info/SOURCES.txt
--rw-r--r--   0 kayce    (319046) primarygroup (89939)        1 2023-04-19 18:35:11.000000 sphinx-embeddings-0.1/sphinx_embeddings.egg-info/dependency_links.txt
--rw-r--r--   0 kayce    (319046) primarygroup (89939)      842 2023-04-19 18:35:11.000000 sphinx-embeddings-0.1/sphinx_embeddings.egg-info/requires.txt
--rw-r--r--   0 kayce    (319046) primarygroup (89939)       18 2023-04-19 18:35:11.000000 sphinx-embeddings-0.1/sphinx_embeddings.egg-info/top_level.txt
+drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-04-23 17:22:25.562544 sphinx-embeddings-0.2/
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)       59 2023-04-23 17:22:25.562544 sphinx-embeddings-0.2/PKG-INFO
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)       19 2023-04-19 18:13:27.000000 sphinx-embeddings-0.2/README.md
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)       38 2023-04-23 17:22:25.562544 sphinx-embeddings-0.2/setup.cfg
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)      320 2023-04-23 17:21:45.000000 sphinx-embeddings-0.2/setup.py
+drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-04-23 17:22:25.562544 sphinx-embeddings-0.2/sphinx-embeddings/
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)     1472 2023-04-23 17:15:53.000000 sphinx-embeddings-0.2/sphinx-embeddings/__init__.py
+drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-04-23 17:22:25.562544 sphinx-embeddings-0.2/sphinx_embeddings.egg-info/
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)       59 2023-04-23 17:22:25.000000 sphinx-embeddings-0.2/sphinx_embeddings.egg-info/PKG-INFO
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)      252 2023-04-23 17:22:25.000000 sphinx-embeddings-0.2/sphinx_embeddings.egg-info/SOURCES.txt
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)        1 2023-04-23 17:22:25.000000 sphinx-embeddings-0.2/sphinx_embeddings.egg-info/dependency_links.txt
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)      842 2023-04-23 17:22:25.000000 sphinx-embeddings-0.2/sphinx_embeddings.egg-info/requires.txt
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)       18 2023-04-23 17:22:25.000000 sphinx-embeddings-0.2/sphinx_embeddings.egg-info/top_level.txt
```

### Comparing `sphinx-embeddings-0.1/sphinx_embeddings.egg-info/requires.txt` & `sphinx-embeddings-0.2/sphinx_embeddings.egg-info/requires.txt`

 * *Files identical despite different names*

