# Comparing `tmp/xia_api-0.1.8-cp39-none-win_amd64.whl.zip` & `tmp/xia_api-0.1.9-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 384746 bytes, number of entries: 9
--rw-r--r--  2.0 unx      497 b- defN 23-Apr-13 06:12 xia_api/__init__.py
--rw-r--r--  2.0 unx   240128 b- defN 23-Apr-13 06:32 xia_api/auth_client.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   286208 b- defN 23-Apr-13 06:33 xia_api/message.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   450560 b- defN 23-Apr-13 06:35 xia_api/rest.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-13 06:35 xia_api-0.1.8.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      675 b- defN 23-Apr-13 06:35 xia_api-0.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Apr-13 06:35 xia_api-0.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Apr-13 06:35 xia_api-0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      742 b- defN 23-Apr-13 06:35 xia_api-0.1.8.dist-info/RECORD
-9 files, 979069 bytes uncompressed, 383470 bytes compressed:  60.8%
+Zip file size: 384649 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      497 b- defN 23-Apr-13 07:37 xia_api/__init__.py
+-rw-r--r--  2.0 unx   240128 b- defN 23-Apr-13 07:39 xia_api/auth_client.cp39-win_amd64.pyd
+-rw-r--r--  2.0 unx   286208 b- defN 23-Apr-13 07:40 xia_api/message.cp39-win_amd64.pyd
+-rw-r--r--  2.0 unx   450560 b- defN 23-Apr-13 07:41 xia_api/rest.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-13 07:41 xia_api-0.1.9.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      675 b- defN 23-Apr-13 07:41 xia_api-0.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Apr-13 07:41 xia_api-0.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Apr-13 07:41 xia_api-0.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      742 b- defN 23-Apr-13 07:41 xia_api-0.1.9.dist-info/RECORD
+9 files, 979069 bytes uncompressed, 383373 bytes compressed:  60.8%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: xia_api/message.cp39-win_amd64.pyd
 Comment: 
 
 Filename: xia_api/rest.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_api-0.1.8.dist-info/LICENSE.txt
+Filename: xia_api-0.1.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_api-0.1.8.dist-info/METADATA
+Filename: xia_api-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: xia_api-0.1.8.dist-info/WHEEL
+Filename: xia_api-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: xia_api-0.1.8.dist-info/top_level.txt
+Filename: xia_api-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_api-0.1.8.dist-info/RECORD
+Filename: xia_api-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_api/__init__.py

```diff
@@ -7,8 +7,8 @@
 __all__ = [
     "AuthClient",
     "RestApi", "error_handle",
     "XiaCollectionDeleteMsg", "XiaDocumentDeleteMsg", "XiaFileMsg", "XiaRecordBook", "XiaRecordItem",
     "XiaErrorMessage", "XiaActionResult"
 ]
 
-__version__ = "0.1.8"
+__version__ = "0.1.9"
```

## Comparing `xia_api-0.1.8.dist-info/METADATA` & `xia_api-0.1.9.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-api
-Version: 0.1.8
+Version: 0.1.9
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-api/0.1.8/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-api/0.1.9/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_api-0.1.8.dist-info/RECORD` & `xia_api-0.1.9.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-xia_api/__init__.py,sha256=Eh5zQwf-aiX7B3oeL8FKA1WMqkRVIaWMWsDAhcjV48s,497
-xia_api/auth_client.cp39-win_amd64.pyd,sha256=cIhmMGGYkjeJkB04NP2StPxph5IhZGeIpL3fhdNtbLM,240128
-xia_api/message.cp39-win_amd64.pyd,sha256=tuFYYCdc9aF4RT8Rcwzp2iQVJEF-hW-5VvpgT_nQW6o,286208
-xia_api/rest.cp39-win_amd64.pyd,sha256=z854PpvDilfiwqbmw2n98fjN6OC98FcihiNosiRwjxU,450560
-xia_api-0.1.8.dist-info/LICENSE.txt,sha256=hxPR04Gu87DDUI5drgmeS7DmKKrZ3oegg3N-QQeTg8k,152
-xia_api-0.1.8.dist-info/METADATA,sha256=rUV2BuFXokonFsUGaleSKjfbsIQDMhJHjYCSiwiFRTM,675
-xia_api-0.1.8.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
-xia_api-0.1.8.dist-info/top_level.txt,sha256=krL7__RbzvbaNfgnuF-oCqAnr2y3Yy6whD8CBZyVXyw,8
-xia_api-0.1.8.dist-info/RECORD,,
+xia_api/__init__.py,sha256=RyIQu-c0TpLQiX48Vl2KM6yqQf8zFoYzsaVGufkFxzM,497
+xia_api/auth_client.cp39-win_amd64.pyd,sha256=u1K264MZK0krOwB9FXoVoYMdSDdQ3MqS6pHP_6-i0mk,240128
+xia_api/message.cp39-win_amd64.pyd,sha256=qQRGEcvYVj3jCJvpk89R5HpwKrIQ6CmLtTSUVoP8W9E,286208
+xia_api/rest.cp39-win_amd64.pyd,sha256=6vlO0w7i7-vqoUeHjCEyX_BHwuKfFtDiGiHsqCqzkoM,450560
+xia_api-0.1.9.dist-info/LICENSE.txt,sha256=hxPR04Gu87DDUI5drgmeS7DmKKrZ3oegg3N-QQeTg8k,152
+xia_api-0.1.9.dist-info/METADATA,sha256=dgPKMlIFA_AKE6eL8xxsFaMUOJbblvLs3fDVvK5PDxM,675
+xia_api-0.1.9.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
+xia_api-0.1.9.dist-info/top_level.txt,sha256=krL7__RbzvbaNfgnuF-oCqAnr2y3Yy6whD8CBZyVXyw,8
+xia_api-0.1.9.dist-info/RECORD,,
```

