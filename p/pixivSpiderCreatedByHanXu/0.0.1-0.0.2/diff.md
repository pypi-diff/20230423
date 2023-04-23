# Comparing `tmp/pixivSpiderCreatedByHanXu-0.0.1.tar.gz` & `tmp/pixivSpiderCreatedByHanXu-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixivSpiderCreatedByHanXu-0.0.1.tar", last modified: Sun Apr 23 13:32:17 2023, max compression
+gzip compressed data, was "pixivSpiderCreatedByHanXu-0.0.2.tar", last modified: Sun Apr 23 13:35:56 2023, max compression
```

## Comparing `pixivSpiderCreatedByHanXu-0.0.1.tar` & `pixivSpiderCreatedByHanXu-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 13:32:17.681662 pixivSpiderCreatedByHanXu-0.0.1/
--rw-rw-rw-   0        0        0     1090 2023-04-23 03:47:51.000000 pixivSpiderCreatedByHanXu-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     2192 2023-04-23 13:32:17.681662 pixivSpiderCreatedByHanXu-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1275 2023-04-23 13:29:21.000000 pixivSpiderCreatedByHanXu-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 13:32:17.662663 pixivSpiderCreatedByHanXu-0.0.1/pixivSpiderCreatedByHanXu/
--rw-rw-rw-   0        0        0        0 2023-04-23 13:11:37.000000 pixivSpiderCreatedByHanXu-0.0.1/pixivSpiderCreatedByHanXu/__init__.py
--rw-rw-rw-   0        0        0     4989 2023-04-23 13:32:13.000000 pixivSpiderCreatedByHanXu-0.0.1/pixivSpiderCreatedByHanXu/keywordSpider.py
--rw-rw-rw-   0        0        0     4220 2023-04-23 13:18:59.000000 pixivSpiderCreatedByHanXu-0.0.1/pixivSpiderCreatedByHanXu/rankSpider.py
-drwxrwxrwx   0        0        0        0 2023-04-23 13:32:17.680679 pixivSpiderCreatedByHanXu-0.0.1/pixivSpiderCreatedByHanXu.egg-info/
--rw-rw-rw-   0        0        0     2192 2023-04-23 13:32:17.000000 pixivSpiderCreatedByHanXu-0.0.1/pixivSpiderCreatedByHanXu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      391 2023-04-23 13:32:17.000000 pixivSpiderCreatedByHanXu-0.0.1/pixivSpiderCreatedByHanXu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 13:32:17.000000 pixivSpiderCreatedByHanXu-0.0.1/pixivSpiderCreatedByHanXu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-23 13:32:17.000000 pixivSpiderCreatedByHanXu-0.0.1/pixivSpiderCreatedByHanXu.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-04-23 13:32:17.000000 pixivSpiderCreatedByHanXu-0.0.1/pixivSpiderCreatedByHanXu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 13:32:17.681662 pixivSpiderCreatedByHanXu-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     4267 2023-04-23 13:32:13.000000 pixivSpiderCreatedByHanXu-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 13:35:56.467869 pixivSpiderCreatedByHanXu-0.0.2/
+-rw-rw-rw-   0        0        0     1090 2023-04-23 03:47:51.000000 pixivSpiderCreatedByHanXu-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2285 2023-04-23 13:35:56.467869 pixivSpiderCreatedByHanXu-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1312 2023-04-23 13:35:13.000000 pixivSpiderCreatedByHanXu-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 13:35:56.455870 pixivSpiderCreatedByHanXu-0.0.2/pixivSpiderCreatedByHanXu/
+-rw-rw-rw-   0        0        0        0 2023-04-23 13:11:37.000000 pixivSpiderCreatedByHanXu-0.0.2/pixivSpiderCreatedByHanXu/__init__.py
+-rw-rw-rw-   0        0        0     4989 2023-04-23 13:32:13.000000 pixivSpiderCreatedByHanXu-0.0.2/pixivSpiderCreatedByHanXu/keywordSpider.py
+-rw-rw-rw-   0        0        0     4220 2023-04-23 13:18:59.000000 pixivSpiderCreatedByHanXu-0.0.2/pixivSpiderCreatedByHanXu/rankSpider.py
+drwxrwxrwx   0        0        0        0 2023-04-23 13:35:56.466870 pixivSpiderCreatedByHanXu-0.0.2/pixivSpiderCreatedByHanXu.egg-info/
+-rw-rw-rw-   0        0        0     2285 2023-04-23 13:35:56.000000 pixivSpiderCreatedByHanXu-0.0.2/pixivSpiderCreatedByHanXu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      391 2023-04-23 13:35:56.000000 pixivSpiderCreatedByHanXu-0.0.2/pixivSpiderCreatedByHanXu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 13:35:56.000000 pixivSpiderCreatedByHanXu-0.0.2/pixivSpiderCreatedByHanXu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-23 13:35:56.000000 pixivSpiderCreatedByHanXu-0.0.2/pixivSpiderCreatedByHanXu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-04-23 13:35:56.000000 pixivSpiderCreatedByHanXu-0.0.2/pixivSpiderCreatedByHanXu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 13:35:56.467869 pixivSpiderCreatedByHanXu-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     4308 2023-04-23 13:35:51.000000 pixivSpiderCreatedByHanXu-0.0.2/setup.py
```

### Comparing `pixivSpiderCreatedByHanXu-0.0.1/LICENSE` & `pixivSpiderCreatedByHanXu-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pixivSpiderCreatedByHanXu-0.0.1/PKG-INFO` & `pixivSpiderCreatedByHanXu-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: pixivSpiderCreatedByHanXu
-Version: 0.0.1
+Version: 0.0.2
 Summary: This package can crawl the images at pixiv in two ways.
