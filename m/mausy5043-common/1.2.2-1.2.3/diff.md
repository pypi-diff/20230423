# Comparing `tmp/mausy5043_common-1.2.2.tar.gz` & `tmp/mausy5043_common-1.2.3.tar.gz`

## Comparing `mausy5043_common-1.2.2.tar` & `mausy5043_common-1.2.3.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 mausy5043_common-1.2.2/.editorconfig
--rw-r--r--   0        0        0    20752 2020-02-02 00:00:00.000000 mausy5043_common-1.2.2/.pylintrc
--rwxr-xr-x   0        0        0     2227 2020-02-02 00:00:00.000000 mausy5043_common-1.2.2/build
--rwxr-xr-x   0        0        0      817 2020-02-02 00:00:00.000000 mausy5043_common-1.2.2/check
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 mausy5043_common-1.2.2/requirements.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 mausy5043_common-1.2.2/tox.ini
--rwxr-xr-x   0        0        0       68 2020-02-02 00:00:00.000000 mausy5043_common-1.2.2/src/mausy5043_common/__init__.py
--rwxr-xr-x   0        0        0      951 2020-02-02 00:00:00.000000 mausy5043_common-1.2.2/src/mausy5043_common/funfile.py
--rwxr-xr-x   0        0        0     1396 2020-02-02 00:00:00.000000 mausy5043_common-1.2.2/src/mausy5043_common/funmeteo.py
--rwxr-xr-x   0        0        0      641 2020-02-02 00:00:00.000000 mausy5043_common-1.2.2/src/mausy5043_common/libsignals.py
--rwxr-xr-x   0        0        0     8037 2020-02-02 00:00:00.000000 mausy5043_common-1.2.2/src/mausy5043_common/libsqlite3.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mausy5043_common-1.2.2/tests/.placeholder
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 mausy5043_common-1.2.2/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 mausy5043_common-1.2.2/LICENSE
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 mausy5043_common-1.2.2/README.md
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 mausy5043_common-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 mausy5043_common-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 mausy5043_common-1.2.3/.editorconfig
+-rw-r--r--   0        0        0    20752 2020-02-02 00:00:00.000000 mausy5043_common-1.2.3/.pylintrc
+-rwxr-xr-x   0        0        0     2227 2020-02-02 00:00:00.000000 mausy5043_common-1.2.3/build
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 mausy5043_common-1.2.3/requirements.txt
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 mausy5043_common-1.2.3/tox.ini
+-rwxr-xr-x   0        0        0       68 2020-02-02 00:00:00.000000 mausy5043_common-1.2.3/src/mausy5043_common/__init__.py
+-rwxr-xr-x   0        0        0      951 2020-02-02 00:00:00.000000 mausy5043_common-1.2.3/src/mausy5043_common/funfile.py
+-rwxr-xr-x   0        0        0     1396 2020-02-02 00:00:00.000000 mausy5043_common-1.2.3/src/mausy5043_common/funmeteo.py
+-rwxr-xr-x   0        0        0      641 2020-02-02 00:00:00.000000 mausy5043_common-1.2.3/src/mausy5043_common/libsignals.py
+-rwxr-xr-x   0        0        0     8049 2020-02-02 00:00:00.000000 mausy5043_common-1.2.3/src/mausy5043_common/libsqlite3.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mausy5043_common-1.2.3/tests/.placeholder
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 mausy5043_common-1.2.3/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 mausy5043_common-1.2.3/LICENSE
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 mausy5043_common-1.2.3/README.md
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 mausy5043_common-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 mausy5043_common-1.2.3/PKG-INFO
```

### Comparing `mausy5043_common-1.2.2/.pylintrc` & `mausy5043_common-1.2.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `mausy5043_common-1.2.2/build` & `mausy5043_common-1.2.3/build`

 * *Files identical despite different names*

### Comparing `mausy5043_common-1.2.2/src/mausy5043_common/funfile.py` & `mausy5043_common-1.2.3/src/mausy5043_common/funfile.py`

 * *Files identical despite different names*

### Comparing `mausy5043_common-1.2.2/src/mausy5043_common/funmeteo.py` & `mausy5043_common-1.2.3/src/mausy5043_common/funmeteo.py`

 * *Files identical despite different names*

### Comparing `mausy5043_common-1.2.2/src/mausy5043_common/libsignals.py` & `mausy5043_common-1.2.3/src/mausy5043_common/libsignals.py`

 * *Files identical despite different names*

### Comparing `mausy5043_common-1.2.2/src/mausy5043_common/libsqlite3.py` & `mausy5043_common-1.2.3/src/mausy5043_common/libsqlite3.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 class SqlDatabase:
     """A class to interact with SQLite3 databases."""
 
     def __init__(
         self,
-        database=".local/databasefile",
+        database=".local/databasefile.sqlite3",
         schema=None,
         table=None,
         insert=None,
         debug=False,
     ):
         self.debug = debug
         self.home = os.environ["HOME"]
