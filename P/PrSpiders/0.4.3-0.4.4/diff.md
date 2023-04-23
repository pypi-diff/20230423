# Comparing `tmp/PrSpiders-0.4.3.tar.gz` & `tmp/PrSpiders-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PrSpiders-0.4.3.tar", last modified: Sun Apr 23 03:20:50 2023, max compression
+gzip compressed data, was "PrSpiders-0.4.4.tar", last modified: Sun Apr 23 03:23:39 2023, max compression
```

## Comparing `PrSpiders-0.4.3.tar` & `PrSpiders-0.4.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 03:20:50.391813 PrSpiders-0.4.3/
--rw-rw-rw-   0        0        0     1091 2023-02-21 09:22:44.000000 PrSpiders-0.4.3/LICENSE.txt
--rw-rw-rw-   0        0        0     4583 2023-04-23 03:20:50.388810 PrSpiders-0.4.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-23 03:20:50.157814 PrSpiders-0.4.3/PrSpider/
--rw-rw-rw-   0        0        0    11323 2023-04-21 05:29:18.000000 PrSpiders-0.4.3/PrSpider/PrSpiders.py
--rw-rw-rw-   0        0        0       44 2023-03-28 05:34:05.000000 PrSpiders-0.4.3/PrSpider/__init__.py
--rw-rw-rw-   0        0        0    11024 2023-04-23 03:20:27.000000 PrSpiders-0.4.3/PrSpider/pxpath.py
--rw-rw-rw-   0        0        0     4527 2023-04-21 06:07:41.000000 PrSpiders-0.4.3/PrSpider/requestXpath.py
--rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.4.3/PrSpider/useragent.py
-drwxrwxrwx   0        0        0        0 2023-04-23 03:20:50.236809 PrSpiders-0.4.3/PrSpiders.egg-info/
--rw-rw-rw-   0        0        0     4583 2023-04-23 03:20:49.000000 PrSpiders-0.4.3/PrSpiders.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      563 2023-04-23 03:20:49.000000 PrSpiders-0.4.3/PrSpiders.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 03:20:49.000000 PrSpiders-0.4.3/PrSpiders.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-04-23 03:20:49.000000 PrSpiders-0.4.3/PrSpiders.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       40 2023-04-23 03:20:49.000000 PrSpiders-0.4.3/PrSpiders.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-04-23 03:20:49.000000 PrSpiders-0.4.3/PrSpiders.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4071 2023-04-18 02:48:25.000000 PrSpiders-0.4.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 03:20:50.242809 PrSpiders-0.4.3/pkg/
--rw-rw-rw-   0        0        0       23 2023-04-23 03:20:35.000000 PrSpiders-0.4.3/pkg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 03:20:50.303813 PrSpiders-0.4.3/pkg/prspider/
--rw-rw-rw-   0        0        0     1212 2023-04-20 09:13:43.000000 PrSpiders-0.4.3/pkg/prspider/PrSpider_CMD.py
--rw-rw-rw-   0        0        0      257 2023-04-17 12:23:25.000000 PrSpiders-0.4.3/pkg/prspider/PrSpider_run.py
--rw-rw-rw-   0        0        0       73 2023-03-31 05:29:27.000000 PrSpiders-0.4.3/pkg/prspider/__init__.py
--rw-rw-rw-   0        0        0      908 2023-04-21 05:38:54.000000 PrSpiders-0.4.3/pkg/prspider/start.py
-drwxrwxrwx   0        0        0        0 2023-04-23 03:20:50.373814 PrSpiders-0.4.3/requestXpath/
--rw-rw-rw-   0        0        0      933 2023-03-23 08:11:59.000000 PrSpiders-0.4.3/requestXpath/__init__.py
--rw-rw-rw-   0        0        0     8642 2023-04-18 08:44:05.000000 PrSpiders-0.4.3/requestXpath/pxpath.py
--rw-rw-rw-   0        0        0     4210 2023-03-23 08:11:59.000000 PrSpiders-0.4.3/requestXpath/requestXpath.py
--rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.4.3/requestXpath/useragent.py
--rw-rw-rw-   0        0        0       42 2023-04-23 03:20:50.396817 PrSpiders-0.4.3/setup.cfg
--rw-rw-rw-   0        0        0     1022 2023-04-23 03:20:42.000000 PrSpiders-0.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:23:39.163632 PrSpiders-0.4.4/
+-rw-rw-rw-   0        0        0     1091 2023-02-21 09:22:44.000000 PrSpiders-0.4.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     4583 2023-04-23 03:23:39.157626 PrSpiders-0.4.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-23 03:23:38.929631 PrSpiders-0.4.4/PrSpider/
+-rw-rw-rw-   0        0        0    11323 2023-04-21 05:29:18.000000 PrSpiders-0.4.4/PrSpider/PrSpiders.py
+-rw-rw-rw-   0        0        0       44 2023-03-28 05:34:05.000000 PrSpiders-0.4.4/PrSpider/__init__.py
+-rw-rw-rw-   0        0        0    11024 2023-04-23 03:20:27.000000 PrSpiders-0.4.4/PrSpider/pxpath.py
+-rw-rw-rw-   0        0        0     4527 2023-04-21 06:07:41.000000 PrSpiders-0.4.4/PrSpider/requestXpath.py
+-rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.4.4/PrSpider/useragent.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:23:39.006630 PrSpiders-0.4.4/PrSpiders.egg-info/
+-rw-rw-rw-   0        0        0     4583 2023-04-23 03:23:38.000000 PrSpiders-0.4.4/PrSpiders.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      563 2023-04-23 03:23:38.000000 PrSpiders-0.4.4/PrSpiders.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 03:23:38.000000 PrSpiders-0.4.4/PrSpiders.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-04-23 03:23:38.000000 PrSpiders-0.4.4/PrSpiders.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       40 2023-04-23 03:23:38.000000 PrSpiders-0.4.4/PrSpiders.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-04-23 03:23:38.000000 PrSpiders-0.4.4/PrSpiders.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4071 2023-04-18 02:48:25.000000 PrSpiders-0.4.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 03:23:39.026631 PrSpiders-0.4.4/pkg/
+-rw-rw-rw-   0        0        0       23 2023-04-23 03:23:07.000000 PrSpiders-0.4.4/pkg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:23:39.095630 PrSpiders-0.4.4/pkg/prspider/
+-rw-rw-rw-   0        0        0     1212 2023-04-20 09:13:43.000000 PrSpiders-0.4.4/pkg/prspider/PrSpider_CMD.py
+-rw-rw-rw-   0        0        0      257 2023-04-17 12:23:25.000000 PrSpiders-0.4.4/pkg/prspider/PrSpider_run.py
+-rw-rw-rw-   0        0        0       73 2023-03-31 05:29:27.000000 PrSpiders-0.4.4/pkg/prspider/__init__.py
+-rw-rw-rw-   0        0        0      833 2023-04-23 03:22:54.000000 PrSpiders-0.4.4/pkg/prspider/start.py
+drwxrwxrwx   0        0        0        0 2023-04-23 03:23:39.142626 PrSpiders-0.4.4/requestXpath/
+-rw-rw-rw-   0        0        0      933 2023-03-23 08:11:59.000000 PrSpiders-0.4.4/requestXpath/__init__.py
+-rw-rw-rw-   0        0        0     8642 2023-04-18 08:44:05.000000 PrSpiders-0.4.4/requestXpath/pxpath.py
+-rw-rw-rw-   0        0        0     4210 2023-03-23 08:11:59.000000 PrSpiders-0.4.4/requestXpath/requestXpath.py
+-rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.4.4/requestXpath/useragent.py
+-rw-rw-rw-   0        0        0       42 2023-04-23 03:23:39.164628 PrSpiders-0.4.4/setup.cfg
+-rw-rw-rw-   0        0        0     1022 2023-04-23 03:23:08.000000 PrSpiders-0.4.4/setup.py
```

### Comparing `PrSpiders-0.4.3/LICENSE.txt` & `PrSpiders-0.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.4.3/PKG-INFO` & `PrSpiders-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrSpiders
-Version: 0.4.3
+Version: 0.4.4
 Summary: Inherit the requests module, add xpath functionality to expand the API, and handle request failures and retries
 Home-page: https://github.com/peng0928/prequests
 Author: penr
 Author-email: 1944542244@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `PrSpiders-0.4.3/PrSpider/PrSpiders.py` & `PrSpiders-0.4.4/PrSpider/PrSpiders.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.4.3/PrSpider/pxpath.py` & `PrSpiders-0.4.4/PrSpider/pxpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.4.3/PrSpider/requestXpath.py` & `PrSpiders-0.4.4/PrSpider/requestXpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.4.3/PrSpider/useragent.py` & `PrSpiders-0.4.4/PrSpider/useragent.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.4.3/PrSpiders.egg-info/PKG-INFO` & `PrSpiders-0.4.4/PrSpiders.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrSpiders
-Version: 0.4.3
+Version: 0.4.4
 Summary: Inherit the requests module, add xpath functionality to expand the API, and handle request failures and retries
 Home-page: https://github.com/peng0928/prequests
 Author: penr
 Author-email: 1944542244@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `PrSpiders-0.4.3/PrSpiders.egg-info/SOURCES.txt` & `PrSpiders-0.4.4/PrSpiders.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.4.3/README.md` & `PrSpiders-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.4.3/pkg/prspider/PrSpider_CMD.py` & `PrSpiders-0.4.4/pkg/prspider/PrSpider_CMD.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.4.3/pkg/prspider/start.py` & `PrSpiders-0.4.4/pkg/prspider/start.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,10 +31,7 @@
 
     def start_requests(self, **kwargs):
         PrSpiders.Requests(url=self.url, callback=self.parse)
 
     def parse(self, response):
         print(response.text)
         print(response)
-
-
-spider("https://blog.csdn.net/qq_43428929/article/details/126153264")
```

### Comparing `PrSpiders-0.4.3/requestXpath/__init__.py` & `PrSpiders-0.4.4/requestXpath/__init__.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.4.3/requestXpath/pxpath.py` & `PrSpiders-0.4.4/requestXpath/pxpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.4.3/requestXpath/requestXpath.py` & `PrSpiders-0.4.4/requestXpath/requestXpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.4.3/requestXpath/useragent.py` & `PrSpiders-0.4.4/requestXpath/useragent.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.4.3/setup.py` & `PrSpiders-0.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!python
 # -*- coding:utf-8 -*-
 from __future__ import print_function
 from setuptools import setup, find_packages
 
-__version__ = "0.4.3"
+__version__ = "0.4.4"
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="PrSpiders",
     version=__version__,
```

