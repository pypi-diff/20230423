# Comparing `tmp/megabot-0.0.4.tar.gz` & `tmp/megabot-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "megabot-0.0.4.tar", last modified: Thu Apr  6 06:57:25 2023, max compression
+gzip compressed data, was "megabot-0.0.5.tar", last modified: Sun Apr 23 07:50:56 2023, max compression
```

## Comparing `megabot-0.0.4.tar` & `megabot-0.0.5.tar`

### file list

```diff
@@ -1,36 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 06:57:25.130119 megabot-0.0.4/
--rw-rw-rw-   0        0        0     1094 2023-04-03 06:41:39.000000 megabot-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     3275 2023-04-06 06:57:25.131123 megabot-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2391 2023-04-05 10:57:01.000000 megabot-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-06 06:57:25.064118 megabot-0.0.4/megabot/
--rw-rw-rw-   0        0        0       69 2023-04-03 09:14:42.000000 megabot-0.0.4/megabot/__init__.py
--rw-rw-rw-   0        0        0     4342 2023-04-03 06:16:26.000000 megabot-0.0.4/megabot/dispatcher.py
-drwxrwxrwx   0        0        0        0 2023-04-06 06:57:25.124120 megabot-0.0.4/megabot/models/
--rw-rw-rw-   0        0        0      411 2023-04-03 06:16:34.000000 megabot-0.0.4/megabot/models/__init__.py
--rw-rw-rw-   0        0        0      850 2023-04-03 08:40:51.000000 megabot-0.0.4/megabot/models/base.py
--rw-rw-rw-   0        0        0      610 2023-04-03 08:40:51.000000 megabot-0.0.4/megabot/models/callback.py
--rw-rw-rw-   0        0        0     2728 2023-04-03 06:16:34.000000 megabot-0.0.4/megabot/models/chats.py
--rw-rw-rw-   0        0        0       99 2023-04-03 06:19:35.000000 megabot-0.0.4/megabot/models/emodj.py
--rw-rw-rw-   0        0        0      503 2023-04-03 06:19:35.000000 megabot-0.0.4/megabot/models/forum.py
--rw-rw-rw-   0        0        0      369 2023-04-03 06:19:35.000000 megabot-0.0.4/megabot/models/game.py
--rw-rw-rw-   0        0        0     2236 2023-04-03 06:16:34.000000 megabot-0.0.4/megabot/models/keyboards.py
--rw-rw-rw-   0        0        0     1583 2023-04-03 06:19:35.000000 megabot-0.0.4/megabot/models/media.py
--rw-rw-rw-   0        0        0     5124 2023-04-03 06:19:35.000000 megabot-0.0.4/megabot/models/message.py
--rw-rw-rw-   0        0        0      794 2023-04-03 06:19:36.000000 megabot-0.0.4/megabot/models/payment.py
--rw-rw-rw-   0        0        0      639 2023-04-03 06:19:35.000000 megabot-0.0.4/megabot/models/poll.py
--rw-rw-rw-   0        0        0      655 2023-04-03 06:19:35.000000 megabot-0.0.4/megabot/models/sticker.py
--rw-rw-rw-   0        0        0     1523 2023-04-03 06:19:35.000000 megabot-0.0.4/megabot/models/users.py
--rw-rw-rw-   0        0        0      374 2023-04-03 06:19:35.000000 megabot-0.0.4/megabot/models/video.py
--rw-rw-rw-   0        0        0      104 2023-04-03 06:19:35.000000 megabot-0.0.4/megabot/models/web_app.py
--rw-rw-rw-   0        0        0     2734 2023-04-03 06:16:26.000000 megabot-0.0.4/megabot/poster.py
-drwxrwxrwx   0        0        0        0 2023-04-06 06:57:25.128119 megabot-0.0.4/megabot/utils/
--rw-rw-rw-   0        0        0       41 2023-04-03 09:14:42.000000 megabot-0.0.4/megabot/utils/__init__.py
--rw-rw-rw-   0        0        0     1299 2023-03-31 11:42:03.000000 megabot-0.0.4/megabot/utils/callback_data.py
-drwxrwxrwx   0        0        0        0 2023-04-06 06:57:25.091117 megabot-0.0.4/megabot.egg-info/
--rw-rw-rw-   0        0        0     3275 2023-04-06 06:57:24.000000 megabot-0.0.4/megabot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      706 2023-04-06 06:57:24.000000 megabot-0.0.4/megabot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 06:57:24.000000 megabot-0.0.4/megabot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-04-06 06:57:24.000000 megabot-0.0.4/megabot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-06 06:57:24.000000 megabot-0.0.4/megabot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       80 2023-04-06 06:57:25.133118 megabot-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1206 2023-04-06 06:57:00.000000 megabot-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 07:50:56.583901 megabot-0.0.5/
+-rw-rw-rw-   0        0        0     1094 2023-04-03 06:41:39.000000 megabot-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     3258 2023-04-23 07:50:56.583901 megabot-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2391 2023-04-05 10:57:01.000000 megabot-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 07:50:56.501878 megabot-0.0.5/megabot/
+-rw-rw-rw-   0        0        0       82 2023-04-23 07:30:07.000000 megabot-0.0.5/megabot/__init__.py
+-rw-rw-rw-   0        0        0      418 2023-04-23 07:30:07.000000 megabot-0.0.5/megabot/command.py
+-rw-rw-rw-   0        0        0     4479 2023-04-23 07:30:07.000000 megabot-0.0.5/megabot/dispatcher.py
+drwxrwxrwx   0        0        0        0 2023-04-23 07:50:56.576892 megabot-0.0.5/megabot/models/
+-rw-rw-rw-   0        0        0      529 2023-04-23 07:30:07.000000 megabot-0.0.5/megabot/models/__init__.py
+-rw-rw-rw-   0        0        0     1035 2023-04-23 07:30:07.000000 megabot-0.0.5/megabot/models/base.py
+-rw-rw-rw-   0        0        0      610 2023-04-23 07:30:02.000000 megabot-0.0.5/megabot/models/callback.py
+-rw-rw-rw-   0        0        0     2730 2023-04-23 07:30:02.000000 megabot-0.0.5/megabot/models/chats.py
+-rw-rw-rw-   0        0        0      287 2023-04-23 07:30:07.000000 megabot-0.0.5/megabot/models/command.py
+-rw-rw-rw-   0        0        0       99 2023-04-23 07:30:07.000000 megabot-0.0.5/megabot/models/emodj.py
+-rw-rw-rw-   0        0        0      386 2023-04-23 07:30:02.000000 megabot-0.0.5/megabot/models/file.py
+-rw-rw-rw-   0        0        0      503 2023-04-23 07:30:07.000000 megabot-0.0.5/megabot/models/forum.py
+-rw-rw-rw-   0        0        0      371 2023-04-23 07:30:07.000000 megabot-0.0.5/megabot/models/game.py
+-rw-rw-rw-   0        0        0     2240 2023-04-23 07:30:02.000000 megabot-0.0.5/megabot/models/keyboards.py
+-rw-rw-rw-   0        0        0     1583 2023-04-23 07:30:07.000000 megabot-0.0.5/megabot/models/media.py
+-rw-rw-rw-   0        0        0     5399 2023-04-23 07:30:07.000000 megabot-0.0.5/megabot/models/message.py
+-rw-rw-rw-   0        0        0      794 2023-04-23 07:30:07.000000 megabot-0.0.5/megabot/models/payment.py
+-rw-rw-rw-   0        0        0      826 2023-04-23 07:30:02.000000 megabot-0.0.5/megabot/models/photo.py
+-rw-rw-rw-   0        0        0      641 2023-04-23 07:30:07.000000 megabot-0.0.5/megabot/models/poll.py
+-rw-rw-rw-   0        0        0      655 2023-04-23 07:30:02.000000 megabot-0.0.5/megabot/models/sticker.py
+-rw-rw-rw-   0        0        0     1523 2023-04-23 07:30:07.000000 megabot-0.0.5/megabot/models/users.py
+-rw-rw-rw-   0        0        0      374 2023-04-23 07:30:07.000000 megabot-0.0.5/megabot/models/video.py
+-rw-rw-rw-   0        0        0      104 2023-04-23 07:30:07.000000 megabot-0.0.5/megabot/models/web_app.py
+-rw-rw-rw-   0        0        0     5224 2023-04-23 07:30:07.000000 megabot-0.0.5/megabot/sender.py
+drwxrwxrwx   0        0        0        0 2023-04-23 07:50:56.581877 megabot-0.0.5/megabot/utils/
+-rw-rw-rw-   0        0        0       41 2023-04-23 07:30:07.000000 megabot-0.0.5/megabot/utils/__init__.py
+-rw-rw-rw-   0        0        0     1300 2023-04-23 07:30:07.000000 megabot-0.0.5/megabot/utils/callback_data.py
+drwxrwxrwx   0        0        0        0 2023-04-23 07:50:56.533898 megabot-0.0.5/megabot.egg-info/
+-rw-rw-rw-   0        0        0     3258 2023-04-23 07:50:56.000000 megabot-0.0.5/megabot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      813 2023-04-23 07:50:56.000000 megabot-0.0.5/megabot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 07:50:56.000000 megabot-0.0.5/megabot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-04-23 07:50:56.000000 megabot-0.0.5/megabot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-23 07:50:56.000000 megabot-0.0.5/megabot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       67 2023-04-12 15:12:33.000000 megabot-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       80 2023-04-23 07:50:56.586893 megabot-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1198 2023-04-23 07:50:16.000000 megabot-0.0.5/setup.py
```

### Comparing `megabot-0.0.4/LICENSE` & `megabot-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `megabot-0.0.4/PKG-INFO` & `megabot-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: megabot
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python telegram API adapter for FastAPI and asyncio
 Home-page: https://github.com/imoknot/megabot
 Author: Aleksandr Koksharov
 Author-email: koksharov@yandex.ru
 License: MIT
 Project-URL: Bug Tracker, https://github.com/imoknot/megabot/issues
 Project-URL: Changelog, https://github.com/imoknot/megabot/blob/master/CHANGELOG.md
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10
@@ -100,8 +99,7 @@
             await asyncio.sleep(1)
     
     
     await def start_bot()
         asyncio.create_task(check_updates())
 
 add start_bot() to main file web_hooks 
-
```

