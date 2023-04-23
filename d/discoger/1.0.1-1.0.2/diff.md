# Comparing `tmp/discoger-1.0.1.tar.gz` & `tmp/discoger-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discoger-1.0.1.tar", last modified: Sun Apr 23 12:40:17 2023, max compression
+gzip compressed data, was "discoger-1.0.2.tar", last modified: Sun Apr 23 17:08:01 2023, max compression
```

## Comparing `discoger-1.0.1.tar` & `discoger-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:40:17.751697 discoger-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-23 12:40:03.000000 discoger-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-23 12:40:17.751697 discoger-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-23 12:40:03.000000 discoger-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:40:17.747697 discoger-1.0.1/discoger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:40:03.000000 discoger-1.0.1/discoger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-23 12:40:03.000000 discoger-1.0.1/discoger/_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-04-23 12:40:03.000000 discoger-1.0.1/discoger/discoger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:40:17.751697 discoger-1.0.1/discoger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-23 12:40:17.000000 discoger-1.0.1/discoger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-23 12:40:17.000000 discoger-1.0.1/discoger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 12:40:17.000000 discoger-1.0.1/discoger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-23 12:40:17.000000 discoger-1.0.1/discoger.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-23 12:40:17.000000 discoger-1.0.1/discoger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-23 12:40:17.000000 discoger-1.0.1/discoger.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-23 12:40:17.751697 discoger-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-04-23 12:40:03.000000 discoger-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:08:01.724452 discoger-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-23 17:07:44.000000 discoger-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-23 17:08:01.728452 discoger-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-23 17:07:44.000000 discoger-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:08:01.724452 discoger-1.0.2/discoger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 17:07:44.000000 discoger-1.0.2/discoger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-23 17:07:44.000000 discoger-1.0.2/discoger/_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7387 2023-04-23 17:07:44.000000 discoger-1.0.2/discoger/discoger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:08:01.724452 discoger-1.0.2/discoger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-23 17:08:01.000000 discoger-1.0.2/discoger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-23 17:08:01.000000 discoger-1.0.2/discoger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 17:08:01.000000 discoger-1.0.2/discoger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-23 17:08:01.000000 discoger-1.0.2/discoger.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-23 17:08:01.000000 discoger-1.0.2/discoger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-23 17:08:01.000000 discoger-1.0.2/discoger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-23 17:08:01.728452 discoger-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-04-23 17:07:44.000000 discoger-1.0.2/setup.py
```

### Comparing `discoger-1.0.1/LICENSE` & `discoger-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `discoger-1.0.1/PKG-INFO` & `discoger-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: discoger
-Version: 1.0.1
+Version: 1.0.2
 Summary: Get notification from Discogs
 Home-page: https://github.com/beudbeud/discoger
 Author: Beudbeud
 Author-email: beudbeud@gmail.com
 License: GNU General Public License v3 (GPLv3)
-Download-URL: https://github.com/beudbeud/discoger/archive/1.0.1.tar.gz
+Download-URL: https://github.com/beudbeud/discoger/archive/1.0.2.tar.gz
 Description: # Discoger
         
         Telegram bot for checking if there are new sell in one specific list on Discogs
         
         ## How to use it
         
         ### Installation
```

### Comparing `discoger-1.0.1/README.md` & `discoger-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `discoger-1.0.1/discoger/discoger.py` & `discoger-1.0.2/discoger/discoger.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,35 +9,26 @@
 
 import threading
 import schedule
 import time
 from time import sleep
 
 import telebot
-from telebot import types
+from telebot import types, util
 
 import logging
 logging.basicConfig(format='%(asctime)s %(levelname)s - %(message)s', level=logging.INFO)
 
 home = str(Path.home())
 config_file = Path(home + "/.config/discoger/config.ini")
 database_dir = Path(home + "/.config/discoger/databases")
 
 
