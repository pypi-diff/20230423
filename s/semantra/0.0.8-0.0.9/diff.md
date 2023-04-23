# Comparing `tmp/semantra-0.0.8.tar.gz` & `tmp/semantra-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantra-0.0.8.tar", last modified: Sun Apr 23 12:20:30 2023, max compression
+gzip compressed data, was "semantra-0.0.9.tar", last modified: Sun Apr 23 12:50:03 2023, max compression
```

## Comparing `semantra-0.0.8.tar` & `semantra-0.0.9.tar`

### file list

```diff
@@ -1,32 +1,43 @@
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 12:20:30.733525 semantra-0.0.8/
--rw-r--r--   0 freedmand   (501) staff       (20)     1071 2023-03-31 03:28:18.000000 semantra-0.0.8/LICENSE
--rw-r--r--   0 freedmand   (501) staff       (20)      102 2023-04-23 12:16:47.000000 semantra-0.0.8/MANIFEST.in
--rw-r--r--   0 freedmand   (501) staff       (20)     3488 2023-04-23 12:20:30.733363 semantra-0.0.8/PKG-INFO
--rw-r--r--   0 freedmand   (501) staff       (20)     3102 2023-04-16 16:45:22.000000 semantra-0.0.8/README.md
--rw-r--r--   0 freedmand   (501) staff       (20)        5 2023-04-23 12:20:01.000000 semantra-0.0.8/VERSION
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 12:20:30.722785 semantra-0.0.8/client/
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 12:20:30.724829 semantra-0.0.8/client/public/
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 12:20:30.726884 semantra-0.0.8/client/public/build/
--rw-r--r--   0 freedmand   (501) staff       (20)    14441 2023-04-22 21:42:14.000000 semantra-0.0.8/client/public/build/bundle.css
--rw-r--r--   0 freedmand   (501) staff       (20)   449074 2023-04-22 21:42:14.000000 semantra-0.0.8/client/public/build/bundle.js
--rw-r--r--   0 freedmand   (501) staff       (20)  1495716 2023-04-22 21:42:14.000000 semantra-0.0.8/client/public/build/bundle.js.map
--rw-r--r--   0 freedmand   (501) staff       (20)     3300 2023-04-09 04:23:49.000000 semantra-0.0.8/client/public/favicon.png
--rw-r--r--   0 freedmand   (501) staff       (20)      890 2023-02-15 22:52:41.000000 semantra-0.0.8/client/public/global.css
--rw-r--r--   0 freedmand   (501) staff       (20)      434 2023-04-09 20:49:05.000000 semantra-0.0.8/client/public/index.html
--rw-r--r--   0 freedmand   (501) staff       (20)      156 2023-04-23 03:03:00.000000 semantra-0.0.8/requirements.txt
--rw-r--r--   0 freedmand   (501) staff       (20)       38 2023-04-23 12:20:30.733568 semantra-0.0.8/setup.cfg
--rw-r--r--   0 freedmand   (501) staff       (20)     1185 2023-04-23 12:19:56.000000 semantra-0.0.8/setup.py
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 12:20:30.723062 semantra-0.0.8/src/
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 12:20:30.732085 semantra-0.0.8/src/semantra/
--rw-r--r--   0 freedmand   (501) staff       (20)        0 2023-04-23 04:39:23.000000 semantra-0.0.8/src/semantra/__init__.py
--rw-r--r--   0 freedmand   (501) staff       (20)    11172 2023-04-20 17:02:30.000000 semantra-0.0.8/src/semantra/models.py
--rw-r--r--   0 freedmand   (501) staff       (20)     3118 2023-04-23 04:31:52.000000 semantra-0.0.8/src/semantra/pdf.py
--rw-r--r--   0 freedmand   (501) staff       (20)    28787 2023-04-23 12:15:14.000000 semantra-0.0.8/src/semantra/semantra.py
--rw-r--r--   0 freedmand   (501) staff       (20)     4524 2023-04-22 20:05:23.000000 semantra-0.0.8/src/semantra/util.py
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 12:20:30.733153 semantra-0.0.8/src/semantra.egg-info/
--rw-r--r--   0 freedmand   (501) staff       (20)     3488 2023-04-23 12:20:30.000000 semantra-0.0.8/src/semantra.egg-info/PKG-INFO
--rw-r--r--   0 freedmand   (501) staff       (20)      566 2023-04-23 12:20:30.000000 semantra-0.0.8/src/semantra.egg-info/SOURCES.txt
--rw-r--r--   0 freedmand   (501) staff       (20)        1 2023-04-23 12:20:30.000000 semantra-0.0.8/src/semantra.egg-info/dependency_links.txt
--rw-r--r--   0 freedmand   (501) staff       (20)       52 2023-04-23 12:20:30.000000 semantra-0.0.8/src/semantra.egg-info/entry_points.txt
--rw-r--r--   0 freedmand   (501) staff       (20)      156 2023-04-23 12:20:30.000000 semantra-0.0.8/src/semantra.egg-info/requires.txt
--rw-r--r--   0 freedmand   (501) staff       (20)        9 2023-04-23 12:20:30.000000 semantra-0.0.8/src/semantra.egg-info/top_level.txt
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 12:50:03.430593 semantra-0.0.9/
+-rw-r--r--   0 freedmand   (501) staff       (20)     1071 2023-03-31 03:28:18.000000 semantra-0.0.9/LICENSE
+-rw-r--r--   0 freedmand   (501) staff       (20)     3645 2023-04-23 12:50:03.430233 semantra-0.0.9/PKG-INFO
+-rw-r--r--   0 freedmand   (501) staff       (20)     3102 2023-04-16 16:45:22.000000 semantra-0.0.9/README.md
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 12:50:03.414899 semantra-0.0.9/client/
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 12:50:03.416773 semantra-0.0.9/client/public/
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 12:50:03.418745 semantra-0.0.9/client/public/build/
+-rw-r--r--   0 freedmand   (501) staff       (20)    14441 2023-04-22 21:42:14.000000 semantra-0.0.9/client/public/build/bundle.css
+-rw-r--r--   0 freedmand   (501) staff       (20)   449074 2023-04-22 21:42:14.000000 semantra-0.0.9/client/public/build/bundle.js
+-rw-r--r--   0 freedmand   (501) staff       (20)  1495716 2023-04-22 21:42:14.000000 semantra-0.0.9/client/public/build/bundle.js.map
+-rw-r--r--   0 freedmand   (501) staff       (20)     3300 2023-04-09 04:23:49.000000 semantra-0.0.9/client/public/favicon.png
+-rw-r--r--   0 freedmand   (501) staff       (20)      890 2023-02-15 22:52:41.000000 semantra-0.0.9/client/public/global.css
+-rw-r--r--   0 freedmand   (501) staff       (20)      434 2023-04-09 20:49:05.000000 semantra-0.0.9/client/public/index.html
+-rw-r--r--   0 freedmand   (501) staff       (20)      995 2023-04-23 12:48:41.000000 semantra-0.0.9/pyproject.toml
+-rw-r--r--   0 freedmand   (501) staff       (20)       38 2023-04-23 12:50:03.430681 semantra-0.0.9/setup.cfg
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 12:50:03.415205 semantra-0.0.9/src/
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 12:50:03.422414 semantra-0.0.9/src/semantra/
+-rw-r--r--   0 freedmand   (501) staff       (20)        0 2023-04-23 04:39:23.000000 semantra-0.0.9/src/semantra/__init__.py
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 12:50:03.425724 semantra-0.0.9/src/semantra/__pycache__/
+-rw-r--r--   0 freedmand   (501) staff       (20)      148 2023-04-23 04:39:41.000000 semantra-0.0.9/src/semantra/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 freedmand   (501) staff       (20)    10961 2023-04-23 04:37:57.000000 semantra-0.0.9/src/semantra/__pycache__/models.cpython-39.pyc
+-rw-r--r--   0 freedmand   (501) staff       (20)     3086 2023-04-23 04:37:58.000000 semantra-0.0.9/src/semantra/__pycache__/pdf.cpython-39.pyc
+-rw-r--r--   0 freedmand   (501) staff       (20)    19561 2023-04-23 12:15:19.000000 semantra-0.0.9/src/semantra/__pycache__/semantra.cpython-39.pyc
+-rw-r--r--   0 freedmand   (501) staff       (20)     4744 2023-04-23 04:37:58.000000 semantra-0.0.9/src/semantra/__pycache__/util.cpython-39.pyc
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 12:50:03.426299 semantra-0.0.9/src/semantra/client_public/
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 12:50:03.427832 semantra-0.0.9/src/semantra/client_public/build/
+-rw-r--r--   0 freedmand   (501) staff       (20)    14441 2023-04-22 21:42:14.000000 semantra-0.0.9/src/semantra/client_public/build/bundle.css
+-rw-r--r--   0 freedmand   (501) staff       (20)   449074 2023-04-22 21:42:14.000000 semantra-0.0.9/src/semantra/client_public/build/bundle.js
+-rw-r--r--   0 freedmand   (501) staff       (20)  1495716 2023-04-22 21:42:14.000000 semantra-0.0.9/src/semantra/client_public/build/bundle.js.map
+-rw-r--r--   0 freedmand   (501) staff       (20)     3300 2023-04-09 04:23:49.000000 semantra-0.0.9/src/semantra/client_public/favicon.png
+-rw-r--r--   0 freedmand   (501) staff       (20)      890 2023-02-15 22:52:41.000000 semantra-0.0.9/src/semantra/client_public/global.css
+-rw-r--r--   0 freedmand   (501) staff       (20)      434 2023-04-09 20:49:05.000000 semantra-0.0.9/src/semantra/client_public/index.html
+-rw-r--r--   0 freedmand   (501) staff       (20)    11172 2023-04-20 17:02:30.000000 semantra-0.0.9/src/semantra/models.py
+-rw-r--r--   0 freedmand   (501) staff       (20)     3118 2023-04-23 04:31:52.000000 semantra-0.0.9/src/semantra/pdf.py
+-rw-r--r--   0 freedmand   (501) staff       (20)    28701 2023-04-23 12:49:54.000000 semantra-0.0.9/src/semantra/semantra.py
+-rw-r--r--   0 freedmand   (501) staff       (20)     4524 2023-04-22 20:05:23.000000 semantra-0.0.9/src/semantra/util.py
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 12:50:03.423626 semantra-0.0.9/src/semantra.egg-info/
+-rw-r--r--   0 freedmand   (501) staff       (20)     3645 2023-04-23 12:50:03.000000 semantra-0.0.9/src/semantra.egg-info/PKG-INFO
+-rw-r--r--   0 freedmand   (501) staff       (20)     1018 2023-04-23 12:50:03.000000 semantra-0.0.9/src/semantra.egg-info/SOURCES.txt
+-rw-r--r--   0 freedmand   (501) staff       (20)        1 2023-04-23 12:50:03.000000 semantra-0.0.9/src/semantra.egg-info/dependency_links.txt
+-rw-r--r--   0 freedmand   (501) staff       (20)       52 2023-04-23 12:50:03.000000 semantra-0.0.9/src/semantra.egg-info/entry_points.txt
+-rw-r--r--   0 freedmand   (501) staff       (20)      156 2023-04-23 12:50:03.000000 semantra-0.0.9/src/semantra.egg-info/requires.txt
+-rw-r--r--   0 freedmand   (501) staff       (20)        9 2023-04-23 12:50:03.000000 semantra-0.0.9/src/semantra.egg-info/top_level.txt
```

### Comparing `semantra-0.0.8/LICENSE` & `semantra-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `semantra-0.0.8/PKG-INFO` & `semantra-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: semantra
-Version: 0.0.8
+Version: 0.0.9
 Summary: A semantic search CLI tool
-Home-page: https://github.com/freedmand/semantra
-Author: Dylan Freedman
-Author-email: freedmand@gmail.com
+Author-email: Dylan Freedman <freedmand@gmail.com>
+Project-URL: Homepage, https://github.com/freedmand/semantra
+Project-URL: Repository, https://github.com/freedmand/semantra
+Project-URL: Bug Tracker, https://github.com/freedmand/semantra/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
 (Work-in-progress documentation; the tool is not yet ready)
 
 # Semantra
 
 Semantra is a multipurpose tool for semantically searching documents. Query by meaning rather than just by matching text.
```

