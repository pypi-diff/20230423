# Comparing `tmp/botterino-0.4.8.tar.gz` & `tmp/botterino-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botterino-0.4.8.tar", last modified: Sun Apr 23 06:21:18 2023, max compression
+gzip compressed data, was "botterino-0.4.9.tar", last modified: Sun Apr 23 06:34:58 2023, max compression
```

## Comparing `botterino-0.4.8.tar` & `botterino-0.4.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 adarsharegmi   (501) staff       (20)        0 2023-04-23 06:21:18.008434 botterino-0.4.8/
--rw-r--r--   0 adarsharegmi   (501) staff       (20)     1063 2021-06-10 02:59:26.000000 botterino-0.4.8/LICENSE
--rw-r--r--   0 adarsharegmi   (501) staff       (20)     5014 2023-04-23 06:21:18.009084 botterino-0.4.8/PKG-INFO
--rw-r--r--   0 adarsharegmi   (501) staff       (20)     4566 2022-08-30 05:36:56.000000 botterino-0.4.8/README.md
-drwxr-xr-x   0 adarsharegmi   (501) staff       (20)        0 2023-04-23 06:21:17.987075 botterino-0.4.8/botterino/
-drwxr-xr-x   0 adarsharegmi   (501) staff       (20)        0 2023-04-23 06:21:17.995619 botterino-0.4.8/botterino/Loader/
--rw-r--r--   0 adarsharegmi   (501) staff       (20)        0 2021-06-17 04:44:47.000000 botterino-0.4.8/botterino/Loader/__init__.py
--rw-r--r--   0 adarsharegmi   (501) staff       (20)      868 2023-04-23 04:36:39.000000 botterino-0.4.8/botterino/Loader/loader.py
-drwxr-xr-x   0 adarsharegmi   (501) staff       (20)        0 2023-04-23 06:21:17.999803 botterino-0.4.8/botterino/Map/
--rw-r--r--   0 adarsharegmi   (501) staff       (20)        0 2023-04-23 04:46:10.000000 botterino-0.4.8/botterino/Map/__init__.py
--rw-r--r--   0 adarsharegmi   (501) staff       (20)     1471 2023-04-23 06:15:24.000000 botterino-0.4.8/botterino/Map/map.py
-drwxr-xr-x   0 adarsharegmi   (501) staff       (20)        0 2023-04-23 06:21:18.004857 botterino-0.4.8/botterino/RedditPoller/
--rw-r--r--   0 adarsharegmi   (501) staff       (20)     1368 2023-04-23 04:36:39.000000 botterino-0.4.8/botterino/RedditPoller/RedditPoller.py
--rw-r--r--   0 adarsharegmi   (501) staff       (20)     2443 2023-04-23 04:36:39.000000 botterino-0.4.8/botterino/RedditPoller/Retry.py
--rw-r--r--   0 adarsharegmi   (501) staff       (20)        0 2020-10-17 08:27:10.000000 botterino-0.4.8/botterino/RedditPoller/__init__.py
-drwxr-xr-x   0 adarsharegmi   (501) staff       (20)        0 2023-04-23 06:21:18.006036 botterino-0.4.8/botterino/Utils/
--rw-r--r--   0 adarsharegmi   (501) staff       (20)        0 2021-04-08 15:21:02.000000 botterino-0.4.8/botterino/Utils/__init__.py
--rw-r--r--   0 adarsharegmi   (501) staff       (20)     3821 2023-04-23 04:36:39.000000 botterino-0.4.8/botterino/Utils/utils.py
--rw-r--r--   0 adarsharegmi   (501) staff       (20)     1508 2023-04-23 04:36:39.000000 botterino-0.4.8/botterino/__init__.py
--rw-r--r--   0 adarsharegmi   (501) staff       (20)       36 2023-04-23 04:36:39.000000 botterino-0.4.8/botterino/__main__.py
--rw-r--r--   0 adarsharegmi   (501) staff       (20)     2673 2023-04-23 04:36:39.000000 botterino-0.4.8/botterino/botterino.py
--rw-r--r--   0 adarsharegmi   (501) staff       (20)     3194 2023-04-23 06:14:00.000000 botterino-0.4.8/botterino/config.py
--rw-r--r--   0 adarsharegmi   (501) staff       (20)      544 2023-04-23 04:36:39.000000 botterino-0.4.8/botterino/failure.py
--rw-r--r--   0 adarsharegmi   (501) staff       (20)     6907 2023-04-23 06:15:17.000000 botterino-0.4.8/botterino/hosterino.py
--rw-r--r--   0 adarsharegmi   (501) staff       (20)     1127 2023-04-23 04:36:40.000000 botterino-0.4.8/botterino/posterino.py
--rw-r--r--   0 adarsharegmi   (501) staff       (20)     4615 2023-04-23 04:36:40.000000 botterino-0.4.8/botterino/ui.py
-drwxr-xr-x   0 adarsharegmi   (501) staff       (20)        0 2023-04-23 06:21:17.994415 botterino-0.4.8/botterino.egg-info/
--rw-r--r--   0 adarsharegmi   (501) staff       (20)     5014 2023-04-23 06:21:17.000000 botterino-0.4.8/botterino.egg-info/PKG-INFO
--rw-r--r--   0 adarsharegmi   (501) staff       (20)      638 2023-04-23 06:21:17.000000 botterino-0.4.8/botterino.egg-info/SOURCES.txt
--rw-r--r--   0 adarsharegmi   (501) staff       (20)        1 2023-04-23 06:21:17.000000 botterino-0.4.8/botterino.egg-info/dependency_links.txt
--rw-r--r--   0 adarsharegmi   (501) staff       (20)       70 2023-04-23 06:21:17.000000 botterino-0.4.8/botterino.egg-info/requires.txt
--rw-r--r--   0 adarsharegmi   (501) staff       (20)       10 2023-04-23 06:21:17.000000 botterino-0.4.8/botterino.egg-info/top_level.txt
--rw-r--r--   0 adarsharegmi   (501) staff       (20)      103 2021-06-10 03:23:33.000000 botterino-0.4.8/pyproject.toml
--rw-r--r--   0 adarsharegmi   (501) staff       (20)      636 2023-04-23 06:21:18.012091 botterino-0.4.8/setup.cfg
+drwxr-xr-x   0 adarsharegmi   (501) staff       (20)        0 2023-04-23 06:34:58.928062 botterino-0.4.9/
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     1063 2021-06-10 02:59:26.000000 botterino-0.4.9/LICENSE
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     5014 2023-04-23 06:34:58.928395 botterino-0.4.9/PKG-INFO
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     4566 2022-08-30 05:36:56.000000 botterino-0.4.9/README.md
+drwxr-xr-x   0 adarsharegmi   (501) staff       (20)        0 2023-04-23 06:34:58.848723 botterino-0.4.9/botterino/
+drwxr-xr-x   0 adarsharegmi   (501) staff       (20)        0 2023-04-23 06:34:58.876918 botterino-0.4.9/botterino/Loader/
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)        0 2021-06-17 04:44:47.000000 botterino-0.4.9/botterino/Loader/__init__.py
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)      868 2023-04-23 04:36:39.000000 botterino-0.4.9/botterino/Loader/loader.py
+drwxr-xr-x   0 adarsharegmi   (501) staff       (20)        0 2023-04-23 06:34:58.900572 botterino-0.4.9/botterino/Map/
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)        0 2023-04-23 04:46:10.000000 botterino-0.4.9/botterino/Map/__init__.py
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     1471 2023-04-23 06:15:24.000000 botterino-0.4.9/botterino/Map/map.py
+drwxr-xr-x   0 adarsharegmi   (501) staff       (20)        0 2023-04-23 06:34:58.924479 botterino-0.4.9/botterino/RedditPoller/
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     1368 2023-04-23 04:36:39.000000 botterino-0.4.9/botterino/RedditPoller/RedditPoller.py
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     2443 2023-04-23 04:36:39.000000 botterino-0.4.9/botterino/RedditPoller/Retry.py
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)        0 2020-10-17 08:27:10.000000 botterino-0.4.9/botterino/RedditPoller/__init__.py
+drwxr-xr-x   0 adarsharegmi   (501) staff       (20)        0 2023-04-23 06:34:58.926519 botterino-0.4.9/botterino/Utils/
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)        0 2021-04-08 15:21:02.000000 botterino-0.4.9/botterino/Utils/__init__.py
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     3821 2023-04-23 04:36:39.000000 botterino-0.4.9/botterino/Utils/utils.py
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     1508 2023-04-23 04:36:39.000000 botterino-0.4.9/botterino/__init__.py
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)       36 2023-04-23 04:36:39.000000 botterino-0.4.9/botterino/__main__.py
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     2673 2023-04-23 04:36:39.000000 botterino-0.4.9/botterino/botterino.py
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     3235 2023-04-23 06:32:23.000000 botterino-0.4.9/botterino/config.py
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)      544 2023-04-23 04:36:39.000000 botterino-0.4.9/botterino/failure.py
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     6907 2023-04-23 06:15:17.000000 botterino-0.4.9/botterino/hosterino.py
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     1127 2023-04-23 04:36:40.000000 botterino-0.4.9/botterino/posterino.py
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     4615 2023-04-23 04:36:40.000000 botterino-0.4.9/botterino/ui.py
+drwxr-xr-x   0 adarsharegmi   (501) staff       (20)        0 2023-04-23 06:34:58.869334 botterino-0.4.9/botterino.egg-info/
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     5014 2023-04-23 06:34:58.000000 botterino-0.4.9/botterino.egg-info/PKG-INFO
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)      638 2023-04-23 06:34:58.000000 botterino-0.4.9/botterino.egg-info/SOURCES.txt
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)        1 2023-04-23 06:34:58.000000 botterino-0.4.9/botterino.egg-info/dependency_links.txt
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)       70 2023-04-23 06:34:58.000000 botterino-0.4.9/botterino.egg-info/requires.txt
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)       10 2023-04-23 06:34:58.000000 botterino-0.4.9/botterino.egg-info/top_level.txt
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)      103 2021-06-10 03:23:33.000000 botterino-0.4.9/pyproject.toml
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)      636 2023-04-23 06:34:58.932513 botterino-0.4.9/setup.cfg
```

### Comparing `botterino-0.4.8/LICENSE` & `botterino-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `botterino-0.4.8/PKG-INFO` & `botterino-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botterino
-Version: 0.4.8
+Version: 0.4.9
 Summary: Automate posting and hosting of rounds on /r/picturegame
 Home-page: https://github.com/pgitox/botterino
 Author: itoxici
 Author-email: itox@picturegame.co
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `botterino-0.4.8/README.md` & `botterino-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `botterino-0.4.8/botterino/Loader/loader.py` & `botterino-0.4.9/botterino/Loader/loader.py`

 * *Files identical despite different names*

