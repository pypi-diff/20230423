# Comparing `tmp/twitter-api-client-0.7.3.tar.gz` & `tmp/twitter-api-client-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitter-api-client-0.7.3.tar", last modified: Sun Apr 23 01:47:00 2023, max compression
+gzip compressed data, was "twitter-api-client-0.7.4.tar", last modified: Sun Apr 23 02:06:02 2023, max compression
```

## Comparing `twitter-api-client-0.7.3.tar` & `twitter-api-client-0.7.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-23 01:47:00.416847 twitter-api-client-0.7.3/
--rw-r--r--   0 x         (1000) x         (1000)     1075 2023-04-17 21:53:35.000000 twitter-api-client-0.7.3/LICENSE
--rw-r--r--   0 x         (1000) x         (1000)     6391 2023-04-23 01:47:00.416847 twitter-api-client-0.7.3/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)       38 2023-04-23 01:47:00.416847 twitter-api-client-0.7.3/setup.cfg
--rw-r--r--   0 x         (1000) x         (1000)     7621 2023-04-23 01:46:44.000000 twitter-api-client-0.7.3/setup.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-23 01:47:00.416847 twitter-api-client-0.7.3/twitter/
--rw-r--r--   0 x         (1000) x         (1000)        0 2023-04-17 21:53:35.000000 twitter-api-client-0.7.3/twitter/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)    21689 2023-04-22 23:30:33.000000 twitter-api-client-0.7.3/twitter/account.py
--rw-r--r--   0 x         (1000) x         (1000)    27260 2023-04-19 22:52:46.000000 twitter-api-client-0.7.3/twitter/constants.py
--rw-r--r--   0 x         (1000) x         (1000)     5501 2023-04-21 22:39:59.000000 twitter-api-client-0.7.3/twitter/login.py
--rw-r--r--   0 x         (1000) x         (1000)    10624 2023-04-22 23:27:35.000000 twitter-api-client-0.7.3/twitter/scraper.py
--rw-r--r--   0 x         (1000) x         (1000)     4469 2023-04-21 23:25:19.000000 twitter-api-client-0.7.3/twitter/search.py
--rw-r--r--   0 x         (1000) x         (1000)     3277 2023-04-21 23:31:42.000000 twitter-api-client-0.7.3/twitter/util.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-23 01:47:00.416847 twitter-api-client-0.7.3/twitter_api_client.egg-info/
--rw-r--r--   0 x         (1000) x         (1000)     6391 2023-04-23 01:47:00.000000 twitter-api-client-0.7.3/twitter_api_client.egg-info/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)      355 2023-04-23 01:47:00.000000 twitter-api-client-0.7.3/twitter_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 x         (1000) x         (1000)        1 2023-04-23 01:47:00.000000 twitter-api-client-0.7.3/twitter_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 x         (1000) x         (1000)       79 2023-04-23 01:47:00.000000 twitter-api-client-0.7.3/twitter_api_client.egg-info/requires.txt
--rw-r--r--   0 x         (1000) x         (1000)        8 2023-04-23 01:47:00.000000 twitter-api-client-0.7.3/twitter_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-23 02:06:02.484122 twitter-api-client-0.7.4/
+-rw-r--r--   0 x         (1000) x         (1000)     1075 2023-04-17 21:53:35.000000 twitter-api-client-0.7.4/LICENSE
+-rw-r--r--   0 x         (1000) x         (1000)     6490 2023-04-23 02:06:02.484122 twitter-api-client-0.7.4/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)       38 2023-04-23 02:06:02.484122 twitter-api-client-0.7.4/setup.cfg
+-rw-r--r--   0 x         (1000) x         (1000)     7736 2023-04-23 02:05:42.000000 twitter-api-client-0.7.4/setup.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-23 02:06:02.484122 twitter-api-client-0.7.4/twitter/
+-rw-r--r--   0 x         (1000) x         (1000)        0 2023-04-17 21:53:35.000000 twitter-api-client-0.7.4/twitter/__init__.py
+-rw-r--r--   0 x         (1000) x         (1000)    21689 2023-04-22 23:30:33.000000 twitter-api-client-0.7.4/twitter/account.py
+-rw-r--r--   0 x         (1000) x         (1000)    27271 2023-04-23 02:05:42.000000 twitter-api-client-0.7.4/twitter/constants.py
+-rw-r--r--   0 x         (1000) x         (1000)     5501 2023-04-21 22:39:59.000000 twitter-api-client-0.7.4/twitter/login.py
+-rw-r--r--   0 x         (1000) x         (1000)    11326 2023-04-23 02:02:26.000000 twitter-api-client-0.7.4/twitter/scraper.py
+-rw-r--r--   0 x         (1000) x         (1000)     4469 2023-04-21 23:25:19.000000 twitter-api-client-0.7.4/twitter/search.py
+-rw-r--r--   0 x         (1000) x         (1000)     3277 2023-04-21 23:31:42.000000 twitter-api-client-0.7.4/twitter/util.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-23 02:06:02.484122 twitter-api-client-0.7.4/twitter_api_client.egg-info/
+-rw-r--r--   0 x         (1000) x         (1000)     6490 2023-04-23 02:06:02.000000 twitter-api-client-0.7.4/twitter_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)      355 2023-04-23 02:06:02.000000 twitter-api-client-0.7.4/twitter_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 x         (1000) x         (1000)        1 2023-04-23 02:06:02.000000 twitter-api-client-0.7.4/twitter_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 x         (1000) x         (1000)       79 2023-04-23 02:06:02.000000 twitter-api-client-0.7.4/twitter_api_client.egg-info/requires.txt
+-rw-r--r--   0 x         (1000) x         (1000)        8 2023-04-23 02:06:02.000000 twitter-api-client-0.7.4/twitter_api_client.egg-info/top_level.txt
```

### Comparing `twitter-api-client-0.7.3/LICENSE` & `twitter-api-client-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.3/PKG-INFO` & `twitter-api-client-0.7.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.7.3
+Version: 0.7.4
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
@@ -183,28 +183,33 @@
 likes = scraper.likes([123, 234, 345])
 tweets_and_replies = scraper.tweets_and_replies([123, 234, 345])
 media = scraper.media([123, 234, 345])
 following = scraper.following([123, 234, 345])
 followers = scraper.followers([123, 234, 345])
 scraper.tweet_stats([111111, 222222, 333333])
 
