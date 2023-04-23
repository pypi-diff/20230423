# Comparing `tmp/nonebot-plugin-mcqq-1.1.5.post4.tar.gz` & `tmp/nonebot-plugin-mcqq-1.1.5.post5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-mcqq-1.1.5.post4.tar", last modified: Sun Apr 23 07:51:49 2023, max compression
+gzip compressed data, was "nonebot-plugin-mcqq-1.1.5.post5.tar", last modified: Sun Apr 23 10:04:49 2023, max compression
```

## Comparing `nonebot-plugin-mcqq-1.1.5.post4.tar` & `nonebot-plugin-mcqq-1.1.5.post5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 07:51:49.297675 nonebot-plugin-mcqq-1.1.5.post4/
--rw-rw-rw-   0        0        0    35184 2022-08-07 15:18:53.000000 nonebot-plugin-mcqq-1.1.5.post4/LICENSE
--rw-rw-rw-   0        0        0     3025 2023-04-23 07:51:49.297675 nonebot-plugin-mcqq-1.1.5.post4/PKG-INFO
--rw-rw-rw-   0        0        0     2524 2023-04-23 07:50:03.000000 nonebot-plugin-mcqq-1.1.5.post4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 07:51:49.293672 nonebot-plugin-mcqq-1.1.5.post4/nonebot_plugin_mcqq/
--rw-rw-rw-   0        0        0     1786 2023-04-23 07:24:20.000000 nonebot-plugin-mcqq-1.1.5.post4/nonebot_plugin_mcqq/__init__.py
--rw-rw-rw-   0        0        0     2847 2023-04-23 06:12:28.000000 nonebot-plugin-mcqq-1.1.5.post4/nonebot_plugin_mcqq/data_source.py
--rw-rw-rw-   0        0        0     1024 2023-04-22 05:52:16.000000 nonebot-plugin-mcqq-1.1.5.post4/nonebot_plugin_mcqq/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-23 07:51:49.296674 nonebot-plugin-mcqq-1.1.5.post4/nonebot_plugin_mcqq.egg-info/
--rw-rw-rw-   0        0        0     3025 2023-04-23 07:51:49.000000 nonebot-plugin-mcqq-1.1.5.post4/nonebot_plugin_mcqq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      336 2023-04-23 07:51:49.000000 nonebot-plugin-mcqq-1.1.5.post4/nonebot_plugin_mcqq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 07:51:49.000000 nonebot-plugin-mcqq-1.1.5.post4/nonebot_plugin_mcqq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      136 2023-04-23 07:51:49.000000 nonebot-plugin-mcqq-1.1.5.post4/nonebot_plugin_mcqq.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-04-23 07:51:49.000000 nonebot-plugin-mcqq-1.1.5.post4/nonebot_plugin_mcqq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 07:51:49.298676 nonebot-plugin-mcqq-1.1.5.post4/setup.cfg
--rw-rw-rw-   0        0        0     1246 2023-04-23 07:51:34.000000 nonebot-plugin-mcqq-1.1.5.post4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 10:04:49.023323 nonebot-plugin-mcqq-1.1.5.post5/
+-rw-rw-rw-   0        0        0    35184 2022-08-07 15:18:53.000000 nonebot-plugin-mcqq-1.1.5.post5/LICENSE
+-rw-rw-rw-   0        0        0     3004 2023-04-23 10:04:49.023323 nonebot-plugin-mcqq-1.1.5.post5/PKG-INFO
+-rw-rw-rw-   0        0        0     2503 2023-04-23 10:04:21.000000 nonebot-plugin-mcqq-1.1.5.post5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 10:04:49.018319 nonebot-plugin-mcqq-1.1.5.post5/nonebot_plugin_mcqq/
+-rw-rw-rw-   0        0        0     1786 2023-04-23 07:24:20.000000 nonebot-plugin-mcqq-1.1.5.post5/nonebot_plugin_mcqq/__init__.py
+-rw-rw-rw-   0        0        0     2847 2023-04-23 06:12:28.000000 nonebot-plugin-mcqq-1.1.5.post5/nonebot_plugin_mcqq/data_source.py
+-rw-rw-rw-   0        0        0     1024 2023-04-22 05:52:16.000000 nonebot-plugin-mcqq-1.1.5.post5/nonebot_plugin_mcqq/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-23 10:04:49.022321 nonebot-plugin-mcqq-1.1.5.post5/nonebot_plugin_mcqq.egg-info/
+-rw-rw-rw-   0        0        0     3004 2023-04-23 10:04:48.000000 nonebot-plugin-mcqq-1.1.5.post5/nonebot_plugin_mcqq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      336 2023-04-23 10:04:49.000000 nonebot-plugin-mcqq-1.1.5.post5/nonebot_plugin_mcqq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 10:04:49.000000 nonebot-plugin-mcqq-1.1.5.post5/nonebot_plugin_mcqq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      136 2023-04-23 10:04:49.000000 nonebot-plugin-mcqq-1.1.5.post5/nonebot_plugin_mcqq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-04-23 10:04:49.000000 nonebot-plugin-mcqq-1.1.5.post5/nonebot_plugin_mcqq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 10:04:49.023323 nonebot-plugin-mcqq-1.1.5.post5/setup.cfg
+-rw-rw-rw-   0        0        0     1244 2023-04-23 10:03:54.000000 nonebot-plugin-mcqq-1.1.5.post5/setup.py
```

### Comparing `nonebot-plugin-mcqq-1.1.5.post4/LICENSE` & `nonebot-plugin-mcqq-1.1.5.post5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcqq-1.1.5.post4/PKG-INFO` & `nonebot-plugin-mcqq-1.1.5.post5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mcqq
-Version: 1.1.5.post4
+Version: 1.1.5.post5
 Summary: 基于NoneBot的QQ群聊与Minecraft Server消息互通插件
 Home-page: https://github.com/17TheWord/nonebot-plugin-mcqq
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -25,19 +25,19 @@
 - [正在不断更新的文档](https://17theword.github.io/mc_qq/)
 
 # 支持的服务端列表
 
 - Spigot
     - `MC_QQ_Spigot_XXX.jar` + `nonebot-plugin-mcqq`
 - MinecraftServer
-    - `MC_QQ_Minecraft_Server` + `nonebot-plugin-mcqq-mcrcon`
+    - `MC_QQ_Minecraft_Server` + `nonebot-plugin-mcqq`
 - ForgeServer
-    - `MC_QQ_Minecraft_Server` + `nonebot-plugin-mcqq-mcrcon`
+    - `MC_QQ_Minecraft_Server` + `nonebot-plugin-mcqq`
 - Fabric
-    - `MC_QQ_Minecraft_Server` + `nonebot-plugin-mcqq-mcrcon`
+    - `MC_QQ_Minecraft_Server` + `nonebot-plugin-mcqq`
 
 # 功能
 
 - 推送消息列表
     - 服务器 -> QQ
         - [x] 加入 / 离开 服务器消息
         - [x] 玩家聊天信息
```

### Comparing `nonebot-plugin-mcqq-1.1.5.post4/README.md` & `nonebot-plugin-mcqq-1.1.5.post5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 - [正在不断更新的文档](https://17theword.github.io/mc_qq/)
 
 # 支持的服务端列表
 
 - Spigot
     - `MC_QQ_Spigot_XXX.jar` + `nonebot-plugin-mcqq`
 - MinecraftServer
-    - `MC_QQ_Minecraft_Server` + `nonebot-plugin-mcqq-mcrcon`
+    - `MC_QQ_Minecraft_Server` + `nonebot-plugin-mcqq`
 - ForgeServer
-    - `MC_QQ_Minecraft_Server` + `nonebot-plugin-mcqq-mcrcon`
+    - `MC_QQ_Minecraft_Server` + `nonebot-plugin-mcqq`
 - Fabric
-    - `MC_QQ_Minecraft_Server` + `nonebot-plugin-mcqq-mcrcon`
+    - `MC_QQ_Minecraft_Server` + `nonebot-plugin-mcqq`
 
 # 功能
 
 - 推送消息列表
     - 服务器 -> QQ
         - [x] 加入 / 离开 服务器消息
         - [x] 玩家聊天信息
```

### Comparing `nonebot-plugin-mcqq-1.1.5.post4/nonebot_plugin_mcqq/__init__.py` & `nonebot-plugin-mcqq-1.1.5.post5/nonebot_plugin_mcqq/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcqq-1.1.5.post4/nonebot_plugin_mcqq/data_source.py` & `nonebot-plugin-mcqq-1.1.5.post5/nonebot_plugin_mcqq/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcqq-1.1.5.post4/nonebot_plugin_mcqq/utils.py` & `nonebot-plugin-mcqq-1.1.5.post5/nonebot_plugin_mcqq/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcqq-1.1.5.post4/nonebot_plugin_mcqq.egg-info/PKG-INFO` & `nonebot-plugin-mcqq-1.1.5.post5/nonebot_plugin_mcqq.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mcqq
-Version: 1.1.5.post4
+Version: 1.1.5.post5
 Summary: 基于NoneBot的QQ群聊与Minecraft Server消息互通插件
 Home-page: https://github.com/17TheWord/nonebot-plugin-mcqq
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -25,19 +25,19 @@
 - [正在不断更新的文档](https://17theword.github.io/mc_qq/)
 
 # 支持的服务端列表
 
 - Spigot
     - `MC_QQ_Spigot_XXX.jar` + `nonebot-plugin-mcqq`
 - MinecraftServer
-    - `MC_QQ_Minecraft_Server` + `nonebot-plugin-mcqq-mcrcon`
+    - `MC_QQ_Minecraft_Server` + `nonebot-plugin-mcqq`
 - ForgeServer
-    - `MC_QQ_Minecraft_Server` + `nonebot-plugin-mcqq-mcrcon`
+    - `MC_QQ_Minecraft_Server` + `nonebot-plugin-mcqq`
 - Fabric
-    - `MC_QQ_Minecraft_Server` + `nonebot-plugin-mcqq-mcrcon`
+    - `MC_QQ_Minecraft_Server` + `nonebot-plugin-mcqq`
 
 # 功能
 
 - 推送消息列表
     - 服务器 -> QQ
         - [x] 加入 / 离开 服务器消息
         - [x] 玩家聊天信息
```

### Comparing `nonebot-plugin-mcqq-1.1.5.post4/setup.py` & `nonebot-plugin-mcqq-1.1.5.post5/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="nonebot-plugin-mcqq",  # 项目名称，保证它的唯一性，不要跟已存在的包名冲突即可
-    version="1.1.5-post4",  # 程序版本
+    version="1.1.5-post5",  # 程序版本
     author="17TheWord",  # 项目作者
     author_email="17theword@gmail.com",  # 作者邮件
     description="基于NoneBot的QQ群聊与Minecraft Server消息互通插件",  # 项目的一句话描述
     long_description=long_description,  # 加长版描述？
     long_description_content_type="text/markdown",  # 描述使用Markdown
     url="https://github.com/17TheWord/nonebot-plugin-mcqq",  # 项目地址
     packages=setuptools.find_packages(),  # 无需修改
     classifiers=[
         "Programming Language :: Python :: 3.9",  # 使用Python3.10
         "License :: OSI Approved :: GNU Affero General Public License v3",  # 开源协议
-        "Operating System :: OS Independent",
+        "Operating System :: OS Independent"
     ],
     install_requires=[
-        'mcqq-tool>=0.0.4',
-        'nonebot2>=2.0.0rc3',
+        'mcqq-tool>=0.0.5',
+        'nonebot2>=2.0.0rc4',
         'nonebot-adapter-onebot>=2.1.1',
         'nonebot-plugin-guild-patch>=0.2.0',
         'websockets>=10.3',
         'aio-mc-rcon>=3.2.0'
-    ],
+    ]
 )
```

