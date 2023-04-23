# Comparing `tmp/xia_compiler_openapi-0.1.1-cp39-none-win_amd64.whl.zip` & `tmp/xia_compiler_openapi-0.1.2-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 224127 bytes, number of entries: 7
--rw-r--r--  2.0 unx      126 b- defN 23-Feb-01 20:47 xia_compiler_openapi/__init__.py
--rw-r--r--  2.0 unx   622592 b- defN 23-Feb-01 20:50 xia_compiler_openapi/compiler.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      154 b- defN 23-Feb-01 20:50 xia_compiler_openapi-0.1.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      695 b- defN 23-Feb-01 20:50 xia_compiler_openapi-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Feb-01 20:50 xia_compiler_openapi-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       21 b- defN 23-Feb-01 20:50 xia_compiler_openapi-0.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      648 b- defN 23-Feb-01 20:50 xia_compiler_openapi-0.1.1.dist-info/RECORD
-7 files, 624335 bytes uncompressed, 222957 bytes compressed:  64.3%
+Zip file size: 222882 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      126 b- defN 23-Apr-23 11:49 xia_compiler_openapi/__init__.py
+-rw-r--r--  2.0 unx   620544 b- defN 23-Apr-23 11:56 xia_compiler_openapi/compiler.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-23 11:56 xia_compiler_openapi-0.1.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      695 b- defN 23-Apr-23 11:56 xia_compiler_openapi-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Apr-23 11:56 xia_compiler_openapi-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       21 b- defN 23-Apr-23 11:56 xia_compiler_openapi-0.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      648 b- defN 23-Apr-23 11:56 xia_compiler_openapi-0.1.2.dist-info/RECORD
+7 files, 622285 bytes uncompressed, 221712 bytes compressed:  64.4%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_compiler_openapi/__init__.py
 Comment: 
 
 Filename: xia_compiler_openapi/compiler.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_compiler_openapi-0.1.1.dist-info/LICENSE.txt
+Filename: xia_compiler_openapi-0.1.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_compiler_openapi-0.1.1.dist-info/METADATA
+Filename: xia_compiler_openapi-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: xia_compiler_openapi-0.1.1.dist-info/WHEEL
+Filename: xia_compiler_openapi-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: xia_compiler_openapi-0.1.1.dist-info/top_level.txt
+Filename: xia_compiler_openapi-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_compiler_openapi-0.1.1.dist-info/RECORD
+Filename: xia_compiler_openapi-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_compiler_openapi/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_compiler_openapi.compiler import XiaCompilerOpenapi
 
 
 __all__ = [
     "XiaCompilerOpenapi",
 ]
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
```

## Comparing `xia_compiler_openapi-0.1.1.dist-info/METADATA` & `xia_compiler_openapi-0.1.2.dist-info/METADATA`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-compiler-openapi
-Version: 0.1.1
+Version: 0.1.2
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-compiler-openapi/0.1.1/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-compiler-openapi/0.1.2/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_compiler_openapi-0.1.1.dist-info/RECORD` & `xia_compiler_openapi-0.1.2.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_compiler_openapi/__init__.py,sha256=N2Vo1mggQPOBQid8IueuSVsFl3GTjuNLBoI63B-zR5s,126
-xia_compiler_openapi/compiler.cp39-win_amd64.pyd,sha256=cYrD-3S-UD_eC59K7gJPVU3ztNy1JhfzKUVeh8irLEo,622592
-xia_compiler_openapi-0.1.1.dist-info/LICENSE.txt,sha256=h07omO2Zqb3EYhslHI3GGu_hZMl8fMEzlfVND-EtoYo,154
-xia_compiler_openapi-0.1.1.dist-info/METADATA,sha256=s2EdHvykLYsEBeq1gv9aA8TqI18g7ojQ7B73y4GErf0,695
-xia_compiler_openapi-0.1.1.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
-xia_compiler_openapi-0.1.1.dist-info/top_level.txt,sha256=l-dHwHri9HVBghJIDfyblbK8E8exERfi3dhMi7vW3bE,21
-xia_compiler_openapi-0.1.1.dist-info/RECORD,,
+xia_compiler_openapi/__init__.py,sha256=-dE50s7Ppx66LRhMtlDLJtVjeYwkH8Fzg-lsQ6kyTn0,126
+xia_compiler_openapi/compiler.cp39-win_amd64.pyd,sha256=PR9oDoY8i3F7DixUy3bG9eZfsDvmne7_IUfFLXJNdC0,620544
+xia_compiler_openapi-0.1.2.dist-info/LICENSE.txt,sha256=30wWxpufZqbxK7WdwZRoX8iA_veQA4gbl5oih3j5vFs,152
+xia_compiler_openapi-0.1.2.dist-info/METADATA,sha256=BF0bqAQUpYhayB1ThyWvbta2ttxNr7SmZTbD-rcUvqY,695
+xia_compiler_openapi-0.1.2.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
+xia_compiler_openapi-0.1.2.dist-info/top_level.txt,sha256=l-dHwHri9HVBghJIDfyblbK8E8exERfi3dhMi7vW3bE,21
+xia_compiler_openapi-0.1.2.dist-info/RECORD,,
```

