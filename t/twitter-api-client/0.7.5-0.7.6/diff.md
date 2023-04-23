# Comparing `tmp/twitter-api-client-0.7.5.tar.gz` & `tmp/twitter-api-client-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitter-api-client-0.7.5.tar", last modified: Sun Apr 23 03:57:02 2023, max compression
+gzip compressed data, was "twitter-api-client-0.7.6.tar", last modified: Sun Apr 23 20:08:51 2023, max compression
```

## Comparing `twitter-api-client-0.7.5.tar` & `twitter-api-client-0.7.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-23 03:57:02.877258 twitter-api-client-0.7.5/
--rw-r--r--   0 x         (1000) x         (1000)     1075 2023-04-17 21:53:35.000000 twitter-api-client-0.7.5/LICENSE
--rw-r--r--   0 x         (1000) x         (1000)     6490 2023-04-23 03:57:02.877258 twitter-api-client-0.7.5/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)       38 2023-04-23 03:57:02.877258 twitter-api-client-0.7.5/setup.cfg
--rw-r--r--   0 x         (1000) x         (1000)     7736 2023-04-23 03:56:44.000000 twitter-api-client-0.7.5/setup.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-23 03:57:02.877258 twitter-api-client-0.7.5/twitter/
--rw-r--r--   0 x         (1000) x         (1000)        0 2023-04-17 21:53:35.000000 twitter-api-client-0.7.5/twitter/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)    21689 2023-04-22 23:30:33.000000 twitter-api-client-0.7.5/twitter/account.py
--rw-r--r--   0 x         (1000) x         (1000)    27271 2023-04-23 02:05:42.000000 twitter-api-client-0.7.5/twitter/constants.py
--rw-r--r--   0 x         (1000) x         (1000)     5501 2023-04-21 22:39:59.000000 twitter-api-client-0.7.5/twitter/login.py
--rw-r--r--   0 x         (1000) x         (1000)    11158 2023-04-23 03:55:18.000000 twitter-api-client-0.7.5/twitter/scraper.py
--rw-r--r--   0 x         (1000) x         (1000)     4469 2023-04-21 23:25:19.000000 twitter-api-client-0.7.5/twitter/search.py
--rw-r--r--   0 x         (1000) x         (1000)     3277 2023-04-21 23:31:42.000000 twitter-api-client-0.7.5/twitter/util.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-23 03:57:02.877258 twitter-api-client-0.7.5/twitter_api_client.egg-info/
--rw-r--r--   0 x         (1000) x         (1000)     6490 2023-04-23 03:57:02.000000 twitter-api-client-0.7.5/twitter_api_client.egg-info/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)      355 2023-04-23 03:57:02.000000 twitter-api-client-0.7.5/twitter_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 x         (1000) x         (1000)        1 2023-04-23 03:57:02.000000 twitter-api-client-0.7.5/twitter_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 x         (1000) x         (1000)       79 2023-04-23 03:57:02.000000 twitter-api-client-0.7.5/twitter_api_client.egg-info/requires.txt
--rw-r--r--   0 x         (1000) x         (1000)        8 2023-04-23 03:57:02.000000 twitter-api-client-0.7.5/twitter_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-23 20:08:51.453165 twitter-api-client-0.7.6/
+-rw-r--r--   0 x         (1000) x         (1000)     1075 2023-04-17 21:53:35.000000 twitter-api-client-0.7.6/LICENSE
+-rw-r--r--   0 x         (1000) x         (1000)     6242 2023-04-23 20:08:51.453165 twitter-api-client-0.7.6/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)       38 2023-04-23 20:08:51.453165 twitter-api-client-0.7.6/setup.cfg
+-rw-r--r--   0 x         (1000) x         (1000)     7452 2023-04-23 20:08:46.000000 twitter-api-client-0.7.6/setup.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-23 20:08:51.453165 twitter-api-client-0.7.6/twitter/
+-rw-r--r--   0 x         (1000) x         (1000)        0 2023-04-17 21:53:35.000000 twitter-api-client-0.7.6/twitter/__init__.py
+-rw-r--r--   0 x         (1000) x         (1000)    21689 2023-04-22 23:30:33.000000 twitter-api-client-0.7.6/twitter/account.py
+-rw-r--r--   0 x         (1000) x         (1000)    27271 2023-04-23 02:05:42.000000 twitter-api-client-0.7.6/twitter/constants.py
+-rw-r--r--   0 x         (1000) x         (1000)     5501 2023-04-21 22:39:59.000000 twitter-api-client-0.7.6/twitter/login.py
+-rw-r--r--   0 x         (1000) x         (1000)    11158 2023-04-23 03:55:18.000000 twitter-api-client-0.7.6/twitter/scraper.py
+-rw-r--r--   0 x         (1000) x         (1000)     4469 2023-04-21 23:25:19.000000 twitter-api-client-0.7.6/twitter/search.py
+-rw-r--r--   0 x         (1000) x         (1000)     3277 2023-04-21 23:31:42.000000 twitter-api-client-0.7.6/twitter/util.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-23 20:08:51.453165 twitter-api-client-0.7.6/twitter_api_client.egg-info/
+-rw-r--r--   0 x         (1000) x         (1000)     6242 2023-04-23 20:08:51.000000 twitter-api-client-0.7.6/twitter_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)      355 2023-04-23 20:08:51.000000 twitter-api-client-0.7.6/twitter_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 x         (1000) x         (1000)        1 2023-04-23 20:08:51.000000 twitter-api-client-0.7.6/twitter_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 x         (1000) x         (1000)       79 2023-04-23 20:08:51.000000 twitter-api-client-0.7.6/twitter_api_client.egg-info/requires.txt
+-rw-r--r--   0 x         (1000) x         (1000)        8 2023-04-23 20:08:51.000000 twitter-api-client-0.7.6/twitter_api_client.egg-info/top_level.txt
```

### Comparing `twitter-api-client-0.7.5/LICENSE` & `twitter-api-client-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.5/PKG-INFO` & `twitter-api-client-0.7.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,23 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.7.5
+Version: 0.7.6
 Summary: Twitter API
