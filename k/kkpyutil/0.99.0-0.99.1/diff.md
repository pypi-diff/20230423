# Comparing `tmp/kkpyutil-0.99.0.tar.gz` & `tmp/kkpyutil-0.99.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kkpyutil-0.99.0.tar", max compression
+gzip compressed data, was "kkpyutil-0.99.1.tar", max compression
```

## Comparing `kkpyutil-0.99.0.tar` & `kkpyutil-0.99.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1065 2021-08-27 02:37:07.874512 kkpyutil-0.99.0/LICENSE
--rw-r--r--   0        0        0      280 2021-08-27 02:37:07.874614 kkpyutil-0.99.0/README.md
--rwxr-xr-x   0        0        0    83476 2022-09-24 09:20:59.790905 kkpyutil-0.99.0/kkpyutil.py
--rw-r--r--   0        0        0      759 2022-09-24 09:21:10.813251 kkpyutil-0.99.0/pyproject.toml
--rw-r--r--   0        0        0      864 2022-09-24 09:21:36.835949 kkpyutil-0.99.0/setup.py
--rw-r--r--   0        0        0     1111 2022-09-24 09:21:36.836158 kkpyutil-0.99.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2021-08-27 02:37:07.874512 kkpyutil-0.99.1/LICENSE
+-rw-r--r--   0        0        0      280 2021-08-27 02:37:07.874614 kkpyutil-0.99.1/README.md
+-rwxr-xr-x   0        0        0    83564 2022-09-24 10:11:19.837264 kkpyutil-0.99.1/kkpyutil.py
+-rw-r--r--   0        0        0      759 2022-09-24 10:06:23.709825 kkpyutil-0.99.1/pyproject.toml
+-rw-r--r--   0        0        0      864 2022-09-24 10:17:30.000764 kkpyutil-0.99.1/setup.py
+-rw-r--r--   0        0        0     1111 2022-09-24 10:17:30.001010 kkpyutil-0.99.1/PKG-INFO
```

### Comparing `kkpyutil-0.99.0/LICENSE` & `kkpyutil-0.99.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kkpyutil-0.99.0/kkpyutil.py` & `kkpyutil-0.99.1/kkpyutil.py`

 * *Files 0% similar despite different names*

```diff
@@ -1388,16 +1388,16 @@
     if style == 'ONEWORD':
         return snake_text.replace('_', '').upper()
     if style == 'SNAKE':
         return snake_text.upper()
     if style == 'kebab':
         return snake_text.replace('_', '-')
     split_strs = snake_text.split('_')
-    if style == 'title':
-        return ' '.join([part.title() for part in split_strs])
+    if style == 'title':  # en_US => en US, this_is_title => This is Title
+        return ' '.join([part[0].title()+part[1:] if part else part.title() for part in split_strs])
     if style == 'phrase':
         return ' '.join(split_strs)
     # if input is one-piece, then we preserve its middle chars' cases
     # to avoid str.capitalize() turning a string into Titlecase
     if len(split_strs) == 1:
         out_text = split_strs
         leading = out_text[0][0].lower() if style == 'camel' else out_text[0][0].upper()
```

### Comparing `kkpyutil-0.99.0/pyproject.toml` & `kkpyutil-0.99.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kkpyutil"
-version = "0.99.0"
+version = "0.99.1"
 description = "Personal utility functions and classes frequently used by myself for daily Python work."
 authors = ["Beinan Li <li.beinan@gmail.com>"]
 maintainers = ["Beinan Li <li.beinan@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = ""
 repository = "https://github.com/kakyoism/kkpyutil/"
```

### Comparing `kkpyutil-0.99.0/setup.py` & `kkpyutil-0.99.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 modules = \
 ['kkpyutil']
 setup_kwargs = {
     'name': 'kkpyutil',
-    'version': '0.99.0',
+    'version': '0.99.1',
     'description': 'Personal utility functions and classes frequently used by myself for daily Python work.',
     'long_description': '# kkpyutil\nPersonal utility functions and classes frequently used by myself for daily Python work.\n\nIt does not necessarily benefit everybody, but I hope it \nmay occasionally shed light on some issues you may have in your own work.\n\n## INSTALL\n\n```shell\npip3 install kkpyutil\n```\n',
     'author': 'Beinan Li',
     'author_email': 'li.beinan@gmail.com',
     'maintainer': 'Beinan Li',
     'maintainer_email': 'li.beinan@gmail.com',
     'url': 'https://github.com/kakyoism/kkpyutil/',
```

### Comparing `kkpyutil-0.99.0/PKG-INFO` & `kkpyutil-0.99.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kkpyutil
-Version: 0.99.0
+Version: 0.99.1
 Summary: Personal utility functions and classes frequently used by myself for daily Python work.
 Home-page: https://github.com/kakyoism/kkpyutil/
 License: MIT
 Keywords: utility,logging,i/o,oop
 Author: Beinan Li
 Author-email: li.beinan@gmail.com
 Maintainer: Beinan Li
```

