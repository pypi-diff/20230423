# Comparing `tmp/nonebot_plugin_steam_game_status-0.0.7.tar.gz` & `tmp/nonebot_plugin_steam_game_status-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_steam_game_status-0.0.7.tar", last modified: Tue Apr  4 08:43:16 2023, max compression
+gzip compressed data, was "nonebot_plugin_steam_game_status-0.0.8.tar", last modified: Sun Apr 23 03:41:50 2023, max compression
```

## Comparing `nonebot_plugin_steam_game_status-0.0.7.tar` & `nonebot_plugin_steam_game_status-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-04 08:43:16.573281 nonebot_plugin_steam_game_status-0.0.7/
--rw-rw-rw-   0        0        0    35823 2023-04-03 08:15:10.000000 nonebot_plugin_steam_game_status-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     1781 2023-04-04 08:43:16.572282 nonebot_plugin_steam_game_status-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1352 2023-04-04 08:42:04.000000 nonebot_plugin_steam_game_status-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-04 08:43:16.566263 nonebot_plugin_steam_game_status-0.0.7/nonebot_plugin_steam_game_status/
--rw-rw-rw-   0        0        0    11621 2023-04-04 08:42:12.000000 nonebot_plugin_steam_game_status-0.0.7/nonebot_plugin_steam_game_status/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-04 08:43:16.571282 nonebot_plugin_steam_game_status-0.0.7/nonebot_plugin_steam_game_status.egg-info/
--rw-rw-rw-   0        0        0     1781 2023-04-04 08:43:16.000000 nonebot_plugin_steam_game_status-0.0.7/nonebot_plugin_steam_game_status.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      350 2023-04-04 08:43:16.000000 nonebot_plugin_steam_game_status-0.0.7/nonebot_plugin_steam_game_status.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-04 08:43:16.000000 nonebot_plugin_steam_game_status-0.0.7/nonebot_plugin_steam_game_status.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-04-04 08:43:16.000000 nonebot_plugin_steam_game_status-0.0.7/nonebot_plugin_steam_game_status.egg-info/requires.txt
--rw-rw-rw-   0        0        0       33 2023-04-04 08:43:16.000000 nonebot_plugin_steam_game_status-0.0.7/nonebot_plugin_steam_game_status.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-04 08:43:16.573281 nonebot_plugin_steam_game_status-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      868 2023-04-04 08:40:12.000000 nonebot_plugin_steam_game_status-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:41:50.274453 nonebot_plugin_steam_game_status-0.0.8/
+-rw-rw-rw-   0        0        0    35823 2023-04-03 08:15:10.000000 nonebot_plugin_steam_game_status-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     1927 2023-04-23 03:41:50.274453 nonebot_plugin_steam_game_status-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1498 2023-04-23 03:41:17.000000 nonebot_plugin_steam_game_status-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 03:41:50.268453 nonebot_plugin_steam_game_status-0.0.8/nonebot_plugin_steam_game_status/
+-rw-rw-rw-   0        0        0    11023 2023-04-23 03:37:54.000000 nonebot_plugin_steam_game_status-0.0.8/nonebot_plugin_steam_game_status/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:41:50.272452 nonebot_plugin_steam_game_status-0.0.8/nonebot_plugin_steam_game_status.egg-info/
+-rw-rw-rw-   0        0        0     1927 2023-04-23 03:41:50.000000 nonebot_plugin_steam_game_status-0.0.8/nonebot_plugin_steam_game_status.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      350 2023-04-23 03:41:50.000000 nonebot_plugin_steam_game_status-0.0.8/nonebot_plugin_steam_game_status.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 03:41:50.000000 nonebot_plugin_steam_game_status-0.0.8/nonebot_plugin_steam_game_status.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-04-23 03:41:50.000000 nonebot_plugin_steam_game_status-0.0.8/nonebot_plugin_steam_game_status.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       33 2023-04-23 03:41:50.000000 nonebot_plugin_steam_game_status-0.0.8/nonebot_plugin_steam_game_status.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 03:41:50.275452 nonebot_plugin_steam_game_status-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      868 2023-04-23 03:38:42.000000 nonebot_plugin_steam_game_status-0.0.8/setup.py
```

### Comparing `nonebot_plugin_steam_game_status-0.0.7/LICENSE` & `nonebot_plugin_steam_game_status-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_steam_game_status-0.0.7/PKG-INFO` & `nonebot_plugin_steam_game_status-0.0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_steam_game_status
-Version: 0.0.7
+Version: 0.0.8
 Summary: 在群内播报steam游戏状态的Nonebot插件
 Home-page: https://github.com/nek0us/nonebot_plugin_steam_game_status
 Author: nek0us
 Author-email: nekouss@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -46,7 +46,13 @@
 | steam列表/绑定列表 | 否 | 群聊 | 超管/群管 | 管理员命令 |    
 | steam播报开启/播报打开 | 否 | 群聊 | 超管/群管 | 管理员命令 |    
 | steam播报关闭/播报停止 | 否 | 群聊 | 超管/群管 | 管理员命令 |    
 
 ## 创意来源
 
 群友的koishi bot的该效果插件