### Comparing `megabot-0.0.4/README.md` & `megabot-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `megabot-0.0.4/megabot/dispatcher.py` & `megabot-0.0.5/megabot/dispatcher.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from typing import NoReturn
 from dataclasses import dataclass
+from typing import NoReturn
+
 from .models import CallbackQuery, Message
 
 
 @dataclass
 class Handler:
     handler: callable
 
@@ -94,11 +95,12 @@
                 if entities:
                     if entities[0]['type'] == 'bot_command':
                         command = message['text'][1:]
                         msg = command.split(' ')
                         current_handler = cls.handlers_command.get(msg[0], None)
                         if current_handler:
                             message = Message(**message)
-                            await current_handler.handler(bot_id, message, msg[1] if len(msg) == 2 else None)
+                            if len(msg) == 2:
+                                await current_handler.handler(bot_id, message, msg[1])
+                            else:
+                                await current_handler.handler(bot_id, message)
                         continue
-
-
```

### Comparing `megabot-0.0.4/megabot/models/base.py` & `megabot-0.0.5/megabot/models/base.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 
 class ExcludeNone(BaseModel):
     def dict(self, *args, **kwargs):
         if kwargs.get('exclude_none'):
             del kwargs['exclude_none']
         return super().dict(*args, exclude_none=True, **kwargs)
 
