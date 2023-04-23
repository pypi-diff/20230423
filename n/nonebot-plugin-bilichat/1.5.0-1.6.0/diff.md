# Comparing `tmp/nonebot_plugin_bilichat-1.5.0.tar.gz` & `tmp/nonebot_plugin_bilichat-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilichat-1.5.0.tar", last modified: Fri Apr 21 16:46:38 2023, max compression
+gzip compressed data, was "nonebot_plugin_bilichat-1.6.0.tar", last modified: Sun Apr 23 05:57:40 2023, max compression
```

## Comparing `nonebot_plugin_bilichat-1.5.0.tar` & `nonebot_plugin_bilichat-1.6.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0    34523 2023-04-21 16:46:25.797468 nonebot_plugin_bilichat-1.5.0/LICENSE
--rw-r--r--   0        0        0    11167 2023-04-21 16:46:25.797468 nonebot_plugin_bilichat-1.5.0/README.md
--rw-r--r--   0        0        0     7289 2023-04-21 16:46:25.805468 nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/__init__.py
--rw-r--r--   0        0        0     4809 2023-04-21 16:46:25.805468 nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/config.py
--rw-r--r--   0        0        0      513 2023-04-21 16:46:25.805468 nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/lib/b23_extract.py
--rw-r--r--   0        0        0     6226 2023-04-21 16:46:25.805468 nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/lib/bcut_asr.py
--rw-r--r--   0        0        0     4806 2023-04-21 16:46:25.805468 nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/lib/bilibili_request.py
--rw-r--r--   0        0        0      927 2023-04-21 16:46:25.805468 nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/lib/column_resolve.py
--rw-r--r--   0        0        0     4657 2023-04-21 16:46:25.805468 nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/lib/content_resolve.py
--rw-r--r--   0        0        0     8900 2023-04-21 16:46:25.805468 nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/lib/draw_bili_image.py
--rw-r--r--   0        0        0     3800 2023-04-21 16:46:25.805468 nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/lib/fonts_provider.py
--rw-r--r--   0        0        0      399 2023-04-21 16:46:25.805468 nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/lib/store.py
--rw-r--r--   0        0        0     1868 2023-04-21 16:46:25.805468 nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/lib/strings.py
--rw-r--r--   0        0        0     4102 2023-04-21 16:46:25.805468 nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/lib/video_subtitle.py
--rw-r--r--   0        0        0     2854 2023-04-21 16:46:25.805468 nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/model/bcut_asr.py
--rw-r--r--   0        0        0      893 2023-04-21 16:46:25.805468 nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/model/cache.py
--rw-r--r--   0        0        0       93 2023-04-21 16:46:25.805468 nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/model/exception.py
--rw-r--r--   0        0        0      323 2023-04-21 16:46:25.805468 nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/model/openai.py
--rw-r--r--   0        0        0      261 2023-04-21 16:46:25.805468 nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/optional.py
--rw-r--r--   0        0        0   248896 2023-04-21 16:46:25.805468 nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/static/bing_apology.jpg
--rw-r--r--   0        0        0     1045 2023-04-21 16:46:25.805468 nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/summary/__init__.py
--rw-r--r--   0        0        0     5681 2023-04-21 16:46:25.805468 nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/summary/newbing_summarise.py
--rw-r--r--   0        0        0     4856 2023-04-21 16:46:25.809468 nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/summary/openai.py
--rw-r--r--   0        0        0     2359 2023-04-21 16:46:25.809468 nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/summary/openai_summarise.py
--rw-r--r--   0        0        0     1448 2023-04-21 16:46:25.809468 nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/summary/text_to_image.py
--rw-r--r--   0        0        0     1764 2023-04-21 16:46:25.809468 nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py
--rw-r--r--   0        0        0     1407 2023-04-21 16:46:38.373550 nonebot_plugin_bilichat-1.5.0/pyproject.toml
--rw-r--r--   0        0        0    12456 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-04-23 05:57:30.828880 nonebot_plugin_bilichat-1.6.0/LICENSE
+-rw-r--r--   0        0        0    11739 2023-04-23 05:57:30.828880 nonebot_plugin_bilichat-1.6.0/README.md
+-rw-r--r--   0        0        0     7893 2023-04-23 05:57:30.836880 nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/__init__.py
+-rw-r--r--   0        0        0     4809 2023-04-23 05:57:30.836880 nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/config.py
+-rw-r--r--   0        0        0      513 2023-04-23 05:57:30.836880 nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/lib/b23_extract.py
+-rw-r--r--   0        0        0     6226 2023-04-23 05:57:30.836880 nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/lib/bcut_asr.py
+-rw-r--r--   0        0        0     4806 2023-04-23 05:57:30.836880 nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/lib/bilibili_request.py
+-rw-r--r--   0        0        0      927 2023-04-23 05:57:30.836880 nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/lib/column_resolve.py
+-rw-r--r--   0        0        0     5262 2023-04-23 05:57:30.836880 nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/lib/content_resolve.py
+-rw-r--r--   0        0        0     8900 2023-04-23 05:57:30.836880 nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/lib/draw_bili_image.py
+-rw-r--r--   0        0        0     3800 2023-04-23 05:57:30.836880 nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/lib/fonts_provider.py
+-rw-r--r--   0        0        0      399 2023-04-23 05:57:30.836880 nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/lib/store.py
+-rw-r--r--   0        0        0     1868 2023-04-23 05:57:30.836880 nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/lib/strings.py
+-rw-r--r--   0        0        0     4102 2023-04-23 05:57:30.836880 nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/lib/video_subtitle.py
+-rw-r--r--   0        0        0      341 2023-04-23 05:57:30.836880 nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/model/arguments.py
+-rw-r--r--   0        0        0     2854 2023-04-23 05:57:30.836880 nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/model/bcut_asr.py
+-rw-r--r--   0        0        0     1127 2023-04-23 05:57:30.836880 nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/model/cache.py
+-rw-r--r--   0        0        0       93 2023-04-23 05:57:30.836880 nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/model/exception.py
+-rw-r--r--   0        0        0      323 2023-04-23 05:57:30.836880 nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/model/openai.py
+-rw-r--r--   0        0        0      261 2023-04-23 05:57:30.836880 nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/optional.py
+-rw-r--r--   0        0        0   248896 2023-04-23 05:57:30.840880 nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/static/bing_apology.jpg
+-rw-r--r--   0        0        0     1045 2023-04-23 05:57:30.840880 nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/summary/__init__.py
+-rw-r--r--   0        0        0     5681 2023-04-23 05:57:30.840880 nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/summary/newbing_summarise.py
+-rw-r--r--   0        0        0     4856 2023-04-23 05:57:30.840880 nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/summary/openai.py
+-rw-r--r--   0        0        0     2359 2023-04-23 05:57:30.840880 nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/summary/openai_summarise.py
+-rw-r--r--   0        0        0     1448 2023-04-23 05:57:30.840880 nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/summary/text_to_image.py
+-rw-r--r--   0        0        0     1764 2023-04-23 05:57:30.840880 nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py
+-rw-r--r--   0        0        0     1407 2023-04-23 05:57:40.672985 nonebot_plugin_bilichat-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0    13028 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-1.6.0/PKG-INFO
```

### Comparing `nonebot_plugin_bilichat-1.5.0/LICENSE` & `nonebot_plugin_bilichat-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.5.0/README.md` & `nonebot_plugin_bilichat-1.6.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -199,14 +199,30 @@
 4. 经测试，目前 `newbing` 至少能总结 12000 字符以上的文本，推测 token 上限应为 `gpt-4-32k-0314` 的 `32200` token，但过长的内容易造成输出内容包含额外内容或总结失败，因此也建议设置一个合理的 token 上限 ~~（反正不要钱，要啥自行车）~~
 5. 由于 `newbing` 限制较大，也不如 `openai` 听话，且需要联网查询资料，因此使用体验并不如 chatgpt ~~（反正不要钱，要啥自行车）~~
 
 ## 🎉 使用
 
 直接发送视频(专栏)链接即可
 
