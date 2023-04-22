# Comparing `tmp/discord-ext-pager-1.0.0.post1.tar.gz` & `tmp/discord-ext-pager-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord-ext-pager-1.0.0.post1.tar", last modified: Sat Apr 15 14:38:44 2023, max compression
+gzip compressed data, was "discord-ext-pager-1.0.1.tar", last modified: Sat Apr 22 22:39:59 2023, max compression
```

## Comparing `discord-ext-pager-1.0.0.post1.tar` & `discord-ext-pager-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 14:38:44.722700 discord-ext-pager-1.0.0.post1/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-04-15 14:38:30.000000 discord-ext-pager-1.0.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5838 2023-04-15 14:38:44.722700 discord-ext-pager-1.0.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-04-15 14:38:30.000000 discord-ext-pager-1.0.0.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-15 14:38:30.000000 discord-ext-pager-1.0.0.post1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 14:38:44.722700 discord-ext-pager-1.0.0.post1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 14:38:44.722700 discord-ext-pager-1.0.0.post1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 14:38:44.722700 discord-ext-pager-1.0.0.post1/src/discord/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 14:38:44.722700 discord-ext-pager-1.0.0.post1/src/discord/ext/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 14:38:44.722700 discord-ext-pager-1.0.0.post1/src/discord/ext/pager/
--rw-r--r--   0 runner    (1001) docker     (123)    15626 2023-04-15 14:38:30.000000 discord-ext-pager-1.0.0.post1/src/discord/ext/pager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 14:38:44.722700 discord-ext-pager-1.0.0.post1/src/discord_ext_pager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5838 2023-04-15 14:38:44.000000 discord-ext-pager-1.0.0.post1/src/discord_ext_pager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-15 14:38:44.000000 discord-ext-pager-1.0.0.post1/src/discord_ext_pager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 14:38:44.000000 discord-ext-pager-1.0.0.post1/src/discord_ext_pager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-15 14:38:44.000000 discord-ext-pager-1.0.0.post1/src/discord_ext_pager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-15 14:38:44.000000 discord-ext-pager-1.0.0.post1/src/discord_ext_pager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:39:59.754344 discord-ext-pager-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-04-22 22:39:47.000000 discord-ext-pager-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-04-22 22:39:59.754344 discord-ext-pager-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-04-22 22:39:47.000000 discord-ext-pager-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-22 22:39:47.000000 discord-ext-pager-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 22:39:59.754344 discord-ext-pager-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:39:59.750344 discord-ext-pager-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:39:59.750344 discord-ext-pager-1.0.1/src/discord/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:39:59.750344 discord-ext-pager-1.0.1/src/discord/ext/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:39:59.750344 discord-ext-pager-1.0.1/src/discord/ext/pager/
+-rw-r--r--   0 runner    (1001) docker     (123)    15625 2023-04-22 22:39:47.000000 discord-ext-pager-1.0.1/src/discord/ext/pager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:39:59.754344 discord-ext-pager-1.0.1/src/discord_ext_pager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-04-22 22:39:59.000000 discord-ext-pager-1.0.1/src/discord_ext_pager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-22 22:39:59.000000 discord-ext-pager-1.0.1/src/discord_ext_pager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 22:39:59.000000 discord-ext-pager-1.0.1/src/discord_ext_pager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-22 22:39:59.000000 discord-ext-pager-1.0.1/src/discord_ext_pager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-22 22:39:59.000000 discord-ext-pager-1.0.1/src/discord_ext_pager.egg-info/top_level.txt
```

### Comparing `discord-ext-pager-1.0.0.post1/LICENSE` & `discord-ext-pager-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `discord-ext-pager-1.0.0.post1/PKG-INFO` & `discord-ext-pager-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: discord-ext-pager
-Version: 1.0.0.post1
+Version: 1.0.1
 Summary: A view-based paginator library for discord.py 2.0
 Author: thegamecracks
 Keywords: discord,discord.py,paginator,view
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
@@ -22,24 +23,20 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # discord-ext-pager
 
 [![PyPI](https://img.shields.io/pypi/v/discord-ext-pager?label=View%20on%20pypi&style=flat-square)](https://pypi.org/project/discord-ext-pager/)
 
-A simple view-based paginator library for discord.py 2.0.
+A simple view-based paginator library for discord.py 2.0. Works with Python 3.8+.
 
-## Installation
+## Usage
 
 [discord-ext-pager] is available on PyPI, and as such can be installed using pip.
 
-[discord-ext-pager]: https://pypi.org/project/discord-ext-pager/
-
-## Usage
-
 Users of Danny's [discord-ext-menus] will find some familiarity
 in this library. Provided are the following classes:
 
 - PaginatorView:
   The view class that manages pagination and navigation.
 - PageSource:
   The base class for sources the paginator view can accept.
@@ -48,14 +45,15 @@
 - AsyncIteratorPageSource:
   The base class for formatting an asynchronous iterator of items.
 - PageOption:
   A subclass of `discord.SelectOption` used for presenting navigation options.
 - TimeoutAction:
   An enum for customizing PaginatorView's timeout behaviour.
 
+[discord-ext-pager]: https://pypi.org/project/discord-ext-pager/
 [discord-ext-menus]: https://github.com/Rapptz/discord-ext-menus
 
 The `PaginatorView` can be instantiated and used by itself, but page formatting
 is handled by subclassing one of the `PageSource` base classes.
 
 ```py
 from typing import Any, List
