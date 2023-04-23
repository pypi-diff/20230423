# Comparing `tmp/mausy5043_common-1.4.1.tar.gz` & `tmp/mausy5043_common-1.4.2.tar.gz`

## Comparing `mausy5043_common-1.4.1.tar` & `mausy5043_common-1.4.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 mausy5043_common-1.4.1/.editorconfig
--rw-r--r--   0        0        0    20752 2020-02-02 00:00:00.000000 mausy5043_common-1.4.1/.pylintrc
--rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 mausy5043_common-1.4.1/BUILDING.md
--rwxr-xr-x   0        0        0     2227 2020-02-02 00:00:00.000000 mausy5043_common-1.4.1/build
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 mausy5043_common-1.4.1/requirements.txt
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 mausy5043_common-1.4.1/tox.ini
--rwxr-xr-x   0        0        0       68 2020-02-02 00:00:00.000000 mausy5043_common-1.4.1/src/mausy5043_common/__init__.py
--rwxr-xr-x   0        0        0      951 2020-02-02 00:00:00.000000 mausy5043_common-1.4.1/src/mausy5043_common/funfile.py
--rwxr-xr-x   0        0        0     1396 2020-02-02 00:00:00.000000 mausy5043_common-1.4.1/src/mausy5043_common/funmeteo.py
--rwxr-xr-x   0        0        0      641 2020-02-02 00:00:00.000000 mausy5043_common-1.4.1/src/mausy5043_common/libsignals.py
--rwxr-xr-x   0        0        0     8699 2020-02-02 00:00:00.000000 mausy5043_common-1.4.1/src/mausy5043_common/libsqlite3.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mausy5043_common-1.4.1/tests/.placeholder
--rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 mausy5043_common-1.4.1/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 mausy5043_common-1.4.1/LICENSE
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 mausy5043_common-1.4.1/README.md
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 mausy5043_common-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 mausy5043_common-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 mausy5043_common-1.4.2/.editorconfig
+-rw-r--r--   0        0        0    20752 2020-02-02 00:00:00.000000 mausy5043_common-1.4.2/.pylintrc
+-rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 mausy5043_common-1.4.2/BUILDING.md
+-rwxr-xr-x   0        0        0     2210 2020-02-02 00:00:00.000000 mausy5043_common-1.4.2/build
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 mausy5043_common-1.4.2/requirements.txt
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 mausy5043_common-1.4.2/tox.ini
+-rwxr-xr-x   0        0        0       68 2020-02-02 00:00:00.000000 mausy5043_common-1.4.2/src/mausy5043_common/__init__.py
+-rwxr-xr-x   0        0        0      951 2020-02-02 00:00:00.000000 mausy5043_common-1.4.2/src/mausy5043_common/funfile.py
+-rwxr-xr-x   0        0        0     1396 2020-02-02 00:00:00.000000 mausy5043_common-1.4.2/src/mausy5043_common/funmeteo.py
+-rwxr-xr-x   0        0        0      641 2020-02-02 00:00:00.000000 mausy5043_common-1.4.2/src/mausy5043_common/libsignals.py
+-rwxr-xr-x   0        0        0     8906 2020-02-02 00:00:00.000000 mausy5043_common-1.4.2/src/mausy5043_common/libsqlite3.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mausy5043_common-1.4.2/tests/.placeholder
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 mausy5043_common-1.4.2/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 mausy5043_common-1.4.2/LICENSE
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 mausy5043_common-1.4.2/README.md
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 mausy5043_common-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 mausy5043_common-1.4.2/PKG-INFO
```

### Comparing `mausy5043_common-1.4.1/.pylintrc` & `mausy5043_common-1.4.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `mausy5043_common-1.4.1/BUILDING.md` & `mausy5043_common-1.4.2/BUILDING.md`

 * *Files identical despite different names*

### Comparing `mausy5043_common-1.4.1/build` & `mausy5043_common-1.4.2/build`

 * *Files 1% similar despite different names*

```diff
@@ -48,16 +48,14 @@
     branch_name=$1
     git fetch origin "${branch_name}" || { sleep 60; git fetch origin "${branch_name}" || exit 1; }
     git reset --hard "origin/${branch_name}" || exit 1
     git clean -f -d || exit 1
     git pull || exit 1
 }
 
-"${HERE}"/check
-
 # check commandline parameters
 case $CMD in
     -b | --build)
         # build
         build_app "${HERE}" || exit 1
         ;;
     -d | --dist)
```

### Comparing `mausy5043_common-1.4.1/tox.ini` & `mausy5043_common-1.4.2/tox.ini`

 * *Files identical despite different names*

### Comparing `mausy5043_common-1.4.1/src/mausy5043_common/funfile.py` & `mausy5043_common-1.4.2/src/mausy5043_common/funfile.py`

 * *Files identical despite different names*

### Comparing `mausy5043_common-1.4.1/src/mausy5043_common/funmeteo.py` & `mausy5043_common-1.4.2/src/mausy5043_common/funmeteo.py`

 * *Files identical despite different names*

### Comparing `mausy5043_common-1.4.1/src/mausy5043_common/libsignals.py` & `mausy5043_common-1.4.2/src/mausy5043_common/libsignals.py`

 * *Files identical despite different names*

### Comparing `mausy5043_common-1.4.1/src/mausy5043_common/libsqlite3.py` & `mausy5043_common-1.4.2/src/mausy5043_common/libsqlite3.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,14 +153,18 @@
                     sql_command = f'DELETE FROM {self.table} WHERE {df_idx} = "{element_time}";'
                     cursor = consql.cursor()
                     try:
                         cursor.execute(sql_command)
                         cursor.fetchone()
                         cursor.close()
                         consql.commit()
+                    except s3.IntegrityError:
+                        pass
+                        # probably "sqlite3.IntegrityError: UNIQUE constraint failed".
+                        # this can be passed
                     except s3.Error as her:
                         mf.syslog_trace(
                             # pylint: disable-next=C0301
                             f"SQLite3 error of type {type(her).__name__} when commiting to server.",
                             syslog.LOG_ERR,
                             self.debug,
                         )
```

### Comparing `mausy5043_common-1.4.1/.gitignore` & `mausy5043_common-1.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `mausy5043_common-1.4.1/LICENSE` & `mausy5043_common-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mausy5043_common-1.4.1/README.md` & `mausy5043_common-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `mausy5043_common-1.4.1/pyproject.toml` & `mausy5043_common-1.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mausy5043-common"
 description = "Common python functions"
-version = "1.4.1"
+version = "1.4.2"
 dependencies = [
     "numpy",
     "pandas",
 ]
 authors = [
   { name="Mausy5043" },
 ]
```

### Comparing `mausy5043_common-1.4.1/PKG-INFO` & `mausy5043_common-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mausy5043-common
-Version: 1.4.1
+Version: 1.4.2
 Summary: Common python functions
 Project-URL: Homepage, https://github.com/Mausy5043/mausy5043-common
 Project-URL: Bug Tracker, https://github.com/Mausy5043/mausy5043-common/issues
 Author: Mausy5043
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
```