+### 参数表
+
+在发送视频时，可以额外添加以下类似 shell 指令的参数，进而对解析流程进行调整。例如
+
+```shell
+BV12v4y1E7NT --refresh
+BV12v4y1E7NT -r # 可以使用简写
+BV12v4y1E7NT -r --no-cache # 可以多个参数混用
+-r BV12v4y1E7NT -n # 虽然不建议，但确实可以把参数放前面
+```
+
+| 指令 | 简写 | 说明 |
+|:-----:|:----:|:----:|
+| --no-cache | -n | 本次总结禁用缓存(不会影响已存在的缓存文件) |
+| --refresh  | -r | 刷新此视频的词云和总结缓存(会覆盖已存在的缓存文件) |
+
 ### 指令表
 
 > 正在开发指令相关，请无视这里的模板
 > 指令设计方案征集中，如果有什么想要实现的功能可以在issue中提出
 
 | 指令 | 权限 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
```

#### html2text {}

```diff
@@ -90,16 +90,24 @@
 4. ç»æµè¯ï¼ç®å `newbing` è³å°è½æ»ç» 12000
 å­ç¬¦ä»¥ä¸çææ¬ï¼æ¨æµ token ä¸éåºä¸º `gpt-4-32k-0314` ç `32200`
 tokenï¼ä½è¿é¿çåå®¹æé æè¾åºåå®¹åå«é¢å¤åå®¹ææ»ç»å¤±è´¥ï¼å æ­¤ä¹å»ºè®®è®¾ç½®ä¸ä¸ªåçç
 token ä¸é ~~ï¼åæ­£ä¸è¦é±ï¼è¦å¥èªè¡è½¦ï¼~~ 5. ç±äº `newbing`
 éå¶è¾å¤§ï¼ä¹ä¸å¦ `openai`
 å¬è¯ï¼ä¸éè¦èç½æ¥è¯¢èµæï¼å æ­¤ä½¿ç¨ä½éªå¹¶ä¸å¦ chatgpt
 ~~ï¼åæ­£ä¸è¦é±ï¼è¦å¥èªè¡è½¦ï¼~~ ## ð ä½¿ç¨ ç´æ¥åéè§é¢
