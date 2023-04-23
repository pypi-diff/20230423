# Comparing `tmp/gitopenlib-0.2.7.28.tar.gz` & `tmp/gitopenlib-0.2.8.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gitopenlib-0.2.7.28.tar", last modified: Tue Jan 10 12:58:35 2023, max compression
+gzip compressed data, was "dist/gitopenlib-0.2.8.28.tar", last modified: Sun Jan 15 14:39:13 2023, max compression
```

## Comparing `gitopenlib-0.2.7.28.tar` & `gitopenlib-0.2.8.28.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 sunjiajia   (501) staff       (20)        0 2023-01-10 12:58:35.197945 gitopenlib-0.2.7.28/
--rw-r--r--   0 sunjiajia   (501) staff       (20)     1064 2022-08-13 14:06:12.000000 gitopenlib-0.2.7.28/LICENSE
--rw-r--r--   0 sunjiajia   (501) staff       (20)      877 2023-01-10 12:58:35.197646 gitopenlib-0.2.7.28/PKG-INFO
--rw-r--r--   0 sunjiajia   (501) staff       (20)      211 2022-08-13 14:06:12.000000 gitopenlib-0.2.7.28/README.md
-drwxr-xr-x   0 sunjiajia   (501) staff       (20)        0 2023-01-10 12:58:35.184033 gitopenlib-0.2.7.28/gitopenlib/
--rw-r--r--   0 sunjiajia   (501) staff       (20)      189 2022-08-13 14:06:12.000000 gitopenlib-0.2.7.28/gitopenlib/__init__.py
-drwxr-xr-x   0 sunjiajia   (501) staff       (20)        0 2023-01-10 12:58:35.187739 gitopenlib-0.2.7.28/gitopenlib/helpers/
--rw-r--r--   0 sunjiajia   (501) staff       (20)      278 2022-08-13 14:06:12.000000 gitopenlib-0.2.7.28/gitopenlib/helpers/__init__.py
--rw-r--r--   0 sunjiajia   (501) staff       (20)     9242 2022-08-13 14:06:12.000000 gitopenlib-0.2.7.28/gitopenlib/helpers/mongo.py
--rw-r--r--   0 sunjiajia   (501) staff       (20)      642 2022-08-13 14:06:12.000000 gitopenlib-0.2.7.28/gitopenlib/helpers/networks.py
-drwxr-xr-x   0 sunjiajia   (501) staff       (20)        0 2023-01-10 12:58:35.189657 gitopenlib-0.2.7.28/gitopenlib/indicators/
--rw-r--r--   0 sunjiajia   (501) staff       (20)      189 2022-08-13 14:06:12.000000 gitopenlib-0.2.7.28/gitopenlib/indicators/__init__.py
--rw-r--r--   0 sunjiajia   (501) staff       (20)     5548 2022-08-13 14:06:12.000000 gitopenlib-0.2.7.28/gitopenlib/indicators/diversity.py
--rw-r--r--   0 sunjiajia   (501) staff       (20)     1997 2022-08-13 14:06:12.000000 gitopenlib-0.2.7.28/gitopenlib/indicators/entropy_weight_method.py
--rw-r--r--   0 sunjiajia   (501) staff       (20)    20969 2022-08-13 14:06:12.000000 gitopenlib-0.2.7.28/gitopenlib/indicators/statistics.py
--rw-r--r--   0 sunjiajia   (501) staff       (20)     1418 2022-09-17 03:36:04.000000 gitopenlib-0.2.7.28/gitopenlib/libs.py
-drwxr-xr-x   0 sunjiajia   (501) staff       (20)        0 2023-01-10 12:58:35.196845 gitopenlib-0.2.7.28/gitopenlib/utils/
--rw-r--r--   0 sunjiajia   (501) staff       (20)      266 2022-08-13 14:06:12.000000 gitopenlib-0.2.7.28/gitopenlib/utils/__init__.py
--rw-r--r--   0 sunjiajia   (501) staff       (20)     3316 2022-09-18 23:47:01.000000 gitopenlib-0.2.7.28/gitopenlib/utils/ai.py
--rw-r--r--   0 sunjiajia   (501) staff       (20)    12238 2023-01-04 17:11:24.000000 gitopenlib-0.2.7.28/gitopenlib/utils/basics.py
--rw-r--r--   0 sunjiajia   (501) staff       (20)      840 2022-09-28 08:25:43.000000 gitopenlib-0.2.7.28/gitopenlib/utils/clazz.py
--rw-r--r--   0 sunjiajia   (501) staff       (20)     5991 2022-08-13 14:06:12.000000 gitopenlib-0.2.7.28/gitopenlib/utils/comatrix.py
--rw-r--r--   0 sunjiajia   (501) staff       (20)      769 2022-08-13 14:06:12.000000 gitopenlib-0.2.7.28/gitopenlib/utils/crawler.py
--rw-r--r--   0 sunjiajia   (501) staff       (20)      692 2022-12-09 13:32:51.000000 gitopenlib-0.2.7.28/gitopenlib/utils/debuger.py
--rw-r--r--   0 sunjiajia   (501) staff       (20)    12950 2023-01-04 17:07:52.000000 gitopenlib-0.2.7.28/gitopenlib/utils/files.py
--rw-r--r--   0 sunjiajia   (501) staff       (20)     1490 2022-08-13 14:11:29.000000 gitopenlib-0.2.7.28/gitopenlib/utils/get_ip.py
--rw-r--r--   0 sunjiajia   (501) staff       (20)     9860 2022-08-13 14:06:12.000000 gitopenlib-0.2.7.28/gitopenlib/utils/k_cluster.py
--rw-r--r--   0 sunjiajia   (501) staff       (20)     5684 2022-08-13 14:06:12.000000 gitopenlib-0.2.7.28/gitopenlib/utils/nlp.py
--rw-r--r--   0 sunjiajia   (501) staff       (20)     3785 2022-08-13 14:06:12.000000 gitopenlib-0.2.7.28/gitopenlib/utils/others.py
--rw-r--r--   0 sunjiajia   (501) staff       (20)     1820 2022-08-13 14:06:12.000000 gitopenlib-0.2.7.28/gitopenlib/utils/parser.py
--rw-r--r--   0 sunjiajia   (501) staff       (20)     4413 2022-11-07 14:52:49.000000 gitopenlib-0.2.7.28/gitopenlib/utils/plot.py
--rw-r--r--   0 sunjiajia   (501) staff       (20)     7733 2022-08-13 14:06:12.000000 gitopenlib-0.2.7.28/gitopenlib/utils/sorts.py
--rw-r--r--   0 sunjiajia   (501) staff       (20)     4017 2023-01-10 12:57:50.000000 gitopenlib-0.2.7.28/gitopenlib/utils/wonders.py
-drwxr-xr-x   0 sunjiajia   (501) staff       (20)        0 2023-01-10 12:58:35.185797 gitopenlib-0.2.7.28/gitopenlib.egg-info/
--rw-r--r--   0 sunjiajia   (501) staff       (20)      877 2023-01-10 12:58:35.000000 gitopenlib-0.2.7.28/gitopenlib.egg-info/PKG-INFO
--rw-r--r--   0 sunjiajia   (501) staff       (20)      876 2023-01-10 12:58:35.000000 gitopenlib-0.2.7.28/gitopenlib.egg-info/SOURCES.txt
--rw-r--r--   0 sunjiajia   (501) staff       (20)        1 2023-01-10 12:58:35.000000 gitopenlib-0.2.7.28/gitopenlib.egg-info/dependency_links.txt
--rw-r--r--   0 sunjiajia   (501) staff       (20)       11 2023-01-10 12:58:35.000000 gitopenlib-0.2.7.28/gitopenlib.egg-info/top_level.txt
--rw-r--r--   0 sunjiajia   (501) staff       (20)       38 2023-01-10 12:58:35.198052 gitopenlib-0.2.7.28/setup.cfg
--rw-r--r--   0 sunjiajia   (501) staff       (20)     4143 2023-01-10 12:58:05.000000 gitopenlib-0.2.7.28/setup.py
+drwxr-xr-x   0 sunjiajia   (501) staff       (20)        0 2023-01-15 14:39:13.121372 gitopenlib-0.2.8.28/
+-rw-r--r--   0 sunjiajia   (501) staff       (20)     1064 2022-08-13 14:06:12.000000 gitopenlib-0.2.8.28/LICENSE
+-rw-r--r--   0 sunjiajia   (501) staff       (20)      877 2023-01-15 14:39:13.120346 gitopenlib-0.2.8.28/PKG-INFO
+-rw-r--r--   0 sunjiajia   (501) staff       (20)      211 2022-08-13 14:06:12.000000 gitopenlib-0.2.8.28/README.md
+drwxr-xr-x   0 sunjiajia   (501) staff       (20)        0 2023-01-15 14:39:13.106318 gitopenlib-0.2.8.28/gitopenlib/
+-rw-r--r--   0 sunjiajia   (501) staff       (20)      189 2022-08-13 14:06:12.000000 gitopenlib-0.2.8.28/gitopenlib/__init__.py
+drwxr-xr-x   0 sunjiajia   (501) staff       (20)        0 2023-01-15 14:39:13.108529 gitopenlib-0.2.8.28/gitopenlib/helpers/
+-rw-r--r--   0 sunjiajia   (501) staff       (20)      278 2022-08-13 14:06:12.000000 gitopenlib-0.2.8.28/gitopenlib/helpers/__init__.py
+-rw-r--r--   0 sunjiajia   (501) staff       (20)     9242 2022-08-13 14:06:12.000000 gitopenlib-0.2.8.28/gitopenlib/helpers/mongo.py
+-rw-r--r--   0 sunjiajia   (501) staff       (20)      642 2022-08-13 14:06:12.000000 gitopenlib-0.2.8.28/gitopenlib/helpers/networks.py
+drwxr-xr-x   0 sunjiajia   (501) staff       (20)        0 2023-01-15 14:39:13.109851 gitopenlib-0.2.8.28/gitopenlib/indicators/
+-rw-r--r--   0 sunjiajia   (501) staff       (20)      189 2022-08-13 14:06:12.000000 gitopenlib-0.2.8.28/gitopenlib/indicators/__init__.py
+-rw-r--r--   0 sunjiajia   (501) staff       (20)     5548 2022-08-13 14:06:12.000000 gitopenlib-0.2.8.28/gitopenlib/indicators/diversity.py
+-rw-r--r--   0 sunjiajia   (501) staff       (20)     1997 2022-08-13 14:06:12.000000 gitopenlib-0.2.8.28/gitopenlib/indicators/entropy_weight_method.py
+-rw-r--r--   0 sunjiajia   (501) staff       (20)    20969 2022-08-13 14:06:12.000000 gitopenlib-0.2.8.28/gitopenlib/indicators/statistics.py
+-rw-r--r--   0 sunjiajia   (501) staff       (20)     1418 2022-09-17 03:36:04.000000 gitopenlib-0.2.8.28/gitopenlib/libs.py
+drwxr-xr-x   0 sunjiajia   (501) staff       (20)        0 2023-01-15 14:39:13.118268 gitopenlib-0.2.8.28/gitopenlib/utils/
+-rw-r--r--   0 sunjiajia   (501) staff       (20)      266 2022-08-13 14:06:12.000000 gitopenlib-0.2.8.28/gitopenlib/utils/__init__.py
+-rw-r--r--   0 sunjiajia   (501) staff       (20)     3316 2022-09-18 23:47:01.000000 gitopenlib-0.2.8.28/gitopenlib/utils/ai.py
+-rw-r--r--   0 sunjiajia   (501) staff       (20)    12238 2023-01-04 17:11:24.000000 gitopenlib-0.2.8.28/gitopenlib/utils/basics.py
+-rw-r--r--   0 sunjiajia   (501) staff       (20)      840 2022-09-28 08:25:43.000000 gitopenlib-0.2.8.28/gitopenlib/utils/clazz.py
+-rw-r--r--   0 sunjiajia   (501) staff       (20)     5991 2022-08-13 14:06:12.000000 gitopenlib-0.2.8.28/gitopenlib/utils/comatrix.py
+-rw-r--r--   0 sunjiajia   (501) staff       (20)      769 2022-08-13 14:06:12.000000 gitopenlib-0.2.8.28/gitopenlib/utils/crawler.py
+-rw-r--r--   0 sunjiajia   (501) staff       (20)      692 2022-12-09 13:32:51.000000 gitopenlib-0.2.8.28/gitopenlib/utils/debuger.py
+-rw-r--r--   0 sunjiajia   (501) staff       (20)    12950 2023-01-04 17:07:52.000000 gitopenlib-0.2.8.28/gitopenlib/utils/files.py
+-rw-r--r--   0 sunjiajia   (501) staff       (20)     1490 2022-08-13 14:11:29.000000 gitopenlib-0.2.8.28/gitopenlib/utils/get_ip.py
+-rw-r--r--   0 sunjiajia   (501) staff       (20)     9860 2022-08-13 14:06:12.000000 gitopenlib-0.2.8.28/gitopenlib/utils/k_cluster.py
+-rw-r--r--   0 sunjiajia   (501) staff       (20)     5684 2022-08-13 14:06:12.000000 gitopenlib-0.2.8.28/gitopenlib/utils/nlp.py
+-rw-r--r--   0 sunjiajia   (501) staff       (20)     3785 2022-08-13 14:06:12.000000 gitopenlib-0.2.8.28/gitopenlib/utils/others.py
+-rw-r--r--   0 sunjiajia   (501) staff       (20)     1820 2022-08-13 14:06:12.000000 gitopenlib-0.2.8.28/gitopenlib/utils/parser.py
+-rw-r--r--   0 sunjiajia   (501) staff       (20)     4685 2023-01-15 14:38:14.000000 gitopenlib-0.2.8.28/gitopenlib/utils/plot.py
+-rw-r--r--   0 sunjiajia   (501) staff       (20)     7733 2022-08-13 14:06:12.000000 gitopenlib-0.2.8.28/gitopenlib/utils/sorts.py
+-rw-r--r--   0 sunjiajia   (501) staff       (20)     4017 2023-01-10 12:57:50.000000 gitopenlib-0.2.8.28/gitopenlib/utils/wonders.py
+drwxr-xr-x   0 sunjiajia   (501) staff       (20)        0 2023-01-15 14:39:13.107614 gitopenlib-0.2.8.28/gitopenlib.egg-info/
+-rw-r--r--   0 sunjiajia   (501) staff       (20)      877 2023-01-15 14:39:13.000000 gitopenlib-0.2.8.28/gitopenlib.egg-info/PKG-INFO
+-rw-r--r--   0 sunjiajia   (501) staff       (20)      876 2023-01-15 14:39:13.000000 gitopenlib-0.2.8.28/gitopenlib.egg-info/SOURCES.txt
+-rw-r--r--   0 sunjiajia   (501) staff       (20)        1 2023-01-15 14:39:13.000000 gitopenlib-0.2.8.28/gitopenlib.egg-info/dependency_links.txt
+-rw-r--r--   0 sunjiajia   (501) staff       (20)       11 2023-01-15 14:39:13.000000 gitopenlib-0.2.8.28/gitopenlib.egg-info/top_level.txt
+-rw-r--r--   0 sunjiajia   (501) staff       (20)       38 2023-01-15 14:39:13.121801 gitopenlib-0.2.8.28/setup.cfg
+-rw-r--r--   0 sunjiajia   (501) staff       (20)     4143 2023-01-15 14:38:26.000000 gitopenlib-0.2.8.28/setup.py
```

### Comparing `gitopenlib-0.2.7.28/LICENSE` & `gitopenlib-0.2.8.28/LICENSE`

 * *Files identical despite different names*

### Comparing `gitopenlib-0.2.7.28/PKG-INFO` & `gitopenlib-0.2.8.28/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitopenlib
-Version: 0.2.7.28
+Version: 0.2.8.28
 Summary: A library containing some useful functions. Powered by GitOPEN.
 Home-page: https://github.com/opengit/gitopenlib.git
 Author: gitopen
 Author-email: gitopen@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `gitopenlib-0.2.7.28/gitopenlib/helpers/mongo.py` & `gitopenlib-0.2.8.28/gitopenlib/helpers/mongo.py`

 * *Files identical despite different names*

