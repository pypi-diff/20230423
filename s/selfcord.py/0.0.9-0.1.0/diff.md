# Comparing `tmp/selfcord.py-0.0.9.tar.gz` & `tmp/selfcord.py-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selfcord.py-0.0.9.tar", last modified: Sun Nov 27 20:34:13 2022, max compression
+gzip compressed data, was "selfcord.py-0.1.0.tar", last modified: Sun Apr 23 01:45:09 2023, max compression
```

## Comparing `selfcord.py-0.0.9.tar` & `selfcord.py-0.1.0.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2022-11-27 20:34:13.666568 selfcord.py-0.0.9/
--rw-r--r--   0 shell     (1000) shell     (1001)     2338 2022-11-27 20:34:13.666568 selfcord.py-0.0.9/PKG-INFO
--rw-r--r--   0 shell     (1000) shell     (1001)     2050 2022-11-20 03:11:59.000000 selfcord.py-0.0.9/README.md
-drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2022-11-27 20:34:13.653235 selfcord.py-0.0.9/selfcord/
--rw-r--r--   0 shell     (1000) shell     (1001)       82 2022-11-11 20:03:04.000000 selfcord.py-0.0.9/selfcord/__init__.py
-drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2022-11-27 20:34:13.656568 selfcord.py-0.0.9/selfcord/api/
--rw-r--r--   0 shell     (1000) shell     (1001)      127 2022-11-11 20:02:32.000000 selfcord.py-0.0.9/selfcord/api/__init__.py
--rw-r--r--   0 shell     (1000) shell     (1001)      527 2022-11-11 01:44:22.000000 selfcord.py-0.0.9/selfcord/api/errors.py
--rw-r--r--   0 shell     (1000) shell     (1001)     7824 2022-11-11 01:44:22.000000 selfcord.py-0.0.9/selfcord/api/events.py
--rw-r--r--   0 shell     (1000) shell     (1001)    14476 2022-11-24 14:11:05.000000 selfcord.py-0.0.9/selfcord/api/gateway.py
--rw-r--r--   0 shell     (1000) shell     (1001)     7642 2022-11-24 14:12:34.000000 selfcord.py-0.0.9/selfcord/api/http.py
--rw-r--r--   0 shell     (1000) shell     (1001)    13164 2022-11-27 03:02:07.000000 selfcord.py-0.0.9/selfcord/bot.py
-drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2022-11-27 20:34:13.663235 selfcord.py-0.0.9/selfcord/models/
--rw-r--r--   0 shell     (1000) shell     (1001)      412 2022-11-21 22:16:05.000000 selfcord.py-0.0.9/selfcord/models/__init__.py
--rw-r--r--   0 shell     (1000) shell     (1001)    13093 2022-11-24 14:12:20.000000 selfcord.py-0.0.9/selfcord/models/channel.py
--rw-r--r--   0 shell     (1000) shell     (1001)      902 2022-11-21 18:38:16.000000 selfcord.py-0.0.9/selfcord/models/client.py
--rw-r--r--   0 shell     (1000) shell     (1001)      697 2022-10-31 21:14:11.000000 selfcord.py-0.0.9/selfcord/models/emoji.py
--rw-r--r--   0 shell     (1000) shell     (1001)     5149 2022-11-21 17:56:07.000000 selfcord.py-0.0.9/selfcord/models/guild.py
--rw-r--r--   0 shell     (1000) shell     (1001)      783 2022-11-21 18:38:32.000000 selfcord.py-0.0.9/selfcord/models/member.py
--rw-r--r--   0 shell     (1000) shell     (1001)     1558 2022-11-17 17:14:15.000000 selfcord.py-0.0.9/selfcord/models/message.py
--rw-r--r--   0 shell     (1000) shell     (1001)     2125 2022-10-18 15:17:31.000000 selfcord.py-0.0.9/selfcord/models/permission.py
--rw-r--r--   0 shell     (1000) shell     (1001)     1360 2022-11-22 16:33:43.000000 selfcord.py-0.0.9/selfcord/models/role.py
--rw-r--r--   0 shell     (1000) shell     (1001)     2993 2022-11-21 18:40:17.000000 selfcord.py-0.0.9/selfcord/models/user.py
--rw-r--r--   0 shell     (1000) shell     (1001)      999 2022-10-25 00:32:59.000000 selfcord.py-0.0.9/selfcord/models/webhook.py
-drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2022-11-27 20:34:13.666568 selfcord.py-0.0.9/selfcord/utils/
--rw-r--r--   0 shell     (1000) shell     (1001)      150 2022-11-27 03:03:09.000000 selfcord.py-0.0.9/selfcord/utils/__init__.py
--rw-r--r--   0 shell     (1000) shell     (1001)    12664 2022-11-24 15:50:53.000000 selfcord.py-0.0.9/selfcord/utils/command.py
-drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2022-11-27 20:34:13.653235 selfcord.py-0.0.9/selfcord.py.egg-info/
--rw-r--r--   0 shell     (1000) shell     (1001)     2338 2022-11-27 20:34:13.000000 selfcord.py-0.0.9/selfcord.py.egg-info/PKG-INFO
--rw-r--r--   0 shell     (1000) shell     (1001)      687 2022-11-27 20:34:13.000000 selfcord.py-0.0.9/selfcord.py.egg-info/SOURCES.txt
--rw-r--r--   0 shell     (1000) shell     (1001)        1 2022-11-27 20:34:13.000000 selfcord.py-0.0.9/selfcord.py.egg-info/dependency_links.txt
--rw-r--r--   0 shell     (1000) shell     (1001)       75 2022-11-27 20:34:13.000000 selfcord.py-0.0.9/selfcord.py.egg-info/requires.txt
--rw-r--r--   0 shell     (1000) shell     (1001)        9 2022-11-27 20:34:13.000000 selfcord.py-0.0.9/selfcord.py.egg-info/top_level.txt
--rw-r--r--   0 shell     (1000) shell     (1001)       38 2022-11-27 20:34:13.666568 selfcord.py-0.0.9/setup.cfg
--rw-r--r--   0 shell     (1000) shell     (1001)     1016 2022-11-27 20:34:09.000000 selfcord.py-0.0.9/setup.py
+drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-04-23 01:45:09.386142 selfcord.py-0.1.0/
+-rw-r--r--   0 shell     (1000) shell     (1001)     2338 2023-04-23 01:45:09.382809 selfcord.py-0.1.0/PKG-INFO
+-rw-r--r--   0 shell     (1000) shell     (1001)     2051 2023-04-23 01:42:38.000000 selfcord.py-0.1.0/README.md
+drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-04-23 01:45:09.369475 selfcord.py-0.1.0/selfcord/
+-rw-r--r--   0 shell     (1000) shell     (1001)       82 2022-11-11 20:03:04.000000 selfcord.py-0.1.0/selfcord/__init__.py
+drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-04-23 01:45:09.376142 selfcord.py-0.1.0/selfcord/api/
+-rw-r--r--   0 shell     (1000) shell     (1001)      127 2022-11-11 20:02:32.000000 selfcord.py-0.1.0/selfcord/api/__init__.py
+-rw-r--r--   0 shell     (1000) shell     (1001)      527 2022-11-11 01:44:22.000000 selfcord.py-0.1.0/selfcord/api/errors.py
+-rw-r--r--   0 shell     (1000) shell     (1001)     7821 2023-04-22 21:54:23.000000 selfcord.py-0.1.0/selfcord/api/events.py
+-rw-r--r--   0 shell     (1000) shell     (1001)    14248 2023-04-22 21:54:23.000000 selfcord.py-0.1.0/selfcord/api/gateway.py
+-rw-r--r--   0 shell     (1000) shell     (1001)     7729 2023-04-21 02:29:42.000000 selfcord.py-0.1.0/selfcord/api/http.py
+-rw-r--r--   0 shell     (1000) shell     (1001)    12960 2023-04-23 01:18:18.000000 selfcord.py-0.1.0/selfcord/bot.py
+drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-04-23 01:45:09.382809 selfcord.py-0.1.0/selfcord/models/
+-rw-r--r--   0 shell     (1000) shell     (1001)      412 2022-11-21 22:16:05.000000 selfcord.py-0.1.0/selfcord/models/__init__.py
+-rw-r--r--   0 shell     (1000) shell     (1001)    13535 2023-04-21 02:29:42.000000 selfcord.py-0.1.0/selfcord/models/channel.py
+-rw-r--r--   0 shell     (1000) shell     (1001)      902 2022-11-21 18:38:16.000000 selfcord.py-0.1.0/selfcord/models/client.py
+-rw-r--r--   0 shell     (1000) shell     (1001)      697 2022-10-31 21:14:11.000000 selfcord.py-0.1.0/selfcord/models/emoji.py
+-rw-r--r--   0 shell     (1000) shell     (1001)     5149 2022-11-21 17:56:07.000000 selfcord.py-0.1.0/selfcord/models/guild.py
+-rw-r--r--   0 shell     (1000) shell     (1001)      783 2022-11-21 18:38:32.000000 selfcord.py-0.1.0/selfcord/models/member.py
+-rw-r--r--   0 shell     (1000) shell     (1001)     1558 2022-11-17 17:14:15.000000 selfcord.py-0.1.0/selfcord/models/message.py
+-rw-r--r--   0 shell     (1000) shell     (1001)     2125 2022-10-18 15:17:31.000000 selfcord.py-0.1.0/selfcord/models/permission.py
+-rw-r--r--   0 shell     (1000) shell     (1001)     1360 2022-11-22 16:33:43.000000 selfcord.py-0.1.0/selfcord/models/role.py
+-rw-r--r--   0 shell     (1000) shell     (1001)     3024 2023-04-21 02:29:42.000000 selfcord.py-0.1.0/selfcord/models/user.py
+-rw-r--r--   0 shell     (1000) shell     (1001)      999 2022-10-25 00:32:59.000000 selfcord.py-0.1.0/selfcord/models/webhook.py
+drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-04-23 01:45:09.382809 selfcord.py-0.1.0/selfcord/utils/
+-rw-r--r--   0 shell     (1000) shell     (1001)      150 2022-11-27 03:03:09.000000 selfcord.py-0.1.0/selfcord/utils/__init__.py
+-rw-r--r--   0 shell     (1000) shell     (1001)    12830 2023-04-23 01:21:27.000000 selfcord.py-0.1.0/selfcord/utils/command.py
+drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-04-23 01:45:09.372808 selfcord.py-0.1.0/selfcord.py.egg-info/
+-rw-r--r--   0 shell     (1000) shell     (1001)     2338 2023-04-23 01:45:09.000000 selfcord.py-0.1.0/selfcord.py.egg-info/PKG-INFO
+-rw-r--r--   0 shell     (1000) shell     (1001)      710 2023-04-23 01:45:09.000000 selfcord.py-0.1.0/selfcord.py.egg-info/SOURCES.txt
+-rw-r--r--   0 shell     (1000) shell     (1001)        1 2023-04-23 01:45:09.000000 selfcord.py-0.1.0/selfcord.py.egg-info/dependency_links.txt
+-rw-r--r--   0 shell     (1000) shell     (1001)       75 2023-04-23 01:45:09.000000 selfcord.py-0.1.0/selfcord.py.egg-info/requires.txt
+-rw-r--r--   0 shell     (1000) shell     (1001)        9 2023-04-23 01:45:09.000000 selfcord.py-0.1.0/selfcord.py.egg-info/top_level.txt
+-rw-r--r--   0 shell     (1000) shell     (1001)       38 2023-04-23 01:45:09.386142 selfcord.py-0.1.0/setup.cfg
+-rw-r--r--   0 shell     (1000) shell     (1001)     1016 2023-04-23 01:44:56.000000 selfcord.py-0.1.0/setup.py
+drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-04-23 01:45:09.382809 selfcord.py-0.1.0/tests/
+-rw-r--r--   0 shell     (1000) shell     (1001)      475 2022-10-24 15:21:37.000000 selfcord.py-0.1.0/tests/test_commands.py
```

### Comparing `selfcord.py-0.0.9/PKG-INFO` & `selfcord.py-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selfcord.py
-Version: 0.0.9
+Version: 0.1.0
 Summary: A Discord API wrapper designed for selfbots!
 Home-page: https://github.com/Shell1010/Selfcord
 Author: Shell of OMEGA
 License: MIT
 Keywords: selfbot,discord,discordapi,discordwrapper
 Description-Content-Type: text/markdown
 
