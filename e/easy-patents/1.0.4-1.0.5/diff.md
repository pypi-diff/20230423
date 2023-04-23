# Comparing `tmp/easy_patents-1.0.4.tar.gz` & `tmp/easy_patents-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/easy_patents-1.0.4.tar", last modified: Thu Apr 20 13:16:59 2023, max compression
+gzip compressed data, was "dist/easy_patents-1.0.5.tar", last modified: Sun Apr 23 07:14:04 2023, max compression
```

## Comparing `easy_patents-1.0.4.tar` & `easy_patents-1.0.5.tar`

### file list

```diff
@@ -1,26 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 13:16:59.000000 easy_patents-1.0.4/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 13:16:59.000000 easy_patents-1.0.4/easy_patents/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 13:16:59.000000 easy_patents-1.0.4/easy_patents/config/
--rw-r--r--   0 root         (0) root         (0)      172 2023-04-20 13:16:59.000000 easy_patents-1.0.4/easy_patents/config/config.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 13:16:59.000000 easy_patents-1.0.4/easy_patents/sample/
--rw-r--r--   0 root         (0) root         (0)     1165 2022-04-30 07:02:34.000000 easy_patents-1.0.4/easy_patents/sample/mail_notify.py
--rw-r--r--   0 root         (0) root         (0)     2166 2022-04-30 07:02:34.000000 easy_patents-1.0.4/easy_patents/sample/sample.py
--rw-r--r--   0 root         (0) root         (0)     7932 2022-04-30 07:02:34.000000 easy_patents-1.0.4/easy_patents/sample/sample_check_due_date.py
--rw-r--r--   0 root         (0) root         (0)     3451 2022-04-30 07:02:34.000000 easy_patents-1.0.4/easy_patents/sample/sample_update_monitor_excel.py
--rw-r--r--   0 root         (0) root         (0)     2808 2022-04-30 07:02:34.000000 easy_patents-1.0.4/easy_patents/auth_info.py
--rw-r--r--   0 root         (0) root         (0)     1113 2022-04-30 07:02:34.000000 easy_patents-1.0.4/easy_patents/delete_caches.py
--rw-r--r--   0 root         (0) root         (0)     1574 2022-04-30 07:02:34.000000 easy_patents-1.0.4/easy_patents/errors.py
--rw-r--r--   0 root         (0) root         (0)      934 2022-04-30 07:02:34.000000 easy_patents-1.0.4/easy_patents/get_apitoken.py
--rw-r--r--   0 root         (0) root         (0)    35935 2023-04-20 13:15:55.000000 easy_patents-1.0.4/easy_patents/get_info.py
--rw-r--r--   0 root         (0) root         (0)     1321 2022-04-30 07:02:34.000000 easy_patents-1.0.4/easy_patents/update_authinfo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 13:16:59.000000 easy_patents-1.0.4/easy_patents.egg-info/
--rw-r--r--   0 root         (0) root         (0)      243 2023-04-20 13:16:59.000000 easy_patents-1.0.4/easy_patents.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      566 2023-04-20 13:16:59.000000 easy_patents-1.0.4/easy_patents.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 13:16:59.000000 easy_patents-1.0.4/easy_patents.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       34 2023-04-20 13:16:59.000000 easy_patents-1.0.4/easy_patents.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-20 13:16:59.000000 easy_patents-1.0.4/easy_patents.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       85 2022-04-30 07:02:34.000000 easy_patents-1.0.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)       69 2022-04-30 07:02:34.000000 easy_patents-1.0.4/README.md
--rw-r--r--   0 root         (0) root         (0)      448 2023-04-20 13:16:58.000000 easy_patents-1.0.4/setup.py
--rw-r--r--   0 root         (0) root         (0)      243 2023-04-20 13:16:59.000000 easy_patents-1.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 13:16:59.000000 easy_patents-1.0.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 07:14:04.000000 easy_patents-1.0.5/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 07:14:04.000000 easy_patents-1.0.5/easy_patents/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 07:14:04.000000 easy_patents-1.0.5/easy_patents/config/
+-rw-r--r--   0 root         (0) root         (0)      172 2023-04-23 07:14:03.000000 easy_patents-1.0.5/easy_patents/config/config.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 07:14:04.000000 easy_patents-1.0.5/easy_patents/sample/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 07:14:04.000000 easy_patents-1.0.5/easy_patents/sample/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      579 2023-04-21 22:07:19.000000 easy_patents-1.0.5/easy_patents/sample/__pycache__/sample_openai.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)      645 2023-04-21 08:16:33.000000 easy_patents-1.0.5/easy_patents/sample/__pycache__/sample_translate.cpython-36.pyc
+-rw-r--r--   0 root         (0) root         (0)      661 2023-04-21 22:07:19.000000 easy_patents-1.0.5/easy_patents/sample/__pycache__/sample_translate.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     1165 2022-04-30 07:02:34.000000 easy_patents-1.0.5/easy_patents/sample/mail_notify.py
+-rw-r--r--   0 root         (0) root         (0)    70294 2023-04-04 17:48:22.000000 easy_patents-1.0.5/easy_patents/sample/openai-0.27.4-py3-none-any.whl
+-rw-r--r--   0 root         (0) root         (0)     2166 2022-04-30 07:02:34.000000 easy_patents-1.0.5/easy_patents/sample/sample.py
+-rw-r--r--   0 root         (0) root         (0)     7932 2022-04-30 07:02:34.000000 easy_patents-1.0.5/easy_patents/sample/sample_check_due_date.py
+-rw-r--r--   0 root         (0) root         (0)     1443 2023-04-21 13:10:49.000000 easy_patents-1.0.5/easy_patents/sample/sample_draft_apeal.py
+-rw-r--r--   0 root         (0) root         (0)      376 2023-04-21 22:04:19.000000 easy_patents-1.0.5/easy_patents/sample/sample_openai.py
+-rw-r--r--   0 root         (0) root         (0)     2548 2023-04-21 22:41:07.000000 easy_patents-1.0.5/easy_patents/sample/sample_report_oa.py
+-rw-r--r--   0 root         (0) root         (0)      519 2023-04-21 08:11:06.000000 easy_patents-1.0.5/easy_patents/sample/sample_translate.py
+-rw-r--r--   0 root         (0) root         (0)     2679 2023-04-21 11:02:27.000000 easy_patents-1.0.5/easy_patents/sample/sample_translate_oa.py
+-rw-r--r--   0 root         (0) root         (0)     3451 2022-04-30 07:02:34.000000 easy_patents-1.0.5/easy_patents/sample/sample_update_monitor_excel.py
+-rw-r--r--   0 root         (0) root         (0)     2929 2023-04-21 04:50:43.000000 easy_patents-1.0.5/easy_patents/auth_info.py
+-rw-r--r--   0 root         (0) root         (0)     1113 2022-04-30 07:02:34.000000 easy_patents-1.0.5/easy_patents/delete_caches.py
+-rw-r--r--   0 root         (0) root         (0)     1574 2022-04-30 07:02:34.000000 easy_patents-1.0.5/easy_patents/errors.py
+-rw-r--r--   0 root         (0) root         (0)     1011 2023-04-21 04:51:41.000000 easy_patents-1.0.5/easy_patents/get_apitoken.py
+-rw-r--r--   0 root         (0) root         (0)    36126 2023-04-21 04:56:42.000000 easy_patents-1.0.5/easy_patents/get_info.py
+-rw-r--r--   0 root         (0) root         (0)     1810 2023-04-23 07:12:37.000000 easy_patents-1.0.5/easy_patents/update_authinfo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 07:14:04.000000 easy_patents-1.0.5/easy_patents.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      243 2023-04-23 07:14:04.000000 easy_patents-1.0.5/easy_patents.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-04-23 07:14:04.000000 easy_patents-1.0.5/easy_patents.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 07:14:04.000000 easy_patents-1.0.5/easy_patents.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       34 2023-04-23 07:14:04.000000 easy_patents-1.0.5/easy_patents.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-23 07:14:04.000000 easy_patents-1.0.5/easy_patents.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2022-04-30 07:02:34.000000 easy_patents-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)       69 2022-04-30 07:02:34.000000 easy_patents-1.0.5/README.md
+-rw-r--r--   0 root         (0) root         (0)      448 2023-04-23 07:13:58.000000 easy_patents-1.0.5/setup.py
+-rw-r--r--   0 root         (0) root         (0)      243 2023-04-23 07:14:04.000000 easy_patents-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-23 07:14:04.000000 easy_patents-1.0.5/setup.cfg
```

### Comparing `easy_patents-1.0.4/easy_patents/sample/mail_notify.py` & `easy_patents-1.0.5/easy_patents/sample/mail_notify.py`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.4/easy_patents/sample/sample.py` & `easy_patents-1.0.5/easy_patents/sample/sample.py`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.4/easy_patents/sample/sample_check_due_date.py` & `easy_patents-1.0.5/easy_patents/sample/sample_check_due_date.py`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.4/easy_patents/sample/sample_update_monitor_excel.py` & `easy_patents-1.0.5/easy_patents/sample/sample_update_monitor_excel.py`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.4/easy_patents/auth_info.py` & `easy_patents-1.0.5/easy_patents/auth_info.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 from easy_patents.get_apitoken import get_token, get_token_by
 import configparser
 from datetime import datetime, timedelta
 import os
 
