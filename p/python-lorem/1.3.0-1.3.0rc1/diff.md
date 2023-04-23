# Comparing `tmp/python-lorem-1.3.0.tar.gz` & `tmp/python-lorem-1.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-lorem-1.3.0.tar", last modified: Sun Apr 23 06:40:03 2023, max compression
+gzip compressed data, was "python-lorem-1.3.0rc1.tar", last modified: Sun Apr 23 06:32:02 2023, max compression
```

## Comparing `python-lorem-1.3.0.tar` & `python-lorem-1.3.0rc1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:40:03.852657 python-lorem-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-23 06:39:52.000000 python-lorem-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-23 06:39:52.000000 python-lorem-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-04-23 06:40:03.852657 python-lorem-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-23 06:39:52.000000 python-lorem-1.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    17538 2023-04-23 06:39:52.000000 python-lorem-1.3.0/lorem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-04-23 06:39:52.000000 python-lorem-1.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:40:03.852657 python-lorem-1.3.0/python_lorem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-04-23 06:40:03.000000 python-lorem-1.3.0/python_lorem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-23 06:40:03.000000 python-lorem-1.3.0/python_lorem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 06:40:03.000000 python-lorem-1.3.0/python_lorem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-23 06:40:03.000000 python-lorem-1.3.0/python_lorem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-23 06:40:03.000000 python-lorem-1.3.0/python_lorem.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 06:40:03.000000 python-lorem-1.3.0/python_lorem.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-23 06:40:03.852657 python-lorem-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-04-23 06:39:52.000000 python-lorem-1.3.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-04-23 06:39:52.000000 python-lorem-1.3.0/test_lorem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:32:02.891667 python-lorem-1.3.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-23 06:31:49.000000 python-lorem-1.3.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-23 06:31:49.000000 python-lorem-1.3.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-04-23 06:32:02.891667 python-lorem-1.3.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-23 06:31:49.000000 python-lorem-1.3.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    17541 2023-04-23 06:31:49.000000 python-lorem-1.3.0rc1/lorem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-04-23 06:31:49.000000 python-lorem-1.3.0rc1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:32:02.891667 python-lorem-1.3.0rc1/python_lorem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-04-23 06:32:02.000000 python-lorem-1.3.0rc1/python_lorem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-23 06:32:02.000000 python-lorem-1.3.0rc1/python_lorem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 06:32:02.000000 python-lorem-1.3.0rc1/python_lorem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-23 06:32:02.000000 python-lorem-1.3.0rc1/python_lorem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-23 06:32:02.000000 python-lorem-1.3.0rc1/python_lorem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 06:32:02.000000 python-lorem-1.3.0rc1/python_lorem.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-23 06:32:02.891667 python-lorem-1.3.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-04-23 06:31:49.000000 python-lorem-1.3.0rc1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-04-23 06:31:49.000000 python-lorem-1.3.0rc1/test_lorem.py
```

### Comparing `python-lorem-1.3.0/LICENSE` & `python-lorem-1.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-lorem-1.3.0/PKG-INFO` & `python-lorem-1.3.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-lorem
-Version: 1.3.0
+Version: 1.3.0rc1
 Summary: Lorem ipsum generator.
 Author-email: Jarry Shaw <jarryshaw@icloud.com>
 Maintainer: Jarry Shaw
 License: BSD 3-Clause License
 Project-URL: homepage, https://jarryshaw.github.io/lorem/
 Project-URL: documentation, https://jarryshaw.github.io/lorem/
 Project-URL: repository, https://github.com/JarryShaw/lorem
```

### Comparing `python-lorem-1.3.0/README.md` & `python-lorem-1.3.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `python-lorem-1.3.0/lorem.py` & `python-lorem-1.3.0rc1/lorem.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 __all__ = [
     'LoremGenerator',
     'word', 'sentence', 'paragraph',
     'get_word', 'get_sentence', 'get_paragraph',
 ]
 
 # version string
-__version__ = '1.3.0'
+__version__ = '1.3.0rc1'
 
 #: The original lorem ipsum text pool.
 _TEXT = ('ad', 'adipiscing', 'aliqua', 'aliquip', 'amet', 'anim', 'aute', 'cillum', 'commodo',
          'consectetur', 'consequat', 'culpa', 'cupidatat', 'deserunt', 'do', 'dolor', 'dolore',
          'duis', 'ea', 'eiusmod', 'elit', 'enim', 'esse', 'est', 'et', 'eu', 'ex', 'excepteur',
          'exercitation', 'fugiat', 'id', 'in', 'incididunt', 'ipsum', 'irure', 'labore', 'laboris',
          'laborum', 'lorem', 'magna', 'minim', 'mollit', 'nisi', 'non', 'nostrud', 'nulla',
```

### Comparing `python-lorem-1.3.0/pyproject.toml` & `python-lorem-1.3.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python-lorem-1.3.0/python_lorem.egg-info/PKG-INFO` & `python-lorem-1.3.0rc1/python_lorem.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-lorem
-Version: 1.3.0
+Version: 1.3.0rc1
 Summary: Lorem ipsum generator.
 Author-email: Jarry Shaw <jarryshaw@icloud.com>
 Maintainer: Jarry Shaw
 License: BSD 3-Clause License
 Project-URL: homepage, https://jarryshaw.github.io/lorem/
 Project-URL: documentation, https://jarryshaw.github.io/lorem/
 Project-URL: repository, https://github.com/JarryShaw/lorem
```

### Comparing `python-lorem-1.3.0/setup.py` & `python-lorem-1.3.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `python-lorem-1.3.0/test_lorem.py` & `python-lorem-1.3.0rc1/test_lorem.py`

 * *Files identical despite different names*

