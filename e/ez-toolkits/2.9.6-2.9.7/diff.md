# Comparing `tmp/ez-toolkits-2.9.6.tar.gz` & `tmp/ez-toolkits-2.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ez-toolkits-2.9.6.tar", last modified: Tue Jan 31 09:42:58 2023, max compression
+gzip compressed data, was "ez-toolkits-2.9.7.tar", last modified: Wed Feb  1 03:09:01 2023, max compression
```

## Comparing `ez-toolkits-2.9.6.tar` & `ez-toolkits-2.9.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 admin      (502) staff       (20)        0 2023-01-31 09:42:58.981224 ez-toolkits-2.9.6/
--rw-r--r--   0 admin      (502) staff       (20)    35149 2022-05-31 10:26:14.000000 ez-toolkits-2.9.6/LICENSE
--rw-r--r--   0 admin      (502) staff       (20)       13 2022-05-31 10:26:14.000000 ez-toolkits-2.9.6/MANIFEST.in
--rw-r--r--   0 admin      (502) staff       (20)      174 2023-01-31 09:42:58.980728 ez-toolkits-2.9.6/PKG-INFO
--rw-r--r--   0 admin      (502) staff       (20)     1952 2023-01-29 11:22:41.000000 ez-toolkits-2.9.6/README.md
-drwxr-xr-x   0 admin      (502) staff       (20)        0 2023-01-31 09:42:58.967975 ez-toolkits-2.9.6/ez_toolkits.egg-info/
--rw-r--r--   0 admin      (502) staff       (20)      174 2023-01-31 09:42:58.000000 ez-toolkits-2.9.6/ez_toolkits.egg-info/PKG-INFO
--rw-r--r--   0 admin      (502) staff       (20)      441 2023-01-31 09:42:58.000000 ez-toolkits-2.9.6/ez_toolkits.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (502) staff       (20)        1 2023-01-31 09:42:58.000000 ez-toolkits-2.9.6/ez_toolkits.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (502) staff       (20)       14 2023-01-31 09:42:58.000000 ez-toolkits-2.9.6/ez_toolkits.egg-info/requires.txt
--rw-r--r--   0 admin      (502) staff       (20)        9 2023-01-31 09:42:58.000000 ez-toolkits-2.9.6/ez_toolkits.egg-info/top_level.txt
--rw-r--r--   0 admin      (502) staff       (20)       38 2023-01-31 09:42:58.981401 ez-toolkits-2.9.6/setup.cfg
--rw-r--r--   0 admin      (502) staff       (20)      367 2023-01-31 09:41:07.000000 ez-toolkits-2.9.6/setup.py
-drwxr-xr-x   0 admin      (502) staff       (20)        0 2023-01-31 09:42:58.979414 ez-toolkits-2.9.6/toolkits/
--rw-r--r--   0 admin      (502) staff       (20)       70 2022-12-15 02:24:35.000000 ez-toolkits-2.9.6/toolkits/__init__.py
--rw-r--r--   0 admin      (502) staff       (20)   151840 2023-01-23 14:24:50.000000 ez-toolkits-2.9.6/toolkits/bottle.py
--rw-r--r--   0 admin      (502) staff       (20)     6098 2023-01-31 09:42:09.000000 ez-toolkits-2.9.6/toolkits/database.py
--rw-r--r--   0 admin      (502) staff       (20)    12710 2023-01-26 16:32:02.000000 ez-toolkits-2.9.6/toolkits/files.py
--rw-r--r--   0 admin      (502) staff       (20)     1589 2023-01-29 03:42:18.000000 ez-toolkits-2.9.6/toolkits/mongo.py
--rw-r--r--   0 admin      (502) staff       (20)     5322 2023-01-02 09:30:51.000000 ez-toolkits-2.9.6/toolkits/plots.py
--rw-r--r--   0 admin      (502) staff       (20)     8895 2023-01-26 16:32:19.000000 ez-toolkits-2.9.6/toolkits/reports.py
--rw-r--r--   0 admin      (502) staff       (20)     4625 2023-01-29 11:19:37.000000 ez-toolkits-2.9.6/toolkits/sendmail.py
--rw-r--r--   0 admin      (502) staff       (20)    24857 2023-01-29 11:22:52.000000 ez-toolkits-2.9.6/toolkits/utils.py
--rw-r--r--   0 admin      (502) staff       (20)     5075 2023-01-26 16:39:45.000000 ez-toolkits-2.9.6/toolkits/weixin.py
--rw-r--r--   0 admin      (502) staff       (20)     6982 2023-01-26 16:33:26.000000 ez-toolkits-2.9.6/toolkits/xftp.py
--rw-r--r--   0 admin      (502) staff       (20)    28996 2023-01-27 08:25:23.000000 ez-toolkits-2.9.6/toolkits/zabbix.py
+drwxr-xr-x   0 admin      (502) staff       (20)        0 2023-02-01 03:09:01.633237 ez-toolkits-2.9.7/
+-rw-r--r--   0 admin      (502) staff       (20)    35149 2022-05-31 10:26:14.000000 ez-toolkits-2.9.7/LICENSE
+-rw-r--r--   0 admin      (502) staff       (20)       13 2022-05-31 10:26:14.000000 ez-toolkits-2.9.7/MANIFEST.in
+-rw-r--r--   0 admin      (502) staff       (20)      174 2023-02-01 03:09:01.632885 ez-toolkits-2.9.7/PKG-INFO
+-rw-r--r--   0 admin      (502) staff       (20)     1952 2023-01-29 11:22:41.000000 ez-toolkits-2.9.7/README.md
+drwxr-xr-x   0 admin      (502) staff       (20)        0 2023-02-01 03:09:01.619753 ez-toolkits-2.9.7/ez_toolkits.egg-info/
+-rw-r--r--   0 admin      (502) staff       (20)      174 2023-02-01 03:09:01.000000 ez-toolkits-2.9.7/ez_toolkits.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (502) staff       (20)      441 2023-02-01 03:09:01.000000 ez-toolkits-2.9.7/ez_toolkits.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (502) staff       (20)        1 2023-02-01 03:09:01.000000 ez-toolkits-2.9.7/ez_toolkits.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (502) staff       (20)       14 2023-02-01 03:09:01.000000 ez-toolkits-2.9.7/ez_toolkits.egg-info/requires.txt
+-rw-r--r--   0 admin      (502) staff       (20)        9 2023-02-01 03:09:01.000000 ez-toolkits-2.9.7/ez_toolkits.egg-info/top_level.txt
+-rw-r--r--   0 admin      (502) staff       (20)       38 2023-02-01 03:09:01.633337 ez-toolkits-2.9.7/setup.cfg
+-rw-r--r--   0 admin      (502) staff       (20)      367 2023-02-01 03:07:16.000000 ez-toolkits-2.9.7/setup.py
+drwxr-xr-x   0 admin      (502) staff       (20)        0 2023-02-01 03:09:01.631736 ez-toolkits-2.9.7/toolkits/
+-rw-r--r--   0 admin      (502) staff       (20)       70 2022-12-15 02:24:35.000000 ez-toolkits-2.9.7/toolkits/__init__.py
+-rw-r--r--   0 admin      (502) staff       (20)   151840 2023-01-23 14:24:50.000000 ez-toolkits-2.9.7/toolkits/bottle.py
+-rw-r--r--   0 admin      (502) staff       (20)     6158 2023-02-01 03:04:42.000000 ez-toolkits-2.9.7/toolkits/database.py
+-rw-r--r--   0 admin      (502) staff       (20)    12710 2023-01-26 16:32:02.000000 ez-toolkits-2.9.7/toolkits/files.py
+-rw-r--r--   0 admin      (502) staff       (20)     1589 2023-01-29 03:42:18.000000 ez-toolkits-2.9.7/toolkits/mongo.py
+-rw-r--r--   0 admin      (502) staff       (20)     5322 2023-01-02 09:30:51.000000 ez-toolkits-2.9.7/toolkits/plots.py
+-rw-r--r--   0 admin      (502) staff       (20)     8895 2023-01-26 16:32:19.000000 ez-toolkits-2.9.7/toolkits/reports.py
+-rw-r--r--   0 admin      (502) staff       (20)     4625 2023-01-29 11:19:37.000000 ez-toolkits-2.9.7/toolkits/sendmail.py
+-rw-r--r--   0 admin      (502) staff       (20)    24857 2023-01-29 11:22:52.000000 ez-toolkits-2.9.7/toolkits/utils.py
+-rw-r--r--   0 admin      (502) staff       (20)     5075 2023-01-26 16:39:45.000000 ez-toolkits-2.9.7/toolkits/weixin.py
+-rw-r--r--   0 admin      (502) staff       (20)     6982 2023-01-26 16:33:26.000000 ez-toolkits-2.9.7/toolkits/xftp.py
+-rw-r--r--   0 admin      (502) staff       (20)    28996 2023-01-27 08:25:23.000000 ez-toolkits-2.9.7/toolkits/zabbix.py
```

### Comparing `ez-toolkits-2.9.6/LICENSE` & `ez-toolkits-2.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ez-toolkits-2.9.6/README.md` & `ez-toolkits-2.9.7/README.md`

 * *Files identical despite different names*

### Comparing `ez-toolkits-2.9.6/toolkits/bottle.py` & `ez-toolkits-2.9.7/toolkits/bottle.py`

 * *Files identical despite different names*

### Comparing `ez-toolkits-2.9.6/toolkits/database.py` & `ez-toolkits-2.9.7/toolkits/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+'''
+Column, Table, MetaData API
+    https://docs.sqlalchemy.org/en/14/core/metadata.html#column-table-metadata-api
+'''
 import csv
 
 from loguru import logger
 from sqlalchemy import create_engine, text
 
 from . import utils
 
