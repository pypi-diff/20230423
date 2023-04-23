# Comparing `tmp/diambra-engine-2.1.0rc8.tar.gz` & `tmp/diambra-engine-2.1.0rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diambra-engine-2.1.0rc8.tar", last modified: Wed Feb 15 11:59:56 2023, max compression
+gzip compressed data, was "diambra-engine-2.1.0rc9.tar", last modified: Tue Feb 28 11:35:43 2023, max compression
```

## Comparing `diambra-engine-2.1.0rc8.tar` & `diambra-engine-2.1.0rc9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 11:59:56.232907 diambra-engine-2.1.0rc8/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-02-15 11:59:56.232907 diambra-engine-2.1.0rc8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-02-15 11:59:41.000000 diambra-engine-2.1.0rc8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 11:59:56.232907 diambra-engine-2.1.0rc8/diambra/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 11:59:41.000000 diambra-engine-2.1.0rc8/diambra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 11:59:56.232907 diambra-engine-2.1.0rc8/diambra/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-02-15 11:59:41.000000 diambra-engine-2.1.0rc8/diambra/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18922 2023-02-15 11:59:54.000000 diambra-engine-2.1.0rc8/diambra/engine/interface_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12064 2023-02-15 11:59:54.000000 diambra-engine-2.1.0rc8/diambra/engine/interface_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 11:59:56.232907 diambra-engine-2.1.0rc8/diambra_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-02-15 11:59:56.000000 diambra-engine-2.1.0rc8/diambra_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-02-15 11:59:56.000000 diambra-engine-2.1.0rc8/diambra_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 11:59:56.000000 diambra-engine-2.1.0rc8/diambra_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-02-15 11:59:56.000000 diambra-engine-2.1.0rc8/diambra_engine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-15 11:59:56.000000 diambra-engine-2.1.0rc8/diambra_engine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-15 11:59:56.232907 diambra-engine-2.1.0rc8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-02-15 11:59:41.000000 diambra-engine-2.1.0rc8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 11:35:43.628759 diambra-engine-2.1.0rc9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-02-28 11:35:43.628759 diambra-engine-2.1.0rc9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-02-28 11:35:28.000000 diambra-engine-2.1.0rc9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 11:35:43.628759 diambra-engine-2.1.0rc9/diambra/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 11:35:28.000000 diambra-engine-2.1.0rc9/diambra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 11:35:43.628759 diambra-engine-2.1.0rc9/diambra/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-02-28 11:35:28.000000 diambra-engine-2.1.0rc9/diambra/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18922 2023-02-28 11:35:41.000000 diambra-engine-2.1.0rc9/diambra/engine/interface_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12064 2023-02-28 11:35:41.000000 diambra-engine-2.1.0rc9/diambra/engine/interface_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 11:35:43.628759 diambra-engine-2.1.0rc9/diambra_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-02-28 11:35:43.000000 diambra-engine-2.1.0rc9/diambra_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-02-28 11:35:43.000000 diambra-engine-2.1.0rc9/diambra_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 11:35:43.000000 diambra-engine-2.1.0rc9/diambra_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-02-28 11:35:43.000000 diambra-engine-2.1.0rc9/diambra_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-28 11:35:43.000000 diambra-engine-2.1.0rc9/diambra_engine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-28 11:35:43.628759 diambra-engine-2.1.0rc9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-02-28 11:35:28.000000 diambra-engine-2.1.0rc9/setup.py
```

### Comparing `diambra-engine-2.1.0rc8/PKG-INFO` & `diambra-engine-2.1.0rc9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diambra-engine
-Version: 2.1.0rc8
+Version: 2.1.0rc9
 Summary: DIAMBRA™ Arena Engine API Client
 Home-page: https://diambra.ai
 Author: DIAMBRA Team
 Author-email: info@diambra.ai
 License: Custom
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
```

### Comparing `diambra-engine-2.1.0rc8/diambra/engine/interface_pb2.py` & `diambra-engine-2.1.0rc9/diambra/engine/interface_pb2.py`

 * *Files identical despite different names*

### Comparing `diambra-engine-2.1.0rc8/diambra/engine/interface_pb2_grpc.py` & `diambra-engine-2.1.0rc9/diambra/engine/interface_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `diambra-engine-2.1.0rc8/diambra_engine.egg-info/PKG-INFO` & `diambra-engine-2.1.0rc9/diambra_engine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diambra-engine
-Version: 2.1.0rc8
+Version: 2.1.0rc9
 Summary: DIAMBRA™ Arena Engine API Client
 Home-page: https://diambra.ai
 Author: DIAMBRA Team
 Author-email: info@diambra.ai
 License: Custom
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
```

### Comparing `diambra-engine-2.1.0rc8/setup.py` & `diambra-engine-2.1.0rc9/setup.py`

 * *Files identical despite different names*

