# Comparing `tmp/ats_case-0.5.6.tar.gz` & `tmp/ats_case-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ats_case-0.5.6.tar", last modified: Sun Apr 23 06:01:58 2023, max compression
+gzip compressed data, was "ats_case-0.5.8.tar", last modified: Sun Apr 23 08:37:59 2023, max compression
```

## Comparing `ats_case-0.5.6.tar` & `ats_case-0.5.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 06:01:58.183908 ats_case-0.5.6/
--rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.5.6/LICENSE
--rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.5.6/MANIFEST.in
--rw-rw-rw-   0        0        0     1042 2023-04-23 06:01:58.181913 ats_case-0.5.6/PKG-INFO
--rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.5.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 06:01:57.534641 ats_case-0.5.6/ats_case/
--rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.5.6/ats_case/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 06:01:57.995411 ats_case-0.5.6/ats_case/case/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.5.6/ats_case/case/__init__.py
--rw-rw-rw-   0        0        0    17411 2023-04-23 03:33:45.000000 ats_case-0.5.6/ats_case/case/command.py
--rw-rw-rw-   0        0        0     9976 2023-04-23 06:01:24.000000 ats_case-0.5.6/ats_case/case/context.py
--rw-rw-rw-   0        0        0     7383 2023-04-23 03:03:58.000000 ats_case-0.5.6/ats_case/case/executor.py
--rw-rw-rw-   0        0        0     5593 2023-04-21 02:33:28.000000 ats_case-0.5.6/ats_case/case/translator.py
-drwxrwxrwx   0        0        0        0 2023-04-23 06:01:58.068217 ats_case-0.5.6/ats_case/common/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.5.6/ats_case/common/__init__.py
--rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.5.6/ats_case/common/enum.py
--rw-rw-rw-   0        0        0      640 2023-04-20 02:04:10.000000 ats_case-0.5.6/ats_case/common/error.py
-drwxrwxrwx   0        0        0        0 2023-04-23 06:01:58.130052 ats_case-0.5.6/ats_case/manage/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.5.6/ats_case/manage/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-03-03 01:15:16.000000 ats_case-0.5.6/ats_case/manage/core.py
--rw-rw-rw-   0        0        0     2953 2023-04-20 07:40:35.000000 ats_case-0.5.6/ats_case/manage/start.py
-drwxrwxrwx   0        0        0        0 2023-04-23 06:01:58.162964 ats_case-0.5.6/ats_case/template/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.5.6/ats_case/template/__init__.py
--rw-rw-rw-   0        0        0     2067 2023-04-20 00:58:29.000000 ats_case-0.5.6/ats_case/template/testcase_v1.tmp
-drwxrwxrwx   0        0        0        0 2023-04-23 06:01:57.708176 ats_case-0.5.6/ats_case.egg-info/
--rw-rw-rw-   0        0        0     1042 2023-04-23 06:01:57.000000 ats_case-0.5.6/ats_case.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      566 2023-04-23 06:01:57.000000 ats_case-0.5.6/ats_case.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 06:01:57.000000 ats_case-0.5.6/ats_case.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-04-23 06:01:57.000000 ats_case-0.5.6/ats_case.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-23 06:01:57.000000 ats_case-0.5.6/ats_case.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 06:01:58.183908 ats_case-0.5.6/setup.cfg
--rw-rw-rw-   0        0        0      935 2023-04-23 06:01:46.000000 ats_case-0.5.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 08:37:59.037916 ats_case-0.5.8/
+-rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.5.8/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.5.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     1042 2023-04-23 08:37:59.034924 ats_case-0.5.8/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.5.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 08:37:58.588131 ats_case-0.5.8/ats_case/
+-rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.5.8/ats_case/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 08:37:58.794243 ats_case-0.5.8/ats_case/case/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.5.8/ats_case/case/__init__.py
+-rw-rw-rw-   0        0        0    17317 2023-04-23 08:37:16.000000 ats_case-0.5.8/ats_case/case/command.py
+-rw-rw-rw-   0        0        0     9976 2023-04-23 06:01:24.000000 ats_case-0.5.8/ats_case/case/context.py
+-rw-rw-rw-   0        0        0     7383 2023-04-23 03:03:58.000000 ats_case-0.5.8/ats_case/case/executor.py
+-rw-rw-rw-   0        0        0     5549 2023-04-23 08:37:16.000000 ats_case-0.5.8/ats_case/case/translator.py
+drwxrwxrwx   0        0        0        0 2023-04-23 08:37:58.853284 ats_case-0.5.8/ats_case/common/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.5.8/ats_case/common/__init__.py
+-rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.5.8/ats_case/common/enum.py
+-rw-rw-rw-   0        0        0      640 2023-04-20 02:04:10.000000 ats_case-0.5.8/ats_case/common/error.py
+drwxrwxrwx   0        0        0        0 2023-04-23 08:37:58.912091 ats_case-0.5.8/ats_case/manage/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.5.8/ats_case/manage/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-03-03 01:15:16.000000 ats_case-0.5.8/ats_case/manage/core.py
+-rw-rw-rw-   0        0        0     2953 2023-04-20 07:40:35.000000 ats_case-0.5.8/ats_case/manage/start.py
+drwxrwxrwx   0        0        0        0 2023-04-23 08:37:59.020761 ats_case-0.5.8/ats_case/template/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.5.8/ats_case/template/__init__.py
+-rw-rw-rw-   0        0        0     2067 2023-04-20 00:58:29.000000 ats_case-0.5.8/ats_case/template/testcase_v1.tmp
+drwxrwxrwx   0        0        0        0 2023-04-23 08:37:58.679886 ats_case-0.5.8/ats_case.egg-info/
+-rw-rw-rw-   0        0        0     1042 2023-04-23 08:37:58.000000 ats_case-0.5.8/ats_case.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      566 2023-04-23 08:37:58.000000 ats_case-0.5.8/ats_case.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 08:37:58.000000 ats_case-0.5.8/ats_case.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-04-23 08:37:58.000000 ats_case-0.5.8/ats_case.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-23 08:37:58.000000 ats_case-0.5.8/ats_case.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 08:37:59.037916 ats_case-0.5.8/setup.cfg
+-rw-rw-rw-   0        0        0      935 2023-04-23 08:37:50.000000 ats_case-0.5.8/setup.py
```

### Comparing `ats_case-0.5.6/PKG-INFO` & `ats_case-0.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats_case
-Version: 0.5.6
+Version: 0.5.8
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.5.6/README.md` & `ats_case-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.6/ats_case/case/command.py` & `ats_case-0.5.8/ats_case/case/command.py`

 * *Files 4% similar despite different names*

```diff
@@ -355,21 +355,20 @@
 
 
 """
     表台篇
 """
 
 
