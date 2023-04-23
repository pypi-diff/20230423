# Comparing `tmp/py-aiger-gridworld-0.4.1.tar.gz` & `tmp/py_aiger_gridworld-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-aiger-gridworld-0.4.1.tar", max compression
+gzip compressed data, was "py_aiger_gridworld-0.4.3.tar", max compression
```

## Comparing `py-aiger-gridworld-0.4.1.tar` & `py_aiger_gridworld-0.4.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1082 2021-11-17 01:13:18.852940 py-aiger-gridworld-0.4.1/LICENSE
--rw-r--r--   0        0        0     1029 2021-11-17 01:13:18.852940 py-aiger-gridworld-0.4.1/README.md
--rw-r--r--   0        0        0       88 2021-11-17 01:13:18.852940 py-aiger-gridworld-0.4.1/aiger_gridworld/__init__.py
--rw-r--r--   0        0        0     2716 2021-11-17 01:13:18.852940 py-aiger-gridworld-0.4.1/aiger_gridworld/dynamics.py
--rw-r--r--   0        0        0      873 2021-11-17 01:13:18.852940 py-aiger-gridworld-0.4.1/aiger_gridworld/vis.py
--rw-r--r--   0        0        0      600 2021-11-17 01:15:49.864173 py-aiger-gridworld-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     1827 2021-11-17 01:16:03.764273 py-aiger-gridworld-0.4.1/setup.py
--rw-r--r--   0        0        0     1707 2021-11-17 01:16:03.765489 py-aiger-gridworld-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1082 2022-11-03 04:30:44.525858 py_aiger_gridworld-0.4.3/LICENSE
+-rw-r--r--   0        0        0      882 2022-11-03 04:34:01.658556 py_aiger_gridworld-0.4.3/README.md
+-rw-r--r--   0        0        0       88 2022-11-03 04:30:44.525858 py_aiger_gridworld-0.4.3/aiger_gridworld/__init__.py
+-rw-r--r--   0        0        0     2716 2022-11-03 04:30:44.525858 py_aiger_gridworld-0.4.3/aiger_gridworld/dynamics.py
+-rw-r--r--   0        0        0      873 2022-11-03 04:30:44.525858 py_aiger_gridworld-0.4.3/aiger_gridworld/vis.py
+-rw-r--r--   0        0        0      578 2023-04-23 07:03:03.487871 py_aiger_gridworld-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     1682 1970-01-01 00:00:00.000000 py_aiger_gridworld-0.4.3/setup.py
+-rw-r--r--   0        0        0     1608 1970-01-01 00:00:00.000000 py_aiger_gridworld-0.4.3/PKG-INFO
```

### Comparing `py-aiger-gridworld-0.4.1/LICENSE` & `py_aiger_gridworld-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `py-aiger-gridworld-0.4.1/README.md` & `py_aiger_gridworld-0.4.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # py-aiger-gridworld
 
 Library for modeling gridworlds as AIGER circuits.
 
 [![Build Status](https://cloud.drone.io/api/badges/mvcisback/py-aiger-gridworld/status.svg)](https://cloud.drone.io/mvcisback/py-aiger-gridworld)
-[![codecov](https://codecov.io/gh/mvcisback/py-aiger-gridworld/branch/master/graph/badge.svg)](https://codecov.io/gh/mvcisback/py-aiger-gridworld)
 [![PyPI version](https://badge.fury.io/py/py-aiger-gridworld.svg)](https://badge.fury.io/py/py-aiger-gridworld)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 <object data="assets/visualization_example.svg" type="image/svg+xml">
   <img src="assets/visualization_example.svg" />
 </object>
```

### Comparing `py-aiger-gridworld-0.4.1/aiger_gridworld/dynamics.py` & `py_aiger_gridworld-0.4.3/aiger_gridworld/dynamics.py`

 * *Files identical despite different names*

### Comparing `py-aiger-gridworld-0.4.1/aiger_gridworld/vis.py` & `py_aiger_gridworld-0.4.3/aiger_gridworld/vis.py`

 * *Files identical despite different names*

