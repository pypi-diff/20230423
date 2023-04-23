# Comparing `tmp/nonebot_poe_chat-0.1.0.tar.gz` & `tmp/nonebot_poe_chat-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_poe_chat-0.1.0.tar", last modified: Sat Apr 22 14:50:33 2023, max compression
+gzip compressed data, was "nonebot_poe_chat-1.0.0.tar", last modified: Sun Apr 23 07:33:21 2023, max compression
```

## Comparing `nonebot_poe_chat-0.1.0.tar` & `nonebot_poe_chat-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 14:50:33.908421 nonebot_poe_chat-0.1.0/
--rw-rw-rw-   0        0        0    12533 2023-04-02 14:35:33.000000 nonebot_poe_chat-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0     3044 2023-04-22 14:50:33.907420 nonebot_poe_chat-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2549 2023-04-22 14:39:54.000000 nonebot_poe_chat-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-22 14:50:33.901421 nonebot_poe_chat-0.1.0/nonebot_poe_chat/
--rw-rw-rw-   0        0        0    23252 2023-04-22 14:49:51.000000 nonebot_poe_chat-0.1.0/nonebot_poe_chat/__init__.py
--rw-rw-rw-   0        0        0     3026 2023-04-21 14:27:42.000000 nonebot_poe_chat-0.1.0/nonebot_poe_chat/config.py
--rw-rw-rw-   0        0        0     4112 2023-04-22 14:35:57.000000 nonebot_poe_chat-0.1.0/nonebot_poe_chat/poe_chat.py
--rw-rw-rw-   0        0        0     1440 2023-04-21 14:27:42.000000 nonebot_poe_chat-0.1.0/nonebot_poe_chat/poe_clear.py
--rw-rw-rw-   0        0        0     2884 2023-04-21 14:53:32.000000 nonebot_poe_chat-0.1.0/nonebot_poe_chat/poe_create.py
--rw-rw-rw-   0        0        0     1261 2023-04-22 14:26:17.000000 nonebot_poe_chat-0.1.0/nonebot_poe_chat/poe_func.py
--rw-rw-rw-   0        0        0     2394 2023-04-22 14:36:31.000000 nonebot_poe_chat-0.1.0/nonebot_poe_chat/poe_login.py
-drwxrwxrwx   0        0        0        0 2023-04-22 14:50:33.906421 nonebot_poe_chat-0.1.0/nonebot_poe_chat.egg-info/
--rw-rw-rw-   0        0        0     3044 2023-04-22 14:50:33.000000 nonebot_poe_chat-0.1.0/nonebot_poe_chat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      434 2023-04-22 14:50:33.000000 nonebot_poe_chat-0.1.0/nonebot_poe_chat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 14:50:33.000000 nonebot_poe_chat-0.1.0/nonebot_poe_chat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      104 2023-04-22 14:50:33.000000 nonebot_poe_chat-0.1.0/nonebot_poe_chat.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-22 14:50:33.000000 nonebot_poe_chat-0.1.0/nonebot_poe_chat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-22 14:50:33.908421 nonebot_poe_chat-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1155 2023-04-22 14:50:16.000000 nonebot_poe_chat-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 07:33:21.586162 nonebot_poe_chat-1.0.0/
+-rw-rw-rw-   0        0        0    12533 2023-04-02 14:35:33.000000 nonebot_poe_chat-1.0.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     3044 2023-04-23 07:33:21.586162 nonebot_poe_chat-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2549 2023-04-22 14:39:54.000000 nonebot_poe_chat-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 07:33:21.579161 nonebot_poe_chat-1.0.0/nonebot_poe_chat/
+-rw-rw-rw-   0        0        0    24950 2023-04-23 07:23:33.000000 nonebot_poe_chat-1.0.0/nonebot_poe_chat/__init__.py
+-rw-rw-rw-   0        0        0     3609 2023-04-23 06:41:21.000000 nonebot_poe_chat-1.0.0/nonebot_poe_chat/config.py
+-rw-rw-rw-   0        0        0     4736 2023-04-23 07:08:03.000000 nonebot_poe_chat-1.0.0/nonebot_poe_chat/poe_chat.py
+-rw-rw-rw-   0        0        0     1965 2023-04-23 07:08:09.000000 nonebot_poe_chat-1.0.0/nonebot_poe_chat/poe_clear.py
+-rw-rw-rw-   0        0        0     3409 2023-04-23 07:08:14.000000 nonebot_poe_chat-1.0.0/nonebot_poe_chat/poe_create.py
+-rw-rw-rw-   0        0        0     2231 2023-04-23 03:10:23.000000 nonebot_poe_chat-1.0.0/nonebot_poe_chat/poe_func.py
+-rw-rw-rw-   0        0        0     2396 2023-04-23 07:05:56.000000 nonebot_poe_chat-1.0.0/nonebot_poe_chat/poe_login.py
+-rw-rw-rw-   0        0        0      490 2023-04-23 07:06:09.000000 nonebot_poe_chat-1.0.0/nonebot_poe_chat/temp.py
+-rw-rw-rw-   0        0        0    10632 2023-04-23 05:59:48.000000 nonebot_poe_chat-1.0.0/nonebot_poe_chat/txt2img.py
+drwxrwxrwx   0        0        0        0 2023-04-23 07:33:21.585163 nonebot_poe_chat-1.0.0/nonebot_poe_chat.egg-info/
+-rw-rw-rw-   0        0        0     3044 2023-04-23 07:33:21.000000 nonebot_poe_chat-1.0.0/nonebot_poe_chat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      487 2023-04-23 07:33:21.000000 nonebot_poe_chat-1.0.0/nonebot_poe_chat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 07:33:21.000000 nonebot_poe_chat-1.0.0/nonebot_poe_chat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      147 2023-04-23 07:33:21.000000 nonebot_poe_chat-1.0.0/nonebot_poe_chat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-04-23 07:33:21.000000 nonebot_poe_chat-1.0.0/nonebot_poe_chat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 07:33:21.586162 nonebot_poe_chat-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1236 2023-04-23 07:32:42.000000 nonebot_poe_chat-1.0.0/setup.py
```

### Comparing `nonebot_poe_chat-0.1.0/LICENSE.txt` & `nonebot_poe_chat-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nonebot_poe_chat-0.1.0/PKG-INFO` & `nonebot_poe_chat-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_poe_chat
-Version: 0.1.0
+Version: 1.0.0
 Summary: nonebot_poe_chat
 Home-page: https://github.com/canxin121/nonebot_poe_chat
 Author: canxin
 Author-email: 1969730106@qq.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_poe_chat Version: 0.1.0 Summary:
