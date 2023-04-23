# Comparing `tmp/python-sdk-bitable-0.0.9.tar.gz` & `tmp/python-sdk-bitable-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-sdk-bitable-0.0.9.tar", last modified: Tue Nov  1 09:52:50 2022, max compression
+gzip compressed data, was "python-sdk-bitable-0.1.0.tar", last modified: Sun Apr 23 09:47:22 2023, max compression
```

## Comparing `python-sdk-bitable-0.0.9.tar` & `python-sdk-bitable-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 nge6uu     (501) staff       (20)        0 2022-11-01 09:52:50.865430 python-sdk-bitable-0.0.9/
--rw-r--r--   0 nge6uu     (501) staff       (20)     1068 2022-07-19 08:41:05.000000 python-sdk-bitable-0.0.9/LICENSE
--rw-r--r--   0 nge6uu     (501) staff       (20)       26 2022-07-19 08:43:02.000000 python-sdk-bitable-0.0.9/MANIFEST.in
--rw-r--r--   0 nge6uu     (501) staff       (20)     1542 2022-11-01 09:52:50.865213 python-sdk-bitable-0.0.9/PKG-INFO
--rw-r--r--   0 nge6uu     (501) staff       (20)      885 2022-07-19 09:35:43.000000 python-sdk-bitable-0.0.9/README.md
-drwxr-xr-x   0 nge6uu     (501) staff       (20)        0 2022-11-01 09:52:50.863498 python-sdk-bitable-0.0.9/bitable/
--rw-r--r--   0 nge6uu     (501) staff       (20)       71 2022-07-22 07:02:52.000000 python-sdk-bitable-0.0.9/bitable/__init__.py
--rw-r--r--   0 nge6uu     (501) staff       (20)      352 2022-07-22 06:55:00.000000 python-sdk-bitable-0.0.9/bitable/__version__.py
--rw-r--r--   0 nge6uu     (501) staff       (20)     1358 2022-07-19 09:44:51.000000 python-sdk-bitable-0.0.9/bitable/auth.py
--rw-r--r--   0 nge6uu     (501) staff       (20)    15450 2022-11-01 09:52:02.000000 python-sdk-bitable-0.0.9/bitable/bitable.py
--rw-r--r--   0 nge6uu     (501) staff       (20)     8106 2022-07-22 07:09:28.000000 python-sdk-bitable-0.0.9/bitable/contact.py
--rw-r--r--   0 nge6uu     (501) staff       (20)    10342 2022-07-18 09:59:56.000000 python-sdk-bitable-0.0.9/bitable/params.py
--rw-r--r--   0 nge6uu     (501) staff       (20)     5187 2022-07-25 07:33:25.000000 python-sdk-bitable-0.0.9/bitable/spreadsheets.py
-drwxr-xr-x   0 nge6uu     (501) staff       (20)        0 2022-11-01 09:52:50.864810 python-sdk-bitable-0.0.9/python_sdk_bitable.egg-info/
--rw-r--r--   0 nge6uu     (501) staff       (20)     1542 2022-11-01 09:52:50.000000 python-sdk-bitable-0.0.9/python_sdk_bitable.egg-info/PKG-INFO
--rw-r--r--   0 nge6uu     (501) staff       (20)      386 2022-11-01 09:52:50.000000 python-sdk-bitable-0.0.9/python_sdk_bitable.egg-info/SOURCES.txt
--rw-r--r--   0 nge6uu     (501) staff       (20)        1 2022-11-01 09:52:50.000000 python-sdk-bitable-0.0.9/python_sdk_bitable.egg-info/dependency_links.txt
--rw-r--r--   0 nge6uu     (501) staff       (20)        9 2022-11-01 09:52:50.000000 python-sdk-bitable-0.0.9/python_sdk_bitable.egg-info/requires.txt
--rw-r--r--   0 nge6uu     (501) staff       (20)        8 2022-11-01 09:52:50.000000 python-sdk-bitable-0.0.9/python_sdk_bitable.egg-info/top_level.txt
--rw-r--r--   0 nge6uu     (501) staff       (20)       38 2022-11-01 09:52:50.865474 python-sdk-bitable-0.0.9/setup.cfg
--rw-r--r--   0 nge6uu     (501) staff       (20)     3768 2022-11-01 09:52:02.000000 python-sdk-bitable-0.0.9/setup.py
+drwxr-xr-x   0 nge6uu     (501) staff       (20)        0 2023-04-23 09:47:22.032282 python-sdk-bitable-0.1.0/
+-rw-r--r--   0 nge6uu     (501) staff       (20)     1068 2022-07-19 08:41:05.000000 python-sdk-bitable-0.1.0/LICENSE
+-rw-r--r--   0 nge6uu     (501) staff       (20)       26 2022-07-19 08:43:02.000000 python-sdk-bitable-0.1.0/MANIFEST.in
+-rw-r--r--   0 nge6uu     (501) staff       (20)     1542 2023-04-23 09:47:22.032085 python-sdk-bitable-0.1.0/PKG-INFO
+-rw-r--r--   0 nge6uu     (501) staff       (20)      885 2022-07-19 09:35:43.000000 python-sdk-bitable-0.1.0/README.md
+drwxr-xr-x   0 nge6uu     (501) staff       (20)        0 2023-04-23 09:47:22.029784 python-sdk-bitable-0.1.0/bitable/
+-rw-r--r--   0 nge6uu     (501) staff       (20)       71 2022-07-22 07:02:52.000000 python-sdk-bitable-0.1.0/bitable/__init__.py
+-rw-r--r--   0 nge6uu     (501) staff       (20)      352 2022-07-22 06:55:00.000000 python-sdk-bitable-0.1.0/bitable/__version__.py
+-rw-r--r--   0 nge6uu     (501) staff       (20)     1358 2022-07-19 09:44:51.000000 python-sdk-bitable-0.1.0/bitable/auth.py
+-rw-r--r--   0 nge6uu     (501) staff       (20)    15657 2023-04-23 09:45:01.000000 python-sdk-bitable-0.1.0/bitable/bitable.py
+-rw-r--r--   0 nge6uu     (501) staff       (20)     8106 2022-07-22 07:09:28.000000 python-sdk-bitable-0.1.0/bitable/contact.py
+-rw-r--r--   0 nge6uu     (501) staff       (20)     3428 2023-01-12 08:10:26.000000 python-sdk-bitable-0.1.0/bitable/document.py
+-rw-r--r--   0 nge6uu     (501) staff       (20)    10342 2022-07-18 09:59:56.000000 python-sdk-bitable-0.1.0/bitable/params.py
+-rw-r--r--   0 nge6uu     (501) staff       (20)     5187 2022-07-25 07:33:25.000000 python-sdk-bitable-0.1.0/bitable/spreadsheets.py
+drwxr-xr-x   0 nge6uu     (501) staff       (20)        0 2023-04-23 09:47:22.031824 python-sdk-bitable-0.1.0/python_sdk_bitable.egg-info/
+-rw-r--r--   0 nge6uu     (501) staff       (20)     1542 2023-04-23 09:47:21.000000 python-sdk-bitable-0.1.0/python_sdk_bitable.egg-info/PKG-INFO
+-rw-r--r--   0 nge6uu     (501) staff       (20)      406 2023-04-23 09:47:21.000000 python-sdk-bitable-0.1.0/python_sdk_bitable.egg-info/SOURCES.txt
+-rw-r--r--   0 nge6uu     (501) staff       (20)        1 2023-04-23 09:47:21.000000 python-sdk-bitable-0.1.0/python_sdk_bitable.egg-info/dependency_links.txt
+-rw-r--r--   0 nge6uu     (501) staff       (20)        9 2023-04-23 09:47:21.000000 python-sdk-bitable-0.1.0/python_sdk_bitable.egg-info/requires.txt
+-rw-r--r--   0 nge6uu     (501) staff       (20)        8 2023-04-23 09:47:21.000000 python-sdk-bitable-0.1.0/python_sdk_bitable.egg-info/top_level.txt
+-rw-r--r--   0 nge6uu     (501) staff       (20)       38 2023-04-23 09:47:22.032326 python-sdk-bitable-0.1.0/setup.cfg
+-rw-r--r--   0 nge6uu     (501) staff       (20)     3768 2023-04-23 09:45:26.000000 python-sdk-bitable-0.1.0/setup.py
```

### Comparing `python-sdk-bitable-0.0.9/LICENSE` & `python-sdk-bitable-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-sdk-bitable-0.0.9/PKG-INFO` & `python-sdk-bitable-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sdk-bitable
-Version: 0.0.9
+Version: 0.1.0
 Summary: Python sdk for 飞书多维表格
 Home-page: https://github.com/me/myproject
 Author: liushengyi
 Author-email: liuwenxuan123@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `python-sdk-bitable-0.0.9/README.md` & `python-sdk-bitable-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `python-sdk-bitable-0.0.9/bitable/auth.py` & `python-sdk-bitable-0.1.0/bitable/auth.py`

 * *Files identical despite different names*

### Comparing `python-sdk-bitable-0.0.9/bitable/bitable.py` & `python-sdk-bitable-0.1.0/bitable/bitable.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import requests
 import posixpath
 import time
 from collections import OrderedDict