-DIR_NAME = os.path.dirname(__file__)
-CONF_FILE = os.path.join(DIR_NAME, 'config/config.ini')
-USER_FILE = os.path.join(DIR_NAME, 'config/user.ini')
-DATETIME_FORMAT = "%Y-%m-%d %H:%M:%S"
+EASYPATENT_DIR_NAME = os.path.dirname(__file__)
+EASYPATENT_CONF_FILE = os.path.join(DIR_NAME, 'config/config.ini')
+EASYPATENT_USER_FILE = os.path.join(DIR_NAME, 'config/user.ini')
+EASYPATENT_DATETIME_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 class AuthInfo:
     def __init__(self):
         self.config = configparser.ConfigParser()
-        self.config.read(CONF_FILE)
+        self.config.read(EASYPATENT_CONF_FILE)
         self.user_conf = configparser.ConfigParser()
-        self.user_conf.read(USER_FILE)
+        self.user_conf.read(EASYPATENT_USER_FILE)
         self.token_path = self.user_conf['AuthInfo']['token_path']
         self.username = self.user_conf['AuthInfo']['username']
         self.password = self.user_conf['AuthInfo']['password']
         self.read_accesstokens()
 
     def get_accesstoken(self):
         self.refresh()
         return self.access_token
 
     def read_accesstokens(self):
         self.access_token = self.config['AuthInfo']['access_token']
         expire_in = self.config['AuthInfo']['expires_in']