+Metadata-Version: 2.1 Name: nonebot_poe_chat Version: 1.0.0 Summary:
 nonebot_poe_chat Home-page: https://github.com/canxin121/nonebot_poe_chat
 Author: canxin Author-email: 1969730106@qq.com Classifier: Programming Language
 :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.8 Classifier:
 License :: OSI Approved :: GNU Affero General Public License v3 Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
 License-File: LICENSE.txt
                               [nonebot_poe_chat]
```

### Comparing `nonebot_poe_chat-0.1.0/README.md` & `nonebot_poe_chat-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_poe_chat-0.1.0/nonebot_poe_chat/__init__.py` & `nonebot_poe_chat-1.0.0/nonebot_poe_chat/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,44 @@
 import json,asyncio
 from nonebot.plugin import on_command, on
 from nonebot.params import ArgStr, CommandArg
 from nonebot.typing import T_State
 from nonebot.matcher import Matcher
-from nonebot.adapters.onebot.v11 import Message, Event, Bot, MessageEvent
+from nonebot.adapters.onebot.v11 import Message, Event, Bot, MessageEvent,MessageSegment
 from nonebot.internal.rule import Rule
 from playwright.async_api import async_playwright
 from .poe_chat import poe_chat
 from .poe_create import poe_create
 from .poe_clear import poe_clear
 from .poe_login import submit_email, submit_code
 from .config import Config
 from .poe_func import reply_out,generate_uuid,generate_random_string,is_email
+from .txt2img import Txt2Img
+txt2img = Txt2Img()
+
 #一些配置
 config = Config()
+server = config.server
+username = config.username
+passwd = config.passwd
+proxy_config = {}
+if server is not None:
+    proxy_config["server"] = server
+if username is not None:
+    proxy_config["username"] = username
+if passwd is not None:
+    proxy_config["password"] = passwd
 user_dict = config.user_dict
 prompts_dict = config.prompts_dict
 user_path = config.user_path
 prompt_path = config.prompt_path
 cookie_path = config.cookie_path
 superusers = config.superusers
 is_cookie_exists = config.is_cookie_exists
