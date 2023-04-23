# Comparing `tmp/argcomplete-3.0.6.tar.gz` & `tmp/argcomplete-3.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argcomplete-3.0.6.tar", last modified: Sat Apr 22 14:30:58 2023, max compression
+gzip compressed data, was "argcomplete-3.0.7.tar", last modified: Sun Apr 23 21:36:05 2023, max compression
```

## Comparing `argcomplete-3.0.6.tar` & `argcomplete-3.0.7.tar`

### file list

```diff
@@ -1,53 +1,51 @@
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 14:30:58.418194 argcomplete-3.0.6/
--rw-r--r--   0 kislyuk    (501) staff       (20)       35 2016-06-14 14:20:26.000000 argcomplete-3.0.6/Authors.rst
--rw-r--r--   0 kislyuk    (501) staff       (20)    12286 2023-04-22 14:30:41.000000 argcomplete-3.0.6/Changes.rst
--rw-r--r--   0 kislyuk    (501) staff       (20)    10174 2016-06-14 14:20:26.000000 argcomplete-3.0.6/LICENSE.rst
--rw-r--r--   0 kislyuk    (501) staff       (20)       79 2022-08-21 15:59:43.000000 argcomplete-3.0.6/MANIFEST.in
--rw-r--r--   0 kislyuk    (501) staff       (20)      387 2023-03-21 02:49:58.000000 argcomplete-3.0.6/NOTICE
--rw-r--r--   0 kislyuk    (501) staff       (20)    16463 2023-04-22 14:30:58.418271 argcomplete-3.0.6/PKG-INFO
--rw-r--r--   0 kislyuk    (501) staff       (20)    14856 2023-04-22 14:28:37.000000 argcomplete-3.0.6/README.rst
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 14:30:58.413428 argcomplete-3.0.6/argcomplete/
--rw-r--r--   0 kislyuk    (501) staff       (20)      693 2023-03-21 02:49:58.000000 argcomplete-3.0.6/argcomplete/__init__.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     2140 2023-03-05 19:47:13.000000 argcomplete-3.0.6/argcomplete/_check_console_script.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     2600 2023-03-18 19:32:22.000000 argcomplete-3.0.6/argcomplete/_check_module.py
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 14:30:58.414283 argcomplete-3.0.6/argcomplete/bash_completion.d/
--rw-r--r--   0 kislyuk    (501) staff       (20)     5422 2023-03-26 00:26:25.000000 argcomplete-3.0.6/argcomplete/bash_completion.d/python-argcomplete
--rw-r--r--   0 kislyuk    (501) staff       (20)     3980 2023-03-26 15:30:13.000000 argcomplete-3.0.6/argcomplete/completers.py
--rw-r--r--   0 kislyuk    (501) staff       (20)      112 2023-03-19 18:35:55.000000 argcomplete-3.0.6/argcomplete/exceptions.py
--rw-r--r--   0 kislyuk    (501) staff       (20)    26975 2023-03-26 15:30:13.000000 argcomplete-3.0.6/argcomplete/finders.py
--rw-r--r--   0 kislyuk    (501) staff       (20)      866 2023-03-19 18:46:34.000000 argcomplete-3.0.6/argcomplete/io.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     2131 2023-03-21 02:49:58.000000 argcomplete-3.0.6/argcomplete/lexers.py
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 14:30:58.414998 argcomplete-3.0.6/argcomplete/packages/
--rw-r--r--   0 kislyuk    (501) staff       (20)        0 2023-03-19 10:11:13.000000 argcomplete-3.0.6/argcomplete/packages/__init__.py
--rw-r--r--   0 kislyuk    (501) staff       (20)    15846 2023-03-19 18:59:55.000000 argcomplete-3.0.6/argcomplete/packages/_argparse.py
--rw-r--r--   0 kislyuk    (501) staff       (20)    12766 2023-03-18 19:32:22.000000 argcomplete-3.0.6/argcomplete/packages/_shlex.py
--rw-r--r--   0 kislyuk    (501) staff       (20)        0 2023-03-18 19:32:22.000000 argcomplete-3.0.6/argcomplete/py.typed
--rw-r--r--   0 kislyuk    (501) staff       (20)     7012 2023-04-22 14:28:37.000000 argcomplete-3.0.6/argcomplete/shell_integration.py
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 14:30:58.414176 argcomplete-3.0.6/argcomplete.egg-info/
--rw-r--r--   0 kislyuk    (501) staff       (20)    16463 2023-04-22 14:30:58.000000 argcomplete-3.0.6/argcomplete.egg-info/PKG-INFO
--rw-r--r--   0 kislyuk    (501) staff       (20)     1091 2023-04-22 14:30:58.000000 argcomplete-3.0.6/argcomplete.egg-info/SOURCES.txt
--rw-r--r--   0 kislyuk    (501) staff       (20)        1 2023-04-22 14:30:58.000000 argcomplete-3.0.6/argcomplete.egg-info/dependency_links.txt
--rw-r--r--   0 kislyuk    (501) staff       (20)        1 2023-04-22 14:30:49.000000 argcomplete-3.0.6/argcomplete.egg-info/not-zip-safe
--rw-r--r--   0 kislyuk    (501) staff       (20)      153 2023-04-22 14:30:58.000000 argcomplete-3.0.6/argcomplete.egg-info/requires.txt
--rw-r--r--   0 kislyuk    (501) staff       (20)       12 2023-04-22 14:30:58.000000 argcomplete-3.0.6/argcomplete.egg-info/top_level.txt
--rw-r--r--   0 kislyuk    (501) staff       (20)      371 2023-03-26 00:37:29.000000 argcomplete-3.0.6/pyproject.toml
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 14:30:58.415741 argcomplete-3.0.6/scripts/
--rwxr-xr-x   0 kislyuk    (501) staff       (20)     3374 2023-03-26 00:26:25.000000 argcomplete-3.0.6/scripts/activate-global-python-argcomplete
--rwxr-xr-x   0 kislyuk    (501) staff       (20)     2609 2023-03-19 01:09:49.000000 argcomplete-3.0.6/scripts/python-argcomplete-check-easy-install-script
--rwxr-xr-x   0 kislyuk    (501) staff       (20)     1997 2023-04-22 14:28:37.000000 argcomplete-3.0.6/scripts/register-python-argcomplete
--rw-r--r--   0 kislyuk    (501) staff       (20)      143 2023-04-22 14:30:58.418541 argcomplete-3.0.6/setup.cfg
--rwxr-xr-x   0 kislyuk    (501) staff       (20)     2403 2023-04-22 14:29:05.000000 argcomplete-3.0.6/setup.py
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 14:30:58.417409 argcomplete-3.0.6/test/
--rw-r--r--   0 kislyuk    (501) staff       (20)        0 2016-06-14 14:20:26.000000 argcomplete-3.0.6/test/__init__.py
--rw-r--r--   0 kislyuk    (501) staff       (20)      139 2016-06-16 15:02:13.000000 argcomplete-3.0.6/test/__init__.pyc
--rw-r--r--   0 kislyuk    (501) staff       (20)       31 2023-03-05 19:47:13.000000 argcomplete-3.0.6/test/inputrc
--rwxr-xr-x   0 kislyuk    (501) staff       (20)     1765 2022-09-14 03:21:59.000000 argcomplete-3.0.6/test/prog
--rwxr-xr-x   0 kislyuk    (501) staff       (20)    59328 2023-04-22 14:28:37.000000 argcomplete-3.0.6/test/test.py
--rw-r--r--   0 kislyuk    (501) staff       (20)    31570 2016-10-16 02:47:39.000000 argcomplete-3.0.6/test/test.pyc
--rw-r--r--   0 kislyuk    (501) staff       (20)     3183 2023-03-18 19:32:22.000000 argcomplete-3.0.6/test/test_contrib_shells.py
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 14:30:58.417895 argcomplete-3.0.6/test/test_package/
--rw-r--r--   0 kislyuk    (501) staff       (20)        0 2023-03-05 19:47:13.000000 argcomplete-3.0.6/test/test_package/__init__.py
--rw-r--r--   0 kislyuk    (501) staff       (20)      299 2022-09-14 03:21:59.000000 argcomplete-3.0.6/test/test_package/setup.py
--rw-r--r--   0 kislyuk    (501) staff       (20)       94 2022-09-14 03:21:59.000000 argcomplete-3.0.6/test/test_package/test_module.py
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 14:30:58.418068 argcomplete-3.0.6/test/test_package/test_package/
--rw-r--r--   0 kislyuk    (501) staff       (20)      289 2022-09-14 03:21:59.000000 argcomplete-3.0.6/test/test_package/test_package/__init__.py
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-04-23 21:36:05.869456 argcomplete-3.0.7/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       35 2021-06-26 14:08:42.000000 argcomplete-3.0.7/Authors.rst
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    12424 2023-04-23 21:35:30.000000 argcomplete-3.0.7/Changes.rst
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    10174 2021-06-26 14:08:42.000000 argcomplete-3.0.7/LICENSE.rst
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       79 2021-06-26 14:08:42.000000 argcomplete-3.0.7/MANIFEST.in
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      387 2023-03-21 01:42:51.000000 argcomplete-3.0.7/NOTICE
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    16463 2023-04-23 21:36:05.869686 argcomplete-3.0.7/PKG-INFO
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    14856 2023-04-23 21:34:49.000000 argcomplete-3.0.7/README.rst
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-04-23 21:36:05.850972 argcomplete-3.0.7/argcomplete/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      693 2023-03-21 01:39:54.000000 argcomplete-3.0.7/argcomplete/__init__.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     2140 2023-03-04 23:22:21.000000 argcomplete-3.0.7/argcomplete/_check_console_script.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     2600 2023-03-17 18:26:27.000000 argcomplete-3.0.7/argcomplete/_check_module.py
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-04-23 21:36:05.855422 argcomplete-3.0.7/argcomplete/bash_completion.d/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     5422 2023-03-29 02:42:12.000000 argcomplete-3.0.7/argcomplete/bash_completion.d/python-argcomplete
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     3980 2023-03-29 02:42:12.000000 argcomplete-3.0.7/argcomplete/completers.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      112 2023-03-19 19:40:27.000000 argcomplete-3.0.7/argcomplete/exceptions.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    26975 2023-03-29 02:42:12.000000 argcomplete-3.0.7/argcomplete/finders.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      866 2023-03-19 19:40:27.000000 argcomplete-3.0.7/argcomplete/io.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     2131 2023-03-21 01:39:33.000000 argcomplete-3.0.7/argcomplete/lexers.py
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-04-23 21:36:05.857633 argcomplete-3.0.7/argcomplete/packages/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        0 2023-03-19 19:40:27.000000 argcomplete-3.0.7/argcomplete/packages/__init__.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    15846 2023-03-19 19:40:27.000000 argcomplete-3.0.7/argcomplete/packages/_argparse.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    12766 2023-03-19 19:40:27.000000 argcomplete-3.0.7/argcomplete/packages/_shlex.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        0 2023-03-17 19:10:26.000000 argcomplete-3.0.7/argcomplete/py.typed
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     7012 2023-04-23 21:34:49.000000 argcomplete-3.0.7/argcomplete/shell_integration.py
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-04-23 21:36:05.854884 argcomplete-3.0.7/argcomplete.egg-info/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    16463 2023-04-23 21:36:05.000000 argcomplete-3.0.7/argcomplete.egg-info/PKG-INFO
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     1059 2023-04-23 21:36:05.000000 argcomplete-3.0.7/argcomplete.egg-info/SOURCES.txt
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        1 2023-04-23 21:36:05.000000 argcomplete-3.0.7/argcomplete.egg-info/dependency_links.txt
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        1 2023-04-23 21:35:43.000000 argcomplete-3.0.7/argcomplete.egg-info/not-zip-safe
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      153 2023-04-23 21:36:05.000000 argcomplete-3.0.7/argcomplete.egg-info/requires.txt
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       12 2023-04-23 21:36:05.000000 argcomplete-3.0.7/argcomplete.egg-info/top_level.txt
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      371 2023-04-04 02:41:07.000000 argcomplete-3.0.7/pyproject.toml
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-04-23 21:36:05.860015 argcomplete-3.0.7/scripts/
+-rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)     3374 2023-03-22 00:11:35.000000 argcomplete-3.0.7/scripts/activate-global-python-argcomplete
+-rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)     2609 2023-03-19 19:40:27.000000 argcomplete-3.0.7/scripts/python-argcomplete-check-easy-install-script
+-rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)     1997 2023-04-23 21:34:49.000000 argcomplete-3.0.7/scripts/register-python-argcomplete
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      143 2023-04-23 21:36:05.870434 argcomplete-3.0.7/setup.cfg
+-rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)     2403 2023-04-23 21:34:56.000000 argcomplete-3.0.7/setup.py
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-04-23 21:36:05.865171 argcomplete-3.0.7/test/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        0 2021-06-26 14:08:42.000000 argcomplete-3.0.7/test/__init__.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       31 2023-03-04 23:22:21.000000 argcomplete-3.0.7/test/inputrc
+-rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)     1765 2023-03-04 23:22:21.000000 argcomplete-3.0.7/test/prog
+-rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)    59349 2023-04-23 21:34:49.000000 argcomplete-3.0.7/test/test.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     3183 2023-03-17 17:41:01.000000 argcomplete-3.0.7/test/test_contrib_shells.py
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-04-23 21:36:05.867517 argcomplete-3.0.7/test/test_package/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        0 2023-03-04 23:22:21.000000 argcomplete-3.0.7/test/test_package/__init__.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      299 2023-03-04 23:22:21.000000 argcomplete-3.0.7/test/test_package/setup.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       94 2023-03-04 23:22:21.000000 argcomplete-3.0.7/test/test_package/test_module.py
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-04-23 21:36:05.868513 argcomplete-3.0.7/test/test_package/test_package/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      289 2023-03-04 23:22:21.000000 argcomplete-3.0.7/test/test_package/test_package/__init__.py
```

### Comparing `argcomplete-3.0.6/Changes.rst` & `argcomplete-3.0.7/Changes.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+Changes for v3.0.7 (2023-04-23)
+===============================
+
+-  Test suite: Use general regex to cut zsh reset ANSI sequences (#425)
+
 Changes for v3.0.6 (2023-04-22)
 ===============================
 
 -  Allow importlib-metadata 6.x; skip test failures on Python 3.7 (#420,
    #424)
 
 -  Note completers can return iterables of strings, not just lists
```

### Comparing `argcomplete-3.0.6/LICENSE.rst` & `argcomplete-3.0.7/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `argcomplete-3.0.6/PKG-INFO` & `argcomplete-3.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argcomplete
-Version: 3.0.6
+Version: 3.0.7
 Summary: Bash tab completion for argparse
 Home-page: https://github.com/kislyuk/argcomplete
 Author: Andrey Kislyuk
 Author-email: kislyuk@gmail.com
 License: Apache Software License
 Project-URL: Documentation, https://kislyuk.github.io/argcomplete
 Project-URL: Source Code, https://github.com/kislyuk/argcomplete
```

### Comparing `argcomplete-3.0.6/README.rst` & `argcomplete-3.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `argcomplete-3.0.6/argcomplete/__init__.py` & `argcomplete-3.0.7/argcomplete/__init__.py`

 * *Files identical despite different names*

### Comparing `argcomplete-3.0.6/argcomplete/_check_console_script.py` & `argcomplete-3.0.7/argcomplete/_check_console_script.py`

 * *Files identical despite different names*

### Comparing `argcomplete-3.0.6/argcomplete/_check_module.py` & `argcomplete-3.0.7/argcomplete/_check_module.py`

 * *Files identical despite different names*

### Comparing `argcomplete-3.0.6/argcomplete/bash_completion.d/python-argcomplete` & `argcomplete-3.0.7/argcomplete/bash_completion.d/python-argcomplete`

 * *Files identical despite different names*

### Comparing `argcomplete-3.0.6/argcomplete/completers.py` & `argcomplete-3.0.7/argcomplete/completers.py`

 * *Files identical despite different names*

### Comparing `argcomplete-3.0.6/argcomplete/finders.py` & `argcomplete-3.0.7/argcomplete/finders.py`

 * *Files identical despite different names*

### Comparing `argcomplete-3.0.6/argcomplete/io.py` & `argcomplete-3.0.7/argcomplete/io.py`

 * *Files identical despite different names*

### Comparing `argcomplete-3.0.6/argcomplete/lexers.py` & `argcomplete-3.0.7/argcomplete/lexers.py`

 * *Files identical despite different names*

### Comparing `argcomplete-3.0.6/argcomplete/packages/_argparse.py` & `argcomplete-3.0.7/argcomplete/packages/_argparse.py`

 * *Files identical despite different names*

### Comparing `argcomplete-3.0.6/argcomplete/packages/_shlex.py` & `argcomplete-3.0.7/argcomplete/packages/_shlex.py`

 * *Files identical despite different names*

### Comparing `argcomplete-3.0.6/argcomplete/shell_integration.py` & `argcomplete-3.0.7/argcomplete/shell_integration.py`

 * *Files identical despite different names*

### Comparing `argcomplete-3.0.6/argcomplete.egg-info/PKG-INFO` & `argcomplete-3.0.7/argcomplete.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argcomplete
-Version: 3.0.6
+Version: 3.0.7
 Summary: Bash tab completion for argparse
 Home-page: https://github.com/kislyuk/argcomplete
 Author: Andrey Kislyuk
 Author-email: kislyuk@gmail.com
 License: Apache Software License
 Project-URL: Documentation, https://kislyuk.github.io/argcomplete
 Project-URL: Source Code, https://github.com/kislyuk/argcomplete
```

### Comparing `argcomplete-3.0.6/argcomplete.egg-info/SOURCES.txt` & `argcomplete-3.0.7/argcomplete.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -27,17 +27,15 @@
 argcomplete/packages/__init__.py
 argcomplete/packages/_argparse.py
 argcomplete/packages/_shlex.py
 scripts/activate-global-python-argcomplete
 scripts/python-argcomplete-check-easy-install-script
 scripts/register-python-argcomplete
 test/__init__.py
-test/__init__.pyc
 test/inputrc
 test/prog
 test/test.py
-test/test.pyc
 test/test_contrib_shells.py
 test/test_package/__init__.py
 test/test_package/setup.py
 test/test_package/test_module.py
 test/test_package/test_package/__init__.py
```

### Comparing `argcomplete-3.0.6/scripts/activate-global-python-argcomplete` & `argcomplete-3.0.7/scripts/activate-global-python-argcomplete`

 * *Files identical despite different names*

### Comparing `argcomplete-3.0.6/scripts/python-argcomplete-check-easy-install-script` & `argcomplete-3.0.7/scripts/python-argcomplete-check-easy-install-script`

 * *Files identical despite different names*

### Comparing `argcomplete-3.0.6/scripts/register-python-argcomplete` & `argcomplete-3.0.7/scripts/register-python-argcomplete`

 * *Files identical despite different names*

### Comparing `argcomplete-3.0.6/setup.py` & `argcomplete-3.0.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 install_requires = []
 tests_require = ["coverage", "pexpect", "wheel", "ruff", "mypy"]
 importlib_backport_requires = ["importlib-metadata >= 0.23, < 7"]
 
 setup(
     name="argcomplete",
-    version="3.0.6",
+    version="3.0.7",
     url="https://github.com/kislyuk/argcomplete",
     project_urls={
         "Documentation": "https://kislyuk.github.io/argcomplete",
         "Source Code": "https://github.com/kislyuk/argcomplete",
         "Issue Tracker": "https://github.com/kislyuk/argcomplete/issues",
         "Change Log": "https://github.com/kislyuk/argcomplete/blob/master/Changes.rst",
     },
```

### Comparing `argcomplete-3.0.6/test/prog` & `argcomplete-3.0.7/test/prog`

 * *Files identical despite different names*

### Comparing `argcomplete-3.0.6/test/test.py` & `argcomplete-3.0.7/test/test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 #!/usr/bin/env python
 import argparse
 import contextlib
 import os
 import os.path
+import re
 import shutil
 import subprocess
 import sys
 import unittest
 from io import StringIO
 from tempfile import NamedTemporaryFile, TemporaryFile, mkdtemp
 
 import pexpect
-from pexpect.replwrap import REPLWrapper, PEXPECT_PROMPT, PEXPECT_CONTINUATION_PROMPT
+from pexpect.replwrap import PEXPECT_CONTINUATION_PROMPT, PEXPECT_PROMPT, REPLWrapper
 
 TEST_DIR = os.path.abspath(os.path.dirname(__file__))
 BASE_DIR = os.path.dirname(TEST_DIR)
 sys.path.insert(0, BASE_DIR)
 
 from argparse import SUPPRESS, ArgumentParser  # noqa: E402
 
@@ -44,16 +45,16 @@
         if "\n" in command:
             raise Exception("newlines not supported in REPL input")
         res = super().run_command(command, **kwargs)
         if self.child.command.split("/")[-1] == "zsh":
             if "\n" not in res:
                 raise Exception("Expected to see a newline in command response")
             echo_cmd, actual_res = res.split("\n", 1)
-            actual_res = actual_res.replace("\x1b[0m\x1b[23m\x1b[24m\x1b[J", "")
-            return actual_res
+            res_without_ansi_seqs = re.sub(r"\x1b\[0m.+\x1b\[J", "", actual_res)
+            return res_without_ansi_seqs
         else:
             return res
 
 
 def _repl_sh(command, args, non_printable_insert):
     os.environ["PS1"] = "$"
     child = pexpect.spawn(command, args, echo=False, encoding="utf-8")
```

### Comparing `argcomplete-3.0.6/test/test_contrib_shells.py` & `argcomplete-3.0.7/test/test_contrib_shells.py`

 * *Files identical despite different names*