-(ä¸æ )é¾æ¥å³å¯ ### æä»¤è¡¨ >
-æ­£å¨å¼åæä»¤ç¸å³ï¼è¯·æ è§è¿éçæ¨¡æ¿ >
+(ä¸æ )é¾æ¥å³å¯ ### åæ°è¡¨
+å¨åéè§é¢æ¶ï¼å¯ä»¥é¢å¤æ·»å ä»¥ä¸ç±»ä¼¼ shell
+æä»¤çåæ°ï¼è¿èå¯¹è§£ææµç¨è¿è¡è°æ´ãä¾å¦ ```shell
+BV12v4y1E7NT --refresh BV12v4y1E7NT -r # å¯ä»¥ä½¿ç¨ç®å BV12v4y1E7NT -r --
+no-cache # å¯ä»¥å¤ä¸ªåæ°æ··ç¨ -r BV12v4y1E7NT -n #
+è½ç¶ä¸å»ºè®®ï¼ä½ç¡®å®å¯ä»¥æåæ°æ¾åé¢ ``` | æä»¤ | ç®å |
+è¯´æ | |:-----:|:----:|:----:| | --no-cache | -n | æ¬æ¬¡æ»ç»ç¦ç¨ç¼å­
+(ä¸ä¼å½±åå·²å­å¨çç¼å­æä»¶) | | --refresh | -r |
+å·æ°æ­¤è§é¢çè¯äºåæ»ç»ç¼å­(ä¼è¦çå·²å­å¨çç¼å­æä»¶) |
+### æä»¤è¡¨ > æ­£å¨å¼åæä»¤ç¸å³ï¼è¯·æ è§è¿éçæ¨¡æ¿ >
 æä»¤è®¾è®¡æ¹æ¡å¾éä¸­ï¼å¦ææä»ä¹æ³è¦å®ç°çåè½å¯ä»¥å¨issueä¸­æåº
 | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:----:|:----:|:
 ----:| | æä»¤1 | ä¸»äºº | å¦ | ç§è | æä»¤è¯´æ | | æä»¤2 | ç¾¤å |
 æ¯ | ç¾¤è | æä»¤è¯´æ | ## ð æè°¢ å¨æ­¤æè°¢ä»¥ä¸å¼åè
 (é¡¹ç®)å¯¹æ¬é¡¹ç®ååºçè´¡ç®ï¼ - [BibiGPT](https://github.com/JimmyLv/
 BibiGPT) é¡¹ç®çµææ¥æº - [bilibili-API-collect](https://github.com/
 SocialSisterYi/bilibili-API-collect) æå§æ¶éçåç§ BiliBili Api
