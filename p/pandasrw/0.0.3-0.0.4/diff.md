# Comparing `tmp/pandasrw-0.0.3.tar.gz` & `tmp/pandasrw-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasrw-0.0.3.tar", last modified: Wed Apr  5 09:47:24 2023, max compression
+gzip compressed data, was "pandasrw-0.0.4.tar", last modified: Sun Apr 23 06:51:25 2023, max compression
```

## Comparing `pandasrw-0.0.3.tar` & `pandasrw-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-04-05 09:47:24.612158 pandasrw-0.0.3/
--rw-rw-rw-   0        0        0      401 2023-04-05 09:47:24.607158 pandasrw-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-05 09:47:24.602158 pandasrw-0.0.3/pandasrw.egg-info/
--rw-rw-rw-   0        0        0      401 2023-04-05 09:47:24.000000 pandasrw-0.0.3/pandasrw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      163 2023-04-05 09:47:24.000000 pandasrw-0.0.3/pandasrw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-05 09:47:24.000000 pandasrw-0.0.3/pandasrw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-05 09:47:24.000000 pandasrw-0.0.3/pandasrw.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7214 2023-04-05 09:09:54.000000 pandasrw-0.0.3/pandasrw.py
--rw-rw-rw-   0        0        0      484 2023-03-29 01:24:37.000000 pandasrw-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-05 09:47:24.612158 pandasrw-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      859 2023-04-05 09:47:12.000000 pandasrw-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:51:25.938775 pandasrw-0.0.4/
+-rw-rw-rw-   0        0        0      503 2023-04-23 06:51:25.938775 pandasrw-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-23 06:51:25.937780 pandasrw-0.0.4/pandasrw.egg-info/
+-rw-rw-rw-   0        0        0      503 2023-04-23 06:51:25.000000 pandasrw-0.0.4/pandasrw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      163 2023-04-23 06:51:25.000000 pandasrw-0.0.4/pandasrw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 06:51:25.000000 pandasrw-0.0.4/pandasrw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-23 06:51:25.000000 pandasrw-0.0.4/pandasrw.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     8607 2023-04-23 06:41:45.000000 pandasrw-0.0.4/pandasrw.py
+-rw-rw-rw-   0        0        0      484 2023-04-23 06:49:51.000000 pandasrw-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-23 06:51:25.938775 pandasrw-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      776 2023-04-23 06:46:18.000000 pandasrw-0.0.4/setup.py
```

### Comparing `pandasrw-0.0.3/pandasrw.py` & `pandasrw-0.0.4/pandasrw.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,60 @@
+"""
+v0.0.1第一个版本
+v0.0.2
+修改了polar引擎，在read_csv_options中增加了{"infer_schema_length":1000,"ignore_errors":False})两个配置，性能进一步提升，特殊情况下兼容性降低，
+可以采用pandas引擎弥补（之前需要对文件读两次完成类型推断，一次类型推断，一次读文件。当前只对前1000行读进行内容推断）。
+v0.0.3
+更新openpyxl引擎写的load_excel函数，比pandas引擎快20%，兼容性基本一致。该函数可以支持部分行读取。
+polars引擎增加了read_csv_options选项，目前默认关闭。打开后使用者可以自己设置各类参数，主要是{"infer_schema_length":1000,"ignore_errors":False} 该参数影响类型推断的精度和速度。
+polars引擎读取excel表后默认删除全部值为空的行和列。
+v0.0.4
+xlwings引擎增加类型转换
+load函数增加错误提示
+"""
 import os
 import pandas as pd
 import polars as pl
 import xlwings as xw
 from xlsx2csv import Xlsx2csv
 from openpyxl import load_workbook
 from chardet.universaldetector import UniversalDetector
 
-#将csv转化为utf8编码
+
+# 将csv转化为utf8编码
 def encode_to_utf8(filename, des_encode):
     # 读取文件的编码方式
     with open(filename, 'rb') as f:
         detector = UniversalDetector()
         for line in f.readlines():
             detector.feed(line)
             if detector.done:
                 break
         original_encode = detector.result['encoding']
     # 读取文件的内容
     with open(filename, 'rb') as f:
         file_content = f.read()
-    #修改编码
+    # 修改编码
     file_decode = file_content.decode(original_encode, 'ignore')
     file_encode = file_decode.encode(des_encode)
     with open(filename, 'wb') as f:
         f.write(file_encode)
 
 
-#通过xlwings读取表
+# 通过xlwings读取表
 def xw_open(file_path, sheetname='Sheet1', visible=False):
-    #数据类型可能推断不正确。测试时发现可以正确区分object和数据类型，但是数据类型都推断为float64不能区分int64
+    # 数据类型可能推断不正确。测试时发现可以正确区分object和数据类型，但是数据类型都推断为float64不能区分int64
     app = xw.App(visible=visible,
                  add_book=False)
 
     book = app.books.open(file_path)
 
     sheet = book.sheets[sheetname]
     data = sheet.used_range.options(pd.DataFrame, header=1, index=False, expand='table').value
-
+    data = data.convert_dtypes()
     if visible == False:
         book.close()
         app.quit()
 
     return data
 
 
