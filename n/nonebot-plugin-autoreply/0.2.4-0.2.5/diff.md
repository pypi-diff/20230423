# Comparing `tmp/nonebot_plugin_autoreply-0.2.4.tar.gz` & `tmp/nonebot_plugin_autoreply-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_autoreply-0.2.4.tar", last modified: Fri Apr 21 14:05:04 2023, max compression
+gzip compressed data, was "nonebot_plugin_autoreply-0.2.5.tar", last modified: Sun Apr 23 07:08:49 2023, max compression
```

## Comparing `nonebot_plugin_autoreply-0.2.4.tar` & `nonebot_plugin_autoreply-0.2.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1069 2023-04-21 14:04:54.385930 nonebot_plugin_autoreply-0.2.4/LICENSE
--rw-r--r--   0        0        0     8689 2023-04-21 14:04:54.385930 nonebot_plugin_autoreply-0.2.4/README.md
--rw-r--r--   0        0        0      303 2023-04-21 14:04:54.385930 nonebot_plugin_autoreply-0.2.4/nonebot_plugin_autoreply/__init__.py
--rw-r--r--   0        0        0     5086 2023-04-21 14:04:54.385930 nonebot_plugin_autoreply-0.2.4/nonebot_plugin_autoreply/__main__.py
--rw-r--r--   0        0        0     1788 2023-04-21 14:04:54.385930 nonebot_plugin_autoreply-0.2.4/nonebot_plugin_autoreply/config.py
--rw-r--r--   0        0        0      610 2023-04-21 14:05:04.605983 nonebot_plugin_autoreply-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     9230 1970-01-01 00:00:00.000000 nonebot_plugin_autoreply-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-23 07:08:40.541083 nonebot_plugin_autoreply-0.2.5/LICENSE
+-rw-r--r--   0        0        0     8693 2023-04-23 07:08:40.541083 nonebot_plugin_autoreply-0.2.5/README.md
+-rw-r--r--   0        0        0      303 2023-04-23 07:08:40.541083 nonebot_plugin_autoreply-0.2.5/nonebot_plugin_autoreply/__init__.py
+-rw-r--r--   0        0        0     4953 2023-04-23 07:08:40.541083 nonebot_plugin_autoreply-0.2.5/nonebot_plugin_autoreply/__main__.py
+-rw-r--r--   0        0        0     2421 2023-04-23 07:08:40.541083 nonebot_plugin_autoreply-0.2.5/nonebot_plugin_autoreply/config.py
+-rw-r--r--   0        0        0      610 2023-04-23 07:08:49.981943 nonebot_plugin_autoreply-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     9234 1970-01-01 00:00:00.000000 nonebot_plugin_autoreply-0.2.5/PKG-INFO
```

### Comparing `nonebot_plugin_autoreply-0.2.4/LICENSE` & `nonebot_plugin_autoreply-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_autoreply-0.2.4/README.md` & `nonebot_plugin_autoreply-0.2.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -93,16 +93,16 @@
 
 </details>
 
 ## ⚙️ 配置
 
 ### 回复配置
 
-插件的配置文件位于 `data/autoreply/replies.json` 下  
-因为把这种东西写在 env 里会太紧凑不易读，所以我单独弄出来了
+插件的配置文件位于 `data/autoreply` 下  
+在里面新建一个 `json` 后缀文件即可开始配置
 
 请根据下面的注释来编辑配置文件，实际配置文件内不要有注释
 
 ```jsonc
 [
   {
     // 消息的匹配规则，可以放置多个
@@ -282,14 +282,18 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.2.5
+
+- 可以加载多个回复 Json
+
 ### 0.2.4
 
 - 让字符串可以作为默认属性的 `match` 使用
 - 让 `@` 开头的字符串 `reply` 解析为 `plain` 形式的回复
 
 ### 0.2.3
```

#### html2text {}

