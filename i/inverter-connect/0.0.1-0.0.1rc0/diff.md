# Comparing `tmp/inverter-connect-0.0.1.tar.gz` & `tmp/inverter-connect-0.0.1rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inverter-connect-0.0.1.tar", last modified: Sun Apr 23 16:18:41 2023, max compression
+gzip compressed data, was "inverter-connect-0.0.1rc0.tar", last modified: Fri Apr 21 07:05:50 2023, max compression
```

## Comparing `inverter-connect-0.0.1.tar` & `inverter-connect-0.0.1rc0.tar`

### file list

```diff
@@ -1,51 +1,48 @@
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-23 16:18:41.094645 inverter-connect-0.0.1/
--rw-rw-r--   0 jens      (1000) users      (100)      301 2023-04-13 15:18:51.000000 inverter-connect-0.0.1/.editorconfig
--rw-rw-r--   0 jens      (1000) users      (100)      153 2023-04-13 15:18:51.000000 inverter-connect-0.0.1/.flake8
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-23 16:18:41.094645 inverter-connect-0.0.1/.github/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-23 16:18:41.094645 inverter-connect-0.0.1/.github/workflows/
--rw-rw-r--   0 jens      (1000) users      (100)     1460 2023-04-19 06:56:31.000000 inverter-connect-0.0.1/.github/workflows/tests.yml
--rw-rw-r--   0 jens      (1000) users      (100)      118 2023-04-13 15:18:51.000000 inverter-connect-0.0.1/.gitignore
--rw-rw-r--   0 jens      (1000) users      (100)     8827 2023-04-23 16:18:41.094645 inverter-connect-0.0.1/PKG-INFO
--rw-rw-r--   0 jens      (1000) users      (100)     8413 2023-04-23 15:55:16.000000 inverter-connect-0.0.1/README.md
--rwxrwxr-x   0 jens      (1000) users      (100)     3047 2023-04-20 19:23:05.000000 inverter-connect-0.0.1/cli.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-23 16:18:41.094645 inverter-connect-0.0.1/inverter/
--rw-rw-r--   0 jens      (1000) users      (100)      301 2023-04-17 13:29:40.000000 inverter-connect-0.0.1/inverter/.editorconfig
--rw-rw-r--   0 jens      (1000) users      (100)      153 2023-04-17 13:29:40.000000 inverter-connect-0.0.1/inverter/.flake8
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-23 16:18:41.094645 inverter-connect-0.0.1/inverter/.github/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-23 16:18:41.094645 inverter-connect-0.0.1/inverter/.github/workflows/
--rw-rw-r--   0 jens      (1000) users      (100)     1460 2023-04-17 13:29:40.000000 inverter-connect-0.0.1/inverter/.github/workflows/tests.yml
--rw-rw-r--   0 jens      (1000) users      (100)      118 2023-04-17 13:29:40.000000 inverter-connect-0.0.1/inverter/.gitignore
--rw-rw-r--   0 jens      (1000) users      (100)      148 2023-04-23 15:55:16.000000 inverter-connect-0.0.1/inverter/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)      186 2023-04-20 19:23:05.000000 inverter-connect-0.0.1/inverter/__main__.py
--rw-rw-r--   0 jens      (1000) users      (100)     3035 2023-04-23 15:59:09.000000 inverter-connect-0.0.1/inverter/api.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-23 16:18:41.094645 inverter-connect-0.0.1/inverter/cli/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-17 13:29:40.000000 inverter-connect-0.0.1/inverter/cli/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)    11425 2023-04-23 16:17:35.000000 inverter-connect-0.0.1/inverter/cli/cli_app.py
--rw-rw-r--   0 jens      (1000) users      (100)      276 2023-04-23 15:55:16.000000 inverter-connect-0.0.1/inverter/config.py
--rw-rw-r--   0 jens      (1000) users      (100)     7752 2023-04-23 15:55:16.000000 inverter-connect-0.0.1/inverter/connection.py
--rw-rw-r--   0 jens      (1000) users      (100)      136 2023-04-20 19:23:05.000000 inverter-connect-0.0.1/inverter/constants.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-23 16:18:41.094645 inverter-connect-0.0.1/inverter/definitions/
--rw-rw-r--   0 jens      (1000) users      (100)     2885 2023-04-20 19:38:44.000000 inverter-connect-0.0.1/inverter/definitions/deye_2mppt.yaml
--rw-rw-r--   0 jens      (1000) users      (100)     2455 2023-04-23 15:55:16.000000 inverter-connect-0.0.1/inverter/definitions.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-23 16:18:41.094645 inverter-connect-0.0.1/inverter/tests/
--rw-rw-r--   0 jens      (1000) users      (100)      239 2023-04-20 19:23:05.000000 inverter-connect-0.0.1/inverter/tests/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     1618 2023-04-23 16:13:50.000000 inverter-connect-0.0.1/inverter/tests/test_api.py
--rw-rw-r--   0 jens      (1000) users      (100)      795 2023-04-20 19:23:21.000000 inverter-connect-0.0.1/inverter/tests/test_connect.py
--rw-rw-r--   0 jens      (1000) users      (100)     1369 2023-04-20 19:23:05.000000 inverter-connect-0.0.1/inverter/tests/test_definitions.py
--rw-rw-r--   0 jens      (1000) users      (100)      211 2023-04-17 13:29:40.000000 inverter-connect-0.0.1/inverter/tests/test_doctests.py
--rw-rw-r--   0 jens      (1000) users      (100)     2314 2023-04-20 19:36:47.000000 inverter-connect-0.0.1/inverter/tests/test_project_setup.py
--rw-rw-r--   0 jens      (1000) users      (100)     2135 2023-04-21 06:50:23.000000 inverter-connect-0.0.1/inverter/tests/test_readme.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-23 16:18:41.094645 inverter-connect-0.0.1/inverter/utilities/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-17 17:34:28.000000 inverter-connect-0.0.1/inverter/utilities/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     2187 2023-04-21 07:02:38.000000 inverter-connect-0.0.1/inverter/utilities/modbus_converter.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-23 16:18:41.094645 inverter-connect-0.0.1/inverter_connect.egg-info/
--rw-rw-r--   0 jens      (1000) users      (100)     8827 2023-04-23 16:18:41.000000 inverter-connect-0.0.1/inverter_connect.egg-info/PKG-INFO
--rw-rw-r--   0 jens      (1000) users      (100)      990 2023-04-23 16:18:41.000000 inverter-connect-0.0.1/inverter_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 jens      (1000) users      (100)        1 2023-04-23 16:18:41.000000 inverter-connect-0.0.1/inverter_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 jens      (1000) users      (100)       52 2023-04-23 16:18:41.000000 inverter-connect-0.0.1/inverter_connect.egg-info/entry_points.txt
--rw-rw-r--   0 jens      (1000) users      (100)      249 2023-04-23 16:18:41.000000 inverter-connect-0.0.1/inverter_connect.egg-info/requires.txt
--rw-rw-r--   0 jens      (1000) users      (100)        9 2023-04-23 16:18:41.000000 inverter-connect-0.0.1/inverter_connect.egg-info/top_level.txt
--rw-rw-r--   0 jens      (1000) users      (100)     4675 2023-04-21 06:59:46.000000 inverter-connect-0.0.1/pyproject.toml
--rw-rw-r--   0 jens      (1000) users      (100)    50878 2023-04-19 06:56:45.000000 inverter-connect-0.0.1/requirements.dev.txt
--rw-rw-r--   0 jens      (1000) users      (100)     2307 2023-04-19 06:56:45.000000 inverter-connect-0.0.1/requirements.txt
--rw-rw-r--   0 jens      (1000) users      (100)       38 2023-04-23 16:18:41.094645 inverter-connect-0.0.1/setup.cfg
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-21 07:05:50.837658 inverter-connect-0.0.1rc0/
+-rw-rw-r--   0 jens      (1000) users      (100)      301 2023-04-13 15:18:51.000000 inverter-connect-0.0.1rc0/.editorconfig
+-rw-rw-r--   0 jens      (1000) users      (100)      153 2023-04-13 15:18:51.000000 inverter-connect-0.0.1rc0/.flake8
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-21 07:05:50.837658 inverter-connect-0.0.1rc0/.github/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-21 07:05:50.837658 inverter-connect-0.0.1rc0/.github/workflows/
+-rw-rw-r--   0 jens      (1000) users      (100)     1460 2023-04-19 06:56:31.000000 inverter-connect-0.0.1rc0/.github/workflows/tests.yml
+-rw-rw-r--   0 jens      (1000) users      (100)      118 2023-04-13 15:18:51.000000 inverter-connect-0.0.1rc0/.gitignore
+-rw-rw-r--   0 jens      (1000) users      (100)     8702 2023-04-21 07:05:50.837658 inverter-connect-0.0.1rc0/PKG-INFO
+-rw-rw-r--   0 jens      (1000) users      (100)     8285 2023-04-21 06:59:46.000000 inverter-connect-0.0.1rc0/README.md
+-rwxrwxr-x   0 jens      (1000) users      (100)     3047 2023-04-20 19:23:05.000000 inverter-connect-0.0.1rc0/cli.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-21 07:05:50.837658 inverter-connect-0.0.1rc0/inverter/
+-rw-rw-r--   0 jens      (1000) users      (100)      301 2023-04-17 13:29:40.000000 inverter-connect-0.0.1rc0/inverter/.editorconfig
+-rw-rw-r--   0 jens      (1000) users      (100)      153 2023-04-17 13:29:40.000000 inverter-connect-0.0.1rc0/inverter/.flake8
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-21 07:05:50.837658 inverter-connect-0.0.1rc0/inverter/.github/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-21 07:05:50.837658 inverter-connect-0.0.1rc0/inverter/.github/workflows/
+-rw-rw-r--   0 jens      (1000) users      (100)     1460 2023-04-17 13:29:40.000000 inverter-connect-0.0.1rc0/inverter/.github/workflows/tests.yml
+-rw-rw-r--   0 jens      (1000) users      (100)      118 2023-04-17 13:29:40.000000 inverter-connect-0.0.1rc0/inverter/.gitignore
+-rw-rw-r--   0 jens      (1000) users      (100)      151 2023-04-21 07:01:32.000000 inverter-connect-0.0.1rc0/inverter/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      186 2023-04-20 19:23:05.000000 inverter-connect-0.0.1rc0/inverter/__main__.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-21 07:05:50.837658 inverter-connect-0.0.1rc0/inverter/cli/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-17 13:29:40.000000 inverter-connect-0.0.1rc0/inverter/cli/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)    11354 2023-04-21 06:40:55.000000 inverter-connect-0.0.1rc0/inverter/cli/cli_app.py
+-rw-rw-r--   0 jens      (1000) users      (100)     7905 2023-04-21 07:03:09.000000 inverter-connect-0.0.1rc0/inverter/connection.py
+-rw-rw-r--   0 jens      (1000) users      (100)      136 2023-04-20 19:23:05.000000 inverter-connect-0.0.1rc0/inverter/constants.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-21 07:05:50.837658 inverter-connect-0.0.1rc0/inverter/definitions/
+-rw-rw-r--   0 jens      (1000) users      (100)     2885 2023-04-20 19:38:44.000000 inverter-connect-0.0.1rc0/inverter/definitions/deye_2mppt.yaml
+-rw-rw-r--   0 jens      (1000) users      (100)     2367 2023-04-21 07:03:09.000000 inverter-connect-0.0.1rc0/inverter/definitions.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-21 07:05:50.837658 inverter-connect-0.0.1rc0/inverter/tests/
+-rw-rw-r--   0 jens      (1000) users      (100)      239 2023-04-20 19:23:05.000000 inverter-connect-0.0.1rc0/inverter/tests/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      795 2023-04-20 19:23:21.000000 inverter-connect-0.0.1rc0/inverter/tests/test_connect.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1369 2023-04-20 19:23:05.000000 inverter-connect-0.0.1rc0/inverter/tests/test_definitions.py
+-rw-rw-r--   0 jens      (1000) users      (100)      211 2023-04-17 13:29:40.000000 inverter-connect-0.0.1rc0/inverter/tests/test_doctests.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2314 2023-04-20 19:36:47.000000 inverter-connect-0.0.1rc0/inverter/tests/test_project_setup.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2135 2023-04-21 06:50:23.000000 inverter-connect-0.0.1rc0/inverter/tests/test_readme.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-21 07:05:50.837658 inverter-connect-0.0.1rc0/inverter/utilities/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-17 17:34:28.000000 inverter-connect-0.0.1rc0/inverter/utilities/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2187 2023-04-21 07:02:38.000000 inverter-connect-0.0.1rc0/inverter/utilities/modbus_converter.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-21 07:05:50.837658 inverter-connect-0.0.1rc0/inverter_connect.egg-info/
+-rw-rw-r--   0 jens      (1000) users      (100)     8702 2023-04-21 07:05:50.000000 inverter-connect-0.0.1rc0/inverter_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 jens      (1000) users      (100)      928 2023-04-21 07:05:50.000000 inverter-connect-0.0.1rc0/inverter_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 jens      (1000) users      (100)        1 2023-04-21 07:05:50.000000 inverter-connect-0.0.1rc0/inverter_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 jens      (1000) users      (100)       52 2023-04-21 07:05:50.000000 inverter-connect-0.0.1rc0/inverter_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 jens      (1000) users      (100)      249 2023-04-21 07:05:50.000000 inverter-connect-0.0.1rc0/inverter_connect.egg-info/requires.txt
+-rw-rw-r--   0 jens      (1000) users      (100)        9 2023-04-21 07:05:50.000000 inverter-connect-0.0.1rc0/inverter_connect.egg-info/top_level.txt
+-rw-rw-r--   0 jens      (1000) users      (100)     4675 2023-04-21 06:59:46.000000 inverter-connect-0.0.1rc0/pyproject.toml
+-rw-rw-r--   0 jens      (1000) users      (100)    50878 2023-04-19 06:56:45.000000 inverter-connect-0.0.1rc0/requirements.dev.txt
+-rw-rw-r--   0 jens      (1000) users      (100)     2307 2023-04-19 06:56:45.000000 inverter-connect-0.0.1rc0/requirements.txt
+-rw-rw-r--   0 jens      (1000) users      (100)       38 2023-04-21 07:05:50.837658 inverter-connect-0.0.1rc0/setup.cfg
```

### Comparing `inverter-connect-0.0.1/.github/workflows/tests.yml` & `inverter-connect-0.0.1rc0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.0.1/PKG-INFO` & `inverter-connect-0.0.1rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: inverter-connect
-Version: 0.0.1
+Version: 0.0.1rc0
 Summary: Get information from Deye Microinverter
 Author-email: Jens Diemer <inverter-connect@jensdiemer.de>
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://github.com/jedie/inverter-connect
 Project-URL: Source, https://github.com/jedie/inverter-connect
 Requires-Python: <4,>=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # inverter
 
