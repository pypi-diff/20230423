# Comparing `tmp/ats_case-0.5.4.tar.gz` & `tmp/ats_case-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ats_case-0.5.4.tar", last modified: Sat Apr 22 08:11:42 2023, max compression
+gzip compressed data, was "ats_case-0.5.5.tar", last modified: Sun Apr 23 03:07:07 2023, max compression
```

## Comparing `ats_case-0.5.4.tar` & `ats_case-0.5.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 08:11:42.079189 ats_case-0.5.4/
--rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.5.4/LICENSE
--rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.5.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1042 2023-04-22 08:11:42.077187 ats_case-0.5.4/PKG-INFO
--rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.5.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-22 08:11:41.701257 ats_case-0.5.4/ats_case/
--rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.5.4/ats_case/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-22 08:11:41.900642 ats_case-0.5.4/ats_case/case/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.5.4/ats_case/case/__init__.py
--rw-rw-rw-   0        0        0    17443 2023-04-22 08:02:29.000000 ats_case-0.5.4/ats_case/case/command.py
--rw-rw-rw-   0        0        0     9683 2023-04-20 08:35:14.000000 ats_case-0.5.4/ats_case/case/context.py
--rw-rw-rw-   0        0        0     6309 2023-04-21 03:45:03.000000 ats_case-0.5.4/ats_case/case/executor.py
--rw-rw-rw-   0        0        0     5593 2023-04-21 02:33:28.000000 ats_case-0.5.4/ats_case/case/translator.py
-drwxrwxrwx   0        0        0        0 2023-04-22 08:11:41.969703 ats_case-0.5.4/ats_case/common/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.5.4/ats_case/common/__init__.py
--rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.5.4/ats_case/common/enum.py
--rw-rw-rw-   0        0        0      640 2023-04-20 02:04:10.000000 ats_case-0.5.4/ats_case/common/error.py
-drwxrwxrwx   0        0        0        0 2023-04-22 08:11:42.029850 ats_case-0.5.4/ats_case/manage/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.5.4/ats_case/manage/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-03-03 01:15:16.000000 ats_case-0.5.4/ats_case/manage/core.py
--rw-rw-rw-   0        0        0     2953 2023-04-20 07:40:35.000000 ats_case-0.5.4/ats_case/manage/start.py
-drwxrwxrwx   0        0        0        0 2023-04-22 08:11:42.060725 ats_case-0.5.4/ats_case/template/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.5.4/ats_case/template/__init__.py
--rw-rw-rw-   0        0        0     2067 2023-04-20 00:58:29.000000 ats_case-0.5.4/ats_case/template/testcase_v1.tmp
-drwxrwxrwx   0        0        0        0 2023-04-22 08:11:41.787209 ats_case-0.5.4/ats_case.egg-info/
--rw-rw-rw-   0        0        0     1042 2023-04-22 08:11:41.000000 ats_case-0.5.4/ats_case.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      566 2023-04-22 08:11:41.000000 ats_case-0.5.4/ats_case.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 08:11:41.000000 ats_case-0.5.4/ats_case.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-04-22 08:11:41.000000 ats_case-0.5.4/ats_case.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-22 08:11:41.000000 ats_case-0.5.4/ats_case.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-22 08:11:42.079189 ats_case-0.5.4/setup.cfg
--rw-rw-rw-   0        0        0      935 2023-04-22 08:11:37.000000 ats_case-0.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:07:07.719249 ats_case-0.5.5/
+-rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.5.5/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.5.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1042 2023-04-23 03:07:07.717028 ats_case-0.5.5/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.5.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 03:07:07.318953 ats_case-0.5.5/ats_case/
+-rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.5.5/ats_case/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:07:07.536247 ats_case-0.5.5/ats_case/case/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.5.5/ats_case/case/__init__.py
+-rw-rw-rw-   0        0        0    17443 2023-04-22 08:02:29.000000 ats_case-0.5.5/ats_case/case/command.py
+-rw-rw-rw-   0        0        0     9823 2023-04-23 02:57:35.000000 ats_case-0.5.5/ats_case/case/context.py
+-rw-rw-rw-   0        0        0     7383 2023-04-23 03:03:58.000000 ats_case-0.5.5/ats_case/case/executor.py
+-rw-rw-rw-   0        0        0     5593 2023-04-21 02:33:28.000000 ats_case-0.5.5/ats_case/case/translator.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:07:07.601085 ats_case-0.5.5/ats_case/common/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.5.5/ats_case/common/__init__.py
+-rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.5.5/ats_case/common/enum.py
+-rw-rw-rw-   0        0        0      640 2023-04-20 02:04:10.000000 ats_case-0.5.5/ats_case/common/error.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:07:07.676883 ats_case-0.5.5/ats_case/manage/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.5.5/ats_case/manage/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-03-03 01:15:16.000000 ats_case-0.5.5/ats_case/manage/core.py
+-rw-rw-rw-   0        0        0     2953 2023-04-20 07:40:35.000000 ats_case-0.5.5/ats_case/manage/start.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:07:07.708799 ats_case-0.5.5/ats_case/template/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.5.5/ats_case/template/__init__.py
+-rw-rw-rw-   0        0        0     2067 2023-04-20 00:58:29.000000 ats_case-0.5.5/ats_case/template/testcase_v1.tmp
+drwxrwxrwx   0        0        0        0 2023-04-23 03:07:07.413175 ats_case-0.5.5/ats_case.egg-info/
+-rw-rw-rw-   0        0        0     1042 2023-04-23 03:07:06.000000 ats_case-0.5.5/ats_case.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      566 2023-04-23 03:07:06.000000 ats_case-0.5.5/ats_case.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 03:07:06.000000 ats_case-0.5.5/ats_case.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-04-23 03:07:06.000000 ats_case-0.5.5/ats_case.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-23 03:07:06.000000 ats_case-0.5.5/ats_case.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 03:07:07.719249 ats_case-0.5.5/setup.cfg
+-rw-rw-rw-   0        0        0      935 2023-04-23 03:06:59.000000 ats_case-0.5.5/setup.py
```

### Comparing `ats_case-0.5.4/PKG-INFO` & `ats_case-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats_case
-Version: 0.5.4
+Version: 0.5.5
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.5.4/README.md` & `ats_case-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.4/ats_case/case/command.py` & `ats_case-0.5.5/ats_case/case/command.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.4/ats_case/case/context.py` & `ats_case-0.5.5/ats_case/case/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
         self._test_sn = sn
         self._parse()
 
     def _parse(self):
         tl = mm.Dict.get("test:log", self._test_sn)
 
         self._mode = WorkMode(tl.get('mode'))