-def read_ini(file_path):
-    config = configparser.ConfigParser()
-    config.read(file_path)
-    for section in config.sections():
-        for key in config[section]:
-            print((key, config[section][key]))
-    return config
-
-
 if config_file.exists():
-    config = read_ini(config_file)
+    config = configparser.ConfigParser()
     config.read(config_file)
 else:
     logging.error("No config file, please create a config file follwing example")
     raise SystemExit()
 
 if not database_dir.exists():
     database_dir.mkdir(parents=True, exist_ok=True)
@@ -80,41 +71,50 @@
     db = YamlDB(filename="%s/.config/discoger/databases/%s.yaml" % (home, chat_id))
     if db.get("release_list"):
         bot.send_message(chat_id, "Okay i check your discogs list")
         check_discogs(chat_id)
     else:
         db["release_list"] = list()
         db.save()
-        bot.send_message(chat_id, "Your discoger want list is empty, send me item url first")
+        bot.send_message(chat_id, "Your discoger following list is empty, send me item url first")
 
 
 @bot.message_handler(regexp="^https://www.discogs.com/fr/release/.*")
 def handle_message(message):
     release_info = dict()
     chat_id = message.chat.id
     release_id = re.findall(r'\d+', message.text)[0]
-    relase_all_info = d.release(release_id)
-    bot.send_message(chat_id, release_id)
     db = YamlDB(filename="%s/.config/discoger/databases/%s.yaml" % (home, chat_id))
-    release_info["release_id"] = release_id
-    release_info["artist"] = relase_all_info.artists[0].name
-    release_info["title"] = relase_all_info.title
-    release_info["last_sell"] = dict()
-    db["release_list"].append(release_info)
-    db.save()
+    if not db.search("release_list[?release_id=='%s']" % (release_id)):
+        relase_all_info = d.release(release_id)
+        db = YamlDB(filename="%s/.config/discoger/databases/%s.yaml" % (home, chat_id))
+        release_info["release_id"] = release_id
+        release_info["artist"] = relase_all_info.artists[0].name
+        release_info["title"] = relase_all_info.title
+        release_info["last_sell"] = dict()
+        db["release_list"].append(release_info)
+        db.save()
+        bot.send_message(chat_id, "%s is added in following list" % (release_id))
+    else:
+        bot.send_message(chat_id, "%s is already in following list" % (release_id))
 
 
 @bot.message_handler(commands=['list'])
 def get_list(message):
     chat_id = message.chat.id
     db = YamlDB(filename="%s/.config/discoger/databases/%s.yaml" % (home, chat_id))
     id_list = 0
+    all_text = ""
     for i in db["release_list"]:
-        bot.send_message(chat_id, "%s: %s - %s" % (id_list, i["artist"], i["title"]))
+        text = "%s: %s - %s https://www.discogs.com/fr/release/%s" % (id_list, i["artist"], i["title"], i["release_id"])
+        all_text = all_text + "\n" + text
         id_list = id_list + 1
+    splitted_text = util.split_string(all_text, 3000)
+    for text in splitted_text:
+        bot.send_message(chat_id, text, disable_web_page_preview=True)
 
 
 @bot.message_handler(commands=['delete'])
 def delete_release(message):
     msg = "Which item do you want delete in your list?"
     answer = bot.reply_to(message, msg)
     bot.register_next_step_handler(answer, process_delete_step)
@@ -122,26 +122,31 @@
 
 def process_delete_step(message):
     chat_id = message.chat.id
     id_item = message.text
     db = YamlDB(filename="%s/.config/discoger/databases/%s.yaml" % (home, chat_id))
     db["release_list"].pop(int(id_item))
     db.save()
+    bot.send_message(chat_id, "% is deleted in following list" % (id_item))
 
 
 def get_info(release_id):
     data_last_sell = dict()
     url = f"https://www.discogs.com/fr/sell/mplistrss?output=rss&release_id={release_id}"
     feed = feedparser.parse(url)
