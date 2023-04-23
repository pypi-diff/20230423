# Comparing `tmp/tap_shiftbase-0.0.5.tar.gz` & `tmp/tap_shiftbase-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_shiftbase-0.0.5.tar", max compression
+gzip compressed data, was "tap_shiftbase-0.0.6.tar", max compression
```

## Comparing `tap_shiftbase-0.0.5.tar` & `tap_shiftbase-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     3110 2023-04-07 11:27:41.183945 tap_shiftbase-0.0.5/README.md
--rw-r--r--   0        0        0     1078 2023-04-23 14:39:53.842021 tap_shiftbase-0.0.5/pyproject.toml
--rw-r--r--   0        0        0       25 2023-04-07 11:27:41.193691 tap_shiftbase-0.0.5/tap_shiftbase/__init__.py
--rw-r--r--   0        0        0     3007 2023-04-21 09:29:36.361842 tap_shiftbase-0.0.5/tap_shiftbase/client.py
--rw-r--r--   0        0        0     1193 2023-04-21 09:42:21.107406 tap_shiftbase-0.0.5/tap_shiftbase/schemas/absentee_options.json
--rw-r--r--   0        0        0     3098 2023-04-21 09:50:05.463768 tap_shiftbase-0.0.5/tap_shiftbase/schemas/absentees.json
--rw-r--r--   0        0        0     1624 2023-04-21 09:57:56.793047 tap_shiftbase-0.0.5/tap_shiftbase/schemas/contract_types.json
--rw-r--r--   0        0        0      821 2023-04-21 10:00:29.836220 tap_shiftbase-0.0.5/tap_shiftbase/schemas/custom_fields.json
--rw-r--r--   0        0        0     3098 2023-04-21 10:04:04.099596 tap_shiftbase-0.0.5/tap_shiftbase/schemas/departments.json
--rw-r--r--   0        0        0  1373258 2023-04-21 13:49:20.419188 tap_shiftbase-0.0.5/tap_shiftbase/schemas/docs.json
--rw-r--r--   0        0        0      732 2023-04-21 10:11:43.835373 tap_shiftbase-0.0.5/tap_shiftbase/schemas/locations.json
--rw-r--r--   0        0        0     1609 2023-04-21 13:24:37.106460 tap_shiftbase-0.0.5/tap_shiftbase/schemas/rosters.json
--rw-r--r--   0        0        0     1268 2023-04-21 13:26:45.360890 tap_shiftbase-0.0.5/tap_shiftbase/schemas/shifts.json
--rw-r--r--   0        0        0     1129 2023-04-21 13:28:07.154236 tap_shiftbase-0.0.5/tap_shiftbase/schemas/teams.json
--rw-r--r--   0        0        0    16267 2023-04-23 14:16:20.237995 tap_shiftbase-0.0.5/tap_shiftbase/schemas/timesheets.json
--rw-r--r--   0        0        0     3675 2023-04-23 14:39:03.985581 tap_shiftbase-0.0.5/tap_shiftbase/schemas/users.json
--rw-r--r--   0        0        0     2457 2023-04-23 14:39:49.179628 tap_shiftbase-0.0.5/tap_shiftbase/streams.py
--rw-r--r--   0        0        0     1571 2023-04-21 13:29:44.823280 tap_shiftbase-0.0.5/tap_shiftbase/tap.py
--rw-r--r--   0        0        0     3858 1970-01-01 00:00:00.000000 tap_shiftbase-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     3110 2023-04-07 11:27:41.183945 tap_shiftbase-0.0.6/README.md
+-rw-r--r--   0        0        0     1078 2023-04-23 14:57:16.106176 tap_shiftbase-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0       25 2023-04-07 11:27:41.193691 tap_shiftbase-0.0.6/tap_shiftbase/__init__.py
+-rw-r--r--   0        0        0     3440 2023-04-23 14:51:42.320155 tap_shiftbase-0.0.6/tap_shiftbase/client.py
+-rw-r--r--   0        0        0     1193 2023-04-23 14:51:12.161977 tap_shiftbase-0.0.6/tap_shiftbase/schemas/absentee_options.json
+-rw-r--r--   0        0        0     3098 2023-04-23 14:52:20.335499 tap_shiftbase-0.0.6/tap_shiftbase/schemas/absentees.json
+-rw-r--r--   0        0        0     1624 2023-04-23 14:56:11.138011 tap_shiftbase-0.0.6/tap_shiftbase/schemas/contract_types.json
+-rw-r--r--   0        0        0      821 2023-04-23 14:52:30.815793 tap_shiftbase-0.0.6/tap_shiftbase/schemas/custom_fields.json
+-rw-r--r--   0        0        0     3098 2023-04-23 14:52:35.921568 tap_shiftbase-0.0.6/tap_shiftbase/schemas/departments.json
+-rw-r--r--   0        0        0  1373258 2023-04-21 13:49:20.419188 tap_shiftbase-0.0.6/tap_shiftbase/schemas/docs.json
+-rw-r--r--   0        0        0      732 2023-04-23 14:52:42.342142 tap_shiftbase-0.0.6/tap_shiftbase/schemas/locations.json
+-rw-r--r--   0        0        0     1609 2023-04-23 14:52:49.186296 tap_shiftbase-0.0.6/tap_shiftbase/schemas/rosters.json
+-rw-r--r--   0        0        0     3699 2023-04-23 14:55:25.002146 tap_shiftbase-0.0.6/tap_shiftbase/schemas/shifts.json
+-rw-r--r--   0        0        0     1129 2023-04-23 14:53:30.521959 tap_shiftbase-0.0.6/tap_shiftbase/schemas/teams.json
+-rw-r--r--   0        0        0    16267 2023-04-23 14:53:35.064834 tap_shiftbase-0.0.6/tap_shiftbase/schemas/timesheets.json
+-rw-r--r--   0        0        0     3675 2023-04-23 14:53:39.566226 tap_shiftbase-0.0.6/tap_shiftbase/schemas/users.json
+-rw-r--r--   0        0        0     2456 2023-04-23 14:57:08.530205 tap_shiftbase-0.0.6/tap_shiftbase/streams.py
+-rw-r--r--   0        0        0     1571 2023-04-21 13:29:44.823280 tap_shiftbase-0.0.6/tap_shiftbase/tap.py
+-rw-r--r--   0        0        0     3858 1970-01-01 00:00:00.000000 tap_shiftbase-0.0.6/PKG-INFO
```

### Comparing `tap_shiftbase-0.0.5/README.md` & `tap_shiftbase-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-0.0.5/pyproject.toml` & `tap_shiftbase-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tap-shiftbase"
-version = "0.0.5"
+version = "0.0.6"
 description = "`tap-shiftbase` is a Singer tap for shiftbase, built with the Meltano Singer SDK."
 readme = "README.md"
 authors = ["Hidde Stokvis"]
 keywords = [
     "ELT",
     "shiftbase",
 ]
