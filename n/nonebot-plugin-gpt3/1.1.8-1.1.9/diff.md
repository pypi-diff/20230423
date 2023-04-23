# Comparing `tmp/nonebot_plugin_gpt3-1.1.8.tar.gz` & `tmp/nonebot_plugin_gpt3-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_gpt3-1.1.8.tar", max compression
+gzip compressed data, was "nonebot_plugin_gpt3-1.1.9.tar", max compression
```

## Comparing `nonebot_plugin_gpt3-1.1.8.tar` & `nonebot_plugin_gpt3-1.1.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     5341 2023-03-07 06:11:13.008265 nonebot_plugin_gpt3-1.1.8/README.md
--rw-r--r--   0        0        0    12847 2023-03-07 06:07:48.891209 nonebot_plugin_gpt3-1.1.8/nonebot_plugin_gpt3/__init__.py
--rw-r--r--   0        0        0     1647 2023-03-07 06:07:48.891634 nonebot_plugin_gpt3-1.1.8/nonebot_plugin_gpt3/config.py
--rw-r--r--   0        0        0     1641 2023-03-10 04:46:45.483333 nonebot_plugin_gpt3-1.1.8/nonebot_plugin_gpt3/openai.py
--rw-r--r--   0        0        0      449 2023-03-10 04:46:45.475062 nonebot_plugin_gpt3-1.1.8/pyproject.toml
--rw-r--r--   0        0        0     6244 1970-01-01 00:00:00.000000 nonebot_plugin_gpt3-1.1.8/setup.py
--rw-r--r--   0        0        0     6017 1970-01-01 00:00:00.000000 nonebot_plugin_gpt3-1.1.8/PKG-INFO
+-rw-r--r--   0        0        0     5392 2023-04-23 03:55:56.456004 nonebot_plugin_gpt3-1.1.9/README.md
+-rw-r--r--   0        0        0    12714 2023-04-23 04:08:01.068564 nonebot_plugin_gpt3-1.1.9/nonebot_plugin_gpt3/__init__.py
+-rw-r--r--   0        0        0     1647 2023-03-07 06:07:48.891634 nonebot_plugin_gpt3-1.1.9/nonebot_plugin_gpt3/config.py
+-rw-r--r--   0        0        0     1717 2023-04-06 08:53:43.965762 nonebot_plugin_gpt3-1.1.9/nonebot_plugin_gpt3/openai.py
+-rw-r--r--   0        0        0      449 2023-04-23 04:11:51.139168 nonebot_plugin_gpt3-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0     6295 1970-01-01 00:00:00.000000 nonebot_plugin_gpt3-1.1.9/setup.py
+-rw-r--r--   0        0        0     6068 1970-01-01 00:00:00.000000 nonebot_plugin_gpt3-1.1.9/PKG-INFO
```

### Comparing `nonebot_plugin_gpt3-1.1.8/README.md` & `nonebot_plugin_gpt3-1.1.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -126,16 +126,16 @@
 之后是一些自定义配置，根据注释可以自行修改，如果需要请在对应的配置文件下进行配置。
 
 ```
 gpt3_command_prefix = "."                          # 基本会话中的指令前缀
 openai_api_key = "xxx"                             # API密钥
 
 # 默认人格
-gpt3_default_preset = "你叫鸡哥，是一个唱跳rap篮球的高手，并且每句话后都会带上厉不厉害你鸡哥!"
-gpt3_proxy = "http://127.0.0.1:6152"               # 代理地址
+gpt3_default_preset = "以下是与一个叫鸡哥的篮球高手的对话。你叫鸡哥，是一个唱跳rap篮球的高手，并且每句话后会带上厉不厉害你鸡哥!"
+gpt3_proxy = "http://127.0.0.1:7890"               # 代理地址
 gpt3_need_at = False                               # 是否需要@才触发命令
 gpt3_image_render = False                          # 是否渲染为图片
 gpt3_image_limit = 150                             # 长度超过多少才会渲染成图片
 gpt3_max_tokens = 1000                             # 回答内容最大长度
 gpt3_chat_count_per_day = 150                      # 普通用户每天聊天次数上限
 gpt3_model = 'gpt-3.5-turbo'                       # 语言模型
 ```
