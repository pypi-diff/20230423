# Comparing `tmp/osgood-1.1.0.tar.gz` & `tmp/osgood-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/tosgood/Desktop/Personal/osgood/osgood/dist/.tmp-zlmv4mqh/osgood-1.1.0.tar", last modified: Fri Feb 24 22:40:31 2023, max compression
+gzip compressed data, was "osgood-1.2.0.tar", last modified: Sat Apr 22 23:04:54 2023, max compression
```

## Comparing `osgood-1.1.0.tar` & `osgood-1.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 tosgood    (501) staff       (20)        0 2023-02-24 22:40:31.507368 osgood-1.1.0/
--rw-r--r--   0 tosgood    (501) staff       (20)     1064 2023-02-19 20:34:31.000000 osgood-1.1.0/LICENSE
--rw-r--r--   0 tosgood    (501) staff       (20)      793 2023-02-24 22:40:31.506927 osgood-1.1.0/PKG-INFO
--rw-r--r--   0 tosgood    (501) staff       (20)      266 2023-02-24 03:52:22.000000 osgood-1.1.0/README.md
-drwxr-xr-x   0 tosgood    (501) staff       (20)        0 2023-02-24 22:40:31.503062 osgood-1.1.0/osgood/
--rw-r--r--   0 tosgood    (501) staff       (20)        0 2023-02-24 18:55:53.000000 osgood-1.1.0/osgood/__init__.py
--rw-r--r--   0 tosgood    (501) staff       (20)     2265 2023-02-24 22:27:59.000000 osgood-1.1.0/osgood/base.py
-drwxr-xr-x   0 tosgood    (501) staff       (20)        0 2023-02-24 22:40:31.505178 osgood-1.1.0/osgood.egg-info/
--rw-r--r--   0 tosgood    (501) staff       (20)      793 2023-02-24 22:40:31.000000 osgood-1.1.0/osgood.egg-info/PKG-INFO
--rw-r--r--   0 tosgood    (501) staff       (20)      205 2023-02-24 22:40:31.000000 osgood-1.1.0/osgood.egg-info/SOURCES.txt
--rw-r--r--   0 tosgood    (501) staff       (20)        1 2023-02-24 22:40:31.000000 osgood-1.1.0/osgood.egg-info/dependency_links.txt
--rw-r--r--   0 tosgood    (501) staff       (20)        7 2023-02-24 22:40:31.000000 osgood-1.1.0/osgood.egg-info/top_level.txt
--rw-r--r--   0 tosgood    (501) staff       (20)      601 2023-02-24 22:34:26.000000 osgood-1.1.0/pyproject.toml
--rw-r--r--   0 tosgood    (501) staff       (20)       38 2023-02-24 22:40:31.507456 osgood-1.1.0/setup.cfg
-drwxr-xr-x   0 tosgood    (501) staff       (20)        0 2023-02-24 22:40:31.505918 osgood-1.1.0/tests/
--rw-r--r--   0 tosgood    (501) staff       (20)     1094 2023-02-24 21:43:18.000000 osgood-1.1.0/tests/test_base.py
+drwxr-xr-x   0 tolyosgood   (501) staff       (20)        0 2023-04-22 23:04:54.877479 osgood-1.2.0/
+-rw-r--r--   0 tolyosgood   (501) staff       (20)     1064 2023-04-01 13:42:12.000000 osgood-1.2.0/LICENSE
+-rw-r--r--   0 tolyosgood   (501) staff       (20)      793 2023-04-22 23:04:54.877262 osgood-1.2.0/PKG-INFO
+-rw-r--r--   0 tolyosgood   (501) staff       (20)      266 2023-04-01 13:42:12.000000 osgood-1.2.0/README.md
+drwxr-xr-x   0 tolyosgood   (501) staff       (20)        0 2023-04-22 23:04:54.875806 osgood-1.2.0/osgood/
+-rw-r--r--   0 tolyosgood   (501) staff       (20)       86 2023-04-01 14:27:32.000000 osgood-1.2.0/osgood/__init__.py
+-rw-r--r--   0 tolyosgood   (501) staff       (20)     2265 2023-04-01 14:27:32.000000 osgood-1.2.0/osgood/base.py
+drwxr-xr-x   0 tolyosgood   (501) staff       (20)        0 2023-04-22 23:04:54.876621 osgood-1.2.0/osgood.egg-info/
+-rw-r--r--   0 tolyosgood   (501) staff       (20)      793 2023-04-22 23:04:54.000000 osgood-1.2.0/osgood.egg-info/PKG-INFO
+-rw-r--r--   0 tolyosgood   (501) staff       (20)      205 2023-04-22 23:04:54.000000 osgood-1.2.0/osgood.egg-info/SOURCES.txt
+-rw-r--r--   0 tolyosgood   (501) staff       (20)        1 2023-04-22 23:04:54.000000 osgood-1.2.0/osgood.egg-info/dependency_links.txt
+-rw-r--r--   0 tolyosgood   (501) staff       (20)        7 2023-04-22 23:04:54.000000 osgood-1.2.0/osgood.egg-info/top_level.txt
+-rw-r--r--   0 tolyosgood   (501) staff       (20)      601 2023-04-22 23:03:04.000000 osgood-1.2.0/pyproject.toml
+-rw-r--r--   0 tolyosgood   (501) staff       (20)       38 2023-04-22 23:04:54.877549 osgood-1.2.0/setup.cfg
+drwxr-xr-x   0 tolyosgood   (501) staff       (20)        0 2023-04-22 23:04:54.876786 osgood-1.2.0/tests/
+-rw-r--r--   0 tolyosgood   (501) staff       (20)     1095 2023-04-01 14:27:32.000000 osgood-1.2.0/tests/test_base.py
```

### Comparing `osgood-1.1.0/LICENSE` & `osgood-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `osgood-1.1.0/PKG-INFO` & `osgood-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osgood
-Version: 1.1.0
+Version: 1.2.0
 Summary: A small collection of useful functions
 Author-email: charlesriver456 <osgood.package@gmail.com>
 Project-URL: Homepage, https://github.com/charlesriver456/osgood
 Project-URL: Bug Tracker, https://github.com/charlesriver456/osgood/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `osgood-1.1.0/osgood/base.py` & `osgood-1.2.0/osgood/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # A collection of useful functions
