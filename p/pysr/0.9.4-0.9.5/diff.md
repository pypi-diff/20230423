# Comparing `tmp/pysr-0.9.4.tar.gz` & `tmp/pysr-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysr-0.9.4.tar", last modified: Fri Jul  8 22:45:39 2022, max compression
+gzip compressed data, was "pysr-0.9.5.tar", last modified: Sat Jul  9 20:38:35 2022, max compression
```

## Comparing `pysr-0.9.4.tar` & `pysr-0.9.5.tar`

### file list

```diff
@@ -1,31 +1,29 @@
-drwxr-xr-x   0 mcranmer   (504) staff       (20)        0 2022-07-08 22:45:39.082820 pysr-0.9.4/
--rw-r--r--   0 mcranmer   (504) staff       (20)    11343 2022-02-01 21:21:09.000000 pysr-0.9.4/LICENSE
--rw-r--r--   0 mcranmer   (504) staff       (20)    11968 2022-07-08 22:45:39.082642 pysr-0.9.4/PKG-INFO
--rw-r--r--   0 mcranmer   (504) staff       (20)    11544 2022-06-21 22:44:34.000000 pysr-0.9.4/README.md
-drwxr-xr-x   0 mcranmer   (504) staff       (20)        0 2022-07-08 22:45:39.081400 pysr-0.9.4/datasets/
--rw-r--r--   0 mcranmer   (504) staff       (20)     9433 2022-02-01 21:21:09.000000 pysr-0.9.4/datasets/FeynmanEquations.csv
-drwxr-xr-x   0 mcranmer   (504) staff       (20)        0 2022-07-08 22:45:39.080590 pysr-0.9.4/pysr/
--rw-r--r--   0 mcranmer   (504) staff       (20)      300 2022-06-16 01:31:36.000000 pysr-0.9.4/pysr/__init__.py
--rw-r--r--   0 mcranmer   (504) staff       (20)     1358 2022-06-04 20:52:09.000000 pysr-0.9.4/pysr/deprecated.py
--rw-r--r--   0 mcranmer   (504) staff       (20)     6320 2022-06-21 23:59:39.000000 pysr-0.9.4/pysr/export_jax.py
--rw-r--r--   0 mcranmer   (504) staff       (20)     1488 2022-06-16 01:31:36.000000 pysr-0.9.4/pysr/export_numpy.py
--rw-r--r--   0 mcranmer   (504) staff       (20)     7576 2022-06-21 23:58:48.000000 pysr-0.9.4/pysr/export_torch.py
--rw-r--r--   0 mcranmer   (504) staff       (20)     5615 2022-02-01 21:21:09.000000 pysr-0.9.4/pysr/feynman_problems.py
--rw-r--r--   0 mcranmer   (504) staff       (20)     3763 2022-06-20 01:18:33.000000 pysr-0.9.4/pysr/julia_helpers.py
--rw-r--r--   0 mcranmer   (504) staff       (20)    79972 2022-07-08 22:43:11.000000 pysr-0.9.4/pysr/sr.py
--rw-r--r--   0 mcranmer   (504) staff       (20)      692 2022-06-20 07:08:14.000000 pysr-0.9.4/pysr/tmp.py
--rw-r--r--   0 mcranmer   (504) staff       (20)       67 2022-07-08 22:44:57.000000 pysr-0.9.4/pysr/version.py
-drwxr-xr-x   0 mcranmer   (504) staff       (20)        0 2022-07-08 22:45:39.081270 pysr-0.9.4/pysr.egg-info/
--rw-r--r--   0 mcranmer   (504) staff       (20)    11968 2022-07-08 22:45:38.000000 pysr-0.9.4/pysr.egg-info/PKG-INFO
--rw-r--r--   0 mcranmer   (504) staff       (20)      464 2022-07-08 22:45:38.000000 pysr-0.9.4/pysr.egg-info/SOURCES.txt
--rw-r--r--   0 mcranmer   (504) staff       (20)        1 2022-07-08 22:45:38.000000 pysr-0.9.4/pysr.egg-info/dependency_links.txt
--rw-r--r--   0 mcranmer   (504) staff       (20)       52 2022-07-08 22:45:38.000000 pysr-0.9.4/pysr.egg-info/requires.txt
--rw-r--r--   0 mcranmer   (504) staff       (20)       10 2022-07-08 22:45:38.000000 pysr-0.9.4/pysr.egg-info/top_level.txt
--rw-r--r--   0 mcranmer   (504) staff       (20)       38 2022-07-08 22:45:39.082867 pysr-0.9.4/setup.cfg
--rw-r--r--   0 mcranmer   (504) staff       (20)      947 2022-06-22 23:17:41.000000 pysr-0.9.4/setup.py
-drwxr-xr-x   0 mcranmer   (504) staff       (20)        0 2022-07-08 22:45:39.082134 pysr-0.9.4/test/
--rw-r--r--   0 mcranmer   (504) staff       (20)        0 2022-02-01 21:21:09.000000 pysr-0.9.4/test/__init__.py
--rw-r--r--   0 mcranmer   (504) staff       (20)    18928 2022-07-08 22:42:13.000000 pysr-0.9.4/test/test.py
--rw-r--r--   0 mcranmer   (504) staff       (20)     3719 2022-06-21 23:51:25.000000 pysr-0.9.4/test/test_jax.py
--rw-r--r--   0 mcranmer   (504) staff       (20)     6044 2022-07-02 03:09:41.000000 pysr-0.9.4/test/test_torch.py
--rw-r--r--   0 mcranmer   (504) staff       (20)      401 2022-04-01 00:01:13.000000 pysr-0.9.4/test/tmp.py
+drwxr-xr-x   0 mcranmer   (504) staff       (20)        0 2022-07-09 20:38:35.879252 pysr-0.9.5/
+-rw-r--r--   0 mcranmer   (504) staff       (20)    11343 2022-02-01 21:21:09.000000 pysr-0.9.5/LICENSE
+-rw-r--r--   0 mcranmer   (504) staff       (20)    11968 2022-07-09 20:38:35.879044 pysr-0.9.5/PKG-INFO
+-rw-r--r--   0 mcranmer   (504) staff       (20)    11544 2022-06-21 22:44:34.000000 pysr-0.9.5/README.md
+drwxr-xr-x   0 mcranmer   (504) staff       (20)        0 2022-07-09 20:38:35.877847 pysr-0.9.5/datasets/
+-rw-r--r--   0 mcranmer   (504) staff       (20)     9433 2022-02-01 21:21:09.000000 pysr-0.9.5/datasets/FeynmanEquations.csv
+drwxr-xr-x   0 mcranmer   (504) staff       (20)        0 2022-07-09 20:38:35.877132 pysr-0.9.5/pysr/
+-rw-r--r--   0 mcranmer   (504) staff       (20)      300 2022-06-16 01:31:36.000000 pysr-0.9.5/pysr/__init__.py
+-rw-r--r--   0 mcranmer   (504) staff       (20)     1358 2022-06-04 20:52:09.000000 pysr-0.9.5/pysr/deprecated.py
+-rw-r--r--   0 mcranmer   (504) staff       (20)     6320 2022-06-21 23:59:39.000000 pysr-0.9.5/pysr/export_jax.py
+-rw-r--r--   0 mcranmer   (504) staff       (20)     1488 2022-06-16 01:31:36.000000 pysr-0.9.5/pysr/export_numpy.py
+-rw-r--r--   0 mcranmer   (504) staff       (20)     7576 2022-06-21 23:58:48.000000 pysr-0.9.5/pysr/export_torch.py
+-rw-r--r--   0 mcranmer   (504) staff       (20)     5615 2022-02-01 21:21:09.000000 pysr-0.9.5/pysr/feynman_problems.py
+-rw-r--r--   0 mcranmer   (504) staff       (20)     3763 2022-06-20 01:18:33.000000 pysr-0.9.5/pysr/julia_helpers.py
+-rw-r--r--   0 mcranmer   (504) staff       (20)    79972 2022-07-08 22:43:11.000000 pysr-0.9.5/pysr/sr.py
+-rw-r--r--   0 mcranmer   (504) staff       (20)       67 2022-07-09 19:22:00.000000 pysr-0.9.5/pysr/version.py
+drwxr-xr-x   0 mcranmer   (504) staff       (20)        0 2022-07-09 20:38:35.877725 pysr-0.9.5/pysr.egg-info/
+-rw-r--r--   0 mcranmer   (504) staff       (20)    11968 2022-07-09 20:38:35.000000 pysr-0.9.5/pysr.egg-info/PKG-INFO
+-rw-r--r--   0 mcranmer   (504) staff       (20)      440 2022-07-09 20:38:35.000000 pysr-0.9.5/pysr.egg-info/SOURCES.txt
+-rw-r--r--   0 mcranmer   (504) staff       (20)        1 2022-07-09 20:38:35.000000 pysr-0.9.5/pysr.egg-info/dependency_links.txt
+-rw-r--r--   0 mcranmer   (504) staff       (20)       52 2022-07-09 20:38:35.000000 pysr-0.9.5/pysr.egg-info/requires.txt
+-rw-r--r--   0 mcranmer   (504) staff       (20)       10 2022-07-09 20:38:35.000000 pysr-0.9.5/pysr.egg-info/top_level.txt
+-rw-r--r--   0 mcranmer   (504) staff       (20)       38 2022-07-09 20:38:35.879307 pysr-0.9.5/setup.cfg
+-rw-r--r--   0 mcranmer   (504) staff       (20)      947 2022-06-22 23:17:41.000000 pysr-0.9.5/setup.py
+drwxr-xr-x   0 mcranmer   (504) staff       (20)        0 2022-07-09 20:38:35.878798 pysr-0.9.5/test/
+-rw-r--r--   0 mcranmer   (504) staff       (20)        0 2022-02-01 21:21:09.000000 pysr-0.9.5/test/__init__.py
+-rw-r--r--   0 mcranmer   (504) staff       (20)    18928 2022-07-08 22:42:13.000000 pysr-0.9.5/test/test.py
+-rw-r--r--   0 mcranmer   (504) staff       (20)     3719 2022-06-21 23:51:25.000000 pysr-0.9.5/test/test_jax.py
+-rw-r--r--   0 mcranmer   (504) staff       (20)     6044 2022-07-02 03:09:41.000000 pysr-0.9.5/test/test_torch.py
```

### Comparing `pysr-0.9.4/LICENSE` & `pysr-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pysr-0.9.4/PKG-INFO` & `pysr-0.9.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysr
-Version: 0.9.4
+Version: 0.9.5
 Summary: Simple and efficient symbolic regression
 Home-page: https://github.com/MilesCranmer/pysr
 Author: Miles Cranmer
 Author-email: miles.cranmer@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pysr-0.9.4/README.md` & `pysr-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `pysr-0.9.4/datasets/FeynmanEquations.csv` & `pysr-0.9.5/datasets/FeynmanEquations.csv`

 * *Files identical despite different names*

