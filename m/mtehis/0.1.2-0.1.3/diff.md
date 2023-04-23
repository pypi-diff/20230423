# Comparing `tmp/mtehis-0.1.2.tar.gz` & `tmp/mtehis-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mtehis-0.1.2.tar", last modified: Mon Apr 17 13:45:38 2023, max compression
+gzip compressed data, was "mtehis-0.1.3.tar", last modified: Sun Apr 23 13:32:31 2023, max compression
```

## Comparing `mtehis-0.1.2.tar` & `mtehis-0.1.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:45:38.221960 mtehis-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-17 13:45:24.000000 mtehis-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-17 13:45:38.221960 mtehis-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-17 13:45:24.000000 mtehis-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:45:38.221960 mtehis-0.1.2/mtehis/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-17 13:45:24.000000 mtehis-0.1.2/mtehis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:45:38.221960 mtehis-0.1.2/mtehis/base/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-17 13:45:24.000000 mtehis-0.1.2/mtehis/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-17 13:45:24.000000 mtehis-0.1.2/mtehis/base/detector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:45:38.221960 mtehis-0.1.2/mtehis/data/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-17 13:45:24.000000 mtehis-0.1.2/mtehis/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-17 13:45:24.000000 mtehis-0.1.2/mtehis/data/detector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:45:38.221960 mtehis-0.1.2/mtehis/model/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-17 13:45:24.000000 mtehis-0.1.2/mtehis/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-17 13:45:24.000000 mtehis-0.1.2/mtehis/model/classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-04-17 13:45:24.000000 mtehis-0.1.2/mtehis/model/detector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:45:38.221960 mtehis-0.1.2/mtehis/util/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-17 13:45:24.000000 mtehis-0.1.2/mtehis/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-17 13:45:24.000000 mtehis-0.1.2/mtehis/util/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-17 13:45:24.000000 mtehis-0.1.2/mtehis/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:45:38.221960 mtehis-0.1.2/mtehis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-17 13:45:38.000000 mtehis-0.1.2/mtehis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-17 13:45:38.000000 mtehis-0.1.2/mtehis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 13:45:38.000000 mtehis-0.1.2/mtehis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-17 13:45:38.000000 mtehis-0.1.2/mtehis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-17 13:45:38.000000 mtehis-0.1.2/mtehis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 13:45:38.221960 mtehis-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-17 13:45:24.000000 mtehis-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:32:31.389829 mtehis-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-23 13:32:15.000000 mtehis-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-23 13:32:31.389829 mtehis-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-23 13:32:15.000000 mtehis-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:32:31.381829 mtehis-0.1.3/mtehis/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-23 13:32:15.000000 mtehis-0.1.3/mtehis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:32:31.385829 mtehis-0.1.3/mtehis/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-23 13:32:15.000000 mtehis-0.1.3/mtehis/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-23 13:32:15.000000 mtehis-0.1.3/mtehis/base/detector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:32:31.385829 mtehis-0.1.3/mtehis/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-23 13:32:15.000000 mtehis-0.1.3/mtehis/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-23 13:32:15.000000 mtehis-0.1.3/mtehis/data/detector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:32:31.385829 mtehis-0.1.3/mtehis/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-23 13:32:15.000000 mtehis-0.1.3/mtehis/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-23 13:32:15.000000 mtehis-0.1.3/mtehis/model/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-04-23 13:32:15.000000 mtehis-0.1.3/mtehis/model/detector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:32:31.385829 mtehis-0.1.3/mtehis/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-23 13:32:15.000000 mtehis-0.1.3/mtehis/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-23 13:32:15.000000 mtehis-0.1.3/mtehis/util/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-23 13:32:15.000000 mtehis-0.1.3/mtehis/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:32:31.385829 mtehis-0.1.3/mtehis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-23 13:32:31.000000 mtehis-0.1.3/mtehis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-23 13:32:31.000000 mtehis-0.1.3/mtehis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 13:32:31.000000 mtehis-0.1.3/mtehis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-23 13:32:31.000000 mtehis-0.1.3/mtehis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-23 13:32:31.000000 mtehis-0.1.3/mtehis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 13:32:31.389829 mtehis-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-23 13:32:15.000000 mtehis-0.1.3/setup.py
```

### Comparing `mtehis-0.1.2/LICENSE` & `mtehis-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mtehis-0.1.2/PKG-INFO` & `mtehis-0.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtehis
-Version: 0.1.2
+Version: 0.1.3
 Summary: Maintenance Tool for Evolving Hybrid Intelligent Systems: Core Package.
 Home-page: https://github.com/MT-EHIS/core
 Author: Oleksandr Pokhylenko
 Author-email: pokhilenko.alex@gmail.com
 License: UNKNOWN
 Platform: all
 Classifier: Intended Audience :: Developers
```

### Comparing `mtehis-0.1.2/mtehis/base/detector.py` & `mtehis-0.1.3/mtehis/base/detector.py`

 * *Files identical despite different names*

### Comparing `mtehis-0.1.2/mtehis/data/detector.py` & `mtehis-0.1.3/mtehis/data/detector.py`

 * *Files identical despite different names*

### Comparing `mtehis-0.1.2/mtehis/model/classifier.py` & `mtehis-0.1.3/mtehis/model/classifier.py`

 * *Files identical despite different names*

### Comparing `mtehis-0.1.2/mtehis/model/detector.py` & `mtehis-0.1.3/mtehis/model/detector.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,7 +58,12 @@
         scores = scores[~np.isnan(scores).any(axis=1)]
         self.classifier.fit(scores, ys)
 
     def predict(self, xs):
         scores = self._get_scores(xs)
         scores[np.isnan(scores)] = 0
         return self.classifier.predict(scores)
+
+    def predict_with_scores(self, xs):
+        scores = self._get_scores(xs)
+        scores[np.isnan(scores)] = 0
+        return self.classifier.predict(scores), scores
```

### Comparing `mtehis-0.1.2/mtehis/util/evaluate.py` & `mtehis-0.1.3/mtehis/util/evaluate.py`

 * *Files identical despite different names*

### Comparing `mtehis-0.1.2/mtehis.egg-info/PKG-INFO` & `mtehis-0.1.3/mtehis.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtehis
-Version: 0.1.2
+Version: 0.1.3
 Summary: Maintenance Tool for Evolving Hybrid Intelligent Systems: Core Package.
 Home-page: https://github.com/MT-EHIS/core
 Author: Oleksandr Pokhylenko
 Author-email: pokhilenko.alex@gmail.com
 License: UNKNOWN
 Platform: all
 Classifier: Intended Audience :: Developers
```

### Comparing `mtehis-0.1.2/setup.py` & `mtehis-0.1.3/setup.py`

 * *Files identical despite different names*

