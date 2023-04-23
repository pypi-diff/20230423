# Comparing `tmp/mcqq-tool-0.0.4.tar.gz` & `tmp/mcqq-tool-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcqq-tool-0.0.4.tar", last modified: Sun Apr 23 07:27:50 2023, max compression
+gzip compressed data, was "mcqq-tool-0.0.5.tar", last modified: Sun Apr 23 10:02:13 2023, max compression
```

## Comparing `mcqq-tool-0.0.4.tar` & `mcqq-tool-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 07:27:50.139073 mcqq-tool-0.0.4/
--rw-rw-rw-   0        0        0    35184 2023-04-21 09:49:28.000000 mcqq-tool-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      511 2023-04-23 07:27:50.139073 mcqq-tool-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       82 2023-04-21 08:06:01.000000 mcqq-tool-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 07:27:50.131065 mcqq-tool-0.0.4/mcqq_tool/
--rw-rw-rw-   0        0        0       33 2023-04-22 04:16:51.000000 mcqq-tool-0.0.4/mcqq_tool/__init__.py
--rw-rw-rw-   0        0        0     4283 2023-04-23 06:09:58.000000 mcqq-tool-0.0.4/mcqq_tool/common.py
--rw-rw-rw-   0        0        0     1879 2023-04-23 07:27:30.000000 mcqq-tool-0.0.4/mcqq_tool/config.py
-drwxrwxrwx   0        0        0        0 2023-04-23 07:27:50.137071 mcqq-tool-0.0.4/mcqq_tool/model/
--rw-rw-rw-   0        0        0      597 2023-04-21 08:09:17.000000 mcqq-tool-0.0.4/mcqq_tool/model/__init__.py
--rw-rw-rw-   0        0        0     1041 2023-04-21 08:09:17.000000 mcqq-tool-0.0.4/mcqq_tool/model/basemodel.py
--rw-rw-rw-   0        0        0      640 2023-04-21 08:09:17.000000 mcqq-tool-0.0.4/mcqq_tool/model/minecraft.py
--rw-rw-rw-   0        0        0     1389 2023-04-21 08:09:17.000000 mcqq-tool-0.0.4/mcqq_tool/model/spigot.py
--rw-rw-rw-   0        0        0    13352 2023-04-23 06:28:43.000000 mcqq-tool-0.0.4/mcqq_tool/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-23 07:27:50.134068 mcqq-tool-0.0.4/mcqq_tool.egg-info/
--rw-rw-rw-   0        0        0      511 2023-04-23 07:27:50.000000 mcqq-tool-0.0.4/mcqq_tool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2023-04-23 07:27:50.000000 mcqq-tool-0.0.4/mcqq_tool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 07:27:50.000000 mcqq-tool-0.0.4/mcqq_tool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-04-23 07:27:50.000000 mcqq-tool-0.0.4/mcqq_tool.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-23 07:27:50.000000 mcqq-tool-0.0.4/mcqq_tool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 07:27:50.139073 mcqq-tool-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1023 2023-04-23 07:27:38.000000 mcqq-tool-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 10:02:13.218857 mcqq-tool-0.0.5/
+-rw-rw-rw-   0        0        0    35184 2023-04-21 09:49:28.000000 mcqq-tool-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      589 2023-04-23 10:02:13.217856 mcqq-tool-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      160 2023-04-23 07:53:23.000000 mcqq-tool-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 10:02:13.209955 mcqq-tool-0.0.5/mcqq_tool/
+-rw-rw-rw-   0        0        0        0 2023-04-23 08:51:16.000000 mcqq-tool-0.0.5/mcqq_tool/__init__.py
+-rw-rw-rw-   0        0        0     4254 2023-04-23 08:42:34.000000 mcqq-tool-0.0.5/mcqq_tool/common.py
+-rw-rw-rw-   0        0        0     1879 2023-04-23 07:27:30.000000 mcqq-tool-0.0.5/mcqq_tool/config.py
+drwxrwxrwx   0        0        0        0 2023-04-23 10:02:13.217856 mcqq-tool-0.0.5/mcqq_tool/model/
+-rw-rw-rw-   0        0        0      692 2023-04-23 08:49:34.000000 mcqq-tool-0.0.5/mcqq_tool/model/__init__.py
+-rw-rw-rw-   0        0        0      929 2023-04-23 08:42:34.000000 mcqq-tool-0.0.5/mcqq_tool/model/basemodel.py
+-rw-rw-rw-   0        0        0      640 2023-04-23 08:49:34.000000 mcqq-tool-0.0.5/mcqq_tool/model/minecraft.py
+-rw-rw-rw-   0        0        0        0 2023-04-23 08:49:34.000000 mcqq-tool-0.0.5/mcqq_tool/model/model_type.py
+-rw-rw-rw-   0        0        0     1389 2023-04-21 08:09:17.000000 mcqq-tool-0.0.5/mcqq_tool/model/spigot.py
+-rw-rw-rw-   0        0        0    13352 2023-04-23 06:28:43.000000 mcqq-tool-0.0.5/mcqq_tool/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-23 10:02:13.212955 mcqq-tool-0.0.5/mcqq_tool.egg-info/
+-rw-rw-rw-   0        0        0      589 2023-04-23 10:02:13.000000 mcqq-tool-0.0.5/mcqq_tool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2023-04-23 10:02:13.000000 mcqq-tool-0.0.5/mcqq_tool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 10:02:13.000000 mcqq-tool-0.0.5/mcqq_tool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-04-23 10:02:13.000000 mcqq-tool-0.0.5/mcqq_tool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-23 10:02:13.000000 mcqq-tool-0.0.5/mcqq_tool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 10:02:13.218857 mcqq-tool-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1023 2023-04-23 10:01:17.000000 mcqq-tool-0.0.5/setup.py
```

### Comparing `mcqq-tool-0.0.4/LICENSE` & `mcqq-tool-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mcqq-tool-0.0.4/mcqq_tool/common.py` & `mcqq-tool-0.0.5/mcqq_tool/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 
 from nonebot import logger, get_driver
 from nonebot.adapters.onebot.v11 import Bot, GroupMessageEvent
 from nonebot.internal.permission import Permission
 from nonebot_plugin_guild_patch import GuildMessageEvent
 
 from .config import Config
