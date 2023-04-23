# Comparing `tmp/xia_engine_sql-0.1.8-cp39-none-win_amd64.whl.zip` & `tmp/xia_engine_sql-0.1.9-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 293363 bytes, number of entries: 7
--rw-r--r--  2.0 unx      171 b- defN 23-Feb-03 21:46 xia_engine_sql/__init__.py
--rw-r--r--  2.0 unx   805376 b- defN 23-Feb-03 21:49 xia_engine_sql/engine.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      155 b- defN 23-Feb-03 21:49 xia_engine_sql-0.1.8.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      669 b- defN 23-Feb-03 21:49 xia_engine_sql-0.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Feb-03 21:49 xia_engine_sql-0.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-Feb-03 21:49 xia_engine_sql-0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      604 b- defN 23-Feb-03 21:49 xia_engine_sql-0.1.8.dist-info/RECORD
-7 files, 807089 bytes uncompressed, 292281 bytes compressed:  63.8%
+Zip file size: 296211 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      171 b- defN 23-Feb-04 21:52 xia_engine_sql/__init__.py
+-rw-r--r--  2.0 unx   817152 b- defN 23-Feb-04 21:56 xia_engine_sql/engine.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      155 b- defN 23-Feb-04 21:56 xia_engine_sql-0.1.9.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      669 b- defN 23-Feb-04 21:56 xia_engine_sql-0.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Feb-04 21:56 xia_engine_sql-0.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-Feb-04 21:56 xia_engine_sql-0.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      604 b- defN 23-Feb-04 21:56 xia_engine_sql-0.1.9.dist-info/RECORD
+7 files, 818865 bytes uncompressed, 295129 bytes compressed:  64.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_engine_sql/__init__.py
 Comment: 
 
 Filename: xia_engine_sql/engine.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_engine_sql-0.1.8.dist-info/LICENSE.txt
+Filename: xia_engine_sql-0.1.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_engine_sql-0.1.8.dist-info/METADATA
+Filename: xia_engine_sql-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: xia_engine_sql-0.1.8.dist-info/WHEEL
+Filename: xia_engine_sql-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: xia_engine_sql-0.1.8.dist-info/top_level.txt
+Filename: xia_engine_sql-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_engine_sql-0.1.8.dist-info/RECORD
+Filename: xia_engine_sql-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_engine_sql/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_engine_sql.engine import SqlEngine, SqliteEngine, SqliteConnectParam
 
 
 __all__ = [
     "SqlEngine", "SqliteEngine", "SqliteConnectParam"
 ]
 
-__version__ = "0.1.8"
+__version__ = "0.1.9"
```

## Comparing `xia_engine_sql-0.1.8.dist-info/METADATA` & `xia_engine_sql-0.1.9.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-engine-sql
-Version: 0.1.8
+Version: 0.1.9
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-engine-sql/0.1.8/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-engine-sql/0.1.9/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_engine_sql-0.1.8.dist-info/RECORD` & `xia_engine_sql-0.1.9.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_engine_sql/__init__.py,sha256=fIjKSN46fyRxYt6Q-RHfgwLW27nnK_mztQhCHqX2Hfw,171
-xia_engine_sql/engine.cp39-win_amd64.pyd,sha256=V-J2_t865TSI5Fliooh5gm-BdOw_nMEkXVvncFR0xGg,805376
-xia_engine_sql-0.1.8.dist-info/LICENSE.txt,sha256=K2i1H9CJVD-zlJG5T8SxvyiOROUkyUC5bhX7a3usFJA,155
-xia_engine_sql-0.1.8.dist-info/METADATA,sha256=uNSDf_sJMuOPzGoQfjdoRIu_el4fhEKA62EJkRNchOY,669
-xia_engine_sql-0.1.8.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
-xia_engine_sql-0.1.8.dist-info/top_level.txt,sha256=h1_hqTerPqRAQlyzQJgg61c-xJeOvLMmlDjskvb4uVA,15
-xia_engine_sql-0.1.8.dist-info/RECORD,,
+xia_engine_sql/__init__.py,sha256=v3A-Uzay3crZs8pE9WPtQl6RqVzTZjYE6BEwvyQLnss,171
+xia_engine_sql/engine.cp39-win_amd64.pyd,sha256=xigpY1e3g5iUuG17XWYoRDEdICmpdqZi6sRPHjWPcHc,817152
+xia_engine_sql-0.1.9.dist-info/LICENSE.txt,sha256=K2i1H9CJVD-zlJG5T8SxvyiOROUkyUC5bhX7a3usFJA,155
+xia_engine_sql-0.1.9.dist-info/METADATA,sha256=o0sCcwbo5m_ESXVJTT3PyT5cFxCnuEDh3lRtMHgj8ts,669
+xia_engine_sql-0.1.9.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
+xia_engine_sql-0.1.9.dist-info/top_level.txt,sha256=h1_hqTerPqRAQlyzQJgg61c-xJeOvLMmlDjskvb4uVA,15
+xia_engine_sql-0.1.9.dist-info/RECORD,,
```