```

### Comparing `nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/__init__.py` & `nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import re
-from typing import Union
+import shlex
+from itertools import chain
+from typing import Union, cast
 
+from nonebot.adapters import MessageSegment
 from nonebot.adapters.onebot.v11 import Bot as V11_Bot
 from nonebot.adapters.onebot.v11 import GroupMessageEvent as V11_GME
 from nonebot.adapters.onebot.v11 import Message as V11_Message
 from nonebot.adapters.onebot.v11 import MessageEvent as V11_ME
 from nonebot.adapters.onebot.v11 import MessageSegment as V11_MS
 from nonebot.adapters.onebot.v11 import PrivateMessageEvent as V11_PME
 from nonebot.adapters.onebot.v12 import Bot as V12_Bot
@@ -13,21 +16,23 @@
 from nonebot.adapters.onebot.v12 import MessageEvent as V12_ME
 from nonebot.adapters.onebot.v12 import MessageSegment as V12_MS
 from nonebot.adapters.onebot.v12 import PrivateMessageEvent as V12_PME
 from nonebot.consts import REGEX_GROUP, REGEX_STR
 from nonebot.exception import FinishedException
 from nonebot.log import logger
 from nonebot.matcher import Matcher
+from nonebot.params import Depends
 from nonebot.plugin import PluginMetadata, on_regex
 from nonebot.rule import Rule
 from nonebot.typing import T_State
 
 from .config import __version__, plugin_config
 from .lib.b23_extract import b23_extract
 from .lib.content_resolve import get_video_basic, get_video_cache
+from .model.arguments import Options, parser
 from .model.exception import AbortError
 from .optional import capture_exception  # type: ignore
 
 if plugin_config.bilichat_openai_token or plugin_config.bilichat_newbing_cookie:
     ENABLE_SUMMARY = True
     from .summary import summarization
 else:
@@ -68,39 +73,51 @@
 bili = on_regex(
     r"av(\d{1,15})|BV(1[A-Za-z0-9]{2}4.1.7[A-Za-z0-9]{2})",
     block=plugin_config.bilichat_block,
     priority=1,
     rule=Rule(_bili_check),
 )
 
-
-@bili.handle()
-async def get_bili_number_re(state: T_State):
-    state["bili_number"] = state[REGEX_STR]
-
-
 b23 = on_regex(
     r"b23.(tv|wtf)[\\/]+(\w+)",
     block=plugin_config.bilichat_block,
     priority=1,
     rule=Rule(_bili_check),
 )
 
 
