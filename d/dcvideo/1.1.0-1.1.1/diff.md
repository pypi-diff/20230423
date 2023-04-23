# Comparing `tmp/dcvideo-1.1.0.tar.gz` & `tmp/dcvideo-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcvideo-1.1.0.tar", last modified: Sun Apr  9 16:30:11 2023, max compression
+gzip compressed data, was "dcvideo-1.1.1.tar", last modified: Sun Apr 23 14:22:34 2023, max compression
```

## Comparing `dcvideo-1.1.0.tar` & `dcvideo-1.1.1.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 netfere    (501) staff       (20)        0 2023-04-09 16:30:11.753178 dcvideo-1.1.0/
--rw-r--r--   0 netfere    (501) staff       (20)      223 2023-04-09 16:30:11.752936 dcvideo-1.1.0/PKG-INFO
-drwxr-xr-x   0 netfere    (501) staff       (20)        0 2023-04-09 16:30:11.750910 dcvideo-1.1.0/dcvideo/
--rw-r--r--   0 netfere    (501) staff       (20)        0 2023-04-02 06:57:57.000000 dcvideo-1.1.0/dcvideo/__init__.py
--rw-r--r--   0 netfere    (501) staff       (20)     5380 2023-04-02 08:30:31.000000 dcvideo-1.1.0/dcvideo/_message.py
--rw-r--r--   0 netfere    (501) staff       (20)      894 2023-04-02 03:47:14.000000 dcvideo-1.1.0/dcvideo/_object.py
--rw-r--r--   0 netfere    (501) staff       (20)      305 2023-04-02 08:30:31.000000 dcvideo-1.1.0/dcvideo/_result.py
--rw-r--r--   0 netfere    (501) staff       (20)    10210 2023-04-02 16:15:46.000000 dcvideo-1.1.0/dcvideo/_youban.py
--rw-r--r--   0 netfere    (501) staff       (20)     3886 2023-04-09 16:30:01.000000 dcvideo-1.1.0/dcvideo/config.py
--rw-r--r--   0 netfere    (501) staff       (20)     6165 2023-04-02 08:30:31.000000 dcvideo-1.1.0/dcvideo/export.py
--rw-r--r--   0 netfere    (501) staff       (20)    11475 2023-04-02 08:30:31.000000 dcvideo-1.1.0/dcvideo/publish.py
--rw-r--r--   0 netfere    (501) staff       (20)     4607 2023-04-02 08:30:31.000000 dcvideo-1.1.0/dcvideo/utils.py
--rw-r--r--   0 netfere    (501) staff       (20)     2536 2023-04-02 12:01:59.000000 dcvideo-1.1.0/dcvideo/web.py
-drwxr-xr-x   0 netfere    (501) staff       (20)        0 2023-04-09 16:30:11.752578 dcvideo-1.1.0/dcvideo.egg-info/
--rw-r--r--   0 netfere    (501) staff       (20)      223 2023-04-09 16:30:11.000000 dcvideo-1.1.0/dcvideo.egg-info/PKG-INFO
--rw-r--r--   0 netfere    (501) staff       (20)      380 2023-04-09 16:30:11.000000 dcvideo-1.1.0/dcvideo.egg-info/SOURCES.txt
--rw-r--r--   0 netfere    (501) staff       (20)        1 2023-04-09 16:30:11.000000 dcvideo-1.1.0/dcvideo.egg-info/dependency_links.txt
--rw-r--r--   0 netfere    (501) staff       (20)      113 2023-04-09 16:30:11.000000 dcvideo-1.1.0/dcvideo.egg-info/entry_points.txt
--rw-r--r--   0 netfere    (501) staff       (20)      122 2023-04-09 16:30:11.000000 dcvideo-1.1.0/dcvideo.egg-info/requires.txt
--rw-r--r--   0 netfere    (501) staff       (20)        8 2023-04-09 16:30:11.000000 dcvideo-1.1.0/dcvideo.egg-info/top_level.txt
--rw-r--r--   0 netfere    (501) staff       (20)       38 2023-04-09 16:30:11.753270 dcvideo-1.1.0/setup.cfg
--rw-r--r--   0 netfere    (501) staff       (20)      813 2023-04-02 07:50:13.000000 dcvideo-1.1.0/setup.py
+drwxr-xr-x   0 netfere    (501) staff       (20)        0 2023-04-23 14:22:34.002905 dcvideo-1.1.1/
+-rw-r--r--   0 netfere    (501) staff       (20)      223 2023-04-23 14:22:34.002643 dcvideo-1.1.1/PKG-INFO
+drwxr-xr-x   0 netfere    (501) staff       (20)        0 2023-04-23 14:22:33.989567 dcvideo-1.1.1/dcvideo/
+-rw-r--r--   0 netfere    (501) staff       (20)        0 2023-04-02 06:57:57.000000 dcvideo-1.1.1/dcvideo/__init__.py
+-rw-r--r--   0 netfere    (501) staff       (20)     5380 2023-04-02 08:30:31.000000 dcvideo-1.1.1/dcvideo/_message.py
+-rw-r--r--   0 netfere    (501) staff       (20)      894 2023-04-02 03:47:14.000000 dcvideo-1.1.1/dcvideo/_object.py
+-rw-r--r--   0 netfere    (501) staff       (20)      305 2023-04-02 08:30:31.000000 dcvideo-1.1.1/dcvideo/_result.py
+-rw-r--r--   0 netfere    (501) staff       (20)    10210 2023-04-02 16:15:46.000000 dcvideo-1.1.1/dcvideo/_youban.py
+-rw-r--r--   0 netfere    (501) staff       (20)     6195 2023-04-21 18:05:46.000000 dcvideo-1.1.1/dcvideo/alioss.py
+-rw-r--r--   0 netfere    (501) staff       (20)     4936 2023-04-23 14:16:28.000000 dcvideo-1.1.1/dcvideo/config.py
+-rw-r--r--   0 netfere    (501) staff       (20)     6153 2023-04-23 14:11:16.000000 dcvideo-1.1.1/dcvideo/export.py
+-rw-r--r--   0 netfere    (501) staff       (20)    11430 2023-04-23 13:35:04.000000 dcvideo-1.1.1/dcvideo/publish.py
+-rw-r--r--   0 netfere    (501) staff       (20)     4607 2023-04-21 17:41:05.000000 dcvideo-1.1.1/dcvideo/utils.py
+-rw-r--r--   0 netfere    (501) staff       (20)     2536 2023-04-02 12:01:59.000000 dcvideo-1.1.1/dcvideo/web.py
+drwxr-xr-x   0 netfere    (501) staff       (20)        0 2023-04-23 14:22:34.002285 dcvideo-1.1.1/dcvideo.egg-info/
+-rw-r--r--   0 netfere    (501) staff       (20)      223 2023-04-23 14:22:33.000000 dcvideo-1.1.1/dcvideo.egg-info/PKG-INFO
+-rw-r--r--   0 netfere    (501) staff       (20)      398 2023-04-23 14:22:33.000000 dcvideo-1.1.1/dcvideo.egg-info/SOURCES.txt
+-rw-r--r--   0 netfere    (501) staff       (20)        1 2023-04-23 14:22:33.000000 dcvideo-1.1.1/dcvideo.egg-info/dependency_links.txt
+-rw-r--r--   0 netfere    (501) staff       (20)      113 2023-04-23 14:22:33.000000 dcvideo-1.1.1/dcvideo.egg-info/entry_points.txt
+-rw-r--r--   0 netfere    (501) staff       (20)      135 2023-04-23 14:22:33.000000 dcvideo-1.1.1/dcvideo.egg-info/requires.txt
+-rw-r--r--   0 netfere    (501) staff       (20)        8 2023-04-23 14:22:33.000000 dcvideo-1.1.1/dcvideo.egg-info/top_level.txt
+-rw-r--r--   0 netfere    (501) staff       (20)       38 2023-04-23 14:22:34.002998 dcvideo-1.1.1/setup.cfg
+-rw-r--r--   0 netfere    (501) staff       (20)      833 2023-04-21 13:30:03.000000 dcvideo-1.1.1/setup.py
```

### Comparing `dcvideo-1.1.0/dcvideo/_message.py` & `dcvideo-1.1.1/dcvideo/_message.py`

 * *Files identical despite different names*

### Comparing `dcvideo-1.1.0/dcvideo/_object.py` & `dcvideo-1.1.1/dcvideo/_object.py`

 * *Files identical despite different names*

### Comparing `dcvideo-1.1.0/dcvideo/_youban.py` & `dcvideo-1.1.1/dcvideo/_youban.py`

 * *Files identical despite different names*

### Comparing `dcvideo-1.1.0/dcvideo/config.py` & `dcvideo-1.1.1/dcvideo/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import re
 from tkinter import filedialog
 from .utils import port_is_used,get_host_ip
 
 filepath = os.path.join(os.path.dirname(__file__), 'config.ini')
 config = configparser.ConfigParser()
