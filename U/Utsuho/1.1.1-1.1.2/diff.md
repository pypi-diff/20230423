# Comparing `tmp/Utsuho-1.1.1.tar.gz` & `tmp/Utsuho-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/juno/Projects/utsuho/dist/.tmp-bukvldrb/Utsuho-1.1.1.tar", last modified: Thu Apr  6 16:32:26 2023, max compression
+gzip compressed data, was "/Users/juno/Projects/utsuho/dist/.tmp-wt37ws0f/Utsuho-1.1.2.tar", last modified: Sun Apr 23 10:28:02 2023, max compression
```

## Comparing `Utsuho-1.1.1.tar` & `Utsuho-1.1.2.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 juno       (501) staff       (20)        0 2023-04-06 16:32:26.000000 Utsuho-1.1.1/
--rw-r--r--   0 juno       (501) staff       (20)      558 2023-04-05 13:04:55.000000 Utsuho-1.1.1/LICENSE
--rw-r--r--   0 juno       (501) staff       (20)     2124 2023-04-06 16:32:26.000000 Utsuho-1.1.1/PKG-INFO
--rw-r--r--   0 juno       (501) staff       (20)     1446 2023-04-05 13:04:55.000000 Utsuho-1.1.1/README.md
--rw-r--r--   0 juno       (501) staff       (20)     1456 2023-04-06 16:23:35.000000 Utsuho-1.1.1/pyproject.toml
--rw-r--r--   0 juno       (501) staff       (20)       38 2023-04-06 16:32:26.000000 Utsuho-1.1.1/setup.cfg
-drwxr-xr-x   0 juno       (501) staff       (20)        0 2023-04-06 16:32:26.000000 Utsuho-1.1.1/src/
-drwxr-xr-x   0 juno       (501) staff       (20)        0 2023-04-06 16:32:26.000000 Utsuho-1.1.1/src/Utsuho.egg-info/
--rw-r--r--   0 juno       (501) staff       (20)     2124 2023-04-06 16:32:26.000000 Utsuho-1.1.1/src/Utsuho.egg-info/PKG-INFO
--rw-r--r--   0 juno       (501) staff       (20)      243 2023-04-06 16:32:26.000000 Utsuho-1.1.1/src/Utsuho.egg-info/SOURCES.txt
--rw-r--r--   0 juno       (501) staff       (20)        1 2023-04-06 16:32:26.000000 Utsuho-1.1.1/src/Utsuho.egg-info/dependency_links.txt
--rw-r--r--   0 juno       (501) staff       (20)      210 2023-04-06 16:32:26.000000 Utsuho-1.1.1/src/Utsuho.egg-info/requires.txt
--rw-r--r--   0 juno       (501) staff       (20)        7 2023-04-06 16:32:26.000000 Utsuho-1.1.1/src/Utsuho.egg-info/top_level.txt
-drwxr-xr-x   0 juno       (501) staff       (20)        0 2023-04-06 16:32:26.000000 Utsuho-1.1.1/src/utsuho/
--rw-r--r--   0 juno       (501) staff       (20)     8193 2023-04-06 16:23:35.000000 Utsuho-1.1.1/src/utsuho/__init__.py
--rw-r--r--   0 juno       (501) staff       (20)     7423 2023-04-05 13:04:55.000000 Utsuho-1.1.1/src/utsuho/maps.py
+drwxr-xr-x   0 juno       (501) staff       (20)        0 2023-04-23 10:28:02.000000 Utsuho-1.1.2/
+-rw-r--r--   0 juno       (501) staff       (20)      558 2023-04-05 13:04:55.000000 Utsuho-1.1.2/LICENSE
+-rw-r--r--   0 juno       (501) staff       (20)     3237 2023-04-23 10:28:02.000000 Utsuho-1.1.2/PKG-INFO
+-rw-r--r--   0 juno       (501) staff       (20)     2559 2023-04-23 10:25:06.000000 Utsuho-1.1.2/README.md
+-rw-r--r--   0 juno       (501) staff       (20)     1515 2023-04-23 10:25:06.000000 Utsuho-1.1.2/pyproject.toml
+-rw-r--r--   0 juno       (501) staff       (20)       38 2023-04-23 10:28:02.000000 Utsuho-1.1.2/setup.cfg
+drwxr-xr-x   0 juno       (501) staff       (20)        0 2023-04-23 10:28:02.000000 Utsuho-1.1.2/src/
+drwxr-xr-x   0 juno       (501) staff       (20)        0 2023-04-23 10:28:02.000000 Utsuho-1.1.2/src/Utsuho.egg-info/
+-rw-r--r--   0 juno       (501) staff       (20)     3237 2023-04-23 10:28:02.000000 Utsuho-1.1.2/src/Utsuho.egg-info/PKG-INFO
+-rw-r--r--   0 juno       (501) staff       (20)      323 2023-04-23 10:28:02.000000 Utsuho-1.1.2/src/Utsuho.egg-info/SOURCES.txt
+-rw-r--r--   0 juno       (501) staff       (20)        1 2023-04-23 10:28:02.000000 Utsuho-1.1.2/src/Utsuho.egg-info/dependency_links.txt
+-rw-r--r--   0 juno       (501) staff       (20)       42 2023-04-23 10:28:02.000000 Utsuho-1.1.2/src/Utsuho.egg-info/entry_points.txt
+-rw-r--r--   0 juno       (501) staff       (20)      223 2023-04-23 10:28:02.000000 Utsuho-1.1.2/src/Utsuho.egg-info/requires.txt
+-rw-r--r--   0 juno       (501) staff       (20)        7 2023-04-23 10:28:02.000000 Utsuho-1.1.2/src/Utsuho.egg-info/top_level.txt
+drwxr-xr-x   0 juno       (501) staff       (20)        0 2023-04-23 10:28:02.000000 Utsuho-1.1.2/src/utsuho/
+-rw-r--r--   0 juno       (501) staff       (20)      203 2023-04-23 10:25:06.000000 Utsuho-1.1.2/src/utsuho/__init__.py
+-rw-r--r--   0 juno       (501) staff       (20)     2091 2023-04-23 10:25:06.000000 Utsuho-1.1.2/src/utsuho/cli.py
+-rw-r--r--   0 juno       (501) staff       (20)     8092 2023-04-23 10:25:06.000000 Utsuho-1.1.2/src/utsuho/converters.py
+-rw-r--r--   0 juno       (501) staff       (20)     6329 2023-04-23 10:25:06.000000 Utsuho-1.1.2/src/utsuho/maps.py
```

### Comparing `Utsuho-1.1.1/LICENSE` & `Utsuho-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Utsuho-1.1.1/PKG-INFO` & `Utsuho-1.1.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,15 @@
-Metadata-Version: 2.1
-Name: Utsuho
-Version: 1.1.1
-Summary: Utsuho is a Python module that provides interconversion between Japanese half-width katakana and full-width katakana.
-Author-email: Nobuyuki Sekimori <43375309+juno-rmks@users.noreply.github.com>
-Project-URL: Source Code, https://github.com/juno-rmks/utsuho/
-Project-URL: Documentation, https://utsuho.readthedocs.io/
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: dev
-Provides-Extra: docs
-License-File: LICENSE
-
 # Utsuho
 
 Utsuho is a Python module that provides interconversion between Japanese half-width katakana and full-width katakana.
 
 The name Utsuho comes from the long story "Utsuho Monogatari," which is said to have been written in the middle of the Heian period, and contains descriptions of katakana.
 