### Comparing `botterino-0.4.8/botterino/Map/map.py` & `botterino-0.4.9/botterino/Map/map.py`

 * *Files identical despite different names*

### Comparing `botterino-0.4.8/botterino/RedditPoller/RedditPoller.py` & `botterino-0.4.9/botterino/RedditPoller/RedditPoller.py`

 * *Files identical despite different names*

### Comparing `botterino-0.4.8/botterino/RedditPoller/Retry.py` & `botterino-0.4.9/botterino/RedditPoller/Retry.py`

 * *Files identical despite different names*

### Comparing `botterino-0.4.8/botterino/Utils/utils.py` & `botterino-0.4.9/botterino/Utils/utils.py`

 * *Files identical despite different names*

### Comparing `botterino-0.4.8/botterino/__init__.py` & `botterino-0.4.9/botterino/__init__.py`

 * *Files identical despite different names*

### Comparing `botterino-0.4.8/botterino/botterino.py` & `botterino-0.4.9/botterino/botterino.py`

 * *Files identical despite different names*

### Comparing `botterino-0.4.8/botterino/config.py` & `botterino-0.4.9/botterino/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import praw
 import os
 import sys
-from . import botfiles
+from . import botfiles, correctMessage, incorrectMessage, hints
 from sty import fg
 import random
 import webbrowser
 import socket
 
 
 def receive_connection():
