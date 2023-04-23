# Comparing `tmp/Aciembler-1.0.0-py2.py3-none-any.whl.zip` & `tmp/Aciembler-1.0.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,8 @@
-Zip file size: 2107 bytes, number of entries: 5
--rwxr-xr-x  2.0 unx     1091 b- defN 23-Apr-23 06:28 Aciembler-1.0.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      641 b- defN 23-Apr-23 06:28 Aciembler-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Apr-23 06:28 Aciembler-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-23 06:28 Aciembler-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      399 b- defN 23-Apr-23 06:28 Aciembler-1.0.0.dist-info/RECORD
-5 files, 2242 bytes uncompressed, 1359 bytes compressed:  39.4%
+Zip file size: 10025 bytes, number of entries: 6
+-rw-r--r--  2.0 unx    10686 b- defN 23-Apr-23 05:03 Aciembler-1.0.1.data/data/System file/Template.xlsx
+-rwxr-xr-x  2.0 unx     1091 b- defN 23-Apr-23 06:49 Aciembler-1.0.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      736 b- defN 23-Apr-23 06:49 Aciembler-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Apr-23 06:49 Aciembler-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-23 06:49 Aciembler-1.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      508 b- defN 23-Apr-23 06:49 Aciembler-1.0.1.dist-info/RECORD
+6 files, 13132 bytes uncompressed, 9099 bytes compressed:  30.7%
```

## zipnote {}

```diff
@@ -1,16 +1,19 @@
-Filename: Aciembler-1.0.0.dist-info/LICENSE.txt
+Filename: Aciembler-1.0.1.data/data/System file/Template.xlsx
 Comment: 
 
-Filename: Aciembler-1.0.0.dist-info/METADATA
+Filename: Aciembler-1.0.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: Aciembler-1.0.0.dist-info/WHEEL
+Filename: Aciembler-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: Aciembler-1.0.0.dist-info/top_level.txt
+Filename: Aciembler-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: Aciembler-1.0.0.dist-info/RECORD
+Filename: Aciembler-1.0.1.dist-info/top_level.txt
+Comment: 
+
+Filename: Aciembler-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `Aciembler-1.0.0.dist-info/LICENSE.txt` & `Aciembler-1.0.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `Aciembler-1.0.0.dist-info/METADATA` & `Aciembler-1.0.1.dist-info/METADATA`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: Aciembler
-Version: 1.0.0
+Version: 1.0.1
 Summary: A CAIE 9618 assembler
 Author: hhaolin, AY
 Author-email: 2813579566@qq.com, Andrewsly@163.com
 License: MIT
 Keywords: CAIE,9618,Assembler
-Platform: Windows
-Platform: MacOS
+Platform: all
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
+Requires: HHLtools
+Requires: tabulate
 License-File: LICENSE.txt
 
 Aciembler-preter
 --------------------------
 2023/4/23:
     | 1.0.0 alpha testing
+    | 1.0.1 alpha testing
```

