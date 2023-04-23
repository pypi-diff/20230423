# Comparing `tmp/yyets-1.0.0.tar.gz` & `tmp/yyets-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yyets-1.0.0.tar", last modified: Tue Sep 21 11:36:33 2021, max compression
+gzip compressed data, was "yyets-1.0.1.tar", last modified: Sun Apr 23 20:09:48 2023, max compression
```

## Comparing `yyets-1.0.0.tar` & `yyets-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 benny      (501) staff       (20)        0 2021-09-21 11:36:33.070679 yyets-1.0.0/
--rw-r--r--   0 benny      (501) staff       (20)     1083 2021-01-21 15:19:29.000000 yyets-1.0.0/LICENSE
--rw-r--r--   0 benny      (501) staff       (20)     6839 2021-09-21 11:36:33.070446 yyets-1.0.0/PKG-INFO
--rw-r--r--   0 benny      (501) staff       (20)     5065 2021-09-21 11:26:35.000000 yyets-1.0.0/README.md
--rw-r--r--   0 benny      (501) staff       (20)       38 2021-09-21 11:36:33.070771 yyets-1.0.0/setup.cfg
--rw-r--r--   0 benny      (501) staff       (20)     3761 2021-09-21 11:35:57.000000 yyets-1.0.0/setup.py
-drwxr-xr-x   0 benny      (501) staff       (20)        0 2021-09-21 11:36:33.068713 yyets-1.0.0/yyets/
--rw-r--r--   0 benny      (501) staff       (20)     1536 2021-09-21 10:45:29.000000 yyets-1.0.0/yyets/__init__.py
-drwxr-xr-x   0 benny      (501) staff       (20)        0 2021-09-21 11:36:33.070023 yyets-1.0.0/yyets.egg-info/
--rw-r--r--   0 benny      (501) staff       (20)     6839 2021-09-21 11:36:32.000000 yyets-1.0.0/yyets.egg-info/PKG-INFO
--rw-r--r--   0 benny      (501) staff       (20)      188 2021-09-21 11:36:32.000000 yyets-1.0.0/yyets.egg-info/SOURCES.txt
--rw-r--r--   0 benny      (501) staff       (20)        1 2021-09-21 11:36:32.000000 yyets-1.0.0/yyets.egg-info/dependency_links.txt
--rw-r--r--   0 benny      (501) staff       (20)        9 2021-09-21 11:36:32.000000 yyets-1.0.0/yyets.egg-info/requires.txt
--rw-r--r--   0 benny      (501) staff       (20)        6 2021-09-21 11:36:32.000000 yyets-1.0.0/yyets.egg-info/top_level.txt
+drwxr-xr-x   0 benny      (501) staff       (20)        0 2023-04-23 20:09:48.852291 yyets-1.0.1/
+-rw-r--r--   0 benny      (501) staff       (20)     1083 2022-08-26 15:16:25.000000 yyets-1.0.1/LICENSE
+-rw-r--r--   0 benny      (501) staff       (20)     6392 2023-04-23 20:09:48.852172 yyets-1.0.1/PKG-INFO
+-rw-r--r--   0 benny      (501) staff       (20)     5924 2023-04-05 17:16:31.000000 yyets-1.0.1/README.md
+-rw-r--r--   0 benny      (501) staff       (20)       38 2023-04-23 20:09:48.852323 yyets-1.0.1/setup.cfg
+-rw-r--r--   0 benny      (501) staff       (20)     3741 2023-04-23 20:09:04.000000 yyets-1.0.1/setup.py
+drwxr-xr-x   0 benny      (501) staff       (20)        0 2023-04-23 20:09:48.851437 yyets-1.0.1/yyets/
+-rw-r--r--   0 benny      (501) staff       (20)     1502 2023-04-23 20:06:41.000000 yyets-1.0.1/yyets/__init__.py
+drwxr-xr-x   0 benny      (501) staff       (20)        0 2023-04-23 20:09:48.852014 yyets-1.0.1/yyets.egg-info/
+-rw-r--r--   0 benny      (501) staff       (20)     6392 2023-04-23 20:09:48.000000 yyets-1.0.1/yyets.egg-info/PKG-INFO
+-rw-r--r--   0 benny      (501) staff       (20)      188 2023-04-23 20:09:48.000000 yyets-1.0.1/yyets.egg-info/SOURCES.txt
+-rw-r--r--   0 benny      (501) staff       (20)        1 2023-04-23 20:09:48.000000 yyets-1.0.1/yyets.egg-info/dependency_links.txt
+-rw-r--r--   0 benny      (501) staff       (20)        9 2023-04-23 20:09:48.000000 yyets-1.0.1/yyets.egg-info/requires.txt
+-rw-r--r--   0 benny      (501) staff       (20)        6 2023-04-23 20:09:48.000000 yyets-1.0.1/yyets.egg-info/top_level.txt
```

### Comparing `yyets-1.0.0/LICENSE` & `yyets-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yyets-1.0.0/PKG-INFO` & `yyets-1.0.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,179 +1,188 @@
 Metadata-Version: 2.1
 Name: yyets
