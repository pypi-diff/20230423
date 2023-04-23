# Comparing `tmp/bingImageSpiderCreatedByHanXu-0.0.1.tar.gz` & `tmp/bingImageSpiderCreatedByHanXu-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bingImageSpiderCreatedByHanXu-0.0.1.tar", last modified: Sun Apr 23 13:44:11 2023, max compression
+gzip compressed data, was "bingImageSpiderCreatedByHanXu-0.0.2.tar", last modified: Sun Apr 23 13:57:51 2023, max compression
```

## Comparing `bingImageSpiderCreatedByHanXu-0.0.1.tar` & `bingImageSpiderCreatedByHanXu-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 13:44:11.918558 bingImageSpiderCreatedByHanXu-0.0.1/
--rw-rw-rw-   0        0        0     1090 2023-04-23 13:10:22.000000 bingImageSpiderCreatedByHanXu-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1441 2023-04-23 13:44:11.918558 bingImageSpiderCreatedByHanXu-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      478 2023-04-23 13:42:59.000000 bingImageSpiderCreatedByHanXu-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 13:44:11.902108 bingImageSpiderCreatedByHanXu-0.0.1/bingImageSpiderCreatedByHanXu/
--rw-rw-rw-   0        0        0     3762 2023-04-23 13:39:10.000000 bingImageSpiderCreatedByHanXu-0.0.1/bingImageSpiderCreatedByHanXu/Spider.py
--rw-rw-rw-   0        0        0        0 2023-04-23 13:39:10.000000 bingImageSpiderCreatedByHanXu-0.0.1/bingImageSpiderCreatedByHanXu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 13:44:11.916561 bingImageSpiderCreatedByHanXu-0.0.1/bingImageSpiderCreatedByHanXu.egg-info/
--rw-rw-rw-   0        0        0     1441 2023-04-23 13:44:11.000000 bingImageSpiderCreatedByHanXu-0.0.1/bingImageSpiderCreatedByHanXu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2023-04-23 13:44:11.000000 bingImageSpiderCreatedByHanXu-0.0.1/bingImageSpiderCreatedByHanXu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 13:44:11.000000 bingImageSpiderCreatedByHanXu-0.0.1/bingImageSpiderCreatedByHanXu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-23 13:44:11.000000 bingImageSpiderCreatedByHanXu-0.0.1/bingImageSpiderCreatedByHanXu.egg-info/requires.txt
--rw-rw-rw-   0        0        0       30 2023-04-23 13:44:11.000000 bingImageSpiderCreatedByHanXu-0.0.1/bingImageSpiderCreatedByHanXu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 13:44:11.918558 bingImageSpiderCreatedByHanXu-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     4248 2023-04-23 13:42:59.000000 bingImageSpiderCreatedByHanXu-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 13:57:51.622903 bingImageSpiderCreatedByHanXu-0.0.2/
+-rw-rw-rw-   0        0        0     1090 2023-04-23 13:10:22.000000 bingImageSpiderCreatedByHanXu-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1527 2023-04-23 13:57:51.622903 bingImageSpiderCreatedByHanXu-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      548 2023-04-23 13:56:09.000000 bingImageSpiderCreatedByHanXu-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 13:57:51.607902 bingImageSpiderCreatedByHanXu-0.0.2/bingImageSpiderCreatedByHanXu/
+-rw-rw-rw-   0        0        0     3762 2023-04-23 13:39:10.000000 bingImageSpiderCreatedByHanXu-0.0.2/bingImageSpiderCreatedByHanXu/Spider.py
+-rw-rw-rw-   0        0        0        0 2023-04-23 13:39:10.000000 bingImageSpiderCreatedByHanXu-0.0.2/bingImageSpiderCreatedByHanXu/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 13:57:51.618904 bingImageSpiderCreatedByHanXu-0.0.2/bingImageSpiderCreatedByHanXu.egg-info/
+-rw-rw-rw-   0        0        0     1527 2023-04-23 13:57:51.000000 bingImageSpiderCreatedByHanXu-0.0.2/bingImageSpiderCreatedByHanXu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2023-04-23 13:57:51.000000 bingImageSpiderCreatedByHanXu-0.0.2/bingImageSpiderCreatedByHanXu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 13:57:51.000000 bingImageSpiderCreatedByHanXu-0.0.2/bingImageSpiderCreatedByHanXu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-23 13:57:51.000000 bingImageSpiderCreatedByHanXu-0.0.2/bingImageSpiderCreatedByHanXu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       30 2023-04-23 13:57:51.000000 bingImageSpiderCreatedByHanXu-0.0.2/bingImageSpiderCreatedByHanXu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 13:57:51.622903 bingImageSpiderCreatedByHanXu-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     4264 2023-04-23 13:57:50.000000 bingImageSpiderCreatedByHanXu-0.0.2/setup.py
```

### Comparing `bingImageSpiderCreatedByHanXu-0.0.1/LICENSE` & `bingImageSpiderCreatedByHanXu-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bingImageSpiderCreatedByHanXu-0.0.1/PKG-INFO` & `bingImageSpiderCreatedByHanXu-0.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: bingImageSpiderCreatedByHanXu
-Version: 0.0.1
+Version: 0.0.2
 Summary: get a large mount of images at Bing.
 Home-page: https://gitee.com/UnderTurrets/bing-image-spider
 Author: Han Xu
 Author-email: 736946693@qq.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
