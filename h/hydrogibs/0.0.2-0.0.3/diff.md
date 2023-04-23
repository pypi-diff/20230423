# Comparing `tmp/hydrogibs-0.0.2.tar.gz` & `tmp/hydrogibs-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydrogibs-0.0.2.tar", last modified: Sun Apr 23 14:13:03 2023, max compression
+gzip compressed data, was "hydrogibs-0.0.3.tar", last modified: Sun Apr 23 14:19:37 2023, max compression
```

## Comparing `hydrogibs-0.0.2.tar` & `hydrogibs-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-23 14:13:03.308433 hydrogibs-0.0.2/
--rw-rw-r--   0 axel      (1000) axel      (1000)     1073 2023-04-23 13:58:07.000000 hydrogibs-0.0.2/LICENSE
--rw-rw-r--   0 axel      (1000) axel      (1000)      541 2023-04-23 14:13:03.308433 hydrogibs-0.0.2/PKG-INFO
--rw-rw-r--   0 axel      (1000) axel      (1000)       37 2023-04-23 13:57:53.000000 hydrogibs-0.0.2/README.md
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-23 14:13:03.304432 hydrogibs-0.0.2/hydrogibs/
--rw-rw-r--   0 axel      (1000) axel      (1000)       13 2023-04-23 13:28:00.000000 hydrogibs-0.0.2/hydrogibs/__init_.py
--rw-rw-r--   0 axel      (1000) axel      (1000)       42 2023-04-23 13:53:43.000000 hydrogibs-0.0.2/hydrogibs/example.py
--rw-rw-r--   0 axel      (1000) axel      (1000)    24140 2023-04-23 13:17:14.000000 hydrogibs-0.0.2/hydrogibs/floods.py
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-23 14:13:03.308433 hydrogibs-0.0.2/hydrogibs.egg-info/
--rw-rw-r--   0 axel      (1000) axel      (1000)      541 2023-04-23 14:13:03.000000 hydrogibs-0.0.2/hydrogibs.egg-info/PKG-INFO
--rw-rw-r--   0 axel      (1000) axel      (1000)      226 2023-04-23 14:13:03.000000 hydrogibs-0.0.2/hydrogibs.egg-info/SOURCES.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)        1 2023-04-23 14:13:03.000000 hydrogibs-0.0.2/hydrogibs.egg-info/dependency_links.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)       10 2023-04-23 14:13:03.000000 hydrogibs-0.0.2/hydrogibs.egg-info/top_level.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)      489 2023-04-23 14:12:46.000000 hydrogibs-0.0.2/pyproject.toml
--rw-rw-r--   0 axel      (1000) axel      (1000)       38 2023-04-23 14:13:03.308433 hydrogibs-0.0.2/setup.cfg
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-23 14:19:37.689379 hydrogibs-0.0.3/
+-rw-rw-r--   0 axel      (1000) axel      (1000)     1073 2023-04-23 13:58:07.000000 hydrogibs-0.0.3/LICENSE
+-rw-rw-r--   0 axel      (1000) axel      (1000)      541 2023-04-23 14:19:37.689379 hydrogibs-0.0.3/PKG-INFO
+-rw-rw-r--   0 axel      (1000) axel      (1000)       37 2023-04-23 13:57:53.000000 hydrogibs-0.0.3/README.md
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-23 14:19:37.689379 hydrogibs-0.0.3/hydrogibs/
+-rw-rw-r--   0 axel      (1000) axel      (1000)       13 2023-04-23 13:28:00.000000 hydrogibs-0.0.3/hydrogibs/__init_.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)       42 2023-04-23 13:53:43.000000 hydrogibs-0.0.3/hydrogibs/example.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)    24140 2023-04-23 13:17:14.000000 hydrogibs-0.0.3/hydrogibs/floods.py
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-23 14:19:37.689379 hydrogibs-0.0.3/hydrogibs.egg-info/
+-rw-rw-r--   0 axel      (1000) axel      (1000)      541 2023-04-23 14:19:37.000000 hydrogibs-0.0.3/hydrogibs.egg-info/PKG-INFO
+-rw-rw-r--   0 axel      (1000) axel      (1000)      226 2023-04-23 14:19:37.000000 hydrogibs-0.0.3/hydrogibs.egg-info/SOURCES.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)        1 2023-04-23 14:19:37.000000 hydrogibs-0.0.3/hydrogibs.egg-info/dependency_links.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)       10 2023-04-23 14:19:37.000000 hydrogibs-0.0.3/hydrogibs.egg-info/top_level.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)      489 2023-04-23 14:17:46.000000 hydrogibs-0.0.3/pyproject.toml
+-rw-rw-r--   0 axel      (1000) axel      (1000)       38 2023-04-23 14:19:37.689379 hydrogibs-0.0.3/setup.cfg
```

### Comparing `hydrogibs-0.0.2/LICENSE` & `hydrogibs-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.0.2/PKG-INFO` & `hydrogibs-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydrogibs
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small hydrology package
 Author-email: axel Giboulot <axel.giboulot@epfl.ch>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hydrogibs-0.0.2/hydrogibs/floods.py` & `hydrogibs-0.0.3/hydrogibs/floods.py`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.0.2/hydrogibs.egg-info/PKG-INFO` & `hydrogibs-0.0.3/hydrogibs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydrogibs
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small hydrology package
 Author-email: axel Giboulot <axel.giboulot@epfl.ch>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

