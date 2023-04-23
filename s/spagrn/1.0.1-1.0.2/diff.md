# Comparing `tmp/spagrn-1.0.1.tar.gz` & `tmp/spagrn-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spagrn-1.0.1.tar", last modified: Fri Apr 21 12:33:33 2023, max compression
+gzip compressed data, was "spagrn-1.0.2.tar", last modified: Sun Apr 23 10:28:21 2023, max compression
```

## Comparing `spagrn-1.0.1.tar` & `spagrn-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 yao        (502) staff       (20)        0 2023-04-21 12:33:33.485158 spagrn-1.0.1/
--rw-r--r--   0 yao        (502) staff       (20)    35149 2023-04-11 12:27:22.000000 spagrn-1.0.1/LICENSE
--rw-r--r--   0 yao        (502) staff       (20)      598 2023-04-21 12:33:33.485208 spagrn-1.0.1/PKG-INFO
--rw-r--r--   0 yao        (502) staff       (20)     3533 2023-04-21 12:32:52.000000 spagrn-1.0.1/README.md
--rw-r--r--   0 yao        (502) staff       (20)       79 2023-04-21 12:33:33.485392 spagrn-1.0.1/setup.cfg
--rw-r--r--   0 yao        (502) staff       (20)      938 2023-04-21 12:29:39.000000 spagrn-1.0.1/setup.py
-drwxr-xr-x   0 yao        (502) staff       (20)        0 2023-04-21 12:33:33.484551 spagrn-1.0.1/spagrn/
--rw-r--r--   0 yao        (502) staff       (20)      282 2023-04-21 12:16:13.000000 spagrn-1.0.1/spagrn/__init__.py
--rw-r--r--   0 yao        (502) staff       (20)    13782 2023-04-21 12:16:13.000000 spagrn-1.0.1/spagrn/plot.py
--rw-r--r--   0 yao        (502) staff       (20)    39463 2023-04-21 12:16:13.000000 spagrn-1.0.1/spagrn/regulatory_network.py
--rw-r--r--   0 yao        (502) staff       (20)     1202 2023-04-08 12:20:26.000000 spagrn-1.0.1/spagrn/spa_logger.py
-drwxr-xr-x   0 yao        (502) staff       (20)        0 2023-04-21 12:33:33.485060 spagrn-1.0.1/spagrn/spagrn.egg-info/
--rw-r--r--   0 yao        (502) staff       (20)      598 2023-04-21 12:33:33.000000 spagrn-1.0.1/spagrn/spagrn.egg-info/PKG-INFO
--rw-r--r--   0 yao        (502) staff       (20)      283 2023-04-21 12:33:33.000000 spagrn-1.0.1/spagrn/spagrn.egg-info/SOURCES.txt
--rw-r--r--   0 yao        (502) staff       (20)        1 2023-04-21 12:33:33.000000 spagrn-1.0.1/spagrn/spagrn.egg-info/dependency_links.txt
--rw-r--r--   0 yao        (502) staff       (20)       49 2023-04-21 12:33:33.000000 spagrn-1.0.1/spagrn/spagrn.egg-info/top_level.txt
--rw-r--r--   0 yao        (502) staff       (20)     1867 2023-04-08 12:23:27.000000 spagrn-1.0.1/spagrn/test.py
+drwxr-xr-x   0 yao        (502) staff       (20)        0 2023-04-23 10:28:21.098391 spagrn-1.0.2/
+-rw-r--r--   0 yao        (502) staff       (20)    35149 2023-04-11 12:27:22.000000 spagrn-1.0.2/LICENSE
+-rw-r--r--   0 yao        (502) staff       (20)      627 2023-04-23 10:28:21.098441 spagrn-1.0.2/PKG-INFO
+-rw-r--r--   0 yao        (502) staff       (20)     3617 2023-04-23 10:09:19.000000 spagrn-1.0.2/README.md
+-rw-r--r--   0 yao        (502) staff       (20)       79 2023-04-23 10:28:21.098631 spagrn-1.0.2/setup.cfg
+-rw-r--r--   0 yao        (502) staff       (20)      972 2023-04-23 10:28:11.000000 spagrn-1.0.2/setup.py
+drwxr-xr-x   0 yao        (502) staff       (20)        0 2023-04-23 10:28:21.097683 spagrn-1.0.2/spagrn/
+-rw-r--r--   0 yao        (502) staff       (20)      282 2023-04-21 12:16:13.000000 spagrn-1.0.2/spagrn/__init__.py
+-rw-r--r--   0 yao        (502) staff       (20)    13782 2023-04-21 12:16:13.000000 spagrn-1.0.2/spagrn/plot.py
+-rw-r--r--   0 yao        (502) staff       (20)    39463 2023-04-21 12:16:13.000000 spagrn-1.0.2/spagrn/regulatory_network.py
+-rw-r--r--   0 yao        (502) staff       (20)     1202 2023-04-08 12:20:26.000000 spagrn-1.0.2/spagrn/spa_logger.py
+-rw-r--r--   0 yao        (502) staff       (20)     1867 2023-04-08 12:23:27.000000 spagrn-1.0.2/spagrn/test.py
+drwxr-xr-x   0 yao        (502) staff       (20)        0 2023-04-23 10:28:21.098307 spagrn-1.0.2/spagrn.egg-info/
+-rw-r--r--   0 yao        (502) staff       (20)      627 2023-04-23 10:28:21.000000 spagrn-1.0.2/spagrn.egg-info/PKG-INFO
+-rw-r--r--   0 yao        (502) staff       (20)      284 2023-04-23 10:28:21.000000 spagrn-1.0.2/spagrn.egg-info/SOURCES.txt
+-rw-r--r--   0 yao        (502) staff       (20)        1 2023-04-23 10:28:21.000000 spagrn-1.0.2/spagrn.egg-info/dependency_links.txt
+-rw-r--r--   0 yao        (502) staff       (20)      162 2023-04-23 10:28:21.000000 spagrn-1.0.2/spagrn.egg-info/requires.txt
+-rw-r--r--   0 yao        (502) staff       (20)        7 2023-04-23 10:28:21.000000 spagrn-1.0.2/spagrn.egg-info/top_level.txt
```

### Comparing `spagrn-1.0.1/LICENSE` & `spagrn-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spagrn-1.0.1/PKG-INFO` & `spagrn-1.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: spagrn
-Version: 1.0.1
+Version: 1.0.2
 Summary: A comprehensive tool to infer TF-centered, spatial gene regulatory networks for the spatially resolved transcriptomic data.
 Home-page: https://github.com/BGI-Qingdao/SpaGRN
 Author: Yao LI, Lidong GUO, Mengyang XU
 Author-email: liyao1@genomics.cn, guolidong@genomics.cn, xumengyang@genomics.cn
 License: GPL-3.0+
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7,<3.11
 License-File: LICENSE
 
 UNKNOWN
