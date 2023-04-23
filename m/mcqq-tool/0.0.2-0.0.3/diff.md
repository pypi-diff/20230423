# Comparing `tmp/mcqq-tool-0.0.2.tar.gz` & `tmp/mcqq-tool-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcqq-tool-0.0.2.tar", last modified: Sat Apr 22 05:41:19 2023, max compression
+gzip compressed data, was "mcqq-tool-0.0.3.tar", last modified: Sun Apr 23 06:40:51 2023, max compression
```

## Comparing `mcqq-tool-0.0.2.tar` & `mcqq-tool-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 05:41:19.554635 mcqq-tool-0.0.2/
--rw-rw-rw-   0        0        0    35184 2023-04-21 09:49:28.000000 mcqq-tool-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      511 2023-04-22 05:41:19.554635 mcqq-tool-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       82 2023-04-21 08:06:01.000000 mcqq-tool-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-22 05:41:19.545627 mcqq-tool-0.0.2/mcqq_tool/
--rw-rw-rw-   0        0        0       33 2023-04-22 04:16:51.000000 mcqq-tool-0.0.2/mcqq_tool/__init__.py
--rw-rw-rw-   0        0        0     4414 2023-04-22 04:20:30.000000 mcqq-tool-0.0.2/mcqq_tool/common.py
--rw-rw-rw-   0        0        0     1902 2023-04-22 05:19:28.000000 mcqq-tool-0.0.2/mcqq_tool/config.py
-drwxrwxrwx   0        0        0        0 2023-04-22 05:41:19.553635 mcqq-tool-0.0.2/mcqq_tool/model/
--rw-rw-rw-   0        0        0      597 2023-04-21 08:09:17.000000 mcqq-tool-0.0.2/mcqq_tool/model/__init__.py
--rw-rw-rw-   0        0        0     1041 2023-04-21 08:09:17.000000 mcqq-tool-0.0.2/mcqq_tool/model/basemodel.py
--rw-rw-rw-   0        0        0      640 2023-04-21 08:09:17.000000 mcqq-tool-0.0.2/mcqq_tool/model/minecraft.py
--rw-rw-rw-   0        0        0     1389 2023-04-21 08:09:17.000000 mcqq-tool-0.0.2/mcqq_tool/model/spigot.py
--rw-rw-rw-   0        0        0    11652 2023-04-22 05:19:28.000000 mcqq-tool-0.0.2/mcqq_tool/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-22 05:41:19.550631 mcqq-tool-0.0.2/mcqq_tool.egg-info/
--rw-rw-rw-   0        0        0      511 2023-04-22 05:41:19.000000 mcqq-tool-0.0.2/mcqq_tool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2023-04-22 05:41:19.000000 mcqq-tool-0.0.2/mcqq_tool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 05:41:19.000000 mcqq-tool-0.0.2/mcqq_tool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-04-22 05:41:19.000000 mcqq-tool-0.0.2/mcqq_tool.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-22 05:41:19.000000 mcqq-tool-0.0.2/mcqq_tool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-22 05:41:19.555636 mcqq-tool-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1024 2023-04-22 05:28:24.000000 mcqq-tool-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:40:51.572990 mcqq-tool-0.0.3/
+-rw-rw-rw-   0        0        0    35184 2023-04-21 09:49:28.000000 mcqq-tool-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      511 2023-04-23 06:40:51.572481 mcqq-tool-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       82 2023-04-21 08:06:01.000000 mcqq-tool-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 06:40:51.565647 mcqq-tool-0.0.3/mcqq_tool/
+-rw-rw-rw-   0        0        0       33 2023-04-22 04:16:51.000000 mcqq-tool-0.0.3/mcqq_tool/__init__.py
+-rw-rw-rw-   0        0        0     4283 2023-04-23 06:09:58.000000 mcqq-tool-0.0.3/mcqq_tool/common.py
+-rw-rw-rw-   0        0        0     1873 2023-04-23 06:00:48.000000 mcqq-tool-0.0.3/mcqq_tool/config.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:40:51.571400 mcqq-tool-0.0.3/mcqq_tool/model/
+-rw-rw-rw-   0        0        0      597 2023-04-21 08:09:17.000000 mcqq-tool-0.0.3/mcqq_tool/model/__init__.py
+-rw-rw-rw-   0        0        0     1041 2023-04-21 08:09:17.000000 mcqq-tool-0.0.3/mcqq_tool/model/basemodel.py
+-rw-rw-rw-   0        0        0      640 2023-04-21 08:09:17.000000 mcqq-tool-0.0.3/mcqq_tool/model/minecraft.py
+-rw-rw-rw-   0        0        0     1389 2023-04-21 08:09:17.000000 mcqq-tool-0.0.3/mcqq_tool/model/spigot.py
+-rw-rw-rw-   0        0        0    13352 2023-04-23 06:28:43.000000 mcqq-tool-0.0.3/mcqq_tool/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-23 06:40:51.569398 mcqq-tool-0.0.3/mcqq_tool.egg-info/
+-rw-rw-rw-   0        0        0      511 2023-04-23 06:40:51.000000 mcqq-tool-0.0.3/mcqq_tool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2023-04-23 06:40:51.000000 mcqq-tool-0.0.3/mcqq_tool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 06:40:51.000000 mcqq-tool-0.0.3/mcqq_tool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-04-23 06:40:51.000000 mcqq-tool-0.0.3/mcqq_tool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-23 06:40:51.000000 mcqq-tool-0.0.3/mcqq_tool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 06:40:51.572990 mcqq-tool-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1023 2023-04-23 06:37:23.000000 mcqq-tool-0.0.3/setup.py
```

### Comparing `mcqq-tool-0.0.2/LICENSE` & `mcqq-tool-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mcqq-tool-0.0.2/mcqq_tool/common.py` & `mcqq-tool-0.0.3/mcqq_tool/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import json
-from typing import Union, Optional
+from typing import Union
 
 from nonebot import logger, get_driver
 from nonebot.adapters.onebot.v11 import Bot, GroupMessageEvent
 from nonebot.internal.permission import Permission
 from nonebot_plugin_guild_patch import GuildMessageEvent
 
