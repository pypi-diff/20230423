# Comparing `tmp/twitter-api-client-0.7.2.tar.gz` & `tmp/twitter-api-client-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitter-api-client-0.7.2.tar", last modified: Fri Apr 21 23:31:46 2023, max compression
+gzip compressed data, was "twitter-api-client-0.7.3.tar", last modified: Sun Apr 23 01:47:00 2023, max compression
```

## Comparing `twitter-api-client-0.7.2.tar` & `twitter-api-client-0.7.3.tar`

### file list

```diff
@@ -1,24 +1,19 @@
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-21 23:31:46.213567 twitter-api-client-0.7.2/
--rw-r--r--   0 x         (1000) x         (1000)     1075 2023-04-17 21:53:35.000000 twitter-api-client-0.7.2/LICENSE
--rw-r--r--   0 x         (1000) x         (1000)     6933 2023-04-21 23:31:46.213567 twitter-api-client-0.7.2/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)       38 2023-04-21 23:31:46.213567 twitter-api-client-0.7.2/setup.cfg
--rw-r--r--   0 x         (1000) x         (1000)     8239 2023-04-21 23:31:42.000000 twitter-api-client-0.7.2/setup.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-21 23:31:46.213567 twitter-api-client-0.7.2/twitter/
--rw-r--r--   0 x         (1000) x         (1000)        0 2023-04-17 21:53:35.000000 twitter-api-client-0.7.2/twitter/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)    21689 2023-04-21 23:27:09.000000 twitter-api-client-0.7.2/twitter/account.py
--rw-r--r--   0 x         (1000) x         (1000)    27260 2023-04-19 22:52:46.000000 twitter-api-client-0.7.2/twitter/constants.py
--rw-r--r--   0 x         (1000) x         (1000)     5501 2023-04-21 22:39:59.000000 twitter-api-client-0.7.2/twitter/login.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-21 23:31:46.213567 twitter-api-client-0.7.2/twitter/noauth/
--rw-r--r--   0 x         (1000) x         (1000)        0 2023-04-17 21:53:35.000000 twitter-api-client-0.7.2/twitter/noauth/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)     2567 2023-04-19 22:52:46.000000 twitter-api-client-0.7.2/twitter/noauth/operation.py
--rw-r--r--   0 x         (1000) x         (1000)     7398 2023-04-21 23:29:07.000000 twitter-api-client-0.7.2/twitter/noauth/scraper.py
--rw-r--r--   0 x         (1000) x         (1000)     2852 2023-04-17 21:53:35.000000 twitter-api-client-0.7.2/twitter/noauth/util.py
--rw-r--r--   0 x         (1000) x         (1000)    10604 2023-04-21 23:27:09.000000 twitter-api-client-0.7.2/twitter/scraper.py
--rw-r--r--   0 x         (1000) x         (1000)     4469 2023-04-21 23:25:19.000000 twitter-api-client-0.7.2/twitter/search.py
--rw-r--r--   0 x         (1000) x         (1000)     3277 2023-04-21 23:31:42.000000 twitter-api-client-0.7.2/twitter/util.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-21 23:31:46.213567 twitter-api-client-0.7.2/twitter_api_client.egg-info/
--rw-r--r--   0 x         (1000) x         (1000)     6933 2023-04-21 23:31:46.000000 twitter-api-client-0.7.2/twitter_api_client.egg-info/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)      459 2023-04-21 23:31:46.000000 twitter-api-client-0.7.2/twitter_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 x         (1000) x         (1000)        1 2023-04-21 23:31:46.000000 twitter-api-client-0.7.2/twitter_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 x         (1000) x         (1000)       79 2023-04-21 23:31:46.000000 twitter-api-client-0.7.2/twitter_api_client.egg-info/requires.txt
--rw-r--r--   0 x         (1000) x         (1000)        8 2023-04-21 23:31:46.000000 twitter-api-client-0.7.2/twitter_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-23 01:47:00.416847 twitter-api-client-0.7.3/
+-rw-r--r--   0 x         (1000) x         (1000)     1075 2023-04-17 21:53:35.000000 twitter-api-client-0.7.3/LICENSE
+-rw-r--r--   0 x         (1000) x         (1000)     6391 2023-04-23 01:47:00.416847 twitter-api-client-0.7.3/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)       38 2023-04-23 01:47:00.416847 twitter-api-client-0.7.3/setup.cfg
+-rw-r--r--   0 x         (1000) x         (1000)     7621 2023-04-23 01:46:44.000000 twitter-api-client-0.7.3/setup.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-23 01:47:00.416847 twitter-api-client-0.7.3/twitter/
+-rw-r--r--   0 x         (1000) x         (1000)        0 2023-04-17 21:53:35.000000 twitter-api-client-0.7.3/twitter/__init__.py
+-rw-r--r--   0 x         (1000) x         (1000)    21689 2023-04-22 23:30:33.000000 twitter-api-client-0.7.3/twitter/account.py
+-rw-r--r--   0 x         (1000) x         (1000)    27260 2023-04-19 22:52:46.000000 twitter-api-client-0.7.3/twitter/constants.py
+-rw-r--r--   0 x         (1000) x         (1000)     5501 2023-04-21 22:39:59.000000 twitter-api-client-0.7.3/twitter/login.py
+-rw-r--r--   0 x         (1000) x         (1000)    10624 2023-04-22 23:27:35.000000 twitter-api-client-0.7.3/twitter/scraper.py
+-rw-r--r--   0 x         (1000) x         (1000)     4469 2023-04-21 23:25:19.000000 twitter-api-client-0.7.3/twitter/search.py
+-rw-r--r--   0 x         (1000) x         (1000)     3277 2023-04-21 23:31:42.000000 twitter-api-client-0.7.3/twitter/util.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-23 01:47:00.416847 twitter-api-client-0.7.3/twitter_api_client.egg-info/
+-rw-r--r--   0 x         (1000) x         (1000)     6391 2023-04-23 01:47:00.000000 twitter-api-client-0.7.3/twitter_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)      355 2023-04-23 01:47:00.000000 twitter-api-client-0.7.3/twitter_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 x         (1000) x         (1000)        1 2023-04-23 01:47:00.000000 twitter-api-client-0.7.3/twitter_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 x         (1000) x         (1000)       79 2023-04-23 01:47:00.000000 twitter-api-client-0.7.3/twitter_api_client.egg-info/requires.txt
+-rw-r--r--   0 x         (1000) x         (1000)        8 2023-04-23 01:47:00.000000 twitter-api-client-0.7.3/twitter_api_client.egg-info/top_level.txt
```

### Comparing `twitter-api-client-0.7.2/LICENSE` & `twitter-api-client-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.2/PKG-INFO` & `twitter-api-client-0.7.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.7.2
+Version: 0.7.3
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
@@ -201,33 +201,14 @@
     444444,
 ])
 
 # trends
 scraper.trends()
 ```
 
-#### Get user/tweet data (no auth)
-
-```python
-from twitter.noauth.scraper import Scraper
-
-scraper = Scraper()
-
-users = scraper.users(['foo', 'bar', 'baz'])
-users = scraper.users_by_id([123, 234, 345])
-users = scraper.users_by_ids([123, 234, 345])  # special batch query
-
-tweets = scraper.tweets_by_id([987, 876, 765])  # condensed
-tweets = scraper.tweets_details([987, 876, 765])
-
-user_tweets = scraper.tweets([123, 234, 345])
-user_tweets_replies = scraper.tweets_and_replies([123, 234, 345])
-user_media = scraper.media([123, 234, 345])
-```
-
 #### Search
 
 ```python   
 from twitter.search import Search
 
 email, username, password = ..., ..., ...
 search = Search(email, username, password)
