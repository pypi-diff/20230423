# Comparing `tmp/nonebot-plugin-mixin-0.1.0.tar.gz` & `tmp/nonebot-plugin-mixin-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-mixin-0.1.0.tar", last modified: Sun Apr 23 05:48:56 2023, max compression
+gzip compressed data, was "nonebot-plugin-mixin-0.1.1.tar", last modified: Sun Apr 23 11:30:24 2023, max compression
```

## Comparing `nonebot-plugin-mixin-0.1.0.tar` & `nonebot-plugin-mixin-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 05:48:56.001417 nonebot-plugin-mixin-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-23 05:48:44.000000 nonebot-plugin-mixin-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-04-23 05:48:56.001417 nonebot-plugin-mixin-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-04-23 05:48:44.000000 nonebot-plugin-mixin-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 05:48:56.001417 nonebot-plugin-mixin-0.1.0/nonebot_plugin_mixin/
--rw-r--r--   0 runner    (1001) docker     (123)     8015 2023-04-23 05:48:44.000000 nonebot-plugin-mixin-0.1.0/nonebot_plugin_mixin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-23 05:48:44.000000 nonebot-plugin-mixin-0.1.0/nonebot_plugin_mixin/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 05:48:56.001417 nonebot-plugin-mixin-0.1.0/nonebot_plugin_mixin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-04-23 05:48:55.000000 nonebot-plugin-mixin-0.1.0/nonebot_plugin_mixin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-23 05:48:56.000000 nonebot-plugin-mixin-0.1.0/nonebot_plugin_mixin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 05:48:55.000000 nonebot-plugin-mixin-0.1.0/nonebot_plugin_mixin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-23 05:48:55.000000 nonebot-plugin-mixin-0.1.0/nonebot_plugin_mixin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-23 05:48:55.000000 nonebot-plugin-mixin-0.1.0/nonebot_plugin_mixin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-23 05:48:44.000000 nonebot-plugin-mixin-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 05:48:56.001417 nonebot-plugin-mixin-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:30:24.405837 nonebot-plugin-mixin-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-23 11:30:13.000000 nonebot-plugin-mixin-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-04-23 11:30:24.405837 nonebot-plugin-mixin-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-04-23 11:30:13.000000 nonebot-plugin-mixin-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:30:24.405837 nonebot-plugin-mixin-0.1.1/nonebot_plugin_mixin/
+-rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-04-23 11:30:13.000000 nonebot-plugin-mixin-0.1.1/nonebot_plugin_mixin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-23 11:30:13.000000 nonebot-plugin-mixin-0.1.1/nonebot_plugin_mixin/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:30:24.405837 nonebot-plugin-mixin-0.1.1/nonebot_plugin_mixin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-04-23 11:30:24.000000 nonebot-plugin-mixin-0.1.1/nonebot_plugin_mixin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-23 11:30:24.000000 nonebot-plugin-mixin-0.1.1/nonebot_plugin_mixin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 11:30:24.000000 nonebot-plugin-mixin-0.1.1/nonebot_plugin_mixin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-23 11:30:24.000000 nonebot-plugin-mixin-0.1.1/nonebot_plugin_mixin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-23 11:30:24.000000 nonebot-plugin-mixin-0.1.1/nonebot_plugin_mixin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-23 11:30:13.000000 nonebot-plugin-mixin-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 11:30:24.405837 nonebot-plugin-mixin-0.1.1/setup.cfg
```

### Comparing `nonebot-plugin-mixin-0.1.0/LICENSE` & `nonebot-plugin-mixin-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mixin-0.1.0/PKG-INFO` & `nonebot-plugin-mixin-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mixin
-Version: 0.1.0
+Version: 0.1.1
 Summary: 通过代码或非代码方式外部介入 NoneBot2 插件行为
 Author-email: HivertMoZara <worldmozara@163.com>
 License: MIT
 Project-URL: Homepage, https://github.com/NCBM/nonebot-plugin-mixin
 Project-URL: Repository, https://github.com/NCBM/nonebot-plugin-mixin
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -154,14 +154,15 @@
                 ("command1",)
                 ("command2", "sub")
                 ...
             regex: *ReMatch
                 regex: str
                 flags: int = 0
             to_me: bool = False
+        rule_override: bool = False  # 为 True 时完全覆盖 rule 数据 (v0.1.1 新增)
         priority: *int
         block: *bool
 ```
 
 而读取静态文件时，本插件默认会从某个文件中读取单个或多个并列的 Mixin 规则，因此数据文件的最上级必须是一个序列。例如：
 
 ```json
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-mixin Version: 0.1.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-mixin Version: 0.1.1 Summary:
 éè¿ä»£ç æéä»£ç æ¹å¼å¤é¨ä»å¥ NoneBot2 æä»¶è¡ä¸º Author-email:
 HivertMoZara
 163.com> License: MIT Project-URL: Homepage, https://github.com/NCBM/nonebot-
 plugin-mixin Project-URL: Repository, https://github.com/NCBM/nonebot-plugin-
 mixin Requires-Python: >=3.8 Description-Content-Type: text/markdown License-
 File: LICENSE
 # nonebot-plugin-mixin _â¨ éè¿ä»£ç æéä»£ç æ¹å¼å¤é¨ä»å¥ NoneBot2
