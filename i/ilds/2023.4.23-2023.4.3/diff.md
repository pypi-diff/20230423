# Comparing `tmp/ilds-2023.4.23.tar.gz` & `tmp/ilds-2023.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ilds-2023.4.23.tar", last modified: Sun Apr 23 03:05:34 2023, max compression
+gzip compressed data, was "dist\ilds-2023.4.3.tar", last modified: Mon Apr  3 10:59:19 2023, max compression
```

## Comparing `ilds-2023.4.23.tar` & `ilds-2023.4.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 03:05:34.000000 ilds-2023.4.23/
-drwxrwxrwx   0        0        0        0 2023-04-23 03:05:34.000000 ilds-2023.4.23/ilds/
--rw-rw-rw-   0        0        0     1797 2021-09-26 05:21:21.000000 ilds-2023.4.23/ilds/cmd.py
-drwxrwxrwx   0        0        0        0 2023-04-23 03:05:34.000000 ilds-2023.4.23/ilds/django/
--rw-rw-rw-   0        0        0     3407 2019-10-30 05:10:14.000000 ilds-2023.4.23/ilds/django/admin.py
--rw-rw-rw-   0        0        0    14906 2019-10-30 03:18:15.000000 ilds-2023.4.23/ilds/django/import_export.py
--rw-rw-rw-   0        0        0    15417 2019-11-27 09:35:07.000000 ilds-2023.4.23/ilds/django/model.py
--rw-rw-rw-   0        0        0     1840 2019-04-12 05:15:43.000000 ilds-2023.4.23/ilds/django/user.py
--rw-rw-rw-   0        0        0     2085 2021-09-28 08:04:39.000000 ilds-2023.4.23/ilds/django/util.py
--rw-rw-rw-   0        0        0        0 2018-08-07 03:24:52.000000 ilds-2023.4.23/ilds/django/__init__.py
--rw-rw-rw-   0        0        0     9150 2021-12-06 10:18:15.000000 ilds-2023.4.23/ilds/everything.py
--rw-rw-rw-   0        0        0     9470 2019-03-29 08:26:49.000000 ilds-2023.4.23/ilds/excel_xlrd.py
--rw-rw-rw-   0        0        0     7970 2022-10-19 09:11:30.000000 ilds-2023.4.23/ilds/excel_xlsx.py
--rw-rw-rw-   0        0        0    26848 2023-04-03 10:59:15.000000 ilds-2023.4.23/ilds/file.py
--rw-rw-rw-   0        0        0     1530 2023-04-10 12:39:32.000000 ilds-2023.4.23/ilds/json.py
-drwxrwxrwx   0        0        0        0 2023-04-23 03:05:34.000000 ilds-2023.4.23/ilds/lib/
--rw-rw-rw-   0        0        0    13740 2018-11-26 09:16:44.000000 ilds-2023.4.23/ilds/lib/browsercookie.py
-drwxrwxrwx   0        0        0        0 2023-04-23 03:05:34.000000 ilds-2023.4.23/ilds/lib/configobj/
--rw-rw-rw-   0        0        0    46989 2019-05-06 20:45:36.000000 ilds-2023.4.23/ilds/lib/configobj/validate.py
--rw-rw-rw-   0        0        0       44 2019-05-06 20:45:36.000000 ilds-2023.4.23/ilds/lib/configobj/_version.py
--rw-rw-rw-   0        0        0    88030 2019-05-06 20:45:36.000000 ilds-2023.4.23/ilds/lib/configobj/__init__.py
--rw-rw-rw-   0        0        0    13829 2018-10-24 05:15:43.000000 ilds-2023.4.23/ilds/lib/hexdump.py
--rw-rw-rw-   0        0        0        0 2018-10-24 05:29:38.000000 ilds-2023.4.23/ilds/lib/__init__.py
--rw-rw-rw-   0        0        0    15494 2021-10-24 10:49:44.000000 ilds-2023.4.23/ilds/match_data.py
--rw-rw-rw-   0        0        0     7121 2019-11-18 03:49:54.000000 ilds-2023.4.23/ilds/md.py
--rw-rw-rw-   0        0        0     4832 2022-09-07 09:59:12.000000 ilds-2023.4.23/ilds/md5summer.py
--rw-rw-rw-   0        0        0     3513 2019-10-11 11:13:36.000000 ilds-2023.4.23/ilds/mycsv.py
--rw-rw-rw-   0        0        0     5123 2022-12-12 02:45:33.000000 ilds-2023.4.23/ilds/net.py
--rw-rw-rw-   0        0        0     8368 2023-04-23 03:03:14.000000 ilds-2023.4.23/ilds/pd.py
--rw-rw-rw-   0        0        0     7064 2019-09-09 02:27:39.000000 ilds-2023.4.23/ilds/spider.py
--rw-rw-rw-   0        0        0    13238 2021-03-05 07:49:55.000000 ilds-2023.4.23/ilds/time.py
--rw-rw-rw-   0        0        0     7637 2022-10-08 10:21:44.000000 ilds-2023.4.23/ilds/util.py
--rw-rw-rw-   0        0        0       23 2023-04-23 03:04:41.000000 ilds-2023.4.23/ilds/versions.py
--rw-rw-rw-   0        0        0        0 2018-07-04 06:42:08.000000 ilds-2023.4.23/ilds/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 03:05:34.000000 ilds-2023.4.23/ilds.egg-info/
--rw-rw-rw-   0        0        0        1 2023-04-23 03:05:33.000000 ilds-2023.4.23/ilds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1317 2023-04-23 03:05:33.000000 ilds-2023.4.23/ilds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       75 2023-04-23 03:05:33.000000 ilds-2023.4.23/ilds.egg-info/requires.txt
--rw-rw-rw-   0        0        0      708 2023-04-23 03:05:33.000000 ilds-2023.4.23/ilds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        5 2023-04-23 03:05:33.000000 ilds-2023.4.23/ilds.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1317 2023-04-23 03:05:34.000000 ilds-2023.4.23/PKG-INFO
--rw-rw-rw-   0        0        0      456 2019-10-24 10:28:45.000000 ilds-2023.4.23/README.rst
--rw-rw-rw-   0        0        0       42 2023-04-23 03:05:34.000000 ilds-2023.4.23/setup.cfg
--rw-rw-rw-   0        0        0     6394 2021-04-15 11:13:47.000000 ilds-2023.4.23/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-03 10:59:19.000000 ilds-2023.4.3/
+drwxrwxrwx   0        0        0        0 2023-04-03 10:59:19.000000 ilds-2023.4.3/ilds/
+-rw-rw-rw-   0        0        0     1797 2021-09-26 05:21:21.000000 ilds-2023.4.3/ilds/cmd.py
+drwxrwxrwx   0        0        0        0 2023-04-03 10:59:19.000000 ilds-2023.4.3/ilds/django/
+-rw-rw-rw-   0        0        0     3407 2019-10-30 05:10:14.000000 ilds-2023.4.3/ilds/django/admin.py
+-rw-rw-rw-   0        0        0    14906 2019-10-30 03:18:15.000000 ilds-2023.4.3/ilds/django/import_export.py
+-rw-rw-rw-   0        0        0    15417 2019-11-27 09:35:07.000000 ilds-2023.4.3/ilds/django/model.py
+-rw-rw-rw-   0        0        0     1840 2019-04-12 05:15:43.000000 ilds-2023.4.3/ilds/django/user.py
+-rw-rw-rw-   0        0        0     2085 2021-09-28 08:04:39.000000 ilds-2023.4.3/ilds/django/util.py
+-rw-rw-rw-   0        0        0        0 2018-08-07 03:24:52.000000 ilds-2023.4.3/ilds/django/__init__.py
+-rw-rw-rw-   0        0        0     9150 2021-12-06 10:18:15.000000 ilds-2023.4.3/ilds/everything.py
+-rw-rw-rw-   0        0        0     9470 2019-03-29 08:26:49.000000 ilds-2023.4.3/ilds/excel_xlrd.py
+-rw-rw-rw-   0        0        0     7970 2022-10-19 09:11:30.000000 ilds-2023.4.3/ilds/excel_xlsx.py
+-rw-rw-rw-   0        0        0    26848 2023-04-03 10:59:15.000000 ilds-2023.4.3/ilds/file.py
+-rw-rw-rw-   0        0        0     1530 2021-09-26 05:15:22.000000 ilds-2023.4.3/ilds/json.py
+drwxrwxrwx   0        0        0        0 2023-04-03 10:59:19.000000 ilds-2023.4.3/ilds/lib/
+-rw-rw-rw-   0        0        0    13740 2018-11-26 09:16:44.000000 ilds-2023.4.3/ilds/lib/browsercookie.py
+drwxrwxrwx   0        0        0        0 2023-04-03 10:59:19.000000 ilds-2023.4.3/ilds/lib/configobj/
+-rw-rw-rw-   0        0        0    46989 2019-05-06 20:45:36.000000 ilds-2023.4.3/ilds/lib/configobj/validate.py
+-rw-rw-rw-   0        0        0       44 2019-05-06 20:45:36.000000 ilds-2023.4.3/ilds/lib/configobj/_version.py
+-rw-rw-rw-   0        0        0    88030 2019-05-06 20:45:36.000000 ilds-2023.4.3/ilds/lib/configobj/__init__.py
+-rw-rw-rw-   0        0        0    13829 2018-10-24 05:15:43.000000 ilds-2023.4.3/ilds/lib/hexdump.py
+-rw-rw-rw-   0        0        0        0 2018-10-24 05:29:38.000000 ilds-2023.4.3/ilds/lib/__init__.py
+-rw-rw-rw-   0        0        0    15494 2021-10-24 10:49:44.000000 ilds-2023.4.3/ilds/match_data.py
+-rw-rw-rw-   0        0        0     7121 2019-11-18 03:49:54.000000 ilds-2023.4.3/ilds/md.py
+-rw-rw-rw-   0        0        0     4832 2022-09-07 09:59:12.000000 ilds-2023.4.3/ilds/md5summer.py
+-rw-rw-rw-   0        0        0     3513 2019-10-11 11:13:36.000000 ilds-2023.4.3/ilds/mycsv.py
+-rw-rw-rw-   0        0        0     5123 2022-12-12 02:45:33.000000 ilds-2023.4.3/ilds/net.py
+-rw-rw-rw-   0        0        0     7906 2023-04-03 10:59:05.000000 ilds-2023.4.3/ilds/pd.py
+-rw-rw-rw-   0        0        0     7064 2019-09-09 02:27:39.000000 ilds-2023.4.3/ilds/spider.py
+-rw-rw-rw-   0        0        0    13238 2021-03-05 07:49:55.000000 ilds-2023.4.3/ilds/time.py
+-rw-rw-rw-   0        0        0     7637 2022-10-08 10:21:44.000000 ilds-2023.4.3/ilds/util.py
+-rw-rw-rw-   0        0        0       22 2023-04-03 10:59:05.000000 ilds-2023.4.3/ilds/versions.py
+-rw-rw-rw-   0        0        0        0 2018-07-04 06:42:08.000000 ilds-2023.4.3/ilds/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-03 10:59:19.000000 ilds-2023.4.3/ilds.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-04-03 10:59:19.000000 ilds-2023.4.3/ilds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1316 2023-04-03 10:59:19.000000 ilds-2023.4.3/ilds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       75 2023-04-03 10:59:19.000000 ilds-2023.4.3/ilds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      708 2023-04-03 10:59:19.000000 ilds-2023.4.3/ilds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        5 2023-04-03 10:59:19.000000 ilds-2023.4.3/ilds.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1316 2023-04-03 10:59:19.000000 ilds-2023.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0      456 2019-10-24 10:28:45.000000 ilds-2023.4.3/README.rst
+-rw-rw-rw-   0        0        0       42 2023-04-03 10:59:19.000000 ilds-2023.4.3/setup.cfg
+-rw-rw-rw-   0        0        0     6394 2021-04-15 11:13:47.000000 ilds-2023.4.3/setup.py
```

### Comparing `ilds-2023.4.23/ilds/cmd.py` & `ilds-2023.4.3/ilds/cmd.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.23/ilds/django/admin.py` & `ilds-2023.4.3/ilds/django/admin.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.23/ilds/django/import_export.py` & `ilds-2023.4.3/ilds/django/import_export.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.23/ilds/django/model.py` & `ilds-2023.4.3/ilds/django/model.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.23/ilds/django/user.py` & `ilds-2023.4.3/ilds/django/user.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.23/ilds/django/util.py` & `ilds-2023.4.3/ilds/django/util.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.23/ilds/everything.py` & `ilds-2023.4.3/ilds/everything.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.23/ilds/excel_xlrd.py` & `ilds-2023.4.3/ilds/excel_xlrd.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.23/ilds/excel_xlsx.py` & `ilds-2023.4.3/ilds/excel_xlsx.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.23/ilds/file.py` & `ilds-2023.4.3/ilds/file.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.23/ilds/json.py` & `ilds-2023.4.3/ilds/json.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.23/ilds/lib/browsercookie.py` & `ilds-2023.4.3/ilds/lib/browsercookie.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.23/ilds/lib/configobj/validate.py` & `ilds-2023.4.3/ilds/lib/configobj/validate.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.23/ilds/lib/configobj/__init__.py` & `ilds-2023.4.3/ilds/lib/configobj/__init__.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.23/ilds/lib/hexdump.py` & `ilds-2023.4.3/ilds/lib/hexdump.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.23/ilds/match_data.py` & `ilds-2023.4.3/ilds/match_data.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.23/ilds/md.py` & `ilds-2023.4.3/ilds/md.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.23/ilds/md5summer.py` & `ilds-2023.4.3/ilds/md5summer.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.23/ilds/mycsv.py` & `ilds-2023.4.3/ilds/mycsv.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.23/ilds/net.py` & `ilds-2023.4.3/ilds/net.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.23/ilds/pd.py` & `ilds-2023.4.3/ilds/pd.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 import os
 from pathlib import Path
 from collections import OrderedDict
 
 from colorama import Fore, Back, Style
 
 from ilds.file import get_dir_files
