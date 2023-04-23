# Comparing `tmp/gama_config-1.12.0.tar.gz` & `tmp/gama_config-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gama_config-1.12.0.tar", last modified: Sun Apr 23 04:19:36 2023, max compression
+gzip compressed data, was "gama_config-1.9.0.tar", last modified: Sun Apr 16 23:29:11 2023, max compression
```

## Comparing `gama_config-1.12.0.tar` & `gama_config-1.9.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-23 04:19:36.270599 gama_config-1.12.0/
--rw-rw-r--   0 runner    (1000) runner    (1001)     1529 2023-04-23 04:19:36.270599 gama_config-1.12.0/PKG-INFO
--rw-rw-r--   0 runner    (1000) runner    (1001)      886 2023-04-23 04:18:48.000000 gama_config-1.12.0/README.md
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-23 04:19:36.270599 gama_config-1.12.0/gama_config/
--rw-rw-r--   0 runner    (1000) runner    (1001)        0 2023-04-23 04:18:48.000000 gama_config-1.12.0/gama_config/__init__.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     1657 2023-04-23 04:18:48.000000 gama_config-1.12.0/gama_config/gama_gs.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     2084 2023-04-23 04:18:48.000000 gama_config-1.12.0/gama_config/gama_vessel.py
--rw-rw-r--   0 runner    (1000) runner    (1001)      620 2023-04-23 04:18:48.000000 gama_config-1.12.0/gama_config/generate_schemas.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     1340 2023-04-23 04:18:48.000000 gama_config-1.12.0/gama_config/helpers.py
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-23 04:19:36.270599 gama_config-1.12.0/gama_config/schemas/
--rw-rw-r--   0 runner    (1000) runner    (1001)     1844 2023-04-23 04:18:48.000000 gama_config-1.12.0/gama_config/schemas/gama_gs.schema.json
--rw-rw-r--   0 runner    (1000) runner    (1001)     2990 2023-04-23 04:18:48.000000 gama_config-1.12.0/gama_config/schemas/gama_vessel.schema.json
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-23 04:19:36.270599 gama_config-1.12.0/gama_config.egg-info/
--rw-rw-r--   0 runner    (1000) runner    (1001)     1529 2023-04-23 04:19:36.000000 gama_config-1.12.0/gama_config.egg-info/PKG-INFO
--rw-rw-r--   0 runner    (1000) runner    (1001)      445 2023-04-23 04:19:36.000000 gama_config-1.12.0/gama_config.egg-info/SOURCES.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)        1 2023-04-23 04:19:36.000000 gama_config-1.12.0/gama_config.egg-info/dependency_links.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)       35 2023-04-23 04:19:36.000000 gama_config-1.12.0/gama_config.egg-info/requires.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)       12 2023-04-23 04:19:36.000000 gama_config-1.12.0/gama_config.egg-info/top_level.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)        1 2023-04-23 04:19:22.000000 gama_config-1.12.0/gama_config.egg-info/zip-safe
--rw-rw-r--   0 runner    (1000) runner    (1001)      864 2023-04-23 04:19:36.270599 gama_config-1.12.0/setup.cfg
--rw-rw-r--   0 runner    (1000) runner    (1001)       38 2023-04-23 04:18:48.000000 gama_config-1.12.0/setup.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-16 23:29:11.865756 gama_config-1.9.0/
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1470 2023-04-16 23:29:11.865756 gama_config-1.9.0/PKG-INFO
+-rw-rw-r--   0 runner    (1000) runner    (1001)      828 2023-04-16 23:28:20.000000 gama_config-1.9.0/README.md
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-16 23:29:11.865756 gama_config-1.9.0/gama_config/
+-rw-rw-r--   0 runner    (1000) runner    (1001)        0 2023-04-16 23:28:20.000000 gama_config-1.9.0/gama_config/__init__.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1657 2023-04-16 23:28:20.000000 gama_config-1.9.0/gama_config/gama_gs.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     2084 2023-04-16 23:28:20.000000 gama_config-1.9.0/gama_config/gama_vessel.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)      620 2023-04-16 23:28:20.000000 gama_config-1.9.0/gama_config/generate_schemas.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1340 2023-04-16 23:28:20.000000 gama_config-1.9.0/gama_config/helpers.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-16 23:29:11.865756 gama_config-1.9.0/gama_config/schemas/
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1844 2023-04-16 23:28:20.000000 gama_config-1.9.0/gama_config/schemas/gama_gs.schema.json
+-rw-rw-r--   0 runner    (1000) runner    (1001)     2990 2023-04-16 23:28:20.000000 gama_config-1.9.0/gama_config/schemas/gama_vessel.schema.json
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-16 23:29:11.865756 gama_config-1.9.0/gama_config.egg-info/
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1470 2023-04-16 23:29:11.000000 gama_config-1.9.0/gama_config.egg-info/PKG-INFO
+-rw-rw-r--   0 runner    (1000) runner    (1001)      445 2023-04-16 23:29:11.000000 gama_config-1.9.0/gama_config.egg-info/SOURCES.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)        1 2023-04-16 23:29:11.000000 gama_config-1.9.0/gama_config.egg-info/dependency_links.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)       35 2023-04-16 23:29:11.000000 gama_config-1.9.0/gama_config.egg-info/requires.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)       12 2023-04-16 23:29:11.000000 gama_config-1.9.0/gama_config.egg-info/top_level.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)        1 2023-04-16 23:28:56.000000 gama_config-1.9.0/gama_config.egg-info/zip-safe
+-rw-rw-r--   0 runner    (1000) runner    (1001)      863 2023-04-16 23:29:11.869756 gama_config-1.9.0/setup.cfg
+-rw-rw-r--   0 runner    (1000) runner    (1001)       38 2023-04-16 23:28:20.000000 gama_config-1.9.0/setup.py
```

### Comparing `gama_config-1.12.0/PKG-INFO` & `gama_config-1.9.0/gama_config.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gama_config
-Version: 1.12.0
+Name: gama-config
+Version: 1.9.0
 Summary: A library for reading / writing GAMA config files
 Home-page: https://github.com/Greenroom-Robotics/gama
 Author: Greenroom Robotics
 Author-email: team@greenroomrobotics.com
 Maintainer: David Revay
 Maintainer-email: david.revay@greenroomrobotics.com
 License: Copyright (C) 2023, Greenroom Robotics