```

#### html2text {}

```diff
@@ -41,16 +41,16 @@
 Keyså³å¯ï¼æä»¥è¯·å¡«åAPIå¨æ¨çéç½®æä»¶ä¸­éç½®API KEYS ```
 openai_api_key = "xxx" # APIå¯é¥ ```
 æ­¤å¤å¯ä»¥éè¿ç¯å¢åééç½®ï¼ä¾å¦å¨Linuxå½ä»¤è¡ä¸­è¾å¥å¦ä¸å½ä»¤ä¹åï¼ç´æ¥å¯å¨å³å¯
 ``` export openai_api_key="xxx" ```
 ä¹åæ¯ä¸äºèªå®ä¹éç½®ï¼æ ¹æ®æ³¨éå¯ä»¥èªè¡ä¿®æ¹ï¼å¦æéè¦è¯·å¨å¯¹åºçéç½®æä»¶ä¸è¿è¡éç½®ã
 ``` gpt3_command_prefix = "." # åºæ¬ä¼è¯ä¸­çæä»¤åç¼ openai_api_key =
 "xxx" # APIå¯é¥ # é»è®¤äººæ ¼ gpt3_default_preset =
-"ä½ å«é¸¡å¥ï¼æ¯ä¸ä¸ªå±è·³rapç¯®ççé«æï¼å¹¶ä¸æ¯å¥è¯åé½ä¼å¸¦ä¸åä¸åå®³ä½ é¸¡å¥!"
-gpt3_proxy = "http://127.0.0.1:6152" # ä»£çå°å gpt3_need_at = False #
+"ä»¥ä¸æ¯ä¸ä¸ä¸ªå«é¸¡å¥çç¯®çé«æçå¯¹è¯ãä½ å«é¸¡å¥ï¼æ¯ä¸ä¸ªå±è·³rapç¯®ççé«æï¼å¹¶ä¸æ¯å¥è¯åä¼å¸¦ä¸åä¸åå®³ä½ é¸¡å¥!"
+gpt3_proxy = "http://127.0.0.1:7890" # ä»£çå°å gpt3_need_at = False #
 æ¯å¦éè¦@æè§¦åå½ä»¤ gpt3_image_render = False # æ¯å¦æ¸²æä¸ºå¾ç
 gpt3_image_limit = 150 # é¿åº¦è¶è¿å¤å°æä¼æ¸²ææå¾ç
 gpt3_max_tokens = 1000 # åç­åå®¹æå¤§é¿åº¦ gpt3_chat_count_per_day = 150
 # æ®éç¨æ·æ¯å¤©èå¤©æ¬¡æ°ä¸é gpt3_model = 'gpt-3.5-turbo' #
 è¯­è¨æ¨¡å ``` ## å¾çæ¸²æ
 å¦æéè¦å¼å¯å¾çæ¸²æï¼è¯·å¨éç½®æä»¶ä¸­ï¼éç½®`gpt3_image_render
 = True ` å¹¶å®è£`playwright`ï¼å¦æå·²ç»å®è£äº`playwright`åè¯·å¿½ç¥
```

### Comparing `nonebot_plugin_gpt3-1.1.8/nonebot_plugin_gpt3/__init__.py` & `nonebot_plugin_gpt3-1.1.9/nonebot_plugin_gpt3/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -372,16 +372,12 @@
 
     await chat_gpt3.finish('聊天结束...')
 
 # for test
 # @driver.on_startup
 # async def _():
 #     bot = Session(0)
-#     logger.debug(len(tokenizer.encode('你好, 我叫chris')))
-#     a = await bot.get_chat_response('你好, 我叫chris', True)
-#     print(a)
-#
-#     logger.debug(len(tokenizer.encode('写一个反转二叉树')))
+#     res = await bot.get_chat_response('你好, 我叫chris', True)
+#     print(res)
 #     a = await bot.get_chat_response('写一个反转二叉树', True)
