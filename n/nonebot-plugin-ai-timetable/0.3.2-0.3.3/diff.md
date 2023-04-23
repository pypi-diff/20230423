# Comparing `tmp/nonebot_plugin_ai_timetable-0.3.2.tar.gz` & `tmp/nonebot_plugin_ai_timetable-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_ai_timetable-0.3.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_ai_timetable-0.3.3.tar", max compression
```

## Comparing `nonebot_plugin_ai_timetable-0.3.2.tar` & `nonebot_plugin_ai_timetable-0.3.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1065 2023-04-14 08:36:46.151410 nonebot_plugin_ai_timetable-0.3.2/LICENSE
--rw-r--r--   0        0        0     7671 2023-04-14 08:36:46.151410 nonebot_plugin_ai_timetable-0.3.2/README.md
--rw-r--r--   0        0        0    10863 2023-04-14 08:36:46.151410 nonebot_plugin_ai_timetable-0.3.2/nonebot_plugin_ai_timetable/__init__.py
--rw-r--r--   0        0        0    16712 2023-04-14 08:36:46.155410 nonebot_plugin_ai_timetable-0.3.2/nonebot_plugin_ai_timetable/utils.py
--rw-r--r--   0        0        0      496 2023-04-14 08:36:46.155410 nonebot_plugin_ai_timetable-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     8390 1970-01-01 00:00:00.000000 nonebot_plugin_ai_timetable-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-23 14:11:01.873509 nonebot_plugin_ai_timetable-0.3.3/LICENSE
+-rw-r--r--   0        0        0     7743 2023-04-23 14:11:01.873509 nonebot_plugin_ai_timetable-0.3.3/README.md
+-rw-r--r--   0        0        0    10816 2023-04-23 14:11:01.873509 nonebot_plugin_ai_timetable-0.3.3/nonebot_plugin_ai_timetable/__init__.py
+-rw-r--r--   0        0        0    16800 2023-04-23 14:11:01.873509 nonebot_plugin_ai_timetable-0.3.3/nonebot_plugin_ai_timetable/utils.py
+-rw-r--r--   0        0        0      496 2023-04-23 14:11:01.873509 nonebot_plugin_ai_timetable-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     8462 1970-01-01 00:00:00.000000 nonebot_plugin_ai_timetable-0.3.3/PKG-INFO
```

### Comparing `nonebot_plugin_ai_timetable-0.3.2/LICENSE` & `nonebot_plugin_ai_timetable-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ai_timetable-0.3.2/README.md` & `nonebot_plugin_ai_timetable-0.3.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -105,14 +105,19 @@
 4. 增加订阅指定课程的功能
 
 - 2023-04-14:
 
 1. 修复了订阅课程发送时间错误的bug
 2. 删去了文本中所有奇怪的口癖喵
 
+- 2023-04-23:
+
+1. 修改帮助
+2. 修复定时提醒重复发送的bug
+
 </details>
 
 ## 🎉命令
 
 1. 我的课表|小爱课表|本周课表|下周课表：获取本周|下周的完全课表，使用前须先导入课表，这里的课表是在线课表
 
 2. 导入课表：需要有小爱课表分享出来的链接，打开小爱课程表，手动添加课程或从教务导入(已适配了大部分高校)课程后
```

#### html2text {}

```diff
@@ -47,15 +47,16 @@
 - 2023-03-13ï¼ ä¿®å¤è®¢éæ©å«çä¸äºbug - 2023-03-29: 1.
 éæäºä»£ç ï¼ä¼åäºè®¸å¤å°æ¹~~ççç´¯æ­»äº~~ 2.
 ä¿®å¤äºä¸äºbugï¼ä¼åäºä½éª 3. å¢å äºæ©å«|ææ¥æ©å«çæ¥è¯¢
 4. æ´æ°çæ¬åå»ºè®®éæ°`å¯¼å¥è¯¾è¡¨`ï¼é¿ååºç°æäºbug - 2023-04-
 02: 1. ä¿®å¤bug 2. ä¼åå¸®å©å¾ç 3. å®æ¶ä»»å¡éæºå»¶å0-
 60sï¼é²æ­¢é£æ§ 4. å¢å è®¢éæå®è¯¾ç¨çåè½ - 2023-04-14: 1.
 ä¿®å¤äºè®¢éè¯¾ç¨åéæ¶é´éè¯¯çbug 2.
