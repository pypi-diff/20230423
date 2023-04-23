# Comparing `tmp/botterino-0.4.6.tar.gz` & `tmp/botterino-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botterino-0.4.6.tar", last modified: Sat Apr 22 20:12:07 2023, max compression
+gzip compressed data, was "botterino-0.4.7.tar", last modified: Sun Apr 23 04:16:35 2023, max compression
```

## Comparing `botterino-0.4.6.tar` & `botterino-0.4.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 adarsharegmi   (501) staff       (20)        0 2023-04-22 20:12:07.281185 botterino-0.4.6/
--rw-r--r--   0 adarsharegmi   (501) staff       (20)     1063 2021-06-10 02:59:26.000000 botterino-0.4.6/LICENSE
--rw-r--r--   0 adarsharegmi   (501) staff       (20)     5014 2023-04-22 20:12:07.281531 botterino-0.4.6/PKG-INFO
--rw-r--r--   0 adarsharegmi   (501) staff       (20)     4566 2022-08-30 05:36:56.000000 botterino-0.4.6/README.md
-drwxr-xr-x   0 adarsharegmi   (501) staff       (20)        0 2023-04-22 20:12:07.262874 botterino-0.4.6/botterino/
-drwxr-xr-x   0 adarsharegmi   (501) staff       (20)        0 2023-04-22 20:12:07.271298 botterino-0.4.6/botterino/Loader/
--rw-r--r--   0 adarsharegmi   (501) staff       (20)        0 2021-06-17 04:44:47.000000 botterino-0.4.6/botterino/Loader/__init__.py
--rw-r--r--   0 adarsharegmi   (501) staff       (20)      872 2022-08-14 01:33:23.000000 botterino-0.4.6/botterino/Loader/loader.py
-drwxr-xr-x   0 adarsharegmi   (501) staff       (20)        0 2023-04-22 20:12:07.278623 botterino-0.4.6/botterino/RedditPoller/
--rw-r--r--   0 adarsharegmi   (501) staff       (20)     1350 2021-06-10 06:21:42.000000 botterino-0.4.6/botterino/RedditPoller/RedditPoller.py
--rw-r--r--   0 adarsharegmi   (501) staff       (20)     2404 2021-04-17 04:06:11.000000 botterino-0.4.6/botterino/RedditPoller/Retry.py
--rw-r--r--   0 adarsharegmi   (501) staff       (20)        0 2020-10-17 08:27:10.000000 botterino-0.4.6/botterino/RedditPoller/__init__.py
-drwxr-xr-x   0 adarsharegmi   (501) staff       (20)        0 2023-04-22 20:12:07.280576 botterino-0.4.6/botterino/Utils/
--rw-r--r--   0 adarsharegmi   (501) staff       (20)        0 2021-04-08 15:21:02.000000 botterino-0.4.6/botterino/Utils/__init__.py
--rw-r--r--   0 adarsharegmi   (501) staff       (20)     3740 2023-04-22 20:09:11.000000 botterino-0.4.6/botterino/Utils/utils.py
--rw-r--r--   0 adarsharegmi   (501) staff       (20)     1499 2022-02-14 00:45:23.000000 botterino-0.4.6/botterino/__init__.py
--rw-r--r--   0 adarsharegmi   (501) staff       (20)       35 2022-08-30 04:36:07.000000 botterino-0.4.6/botterino/__main__.py
--rw-r--r--   0 adarsharegmi   (501) staff       (20)     2510 2022-11-02 21:19:09.000000 botterino-0.4.6/botterino/botterino.py
--rw-r--r--   0 adarsharegmi   (501) staff       (20)     3084 2023-04-06 08:15:56.000000 botterino-0.4.6/botterino/config.py
--rw-r--r--   0 adarsharegmi   (501) staff       (20)      532 2022-06-06 01:25:42.000000 botterino-0.4.6/botterino/failure.py
--rw-r--r--   0 adarsharegmi   (501) staff       (20)     5549 2023-04-06 08:18:19.000000 botterino-0.4.6/botterino/hosterino.py
--rw-r--r--   0 adarsharegmi   (501) staff       (20)     1151 2022-08-14 00:54:21.000000 botterino-0.4.6/botterino/posterino.py
--rw-r--r--   0 adarsharegmi   (501) staff       (20)     4577 2022-08-30 05:57:18.000000 botterino-0.4.6/botterino/ui.py
-drwxr-xr-x   0 adarsharegmi   (501) staff       (20)        0 2023-04-22 20:12:07.268825 botterino-0.4.6/botterino.egg-info/
--rw-r--r--   0 adarsharegmi   (501) staff       (20)     5014 2023-04-22 20:12:07.000000 botterino-0.4.6/botterino.egg-info/PKG-INFO
--rw-r--r--   0 adarsharegmi   (501) staff       (20)      591 2023-04-22 20:12:07.000000 botterino-0.4.6/botterino.egg-info/SOURCES.txt
--rw-r--r--   0 adarsharegmi   (501) staff       (20)        1 2023-04-22 20:12:07.000000 botterino-0.4.6/botterino.egg-info/dependency_links.txt
--rw-r--r--   0 adarsharegmi   (501) staff       (20)       63 2023-04-22 20:12:07.000000 botterino-0.4.6/botterino.egg-info/requires.txt
--rw-r--r--   0 adarsharegmi   (501) staff       (20)       10 2023-04-22 20:12:07.000000 botterino-0.4.6/botterino.egg-info/top_level.txt
--rw-r--r--   0 adarsharegmi   (501) staff       (20)      103 2021-06-10 03:23:33.000000 botterino-0.4.6/pyproject.toml
--rw-r--r--   0 adarsharegmi   (501) staff       (20)      628 2023-04-22 20:12:07.283027 botterino-0.4.6/setup.cfg
+drwxr-xr-x   0 adarsharegmi   (501) staff       (20)        0 2023-04-23 04:16:35.335624 botterino-0.4.7/
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     1063 2021-06-10 02:59:26.000000 botterino-0.4.7/LICENSE
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     5014 2023-04-23 04:16:35.336010 botterino-0.4.7/PKG-INFO
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     4566 2022-08-30 05:36:56.000000 botterino-0.4.7/README.md
+drwxr-xr-x   0 adarsharegmi   (501) staff       (20)        0 2023-04-23 04:16:35.264879 botterino-0.4.7/botterino/
+drwxr-xr-x   0 adarsharegmi   (501) staff       (20)        0 2023-04-23 04:16:35.289656 botterino-0.4.7/botterino/Loader/
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)        0 2021-06-17 04:44:47.000000 botterino-0.4.7/botterino/Loader/__init__.py
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)      872 2022-08-14 01:33:23.000000 botterino-0.4.7/botterino/Loader/loader.py
+drwxr-xr-x   0 adarsharegmi   (501) staff       (20)        0 2023-04-23 04:16:35.307697 botterino-0.4.7/botterino/RedditPoller/
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     1350 2021-06-10 06:21:42.000000 botterino-0.4.7/botterino/RedditPoller/RedditPoller.py
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     2404 2021-04-17 04:06:11.000000 botterino-0.4.7/botterino/RedditPoller/Retry.py
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)        0 2020-10-17 08:27:10.000000 botterino-0.4.7/botterino/RedditPoller/__init__.py
+drwxr-xr-x   0 adarsharegmi   (501) staff       (20)        0 2023-04-23 04:16:35.316227 botterino-0.4.7/botterino/Utils/
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)        0 2021-04-08 15:21:02.000000 botterino-0.4.7/botterino/Utils/__init__.py
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     3687 2023-04-23 04:07:21.000000 botterino-0.4.7/botterino/Utils/utils.py
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     1499 2022-02-14 00:45:23.000000 botterino-0.4.7/botterino/__init__.py
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)       35 2022-08-30 04:36:07.000000 botterino-0.4.7/botterino/__main__.py
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     2510 2022-11-02 21:19:09.000000 botterino-0.4.7/botterino/botterino.py
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     3116 2023-04-23 04:12:56.000000 botterino-0.4.7/botterino/config.py
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)      532 2022-06-06 01:25:42.000000 botterino-0.4.7/botterino/failure.py
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     5549 2023-04-06 08:18:19.000000 botterino-0.4.7/botterino/hosterino.py
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     1151 2022-08-14 00:54:21.000000 botterino-0.4.7/botterino/posterino.py
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     4577 2022-08-30 05:57:18.000000 botterino-0.4.7/botterino/ui.py
+drwxr-xr-x   0 adarsharegmi   (501) staff       (20)        0 2023-04-23 04:16:35.285813 botterino-0.4.7/botterino.egg-info/
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     5014 2023-04-23 04:16:35.000000 botterino-0.4.7/botterino.egg-info/PKG-INFO
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)      591 2023-04-23 04:16:35.000000 botterino-0.4.7/botterino.egg-info/SOURCES.txt
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)        1 2023-04-23 04:16:35.000000 botterino-0.4.7/botterino.egg-info/dependency_links.txt
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)       63 2023-04-23 04:16:35.000000 botterino-0.4.7/botterino.egg-info/requires.txt
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)       10 2023-04-23 04:16:35.000000 botterino-0.4.7/botterino.egg-info/top_level.txt
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)      103 2021-06-10 03:23:33.000000 botterino-0.4.7/pyproject.toml
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)      628 2023-04-23 04:16:35.337553 botterino-0.4.7/setup.cfg
```

### Comparing `botterino-0.4.6/LICENSE` & `botterino-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `botterino-0.4.6/PKG-INFO` & `botterino-0.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botterino
-Version: 0.4.6
+Version: 0.4.7
 Summary: Automate posting and hosting of rounds on /r/picturegame
 Home-page: https://github.com/pgitox/botterino
 Author: itoxici
 Author-email: itox@picturegame.co
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `botterino-0.4.6/README.md` & `botterino-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `botterino-0.4.6/botterino/Loader/loader.py` & `botterino-0.4.7/botterino/Loader/loader.py`

 * *Files identical despite different names*