+
+## 更新记录
+
+2023.04.23
+1.优化了监控代码，解决请求阻塞过久的问题
+2.解决消息在多账号下无法发送的问题
```

### Comparing `nonebot_plugin_steam_game_status-0.0.7/README.md` & `nonebot_plugin_steam_game_status-0.0.8/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -33,8 +33,14 @@
 | steam解绑/删除/.del | 否 | 群聊 | 群员 | 后加个人Steam ID |   
 | steam列表/绑定列表 | 否 | 群聊 | 超管/群管 | 管理员命令 |    
 | steam播报开启/播报打开 | 否 | 群聊 | 超管/群管 | 管理员命令 |    
 | steam播报关闭/播报停止 | 否 | 群聊 | 超管/群管 | 管理员命令 |    
 
 ## 创意来源
 
-群友的koishi bot的该效果插件
+群友的koishi bot的该效果插件
+
+## 更新记录
+
+2023.04.23
+1.优化了监控代码，解决请求阻塞过久的问题
+2.解决消息在多账号下无法发送的问题
```

### Comparing `nonebot_plugin_steam_game_status-0.0.7/nonebot_plugin_steam_game_status/__init__.py` & `nonebot_plugin_steam_game_status-0.0.8/nonebot_plugin_steam_game_status/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,18 +3,21 @@
 from nonebot_plugin_apscheduler import scheduler
 from nonebot.permission import SUPERUSER
 from nonebot.adapters.onebot.v11.permission import GROUP_ADMIN,GROUP_OWNER
 from nonebot.adapters.onebot.v11 import Message,MessageEvent,Bot,GroupMessageEvent
 from nonebot.matcher import Matcher
 from nonebot.params import CommandArg
 from nonebot.log import logger
+import nonebot
+from nonebot.adapters.onebot.v11.adapter import Adapter
 from pathlib import Path
 import json
 import time
 from httpx import AsyncClient
+import asyncio
 
 
 config_dev = get_driver().config
 try:
     steam_web_key = config_dev.steam_web_key
 except:
     logger.error("steam_web_key未配置")
@@ -22,91 +25,99 @@
     steam_web_key = ""
 
 dirpath = Path() / "data" / "steam_group"
 dirpath.mkdir(parents=True, exist_ok=True)
 dirpath = Path() / "data" / "steam_group" / "group_list.json"
 dirpath.touch()
 if not dirpath.stat().st_size:
-    with open(dirpath.__str__(),"w") as f:
-        f.write("{}")
-        f.close()
+    dirpath.write_text("{}")
 
 header = {
         "Host":"api.steampowered.com",
         "User-Agent":"Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/111.0",
         "Accept":"text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,*/*;q=0.8",
         "Accept-Language":"zh-CN,zh;q=0.8,zh-TW;q=0.7,zh-HK;q=0.5,en-US;q=0.3,en;q=0.2",
         "Accept-Encoding":"gzip, deflate, br",
         "Connection":"keep-alive",
         "Referer":"https://api.steampowered.com/ISteamUser/GetPlayerSummaries/v0002/",
         "TE":"trailers"
     }
+driver = get_driver()
+status = True
 