@@ -29,20 +33,19 @@
             logger.success(f'{info}[成功]')
             return True
         except Exception as e:
             logger.error(f'{info}[失败]')
             logger.exception(e)
             return False
 
-    def metadata_create_all(self, base, init=None, **kwargs):
-        info = '初始化所有表'
+    def metadata_init(self, base, **kwargs):
+        info = '初始化'
         try:
             logger.info(f'{info}......')
-            if init == True:
-                base.metadata.drop_all(self.engine, **kwargs)
+            base.metadata.drop_all(self.engine, **kwargs)
             base.metadata.create_all(self.engine, **kwargs)
             logger.success(f'{info}[成功]')
             return True
         except Exception as e:
             logger.error(f'{info}[失败]')
             logger.exception(e)
             return False
```

### Comparing `ez-toolkits-2.9.6/toolkits/files.py` & `ez-toolkits-2.9.7/toolkits/files.py`

 * *Files identical despite different names*

### Comparing `ez-toolkits-2.9.6/toolkits/mongo.py` & `ez-toolkits-2.9.7/toolkits/mongo.py`

 * *Files identical despite different names*

### Comparing `ez-toolkits-2.9.6/toolkits/plots.py` & `ez-toolkits-2.9.7/toolkits/plots.py`

 * *Files identical despite different names*

### Comparing `ez-toolkits-2.9.6/toolkits/reports.py` & `ez-toolkits-2.9.7/toolkits/reports.py`

 * *Files identical despite different names*

### Comparing `ez-toolkits-2.9.6/toolkits/sendmail.py` & `ez-toolkits-2.9.7/toolkits/sendmail.py`

 * *Files identical despite different names*

### Comparing `ez-toolkits-2.9.6/toolkits/utils.py` & `ez-toolkits-2.9.7/toolkits/utils.py`

 * *Files identical despite different names*

### Comparing `ez-toolkits-2.9.6/toolkits/weixin.py` & `ez-toolkits-2.9.7/toolkits/weixin.py`

 * *Files identical despite different names*

### Comparing `ez-toolkits-2.9.6/toolkits/xftp.py` & `ez-toolkits-2.9.7/toolkits/xftp.py`

 * *Files identical despite different names*

### Comparing `ez-toolkits-2.9.6/toolkits/zabbix.py` & `ez-toolkits-2.9.7/toolkits/zabbix.py`

 * *Files identical despite different names*

