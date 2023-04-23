# Comparing `tmp/megabot-0.0.5.tar.gz` & `tmp/megabot-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "megabot-0.0.5.tar", last modified: Sun Apr 23 07:50:56 2023, max compression
+gzip compressed data, was "megabot-0.0.6.tar", last modified: Sun Apr 23 08:16:56 2023, max compression
```

## Comparing `megabot-0.0.5.tar` & `megabot-0.0.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 07:50:56.583901 megabot-0.0.5/
--rw-rw-rw-   0        0        0     1094 2023-04-03 06:41:39.000000 megabot-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     3258 2023-04-23 07:50:56.583901 megabot-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2391 2023-04-05 10:57:01.000000 megabot-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 07:50:56.501878 megabot-0.0.5/megabot/
--rw-rw-rw-   0        0        0       82 2023-04-23 07:30:07.000000 megabot-0.0.5/megabot/__init__.py
--rw-rw-rw-   0        0        0      418 2023-04-23 07:30:07.000000 megabot-0.0.5/megabot/command.py
--rw-rw-rw-   0        0        0     4479 2023-04-23 07:30:07.000000 megabot-0.0.5/megabot/dispatcher.py
-drwxrwxrwx   0        0        0        0 2023-04-23 07:50:56.576892 megabot-0.0.5/megabot/models/
--rw-rw-rw-   0        0        0      529 2023-04-23 07:30:07.000000 megabot-0.0.5/megabot/models/__init__.py
--rw-rw-rw-   0        0        0     1035 2023-04-23 07:30:07.000000 megabot-0.0.5/megabot/models/base.py
--rw-rw-rw-   0        0        0      610 2023-04-23 07:30:02.000000 megabot-0.0.5/megabot/models/callback.py
--rw-rw-rw-   0        0        0     2730 2023-04-23 07:30:02.000000 megabot-0.0.5/megabot/models/chats.py
--rw-rw-rw-   0        0        0      287 2023-04-23 07:30:07.000000 megabot-0.0.5/megabot/models/command.py
--rw-rw-rw-   0        0        0       99 2023-04-23 07:30:07.000000 megabot-0.0.5/megabot/models/emodj.py
--rw-rw-rw-   0        0        0      386 2023-04-23 07:30:02.000000 megabot-0.0.5/megabot/models/file.py
--rw-rw-rw-   0        0        0      503 2023-04-23 07:30:07.000000 megabot-0.0.5/megabot/models/forum.py
--rw-rw-rw-   0        0        0      371 2023-04-23 07:30:07.000000 megabot-0.0.5/megabot/models/game.py
--rw-rw-rw-   0        0        0     2240 2023-04-23 07:30:02.000000 megabot-0.0.5/megabot/models/keyboards.py
--rw-rw-rw-   0        0        0     1583 2023-04-23 07:30:07.000000 megabot-0.0.5/megabot/models/media.py
--rw-rw-rw-   0        0        0     5399 2023-04-23 07:30:07.000000 megabot-0.0.5/megabot/models/message.py
--rw-rw-rw-   0        0        0      794 2023-04-23 07:30:07.000000 megabot-0.0.5/megabot/models/payment.py
--rw-rw-rw-   0        0        0      826 2023-04-23 07:30:02.000000 megabot-0.0.5/megabot/models/photo.py
--rw-rw-rw-   0        0        0      641 2023-04-23 07:30:07.000000 megabot-0.0.5/megabot/models/poll.py
--rw-rw-rw-   0        0        0      655 2023-04-23 07:30:02.000000 megabot-0.0.5/megabot/models/sticker.py
--rw-rw-rw-   0        0        0     1523 2023-04-23 07:30:07.000000 megabot-0.0.5/megabot/models/users.py
--rw-rw-rw-   0        0        0      374 2023-04-23 07:30:07.000000 megabot-0.0.5/megabot/models/video.py
--rw-rw-rw-   0        0        0      104 2023-04-23 07:30:07.000000 megabot-0.0.5/megabot/models/web_app.py
--rw-rw-rw-   0        0        0     5224 2023-04-23 07:30:07.000000 megabot-0.0.5/megabot/sender.py
-drwxrwxrwx   0        0        0        0 2023-04-23 07:50:56.581877 megabot-0.0.5/megabot/utils/
--rw-rw-rw-   0        0        0       41 2023-04-23 07:30:07.000000 megabot-0.0.5/megabot/utils/__init__.py
--rw-rw-rw-   0        0        0     1300 2023-04-23 07:30:07.000000 megabot-0.0.5/megabot/utils/callback_data.py
-drwxrwxrwx   0        0        0        0 2023-04-23 07:50:56.533898 megabot-0.0.5/megabot.egg-info/
--rw-rw-rw-   0        0        0     3258 2023-04-23 07:50:56.000000 megabot-0.0.5/megabot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      813 2023-04-23 07:50:56.000000 megabot-0.0.5/megabot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 07:50:56.000000 megabot-0.0.5/megabot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-04-23 07:50:56.000000 megabot-0.0.5/megabot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-23 07:50:56.000000 megabot-0.0.5/megabot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       67 2023-04-12 15:12:33.000000 megabot-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       80 2023-04-23 07:50:56.586893 megabot-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1198 2023-04-23 07:50:16.000000 megabot-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 08:16:56.620263 megabot-0.0.6/
+-rw-rw-rw-   0        0        0     1094 2023-04-03 06:41:39.000000 megabot-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     3258 2023-04-23 08:16:56.621258 megabot-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2391 2023-04-05 10:57:01.000000 megabot-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 08:16:56.535272 megabot-0.0.6/megabot/
+-rw-rw-rw-   0        0        0      119 2023-04-23 08:13:39.000000 megabot-0.0.6/megabot/__init__.py
+-rw-rw-rw-   0        0        0      418 2023-04-23 07:30:07.000000 megabot-0.0.6/megabot/command.py
+-rw-rw-rw-   0        0        0     4479 2023-04-23 07:30:07.000000 megabot-0.0.6/megabot/dispatcher.py
+drwxrwxrwx   0        0        0        0 2023-04-23 08:16:56.612254 megabot-0.0.6/megabot/models/
+-rw-rw-rw-   0        0        0      529 2023-04-23 07:30:07.000000 megabot-0.0.6/megabot/models/__init__.py
+-rw-rw-rw-   0        0        0     1035 2023-04-23 07:30:07.000000 megabot-0.0.6/megabot/models/base.py
+-rw-rw-rw-   0        0        0      610 2023-04-23 07:30:02.000000 megabot-0.0.6/megabot/models/callback.py
+-rw-rw-rw-   0        0        0     2730 2023-04-23 07:30:02.000000 megabot-0.0.6/megabot/models/chats.py
+-rw-rw-rw-   0        0        0      287 2023-04-23 07:30:07.000000 megabot-0.0.6/megabot/models/command.py
+-rw-rw-rw-   0        0        0       99 2023-04-23 07:30:07.000000 megabot-0.0.6/megabot/models/emodj.py
+-rw-rw-rw-   0        0        0      386 2023-04-23 07:30:02.000000 megabot-0.0.6/megabot/models/file.py
+-rw-rw-rw-   0        0        0      503 2023-04-23 07:30:07.000000 megabot-0.0.6/megabot/models/forum.py
+-rw-rw-rw-   0        0        0      371 2023-04-23 07:30:07.000000 megabot-0.0.6/megabot/models/game.py
+-rw-rw-rw-   0        0        0     2240 2023-04-23 07:30:02.000000 megabot-0.0.6/megabot/models/keyboards.py
+-rw-rw-rw-   0        0        0     1583 2023-04-23 07:30:07.000000 megabot-0.0.6/megabot/models/media.py
+-rw-rw-rw-   0        0        0     5399 2023-04-23 07:30:07.000000 megabot-0.0.6/megabot/models/message.py
+-rw-rw-rw-   0        0        0      794 2023-04-23 07:30:07.000000 megabot-0.0.6/megabot/models/payment.py
+-rw-rw-rw-   0        0        0      826 2023-04-23 07:30:02.000000 megabot-0.0.6/megabot/models/photo.py
+-rw-rw-rw-   0        0        0      641 2023-04-23 07:30:07.000000 megabot-0.0.6/megabot/models/poll.py
+-rw-rw-rw-   0        0        0      655 2023-04-23 07:30:02.000000 megabot-0.0.6/megabot/models/sticker.py
+-rw-rw-rw-   0        0        0     1523 2023-04-23 07:30:07.000000 megabot-0.0.6/megabot/models/users.py
+-rw-rw-rw-   0        0        0      374 2023-04-23 07:30:07.000000 megabot-0.0.6/megabot/models/video.py
+-rw-rw-rw-   0        0        0      104 2023-04-23 07:30:07.000000 megabot-0.0.6/megabot/models/web_app.py
+-rw-rw-rw-   0        0        0     5224 2023-04-23 07:30:07.000000 megabot-0.0.6/megabot/sender.py
+drwxrwxrwx   0        0        0        0 2023-04-23 08:16:56.618262 megabot-0.0.6/megabot/utils/
+-rw-rw-rw-   0        0        0       41 2023-04-23 07:30:07.000000 megabot-0.0.6/megabot/utils/__init__.py
+-rw-rw-rw-   0        0        0     1300 2023-04-23 07:30:07.000000 megabot-0.0.6/megabot/utils/callback_data.py
+drwxrwxrwx   0        0        0        0 2023-04-23 08:16:56.563262 megabot-0.0.6/megabot.egg-info/
+-rw-rw-rw-   0        0        0     3258 2023-04-23 08:16:56.000000 megabot-0.0.6/megabot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      813 2023-04-23 08:16:56.000000 megabot-0.0.6/megabot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 08:16:56.000000 megabot-0.0.6/megabot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-04-23 08:16:56.000000 megabot-0.0.6/megabot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-23 08:16:56.000000 megabot-0.0.6/megabot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       67 2023-04-12 15:12:33.000000 megabot-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       80 2023-04-23 08:16:56.624265 megabot-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1198 2023-04-23 08:16:28.000000 megabot-0.0.6/setup.py
```

### Comparing `megabot-0.0.5/LICENSE` & `megabot-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `megabot-0.0.5/PKG-INFO` & `megabot-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: megabot
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python telegram API adapter for FastAPI and asyncio
 Home-page: https://github.com/imoknot/megabot
 Author: Aleksandr Koksharov
 Author-email: koksharov@yandex.ru
 License: MIT
 Project-URL: Bug Tracker, https://github.com/imoknot/megabot/issues
 Project-URL: Changelog, https://github.com/imoknot/megabot/blob/master/CHANGELOG.md
```