-from .model import event_dict
-from .model.basemodel import BaseEvent, BaseChatEvent, BaseDeathEvent, BaseJoinEvent, BaseQuitEvent
+from .model import event_dict, BaseEvent, BaseChatEvent, BaseDeathEvent, BaseJoinEvent, BaseQuitEvent
 
 plugin_config: Config = Config.parse_obj(get_driver().config)
 
 
 async def _guild_admin(
         bot: Bot,
         event: GuildMessageEvent,
```

### Comparing `mcqq-tool-0.0.4/mcqq_tool/config.py` & `mcqq-tool-0.0.5/mcqq_tool/config.py`

 * *Files identical despite different names*

### Comparing `mcqq-tool-0.0.4/mcqq_tool/model/basemodel.py` & `mcqq-tool-0.0.5/mcqq_tool/model/basemodel.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,38 +15,33 @@
 
 class BaseMessageEvent(BaseEvent):
     """消息事件基类"""
     post_type = "message"
     player: BasePlayer
 
 
-class BaseChatEvent(BaseEvent):
+class BaseChatEvent(BaseMessageEvent):
     """玩家聊天事件基类"""
-    post_type = "message"
     sub_type = "chat"
     message: str
-    player: BasePlayer
 
 
-class BaseDeathEvent(BaseEvent):
+class BaseDeathEvent(BaseMessageEvent):
     """玩家死亡事件基类"""
-    post_type = "message"
     sub_type = "death"
-    player: BasePlayer
     death_message: str
 
 
 class BaseNoticeEvent(BaseEvent):
     """通知事件基类"""
     post_type = "notice"
+    player: BasePlayer
 
 
 class BaseJoinEvent(BaseNoticeEvent):
     """玩家加入事件基类"""
     sub_type = "join"
-    player: BasePlayer
 
 
 class BaseQuitEvent(BaseNoticeEvent):
     """玩家退出事件基类"""
     sub_type = "quit"
-    player: BasePlayer
```

### Comparing `mcqq-tool-0.0.4/mcqq_tool/model/minecraft.py` & `mcqq-tool-0.0.5/mcqq_tool/model/minecraft.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from .basemodel import BasePlayer, BaseChatEvent, BaseJoinEvent, BaseQuitEvent
 
 
 class MineCraftPlayer(BasePlayer):
     """原版 玩家信息"""
 
 
-class MineCraftPlayerChatEvent(BaseChatEvent):
+class MinecraftPlayerChatEvent(BaseChatEvent):
     """原版 玩家聊天事件"""
-    event_name = "MineCraftPlayerChatEvent"
+    event_name = "MinecraftPlayerChatEvent"
     player: MineCraftPlayer
 
 
 class MinecraftPlayerJoinEvent(BaseJoinEvent):
     """原版 玩家加入事件"""
     event_name = "MinecraftPlayerJoinEvent"
     player: MineCraftPlayer
```

### Comparing `mcqq-tool-0.0.4/mcqq_tool/model/spigot.py` & `mcqq-tool-0.0.5/mcqq_tool/model/spigot.py`

 * *Files identical despite different names*

### Comparing `mcqq-tool-0.0.4/mcqq_tool/utils.py` & `mcqq-tool-0.0.5/mcqq_tool/utils.py`

 * *Files identical despite different names*

### Comparing `mcqq-tool-0.0.4/setup.py` & `mcqq-tool-0.0.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="mcqq-tool",  # 项目名称，保证它的唯一性，不要跟已存在的包名冲突即可
-    version="0.0.4",  # 程序版本
+    version="0.0.5",  # 程序版本
     author="17TheWord",  # 项目作者
     author_email="17theword@gmail.com",  # 作者邮件
     description="MC_QQ 工具包",  # 项目的一句话描述
     long_description=long_description,  # 加长版描述？
     long_description_content_type="text/markdown",  # 描述使用Markdown
     url="https://github.com/17TheWord/mcqq-tool",  # 项目地址
     packages=setuptools.find_packages(),  # 无需修改
```

