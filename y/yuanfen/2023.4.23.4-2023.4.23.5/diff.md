# Comparing `tmp/yuanfen-2023.4.23.4.tar.gz` & `tmp/yuanfen-2023.4.23.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yuanfen-2023.4.23.4.tar", last modified: Sun Apr 23 08:36:41 2023, max compression
+gzip compressed data, was "yuanfen-2023.4.23.5.tar", last modified: Sun Apr 23 09:27:45 2023, max compression
```

## Comparing `yuanfen-2023.4.23.4.tar` & `yuanfen-2023.4.23.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 08:36:41.216824 yuanfen-2023.4.23.4/
--rw-r--r--   0 root         (0) root         (0)      968 2023-04-23 08:36:41.216824 yuanfen-2023.4.23.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      635 2023-04-23 08:17:06.000000 yuanfen-2023.4.23.4/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-23 08:36:41.216824 yuanfen-2023.4.23.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      647 2023-04-23 08:36:40.000000 yuanfen-2023.4.23.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 08:36:41.215824 yuanfen-2023.4.23.4/yuanfen/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-23 08:36:40.000000 yuanfen-2023.4.23.4/yuanfen/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1780 2023-04-23 08:17:06.000000 yuanfen-2023.4.23.4/yuanfen/config.py
--rw-rw-rw-   0 root         (0) root         (0)      804 2023-04-23 08:17:06.000000 yuanfen-2023.4.23.4/yuanfen/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 08:36:41.215824 yuanfen-2023.4.23.4/yuanfen.egg-info/
--rw-r--r--   0 root         (0) root         (0)      968 2023-04-23 08:36:41.000000 yuanfen-2023.4.23.4/yuanfen.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      228 2023-04-23 08:36:41.000000 yuanfen-2023.4.23.4/yuanfen.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 08:36:41.000000 yuanfen-2023.4.23.4/yuanfen.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-04-23 08:36:41.000000 yuanfen-2023.4.23.4/yuanfen.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-23 08:36:41.000000 yuanfen-2023.4.23.4/yuanfen.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 09:27:45.803781 yuanfen-2023.4.23.5/
+-rw-r--r--   0 root         (0) root         (0)      968 2023-04-23 09:27:45.803781 yuanfen-2023.4.23.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      635 2023-04-23 08:17:06.000000 yuanfen-2023.4.23.5/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-23 09:27:45.803781 yuanfen-2023.4.23.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      647 2023-04-23 08:36:40.000000 yuanfen-2023.4.23.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 09:27:45.803781 yuanfen-2023.4.23.5/yuanfen/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-23 09:27:44.000000 yuanfen-2023.4.23.5/yuanfen/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1780 2023-04-23 08:17:06.000000 yuanfen-2023.4.23.5/yuanfen/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      841 2023-04-23 09:27:44.000000 yuanfen-2023.4.23.5/yuanfen/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 09:27:45.803781 yuanfen-2023.4.23.5/yuanfen.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      968 2023-04-23 09:27:45.000000 yuanfen-2023.4.23.5/yuanfen.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      228 2023-04-23 09:27:45.000000 yuanfen-2023.4.23.5/yuanfen.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 09:27:45.000000 yuanfen-2023.4.23.5/yuanfen.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-04-23 09:27:45.000000 yuanfen-2023.4.23.5/yuanfen.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-23 09:27:45.000000 yuanfen-2023.4.23.5/yuanfen.egg-info/top_level.txt
```

### Comparing `yuanfen-2023.4.23.4/PKG-INFO` & `yuanfen-2023.4.23.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yuanfen
-Version: 2023.4.23.4
+Version: 2023.4.23.5
 Summary: Yuanfen Python Library
 Home-page: 
 Author: Bean
 Author-email: bean@yuanfen.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yuanfen-2023.4.23.4/README.md` & `yuanfen-2023.4.23.5/README.md`

 * *Files identical despite different names*

### Comparing `yuanfen-2023.4.23.4/setup.py` & `yuanfen-2023.4.23.5/setup.py`

 * *Files identical despite different names*

### Comparing `yuanfen-2023.4.23.4/yuanfen/config.py` & `yuanfen-2023.4.23.5/yuanfen/config.py`

 * *Files identical despite different names*

### Comparing `yuanfen-2023.4.23.4/yuanfen/logger.py` & `yuanfen-2023.4.23.5/yuanfen/logger.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 file_handler = TimedRotatingFileHandler(
     "logs/log",
     when="midnight",
     backupCount=365,
     encoding="utf-8",
 )
+file_handler.suffix = "%Y-%m-%d.log"
 file_handler.setFormatter(log_formatter)
 
 logger = logging.getLogger()
 logger.setLevel(level=logging.INFO)
 logger.addHandler(stream_handler)
 logger.addHandler(file_handler)
```

### Comparing `yuanfen-2023.4.23.4/yuanfen.egg-info/PKG-INFO` & `yuanfen-2023.4.23.5/yuanfen.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yuanfen
-Version: 2023.4.23.4
+Version: 2023.4.23.5
 Summary: Yuanfen Python Library
 Home-page: 
 Author: Bean
 Author-email: bean@yuanfen.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

