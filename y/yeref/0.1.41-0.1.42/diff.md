# Comparing `tmp/yeref-0.1.41.tar.gz` & `tmp/yeref-0.1.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.1.41.tar", last modified: Sun Apr 23 10:46:54 2023, max compression
+gzip compressed data, was "yeref-0.1.42.tar", last modified: Sun Apr 23 11:20:01 2023, max compression
```

## Comparing `yeref-0.1.41.tar` & `yeref-0.1.42.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-23 10:46:54.813516 yeref-0.1.41/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-04-23 10:46:54.813762 yeref-0.1.41/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-04-23 10:46:54.814895 yeref-0.1.41/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1154 2023-04-23 10:46:51.000000 yeref-0.1.41/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-23 10:46:54.807421 yeref-0.1.41/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.41/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)    69861 2023-04-23 10:46:01.000000 yeref-0.1.41/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   183551 2023-04-23 10:34:36.000000 yeref-0.1.41/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-23 10:46:54.812554 yeref-0.1.41/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-04-23 10:46:54.000000 yeref-0.1.41/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-04-23 10:46:54.000000 yeref-0.1.41/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-04-23 10:46:54.000000 yeref-0.1.41/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-04-23 10:46:54.000000 yeref-0.1.41/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-23 11:20:01.833575 yeref-0.1.42/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-04-23 11:20:01.833731 yeref-0.1.42/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-04-23 11:20:01.834451 yeref-0.1.42/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1154 2023-04-23 11:19:14.000000 yeref-0.1.42/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-23 11:20:01.830471 yeref-0.1.42/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.42/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)    69861 2023-04-23 10:46:01.000000 yeref-0.1.42/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   184285 2023-04-23 11:14:41.000000 yeref-0.1.42/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-23 11:20:01.833003 yeref-0.1.42/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-04-23 11:20:01.000000 yeref-0.1.42/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-04-23 11:20:01.000000 yeref-0.1.42/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-04-23 11:20:01.000000 yeref-0.1.42/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-04-23 11:20:01.000000 yeref-0.1.42/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.1.41/setup.py` & `yeref-0.1.42/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.1.41',
+      version='0.1.42',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
@@ -39,10 +39,10 @@
 # python setup.py bdist_wheel
 # endregion
 
 # python -m build
 
 # twine upload dist/*
 
-# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.41-py3-none-any.whl
+# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.42-py3-none-any.whl
 
 # python3 -m pip install --upgrade yeref
```

### Comparing `yeref-0.1.41/yeref/l_.py` & `yeref-0.1.42/yeref/l_.py`

 * *Files identical despite different names*

### Comparing `yeref-0.1.41/yeref/yeref.py` & `yeref-0.1.42/yeref/yeref.py`

 * *Files 1% similar despite different names*

```diff
@@ -313,31 +313,42 @@
         for item in pages['pages']:
             try:
                 if item['path'] == 'broadcasting-04-22':
                     page = telegraph_.get_page(path=item['path'], return_content=True, return_html=False)
                     content_json = json.loads(str(page['content'][0]))
 
                     for OFFER_USERTID, v in content_json.items():
-                        if bot_username in v['bots']:
-                            bots_, OFFER_TEXT, OFFER_MEDIATYPE, OFFER_FILEID, OFFER_BUTTON, OFFER_ISBUTTON, \
-                                OFFER_TGPHLINK, OFFER_ISTGPH, OFFER_ISSPOILER, OFFER_ISPIN, OFFER_ISSILENCE, \
-                                OFFER_ISGALLERY, OFFER_DT, OFFER_TZ = v
+                        if v[bot_username]:
+                            FereyAdsBot, FereyDemoBot, FereyWorkBot, FereyVPNBot, FereyAIBot, FereyToolsBot, \
+                                FereyMediaBot, FereyFindBot, FereyTargetBot, FereyPostBot, FereyBotBot, FereyUserBot, \
+                                FereyChannelBot, FereyGroupBot, OFFER_TEXT, OFFER_MEDIATYPE, OFFER_FILEID, \
+                                OFFER_BUTTON, OFFER_ISBUTTON, OFFER_TGPHLINK, OFFER_ISTGPH, OFFER_ISSPOILER, \
+                                OFFER_ISPIN, OFFER_ISSILENCE, OFFER_ISGALLERY, OFFER_DT, OFFER_TZ = v
 
                             sql = "INSERT OR IGNORE INTO OFFER (OFFER_USERTID, OFFER_TEXT, OFFER_MEDIATYPE, " \
                                   "OFFER_FILEID, OFFER_BUTTON, OFFER_ISBUTTON, OFFER_TGPHLINK, OFFER_ISTGPH, " \
                                   "OFFER_ISSPOILER, OFFER_ISPIN, OFFER_ISSILENCE, OFFER_ISGALLERY, OFFER_DT, " \
                                   "OFFER_TZ) VALUES (?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?)"
                             await db_change(sql, (int(OFFER_USERTID), v[OFFER_TEXT], v[OFFER_MEDIATYPE],
                                                   v[OFFER_FILEID], v[OFFER_BUTTON], v[OFFER_ISBUTTON],
                                                   v[OFFER_TGPHLINK], v[OFFER_ISTGPH], v[OFFER_ISSPOILER],
                                                   v[OFFER_ISPIN], v[OFFER_ISSILENCE], v[OFFER_ISGALLERY],
                                                   v[OFFER_DT], v[OFFER_TZ],), BASE_D)
 
-                            v['bots'].remove(bot_username)
-                            if not len(v['bots']):
+                            v[bot_username] = not v[bot_username]
+                            tmp_lst = [FereyAdsBot, FereyDemoBot, FereyWorkBot, FereyVPNBot, FereyAIBot, FereyToolsBot,
+                                       FereyMediaBot, FereyFindBot, FereyTargetBot, FereyPostBot, FereyBotBot,
+                                       FereyUserBot, FereyChannelBot, FereyGroupBot]
+
+                            cnt = 0
+                            for it in tmp_lst:
+                                if v[it]:
+                                    cnt += 1
+
+                            if not cnt:
                                 del content_json[str(OFFER_USERTID)]
                             else:
                                 content_json[str(OFFER_USERTID)] = v
 
                             post_dumps = json.dumps(content_json, ensure_ascii=False)
                             telegraph_.edit_page(path=item['path'], title="broadcasting", html_content=post_dumps)
                     break
```

