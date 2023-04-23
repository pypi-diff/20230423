# Comparing `tmp/tap_shiftbase-0.0.1.tar.gz` & `tmp/tap_shiftbase-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_shiftbase-0.0.1.tar", max compression
+gzip compressed data, was "tap_shiftbase-0.0.2.tar", max compression
```

## Comparing `tap_shiftbase-0.0.1.tar` & `tap_shiftbase-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     3110 2023-04-07 11:27:41.183945 tap_shiftbase-0.0.1/README.md
--rw-r--r--   0        0        0     1078 2023-04-07 11:27:41.181174 tap_shiftbase-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       25 2023-04-07 11:27:41.193691 tap_shiftbase-0.0.1/tap_shiftbase/__init__.py
--rw-r--r--   0        0        0     3007 2023-04-21 09:29:36.361842 tap_shiftbase-0.0.1/tap_shiftbase/client.py
--rw-r--r--   0        0        0     1193 2023-04-21 09:42:21.107406 tap_shiftbase-0.0.1/tap_shiftbase/schemas/absentee_options.json
--rw-r--r--   0        0        0     3098 2023-04-21 09:50:05.463768 tap_shiftbase-0.0.1/tap_shiftbase/schemas/absentees.json
--rw-r--r--   0        0        0     1624 2023-04-21 09:57:56.793047 tap_shiftbase-0.0.1/tap_shiftbase/schemas/contract_types.json
--rw-r--r--   0        0        0      821 2023-04-21 10:00:29.836220 tap_shiftbase-0.0.1/tap_shiftbase/schemas/custom_fields.json
--rw-r--r--   0        0        0     3098 2023-04-21 10:04:04.099596 tap_shiftbase-0.0.1/tap_shiftbase/schemas/departments.json
--rw-r--r--   0        0        0  1373258 2023-04-21 13:49:20.419188 tap_shiftbase-0.0.1/tap_shiftbase/schemas/docs.json
--rw-r--r--   0        0        0      732 2023-04-21 10:11:43.835373 tap_shiftbase-0.0.1/tap_shiftbase/schemas/locations.json
--rw-r--r--   0        0        0     1609 2023-04-21 13:24:37.106460 tap_shiftbase-0.0.1/tap_shiftbase/schemas/rosters.json
--rw-r--r--   0        0        0     1268 2023-04-21 13:26:45.360890 tap_shiftbase-0.0.1/tap_shiftbase/schemas/shifts.json
--rw-r--r--   0        0        0     1129 2023-04-21 13:28:07.154236 tap_shiftbase-0.0.1/tap_shiftbase/schemas/teams.json
--rw-r--r--   0        0        0    16474 2023-04-23 13:31:19.307792 tap_shiftbase-0.0.1/tap_shiftbase/schemas/timesheets.json
--rw-r--r--   0        0        0     5838 2023-04-21 09:28:54.524445 tap_shiftbase-0.0.1/tap_shiftbase/schemas/users.json
--rw-r--r--   0        0        0     2435 2023-04-21 13:29:32.513748 tap_shiftbase-0.0.1/tap_shiftbase/streams.py
--rw-r--r--   0        0        0     1571 2023-04-21 13:29:44.823280 tap_shiftbase-0.0.1/tap_shiftbase/tap.py
--rw-r--r--   0        0        0     3858 1970-01-01 00:00:00.000000 tap_shiftbase-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3110 2023-04-07 11:27:41.183945 tap_shiftbase-0.0.2/README.md
+-rw-r--r--   0        0        0     1078 2023-04-23 13:45:23.942986 tap_shiftbase-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       25 2023-04-07 11:27:41.193691 tap_shiftbase-0.0.2/tap_shiftbase/__init__.py
+-rw-r--r--   0        0        0     3007 2023-04-21 09:29:36.361842 tap_shiftbase-0.0.2/tap_shiftbase/client.py
+-rw-r--r--   0        0        0     1193 2023-04-21 09:42:21.107406 tap_shiftbase-0.0.2/tap_shiftbase/schemas/absentee_options.json
+-rw-r--r--   0        0        0     3098 2023-04-21 09:50:05.463768 tap_shiftbase-0.0.2/tap_shiftbase/schemas/absentees.json
+-rw-r--r--   0        0        0     1624 2023-04-21 09:57:56.793047 tap_shiftbase-0.0.2/tap_shiftbase/schemas/contract_types.json
+-rw-r--r--   0        0        0      821 2023-04-21 10:00:29.836220 tap_shiftbase-0.0.2/tap_shiftbase/schemas/custom_fields.json
+-rw-r--r--   0        0        0     3098 2023-04-21 10:04:04.099596 tap_shiftbase-0.0.2/tap_shiftbase/schemas/departments.json
+-rw-r--r--   0        0        0  1373258 2023-04-21 13:49:20.419188 tap_shiftbase-0.0.2/tap_shiftbase/schemas/docs.json
+-rw-r--r--   0        0        0      732 2023-04-21 10:11:43.835373 tap_shiftbase-0.0.2/tap_shiftbase/schemas/locations.json
+-rw-r--r--   0        0        0     1609 2023-04-21 13:24:37.106460 tap_shiftbase-0.0.2/tap_shiftbase/schemas/rosters.json
+-rw-r--r--   0        0        0     1268 2023-04-21 13:26:45.360890 tap_shiftbase-0.0.2/tap_shiftbase/schemas/shifts.json
+-rw-r--r--   0        0        0     1129 2023-04-21 13:28:07.154236 tap_shiftbase-0.0.2/tap_shiftbase/schemas/teams.json
+-rw-r--r--   0        0        0    16474 2023-04-23 13:31:19.307792 tap_shiftbase-0.0.2/tap_shiftbase/schemas/timesheets.json
+-rw-r--r--   0        0        0    11444 2023-04-23 13:45:18.202565 tap_shiftbase-0.0.2/tap_shiftbase/schemas/users.json
+-rw-r--r--   0        0        0     2435 2023-04-21 13:29:32.513748 tap_shiftbase-0.0.2/tap_shiftbase/streams.py
+-rw-r--r--   0        0        0     1571 2023-04-21 13:29:44.823280 tap_shiftbase-0.0.2/tap_shiftbase/tap.py
+-rw-r--r--   0        0        0     3858 1970-01-01 00:00:00.000000 tap_shiftbase-0.0.2/PKG-INFO
```

### Comparing `tap_shiftbase-0.0.1/README.md` & `tap_shiftbase-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-0.0.1/pyproject.toml` & `tap_shiftbase-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tap-shiftbase"
-version = "0.0.1"
+version = "0.0.2"
 description = "`tap-shiftbase` is a Singer tap for shiftbase, built with the Meltano Singer SDK."
 readme = "README.md"
 authors = ["Hidde Stokvis"]
 keywords = [
     "ELT",
     "shiftbase",
 ]