### Comparing `semantra-0.0.8/README.md` & `semantra-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `semantra-0.0.8/client/public/build/bundle.css` & `semantra-0.0.9/client/public/build/bundle.css`

 * *Files identical despite different names*

### Comparing `semantra-0.0.8/client/public/build/bundle.js` & `semantra-0.0.9/client/public/build/bundle.js`

 * *Files identical despite different names*

### Comparing `semantra-0.0.8/client/public/build/bundle.js.map` & `semantra-0.0.9/client/public/build/bundle.js.map`

 * *Files identical despite different names*

### Comparing `semantra-0.0.8/client/public/favicon.png` & `semantra-0.0.9/client/public/favicon.png`

 * *Files identical despite different names*

### Comparing `semantra-0.0.8/client/public/global.css` & `semantra-0.0.9/client/public/global.css`

 * *Files identical despite different names*

### Comparing `semantra-0.0.8/src/semantra/models.py` & `semantra-0.0.9/src/semantra/models.py`

 * *Files identical despite different names*

### Comparing `semantra-0.0.8/src/semantra/pdf.py` & `semantra-0.0.9/src/semantra/pdf.py`

 * *Files identical despite different names*

### Comparing `semantra-0.0.8/src/semantra/semantra.py` & `semantra-0.0.9/src/semantra/semantra.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,18 +24,15 @@
     write_annoy_db,
     load_annoy_db,
     sort_results,
     HASH_LENGTH,
 )
 import pkg_resources
 