-å å»äºææ¬ä¸­ææå¥æªçå£çåµ  ## ðå½ä»¤ 1.
+å å»äºææ¬ä¸­ææå¥æªçå£çåµ - 2023-04-23: 1. ä¿®æ¹å¸®å© 2.
+ä¿®å¤å®æ¶æééå¤åéçbug  ## ðå½ä»¤ 1.
 æçè¯¾è¡¨|å°ç±è¯¾è¡¨|æ¬å¨è¯¾è¡¨|ä¸å¨è¯¾è¡¨ï¼è·åæ¬å¨|ä¸å¨çå®å¨è¯¾è¡¨ï¼ä½¿ç¨åé¡»åå¯¼å¥è¯¾è¡¨ï¼è¿éçè¯¾è¡¨æ¯å¨çº¿è¯¾è¡¨
 2.
 å¯¼å¥è¯¾è¡¨ï¼éè¦æå°ç±è¯¾è¡¨åäº«åºæ¥çé¾æ¥ï¼æå¼å°ç±è¯¾ç¨è¡¨ï¼æå¨æ·»å è¯¾ç¨æä»æå¡å¯¼å¥
 (å·²ééäºå¤§é¨åé«æ ¡)è¯¾ç¨å ![Image text](https://github.com/maoxig/
 nonebot-plugin-ai-timetable/blob/main/resource/export.jpg)
 å¨åºæ¬è®¾ç½®éæå¼å§ä¸è¯¾æ¶é´ç­è°æ´å¥½ä¹å
 (å°¤å¶æ¯æ¶é´ãèæ°)ï¼æåäº«è¯¾è¡¨å¾å°çé¾æ¥åéç»botå³å¯å¯¼å¥æ¬å°
```

### Comparing `nonebot_plugin_ai_timetable-0.3.2/nonebot_plugin_ai_timetable/__init__.py` & `nonebot_plugin_ai_timetable-0.3.3/nonebot_plugin_ai_timetable/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,15 +129,15 @@
         await add_alock_someday.finish('你还没有导入课表,发送/导入课表来导入吧！', at_sender=True)
     else:
         if scheduler:
             send_day = (AiTimetable.weekday_int(key)+5) % 7
             if scheduler.get_job(str(uid+"post_alock"+str(send_day))):
                 await add_alock_someday.finish("出错了！你好像已经订阅过这天的课表了呢", at_sender=True)
             scheduler.add_job(AiTimetable.post_alock, "cron", hour=timetable_alock_someday, second=random.randint(0, 60), id=str(
-                uid+"post_alock"+str(send_day)), day_of_week=send_day, misfire_grace_time=60, kwargs={"key": key, "uid": uid, "bot": bot, "event": event})
+                uid+"post_alock"+str(send_day)), day_of_week=send_day,kwargs={"key": key, "uid": uid, "bot": bot, "event": event})
             await add_alock_someday.finish("定时提醒添加成功！", at_sender=True)
         else:
             await add_alock_someday.finish("apscheduler插件未载入,无法添加定时提醒", at_sender=True)
 
 
 @remove_alock_someday.handle()
 async def _(bot: Bot, event: MessageEvent, key: str = RegexMatched()):
@@ -165,15 +165,15 @@
     if uid not in userdata:
         await add_alock_morningcalss.finish('你还没有导入课表,发送/导入课表来导入吧！', at_sender=True)
     else:
         if scheduler:
             if scheduler.get_job(str(uid+"post_alock_morningclass")):
                 await add_alock_morningcalss.finish("出错了！你好像已经订阅过早八提醒了呢", at_sender=True)
             scheduler.add_job(AiTimetable.post_alock_morningclass, "cron", hour=timetable_alock_8, second=random.randint(
-                0, 60), id=str(uid+"post_alock_morningclass"), misfire_grace_time=60, kwargs={"uid": uid, "bot": bot, "event": event})
+                0, 60), id=str(uid+"post_alock_morningclass"), kwargs={"uid": uid, "bot": bot, "event": event})
             await add_alock_morningcalss.finish("定时提醒添加成功！", at_sender=True)
         else:
             await add_alock_morningcalss.finish("apscheduler插件未载入,无法添加定时提醒", at_sender=True)
 
 
 @remove_alock_morningclass.handle()
 async def _(event: MessageEvent):
```

### Comparing `nonebot_plugin_ai_timetable-0.3.2/nonebot_plugin_ai_timetable/utils.py` & `nonebot_plugin_ai_timetable-0.3.3/nonebot_plugin_ai_timetable/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 
 
 class AiTimetable:
     res_url_re = r'^(https://i\.ai\.mi\.com/course-multi/table\?)*(ctId=)\d+(&userId=)\d*[1-9]\d*(&deviceId=)[0-9a-zA-Z]*(&sourceName=course-app-browser)'
     base_url_re = r'https://cdn\.cnbj1\.fds\.api\.mi-img.com/miai-fe-aischedule-wx-redirect-fe/redirect.html\?linkToken=.+'
 
