# Comparing `tmp/synthea-rdf-0.1.4.tar.gz` & `tmp/synthea-rdf-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synthea-rdf-0.1.4.tar", last modified: Sun Apr 23 04:06:39 2023, max compression
+gzip compressed data, was "synthea-rdf-0.1.5.tar", last modified: Sun Apr 23 05:55:35 2023, max compression
```

## Comparing `synthea-rdf-0.1.4.tar` & `synthea-rdf-0.1.5.tar`

### file list

```diff
@@ -1,40 +1,43 @@
-drwxrwxr-x   0 k163     (65010) k163      (1049)        0 2023-04-23 04:06:39.130283 synthea-rdf-0.1.4/
--rw-rw-r--   0 k163     (65010) k163      (1049)    35130 2023-03-24 16:59:14.000000 synthea-rdf-0.1.4/LICENSE
--rw-rw-r--   0 k163     (65010) k163      (1049)      100 2023-04-23 04:03:43.000000 synthea-rdf-0.1.4/MANIFEST.in
--rw-rw-r--   0 k163     (65010) k163      (1049)     1990 2023-04-23 04:06:39.130283 synthea-rdf-0.1.4/PKG-INFO
--rw-rw-r--   0 k163     (65010) k163      (1049)     1510 2023-03-24 16:59:14.000000 synthea-rdf-0.1.4/README.md
-drwxrwxr-x   0 k163     (65010) k163      (1049)        0 2023-04-23 04:06:39.130283 synthea-rdf-0.1.4/abstract/
--rw-rw-r--   0 k163     (65010) k163      (1049)       31 2023-04-07 02:02:05.000000 synthea-rdf-0.1.4/abstract/__init__.py
--rw-rw-r--   0 k163     (65010) k163      (1049)     1543 2023-04-10 20:00:28.000000 synthea-rdf-0.1.4/abstract/literal.py
--rw-rw-r--   0 k163     (65010) k163      (1049)      456 2023-04-10 19:53:47.000000 synthea-rdf-0.1.4/abstract/namespace.py
--rw-rw-r--   0 k163     (65010) k163      (1049)      410 2023-04-06 06:27:31.000000 synthea-rdf-0.1.4/abstract/resource.py
--rw-rw-r--   0 k163     (65010) k163      (1049)     2245 2023-04-10 20:40:37.000000 synthea-rdf-0.1.4/abstract/uri.py
-drwxrwxr-x   0 k163     (65010) k163      (1049)        0 2023-04-23 04:06:39.130283 synthea-rdf-0.1.4/dua/
--rw-rw-r--   0 k163     (65010) k163      (1049)        0 2023-04-05 20:11:51.000000 synthea-rdf-0.1.4/dua/__init__.py
--rw-rw-r--   0 k163     (65010) k163      (1049)      683 2023-04-06 19:49:21.000000 synthea-rdf-0.1.4/dua/constants.py
--rw-rw-r--   0 k163     (65010) k163      (1049)     6044 2023-04-23 01:11:11.000000 synthea-rdf-0.1.4/dua/generator.py
--rw-rw-r--   0 k163     (65010) k163      (1049)     4954 2023-04-11 05:20:57.000000 synthea-rdf-0.1.4/dua/resource.py
-drwxrwxr-x   0 k163     (65010) k163      (1049)        0 2023-04-23 04:06:39.130283 synthea-rdf-0.1.4/generator_gui/
--rw-rw-r--   0 k163     (65010) k163      (1049)     3137 2023-04-23 04:00:58.000000 synthea-rdf-0.1.4/generator_gui/dua_generator.py
--rw-rw-r--   0 k163     (65010) k163      (1049)       38 2023-04-23 04:06:39.130283 synthea-rdf-0.1.4/setup.cfg
--rw-rw-r--   0 k163     (65010) k163      (1049)      789 2023-04-23 04:05:05.000000 synthea-rdf-0.1.4/setup.py
-drwxrwxr-x   0 k163     (65010) k163      (1049)        0 2023-04-23 04:06:39.130283 synthea-rdf-0.1.4/synthea_ontology/
--rw-rw-r--   0 k163     (65010) k163      (1049)   565508 2023-03-24 16:59:14.000000 synthea-rdf-0.1.4/synthea_ontology/synthea_ontology.png
--rw-rw-r--   0 k163     (65010) k163      (1049)    71879 2023-03-24 16:59:14.000000 synthea-rdf-0.1.4/synthea_ontology/synthea_ontology.ttl
-drwxrwxr-x   0 k163     (65010) k163      (1049)        0 2023-04-23 04:06:39.130283 synthea-rdf-0.1.4/synthea_rdf/
--rw-rw-r--   0 k163     (65010) k163      (1049)        0 2023-04-05 20:12:52.000000 synthea-rdf-0.1.4/synthea_rdf/__init__.py
--rw-rw-r--   0 k163     (65010) k163      (1049)    13774 2023-04-21 04:57:51.000000 synthea-rdf-0.1.4/synthea_rdf/graph.py
--rw-rw-r--   0 k163     (65010) k163      (1049)    40887 2023-04-22 00:58:58.000000 synthea-rdf-0.1.4/synthea_rdf/resource.py
--rw-rw-r--   0 k163     (65010) k163      (1049)      152 2023-04-10 19:53:56.000000 synthea-rdf-0.1.4/synthea_rdf/settings.py
-drwxrwxr-x   0 k163     (65010) k163      (1049)        0 2023-04-23 04:06:39.130283 synthea-rdf-0.1.4/synthea_rdf.egg-info/
--rw-rw-r--   0 k163     (65010) k163      (1049)     1990 2023-04-23 04:06:39.000000 synthea-rdf-0.1.4/synthea_rdf.egg-info/PKG-INFO
--rw-rw-r--   0 k163     (65010) k163      (1049)      670 2023-04-23 04:06:39.000000 synthea-rdf-0.1.4/synthea_rdf.egg-info/SOURCES.txt
--rw-rw-r--   0 k163     (65010) k163      (1049)        1 2023-04-23 04:06:39.000000 synthea-rdf-0.1.4/synthea_rdf.egg-info/dependency_links.txt
--rw-rw-r--   0 k163     (65010) k163      (1049)       35 2023-04-23 04:06:39.000000 synthea-rdf-0.1.4/synthea_rdf.egg-info/requires.txt
--rw-rw-r--   0 k163     (65010) k163      (1049)       36 2023-04-23 04:06:39.000000 synthea-rdf-0.1.4/synthea_rdf.egg-info/top_level.txt
-drwxrwxr-x   0 k163     (65010) k163      (1049)        0 2023-04-23 04:06:39.130283 synthea-rdf-0.1.4/tests/
--rw-rw-r--   0 k163     (65010) k163      (1049)     3985 2023-03-24 16:59:14.000000 synthea-rdf-0.1.4/tests/test_convert.py
-drwxrwxr-x   0 k163     (65010) k163      (1049)        0 2023-04-23 04:06:39.130283 synthea-rdf-0.1.4/trustscore/
--rw-rw-r--   0 k163     (65010) k163      (1049)        0 2023-04-06 06:09:53.000000 synthea-rdf-0.1.4/trustscore/__init__.py
--rw-rw-r--   0 k163     (65010) k163      (1049)     5535 2023-04-11 01:51:24.000000 synthea-rdf-0.1.4/trustscore/generator.py
--rw-rw-r--   0 k163     (65010) k163      (1049)     2637 2023-04-22 05:22:38.000000 synthea-rdf-0.1.4/trustscore/resource.py
+drwxrwxr-x   0 k163     (65010) k163      (1049)        0 2023-04-23 05:55:35.322016 synthea-rdf-0.1.5/
+-rw-rw-r--   0 k163     (65010) k163      (1049)    35130 2023-03-24 16:59:14.000000 synthea-rdf-0.1.5/LICENSE
+-rw-rw-r--   0 k163     (65010) k163      (1049)      134 2023-04-23 05:53:26.000000 synthea-rdf-0.1.5/MANIFEST.in
+-rw-rw-r--   0 k163     (65010) k163      (1049)     1393 2023-04-23 05:55:35.322016 synthea-rdf-0.1.5/PKG-INFO
+-rw-rw-r--   0 k163     (65010) k163      (1049)      913 2023-04-23 05:46:10.000000 synthea-rdf-0.1.5/README.md
+drwxrwxr-x   0 k163     (65010) k163      (1049)        0 2023-04-23 05:55:35.318016 synthea-rdf-0.1.5/abstract/
+-rw-rw-r--   0 k163     (65010) k163      (1049)       31 2023-04-07 02:02:05.000000 synthea-rdf-0.1.5/abstract/__init__.py
+-rw-rw-r--   0 k163     (65010) k163      (1049)     1543 2023-04-10 20:00:28.000000 synthea-rdf-0.1.5/abstract/literal.py
+-rw-rw-r--   0 k163     (65010) k163      (1049)      456 2023-04-10 19:53:47.000000 synthea-rdf-0.1.5/abstract/namespace.py
+-rw-rw-r--   0 k163     (65010) k163      (1049)      410 2023-04-06 06:27:31.000000 synthea-rdf-0.1.5/abstract/resource.py
+-rw-rw-r--   0 k163     (65010) k163      (1049)     2245 2023-04-10 20:40:37.000000 synthea-rdf-0.1.5/abstract/uri.py
+drwxrwxr-x   0 k163     (65010) k163      (1049)        0 2023-04-23 05:55:35.318016 synthea-rdf-0.1.5/dua/
+-rw-rw-r--   0 k163     (65010) k163      (1049)        0 2023-04-05 20:11:51.000000 synthea-rdf-0.1.5/dua/__init__.py
+-rw-rw-r--   0 k163     (65010) k163      (1049)      683 2023-04-06 19:49:21.000000 synthea-rdf-0.1.5/dua/constants.py
+-rw-rw-r--   0 k163     (65010) k163      (1049)     6044 2023-04-23 01:11:11.000000 synthea-rdf-0.1.5/dua/generator.py
+-rw-rw-r--   0 k163     (65010) k163      (1049)     4954 2023-04-11 05:20:57.000000 synthea-rdf-0.1.5/dua/resource.py
+drwxrwxr-x   0 k163     (65010) k163      (1049)        0 2023-04-23 05:55:35.318016 synthea-rdf-0.1.5/gui/
+-rw-rw-r--   0 k163     (65010) k163      (1049)     3701 2023-04-23 05:33:30.000000 synthea-rdf-0.1.5/gui/synthea_converter.py
+-rw-rw-r--   0 k163     (65010) k163      (1049)     3137 2023-04-23 04:00:58.000000 synthea-rdf-0.1.5/gui/trustscore_dua_generator.py
+-rw-rw-r--   0 k163     (65010) k163      (1049)       38 2023-04-23 05:55:35.322016 synthea-rdf-0.1.5/setup.cfg
+-rw-rw-r--   0 k163     (65010) k163      (1049)      777 2023-04-23 05:54:36.000000 synthea-rdf-0.1.5/setup.py
+drwxrwxr-x   0 k163     (65010) k163      (1049)        0 2023-04-23 05:55:35.318016 synthea-rdf-0.1.5/synthea_ontology/
+-rw-rw-r--   0 k163     (65010) k163      (1049)   400059 2023-04-23 05:37:50.000000 synthea-rdf-0.1.5/synthea_ontology/synthea_converter.png
+-rw-rw-r--   0 k163     (65010) k163      (1049)   565508 2023-03-24 16:59:14.000000 synthea-rdf-0.1.5/synthea_ontology/synthea_ontology.png
+-rw-rw-r--   0 k163     (65010) k163      (1049)    71879 2023-03-24 16:59:14.000000 synthea-rdf-0.1.5/synthea_ontology/synthea_ontology.ttl
+-rw-rw-r--   0 k163     (65010) k163      (1049)   161859 2023-04-23 05:44:10.000000 synthea-rdf-0.1.5/synthea_ontology/trustscore_dua_generator.png
+drwxrwxr-x   0 k163     (65010) k163      (1049)        0 2023-04-23 05:55:35.318016 synthea-rdf-0.1.5/synthea_rdf/
+-rw-rw-r--   0 k163     (65010) k163      (1049)        0 2023-04-05 20:12:52.000000 synthea-rdf-0.1.5/synthea_rdf/__init__.py
+-rw-rw-r--   0 k163     (65010) k163      (1049)    13774 2023-04-21 04:57:51.000000 synthea-rdf-0.1.5/synthea_rdf/graph.py
+-rw-rw-r--   0 k163     (65010) k163      (1049)    40887 2023-04-22 00:58:58.000000 synthea-rdf-0.1.5/synthea_rdf/resource.py
+-rw-rw-r--   0 k163     (65010) k163      (1049)      152 2023-04-10 19:53:56.000000 synthea-rdf-0.1.5/synthea_rdf/settings.py
+drwxrwxr-x   0 k163     (65010) k163      (1049)        0 2023-04-23 05:55:35.318016 synthea-rdf-0.1.5/synthea_rdf.egg-info/
+-rw-rw-r--   0 k163     (65010) k163      (1049)     1393 2023-04-23 05:55:35.000000 synthea-rdf-0.1.5/synthea_rdf.egg-info/PKG-INFO
+-rw-rw-r--   0 k163     (65010) k163      (1049)      781 2023-04-23 05:55:35.000000 synthea-rdf-0.1.5/synthea_rdf.egg-info/SOURCES.txt
+-rw-rw-r--   0 k163     (65010) k163      (1049)        1 2023-04-23 05:55:35.000000 synthea-rdf-0.1.5/synthea_rdf.egg-info/dependency_links.txt
+-rw-rw-r--   0 k163     (65010) k163      (1049)       35 2023-04-23 05:55:35.000000 synthea-rdf-0.1.5/synthea_rdf.egg-info/requires.txt
+-rw-rw-r--   0 k163     (65010) k163      (1049)       36 2023-04-23 05:55:35.000000 synthea-rdf-0.1.5/synthea_rdf.egg-info/top_level.txt
+drwxrwxr-x   0 k163     (65010) k163      (1049)        0 2023-04-23 05:55:35.318016 synthea-rdf-0.1.5/tests/
+-rw-rw-r--   0 k163     (65010) k163      (1049)     3985 2023-03-24 16:59:14.000000 synthea-rdf-0.1.5/tests/test_convert.py
+drwxrwxr-x   0 k163     (65010) k163      (1049)        0 2023-04-23 05:55:35.322016 synthea-rdf-0.1.5/trustscore/
+-rw-rw-r--   0 k163     (65010) k163      (1049)        0 2023-04-06 06:09:53.000000 synthea-rdf-0.1.5/trustscore/__init__.py
+-rw-rw-r--   0 k163     (65010) k163      (1049)     5535 2023-04-11 01:51:24.000000 synthea-rdf-0.1.5/trustscore/generator.py
+-rw-rw-r--   0 k163     (65010) k163      (1049)     2637 2023-04-22 05:22:38.000000 synthea-rdf-0.1.5/trustscore/resource.py
```

### Comparing `synthea-rdf-0.1.4/LICENSE` & `synthea-rdf-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `synthea-rdf-0.1.4/abstract/literal.py` & `synthea-rdf-0.1.5/abstract/literal.py`

 * *Files identical despite different names*

