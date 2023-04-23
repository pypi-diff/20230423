# Comparing `tmp/xia_engine_firestore-0.2.6-cp39-none-win_amd64.whl.zip` & `tmp/xia_engine_firestore-0.2.7-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
 Zip file size: 148576 bytes, number of entries: 7
--rw-r--r--  2.0 unx      117 b- defN 23-Mar-12 18:06 xia_engine_firestore/__init__.py
--rw-r--r--  2.0 unx   370688 b- defN 23-Mar-12 18:10 xia_engine_firestore/engine.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      152 b- defN 23-Mar-12 18:10 xia_engine_firestore-0.2.6.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      817 b- defN 23-Mar-12 18:10 xia_engine_firestore-0.2.6.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Mar-12 18:10 xia_engine_firestore-0.2.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       21 b- defN 23-Mar-12 18:10 xia_engine_firestore-0.2.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      646 b- defN 23-Mar-12 18:10 xia_engine_firestore-0.2.6.dist-info/RECORD
+-rw-r--r--  2.0 unx      117 b- defN 23-Apr-23 08:36 xia_engine_firestore/__init__.py
+-rw-r--r--  2.0 unx   370688 b- defN 23-Apr-23 08:39 xia_engine_firestore/engine.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-23 08:39 xia_engine_firestore-0.2.7.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      817 b- defN 23-Apr-23 08:39 xia_engine_firestore-0.2.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Apr-23 08:39 xia_engine_firestore-0.2.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       21 b- defN 23-Apr-23 08:39 xia_engine_firestore-0.2.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      646 b- defN 23-Apr-23 08:39 xia_engine_firestore-0.2.7.dist-info/RECORD
 7 files, 372540 bytes uncompressed, 147410 bytes compressed:  60.4%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_engine_firestore/__init__.py
 Comment: 
 
 Filename: xia_engine_firestore/engine.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_engine_firestore-0.2.6.dist-info/LICENSE.txt
+Filename: xia_engine_firestore-0.2.7.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_engine_firestore-0.2.6.dist-info/METADATA
+Filename: xia_engine_firestore-0.2.7.dist-info/METADATA
 Comment: 
 
-Filename: xia_engine_firestore-0.2.6.dist-info/WHEEL
+Filename: xia_engine_firestore-0.2.7.dist-info/WHEEL
 Comment: 
 
-Filename: xia_engine_firestore-0.2.6.dist-info/top_level.txt
+Filename: xia_engine_firestore-0.2.7.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_engine_firestore-0.2.6.dist-info/RECORD
+Filename: xia_engine_firestore-0.2.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_engine_firestore/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_engine_firestore.engine import FirestoreEngine
 
 
 __all__ = [
     "FirestoreEngine"
 ]
 
-__version__ = "0.2.6"
+__version__ = "0.2.7"
```

## Comparing `xia_engine_firestore-0.2.6.dist-info/METADATA` & `xia_engine_firestore-0.2.7.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-engine-firestore
-Version: 0.2.6
+Version: 0.2.7
 Summary: X-I-A Firestore Engine
-Home-page: https://develop.x-i-a.com/docs/xia-engine-firestore/0.2.6/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-engine-firestore/0.2.7/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_engine_firestore-0.2.6.dist-info/RECORD` & `xia_engine_firestore-0.2.7.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_engine_firestore/__init__.py,sha256=8oohS29aKrM4u2P7CwDE4MkMxF1zc3d0XQkn-qH9YOQ,117
-xia_engine_firestore/engine.cp39-win_amd64.pyd,sha256=uwdt4bxxEMUnGY2lBsWRYAgZSTbOFi29NTCD6xrG3_0,370688
-xia_engine_firestore-0.2.6.dist-info/LICENSE.txt,sha256=hxPR04Gu87DDUI5drgmeS7DmKKrZ3oegg3N-QQeTg8k,152
-xia_engine_firestore-0.2.6.dist-info/METADATA,sha256=1Ui-ZjqnqyKhgtG6M55hGpvfFCumOpq5dPeDy97lyFc,817
-xia_engine_firestore-0.2.6.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
-xia_engine_firestore-0.2.6.dist-info/top_level.txt,sha256=NUY0_anDQ8KVQ1TnPs_SCf-78KqRmu8_ARIL_J5agrg,21
-xia_engine_firestore-0.2.6.dist-info/RECORD,,
+xia_engine_firestore/__init__.py,sha256=vQATpFymIDBWWrblHRo9NRkTIhg6tFLK7ab5WXvca2U,117
+xia_engine_firestore/engine.cp39-win_amd64.pyd,sha256=29yOYrIrOqMzwpJGxkkk7-RoJkicSucIi_G8er2UKHI,370688
+xia_engine_firestore-0.2.7.dist-info/LICENSE.txt,sha256=30wWxpufZqbxK7WdwZRoX8iA_veQA4gbl5oih3j5vFs,152
+xia_engine_firestore-0.2.7.dist-info/METADATA,sha256=TAKwhRiu3QJiRgiYVcRgOvQZWOP9GKjGH90j9I2RQWc,817
+xia_engine_firestore-0.2.7.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
+xia_engine_firestore-0.2.7.dist-info/top_level.txt,sha256=NUY0_anDQ8KVQ1TnPs_SCf-78KqRmu8_ARIL_J5agrg,21
+xia_engine_firestore-0.2.7.dist-info/RECORD,,
```