-import warnings
 import time
+import warnings
 from functools import wraps
-from itertools import repeat, chain
-from typing import List, Optional, Callable, Any
+from itertools import chain, repeat
+from typing import Any, Callable, List, Optional
 
 
 def timeit(fn_identifier: Optional[str] = None) -> Callable:
     """Decorates a function such that its execution time is printed.
     Parameters
     ----------
     fn_identifier
```

### Comparing `osgood-1.1.0/osgood.egg-info/PKG-INFO` & `osgood-1.2.0/osgood.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osgood
-Version: 1.1.0
+Version: 1.2.0
 Summary: A small collection of useful functions
 Author-email: charlesriver456 <osgood.package@gmail.com>
 Project-URL: Homepage, https://github.com/charlesriver456/osgood
 Project-URL: Bug Tracker, https://github.com/charlesriver456/osgood/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `osgood-1.1.0/pyproject.toml` & `osgood-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "osgood"
-version = "1.1.0"
+version = "1.2.0"
 authors = [
   { name="charlesriver456", email="osgood.package@gmail.com" },
 ]
 description = "A small collection of useful functions"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `osgood-1.1.0/tests/test_base.py` & `osgood-1.2.0/tests/test_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-import osgood
-from osgood.base import ozip, timeit
 import pytest
 from pytest import fixture
 
+import osgood
+from osgood.base import ozip, timeit
+
 DEFAULT_LIST = [1, 2, 3, 4]
 
 
 @pytest.mark.parametrize(
     "passed_int, expected",
     [
         (1, [(1,), (2,), (3,), (4,)]),
```