```

### Comparing `discord-ext-pager-1.0.0.post1/README.md` & `discord-ext-pager-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 # discord-ext-pager
 
 [![PyPI](https://img.shields.io/pypi/v/discord-ext-pager?label=View%20on%20pypi&style=flat-square)](https://pypi.org/project/discord-ext-pager/)
 
-A simple view-based paginator library for discord.py 2.0.
+A simple view-based paginator library for discord.py 2.0. Works with Python 3.8+.
 
-## Installation
+## Usage
 
 [discord-ext-pager] is available on PyPI, and as such can be installed using pip.
 
-[discord-ext-pager]: https://pypi.org/project/discord-ext-pager/
-
-## Usage
-
 Users of Danny's [discord-ext-menus] will find some familiarity
 in this library. Provided are the following classes:
 
 - PaginatorView:
   The view class that manages pagination and navigation.
 - PageSource:
   The base class for sources the paginator view can accept.
@@ -24,14 +20,15 @@
 - AsyncIteratorPageSource:
   The base class for formatting an asynchronous iterator of items.
 - PageOption:
   A subclass of `discord.SelectOption` used for presenting navigation options.
 - TimeoutAction:
   An enum for customizing PaginatorView's timeout behaviour.
 
+[discord-ext-pager]: https://pypi.org/project/discord-ext-pager/
 [discord-ext-menus]: https://github.com/Rapptz/discord-ext-menus
 
 The `PaginatorView` can be instantiated and used by itself, but page formatting
 is handled by subclassing one of the `PageSource` base classes.
 
 ```py
 from typing import Any, List
```

### Comparing `discord-ext-pager-1.0.0.post1/src/discord/ext/pager/__init__.py` & `discord-ext-pager-1.0.1/src/discord/ext/pager/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     Union,
     cast,
 )
 
 import discord
 from typing_extensions import TypeAlias
 
-__version__ = "1.0.0.post1"
+__version__ = "1.0.1"
 
 __all__ = (
     "PageOption",
     "PageSource",
     "ListPageSource",
     "AsyncIteratorPageSource",
     "TimeoutAction",
@@ -225,15 +225,15 @@
         ],
         allowed_users: Optional[Collection[int]] = None,
         timeout_action: TimeoutAction = TimeoutAction.CLEAR,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
         if isinstance(sources, PageSource):
-            sources = [sources]
+            self.sources = [sources]
         else:
             self.sources = list(sources)
             if len(self.sources) == 0:
                 raise ValueError("must provide at least one page source")
         self.allowed_users = allowed_users
         self.timeout_action = timeout_action
```

### Comparing `discord-ext-pager-1.0.0.post1/src/discord_ext_pager.egg-info/PKG-INFO` & `discord-ext-pager-1.0.1/src/discord_ext_pager.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: discord-ext-pager
-Version: 1.0.0.post1
+Version: 1.0.1
 Summary: A view-based paginator library for discord.py 2.0
 Author: thegamecracks
 Keywords: discord,discord.py,paginator,view
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
@@ -22,24 +23,20 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # discord-ext-pager
 
 [![PyPI](https://img.shields.io/pypi/v/discord-ext-pager?label=View%20on%20pypi&style=flat-square)](https://pypi.org/project/discord-ext-pager/)
 
-A simple view-based paginator library for discord.py 2.0.
+A simple view-based paginator library for discord.py 2.0. Works with Python 3.8+.
 
-## Installation
+## Usage
 
 [discord-ext-pager] is available on PyPI, and as such can be installed using pip.
 
-[discord-ext-pager]: https://pypi.org/project/discord-ext-pager/
-
-## Usage
-
 Users of Danny's [discord-ext-menus] will find some familiarity
 in this library. Provided are the following classes:
 
 - PaginatorView:
   The view class that manages pagination and navigation.
 - PageSource:
   The base class for sources the paginator view can accept.
@@ -48,14 +45,15 @@
 - AsyncIteratorPageSource:
   The base class for formatting an asynchronous iterator of items.
 - PageOption:
   A subclass of `discord.SelectOption` used for presenting navigation options.
 - TimeoutAction:
   An enum for customizing PaginatorView's timeout behaviour.
 
+[discord-ext-pager]: https://pypi.org/project/discord-ext-pager/
 [discord-ext-menus]: https://github.com/Rapptz/discord-ext-menus
 
 The `PaginatorView` can be instantiated and used by itself, but page formatting
 is handled by subclassing one of the `PageSource` base classes.
 
 ```py
 from typing import Any, List
```

