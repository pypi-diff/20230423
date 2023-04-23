# Comparing `tmp/har2jicase-0.1.7.tar.gz` & `tmp/har2jicase-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "har2jicase-0.1.7.tar", last modified: Fri Apr 21 09:51:18 2023, max compression
+gzip compressed data, was "har2jicase-0.1.8.tar", last modified: Sun Apr 23 10:37:34 2023, max compression
```

## Comparing `har2jicase-0.1.7.tar` & `har2jicase-0.1.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 09:51:18.011957 har2jicase-0.1.7/
--rw-rw-rw-   0        0        0      518 2023-04-21 09:51:18.011957 har2jicase-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0      158 2023-04-21 03:08:02.000000 har2jicase-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 09:51:18.007958 har2jicase-0.1.7/har2jicase.egg-info/
--rw-rw-rw-   0        0        0      518 2023-04-21 09:51:17.000000 har2jicase-0.1.7/har2jicase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-04-21 09:51:17.000000 har2jicase-0.1.7/har2jicase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 09:51:17.000000 har2jicase-0.1.7/har2jicase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-04-21 09:51:17.000000 har2jicase-0.1.7/har2jicase.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       43 2023-04-21 09:51:17.000000 har2jicase-0.1.7/har2jicase.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-21 09:51:17.000000 har2jicase-0.1.7/har2jicase.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-21 04:57:38.000000 har2jicase-0.1.7/har2jicase.egg-info/zip-safe
-drwxrwxrwx   0        0        0        0 2023-04-21 09:51:18.009957 har2jicase-0.1.7/har_to_case/
--rw-rw-rw-   0        0        0      260 2023-04-21 09:51:17.000000 har2jicase-0.1.7/har_to_case/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 09:51:18.010957 har2jicase-0.1.7/har_to_case/common/
--rw-rw-rw-   0        0        0      204 2022-10-26 08:00:20.000000 har2jicase-0.1.7/har_to_case/common/__init__.py
--rw-rw-rw-   0        0        0     3070 2023-04-20 06:19:26.000000 har2jicase-0.1.7/har_to_case/common/tools.py
--rw-rw-rw-   0        0        0     1383 2023-04-21 09:06:51.000000 har2jicase-0.1.7/har_to_case/main.py
--rw-rw-rw-   0        0        0     8754 2023-04-21 08:37:55.000000 har2jicase-0.1.7/har_to_case/parse_har.py
--rw-rw-rw-   0        0        0       42 2023-04-21 09:51:18.011957 har2jicase-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     3945 2023-04-21 09:51:16.000000 har2jicase-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 10:37:34.276045 har2jicase-0.1.8/
+-rw-rw-rw-   0        0        0      518 2023-04-23 10:37:34.276045 har2jicase-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0      158 2023-04-21 03:08:02.000000 har2jicase-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 10:37:34.271043 har2jicase-0.1.8/har2jicase.egg-info/
+-rw-rw-rw-   0        0        0      518 2023-04-23 10:37:34.000000 har2jicase-0.1.8/har2jicase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-04-23 10:37:34.000000 har2jicase-0.1.8/har2jicase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 10:37:34.000000 har2jicase-0.1.8/har2jicase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-04-23 10:37:34.000000 har2jicase-0.1.8/har2jicase.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       43 2023-04-23 10:37:34.000000 har2jicase-0.1.8/har2jicase.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-23 10:37:34.000000 har2jicase-0.1.8/har2jicase.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-21 04:57:38.000000 har2jicase-0.1.8/har2jicase.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-04-23 10:37:34.274046 har2jicase-0.1.8/har_to_case/
+-rw-rw-rw-   0        0        0      260 2023-04-23 10:37:34.000000 har2jicase-0.1.8/har_to_case/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 10:37:34.275046 har2jicase-0.1.8/har_to_case/common/
+-rw-rw-rw-   0        0        0      204 2022-10-26 08:00:20.000000 har2jicase-0.1.8/har_to_case/common/__init__.py
+-rw-rw-rw-   0        0        0     3070 2023-04-20 06:19:26.000000 har2jicase-0.1.8/har_to_case/common/tools.py
+-rw-rw-rw-   0        0        0     1383 2023-04-21 09:06:51.000000 har2jicase-0.1.8/har_to_case/main.py
+-rw-rw-rw-   0        0        0     8756 2023-04-23 10:36:59.000000 har2jicase-0.1.8/har_to_case/parse_har.py
+-rw-rw-rw-   0        0        0       42 2023-04-23 10:37:34.277045 har2jicase-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     4102 2023-04-23 10:37:23.000000 har2jicase-0.1.8/setup.py
```

### Comparing `har2jicase-0.1.7/PKG-INFO` & `har2jicase-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: har2jicase
-Version: 0.1.7
+Version: 0.1.8
 Summary: 将浏览器录制的har文件转换为极星测试框架的YAML测试用例
 Home-page: 
 Author: Captain Ji
 Author-email: qing.ji@extremevision.com.cn
 License: MIT
 Keywords: har json compare comparison case yaml yml
 Requires-Python: >=3.6.13