@@ -60,104 +74,109 @@
     sheet.range('A1').value = df
     # 保存并关闭Workbook
     wb.save(file_path)
     if visible == False:
         wb.close()
         app.quit()
 
-#xlsx转换为csv
+
+# xlsx转换为csv
 def xlsxtocsv(file_path):
-    file_path_csv=file_path.replace(".xlsx", ".csv")
+    file_path_csv = file_path.replace(".xlsx", ".csv")
     Xlsx2csv(file_path, outputencoding="utf-8").convert(file_path_csv)
     return file_path_csv
 
 
-#自适用后缀、多引擎读取表，默认为polars
-def load(file_path, col_name=None,sheetname='Sheet1',engine="polars",read_csv_options=None):
-
+# 自适用后缀、多引擎读取表，默认为polars
+def load(file_path, col_name=None, sheetname='Sheet1', engine="polars", read_csv_options=None):
     name, ext = os.path.splitext(file_path)
+    try:
+        if '.csv' == ext:
+            if engine == "polars":
+                encode_to_utf8(file_path, des_encode="utf-8")
+                df_read = pl.read_csv(file_path, columns=col_name)
+                df_read = df_read.to_pandas()
+            if engine == "pandas":
+                encode_to_utf8(file_path, des_encode="utf-8")
+                df_read = pd.read_csv(file_path, usecols=col_name)
+            if engine == "xlwings":
+                # xlwings读取csv兼容性和效率都较差调用pandas读取
+                encode_to_utf8(file_path, des_encode="utf-8")
+                df_read = pd.read_csv(file_path, usecols=col_name)
+
+        if ".xlsx" == ext:
+            if engine == "polars":
+                df_read = pl.read_excel(file_path,
+                                        read_csv_options=read_csv_options,
+                                        sheet_name=sheetname)
+                # 删除所有空行
+                df_read = df_read.filter(~pl.all(pl.all().is_null()))
+                df_read = df_read[[s.name for s in df_read if not (s.null_count() == df_read.height)]]
+                df_read = df_read.to_pandas()
+            if engine == "pandas":
+                df_read = pd.read_excel(file_path, usecols=col_name, sheet_name=sheetname)
+            if engine == "xlwings":
+                df_read = xw_open(file_path, sheetname=sheetname, visible=False)
+
+        if ".xls" == ext:
+            if engine == "polars":
+                # polars不能读xls格式，调用pandas解决
+                df_read = pd.read_excel(file_path, usecols=col_name, sheet_name=sheetname)
+            if engine == "pandas":
+                df_read = pd.read_excel(file_path, usecols=col_name, sheet_name=sheetname)
+            if engine == "xlwings":
+                df_read = xw_open(file_path, sheetname=sheetname, visible=False)
+
+        if ".pkl" == ext:
+            df_read = pd.read_pickle(file_path)
+
+        return df_read
+
+    except Exception as e:
+        print(f"读取文件发生错误：{e}")
+        print(
+            f'请使用兼容性更好的pandas引擎，语法为load(file_path, engine="pandas")，对于大文件尝试使用engine="xlwings"。')
 
-    if '.csv' == ext:
-        if engine=="polars":
-            encode_to_utf8(file_path, des_encode="utf-8")
-            df_read = pl.read_csv(file_path, columns=col_name)
-            df_read = df_read.to_pandas()
-        if engine=="pandas":
-            encode_to_utf8(file_path, des_encode="utf-8")
-            df_read = pd.read_csv(file_path, usecols=col_name)
-        if engine == "xlwings":
-            #xlwings读取csv兼容性和效率都较差调用pandas读取
-            encode_to_utf8(file_path, des_encode="utf-8")
-            df_read = pd.read_csv(file_path, usecols=col_name)
-
-    if ".xlsx" == ext:
-        if engine == "polars":
-            df_read = pl.read_excel(file_path,
-                                    read_csv_options=read_csv_options,
-                                    sheet_name=sheetname)
-            #删除所有空行
-            df_read = df_read.filter(~pl.all(pl.all().is_null()))
-            df_read =df_read[[s.name for s in df_read if not (s.null_count() == df_read.height)]]
-            df_read = df_read.to_pandas()
-        if engine == "pandas":
-            df_read = pd.read_excel(file_path, usecols=col_name, sheet_name=sheetname)
-        if engine == "xlwings":
-            df_read = xw_open(file_path, sheetname=sheetname, visible=False)
-
-    if ".xls" == ext:
-        if engine == "polars":
-            #polars不能读xls格式，调用pandas解决
-            df_read = pd.read_excel(file_path, usecols=col_name, sheet_name=sheetname)
-        if engine == "pandas":
-            df_read = pd.read_excel(file_path, usecols=col_name, sheet_name=sheetname)
-        if engine == "xlwings":
-            df_read = xw_open(file_path, sheetname=sheetname, visible=False)
-
-    if ".pkl" == ext:
-        df_read=pd.read_pickle(file_path)
-
-    return df_read
 