-from .params import BitableParams
-from .auth import FeiShuAuth
+from params import BitableParams
+from auth import FeiShuAuth
 
 
 class BITable:
     VERSION = "v1"
     API_BASE_URL = "https://open.feishu.cn/open-apis/bitable/"
     API_LIMIT = 1.0 / 5  # 5 per second
     API_URL = posixpath.join(API_BASE_URL, VERSION, "apps")
@@ -294,14 +294,16 @@
         """
         inserted_records = []
         for chunk in self._chunk(records, self.MAX_RECORDS_PER_REQUEST):
             new_records = self._build_batch_record_objects(chunk)
             response = self._post(
                 self.url_table + "/records/batch_create", json_data={"records": new_records}
             )
+            if response.get("error"):
+                raise ValueError(response.get("error"))
             inserted_records += response["data"]["records"]
             time.sleep(self.API_LIMIT)
         return inserted_records
 
     def update(self, record_id, fields):
         """
         Updates a record by its record id.
@@ -337,14 +339,16 @@
         """
         updated_records = []
         for chunk in self._chunk(records, self.MAX_RECORDS_PER_REQUEST):
             chunk_records = [{"id": x["id"], "fields": x["fields"]} for x in chunk]
             response = self._post(
                 self.url_table + "/records/batch_update", json_data={"records": chunk_records}
             )
+            if response.get("error"):
+                raise ValueError(response.get("error"))
             updated_records += response["data"]["records"]
         #
         return updated_records
 
     def update_by_field(self, field_name, field_value, fields, **options):
         """
         Updates the first record to match field name and value.
