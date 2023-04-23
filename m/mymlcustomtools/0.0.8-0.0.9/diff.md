# Comparing `tmp/mymlcustomtools-0.0.8.tar.gz` & `tmp/mymlcustomtools-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mymlcustomtools-0.0.8.tar", last modified: Mon Apr 17 20:37:36 2023, max compression
+gzip compressed data, was "dist\mymlcustomtools-0.0.9.tar", last modified: Mon Apr 17 20:43:14 2023, max compression
```

## Comparing `mymlcustomtools-0.0.8.tar` & `mymlcustomtools-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 20:37:36.622747 mymlcustomtools-0.0.8/
--rw-rw-rw-   0        0        0      321 2023-04-17 20:37:36.622747 mymlcustomtools-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       67 2023-04-17 14:36:20.000000 mymlcustomtools-0.0.8/README.txt
-drwxrwxrwx   0        0        0        0 2023-04-17 20:37:36.604851 mymlcustomtools-0.0.8/mymlcustomtools/
--rw-rw-rw-   0        0        0       60 2023-04-17 14:17:11.000000 mymlcustomtools-0.0.8/mymlcustomtools/__init__.py
--rw-rw-rw-   0        0        0     3033 2023-04-17 14:34:13.000000 mymlcustomtools-0.0.8/mymlcustomtools/imports.py
--rw-rw-rw-   0        0        0     2788 2023-04-17 20:37:11.000000 mymlcustomtools-0.0.8/mymlcustomtools/main.py
-drwxrwxrwx   0        0        0        0 2023-04-17 20:37:36.618748 mymlcustomtools-0.0.8/mymlcustomtools.egg-info/
--rw-rw-rw-   0        0        0      321 2023-04-17 20:37:32.000000 mymlcustomtools-0.0.8/mymlcustomtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-04-17 20:37:33.000000 mymlcustomtools-0.0.8/mymlcustomtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 20:37:32.000000 mymlcustomtools-0.0.8/mymlcustomtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-17 14:47:42.000000 mymlcustomtools-0.0.8/mymlcustomtools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       16 2023-04-17 20:37:32.000000 mymlcustomtools-0.0.8/mymlcustomtools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 20:37:36.622747 mymlcustomtools-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      725 2023-04-17 20:37:25.000000 mymlcustomtools-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 20:43:14.216183 mymlcustomtools-0.0.9/
+-rw-rw-rw-   0        0        0      321 2023-04-17 20:43:14.216183 mymlcustomtools-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       67 2023-04-17 14:36:20.000000 mymlcustomtools-0.0.9/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 20:43:14.160892 mymlcustomtools-0.0.9/mymlcustomtools/
+-rw-rw-rw-   0        0        0       60 2023-04-17 14:17:11.000000 mymlcustomtools-0.0.9/mymlcustomtools/__init__.py
+-rw-rw-rw-   0        0        0     3033 2023-04-17 14:34:13.000000 mymlcustomtools-0.0.9/mymlcustomtools/imports.py
+-rw-rw-rw-   0        0        0     2881 2023-04-17 20:43:09.000000 mymlcustomtools-0.0.9/mymlcustomtools/main.py
+drwxrwxrwx   0        0        0        0 2023-04-17 20:43:14.216183 mymlcustomtools-0.0.9/mymlcustomtools.egg-info/
+-rw-rw-rw-   0        0        0      321 2023-04-17 20:43:13.000000 mymlcustomtools-0.0.9/mymlcustomtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-04-17 20:43:13.000000 mymlcustomtools-0.0.9/mymlcustomtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 20:43:13.000000 mymlcustomtools-0.0.9/mymlcustomtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-17 14:47:42.000000 mymlcustomtools-0.0.9/mymlcustomtools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       16 2023-04-17 20:43:13.000000 mymlcustomtools-0.0.9/mymlcustomtools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 20:43:14.216183 mymlcustomtools-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      725 2023-04-17 20:43:13.000000 mymlcustomtools-0.0.9/setup.py
```

### Comparing `mymlcustomtools-0.0.8/mymlcustomtools/imports.py` & `mymlcustomtools-0.0.9/mymlcustomtools/imports.py`

 * *Files identical despite different names*

### Comparing `mymlcustomtools-0.0.8/mymlcustomtools/main.py` & `mymlcustomtools-0.0.9/mymlcustomtools/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import time
 import inspect
 import os
 import pickle
+from sklearn.model_selection import GridSearchCV
 
 __fit_model_counter = 0
 def save(model):
 	global __fit_model_counter, DIR_PATH
 
 	existing_models = [fn[:-6] for fn in os.listdir(DIR_PATH) if fn[-6:]==".model"]
 	__fit_model_counter = 1 + max(__fit_model_counter, *[int(model_name) if model_name.isnumeric() else 0 for model_name in existing_models], -1)
@@ -57,16 +58,18 @@
 
 def fit(model, X, y, debug=False):
 	mount()
 	print(DIR_PATH)
 
 	initial_time = time.time()
 	if type(model)==GridSearchCV:
+		print("Bar fit")
 		bar_fit(model, X, y)
 	else:
+		print("Normal fit")
 		model.fit(X, y)
 	final_time   = time.time()
 	elapsed_time = final_time - initial_time
 	print("Elapsed time: " + ("{:.1f} s".format(elapsed_time)) if elapsed_time < 60 else ("{:.0f} min {:.0f} s".format(round(elapsed_time,0)//60,round(elapsed_time,0)%60)) )
 
 	save(model)
```

### Comparing `mymlcustomtools-0.0.8/setup.py` & `mymlcustomtools-0.0.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
 	name = "mymlcustomtools",
-	version = "0.0.8",
+	version = "0.0.9",
 	description = """
 	A package with frequently and useful functions for machine learning
 	""",
 	author = "Gustavo Exel",
 	author_email = "gustavoexelgpe@gmail.com",
 	url = "https://pypi.org/project/mymlcustomtools/",
 	packages = ["mymlcustomtools"],
```