-def bench(manufacture: str):
-    return Bench(manufacture)
+def bench():
+    return Bench()
 
 
 class Bench(object):
-    def __init__(self, manufacture):
-        self._manufacture = manufacture
+    def __init__(self):
         self._operation = None
         self._parameter = None
         self._function = None
         self._interval = None
         self._result = None
         self._exec_times = 0
         self._sleep = 0
@@ -392,24 +391,24 @@
 
     def interval(self, times=0):
         self._interval = times
         return self
 
     def encode(self, context: Context):
         logger.info(
-            '~ @BENCH-> manufacture:{} operation:{} parameter:{}'.format(self._manufacture, self._operation,
+            '~ @BENCH-> manufacture:{} operation:{} parameter:{}'.format(context.bench.manufacture, self._operation,
                                                                          self._parameter))
 
         if type(self._parameter) is dict:
             self._parameter = _replace_bench0(context, self._parameter)
         if self._function is not None and len(self._function) > 0:
             self._build_in(context)
 
     def decode(self, context: Context):
-        logger.info('~ @BENCH<- manufacture:{} operation:{} result:{}'.format(self._manufacture,
+        logger.info('~ @BENCH<- manufacture:{} operation:{} result:{}'.format(context.bench.manufacture,
                                                                               self._operation, self._result))
 
         self._result = self._result.get('result')
         self._flush(context)
 
     def _build_in(self, context: Context):
         logger.info('~ @BUILTIN-> module:{} parameter:{}'.format('bench', self._parameter))
@@ -422,15 +421,15 @@
         logger.info('~ @BUILTIN<- module:{} parameter:{}'.format('bench', self._parameter))
 
     def acv(self, context: Context):
         data = func.to_dict(result=self._result)
 
         logger.info('~ @ACD-> module:{} function:{} parameter:{}'.format(
             'bench', self._operation, self._result))
-        result = udm.handle(module='bench.{}'.format(self._manufacture), function=self._operation
+        result = udm.handle(module='bench', function=self._operation
                             , data=data, debug_url=context.acd_url)
         logger.info('~ @ACD<- module:{} function:{} result:{}'.format('bench', self._operation, result))
 
         return result
 
     def _flush(self, context: Context):
         context.runtime.steps.update({context.runtime.step: func.to_dict(obj='bench', op=self._operation
```

### Comparing `ats_case-0.5.6/ats_case/case/context.py` & `ats_case-0.5.8/ats_case/case/context.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.6/ats_case/case/executor.py` & `ats_case-0.5.8/ats_case/case/executor.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.6/ats_case/case/translator.py` & `ats_case-0.5.8/ats_case/case/translator.py`

 * *Files 5% similar despite different names*

```diff
@@ -132,22 +132,21 @@
         code = "command.encrypt('{}').operation('{}').parameter({}).exec(context)".format(clazz, opt, param)
 
         return code
 
 
 class BENCH(Operation):
     def translate(self, op: dict):
-        clazz = op.get('clazz')
         opt = op.get('operation')
         param = op.get('parameter')
         function = op.get('function')
         sleep = op.get('sleep')
         interval = op.get('interval')
 
-        code = "command.bench('{}').operation('{}')".format(clazz, opt)
+        code = "command.bench().operation('{}')".format(opt)
 
         if param is not None:
             code += ".parameter({})".format(param)
         if function is not None:
             code += ".function({})".format(function)
         if sleep is not None:
             code += ".sleep({})".format(sleep)
```

### Comparing `ats_case-0.5.6/ats_case/common/error.py` & `ats_case-0.5.8/ats_case/common/error.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.6/ats_case/manage/core.py` & `ats_case-0.5.8/ats_case/manage/core.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.6/ats_case/manage/start.py` & `ats_case-0.5.8/ats_case/manage/start.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.6/ats_case/template/testcase_v1.tmp` & `ats_case-0.5.8/ats_case/template/testcase_v1.tmp`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.6/ats_case.egg-info/PKG-INFO` & `ats_case-0.5.8/ats_case.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats-case
-Version: 0.5.6
+Version: 0.5.8
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.5.6/ats_case.egg-info/SOURCES.txt` & `ats_case-0.5.8/ats_case.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.6/setup.py` & `ats_case-0.5.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ats_case",
-    version="0.5.6",
+    version="0.5.8",
     py_modules=['ats_case'],
     author="zhangyue",
     author_email="zhangyue@techen.cn",
     description="Test Script Development Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/henry9000/ats_case",
```

