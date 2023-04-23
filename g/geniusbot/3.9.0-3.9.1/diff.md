# Comparing `tmp/geniusbot-3.9.0-py2.py3-none-any.whl.zip` & `tmp/geniusbot-3.9.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 127867 bytes, number of entries: 13
+Zip file size: 127864 bytes, number of entries: 13
 -rw-r--r--  2.0 unx      268 b- defN 22-Dec-23 07:24 geniusbot/__init__.py
 -rw-r--r--  2.0 unx    74150 b- defN 22-Dec-23 08:32 geniusbot/geniusbot.py
 -rw-r--r--  2.0 unx     3150 b- defN 22-Dec-23 03:24 geniusbot/logger.py
--rw-r--r--  2.0 unx      116 b- defN 22-Dec-23 19:13 geniusbot/version.py
+-rw-r--r--  2.0 unx      116 b- defN 22-Dec-23 19:19 geniusbot/version.py
 -rwxr-xr-x  2.0 unx    67646 b- defN 22-Dec-23 03:24 geniusbot/img/geniusbot.ico
 -rwxr-xr-x  2.0 unx    43416 b- defN 22-Dec-23 03:24 geniusbot/img/geniusbot.png
--rwxr-xr-x  2.0 unx    67646 b- defN 22-Dec-23 03:24 geniusbot-3.9.0.data/data/geniusbot/geniusbot.ico
--rwxr-xr-x  2.0 unx    43416 b- defN 22-Dec-23 03:24 geniusbot-3.9.0.data/data/geniusbot/geniusbot.png
--rw-r--r--  2.0 unx     6409 b- defN 22-Dec-23 19:14 geniusbot-3.9.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 22-Dec-23 19:14 geniusbot-3.9.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       56 b- defN 22-Dec-23 19:14 geniusbot-3.9.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 22-Dec-23 19:14 geniusbot-3.9.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1097 b- defN 22-Dec-23 19:14 geniusbot-3.9.0.dist-info/RECORD
-13 files, 307490 bytes uncompressed, 126033 bytes compressed:  59.0%
+-rwxr-xr-x  2.0 unx    67646 b- defN 22-Dec-23 03:24 geniusbot-3.9.1.data/data/geniusbot/geniusbot.ico
+-rwxr-xr-x  2.0 unx    43416 b- defN 22-Dec-23 03:24 geniusbot-3.9.1.data/data/geniusbot/geniusbot.png
+-rw-r--r--  2.0 unx     6409 b- defN 22-Dec-23 19:19 geniusbot-3.9.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 22-Dec-23 19:19 geniusbot-3.9.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       56 b- defN 22-Dec-23 19:19 geniusbot-3.9.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 22-Dec-23 19:19 geniusbot-3.9.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1097 b- defN 22-Dec-23 19:19 geniusbot-3.9.1.dist-info/RECORD
+13 files, 307490 bytes uncompressed, 126030 bytes compressed:  59.0%
```

## zipnote {}

```diff
@@ -12,29 +12,29 @@
 
 Filename: geniusbot/img/geniusbot.ico
 Comment: 
 
 Filename: geniusbot/img/geniusbot.png
 Comment: 
 
-Filename: geniusbot-3.9.0.data/data/geniusbot/geniusbot.ico
+Filename: geniusbot-3.9.1.data/data/geniusbot/geniusbot.ico
 Comment: 
 
-Filename: geniusbot-3.9.0.data/data/geniusbot/geniusbot.png
+Filename: geniusbot-3.9.1.data/data/geniusbot/geniusbot.png
 Comment: 
 
-Filename: geniusbot-3.9.0.dist-info/METADATA
+Filename: geniusbot-3.9.1.dist-info/METADATA
 Comment: 
 
-Filename: geniusbot-3.9.0.dist-info/WHEEL
+Filename: geniusbot-3.9.1.dist-info/WHEEL
 Comment: 
 
-Filename: geniusbot-3.9.0.dist-info/entry_points.txt
+Filename: geniusbot-3.9.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: geniusbot-3.9.0.dist-info/top_level.txt
+Filename: geniusbot-3.9.1.dist-info/top_level.txt
 Comment: 
 
-Filename: geniusbot-3.9.0.dist-info/RECORD
+Filename: geniusbot-3.9.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## geniusbot/version.py

```diff
@@ -1,6 +1,6 @@
 #!/usr/bin/env python
 # coding: utf-8
 
-__version__ = '3.9.0'
+__version__ = '3.9.1'
 __author__ = 'Audel Rouhi'
 __credits__ = 'Audel Rouhi'
```

## Comparing `geniusbot-3.9.0.data/data/geniusbot/geniusbot.ico` & `geniusbot-3.9.1.data/data/geniusbot/geniusbot.ico`

 * *Files identical despite different names*

