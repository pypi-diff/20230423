# Comparing `tmp/openlimit-0.2.1.tar.gz` & `tmp/openlimit-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openlimit-0.2.1.tar", last modified: Sun Apr 23 11:36:25 2023, max compression
+gzip compressed data, was "openlimit-0.2.2.tar", last modified: Sun Apr 23 11:42:20 2023, max compression
```

## Comparing `openlimit-0.2.1.tar` & `openlimit-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-04-23 11:36:25.660903 openlimit-0.2.1/
--rw-r--r--   0 jshobrook   (501) staff       (20)      351 2023-04-23 11:36:25.660782 openlimit-0.2.1/PKG-INFO
--rw-r--r--   0 jshobrook   (501) staff       (20)     3216 2023-04-23 09:54:09.000000 openlimit-0.2.1/README.md
-drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-04-23 11:36:25.659952 openlimit-0.2.1/openlimit/
--rw-r--r--   0 jshobrook   (501) staff       (20)      226 2023-04-23 11:35:43.000000 openlimit-0.2.1/openlimit/__init__.py
--rw-r--r--   0 jshobrook   (501) staff       (20)     1766 2023-04-23 11:05:14.000000 openlimit-0.2.1/openlimit/rate_limiters.py
--rw-r--r--   0 jshobrook   (501) staff       (20)     2835 2023-04-23 11:02:37.000000 openlimit-0.2.1/openlimit/redis_rate_limiters.py
-drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-04-23 11:36:25.660647 openlimit-0.2.1/openlimit.egg-info/
--rw-r--r--   0 jshobrook   (501) staff       (20)      351 2023-04-23 11:36:25.000000 openlimit-0.2.1/openlimit.egg-info/PKG-INFO
--rw-r--r--   0 jshobrook   (501) staff       (20)      264 2023-04-23 11:36:25.000000 openlimit-0.2.1/openlimit.egg-info/SOURCES.txt
--rw-r--r--   0 jshobrook   (501) staff       (20)        1 2023-04-23 11:36:25.000000 openlimit-0.2.1/openlimit.egg-info/dependency_links.txt
--rw-r--r--   0 jshobrook   (501) staff       (20)       15 2023-04-23 11:36:25.000000 openlimit-0.2.1/openlimit.egg-info/requires.txt
--rw-r--r--   0 jshobrook   (501) staff       (20)       10 2023-04-23 11:36:25.000000 openlimit-0.2.1/openlimit.egg-info/top_level.txt
--rw-r--r--   0 jshobrook   (501) staff       (20)       38 2023-04-23 11:36:25.660942 openlimit-0.2.1/setup.cfg
--rw-r--r--   0 jshobrook   (501) staff       (20)      515 2023-04-23 11:36:18.000000 openlimit-0.2.1/setup.py
+drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-04-23 11:42:20.008410 openlimit-0.2.2/
+-rw-r--r--   0 jshobrook   (501) staff       (20)      351 2023-04-23 11:42:20.008291 openlimit-0.2.2/PKG-INFO
+-rw-r--r--   0 jshobrook   (501) staff       (20)     3216 2023-04-23 09:54:09.000000 openlimit-0.2.2/README.md
+drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-04-23 11:42:20.007590 openlimit-0.2.2/openlimit/
+-rw-r--r--   0 jshobrook   (501) staff       (20)      226 2023-04-23 11:35:43.000000 openlimit-0.2.2/openlimit/__init__.py
+-rw-r--r--   0 jshobrook   (501) staff       (20)     1717 2023-04-23 11:41:46.000000 openlimit-0.2.2/openlimit/rate_limiters.py
+-rw-r--r--   0 jshobrook   (501) staff       (20)     2786 2023-04-23 11:42:05.000000 openlimit-0.2.2/openlimit/redis_rate_limiters.py
+drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-04-23 11:42:20.008145 openlimit-0.2.2/openlimit.egg-info/
+-rw-r--r--   0 jshobrook   (501) staff       (20)      351 2023-04-23 11:42:19.000000 openlimit-0.2.2/openlimit.egg-info/PKG-INFO
+-rw-r--r--   0 jshobrook   (501) staff       (20)      264 2023-04-23 11:42:20.000000 openlimit-0.2.2/openlimit.egg-info/SOURCES.txt
+-rw-r--r--   0 jshobrook   (501) staff       (20)        1 2023-04-23 11:42:19.000000 openlimit-0.2.2/openlimit.egg-info/dependency_links.txt
+-rw-r--r--   0 jshobrook   (501) staff       (20)       15 2023-04-23 11:42:19.000000 openlimit-0.2.2/openlimit.egg-info/requires.txt
+-rw-r--r--   0 jshobrook   (501) staff       (20)       10 2023-04-23 11:42:19.000000 openlimit-0.2.2/openlimit.egg-info/top_level.txt
+-rw-r--r--   0 jshobrook   (501) staff       (20)       38 2023-04-23 11:42:20.008451 openlimit-0.2.2/setup.cfg
+-rw-r--r--   0 jshobrook   (501) staff       (20)      515 2023-04-23 11:42:16.000000 openlimit-0.2.2/setup.py
```

### Comparing `openlimit-0.2.1/README.md` & `openlimit-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `openlimit-0.2.1/openlimit/rate_limiters.py` & `openlimit-0.2.2/openlimit/rate_limiters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Standard library
 import asyncio
 
 # Local
-import openlimit.utilities.token_counters as tc
-import openlimit.utilities.context_decorators as cd
+import openlimit.utilities as utils
 from openlimit.buckets import Bucket
 
 
 ############
 # BASE CLASS
 ############
 
@@ -29,43 +28,43 @@
         await asyncio.gather(
             self._token_bucket.wait_for_capacity(num_tokens),
             self._request_bucket.wait_for_capacity(1)
         )
     
     def limit(self, **kwargs):
         num_tokens = self.token_counter(**kwargs)
-        return cd.ContextManager(num_tokens, self)
+        return utils.ContextManager(num_tokens, self)
     
     def is_limited(self):
-        return cd.FunctionDecorator(self)
+        return utils.FunctionDecorator(self)
 
 
 ######
 # MAIN
 ######
 
 
 class ChatRateLimiter(RateLimiter):
     def __init__(self, request_limit, token_limit):
         super().__init__(
             request_limit, 
             token_limit, 
-            tc.num_tokens_consumed_by_chat_request
+            utils.num_tokens_consumed_by_chat_request
         )
 
 
 class CompletionRateLimiter(RateLimiter):
     def __init__(self, request_limit, token_limit):
         super().__init__(
             request_limit, 
             token_limit, 
-            tc.num_tokens_consumed_by_completion_request
+            utils.num_tokens_consumed_by_completion_request
         )
 
 
 class EmbeddingRateLimiter(RateLimiter):
     def __init__(self, request_limit, token_limit):
         super().__init__(
             request_limit, 
             token_limit, 
-            tc.num_tokens_consumed_by_embedding_request
+            utils.num_tokens_consumed_by_embedding_request
         )
```