-from .config import RoleConfig
+from .config import Config
 from .model import event_dict
 from .model.basemodel import BaseEvent, BaseChatEvent, BaseDeathEvent, BaseJoinEvent, BaseQuitEvent
 
-role_config: RoleConfig = RoleConfig.parse_obj(get_driver().config)
+plugin_config: Config = Config.parse_obj(get_driver().config)
 
 
 async def _guild_admin(
         bot: Bot,
         event: GuildMessageEvent,
 ):
     """检测是否为频道管理员"""
@@ -22,15 +22,15 @@
         role["role_name"]
         for role in (
             await bot.get_guild_member_profile(
                 guild_id=event.guild_id, user_id=event.user_id
             )
         )["roles"]
     )
-    return bool(roles & set(role_config.mc_qq_guild_admin_roles))
+    return bool(roles & set(plugin_config.mc_qq_guild_admin_roles))
 
 
 GUILD_ADMIN: Permission = Permission(_guild_admin)
 """频道管理员权限"""
 
 
 async def msg_to_qq_process(event: BaseEvent) -> str:
@@ -46,44 +46,41 @@
     else:
         return "未知消息"
 
 
 async def send_msg_to_qq_common(
         bot: Bot,
         message: str,
-        server_list: list,
-        display_server_name: Optional[bool] = False,
-        plugin_name: Optional[str] = "MC_QQ"
 ):
     """发送消息到 QQ"""
     json_msg = json.loads(message)
     event = event_dict[json_msg["event_name"]].parse_obj(json_msg)
 
     msg = await msg_to_qq_process(event)
-    if display_server_name:
+    if plugin_config.mc_qq_display_server_name:
         msg = f"[{event.server_name}] {msg}"
     # 循环服务器列表并发送消息
