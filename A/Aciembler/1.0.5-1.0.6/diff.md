# Comparing `tmp/Aciembler-1.0.5-py2.py3-none-any.whl.zip` & `tmp/Aciembler-1.0.6-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,7 @@
-Zip file size: 10022 bytes, number of entries: 6
--rw-r--r--  2.0 unx    10686 b- defN 23-Apr-23 05:03 Aciembler-1.0.5.data/data/System file/Template.xlsx
--rwxr-xr-x  2.0 unx     1091 b- defN 23-Apr-23 07:29 Aciembler-1.0.5.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      685 b- defN 23-Apr-23 07:29 Aciembler-1.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Apr-23 07:29 Aciembler-1.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-23 07:29 Aciembler-1.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      508 b- defN 23-Apr-23 07:29 Aciembler-1.0.5.dist-info/RECORD
-6 files, 13081 bytes uncompressed, 9096 bytes compressed:  30.5%
+Zip file size: 2105 bytes, number of entries: 5
+-rwxr-xr-x  2.0 unx     1091 b- defN 23-Apr-23 07:32 Aciembler-1.0.6.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      647 b- defN 23-Apr-23 07:32 Aciembler-1.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Apr-23 07:32 Aciembler-1.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-23 07:32 Aciembler-1.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      399 b- defN 23-Apr-23 07:32 Aciembler-1.0.6.dist-info/RECORD
+5 files, 2248 bytes uncompressed, 1357 bytes compressed:  39.6%
```

## zipnote {}

```diff
@@ -1,19 +1,16 @@
-Filename: Aciembler-1.0.5.data/data/System file/Template.xlsx
+Filename: Aciembler-1.0.6.dist-info/LICENSE.txt
 Comment: 
 
-Filename: Aciembler-1.0.5.dist-info/LICENSE.txt
+Filename: Aciembler-1.0.6.dist-info/METADATA
 Comment: 
 
-Filename: Aciembler-1.0.5.dist-info/METADATA
+Filename: Aciembler-1.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: Aciembler-1.0.5.dist-info/WHEEL
+Filename: Aciembler-1.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: Aciembler-1.0.5.dist-info/top_level.txt
-Comment: 
-
-Filename: Aciembler-1.0.5.dist-info/RECORD
+Filename: Aciembler-1.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `Aciembler-1.0.5.dist-info/LICENSE.txt` & `Aciembler-1.0.6.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `Aciembler-1.0.5.dist-info/METADATA` & `Aciembler-1.0.6.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: Aciembler
-Version: 1.0.5
+Version: 1.0.6
 Summary: A CAIE 9618 assembler
 Author: hhaolin, AY
 Author-email: 2813579566@qq.com, Andrewsly@163.com
 License: MIT
 Keywords: CAIE,9618,Assembler
 Platform: all
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
-Requires: HHLtools
-Requires: tabulate
 License-File: LICENSE.txt
 
 Aciembler-preter
 --------------------------
 2023/4/23:
     | 1.0.0 alpha testing
     | 1.0.1 alpha testing
```