### Comparing `pysr-0.9.4/pysr/deprecated.py` & `pysr-0.9.5/pysr/deprecated.py`

 * *Files identical despite different names*

### Comparing `pysr-0.9.4/pysr/export_jax.py` & `pysr-0.9.5/pysr/export_jax.py`

 * *Files identical despite different names*

### Comparing `pysr-0.9.4/pysr/export_numpy.py` & `pysr-0.9.5/pysr/export_numpy.py`

 * *Files identical despite different names*

### Comparing `pysr-0.9.4/pysr/export_torch.py` & `pysr-0.9.5/pysr/export_torch.py`

 * *Files identical despite different names*

### Comparing `pysr-0.9.4/pysr/feynman_problems.py` & `pysr-0.9.5/pysr/feynman_problems.py`

 * *Files identical despite different names*

### Comparing `pysr-0.9.4/pysr/julia_helpers.py` & `pysr-0.9.5/pysr/julia_helpers.py`

 * *Files identical despite different names*

### Comparing `pysr-0.9.4/pysr/sr.py` & `pysr-0.9.5/pysr/sr.py`

 * *Files identical despite different names*

### Comparing `pysr-0.9.4/pysr.egg-info/PKG-INFO` & `pysr-0.9.5/pysr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysr
-Version: 0.9.4
+Version: 0.9.5
 Summary: Simple and efficient symbolic regression
 Home-page: https://github.com/MilesCranmer/pysr
 Author: Miles Cranmer
 Author-email: miles.cranmer@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pysr-0.9.4/setup.py` & `pysr-0.9.5/setup.py`

 * *Files identical despite different names*

### Comparing `pysr-0.9.4/test/test.py` & `pysr-0.9.5/test/test.py`

 * *Files identical despite different names*

### Comparing `pysr-0.9.4/test/test_jax.py` & `pysr-0.9.5/test/test_jax.py`

 * *Files identical despite different names*

### Comparing `pysr-0.9.4/test/test_torch.py` & `pysr-0.9.5/test/test_torch.py`

 * *Files identical despite different names*