-
+is_pic_able = config.pic_able
 ######################################################
 
 async def delete_messages(bot, user_id, dict_list):
     if user_id in dict_list:
         for eachmsg in dict_list[user_id]:
             await bot.delete_msg(message_id=eachmsg['message_id'])
         del dict_list[user_id]
@@ -116,26 +129,27 @@
             await poe_switch.finish()
 
 ######################################################    
 
 #保留上一个回答的chatsuggest
 chat_lock = asyncio.Semaphore(3)
 chat_suggest = {}
+last_messageid = {}
 waitque = []
 poe_chat_ = on_command(
     "poetalk",
     aliases={
         "ptalk",
         "pt"
         },
     priority=1,
     block=False)
 @poe_chat_.handle()
 async def __chat_bot__(matcher:Matcher,event: Event, args: Message = CommandArg()):
-    global chat_lock,chat_suggest
+    global chat_lock,chat_suggest,last_messageid
     userid = str(event.user_id)
     if not is_cookie_exists:
         await matcher.finish(reply_out(event, "管理员还没填写可用的poe_cookie或登陆"))
     if userid not in user_dict:
         random = generate_random_string()
         truename = str(generate_uuid(str(userid + random)))
         is_created = await poe_create(cookie_path,truename,1,"一个智能助理")
@@ -175,29 +189,35 @@
             #这个应该不可能出现
             raise ValueError("Unexpected return type from get_message_async")
 
         if is_successful:
             suggest_str = '\n'.join([f"{i+1}: {s}" for i, s in enumerate(chat_suggest[userid])])
             msg = f"{last_answer}\n\n建议回复：\n{suggest_str}"
             waitque.remove(userid)
-            await matcher.finish(reply_out(event, msg))
+            if is_pic_able:
+                pic = await txt2img.draw(title=" ",text=msg)
+                last_messageid[userid] = await matcher.send(reply_out(event, pic))
+                matcher.finish()
+            else:
+                await matcher.finish(reply_out(event, msg))
         else:
             waitque.remove(userid)
             await matcher.finish(reply_out(event, "出错了，多次出错请联系机器人管理员"))
 
 ######################################################
 #判断是不是同一个对话中
 async def _is_reply_(event:MessageEvent,bot:Bot):
     if bool(event.reply):
         reply = event.reply
         user_id = str(event.user_id)
+        last_message_id = last_messageid[user_id]["message_id"]
         bot_id = bot.self_id
         sender_id = str(reply.sender.user_id)
         lastsuggest = str(reply.message).split("\n")[-1][3:]
-        if user_id in chat_suggest and sender_id == bot_id and lastsuggest == chat_suggest[user_id][-1]:
+        if user_id in chat_suggest and sender_id == bot_id and (lastsuggest == chat_suggest[user_id][-1] or last_message_id==reply.message_id):
             return True
     return False
 is_reply = Rule(_is_reply_)
 
 _poe_continue_ = on(rule=is_reply)
 @_poe_continue_.handle()
 async def __poe_continue__(matcher: Matcher,event:MessageEvent):
@@ -206,15 +226,15 @@
     if userid in waitque:
         await matcher.finish(reply_out(event, "你已经有一个对话进行中了，请等结束后在发送"))
     if userid in chat_suggest and len(raw_message) == 1 and raw_message in ['1','2','3','4']:
             text = chat_suggest[userid][int(raw_message)-1]
     else:
         text = raw_message
     
-    global chat_lock
+    global chat_lock,last_messageid
     if chat_lock.locked():
         await matcher.send(reply_out(event, '请稍等,你前面已有3个用户'))
         
     botname = str(list(user_dict[userid]["now"].values())[0])
         
     async with chat_lock:
         waitque.append(userid)
@@ -231,15 +251,20 @@
         else:
             raise ValueError("Unexpected return type from get_message_async")
 
         if is_successful:
             suggest_str = '\n'.join([f"{i+1}: {s}" for i, s in enumerate(chat_suggest[userid])])
             msg = f"{last_answer}\n\n建议回复：\n{suggest_str}"
             waitque.remove(userid)