-    entry = feed.entries[-1]
-    data_last_sell["id"] = re.findall(r'\d+', entry["link"])[0]
-    data_last_sell["date"] = entry["updated"]
-    data_last_sell["url"] = entry["link"]
-    data_last_sell["price"] = re.findall(r'... \d?\d?\d\d.\d\d', entry["summary_detail"]["value"])[0]
-    return data_last_sell
+    try:
+        entry = feed.entries[-1]
+        data_last_sell["id"] = re.findall(r'\d+', entry["link"])[0]
+        data_last_sell["date"] = entry["updated"]
+        data_last_sell["url"] = entry["link"]
+        data_last_sell["price"] = re.findall(r'... \d?\d?\d\d.\d\d', entry["summary_detail"]["value"])[0]
+        return data_last_sell
+    except Exception as e:
+        logging.debug("%s: for %s item" % (e, release_id))
+        return None
 
 
 def check_discogs(chat_id=None):
     if chat_id:
         logging.info("Check user list %s" % (chat_id))
         scrap_data(chat_id)
     else:
@@ -151,23 +156,27 @@
             logging.info("Check user list %s" % (chat_id))
             scrap_data(chat_id)
 
 
 def scrap_data(chat_id):
     db = YamlDB(filename="%s/.config/discoger/databases/%s.yaml" % (home, chat_id))
     chat_id = db.get("chat_id")
-    for i in db["release_list"]:
-        data_last_sell = get_info(i["release_id"])
-        if not i["last_sell"] or (i["last_sell"]["id"] != data_last_sell["id"] and i["last_sell"]["date"] < data_last_sell["date"]):
-            logging.info("New item for %s - %s" % (i["artist"], i["title"]))
-            text = "New release for :\n%s\ndate: %s\nprice: %s\n%s" % (i["title"], data_last_sell["date"], data_last_sell["price"], data_last_sell["url"])
-            bot.send_message(chat_id, text)
-            i["last_sell"] = data_last_sell
+    for i in range(len(db["release_list"])):
+        item = db.search("release_list[%s]" % (str(i)))
+        data_last_sell = get_info(item["release_id"])
+        if data_last_sell:
+            if not item["last_sell"] or (item["last_sell"]["id"] != data_last_sell["id"] and item["last_sell"]["date"] < data_last_sell["date"]):
+                logging.info("New item for %s - %s" % (item["artist"], item["title"]))
+                text = "New release for :\n%s\ndate: %s\nprice: %s\n%s" % (item["title"], data_last_sell["date"], data_last_sell["price"], data_last_sell["url"])
+                bot.send_message(chat_id, text)
+                db["release_list"][i]["last_sell"] = data_last_sell
+            else:
+                logging.info("Not new item for %s - %s" % (db["release_list"][i]["artist"], db["release_list"][i]["title"]))
         else:
-            logging.info("Not new item for %s - %s" % (i["artist"], i["title"]))
+            logging.info("Nothing available for %s - %s" % (db["release_list"][i]["artist"], db["release_list"][i]["title"]))
     db.save()
 
 
 def bot_polling():
     while True:
         try:
             logging.info("Starting bot polling now. New bot instance started!")
```

### Comparing `discoger-1.0.1/discoger.egg-info/PKG-INFO` & `discoger-1.0.2/discoger.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: discoger
-Version: 1.0.1
+Version: 1.0.2
 Summary: Get notification from Discogs
 Home-page: https://github.com/beudbeud/discoger
 Author: Beudbeud
 Author-email: beudbeud@gmail.com
 License: GNU General Public License v3 (GPLv3)
-Download-URL: https://github.com/beudbeud/discoger/archive/1.0.1.tar.gz
+Download-URL: https://github.com/beudbeud/discoger/archive/1.0.2.tar.gz
 Description: # Discoger
         
         Telegram bot for checking if there are new sell in one specific list on Discogs
         
         ## How to use it
         
         ### Installation
```

### Comparing `discoger-1.0.1/setup.py` & `discoger-1.0.2/setup.py`

 * *Files identical despite different names*

