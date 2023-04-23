# Comparing `tmp/openlimit-0.2.3.tar.gz` & `tmp/openlimit-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openlimit-0.2.3.tar", last modified: Sun Apr 23 11:47:56 2023, max compression
+gzip compressed data, was "openlimit-0.2.4.tar", last modified: Sun Apr 23 14:05:53 2023, max compression
```

## Comparing `openlimit-0.2.3.tar` & `openlimit-0.2.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-04-23 11:47:56.421100 openlimit-0.2.3/
--rw-r--r--   0 jshobrook   (501) staff       (20)      351 2023-04-23 11:47:56.420981 openlimit-0.2.3/PKG-INFO
--rw-r--r--   0 jshobrook   (501) staff       (20)     3216 2023-04-23 09:54:09.000000 openlimit-0.2.3/README.md
-drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-04-23 11:47:56.419140 openlimit-0.2.3/openlimit/
--rw-r--r--   0 jshobrook   (501) staff       (20)      226 2023-04-23 11:35:43.000000 openlimit-0.2.3/openlimit/__init__.py
-drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-04-23 11:47:56.420232 openlimit-0.2.3/openlimit/buckets/
--rw-r--r--   0 jshobrook   (501) staff       (20)       98 2023-04-23 11:38:27.000000 openlimit-0.2.3/openlimit/buckets/__init__.py
--rw-r--r--   0 jshobrook   (501) staff       (20)      988 2023-04-23 11:03:59.000000 openlimit-0.2.3/openlimit/buckets/bucket.py
--rw-r--r--   0 jshobrook   (501) staff       (20)     1869 2023-04-23 11:01:20.000000 openlimit-0.2.3/openlimit/buckets/redis_bucket.py
--rw-r--r--   0 jshobrook   (501) staff       (20)     1717 2023-04-23 11:41:46.000000 openlimit-0.2.3/openlimit/rate_limiters.py
--rw-r--r--   0 jshobrook   (501) staff       (20)     2786 2023-04-23 11:42:05.000000 openlimit-0.2.3/openlimit/redis_rate_limiters.py
-drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-04-23 11:47:56.420717 openlimit-0.2.3/openlimit/utilities/
--rw-r--r--   0 jshobrook   (501) staff       (20)      252 2023-04-23 11:41:16.000000 openlimit-0.2.3/openlimit/utilities/__init__.py
--rw-r--r--   0 jshobrook   (501) staff       (20)     1576 2023-04-23 11:03:35.000000 openlimit-0.2.3/openlimit/utilities/context_decorators.py
--rw-r--r--   0 jshobrook   (501) staff       (20)     1681 2023-04-20 01:13:53.000000 openlimit-0.2.3/openlimit/utilities/token_counters.py
-drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-04-23 11:47:56.419749 openlimit-0.2.3/openlimit.egg-info/
--rw-r--r--   0 jshobrook   (501) staff       (20)      351 2023-04-23 11:47:56.000000 openlimit-0.2.3/openlimit.egg-info/PKG-INFO
--rw-r--r--   0 jshobrook   (501) staff       (20)      468 2023-04-23 11:47:56.000000 openlimit-0.2.3/openlimit.egg-info/SOURCES.txt
--rw-r--r--   0 jshobrook   (501) staff       (20)        1 2023-04-23 11:47:56.000000 openlimit-0.2.3/openlimit.egg-info/dependency_links.txt
--rw-r--r--   0 jshobrook   (501) staff       (20)       15 2023-04-23 11:47:56.000000 openlimit-0.2.3/openlimit.egg-info/requires.txt
--rw-r--r--   0 jshobrook   (501) staff       (20)       10 2023-04-23 11:47:56.000000 openlimit-0.2.3/openlimit.egg-info/top_level.txt
--rw-r--r--   0 jshobrook   (501) staff       (20)       38 2023-04-23 11:47:56.421144 openlimit-0.2.3/setup.cfg
--rw-r--r--   0 jshobrook   (501) staff       (20)      559 2023-04-23 11:47:52.000000 openlimit-0.2.3/setup.py
+drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-04-23 14:05:53.342349 openlimit-0.2.4/
+-rw-r--r--   0 jshobrook   (501) staff       (20)      351 2023-04-23 14:05:53.342236 openlimit-0.2.4/PKG-INFO
+-rw-r--r--   0 jshobrook   (501) staff       (20)     3216 2023-04-23 12:13:25.000000 openlimit-0.2.4/README.md
+drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-04-23 14:05:53.340301 openlimit-0.2.4/openlimit/
+-rw-r--r--   0 jshobrook   (501) staff       (20)      226 2023-04-23 11:35:43.000000 openlimit-0.2.4/openlimit/__init__.py
+drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-04-23 14:05:53.341293 openlimit-0.2.4/openlimit/buckets/
+-rw-r--r--   0 jshobrook   (501) staff       (20)       98 2023-04-23 11:38:27.000000 openlimit-0.2.4/openlimit/buckets/__init__.py
+-rw-r--r--   0 jshobrook   (501) staff       (20)      988 2023-04-23 11:03:59.000000 openlimit-0.2.4/openlimit/buckets/bucket.py
+-rw-r--r--   0 jshobrook   (501) staff       (20)     1869 2023-04-23 11:01:20.000000 openlimit-0.2.4/openlimit/buckets/redis_bucket.py
+-rw-r--r--   0 jshobrook   (501) staff       (20)     1750 2023-04-23 14:04:33.000000 openlimit-0.2.4/openlimit/rate_limiters.py
+-rw-r--r--   0 jshobrook   (501) staff       (20)     2823 2023-04-23 14:05:00.000000 openlimit-0.2.4/openlimit/redis_rate_limiters.py
+drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-04-23 14:05:53.341884 openlimit-0.2.4/openlimit/utilities/
+-rw-r--r--   0 jshobrook   (501) staff       (20)      252 2023-04-23 11:41:16.000000 openlimit-0.2.4/openlimit/utilities/__init__.py
+-rw-r--r--   0 jshobrook   (501) staff       (20)     1576 2023-04-23 11:03:35.000000 openlimit-0.2.4/openlimit/utilities/context_decorators.py
+-rw-r--r--   0 jshobrook   (501) staff       (20)     1681 2023-04-20 01:13:53.000000 openlimit-0.2.4/openlimit/utilities/token_counters.py
+drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-04-23 14:05:53.340799 openlimit-0.2.4/openlimit.egg-info/
+-rw-r--r--   0 jshobrook   (501) staff       (20)      351 2023-04-23 14:05:53.000000 openlimit-0.2.4/openlimit.egg-info/PKG-INFO
+-rw-r--r--   0 jshobrook   (501) staff       (20)      468 2023-04-23 14:05:53.000000 openlimit-0.2.4/openlimit.egg-info/SOURCES.txt
+-rw-r--r--   0 jshobrook   (501) staff       (20)        1 2023-04-23 14:05:53.000000 openlimit-0.2.4/openlimit.egg-info/dependency_links.txt
+-rw-r--r--   0 jshobrook   (501) staff       (20)       15 2023-04-23 14:05:53.000000 openlimit-0.2.4/openlimit.egg-info/requires.txt
+-rw-r--r--   0 jshobrook   (501) staff       (20)       10 2023-04-23 14:05:53.000000 openlimit-0.2.4/openlimit.egg-info/top_level.txt
+-rw-r--r--   0 jshobrook   (501) staff       (20)       38 2023-04-23 14:05:53.342409 openlimit-0.2.4/setup.cfg
+-rw-r--r--   0 jshobrook   (501) staff       (20)      559 2023-04-23 14:05:17.000000 openlimit-0.2.4/setup.py
```

### Comparing `openlimit-0.2.3/README.md` & `openlimit-0.2.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # openlimit
 