+def get_args(event: Union[V11_ME, V12_ME]):
+    return parser.parse_known_args(
+        list(
+            chain.from_iterable(
+                shlex.split(str(seg)) if cast(MessageSegment, seg).is_text() else (seg,) for seg in event.get_message()
+            )
+        ),  # type: ignore
+        namespace=Options(),
+    )[0]
+
+
+@bili.handle()
+async def get_bili_number_re(state: T_State):
+    state["bili_number"] = state[REGEX_STR]
+
+
 @b23.handle()
 async def get_bili_number_b23(state: T_State):
     if matched := re.search(
         r"av(\d{1,15})|BV(1[A-Za-z0-9]{2}4.1.7[A-Za-z0-9]{2})", await b23_extract(state[REGEX_GROUP])  # type: ignore
     ):
         state["bili_number"] = matched.group()
 
 
 @bili.handle()
 @b23.handle()
-async def video_info_v11(bot: V11_Bot, event: V11_ME, state: T_State, matcher: Matcher):
+async def video_info_v11(
+    bot: V11_Bot, event: V11_ME, state: T_State, matcher: Matcher, options: Options = Depends(get_args)
+):
     # sourcery skip: raise-from-previous-error
     # basic info
     msg, img, info = await get_video_basic(state["bili_number"], state["_uid_"])
     if not msg or not info:
         await matcher.finish()
     reply = V11_MS.reply(event.message_id)
     if not img:
@@ -113,15 +130,15 @@
 
     # furtuer fuctions
     if not ENABLE_SUMMARY and not plugin_config.bilichat_word_cloud:
         raise FinishedException
 
     # get video cache
     try:
-        cache = await get_video_cache(info)
+        cache = await get_video_cache(info, options)
     except AbortError as e:
         logger.exception(e)
         await matcher.finish(f"{reply}视频字幕获取失败: {str(e)}")
     except Exception as e:
         capture_exception()
         logger.exception(e)
         await matcher.finish(f"{reply}未知错误: {e}")
@@ -150,15 +167,17 @@
 async def get_image_v12(bot: V12_Bot, bili_number: str, suffix: str, data):
     fileid = await bot.upload_file(type="data", name=f"{bili_number}_{suffix}.jpg", data=data)
     return V12_MS.image(file_id=fileid["file_id"])
 
 
 @bili.handle()
 @b23.handle()
-async def video_info_v12(bot: V12_Bot, event: V12_ME, state: T_State, matcher: Matcher):
+async def video_info_v12(
+    bot: V12_Bot, event: V12_ME, state: T_State, matcher: Matcher, options: Options = Depends(get_args)
+):
     # basic info
     msg, img, info = await get_video_basic(state["bili_number"], state["_uid_"])
     if not msg:
         await matcher.finish()
     reply = V12_MS.reply(message_id=event.message_id, user_id=event.get_user_id())
     if not img or not info:
         await matcher.finish(reply + msg)
@@ -169,15 +188,15 @@
             reply = V12_MS.reply(msgid)
 
     # furtuer fuctions
     if not ENABLE_SUMMARY and not plugin_config.bilichat_word_cloud:
         raise FinishedException
 
     try:
-        cache = await get_video_cache(info)
+        cache = await get_video_cache(info, options)
     except AbortError as e:
         logger.exception(e)
         await matcher.finish(f"{reply}视频字幕获取失败: {str(e)}")
     except Exception as e:
         capture_exception()
         logger.exception(e)
         await matcher.finish(f"{reply}未知错误: {str(e)}")
```

### Comparing `nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/config.py` & `nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/lib/b23_extract.py` & `nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/lib/b23_extract.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/lib/bcut_asr.py` & `nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/lib/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/lib/bilibili_request.py` & `nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/lib/bilibili_request.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/lib/column_resolve.py` & `nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/lib/column_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/lib/content_resolve.py` & `nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/lib/content_resolve.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from bilireq.exceptions import GrpcError
 from grpc.aio import AioRpcError
 from httpx._exceptions import TimeoutException
 from nonebot.log import logger
 
 from ..config import plugin_config
+from ..model.arguments import Options
 from ..model.cache import Cache, Episode
 from ..optional import capture_exception  # type: ignore
 from .bilibili_request import get_b23_url, grpc_get_view_info
 from .draw_bili_image import binfo_image_create
 from .video_subtitle import get_subtitle
 
 cd: Dict[str, int] = {}