-[![tests](https://github.com/jedie/inverter-connect/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/jedie/inverter-connect/actions/workflows/tests.yml)
+[![tests](https://github.com/jedie/inverter-connect/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/jedie/inverter-connect-connect/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/github/jedie/inverter-connect/branch/main/graph/badge.svg)](https://app.codecov.io/github/jedie/inverter-connect)
 [![inverter-connect @ PyPi](https://img.shields.io/pypi/v/inverter-connect?label=inverter-connect%20%40%20PyPi)](https://pypi.org/project/inverter-connect/)
-[![Python Versions](https://img.shields.io/pypi/pyversions/inverter-connect)](https://github.com/jedie/inverter-connect/blob/main/pyproject.toml)
-[![License GPL-3.0-or-later](https://img.shields.io/pypi/l/inverter-connect)](https://github.com/jedie/inverter-connect/blob/main/LICENSE)
+[![Python Versions](https://img.shields.io/pypi/pyversions/inverter-connect)](https://github.com/jedie/inverter-connect-connect/blob/main/pyproject.toml)
+[![License GPL-3.0-or-later](https://img.shields.io/pypi/l/inverter-connect)](https://github.com/jedie/inverter-connect-connect/blob/main/LICENSE)
 
 Get information from Deye Microinverter
 
 The whole thing is just a learning exercise for now. We will see.
 
 ## screenshots
 
@@ -137,10 +137,7 @@
 * https://github.com/StephanJoubert/home_assistant_solarman
 
 The included definitions yaml files are from:
 
 https://github.com/StephanJoubert/home_assistant_solarman/tree/main/custom_components/solarman/inverter_definitions
 
 
-## various links
-
-* Discussion: https://www.photovoltaikforum.com/thread/201065-inverter-connect-daten-vom-deye-wechselrichter-per-python-abrufen/ (de)
```

### Comparing `inverter-connect-0.0.1/README.md` & `inverter-connect-0.0.1rc0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # inverter
 
-[![tests](https://github.com/jedie/inverter-connect/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/jedie/inverter-connect/actions/workflows/tests.yml)
+[![tests](https://github.com/jedie/inverter-connect/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/jedie/inverter-connect-connect/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/github/jedie/inverter-connect/branch/main/graph/badge.svg)](https://app.codecov.io/github/jedie/inverter-connect)
 [![inverter-connect @ PyPi](https://img.shields.io/pypi/v/inverter-connect?label=inverter-connect%20%40%20PyPi)](https://pypi.org/project/inverter-connect/)
-[![Python Versions](https://img.shields.io/pypi/pyversions/inverter-connect)](https://github.com/jedie/inverter-connect/blob/main/pyproject.toml)
-[![License GPL-3.0-or-later](https://img.shields.io/pypi/l/inverter-connect)](https://github.com/jedie/inverter-connect/blob/main/LICENSE)
+[![Python Versions](https://img.shields.io/pypi/pyversions/inverter-connect)](https://github.com/jedie/inverter-connect-connect/blob/main/pyproject.toml)
+[![License GPL-3.0-or-later](https://img.shields.io/pypi/l/inverter-connect)](https://github.com/jedie/inverter-connect-connect/blob/main/LICENSE)
 
 Get information from Deye Microinverter
 
 The whole thing is just a learning exercise for now. We will see.
 
 ## screenshots
 
@@ -125,10 +125,7 @@
 * https://github.com/StephanJoubert/home_assistant_solarman
 
 The included definitions yaml files are from:
 
 https://github.com/StephanJoubert/home_assistant_solarman/tree/main/custom_components/solarman/inverter_definitions
 
 
-## various links
-
-* Discussion: https://www.photovoltaikforum.com/thread/201065-inverter-connect-daten-vom-deye-wechselrichter-per-python-abrufen/ (de)
```

### Comparing `inverter-connect-0.0.1/cli.py` & `inverter-connect-0.0.1rc0/cli.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.0.1/inverter/.github/workflows/tests.yml` & `inverter-connect-0.0.1rc0/inverter/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.0.1/inverter/cli/cli_app.py` & `inverter-connect-0.0.1rc0/inverter/cli/cli_app.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,18 +9,16 @@
 from manageprojects.utilities.subprocess_utils import verbose_check_call
 from manageprojects.utilities.version_info import print_version
 from rich import print  # noqa
 from rich_click import RichGroup
 
 import inverter
 from inverter import constants
-from inverter.api import Inverter, ValueType
-from inverter.config import Config
-from inverter.connection import ERROR_STR_NO_DATA, InverterSock
-from inverter.definitions import Parameter
+from inverter.connection import ERROR_STR_NO_DATA, Config, InverterSock, ModbusReadResult
+from inverter.definitions import get_parameter
 
 
 logger = logging.getLogger(__name__)
 
 
 PACKAGE_ROOT = Path(inverter.__file__).parent.parent
 assert_is_file(PACKAGE_ROOT / 'pyproject.toml')
@@ -165,15 +163,14 @@
     Build and upload this project to PyPi
     """
     _run_unittest_cli(verbose=False, exit_after_run=False)  # Don't publish a broken state
 
     publish_package(
         module=inverter,
         package_path=PACKAGE_ROOT,
-        distribution_name='inverter-connect',
     )
 
 
 cli.add_command(publish)
 
 
 @click.command()
@@ -319,35 +316,42 @@
     """
     if debug:
         level = logging.DEBUG
     else:
         level = logging.INFO
 
     logging.basicConfig(level=level)
-    config = Config(yaml_filename='deye_2mppt.yaml', host=ip, port=port, debug=debug)
-    with Inverter(config=config) as inverter:
-        for value in inverter:
-            print(f'\t* [yellow]{value.name:<31}[/yellow]:', end=' ')
-            if value.value == ERROR_STR_NO_DATA:
+    parameters = get_parameter(yaml_filename='deye_2mppt.yaml', debug=debug)
+    config = Config(host=ip, port=port, debug=debug)
+    if debug:
+        print(config)
+
+    with InverterSock(config) as inv_sock:
+        print(inv_sock.inverter_info)
+        print()
+
+        for parameter in parameters:
+            if debug:
+                print('_' * 100)
+                print(parameter.name)
+
+            result: ModbusReadResult = inv_sock.read(parameter=parameter)
+
+            print(f'\t* [yellow]{result.parameter.name:<31}[/yellow]:', end=' ')
+            if result.parsed_value == ERROR_STR_NO_DATA:
                 color = 'red'
-                msg = ERROR_STR_NO_DATA
+                value = ERROR_STR_NO_DATA
             else:
                 color = 'green'
-                msg = f'{value.value} {value.unit}'
-            print(f'[{color}]{msg:<11}[/{color}]', end=' ')
-
-            if value.type == ValueType.READ_OUT:
-                parameter: Parameter = value.result.parameter
-                print(
-                    f'(Register: [cyan]{parameter.start_register:04X}[/cyan], length:'
-                    f' [blue]{parameter.length}[/blue])'
-                )
-            elif value.type == ValueType.COMPUTED:
-                print('(Computed)')
+                value = f'{result.parsed_value} {result.parameter.unit}'
+            print(f'[{color}]{value:<11}[/{color}]', end=' ')
 
+            print(
+                f'(Register: [cyan]{parameter.start_register:04X}[/cyan], length:' f' [blue]{parameter.length}[/blue])'
+            )
             if debug:
                 print()
 
 
 cli.add_command(print_values)
 
 
@@ -385,19 +389,17 @@
             'WANN',
             'WEBVER',
             'WEBU',
             'WAP',
             'WSSSID',
             'WSKEY',
             'YZAPP',
-            'UPURL',
-            'WAPMXSTA',  # max. number of wifi clients
         )
 
-    config = Config(yaml_filename=None, host=ip, port=port, debug=debug)
+    config = Config(host=ip, port=port, debug=debug)
     if debug:
         print(config)
 
     with InverterSock(config) as inv_sock:
         print(inv_sock.inverter_info)
         print()
```

### Comparing `inverter-connect-0.0.1/inverter/connection.py` & `inverter-connect-0.0.1rc0/inverter/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
 import dataclasses
 import logging
 import socket
 import time
 
-from inverter.config import Config
 from inverter.definitions import Parameter
 
 
 logger = logging.getLogger(__name__)
 
 ERROR_STR_NO_DATA = 'no data'
 
@@ -19,14 +18,24 @@
     Modbus register value is: 'no data' == ERROR_STR_NO_DATA
     """
 
     pass
 
 
 @dataclasses.dataclass
+class Config:
+    host: str
+    port: int = 48899
+    pause: float = 0.1
+    timeout: int = 5
+    debug: bool = False
+    init_cmd: bytes = b'WIFIKIT-214028-READ'
+
+
+@dataclasses.dataclass
 class InverterInfo:
     ip: str
     mac: str
     serial: int
 
 
 @dataclasses.dataclass
```

### Comparing `inverter-connect-0.0.1/inverter/definitions/deye_2mppt.yaml` & `inverter-connect-0.0.1rc0/inverter/definitions/deye_2mppt.yaml`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.0.1/inverter/definitions.py` & `inverter-connect-0.0.1rc0/inverter/definitions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from __future__ import annotations
 
 import dataclasses
-from collections.abc import Iterable
-from typing import Callable
 
 import yaml
 from bx_py_utils.dict_utils import pluck
 from bx_py_utils.path import assert_is_file
 
 from inverter.constants import BASE_PATH
 from inverter.utilities.modbus_converter import debug_converter, parse_number, parse_string, parse_swapped_number
@@ -16,15 +14,15 @@
 class Parameter:
     start_register: int
     length: int
     group: str
     name: str
     unit: str
     scale: float | int
-    parser: Callable
+    parser: callable
     offset: int | None = None
     lookup: dict | None = None
 
 
 rule2converter = {
     1: parse_number,
     3: parse_swapped_number,
@@ -44,15 +42,15 @@
     """
     >>> convert_lookup([{'key': 2, 'value': 'Normal'},{'key': 3, 'value': 'Warning'}])
     {2: 'Normal', 3: 'Warning'}
     """
     return {entry['key']: entry['value'] for entry in raw_lookup}
 
 
-def get_parameter(yaml_filename, debug=False) -> Iterable[Parameter]:
+def get_parameter(yaml_filename, debug=False):
     data = get_definition(yaml_filename)
     parameters = []
     for group_data in data:
         group_name = group_data['group']
         for item in group_data['items']:
             # example = {
             #     'name': 'PV1 Voltage',
```

### Comparing `inverter-connect-0.0.1/inverter/tests/test_connect.py` & `inverter-connect-0.0.1rc0/inverter/tests/test_connect.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.0.1/inverter/tests/test_definitions.py` & `inverter-connect-0.0.1rc0/inverter/tests/test_definitions.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.0.1/inverter/tests/test_project_setup.py` & `inverter-connect-0.0.1rc0/inverter/tests/test_project_setup.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.0.1/inverter/tests/test_readme.py` & `inverter-connect-0.0.1rc0/inverter/tests/test_readme.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.0.1/inverter/utilities/modbus_converter.py` & `inverter-connect-0.0.1rc0/inverter/utilities/modbus_converter.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.0.1/inverter_connect.egg-info/PKG-INFO` & `inverter-connect-0.0.1rc0/inverter_connect.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: inverter-connect
-Version: 0.0.1
+Version: 0.0.1rc0
 Summary: Get information from Deye Microinverter
 Author-email: Jens Diemer <inverter-connect@jensdiemer.de>
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://github.com/jedie/inverter-connect
 Project-URL: Source, https://github.com/jedie/inverter-connect
 Requires-Python: <4,>=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # inverter
 
-[![tests](https://github.com/jedie/inverter-connect/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/jedie/inverter-connect/actions/workflows/tests.yml)
+[![tests](https://github.com/jedie/inverter-connect/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/jedie/inverter-connect-connect/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/github/jedie/inverter-connect/branch/main/graph/badge.svg)](https://app.codecov.io/github/jedie/inverter-connect)
 [![inverter-connect @ PyPi](https://img.shields.io/pypi/v/inverter-connect?label=inverter-connect%20%40%20PyPi)](https://pypi.org/project/inverter-connect/)
-[![Python Versions](https://img.shields.io/pypi/pyversions/inverter-connect)](https://github.com/jedie/inverter-connect/blob/main/pyproject.toml)
-[![License GPL-3.0-or-later](https://img.shields.io/pypi/l/inverter-connect)](https://github.com/jedie/inverter-connect/blob/main/LICENSE)
+[![Python Versions](https://img.shields.io/pypi/pyversions/inverter-connect)](https://github.com/jedie/inverter-connect-connect/blob/main/pyproject.toml)
+[![License GPL-3.0-or-later](https://img.shields.io/pypi/l/inverter-connect)](https://github.com/jedie/inverter-connect-connect/blob/main/LICENSE)
 
 Get information from Deye Microinverter
 
 The whole thing is just a learning exercise for now. We will see.
 
 ## screenshots
 
@@ -137,10 +137,7 @@
 * https://github.com/StephanJoubert/home_assistant_solarman
 
 The included definitions yaml files are from:
 
 https://github.com/StephanJoubert/home_assistant_solarman/tree/main/custom_components/solarman/inverter_definitions
 
 
-## various links
-
-* Discussion: https://www.photovoltaikforum.com/thread/201065-inverter-connect-daten-vom-deye-wechselrichter-per-python-abrufen/ (de)
```

### Comparing `inverter-connect-0.0.1/inverter_connect.egg-info/SOURCES.txt` & `inverter-connect-0.0.1rc0/inverter_connect.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -8,25 +8,22 @@
 requirements.txt
 .github/workflows/tests.yml
 inverter/.editorconfig
 inverter/.flake8
 inverter/.gitignore
 inverter/__init__.py
 inverter/__main__.py
-inverter/api.py
-inverter/config.py
 inverter/connection.py
 inverter/constants.py
 inverter/definitions.py
 inverter/.github/workflows/tests.yml
 inverter/cli/__init__.py
 inverter/cli/cli_app.py
 inverter/definitions/deye_2mppt.yaml
 inverter/tests/__init__.py
-inverter/tests/test_api.py
 inverter/tests/test_connect.py
 inverter/tests/test_definitions.py
 inverter/tests/test_doctests.py
 inverter/tests/test_project_setup.py
 inverter/tests/test_readme.py
 inverter/utilities/__init__.py
 inverter/utilities/modbus_converter.py
```

### Comparing `inverter-connect-0.0.1/pyproject.toml` & `inverter-connect-0.0.1rc0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.0.1/requirements.dev.txt` & `inverter-connect-0.0.1rc0/requirements.dev.txt`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.0.1/requirements.txt` & `inverter-connect-0.0.1rc0/requirements.txt`

 * *Files identical despite different names*