+    def json(self, *args, **kwargs):
+        if kwargs.get('exclude_none'):
+            del kwargs['exclude_none']
+        return super().json(*args, exclude_none=True, **kwargs)
+
 
 class Location(ExcludeNone):
     longitude: float
     latitude: float
     horizontal_accuracy: float
     live_period: int | None = None
     heading: int | None = None
```

### Comparing `megabot-0.0.4/megabot/models/callback.py` & `megabot-0.0.5/megabot/models/callback.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pydantic import Field
 
 from .base import ExcludeNone
-from .users import User
 from .message import Message
+from .users import User
 
 
 class CallbackQuery(ExcludeNone):
     id: str
     from_user: User = Field(None, alias='from')
     message: Message | None = None
     inline_message_id: str | None = None
```

### Comparing `megabot-0.0.4/megabot/models/chats.py` & `megabot-0.0.5/megabot/models/chats.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import ForwardRef
+
 from .base import ExcludeNone, Location
 
 Message = ForwardRef('Message')
 
 
 class ChatAdministratorRights(ExcludeNone):
     is_anonymous: bool
```

### Comparing `megabot-0.0.4/megabot/models/keyboards.py` & `megabot-0.0.5/megabot/models/keyboards.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from typing import List, Tuple
+
 from pydantic import Field
