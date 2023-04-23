# Comparing `tmp/easy_patents-1.0.5.tar.gz` & `tmp/easy_patents-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/easy_patents-1.0.5.tar", last modified: Sun Apr 23 07:14:04 2023, max compression
+gzip compressed data, was "dist/easy_patents-1.0.6.tar", last modified: Sun Apr 23 07:23:46 2023, max compression
```

## Comparing `easy_patents-1.0.5.tar` & `easy_patents-1.0.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 07:14:04.000000 easy_patents-1.0.5/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 07:14:04.000000 easy_patents-1.0.5/easy_patents/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 07:14:04.000000 easy_patents-1.0.5/easy_patents/config/
--rw-r--r--   0 root         (0) root         (0)      172 2023-04-23 07:14:03.000000 easy_patents-1.0.5/easy_patents/config/config.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 07:14:04.000000 easy_patents-1.0.5/easy_patents/sample/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 07:14:04.000000 easy_patents-1.0.5/easy_patents/sample/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      579 2023-04-21 22:07:19.000000 easy_patents-1.0.5/easy_patents/sample/__pycache__/sample_openai.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)      645 2023-04-21 08:16:33.000000 easy_patents-1.0.5/easy_patents/sample/__pycache__/sample_translate.cpython-36.pyc
--rw-r--r--   0 root         (0) root         (0)      661 2023-04-21 22:07:19.000000 easy_patents-1.0.5/easy_patents/sample/__pycache__/sample_translate.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     1165 2022-04-30 07:02:34.000000 easy_patents-1.0.5/easy_patents/sample/mail_notify.py
--rw-r--r--   0 root         (0) root         (0)    70294 2023-04-04 17:48:22.000000 easy_patents-1.0.5/easy_patents/sample/openai-0.27.4-py3-none-any.whl
--rw-r--r--   0 root         (0) root         (0)     2166 2022-04-30 07:02:34.000000 easy_patents-1.0.5/easy_patents/sample/sample.py
--rw-r--r--   0 root         (0) root         (0)     7932 2022-04-30 07:02:34.000000 easy_patents-1.0.5/easy_patents/sample/sample_check_due_date.py
--rw-r--r--   0 root         (0) root         (0)     1443 2023-04-21 13:10:49.000000 easy_patents-1.0.5/easy_patents/sample/sample_draft_apeal.py
--rw-r--r--   0 root         (0) root         (0)      376 2023-04-21 22:04:19.000000 easy_patents-1.0.5/easy_patents/sample/sample_openai.py
--rw-r--r--   0 root         (0) root         (0)     2548 2023-04-21 22:41:07.000000 easy_patents-1.0.5/easy_patents/sample/sample_report_oa.py
--rw-r--r--   0 root         (0) root         (0)      519 2023-04-21 08:11:06.000000 easy_patents-1.0.5/easy_patents/sample/sample_translate.py
--rw-r--r--   0 root         (0) root         (0)     2679 2023-04-21 11:02:27.000000 easy_patents-1.0.5/easy_patents/sample/sample_translate_oa.py
--rw-r--r--   0 root         (0) root         (0)     3451 2022-04-30 07:02:34.000000 easy_patents-1.0.5/easy_patents/sample/sample_update_monitor_excel.py
--rw-r--r--   0 root         (0) root         (0)     2929 2023-04-21 04:50:43.000000 easy_patents-1.0.5/easy_patents/auth_info.py
--rw-r--r--   0 root         (0) root         (0)     1113 2022-04-30 07:02:34.000000 easy_patents-1.0.5/easy_patents/delete_caches.py
--rw-r--r--   0 root         (0) root         (0)     1574 2022-04-30 07:02:34.000000 easy_patents-1.0.5/easy_patents/errors.py
--rw-r--r--   0 root         (0) root         (0)     1011 2023-04-21 04:51:41.000000 easy_patents-1.0.5/easy_patents/get_apitoken.py
--rw-r--r--   0 root         (0) root         (0)    36126 2023-04-21 04:56:42.000000 easy_patents-1.0.5/easy_patents/get_info.py
--rw-r--r--   0 root         (0) root         (0)     1810 2023-04-23 07:12:37.000000 easy_patents-1.0.5/easy_patents/update_authinfo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 07:14:04.000000 easy_patents-1.0.5/easy_patents.egg-info/
--rw-r--r--   0 root         (0) root         (0)      243 2023-04-23 07:14:04.000000 easy_patents-1.0.5/easy_patents.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-04-23 07:14:04.000000 easy_patents-1.0.5/easy_patents.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 07:14:04.000000 easy_patents-1.0.5/easy_patents.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       34 2023-04-23 07:14:04.000000 easy_patents-1.0.5/easy_patents.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-23 07:14:04.000000 easy_patents-1.0.5/easy_patents.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       85 2022-04-30 07:02:34.000000 easy_patents-1.0.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)       69 2022-04-30 07:02:34.000000 easy_patents-1.0.5/README.md
--rw-r--r--   0 root         (0) root         (0)      448 2023-04-23 07:13:58.000000 easy_patents-1.0.5/setup.py
--rw-r--r--   0 root         (0) root         (0)      243 2023-04-23 07:14:04.000000 easy_patents-1.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-23 07:14:04.000000 easy_patents-1.0.5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 07:23:46.000000 easy_patents-1.0.6/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 07:23:46.000000 easy_patents-1.0.6/easy_patents/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 07:23:46.000000 easy_patents-1.0.6/easy_patents/config/
+-rw-r--r--   0 root         (0) root         (0)      172 2023-04-23 07:23:45.000000 easy_patents-1.0.6/easy_patents/config/config.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 07:23:46.000000 easy_patents-1.0.6/easy_patents/sample/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 07:23:46.000000 easy_patents-1.0.6/easy_patents/sample/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      579 2023-04-21 22:07:19.000000 easy_patents-1.0.6/easy_patents/sample/__pycache__/sample_openai.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)      645 2023-04-21 08:16:33.000000 easy_patents-1.0.6/easy_patents/sample/__pycache__/sample_translate.cpython-36.pyc
+-rw-r--r--   0 root         (0) root         (0)      661 2023-04-21 22:07:19.000000 easy_patents-1.0.6/easy_patents/sample/__pycache__/sample_translate.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     1165 2022-04-30 07:02:34.000000 easy_patents-1.0.6/easy_patents/sample/mail_notify.py
+-rw-r--r--   0 root         (0) root         (0)    70294 2023-04-04 17:48:22.000000 easy_patents-1.0.6/easy_patents/sample/openai-0.27.4-py3-none-any.whl
+-rw-r--r--   0 root         (0) root         (0)     2166 2022-04-30 07:02:34.000000 easy_patents-1.0.6/easy_patents/sample/sample.py
+-rw-r--r--   0 root         (0) root         (0)     7932 2022-04-30 07:02:34.000000 easy_patents-1.0.6/easy_patents/sample/sample_check_due_date.py
+-rw-r--r--   0 root         (0) root         (0)     1443 2023-04-21 13:10:49.000000 easy_patents-1.0.6/easy_patents/sample/sample_draft_apeal.py
+-rw-r--r--   0 root         (0) root         (0)      376 2023-04-21 22:04:19.000000 easy_patents-1.0.6/easy_patents/sample/sample_openai.py
+-rw-r--r--   0 root         (0) root         (0)     2548 2023-04-21 22:41:07.000000 easy_patents-1.0.6/easy_patents/sample/sample_report_oa.py
+-rw-r--r--   0 root         (0) root         (0)      519 2023-04-21 08:11:06.000000 easy_patents-1.0.6/easy_patents/sample/sample_translate.py
+-rw-r--r--   0 root         (0) root         (0)     2679 2023-04-21 11:02:27.000000 easy_patents-1.0.6/easy_patents/sample/sample_translate_oa.py
+-rw-r--r--   0 root         (0) root         (0)     3451 2022-04-30 07:02:34.000000 easy_patents-1.0.6/easy_patents/sample/sample_update_monitor_excel.py
+-rw-r--r--   0 root         (0) root         (0)     3099 2023-04-23 07:23:07.000000 easy_patents-1.0.6/easy_patents/auth_info.py
+-rw-r--r--   0 root         (0) root         (0)     1113 2022-04-30 07:02:34.000000 easy_patents-1.0.6/easy_patents/delete_caches.py
+-rw-r--r--   0 root         (0) root         (0)     1574 2022-04-30 07:02:34.000000 easy_patents-1.0.6/easy_patents/errors.py
+-rw-r--r--   0 root         (0) root         (0)     1011 2023-04-21 04:51:41.000000 easy_patents-1.0.6/easy_patents/get_apitoken.py
+-rw-r--r--   0 root         (0) root         (0)    36126 2023-04-21 04:56:42.000000 easy_patents-1.0.6/easy_patents/get_info.py
+-rw-r--r--   0 root         (0) root         (0)     1810 2023-04-23 07:12:37.000000 easy_patents-1.0.6/easy_patents/update_authinfo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 07:23:46.000000 easy_patents-1.0.6/easy_patents.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      243 2023-04-23 07:23:46.000000 easy_patents-1.0.6/easy_patents.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-04-23 07:23:46.000000 easy_patents-1.0.6/easy_patents.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 07:23:46.000000 easy_patents-1.0.6/easy_patents.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       34 2023-04-23 07:23:46.000000 easy_patents-1.0.6/easy_patents.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-23 07:23:46.000000 easy_patents-1.0.6/easy_patents.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2022-04-30 07:02:34.000000 easy_patents-1.0.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)       69 2022-04-30 07:02:34.000000 easy_patents-1.0.6/README.md
+-rw-r--r--   0 root         (0) root         (0)      448 2023-04-23 07:23:37.000000 easy_patents-1.0.6/setup.py
+-rw-r--r--   0 root         (0) root         (0)      243 2023-04-23 07:23:46.000000 easy_patents-1.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-23 07:23:46.000000 easy_patents-1.0.6/setup.cfg
```

### Comparing `easy_patents-1.0.5/easy_patents/sample/__pycache__/sample_openai.cpython-39.pyc` & `easy_patents-1.0.6/easy_patents/sample/__pycache__/sample_openai.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.5/easy_patents/sample/__pycache__/sample_translate.cpython-36.pyc` & `easy_patents-1.0.6/easy_patents/sample/__pycache__/sample_translate.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.5/easy_patents/sample/__pycache__/sample_translate.cpython-39.pyc` & `easy_patents-1.0.6/easy_patents/sample/__pycache__/sample_translate.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.5/easy_patents/sample/mail_notify.py` & `easy_patents-1.0.6/easy_patents/sample/mail_notify.py`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.5/easy_patents/sample/openai-0.27.4-py3-none-any.whl` & `easy_patents-1.0.6/easy_patents/sample/openai-0.27.4-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.5/easy_patents/sample/sample.py` & `easy_patents-1.0.6/easy_patents/sample/sample.py`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.5/easy_patents/sample/sample_check_due_date.py` & `easy_patents-1.0.6/easy_patents/sample/sample_check_due_date.py`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.5/easy_patents/sample/sample_draft_apeal.py` & `easy_patents-1.0.6/easy_patents/sample/sample_draft_apeal.py`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.5/easy_patents/sample/sample_report_oa.py` & `easy_patents-1.0.6/easy_patents/sample/sample_report_oa.py`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.5/easy_patents/sample/sample_translate.py` & `easy_patents-1.0.6/easy_patents/sample/sample_translate.py`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.5/easy_patents/sample/sample_translate_oa.py` & `easy_patents-1.0.6/easy_patents/sample/sample_translate_oa.py`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.5/easy_patents/sample/sample_update_monitor_excel.py` & `easy_patents-1.0.6/easy_patents/sample/sample_update_monitor_excel.py`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.5/easy_patents/auth_info.py` & `easy_patents-1.0.6/easy_patents/auth_info.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from easy_patents.get_apitoken import get_token, get_token_by
 import configparser
 from datetime import datetime, timedelta
 import os
 
 EASYPATENT_DIR_NAME = os.path.dirname(__file__)
