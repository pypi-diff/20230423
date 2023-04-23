# Comparing `tmp/polario-0.2.1.tar.gz` & `tmp/polario-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polario-0.2.1.tar", max compression
+gzip compressed data, was "polario-0.2.2.tar", max compression
```

## Comparing `polario-0.2.1.tar` & `polario-0.2.2.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-03-27 15:34:29.430403 polario-0.2.1/LICENSE
--rw-r--r--   0        0        0      694 2023-03-27 15:34:29.430403 polario-0.2.1/README.md
--rw-r--r--   0        0        0      106 2023-03-27 15:34:29.430403 polario-0.2.1/polario/__init__.py
--rw-r--r--   0        0        0    11443 2023-03-27 15:34:29.430403 polario-0.2.1/polario/dataset.py
--rw-r--r--   0        0        0     1644 2023-03-27 15:34:29.430403 polario-0.2.1/polario/main.py
--rw-r--r--   0        0        0      997 2023-03-27 15:34:48.891522 polario-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1507 1970-01-01 00:00:00.000000 polario-0.2.1/setup.py
--rw-r--r--   0        0        0     1440 1970-01-01 00:00:00.000000 polario-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-23 17:52:08.816507 polario-0.2.2/LICENSE
+-rw-r--r--   0        0        0      694 2023-04-23 17:52:08.816507 polario-0.2.2/README.md
+-rw-r--r--   0        0        0      106 2023-04-23 17:52:08.816507 polario-0.2.2/polario/__init__.py
+-rw-r--r--   0        0        0    11443 2023-04-23 17:52:08.816507 polario-0.2.2/polario/dataset.py
+-rw-r--r--   0        0        0     1644 2023-04-23 17:52:08.816507 polario-0.2.2/polario/main.py
+-rw-r--r--   0        0        0        0 2023-04-23 17:52:08.816507 polario-0.2.2/polario/py.typed
+-rw-r--r--   0        0        0      997 2023-04-23 17:52:29.460622 polario-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1507 1970-01-01 00:00:00.000000 polario-0.2.2/setup.py
+-rw-r--r--   0        0        0     1440 1970-01-01 00:00:00.000000 polario-0.2.2/PKG-INFO
```

### Comparing `polario-0.2.1/LICENSE` & `polario-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `polario-0.2.1/README.md` & `polario-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `polario-0.2.1/polario/dataset.py` & `polario-0.2.2/polario/dataset.py`

 * *Files identical despite different names*

### Comparing `polario-0.2.1/polario/main.py` & `polario-0.2.2/polario/main.py`

 * *Files identical despite different names*

### Comparing `polario-0.2.1/pyproject.toml` & `polario-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "polario"
-version = "0.2.1"
+version = "0.2.2"
 description = "Polars IO"
 authors = ["Bram Neijt <bram@neijt.nl>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://bneijt.github.io/polario/"
 repository = "https://github.com/bneijt/polario"
 classifiers = [
```

### Comparing `polario-0.2.1/setup.py` & `polario-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'pyarrow>=11.0.0,<12.0.0']
 
 entry_points = \
 {'console_scripts': ['polario = polario.main:main']}
 
 setup_kwargs = {
     'name': 'polario',
-    'version': '0.2.1',
+    'version': '0.2.2',
     'description': 'Polars IO',
     'long_description': 'Polars IO utility library\n=================\n\nHelpers to make it easier to read and write Hive partitioned parquet dataset with Polars.\n\nIt is meant to be a library to deal with datasets easily, but also contains a commandline interface\nwhich allows you to inspect parquet files and datasets more easily.\n\nDataset\n=======\nExample of use of `polario.dataset.HiveDataset`\n```python\n\nfrom polario.dataset import HiveDataset\nimport polars as pl\ndf = pl.from_dicts(\n        [\n            {"p1": 1, "v": 1},\n            {"p1": 2, "v": 1},\n        ]\n    )\n\nds = HiveDataset("file:///tmp/", partition_columns=["p1"])\n\nds.write(df)\n\nfor partition_df in ds.read_partitions():\n    print(partition_df)\n\n```\n',
     'author': 'Bram Neijt',
     'author_email': 'bram@neijt.nl',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://bneijt.github.io/polario/',
```

### Comparing `polario-0.2.1/PKG-INFO` & `polario-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polario
-Version: 0.2.1
+Version: 0.2.2
 Summary: Polars IO
 Home-page: https://bneijt.github.io/polario/
 License: Apache-2.0
 Author: Bram Neijt
 Author-email: bram@neijt.nl
 Requires-Python: >=3.9,<4.0
 Classifier: Intended Audience :: Developers
```

