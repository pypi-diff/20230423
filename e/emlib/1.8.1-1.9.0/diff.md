# Comparing `tmp/emlib-1.8.1.tar.gz` & `tmp/emlib-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emlib-1.8.1.tar", last modified: Tue Apr 18 11:11:24 2023, max compression
+gzip compressed data, was "emlib-1.9.0.tar", last modified: Sun Apr 23 11:22:08 2023, max compression
```

## Comparing `emlib-1.8.1.tar` & `emlib-1.9.0.tar`

### file list

```diff
@@ -1,44 +1,46 @@
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-18 11:11:24.140437 emlib-1.8.1/
--rw-rw-r--   0 em        (1000) em        (1000)     1065 2023-04-18 11:11:24.141437 emlib-1.8.1/PKG-INFO
--rwxrwxr-x   0 em        (1000) em        (1000)      612 2021-11-22 12:50:35.000000 emlib-1.8.1/README.rst
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-18 11:11:24.136437 emlib-1.8.1/emlib/
--rwxrwxr-x   0 em        (1000) em        (1000)      552 2021-11-22 12:50:35.000000 emlib-1.8.1/emlib/__init__.py
--rw-rw-r--   0 em        (1000) em        (1000)     9290 2022-02-28 20:16:06.000000 emlib-1.8.1/emlib/_dialogsqt.py
--rwxrwxr-x   0 em        (1000) em        (1000)     5276 2021-11-22 12:50:35.000000 emlib-1.8.1/emlib/calculus.py
--rwxrwxr-x   0 em        (1000) em        (1000)    13951 2021-11-22 12:51:36.000000 emlib-1.8.1/emlib/combinatorics.py
--rwxrwxr-x   0 em        (1000) em        (1000)    11691 2023-01-05 02:24:33.000000 emlib-1.8.1/emlib/containers.py
--rwxrwxr-x   0 em        (1000) em        (1000)     7381 2021-11-22 12:52:47.000000 emlib-1.8.1/emlib/csvtools.py
--rw-rw-r--   0 em        (1000) em        (1000)    14750 2023-03-29 14:12:27.000000 emlib-1.8.1/emlib/dialogs.py
--rw-rw-r--   0 em        (1000) em        (1000)    40862 2022-05-02 12:30:18.000000 emlib-1.8.1/emlib/doctools.py
--rwxrwxr-x   0 em        (1000) em        (1000)    11931 2023-02-13 09:29:14.000000 emlib-1.8.1/emlib/electronics.py
--rwxrwxr-x   0 em        (1000) em        (1000)     4783 2022-05-26 12:13:22.000000 emlib-1.8.1/emlib/filetools.py
--rw-rw-r--   0 em        (1000) em        (1000)     1666 2021-11-22 12:50:35.000000 emlib-1.8.1/emlib/graphlib.py
--rw-rw-r--   0 em        (1000) em        (1000)     4888 2021-11-22 12:50:35.000000 emlib-1.8.1/emlib/img.py
--rwxrwxr-x   0 em        (1000) em        (1000)    17569 2023-02-09 09:01:05.000000 emlib-1.8.1/emlib/iterlib.py
--rw-rw-r--   0 em        (1000) em        (1000)     3726 2021-11-22 12:50:35.000000 emlib-1.8.1/emlib/jsontools.py
--rwxrwxr-x   0 em        (1000) em        (1000)     1836 2022-12-11 17:42:25.000000 emlib-1.8.1/emlib/logutils.py
--rw-rw-r--   0 em        (1000) em        (1000)    20805 2023-02-27 19:03:05.000000 emlib-1.8.1/emlib/mathlib.py
--rw-rw-r--   0 em        (1000) em        (1000)    12649 2021-11-22 12:50:35.000000 emlib-1.8.1/emlib/matplotting.py
--rw-rw-r--   0 em        (1000) em        (1000)     3000 2021-11-22 12:50:35.000000 emlib-1.8.1/emlib/minizinctools.py
--rwxrwxr-x   0 em        (1000) em        (1000)    57495 2023-04-18 11:09:30.000000 emlib-1.8.1/emlib/misc.py
--rwxrwxr-x   0 em        (1000) em        (1000)     1361 2021-11-22 12:50:35.000000 emlib-1.8.1/emlib/net.py
--rw-rw-r--   0 em        (1000) em        (1000)     1824 2021-11-22 12:50:35.000000 emlib-1.8.1/emlib/numberseries.py
--rwxrwxr-x   0 em        (1000) em        (1000)     8133 2022-04-05 12:38:34.000000 emlib-1.8.1/emlib/numpytools.py
--rwxrwxr-x   0 em        (1000) em        (1000)     4890 2021-11-22 12:50:35.000000 emlib-1.8.1/emlib/numtheory.py
--rwxrwxr-x   0 em        (1000) em        (1000)     2126 2022-05-02 20:42:02.000000 emlib-1.8.1/emlib/parabolicinterpol.py
--rwxrwxr-x   0 em        (1000) em        (1000)     1840 2021-11-22 12:50:35.000000 emlib-1.8.1/emlib/readbytes.py
--rw-rw-r--   0 em        (1000) em        (1000)     2128 2021-11-22 12:50:35.000000 emlib-1.8.1/emlib/shelling.py
--rwxrwxr-x   0 em        (1000) em        (1000)     7950 2022-05-02 20:07:38.000000 emlib-1.8.1/emlib/smooth.py
--rwxrwxr-x   0 em        (1000) em        (1000)     7777 2022-05-02 20:07:38.000000 emlib-1.8.1/emlib/stochastic.py
--rw-rw-r--   0 em        (1000) em        (1000)     6060 2023-03-15 10:12:58.000000 emlib-1.8.1/emlib/textlib.py
--rwxrwxr-x   0 em        (1000) em        (1000)     1301 2022-05-02 19:50:30.000000 emlib-1.8.1/emlib/video.py
--rwxrwxr-x   0 em        (1000) em        (1000)     8527 2022-05-02 20:00:33.000000 emlib-1.8.1/emlib/xmlprinter.py
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-18 11:11:24.140437 emlib-1.8.1/emlib.egg-info/
--rw-rw-r--   0 em        (1000) em        (1000)     1065 2023-04-18 11:11:23.000000 emlib-1.8.1/emlib.egg-info/PKG-INFO
--rw-rw-r--   0 em        (1000) em        (1000)      779 2023-04-18 11:11:24.000000 emlib-1.8.1/emlib.egg-info/SOURCES.txt
--rw-rw-r--   0 em        (1000) em        (1000)        1 2023-04-18 11:11:23.000000 emlib-1.8.1/emlib.egg-info/dependency_links.txt
--rw-rw-r--   0 em        (1000) em        (1000)        1 2022-02-27 18:43:41.000000 emlib-1.8.1/emlib.egg-info/not-zip-safe
--rw-rw-r--   0 em        (1000) em        (1000)      117 2023-04-18 11:11:23.000000 emlib-1.8.1/emlib.egg-info/requires.txt
--rw-rw-r--   0 em        (1000) em        (1000)        6 2023-04-18 11:11:23.000000 emlib-1.8.1/emlib.egg-info/top_level.txt
--rwxrwxr-x   0 em        (1000) em        (1000)       61 2023-04-18 11:11:24.141437 emlib-1.8.1/setup.cfg
--rw-rw-r--   0 em        (1000) em        (1000)     1074 2023-04-18 11:10:58.000000 emlib-1.8.1/setup.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-23 11:22:08.363145 emlib-1.9.0/
+-rw-rw-r--   0 em        (1000) em        (1000)     1065 2023-04-23 11:22:08.363145 emlib-1.9.0/PKG-INFO
+-rwxrwxr-x   0 em        (1000) em        (1000)      612 2021-11-22 12:50:35.000000 emlib-1.9.0/README.rst
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-23 11:22:08.360145 emlib-1.9.0/emlib/
+-rwxrwxr-x   0 em        (1000) em        (1000)      552 2021-11-22 12:50:35.000000 emlib-1.9.0/emlib/__init__.py
+-rw-rw-r--   0 em        (1000) em        (1000)     9290 2022-02-28 20:16:06.000000 emlib-1.9.0/emlib/_dialogsqt.py
+-rwxrwxr-x   0 em        (1000) em        (1000)     5276 2021-11-22 12:50:35.000000 emlib-1.9.0/emlib/calculus.py
+-rwxrwxr-x   0 em        (1000) em        (1000)    13951 2021-11-22 12:51:36.000000 emlib-1.9.0/emlib/combinatorics.py
+-rw-rw-r--   0 em        (1000) em        (1000)      783 2023-04-23 09:50:49.000000 emlib-1.9.0/emlib/common.py
+-rwxrwxr-x   0 em        (1000) em        (1000)    11691 2023-01-05 02:24:33.000000 emlib-1.9.0/emlib/containers.py
+-rwxrwxr-x   0 em        (1000) em        (1000)     7381 2021-11-22 12:52:47.000000 emlib-1.9.0/emlib/csvtools.py
+-rw-rw-r--   0 em        (1000) em        (1000)    14750 2023-03-29 14:12:27.000000 emlib-1.9.0/emlib/dialogs.py
+-rw-rw-r--   0 em        (1000) em        (1000)    40862 2022-05-02 12:30:18.000000 emlib-1.9.0/emlib/doctools.py
+-rwxrwxr-x   0 em        (1000) em        (1000)    11931 2023-02-13 09:29:14.000000 emlib-1.9.0/emlib/electronics.py
+-rw-rw-r--   0 em        (1000) em        (1000)     4473 2023-04-23 09:55:27.000000 emlib-1.9.0/emlib/envir.py
+-rwxrwxr-x   0 em        (1000) em        (1000)     4783 2022-05-26 12:13:22.000000 emlib-1.9.0/emlib/filetools.py
+-rw-rw-r--   0 em        (1000) em        (1000)     1666 2021-11-22 12:50:35.000000 emlib-1.9.0/emlib/graphlib.py
+-rw-rw-r--   0 em        (1000) em        (1000)     4888 2021-11-22 12:50:35.000000 emlib-1.9.0/emlib/img.py
+-rwxrwxr-x   0 em        (1000) em        (1000)    17569 2023-02-09 09:01:05.000000 emlib-1.9.0/emlib/iterlib.py
+-rw-rw-r--   0 em        (1000) em        (1000)     3726 2021-11-22 12:50:35.000000 emlib-1.9.0/emlib/jsontools.py
+-rwxrwxr-x   0 em        (1000) em        (1000)     1836 2022-12-11 17:42:25.000000 emlib-1.9.0/emlib/logutils.py
+-rw-rw-r--   0 em        (1000) em        (1000)    20805 2023-02-27 19:03:05.000000 emlib-1.9.0/emlib/mathlib.py
+-rw-rw-r--   0 em        (1000) em        (1000)    12649 2021-11-22 12:50:35.000000 emlib-1.9.0/emlib/matplotting.py
+-rw-rw-r--   0 em        (1000) em        (1000)     3000 2021-11-22 12:50:35.000000 emlib-1.9.0/emlib/minizinctools.py
+-rwxrwxr-x   0 em        (1000) em        (1000)    52792 2023-04-23 11:17:53.000000 emlib-1.9.0/emlib/misc.py
+-rwxrwxr-x   0 em        (1000) em        (1000)     1361 2021-11-22 12:50:35.000000 emlib-1.9.0/emlib/net.py
+-rw-rw-r--   0 em        (1000) em        (1000)     1824 2021-11-22 12:50:35.000000 emlib-1.9.0/emlib/numberseries.py
+-rwxrwxr-x   0 em        (1000) em        (1000)     8133 2022-04-05 12:38:34.000000 emlib-1.9.0/emlib/numpytools.py
+-rwxrwxr-x   0 em        (1000) em        (1000)     4890 2021-11-22 12:50:35.000000 emlib-1.9.0/emlib/numtheory.py
+-rwxrwxr-x   0 em        (1000) em        (1000)     2126 2022-05-02 20:42:02.000000 emlib-1.9.0/emlib/parabolicinterpol.py
+-rwxrwxr-x   0 em        (1000) em        (1000)     1840 2021-11-22 12:50:35.000000 emlib-1.9.0/emlib/readbytes.py
+-rw-rw-r--   0 em        (1000) em        (1000)     2128 2021-11-22 12:50:35.000000 emlib-1.9.0/emlib/shelling.py
+-rwxrwxr-x   0 em        (1000) em        (1000)     7950 2022-05-02 20:07:38.000000 emlib-1.9.0/emlib/smooth.py
+-rwxrwxr-x   0 em        (1000) em        (1000)     7777 2022-05-02 20:07:38.000000 emlib-1.9.0/emlib/stochastic.py
+-rw-rw-r--   0 em        (1000) em        (1000)     6060 2023-03-15 10:12:58.000000 emlib-1.9.0/emlib/textlib.py
+-rwxrwxr-x   0 em        (1000) em        (1000)     1301 2022-05-02 19:50:30.000000 emlib-1.9.0/emlib/video.py
+-rwxrwxr-x   0 em        (1000) em        (1000)     8527 2022-05-02 20:00:33.000000 emlib-1.9.0/emlib/xmlprinter.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-23 11:22:08.363145 emlib-1.9.0/emlib.egg-info/
+-rw-rw-r--   0 em        (1000) em        (1000)     1065 2023-04-23 11:22:08.000000 emlib-1.9.0/emlib.egg-info/PKG-INFO
+-rw-rw-r--   0 em        (1000) em        (1000)      810 2023-04-23 11:22:08.000000 emlib-1.9.0/emlib.egg-info/SOURCES.txt
+-rw-rw-r--   0 em        (1000) em        (1000)        1 2023-04-23 11:22:08.000000 emlib-1.9.0/emlib.egg-info/dependency_links.txt
+-rw-rw-r--   0 em        (1000) em        (1000)        1 2022-02-27 18:43:41.000000 emlib-1.9.0/emlib.egg-info/not-zip-safe
+-rw-rw-r--   0 em        (1000) em        (1000)      117 2023-04-23 11:22:08.000000 emlib-1.9.0/emlib.egg-info/requires.txt
+-rw-rw-r--   0 em        (1000) em        (1000)        6 2023-04-23 11:22:08.000000 emlib-1.9.0/emlib.egg-info/top_level.txt
+-rwxrwxr-x   0 em        (1000) em        (1000)       61 2023-04-23 11:22:08.364145 emlib-1.9.0/setup.cfg
+-rw-rw-r--   0 em        (1000) em        (1000)     1053 2023-04-23 11:19:03.000000 emlib-1.9.0/setup.py
```

### Comparing `emlib-1.8.1/PKG-INFO` & `emlib-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emlib
-Version: 1.8.1
+Version: 1.9.0
 Summary: Miscellaneous utilities
 Home-page: https://github.com/gesellkammer/emlib
 Author: Eduardo Moguillansky
 Author-email: eduardo.moguillansky@gmail.com
 License: BSD
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `emlib-1.8.1/README.rst` & `emlib-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `emlib-1.8.1/emlib/__init__.py` & `emlib-1.9.0/emlib/__init__.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.1/emlib/_dialogsqt.py` & `emlib-1.9.0/emlib/_dialogsqt.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.1/emlib/calculus.py` & `emlib-1.9.0/emlib/calculus.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.1/emlib/combinatorics.py` & `emlib-1.9.0/emlib/combinatorics.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.1/emlib/containers.py` & `emlib-1.9.0/emlib/containers.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.1/emlib/csvtools.py` & `emlib-1.9.0/emlib/csvtools.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.1/emlib/dialogs.py` & `emlib-1.9.0/emlib/dialogs.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.1/emlib/doctools.py` & `emlib-1.9.0/emlib/doctools.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.1/emlib/electronics.py` & `emlib-1.9.0/emlib/electronics.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.1/emlib/filetools.py` & `emlib-1.9.0/emlib/filetools.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.1/emlib/graphlib.py` & `emlib-1.9.0/emlib/graphlib.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.1/emlib/img.py` & `emlib-1.9.0/emlib/img.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.1/emlib/iterlib.py` & `emlib-1.9.0/emlib/iterlib.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.1/emlib/jsontools.py` & `emlib-1.9.0/emlib/jsontools.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.1/emlib/logutils.py` & `emlib-1.9.0/emlib/logutils.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.1/emlib/mathlib.py` & `emlib-1.9.0/emlib/mathlib.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.1/emlib/matplotting.py` & `emlib-1.9.0/emlib/matplotting.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.1/emlib/minizinctools.py` & `emlib-1.9.0/emlib/minizinctools.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.1/emlib/misc.py` & `emlib-1.9.0/emlib/misc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 """
 
 Miscellaneous functionality
 
 * **Search**: `nearest_element`, `nearest_unsorted`, `nearest_index`
 * **Sort**: `sort_natural`, `zipsort`, `issorted`
 * **Namedtuples**: `namedtupled_addcolumn`, `namedtuple_extend`, etc.
-* **IPython / Jupyter**: `inside_jupyter`, `is_interactive_session`, `session_type`
 * **Open files**: `open_with_standard_app`, `wait_for_file_modified`, `open_with`
 * **Unit conversions**: `cm_to_pixels`, `page_dinsize_to_mm`, etc.
-* **Other**: `runonce`, `singleton`
+* **Other**: `singleton`
 
 """
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 import os as _os
 import sys as _sys
 import math
 from bisect import bisect as _bisect
 from collections import namedtuple as _namedtuple
 import re as _re
 import dataclasses
