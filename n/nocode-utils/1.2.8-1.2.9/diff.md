# Comparing `tmp/nocode_utils-1.2.8.tar.gz` & `tmp/nocode_utils-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nocode_utils-1.2.8.tar", last modified: Mon Feb 20 02:45:12 2023, max compression
+gzip compressed data, was "dist/nocode_utils-1.2.9.tar", last modified: Sun Apr 23 08:38:27 2023, max compression
```

## Comparing `nocode_utils-1.2.8.tar` & `nocode_utils-1.2.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 nocode     (502) staff       (20)        0 2023-02-20 02:45:12.000000 nocode_utils-1.2.8/
--rw-r--r--   0 nocode     (502) staff       (20)       33 2022-05-31 03:27:00.000000 nocode_utils-1.2.8/LICENSE
--rw-r--r--   0 nocode     (502) staff       (20)       27 2022-07-18 05:41:09.000000 nocode_utils-1.2.8/MANIFEST.in
--rw-r--r--   0 nocode     (502) staff       (20)     1387 2023-02-20 02:45:12.000000 nocode_utils-1.2.8/PKG-INFO
--rw-r--r--   0 nocode     (502) staff       (20)      864 2022-07-15 06:30:05.000000 nocode_utils-1.2.8/README.md
-drwxr-xr-x   0 nocode     (502) staff       (20)        0 2023-02-20 02:45:12.000000 nocode_utils-1.2.8/nocode_utils/
--rw-r--r--   0 nocode     (502) staff       (20)      244 2022-05-31 03:22:16.000000 nocode_utils-1.2.8/nocode_utils/__init__.py
--rw-r--r--   0 nocode     (502) staff       (20)      461 2022-07-15 09:58:39.000000 nocode_utils-1.2.8/nocode_utils/config.py
-drwxr-xr-x   0 nocode     (502) staff       (20)        0 2023-02-20 02:45:12.000000 nocode_utils-1.2.8/nocode_utils/database_utils/
--rw-r--r--   0 nocode     (502) staff       (20)     2797 2022-07-11 06:19:45.000000 nocode_utils-1.2.8/nocode_utils/database_utils/DBProcessor.py
--rw-r--r--   0 nocode     (502) staff       (20)      244 2022-05-31 06:19:46.000000 nocode_utils-1.2.8/nocode_utils/database_utils/__init__.py
-drwxr-xr-x   0 nocode     (502) staff       (20)        0 2023-02-20 02:45:12.000000 nocode_utils-1.2.8/nocode_utils/feishu_utils/
--rw-r--r--   0 nocode     (502) staff       (20)     1029 2023-01-29 08:23:56.000000 nocode_utils-1.2.8/nocode_utils/feishu_utils/AESCipher.py
--rw-r--r--   0 nocode     (502) staff       (20)    10554 2023-02-20 02:44:02.000000 nocode_utils-1.2.8/nocode_utils/feishu_utils/__init__.py
-drwxr-xr-x   0 nocode     (502) staff       (20)        0 2023-02-20 02:45:12.000000 nocode_utils-1.2.8/nocode_utils/http_utils/
--rw-r--r--   0 nocode     (502) staff       (20)     2127 2022-06-20 09:06:30.000000 nocode_utils-1.2.8/nocode_utils/http_utils/__init__.py
-drwxr-xr-x   0 nocode     (502) staff       (20)        0 2023-02-20 02:45:12.000000 nocode_utils-1.2.8/nocode_utils/nlp_utils/
--rw-r--r--   0 nocode     (502) staff       (20)     3429 2022-08-09 02:43:50.000000 nocode_utils-1.2.8/nocode_utils/nlp_utils/Simbert.py
--rw-r--r--   0 nocode     (502) staff       (20)      244 2022-05-31 06:50:22.000000 nocode_utils-1.2.8/nocode_utils/nlp_utils/__init__.py
--rw-r--r--   0 nocode     (502) staff       (20)     1270 2022-07-11 05:13:33.000000 nocode_utils-1.2.8/nocode_utils/nlp_utils/common.py
--rw-r--r--   0 nocode     (502) staff       (20)     2867 2022-08-09 02:47:13.000000 nocode_utils-1.2.8/nocode_utils/nlp_utils/data_augmentation.py
--rw-r--r--   0 nocode     (502) staff       (20)     1498 2022-07-15 05:59:20.000000 nocode_utils-1.2.8/nocode_utils/nlp_utils/data_preprocess.py
-drwxr-xr-x   0 nocode     (502) staff       (20)        0 2023-02-20 02:45:12.000000 nocode_utils-1.2.8/nocode_utils/threading_utils/
--rw-r--r--   0 nocode     (502) staff       (20)     1048 2023-01-28 06:15:51.000000 nocode_utils-1.2.8/nocode_utils/threading_utils/Threads.py
--rw-r--r--   0 nocode     (502) staff       (20)      244 2022-05-31 06:59:57.000000 nocode_utils-1.2.8/nocode_utils/threading_utils/__init__.py
-drwxr-xr-x   0 nocode     (502) staff       (20)        0 2023-02-20 02:45:12.000000 nocode_utils-1.2.8/nocode_utils.egg-info/
--rw-r--r--   0 nocode     (502) staff       (20)     1387 2023-02-20 02:45:11.000000 nocode_utils-1.2.8/nocode_utils.egg-info/PKG-INFO
--rw-r--r--   0 nocode     (502) staff       (20)      695 2023-02-20 02:45:12.000000 nocode_utils-1.2.8/nocode_utils.egg-info/SOURCES.txt
--rw-r--r--   0 nocode     (502) staff       (20)        1 2023-02-20 02:45:11.000000 nocode_utils-1.2.8/nocode_utils.egg-info/dependency_links.txt
--rw-r--r--   0 nocode     (502) staff       (20)       13 2023-02-20 02:45:11.000000 nocode_utils-1.2.8/nocode_utils.egg-info/top_level.txt
--rw-r--r--   0 nocode     (502) staff       (20)       38 2023-02-20 02:45:12.000000 nocode_utils-1.2.8/setup.cfg
--rw-r--r--   0 nocode     (502) staff       (20)     1079 2023-02-20 02:44:11.000000 nocode_utils-1.2.8/setup.py
+drwxr-xr-x   0 nocode     (502) staff       (20)        0 2023-04-23 08:38:27.000000 nocode_utils-1.2.9/
+-rw-r--r--   0 nocode     (502) staff       (20)       33 2022-05-31 03:27:00.000000 nocode_utils-1.2.9/LICENSE
+-rw-r--r--   0 nocode     (502) staff       (20)       27 2022-07-18 05:41:09.000000 nocode_utils-1.2.9/MANIFEST.in
+-rw-r--r--   0 nocode     (502) staff       (20)     1387 2023-04-23 08:38:27.000000 nocode_utils-1.2.9/PKG-INFO
+-rw-r--r--   0 nocode     (502) staff       (20)      864 2022-07-15 06:30:05.000000 nocode_utils-1.2.9/README.md
+drwxr-xr-x   0 nocode     (502) staff       (20)        0 2023-04-23 08:38:27.000000 nocode_utils-1.2.9/nocode_utils/
+-rw-r--r--   0 nocode     (502) staff       (20)      244 2022-05-31 03:22:16.000000 nocode_utils-1.2.9/nocode_utils/__init__.py
+-rw-r--r--   0 nocode     (502) staff       (20)      461 2022-07-15 09:58:39.000000 nocode_utils-1.2.9/nocode_utils/config.py
+drwxr-xr-x   0 nocode     (502) staff       (20)        0 2023-04-23 08:38:27.000000 nocode_utils-1.2.9/nocode_utils/database_utils/
+-rw-r--r--   0 nocode     (502) staff       (20)     2797 2022-07-11 06:19:45.000000 nocode_utils-1.2.9/nocode_utils/database_utils/DBProcessor.py
+-rw-r--r--   0 nocode     (502) staff       (20)      244 2022-05-31 06:19:46.000000 nocode_utils-1.2.9/nocode_utils/database_utils/__init__.py
+drwxr-xr-x   0 nocode     (502) staff       (20)        0 2023-04-23 08:38:27.000000 nocode_utils-1.2.9/nocode_utils/feishu_utils/
+-rw-r--r--   0 nocode     (502) staff       (20)     1029 2023-01-29 08:23:56.000000 nocode_utils-1.2.9/nocode_utils/feishu_utils/AESCipher.py
+-rw-r--r--   0 nocode     (502) staff       (20)    10561 2023-04-23 07:33:51.000000 nocode_utils-1.2.9/nocode_utils/feishu_utils/__init__.py
+drwxr-xr-x   0 nocode     (502) staff       (20)        0 2023-04-23 08:38:27.000000 nocode_utils-1.2.9/nocode_utils/http_utils/
+-rw-r--r--   0 nocode     (502) staff       (20)     2127 2022-06-20 09:06:30.000000 nocode_utils-1.2.9/nocode_utils/http_utils/__init__.py
+drwxr-xr-x   0 nocode     (502) staff       (20)        0 2023-04-23 08:38:27.000000 nocode_utils-1.2.9/nocode_utils/nlp_utils/
+-rw-r--r--   0 nocode     (502) staff       (20)     3429 2022-08-09 02:43:50.000000 nocode_utils-1.2.9/nocode_utils/nlp_utils/Simbert.py
+-rw-r--r--   0 nocode     (502) staff       (20)      244 2022-05-31 06:50:22.000000 nocode_utils-1.2.9/nocode_utils/nlp_utils/__init__.py
+-rw-r--r--   0 nocode     (502) staff       (20)     1270 2022-07-11 05:13:33.000000 nocode_utils-1.2.9/nocode_utils/nlp_utils/common.py
+-rw-r--r--   0 nocode     (502) staff       (20)     2867 2022-08-09 02:47:13.000000 nocode_utils-1.2.9/nocode_utils/nlp_utils/data_augmentation.py
+-rw-r--r--   0 nocode     (502) staff       (20)     1498 2022-07-15 05:59:20.000000 nocode_utils-1.2.9/nocode_utils/nlp_utils/data_preprocess.py
+drwxr-xr-x   0 nocode     (502) staff       (20)        0 2023-04-23 08:38:27.000000 nocode_utils-1.2.9/nocode_utils/threading_utils/
+-rw-r--r--   0 nocode     (502) staff       (20)     1048 2023-01-28 06:15:51.000000 nocode_utils-1.2.9/nocode_utils/threading_utils/Threads.py
+-rw-r--r--   0 nocode     (502) staff       (20)      244 2022-05-31 06:59:57.000000 nocode_utils-1.2.9/nocode_utils/threading_utils/__init__.py
+drwxr-xr-x   0 nocode     (502) staff       (20)        0 2023-04-23 08:38:27.000000 nocode_utils-1.2.9/nocode_utils.egg-info/
+-rw-r--r--   0 nocode     (502) staff       (20)     1387 2023-04-23 08:38:27.000000 nocode_utils-1.2.9/nocode_utils.egg-info/PKG-INFO
+-rw-r--r--   0 nocode     (502) staff       (20)      695 2023-04-23 08:38:27.000000 nocode_utils-1.2.9/nocode_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 nocode     (502) staff       (20)        1 2023-04-23 08:38:27.000000 nocode_utils-1.2.9/nocode_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 nocode     (502) staff       (20)       13 2023-04-23 08:38:27.000000 nocode_utils-1.2.9/nocode_utils.egg-info/top_level.txt
+-rw-r--r--   0 nocode     (502) staff       (20)       38 2023-04-23 08:38:27.000000 nocode_utils-1.2.9/setup.cfg
+-rw-r--r--   0 nocode     (502) staff       (20)     1079 2023-04-23 08:36:30.000000 nocode_utils-1.2.9/setup.py
```

### Comparing `nocode_utils-1.2.8/PKG-INFO` & `nocode_utils-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nocode_utils
-Version: 1.2.8
+Version: 1.2.9
 Summary: 封装常用函数和类
 Home-page: https://github.com/jasonhhao
 Author: JasonHao
 Author-email: hhao9483@gmail.com
 License: UNKNOWN
 Platform: all
 Classifier: Intended Audience :: Developers