@@ -90,39 +91,54 @@
         return (f"{bili_number} 视频信息生成超时，请稍后再试。", None, None)
     except Exception as e:  # noqa
         capture_exception()
         logger.exception(f"Video parsing API call error: {e}")
         return (f"视频解析 API 调用出错：{e}", None, None)
 
 
-async def get_video_cache(info: Dict):
-    cache = Cache.get(f'av{info["aid"]}')
-    # cache file not exists
-    if not cache:
-        logger.debug(f'cache of av{info["aid"]} not exists, create cache')
-        cache = Cache.create(
+async def get_video_cache(info: Dict, options: Options):
+    async def create_cache():
+        return Cache.create(
             id=f'av{info["aid"]}',
             title=info["title"],
             episodes={
                 str(info["cid"]): Episode(
                     title=None,
                     content=await get_subtitle(int(info["aid"]), int(info["cid"])),
                     jieba=None,
                     openai=None,
                     newbing=None,
                 )
             },
+            temp=options.no_cache,
         )
+
+    if options.no_cache:
+        logger.debug(f'parameter --no-cache of av{info["aid"]} detected, using temporary cache')
+        return await create_cache()
+
+    cache = Cache.get(f'av{info["aid"]}')
+    # cache file not exists
+    if not cache:
+        logger.debug(f'cache of av{info["aid"]} not exists, create cache')
+        return await create_cache()
     # cache file exists but cid not found
     elif str(info["cid"]) not in cache.episodes.keys():
         logger.debug(f'cache of av{info["aid"]} exists, but cid{info["cid"]} not found, appending cache')
         cache.episodes[str(info["cid"])] = Episode(
             title=None,
             content=await get_subtitle(int(info["aid"]), int(info["cid"])),
             jieba=None,
             openai=None,
             newbing=None,
         )
-    # cache file exists
+    # all exists but need refresh
+    elif options.refresh:
+        logger.debug(f'parameter --refresh of av{info["aid"]} detected, remove summary cache')
+        episode = cache.episodes[str(info["cid"])]
+        episode.jieba = None
+        episode.openai = None
+        episode.newbing = None
+    # all exists
     else:
         logger.debug(f'cache of av{info["aid"]} exists, use cache')
     return cache
```

### Comparing `nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/lib/draw_bili_image.py` & `nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/lib/draw_bili_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/lib/fonts_provider.py` & `nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/lib/fonts_provider.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/lib/strings.py` & `nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/lib/strings.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/lib/video_subtitle.py` & `nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/lib/video_subtitle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/model/bcut_asr.py` & `nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/model/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/model/cache.py` & `nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/model/cache.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,23 +11,34 @@
     newbing: Optional[str]
 
 
 class Cache(BaseModel):
     id: str
     title: str
     episodes: Dict[str, Episode]
+    temp: bool = False
 
     @classmethod
-    def create(cls, id: str, title: str, episodes: Dict[str, Episode]):
-        cache = cls(id=id, title=title, episodes=episodes)
+    def create(cls, id: str, title: str, episodes: Dict[str, Episode], temp: bool = False):
+        cache = cls(id=id, title=title, episodes=episodes, temp=temp)
         cache.save()
         return cache
 
     @classmethod
     def get(cls, id: Union[str, int]):
         f = cache_dir.joinpath(f"{id}.json")
         return cls.parse_file(f, encoding="utf-8") if f.exists() else None
 
     def save(self):
+        if self.temp:
+            return
         cache_dir.touch(0o755)
         f = cache_dir.joinpath(f"{self.id}.json")
-        f.write_text(self.json(ensure_ascii=False), encoding="utf-8")
+        f.write_text(
+            self.json(
+                ensure_ascii=False,
+                exclude={
+                    "temp",
+                },
+            ),
+            encoding="utf-8",
+        )
```

### Comparing `nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/static/bing_apology.jpg` & `nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/static/bing_apology.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/summary/__init__.py` & `nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/summary/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/summary/newbing_summarise.py` & `nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/summary/newbing_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/summary/openai.py` & `nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/summary/openai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/summary/openai_summarise.py` & `nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/summary/openai_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/summary/text_to_image.py` & `nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/summary/text_to_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py` & `nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.5.0/pyproject.toml` & `nonebot_plugin_bilichat-1.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "py311",
 ]
 include = "\\.pyi?$"
 extend-exclude = ""
 
 [project]
 name = "nonebot-plugin-bilichat"