-    ai_timetable__usage = "## 小爱课表帮助:\n- 我的/本周课表: 获取本周课表,也可以是下周\n- 导入课表: 使用小爱课程表分享的链接一键导入\n- 某日课表: 获取某日课表,如今日课表、周一课表\n- 更新课表: 更新本地课表信息,如果线上修改过小爱课表,发送该指令即可更新本地课表\n- 订阅/取消订阅xx课表: 可以订阅某天(如周一)的课表,在前一天晚上10点推送\n- 订阅/取消订阅早八: 订阅所有早八,在前一天晚上发出提醒\n- 上课/下节课: 获取当前课程信息以及今天以内的下节课信息\n- 早八|明日早八: 查询明天的早八"
+    ai_timetable__usage = "## 小爱课表帮助:\n- 我的/本周课表: 获取本周课表,也可以是下周\n- 导入课表: 使用小爱课程表分享的链接一键导入\n- 某日课表: 获取某日课表,如今日课表、周一课表\n- 更新课表: 更新本地课表信息,如果线上修改过小爱课表,发送该指令即可更新本地课表\n- 订阅/取消订阅xx课表: 可以订阅某天(如周一)的课表,在前一天晚上10点推送\n- 订阅/取消订阅早八: 订阅所有早八,在前一天晚上发出提醒\n- 订阅/取消订阅课程+课程名：订阅某节课程\n- 上课/下节课: 获取当前课程信息以及今天以内的下节课信息\n- 早八|明日早八: 查询明天的早八"
 
     headers = {
         'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/110.0.0.0 Safari/537.36 Edg/110.0.1587.63'
     }
     def __init__(self, uid) -> None:
         self.uid=uid
 
@@ -146,23 +146,25 @@
                 else:
                     msg = msg+'\n'+starttime+'-'+endtime+'\n' + \
                         courses["name"]+"\n@"+courses["position"]+'\n'
         return msg
 
     @staticmethod
     async def my_table(uid, key):
-        """获取本周或者下周课表"""
+        """
+        获取本周或者下周课表
+        """
         try:
-            async with get_new_page(viewport={"width": 1000, "height": 1200}) as page:
+            async with get_new_page(viewport={"width": 1000, "height": 1000}) as page:
                 await page.goto(userdata[uid][0],wait_until="networkidle")
                 # 这里使小爱课程表的导入按钮隐藏,防止遮挡课表
                 await page.evaluate('var t = document.querySelector("#root>div>div.importSchedule___UjEKt>div.footer___1iAis.toUp___2mciB"); t.style.display = "none"')
                 if '下' in key:  # 如果命令中有下字,就点击下一周的按钮
                     await page.click("#schedule-view > div.header___26sI1 > div.presentWeek___-o65e > div.rightBtn___2ZhSY")
-                pic = await page.screenshot(full_page=True,type="png")
+                pic = await page.screenshot(full_page=True,type="jpeg",quality=70)
                 return pic
         except Exception as e:
             logger.warning(f"获取课表时出错：{e}")
     @classmethod
     async def response_listener(cls,base_url, uid, response):
         """监听请求"""  
         if re.match(cls.res_url_re,response.url):
@@ -200,15 +202,17 @@
                     return "出错了，可能是没有在小爱课表内登录账户"
         except Exception as e:
             logger.warning(f"获取课表时出错：{e}")
             return f"出错了：{e}"
             
     @classmethod
     async def renew_table(cls,uid):
-        """用户已有url的情况下更新本地课表"""
+        """
+        用户已有url的情况下更新本地课表
+        """
         try:
             async with httpx.AsyncClient() as client:
                 res=await client.get(userdata[uid][1],headers=cls.headers)
                 usertable.update({uid:res.json()})
                         #更新课表
                 usertable[uid]["data"]["courses"].sort(
                     key=lambda x: int(x["sections"].split(",")[0]))
@@ -288,15 +292,15 @@
                     hours = int(timetable_send_time)#从设置中获取提前的小时数
                     minutes = int((timetable_send_time - hours) * 60)#从设置中获取提前的分钟数
                     time_obj = datetime.datetime.strptime(starttime, "%H:%M")#将字符串转换为datetime
                     new_time_obj = time_obj - datetime.timedelta(hours=hours, minutes=minutes)#进行时间的运算
                     sub_hour=new_time_obj.hour#获取发送时间的小时
                     sub_minute=new_time_obj.minute#获取发送时间的分钟
                     sub_day=courses["day"]-1
-                    scheduler.add_job(cls.send_sub_class,"cron",id=uid+courses["name"]+str(i), hour=sub_hour, minute=sub_minute, day_of_week=sub_day, second=random.randint(0, 60), misfire_grace_time=60, kwargs={"uid": uid, "bot": bot, "event": event,"course":{"name":courses["name"],"position":courses["position"],"teacher":courses["teacher"]}})
+                    scheduler.add_job(cls.send_sub_class,"cron",id=uid+courses["name"]+str(i), hour=sub_hour, minute=sub_minute, day_of_week=sub_day, second=random.randint(0, 60),kwargs={"uid": uid, "bot": bot, "event": event,"course":{"name":courses["name"],"position":courses["position"],"teacher":courses["teacher"]}})
         return f"成功订阅了{i}节课~"
     
     @classmethod
     def remove_sub_class(cls,**kwargs):
         uid,key=kwargs["uid"],kwargs["key"]
         i=0
         for courses in usertable[uid]["data"]["courses"]:
```

### Comparing `nonebot_plugin_ai_timetable-0.3.2/PKG-INFO` & `nonebot_plugin_ai_timetable-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-ai-timetable
-Version: 0.3.2
+Version: 0.3.3
 Summary: 小爱课程表
 Author: maoxiog
 Author-email: 674550338@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -124,14 +124,19 @@
 4. 增加订阅指定课程的功能
 
 - 2023-04-14:
 
 1. 修复了订阅课程发送时间错误的bug
 2. 删去了文本中所有奇怪的口癖喵
 
+- 2023-04-23:
+
+1. 修改帮助
+2. 修复定时提醒重复发送的bug
+
 </details>
 
 ## 🎉命令
 
 1. 我的课表|小爱课表|本周课表|下周课表：获取本周|下周的完全课表，使用前须先导入课表，这里的课表是在线课表
 
 2. 导入课表：需要有小爱课表分享出来的链接，打开小爱课程表，手动添加课程或从教务导入(已适配了大部分高校)课程后
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-ai-timetable Version: 0.3.2 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-ai-timetable Version: 0.3.3 Summary:
 å°ç±è¯¾ç¨è¡¨ Author: maoxiog Author-email: 674550338@qq.com Requires-Python:
 >=3.8,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: httpx (>=0.23.0,<0.24.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.1.0,<3.0.0) Requires-Dist: nonebot-
 plugin-apscheduler (>=0.2.0,<0.3.0) Requires-Dist: nonebot-plugin-htmlrender
@@ -57,15 +57,16 @@
 - 2023-03-13ï¼ ä¿®å¤è®¢éæ©å«çä¸äºbug - 2023-03-29: 1.
 éæäºä»£ç ï¼ä¼åäºè®¸å¤å°æ¹~~ççç´¯æ­»äº~~ 2.
 ä¿®å¤äºä¸äºbugï¼ä¼åäºä½éª 3. å¢å äºæ©å«|ææ¥æ©å«çæ¥è¯¢
 4. æ´æ°çæ¬åå»ºè®®éæ°`å¯¼å¥è¯¾è¡¨`ï¼é¿ååºç°æäºbug - 2023-04-
 02: 1. ä¿®å¤bug 2. ä¼åå¸®å©å¾ç 3. å®æ¶ä»»å¡éæºå»¶å0-
 60sï¼é²æ­¢é£æ§ 4. å¢å è®¢éæå®è¯¾ç¨çåè½ - 2023-04-14: 1.
 ä¿®å¤äºè®¢éè¯¾ç¨åéæ¶é´éè¯¯çbug 2.
-å å»äºææ¬ä¸­ææå¥æªçå£çåµ  ## ðå½ä»¤ 1.
+å å»äºææ¬ä¸­ææå¥æªçå£çåµ - 2023-04-23: 1. ä¿®æ¹å¸®å© 2.
+ä¿®å¤å®æ¶æééå¤åéçbug  ## ðå½ä»¤ 1.
 æçè¯¾è¡¨|å°ç±è¯¾è¡¨|æ¬å¨è¯¾è¡¨|ä¸å¨è¯¾è¡¨ï¼è·åæ¬å¨|ä¸å¨çå®å¨è¯¾è¡¨ï¼ä½¿ç¨åé¡»åå¯¼å¥è¯¾è¡¨ï¼è¿éçè¯¾è¡¨æ¯å¨çº¿è¯¾è¡¨
 2.
 å¯¼å¥è¯¾è¡¨ï¼éè¦æå°ç±è¯¾è¡¨åäº«åºæ¥çé¾æ¥ï¼æå¼å°ç±è¯¾ç¨è¡¨ï¼æå¨æ·»å è¯¾ç¨æä»æå¡å¯¼å¥
 (å·²ééäºå¤§é¨åé«æ ¡)è¯¾ç¨å ![Image text](https://github.com/maoxig/
 nonebot-plugin-ai-timetable/blob/main/resource/export.jpg)
 å¨åºæ¬è®¾ç½®éæå¼å§ä¸è¯¾æ¶é´ç­è°æ´å¥½ä¹å
 (å°¤å¶æ¯æ¶é´ãèæ°)ï¼æåäº«è¯¾è¡¨å¾å°çé¾æ¥åéç»botå³å¯å¯¼å¥æ¬å°
```