```

### Comparing `har2jicase-0.1.7/har2jicase.egg-info/PKG-INFO` & `har2jicase-0.1.8/har2jicase.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: har2jicase
-Version: 0.1.7
+Version: 0.1.8
 Summary: 将浏览器录制的har文件转换为极星测试框架的YAML测试用例
 Home-page: 
 Author: Captain Ji
 Author-email: qing.ji@extremevision.com.cn
 License: MIT
 Keywords: har json compare comparison case yaml yml
 Requires-Python: >=3.6.13
```

### Comparing `har2jicase-0.1.7/har_to_case/common/tools.py` & `har2jicase-0.1.8/har_to_case/common/tools.py`

 * *Files identical despite different names*

### Comparing `har2jicase-0.1.7/har_to_case/main.py` & `har2jicase-0.1.8/har_to_case/main.py`

 * *Files identical despite different names*

### Comparing `har2jicase-0.1.7/har_to_case/parse_har.py` & `har2jicase-0.1.8/har_to_case/parse_har.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
             if isinstance(data, dict):
                 for key in data.keys():
                     if validate_contains == '':
                         validate_contains = key
                     else:
                         validate_contains = validate_contains + '-' + key
             elif isinstance(data, str):
-                validate_contains = data
+                validate_contains = 'data'
             else:
                 for item in data:
                     # todo: data中的data继续解析，后续看需求再定
                     if isinstance(item, dict):
                         pass
                     else:
                         if validate_contains == '':
```

### Comparing `har2jicase-0.1.7/setup.py` & `har2jicase-0.1.8/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,37 +19,40 @@
 import io
 import os
 import sys
 from shutil import rmtree
 from setuptools import find_packages, setup, Command
 
 # 写入自己的内容
-VERSION = '0.1.7'  # 为项目指定目前的版本号
+VERSION = '0.1.8'  # 为项目指定目前的版本号
+# 项目目录
+PROJECT_PATH = 'har_to_case'
 
 NAME = 'har2jicase'  # 项目名
 DESCRIPTION = '将浏览器录制的har文件转换为极星测试框架的YAML测试用例'
 KEYWORDS = 'har json compare comparison case yaml yml'
 AUTHOR = 'Captain Ji'
 EMAIL = 'qing.ji@extremevision.com.cn'
 URL = ''  # 项目git地址
 LICENSE = 'MIT'  # 项目license
-PACKAGES = find_packages(include=('har*',))  # 项目包含的包exclude为排除的包
+PACKAGES = find_packages(include=('har*',))  # 项目包含的包exclude=为排除的包
 REQUIRES_PYTHON = '>=3.6.13'
-PROJECT_PATH = 'har_to_case'
 pypi_username = 'jiqing19861123'
 pypi_password = 'CJ2938cj'
 # 项目依赖的库
 REQUIRED = ['loguru~=0.6.0', 'haralyzer~=2.2.0', 'PyYAML~=6.0']
 # 项目入口文件
 ENTRY_POINTS = {
     'console_scripts': [
         f'har2case = {PROJECT_PATH}.main:main'
     ]
 }
 
+# -------------------------------------以下为自动内容如无必要无需改动----------------------------------------------------
+
 here = os.path.abspath(os.path.dirname(__file__))
 
 try:
     with io.open(os.path.join(f"{here}/{PROJECT_PATH}", 'README.md'), encoding='utf-8') as f:
         LONG_DESC = '\n' + f.read()
 except FileNotFoundError:
     LONG_DESC = DESCRIPTION
```

