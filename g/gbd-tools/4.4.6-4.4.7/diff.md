# Comparing `tmp/gbd_tools-4.4.6.tar.gz` & `tmp/gbd_tools-4.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gbd_tools-4.4.6.tar", last modified: Fri Apr 21 07:58:06 2023, max compression
+gzip compressed data, was "gbd_tools-4.4.7.tar", last modified: Sun Apr 23 09:07:43 2023, max compression
```

## Comparing `gbd_tools-4.4.6.tar` & `gbd_tools-4.4.7.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 07:58:06.851119 gbd_tools-4.4.6/
--rw-rw-r--   0 root         (0) root         (0)     1109 2023-01-02 08:34:51.000000 gbd_tools-4.4.6/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      206 2022-12-15 15:28:20.000000 gbd_tools-4.4.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3757 2023-04-21 07:58:06.851119 gbd_tools-4.4.6/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3248 2023-02-07 16:30:01.000000 gbd_tools-4.4.6/README.md
--rwxrwxr-x   0 root         (0) root         (0)    11281 2023-04-21 07:57:32.000000 gbd_tools-4.4.6/gbd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 07:58:06.847119 gbd_tools-4.4.6/gbd_core/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-12-12 14:03:01.000000 gbd_tools-4.4.6/gbd_core/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8294 2023-02-07 16:30:01.000000 gbd_tools-4.4.6/gbd_core/api.py
--rw-rw-r--   0 root         (0) root         (0)     1937 2023-04-20 08:28:49.000000 gbd_tools-4.4.6/gbd_core/contexts.py
--rw-rw-r--   0 root         (0) root         (0)    10190 2023-04-20 15:30:43.000000 gbd_tools-4.4.6/gbd_core/database.py
--rw-rw-r--   0 root         (0) root         (0)     5050 2023-02-07 16:30:01.000000 gbd_tools-4.4.6/gbd_core/grammar.py
--rw-rw-r--   0 root         (0) root         (0)     5786 2023-04-20 15:29:05.000000 gbd_tools-4.4.6/gbd_core/query.py
--rw-rw-r--   0 root         (0) root         (0)    12276 2023-04-20 15:44:03.000000 gbd_tools-4.4.6/gbd_core/schema.py
--rw-rw-r--   0 root         (0) root         (0)     4015 2023-04-20 08:28:49.000000 gbd_tools-4.4.6/gbd_core/util.py
--rw-rw-r--   0 root         (0) root         (0)     3333 2023-04-21 07:48:32.000000 gbd_tools-4.4.6/gbd_core/util_argparse.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 07:58:06.847119 gbd_tools-4.4.6/gbd_init/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-12-12 14:00:05.000000 gbd_tools-4.4.6/gbd_init/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7647 2023-04-20 08:28:49.000000 gbd_tools-4.4.6/gbd_init/cnf_extractors.py
--rw-rw-r--   0 root         (0) root         (0)     3853 2023-04-20 08:28:49.000000 gbd_tools-4.4.6/gbd_init/cnf_transformers.py
--rw-rw-r--   0 root         (0) root         (0)     2940 2023-04-20 08:28:49.000000 gbd_tools-4.4.6/gbd_init/gbdhash.py
--rw-rw-r--   0 root         (0) root         (0)     3513 2023-04-20 08:28:49.000000 gbd_tools-4.4.6/gbd_init/initializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 07:58:06.847119 gbd_tools-4.4.6/gbd_server/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-09-06 14:45:24.000000 gbd_tools-4.4.6/gbd_server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 07:58:06.847119 gbd_tools-4.4.6/gbd_server/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 07:58:06.847119 gbd_tools-4.4.6/gbd_server/static/img/
--rw-rw-r--   0 root         (0) root         (0)   125407 2022-09-06 14:45:24.000000 gbd_tools-4.4.6/gbd_server/static/img/gbd_logo.jpg
--rw-rw-r--   0 root         (0) root         (0)   835988 2022-09-06 14:45:24.000000 gbd_tools-4.4.6/gbd_server/static/img/gbd_logo.png
--rw-rw-r--   0 root         (0) root         (0)    32090 2022-09-06 14:45:24.000000 gbd_tools-4.4.6/gbd_server/static/img/gbd_logo_small.png
--rw-rw-r--   0 root         (0) root         (0)     1773 2023-04-16 15:10:50.000000 gbd_tools-4.4.6/gbd_server/static/main.css
--rw-rw-r--   0 root         (0) root         (0)    11975 2022-09-08 11:53:31.000000 gbd_tools-4.4.6/gbd_server/static/w3.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 07:58:06.847119 gbd_tools-4.4.6/gbd_server/templates/
--rw-rw-r--   0 root         (0) root         (0)     5016 2023-04-16 15:24:02.000000 gbd_tools-4.4.6/gbd_server/templates/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 07:58:06.851119 gbd_tools-4.4.6/gbd_tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3757 2023-04-21 07:58:06.000000 gbd_tools-4.4.6/gbd_tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      772 2023-04-21 07:58:06.000000 gbd_tools-4.4.6/gbd_tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 07:58:06.000000 gbd_tools-4.4.6/gbd_tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2023-04-21 07:58:06.000000 gbd_tools-4.4.6/gbd_tools.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       35 2023-04-21 07:58:06.000000 gbd_tools-4.4.6/gbd_tools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-21 07:58:06.000000 gbd_tools-4.4.6/gbd_tools.egg-info/top_level.txt
--rwxrwxr-x   0 root         (0) root         (0)    11989 2023-04-20 15:30:11.000000 gbd_tools-4.4.6/server.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-21 07:58:06.851119 gbd_tools-4.4.6/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)     1034 2023-04-21 07:57:40.000000 gbd_tools-4.4.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 09:07:43.355466 gbd_tools-4.4.7/
+-rw-rw-r--   0 root         (0) root         (0)     1109 2023-01-02 08:34:51.000000 gbd_tools-4.4.7/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      206 2022-12-15 15:28:20.000000 gbd_tools-4.4.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3757 2023-04-23 09:07:43.355466 gbd_tools-4.4.7/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     3248 2023-02-07 16:30:01.000000 gbd_tools-4.4.7/README.md
+-rwxrwxr-x   0 root         (0) root         (0)    11281 2023-04-21 07:57:32.000000 gbd_tools-4.4.7/gbd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 09:07:43.347466 gbd_tools-4.4.7/gbd_core/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-12-12 14:03:01.000000 gbd_tools-4.4.7/gbd_core/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8597 2023-04-23 09:05:25.000000 gbd_tools-4.4.7/gbd_core/api.py
+-rw-rw-r--   0 root         (0) root         (0)     1937 2023-04-20 08:28:49.000000 gbd_tools-4.4.7/gbd_core/contexts.py
+-rw-rw-r--   0 root         (0) root         (0)    10190 2023-04-20 15:30:43.000000 gbd_tools-4.4.7/gbd_core/database.py
+-rw-rw-r--   0 root         (0) root         (0)     5050 2023-02-07 16:30:01.000000 gbd_tools-4.4.7/gbd_core/grammar.py
+-rw-rw-r--   0 root         (0) root         (0)     5786 2023-04-20 15:29:05.000000 gbd_tools-4.4.7/gbd_core/query.py
+-rw-rw-r--   0 root         (0) root         (0)    12276 2023-04-20 15:44:03.000000 gbd_tools-4.4.7/gbd_core/schema.py
+-rw-rw-r--   0 root         (0) root         (0)     4015 2023-04-20 08:28:49.000000 gbd_tools-4.4.7/gbd_core/util.py
+-rw-rw-r--   0 root         (0) root         (0)     3333 2023-04-21 07:48:32.000000 gbd_tools-4.4.7/gbd_core/util_argparse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 09:07:43.347466 gbd_tools-4.4.7/gbd_init/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-12-12 14:00:05.000000 gbd_tools-4.4.7/gbd_init/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7647 2023-04-20 08:28:49.000000 gbd_tools-4.4.7/gbd_init/cnf_extractors.py
+-rw-rw-r--   0 root         (0) root         (0)     3853 2023-04-20 08:28:49.000000 gbd_tools-4.4.7/gbd_init/cnf_transformers.py
+-rw-rw-r--   0 root         (0) root         (0)     2940 2023-04-20 08:28:49.000000 gbd_tools-4.4.7/gbd_init/gbdhash.py
+-rw-rw-r--   0 root         (0) root         (0)     3513 2023-04-20 08:28:49.000000 gbd_tools-4.4.7/gbd_init/initializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 09:07:43.347466 gbd_tools-4.4.7/gbd_server/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-09-06 14:45:24.000000 gbd_tools-4.4.7/gbd_server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 09:07:43.347466 gbd_tools-4.4.7/gbd_server/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 09:07:43.351466 gbd_tools-4.4.7/gbd_server/static/img/
+-rw-rw-r--   0 root         (0) root         (0)   125407 2022-09-06 14:45:24.000000 gbd_tools-4.4.7/gbd_server/static/img/gbd_logo.jpg
+-rw-rw-r--   0 root         (0) root         (0)   835988 2022-09-06 14:45:24.000000 gbd_tools-4.4.7/gbd_server/static/img/gbd_logo.png
+-rw-rw-r--   0 root         (0) root         (0)    32090 2022-09-06 14:45:24.000000 gbd_tools-4.4.7/gbd_server/static/img/gbd_logo_small.png
+-rw-rw-r--   0 root         (0) root         (0)     1773 2023-04-16 15:10:50.000000 gbd_tools-4.4.7/gbd_server/static/main.css
+-rw-rw-r--   0 root         (0) root         (0)    11975 2022-09-08 11:53:31.000000 gbd_tools-4.4.7/gbd_server/static/w3.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 09:07:43.351466 gbd_tools-4.4.7/gbd_server/templates/
+-rw-rw-r--   0 root         (0) root         (0)     5016 2023-04-16 15:24:02.000000 gbd_tools-4.4.7/gbd_server/templates/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 09:07:43.355466 gbd_tools-4.4.7/gbd_tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3757 2023-04-23 09:07:43.000000 gbd_tools-4.4.7/gbd_tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      772 2023-04-23 09:07:43.000000 gbd_tools-4.4.7/gbd_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 09:07:43.000000 gbd_tools-4.4.7/gbd_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-04-23 09:07:43.000000 gbd_tools-4.4.7/gbd_tools.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-04-23 09:07:43.000000 gbd_tools-4.4.7/gbd_tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-23 09:07:43.000000 gbd_tools-4.4.7/gbd_tools.egg-info/top_level.txt
+-rwxrwxr-x   0 root         (0) root         (0)    11989 2023-04-20 15:30:11.000000 gbd_tools-4.4.7/server.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-23 09:07:43.355466 gbd_tools-4.4.7/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)     1034 2023-04-23 09:05:59.000000 gbd_tools-4.4.7/setup.py
```

### Comparing `gbd_tools-4.4.6/LICENSE` & `gbd_tools-4.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.6/PKG-INFO` & `gbd_tools-4.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gbd_tools
-Version: 4.4.6
+Version: 4.4.7
 Summary: GBD Benchmark Database Tools: Maintenance of Benchmark Instances and their Attributes
 Home-page: https://github.com/Udopia/gbd
 Author: Markus Iser, Karlsruhe Institute of Technology (KIT)
 Author-email: markus.iser@kit.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `gbd_tools-4.4.6/README.md` & `gbd_tools-4.4.7/README.md`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.6/gbd.py` & `gbd_tools-4.4.7/gbd.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.6/gbd_core/api.py` & `gbd_tools-4.4.7/gbd_core/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 from contextlib import ExitStack
 import traceback
 
 from gbd_core.query import GBDQuery
 from gbd_core.database import Database
 from gbd_core import util
