# Comparing `tmp/mausy5043_common-1.2.3.tar.gz` & `tmp/mausy5043_common-1.4.1.tar.gz`

## Comparing `mausy5043_common-1.2.3.tar` & `mausy5043_common-1.4.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 mausy5043_common-1.2.3/.editorconfig
--rw-r--r--   0        0        0    20752 2020-02-02 00:00:00.000000 mausy5043_common-1.2.3/.pylintrc
--rwxr-xr-x   0        0        0     2227 2020-02-02 00:00:00.000000 mausy5043_common-1.2.3/build
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 mausy5043_common-1.2.3/requirements.txt
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 mausy5043_common-1.2.3/tox.ini
--rwxr-xr-x   0        0        0       68 2020-02-02 00:00:00.000000 mausy5043_common-1.2.3/src/mausy5043_common/__init__.py
--rwxr-xr-x   0        0        0      951 2020-02-02 00:00:00.000000 mausy5043_common-1.2.3/src/mausy5043_common/funfile.py
--rwxr-xr-x   0        0        0     1396 2020-02-02 00:00:00.000000 mausy5043_common-1.2.3/src/mausy5043_common/funmeteo.py
--rwxr-xr-x   0        0        0      641 2020-02-02 00:00:00.000000 mausy5043_common-1.2.3/src/mausy5043_common/libsignals.py
--rwxr-xr-x   0        0        0     8049 2020-02-02 00:00:00.000000 mausy5043_common-1.2.3/src/mausy5043_common/libsqlite3.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mausy5043_common-1.2.3/tests/.placeholder
--rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 mausy5043_common-1.2.3/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 mausy5043_common-1.2.3/LICENSE
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 mausy5043_common-1.2.3/README.md
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 mausy5043_common-1.2.3/pyproject.toml
--rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 mausy5043_common-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 mausy5043_common-1.4.1/.editorconfig
+-rw-r--r--   0        0        0    20752 2020-02-02 00:00:00.000000 mausy5043_common-1.4.1/.pylintrc
+-rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 mausy5043_common-1.4.1/BUILDING.md
+-rwxr-xr-x   0        0        0     2227 2020-02-02 00:00:00.000000 mausy5043_common-1.4.1/build
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 mausy5043_common-1.4.1/requirements.txt
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 mausy5043_common-1.4.1/tox.ini
+-rwxr-xr-x   0        0        0       68 2020-02-02 00:00:00.000000 mausy5043_common-1.4.1/src/mausy5043_common/__init__.py
+-rwxr-xr-x   0        0        0      951 2020-02-02 00:00:00.000000 mausy5043_common-1.4.1/src/mausy5043_common/funfile.py
+-rwxr-xr-x   0        0        0     1396 2020-02-02 00:00:00.000000 mausy5043_common-1.4.1/src/mausy5043_common/funmeteo.py
+-rwxr-xr-x   0        0        0      641 2020-02-02 00:00:00.000000 mausy5043_common-1.4.1/src/mausy5043_common/libsignals.py
+-rwxr-xr-x   0        0        0     8699 2020-02-02 00:00:00.000000 mausy5043_common-1.4.1/src/mausy5043_common/libsqlite3.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mausy5043_common-1.4.1/tests/.placeholder
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 mausy5043_common-1.4.1/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 mausy5043_common-1.4.1/LICENSE
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 mausy5043_common-1.4.1/README.md
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 mausy5043_common-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 mausy5043_common-1.4.1/PKG-INFO
```

### Comparing `mausy5043_common-1.2.3/.pylintrc` & `mausy5043_common-1.4.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `mausy5043_common-1.2.3/build` & `mausy5043_common-1.4.1/build`

 * *Files identical despite different names*

### Comparing `mausy5043_common-1.2.3/tox.ini` & `mausy5043_common-1.4.1/tox.ini`

 * *Files 24% similar despite different names*

```diff
@@ -18,13 +18,13 @@
 builtins = _
 
 [pylama:pydocstyle]
 convention = google
 
 [pylama:pycodestyle]
 max_line_length = 98
-ignore=E203,E402,W503
+ignore=E203,E402,E501,W503
 
 [pylama:pylint]
 max_line_length = 98
 rcfile = .pylintrc
 disable = C0103,C0114,C0116,E1136,R0913,R0914,R0915,W1203
```