-Rate limiter for the OpenAI API. Implements the [generic cell rate algorithm,](https://en.wikipedia.org/wiki/Generic_cell_rate_algorithm) an efficient variant of the leaky bucket pattern. 
-
-`openlimit` can:
+Simple and efficient rate limiter for the OpenAI API. It can:
 
 - Handle both _request_ and _token_ limits
 - Precisely enforce rate limits with one line of code
 - Limit _synchronous_ and _asynchronous_ requests
 - Use Redis to track limits across multiple threads or processes
 
+Implements the [generic cell rate algorithm,](https://en.wikipedia.org/wiki/Generic_cell_rate_algorithm) a variant of the leaky bucket pattern.
+
 ## Installation
 
 You can install `openlimit` with pip:
 
 ```bash
 $ pip install openlimit
 ```
```

### Comparing `openlimit-0.2.3/openlimit/buckets/bucket.py` & `openlimit-0.2.4/openlimit/buckets/bucket.py`

 * *Files identical despite different names*

### Comparing `openlimit-0.2.3/openlimit/buckets/redis_bucket.py` & `openlimit-0.2.4/openlimit/buckets/redis_bucket.py`

 * *Files identical despite different names*

### Comparing `openlimit-0.2.3/openlimit/rate_limiters.py` & `openlimit-0.2.4/openlimit/rate_limiters.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,29 +42,29 @@
 # MAIN
 ######
 
 
 class ChatRateLimiter(RateLimiter):
     def __init__(self, request_limit, token_limit):
         super().__init__(
-            request_limit, 
-            token_limit, 
+            request_limit=3500,
+            token_limit=90000,
             utils.num_tokens_consumed_by_chat_request
         )
 
 
 class CompletionRateLimiter(RateLimiter):
     def __init__(self, request_limit, token_limit):
         super().__init__(
-            request_limit, 
-            token_limit, 
+            request_limit=3500,
+            token_limit=350000,
             utils.num_tokens_consumed_by_completion_request
         )
 
 
 class EmbeddingRateLimiter(RateLimiter):
     def __init__(self, request_limit, token_limit):
         super().__init__(
-            request_limit, 
-            token_limit, 
+            request_limit=3500, 
+            token_limit=70000000, 
             utils.num_tokens_consumed_by_embedding_request
         )
```

### Comparing `openlimit-0.2.3/openlimit/redis_rate_limiters.py` & `openlimit-0.2.4/openlimit/redis_rate_limiters.py`

 * *Files 12% similar despite different names*

```diff
@@ -69,35 +69,35 @@
 # MAIN
 ######
 
 
 class ChatRateLimiterWithRedis(RateLimiterWithRedis):
     def __init__(self, request_limit, token_limit, redis_url="redis://localhost:5050"):
         super().__init__(
-            request_limit, 
-            token_limit, 
+            request_limit=3500, 
+            token_limit=90000, 
             utils.num_tokens_consumed_by_chat_request,
             "chat", 
             redis_url
         )
 
 
 class CompletionRateLimiterWithRedis(RateLimiterWithRedis):
     def __init__(self, request_limit, token_limit, redis_url="redis://localhost:5050"):
         super().__init__(
-            request_limit, 
-            token_limit, 
+            request_limit=3500, 
+            token_limit=350000, 
             utils.num_tokens_consumed_by_completion_request,
             "completion", 
             redis_url
         )
 
 
 class EmbeddingRateLimiterWithRedis(RateLimiterWithRedis):
     def __init__(self, request_limit, token_limit, redis_url="redis://localhost:5050"):
         super().__init__(
-            request_limit, 
-            token_limit, 
+            request_limit=3500, 
+            token_limit=70000000, 
             utils.num_tokens_consumed_by_embedding_request,
             "embedding", 
             redis_url
         )
```

### Comparing `openlimit-0.2.3/openlimit/utilities/context_decorators.py` & `openlimit-0.2.4/openlimit/utilities/context_decorators.py`

 * *Files identical despite different names*

### Comparing `openlimit-0.2.3/openlimit/utilities/token_counters.py` & `openlimit-0.2.4/openlimit/utilities/token_counters.py`

 * *Files identical despite different names*

### Comparing `openlimit-0.2.3/setup.py` & `openlimit-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 from setuptools import setup
 
 setup(
     name="openlimit",
     description="Rate limiter for the OpenAI API",
-    version="v0.2.3",
+    version="v0.2.4",
     packages=["openlimit", "openlimit.utilities", "openlimit.buckets"],
     python_requires=">=3",
     url="https://github.com/shobrook/openlimit",
     author="shobrook",
     author_email="shobrookj@gmail.com",
     # classifiers=[],
     install_requires=["redis", "tiktoken"],
```

