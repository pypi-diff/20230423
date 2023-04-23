# Comparing `tmp/biblebot-0.4.1.tar.gz` & `tmp/biblebot-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biblebot-0.4.1.tar", last modified: Wed Aug  3 06:19:18 2022, max compression
+gzip compressed data, was "dist\biblebot-0.4.2.tar", last modified: Sun Apr 23 07:50:07 2023, max compression
```

## Comparing `biblebot-0.4.1.tar` & `biblebot-0.4.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2022-08-03 06:19:18.623063 biblebot-0.4.1/
--rw-rw-rw-   0        0        0     1092 2022-05-30 10:06:22.000000 biblebot-0.4.1/LICENSE
--rw-rw-rw-   0        0        0    11726 2022-08-03 06:19:18.623063 biblebot-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0    11028 2022-05-30 10:10:18.000000 biblebot-0.4.1/README.md
-drwxrwxrwx   0        0        0        0 2022-08-03 06:19:18.466819 biblebot-0.4.1/biblebot/
--rw-rw-rw-   0        0        0      691 2021-02-02 08:18:09.000000 biblebot-0.4.1/biblebot/__init__.py
--rw-rw-rw-   0        0        0      557 2022-08-03 06:17:43.000000 biblebot-0.4.1/biblebot/__version__.py
-drwxrwxrwx   0        0        0        0 2022-08-03 06:19:18.576193 biblebot-0.4.1/biblebot/api/
--rw-rw-rw-   0        0        0     2494 2022-06-27 05:51:38.000000 biblebot-0.4.1/biblebot/api/__init__.py
--rw-rw-rw-   0        0        0     6463 2020-10-28 08:43:32.000000 biblebot-0.4.1/biblebot/api/_mileage.py
--rw-rw-rw-   0        0        0     2974 2020-10-28 08:43:32.000000 biblebot-0.4.1/biblebot/api/base.py
--rw-rw-rw-   0        0        0     3398 2022-05-30 10:06:22.000000 biblebot-0.4.1/biblebot/api/common.py
--rw-rw-rw-   0        0        0    19912 2022-08-03 06:17:43.000000 biblebot-0.4.1/biblebot/api/intranet.py
--rw-rw-rw-   0        0        0     4599 2020-10-28 08:43:32.000000 biblebot-0.4.1/biblebot/api/kbu.py
--rw-rw-rw-   0        0        0     6410 2022-05-30 10:06:22.000000 biblebot-0.4.1/biblebot/api/library.py
--rw-rw-rw-   0        0        0    13916 2022-05-31 09:04:43.000000 biblebot-0.4.1/biblebot/api/lms.py
--rw-rw-rw-   0        0        0     6692 2022-05-23 10:36:47.000000 biblebot-0.4.1/biblebot/api/mileage.py
--rw-rw-rw-   0        0        0     1387 2020-10-28 08:43:32.000000 biblebot-0.4.1/biblebot/exceptions.py
-drwxrwxrwx   0        0        0        0 2022-08-03 06:19:18.623063 biblebot-0.4.1/biblebot/reqeust/
--rw-rw-rw-   0        0        0      377 2020-10-28 08:43:32.000000 biblebot-0.4.1/biblebot/reqeust/__init__.py
--rw-rw-rw-   0        0        0     2821 2021-02-04 04:00:45.000000 biblebot-0.4.1/biblebot/reqeust/aiohttp_conn.py
--rw-rw-rw-   0        0        0     5087 2020-10-28 08:43:32.000000 biblebot-0.4.1/biblebot/reqeust/base.py
--rw-rw-rw-   0        0        0     2312 2020-10-28 08:43:32.000000 biblebot-0.4.1/biblebot/reqeust/requests_conn.py
-drwxrwxrwx   0        0        0        0 2022-08-03 06:19:18.513691 biblebot-0.4.1/biblebot.egg-info/
--rw-rw-rw-   0        0        0    11726 2022-08-03 06:19:15.000000 biblebot-0.4.1/biblebot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      581 2022-08-03 06:19:18.000000 biblebot-0.4.1/biblebot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-03 06:19:16.000000 biblebot-0.4.1/biblebot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2022-08-03 06:19:17.000000 biblebot-0.4.1/biblebot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-08-03 06:19:17.000000 biblebot-0.4.1/biblebot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-08-03 06:19:18.623063 biblebot-0.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1258 2022-05-30 10:06:22.000000 biblebot-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 07:50:07.000000 biblebot-0.4.2/
+-rw-rw-rw-   0        0        0     1092 2023-04-23 07:47:19.000000 biblebot-0.4.2/LICENSE
+-rw-rw-rw-   0        0        0    11662 2023-04-23 07:50:07.000000 biblebot-0.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0    10964 2023-04-23 07:47:19.000000 biblebot-0.4.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 07:50:06.000000 biblebot-0.4.2/biblebot/
+-rw-rw-rw-   0        0        0      691 2021-02-02 08:18:09.000000 biblebot-0.4.2/biblebot/__init__.py
+-rw-rw-rw-   0        0        0      557 2023-04-23 07:48:38.000000 biblebot-0.4.2/biblebot/__version__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 07:50:06.000000 biblebot-0.4.2/biblebot/api/
+-rw-rw-rw-   0        0        0     2494 2023-04-03 06:31:51.000000 biblebot-0.4.2/biblebot/api/__init__.py
+-rw-rw-rw-   0        0        0     6463 2020-10-28 08:43:32.000000 biblebot-0.4.2/biblebot/api/_mileage.py
+-rw-rw-rw-   0        0        0     2974 2020-10-28 08:43:32.000000 biblebot-0.4.2/biblebot/api/base.py
+-rw-rw-rw-   0        0        0     3398 2023-04-03 06:31:51.000000 biblebot-0.4.2/biblebot/api/common.py
+-rw-rw-rw-   0        0        0    19912 2023-04-03 06:31:51.000000 biblebot-0.4.2/biblebot/api/intranet.py
+-rw-rw-rw-   0        0        0     4599 2020-10-28 08:43:32.000000 biblebot-0.4.2/biblebot/api/kbu.py
+-rw-rw-rw-   0        0        0     6410 2023-04-03 06:31:51.000000 biblebot-0.4.2/biblebot/api/library.py
+-rw-rw-rw-   0        0        0    13916 2022-05-31 09:04:43.000000 biblebot-0.4.2/biblebot/api/lms.py
+-rw-rw-rw-   0        0        0     6692 2023-04-03 06:31:51.000000 biblebot-0.4.2/biblebot/api/mileage.py
+-rw-rw-rw-   0        0        0     1387 2020-10-28 08:43:32.000000 biblebot-0.4.2/biblebot/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-23 07:50:07.000000 biblebot-0.4.2/biblebot/reqeust/
+-rw-rw-rw-   0        0        0      377 2020-10-28 08:43:32.000000 biblebot-0.4.2/biblebot/reqeust/__init__.py
+-rw-rw-rw-   0        0        0     2821 2021-02-04 04:00:45.000000 biblebot-0.4.2/biblebot/reqeust/aiohttp_conn.py
+-rw-rw-rw-   0        0        0     5087 2020-10-28 08:43:32.000000 biblebot-0.4.2/biblebot/reqeust/base.py
+-rw-rw-rw-   0        0        0     2312 2020-10-28 08:43:32.000000 biblebot-0.4.2/biblebot/reqeust/requests_conn.py
+drwxrwxrwx   0        0        0        0 2023-04-23 07:50:06.000000 biblebot-0.4.2/biblebot.egg-info/
+-rw-rw-rw-   0        0        0    11662 2023-04-23 07:50:06.000000 biblebot-0.4.2/biblebot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      581 2023-04-23 07:50:06.000000 biblebot-0.4.2/biblebot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 07:50:06.000000 biblebot-0.4.2/biblebot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-04-23 07:50:06.000000 biblebot-0.4.2/biblebot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-23 07:50:06.000000 biblebot-0.4.2/biblebot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 07:50:07.000000 biblebot-0.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     1258 2023-04-03 06:31:06.000000 biblebot-0.4.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `biblebot-0.4.1/LICENSE` & `biblebot-0.4.2/LICENSE`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License
 
