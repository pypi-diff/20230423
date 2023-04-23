# Comparing `tmp/nonebot-plugin-mcqq-1.1.5.post3.tar.gz` & `tmp/nonebot-plugin-mcqq-1.1.5.post4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-mcqq-1.1.5.post3.tar", last modified: Sun Apr 23 07:29:14 2023, max compression
+gzip compressed data, was "nonebot-plugin-mcqq-1.1.5.post4.tar", last modified: Sun Apr 23 07:51:49 2023, max compression
```

## Comparing `nonebot-plugin-mcqq-1.1.5.post3.tar` & `nonebot-plugin-mcqq-1.1.5.post4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 07:29:14.738019 nonebot-plugin-mcqq-1.1.5.post3/
--rw-rw-rw-   0        0        0    35184 2022-08-07 15:18:53.000000 nonebot-plugin-mcqq-1.1.5.post3/LICENSE
--rw-rw-rw-   0        0        0     2647 2023-04-23 07:29:14.738019 nonebot-plugin-mcqq-1.1.5.post3/PKG-INFO
--rw-rw-rw-   0        0        0     2146 2023-01-26 17:04:35.000000 nonebot-plugin-mcqq-1.1.5.post3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 07:29:14.734015 nonebot-plugin-mcqq-1.1.5.post3/nonebot_plugin_mcqq/
--rw-rw-rw-   0        0        0     1786 2023-04-23 07:24:20.000000 nonebot-plugin-mcqq-1.1.5.post3/nonebot_plugin_mcqq/__init__.py
--rw-rw-rw-   0        0        0     2847 2023-04-23 06:12:28.000000 nonebot-plugin-mcqq-1.1.5.post3/nonebot_plugin_mcqq/data_source.py
--rw-rw-rw-   0        0        0     1024 2023-04-22 05:52:16.000000 nonebot-plugin-mcqq-1.1.5.post3/nonebot_plugin_mcqq/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-23 07:29:14.737018 nonebot-plugin-mcqq-1.1.5.post3/nonebot_plugin_mcqq.egg-info/
--rw-rw-rw-   0        0        0     2647 2023-04-23 07:29:14.000000 nonebot-plugin-mcqq-1.1.5.post3/nonebot_plugin_mcqq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      336 2023-04-23 07:29:14.000000 nonebot-plugin-mcqq-1.1.5.post3/nonebot_plugin_mcqq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 07:29:14.000000 nonebot-plugin-mcqq-1.1.5.post3/nonebot_plugin_mcqq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      117 2023-04-23 07:29:14.000000 nonebot-plugin-mcqq-1.1.5.post3/nonebot_plugin_mcqq.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-04-23 07:29:14.000000 nonebot-plugin-mcqq-1.1.5.post3/nonebot_plugin_mcqq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 07:29:14.738019 nonebot-plugin-mcqq-1.1.5.post3/setup.cfg
--rw-rw-rw-   0        0        0     1216 2023-04-23 07:29:07.000000 nonebot-plugin-mcqq-1.1.5.post3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 07:51:49.297675 nonebot-plugin-mcqq-1.1.5.post4/
+-rw-rw-rw-   0        0        0    35184 2022-08-07 15:18:53.000000 nonebot-plugin-mcqq-1.1.5.post4/LICENSE
+-rw-rw-rw-   0        0        0     3025 2023-04-23 07:51:49.297675 nonebot-plugin-mcqq-1.1.5.post4/PKG-INFO
+-rw-rw-rw-   0        0        0     2524 2023-04-23 07:50:03.000000 nonebot-plugin-mcqq-1.1.5.post4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 07:51:49.293672 nonebot-plugin-mcqq-1.1.5.post4/nonebot_plugin_mcqq/
+-rw-rw-rw-   0        0        0     1786 2023-04-23 07:24:20.000000 nonebot-plugin-mcqq-1.1.5.post4/nonebot_plugin_mcqq/__init__.py
+-rw-rw-rw-   0        0        0     2847 2023-04-23 06:12:28.000000 nonebot-plugin-mcqq-1.1.5.post4/nonebot_plugin_mcqq/data_source.py
+-rw-rw-rw-   0        0        0     1024 2023-04-22 05:52:16.000000 nonebot-plugin-mcqq-1.1.5.post4/nonebot_plugin_mcqq/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-23 07:51:49.296674 nonebot-plugin-mcqq-1.1.5.post4/nonebot_plugin_mcqq.egg-info/
+-rw-rw-rw-   0        0        0     3025 2023-04-23 07:51:49.000000 nonebot-plugin-mcqq-1.1.5.post4/nonebot_plugin_mcqq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      336 2023-04-23 07:51:49.000000 nonebot-plugin-mcqq-1.1.5.post4/nonebot_plugin_mcqq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 07:51:49.000000 nonebot-plugin-mcqq-1.1.5.post4/nonebot_plugin_mcqq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      136 2023-04-23 07:51:49.000000 nonebot-plugin-mcqq-1.1.5.post4/nonebot_plugin_mcqq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-04-23 07:51:49.000000 nonebot-plugin-mcqq-1.1.5.post4/nonebot_plugin_mcqq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 07:51:49.298676 nonebot-plugin-mcqq-1.1.5.post4/setup.cfg
+-rw-rw-rw-   0        0        0     1246 2023-04-23 07:51:34.000000 nonebot-plugin-mcqq-1.1.5.post4/setup.py
```

### Comparing `nonebot-plugin-mcqq-1.1.5.post3/LICENSE` & `nonebot-plugin-mcqq-1.1.5.post4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcqq-1.1.5.post3/PKG-INFO` & `nonebot-plugin-mcqq-1.1.5.post4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,68 +1,66 @@
-Metadata-Version: 2.1
-Name: nonebot-plugin-mcqq
-Version: 1.1.5.post3
-Summary: 基于NoneBot的QQ群聊与Minecraft Server消息互通插件
-Home-page: https://github.com/17TheWord/nonebot-plugin-mcqq
-Author: 17TheWord
-Author-email: 17theword@gmail.com
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![nonebot-plugin-mcqq](https://socialify.git.ci/17TheWord/nonebot-plugin-mcqq/image?description=1&font=Inter&forks=1&issues=1&language=1&logo=https%3A%2F%2Favatars.githubusercontent.com%2F17TheWord&owner=1&pattern=Plus&stargazers=1&theme=Dark)](https://17theword.github.io/mc_qq/)
 
 # NoneBot-Plugin-MCQQ
 
-基于 `NoneBot` 的与 `Minecraft Bot` 互通消息插件
+基于 `NoneBot` 的与 `Minecraft Server` 互通消息插件
 
 - 支持QQ群、QQ频道
 - 支持多个服务器与多个群聊的互通
 
 # 文档
 
 - [正在不断更新的文档](https://17theword.github.io/mc_qq/)
 
 # 支持的服务端列表
 
 - Spigot
-  - `MC_QQ_Spigot_XXX.jar` + `nonebot-plugin-mcqq`
-  - `MC_QQ_Spigot_XXX.jar` + `nonebot-plugin-mcqq-mcrcon`
+    - `MC_QQ_Spigot_XXX.jar` + `nonebot-plugin-mcqq`
 - MinecraftServer
-  -  `MC_QQ_Minecraft_Server` + `nonebot-plugin-mcqq-mcrcon`
+    - `MC_QQ_Minecraft_Server` + `nonebot-plugin-mcqq-mcrcon`
 - ForgeServer
-  -  `MC_QQ_Minecraft_Server` + `nonebot-plugin-mcqq-mcrcon`
+    - `MC_QQ_Minecraft_Server` + `nonebot-plugin-mcqq-mcrcon`
 - Fabric
-  -  `MC_QQ_Minecraft_Server` + `nonebot-plugin-mcqq-mcrcon`
+    - `MC_QQ_Minecraft_Server` + `nonebot-plugin-mcqq-mcrcon`
 
 # 功能
 
 - 推送消息列表
-  - 服务器 -> QQ
-    - [x] 加入 / 离开 服务器消息
-    - [x] 玩家聊天信息
-    - [x] 玩家死亡信息（死亡信息为英文，计划使用翻译解决。非插件服务端不适用。）
-  - QQ -> 服务器
-    - [x] 指令（`nonebot-plugin-mcqq-mcrcon` 可用）
-    - [x] 群员聊天文本
-    - [x] 图片、视频等内容转换为 `[图片]`、`[视频]`
+    - 服务器 -> QQ
+        - [x] 加入 / 离开 服务器消息
+        - [x] 玩家聊天信息
+        - [x] 玩家死亡信息（死亡信息为英文，非插件服务端不适用。）
+    - QQ -> 服务器
+        - [x] 指令
+        - [x] 群员聊天文本
+        - [x] 图片、视频等内容转换为 `[图片]`、`[视频]`
 
 - 特殊消息支持
-  - 群聊
-    - [x] @ 消息
-    - [x] 回复消息（转换成@消息）
-  - 频道
-    - [x] @ 消息
-    - [x] 回复消息（转换成@消息）
-  - 未支持的消息已被替换，如： `[图片]`、 `[视频]` 等等
+    - 群聊
+        - [x] @ 消息
+        - [x] 回复消息（转换成@消息）
+    - 频道
+        - [x] @ 消息
+        - [x] 回复消息（转换成@消息）
+    - 未支持的消息已被替换，如： `[图片]`、 `[视频]` 等等
 
 # 特别感谢
+
 - [@SK-415](https://github.com/SK-415) ：感谢SK佬给予许多优秀的建议和耐心的解答。
 - [@zhz-红石头](https://github.com/zhzhongshi) ：感谢红石头在代码上的帮助
 - [NoneBot2](https://github.com/nonebot/nonebot2)： 插件使用的开发框架。
 - [go-cqhttp](https://github.com/Mrs4s/go-cqhttp)： 稳定完善的 CQHTTP 实现。
 
 # 二创
 
 - [mcqq服主版](https://github.com/KarisAya/nonebot_plugin_mcqq_server) 采用本地读取log信息的方法的Minecraft Server互通消息的插件
+
+## 贡献与支持
+
+觉得好用可以给这个项目点个 `Star` 或者去 [爱发电](https://afdian.net/a/17TheWord) 投喂我。
+
+有意见或者建议也欢迎提交 [Issues](https://github.com/17TheWord/nonebot-plugin-mcqq/issues)
+和 [Pull requests](https://github.com/17TheWord/nonebot-plugin-mcqq/pulls)。
+
+## 许可证
+
+本项目使用 [GNU AGPLv3](https://choosealicense.com/licenses/agpl-3.0/) 作为开源许可证。
```

### Comparing `nonebot-plugin-mcqq-1.1.5.post3/README.md` & `nonebot-plugin-mcqq-1.1.5.post4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,79 @@
+Metadata-Version: 2.1
+Name: nonebot-plugin-mcqq
+Version: 1.1.5.post4
+Summary: 基于NoneBot的QQ群聊与Minecraft Server消息互通插件
+Home-page: https://github.com/17TheWord/nonebot-plugin-mcqq
+Author: 17TheWord
+Author-email: 17theword@gmail.com
+Classifier: Programming Language :: Python :: 3.9
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![nonebot-plugin-mcqq](https://socialify.git.ci/17TheWord/nonebot-plugin-mcqq/image?description=1&font=Inter&forks=1&issues=1&language=1&logo=https%3A%2F%2Favatars.githubusercontent.com%2F17TheWord&owner=1&pattern=Plus&stargazers=1&theme=Dark)](https://17theword.github.io/mc_qq/)
 
 # NoneBot-Plugin-MCQQ
 
-基于 `NoneBot` 的与 `Minecraft Bot` 互通消息插件
+基于 `NoneBot` 的与 `Minecraft Server` 互通消息插件
 
 - 支持QQ群、QQ频道
 - 支持多个服务器与多个群聊的互通
 
 # 文档
 
 - [正在不断更新的文档](https://17theword.github.io/mc_qq/)
 
 # 支持的服务端列表
 
 - Spigot
-  - `MC_QQ_Spigot_XXX.jar` + `nonebot-plugin-mcqq`
-  - `MC_QQ_Spigot_XXX.jar` + `nonebot-plugin-mcqq-mcrcon`
+    - `MC_QQ_Spigot_XXX.jar` + `nonebot-plugin-mcqq`
 - MinecraftServer
-  -  `MC_QQ_Minecraft_Server` + `nonebot-plugin-mcqq-mcrcon`
+    - `MC_QQ_Minecraft_Server` + `nonebot-plugin-mcqq-mcrcon`
 - ForgeServer
-  -  `MC_QQ_Minecraft_Server` + `nonebot-plugin-mcqq-mcrcon`
+    - `MC_QQ_Minecraft_Server` + `nonebot-plugin-mcqq-mcrcon`
 - Fabric
-  -  `MC_QQ_Minecraft_Server` + `nonebot-plugin-mcqq-mcrcon`
+    - `MC_QQ_Minecraft_Server` + `nonebot-plugin-mcqq-mcrcon`
 
 # 功能
 
 - 推送消息列表
-  - 服务器 -> QQ
-    - [x] 加入 / 离开 服务器消息
-    - [x] 玩家聊天信息
-    - [x] 玩家死亡信息（死亡信息为英文，计划使用翻译解决。非插件服务端不适用。）
-  - QQ -> 服务器
-    - [x] 指令（`nonebot-plugin-mcqq-mcrcon` 可用）
-    - [x] 群员聊天文本
-    - [x] 图片、视频等内容转换为 `[图片]`、`[视频]`
+    - 服务器 -> QQ
+        - [x] 加入 / 离开 服务器消息
+        - [x] 玩家聊天信息
+        - [x] 玩家死亡信息（死亡信息为英文，非插件服务端不适用。）
+    - QQ -> 服务器
+        - [x] 指令
+        - [x] 群员聊天文本
+        - [x] 图片、视频等内容转换为 `[图片]`、`[视频]`
 
 - 特殊消息支持
-  - 群聊
-    - [x] @ 消息
-    - [x] 回复消息（转换成@消息）
-  - 频道
-    - [x] @ 消息
-    - [x] 回复消息（转换成@消息）
-  - 未支持的消息已被替换，如： `[图片]`、 `[视频]` 等等
+    - 群聊
+        - [x] @ 消息
+        - [x] 回复消息（转换成@消息）
+    - 频道
+        - [x] @ 消息
+        - [x] 回复消息（转换成@消息）
+    - 未支持的消息已被替换，如： `[图片]`、 `[视频]` 等等
 
 # 特别感谢
+
 - [@SK-415](https://github.com/SK-415) ：感谢SK佬给予许多优秀的建议和耐心的解答。
 - [@zhz-红石头](https://github.com/zhzhongshi) ：感谢红石头在代码上的帮助
 - [NoneBot2](https://github.com/nonebot/nonebot2)： 插件使用的开发框架。
 - [go-cqhttp](https://github.com/Mrs4s/go-cqhttp)： 稳定完善的 CQHTTP 实现。
 
 # 二创
 
 - [mcqq服主版](https://github.com/KarisAya/nonebot_plugin_mcqq_server) 采用本地读取log信息的方法的Minecraft Server互通消息的插件
+
+## 贡献与支持
+
+觉得好用可以给这个项目点个 `Star` 或者去 [爱发电](https://afdian.net/a/17TheWord) 投喂我。
+
+有意见或者建议也欢迎提交 [Issues](https://github.com/17TheWord/nonebot-plugin-mcqq/issues)
+和 [Pull requests](https://github.com/17TheWord/nonebot-plugin-mcqq/pulls)。
+
+## 许可证
+
+本项目使用 [GNU AGPLv3](https://choosealicense.com/licenses/agpl-3.0/) 作为开源许可证。
```

### Comparing `nonebot-plugin-mcqq-1.1.5.post3/nonebot_plugin_mcqq/__init__.py` & `nonebot-plugin-mcqq-1.1.5.post4/nonebot_plugin_mcqq/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcqq-1.1.5.post3/nonebot_plugin_mcqq/data_source.py` & `nonebot-plugin-mcqq-1.1.5.post4/nonebot_plugin_mcqq/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcqq-1.1.5.post3/nonebot_plugin_mcqq/utils.py` & `nonebot-plugin-mcqq-1.1.5.post4/nonebot_plugin_mcqq/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcqq-1.1.5.post3/nonebot_plugin_mcqq.egg-info/PKG-INFO` & `nonebot-plugin-mcqq-1.1.5.post4/nonebot_plugin_mcqq.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,68 +1,79 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mcqq
-Version: 1.1.5.post3
+Version: 1.1.5.post4
 Summary: 基于NoneBot的QQ群聊与Minecraft Server消息互通插件
 Home-page: https://github.com/17TheWord/nonebot-plugin-mcqq
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![nonebot-plugin-mcqq](https://socialify.git.ci/17TheWord/nonebot-plugin-mcqq/image?description=1&font=Inter&forks=1&issues=1&language=1&logo=https%3A%2F%2Favatars.githubusercontent.com%2F17TheWord&owner=1&pattern=Plus&stargazers=1&theme=Dark)](https://17theword.github.io/mc_qq/)
 
 # NoneBot-Plugin-MCQQ
 
-基于 `NoneBot` 的与 `Minecraft Bot` 互通消息插件
+基于 `NoneBot` 的与 `Minecraft Server` 互通消息插件
 
 - 支持QQ群、QQ频道
 - 支持多个服务器与多个群聊的互通
 
 # 文档
 
 - [正在不断更新的文档](https://17theword.github.io/mc_qq/)
 
 # 支持的服务端列表
 
 - Spigot
-  - `MC_QQ_Spigot_XXX.jar` + `nonebot-plugin-mcqq`
-  - `MC_QQ_Spigot_XXX.jar` + `nonebot-plugin-mcqq-mcrcon`
+    - `MC_QQ_Spigot_XXX.jar` + `nonebot-plugin-mcqq`
 - MinecraftServer
-  -  `MC_QQ_Minecraft_Server` + `nonebot-plugin-mcqq-mcrcon`
+    - `MC_QQ_Minecraft_Server` + `nonebot-plugin-mcqq-mcrcon`
 - ForgeServer
-  -  `MC_QQ_Minecraft_Server` + `nonebot-plugin-mcqq-mcrcon`
+    - `MC_QQ_Minecraft_Server` + `nonebot-plugin-mcqq-mcrcon`
 - Fabric
-  -  `MC_QQ_Minecraft_Server` + `nonebot-plugin-mcqq-mcrcon`
+    - `MC_QQ_Minecraft_Server` + `nonebot-plugin-mcqq-mcrcon`
 
 # 功能
 
 - 推送消息列表
-  - 服务器 -> QQ
-    - [x] 加入 / 离开 服务器消息
-    - [x] 玩家聊天信息
-    - [x] 玩家死亡信息（死亡信息为英文，计划使用翻译解决。非插件服务端不适用。）
-  - QQ -> 服务器
-    - [x] 指令（`nonebot-plugin-mcqq-mcrcon` 可用）
-    - [x] 群员聊天文本
-    - [x] 图片、视频等内容转换为 `[图片]`、`[视频]`
+    - 服务器 -> QQ
+        - [x] 加入 / 离开 服务器消息
+        - [x] 玩家聊天信息
+        - [x] 玩家死亡信息（死亡信息为英文，非插件服务端不适用。）
+    - QQ -> 服务器
+        - [x] 指令
+        - [x] 群员聊天文本
+        - [x] 图片、视频等内容转换为 `[图片]`、`[视频]`
 
 - 特殊消息支持
-  - 群聊
-    - [x] @ 消息
-    - [x] 回复消息（转换成@消息）
-  - 频道
-    - [x] @ 消息
-    - [x] 回复消息（转换成@消息）
-  - 未支持的消息已被替换，如： `[图片]`、 `[视频]` 等等
+    - 群聊
+        - [x] @ 消息
+        - [x] 回复消息（转换成@消息）
+    - 频道
+        - [x] @ 消息
+        - [x] 回复消息（转换成@消息）
+    - 未支持的消息已被替换，如： `[图片]`、 `[视频]` 等等
 
 # 特别感谢
+
 - [@SK-415](https://github.com/SK-415) ：感谢SK佬给予许多优秀的建议和耐心的解答。
 - [@zhz-红石头](https://github.com/zhzhongshi) ：感谢红石头在代码上的帮助
 - [NoneBot2](https://github.com/nonebot/nonebot2)： 插件使用的开发框架。
 - [go-cqhttp](https://github.com/Mrs4s/go-cqhttp)： 稳定完善的 CQHTTP 实现。
 
 # 二创
 
 - [mcqq服主版](https://github.com/KarisAya/nonebot_plugin_mcqq_server) 采用本地读取log信息的方法的Minecraft Server互通消息的插件
+
+## 贡献与支持
+
+觉得好用可以给这个项目点个 `Star` 或者去 [爱发电](https://afdian.net/a/17TheWord) 投喂我。
+
+有意见或者建议也欢迎提交 [Issues](https://github.com/17TheWord/nonebot-plugin-mcqq/issues)
+和 [Pull requests](https://github.com/17TheWord/nonebot-plugin-mcqq/pulls)。
+
+## 许可证
+
+本项目使用 [GNU AGPLv3](https://choosealicense.com/licenses/agpl-3.0/) 作为开源许可证。
```

### Comparing `nonebot-plugin-mcqq-1.1.5.post3/setup.py` & `nonebot-plugin-mcqq-1.1.5.post4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="nonebot-plugin-mcqq",  # 项目名称，保证它的唯一性，不要跟已存在的包名冲突即可
-    version="1.1.5-post3",  # 程序版本
+    version="1.1.5-post4",  # 程序版本
     author="17TheWord",  # 项目作者
     author_email="17theword@gmail.com",  # 作者邮件
     description="基于NoneBot的QQ群聊与Minecraft Server消息互通插件",  # 项目的一句话描述
     long_description=long_description,  # 加长版描述？
     long_description_content_type="text/markdown",  # 描述使用Markdown
     url="https://github.com/17TheWord/nonebot-plugin-mcqq",  # 项目地址
     packages=setuptools.find_packages(),  # 无需修改
@@ -20,9 +20,10 @@
     ],
     install_requires=[
         'mcqq-tool>=0.0.4',
         'nonebot2>=2.0.0rc3',
         'nonebot-adapter-onebot>=2.1.1',
         'nonebot-plugin-guild-patch>=0.2.0',
         'websockets>=10.3',
+        'aio-mc-rcon>=3.2.0'
     ],
 )
```

