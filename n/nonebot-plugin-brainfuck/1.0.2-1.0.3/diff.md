# Comparing `tmp/nonebot-plugin-brainfuck-1.0.2.tar.gz` & `tmp/nonebot-plugin-brainfuck-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nonebot-plugin-brainfuck-1.0.2.tar", last modified: Sun Apr 23 04:15:36 2023, max compression
+gzip compressed data, was "dist/nonebot-plugin-brainfuck-1.0.3.tar", last modified: Sun Apr 23 04:21:25 2023, max compression
```

## Comparing `nonebot-plugin-brainfuck-1.0.2.tar` & `nonebot-plugin-brainfuck-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 Campanula   (501) staff       (20)        0 2023-04-23 04:15:36.163995 nonebot-plugin-brainfuck-1.0.2/
--rw-r--r--   0 Campanula   (501) staff       (20)     1066 2023-04-23 03:08:01.000000 nonebot-plugin-brainfuck-1.0.2/LICENSE
--rw-r--r--   0 Campanula   (501) staff       (20)      563 2023-04-23 04:15:36.163735 nonebot-plugin-brainfuck-1.0.2/PKG-INFO
--rw-r--r--   0 Campanula   (501) staff       (20)     2523 2023-04-23 03:22:10.000000 nonebot-plugin-brainfuck-1.0.2/README.md
-drwxr-xr-x   0 Campanula   (501) staff       (20)        0 2023-04-23 04:15:36.161425 nonebot-plugin-brainfuck-1.0.2/nonebot_plugin_brainfuck/
--rw-r--r--   0 Campanula   (501) staff       (20)      981 2023-04-23 03:50:36.000000 nonebot-plugin-brainfuck-1.0.2/nonebot_plugin_brainfuck/__init__.py
--rw-r--r--   0 Campanula   (501) staff       (20)     4556 2023-04-23 02:41:05.000000 nonebot-plugin-brainfuck-1.0.2/nonebot_plugin_brainfuck/brainfuck_interpreter.py
--rw-r--r--   0 Campanula   (501) staff       (20)      240 2023-04-23 02:06:44.000000 nonebot-plugin-brainfuck-1.0.2/nonebot_plugin_brainfuck/error_info.py
--rw-r--r--   0 Campanula   (501) staff       (20)      404 2023-04-23 03:09:37.000000 nonebot-plugin-brainfuck-1.0.2/nonebot_plugin_brainfuck/test.py
-drwxr-xr-x   0 Campanula   (501) staff       (20)        0 2023-04-23 04:15:36.163383 nonebot-plugin-brainfuck-1.0.2/nonebot_plugin_brainfuck.egg-info/
--rw-r--r--   0 Campanula   (501) staff       (20)      563 2023-04-23 04:15:36.000000 nonebot-plugin-brainfuck-1.0.2/nonebot_plugin_brainfuck.egg-info/PKG-INFO
--rw-r--r--   0 Campanula   (501) staff       (20)      467 2023-04-23 04:15:36.000000 nonebot-plugin-brainfuck-1.0.2/nonebot_plugin_brainfuck.egg-info/SOURCES.txt
--rw-r--r--   0 Campanula   (501) staff       (20)        1 2023-04-23 04:15:36.000000 nonebot-plugin-brainfuck-1.0.2/nonebot_plugin_brainfuck.egg-info/dependency_links.txt
--rw-r--r--   0 Campanula   (501) staff       (20)       74 2023-04-23 04:15:36.000000 nonebot-plugin-brainfuck-1.0.2/nonebot_plugin_brainfuck.egg-info/requires.txt
--rw-r--r--   0 Campanula   (501) staff       (20)       25 2023-04-23 04:15:36.000000 nonebot-plugin-brainfuck-1.0.2/nonebot_plugin_brainfuck.egg-info/top_level.txt
--rw-r--r--   0 Campanula   (501) staff       (20)        1 2023-04-23 04:15:36.000000 nonebot-plugin-brainfuck-1.0.2/nonebot_plugin_brainfuck.egg-info/zip-safe
--rw-r--r--   0 Campanula   (501) staff       (20)       38 2023-04-23 04:15:36.164083 nonebot-plugin-brainfuck-1.0.2/setup.cfg
--rw-r--r--   0 Campanula   (501) staff       (20)     1295 2023-04-23 04:15:35.000000 nonebot-plugin-brainfuck-1.0.2/setup.py
+drwxr-xr-x   0 Campanula   (501) staff       (20)        0 2023-04-23 04:21:25.105203 nonebot-plugin-brainfuck-1.0.3/
+-rw-r--r--   0 Campanula   (501) staff       (20)     1066 2023-04-23 03:08:01.000000 nonebot-plugin-brainfuck-1.0.3/LICENSE
+-rw-r--r--   0 Campanula   (501) staff       (20)      563 2023-04-23 04:21:25.104892 nonebot-plugin-brainfuck-1.0.3/PKG-INFO
+-rw-r--r--   0 Campanula   (501) staff       (20)     2523 2023-04-23 03:22:10.000000 nonebot-plugin-brainfuck-1.0.3/README.md
+drwxr-xr-x   0 Campanula   (501) staff       (20)        0 2023-04-23 04:21:25.102186 nonebot-plugin-brainfuck-1.0.3/nonebot_plugin_brainfuck/
+-rw-r--r--   0 Campanula   (501) staff       (20)      982 2023-04-23 04:21:24.000000 nonebot-plugin-brainfuck-1.0.3/nonebot_plugin_brainfuck/__init__.py
+-rw-r--r--   0 Campanula   (501) staff       (20)     4556 2023-04-23 02:41:05.000000 nonebot-plugin-brainfuck-1.0.3/nonebot_plugin_brainfuck/brainfuck_interpreter.py
+-rw-r--r--   0 Campanula   (501) staff       (20)      240 2023-04-23 02:06:44.000000 nonebot-plugin-brainfuck-1.0.3/nonebot_plugin_brainfuck/error_info.py
+-rw-r--r--   0 Campanula   (501) staff       (20)      404 2023-04-23 03:09:37.000000 nonebot-plugin-brainfuck-1.0.3/nonebot_plugin_brainfuck/test.py
+drwxr-xr-x   0 Campanula   (501) staff       (20)        0 2023-04-23 04:21:25.104451 nonebot-plugin-brainfuck-1.0.3/nonebot_plugin_brainfuck.egg-info/
+-rw-r--r--   0 Campanula   (501) staff       (20)      563 2023-04-23 04:21:25.000000 nonebot-plugin-brainfuck-1.0.3/nonebot_plugin_brainfuck.egg-info/PKG-INFO
+-rw-r--r--   0 Campanula   (501) staff       (20)      467 2023-04-23 04:21:25.000000 nonebot-plugin-brainfuck-1.0.3/nonebot_plugin_brainfuck.egg-info/SOURCES.txt
+-rw-r--r--   0 Campanula   (501) staff       (20)        1 2023-04-23 04:21:25.000000 nonebot-plugin-brainfuck-1.0.3/nonebot_plugin_brainfuck.egg-info/dependency_links.txt
+-rw-r--r--   0 Campanula   (501) staff       (20)       74 2023-04-23 04:21:25.000000 nonebot-plugin-brainfuck-1.0.3/nonebot_plugin_brainfuck.egg-info/requires.txt
+-rw-r--r--   0 Campanula   (501) staff       (20)       25 2023-04-23 04:21:25.000000 nonebot-plugin-brainfuck-1.0.3/nonebot_plugin_brainfuck.egg-info/top_level.txt
+-rw-r--r--   0 Campanula   (501) staff       (20)        1 2023-04-23 04:21:25.000000 nonebot-plugin-brainfuck-1.0.3/nonebot_plugin_brainfuck.egg-info/zip-safe
+-rw-r--r--   0 Campanula   (501) staff       (20)       38 2023-04-23 04:21:25.105296 nonebot-plugin-brainfuck-1.0.3/setup.cfg
+-rw-r--r--   0 Campanula   (501) staff       (20)     1295 2023-04-23 04:21:24.000000 nonebot-plugin-brainfuck-1.0.3/setup.py
```

### Comparing `nonebot-plugin-brainfuck-1.0.2/LICENSE` & `nonebot-plugin-brainfuck-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-brainfuck-1.0.2/PKG-INFO` & `nonebot-plugin-brainfuck-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-brainfuck
-Version: 1.0.2
+Version: 1.0.3
 Summary: a brainfuck interpreter for nonebot
 Home-page: https://github.com/campanulamediuml/nonebot-plugin-brainfuck
 Author: campanula
 Author-email: campanulamediuml@gmail.com
 License: MIT
 Keywords: brainfuck
 Platform: any