+from gbd_init.gbdhash import identify
 
 
 class GBDException(Exception):
     pass
 
 
 class GBD:
@@ -43,14 +44,27 @@
             self._stack = stack.pop_all()
         return self
 
     def __exit__(self, exc_type, exc, traceback):
         self._stack.__exit__(exc_type, exc, traceback)
 
 
+    @classmethod
+    def identify(cls, path):
+        """ Identify the given benchmark by its GBD hash 
+
+            Args:
+                path (str): path to benchmark
+
+            Returns:
+                str: GBD hash
+        """
+        return identify(path)
+
+
     def query(self, gbd_query=None, hashes=[], resolve=[], collapse="group_concat", group_by="hash", join_type="LEFT", subselect=False):
         query_builder = GBDQuery(self.database, gbd_query)
         try:
             sql = query_builder.build_query(hashes, resolve or [], group_by or "hash", join_type, collapse, subselect)
         except tatsu.exceptions.FailedParse as err:
             if self.verbose:
                 util.eprint(traceback.format_exc())
```

### Comparing `gbd_tools-4.4.6/gbd_core/contexts.py` & `gbd_tools-4.4.7/gbd_core/contexts.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.6/gbd_core/database.py` & `gbd_tools-4.4.7/gbd_core/database.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.6/gbd_core/grammar.py` & `gbd_tools-4.4.7/gbd_core/grammar.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.6/gbd_core/query.py` & `gbd_tools-4.4.7/gbd_core/query.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.6/gbd_core/schema.py` & `gbd_tools-4.4.7/gbd_core/schema.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.6/gbd_core/util.py` & `gbd_tools-4.4.7/gbd_core/util.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.6/gbd_core/util_argparse.py` & `gbd_tools-4.4.7/gbd_core/util_argparse.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.6/gbd_init/cnf_extractors.py` & `gbd_tools-4.4.7/gbd_init/cnf_extractors.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.6/gbd_init/cnf_transformers.py` & `gbd_tools-4.4.7/gbd_init/cnf_transformers.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.6/gbd_init/gbdhash.py` & `gbd_tools-4.4.7/gbd_init/gbdhash.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.6/gbd_init/initializer.py` & `gbd_tools-4.4.7/gbd_init/initializer.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.6/gbd_server/static/img/gbd_logo.jpg` & `gbd_tools-4.4.7/gbd_server/static/img/gbd_logo.jpg`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.6/gbd_server/static/img/gbd_logo.png` & `gbd_tools-4.4.7/gbd_server/static/img/gbd_logo.png`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.6/gbd_server/static/img/gbd_logo_small.png` & `gbd_tools-4.4.7/gbd_server/static/img/gbd_logo_small.png`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.6/gbd_server/static/main.css` & `gbd_tools-4.4.7/gbd_server/static/main.css`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.6/gbd_server/static/w3.js` & `gbd_tools-4.4.7/gbd_server/static/w3.js`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.6/gbd_server/templates/index.html` & `gbd_tools-4.4.7/gbd_server/templates/index.html`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.6/gbd_tools.egg-info/PKG-INFO` & `gbd_tools-4.4.7/gbd_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gbd-tools
-Version: 4.4.6
+Version: 4.4.7
 Summary: GBD Benchmark Database Tools: Maintenance of Benchmark Instances and their Attributes
 Home-page: https://github.com/Udopia/gbd
 Author: Markus Iser, Karlsruhe Institute of Technology (KIT)
 Author-email: markus.iser@kit.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `gbd_tools-4.4.6/gbd_tools.egg-info/SOURCES.txt` & `gbd_tools-4.4.7/gbd_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.6/server.py` & `gbd_tools-4.4.7/server.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.6/setup.py` & `gbd_tools-4.4.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 setup(name='gbd_tools',
-  version='4.4.6',
+  version='4.4.7',
   description='GBD Benchmark Database Tools: Maintenance of Benchmark Instances and their Attributes',
   long_description=open('README.md', 'rt').read(),
   long_description_content_type="text/markdown",
   url='https://github.com/Udopia/gbd',
   author='Markus Iser, Karlsruhe Institute of Technology (KIT)',
   author_email='markus.iser@kit.edu',
   packages=[
```