+
 from .base import ExcludeNone
 from .chats import ChatAdministratorRights
 
 
 class WebAppInfo(ExcludeNone):
     pass
```

### Comparing `megabot-0.0.4/megabot/models/media.py` & `megabot-0.0.5/megabot/models/media.py`

 * *Files identical despite different names*

### Comparing `megabot-0.0.4/megabot/models/message.py` & `megabot-0.0.5/megabot/models/message.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,36 @@
 from typing import ForwardRef
+
 from pydantic import Field
 
 from .base import ExcludeNone, Location, Venue
 from .chats import Chat, ChatShared
-from .game import Game
 from .emodj import Dice
 from .forum import (
+    ForumTopicClosed,
     ForumTopicCreated,
     ForumTopicEdited,
-    ForumTopicClosed,
     ForumTopicReopened,
     GeneralForumTopicHidden,
-    GeneralForumTopicUnhidden
+    GeneralForumTopicUnhidden,
 )
+from .game import Game
+from .keyboards import ForceReply, InlineKeyboardMarkup, ReplyKeyboardMarkup, ReplyKeyboardRemove
+from .media import Animation, Audio, Document, PhotoSize, Video, VideoNote, Voice
 from .payment import Invoice, SuccessfulPayment
 from .poll import Poll
-from .media import Animation, Audio, Document, PhotoSize, Video, VideoNote, Voice
 from .sticker import Sticker
-from .users import User, Contact, UserShared, PassportData, ProximityAlertTriggered
+from .users import Contact, PassportData, ProximityAlertTriggered, User, UserShared
 from .video import (
+    VideoChatEnded,
+    VideoChatParticipantsInvited,
     VideoChatScheduled,
-    WriteAccessAllowed,
     VideoChatStarted,
-    VideoChatEnded,
-    VideoChatParticipantsInvited
-)
-
-from .keyboards import (
-    ForceReply,
-    InlineKeyboardMarkup,
-    ReplyKeyboardMarkup,
-    ReplyKeyboardRemove,
+    WriteAccessAllowed,
 )
-
 from .web_app import WebAppData
 
 Message = ForwardRef('Message')
 
 
 class MessageAutoDeleteTimerChanged(ExcludeNone):
     message_auto_delete_time: int