@@ -36,12 +36,13 @@
 *ReMatch regex: str flags: int = 0 to_me: bool = False priority: *int block:
 *bool dest: MixinData # æ­¤æ®µåæ°åªç¨äºéæ©æ§ä¿®æ¹ Matcher çå±æ§
 type: *str rule: *MixinRule startswith: *CaseMatch msg: Tuple[str, ...]
 ignorecase: bool = False endswith: *CaseMatch msg: Tuple[str, ...] ignorecase:
 bool = False fullmatch: *CaseMatch msg: Tuple[str, ...] ignorecase: bool =
 False keywords: *Tuple[str, ...] "keyword1" ... command: *Tuple[Tuple[str,
 ...]] ("command1",) ("command2", "sub") ... regex: *ReMatch regex: str flags:
-int = 0 to_me: bool = False priority: *int block: *bool ```
+int = 0 to_me: bool = False rule_override: bool = False # ä¸º True
+æ¶å®å¨è¦ç rule æ°æ® (v0.1.1 æ°å¢) priority: *int block: *bool ```
 èè¯»åéææä»¶æ¶ï¼æ¬æä»¶é»è®¤ä¼ä»æä¸ªæä»¶ä¸­è¯»ååä¸ªæå¤ä¸ªå¹¶åç
 Mixin è§åï¼å æ­¤æ°æ®æä»¶çæä¸çº§å¿é¡»æ¯ä¸ä¸ªåºåãä¾å¦ï¼
 ```json [ { "source": ..., "dest": ... }, ... ] ``` ### è¦çè§å
 å¯éåæ°åªæç»å®å·ä½ææå¼çå±æ§ä¼è¢«å®å¨è¦çï¼æªç»å®å·ä½ææå¼çå±æ§é»è®¤ä¿çã
```

### Comparing `nonebot-plugin-mixin-0.1.0/README.md` & `nonebot-plugin-mixin-0.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -142,14 +142,15 @@
                 ("command1",)
                 ("command2", "sub")
                 ...
             regex: *ReMatch
                 regex: str
                 flags: int = 0
             to_me: bool = False
+        rule_override: bool = False  # 为 True 时完全覆盖 rule 数据 (v0.1.1 新增)
         priority: *int
         block: *bool
 ```
 
 而读取静态文件时，本插件默认会从某个文件中读取单个或多个并列的 Mixin 规则，因此数据文件的最上级必须是一个序列。例如：
 
 ```json
```

#### html2text {}

```diff
@@ -29,12 +29,13 @@
 *ReMatch regex: str flags: int = 0 to_me: bool = False priority: *int block:
 *bool dest: MixinData # æ­¤æ®µåæ°åªç¨äºéæ©æ§ä¿®æ¹ Matcher çå±æ§
 type: *str rule: *MixinRule startswith: *CaseMatch msg: Tuple[str, ...]
 ignorecase: bool = False endswith: *CaseMatch msg: Tuple[str, ...] ignorecase:
 bool = False fullmatch: *CaseMatch msg: Tuple[str, ...] ignorecase: bool =
 False keywords: *Tuple[str, ...] "keyword1" ... command: *Tuple[Tuple[str,
 ...]] ("command1",) ("command2", "sub") ... regex: *ReMatch regex: str flags:
-int = 0 to_me: bool = False priority: *int block: *bool ```
+int = 0 to_me: bool = False rule_override: bool = False # ä¸º True
+æ¶å®å¨è¦ç rule æ°æ® (v0.1.1 æ°å¢) priority: *int block: *bool ```
 èè¯»åéææä»¶æ¶ï¼æ¬æä»¶é»è®¤ä¼ä»æä¸ªæä»¶ä¸­è¯»ååä¸ªæå¤ä¸ªå¹¶åç
 Mixin è§åï¼å æ­¤æ°æ®æä»¶çæä¸çº§å¿é¡»æ¯ä¸ä¸ªåºåãä¾å¦ï¼
 ```json [ { "source": ..., "dest": ... }, ... ] ``` ### è¦çè§å
 å¯éåæ°åªæç»å®å·ä½ææå¼çå±æ§ä¼è¢«å®å¨è¦çï¼æªç»å®å·ä½ææå¼çå±æ§é»è®¤ä¿çã
