# Comparing `tmp/zcbot-celery-sdk-0.0.8.tar.gz` & `tmp/zcbot-celery-sdk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\zcbot-celery-sdk-0.0.8.tar", last modified: Thu Mar 16 03:17:25 2023, max compression
+gzip compressed data, was "dist\zcbot-celery-sdk-0.0.9.tar", last modified: Thu Mar 16 03:30:57 2023, max compression
```

## Comparing `zcbot-celery-sdk-0.0.8.tar` & `zcbot-celery-sdk-0.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-03-16 03:17:25.971374 zcbot-celery-sdk-0.0.8/
--rw-rw-rw-   0        0        0        0 2023-03-14 04:29:15.000000 zcbot-celery-sdk-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0      379 2023-03-16 03:17:25.970374 zcbot-celery-sdk-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      135 2023-03-16 02:53:02.000000 zcbot-celery-sdk-0.0.8/README.rst
--rw-rw-rw-   0        0        0       42 2023-03-16 03:17:25.971374 zcbot-celery-sdk-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      599 2023-03-16 03:17:20.000000 zcbot-celery-sdk-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-16 03:17:25.949375 zcbot-celery-sdk-0.0.8/zcbot_celery_sdk/
--rw-rw-rw-   0        0        0       40 2023-03-14 03:58:21.000000 zcbot-celery-sdk-0.0.8/zcbot_celery_sdk/__init__.py
--rw-rw-rw-   0        0        0     5215 2023-03-16 03:05:16.000000 zcbot-celery-sdk-0.0.8/zcbot_celery_sdk/client.py
-drwxrwxrwx   0        0        0        0 2023-03-16 03:17:25.964376 zcbot-celery-sdk-0.0.8/zcbot_celery_sdk/common/
--rw-rw-rw-   0        0        0       40 2023-03-14 03:58:21.000000 zcbot-celery-sdk-0.0.8/zcbot_celery_sdk/common/__init__.py
--rw-rw-rw-   0        0        0      272 2022-04-08 15:27:48.000000 zcbot-celery-sdk-0.0.8/zcbot_celery_sdk/common/decator.py
--rw-rw-rw-   0        0        0      705 2022-08-22 07:41:36.000000 zcbot-celery-sdk-0.0.8/zcbot_celery_sdk/common/exceptions.py
--rw-rw-rw-   0        0        0      423 2022-12-19 10:07:28.000000 zcbot-celery-sdk-0.0.8/zcbot_celery_sdk/common/keys.py
--rw-rw-rw-   0        0        0     1290 2023-03-15 08:30:09.000000 zcbot-celery-sdk-0.0.8/zcbot_celery_sdk/common/model.py
--rw-rw-rw-   0        0        0     2132 2023-03-15 06:40:08.000000 zcbot-celery-sdk-0.0.8/zcbot_celery_sdk/common/thread_pool.py
--rw-rw-rw-   0        0        0     3138 2022-12-19 10:07:28.000000 zcbot-celery-sdk-0.0.8/zcbot_celery_sdk/common/utils.py
--rw-rw-rw-   0        0        0     2894 2023-03-15 09:18:37.000000 zcbot-celery-sdk-0.0.8/zcbot_celery_sdk/monitor.py
-drwxrwxrwx   0        0        0        0 2023-03-16 03:17:25.969376 zcbot-celery-sdk-0.0.8/zcbot_celery_sdk/service/
--rw-rw-rw-   0        0        0        0 2023-03-14 05:49:28.000000 zcbot-celery-sdk-0.0.8/zcbot_celery_sdk/service/__init__.py
--rw-rw-rw-   0        0        0     1678 2023-03-16 02:17:29.000000 zcbot-celery-sdk-0.0.8/zcbot_celery_sdk/service/base.py
--rw-rw-rw-   0        0        0     1568 2023-03-16 02:30:41.000000 zcbot-celery-sdk-0.0.8/zcbot_celery_sdk/service/sku_search.py
--rw-rw-rw-   0        0        0      565 2023-03-16 02:29:58.000000 zcbot-celery-sdk-0.0.8/zcbot_celery_sdk/service/tax.py
-drwxrwxrwx   0        0        0        0 2023-03-16 03:17:25.955375 zcbot-celery-sdk-0.0.8/zcbot_celery_sdk.egg-info/
--rw-rw-rw-   0        0        0      379 2023-03-16 03:17:25.000000 zcbot-celery-sdk-0.0.8/zcbot_celery_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      701 2023-03-16 03:17:25.000000 zcbot-celery-sdk-0.0.8/zcbot_celery_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-16 03:17:25.000000 zcbot-celery-sdk-0.0.8/zcbot_celery_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-03-16 03:17:25.000000 zcbot-celery-sdk-0.0.8/zcbot_celery_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-03-16 03:17:25.000000 zcbot-celery-sdk-0.0.8/zcbot_celery_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-03-16 03:30:57.641530 zcbot-celery-sdk-0.0.9/
+-rw-rw-rw-   0        0        0        0 2023-03-14 04:29:15.000000 zcbot-celery-sdk-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      379 2023-03-16 03:30:57.640532 zcbot-celery-sdk-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      135 2023-03-16 02:53:02.000000 zcbot-celery-sdk-0.0.9/README.rst
+-rw-rw-rw-   0        0        0       42 2023-03-16 03:30:57.641530 zcbot-celery-sdk-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      599 2023-03-16 03:30:51.000000 zcbot-celery-sdk-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-16 03:30:57.616531 zcbot-celery-sdk-0.0.9/zcbot_celery_sdk/
+-rw-rw-rw-   0        0        0       40 2023-03-14 03:58:21.000000 zcbot-celery-sdk-0.0.9/zcbot_celery_sdk/__init__.py
+-rw-rw-rw-   0        0        0     5634 2023-03-16 03:28:43.000000 zcbot-celery-sdk-0.0.9/zcbot_celery_sdk/client.py
+drwxrwxrwx   0        0        0        0 2023-03-16 03:30:57.633533 zcbot-celery-sdk-0.0.9/zcbot_celery_sdk/common/
+-rw-rw-rw-   0        0        0       40 2023-03-14 03:58:21.000000 zcbot-celery-sdk-0.0.9/zcbot_celery_sdk/common/__init__.py
+-rw-rw-rw-   0        0        0      272 2022-04-08 15:27:48.000000 zcbot-celery-sdk-0.0.9/zcbot_celery_sdk/common/decator.py
+-rw-rw-rw-   0        0        0      705 2022-08-22 07:41:36.000000 zcbot-celery-sdk-0.0.9/zcbot_celery_sdk/common/exceptions.py
+-rw-rw-rw-   0        0        0      423 2022-12-19 10:07:28.000000 zcbot-celery-sdk-0.0.9/zcbot_celery_sdk/common/keys.py
+-rw-rw-rw-   0        0        0     1290 2023-03-15 08:30:09.000000 zcbot-celery-sdk-0.0.9/zcbot_celery_sdk/common/model.py
+-rw-rw-rw-   0        0        0     2132 2023-03-15 06:40:08.000000 zcbot-celery-sdk-0.0.9/zcbot_celery_sdk/common/thread_pool.py
+-rw-rw-rw-   0        0        0     3138 2022-12-19 10:07:28.000000 zcbot-celery-sdk-0.0.9/zcbot_celery_sdk/common/utils.py
+-rw-rw-rw-   0        0        0     2894 2023-03-15 09:18:37.000000 zcbot-celery-sdk-0.0.9/zcbot_celery_sdk/monitor.py
+drwxrwxrwx   0        0        0        0 2023-03-16 03:30:57.638533 zcbot-celery-sdk-0.0.9/zcbot_celery_sdk/service/
+-rw-rw-rw-   0        0        0        0 2023-03-14 05:49:28.000000 zcbot-celery-sdk-0.0.9/zcbot_celery_sdk/service/__init__.py
+-rw-rw-rw-   0        0        0     1678 2023-03-16 02:17:29.000000 zcbot-celery-sdk-0.0.9/zcbot_celery_sdk/service/base.py
+-rw-rw-rw-   0        0        0     1568 2023-03-16 02:30:41.000000 zcbot-celery-sdk-0.0.9/zcbot_celery_sdk/service/sku_search.py
+-rw-rw-rw-   0        0        0      565 2023-03-16 02:29:58.000000 zcbot-celery-sdk-0.0.9/zcbot_celery_sdk/service/tax.py
+drwxrwxrwx   0        0        0        0 2023-03-16 03:30:57.623533 zcbot-celery-sdk-0.0.9/zcbot_celery_sdk.egg-info/
+-rw-rw-rw-   0        0        0      379 2023-03-16 03:30:57.000000 zcbot-celery-sdk-0.0.9/zcbot_celery_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      701 2023-03-16 03:30:57.000000 zcbot-celery-sdk-0.0.9/zcbot_celery_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-16 03:30:57.000000 zcbot-celery-sdk-0.0.9/zcbot_celery_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-03-16 03:30:57.000000 zcbot-celery-sdk-0.0.9/zcbot_celery_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-03-16 03:30:57.000000 zcbot-celery-sdk-0.0.9/zcbot_celery_sdk.egg-info/top_level.txt
```

### Comparing `zcbot-celery-sdk-0.0.8/setup.py` & `zcbot-celery-sdk-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 with open('README.rst', 'r') as f:
     long_description = f.read()
 
 setup(name='zcbot-celery-sdk',
-      version='0.0.8',
+      version='0.0.9',
       description='zcbot celery sdk for zsodata',
       long_description=long_description,
       author='zsodata',
       author_email='team@zso.io',
       url='http://www.zsodata.com',
       install_requires=['celery', 'redis'],
       python_requires='>=3.7',
```

### Comparing `zcbot-celery-sdk-0.0.8/zcbot_celery_sdk/client.py` & `zcbot-celery-sdk-0.0.9/zcbot_celery_sdk/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -35,16 +35,23 @@
         self.task_map = dict()
 
     # 异步结果处理函数绑定
     def _bind_callback(self, task_name: str, async_result: AsyncResult, callback: Callback):
         rs_key = get_result_key(app_code=self.app_code, task_name=task_name, task_id=async_result.id)
         self.rds_client.set(rs_key, callback.json(), ex=self.default_expire_seconds)
 
-    # 异步请求
     def apply_async(self, task_name: str, task_params: Dict = None, callback: Callback = None, **kwargs):
+        """
+        异步请求
+        :param task_name: 任务名
+        :param task_params: 任务参数
+        :param callback: 回调对象
+        :param kwargs: 扩展参数
+        :return:
+        """
         LOGGER.info(f'[服务]异步调用 task={task_name}')
         try:
             _headers = dict()
             if callback:
                 _headers.update(callback.dict())
             _headers['app_code'] = _headers.get('app_code', None) or self.app_code
 
@@ -53,26 +60,34 @@
             # 绑定回调处理函数
             self._bind_callback(task_name, async_result, callback)
             return async_result
         except Exception as e:
             LOGGER.error(f'处理异常: task_name={task_name}, kwargs={task_params}, callback={callback}, e={e}')
             raise e
 
-    # 同步请求
     def apply_sync(self, task_name: str, task_params: Dict = None, **kwargs):
+        """
+        同步请求
+        :param task_name: 任务名
+        :param task_params: 任务参数
+        :param kwargs: 扩展参数
+        :return:
+        """
         LOGGER.info(f'[服务]同步调用 task={task_name}')
         try:
             _headers = {'app_code': self.app_code}
             # 异步调用
             async_result = self._get_task(task_name).apply_async(kwargs=task_params, queue=f'task.{task_name}', headers=_headers)
             # 等待结果
             _timeout = 60
             if kwargs and kwargs.get('timeout', None):
                 _timeout = float(kwargs.get('timeout'))
-            return async_result.get(timeout=_timeout)
+            rs = async_result.get(timeout=_timeout)
+            async_result.forget()
+            return rs
         except Exception as e:
             LOGGER.error(f'处理异常: task_name={task_name}, kwargs={task_params}, e={e}')
             raise e
 
     # 兼容方式请求调用
     def apply(self, task_name: str, task_params: Dict = None, callback: Callback = None, **kwargs):
         """
```

### Comparing `zcbot-celery-sdk-0.0.8/zcbot_celery_sdk/common/exceptions.py` & `zcbot-celery-sdk-0.0.9/zcbot_celery_sdk/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `zcbot-celery-sdk-0.0.8/zcbot_celery_sdk/common/model.py` & `zcbot-celery-sdk-0.0.9/zcbot_celery_sdk/common/model.py`

 * *Files identical despite different names*

### Comparing `zcbot-celery-sdk-0.0.8/zcbot_celery_sdk/common/thread_pool.py` & `zcbot-celery-sdk-0.0.9/zcbot_celery_sdk/common/thread_pool.py`

 * *Files identical despite different names*

### Comparing `zcbot-celery-sdk-0.0.8/zcbot_celery_sdk/common/utils.py` & `zcbot-celery-sdk-0.0.9/zcbot_celery_sdk/common/utils.py`

 * *Files identical despite different names*

### Comparing `zcbot-celery-sdk-0.0.8/zcbot_celery_sdk/monitor.py` & `zcbot-celery-sdk-0.0.9/zcbot_celery_sdk/monitor.py`

 * *Files identical despite different names*

### Comparing `zcbot-celery-sdk-0.0.8/zcbot_celery_sdk/service/base.py` & `zcbot-celery-sdk-0.0.9/zcbot_celery_sdk/service/base.py`

 * *Files identical despite different names*

### Comparing `zcbot-celery-sdk-0.0.8/zcbot_celery_sdk/service/sku_search.py` & `zcbot-celery-sdk-0.0.9/zcbot_celery_sdk/service/sku_search.py`

 * *Files identical despite different names*

### Comparing `zcbot-celery-sdk-0.0.8/zcbot_celery_sdk/service/tax.py` & `zcbot-celery-sdk-0.0.9/zcbot_celery_sdk/service/tax.py`

 * *Files identical despite different names*

### Comparing `zcbot-celery-sdk-0.0.8/zcbot_celery_sdk.egg-info/SOURCES.txt` & `zcbot-celery-sdk-0.0.9/zcbot_celery_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