## Comparing `geniusbot-3.9.0.data/data/geniusbot/geniusbot.png` & `geniusbot-3.9.1.data/data/geniusbot/geniusbot.png`

 * *Files identical despite different names*

## Comparing `geniusbot-3.9.0.dist-info/METADATA` & `geniusbot-3.9.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geniusbot
-Version: 3.9.0
+Version: 3.9.1
 Summary: The Ever-learning and ever-improving tool!
 Home-page: https://github.com/Knuckles-Team/geniusbot
 Author: Audel Rouhi
 Author-email: knucklessg1@gmail.com
 License: Unlicensed
 Keywords: genius,geniusbot,download,video,subtitle,website,screenshot,media,manage,chatbot,report,profiling,merge
 Platform: UNKNOWN
@@ -26,15 +26,15 @@
 Requires-Dist: subshift (>=0.7.0)
 Requires-Dist: systems-manager (>=0.3.0)
 Requires-Dist: webarchiver (>=0.5.0)
 Requires-Dist: pypiwin32 ; platform_system == "Windows"
 Requires-Dist: winshell (>=0.6) ; platform_system == "Windows"
 
 # Geniusbot 
-*Version: 3.9.0*
+*Version: 3.9.1*
 
 ![Geniusbot](https://raw.githubusercontent.com/Knucklessg1/geniusbot/master/geniusbot/img/geniusbot-small.png "Geniusbot") 
 
 The Ever-learning and ever-improving tool!
 
 Click the arrows on the left of each of the items below to see more information about them.
```

## Comparing `geniusbot-3.9.0.dist-info/RECORD` & `geniusbot-3.9.1.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 geniusbot/__init__.py,sha256=c1vTpQ28rblFxxvGBef4Y7k73CLjEJ8EB74NI7pzgSI,268
 geniusbot/geniusbot.py,sha256=nwrADwjMLBKHVDjEoTx_IvZ_7jj4YrP9RFjVPrSC4tQ,74150
 geniusbot/logger.py,sha256=fjYSTx7WxRPum0Jt8sbFbqSyvWq7SR5RumGzGR7xuYo,3150
-geniusbot/version.py,sha256=h3y5Cv4QztBtObyPKiOJUL0kx4wv6Qw4Gupn3Y4WCbI,116
+geniusbot/version.py,sha256=PODoG_lAfaZSw83wtlqlXSJphP8IS-Or_MldiYyyJY8,116
 geniusbot/img/geniusbot.ico,sha256=lPHlX5iI6-xUF-Ewr40Kg7ZOIX3_WvHaFX_Yl6tlY5g,67646
 geniusbot/img/geniusbot.png,sha256=1KYCHopRoNqMHwHRBgkcLF_xqC8hSKlhkTKqsIbhZRQ,43416
-geniusbot-3.9.0.data/data/geniusbot/geniusbot.ico,sha256=lPHlX5iI6-xUF-Ewr40Kg7ZOIX3_WvHaFX_Yl6tlY5g,67646
-geniusbot-3.9.0.data/data/geniusbot/geniusbot.png,sha256=1KYCHopRoNqMHwHRBgkcLF_xqC8hSKlhkTKqsIbhZRQ,43416
-geniusbot-3.9.0.dist-info/METADATA,sha256=2YUkvvW8mrqvIPHUvY8s7tdKNkpTMFIOz6EGHDVqKaQ,6409
-geniusbot-3.9.0.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
-geniusbot-3.9.0.dist-info/entry_points.txt,sha256=up_Yx2Mw3sjfCvz8FQBEfvcViJrpoT_gMXdV_lU5Zak,56
-geniusbot-3.9.0.dist-info/top_level.txt,sha256=x1L29i9WrbOlWSxPuBTKVXU3VQReT8NnSNW3xjB4PfE,10
-geniusbot-3.9.0.dist-info/RECORD,,
+geniusbot-3.9.1.data/data/geniusbot/geniusbot.ico,sha256=lPHlX5iI6-xUF-Ewr40Kg7ZOIX3_WvHaFX_Yl6tlY5g,67646
+geniusbot-3.9.1.data/data/geniusbot/geniusbot.png,sha256=1KYCHopRoNqMHwHRBgkcLF_xqC8hSKlhkTKqsIbhZRQ,43416
+geniusbot-3.9.1.dist-info/METADATA,sha256=3NC6SJbsHc-uHcCQFwaRnvn0I8ksQl05HwzlePP4CsQ,6409
+geniusbot-3.9.1.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
+geniusbot-3.9.1.dist-info/entry_points.txt,sha256=up_Yx2Mw3sjfCvz8FQBEfvcViJrpoT_gMXdV_lU5Zak,56
+geniusbot-3.9.1.dist-info/top_level.txt,sha256=x1L29i9WrbOlWSxPuBTKVXU3VQReT8NnSNW3xjB4PfE,10
+geniusbot-3.9.1.dist-info/RECORD,,
```