@@ -138,7 +132,19 @@
     video_chat_participants_invited: VideoChatParticipantsInvited | None = None
     web_app_data: WebAppData | None = None
     reply_markup: InlineKeyboardMarkup | None = None
 
 
 Message.update_forward_refs()
 MessageEntity.update_forward_refs()
+
+
+class DeleteMessage(ExcludeNone):
+    chat_id: int | str
+    message_id: int
+
+
+class EditMessageReplyMarkup(ExcludeNone):
+    chat_id: int | str | None = None
+    message_id: int | None = None
+    inline_message_id: str | None = None
+    reply_markup: InlineKeyboardMarkup | None = None
```

### Comparing `megabot-0.0.4/megabot/models/payment.py` & `megabot-0.0.5/megabot/models/payment.py`

 * *Files identical despite different names*

### Comparing `megabot-0.0.4/megabot/models/poll.py` & `megabot-0.0.5/megabot/models/poll.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import ForwardRef
+
 from .base import ExcludeNone
 
 MessageEntity = ForwardRef('MessageEntity')
 
 
 class PollOption(ExcludeNone):
     text: str
```

### Comparing `megabot-0.0.4/megabot/models/sticker.py` & `megabot-0.0.5/megabot/models/sticker.py`

 * *Files identical despite different names*

### Comparing `megabot-0.0.4/megabot/models/users.py` & `megabot-0.0.5/megabot/models/users.py`

 * *Files identical despite different names*

### Comparing `megabot-0.0.4/megabot/poster.py` & `megabot-0.0.5/megabot/sender.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,76 +1,137 @@
 import requests
+
 from .models import (
     AnswerCallbackQuery,
+    DeleteMessage,
+    EditMessageReplyMarkup,
     ForceReply,
     InlineKeyboardMarkup,
-    SendMessage,
+    InputFile,
     ReplyKeyboardMarkup,
     ReplyKeyboardRemove,
+    SendMessage,
+    SendPhoto,
 )
 
 
 class Base:
     def request_url(self, token, command):
         return f'https://api.telegram.org/bot{token}/{command}'
 
 
 class MessageService(Base):
+    async def delete_message(self, token: str, chat_id: int | str, message_id: int):
+        message = DeleteMessage(chat_id=chat_id, message_id=message_id).dict()
+        request_url = self.request_url(token, 'deleteMessage')
+        response = requests.post(url=request_url, json=message)
+        return response
+
+    async def edit_message_reply_markup(
+        self,
+        token: str,
+        chat_id: int | str | None = None,
+        message_id: int | None = None,
+        inline_message_id: str | None = None,
+        reply_markup: InlineKeyboardMarkup | None = None,
+    ):
+        message = EditMessageReplyMarkup(
+            chat_id=chat_id, message_id=message_id, inline_message_id=inline_message_id, reply_markup=reply_markup
+        ).dict()
+        request_url = self.request_url(token, 'editMessageReplyMarkup')
+        response = requests.post(url=request_url, json=message)
+        return response
+
     async def callback_answer(
-            self,
-            token: str,
-            callback_query_id: str,
-            text: str | None = None,
-            show_alert: bool | None = None,
-            url: str | None = None,
-            cache_time: str | None = None,
+        self,
+        token: str,
+        callback_query_id: str,
+        text: str | None = None,
+        show_alert: bool | None = None,
+        url: str | None = None,
+        cache_time: str | None = None,
     ):
         message = AnswerCallbackQuery(
-            callback_query_id=callback_query_id,
-            text=text,
-            show_alert=show_alert,
-            url=url,
-            cache_time=cache_time
+            callback_query_id=callback_query_id, text=text, show_alert=show_alert, url=url, cache_time=cache_time
         ).dict()
         request_url = self.request_url(token, 'answerCallbackQuery')
         response = requests.post(url=request_url, json=message)
         return response
 
     async def send_message(
-            self,
-            token: str,
-            chat_id: int,
-            message_thread_id: int | None = None,
-            text: str | None = None,
-            parse_mode: str | None = None,
-            entities: list | None = None,
-            disable_web_page_preview: bool | None = None,
-            disable_notification: bool | None = None,
-            protect_content: bool | None = None,
-            reply_to_message_id: int | None = None,
-            allow_sending_without_reply: bool | None = None,
-            reply_markup: InlineKeyboardMarkup | ReplyKeyboardMarkup | ReplyKeyboardRemove | ForceReply | None = None
+        self,
+        token: str,
+        chat_id: int,
+        message_thread_id: int | None = None,
+        text: str | None = None,
+        parse_mode: str | None = None,
+        entities: list | None = None,
+        disable_web_page_preview: bool | None = None,
+        disable_notification: bool | None = None,
+        protect_content: bool | None = None,
+        reply_to_message_id: int | None = None,
+        allow_sending_without_reply: bool | None = None,
+        reply_markup: InlineKeyboardMarkup | ReplyKeyboardMarkup | ReplyKeyboardRemove | ForceReply | None = None,
     ):
         message = SendMessage(
             chat_id=chat_id,
             message_thread_id=message_thread_id,
             text=text,
             parse_mode=parse_mode,
             entities=entities,
             disable_web_page_preview=disable_web_page_preview,
             disable_notification=disable_notification,
             protect_content=protect_content,
             reply_to_message_id=reply_to_message_id,
             allow_sending_without_reply=allow_sending_without_reply,
-            reply_markup=reply_markup
+            reply_markup=reply_markup,
         ).dict()
         request_url = self.request_url(token, 'sendMessage')
         response = requests.post(url=request_url, json=message)
         return response
 
