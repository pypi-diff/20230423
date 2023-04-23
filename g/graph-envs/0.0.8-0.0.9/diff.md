# Comparing `tmp/graph-envs-0.0.8.tar.gz` & `tmp/graph-envs-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graph-envs-0.0.8.tar", last modified: Wed Feb 15 02:28:04 2023, max compression
+gzip compressed data, was "graph-envs-0.0.9.tar", last modified: Wed Feb 15 02:37:10 2023, max compression
```

## Comparing `graph-envs-0.0.8.tar` & `graph-envs-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 teshnizi   (501) staff       (20)        0 2023-02-15 02:28:04.946160 graph-envs-0.0.8/
--rw-r--r--   0 teshnizi   (501) staff       (20)     1069 2023-02-07 22:43:46.000000 graph-envs-0.0.8/LICENSE
--rw-r--r--   0 teshnizi   (501) staff       (20)     1592 2023-02-15 02:28:04.946221 graph-envs-0.0.8/PKG-INFO
--rw-r--r--   0 teshnizi   (501) staff       (20)     1082 2023-02-15 02:20:00.000000 graph-envs-0.0.8/README.md
--rw-r--r--   0 teshnizi   (501) staff       (20)      106 2023-02-15 00:57:26.000000 graph-envs-0.0.8/pyproject.toml
--rw-r--r--   0 teshnizi   (501) staff       (20)      714 2023-02-15 02:28:04.946692 graph-envs-0.0.8/setup.cfg
-drwxr-xr-x   0 teshnizi   (501) staff       (20)        0 2023-02-15 02:28:04.944490 graph-envs-0.0.8/src/
-drwxr-xr-x   0 teshnizi   (501) staff       (20)        0 2023-02-15 02:28:04.945478 graph-envs-0.0.8/src/graph_envs/
--rw-r--r--   0 teshnizi   (501) staff       (20)     5611 2023-02-07 22:45:03.000000 graph-envs-0.0.8/src/graph_envs/MultiCast.py
--rw-r--r--   0 teshnizi   (501) staff       (20)      284 2023-02-15 02:26:37.000000 graph-envs-0.0.8/src/graph_envs/__init__.py
--rw-r--r--   0 teshnizi   (501) staff       (20)     4235 2023-02-15 02:17:11.000000 graph-envs-0.0.8/src/graph_envs/shortest_path.py
-drwxr-xr-x   0 teshnizi   (501) staff       (20)        0 2023-02-15 02:28:04.946042 graph-envs-0.0.8/src/graph_envs.egg-info/
--rw-r--r--   0 teshnizi   (501) staff       (20)     1592 2023-02-15 02:28:04.000000 graph-envs-0.0.8/src/graph_envs.egg-info/PKG-INFO
--rw-r--r--   0 teshnizi   (501) staff       (20)      281 2023-02-15 02:28:04.000000 graph-envs-0.0.8/src/graph_envs.egg-info/SOURCES.txt
--rw-r--r--   0 teshnizi   (501) staff       (20)        1 2023-02-15 02:28:04.000000 graph-envs-0.0.8/src/graph_envs.egg-info/dependency_links.txt
--rw-r--r--   0 teshnizi   (501) staff       (20)       11 2023-02-15 02:28:04.000000 graph-envs-0.0.8/src/graph_envs.egg-info/top_level.txt
+drwxr-xr-x   0 teshnizi   (501) staff       (20)        0 2023-02-15 02:37:10.576296 graph-envs-0.0.9/
+-rw-r--r--   0 teshnizi   (501) staff       (20)     1069 2023-02-07 22:43:46.000000 graph-envs-0.0.9/LICENSE
+-rw-r--r--   0 teshnizi   (501) staff       (20)     1592 2023-02-15 02:37:10.576367 graph-envs-0.0.9/PKG-INFO
+-rw-r--r--   0 teshnizi   (501) staff       (20)     1082 2023-02-15 02:20:00.000000 graph-envs-0.0.9/README.md
+-rw-r--r--   0 teshnizi   (501) staff       (20)      106 2023-02-15 00:57:26.000000 graph-envs-0.0.9/pyproject.toml
+-rw-r--r--   0 teshnizi   (501) staff       (20)      714 2023-02-15 02:37:10.576697 graph-envs-0.0.9/setup.cfg
+drwxr-xr-x   0 teshnizi   (501) staff       (20)        0 2023-02-15 02:37:10.573377 graph-envs-0.0.9/src/
+drwxr-xr-x   0 teshnizi   (501) staff       (20)        0 2023-02-15 02:37:10.575355 graph-envs-0.0.9/src/graph_envs/
+-rw-r--r--   0 teshnizi   (501) staff       (20)     5611 2023-02-07 22:45:03.000000 graph-envs-0.0.9/src/graph_envs/MultiCast.py
+-rw-r--r--   0 teshnizi   (501) staff       (20)      299 2023-02-15 02:36:47.000000 graph-envs-0.0.9/src/graph_envs/__init__.py
+-rw-r--r--   0 teshnizi   (501) staff       (20)     4235 2023-02-15 02:17:11.000000 graph-envs-0.0.9/src/graph_envs/shortest_path.py
+drwxr-xr-x   0 teshnizi   (501) staff       (20)        0 2023-02-15 02:37:10.576173 graph-envs-0.0.9/src/graph_envs.egg-info/
+-rw-r--r--   0 teshnizi   (501) staff       (20)     1592 2023-02-15 02:37:10.000000 graph-envs-0.0.9/src/graph_envs.egg-info/PKG-INFO
+-rw-r--r--   0 teshnizi   (501) staff       (20)      281 2023-02-15 02:37:10.000000 graph-envs-0.0.9/src/graph_envs.egg-info/SOURCES.txt
+-rw-r--r--   0 teshnizi   (501) staff       (20)        1 2023-02-15 02:37:10.000000 graph-envs-0.0.9/src/graph_envs.egg-info/dependency_links.txt
+-rw-r--r--   0 teshnizi   (501) staff       (20)       11 2023-02-15 02:37:10.000000 graph-envs-0.0.9/src/graph_envs.egg-info/top_level.txt
```

### Comparing `graph-envs-0.0.8/LICENSE` & `graph-envs-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `graph-envs-0.0.8/PKG-INFO` & `graph-envs-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graph-envs
-Version: 0.0.8
+Version: 0.0.9
 Summary: Graph Reinforcement Learning Environments
 Home-page: https://github.com/teshnizi/GraphEnvs
 Author: Teshnizi
 Author-email: teshnizi@stanford.edu
 Project-URL: Bug Tracker, https://github.com/teshnizi/GraphEnvs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `graph-envs-0.0.8/README.md` & `graph-envs-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `graph-envs-0.0.8/setup.cfg` & `graph-envs-0.0.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = graph-envs
-version = 0.0.8
+version = 0.0.9
 author = Teshnizi
 author_email = teshnizi@stanford.edu
 description = Graph Reinforcement Learning Environments
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/teshnizi/GraphEnvs
 project_urls =
```

### Comparing `graph-envs-0.0.8/src/graph_envs/MultiCast.py` & `graph-envs-0.0.9/src/graph_envs/MultiCast.py`

 * *Files identical despite different names*

### Comparing `graph-envs-0.0.8/src/graph_envs/shortest_path.py` & `graph-envs-0.0.9/src/graph_envs/shortest_path.py`

 * *Files identical despite different names*

### Comparing `graph-envs-0.0.8/src/graph_envs.egg-info/PKG-INFO` & `graph-envs-0.0.9/src/graph_envs.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graph-envs
-Version: 0.0.8
+Version: 0.0.9
 Summary: Graph Reinforcement Learning Environments
 Home-page: https://github.com/teshnizi/GraphEnvs
 Author: Teshnizi
 Author-email: teshnizi@stanford.edu
 Project-URL: Bug Tracker, https://github.com/teshnizi/GraphEnvs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

