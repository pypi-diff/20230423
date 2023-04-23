# Comparing `tmp/nonebot_poe_chat-1.0.1.tar.gz` & `tmp/nonebot_poe_chat-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_poe_chat-1.0.1.tar", last modified: Sun Apr 23 07:35:24 2023, max compression
+gzip compressed data, was "nonebot_poe_chat-1.0.2.tar", last modified: Sun Apr 23 08:10:18 2023, max compression
```

## Comparing `nonebot_poe_chat-1.0.1.tar` & `nonebot_poe_chat-1.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 07:35:24.410920 nonebot_poe_chat-1.0.1/
--rw-rw-rw-   0        0        0    12533 2023-04-02 14:35:33.000000 nonebot_poe_chat-1.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     3095 2023-04-23 07:35:24.410920 nonebot_poe_chat-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2549 2023-04-22 14:39:54.000000 nonebot_poe_chat-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 07:35:24.403920 nonebot_poe_chat-1.0.1/nonebot_poe_chat/
--rw-rw-rw-   0        0        0    24950 2023-04-23 07:23:33.000000 nonebot_poe_chat-1.0.1/nonebot_poe_chat/__init__.py
--rw-rw-rw-   0        0        0     3609 2023-04-23 06:41:21.000000 nonebot_poe_chat-1.0.1/nonebot_poe_chat/config.py
--rw-rw-rw-   0        0        0     4736 2023-04-23 07:08:03.000000 nonebot_poe_chat-1.0.1/nonebot_poe_chat/poe_chat.py
--rw-rw-rw-   0        0        0     1965 2023-04-23 07:08:09.000000 nonebot_poe_chat-1.0.1/nonebot_poe_chat/poe_clear.py
--rw-rw-rw-   0        0        0     3409 2023-04-23 07:08:14.000000 nonebot_poe_chat-1.0.1/nonebot_poe_chat/poe_create.py
--rw-rw-rw-   0        0        0     2231 2023-04-23 03:10:23.000000 nonebot_poe_chat-1.0.1/nonebot_poe_chat/poe_func.py
--rw-rw-rw-   0        0        0     2396 2023-04-23 07:05:56.000000 nonebot_poe_chat-1.0.1/nonebot_poe_chat/poe_login.py
--rw-rw-rw-   0        0        0      490 2023-04-23 07:06:09.000000 nonebot_poe_chat-1.0.1/nonebot_poe_chat/temp.py
--rw-rw-rw-   0        0        0    10632 2023-04-23 05:59:48.000000 nonebot_poe_chat-1.0.1/nonebot_poe_chat/txt2img.py
-drwxrwxrwx   0        0        0        0 2023-04-23 07:35:24.409921 nonebot_poe_chat-1.0.1/nonebot_poe_chat.egg-info/
--rw-rw-rw-   0        0        0     3095 2023-04-23 07:35:24.000000 nonebot_poe_chat-1.0.1/nonebot_poe_chat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      487 2023-04-23 07:35:24.000000 nonebot_poe_chat-1.0.1/nonebot_poe_chat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 07:35:24.000000 nonebot_poe_chat-1.0.1/nonebot_poe_chat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      147 2023-04-23 07:35:24.000000 nonebot_poe_chat-1.0.1/nonebot_poe_chat.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-23 07:35:24.000000 nonebot_poe_chat-1.0.1/nonebot_poe_chat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 07:35:24.410920 nonebot_poe_chat-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1286 2023-04-23 07:34:45.000000 nonebot_poe_chat-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 08:10:18.958018 nonebot_poe_chat-1.0.2/
+-rw-rw-rw-   0        0        0    12533 2023-04-02 14:35:33.000000 nonebot_poe_chat-1.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     3095 2023-04-23 08:10:18.957013 nonebot_poe_chat-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2549 2023-04-22 14:39:54.000000 nonebot_poe_chat-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 08:10:18.950013 nonebot_poe_chat-1.0.2/nonebot_poe_chat/
+-rw-rw-rw-   0        0        0    24950 2023-04-23 07:23:33.000000 nonebot_poe_chat-1.0.2/nonebot_poe_chat/__init__.py
+-rw-rw-rw-   0        0        0     3609 2023-04-23 06:41:21.000000 nonebot_poe_chat-1.0.2/nonebot_poe_chat/config.py
+-rw-rw-rw-   0        0        0     4736 2023-04-23 07:08:03.000000 nonebot_poe_chat-1.0.2/nonebot_poe_chat/poe_chat.py
+-rw-rw-rw-   0        0        0     1965 2023-04-23 07:08:09.000000 nonebot_poe_chat-1.0.2/nonebot_poe_chat/poe_clear.py
+-rw-rw-rw-   0        0        0     3409 2023-04-23 07:08:14.000000 nonebot_poe_chat-1.0.2/nonebot_poe_chat/poe_create.py
+-rw-rw-rw-   0        0        0     2231 2023-04-23 03:10:23.000000 nonebot_poe_chat-1.0.2/nonebot_poe_chat/poe_func.py
+-rw-rw-rw-   0        0        0     2396 2023-04-23 07:05:56.000000 nonebot_poe_chat-1.0.2/nonebot_poe_chat/poe_login.py
+-rw-rw-rw-   0        0        0      490 2023-04-23 07:06:09.000000 nonebot_poe_chat-1.0.2/nonebot_poe_chat/temp.py
+-rw-rw-rw-   0        0        0    10632 2023-04-23 05:59:48.000000 nonebot_poe_chat-1.0.2/nonebot_poe_chat/txt2img.py
+drwxrwxrwx   0        0        0        0 2023-04-23 08:10:18.956013 nonebot_poe_chat-1.0.2/nonebot_poe_chat.egg-info/
+-rw-rw-rw-   0        0        0     3095 2023-04-23 08:10:18.000000 nonebot_poe_chat-1.0.2/nonebot_poe_chat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      487 2023-04-23 08:10:18.000000 nonebot_poe_chat-1.0.2/nonebot_poe_chat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 08:10:18.000000 nonebot_poe_chat-1.0.2/nonebot_poe_chat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      147 2023-04-23 08:10:18.000000 nonebot_poe_chat-1.0.2/nonebot_poe_chat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-04-23 08:10:18.000000 nonebot_poe_chat-1.0.2/nonebot_poe_chat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 08:10:18.958018 nonebot_poe_chat-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1340 2023-04-23 08:10:04.000000 nonebot_poe_chat-1.0.2/setup.py
```

### Comparing `nonebot_poe_chat-1.0.1/LICENSE.txt` & `nonebot_poe_chat-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nonebot_poe_chat-1.0.1/PKG-INFO` & `nonebot_poe_chat-1.0.2/nonebot_poe_chat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nonebot_poe_chat
-Version: 1.0.1
+Name: nonebot-poe-chat
+Version: 1.0.2
 Summary: nonebot_poe_chat
 Home-page: https://github.com/canxin121/nonebot_poe_chat
 Author: canxin
 Author-email: 1969730106@qq.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_poe_chat Version: 1.0.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-poe-chat Version: 1.0.2 Summary:
 nonebot_poe_chat Home-page: https://github.com/canxin121/nonebot_poe_chat
 Author: canxin Author-email: 1969730106@qq.com Classifier: Programming Language
 :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.8 Classifier: License :: OSI Approved ::
 GNU Affero General Public License v3 Classifier: Operating System :: OS
 Independent Description-Content-Type: text/markdown License-File: LICENSE.txt
                               [nonebot_poe_chat]