-version = "1.5.0"
+version = "1.6.0"
 description = "一个通过 OpenAI 来对b站视频进行总结插件"
 authors = [
     { name = "djkcyl", email = "cyl@cyllive.cn" },
     { name = "Well404", email = "well_404@outlook.com" },
 ]
 dependencies = [
     "httpx>=0.23.3",
```

### Comparing `nonebot_plugin_bilichat-1.5.0/PKG-INFO` & `nonebot_plugin_bilichat-1.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilichat
-Version: 1.5.0
+Version: 1.6.0
 Summary: 一个通过 OpenAI 来对b站视频进行总结插件
 Author-Email: djkcyl <cyl@cyllive.cn>, Well404 <well_404@outlook.com>
 License: AGPL3.0
 Requires-Python: <4.0,>=3.8
 Requires-Dist: httpx>=0.23.3
 Requires-Dist: bilireq>=0.2.4
 Requires-Dist: qrcode>=7.4.2
@@ -232,14 +232,30 @@
 4. 经测试，目前 `newbing` 至少能总结 12000 字符以上的文本，推测 token 上限应为 `gpt-4-32k-0314` 的 `32200` token，但过长的内容易造成输出内容包含额外内容或总结失败，因此也建议设置一个合理的 token 上限 ~~（反正不要钱，要啥自行车）~~
 5. 由于 `newbing` 限制较大，也不如 `openai` 听话，且需要联网查询资料，因此使用体验并不如 chatgpt ~~（反正不要钱，要啥自行车）~~
 
 ## 🎉 使用
 
 直接发送视频(专栏)链接即可
 
+### 参数表
+
+在发送视频时，可以额外添加以下类似 shell 指令的参数，进而对解析流程进行调整。例如
+
+```shell
+BV12v4y1E7NT --refresh
+BV12v4y1E7NT -r # 可以使用简写
+BV12v4y1E7NT -r --no-cache # 可以多个参数混用
+-r BV12v4y1E7NT -n # 虽然不建议，但确实可以把参数放前面
+```
+
+| 指令 | 简写 | 说明 |
+|:-----:|:----:|:----:|
+| --no-cache | -n | 本次总结禁用缓存(不会影响已存在的缓存文件) |
+| --refresh  | -r | 刷新此视频的词云和总结缓存(会覆盖已存在的缓存文件) |
+
 ### 指令表
 
 > 正在开发指令相关，请无视这里的模板
 > 指令设计方案征集中，如果有什么想要实现的功能可以在issue中提出
 
 | 指令 | 权限 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 1.5.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 1.6.0 Summary:
 ä¸ä¸ªéè¿ OpenAI æ¥å¯¹bç«è§é¢è¿è¡æ»ç»æä»¶ Author-Email: djkcyl
 cyllive.cn>, Well404
 outlook.com> License: AGPL3.0 Requires-Python: <4.0,>=3.8 Requires-Dist:
 httpx>=0.23.3 Requires-Dist: bilireq>=0.2.4 Requires-Dist: qrcode>=7.4.2
 Requires-Dist: pillow>=9.5.0 Requires-Dist: lxml>=4.9.2 Requires-Dist: nonebot-
 plugin-localstore>=0.4.1 Requires-Dist: nonebot-adapter-onebot>=2.2.2 Requires-
 Dist: nonebot-plugin-sentry>=0.2.2; extra == "extra" Requires-Dist:
@@ -108,16 +108,24 @@
 4. ç»æµè¯ï¼ç®å `newbing` è³å°è½æ»ç» 12000
 å­ç¬¦ä»¥ä¸çææ¬ï¼æ¨æµ token ä¸éåºä¸º `gpt-4-32k-0314` ç `32200`
 tokenï¼ä½è¿é¿çåå®¹æé æè¾åºåå®¹åå«é¢å¤åå®¹ææ»ç»å¤±è´¥ï¼å æ­¤ä¹å»ºè®®è®¾ç½®ä¸ä¸ªåçç
 token ä¸é ~~ï¼åæ­£ä¸è¦é±ï¼è¦å¥èªè¡è½¦ï¼~~ 5. ç±äº `newbing`
 éå¶è¾å¤§ï¼ä¹ä¸å¦ `openai`
 å¬è¯ï¼ä¸éè¦èç½æ¥è¯¢èµæï¼å æ­¤ä½¿ç¨ä½éªå¹¶ä¸å¦ chatgpt
 ~~ï¼åæ­£ä¸è¦é±ï¼è¦å¥èªè¡è½¦ï¼~~ ## ð ä½¿ç¨ ç´æ¥åéè§é¢
-(ä¸æ )é¾æ¥å³å¯ ### æä»¤è¡¨ >
-æ­£å¨å¼åæä»¤ç¸å³ï¼è¯·æ è§è¿éçæ¨¡æ¿ >
+(ä¸æ )é¾æ¥å³å¯ ### åæ°è¡¨
+å¨åéè§é¢æ¶ï¼å¯ä»¥é¢å¤æ·»å ä»¥ä¸ç±»ä¼¼ shell
+æä»¤çåæ°ï¼è¿èå¯¹è§£ææµç¨è¿è¡è°æ´ãä¾å¦ ```shell
+BV12v4y1E7NT --refresh BV12v4y1E7NT -r # å¯ä»¥ä½¿ç¨ç®å BV12v4y1E7NT -r --
+no-cache # å¯ä»¥å¤ä¸ªåæ°æ··ç¨ -r BV12v4y1E7NT -n #
+è½ç¶ä¸å»ºè®®ï¼ä½ç¡®å®å¯ä»¥æåæ°æ¾åé¢ ``` | æä»¤ | ç®å |
+è¯´æ | |:-----:|:----:|:----:| | --no-cache | -n | æ¬æ¬¡æ»ç»ç¦ç¨ç¼å­
+(ä¸ä¼å½±åå·²å­å¨çç¼å­æä»¶) | | --refresh | -r |
+å·æ°æ­¤è§é¢çè¯äºåæ»ç»ç¼å­(ä¼è¦çå·²å­å¨çç¼å­æä»¶) |
+### æä»¤è¡¨ > æ­£å¨å¼åæä»¤ç¸å³ï¼è¯·æ è§è¿éçæ¨¡æ¿ >
 æä»¤è®¾è®¡æ¹æ¡å¾éä¸­ï¼å¦ææä»ä¹æ³è¦å®ç°çåè½å¯ä»¥å¨issueä¸­æåº
 | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:----:|:----:|:
 ----:| | æä»¤1 | ä¸»äºº | å¦ | ç§è | æä»¤è¯´æ | | æä»¤2 | ç¾¤å |
 æ¯ | ç¾¤è | æä»¤è¯´æ | ## ð æè°¢ å¨æ­¤æè°¢ä»¥ä¸å¼åè
 (é¡¹ç®)å¯¹æ¬é¡¹ç®ååºçè´¡ç®ï¼ - [BibiGPT](https://github.com/JimmyLv/
 BibiGPT) é¡¹ç®çµææ¥æº - [bilibili-API-collect](https://github.com/
 SocialSisterYi/bilibili-API-collect) æå§æ¶éçåç§ BiliBili Api
```

