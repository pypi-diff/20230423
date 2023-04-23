# Comparing `tmp/AISimuToolKit-0.0.5.tar.gz` & `tmp/AISimuToolKit-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AISimuToolKit-0.0.5.tar", last modified: Sun Apr 23 09:02:07 2023, max compression
+gzip compressed data, was "AISimuToolKit-0.0.6.tar", last modified: Sun Apr 23 13:50:25 2023, max compression
```

## Comparing `AISimuToolKit-0.0.5.tar` & `AISimuToolKit-0.0.6.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-23 09:02:07.866675 AISimuToolKit-0.0.5/
-drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-23 09:02:07.862675 AISimuToolKit-0.0.5/AISimuToolKit/
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)       85 2023-04-22 08:15:55.000000 AISimuToolKit-0.0.5/AISimuToolKit/__init__.py
-drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-23 09:02:07.862675 AISimuToolKit-0.0.5/AISimuToolKit/exp/
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)      112 2023-04-22 08:15:55.000000 AISimuToolKit-0.0.5/AISimuToolKit/exp/__init__.py
-drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-23 09:02:07.866675 AISimuToolKit-0.0.5/AISimuToolKit/exp/actions/
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)      307 2023-04-22 08:15:55.000000 AISimuToolKit-0.0.5/AISimuToolKit/exp/actions/__init__.py
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)      434 2023-04-22 08:28:12.000000 AISimuToolKit-0.0.5/AISimuToolKit/exp/actions/base_action.py
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     1317 2023-04-22 08:28:12.000000 AISimuToolKit-0.0.5/AISimuToolKit/exp/actions/finetune_action.py
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     1273 2023-04-22 08:28:12.000000 AISimuToolKit-0.0.5/AISimuToolKit/exp/actions/instruct_action.py
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     2091 2023-04-22 08:28:12.000000 AISimuToolKit-0.0.5/AISimuToolKit/exp/actions/probe_action.py
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     2410 2023-04-22 08:28:12.000000 AISimuToolKit-0.0.5/AISimuToolKit/exp/actions/reflection_action.py
-drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-23 09:02:07.866675 AISimuToolKit-0.0.5/AISimuToolKit/exp/agents/
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)       83 2023-04-22 08:15:55.000000 AISimuToolKit-0.0.5/AISimuToolKit/exp/agents/__init__.py
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)      610 2023-04-22 08:28:12.000000 AISimuToolKit-0.0.5/AISimuToolKit/exp/agents/agent.py
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     2769 2023-04-22 08:15:55.000000 AISimuToolKit-0.0.5/AISimuToolKit/exp/agents/memory.py
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     6732 2023-04-22 08:28:12.000000 AISimuToolKit-0.0.5/AISimuToolKit/exp/experiment.py
-drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-23 09:02:07.866675 AISimuToolKit-0.0.5/AISimuToolKit/model/
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)      237 2023-04-23 08:27:14.000000 AISimuToolKit-0.0.5/AISimuToolKit/model/__init__.py
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     9470 2023-04-22 08:28:12.000000 AISimuToolKit-0.0.5/AISimuToolKit/model/model.py
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     2244 2023-04-22 08:28:12.000000 AISimuToolKit-0.0.5/AISimuToolKit/model/register.py
-drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-23 09:02:07.866675 AISimuToolKit-0.0.5/AISimuToolKit/store/
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)       39 2023-04-23 08:55:06.000000 AISimuToolKit-0.0.5/AISimuToolKit/store/__init__.py
-drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-23 09:02:07.866675 AISimuToolKit-0.0.5/AISimuToolKit/store/text/
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)       47 2023-04-23 08:54:42.000000 AISimuToolKit-0.0.5/AISimuToolKit/store/text/__init__.py
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     6494 2023-04-22 08:15:55.000000 AISimuToolKit-0.0.5/AISimuToolKit/store/text/logger.py
-drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-23 09:02:07.866675 AISimuToolKit-0.0.5/AISimuToolKit/utils/
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)      559 2023-04-22 08:15:55.000000 AISimuToolKit-0.0.5/AISimuToolKit/utils/__init__.py
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     1369 2023-04-22 08:15:55.000000 AISimuToolKit-0.0.5/AISimuToolKit/utils/utils.py
-drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-23 09:02:07.862675 AISimuToolKit-0.0.5/AISimuToolKit.egg-info/
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)      407 2023-04-23 09:02:07.000000 AISimuToolKit-0.0.5/AISimuToolKit.egg-info/PKG-INFO
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)      902 2023-04-23 09:02:07.000000 AISimuToolKit-0.0.5/AISimuToolKit.egg-info/SOURCES.txt
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)        1 2023-04-23 09:02:07.000000 AISimuToolKit-0.0.5/AISimuToolKit.egg-info/dependency_links.txt
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)       44 2023-04-23 09:02:07.000000 AISimuToolKit-0.0.5/AISimuToolKit.egg-info/requires.txt
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)       14 2023-04-23 09:02:07.000000 AISimuToolKit-0.0.5/AISimuToolKit.egg-info/top_level.txt
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)      407 2023-04-23 09:02:07.866675 AISimuToolKit-0.0.5/PKG-INFO
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)       38 2023-04-23 09:02:07.866675 AISimuToolKit-0.0.5/setup.cfg
--rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     1011 2023-04-23 09:02:05.000000 AISimuToolKit-0.0.5/setup.py
+drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-23 13:50:25.662062 AISimuToolKit-0.0.6/
+drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-23 13:50:25.658062 AISimuToolKit-0.0.6/AISimuToolKit/
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)       85 2023-04-22 08:15:55.000000 AISimuToolKit-0.0.6/AISimuToolKit/__init__.py
+drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-23 13:50:25.658062 AISimuToolKit-0.0.6/AISimuToolKit/exp/
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)      112 2023-04-22 08:15:55.000000 AISimuToolKit-0.0.6/AISimuToolKit/exp/__init__.py
+drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-23 13:50:25.658062 AISimuToolKit-0.0.6/AISimuToolKit/exp/actions/
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)      307 2023-04-22 08:15:55.000000 AISimuToolKit-0.0.6/AISimuToolKit/exp/actions/__init__.py
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)      434 2023-04-22 08:28:12.000000 AISimuToolKit-0.0.6/AISimuToolKit/exp/actions/base_action.py
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     1317 2023-04-22 08:28:12.000000 AISimuToolKit-0.0.6/AISimuToolKit/exp/actions/finetune_action.py
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     1273 2023-04-22 08:28:12.000000 AISimuToolKit-0.0.6/AISimuToolKit/exp/actions/instruct_action.py
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     2091 2023-04-22 08:28:12.000000 AISimuToolKit-0.0.6/AISimuToolKit/exp/actions/probe_action.py
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     2410 2023-04-22 08:28:12.000000 AISimuToolKit-0.0.6/AISimuToolKit/exp/actions/reflection_action.py
+drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-23 13:50:25.658062 AISimuToolKit-0.0.6/AISimuToolKit/exp/agents/
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)       83 2023-04-22 08:15:55.000000 AISimuToolKit-0.0.6/AISimuToolKit/exp/agents/__init__.py
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)      610 2023-04-22 08:28:12.000000 AISimuToolKit-0.0.6/AISimuToolKit/exp/agents/agent.py
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     2769 2023-04-22 08:15:55.000000 AISimuToolKit-0.0.6/AISimuToolKit/exp/agents/memory.py
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     6732 2023-04-22 08:28:12.000000 AISimuToolKit-0.0.6/AISimuToolKit/exp/experiment.py
+drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-23 13:50:25.658062 AISimuToolKit-0.0.6/AISimuToolKit/model/
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)      237 2023-04-23 08:27:14.000000 AISimuToolKit-0.0.6/AISimuToolKit/model/__init__.py
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     9510 2023-04-23 13:44:17.000000 AISimuToolKit-0.0.6/AISimuToolKit/model/model.py
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     2352 2023-04-23 13:48:33.000000 AISimuToolKit-0.0.6/AISimuToolKit/model/register.py
+drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-23 13:50:25.658062 AISimuToolKit-0.0.6/AISimuToolKit/store/
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)       39 2023-04-23 08:55:06.000000 AISimuToolKit-0.0.6/AISimuToolKit/store/__init__.py
+drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-23 13:50:25.658062 AISimuToolKit-0.0.6/AISimuToolKit/store/text/
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)       47 2023-04-23 08:54:42.000000 AISimuToolKit-0.0.6/AISimuToolKit/store/text/__init__.py
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     6494 2023-04-22 08:15:55.000000 AISimuToolKit-0.0.6/AISimuToolKit/store/text/logger.py
+drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-23 13:50:25.662062 AISimuToolKit-0.0.6/AISimuToolKit/utils/
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)      559 2023-04-22 08:15:55.000000 AISimuToolKit-0.0.6/AISimuToolKit/utils/__init__.py
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     1369 2023-04-22 08:15:55.000000 AISimuToolKit-0.0.6/AISimuToolKit/utils/utils.py
+drwxrwxr-x   0 renmengjie2021  (1054) renmengjie2021  (1054)        0 2023-04-23 13:50:25.658062 AISimuToolKit-0.0.6/AISimuToolKit.egg-info/
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)      407 2023-04-23 13:50:25.000000 AISimuToolKit-0.0.6/AISimuToolKit.egg-info/PKG-INFO
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)      902 2023-04-23 13:50:25.000000 AISimuToolKit-0.0.6/AISimuToolKit.egg-info/SOURCES.txt
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)        1 2023-04-23 13:50:25.000000 AISimuToolKit-0.0.6/AISimuToolKit.egg-info/dependency_links.txt
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)       44 2023-04-23 13:50:25.000000 AISimuToolKit-0.0.6/AISimuToolKit.egg-info/requires.txt
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)       14 2023-04-23 13:50:25.000000 AISimuToolKit-0.0.6/AISimuToolKit.egg-info/top_level.txt
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)      407 2023-04-23 13:50:25.662062 AISimuToolKit-0.0.6/PKG-INFO
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)       38 2023-04-23 13:50:25.662062 AISimuToolKit-0.0.6/setup.cfg
+-rw-rw-r--   0 renmengjie2021  (1054) renmengjie2021  (1054)     1011 2023-04-23 13:50:23.000000 AISimuToolKit-0.0.6/setup.py
```

### Comparing `AISimuToolKit-0.0.5/AISimuToolKit/exp/actions/finetune_action.py` & `AISimuToolKit-0.0.6/AISimuToolKit/exp/actions/finetune_action.py`

 * *Files identical despite different names*

### Comparing `AISimuToolKit-0.0.5/AISimuToolKit/exp/actions/instruct_action.py` & `AISimuToolKit-0.0.6/AISimuToolKit/exp/actions/instruct_action.py`

 * *Files identical despite different names*

### Comparing `AISimuToolKit-0.0.5/AISimuToolKit/exp/actions/probe_action.py` & `AISimuToolKit-0.0.6/AISimuToolKit/exp/actions/probe_action.py`

 * *Files identical despite different names*

### Comparing `AISimuToolKit-0.0.5/AISimuToolKit/exp/actions/reflection_action.py` & `AISimuToolKit-0.0.6/AISimuToolKit/exp/actions/reflection_action.py`

 * *Files identical despite different names*

### Comparing `AISimuToolKit-0.0.5/AISimuToolKit/exp/agents/agent.py` & `AISimuToolKit-0.0.6/AISimuToolKit/exp/agents/agent.py`

 * *Files identical despite different names*

### Comparing `AISimuToolKit-0.0.5/AISimuToolKit/exp/agents/memory.py` & `AISimuToolKit-0.0.6/AISimuToolKit/exp/agents/memory.py`

 * *Files identical despite different names*

### Comparing `AISimuToolKit-0.0.5/AISimuToolKit/exp/experiment.py` & `AISimuToolKit-0.0.6/AISimuToolKit/exp/experiment.py`

 * *Files identical despite different names*

### Comparing `AISimuToolKit-0.0.5/AISimuToolKit/model/model.py` & `AISimuToolKit-0.0.6/AISimuToolKit/model/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,19 +42,20 @@
 
 
 # @ModelApiRegister.register("chatgpt")
 class GPT_35_API(PublicApiBase):
     
     def __new__(cls, 
                 urls: List[str], 
+                conf: dict,
                 *args, **kwargs):
         if cls._instance is None:
             cls._instance = super().__new__(cls)
             openai.api_base = urls[0]
