# Comparing `tmp/scandb-1.0.0.tar.gz` & `tmp/scandb-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scandb-1.0.0.tar", last modified: Sat Jan 28 23:40:54 2023, max compression
+gzip compressed data, was "scandb-1.0.1.tar", last modified: Sun Apr 23 20:41:44 2023, max compression
```

## Comparing `scandb-1.0.0.tar` & `scandb-1.0.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-01-28 23:40:54.332509 scandb-1.0.0/
--rw-r--r--   0 cb        (1000) cb        (1000)    12259 2023-01-28 23:40:54.332509 scandb-1.0.0/PKG-INFO
--rw-r--r--   0 cb        (1000) cb        (1000)    11881 2021-01-24 22:23:04.000000 scandb-1.0.0/README.md
-drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-01-28 23:40:54.332509 scandb-1.0.0/scandb/
--rw-r--r--   0 cb        (1000) cb        (1000)        0 2021-01-08 23:12:58.000000 scandb-1.0.0/scandb/__init__.py
--rw-r--r--   0 cb        (1000) cb        (1000)     6776 2023-01-28 23:32:36.000000 scandb-1.0.0/scandb/compare.py
-drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-01-28 23:40:54.332509 scandb-1.0.0/scandb/importer/
--rw-r--r--   0 cb        (1000) cb        (1000)        0 2021-01-08 23:12:58.000000 scandb-1.0.0/scandb/importer/__init__.py
--rw-r--r--   0 cb        (1000) cb        (1000)     1981 2023-01-28 23:32:36.000000 scandb-1.0.0/scandb/importer/cli.py
--rwxr-xr-x   0 cb        (1000) cb        (1000)     5216 2023-01-28 23:32:36.000000 scandb-1.0.0/scandb/importer/nessus.py
--rwxr-xr-x   0 cb        (1000) cb        (1000)     2690 2023-01-28 23:32:36.000000 scandb-1.0.0/scandb/importer/nmap.py
--rw-r--r--   0 cb        (1000) cb        (1000)     2114 2021-01-08 23:12:58.000000 scandb-1.0.0/scandb/importer/util.py
-drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-01-28 23:40:54.332509 scandb-1.0.0/scandb/models/
--rw-r--r--   0 cb        (1000) cb        (1000)        0 2021-01-08 23:12:58.000000 scandb-1.0.0/scandb/models/__init__.py
--rwxr-xr-x   0 cb        (1000) cb        (1000)     5586 2023-01-28 23:32:36.000000 scandb-1.0.0/scandb/models/db.py
--rw-r--r--   0 cb        (1000) cb        (1000)    23113 2021-04-07 19:45:57.000000 scandb-1.0.0/scandb/models/report.py
-drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-01-28 23:40:54.332509 scandb-1.0.0/scandb/report/
--rw-r--r--   0 cb        (1000) cb        (1000)        0 2021-01-08 23:12:58.000000 scandb-1.0.0/scandb/report/__init__.py
--rw-r--r--   0 cb        (1000) cb        (1000)     5629 2023-01-28 23:32:36.000000 scandb-1.0.0/scandb/report/cli.py
--rw-r--r--   0 cb        (1000) cb        (1000)     4383 2023-01-28 23:32:36.000000 scandb-1.0.0/scandb/report/queries.py
--rw-r--r--   0 cb        (1000) cb        (1000)     3195 2023-01-28 23:32:36.000000 scandb-1.0.0/scandb/report/util.py
-drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-01-28 23:40:54.332509 scandb-1.0.0/scandb/services/
--rw-r--r--   0 cb        (1000) cb        (1000)        0 2021-01-08 23:12:58.000000 scandb-1.0.0/scandb/services/__init__.py
--rw-r--r--   0 cb        (1000) cb        (1000)     2457 2021-01-08 23:12:58.000000 scandb-1.0.0/scandb/services/cli.py
--rw-r--r--   0 cb        (1000) cb        (1000)     1574 2023-01-28 23:32:36.000000 scandb-1.0.0/scandb/services/queries.py
-drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-01-28 23:40:54.332509 scandb-1.0.0/scandb/statistics/
--rw-r--r--   0 cb        (1000) cb        (1000)        0 2021-01-08 23:12:58.000000 scandb-1.0.0/scandb/statistics/__init__.py
--rw-r--r--   0 cb        (1000) cb        (1000)     7722 2021-04-16 22:44:27.000000 scandb-1.0.0/scandb/statistics/cli.py
--rw-r--r--   0 cb        (1000) cb        (1000)     4687 2023-01-28 23:32:36.000000 scandb-1.0.0/scandb/statistics/queries.py
-drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-01-28 23:40:54.332509 scandb-1.0.0/scandb/vulns/
--rw-r--r--   0 cb        (1000) cb        (1000)        0 2021-01-08 23:12:58.000000 scandb-1.0.0/scandb/vulns/__init__.py
--rw-r--r--   0 cb        (1000) cb        (1000)     6872 2023-01-28 23:32:36.000000 scandb-1.0.0/scandb/vulns/cli.py
--rw-r--r--   0 cb        (1000) cb        (1000)     3655 2023-01-28 23:32:36.000000 scandb-1.0.0/scandb/vulns/queries.py
-drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-01-28 23:40:54.332509 scandb-1.0.0/scandb.egg-info/
--rw-r--r--   0 cb        (1000) cb        (1000)    12259 2023-01-28 23:40:54.000000 scandb-1.0.0/scandb.egg-info/PKG-INFO
--rw-r--r--   0 cb        (1000) cb        (1000)      757 2023-01-28 23:40:54.000000 scandb-1.0.0/scandb.egg-info/SOURCES.txt
--rw-r--r--   0 cb        (1000) cb        (1000)        1 2023-01-28 23:40:54.000000 scandb-1.0.0/scandb.egg-info/dependency_links.txt
--rw-r--r--   0 cb        (1000) cb        (1000)      309 2023-01-28 23:40:54.000000 scandb-1.0.0/scandb.egg-info/entry_points.txt
--rw-r--r--   0 cb        (1000) cb        (1000)       87 2023-01-28 23:40:54.000000 scandb-1.0.0/scandb.egg-info/requires.txt
--rw-r--r--   0 cb        (1000) cb        (1000)        7 2023-01-28 23:40:54.000000 scandb-1.0.0/scandb.egg-info/top_level.txt
--rw-r--r--   0 cb        (1000) cb        (1000)       38 2023-01-28 23:40:54.332509 scandb-1.0.0/setup.cfg
--rw-r--r--   0 cb        (1000) cb        (1000)     1581 2023-01-28 23:32:36.000000 scandb-1.0.0/setup.py
+drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-04-23 20:41:44.761252 scandb-1.0.1/
+-rw-r--r--   0 cb        (1000) cb        (1000)    12259 2023-04-23 20:41:44.761252 scandb-1.0.1/PKG-INFO
+-rw-r--r--   0 cb        (1000) cb        (1000)    11881 2021-01-24 22:23:04.000000 scandb-1.0.1/README.md
+drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-04-23 20:41:44.757919 scandb-1.0.1/scandb/
+-rw-r--r--   0 cb        (1000) cb        (1000)        0 2021-01-08 23:12:58.000000 scandb-1.0.1/scandb/__init__.py
+-rw-r--r--   0 cb        (1000) cb        (1000)     6776 2023-01-28 23:32:36.000000 scandb-1.0.1/scandb/compare.py
+drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-04-23 20:41:44.757919 scandb-1.0.1/scandb/importer/
+-rw-r--r--   0 cb        (1000) cb        (1000)        0 2021-01-08 23:12:58.000000 scandb-1.0.1/scandb/importer/__init__.py
+-rw-r--r--   0 cb        (1000) cb        (1000)     1981 2023-01-28 23:32:36.000000 scandb-1.0.1/scandb/importer/cli.py
+-rwxr-xr-x   0 cb        (1000) cb        (1000)     5216 2023-01-28 23:32:36.000000 scandb-1.0.1/scandb/importer/nessus.py
+-rwxr-xr-x   0 cb        (1000) cb        (1000)     2690 2023-01-28 23:32:36.000000 scandb-1.0.1/scandb/importer/nmap.py
+-rw-r--r--   0 cb        (1000) cb        (1000)     2114 2021-01-08 23:12:58.000000 scandb-1.0.1/scandb/importer/util.py
+drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-04-23 20:41:44.757919 scandb-1.0.1/scandb/models/
+-rw-r--r--   0 cb        (1000) cb        (1000)        0 2021-01-08 23:12:58.000000 scandb-1.0.1/scandb/models/__init__.py
+-rwxr-xr-x   0 cb        (1000) cb        (1000)     5586 2023-04-23 20:34:45.000000 scandb-1.0.1/scandb/models/db.py
+-rw-r--r--   0 cb        (1000) cb        (1000)    23113 2021-04-07 19:45:57.000000 scandb-1.0.1/scandb/models/report.py
+drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-04-23 20:41:44.757919 scandb-1.0.1/scandb/report/
+-rw-r--r--   0 cb        (1000) cb        (1000)        0 2021-01-08 23:12:58.000000 scandb-1.0.1/scandb/report/__init__.py
+-rw-r--r--   0 cb        (1000) cb        (1000)     5629 2023-01-28 23:32:36.000000 scandb-1.0.1/scandb/report/cli.py
+-rw-r--r--   0 cb        (1000) cb        (1000)     4383 2023-01-28 23:32:36.000000 scandb-1.0.1/scandb/report/queries.py
+-rw-r--r--   0 cb        (1000) cb        (1000)     3195 2023-01-28 23:32:36.000000 scandb-1.0.1/scandb/report/util.py
+drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-04-23 20:41:44.757919 scandb-1.0.1/scandb/services/
+-rw-r--r--   0 cb        (1000) cb        (1000)        0 2021-01-08 23:12:58.000000 scandb-1.0.1/scandb/services/__init__.py
+-rw-r--r--   0 cb        (1000) cb        (1000)     2457 2021-01-08 23:12:58.000000 scandb-1.0.1/scandb/services/cli.py
+-rw-r--r--   0 cb        (1000) cb        (1000)     1574 2023-01-28 23:32:36.000000 scandb-1.0.1/scandb/services/queries.py
+drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-04-23 20:41:44.757919 scandb-1.0.1/scandb/statistics/
+-rw-r--r--   0 cb        (1000) cb        (1000)        0 2021-01-08 23:12:58.000000 scandb-1.0.1/scandb/statistics/__init__.py
+-rw-r--r--   0 cb        (1000) cb        (1000)     7722 2021-04-16 22:44:27.000000 scandb-1.0.1/scandb/statistics/cli.py
+-rw-r--r--   0 cb        (1000) cb        (1000)     4687 2023-01-28 23:32:36.000000 scandb-1.0.1/scandb/statistics/queries.py
+drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-04-23 20:41:44.761252 scandb-1.0.1/scandb/vulns/
+-rw-r--r--   0 cb        (1000) cb        (1000)        0 2021-01-08 23:12:58.000000 scandb-1.0.1/scandb/vulns/__init__.py
+-rw-r--r--   0 cb        (1000) cb        (1000)     6872 2023-01-28 23:32:36.000000 scandb-1.0.1/scandb/vulns/cli.py
+-rw-r--r--   0 cb        (1000) cb        (1000)     3655 2023-01-28 23:32:36.000000 scandb-1.0.1/scandb/vulns/queries.py
+drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-04-23 20:41:44.757919 scandb-1.0.1/scandb.egg-info/
+-rw-r--r--   0 cb        (1000) cb        (1000)    12259 2023-04-23 20:41:44.000000 scandb-1.0.1/scandb.egg-info/PKG-INFO
+-rw-r--r--   0 cb        (1000) cb        (1000)      757 2023-04-23 20:41:44.000000 scandb-1.0.1/scandb.egg-info/SOURCES.txt
+-rw-r--r--   0 cb        (1000) cb        (1000)        1 2023-04-23 20:41:44.000000 scandb-1.0.1/scandb.egg-info/dependency_links.txt
+-rw-r--r--   0 cb        (1000) cb        (1000)      309 2023-04-23 20:41:44.000000 scandb-1.0.1/scandb.egg-info/entry_points.txt
+-rw-r--r--   0 cb        (1000) cb        (1000)       93 2023-04-23 20:41:44.000000 scandb-1.0.1/scandb.egg-info/requires.txt
+-rw-r--r--   0 cb        (1000) cb        (1000)        7 2023-04-23 20:41:44.000000 scandb-1.0.1/scandb.egg-info/top_level.txt
+-rw-r--r--   0 cb        (1000) cb        (1000)       38 2023-04-23 20:41:44.761252 scandb-1.0.1/setup.cfg
+-rw-r--r--   0 cb        (1000) cb        (1000)     1587 2023-04-23 20:36:37.000000 scandb-1.0.1/setup.py
```

### Comparing `scandb-1.0.0/PKG-INFO` & `scandb-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scandb
-Version: 1.0.0
+Version: 1.0.1
 Summary: Scripts to import nmap and nessus scan results into a SQLite database, analyze the overall results and generate reports or target lists.
 Home-page: https://bitbucket.org/cbless/scandb
 Author: Christoph Bless
 Author-email: bitbucket@cbless.de
 License:  GPLv3
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `scandb-1.0.0/README.md` & `scandb-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `scandb-1.0.0/scandb/compare.py` & `scandb-1.0.1/scandb/compare.py`

 * *Files identical despite different names*

### Comparing `scandb-1.0.0/scandb/importer/cli.py` & `scandb-1.0.1/scandb/importer/cli.py`

 * *Files identical despite different names*

### Comparing `scandb-1.0.0/scandb/importer/nessus.py` & `scandb-1.0.1/scandb/importer/nessus.py`

 * *Files identical despite different names*

### Comparing `scandb-1.0.0/scandb/importer/nmap.py` & `scandb-1.0.1/scandb/importer/nmap.py`

 * *Files identical despite different names*

### Comparing `scandb-1.0.0/scandb/importer/util.py` & `scandb-1.0.1/scandb/importer/util.py`

 * *Files identical despite different names*

### Comparing `scandb-1.0.0/scandb/models/db.py` & `scandb-1.0.1/scandb/models/db.py`

 * *Files identical despite different names*

### Comparing `scandb-1.0.0/scandb/models/report.py` & `scandb-1.0.1/scandb/models/report.py`

 * *Files identical despite different names*

### Comparing `scandb-1.0.0/scandb/report/cli.py` & `scandb-1.0.1/scandb/report/cli.py`

 * *Files identical despite different names*

### Comparing `scandb-1.0.0/scandb/report/queries.py` & `scandb-1.0.1/scandb/report/queries.py`

 * *Files identical despite different names*

### Comparing `scandb-1.0.0/scandb/report/util.py` & `scandb-1.0.1/scandb/report/util.py`

 * *Files identical despite different names*

### Comparing `scandb-1.0.0/scandb/services/cli.py` & `scandb-1.0.1/scandb/services/cli.py`

 * *Files identical despite different names*

### Comparing `scandb-1.0.0/scandb/services/queries.py` & `scandb-1.0.1/scandb/services/queries.py`

 * *Files identical despite different names*

### Comparing `scandb-1.0.0/scandb/statistics/cli.py` & `scandb-1.0.1/scandb/statistics/cli.py`

 * *Files identical despite different names*

### Comparing `scandb-1.0.0/scandb/statistics/queries.py` & `scandb-1.0.1/scandb/statistics/queries.py`

 * *Files identical despite different names*

### Comparing `scandb-1.0.0/scandb/vulns/cli.py` & `scandb-1.0.1/scandb/vulns/cli.py`

 * *Files identical despite different names*

### Comparing `scandb-1.0.0/scandb/vulns/queries.py` & `scandb-1.0.1/scandb/vulns/queries.py`

 * *Files identical despite different names*

### Comparing `scandb-1.0.0/scandb.egg-info/PKG-INFO` & `scandb-1.0.1/scandb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scandb
-Version: 1.0.0
+Version: 1.0.1
 Summary: Scripts to import nmap and nessus scan results into a SQLite database, analyze the overall results and generate reports or target lists.
 Home-page: https://bitbucket.org/cbless/scandb
 Author: Christoph Bless
 Author-email: bitbucket@cbless.de
 License:  GPLv3
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `scandb-1.0.0/scandb.egg-info/SOURCES.txt` & `scandb-1.0.1/scandb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scandb-1.0.0/setup.py` & `scandb-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 long_description = ""
 # Get the long description from the README file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='scandb',
-    version='1.0.0',
+    version='1.0.1',
     author='Christoph Bless',
     author_email='bitbucket@cbless.de',
     url='https://bitbucket.org/cbless/scandb',
     license=' GPLv3',
     description=("Scripts to import nmap and nessus scan results into a SQLite database, analyze the overall results and generate reports or target lists."),
     long_description=long_description,
     long_description_content_type='text/markdown',
@@ -30,15 +30,15 @@
         'scandb.vulns'
     ],
     install_requires=[
         'argparse',
         'termcolor',
         'python-libnmap',
         'python-libnessus',
-        'SQLAlchemy',
+        'SQLAlchemy<2.0.0',
         'sqlalchemy-views',
         'docxtpl'
     ],
     entry_points = {
         "console_scripts": [
             "scandb-vulns = scandb.vulns.cli:vulns_cli",
             "scandb-services = scandb.services.cli:services_cli",
```

