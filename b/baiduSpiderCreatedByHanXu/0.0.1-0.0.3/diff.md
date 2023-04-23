# Comparing `tmp/baiduspiderCreatedByHanXu-0.0.1.tar.gz` & `tmp/baiduSpiderCreatedByHanXu-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baiduspiderCreatedByHanXu-0.0.1.tar", last modified: Fri Apr 21 15:37:35 2023, max compression
+gzip compressed data, was "baiduSpiderCreatedByHanXu-0.0.3.tar", last modified: Sun Apr 23 14:04:08 2023, max compression
```

## Comparing `baiduspiderCreatedByHanXu-0.0.1.tar` & `baiduSpiderCreatedByHanXu-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 15:37:35.631669 baiduspiderCreatedByHanXu-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-04-21 15:37:35.617668 baiduspiderCreatedByHanXu-0.0.1/BaiduImageSpider/
--rw-rw-rw-   0        0        0        0 2023-04-21 12:42:30.000000 baiduspiderCreatedByHanXu-0.0.1/BaiduImageSpider/__init__.py
--rw-rw-rw-   0        0        0     3874 2023-04-21 15:33:25.000000 baiduspiderCreatedByHanXu-0.0.1/BaiduImageSpider/spider.py
--rw-rw-rw-   0        0        0     1090 2023-04-20 14:42:03.000000 baiduspiderCreatedByHanXu-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1005 2023-04-21 15:37:35.630682 baiduspiderCreatedByHanXu-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       64 2023-04-21 12:48:11.000000 baiduspiderCreatedByHanXu-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 15:37:35.627669 baiduspiderCreatedByHanXu-0.0.1/baiduspiderCreatedByHanXu.egg-info/
--rw-rw-rw-   0        0        0     1005 2023-04-21 15:37:35.000000 baiduspiderCreatedByHanXu-0.0.1/baiduspiderCreatedByHanXu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      326 2023-04-21 15:37:35.000000 baiduspiderCreatedByHanXu-0.0.1/baiduspiderCreatedByHanXu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 15:37:35.000000 baiduspiderCreatedByHanXu-0.0.1/baiduspiderCreatedByHanXu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-21 15:37:35.000000 baiduspiderCreatedByHanXu-0.0.1/baiduspiderCreatedByHanXu.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-21 15:37:35.000000 baiduspiderCreatedByHanXu-0.0.1/baiduspiderCreatedByHanXu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 15:37:35.631669 baiduspiderCreatedByHanXu-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     3212 2023-04-21 15:37:29.000000 baiduspiderCreatedByHanXu-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 14:04:08.038834 baiduSpiderCreatedByHanXu-0.0.3/
+-rw-rw-rw-   0        0        0     1090 2023-04-23 13:11:05.000000 baiduSpiderCreatedByHanXu-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1549 2023-04-23 14:04:08.038834 baiduSpiderCreatedByHanXu-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      551 2023-04-23 14:03:49.000000 baiduSpiderCreatedByHanXu-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 14:04:08.022431 baiduSpiderCreatedByHanXu-0.0.3/baiduSpiderCreatedByHanXu/
+-rw-rw-rw-   0        0        0        0 2023-04-23 13:11:05.000000 baiduSpiderCreatedByHanXu-0.0.3/baiduSpiderCreatedByHanXu/__init__.py
+-rw-rw-rw-   0        0        0     3795 2023-04-23 14:03:15.000000 baiduSpiderCreatedByHanXu-0.0.3/baiduSpiderCreatedByHanXu/spider.py
+drwxrwxrwx   0        0        0        0 2023-04-23 14:04:08.038834 baiduSpiderCreatedByHanXu-0.0.3/baiduSpiderCreatedByHanXu.egg-info/
+-rw-rw-rw-   0        0        0     1549 2023-04-23 14:04:07.000000 baiduSpiderCreatedByHanXu-0.0.3/baiduSpiderCreatedByHanXu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      344 2023-04-23 14:04:07.000000 baiduSpiderCreatedByHanXu-0.0.3/baiduSpiderCreatedByHanXu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 14:04:07.000000 baiduSpiderCreatedByHanXu-0.0.3/baiduSpiderCreatedByHanXu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-23 14:04:07.000000 baiduSpiderCreatedByHanXu-0.0.3/baiduSpiderCreatedByHanXu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-04-23 14:04:07.000000 baiduSpiderCreatedByHanXu-0.0.3/baiduSpiderCreatedByHanXu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 14:04:08.038834 baiduSpiderCreatedByHanXu-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     3280 2023-04-23 14:01:37.000000 baiduSpiderCreatedByHanXu-0.0.3/setup.py
```

### Comparing `baiduspiderCreatedByHanXu-0.0.1/BaiduImageSpider/spider.py` & `baiduSpiderCreatedByHanXu-0.0.3/baiduSpiderCreatedByHanXu/spider.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,12 +101,7 @@
         @:return
         """
         self.path=self.get_path()
         urls = self.get_urls()
         image_url = self.get_image_url(urls)
         self.get_image(image_url)
         return
-
-
-if __name__ == '__main__':
-    spider = Spider_baidu_image()
-    spider()
```

### Comparing `baiduspiderCreatedByHanXu-0.0.1/LICENSE` & `baiduSpiderCreatedByHanXu-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `baiduspiderCreatedByHanXu-0.0.1/setup.py` & `baiduSpiderCreatedByHanXu-0.0.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         #   5 - Production/Stable
         "Development Status :: 3 - Alpha",
 
         # 开发的目标用户
         "Intended Audience :: Developers",
 
         # 属于什么类型
-        "Topic :: Software Development :: Build Tools",
+        "Topic :: Software Development :: Libraries :: Python Modules",
 
         # 许可证信息
         "License :: OSI Approved :: MIT License",
 
         # 目标 Python 版本
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.3",
@@ -29,20 +29,21 @@
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
     ],
 
     #如果上传时出现ERROR：The user '' isn't allowed to upload to project ''，换个名字，长一点无所谓，不能跟别人重复
-    name="baiduspiderCreatedByHanXu",
-    version="0.0.1",
+    name="baiduSpiderCreatedByHanXu",
+    version="0.0.3",
     author="Han Xu",
     author_email="736946693@qq.com",
     description="This is a project used to get a large number of images in Baidu.",
     long_description=long_description,
+    long_description_content_type="text/markdown",
     url="https://gitee.com/UnderTurrets/baidu_image_spider",
     packages=find_packages(),
 
     # 安装过程中，需要安装的静态文件，如配置文件、service文件、图片等
     # data_files=[
     #     ("", ["conf/*.conf"]),
     #     ("/usr/lib/systemd/system/", ["bin/*.service"]),
```