-Version: 1.0.0
+Version: 1.0.1
 Summary: https://yyets.dmesg.app/ wrapper
 Home-page: https://github.com/tgbot-collection/YYeTsBot
 Author: BennyThink
 Author-email: benny.think@gmail.com
 License: MIT
-Description: 
-        # YYeTsBot
-        
-        [![Build Status](https://travis-ci.com/tgbot-collection/YYeTsBot.svg?branch=master)](https://travis-ci.com/tgbot-collection/YYeTsBot)
-        
-        [![codecov](https://codecov.io/gh/tgbot-collection/YYeTsBot/branch/master/graph/badge.svg?token=ZL1GCIF95D)](https://codecov.io/gh/tgbot-collection/YYeTsBot)
-        
-        * 人人影视bot，[戳我使用](https://t.me/yyets_bot)
-        
-        * 人人影视分享站，[戳我使用](https://yyets.dmesg.app/)
-        
-        机器人和网站由我长期维护，如果遇到问题可以提issue。
-        
-        ![](assets/index.png)
-        
-        👉 前端[在这里](https://github.com/tgbot-collection/YYeTsFE) 👈
-        
-        # 使用说明
-        
-        直接发送想要看的剧集名称就可以了，可选分享网页或者链接（ed2k和磁力链接）。
-        
-        支持字幕侠、人人影视离线资源
-        
-        搜索资源时，会按照我预定的优先级（人人影视离线、字幕侠）进行搜索，当然也可以使用命令强制某个字幕组，如 `/yyets_offline 逃避可耻`
-        
-        **由于译名的不同，建议输入部分译名，然后从列表中进行选择。比如说想看权力的游戏第四季，那么直接搜索"权力的游戏"就可以了。**
-        
-        ## 命令
-        
-        ```
-        start - 开始使用
-        help - 帮助
-        credits - 致谢
-        ping - 运行状态
-        settings - 获取公告
-        zimuxia_online - 字幕侠在线数据  
-        newzmz_online - new字幕组在线数据 
-        yyets_offline - 人人影视离线数据
-        ```
-        
-        # 截图
-        
-        ## 常规搜索
-        
-        ![](assets/1.png)
-        
-        ## 资源分享站截图
-        
-        本网站永久免费，并且没有任何限制。
-        ![](assets/new_resource.png)
-        
-        ![](assets/2.png)
-        
-        支持收藏功能，会跨设备同步
-        ![](assets/like.png)
-        
-        ## 指定字幕组搜索
-        
-        目前只支持YYeTsOffline、ZimuxiaOnline和NewzmzOnline
-        
-        ![](assets/3.png)
-        
-        # 如何下载磁力和电驴资源？迅雷提示资源敏感
-        
-        ## 电驴资源
-        
-        请下载使用 [eMule](https://www.emule-project.net/home/perl/general.cgi?l=42) ，然后添加如下两个server list
-        
-        * [server.met](http://www.server-met.de/)
-        * [server list for emule](https://www.emule-security.org/serverlist/)
-        
-        ![](assets/emule.jpeg)
-        速度还可以哦
-        
-        ## 磁力
-        
-        使用百度网盘、115等离线，或使用utorrent等工具，记得更新下 [tracker list](https://raw.githubusercontent.com/ngosang/trackerslist/master/trackers_all.txt)
-        哦
-        
-        # 小白使用
-        
-        想要自己留一份资源，但是又不懂编程？ 没关系！目前提供两种方式，请根据自己情况选择
-        
-        ## 一键安装包
-        
-        这个版本是新的UI，拥有全部的最新功能。
-        [参考文档](https://github.com/tgbot-collection/YYeTsBot/blob/master/DEVELOPMENT.md#%E4%B8%80%E9%94%AE%E8%84%9A%E6%9C%AC)
-        
-        ## 一键运行包
-        
-        这个版本使用起来也很简单，无依赖。步骤如下
-        
-        1. 请到 [GitHub Release](https://github.com/tgbot-collection/YYeTsBot/releases) 根据自己平台下载一键运行包
-        2. 请到 [database download](https://yyets.dmesg.app/database) 下载SQLite数据库，然后解压缩
-        3. 把这两个文件放到同一个目录，结构如下 `yyets.sqlite yyetsweb`
-        4. windows：双击第一步下载的文件； macos/Linux，cd到你的目录, `chmod +x yyetsweb ; ./yyetsweb`
-        
-        打开浏览器 http://127.0.0.1:8888 就可以看到熟悉的搜索界面啦！
-        
-        # 开发
-        
-        ## 网站开发
-        
-        如何部署、参与开发、具体API接口，可以 [参考这个文档](DEVELOPMENT.md)
-        
-        ## Python Library
-        
-        也可以作为Python Library去调用
-        
-        `pip3 install yyets`
-        
-        ```
-        >>> from yyets import YYeTs
-        >>> yy=YYeTs("逃避")
-        [2021-09-21 19:22:32 __init__.py:54 I] Fetching 逃避可耻却有用...https://yyets.dmesg.app/api/resource?id=34812
-        [2021-09-21 19:22:33 __init__.py:54 I] Fetching 无法逃避...https://yyets.dmesg.app/api/resource?id=29540
-        [2021-09-21 19:22:35 __init__.py:54 I] Fetching 逃避者...https://yyets.dmesg.app/api/resource?id=37089
-        
-        >>> yy.result
-        [<yyets.Resource object at 0x10cc7b130>, <yyets.Resource object at 0x10ca0e880>, <yyets.Resource object at 0x10cc7b040>]
-        
-        >>> for y in yy.result:
-                print(y)
-            
-        逃避可耻却有用 - NIGERUHA HAJIDAGA YAKUNITATSU
-        无法逃避 - Inescapable
-        逃避者 - Shirkers
-        
-        >>> yy.result[0].cnname
-        '逃避可耻却有用'
-        
-        >>> yy.result[0].list
-        [{'season_num': '101', 'season_cn': '单剧', 'items': {'APP': [{'ite
-        ```
-        
-        # Credits
-        
-        * [人人影视](http://www.zmz2019.com/)
-        * [追新番](http://www.fanxinzhui.com/)
-        * [FIX字幕侠](https://www.zimuxia.cn/)
-        * [new字幕组](https://newzmz.com/)
-        
-        # 支持我
-        
-        觉得本项目对你有帮助？你可以通过以下方式表达你的感受：
-        
-        * 感谢字幕组
-        * 点一个star🌟和fork🍴
-        * 宣传，使用，提交问题报告
-        * 收藏[我的博客](https://dmesg.app/)
-        * [Telegram Channel](https://t.me/mikuri520)
-        * 捐助我，[给我买杯咖啡？](https://www.buymeacoffee.com/bennythink)
-        * 捐助我，[爱发电？](https://afdian.net/@BennyThink)
-        
-        # 感谢
-        
-        感谢所有[支持本项目](SPONSOR.md)的人！
-        
-        # License
-        
-        [MIT](LICENSE)
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+# YYeTsBot
+
+[![build docker image](https://github.com/tgbot-collection/YYeTsBot/actions/workflows/docker.yaml/badge.svg)](https://github.com/tgbot-collection/YYeTsBot/actions/workflows/docker.yaml)
+[![Docker Pulls](https://img.shields.io/docker/pulls/bennythink/yyetsbot)](https://hub.docker.com/r/bennythink/yyetsbot)
+
+* 人人影视bot，[戳我使用](https://t.me/yyets_bot)
+
+* 人人影视分享站，[戳我使用](https://yyets.dmesg.app/)
+
+机器人和网站由我长期维护，如果遇到问题可以提issue。
+
+![](assets/index.png)
+
+👉 前端[在这里](https://github.com/tgbot-collection/YYeTsFE) 👈
+
+# 使用说明
+
+直接发送想要看的剧集名称就可以了，可选分享网页或者链接（ed2k和磁力链接）。
+
+支持字幕侠、人人影视离线资源
+
+搜索资源时，会按照我预定的优先级（人人影视离线、字幕侠）进行搜索，当然也可以使用命令强制某个字幕组，如 `/yyets_offline 逃避可耻`
+
+**由于译名的不同，建议输入部分译名，然后从列表中进行选择。比如说想看权力的游戏第四季，那么直接搜索"权力的游戏"就可以了。**
+
+## 命令
+
+```
+start - 开始使用
+help - 帮助
+credits - 致谢
+ping - 运行状态
+settings - 获取公告
+zimuxia_online - 字幕侠在线数据  
+newzmz_online - new字幕组在线数据 
+yyets_offline - 人人影视离线数据
+```
+
+# 截图
+
+## 常规搜索
+
+![](assets/1.png)
+
+## 资源分享站截图
+
+本网站永久免费，并且没有任何限制。
+![](assets/new_resource.png)
+
+![](assets/2.png)
+
+支持收藏功能，会跨设备同步
+![](assets/like.png)
+
+## 指定字幕组搜索
+
+目前只支持YYeTsOffline、ZimuxiaOnline和NewzmzOnline
+
+![](assets/3.png)
+
+# 如何下载磁力和电驴资源？迅雷提示资源敏感
+
+## 电驴资源
+
+请下载使用 [eMule](https://www.emule-project.net/home/perl/general.cgi?l=42) ，然后添加如下两个server list
+
+* [server.met](http://www.server-met.de/)
+* [server list for emule](https://www.emule-security.org/serverlist/)
+
+![](assets/emule.jpeg)
+速度还可以哦
+
+## 磁力
+
+使用百度网盘、115等离线，或使用utorrent等工具，记得更新下 [tracker list](https://raw.githubusercontent.com/ngosang/trackerslist/master/trackers_all.txt)
+哦
+
+# 小白使用
+
+想要自己留一份资源，但是又不懂编程？ 没关系！目前提供两种方式，请根据自己情况选择
+“离线使用” 意味着可以断网使用，但是不会自动更新资源，需要手动更新数据库；“在线应用” 意味着需要有互联网才可以使用。
+
+## 离线  完整运行包
+
+这个版本是新的UI，拥有全部的最新功能。运行在你本地的电脑上，不依赖外界环境。
+[参考文档](https://github.com/tgbot-collection/YYeTsBot/blob/master/DEVELOPMENT.md#%E4%B8%80%E9%94%AE%E8%84%9A%E6%9C%AC)
+
+## 离线  一键运行包
+
+一键运行包。拥有比较新的UI，只不过只有最基础的搜索、查看资源的功能。使用方法步骤如下
+
+1. 请到 [GitHub Release](https://github.com/tgbot-collection/YYeTsBot/releases) ，找最新的 `YYeTsBot 离线一键运行包`
+2. windows：双击第一步下载的exe文件； macos/Linux，cd到你的目录, `chmod +x yyetsweb ; ./yyetsweb`
+3. 程序会自动下载数据库并启动。等到出现启动提示时， 打开浏览器 http://127.0.0.1:8888 就可以看到熟悉的搜索界面啦！
+
+## 在线 原生应用程序
+
+使用tauri封装的网页。内容等同于 `https://yyets.dmesg.app`，只不过是原生的App。使用方法如下
+
+1. 请到 [GitHub Release](https://github.com/tgbot-collection/YYeTsBot/releases) ，找最新的 `YYeTsBot App`
+2. windows下载msi，macos下载dmg或tar.gz，Linux下载AppImage或deb（Debian based）
+3. 安装后，打开App，就可以看到熟悉的搜索界面啦！
+
+# 开发
+
+## 网站开发
+
+如何部署、参与开发、具体API接口，可以 [参考这个文档](DEVELOPMENT.md)
+
+## Python Library
+
+也可以作为Python Library去调用
+
+`pip3 install yyets`
+
+```
+>>> from yyets import YYeTs
+>>> yy=YYeTs("逃避")
+[2021-09-21 19:22:32 __init__.py:54 I] Fetching 逃避可耻却有用...https://yyets.dmesg.app/api/resource?id=34812
+[2021-09-21 19:22:33 __init__.py:54 I] Fetching 无法逃避...https://yyets.dmesg.app/api/resource?id=29540
+[2021-09-21 19:22:35 __init__.py:54 I] Fetching 逃避者...https://yyets.dmesg.app/api/resource?id=37089
+
+>>> yy.result
+[<yyets.Resource object at 0x10cc7b130>, <yyets.Resource object at 0x10ca0e880>, <yyets.Resource object at 0x10cc7b040>]
+
+>>> for y in yy.result:
+        print(y)
+    
+逃避可耻却有用 - NIGERUHA HAJIDAGA YAKUNITATSU
+无法逃避 - Inescapable
+逃避者 - Shirkers
+
+>>> yy.result[0].cnname
+'逃避可耻却有用'
+
+>>> yy.result[0].list
+[{'season_num': '101', 'season_cn': '单剧', 'items': {'APP': [{'ite
+```
+
+# Credits
+
+* [人人影视](http://www.zmz2019.com/)
+* [追新番](http://www.fanxinzhui.com/)
+* [FIX字幕侠](https://www.zimuxia.cn/)
+* [new字幕组](https://newzmz.com/)
+
+# 支持我
+
+觉得本项目对你有帮助？你可以通过以下方式表达你的感受：
+
+* 感谢字幕组
+* 点一个star🌟和fork🍴
+* 宣传，使用，提交问题报告
+* 收藏[我的博客](https://dmesg.app/)
+* [Telegram Channel](https://t.me/mikuri520)
+* 捐助我，[给我买杯咖啡？](https://www.buymeacoffee.com/bennythink)
+* 捐助我，[爱发电？](https://afdian.net/@BennyThink)
+* 捐助我，[GitHub Sponsor](https://github.com/sponsors/BennyThink)
+* 捐助我，[Stripe](https://buy.stripe.com/dR67vU4p13Ox73a6oq)
+
+ <img src="./assets/CNY.png" width = 30%  alt="stripe"  />
+
+# 感谢
+
+感谢所有[支持本项目](SPONSOR.md)的人！
+
+# License
+
+[MIT](LICENSE)
```

### Comparing `yyets-1.0.0/setup.py` & `yyets-1.0.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,29 +5,27 @@
 #   $ pipenv install twine --dev
 
 import io
 import os
 import sys
 from shutil import rmtree
 
-from setuptools import find_packages, setup, Command
+from setuptools import Command, setup
 
 # Package meta-data.
-NAME = 'yyets'
-DESCRIPTION = 'https://yyets.dmesg.app/ wrapper'
-URL = 'https://github.com/tgbot-collection/YYeTsBot'
-EMAIL = 'benny.think@gmail.com'
-AUTHOR = 'BennyThink'
-REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '1.0.0'
+NAME = "yyets"
+DESCRIPTION = "https://yyets.dmesg.app/ wrapper"
+URL = "https://github.com/tgbot-collection/YYeTsBot"
+EMAIL = "benny.think@gmail.com"
+AUTHOR = "BennyThink"
+REQUIRES_PYTHON = ">=3.6.0"
+VERSION = "1.0.1"
 
 # What packages are required for this module to be executed?
-REQUIRED = [
-    "requests"
-]
+REQUIRED = ["requests"]
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
 
 # The rest you shouldn't have to touch too much :)
@@ -36,96 +34,95 @@
 # If you do change the License, remember to change the Trove Classifier for that!
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 # Import the README and use it as the long-description.
 # Note: this will only work if 'README.md' is present in your MANIFEST.in file!
 try:
-    with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
-        long_description = '\n' + f.read()
+    with io.open(os.path.join(here, "README.md"), encoding="utf-8") as f:
+        long_description = "\n" + f.read()
 except FileNotFoundError:
     long_description = DESCRIPTION
 
 # Load the package's __version__.py module as a dictionary.
 about = {}
 if not VERSION:
     project_slug = NAME.lower().replace("-", "_").replace(" ", "_")
-    with open(os.path.join(here, project_slug, '__version__.py')) as f:
+    with open(os.path.join(here, project_slug, "__version__.py")) as f:
         exec(f.read(), about)
 else:
-    about['__version__'] = VERSION
+    about["__version__"] = VERSION
 
 
 class UploadCommand(Command):
     """Support setup.py upload."""
 
-    description = 'Build and publish the package.'
+    description = "Build and publish the package."
     user_options = []
 
     @staticmethod
     def status(s):
         """Prints things in bold."""
-        print('\033[1m{0}\033[0m'.format(s))
+        print("\033[1m{0}\033[0m".format(s))
 
     def initialize_options(self):
         pass
 
     def finalize_options(self):
         pass
 
     def run(self):
         try:
-            self.status('Removing previous builds…')
-            rmtree(os.path.join(here, 'dist'))
+            self.status("Removing previous builds…")
+            rmtree(os.path.join(here, "dist"))
         except OSError:
             pass
 
-        self.status('Building Source and Wheel (universal) distribution…')
-        os.system('{0} setup.py sdist bdist_wheel --universal'.format(sys.executable))
+        self.status("Building Source and Wheel (universal) distribution…")
+        os.system("{0} setup.py sdist bdist_wheel --universal".format(sys.executable))
 
-        self.status('Uploading the package to PyPI via Twine…')
-        os.system('twine upload dist/*')
+        self.status("Uploading the package to PyPI via Twine…")
+        os.system("twine upload dist/*")
 
-        self.status('Pushing git tags…')
-        os.system('git tag v{0}'.format(about['__version__']))
-        os.system('git push --tags')
+        self.status("Pushing git tags…")
+        os.system("git tag v{0}".format(about["__version__"]))
+        os.system("git push --tags")
 
         sys.exit()
 
 
 # Where the magic happens:
 setup(
     name=NAME,
-    version=about['__version__'],
+    version=about["__version__"],
     description=DESCRIPTION,
     long_description=long_description,
-    long_description_content_type='text/markdown',
+    long_description_content_type="text/markdown",
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     url=URL,
     # packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
     # If your package is a single module, use this instead of 'packages':
-    packages=['yyets'],
-
+    packages=["yyets"],
     # entry_points={
     #     'console_scripts': ['mycli=mymodule:cli'],
     # },
     install_requires=REQUIRED,
     extras_require=EXTRAS,
     include_package_data=True,
-    license='MIT',
+    license="MIT",
     classifiers=[
         # Trove classifiers
         # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: Implementation :: CPython',
-        'Programming Language :: Python :: Implementation :: PyPy'
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: Implementation :: CPython",
+        "Programming Language :: Python :: Implementation :: PyPy",
     ],
     # $ setup.py publish support.
     cmdclass={
-        'upload': UploadCommand,
+        "upload": UploadCommand,
     },
-)
+)
```

### Comparing `yyets-1.0.0/yyets/__init__.py` & `yyets-1.0.1/yyets/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,21 +10,20 @@
 import requests
 import logging
 
 API = "https://yyets.dmesg.app/api/resource?"
 
 logging.basicConfig(
     level=logging.INFO,
-    format='[%(asctime)s %(filename)s:%(lineno)d %(levelname).1s] %(message)s',
-    datefmt="%Y-%m-%d %H:%M:%S"
+    format="[%(asctime)s %(filename)s:%(lineno)d %(levelname).1s] %(message)s",
+    datefmt="%Y-%m-%d %H:%M:%S",
 )
 
 
 class Resource:
-
     def __init__(self):
         self.enname = None
         self.cnname = None
 
     def __str__(self):
         return f"{self.cnname} - {self.enname}"
 
@@ -35,17 +34,16 @@
         self.keyword = keyword
         self.search_api = f"{API}keyword={self.keyword}"
         self.resource_api = f"{API}id=%s"
         self.search()
 
     def search(self):
         data = requests.get(self.search_api).json()
-        for item in data["data"]:
+        for info in data["data"]:
             r = Resource()
-            info = item["data"]["info"]
             setattr(r, "list", self.fetch(info))
             for k, v in info.items():
                 setattr(r, k, v)
             self.result.append(r)
 
     def fetch(self, info):
         rid = info["id"]
@@ -54,11 +52,11 @@
         logging.info("Fetching %s...%s", info["cnname"], url)
         return requests.get(url, headers=headers).json()["data"]["list"]
 
     def __str__(self):
         return f"{self.keyword} - {self.search_api}"
 
 
-if __name__ == '__main__':
-    ins = YYeTs("逃避")
+if __name__ == "__main__":
+    ins = YYeTs("逃避可耻")
     for i in ins.result:
         print(i)
```

### Comparing `yyets-1.0.0/yyets.egg-info/PKG-INFO` & `yyets-1.0.1/yyets.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,179 +1,188 @@
 Metadata-Version: 2.1
 Name: yyets
-Version: 1.0.0
+Version: 1.0.1
 Summary: https://yyets.dmesg.app/ wrapper
 Home-page: https://github.com/tgbot-collection/YYeTsBot
 Author: BennyThink
 Author-email: benny.think@gmail.com
 License: MIT
-Description: 
-        # YYeTsBot
-        
-        [![Build Status](https://travis-ci.com/tgbot-collection/YYeTsBot.svg?branch=master)](https://travis-ci.com/tgbot-collection/YYeTsBot)
-        
-        [![codecov](https://codecov.io/gh/tgbot-collection/YYeTsBot/branch/master/graph/badge.svg?token=ZL1GCIF95D)](https://codecov.io/gh/tgbot-collection/YYeTsBot)
-        
-        * 人人影视bot，[戳我使用](https://t.me/yyets_bot)
-        
-        * 人人影视分享站，[戳我使用](https://yyets.dmesg.app/)
-        
-        机器人和网站由我长期维护，如果遇到问题可以提issue。
-        
-        ![](assets/index.png)
-        
-        👉 前端[在这里](https://github.com/tgbot-collection/YYeTsFE) 👈
-        
-        # 使用说明
-        
-        直接发送想要看的剧集名称就可以了，可选分享网页或者链接（ed2k和磁力链接）。
-        
-        支持字幕侠、人人影视离线资源
-        
-        搜索资源时，会按照我预定的优先级（人人影视离线、字幕侠）进行搜索，当然也可以使用命令强制某个字幕组，如 `/yyets_offline 逃避可耻`
-        
-        **由于译名的不同，建议输入部分译名，然后从列表中进行选择。比如说想看权力的游戏第四季，那么直接搜索"权力的游戏"就可以了。**
-        
-        ## 命令
-        
-        ```
-        start - 开始使用
-        help - 帮助
-        credits - 致谢
-        ping - 运行状态
-        settings - 获取公告
-        zimuxia_online - 字幕侠在线数据  
-        newzmz_online - new字幕组在线数据 
-        yyets_offline - 人人影视离线数据
-        ```
-        
-        # 截图
-        
-        ## 常规搜索
-        
-        ![](assets/1.png)
-        
-        ## 资源分享站截图
-        
-        本网站永久免费，并且没有任何限制。
-        ![](assets/new_resource.png)
-        
-        ![](assets/2.png)
-        
-        支持收藏功能，会跨设备同步
-        ![](assets/like.png)
-        
-        ## 指定字幕组搜索
-        
-        目前只支持YYeTsOffline、ZimuxiaOnline和NewzmzOnline
-        
-        ![](assets/3.png)
-        
-        # 如何下载磁力和电驴资源？迅雷提示资源敏感
-        
-        ## 电驴资源
-        
-        请下载使用 [eMule](https://www.emule-project.net/home/perl/general.cgi?l=42) ，然后添加如下两个server list
-        
-        * [server.met](http://www.server-met.de/)
-        * [server list for emule](https://www.emule-security.org/serverlist/)
-        
-        ![](assets/emule.jpeg)
-        速度还可以哦
-        
-        ## 磁力
-        
-        使用百度网盘、115等离线，或使用utorrent等工具，记得更新下 [tracker list](https://raw.githubusercontent.com/ngosang/trackerslist/master/trackers_all.txt)
-        哦
-        
-        # 小白使用
-        
-        想要自己留一份资源，但是又不懂编程？ 没关系！目前提供两种方式，请根据自己情况选择
-        
-        ## 一键安装包
-        
-        这个版本是新的UI，拥有全部的最新功能。
-        [参考文档](https://github.com/tgbot-collection/YYeTsBot/blob/master/DEVELOPMENT.md#%E4%B8%80%E9%94%AE%E8%84%9A%E6%9C%AC)
-        
-        ## 一键运行包
-        
-        这个版本使用起来也很简单，无依赖。步骤如下
-        
-        1. 请到 [GitHub Release](https://github.com/tgbot-collection/YYeTsBot/releases) 根据自己平台下载一键运行包
-        2. 请到 [database download](https://yyets.dmesg.app/database) 下载SQLite数据库，然后解压缩
-        3. 把这两个文件放到同一个目录，结构如下 `yyets.sqlite yyetsweb`
-        4. windows：双击第一步下载的文件； macos/Linux，cd到你的目录, `chmod +x yyetsweb ; ./yyetsweb`
-        
-        打开浏览器 http://127.0.0.1:8888 就可以看到熟悉的搜索界面啦！
-        
-        # 开发
-        
-        ## 网站开发
-        
-        如何部署、参与开发、具体API接口，可以 [参考这个文档](DEVELOPMENT.md)
-        
-        ## Python Library
-        
-        也可以作为Python Library去调用
-        
-        `pip3 install yyets`
-        
-        ```
-        >>> from yyets import YYeTs
-        >>> yy=YYeTs("逃避")
-        [2021-09-21 19:22:32 __init__.py:54 I] Fetching 逃避可耻却有用...https://yyets.dmesg.app/api/resource?id=34812
-        [2021-09-21 19:22:33 __init__.py:54 I] Fetching 无法逃避...https://yyets.dmesg.app/api/resource?id=29540
-        [2021-09-21 19:22:35 __init__.py:54 I] Fetching 逃避者...https://yyets.dmesg.app/api/resource?id=37089
-        
-        >>> yy.result
-        [<yyets.Resource object at 0x10cc7b130>, <yyets.Resource object at 0x10ca0e880>, <yyets.Resource object at 0x10cc7b040>]
-        
-        >>> for y in yy.result:
-                print(y)
-            
-        逃避可耻却有用 - NIGERUHA HAJIDAGA YAKUNITATSU
-        无法逃避 - Inescapable
-        逃避者 - Shirkers
-        
-        >>> yy.result[0].cnname
-        '逃避可耻却有用'
-        
-        >>> yy.result[0].list
-        [{'season_num': '101', 'season_cn': '单剧', 'items': {'APP': [{'ite
-        ```
-        
-        # Credits
-        
-        * [人人影视](http://www.zmz2019.com/)
-        * [追新番](http://www.fanxinzhui.com/)
-        * [FIX字幕侠](https://www.zimuxia.cn/)
-        * [new字幕组](https://newzmz.com/)
-        
-        # 支持我
-        
-        觉得本项目对你有帮助？你可以通过以下方式表达你的感受：
-        
-        * 感谢字幕组
-        * 点一个star🌟和fork🍴
-        * 宣传，使用，提交问题报告
-        * 收藏[我的博客](https://dmesg.app/)
-        * [Telegram Channel](https://t.me/mikuri520)
-        * 捐助我，[给我买杯咖啡？](https://www.buymeacoffee.com/bennythink)
-        * 捐助我，[爱发电？](https://afdian.net/@BennyThink)
-        
-        # 感谢
-        
-        感谢所有[支持本项目](SPONSOR.md)的人！
-        
-        # License
-        
-        [MIT](LICENSE)
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+# YYeTsBot
+
+[![build docker image](https://github.com/tgbot-collection/YYeTsBot/actions/workflows/docker.yaml/badge.svg)](https://github.com/tgbot-collection/YYeTsBot/actions/workflows/docker.yaml)
+[![Docker Pulls](https://img.shields.io/docker/pulls/bennythink/yyetsbot)](https://hub.docker.com/r/bennythink/yyetsbot)
+
+* 人人影视bot，[戳我使用](https://t.me/yyets_bot)
+
+* 人人影视分享站，[戳我使用](https://yyets.dmesg.app/)
+
+机器人和网站由我长期维护，如果遇到问题可以提issue。
+
+![](assets/index.png)
+
+👉 前端[在这里](https://github.com/tgbot-collection/YYeTsFE) 👈
+
+# 使用说明
+
+直接发送想要看的剧集名称就可以了，可选分享网页或者链接（ed2k和磁力链接）。
+
+支持字幕侠、人人影视离线资源
+
+搜索资源时，会按照我预定的优先级（人人影视离线、字幕侠）进行搜索，当然也可以使用命令强制某个字幕组，如 `/yyets_offline 逃避可耻`
+
+**由于译名的不同，建议输入部分译名，然后从列表中进行选择。比如说想看权力的游戏第四季，那么直接搜索"权力的游戏"就可以了。**
+
+## 命令
+
+```
+start - 开始使用
+help - 帮助
+credits - 致谢
+ping - 运行状态
+settings - 获取公告
+zimuxia_online - 字幕侠在线数据  
+newzmz_online - new字幕组在线数据 
+yyets_offline - 人人影视离线数据
+```
+
+# 截图
+
+## 常规搜索
+
+![](assets/1.png)
+
+## 资源分享站截图
+
+本网站永久免费，并且没有任何限制。
+![](assets/new_resource.png)
+
+![](assets/2.png)
+
+支持收藏功能，会跨设备同步
+![](assets/like.png)
+
+## 指定字幕组搜索
+
+目前只支持YYeTsOffline、ZimuxiaOnline和NewzmzOnline
+
+![](assets/3.png)
+
+# 如何下载磁力和电驴资源？迅雷提示资源敏感
+
+## 电驴资源
+
+请下载使用 [eMule](https://www.emule-project.net/home/perl/general.cgi?l=42) ，然后添加如下两个server list
+
+* [server.met](http://www.server-met.de/)
+* [server list for emule](https://www.emule-security.org/serverlist/)
+
+![](assets/emule.jpeg)
+速度还可以哦
+
+## 磁力
+
+使用百度网盘、115等离线，或使用utorrent等工具，记得更新下 [tracker list](https://raw.githubusercontent.com/ngosang/trackerslist/master/trackers_all.txt)
+哦
+
+# 小白使用
+
+想要自己留一份资源，但是又不懂编程？ 没关系！目前提供两种方式，请根据自己情况选择
+“离线使用” 意味着可以断网使用，但是不会自动更新资源，需要手动更新数据库；“在线应用” 意味着需要有互联网才可以使用。
+
+## 离线  完整运行包
+
+这个版本是新的UI，拥有全部的最新功能。运行在你本地的电脑上，不依赖外界环境。
+[参考文档](https://github.com/tgbot-collection/YYeTsBot/blob/master/DEVELOPMENT.md#%E4%B8%80%E9%94%AE%E8%84%9A%E6%9C%AC)
+
+## 离线  一键运行包
+
+一键运行包。拥有比较新的UI，只不过只有最基础的搜索、查看资源的功能。使用方法步骤如下
+
+1. 请到 [GitHub Release](https://github.com/tgbot-collection/YYeTsBot/releases) ，找最新的 `YYeTsBot 离线一键运行包`
+2. windows：双击第一步下载的exe文件； macos/Linux，cd到你的目录, `chmod +x yyetsweb ; ./yyetsweb`
+3. 程序会自动下载数据库并启动。等到出现启动提示时， 打开浏览器 http://127.0.0.1:8888 就可以看到熟悉的搜索界面啦！
+
+## 在线 原生应用程序
+
+使用tauri封装的网页。内容等同于 `https://yyets.dmesg.app`，只不过是原生的App。使用方法如下
+
+1. 请到 [GitHub Release](https://github.com/tgbot-collection/YYeTsBot/releases) ，找最新的 `YYeTsBot App`
+2. windows下载msi，macos下载dmg或tar.gz，Linux下载AppImage或deb（Debian based）
+3. 安装后，打开App，就可以看到熟悉的搜索界面啦！
+
+# 开发
+
+## 网站开发
+
+如何部署、参与开发、具体API接口，可以 [参考这个文档](DEVELOPMENT.md)
+
+## Python Library
+
+也可以作为Python Library去调用
+
+`pip3 install yyets`
+
+```
+>>> from yyets import YYeTs
+>>> yy=YYeTs("逃避")
+[2021-09-21 19:22:32 __init__.py:54 I] Fetching 逃避可耻却有用...https://yyets.dmesg.app/api/resource?id=34812
+[2021-09-21 19:22:33 __init__.py:54 I] Fetching 无法逃避...https://yyets.dmesg.app/api/resource?id=29540
+[2021-09-21 19:22:35 __init__.py:54 I] Fetching 逃避者...https://yyets.dmesg.app/api/resource?id=37089
+
+>>> yy.result
+[<yyets.Resource object at 0x10cc7b130>, <yyets.Resource object at 0x10ca0e880>, <yyets.Resource object at 0x10cc7b040>]
+
+>>> for y in yy.result:
+        print(y)
+    
+逃避可耻却有用 - NIGERUHA HAJIDAGA YAKUNITATSU
+无法逃避 - Inescapable
+逃避者 - Shirkers
+
+>>> yy.result[0].cnname
+'逃避可耻却有用'
+
+>>> yy.result[0].list
+[{'season_num': '101', 'season_cn': '单剧', 'items': {'APP': [{'ite
+```
+
+# Credits
+
+* [人人影视](http://www.zmz2019.com/)
+* [追新番](http://www.fanxinzhui.com/)
+* [FIX字幕侠](https://www.zimuxia.cn/)
+* [new字幕组](https://newzmz.com/)
+
+# 支持我
+
+觉得本项目对你有帮助？你可以通过以下方式表达你的感受：
+
+* 感谢字幕组
+* 点一个star🌟和fork🍴
+* 宣传，使用，提交问题报告
+* 收藏[我的博客](https://dmesg.app/)
+* [Telegram Channel](https://t.me/mikuri520)
+* 捐助我，[给我买杯咖啡？](https://www.buymeacoffee.com/bennythink)
+* 捐助我，[爱发电？](https://afdian.net/@BennyThink)
+* 捐助我，[GitHub Sponsor](https://github.com/sponsors/BennyThink)
+* 捐助我，[Stripe](https://buy.stripe.com/dR67vU4p13Ox73a6oq)
+
+ <img src="./assets/CNY.png" width = 30%  alt="stripe"  />
+
+# 感谢
+
+感谢所有[支持本项目](SPONSOR.md)的人！
+
+# License
+
+[MIT](LICENSE)
```

