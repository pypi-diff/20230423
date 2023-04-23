# Comparing `tmp/botterino-0.4.7.tar.gz` & `tmp/botterino-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botterino-0.4.7.tar", last modified: Sun Apr 23 04:16:35 2023, max compression
+gzip compressed data, was "botterino-0.4.8.tar", last modified: Sun Apr 23 06:21:18 2023, max compression
```

## Comparing `botterino-0.4.7.tar` & `botterino-0.4.8.tar`

### file list

```diff
@@ -1,31 +1,34 @@
-drwxr-xr-x   0 adarsharegmi   (501) staff       (20)        0 2023-04-23 04:16:35.335624 botterino-0.4.7/
--rw-r--r--   0 adarsharegmi   (501) staff       (20)     1063 2021-06-10 02:59:26.000000 botterino-0.4.7/LICENSE
--rw-r--r--   0 adarsharegmi   (501) staff       (20)     5014 2023-04-23 04:16:35.336010 botterino-0.4.7/PKG-INFO
--rw-r--r--   0 adarsharegmi   (501) staff       (20)     4566 2022-08-30 05:36:56.000000 botterino-0.4.7/README.md
-drwxr-xr-x   0 adarsharegmi   (501) staff       (20)        0 2023-04-23 04:16:35.264879 botterino-0.4.7/botterino/
-drwxr-xr-x   0 adarsharegmi   (501) staff       (20)        0 2023-04-23 04:16:35.289656 botterino-0.4.7/botterino/Loader/
--rw-r--r--   0 adarsharegmi   (501) staff       (20)        0 2021-06-17 04:44:47.000000 botterino-0.4.7/botterino/Loader/__init__.py
--rw-r--r--   0 adarsharegmi   (501) staff       (20)      872 2022-08-14 01:33:23.000000 botterino-0.4.7/botterino/Loader/loader.py
-drwxr-xr-x   0 adarsharegmi   (501) staff       (20)        0 2023-04-23 04:16:35.307697 botterino-0.4.7/botterino/RedditPoller/
--rw-r--r--   0 adarsharegmi   (501) staff       (20)     1350 2021-06-10 06:21:42.000000 botterino-0.4.7/botterino/RedditPoller/RedditPoller.py
--rw-r--r--   0 adarsharegmi   (501) staff       (20)     2404 2021-04-17 04:06:11.000000 botterino-0.4.7/botterino/RedditPoller/Retry.py
--rw-r--r--   0 adarsharegmi   (501) staff       (20)        0 2020-10-17 08:27:10.000000 botterino-0.4.7/botterino/RedditPoller/__init__.py
-drwxr-xr-x   0 adarsharegmi   (501) staff       (20)        0 2023-04-23 04:16:35.316227 botterino-0.4.7/botterino/Utils/
--rw-r--r--   0 adarsharegmi   (501) staff       (20)        0 2021-04-08 15:21:02.000000 botterino-0.4.7/botterino/Utils/__init__.py
--rw-r--r--   0 adarsharegmi   (501) staff       (20)     3687 2023-04-23 04:07:21.000000 botterino-0.4.7/botterino/Utils/utils.py
--rw-r--r--   0 adarsharegmi   (501) staff       (20)     1499 2022-02-14 00:45:23.000000 botterino-0.4.7/botterino/__init__.py
--rw-r--r--   0 adarsharegmi   (501) staff       (20)       35 2022-08-30 04:36:07.000000 botterino-0.4.7/botterino/__main__.py
--rw-r--r--   0 adarsharegmi   (501) staff       (20)     2510 2022-11-02 21:19:09.000000 botterino-0.4.7/botterino/botterino.py
--rw-r--r--   0 adarsharegmi   (501) staff       (20)     3116 2023-04-23 04:12:56.000000 botterino-0.4.7/botterino/config.py
--rw-r--r--   0 adarsharegmi   (501) staff       (20)      532 2022-06-06 01:25:42.000000 botterino-0.4.7/botterino/failure.py
--rw-r--r--   0 adarsharegmi   (501) staff       (20)     5549 2023-04-06 08:18:19.000000 botterino-0.4.7/botterino/hosterino.py
--rw-r--r--   0 adarsharegmi   (501) staff       (20)     1151 2022-08-14 00:54:21.000000 botterino-0.4.7/botterino/posterino.py
--rw-r--r--   0 adarsharegmi   (501) staff       (20)     4577 2022-08-30 05:57:18.000000 botterino-0.4.7/botterino/ui.py
-drwxr-xr-x   0 adarsharegmi   (501) staff       (20)        0 2023-04-23 04:16:35.285813 botterino-0.4.7/botterino.egg-info/
--rw-r--r--   0 adarsharegmi   (501) staff       (20)     5014 2023-04-23 04:16:35.000000 botterino-0.4.7/botterino.egg-info/PKG-INFO
--rw-r--r--   0 adarsharegmi   (501) staff       (20)      591 2023-04-23 04:16:35.000000 botterino-0.4.7/botterino.egg-info/SOURCES.txt
--rw-r--r--   0 adarsharegmi   (501) staff       (20)        1 2023-04-23 04:16:35.000000 botterino-0.4.7/botterino.egg-info/dependency_links.txt
--rw-r--r--   0 adarsharegmi   (501) staff       (20)       63 2023-04-23 04:16:35.000000 botterino-0.4.7/botterino.egg-info/requires.txt
--rw-r--r--   0 adarsharegmi   (501) staff       (20)       10 2023-04-23 04:16:35.000000 botterino-0.4.7/botterino.egg-info/top_level.txt
--rw-r--r--   0 adarsharegmi   (501) staff       (20)      103 2021-06-10 03:23:33.000000 botterino-0.4.7/pyproject.toml
--rw-r--r--   0 adarsharegmi   (501) staff       (20)      628 2023-04-23 04:16:35.337553 botterino-0.4.7/setup.cfg
+drwxr-xr-x   0 adarsharegmi   (501) staff       (20)        0 2023-04-23 06:21:18.008434 botterino-0.4.8/
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     1063 2021-06-10 02:59:26.000000 botterino-0.4.8/LICENSE
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     5014 2023-04-23 06:21:18.009084 botterino-0.4.8/PKG-INFO
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     4566 2022-08-30 05:36:56.000000 botterino-0.4.8/README.md
+drwxr-xr-x   0 adarsharegmi   (501) staff       (20)        0 2023-04-23 06:21:17.987075 botterino-0.4.8/botterino/
+drwxr-xr-x   0 adarsharegmi   (501) staff       (20)        0 2023-04-23 06:21:17.995619 botterino-0.4.8/botterino/Loader/
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)        0 2021-06-17 04:44:47.000000 botterino-0.4.8/botterino/Loader/__init__.py
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)      868 2023-04-23 04:36:39.000000 botterino-0.4.8/botterino/Loader/loader.py
+drwxr-xr-x   0 adarsharegmi   (501) staff       (20)        0 2023-04-23 06:21:17.999803 botterino-0.4.8/botterino/Map/
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)        0 2023-04-23 04:46:10.000000 botterino-0.4.8/botterino/Map/__init__.py
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     1471 2023-04-23 06:15:24.000000 botterino-0.4.8/botterino/Map/map.py
+drwxr-xr-x   0 adarsharegmi   (501) staff       (20)        0 2023-04-23 06:21:18.004857 botterino-0.4.8/botterino/RedditPoller/
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     1368 2023-04-23 04:36:39.000000 botterino-0.4.8/botterino/RedditPoller/RedditPoller.py
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     2443 2023-04-23 04:36:39.000000 botterino-0.4.8/botterino/RedditPoller/Retry.py
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)        0 2020-10-17 08:27:10.000000 botterino-0.4.8/botterino/RedditPoller/__init__.py
+drwxr-xr-x   0 adarsharegmi   (501) staff       (20)        0 2023-04-23 06:21:18.006036 botterino-0.4.8/botterino/Utils/
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)        0 2021-04-08 15:21:02.000000 botterino-0.4.8/botterino/Utils/__init__.py
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     3821 2023-04-23 04:36:39.000000 botterino-0.4.8/botterino/Utils/utils.py
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     1508 2023-04-23 04:36:39.000000 botterino-0.4.8/botterino/__init__.py
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)       36 2023-04-23 04:36:39.000000 botterino-0.4.8/botterino/__main__.py
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     2673 2023-04-23 04:36:39.000000 botterino-0.4.8/botterino/botterino.py
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     3194 2023-04-23 06:14:00.000000 botterino-0.4.8/botterino/config.py
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)      544 2023-04-23 04:36:39.000000 botterino-0.4.8/botterino/failure.py
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     6907 2023-04-23 06:15:17.000000 botterino-0.4.8/botterino/hosterino.py
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     1127 2023-04-23 04:36:40.000000 botterino-0.4.8/botterino/posterino.py
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     4615 2023-04-23 04:36:40.000000 botterino-0.4.8/botterino/ui.py
+drwxr-xr-x   0 adarsharegmi   (501) staff       (20)        0 2023-04-23 06:21:17.994415 botterino-0.4.8/botterino.egg-info/
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     5014 2023-04-23 06:21:17.000000 botterino-0.4.8/botterino.egg-info/PKG-INFO
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)      638 2023-04-23 06:21:17.000000 botterino-0.4.8/botterino.egg-info/SOURCES.txt
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)        1 2023-04-23 06:21:17.000000 botterino-0.4.8/botterino.egg-info/dependency_links.txt
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)       70 2023-04-23 06:21:17.000000 botterino-0.4.8/botterino.egg-info/requires.txt
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)       10 2023-04-23 06:21:17.000000 botterino-0.4.8/botterino.egg-info/top_level.txt
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)      103 2021-06-10 03:23:33.000000 botterino-0.4.8/pyproject.toml
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)      636 2023-04-23 06:21:18.012091 botterino-0.4.8/setup.cfg
```

### Comparing `botterino-0.4.7/LICENSE` & `botterino-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `botterino-0.4.7/PKG-INFO` & `botterino-0.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botterino
-Version: 0.4.7
+Version: 0.4.8
 Summary: Automate posting and hosting of rounds on /r/picturegame
 Home-page: https://github.com/pgitox/botterino
 Author: itoxici
 Author-email: itox@picturegame.co
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `botterino-0.4.7/README.md` & `botterino-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `botterino-0.4.7/botterino/Loader/loader.py` & `botterino-0.4.8/botterino/Loader/loader.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,38 +2,42 @@
 from ..config import roundfile, archivefile
 import ruamel.yaml
 
 yaml = ruamel.yaml.YAML()
 yaml.preserve_quotes = True
 yaml.allow_duplicate_keys = True
 
+
 def dump(data, file):
-    with open(file, 'w', encoding='utf-8') as f:
+    with open(file, "w", encoding="utf-8") as f:
         yaml.dump(data, f)
-        
+
+
 def append(data, file):
-    with open(file, 'r', encoding='utf-8') as f:
+    with open(file, "r", encoding="utf-8") as f:
         x = yaml.load(f)
     if not x:
         dump(data, file)
         return
     x.update(data)
     dump(x, file)
 
+
 def load(file):
-    with open(file, 'r', encoding='utf-8') as f:
+    with open(file, "r", encoding="utf-8") as f:
         return yaml.load(f)
 
+
 def getRound():
     x = load(roundfile)
     if not x:
         return None
     k = next(iter(x))
     top = x.pop(k)
     if x:
         dump(x, roundfile)
     else:
-        open(roundfile, 'w', encoding='utf-8').close()
+        open(roundfile, "w", encoding="utf-8").close()
     y = load(archivefile) or {}
     y[k] = top
     dump(y, archivefile)
     return top
```