@@ -436,12 +440,12 @@
 
 
 def main():
     table = BITable(app_id='',
                     app_secret='',
                     base_id='bascnTIHCOcDLuXxhx89Z7lUwoc',
                     table_id='tblqKf7lzTKsGhkj')
-    table_data = table.list_records()
+    # table_data = table.insert({"合同编号1":1231232})
     # print(table_data)
 
 if __name__ == '__main__':
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `python-sdk-bitable-0.0.9/bitable/contact.py` & `python-sdk-bitable-0.1.0/bitable/contact.py`

 * *Files identical despite different names*

### Comparing `python-sdk-bitable-0.0.9/bitable/params.py` & `python-sdk-bitable-0.1.0/bitable/params.py`

 * *Files identical despite different names*

### Comparing `python-sdk-bitable-0.0.9/bitable/spreadsheets.py` & `python-sdk-bitable-0.1.0/bitable/spreadsheets.py`

 * *Files identical despite different names*

### Comparing `python-sdk-bitable-0.0.9/python_sdk_bitable.egg-info/PKG-INFO` & `python-sdk-bitable-0.1.0/python_sdk_bitable.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sdk-bitable
-Version: 0.0.9
+Version: 0.1.0
 Summary: Python sdk for 飞书多维表格
 Home-page: https://github.com/me/myproject
 Author: liushengyi
 Author-email: liuwenxuan123@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `python-sdk-bitable-0.0.9/setup.py` & `python-sdk-bitable-0.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'python-sdk-bitable'
 DESCRIPTION = 'Python sdk for 飞书多维表格'
 URL = 'https://github.com/me/myproject'
 EMAIL = 'liuwenxuan123@qq.com'
 AUTHOR = 'liushengyi'
 REQUIRES_PYTHON = '>=3.6.5'
-VERSION = '0.0.9'
+VERSION = '0.1.0'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'requests'
 ]
 
 # What packages are optional?
```