+        self._renew = tl.get('renew', 0)
         self._tester = self.Tester(tl.get('tester'))
         self._case = self.Case(tl.get('usercase'))
         self._meter = self.Meter(tl.get('meter'))
         self._bench = self.Bench(tl.get('bench'))
         # 运行时
         self._runtime = self.Runtime()
         self._session = self.Session(self)
@@ -27,14 +28,18 @@
         self._acd_url = tl.get('acd_url')
 
     @property
     def mode(self):
         return self._mode
 
     @property
+    def renew(self):
+        return self._renew
+
+    @property
     def test_sn(self):
         return self._test_sn
 
     @property
     def tester(self):
         return self._tester
 
@@ -279,14 +284,15 @@
             self._step = -1
             self._loop_sn = 0
             self._loop_start_step = 0
             self._loop_end_step = 0
             self._loop_count = 0
             self._loop_index = 0
             self._steps = {}
+            # 多帧时使用
             self._final_result = None
 
         @property
         def step(self):
             return self._step
 
         @step.setter
```

### Comparing `ats_case-0.5.4/ats_case/case/executor.py` & `ats_case-0.5.5/ats_case/case/executor.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,38 +37,61 @@
         self._context = context
         self._model = None
         self._steps = []
 
     def exec(self):
         self.handle()
 
-        index = 0
+        index = self._load()  # 加载在断点续测时所需关键变量
         while index < len(self._steps):
             self._context.runtime.step = self._steps[index]
             if self.loop_meet():
                 self.loop_exec()
             else:
                 self.step_exec()
 
             index = self._steps.index(self._context.runtime.step) + 1
 
     def handle(self):
         pass
 
+    def _load(self):
+        if self._context.renew == 1:
+            self._context.runtime.loop_index = self._context.session.get('breakpoint', 'loop_index')
+            if self._context.runtime.loop_index == 'NULL':
+                self._context.runtime.loop_index = 0
+
+            self._context.runtime.loop_sn = self._context.session.get('breakpoint', 'loop_sn')
+            if self._context.runtime.loop_sn == 'NULL':
+                self._context.runtime.loop_sn = 0
+
+            try:
+                return self._steps.index(self._context.session.get('breakpoint', 'step'))
+            except:
+                pass
+
+        return 0
+
+    def _flush(self):
+        self._context.session.set('breakpoint', 'step', self._context.runtime.step)
+        self._context.session.set('breakpoint', 'loop_sn', self._context.runtime.loop_sn)
+        self._context.session.set('breakpoint', 'loop_index', self._context.runtime.loop_index)
+
     def is_exec(self):
         ifs = self._context.case.control.get('ifs')
         if ifs is not None and type(ifs) is dict and len(ifs) > 0:
             for fc, values in ifs.items():
                 if command.ats().operation(fc).parameter(values).exec(self._context):
                     return False
         return True
 
     def step_exec(self):
         logger.info('~ @TCC-STEP-> steps[#{}] execute'.format(self._context.runtime.step))
 