### Comparing `botterino-0.4.7/botterino/RedditPoller/RedditPoller.py` & `botterino-0.4.8/botterino/RedditPoller/RedditPoller.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import itertools
 
 from .Retry import retry
 
 POLL_LIMIT = 50
 
+
 class FifoSet:
     def __init__(self, size):
         self.size = size
         self._fifo = []
         self._set = set()
 
     def __contains__(self, item):
@@ -15,24 +16,26 @@
 
     def add(self, item):
         if len(self._set) == self.size:
             self._set.remove(self._fifo.pop(0))
         self._fifo.append(item)
         self._set.add(item)
 
+
 class CommentWrapper:
     def __init__(self, func1, func2):
         self.f1 = func1
         self.f2 = func2
+
     def __call__(self, *args, **kwargs):
         return itertools.chain(self.f1(*args, **kwargs), self.f2(*args, **kwargs))
 
 
 class RedditPoller:
-    def __init__(self, function, before = None):
+    def __init__(self, function, before=None):
         self.function = function
         self.seenNames = FifoSet(POLL_LIMIT * 1000)
         self.beforeName = before
 
     def getLatest(self):
         while True:
             newestName = None
@@ -44,8 +47,10 @@
                 yield item
 
             self.beforeName = newestName
             yield None
 
     @retry
     def _poll(self):
