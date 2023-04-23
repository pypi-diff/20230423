# Comparing `tmp/sql_test_kit-0.2.1.tar.gz` & `tmp/sql_test_kit-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sql_test_kit-0.2.1.tar", max compression
+gzip compressed data, was "sql_test_kit-0.2.2.tar", max compression
```

## Comparing `sql_test_kit-0.2.1.tar` & `sql_test_kit-0.2.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    13595 2023-04-23 14:08:45.896932 sql_test_kit-0.2.1/LICENSE
--rw-r--r--   0        0        0      502 2023-04-23 14:57:57.897057 sql_test_kit-0.2.1/README.md
--rw-r--r--   0        0        0      580 2023-04-23 15:13:55.992759 sql_test_kit-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      229 2023-04-23 11:25:03.317853 sql_test_kit-0.2.1/sql_test_kit/__init__.py
--rw-r--r--   0        0        0      371 2023-04-23 14:42:07.639950 sql_test_kit-0.2.1/sql_test_kit/bigquery.py
--rw-r--r--   0        0        0      115 2023-04-22 22:03:27.645182 sql_test_kit-0.2.1/sql_test_kit/column.py
--rw-r--r--   0        0        0     1263 2023-04-23 14:34:33.086277 sql_test_kit-0.2.1/sql_test_kit/query_interpolation.py
--rw-r--r--   0        0        0      390 2023-04-23 15:12:13.214333 sql_test_kit-0.2.1/sql_test_kit/table.py
--rw-r--r--   0        0        0     1233 1970-01-01 00:00:00.000000 sql_test_kit-0.2.1/setup.py
--rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 sql_test_kit-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    13595 2023-04-23 14:08:45.896932 sql_test_kit-0.2.2/LICENSE
+-rw-r--r--   0        0        0      502 2023-04-23 14:57:57.897057 sql_test_kit-0.2.2/README.md
+-rw-r--r--   0        0        0      580 2023-04-23 15:20:23.974682 sql_test_kit-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      229 2023-04-23 11:25:03.317853 sql_test_kit-0.2.2/sql_test_kit/__init__.py
+-rw-r--r--   0        0        0      371 2023-04-23 14:42:07.639950 sql_test_kit-0.2.2/sql_test_kit/bigquery.py
+-rw-r--r--   0        0        0      115 2023-04-22 22:03:27.645182 sql_test_kit-0.2.2/sql_test_kit/column.py
+-rw-r--r--   0        0        0     1251 2023-04-23 15:18:31.643186 sql_test_kit-0.2.2/sql_test_kit/query_interpolation.py
+-rw-r--r--   0        0        0      390 2023-04-23 15:12:13.214333 sql_test_kit-0.2.2/sql_test_kit/table.py
+-rw-r--r--   0        0        0     1233 1970-01-01 00:00:00.000000 sql_test_kit-0.2.2/setup.py
+-rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 sql_test_kit-0.2.2/PKG-INFO
```

### Comparing `sql_test_kit-0.2.1/LICENSE` & `sql_test_kit-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sql_test_kit-0.2.1/pyproject.toml` & `sql_test_kit-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sql-test-kit"
-version = "0.2.1"
+version = "0.2.2"
 description = "Framework for testing SQL queries"
 authors = ["victorlandeau <vlandeau@gmail.com>"]
 readme = "README.md"
 packages = [{include = "sql_test_kit"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `sql_test_kit-0.2.1/sql_test_kit/query_interpolation.py` & `sql_test_kit-0.2.2/sql_test_kit/query_interpolation.py`

 * *Files 19% similar despite different names*

```diff
@@ -21,26 +21,26 @@
             interpolation_data.table.table_path,
             get_data_literals_query(interpolation_data),
         )
     return interpolated_query
 
 
 def get_data_literals_query(interpolation_data: InterpolationData) -> str:
-    data_dict_list = interpolation_data.data.to_dict(orient="records")
+    records = interpolation_data.data.to_dict(orient="records")
     columns = interpolation_data.table.columns
 
     return (
         "(\n\t\t\t"
-        + "\n\t\tUNION ALL\n\t\t\t".join(
+        + "\n\t\t\tUNION ALL\n\t\t\t".join(
             [
                 "SELECT "
                 + ", ".join(
                     [
                         f'CAST("{record[column.name]}" AS {column.type}) AS {column.name}'
                         for column in columns
                     ]
                 )
-                for record in data_dict_list
+                for record in records
             ]
         )
         + "\n\t\t)"
     )
```

### Comparing `sql_test_kit-0.2.1/setup.py` & `sql_test_kit-0.2.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = \
 ['db-dtypes[bigquery]>=1.1.1,<2.0.0',
  'google-cloud-bigquery[bigquery]>=3.10.0,<4.0.0',
  'pandas>=2.0.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'sql-test-kit',
-    'version': '0.2.1',
+    'version': '0.2.2',
     'description': 'Framework for testing SQL queries',
     'long_description': '# sql-test-kit\n\nThis is a framework for testing SQL queries.\nIt works by directly running the queries against the targeted engine, thus being robust to any change in the\ncorresponding SQL dialect.\nMoreover, it is currently focused on interpolating test data directly inside the SQL queries, making the test much\nquicker than if it were creating temporary tables.\n\n# Application example\n\nYou can find an example in applying the framework to bigquery in the [test_bigquery](tests/test_bigquery.py) file.\n',
     'author': 'victorlandeau',
     'author_email': 'vlandeau@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `sql_test_kit-0.2.1/PKG-INFO` & `sql_test_kit-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sql-test-kit
-Version: 0.2.1
+Version: 0.2.2
 Summary: Framework for testing SQL queries
 Author: victorlandeau
 Author-email: vlandeau@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

