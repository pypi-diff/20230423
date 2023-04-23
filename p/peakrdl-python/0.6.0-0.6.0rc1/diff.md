# Comparing `tmp/peakrdl-python-0.6.0.tar.gz` & `tmp/peakrdl-python-0.6.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peakrdl-python-0.6.0.tar", last modified: Sun Apr 23 18:48:31 2023, max compression
+gzip compressed data, was "peakrdl-python-0.6.0rc1.tar", last modified: Sun Apr 16 18:46:48 2023, max compression
```

## Comparing `peakrdl-python-0.6.0.tar` & `peakrdl-python-0.6.0rc1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:48:31.176963 peakrdl-python-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-23 18:48:30.000000 peakrdl-python-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-23 18:48:30.000000 peakrdl-python-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-23 18:48:31.176963 peakrdl-python-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-23 18:48:30.000000 peakrdl-python-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 18:48:31.176963 peakrdl-python-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-04-23 18:48:30.000000 peakrdl-python-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:48:31.168963 peakrdl-python-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:48:31.172963 peakrdl-python-0.6.0/src/peakrdl_python/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-23 18:48:30.000000 peakrdl-python-0.6.0/src/peakrdl_python/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-23 18:48:30.000000 peakrdl-python-0.6.0/src/peakrdl_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-23 18:48:30.000000 peakrdl-python-0.6.0/src/peakrdl_python/__peakrdl__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-04-23 18:48:30.000000 peakrdl-python-0.6.0/src/peakrdl_python/_node_walkers.py
--rw-r--r--   0 runner    (1001) docker     (123)    17790 2023-04-23 18:48:30.000000 peakrdl-python-0.6.0/src/peakrdl_python/exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:48:31.172963 peakrdl-python-0.6.0/src/peakrdl_python/lib/
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-23 18:48:30.000000 peakrdl-python-0.6.0/src/peakrdl_python/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-04-23 18:48:30.000000 peakrdl-python-0.6.0/src/peakrdl_python/lib/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-04-23 18:48:30.000000 peakrdl-python-0.6.0/src/peakrdl_python/lib/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    27632 2023-04-23 18:48:30.000000 peakrdl-python-0.6.0/src/peakrdl_python/lib/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    27934 2023-04-23 18:48:30.000000 peakrdl-python-0.6.0/src/peakrdl_python/lib/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)    31302 2023-04-23 18:48:30.000000 peakrdl-python-0.6.0/src/peakrdl_python/lib/register.py
--rw-r--r--   0 runner    (1001) docker     (123)     7819 2023-04-23 18:48:30.000000 peakrdl-python-0.6.0/src/peakrdl_python/peakpython.py
--rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-04-23 18:48:30.000000 peakrdl-python-0.6.0/src/peakrdl_python/safe_name_utility.py
--rw-r--r--   0 runner    (1001) docker     (123)    10197 2023-04-23 18:48:30.000000 peakrdl-python-0.6.0/src/peakrdl_python/systemrdl_node_utility_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:48:31.176963 peakrdl-python-0.6.0/src/peakrdl_python/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-23 18:48:30.000000 peakrdl-python-0.6.0/src/peakrdl_python/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21835 2023-04-23 18:48:30.000000 peakrdl-python-0.6.0/src/peakrdl_python/templates/addrmap.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-04-23 18:48:30.000000 peakrdl-python-0.6.0/src/peakrdl_python/templates/addrmap_field.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-04-23 18:48:30.000000 peakrdl-python-0.6.0/src/peakrdl_python/templates/addrmap_memory.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)    10725 2023-04-23 18:48:30.000000 peakrdl-python-0.6.0/src/peakrdl_python/templates/addrmap_register.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 18:48:30.000000 peakrdl-python-0.6.0/src/peakrdl_python/templates/addrmap_simulation.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 18:48:30.000000 peakrdl-python-0.6.0/src/peakrdl_python/templates/addrmap_simulation_tb.jinja
--rw-r--r--   0 runner    (1001) docker     (123)    72721 2023-04-23 18:48:30.000000 peakrdl-python-0.6.0/src/peakrdl_python/templates/addrmap_tb.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-04-23 18:48:30.000000 peakrdl-python-0.6.0/src/peakrdl_python/templates/baseclass_tb.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-23 18:48:30.000000 peakrdl-python-0.6.0/src/peakrdl_python/templates/header.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-23 18:48:30.000000 peakrdl-python-0.6.0/src/peakrdl_python/templates/header_tb.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-04-23 18:48:30.000000 peakrdl-python-0.6.0/src/peakrdl_python/templates/reg_definitions.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:48:31.172963 peakrdl-python-0.6.0/src/peakrdl_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-23 18:48:31.000000 peakrdl-python-0.6.0/src/peakrdl_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-23 18:48:31.000000 peakrdl-python-0.6.0/src/peakrdl_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 18:48:31.000000 peakrdl-python-0.6.0/src/peakrdl_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-23 18:48:31.000000 peakrdl-python-0.6.0/src/peakrdl_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-23 18:48:31.000000 peakrdl-python-0.6.0/src/peakrdl_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-23 18:48:31.000000 peakrdl-python-0.6.0/src/peakrdl_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:46:48.203227 peakrdl-python-0.6.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-16 18:46:48.203227 peakrdl-python-0.6.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 18:46:48.203227 peakrdl-python-0.6.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:46:48.199227 peakrdl-python-0.6.0rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:46:48.199227 peakrdl-python-0.6.0rc1/src/peakrdl_python/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/__peakrdl__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/_node_walkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17790 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:46:48.199227 peakrdl-python-0.6.0rc1/src/peakrdl_python/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/lib/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/lib/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27632 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/lib/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27934 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/lib/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31302 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/lib/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7819 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/peakpython.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/safe_name_utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10197 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/systemrdl_node_utility_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:46:48.203227 peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21835 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/addrmap.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/addrmap_field.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/addrmap_memory.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)    10725 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/addrmap_register.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/addrmap_simulation.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/addrmap_simulation_tb.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)    72721 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/addrmap_tb.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/baseclass_tb.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/header.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/header_tb.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/reg_definitions.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:46:48.199227 peakrdl-python-0.6.0rc1/src/peakrdl_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-16 18:46:48.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-16 18:46:48.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 18:46:48.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-16 18:46:48.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-16 18:46:48.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-16 18:46:48.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python.egg-info/top_level.txt
```

### Comparing `peakrdl-python-0.6.0/LICENSE` & `peakrdl-python-0.6.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.0/PKG-INFO` & `peakrdl-python-0.6.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peakrdl-python
-Version: 0.6.0
+Version: 0.6.0rc1
 Summary: Generate python wrapper for a register model compiled SystemRDL input
 Home-page: https://github.com/krcb197/PeakRDL-python
 Author: Keith Brady
 License: UNKNOWN
 Project-URL: Source, https://github.com/krcb197/PeakRDL-python
 Project-URL: Tracker, https://github.com/krcb197/PeakRDL-python/issues
 Project-URL: Documentation, https://peakrdl-python.readthedocs.io/