-        return reversed(list(self.function(limit = POLL_LIMIT, params = { "before": self.beforeName })))
+        return reversed(
+            list(self.function(limit=POLL_LIMIT, params={"before": self.beforeName}))
+        )
```

### Comparing `botterino-0.4.7/botterino/RedditPoller/Retry.py` & `botterino-0.4.8/botterino/RedditPoller/Retry.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 
 from praw.exceptions import APIException
 from prawcore.exceptions import BadRequest, ResponseException, RequestException
 from requests.exceptions import ConnectionError
 
 # from ..models import Logger
 
+
 def retry(action):
     def actionWithRetry(*args, **kwargs):
-        '''Perform the given action. If an exception is raised, retry every ten seconds
+        """Perform the given action. If an exception is raised, retry every ten seconds
 
         @param throwOnPayloadTooLarge boolean If a 413 error is caught, throw it instead of retrying (default False)
         Return the return value of the action, if any
-        '''
+        """
 
         failCount = 0
 
         while True:
             try:
                 result = action(*args, **kwargs)
 
@@ -39,15 +40,17 @@
                 #     "responseUrl": e.response.url,
                 #     "requestUrl": e.response.request.url,
                 #     "requestBody": e.response.request.body,
                 # })
                 return
 
             except APIException as e:
-                if e.error_type == "TOO_LONG" and kwargs.get('throwOnPayloadTooLarge', False):
+                if e.error_type == "TOO_LONG" and kwargs.get(
+                    "throwOnPayloadTooLarge", False
+                ):
                     # Logger.warn("Action failed with HTTP status 413, raising", { "action": action.__name__ })
                     raise e
 
                 failCount += 1
 
                 if failCount == 1:
                     pass
```

### Comparing `botterino-0.4.7/botterino/Utils/utils.py` & `botterino-0.4.8/botterino/Utils/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,80 +21,89 @@
 )
 
 # google earth formats, other formats
 everything_else = re.compile(
     """(^| )(-?\d{1,2}(\.\d+)?(?=\s*,?\s*)[\s,]+-?\d{1,3}(\.\d+)?|\d{1,2}(\.\d+°|°(\d{1,2}(\.\d+'|'(\d{1,2}(\.\d+)?\")?))?)[NS](?=\s*,?\s*)[\s,]+\d{1,3}(\.\d+°|°(\d{1,2}(\.\d+'|'(\d{1,2}(\.\d+)?\")?))?)[EW])"""
 )
 
-MAPS_URL = 'https://maps.google.com/maps?t=k&q=loc:{},{}'
+MAPS_URL = "https://maps.google.com/maps?t=k&q=loc:{},{}"
+
+badColors = [0, 16, 17, 18, 22, 52, 88, 90] + list(range(232, 256))
 
-badColors = [0, 16, 17, 18, 22, 52, 88, 90] + list(range(232,256))
 
 def submissions():
-    '''
+    """
     returns a generator of titles of submissions to pg
     newest submissions first
-    '''
+    """
     for submission in reddit.user.me().submissions.new(limit=200):
         if submission.subreddit != pg:
             continue
         yield submission.title
 
+
 def randomColorWithAuthor(author):
     seed = hash(author)
     random.seed(seed)
     color = randrange(256)
     while color in badColors:
         color = (color + 1) % 256
     return fg(color)
 
+
 def randomColor():
     color = randrange(256)
     while color in badColors:
         color = randrange(256)
     return fg(color)
 
+
 def postDelay():
     if debug:
         return -1
 
-    r = requests.get(f'{api}/current')
+    r = requests.get(f"{api}/current")
     data = json.loads(r.content)
     tries = 1
 
-    while data['round']['hostName'].lower() != username.lower():
+    while data["round"]["hostName"].lower() != username.lower():
         tries += 1
         if tries > 5:
             return -1
-        r = requests.get(f'{api}/current')
+        r = requests.get(f"{api}/current")
         data = json.loads(r.content)
         time.sleep(5)
 
-    return data['round'].get('postDelay', -1)
+    return data["round"].get("postDelay", -1)
+
 
 def hyperlink(alias, url):
-    return f'\u001b]8;;{url}\u001b\\{alias}\u001b]8;;\u001b\\'
+    return f"\u001b]8;;{url}\u001b\\{alias}\u001b]8;;\u001b\\"
+
 
 def getRoundPrefix():
-    r = requests.get(f'{api}/current')
-    roundnum = int(json.loads(r.content)['round']['roundNumber']) + 1
-    return f'[Round {roundnum}]'
+    r = requests.get(f"{api}/current")
+    roundnum = int(json.loads(r.content)["round"]["roundNumber"]) + 1
+    return f"[Round {roundnum}]"
+
 
 def approved():
     c = next(iter(pg.contributor()))
     return c and c.name.lower() == username.lower()
 
+
 @retry
-@Halo(spinner='dots', color='yellow')
+@Halo(spinner="dots", color="yellow")
 def waitForApproval(stop=None):
     while not approved() and not stop:
         continue
     if stop:
         return True
 
+
 def getDistance(guess, answer):
     match = re.search(decimal_or_DMS, guess)
     if not match:
         match = re.search(everything_else, guess)
     try:
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
@@ -111,15 +120,24 @@
     rp = RedditPoller(CommentWrapper(pg.comments, reddit.inbox.all))
     comments = rp.getLatest()
     # flush old comments
     while next(comments):
         continue
 
     for c in comments:
-        if hasattr(c, 'submission') and hasattr(c, 'author') and c.author and c.submission:
-            if c.author.name.lower() == username.lower() and '+correct' in c.body and not c.is_root:
+        if (
+            hasattr(c, "submission")
+            and hasattr(c, "author")
+            and c.author
+            and c.submission
+        ):
+            if (
+                c.author.name.lower() == username.lower()
+                and "+correct" in c.body
+                and not c.is_root
+            ):
                 return
             if not c.is_root:
                 continue
             if c.author.name.lower() in donotreply or c.submission != submission:
                 continue
             yield c
```

### Comparing `botterino-0.4.7/botterino/__init__.py` & `botterino-0.4.8/botterino/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 import os
 import json
 from pathlib import Path
 from configparser import ConfigParser
 
-class files():
+
+class files:
     def __init__(self):
-        self.home = os.path.expanduser('~')
-        self.botconfig = os.path.join(self.home, 'botterino-config')
-        self.configfile = os.path.join(self.botconfig, 'config.ini')
-        self.roundsdir = os.path.join(self.botconfig, 'rounds')
-        self.rounds = os.path.join(self.roundsdir, 'rounds.yaml')
-        self.archive = os.path.join(self.roundsdir, 'archive.yaml')
-        self.prawconfig = os.path.join(self.botconfig, 'praw.ini')
-        self.hintfile = os.path.join(self.botconfig, 'hints.txt')
+        self.home = os.path.expanduser("~")
+        self.botconfig = os.path.join(self.home, "botterino-config")
+        self.configfile = os.path.join(self.botconfig, "config.ini")
+        self.roundsdir = os.path.join(self.botconfig, "rounds")
+        self.rounds = os.path.join(self.roundsdir, "rounds.yaml")
+        self.archive = os.path.join(self.roundsdir, "archive.yaml")
+        self.prawconfig = os.path.join(self.botconfig, "praw.ini")
+        self.hintfile = os.path.join(self.botconfig, "hints.txt")
+
 
 botfiles = files()
 dirs = [botfiles.botconfig, botfiles.roundsdir]
 files = [botfiles.rounds, botfiles.archive, botfiles.prawconfig, botfiles.hintfile]
 for d in dirs:
     Path(d).mkdir(parents=True, exist_ok=True)
 for f in files:
-    with open(f, 'a+'):
+    with open(f, "a+"):
         pass
 
 if not os.path.exists(botfiles.configfile):
     parser = ConfigParser()
-    parser.add_section('config')
-    parser.set('config', 'correct_message', '+correct')
-    parser.set('config', 'incorrect_message', '❌')
-    parser.set('config', 'hints', '[25,45]')
-    with open(botfiles.configfile, 'w', encoding='utf-8') as f:
+    parser.add_section("config")
+    parser.set("config", "correct_message", "+correct")
+    parser.set("config", "incorrect_message", "❌")
+    parser.set("config", "hints", "[25,45]")
+    with open(botfiles.configfile, "w", encoding="utf-8") as f:
         parser.write(f)
 
 parser = ConfigParser()
-parser.read(botfiles.configfile, encoding='utf-8')
-correctMessage, incorrectMessage = parser['config']['correct_message'], parser[
-    'config']['incorrect_message']
-hints = json.loads(parser['config'].get('hints', '[]'))
+parser.read(botfiles.configfile, encoding="utf-8")
+correctMessage, incorrectMessage = (
+    parser["config"]["correct_message"],
+    parser["config"]["incorrect_message"],
+)
+hints = json.loads(parser["config"].get("hints", "[]"))
```

### Comparing `botterino-0.4.7/botterino/botterino.py` & `botterino-0.4.8/botterino/botterino.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,60 +5,75 @@
 from .Loader.loader import getRound
 from sty import fg
 from importlib.metadata import version
 from update_checker import UpdateChecker
 from threading import Thread
 import time
 
-v = version('botterino')
+v = version("botterino")
 checker = UpdateChecker()
-result = checker.check('botterino', v)
+result = checker.check("botterino", v)
 if result:
-    print(f'{fg.yellow}{result}')
+    print(f"{fg.yellow}{result}")
     print(f'{fg.yellow}run "pip install --upgrade botterino" to update')
 
+
 def checkType(r):
     types = []
-    if 'tolerance' in r and 'answer' in r:
-        types.append('coordinates')
-    if 'tolerances' in r and 'answers' in r:
-        types.append('multiple coordinates')
-    if 'text' in r and 'similarity' in r:
-        types.append('text match')
-    if 'manual' in r:
-        types.append('x wrong guesses with manual correct')
+    if "tolerance" in r and "answer" in r:
+        types.append("coordinates")
+    if "tolerances" in r and "answers" in r:
+        types.append("multiple coordinates")
+    if "text" in r and "similarity" in r:
+        types.append("text match")
+    if "manual" in r:
+        types.append("x wrong guesses with manual correct")
     if not types:
-        return 'no automatic replies'
-    if 'manual' not in r:
-        types.append('automatic')
-    return ','.join(types)
+        return "no automatic replies"
+    if "manual" not in r:
+        types.append("automatic")
+    return ",".join(types)
+
 
 def main(stop=None):
     while True:
-        print(f'{fg.yellow}Waiting for {username} to win a round... 🐌', end=f'{fg.rs}\n')
+        print(
+            f"{fg.yellow}Waiting for {username} to win a round... 🐌", end=f"{fg.rs}\n"
+        )
         stopped = waitForApproval(stop)
         if stopped or stop:
-            print(f'{fg.red}Stopped botterino{fg.rs}')
+            print(f"{fg.red}Stopped botterino{fg.rs}")
             return
-        print(f'{fg.blue}Congrats on a well deserved win {username}! ⭐', end=f'{fg.rs}\n')
+        print(
+            f"{fg.blue}Congrats on a well deserved win {username}! ⭐", end=f"{fg.rs}\n"
+        )
         r = getRound()
         while not r:
-            print(f'{fg.red}No rounds in round file! checking again in 10s')
+            print(f"{fg.red}No rounds in round file! checking again in 10s")
             time.sleep(10)
             r = getRound()
         submission = submitRound(r)
-        print(f'{randomColor()}Your round was posted to https://reddit.com{submission.permalink}', end=f'{fg.rs}\n')
-        print(f'{fg.magenta}Round \'{r["title"]}\' posted in {postDelay()}s', end=f'{fg.rs}\n')
-        print(f'{fg.cyan}Checking Answers: {checkType(r)}...{fg.rs}', end=f'{fg.rs}\n')
-        H = hints if not r.get('hints') else r.get('hints')
+        print(
+            f"{randomColor()}Your round was posted to https://reddit.com{submission.permalink}",
+            end=f"{fg.rs}\n",
+        )
+        print(
+            f'{fg.magenta}Round \'{r["title"]}\' posted in {postDelay()}s',
+            end=f"{fg.rs}\n",
+        )
+        print(f"{fg.cyan}Checking Answers: {checkType(r)}...{fg.rs}", end=f"{fg.rs}\n")
+        H = hints if not r.get("hints") else r.get("hints")
         CheckAnswers = Thread(target=checkAnswers, args=(r, submission))
         CheckHints = Thread(target=checkHints, args=(H, submission))
         CheckAnswers.start()
         CheckHints.start()
         CheckAnswers.join()
         CheckHints.join()
         while approved():
             continue
-        after = r.get('after')
+        after = r.get("after")
         if after:
             submission.reply(after)
-            print(f'{randomColor()}Posted your message after the round: {after}', end=f'{fg.rs}\n')
+            print(
+                f"{randomColor()}Posted your message after the round: {after}",
+                end=f"{fg.rs}\n",
+            )
```

### Comparing `botterino-0.4.7/botterino/config.py` & `botterino-0.4.8/botterino/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,95 +1,110 @@
 import praw
 import os
 import sys
-from . import botfiles, correctMessage, incorrectMessage, hints
+from . import botfiles
 from sty import fg
 import random
 import webbrowser
 import socket
-from prawcore import exceptions
 
 
 def receive_connection():
     """
     Wait for and then return a connected socket..
     Opens a TCP connection on port 8080, and waits for a single client.
     """
     server = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
     server.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
-    server.bind(('localhost', 8080))
+    server.bind(("localhost", 8080))
     server.listen(1)
     client = server.accept()[0]
     server.close()
     return client
 
 
 def send_message(client, message):
     """
     Send message to client and close the connection.
     """
-    client.send('HTTP/1.1 200 OK\r\n\r\n{}'.format(message).encode('utf-8'))
+    client.send("HTTP/1.1 200 OK\r\n\r\n{}".format(message).encode("utf-8"))
     client.close()
 
 
-if sys.platform == 'win32':
-    os.system('color')
+if sys.platform == "win32":
+    os.system("color")
 
 debug = False
 roundfile = botfiles.rounds
 archivefile = botfiles.archive
 cwd = os.getcwd()
-#FIXME: clean this up
+# FIXME: clean this up
 try:
     os.chdir(botfiles.botconfig)
-    reddit = praw.Reddit('botterino')
+    reddit = praw.Reddit("botterino")
     if reddit.user.me():
-        print(f'{fg.green}Successfully logged into reddit as {reddit.user.me()}', end=f'{fg.rs}\n')
+        print(
+            f"{fg.green}Successfully logged into reddit as {reddit.user.me()}",
+            end=f"{fg.rs}\n",
+        )
     else:
-        print(f'{fg.yellow}Unable to login with username/password. If your account has 2fa continue in browser. Otherwise check {botfiles.prawconfig}', end=f'{fg.rs}\n')
+        print(
+            f"{fg.yellow}Unable to login with username/password. If your account has 2fa continue in browser. Otherwise check {botfiles.prawconfig}",
+            end=f"{fg.rs}\n",
+        )
         os.chdir(botfiles.botconfig)
-        reddit = praw.Reddit(
-            'botterino', redirect_uri='http://localhost:8080')
+        reddit = praw.Reddit("botterino", redirect_uri="http://localhost:8080")
         state = str(random.randint(0, 65000))
-        scopes = ['identity', 'history', 'read',
-                  'edit', 'submit', 'privatemessages']
-        url = reddit.auth.url(scopes, state, 'permanent')
+        scopes = [
+            "identity", "history", "read", "edit", "submit", "privatemessages"
+        ]
+        url = reddit.auth.url(scopes, state, "permanent")
         print(
-            'A window will be opened in the browser to complete the login process to reddit.')
+            "A window will be opened in the browser to complete the login process to reddit."
+        )
         webbrowser.open(url)
 
         client = receive_connection()
-        data = client.recv(1024).decode('utf-8')
-        param_tokens = data.split(' ', 2)[1].split('?', 1)[1].split('&')
-        params = {key: value for (key, value) in [token.split('=')
-                                                  for token in param_tokens]}
-
-        if state != params['state']:
-            send_message(client, 'State mismatch. Expected: {} Received: {}'.format(
-                state, params['state']))
-        elif 'error' in params:
-            send_message(client, params['error'])
+        data = client.recv(1024).decode("utf-8")
+        param_tokens = data.split(" ", 2)[1].split("?", 1)[1].split("&")
+        params = {
+            key: value
+            for (key, value) in [token.split("=") for token in param_tokens]
+        }
+
+        if state != params["state"]:
+            send_message(
+                client,
+                "State mismatch. Expected: {} Received: {}".format(
+                    state, params["state"]),
+            )
+        elif "error" in params:
+            send_message(client, params["error"])
 
         refresh_token = reddit.auth.authorize(params["code"])
         send_message(client, "Refresh token: {}".format(refresh_token))
         print(refresh_token)
         if not reddit.user.me():
-            print(f'{fg.red}Unable to login to reddit. Please check {botfiles.prawconfig}')
+            print(
+                f"{fg.red}Unable to login to reddit. Please check {botfiles.prawconfig}"
+            )
             exit(1)
 except Exception as e:
-    print(f'{fg.red}Unable to login to reddit. Please check {botfiles.prawconfig}')
-    print(f'{fg.red}{e}')
+    print(
+        f"{fg.red}Unable to login to reddit. Please check {botfiles.prawconfig}"
+    )
+    print(f"{fg.red}{e}")
 finally:
     os.chdir(cwd)
 
-pg = reddit.subreddit('itoxtestingfacility' if debug else 'picturegame')
+pg = reddit.subreddit("itoxtestingfacility" if debug else "picturegame")
 
 username = str(reddit.user.me())
 
 donotreply = {
-    'achievements-bot',
+    "achievements-bot",
     username.lower(),
-    'r-picturegame',
-    'imreallycuriousbird',
+    "r-picturegame",
+    "imreallycuriousbird",
 }
 
-api = 'https://api.picturega.me'
+api = "https://api.picturega.me"
```

### Comparing `botterino-0.4.7/botterino/failure.py` & `botterino-0.4.8/botterino/failure.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,17 +4,20 @@
 from .Loader import loader
 from sty import fg
 import time
 
 
 r = loader.getRound()
 while not r:
-    print(f'{fg.red}No rounds in round file! checking again in 10s')
+    print(f"{fg.red}No rounds in round file! checking again in 10s")
     time.sleep(10)
     r = loader.getRound()
 
 submission = next(iter(pg.new()))
-print(f'{randomColor()}Checking answers on https://reddit.com{submission.permalink}', end=f'{fg.rs}\n')
+print(
+    f"{randomColor()}Checking answers on https://reddit.com{submission.permalink}",
+    end=f"{fg.rs}\n",
+)
 checkAnswers(r, submission)
-after = r.get('after')
+after = r.get("after")
 if after:
-    submission.reply(after)
+    submission.reply(after)
```

### Comparing `botterino-0.4.7/botterino/hosterino.py` & `botterino-0.4.8/botterino/hosterino.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,136 +1,227 @@
 from geopy.distance import distance
 from geopy.point import Point
-from .config import donotreply, correctMessage, incorrectMessage, reddit, username, pg, botfiles
+from .config import (
+    correctMessage,
+    incorrectMessage,
+    botfiles,
+)
 from itertools import permutations
 import re
 from sty import fg
-from .Utils.utils import approved, decimal, getComments, getDistance, randomColor, randomColorWithAuthor, MAPS_URL, hyperlink
+from .Utils.utils import (
+    approved,
+    decimal,
+    getComments,
+    getDistance,
+    randomColor,
+    randomColorWithAuthor,
+    MAPS_URL,
+    hyperlink,
+)
 from difflib import SequenceMatcher
+from .Map.map import Map
 import time
 
+
 def withinTolerance(guess, answer, tolerance):
     return distance(guess, answer).m <= tolerance
 
+
 def checkMultipleCoordinates(guess, answers, tolerances):
     guesser = guess.author.name
     answers = [Point(a) for a in answers]
     match = re.findall(decimal, guess.body)
     if len(match) != len(answers):
         # TODO print a message here
-        print(f'{randomColorWithAuthor(guesser)}{guesser}\'s guess {guess.body} was incorrect', end=f'{fg.rs}\n')
+        print(
+            f"{randomColorWithAuthor(guesser)}{guesser}'s guess {guess.body} was incorrect",
+            end=f"{fg.rs}\n",
+        )
         return False
     try:
-        points = [Point(f'{lat},{lon}') for lat, lon in match]
+        points = [Point(f"{lat},{lon}") for lat, lon in match]
         points = permutations(points)
     except Exception as e:
-        print(f'{randomColor()}Something happened: ', e, 'it probably does not matter')
+        print(f"{randomColor()}Something happened: ", e,
+              "it probably does not matter")
         return False
 
-    results = [[withinTolerance(p, a, t) for p, a, t in zip(ps, answers, tolerances)] for ps in points]
+    results = [[
+        withinTolerance(p, a, t) for p, a, t in zip(ps, answers, tolerances)
+    ] for ps in points]
     results = [all(r) for r in results]
     result = any(results)
     if not result:
-        print(f'{randomColorWithAuthor(guesser)}{guesser}\'s guess {guess.body} was incorrect')
+        print(
+            f"{randomColorWithAuthor(guesser)}{guesser}'s guess {guess.body} was incorrect"
+        )
     return result
 
-def checkCoordinates(guess, answer, tolerance):
+
+def checkCoordinates(guess, answer, tolerance, map):
     guesser = guess.author.name
     answer = Point(answer)
     errorAndPoint = getDistance(guess.body, answer)
     error, point = errorAndPoint if errorAndPoint else (None, None)
     if error is None:
-        print(f"{randomColorWithAuthor(guesser)}Could not find a coordinate in guess '{guess.body}' by {guesser}", end=f'{fg.rs}\n')
-        return 'ignore'
+        print(
+            f"{randomColorWithAuthor(guesser)}Could not find a coordinate in guess '{guess.body}' by {guesser}",
+            end=f"{fg.rs}\n",
+        )
+        return "ignore"
     error = round(error, 2)
     mapslink = MAPS_URL.format(point.latitude, point.longitude)
     color = fg.green if error <= tolerance else randomColorWithAuthor(guesser)
-    pl = ''
-    if hasattr(guess, 'context'):
+    pl = ""
+    if hasattr(guess, "context"):
         pl = guess.context
-    elif hasattr(guess, 'permalink'):
+    elif hasattr(guess, "permalink"):
         pl = guess.permalink
-    commentlink = f'https://reddit.com{pl}'
+    commentLink = f"https://reddit.com{pl}"
     if error < 1000:
-        print(f'{color}{guesser}\'s {hyperlink("guess", commentlink)} was {error}m {hyperlink("off", mapslink)}', end=f'{fg.rs}\n')
+        print(
+            f'{color}{guesser}\'s {hyperlink("guess", commentLink)} was {error}m {hyperlink("off", mapslink)}',
+            end=f"{fg.rs}\n",
+        )
     else:
-        print(f'{color}{guesser}\'s {hyperlink("guess", commentlink)} was {round(error/1000,2)}km {hyperlink("off", mapslink)}', end=f'{fg.rs}\n')
+        print(
+            f'{color}{guesser}\'s {hyperlink("guess", commentLink)} was {round(error/1000,2)}km {hyperlink("off", mapslink)}',
+            end=f"{fg.rs}\n",
+        )
+
+    if map:
+        # TODO: try to give different users differnt colors
+        map.addPoint(point.latitude, point.longitude, guesser, error,
+                     commentLink, "red" if error > tolerance else "green")
+
     return error <= tolerance
 
+
 def checkText(guess, answer, tolerance, ignorecase):
     guesser = guess.author.name
-    text = guess.body.strip().replace('\\', '')
+    text = guess.body.strip().replace("\\", "")
 
     if ignorecase:
-        text,answer = text.lower(), answer.lower()
+        text, answer = text.lower(), answer.lower()
 
     similarity = SequenceMatcher(None, text, answer).ratio()
-    print(f'{randomColorWithAuthor(guesser)}{guesser}\'s guess was {round(similarity * 100, 3)}% similar to the correct answer', end=f'{fg.rs}\n')
+    print(
+        f"{randomColorWithAuthor(guesser)}{guesser}'s guess was {round(similarity * 100, 3)}% similar to the correct answer",
+        end=f"{fg.rs}\n",
+    )
     return similarity >= tolerance
 
+
 def postHint(submission, time):
-    with open(botfiles.hintfile, 'r') as F:
+    with open(botfiles.hintfile, "r") as F:
         hintText = F.read()
     if not hintText:
-        print(f'{fg.yellow}Skipping {time}m hint: hints.txt is empty')
+        print(f"{fg.yellow}Skipping {time}m hint: hints.txt is empty")
         return
-    hint = submission.reply(f'Hint({time}m): {hintText}')
-    print(f'{fg.green}Posted hint ({time}m) to https://reddit.com{hint.permalink}')
-    open(botfiles.hintfile, 'w').close()
+    hint = submission.reply(f"Hint({time}m): {hintText}")
+    print(
+        f"{fg.green}Posted hint ({time}m) to https://reddit.com{hint.permalink}"
+    )
+    open(botfiles.hintfile, "w").close()
+
 
 def checkHints(hints, submission):
     hints = list(hints)
     hints += [60, 120, 180, 240]
     hints = sorted(list(set(hints)))
     while hints and approved():
         top = hints[0]
         duration = int(time.time() - submission.created_utc)
-        duration = duration//60
+        duration = duration // 60
         if duration >= top:
             postHint(submission, duration)
             hints.pop(0)
         time.sleep(10)
         pass
 
+
 def checkAnswers(r, submission):
-    tolerance, manual, text, answer, tolerances, answers, similarity, ignorecase, hints, = r.get(
-        'tolerance'), r.get('manual'), r.get('text'), r.get(
-            'answer'), r.get('tolerances'), r.get('answers'), r.get(
-                'similarity'), r.get('ignorecase'), r.get('hints', [])
+    (
+        tolerance,
+        manual,
+        text,
+        answer,
+        tolerances,
+        answers,
+        similarity,
+        ignorecase,
+    ) = (
+        r.get("tolerance"),
+        r.get("manual"),
+        r.get("text"),
+        r.get("answer"),
+        r.get("tolerances"),
+        r.get("answers"),
+        r.get("similarity"),
+        r.get("ignorecase"),
+    )
+
+    answerPlot = None
+    if answer and tolerance and not answers:
+        try:
+            answerPoint = Point(answer)
+            answerPlot = Map(answerPoint.latitude, answerPoint.longitude)
+        except Exception:
+            pass
 
     if tolerance is None and tolerances is None and text is None:
         return
 
     for c in getComments(submission):
         result = True
         if tolerance is not None:
             tolerance = float(tolerance)
-            r = checkCoordinates(c, answer, tolerance)
-            if r == 'ignore':
+            r = checkCoordinates(c, answer, tolerance, answerPlot)
+            if r == "ignore":
                 continue
             result = result and r
         elif tolerances:
-            tolerances = [float(t) for t in r['tolerances']]
+            tolerances = [float(t) for t in r["tolerances"]]
             if len(answers) != len(tolerances):
-                print('{fg.red}Refusing to check answers, number of tolerances must equal number of answers.', end=f'{fg.rs}\n')
-            result = result and checkMultipleCoordinates(c, answers, tolerances)
+                print(
+                    "{fg.red}Refusing to check answers, number of tolerances must equal number of answers.",
+                    end=f"{fg.rs}\n",
+                )
+            result = result and checkMultipleCoordinates(
+                c, answers, tolerances)
 
         if text and similarity is None:
             continue
 
         if ignorecase is None:
             ignorecase = True
 
         if text:
             result = result and checkText(c, text, similarity, ignorecase)
 
         if not result:
             c.reply(incorrectMessage)
         if result:
             if manual:
-                print(f"{randomColor()}Guess '{c.body}' looks correct, but you will have to check it out.", end=f'{fg.rs}\n')
+                print(
+                    f"{randomColor()}Guess '{c.body}' looks correct, but you will have to check it out.",
+                    end=f"{fg.rs}\n",
+                )
             else:
                 plusCorrect = c.reply(correctMessage)
                 guesser = c.author.name
                 print(
-                    f'{fg.green}Corrected {guesser} in {plusCorrect.created_utc - c.created_utc}s', end=f'{fg.rs}\n')
+                    f"{fg.green}Corrected {guesser} in {plusCorrect.created_utc - c.created_utc}s",
+                    end=f"{fg.rs}\n",
+                )
                 break
+
+    # TODO: show the map on every guess instead of only when the round is over
+    if answerPlot:
+        answerPlot.saveMap()
+        outputFile = answerPlot.getFilePath()
+        if outputFile:
+            print(
+                f'{fg.green}Answers to your round plotted at {outputFile}{fg.rs}'
+            )
+            answerPlot.openMapInBrowser()
```

### Comparing `botterino-0.4.7/botterino/posterino.py` & `botterino-0.4.8/botterino/posterino.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 import math
 from .config import pg
 from .Utils.utils import randomColor, getRoundPrefix, submissions
 from sty import fg
 import time
 import re
 
+
 def getSeriesPrefix(name):
     if not name:
-        return ''
+        return ""
     name = name.strip()
-    indefinite = re.compile(f'\s*{name}\s*#?\s*(\d+)\s*')
-    definite = re.compile(f'\s*{name}\s*#?\s*(\d+)\s*\/\s*(\d+)\s*')
+    indefinite = re.compile(f"\s*{name}\s*#?\s*(\d+)\s*")
+    definite = re.compile(f"\s*{name}\s*#?\s*(\d+)\s*\/\s*(\d+)\s*")
     for title in submissions():
         defmatch = re.search(definite, title)
         if defmatch:
-            return f'[{name} #{int(defmatch.group(1)) + 1}/{defmatch.group(2)}]'
+            return f"[{name} #{int(defmatch.group(1)) + 1}/{defmatch.group(2)}]"
         indefmatch = re.search(indefinite, title)
         if indefmatch:
-            return f'[{name} #{int(indefmatch.group(1)) + 1}]'
-    return f'[{name} #1]'
+            return f"[{name} #{int(indefmatch.group(1)) + 1}]"
+    return f"[{name} #1]"
+
 
 def submitRound(r):
-    series_prefix = getSeriesPrefix(r.get('series'))
+    series_prefix = getSeriesPrefix(r.get("series"))
     title = f'{getRoundPrefix()} {series_prefix} {r["title"]}'
-    submission = pg.submit(title=title,
-                           url=r['url'].strip())
+    submission = pg.submit(title=title, url=r["url"].strip())
 
-    message = r.get('message')
+    message = r.get("message")
     if message is not None:
         time.sleep(15)
         submission.reply(message)
 
-        print(f'{randomColor()}Message posted to thread: {message}', end=f'{fg.rs}\n')
+        print(f"{randomColor()}Message posted to thread: {message}", end=f"{fg.rs}\n")
 
-    return submission
+    return submission
```

### Comparing `botterino-0.4.7/botterino/ui.py` & `botterino-0.4.8/botterino/ui.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,34 +9,42 @@
 root = Tk()
 root.title("Botterino")
 
 # Todo: place this in a sensible place
 class Stopper:
     def __init__(self):
         self.stopped = False
+
     def __bool__(self):
         return self.stopped
+
     def stop(self):
         self.stopped = True
+
     def unstop(self):
         self.stopped = False
 
+
 class Runner:
     def __init__(self):
         self.stopper = Stopper()
         self.T = Thread(target=main, args=(self.stopper,))
+
     def start(self):
         self.stopper.unstop()
         self.T.start()
+
     def stop(self):
         self.stopper.stop()
         self.T = Thread(target=main, args=(self.stopper,))
 
+
 R = Runner()
 
+
 def append_entry():
     name_input = str(name.get())
     if not name_input:
         error_text.set("Name is missing")
         return
     d = load(roundfile)
     if d and name_input in d:
@@ -73,48 +81,52 @@
     if url_input:
         inner["url"] = url_input
     if manual_input:
         inner["manual"] = manual_input
     data[name_input] = inner
     append(data, roundfile)
     clear_entries()
-    print(f'{fg.green}Added round {name_input} to rounds.yaml{fg.rs}')
+    print(f"{fg.green}Added round {name_input} to rounds.yaml{fg.rs}")
+
 
 def clear_entries():
     name_entry.delete(0, END)
     title_entry.delete(0, END)
     answer_entry.delete(0, END)
     tolerance_entry.delete(0, END)
     url_entry.delete(0, END)
     error_text.set("")
     manual.set(False)
 
+
 def start_botterino():
-    #dummy function to start botterino
+    # dummy function to start botterino
     R.start()
 
+
 def stop_botterino():
-    #dummy function to end botterino
+    # dummy function to end botterino
     R.stop()
 
+
 mainframe = ttk.Frame(root, padding="3 6 3 12")
 mainframe.grid(column=0, row=0, sticky=(N, W, E, S))
 root.columnconfigure(0, weight=1)
 root.rowconfigure(0, weight=1)
 
 ttk.Label(mainframe, text="Name").grid(column=1, row=1, sticky=W)
 ttk.Label(mainframe, text="Title").grid(column=1, row=2, sticky=W)
 ttk.Label(mainframe, text="Answer").grid(column=1, row=3, sticky=W)
 ttk.Label(mainframe, text="Tolerance").grid(column=1, row=4, sticky=W)
 ttk.Label(mainframe, text="URL").grid(column=1, row=5, sticky=W)
 ttk.Label(mainframe, text="Manual").grid(column=1, row=6, sticky=W)
 
 error_text = StringVar()
 error_label = ttk.Label(mainframe, foreground="red", textvariable=error_text)
-error_label.grid(column=1, row=7, sticky=(W,E))
+error_label.grid(column=1, row=7, sticky=(W, E))
 
 name = StringVar()
 name_entry = ttk.Entry(mainframe, width=50, textvariable=name)
 name_entry.grid(column=2, row=1, sticky=(W, E))
 
 title = StringVar()
 title_entry = ttk.Entry(mainframe, width=50, textvariable=title)
@@ -132,17 +144,24 @@
 url_entry = ttk.Entry(mainframe, width=50, textvariable=url)
 url_entry.grid(column=2, row=5, sticky=(W, E))
 
 manual = BooleanVar(value=False)
 manual_entry = ttk.Checkbutton(mainframe, variable=manual, onvalue=True, offvalue=False)
 manual_entry.grid(column=2, row=6, sticky=(W, E))
 
-ttk.Button(mainframe, text="Clear", command=clear_entries).grid(column=2, row=7, sticky=W)
-ttk.Button(mainframe, text="Submit", command=append_entry).grid(column=2, row=7, sticky=E)
-ttk.Button(mainframe, text="Start", command=start_botterino).grid(column=2, row=8, sticky=W)
-ttk.Button(mainframe, text="Stop", command=stop_botterino).grid(column=2, row=8, sticky=E)
+ttk.Button(mainframe, text="Clear", command=clear_entries).grid(
+    column=2, row=7, sticky=W
+)
+ttk.Button(mainframe, text="Submit", command=append_entry).grid(
+    column=2, row=7, sticky=E
+)
+ttk.Button(mainframe, text="Start", command=start_botterino).grid(
+    column=2, row=8, sticky=W
+)
+ttk.Button(mainframe, text="Stop", command=stop_botterino).grid(
+    column=2, row=8, sticky=E
+)
 
 for child in mainframe.winfo_children():
     child.grid_configure(padx=5, pady=2)
 
 root.mainloop()
-
```

### Comparing `botterino-0.4.7/botterino.egg-info/PKG-INFO` & `botterino-0.4.8/botterino.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botterino
-Version: 0.4.7
+Version: 0.4.8
 Summary: Automate posting and hosting of rounds on /r/picturegame
 Home-page: https://github.com/pgitox/botterino
 Author: itoxici
 Author-email: itox@picturegame.co
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `botterino-0.4.7/botterino.egg-info/SOURCES.txt` & `botterino-0.4.8/botterino.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -13,12 +13,14 @@
 botterino.egg-info/PKG-INFO
 botterino.egg-info/SOURCES.txt
 botterino.egg-info/dependency_links.txt
 botterino.egg-info/requires.txt
 botterino.egg-info/top_level.txt
 botterino/Loader/__init__.py
 botterino/Loader/loader.py
+botterino/Map/__init__.py
+botterino/Map/map.py
 botterino/RedditPoller/RedditPoller.py
 botterino/RedditPoller/Retry.py
 botterino/RedditPoller/__init__.py
 botterino/Utils/__init__.py
 botterino/Utils/utils.py
```

### Comparing `botterino-0.4.7/setup.cfg` & `botterino-0.4.8/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = botterino
-version = 0.4.7
+version = 0.4.8
 author = itoxici
 author_email = itox@picturegame.co
 description = Automate posting and hosting of rounds on /r/picturegame
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pgitox/botterino
 classifiers = 
@@ -13,14 +13,15 @@
 	Operating System :: OS Independent
 
 [options]
 packages = find:
 python_requires = >=3.8
 include_package_data = True
 install_requires = 
+	folium
 	praw
 	geopy
 	pyyaml
 	ruamel.yaml
 	sty
 	requests
 	update_checker
```