```

### Comparing `spagrn-1.0.1/README.md` & `spagrn-1.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -28,15 +28,28 @@
 ```
 from spagrn import InferRegulatoryNetwork as irn
 from spagrn import PlotRegulatoryNetwork as prn
 ```
 
 Dependencies
 ```
-Pandas, numpy, scanpy, matplotlib, and seaborn are required to be pre-installed
+anndata==0.8.0 
+pandas>=1.3.5
+scanpy
+seaborn
+matplotlib 
+pyscenic==0.12.1
+hotspotsc==1.1.1
+scipy
+numpy
+dask
+arboreto
+ctxcore>=0.2.0
+sklearn
+multiprocessing_on_dill
 ```
 
 
 # Usage
 The package provides functions for loading data, preprocessing data, reconstructing gene network, and visualizing the inferred GRNs. The main functions are:
 * Load and process data
 * Compute TF-gene similarities
```

### Comparing `spagrn-1.0.1/spagrn/plot.py` & `spagrn-1.0.2/spagrn/plot.py`

 * *Files identical despite different names*

### Comparing `spagrn-1.0.1/spagrn/regulatory_network.py` & `spagrn-1.0.2/spagrn/regulatory_network.py`

 * *Files identical despite different names*

### Comparing `spagrn-1.0.1/spagrn/spa_logger.py` & `spagrn-1.0.2/spagrn/spa_logger.py`

 * *Files identical despite different names*

### Comparing `spagrn-1.0.1/spagrn/spagrn.egg-info/PKG-INFO` & `spagrn-1.0.2/spagrn.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: spagrn
-Version: 1.0.1
+Version: 1.0.2
 Summary: A comprehensive tool to infer TF-centered, spatial gene regulatory networks for the spatially resolved transcriptomic data.
 Home-page: https://github.com/BGI-Qingdao/SpaGRN
 Author: Yao LI, Lidong GUO, Mengyang XU
 Author-email: liyao1@genomics.cn, guolidong@genomics.cn, xumengyang@genomics.cn
 License: GPL-3.0+
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7,<3.11
 License-File: LICENSE
 
 UNKNOWN
```

### Comparing `spagrn-1.0.1/spagrn/test.py` & `spagrn-1.0.2/spagrn/test.py`

 * *Files identical despite different names*

