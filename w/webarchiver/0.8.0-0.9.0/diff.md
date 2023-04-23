# Comparing `tmp/webarchiver-0.8.0-py2.py3-none-any.whl.zip` & `tmp/webarchiver-0.9.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 5912079 bytes, number of entries: 11
+Zip file size: 5912092 bytes, number of entries: 11
 -rw-r--r--  2.0 unx      296 b- defN 23-Apr-23 06:10 webarchiver/__init__.py
--rw-r--r--  2.0 unx      116 b- defN 23-Apr-23 06:10 webarchiver/version.py
--rw-r--r--  2.0 unx    39135 b- defN 23-Apr-23 06:10 webarchiver/webarchiver.py
+-rw-r--r--  2.0 unx      116 b- defN 23-Apr-23 06:16 webarchiver/version.py
+-rw-r--r--  2.0 unx    39148 b- defN 23-Apr-23 06:16 webarchiver/webarchiver.py
 -rw-r--r--  2.0 unx  2984341 b- defN 23-Apr-23 06:10 webarchiver/lib/uBlock-Origin_v1.27.0.crx
--rw-r--r--  2.0 unx  2984341 b- defN 23-Apr-23 06:10 webarchiver-0.8.0.data/data/webarchiver/uBlock-Origin_v1.27.0.crx
--rw-r--r--  2.0 unx     1211 b- defN 23-Apr-23 06:10 webarchiver-0.8.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     3295 b- defN 23-Apr-23 06:10 webarchiver-0.8.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Apr-23 06:10 webarchiver-0.8.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       62 b- defN 23-Apr-23 06:10 webarchiver-0.8.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 23-Apr-23 06:10 webarchiver-0.8.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      973 b- defN 23-Apr-23 06:10 webarchiver-0.8.0.dist-info/RECORD
-11 files, 6013892 bytes uncompressed, 5910421 bytes compressed:  1.7%
+-rw-r--r--  2.0 unx  2984341 b- defN 23-Apr-23 06:10 webarchiver-0.9.0.data/data/webarchiver/uBlock-Origin_v1.27.0.crx
+-rw-r--r--  2.0 unx     1211 b- defN 23-Apr-23 06:16 webarchiver-0.9.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3306 b- defN 23-Apr-23 06:16 webarchiver-0.9.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Apr-23 06:16 webarchiver-0.9.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       62 b- defN 23-Apr-23 06:16 webarchiver-0.9.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 23-Apr-23 06:16 webarchiver-0.9.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      973 b- defN 23-Apr-23 06:16 webarchiver-0.9.0.dist-info/RECORD
+11 files, 6013916 bytes uncompressed, 5910434 bytes compressed:  1.7%
```

## zipnote {}

```diff
@@ -6,29 +6,29 @@
 
 Filename: webarchiver/webarchiver.py
 Comment: 
 
 Filename: webarchiver/lib/uBlock-Origin_v1.27.0.crx
 Comment: 
 
-Filename: webarchiver-0.8.0.data/data/webarchiver/uBlock-Origin_v1.27.0.crx
+Filename: webarchiver-0.9.0.data/data/webarchiver/uBlock-Origin_v1.27.0.crx
 Comment: 
 
-Filename: webarchiver-0.8.0.dist-info/LICENSE
+Filename: webarchiver-0.9.0.dist-info/LICENSE
 Comment: 
 
-Filename: webarchiver-0.8.0.dist-info/METADATA
+Filename: webarchiver-0.9.0.dist-info/METADATA
 Comment: 
 
-Filename: webarchiver-0.8.0.dist-info/WHEEL
+Filename: webarchiver-0.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: webarchiver-0.8.0.dist-info/entry_points.txt
+Filename: webarchiver-0.9.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: webarchiver-0.8.0.dist-info/top_level.txt
+Filename: webarchiver-0.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: webarchiver-0.8.0.dist-info/RECORD
+Filename: webarchiver-0.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## webarchiver/version.py