-
-#自适应后缀、多引擎写入表,默认为polars
-def dump(df,file_path,sheetname='Sheet1',engine="polars"):
+# 自适应后缀、多引擎写入表,默认为polars
+def dump(df, file_path, sheetname='Sheet1', engine="polars"):
     name, ext = os.path.splitext(file_path)
-    if '.csv' ==ext:
+    if '.csv' == ext:
         if engine == "polars":
-            df=pl.from_pandas(df)
+            df = pl.from_pandas(df)
             df.write_csv(file_path, separator=",")
         if engine == "pandas":
-            df.to_csv(file_path,index=False)
+            df.to_csv(file_path, index=False)
         if engine == "xlwings":
-            #xlwings不能写入csv，调用pandas写入
-            df.to_csv(file_path,index=False)
+            # xlwings不能写入csv，调用pandas写入
+            df.to_csv(file_path, index=False)
 
     if ".xlsx" == ext:
         if engine == "polars":
-            df=pl.from_pandas(df)
+            df = pl.from_pandas(df)
             df.write_excel(file_path, worksheet=sheetname)
         if engine == "pandas":
-            df.to_excel(file_path, index=False,sheet_name=sheetname)
+            df.to_excel(file_path, index=False, sheet_name=sheetname)
         if engine == "xlwings":
             xw_write(df, file_path, sheetname=sheetname, visible=False)
 
     if ".xls" == ext:
         if engine == "polars":
-            df.to_excel(file_path, index=False,sheet_name=sheetname)
+            df.to_excel(file_path, index=False, sheet_name=sheetname)
         if engine == "pandas":
-            df.to_excel(file_path, index=False,sheet_name=sheetname)
+            df.to_excel(file_path, index=False, sheet_name=sheetname)
         if engine == "xlwings":
             xw_write(df, file_path, sheetname=sheetname, visible=False)
 
     if ".pkl" == ext:
         df.to_pickle(file_path)
 
-#row_count每次读取的行数
-def load_stream_row(file_path, row_count,col_name=None):
 
+# row_count每次读取的行数
+def load_stream_row(file_path, row_count, col_name=None):
     name, ext = os.path.splitext(file_path)
     if '.csv' == ext:
         encode_to_utf8(file_path, des_encode="utf-8")
         df_read = pd.read_csv(file_path, usecols=col_name, chunksize=row_count)
     if ".xls" == ext:
         df_read = pd.read_excel(file_path, usecols=col_name)
         # 转化为csv再分块读
@@ -166,23 +185,24 @@
         # encode_to_utf8(file_path_csv, des_encode="utf-8")
         df_read = pd.read_csv(file_path_csv, usecols=col_name, chunksize=row_count)
     if ".xlsx" == ext:
         file_path_csv = xlsxtocsv(file_path)
         df_read = pd.read_csv(file_path_csv, usecols=col_name, chunksize=row_count)
     return df_read
 
-#第一行是列名，从第二行开始读内容
-def load_excel(file_path,sheetname='Sheet1',start_row=2,end_row=None):
-    lst=[]
+
+# 第一行是列名，从第二行开始读内容
+def load_excel(file_path, sheetname='Sheet1', start_row=2, end_row=None):
+    lst = []
     wb = load_workbook(filename=file_path, read_only=True)
     ws = wb[sheetname]
-    max_row=ws.max_row
-    #[*迭代器]方法性能高于list(迭代器)和逐行取值的方法
+    max_row = ws.max_row
+    # [*迭代器]方法性能高于list(迭代器)和逐行取值的方法
     row_columns = [*ws.iter_rows(min_row=1, max_row=1, values_only=True)]
-    if end_row !=None:
+    if end_row != None:
         row_data = [*ws.iter_rows(min_row=start_row, max_row=end_row, values_only=True)]
     else:
         row_data = [*ws.iter_rows(min_row=start_row, max_row=max_row, values_only=True)]
-    #将列名和数据合并
+    # 将列名和数据合并
     row_columns.extend(row_data)
-    df=pd.DataFrame(row_columns)
+    df = pd.DataFrame(row_columns)
     return df
```

### Comparing `pandasrw-0.0.3/setup.py` & `pandasrw-0.0.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 from setuptools import setup
 
-with open("readme.md","r",encoding="utf-8") as f:
-    long_description=f.read()
 
 setup(
     name='pandasrw',# 需要打包的名字,即本模块要发布的名字
-    version='0.0.3',#版本
+    version='0.0.4',#版本
     description='A pandas IO library for efficiently load and dump excel、csv、pkl', # 简要描述
     py_modules=['pandasrw'],   #  需要打包的模块
     author='storm', # 作者名
-    #long_description="pandasrw提升了pandas读写excel、csv、pickle文件的性能和易用性。https://github.com/stormtozero/pandasio",
+    long_description="pandasrw提升了pandas读写excel、csv、pickle文件的性能和易用性。https://github.com/stormtozero/pandasio",
     author_email='41915460@163.com',   # 作者邮件
     url='https://github.com/stormtozero/pandasrw', # 项目地址,一般是代码托管的网站
     requires=['pandas','polars','xlwings','chardet','xlsx2csv',"openpyxl"], # 依赖包,如果没有,可以不要
     license='MIT'
 )
```