@@ -90,8 +90,8 @@
     await ctx.reply(f"{bot.user.deleted_messages[-1].author}: {bot.user.deleted_messages[-1]}")
 
 bot.run(token)
 ```
 
 ## Help & Support
 
-Please join our [discord server](https://discord.gg/W5QMKHejQB) here.
+Please join our [discord server](https://discord.gg/FCFnnBGzkg) here.
```

### Comparing `selfcord.py-0.0.9/README.md` & `selfcord.py-0.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -80,8 +80,8 @@
     await ctx.reply(f"{bot.user.deleted_messages[-1].author}: {bot.user.deleted_messages[-1]}")
 
 bot.run(token)
 ```
 
 ## Help & Support
 
-Please join our [discord server](https://discord.gg/W5QMKHejQB) here.
+Please join our [discord server](https://discord.gg/FCFnnBGzkg) here.
```

### Comparing `selfcord.py-0.0.9/selfcord/api/errors.py` & `selfcord.py-0.1.0/selfcord/api/errors.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.0.9/selfcord/api/events.py` & `selfcord.py-0.1.0/selfcord/api/events.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,10 +191,7 @@
 
 
 
 
 
 
 
-
-
-
```

### Comparing `selfcord.py-0.0.9/selfcord/api/gateway.py` & `selfcord.py-0.1.0/selfcord/api/gateway.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,19 +9,20 @@
 from selfcord.models.client import Client
 import requests
 from traceback import format_exception
 
 class Activity:
 
     @staticmethod
