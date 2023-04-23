# Comparing `tmp/tap_shiftbase-0.0.8.tar.gz` & `tmp/tap_shiftbase-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_shiftbase-0.0.8.tar", max compression
+gzip compressed data, was "tap_shiftbase-0.0.9.tar", max compression
```

## Comparing `tap_shiftbase-0.0.8.tar` & `tap_shiftbase-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     3110 2023-04-07 11:27:41.183945 tap_shiftbase-0.0.8/README.md
--rw-r--r--   0        0        0     1078 2023-04-23 15:02:22.487637 tap_shiftbase-0.0.8/pyproject.toml
--rw-r--r--   0        0        0       25 2023-04-07 11:27:41.193691 tap_shiftbase-0.0.8/tap_shiftbase/__init__.py
--rw-r--r--   0        0        0     3440 2023-04-23 14:51:42.320155 tap_shiftbase-0.0.8/tap_shiftbase/client.py
--rw-r--r--   0        0        0     1193 2023-04-23 14:51:12.161977 tap_shiftbase-0.0.8/tap_shiftbase/schemas/absentee_options.json
--rw-r--r--   0        0        0     3098 2023-04-23 14:52:20.335499 tap_shiftbase-0.0.8/tap_shiftbase/schemas/absentees.json
--rw-r--r--   0        0        0     1624 2023-04-23 14:56:11.138011 tap_shiftbase-0.0.8/tap_shiftbase/schemas/contract_types.json
--rw-r--r--   0        0        0      821 2023-04-23 14:52:30.815793 tap_shiftbase-0.0.8/tap_shiftbase/schemas/custom_fields.json
--rw-r--r--   0        0        0     3098 2023-04-23 14:52:35.921568 tap_shiftbase-0.0.8/tap_shiftbase/schemas/departments.json
--rw-r--r--   0        0        0  1373258 2023-04-21 13:49:20.419188 tap_shiftbase-0.0.8/tap_shiftbase/schemas/docs.json
--rw-r--r--   0        0        0      732 2023-04-23 14:52:42.342142 tap_shiftbase-0.0.8/tap_shiftbase/schemas/locations.json
--rw-r--r--   0        0        0     1609 2023-04-23 14:52:49.186296 tap_shiftbase-0.0.8/tap_shiftbase/schemas/rosters.json
--rw-r--r--   0        0        0     3699 2023-04-23 14:55:25.002146 tap_shiftbase-0.0.8/tap_shiftbase/schemas/shifts.json
--rw-r--r--   0        0        0     1129 2023-04-23 14:53:30.521959 tap_shiftbase-0.0.8/tap_shiftbase/schemas/teams.json
--rw-r--r--   0        0        0    16267 2023-04-23 14:53:35.064834 tap_shiftbase-0.0.8/tap_shiftbase/schemas/timesheets.json
--rw-r--r--   0        0        0     3675 2023-04-23 14:53:39.566226 tap_shiftbase-0.0.8/tap_shiftbase/schemas/users.json
--rw-r--r--   0        0        0     2461 2023-04-23 15:01:59.477425 tap_shiftbase-0.0.8/tap_shiftbase/streams.py
--rw-r--r--   0        0        0     1571 2023-04-21 13:29:44.823280 tap_shiftbase-0.0.8/tap_shiftbase/tap.py
--rw-r--r--   0        0        0     3858 1970-01-01 00:00:00.000000 tap_shiftbase-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     3110 2023-04-07 11:27:41.183945 tap_shiftbase-0.0.9/README.md
+-rw-r--r--   0        0        0     1078 2023-04-23 15:04:30.531566 tap_shiftbase-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0       25 2023-04-07 11:27:41.193691 tap_shiftbase-0.0.9/tap_shiftbase/__init__.py
+-rw-r--r--   0        0        0     3440 2023-04-23 14:51:42.320155 tap_shiftbase-0.0.9/tap_shiftbase/client.py
+-rw-r--r--   0        0        0     1193 2023-04-23 14:51:12.161977 tap_shiftbase-0.0.9/tap_shiftbase/schemas/absentee_options.json
+-rw-r--r--   0        0        0     3098 2023-04-23 14:52:20.335499 tap_shiftbase-0.0.9/tap_shiftbase/schemas/absentees.json
+-rw-r--r--   0        0        0     1624 2023-04-23 14:56:11.138011 tap_shiftbase-0.0.9/tap_shiftbase/schemas/contract_types.json
+-rw-r--r--   0        0        0      821 2023-04-23 14:52:30.815793 tap_shiftbase-0.0.9/tap_shiftbase/schemas/custom_fields.json
+-rw-r--r--   0        0        0     3098 2023-04-23 14:52:35.921568 tap_shiftbase-0.0.9/tap_shiftbase/schemas/departments.json
+-rw-r--r--   0        0        0  1373258 2023-04-21 13:49:20.419188 tap_shiftbase-0.0.9/tap_shiftbase/schemas/docs.json
+-rw-r--r--   0        0        0      732 2023-04-23 14:52:42.342142 tap_shiftbase-0.0.9/tap_shiftbase/schemas/locations.json
+-rw-r--r--   0        0        0     1609 2023-04-23 14:52:49.186296 tap_shiftbase-0.0.9/tap_shiftbase/schemas/rosters.json
+-rw-r--r--   0        0        0     3699 2023-04-23 14:55:25.002146 tap_shiftbase-0.0.9/tap_shiftbase/schemas/shifts.json
+-rw-r--r--   0        0        0     1129 2023-04-23 14:53:30.521959 tap_shiftbase-0.0.9/tap_shiftbase/schemas/teams.json
+-rw-r--r--   0        0        0    16267 2023-04-23 14:53:35.064834 tap_shiftbase-0.0.9/tap_shiftbase/schemas/timesheets.json
+-rw-r--r--   0        0        0     3675 2023-04-23 14:53:39.566226 tap_shiftbase-0.0.9/tap_shiftbase/schemas/users.json
+-rw-r--r--   0        0        0     2455 2023-04-23 15:04:01.827316 tap_shiftbase-0.0.9/tap_shiftbase/streams.py
+-rw-r--r--   0        0        0     1571 2023-04-21 13:29:44.823280 tap_shiftbase-0.0.9/tap_shiftbase/tap.py
+-rw-r--r--   0        0        0     3858 1970-01-01 00:00:00.000000 tap_shiftbase-0.0.9/PKG-INFO
```

### Comparing `tap_shiftbase-0.0.8/README.md` & `tap_shiftbase-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-0.0.8/pyproject.toml` & `tap_shiftbase-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tap-shiftbase"
-version = "0.0.8"
+version = "0.0.9"
 description = "`tap-shiftbase` is a Singer tap for shiftbase, built with the Meltano Singer SDK."
 readme = "README.md"
 authors = ["Hidde Stokvis"]
 keywords = [
     "ELT",
     "shiftbase",
 ]
