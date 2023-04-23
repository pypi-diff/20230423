# Comparing `tmp/excel-sql-engine-1.6.tar.gz` & `tmp/excel-sql-engine-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "excel-sql-engine-1.6.tar", last modified: Fri Apr 21 18:46:59 2023, max compression
+gzip compressed data, was "excel-sql-engine-1.6.1.tar", last modified: Sun Apr 23 17:33:33 2023, max compression
```

## Comparing `excel-sql-engine-1.6.tar` & `excel-sql-engine-1.6.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 18:46:59.830321 excel-sql-engine-1.6/
--rw-rw-rw-   0        0        0    14408 2023-03-13 18:23:44.000000 excel-sql-engine-1.6/LICENCE
--rw-rw-rw-   0        0        0     8284 2023-04-21 18:46:59.826719 excel-sql-engine-1.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-21 18:46:59.764020 excel-sql-engine-1.6/PyxlSql/
--rw-rw-rw-   0        0        0      563 2023-03-13 18:23:44.000000 excel-sql-engine-1.6/PyxlSql/__init__.py
--rw-rw-rw-   0        0        0     7211 2023-04-16 21:00:33.000000 excel-sql-engine-1.6/PyxlSql/pyxlAbstracts.py
--rw-rw-rw-   0        0        0    15468 2023-04-18 13:41:16.000000 excel-sql-engine-1.6/PyxlSql/pyxlArgs.py
--rw-rw-rw-   0        0        0    37421 2023-04-21 17:35:39.000000 excel-sql-engine-1.6/PyxlSql/pyxlEngine.py
--rw-rw-rw-   0        0        0     2934 2023-03-13 18:23:44.000000 excel-sql-engine-1.6/PyxlSql/pyxlErrors.py
--rw-rw-rw-   0        0        0    26449 2023-04-18 13:02:23.000000 excel-sql-engine-1.6/PyxlSql/pyxlGrammar.py
--rw-rw-rw-   0        0        0     9159 2023-04-21 18:05:53.000000 excel-sql-engine-1.6/PyxlSql/pyxlPivot.py
--rw-rw-rw-   0        0        0     7231 2023-03-21 21:57:15.000000 excel-sql-engine-1.6/PyxlSql/pyxlResults.py
--rw-rw-rw-   0        0        0    14165 2023-04-21 18:17:44.000000 excel-sql-engine-1.6/PyxlSql/pyxlSheets.py
--rw-rw-rw-   0        0        0    14097 2023-04-20 17:00:21.000000 excel-sql-engine-1.6/PyxlSql/pyxlSql.py
--rw-rw-rw-   0        0        0    14413 2023-03-20 16:49:03.000000 excel-sql-engine-1.6/PyxlSql/pyxlStages.py
--rw-rw-rw-   0        0        0    18944 2023-04-21 15:56:11.000000 excel-sql-engine-1.6/PyxlSql/pyxlWorkbook.py
--rw-rw-rw-   0        0        0     7585 2023-04-21 09:26:14.000000 excel-sql-engine-1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 18:46:59.814466 excel-sql-engine-1.6/excel_sql_engine.egg-info/
--rw-rw-rw-   0        0        0     8284 2023-04-21 18:46:59.000000 excel-sql-engine-1.6/excel_sql_engine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      574 2023-04-21 18:46:59.000000 excel-sql-engine-1.6/excel_sql_engine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 18:46:59.000000 excel-sql-engine-1.6/excel_sql_engine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-04-21 18:46:59.000000 excel-sql-engine-1.6/excel_sql_engine.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      196 2023-04-20 15:20:18.000000 excel-sql-engine-1.6/excel_sql_engine.egg-info/setup.cfg
--rw-rw-rw-   0        0        0        8 2023-04-21 18:46:59.000000 excel-sql-engine-1.6/excel_sql_engine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 18:46:59.830321 excel-sql-engine-1.6/setup.cfg
--rw-rw-rw-   0        0        0     1304 2023-04-21 18:38:21.000000 excel-sql-engine-1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-21 18:46:59.822717 excel-sql-engine-1.6/tests/
--rw-rw-rw-   0        0        0     7703 2023-04-17 15:39:30.000000 excel-sql-engine-1.6/tests/test_Northwind.py
--rw-rw-rw-   0        0        0     6381 2023-04-18 14:00:43.000000 excel-sql-engine-1.6/tests/test_tooling.py
+drwxrwxrwx   0        0        0        0 2023-04-23 17:33:33.469143 excel-sql-engine-1.6.1/
+-rw-rw-rw-   0        0        0    14408 2023-03-13 18:23:44.000000 excel-sql-engine-1.6.1/LICENCE
+-rw-rw-rw-   0        0        0     8286 2023-04-23 17:33:33.467110 excel-sql-engine-1.6.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-23 17:33:33.398037 excel-sql-engine-1.6.1/PyxlSql/
+-rw-rw-rw-   0        0        0      563 2023-03-13 18:23:44.000000 excel-sql-engine-1.6.1/PyxlSql/__init__.py
+-rw-rw-rw-   0        0        0     7165 2023-04-22 19:48:11.000000 excel-sql-engine-1.6.1/PyxlSql/pyxlAbstracts.py
+-rw-rw-rw-   0        0        0    15468 2023-04-18 13:41:16.000000 excel-sql-engine-1.6.1/PyxlSql/pyxlArgs.py
+-rw-rw-rw-   0        0        0    37421 2023-04-21 17:35:39.000000 excel-sql-engine-1.6.1/PyxlSql/pyxlEngine.py
+-rw-rw-rw-   0        0        0     2934 2023-03-13 18:23:44.000000 excel-sql-engine-1.6.1/PyxlSql/pyxlErrors.py
+-rw-rw-rw-   0        0        0    26449 2023-04-18 13:02:23.000000 excel-sql-engine-1.6.1/PyxlSql/pyxlGrammar.py
+-rw-rw-rw-   0        0        0     9159 2023-04-21 18:05:53.000000 excel-sql-engine-1.6.1/PyxlSql/pyxlPivot.py
+-rw-rw-rw-   0        0        0     7231 2023-03-21 21:57:15.000000 excel-sql-engine-1.6.1/PyxlSql/pyxlResults.py
+-rw-rw-rw-   0        0        0    14165 2023-04-21 18:17:44.000000 excel-sql-engine-1.6.1/PyxlSql/pyxlSheets.py
+-rw-rw-rw-   0        0        0    14107 2023-04-22 19:48:11.000000 excel-sql-engine-1.6.1/PyxlSql/pyxlSql.py
+-rw-rw-rw-   0        0        0    14413 2023-03-20 16:49:03.000000 excel-sql-engine-1.6.1/PyxlSql/pyxlStages.py
+-rw-rw-rw-   0        0        0    18944 2023-04-21 15:56:11.000000 excel-sql-engine-1.6.1/PyxlSql/pyxlWorkbook.py
+-rw-rw-rw-   0        0        0     7585 2023-04-21 09:26:14.000000 excel-sql-engine-1.6.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 17:33:33.451088 excel-sql-engine-1.6.1/excel_sql_engine.egg-info/
+-rw-rw-rw-   0        0        0     8286 2023-04-23 17:33:33.000000 excel-sql-engine-1.6.1/excel_sql_engine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      574 2023-04-23 17:33:33.000000 excel-sql-engine-1.6.1/excel_sql_engine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 17:33:33.000000 excel-sql-engine-1.6.1/excel_sql_engine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-04-23 17:33:33.000000 excel-sql-engine-1.6.1/excel_sql_engine.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      196 2023-04-20 15:20:18.000000 excel-sql-engine-1.6.1/excel_sql_engine.egg-info/setup.cfg
+-rw-rw-rw-   0        0        0        8 2023-04-23 17:33:33.000000 excel-sql-engine-1.6.1/excel_sql_engine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 17:33:33.470154 excel-sql-engine-1.6.1/setup.cfg
+-rw-rw-rw-   0        0        0     1306 2023-04-23 17:27:56.000000 excel-sql-engine-1.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 17:33:33.461088 excel-sql-engine-1.6.1/tests/
+-rw-rw-rw-   0        0        0     7703 2023-04-17 15:39:30.000000 excel-sql-engine-1.6.1/tests/test_Northwind.py
+-rw-rw-rw-   0        0        0     6381 2023-04-18 14:00:43.000000 excel-sql-engine-1.6.1/tests/test_tooling.py
```

### Comparing `excel-sql-engine-1.6/LICENCE` & `excel-sql-engine-1.6.1/LICENCE`

 * *Files identical despite different names*

### Comparing `excel-sql-engine-1.6/PKG-INFO` & `excel-sql-engine-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: excel-sql-engine
-Version: 1.6
+Version: 1.6.1
 Summary: A tiny SQL engine for Excel files, based on Openpyxl
 Home-page: https://gitlab.com/fabien.battini/pyxlsql
 Author: Fabien BATTINI
 Author-email: fabien.battini@gmail.com
 Keywords: excel sql
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
```

### Comparing `excel-sql-engine-1.6/PyxlSql/__init__.py` & `excel-sql-engine-1.6.1/PyxlSql/__init__.py`

 * *Files identical despite different names*

### Comparing `excel-sql-engine-1.6/PyxlSql/pyxlAbstracts.py` & `excel-sql-engine-1.6.1/PyxlSql/pyxlAbstracts.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,20 +105,20 @@
 
 class Arg(AbstractStatement):
     name = "Generic ARG"
     """A Statement that describes an actual argument"""
 
     def __init__(self, command, specification: str):
         """
-        :param command: Cmd : self is an argument to a clause inside this command
+        :param command: Cmd : is an argument to a clause inside this command
         :param specification: str : the initial specification of the argument as found in the Excel file (or similar)
         """
         super().__init__()
         self.command = command
