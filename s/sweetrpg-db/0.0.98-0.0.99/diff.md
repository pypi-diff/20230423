# Comparing `tmp/sweetrpg-db-0.0.98.tar.gz` & `tmp/sweetrpg-db-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sweetrpg-db-0.0.98.tar", last modified: Sun Mar 19 00:25:14 2023, max compression
+gzip compressed data, was "sweetrpg-db-0.0.99.tar", last modified: Sun Mar 19 01:39:05 2023, max compression
```

## Comparing `sweetrpg-db-0.0.98.tar` & `sweetrpg-db-0.0.99.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-19 00:25:14.947989 sweetrpg-db-0.0.98/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-03-19 00:25:11.000000 sweetrpg-db-0.0.98/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1974 2023-03-19 00:25:14.947989 sweetrpg-db-0.0.98/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1354 2023-03-19 00:25:11.000000 sweetrpg-db-0.0.98/README.md
--rw-r--r--   0 root         (0) root         (0)     1125 2023-03-19 00:25:14.947989 sweetrpg-db-0.0.98/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      334 2023-03-19 00:25:11.000000 sweetrpg-db-0.0.98/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-19 00:25:14.943989 sweetrpg-db-0.0.98/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-19 00:25:14.943989 sweetrpg-db-0.0.98/src/sweetrpg_db/
--rw-r--r--   0 root         (0) root         (0)      387 2023-03-19 00:25:12.000000 sweetrpg-db-0.0.98/src/sweetrpg_db/__init__.py
--rw-r--r--   0 root         (0) root         (0)      190 2023-03-19 00:25:11.000000 sweetrpg-db-0.0.98/src/sweetrpg_db/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-19 00:25:14.947989 sweetrpg-db-0.0.98/src/sweetrpg_db/mongodb/
--rw-r--r--   0 root         (0) root         (0)      118 2023-03-19 00:25:11.000000 sweetrpg-db-0.0.98/src/sweetrpg_db/mongodb/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3749 2023-03-19 00:25:11.000000 sweetrpg-db-0.0.98/src/sweetrpg_db/mongodb/options.py
--rw-r--r--   0 root         (0) root         (0)     9966 2023-03-19 00:25:11.000000 sweetrpg-db-0.0.98/src/sweetrpg_db/mongodb/repo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-19 00:25:14.947989 sweetrpg-db-0.0.98/src/sweetrpg_db/schema/
--rw-r--r--   0 root         (0) root         (0)       96 2023-03-19 00:25:11.000000 sweetrpg-db-0.0.98/src/sweetrpg_db/schema/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-19 00:25:11.000000 sweetrpg-db-0.0.98/src/sweetrpg_db/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-19 00:25:14.947989 sweetrpg-db-0.0.98/src/sweetrpg_db.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1974 2023-03-19 00:25:14.000000 sweetrpg-db-0.0.98/src/sweetrpg_db.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      493 2023-03-19 00:25:14.000000 sweetrpg-db-0.0.98/src/sweetrpg_db.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-19 00:25:14.000000 sweetrpg-db-0.0.98/src/sweetrpg_db.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-03-19 00:25:14.000000 sweetrpg-db-0.0.98/src/sweetrpg_db.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       87 2023-03-19 00:25:14.000000 sweetrpg-db-0.0.98/src/sweetrpg_db.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-03-19 00:25:14.000000 sweetrpg-db-0.0.98/src/sweetrpg_db.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-19 01:39:05.035914 sweetrpg-db-0.0.99/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-03-19 01:39:01.000000 sweetrpg-db-0.0.99/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1974 2023-03-19 01:39:05.035914 sweetrpg-db-0.0.99/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1354 2023-03-19 01:39:01.000000 sweetrpg-db-0.0.99/README.md
+-rw-r--r--   0 root         (0) root         (0)     1125 2023-03-19 01:39:05.039914 sweetrpg-db-0.0.99/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      334 2023-03-19 01:39:01.000000 sweetrpg-db-0.0.99/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-19 01:39:05.035914 sweetrpg-db-0.0.99/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-19 01:39:05.035914 sweetrpg-db-0.0.99/src/sweetrpg_db/
+-rw-r--r--   0 root         (0) root         (0)      387 2023-03-19 01:39:02.000000 sweetrpg-db-0.0.99/src/sweetrpg_db/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      190 2023-03-19 01:39:01.000000 sweetrpg-db-0.0.99/src/sweetrpg_db/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-19 01:39:05.035914 sweetrpg-db-0.0.99/src/sweetrpg_db/mongodb/
+-rw-r--r--   0 root         (0) root         (0)      118 2023-03-19 01:39:01.000000 sweetrpg-db-0.0.99/src/sweetrpg_db/mongodb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3749 2023-03-19 01:39:01.000000 sweetrpg-db-0.0.99/src/sweetrpg_db/mongodb/options.py
+-rw-r--r--   0 root         (0) root         (0)     9966 2023-03-19 01:39:01.000000 sweetrpg-db-0.0.99/src/sweetrpg_db/mongodb/repo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-19 01:39:05.035914 sweetrpg-db-0.0.99/src/sweetrpg_db/schema/
+-rw-r--r--   0 root         (0) root         (0)       96 2023-03-19 01:39:01.000000 sweetrpg-db-0.0.99/src/sweetrpg_db/schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-19 01:39:01.000000 sweetrpg-db-0.0.99/src/sweetrpg_db/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-19 01:39:05.035914 sweetrpg-db-0.0.99/src/sweetrpg_db.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1974 2023-03-19 01:39:05.000000 sweetrpg-db-0.0.99/src/sweetrpg_db.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      493 2023-03-19 01:39:05.000000 sweetrpg-db-0.0.99/src/sweetrpg_db.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-19 01:39:05.000000 sweetrpg-db-0.0.99/src/sweetrpg_db.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-03-19 01:39:05.000000 sweetrpg-db-0.0.99/src/sweetrpg_db.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       87 2023-03-19 01:39:05.000000 sweetrpg-db-0.0.99/src/sweetrpg_db.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-03-19 01:39:05.000000 sweetrpg-db-0.0.99/src/sweetrpg_db.egg-info/top_level.txt
```

### Comparing `sweetrpg-db-0.0.98/LICENSE` & `sweetrpg-db-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `sweetrpg-db-0.0.98/PKG-INFO` & `sweetrpg-db-0.0.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sweetrpg-db
-Version: 0.0.98
+Version: 0.0.99
 Home-page: https://sweetrpg.com
 Author: Paul Schifferer
 Author-email: dm@sweetrpg.com
 License: MIT
 Project-URL: Documentation, https://sweetrpg.github.io/db
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
```

### Comparing `sweetrpg-db-0.0.98/README.md` & `sweetrpg-db-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `sweetrpg-db-0.0.98/setup.cfg` & `sweetrpg-db-0.0.99/setup.cfg`

 * *Files identical despite different names*

### Comparing `sweetrpg-db-0.0.98/src/sweetrpg_db/mongodb/options.py` & `sweetrpg-db-0.0.99/src/sweetrpg_db/mongodb/options.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-db-0.0.98/src/sweetrpg_db/mongodb/repo.py` & `sweetrpg-db-0.0.99/src/sweetrpg_db/mongodb/repo.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-db-0.0.98/src/sweetrpg_db.egg-info/PKG-INFO` & `sweetrpg-db-0.0.99/src/sweetrpg_db.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sweetrpg-db
-Version: 0.0.98
+Version: 0.0.99
 Home-page: https://sweetrpg.com
 Author: Paul Schifferer
 Author-email: dm@sweetrpg.com
 License: MIT
 Project-URL: Documentation, https://sweetrpg.github.io/db
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
```

