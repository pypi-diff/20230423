# Comparing `tmp/cleopatra-0.3.1.tar.gz` & `tmp/cleopatra-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleopatra-0.3.1.tar", last modified: Mon Apr 17 03:45:09 2023, max compression
+gzip compressed data, was "cleopatra-0.3.2.tar", last modified: Sun Apr 23 03:15:41 2023, max compression
```

## Comparing `cleopatra-0.3.1.tar` & `cleopatra-0.3.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 03:45:09.612063 cleopatra-0.3.1/
--rw-rw-rw-   0        0        0      173 2022-03-20 16:23:15.000000 cleopatra-0.3.1/AUTHORS.rst
--rw-rw-rw-   0        0        0    35591 2022-03-20 16:22:07.000000 cleopatra-0.3.1/LICENSE.md
--rw-rw-rw-   0        0        0     6887 2023-04-17 03:45:09.611064 cleopatra-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     5081 2023-04-17 03:25:28.000000 cleopatra-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 03:45:09.592188 cleopatra-0.3.1/cleopatra/
--rw-rw-rw-   0        0        0     1038 2023-04-11 15:41:59.000000 cleopatra-0.3.1/cleopatra/__init__.py
--rw-rw-rw-   0        0        0    37346 2023-04-17 03:25:28.000000 cleopatra-0.3.1/cleopatra/array.py
--rw-rw-rw-   0        0        0     2892 2023-04-11 15:41:59.000000 cleopatra-0.3.1/cleopatra/statistics.py
--rw-rw-rw-   0        0        0     6398 2023-04-17 03:25:28.000000 cleopatra-0.3.1/cleopatra/styles.py
-drwxrwxrwx   0        0        0        0 2023-04-17 03:45:09.601556 cleopatra-0.3.1/cleopatra.egg-info/
--rw-rw-rw-   0        0        0     6887 2023-04-17 03:45:09.000000 cleopatra-0.3.1/cleopatra.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      393 2023-04-17 03:45:09.000000 cleopatra-0.3.1/cleopatra.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 03:45:09.000000 cleopatra-0.3.1/cleopatra.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-11 15:48:52.000000 cleopatra-0.3.1/cleopatra.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      107 2023-04-17 03:45:09.000000 cleopatra-0.3.1/cleopatra.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-17 03:45:09.000000 cleopatra-0.3.1/cleopatra.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 03:45:09.612063 cleopatra-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1689 2023-04-17 03:25:28.000000 cleopatra-0.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 03:45:09.608555 cleopatra-0.3.1/tests/
--rw-rw-rw-   0        0        0     8159 2023-04-17 03:25:28.000000 cleopatra-0.3.1/tests/test_plot_array.py
--rw-rw-rw-   0        0        0      414 2023-04-11 15:41:59.000000 cleopatra-0.3.1/tests/test_statistics.py
--rw-rw-rw-   0        0        0      218 2023-04-11 15:41:59.000000 cleopatra-0.3.1/tests/test_styles.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:15:41.521115 cleopatra-0.3.2/
+-rw-rw-rw-   0        0        0      173 2022-03-20 16:23:15.000000 cleopatra-0.3.2/AUTHORS.rst
+-rw-rw-rw-   0        0        0    35591 2022-03-20 16:22:07.000000 cleopatra-0.3.2/LICENSE.md
+-rw-rw-rw-   0        0        0     6952 2023-04-23 03:15:41.520114 cleopatra-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5081 2023-04-23 03:09:51.000000 cleopatra-0.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 03:15:41.502096 cleopatra-0.3.2/cleopatra/
+-rw-rw-rw-   0        0        0     1038 2023-04-11 15:41:59.000000 cleopatra-0.3.2/cleopatra/__init__.py
+-rw-rw-rw-   0        0        0    37348 2023-04-23 03:09:51.000000 cleopatra-0.3.2/cleopatra/array.py
+-rw-rw-rw-   0        0        0     2892 2023-04-11 15:41:59.000000 cleopatra-0.3.2/cleopatra/statistics.py
+-rw-rw-rw-   0        0        0     6398 2023-04-17 03:25:28.000000 cleopatra-0.3.2/cleopatra/styles.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:15:41.511605 cleopatra-0.3.2/cleopatra.egg-info/
+-rw-rw-rw-   0        0        0     6952 2023-04-23 03:15:41.000000 cleopatra-0.3.2/cleopatra.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      393 2023-04-23 03:15:41.000000 cleopatra-0.3.2/cleopatra.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 03:15:41.000000 cleopatra-0.3.2/cleopatra.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-23 03:15:41.000000 cleopatra-0.3.2/cleopatra.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      107 2023-04-23 03:15:41.000000 cleopatra-0.3.2/cleopatra.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-23 03:15:41.000000 cleopatra-0.3.2/cleopatra.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 03:15:41.521115 cleopatra-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1689 2023-04-23 03:09:51.000000 cleopatra-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:15:41.518114 cleopatra-0.3.2/tests/
+-rw-rw-rw-   0        0        0     8159 2023-04-17 03:25:28.000000 cleopatra-0.3.2/tests/test_plot_array.py
+-rw-rw-rw-   0        0        0      414 2023-04-11 15:41:59.000000 cleopatra-0.3.2/tests/test_statistics.py
+-rw-rw-rw-   0        0        0      218 2023-04-11 15:41:59.000000 cleopatra-0.3.2/tests/test_styles.py
```

### Comparing `cleopatra-0.3.1/LICENSE.md` & `cleopatra-0.3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cleopatra-0.3.1/PKG-INFO` & `cleopatra-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleopatra
-Version: 0.3.1
+Version: 0.3.2
 Summary: visualization package
 Home-page: https://github.com/MAfarrag/cleopatra
 Author: Mostafa Farrag
 Author-email: moah.farag@gmail.come
 License: GNU General Public License v3
 Keywords: matplotlib,arrays,visualization
 Classifier: Development Status :: 5 - Production/Stable
