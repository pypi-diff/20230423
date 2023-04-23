# Comparing `tmp/pysparkplus-0.0.2.tar.gz` & `tmp/pysparkplus-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysparkplus-0.0.2.tar", max compression
+gzip compressed data, was "pysparkplus-0.0.3.tar", max compression
```

## Comparing `pysparkplus-0.0.2.tar` & `pysparkplus-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1069 2023-04-22 10:34:16.168105 pysparkplus-0.0.2/LICENSE
--rw-r--r--   0        0        0     2485 2023-04-22 13:12:53.607243 pysparkplus-0.0.2/README.md
--rw-r--r--   0        0        0     1044 2023-04-22 13:13:32.717240 pysparkplus-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-22 10:34:16.188105 pysparkplus-0.0.2/pysparkplus/__init__.py
--rw-r--r--   0        0        0     3554 2023-04-22 13:08:34.067266 pysparkplus-0.0.2/pysparkplus/functions.py
--rw-r--r--   0        0        0     3228 1970-01-01 00:00:00.000000 pysparkplus-0.0.2/setup.py
--rw-r--r--   0        0        0     3133 1970-01-01 00:00:00.000000 pysparkplus-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-22 10:34:16.168105 pysparkplus-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2485 2023-04-22 13:12:53.607243 pysparkplus-0.0.3/README.md
+-rw-r--r--   0        0        0     1044 2023-04-23 16:31:28.147487 pysparkplus-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      141 2023-04-23 16:31:28.147487 pysparkplus-0.0.3/pysparkplus/__init__.py
+-rw-r--r--   0        0        0     3795 2023-04-23 16:41:05.717441 pysparkplus-0.0.3/pysparkplus/functions.py
+-rw-r--r--   0        0        0     3228 1970-01-01 00:00:00.000000 pysparkplus-0.0.3/setup.py
+-rw-r--r--   0        0        0     3133 1970-01-01 00:00:00.000000 pysparkplus-0.0.3/PKG-INFO
```

### Comparing `pysparkplus-0.0.2/LICENSE` & `pysparkplus-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pysparkplus-0.0.2/README.md` & `pysparkplus-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pysparkplus-0.0.2/pyproject.toml` & `pysparkplus-0.0.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysparkplus"
-version = "0.0.2"
+version = "0.0.3"
 authors = ["wiseupdata <silvio.liborio@wiseupdata.com>"]
 readme = "README.md"
 packages = [{include = "pysparkplus"}]
 
 description = "Pyspark extra functions!"
 
 classifiers = [
@@ -17,15 +17,15 @@
 "Homepage" = "https://github.com/wiseupdata/pysparkplus"
 "Bug Tracker" = "https://github.com/wiseupdata/pysparkplus/issues"
 
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pyspark = "^3.4.0"
-strplus = "^1.0.6"
+strplus = "^1.0.8"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.0"
 mkdocs = "^1.4.2"
 mkdocstrings = {extras = ["python"], version = "^0.21.2"}
 mkdocs-gen-files = "^0.4.0"
```

### Comparing `pysparkplus-0.0.2/pysparkplus/functions.py` & `pysparkplus-0.0.3/pysparkplus/functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,21 @@
-from typing import List
+from typing import List, Optional
 
 from pyspark.sql import DataFrame, Window
 from pyspark.sql.functions import desc, row_number
 from strplus import Str
 
 
-def deduplicate(df: DataFrame, by_columns, order_by=None) -> DataFrame:
+def count_cols(df: DataFrame):
+    return len(df.columns)
+
+
+def deduplicate(df: DataFrame, by_columns: Optional[List[str] or str] = None, order_by: Optional[List[str] or str] = None, desc_: bool = True) -> DataFrame:
     """
-    
+
     Returns a DataFrame with duplicate rows removed based on the given columns.
 
     Args:
         df (pyspark.sql.DataFrame): The input DataFrame.
         by_columns (Union[str, List[str]]): A column or list of columns to group by for deduplication.
         order_by (Optional[Union[str, List[str]]]): A column or list of columns to order by before deduplication. If not
             specified, the deduplication will be performed based on the `by_columns` parameter.
@@ -74,31 +78,30 @@
     Info: Important
         - This function preserves the first occurrence of each unique row and removes subsequent duplicates.
         - If there are no duplicate rows in the DataFrame, this function returns the input DataFrame unchanged.
         - The `order_by` parameter can be used to specify a custom order for the deduplication. By default, the function
           orders by the columns specified in the `by_columns` parameter.
         - The input DataFrame should not contain null values, as these may cause unexpected behavior in the deduplication.
     """
-    order_by = by_columns if order_by is None else order_by
-
-    order_by = Str(order_by) if isinstance(order_by, str) else order_by
 
-    if len(df.columns) == 1:
+    if count_cols(df) == 1:
+        # Native spark function!
         return df.distinct()
 
+    elif order_by is None or len(order_by) == 0:
+        # Native spark function!
+        df.dropDuplicates(subset=columns)
+
     else:
-        order_by = ",".join(order_by) if isinstance(order_by, list) else order_by
+        columns = Str(by_columns).split_by_sep if isinstance(by_columns, str) else by_columns
+        order_by_cols = Str(order_by) if isinstance(order_by, str) else Str(",".join(order_by))
 
         # Create a window specification to partition by key columns and order by order columns in descending order
-        window_spec = Window.partitionBy(by_columns).orderBy(desc(order_by))
+        window_spec = Window.partitionBy(by_columns).orderBy(desc(order_by_cols.sep_to_comma))
 
         # Add a new column called "row_num" to the DataFrame based on the window specification
         df_num = df.withColumn("row_num", row_number().over(window_spec))
 
         # Filter the DataFrame to keep only rows where the "row_num" column equals 1
         df_dedup = df_num.filter(df_num.row_num == 1)
 
         return df_dedup.drop("row_num")
-
-
-def count_cols(df: DataFrame):
-    return len(df.columns)
```

### Comparing `pysparkplus-0.0.2/setup.py` & `pysparkplus-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['pysparkplus']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['pyspark>=3.4.0,<4.0.0', 'strplus>=1.0.6,<2.0.0']
+['pyspark>=3.4.0,<4.0.0', 'strplus>=1.0.8,<2.0.0']
 
 setup_kwargs = {
     'name': 'pysparkplus',
-    'version': '0.0.2',
+    'version': '0.0.3',
     'description': 'Pyspark extra functions!',
     'long_description': '<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="Wise Up Data\'s Instagram" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/instagram.png" />   \n</a> \n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data\'s Discord" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/discord.png" />\n</a>\n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data | Twitter" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/twitter.png" />\n</a>\n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data\'s LinkedIN" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/linkedin.png" />\n</a>\n\n![visitors](https://visitor-badge.glitch.me/badge?page_id=wiseupdata.pysparkplus&left_color=green&right_color=black)\n![license](https://img.shields.io/github/license/wiseupdata/pysparkplus)\n[![pypi](https://img.shields.io/pypi/v/pysparkplus?color=green)](https://pypi.python.org/pypi/pysparkplus)\n[![downloads](https://pepy.tech/badge/pysparkplus/month)](https://pepy.tech/project/pysparkplus)\n[![versions](https://img.shields.io/pypi/pyversions/pysparkplus.svg)](https://github.com/wiseupdata/pysparkplus)\n\n---\n\n<a href="https://github.com/wiseupdata/wiseupdata">\n<img align="left" alt="img" src="https://raw.githubusercontent.com/wiseupdata/pysparkplus/main/assets/imgs/pyspark.png" width="300" />\n</a>\n\n<h1>\nPyspark extra functions ❤️\n</h1>\n\n<br>\n<br>\n<br>\n<br>\n<br>\n<br>\n<br>\n<br>\n\n[Documentation](https://wiseupdata.github.io/pysparkplus/index.html)  🚀\n\n<br>\n\n## Features ✨️\n\n- Wrapper Class!\n- Simple use!\n- Made with A.I. contribution 🤖 \n\n<br>\n</a>\n\n<br>\n<br>\n<br>\n\n* [Documentation and examples! ](https://wiseupdata.github.io/pysparkplus/index.html)! \n<br>\n<br>\n\n\n<br>\n\n### Development on go!\n\n\n<br>\n\n# References 🌍 🗄️\n\n1. [Pyspark+](https://wiseupdata.github.io/pysparkplus/index.html)\n1. [Wise Up Data](https://github.com/wiseupdata)\n1. [Emojis](https://github.com/wiseupdata/emojis)\n\n<br><br>\n---\n\n#### Maintainer 🤗 👨\u200d💻\n\nSivio Liborio\n\n📧 silvio.liborio@wiseupdata.com\n\n<a href="https://www.linkedin.com/in/silvio-de-melo-liborio">silvio-de-melo-liborio <img align="left" alt="LinkedIN" width="18px" src="https://raw.githubusercontent.com/wiseupdata/wsl-latest/main/assets/linkedin.svg" />\n</a>\n',
     'author': 'wiseupdata',
     'author_email': 'silvio.liborio@wiseupdata.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['pysparkplus'] package_data = \ {'': ['*']} install_requires = \
-['pyspark>=3.4.0,<4.0.0', 'strplus>=1.0.6,<2.0.0'] setup_kwargs = { 'name':
-'pysparkplus', 'version': '0.0.2', 'description': 'Pyspark extra functions!',
+['pyspark>=3.4.0,<4.0.0', 'strplus>=1.0.8,<2.0.0'] setup_kwargs = { 'name':
+'pysparkplus', 'version': '0.0.3', 'description': 'Pyspark extra functions!',
 'long_description': '\n_[Wise_Up_Data\'s_Instagram]_\n \n\n_[wise_Up_Data\'s
 Discord]\n\n\n_[wise_Up_Data_|_Twitter]\n\n\n_[wise_Up_Data\'s_LinkedIN]\n\n\n!
 [visitors](https://visitor-badge.glitch.me/
 badge?page_id=wiseupdata.pysparkplus&left_color=green&right_color=black)\n!
 [license](https://img.shields.io/github/license/wiseupdata/pysparkplus)\n[!
 [pypi](https://img.shields.io/pypi/v/pysparkplus?color=green)](https://
 pypi.python.org/pypi/pysparkplus)\n[![downloads](https://pepy.tech/badge/
```

### Comparing `pysparkplus-0.0.2/PKG-INFO` & `pysparkplus-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pysparkplus
-Version: 0.0.2
+Version: 0.0.3
 Summary: Pyspark extra functions!
 Author: wiseupdata
 Author-email: silvio.liborio@wiseupdata.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: pyspark (>=3.4.0,<4.0.0)
-Requires-Dist: strplus (>=1.0.6,<2.0.0)
+Requires-Dist: strplus (>=1.0.8,<2.0.0)
 Description-Content-Type: text/markdown
 
 <a href="https://github.com/wiseupdata/wiseupdata">
   <img align="left" alt="Wise Up Data's Instagram" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/instagram.png" />   
 </a> 
 <a href="https://github.com/wiseupdata/wiseupdata">
   <img align="left" alt="wise Up Data's Discord" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/discord.png" />
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: pysparkplus Version: 0.0.2 Summary: Pyspark extra
+Metadata-Version: 2.1 Name: pysparkplus Version: 0.0.3 Summary: Pyspark extra
 functions! Author: wiseupdata Author-email: silvio.liborio@wiseupdata.com
 Requires-Python: >=3.9,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3 Requires-Dist:
-pyspark (>=3.4.0,<4.0.0) Requires-Dist: strplus (>=1.0.6,<2.0.0) Description-
+pyspark (>=3.4.0,<4.0.0) Requires-Dist: strplus (>=1.0.8,<2.0.0) Description-
 Content-Type: text/markdown [Wise_Up_Data's_Instagram] [wise_Up_Data's_Discord]
 [wise_Up_Data_|_Twitter] [wise_Up_Data's_LinkedIN] ![visitors](https://visitor-
 badge.glitch.me/
 badge?page_id=wiseupdata.pysparkplus&left_color=green&right_color=black) !
 [license](https://img.shields.io/github/license/wiseupdata/pysparkplus) [!
 [pypi](https://img.shields.io/pypi/v/pysparkplus?color=green)](https://
 pypi.python.org/pypi/pysparkplus) [![downloads](https://pepy.tech/badge/
```