-    def Game(name, details: str="", state: str="", buttons: dict={}, application_id: str="1037788701318729799", key: str = "dolphine"):
+    def Game(name, details: str, state: str, buttons: dict, application_id: str, key: str):
         type = 0
         button_urls = [button for button in buttons.values()]
         buttons: list = [button for button in buttons.keys()]
         req = requests.get(f"https://discordapp.com/api/oauth2/applications/{application_id}/assets")
+        print(req.json())
         for item in req.json():
 
             if item['name'] == key:
                 key = item['id']
 
         if len(button_urls) == 0 or len(buttons) == 0:
             payload = {
@@ -52,15 +53,15 @@
                 "created_at": int(time.time())
             }
 
 
         return payload
 
     @staticmethod
-    def Stream(name, details: str="", state: str="", url: str="https://www.youtube.com/watch?v=CyIrJVp-sH8",buttons: dict={}, application_id: str="1037788701318729799", key: str = "dolphine"):
+    def Stream(name, details: str, state: str, url: str, buttons: dict, application_id: str, key: str):
         type = 1
         button_urls = [button for button in buttons.values()]
         buttons: list = [button for button in buttons.keys()]
         req = requests.get(f"https://discordapp.com/api/oauth2/applications/{application_id}/assets")
         for item in req.json():
 
             if item['name'] == key:
@@ -96,15 +97,15 @@
                 },
                 "created_at": int(time.time())
             }
 
         return payload
 
     @staticmethod
-    def Listen(name, details: str="", state: str="", buttons: dict={}, application_id: str="1037788701318729799", key: str = "dolphine"):
+    def Listen(name, details: str, state: str, buttons: dict, application_id: str, key: str ):
         type = 2
         button_urls = [button for button in buttons.values()]
         buttons: list = [button for button in buttons.keys()]
         req = requests.get(f"https://discordapp.com/api/oauth2/applications/{application_id}/assets")
         for item in req.json():
 
             if item['name'] == key:
@@ -138,15 +139,15 @@
                 },
                 "created_at": int(time.time())
             }
 
 
         return payload
     @staticmethod
-    def Watch(name, details: str="", state: str="", buttons: dict={}, application_id: str="1037788701318729799", key: str = "dolphine"):
+    def Watch(name, details: str, state: str, buttons: dict, application_id: str, key: str ):
         type = 3
 
         button_urls = [button for button in buttons.values()]
         buttons: list = [button for button in buttons.keys()]
 
         req = requests.get(f"https://discordapp.com/api/oauth2/applications/{application_id}/assets")
         for item in req.json():
@@ -252,14 +253,15 @@
                 await self.heartbeat_ack()
 
             elif op == self.DISPATCH:
                 # If op is 0 it signifies a regular gateway event
                 # These events are discord events like message_create, role_create whatever.
 
                 handle = f'handle_{event.lower()}'