### Comparing `botterino-0.4.6/botterino/RedditPoller/RedditPoller.py` & `botterino-0.4.7/botterino/RedditPoller/RedditPoller.py`

 * *Files identical despite different names*

### Comparing `botterino-0.4.6/botterino/RedditPoller/Retry.py` & `botterino-0.4.7/botterino/RedditPoller/Retry.py`

 * *Files identical despite different names*

### Comparing `botterino-0.4.6/botterino/Utils/utils.py` & `botterino-0.4.7/botterino/Utils/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..config import pg, username, debug, reddit, donotreply
+from ..config import pg, username, debug, reddit, donotreply, api
 from ..RedditPoller.RedditPoller import RedditPoller, CommentWrapper
 from ..RedditPoller.Retry import retry
 from geopy.point import Point
 from geopy.distance import distance
 from sty import fg
 from random import randrange
 from halo import Halo
@@ -53,33 +53,33 @@
         color = randrange(256)
     return fg(color)
 
 def postDelay():
     if debug:
         return -1
 
-    r = requests.get('https://api.picturegame.co/current')
+    r = requests.get(f'{api}/current')
     data = json.loads(r.content)
     tries = 1
 
     while data['round']['hostName'].lower() != username.lower():
         tries += 1
         if tries > 5:
             return -1