-    if mc_qq_servers_list := server_list:
-        for per_server in mc_qq_servers_list:
+    if plugin_config.mc_qq_server_list:
+        for per_server in plugin_config.mc_qq_server_list:
             # 判断服务器名称是否相同
             if per_server.server_name == event.server_name:
                 # 判断是否发送到群聊
                 if group_list := per_server.group_list:
                     for per_group in group_list:
                         logger.success(
-                            f"[{plugin_name}]丨from [{event.server_name}] to [群:{per_group}] \"{msg}\"")
+                            f"[MC_QQ]丨from [{event.server_name}] to [群:{per_group}] \"{msg}\"")
                         await bot.send_group_msg(
                             group_id=per_group,
                             message=msg
                         )
                 # 判断是否发送到频道
                 if guild_list := per_server.guild_list:
                     for per_guild in guild_list:
                         logger.success(
-                            f"[{plugin_name}]丨from [{event.server_name}] to [频道:{per_guild.guild_id}/{per_guild.channel_id}] \"{msg}\"")
+                            f"[MC_QQ]丨from [{event.server_name}] to [频道:{per_guild.guild_id}/{per_guild.channel_id}] \"{msg}\"")
                         await bot.send_guild_channel_msg(
                             guild_id=per_guild.guild_id,
                             channel_id=per_guild.channel_id,
                             message=msg
                         )
```

### Comparing `mcqq-tool-0.0.2/mcqq_tool/config.py` & `mcqq-tool-0.0.3/mcqq_tool/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
             rcon: Optional[aiomcrcon.Client] = None
     ):
         self.server_name: str = server_name
         self.websocket: websockets.WebSocketServerProtocol = websocket
         self.rcon: Optional[aiomcrcon.Client] = rcon
 
 
-CLIENTS: List[Client] = []
+CLIENTS: Dict[str, Client] = {}
 
 
 class Guild(BaseModel):
     """频道配置"""
     # 频道ID
     guild_id: int
     # 子频道ID
@@ -39,19 +39,14 @@
     group_list: Optional[List[int]] = []
     # 服务器频道列表
     guild_list: Optional[List[Guild]] = []
     # 是否开启 Rcon
     rcon_enable: Optional[bool] = False
 
 
-class RoleConfig(BaseModel):
-    # MC_QQ 频道管理员身份组
-    mc_qq_guild_admin_roles: Optional[List[str]] = ["频道主", "管理员"]
-
-
 class Config(BaseModel, extra=Extra.ignore):
     """配置"""
     # 服务器地址
     mc_qq_ws_ip: Optional[str] = "127.0.0.1"
     # 服务器端口
     mc_qq_ws_port: Optional[int] = 8765
     # 是否发送群聊名称
@@ -60,7 +55,9 @@
     mc_qq_display_server_name: Optional[bool] = False
     # 服务器列表
     mc_qq_server_list: Optional[List[Server]] = Field(default_factory=list)
     # MCRcon 密码
     mc_qq_rcon_password: Optional[str] = "password"
     # Rcon 字典
     mc_qq_rcon_dict: Optional[Dict[str, int]] = Field(default_factory=dict)
+    # MC_QQ 频道管理员身份组
+    mc_qq_guild_admin_roles: Optional[List[str]] = ["频道主", "管理员"]
```

### Comparing `mcqq-tool-0.0.2/mcqq_tool/model/__init__.py` & `mcqq-tool-0.0.3/mcqq_tool/model/__init__.py`

 * *Files identical despite different names*

### Comparing `mcqq-tool-0.0.2/mcqq_tool/model/basemodel.py` & `mcqq-tool-0.0.3/mcqq_tool/model/basemodel.py`

 * *Files identical despite different names*

### Comparing `mcqq-tool-0.0.2/mcqq_tool/model/minecraft.py` & `mcqq-tool-0.0.3/mcqq_tool/model/minecraft.py`

 * *Files identical despite different names*

### Comparing `mcqq-tool-0.0.2/mcqq_tool/model/spigot.py` & `mcqq-tool-0.0.3/mcqq_tool/model/spigot.py`

 * *Files identical despite different names*

### Comparing `mcqq-tool-0.0.2/mcqq_tool/utils.py` & `mcqq-tool-0.0.3/mcqq_tool/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,136 +1,175 @@
 import json
-from typing import List, Union, Optional
+from typing import List, Union, Optional, Tuple
 
