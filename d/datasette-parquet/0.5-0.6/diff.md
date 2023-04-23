# Comparing `tmp/datasette-parquet-0.5.tar.gz` & `tmp/datasette-parquet-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasette-parquet-0.5.tar", last modified: Wed Mar  1 23:19:27 2023, max compression
+gzip compressed data, was "datasette-parquet-0.6.tar", last modified: Sun Apr 23 03:48:30 2023, max compression
```

## Comparing `datasette-parquet-0.5.tar` & `datasette-parquet-0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 23:19:27.219607 datasette-parquet-0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-03-01 23:19:07.000000 datasette-parquet-0.5/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-01 23:19:07.000000 datasette-parquet-0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-03-01 23:19:27.219607 datasette-parquet-0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7423 2023-03-01 23:19:07.000000 datasette-parquet-0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 23:19:27.215607 datasette-parquet-0.5/datasette_parquet/
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-03-01 23:19:07.000000 datasette-parquet-0.5/datasette_parquet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-03-01 23:19:07.000000 datasette-parquet-0.5/datasette_parquet/ddl.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-03-01 23:19:07.000000 datasette-parquet-0.5/datasette_parquet/debounce.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-03-01 23:19:07.000000 datasette-parquet-0.5/datasette_parquet/ducky.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-03-01 23:19:07.000000 datasette-parquet-0.5/datasette_parquet/patches.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-03-01 23:19:07.000000 datasette-parquet-0.5/datasette_parquet/rewrite.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-03-01 23:19:07.000000 datasette-parquet-0.5/datasette_parquet/winging_it.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 23:19:27.219607 datasette-parquet-0.5/datasette_parquet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-03-01 23:19:27.000000 datasette-parquet-0.5/datasette_parquet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-03-01 23:19:27.000000 datasette-parquet-0.5/datasette_parquet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 23:19:27.000000 datasette-parquet-0.5/datasette_parquet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-01 23:19:27.000000 datasette-parquet-0.5/datasette_parquet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-01 23:19:27.000000 datasette-parquet-0.5/datasette_parquet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-01 23:19:27.000000 datasette-parquet-0.5/datasette_parquet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-01 23:19:27.219607 datasette-parquet-0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-03-01 23:19:07.000000 datasette-parquet-0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 23:19:27.219607 datasette-parquet-0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-03-01 23:19:07.000000 datasette-parquet-0.5/tests/test_parquet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 03:48:30.944607 datasette-parquet-0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-23 03:48:14.000000 datasette-parquet-0.6/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-23 03:48:14.000000 datasette-parquet-0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-04-23 03:48:30.944607 datasette-parquet-0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7423 2023-04-23 03:48:14.000000 datasette-parquet-0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 03:48:30.944607 datasette-parquet-0.6/datasette_parquet/
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-23 03:48:14.000000 datasette-parquet-0.6/datasette_parquet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-23 03:48:14.000000 datasette-parquet-0.6/datasette_parquet/ddl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-23 03:48:14.000000 datasette-parquet-0.6/datasette_parquet/debounce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-04-23 03:48:14.000000 datasette-parquet-0.6/datasette_parquet/ducky.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-23 03:48:14.000000 datasette-parquet-0.6/datasette_parquet/patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-04-23 03:48:14.000000 datasette-parquet-0.6/datasette_parquet/rewrite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-04-23 03:48:14.000000 datasette-parquet-0.6/datasette_parquet/winging_it.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 03:48:30.944607 datasette-parquet-0.6/datasette_parquet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-04-23 03:48:30.000000 datasette-parquet-0.6/datasette_parquet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-23 03:48:30.000000 datasette-parquet-0.6/datasette_parquet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 03:48:30.000000 datasette-parquet-0.6/datasette_parquet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-23 03:48:30.000000 datasette-parquet-0.6/datasette_parquet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-23 03:48:30.000000 datasette-parquet-0.6/datasette_parquet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-23 03:48:30.000000 datasette-parquet-0.6/datasette_parquet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 03:48:30.944607 datasette-parquet-0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-23 03:48:14.000000 datasette-parquet-0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 03:48:30.944607 datasette-parquet-0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-04-23 03:48:14.000000 datasette-parquet-0.6/tests/test_parquet.py
```

### Comparing `datasette-parquet-0.5/COPYING` & `datasette-parquet-0.6/COPYING`

 * *Files identical despite different names*

### Comparing `datasette-parquet-0.5/LICENSE` & `datasette-parquet-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `datasette-parquet-0.5/PKG-INFO` & `datasette-parquet-0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-parquet
-Version: 0.5
+Version: 0.6
 Summary: Read Parquet files in Datasette
 Home-page: https://github.com/cldellow/datasette-parquet
 Author: Colin Dellow
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/cldellow/datasette-parquet/issues
 Project-URL: CI, https://github.com/cldellow/datasette-parquet/actions
 Project-URL: Changelog, https://github.com/cldellow/datasette-parquet/releases
```