@@ -68,15 +68,15 @@
 ```
 pip install git+https://github.com/MAfarrag/cleopatra
 ```
 
 ## pip
 to install the last release you can easly use pip
 ```
-pip install cleopatra==0.3.1
+pip install cleopatra==0.3.2
 ```
 
 Quick start
 ===========
 
 ```
   >>> import cleopatra
@@ -122,7 +122,11 @@
 * restructure the whole modules to array, statistics, and styles modules.
 * all modules has classes.
 * save animation function using ffmpeg.
 
 0.3.1 (2023-04-17)
 ------------------
 * plot RGB plots
+
+0.3.2 (2023-04-23)
+------------------
+* bump up hpc version
```

### Comparing `cleopatra-0.3.1/README.md` & `cleopatra-0.3.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 ```
 pip install git+https://github.com/MAfarrag/cleopatra
 ```
 
 ## pip
 to install the last release you can easly use pip
 ```
-pip install cleopatra==0.3.1
+pip install cleopatra==0.3.2
 ```
 
 Quick start
 ===========
 
 ```
   >>> import cleopatra
```

### Comparing `cleopatra-0.3.1/cleopatra/__init__.py` & `cleopatra-0.3.2/cleopatra/__init__.py`

 * *Files identical despite different names*

### Comparing `cleopatra-0.3.1/cleopatra/array.py` & `cleopatra-0.3.2/cleopatra/array.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """plotting Array."""
 from typing import Any, Union, List
 
 import matplotlib.colors as colors
 import matplotlib.pyplot as plt
 import numpy as np
-from hpc.filter import get_indices2
+from hpc.indexing import get_indices2
 
 # from matplotlib import gridspec
 from matplotlib.animation import FuncAnimation
 from matplotlib import animation
 from matplotlib.ticker import LogFormatter
 from cleopatra.styles import DEFAULT_OPTIONS as style_defaults
 from cleopatra.styles import MidpointNormalize
```

### Comparing `cleopatra-0.3.1/cleopatra/statistics.py` & `cleopatra-0.3.2/cleopatra/statistics.py`

 * *Files identical despite different names*

### Comparing `cleopatra-0.3.1/cleopatra/styles.py` & `cleopatra-0.3.2/cleopatra/styles.py`

 * *Files identical despite different names*

### Comparing `cleopatra-0.3.1/cleopatra.egg-info/PKG-INFO` & `cleopatra-0.3.2/cleopatra.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleopatra
-Version: 0.3.1
+Version: 0.3.2
 Summary: visualization package
 Home-page: https://github.com/MAfarrag/cleopatra
 Author: Mostafa Farrag
 Author-email: moah.farag@gmail.come
 License: GNU General Public License v3
 Keywords: matplotlib,arrays,visualization
 Classifier: Development Status :: 5 - Production/Stable
@@ -68,15 +68,15 @@
 ```
 pip install git+https://github.com/MAfarrag/cleopatra
 ```
 
 ## pip
 to install the last release you can easly use pip
 ```
-pip install cleopatra==0.3.1
+pip install cleopatra==0.3.2
 ```
 
 Quick start
 ===========
 
 ```
   >>> import cleopatra
@@ -122,7 +122,11 @@
 * restructure the whole modules to array, statistics, and styles modules.
 * all modules has classes.
 * save animation function using ffmpeg.
 
 0.3.1 (2023-04-17)
 ------------------
 * plot RGB plots
+
+0.3.2 (2023-04-23)
+------------------
+* bump up hpc version
```

### Comparing `cleopatra-0.3.1/setup.py` & `cleopatra-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     history = history_file.read()
 
 requirements = [line.strip() for line in open("requirements.txt").readlines()]
 requirements_dev = [line.strip() for line in open("requirements-dev.txt").readlines()]
 
 setup(
     name="cleopatra",
-    version="0.3.1",
+    version="0.3.2",
     description="visualization package",
     author="Mostafa Farrag",
     author_email="moah.farag@gmail.come",
     url="https://github.com/MAfarrag/cleopatra",
     keywords=["matplotlib", "arrays", "visualization"],
     long_description=readme + "\n\n" + history,
     repository="https://github.com/MAfarrag/celopatra",
```

### Comparing `cleopatra-0.3.1/tests/test_plot_array.py` & `cleopatra-0.3.2/tests/test_plot_array.py`

 * *Files identical despite different names*

