# Comparing `tmp/nonebot-plugin-brainfuck-1.0.3.tar.gz` & `tmp/nonebot-plugin-brainfuck-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nonebot-plugin-brainfuck-1.0.3.tar", last modified: Sun Apr 23 04:21:25 2023, max compression
+gzip compressed data, was "dist/nonebot-plugin-brainfuck-1.0.4.tar", last modified: Sun Apr 23 04:37:02 2023, max compression
```

## Comparing `nonebot-plugin-brainfuck-1.0.3.tar` & `nonebot-plugin-brainfuck-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 Campanula   (501) staff       (20)        0 2023-04-23 04:21:25.105203 nonebot-plugin-brainfuck-1.0.3/
--rw-r--r--   0 Campanula   (501) staff       (20)     1066 2023-04-23 03:08:01.000000 nonebot-plugin-brainfuck-1.0.3/LICENSE
--rw-r--r--   0 Campanula   (501) staff       (20)      563 2023-04-23 04:21:25.104892 nonebot-plugin-brainfuck-1.0.3/PKG-INFO
--rw-r--r--   0 Campanula   (501) staff       (20)     2523 2023-04-23 03:22:10.000000 nonebot-plugin-brainfuck-1.0.3/README.md
-drwxr-xr-x   0 Campanula   (501) staff       (20)        0 2023-04-23 04:21:25.102186 nonebot-plugin-brainfuck-1.0.3/nonebot_plugin_brainfuck/
--rw-r--r--   0 Campanula   (501) staff       (20)      982 2023-04-23 04:21:24.000000 nonebot-plugin-brainfuck-1.0.3/nonebot_plugin_brainfuck/__init__.py
--rw-r--r--   0 Campanula   (501) staff       (20)     4556 2023-04-23 02:41:05.000000 nonebot-plugin-brainfuck-1.0.3/nonebot_plugin_brainfuck/brainfuck_interpreter.py
--rw-r--r--   0 Campanula   (501) staff       (20)      240 2023-04-23 02:06:44.000000 nonebot-plugin-brainfuck-1.0.3/nonebot_plugin_brainfuck/error_info.py
--rw-r--r--   0 Campanula   (501) staff       (20)      404 2023-04-23 03:09:37.000000 nonebot-plugin-brainfuck-1.0.3/nonebot_plugin_brainfuck/test.py
-drwxr-xr-x   0 Campanula   (501) staff       (20)        0 2023-04-23 04:21:25.104451 nonebot-plugin-brainfuck-1.0.3/nonebot_plugin_brainfuck.egg-info/
--rw-r--r--   0 Campanula   (501) staff       (20)      563 2023-04-23 04:21:25.000000 nonebot-plugin-brainfuck-1.0.3/nonebot_plugin_brainfuck.egg-info/PKG-INFO
--rw-r--r--   0 Campanula   (501) staff       (20)      467 2023-04-23 04:21:25.000000 nonebot-plugin-brainfuck-1.0.3/nonebot_plugin_brainfuck.egg-info/SOURCES.txt
--rw-r--r--   0 Campanula   (501) staff       (20)        1 2023-04-23 04:21:25.000000 nonebot-plugin-brainfuck-1.0.3/nonebot_plugin_brainfuck.egg-info/dependency_links.txt
--rw-r--r--   0 Campanula   (501) staff       (20)       74 2023-04-23 04:21:25.000000 nonebot-plugin-brainfuck-1.0.3/nonebot_plugin_brainfuck.egg-info/requires.txt
--rw-r--r--   0 Campanula   (501) staff       (20)       25 2023-04-23 04:21:25.000000 nonebot-plugin-brainfuck-1.0.3/nonebot_plugin_brainfuck.egg-info/top_level.txt
--rw-r--r--   0 Campanula   (501) staff       (20)        1 2023-04-23 04:21:25.000000 nonebot-plugin-brainfuck-1.0.3/nonebot_plugin_brainfuck.egg-info/zip-safe
--rw-r--r--   0 Campanula   (501) staff       (20)       38 2023-04-23 04:21:25.105296 nonebot-plugin-brainfuck-1.0.3/setup.cfg
--rw-r--r--   0 Campanula   (501) staff       (20)     1295 2023-04-23 04:21:24.000000 nonebot-plugin-brainfuck-1.0.3/setup.py
+drwxr-xr-x   0 Campanula   (501) staff       (20)        0 2023-04-23 04:37:02.270666 nonebot-plugin-brainfuck-1.0.4/
+-rw-r--r--   0 Campanula   (501) staff       (20)     1066 2023-04-23 03:08:01.000000 nonebot-plugin-brainfuck-1.0.4/LICENSE
+-rw-r--r--   0 Campanula   (501) staff       (20)      563 2023-04-23 04:37:02.270408 nonebot-plugin-brainfuck-1.0.4/PKG-INFO
+-rw-r--r--   0 Campanula   (501) staff       (20)     2523 2023-04-23 04:27:31.000000 nonebot-plugin-brainfuck-1.0.4/README.md
+drwxr-xr-x   0 Campanula   (501) staff       (20)        0 2023-04-23 04:37:02.268062 nonebot-plugin-brainfuck-1.0.4/nonebot_plugin_brainfuck/
+-rw-r--r--   0 Campanula   (501) staff       (20)      982 2023-04-23 04:21:24.000000 nonebot-plugin-brainfuck-1.0.4/nonebot_plugin_brainfuck/__init__.py
+-rw-r--r--   0 Campanula   (501) staff       (20)     4563 2023-04-23 04:24:45.000000 nonebot-plugin-brainfuck-1.0.4/nonebot_plugin_brainfuck/brainfuck_interpreter.py
+-rw-r--r--   0 Campanula   (501) staff       (20)      240 2023-04-23 02:06:44.000000 nonebot-plugin-brainfuck-1.0.4/nonebot_plugin_brainfuck/error_info.py
+drwxr-xr-x   0 Campanula   (501) staff       (20)        0 2023-04-23 04:37:02.270036 nonebot-plugin-brainfuck-1.0.4/nonebot_plugin_brainfuck.egg-info/
+-rw-r--r--   0 Campanula   (501) staff       (20)      563 2023-04-23 04:37:02.000000 nonebot-plugin-brainfuck-1.0.4/nonebot_plugin_brainfuck.egg-info/PKG-INFO
+-rw-r--r--   0 Campanula   (501) staff       (20)      434 2023-04-23 04:37:02.000000 nonebot-plugin-brainfuck-1.0.4/nonebot_plugin_brainfuck.egg-info/SOURCES.txt
+-rw-r--r--   0 Campanula   (501) staff       (20)        1 2023-04-23 04:37:02.000000 nonebot-plugin-brainfuck-1.0.4/nonebot_plugin_brainfuck.egg-info/dependency_links.txt
+-rw-r--r--   0 Campanula   (501) staff       (20)       74 2023-04-23 04:37:02.000000 nonebot-plugin-brainfuck-1.0.4/nonebot_plugin_brainfuck.egg-info/requires.txt
+-rw-r--r--   0 Campanula   (501) staff       (20)       25 2023-04-23 04:37:02.000000 nonebot-plugin-brainfuck-1.0.4/nonebot_plugin_brainfuck.egg-info/top_level.txt
+-rw-r--r--   0 Campanula   (501) staff       (20)        1 2023-04-23 04:37:02.000000 nonebot-plugin-brainfuck-1.0.4/nonebot_plugin_brainfuck.egg-info/zip-safe
+-rw-r--r--   0 Campanula   (501) staff       (20)       38 2023-04-23 04:37:02.270751 nonebot-plugin-brainfuck-1.0.4/setup.cfg
+-rw-r--r--   0 Campanula   (501) staff       (20)     1295 2023-04-23 04:34:47.000000 nonebot-plugin-brainfuck-1.0.4/setup.py
```

### Comparing `nonebot-plugin-brainfuck-1.0.3/LICENSE` & `nonebot-plugin-brainfuck-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-brainfuck-1.0.3/PKG-INFO` & `nonebot-plugin-brainfuck-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-brainfuck
-Version: 1.0.3
+Version: 1.0.4
 Summary: a brainfuck interpreter for nonebot
 Home-page: https://github.com/campanulamediuml/nonebot-plugin-brainfuck
 Author: campanula
 Author-email: campanulamediuml@gmail.com
 License: MIT
 Keywords: brainfuck
 Platform: any
