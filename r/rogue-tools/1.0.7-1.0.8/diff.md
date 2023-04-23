# Comparing `tmp/rogue_tools-1.0.7.tar.gz` & `tmp/rogue_tools-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rogue_tools-1.0.7.tar", last modified: Sun Apr 23 02:10:28 2023, max compression
+gzip compressed data, was "rogue_tools-1.0.8.tar", last modified: Sun Apr 23 02:18:05 2023, max compression
```

## Comparing `rogue_tools-1.0.7.tar` & `rogue_tools-1.0.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 02:10:28.370207 rogue_tools-1.0.7/
--rw-rw-rw-   0        0        0      517 2023-04-23 02:10:28.370207 rogue_tools-1.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-23 02:10:28.356335 rogue_tools-1.0.7/rogue_tools/
--rw-rw-rw-   0        0        0        0 2023-03-03 12:10:10.000000 rogue_tools-1.0.7/rogue_tools/__init__.py
--rw-rw-rw-   0        0        0     6206 2023-04-12 11:49:44.000000 rogue_tools-1.0.7/rogue_tools/android_tool.py
--rw-rw-rw-   0        0        0     6255 2023-04-12 11:49:44.000000 rogue_tools-1.0.7/rogue_tools/excel_tool.py
--rw-rw-rw-   0        0        0     4056 2023-04-12 11:49:44.000000 rogue_tools-1.0.7/rogue_tools/file_tool.py
--rw-rw-rw-   0        0        0     1157 2023-04-12 11:49:44.000000 rogue_tools-1.0.7/rogue_tools/filter_tool.py
--rw-rw-rw-   0        0        0     2353 2023-04-12 11:49:44.000000 rogue_tools-1.0.7/rogue_tools/ini_tool.py
--rw-rw-rw-   0        0        0    13260 2023-04-13 10:09:49.000000 rogue_tools-1.0.7/rogue_tools/path_tool.py
--rw-rw-rw-   0        0        0     2416 2023-04-12 11:49:44.000000 rogue_tools-1.0.7/rogue_tools/robot_tool.py
--rw-rw-rw-   0        0        0     4064 2023-04-12 11:49:45.000000 rogue_tools-1.0.7/rogue_tools/show_tool.py
--rw-rw-rw-   0        0        0      147 2023-04-12 11:49:45.000000 rogue_tools-1.0.7/rogue_tools/string_tool.py
--rw-rw-rw-   0        0        0     1862 2023-04-20 11:22:01.000000 rogue_tools-1.0.7/rogue_tools/time_tool.py
--rw-rw-rw-   0        0        0     2922 2023-04-12 11:49:45.000000 rogue_tools-1.0.7/rogue_tools/ui_tool.py
--rw-rw-rw-   0        0        0     2284 2023-04-19 08:46:05.000000 rogue_tools-1.0.7/rogue_tools/web_tool.py
--rw-rw-rw-   0        0        0    17995 2023-04-12 11:49:45.000000 rogue_tools-1.0.7/rogue_tools/win_tool.py
--rw-rw-rw-   0        0        0     3912 2023-04-20 09:55:42.000000 rogue_tools-1.0.7/rogue_tools/yaml_tool.py
--rw-rw-rw-   0        0        0     1260 2023-04-12 11:49:45.000000 rogue_tools-1.0.7/rogue_tools/zip_tool.py
-drwxrwxrwx   0        0        0        0 2023-04-23 02:10:28.368210 rogue_tools-1.0.7/rogue_tools.egg-info/
--rw-rw-rw-   0        0        0      517 2023-04-23 02:10:28.000000 rogue_tools-1.0.7/rogue_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      614 2023-04-23 02:10:28.000000 rogue_tools-1.0.7/rogue_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 02:10:28.000000 rogue_tools-1.0.7/rogue_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2023-04-23 02:10:28.000000 rogue_tools-1.0.7/rogue_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-23 02:10:28.000000 rogue_tools-1.0.7/rogue_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-23 02:10:28.000000 rogue_tools-1.0.7/rogue_tools.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-04-23 02:10:28.370207 rogue_tools-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1777 2023-04-23 02:10:21.000000 rogue_tools-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 02:18:05.889085 rogue_tools-1.0.8/
+-rw-rw-rw-   0        0        0      517 2023-04-23 02:18:05.889085 rogue_tools-1.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-23 02:18:05.876226 rogue_tools-1.0.8/rogue_tools/
+-rw-rw-rw-   0        0        0        0 2023-03-03 12:10:10.000000 rogue_tools-1.0.8/rogue_tools/__init__.py
+-rw-rw-rw-   0        0        0     6206 2023-04-12 11:49:44.000000 rogue_tools-1.0.8/rogue_tools/android_tool.py
+-rw-rw-rw-   0        0        0     6255 2023-04-12 11:49:44.000000 rogue_tools-1.0.8/rogue_tools/excel_tool.py
+-rw-rw-rw-   0        0        0     4056 2023-04-12 11:49:44.000000 rogue_tools-1.0.8/rogue_tools/file_tool.py
+-rw-rw-rw-   0        0        0     1157 2023-04-12 11:49:44.000000 rogue_tools-1.0.8/rogue_tools/filter_tool.py
+-rw-rw-rw-   0        0        0     2353 2023-04-12 11:49:44.000000 rogue_tools-1.0.8/rogue_tools/ini_tool.py
+-rw-rw-rw-   0        0        0    13260 2023-04-13 10:09:49.000000 rogue_tools-1.0.8/rogue_tools/path_tool.py
+-rw-rw-rw-   0        0        0     2416 2023-04-12 11:49:44.000000 rogue_tools-1.0.8/rogue_tools/robot_tool.py
+-rw-rw-rw-   0        0        0     4064 2023-04-12 11:49:45.000000 rogue_tools-1.0.8/rogue_tools/show_tool.py
+-rw-rw-rw-   0        0        0      147 2023-04-12 11:49:45.000000 rogue_tools-1.0.8/rogue_tools/string_tool.py
+-rw-rw-rw-   0        0        0     1862 2023-04-20 11:22:01.000000 rogue_tools-1.0.8/rogue_tools/time_tool.py
+-rw-rw-rw-   0        0        0     2922 2023-04-12 11:49:45.000000 rogue_tools-1.0.8/rogue_tools/ui_tool.py
+-rw-rw-rw-   0        0        0     2300 2023-04-23 02:16:48.000000 rogue_tools-1.0.8/rogue_tools/web_tool.py
+-rw-rw-rw-   0        0        0    17995 2023-04-12 11:49:45.000000 rogue_tools-1.0.8/rogue_tools/win_tool.py
+-rw-rw-rw-   0        0        0     3912 2023-04-20 09:55:42.000000 rogue_tools-1.0.8/rogue_tools/yaml_tool.py
+-rw-rw-rw-   0        0        0     1260 2023-04-12 11:49:45.000000 rogue_tools-1.0.8/rogue_tools/zip_tool.py
+drwxrwxrwx   0        0        0        0 2023-04-23 02:18:05.887091 rogue_tools-1.0.8/rogue_tools.egg-info/
+-rw-rw-rw-   0        0        0      517 2023-04-23 02:18:05.000000 rogue_tools-1.0.8/rogue_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      614 2023-04-23 02:18:05.000000 rogue_tools-1.0.8/rogue_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 02:18:05.000000 rogue_tools-1.0.8/rogue_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2023-04-23 02:18:05.000000 rogue_tools-1.0.8/rogue_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-23 02:18:05.000000 rogue_tools-1.0.8/rogue_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-23 02:18:05.000000 rogue_tools-1.0.8/rogue_tools.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-04-23 02:18:05.889085 rogue_tools-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1777 2023-04-23 02:17:59.000000 rogue_tools-1.0.8/setup.py
```

### Comparing `rogue_tools-1.0.7/PKG-INFO` & `rogue_tools-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rogue_tools
-Version: 1.0.7
+Version: 1.0.8
 Summary: private tools
 Home-page: 
 Author: luohao
 Author-email: luohao@aobi.com
 License: MIT
 Classifier: Operating System :: Microsoft
 Classifier: Intended Audience :: Developers