```

### Comparing `nonebot-plugin-mixin-0.1.0/nonebot_plugin_mixin/__init__.py` & `nonebot-plugin-mixin-0.1.1/nonebot_plugin_mixin/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,14 +149,15 @@
             ) if getattr(self, x) is not None
         )
 
 
 class MixinData(BaseModel):
     type: Optional[str] = None
     rule: MixinRule = Field(default_factory=MixinRule)
+    rule_override: bool = False
     priority: Optional[int] = None
     block: Optional[bool] = None
 
 
 class Mixin(BaseModel):
     source: MixinQuery
     dest: MixinData
@@ -164,15 +165,15 @@
 
 mixins: List[Mixin] = []
 
 
 def mixin(ma: Type[Matcher], ch: MixinData):
     if ch.type is not None:
         ma.type = ch.type
-    ma.rule = ch.rule.to_rule(ma.rule)
+    ma.rule = ch.rule.to_rule(None if ch.rule_override else ma.rule)
     if ch.priority is not None:
         # This operation only changes the priority in the matcher, which
         # means another place the priority stored in should also be changed.
         ma.priority = ch.priority
     if ch.block is not None:
         ma.block = ch.block
     logger.info(f"已介入 {ma!r} 的属性")
```

### Comparing `nonebot-plugin-mixin-0.1.0/nonebot_plugin_mixin.egg-info/PKG-INFO` & `nonebot-plugin-mixin-0.1.1/nonebot_plugin_mixin.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mixin
-Version: 0.1.0
+Version: 0.1.1
 Summary: 通过代码或非代码方式外部介入 NoneBot2 插件行为
 Author-email: HivertMoZara <worldmozara@163.com>
 License: MIT
 Project-URL: Homepage, https://github.com/NCBM/nonebot-plugin-mixin
 Project-URL: Repository, https://github.com/NCBM/nonebot-plugin-mixin
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -154,14 +154,15 @@
                 ("command1",)
                 ("command2", "sub")
                 ...
             regex: *ReMatch
                 regex: str
                 flags: int = 0
             to_me: bool = False
+        rule_override: bool = False  # 为 True 时完全覆盖 rule 数据 (v0.1.1 新增)
         priority: *int
         block: *bool
 ```
 
 而读取静态文件时，本插件默认会从某个文件中读取单个或多个并列的 Mixin 规则，因此数据文件的最上级必须是一个序列。例如：
 
 ```json
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-mixin Version: 0.1.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-mixin Version: 0.1.1 Summary:
 éè¿ä»£ç æéä»£ç æ¹å¼å¤é¨ä»å¥ NoneBot2 æä»¶è¡ä¸º Author-email:
 HivertMoZara
 163.com> License: MIT Project-URL: Homepage, https://github.com/NCBM/nonebot-
 plugin-mixin Project-URL: Repository, https://github.com/NCBM/nonebot-plugin-
 mixin Requires-Python: >=3.8 Description-Content-Type: text/markdown License-
 File: LICENSE
 # nonebot-plugin-mixin _â¨ éè¿ä»£ç æéä»£ç æ¹å¼å¤é¨ä»å¥ NoneBot2
@@ -36,12 +36,13 @@
 *ReMatch regex: str flags: int = 0 to_me: bool = False priority: *int block:
 *bool dest: MixinData # æ­¤æ®µåæ°åªç¨äºéæ©æ§ä¿®æ¹ Matcher çå±æ§
 type: *str rule: *MixinRule startswith: *CaseMatch msg: Tuple[str, ...]
 ignorecase: bool = False endswith: *CaseMatch msg: Tuple[str, ...] ignorecase:
 bool = False fullmatch: *CaseMatch msg: Tuple[str, ...] ignorecase: bool =
 False keywords: *Tuple[str, ...] "keyword1" ... command: *Tuple[Tuple[str,
 ...]] ("command1",) ("command2", "sub") ... regex: *ReMatch regex: str flags:
-int = 0 to_me: bool = False priority: *int block: *bool ```
+int = 0 to_me: bool = False rule_override: bool = False # ä¸º True
+æ¶å®å¨è¦ç rule æ°æ® (v0.1.1 æ°å¢) priority: *int block: *bool ```
 èè¯»åéææä»¶æ¶ï¼æ¬æä»¶é»è®¤ä¼ä»æä¸ªæä»¶ä¸­è¯»ååä¸ªæå¤ä¸ªå¹¶åç
 Mixin è§åï¼å æ­¤æ°æ®æä»¶çæä¸çº§å¿é¡»æ¯ä¸ä¸ªåºåãä¾å¦ï¼
 ```json [ { "source": ..., "dest": ... }, ... ] ``` ### è¦çè§å
 å¯éåæ°åªæç»å®å·ä½ææå¼çå±æ§ä¼è¢«å®å¨è¦çï¼æªç»å®å·ä½ææå¼çå±æ§é»è®¤ä¿çã
```