```

### Comparing `nonebot-plugin-brainfuck-1.0.2/README.md` & `nonebot-plugin-brainfuck-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-brainfuck-1.0.2/nonebot_plugin_brainfuck/__init__.py` & `nonebot-plugin-brainfuck-1.0.3/nonebot_plugin_brainfuck/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from nonebot import  on_startswith
 from nonebot.adapters.onebot.v11 import GroupMessageEvent
 from nonebot.plugin import PluginMetadata
-from brainfuck_interpreter import call
+from .brainfuck_interpreter import call
 from nonebot.matcher import Matcher
 
 __plugin_meta__ = PluginMetadata(
     name="nonebot_plugin_brainfuck",
     description="brainfuck解释器，brainfuck是一种仅含有八个字符的图灵完备语言",
     usage="在qq中进行交互对brainfuck代码进行解释",
     extra={},
```

### Comparing `nonebot-plugin-brainfuck-1.0.2/nonebot_plugin_brainfuck/brainfuck_interpreter.py` & `nonebot-plugin-brainfuck-1.0.3/nonebot_plugin_brainfuck/brainfuck_interpreter.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-brainfuck-1.0.2/nonebot_plugin_brainfuck.egg-info/PKG-INFO` & `nonebot-plugin-brainfuck-1.0.3/nonebot_plugin_brainfuck.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-brainfuck
-Version: 1.0.2
+Version: 1.0.3
 Summary: a brainfuck interpreter for nonebot
 Home-page: https://github.com/campanulamediuml/nonebot-plugin-brainfuck
 Author: campanula
 Author-email: campanulamediuml@gmail.com
 License: MIT
 Keywords: brainfuck
 Platform: any
```

### Comparing `nonebot-plugin-brainfuck-1.0.2/setup.py` & `nonebot-plugin-brainfuck-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 def read_file(fname):
     return codecs.open(os.path.join(os.path.dirname(__file__), fname), encoding='utf-8').read()
 
 
 setup(
         # 以下为必需参数
         name='nonebot-plugin-brainfuck',  # 模块名
-        version='1.0.2',  # 当前版本
+        version='1.0.3',  # 当前版本
         description='a brainfuck interpreter for nonebot',
         # 简短描述
         license='MIT',
         long_description='a brainfuck interpreter for nonebot',
         author='campanula',
         author_email='campanulamediuml@gmail.com',
         platforms='any',
```