-            openai.api_key = ""
+            openai.api_key = conf['key'][0]
         return cls._instance
 
     # TODO 加入多轮对话
     # TODO 设置system
     # TODO 测试长对话，目前没有找到返回为length的例子
     def chat(self, query: str, config: dict, *args, **kwargs):
         """
```

### Comparing `AISimuToolKit-0.0.5/AISimuToolKit/model/register.py` & `AISimuToolKit-0.0.6/AISimuToolKit/model/register.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,11 +50,12 @@
     conf = parse_yaml_config(path=model_config)
     model_register = ApiRegister()
     for agent_id, model_settings in agent_model_dict.items():
         model_name = model_settings["model_name"]
         inner_model_name = get_model_by_name(ModelNameDict, model_name)
         model_register[int(agent_id)] = inner_model_name(exp=exp_id,
                                                          agents=agents,
-                                                         urls=conf[model_name]['url'])
+                                                         urls=conf[model_name]['url'],
+                                                         conf=conf[model_name])
     if 'GPT-3.5-turbo' in conf.keys():
-        model_register[-1] = GPT_35_API(urls=conf['GPT-3.5-turbo']['url'])
+        model_register[-1] = GPT_35_API(urls=conf['GPT-3.5-turbo']['url'], conf=conf['GPT-3.5-turbo'])
     return model_register
```

### Comparing `AISimuToolKit-0.0.5/AISimuToolKit/store/text/logger.py` & `AISimuToolKit-0.0.6/AISimuToolKit/store/text/logger.py`

 * *Files identical despite different names*

### Comparing `AISimuToolKit-0.0.5/AISimuToolKit/utils/__init__.py` & `AISimuToolKit-0.0.6/AISimuToolKit/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `AISimuToolKit-0.0.5/AISimuToolKit/utils/utils.py` & `AISimuToolKit-0.0.6/AISimuToolKit/utils/utils.py`

 * *Files identical despite different names*

### Comparing `AISimuToolKit-0.0.5/AISimuToolKit.egg-info/SOURCES.txt` & `AISimuToolKit-0.0.6/AISimuToolKit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AISimuToolKit-0.0.5/setup.py` & `AISimuToolKit-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 #-*- coding:utf-8 -*-
 
 from setuptools import setup, find_packages            #这个包没有的可以pip一下
 
 setup(
     name = "AISimuToolKit",      #这里是pip项目发布的名称
-    version = "0.0.5",  #版本号，数值大的会优先被pip
+    version = "0.0.6",  #版本号，数值大的会优先被pip
     keywords = ["pip", "AISimuToolKit"],			# 关键字
     description = "ICIP's private utils.",	# 描述
     long_description = "ICIP's private utils. The development version will be released when it is sufficiently refined",
     license = "MIT Licence",		# 许可证
     url = "http://git.cipsup.cn/aisimulationplatform/toolkit/aisimulation",     #项目相关文件地址，一般是github项目地址即可
     author = "Ren & Guo",			# 作者
     author_email = "renmengjie22@mails.ucas.ac.cn",
```