-VERSION = '1.1.0'
+VERSION = '1.1.1'
 HOST = 'https://www.shortvideo.work'
 
 def save_config(section,key,value):
     config.read(filepath)
     if not config.has_section(section):
         config.add_section(section)
     config.set(section, key, value)
@@ -81,14 +81,42 @@
                 config.set(key, 'workdir', value)
                 config.write(open(filepath, "w"))
                 break
         else:
             break
     return workdir
 
+def read_alioss():
+    config.read(filepath)
+    if not config.has_section('alioss'):
+        config.add_section("alioss")
+    access_key_id = config.get('alioss', 'access_key_id', fallback='')
+    access_secret = config.get('alioss', 'access_secret', fallback='')
+    bucket = config.get('alioss', 'bucket', fallback='')
+
+    if not access_key_id:
+        access_key_id = input('\n请输入阿里云OSS的access_key_id：')
+        if access_key_id:
+            config.set('alioss', 'access_key_id', access_key_id)
+            config.write(open(filepath, "w"))
+
+    if not access_secret:
+        access_secret = input('\n请输入阿里云OSS的access_secret：')
+        if access_secret:
+            config.set('alioss', 'access_secret', access_secret)
+            config.write(open(filepath, "w"))
+
+    if not bucket:
+        bucket = input('\n请输入阿里云OSS的bucket：')
+        if bucket:
+            config.set('alioss', 'bucket', bucket)
+            config.write(open(filepath, "w"))
+
+    return (access_key_id,access_secret,bucket)
+
 def read_web():
     if not os.path.exists(filepath):
         config.add_section("video")
         config.set("video", "version", VERSION)
         config.set("video", "desc", "请不在擅自修改配置文件，以免引发异常！")
         config.write(open(filepath, "w"))
