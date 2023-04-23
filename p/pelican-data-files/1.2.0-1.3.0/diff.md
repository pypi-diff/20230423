# Comparing `tmp/pelican-data-files-1.2.0.tar.gz` & `tmp/pelican-data-files-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pelican-data-files-1.2.0.tar", last modified: Mon Oct  3 18:05:01 2022, max compression
+gzip compressed data, was "pelican-data-files-1.3.0.tar", last modified: Sun Apr 23 09:25:16 2023, max compression
```

## Comparing `pelican-data-files-1.2.0.tar` & `pelican-data-files-1.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 vhash     (1000) vhash     (1000)        0 2022-10-03 18:05:01.674946 pelican-data-files-1.2.0/
--rw-rw-r--   0 vhash     (1000) vhash     (1000)     1062 2022-10-03 17:40:29.000000 pelican-data-files-1.2.0/LICENSE
--rw-rw-r--   0 vhash     (1000) vhash     (1000)     5648 2022-10-03 18:05:01.674946 pelican-data-files-1.2.0/PKG-INFO
--rw-rw-r--   0 vhash     (1000) vhash     (1000)     3945 2022-10-03 17:40:29.000000 pelican-data-files-1.2.0/README.md
-drwxrwxr-x   0 vhash     (1000) vhash     (1000)        0 2022-10-03 18:05:01.674946 pelican-data-files-1.2.0/pelican/
-drwxrwxr-x   0 vhash     (1000) vhash     (1000)        0 2022-10-03 18:05:01.674946 pelican-data-files-1.2.0/pelican/plugins/
-drwxrwxr-x   0 vhash     (1000) vhash     (1000)        0 2022-10-03 18:05:01.674946 pelican-data-files-1.2.0/pelican/plugins/data_files/
--rw-rw-r--   0 vhash     (1000) vhash     (1000)      401 2022-10-03 17:40:29.000000 pelican-data-files-1.2.0/pelican/plugins/data_files/__init__.py
--rw-rw-r--   0 vhash     (1000) vhash     (1000)     2440 2022-10-03 17:40:29.000000 pelican-data-files-1.2.0/pelican/plugins/data_files/generator.py
--rw-rw-r--   0 vhash     (1000) vhash     (1000)     2226 2022-10-03 17:40:29.000000 pelican-data-files-1.2.0/pelican/plugins/data_files/parser.py
-drwxrwxr-x   0 vhash     (1000) vhash     (1000)        0 2022-10-03 18:05:01.674946 pelican-data-files-1.2.0/pelican/plugins/data_files/tools/
--rw-rw-r--   0 vhash     (1000) vhash     (1000)        0 2022-10-03 17:40:29.000000 pelican-data-files-1.2.0/pelican/plugins/data_files/tools/__init__.py
--rw-rw-r--   0 vhash     (1000) vhash     (1000)     2762 2022-10-03 17:40:29.000000 pelican-data-files-1.2.0/pelican/plugins/data_files/tools/cli.py
-drwxrwxr-x   0 vhash     (1000) vhash     (1000)        0 2022-10-03 18:05:01.674946 pelican-data-files-1.2.0/pelican_data_files.egg-info/
--rw-rw-r--   0 vhash     (1000) vhash     (1000)     5648 2022-10-03 18:05:01.000000 pelican-data-files-1.2.0/pelican_data_files.egg-info/PKG-INFO
--rw-rw-r--   0 vhash     (1000) vhash     (1000)      528 2022-10-03 18:05:01.000000 pelican-data-files-1.2.0/pelican_data_files.egg-info/SOURCES.txt
--rw-rw-r--   0 vhash     (1000) vhash     (1000)        1 2022-10-03 18:05:01.000000 pelican-data-files-1.2.0/pelican_data_files.egg-info/dependency_links.txt
--rw-rw-r--   0 vhash     (1000) vhash     (1000)       82 2022-10-03 18:05:01.000000 pelican-data-files-1.2.0/pelican_data_files.egg-info/entry_points.txt
--rw-rw-r--   0 vhash     (1000) vhash     (1000)      132 2022-10-03 18:05:01.000000 pelican-data-files-1.2.0/pelican_data_files.egg-info/requires.txt
--rw-rw-r--   0 vhash     (1000) vhash     (1000)        8 2022-10-03 18:05:01.000000 pelican-data-files-1.2.0/pelican_data_files.egg-info/top_level.txt
--rw-rw-r--   0 vhash     (1000) vhash     (1000)        1 2022-10-03 17:50:25.000000 pelican-data-files-1.2.0/pelican_data_files.egg-info/zip-safe
--rw-rw-r--   0 vhash     (1000) vhash     (1000)     1205 2022-10-03 18:05:01.674946 pelican-data-files-1.2.0/setup.cfg
--rw-rw-r--   0 vhash     (1000) vhash     (1000)       38 2022-10-03 17:40:29.000000 pelican-data-files-1.2.0/setup.py
+drwxrwxr-x   0 vhash     (1000) vhash     (1000)        0 2023-04-23 09:25:16.955264 pelican-data-files-1.3.0/
+-rw-rw-r--   0 vhash     (1000) vhash     (1000)     1062 2023-04-23 09:08:39.000000 pelican-data-files-1.3.0/LICENSE
+-rw-rw-r--   0 vhash     (1000) vhash     (1000)     5648 2023-04-23 09:25:16.955264 pelican-data-files-1.3.0/PKG-INFO
+-rw-rw-r--   0 vhash     (1000) vhash     (1000)     3945 2023-04-23 09:08:39.000000 pelican-data-files-1.3.0/README.md
+drwxrwxr-x   0 vhash     (1000) vhash     (1000)        0 2023-04-23 09:25:16.955264 pelican-data-files-1.3.0/pelican/
+drwxrwxr-x   0 vhash     (1000) vhash     (1000)        0 2023-04-23 09:25:16.955264 pelican-data-files-1.3.0/pelican/plugins/
+drwxrwxr-x   0 vhash     (1000) vhash     (1000)        0 2023-04-23 09:25:16.955264 pelican-data-files-1.3.0/pelican/plugins/data_files/
+-rw-rw-r--   0 vhash     (1000) vhash     (1000)      401 2023-04-23 09:08:39.000000 pelican-data-files-1.3.0/pelican/plugins/data_files/__init__.py
+-rw-rw-r--   0 vhash     (1000) vhash     (1000)     2680 2023-04-23 09:17:25.000000 pelican-data-files-1.3.0/pelican/plugins/data_files/generator.py
+-rw-rw-r--   0 vhash     (1000) vhash     (1000)     2226 2023-04-23 09:08:39.000000 pelican-data-files-1.3.0/pelican/plugins/data_files/parser.py
+drwxrwxr-x   0 vhash     (1000) vhash     (1000)        0 2023-04-23 09:25:16.955264 pelican-data-files-1.3.0/pelican/plugins/data_files/tools/
+-rw-rw-r--   0 vhash     (1000) vhash     (1000)        0 2023-04-23 09:08:39.000000 pelican-data-files-1.3.0/pelican/plugins/data_files/tools/__init__.py
+-rw-rw-r--   0 vhash     (1000) vhash     (1000)     2762 2023-04-23 09:08:39.000000 pelican-data-files-1.3.0/pelican/plugins/data_files/tools/cli.py
+drwxrwxr-x   0 vhash     (1000) vhash     (1000)        0 2023-04-23 09:25:16.955264 pelican-data-files-1.3.0/pelican_data_files.egg-info/
+-rw-rw-r--   0 vhash     (1000) vhash     (1000)     5648 2023-04-23 09:25:16.000000 pelican-data-files-1.3.0/pelican_data_files.egg-info/PKG-INFO
+-rw-rw-r--   0 vhash     (1000) vhash     (1000)      528 2023-04-23 09:25:16.000000 pelican-data-files-1.3.0/pelican_data_files.egg-info/SOURCES.txt
+-rw-rw-r--   0 vhash     (1000) vhash     (1000)        1 2023-04-23 09:25:16.000000 pelican-data-files-1.3.0/pelican_data_files.egg-info/dependency_links.txt
+-rw-rw-r--   0 vhash     (1000) vhash     (1000)       82 2023-04-23 09:25:16.000000 pelican-data-files-1.3.0/pelican_data_files.egg-info/entry_points.txt
+-rw-rw-r--   0 vhash     (1000) vhash     (1000)      132 2023-04-23 09:25:16.000000 pelican-data-files-1.3.0/pelican_data_files.egg-info/requires.txt
+-rw-rw-r--   0 vhash     (1000) vhash     (1000)        8 2023-04-23 09:25:16.000000 pelican-data-files-1.3.0/pelican_data_files.egg-info/top_level.txt
+-rw-rw-r--   0 vhash     (1000) vhash     (1000)        1 2023-04-23 09:10:03.000000 pelican-data-files-1.3.0/pelican_data_files.egg-info/zip-safe
+-rw-rw-r--   0 vhash     (1000) vhash     (1000)     1205 2023-04-23 09:25:16.955264 pelican-data-files-1.3.0/setup.cfg
+-rw-rw-r--   0 vhash     (1000) vhash     (1000)       38 2023-04-23 09:08:39.000000 pelican-data-files-1.3.0/setup.py
```

### Comparing `pelican-data-files-1.2.0/LICENSE` & `pelican-data-files-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pelican-data-files-1.2.0/PKG-INFO` & `pelican-data-files-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pelican-data-files
-Version: 1.2.0
+Version: 1.3.0
 Summary: Pelican plugin that allows to load data from files like JSON or YAML.
 Home-page: https://github.com/LucasVanHaaren/pelican-data-files
 Author: vhash
 Author-email: vanhaaren.lucas+dev@gmail.com
 License: MIT
 Keywords: pelican,pelican-plugin,data
 Platform: UNKNOWN
