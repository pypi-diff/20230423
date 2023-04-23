# Comparing `tmp/yuanfen-2023.4.23.6.tar.gz` & `tmp/yuanfen-2023.4.23.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yuanfen-2023.4.23.6.tar", last modified: Sun Apr 23 10:31:01 2023, max compression
+gzip compressed data, was "yuanfen-2023.4.23.7.tar", last modified: Sun Apr 23 10:54:22 2023, max compression
```

## Comparing `yuanfen-2023.4.23.6.tar` & `yuanfen-2023.4.23.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 10:31:01.958498 yuanfen-2023.4.23.6/
--rw-r--r--   0 root         (0) root         (0)      968 2023-04-23 10:31:01.958498 yuanfen-2023.4.23.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      635 2023-04-23 08:17:06.000000 yuanfen-2023.4.23.6/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-23 10:31:01.958498 yuanfen-2023.4.23.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      647 2023-04-23 08:36:40.000000 yuanfen-2023.4.23.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 10:31:01.957498 yuanfen-2023.4.23.6/yuanfen/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-23 10:31:01.000000 yuanfen-2023.4.23.6/yuanfen/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1787 2023-04-23 10:31:01.000000 yuanfen-2023.4.23.6/yuanfen/config.py
--rw-rw-rw-   0 root         (0) root         (0)      841 2023-04-23 09:27:44.000000 yuanfen-2023.4.23.6/yuanfen/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 10:31:01.957498 yuanfen-2023.4.23.6/yuanfen.egg-info/
--rw-r--r--   0 root         (0) root         (0)      968 2023-04-23 10:31:01.000000 yuanfen-2023.4.23.6/yuanfen.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      228 2023-04-23 10:31:01.000000 yuanfen-2023.4.23.6/yuanfen.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 10:31:01.000000 yuanfen-2023.4.23.6/yuanfen.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-04-23 10:31:01.000000 yuanfen-2023.4.23.6/yuanfen.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-23 10:31:01.000000 yuanfen-2023.4.23.6/yuanfen.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 10:54:22.872555 yuanfen-2023.4.23.7/
+-rw-r--r--   0 root         (0) root         (0)     1019 2023-04-23 10:54:22.872555 yuanfen-2023.4.23.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      686 2023-04-23 10:54:21.000000 yuanfen-2023.4.23.7/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-23 10:54:22.872555 yuanfen-2023.4.23.7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      647 2023-04-23 08:36:40.000000 yuanfen-2023.4.23.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 10:54:22.871555 yuanfen-2023.4.23.7/yuanfen/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-23 10:54:21.000000 yuanfen-2023.4.23.7/yuanfen/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1787 2023-04-23 10:31:01.000000 yuanfen-2023.4.23.7/yuanfen/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      841 2023-04-23 09:27:44.000000 yuanfen-2023.4.23.7/yuanfen/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 10:54:22.871555 yuanfen-2023.4.23.7/yuanfen.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1019 2023-04-23 10:54:22.000000 yuanfen-2023.4.23.7/yuanfen.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      228 2023-04-23 10:54:22.000000 yuanfen-2023.4.23.7/yuanfen.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 10:54:22.000000 yuanfen-2023.4.23.7/yuanfen.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-04-23 10:54:22.000000 yuanfen-2023.4.23.7/yuanfen.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-23 10:54:22.000000 yuanfen-2023.4.23.7/yuanfen.egg-info/top_level.txt
```

### Comparing `yuanfen-2023.4.23.6/PKG-INFO` & `yuanfen-2023.4.23.7/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yuanfen
-Version: 2023.4.23.6
+Version: 2023.4.23.7
 Summary: Yuanfen Python Library
 Home-page: 
 Author: Bean
 Author-email: bean@yuanfen.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,17 +21,17 @@
 
 ## utils.config
 
 Support .json, .yaml, .ini files.
 Support auto reloading while config file changes.
 
 ```python
-config_json = Config("config.json")
-config_yaml = Config("config.yaml")
-config_ini = Config("config.ini")
+config_json = Config(os.path.abspath("config.json"))
+config_yaml = Config(os.path.abspath("config.yaml"))
+config_ini = Config(os.path.abspath("config.ini"))
 
 print(config_ini["app"]["config_a"])
 print(config_yaml["movie"]["name"])
 ```
 
 ## utils.logger
```

### Comparing `yuanfen-2023.4.23.6/README.md` & `yuanfen-2023.4.23.7/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 ## utils.config
 
 Support .json, .yaml, .ini files.
 Support auto reloading while config file changes.
 
 ```python
-config_json = Config("config.json")
-config_yaml = Config("config.yaml")
-config_ini = Config("config.ini")
+config_json = Config(os.path.abspath("config.json"))
+config_yaml = Config(os.path.abspath("config.yaml"))
+config_ini = Config(os.path.abspath("config.ini"))
 
 print(config_ini["app"]["config_a"])
 print(config_yaml["movie"]["name"])
 ```
 
 ## utils.logger
```

### Comparing `yuanfen-2023.4.23.6/setup.py` & `yuanfen-2023.4.23.7/setup.py`

 * *Files identical despite different names*

### Comparing `yuanfen-2023.4.23.6/yuanfen/config.py` & `yuanfen-2023.4.23.7/yuanfen/config.py`

 * *Files identical despite different names*

### Comparing `yuanfen-2023.4.23.6/yuanfen/logger.py` & `yuanfen-2023.4.23.7/yuanfen/logger.py`

 * *Files identical despite different names*

### Comparing `yuanfen-2023.4.23.6/yuanfen.egg-info/PKG-INFO` & `yuanfen-2023.4.23.7/yuanfen.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yuanfen
-Version: 2023.4.23.6
+Version: 2023.4.23.7
 Summary: Yuanfen Python Library
 Home-page: 
 Author: Bean
 Author-email: bean@yuanfen.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,17 +21,17 @@
 
 ## utils.config
 
 Support .json, .yaml, .ini files.
 Support auto reloading while config file changes.
 
 ```python
-config_json = Config("config.json")
-config_yaml = Config("config.yaml")
-config_ini = Config("config.ini")
+config_json = Config(os.path.abspath("config.json"))
+config_yaml = Config(os.path.abspath("config.yaml"))
+config_ini = Config(os.path.abspath("config.ini"))
 
 print(config_ini["app"]["config_a"])
 print(config_yaml["movie"]["name"])
 ```
 
 ## utils.logger
```