```

### Comparing `rogue_tools-1.0.7/rogue_tools/android_tool.py` & `rogue_tools-1.0.8/rogue_tools/android_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.7/rogue_tools/excel_tool.py` & `rogue_tools-1.0.8/rogue_tools/excel_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.7/rogue_tools/file_tool.py` & `rogue_tools-1.0.8/rogue_tools/file_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.7/rogue_tools/filter_tool.py` & `rogue_tools-1.0.8/rogue_tools/filter_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.7/rogue_tools/ini_tool.py` & `rogue_tools-1.0.8/rogue_tools/ini_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.7/rogue_tools/path_tool.py` & `rogue_tools-1.0.8/rogue_tools/path_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.7/rogue_tools/robot_tool.py` & `rogue_tools-1.0.8/rogue_tools/robot_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.7/rogue_tools/show_tool.py` & `rogue_tools-1.0.8/rogue_tools/show_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.7/rogue_tools/time_tool.py` & `rogue_tools-1.0.8/rogue_tools/time_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.7/rogue_tools/ui_tool.py` & `rogue_tools-1.0.8/rogue_tools/ui_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.7/rogue_tools/web_tool.py` & `rogue_tools-1.0.8/rogue_tools/web_tool.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import re
 import time
 from tqdm import tqdm
 from concurrent.futures import ThreadPoolExecutor
 import traceback
 
 