```

### Comparing `tap_shiftbase-0.0.8/tap_shiftbase/client.py` & `tap_shiftbase-0.0.9/tap_shiftbase/client.py`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-0.0.8/tap_shiftbase/schemas/absentee_options.json` & `tap_shiftbase-0.0.9/tap_shiftbase/schemas/absentee_options.json`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-0.0.8/tap_shiftbase/schemas/absentees.json` & `tap_shiftbase-0.0.9/tap_shiftbase/schemas/absentees.json`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-0.0.8/tap_shiftbase/schemas/contract_types.json` & `tap_shiftbase-0.0.9/tap_shiftbase/schemas/contract_types.json`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-0.0.8/tap_shiftbase/schemas/custom_fields.json` & `tap_shiftbase-0.0.9/tap_shiftbase/schemas/custom_fields.json`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-0.0.8/tap_shiftbase/schemas/departments.json` & `tap_shiftbase-0.0.9/tap_shiftbase/schemas/departments.json`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-0.0.8/tap_shiftbase/schemas/docs.json` & `tap_shiftbase-0.0.9/tap_shiftbase/schemas/docs.json`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-0.0.8/tap_shiftbase/schemas/locations.json` & `tap_shiftbase-0.0.9/tap_shiftbase/schemas/locations.json`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-0.0.8/tap_shiftbase/schemas/rosters.json` & `tap_shiftbase-0.0.9/tap_shiftbase/schemas/rosters.json`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-0.0.8/tap_shiftbase/schemas/shifts.json` & `tap_shiftbase-0.0.9/tap_shiftbase/schemas/shifts.json`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-0.0.8/tap_shiftbase/schemas/teams.json` & `tap_shiftbase-0.0.9/tap_shiftbase/schemas/teams.json`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-0.0.8/tap_shiftbase/schemas/timesheets.json` & `tap_shiftbase-0.0.9/tap_shiftbase/schemas/timesheets.json`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-0.0.8/tap_shiftbase/schemas/users.json` & `tap_shiftbase-0.0.9/tap_shiftbase/schemas/users.json`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-0.0.8/tap_shiftbase/streams.py` & `tap_shiftbase-0.0.9/tap_shiftbase/streams.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
     primary_keys = ["Users.id"]
     replication_key = None
     schema_filepath = SCHEMAS_DIR / "users.json"
 
 class AbsenteeOptionsStream(shiftbaseStream):
     name = "absentee_options"
     path = "/absentee_options"
-    # primary_keys = ["absenteeoption__id"]
-    # replication_key = None
+    primary_keys = "absenteeoption__id"
+    replication_key = None
     schema_filepath = SCHEMAS_DIR / "absentee_options.json"
 
 class AbsenteesStream(shiftbaseStream):
     name = "absentees"
     path = "/absentees"
     primary_keys = ["id"]
     replication_key = None
```

### Comparing `tap_shiftbase-0.0.8/tap_shiftbase/tap.py` & `tap_shiftbase-0.0.9/tap_shiftbase/tap.py`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-0.0.8/PKG-INFO` & `tap_shiftbase-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-shiftbase
-Version: 0.0.8
+Version: 0.0.9
 Summary: `tap-shiftbase` is a Singer tap for shiftbase, built with the Meltano Singer SDK.
 License: Apache 2.0
 Keywords: ELT,shiftbase
 Author: Hidde Stokvis
 Requires-Python: >=3.7.1,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