```

### Comparing `pelican-data-files-1.2.0/README.md` & `pelican-data-files-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pelican-data-files-1.2.0/pelican/plugins/data_files/generator.py` & `pelican-data-files-1.3.0/pelican/plugins/data_files/generator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import sys
 import os
+import re
 import logging
 import pathlib
 
 from pelican.generators import Generator
 
 from .parser import DataParser
 
@@ -61,39 +62,45 @@
             log.error("pelican-data-files: DATA_FILES_DIR path isn't a directory.")
             sys.exit(1)
 
         # Initialize parser object
         obj = DataParser()
 
         # Sort files by modified time
-        files = sorted(data_dir.iterdir(), key=os.path.getmtime, reverse=True)
+        files = sorted(data_dir.rglob("*"), key=os.path.getmtime, reverse=True)
 
         # Create data array
         buffer = []
 
         for file in files:
+            # Check whether file is a directory
+            if file.is_dir():
+                # Move on to next file
+                continue
+
             # Skip duplicate files
-            if file.stem in buffer:
+            if file.with_suffix("") in buffer:
                 continue
 
             # Load data from file
             data = obj.load(file)
 
             # Check whether file (type) is supported
             if data is None:
                 # Report back
-                log.info(f"{file.name} wasn't loaded.")
+                log.info(f"{file} wasn't loaded.")
 
                 # Move on to next file
                 continue
 
             # Determine context variable
