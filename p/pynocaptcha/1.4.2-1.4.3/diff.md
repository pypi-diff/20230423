# Comparing `tmp/pynocaptcha-1.4.2.tar.gz` & `tmp/pynocaptcha-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pynocaptcha-1.4.2.tar", last modified: Sun Apr 23 10:24:12 2023, max compression
+gzip compressed data, was "dist/pynocaptcha-1.4.3.tar", last modified: Sun Apr 23 14:45:48 2023, max compression
```

## Comparing `pynocaptcha-1.4.2.tar` & `pynocaptcha-1.4.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-04-23 10:24:12.000000 pynocaptcha-1.4.2/
--rw-r--r--   0 esbiya     (501) staff       (20)      566 2023-04-23 10:24:12.000000 pynocaptcha-1.4.2/PKG-INFO
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-04-23 10:24:12.000000 pynocaptcha-1.4.2/pynocaptcha/
--rw-r--r--   0 esbiya     (501) staff       (20)      508 2023-04-23 09:05:33.000000 pynocaptcha-1.4.2/pynocaptcha/__init__.py
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-04-23 10:24:12.000000 pynocaptcha-1.4.2/pynocaptcha/crackers/
--rw-r--r--   0 esbiya     (501) staff       (20)      722 2023-04-23 09:55:53.000000 pynocaptcha-1.4.2/pynocaptcha/crackers/akamai.py
--rw-r--r--   0 esbiya     (501) staff       (20)     4430 2023-04-23 10:23:31.000000 pynocaptcha-1.4.2/pynocaptcha/crackers/base.py
--rw-r--r--   0 esbiya     (501) staff       (20)     5186 2023-04-23 09:01:32.000000 pynocaptcha-1.4.2/pynocaptcha/crackers/cloudflare.py
--rw-r--r--   0 esbiya     (501) staff       (20)     1339 2023-04-05 02:45:58.000000 pynocaptcha-1.4.2/pynocaptcha/crackers/hcaptcha.py
--rw-r--r--   0 esbiya     (501) staff       (20)     1454 2023-04-10 03:49:32.000000 pynocaptcha-1.4.2/pynocaptcha/crackers/incapsula.py
--rw-r--r--   0 esbiya     (501) staff       (20)     2449 2023-04-23 08:59:52.000000 pynocaptcha-1.4.2/pynocaptcha/crackers/recaptcha.py
--rw-r--r--   0 esbiya     (501) staff       (20)      846 2023-04-23 09:07:34.000000 pynocaptcha-1.4.2/setup.py
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-04-23 14:45:48.000000 pynocaptcha-1.4.3/
+-rw-r--r--   0 esbiya     (501) staff       (20)      566 2023-04-23 14:45:48.000000 pynocaptcha-1.4.3/PKG-INFO
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-04-23 14:45:48.000000 pynocaptcha-1.4.3/pynocaptcha/
+-rw-r--r--   0 esbiya     (501) staff       (20)      508 2023-04-23 09:05:33.000000 pynocaptcha-1.4.3/pynocaptcha/__init__.py
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-04-23 14:45:48.000000 pynocaptcha-1.4.3/pynocaptcha/crackers/
+-rw-r--r--   0 esbiya     (501) staff       (20)      722 2023-04-23 09:55:53.000000 pynocaptcha-1.4.3/pynocaptcha/crackers/akamai.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     4505 2023-04-23 14:44:09.000000 pynocaptcha-1.4.3/pynocaptcha/crackers/base.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     5186 2023-04-23 09:01:32.000000 pynocaptcha-1.4.3/pynocaptcha/crackers/cloudflare.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     1339 2023-04-05 02:45:58.000000 pynocaptcha-1.4.3/pynocaptcha/crackers/hcaptcha.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     1488 2023-04-23 14:39:24.000000 pynocaptcha-1.4.3/pynocaptcha/crackers/incapsula.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     2449 2023-04-23 08:59:52.000000 pynocaptcha-1.4.3/pynocaptcha/crackers/recaptcha.py
+-rw-r--r--   0 esbiya     (501) staff       (20)      846 2023-04-23 14:39:38.000000 pynocaptcha-1.4.3/setup.py
```

### Comparing `pynocaptcha-1.4.2/PKG-INFO` & `pynocaptcha-1.4.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pynocaptcha
-Version: 1.4.2
+Version: 1.4.3
 Summary: nocaptcha.io api
 Home-page: UNKNOWN
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: MIT
 Description: nocaptcha.io python api
 Keywords: nocaptcha
