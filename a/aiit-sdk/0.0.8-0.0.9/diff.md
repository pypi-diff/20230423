# Comparing `tmp/aiit_sdk-0.0.8.tar.gz` & `tmp/aiit_sdk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiit_sdk-0.0.8.tar", last modified: Wed Apr 20 02:04:28 2022, max compression
+gzip compressed data, was "aiit_sdk-0.0.9.tar", last modified: Tue May 17 08:57:37 2022, max compression
```

## Comparing `aiit_sdk-0.0.8.tar` & `aiit_sdk-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 guoqun    (1000) guoqun    (1000)        0 2022-04-20 02:04:28.507524 aiit_sdk-0.0.8/
--rw-rw-r--   0 guoqun    (1000) guoqun    (1000)    35128 2022-02-24 08:49:57.000000 aiit_sdk-0.0.8/LICENSE
--rw-rw-r--   0 guoqun    (1000) guoqun    (1000)     4738 2022-04-20 02:04:28.507524 aiit_sdk-0.0.8/PKG-INFO
--rw-rw-r--   0 guoqun    (1000) guoqun    (1000)     4143 2022-03-08 07:39:41.000000 aiit_sdk-0.0.8/README.md
--rw-rw-r--   0 guoqun    (1000) guoqun    (1000)      104 2022-02-25 01:47:34.000000 aiit_sdk-0.0.8/pyproject.toml
--rw-rw-r--   0 guoqun    (1000) guoqun    (1000)       38 2022-04-20 02:04:28.507524 aiit_sdk-0.0.8/setup.cfg
--rw-rw-r--   0 guoqun    (1000) guoqun    (1000)     1088 2022-04-20 02:00:18.000000 aiit_sdk-0.0.8/setup.py
-drwxrwxr-x   0 guoqun    (1000) guoqun    (1000)        0 2022-04-20 02:04:28.507524 aiit_sdk-0.0.8/src/
-drwxrwxr-x   0 guoqun    (1000) guoqun    (1000)        0 2022-04-20 02:04:28.507524 aiit_sdk-0.0.8/src/aiit_sdk/
--rw-rw-r--   0 guoqun    (1000) guoqun    (1000)        0 2022-02-25 02:02:13.000000 aiit_sdk-0.0.8/src/aiit_sdk/__init__.py
--rw-rw-r--   0 guoqun    (1000) guoqun    (1000)     2105 2022-03-10 02:58:14.000000 aiit_sdk-0.0.8/src/aiit_sdk/algo.py
--rw-rw-r--   0 guoqun    (1000) guoqun    (1000)     4644 2022-04-20 01:40:14.000000 aiit_sdk-0.0.8/src/aiit_sdk/auth.py
--rw-rw-r--   0 guoqun    (1000) guoqun    (1000)     3795 2022-03-04 09:45:33.000000 aiit_sdk-0.0.8/src/aiit_sdk/log.py
--rw-rw-r--   0 guoqun    (1000) guoqun    (1000)     2607 2022-02-25 02:18:54.000000 aiit_sdk-0.0.8/src/aiit_sdk/page.py
--rw-rw-r--   0 guoqun    (1000) guoqun    (1000)      541 2022-02-25 02:18:54.000000 aiit_sdk-0.0.8/src/aiit_sdk/response.py
--rw-rw-r--   0 guoqun    (1000) guoqun    (1000)     1573 2022-02-25 02:25:03.000000 aiit_sdk-0.0.8/src/aiit_sdk/storage.py
--rw-rw-r--   0 guoqun    (1000) guoqun    (1000)     6674 2022-03-08 07:36:36.000000 aiit_sdk-0.0.8/src/aiit_sdk/view.py
-drwxrwxr-x   0 guoqun    (1000) guoqun    (1000)        0 2022-04-20 02:04:28.507524 aiit_sdk-0.0.8/src/aiit_sdk.egg-info/
--rw-rw-r--   0 guoqun    (1000) guoqun    (1000)     4738 2022-04-20 02:04:28.000000 aiit_sdk-0.0.8/src/aiit_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 guoqun    (1000) guoqun    (1000)      398 2022-04-20 02:04:28.000000 aiit_sdk-0.0.8/src/aiit_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 guoqun    (1000) guoqun    (1000)        1 2022-04-20 02:04:28.000000 aiit_sdk-0.0.8/src/aiit_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 guoqun    (1000) guoqun    (1000)      123 2022-04-20 02:04:28.000000 aiit_sdk-0.0.8/src/aiit_sdk.egg-info/requires.txt
--rw-rw-r--   0 guoqun    (1000) guoqun    (1000)        9 2022-04-20 02:04:28.000000 aiit_sdk-0.0.8/src/aiit_sdk.egg-info/top_level.txt
+drwxrwxr-x   0 guoqun    (1000) guoqun    (1000)        0 2022-05-17 08:57:37.036083 aiit_sdk-0.0.9/
+-rw-rw-r--   0 guoqun    (1000) guoqun    (1000)    35128 2022-02-24 08:49:57.000000 aiit_sdk-0.0.9/LICENSE
+-rw-rw-r--   0 guoqun    (1000) guoqun    (1000)     4718 2022-05-17 08:57:37.036083 aiit_sdk-0.0.9/PKG-INFO
+-rw-rw-r--   0 guoqun    (1000) guoqun    (1000)     4143 2022-03-08 07:39:41.000000 aiit_sdk-0.0.9/README.md
+-rw-rw-r--   0 guoqun    (1000) guoqun    (1000)      104 2022-02-25 01:47:34.000000 aiit_sdk-0.0.9/pyproject.toml
+-rw-rw-r--   0 guoqun    (1000) guoqun    (1000)       38 2022-05-17 08:57:37.036083 aiit_sdk-0.0.9/setup.cfg
+-rw-rw-r--   0 guoqun    (1000) guoqun    (1000)     1088 2022-05-17 08:56:36.000000 aiit_sdk-0.0.9/setup.py
+drwxrwxr-x   0 guoqun    (1000) guoqun    (1000)        0 2022-05-17 08:57:37.036083 aiit_sdk-0.0.9/src/
+drwxrwxr-x   0 guoqun    (1000) guoqun    (1000)        0 2022-05-17 08:57:37.036083 aiit_sdk-0.0.9/src/aiit_sdk/
+-rw-rw-r--   0 guoqun    (1000) guoqun    (1000)        0 2022-02-25 02:02:13.000000 aiit_sdk-0.0.9/src/aiit_sdk/__init__.py
+-rw-rw-r--   0 guoqun    (1000) guoqun    (1000)     2105 2022-03-10 02:58:14.000000 aiit_sdk-0.0.9/src/aiit_sdk/algo.py
+-rw-rw-r--   0 guoqun    (1000) guoqun    (1000)     4644 2022-04-20 01:40:14.000000 aiit_sdk-0.0.9/src/aiit_sdk/auth.py
+-rw-rw-r--   0 guoqun    (1000) guoqun    (1000)     3918 2022-05-17 08:47:42.000000 aiit_sdk-0.0.9/src/aiit_sdk/log.py
+-rw-rw-r--   0 guoqun    (1000) guoqun    (1000)     2607 2022-02-25 02:18:54.000000 aiit_sdk-0.0.9/src/aiit_sdk/page.py
+-rw-rw-r--   0 guoqun    (1000) guoqun    (1000)      541 2022-02-25 02:18:54.000000 aiit_sdk-0.0.9/src/aiit_sdk/response.py
+-rw-rw-r--   0 guoqun    (1000) guoqun    (1000)     1573 2022-02-25 02:25:03.000000 aiit_sdk-0.0.9/src/aiit_sdk/storage.py
+-rw-rw-r--   0 guoqun    (1000) guoqun    (1000)     6674 2022-03-08 07:36:36.000000 aiit_sdk-0.0.9/src/aiit_sdk/view.py
+drwxrwxr-x   0 guoqun    (1000) guoqun    (1000)        0 2022-05-17 08:57:37.036083 aiit_sdk-0.0.9/src/aiit_sdk.egg-info/
+-rw-rw-r--   0 guoqun    (1000) guoqun    (1000)     4718 2022-05-17 08:57:36.000000 aiit_sdk-0.0.9/src/aiit_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 guoqun    (1000) guoqun    (1000)      398 2022-05-17 08:57:37.000000 aiit_sdk-0.0.9/src/aiit_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 guoqun    (1000) guoqun    (1000)        1 2022-05-17 08:57:36.000000 aiit_sdk-0.0.9/src/aiit_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 guoqun    (1000) guoqun    (1000)      123 2022-05-17 08:57:36.000000 aiit_sdk-0.0.9/src/aiit_sdk.egg-info/requires.txt
+-rw-rw-r--   0 guoqun    (1000) guoqun    (1000)        9 2022-05-17 08:57:36.000000 aiit_sdk-0.0.9/src/aiit_sdk.egg-info/top_level.txt
```

### Comparing `aiit_sdk-0.0.8/LICENSE` & `aiit_sdk-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aiit_sdk-0.0.8/PKG-INFO` & `aiit_sdk-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: aiit_sdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: A python sdk for AIIT OS
 Home-page: http://192.168.140.202/unstructured-etl-group/aiit-sdk.git
 Author: Guoqun Jin
 Author-email: guoqun.jin@hotmail.com
 License: GNU General Public License v3.0
 Project-URL: Bug Tracker, http://192.168.140.202/unstructured-etl-group/aiit-sdk/-/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -165,9 +164,7 @@
 
 ### 日志记录模块
 
 位于 `log` 模块下面，有 `create_addition_log()`，`create_change_log()` 和 `create_delete_log()` 3个函数，分别用于记录`添加数据`，`更新数据` 和 `删除数据`的操作。
 
 日志会被记录到 `django.contrib.admin.models` 内的 `LogEntry` 模块内。
 
