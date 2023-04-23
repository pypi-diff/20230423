# Comparing `tmp/AISimuToolKit-0.0.2.tar.gz` & `tmp/AISimuToolKit-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AISimuToolKit-0.0.2.tar", last modified: Sat Apr 22 08:33:41 2023, max compression
+gzip compressed data, was "AISimuToolKit-0.0.3.tar", last modified: Sat Apr 22 08:42:21 2023, max compression
```

## Comparing `AISimuToolKit-0.0.2.tar` & `AISimuToolKit-0.0.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-22 08:33:41.525884 AISimuToolKit-0.0.2/
-drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-22 08:33:41.521885 AISimuToolKit-0.0.2/AISimuToolKit/
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)       85 2023-04-22 08:15:55.000000 AISimuToolKit-0.0.2/AISimuToolKit/__init__.py
-drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-22 08:33:41.521885 AISimuToolKit-0.0.2/AISimuToolKit/exp/
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)      112 2023-04-22 08:15:55.000000 AISimuToolKit-0.0.2/AISimuToolKit/exp/__init__.py
-drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-22 08:33:41.521885 AISimuToolKit-0.0.2/AISimuToolKit/exp/actions/
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)      307 2023-04-22 08:15:55.000000 AISimuToolKit-0.0.2/AISimuToolKit/exp/actions/__init__.py
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)      434 2023-04-22 08:28:12.000000 AISimuToolKit-0.0.2/AISimuToolKit/exp/actions/base_action.py
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     1317 2023-04-22 08:28:12.000000 AISimuToolKit-0.0.2/AISimuToolKit/exp/actions/finetune_action.py
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     1273 2023-04-22 08:28:12.000000 AISimuToolKit-0.0.2/AISimuToolKit/exp/actions/instruct_action.py
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     2091 2023-04-22 08:28:12.000000 AISimuToolKit-0.0.2/AISimuToolKit/exp/actions/probe_action.py
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     2410 2023-04-22 08:28:12.000000 AISimuToolKit-0.0.2/AISimuToolKit/exp/actions/reflection_action.py
-drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-22 08:33:41.521885 AISimuToolKit-0.0.2/AISimuToolKit/exp/agents/
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)       83 2023-04-22 08:15:55.000000 AISimuToolKit-0.0.2/AISimuToolKit/exp/agents/__init__.py
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)      610 2023-04-22 08:28:12.000000 AISimuToolKit-0.0.2/AISimuToolKit/exp/agents/agent.py
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     2769 2023-04-22 08:15:55.000000 AISimuToolKit-0.0.2/AISimuToolKit/exp/agents/memory.py
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     6732 2023-04-22 08:28:12.000000 AISimuToolKit-0.0.2/AISimuToolKit/exp/experiment.py
-drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-22 08:33:41.521885 AISimuToolKit-0.0.2/AISimuToolKit/model/
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)      237 2023-04-22 08:15:55.000000 AISimuToolKit-0.0.2/AISimuToolKit/model/__init__.py
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     9470 2023-04-22 08:28:12.000000 AISimuToolKit-0.0.2/AISimuToolKit/model/model.py
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     2244 2023-04-22 08:28:12.000000 AISimuToolKit-0.0.2/AISimuToolKit/model/register.py
-drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-22 08:33:41.521885 AISimuToolKit-0.0.2/AISimuToolKit/store/
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)       54 2023-04-22 08:15:55.000000 AISimuToolKit-0.0.2/AISimuToolKit/store/__init__.py
-drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-22 08:33:41.525884 AISimuToolKit-0.0.2/AISimuToolKit/utils/
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)      559 2023-04-22 08:15:55.000000 AISimuToolKit-0.0.2/AISimuToolKit/utils/__init__.py
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     1369 2023-04-22 08:15:55.000000 AISimuToolKit-0.0.2/AISimuToolKit/utils/utils.py
-drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-22 08:33:41.521885 AISimuToolKit-0.0.2/AISimuToolKit.egg-info/
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)      407 2023-04-22 08:33:41.000000 AISimuToolKit-0.0.2/AISimuToolKit.egg-info/PKG-INFO
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)      830 2023-04-22 08:33:41.000000 AISimuToolKit-0.0.2/AISimuToolKit.egg-info/SOURCES.txt
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)        1 2023-04-22 08:33:41.000000 AISimuToolKit-0.0.2/AISimuToolKit.egg-info/dependency_links.txt
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)       57 2023-04-22 08:33:41.000000 AISimuToolKit-0.0.2/AISimuToolKit.egg-info/requires.txt
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)       14 2023-04-22 08:33:41.000000 AISimuToolKit-0.0.2/AISimuToolKit.egg-info/top_level.txt
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)      407 2023-04-22 08:33:41.525884 AISimuToolKit-0.0.2/PKG-INFO
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)       38 2023-04-22 08:33:41.525884 AISimuToolKit-0.0.2/setup.cfg
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     1027 2023-04-22 08:33:15.000000 AISimuToolKit-0.0.2/setup.py
+drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-22 08:42:21.170009 AISimuToolKit-0.0.3/
+drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-22 08:42:21.166010 AISimuToolKit-0.0.3/AISimuToolKit/
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)       85 2023-04-22 08:15:55.000000 AISimuToolKit-0.0.3/AISimuToolKit/__init__.py
+drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-22 08:42:21.166010 AISimuToolKit-0.0.3/AISimuToolKit/exp/
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)      112 2023-04-22 08:15:55.000000 AISimuToolKit-0.0.3/AISimuToolKit/exp/__init__.py
+drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-22 08:42:21.166010 AISimuToolKit-0.0.3/AISimuToolKit/exp/actions/
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)      307 2023-04-22 08:15:55.000000 AISimuToolKit-0.0.3/AISimuToolKit/exp/actions/__init__.py
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)      434 2023-04-22 08:28:12.000000 AISimuToolKit-0.0.3/AISimuToolKit/exp/actions/base_action.py
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     1317 2023-04-22 08:28:12.000000 AISimuToolKit-0.0.3/AISimuToolKit/exp/actions/finetune_action.py
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     1273 2023-04-22 08:28:12.000000 AISimuToolKit-0.0.3/AISimuToolKit/exp/actions/instruct_action.py
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     2091 2023-04-22 08:28:12.000000 AISimuToolKit-0.0.3/AISimuToolKit/exp/actions/probe_action.py
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     2410 2023-04-22 08:28:12.000000 AISimuToolKit-0.0.3/AISimuToolKit/exp/actions/reflection_action.py
+drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-22 08:42:21.166010 AISimuToolKit-0.0.3/AISimuToolKit/exp/agents/
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)       83 2023-04-22 08:15:55.000000 AISimuToolKit-0.0.3/AISimuToolKit/exp/agents/__init__.py
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)      610 2023-04-22 08:28:12.000000 AISimuToolKit-0.0.3/AISimuToolKit/exp/agents/agent.py
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     2769 2023-04-22 08:15:55.000000 AISimuToolKit-0.0.3/AISimuToolKit/exp/agents/memory.py
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     6732 2023-04-22 08:28:12.000000 AISimuToolKit-0.0.3/AISimuToolKit/exp/experiment.py
+drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-22 08:42:21.170009 AISimuToolKit-0.0.3/AISimuToolKit/model/
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)      237 2023-04-22 08:15:55.000000 AISimuToolKit-0.0.3/AISimuToolKit/model/__init__.py
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     9470 2023-04-22 08:28:12.000000 AISimuToolKit-0.0.3/AISimuToolKit/model/model.py
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     2244 2023-04-22 08:28:12.000000 AISimuToolKit-0.0.3/AISimuToolKit/model/register.py
+drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-22 08:42:21.170009 AISimuToolKit-0.0.3/AISimuToolKit/store/
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)       54 2023-04-22 08:15:55.000000 AISimuToolKit-0.0.3/AISimuToolKit/store/__init__.py
+drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-22 08:42:21.170009 AISimuToolKit-0.0.3/AISimuToolKit/utils/
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)      559 2023-04-22 08:15:55.000000 AISimuToolKit-0.0.3/AISimuToolKit/utils/__init__.py
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     1369 2023-04-22 08:15:55.000000 AISimuToolKit-0.0.3/AISimuToolKit/utils/utils.py
+drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-22 08:42:21.166010 AISimuToolKit-0.0.3/AISimuToolKit.egg-info/
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)      407 2023-04-22 08:42:21.000000 AISimuToolKit-0.0.3/AISimuToolKit.egg-info/PKG-INFO
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)      830 2023-04-22 08:42:21.000000 AISimuToolKit-0.0.3/AISimuToolKit.egg-info/SOURCES.txt
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)        1 2023-04-22 08:42:21.000000 AISimuToolKit-0.0.3/AISimuToolKit.egg-info/dependency_links.txt
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)       44 2023-04-22 08:42:21.000000 AISimuToolKit-0.0.3/AISimuToolKit.egg-info/requires.txt
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)       14 2023-04-22 08:42:21.000000 AISimuToolKit-0.0.3/AISimuToolKit.egg-info/top_level.txt
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)      407 2023-04-22 08:42:21.170009 AISimuToolKit-0.0.3/PKG-INFO
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)       38 2023-04-22 08:42:21.170009 AISimuToolKit-0.0.3/setup.cfg
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     1011 2023-04-22 08:42:20.000000 AISimuToolKit-0.0.3/setup.py
```

### Comparing `AISimuToolKit-0.0.2/AISimuToolKit/exp/actions/finetune_action.py` & `AISimuToolKit-0.0.3/AISimuToolKit/exp/actions/finetune_action.py`

 * *Files identical despite different names*

### Comparing `AISimuToolKit-0.0.2/AISimuToolKit/exp/actions/instruct_action.py` & `AISimuToolKit-0.0.3/AISimuToolKit/exp/actions/instruct_action.py`

 * *Files identical despite different names*

### Comparing `AISimuToolKit-0.0.2/AISimuToolKit/exp/actions/probe_action.py` & `AISimuToolKit-0.0.3/AISimuToolKit/exp/actions/probe_action.py`

 * *Files identical despite different names*

### Comparing `AISimuToolKit-0.0.2/AISimuToolKit/exp/actions/reflection_action.py` & `AISimuToolKit-0.0.3/AISimuToolKit/exp/actions/reflection_action.py`

 * *Files identical despite different names*

### Comparing `AISimuToolKit-0.0.2/AISimuToolKit/exp/agents/agent.py` & `AISimuToolKit-0.0.3/AISimuToolKit/exp/agents/agent.py`

 * *Files identical despite different names*

### Comparing `AISimuToolKit-0.0.2/AISimuToolKit/exp/agents/memory.py` & `AISimuToolKit-0.0.3/AISimuToolKit/exp/agents/memory.py`

 * *Files identical despite different names*

### Comparing `AISimuToolKit-0.0.2/AISimuToolKit/exp/experiment.py` & `AISimuToolKit-0.0.3/AISimuToolKit/exp/experiment.py`

 * *Files identical despite different names*

### Comparing `AISimuToolKit-0.0.2/AISimuToolKit/model/model.py` & `AISimuToolKit-0.0.3/AISimuToolKit/model/model.py`

 * *Files identical despite different names*

### Comparing `AISimuToolKit-0.0.2/AISimuToolKit/model/register.py` & `AISimuToolKit-0.0.3/AISimuToolKit/model/register.py`

 * *Files identical despite different names*

### Comparing `AISimuToolKit-0.0.2/AISimuToolKit/utils/__init__.py` & `AISimuToolKit-0.0.3/AISimuToolKit/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `AISimuToolKit-0.0.2/AISimuToolKit/utils/utils.py` & `AISimuToolKit-0.0.3/AISimuToolKit/utils/utils.py`

 * *Files identical despite different names*

