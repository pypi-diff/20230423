# Comparing `tmp/nonebot-plugin-mcqq-1.1.5.post1.tar.gz` & `tmp/nonebot-plugin-mcqq-1.1.5.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-mcqq-1.1.5.post1.tar", last modified: Fri Apr 21 09:59:51 2023, max compression
+gzip compressed data, was "nonebot-plugin-mcqq-1.1.5.post2.tar", last modified: Sun Apr 23 06:43:00 2023, max compression
```

## Comparing `nonebot-plugin-mcqq-1.1.5.post1.tar` & `nonebot-plugin-mcqq-1.1.5.post2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 09:59:51.280689 nonebot-plugin-mcqq-1.1.5.post1/
--rw-rw-rw-   0        0        0    35184 2022-08-07 15:18:53.000000 nonebot-plugin-mcqq-1.1.5.post1/LICENSE
--rw-rw-rw-   0        0        0     2647 2023-04-21 09:59:51.280689 nonebot-plugin-mcqq-1.1.5.post1/PKG-INFO
--rw-rw-rw-   0        0        0     2146 2023-01-26 17:04:35.000000 nonebot-plugin-mcqq-1.1.5.post1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 09:59:51.269679 nonebot-plugin-mcqq-1.1.5.post1/nonebot_plugin_mcqq/
--rw-rw-rw-   0        0        0      911 2023-04-21 09:31:25.000000 nonebot-plugin-mcqq-1.1.5.post1/nonebot_plugin_mcqq/__init__.py
--rw-rw-rw-   0        0        0     2422 2023-04-21 09:32:08.000000 nonebot-plugin-mcqq-1.1.5.post1/nonebot_plugin_mcqq/data_source.py
--rw-rw-rw-   0        0        0     1023 2023-04-21 09:31:25.000000 nonebot-plugin-mcqq-1.1.5.post1/nonebot_plugin_mcqq/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-21 09:59:51.279688 nonebot-plugin-mcqq-1.1.5.post1/nonebot_plugin_mcqq.egg-info/
--rw-rw-rw-   0        0        0     2647 2023-04-21 09:59:51.000000 nonebot-plugin-mcqq-1.1.5.post1/nonebot_plugin_mcqq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      336 2023-04-21 09:59:51.000000 nonebot-plugin-mcqq-1.1.5.post1/nonebot_plugin_mcqq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 09:59:51.000000 nonebot-plugin-mcqq-1.1.5.post1/nonebot_plugin_mcqq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      117 2023-04-21 09:59:51.000000 nonebot-plugin-mcqq-1.1.5.post1/nonebot_plugin_mcqq.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-04-21 09:59:51.000000 nonebot-plugin-mcqq-1.1.5.post1/nonebot_plugin_mcqq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 09:59:51.280689 nonebot-plugin-mcqq-1.1.5.post1/setup.cfg
--rw-rw-rw-   0        0        0     1216 2023-04-21 09:58:44.000000 nonebot-plugin-mcqq-1.1.5.post1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:43:00.919315 nonebot-plugin-mcqq-1.1.5.post2/
+-rw-rw-rw-   0        0        0    35184 2022-08-07 15:18:53.000000 nonebot-plugin-mcqq-1.1.5.post2/LICENSE
+-rw-rw-rw-   0        0        0     2647 2023-04-23 06:43:00.919315 nonebot-plugin-mcqq-1.1.5.post2/PKG-INFO
+-rw-rw-rw-   0        0        0     2146 2023-01-26 17:04:35.000000 nonebot-plugin-mcqq-1.1.5.post2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 06:43:00.914923 nonebot-plugin-mcqq-1.1.5.post2/nonebot_plugin_mcqq/
+-rw-rw-rw-   0        0        0     1277 2023-04-23 06:30:14.000000 nonebot-plugin-mcqq-1.1.5.post2/nonebot_plugin_mcqq/__init__.py
+-rw-rw-rw-   0        0        0     2847 2023-04-23 06:12:28.000000 nonebot-plugin-mcqq-1.1.5.post2/nonebot_plugin_mcqq/data_source.py
+-rw-rw-rw-   0        0        0     1024 2023-04-22 05:52:16.000000 nonebot-plugin-mcqq-1.1.5.post2/nonebot_plugin_mcqq/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:43:00.917925 nonebot-plugin-mcqq-1.1.5.post2/nonebot_plugin_mcqq.egg-info/
+-rw-rw-rw-   0        0        0     2647 2023-04-23 06:43:00.000000 nonebot-plugin-mcqq-1.1.5.post2/nonebot_plugin_mcqq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      336 2023-04-23 06:43:00.000000 nonebot-plugin-mcqq-1.1.5.post2/nonebot_plugin_mcqq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 06:43:00.000000 nonebot-plugin-mcqq-1.1.5.post2/nonebot_plugin_mcqq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      117 2023-04-23 06:43:00.000000 nonebot-plugin-mcqq-1.1.5.post2/nonebot_plugin_mcqq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-04-23 06:43:00.000000 nonebot-plugin-mcqq-1.1.5.post2/nonebot_plugin_mcqq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 06:43:00.919315 nonebot-plugin-mcqq-1.1.5.post2/setup.cfg
+-rw-rw-rw-   0        0        0     1216 2023-04-23 06:42:00.000000 nonebot-plugin-mcqq-1.1.5.post2/setup.py
```

### Comparing `nonebot-plugin-mcqq-1.1.5.post1/LICENSE` & `nonebot-plugin-mcqq-1.1.5.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcqq-1.1.5.post1/PKG-INFO` & `nonebot-plugin-mcqq-1.1.5.post2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mcqq
-Version: 1.1.5.post1
+Version: 1.1.5.post2
 Summary: 基于NoneBot的QQ群聊与Minecraft Server消息互通插件
 Home-page: https://github.com/17TheWord/nonebot-plugin-mcqq
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `nonebot-plugin-mcqq-1.1.5.post1/README.md` & `nonebot-plugin-mcqq-1.1.5.post2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcqq-1.1.5.post1/nonebot_plugin_mcqq/__init__.py` & `nonebot-plugin-mcqq-1.1.5.post2/nonebot_plugin_mcqq/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,20 @@
-from nonebot import on_message, get_driver
+from typing import Union
+from nonebot import on_message, on_command, get_driver
+from nonebot.adapters import Message
+from nonebot.params import CommandArg
 from nonebot.adapters.onebot.v11 import Bot, GroupMessageEvent
 from nonebot_plugin_guild_patch import GuildMessageEvent
-from typing import Union
-from mcqq_tool.mcqq import send_msg_to_mc
+from mcqq_tool.utils import send_msg_to_mc, send_cmd_to_mc
 from .data_source import start_ws_server, stop_ws_server
 from .utils import msg_rule, plugin_config
 
-mc_qq = on_message(priority=5, rule=msg_rule, block=False)
+mc_qq = on_message(priority=1, rule=msg_rule)
+
+mc_qq_cmd = on_command("minecraft_command", aliases={"mcc"}, priority=1, rule=msg_rule, block=True)
 
 driver = get_driver()
 
 
 # bot连接时
 @driver.on_bot_connect
 async def on_start():
@@ -20,11 +24,17 @@
 
 @driver.on_bot_disconnect
 async def on_close():
     # 关闭 WebSocket 服务器
     await stop_ws_server()
 
 
-# 收到 群/频 道消息时
+# 收到消息时
 @mc_qq.handle()
-async def handle_first_receive(bot: Bot, event: Union[GroupMessageEvent, GuildMessageEvent]):
-    await send_msg_to_mc(bot=bot, event=event, server_list=plugin_config.mc_qq_servers_list)
+async def handle_msg(bot: Bot, event: Union[GroupMessageEvent, GuildMessageEvent]):
+    await send_msg_to_mc(bot=bot, event=event)
+
+
+# 收到命令时
+@mc_qq_cmd.handle()
+async def handle_cmd(bot: Bot, event: Union[GroupMessageEvent, GuildMessageEvent], args: Message = CommandArg()):
+    await send_cmd_to_mc(bot=bot, event=event, cmd=args.extract_plain_text())
```