-Classifier: Topic :: Software Development :: Build Tools
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
@@ -32,7 +32,11 @@
     ex()
 ```
 ```shell
 type in the path where you want to reserve the images:秋山澪
 type in the keywords used to search in bing:秋山澪
 Type in the number of pages you want.Each page has almost 30 images:1
 ```
+# Download
+```shell
+pip install bingImageSpiderCreatedByHanXu
+```
```

### Comparing `bingImageSpiderCreatedByHanXu-0.0.1/bingImageSpiderCreatedByHanXu/Spider.py` & `bingImageSpiderCreatedByHanXu-0.0.2/bingImageSpiderCreatedByHanXu/Spider.py`

 * *Files identical despite different names*

### Comparing `bingImageSpiderCreatedByHanXu-0.0.1/bingImageSpiderCreatedByHanXu.egg-info/PKG-INFO` & `bingImageSpiderCreatedByHanXu-0.0.2/bingImageSpiderCreatedByHanXu.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: bingImageSpiderCreatedByHanXu
-Version: 0.0.1
+Version: 0.0.2
 Summary: get a large mount of images at Bing.
 Home-page: https://gitee.com/UnderTurrets/bing-image-spider
 Author: Han Xu
 Author-email: 736946693@qq.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
-Classifier: Topic :: Software Development :: Build Tools
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
@@ -32,7 +32,11 @@
     ex()
 ```
 ```shell
 type in the path where you want to reserve the images:秋山澪
 type in the keywords used to search in bing:秋山澪
 Type in the number of pages you want.Each page has almost 30 images:1
 ```
+# Download
+```shell
+pip install bingImageSpiderCreatedByHanXu
+```
```

### Comparing `bingImageSpiderCreatedByHanXu-0.0.1/setup.py` & `bingImageSpiderCreatedByHanXu-0.0.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         # Intended Audience :: Education
         # Intended Audience :: End Users/Desktop
         # Intended Audience :: Financial and Insurance Industry
         # Intended Audience :: Healthcare Industry
         "Intended Audience :: End Users/Desktop",
 
         # 属于什么类型
-        "Topic :: Software Development :: Build Tools",
+        "Topic :: Software Development :: Libraries :: Python Modules",
 
         # 许可证信息
         "License :: OSI Approved :: MIT License",
 
         # 目标编程语言
         # Programming Language :: Basic
         # Programming Language :: C
@@ -49,15 +49,15 @@
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
     ],
 
     #如果上传时出现ERROR：The user '' isn't allowed to upload to project ''，换个名字，长一点无所谓，不能跟别人重复
     name="bingImageSpiderCreatedByHanXu",
-    version="0.0.1",
+    version="0.0.2",
     author="Han Xu",
     author_email="736946693@qq.com",
     description="get a large mount of images at Bing.",
 
     long_description=long_description,
     #README.md文本的格式，如果希望使用markdown语言就需要下面这句话
     long_description_content_type="text/markdown",
```

