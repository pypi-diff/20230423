# Comparing `tmp/dg-itest-0.0.4.tar.gz` & `tmp/dg-itest-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dg-itest-0.0.4.tar", last modified: Thu Apr 20 10:57:41 2023, max compression
+gzip compressed data, was "dg-itest-0.0.5.tar", last modified: Sun Apr 23 02:30:07 2023, max compression
```

## Comparing `dg-itest-0.0.4.tar` & `dg-itest-0.0.5.tar`

### file list

```diff
@@ -1,36 +1,38 @@
-drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-20 10:57:41.268612 dg-itest-0.0.4/
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      150 2023-04-20 10:13:24.000000 dg-itest-0.0.4/MANIFEST.in
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      286 2023-04-20 10:57:41.268482 dg-itest-0.0.4/PKG-INFO
--rw-r--r--   0 yaitzayoung   (501) staff       (20)     6266 2023-04-20 09:12:27.000000 dg-itest-0.0.4/README.md
-drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-20 10:57:41.267008 dg-itest-0.0.4/dg_itest/
--rw-r--r--   0 yaitzayoung   (501) staff       (20)     1579 2023-04-20 10:57:05.000000 dg-itest-0.0.4/dg_itest/__init__.py
-drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-20 10:57:41.267896 dg-itest-0.0.4/dg_itest/servers/
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      127 2023-04-20 10:36:06.000000 dg-itest-0.0.4/dg_itest/servers/__init__.py
-drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-20 10:57:41.261618 dg-itest-0.0.4/dg_itest/servers/dg_servers/
--rw-r--r--   0 yaitzayoung   (501) staff       (20)        0 2023-04-20 10:34:49.000000 dg-itest-0.0.4/dg_itest/servers/dg_servers/__init__.py
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      793 2023-04-20 07:15:06.000000 dg-itest-0.0.4/dg_itest/servers/dg_servers/dg_requsts.py
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      531 2023-04-20 07:15:06.000000 dg-itest-0.0.4/dg_itest/servers/dg_servers/dg_singleton.py
-drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-20 10:57:41.264030 dg-itest-0.0.4/dg_itest/servers/file_handler/
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      127 2023-04-20 10:36:06.000000 dg-itest-0.0.4/dg_itest/servers/file_handler/__init__.py
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      591 2023-04-20 07:15:06.000000 dg-itest-0.0.4/dg_itest/servers/file_handler/file_handler.py
--rw-r--r--   0 yaitzayoung   (501) staff       (20)     1470 2023-04-20 07:15:06.000000 dg-itest-0.0.4/dg_itest/servers/file_handler/xlsx_handler.py
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      343 2023-04-20 07:15:06.000000 dg-itest-0.0.4/dg_itest/servers/file_handler/yaml_handler.py
-drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-20 10:57:41.265193 dg-itest-0.0.4/dg_itest/servers/test_handler/
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      127 2023-04-20 10:36:06.000000 dg-itest-0.0.4/dg_itest/servers/test_handler/__init__.py
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      558 2023-04-20 08:25:46.000000 dg-itest-0.0.4/dg_itest/servers/test_handler/test_file.py
--rw-r--r--   0 yaitzayoung   (501) staff       (20)     3477 2023-04-20 07:15:06.000000 dg-itest-0.0.4/dg_itest/servers/test_handler/test_item.py
-drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-20 10:57:41.266747 dg-itest-0.0.4/dg_itest/utils/
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      127 2023-04-20 10:36:06.000000 dg-itest-0.0.4/dg_itest/utils/__init__.py
--rw-r--r--   0 yaitzayoung   (501) staff       (20)       53 2023-04-18 13:18:59.000000 dg-itest-0.0.4/dg_itest/utils/cache.py
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      661 2023-04-20 09:01:39.000000 dg-itest-0.0.4/dg_itest/utils/diff_helper.py
--rw-r--r--   0 yaitzayoung   (501) staff       (20)     1276 2023-04-20 08:19:36.000000 dg-itest-0.0.4/dg_itest/utils/env_generater.py
--rw-r--r--   0 yaitzayoung   (501) staff       (20)     1209 2023-04-18 13:18:59.000000 dg-itest-0.0.4/dg_itest/utils/string_helper.py
-drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-20 10:57:41.267794 dg-itest-0.0.4/dg_itest.egg-info/
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      286 2023-04-20 10:57:41.000000 dg-itest-0.0.4/dg_itest.egg-info/PKG-INFO
--rw-r--r--   0 yaitzayoung   (501) staff       (20)     1458 2023-04-20 10:57:41.000000 dg-itest-0.0.4/dg_itest.egg-info/SOURCES.txt
--rw-r--r--   0 yaitzayoung   (501) staff       (20)        1 2023-04-20 10:57:41.000000 dg-itest-0.0.4/dg_itest.egg-info/dependency_links.txt
--rw-r--r--   0 yaitzayoung   (501) staff       (20)        1 2023-04-20 10:57:41.000000 dg-itest-0.0.4/dg_itest.egg-info/not-zip-safe
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      362 2023-04-20 10:57:41.000000 dg-itest-0.0.4/dg_itest.egg-info/requires.txt
--rw-r--r--   0 yaitzayoung   (501) staff       (20)        9 2023-04-20 10:57:41.000000 dg-itest-0.0.4/dg_itest.egg-info/top_level.txt
--rw-r--r--   0 yaitzayoung   (501) staff       (20)       38 2023-04-20 10:57:41.268646 dg-itest-0.0.4/setup.cfg
--rw-r--r--   0 yaitzayoung   (501) staff       (20)      879 2023-04-20 10:57:06.000000 dg-itest-0.0.4/setup.py
+drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-23 02:30:07.293654 dg-itest-0.0.5/
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      286 2023-04-23 02:30:07.293563 dg-itest-0.0.5/PKG-INFO
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)     5861 2023-04-21 02:26:19.000000 dg-itest-0.0.5/README.md
+drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-23 02:30:07.289245 dg-itest-0.0.5/dg_itest/
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)     1738 2023-04-21 07:56:28.000000 dg-itest-0.0.5/dg_itest/__init__.py
+drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-23 02:30:07.290254 dg-itest-0.0.5/dg_itest/servers/
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      127 2023-04-21 01:59:08.000000 dg-itest-0.0.5/dg_itest/servers/__init__.py
+drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-23 02:30:07.290829 dg-itest-0.0.5/dg_itest/servers/dg_servers/
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)        0 2023-04-21 01:59:08.000000 dg-itest-0.0.5/dg_itest/servers/dg_servers/__init__.py
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      793 2023-04-21 01:59:08.000000 dg-itest-0.0.5/dg_itest/servers/dg_servers/dg_requsts.py
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      531 2023-04-21 01:59:08.000000 dg-itest-0.0.5/dg_itest/servers/dg_servers/dg_singleton.py
+drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-23 02:30:07.291365 dg-itest-0.0.5/dg_itest/servers/file_handler/
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      127 2023-04-21 01:59:08.000000 dg-itest-0.0.5/dg_itest/servers/file_handler/__init__.py
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      591 2023-04-21 01:59:08.000000 dg-itest-0.0.5/dg_itest/servers/file_handler/file_handler.py
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)     1470 2023-04-21 01:59:08.000000 dg-itest-0.0.5/dg_itest/servers/file_handler/xlsx_handler.py
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      343 2023-04-21 01:59:08.000000 dg-itest-0.0.5/dg_itest/servers/file_handler/yaml_handler.py
+drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-23 02:30:07.291743 dg-itest-0.0.5/dg_itest/servers/test_handler/
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      127 2023-04-21 01:59:08.000000 dg-itest-0.0.5/dg_itest/servers/test_handler/__init__.py
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      558 2023-04-21 01:59:08.000000 dg-itest-0.0.5/dg_itest/servers/test_handler/test_file.py
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)     3712 2023-04-23 01:37:13.000000 dg-itest-0.0.5/dg_itest/servers/test_handler/test_item.py
+drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-23 02:30:07.293120 dg-itest-0.0.5/dg_itest/utils/
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      127 2023-04-21 01:59:08.000000 dg-itest-0.0.5/dg_itest/utils/__init__.py
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)       53 2023-04-21 11:38:22.000000 dg-itest-0.0.5/dg_itest/utils/cache.py
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      661 2023-04-21 01:59:08.000000 dg-itest-0.0.5/dg_itest/utils/diff_helper.py
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)     1276 2023-04-21 01:59:08.000000 dg-itest-0.0.5/dg_itest/utils/env_generater.py
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)     1568 2023-04-23 02:09:23.000000 dg-itest-0.0.5/dg_itest/utils/replace.py
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)     1209 2023-04-21 01:59:08.000000 dg-itest-0.0.5/dg_itest/utils/string_helper.py
+drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-23 02:30:07.290162 dg-itest-0.0.5/dg_itest.egg-info/
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      286 2023-04-23 02:30:07.000000 dg-itest-0.0.5/dg_itest.egg-info/PKG-INFO
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      884 2023-04-23 02:30:07.000000 dg-itest-0.0.5/dg_itest.egg-info/SOURCES.txt
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)        1 2023-04-23 02:30:07.000000 dg-itest-0.0.5/dg_itest.egg-info/dependency_links.txt
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)        1 2023-04-23 02:30:07.000000 dg-itest-0.0.5/dg_itest.egg-info/not-zip-safe
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      362 2023-04-23 02:30:07.000000 dg-itest-0.0.5/dg_itest.egg-info/requires.txt
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)        9 2023-04-23 02:30:07.000000 dg-itest-0.0.5/dg_itest.egg-info/top_level.txt
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)       38 2023-04-23 02:30:07.293685 dg-itest-0.0.5/setup.cfg
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      879 2023-04-23 02:29:24.000000 dg-itest-0.0.5/setup.py
+drwxr-xr-x   0 yaitzayoung   (501) staff       (20)        0 2023-04-23 02:30:07.293273 dg-itest-0.0.5/test/
+-rw-r--r--   0 yaitzayoung   (501) staff       (20)      549 2023-04-23 02:09:23.000000 dg-itest-0.0.5/test/test_replace.py
```

### Comparing `dg-itest-0.0.4/README.md` & `dg-itest-0.0.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 # 1. 文档说明
 
