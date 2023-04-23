# Comparing `tmp/telegram_util-0.0.98.tar.gz` & `tmp/telegram_util-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/telegram_util-0.0.98.tar", last modified: Tue Jun  9 03:14:39 2020, max compression
+gzip compressed data, was "dist/telegram_util-0.0.99.tar", last modified: Fri Jun 12 15:16:32 2020, max compression
```

## Comparing `telegram_util-0.0.98.tar` & `telegram_util-0.0.99.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2020-06-09 03:14:39.000000 telegram_util-0.0.98/
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      619 2020-06-09 03:14:39.000000 telegram_util-0.0.98/PKG-INFO
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      124 2019-11-12 07:01:42.000000 telegram_util-0.0.98/README.md
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       38 2020-06-09 03:14:39.000000 telegram_util-0.0.98/setup.cfg
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      681 2020-06-09 03:14:32.000000 telegram_util-0.0.98/setup.py
-drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2020-06-09 03:14:39.000000 telegram_util-0.0.98/telegram_util/
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)     7948 2020-06-09 03:14:27.000000 telegram_util-0.0.98/telegram_util/__init__.py
-drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2020-06-09 03:14:39.000000 telegram_util-0.0.98/telegram_util.egg-info/
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      619 2020-06-09 03:14:39.000000 telegram_util-0.0.98/telegram_util.egg-info/PKG-INFO
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      228 2020-06-09 03:14:39.000000 telegram_util-0.0.98/telegram_util.egg-info/SOURCES.txt
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)        1 2020-06-09 03:14:39.000000 telegram_util-0.0.98/telegram_util.egg-info/dependency_links.txt
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)        4 2020-06-09 03:14:39.000000 telegram_util-0.0.98/telegram_util.egg-info/requires.txt
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       14 2020-06-09 03:14:39.000000 telegram_util-0.0.98/telegram_util.egg-info/top_level.txt
+drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2020-06-12 15:16:32.000000 telegram_util-0.0.99/
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      619 2020-06-12 15:16:32.000000 telegram_util-0.0.99/PKG-INFO
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      124 2019-11-12 07:01:42.000000 telegram_util-0.0.99/README.md
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       38 2020-06-12 15:16:32.000000 telegram_util-0.0.99/setup.cfg
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      681 2020-06-12 15:16:30.000000 telegram_util-0.0.99/setup.py
+drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2020-06-12 15:16:32.000000 telegram_util-0.0.99/telegram_util/
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)     7964 2020-06-12 15:16:22.000000 telegram_util-0.0.99/telegram_util/__init__.py
+drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2020-06-12 15:16:32.000000 telegram_util-0.0.99/telegram_util.egg-info/
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      619 2020-06-12 15:16:32.000000 telegram_util-0.0.99/telegram_util.egg-info/PKG-INFO
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      228 2020-06-12 15:16:32.000000 telegram_util-0.0.99/telegram_util.egg-info/SOURCES.txt
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)        1 2020-06-12 15:16:32.000000 telegram_util-0.0.99/telegram_util.egg-info/dependency_links.txt
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)        4 2020-06-12 15:16:32.000000 telegram_util-0.0.99/telegram_util.egg-info/requires.txt
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       14 2020-06-12 15:16:32.000000 telegram_util-0.0.99/telegram_util.egg-info/top_level.txt
```

### Comparing `telegram_util-0.0.98/PKG-INFO` & `telegram_util-0.0.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telegram_util
-Version: 0.0.98
+Version: 0.0.99
 Summary: Telegram Util.
 Home-page: https://github.com/gaoyunzhi/telegram_util
 Author: Yunzhi Gao
 Author-email: gaoyunzhi@gmail.com
 License: UNKNOWN
 Description: # telegram_util
```

### Comparing `telegram_util-0.0.98/setup.py` & `telegram_util-0.0.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="telegram_util",
-    version="0.0.98",
+    version="0.0.99",
     author="Yunzhi Gao",
     author_email="gaoyunzhi@gmail.com",
     description="Telegram Util.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gaoyunzhi/telegram_util",
     packages=setuptools.find_packages(),
```

### Comparing `telegram_util-0.0.98/telegram_util/__init__.py` & `telegram_util-0.0.99/telegram_util/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 		self.cap = ''
 		self.video = ''
 		self.cap_html = '' # weibo status only
 		self.title = '' # weibo status only
 		self.wid = '' # weibo status only 
 		self.rwid = '' # weibo status only retweet id
 		self.hash = ''
+		self.url = ''
 
 	def empty(self):
 		return (not self.imgs) and (not self.cap) and (not self.video)
 
 	def __str__(self):
 		return '\t'.join([k + ':' + str(v) for (k,v) in self.__dict__.items() if v])
```

### Comparing `telegram_util-0.0.98/telegram_util.egg-info/PKG-INFO` & `telegram_util-0.0.99/telegram_util.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telegram-util
-Version: 0.0.98
+Version: 0.0.99
 Summary: Telegram Util.
 Home-page: https://github.com/gaoyunzhi/telegram_util
 Author: Yunzhi Gao
 Author-email: gaoyunzhi@gmail.com
 License: UNKNOWN
 Description: # telegram_util
```