### Comparing `gitopenlib-0.2.7.28/gitopenlib/helpers/networks.py` & `gitopenlib-0.2.8.28/gitopenlib/helpers/networks.py`

 * *Files identical despite different names*

### Comparing `gitopenlib-0.2.7.28/gitopenlib/indicators/diversity.py` & `gitopenlib-0.2.8.28/gitopenlib/indicators/diversity.py`

 * *Files identical despite different names*

### Comparing `gitopenlib-0.2.7.28/gitopenlib/indicators/entropy_weight_method.py` & `gitopenlib-0.2.8.28/gitopenlib/indicators/entropy_weight_method.py`

 * *Files identical despite different names*

### Comparing `gitopenlib-0.2.7.28/gitopenlib/indicators/statistics.py` & `gitopenlib-0.2.8.28/gitopenlib/indicators/statistics.py`

 * *Files identical despite different names*

### Comparing `gitopenlib-0.2.7.28/gitopenlib/libs.py` & `gitopenlib-0.2.8.28/gitopenlib/libs.py`

 * *Files identical despite different names*

### Comparing `gitopenlib-0.2.7.28/gitopenlib/utils/ai.py` & `gitopenlib-0.2.8.28/gitopenlib/utils/ai.py`

 * *Files identical despite different names*

### Comparing `gitopenlib-0.2.7.28/gitopenlib/utils/basics.py` & `gitopenlib-0.2.8.28/gitopenlib/utils/basics.py`

 * *Files identical despite different names*