+import aiomcrcon
 import websockets
 from nonebot import logger
-from aiomcrcon.errors import ClientNotConnectedError
 from nonebot.adapters.onebot.v11 import Bot, GroupMessageEvent
 from nonebot_plugin_guild_patch import GuildMessageEvent
-from .config import Client, CLIENTS, Server
-from .common import get_member_nickname, send_msg_to_qq_common
 
+from .common import get_member_nickname, send_msg_to_qq_common, plugin_config
+from .config import Client, CLIENTS
 
-async def send_msg_to_mc(
-        bot: Bot, event: Union[GroupMessageEvent, GuildMessageEvent],
-        server_list: List[Server],
-        send_group_name: Optional[bool] = False
-):
+
+async def send_msg_to_mc(bot: Bot, event: Union[GroupMessageEvent, GuildMessageEvent]):
     """
     发送消息到 MC
     :param bot: Bot
     :param event: 事件
-    :param server_list: 服务器列表
-    :param send_group_name: 是否发送群聊名称
     """
     # 处理来自QQ的消息
-    text_msg, msgJson = await msg_process_to_json(bot=bot, event=event, send_group_name=send_group_name)
-    rcon_text_msg, msgCmd = await msg_process_to_cmd(bot=bot, event=event, send_group_name=send_group_name)
-    if client_list := await get_clients(event=event, server_list=server_list):
+    if client_list := await get_clients(event=event):
         for client in client_list:
             if client:
-                if client.websocket:
+                # 先判断是否有Rcon进行发送
+                if client.rcon:
+                    rcon_text_msg, msgCmd = await msg_process_to_cmd(bot=bot, event=event)
+                    try:
+                        await client.rcon.send_cmd(msgCmd)
+                    except aiomcrcon.errors.ClientNotConnectedError as e:
+                        logger.error(f"[MC_QQ_Rcon]丨发送至 [Server:{client.server_name}] 的过程中出现了错误：{e}")
+                        await remove_client(client.server_name)
+                    else:
+                        logger.success(f"[MC_QQ_Rcon]丨发送至 [server:{client.server_name}] 的消息 \"{rcon_text_msg}\"")
+                elif client.websocket:
+                    text_msg, msgJson = await msg_process_to_json(bot=bot, event=event)
                     try:
                         await client.websocket.send(msgJson)
                     except websockets.WebSocketException as e:
                         logger.error(f"[MC_QQ]丨发送至 [Server:{client.server_name}] 的过程中出现了错误：{e}")
-                        CLIENTS.remove(client)
+                        await remove_client(client.server_name)
                     else:
                         logger.success(f"[MC_QQ]丨发送至 [server:{client.server_name}] 的消息 \"{text_msg}\"")
-                elif client.rcon:
+                else:
+                    logger.error(f"[MC_QQ]丨发送至 [Server:{client.server_name}] 的过程中出现了错误：该客户端没有连接")
+                    await remove_client(client.server_name)
+
+
+async def send_cmd_to_mc(bot: Bot, event: Union[GroupMessageEvent, GuildMessageEvent], cmd: str):
+    """
+    发送命令到 MC
+    :param bot: Bot
+    :param event: 事件
+    :param cmd: 命令
+    """
+    # 处理来自QQ的消息
+    if client_list := await get_clients(event=event):
+        for client in client_list:
+            if client:
+                # 先判断是否有Rcon进行发送
+                if client.rcon:
                     try:
-                        await client.rcon.send_cmd(msgCmd)
-                    except ClientNotConnectedError as e:
+                        back_msg = await client.rcon.send_cmd(cmd)
+                        await bot.send(event=event, message=f"服务器返回：{back_msg[0]}")
+                    except aiomcrcon.errors.ClientNotConnectedError as e:
                         logger.error(f"[MC_QQ_Rcon]丨发送至 [Server:{client.server_name}] 的过程中出现了错误：{e}")
-                        CLIENTS.remove(client)
+                        await remove_client(client.server_name)
                     else:
-                        logger.success(f"[MC_QQ_Rcon]丨发送至 [server:{client.server_name}] 的消息 \"{rcon_text_msg}\"")
+                        logger.success(f"[MC_QQ_Rcon]丨发送至 [server:{client.server_name}] 的消息 \"{cmd}\"")
+                elif client.websocket:
+                    await bot.send(event=event, message="该服务器不支持Rcon，无法执行该命令")
+                else:
+                    logger.error(f"[MC_QQ]丨发送至 [Server:{client.server_name}] 的过程中出现了错误：该客户端没有连接")
+                    await remove_client(client.server_name)
 
 
-async def get_clients(
-        event: Union[GroupMessageEvent, GuildMessageEvent],
-        server_list: List[Server]
-) -> List[Client]:
+async def get_clients(event: Union[GroupMessageEvent, GuildMessageEvent]) -> List[Client]:
     """
     获取 服务器名、ws客户端, 返回client列表
     :param event: 事件
-    :param server_list: 服务器列表
     :return: client列表
     """
     res: List[Client] = []
-    for per_client in CLIENTS:
-        for per_server in server_list:
-            # 如果 服务器名 == ws客户端中记录的服务器名，且ws客户端存在
-            if per_server.server_name == per_client.server_name and per_client.websocket and (per_client not in res):
-                if isinstance(event, GroupMessageEvent):
-                    if event.group_id in per_server.group_list:
-                        res.append(per_client)
-                if isinstance(event, GuildMessageEvent):
-                    for per_guild in per_server.guild_list:
-                        if per_guild.guild_id == event.guild_id and per_guild.channel_id == event.channel_id:
-                            res.append(per_client)
+    for per_server in plugin_config.mc_qq_server_list:
+        if isinstance(event, GroupMessageEvent):
+            if event.group_id in per_server.group_list:
+                res.append(get_client(per_server.server_name))
+        if isinstance(event, GuildMessageEvent):
+            for per_guild in per_server.guild_list:
+                if per_guild.guild_id == event.guild_id and per_guild.channel_id == event.channel_id:
+                    res.append(get_client(per_server.server_name))
     return res
 
 
+def get_client(server_name: str) -> Optional[Client]:
+    """
+    获取客户端
+    :param server_name: 服务器名
+    :return: 客户端
+    """
+    try:
+        return CLIENTS[server_name]
+    except KeyError as e:
+        logger.error(f"[MC_QQ_Rcon]丨获取客户端时出现了错误，该客户端不在列表中：{e}")
+        return None
+
+
 async def remove_client(server_name: str):
     """
     移除客户端
     :param server_name: 服务器名
     """
-    for client in CLIENTS:
-        if client.server_name == server_name:
-            if client.rcon:
-                await client.websocket.close()
-            CLIENTS.remove(client)
+    if client := get_client(server_name):
+        if client.websocket:
+            await client.websocket.close()
+        if client.rcon:
+            await client.rcon.close()
+        del CLIENTS[server_name]
+
+
+async def rcon_connect(rcon_client: aiomcrcon.Client, server_name: str):
+    """
+    连接 Rcon
+    :param rcon_client: Rcon 客户端
+    :param server_name: 服务器名
+    """
+    try:
+        await rcon_client.connect()
+    except aiomcrcon.RCONConnectionError as e:
+        logger.error(f"[MC_QQ]丨[Server:{server_name}] 的Rcon连接失败：{str(e)}")
+    except aiomcrcon.IncorrectPasswordError as e:
+        logger.error(f"[MC_QQ]丨[Server:{server_name}] 的Rcon密码错误：{str(e)}")
+    else:
+        logger.success(f"[MC_QQ]丨[Server:{server_name}] 的Rcon连接成功")
 
 
 async def send_msg_to_qq(
         bot: Bot,
-        message: str,
-        server_list: List[Server],
-        display_server_name: Optional[bool] = False,
+        message: str
 ):
     """
     发送消息到 QQ
     :param bot: Bot
     :param message: 消息
-    :param server_list: 服务器列表
-    :param display_server_name: 是否显示服务器名
     """
     await send_msg_to_qq_common(
         bot=bot,
-        message=message,
-        server_list=server_list,
-        display_server_name=display_server_name,
-        plugin_name="MC_QQ"
+        message=message
     )
 
 