```

### Comparing `twitter-api-client-0.7.2/setup.py` & `twitter-api-client-0.7.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "tqdm",
     "orjson",
     'uvloop; platform_system != "Windows"',
 ]
 
 setup(
     name="twitter-api-client",
-    version="0.7.2",
+    version="0.7.3",
     python_requires=">=3.11.0",
     description="Twitter API",
     long_description=dedent('''
     Complete implementation of the undocumented Twitter API
     
     Includes tools to **scrape**, **automate**, and **search** twitter
     
@@ -207,33 +207,14 @@
         444444,
     ])
     
     # trends
     scraper.trends()
     ```
     
-    #### Get user/tweet data (no auth)
-    
-    ```python
-    from twitter.noauth.scraper import Scraper
-    
-    scraper = Scraper()
-    
-    users = scraper.users(['foo', 'bar', 'baz'])
-    users = scraper.users_by_id([123, 234, 345])
-    users = scraper.users_by_ids([123, 234, 345])  # special batch query
-    
-    tweets = scraper.tweets_by_id([987, 876, 765])  # condensed
-    tweets = scraper.tweets_details([987, 876, 765])
-    
-    user_tweets = scraper.tweets([123, 234, 345])
-    user_tweets_replies = scraper.tweets_and_replies([123, 234, 345])
-    user_media = scraper.media([123, 234, 345])
-    ```
-    
     #### Search
     
     ```python   
     from twitter.search import Search
     
     email, username, password = ..., ..., ...
     search = Search(email, username, password)
```

### Comparing `twitter-api-client-0.7.2/twitter/account.py` & `twitter-api-client-0.7.3/twitter/account.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         self.debug = debug
 
     def gql(self, method: str, operation: tuple, variables: dict, features: dict = Operation.default_features) -> dict:
         qid, op = operation
         params = {
             'queryId': qid,
             'features': features,
-            'variables': variables | Operation.default_variables
+            'variables': Operation.default_variables | variables
         }
         if method == 'POST':
             data = {'json': params}
         else:
             data = {'params': {k: orjson.dumps(v).decode() for k, v in params.items()}}
         r = self.session.request(
             method=method,
```

### Comparing `twitter-api-client-0.7.2/twitter/constants.py` & `twitter-api-client-0.7.3/twitter/constants.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.2/twitter/login.py` & `twitter-api-client-0.7.3/twitter/login.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.2/twitter/scraper.py` & `twitter-api-client-0.7.3/twitter/scraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import math
 import platform
 import time
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from pathlib import Path
 from urllib.parse import urlsplit
 
+import httpx
 import orjson
 from httpx import AsyncClient, Response
 from tqdm import tqdm
 
 from .constants import *
 from .login import login
 from .util import find_key, save_data, get_cursor, get_headers, set_qs, fmt_status
@@ -98,15 +99,15 @@
         """
         Get user data in batches
 
         Batch-size limited to around 200-300 users
         """
         qid, op, k = Operation.UsersByRestIds
         params = {k: orjson.dumps(v).decode() for k, v in {
-            'variables': {k: user_ids} | Operation.default_variables,
+            'variables': Operation.default_variables | {k: user_ids},
             'features': Operation.default_features,
         }.items()}
         r = self.session.get(f'{self.api}/{qid}/{op}', headers=get_headers(self.session), params=params)
         txt = r.text
         data = r.json()
         if self.debug:
             self.log(r, txt, data)
@@ -158,15 +159,15 @@
 
             res.append(data)
         return res
 
     async def _query(self, session: AsyncClient, _id: int | str | list, operation: tuple, **kwargs) -> Response:
         qid, op, k = operation
         params = {k: orjson.dumps(v).decode() for k, v in {
-            'variables': {k: _id} | kwargs | Operation.default_variables,
+            'variables': {k: _id} | Operation.default_variables | kwargs,
             'features': Operation.default_features,
         }.items()}
         r = await session.get(f'{self.api}/{qid}/{op}', params=params)
         txt = r.text
         data = r.json()
         if self.debug:
             self.log(r, txt, data)
@@ -196,18 +197,18 @@
                     pbar.update()
 
     def _download(self, post_url: str, cdn_url: str, path: str = 'media', chunk_size: int = 4096) -> None:
         Path(path).mkdir(parents=True, exist_ok=True)
         name = urlsplit(post_url).path.replace('/', '_')[1:]
         ext = urlsplit(cdn_url).path.split('/')[-1]
         try:
-            r = self.session.get(cdn_url, stream=True)
-            with open(f'{path}/{name}_{ext}', 'wb') as f:
-                for chunk in r.iter_content(chunk_size=chunk_size):
-                    f.write(chunk)
+            with httpx.stream('GET', cdn_url) as r:
+                with open(f'{path}/{name}_{ext}', 'wb') as f:
+                    for chunk in r.iter_bytes(chunk_size=chunk_size):
+                        f.write(chunk)
         except Exception as e:
             logger.debug(f'[{RED}error{RESET}] failed to download media: {post_url} {e}')
 
     def trends(self) -> dict:
         """Get trends for all UTC offsets"""
 
         def get_trends(offset: str, url: str, headers: dict):
```

### Comparing `twitter-api-client-0.7.2/twitter/search.py` & `twitter-api-client-0.7.3/twitter/search.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.2/twitter/util.py` & `twitter-api-client-0.7.3/twitter/util.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.2/twitter_api_client.egg-info/PKG-INFO` & `twitter-api-client-0.7.3/twitter_api_client.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.7.2
+Version: 0.7.3
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
@@ -201,33 +201,14 @@
     444444,
 ])
 
 # trends
 scraper.trends()
 ```
 
-#### Get user/tweet data (no auth)
-
-```python
-from twitter.noauth.scraper import Scraper
-
-scraper = Scraper()
-
-users = scraper.users(['foo', 'bar', 'baz'])
-users = scraper.users_by_id([123, 234, 345])
-users = scraper.users_by_ids([123, 234, 345])  # special batch query
-
-tweets = scraper.tweets_by_id([987, 876, 765])  # condensed
-tweets = scraper.tweets_details([987, 876, 765])
-
-user_tweets = scraper.tweets([123, 234, 345])
-user_tweets_replies = scraper.tweets_and_replies([123, 234, 345])
-user_media = scraper.media([123, 234, 345])
-```
-
 #### Search
 
 ```python   
 from twitter.search import Search
 
 email, username, password = ..., ..., ...
 search = Search(email, username, password)
```