### Comparing `gitopenlib-0.2.7.28/gitopenlib/utils/clazz.py` & `gitopenlib-0.2.8.28/gitopenlib/utils/clazz.py`

 * *Files identical despite different names*

### Comparing `gitopenlib-0.2.7.28/gitopenlib/utils/comatrix.py` & `gitopenlib-0.2.8.28/gitopenlib/utils/comatrix.py`

 * *Files identical despite different names*

### Comparing `gitopenlib-0.2.7.28/gitopenlib/utils/crawler.py` & `gitopenlib-0.2.8.28/gitopenlib/utils/crawler.py`

 * *Files identical despite different names*

### Comparing `gitopenlib-0.2.7.28/gitopenlib/utils/debuger.py` & `gitopenlib-0.2.8.28/gitopenlib/utils/debuger.py`

 * *Files identical despite different names*

### Comparing `gitopenlib-0.2.7.28/gitopenlib/utils/files.py` & `gitopenlib-0.2.8.28/gitopenlib/utils/files.py`

 * *Files identical despite different names*

### Comparing `gitopenlib-0.2.7.28/gitopenlib/utils/get_ip.py` & `gitopenlib-0.2.8.28/gitopenlib/utils/get_ip.py`

 * *Files identical despite different names*

### Comparing `gitopenlib-0.2.7.28/gitopenlib/utils/k_cluster.py` & `gitopenlib-0.2.8.28/gitopenlib/utils/k_cluster.py`

 * *Files identical despite different names*