-
-
-@scheduler.scheduled_job("interval",minutes=1,id="steam")
-async def now_steam():
-    f = open(dirpath.__str__(),"r+")
-    group_list = f.read()
-    f.close()
-    group_list = json.loads(group_list)
-    for group_num in group_list:
-        if group_num and group_list[group_num]["status"] == "on":
-            for id in group_list[group_num]:
-                async with AsyncClient() as client:
+async def get_status(group_list,group_num,id):
+    async with AsyncClient() as client:
+        try:
+            url = "https://api.steampowered.com/ISteamUser/GetPlayerSummaries/v0002/?key=" + steam_web_key + "&steamids=" + id
+            res = await client.get(url,headers=header,timeout=30)
+            res_info = json.loads(res.text)["response"]["players"][0]
+            user_info = []
+            bots = nonebot.get_adapter(Adapter).bots
+            if "gameextrainfo" in res_info and group_list[group_num][id][1] == "":
+                #如果发现开始玩了而之前未玩
+                timestamp = int(time.time()/60)
+                user_info.append(timestamp)
+                user_info.append(res_info["gameextrainfo"])
+                user_info.append(res_info['personaname'])
+                group_list[group_num][id] = user_info
+                for bot in bots:
                     try:
-                        url = "https://api.steampowered.com/ISteamUser/GetPlayerSummaries/v0002/?key=" + steam_web_key + "&steamids=" + id
-                        res = await client.get(url,headers=header,timeout=30)
-                        res_info = json.loads(res.text)["response"]["players"][0]
-                        user_info = []
-                        bot = get_bot()
-                        if "gameextrainfo" in res_info and group_list[group_num][id][1] == "":
-                            #如果发现开始玩了而之前未玩
-                            timestamp = int(time.time()/60)
-                            user_info.append(timestamp)
-                            user_info.append(res_info["gameextrainfo"])
-                            user_info.append(res_info['personaname'])
-                            group_list[group_num][id] = user_info
-                            await bot.send_group_msg(group_id=int(group_num),message=Message(f"{res_info['personaname']} 开始玩 {res_info['gameextrainfo']} 。"))
-                            f = open(dirpath.__str__(),"w")
-                            f.write(json.dumps(group_list))
-                            f.close()
-                            pass
-                        elif "gameextrainfo" in res_info and group_list[group_num][id][1] != "":
-                            #如果发现开始玩了而之前也在玩
-                            if res_info["gameextrainfo"] != group_list[group_num][id][1]:
-                                #如果发现玩的是新游戏
-                                timestamp = int(time.time()/60)
-                                user_info.append(timestamp)
-                                user_info.append(res_info["gameextrainfo"])
-                                user_info.append(res_info['personaname'])
-                                group_list[group_num][id] = user_info
-                                await bot.send_group_msg(group_id=int(group_num),message=Message(f"{res_info['personaname']} 又开始玩 {res_info['gameextrainfo']} 。"))
-                                f = open(dirpath.__str__(),"w")
-                                f.write(json.dumps(group_list))
-                                f.close()
-                            pass
-                        elif "gameextrainfo" not in res_info and group_list[group_num][id][1] != "":
-                            # 之前有玩，现在没玩
-                            timestamp = int(time.time()/60)
-                            user_info.append(timestamp)
-                            user_info.append("")
-                            user_info.append(res_info['personaname'])
-                            game_time = timestamp - group_list[group_num][id][0]
-                            await bot.send_group_msg(group_id=int(group_num),message=Message(f"{res_info['personaname']} 玩了 {game_time} 分钟 {group_list[group_num][id][1]} 后不玩了。"))
-                            group_list[group_num][id] = user_info
-                            f = open(dirpath.__str__(),"w")
-                            f.write(json.dumps(group_list))
-                            f.close() 
-                            pass
-                        elif "gameextrainfo" not in res_info and group_list[group_num][id][1] == "":
-                            # 一直没玩
+                        await bots[bot].send_group_msg(group_id=int(group_num),message=Message(f"{res_info['personaname']} 开始玩 {res_info['gameextrainfo']} 了。"))
+                    except:
+                        pass
+                dirpath.write_text(json.dumps(group_list))
+            elif "gameextrainfo" in res_info and group_list[group_num][id][1] != "":
+                #如果发现开始玩了而之前也在玩
+                if res_info["gameextrainfo"] != group_list[group_num][id][1]:
+                    #如果发现玩的是新游戏
+                    timestamp = int(time.time()/60)
+                    user_info.append(timestamp)
+                    user_info.append(res_info["gameextrainfo"])
+                    user_info.append(res_info['personaname'])
+                    group_list[group_num][id] = user_info
+                    for bot in bots:
+                        try:
+                            await bots[bot].send_group_msg(group_id=int(group_num),message=Message(f"{res_info['personaname']} 又开始玩 {res_info['gameextrainfo']} 了。"))
+                        except:
                             pass