@@ -94,16 +94,18 @@
             mf.syslog_trace("Data must be a dictionary!", syslog.LOG_CRIT, self.debug)
             raise TypeError
 
     def insert(self, method="ignore", index="sample_time"):
         """Commit queued data to the database.
 
         Args:
-            method (str):   how to handle duplicates in the database. Possible options are 'ignore' (database will not
-                            be changed) or 'replace' (existing data will be removed and new data inserted).
+            method (str):   how to handle duplicates in the database.
+                            Possible options are 'ignore' (database will not
+                            be changed) or 'replace' (existing data will be removed
+                            and new data inserted).
             index (str):    name of the field to be used as the index.
 
         Returns:
             None
 
         Raises:
             sqlite3.Error : when commit fails serverside
@@ -137,35 +139,33 @@
                 # this can be passed
                 if method == "ignore":
                     mf.syslog_trace(
                         "Duplicate entry. Not adding to database.", False, self.debug
                     )
                 if method == "replace":
                     element_time = element[f"{df_idx}"]
-                    sql_command = f'DELETE FROM {self.table} WHERE sample_time = "{element_time}";'
+                    sql_command = (
+                        f'DELETE FROM {self.table} WHERE sample_time = "{element_time}";'
+                    )
                     # mf.syslog_trace(f"{sql_command}", False, self.debug)
                     cursor = consql.cursor()
                     try:
                         cursor.execute(sql_command)
                         cursor.fetchone()
                         cursor.close()
                         consql.commit()
                     except s3.Error:
                         mf.syslog_trace(
                             "SQLite3 error when commiting to server.",
                             syslog.LOG_ERR,
                             self.debug,
                         )
-                        mf.syslog_trace(
-                            traceback.format_exc(), syslog.LOG_ERR, self.debug
-                        )
+                        mf.syslog_trace(traceback.format_exc(), syslog.LOG_ERR, self.debug)
                         raise
-                    df.to_sql(
-                        name=self.table, con=consql, if_exists="append", index=False
-                    )
+                    df.to_sql(name=self.table, con=consql, if_exists="append", index=False)
                     mf.syslog_trace(f"Replaced : \n{df}", False, self.debug)
             except s3.Error:
                 mf.syslog_trace(
                     "SQLite3 error when commiting to server.",
                     syslog.LOG_ERR,
                     self.debug,
                 )
```

### Comparing `mausy5043_common-1.2.2/.gitignore` & `mausy5043_common-1.2.3/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Created by https://www.gitignore.io/api/python,pycharm
 # Edit at https://www.gitignore.io/?templates=python,pycharm
 
 ### local linting
 FIXME
 FIXME-2
+FIXME-SECURITY
 
 ### PyCharm ###
 .idea/
 
 ### Visual Studio ###
 .vscode/
```

### Comparing `mausy5043_common-1.2.2/LICENSE` & `mausy5043_common-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mausy5043_common-1.2.2/README.md` & `mausy5043_common-1.2.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 
 ## NOTE:
 ### user action required !!
 Before trying to use the SQLITE3 functions in this package make sure you have installed the sqlite3 server/client and 
 the default Python package that comes with it.
 
 ## Available commands for package building
-`./build --build` builds the distribution files   
-`./build --dist` uploads the distribution files to PyPi   
-`./build --test` uploads the dictribution files to TestPyPi   
-`./build --update` **discards all changes to the local copy** of the repo and pulls the current state of the repo from GitHub.
+`./build --build|-b` builds the distribution files   
+`./build --dist|-d` uploads the distribution files to PyPi   
+`./build --test|-t` uploads the dictribution files to TestPyPi   
+`./build --discard` **discards all changes to the local copy** of the repo and pulls the current state of the repo from GitHub.
 
 ## Functions provided
 `cat(filename)` : Read a file into a variable.   
 `syslog_trace(trace, logerr, out2console)` : Log messages to console and/or system log.   
 `moisture(temperature, relative_humidity, pressure)` : Calculate the moisture content of air given T [degC], RH [%] and P [hPa].   
 `wet_bulb_temperature(temperature, relative_humidity)` : Calculate the wet bulb temperature of the air given T [degC] and RH [%].
```

### Comparing `mausy5043_common-1.2.2/pyproject.toml` & `mausy5043_common-1.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mausy5043-common"
 description = "Common python functions"
-version = "1.2.2"
+version = "1.2.3"
 dependencies = [
     "numpy",
     "pandas",
 ]
 authors = [
   { name="Mausy5043" },
 ]
```

### Comparing `mausy5043_common-1.2.2/PKG-INFO` & `mausy5043_common-1.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mausy5043-common
-Version: 1.2.2
+Version: 1.2.3
 Summary: Common python functions
 Project-URL: Homepage, https://github.com/Mausy5043/mausy5043-common
 Project-URL: Bug Tracker, https://github.com/Mausy5043/mausy5043-common/issues
 Author: Mausy5043
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
@@ -30,18 +30,18 @@
 
 ## NOTE:
 ### user action required !!
 Before trying to use the SQLITE3 functions in this package make sure you have installed the sqlite3 server/client and 
 the default Python package that comes with it.
 
 ## Available commands for package building
-`./build --build` builds the distribution files   
-`./build --dist` uploads the distribution files to PyPi   
-`./build --test` uploads the dictribution files to TestPyPi   
-`./build --update` **discards all changes to the local copy** of the repo and pulls the current state of the repo from GitHub.
+`./build --build|-b` builds the distribution files   
+`./build --dist|-d` uploads the distribution files to PyPi   
+`./build --test|-t` uploads the dictribution files to TestPyPi   
+`./build --discard` **discards all changes to the local copy** of the repo and pulls the current state of the repo from GitHub.
 
 ## Functions provided
 `cat(filename)` : Read a file into a variable.   
 `syslog_trace(trace, logerr, out2console)` : Log messages to console and/or system log.   
 `moisture(temperature, relative_humidity, pressure)` : Calculate the moisture content of air given T [degC], RH [%] and P [hPa].   
 `wet_bulb_temperature(temperature, relative_humidity)` : Calculate the wet bulb temperature of the air given T [degC] and RH [%].
```

