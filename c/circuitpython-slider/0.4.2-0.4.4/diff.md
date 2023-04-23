# Comparing `tmp/circuitpython-slider-0.4.2.tar.gz` & `tmp/circuitpython-slider-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-slider-0.4.2.tar", last modified: Tue Jan 31 00:41:32 2023, max compression
+gzip compressed data, was "circuitpython-slider-0.4.4.tar", last modified: Sun Apr 23 18:42:40 2023, max compression
```

## Comparing `circuitpython-slider-0.4.2.tar` & `circuitpython-slider-0.4.4.tar`

### file list

```diff
@@ -1,46 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 00:41:32.263971 circuitpython-slider-0.4.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 00:41:32.259971 circuitpython-slider-0.4.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 00:41:32.259971 circuitpython-slider-0.4.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-01-31 00:41:11.000000 circuitpython-slider-0.4.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-01-31 00:41:11.000000 circuitpython-slider-0.4.2/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-01-31 00:41:11.000000 circuitpython-slider-0.4.2/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-01-31 00:41:11.000000 circuitpython-slider-0.4.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-01-31 00:41:11.000000 circuitpython-slider-0.4.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-01-31 00:41:11.000000 circuitpython-slider-0.4.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-01-31 00:41:11.000000 circuitpython-slider-0.4.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-01-31 00:41:11.000000 circuitpython-slider-0.4.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-01-31 00:41:11.000000 circuitpython-slider-0.4.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 00:41:32.259971 circuitpython-slider-0.4.2/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-01-31 00:41:11.000000 circuitpython-slider-0.4.2/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-01-31 00:41:11.000000 circuitpython-slider-0.4.2/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-01-31 00:41:11.000000 circuitpython-slider-0.4.2/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-01-31 00:41:32.263971 circuitpython-slider-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-01-31 00:41:11.000000 circuitpython-slider-0.4.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-01-31 00:41:11.000000 circuitpython-slider-0.4.2/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 00:41:32.259971 circuitpython-slider-0.4.2/circuitpython_slider.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-01-31 00:41:32.000000 circuitpython-slider-0.4.2/circuitpython_slider.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-01-31 00:41:32.000000 circuitpython-slider-0.4.2/circuitpython_slider.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 00:41:32.000000 circuitpython-slider-0.4.2/circuitpython_slider.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-01-31 00:41:32.000000 circuitpython-slider-0.4.2/circuitpython_slider.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-01-31 00:41:32.000000 circuitpython-slider-0.4.2/circuitpython_slider.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 00:41:32.263971 circuitpython-slider-0.4.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 00:41:32.263971 circuitpython-slider-0.4.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-01-31 00:41:11.000000 circuitpython-slider-0.4.2/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-01-31 00:41:11.000000 circuitpython-slider-0.4.2/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-01-31 00:41:11.000000 circuitpython-slider-0.4.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-01-31 00:41:11.000000 circuitpython-slider-0.4.2/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-01-31 00:41:11.000000 circuitpython-slider-0.4.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-01-31 00:41:11.000000 circuitpython-slider-0.4.2/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-01-31 00:41:11.000000 circuitpython-slider-0.4.2/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-01-31 00:41:11.000000 circuitpython-slider-0.4.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-01-31 00:41:11.000000 circuitpython-slider-0.4.2/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-01-31 00:41:11.000000 circuitpython-slider-0.4.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-01-31 00:41:11.000000 circuitpython-slider-0.4.2/docs/slider.png
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-01-31 00:41:11.000000 circuitpython-slider-0.4.2/docs/slider.png.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 00:41:32.263971 circuitpython-slider-0.4.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-01-31 00:41:24.000000 circuitpython-slider-0.4.2/examples/slider_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-01-31 00:41:24.000000 circuitpython-slider-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-01-31 00:41:11.000000 circuitpython-slider-0.4.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-31 00:41:32.263971 circuitpython-slider-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-01-31 00:41:24.000000 circuitpython-slider-0.4.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    10393 2023-01-31 00:41:24.000000 circuitpython-slider-0.4.2/slider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:42:40.481022 circuitpython-slider-0.4.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:42:40.473022 circuitpython-slider-0.4.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:42:40.477022 circuitpython-slider-0.4.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-23 18:42:23.000000 circuitpython-slider-0.4.4/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-23 18:42:23.000000 circuitpython-slider-0.4.4/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-23 18:42:23.000000 circuitpython-slider-0.4.4/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-23 18:42:23.000000 circuitpython-slider-0.4.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-23 18:42:23.000000 circuitpython-slider-0.4.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-23 18:42:23.000000 circuitpython-slider-0.4.4/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-23 18:42:23.000000 circuitpython-slider-0.4.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-04-23 18:42:23.000000 circuitpython-slider-0.4.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-23 18:42:23.000000 circuitpython-slider-0.4.4/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:42:40.477022 circuitpython-slider-0.4.4/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-23 18:42:23.000000 circuitpython-slider-0.4.4/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-23 18:42:23.000000 circuitpython-slider-0.4.4/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-23 18:42:23.000000 circuitpython-slider-0.4.4/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-04-23 18:42:40.477022 circuitpython-slider-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-23 18:42:23.000000 circuitpython-slider-0.4.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-23 18:42:23.000000 circuitpython-slider-0.4.4/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:42:40.477022 circuitpython-slider-0.4.4/circuitpython_slider.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-04-23 18:42:40.000000 circuitpython-slider-0.4.4/circuitpython_slider.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-23 18:42:40.000000 circuitpython-slider-0.4.4/circuitpython_slider.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 18:42:40.000000 circuitpython-slider-0.4.4/circuitpython_slider.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-23 18:42:40.000000 circuitpython-slider-0.4.4/circuitpython_slider.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-23 18:42:40.000000 circuitpython-slider-0.4.4/circuitpython_slider.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:42:40.477022 circuitpython-slider-0.4.4/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:42:40.477022 circuitpython-slider-0.4.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-23 18:42:23.000000 circuitpython-slider-0.4.4/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-23 18:42:23.000000 circuitpython-slider-0.4.4/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-23 18:42:23.000000 circuitpython-slider-0.4.4/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-23 18:42:23.000000 circuitpython-slider-0.4.4/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-04-23 18:42:23.000000 circuitpython-slider-0.4.4/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-23 18:42:23.000000 circuitpython-slider-0.4.4/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-23 18:42:23.000000 circuitpython-slider-0.4.4/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-23 18:42:23.000000 circuitpython-slider-0.4.4/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-04-23 18:42:23.000000 circuitpython-slider-0.4.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-23 18:42:23.000000 circuitpython-slider-0.4.4/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-23 18:42:23.000000 circuitpython-slider-0.4.4/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-23 18:42:23.000000 circuitpython-slider-0.4.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-23 18:42:23.000000 circuitpython-slider-0.4.4/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-23 18:42:23.000000 circuitpython-slider-0.4.4/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-23 18:42:23.000000 circuitpython-slider-0.4.4/docs/slider.png
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-23 18:42:23.000000 circuitpython-slider-0.4.4/docs/slider.png.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:42:40.477022 circuitpython-slider-0.4.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-23 18:42:33.000000 circuitpython-slider-0.4.4/examples/slider_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-04-23 18:42:33.000000 circuitpython-slider-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-23 18:42:23.000000 circuitpython-slider-0.4.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 18:42:40.481022 circuitpython-slider-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-04-23 18:42:33.000000 circuitpython-slider-0.4.4/slider.py
```

### Comparing `circuitpython-slider-0.4.2/.pre-commit-config.yaml` & `circuitpython-slider-0.4.4/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -3,18 +3,14 @@
 # SPDX-License-Identifier: Unlicense
 
 repos:
   - repo: https://github.com/python/black
     rev: 22.3.0
     hooks:
       - id: black