```diff
@@ -16,17 +16,16 @@
 nonebot2 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡,
 æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤  pip ```bash pip
 install nonebot-plugin-autoreply ```   pdm ```bash pdm add nonebot-plugin-
 autoreply ```   poetry ```bash poetry add nonebot-plugin-autoreply ```   conda
 ```bash conda install nonebot-plugin-autoreply ```  æå¼ nonebot2 é¡¹ç®ç
 `bot.py` æä»¶, å¨å¶ä¸­åå¥ ```py nonebot.load_plugin
 ('nonebot_plugin_autoreply') ```  ## âï¸ éç½® ### åå¤éç½®
-æä»¶çéç½®æä»¶ä½äº `data/autoreply/replies.json` ä¸
-å ä¸ºæè¿ç§ä¸è¥¿åå¨ env
-éä¼å¤ªç´§åä¸æè¯»ï¼æä»¥æåç¬å¼åºæ¥äº
+æä»¶çéç½®æä»¶ä½äº `data/autoreply` ä¸ å¨éé¢æ°å»ºä¸ä¸ª `json`
+åç¼æä»¶å³å¯å¼å§éç½®
 è¯·æ ¹æ®ä¸é¢çæ³¨éæ¥ç¼è¾éç½®æä»¶ï¼å®ééç½®æä»¶åä¸è¦ææ³¨é
 ```jsonc [ { // æ¶æ¯çå¹éè§åï¼å¯ä»¥æ¾ç½®å¤ä¸ª "matches": [ { /
 / ç¨äºå¹éæ¶æ¯çææ¬ "match": "æµè¯", // å¹éæ¨¡å¼ï¼å¯é
 `full`(å®å¨å¹é)ã`fuzzy`(æ¨¡ç³å¹é)ã`regex`(æ­£åå¹é) /
 / å¨æ­£åå¹éä¸ï¼è¯·ä½¿ç¨ `\\` å¨ json éçæ­£åè¡¨è¾¾å¼éè¡¨ç¤º
 `\`ï¼å ä¸º json è§£ææ¶æ¬èº«å°±ä¼å° `\` ä½ä¸ºè½¬ä¹å­ç¬¦ /
 / å¯ä»¥ä¸å¡«ï¼é»è®¤ä¸º `fuzzy` "type": "fuzzy", // æ¯å¦éè¦ at
@@ -80,16 +79,16 @@
 æ­¤å½ä»¤ç¨äºéè½½èªå¨åå¤éç½®ï¼ä» `SUPERUSER` å¯ä»¥æ§è¡ ## ð
 èç³» QQï¼3076823485 Telegramï¼[@lgc2333](https://t.me/lgc2333) å¹æ°´ç¾¤ï¼
 [1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) -  èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.2.4 -
-è®©å­ç¬¦ä¸²å¯ä»¥ä½ä¸ºé»è®¤å±æ§ç `match` ä½¿ç¨ - è®© `@`
-å¼å¤´çå­ç¬¦ä¸² `reply` è§£æä¸º `plain` å½¢å¼çåå¤ ### 0.2.3 -
+imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.2.5 - å¯ä»¥å è½½å¤ä¸ªåå¤
+Json ### 0.2.4 - è®©å­ç¬¦ä¸²å¯ä»¥ä½ä¸ºé»è®¤å±æ§ç `match` ä½¿ç¨ - è®©
+`@` å¼å¤´çå­ç¬¦ä¸² `reply` è§£æä¸º `plain` å½¢å¼çåå¤ ### 0.2.3 -
 ä¿®å¤ä¸å¤ py 3.8 æ æ³ä½¿ç¨çç±»åæ³¨è§£ ### 0.2.2 -
 ä¿®å¤ç¾¤èåç¨æ·è¿æ»¤å¨æ æ³æ­£å¸¸ä½¿ç¨çé®é¢ ### 0.2.1 - ä¿®å¤å¤
 `match` æ æ³ä½¿ç¨çé®é¢ ### 0.2.0 - ä½¿ç¨ `rule`
 å¹éæ¶æ¯ï¼é¿åæ¥å¿å·å± -
 æ¯æä¸æ¬¡åå¤å¤æ¡æ¶æ¯ï¼è°æ´éç½®æä»¶ç»æ - å¢å äºä¸¤ä¸ª
 `.env` éç½®é¡¹ - å¢å ç­éè½½éç½®æä»¶çæä»¤
```

### Comparing `nonebot_plugin_autoreply-0.2.4/nonebot_plugin_autoreply/__main__.py` & `nonebot_plugin_autoreply-0.2.5/nonebot_plugin_autoreply/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from nonebot import on_command, on_message
 from nonebot.adapters.onebot.v11 import (
     GroupMessageEvent,
     Message,
     MessageEvent,
     MessageSegment,
 )
-from nonebot.log import logger
 from nonebot.matcher import Matcher
 from nonebot.permission import SUPERUSER
 from nonebot.typing import T_State
 from typing_extensions import TypeVarTuple, Unpack
 
 from .config import (
     FilterModel,
@@ -175,14 +174,9 @@
 
 
 reload_matcher = on_command("重载自动回复", permission=SUPERUSER)
 
 
 @reload_matcher.handle()
 async def _(matcher: Matcher):
-    try:
-        reload_replies()
-    except:
-        logger.exception("重载配置失败")
-        await matcher.finish("重载失败，请检查后台输出")
-    else:
-        await matcher.finish("重载自动回复配置成功~")
+    success, fail = reload_replies()
+    await matcher.finish(f"重载回复配置完毕~\n成功 {success} 个，失败 {fail} 个")
```

### Comparing `nonebot_plugin_autoreply-0.2.4/nonebot_plugin_autoreply/config.py` & `nonebot_plugin_autoreply-0.2.5/nonebot_plugin_autoreply/config.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 import json
 from pathlib import Path
 from typing import Any, Dict, Generic, List, Literal, Tuple, TypeVar, Union
 
 from nonebot import get_driver
+from nonebot.log import logger
 from pydantic import BaseModel
 
 T = TypeVar("T")
 
 DATA_PATH = Path.cwd() / "data" / "autoreply"
 if not DATA_PATH.exists():
     DATA_PATH.mkdir(parents=True)
 
-REPLY_JSON_PATH = DATA_PATH / "replies.json"
-if not REPLY_JSON_PATH.exists():
-    REPLY_JSON_PATH.write_text("[]", encoding="u8")
 
 MatchType = Union[str, "MatchModel"]
 ReplyType = Union[str, List["MessageSegmentModel"], "ReplyModel"]
 
 
 class MatchModel(BaseModel):
     match: str
@@ -56,18 +54,43 @@
     autoreply_priority: int = 99
 
 
 replies: List[ReplyEntryModel] = []
 config = ConfigModel.parse_obj(get_driver().config)
 
 
-def reload_replies():
+def reload_replies() -> Tuple[int, int]:
     replies.clear()
-    replies.extend(
-        [
-            ReplyEntryModel(**x)
-            for x in json.loads(REPLY_JSON_PATH.read_text(encoding="u8"))
-        ],
+
+    success = 0
+    fail = 0
+
+    for json_path in DATA_PATH.glob("*.json"):
+        file_name = json_path.name
+
+        try:
+            replies.extend(
+                [
+                    ReplyEntryModel(**x)
+                    for x in json.loads(json_path.read_text(encoding="u8"))
+                ],
+            )
+
+        except Exception:
+            logger.opt(colors=True).exception(
+                f"加载回复配置 <y>{file_name}</y> <l><r>失败</r></l>",
+            )
+            fail += 1
+
+        else:
+            logger.opt(colors=True).info(f"加载回复配置 <y>{file_name}</y> <l><g>成功</g></l>")
+            success += 1
+
+    logger.opt(colors=True).info(
+        "加载回复配置完毕，"
+        f"<l><g>成功</g></l> <y>{success}</y> 个，"
+        f"<l><r>失败</r></l> <y>{fail}</y> 个",
     )
+    return success, fail
 
 
 reload_replies()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nonebot_plugin_autoreply-0.2.4/pyproject.toml` & `nonebot_plugin_autoreply-0.2.5/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-autoreply"
-version = "0.2.4"
+version = "0.2.5"
 description = "A powerful auto reply plugin for NoneBot2"
 authors = [
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0rc1",
     "pydantic>=1.10.4",
```

### Comparing `nonebot_plugin_autoreply-0.2.4/PKG-INFO` & `nonebot_plugin_autoreply-0.2.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-autoreply
-Version: 0.2.4
+Version: 0.2.5
 Summary: A powerful auto reply plugin for NoneBot2
 Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-autoreply
 Author-Email: student_2333 <lgc2333@126.com>
 License: MIT
 Project-URL: Homepage, https://github.com/lgc-NB2Dev/nonebot-plugin-autoreply
 Requires-Python: <4.0,>=3.8
 Requires-Dist: nonebot2>=2.0.0rc1
@@ -108,16 +108,16 @@
 
 </details>
 
 ## ⚙️ 配置
 
 ### 回复配置
 
-插件的配置文件位于 `data/autoreply/replies.json` 下  
-因为把这种东西写在 env 里会太紧凑不易读，所以我单独弄出来了
+插件的配置文件位于 `data/autoreply` 下  
+在里面新建一个 `json` 后缀文件即可开始配置
 
 请根据下面的注释来编辑配置文件，实际配置文件内不要有注释
 
 ```jsonc
 [
   {
     // 消息的匹配规则，可以放置多个
@@ -297,14 +297,18 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.2.5
+
+- 可以加载多个回复 Json
+
 ### 0.2.4
 
 - 让字符串可以作为默认属性的 `match` 使用
 - 让 `@` 开头的字符串 `reply` 解析为 `plain` 形式的回复
 
 ### 0.2.3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-autoreply Version: 0.2.4 Summary: A
+Metadata-Version: 2.1 Name: nonebot-plugin-autoreply Version: 0.2.5 Summary: A
 powerful auto reply plugin for NoneBot2 Home-page: https://github.com/lgc-
 NB2Dev/nonebot-plugin-autoreply Author-Email: student_2333
 126.com> License: MIT Project-URL: Homepage, https://github.com/lgc-NB2Dev/
 nonebot-plugin-autoreply Requires-Python: <4.0,>=3.8 Requires-Dist:
 nonebot2>=2.0.0rc1 Requires-Dist: pydantic>=1.10.4 Requires-Dist: nonebot-
 adapter-onebot>=2.1.0 Requires-Dist: typing-extensions>=4.4.0 Description-
 Content-Type: text/markdown
@@ -24,17 +24,16 @@
 nonebot2 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡,
 æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤  pip ```bash pip
 install nonebot-plugin-autoreply ```   pdm ```bash pdm add nonebot-plugin-
 autoreply ```   poetry ```bash poetry add nonebot-plugin-autoreply ```   conda
 ```bash conda install nonebot-plugin-autoreply ```  æå¼ nonebot2 é¡¹ç®ç
 `bot.py` æä»¶, å¨å¶ä¸­åå¥ ```py nonebot.load_plugin
 ('nonebot_plugin_autoreply') ```  ## âï¸ éç½® ### åå¤éç½®
-æä»¶çéç½®æä»¶ä½äº `data/autoreply/replies.json` ä¸
-å ä¸ºæè¿ç§ä¸è¥¿åå¨ env
-éä¼å¤ªç´§åä¸æè¯»ï¼æä»¥æåç¬å¼åºæ¥äº
+æä»¶çéç½®æä»¶ä½äº `data/autoreply` ä¸ å¨éé¢æ°å»ºä¸ä¸ª `json`
+åç¼æä»¶å³å¯å¼å§éç½®
 è¯·æ ¹æ®ä¸é¢çæ³¨éæ¥ç¼è¾éç½®æä»¶ï¼å®ééç½®æä»¶åä¸è¦ææ³¨é
 ```jsonc [ { // æ¶æ¯çå¹éè§åï¼å¯ä»¥æ¾ç½®å¤ä¸ª "matches": [ { /
 / ç¨äºå¹éæ¶æ¯çææ¬ "match": "æµè¯", // å¹éæ¨¡å¼ï¼å¯é
 `full`(å®å¨å¹é)ã`fuzzy`(æ¨¡ç³å¹é)ã`regex`(æ­£åå¹é) /
 / å¨æ­£åå¹éä¸ï¼è¯·ä½¿ç¨ `\\` å¨ json éçæ­£åè¡¨è¾¾å¼éè¡¨ç¤º
 `\`ï¼å ä¸º json è§£ææ¶æ¬èº«å°±ä¼å° `\` ä½ä¸ºè½¬ä¹å­ç¬¦ /
 / å¯ä»¥ä¸å¡«ï¼é»è®¤ä¸º `fuzzy` "type": "fuzzy", // æ¯å¦éè¦ at
@@ -88,16 +87,16 @@
 æ­¤å½ä»¤ç¨äºéè½½èªå¨åå¤éç½®ï¼ä» `SUPERUSER` å¯ä»¥æ§è¡ ## ð
 èç³» QQï¼3076823485 Telegramï¼[@lgc2333](https://t.me/lgc2333) å¹æ°´ç¾¤ï¼
 [1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) -  èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.2.4 -
-è®©å­ç¬¦ä¸²å¯ä»¥ä½ä¸ºé»è®¤å±æ§ç `match` ä½¿ç¨ - è®© `@`
-å¼å¤´çå­ç¬¦ä¸² `reply` è§£æä¸º `plain` å½¢å¼çåå¤ ### 0.2.3 -
+imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.2.5 - å¯ä»¥å è½½å¤ä¸ªåå¤
+Json ### 0.2.4 - è®©å­ç¬¦ä¸²å¯ä»¥ä½ä¸ºé»è®¤å±æ§ç `match` ä½¿ç¨ - è®©
+`@` å¼å¤´çå­ç¬¦ä¸² `reply` è§£æä¸º `plain` å½¢å¼çåå¤ ### 0.2.3 -
 ä¿®å¤ä¸å¤ py 3.8 æ æ³ä½¿ç¨çç±»åæ³¨è§£ ### 0.2.2 -
 ä¿®å¤ç¾¤èåç¨æ·è¿æ»¤å¨æ æ³æ­£å¸¸ä½¿ç¨çé®é¢ ### 0.2.1 - ä¿®å¤å¤
 `match` æ æ³ä½¿ç¨çé®é¢ ### 0.2.0 - ä½¿ç¨ `rule`
 å¹éæ¶æ¯ï¼é¿åæ¥å¿å·å± -
 æ¯æä¸æ¬¡åå¤å¤æ¡æ¶æ¯ï¼è°æ´éç½®æä»¶ç»æ - å¢å äºä¸¤ä¸ª
 `.env` éç½®é¡¹ - å¢å ç­éè½½éç½®æä»¶çæä»¤
```