-            await matcher.finish(reply_out(event, msg))
+            if is_pic_able:
+                pic = await txt2img.draw(title=" ",text=msg)
+                last_messageid[userid] = await matcher.send(reply_out(event, pic))
+                matcher.finish()
+            else:
+                await matcher.finish(reply_out(event, msg))
         else:
             waitque.remove(userid)
             await matcher.finish(reply_out(event, "出错了，多次出错请联系机器人管理员"))
     
 ######################################################   
 poe_clear_ = on_command(
     "poedump",
@@ -253,14 +278,16 @@
 async def __poe_clear___(event: Event,matcher:Matcher):
     if not is_cookie_exists:
         await matcher.finish(reply_out(event, "机器人管理员还没填写可用的poe_cookie或登陆"))
     userid = str(event.user_id)
     
     if userid not in user_dict:
         await matcher.finish(reply_out(event, "你还没有创建任何bot"))
+    if userid in waitque:
+        await matcher.finish(reply_out(event, "你现在有一个回话在进行中，不能清除历史记录"))
     botname = str(list(user_dict[userid]["now"].values())[0])
     nickname = str(list(user_dict[userid]["now"].keys())[0])
     is_cleared = await poe_clear(cookie_path,botname)
     if is_cleared:
         msg = f"成功清除了{nickname}的历史消息"
     else:
         msg = "出错了，多次错误请联系机器人主人"
@@ -316,51 +343,58 @@
     with open(user_path, 'w') as f:
         json.dump(user_dict, f)
     msg = f"已切换为{nickname}"
     await matcher.send(reply_out(event, msg))
     await asyncio.sleep(1)
     await delete_messages(bot,userid,switch_msgs)
     await poe_switch.finish()
-    
+remove_list = {}    
 ######################################################
 poe_remove = on_command(
     "poeremove",
     aliases={
         "删除bot",
         "pr"
         },
     priority=4,
     block=False)
 @poe_remove.handle()
 async def __poe_remove__(matcher:Matcher,event: Event):
     if not is_cookie_exists:
         await matcher.finish(reply_out(event, "管理员还没填写可用的poe_cookie或登陆"))
     userid = str(event.user_id)
+    remove_list[userid] = []
     if userid not in user_dict:
         await matcher.finish(reply_out(event, "你还没创建任何bot"))
     bots = list(user_dict[userid]["all"].keys())
     bot_str = '\n'.join(str(bot) for bot in bots)
     # bot_truname = str(list(user_dict[userid]["now"].values())[0])
     nickname = str(list(user_dict[userid]["now"].keys())[0])
     msg = "你已经创建的的bot有：\n" + bot_str +f"\n当前使用的bot是{nickname}\n\n请输入要删除的机器人名称"
-    await matcher.send(reply_out(event, msg))
+    remove_list.append(await matcher.send(reply_out(event, msg)))
 
 @poe_remove.got('nickname')
-async def __poe_remove____(matcher:Matcher,event: Event, infos: str = ArgStr("nickname")):
+async def __poe_remove____(bot:Bot,matcher:Matcher,event: Event, infos: str = ArgStr("nickname")):
     userid = str(event.user_id)
     bots = list(user_dict[userid]["all"].keys())
     if infos in ["取消", "算了"]:
-        await matcher.finish(reply_out(event, "终止切换"))
+        remove_list.append(await matcher.send(reply_out(event, "终止切换")))
+        await asyncio.sleep(1)
+        await delete_messages(bot,userid,remove_list)
     infos = infos.split(" ")
     nickname_delete = infos[0]
     nickname_now = str(list(user_dict[userid]["now"].keys())[0])
     if not (nickname_delete in bots): 
-        await matcher.reject(reply_out(event, "输入信息有误，请检查后重新输入"))
+        remove_list.append(await matcher.send(reply_out(event, "输入信息有误，请检查后重新输入")))
+        await poe_remove.reject()
     if nickname_delete == nickname_now:
-        await matcher.finish(reply_out(event, "不能删除正在使用的bot哦"))
+        remove_list.append(await matcher.send(reply_out(event, "不能删除正在使用的bot哦")))
+        await asyncio.sleep(1)
+        await delete_messages(bot,userid,remove_list)
+        await poe_remove.finish()
     del user_dict[userid]["all"][nickname_delete]
     with open(user_path, 'w') as f:
         json.dump(user_dict, f)
     await matcher.finish(reply_out(event, f"已删除{nickname_delete}"))
     
 #####################################################
 
@@ -388,18 +422,20 @@
     if infos in ["取消", "算了"]:
         await poe_login.finish("终止登陆")
     infos = infos.split(" ")
     if len(infos) != 1 or not is_email(infos[0]):
         await poe_login.reject("你输入的邮箱有误，请重新输入")
 
     playwright = await create_playwright_instance()
-    browser = await playwright.chromium.launch()
+    if proxy_config:
+        browser = await playwright.chromium.launch(proxy=proxy_config,headless=False)
+    else:
+        browser = await playwright.chromium.launch()
     context = await browser.new_context()
     page = await context.new_page()
-
     state["playwright"] = playwright
     state["browser"] = browser
     state["context"] = context
     state["page"] = page
 
     is_submitted_email = await submit_email(page, infos[0])
     if is_submitted_email:
@@ -514,15 +550,14 @@
         "ph"
         },
     priority=4,
     block=False)
 @poe_help.handle()
 async def __poe_help__(bot: Bot,event: Event):
     msg = (
-    "-poe功能大全\n"
     "--注意所有功能都是用户独立的，每个用户只能操作自己的内容\n"
     "--所有分步操作都可以用 取消 或 算了来终止,并且支持错误重输\n"
     "--如果未创建机器人，对话命令将默认创建gpt3.5\n"
     "--可以直接回复机器人给你的回答来继续对话，无需命令\n"
     "--可以使用数字索引来使用建议回复\n\n"
     "--以下命令前面全部要加 / \n"
     "~对话:poetalk / ptalk / pt\n"
@@ -533,11 +568,12 @@
     "************************\n"
     "--以下功能仅限poe管理员使用\n"
     "~登录:poelogin / plogin / pl\n"
     "~添加预设:poeaddprompt / 添加预设 / pap\n"
     "~删除预设:poeremoveprompt / 删除预设 / prp"
     )
     