### Comparing `megabot-0.0.5/README.md` & `megabot-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `megabot-0.0.5/megabot/dispatcher.py` & `megabot-0.0.6/megabot/dispatcher.py`

 * *Files identical despite different names*

### Comparing `megabot-0.0.5/megabot/models/__init__.py` & `megabot-0.0.6/megabot/models/__init__.py`

 * *Files identical despite different names*

### Comparing `megabot-0.0.5/megabot/models/base.py` & `megabot-0.0.6/megabot/models/base.py`

 * *Files identical despite different names*

### Comparing `megabot-0.0.5/megabot/models/callback.py` & `megabot-0.0.6/megabot/models/callback.py`

 * *Files identical despite different names*

### Comparing `megabot-0.0.5/megabot/models/chats.py` & `megabot-0.0.6/megabot/models/chats.py`

 * *Files identical despite different names*

### Comparing `megabot-0.0.5/megabot/models/keyboards.py` & `megabot-0.0.6/megabot/models/keyboards.py`

 * *Files identical despite different names*

### Comparing `megabot-0.0.5/megabot/models/media.py` & `megabot-0.0.6/megabot/models/media.py`

 * *Files identical despite different names*

### Comparing `megabot-0.0.5/megabot/models/message.py` & `megabot-0.0.6/megabot/models/message.py`

 * *Files identical despite different names*