-from openpyxl import load_workbook
 
 try:
     import pandas as pd
 except ImportError as e:
     print(Fore.RED + "注：导入 pandas 失败，请安装它: pip install pandas", Style.RESET_ALL)
     pass
 
@@ -72,32 +71,22 @@
     :param add_source_column: 添加内容来源
     :param only_read_first_table: 只读取第一个表格
     :param is_print: 打印读取信息
     :return: {'file_name', 'index', 'sheet_name', 'sheet_names', 'count', 'columns', 'df'}
     """
     data = OrderedDict()
 
-    try:
-        wb = load_workbook(file)
-        sheet_state_data = {name: wb[name].sheet_state for name in wb.sheetnames}
-        # print(sheet_state_data)
-        wb.close()
-    except Exception as e:
-        print('get_excel_data 错误', e)
-        sheet_state_data = {}
-
     with pd.ExcelFile(file) as excel:
         sheet_names = excel.sheet_names
         if is_print:
             print('表薄名称列表：', sheet_names)
         # 通过表薄名字读取表单
         # data['总表'] = pd.read_excel(excel, sheet_name='总表')
         # 读取全部表
         for index, sheet_name in enumerate(sheet_names):
-            sheet_state = sheet_state_data.get(sheet_name, None)
             _df = pd.read_excel(excel, sheet_name=sheet_name, header=0)
             file_name = os.path.basename(file)
             count = len(_df)
 
             if is_print:
                 print('表薄名称：', sheet_name, '\t', '行数：', count, '\t', '文件：', file)
 
@@ -109,15 +98,14 @@
                 _df = _df[columns]
 
             df_data = {
                 'file_name': file_name,
                 'index': index,
                 'sheet_name': sheet_name,
                 'sheet_names': sheet_names,
-                'sheet_state': sheet_state,
                 'count': count,
                 'columns': list(_df.columns),
                 'df': _df,
             }
 
             if only_read_first_table:
                 data = df_data
@@ -141,37 +129,36 @@
     df_list = get_df_list(file, concat_columns, add_source_column, is_print)
     count = sum([len(df) for df in df_list])
     df = pd.concat(df_list, **concat_kwargs)  # result
     print('合并数据行数：', len(df), '导入数据行数统计：', count)
     return df
 
 
-def merging_excel_file_data(file_dir_or_file_list, ext='', concat_columns=None, add_source_column=True, is_print=True,
-                            **concat_kwargs):
+def merging_excel_file_data(file_dir, ext='', concat_columns=None, add_source_column=True, is_print=True,
+                            get_files_function=None, **concat_kwargs):
     """
     合并多个 Excel 文件内容
 
