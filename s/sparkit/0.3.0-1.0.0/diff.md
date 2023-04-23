# Comparing `tmp/sparkit-0.3.0.tar.gz` & `tmp/sparkit-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparkit-0.3.0.tar", max compression
+gzip compressed data, was "sparkit-1.0.0.tar", max compression
```

## Comparing `sparkit-0.3.0.tar` & `sparkit-1.0.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1520 2023-03-20 22:05:31.332862 sparkit-0.3.0/LICENSE
--rw-r--r--   0        0        0     3265 2023-03-20 22:05:31.332862 sparkit-0.3.0/README.md
--rw-r--r--   0        0        0     1191 2023-03-20 22:07:36.849895 sparkit-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      190 2023-03-20 22:05:31.336862 sparkit-0.3.0/src/sparkit/__init__.py
--rw-r--r--   0        0        0     2261 2023-03-20 22:05:31.336862 sparkit-0.3.0/src/sparkit/exception.py
--rw-r--r--   0        0        0    11122 2023-03-20 22:05:31.336862 sparkit-0.3.0/src/sparkit/transformation.py
--rw-r--r--   0        0        0    12732 2023-03-20 22:05:31.336862 sparkit-0.3.0/src/sparkit/validation.py
--rw-r--r--   0        0        0     4134 1970-01-01 00:00:00.000000 sparkit-0.3.0/setup.py
--rw-r--r--   0        0        0     4184 1970-01-01 00:00:00.000000 sparkit-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1520 2023-04-23 21:13:01.764802 sparkit-1.0.0/LICENSE
+-rw-r--r--   0        0        0     3265 2023-04-23 21:13:01.764802 sparkit-1.0.0/README.md
+-rw-r--r--   0        0        0     1191 2023-04-23 21:15:26.837583 sparkit-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      190 2023-04-23 21:13:01.768802 sparkit-1.0.0/src/sparkit/__init__.py
+-rw-r--r--   0        0        0     2261 2023-04-23 21:13:01.768802 sparkit-1.0.0/src/sparkit/exception.py
+-rw-r--r--   0        0        0    19731 2023-04-23 21:13:01.768802 sparkit-1.0.0/src/sparkit/transformation.py
+-rw-r--r--   0        0        0    12756 2023-04-23 21:13:01.768802 sparkit-1.0.0/src/sparkit/validation.py
+-rw-r--r--   0        0        0     4134 1970-01-01 00:00:00.000000 sparkit-1.0.0/setup.py
+-rw-r--r--   0        0        0     4184 1970-01-01 00:00:00.000000 sparkit-1.0.0/PKG-INFO
```

### Comparing `sparkit-0.3.0/LICENSE` & `sparkit-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sparkit-0.3.0/README.md` & `sparkit-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `sparkit-0.3.0/pyproject.toml` & `sparkit-1.0.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sparkit"
-version = "0.3.0"
+version = "1.0.0"
 description = "A package for PySpark utility functions."
 authors = ["sparkit Developers"]
 license = "BSD 3-Clause"
 readme = "README.md"
 repository = "https://github.com/estripling/sparkit"
 documentation = "https://sparkit.readthedocs.io/en/stable/"
 keywords = ["sparkit"]
```

### Comparing `sparkit-0.3.0/src/sparkit/exception.py` & `sparkit-1.0.0/src/sparkit/exception.py`

 * *Files identical despite different names*

### Comparing `sparkit-0.3.0/src/sparkit/validation.py` & `sparkit-1.0.0/src/sparkit/validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "is_dataframe_equal",
     "is_row_count_equal",
     "is_row_equal",
     "is_schema_equal",
 )
 
 
-def check_dataframe_equal(lft_df, rgt_df):
+def check_dataframe_equal(lft_df, rgt_df, /):
     """Validate that the left and right data frames are equal.
 
     Function performs:
         - A schema check
         - A row count check
         - A row content check
 
@@ -91,15 +91,15 @@
     lft_count=2 rgt_count=2
     """
     check_schema_equal(lft_df, rgt_df)
     check_row_count_equal(lft_df, rgt_df)
     check_row_equal(lft_df, rgt_df)
 
 
-def check_row_count_equal(lft_df, rgt_df):
+def check_row_count_equal(lft_df, rgt_df, /):
     """Validate that the row counts of the left and right data frames are equal.
 
     Parameters
     ----------
     lft_df : pyspark.sql.DataFrame
         Left data frame.
     rgt_df : pyspark.sql.DataFrame
@@ -144,15 +144,15 @@
     lft_row_count = lft_df.count()
     rgt_row_count = rgt_df.count()
 
     if lft_row_count != rgt_row_count:
         raise exception.RowCountMismatchError(lft_row_count, rgt_row_count)
 
 
-def check_row_equal(lft_df, rgt_df):
+def check_row_equal(lft_df, rgt_df, /):
     """Validate that the rows of the left and right data frames are equal.
 
     Parameters
     ----------
     lft_df : pyspark.sql.DataFrame
         Left data frame.
     rgt_df : pyspark.sql.DataFrame
