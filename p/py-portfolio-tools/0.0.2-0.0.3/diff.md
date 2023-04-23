# Comparing `tmp/py-portfolio-tools-0.0.2.tar.gz` & `tmp/py-portfolio-tools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-portfolio-tools-0.0.2.tar", last modified: Mon Apr 17 12:41:52 2023, max compression
+gzip compressed data, was "py-portfolio-tools-0.0.3.tar", last modified: Sun Apr 23 17:05:07 2023, max compression
```

## Comparing `py-portfolio-tools-0.0.2.tar` & `py-portfolio-tools-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 12:41:52.187679 py-portfolio-tools-0.0.2/
--rw-rw-rw-   0        0        0     1075 2023-04-17 11:45:54.000000 py-portfolio-tools-0.0.2/LICENSE.md
--rw-rw-rw-   0        0        0     1198 2023-04-17 12:41:52.187679 py-portfolio-tools-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       44 2023-04-17 11:54:14.000000 py-portfolio-tools-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 12:41:52.170352 py-portfolio-tools-0.0.2/py-portfolio-tools/
--rw-rw-rw-   0        0        0        0 2023-04-17 11:57:01.000000 py-portfolio-tools-0.0.2/py-portfolio-tools/__init__.py
--rw-rw-rw-   0        0        0       84 2023-04-17 12:05:05.000000 py-portfolio-tools-0.0.2/py-portfolio-tools/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 12:41:52.186676 py-portfolio-tools-0.0.2/py_portfolio_tools.egg-info/
--rw-rw-rw-   0        0        0     1198 2023-04-17 12:41:52.000000 py-portfolio-tools-0.0.2/py_portfolio_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      300 2023-04-17 12:41:52.000000 py-portfolio-tools-0.0.2/py_portfolio_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 12:41:52.000000 py-portfolio-tools-0.0.2/py_portfolio_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-04-17 12:41:52.000000 py-portfolio-tools-0.0.2/py_portfolio_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-17 12:41:52.000000 py-portfolio-tools-0.0.2/py_portfolio_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 12:41:52.187679 py-portfolio-tools-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1576 2023-04-17 12:40:58.000000 py-portfolio-tools-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 17:05:07.423438 py-portfolio-tools-0.0.3/
+-rw-rw-rw-   0        0        0     1075 2023-04-17 11:45:54.000000 py-portfolio-tools-0.0.3/LICENSE.md
+-rw-rw-rw-   0        0        0     1198 2023-04-23 17:05:07.423438 py-portfolio-tools-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2023-04-17 11:54:14.000000 py-portfolio-tools-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 17:05:07.404878 py-portfolio-tools-0.0.3/py-portfolio-tools/
+-rw-rw-rw-   0        0        0     2545 2023-04-17 18:42:57.000000 py-portfolio-tools-0.0.3/py-portfolio-tools/DataFetch.py
+-rw-rw-rw-   0        0        0      703 2023-04-17 13:42:55.000000 py-portfolio-tools-0.0.3/py-portfolio-tools/Logger.py
+-rw-rw-rw-   0        0        0     5878 2023-04-22 19:00:29.000000 py-portfolio-tools-0.0.3/py-portfolio-tools/Portfolio.py
+-rw-rw-rw-   0        0        0     3214 2023-04-22 08:15:11.000000 py-portfolio-tools-0.0.3/py-portfolio-tools/PortfolioInputWindow.py
+-rw-rw-rw-   0        0        0     6325 2023-04-22 08:18:46.000000 py-portfolio-tools-0.0.3/py-portfolio-tools/PortfolioManager.py
+-rw-rw-rw-   0        0        0       30 2023-04-17 14:28:58.000000 py-portfolio-tools-0.0.3/py-portfolio-tools/Predictor.py
+-rw-rw-rw-   0        0        0     2554 2023-04-22 08:12:50.000000 py-portfolio-tools-0.0.3/py-portfolio-tools/Tickers.py
+-rw-rw-rw-   0        0        0     6864 2023-04-22 07:56:08.000000 py-portfolio-tools-0.0.3/py-portfolio-tools/Utils.py
+-rw-rw-rw-   0        0        0      243 2023-04-22 07:44:44.000000 py-portfolio-tools-0.0.3/py-portfolio-tools/__init__.py
+-rw-rw-rw-   0        0        0     1397 2023-04-21 18:15:14.000000 py-portfolio-tools-0.0.3/py-portfolio-tools/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 17:05:07.422440 py-portfolio-tools-0.0.3/py_portfolio_tools.egg-info/
+-rw-rw-rw-   0        0        0     1198 2023-04-23 17:05:07.000000 py-portfolio-tools-0.0.3/py_portfolio_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      565 2023-04-23 17:05:07.000000 py-portfolio-tools-0.0.3/py_portfolio_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 17:05:07.000000 py-portfolio-tools-0.0.3/py_portfolio_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2023-04-23 17:05:07.000000 py-portfolio-tools-0.0.3/py_portfolio_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-23 17:05:07.000000 py-portfolio-tools-0.0.3/py_portfolio_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 17:05:07.423438 py-portfolio-tools-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1633 2023-04-23 17:04:50.000000 py-portfolio-tools-0.0.3/setup.py
```

### Comparing `py-portfolio-tools-0.0.2/LICENSE.md` & `py-portfolio-tools-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `py-portfolio-tools-0.0.2/PKG-INFO` & `py-portfolio-tools-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-portfolio-tools
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python Library and set of GUI tools for Portfolio Management
 Home-page: https://gitlab.com/Jaysmito101/py-portfolio-tools
 Author: Jaysmito Mukherjee
 Author-email: jaysmito101@gmail.com
 License: MIT
 Project-URL: Documentation, https://gitlab.com/Jaysmito101/py-portfolio-tools/-/wikis/Home
 Project-URL: Issue tracker, https://gitlab.com/Jaysmito101/py-portfolio-tools/-/issues
```

### Comparing `py-portfolio-tools-0.0.2/py_portfolio_tools.egg-info/PKG-INFO` & `py-portfolio-tools-0.0.3/py_portfolio_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-portfolio-tools
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python Library and set of GUI tools for Portfolio Management
 Home-page: https://gitlab.com/Jaysmito101/py-portfolio-tools
 Author: Jaysmito Mukherjee
 Author-email: jaysmito101@gmail.com
 License: MIT
 Project-URL: Documentation, https://gitlab.com/Jaysmito101/py-portfolio-tools/-/wikis/Home
 Project-URL: Issue tracker, https://gitlab.com/Jaysmito101/py-portfolio-tools/-/issues
```

### Comparing `py-portfolio-tools-0.0.2/setup.py` & `py-portfolio-tools-0.0.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import re
 
-requirements = ['numpy', 'pandas', 'matplotlib'] 
+requirements = ['numpy', 'pandas', 'matplotlib', 'yfinance', "PyOpenGL", "glfw", "imgui[glfw]", "Pillow"] 
 
-version = '0.0.2'
+version = '0.0.3'
 
 if not version:
     raise RuntimeError('version is not set')
 
 readme = 'Coming Soon ...'
 
 setup(
```