```

### Comparing `peakrdl-python-0.6.0/setup.py` & `peakrdl-python-0.6.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.0/src/peakrdl_python/__peakrdl__.py` & `peakrdl-python-0.6.0rc1/src/peakrdl_python/__peakrdl__.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.0/src/peakrdl_python/_node_walkers.py` & `peakrdl-python-0.6.0rc1/src/peakrdl_python/_node_walkers.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.0/src/peakrdl_python/exporter.py` & `peakrdl-python-0.6.0rc1/src/peakrdl_python/exporter.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.0/src/peakrdl_python/lib/__init__.py` & `peakrdl-python-0.6.0rc1/src/peakrdl_python/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.0/src/peakrdl_python/lib/base.py` & `peakrdl-python-0.6.0rc1/src/peakrdl_python/lib/base.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.0/src/peakrdl_python/lib/callbacks.py` & `peakrdl-python-0.6.0rc1/src/peakrdl_python/lib/callbacks.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.0/src/peakrdl_python/lib/fields.py` & `peakrdl-python-0.6.0rc1/src/peakrdl_python/lib/fields.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.0/src/peakrdl_python/lib/memory.py` & `peakrdl-python-0.6.0rc1/src/peakrdl_python/lib/memory.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.0/src/peakrdl_python/lib/register.py` & `peakrdl-python-0.6.0rc1/src/peakrdl_python/lib/register.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.0/src/peakrdl_python/peakpython.py` & `peakrdl-python-0.6.0rc1/src/peakrdl_python/peakpython.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.0/src/peakrdl_python/safe_name_utility.py` & `peakrdl-python-0.6.0rc1/src/peakrdl_python/safe_name_utility.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.0/src/peakrdl_python/systemrdl_node_utility_functions.py` & `peakrdl-python-0.6.0rc1/src/peakrdl_python/systemrdl_node_utility_functions.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.0/src/peakrdl_python/templates/addrmap.py.jinja` & `peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/addrmap.py.jinja`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.0/src/peakrdl_python/templates/addrmap_field.py.jinja` & `peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/addrmap_field.py.jinja`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.0/src/peakrdl_python/templates/addrmap_memory.py.jinja` & `peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/addrmap_memory.py.jinja`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.0/src/peakrdl_python/templates/addrmap_register.py.jinja` & `peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/addrmap_register.py.jinja`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.0/src/peakrdl_python/templates/addrmap_tb.py.jinja` & `peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/addrmap_tb.py.jinja`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.0/src/peakrdl_python/templates/baseclass_tb.py.jinja` & `peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/baseclass_tb.py.jinja`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.0/src/peakrdl_python/templates/reg_definitions.py.jinja` & `peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/reg_definitions.py.jinja`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.0/src/peakrdl_python.egg-info/PKG-INFO` & `peakrdl-python-0.6.0rc1/src/peakrdl_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peakrdl-python
-Version: 0.6.0
+Version: 0.6.0rc1
 Summary: Generate python wrapper for a register model compiled SystemRDL input
 Home-page: https://github.com/krcb197/PeakRDL-python
 Author: Keith Brady
 License: UNKNOWN
 Project-URL: Source, https://github.com/krcb197/PeakRDL-python
 Project-URL: Tracker, https://github.com/krcb197/PeakRDL-python/issues
 Project-URL: Documentation, https://peakrdl-python.readthedocs.io/
```

### Comparing `peakrdl-python-0.6.0/src/peakrdl_python.egg-info/SOURCES.txt` & `peakrdl-python-0.6.0rc1/src/peakrdl_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