```

### Comparing `tap_shiftbase-0.0.1/tap_shiftbase/client.py` & `tap_shiftbase-0.0.2/tap_shiftbase/client.py`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-0.0.1/tap_shiftbase/schemas/absentee_options.json` & `tap_shiftbase-0.0.2/tap_shiftbase/schemas/absentee_options.json`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-0.0.1/tap_shiftbase/schemas/absentees.json` & `tap_shiftbase-0.0.2/tap_shiftbase/schemas/absentees.json`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-0.0.1/tap_shiftbase/schemas/contract_types.json` & `tap_shiftbase-0.0.2/tap_shiftbase/schemas/contract_types.json`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-0.0.1/tap_shiftbase/schemas/custom_fields.json` & `tap_shiftbase-0.0.2/tap_shiftbase/schemas/custom_fields.json`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-0.0.1/tap_shiftbase/schemas/departments.json` & `tap_shiftbase-0.0.2/tap_shiftbase/schemas/departments.json`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-0.0.1/tap_shiftbase/schemas/docs.json` & `tap_shiftbase-0.0.2/tap_shiftbase/schemas/docs.json`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-0.0.1/tap_shiftbase/schemas/locations.json` & `tap_shiftbase-0.0.2/tap_shiftbase/schemas/locations.json`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-0.0.1/tap_shiftbase/schemas/rosters.json` & `tap_shiftbase-0.0.2/tap_shiftbase/schemas/rosters.json`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-0.0.1/tap_shiftbase/schemas/shifts.json` & `tap_shiftbase-0.0.2/tap_shiftbase/schemas/shifts.json`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-0.0.1/tap_shiftbase/schemas/teams.json` & `tap_shiftbase-0.0.2/tap_shiftbase/schemas/teams.json`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-0.0.1/tap_shiftbase/schemas/timesheets.json` & `tap_shiftbase-0.0.2/tap_shiftbase/schemas/timesheets.json`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-0.0.1/tap_shiftbase/streams.py` & `tap_shiftbase-0.0.2/tap_shiftbase/streams.py`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-0.0.1/tap_shiftbase/tap.py` & `tap_shiftbase-0.0.2/tap_shiftbase/tap.py`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-0.0.1/PKG-INFO` & `tap_shiftbase-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-shiftbase
-Version: 0.0.1
+Version: 0.0.2
 Summary: `tap-shiftbase` is a Singer tap for shiftbase, built with the Meltano Singer SDK.
 License: Apache 2.0
 Keywords: ELT,shiftbase
 Author: Hidde Stokvis
 Requires-Python: >=3.7.1,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

