# Comparing `tmp/xia_api_flask-0.1.8-cp39-none-win_amd64.whl.zip` & `tmp/xia_api_flask-0.1.9-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 171983 bytes, number of entries: 7
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-13 07:56 xia_api_flask/__init__.py
--rw-r--r--  2.0 unx   450560 b- defN 23-Apr-13 07:59 xia_api_flask/rest.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-13 07:59 xia_api_flask-0.1.8.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      737 b- defN 23-Apr-13 07:59 xia_api_flask-0.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Apr-13 07:59 xia_api_flask-0.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-Apr-13 07:59 xia_api_flask-0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      594 b- defN 23-Apr-13 07:59 xia_api_flask-0.1.8.dist-info/RECORD
-7 files, 452248 bytes uncompressed, 170919 bytes compressed:  62.2%
+Zip file size: 172383 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-14 20:50 xia_api_flask/__init__.py
+-rw-r--r--  2.0 unx   451072 b- defN 23-Apr-14 20:53 xia_api_flask/rest.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-14 20:53 xia_api_flask-0.1.9.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      737 b- defN 23-Apr-14 20:53 xia_api_flask-0.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Apr-14 20:53 xia_api_flask-0.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-Apr-14 20:53 xia_api_flask-0.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      594 b- defN 23-Apr-14 20:53 xia_api_flask-0.1.9.dist-info/RECORD
+7 files, 452760 bytes uncompressed, 171319 bytes compressed:  62.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_api_flask/__init__.py
 Comment: 
 
 Filename: xia_api_flask/rest.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_api_flask-0.1.8.dist-info/LICENSE.txt
+Filename: xia_api_flask-0.1.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_api_flask-0.1.8.dist-info/METADATA
+Filename: xia_api_flask-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: xia_api_flask-0.1.8.dist-info/WHEEL
+Filename: xia_api_flask-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: xia_api_flask-0.1.8.dist-info/top_level.txt
+Filename: xia_api_flask-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_api_flask-0.1.8.dist-info/RECORD
+Filename: xia_api_flask-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_api_flask/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_api_flask.rest import Restful
 
 __all__ = [
     "Restful",
 ]
 
-__version__ = "0.1.8"
+__version__ = "0.1.9"
```

## Comparing `xia_api_flask-0.1.8.dist-info/METADATA` & `xia_api_flask-0.1.9.dist-info/METADATA`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-api-flask
-Version: 0.1.8
+Version: 0.1.9
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-api-flask/0.1.8/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-api-flask/0.1.9/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