```

### Comparing `nonebot_poe_chat-1.0.1/README.md` & `nonebot_poe_chat-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_poe_chat-1.0.1/nonebot_poe_chat/__init__.py` & `nonebot_poe_chat-1.0.2/nonebot_poe_chat/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_poe_chat-1.0.1/nonebot_poe_chat/config.py` & `nonebot_poe_chat-1.0.2/nonebot_poe_chat/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_poe_chat-1.0.1/nonebot_poe_chat/poe_chat.py` & `nonebot_poe_chat-1.0.2/nonebot_poe_chat/poe_chat.py`

 * *Files identical despite different names*

### Comparing `nonebot_poe_chat-1.0.1/nonebot_poe_chat/poe_clear.py` & `nonebot_poe_chat-1.0.2/nonebot_poe_chat/poe_clear.py`

 * *Files identical despite different names*

### Comparing `nonebot_poe_chat-1.0.1/nonebot_poe_chat/poe_create.py` & `nonebot_poe_chat-1.0.2/nonebot_poe_chat/poe_create.py`

 * *Files identical despite different names*

### Comparing `nonebot_poe_chat-1.0.1/nonebot_poe_chat/poe_func.py` & `nonebot_poe_chat-1.0.2/nonebot_poe_chat/poe_func.py`

 * *Files identical despite different names*

### Comparing `nonebot_poe_chat-1.0.1/nonebot_poe_chat/poe_login.py` & `nonebot_poe_chat-1.0.2/nonebot_poe_chat/poe_login.py`

 * *Files identical despite different names*

### Comparing `nonebot_poe_chat-1.0.1/nonebot_poe_chat/txt2img.py` & `nonebot_poe_chat-1.0.2/nonebot_poe_chat/txt2img.py`

 * *Files identical despite different names*

### Comparing `nonebot_poe_chat-1.0.1/nonebot_poe_chat.egg-info/PKG-INFO` & `nonebot_poe_chat-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nonebot-poe-chat
-Version: 1.0.1
+Name: nonebot_poe_chat
+Version: 1.0.2
 Summary: nonebot_poe_chat
 Home-page: https://github.com/canxin121/nonebot_poe_chat
 Author: canxin
 Author-email: 1969730106@qq.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-poe-chat Version: 1.0.1 Summary:
+Metadata-Version: 2.1 Name: nonebot_poe_chat Version: 1.0.2 Summary:
 nonebot_poe_chat Home-page: https://github.com/canxin121/nonebot_poe_chat
 Author: canxin Author-email: 1969730106@qq.com Classifier: Programming Language
 :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.8 Classifier: License :: OSI Approved ::
 GNU Affero General Public License v3 Classifier: Operating System :: OS
 Independent Description-Content-Type: text/markdown License-File: LICENSE.txt
                               [nonebot_poe_chat]
```

### Comparing `nonebot_poe_chat-1.0.1/setup.py` & `nonebot_poe_chat-1.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="nonebot_poe_chat",  # 项目名称，保证它的唯一性，不要跟已存在的包名冲突即可
-    version="1.0.1",  # 程序版本
+    version="1.0.2",  # 程序版本
+    package_data={"nonebot_poe_chat":["TXT2IMG\*"]},
     author="canxin",  # 项目作者
     author_email="1969730106@qq.com",  # 作者邮件
     description="nonebot_poe_chat",  # 项目的一句话描述
     long_description=long_description,  # 加长版描述
     long_description_content_type="text/markdown",  # 描述使用Markdown
     url="https://github.com/canxin121/nonebot_poe_chat",  # 项目地址
     packages=setuptools.find_packages(),  # 无需修改
```