-EASYPATENT_CONF_FILE = os.path.join(DIR_NAME, 'config/config.ini')
-EASYPATENT_USER_FILE = os.path.join(DIR_NAME, 'config/user.ini')
+EASYPATENT_CONF_FILE = os.path.join(EASYPATENT_DIR_NAME, 'config/config.ini')
+EASYPATENT_USER_FILE = os.path.join(EASYPATENT_DIR_NAME, 'config/user.ini')
 EASYPATENT_DATETIME_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 class AuthInfo:
     def __init__(self):
         self.config = configparser.ConfigParser()
         self.config.read(EASYPATENT_CONF_FILE)
@@ -62,11 +62,17 @@
 
     def get_token_by_refresh_token(self):
         now = datetime.now()
         response = get_token_by(self.refresh_token, self.token_path)
         self.update_tokens(now, response)
 
 
+def get_deepl_key(conf=EASYPATENT_USER_FILE):
+    config = configparser.ConfigParser()
+    config.read(conf)
+    return config['DeepL']['key']
+   
+
 if __name__ == "__main__":
     authinfo = AuthInfo()
     print(authinfo.get_accesstoken())
```

### Comparing `easy_patents-1.0.5/easy_patents/delete_caches.py` & `easy_patents-1.0.6/easy_patents/delete_caches.py`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.5/easy_patents/errors.py` & `easy_patents-1.0.6/easy_patents/errors.py`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.5/easy_patents/get_apitoken.py` & `easy_patents-1.0.6/easy_patents/get_apitoken.py`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.5/easy_patents/get_info.py` & `easy_patents-1.0.6/easy_patents/get_info.py`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.5/easy_patents/update_authinfo.py` & `easy_patents-1.0.6/easy_patents/update_authinfo.py`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.5/easy_patents.egg-info/SOURCES.txt` & `easy_patents-1.0.6/easy_patents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

