# Comparing `tmp/media_downloader-0.4.0-py2.py3-none-any.whl.zip` & `tmp/media_downloader-0.5.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 6158 bytes, number of entries: 9
+Zip file size: 6263 bytes, number of entries: 9
 -rw-r--r--  2.0 unx      348 b- defN 23-Apr-16 04:38 media_downloader/__init__.py
--rw-r--r--  2.0 unx     8954 b- defN 23-Apr-16 04:38 media_downloader/media_downloader.py
--rw-r--r--  2.0 unx      116 b- defN 23-Apr-16 04:38 media_downloader/version.py
--rw-r--r--  2.0 unx     1210 b- defN 23-Apr-16 04:38 media_downloader-0.4.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     2127 b- defN 23-Apr-16 04:38 media_downloader-0.4.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Apr-16 04:38 media_downloader-0.4.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       77 b- defN 23-Apr-16 04:38 media_downloader-0.4.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       17 b- defN 23-Apr-16 04:38 media_downloader-0.4.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      796 b- defN 23-Apr-16 04:38 media_downloader-0.4.0.dist-info/RECORD
-9 files, 13755 bytes uncompressed, 4764 bytes compressed:  65.4%
+-rw-r--r--  2.0 unx     9230 b- defN 23-Apr-23 19:24 media_downloader/media_downloader.py
+-rw-r--r--  2.0 unx      116 b- defN 23-Apr-23 19:24 media_downloader/version.py
+-rw-r--r--  2.0 unx     1210 b- defN 23-Apr-23 19:24 media_downloader-0.5.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2127 b- defN 23-Apr-23 19:24 media_downloader-0.5.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Apr-23 19:24 media_downloader-0.5.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       77 b- defN 23-Apr-23 19:24 media_downloader-0.5.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       17 b- defN 23-Apr-23 19:24 media_downloader-0.5.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      796 b- defN 23-Apr-23 19:24 media_downloader-0.5.0.dist-info/RECORD
+9 files, 14031 bytes uncompressed, 4869 bytes compressed:  65.3%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: media_downloader/media_downloader.py
 Comment: 
 
 Filename: media_downloader/version.py
 Comment: 
 
-Filename: media_downloader-0.4.0.dist-info/LICENSE
+Filename: media_downloader-0.5.0.dist-info/LICENSE
 Comment: 
 
-Filename: media_downloader-0.4.0.dist-info/METADATA
+Filename: media_downloader-0.5.0.dist-info/METADATA
 Comment: 
 
-Filename: media_downloader-0.4.0.dist-info/WHEEL
+Filename: media_downloader-0.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: media_downloader-0.4.0.dist-info/entry_points.txt
+Filename: media_downloader-0.5.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: media_downloader-0.4.0.dist-info/top_level.txt
+Filename: media_downloader-0.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: media_downloader-0.4.0.dist-info/RECORD
+Filename: media_downloader-0.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## media_downloader/media_downloader.py

```diff
@@ -4,14 +4,15 @@
 import os
 import sys
 import re
 import getopt
 import requests
 import yt_dlp
 from multiprocessing import Pool
+from media_downloader.version import __version__, __author__, __credits__
 
 
 class StdOutLogger(object):
     def debug(self, msg):
         print(f'{msg}')
 
     def warning(self, msg):
@@ -229,22 +230,26 @@
             for url in url_list:
                 video_downloader_instance.append_link(url)
 
     video_downloader_instance.download_all()
 
 
 def usage():
-    print(f'Usage:\n'
+    print(f'Media-Downloader: A tool to download any video off the internet!\n'
+          f'Version: {__version__}\n'
+          f'Author: {__author__}\n'
+          f'Credits: {__credits__}\n'
+          f'Usage:\n'
           f'-h | --help      [ See usage ]\n'
           f'-a | --audio     [ Download audio only ]\n'
           f'-c | --channel   [ YouTube Channel/User - Downloads all videos ]\n'
           f'-d | --directory [ Location where the images will be saved ]\n'
           f'-f | --file      [ Text file to read the URLs from ]\n'
           f'-l | --links     [ Comma separated URLs (No spaces) ]\n'
-          f'\n'
+          f'\nExample:\n'
           f'media-downloader -f "file_of_urls.txt" -l "URL1,URL2,URL3" -c "WhiteHouse" -d "~/Downloads"\n')
 
 
 def main():
     media_downloader(sys.argv[1:])
```