+                    dirpath.write_text(json.dumps(group_list))
+                pass
+            elif "gameextrainfo" not in res_info and group_list[group_num][id][1] != "":
+                # 之前有玩，现在没玩
+                timestamp = int(time.time()/60)
+                user_info.append(timestamp)
+                user_info.append("")
+                user_info.append(res_info['personaname'])
+                game_time = timestamp - group_list[group_num][id][0]
+                for bot in bots:
+                    try:
+                        await bots[bot].send_group_msg(group_id=int(group_num),message=Message(f"{res_info['personaname']} 玩了 {game_time} 分钟 {group_list[group_num][id][1]} 后不玩了。"))
                     except:
                         pass
+                group_list[group_num][id] = user_info
+                dirpath.write_text(json.dumps(group_list))
+            elif "gameextrainfo" not in res_info and group_list[group_num][id][1] == "":
+                # 一直没玩
+                pass
+        except:
+            pass
+    
+    
+    
+@scheduler.scheduled_job("interval",minutes=1,id="steam",misfire_grace_time=59)
+async def now_steam():
+    task_list = []
+    group_list = json.loads(dirpath.read_text("utf8"))
+    for group_num in group_list:
+        if group_num and group_list[group_num]["status"] == "on":
+            for id in group_list[group_num]:
+                if id != "status":
+                    task_list.append(get_status(group_list,group_num,id))
+    asyncio.gather(*task_list)
+                
                     
                     
 steam_bind = on_command("steam绑定",aliases={"steam.add","steam添加"},priority=5)
 @steam_bind.handle()
 async def steam_bind_handle(bot: Bot,event: MessageEvent,matcher: Matcher,arg: Message = CommandArg()):
     if isinstance(event,GroupMessageEvent):
         if not steam_web_key:
@@ -120,24 +131,19 @@
                 res = await client.get(url,headers=header,timeout=30)
                 if res.status_code != 200:
                     await steam_bind.finish(arg + " 绑定失败") 
                 steam_name = json.loads(res.text)["response"]["players"][0]['personaname']
         except:
             await steam_bind.finish(arg + " 绑定失败")
         
-        f = open(dirpath.__str__(),"r+")
-        group_list = f.read()
-        f.close()
-        group_list = json.loads(group_list)
+        group_list = json.loads(dirpath.read_text("utf8"))
         if str(event.group_id) not in group_list:
             group_list[str(event.group_id)] = {"status":"on"}
         group_list[str(event.group_id)][arg.extract_plain_text()] = [0,"",steam_name]
-        f = open(dirpath.__str__(),"w")
-        f.write(json.dumps(group_list))
-        f.close()
+        dirpath.write_text(json.dumps(group_list))
         await steam_bind.finish(f"Steam ID：{arg}\nSteam Name：{steam_name}\n 绑定成功了")
                             
 steam_del = on_command("steam删除",aliases={"steam.del","steam解绑"},priority=5)
 @steam_del.handle()
 async def steam_del_handle(bot: Bot,event: MessageEvent,matcher: Matcher,arg: Message = CommandArg()):
     if isinstance(event,GroupMessageEvent):
         if not steam_web_key:
@@ -152,41 +158,33 @@
                 if res.status_code != 200:
                     await steam_bind.finish(arg + " 解绑失败") 
                 steam_name = json.loads(res.text)["response"]["players"][0]['personaname']
         except:
             await steam_bind.finish(arg + " 解绑失败")
         
         
-        f = open(dirpath.__str__(),"r+")
-        group_list = f.read()
-        f.close()
-        group_list = json.loads(group_list)
+        group_list = json.loads(dirpath.read_text("utf8"))
         if str(event.group_id) not in group_list:
             group_list[str(event.group_id)] = {}
         try:
             group_list[str(event.group_id)].pop(arg.extract_plain_text()) 
         except:
             await steam_bind.finish(f"没有找到Steam ID：{arg}")