### Comparing `nonebot-plugin-mcqq-1.1.5.post1/nonebot_plugin_mcqq/data_source.py` & `nonebot-plugin-mcqq-1.1.5.post2/nonebot_plugin_mcqq/data_source.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+import aiomcrcon
 import websockets
-from mcqq_tool.mcqq import Client, CLIENTS, send_msg_to_qq, remove_client
+from mcqq_tool.config import Client, CLIENTS
+from mcqq_tool.utils import send_msg_to_qq, remove_client, rcon_connect
 from nonebot import logger, get_bot
 
 from .utils import plugin_config
 
 
 async def ws_client(websocket: websockets.WebSocketServerProtocol):
     """WebSocket"""
@@ -11,31 +13,41 @@
         server_name = websocket.request_headers["x-self-name"].encode('utf-8').decode('unicode_escape')
     except KeyError as e:
         # 服务器名为空
         logger.error(f"[MC_QQ]丨未获取到该服务器的名称，连接断开：{e}")
         await websocket.close(1008, "[MC_QQ]丨未获取到该服务器的名称，连接断开")
         return
     else:
-        for client in CLIENTS:
-            # 重复连接
-            if server_name == client.server_name:
-                logger.error(f"[MC_QQ]丨[Server:{server_name}] 已连接至 WebSocket 服务器，无需重复连接")
-                await websocket.close(1008, f"[MC_QQ]丨[Server:{server_name}] 已连接至 WebSocket 服务器，无需重复连接")
-                return
-
-        CLIENTS.append(Client(server_name=server_name, websocket=websocket))
+        try:
+            CLIENTS.get(server_name)
+        except KeyError as e:
+            # 服务器名不在配置文件中
+            logger.error(f"[MC_QQ]丨[Server:{server_name}] 未在配置文件中配置，连接断开：{e}")
+            await websocket.close(1008, f"[MC_QQ]丨[Server:{server_name}] 未在配置文件中配置，连接断开")
+            return
+        rcon_client = None
+        for server in plugin_config.mc_qq_server_list:
+            if server_name == server.server_name and server.rcon_enable:
+                rcon_client = aiomcrcon.Client(
+                    websocket.remote_address[0],
+                    plugin_config.mc_qq_rcon_dict[server_name],
+                    plugin_config.mc_qq_rcon_password
+                )
+                await rcon_connect(rcon_client=rcon_client, server_name=server_name)
+                break
+        CLIENTS[server_name] = Client(
+            server_name=server_name,
+            websocket=websocket,
+            rcon=rcon_client
+        )
         logger.success(f"[MC_QQ]丨[Server:{server_name}] 已连接至 WebSocket 服务器")
