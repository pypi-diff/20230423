# Comparing `tmp/spagrn-1.0.2.tar.gz` & `tmp/spagrn-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spagrn-1.0.2.tar", last modified: Sun Apr 23 10:28:21 2023, max compression
+gzip compressed data, was "spagrn-1.0.3.tar", last modified: Sun Apr 23 10:43:30 2023, max compression
```

## Comparing `spagrn-1.0.2.tar` & `spagrn-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 yao        (502) staff       (20)        0 2023-04-23 10:28:21.098391 spagrn-1.0.2/
--rw-r--r--   0 yao        (502) staff       (20)    35149 2023-04-11 12:27:22.000000 spagrn-1.0.2/LICENSE
--rw-r--r--   0 yao        (502) staff       (20)      627 2023-04-23 10:28:21.098441 spagrn-1.0.2/PKG-INFO
--rw-r--r--   0 yao        (502) staff       (20)     3617 2023-04-23 10:09:19.000000 spagrn-1.0.2/README.md
--rw-r--r--   0 yao        (502) staff       (20)       79 2023-04-23 10:28:21.098631 spagrn-1.0.2/setup.cfg
--rw-r--r--   0 yao        (502) staff       (20)      972 2023-04-23 10:28:11.000000 spagrn-1.0.2/setup.py
-drwxr-xr-x   0 yao        (502) staff       (20)        0 2023-04-23 10:28:21.097683 spagrn-1.0.2/spagrn/
--rw-r--r--   0 yao        (502) staff       (20)      282 2023-04-21 12:16:13.000000 spagrn-1.0.2/spagrn/__init__.py
--rw-r--r--   0 yao        (502) staff       (20)    13782 2023-04-21 12:16:13.000000 spagrn-1.0.2/spagrn/plot.py
--rw-r--r--   0 yao        (502) staff       (20)    39463 2023-04-21 12:16:13.000000 spagrn-1.0.2/spagrn/regulatory_network.py
--rw-r--r--   0 yao        (502) staff       (20)     1202 2023-04-08 12:20:26.000000 spagrn-1.0.2/spagrn/spa_logger.py
--rw-r--r--   0 yao        (502) staff       (20)     1867 2023-04-08 12:23:27.000000 spagrn-1.0.2/spagrn/test.py
-drwxr-xr-x   0 yao        (502) staff       (20)        0 2023-04-23 10:28:21.098307 spagrn-1.0.2/spagrn.egg-info/
--rw-r--r--   0 yao        (502) staff       (20)      627 2023-04-23 10:28:21.000000 spagrn-1.0.2/spagrn.egg-info/PKG-INFO
--rw-r--r--   0 yao        (502) staff       (20)      284 2023-04-23 10:28:21.000000 spagrn-1.0.2/spagrn.egg-info/SOURCES.txt
--rw-r--r--   0 yao        (502) staff       (20)        1 2023-04-23 10:28:21.000000 spagrn-1.0.2/spagrn.egg-info/dependency_links.txt
--rw-r--r--   0 yao        (502) staff       (20)      162 2023-04-23 10:28:21.000000 spagrn-1.0.2/spagrn.egg-info/requires.txt
--rw-r--r--   0 yao        (502) staff       (20)        7 2023-04-23 10:28:21.000000 spagrn-1.0.2/spagrn.egg-info/top_level.txt
+drwxr-xr-x   0 yao        (502) staff       (20)        0 2023-04-23 10:43:30.546115 spagrn-1.0.3/
+-rw-r--r--   0 yao        (502) staff       (20)    35149 2023-04-11 12:27:22.000000 spagrn-1.0.3/LICENSE
+-rw-r--r--   0 yao        (502) staff       (20)      627 2023-04-23 10:43:30.546161 spagrn-1.0.3/PKG-INFO
+-rw-r--r--   0 yao        (502) staff       (20)     3617 2023-04-23 10:09:19.000000 spagrn-1.0.3/README.md
+-rw-r--r--   0 yao        (502) staff       (20)       79 2023-04-23 10:43:30.546359 spagrn-1.0.3/setup.cfg
+-rw-r--r--   0 yao        (502) staff       (20)     1168 2023-04-23 10:43:27.000000 spagrn-1.0.3/setup.py
+drwxr-xr-x   0 yao        (502) staff       (20)        0 2023-04-23 10:43:30.545371 spagrn-1.0.3/spagrn/
+-rw-r--r--   0 yao        (502) staff       (20)      282 2023-04-21 12:16:13.000000 spagrn-1.0.3/spagrn/__init__.py
+-rw-r--r--   0 yao        (502) staff       (20)    13782 2023-04-21 12:16:13.000000 spagrn-1.0.3/spagrn/plot.py
+-rw-r--r--   0 yao        (502) staff       (20)    39463 2023-04-21 12:16:13.000000 spagrn-1.0.3/spagrn/regulatory_network.py
+-rw-r--r--   0 yao        (502) staff       (20)     1202 2023-04-08 12:20:26.000000 spagrn-1.0.3/spagrn/spa_logger.py
+-rw-r--r--   0 yao        (502) staff       (20)     1867 2023-04-08 12:23:27.000000 spagrn-1.0.3/spagrn/test.py
+drwxr-xr-x   0 yao        (502) staff       (20)        0 2023-04-23 10:43:30.546026 spagrn-1.0.3/spagrn.egg-info/
+-rw-r--r--   0 yao        (502) staff       (20)      627 2023-04-23 10:43:30.000000 spagrn-1.0.3/spagrn.egg-info/PKG-INFO
+-rw-r--r--   0 yao        (502) staff       (20)      284 2023-04-23 10:43:30.000000 spagrn-1.0.3/spagrn.egg-info/SOURCES.txt
+-rw-r--r--   0 yao        (502) staff       (20)        1 2023-04-23 10:43:30.000000 spagrn-1.0.3/spagrn.egg-info/dependency_links.txt
+-rw-r--r--   0 yao        (502) staff       (20)      138 2023-04-23 10:43:30.000000 spagrn-1.0.3/spagrn.egg-info/requires.txt
+-rw-r--r--   0 yao        (502) staff       (20)        7 2023-04-23 10:43:30.000000 spagrn-1.0.3/spagrn.egg-info/top_level.txt
```

### Comparing `spagrn-1.0.2/LICENSE` & `spagrn-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spagrn-1.0.2/PKG-INFO` & `spagrn-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spagrn
-Version: 1.0.2
+Version: 1.0.3
 Summary: A comprehensive tool to infer TF-centered, spatial gene regulatory networks for the spatially resolved transcriptomic data.
 Home-page: https://github.com/BGI-Qingdao/SpaGRN
 Author: Yao LI, Lidong GUO, Mengyang XU
 Author-email: liyao1@genomics.cn, guolidong@genomics.cn, xumengyang@genomics.cn
 License: GPL-3.0+
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `spagrn-1.0.2/README.md` & `spagrn-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `spagrn-1.0.2/setup.py` & `spagrn-1.0.3/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,23 +2,35 @@
 import setuptools
 import glob
 import os
 from pathlib import Path
 
 setuptools.setup(
     name="spagrn",
-    version="1.0.2",
+    version="1.0.3",
     author="Yao LI, Lidong GUO, Mengyang XU",
     author_email="liyao1@genomics.cn, guolidong@genomics.cn, xumengyang@genomics.cn",
     url="https://github.com/BGI-Qingdao/SpaGRN",
     #long_description=Path('README.md').read_text('utf-8'),
     python_requires=">=3.7,<3.11",
     packages=setuptools.find_packages(),
     install_requires=[
-        l.strip() for l in Path('requirements.txt').read_text('utf-8').splitlines()
+        "anndata==0.8.0",
+        "pandas>=1.3.5",
+        "scanpy",
+        "seaborn",
+        "matplotlib",
+        "pyscenic==0.12.1",
+        "hotspotsc==1.1.1",
+        "scipy",
+        "numpy",
+        "dask",
+        "arboreto",
+        "ctxcore>=0.2.0",
+        "sklearn"
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         "Operating System :: OS Independent",
     ],
     license="GPL-3.0+",
```

### Comparing `spagrn-1.0.2/spagrn/plot.py` & `spagrn-1.0.3/spagrn/plot.py`

 * *Files identical despite different names*

### Comparing `spagrn-1.0.2/spagrn/regulatory_network.py` & `spagrn-1.0.3/spagrn/regulatory_network.py`

 * *Files identical despite different names*

### Comparing `spagrn-1.0.2/spagrn/spa_logger.py` & `spagrn-1.0.3/spagrn/spa_logger.py`

 * *Files identical despite different names*

### Comparing `spagrn-1.0.2/spagrn/test.py` & `spagrn-1.0.3/spagrn/test.py`

 * *Files identical despite different names*

### Comparing `spagrn-1.0.2/spagrn.egg-info/PKG-INFO` & `spagrn-1.0.3/spagrn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spagrn
-Version: 1.0.2
+Version: 1.0.3
 Summary: A comprehensive tool to infer TF-centered, spatial gene regulatory networks for the spatially resolved transcriptomic data.
 Home-page: https://github.com/BGI-Qingdao/SpaGRN
 Author: Yao LI, Lidong GUO, Mengyang XU
 Author-email: liyao1@genomics.cn, guolidong@genomics.cn, xumengyang@genomics.cn
 License: GPL-3.0+
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

