# Comparing `tmp/nonebot_plugin_bilifan-0.1.0.tar.gz` & `tmp/nonebot_plugin_bilifan-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilifan-0.1.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_bilifan-0.1.1.tar", max compression
```

## Comparing `nonebot_plugin_bilifan-0.1.0.tar` & `nonebot_plugin_bilifan-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35823 2023-04-13 11:46:28.243648 nonebot_plugin_bilifan-0.1.0/LICENSE
--rw-r--r--   0        0        0     5980 2023-04-16 08:59:13.519088 nonebot_plugin_bilifan-0.1.0/nonebot_plugin_bilifan/__init__.py
--rw-r--r--   0        0        0     4993 2023-04-13 14:32:49.994527 nonebot_plugin_bilifan-0.1.0/nonebot_plugin_bilifan/login/__init__.py
--rw-r--r--   0        0        0     4458 2023-04-16 08:49:13.391830 nonebot_plugin_bilifan-0.1.0/nonebot_plugin_bilifan/main.py
--rw-r--r--   0        0        0       54 2023-04-13 11:46:28.244641 nonebot_plugin_bilifan-0.1.0/nonebot_plugin_bilifan/src/__init__.py
--rw-r--r--   0        0        0    17462 2023-04-13 14:33:29.648335 nonebot_plugin_bilifan-0.1.0/nonebot_plugin_bilifan/src/api.py
--rw-r--r--   0        0        0    17061 2023-04-13 14:33:35.987716 nonebot_plugin_bilifan-0.1.0/nonebot_plugin_bilifan/src/user.py
--rw-r--r--   0        0        0     2217 2023-04-16 08:54:25.356364 nonebot_plugin_bilifan-0.1.0/nonebot_plugin_bilifan/users.yaml
--rw-r--r--   0        0        0     1099 2023-04-16 08:59:21.623283 nonebot_plugin_bilifan-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2043 2023-04-16 08:57:26.125573 nonebot_plugin_bilifan-0.1.0/README.md
--rw-r--r--   0        0        0     3017 1970-01-01 00:00:00.000000 nonebot_plugin_bilifan-0.1.0/setup.py
--rw-r--r--   0        0        0     3332 1970-01-01 00:00:00.000000 nonebot_plugin_bilifan-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35823 2023-04-13 11:46:28.243648 nonebot_plugin_bilifan-0.1.1/LICENSE
+-rw-r--r--   0        0        0     5992 2023-04-23 12:29:18.448941 nonebot_plugin_bilifan-0.1.1/nonebot_plugin_bilifan/__init__.py
+-rw-r--r--   0        0        0     4993 2023-04-13 14:32:49.994527 nonebot_plugin_bilifan-0.1.1/nonebot_plugin_bilifan/login/__init__.py
+-rw-r--r--   0        0        0     4458 2023-04-19 14:35:41.509222 nonebot_plugin_bilifan-0.1.1/nonebot_plugin_bilifan/main.py
+-rw-r--r--   0        0        0       54 2023-04-13 11:46:28.244641 nonebot_plugin_bilifan-0.1.1/nonebot_plugin_bilifan/src/__init__.py
+-rw-r--r--   0        0        0    17462 2023-04-13 14:33:29.648335 nonebot_plugin_bilifan-0.1.1/nonebot_plugin_bilifan/src/api.py
+-rw-r--r--   0        0        0    17061 2023-04-13 14:33:35.987716 nonebot_plugin_bilifan-0.1.1/nonebot_plugin_bilifan/src/user.py
+-rw-r--r--   0        0        0     2230 2023-04-19 14:34:33.086319 nonebot_plugin_bilifan-0.1.1/nonebot_plugin_bilifan/users.yaml
+-rw-r--r--   0        0        0     1099 2023-04-23 12:18:53.173460 nonebot_plugin_bilifan-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2043 2023-04-16 08:57:26.125573 nonebot_plugin_bilifan-0.1.1/README.md
+-rw-r--r--   0        0        0     3017 1970-01-01 00:00:00.000000 nonebot_plugin_bilifan-0.1.1/setup.py
+-rw-r--r--   0        0        0     3332 1970-01-01 00:00:00.000000 nonebot_plugin_bilifan-0.1.1/PKG-INFO
```

### Comparing `nonebot_plugin_bilifan-0.1.0/LICENSE` & `nonebot_plugin_bilifan-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilifan-0.1.0/nonebot_plugin_bilifan/__init__.py` & `nonebot_plugin_bilifan-0.1.1/nonebot_plugin_bilifan/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 logger.opt(colors=True).info(
     "已检测到软依赖<y>nonebot_plugin_apscheduler</y>, <g>开启定时任务功能</g>"
     if scheduler
     else "未检测到软依赖<y>nonebot_plugin_apscheduler</y>，<r>禁用定时任务功能</r>"
 )
 
 driver = get_driver()
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 __plugin_meta__ = PluginMetadata(
     name="bilifan",
     description='b站粉丝牌~',
     usage='自动刷b站粉丝牌',
     extra={
         "version": __version__,
         "author": "Agnes-Digital <Z735803792@163.com>",
@@ -87,15 +87,15 @@
             await matcher.send('开始执行~')
         else:
             logger.info(msg_path)
             await matcher.finish('你尚未登录，请输入【b站登录】')
         messageList = await main(msg_path.parent)
         message_str = '\n'.join(messageList)
         await matcher.finish(message_str)
-    except asyncio.exceptions.CancelledError :
+    except (FileNotFoundError,SystemExit):
         await matcher.finish('你尚未登录，请输入【b站登录】')
 
     
    
 def load_config():
     if not CONFIG_PATH.exists():
         CONFIG_PATH.touch()
@@ -155,8 +155,9 @@
 async def _():
     users = await read_yaml(Path().joinpath('data/bilifan'))
     cron = users.get('CRON', None)
     try:
         fields = cron.split(" ")
     except AttributeError:
         logger.error('定时格式不正确，不启用定时功能')
+        return
     scheduler.add_job(auto_cup, "cron", hour=fields[0], minute=fields[1],id="auto_cup")
```

### Comparing `nonebot_plugin_bilifan-0.1.0/nonebot_plugin_bilifan/login/__init__.py` & `nonebot_plugin_bilifan-0.1.1/nonebot_plugin_bilifan/login/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilifan-0.1.0/nonebot_plugin_bilifan/main.py` & `nonebot_plugin_bilifan-0.1.1/nonebot_plugin_bilifan/main.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilifan-0.1.0/nonebot_plugin_bilifan/src/api.py` & `nonebot_plugin_bilifan-0.1.1/nonebot_plugin_bilifan/src/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilifan-0.1.0/nonebot_plugin_bilifan/src/user.py` & `nonebot_plugin_bilifan-0.1.1/nonebot_plugin_bilifan/src/user.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilifan-0.1.0/nonebot_plugin_bilifan/users.yaml` & `nonebot_plugin_bilifan-0.1.1/nonebot_plugin_bilifan/users.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -6,27 +6,27 @@
       white_uid: 0
       banned_uid: 0
     # 注意对齐
     # 多用户以上格式添加
     # 井号后为注释 井号前后必须有空格！井号前后必须有空格！井号前后必须有空格！
     # 冒号后面也要有空格！冒号前面也要有空格！冒号前面也要有空格！
     # 英文冒号,英文逗号！英文逗号！英文逗号！
-CRON: 0 0 * * *
+CRON: 0 0 * * * # 0 0 * * *
 # 这里是 cron 表达式, 第一个参数是分钟, 第二个参数是小时
 # 例如每天凌晨0点0分执行一次为 0 0 * * *
 # 如果不填,则不使用内置定时器,填写正确后要保持该进程一直运行
 
 #########以下为自定义配置#########
 ASYNC: 1 # 异步执行,默认异步执行,设置为0则同步执行,开启异步后,将不支持设置点赞CD时间
 
 LIKE_CD: 2 # 点赞间隔时间,单位秒,默认2秒,仅为同步时生效,设置为0则不点赞
 
 DANMAKU_CD: 6 # 弹幕间隔时间,单位秒,默认6秒,设置为0则不发弹幕打卡,只能同步打卡
 
-WATCHINGLIVE: 2 # 每日观看直播时长，单位 min ，设置为0则关闭, 默认 65 分钟
+WATCHINGLIVE: 65 # 每日观看直播时长，单位 min ，设置为0则关闭, 默认 65 分钟
 
 WEARMEDAL: 0 # 是否弹幕打卡时自动带上当前房间的粉丝牌，避免房间有粉丝牌等级禁言，默认关闭，设置为1则开启
 
 SIGNINGROUP: 2 # 应援团签到CD时间,单位秒,默认2秒,设置为0则不签到
 # 说明：
 # 本项目中的异步执行指的是：同时点赞或者分享所有直播间，速度非常快，但缺点就是可能会被B站吞掉亲密度，所以建议粉丝牌较少的用户开启异步执行
 # 粉丝牌数大于30的用户建议使用同步，会更加稳定。缺点就是速度比较慢，但是可以设置点赞和分享的CD时间，避免被B站吞掉亲密度
```

### Comparing `nonebot_plugin_bilifan-0.1.0/pyproject.toml` & `nonebot_plugin_bilifan-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_bilifan"
-version = "0.1.0"
+version = "0.1.1"
 description = "刷bili粉丝牌子的机器人插件"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 repository = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 keywords = ["bilibili", "nonebot2", "plugin"]
```

### Comparing `nonebot_plugin_bilifan-0.1.0/README.md` & `nonebot_plugin_bilifan-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilifan-0.1.0/setup.py` & `nonebot_plugin_bilifan-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'nonebot_plugin_apscheduler>=0.2.0',
  'pillow>=9.3.0,<10.0.0',
  'pyyaml>=6.0,<7.0',
  'qrcode>=7.4.2,<8.0.0']
 
 setup_kwargs = {
     'name': 'nonebot-plugin-bilifan',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': '刷bili粉丝牌子的机器人插件',
     'long_description': '<div align="center">\n  <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">\n  <br>\n  <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>\n</div>\n\n<div align="center">\n\n# nonebot_plugin_bilifan\n_✨自动b站粉丝牌✨_\n\n<a href="https://github.com/Agnes4m/nonebot_plugin_bilifan/stargazers">\n        <img alt="GitHub stars" src="https://img.shields.io/github/stars/Agnes4m/nonebot_plugin_bilifan" alt="stars">\n</a>\n<a href="https://github.com/Agnes4m/nonebot_plugin_bilifan/issues">\n        <img alt="GitHub issues" src="https://img.shields.io/github/issues/Agnes4m/nonebot_plugin_bilifan" alt="issues">\n</a>\n<a href="https://jq.qq.com/?_wv=1027&k=HdjoCcAe">\n        <img src="https://img.shields.io/badge/QQ%E7%BE%A4-399365126-orange?style=flat-square" alt="QQ Chat Group">\n</a>\n<a href="https://pypi.python.org/pypi/nonebot_plugin_bilifan">\n        <img src="https://img.shields.io/pypi/v/nonebot_plugin_bilifan.svg" alt="pypi">\n</a>\n    <img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">\n    <img src="https://img.shields.io/badge/nonebot-2.0.0rc4-red.svg" alt="NoneBot">\n</div>\n\n\n## 配置\n\n启动一次插件，在bot路径下，"data/bilifan"文件夹内，按需求修改"users.yaml"文件\n\n## 指令\n\n - b站登录 - 返回b站二维码，扫码登录，绑定qq号\n - 开始刷牌子 - 开始执行命令\n - 自动刷牌子 - 添加或取消定时任务\n\n\n</details>\n\n## 🙈 其他\n\n+ 如果本插件对你有帮助，不要忘了点个Star~\n+ 本项目仅供学习使用，请勿用于商业用途\n+ [爱发电](https://afdian.net/a/agnes_digital)\n+ [GPL-3.0 License](https://github.com/Agnes4m/nonebot_plugin_bilifan/blob/main/LICENSE) ©[@Agnes4m](https://github.com/Agnes4m)\n        \n\n## 🌐 感谢\n\n- [新 B 站粉丝牌助手](https://github.com/XiaoMiku01/fansMedalHelper) - 源代码来自于他\n',
     'author': 'Agnes_Digital',
     'author_email': 'Z735803792@163.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Agnes4m/nonebot_plugin_l4d2_server',
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['nonebot_plugin_bilifan', 'nonebot_plugin_bilifan.login',
 'nonebot_plugin_bilifan.src'] package_data = \ {'': ['*']} install_requires = \
 ['aiohttp-socks>=0.8.0,<0.9.0', 'aiohttp>=3.8.3,<4.0.0', 'nonebot-adapter-
 onebot>=2.1.5', 'nonebot2>=2.0.0rc4,<3.0.0',
 'nonebot_plugin_apscheduler>=0.2.0', 'pillow>=9.3.0,<10.0.0',
 'pyyaml>=6.0,<7.0', 'qrcode>=7.4.2,<8.0.0'] setup_kwargs = { 'name': 'nonebot-
-plugin-bilifan', 'version': '0.1.0', 'description':
+plugin-bilifan', 'version': '0.1.1', 'description':
 'å·biliç²ä¸çå­çæºå¨äººæä»¶', 'long_description': '
                            \n [AgnesDigitalLogo]\n
                                       \n
                               [NoneBotPluginText]
                                       \n
 \n\n
     \n\n# nonebot_plugin_bilifan\n_â¨èªå¨bç«ç²ä¸çâ¨_\n\n\n_[GitHub
```

### Comparing `nonebot_plugin_bilifan-0.1.0/PKG-INFO` & `nonebot_plugin_bilifan-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilifan
-Version: 0.1.0
+Version: 0.1.1
 Summary: 刷bili粉丝牌子的机器人插件
 Home-page: https://github.com/Agnes4m/nonebot_plugin_l4d2_server
 License: GPLv3
 Keywords: bilibili,nonebot2,plugin
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.9,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bilifan Version: 0.1.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-bilifan Version: 0.1.1 Summary:
 å·biliç²ä¸çå­çæºå¨äººæä»¶ Home-page: https://github.com/Agnes4m/
 nonebot_plugin_l4d2_server License: GPLv3 Keywords: bilibili,nonebot2,plugin
 Author: Agnes_Digital Author-email: Z735803792@163.com Requires-Python:
 >=3.9,<4.0 Classifier: License :: OSI Approved :: GNU General Public License v3
 (GPLv3) Classifier: License :: Other/Proprietary License Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
```