-
-
```

### Comparing `aiit_sdk-0.0.8/README.md` & `aiit_sdk-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `aiit_sdk-0.0.8/setup.py` & `aiit_sdk-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='aiit_sdk',
-    version='0.0.8',
+    version='0.0.9',
     author='Guoqun Jin',
     author_email='guoqun.jin@hotmail.com',
     description='A python sdk for AIIT OS',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='http://192.168.140.202/unstructured-etl-group/aiit-sdk.git',
     license='GNU General Public License v3.0',
```

### Comparing `aiit_sdk-0.0.8/src/aiit_sdk/algo.py` & `aiit_sdk-0.0.9/src/aiit_sdk/algo.py`

 * *Files identical despite different names*

### Comparing `aiit_sdk-0.0.8/src/aiit_sdk/auth.py` & `aiit_sdk-0.0.9/src/aiit_sdk/auth.py`

 * *Files identical despite different names*

### Comparing `aiit_sdk-0.0.8/src/aiit_sdk/log.py` & `aiit_sdk-0.0.9/src/aiit_sdk/log.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,14 +31,16 @@
         value = str(float(f_value))
     else:
         value = str(f_value)
     return value
 
 
 def create_addition_log(user_id, oj):
+    if not user_id:
+        return False
     lg = LogEntry.objects.log_action(
         user_id=user_id,
         content_type_id=get_content_type_for_model(oj).pk,
         object_id=oj.pk,
         object_repr=str(oj),
         action_flag=ADDITION,
     )
