# Comparing `tmp/ShynaTelegramBotNotification-0.0.3.tar.gz` & `tmp/ShynaTelegramBotNotification-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ShynaTelegramBotNotification-0.0.3.tar", last modified: Thu Mar 23 20:08:06 2023, max compression
+gzip compressed data, was "ShynaTelegramBotNotification-0.0.4.tar", last modified: Sun Apr 23 12:11:37 2023, max compression
```

## Comparing `ShynaTelegramBotNotification-0.0.3.tar` & `ShynaTelegramBotNotification-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 shyna     (1000) shyna     (1000)        0 2023-03-23 20:08:06.572186 ShynaTelegramBotNotification-0.0.3/
--rw-rw-r--   0 shyna     (1000) shyna     (1000)     1070 2023-03-23 20:06:28.000000 ShynaTelegramBotNotification-0.0.3/LICENSE
--rw-rw-r--   0 shyna     (1000) shyna     (1000)      980 2023-03-23 20:08:06.572186 ShynaTelegramBotNotification-0.0.3/PKG-INFO
--rw-rw-r--   0 shyna     (1000) shyna     (1000)      691 2023-03-23 20:06:28.000000 ShynaTelegramBotNotification-0.0.3/README.md
-drwxrwxr-x   0 shyna     (1000) shyna     (1000)        0 2023-03-23 20:08:06.572186 ShynaTelegramBotNotification-0.0.3/ShynaTelegramBotNotification/
--rw-rw-r--   0 shyna     (1000) shyna     (1000)     1405 2023-03-23 20:06:28.000000 ShynaTelegramBotNotification-0.0.3/ShynaTelegramBotNotification/BotNotify.py
--rw-rw-r--   0 shyna     (1000) shyna     (1000)     1376 2023-03-23 20:07:12.000000 ShynaTelegramBotNotification-0.0.3/ShynaTelegramBotNotification/Notify_Boss.py
--rw-rw-r--   0 shyna     (1000) shyna     (1000)        0 2023-03-23 20:06:28.000000 ShynaTelegramBotNotification-0.0.3/ShynaTelegramBotNotification/__init__.py
-drwxrwxr-x   0 shyna     (1000) shyna     (1000)        0 2023-03-23 20:08:06.572186 ShynaTelegramBotNotification-0.0.3/ShynaTelegramBotNotification.egg-info/
--rw-rw-r--   0 shyna     (1000) shyna     (1000)      980 2023-03-23 20:08:06.000000 ShynaTelegramBotNotification-0.0.3/ShynaTelegramBotNotification.egg-info/PKG-INFO
--rw-rw-r--   0 shyna     (1000) shyna     (1000)      427 2023-03-23 20:08:06.000000 ShynaTelegramBotNotification-0.0.3/ShynaTelegramBotNotification.egg-info/SOURCES.txt
--rw-rw-r--   0 shyna     (1000) shyna     (1000)        1 2023-03-23 20:08:06.000000 ShynaTelegramBotNotification-0.0.3/ShynaTelegramBotNotification.egg-info/dependency_links.txt
--rw-rw-r--   0 shyna     (1000) shyna     (1000)       66 2023-03-23 20:08:06.000000 ShynaTelegramBotNotification-0.0.3/ShynaTelegramBotNotification.egg-info/requires.txt
--rw-rw-r--   0 shyna     (1000) shyna     (1000)       29 2023-03-23 20:08:06.000000 ShynaTelegramBotNotification-0.0.3/ShynaTelegramBotNotification.egg-info/top_level.txt
--rw-rw-r--   0 shyna     (1000) shyna     (1000)      138 2023-03-23 20:06:28.000000 ShynaTelegramBotNotification-0.0.3/pyproject.toml
--rw-rw-r--   0 shyna     (1000) shyna     (1000)       38 2023-03-23 20:08:06.572186 ShynaTelegramBotNotification-0.0.3/setup.cfg
--rw-rw-r--   0 shyna     (1000) shyna     (1000)      725 2023-03-23 20:07:12.000000 ShynaTelegramBotNotification-0.0.3/setup.py
+drwxrwxr-x   0 shyna     (1000) shyna     (1000)        0 2023-04-23 12:11:37.122620 ShynaTelegramBotNotification-0.0.4/
+-rw-rw-r--   0 shyna     (1000) shyna     (1000)     1070 2023-03-23 20:06:28.000000 ShynaTelegramBotNotification-0.0.4/LICENSE
+-rw-rw-r--   0 shyna     (1000) shyna     (1000)      980 2023-04-23 12:11:37.122620 ShynaTelegramBotNotification-0.0.4/PKG-INFO
+-rw-rw-r--   0 shyna     (1000) shyna     (1000)      691 2023-03-23 20:06:28.000000 ShynaTelegramBotNotification-0.0.4/README.md
+drwxrwxr-x   0 shyna     (1000) shyna     (1000)        0 2023-04-23 12:11:37.122620 ShynaTelegramBotNotification-0.0.4/ShynaTelegramBotNotification/
+-rw-rw-r--   0 shyna     (1000) shyna     (1000)     1405 2023-03-23 20:06:28.000000 ShynaTelegramBotNotification-0.0.4/ShynaTelegramBotNotification/BotNotify.py
+-rw-rw-r--   0 shyna     (1000) shyna     (1000)     1401 2023-04-23 12:09:05.000000 ShynaTelegramBotNotification-0.0.4/ShynaTelegramBotNotification/Notify_Boss.py
+-rw-rw-r--   0 shyna     (1000) shyna     (1000)        0 2023-03-23 20:06:28.000000 ShynaTelegramBotNotification-0.0.4/ShynaTelegramBotNotification/__init__.py
+drwxrwxr-x   0 shyna     (1000) shyna     (1000)        0 2023-04-23 12:11:37.122620 ShynaTelegramBotNotification-0.0.4/ShynaTelegramBotNotification.egg-info/
+-rw-rw-r--   0 shyna     (1000) shyna     (1000)      980 2023-04-23 12:11:37.000000 ShynaTelegramBotNotification-0.0.4/ShynaTelegramBotNotification.egg-info/PKG-INFO
+-rw-rw-r--   0 shyna     (1000) shyna     (1000)      427 2023-04-23 12:11:37.000000 ShynaTelegramBotNotification-0.0.4/ShynaTelegramBotNotification.egg-info/SOURCES.txt
+-rw-rw-r--   0 shyna     (1000) shyna     (1000)        1 2023-04-23 12:11:37.000000 ShynaTelegramBotNotification-0.0.4/ShynaTelegramBotNotification.egg-info/dependency_links.txt
+-rw-rw-r--   0 shyna     (1000) shyna     (1000)       66 2023-04-23 12:11:37.000000 ShynaTelegramBotNotification-0.0.4/ShynaTelegramBotNotification.egg-info/requires.txt
+-rw-rw-r--   0 shyna     (1000) shyna     (1000)       29 2023-04-23 12:11:37.000000 ShynaTelegramBotNotification-0.0.4/ShynaTelegramBotNotification.egg-info/top_level.txt
+-rw-rw-r--   0 shyna     (1000) shyna     (1000)      138 2023-03-23 20:06:28.000000 ShynaTelegramBotNotification-0.0.4/pyproject.toml
+-rw-rw-r--   0 shyna     (1000) shyna     (1000)       38 2023-04-23 12:11:37.122620 ShynaTelegramBotNotification-0.0.4/setup.cfg
+-rw-rw-r--   0 shyna     (1000) shyna     (1000)      725 2023-04-23 12:10:04.000000 ShynaTelegramBotNotification-0.0.4/setup.py
```

### Comparing `ShynaTelegramBotNotification-0.0.3/LICENSE` & `ShynaTelegramBotNotification-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ShynaTelegramBotNotification-0.0.3/PKG-INFO` & `ShynaTelegramBotNotification-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ShynaTelegramBotNotification
-Version: 0.0.3
+Version: 0.0.4
 Summary: Shyna Telegram Bot Notification.Notifications will be taken care by this package.
 Author: Shivam Sharma
 Author-email: shivamsharma1913@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # shyna/ShynaTelegramBotNotification
