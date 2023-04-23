# Comparing `tmp/rogue_tools-1.0.6.tar.gz` & `tmp/rogue_tools-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rogue_tools-1.0.6.tar", last modified: Mon Apr 10 04:00:16 2023, max compression
+gzip compressed data, was "rogue_tools-1.0.7.tar", last modified: Sun Apr 23 02:10:28 2023, max compression
```

## Comparing `rogue_tools-1.0.6.tar` & `rogue_tools-1.0.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 04:00:16.676977 rogue_tools-1.0.6/
--rw-rw-rw-   0        0        0      517 2023-04-10 04:00:16.676006 rogue_tools-1.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-10 04:00:16.656490 rogue_tools-1.0.6/rogue_tools/
--rw-rw-rw-   0        0        0        0 2023-03-03 12:10:10.000000 rogue_tools-1.0.6/rogue_tools/__init__.py
--rw-rw-rw-   0        0        0     6206 2023-03-03 12:10:10.000000 rogue_tools-1.0.6/rogue_tools/android_tool.py
--rw-rw-rw-   0        0        0     6255 2023-03-07 02:54:55.000000 rogue_tools-1.0.6/rogue_tools/excel_tool.py
--rw-rw-rw-   0        0        0     4056 2023-03-03 12:10:10.000000 rogue_tools-1.0.6/rogue_tools/file_tool.py
--rw-rw-rw-   0        0        0     1157 2023-03-03 12:10:10.000000 rogue_tools-1.0.6/rogue_tools/filter_tool.py
--rw-rw-rw-   0        0        0     2353 2023-03-03 12:10:10.000000 rogue_tools-1.0.6/rogue_tools/ini_tool.py
--rw-rw-rw-   0        0        0    13253 2023-04-10 03:02:30.000000 rogue_tools-1.0.6/rogue_tools/path_tool.py
--rw-rw-rw-   0        0        0     2416 2023-03-03 12:10:10.000000 rogue_tools-1.0.6/rogue_tools/robot_tool.py
--rw-rw-rw-   0        0        0     4064 2023-03-03 12:10:10.000000 rogue_tools-1.0.6/rogue_tools/show_tool.py
--rw-rw-rw-   0        0        0      147 2023-03-03 12:10:10.000000 rogue_tools-1.0.6/rogue_tools/string_tool.py
--rw-rw-rw-   0        0        0     1862 2023-04-10 03:55:21.000000 rogue_tools-1.0.6/rogue_tools/time_tool.py
--rw-rw-rw-   0        0        0     2922 2023-03-28 09:52:02.000000 rogue_tools-1.0.6/rogue_tools/ui_tool.py
--rw-rw-rw-   0        0        0     1967 2023-03-03 12:10:10.000000 rogue_tools-1.0.6/rogue_tools/web_tool.py
--rw-rw-rw-   0        0        0    17995 2023-03-03 12:10:10.000000 rogue_tools-1.0.6/rogue_tools/win_tool.py
--rw-rw-rw-   0        0        0     3914 2023-03-03 12:10:10.000000 rogue_tools-1.0.6/rogue_tools/yaml_tool.py
--rw-rw-rw-   0        0        0     1260 2023-03-03 12:10:10.000000 rogue_tools-1.0.6/rogue_tools/zip_tool.py
-drwxrwxrwx   0        0        0        0 2023-04-10 04:00:16.674010 rogue_tools-1.0.6/rogue_tools.egg-info/
--rw-rw-rw-   0        0        0      517 2023-04-10 04:00:16.000000 rogue_tools-1.0.6/rogue_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      614 2023-04-10 04:00:16.000000 rogue_tools-1.0.6/rogue_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 04:00:16.000000 rogue_tools-1.0.6/rogue_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2023-04-10 04:00:16.000000 rogue_tools-1.0.6/rogue_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-10 04:00:16.000000 rogue_tools-1.0.6/rogue_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-10 04:00:16.000000 rogue_tools-1.0.6/rogue_tools.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-04-10 04:00:16.676977 rogue_tools-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1599 2023-04-10 03:56:58.000000 rogue_tools-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 02:10:28.370207 rogue_tools-1.0.7/
+-rw-rw-rw-   0        0        0      517 2023-04-23 02:10:28.370207 rogue_tools-1.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-23 02:10:28.356335 rogue_tools-1.0.7/rogue_tools/
+-rw-rw-rw-   0        0        0        0 2023-03-03 12:10:10.000000 rogue_tools-1.0.7/rogue_tools/__init__.py
+-rw-rw-rw-   0        0        0     6206 2023-04-12 11:49:44.000000 rogue_tools-1.0.7/rogue_tools/android_tool.py
+-rw-rw-rw-   0        0        0     6255 2023-04-12 11:49:44.000000 rogue_tools-1.0.7/rogue_tools/excel_tool.py
+-rw-rw-rw-   0        0        0     4056 2023-04-12 11:49:44.000000 rogue_tools-1.0.7/rogue_tools/file_tool.py
+-rw-rw-rw-   0        0        0     1157 2023-04-12 11:49:44.000000 rogue_tools-1.0.7/rogue_tools/filter_tool.py
+-rw-rw-rw-   0        0        0     2353 2023-04-12 11:49:44.000000 rogue_tools-1.0.7/rogue_tools/ini_tool.py
+-rw-rw-rw-   0        0        0    13260 2023-04-13 10:09:49.000000 rogue_tools-1.0.7/rogue_tools/path_tool.py
+-rw-rw-rw-   0        0        0     2416 2023-04-12 11:49:44.000000 rogue_tools-1.0.7/rogue_tools/robot_tool.py
+-rw-rw-rw-   0        0        0     4064 2023-04-12 11:49:45.000000 rogue_tools-1.0.7/rogue_tools/show_tool.py
+-rw-rw-rw-   0        0        0      147 2023-04-12 11:49:45.000000 rogue_tools-1.0.7/rogue_tools/string_tool.py
+-rw-rw-rw-   0        0        0     1862 2023-04-20 11:22:01.000000 rogue_tools-1.0.7/rogue_tools/time_tool.py
+-rw-rw-rw-   0        0        0     2922 2023-04-12 11:49:45.000000 rogue_tools-1.0.7/rogue_tools/ui_tool.py
+-rw-rw-rw-   0        0        0     2284 2023-04-19 08:46:05.000000 rogue_tools-1.0.7/rogue_tools/web_tool.py
+-rw-rw-rw-   0        0        0    17995 2023-04-12 11:49:45.000000 rogue_tools-1.0.7/rogue_tools/win_tool.py
+-rw-rw-rw-   0        0        0     3912 2023-04-20 09:55:42.000000 rogue_tools-1.0.7/rogue_tools/yaml_tool.py
+-rw-rw-rw-   0        0        0     1260 2023-04-12 11:49:45.000000 rogue_tools-1.0.7/rogue_tools/zip_tool.py
+drwxrwxrwx   0        0        0        0 2023-04-23 02:10:28.368210 rogue_tools-1.0.7/rogue_tools.egg-info/
+-rw-rw-rw-   0        0        0      517 2023-04-23 02:10:28.000000 rogue_tools-1.0.7/rogue_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      614 2023-04-23 02:10:28.000000 rogue_tools-1.0.7/rogue_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 02:10:28.000000 rogue_tools-1.0.7/rogue_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2023-04-23 02:10:28.000000 rogue_tools-1.0.7/rogue_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-23 02:10:28.000000 rogue_tools-1.0.7/rogue_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-23 02:10:28.000000 rogue_tools-1.0.7/rogue_tools.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-04-23 02:10:28.370207 rogue_tools-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1777 2023-04-23 02:10:21.000000 rogue_tools-1.0.7/setup.py
```

### Comparing `rogue_tools-1.0.6/PKG-INFO` & `rogue_tools-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rogue_tools
-Version: 1.0.6
+Version: 1.0.7
 Summary: private tools
 Home-page: 
 Author: luohao
 Author-email: luohao@aobi.com
 License: MIT
 Classifier: Operating System :: Microsoft
 Classifier: Intended Audience :: Developers