-            name = file.stem.replace(".", "_").upper()
+            name = str(file.relative_to(data_dir).with_suffix(""))
+            name = re.sub("[^0-9a-zA-Z]+", "_", name).upper()
 
             # Add data to context
             self.context[f"DATA_{name}"] = data
 
             # Remember filename
-            buffer.append(file.stem)
+            buffer.append(file.with_suffix(""))
 
             # Report back
-            log.info(f"{file.name} was loaded.")
+            log.info(f"{file} was loaded.")
```

### Comparing `pelican-data-files-1.2.0/pelican/plugins/data_files/parser.py` & `pelican-data-files-1.3.0/pelican/plugins/data_files/parser.py`

 * *Files identical despite different names*

### Comparing `pelican-data-files-1.2.0/pelican/plugins/data_files/tools/cli.py` & `pelican-data-files-1.3.0/pelican/plugins/data_files/tools/cli.py`

 * *Files identical despite different names*

### Comparing `pelican-data-files-1.2.0/pelican_data_files.egg-info/PKG-INFO` & `pelican-data-files-1.3.0/pelican_data_files.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pelican-data-files
-Version: 1.2.0
+Version: 1.3.0
 Summary: Pelican plugin that allows to load data from files like JSON or YAML.
 Home-page: https://github.com/LucasVanHaaren/pelican-data-files
 Author: vhash
 Author-email: vanhaaren.lucas+dev@gmail.com
 License: MIT
 Keywords: pelican,pelican-plugin,data
 Platform: UNKNOWN
```

### Comparing `pelican-data-files-1.2.0/pelican_data_files.egg-info/SOURCES.txt` & `pelican-data-files-1.3.0/pelican_data_files.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pelican-data-files-1.2.0/setup.cfg` & `pelican-data-files-1.3.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pelican-data-files
-version = 1.2.0
+version = 1.3.0
 url = https://github.com/LucasVanHaaren/pelican-data-files
 author = vhash
 author_email = vanhaaren.lucas+dev@gmail.com
 license = MIT
 license_files = LICENSE
 description = Pelican plugin that allows to load data from files like JSON or YAML.
 long_description = file: README.md, LICENSE
```