@@ -204,15 +204,15 @@
             lft_rows_not_in_rgt,
             rgt_rows_not_in_lft,
             lft_count,
             rgt_count,
         )
 
 
-def check_schema_equal(lft_df, rgt_df):
+def check_schema_equal(lft_df, rgt_df, /):
     """Validate that the schemas of the left and right data frames are equal.
 
     Parameters
     ----------
     lft_df : pyspark.sql.DataFrame
         Left data frame.
     rgt_df : pyspark.sql.DataFrame
@@ -258,15 +258,15 @@
     lft_schema = lft_df.schema.simpleString()
     rgt_schema = rgt_df.schema.simpleString()
 
     if lft_schema != rgt_schema:
         raise exception.SchemaMismatchError(lft_schema, rgt_schema)
 
 
-def is_dataframe_equal(lft_df, rgt_df):
+def is_dataframe_equal(lft_df, rgt_df, /):
     """Evaluate if the left and right data frames are equal.
 
     Function performs:
         - A schema check
         - A row count check
         - A row content check
 
@@ -318,15 +318,15 @@
         check_row_count_equal(lft_df, rgt_df)
         check_row_equal(lft_df, rgt_df)
         return True
     except exception.SparkitError:
         return False
 
 
-def is_row_count_equal(lft_df, rgt_df):
+def is_row_count_equal(lft_df, rgt_df, /):
     """Evaluate if the row counts of the left and right data frames are equal.
 
     Parameters
     ----------
     lft_df : pyspark.sql.DataFrame
         Left data frame.
     rgt_df : pyspark.sql.DataFrame
@@ -359,15 +359,15 @@
     try:
         check_row_count_equal(lft_df, rgt_df)
         return True
     except exception.RowCountMismatchError:
         return False
 
 
-def is_row_equal(lft_df, rgt_df):
+def is_row_equal(lft_df, rgt_df, /):
     """Evaluate if the rows of the left and right data frames are equal.
 
     Parameters
     ----------
     lft_df : pyspark.sql.DataFrame
         Left data frame.
     rgt_df : pyspark.sql.DataFrame
@@ -400,15 +400,15 @@
     try:
         check_row_equal(lft_df, rgt_df)
         return True
     except exception.RowMismatchError:
         return False
 
 