-  - repo: https://github.com/fsfe/reuse-tool
-    rev: v0.14.0
-    hooks:
-      - id: reuse
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.2.0
     hooks:
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/pycqa/pylint
```

### Comparing `circuitpython-slider-0.4.2/.pylintrc` & `circuitpython-slider-0.4.4/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython-slider-0.4.2/CODE_OF_CONDUCT.md` & `circuitpython-slider-0.4.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `circuitpython-slider-0.4.2/LICENSE` & `circuitpython-slider-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-slider-0.4.2/LICENSES/CC-BY-4.0.txt` & `circuitpython-slider-0.4.4/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-slider-0.4.2/LICENSES/MIT.txt` & `circuitpython-slider-0.4.4/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-slider-0.4.2/LICENSES/Unlicense.txt` & `circuitpython-slider-0.4.4/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-slider-0.4.2/PKG-INFO` & `circuitpython-slider-0.4.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: circuitpython-slider
-Version: 0.4.2
+Version: 0.4.4
 Summary: CircuitPython slider Library
-Home-page: https://github.com/jposada202020/CircuitPython_slider.git
-Author: Jose David M.
 Author-email: "Jose D. Montoya" <slider@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_slider.git
 Keywords: hardware,micropython,circuitpython,graphic,widget,displayio,slider
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
@@ -27,14 +25,22 @@
     :alt: Documentation Status
 
 
 .. image:: https://github.com/jposada202020/CircuitPython_slider/workflows/Build%20CI/badge.svg
     :target: https://github.com/jposada202020/CircuitPython_slider/actions
     :alt: Build Status
 
+.. image:: https://img.shields.io/pypi/v/circuitpython-slider.svg
+    :alt: latest version on PyPI
+    :target: https://pypi.python.org/pypi/circuitpython-slider
+
+.. image:: https://static.pepy.tech/personalized-badge/circuitpython-slider?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Pypi%20Downloads
+    :alt: Total PyPI downloads
+    :target: https://pepy.tech/project/circuitpython-slider
+
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 slider widget to work with non discrete values in touch resistive screens
```

