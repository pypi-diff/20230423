# Comparing `tmp/onedice-1.0.5.tar.gz` & `tmp/onedice-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\onedice-1.0.5.tar", last modified: Fri Nov 25 02:14:26 2022, max compression
+gzip compressed data, was "dist\onedice-1.0.7.tar", last modified: Sun Apr 23 07:57:12 2023, max compression
```

## Comparing `onedice-1.0.5.tar` & `onedice-1.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2022-11-25 02:14:26.000000 onedice-1.0.5/
--rw-rw-rw-   0        0        0      592 2022-11-25 02:14:26.000000 onedice-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      147 2022-04-17 04:14:08.000000 onedice-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2022-11-25 02:14:26.000000 onedice-1.0.5/onedice/
--rw-rw-rw-   0        0        0      503 2022-04-17 04:14:08.000000 onedice-1.0.5/onedice/__init__.py
--rw-rw-rw-   0        0        0   200698 2022-11-25 01:40:23.000000 onedice-1.0.5/onedice/main.py
-drwxrwxrwx   0        0        0        0 2022-11-25 02:14:26.000000 onedice-1.0.5/onedice.egg-info/
--rw-rw-rw-   0        0        0      592 2022-11-25 02:14:26.000000 onedice-1.0.5/onedice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      178 2022-11-25 02:14:26.000000 onedice-1.0.5/onedice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-25 02:14:26.000000 onedice-1.0.5/onedice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2022-11-25 02:14:26.000000 onedice-1.0.5/onedice.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-11-25 02:14:26.000000 onedice-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1135 2022-11-25 02:03:42.000000 onedice-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 07:57:12.000000 onedice-1.0.7/
+-rw-rw-rw-   0        0        0      592 2023-04-23 07:57:12.000000 onedice-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      147 2022-04-17 04:14:08.000000 onedice-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 07:57:12.000000 onedice-1.0.7/onedice/
+-rw-rw-rw-   0        0        0      503 2022-04-17 04:14:08.000000 onedice-1.0.7/onedice/__init__.py
+-rw-rw-rw-   0        0        0   203168 2023-04-23 07:40:04.000000 onedice-1.0.7/onedice/main.py
+drwxrwxrwx   0        0        0        0 2023-04-23 07:57:12.000000 onedice-1.0.7/onedice.egg-info/
+-rw-rw-rw-   0        0        0      592 2023-04-23 07:57:12.000000 onedice-1.0.7/onedice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-04-23 07:57:12.000000 onedice-1.0.7/onedice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 07:57:12.000000 onedice-1.0.7/onedice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-23 07:57:12.000000 onedice-1.0.7/onedice.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 07:57:12.000000 onedice-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1135 2023-04-23 07:52:14.000000 onedice-1.0.7/setup.py
```

### Comparing `onedice-1.0.5/PKG-INFO` & `onedice-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onedice
-Version: 1.0.5
+Version: 1.0.7
 Summary: OneDice offical standard library for Python
 Home-page: https://github.com/OlivOS-Team/lib-onedice
 Author: lunzhiPenxil
 Author-email: lunzhiPenxil@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `onedice-1.0.5/onedice/main.py` & `onedice-1.0.7/onedice/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 @Desc      :   None
 '''
 
 from enum import Enum
 import random
 import traceback
 
-pypi_version = '1.0.5'
+pypi_version = '1.0.7'
 
 dictOperationPriority = {
     '[' : None,
     ']' : None,
     ',' : None,
     '(' : None,
     ')' : None,
@@ -74,14 +74,18 @@
     '$T' : 9
 }
 
 dictOperationMapping = {
     'df' : 'f'
 }
 
+dictRuleOperationPriority = {}
+
+dictRuleOperationMapping = {}
+
 listOperationSub = [
     'm',
     'M',
     'k',
     'K',
     'q',
     'Q',
@@ -222,27 +226,34 @@
         self.type = self.nodeType.TUPLE
         self.num = 0
 
 '''
 语法树运算符节点结构体
 '''
 class calOperationNode(calNode):
-    def __init__(self, data, customDefault = None):
+    def __init__(
+        self,
+        data,
+        customDefault = None,
+        ruleMode = 'default'
+    ):
         calNode.__init__(self)
         self.data = data.lower()
         self.type = self.nodeType.OPERATION
         self.vals = {}
         self.valsDefault = {}
         self.valLeftDefault = None
         self.valRightDefault = None
         self.valStarterLeftDefault = None
         self.valEnderRightDefault = None
         self.priority = None
         self.dictOperationPriority = dictOperationPriority
+        self.dictRuleOperationPriority = dictRuleOperationPriority
         self.customDefault = customDefault
+        self.ruleMode = ruleMode
         self.initOperation()
 
     def initOperation(self):
         if self.inOperation():
             self.getPriority()
         if self.data == '-':
             self.valStarterLeftDefault = 0
@@ -303,40 +314,54 @@
                     for val_this in self.valsDefault:
                         if val_this in self.customDefault[self.data]['subD']:
                             self.valsDefault[val_this] = self.customDefault[self.data]['subD'][val_this]
 
     def getPriority(self):
         if self.data in self.dictOperationPriority:
             self.priority = self.dictOperationPriority[self.data]
+        elif self.ruleMode in self.dictRuleOperationPriority \
+        and self.data in self.dictRuleOperationPriority[self.ruleMode]:
+            self.priority = self.dictRuleOperationPriority[self.ruleMode][self.data]
         return self.priority
 
     def inOperation(self):
         res = False
         if self.data in self.dictOperationPriority:
             res = True
+        elif self.ruleMode in self.dictRuleOperationPriority \
+        and self.data in self.dictRuleOperationPriority[self.ruleMode]:
+            res = True
         return res
 
 class RD(object):
-    def __init__(self, initData, customDefault = None, valueTable = None):
+    def __init__(
+        self,
+        initData,
+        customDefault = None,
+        valueTable = None,
+        ruleMode = 'default'
+    ):
         self.originDataRaw = initData
         self.originData = initData.lower()
         self.calTree = calNodeStack([])
         self.resInt = None
         self.resIntMin = None
         self.resIntMax = None
         self.resIntMinType = None
         self.resIntMaxType = None
         self.resDetail = None
         self.resDetailData = []
         self.resMetaTuple = []
         self.resMetaTupleEnable = False
         self.resError = None
         self.dictOperationPriority = dictOperationPriority
+        self.dictRuleOperationPriority = dictRuleOperationPriority
         self.customDefault = customDefault
         self.valueTable = valueTable
+        self.ruleMode = ruleMode
 
     def roll(self):
         try:
             if type(self.valueTable) == dict:
                 self.__replace()
         except Exception as e:
             traceback.print_exc()
@@ -405,20 +430,26 @@
             self.resMetaTuple = []
             self.resMetaTupleEnable = False
 
     def getPriority(self, data):
         res = None
         if data in self.dictOperationPriority:
             res = self.dictOperationPriority[data]
+        elif self.ruleMode in self.dictRuleOperationPriority \
+        and data in self.dictRuleOperationPriority[self.ruleMode]:
+            res = self.dictRuleOperationPriority[self.ruleMode][data]
         return res
 
     def inOperation(self, data):
         res = False
         if data in self.dictOperationPriority:
             res = True
+        elif self.ruleMode in self.dictRuleOperationPriority \
+        and data in self.dictRuleOperationPriority[self.ruleMode]:
+            res = True
         return res
 
     '''
     该方法实现自定义随机数生成函数，可通过继承后重写来完成随机数算法的修改
     '''
     def random(self, nMin, nMax):
         return random.randint(nMin, nMax)
@@ -629,15 +660,22 @@
                         break
                 elif self.inOperation(tmp_data_this):
                     if self.getPriority(tmp_data_this) != None:
                         tmp_op_peek_this = op_stack.peek()
                         tmp_data_this_real = tmp_data_this
                         if tmp_data_this.lower() in dictOperationMapping:
                             tmp_data_this_real = dictOperationMapping[tmp_data_this.lower()]
-                        tmp_calOperationNode_this = calOperationNode(tmp_data_this_real, self.customDefault)
+                        elif self.ruleMode in dictRuleOperationMapping \
+                        and tmp_data_this.lower() in dictRuleOperationMapping[self.ruleMode]:
+                            tmp_data_this_real = dictRuleOperationMapping[self.ruleMode][tmp_data_this.lower()]
+                        tmp_calOperationNode_this = calOperationNode(
+                            data = tmp_data_this_real,
+                            customDefault = self.customDefault,
+                            ruleMode = self.ruleMode
+                        )
                         if not flag_left_as_number:
                             if tmp_op_peek_this == None:
                                 if tmp_calOperationNode_this.valStarterLeftDefault != None:
                                     tmp_res.push(calNumberNode(str(tmp_calOperationNode_this.valStarterLeftDefault)))
                                     flag_left_as_number = True
                                 elif tmp_calOperationNode_this.valLeftDefault != None:
                                     tmp_res.push(calNumberNode(str(tmp_calOperationNode_this.valLeftDefault)))
@@ -672,20 +710,28 @@
                                 self.resError = self.resErrorType.INPUT_RAW_INVALID
                                 break
                         if tmp_op_peek_this != None:
                             if tmp_op_peek_this.getPriority() == None:
                                 pass
                             elif self.getPriority(tmp_data_this_real) <= tmp_op_peek_this.getPriority():
                                 tmp_res.pushList(op_stack.popTo('(', self.getPriority(tmp_data_this_real), True))
-                        op_stack.push(calOperationNode(tmp_data_this_real, self.customDefault))
+                        op_stack.push(calOperationNode(
+                            data = tmp_data_this_real,
+                            customDefault = self.customDefault,
+                            ruleMode = self.ruleMode
+                        ))
                         flag_old_number = False
                         flag_left_as_number = False
                         tmp_offset = lenOperation_this
                     elif tmp_data_this == '(':
-                        op_stack.push(calOperationNode(tmp_data_this, self.customDefault))
+                        op_stack.push(calOperationNode(
+                            data = tmp_data_this,
+                            customDefault = self.customDefault,
+                            ruleMode = self.ruleMode
+                        ))
                         count_child_para += 1
                         flag_old_number = False
                         flag_left_as_number = False
                         tmp_offset = 1
                     elif tmp_data_this == ')':
                         if not flag_left_as_number:
                             tmp_op_peek_this = op_stack.peek()
@@ -2630,22 +2676,26 @@
                     tmp_node_this_output_data_1 = []
                     tmp_node_this_output_data_2 = []
                     tmp_node_this_output_data_3 = []
                     tmp_node_this_output_data_final = []
                     tmp_node_this_output_this = self.random(1, 100)
                     tmp_node_this_output_1 = tmp_node_this_output_this
                     tmp_range_list = range(0, tmp_main_val_right[0])
+                    tmp_node_this_output_1_1 = int(tmp_node_this_output_1 / 10)
+                    tmp_node_this_output_1_2 = int(tmp_node_this_output_1 % 10)
                     for tmp_it_this in tmp_range_list:
                         tmp_node_this_output_this = self.random(1, 10) - 1
+                        if tmp_node_this_output_1_2 == 0 and tmp_node_this_output_this == 0:
+                            tmp_node_this_output_this = 10
                         tmp_node_this_output_list_2.append(tmp_node_this_output_this)
                         if tmp_node_this_output_2_mark > tmp_node_this_output_this:
                             tmp_node_this_output_2_mark = tmp_node_this_output_this
-                    tmp_node_this_output_1_1 = int(tmp_node_this_output_1 / 10)
-                    tmp_node_this_output_1_2 = int(tmp_node_this_output_1 % 10)
-                    if tmp_node_this_output_1_1 > tmp_node_this_output_2_mark:
+                    if tmp_node_this_output_1_2 == 0 and tmp_node_this_output_2_mark == 0:
+                        tmp_node_this_output = 100
+                    elif tmp_node_this_output_1_1 > tmp_node_this_output_2_mark:
                         tmp_node_this_output = tmp_node_this_output_1_2 + tmp_node_this_output_2_mark * 10
                     else:
                         tmp_node_this_output = tmp_node_this_output_1
                     # data主要处理流程
                     tmp_node_this_output_data_1 = [tmp_node_this_output_1]
                     for tmp_node_this_output_list_2_this in tmp_node_this_output_list_2:
                         tmp_node_this_output_list_2_this_res = tmp_node_this_output_list_2_this
@@ -2708,22 +2758,26 @@
                     tmp_node_this_output_data_1 = []
                     tmp_node_this_output_data_2 = []
                     tmp_node_this_output_data_3 = []
                     tmp_node_this_output_data_final = []
                     tmp_node_this_output_this = self.random(1, 100)
                     tmp_node_this_output_1 = tmp_node_this_output_this
                     tmp_range_list = range(0, tmp_main_val_right[0])
+                    tmp_node_this_output_1_1 = int(tmp_node_this_output_1 / 10)
+                    tmp_node_this_output_1_2 = int(tmp_node_this_output_1 % 10)
                     for tmp_it_this in tmp_range_list:
                         tmp_node_this_output_this = self.random(1, 10) - 1
+                        if tmp_node_this_output_1_2 == 0 and tmp_node_this_output_this == 0:
+                            tmp_node_this_output_this = 10
                         tmp_node_this_output_list_2.append(tmp_node_this_output_this)
                         if tmp_node_this_output_2_mark < tmp_node_this_output_this:
                             tmp_node_this_output_2_mark = tmp_node_this_output_this
-                    tmp_node_this_output_1_1 = int(tmp_node_this_output_1 / 10)
-                    tmp_node_this_output_1_2 = int(tmp_node_this_output_1 % 10)
-                    if tmp_node_this_output_1_1 < tmp_node_this_output_2_mark:
+                    if tmp_node_this_output_1_2 == 0 and tmp_node_this_output_2_mark == 0:
+                        tmp_node_this_output = 100
+                    elif tmp_node_this_output_1_1 < tmp_node_this_output_2_mark:
                         tmp_node_this_output = tmp_node_this_output_1_2 + tmp_node_this_output_2_mark * 10
                     else:
                         tmp_node_this_output = tmp_node_this_output_1
                     # data主要处理流程
                     tmp_node_this_output_data_1 = [tmp_node_this_output_1]
                     for tmp_node_this_output_list_2_this in tmp_node_this_output_list_2:
                         tmp_node_this_output_list_2_this_res = tmp_node_this_output_list_2_this
```

### Comparing `onedice-1.0.5/onedice.egg-info/PKG-INFO` & `onedice-1.0.7/onedice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onedice
-Version: 1.0.5
+Version: 1.0.7
 Summary: OneDice offical standard library for Python
 Home-page: https://github.com/OlivOS-Team/lib-onedice
 Author: lunzhiPenxil
 Author-email: lunzhiPenxil@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `onedice-1.0.5/setup.py` & `onedice-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="onedice",
-    version="1.0.5",
+    version="1.0.7",
     author="lunzhiPenxil",
     author_email="lunzhiPenxil@gmail.com",
     description="OneDice offical standard library for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/OlivOS-Team/lib-onedice",
     packages=setuptools.find_packages(),
```