-import warnings
 
 import numpy as np
 from fractions import Fraction
 import numbers
+from .envir import inside_jupyter
+
 
 from typing import TYPE_CHECKING
 if TYPE_CHECKING or 'sphinx' in _sys.modules:
     from typing import TypeVar, Sequence, Union, Optional, Callable, Any, Iterable
     T = TypeVar("T")
     T2 = TypeVar("T2")
     number_t = Union[float, numbers.Rational]
@@ -869,15 +869,16 @@
     if nearest:
         return t(round((x - offset) / tick)) * tick + offset
     else:
         return t(int((x - offset) / tick)) * tick + offset
 
 
 def snap_array(X: np.ndarray, tick:float, offset:float=0.,
-               out:Optional[np.ndarray]=None, nearest=True) -> np.ndarray:
+               out: Optional[np.ndarray] = None, nearest=True
+               ) -> np.ndarray:
     """
     Snap the values of X to the nearest slot in a grid
 
     Assuming a grid t defined by ``t(n) = offset + tick*n``, snap the values of X
     to the nearest value of t
 
     **NB**: tick > 0
@@ -898,15 +899,19 @@
         raise ValueError("tick should be > 0")
 
     if nearest:
         return _snap_array_nearest(X, tick, offset=float(offset), out=out)
     return _snap_array_floor(X, tick, offset=float(offset), out=out)
 
 
-def _snap_array_nearest(X: np.ndarray, tick: number_t, offset=0, out=None) -> np.ndarray:
+def _snap_array_nearest(X: np.ndarray, 
+                        tick: number_t, 
+                        offset: number_t = 0., 
+                        out: Optional[np.ndarray] = None
+                        ) -> np.ndarray:
     if out is None:
         out = X.copy()
     if offset != 0:
         out -= offset
         out /= tick
         out = np.round(out, out=out)
         out *= tick
@@ -914,16 +919,16 @@
     else:
         out /= tick
         out = np.round(out, out=out)
         out *= tick
     return out
 
 
-def _snap_array_floor(X: np.ndarray, tick:float, offset=0., out: np.ndarray=None) -> \
-        np.ndarray:
+def _snap_array_floor(X: np.ndarray, tick:float, offset=0., out: np.ndarray=None
+                      ) -> np.ndarray:
     arr = out if out is not None else X.copy()
     if offset != 0:
 
         arr -= offset
         arr /= tick
         arr = np.floor(arr, out=arr)
         arr *= tick
@@ -932,15 +937,15 @@
         arr /= tick
         arr = np.floor(arr, out=arr)
         arr *= tick
     return arr
 
 
 def snap_to_grids(x: number_t, ticks: Sequence[number_t], 
-                  offsets: Sequence[number_t]=None, mode='nearest'
+                  offsets: Sequence[number_t] = None, mode='nearest'
                   ) -> number_t:
     """
     Snap x to the nearest slot within multiple overlapping grids
 
     A regular grid is defined as ``x = offset + tick*n``, where ``n`` is an integer
     from -inf to inf.
 