-Copyright (c) 2022 Kyungmin Lee
+Copyright (c) 2023 Kyungmin Lee
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `biblebot-0.4.1/PKG-INFO` & `biblebot-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biblebot
-Version: 0.4.1
+Version: 0.4.2
 Summary: Scraper for KBU students
 Home-page: https://github.com/rekyungmin/biblebot-scraper
 Author: Kyungmin Lee
 Author-email: rekyungmin@gmail.com
 Maintainer: Kyungmin Lee <rekyungmin@gmail.com>, Yongki Kim <ygflove@likelion.org>
 License: UNKNOWN
 Platform: UNKNOWN
@@ -22,15 +22,15 @@
 <p align="center">
 <a href="https://www.python.org/downloads/release/python-370/"><img alt="Python" src="https://img.shields.io/badge/python-3.7-blue?logo=python&logoColor=white"></a>
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 </p>
 
 성서봇 스크래이퍼는 한국성서대학교와 연관된 정보를 수집할 수 있는 파이썬 패키지입니다.
 
-이 패키지를 바탕으로, **성서봇** 모바일 애플리케이션([Android](https://play.google.com/store/apps/details?id=com.blogspot.ramming125.kbubot&hl=ko) / [IOS](https://apps.apple.com/kr/app/성서봇/id1441276020))이 한국성서대학교학생들에게 2018년부터 실서비스 되고 있습니다.  
+이 패키지를 바탕으로, **성서봇** 모바일 애플리케이션([Android](https://play.google.com/store/apps/details?id=com.blogspot.ramming125.kbubot&hl=ko))이 한국성서대학교학생들에게 2018년부터 실서비스 되고 있습니다.
 
 이 패키지는 다섯 가지 웹사이트에 대한 스크래이퍼를 제공합니다.
 
 1. [한국성서대학교 인트라넷](https://kbuis.bible.ac.kr/) 스크래이퍼  
 2. [한국성서대학교 LMS](https://lms.bible.ac.kr/) 스크래이퍼
 3. [한국성서대학교 홈페이지](https://www.bible.ac.kr/) 스크래이퍼  
 4. [OKPOS 마일리지 시스템](https://asp.netusys.com/) 스크래이퍼
```