-        self.expires_in = datetime.strptime(expire_in, DATETIME_FORMAT)
+        self.expires_in = datetime.strptime(expire_in, EASYPATENT_DATETIME_FORMAT)
         self.refresh_token = self.config['AuthInfo']['refresh_token']
         refresh_expires_in = self.config['AuthInfo']['refresh_expires_in']
-        self.refresh_expires_in = datetime.strptime(refresh_expires_in, DATETIME_FORMAT)
+        self.refresh_expires_in = datetime.strptime(refresh_expires_in, EASYPATENT_DATETIME_FORMAT)
 
     def refresh(self):
         now = datetime.now()
         if now > self.refresh_expires_in:
             self.get_token_by_username()
         elif now > self.expires_in:
             self.get_token_by_refresh_token()
@@ -42,19 +42,19 @@
     def update_tokens(self, now, response):
         response = response.json()
         # Configファイルのアップデート
         self.config['AuthInfo']['access_token'] = response['access_token']
         self.config['AuthInfo']['refresh_token'] = response['refresh_token']
         expire_td = timedelta(seconds=(response['expires_in']))
         expires_in = now + expire_td
-        self.config['AuthInfo']['expires_in'] = expires_in.strftime(DATETIME_FORMAT)
+        self.config['AuthInfo']['expires_in'] = expires_in.strftime(EASYPATENT_DATETIME_FORMAT)
         refresh_expire_td = timedelta(seconds=(response['refresh_expires_in']))
         refresh_expires_in = now + refresh_expire_td