-    helpmsg = await poe_help.send(msg)
+    pic = await txt2img.draw(title="poe功能大全",text=msg)
+    helpmsg = await poe_help.send(MessageSegment.image(pic))
     await asyncio.sleep(30)
     await bot.delete_msg(message_id=helpmsg['message_id'])
     await poe_help.finish()
```

### Comparing `nonebot_poe_chat-0.1.0/nonebot_poe_chat/config.py` & `nonebot_poe_chat-1.0.0/nonebot_poe_chat/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -40,23 +40,43 @@
     return False
 class Config:
     def __init__(self):
         self.path_ = str(Path()) + "/data/poe_chat"
         self.user_path = str(self.path_ + r'/user_dict.json')
         self.prompt_path = str(self.path_ + r'/poe_prompt.json')
         self.cookie_path = str(self.path_ + r'/poe_cookie.json')
+        self.pic_able = True
+        self.server = None
+        self.username = None
+        self.passwd = None
         self.superusers = []
         self.user_dict = {}
         self.prompts_dict = {}
         self.is_cookie_exists = check_cookie(self)
         # 加载超级用户配置
         try:
             self.superusers = nonebot.get_driver().config.poe_superusers
         except:
             pass
+        try:
+            self.pic_able = nonebot.get_driver().config.poe_picable
+        except:
+            pass
+        try:
+            self.server = nonebot.get_driver().config.poe_server
+        except:
+            pass
+        try:
+            self.username = nonebot.get_driver().config.poe_username
+        except:
+            pass
+        try:
+            self.passwd = nonebot.get_driver().config.poe_passwd
+        except:
+            pass
         
         # 加载用户配置文件
         if not os.path.exists(self.user_path):
             # 获取目录路径
             dir_path = os.path.dirname(self.user_path)
             # 如果目录不存在，则创建目录
             if not os.path.exists(dir_path):
```

### Comparing `nonebot_poe_chat-0.1.0/nonebot_poe_chat/poe_chat.py` & `nonebot_poe_chat-1.0.0/nonebot_poe_chat/poe_chat.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import asyncio
 import json
 import re
 from playwright.async_api import async_playwright
 from playwright.sync_api import Page
