# Comparing `tmp/np_queuey-0.1.8.tar.gz` & `tmp/np_queuey-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np_queuey-0.1.8.tar", last modified: Fri Apr 21 18:48:10 2023, max compression
+gzip compressed data, was "np_queuey-0.1.9.tar", last modified: Sat Apr 22 23:27:15 2023, max compression
```

## Comparing `np_queuey-0.1.8.tar` & `np_queuey-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,16 @@
--rw-r--r--   0        0        0      227 2023-04-19 04:15:23.193498 np_queuey-0.1.8/README.md
--rw-r--r--   0        0        0     2495 2023-04-21 18:48:10.734070 np_queuey-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       73 2023-04-19 04:15:23.199506 np_queuey-0.1.8/src/np_queuey/__init__.py
--rw-r--r--   0        0        0        0 2023-04-13 22:30:49.775239 np_queuey-0.1.8/src/np_queuey/hueys/__init__.py
--rw-r--r--   0        0        0     9080 2023-04-21 18:42:21.408358 np_queuey-0.1.8/src/np_queuey/hueys/dynamicrouting_behavior_session_mtrain_upload.py
--rw-r--r--   0        0        0        0 2023-04-13 22:30:49.775239 np_queuey-0.1.8/src/np_queuey/jobs/__init__.py
--rw-r--r--   0        0        0     6936 2023-04-18 18:55:14.478321 np_queuey-0.1.8/src/np_queuey/jobs/dynamicrouting_behavior_session_mtrain_upload.py
--rw-r--r--   0        0        0      262 2023-04-15 22:53:44.311082 np_queuey-0.1.8/src/np_queuey/jobs/run_small_jobs.py
--rw-r--r--   0        0        0     3136 2023-04-19 04:15:23.202499 np_queuey-0.1.8/src/np_queuey/queues.py
--rw-r--r--   0        0        0       51 2023-04-13 23:41:50.828823 np_queuey-0.1.8/src/np_queuey/tasks.py
--rw-r--r--   0        0        0      140 2023-04-19 04:15:23.203497 np_queuey-0.1.8/src/np_queuey/utils.py
--rw-r--r--   0        0        0      593 2023-04-19 04:15:23.204497 np_queuey-0.1.8/tests/test_huey.py
--rw-r--r--   0        0        0     1731 1970-01-01 00:00:00.000000 np_queuey-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      227 2023-04-19 04:15:23.193498 np_queuey-0.1.9/README.md
+-rw-r--r--   0        0        0     2543 2023-04-22 23:27:15.823603 np_queuey-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       73 2023-04-19 04:15:23.199506 np_queuey-0.1.9/src/np_queuey/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 22:30:49.775239 np_queuey-0.1.9/src/np_queuey/hueys/__init__.py
+-rw-r--r--   0        0        0     9080 2023-04-21 18:42:21.408358 np_queuey-0.1.9/src/np_queuey/hueys/dynamicrouting_behavior_session_mtrain_upload.py
+-rw-r--r--   0        0        0     3080 2023-04-22 23:23:37.320022 np_queuey-0.1.9/src/np_queuey/hueys/sorting.py
+-rw-r--r--   0        0        0        0 2023-04-13 22:30:49.775239 np_queuey-0.1.9/src/np_queuey/jobs/__init__.py
+-rw-r--r--   0        0        0     6934 2023-04-22 06:53:15.575715 np_queuey-0.1.9/src/np_queuey/jobs/dynamicrouting_behavior_session_mtrain_upload.py
+-rw-r--r--   0        0        0      262 2023-04-15 22:53:44.311082 np_queuey-0.1.9/src/np_queuey/jobs/run_small_jobs.py
+-rw-r--r--   0        0        0      224 2023-04-22 23:11:08.240455 np_queuey-0.1.9/src/np_queuey/jobs/run_sorting.py
+-rw-r--r--   0        0        0    10449 2023-04-22 23:24:10.301324 np_queuey-0.1.9/src/np_queuey/jobs/sorting.py
+-rw-r--r--   0        0        0     3136 2023-04-19 04:15:23.202499 np_queuey-0.1.9/src/np_queuey/queues.py
+-rw-r--r--   0        0        0       51 2023-04-13 23:41:50.828823 np_queuey-0.1.9/src/np_queuey/tasks.py
+-rw-r--r--   0        0        0      417 2023-04-21 23:15:44.215013 np_queuey-0.1.9/src/np_queuey/utils.py
+-rw-r--r--   0        0        0      593 2023-04-19 04:15:23.204497 np_queuey-0.1.9/tests/test_huey.py
+-rw-r--r--   0        0        0     1731 1970-01-01 00:00:00.000000 np_queuey-0.1.9/PKG-INFO
```

### Comparing `np_queuey-0.1.8/pyproject.toml` & `np_queuey-0.1.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "np_queuey"
-version = "0.1.8"
+version = "0.1.9"
 description = "Tools for submitting and processing jobs through a message queue for Mindscope Neuropixels workflows."
 authors = [
     { name = "Ben Hardcastle", email = "ben.hardcastle@alleninstitute.org" },
 ]
 dependencies = [
     "huey>=2.4.5",
     "peewee>=3.16.1",
@@ -28,14 +28,15 @@
 ]
 
 [project.license]
 text = "MIT"
 
 [project.scripts]
 run_small_jobs = "np_queuey.jobs.run_small_jobs:main"
+run_sorting = "np_queuey.jobs.run_sorting:main"
 
 [project.urls]
 Repository = "https://github.com/AllenInstitute/np_queuey"
 "Bug Tracker" = "https://github.com/AllenInstitute/np_queuey/issues"
 
 [project.optional-dependencies]
 dev = [
```

### Comparing `np_queuey-0.1.8/src/np_queuey/hueys/dynamicrouting_behavior_session_mtrain_upload.py` & `np_queuey-0.1.9/src/np_queuey/hueys/dynamicrouting_behavior_session_mtrain_upload.py`

 * *Files identical despite different names*

### Comparing `np_queuey-0.1.8/src/np_queuey/jobs/dynamicrouting_behavior_session_mtrain_upload.py` & `np_queuey-0.1.9/src/np_queuey/jobs/dynamicrouting_behavior_session_mtrain_upload.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 def dynamic_routing_task_db():
     """
     >>> conn = dynamic_routing_task_db()
     >>> _ = conn.cursor()
     """
     conn = sqlite3.connect(DB_PATH, timeout=1)
     conn.isolation_level = None  # autocommit mode
-    conn.execute('pragma journal_mode="truncate"')
+    conn.execute('pragma journal_mode="delete"')
     conn.execute('pragma synchronous=2')
     return conn
 
 
 @contextlib.contextmanager
 def task_db_cursor():
     """
```

### Comparing `np_queuey-0.1.8/src/np_queuey/queues.py` & `np_queuey-0.1.9/src/np_queuey/queues.py`

 * *Files identical despite different names*

### Comparing `np_queuey-0.1.8/tests/test_huey.py` & `np_queuey-0.1.9/tests/test_huey.py`

 * *Files identical despite different names*

### Comparing `np_queuey-0.1.8/PKG-INFO` & `np_queuey-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: np-queuey
-Version: 0.1.8
+Version: 0.1.9
 Summary: Tools for submitting and processing jobs through a message queue for Mindscope Neuropixels workflows.
 Author-Email: Ben Hardcastle <ben.hardcastle@alleninstitute.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