## media_downloader/version.py

```diff
@@ -1,6 +1,6 @@
 #!/usr/bin/env python
 # coding: utf-8
 
-__version__ = '0.4.0'
+__version__ = '0.5.0'
 __author__ = 'Audel Rouhi'
 __credits__ = 'Audel Rouhi'
```

## Comparing `media_downloader-0.4.0.dist-info/LICENSE` & `media_downloader-0.5.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `media_downloader-0.4.0.dist-info/METADATA` & `media_downloader-0.5.0.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: media-downloader
-Version: 0.4.0
+Version: 0.5.0
 Summary: Download audio/videos from the internet!
 Home-page: https://github.com/Knuckles-Team/media-downloader
 Author: Audel Rouhi
 Author-email: knucklessg1@gmail.com
 License: Unlicense
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests (>=2.28.1)
 Requires-Dist: yt-dlp (>=2023.3.4)
 
 # Media Downloader
-*Version: 0.4.0*
+*Version: 0.5.0*
 
 Download videos and audio from the internet!
 
 ### Supports:
 - YouTube
 - Twitter
 - Rumble
```

## Comparing `media_downloader-0.4.0.dist-info/RECORD` & `media_downloader-0.5.0.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 media_downloader/__init__.py,sha256=iCl7rzarsiHgt6a5R_A1aANqNfD5rhJi4Zvj8oQ47zo,348
-media_downloader/media_downloader.py,sha256=yIZcQXvgByLzf1fzAdPZi5DADE-Zrn6tSCD57sL1fOs,8954
-media_downloader/version.py,sha256=oG1CxokHsCjaBeI2nIqR2VaJkO1zY0M2gRb5qgvMB-k,116
-media_downloader-0.4.0.dist-info/LICENSE,sha256=yiq99pWITHfqS0pbZMp7cy2dnbreTuvBwudsU-njvIM,1210
-media_downloader-0.4.0.dist-info/METADATA,sha256=xdtyNTFkHBtpmWByk3HE5syi8l6v2LqXOUQTYB7htHI,2127
-media_downloader-0.4.0.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
-media_downloader-0.4.0.dist-info/entry_points.txt,sha256=ZYFDwE25i9D2Mc_ZkLbA0ASaUJo_IEOGDU2gXO7OQnE,77
-media_downloader-0.4.0.dist-info/top_level.txt,sha256=B2OBmgONOm0hIyx2HJ8qFPOI_p5HOeolrYvmslVC1fc,17
-media_downloader-0.4.0.dist-info/RECORD,,
+media_downloader/media_downloader.py,sha256=7ReDbvRTOKvNDAgGxFfStePjwup3_xWwjeghOmlBE2o,9230
+media_downloader/version.py,sha256=6IhjTbl3T306PyVy-FZE4rpQc3haUwFDchvvd4igGpw,116
+media_downloader-0.5.0.dist-info/LICENSE,sha256=yiq99pWITHfqS0pbZMp7cy2dnbreTuvBwudsU-njvIM,1210
+media_downloader-0.5.0.dist-info/METADATA,sha256=EJuC98B6XylXo19wKc40QTOIhh499lAjR5-1PtzO4Mg,2127
+media_downloader-0.5.0.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
+media_downloader-0.5.0.dist-info/entry_points.txt,sha256=ZYFDwE25i9D2Mc_ZkLbA0ASaUJo_IEOGDU2gXO7OQnE,77
+media_downloader-0.5.0.dist-info/top_level.txt,sha256=B2OBmgONOm0hIyx2HJ8qFPOI_p5HOeolrYvmslVC1fc,17
+media_downloader-0.5.0.dist-info/RECORD,,
```

