# Comparing `tmp/openlimit-0.1.0.tar.gz` & `tmp/openlimit-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openlimit-0.1.0.tar", last modified: Thu Apr 20 02:31:11 2023, max compression
+gzip compressed data, was "openlimit-0.2.0.tar", last modified: Sun Apr 23 11:06:36 2023, max compression
```

## Comparing `openlimit-0.1.0.tar` & `openlimit-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-04-20 02:31:11.172664 openlimit-0.1.0/
--rw-r--r--   0 jshobrook   (501) staff       (20)      351 2023-04-20 02:31:11.172551 openlimit-0.1.0/PKG-INFO
--rw-r--r--   0 jshobrook   (501) staff       (20)     2953 2023-04-20 02:04:04.000000 openlimit-0.1.0/README.md
-drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-04-20 02:31:11.171694 openlimit-0.1.0/openlimit/
--rw-r--r--   0 jshobrook   (501) staff       (20)      206 2023-04-19 18:27:50.000000 openlimit-0.1.0/openlimit/__init__.py
--rw-r--r--   0 jshobrook   (501) staff       (20)     1774 2023-04-20 02:30:45.000000 openlimit-0.1.0/openlimit/rate_limiters.py
--rw-r--r--   0 jshobrook   (501) staff       (20)     2864 2023-04-20 02:30:35.000000 openlimit-0.1.0/openlimit/redis_rate_limiters.py
-drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-04-20 02:31:11.172388 openlimit-0.1.0/openlimit.egg-info/
--rw-r--r--   0 jshobrook   (501) staff       (20)      351 2023-04-20 02:31:11.000000 openlimit-0.1.0/openlimit.egg-info/PKG-INFO
--rw-r--r--   0 jshobrook   (501) staff       (20)      264 2023-04-20 02:31:11.000000 openlimit-0.1.0/openlimit.egg-info/SOURCES.txt
--rw-r--r--   0 jshobrook   (501) staff       (20)        1 2023-04-20 02:31:11.000000 openlimit-0.1.0/openlimit.egg-info/dependency_links.txt
--rw-r--r--   0 jshobrook   (501) staff       (20)       15 2023-04-20 02:31:11.000000 openlimit-0.1.0/openlimit.egg-info/requires.txt
--rw-r--r--   0 jshobrook   (501) staff       (20)       10 2023-04-20 02:31:11.000000 openlimit-0.1.0/openlimit.egg-info/top_level.txt
--rw-r--r--   0 jshobrook   (501) staff       (20)       38 2023-04-20 02:31:11.172706 openlimit-0.1.0/setup.cfg
--rw-r--r--   0 jshobrook   (501) staff       (20)      515 2023-04-20 02:31:04.000000 openlimit-0.1.0/setup.py
+drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-04-23 11:06:36.438891 openlimit-0.2.0/
+-rw-r--r--   0 jshobrook   (501) staff       (20)      351 2023-04-23 11:06:36.438750 openlimit-0.2.0/PKG-INFO
+-rw-r--r--   0 jshobrook   (501) staff       (20)     3216 2023-04-23 09:54:09.000000 openlimit-0.2.0/README.md
+drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-04-23 11:06:36.438080 openlimit-0.2.0/openlimit/
+-rw-r--r--   0 jshobrook   (501) staff       (20)      206 2023-04-19 18:27:50.000000 openlimit-0.2.0/openlimit/__init__.py
+-rw-r--r--   0 jshobrook   (501) staff       (20)     1766 2023-04-23 11:05:14.000000 openlimit-0.2.0/openlimit/rate_limiters.py
+-rw-r--r--   0 jshobrook   (501) staff       (20)     2835 2023-04-23 11:02:37.000000 openlimit-0.2.0/openlimit/redis_rate_limiters.py
+drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-04-23 11:06:36.438591 openlimit-0.2.0/openlimit.egg-info/
+-rw-r--r--   0 jshobrook   (501) staff       (20)      351 2023-04-23 11:06:36.000000 openlimit-0.2.0/openlimit.egg-info/PKG-INFO
+-rw-r--r--   0 jshobrook   (501) staff       (20)      264 2023-04-23 11:06:36.000000 openlimit-0.2.0/openlimit.egg-info/SOURCES.txt
+-rw-r--r--   0 jshobrook   (501) staff       (20)        1 2023-04-23 11:06:36.000000 openlimit-0.2.0/openlimit.egg-info/dependency_links.txt
+-rw-r--r--   0 jshobrook   (501) staff       (20)       15 2023-04-23 11:06:36.000000 openlimit-0.2.0/openlimit.egg-info/requires.txt
+-rw-r--r--   0 jshobrook   (501) staff       (20)       10 2023-04-23 11:06:36.000000 openlimit-0.2.0/openlimit.egg-info/top_level.txt
+-rw-r--r--   0 jshobrook   (501) staff       (20)       38 2023-04-23 11:06:36.438946 openlimit-0.2.0/setup.cfg
+-rw-r--r--   0 jshobrook   (501) staff       (20)      515 2023-04-23 11:06:18.000000 openlimit-0.2.0/setup.py
```

### Comparing `openlimit-0.1.0/README.md` & `openlimit-0.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,71 +1,76 @@
 # openlimit
 
 Rate limiter for the OpenAI API. Implements the [generic cell rate algorithm,](https://en.wikipedia.org/wiki/Generic_cell_rate_algorithm) an efficient variant of the leaky bucket pattern. 
 
 `openlimit` can:
 
 - Handle both _request_ and _token_ limits
-- Apply rate limits with one line of code
+- Precisely enforce rate limits with one line of code
 - Limit _synchronous_ and _asynchronous_ requests
 - Use Redis to track limits across multiple threads or processes
 
-## Installation 
+## Installation
 
 You can install `openlimit` with pip:
 
 ```bash
 $ pip install openlimit
 ```
 
 ## Usage
 
-Applying a rate limit is as simple as adding a `with` statement to your API calls. For example:
+### Define a rate limit
+
+First, define your rate limits for the OpenAI model you're using. For example:
 
 ```python
 from openlimit import ChatRateLimiter
 
 rate_limiter = ChatRateLimiter(request_limit=200, token_limit=40000)
+```
+
+This sets a rate limit for a chat completion model (e.g. gpt-4, gpt-3.5-turbo). `openlimit` offers different rate limiter objects for different OpenAI models, all with the same parameters: `request_limit` and `token_limit`. Both limits are measured _per-minute_ and may vary depending on the user.
+
+| Rate limiter | Supported models |
+| --- | --- |
+| `ChatRateLimiter` | gpt-4, gpt-4-0314, gpt-4-32k, gpt-4-32k-0314, gpt-3.5-turbo, gpt-3.5-turbo-0301 |
+| `CompletionRateLimiter` | text-davinci-003, text-davinci-002, text-curie-001, text-babbage-001, text-ada-001 |
+| `EmbeddingRateLimiter` | text-embedding-ada-002 |
+
+### Apply the rate limit
+
+To apply the rate limit, add a `with` statement to your API calls:
+
+```python
 chat_params = { 
     "model": "gpt-4", 
     "messages": [{"role": "user", "content": "Hello!"}]
 }
 
 with rate_limiter.limit(**chat_params):
     response = openai.ChatCompletion.create(**chat_params)
 ```
 
-Notice that `rate_limiter.limit` expects the same parameters as the actual API call. 
+Ensure that `rate_limiter.limit` receives the same parameters as the actual API call. This is important for calculating expected token usage.
 
-You can also decorate functions that make API calls, so long as the decorated function is passed the same parameters that are passed to the API call.
+Alternatively, you can decorate functions that make API calls, as long as the decorated function receives the same parameters as the API call:
 
 ```python
 @rate_limiter.is_limited()
 def call_openai(**chat_params):
     response = openai.ChatCompletion.create(**chat_params)
     return response
 ```
 
-`openlimit` provides different rate limiter classes for different OpenAI models, listed in the table below. Each have the same parameters: `request_limit` and `token_limit`.
-
-| Rate limiter | Supported models |
-| --- | --- |
-| `ChatRateLimiter` | gpt-4, gpt-4-0314, gpt-4-32k, gpt-4-32k-0314, gpt-3.5-turbo, gpt-3.5-turbo-0301 |
-| `CompletionRateLimiter` | text-davinci-003, text-davinci-002, text-curie-001, text-babbage-001, text-ada-001 |
-| `EmbeddingRateLimiter` | text-embedding-ada-002 |
-
 ### Asynchronous requests
 
-Rate limits can be enforced for asynchronous requests too.
+Rate limits can be enforced for asynchronous requests too:
 
 ```python
-from openlimit import ChatRateLimiter
-
-rate_limiter = ChatRateLimiter(request_limit=200, token_limit=40000)
-
 async def call_openai():
     chat_params = { 
         "model": "gpt-4", 
         "messages": [{"role": "user", "content": "Hello!"}]
     }
 
     async with rate_limiter.limit(**chat_params):
@@ -84,10 +89,12 @@
     token_limit=40000,
     redis_url="redis://localhost:5050"
 )
 
 # Use `rate_limiter` like you would normally ...
 ```
 
+All `RateLimiter` objects have `RateLimiterWithRedis` counterparts.
+
 ## Contributing
 
-If you want to contribute to the library, get started with [Adrenaline.](https://useadrenaline.com/) Just paste in a link to this repository to familiarize yourself.
+If you want to contribute to the library, get started with [Adrenaline.](https://useadrenaline.com/) Simply paste in a link to this repository to familiarize yourself.
```

### Comparing `openlimit-0.1.0/openlimit/rate_limiters.py` & `openlimit-0.2.0/openlimit/rate_limiters.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,24 +20,24 @@
 
         # Token counter
         self.token_counter = token_counter
 
         # Buckets
         self._request_bucket = Bucket(request_limit)
         self._token_bucket = Bucket(token_limit)
-    
+ 
     async def wait_for_capacity(self, num_tokens):
         await asyncio.gather(
-            self._request_bucket.wait_for_capacity(1),
-            self._token_bucket.wait_for_capacity(num_tokens)
+            self._token_bucket.wait_for_capacity(num_tokens),
+            self._request_bucket.wait_for_capacity(1)
         )
     
     def limit(self, **kwargs):
         num_tokens = self.token_counter(**kwargs)
-        return cd.AsyncContextManager(num_tokens, self)
+        return cd.ContextManager(num_tokens, self)
     
     def is_limited(self):
         return cd.FunctionDecorator(self)
 
 
 ######
 # MAIN
```

### Comparing `openlimit-0.1.0/openlimit/redis_rate_limiters.py` & `openlimit-0.2.0/openlimit/redis_rate_limiters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Standard library
 import asyncio
 
 # Third party
-from redis import asyncio as aioredis
+import redis
 
 # Local
 import openlimit.utilities.token_counters as tc
 import openlimit.utilities.context_decorators as cd
 from openlimit.buckets import RedisBucket
 
 
@@ -34,37 +34,37 @@
         # Bucket prefix (for Redis)
         self._bucket_key = bucket_key
     
     async def _init_buckets(self):
         if self._request_bucket and self._token_bucket:
             return
 
-        redis = await aioredis.from_url(self._redis_url, encoding="utf-8", decode_responses=True)
+        redis = await redis.asyncio.from_url(self._redis_url, encoding="utf-8", decode_responses=True)
 
         self._request_bucket = RedisBucket(
             self.request_limit,
             bucket_key=f"{self._bucket_key}_requests",
             redis=redis
         )
         self._token_bucket = RedisBucket(
             self.token_limit,
             bucket_key=f"{self._bucket_key}_tokens",
             redis=redis
         )
-    
+
     async def wait_for_capacity(self, num_tokens):
         await self._init_buckets()
         await asyncio.gather(
-            self._request_bucket.wait_for_capacity(1),
-            self._token_bucket.wait_for_capacity(num_tokens)
+            self._token_bucket.wait_for_capacity(num_tokens),
+            self._request_bucket.wait_for_capacity(1)
         )
     
     def limit(self, **kwargs):
         num_tokens = self.token_counter(**kwargs)
-        return cd.AsyncContextManager(num_tokens, self)
+        return cd.ContextManager(num_tokens, self)
     
     def is_limited(self):
         return cd.FunctionDecorator(self)
 
 
 ######
 # MAIN
```

### Comparing `openlimit-0.1.0/setup.py` & `openlimit-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 from setuptools import setup
 
 setup(
     name="openlimit",
     description="Rate limiter for the OpenAI API",
-    version="v0.1.0",
+    version="v0.2.0",
     packages=["openlimit"],
     python_requires=">=3",
     url="https://github.com/shobrook/openlimit",
     author="shobrook",
     author_email="shobrookj@gmail.com",
     # classifiers=[],
     install_requires=["redis", "tiktoken"],
```