### Comparing `openlimit-0.2.1/openlimit/redis_rate_limiters.py` & `openlimit-0.2.2/openlimit/redis_rate_limiters.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # Standard library
 import asyncio
 
 # Third party
 import redis
 
 # Local
-import openlimit.utilities.token_counters as tc
-import openlimit.utilities.context_decorators as cd
+import openlimit.utilities as utils
 from openlimit.buckets import RedisBucket
 
 
 ############
 # BASE CLASS
 ############
 
@@ -56,49 +55,49 @@
         await asyncio.gather(
             self._token_bucket.wait_for_capacity(num_tokens),
             self._request_bucket.wait_for_capacity(1)
         )
     
     def limit(self, **kwargs):
         num_tokens = self.token_counter(**kwargs)
-        return cd.ContextManager(num_tokens, self)
+        return utils.ContextManager(num_tokens, self)
     
     def is_limited(self):
-        return cd.FunctionDecorator(self)
+        return utils.FunctionDecorator(self)
 
 
 ######
 # MAIN
 ######
 
 
 class ChatRateLimiterWithRedis(RateLimiterWithRedis):
     def __init__(self, request_limit, token_limit, redis_url="redis://localhost:5050"):
         super().__init__(
             request_limit, 
             token_limit, 
-            tc.num_tokens_consumed_by_chat_request,
+            utils.num_tokens_consumed_by_chat_request,
             "chat", 
             redis_url
         )
 
 
 class CompletionRateLimiterWithRedis(RateLimiterWithRedis):
     def __init__(self, request_limit, token_limit, redis_url="redis://localhost:5050"):
         super().__init__(
             request_limit, 
             token_limit, 
-            tc.num_tokens_consumed_by_completion_request,
+            utils.num_tokens_consumed_by_completion_request,
             "completion", 
             redis_url
         )
 
 
 class EmbeddingRateLimiterWithRedis(RateLimiterWithRedis):
     def __init__(self, request_limit, token_limit, redis_url="redis://localhost:5050"):
         super().__init__(
             request_limit, 
             token_limit, 
-            tc.num_tokens_consumed_by_embedding_request,
+            utils.num_tokens_consumed_by_embedding_request,
             "embedding", 
             redis_url
         )
```

### Comparing `openlimit-0.2.1/setup.py` & `openlimit-0.2.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 from setuptools import setup
 
 setup(
     name="openlimit",
     description="Rate limiter for the OpenAI API",
-    version="v0.2.1",
+    version="v0.2.2",
     packages=["openlimit"],
     python_requires=">=3",
     url="https://github.com/shobrook/openlimit",
     author="shobrook",
     author_email="shobrookj@gmail.com",
     # classifiers=[],
     install_requires=["redis", "tiktoken"],
```