### Comparing `synthea-rdf-0.1.4/abstract/uri.py` & `synthea-rdf-0.1.5/abstract/uri.py`

 * *Files identical despite different names*

### Comparing `synthea-rdf-0.1.4/dua/constants.py` & `synthea-rdf-0.1.5/dua/constants.py`

 * *Files identical despite different names*

### Comparing `synthea-rdf-0.1.4/dua/generator.py` & `synthea-rdf-0.1.5/dua/generator.py`

 * *Files identical despite different names*

### Comparing `synthea-rdf-0.1.4/dua/resource.py` & `synthea-rdf-0.1.5/dua/resource.py`

 * *Files identical despite different names*

### Comparing `synthea-rdf-0.1.4/generator_gui/dua_generator.py` & `synthea-rdf-0.1.5/gui/trustscore_dua_generator.py`

 * *Files identical despite different names*

### Comparing `synthea-rdf-0.1.4/setup.py` & `synthea-rdf-0.1.5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup
 
 setup(
     name="synthea-rdf",
-    version="0.1.4",
+    version="0.1.5",
     description="Semantic web representation for the Synthea.",
     author="Dae-young Kim",
     author_email="leroy.kim@umbc.edu",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     project_urls={"Source Code": "https://github.com/leroykim/synthea-rdf"},
     license="GPLv3",
     packages=["synthea_rdf", "dua", "trustscore", "abstract"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
-    ],  # Optional
+    ],
     install_requires=[
         "rdflib",
         "pandas",
         "alive_progress",
         "panel",
     ],
 )