-        r = requests.get('https://api.picturegame.co/current')
+        r = requests.get(f'{api}/current')
         data = json.loads(r.content)
         time.sleep(5)
 
     return data['round'].get('postDelay', -1)
 
 def hyperlink(alias, url):
     return f'\u001b]8;;{url}\u001b\\{alias}\u001b]8;;\u001b\\'
 
 def getRoundPrefix():
-    r = requests.get('https://api.picturega.me/current')
+    r = requests.get(f'{api}/current')
     roundnum = int(json.loads(r.content)['round']['roundNumber']) + 1
     return f'[Round {roundnum}]'
 
 def approved():
     c = next(iter(pg.contributor()))
     return c and c.name.lower() == username.lower()
```

### Comparing `botterino-0.4.6/botterino/__init__.py` & `botterino-0.4.7/botterino/__init__.py`

 * *Files identical despite different names*

### Comparing `botterino-0.4.6/botterino/botterino.py` & `botterino-0.4.7/botterino/botterino.py`

 * *Files identical despite different names*

### Comparing `botterino-0.4.6/botterino/config.py` & `botterino-0.4.7/botterino/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,7 +88,8 @@
 donotreply = {
     'achievements-bot',
     username.lower(),
     'r-picturegame',
     'imreallycuriousbird',
 }
 
+api = 'https://api.picturega.me'
```

### Comparing `botterino-0.4.6/botterino/failure.py` & `botterino-0.4.7/botterino/failure.py`

 * *Files identical despite different names*

### Comparing `botterino-0.4.6/botterino/hosterino.py` & `botterino-0.4.7/botterino/hosterino.py`

 * *Files identical despite different names*

### Comparing `botterino-0.4.6/botterino/posterino.py` & `botterino-0.4.7/botterino/posterino.py`

 * *Files identical despite different names*

### Comparing `botterino-0.4.6/botterino/ui.py` & `botterino-0.4.7/botterino/ui.py`

 * *Files identical despite different names*

### Comparing `botterino-0.4.6/botterino.egg-info/PKG-INFO` & `botterino-0.4.7/botterino.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botterino
-Version: 0.4.6
+Version: 0.4.7
 Summary: Automate posting and hosting of rounds on /r/picturegame
 Home-page: https://github.com/pgitox/botterino
 Author: itoxici
 Author-email: itox@picturegame.co
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `botterino-0.4.6/botterino.egg-info/SOURCES.txt` & `botterino-0.4.7/botterino.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botterino-0.4.6/setup.cfg` & `botterino-0.4.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = botterino
-version = 0.4.6
+version = 0.4.7
 author = itoxici
 author_email = itox@picturegame.co
 description = Automate posting and hosting of rounds on /r/picturegame
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pgitox/botterino
 classifiers =
```