@@ -57,14 +59,16 @@
     addition_message = json.dumps(addition_message_dict, ensure_ascii=False)
     lg.change_message = addition_message
     lg.save()
     return True
 
 
 def create_change_log(user_id, oj, origin_data, new_data):
+    if not user_id:
+        return False
     lg = LogEntry.objects.log_action(
         user_id=user_id,
         content_type_id=get_content_type_for_model(oj).pk,
         object_id=oj.pk,
         object_repr=str(oj),
         action_flag=CHANGE,
     )
@@ -84,14 +88,16 @@
     change_message = json.dumps(change_message_dict, ensure_ascii=False)
     lg.change_message = change_message
     lg.save()
     return True
 
 
 def create_delete_log(user_id, oj):
+    if not user_id:
+        return False
     lg = LogEntry.objects.log_action(
         user_id=user_id,
         content_type_id=get_content_type_for_model(oj).pk,
         object_id=oj.pk,
         object_repr=str(oj),
         action_flag=DELETION,
     )
```

### Comparing `aiit_sdk-0.0.8/src/aiit_sdk/page.py` & `aiit_sdk-0.0.9/src/aiit_sdk/page.py`

 * *Files identical despite different names*

### Comparing `aiit_sdk-0.0.8/src/aiit_sdk/response.py` & `aiit_sdk-0.0.9/src/aiit_sdk/response.py`

 * *Files identical despite different names*

### Comparing `aiit_sdk-0.0.8/src/aiit_sdk/storage.py` & `aiit_sdk-0.0.9/src/aiit_sdk/storage.py`

 * *Files identical despite different names*

### Comparing `aiit_sdk-0.0.8/src/aiit_sdk/view.py` & `aiit_sdk-0.0.9/src/aiit_sdk/view.py`

 * *Files identical despite different names*

### Comparing `aiit_sdk-0.0.8/src/aiit_sdk.egg-info/PKG-INFO` & `aiit_sdk-0.0.9/src/aiit_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: aiit-sdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: A python sdk for AIIT OS
 Home-page: http://192.168.140.202/unstructured-etl-group/aiit-sdk.git
 Author: Guoqun Jin
 Author-email: guoqun.jin@hotmail.com
 License: GNU General Public License v3.0
 Project-URL: Bug Tracker, http://192.168.140.202/unstructured-etl-group/aiit-sdk/-/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -165,9 +164,7 @@
 
 ### 日志记录模块
 
 位于 `log` 模块下面，有 `create_addition_log()`，`create_change_log()` 和 `create_delete_log()` 3个函数，分别用于记录`添加数据`，`更新数据` 和 `删除数据`的操作。
 
 日志会被记录到 `django.contrib.admin.models` 内的 `LogEntry` 模块内。
 
-
-
```

