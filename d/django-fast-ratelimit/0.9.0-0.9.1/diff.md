# Comparing `tmp/django_fast_ratelimit-0.9.0.tar.gz` & `tmp/django_fast_ratelimit-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_fast_ratelimit-0.9.0.tar", max compression
+gzip compressed data, was "django_fast_ratelimit-0.9.1.tar", max compression
```

## Comparing `django_fast_ratelimit-0.9.0.tar` & `django_fast_ratelimit-0.9.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1065 2022-08-02 08:04:04.663327 django_fast_ratelimit-0.9.0/LICENSE
--rw-r--r--   0        0        0     7751 2023-01-06 12:31:43.682677 django_fast_ratelimit-0.9.0/README.md
--rw-r--r--   0        0        0      815 2023-01-06 12:31:56.509261 django_fast_ratelimit-0.9.0/pyproject.toml
--rw-r--r--   0        0        0       57 2022-08-03 08:10:59.641136 django_fast_ratelimit-0.9.0/ratelimit/__init__.py
--rw-r--r--   0        0        0    18108 2023-01-06 12:28:08.705157 django_fast_ratelimit-0.9.0/ratelimit/_core.py
--rw-r--r--   0        0        0     4822 2022-08-03 08:10:55.701253 django_fast_ratelimit-0.9.0/ratelimit/methods.py
--rw-r--r--   0        0        0     1418 2023-01-06 11:44:43.744905 django_fast_ratelimit-0.9.0/ratelimit/misc.py
--rw-r--r--   0        0        0     8721 1970-01-01 00:00:00.000000 django_fast_ratelimit-0.9.0/setup.py
--rw-r--r--   0        0        0     8642 1970-01-01 00:00:00.000000 django_fast_ratelimit-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-08-02 08:04:04.663327 django_fast_ratelimit-0.9.1/LICENSE
+-rw-r--r--   0        0        0     7751 2023-01-06 12:31:43.682677 django_fast_ratelimit-0.9.1/README.md
+-rw-r--r--   0        0        0      797 2023-01-08 21:43:04.907198 django_fast_ratelimit-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0       57 2022-08-03 08:10:59.641136 django_fast_ratelimit-0.9.1/ratelimit/__init__.py
+-rw-r--r--   0        0        0    18108 2023-01-06 12:28:08.705157 django_fast_ratelimit-0.9.1/ratelimit/_core.py
+-rw-r--r--   0        0        0     4822 2022-08-03 08:10:55.701253 django_fast_ratelimit-0.9.1/ratelimit/methods.py
+-rw-r--r--   0        0        0     1418 2023-01-06 11:44:43.744905 django_fast_ratelimit-0.9.1/ratelimit/misc.py
+-rw-r--r--   0        0        0     8645 1970-01-01 00:00:00.000000 django_fast_ratelimit-0.9.1/setup.py
+-rw-r--r--   0        0        0     8584 1970-01-01 00:00:00.000000 django_fast_ratelimit-0.9.1/PKG-INFO
```

### Comparing `django_fast_ratelimit-0.9.0/LICENSE` & `django_fast_ratelimit-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_fast_ratelimit-0.9.0/README.md` & `django_fast_ratelimit-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `django_fast_ratelimit-0.9.0/pyproject.toml` & `django_fast_ratelimit-0.9.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "django-fast-ratelimit"
 description = "Fast ratelimit implementation with django caches"
-version = "0.9.0"
+version = "0.9.1"
 license = "MIT"
 authors = ["Alexander Kaftan"]
 readme = "README.md"
 repository = "https://github.com/devkral/django-fast-ratelimit"
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Environment :: Web Environment",
@@ -16,20 +16,18 @@
 packages = [
   { include = "ratelimit" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 django = ">=3.0"
-tox = {version="*", optional=true}
 
+[tool.poetry.group.test.dependencies]
+tox = "*"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 tox = "*"
 django = ">=4.0"
 
-[tool.poetry.extras]
-test = ["tox"]
-
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `django_fast_ratelimit-0.9.0/ratelimit/_core.py` & `django_fast_ratelimit-0.9.1/ratelimit/_core.py`

 * *Files identical despite different names*

### Comparing `django_fast_ratelimit-0.9.0/ratelimit/methods.py` & `django_fast_ratelimit-0.9.1/ratelimit/methods.py`

 * *Files identical despite different names*

### Comparing `django_fast_ratelimit-0.9.0/ratelimit/misc.py` & `django_fast_ratelimit-0.9.1/ratelimit/misc.py`

 * *Files identical despite different names*

### Comparing `django_fast_ratelimit-0.9.0/setup.py` & `django_fast_ratelimit-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,29 +6,25 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['django>=3.0']
 
