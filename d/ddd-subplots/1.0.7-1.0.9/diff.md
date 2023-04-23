# Comparing `tmp/ddd_subplots-1.0.7.tar.gz` & `tmp/ddd_subplots-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ddd_subplots-1.0.7.tar", last modified: Fri Mar  5 20:41:07 2021, max compression
+gzip compressed data, was "dist/ddd_subplots-1.0.9.tar", last modified: Sat May 15 19:30:39 2021, max compression
```

## Comparing `ddd_subplots-1.0.7.tar` & `ddd_subplots-1.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2021-03-05 20:41:07.000000 ddd_subplots-1.0.7/
--rw-r--r--   0 lucacappelletti   (501) staff       (20)        0 2021-03-05 20:36:41.000000 ddd_subplots-1.0.7/MANIFEST.in
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     6508 2021-03-05 20:41:07.000000 ddd_subplots-1.0.7/PKG-INFO
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     5045 2021-03-05 20:36:41.000000 ddd_subplots-1.0.7/README.rst
-drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2021-03-05 20:41:07.000000 ddd_subplots-1.0.7/ddd_subplots/
--rw-r--r--   0 lucacappelletti   (501) staff       (20)       91 2021-03-05 20:36:41.000000 ddd_subplots-1.0.7/ddd_subplots/__init__.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)       67 2021-03-05 20:40:33.000000 ddd_subplots-1.0.7/ddd_subplots/__version__.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     3008 2021-03-05 20:36:41.000000 ddd_subplots-1.0.7/ddd_subplots/rotate.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     1909 2021-03-05 20:40:25.000000 ddd_subplots-1.0.7/ddd_subplots/subplots.py
-drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2021-03-05 20:41:07.000000 ddd_subplots-1.0.7/ddd_subplots.egg-info/
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     6508 2021-03-05 20:41:07.000000 ddd_subplots-1.0.7/ddd_subplots.egg-info/PKG-INFO
--rw-r--r--   0 lucacappelletti   (501) staff       (20)      311 2021-03-05 20:41:07.000000 ddd_subplots-1.0.7/ddd_subplots.egg-info/SOURCES.txt
--rw-r--r--   0 lucacappelletti   (501) staff       (20)        1 2021-03-05 20:41:07.000000 ddd_subplots-1.0.7/ddd_subplots.egg-info/dependency_links.txt
--rw-r--r--   0 lucacappelletti   (501) staff       (20)      123 2021-03-05 20:41:07.000000 ddd_subplots-1.0.7/ddd_subplots.egg-info/requires.txt
--rw-r--r--   0 lucacappelletti   (501) staff       (20)       13 2021-03-05 20:41:07.000000 ddd_subplots-1.0.7/ddd_subplots.egg-info/top_level.txt
--rw-r--r--   0 lucacappelletti   (501) staff       (20)       38 2021-03-05 20:41:07.000000 ddd_subplots-1.0.7/setup.cfg
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     1784 2021-03-05 20:36:41.000000 ddd_subplots-1.0.7/setup.py
+drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2021-05-15 19:30:39.000000 ddd_subplots-1.0.9/
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)        0 2021-04-23 09:02:12.000000 ddd_subplots-1.0.9/MANIFEST.in
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     6508 2021-05-15 19:30:39.000000 ddd_subplots-1.0.9/PKG-INFO
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     5045 2021-04-23 09:02:12.000000 ddd_subplots-1.0.9/README.rst
+drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2021-05-15 19:30:39.000000 ddd_subplots-1.0.9/ddd_subplots/
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)       91 2021-04-23 09:02:12.000000 ddd_subplots-1.0.9/ddd_subplots/__init__.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)       68 2021-05-15 19:27:31.000000 ddd_subplots-1.0.9/ddd_subplots/__version__.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     5529 2021-05-15 19:28:13.000000 ddd_subplots-1.0.9/ddd_subplots/rotate.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     1718 2021-05-15 19:28:14.000000 ddd_subplots-1.0.9/ddd_subplots/subplots.py
+drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2021-05-15 19:30:39.000000 ddd_subplots-1.0.9/ddd_subplots.egg-info/
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     6508 2021-05-15 19:30:39.000000 ddd_subplots-1.0.9/ddd_subplots.egg-info/PKG-INFO
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      311 2021-05-15 19:30:39.000000 ddd_subplots-1.0.9/ddd_subplots.egg-info/SOURCES.txt
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)        1 2021-05-15 19:30:39.000000 ddd_subplots-1.0.9/ddd_subplots.egg-info/dependency_links.txt
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      123 2021-05-15 19:30:39.000000 ddd_subplots-1.0.9/ddd_subplots.egg-info/requires.txt
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)       13 2021-05-15 19:30:39.000000 ddd_subplots-1.0.9/ddd_subplots.egg-info/top_level.txt
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)       38 2021-05-15 19:30:39.000000 ddd_subplots-1.0.9/setup.cfg
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     1784 2021-04-23 09:02:12.000000 ddd_subplots-1.0.9/setup.py
```

### Comparing `ddd_subplots-1.0.7/PKG-INFO` & `ddd_subplots-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddd_subplots
-Version: 1.0.7
+Version: 1.0.9
 Summary: Python package making it easier to handle mixed 3d and 2d subplots.
 Home-page: https://github.com/LucaCappelletti94/ddd_subplots
 Author: Luca Cappelletti
 Author-email: cappelletti.luca94@gmail.com
 License: MIT
 Description: ddd_subplots
         =========================================================================================