### Comparing `datasette-parquet-0.5/README.md` & `datasette-parquet-0.6/README.md`

 * *Files identical despite different names*

### Comparing `datasette-parquet-0.5/datasette_parquet/__init__.py` & `datasette-parquet-0.6/datasette_parquet/__init__.py`

 * *Files identical despite different names*

### Comparing `datasette-parquet-0.5/datasette_parquet/ddl.py` & `datasette-parquet-0.6/datasette_parquet/ddl.py`

 * *Files identical despite different names*

### Comparing `datasette-parquet-0.5/datasette_parquet/debounce.py` & `datasette-parquet-0.6/datasette_parquet/debounce.py`

 * *Files identical despite different names*

### Comparing `datasette-parquet-0.5/datasette_parquet/ducky.py` & `datasette-parquet-0.6/datasette_parquet/ducky.py`

 * *Files identical despite different names*

### Comparing `datasette-parquet-0.5/datasette_parquet/patches.py` & `datasette-parquet-0.6/datasette_parquet/patches.py`

 * *Files identical despite different names*

### Comparing `datasette-parquet-0.5/datasette_parquet/rewrite.py` & `datasette-parquet-0.6/datasette_parquet/rewrite.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import re
 import sqlglot
 import sqlite3
 table_xinfo_re = re.compile('^PRAGMA table_xinfo[(](.+)[)]')
+table_info_square_re = re.compile('^PRAGMA table_info[(]\[(.+)][)]')
 
 NO_OP_SQL = 'SELECT 0 WHERE 1 = 0'
 
 
 def rewrite(sql):
     # print('rewrite: {}'.format(sql))
 
@@ -48,24 +49,31 @@
         raise sqlite3.DatabaseError()
 
     # DuckDB doesn't support table_xinfo, so use table_info with a faked hidden column
     m = table_xinfo_re.search(sql)
     if m:
         sql = 'SELECT *, 0 FROM pragma_table_info({})'.format(m.group(1))
 
+    m = table_info_square_re.search(sql)
+    if m:
+        sql = 'PRAGMA table_info("{}")'.format(m.group(1))
+
     # DuckDB doesn't support this pragma.
     # Luckily, Parquet doesn't have foreign keys, so just return no rows
     if sql.startswith('PRAGMA foreign_key_list'):
         sql = NO_OP_SQL
 
     # DuckDB doesn't support this pragma.
     # Luckily, Parquet doesn't have indexes, so just return no rows
     if sql.startswith('PRAGMA index_list'):
         sql = NO_OP_SQL
 
+    if sql.startswith('PRAGMA recursive_triggers'):
+        sql = NO_OP_SQL
+
     # This is some query to discover if FTS is enabled?
     if 'VIRTUAL TABLE%USING FTS' in sql:
         sql = NO_OP_SQL
 
     # Transpile queries, eg [test] is not a valid way to quote a table
     # in DuckDB.
     #print('before transpile: {}'.format(sql))
```

### Comparing `datasette-parquet-0.5/datasette_parquet/winging_it.py` & `datasette-parquet-0.6/datasette_parquet/winging_it.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,14 +121,15 @@
 
     def __exit__(self, exc_type,exc_value, exc_traceback):
         pass
 
     def execute(self, sql, parameters=None):
         #print('! params={} sql={}'.format(parameters, sql))
         sql = rewrite(sql)
+        #print('! rewritten sql={}'.format(sql))
         sql, parameters = fixup_params(sql, parameters)
         #print('!! params={} sql={}'.format(parameters, sql))
         rv = self.conn.execute(sql, parameters)
 
         return ProxyCursor(self.conn, rv)
 
     def fetchall(self):
```

### Comparing `datasette-parquet-0.5/datasette_parquet.egg-info/PKG-INFO` & `datasette-parquet-0.6/datasette_parquet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-parquet
-Version: 0.5
+Version: 0.6
 Summary: Read Parquet files in Datasette
 Home-page: https://github.com/cldellow/datasette-parquet
 Author: Colin Dellow
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/cldellow/datasette-parquet/issues
 Project-URL: CI, https://github.com/cldellow/datasette-parquet/actions
 Project-URL: Changelog, https://github.com/cldellow/datasette-parquet/releases
```

### Comparing `datasette-parquet-0.5/setup.py` & `datasette-parquet-0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "0.5"
+VERSION = "0.6"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
```

### Comparing `datasette-parquet-0.5/tests/test_parquet.py` & `datasette-parquet-0.6/tests/test_parquet.py`

 * *Files identical despite different names*