-
+from .config import Config
+config = Config()
 async def send_message_async(page: Page, botname: str, input_str: str):
     # 定义重试次数和重试间隔时间
     retry_count = 5
     retry_interval = 0.5
 
     # 定义当前重试次数和报错次数
     current_retry = 0
@@ -19,22 +20,22 @@
             # 打开目标网页
             await page.goto(f'https://poe.com/{botname}')
             text = "This bot has been deleted for violating our"
             content = await page.content()
             if text in content:
                 return "banned"
             # 找到输入框元素
-            input_box = await page.wait_for_selector('.ChatMessageInputView_textInput__Aervw')
+            input_box = await page.wait_for_selector('.ChatMessageInputView_textInput__Aervw',timeout=2000)
 
             # 将字符串发送到输入框中
             await input_box.fill(input_str)
 
-            # 找到发送按钮元素并点击
-            await page.wait_for_selector('button.Button_primary__pIDjn')
-            send_button = await page.wait_for_selector('button.Button_primary__pIDjn')
+            # 找到发送按钮元素并点击,容易点不到，多等一次
+            await page.wait_for_selector('button.Button_primary__pIDjn',timeout=1000)
+            send_button = await page.wait_for_selector('button.Button_primary__pIDjn',timeout=1000)
             # await asyncio.sleep(0.5)
             await send_button.click()
             # 发送成功后退出循环
             break
         except:
             # 如果出现超时异常，打印错误信息并稍等一段时间后重试
             error_count += 1
@@ -74,27 +75,42 @@
             if consecutive_errors >= 10:
                 return False
         else:
             consecutive_errors = 0
 
 async def poe_chat(cookie_path,botname,question):
     async with async_playwright() as p:
-        browser = await p.chromium.launch()
+        server = config.server
+        username = config.username
+        passwd = config.passwd
+        proxy_config = {}
+        if server is not None:
+            proxy_config["server"] = server
+        if username is not None:
+            proxy_config["username"] = username
+        if passwd is not None:
+            proxy_config["password"] = passwd
+
+        if proxy_config:
+            browser = await p.chromium.launch(proxy=proxy_config)
+        else:
+            browser = await p.chromium.launch()
         context = await browser.new_context()
         page = await context.new_page()
         with open(cookie_path, 'r') as f:
             cookies = json.load(f)
         await context.add_cookies(cookies=cookies)
         is_banned = await send_message_async(page, botname, question)
         if is_banned == "banned":
             return "banned"
-        result = await get_message_async(page, botname, sleep=5)
+        result = await get_message_async(page, botname, sleep=3)
         if isinstance(result, tuple):
             answers, suggests = result
+            return answers[-1],suggests
         elif isinstance(result, str):
             is_banned = result
             return "banned"
         elif isinstance(result, bool):
             is_got = result
+            return is_got
         else:
-            raise ValueError("Unexpected return type from get_message_async")
-        return answers[-1],suggests
+            raise ValueError("Unexpected return type from get_message_async")
```

#### html2text {}

```diff
@@ -1,21 +1,23 @@
 import asyncio import json import re from playwright.async_api import