+    async def send_photo(
+        self,
+        token: str,
+        chat_id: int,
+        photo: str | InputFile,
+        message_thread_id: int | None = None,
+        caption: str | None = None,
+        parse_mode: str | None = None,
+        caption_entities: list | None = None,
+        has_spoiler: bool | None = None,
+        disable_notification: bool | None = None,
+        protect_content: bool | None = None,
+        reply_to_message_id: int | None = None,
+        allow_sending_without_reply: bool | None = None,
+        reply_markup: InlineKeyboardMarkup | ReplyKeyboardMarkup | ReplyKeyboardRemove | ForceReply | None = None,
+    ):
+        message = SendPhoto(
+            chat_id=chat_id,
+            message_thread_id=message_thread_id,
+            caption=caption,
+            parse_mode=parse_mode,
+            caption_entities=caption_entities,
+            has_spoiler=has_spoiler,
+            disable_notification=disable_notification,
+            protect_content=protect_content,
+            reply_to_message_id=reply_to_message_id,
+            allow_sending_without_reply=allow_sending_without_reply,
+        ).dict()
+        if reply_markup:
+            message['reply_markup'] = reply_markup.json()
+
+        request_url = self.request_url(token, 'sendPhoto')
+        if isinstance(photo, str):
+            message['photo'] = photo
+            response = requests.post(url=request_url, data=message)
+        else:
+            response = requests.post(url=request_url, data=message, files={'photo': photo})
+        return response.json()
+
 
 async def get_updates(token: str, offset=0):
     request_url = f'https://api.telegram.org/bot{token}/getUpdates'
     data = {'offset': offset}
     response = requests.post(url=request_url, data=data)
     if response.status_code == 200:
         result = response.json()
```

### Comparing `megabot-0.0.4/megabot/utils/callback_data.py` & `megabot-0.0.5/megabot/utils/callback_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,10 +24,10 @@
 
     def filter(self, **config):
         filter_hash = dict()
         current_filter = self.class_prefix + self.separator
         for key in self._part_names:
             current_filter += str(config.get(key, '')) + self.separator
             filter_hash[key] = str(config.get(key, ''))
-        current_filter = self.separator + current_filter[:len(current_filter) - 1]
+        current_filter = self.separator + current_filter[: len(current_filter) - 1]
 
         return {self.class_prefix: {current_filter: filter_hash}}