```

### Comparing `botterino-0.4.8/botterino/failure.py` & `botterino-0.4.9/botterino/failure.py`

 * *Files identical despite different names*

### Comparing `botterino-0.4.8/botterino/hosterino.py` & `botterino-0.4.9/botterino/hosterino.py`

 * *Files identical despite different names*

### Comparing `botterino-0.4.8/botterino/posterino.py` & `botterino-0.4.9/botterino/posterino.py`

 * *Files identical despite different names*

### Comparing `botterino-0.4.8/botterino/ui.py` & `botterino-0.4.9/botterino/ui.py`

 * *Files identical despite different names*

### Comparing `botterino-0.4.8/botterino.egg-info/PKG-INFO` & `botterino-0.4.9/botterino.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botterino
-Version: 0.4.8
+Version: 0.4.9
 Summary: Automate posting and hosting of rounds on /r/picturegame
 Home-page: https://github.com/pgitox/botterino
 Author: itoxici
 Author-email: itox@picturegame.co
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `botterino-0.4.8/botterino.egg-info/SOURCES.txt` & `botterino-0.4.9/botterino.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botterino-0.4.8/setup.cfg` & `botterino-0.4.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = botterino
-version = 0.4.8
+version = 0.4.9
 author = itoxici
 author_email = itox@picturegame.co
 description = Automate posting and hosting of rounds on /r/picturegame
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pgitox/botterino
 classifiers =
```