### Comparing `circuitpython-slider-0.4.2/README.rst` & `circuitpython-slider-0.4.4/README.rst`

 * *Files 19% similar despite different names*

```diff
@@ -7,14 +7,22 @@
     :alt: Documentation Status
 
 
 .. image:: https://github.com/jposada202020/CircuitPython_slider/workflows/Build%20CI/badge.svg
     :target: https://github.com/jposada202020/CircuitPython_slider/actions
     :alt: Build Status
 
+.. image:: https://img.shields.io/pypi/v/circuitpython-slider.svg
+    :alt: latest version on PyPI
+    :target: https://pypi.python.org/pypi/circuitpython-slider
+
+.. image:: https://static.pepy.tech/personalized-badge/circuitpython-slider?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Pypi%20Downloads
+    :alt: Total PyPI downloads
+    :target: https://pepy.tech/project/circuitpython-slider
+
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 slider widget to work with non discrete values in touch resistive screens
```

### Comparing `circuitpython-slider-0.4.2/circuitpython_slider.egg-info/PKG-INFO` & `circuitpython-slider-0.4.4/circuitpython_slider.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: circuitpython-slider
-Version: 0.4.2
+Version: 0.4.4
 Summary: CircuitPython slider Library
-Home-page: https://github.com/jposada202020/CircuitPython_slider.git
-Author: Jose David M.
 Author-email: "Jose D. Montoya" <slider@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_slider.git
 Keywords: hardware,micropython,circuitpython,graphic,widget,displayio,slider
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
@@ -27,14 +25,22 @@
     :alt: Documentation Status
 
 
 .. image:: https://github.com/jposada202020/CircuitPython_slider/workflows/Build%20CI/badge.svg
     :target: https://github.com/jposada202020/CircuitPython_slider/actions
     :alt: Build Status
 