-本文档主要用于接口自动化测试框架说明以及相关实现规范。
+本文档主要用于接口自动化测试框架说明以及使用。
 
 ## 1.1 环境准备
 
 * IDE：Pycharm 等;
 * Python 3.7以上;
-* 引用类库，见requirments.txt; 命令：`pip install -r requirements.txt`  
-**备注：** 新增引用类库，请更新requirements.txt。
-  
-    本地python环境，项目根目录下，`pip install pipreqs; pipreqs . --encoding=utf8 --force`;建议使用此项更新  requirements.txt。
-    python虚拟环境：`pip freeze > requirements.txt`
-  
+* 引用类库，dg-itest; 命令：`pip install dg-itest`
 * allure 本地环境配置  
 
     **step 1** pip install allure-pytest  
     **step 2** 下载Allure版本：[Download](https://github.com/allure-framework/allure2/releases) 并配置到PATH路径下
         对应家目录下，`.bash_profile` 配置如下：  
     
         # Setting PATH for Python 3.9
@@ -124,8 +119,7 @@
 * 支持断言关键字：
   - eq：将根据请求按照路径获取的值与expect进行判等
   - sa：将把请求得到的值按照路径获取并以对应$key$存储以供后续使用。
 
 # 5. 参考文档
 - [1] [pytest](https://www.osgeo.cn/pytest/contents.html) - https://www.osgeo.cn/pytest/contents.html
 - [2] [allure en](https://docs.qameta.io/allure/) - https://docs.qameta.io/allure/
-- [2] [allure zh](https://qualitysphere.github.io/4_allure/) - https://docs.qameta.io/allure/
```

### Comparing `dg-itest-0.0.4/dg_itest/__init__.py` & `dg-itest-0.0.5/dg_itest/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # @Author  : yaitza
 # @Email   : yaitza@foxmail.com
 
 __all__ = ["DgItest"]
 
 import os
 import logging
+import sys
 from pathlib import *
 from dg_itest.utils.env_generater import EnvGenerater
 
 import pytest
 
 _logger = logging.root
 
@@ -54,8 +55,15 @@
         try:
             # 生成allure report中environment相关配置
             EnvGenerater.generate_env_file(host_url, Path(test_report))
 
             # 本地生成allure report 使用; 本地生成报告使用，commit时请注释
             os.system("allure generate ./test_report/result/ -o ./test_report/report --clean")
         except Exception:
-            get_logger().error("请确保本地安装有allure，参考：https://docs.qameta.io/allure/")
+            get_logger().error("请确保本地安装有allure，参考：https://docs.qameta.io/allure/")
+
+if __name__ == '__main__':
+    url = sys.argv[0]
+    test_src = sys.argv[1]
+    test_res = sys.argv[2]
+
+    DgItest(url, test_src, test_res).run()
```

### Comparing `dg-itest-0.0.4/dg_itest/servers/dg_servers/dg_requsts.py` & `dg-itest-0.0.5/dg_itest/servers/dg_servers/dg_requsts.py`

 * *Files identical despite different names*

### Comparing `dg-itest-0.0.4/dg_itest/servers/dg_servers/dg_singleton.py` & `dg-itest-0.0.5/dg_itest/servers/dg_servers/dg_singleton.py`

 * *Files identical despite different names*

### Comparing `dg-itest-0.0.4/dg_itest/servers/file_handler/file_handler.py` & `dg-itest-0.0.5/dg_itest/servers/file_handler/file_handler.py`

 * *Files identical despite different names*

### Comparing `dg-itest-0.0.4/dg_itest/servers/file_handler/xlsx_handler.py` & `dg-itest-0.0.5/dg_itest/servers/file_handler/xlsx_handler.py`

 * *Files identical despite different names*

### Comparing `dg-itest-0.0.4/dg_itest/servers/test_handler/test_file.py` & `dg-itest-0.0.5/dg_itest/servers/test_handler/test_file.py`

 * *Files identical despite different names*

### Comparing `dg-itest-0.0.4/dg_itest/servers/test_handler/test_item.py` & `dg-itest-0.0.5/dg_itest/servers/test_handler/test_item.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,28 +8,30 @@
 import pytest
 import jsonpath
 from pathlib import *
 from dg_itest import local_test_res
 from dg_itest.utils.diff_helper import DiffHelper
 from dg_itest.servers.dg_servers.dg_singleton import DgSingleton
 from dg_itest.utils.cache import local_cache
+from dg_itest.utils.replace import Replace
 
 
 class TestItem(pytest.Item):
     def __init__(self, name, parent, values):
         super(TestItem, self).__init__(name, parent)
         self.name = name
         self.values = values
         self.request = self.values.get("request")
         self.validate = self.values.get("validate")
         self.expect = self.values.get('expect')
 
     def runtest(self):
         request_data = self.values['request']
-        params = self.replace(request_data['params'])
+        params = self.replace(request_data)
+        params = request_data['params']
         if "files" in params.keys():
                 params.update({"files": self.get_files(params.get("files"))})
         request_data.pop('params')
         request_data.update(params)
 
         try:
             api = DgSingleton().apis
@@ -54,22 +56,27 @@
             if "sa" in item.keys():
                 sa_value = item.get("sa")
                 for sa_item_key in sa_value.keys():
                     sa_item_value =  jsonpath.jsonpath(response.json(), sa_value.get(sa_item_key))
                     assert type(sa_item_value) is list and len(sa_item_value) > 0, '\n' + '未获取到值'
                     local_cache[f"${sa_item_key}$"] = sa_item_value[0]
 
-    def replace(self, source_dict):
-        source_str = json.dumps(source_dict)
-        pattern = re.compile(r'\$.*?\$', re.DOTALL)
-        results = pattern.findall(source_str)
-
-        for item in results:
-            source_str = source_str.replace(item, str(local_cache[item]))
-        return json.loads(source_str)
+    def replace(self, source):
+        pattern_str = r'\$.*?\$'
+        source_str = json.dumps(source)
+        pattern = re.compile(pattern_str, re.DOTALL)
+        match_items = pattern.findall(source_str)
+        update = {}
+        for items in match_items:
+            update.update({items: local_cache[items]})
+        if len(update.keys()) > 0:
+            result = Replace.replace(pattern_str, source, update)
+            return result
+        else:
+            return source
 
     def get_files(self, files_array):
         all_resource_files = Path(local_test_res).rglob("*.*")
         files_buffer = []
         for file_name in files_array:
             file = [file_item for file_item in all_resource_files if file_item.name == file_name]
             if len(file) > 0:
```

### Comparing `dg-itest-0.0.4/dg_itest/utils/diff_helper.py` & `dg-itest-0.0.5/dg_itest/utils/diff_helper.py`

 * *Files identical despite different names*

### Comparing `dg-itest-0.0.4/dg_itest/utils/env_generater.py` & `dg-itest-0.0.5/dg_itest/utils/env_generater.py`

 * *Files identical despite different names*

### Comparing `dg-itest-0.0.4/dg_itest/utils/string_helper.py` & `dg-itest-0.0.5/dg_itest/utils/string_helper.py`

 * *Files identical despite different names*

### Comparing `dg-itest-0.0.4/dg_itest.egg-info/SOURCES.txt` & `dg-itest-0.0.5/dg_itest.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,9 @@
-MANIFEST.in
 README.md
 setup.py
-./dg_itest/servers/dg_servers/__init__.py
-./dg_itest/servers/dg_servers/dg_requsts.py
-./dg_itest/servers/dg_servers/dg_singleton.py
-./dg_itest/servers/file_handler/__init__.py
-./dg_itest/servers/file_handler/file_handler.py
-./dg_itest/servers/file_handler/xlsx_handler.py
-./dg_itest/servers/file_handler/yaml_handler.py
-./dg_itest/servers/test_handler/__init__.py
-./dg_itest/servers/test_handler/test_file.py
-./dg_itest/servers/test_handler/test_item.py
-./dg_itest/utils/__init__.py
-./dg_itest/utils/cache.py
-./dg_itest/utils/diff_helper.py
-./dg_itest/utils/env_generater.py
-./dg_itest/utils/string_helper.py
 dg_itest/__init__.py
 dg_itest.egg-info/PKG-INFO
 dg_itest.egg-info/SOURCES.txt
 dg_itest.egg-info/dependency_links.txt
 dg_itest.egg-info/not-zip-safe
 dg_itest.egg-info/requires.txt
 dg_itest.egg-info/top_level.txt
@@ -34,8 +18,10 @@
 dg_itest/servers/test_handler/__init__.py
 dg_itest/servers/test_handler/test_file.py
 dg_itest/servers/test_handler/test_item.py
 dg_itest/utils/__init__.py
 dg_itest/utils/cache.py
 dg_itest/utils/diff_helper.py
 dg_itest/utils/env_generater.py
-dg_itest/utils/string_helper.py
+dg_itest/utils/replace.py
+dg_itest/utils/string_helper.py
+test/test_replace.py
```

### Comparing `dg-itest-0.0.4/setup.py` & `dg-itest-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     if not os.path.exists(requirements):  # install from tar
         requirements = 'dg_itest.egg-info/requires.txt'
     with open(requirements) as fp:
         install_requires = fp.read()
     return install_requires.split('\n')
 
 setup(name='dg-itest',
-      version='0.0.4',
+      version='0.0.5',
       description='接口自动化测试框架',
       url='https://github.com/yaitza/dg-itest',
       download_url='https://github.com/yaitza/dg-itest/releases',
       author='yaitza',
       author_email='yaitza@foxmail.com',
       packages=find_packages(),
       package_data={'': ['*.py']},
```