-#     print(a)
-#
+#     print(res)
 #     exit(0)
```

### Comparing `nonebot_plugin_gpt3-1.1.8/nonebot_plugin_gpt3/config.py` & `nonebot_plugin_gpt3-1.1.9/nonebot_plugin_gpt3/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gpt3-1.1.8/nonebot_plugin_gpt3/openai.py` & `nonebot_plugin_gpt3-1.1.9/nonebot_plugin_gpt3/openai.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,14 +39,17 @@
             json={
                 "model": gpt3_model,
                 "messages": system + conversation,
                 "max_tokens": gpt3_max_tokens,
             },
         )
         response = response.json()
-        res: str = remove_punctuation(response['choices'][0]['message']['content'].strip())
-        conversation.append({"role": "assistant", "content": res})
-        return response, True
+        try:
+            res: str = remove_punctuation(response['choices'][0]['message']['content'].strip())
+            conversation.append({"role": "assistant", "content": res})
+            return response, True
+        except:
+            return response, False
     except httpx.ConnectTimeout as e:
         return f"发生HTTP超时错误: {e.request.url}", False
     except Exception as e:
         return f"发生未知错误: {type(e)} {e}", False
```

### Comparing `nonebot_plugin_gpt3-1.1.8/setup.py` & `nonebot_plugin_gpt3-1.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,17 @@
  'nonebot-adapter-onebot>=2.1.5,<3.0.0',
  'nonebot-plugin-htmlrender>=0.2.0.3,<0.3.0.0',
  'nonebot2>=2.0.0rc2,<3.0.0',
  'tiktoken==0.3.0']
 
 setup_kwargs = {
     'name': 'nonebot-plugin-gpt3',
-    'version': '1.1.8',
+    'version': '1.1.9',
     'description': '',
-    'long_description': '<div align="center">\n  <img src="https://s2.loli.net/2022/06/16/opBDE8Swad5rU3n.png" width="180" height="180" alt="NoneBotPluginLogo">\n  <br>\n  <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>\n</div>\n\n\n<div align="center">\n\n# Nonebot-plugin-gpt3\n## 3.3日更新: 支持gpt-3.5-turbo模型\n_✨ 基于OpenAI 官方API的对话插件 ✨_\n\n<p align="center">\n  <img src="https://img.shields.io/github/license/EtherLeaF/nonebot-plugin-colab-novelai" alt="license">\n  <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="Python">\n  <img src="https://img.shields.io/badge/nonebot-2.0.0r4+-red.svg" alt="NoneBot">\n  <a href="https://pypi.python.org/pypi/nonebot-plugin-gpt3">\n      <img src="https://img.shields.io/pypi/dm/nonebot-plugin-gpt3" alt="pypi download">\n  </a>\n</p>\n</div>\n\n# 功能\n\n- [x] 上下文功能\n- [x] 连续会话\n- [x] 人格设置\n- [x] 切换群聊/会话导出\n- [x] 回答图片渲染\n\n# 如何使用\n\n私聊中是直接发送消息，**群聊中是以回复的方式发送。**\n\n以下是功能列表\n\n|        功能        |             指令             |\n| :----------------: | :--------------------------: |\n| **基本的聊天对话** | 基本会话（默认【gpt3】触发） |\n|    **连续对话**    |      chat/聊天/开始聊天      |\n|    **结束聊天**    |      stop/结束/结束聊天      |\n|    **切换会话**    |    切换群聊/切换会话/切换    |\n|    重置会话记录    |        刷新/重置对话         |\n|     重置AI人格     |           重置人格           |\n|     设置AI人格     |           设置人格           |\n|    导出历史会话    |      导出会话/导出对话       |\n|   回答渲染为图片   |     图片渲染（默认关闭）     |\n\n\n## 基本会话\n\n对话前，加上**默认前缀**即可与GPT3对话。\n\n<img src="https://chrisyy-images.oss-cn-chengdu.aliyuncs.com/img/image-20230118155505182.png" width="40%" />\n\n## 连续会话\n\n输入**chat/聊天/开始聊天**即可不加前缀，连续的对话，输入**结束/结束聊天**，即可结束聊天\n\n<img src="https://chrisyy-images.oss-cn-chengdu.aliyuncs.com/img/image-20221217230058979.png" width="40%" />\n\n## 人格设置\n\n预设了**AI助手/猫娘/nsfw猫娘**三种人格，可以通过人格设置切换。内置的设定可以从[这里看到](https://github.com/chrisyy2003/lingyin-bot/blob/main/plugins/gpt3/nonebot_plugin_gpt3/__init__.py#L16-L18)。\n\n<img src="https://chrisyy-images.oss-cn-chengdu.aliyuncs.com/img/image-20221217231703614.png" width="40%" />\n\n同样也可以手动指定人格\n\n<img src="https://chrisyy-images.oss-cn-chengdu.aliyuncs.com/img/202303061532626.png" width="40%" />\n\n## 切换群聊\n\n命令切换+群号即可保留聊天信息并切换群聊。\n\n<img src="https://chrisyy-images.oss-cn-chengdu.aliyuncs.com/img/image-20230118161015957.png" width="40%"/>\n\n切换群聊到702280361\n\n<img src="https://chrisyy-images.oss-cn-chengdu.aliyuncs.com/img/image-20230118161509269.png" width="40%"/>\n\n\n\n\n## 图片渲染\n\n图片渲染可以在配置文件中选择配置是否需要渲染。\n\n<img src="https://chrisyy-images.oss-cn-chengdu.aliyuncs.com/img/image-20221217233729263.png" width="40%" />\n\n# 安装\n\n1.  使用 nb-cli\n\n```\nnb plugin install nonebot-plugin-gpt3\n```\n\n2.   通过包管理器安装，可以通过nb，pip，或者poetry等方式安装，以pip为例\n\n```\npip install nonebot-plugin-gpt3 -U\n```\n\n随后在`bot.py`中加上如下代码，加载插件\n\n```\nnonebot.load_plugin(\'nonebot_plugin_gpt3\')\n```\n\n# 配置\n\n对于官方OpenAI接口只需配置API Keys即可，所以请填写API在您的配置文件中配置API KEYS\n\n```\nopenai_api_key = "xxx"                             # API密钥\n```\n\n此外可以通过环境变量配置，例如在Linux命令行中输入如下命令之后，直接启动即可\n\n```\nexport openai_api_key="xxx"\n```\n\n之后是一些自定义配置，根据注释可以自行修改，如果需要请在对应的配置文件下进行配置。\n\n```\ngpt3_command_prefix = "."                          # 基本会话中的指令前缀\nopenai_api_key = "xxx"                             # API密钥\n\n# 默认人格\ngpt3_default_preset = "你叫鸡哥，是一个唱跳rap篮球的高手，并且每句话后都会带上厉不厉害你鸡哥!"\ngpt3_proxy = "http://127.0.0.1:6152"               # 代理地址\ngpt3_need_at = False                               # 是否需要@才触发命令\ngpt3_image_render = False                          # 是否渲染为图片\ngpt3_image_limit = 150                             # 长度超过多少才会渲染成图片\ngpt3_max_tokens = 1000                             # 回答内容最大长度\ngpt3_chat_count_per_day = 150                      # 普通用户每天聊天次数上限\ngpt3_model = \'gpt-3.5-turbo\'                       # 语言模型\n```\n\n## 图片渲染\n\n如果需要开启图片渲染，请在配置文件中，配置`gpt3_image_render = True  `\n\n并安装`playwright`，如果已经安装了`playwright`则请忽略\n\n```\npip3 install playwright && playwright install \n```\n\n>   启动后出现`PyTorch, TensorFlow`等提示问题，**忽略即可**\n>\n>   ![image-20230118105930615](https://chrisyy-images.oss-cn-chengdu.aliyuncs.com/img/image-20230118105930615.png)\n',
+    'long_description': '<div align="center">\n  <img src="https://s2.loli.net/2022/06/16/opBDE8Swad5rU3n.png" width="180" height="180" alt="NoneBotPluginLogo">\n  <br>\n  <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>\n</div>\n\n\n<div align="center">\n\n# Nonebot-plugin-gpt3\n## 3.3日更新: 支持gpt-3.5-turbo模型\n_✨ 基于OpenAI 官方API的对话插件 ✨_\n\n<p align="center">\n  <img src="https://img.shields.io/github/license/EtherLeaF/nonebot-plugin-colab-novelai" alt="license">\n  <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="Python">\n  <img src="https://img.shields.io/badge/nonebot-2.0.0r4+-red.svg" alt="NoneBot">\n  <a href="https://pypi.python.org/pypi/nonebot-plugin-gpt3">\n      <img src="https://img.shields.io/pypi/dm/nonebot-plugin-gpt3" alt="pypi download">\n  </a>\n</p>\n</div>\n\n# 功能\n\n- [x] 上下文功能\n- [x] 连续会话\n- [x] 人格设置\n- [x] 切换群聊/会话导出\n- [x] 回答图片渲染\n\n# 如何使用\n\n私聊中是直接发送消息，**群聊中是以回复的方式发送。**\n\n以下是功能列表\n\n|        功能        |             指令             |\n| :----------------: | :--------------------------: |\n| **基本的聊天对话** | 基本会话（默认【gpt3】触发） |\n|    **连续对话**    |      chat/聊天/开始聊天      |\n|    **结束聊天**    |      stop/结束/结束聊天      |\n|    **切换会话**    |    切换群聊/切换会话/切换    |\n|    重置会话记录    |        刷新/重置对话         |\n|     重置AI人格     |           重置人格           |\n|     设置AI人格     |           设置人格           |\n|    导出历史会话    |      导出会话/导出对话       |\n|   回答渲染为图片   |     图片渲染（默认关闭）     |\n\n\n## 基本会话\n\n对话前，加上**默认前缀**即可与GPT3对话。\n\n<img src="https://chrisyy-images.oss-cn-chengdu.aliyuncs.com/img/image-20230118155505182.png" width="40%" />\n\n## 连续会话\n\n输入**chat/聊天/开始聊天**即可不加前缀，连续的对话，输入**结束/结束聊天**，即可结束聊天\n\n<img src="https://chrisyy-images.oss-cn-chengdu.aliyuncs.com/img/image-20221217230058979.png" width="40%" />\n\n## 人格设置\n\n预设了**AI助手/猫娘/nsfw猫娘**三种人格，可以通过人格设置切换。内置的设定可以从[这里看到](https://github.com/chrisyy2003/lingyin-bot/blob/main/plugins/gpt3/nonebot_plugin_gpt3/__init__.py#L16-L18)。\n\n<img src="https://chrisyy-images.oss-cn-chengdu.aliyuncs.com/img/image-20221217231703614.png" width="40%" />\n\n同样也可以手动指定人格\n\n<img src="https://chrisyy-images.oss-cn-chengdu.aliyuncs.com/img/202303061532626.png" width="40%" />\n\n## 切换群聊\n\n命令切换+群号即可保留聊天信息并切换群聊。\n\n<img src="https://chrisyy-images.oss-cn-chengdu.aliyuncs.com/img/image-20230118161015957.png" width="40%"/>\n\n切换群聊到702280361\n\n<img src="https://chrisyy-images.oss-cn-chengdu.aliyuncs.com/img/image-20230118161509269.png" width="40%"/>\n\n\n\n\n## 图片渲染\n\n图片渲染可以在配置文件中选择配置是否需要渲染。\n\n<img src="https://chrisyy-images.oss-cn-chengdu.aliyuncs.com/img/image-20221217233729263.png" width="40%" />\n\n# 安装\n\n1.  使用 nb-cli\n\n```\nnb plugin install nonebot-plugin-gpt3\n```\n\n2.   通过包管理器安装，可以通过nb，pip，或者poetry等方式安装，以pip为例\n\n```\npip install nonebot-plugin-gpt3 -U\n```\n\n随后在`bot.py`中加上如下代码，加载插件\n\n```\nnonebot.load_plugin(\'nonebot_plugin_gpt3\')\n```\n\n# 配置\n\n对于官方OpenAI接口只需配置API Keys即可，所以请填写API在您的配置文件中配置API KEYS\n\n```\nopenai_api_key = "xxx"                             # API密钥\n```\n\n此外可以通过环境变量配置，例如在Linux命令行中输入如下命令之后，直接启动即可\n\n```\nexport openai_api_key="xxx"\n```\n\n之后是一些自定义配置，根据注释可以自行修改，如果需要请在对应的配置文件下进行配置。\n\n```\ngpt3_command_prefix = "."                          # 基本会话中的指令前缀\nopenai_api_key = "xxx"                             # API密钥\n\n# 默认人格\ngpt3_default_preset = "以下是与一个叫鸡哥的篮球高手的对话。你叫鸡哥，是一个唱跳rap篮球的高手，并且每句话后会带上厉不厉害你鸡哥!"\ngpt3_proxy = "http://127.0.0.1:7890"               # 代理地址\ngpt3_need_at = False                               # 是否需要@才触发命令\ngpt3_image_render = False                          # 是否渲染为图片\ngpt3_image_limit = 150                             # 长度超过多少才会渲染成图片\ngpt3_max_tokens = 1000                             # 回答内容最大长度\ngpt3_chat_count_per_day = 150                      # 普通用户每天聊天次数上限\ngpt3_model = \'gpt-3.5-turbo\'                       # 语言模型\n```\n\n## 图片渲染\n\n如果需要开启图片渲染，请在配置文件中，配置`gpt3_image_render = True  `\n\n并安装`playwright`，如果已经安装了`playwright`则请忽略\n\n```\npip3 install playwright && playwright install \n```\n\n>   启动后出现`PyTorch, TensorFlow`等提示问题，**忽略即可**\n>\n>   ![image-20230118105930615](https://chrisyy-images.oss-cn-chengdu.aliyuncs.com/img/image-20230118105930615.png)\n',
     'author': 'chrisyy',
     'author_email': '1017975501@qq.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['nonebot_plugin_gpt3'] package_data = \ {'': ['*']} install_requires = \
 ['httpx>=0.23.1,<0.24.0', 'nonebot-adapter-onebot>=2.1.5,<3.0.0', 'nonebot-
 plugin-htmlrender>=0.2.0.3,<0.3.0.0', 'nonebot2>=2.0.0rc2,<3.0.0',
 'tiktoken==0.3.0'] setup_kwargs = { 'name': 'nonebot-plugin-gpt3', 'version':
-'1.1.8', 'description': '', 'long_description': '
+'1.1.9', 'description': '', 'long_description': '
                            \n [NoneBotPluginLogo]\n
                                       \n
                               [NoneBotPluginText]
                                       \n
 \n\n\n
   \n\n# Nonebot-plugin-gpt3\n## 3.3æ¥æ´æ°: æ¯ægpt-3.5-turboæ¨¡å\n_â¨
                 åºäºOpenAI å®æ¹APIçå¯¹è¯æä»¶ â¨_\n\n
@@ -52,16 +52,16 @@
 éç½®\n\nå¯¹äºå®æ¹OpenAIæ¥å£åªééç½®API
 Keyså³å¯ï¼æä»¥è¯·å¡«åAPIå¨æ¨çéç½®æä»¶ä¸­éç½®API
 KEYS\n\n```\nopenai_api_key = "xxx" #
 APIå¯é¥\n```\n\næ­¤å¤å¯ä»¥éè¿ç¯å¢åééç½®ï¼ä¾å¦å¨Linuxå½ä»¤è¡ä¸­è¾å¥å¦ä¸å½ä»¤ä¹åï¼ç´æ¥å¯å¨å³å¯\n\n```\nexport
 openai_api_key="xxx"\n```\n\nä¹åæ¯ä¸äºèªå®ä¹éç½®ï¼æ ¹æ®æ³¨éå¯ä»¥èªè¡ä¿®æ¹ï¼å¦æéè¦è¯·å¨å¯¹åºçéç½®æä»¶ä¸è¿è¡éç½®ã\n\n```\ngpt3_command_prefix
 = "." # åºæ¬ä¼è¯ä¸­çæä»¤åç¼\nopenai_api_key = "xxx" # APIå¯é¥\n\n#
 é»è®¤äººæ ¼\ngpt3_default_preset =
-"ä½ å«é¸¡å¥ï¼æ¯ä¸ä¸ªå±è·³rapç¯®ççé«æï¼å¹¶ä¸æ¯å¥è¯åé½ä¼å¸¦ä¸åä¸åå®³ä½ é¸¡å¥!"\ngpt3_proxy
-= "http://127.0.0.1:6152" # ä»£çå°å\ngpt3_need_at = False #
+"ä»¥ä¸æ¯ä¸ä¸ä¸ªå«é¸¡å¥çç¯®çé«æçå¯¹è¯ãä½ å«é¸¡å¥ï¼æ¯ä¸ä¸ªå±è·³rapç¯®ççé«æï¼å¹¶ä¸æ¯å¥è¯åä¼å¸¦ä¸åä¸åå®³ä½ é¸¡å¥!"\ngpt3_proxy
+= "http://127.0.0.1:7890" # ä»£çå°å\ngpt3_need_at = False #
 æ¯å¦éè¦@æè§¦åå½ä»¤\ngpt3_image_render = False #
 æ¯å¦æ¸²æä¸ºå¾ç\ngpt3_image_limit = 150 #
 é¿åº¦è¶è¿å¤å°æä¼æ¸²ææå¾ç\ngpt3_max_tokens = 1000 #
 åç­åå®¹æå¤§é¿åº¦\ngpt3_chat_count_per_day = 150 #
 æ®éç¨æ·æ¯å¤©èå¤©æ¬¡æ°ä¸é\ngpt3_model = \'gpt-3.5-turbo\' #
 è¯­è¨æ¨¡å\n```\n\n##
 å¾çæ¸²æ\n\nå¦æéè¦å¼å¯å¾çæ¸²æï¼è¯·å¨éç½®æä»¶ä¸­ï¼éç½®`gpt3_image_render
```

### Comparing `nonebot_plugin_gpt3-1.1.8/PKG-INFO` & `nonebot_plugin_gpt3-1.1.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-gpt3
-Version: 1.1.8
+Version: 1.1.9
 Summary: 
 Author: chrisyy
 Author-email: 1017975501@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -145,16 +145,16 @@
 之后是一些自定义配置，根据注释可以自行修改，如果需要请在对应的配置文件下进行配置。
 
 ```
 gpt3_command_prefix = "."                          # 基本会话中的指令前缀
 openai_api_key = "xxx"                             # API密钥
 
 # 默认人格
-gpt3_default_preset = "你叫鸡哥，是一个唱跳rap篮球的高手，并且每句话后都会带上厉不厉害你鸡哥!"
-gpt3_proxy = "http://127.0.0.1:6152"               # 代理地址
+gpt3_default_preset = "以下是与一个叫鸡哥的篮球高手的对话。你叫鸡哥，是一个唱跳rap篮球的高手，并且每句话后会带上厉不厉害你鸡哥!"
+gpt3_proxy = "http://127.0.0.1:7890"               # 代理地址
 gpt3_need_at = False                               # 是否需要@才触发命令
 gpt3_image_render = False                          # 是否渲染为图片
 gpt3_image_limit = 150                             # 长度超过多少才会渲染成图片
 gpt3_max_tokens = 1000                             # 回答内容最大长度
 gpt3_chat_count_per_day = 150                      # 普通用户每天聊天次数上限
 gpt3_model = 'gpt-3.5-turbo'                       # 语言模型
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-gpt3 Version: 1.1.8 Summary: Author:
+Metadata-Version: 2.1 Name: nonebot-plugin-gpt3 Version: 1.1.9 Summary: Author:
 chrisyy Author-email: 1017975501@qq.com Requires-Python: >=3.8,<4.0 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Dist: httpx (>=0.23.1,<0.24.0) Requires-Dist: nonebot-
 adapter-onebot (>=2.1.5,<3.0.0) Requires-Dist: nonebot-plugin-htmlrender
 (>=0.2.0.3,<0.3.0.0) Requires-Dist: nonebot2 (>=2.0.0rc2,<3.0.0) Requires-Dist:
@@ -50,16 +50,16 @@
 Keyså³å¯ï¼æä»¥è¯·å¡«åAPIå¨æ¨çéç½®æä»¶ä¸­éç½®API KEYS ```
 openai_api_key = "xxx" # APIå¯é¥ ```
 æ­¤å¤å¯ä»¥éè¿ç¯å¢åééç½®ï¼ä¾å¦å¨Linuxå½ä»¤è¡ä¸­è¾å¥å¦ä¸å½ä»¤ä¹åï¼ç´æ¥å¯å¨å³å¯
 ``` export openai_api_key="xxx" ```
 ä¹åæ¯ä¸äºèªå®ä¹éç½®ï¼æ ¹æ®æ³¨éå¯ä»¥èªè¡ä¿®æ¹ï¼å¦æéè¦è¯·å¨å¯¹åºçéç½®æä»¶ä¸è¿è¡éç½®ã
 ``` gpt3_command_prefix = "." # åºæ¬ä¼è¯ä¸­çæä»¤åç¼ openai_api_key =
 "xxx" # APIå¯é¥ # é»è®¤äººæ ¼ gpt3_default_preset =
-"ä½ å«é¸¡å¥ï¼æ¯ä¸ä¸ªå±è·³rapç¯®ççé«æï¼å¹¶ä¸æ¯å¥è¯åé½ä¼å¸¦ä¸åä¸åå®³ä½ é¸¡å¥!"
-gpt3_proxy = "http://127.0.0.1:6152" # ä»£çå°å gpt3_need_at = False #
+"ä»¥ä¸æ¯ä¸ä¸ä¸ªå«é¸¡å¥çç¯®çé«æçå¯¹è¯ãä½ å«é¸¡å¥ï¼æ¯ä¸ä¸ªå±è·³rapç¯®ççé«æï¼å¹¶ä¸æ¯å¥è¯åä¼å¸¦ä¸åä¸åå®³ä½ é¸¡å¥!"
+gpt3_proxy = "http://127.0.0.1:7890" # ä»£çå°å gpt3_need_at = False #
 æ¯å¦éè¦@æè§¦åå½ä»¤ gpt3_image_render = False # æ¯å¦æ¸²æä¸ºå¾ç
 gpt3_image_limit = 150 # é¿åº¦è¶è¿å¤å°æä¼æ¸²ææå¾ç
 gpt3_max_tokens = 1000 # åç­åå®¹æå¤§é¿åº¦ gpt3_chat_count_per_day = 150
 # æ®éç¨æ·æ¯å¤©èå¤©æ¬¡æ°ä¸é gpt3_model = 'gpt-3.5-turbo' #
 è¯­è¨æ¨¡å ``` ## å¾çæ¸²æ
 å¦æéè¦å¼å¯å¾çæ¸²æï¼è¯·å¨éç½®æä»¶ä¸­ï¼éç½®`gpt3_image_render
 = True ` å¹¶å®è£`playwright`ï¼å¦æå·²ç»å®è£äº`playwright`åè¯·å¿½ç¥
```