+# get recommended users based on user
+scraper.recommended_users()
+scraper.recommended_users(123)
 
 # tweet data
 tweets_by_ids = scraper.tweets_by_id([987, 876, 754])
 tweets_details = scraper.tweets_details([987, 876, 754])
 retweeters = scraper.retweeters([987, 876, 754])
 favoriters = scraper.favoriters([987, 876, 754])
 
 scraper.download_media([
     111111,
     222222,
     333333,
     444444,
 ])
 
+
+
 # trends
 scraper.trends()
 ```
 
 #### Search
 
 ```python
```

### Comparing `twitter-api-client-0.7.3/setup.py` & `twitter-api-client-0.7.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "tqdm",
     "orjson",
     'uvloop; platform_system != "Windows"',
 ]
 
 setup(
     name="twitter-api-client",
-    version="0.7.3",
+    version="0.7.4",
     python_requires=">=3.11.0",
     description="Twitter API",
     long_description=dedent('''
     Complete implementation of the undocumented Twitter API
     
     Includes tools to **scrape**, **automate**, and **search** twitter
     
@@ -189,28 +189,33 @@
     likes = scraper.likes([123, 234, 345])
     tweets_and_replies = scraper.tweets_and_replies([123, 234, 345])
     media = scraper.media([123, 234, 345])
     following = scraper.following([123, 234, 345])
     followers = scraper.followers([123, 234, 345])
     scraper.tweet_stats([111111, 222222, 333333])
     
+    # get recommended users based on user
+    scraper.recommended_users()
+    scraper.recommended_users(123)
     
     # tweet data
     tweets_by_ids = scraper.tweets_by_id([987, 876, 754])
     tweets_details = scraper.tweets_details([987, 876, 754])
     retweeters = scraper.retweeters([987, 876, 754])
     favoriters = scraper.favoriters([987, 876, 754])
     
     scraper.download_media([
         111111,
         222222,
         333333,
         444444,
     ])
     
+
+    
     # trends
     scraper.trends()
     ```
     
     #### Search
     
     ```python
```

### Comparing `twitter-api-client-0.7.3/twitter/account.py` & `twitter-api-client-0.7.4/twitter/account.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.3/twitter/constants.py` & `twitter-api-client-0.7.4/twitter/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,15 @@
 
     # auth required
     Likes = 'nYrjBgnUWQFt_tRyCGatZA', 'Likes', 'userId'
     Followers = 'pd8Tt1qUz1YWrICegqZ8cw', 'Followers', 'userId'
     Following = 'wjvx62Hye2dGVvnvVco0xA', 'Following', 'userId'
     Retweeters = '0BoJlKAxoNPQUHRftlwZ2w', 'Retweeters', 'tweetId'
     Favoriters = 'XRRjv1-uj1HZn3o324etOQ', 'Favoriters', 'tweetId'
+    ConnectTabTimeline = 'lq02A-gEzbLefqTgD_PFzQ', 'ConnectTabTimeline', 'context'
 
     # Account Operations
     useSendMessageMutation = 'MaxK2PKX1F9Z-9SwqwavTw', 'useSendMessageMutation'
     CreateTweet = '7TKRKCPuAGsmYde0CudbVg', 'CreateTweet'
     DeleteTweet = 'VaenaVgh5q5ih7kvyVjgtg', 'DeleteTweet'
     CreateScheduledTweet = 'LCVzRQGxOaGnOnYH01NQXg', 'CreateScheduledTweet'
     DeleteScheduledTweet = 'CTOVqej0JBXAZSwkp1US0g', 'DeleteScheduledTweet'
@@ -167,15 +168,14 @@
     CommunityRemoveRule = 'EI_g43Ss_Ixg0EC4K7nzlQ', 'CommunityRemoveRule'
     CommunityReorderRules = 'VwluNMGnl5uaNZ3LnlCQ_A', 'CommunityReorderRules'
     CommunityTweetsRankedTimeline = 'P38EspBBPhAfSKPP74-s2Q', 'CommunityTweetsRankedTimeline'
     CommunityTweetsTimeline = '2JgHOlqfeLusxAT0yGQJjg', 'CommunityTweetsTimeline'
     CommunityUpdateRole = '5eq76kkUqfdCzInCtcxQOA', 'CommunityUpdateRole'
     CommunityUserInvite = 'x8hUNaBCOV2tSalqB9cwWQ', 'CommunityUserInvite'
     CommunityUserRelationshipTypeahead = 'gi_UGcUurYp6N6p2BaLJqQ', 'CommunityUserRelationshipTypeahead'
-    ConnectTabTimeline = 'lq02A-gEzbLefqTgD_PFzQ', 'ConnectTabTimeline'
     ConversationControlChange = 'hb1elGcj6769uT8qVYqtjw', 'ConversationControlChange'
     ConversationControlDelete = 'OoMO_aSZ1ZXjegeamF9QmA', 'ConversationControlDelete'
     ConvertRitoSuggestedActions = '2njnYoE69O2jdUM7KMEnDw', 'ConvertRitoSuggestedActions'
     Coupons = 'R1h43jnAl2bsDoUkgZb7NQ', 'Coupons'
     CreateCommunity = 'lRjZKTRcWuqwtYwCWGy9_w', 'CreateCommunity'
     CreateCustomerPortalSession = '2LHXrd1uYeaMWhciZgPZFw', 'CreateCustomerPortalSession'
     CreateDraftTweet = 'cH9HZWz_EW9gnswvA4ZRiQ', 'CreateDraftTweet'
```

### Comparing `twitter-api-client-0.7.3/twitter/login.py` & `twitter-api-client-0.7.4/twitter/login.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.3/twitter/scraper.py` & `twitter-api-client-0.7.4/twitter/scraper.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,24 +90,40 @@
         Use the batched query `users_by_ids` instead if you wish to pull user profile data.
         """
         return self._run(user_ids, Operation.UserByRestId)
 
     def tweet_stats(self, user_ids: list[int]) -> list[dict]:
         return self._run(user_ids, Operation.TweetStats)
 
+    def recommended_users(self, user_id: int = None) -> dict:
+        qid, op, key = Operation.ConnectTabTimeline
+        context = {"contextualUserId": user_id} if user_id else {}
+        params = {k: orjson.dumps(v).decode() for k, v in {
+            'variables': Operation.default_variables | {key: orjson.dumps(context).decode()},
+            'features': Operation.default_features,
+        }.items()}
+        r = self.session.get(f'{self.api}/{qid}/{op}', headers=get_headers(self.session), params=params)
+        txt = r.text
+        data = r.json()
+        if self.debug:
+            self.log(r, txt, data)
+        if self.save:
+            save_data(data, op, user_id)
+        return data
+
     # special case, batch query
     def users_by_ids(self, user_ids: list[int]) -> dict:
         """
         Get user data in batches
 
         Batch-size limited to around 200-300 users
         """
-        qid, op, k = Operation.UsersByRestIds
+        qid, op, key = Operation.UsersByRestIds
         params = {k: orjson.dumps(v).decode() for k, v in {
-            'variables': Operation.default_variables | {k: user_ids},
+            'variables': Operation.default_variables | {key: user_ids},
             'features': Operation.default_features,
         }.items()}
         r = self.session.get(f'{self.api}/{qid}/{op}', headers=get_headers(self.session), params=params)
         txt = r.text
         data = r.json()
         if self.debug:
             self.log(r, txt, data)
```

### Comparing `twitter-api-client-0.7.3/twitter/search.py` & `twitter-api-client-0.7.4/twitter/search.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.3/twitter/util.py` & `twitter-api-client-0.7.4/twitter/util.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.3/twitter_api_client.egg-info/PKG-INFO` & `twitter-api-client-0.7.4/twitter_api_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.7.3
+Version: 0.7.4
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
@@ -183,28 +183,33 @@
 likes = scraper.likes([123, 234, 345])
 tweets_and_replies = scraper.tweets_and_replies([123, 234, 345])
 media = scraper.media([123, 234, 345])
 following = scraper.following([123, 234, 345])
 followers = scraper.followers([123, 234, 345])
 scraper.tweet_stats([111111, 222222, 333333])
 
+# get recommended users based on user
+scraper.recommended_users()
+scraper.recommended_users(123)
 
 # tweet data
 tweets_by_ids = scraper.tweets_by_id([987, 876, 754])
 tweets_details = scraper.tweets_details([987, 876, 754])
 retweeters = scraper.retweeters([987, 876, 754])
 favoriters = scraper.favoriters([987, 876, 754])
 
 scraper.download_media([
     111111,
     222222,
     333333,
     444444,
 ])
 
+
+
 # trends
 scraper.trends()
 ```
 
 #### Search
 
 ```python
```