-async_playwright from playwright.sync_api import Page async def
-send_message_async(page: Page, botname: str, input_str: str): #
-å®ä¹éè¯æ¬¡æ°åéè¯é´éæ¶é´ retry_count = 5 retry_interval = 0.5 #
-å®ä¹å½åéè¯æ¬¡æ°åæ¥éæ¬¡æ° current_retry = 0 error_count = 0 while
-current_retry < retry_count: try: # æå¼ç®æ ç½é¡µ await page.goto(f'https:
-//poe.com/{botname}') text = "This bot has been deleted for violating our"
-content = await page.content() if text in content: return "banned" #
-æ¾å°è¾å¥æ¡åç´  input_box = await page.wait_for_selector
-('.ChatMessageInputView_textInput__Aervw') # å°å­ç¬¦ä¸²åéå°è¾å¥æ¡ä¸­
-await input_box.fill(input_str) # æ¾å°åéæé®åç´ å¹¶ç¹å» await
-page.wait_for_selector('button.Button_primary__pIDjn') send_button = await
-page.wait_for_selector('button.Button_primary__pIDjn') # await asyncio.sleep
-(0.5) await send_button.click() # åéæååéåºå¾ªç¯ break except: #
+async_playwright from playwright.sync_api import Page from .config import
+Config config = Config() async def send_message_async(page: Page, botname: str,
+input_str: str): # å®ä¹éè¯æ¬¡æ°åéè¯é´éæ¶é´ retry_count = 5
+retry_interval = 0.5 # å®ä¹å½åéè¯æ¬¡æ°åæ¥éæ¬¡æ° current_retry =
+0 error_count = 0 while current_retry < retry_count: try: # æå¼ç®æ ç½é¡µ
+await page.goto(f'https://poe.com/{botname}') text = "This bot has been deleted
+for violating our" content = await page.content() if text in content: return
+"banned" # æ¾å°è¾å¥æ¡åç´  input_box = await page.wait_for_selector
+('.ChatMessageInputView_textInput__Aervw',timeout=2000) #
+å°å­ç¬¦ä¸²åéå°è¾å¥æ¡ä¸­ await input_box.fill(input_str) #
+æ¾å°åéæé®åç´ å¹¶ç¹å»,å®¹æç¹ä¸å°ï¼å¤ç­ä¸æ¬¡ await
+page.wait_for_selector('button.Button_primary__pIDjn',timeout=1000) send_button
+= await page.wait_for_selector('button.Button_primary__pIDjn',timeout=1000) #
+await asyncio.sleep(0.5) await send_button.click() #
+åéæååéåºå¾ªç¯ break except: #
 å¦æåºç°è¶æ¶å¼å¸¸ï¼æå°éè¯¯ä¿¡æ¯å¹¶ç¨ç­ä¸æ®µæ¶é´åéè¯
 error_count += 1 if error_count >= 1: await asyncio.sleep(retry_interval)
 current_retry += 1 continue if current_retry == retry_count: return False async
 def get_message_async(page,botname, sleep): consecutive_errors = 0 # initialize
 a counter for consecutive errors while True: await asyncio.sleep(sleep) try:
 await page.goto(f'https://poe.com/{botname}') response = await page.content()
 text = "This bot has been deleted for violating our" if text in response:
@@ -26,16 +28,20 @@
 chat_list_raw = [a["node"] for a in chat_list_raw] chat_list_text = [a["text"]
 for a in chat_list_raw] if chat_list_text[-1]: match_suggest = re.search(r'*
 (.*?)', response, re.DOTALL) string_list = re.findall(r'>\s*([^<>\n]+)\s*<',
 match_suggest.group(1)) if len(string_list) == 4: return chat_list_text,
 string_list except : consecutive_errors += 1 print(consecutive_errors) if
 consecutive_errors >= 10: return False else: consecutive_errors = 0 async def
 poe_chat(cookie_path,botname,question): async with async_playwright() as p:
-browser = await p.chromium.launch() context = await browser.new_context() page
-= await context.new_page() with open(cookie_path, 'r') as f: cookies =
-json.load(f) await context.add_cookies(cookies=cookies) is_banned = await
-send_message_async(page, botname, question) if is_banned == "banned": return
-"banned" result = await get_message_async(page, botname, sleep=5) if isinstance
-(result, tuple): answers, suggests = result elif isinstance(result, str):
-is_banned = result return "banned" elif isinstance(result, bool): is_got =
-result else: raise ValueError("Unexpected return type from get_message_async")
-return answers[-1],suggests
+server = config.server username = config.username passwd = config.passwd
+proxy_config = {} if server is not None: proxy_config["server"] = server if
+username is not None: proxy_config["username"] = username if passwd is not
+None: proxy_config["password"] = passwd if proxy_config: browser = await
+p.chromium.launch(proxy=proxy_config) else: browser = await p.chromium.launch()
+context = await browser.new_context() page = await context.new_page() with open
+(cookie_path, 'r') as f: cookies = json.load(f) await context.add_cookies
+(cookies=cookies) is_banned = await send_message_async(page, botname, question)
+if is_banned == "banned": return "banned" result = await get_message_async
+(page, botname, sleep=3) if isinstance(result, tuple): answers, suggests =
+result return answers[-1],suggests elif isinstance(result, str): is_banned =
+result return "banned" elif isinstance(result, bool): is_got = result return
+is_got else: raise ValueError("Unexpected return type from get_message_async")
```

### Comparing `nonebot_poe_chat-0.1.0/nonebot_poe_chat/poe_create.py` & `nonebot_poe_chat-1.0.0/nonebot_poe_chat/poe_create.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 from playwright.async_api import async_playwright, ElementHandle
-
+from .config import Config
+config = Config()
 async def create_bot_async(page, botname, base_bot_index, prompt, retries=2):
     try:
         for i in range(retries):
             await page.goto('https://poe.com/create_bot')
 
             # 定位输入框并清空原有的默认值
             name_input: ElementHandle = await page.wait_for_selector('input[name="name"]')
