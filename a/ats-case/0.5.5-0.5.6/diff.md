# Comparing `tmp/ats_case-0.5.5.tar.gz` & `tmp/ats_case-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ats_case-0.5.5.tar", last modified: Sun Apr 23 03:07:07 2023, max compression
+gzip compressed data, was "ats_case-0.5.6.tar", last modified: Sun Apr 23 06:01:58 2023, max compression
```

## Comparing `ats_case-0.5.5.tar` & `ats_case-0.5.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 03:07:07.719249 ats_case-0.5.5/
--rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.5.5/LICENSE
--rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.5.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1042 2023-04-23 03:07:07.717028 ats_case-0.5.5/PKG-INFO
--rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.5.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 03:07:07.318953 ats_case-0.5.5/ats_case/
--rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.5.5/ats_case/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 03:07:07.536247 ats_case-0.5.5/ats_case/case/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.5.5/ats_case/case/__init__.py
--rw-rw-rw-   0        0        0    17443 2023-04-22 08:02:29.000000 ats_case-0.5.5/ats_case/case/command.py
--rw-rw-rw-   0        0        0     9823 2023-04-23 02:57:35.000000 ats_case-0.5.5/ats_case/case/context.py
--rw-rw-rw-   0        0        0     7383 2023-04-23 03:03:58.000000 ats_case-0.5.5/ats_case/case/executor.py
--rw-rw-rw-   0        0        0     5593 2023-04-21 02:33:28.000000 ats_case-0.5.5/ats_case/case/translator.py
-drwxrwxrwx   0        0        0        0 2023-04-23 03:07:07.601085 ats_case-0.5.5/ats_case/common/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.5.5/ats_case/common/__init__.py
--rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.5.5/ats_case/common/enum.py
--rw-rw-rw-   0        0        0      640 2023-04-20 02:04:10.000000 ats_case-0.5.5/ats_case/common/error.py
-drwxrwxrwx   0        0        0        0 2023-04-23 03:07:07.676883 ats_case-0.5.5/ats_case/manage/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.5.5/ats_case/manage/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-03-03 01:15:16.000000 ats_case-0.5.5/ats_case/manage/core.py
--rw-rw-rw-   0        0        0     2953 2023-04-20 07:40:35.000000 ats_case-0.5.5/ats_case/manage/start.py
-drwxrwxrwx   0        0        0        0 2023-04-23 03:07:07.708799 ats_case-0.5.5/ats_case/template/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.5.5/ats_case/template/__init__.py
--rw-rw-rw-   0        0        0     2067 2023-04-20 00:58:29.000000 ats_case-0.5.5/ats_case/template/testcase_v1.tmp
-drwxrwxrwx   0        0        0        0 2023-04-23 03:07:07.413175 ats_case-0.5.5/ats_case.egg-info/
--rw-rw-rw-   0        0        0     1042 2023-04-23 03:07:06.000000 ats_case-0.5.5/ats_case.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      566 2023-04-23 03:07:06.000000 ats_case-0.5.5/ats_case.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 03:07:06.000000 ats_case-0.5.5/ats_case.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-04-23 03:07:06.000000 ats_case-0.5.5/ats_case.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-23 03:07:06.000000 ats_case-0.5.5/ats_case.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 03:07:07.719249 ats_case-0.5.5/setup.cfg
--rw-rw-rw-   0        0        0      935 2023-04-23 03:06:59.000000 ats_case-0.5.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:01:58.183908 ats_case-0.5.6/
+-rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.5.6/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.5.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1042 2023-04-23 06:01:58.181913 ats_case-0.5.6/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.5.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 06:01:57.534641 ats_case-0.5.6/ats_case/
+-rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.5.6/ats_case/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:01:57.995411 ats_case-0.5.6/ats_case/case/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.5.6/ats_case/case/__init__.py
+-rw-rw-rw-   0        0        0    17411 2023-04-23 03:33:45.000000 ats_case-0.5.6/ats_case/case/command.py
+-rw-rw-rw-   0        0        0     9976 2023-04-23 06:01:24.000000 ats_case-0.5.6/ats_case/case/context.py
+-rw-rw-rw-   0        0        0     7383 2023-04-23 03:03:58.000000 ats_case-0.5.6/ats_case/case/executor.py
+-rw-rw-rw-   0        0        0     5593 2023-04-21 02:33:28.000000 ats_case-0.5.6/ats_case/case/translator.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:01:58.068217 ats_case-0.5.6/ats_case/common/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.5.6/ats_case/common/__init__.py
+-rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.5.6/ats_case/common/enum.py
+-rw-rw-rw-   0        0        0      640 2023-04-20 02:04:10.000000 ats_case-0.5.6/ats_case/common/error.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:01:58.130052 ats_case-0.5.6/ats_case/manage/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.5.6/ats_case/manage/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-03-03 01:15:16.000000 ats_case-0.5.6/ats_case/manage/core.py
+-rw-rw-rw-   0        0        0     2953 2023-04-20 07:40:35.000000 ats_case-0.5.6/ats_case/manage/start.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:01:58.162964 ats_case-0.5.6/ats_case/template/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.5.6/ats_case/template/__init__.py
+-rw-rw-rw-   0        0        0     2067 2023-04-20 00:58:29.000000 ats_case-0.5.6/ats_case/template/testcase_v1.tmp
+drwxrwxrwx   0        0        0        0 2023-04-23 06:01:57.708176 ats_case-0.5.6/ats_case.egg-info/
+-rw-rw-rw-   0        0        0     1042 2023-04-23 06:01:57.000000 ats_case-0.5.6/ats_case.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      566 2023-04-23 06:01:57.000000 ats_case-0.5.6/ats_case.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 06:01:57.000000 ats_case-0.5.6/ats_case.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-04-23 06:01:57.000000 ats_case-0.5.6/ats_case.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-23 06:01:57.000000 ats_case-0.5.6/ats_case.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 06:01:58.183908 ats_case-0.5.6/setup.cfg
+-rw-rw-rw-   0        0        0      935 2023-04-23 06:01:46.000000 ats_case-0.5.6/setup.py
```

### Comparing `ats_case-0.5.5/PKG-INFO` & `ats_case-0.5.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats_case
-Version: 0.5.5
+Version: 0.5.6
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.5.5/README.md` & `ats_case-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.5/ats_case/case/command.py` & `ats_case-0.5.6/ats_case/case/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -243,16 +243,15 @@
         if data.get('error') == 1:
             raise MeterOperationError(data.get('result'))
 
         # 分帧处理开始
         next_frame = data.get('next_frame', None)
         if next_frame is not None:
             result = send(context,
-                          todo={
-                              'meter:comm': {'channel': {'type': 'RS485', 'baudrate': 9600}, 'frame': next_frame}})
+                          todo={'meter:comm': {'channel': {'type': 'RS485', 'baudrate': 9600}, 'frame': next_frame}})
             self._frame = result.get('result')
             self.decode(context, index + 1)
         else:
             context.runtime.final_result = data.get('result')
         # 分帧处理结束
 
         if index == 0:
```

### Comparing `ats_case-0.5.5/ats_case/case/context.py` & `ats_case-0.5.6/ats_case/case/context.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,16 +11,16 @@
     def __init__(self, sn):
         self._test_sn = sn
         self._parse()
 
     def _parse(self):
         tl = mm.Dict.get("test:log", self._test_sn)
 
-        self._mode = WorkMode(tl.get('mode'))
         self._renew = tl.get('renew', 0)
+        self._mode = WorkMode(tl.get('mode'))
         self._tester = self.Tester(tl.get('tester'))
         self._case = self.Case(tl.get('usercase'))
         self._meter = self.Meter(tl.get('meter'))
         self._bench = self.Bench(tl.get('bench'))
         # 运行时
         self._runtime = self.Runtime()
         self._session = self.Session(self)
@@ -215,14 +215,16 @@
             self._no = data.get('no')
             self._protocol = data.get('protocol')
             self._model = data.get('model')
             self._connect = data.get('connect')
             self._rated_voltage = data.get('rated_voltage')
             self._rated_current = data.get('rated_current')
             self._frequency = data.get('frequency')
+            self._mconst = data.get('mconst')
+            self._mpluse = data.get('mpluse')
             self._iabc = 'H'
 
             if self._connect == 0:
                 self._iabc = 'A'
 
         #         self._channel = {'RS485': data.get('baudrate_485'), 'IR': data.get('baudrate_ir'),
         #                          'PLC': data.get('baudrate_plc')}
@@ -263,22 +265,25 @@
             return self._rated_current
 
         @property
         def frequency(self):
             return self._frequency
 
         @property
+        def mconst(self):
+            return self._mconst
+
+        @property
+        def mpluse(self):
+            return self._mpluse
+
+        @property
         def iabc(self):
             return self._iabc
 
-    #
-    #     @property
-    #     def channel(self):
-    #         return self._channel
-    #
     class Runtime(object):
         """
         运行时
         """
 
         def __init__(self):
             self._step = -1
@@ -356,8 +361,7 @@
             self._parent = parent
 
         def get(self, name: str, key: str):
             return mm.Dict.get('{}:{}'.format(self._parent.test_sn, name), key)
 
         def set(self, name: str, key: str, data):
             return mm.Dict.put('{}:{}'.format(self._parent.test_sn, name), key, data)
-
```

### Comparing `ats_case-0.5.5/ats_case/case/executor.py` & `ats_case-0.5.6/ats_case/case/executor.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.5/ats_case/case/translator.py` & `ats_case-0.5.6/ats_case/case/translator.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.5/ats_case/common/error.py` & `ats_case-0.5.6/ats_case/common/error.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.5/ats_case/manage/core.py` & `ats_case-0.5.6/ats_case/manage/core.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.5/ats_case/manage/start.py` & `ats_case-0.5.6/ats_case/manage/start.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.5/ats_case/template/testcase_v1.tmp` & `ats_case-0.5.6/ats_case/template/testcase_v1.tmp`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.5/ats_case.egg-info/PKG-INFO` & `ats_case-0.5.6/ats_case.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats-case
-Version: 0.5.5
+Version: 0.5.6
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.5.5/ats_case.egg-info/SOURCES.txt` & `ats_case-0.5.6/ats_case.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.5/setup.py` & `ats_case-0.5.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ats_case",
-    version="0.5.5",
+    version="0.5.6",
     py_modules=['ats_case'],
     author="zhangyue",
     author_email="zhangyue@techen.cn",
     description="Test Script Development Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/henry9000/ats_case",
```