-extras_require = \
-{'test': ['tox']}
-
 setup_kwargs = {
     'name': 'django-fast-ratelimit',
-    'version': '0.9.0',
+    'version': '0.9.1',
     'description': 'Fast ratelimit implementation with django caches',
     'long_description': '# django-fast-ratelimit\n\nDjango-fast-ratelimit provides a secure and fast ratelimit facility based on the django caching framework.\nIt uses a "Fixed window counter"-algorithm based on:\nhttps://medium.com/figma-design/an-alternative-approach-to-rate-limiting-f8a06cf7c94c\n\n## Installation\n\n```bash\npip install django-fast-ratelimit\n\n```\n\nNote: pip >= 19 is required\n\n## usage\n\nDecorator:\n\n```python\nimport ratelimit\n\n@ratelimit.decorate(key="ip", rate="1/s")\ndef expensive_func(request):\n    # how many ratelimits request limiting\n    if request.ratelimit["request_limit"] > 0:\n        # reschedule with end of rate epoch\n        return request_waiting(request.ratelimit["end"])\n\n```\n\nor async\n\n```python\nimport ratelimit\nimport asyncio\n\n@ratelimit.decorate(key="ip", rate="1/s")\nasync def expensive_func(request):\n    # how many ratelimits request limiting\n    if request.ratelimit["request_limit"] > 0:\n        # reschedule with end of rate epoch\n        await asyncio.sleep(request.ratelimit["end"])\n\n```\n\nblocking Decorator (raises RatelimitError):\n\n```python\nimport ratelimit\n\n@ratelimit.decorate(key="ip", rate="1/s", block=True, methods=ratelimit.UNSAFE)\ndef expensive_func(request):\n    # how many ratelimits request limiting\n    if request.ratelimit["end"] > 0:\n\n```\n\ndecorate View (requires group):\n\n```python\nimport ratelimit\nfrom django.views.generic import View\nfrom django.utils.decorators import method_decorator\n\n\n@method_decorator(ratelimit.decorate(\n  key="ip", rate="1/s", block=True, methods=ratelimit.SAFE, group="required"\n), name="dispatch")\nclass FooView(View):\n    ...\n\n```\n\nmanual\n\n```python\nimport ratelimit\n\n\ndef func(request):\n    ratelimit.get_ratelimit(key="ip", rate="1/s", request=request, group="123")\n    # or only for GET\n    ratelimit.get_ratelimit(\n        key="ip", rate="1/s", request=request, group="123", methods="GET"\n    )\n    # also simple calls possible (note: key in bytes format)\n    ratelimit.get_ratelimit(\n        key=b"abc", rate="1/s", group="123"\n    )\n    # check constraints of rate\n    r = ratelimit.parse_rate("1/s")  # returns tuple (amount, period)\n    assert(r[1]==1)  #  assert period is 1 second\n    # for simple naming use o2g (object to group)\n    ratelimit.get_ratelimit(\n        key=b"abc", rate=r, group=ratelimit.o2g(func)\n    )\n\n```\n\n## parameters\n\n### ratelimit.get_ratelimit:\n\n-   group: group name, can be callable (fun(request))\n-   rate: rate limit, multiple modes\n    Note: if count (first argument) is 0, then it raises the Disabled exception, the second argument must be greater then 0\n    -   str: default mode , specify rate in form of "1/4s" or "2/s" or "2/m"\n    -   2 element tuple/list: first argument is amount, second are seconds\n    -   callable: can return of two\n-   methods: set of checked methods, can be callable (fun(request, group)), modes:\n    -   callable(request, group): allow dynamic\n    -   ratelimit.ALL (default): all methods are checked\n    -   \\("HEAD", "GET"\\): list of checked methods\n    -   ratelimit.invertedset(["HEAD", "GET"]): inverted set of checked methods. Here: every method is checked, except HEAD, GET\n-   request: ingoing request (optional if key supports it and methods=ratelimit.ALL (default))\n-   key: multiple modes possible:\n    -   bool: True: skip key (should only be used for baking), False: disable cache (like RATELIMIT_ENABLE=False)\n    -   int: sidestep cache, value will be used for request_limit. 0 is for never blocking, >=1 blocks\n    -   str: "path.to.method:argument"\n    -   str: "inbuildmethod:argument" see methods for valid arguments\n    -   str: "inbuildmethod" method which is ready to use for (request, group)\n    -   tuple,list: ["method", args...]: method (can be also inbuild) with arbitary arguments\n    -   bytes: static key (supports mode without request)\n    -   callable: check return of function (fun(request, group)), return must be string (converted to bytes), bytes, bool or int (see "key" for effects)\n-   empty_to: convert empty keys (b"") to parameter. Must be bytes, bool or int (see "key" for effects) (default: keep b"")\n-   cache: specify cache to use, defaults to RATELIMIT_DEFAULT_CACHE setting (default: "default")\n-   hash_algo: name of hash algorithm for creating cache_key (defaults to RATELIMIT_KEY_HASH setting (default: "sha256"))\n    Note: group is seperately hashed\n-   hashctx: optimation parameter, read the code and only use if you know what you are doing. It basically circumvents the parameter hashing and only hashes the key. If the key parameter is True even the key is skipped\n-   action {ratelimit.Action}:\n    -   PEEK: only lookup\n    -   INCREASE: count up and return result\n    -   RESET: return former result and reset (default: {PEEK})\n-   include_reset: add reset method to Ratelimit object if no cache bypass is in use\n\nreturns following named_tuple\n\n-   count: how often in the window the ip whatever was calling\n-   limit: limit when it should block\n-   request_limit: >=1 should block or reject, 0: should accept\n-   end: when does the block end\n-   group: group name\n-   reset: function to reset count if cache was used and include_reset specified otherwise None\n\nor raises `ratelimit.Disabled` in case of the count in the rate is zero\n\n### ratelimit.aget_ratelimit:\n\nsame as `get_ratelimit` but supports async methods and has an optional parameter:\n`wait`, which suspends the execution (via `asyncio.sleep`) for the time specified in rate (second argument).\nThis is only possible in async mode, as it would block too much in sync mode.\n\n### ratelimit.decorate:\n\nAll of ratelimit.get_ratelimit except request. group is here optional (except for decorations with method_decorator (no access to wrapped function)).\nAlso supports:\n\n-   block: should hard block with an RatelimitExceeded exception (subclass of PermissionDenied) or only annotate request with ratelimit\n-   wait (only async functions): suspends execution\n\nNote: wait is tricky with method_decorator: you must ensure that the function decorated is async\n\n## helpers\n\n### ratelimit.invertedset:\n\ninverts a collection, useful for http methods\n\n### ratelimit.o2g:\n\nauto generate group names for method/function as input, see tests/test_decorators for more info\n\nExample:\n\n```python\n\n\nimport ratelimit\n\n\nclass O2gView(View):\n    def get(self, request, *args, **kwargs):\n        request.ratelimit2 = ratelimit.get_ratelimit(\n            group=ratelimit.o2g(self.get),\n            rate="1/s",\n            key=b"o2gtest",\n            action=ratelimit.Action.INCREASE,\n            include_reset=True,\n        )\n        if request.ratelimit2.request_limit > 0:\n            return HttpResponse(status=400)\n        return HttpResponse()\n\n\n\n\n```\n\n## methods\n\nSee in methods which methods are available. Here some of them:\n\n-   ip: use ip address as key, argument: [netmask ipv4/]netmask ipv6\n-   user: authenticated user primary key or b""\n-   user_or_ip: use autenticated user primary key as key. If not autenticated fallback to ip, also with netmask argument\n-   user_and_ip: same like user_or_ip except that the ip matching also applies for authenticated users\n-   get: generate key from multiple sources, input can be multiple input args or a dict with options\n\n## settings\n\n-   RATELIMIT_GROUP_HASH: hash function which is used for the group hash (default: md5)\n-   RATELIMIT_KEY_HASH: hash function which is used as default for the key hash, can be overridden with hash_algo (default: md5)\n-   RATELIMIT_ENABLE disable ratelimit (e.g. for tests) (default: enabled)\n-   RATELIMIT_KEY_PREFIX: internal prefix for the hash keys (so you don\'t have to create a new cache). Defaults to "frl:".\n-   RATELIMIT_DEFAULT_CACHE: default cache to use, defaults to "default" and can be overridden by cache parameter\n',
     'author': 'Alexander Kaftan',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/devkral/django-fast-ratelimit',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'extras_require': extras_require,
     'python_requires': '>=3.9,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `django_fast_ratelimit-0.9.0/PKG-INFO` & `django_fast_ratelimit-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: django-fast-ratelimit
-Version: 0.9.0
+Version: 0.9.1
 Summary: Fast ratelimit implementation with django caches
 Home-page: https://github.com/devkral/django-fast-ratelimit
 License: MIT
 Author: Alexander Kaftan
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Provides-Extra: test
 Requires-Dist: django (>=3.0)
-Requires-Dist: tox ; extra == "test"
 Project-URL: Repository, https://github.com/devkral/django-fast-ratelimit
 Description-Content-Type: text/markdown
 
 # django-fast-ratelimit
 
 Django-fast-ratelimit provides a secure and fast ratelimit facility based on the django caching framework.
 It uses a "Fixed window counter"-algorithm based on:
```