### Comparing `megabot-0.0.5/megabot/models/payment.py` & `megabot-0.0.6/megabot/models/payment.py`

 * *Files identical despite different names*

### Comparing `megabot-0.0.5/megabot/models/photo.py` & `megabot-0.0.6/megabot/models/photo.py`

 * *Files identical despite different names*

### Comparing `megabot-0.0.5/megabot/models/poll.py` & `megabot-0.0.6/megabot/models/poll.py`

 * *Files identical despite different names*

### Comparing `megabot-0.0.5/megabot/models/sticker.py` & `megabot-0.0.6/megabot/models/sticker.py`

 * *Files identical despite different names*

### Comparing `megabot-0.0.5/megabot/models/users.py` & `megabot-0.0.6/megabot/models/users.py`

 * *Files identical despite different names*

### Comparing `megabot-0.0.5/megabot/sender.py` & `megabot-0.0.6/megabot/sender.py`

 * *Files identical despite different names*

### Comparing `megabot-0.0.5/megabot/utils/callback_data.py` & `megabot-0.0.6/megabot/utils/callback_data.py`

 * *Files identical despite different names*

### Comparing `megabot-0.0.5/megabot.egg-info/PKG-INFO` & `megabot-0.0.6/megabot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: megabot
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python telegram API adapter for FastAPI and asyncio
 Home-page: https://github.com/imoknot/megabot
 Author: Aleksandr Koksharov
 Author-email: koksharov@yandex.ru
 License: MIT
 Project-URL: Bug Tracker, https://github.com/imoknot/megabot/issues
 Project-URL: Changelog, https://github.com/imoknot/megabot/blob/master/CHANGELOG.md
```

### Comparing `megabot-0.0.5/megabot.egg-info/SOURCES.txt` & `megabot-0.0.6/megabot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `megabot-0.0.5/setup.py` & `megabot-0.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 
 requirements = ['requests', 'pydantic']
 
 setuptools.setup(
     name='megabot',
-    version='0.0.5',
+    version='0.0.6',
     author='Aleksandr Koksharov',
     author_email='koksharov@yandex.ru',
     description='Python telegram API adapter for FastAPI and asyncio',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/imoknot/megabot',
     packages=setuptools.find_packages(),
```