### Comparing `mausy5043_common-1.2.3/src/mausy5043_common/funfile.py` & `mausy5043_common-1.4.1/src/mausy5043_common/funfile.py`

 * *Files identical despite different names*

### Comparing `mausy5043_common-1.2.3/src/mausy5043_common/funmeteo.py` & `mausy5043_common-1.4.1/src/mausy5043_common/funmeteo.py`

 * *Files identical despite different names*

### Comparing `mausy5043_common-1.2.3/src/mausy5043_common/libsignals.py` & `mausy5043_common-1.4.1/src/mausy5043_common/libsignals.py`

 * *Files identical despite different names*

### Comparing `mausy5043_common-1.2.3/src/mausy5043_common/libsqlite3.py` & `mausy5043_common-1.4.1/src/mausy5043_common/libsqlite3.py`

 * *Files 16% similar despite different names*

```diff
@@ -40,17 +40,18 @@
 
         Returns:
             None
         """
         consql = None
         try:
             consql = s3.connect(self.database, timeout=9000)
-        except s3.Error:
+        except s3.Error as her:
             mf.syslog_trace(
-                "Unexpected SQLite3 error when connecting to server.",
+                # pylint: disable-next=C0301
+                f"Unexpected SQLite3 error of type {type(her).__name__} when connecting to server.",
                 syslog.LOG_CRIT,
                 self.debug,
             )
             mf.syslog_trace(traceback.format_exc(), syslog.LOG_CRIT, self.debug)
             if consql:  # attempt to close connection to sqlite3 server
                 consql.close()
                 mf.syslog_trace(" ** Closed SQLite3 connection. **", False, self.debug)
@@ -66,17 +67,19 @@
                 f"Attached to SQLite3 server: {versql}", syslog.LOG_INFO, self.debug
             )
             mf.syslog_trace(
                 f"Using DB file             : {self.database}",
                 syslog.LOG_INFO,
                 self.debug,
             )
-        except s3.Error:
+        except s3.Error as her:
             mf.syslog_trace(
-                "Unexpected SQLite3 error during test.", syslog.LOG_CRIT, self.debug
+                f"Unexpected SQLite3 error of type {type(her).__name__} during test.",
+                syslog.LOG_CRIT,
+                self.debug,
             )
             mf.syslog_trace(traceback.format_exc(), syslog.LOG_CRIT, self.debug)
             raise
         return versql
 
     def queue(self, data):
         """Append data to the queue for insertion.
@@ -95,33 +98,37 @@
             raise TypeError
 
     def insert(self, method="ignore", index="sample_time"):
         """Commit queued data to the database.
 
         Args:
             method (str):   how to handle duplicates in the database.
-                            Possible options are 'ignore' (database will not
-                            be changed) or 'replace' (existing data will be removed
-                            and new data inserted).
+                            Possible options are:
+                            'ignore' (database will not be changed) or
+                            'replace' (existing data will be removed and new data inserted).
             index (str):    name of the field to be used as the index.
 
         Returns:
             None
 
         Raises:
-            sqlite3.Error : when commit fails serverside
-            Exception : to catch unknown errors during the exchange
+            ValueError: if <sql_insert> is not defined
+            sqlite3.Error: when commit fails serverside
+            Exception: to catch unknown errors during the exchange
         """
         consql = None
+        if not self.insert:
+            raise ValueError("No instruction provided")
 
         try:
             consql = s3.connect(self.database, timeout=9000)
-        except s3.Error:
+        except s3.Error as her:
             mf.syslog_trace(
-                "Unexpected SQLite3 error when connecting to server.",
+                # pylint: disable-next=C0301
+                f"Unexpected SQLite3 error of type {type(her).__name__} when connecting to server.",
                 syslog.LOG_CRIT,
                 self.debug,
             )
             mf.syslog_trace(traceback.format_exc(), syslog.LOG_CRIT, self.debug)
             if consql:  # attempt to close connection to sqlite3 server
                 consql.close()
                 mf.syslog_trace(" ** Closed SQLite3 connection. **", False, self.debug)
@@ -129,54 +136,56 @@
 
         while self.dataq:
             element = self.dataq[0]
             df_idx = index  # list(element.keys())[0]    # this should always be 'sample_time'
             df = pd.DataFrame(element, index=[df_idx])
             try:
                 df.to_sql(name=self.table, con=consql, if_exists="append", index=False)
-                mf.syslog_trace(f"Inserted : \n{df}", False, self.debug)
+                mf.syslog_trace(f"Inserted : \n{df}\n", False, self.debug)
             except s3.IntegrityError:
                 # probably "sqlite3.IntegrityError: UNIQUE constraint failed".
                 # this can be passed
                 if method == "ignore":
                     mf.syslog_trace(
                         "Duplicate entry. Not adding to database.", False, self.debug
                     )
                 if method == "replace":
                     element_time = element[f"{df_idx}"]
-                    sql_command = (
-                        f'DELETE FROM {self.table} WHERE sample_time = "{element_time}";'
-                    )
-                    # mf.syslog_trace(f"{sql_command}", False, self.debug)
+                    sql_command = f'DELETE FROM {self.table} WHERE {df_idx} = "{element_time}";'
                     cursor = consql.cursor()
                     try:
                         cursor.execute(sql_command)
                         cursor.fetchone()
                         cursor.close()
                         consql.commit()
-                    except s3.Error:
+                    except s3.Error as her:
                         mf.syslog_trace(
-                            "SQLite3 error when commiting to server.",
+                            # pylint: disable-next=C0301
+                            f"SQLite3 error of type {type(her).__name__} when commiting to server.",
                             syslog.LOG_ERR,
                             self.debug,
                         )
                         mf.syslog_trace(traceback.format_exc(), syslog.LOG_ERR, self.debug)
                         raise
                     df.to_sql(name=self.table, con=consql, if_exists="append", index=False)
-                    mf.syslog_trace(f"Replaced : \n{df}", False, self.debug)
-            except s3.Error:
+                    mf.syslog_trace(f"Replaced : \n{df}\n", False, self.debug)
+            except s3.Error as her:
                 mf.syslog_trace(
-                    "SQLite3 error when commiting to server.",
+                    f"SQLite3 error of type {type(her).__name__} when commiting to server.",
                     syslog.LOG_ERR,
                     self.debug,
                 )
                 mf.syslog_trace(traceback.format_exc(), syslog.LOG_ERR, self.debug)
                 raise
-            except Exception:
-                mf.syslog_trace("Unexpected error!", syslog.LOG_ERR, self.debug)
+            except Exception as her:
+                mf.syslog_trace(
+                    f"Unexpected error of type {type(her).__name__} !",
+                    syslog.LOG_ERR,
+                    self.debug,
+                )
                 mf.syslog_trace(traceback.format_exc(), syslog.LOG_ERR, self.debug)
                 raise
             self.dataq.pop(0)
 
         consql.close()
 
     def latest_datapoint(self):
@@ -185,17 +194,18 @@
 
         Returns:
             date and time of the youngest entry in the table
         """
         consql = None
         try:
             consql = s3.connect(self.database, timeout=9000)
-        except s3.Error:
+        except s3.Error as her:
             mf.syslog_trace(
-                "Unexpected SQLite3 error when connecting to server.",
+                # pylint: disable-next=C0301
+                f"Unexpected SQLite3 error of type {type(her).__name__} when connecting to server.",
                 syslog.LOG_CRIT,
                 self.debug,
             )
             mf.syslog_trace(traceback.format_exc(), syslog.LOG_CRIT, self.debug)
             if consql:  # attempt to close connection to sqlite3 server
                 consql.close()
                 mf.syslog_trace(" ** Closed SQLite3 connection. **", False, self.debug)
@@ -210,14 +220,16 @@
             consql.close()
             mf.syslog_trace(
                 f"Latest datapoint in {self.table}: "
                 f"{max_epoch[0]} = {time.strftime('%Y-%m-%d %H:%M:%S', human_epoch)}",
                 False,
                 self.debug,
             )
-        except s3.Error:
+        except s3.Error as her:
             mf.syslog_trace(
-                "Unexpected SQLite3 error during test.", syslog.LOG_CRIT, self.debug
+                f"Unexpected SQLite3 error of type {type(her).__name__} during test.",
+                syslog.LOG_CRIT,
+                self.debug,
             )
             mf.syslog_trace(traceback.format_exc(), syslog.LOG_CRIT, self.debug)
             raise
         return time.strftime("%Y-%m-%d %H:%M:%S", human_epoch)
```

