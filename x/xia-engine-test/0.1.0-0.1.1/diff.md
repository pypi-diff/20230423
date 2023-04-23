# Comparing `tmp/xia_engine_test-0.1.0-cp39-none-win_amd64.whl.zip` & `tmp/xia_engine_test-0.1.1-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 328239 bytes, number of entries: 9
--rw-r--r--  2.0 unx      308 b- defN 23-Mar-30 15:58 xia_engine_test/__init__.py
--rw-r--r--  2.0 unx   288768 b- defN 23-Mar-30 16:00 xia_engine_test/document_example.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   281600 b- defN 23-Mar-30 16:01 xia_engine_test/field_test.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   244224 b- defN 23-Mar-30 16:02 xia_engine_test/models.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      155 b- defN 23-Mar-30 16:02 xia_engine_test-0.1.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      853 b- defN 23-Mar-30 16:02 xia_engine_test-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Mar-30 16:02 xia_engine_test-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Mar-30 16:02 xia_engine_test-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      825 b- defN 23-Mar-30 16:02 xia_engine_test-0.1.0.dist-info/RECORD
-9 files, 816848 bytes uncompressed, 326799 bytes compressed:  60.0%
+Zip file size: 326576 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      308 b- defN 23-Apr-23 09:11 xia_engine_test/__init__.py
+-rw-r--r--  2.0 unx   281088 b- defN 23-Apr-23 09:13 xia_engine_test/document_example.cp39-win_amd64.pyd
+-rw-r--r--  2.0 unx   281600 b- defN 23-Apr-23 09:14 xia_engine_test/field_test.cp39-win_amd64.pyd
+-rw-r--r--  2.0 unx   244224 b- defN 23-Apr-23 09:15 xia_engine_test/models.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-23 09:15 xia_engine_test-0.1.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      853 b- defN 23-Apr-23 09:15 xia_engine_test-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Apr-23 09:15 xia_engine_test-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Apr-23 09:15 xia_engine_test-0.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      825 b- defN 23-Apr-23 09:15 xia_engine_test-0.1.1.dist-info/RECORD
+9 files, 809165 bytes uncompressed, 325136 bytes compressed:  59.8%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: xia_engine_test/field_test.cp39-win_amd64.pyd
 Comment: 
 
 Filename: xia_engine_test/models.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_engine_test-0.1.0.dist-info/LICENSE.txt
+Filename: xia_engine_test-0.1.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_engine_test-0.1.0.dist-info/METADATA
+Filename: xia_engine_test-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: xia_engine_test-0.1.0.dist-info/WHEEL
+Filename: xia_engine_test-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: xia_engine_test-0.1.0.dist-info/top_level.txt
+Filename: xia_engine_test-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_engine_test-0.1.0.dist-info/RECORD
+Filename: xia_engine_test-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_engine_test/__init__.py

```diff
@@ -5,8 +5,8 @@
 __all__ = [
     "FieldTest",
     "MessageHello", "DocumentSimple", "External",
     "DocumentBasic"
 ]
 
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
```

## Comparing `xia_engine_test-0.1.0.dist-info/METADATA` & `xia_engine_test-0.1.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-engine-test
-Version: 0.1.0
+Version: 0.1.1
 Summary: X-I-A Engine Test Suite
-Home-page: https://develop.x-i-a.com/docs/xia-engine-test/0.1.0/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-engine-test/0.1.1/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_engine_test-0.1.0.dist-info/RECORD` & `xia_engine_test-0.1.1.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-xia_engine_test/__init__.py,sha256=BILtJkMnvaO-O-ZcJsB_2r8zr8z4togKMXRX9WmxHTE,308
-xia_engine_test/document_example.cp39-win_amd64.pyd,sha256=sUw3Cq-n4XW7vLThZz0C_mCMpI7raGdJ2SGBgVhv3P0,288768
-xia_engine_test/field_test.cp39-win_amd64.pyd,sha256=l0eykvBIS_QInnE-2_V20Nq75_BVqmksX2TyJtpyHqk,281600
-xia_engine_test/models.cp39-win_amd64.pyd,sha256=oysUlLqS0AnMoi5u3HAWTsnI1v2p_-ESrZvYQN1Lies,244224
-xia_engine_test-0.1.0.dist-info/LICENSE.txt,sha256=pw407CzwY_qOj6j4RHFf5AEhkOYzrtNAO05GOq0_me4,155
-xia_engine_test-0.1.0.dist-info/METADATA,sha256=Vpqih4aXsRa87G1vfNEUixXPkMgXXPUEcgBnQQ96qyE,853
-xia_engine_test-0.1.0.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
-xia_engine_test-0.1.0.dist-info/top_level.txt,sha256=lNzim7ax9-cnURpBE9M4WcBlHouRrTJJeqeGcQEemxE,16
-xia_engine_test-0.1.0.dist-info/RECORD,,
+xia_engine_test/__init__.py,sha256=pS2l6yxRfi-ChkPwiMMkrU4ekBaP9CVbcft0e-bd9xQ,308
+xia_engine_test/document_example.cp39-win_amd64.pyd,sha256=x1r1_nDrj8vixnT0Idk4ngOIYLgurYFJ2-3UG630VsM,281088
+xia_engine_test/field_test.cp39-win_amd64.pyd,sha256=AwJwqikLROV8DTQfL_MtN0oSl9s4_tG_k-IohZCoxGc,281600
+xia_engine_test/models.cp39-win_amd64.pyd,sha256=4OmiDwah2rGaSVevn8vPLMvBbfhWcs6jCPrCF8YQEC4,244224
+xia_engine_test-0.1.1.dist-info/LICENSE.txt,sha256=30wWxpufZqbxK7WdwZRoX8iA_veQA4gbl5oih3j5vFs,152
+xia_engine_test-0.1.1.dist-info/METADATA,sha256=f6FgmRFhhDybnaiTthE5xxcjQ9jzOHq2GMHXCimA7KE,853
+xia_engine_test-0.1.1.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
+xia_engine_test-0.1.1.dist-info/top_level.txt,sha256=lNzim7ax9-cnURpBE9M4WcBlHouRrTJJeqeGcQEemxE,16
+xia_engine_test-0.1.1.dist-info/RECORD,,
```

