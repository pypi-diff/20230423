# Comparing `tmp/chromat-0.0.6.tar.gz` & `tmp/chromat-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chromat-0.0.6.tar", max compression
+gzip compressed data, was "chromat-0.1.0.tar", max compression
```

## Comparing `chromat-0.0.6.tar` & `chromat-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,7 @@
--rw-r--r--   0        0        0      305 2023-04-18 23:53:29.579167 chromat-0.0.6/chromat/__init__.py
--rw-r--r--   0        0        0      164 2023-04-18 23:54:23.722579 chromat-0.0.6/chromat/palette/__init__.py
--rw-r--r--   0        0        0      357 2023-04-18 23:51:06.245326 chromat-0.0.6/chromat/palette/palettes.py
--rw-r--r--   0        0        0      161 2023-04-18 23:43:53.684606 chromat-0.0.6/chromat/swatch/__init__.py
--rw-r--r--   0        0        0     3237 2023-04-18 23:38:19.613861 chromat-0.0.6/chromat/swatch/props.py
--rw-r--r--   0        0        0     5903 2023-04-18 23:58:02.442868 chromat-0.0.6/chromat/swatch/swatches.py
--rw-r--r--   0        0        0      321 2023-04-18 23:41:26.111699 chromat-0.0.6/chromat/utility/__init__.py
--rw-r--r--   0        0        0     1435 2023-04-18 23:45:11.192797 chromat-0.0.6/chromat/utility/colors.py
--rw-r--r--   0        0        0      606 2023-04-18 23:57:36.596032 chromat-0.0.6/chromat/utility/console.py
--rw-r--r--   0        0        0     1375 2023-04-20 04:22:25.092035 chromat-0.0.6/pyproject.toml
--rw-r--r--   0        0        0       96 2023-04-18 06:50:24.406547 chromat-0.0.6/README.md
--rw-r--r--   0        0        0      920 1970-01-01 00:00:00.000000 chromat-0.0.6/setup.py
--rw-r--r--   0        0        0     1226 1970-01-01 00:00:00.000000 chromat-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      146 2023-04-23 20:39:33.813564 chromat-0.1.0/chromat/__init__.py
+-rw-r--r--   0        0        0     1399 2023-04-23 20:46:21.483415 chromat-0.1.0/chromat/palettes.py
+-rw-r--r--   0        0        0     8333 2023-04-23 20:46:28.723422 chromat-0.1.0/chromat/swatches.py
+-rw-r--r--   0        0        0     1383 2023-04-23 21:33:17.858200 chromat-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0       96 2023-04-18 06:50:24.406547 chromat-0.1.0/README.md
+-rw-r--r--   0        0        0      814 1970-01-01 00:00:00.000000 chromat-0.1.0/setup.py
+-rw-r--r--   0        0        0     1150 1970-01-01 00:00:00.000000 chromat-0.1.0/PKG-INFO
```

### Comparing `chromat-0.0.6/pyproject.toml` & `chromat-0.1.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chromat"
-version = "0.0.6"
+version = "0.1.0"
 description = "color palettes! under heavy construction!"
 license = "GPL-3.0-or-later"
 authors = ["hex benjamin <hex@hexbenjam.in>"]
 readme = "README.md"
 repository = "https://github.com/hexbenjamin/chromat"
 keywords = ["color", "palette"]
 classifiers = [
@@ -29,23 +29,23 @@
     ".gitignore",
     ".replit",
     "replit.nix",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.10.0,<3.11"
+rich = "^13.3.4"
+colour = "^0.1.5"
+colorthief = "^0.2.1"
+
+[tool.poetry.group.dev.dependencies]
 numpy = "^1.22.2"
 replit = "^3.2.4"
 Flask = "^2.2.0"
 urllib3 = "^1.26.12"
-rich = "^13.3.4"
-
-[tool.poetry.dev-dependencies]
+black = "^23.3.0"
 debugpy = "^1.6.2"
 replit-python-lsp-server = {extras = ["yapf", "rope", "pyflakes"], version = "^1.5.9"}
 
-[tool.poetry.group.dev.dependencies]
-black = "^23.3.0"
-
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `chromat-0.0.6/setup.py` & `chromat-0.1.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['chromat', 'chromat.palette', 'chromat.swatch', 'chromat.utility']
+['chromat']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['Flask>=2.2.0,<3.0.0',
- 'numpy>=1.22.2,<2.0.0',
- 'replit>=3.2.4,<4.0.0',
- 'rich>=13.3.4,<14.0.0',
- 'urllib3>=1.26.12,<2.0.0']
+['colorthief>=0.2.1,<0.3.0', 'colour>=0.1.5,<0.2.0', 'rich>=13.3.4,<14.0.0']
 
 setup_kwargs = {
     'name': 'chromat',
-    'version': '0.0.6',
+    'version': '0.1.0',
     'description': 'color palettes! under heavy construction!',
     'long_description': '\ufeff# chromat: algorithmic color palettes\ncoming soon!\n\nhttps://github.com/hexbenjamin/chromat',
     'author': 'hex benjamin',
     'author_email': 'hex@hexbenjam.in',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/hexbenjamin/chromat',
```

### Comparing `chromat-0.0.6/PKG-INFO` & `chromat-0.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromat
-Version: 0.0.6
+Version: 0.1.0
 Summary: color palettes! under heavy construction!
 Home-page: https://github.com/hexbenjamin/chromat
 License: GPL-3.0-or-later
 Keywords: color,palette
 Author: hex benjamin
 Author-email: hex@hexbenjam.in
 Requires-Python: >=3.10.0,<3.11
@@ -15,19 +15,17 @@
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Artistic Software
 Classifier: Topic :: Utilities
-Requires-Dist: Flask (>=2.2.0,<3.0.0)
-Requires-Dist: numpy (>=1.22.2,<2.0.0)
-Requires-Dist: replit (>=3.2.4,<4.0.0)
+Requires-Dist: colorthief (>=0.2.1,<0.3.0)
+Requires-Dist: colour (>=0.1.5,<0.2.0)
 Requires-Dist: rich (>=13.3.4,<14.0.0)
-Requires-Dist: urllib3 (>=1.26.12,<2.0.0)
 Project-URL: Repository, https://github.com/hexbenjamin/chromat
 Description-Content-Type: text/markdown
 
 ﻿# chromat: algorithmic color palettes
 coming soon!
 
 https://github.com/hexbenjamin/chromat
```