@@ -50,15 +51,29 @@
 
         return False
     finally:
         await page.close()
 # cookie_path = r"C:\Users\Administrator\Desktop\nonebot2\cccc\src\plugins\nonebot_poe_chat\data\poe_cookie.json"                      
 async def poe_create(cookie_path,botname, base_bot_index, prompt):
     async with async_playwright() as p:
-        browser = await p.chromium.launch()
+        server = config.server
+        username = config.username
+        passwd = config.passwd
+        proxy_config = {}
+        if server is not None:
+            proxy_config["server"] = server
+        if username is not None:
+            proxy_config["username"] = username
+        if passwd is not None:
+            proxy_config["password"] = passwd
+
+        if proxy_config:
+            browser = await p.chromium.launch(proxy=proxy_config)
+        else:
+            browser = await p.chromium.launch()
         context = await browser.new_context()
         page = await context.new_page()
         with open(cookie_path, 'r') as f:
             cookies = json.load(f)
         await context.add_cookies(cookies=cookies)
         is_created = await create_bot_async(page,botname, base_bot_index, prompt, retries=5)
         await context.close()
```

### Comparing `nonebot_poe_chat-0.1.0/nonebot_poe_chat/poe_login.py` & `nonebot_poe_chat-1.0.0/nonebot_poe_chat/poe_login.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import asyncio
 import json
+
 async def submit_email(page,email):
     for i in range(5):
         try:
             await page.goto("https://poe.com")
             # 点击 "Use email" 按钮
             use_email_button = await page.query_selector('button:has-text("Use email")')
             await use_email_button.click()
```

### Comparing `nonebot_poe_chat-0.1.0/nonebot_poe_chat.egg-info/PKG-INFO` & `nonebot_poe_chat-1.0.0/nonebot_poe_chat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-poe-chat
-Version: 0.1.0
+Version: 1.0.0
 Summary: nonebot_poe_chat
 Home-page: https://github.com/canxin121/nonebot_poe_chat
 Author: canxin
 Author-email: 1969730106@qq.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-poe-chat Version: 0.1.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-poe-chat Version: 1.0.0 Summary:
 nonebot_poe_chat Home-page: https://github.com/canxin121/nonebot_poe_chat
 Author: canxin Author-email: 1969730106@qq.com Classifier: Programming Language
 :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.8 Classifier:
 License :: OSI Approved :: GNU Affero General Public License v3 Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
 License-File: LICENSE.txt
                               [nonebot_poe_chat]
```

### Comparing `nonebot_poe_chat-0.1.0/setup.py` & `nonebot_poe_chat-1.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="nonebot_poe_chat",  # 项目名称，保证它的唯一性，不要跟已存在的包名冲突即可
-    version="0.1.0",  # 程序版本
+    version="1.0.0",  # 程序版本
     author="canxin",  # 项目作者
     author_email="1969730106@qq.com",  # 作者邮件
     description="nonebot_poe_chat",  # 项目的一句话描述
     long_description=long_description,  # 加长版描述
     long_description_content_type="text/markdown",  # 描述使用Markdown
     url="https://github.com/canxin121/nonebot_poe_chat",  # 项目地址
     packages=setuptools.find_packages(),  # 无需修改
@@ -19,10 +19,14 @@
         "License :: OSI Approved :: GNU Affero General Public License v3",  # 开源协议
         "Operating System :: OS Independent",
     ],
     install_requires=[
         'nonebot2>=2.0.0rc3',
         'nonebot-adapter-onebot>=2.0.0b1',
         'nonebot_plugin_guild_patch>=0.2.3',
-        'playwright>=1.32.1'
+        'playwright>=1.32.1',
+        'aiohttp>=3.8.4',
+        'Pillow>=9.5.0',
+        'qrcode>=7.4.2'
+
     ]
 )
```