-        f = open(dirpath.__str__(),"w")
-        f.write(json.dumps(group_list))
-        f.close()
+        dirpath.write_text(json.dumps(group_list))
         await steam_bind.finish(f"Steam ID：{arg}\nSteam Name：{steam_name}\n 删除成功了")
             
         
         
         
 steam_bind_list = on_command("steam列表",aliases={"steam绑定列表","steam播报列表"},priority=5,permission=SUPERUSER|GROUP_ADMIN|GROUP_OWNER)
 @steam_bind_list.handle()
 async def steam_bind_list_handle(bot: Bot,event: MessageEvent,matcher: Matcher):
     if isinstance(event,GroupMessageEvent):
-        f = open(dirpath.__str__(),"r+")
-        group_list = f.read()
-        f.close()
         try:
-            id_list = json.loads(group_list)[str(event.group_id)]
+            id_list = json.loads(dirpath.read_text("utf8"))[str(event.group_id)]
             msg = []
             for id in id_list:
                 if "status" not in id:
                     msg += await node_msg(event.user_id,f"id：{id}\nname：{id_list[id][2]}")
                     
             await bot.send_group_forward_msg(group_id=event.group_id,messages=msg)
         except:
@@ -194,18 +192,15 @@
         
     
 
 steam_on = on_command("steam播报开启",aliases={"steam播报打开"},priority=5,permission=SUPERUSER|GROUP_ADMIN|GROUP_OWNER)
 @steam_on.handle()
 async def steam_on_handle(bot: Bot,event: MessageEvent,matcher: Matcher):
     if isinstance(event,GroupMessageEvent):
-        f = open(dirpath.__str__(),"r+")
-        group_list = f.read()
-        f.close()
-        group_list = json.loads(group_list)
+        group_list = json.loads(dirpath.read_text("utf8"))
         if str(event.group_id) not in group_list:
             group_list[str(event.group_id)] = {}
         group_list[str(event.group_id)]["status"] = "on"
         f = open(dirpath.__str__(),"w")
         f.write(json.dumps(group_list))
         f.close()
         await steam_on.finish("播报开启了")
@@ -217,17 +212,15 @@
         f = open(dirpath.__str__(),"r+")
         group_list = f.read()
         f.close()
         group_list = json.loads(group_list)
         if str(event.group_id) not in group_list:
             group_list[str(event.group_id)] = {}
         group_list[str(event.group_id)]["status"] = "off"
-        f = open(dirpath.__str__(),"w")
-        f.write(json.dumps(group_list))
-        f.close()
+        dirpath.write_text(json.dumps(group_list))
         await steam_on.finish("播报关闭了")
         
 async def node_msg(user_id,plain_text):
     if not plain_text:
         plain_text = "无"
     node = [
 	{
```

### Comparing `nonebot_plugin_steam_game_status-0.0.7/nonebot_plugin_steam_game_status.egg-info/PKG-INFO` & `nonebot_plugin_steam_game_status-0.0.8/nonebot_plugin_steam_game_status.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-steam-game-status
-Version: 0.0.7
+Version: 0.0.8
 Summary: 在群内播报steam游戏状态的Nonebot插件
 Home-page: https://github.com/nek0us/nonebot_plugin_steam_game_status
 Author: nek0us
 Author-email: nekouss@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -46,7 +46,13 @@
 | steam列表/绑定列表 | 否 | 群聊 | 超管/群管 | 管理员命令 |    
 | steam播报开启/播报打开 | 否 | 群聊 | 超管/群管 | 管理员命令 |    
 | steam播报关闭/播报停止 | 否 | 群聊 | 超管/群管 | 管理员命令 |    
 
 ## 创意来源
 
 群友的koishi bot的该效果插件
+
+## 更新记录
+
+2023.04.23
+1.优化了监控代码，解决请求阻塞过久的问题
+2.解决消息在多账号下无法发送的问题
```

### Comparing `nonebot_plugin_steam_game_status-0.0.7/setup.py` & `nonebot_plugin_steam_game_status-0.0.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r",encoding="utf-8") as readme_file:
     readme = readme_file.read()
 
 requirements = ["nonebot2","nonebot-adapter-onebot","nonebot-plugin-apscheduler","httpx"] # 这里填依赖包信息
 
 setup(
     name="nonebot_plugin_steam_game_status",
-    version="0.0.7",
+    version="0.0.8",
     author="nek0us",
     author_email="nekouss@gmail.com",
     description="在群内播报steam游戏状态的Nonebot插件",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/nek0us/nonebot_plugin_steam_game_status",
     packages=find_packages(),
```