+            
 
                 if hasattr(self.handler, handle): # If the event handler exists, so e.g handle_ready
                     method = getattr(self.handler,handle)
 
                     val = await asyncio.gather(asyncio.create_task(method(data, self.user, self.http)), return_exceptions=True) # A background task is created to run the handler
                     for item in val:
                         if item == None: break
@@ -277,15 +279,15 @@
         for i in range(0, len(lst), 1):
             if len(lst[:i+1]) > 3:
                 for i in range(i, len(lst), n): yield lst[i:i + n]
                 break
 
             yield lst[:i+1]
 
-    async def change_presence(self, status: str, afk: bool=False, activity: dict= Activity.Game("Selfcord", "Greatest wrapper" )):
+    async def change_presence(self, status: str, afk: bool, activity: dict):
         """Change the clients current presence
 
         Args:
             status (str): online, offline or dnd
             afk (bool): Whether client is set as AFK
             activity (Activity): Activity object
         """
@@ -413,15 +415,15 @@
         while self.alive:
             try: await self.recv_msg()
             except KeyboardInterrupt:
                 await aprint('Shutting down...')
                 await self.close()
             except Exception as e:
                 error = "".join(format_exception(e, e, e.__traceback__))
-                self.bot.emit("error", error)
+                await self.bot.emit("error", error)
                 await self.close()
 
     async def ring(self, channel, guild=None):
         payload = {
             "op": 4,
             "d": {
                 "guild_id": guild,
```

### Comparing `selfcord.py-0.0.9/selfcord/api/http.py` & `selfcord.py-0.1.0/selfcord/api/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,14 +102,15 @@
                     elif resp.status == 401:
                         json = await resp.json()
                         raise LoginFailure(json, resp.status)
 
                     elif resp.status == 403:
                         json = await resp.json()
                         await aprint(json)
+                        break
 
                     elif resp.status == 201:
                         data = await resp.json()
                         break
 
                     elif resp.status == 204:
                         data = await resp.text()
@@ -135,15 +136,18 @@
                 self.cookies['dcf'] = self.cookies.get('dcf') if dcf != "" else ""
                 self.cookies['sdc'] = self.cookies.get('sdc') if sdc != "" else ""
                 self.cookies['cfr'] = self.cookies.get('cfr') if cfr != "" else ""
                 self.cookies['bm'] = self.cookies.get('bm') if bm != "" else ""
                 self.cookie = set(self.cookies)
         except: pass
 
-        return data
+        try:
+            return data
+        except:
+            return None
 
     async def encode_image(self, url):
         async with ClientSession() as session:
             async with session.get(f'{url}') as resp:
                 image = b64encode(await resp.read())
                 newobj = str(image).split('"', 2)
```

### Comparing `selfcord.py-0.0.9/selfcord/bot.py` & `selfcord.py-0.1.0/selfcord/bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,33 +135,36 @@
                     return result
 
                 return wrapper
 
         return decorator
 
     async def emit(self, event, *args, **kwargs):
-        """Used to essentially push values to the decorator
+        """Used to essentially push values to the decorator when the event fires
 
         Args:
             event (str): The event name
         """
         on_event = "on_{}".format(event)
+
         # try:
         if hasattr(self, on_event):
             await getattr(self, on_event)(*args, **kwargs)
         if event in self._events.keys():
+
             for Event in self._events[event]:
-                # print(Event.coro, Event.name, Event.ext)
+
                 if Event.coro.__code__.co_varnames[0] == "self":
+
                     return asyncio.create_task(Event.coro(Event.ext, *args, **kwargs))
 
                 else:
-                    return asyncio.create_task(Event.coro(*args, **kwargs))
-        # except Exception as e:
-        #     raise RuntimeError("Failure to emit", e)
+
+                    asyncio.create_task(Event.coro(*args, **kwargs))
+
 
     def cmd(self, description="", aliases=[]):
         """Decorator to add commands for the bot
 
         Args:
             description (str, optional): Description of command. Defaults to "".
             aliases (list, optional): Alternative names for command. Defaults to [].
@@ -239,26 +242,27 @@
         except Exception as e:
             raise ModuleNotFoundError(f"Spec could not be loaded {e}")
         try:
             ext = getattr(lib, 'Ext')
         except Exception as e:
             raise ModuleNotFoundError(f"Extension does not exist {e}")
         ext = Extension(name=ext.name, description=ext.description, ext=ext(self), _events=ext._events)
-
+        self.extensions.add(ext)
         try:
             for name, event in ext._events.items():
-                for Event in event:
-                    # print(Event.ext, Event.coro)
-                    self._events[event].append(Event(name=name, coro=Event.coro, ext=Event.ext))
+                for ext_event in event:
+                    self._events[name].append(Event(name=name, coro=ext_event.coro, ext=ext_event.ext))
+
+
 
         except Exception as e:
             error = "".join(format_exception(e, e, e.__traceback__))
             print(error)
 
-        self.extensions.add(ext)
+
 
 
 
 
 
 
 
@@ -379,12 +383,12 @@
         if house.lower() == "bravery":
             await self.http.request(method="post", endpoint = "/hypesquad/online", json = {"house_id": 1})
         if house.lower() == "brilliance":
             await self.http.request(method="post", endpoint = "/hypesquad/online", json = {"house_id": 2})
         if house.lower() == "balance":
             await self.http.request(method="post", endpoint = "/hypesquad/online", json = {"house_id": 3})
 
-    async def change_presence(self, status: str, afk: bool=False, activity: dict=Activity.Game("test", "testing")):
+    async def change_presence(self, status: str, afk: bool, activity: dict):
         await self.gateway.change_presence(status, afk, activity=activity)
```

### Comparing `selfcord.py-0.0.9/selfcord/models/channel.py` & `selfcord.py-0.1.0/selfcord/models/channel.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,14 +61,23 @@
         if amount != None:
             for i in range(0, len(msgs[:amount]), 3):
                 await asyncio.gather(*(asyncio.create_task(message.delete()) for message in msgs[:amount][i:i + 3]))
         else:
             for i in range(0, len(msgs), 3):
                 await asyncio.gather(*(asyncio.create_task(message.delete()) for message in msgs[i:i + 3]))
 
+#            for i in range(0, len(msgs[:amount]), 2):
+#                await asyncio.gather(*(asyncio.create_task(message.delete()) for message in msgs[:amount][i:i + 2]))
+#                await asyncio.sleep(0.2)
+#        else:
+#            for i in range(0, len(msgs), 2):
+#                await asyncio.gather(*(asyncio.create_task(message.delete()) for message in msgs[i:i + 2]))
+#                await asyncio.sleep(0.2)
+             
+
 
     async def spam(self, amount: int, content: str, tts=False):
         """
         Send multiple of the same message.
 
         Args:
             - amount(int) : Number of spam messages to send.
```

### Comparing `selfcord.py-0.0.9/selfcord/models/client.py` & `selfcord.py-0.1.0/selfcord/models/client.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.0.9/selfcord/models/emoji.py` & `selfcord.py-0.1.0/selfcord/models/emoji.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.0.9/selfcord/models/guild.py` & `selfcord.py-0.1.0/selfcord/models/guild.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.0.9/selfcord/models/member.py` & `selfcord.py-0.1.0/selfcord/models/member.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.0.9/selfcord/models/message.py` & `selfcord.py-0.1.0/selfcord/models/message.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.0.9/selfcord/models/permission.py` & `selfcord.py-0.1.0/selfcord/models/permission.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.0.9/selfcord/models/role.py` & `selfcord.py-0.1.0/selfcord/models/role.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.0.9/selfcord/models/user.py` & `selfcord.py-0.1.0/selfcord/models/user.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,9 +87,12 @@
 
 
     async def create_dm(self):
         await self.http.request(method="post", endpoint="/users/@me/channels", json={"recipients": [self.id]})
 
     async def get_profile(self):
         data = await self.http.request(method="get", endpoint=f"/users/{self.id}/profile?with_mutual_guilds=true")
-        data = Profile(data, self.bot, self.http)
+
+        if data != None:
+            data = Profile(data, self.bot, self.http)
+
         return data
```

### Comparing `selfcord.py-0.0.9/selfcord/models/webhook.py` & `selfcord.py-0.1.0/selfcord/models/webhook.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.0.9/selfcord/utils/command.py` & `selfcord.py-0.1.0/selfcord/utils/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,25 @@
 class Extension:
     """Extension object pretty much
     """
     def __init__(self, **kwargs):
         self.name: str | None = kwargs.get("name")
         self.description: str | None = kwargs.get('description')
         self.ext = kwargs.get("ext")
-        self._events = kwargs.get("_events")
+        self._events = defaultdict(list)
+        _events = self.ext._events
         commands = self.ext.commands
         self.commands = CommandCollection()
         for cmd in commands.recents():
             setattr(cmd, "ext", self.ext)
             self.commands.add(cmd)
         self.commands.copy()
+        commands.clear()
+        self._events.update(_events)
+        _events.clear()
 
 
 
 
 class ExtensionCollection:
     """Extension collection, where extensions are stored into
     """
@@ -35,15 +39,15 @@
     def _is_already_registered(self, ext):
         for extension in self.extensions.values():
             if ext.name == extension:
                 return True
 
     def add(self, ext):
         if not isinstance(ext, Extension):
-            raise ValueError('cmd must be a subclass of Command')
+            raise ValueError('cmd must be a subclass of Extension')
         if self._is_already_registered(ext):
             raise ValueError('A name or alias is already registered')
         self.extensions[ext.name] = ext
 
     def get(self, alias, prefix=''):
         try:
             return self.extensions[alias]
@@ -102,15 +106,18 @@
 
     def recents(self):
         for cmd in self.recent_commands.values():
             yield cmd
 
     def copy(self):
         self.commands.update(self.recent_commands)
-        self.recent_commands = {}
+        self.clear()
+
+    def clear(self):
+        self.recent_commands.clear()
 
     def get(self, alias, prefix=''):
         try:
             return self.commands[alias]
         except KeyError:
             pass
         for command in self.commands:
@@ -151,14 +158,15 @@
         def decorator(coro):
             name = coro.__name__
             if not inspect.iscoroutinefunction(coro):
                 raise RuntimeWarning("Not an async function!")
             else:
                 cmd = Command(name=name, description=description, aliases=aliases, func=coro)
                 cls.commands.add(cmd)
+
             return cmd
 
         return decorator
 
     @classmethod
     def on(cls, event: str):
         """Decorator for events
```

### Comparing `selfcord.py-0.0.9/selfcord.py.egg-info/PKG-INFO` & `selfcord.py-0.1.0/selfcord.py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selfcord.py
-Version: 0.0.9
+Version: 0.1.0
 Summary: A Discord API wrapper designed for selfbots!
 Home-page: https://github.com/Shell1010/Selfcord
 Author: Shell of OMEGA
 License: MIT
 Keywords: selfbot,discord,discordapi,discordwrapper
 Description-Content-Type: text/markdown
 
@@ -90,8 +90,8 @@
     await ctx.reply(f"{bot.user.deleted_messages[-1].author}: {bot.user.deleted_messages[-1]}")
 
 bot.run(token)
 ```
 
 ## Help & Support
 
-Please join our [discord server](https://discord.gg/W5QMKHejQB) here.
+Please join our [discord server](https://discord.gg/FCFnnBGzkg) here.
```

### Comparing `selfcord.py-0.0.9/selfcord.py.egg-info/SOURCES.txt` & `selfcord.py-0.1.0/selfcord.py.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -20,8 +20,9 @@
 selfcord/models/member.py
 selfcord/models/message.py
 selfcord/models/permission.py
 selfcord/models/role.py
 selfcord/models/user.py
 selfcord/models/webhook.py
 selfcord/utils/__init__.py
-selfcord/utils/command.py
+selfcord/utils/command.py
+tests/test_commands.py
```

### Comparing `selfcord.py-0.0.9/setup.py` & `selfcord.py-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 this_directory = Path(__file__).parent
 if __name__ == "__main__":
     this_directory = Path(__file__).parent
     long_description = ( this_directory /"README.md").read_text()
     setup(
         name="selfcord.py",
         packages=find_packages(include=['selfcord', 'selfcord.api', 'selfcord.utils', 'selfcord.models']),
-        version="0.0.9",
+        version="0.1.0",
         description="A Discord API wrapper designed for selfbots!",
         readme="README.md",
         author="Shell of OMEGA",
         license="MIT",
         install_requires=["aiohttp==3.7.4.post0","aioconsole==0.3.3", "websockets==10.1", "importlib", "requests"],
         setup_requires=['pytest-runner'],
         tests_require=['pytest'],
```

