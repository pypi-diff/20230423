# Comparing `tmp/twitter-api-client-0.7.4.tar.gz` & `tmp/twitter-api-client-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitter-api-client-0.7.4.tar", last modified: Sun Apr 23 02:06:02 2023, max compression
+gzip compressed data, was "twitter-api-client-0.7.5.tar", last modified: Sun Apr 23 03:57:02 2023, max compression
```

## Comparing `twitter-api-client-0.7.4.tar` & `twitter-api-client-0.7.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-23 02:06:02.484122 twitter-api-client-0.7.4/
--rw-r--r--   0 x         (1000) x         (1000)     1075 2023-04-17 21:53:35.000000 twitter-api-client-0.7.4/LICENSE
--rw-r--r--   0 x         (1000) x         (1000)     6490 2023-04-23 02:06:02.484122 twitter-api-client-0.7.4/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)       38 2023-04-23 02:06:02.484122 twitter-api-client-0.7.4/setup.cfg
--rw-r--r--   0 x         (1000) x         (1000)     7736 2023-04-23 02:05:42.000000 twitter-api-client-0.7.4/setup.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-23 02:06:02.484122 twitter-api-client-0.7.4/twitter/
--rw-r--r--   0 x         (1000) x         (1000)        0 2023-04-17 21:53:35.000000 twitter-api-client-0.7.4/twitter/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)    21689 2023-04-22 23:30:33.000000 twitter-api-client-0.7.4/twitter/account.py
--rw-r--r--   0 x         (1000) x         (1000)    27271 2023-04-23 02:05:42.000000 twitter-api-client-0.7.4/twitter/constants.py
--rw-r--r--   0 x         (1000) x         (1000)     5501 2023-04-21 22:39:59.000000 twitter-api-client-0.7.4/twitter/login.py
--rw-r--r--   0 x         (1000) x         (1000)    11326 2023-04-23 02:02:26.000000 twitter-api-client-0.7.4/twitter/scraper.py
--rw-r--r--   0 x         (1000) x         (1000)     4469 2023-04-21 23:25:19.000000 twitter-api-client-0.7.4/twitter/search.py
--rw-r--r--   0 x         (1000) x         (1000)     3277 2023-04-21 23:31:42.000000 twitter-api-client-0.7.4/twitter/util.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-23 02:06:02.484122 twitter-api-client-0.7.4/twitter_api_client.egg-info/
--rw-r--r--   0 x         (1000) x         (1000)     6490 2023-04-23 02:06:02.000000 twitter-api-client-0.7.4/twitter_api_client.egg-info/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)      355 2023-04-23 02:06:02.000000 twitter-api-client-0.7.4/twitter_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 x         (1000) x         (1000)        1 2023-04-23 02:06:02.000000 twitter-api-client-0.7.4/twitter_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 x         (1000) x         (1000)       79 2023-04-23 02:06:02.000000 twitter-api-client-0.7.4/twitter_api_client.egg-info/requires.txt
--rw-r--r--   0 x         (1000) x         (1000)        8 2023-04-23 02:06:02.000000 twitter-api-client-0.7.4/twitter_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-23 03:57:02.877258 twitter-api-client-0.7.5/
+-rw-r--r--   0 x         (1000) x         (1000)     1075 2023-04-17 21:53:35.000000 twitter-api-client-0.7.5/LICENSE
+-rw-r--r--   0 x         (1000) x         (1000)     6490 2023-04-23 03:57:02.877258 twitter-api-client-0.7.5/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)       38 2023-04-23 03:57:02.877258 twitter-api-client-0.7.5/setup.cfg
+-rw-r--r--   0 x         (1000) x         (1000)     7736 2023-04-23 03:56:44.000000 twitter-api-client-0.7.5/setup.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-23 03:57:02.877258 twitter-api-client-0.7.5/twitter/
+-rw-r--r--   0 x         (1000) x         (1000)        0 2023-04-17 21:53:35.000000 twitter-api-client-0.7.5/twitter/__init__.py
+-rw-r--r--   0 x         (1000) x         (1000)    21689 2023-04-22 23:30:33.000000 twitter-api-client-0.7.5/twitter/account.py
+-rw-r--r--   0 x         (1000) x         (1000)    27271 2023-04-23 02:05:42.000000 twitter-api-client-0.7.5/twitter/constants.py
+-rw-r--r--   0 x         (1000) x         (1000)     5501 2023-04-21 22:39:59.000000 twitter-api-client-0.7.5/twitter/login.py
+-rw-r--r--   0 x         (1000) x         (1000)    11158 2023-04-23 03:55:18.000000 twitter-api-client-0.7.5/twitter/scraper.py
+-rw-r--r--   0 x         (1000) x         (1000)     4469 2023-04-21 23:25:19.000000 twitter-api-client-0.7.5/twitter/search.py
+-rw-r--r--   0 x         (1000) x         (1000)     3277 2023-04-21 23:31:42.000000 twitter-api-client-0.7.5/twitter/util.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-23 03:57:02.877258 twitter-api-client-0.7.5/twitter_api_client.egg-info/
+-rw-r--r--   0 x         (1000) x         (1000)     6490 2023-04-23 03:57:02.000000 twitter-api-client-0.7.5/twitter_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)      355 2023-04-23 03:57:02.000000 twitter-api-client-0.7.5/twitter_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 x         (1000) x         (1000)        1 2023-04-23 03:57:02.000000 twitter-api-client-0.7.5/twitter_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 x         (1000) x         (1000)       79 2023-04-23 03:57:02.000000 twitter-api-client-0.7.5/twitter_api_client.egg-info/requires.txt
+-rw-r--r--   0 x         (1000) x         (1000)        8 2023-04-23 03:57:02.000000 twitter-api-client-0.7.5/twitter_api_client.egg-info/top_level.txt
```

### Comparing `twitter-api-client-0.7.4/LICENSE` & `twitter-api-client-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.4/PKG-INFO` & `twitter-api-client-0.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.7.4
+Version: 0.7.5
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
```

### Comparing `twitter-api-client-0.7.4/setup.py` & `twitter-api-client-0.7.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "tqdm",
     "orjson",
     'uvloop; platform_system != "Windows"',
 ]
 
 setup(
     name="twitter-api-client",
-    version="0.7.4",
+    version="0.7.5",
     python_requires=">=3.11.0",
     description="Twitter API",
     long_description=dedent('''
     Complete implementation of the undocumented Twitter API
     
     Includes tools to **scrape**, **automate**, and **search** twitter
```

### Comparing `twitter-api-client-0.7.4/twitter/account.py` & `twitter-api-client-0.7.5/twitter/account.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.4/twitter/constants.py` & `twitter-api-client-0.7.5/twitter/constants.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.4/twitter/login.py` & `twitter-api-client-0.7.5/twitter/login.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.4/twitter/scraper.py` & `twitter-api-client-0.7.5/twitter/scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,16 @@
         nest_asyncio.apply()
 except:
     ...
 
 if platform.system() != 'Windows':
     try:
         import uvloop
+
+        uvloop.install()
     except ImportError as e:
         ...
 
 
 class Scraper:
     def __init__(self, email: str, username: str, password: str, *, save=True, debug=False):
         self.session = login(email, username, password)
@@ -128,17 +130,14 @@
         if self.debug:
             self.log(r, txt, data)
         if self.save:
             save_data(data, op, user_ids[0])
         return data
 
     def _run(self, ids: list[int | str], operation: tuple, limit=None):
-        if platform.system() != 'Windows':
-            with asyncio.Runner(loop_factory=uvloop.new_event_loop) as runner:
-                return runner.run(self._process(ids, operation, limit))
         return asyncio.run(self._process(ids, operation, limit))
 
     async def _process(self, ids: list[int | str], op: tuple, limit: int | None) -> list:
         async with AsyncClient(headers=get_headers(self.session)) as s:
             return await asyncio.gather(*(self._paginate(s, _id, op, limit) for _id in ids))
 
     async def _paginate(self, session: AsyncClient, _id: int | str | list[int], operation: tuple,
```

### Comparing `twitter-api-client-0.7.4/twitter/search.py` & `twitter-api-client-0.7.5/twitter/search.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.4/twitter/util.py` & `twitter-api-client-0.7.5/twitter/util.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.4/twitter_api_client.egg-info/PKG-INFO` & `twitter-api-client-0.7.5/twitter_api_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.7.4
+Version: 0.7.5
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
```