-def get_ip_public():
+def get_ip_public(timeout=60):
     '''公网ip'''
-    text = requests.get('http://myip.ipip.net',timeout=3).text
+    text = requests.get('http://myip.ipip.net',timeout=timeout).text
     pattern = r"\d{1,3}.\d{1,3}.\d{1,3}.\d{1,3}"
     rs = re.search(pattern,text)
     return rs.group()
 
 def get_ip_local_area_network():
     '''局域网ip'''
     with socket.socket(socket.AF_INET, socket.SOCK_DGRAM) as s:
```

### Comparing `rogue_tools-1.0.7/rogue_tools/win_tool.py` & `rogue_tools-1.0.8/rogue_tools/win_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.7/rogue_tools/yaml_tool.py` & `rogue_tools-1.0.8/rogue_tools/yaml_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.7/rogue_tools/zip_tool.py` & `rogue_tools-1.0.8/rogue_tools/zip_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.7/rogue_tools.egg-info/PKG-INFO` & `rogue_tools-1.0.8/rogue_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rogue-tools
-Version: 1.0.7
+Version: 1.0.8
 Summary: private tools
 Home-page: 
 Author: luohao
 Author-email: luohao@aobi.com
 License: MIT
 Classifier: Operating System :: Microsoft
 Classifier: Intended Audience :: Developers
```

### Comparing `rogue_tools-1.0.7/rogue_tools.egg-info/SOURCES.txt` & `rogue_tools-1.0.8/rogue_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.7/setup.py` & `rogue_tools-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 path_tool.del_('rogue_tools.egg-info')
 time.sleep(1)
 
 
 setup(
     name='rogue_tools',  # 包的名字
     author='luohao',  # 作者
-    version='1.0.7',  # 版本号
+    version='1.0.8',  # 版本号
     license='MIT',
 
     description='private tools',  # 描述
     long_description='''long description''',
     author_email='luohao@aobi.com',  # 你的邮箱**
     url='',  # 可以写github上的地址，或者其他地址
     # 包内需要引用的文件夹
```