```

### Comparing `nonebot-plugin-brainfuck-1.0.3/README.md` & `nonebot-plugin-brainfuck-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-brainfuck-1.0.3/nonebot_plugin_brainfuck/__init__.py` & `nonebot-plugin-brainfuck-1.0.4/nonebot_plugin_brainfuck/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-brainfuck-1.0.3/nonebot_plugin_brainfuck/brainfuck_interpreter.py` & `nonebot-plugin-brainfuck-1.0.4/nonebot_plugin_brainfuck/brainfuck_interpreter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # !/usr/bin/env python
 # -*-coding:utf-8 -*-
 # Author     ：Campanula 梦芸 何
 import struct
 from typing import List, Dict, Optional
 
-import error_info
+from . import error_info
 
 MOVE_L = '<'
 MOVE_R = '>'
 V_ADD = '+'
 V_SUB = '-'
 STD_O = '.'
 STD_I = ','
```

### Comparing `nonebot-plugin-brainfuck-1.0.3/nonebot_plugin_brainfuck.egg-info/PKG-INFO` & `nonebot-plugin-brainfuck-1.0.4/nonebot_plugin_brainfuck.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-brainfuck
-Version: 1.0.3
+Version: 1.0.4
 Summary: a brainfuck interpreter for nonebot
 Home-page: https://github.com/campanulamediuml/nonebot-plugin-brainfuck
 Author: campanula
 Author-email: campanulamediuml@gmail.com
 License: MIT
 Keywords: brainfuck
 Platform: any
```

### Comparing `nonebot-plugin-brainfuck-1.0.3/setup.py` & `nonebot-plugin-brainfuck-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 def read_file(fname):
     return codecs.open(os.path.join(os.path.dirname(__file__), fname), encoding='utf-8').read()
 
 
 setup(
         # 以下为必需参数
         name='nonebot-plugin-brainfuck',  # 模块名
-        version='1.0.3',  # 当前版本
+        version='1.0.4',  # 当前版本
         description='a brainfuck interpreter for nonebot',
         # 简短描述
         license='MIT',
         long_description='a brainfuck interpreter for nonebot',
         author='campanula',
         author_email='campanulamediuml@gmail.com',
         platforms='any',
```

