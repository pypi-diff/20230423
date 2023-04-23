# Comparing `tmp/pynocaptcha-1.4.1.tar.gz` & `tmp/pynocaptcha-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pynocaptcha-1.4.1.tar", last modified: Mon Apr 10 09:55:59 2023, max compression
+gzip compressed data, was "dist/pynocaptcha-1.4.2.tar", last modified: Sun Apr 23 10:24:12 2023, max compression
```

## Comparing `pynocaptcha-1.4.1.tar` & `pynocaptcha-1.4.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-04-10 09:55:59.000000 pynocaptcha-1.4.1/
--rw-r--r--   0 esbiya     (501) staff       (20)      566 2023-04-10 09:55:59.000000 pynocaptcha-1.4.1/PKG-INFO
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-04-10 09:55:59.000000 pynocaptcha-1.4.1/pynocaptcha/
--rw-r--r--   0 esbiya     (501) staff       (20)      440 2023-04-04 08:12:16.000000 pynocaptcha-1.4.1/pynocaptcha/__init__.py
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-04-10 09:55:59.000000 pynocaptcha-1.4.1/pynocaptcha/crackers/
--rw-r--r--   0 esbiya     (501) staff       (20)     4243 2023-04-10 09:54:53.000000 pynocaptcha-1.4.1/pynocaptcha/crackers/base.py
--rw-r--r--   0 esbiya     (501) staff       (20)     5440 2023-04-10 09:55:20.000000 pynocaptcha-1.4.1/pynocaptcha/crackers/cloudflare.py
--rw-r--r--   0 esbiya     (501) staff       (20)     1339 2023-04-05 02:45:58.000000 pynocaptcha-1.4.1/pynocaptcha/crackers/hcaptcha.py
--rw-r--r--   0 esbiya     (501) staff       (20)     1454 2023-04-10 03:49:32.000000 pynocaptcha-1.4.1/pynocaptcha/crackers/incapsula.py
--rw-r--r--   0 esbiya     (501) staff       (20)     2893 2023-03-24 04:08:51.000000 pynocaptcha-1.4.1/pynocaptcha/crackers/recaptcha.py
--rw-r--r--   0 esbiya     (501) staff       (20)      846 2023-04-10 09:55:49.000000 pynocaptcha-1.4.1/setup.py
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-04-23 10:24:12.000000 pynocaptcha-1.4.2/
+-rw-r--r--   0 esbiya     (501) staff       (20)      566 2023-04-23 10:24:12.000000 pynocaptcha-1.4.2/PKG-INFO
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-04-23 10:24:12.000000 pynocaptcha-1.4.2/pynocaptcha/
+-rw-r--r--   0 esbiya     (501) staff       (20)      508 2023-04-23 09:05:33.000000 pynocaptcha-1.4.2/pynocaptcha/__init__.py
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-04-23 10:24:12.000000 pynocaptcha-1.4.2/pynocaptcha/crackers/
+-rw-r--r--   0 esbiya     (501) staff       (20)      722 2023-04-23 09:55:53.000000 pynocaptcha-1.4.2/pynocaptcha/crackers/akamai.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     4430 2023-04-23 10:23:31.000000 pynocaptcha-1.4.2/pynocaptcha/crackers/base.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     5186 2023-04-23 09:01:32.000000 pynocaptcha-1.4.2/pynocaptcha/crackers/cloudflare.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     1339 2023-04-05 02:45:58.000000 pynocaptcha-1.4.2/pynocaptcha/crackers/hcaptcha.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     1454 2023-04-10 03:49:32.000000 pynocaptcha-1.4.2/pynocaptcha/crackers/incapsula.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     2449 2023-04-23 08:59:52.000000 pynocaptcha-1.4.2/pynocaptcha/crackers/recaptcha.py
+-rw-r--r--   0 esbiya     (501) staff       (20)      846 2023-04-23 09:07:34.000000 pynocaptcha-1.4.2/setup.py
```

### Comparing `pynocaptcha-1.4.1/PKG-INFO` & `pynocaptcha-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pynocaptcha
-Version: 1.4.1
+Version: 1.4.2
 Summary: nocaptcha.io api
 Home-page: UNKNOWN
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: MIT
 Description: nocaptcha.io python api
 Keywords: nocaptcha
```

### Comparing `pynocaptcha-1.4.1/pynocaptcha/crackers/base.py` & `pynocaptcha-1.4.2/pynocaptcha/crackers/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 
 import requests
-import traceback
 from loguru import logger
 from typing import Any
 
 
 class BaseCracker:
     
     # 破解器
@@ -28,42 +27,46 @@
         developer_id: str = None,   
         user_agent: str = None,
         proxy: str = None, 
         timeout: int = 30,
         debug: bool = False,
         check_useful: bool = False,
         max_retry_times: int = 3,