```

### Comparing `ShynaTelegramBotNotification-0.0.3/README.md` & `ShynaTelegramBotNotification-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ShynaTelegramBotNotification-0.0.3/ShynaTelegramBotNotification/BotNotify.py` & `ShynaTelegramBotNotification-0.0.4/ShynaTelegramBotNotification/BotNotify.py`

 * *Files identical despite different names*

### Comparing `ShynaTelegramBotNotification-0.0.3/ShynaTelegramBotNotification/Notify_Boss.py` & `ShynaTelegramBotNotification-0.0.4/ShynaTelegramBotNotification/Notify_Boss.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import random
-
+import asyncio
 from ShynaDatabase import Shdatabase
 import telegram
 import os
 
 
 class NotifyBoss:
     s_data = Shdatabase.ShynaDatabase()
@@ -19,20 +19,20 @@
             self.result = self.s_data.select_from_table()
             if str(self.result[0]).lower().__eq__('empty'):
                 print("Empty")
             else:
                 for item in self.result:
                     print(item[3], item[4])
                     self.message = random.choice(str(item[4]).split("|"))
-                    self.bot_send_msg_to_master(bot_name=str(item[3]))
+                    asyncio.run(self.bot_send_msg_to_master(bot_name=str(item[3])))
                     self.s_data.query = "UPDATE bot_msg_backup SET status='True' where count='"+str(item[0])+"'"
                     self.s_data.create_insert_update_or_delete()
         except Exception as e:
             print(e)
 
-    def bot_send_msg_to_master(self, bot_name):
+    async def bot_send_msg_to_master(self, bot_name):
         bot = telegram.Bot(token=os.environ.get(bot_name))
-        self.status = bot.send_message(chat_id=self.master_telegram_chat_id, text=str(self.message))
+        await bot.send_message(chat_id=self.master_telegram_chat_id, text=str(self.message))
 
 
 if __name__ == '__main__':
     NotifyBoss().notify_boss()
```

### Comparing `ShynaTelegramBotNotification-0.0.3/ShynaTelegramBotNotification.egg-info/PKG-INFO` & `ShynaTelegramBotNotification-0.0.4/ShynaTelegramBotNotification.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ShynaTelegramBotNotification
-Version: 0.0.3
+Version: 0.0.4
 Summary: Shyna Telegram Bot Notification.Notifications will be taken care by this package.
 Author: Shivam Sharma
 Author-email: shivamsharma1913@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # shyna/ShynaTelegramBotNotification
```

### Comparing `ShynaTelegramBotNotification-0.0.3/setup.py` & `ShynaTelegramBotNotification-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup_args = dict(
      name='ShynaTelegramBotNotification',
-     version='0.0.03',
+     version='0.0.04',
      packages=find_packages(),
      author="Shivam Sharma",
      author_email="shivamsharma1913@gmail.com",
      description="Shyna Telegram Bot Notification.Notifications will be taken care by this package.",
      long_description=long_description,
      long_description_content_type="text/markdown",
     )
```

