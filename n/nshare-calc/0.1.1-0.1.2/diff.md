# Comparing `tmp/nshare-calc-0.1.1.tar.gz` & `tmp/nshare-calc-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nshare-calc-0.1.1.tar", last modified: Wed Apr 12 20:06:27 2023, max compression
+gzip compressed data, was "nshare-calc-0.1.2.tar", last modified: Sun Apr 23 10:49:59 2023, max compression
```

## Comparing `nshare-calc-0.1.1.tar` & `nshare-calc-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 yfiua     (1000) yfiua     (1000)        0 2023-04-12 20:06:27.541753 nshare-calc-0.1.1/
--rw-rw-r--   0 yfiua     (1000) yfiua     (1000)    11357 2023-04-06 09:24:02.000000 nshare-calc-0.1.1/LICENSE
--rw-rw-r--   0 yfiua     (1000) yfiua     (1000)     1351 2023-04-12 20:06:27.541753 nshare-calc-0.1.1/PKG-INFO
--rw-rw-r--   0 yfiua     (1000) yfiua     (1000)      769 2023-04-12 19:44:04.000000 nshare-calc-0.1.1/README.md
--rw-rw-r--   0 yfiua     (1000) yfiua     (1000)      755 2023-04-12 19:43:24.000000 nshare-calc-0.1.1/pyproject.toml
--rw-rw-r--   0 yfiua     (1000) yfiua     (1000)       26 2023-04-12 18:38:56.000000 nshare-calc-0.1.1/requirements.txt
--rw-rw-r--   0 yfiua     (1000) yfiua     (1000)       38 2023-04-12 20:06:27.541753 nshare-calc-0.1.1/setup.cfg
-drwxrwxr-x   0 yfiua     (1000) yfiua     (1000)        0 2023-04-12 20:06:27.537753 nshare-calc-0.1.1/src/
-drwxrwxr-x   0 yfiua     (1000) yfiua     (1000)        0 2023-04-12 20:06:27.541753 nshare-calc-0.1.1/src/nshare_calc/
--rw-rw-r--   0 yfiua     (1000) yfiua     (1000)       32 2023-04-12 20:03:42.000000 nshare-calc-0.1.1/src/nshare_calc/__init__.py
--rwxrwxr-x   0 yfiua     (1000) yfiua     (1000)     1096 2023-04-12 20:03:42.000000 nshare-calc-0.1.1/src/nshare_calc/nshare_calc.py
-drwxrwxr-x   0 yfiua     (1000) yfiua     (1000)        0 2023-04-12 20:06:27.541753 nshare-calc-0.1.1/src/nshare_calc.egg-info/
--rw-rw-r--   0 yfiua     (1000) yfiua     (1000)     1351 2023-04-12 20:06:27.000000 nshare-calc-0.1.1/src/nshare_calc.egg-info/PKG-INFO
--rw-rw-r--   0 yfiua     (1000) yfiua     (1000)      316 2023-04-12 20:06:27.000000 nshare-calc-0.1.1/src/nshare_calc.egg-info/SOURCES.txt
--rw-rw-r--   0 yfiua     (1000) yfiua     (1000)        1 2023-04-12 20:06:27.000000 nshare-calc-0.1.1/src/nshare_calc.egg-info/dependency_links.txt
--rw-rw-r--   0 yfiua     (1000) yfiua     (1000)       26 2023-04-12 20:06:27.000000 nshare-calc-0.1.1/src/nshare_calc.egg-info/requires.txt
--rw-rw-r--   0 yfiua     (1000) yfiua     (1000)       12 2023-04-12 20:06:27.000000 nshare-calc-0.1.1/src/nshare_calc.egg-info/top_level.txt
-drwxrwxr-x   0 yfiua     (1000) yfiua     (1000)        0 2023-04-12 20:06:27.541753 nshare-calc-0.1.1/test/
--rwxrwxr-x   0 yfiua     (1000) yfiua     (1000)      243 2023-04-12 18:45:20.000000 nshare-calc-0.1.1/test/test1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 10:49:59.822370 nshare-calc-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-23 10:49:49.000000 nshare-calc-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-04-23 10:49:59.822370 nshare-calc-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-23 10:49:49.000000 nshare-calc-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-23 10:49:49.000000 nshare-calc-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-23 10:49:49.000000 nshare-calc-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 10:49:59.822370 nshare-calc-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 10:49:59.818370 nshare-calc-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 10:49:59.822370 nshare-calc-0.1.2/src/nshare_calc/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-23 10:49:49.000000 nshare-calc-0.1.2/src/nshare_calc/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1096 2023-04-23 10:49:49.000000 nshare-calc-0.1.2/src/nshare_calc/nshare_calc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 10:49:59.822370 nshare-calc-0.1.2/src/nshare_calc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-04-23 10:49:59.000000 nshare-calc-0.1.2/src/nshare_calc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-23 10:49:59.000000 nshare-calc-0.1.2/src/nshare_calc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 10:49:59.000000 nshare-calc-0.1.2/src/nshare_calc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-23 10:49:59.000000 nshare-calc-0.1.2/src/nshare_calc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-23 10:49:59.000000 nshare-calc-0.1.2/src/nshare_calc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 10:49:59.822370 nshare-calc-0.1.2/test/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      243 2023-04-23 10:49:49.000000 nshare-calc-0.1.2/test/test1.py
```

### Comparing `nshare-calc-0.1.1/LICENSE` & `nshare-calc-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nshare-calc-0.1.1/PKG-INFO` & `nshare-calc-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
 Name: nshare-calc
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python library for calculating the optimal number of shares given a portfolio using integer programming.
 Author-email: Yfiua <yfiua6@gmail.com>
 Project-URL: Homepage, https://github.com/yfiua/nshare-calc
 Project-URL: Bug Tracker, https://github.com/yfiua/nshare-calc/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # nshare-calc
