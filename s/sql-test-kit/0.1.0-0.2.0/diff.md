# Comparing `tmp/sql_test_kit-0.1.0.tar.gz` & `tmp/sql_test_kit-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sql_test_kit-0.1.0.tar", max compression
+gzip compressed data, was "sql_test_kit-0.2.0.tar", max compression
```

## Comparing `sql_test_kit-0.1.0.tar` & `sql_test_kit-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0       59 2023-04-22 22:07:39.934506 sql_test_kit-0.1.0/README.md
--rw-r--r--   0        0        0      455 2023-04-22 22:07:39.943736 sql_test_kit-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-22 16:35:05.194500 sql_test_kit-0.1.0/sql_test_kit/__init__.py
--rw-r--r--   0        0        0      115 2023-04-22 22:03:27.645182 sql_test_kit-0.1.0/sql_test_kit/column.py
--rw-r--r--   0        0        0     1154 2023-04-22 21:50:14.637594 sql_test_kit-0.1.0/sql_test_kit/query_interpolation.py
--rw-r--r--   0        0        0      151 2023-04-22 22:08:51.220061 sql_test_kit-0.1.0/sql_test_kit/schema.py
--rw-r--r--   0        0        0      396 2023-04-22 21:34:00.502769 sql_test_kit-0.1.0/sql_test_kit/table.py
--rw-r--r--   0        0        0      692 1970-01-01 00:00:00.000000 sql_test_kit-0.1.0/setup.py
--rw-r--r--   0        0        0      473 1970-01-01 00:00:00.000000 sql_test_kit-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    13595 2023-04-23 14:08:45.896932 sql_test_kit-0.2.0/LICENSE
+-rw-r--r--   0        0        0      502 2023-04-23 14:57:57.897057 sql_test_kit-0.2.0/README.md
+-rw-r--r--   0        0        0      580 2023-04-23 14:52:02.831967 sql_test_kit-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      229 2023-04-23 11:25:03.317853 sql_test_kit-0.2.0/sql_test_kit/__init__.py
+-rw-r--r--   0        0        0      371 2023-04-23 14:42:07.639950 sql_test_kit-0.2.0/sql_test_kit/bigquery.py
+-rw-r--r--   0        0        0      115 2023-04-22 22:03:27.645182 sql_test_kit-0.2.0/sql_test_kit/column.py
+-rw-r--r--   0        0        0     1263 2023-04-23 14:34:33.086277 sql_test_kit-0.2.0/sql_test_kit/query_interpolation.py
+-rw-r--r--   0        0        0      481 2023-04-23 14:34:33.094879 sql_test_kit-0.2.0/sql_test_kit/table.py
+-rw-r--r--   0        0        0     1233 1970-01-01 00:00:00.000000 sql_test_kit-0.2.0/setup.py
+-rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 sql_test_kit-0.2.0/PKG-INFO
```

### Comparing `sql_test_kit-0.1.0/sql_test_kit/query_interpolation.py` & `sql_test_kit-0.2.0/sql_test_kit/query_interpolation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,46 @@
 from dataclasses import dataclass
 from typing import List
 
 import pandas as pd
 
-from sql_test_kit.table import Table
+from sql_test_kit.table import AbstractTable
 
 
 @dataclass
 class InterpolationData:
-    table: Table
+    table: AbstractTable
     data: pd.DataFrame
 
 
-def replace_table_names_in_string_by_data_literals(query: str,
-                                                   interpolation_data_list: List[InterpolationData]) -> str:
+def replace_table_names_in_string_by_data_literals(
+    query: str, interpolation_data_list: List[InterpolationData]
+) -> str:
     interpolated_query = query
     for interpolation_data in interpolation_data_list:
-        interpolated_query = interpolated_query.replace(interpolation_data.table.table_path,
-                                                        get_data_literals_query(interpolation_data))
+        interpolated_query = interpolated_query.replace(
+            interpolation_data.table.table_path,
+            get_data_literals_query(interpolation_data),
+        )
     return interpolated_query
 
 
 def get_data_literals_query(interpolation_data: InterpolationData) -> str:
     data_dict_list = interpolation_data.data.to_dict(orient="records")
-    columns = interpolation_data.table.schema.columns
+    columns = interpolation_data.table.columns
 
-    return "(\n\t\t\t" + "\n\t\tUNION ALL\n\t\t\t".join([
-        "SELECT " + ", ".join([
-            f"CAST(\"{record[column.name]}\" AS {column.type}) AS {column.name}"
-            for column in columns
-        ])
-        for record in data_dict_list
-    ]) + "\n\t\t)"
+    return (
+        "(\n\t\t\t"
+        + "\n\t\tUNION ALL\n\t\t\t".join(
+            [
+                "SELECT "
+                + ", ".join(
+                    [
+                        f'CAST("{record[column.name]}" AS {column.type}) AS {column.name}'
+                        for column in columns
+                    ]
+                )
+                for record in data_dict_list
+            ]
+        )
+        + "\n\t\t)"
+    )
```