```

### Comparing `rogue_tools-1.0.6/rogue_tools/android_tool.py` & `rogue_tools-1.0.7/rogue_tools/android_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.6/rogue_tools/excel_tool.py` & `rogue_tools-1.0.7/rogue_tools/excel_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.6/rogue_tools/file_tool.py` & `rogue_tools-1.0.7/rogue_tools/file_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.6/rogue_tools/filter_tool.py` & `rogue_tools-1.0.7/rogue_tools/filter_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.6/rogue_tools/ini_tool.py` & `rogue_tools-1.0.7/rogue_tools/ini_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.6/rogue_tools/path_tool.py` & `rogue_tools-1.0.7/rogue_tools/path_tool.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         
 def copy(src, tar,is_cover=False):
     '''
     通用的复制文件或者文件夹
     is_cover = True 可以不用删除旧文件夹,直接覆盖过去
     仅支持本地copy
     '''
-    print(f'copy:{src} -->> {tar}')
+    #print(f'copy:{src} -->> {tar}')
     if type(src) in [tuple,list]:
         for obj in src:
             copy(obj,tar,is_cover)
         return
     # copy文件
     if os.path.isfile(src):
         #  复制到目录
@@ -237,20 +237,20 @@
         except Exception:
             traceback.print_exc()
 
 def make_folder(folder_path):
     '''
     创建一个文件夹
     '''