+.. image:: https://img.shields.io/pypi/v/circuitpython-slider.svg
+    :alt: latest version on PyPI
+    :target: https://pypi.python.org/pypi/circuitpython-slider
+
+.. image:: https://static.pepy.tech/personalized-badge/circuitpython-slider?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Pypi%20Downloads
+    :alt: Total PyPI downloads
+    :target: https://pepy.tech/project/circuitpython-slider
+
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 slider widget to work with non discrete values in touch resistive screens
```

### Comparing `circuitpython-slider-0.4.2/circuitpython_slider.egg-info/SOURCES.txt` & `circuitpython-slider-0.4.4/circuitpython_slider.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 .readthedocs.yml
 CODE_OF_CONDUCT.md
 LICENSE
 README.rst
 README.rst.license
 pyproject.toml
 requirements.txt
-setup.py
 slider.py
 .github/workflows/build.yml
 .github/workflows/release_gh.yml
 .github/workflows/release_pypi.yml
 LICENSES/CC-BY-4.0.txt
 LICENSES/MIT.txt
 LICENSES/Unlicense.txt
@@ -27,10 +26,14 @@
 docs/examples.rst
 docs/examples.rst.license
 docs/index.rst
 docs/index.rst.license
 docs/requirements.txt
 docs/slider.png
 docs/slider.png.license
+docs/_static/Logo.png
+docs/_static/Logo.png.license
+docs/_static/extra_css.css
+docs/_static/extra_css.css.license
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
 examples/slider_simpletest.py
```

### Comparing `circuitpython-slider-0.4.2/docs/conf.py` & `circuitpython-slider-0.4.4/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,18 @@
     "displayio",
     "adafruit_displayio_layout",
 ]
 
 
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3.4", None),
+    "adafruit_displayio_layout": (
+        "https://circuitpython.readthedocs.io/projects/displayio-layout/en/latest/",
+        None,
+    ),
     "CircuitPython": ("https://circuitpython.readthedocs.io/en/latest/", None),
 }
 
 # Show the docstring from both the class and its __init__() method.
 autoclass_content = "both"
 
 # Add any paths that contain templates here, relative to this directory.
```

### Comparing `circuitpython-slider-0.4.2/docs/slider.png` & `circuitpython-slider-0.4.4/docs/slider.png`

 * *Files identical despite different names*

### Comparing `circuitpython-slider-0.4.2/examples/slider_simpletest.py` & `circuitpython-slider-0.4.4/examples/slider_simpletest.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     calibration=((5200, 59000), (5800, 57000)),
     size=(display.width, display.height),
 )
 
 # Create the slider
 my_slider = Slider(20, 30)
 
-my_group = displayio.Group(max_size=5)
+my_group = displayio.Group()
 my_group.append(my_slider)
 
 # Add my_group to the display
 display.show(my_group)
 
 # Start the main loop
 while True:
```

### Comparing `circuitpython-slider-0.4.2/pyproject.toml` & `circuitpython-slider-0.4.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-slider"
 description = "CircuitPython slider Library"
