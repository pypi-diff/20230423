# Comparing `tmp/xia_compiler_jsoneditor-0.0.8-cp39-none-win_amd64.whl.zip` & `tmp/xia_compiler_jsoneditor-0.0.9-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 166936 bytes, number of entries: 7
--rw-r--r--  2.0 unx      135 b- defN 23-Jan-28 20:44 xia_compiler_jsoneditor/__init__.py
--rw-r--r--  2.0 unx   440320 b- defN 23-Jan-28 20:47 xia_compiler_jsoneditor/compiler.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      154 b- defN 23-Jan-28 20:47 xia_compiler_jsoneditor-0.0.8.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      687 b- defN 23-Jan-28 20:47 xia_compiler_jsoneditor-0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jan-28 20:47 xia_compiler_jsoneditor-0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       24 b- defN 23-Jan-28 20:47 xia_compiler_jsoneditor-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      669 b- defN 23-Jan-28 20:47 xia_compiler_jsoneditor-0.0.8.dist-info/RECORD
-7 files, 442088 bytes uncompressed, 165724 bytes compressed:  62.5%
+Zip file size: 167163 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      135 b- defN 23-Mar-30 19:50 xia_compiler_jsoneditor/__init__.py
+-rw-r--r--  2.0 unx   442368 b- defN 23-Mar-30 19:53 xia_compiler_jsoneditor/compiler.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      152 b- defN 23-Mar-30 19:53 xia_compiler_jsoneditor-0.0.9.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      687 b- defN 23-Mar-30 19:53 xia_compiler_jsoneditor-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Mar-30 19:53 xia_compiler_jsoneditor-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       24 b- defN 23-Mar-30 19:53 xia_compiler_jsoneditor-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      669 b- defN 23-Mar-30 19:53 xia_compiler_jsoneditor-0.0.9.dist-info/RECORD
+7 files, 444134 bytes uncompressed, 165951 bytes compressed:  62.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_compiler_jsoneditor/__init__.py
 Comment: 
 
 Filename: xia_compiler_jsoneditor/compiler.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_compiler_jsoneditor-0.0.8.dist-info/LICENSE.txt
+Filename: xia_compiler_jsoneditor-0.0.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_compiler_jsoneditor-0.0.8.dist-info/METADATA
+Filename: xia_compiler_jsoneditor-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: xia_compiler_jsoneditor-0.0.8.dist-info/WHEEL
+Filename: xia_compiler_jsoneditor-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: xia_compiler_jsoneditor-0.0.8.dist-info/top_level.txt
+Filename: xia_compiler_jsoneditor-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_compiler_jsoneditor-0.0.8.dist-info/RECORD
+Filename: xia_compiler_jsoneditor-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_compiler_jsoneditor/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_compiler_jsoneditor.compiler import XiaCompilerJsoneditor
 
 
 __all__ = [
     "XiaCompilerJsoneditor",
 ]
 
-__version__ = "0.0.8"
+__version__ = "0.0.9"
```

## Comparing `xia_compiler_jsoneditor-0.0.8.dist-info/METADATA` & `xia_compiler_jsoneditor-0.0.9.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-compiler-jsoneditor
-Version: 0.0.8
+Version: 0.0.9
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-compiler-jsoneditor/0.0.8/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-compiler-jsoneditor/0.0.9/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_compiler_jsoneditor-0.0.8.dist-info/RECORD` & `xia_compiler_jsoneditor-0.0.9.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_compiler_jsoneditor/__init__.py,sha256=9H4ExcnLN8hCAT_LN_8Yvk6b1iLBbkekeaj-r4g5-y4,135
-xia_compiler_jsoneditor/compiler.cp39-win_amd64.pyd,sha256=29k7fZsooxAJtzTPtqjgju6jA-w1ILvGSH4a62fyoqU,440320
-xia_compiler_jsoneditor-0.0.8.dist-info/LICENSE.txt,sha256=jaRldKlEH_J8aFHvBUd4JaDsBUUeckTThY0sZLOVZZ8,154
-xia_compiler_jsoneditor-0.0.8.dist-info/METADATA,sha256=LazIu6cBgfOaUTtXwdFJ0DmC537fIPIGw64EfkTtgqU,687
-xia_compiler_jsoneditor-0.0.8.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
-xia_compiler_jsoneditor-0.0.8.dist-info/top_level.txt,sha256=oY6KydARRKWB_3q2LeXeIeKJVyZ1d54IIkH9htejhKA,24
-xia_compiler_jsoneditor-0.0.8.dist-info/RECORD,,
+xia_compiler_jsoneditor/__init__.py,sha256=dLz-GHzknjgWl5WE4Gl5Qqv7LDMCKzO_rr82cZST9ZM,135
+xia_compiler_jsoneditor/compiler.cp39-win_amd64.pyd,sha256=_K9J2sZS7j4JjfHAgz5O-lm6hNXVY1OTTHyuhY51Ypg,442368
+xia_compiler_jsoneditor-0.0.9.dist-info/LICENSE.txt,sha256=hxPR04Gu87DDUI5drgmeS7DmKKrZ3oegg3N-QQeTg8k,152
+xia_compiler_jsoneditor-0.0.9.dist-info/METADATA,sha256=hBLUogY3Pa1mkhCQFye-w68MUtyhcd2FXWvo3xl6PVM,687
+xia_compiler_jsoneditor-0.0.9.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
+xia_compiler_jsoneditor-0.0.9.dist-info/top_level.txt,sha256=oY6KydARRKWB_3q2LeXeIeKJVyZ1d54IIkH9htejhKA,24
+xia_compiler_jsoneditor-0.0.9.dist-info/RECORD,,
```