```

### Comparing `tap_shiftbase-0.0.5/tap_shiftbase/client.py` & `tap_shiftbase-0.0.6/tap_shiftbase/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -96,7 +96,19 @@
         Args:
             response: The HTTP ``requests.Response`` object.
 
         Yields:
             Each record from the source.
         """
         yield from extract_jsonpath(self.records_jsonpath, input=response.json())
+
+    def post_process(self, row: dict, context: dict | None = None) -> dict | None:
+        """As needed, append or transform raw data to match expected structure.
+
+        Args:
+            row: An individual record from the stream.
+            context: The stream context.
+
+        Returns:
+            The updated record dictionary, or ``None`` to skip the record.
+        """
+        return {k.lower(): v for k, v in row.items()}
```

### Comparing `tap_shiftbase-0.0.5/tap_shiftbase/schemas/absentee_options.json` & `tap_shiftbase-0.0.6/tap_shiftbase/schemas/absentee_options.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.875%*

 * *Differences: {"'properties'": "{replace: OrderedDict([('absenteeoption', OrderedDict([('type', 'object'), "*

 * *                 "('properties', OrderedDict([('id', OrderedDict([('type', 'string'), ('format', "*

 * *                 "'uuid')])), ('account_id', OrderedDict([('type', 'string'), ('format', "*

 * *                 "'uuid')])), ('option', OrderedDict([('type', 'string')])), ('percentage', "*

 * *                 "OrderedDict([('type', 'string')])), ('weight', OrderedDict([('type', "*

 * *                 "'string')])), ('has_vacati […]*

```diff
@@ -1,11 +1,11 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
     "properties": {
-        "AbsenteeOption": {
+        "absenteeoption": {
             "properties": {
                 "account_id": {
                     "format": "uuid",
                     "type": "string"
                 },
                 "color": {
                     "format": "color-hex",
```

### Comparing `tap_shiftbase-0.0.5/tap_shiftbase/schemas/absentees.json` & `tap_shiftbase-0.0.6/tap_shiftbase/schemas/absentees.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.875%*

 * *Differences: {"'properties'": "{replace: OrderedDict([('absentee', OrderedDict([('type', 'object'), "*

 * *                 "('properties', OrderedDict([('id', OrderedDict([('type', 'string'), ('format', "*

 * *                 "'uuid')])), ('account_id', OrderedDict([('type', 'string'), ('format', "*

 * *                 "'uuid')])), ('user_id', OrderedDict([('type', 'string'), ('format', 'uuid')])), "*

 * *                 "('startdate', OrderedDict([('type', 'string'), ('format', 'date')])), "*

 * *                 "('enddate', OrderedDict([ […]*

```diff
@@ -1,11 +1,11 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
     "properties": {
-        "Absentee": {
+        "absentee": {
             "properties": {
                 "absentee_option_id": {
                     "format": "uuid",
                     "type": "string"
                 },
                 "account_id": {
                     "format": "uuid",
@@ -106,15 +106,15 @@
                 },
                 "wait_hours": {
                     "type": "string"
                 }
             },
             "type": "object"
         },
-        "ReviewedBy": {
+        "reviewedby": {
             "properties": {
                 "first_name": {
                     "type": [
                         "string",
                         "null"
                     ]
                 },
```

### Comparing `tap_shiftbase-0.0.5/tap_shiftbase/schemas/contract_types.json` & `tap_shiftbase-0.0.6/tap_shiftbase/schemas/contract_types.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333334%*

 * *Differences: {"'properties'": "{replace: OrderedDict([('contracttype', OrderedDict([('type', 'object'), "*

 * *                 "('properties', OrderedDict([('id', OrderedDict([('type', 'string')])), "*

 * *                 "('account_id', OrderedDict([('type', 'string')])), ('name', "*

 * *                 "OrderedDict([('type', 'string')])), ('plus_min', OrderedDict([('type', "*

 * *                 "'boolean')])), ('vacation_calc_type', OrderedDict([('type', 'string')])), "*

 * *                 "('time_off_accrual_source_hours', OrderedDict […]*

```diff
@@ -1,11 +1,11 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
     "properties": {
-        "ContractType": {
+        "contracttype": {
             "properties": {
                 "absence_calculation": {
                     "type": "string"
                 },
                 "account_id": {
                     "type": "string"
                 },
```

### Comparing `tap_shiftbase-0.0.5/tap_shiftbase/schemas/custom_fields.json` & `tap_shiftbase-0.0.6/tap_shiftbase/schemas/custom_fields.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {"'properties'": "{replace: OrderedDict([('customfield', OrderedDict([('type', 'object'), "*

 * *                 "('properties', OrderedDict([('id', OrderedDict([('type', 'string')])), ('name', "*

 * *                 "OrderedDict([('type', 'string')])), ('description', OrderedDict([('type', "*

 * *                 "'string')])), ('type', OrderedDict([('type', 'string')])), ('applies_to', "*

 * *                 "OrderedDict([('type', 'string')])), ('applies_to_user', OrderedDict([('type', "*

 * *                 "'boolean')])), ( […]*

```diff
@@ -1,10 +1,10 @@
 {
     "properties": {
-        "CustomField": {
+        "customfield": {
             "properties": {
                 "applies_to": {
                     "type": "string"
                 },
                 "applies_to_schedule": {
                     "type": "boolean"
                 },
```

### Comparing `tap_shiftbase-0.0.5/tap_shiftbase/schemas/departments.json` & `tap_shiftbase-0.0.6/tap_shiftbase/schemas/departments.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333334%*

 * *Differences: {"'properties'": "{replace: OrderedDict([('department', OrderedDict([('type', 'object'), "*

 * *                 "('properties', OrderedDict([('id', OrderedDict([('type', 'string')])), "*

 * *                 "('account_id', OrderedDict([('type', 'string')])), ('location_id', "*

 * *                 "OrderedDict([('type', 'string')])), ('address', OrderedDict([('type', "*

 * *                 "'string')])), ('longitude', OrderedDict([('type', 'string')])), ('latitude', "*

 * *                 "OrderedDict([('type', 'string')])), (' […]*

```diff
@@ -1,11 +1,11 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
     "properties": {
-        "Department": {
+        "department": {
             "properties": {
                 "account_id": {
                     "type": "string"
                 },
                 "address": {
                     "type": "string"
                 },
```

### Comparing `tap_shiftbase-0.0.5/tap_shiftbase/schemas/docs.json` & `tap_shiftbase-0.0.6/tap_shiftbase/schemas/docs.json`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-0.0.5/tap_shiftbase/schemas/locations.json` & `tap_shiftbase-0.0.6/tap_shiftbase/schemas/locations.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {"'properties'": "{replace: OrderedDict([('location', OrderedDict([('type', 'object'), "*

 * *                 "('properties', OrderedDict([('id', OrderedDict([('type', 'string')])), "*

 * *                 "('account_id', OrderedDict([('type', 'string')])), ('name', "*

 * *                 "OrderedDict([('type', 'string')])), ('street_address', OrderedDict([('type', "*

 * *                 "'string')])), ('zipcode', OrderedDict([('type', 'string')])), ('city', "*

 * *                 "OrderedDict([('type', 'string')])), ('country' […]*

```diff
@@ -1,10 +1,10 @@
 {
     "properties": {
-        "Location": {
+        "location": {
             "properties": {
                 "account_id": {
                     "type": "string"
                 },
                 "city": {
                     "type": "string"
                 },
```

### Comparing `tap_shiftbase-0.0.5/tap_shiftbase/schemas/rosters.json` & `tap_shiftbase-0.0.6/tap_shiftbase/schemas/rosters.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {"'properties'": "{replace: OrderedDict([('roster', OrderedDict([('type', 'object'), "*

 * *                 "('properties', OrderedDict([('id', OrderedDict([('type', 'string')])), "*

 * *                 "('occurrence_id', OrderedDict([('type', 'string')])), ('department_id', "*

 * *                 "OrderedDict([('type', 'string')])), ('team_id', OrderedDict([('type', "*

 * *                 "'string')])), ('shift_id', OrderedDict([('type', 'string')])), ('user_id', "*

 * *                 "OrderedDict([('type', 'string')])), ('d […]*

```diff
@@ -1,16 +1,16 @@
 {
     "properties": {
-        "Exchange": {
+        "exchange": {
             "type": [
                 "null",
                 "object"
             ]
         },
-        "Roster": {
+        "roster": {
             "properties": {
                 "break": {
                     "type": "string"
                 },
                 "coc": {
                     "type": "number"
                 },
```

### Comparing `tap_shiftbase-0.0.5/tap_shiftbase/schemas/shifts.json` & `tap_shiftbase-0.0.6/tap_shiftbase/schemas/teams.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.375%*

 * *Differences: {"'properties'": "{replace: OrderedDict([('team', OrderedDict([('type', 'object'), ('properties', "*

 * *                 "OrderedDict([('id', OrderedDict([('type', 'string')])), ('account_id', "*

 * *                 "OrderedDict([('type', 'string')])), ('department_id', OrderedDict([('type', "*

 * *                 "'string')])), ('name', OrderedDict([('type', 'string')])), ('created', "*

 * *                 "OrderedDict([('type', 'string'), ('format', 'date-time')])), ('updated', "*

 * *                 "OrderedDict([('type', ' […]*

```diff
@@ -1,75 +1,61 @@
 {
-    "$schema": "http://json-schema.org/draft-07/schema#",
     "properties": {
-        "account_id": {
-            "type": "string"
-        },
-        "break": {
-            "type": "integer"
-        },
-        "color": {
-            "format": "color",
-            "type": "string"
-        },
-        "created": {
-            "format": "date-time",
-            "type": "string"
-        },
-        "created_by": {
-            "type": "string"
-        },
-        "custom_fields": {
+        "team": {
+            "properties": {
+                "account_id": {
+                    "type": "string"
+                },
+                "color": {
+                    "type": "string"
+                },
+                "created": {
+                    "format": "date-time",
+                    "type": "string"
+                },
+                "created_by": {
+                    "type": [
+                        "string",
+                        "null"
+                    ]
+                },
+                "deleted": {
+                    "type": "boolean"
+                },
+                "deleted_date": {
+                    "format": "date-time",
+                    "type": [
+                        "string",
+                        "null"
+                    ]
+                },
+                "department_id": {
+                    "type": "string"
+                },
+                "id": {
+                    "type": "string"
+                },
+                "modified_by": {
+                    "type": [
+                        "string",
+                        "null"
+                    ]
+                },
+                "name": {
+                    "type": "string"
+                },
+                "order": {
+                    "type": "string"
+                },
+                "type": {
+                    "type": "string"
+                },
+                "updated": {
+                    "format": "date-time",
+                    "type": "string"
+                }
+            },
             "type": "object"
-        },
-        "deleted": {
-            "type": "boolean"
-        },
-        "department_id": {
-            "type": "string"
-        },
-        "description": {
-            "type": "string"
-        },
-        "endtime": {
-            "format": "time",
-            "type": "string"
-        },
-        "hide_end_time": {
-            "type": "boolean"
-        },
-        "id": {
-            "type": "string"
-        },
-        "is_task": {
-            "type": "boolean"
-        },
-        "long_name": {
-            "type": "string"
-        },
-        "meals": {
-            "type": "integer"
-        },
-        "modified_by": {
-            "type": "string"
-        },
-        "name": {
-            "type": "string"
-        },
-        "order": {
-            "type": "string"
-        },
-        "rate_card_id": {
-            "type": "string"
-        },
-        "starttime": {
-            "format": "time",
-            "type": "string"
-        },
-        "updated": {
-            "format": "date-time",
-            "type": "string"
         }
     },
-    "title": "Shift",
     "type": "object"
 }
```

### Comparing `tap_shiftbase-0.0.5/tap_shiftbase/schemas/timesheets.json` & `tap_shiftbase-0.0.6/tap_shiftbase/schemas/timesheets.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333334%*

 * *Differences: {"'properties'": "{replace: OrderedDict([('timesheet', OrderedDict([('type', 'object'), "*

 * *                 "('properties', OrderedDict([('id', OrderedDict([('type', 'string'), ('pattern', "*

 * *                 "'^[0-9]+$'), ('readOnly', True)])), ('account_id', OrderedDict([('type', "*

 * *                 "'string'), ('pattern', '^[0-9]+$'), ('readOnly', True)])), ('user_id', "*

 * *                 "OrderedDict([('type', 'string'), ('minLength', 1)])), ('team_id', "*

 * *                 "OrderedDict([('type', 'string'), ( […]*

```diff
@@ -1,11 +1,11 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
     "properties": {
-        "Timesheet": {
+        "timesheet": {
             "ClockBreak": {
                 "items": {
                     "properties": {
                         "account_id": {
                             "pattern": "^[0-9]+$",
                             "readOnly": true,
                             "type": "string"
```

### Comparing `tap_shiftbase-0.0.5/tap_shiftbase/schemas/users.json` & `tap_shiftbase-0.0.6/tap_shiftbase/schemas/users.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5%*

 * *Differences: {"'properties'": "{replace: OrderedDict([('user', OrderedDict([('type', 'object'), ('properties', "*

 * *                 "OrderedDict([('id', OrderedDict([('type', 'string')])), ('account_id', "*

 * *                 "OrderedDict([('type', 'string')])), ('employee_nr', OrderedDict([('type', "*

 * *                 "['string', 'null'])])), ('email', OrderedDict([('type', 'string')])), "*

 * *                 "('birthdate', OrderedDict([('type', ['string', 'null']), ('format', 'date')])), "*

 * *                 "('first_name', Orde […]*

```diff
@@ -1,10 +1,10 @@
 {
     "properties": {
-        "User": {
+        "user": {
             "properties": {
                 "account_id": {
                     "type": "string"
                 },
                 "age": {
                     "type": [
                         "string",
```

### Comparing `tap_shiftbase-0.0.5/tap_shiftbase/streams.py` & `tap_shiftbase-0.0.6/tap_shiftbase/streams.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     primary_keys = ["Users.id"]
     replication_key = None
     schema_filepath = SCHEMAS_DIR / "users.json"
 
 class AbsenteeOptionsStream(shiftbaseStream):
     name = "absentee_options"
     path = "/absentee_options"
-    primary_keys = ["AbsenteeOption__id"]
+    primary_keys = ["absenteeoption.id"]
     replication_key = None
     schema_filepath = SCHEMAS_DIR / "absentee_options.json"
 
 class AbsenteesStream(shiftbaseStream):
     name = "absentees"
     path = "/absentees"
     primary_keys = ["id"]
```

### Comparing `tap_shiftbase-0.0.5/tap_shiftbase/tap.py` & `tap_shiftbase-0.0.6/tap_shiftbase/tap.py`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-0.0.5/PKG-INFO` & `tap_shiftbase-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-shiftbase
-Version: 0.0.5
+Version: 0.0.6
 Summary: `tap-shiftbase` is a Singer tap for shiftbase, built with the Meltano Singer SDK.
 License: Apache 2.0
 Keywords: ELT,shiftbase
 Author: Hidde Stokvis
 Requires-Python: >=3.7.1,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