-    print(f'make_folder:{folder_path}')
     if os.path.exists(folder_path):
         return
     if folder_path in ('',None):
         return
     try:
+        #print(f'make_folder:{folder_path}')
         os.makedirs(folder_path,mode=0o777)
     except FileExistsError:
         return
     except Exception:
         traceback.print_exc()
 def del_folder(path,is_keep_folder=True):
     '''
@@ -410,15 +410,15 @@
 
 def wait_file_prepare(path,time_out=600):
     total = 0
     start_time = time_tool.time_stamp_s()
     while True and time_tool.time_stamp_s() - start_time < time_out:
         time.sleep(2)
         temp = file_tool.get_file_size(path)
-        print(f'waiting file:{time_tool.time_stamp_s() - start_time}s , {int(temp/1024)}kb')
+        #print(f'waiting file:{time_tool.time_stamp_s() - start_time}s , {int(temp/1024)}kb')
         if temp == total and temp > 0:
             return True
         else:
             total = temp
     return False
 
 def is_exists(path):
```

### Comparing `rogue_tools-1.0.6/rogue_tools/robot_tool.py` & `rogue_tools-1.0.7/rogue_tools/robot_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.6/rogue_tools/show_tool.py` & `rogue_tools-1.0.7/rogue_tools/show_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.6/rogue_tools/time_tool.py` & `rogue_tools-1.0.7/rogue_tools/time_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.6/rogue_tools/ui_tool.py` & `rogue_tools-1.0.7/rogue_tools/ui_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.6/rogue_tools/web_tool.py` & `rogue_tools-1.0.7/rogue_tools/web_tool.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,31 @@
 import os
 import socket
 import requests
-import os
+import re
 import time
 from tqdm import tqdm
 from concurrent.futures import ThreadPoolExecutor
 import traceback
 
-def get_local_IP():
-    return socket.gethostbyname(socket.getfqdn(socket.gethostname()))
+
+def get_ip_public():
+    '''公网ip'''
+    text = requests.get('http://myip.ipip.net',timeout=3).text
+    pattern = r"\d{1,3}.\d{1,3}.\d{1,3}.\d{1,3}"
+    rs = re.search(pattern,text)
+    return rs.group()
+
+def get_ip_local_area_network():
+    '''局域网ip'''
+    with socket.socket(socket.AF_INET, socket.SOCK_DGRAM) as s:
+        s.connect(("114.114.114.114", 80))
+        return s.getsockname()[0]
+
+
 
 def download_url(url,save_folder_path,is_cover=True,is_show_process=True):
     url=url.replace('\\','/')
     if not save_folder_path.endswith('\\'):
         save_folder_path=save_folder_path+'\\'
```

### Comparing `rogue_tools-1.0.6/rogue_tools/win_tool.py` & `rogue_tools-1.0.7/rogue_tools/win_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.6/rogue_tools/yaml_tool.py` & `rogue_tools-1.0.7/rogue_tools/yaml_tool.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         self.file_path=file_path
         self.cmd_dic={}
         
         try:
             dic:dict            = yaml.safe_load(open(self.file_path, encoding='utf-8'))
             self.name           = dic.get('name',None)
             self.ext_id         = dic.get('extensionId',None)
-            yaml_cmd_list       = dic.get('cmdList',None)
+            yaml_cmd_list       = dic.get('cmdList',[])
 
             for cmd in yaml_cmd_list:
                 yaml_cmd = YamlCmd(cmd)
                 self.cmd_dic[yaml_cmd.index]=yaml_cmd
 
             
         except Exception as err:
```

### Comparing `rogue_tools-1.0.6/rogue_tools/zip_tool.py` & `rogue_tools-1.0.7/rogue_tools/zip_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.6/rogue_tools.egg-info/PKG-INFO` & `rogue_tools-1.0.7/rogue_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rogue-tools
-Version: 1.0.6
+Version: 1.0.7
 Summary: private tools
 Home-page: 
 Author: luohao
 Author-email: luohao@aobi.com
 License: MIT
 Classifier: Operating System :: Microsoft
 Classifier: Intended Audience :: Developers
```

### Comparing `rogue_tools-1.0.6/rogue_tools.egg-info/SOURCES.txt` & `rogue_tools-1.0.7/rogue_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