+        self._flush()  # 缓存在断点续测时所需关键变量
         if self.is_exec():
             getattr(self._model, 'step_{}'.format(self._context.runtime.step))(self._context)
 
     def loop_meet(self):
         loops = self._context.case.control.get('loops')
 
         if loops is None or type(loops) is not list or len(loops) <= 0:
@@ -83,52 +106,53 @@
         step_start = int(ranges.split(':')[0])
         step_end = int(ranges.split(':')[1])
 
         if step_start <= self._context.runtime.step <= step_end:
             self._context.runtime.loop_start_step = step_start
             self._context.runtime.loop_end_step = step_end
             self._context.runtime.loop_count = int(count)
-            self._context.runtime.loop_index = 0
             return True
 
         return False
 
     def loop_exec(self):
         logger.info('~ @TCC-LOOP-> loops[#{}] start. -range {}:{}  -count {}'.format(
             self._context.runtime.loop_sn, self._context.runtime.loop_start_step,
             self._context.runtime.loop_end_step, self._context.runtime.loop_count))
 
-        command.client().message('循环[#{}]开始, 步骤范围[{}-{}], 共{}次'.format(
+        command.client().message('[#{}]循环开始 - 步骤范围[{}-{}], 共{}次'.format(
             self._context.runtime.loop_sn, self._context.runtime.loop_start_step,
             self._context.runtime.loop_end_step, self._context.runtime.loop_count)).show(self._context)
 
-        # while self._context.runtime.loop_index < self._context.runtime.loop_count:
-        for i in range(1, self._context.runtime.loop_count + 1):
-            self._context.runtime.loop_index = i
-
+        while self._context.runtime.loop_index < self._context.runtime.loop_count:
             logger.info('~ @TCC-LOOP-> loops[#{}], -count {}, -index {}'.format(
                 self._context.runtime.loop_sn, self._context.runtime.loop_count,
-                self._context.runtime.loop_index))
-            command.client().message('循环[#{}], 共{}次, 当前第{}次'.format(
+                self._context.runtime.loop_index + 1))
+            command.client().message('[#{}]循环 - 共{}次, 当前执行第{}次'.format(
                 self._context.runtime.loop_sn, self._context.runtime.loop_count,
-                self._context.runtime.loop_index)).show(self._context)
+                self._context.runtime.loop_index + 1)).show(self._context)
 
             for step in range(self._context.runtime.loop_start_step, self._context.runtime.loop_end_step + 1):
                 index = None
                 try:
                     index = self._steps.index(step)
                 except ValueError as e:
                     pass
 
                 if index is not None:
                     self._context.runtime.step = step
                     self.step_exec()
 
-        command.client().message("循环结束...").show(self._context)
+            self._context.runtime.loop_index += 1
+
+        self._context.runtime.loop_index = 0
+
+        command.client().message("[#{}]循环结束...".format(self._context.runtime.loop_sn)).show(self._context)
         logger.info('~ @TCC-LOOP-> loops[#{}] end.'.format(self._context.runtime.loop_sn))
+
         self._context.runtime.loop_sn += 1
 
 
 def extract_steps(content: list):
     n_s = []
     for s in content:
         if s.upper().find('STEP_') >= 0:
```

### Comparing `ats_case-0.5.4/ats_case/case/translator.py` & `ats_case-0.5.5/ats_case/case/translator.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.4/ats_case/common/error.py` & `ats_case-0.5.5/ats_case/common/error.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.4/ats_case/manage/core.py` & `ats_case-0.5.5/ats_case/manage/core.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.4/ats_case/manage/start.py` & `ats_case-0.5.5/ats_case/manage/start.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.4/ats_case/template/testcase_v1.tmp` & `ats_case-0.5.5/ats_case/template/testcase_v1.tmp`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.4/ats_case.egg-info/PKG-INFO` & `ats_case-0.5.5/ats_case.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats-case
-Version: 0.5.4
+Version: 0.5.5
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.5.4/ats_case.egg-info/SOURCES.txt` & `ats_case-0.5.5/ats_case.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.4/setup.py` & `ats_case-0.5.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ats_case",
-    version="0.5.4",
+    version="0.5.5",
     py_modules=['ats_case'],
     author="zhangyue",
     author_email="zhangyue@techen.cn",
     description="Test Script Development Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/henry9000/ats_case",
```