@@ -1333,47 +1338,14 @@
     def get_instance():
         if cls not in instances:
             instances[cls] = cls()
         return instances[cls]
     return get_instance()
 
 
-class runonce:
-    """
-    To be used as decorator. `func` will run only once
-
-    Example::
-
-        # get_config() will only read the file the first time,
-        # return the resulting dict for any further calls
-
-        @runonce
-        def get_config():
-            config = json.load(open("/path/to/config.json"))
-            return config
-
-        config = get_config()
-
-    """
-    __slots__ = ('func', 'result', 'has_run')
-
-    def __init__(self, func):
-        self.func = func
-        self.result = None
-        self.has_run = False
-
-    def __call__(self, *args, **kwargs):
-        if self.has_run:
-            return self.result
-
-        self.result = self.func(*args, **kwargs)
-        self.has_run = True
-        return self.result
-
-
 # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 def istype(obj, *types) -> bool:
     """
     Examples::
 
         >>> istype(1, int, float)
@@ -1537,15 +1509,16 @@
         timeout: a timeout for wait_on_modified
     """
     if app is None:
         assert not shell
         _open_with_standard_app(path, wait=wait, min_wait=min_wait, timeout=timeout)
         return
 
-    import subprocess, time
+    import subprocess
+    import time
 
     if shell:
         assert isinstance(app, str), "shell needs a command-line as string"
         proc = subprocess.Popen(f'{app} "{path}"', shell=True)
     else:
         args = app if isinstance(app, list) else app.split()
         args.append(path)
