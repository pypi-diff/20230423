# Comparing `tmp/pytalentsolution-0.3.2.tar.gz` & `tmp/pytalentsolution-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytalentsolution-0.3.2.tar", last modified: Sun Apr  4 07:36:43 2021, max compression
+gzip compressed data, was "pytalentsolution-0.4.0.tar", max compression
```

## Comparing `pytalentsolution-0.3.2.tar` & `pytalentsolution-0.4.0.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0      771 2021-04-04 07:31:01.938169 pytalentsolution-0.3.2/LICENSE.md
--rw-r--r--   0        0        0      439 2021-04-04 07:36:31.488169 pytalentsolution-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      182 2021-04-04 07:31:01.938169 pytalentsolution-0.3.2/pytalentsolution/__init__.py
--rw-r--r--   0        0        0     2390 2021-04-04 07:36:17.478169 pytalentsolution-0.3.2/pytalentsolution/client_event.py
--rw-r--r--   0        0        0     4899 2021-04-04 07:36:17.538169 pytalentsolution-0.3.2/pytalentsolution/company.py
--rw-r--r--   0        0        0      361 2021-04-04 07:31:38.398169 pytalentsolution-0.3.2/pytalentsolution/config.py
--rw-r--r--   0        0        0     1093 2021-04-04 07:31:01.938169 pytalentsolution-0.3.2/pytalentsolution/cts.py
--rw-r--r--   0        0        0    16982 2021-04-04 07:36:17.508169 pytalentsolution-0.3.2/pytalentsolution/job.py
--rw-r--r--   0        0        0     8490 2021-04-04 07:36:17.448169 pytalentsolution-0.3.2/pytalentsolution/job_search.py
--rw-r--r--   0        0        0    10853 2021-04-04 07:36:17.568169 pytalentsolution-0.3.2/pytalentsolution/profile.py
--rw-r--r--   0        0        0     2071 2021-04-04 07:36:17.408169 pytalentsolution-0.3.2/pytalentsolution/tenant.py
--rw-r--r--   0        0        0      737 2021-04-04 07:36:44.011368 pytalentsolution-0.3.2/setup.py
--rw-r--r--   0        0        0      581 2021-04-04 07:36:44.011587 pytalentsolution-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      771 2023-04-23 10:23:19.200025 pytalentsolution-0.4.0/LICENSE.md
+-rw-r--r--   0        0        0      460 2023-04-23 10:24:54.483498 pytalentsolution-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      182 2023-04-23 10:23:19.202023 pytalentsolution-0.4.0/pytalentsolution/__init__.py
+-rw-r--r--   0        0        0     2390 2023-04-23 10:23:19.202023 pytalentsolution-0.4.0/pytalentsolution/client_event.py
+-rw-r--r--   0        0        0     4899 2023-04-23 10:23:19.203024 pytalentsolution-0.4.0/pytalentsolution/company.py
+-rw-r--r--   0        0        0      361 2023-04-23 10:23:19.203024 pytalentsolution-0.4.0/pytalentsolution/config.py
+-rw-r--r--   0        0        0     1093 2023-04-23 10:23:19.203024 pytalentsolution-0.4.0/pytalentsolution/cts.py
+-rw-r--r--   0        0        0    16982 2023-04-23 10:23:19.204536 pytalentsolution-0.4.0/pytalentsolution/job.py
+-rw-r--r--   0        0        0     8490 2023-04-23 10:23:19.204536 pytalentsolution-0.4.0/pytalentsolution/job_search.py
+-rw-r--r--   0        0        0    10853 2023-04-23 10:23:19.204536 pytalentsolution-0.4.0/pytalentsolution/profile.py
+-rw-r--r--   0        0        0     2071 2023-04-23 10:23:19.205545 pytalentsolution-0.4.0/pytalentsolution/tenant.py
+-rw-r--r--   0        0        0      683 1970-01-01 00:00:00.000000 pytalentsolution-0.4.0/PKG-INFO
```

### Comparing `pytalentsolution-0.3.2/LICENSE.md` & `pytalentsolution-0.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pytalentsolution-0.3.2/pytalentsolution/client_event.py` & `pytalentsolution-0.4.0/pytalentsolution/client_event.py`

 * *Files identical despite different names*

### Comparing `pytalentsolution-0.3.2/pytalentsolution/company.py` & `pytalentsolution-0.4.0/pytalentsolution/company.py`

 * *Files identical despite different names*

### Comparing `pytalentsolution-0.3.2/pytalentsolution/cts.py` & `pytalentsolution-0.4.0/pytalentsolution/cts.py`

 * *Files identical despite different names*

### Comparing `pytalentsolution-0.3.2/pytalentsolution/job.py` & `pytalentsolution-0.4.0/pytalentsolution/job.py`

 * *Files identical despite different names*

### Comparing `pytalentsolution-0.3.2/pytalentsolution/job_search.py` & `pytalentsolution-0.4.0/pytalentsolution/job_search.py`

 * *Files identical despite different names*

### Comparing `pytalentsolution-0.3.2/pytalentsolution/profile.py` & `pytalentsolution-0.4.0/pytalentsolution/profile.py`

 * *Files identical despite different names*

### Comparing `pytalentsolution-0.3.2/pytalentsolution/tenant.py` & `pytalentsolution-0.4.0/pytalentsolution/tenant.py`

 * *Files identical despite different names*

### Comparing `pytalentsolution-0.3.2/PKG-INFO` & `pytalentsolution-0.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: pytalentsolution
-Version: 0.3.2
+Version: 0.4.0
 Summary: 
 License: ISC
 Author: Nutchanon Ninyawee
 Author-email: me@nutchanon.org
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyPika (>=0.43.0,<0.44.0)
 Requires-Dist: fastapi-utils (>=0.2.1,<0.3.0)
 Requires-Dist: google-cloud-talent (>=2.0.0,<3.0.0)
 Requires-Dist: pydantic (>=1.5.1,<2.0.0)
 Requires-Dist: python-dotenv (>=0.15.0,<0.16.0)
```

