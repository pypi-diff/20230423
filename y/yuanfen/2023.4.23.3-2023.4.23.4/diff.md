# Comparing `tmp/yuanfen-2023.4.23.3.tar.gz` & `tmp/yuanfen-2023.4.23.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yuanfen-2023.4.23.3.tar", last modified: Sun Apr 23 08:29:59 2023, max compression
+gzip compressed data, was "yuanfen-2023.4.23.4.tar", last modified: Sun Apr 23 08:36:41 2023, max compression
```

## Comparing `yuanfen-2023.4.23.3.tar` & `yuanfen-2023.4.23.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 08:29:59.955958 yuanfen-2023.4.23.3/
--rw-r--r--   0 root         (0) root         (0)      968 2023-04-23 08:29:59.954958 yuanfen-2023.4.23.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      635 2023-04-23 08:17:06.000000 yuanfen-2023.4.23.3/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-23 08:29:59.955958 yuanfen-2023.4.23.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      645 2023-04-23 08:17:06.000000 yuanfen-2023.4.23.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 08:29:59.953958 yuanfen-2023.4.23.3/yuanfen/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-23 08:29:59.000000 yuanfen-2023.4.23.3/yuanfen/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1780 2023-04-23 08:17:06.000000 yuanfen-2023.4.23.3/yuanfen/config.py
--rw-rw-rw-   0 root         (0) root         (0)      804 2023-04-23 08:17:06.000000 yuanfen-2023.4.23.3/yuanfen/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 08:29:59.954958 yuanfen-2023.4.23.3/yuanfen.egg-info/
--rw-r--r--   0 root         (0) root         (0)      968 2023-04-23 08:29:59.000000 yuanfen-2023.4.23.3/yuanfen.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      228 2023-04-23 08:29:59.000000 yuanfen-2023.4.23.3/yuanfen.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 08:29:59.000000 yuanfen-2023.4.23.3/yuanfen.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-04-23 08:29:59.000000 yuanfen-2023.4.23.3/yuanfen.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-23 08:29:59.000000 yuanfen-2023.4.23.3/yuanfen.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 08:36:41.216824 yuanfen-2023.4.23.4/
+-rw-r--r--   0 root         (0) root         (0)      968 2023-04-23 08:36:41.216824 yuanfen-2023.4.23.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      635 2023-04-23 08:17:06.000000 yuanfen-2023.4.23.4/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-23 08:36:41.216824 yuanfen-2023.4.23.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      647 2023-04-23 08:36:40.000000 yuanfen-2023.4.23.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 08:36:41.215824 yuanfen-2023.4.23.4/yuanfen/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-23 08:36:40.000000 yuanfen-2023.4.23.4/yuanfen/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1780 2023-04-23 08:17:06.000000 yuanfen-2023.4.23.4/yuanfen/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      804 2023-04-23 08:17:06.000000 yuanfen-2023.4.23.4/yuanfen/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 08:36:41.215824 yuanfen-2023.4.23.4/yuanfen.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      968 2023-04-23 08:36:41.000000 yuanfen-2023.4.23.4/yuanfen.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      228 2023-04-23 08:36:41.000000 yuanfen-2023.4.23.4/yuanfen.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 08:36:41.000000 yuanfen-2023.4.23.4/yuanfen.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-04-23 08:36:41.000000 yuanfen-2023.4.23.4/yuanfen.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-23 08:36:41.000000 yuanfen-2023.4.23.4/yuanfen.egg-info/top_level.txt
```

### Comparing `yuanfen-2023.4.23.3/PKG-INFO` & `yuanfen-2023.4.23.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yuanfen
-Version: 2023.4.23.3
+Version: 2023.4.23.4
 Summary: Yuanfen Python Library
 Home-page: 
 Author: Bean
 Author-email: bean@yuanfen.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yuanfen-2023.4.23.3/README.md` & `yuanfen-2023.4.23.4/README.md`

 * *Files identical despite different names*

### Comparing `yuanfen-2023.4.23.3/setup.py` & `yuanfen-2023.4.23.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     version=os.environ.get("CI_COMMIT_TAG", "0.0.0"),
     author="Bean",
     author_email="bean@yuanfen.net",
     description="Yuanfen Python Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
-    install_requires=["yaml", "watchdog"],
+    install_requires=["pyyaml", "watchdog"],
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```

### Comparing `yuanfen-2023.4.23.3/yuanfen/config.py` & `yuanfen-2023.4.23.4/yuanfen/config.py`

 * *Files identical despite different names*

### Comparing `yuanfen-2023.4.23.3/yuanfen/logger.py` & `yuanfen-2023.4.23.4/yuanfen/logger.py`

 * *Files identical despite different names*

### Comparing `yuanfen-2023.4.23.3/yuanfen.egg-info/PKG-INFO` & `yuanfen-2023.4.23.4/yuanfen.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yuanfen
-Version: 2023.4.23.3
+Version: 2023.4.23.4
 Summary: Yuanfen Python Library
 Home-page: 
 Author: Bean
 Author-email: bean@yuanfen.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