```

### Comparing `nocode_utils-1.2.8/README.md` & `nocode_utils-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `nocode_utils-1.2.8/nocode_utils/database_utils/DBProcessor.py` & `nocode_utils-1.2.9/nocode_utils/database_utils/DBProcessor.py`

 * *Files identical despite different names*

### Comparing `nocode_utils-1.2.8/nocode_utils/feishu_utils/AESCipher.py` & `nocode_utils-1.2.9/nocode_utils/feishu_utils/AESCipher.py`

 * *Files identical despite different names*

### Comparing `nocode_utils-1.2.8/nocode_utils/feishu_utils/__init__.py` & `nocode_utils-1.2.9/nocode_utils/feishu_utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,15 +209,15 @@
                     for item in self.rate_limit[email]:
                         if item['path'] == key:
                             if item['count'] < 3 and int(current_time) - int(item['lasttime']) > self.interval:
                                 item['lasttime'] = current_time
                                 item['count'] += 1
                                 valid_emails.append(email)
 
-                            elif int(current_time) - int(last_time) > 3600 * 24:
+                            elif int(current_time) - int(item['lasttime']) > 3600 * 24:
                                 item['lasttime'] = current_time
                                 item['count'] = 1
                                 valid_emails.append(email)
 
         return valid_emails
 
     def alert_message(self, content, emails=[]):