### Comparing `py-aiger-gridworld-0.4.1/setup.py` & `py_aiger_gridworld-0.4.3/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,30 +4,30 @@
 packages = \
 ['aiger_gridworld']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['bidict>=0.21.2,<0.22.0',
+['bidict>=0.22,<0.23',
  'funcy>=1.13,<2.0',
  'py-aiger-bv>=4.0.0,<5.0.0',
- 'py-aiger-discrete>=0.1.6,<0.2.0',
+ 'py-aiger-discrete>=0.1.10,<0.2.0',
  'py-aiger>=6.0.0,<7.0.0']
 
 setup_kwargs = {
     'name': 'py-aiger-gridworld',
-    'version': '0.4.1',
+    'version': '0.4.3',
     'description': 'Library for modeling gridworlds as AIGER circuits.',
-    'long_description': '# py-aiger-gridworld\n\nLibrary for modeling gridworlds as AIGER circuits.\n\n[![Build Status](https://cloud.drone.io/api/badges/mvcisback/py-aiger-gridworld/status.svg)](https://cloud.drone.io/mvcisback/py-aiger-gridworld)\n[![codecov](https://codecov.io/gh/mvcisback/py-aiger-gridworld/branch/master/graph/badge.svg)](https://codecov.io/gh/mvcisback/py-aiger-gridworld)\n[![PyPI version](https://badge.fury.io/py/py-aiger-gridworld.svg)](https://badge.fury.io/py/py-aiger-gridworld)\n[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)\n\n<object data="assets/visualization_example.svg" type="image/svg+xml">\n  <img src="assets/visualization_example.svg" />\n</object>\n\n# Installation\n\nIf you just need to use `aiger_gridworld`, you can just run:\n\n`$ pip install py-aiger-gridwolrd`\n\nFor developers, note that this project uses the\n[poetry](https://poetry.eustace.io/) python package/dependency\nmanagement tool. Please familarize yourself with it and then\nrun:\n\n`$ poetry install`\n',
+    'long_description': '# py-aiger-gridworld\n\nLibrary for modeling gridworlds as AIGER circuits.\n\n[![Build Status](https://cloud.drone.io/api/badges/mvcisback/py-aiger-gridworld/status.svg)](https://cloud.drone.io/mvcisback/py-aiger-gridworld)\n[![PyPI version](https://badge.fury.io/py/py-aiger-gridworld.svg)](https://badge.fury.io/py/py-aiger-gridworld)\n[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)\n\n<object data="assets/visualization_example.svg" type="image/svg+xml">\n  <img src="assets/visualization_example.svg" />\n</object>\n\n# Installation\n\nIf you just need to use `aiger_gridworld`, you can just run:\n\n`$ pip install py-aiger-gridwolrd`\n\nFor developers, note that this project uses the\n[poetry](https://poetry.eustace.io/) python package/dependency\nmanagement tool. Please familarize yourself with it and then\nrun:\n\n`$ poetry install`\n',
     'author': 'Marcell Vazquez-Chanlatte',
     'author_email': 'mvc@linux.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.9,<4.0',
 }
```

### Comparing `py-aiger-gridworld-0.4.1/PKG-INFO` & `py_aiger_gridworld-0.4.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: py-aiger-gridworld
-Version: 0.4.1
+Version: 0.4.3
 Summary: Library for modeling gridworlds as AIGER circuits.
 License: MIT
 Author: Marcell Vazquez-Chanlatte
 Author-email: mvc@linux.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: bidict (>=0.21.2,<0.22.0)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: bidict (>=0.22,<0.23)
 Requires-Dist: funcy (>=1.13,<2.0)
 Requires-Dist: py-aiger (>=6.0.0,<7.0.0)
 Requires-Dist: py-aiger-bv (>=4.0.0,<5.0.0)
-Requires-Dist: py-aiger-discrete (>=0.1.6,<0.2.0)
+Requires-Dist: py-aiger-discrete (>=0.1.10,<0.2.0)
 Description-Content-Type: text/markdown
 
 # py-aiger-gridworld
 
 Library for modeling gridworlds as AIGER circuits.
 
 [![Build Status](https://cloud.drone.io/api/badges/mvcisback/py-aiger-gridworld/status.svg)](https://cloud.drone.io/mvcisback/py-aiger-gridworld)
-[![codecov](https://codecov.io/gh/mvcisback/py-aiger-gridworld/branch/master/graph/badge.svg)](https://codecov.io/gh/mvcisback/py-aiger-gridworld)
 [![PyPI version](https://badge.fury.io/py/py-aiger-gridworld.svg)](https://badge.fury.io/py/py-aiger-gridworld)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 <object data="assets/visualization_example.svg" type="image/svg+xml">
   <img src="assets/visualization_example.svg" />
 </object>
```