```diff
@@ -1,6 +1,6 @@
 #!/usr/bin/env python
 # coding: utf-8
 
-__version__ = '0.8.0'
+__version__ = '0.9.0'
 __author__ = 'Audel Rouhi'
 __credits__ = 'Audel Rouhi'
```

## webarchiver/webarchiver.py

```diff
@@ -825,15 +825,16 @@
           f'-l | --links      [ Comma separated URLs (No spaces) ]\n'
           f'-i | --image-type [ Save images as PNG or JPEG ]\n'
           f'-t | --threads    [ Number of threads to run scrape and download ]\n'
           f'-u | --url-filter [ Only filter for specific files that contain this string ]\n'
           f'-z | --zoom       [ The zoom to use on the browser ]\n'
           f'\n'
           f'webarchiver -c -f <links_file.txt> '
-          '-l "<URL1, URL2, URL3>" -t <JPEG/PNG> -d "~/Downloads" -z 100 --dpi 1 --browser "Chrome" --executor "selenoid|http://selenoid.com/wd/hub"\n')
+          '-l "<URL1, URL2, URL3>" -i <JPEG/PNG> -d "~/Downloads" -z 100 --dpi 1 --browser "Chrome" '
+          '--executor "selenoid|http://selenoid.com/wd/hub"\n')
 
 
 def main():
     if len(sys.argv) < 2:
         usage()
         sys.exit(2)
     webarchiver(sys.argv[1:])
```

## Comparing `webarchiver-0.8.0.data/data/webarchiver/uBlock-Origin_v1.27.0.crx` & `webarchiver-0.9.0.data/data/webarchiver/uBlock-Origin_v1.27.0.crx`

 * *Files identical despite different names*

## Comparing `webarchiver-0.8.0.dist-info/LICENSE` & `webarchiver-0.9.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `webarchiver-0.8.0.dist-info/METADATA` & `webarchiver-0.9.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webarchiver
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python tool that allows you to take multiple full page screenshots of web pages without ads.
 Home-page: https://github.com/Knuckles-Team/webarchiver
 Author: Audel Rouhi
 Author-email: knucklessg1@gmail.com
 License: Unlicense
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,15 +20,15 @@
 Requires-Dist: Pillow (>=9.3.0)
 Requires-Dist: beautifulsoup4 (>=4.11.2)
 Requires-Dist: piexif (>=1.1.3)
 Requires-Dist: selenium (>=4.7.2)
 Requires-Dist: webdriver-manager (>=3.8.5)
 
 # Webarchiver
-*Version: 0.8.0*
+*Version: 0.9.0*
 
 Python tool that allows you to take full page screenshots of pages without ads
 
 Supports batching by adding multiple links in a text file, or my adding links to command line separated by commas.
 
 ### Requirements:
 
@@ -53,19 +53,19 @@
 | -t         | --threads    | Number of threads to run concurrently                       |
 | -u         | --url-filter | Filter URLs that contain this string                        |
 | -z         | --zoom       | The zoom to use on the browser                              |
 
 
 ### Example:
 ```bash
-webarchiver -c -f <links_file.txt> -l "<URL1,URL2,URL3>" -t <JPEG/PNG> -d "~/Downloads" -z 100 --dpi 1
+webarchiver -c -f <links_file.txt> -l "<URL1,URL2,URL3>" -i 'jpeg' -d "~/Downloads" -z 100 --dpi 1 --browser "Firefox"
 ```
 
 ```bash
-webarchiver -c -f <links_file.txt> -l "<URL1,URL2,URL3>" -t <JPEG/PNG> -d "~/Downloads" -z 100 --dpi 1 --executor "selenoid|http://selenoid.com/wd/hub" --browser "Chrome"
+webarchiver -c -f <links_file.txt> -l "<URL1,URL2,URL3>" -i 'png' -d "~/Downloads" -z 100 --dpi 1 --executor "selenoid|http://selenoid.com/wd/hub" --browser "Chrome"
 ```
 
 #### Install Instructions
 Install Python Package
 
 ```bash
 python -m pip install webarchiver
```