### Comparing `gitopenlib-0.2.7.28/gitopenlib/utils/nlp.py` & `gitopenlib-0.2.8.28/gitopenlib/utils/nlp.py`

 * *Files identical despite different names*

### Comparing `gitopenlib-0.2.7.28/gitopenlib/utils/others.py` & `gitopenlib-0.2.8.28/gitopenlib/utils/others.py`

 * *Files identical despite different names*

### Comparing `gitopenlib-0.2.7.28/gitopenlib/utils/parser.py` & `gitopenlib-0.2.8.28/gitopenlib/utils/parser.py`

 * *Files identical despite different names*

### Comparing `gitopenlib-0.2.7.28/gitopenlib/utils/plot.py` & `gitopenlib-0.2.8.28/gitopenlib/utils/plot.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,26 +4,34 @@
 # Copyright (c) 2021
 # @Author :  GitOPEN
 # @Email  :  gitopen@gmail.com
 # @Date   :  2021-05-22 17:08:35
 # @Description :  一些画图的相关工具函数
 
 
-__version__ = "0.7.5.2"
+__version__ = "0.7.6.2"
 
 
 from matplotlib import ticker
 from matplotlib.axes import Axes
 from matplotlib.offsetbox import AnchoredText
 import matplotlib.pyplot as plt
 from matplotlib.ticker import MaxNLocator
 
 from gitopenlib.utils import files as gf
 
 