@@ -1579,15 +1552,14 @@
 
     Returns:
         True if the file was modified, False if it wasn't or if the operation
         timed-out
     """
     from watchdog.observers import Observer
     from watchdog.events import PatternMatchingEventHandler
-    import time
     directory, base = _os.path.split(path)
     if not directory:
         directory = "."
     handler = PatternMatchingEventHandler([base], ignore_patterns="",
                                           ignore_directories=True, case_sensitive=True)
     observer = Observer()
     modified = False
@@ -1622,147 +1594,14 @@
     for p in paths:
         p = _os.path.expanduser(p)
         if _os.path.exists(p):
             return p
     return _os.path.expanduser(default)
 
 
-@runonce
-def inside_jupyter() -> bool:
-    """
-    Are we running inside a jupyter notebook?
-    """
-    return session_type() == 'jupyter'
-
-@runonce
-def inside_ipython() -> bool:
-    """
-    Are we running inside ipython?
-
-    This includes any ipython session (ipython in terminal, jupyter, etc.)
-    """
-    return session_type() in ('jupyter', 'ipython', 'ipython-terminal')
-
-
-@runonce
-def is_interactive_session() -> bool:
-    """ Are we running inside an interactive session? """
-    return _sys.flags.interactive == 1
-
-
-@runonce
-def session_type() -> str:
-    """
-    Returns the kind of python session
-
-    .. note::
-        See also `is_interactive_session` to check if we are inside a REPL
-
-    Returns:
-        Returns one of "jupyter", "ipython-terminal" (if running ipython
-        in a terminal), "ipython" (if running ipython outside of a terminal),
-        "python" if running normal python.
-
-    """
-    try:
-        # get_ipython should be available within an ipython/jupyter session
-        shell = get_ipython().__class__.__name__   # type: ignore
-        if shell == 'ZMQInteractiveShell':
-            return "jupyter"
-        elif shell == 'TerminalInteractiveShell':
-            return "ipython-terminal"
-        else:
-            return "ipython"
-    except NameError:
-        return "python"
-
-
-@runonce
-def running_inside_terminal() -> bool:
-    """
-    Are we running inside a terminal and not in the background?
-
-    """
-    return _sys.stdin and _sys.stdin.isatty()
-
-
-def ipython_qt_eventloop_started() -> bool:
-    """
-    Are we running ipython / jupyter and the qt event loop has been started?
-    ( %gui qt )
-    """
-    session = session_type()
-    if session == 'ipython-terminal' or session == 'jupyter':
-        # we are inside ipython so we can just call 'get_ipython'
-        ip = get_ipython()   # type: ignore
-        return ip.active_eventloop == "qt"
-    else:
-        return False
-
-
-def get_platform() -> tuple[str, str]:
-    """
-    Return a tuple (osname, architecture)
-
-    This attempts to improve upon `sysconfig.get_platform` by fixing some
-    issues when running a Python interpreter with a different architecture than
-    that of the system (e.g. 32bit on 64bit system, or a multiarch build),
-    which should return the machine architecture of the currently running
-    interpreter rather than that of the system (which didn't seem to work
-    properly). The reported machine architectures follow platform-specific
-    naming conventions (e.g. "x86_64" on Linux, but "x64" on Windows).
-
-    Returns:
-        a tuple (osname: str, architecture: str)
-
-
-    Example output strings for common platforms::
-
-        ("darwin", one of ppc|ppc64|i368|x86_64|arm64)
-        ("linux", one of i686|x86_64|armv7l|aarch64)
-        ("windows", one of x86|x64|arm32|arm64
-
-
-
-    """
-    import platform
-    import sysconfig
-
-    system = platform.system().lower()
-    machine = sysconfig.get_platform().split("-")[-1].lower()
-    is_64bit = _sys.maxsize > 2 ** 32
-
-    if system == "darwin": # get machine architecture of multiarch binaries
-        if any([x in machine for x in ("fat", "intel", "universal")]):
-            machine = platform.machine().lower()
-
-    elif system == "linux":  # fix running 32bit interpreter on 64bit system
-        if not is_64bit and machine == "x86_64":
-            machine = "i686"
-        elif not is_64bit and machine == "aarch64":
-            machine = "armv7l"
-
-    elif system == "windows": # return more precise machine architecture names
-        if machine == "amd64":
-            machine = "x64"
-        elif machine == "win32":
-            if is_64bit:
-                machine = platform.machine().lower()
-            else:
-                machine = "x86"
-
-    # some more fixes based on examples in https://en.wikipedia.org/wiki/Uname
-    if not is_64bit and machine in ("x86_64", "amd64"):
-        if any([x in system for x in ("cygwin", "mingw", "msys")]):
-            machine = "i686"
-        else:
-            machine = "i386"
-
-    return system, machine
-
 def html_table(rows: list, 
                headers: list[str], 
                maxwidths: Optional[list[int]]=None,
                rowstyles: Optional[list[str]]=None) -> str:
     """
     Create a html table
```

### Comparing `emlib-1.8.1/emlib/net.py` & `emlib-1.9.0/emlib/net.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.1/emlib/numberseries.py` & `emlib-1.9.0/emlib/numberseries.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.1/emlib/numpytools.py` & `emlib-1.9.0/emlib/numpytools.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.1/emlib/numtheory.py` & `emlib-1.9.0/emlib/numtheory.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.1/emlib/parabolicinterpol.py` & `emlib-1.9.0/emlib/parabolicinterpol.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.1/emlib/readbytes.py` & `emlib-1.9.0/emlib/readbytes.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.1/emlib/shelling.py` & `emlib-1.9.0/emlib/shelling.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.1/emlib/smooth.py` & `emlib-1.9.0/emlib/smooth.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.1/emlib/stochastic.py` & `emlib-1.9.0/emlib/stochastic.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.1/emlib/textlib.py` & `emlib-1.9.0/emlib/textlib.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.1/emlib/video.py` & `emlib-1.9.0/emlib/video.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.1/emlib/xmlprinter.py` & `emlib-1.9.0/emlib/xmlprinter.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.1/emlib.egg-info/PKG-INFO` & `emlib-1.9.0/emlib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emlib
-Version: 1.8.1
+Version: 1.9.0
 Summary: Miscellaneous utilities
 Home-page: https://github.com/gesellkammer/emlib
 Author: Eduardo Moguillansky
 Author-email: eduardo.moguillansky@gmail.com
 License: BSD
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `emlib-1.8.1/emlib.egg-info/SOURCES.txt` & `emlib-1.9.0/emlib.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 README.rst
 setup.cfg
 setup.py
 emlib/__init__.py
 emlib/_dialogsqt.py
 emlib/calculus.py
 emlib/combinatorics.py
+emlib/common.py
 emlib/containers.py
 emlib/csvtools.py
 emlib/dialogs.py
 emlib/doctools.py
 emlib/electronics.py
+emlib/envir.py
 emlib/filetools.py
 emlib/graphlib.py
 emlib/img.py
 emlib/iterlib.py
 emlib/jsontools.py
 emlib/logutils.py
 emlib/mathlib.py
```

### Comparing `emlib-1.8.1/setup.py` & `emlib-1.9.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-import os
-import sys
 
 from setuptools import setup
 
 readme = open('README.rst').read()
-version = (1, 8, 1)
+version = (1, 9, 0)
 
 setup(
     name='emlib',
     python_requires=">=3.9",
     version=".".join(map(str, version)),
     description='Miscellaneous utilities',
     long_description=readme,
```