-Python library for calculating the optimal number of shares given a portfolio using integer programming.
+Python package for calculating the optimal number of shares given a portfolio using integer programming.
 
 ## Problem statement
 
 Given a portfolio with total asset $S$, price vector $\mathbf p$ and weight vector $\mathbf w$, find integer vector $\mathbf n$ such that
 
 * The total value of all stocks must not exceed the total asset, i.e., $\mathbf p \cdot \mathbf n \leq S$;
 * Minimize the total absolute difference between the desired values and the actual values for all stocks, i.e., $\Sigma_i |S w_i - p_i n_i|$.
 
 ## Installation
 
-```
+```sh
 pip install nshare-calc
 ```
 
 ## Usage
 
-```
+```python
 from nshare_calc import calc_n
 
 # params
 S = 100
 p = [6, 5.5]
 w = [0.6, 0.4]         # w will be automatically normalized
```

### Comparing `nshare-calc-0.1.1/pyproject.toml` & `nshare-calc-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nshare-calc"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Yfiua", email="yfiua6@gmail.com" },
 ]
 description = "Python library for calculating the optimal number of shares given a portfolio using integer programming."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `nshare-calc-0.1.1/src/nshare_calc/nshare_calc.py` & `nshare-calc-0.1.2/src/nshare_calc/nshare_calc.py`

 * *Files identical despite different names*

### Comparing `nshare-calc-0.1.1/src/nshare_calc.egg-info/PKG-INFO` & `nshare-calc-0.1.2/src/nshare_calc.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
 Name: nshare-calc
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python library for calculating the optimal number of shares given a portfolio using integer programming.
 Author-email: Yfiua <yfiua6@gmail.com>
 Project-URL: Homepage, https://github.com/yfiua/nshare-calc
 Project-URL: Bug Tracker, https://github.com/yfiua/nshare-calc/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # nshare-calc
-Python library for calculating the optimal number of shares given a portfolio using integer programming.
+Python package for calculating the optimal number of shares given a portfolio using integer programming.
 
 ## Problem statement
 
 Given a portfolio with total asset $S$, price vector $\mathbf p$ and weight vector $\mathbf w$, find integer vector $\mathbf n$ such that
 
 * The total value of all stocks must not exceed the total asset, i.e., $\mathbf p \cdot \mathbf n \leq S$;
 * Minimize the total absolute difference between the desired values and the actual values for all stocks, i.e., $\Sigma_i |S w_i - p_i n_i|$.
 
 ## Installation
 
-```
+```sh
 pip install nshare-calc
 ```
 
 ## Usage
 
-```
+```python
 from nshare_calc import calc_n
 
 # params
 S = 100
 p = [6, 5.5]
 w = [0.6, 0.4]         # w will be automatically normalized
```