+def set_spines_line_width(ax: Axes, left, top, right, bottom):
+    """设置坐标轴的粗细"""
+    ax.spines["left"].set_linewidth(left)
+    ax.spines["top"].set_linewidth(top)
+    ax.spines["right"].set_linewidth(right)
+    ax.spines["bottom"].set_linewidth(bottom)
+
+
 def set_figsize(width: float or int = 4, height: float or int = 3):
     """设置图片的大小，单位为英寸"""
     pt.rcParams["figure.figsize"] = (width, height)
 
 
 def save_svg(plt, path: str, dpi: int = 300, backup: bool = True):
     """保存为svg格式的矢量图。
```

### Comparing `gitopenlib-0.2.7.28/gitopenlib/utils/sorts.py` & `gitopenlib-0.2.8.28/gitopenlib/utils/sorts.py`

 * *Files identical despite different names*

### Comparing `gitopenlib-0.2.7.28/gitopenlib/utils/wonders.py` & `gitopenlib-0.2.8.28/gitopenlib/utils/wonders.py`

 * *Files identical despite different names*

### Comparing `gitopenlib-0.2.7.28/gitopenlib.egg-info/PKG-INFO` & `gitopenlib-0.2.8.28/gitopenlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitopenlib
-Version: 0.2.7.28
+Version: 0.2.8.28
 Summary: A library containing some useful functions. Powered by GitOPEN.
 Home-page: https://github.com/opengit/gitopenlib.git
 Author: gitopen
 Author-email: gitopen@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `gitopenlib-0.2.7.28/gitopenlib.egg-info/SOURCES.txt` & `gitopenlib-0.2.8.28/gitopenlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gitopenlib-0.2.7.28/setup.py` & `gitopenlib-0.2.8.28/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # Package meta-data.
 NAME = "gitopenlib"
 DESCRIPTION = "A library containing some useful functions. Powered by GitOPEN."
 URL = "https://github.com/opengit/gitopenlib.git"
 EMAIL = "gitopen@gmail.com"
 AUTHOR = "gitopen"
 REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "0.2.07.28"
+VERSION = "0.2.08.28"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     #  "scikit-learn",
     #  "pandas",
     #  "matplotlib",
     #  "tqdm",
```

