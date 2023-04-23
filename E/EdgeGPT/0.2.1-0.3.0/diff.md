# Comparing `tmp/EdgeGPT-0.2.1.tar.gz` & `tmp/EdgeGPT-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EdgeGPT-0.2.1.tar", last modified: Thu Apr 20 00:36:06 2023, max compression
+gzip compressed data, was "EdgeGPT-0.3.0.tar", last modified: Sun Apr 23 16:47:14 2023, max compression
```

## Comparing `EdgeGPT-0.2.1.tar` & `EdgeGPT-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:36:06.431137 EdgeGPT-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-20 00:35:38.000000 EdgeGPT-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-04-20 00:36:06.431137 EdgeGPT-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7398 2023-04-20 00:36:06.000000 EdgeGPT-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-20 00:36:06.431137 EdgeGPT-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-20 00:35:38.000000 EdgeGPT-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:36:06.431137 EdgeGPT-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:36:06.431137 EdgeGPT-0.2.1/src/EdgeGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-04-20 00:36:06.000000 EdgeGPT-0.2.1/src/EdgeGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-20 00:36:06.000000 EdgeGPT-0.2.1/src/EdgeGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 00:36:06.000000 EdgeGPT-0.2.1/src/EdgeGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-20 00:36:06.000000 EdgeGPT-0.2.1/src/EdgeGPT.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-20 00:36:06.000000 EdgeGPT-0.2.1/src/EdgeGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-20 00:36:06.000000 EdgeGPT-0.2.1/src/EdgeGPT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    18768 2023-04-20 00:35:38.000000 EdgeGPT-0.2.1/src/EdgeGPT.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-20 00:35:38.000000 EdgeGPT-0.2.1/src/ImageGen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:47:14.008706 EdgeGPT-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-23 16:46:44.000000 EdgeGPT-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-04-23 16:47:14.008706 EdgeGPT-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7398 2023-04-23 16:47:13.000000 EdgeGPT-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-23 16:47:14.008706 EdgeGPT-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-23 16:46:44.000000 EdgeGPT-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:47:14.004706 EdgeGPT-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:47:14.008706 EdgeGPT-0.3.0/src/EdgeGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-04-23 16:47:13.000000 EdgeGPT-0.3.0/src/EdgeGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-23 16:47:14.000000 EdgeGPT-0.3.0/src/EdgeGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 16:47:13.000000 EdgeGPT-0.3.0/src/EdgeGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-23 16:47:13.000000 EdgeGPT-0.3.0/src/EdgeGPT.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-23 16:47:13.000000 EdgeGPT-0.3.0/src/EdgeGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-23 16:47:13.000000 EdgeGPT-0.3.0/src/EdgeGPT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    21858 2023-04-23 16:46:44.000000 EdgeGPT-0.3.0/src/EdgeGPT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-23 16:46:44.000000 EdgeGPT-0.3.0/src/ImageGen.py
```

### Comparing `EdgeGPT-0.2.1/LICENSE` & `EdgeGPT-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.2.1/PKG-INFO` & `EdgeGPT-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.2.1
+Version: 0.3.0
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.2.1 Summary: Reverse engineered
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.3.0 Summary: Reverse engineered
 Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
 Cheong Author-email: acheong@student.dalat.org License: GNU General Public
 License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
 issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `EdgeGPT-0.2.1/README.md` & `EdgeGPT-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.2.1/setup.py` & `EdgeGPT-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="EdgeGPT",
-    version="0.2.1",
+    version="0.3.0",
     license="GNU General Public License v2.0",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="Reverse engineered Edge Chat API",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/EdgeGPT",
```