```

### Comparing `dcvideo-1.1.0/dcvideo/export.py` & `dcvideo-1.1.1/dcvideo/export.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,15 @@
                 await self.download(ExportMessage(**data))
             except Exception as e:
                 print(str(e))
 
         return Result(True, wait=5)
         
     async def download(self, message: ExportMessage):
+        
         message.console_title()
 
         savepath = os.path.join(self.workdir, ymd(), message.category)
         os.makedirs(savepath, exist_ok=True)
 
         def remove_file(path):
             if os.path.exists(path):
@@ -55,15 +56,15 @@
             if os.path.exists(filepath) and md5_value(filepath) != file.md5:
                 file.local_path = filepath
                 message.setFileDown(file, 100)
             else:
                 success = await download(filepath, file.src, lambda p, s, t: message.setFileDown(file, p))
                 if success:
                     if md5_value(filepath) != file.md5:
-                        error = file.label + ' 文件尺寸不一致'
+                        error = file.label + ' 文件不一致'
                         remove_file(filepath)
                         break
                     else:
                         file.local_path = filepath
                 else:
                     error = file.label+' 下载失败'
                     remove_file(filepath)
@@ -75,15 +76,15 @@
                 print(f'\n\t{error}，5秒后尝试第{message.retried+1}次重试')
                 await asyncio.sleep(5)
                 return await self.download(message)
             print(f'\n\t{error}')
             await self.query('/publish/export?action=update',_id=message._id, status='error', error=error)
             return False
         else:
-            print(f'\n\t\033[32m导出完成\033[0m')
+            print(f'\n\t导出完成')
             await self.query('/publish/export?action=update',_id=message._id, status='success')
             return True
 
     async def query(self, url: str, **kwargs):
         sign, nonce = sign_dict(kwargs, self.appsecret)
 
         url = f'{self.host}{url}&appid={self.appid}&nonce={nonce}&sign={sign}&version={self.version}'
```

### Comparing `dcvideo-1.1.0/dcvideo/publish.py` & `dcvideo-1.1.1/dcvideo/publish.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,19 +149,19 @@
 
             payload = message.payload
             if message.category.platform == 'tp':
                 payload['substance_cateid'] = '混剪'
 
             res = await youban.web_submit(message.files[0].local_path, payload)
             if res.success:
-                print(f'\n\t\033[32m发布成功\033[0m')
+                print(f'\n\t发布成功')
                 await self.update(message._id, 'completed', 'publish', title=message.value.title)
                 self.remove_local_files(message)
             else:
-                print(f'\n\t\033[31m{res.msg}\033[0m')
+                print(f'\n\t{res.msg}')
                 await self.update(message._id, 'completed', 'error', message=res.msg)
 
     async def api_publish(self, message: Message):
         error = ''
         youban = Youban(message.category.platform, message.account)
         # 文件上传到cos
         for file in message.files:
@@ -194,15 +194,15 @@
             try:
                 Location = message.video_cos.get('Location')
                 await self.update(message._id, 'publishing', 'uploaded', location=Location)
             except:
                 pass
             res = await youban.api_submit(message.payload)
             if res.success:
-                print(f'\n\t\033[32m发布成功\033[0m')
+                print(f'\n\t发布成功')
                 await self.update(message._id, 'completed', 'publish', title=message.value.title)
                 self.remove_local_files(message)
             else:
                 print(f'\n\t{res.msg}')
                 await self.update(message._id, 'completed', 'error', message=res.msg)
 
     async def update(self, _id: str, status: str, childStatus: str, title: str = None, message: str = None, location: str = None):
```

### Comparing `dcvideo-1.1.0/dcvideo/utils.py` & `dcvideo-1.1.1/dcvideo/utils.py`

 * *Files identical despite different names*

### Comparing `dcvideo-1.1.0/dcvideo/web.py` & `dcvideo-1.1.1/dcvideo/web.py`

 * *Files identical despite different names*

### Comparing `dcvideo-1.1.0/setup.py` & `dcvideo-1.1.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 requires = [
     "requests==2.28.1",
     "requests_toolbelt==0.9.1",
     "cos_python_sdk_v5==1.9.21",
     "fake_useragent==1.1.1",
     "flask==2.2.3",
     "flask-cors==3.0.10",
+    "oss2==2.16.0"
 ]
 
 
 setup(
     name='dcvideo', 
     version=VERSION,
     description='', 
@@ -25,8 +26,8 @@
     entry_points={
         'console_scripts':[
             'video-pub = dcvideo.publish:main',
             'video-exp = dcvideo.export:main',
             'video-web = dcvideo.web:main'
         ]
     },
-)
+)
```