```

### Comparing `ddd_subplots-1.0.7/README.rst` & `ddd_subplots-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `ddd_subplots-1.0.7/ddd_subplots/subplots.py` & `ddd_subplots-1.0.9/ddd_subplots/subplots.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,37 @@
-from typing import Tuple, Dict
-import numpy as np
+"""Submodule providing 3d subplots handler."""
+from typing import Dict, Tuple
+
 import matplotlib.pyplot as plt
+import numpy as np
 from matplotlib.figure import Figure
-from matplotlib.axes import Axes
 from mpl_toolkits.mplot3d import Axes3D
 
 
 def subplots(
     nrows: int = 1,
     ncols: int = 1,
     subplot_kw: Dict = None,
-    gridspec_kw: Dict = None,
     squeeze: bool = True,
     ** fig_kw: Dict
-) -> Tuple[Figure, Axes]:
+) -> Tuple[Figure, Axes3D]:
     """
     Create a figure and a set of subplots.
 
     This utility wrapper makes it convenient to create common layouts of
     subplots, including the enclosing figure object, in a single call.
 
     Parameters
     ----------
     nrows, ncols : int, optional, default: 1
         Number of rows/columns of the subplot grid.
     subplot_kw : dict, optional
         Dict with keywords passed to the
         `~matplotlib.figure.Figure.add_subplot` call used to create each
         subplot.
-    gridspec_kw : dict, optional
-        Dict with keywords passed to the `~matplotlib.gridspec.GridSpec`
-        constructor used to create the grid the subplots are placed on.
     **fig_kw
         All additional keyword arguments are passed to the
         `.pyplot.figure` call.
 
     Returns
     -------
     fig : `~.figure.Figure`
```

### Comparing `ddd_subplots-1.0.7/ddd_subplots.egg-info/PKG-INFO` & `ddd_subplots-1.0.9/ddd_subplots.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddd-subplots
-Version: 1.0.7
+Version: 1.0.9
 Summary: Python package making it easier to handle mixed 3d and 2d subplots.
 Home-page: https://github.com/LucaCappelletti94/ddd_subplots
 Author: Luca Cappelletti
 Author-email: cappelletti.luca94@gmail.com
 License: MIT
 Description: ddd_subplots
         =========================================================================================
```

### Comparing `ddd_subplots-1.0.7/setup.py` & `ddd_subplots-1.0.9/setup.py`

 * *Files identical despite different names*