-Home-page: https://github.com/trevorhobenshield/twitter-api
+Home-page: https://github.com/trevorhobenshield/twitter-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-Complete implementation of the undocumented Twitter API
+Implementation of Twitter's v1, v2, and GraphQL APIs
 
-Includes tools to **scrape**, **automate**, and **search** twitter
-
-* [Installation](#installation)
-* [Automation](#automation)
-* [Scraping](#scraping)
-  * [Get all user/tweet data](#get-all-usertweet-data)
-  * [Get user/tweet data (no auth)](#get-usertweet-data-no-auth)
-  * [Search](#search)
-* [Notes](#notes)
+Includes tools to **scrape**, **automate**, and **search**.
 
 ### Automation
 
 ```python
 from twitter.account import Account
 
 email, username, password = ..., ..., ...
```

### Comparing `twitter-api-client-0.7.5/setup.py` & `twitter-api-client-0.7.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,30 +9,22 @@
     "tqdm",
     "orjson",
     'uvloop; platform_system != "Windows"',
 ]
 
 setup(
     name="twitter-api-client",
-    version="0.7.5",
+    version="0.7.6",
     python_requires=">=3.11.0",
     description="Twitter API",
     long_description=dedent('''
-    Complete implementation of the undocumented Twitter API
-    
-    Includes tools to **scrape**, **automate**, and **search** twitter
-    
-    * [Installation](#installation)
-    * [Automation](#automation)
-    * [Scraping](#scraping)
-      * [Get all user/tweet data](#get-all-usertweet-data)
-      * [Get user/tweet data (no auth)](#get-usertweet-data-no-auth)
-      * [Search](#search)
-    * [Notes](#notes)
+    Implementation of Twitter's v1, v2, and GraphQL APIs
     
+    Includes tools to **scrape**, **automate**, and **search**.
+
     ### Automation
     
     ```python
     from twitter.account import Account
     
     email, username, password = ..., ..., ...
     account = Account(email, username, password, debug=2, save=True)
@@ -235,13 +227,13 @@
         limit=100,
     )
     ```
     '''),
     long_description_content_type='text/markdown',
     author="Trevor Hobenshield",
     author_email="trevorhobenshield@gmail.com",
-    url="https://github.com/trevorhobenshield/twitter-api",
+    url="https://github.com/trevorhobenshield/twitter-api-client",
     install_requires=install_requires,
     keywords="twitter api client async search automation bot scrape",
     packages=find_packages(),
     include_package_data=True,
 )
```

### Comparing `twitter-api-client-0.7.5/twitter/account.py` & `twitter-api-client-0.7.6/twitter/account.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.5/twitter/constants.py` & `twitter-api-client-0.7.6/twitter/constants.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.5/twitter/login.py` & `twitter-api-client-0.7.6/twitter/login.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.5/twitter/scraper.py` & `twitter-api-client-0.7.6/twitter/scraper.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.5/twitter/search.py` & `twitter-api-client-0.7.6/twitter/search.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.5/twitter/util.py` & `twitter-api-client-0.7.6/twitter/util.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.5/twitter_api_client.egg-info/PKG-INFO` & `twitter-api-client-0.7.6/twitter_api_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,23 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.7.5
+Version: 0.7.6
 Summary: Twitter API
-Home-page: https://github.com/trevorhobenshield/twitter-api
+Home-page: https://github.com/trevorhobenshield/twitter-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-Complete implementation of the undocumented Twitter API
+Implementation of Twitter's v1, v2, and GraphQL APIs
 
-Includes tools to **scrape**, **automate**, and **search** twitter
-
-* [Installation](#installation)
-* [Automation](#automation)
-* [Scraping](#scraping)
-  * [Get all user/tweet data](#get-all-usertweet-data)
-  * [Get user/tweet data (no auth)](#get-usertweet-data-no-auth)
-  * [Search](#search)
-* [Notes](#notes)
+Includes tools to **scrape**, **automate**, and **search**.
 
 ### Automation
 
 ```python
 from twitter.account import Account
 
 email, username, password = ..., ..., ...
```