```

### Comparing `megabot-0.0.4/megabot.egg-info/PKG-INFO` & `megabot-0.0.5/megabot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: megabot
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python telegram API adapter for FastAPI and asyncio
 Home-page: https://github.com/imoknot/megabot
 Author: Aleksandr Koksharov
 Author-email: koksharov@yandex.ru
 License: MIT
 Project-URL: Bug Tracker, https://github.com/imoknot/megabot/issues
 Project-URL: Changelog, https://github.com/imoknot/megabot/blob/master/CHANGELOG.md
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10
@@ -100,8 +99,7 @@
             await asyncio.sleep(1)
     
     
     await def start_bot()
         asyncio.create_task(check_updates())
 
 add start_bot() to main file web_hooks 
-
```

### Comparing `megabot-0.0.4/megabot.egg-info/SOURCES.txt` & `megabot-0.0.5/megabot.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 LICENSE
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 megabot/__init__.py
+megabot/command.py
 megabot/dispatcher.py
-megabot/poster.py
+megabot/sender.py
 megabot.egg-info/PKG-INFO
 megabot.egg-info/SOURCES.txt
 megabot.egg-info/dependency_links.txt
 megabot.egg-info/requires.txt
 megabot.egg-info/top_level.txt
 megabot/models/__init__.py
 megabot/models/base.py
 megabot/models/callback.py
 megabot/models/chats.py
+megabot/models/command.py
 megabot/models/emodj.py
+megabot/models/file.py
 megabot/models/forum.py
 megabot/models/game.py
 megabot/models/keyboards.py
 megabot/models/media.py
 megabot/models/message.py
 megabot/models/payment.py
+megabot/models/photo.py
 megabot/models/poll.py
 megabot/models/sticker.py
 megabot/models/users.py
 megabot/models/video.py
 megabot/models/web_app.py
 megabot/utils/__init__.py
 megabot/utils/callback_data.py
```

### Comparing `megabot-0.0.4/setup.py` & `megabot-0.0.5/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 import setuptools
 
-with open("README.md", "r") as f:
+with open('README.md', 'r') as f:
     long_description = f.read()
 
 
-requirements = [
-    "requests",
-    "pydantic"
-]
+requirements = ['requests', 'pydantic']
 
 setuptools.setup(
-    name="megabot",
-    version="0.0.4",
-    author="Aleksandr Koksharov",
-    author_email="koksharov@yandex.ru",
-    description="Python telegram API adapter for FastAPI and asyncio",
+    name='megabot',
+    version='0.0.5',
+    author='Aleksandr Koksharov',
+    author_email='koksharov@yandex.ru',
+    description='Python telegram API adapter for FastAPI and asyncio',
     long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/imoknot/megabot",
+    long_description_content_type='text/markdown',
+    url='https://github.com/imoknot/megabot',
     packages=setuptools.find_packages(),
     install_requires=requirements,
-    license="MIT",
+    license='MIT',
     classifiers=[
-        "Development Status :: 3 - Alpha",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-        "Programming Language :: Python :: 3.12",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-        "Topic :: Software Development :: Libraries :: Python Modules"
+        'Development Status :: 2 - Pre-Alpha',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
+        'License :: OSI Approved :: MIT License',
+        'Operating System :: OS Independent',
+        'Topic :: Software Development :: Libraries :: Python Modules',
     ],
     project_urls={
-        "Bug Tracker": "https://github.com/imoknot/megabot/issues",
-        "Changelog": "https://github.com/imoknot/megabot/blob/master/CHANGELOG.md",
+        'Bug Tracker': 'https://github.com/imoknot/megabot/issues',
+        'Changelog': 'https://github.com/imoknot/megabot/blob/master/CHANGELOG.md',
     },
     python_requires='>=3.10',
 )
```

