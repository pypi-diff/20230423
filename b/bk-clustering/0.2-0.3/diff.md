# Comparing `tmp/bk_clustering-0.2.tar.gz` & `tmp/bk_clustering-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bk_clustering-0.2.tar", max compression
+gzip compressed data, was "bk_clustering-0.3.tar", max compression
```

## Comparing `bk_clustering-0.2.tar` & `bk_clustering-0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0        0 2023-03-09 12:14:06.008282 bk_clustering-0.2/README.md
--rw-r--r--   0        0        0       40 2023-04-08 23:59:03.211844 bk_clustering-0.2/bk_clustering/__init__.py
--rw-r--r--   0        0        0    33769 2023-03-25 12:39:17.568753 bk_clustering-0.2/bk_clustering/_hierarchy.pyx
--rw-r--r--   0        0        0     9236 2023-04-14 23:25:00.737155 bk_clustering-0.2/bk_clustering/main.py
--rw-r--r--   0        0        0     3586 2023-04-14 23:24:33.837484 bk_clustering-0.2/bk_clustering/run_batch.py
--rw-r--r--   0        0        0        1 2023-04-11 00:55:31.723142 bk_clustering-0.2/bk_clustering/utilities/__init__.py
--rw-r--r--   0        0        0     2012 2023-04-08 23:21:19.153823 bk_clustering-0.2/bk_clustering/utilities/calculation_utilities.py
--rw-r--r--   0        0        0     5155 2023-04-11 00:55:31.879142 bk_clustering-0.2/bk_clustering/utilities/cluster_calculations.py
--rw-r--r--   0        0        0     6955 2023-03-30 17:31:18.984431 bk_clustering-0.2/bk_clustering/utilities/density_peak.py
--rw-r--r--   0        0        0     3788 2023-04-13 23:18:23.103160 bk_clustering-0.2/bk_clustering/utilities/load_save.py
--rw-r--r--   0        0        0    17756 2023-04-15 17:21:26.122830 bk_clustering-0.2/bk_clustering/utilities/method_comparison.py
--rw-r--r--   0        0        0     8278 2023-04-13 11:16:17.707177 bk_clustering-0.2/bk_clustering/utilities/metrics.py
--rw-r--r--   0        0        0     4511 2023-04-09 08:12:54.956531 bk_clustering-0.2/bk_clustering/utilities/plot_utilities.py
--rw-r--r--   0        0        0     2607 2023-04-15 00:03:42.881455 bk_clustering-0.2/bk_clustering/utilities/preprocessing.py
--rw-r--r--   0        0        0    13106 2023-04-09 08:13:24.269397 bk_clustering-0.2/bk_clustering/utilities/tree_traversal.py
--rw-r--r--   0        0        0      453 2023-04-15 17:20:13.435314 bk_clustering-0.2/pyproject.toml
--rw-r--r--   0        0        0      538 1970-01-01 00:00:00.000000 bk_clustering-0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-22 21:57:10.406160 bk_clustering-0.3/README.md
+-rw-r--r--   0        0        0       40 2023-04-08 23:59:03.211844 bk_clustering-0.3/bk_clustering/__init__.py
+-rw-r--r--   0        0        0    33769 2023-03-25 12:39:17.568753 bk_clustering-0.3/bk_clustering/_hierarchy.pyx
+-rw-r--r--   0        0        0     9236 2023-04-22 01:06:37.965085 bk_clustering-0.3/bk_clustering/main.py
+-rw-r--r--   0        0        0     3586 2023-04-22 22:05:11.378453 bk_clustering-0.3/bk_clustering/run_batch.py
+-rw-r--r--   0        0        0        1 2023-04-11 00:55:31.723142 bk_clustering-0.3/bk_clustering/utilities/__init__.py
+-rw-r--r--   0        0        0     2012 2023-04-08 23:21:19.153823 bk_clustering-0.3/bk_clustering/utilities/calculation_utilities.py
+-rw-r--r--   0        0        0     5155 2023-04-11 00:55:31.879142 bk_clustering-0.3/bk_clustering/utilities/cluster_calculations.py
+-rw-r--r--   0        0        0     6955 2023-03-30 17:31:18.984431 bk_clustering-0.3/bk_clustering/utilities/density_peak.py
+-rw-r--r--   0        0        0     3788 2023-04-22 01:06:37.965085 bk_clustering-0.3/bk_clustering/utilities/load_save.py
+-rw-r--r--   0        0        0    17756 2023-04-22 01:06:37.965085 bk_clustering-0.3/bk_clustering/utilities/method_comparison.py
+-rw-r--r--   0        0        0     8278 2023-04-13 11:16:17.707177 bk_clustering-0.3/bk_clustering/utilities/metrics.py
+-rw-r--r--   0        0        0     4511 2023-04-09 08:12:54.956531 bk_clustering-0.3/bk_clustering/utilities/plot_utilities.py
+-rw-r--r--   0        0        0     2607 2023-04-15 00:03:42.881455 bk_clustering-0.3/bk_clustering/utilities/preprocessing.py
+-rw-r--r--   0        0        0    13106 2023-04-09 08:13:24.269397 bk_clustering-0.3/bk_clustering/utilities/tree_traversal.py
+-rw-r--r--   0        0        0      453 2023-04-22 22:01:42.307723 bk_clustering-0.3/pyproject.toml
+-rw-r--r--   0        0        0      538 1970-01-01 00:00:00.000000 bk_clustering-0.3/PKG-INFO
```

### Comparing `bk_clustering-0.2/bk_clustering/_hierarchy.pyx` & `bk_clustering-0.3/bk_clustering/_hierarchy.pyx`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.2/bk_clustering/main.py` & `bk_clustering-0.3/bk_clustering/main.py`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.2/bk_clustering/run_batch.py` & `bk_clustering-0.3/bk_clustering/run_batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from utilities import load_save, metrics, method_comparison
+from utilities import load_save, metrics #method_comparison
 import os
 from timeit import default_timer as timer
 from main import BurjKhalifaClustering
 
 SKIP_COLUMNS_IN_DATASET = {
     ("real", "wdbc"): ["idnumber"],
     ("real", "spectrometer"): ["LRS-name"],
```

### Comparing `bk_clustering-0.2/bk_clustering/utilities/calculation_utilities.py` & `bk_clustering-0.3/bk_clustering/utilities/calculation_utilities.py`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.2/bk_clustering/utilities/cluster_calculations.py` & `bk_clustering-0.3/bk_clustering/utilities/cluster_calculations.py`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.2/bk_clustering/utilities/density_peak.py` & `bk_clustering-0.3/bk_clustering/utilities/density_peak.py`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.2/bk_clustering/utilities/load_save.py` & `bk_clustering-0.3/bk_clustering/utilities/load_save.py`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.2/bk_clustering/utilities/method_comparison.py` & `bk_clustering-0.3/bk_clustering/utilities/method_comparison.py`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.2/bk_clustering/utilities/metrics.py` & `bk_clustering-0.3/bk_clustering/utilities/metrics.py`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.2/bk_clustering/utilities/plot_utilities.py` & `bk_clustering-0.3/bk_clustering/utilities/plot_utilities.py`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.2/bk_clustering/utilities/preprocessing.py` & `bk_clustering-0.3/bk_clustering/utilities/preprocessing.py`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.2/bk_clustering/utilities/tree_traversal.py` & `bk_clustering-0.3/bk_clustering/utilities/tree_traversal.py`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.2/PKG-INFO` & `bk_clustering-0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: bk-clustering
-Version: 0.2
-Summary: The package is the implementation of the Burj-Khalifa clustering algorithm
+Version: 0.3
+Summary: The package is the implementation of the Burj Khalifa clustering algorithm
 Author: Ivan Reznikov
 Author-email: ivanreznikov@gmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: arff (>=0.9,<0.10)
```