```

### Comparing `pynocaptcha-1.4.2/pynocaptcha/crackers/akamai.py` & `pynocaptcha-1.4.3/pynocaptcha/crackers/akamai.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.4.2/pynocaptcha/crackers/base.py` & `pynocaptcha-1.4.3/pynocaptcha/crackers/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,17 +61,18 @@
         self.retry_times = 0
         self.max_retry_times = max_retry_times
 
         self.wanda_args = {
             "internal": internal
         }
         for k in self.must_check_params:
-            v = kwargs.get(k)
-            setattr(self, k, v)
-            self.wanda_args.update({ k: v })
+            _v = kwargs.get(k, v)
+            if not hasattr(self, k) or getattr(self, k) is None:
+                setattr(self, k, _v)
+            self.wanda_args.update({ k: _v })
         for k, v in self.option_params.items():
             _v = kwargs.get(k, v)
             if not hasattr(self, k) or getattr(self, k) is None:
                 setattr(self, k, _v)
             self.wanda_args.update({ k: _v })
         
         for k in self.delete_params:
```

### Comparing `pynocaptcha-1.4.2/pynocaptcha/crackers/cloudflare.py` & `pynocaptcha-1.4.3/pynocaptcha/crackers/cloudflare.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.4.2/pynocaptcha/crackers/hcaptcha.py` & `pynocaptcha-1.4.3/pynocaptcha/crackers/hcaptcha.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.4.2/pynocaptcha/crackers/incapsula.py` & `pynocaptcha-1.4.3/pynocaptcha/crackers/incapsula.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,29 +12,31 @@
     incapsula cracker
     :param href: 触发 incapsula 盾验证的首页地址
     :param user_agent: 请求流程使用 ua, 必须使用 MacOS Firefox User-Agent, 否则可能破解失败
     :param submit: 是否提交验证接口, 不提交则返回计算参数
     调用示例:
     cracker = IncapsulaCracker(
         href=href,
+        user_agent='Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/108.0.0.0 Safari/537.36',
+
         user_token="xxx",
 
         # debug=True,
         # check_useful=True,
         # proxy=proxy,
         # submit=False
     )
     ret = cracker.crack()
     """
     
     # 必传参数
-    must_check_params = ["href"]
+    must_check_params = ["href", "user_agent"]
     # 默认可选参数
     option_params = {
-        "user_agent": 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/108.0.0.0 Safari/537.36',
+        "script": "",
         "submit": True,
     }
     
     def check(self, cookies):
         headers = {
             'upgrade-insecure-requests': '1',
             'user-agent': self.user_agent,
```

### Comparing `pynocaptcha-1.4.2/pynocaptcha/crackers/recaptcha.py` & `pynocaptcha-1.4.3/pynocaptcha/crackers/recaptcha.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.4.2/setup.py` & `pynocaptcha-1.4.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 
 from distutils.core import setup
 
 
 setup(
     name='pynocaptcha',
-    version='1.4.2',
+    version='1.4.3',
     description='nocaptcha.io api',
     long_description='nocaptcha.io python api',
     install_requires=["pyhttpx", "loguru"],
     license='MIT',
     packages=["pynocaptcha/crackers", "pynocaptcha"],
     package_dir={'pynocaptcha': 'pynocaptcha'},
     platforms=["all"],
```