-    :param file_dir_or_file_list: 合并文件的路径或者文件列表
+    :param file_dir: 合并文件的路径
     :param ext: 要合并的文件后缀名，默认是文件夹中的全部文件
     :param concat_columns: 指定要合并的列名列表
     :param add_source_column: 是否添加原始来源
     :param is_print: 打印信息
+    :param get_files_function: 支持自定义获取文件的函数
     :return:
     """
-    all_len = 0
-    frames = []
 
-    if isinstance(file_dir_or_file_list, list):
-        file_list = file_dir_or_file_list
-    else:
-        file_list = get_dir_files(file_dir_or_file_list, ext)
+    if get_files_function is None:
+        get_files_function = get_dir_files
 
-    for file in file_list:
+    all_len = 0
+    frames = []
+    for file in get_files_function(file_dir, ext):
         if is_print:
-            print('处理文件:', file)
+            print(file)
         df_list = get_df_list(file, concat_columns, add_source_column, is_print)
         all_len += sum([len(df) for df in df_list])
         frames.extend(df_list)
 
     _df = pd.concat(frames, **concat_kwargs)  # result
     if is_print:
         print('合并数据行数：', len(_df), '原始数据行数：', all_len)
```

### Comparing `ilds-2023.4.23/ilds/spider.py` & `ilds-2023.4.3/ilds/spider.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.23/ilds/time.py` & `ilds-2023.4.3/ilds/time.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.23/ilds/util.py` & `ilds-2023.4.3/ilds/util.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.23/ilds.egg-info/PKG-INFO` & `ilds-2023.4.3/ilds.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ilds
-Version: 2023.4.23
+Version: 2023.4.3
 Summary: 常用模块的集合，为了多平台，多电脑调用方便!
 Home-page: https://github.com/ldsxp/ilds
 Author: lds
 Author-email: 85176878@qq.com
 License: GNU GPL 3
 Download-URL: https://pypi.org/project/ilds
 Description: ====================
```

### Comparing `ilds-2023.4.23/ilds.egg-info/SOURCES.txt` & `ilds-2023.4.3/ilds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.23/PKG-INFO` & `ilds-2023.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ilds
-Version: 2023.4.23
+Version: 2023.4.3
 Summary: 常用模块的集合，为了多平台，多电脑调用方便!
 Home-page: https://github.com/ldsxp/ilds
 Author: lds
 Author-email: 85176878@qq.com
 License: GNU GPL 3
 Download-URL: https://pypi.org/project/ilds
 Description: ====================
```

### Comparing `ilds-2023.4.23/setup.py` & `ilds-2023.4.3/setup.py`

 * *Files identical despite different names*