#### html2text {}

```diff
@@ -1,24 +1,23 @@
-Metadata-Version: 2.1 Name: biblebot Version: 0.4.1 Summary: Scraper for KBU
+Metadata-Version: 2.1 Name: biblebot Version: 0.4.2 Summary: Scraper for KBU
 students Home-page: https://github.com/rekyungmin/biblebot-scraper Author:
 Kyungmin Lee Author-email: rekyungmin@gmail.com Maintainer: Kyungmin Lee
 gmail.com>, Yongki Kim
 likelion.org> License: UNKNOWN Platform: UNKNOWN Classifier: License :: OSI
 Approved :: MIT License Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.7 Requires-Python:
 >=3.7 Description-Content-Type: text/markdown Provides-Extra: http License-
 File: LICENSE
                         ****** Biblebot Scraper ******
                          [Python] [Code_style:_black]
 ì±ìë´ ì¤í¬ëì´í¼ë íêµ­ì±ìëíêµì ì°ê´ë ì ë³´ë¥¼
 ìì§í  ì ìë íì´ì¬ í¨í¤ì§ìëë¤. ì´ í¨í¤ì§ë¥¼
 ë°íì¼ë¡, **ì±ìë´** ëª¨ë°ì¼ ì íë¦¬ì¼ì´ì([Android](https://
-play.google.com/store/apps/details?id=com.blogspot.ramming125.kbubot&hl=ko) /
-[IOS](https://apps.apple.com/kr/app/ì±ìë´/id1441276020))ì´
+play.google.com/store/apps/details?id=com.blogspot.ramming125.kbubot&hl=ko))ì´
 íêµ­ì±ìëíêµíìë¤ìê² 2018ëë¶í° ì¤ìë¹ì¤ ëê³ 
 ììµëë¤. ì´ í¨í¤ì§ë ë¤ì¯ ê°ì§ ì¹ì¬ì´í¸ì ëí
 ì¤í¬ëì´í¼ë¥¼ ì ê³µí©ëë¤. 1. [íêµ­ì±ìëíêµ ì¸í¸ë¼ë·]
 (https://kbuis.bible.ac.kr/) ì¤í¬ëì´í¼ 2. [íêµ­ì±ìëíêµ LMS]
 (https://lms.bible.ac.kr/) ì¤í¬ëì´í¼ 3. [íêµ­ì±ìëíêµ
 ííì´ì§](https://www.bible.ac.kr/) ì¤í¬ëì´í¼ 4. [OKPOS ë§ì¼ë¦¬ì§
 ìì¤í](https://asp.netusys.com/) ì¤í¬ëì´í¼ 5. [íêµ­ì±ìëíêµ
```