+**Utsuho は、日本語を取り扱う Python モジュールであり、日本語を母語とするユーザーを想定しているため、Issue や Discussion を日本語で投稿いただいて構いません。**
+
 ## Installing
 
 Install and update using pip:
 
 ```sh
 pip install Utsuho
 ```
@@ -57,10 +42,62 @@
 
 ## License
 
 This project is licensed under the terms of the Apache license 2.0.
 
 See the ["LICENSE"](https://github.com/juno-rmks/utsuho/blob/main/LICENSE) file for license rights and limitations.
 
+## Development
+
+**This is just a note for me.**
+
+Create a Python virtual environment and activate it.
+
+```console
+% python -m venv .venv
+% . .venv/bin/activate
+```
+
+Install Utsuho locally with `--editable` option.
+
+```console
+% pip install -e .
+% pip install -e .[test]
+% pip install -e .[dev]
+% pip install -e .[docs]
+```
+
+### Update API Reference
+
+Update the documentation source to match the current source structure.
+
+```console
+% sphinx-apidoc -f -T -e -M -o docs/source src
+```
+
+### Build and Publish Package
+
+Generate the distribution archive.
+
+```console
+python -m build
+```
+
+Upload the distribution archive to Test PyPi.
+
+```console
+python -m twine upload --repository testpypi dist/*
+Enter your username: __token__
+Enter your password:
+```
+
+Upload the distribution archive to PyPi.
+
+```console
+python -m twine upload dist/*
+Enter your username: __token__
+Enter your password:
+```
+
 ## Links
 
 * [Utsuho document](https://utsuho.readthedocs.io/ja/latest/)
```

### Comparing `Utsuho-1.1.1/pyproject.toml` & `Utsuho-1.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
 ]
 readme = "README.md"
 requires-python = ">=3.7"
-dependencies = []
+dependencies = ["click>=8.1.3"]
 dynamic = ["version"]
 
 [project.urls]
 "Source Code" = "https://github.com/juno-rmks/utsuho/"
 "Documentation" = "https://utsuho.readthedocs.io/"
 
 [project.optional-dependencies]
@@ -28,14 +28,17 @@
 docs = [
     "Sphinx==5.3.0",
     "sphinx-intl==2.1.0",
     "sphinx-rtd-theme==1.2.0",
     "myst-parser==1.0.0",
 ]
 
+[project.scripts]
+utsuho = "utsuho.cli:cli"
+
 [tool.setuptools.dynamic]
 version = { attr = "utsuho.__version__" }
 
 [tool.autopep8]
 max_line_length = 159
 
 [tool.isort]
```

### Comparing `Utsuho-1.1.1/src/utsuho/__init__.py` & `Utsuho-1.1.2/src/utsuho/converters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""" Utsuho is an interconverter between Japanese half-width katakana and full-width katakana.
+""" Converters.
 """
 from dataclasses import dataclass
 
 from .maps import (
     full_to_half_ascii_alphabet_map,
     full_to_half_ascii_digit_map,
     full_to_half_ascii_symbol_map,
@@ -22,16 +22,14 @@
     half_to_full_length_mark_map,
     half_to_full_letter_map,
     half_to_full_punctuation_map,
     half_to_full_space_map,
     half_to_full_voicing_mark_map
 )
 
-__version__ = '1.1.1'
-
 
 @dataclass
 class ConverterConfig():
     """ Configuration of whether to convert non-katakana characters.
 
     Parameters
     ----------
```