### Comparing `mausy5043_common-1.2.3/.gitignore` & `mausy5043_common-1.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `mausy5043_common-1.2.3/LICENSE` & `mausy5043_common-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mausy5043_common-1.2.3/README.md` & `mausy5043_common-1.4.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 # mausy5043-common
 
 [![PyPI version](https://img.shields.io/pypi/v/mausy5043-common.svg?logo=pypi&logoColor=FFE873)](https://pypi.org/project/mausy5043-common)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/mausy5043-common.svg?logo=python&logoColor=FFE873)](https://pypi.org/project/mausy5043-common)
 [![PyPI downloads](https://img.shields.io/pypi/dm/mausy5043-common.svg)](https://pypistats.org/packages/mausy5043-common)
 [![Code style: Black](https://img.shields.io/badge/code%20style-Black-000000.svg)](https://github.com/psf/black)
 
-Provides various Python3 functions and classes for personal use.
+This is a Python3 library of functions and classes, mainly for personal use.
 
-## NOTE:
-### user action required !!
+## Requirements
+
+**NOTE: user action required !!**  
 Before trying to use the SQLITE3 functions in this package make sure you have installed the sqlite3 server/client and 
 the default Python package that comes with it.
 
-## Available commands for package building
-`./build --build|-b` builds the distribution files   
-`./build --dist|-d` uploads the distribution files to PyPi   
-`./build --test|-t` uploads the dictribution files to TestPyPi   
-`./build --discard` **discards all changes to the local copy** of the repo and pulls the current state of the repo from GitHub.
+## Installation
+
+```
+pip install mausy5043-common
+```
+
 
 ## Functions provided
 `cat(filename)` : Read a file into a variable.   
 `syslog_trace(trace, logerr, out2console)` : Log messages to console and/or system log.   
 `moisture(temperature, relative_humidity, pressure)` : Calculate the moisture content of air given T [degC], RH [%] and P [hPa].   
 `wet_bulb_temperature(temperature, relative_humidity)` : Calculate the wet bulb temperature of the air given T [degC] and RH [%].
```

### Comparing `mausy5043_common-1.2.3/pyproject.toml` & `mausy5043_common-1.4.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mausy5043-common"
 description = "Common python functions"
-version = "1.2.3"
+version = "1.4.1"
 dependencies = [
     "numpy",
     "pandas",
 ]
 authors = [
   { name="Mausy5043" },
 ]
```

### Comparing `mausy5043_common-1.2.3/PKG-INFO` & `mausy5043_common-1.4.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mausy5043-common
-Version: 1.2.3
+Version: 1.4.1
 Summary: Common python functions
 Project-URL: Homepage, https://github.com/Mausy5043/mausy5043-common
 Project-URL: Bug Tracker, https://github.com/Mausy5043/mausy5043-common/issues
 Author: Mausy5043
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
@@ -22,26 +22,28 @@
 # mausy5043-common
 
 [![PyPI version](https://img.shields.io/pypi/v/mausy5043-common.svg?logo=pypi&logoColor=FFE873)](https://pypi.org/project/mausy5043-common)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/mausy5043-common.svg?logo=python&logoColor=FFE873)](https://pypi.org/project/mausy5043-common)
 [![PyPI downloads](https://img.shields.io/pypi/dm/mausy5043-common.svg)](https://pypistats.org/packages/mausy5043-common)
 [![Code style: Black](https://img.shields.io/badge/code%20style-Black-000000.svg)](https://github.com/psf/black)
 
-Provides various Python3 functions and classes for personal use.
+This is a Python3 library of functions and classes, mainly for personal use.
 
-## NOTE:
-### user action required !!
+## Requirements
+
+**NOTE: user action required !!**  
 Before trying to use the SQLITE3 functions in this package make sure you have installed the sqlite3 server/client and 
 the default Python package that comes with it.
 
-## Available commands for package building
-`./build --build|-b` builds the distribution files   
-`./build --dist|-d` uploads the distribution files to PyPi   
-`./build --test|-t` uploads the dictribution files to TestPyPi   
-`./build --discard` **discards all changes to the local copy** of the repo and pulls the current state of the repo from GitHub.
+## Installation
+
+```
+pip install mausy5043-common
+```
+
 
 ## Functions provided
 `cat(filename)` : Read a file into a variable.   
 `syslog_trace(trace, logerr, out2console)` : Log messages to console and/or system log.   
 `moisture(temperature, relative_humidity, pressure)` : Calculate the moisture content of air given T [degC], RH [%] and P [hPa].   
 `wet_bulb_temperature(temperature, relative_humidity)` : Calculate the wet bulb temperature of the air given T [degC] and RH [%].
```