+Home-page: https://gitee.com/UnderTurrets/pixiv-spider
 Author: Han Xu
 Author-email: 736946693@qq.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -55,9 +56,9 @@
 type in the searchMode you want1
 Type in the date you want to search.Follow the format like this:2023042320221001
 type in the path where you want to reserve the images:rank20221001
 Type in the number of pages you want.Each page has almost 50 images:1
 ```
 # Download
 ```shell
-
+pip install pixivSpiderCreatedByHanXu
 ```
```

### Comparing `pixivSpiderCreatedByHanXu-0.0.1/README.md` & `pixivSpiderCreatedByHanXu-0.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -33,9 +33,9 @@
 type in the searchMode you want1
 Type in the date you want to search.Follow the format like this:2023042320221001
 type in the path where you want to reserve the images:rank20221001
 Type in the number of pages you want.Each page has almost 50 images:1
 ```
 # Download
 ```shell
-
+pip install pixivSpiderCreatedByHanXu
 ```
```

### Comparing `pixivSpiderCreatedByHanXu-0.0.1/pixivSpiderCreatedByHanXu/keywordSpider.py` & `pixivSpiderCreatedByHanXu-0.0.2/pixivSpiderCreatedByHanXu/keywordSpider.py`

 * *Files identical despite different names*

### Comparing `pixivSpiderCreatedByHanXu-0.0.1/pixivSpiderCreatedByHanXu/rankSpider.py` & `pixivSpiderCreatedByHanXu-0.0.2/pixivSpiderCreatedByHanXu/rankSpider.py`

 * *Files identical despite different names*

### Comparing `pixivSpiderCreatedByHanXu-0.0.1/pixivSpiderCreatedByHanXu.egg-info/PKG-INFO` & `pixivSpiderCreatedByHanXu-0.0.2/pixivSpiderCreatedByHanXu.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: pixivSpiderCreatedByHanXu
-Version: 0.0.1
+Version: 0.0.2
 Summary: This package can crawl the images at pixiv in two ways.
+Home-page: https://gitee.com/UnderTurrets/pixiv-spider
 Author: Han Xu
 Author-email: 736946693@qq.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -55,9 +56,9 @@
 type in the searchMode you want1
 Type in the date you want to search.Follow the format like this:2023042320221001
 type in the path where you want to reserve the images:rank20221001
 Type in the number of pages you want.Each page has almost 50 images:1
 ```
 # Download
 ```shell
-
+pip install pixivSpiderCreatedByHanXu
 ```
```

### Comparing `pixivSpiderCreatedByHanXu-0.0.1/setup.py` & `pixivSpiderCreatedByHanXu-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,25 +49,25 @@
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
     ],
 
     #如果上传时出现ERROR：The user '' isn't allowed to upload to project ''，换个名字，长一点无所谓，不能跟别人重复
     name="pixivSpiderCreatedByHanXu",
-    version="0.0.1",
+    version="0.0.2",
     author="Han Xu",
     author_email="736946693@qq.com",
     description="This package can crawl the images at pixiv in two ways.",
 
     long_description=long_description,
     #README.md文本的格式，如果希望使用markdown语言就需要下面这句话
     long_description_content_type="text/markdown",
 
     #源码地址，可以填入gitee上链接
-    # url="",
+    url="https://gitee.com/UnderTurrets/pixiv-spider",
 
     packages=find_packages(),
 
     # 安装过程中，需要安装的静态文件，如配置文件、service文件、图片等
     # data_files=[
     #     ("", ["conf/*.conf"]),
     #     ("/usr/lib/systemd/system/", ["bin/*.service"]),
```