```

### Comparing `nocode_utils-1.2.8/nocode_utils/http_utils/__init__.py` & `nocode_utils-1.2.9/nocode_utils/http_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nocode_utils-1.2.8/nocode_utils/nlp_utils/Simbert.py` & `nocode_utils-1.2.9/nocode_utils/nlp_utils/Simbert.py`

 * *Files identical despite different names*

### Comparing `nocode_utils-1.2.8/nocode_utils/nlp_utils/common.py` & `nocode_utils-1.2.9/nocode_utils/nlp_utils/common.py`

 * *Files identical despite different names*

### Comparing `nocode_utils-1.2.8/nocode_utils/nlp_utils/data_augmentation.py` & `nocode_utils-1.2.9/nocode_utils/nlp_utils/data_augmentation.py`

 * *Files identical despite different names*

### Comparing `nocode_utils-1.2.8/nocode_utils/nlp_utils/data_preprocess.py` & `nocode_utils-1.2.9/nocode_utils/nlp_utils/data_preprocess.py`

 * *Files identical despite different names*

### Comparing `nocode_utils-1.2.8/nocode_utils/threading_utils/Threads.py` & `nocode_utils-1.2.9/nocode_utils/threading_utils/Threads.py`

 * *Files identical despite different names*

### Comparing `nocode_utils-1.2.8/nocode_utils.egg-info/PKG-INFO` & `nocode_utils-1.2.9/nocode_utils.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nocode-utils
-Version: 1.2.8
+Version: 1.2.9
 Summary: 封装常用函数和类
 Home-page: https://github.com/jasonhhao
 Author: JasonHao
 Author-email: hhao9483@gmail.com
 License: UNKNOWN
 Platform: all
 Classifier: Intended Audience :: Developers
```

### Comparing `nocode_utils-1.2.8/nocode_utils.egg-info/SOURCES.txt` & `nocode_utils-1.2.9/nocode_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nocode_utils-1.2.8/setup.py` & `nocode_utils-1.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(name='nocode_utils',  # 包名
-      version='1.2.8',  # 版本号
+      version='1.2.9',  # 版本号
       description='封装常用函数和类',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='JasonHao',
       author_email='hhao9483@gmail.com',
       url='https://github.com/jasonhhao',
       install_requires=[
```