-with open(
-    pkg_resources.resource_filename("semantra.semantra", "../../VERSION"), "r"
-) as f:
-    VERSION = f.read().strip()
+VERSION = pkg_resources.require("semantra")[0].version
 
 package_directory = os.path.dirname(os.path.abspath(__file__))
 
 
 class Content:
     def __init__(self, rawtext, filename):
         self.rawtext = rawtext
@@ -628,23 +625,23 @@
 
     # Start a Flask server
     app = Flask(__name__)
 
     @app.route("/")
     def base():
         return send_from_directory(
-            pkg_resources.resource_filename("semantra.semantra", "../../client/public"),
+            pkg_resources.resource_filename("semantra.semantra", "client_public"),
             "index.html",
         )
 
     # Path for all the static files (compiled JS/CSS, etc.)
     @app.route("/<path:path>")
     def home(path):
         return send_from_directory(
-            pkg_resources.resource_filename("semantra.semantra", "../../client/public"),
+            pkg_resources.resource_filename("semantra.semantra", "client_public"),
             path,
         )
 
     @app.route("/api/files", methods=["GET"])
     def files():
         return jsonify(
             [
```

### Comparing `semantra-0.0.8/src/semantra/util.py` & `semantra-0.0.9/src/semantra/util.py`

 * *Files identical despite different names*

### Comparing `semantra-0.0.8/src/semantra.egg-info/PKG-INFO` & `semantra-0.0.9/src/semantra.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: semantra
-Version: 0.0.8
+Version: 0.0.9
 Summary: A semantic search CLI tool
-Home-page: https://github.com/freedmand/semantra
-Author: Dylan Freedman
-Author-email: freedmand@gmail.com
+Author-email: Dylan Freedman <freedmand@gmail.com>
+Project-URL: Homepage, https://github.com/freedmand/semantra
+Project-URL: Repository, https://github.com/freedmand/semantra
+Project-URL: Bug Tracker, https://github.com/freedmand/semantra/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
 (Work-in-progress documentation; the tool is not yet ready)
 
 # Semantra
 
 Semantra is a multipurpose tool for semantically searching documents. Query by meaning rather than just by matching text.
```