-        internal_proxy=True,
+        internal=True,
+        show_ad=True,
         **kwargs
     ) -> None:
         """
         :param user_token: nocaptcha.io 用户 token
         :param developer_id: nocaptcha.io 用户上级代理 token
         :param user_agent: 请求流程使用 ua
         :param proxy: 请求流程代理, 不传默认使用系统代理, 某些强制要求代理一致或者特定区域的站点请传代理, 支持协议 http/https/socks5, 代理格式: {protocol}://{ip}:{port}（如有账号验证：{protocol}://{user}:{password}@{ip}:{port}）
         :param timeout: 破解接口超时时间(秒)
         :param debug: 是否开启 debug 模式
         :param check_useful: 检查破解是否成功
         :param max_retry_times: 最大重试次数
-        :param internal_proxy: 是否使用国内代理
+        :param internal: 是否使用国内代理
         """
+        if show_ad:
+            logger.debug("感谢选择 nocaptcha, 我们只做别人做不到的(手动狗头)~")
+            logger.debug("欢迎推荐注册, 官网地址: https://www.nocaptcha.io/")
         self.user_token = user_token
         if not self.user_token:
             raise Exception("缺少用户凭证")
         self.developer_id = developer_id
         self.user_agent = user_agent
         self.proxy = proxy
         self.timeout = timeout
         self.debug = debug
         self.check_useful = check_useful
         self.retry_times = 0
         self.max_retry_times = max_retry_times
 
         self.wanda_args = {
-            "internal_proxy": internal_proxy
+            "internal": internal
         }
         for k in self.must_check_params:
             v = kwargs.get(k)
             setattr(self, k, v)
             self.wanda_args.update({ k: v })
         for k, v in self.option_params.items():
             _v = kwargs.get(k, v)
```

### Comparing `pynocaptcha-1.4.1/pynocaptcha/crackers/cloudflare.py` & `pynocaptcha-1.4.2/pynocaptcha/crackers/cloudflare.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     """
     cloudflare cracker
     :param href: 触发 cloudfalre 验证的首页地址
     :param user_agent: 请求流程使用 ua, 必须使用 MacOS Firefox User-Agent, 否则可能破解失败
     :param html: 触发 cloudflare 验证的响应源码, 特征: window._cf_chl_opt=.../window["CF$params"]=...
     :param cookies: 触发验证必须的 cookies, 默认 {} 
     :param ja3: 请求客户端使用的 ja3 指纹, 例如: "771,4865-4867-4866-49195-49199-52393-52392-49196-49200-49162-49161-49171-49172-156-157-47-53,0-23-65281-10-11-35-16-5-34-51-43-13-45-28-21,29-23-24-25-256-257,0", 不传则默认使用随机 ja3 指纹, 可通过 https://tls.peet.ws/api/clean 查询你的请求客户端的 tls 指纹, 然后填入返回的 ja3 字段值, 则我们的破解流程将会使用你上传的 ja3 指纹, 从而保持 tls 指纹一致
-    :param auto_alpha: 是否自动过成功进入首页后继续触发的第二层 alpha 验证, 过掉该验证会成功获取一个 __cf_bm 的 cookie
     调用示例:
     cracker = CloudFlareCracker(
         href=href,
         user_token="xxx",
 
         # debug=True,
         # check_useful=True,
@@ -40,18 +39,15 @@
     # 默认可选参数
     option_params = {
         "user_agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10.15; rv:109.0) Gecko/20100101 Firefox/110.0",
         "html": "",
         "headers": {},
         "cookies": {},
         "ja3": "",
-        "auto_alpha": True
     }
-    # 需要删除的多余参数
-    delete_params = ["internal_proxy"]
 
     @staticmethod
     def parse_proxy(proxy):
         _auth, _proxy = None, None
         if proxy:
             _proxy = proxy.split("/")[-1]
             if "@" in _proxy:
```

### Comparing `pynocaptcha-1.4.1/pynocaptcha/crackers/hcaptcha.py` & `pynocaptcha-1.4.2/pynocaptcha/crackers/hcaptcha.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.4.1/pynocaptcha/crackers/incapsula.py` & `pynocaptcha-1.4.2/pynocaptcha/crackers/incapsula.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.4.1/setup.py` & `pynocaptcha-1.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 
 from distutils.core import setup
 
 
 setup(
     name='pynocaptcha',
-    version='1.4.1',
+    version='1.4.2',
     description='nocaptcha.io api',
     long_description='nocaptcha.io python api',
     install_requires=["pyhttpx", "loguru"],
     license='MIT',
     packages=["pynocaptcha/crackers", "pynocaptcha"],
     package_dir={'pynocaptcha': 'pynocaptcha'},
     platforms=["all"],
```