-async def msg_process_to_json(
-        bot: Bot, event: Union[GroupMessageEvent, GuildMessageEvent],
-        send_group_name: Optional[bool] = False
-):
+async def msg_process_to_json(bot: Bot, event: Union[GroupMessageEvent, GuildMessageEvent]) -> Tuple[str, str]:
     """
     消息处理为 JSON
     :param bot: Bot
     :param event: 事件
-    :param send_group_name: 是否发送群聊名称
     :return: text_msg, msgJson
     """
     # 获取昵称
     member_nickname = await get_member_nickname(bot, event, event.user_id)
 
     # 初始化消息
     text_msg = member_nickname + "说："
 
     # 初始化消息字典
     messageList = []
 
     # 发送群聊名称
-    if send_group_name:
+    if plugin_config.mc_qq_send_group_name:
         group_name = {'msgType': "group_name"}
         if isinstance(event, GroupMessageEvent):
             group_name['msgData'] = (await bot.get_group_info(group_id=event.group_id))['group_name']
         elif isinstance(event, GuildMessageEvent):
             guild_name = (await bot.get_guild_meta_by_guest(guild_id=event.guild_id))['guild_name']
             for per_channel in (await bot.get_guild_channel_list(guild_id=event.guild_id, no_cache=True)):
                 if str(event.channel_id) == per_channel['channel_id']:
@@ -190,38 +229,33 @@
         per_msg['msgData'] = msgData
         # 放入消息列表
         messageList.append(per_msg)
 
     return text_msg, str({"message": messageList})
 
 
-async def msg_process_to_cmd(
-        bot: Bot,
-        event: Union[GroupMessageEvent, GuildMessageEvent],
-        send_group_name: Optional[bool] = False
-):
+async def msg_process_to_cmd(bot: Bot, event: Union[GroupMessageEvent, GuildMessageEvent]) -> Tuple[str, str]:
     """
     消息处理为 命令
     :param bot: Bot
     :param event: 事件
-    :param send_group_name: 是否发送群聊名称
     :return: text_msg, command_msg
     """
     # 获取昵称
     member_nickname = await get_member_nickname(bot, event, event.user_id)
 
     # 初始化日志消息
     text_msg = member_nickname + " 说："
 
     command_msg = "tellraw @p "
 
     message_list = [
         {"text": "[MC_QQ] ", "color": "yellow"},
     ]
-    if send_group_name:
+    if plugin_config.mc_qq_send_group_name:
         if isinstance(event, GroupMessageEvent):
             message_list.append(
                 {"text": (await bot.get_group_info(group_id=event.group_id))['group_name'] + " ", "color": "aqua"})
         elif isinstance(event, GuildMessageEvent):
             guild_name = (await bot.get_guild_meta_by_guest(guild_id=event.guild_id))['guild_name']
             for per_channel in (await bot.get_guild_channel_list(guild_id=event.guild_id, no_cache=True)):
                 if str(event.channel_id) == per_channel['channel_id']:
```

### Comparing `mcqq-tool-0.0.2/setup.py` & `mcqq-tool-0.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="mcqq-tool",  # 项目名称，保证它的唯一性，不要跟已存在的包名冲突即可
-    version="0.0.2",  # 程序版本
+    version="0.0.3",  # 程序版本
     author="17TheWord",  # 项目作者
     author_email="17theword@gmail.com",  # 作者邮件
     description="MC_QQ 工具包",  # 项目的一句话描述
     long_description=long_description,  # 加长版描述？
     long_description_content_type="text/markdown",  # 描述使用Markdown
     url="https://github.com/17TheWord/mcqq-tool",  # 项目地址
     packages=setuptools.find_packages(),  # 无需修改
     classifiers=[
         "Programming Language :: Python :: 3.9",  # 使用Python3.9
         "License :: OSI Approved :: GNU Affero General Public License v3",  # 开源协议
-        "Operating System :: OS Independent",
+        "Operating System :: OS Independent"
     ],
     install_requires=[
         'websockets>=10.3',
         'aio-mc-rcon>=3.2.0'
     ]
 )
```