-        self.dst_sheet_arg: Optional[PyxlSheet]  # TODO: Remove this, which is confusing
+        self.dst_sheet_arg: Optional[PyxlSheet]
         if command is None:  # MUST use this syntax to have correct type inference
             self.dst_sheet_arg = None
         else:
             self.dst_sheet_arg = command.dst_sheet_arg
 
         self.specification = specification
```

### Comparing `excel-sql-engine-1.6/PyxlSql/pyxlArgs.py` & `excel-sql-engine-1.6.1/PyxlSql/pyxlArgs.py`

 * *Files identical despite different names*

### Comparing `excel-sql-engine-1.6/PyxlSql/pyxlEngine.py` & `excel-sql-engine-1.6.1/PyxlSql/pyxlEngine.py`

 * *Files identical despite different names*

### Comparing `excel-sql-engine-1.6/PyxlSql/pyxlErrors.py` & `excel-sql-engine-1.6.1/PyxlSql/pyxlErrors.py`

 * *Files identical despite different names*

### Comparing `excel-sql-engine-1.6/PyxlSql/pyxlGrammar.py` & `excel-sql-engine-1.6.1/PyxlSql/pyxlGrammar.py`

 * *Files identical despite different names*

### Comparing `excel-sql-engine-1.6/PyxlSql/pyxlPivot.py` & `excel-sql-engine-1.6.1/PyxlSql/pyxlPivot.py`

 * *Files identical despite different names*

### Comparing `excel-sql-engine-1.6/PyxlSql/pyxlResults.py` & `excel-sql-engine-1.6.1/PyxlSql/pyxlResults.py`

 * *Files identical despite different names*

### Comparing `excel-sql-engine-1.6/PyxlSql/pyxlSheets.py` & `excel-sql-engine-1.6.1/PyxlSql/pyxlSheets.py`

 * *Files identical despite different names*

### Comparing `excel-sql-engine-1.6/PyxlSql/pyxlSql.py` & `excel-sql-engine-1.6.1/PyxlSql/pyxlSql.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,16 +41,16 @@
 # REQ 0008: Generate to do.rst through tox, using parse_requirements.py
 # REQ 0009: publish also htmlcov on gitlab.io
 # REQ 0010: create a downloadable executable for windows user : python -m pip install PyInstaller #
 # TODO: REQ 0011: create a doc specific to windows user that do not know python
 # REQ 0012: manage also .ods files from LibreOffice: NO, this is NOT possible, OpenPyxl does NOT read .ods format
 # REQ 0013: LAZY reading of sheets: only sheets that are referred by the SQL commands are read.
 
