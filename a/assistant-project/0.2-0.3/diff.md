# Comparing `tmp/assistant_project-0.2.tar.gz` & `tmp/assistant_project-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assistant_project-0.2.tar", last modified: Sat Apr  1 17:45:34 2023, max compression
+gzip compressed data, was "assistant_project-0.3.tar", last modified: Sun Apr 23 10:22:24 2023, max compression
```

## Comparing `assistant_project-0.2.tar` & `assistant_project-0.3.tar`

### file list

```diff
@@ -1,27 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-04-01 17:45:34.214121 assistant_project-0.2/
--rw-rw-rw-   0        0        0     1091 2023-03-10 10:20:05.000000 assistant_project-0.2/LICENCE
--rw-rw-rw-   0        0        0     2742 2023-04-01 17:45:34.213101 assistant_project-0.2/PKG-INFO
--rw-rw-rw-   0        0        0      961 2023-04-01 16:54:09.000000 assistant_project-0.2/README.md
--rw-rw-rw-   0        0        0      723 2023-04-01 17:44:12.000000 assistant_project-0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-01 17:45:34.214121 assistant_project-0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-01 17:45:34.151710 assistant_project-0.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-01 17:45:34.165097 assistant_project-0.2/src/assistant_project/
--rw-rw-rw-   0        0        0        0 2023-03-10 10:20:05.000000 assistant_project-0.2/src/assistant_project/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-01 17:45:34.186029 assistant_project-0.2/src/assistant_project/graphdb/
--rw-rw-rw-   0        0        0       68 2023-03-10 10:20:05.000000 assistant_project-0.2/src/assistant_project/graphdb/__init__.py
--rw-rw-rw-   0        0        0     2553 2023-03-10 10:20:05.000000 assistant_project-0.2/src/assistant_project/graphdb/graph_db.py
--rw-rw-rw-   0        0        0     4408 2023-03-10 10:20:05.000000 assistant_project-0.2/src/assistant_project/graphdb/onto_refine.py
--rw-rw-rw-   0        0        0     1066 2023-03-10 10:20:05.000000 assistant_project-0.2/src/assistant_project/graphdb/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-01 17:45:34.210868 assistant_project-0.2/src/assistant_project/production_system/
--rw-rw-rw-   0        0        0       86 2023-03-10 10:20:05.000000 assistant_project-0.2/src/assistant_project/production_system/__init__.py
--rw-rw-rw-   0        0        0       29 2023-03-10 10:20:05.000000 assistant_project-0.2/src/assistant_project/production_system/file_reader.py
--rw-rw-rw-   0        0        0      776 2023-03-10 10:20:05.000000 assistant_project-0.2/src/assistant_project/production_system/opg_list.py
--rw-rw-rw-   0        0        0        0 2023-03-10 10:20:05.000000 assistant_project-0.2/src/assistant_project/production_system/osg_list.py
--rw-rw-rw-   0        0        0      512 2023-03-10 10:20:05.000000 assistant_project-0.2/src/assistant_project/production_system/production_system.py
--rw-rw-rw-   0        0        0      800 2023-03-10 10:20:05.000000 assistant_project-0.2/src/assistant_project/production_system/resource_list.py
--rw-rw-rw-   0        0        0      137 2023-03-10 10:20:05.000000 assistant_project-0.2/src/assistant_project/production_system/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-01 17:45:34.178917 assistant_project-0.2/src/assistant_project.egg-info/
--rw-rw-rw-   0        0        0     2742 2023-04-01 17:45:34.000000 assistant_project-0.2/src/assistant_project.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      792 2023-04-01 17:45:34.000000 assistant_project-0.2/src/assistant_project.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-01 17:45:34.000000 assistant_project-0.2/src/assistant_project.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-04-01 17:45:34.000000 assistant_project-0.2/src/assistant_project.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 10:22:24.115180 assistant_project-0.3/
+-rw-rw-rw-   0        0        0     1091 2023-03-10 10:20:05.000000 assistant_project-0.3/LICENCE
+-rw-rw-rw-   0        0        0     2938 2023-04-23 10:22:24.112505 assistant_project-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1157 2023-04-23 10:00:37.000000 assistant_project-0.3/README.md
+-rw-rw-rw-   0        0        0      723 2023-04-23 10:00:45.000000 assistant_project-0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-23 10:22:24.116426 assistant_project-0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-23 10:22:24.025547 assistant_project-0.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-23 10:22:24.041573 assistant_project-0.3/src/assistant_project/
+-rw-rw-rw-   0        0        0        0 2023-03-10 10:20:05.000000 assistant_project-0.3/src/assistant_project/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 10:22:24.063297 assistant_project-0.3/src/assistant_project/dict_wrapper/
+-rw-rw-rw-   0        0        0        0 2023-04-01 17:48:54.000000 assistant_project-0.3/src/assistant_project/dict_wrapper/__init__.py
+-rw-rw-rw-   0        0        0     1892 2023-04-23 10:00:37.000000 assistant_project-0.3/src/assistant_project/dict_wrapper/dict_wrapper.py
+-rw-rw-rw-   0        0        0      262 2023-04-23 08:12:23.000000 assistant_project-0.3/src/assistant_project/dict_wrapper/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-23 10:22:24.078796 assistant_project-0.3/src/assistant_project/graphdb/
+-rw-rw-rw-   0        0        0       68 2023-03-10 10:20:05.000000 assistant_project-0.3/src/assistant_project/graphdb/__init__.py
+-rw-rw-rw-   0        0        0     2553 2023-03-10 10:20:05.000000 assistant_project-0.3/src/assistant_project/graphdb/graph_db.py
+-rw-rw-rw-   0        0        0     4408 2023-03-10 10:20:05.000000 assistant_project-0.3/src/assistant_project/graphdb/onto_refine.py
+-rw-rw-rw-   0        0        0     1066 2023-03-10 10:20:05.000000 assistant_project-0.3/src/assistant_project/graphdb/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-23 10:22:24.109894 assistant_project-0.3/src/assistant_project/production_system/
+-rw-rw-rw-   0        0        0       86 2023-03-10 10:20:05.000000 assistant_project-0.3/src/assistant_project/production_system/__init__.py
+-rw-rw-rw-   0        0        0       29 2023-03-10 10:20:05.000000 assistant_project-0.3/src/assistant_project/production_system/file_reader.py
+-rw-rw-rw-   0        0        0      776 2023-03-10 10:20:05.000000 assistant_project-0.3/src/assistant_project/production_system/opg_list.py
+-rw-rw-rw-   0        0        0        0 2023-03-10 10:20:05.000000 assistant_project-0.3/src/assistant_project/production_system/osg_list.py
+-rw-rw-rw-   0        0        0      512 2023-03-10 10:20:05.000000 assistant_project-0.3/src/assistant_project/production_system/production_system.py
+-rw-rw-rw-   0        0        0      800 2023-03-10 10:20:05.000000 assistant_project-0.3/src/assistant_project/production_system/resource_list.py
+-rw-rw-rw-   0        0        0      137 2023-03-10 10:20:05.000000 assistant_project-0.3/src/assistant_project/production_system/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-23 10:22:24.055262 assistant_project-0.3/src/assistant_project.egg-info/
+-rw-rw-rw-   0        0        0     2938 2023-04-23 10:22:23.000000 assistant_project-0.3/src/assistant_project.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      934 2023-04-23 10:22:24.000000 assistant_project-0.3/src/assistant_project.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 10:22:23.000000 assistant_project-0.3/src/assistant_project.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-04-23 10:22:23.000000 assistant_project-0.3/src/assistant_project.egg-info/top_level.txt
```

### Comparing `assistant_project-0.2/LICENCE` & `assistant_project-0.3/LICENCE`

 * *Files identical despite different names*

### Comparing `assistant_project-0.2/PKG-INFO` & `assistant_project-0.3/src/assistant_project.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: assistant_project
-Version: 0.2
+Name: assistant-project
+Version: 0.3
 Summary: Python Library for the EU ASSISTANT-Project
 Author-email: Nikolas Laudenbach <nikolas.laudenbach@tum.de>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -34,14 +34,15 @@
 # Python Library for the EU ASSISTANT Project
 
 ## Library Description
 
 This library contains the following sublibraries:
 1. [**graphdb**](#graphdb)
 2. [**production_system**](#production-system)
+3. [**dict_wrapper**](#dict-wrapper)
 
 ### GraphDB
 Enables using the Rest API for 
 [OntoText GraphDB](https://www.ontotext.com/products/graphdb/) 
 to Up-/Download files to
 and from the selected graph inside a repository. 
 
@@ -49,17 +50,25 @@
 
 
 ### Production System
 
 Enables reading ProductionSystem file from GraphDB and turning it into valid json format.
 
 
+### Dict Wrapper
+
+Allows to read every key-value pair and return list/dict based on custom config.
+
 ---
 ## Change History
 
+**0.3**:
+- Create new sublibrary *json_wrapper*
+
+
 **0.2**:
 - Create new sublibrary *production_system*
 - Remove prints from *graphdb*
 
 **0.1.1**:
 - Update graphdb download
```

### Comparing `assistant_project-0.2/README.md` & `assistant_project-0.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Python Library for the EU ASSISTANT Project
 
 ## Library Description
 
 This library contains the following sublibraries:
 1. [**graphdb**](#graphdb)
 2. [**production_system**](#production-system)
+3. [**dict_wrapper**](#dict-wrapper)
 
 ### GraphDB
 Enables using the Rest API for 
 [OntoText GraphDB](https://www.ontotext.com/products/graphdb/) 
 to Up-/Download files to
 and from the selected graph inside a repository. 
 
@@ -16,17 +17,25 @@
 
 
 ### Production System
 
 Enables reading ProductionSystem file from GraphDB and turning it into valid json format.
 
 
+### Dict Wrapper
+
+Allows to read every key-value pair and return list/dict based on custom config.
+
 ---
 ## Change History
 
+**0.3**:
+- Create new sublibrary *json_wrapper*
+
+
 **0.2**:
 - Create new sublibrary *production_system*
 - Remove prints from *graphdb*
 
 **0.1.1**:
 - Update graphdb download
```

### Comparing `assistant_project-0.2/pyproject.toml` & `assistant_project-0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "requests~=2.28"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "assistant_project"
-version = "0.2"
+version = "0.3"
 authors = [
   { name="Nikolas Laudenbach", email="nikolas.laudenbach@tum.de" },
 ]
 description = "Python Library for the EU ASSISTANT-Project"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENCE"}
```

### Comparing `assistant_project-0.2/src/assistant_project/graphdb/graph_db.py` & `assistant_project-0.3/src/assistant_project/graphdb/graph_db.py`

 * *Files identical despite different names*

### Comparing `assistant_project-0.2/src/assistant_project/graphdb/onto_refine.py` & `assistant_project-0.3/src/assistant_project/graphdb/onto_refine.py`

 * *Files identical despite different names*

### Comparing `assistant_project-0.2/src/assistant_project/graphdb/utils.py` & `assistant_project-0.3/src/assistant_project/graphdb/utils.py`

 * *Files identical despite different names*

### Comparing `assistant_project-0.2/src/assistant_project/production_system/opg_list.py` & `assistant_project-0.3/src/assistant_project/production_system/opg_list.py`

 * *Files identical despite different names*

### Comparing `assistant_project-0.2/src/assistant_project/production_system/production_system.py` & `assistant_project-0.3/src/assistant_project/production_system/production_system.py`

 * *Files identical despite different names*

### Comparing `assistant_project-0.2/src/assistant_project/production_system/resource_list.py` & `assistant_project-0.3/src/assistant_project/production_system/resource_list.py`

 * *Files identical despite different names*

### Comparing `assistant_project-0.2/src/assistant_project.egg-info/PKG-INFO` & `assistant_project-0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: assistant-project
-Version: 0.2
+Name: assistant_project
+Version: 0.3
 Summary: Python Library for the EU ASSISTANT-Project
 Author-email: Nikolas Laudenbach <nikolas.laudenbach@tum.de>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -34,14 +34,15 @@
 # Python Library for the EU ASSISTANT Project
 
 ## Library Description
 
 This library contains the following sublibraries:
 1. [**graphdb**](#graphdb)
 2. [**production_system**](#production-system)
+3. [**dict_wrapper**](#dict-wrapper)
 
 ### GraphDB
 Enables using the Rest API for 
 [OntoText GraphDB](https://www.ontotext.com/products/graphdb/) 
 to Up-/Download files to
 and from the selected graph inside a repository. 
 
@@ -49,17 +50,25 @@
 
 
 ### Production System
 
 Enables reading ProductionSystem file from GraphDB and turning it into valid json format.
 
 
+### Dict Wrapper
+
+Allows to read every key-value pair and return list/dict based on custom config.
+
 ---
 ## Change History
 
+**0.3**:
+- Create new sublibrary *json_wrapper*
+
+
 **0.2**:
 - Create new sublibrary *production_system*
 - Remove prints from *graphdb*
 
 **0.1.1**:
 - Update graphdb download
```

### Comparing `assistant_project-0.2/src/assistant_project.egg-info/SOURCES.txt` & `assistant_project-0.3/src/assistant_project.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 README.md
 pyproject.toml
 src/assistant_project/__init__.py
 src/assistant_project.egg-info/PKG-INFO
 src/assistant_project.egg-info/SOURCES.txt
 src/assistant_project.egg-info/dependency_links.txt
 src/assistant_project.egg-info/top_level.txt
+src/assistant_project/dict_wrapper/__init__.py
+src/assistant_project/dict_wrapper/dict_wrapper.py
+src/assistant_project/dict_wrapper/utils.py
 src/assistant_project/graphdb/__init__.py
 src/assistant_project/graphdb/graph_db.py
 src/assistant_project/graphdb/onto_refine.py
 src/assistant_project/graphdb/utils.py
 src/assistant_project/production_system/__init__.py
 src/assistant_project/production_system/file_reader.py
 src/assistant_project/production_system/opg_list.py
```