```

### Comparing `synthea-rdf-0.1.4/synthea_ontology/synthea_ontology.png` & `synthea-rdf-0.1.5/synthea_ontology/synthea_ontology.png`

 * *Files identical despite different names*

### Comparing `synthea-rdf-0.1.4/synthea_ontology/synthea_ontology.ttl` & `synthea-rdf-0.1.5/synthea_ontology/synthea_ontology.ttl`

 * *Files identical despite different names*

### Comparing `synthea-rdf-0.1.4/synthea_rdf/graph.py` & `synthea-rdf-0.1.5/synthea_rdf/graph.py`

 * *Files identical despite different names*

### Comparing `synthea-rdf-0.1.4/synthea_rdf/resource.py` & `synthea-rdf-0.1.5/synthea_rdf/resource.py`

 * *Files identical despite different names*

### Comparing `synthea-rdf-0.1.4/synthea_rdf.egg-info/SOURCES.txt` & `synthea-rdf-0.1.5/synthea_rdf.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -7,17 +7,20 @@
 abstract/namespace.py
 abstract/resource.py
 abstract/uri.py
 dua/__init__.py
 dua/constants.py
 dua/generator.py
 dua/resource.py
-generator_gui/dua_generator.py
+gui/synthea_converter.py
+gui/trustscore_dua_generator.py
+synthea_ontology/synthea_converter.png
 synthea_ontology/synthea_ontology.png
 synthea_ontology/synthea_ontology.ttl
+synthea_ontology/trustscore_dua_generator.png
 synthea_rdf/__init__.py
 synthea_rdf/graph.py
 synthea_rdf/resource.py
 synthea_rdf/settings.py
 synthea_rdf.egg-info/PKG-INFO
 synthea_rdf.egg-info/SOURCES.txt
 synthea_rdf.egg-info/dependency_links.txt
```

### Comparing `synthea-rdf-0.1.4/tests/test_convert.py` & `synthea-rdf-0.1.5/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `synthea-rdf-0.1.4/trustscore/generator.py` & `synthea-rdf-0.1.5/trustscore/generator.py`

 * *Files identical despite different names*

### Comparing `synthea-rdf-0.1.4/trustscore/resource.py` & `synthea-rdf-0.1.5/trustscore/resource.py`

 * *Files identical despite different names*