### Comparing `AISimuToolKit-0.0.2/AISimuToolKit.egg-info/SOURCES.txt` & `AISimuToolKit-0.0.3/AISimuToolKit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AISimuToolKit-0.0.2/setup.py` & `AISimuToolKit-0.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/usr/bin/env python
 #-*- coding:utf-8 -*-
 
 from setuptools import setup, find_packages            #这个包没有的可以pip一下
 
 setup(
     name = "AISimuToolKit",      #这里是pip项目发布的名称
-    version = "0.0.2",  #版本号，数值大的会优先被pip
+    version = "0.0.3",  #版本号，数值大的会优先被pip
     keywords = ["pip", "AISimuToolKit"],			# 关键字
     description = "ICIP's private utils.",	# 描述
     long_description = "ICIP's private utils. The development version will be released when it is sufficiently refined",
     license = "MIT Licence",		# 许可证
     url = "http://git.cipsup.cn/aisimulationplatform/toolkit/aisimulation",     #项目相关文件地址，一般是github项目地址即可
     author = "Ren & Guo",			# 作者
     author_email = "renmengjie22@mails.ucas.ac.cn",
     packages = find_packages(),
     include_package_data = True,
     platforms = "any",
-    python_requires='==3.10',
-    install_requires = ["openai==0.27.4", "Requests==2.28.2", "pyyaml==6.0", "python==3.10"]   #这个项目依赖的第三方库
+    python_requires='>=3.10',
+    install_requires = ["openai==0.27.4", "Requests==2.28.2", "pyyaml==6.0"]   #这个项目依赖的第三方库
 )
```