-        self.config['AuthInfo']['refresh_expires_in'] = refresh_expires_in.strftime(DATETIME_FORMAT)
-        with open(CONF_FILE, "w") as f:
+        self.config['AuthInfo']['refresh_expires_in'] = refresh_expires_in.strftime(EASYPATENT_DATETIME_FORMAT)
+        with open(EASYPATENT_CONF_FILE, "w") as f:
             self.config.write(f)
         self.read_accesstokens()
 
 
     def get_token_by_username(self):
         now = datetime.now()
         response = get_token(self.username, self.password, self.token_path)
```

### Comparing `easy_patents-1.0.4/easy_patents/delete_caches.py` & `easy_patents-1.0.5/easy_patents/delete_caches.py`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.4/easy_patents/errors.py` & `easy_patents-1.0.5/easy_patents/errors.py`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.4/easy_patents/get_apitoken.py` & `easy_patents-1.0.5/easy_patents/get_apitoken.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import sys
 import requests
 
 # パラメータ定義
-HOST = "ip-data.jpo.go.jp"
-CONTENT_TYPE = "application/x-www-form-urlencoded"
-HEADER = {
-    "Host": HOST,
-    "Content-Type": CONTENT_TYPE 
+EASYPATENT_HOST = "ip-data.jpo.go.jp"
+EASYPATENT_CONTENT_TYPE = "application/x-www-form-urlencoded"
+EASYPATENT_HEADER = {
+    "Host": EASYPATENT_HOST,
+    "Content-Type": EASYPATENT_CONTENT_TYPE 
 }
 
 def get_token(user, password, token_path):
     grant_type = "password"
     data = {
         "grant_type": grant_type,
         "username": user,
         "password": password
     }
-    return requests.post(url=token_path, data=data, headers=HEADER)
+    return requests.post(url=token_path, data=data, headers=EASYPATENT_HEADER)
 
 def get_token_by(refresh_token, token_path):
     grant_type = "refresh_token"
     data = {
         "grant_type": grant_type,
         "refresh_token": refresh_token,
     }
-    return requests.post(url=token_path, data=data, headers=HEADER)
+    return requests.post(url=token_path, data=data, headers=EASYPATENT_HEADER)
 
 
 if __name__ == "__main__":
     if len(sys.argv) != 3:
         print('Usage: %s "username" "password"' % sys.argv[0])
         exit()
     user = sys.argv[1]
```

### Comparing `easy_patents-1.0.4/easy_patents/get_info.py` & `easy_patents-1.0.5/easy_patents/get_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 import time
 import datetime
 import configparser
 import zipfile
 import json
 import glob
 import pathlib
-from easy_patents.get_apitoken import HOST
-from easy_patents.auth_info import AuthInfo, DATETIME_FORMAT
+from easy_patents.auth_info import AuthInfo
 from easy_patents.errors import is_error
 
-
-AUTHINFO = AuthInfo()
-CONFIG = AUTHINFO.config
-
-API_RETRY = 3
-API_SLEEP_TIME = 1
-API_TEMPORARY_ERRORS = {'210', '302', '303'}
+EASYPATENT_HOST = "ip-data.jpo.go.jp"
+EASYPATENT_AUTHINFO = AuthInfo()
+EASYPATENT_CONFIG = EASYPATENT_AUTHINFO.config
+EASYPATENT_DATETIME_FORMAT = "%Y-%m-%d %H:%M:%S"
+
+EASYPATENT_API_RETRY = 3
+EASYPATENT_API_SLEEP_TIME = 1
+EASYPATENT_API_TEMPORARY_ERRORS = {'210', '302', '303'}
 
 
 def get_api_info(url):
     '''
     API情報を取得する関数
     レスポンスがjsonデータの場合にはjson形式に変換する
 
@@ -36,30 +36,30 @@
 
     Returns
     -------
     json or response
         取得したデータ
     '''
     # 通信失敗などで取得エラーがありうるので、RETRY回までリトライする
-    for i in range(0, API_RETRY):
-        accesstoken = AUTHINFO.get_accesstoken()
+    for i in range(0, EASYPATENT_API_RETRY):
+        accesstoken = EASYPATENT_AUTHINFO.get_accesstoken()
         header = {
-            "Host": HOST,
+            "Host": EASYPATENT_HOST,
             "Authorization": "Bearer " + accesstoken
         }
         response = requests.get(url, headers=header)
         # jsonファイル以外の場合には取得は成功しているので、breakする
         if response.headers['content-type'] != "application/json":
             break
         response = response.json()
         status_code = response["result"]["statusCode"]
         # statusCodeがAPI_TEMPORARY_ERRORSの場合、
         # API_SLEEP_TIME秒スリープしてからリトライ
-        if status_code in API_TEMPORARY_ERRORS:
-            time.sleep(API_SLEEP_TIME)
+        if status_code in EASYPATENT_API_TEMPORARY_ERRORS:
+            time.sleep(EASYPATENT_API_SLEEP_TIME)
             continue
         break
 
     # ステータスコードを確認してエラーの場合にはエラーを投げる
     # 対象とするのはjsonのみ
     if not isinstance(response, requests.Response):
         is_error(response)
@@ -299,17 +299,17 @@
 
     Returns
     -------
     str
         ディレクトリパス文字列
     '''
     if file_type == "zip":
-        dir_name = CONFIG['DirPath']['zip_dir']
+        dir_name = EASYPATENT_CONFIG['DirPath']['zip_dir']
     else:
-        dir_name = CONFIG['DirPath']['data_dir']
+        dir_name = EASYPATENT_CONFIG['DirPath']['data_dir']
     p = pathlib.Path(dir_name)
     if p.is_absolute():
         dir_path = os.path.join(dir_name, law, key, api_type)
     else:
         base_dir = os.path.dirname(__file__)
         dir_path = os.path.join(base_dir, dir_name,law, key, api_type)
     os.makedirs(dir_path, exist_ok=True)
@@ -453,15 +453,15 @@
     >>> file_path = save_json(info, file_dir)
     >>> os.path.exists(file_path)
     True
     '''
     json_path = get_json_path(file_dir)
     now = datetime.datetime.now()
     json_data['ep_data'] = {
-            'create_date': now.strftime(DATETIME_FORMAT),
+            'create_date': now.strftime(EASYPATENT_DATETIME_FORMAT),
             'file_path': json_path,
     }
     with open(json_path, "w") as f:
         json.dump(json_data, f, indent=4)
     return json_path
 
 
@@ -526,15 +526,15 @@
     json_dir = make_dir_path(api_type, key, law, file_type="json")
     json_file = get_json_path(json_dir, non_exist_ok=False)
     if json_file != "":
         now = datetime.datetime.now()
         expire_date = now - datetime.timedelta(days=reget_date)
         with open(json_file) as f:
             json_data = json.load(f)
-        create_date = datetime.datetime.strptime(json_data['ep_data']['create_date'], DATETIME_FORMAT)
+        create_date = datetime.datetime.strptime(json_data['ep_data']['create_date'], EASYPATENT_DATETIME_FORMAT)
         if expire_date < create_date:
              return json_data
     # 既存ファイルがないか、再取得日数を過ぎている場合には、
     # API情報を取得する
     #json_data = func(key)
     if api_type in ["application_reference", "publication_reference","registration_reference"]:
         seed, _ = api_type.split("_")
```

### Comparing `easy_patents-1.0.4/easy_patents/update_authinfo.py` & `easy_patents-1.0.5/easy_patents/update_authinfo.py`

 * *Files 11% similar despite different names*

```diff
@@ -38,7 +38,25 @@
     config["AuthInfo"]["refresh_token"] = "******"
     config["AuthInfo"]["expires_in"] = "1900-01-01 00:00:00"
     config["AuthInfo"]["refresh_expires_in"] = "1900-01-01 00:00:00"
     with open(conf_file, "w") as f:
         config.write(f)
 
 
+def update_deepl_key(display=True):
+    base_dir = os.path.dirname(__file__)
+
+    # userファイルのアップデート
+    user_conf = configparser.ConfigParser()
+    user_file = os.path.join(base_dir, "config/user.ini")
+    user_conf.read(user_file)
+
+    if display:
+        key = input("enter access key: ")
+    else:
+        key = getpass("enter access key: ")
+
+    user_conf["DeepL"] = { 
+            "key": key,
+    }
+    with open(user_file, "w") as f:
+        user_conf.write(f)
```