+
         try:
             async for message in websocket:
-                await send_msg_to_qq(
-                    bot=get_bot(),
-                    message=message,
-                    server_list=plugin_config.mc_qq_servers_list,
-                    display_server_name=plugin_config.mc_qq_display_server_name
-                )
+                await send_msg_to_qq(bot=get_bot(), message=message)
         except websockets.WebSocketException as e:
             # 移除当前客户端
             await remove_client(server_name=server_name)
             logger.error(f"[MC_QQ]丨[Server:{server_name}] 的 WebSocket 连接已断开：{e}")
         else:
             if websocket.closed:
                 await remove_client(server_name=server_name)
```

### Comparing `nonebot-plugin-mcqq-1.1.5.post1/nonebot_plugin_mcqq/utils.py` & `nonebot-plugin-mcqq-1.1.5.post2/nonebot_plugin_mcqq/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from nonebot import get_driver
 from nonebot.adapters.onebot.v11 import GroupMessageEvent
 from nonebot_plugin_guild_patch import GuildMessageEvent
 from typing import Union
 
-from mcqq_tool.mcqq import Config
+from mcqq_tool.config import Config
 
 plugin_config: Config = Config.parse_obj(get_driver().config)
 
 rule_guild_list = []
 rule_group_list = []
-for per_server in plugin_config.mc_qq_servers_list:
+for per_server in plugin_config.mc_qq_server_list:
     if guild_list := per_server.guild_list:
         for per_guild in guild_list:
             rule_guild_list.append(f"{per_guild.guild_id}:{per_guild.channel_id}")
     if group_list := per_server.group_list:
         for per_group in group_list:
             rule_group_list.append(per_group)
```

### Comparing `nonebot-plugin-mcqq-1.1.5.post1/nonebot_plugin_mcqq.egg-info/PKG-INFO` & `nonebot-plugin-mcqq-1.1.5.post2/nonebot_plugin_mcqq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mcqq
-Version: 1.1.5.post1
+Version: 1.1.5.post2
 Summary: 基于NoneBot的QQ群聊与Minecraft Server消息互通插件
 Home-page: https://github.com/17TheWord/nonebot-plugin-mcqq
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `nonebot-plugin-mcqq-1.1.5.post1/setup.py` & `nonebot-plugin-mcqq-1.1.5.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="nonebot-plugin-mcqq",  # 项目名称，保证它的唯一性，不要跟已存在的包名冲突即可
-    version="1.1.5-post1",  # 程序版本
+    version="1.1.5-post2",  # 程序版本
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
         "Operating System :: OS Independent",
     ],
     install_requires=[
-        'mcqq-tool>=0.0.1',
+        'mcqq-tool>=0.0.3',
         'nonebot2>=2.0.0rc3',
         'nonebot-adapter-onebot>=2.1.1',
         'nonebot-plugin-guild-patch>=0.2.0',
         'websockets>=10.3',
     ],
 )
```