### Comparing `EdgeGPT-0.2.1/src/EdgeGPT.egg-info/PKG-INFO` & `EdgeGPT-0.3.0/src/EdgeGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.2.1
+Version: 0.3.0
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.2.1 Summary: Reverse engineered
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.3.0 Summary: Reverse engineered
 Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
 Cheong Author-email: acheong@student.dalat.org License: GNU General Public
 License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
 issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `EdgeGPT-0.2.1/src/EdgeGPT.py` & `EdgeGPT-0.3.0/src/EdgeGPT.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import uuid
 from enum import Enum
 from pathlib import Path
 from typing import Generator
 from typing import Literal
 from typing import Optional
 from typing import Union
-
+from BingImageCreator import ImageGenAsync
 import certifi
 import httpx
 import websockets.client as websockets
 from prompt_toolkit import PromptSession
 from prompt_toolkit.auto_suggest import AutoSuggestFromHistory
 from prompt_toolkit.completion import WordCompleter
 from prompt_toolkit.history import InMemoryHistory
@@ -90,17 +90,54 @@
 
 
 class NotAllowedToAccess(Exception):
     pass
 
 
 class ConversationStyle(Enum):
-    creative = "h3imaginative,clgalileo,gencontentv3"
-    balanced = "galileo"
-    precise = "h3precise,clgalileo"
+    creative = [
+                "nlu_direct_response_filter",
+                "deepleo",
+                "disable_emoji_spoken_text",
+                "responsible_ai_policy_235",
+                "enablemm",
+                "h3imaginative","travelansgnd","dv3sugg","clgalileo","gencontentv3",
+                "dv3sugg",
+                "responseos",
+                "e2ecachewrite",
+                "cachewriteext",
+                "nodlcpcwrite",
+                "travelansgnd"
+            ]
+    balanced = [
+                "nlu_direct_response_filter",
+                "deepleo",
+                "disable_emoji_spoken_text",
+                "responsible_ai_policy_235",
+                "enablemm",
+                "galileo",
+                "dv3sugg",
+                "responseos",
+                "e2ecachewrite",
+                "cachewriteext",
+                "nodlcpcwrite",
+                "travelansgnd"
+            ]
+    precise = ["nlu_direct_response_filter",
+                "deepleo",
+                "disable_emoji_spoken_text",
+                "responsible_ai_policy_235",
+                "enablemm",
+                "galileo",
+                "dv3sugg",
+                "responseos",
+                "e2ecachewrite",
+                "cachewriteext",
+                "nodlcpcwrite",
+                "travelansgnd","h3precise","clgalileo"]
 
 
 CONVERSATION_STYLE_TYPE = Optional[
     Union[ConversationStyle, Literal["creative", "balanced", "precise"]]
 ]
 
 
@@ -153,35 +190,51 @@
                 "enable_debug_commands",
                 "disable_emoji_spoken_text",
                 "enablemm",
             ]
         if conversation_style:
             if not isinstance(conversation_style, ConversationStyle):
                 conversation_style = getattr(ConversationStyle, conversation_style)
-            options = [
-                "nlu_direct_response_filter",
-                "deepleo",
-                "disable_emoji_spoken_text",
-                "responsible_ai_policy_235",
-                "enablemm",
-                conversation_style.value,
-                "dtappid",
-                "cricinfo",
-                "cricinfov2",
-                "dv3sugg",
-            ]
+            options = conversation_style.value
         self.struct = {
             "arguments": [
                 {
                     "source": "cib",
                     "optionsSets": options,
+                    "allowedMessageTypes": [
+                        "Chat",
+                        "InternalSearchQuery",
+                        "InternalSearchResult",
+                        "Disengaged",
+                        "InternalLoaderMessage",
+                        "RenderCardRequest",
+                        "AdsQuery",
+                        "SemanticSerp",
+                        "GenerateContentQuery",
+                        "SearchQuery"
+                    ],
                     "sliceIds": [
-                        "222dtappid",
-                        "225cricinfo",
-                        "224locals0",
+                        "chk1cf",
+                        "nopreloadsscf",
+                        "winlongmsg2tf",
+                        "perfimpcomb",
+                        "sugdivdis",
+                        "sydnoinputt",
+                        "wpcssopt",
+                        "wintone2tf",
+                        "0404sydicnbs0",
+                        "405suggbs0",
+                        "scctl",
+                        "330uaugs0",
+                        "0329resp",
+                        "udscahrfon",
+                        "udstrblm5",
+                        "404e2ewrt",
+                        "408nodedups0",
+                        "403tvlansgnd"
                     ],
                     "traceId": _get_ran_hex(32),
                     "isStartOfSession": self.invocation_id == 0,
                     "message": {
                         "author": "user",
                         "inputMethod": "Keyboard",
                         "text": prompt,
@@ -276,14 +329,15 @@
             conversation_id=conversation.struct["conversationId"],
         )
 
     async def ask_stream(
         self,
         prompt: str,
         wss_link: str,
+        cookies: str,
         conversation_style: CONVERSATION_STYLE_TYPE = None,
         raw: bool = False,
         options: dict = None,
     ) -> Generator[str, None, None]:
         """
         Ask a question to the bot
         """
@@ -302,30 +356,46 @@
             prompt=prompt,
             conversation_style=conversation_style,
             options=options,
         )
         # Send request
         await self.wss.send(_append_identifier(self.request.struct))
         final = False
+        draw = False
         while not final:
             objects = str(await self.wss.recv()).split(DELIMITER)
             for obj in objects:
                 if obj is None or not obj:
                     continue
                 response = json.loads(obj)
                 if response.get("type") != 2 and raw:
                     yield False, response
                 elif response.get("type") == 1 and response["arguments"][0].get(
                     "messages",
                 ):
-                    resp_txt = response["arguments"][0]["messages"][0]["adaptiveCards"][
-                        0
-                    ]["body"][0].get("text")
-                    yield False, resp_txt
+                    try:
+                        if not draw:
+                            resp_txt = response["arguments"][0]["messages"][0]["adaptiveCards"][
+                                0
+                            ]["body"][0].get("text")
+                        yield False, resp_txt
+                    except:
+                        draw = True
+                        for item in cookies:
+                            if(item["name"] == "_U"):
+                                U = item["value"]
+                        async with ImageGenAsync(U, True) as image_generator:
+                            images = await image_generator.get_images(response["arguments"][0]["messages"][0]["text"])
+                        cache = resp_txt
+                        resp_txt = cache+"\n![image0]("+images[0]+")\n![image1]("+images[1]+")\n![image0]("+images[2]+")\n![image3]("+images[3]+")"
+                        yield False, resp_txt
                 elif response.get("type") == 2:
+                    if draw:
+                        cache = response["item"]["messages"][1]["adaptiveCards"][0]["body"][0]["text"]
+                        response["item"]["messages"][1]["adaptiveCards"][0]["body"][0]["text"] = cache+resp_txt
                     final = True
                     yield True, response
 
     async def _initial_handshake(self) -> None:
         await self.wss.send(_append_identifier({"protocol": "json", "version": 1}))
         await self.wss.recv()
 
@@ -374,14 +444,15 @@
         Ask a question to the bot
         """
         async for final, response in self.chat_hub.ask_stream(
             prompt=prompt,
             conversation_style=conversation_style,
             wss_link=wss_link,
             options=options,
+            cookies=self.cookies
         ):
             if final:
                 return response
         await self.chat_hub.wss.close()
         return None
 
     async def ask_stream(
@@ -397,14 +468,15 @@
         """
         async for response in self.chat_hub.ask_stream(
             prompt=prompt,
             conversation_style=conversation_style,
             wss_link=wss_link,
             raw=raw,
             options=options,
+            cookies=self.cookies
         ):
             yield response
 
     async def close(self) -> None:
         """
         Close the connection
         """
```