### Comparing `biblebot-0.4.1/README.md` & `biblebot-0.4.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <p align="center">
 <a href="https://www.python.org/downloads/release/python-370/"><img alt="Python" src="https://img.shields.io/badge/python-3.7-blue?logo=python&logoColor=white"></a>
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 </p>
 
 성서봇 스크래이퍼는 한국성서대학교와 연관된 정보를 수집할 수 있는 파이썬 패키지입니다.
 
-이 패키지를 바탕으로, **성서봇** 모바일 애플리케이션([Android](https://play.google.com/store/apps/details?id=com.blogspot.ramming125.kbubot&hl=ko) / [IOS](https://apps.apple.com/kr/app/성서봇/id1441276020))이 한국성서대학교학생들에게 2018년부터 실서비스 되고 있습니다.  
+이 패키지를 바탕으로, **성서봇** 모바일 애플리케이션([Android](https://play.google.com/store/apps/details?id=com.blogspot.ramming125.kbubot&hl=ko))이 한국성서대학교학생들에게 2018년부터 실서비스 되고 있습니다.
 
 이 패키지는 다섯 가지 웹사이트에 대한 스크래이퍼를 제공합니다.
 
 1. [한국성서대학교 인트라넷](https://kbuis.bible.ac.kr/) 스크래이퍼  
 2. [한국성서대학교 LMS](https://lms.bible.ac.kr/) 스크래이퍼
 3. [한국성서대학교 홈페이지](https://www.bible.ac.kr/) 스크래이퍼  
 4. [OKPOS 마일리지 시스템](https://asp.netusys.com/) 스크래이퍼
```

#### html2text {}

```diff
@@ -1,14 +1,13 @@
                         ****** Biblebot Scraper ******
                          [Python] [Code_style:_black]
 ì±ìë´ ì¤í¬ëì´í¼ë íêµ­ì±ìëíêµì ì°ê´ë ì ë³´ë¥¼
 ìì§í  ì ìë íì´ì¬ í¨í¤ì§ìëë¤. ì´ í¨í¤ì§ë¥¼
 ë°íì¼ë¡, **ì±ìë´** ëª¨ë°ì¼ ì íë¦¬ì¼ì´ì([Android](https://
-play.google.com/store/apps/details?id=com.blogspot.ramming125.kbubot&hl=ko) /
-[IOS](https://apps.apple.com/kr/app/ì±ìë´/id1441276020))ì´
+play.google.com/store/apps/details?id=com.blogspot.ramming125.kbubot&hl=ko))ì´
 íêµ­ì±ìëíêµíìë¤ìê² 2018ëë¶í° ì¤ìë¹ì¤ ëê³ 
 ììµëë¤. ì´ í¨í¤ì§ë ë¤ì¯ ê°ì§ ì¹ì¬ì´í¸ì ëí
 ì¤í¬ëì´í¼ë¥¼ ì ê³µí©ëë¤. 1. [íêµ­ì±ìëíêµ ì¸í¸ë¼ë·]
 (https://kbuis.bible.ac.kr/) ì¤í¬ëì´í¼ 2. [íêµ­ì±ìëíêµ LMS]
 (https://lms.bible.ac.kr/) ì¤í¬ëì´í¼ 3. [íêµ­ì±ìëíêµ
 ííì´ì§](https://www.bible.ac.kr/) ì¤í¬ëì´í¼ 4. [OKPOS ë§ì¼ë¦¬ì§
 ìì¤í](https://asp.netusys.com/) ì¤í¬ëì´í¼ 5. [íêµ­ì±ìëíêµ
```

### Comparing `biblebot-0.4.1/biblebot/__init__.py` & `biblebot-0.4.2/biblebot/__init__.py`

 * *Files identical despite different names*

### Comparing `biblebot-0.4.1/biblebot/__version__.py` & `biblebot-0.4.2/biblebot/__version__.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,13 +9,13 @@
     "__copyright__",
     "__contributors__",
 )
 
 __title__ = "biblebot"
 __description__ = "Scraper for KBU students"
 __url__ = "https://github.com/rekyungmin/biblebot-scraper"
-__version__ = "0.4.1"
+__version__ = "0.4.2"
 __author__ = "Kyungmin Lee"
 __author_email__ = "rekyungmin@gmail.com"
 __license__ = "MIT"
-__copyright__ = "Copyright 2022 Kyungmin Lee"
+__copyright__ = "Copyright 2023 Kyungmin Lee"
 __contributors__ = "Yongki Kim <ygflove@likelion.org>",
```

### Comparing `biblebot-0.4.1/biblebot/api/__init__.py` & `biblebot-0.4.2/biblebot/api/__init__.py`

 * *Files identical despite different names*

### Comparing `biblebot-0.4.1/biblebot/api/_mileage.py` & `biblebot-0.4.2/biblebot/api/_mileage.py`

 * *Files identical despite different names*

### Comparing `biblebot-0.4.1/biblebot/api/base.py` & `biblebot-0.4.2/biblebot/api/base.py`

 * *Files identical despite different names*

### Comparing `biblebot-0.4.1/biblebot/api/common.py` & `biblebot-0.4.2/biblebot/api/common.py`

 * *Files identical despite different names*

### Comparing `biblebot-0.4.1/biblebot/api/intranet.py` & `biblebot-0.4.2/biblebot/api/intranet.py`

 * *Files identical despite different names*

### Comparing `biblebot-0.4.1/biblebot/api/kbu.py` & `biblebot-0.4.2/biblebot/api/kbu.py`

 * *Files identical despite different names*

### Comparing `biblebot-0.4.1/biblebot/api/library.py` & `biblebot-0.4.2/biblebot/api/library.py`

 * *Files identical despite different names*

### Comparing `biblebot-0.4.1/biblebot/api/lms.py` & `biblebot-0.4.2/biblebot/api/lms.py`

 * *Files identical despite different names*

### Comparing `biblebot-0.4.1/biblebot/api/mileage.py` & `biblebot-0.4.2/biblebot/api/mileage.py`

 * *Files identical despite different names*

### Comparing `biblebot-0.4.1/biblebot/exceptions.py` & `biblebot-0.4.2/biblebot/exceptions.py`

 * *Files identical despite different names*

### Comparing `biblebot-0.4.1/biblebot/reqeust/aiohttp_conn.py` & `biblebot-0.4.2/biblebot/reqeust/aiohttp_conn.py`

 * *Files identical despite different names*

### Comparing `biblebot-0.4.1/biblebot/reqeust/base.py` & `biblebot-0.4.2/biblebot/reqeust/base.py`

 * *Files identical despite different names*

### Comparing `biblebot-0.4.1/biblebot/reqeust/requests_conn.py` & `biblebot-0.4.2/biblebot/reqeust/requests_conn.py`

 * *Files identical despite different names*

### Comparing `biblebot-0.4.1/biblebot.egg-info/PKG-INFO` & `biblebot-0.4.2/biblebot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biblebot
-Version: 0.4.1
+Version: 0.4.2
 Summary: Scraper for KBU students
 Home-page: https://github.com/rekyungmin/biblebot-scraper
 Author: Kyungmin Lee
 Author-email: rekyungmin@gmail.com
 Maintainer: Kyungmin Lee <rekyungmin@gmail.com>, Yongki Kim <ygflove@likelion.org>
 License: UNKNOWN
 Platform: UNKNOWN
@@ -22,15 +22,15 @@
 <p align="center">
 <a href="https://www.python.org/downloads/release/python-370/"><img alt="Python" src="https://img.shields.io/badge/python-3.7-blue?logo=python&logoColor=white"></a>
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 </p>
 
 성서봇 스크래이퍼는 한국성서대학교와 연관된 정보를 수집할 수 있는 파이썬 패키지입니다.
 
-이 패키지를 바탕으로, **성서봇** 모바일 애플리케이션([Android](https://play.google.com/store/apps/details?id=com.blogspot.ramming125.kbubot&hl=ko) / [IOS](https://apps.apple.com/kr/app/성서봇/id1441276020))이 한국성서대학교학생들에게 2018년부터 실서비스 되고 있습니다.  
+이 패키지를 바탕으로, **성서봇** 모바일 애플리케이션([Android](https://play.google.com/store/apps/details?id=com.blogspot.ramming125.kbubot&hl=ko))이 한국성서대학교학생들에게 2018년부터 실서비스 되고 있습니다.
 
 이 패키지는 다섯 가지 웹사이트에 대한 스크래이퍼를 제공합니다.
 
 1. [한국성서대학교 인트라넷](https://kbuis.bible.ac.kr/) 스크래이퍼  
 2. [한국성서대학교 LMS](https://lms.bible.ac.kr/) 스크래이퍼
 3. [한국성서대학교 홈페이지](https://www.bible.ac.kr/) 스크래이퍼  
 4. [OKPOS 마일리지 시스템](https://asp.netusys.com/) 스크래이퍼
```

#### html2text {}

```diff
@@ -1,24 +1,23 @@
-Metadata-Version: 2.1 Name: biblebot Version: 0.4.1 Summary: Scraper for KBU
+Metadata-Version: 2.1 Name: biblebot Version: 0.4.2 Summary: Scraper for KBU
 students Home-page: https://github.com/rekyungmin/biblebot-scraper Author:
 Kyungmin Lee Author-email: rekyungmin@gmail.com Maintainer: Kyungmin Lee
 gmail.com>, Yongki Kim
 likelion.org> License: UNKNOWN Platform: UNKNOWN Classifier: License :: OSI
 Approved :: MIT License Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.7 Requires-Python:
 >=3.7 Description-Content-Type: text/markdown Provides-Extra: http License-
 File: LICENSE
                         ****** Biblebot Scraper ******
                          [Python] [Code_style:_black]
 ì±ìë´ ì¤í¬ëì´í¼ë íêµ­ì±ìëíêµì ì°ê´ë ì ë³´ë¥¼
 ìì§í  ì ìë íì´ì¬ í¨í¤ì§ìëë¤. ì´ í¨í¤ì§ë¥¼
 ë°íì¼ë¡, **ì±ìë´** ëª¨ë°ì¼ ì íë¦¬ì¼ì´ì([Android](https://
-play.google.com/store/apps/details?id=com.blogspot.ramming125.kbubot&hl=ko) /
-[IOS](https://apps.apple.com/kr/app/ì±ìë´/id1441276020))ì´
+play.google.com/store/apps/details?id=com.blogspot.ramming125.kbubot&hl=ko))ì´
 íêµ­ì±ìëíêµíìë¤ìê² 2018ëë¶í° ì¤ìë¹ì¤ ëê³ 
 ììµëë¤. ì´ í¨í¤ì§ë ë¤ì¯ ê°ì§ ì¹ì¬ì´í¸ì ëí
 ì¤í¬ëì´í¼ë¥¼ ì ê³µí©ëë¤. 1. [íêµ­ì±ìëíêµ ì¸í¸ë¼ë·]
 (https://kbuis.bible.ac.kr/) ì¤í¬ëì´í¼ 2. [íêµ­ì±ìëíêµ LMS]
 (https://lms.bible.ac.kr/) ì¤í¬ëì´í¼ 3. [íêµ­ì±ìëíêµ
 ííì´ì§](https://www.bible.ac.kr/) ì¤í¬ëì´í¼ 4. [OKPOS ë§ì¼ë¦¬ì§
 ìì¤í](https://asp.netusys.com/) ì¤í¬ëì´í¼ 5. [íêµ­ì±ìëíêµ
```

### Comparing `biblebot-0.4.1/biblebot.egg-info/SOURCES.txt` & `biblebot-0.4.2/biblebot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biblebot-0.4.1/setup.py` & `biblebot-0.4.2/setup.py`

 * *Files identical despite different names*