-version = "0.4.2"
+version = "0.4.4"
 readme = "README.rst"
 authors = [
     {name = "Jose D. Montoya", email = "slider@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/CircuitPython_slider.git"}
 keywords = [
     "hardware",
```

### Comparing `circuitpython-slider-0.4.2/slider.py` & `circuitpython-slider-0.4.4/slider.py`

 * *Files 16% similar despite different names*

```diff
@@ -48,46 +48,47 @@
 
 class Slider(Widget, Control):
     """
 
     :param int x: pixel position, defaults to 0
     :param int y: pixel position, defaults to 0
     :param int width: width of the slider in pixels. It is recommended to use 100
-     the height will auto-size relative to the width, defaults to 100
+     the height will auto-size relative to the width. Defaults to :const:`100`
     :param int height: height of the slider in pixels, defaults to 40 pixels
     :param int touch_padding: the width of an additional border surrounding the switch
      that extends the touch response boundary, defaults to 0
 
     :param anchor_point: starting point for the annotation line, where ``anchor_point`` is
      an (A,B) tuple in relative units of the size of the widget, for example (0.0, 0.0) is
-     the upper left corner, and (1.0, 1.0) is the lower      right corner of the widget.
-     If ``anchor_point`` is `None`, then ``anchored_position`` is used to set the
-     annotation line starting point, in widget size relative units (default is (0.0, 0.0)).
+     the upper left corner, and (1.0, 1.0) is the lower right corner of the widget.
+     If :attr:`anchor_point` is `None`, then :attr:`anchored_position` is used to set the
+     annotation line starting point, in widget size relative units.
+     Defaults to :const:`(0.0, 0.0)`
     :type anchor_point: Tuple[float, float]
 
     :param anchored_position: pixel position starting point for the annotation line
-     where ``anchored_position`` is an (x,y) tuple in pixel units relative to the
+     where :attr:`anchored_position` is an (x,y) tuple in pixel units relative to the
      upper left corner of the widget, in pixel units (default is None).
     :type anchored_position: Tuple[int, int]
 
     :param fill_color: (*RGB tuple or 24-bit hex value*) slider fill color, default
-     is ``(66, 44, 66)`` gray.
+     is :const:`(66, 44, 66)` gray.
     :param outline_color: (*RGB tuple or 24-bit hex value*) slider outline color,
-     default is ``(30, 30, 30)`` dark gray.
+     default is :const:`(30, 30, 30)` dark gray.
     :param background_color: (*RGB tuple or 24-bit hex value*) background color,
-     default is ``(255, 255, 255)`` white
+     default is :const:`(255, 255, 255)` white
 
     :param int switch_stroke: outline stroke width for the switch and background, in pixels,
      default is 2
     :param Boolean value: the initial value for the switch, default is False
 
 
     **Quickstart: Importing and using Slider**
 
-    Here is one way of importing the ``Slider`` class so you can use it as
+    Here is one way of importing the `Slider` class so you can use it as
     the name ``Slider``:
 
     .. code-block:: python
 
         from adafruit_displayio_layout.widgets.slider import Slider
 
     Now you can create a Slider at pixel position x=20, y=30 using:
@@ -105,43 +106,43 @@
     If you want to have multiple display elements, you can create a group and then
     append the slider and the other elements to the group.  Then, you can add the full
     group to the display as in this example:
 
     .. code-block:: python
 
         my_slider= Slider(20, 30)
-        my_group = displayio.Group(max_size=10) # make a group that can hold 10 items
+        my_group = displayio.Group() # make a group
         my_group.append(my_slider) # Add my_slider to the group
 
         #
         # Append other display elements to the group
         #
 
         display.show(my_group) # add the group to the display
 
 
     **Summary: Slider Features and input variables**
 
     The ``Slider`` widget has some options for controlling its position, visible appearance,
     and value through a collection of input variables:
 
-        - **position**: ``x``, ``y`` or ``anchor_point`` and ``anchored_position``
+        - **position**: :const:`x`, ``y`` or ``anchor_point`` and ``anchored_position``
 
-        - **size**: ``width`` and ``height`` (recommend to leave ``height`` = None to use
+        - **size**: :const:`width` and ``height`` (recommend to leave ``height`` = None to use
           preferred aspect ratio)
 
-        - **switch color**: ``fill_color``, ``outline_color``
+        - **switch color**: :const:`fill_color`, :const:`outline_color`
 
-        - **background color**: ``background_color``
+        - **background color**: :const:`background_color`
 
-        - **linewidths**: ``switch_stroke``
+        - **linewidths**: :const:`switch_stroke`
 
         - **value**: Set ``value`` to the initial value (True or False)
 
-        - **touch boundaries**: ``touch_padding`` defines the number of additional pixels
+        - **touch boundaries**: :attr:`touch_padding` defines the number of additional pixels
           surrounding the switch that should respond to a touch.  (Note: The ``touch_padding``
           variable updates the ``touch_boundary`` Control class variable.  The definition of
           the ``touch_boundary`` is used to determine the region on the Widget that returns
           `True` in the `when_inside` function.)
 
     **The Slider Widget**
 
@@ -152,14 +153,23 @@
        :alt: Diagram of the slider widget.
 
        This is a diagram of a slider with component parts
 
 
     """
 
+    # TODO: [ ] graphics: The slider can go outside the backgroundbox’s             [BUG]
+    #       [ ] range, if slid all the way to the right side.touch behavior:
+    #           The slider does not “center” on the touch point                    [IMPROVEMENT]
+    #       [ ] Touch_Down vs Touch_Move                                           [LONG-THERM]
+    #           Not designed as drag and move. Is desired like
+    #           this to point and select. Maybe could be a parameter
+    #       [ ] Touch MOVE outside box                                              [IMPROVEMENT]
+    #       [ ] Slow Down With movement. No design to act as drag and move          [LONG-THERM]
+
     # pylint: disable=too-many-instance-attributes, too-many-arguments, too-many-locals
     # pylint: disable=too-many-branches, too-many-statements
     def __init__(
         self,
         x: int = 0,
         y: int = 0,
         width: int = 100,  # recommend to default to
@@ -170,32 +180,31 @@
         fill_color: Tuple[int, int, int] = (66, 44, 66),
         outline_color: Tuple[int, int, int] = (30, 30, 30),
         background_color: Tuple[int, int, int] = (255, 255, 255),
         value: bool = False,
         **kwargs,
     ):
 
-        Widget.__init__(
-            self, x=x, y=y, height=height, width=width, **kwargs, max_size=4
-        )
+        Widget.__init__(self, x=x, y=y, height=height, width=width, **kwargs)
         Control.__init__(self)
 
         self._knob_width = height // 2
         self._knob_height = height
 
         self._knob_x = self._knob_width
         self._knob_y = self._knob_height
 
         self._slider_height = height // 5
 
         self._height = self.height
 
         # pylint: disable=access-member-before-definition)
+
         if self._width is None:
-            self._width = 50
+            self._width = 100
         else:
             self._width = self.width
 
         self._fill_color = fill_color
         self._outline_color = outline_color
         self._background_color = background_color
 
@@ -284,44 +293,49 @@
     def _draw_position(self, position):
         # apply the "easing" function to the requested position to adjust motion
         position = easing(position)
 
         # Get the position offset from the motion function
         x_offset, y_offset = self._get_offset_position(position)
 
-        # Update the switch and text x- and y-positions
+        # Update the switch x- and y-positions
         self._switch_handle.x = self._switch_initial_x + x_offset
         self._switch_handle.y = self._switch_initial_y + y_offset
 
     def when_selected(self, touch_point):
         """
         Manages internal logic when widget is selected
         """
 
-        touch_x = touch_point[0] - self.x
+        if touch_point[0] <= self.x + self._knob_width:
+            print("maayor", touch_point[0])
+            touch_x = touch_point[0] - self.x
+        else:
+            print("menor", touch_point[0])
+            touch_x = touch_point[0] - self.x - self._knob_width
+
         touch_y = touch_point[1] - self.y
 
+        self.selected((touch_x, touch_y, 0))
         self._switch_handle.x = touch_x
-
-        super().selected((touch_x, touch_y, 0))
         return self._switch_handle.x
 
     def when_inside(self, touch_point):
         """Checks if the Widget was touched.
 
         :param touch_point: x,y location of the screen, in absolute display coordinates.
         :return: Boolean
 
         """
         touch_x = (
             touch_point[0] - self.x
         )  # adjust touch position for the local position
         touch_y = touch_point[1] - self.y
 
-        return super().contains((touch_x, touch_y, 0))
+        return self.contains((touch_x, touch_y, 0))
 
     @property
     def value(self):
         """The current switch value (Boolean).
 
         :return: Boolean
         """
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