@@ -20,15 +20,15 @@
 
 GAMA Config is used to load config stored inside the `.gama` folder.
 
 ## Install
 
 * `pip install -e ./libs/gama_config`
 * or...
-* `pip install gama_config` (Public on [PyPi](https://pypi.org/project/gama-config/))
+* `pip install gama_config`
 
 ## Usage
 
 ### Reading config
 
 ```python
 from gama_config.gama_vessel import read_vessel_config
```

### Comparing `gama_config-1.12.0/gama_config/gama_gs.py` & `gama_config-1.9.0/gama_config/gama_gs.py`

 * *Files identical despite different names*

### Comparing `gama_config-1.12.0/gama_config/gama_vessel.py` & `gama_config-1.9.0/gama_config/gama_vessel.py`

 * *Files identical despite different names*

### Comparing `gama_config-1.12.0/gama_config/generate_schemas.py` & `gama_config-1.9.0/gama_config/generate_schemas.py`

 * *Files identical despite different names*

### Comparing `gama_config-1.12.0/gama_config/helpers.py` & `gama_config-1.9.0/gama_config/helpers.py`

 * *Files identical despite different names*

### Comparing `gama_config-1.12.0/gama_config/schemas/gama_gs.schema.json` & `gama_config-1.9.0/gama_config/schemas/gama_gs.schema.json`

 * *Files identical despite different names*

### Comparing `gama_config-1.12.0/gama_config/schemas/gama_vessel.schema.json` & `gama_config-1.9.0/gama_config/schemas/gama_vessel.schema.json`

 * *Files identical despite different names*

### Comparing `gama_config-1.12.0/gama_config.egg-info/PKG-INFO` & `gama_config-1.9.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gama-config
-Version: 1.12.0
+Name: gama_config
+Version: 1.9.0
 Summary: A library for reading / writing GAMA config files
 Home-page: https://github.com/Greenroom-Robotics/gama
 Author: Greenroom Robotics
 Author-email: team@greenroomrobotics.com
 Maintainer: David Revay
 Maintainer-email: david.revay@greenroomrobotics.com
 License: Copyright (C) 2023, Greenroom Robotics
@@ -20,15 +20,15 @@
 
 GAMA Config is used to load config stored inside the `.gama` folder.
 
 ## Install
 
 * `pip install -e ./libs/gama_config`
 * or...
-* `pip install gama_config` (Public on [PyPi](https://pypi.org/project/gama-config/))
+* `pip install gama_config`
 
 ## Usage
 
 ### Reading config
 
 ```python
 from gama_config.gama_vessel import read_vessel_config
```

### Comparing `gama_config-1.12.0/setup.cfg` & `gama_config-1.9.0/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = gama_config
-version = 1.12.0
+version = 1.9.0
 url = https://github.com/Greenroom-Robotics/gama
 author = Greenroom Robotics
 author_email = team@greenroomrobotics.com
 maintainer = David Revay
 maintainer_email = david.revay@greenroomrobotics.com
 classifiers = 
 	Development Status :: 3 - Alpha
```