-# TODO: 100% coverage: most of not covered lines are defensive code which is unreachable by design
-# TODO: Update current documentation xxx.rst because @ is often replaced by # in examples, due to more strict typing
+# TODO: REQ 0014: 100% coverage: most of not covered lines are defensive code which is unreachable by design
+# DONE: Update current documentation xxx.rst because @ is often replaced by # in examples, due to more strict typing
 
 
 # ----------------------- Cmdline arguments
 # REQ 1001: --dir/-d directory: processes all Excel files in the directory
 # REQ 1002: --file/-f file (multiple times): process this file
 # REQ 1003: --filepath/-p dir (multiple times): adds directory to path for included Excel files
 # REQ 1004: the directory of the file being processed is added in the filepath
```

### Comparing `excel-sql-engine-1.6/PyxlSql/pyxlStages.py` & `excel-sql-engine-1.6.1/PyxlSql/pyxlStages.py`

 * *Files identical despite different names*

### Comparing `excel-sql-engine-1.6/PyxlSql/pyxlWorkbook.py` & `excel-sql-engine-1.6.1/PyxlSql/pyxlWorkbook.py`

 * *Files identical despite different names*

### Comparing `excel-sql-engine-1.6/README.md` & `excel-sql-engine-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `excel-sql-engine-1.6/excel_sql_engine.egg-info/PKG-INFO` & `excel-sql-engine-1.6.1/excel_sql_engine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: excel-sql-engine
-Version: 1.6
+Version: 1.6.1
 Summary: A tiny SQL engine for Excel files, based on Openpyxl
 Home-page: https://gitlab.com/fabien.battini/pyxlsql
 Author: Fabien BATTINI
 Author-email: fabien.battini@gmail.com
 Keywords: excel sql
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
```

### Comparing `excel-sql-engine-1.6/excel_sql_engine.egg-info/SOURCES.txt` & `excel-sql-engine-1.6.1/excel_sql_engine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `excel-sql-engine-1.6/setup.py` & `excel-sql-engine-1.6.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # CAVEAT : This file is edited by tests/patch_files.py to setup the version name from the latest tag
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 # see https://setuptools.pypa.io/en/latest/references/keywords.html
 setuptools.setup(
     name="excel-sql-engine",
-    version="1.6",
+    version="1.6.1",
     author="Fabien BATTINI",
     author_email="fabien.battini@gmail.com",
     description="A tiny SQL engine for Excel files, based on Openpyxl",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/fabien.battini/pyxlsql",
     license_files=["LICENCE"],
```

### Comparing `excel-sql-engine-1.6/tests/test_Northwind.py` & `excel-sql-engine-1.6.1/tests/test_Northwind.py`

 * *Files identical despite different names*

### Comparing `excel-sql-engine-1.6/tests/test_tooling.py` & `excel-sql-engine-1.6.1/tests/test_tooling.py`

 * *Files identical despite different names*