-def is_schema_equal(lft_df, rgt_df):
+def is_schema_equal(lft_df, rgt_df, /):
     """Evaluate if the schemas of the left and right data frames are equal.
 
     Parameters
     ----------
     lft_df : pyspark.sql.DataFrame
         Left data frame.
     rgt_df : pyspark.sql.DataFrame
```

### Comparing `sparkit-0.3.0/setup.py` & `sparkit-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ['bumbag>=4.0.1,<5.0.0',
  'pandas>=1.5.3,<2.0.0',
  'pyarrow>=11.0.0,<12.0.0',
  'pyspark>=3,<4']
 
 setup_kwargs = {
     'name': 'sparkit',
-    'version': '0.3.0',
+    'version': '1.0.0',
     'description': 'A package for PySpark utility functions.',
     'long_description': '<p align="center">\n<img src="https://raw.githubusercontent.com/estripling/sparkit/main/docs/source/_static/logo.png" width="480" alt="The sparkit logo.">\n</p>\n\n<p align="center">\n<a href="https://pypi.org/project/sparkit"><img alt="pypi" src="https://img.shields.io/pypi/v/sparkit"></a>\n<a href="https://readthedocs.org/projects/sparkit/?badge=latest"><img alt="docs" src="https://readthedocs.org/projects/sparkit/badge/?version=latest"></a>\n<a href="https://github.com/estripling/sparkit/actions/workflows/ci.yml"><img alt="ci status" src="https://github.com/estripling/sparkit/actions/workflows/ci.yml/badge.svg?branch=main"></a>\n<a href="https://codecov.io/gh/estripling/sparkit"><img alt="coverage" src="https://codecov.io/github/estripling/sparkit/coverage.svg?branch=main"></a>\n<a href="https://github.com/estripling/sparkit/blob/main/LICENSE"><img alt="license" src="https://img.shields.io/pypi/l/sparkit"></a>\n</p>\n\n## About\n\nA package for PySpark utility functions:\n\n- [Documentation](https://sparkit.readthedocs.io/en/stable/index.html)\n- [Example usage](https://sparkit.readthedocs.io/en/stable/example.html)\n- [API Reference](https://sparkit.readthedocs.io/en/stable/autoapi/sparkit/index.html)\n\n## Installation\n\n`sparkit` is available on [PyPI](https://pypi.org/project/sparkit/) for Python 3.8+ and Spark 3 (Java 11):\n\n```console\npip install sparkit\n```\n\n## Examples\n\n[`join`](https://sparkit.readthedocs.io/en/stable/autoapi/sparkit/index.html#sparkit.join) multiple data frames on common key (pass single and / or an iterable of data frames):\n\n```python\n>>> import sparkit\n>>> from pyspark.sql import Row, SparkSession\n>>> spark = SparkSession.builder.getOrCreate()\n>>> df1 = spark.createDataFrame([Row(id=1, x="a"), Row(id=2, x="b")])\n>>> df2 = spark.createDataFrame([Row(id=1, y="c"), Row(id=2, y="d")])\n>>> df3 = spark.createDataFrame([Row(id=1, z="e"), Row(id=2, z="f")])\n>>> sparkit.join([df1, df2], df3, on="id").show()\n+---+---+---+---+\n| id|  x|  y|  z|\n+---+---+---+---+\n|  1|  a|  c|  e|\n|  2|  b|  d|  f|\n+---+---+---+---+\n```\n\n[`union`](https://sparkit.readthedocs.io/en/stable/autoapi/sparkit/index.html#sparkit.union) multiple data frames by name (pass single and / or an iterable of data frames):\n\n```python\n>>> import sparkit\n>>> from pyspark.sql import Row, SparkSession\n>>> spark = SparkSession.builder.getOrCreate()\n>>> df1 = spark.createDataFrame([Row(x=1, y=2), Row(x=3, y=4)])\n>>> df2 = spark.createDataFrame([Row(x=5, y=6), Row(x=7, y=8)])\n>>> df3 = spark.createDataFrame([Row(x=0, y=1), Row(x=2, y=3)])\n>>> df4 = spark.createDataFrame([Row(x=5, y=3), Row(x=9, y=6)])\n>>> sparkit.union(df1, [df2, df3], df4).show()\n+---+---+\n|  x|  y|\n+---+---+\n|  1|  2|\n|  3|  4|\n|  5|  6|\n|  7|  8|\n|  0|  1|\n|  2|  3|\n|  5|  3|\n|  9|  6|\n+---+---+\n```\n\n## Contributing to sparkit\n\nYour contribution is greatly appreciated!\nSee the following links to help you get started:\n\n- [Contributing Guide](https://sparkit.readthedocs.io/en/latest/contributing.html)\n- [Developer Guide](https://sparkit.readthedocs.io/en/latest/developers.html)\n- [Contributor Code of Conduct](https://sparkit.readthedocs.io/en/latest/conduct.html)\n\n## License\n\n`sparkit` was created by sparkit Developers.\nIt is licensed under the terms of the BSD 3-Clause license.\n',
     'author': 'sparkit Developers',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/estripling/sparkit',
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['sparkit'] package_data = \ {'': ['*']} install_requires =
 \ ['bumbag>=4.0.1,<5.0.0', 'pandas>=1.5.3,<2.0.0', 'pyarrow>=11.0.0,<12.0.0',
-'pyspark>=3,<4'] setup_kwargs = { 'name': 'sparkit', 'version': '0.3.0',
+'pyspark>=3,<4'] setup_kwargs = { 'name': 'sparkit', 'version': '1.0.0',
 'description': 'A package for PySpark utility functions.', 'long_description':
 '
                             \n[The sparkit logo.]\n
 \n\n
             \n[pypi]\n[docs]\n[ci_status]\n[coverage]\n[license]\n
 \n\n## About\n\nA package for PySpark utility functions:\n\n- [Documentation]
 (https://sparkit.readthedocs.io/en/stable/index.html)\n- [Example usage](https:
```

### Comparing `sparkit-0.3.0/PKG-INFO` & `sparkit-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparkit
-Version: 0.3.0
+Version: 1.0.0
 Summary: A package for PySpark utility functions.
 Home-page: https://github.com/estripling/sparkit
 License: BSD 3-Clause
 Keywords: sparkit
 Author: sparkit Developers
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sparkit Version: 0.3.0 Summary: A package for
+Metadata-Version: 2.1 Name: sparkit Version: 1.0.0 Summary: A package for
 PySpark utility functions. Home-page: https://github.com/estripling/sparkit
 License: BSD 3-Clause Keywords: sparkit Author: sparkit Developers Requires-
 Python: >=3.8,<4.0 Classifier: License :: Other/Proprietary License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3 Requires-Dist:
```

