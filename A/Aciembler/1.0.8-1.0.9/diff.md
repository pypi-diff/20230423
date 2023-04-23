# Comparing `tmp/Aciembler-1.0.8-py2.py3-none-any.whl.zip` & `tmp/Aciembler-1.0.9-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,14 @@
-Zip file size: 15502 bytes, number of entries: 13
--rw-r--r--  2.0 unx     3178 b- defN 23-Apr-23 07:54 Aciembler/Aciembler.py
+Zip file size: 15387 bytes, number of entries: 12
+-rw-r--r--  2.0 unx     3213 b- defN 23-Apr-23 08:27 Aciembler/Aciembler.py
 -rw-r--r--  2.0 unx      749 b- defN 23-Apr-23 05:17 Aciembler/Error.py
 -rw-r--r--  2.0 unx     3421 b- defN 23-Apr-23 07:15 Aciembler/First_pass.py
 -rw-r--r--  2.0 unx      712 b- defN 23-Apr-23 06:11 Aciembler/__init__.py
 -rw-r--r--  2.0 unx      506 b- defN 23-Apr-23 05:41 Aciembler/objectCode.py
 -rw-r--r--  2.0 unx    10544 b- defN 23-Apr-23 06:13 Aciembler/translator.py
--rw-r--r--  2.0 unx    10686 b- defN 23-Apr-23 05:03 data/Template.xlsx
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-23 07:55 data/__init__.py
--rwxr-xr-x  2.0 unx     1091 b- defN 23-Apr-23 08:00 Aciembler-1.0.8.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      685 b- defN 23-Apr-23 08:00 Aciembler-1.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Apr-23 08:00 Aciembler-1.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-Apr-23 08:00 Aciembler-1.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1016 b- defN 23-Apr-23 08:00 Aciembler-1.0.8.dist-info/RECORD
-13 files, 32713 bytes uncompressed, 13818 bytes compressed:  57.8%
+-rw-r--r--  2.0 unx    10686 b- defN 23-Apr-23 05:03 Aciembler/data/Template.xlsx
+-rwxr-xr-x  2.0 unx     1091 b- defN 23-Apr-23 08:31 Aciembler-1.0.9.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      701 b- defN 23-Apr-23 08:31 Aciembler-1.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Apr-23 08:31 Aciembler-1.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Apr-23 08:31 Aciembler-1.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      956 b- defN 23-Apr-23 08:31 Aciembler-1.0.9.dist-info/RECORD
+12 files, 32699 bytes uncompressed, 13791 bytes compressed:  57.8%
```

## zipnote {}

```diff
@@ -12,29 +12,26 @@
 
 Filename: Aciembler/objectCode.py
 Comment: 
 
 Filename: Aciembler/translator.py
 Comment: 
 
-Filename: data/Template.xlsx
+Filename: Aciembler/data/Template.xlsx
 Comment: 
 
-Filename: data/__init__.py
+Filename: Aciembler-1.0.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: Aciembler-1.0.8.dist-info/LICENSE.txt
+Filename: Aciembler-1.0.9.dist-info/METADATA
 Comment: 
 
-Filename: Aciembler-1.0.8.dist-info/METADATA
+Filename: Aciembler-1.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: Aciembler-1.0.8.dist-info/WHEEL
+Filename: Aciembler-1.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: Aciembler-1.0.8.dist-info/top_level.txt
-Comment: 
-
-Filename: Aciembler-1.0.8.dist-info/RECORD
+Filename: Aciembler-1.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Aciembler/Aciembler.py

```diff
@@ -8,20 +8,21 @@
 from tkinter import filedialog
 import random
 import platform
 
 
 
 
+
 def new_file():
-    base = os.getcwd()
+    base = os.path.dirname(os.path.abspath(__file__))
     while ((path := filedialog.asksaveasfilename(defaultextension='.xlsx')) == ''):
         pass
     try:
-        shutil.copy('../data/Template.xlsx', path)
+        shutil.copy(base+'/data/Template.xlsx', path)
         edit_file(path)
     except Exception as e:
         print(e)
 
 
 def edit_file(path=''):
     if path != '':
```

## Comparing `data/Template.xlsx` & `Aciembler/data/Template.xlsx`

 * *Files identical despite different names*

## Comparing `Aciembler-1.0.8.dist-info/LICENSE.txt` & `Aciembler-1.0.9.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `Aciembler-1.0.8.dist-info/METADATA` & `Aciembler-1.0.9.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: Aciembler
-Version: 1.0.8
+Version: 1.0.9
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
 Requires: HHLtools
 Requires: tabulate
+Requires: xlrd2
 License-File: LICENSE.txt
 
 Aciembler-preter
 --------------------------
 2023/4/23:
     | 1.0.0 alpha testing
     | 1.0.1 alpha testing
```

## Comparing `Aciembler-1.0.8.dist-info/RECORD` & `Aciembler-1.0.9.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-Aciembler/Aciembler.py,sha256=A93MLYaBjAjLEDFoiuFNT7wGy8fhLxLNltQr-dtLWnc,3178
+Aciembler/Aciembler.py,sha256=zLQHCaD7bwlTTxlJylYYBdFzrlRJcGprIRUNp5r8wI8,3213
 Aciembler/Error.py,sha256=x9ssz4F3GlmzpjhSqEE8jtYtenGX-lFvYuZR2AM4HsA,749
 Aciembler/First_pass.py,sha256=3k-WFEbr1rBdNlMWx9CaJiU3JSHaJBZ1NllFkOluj9I,3421
 Aciembler/__init__.py,sha256=hkZ7LtHFMTE7y4RIcGuEt8gMAeY2-g1irAYmtvOkR64,712
 Aciembler/objectCode.py,sha256=uNTSYTsNwWJNwYB4pe1LkG_cZVPYPJgUaALnYKm_Fng,506
 Aciembler/translator.py,sha256=HgSSurEBQOSLlAWN7PN1YQUPE8DEhfRkSAbPnnZ8wFQ,10544
-data/Template.xlsx,sha256=USSyDCqjP_lrb5zUIibSM-KZX5ToAg-qLG1iuuL-lnE,10686
-data/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-Aciembler-1.0.8.dist-info/LICENSE.txt,sha256=38hGaAYWJOuEjGRNUyJtwqSjp0GODZZ9UWoMtBbhaG8,1091
-Aciembler-1.0.8.dist-info/METADATA,sha256=FY7O0DgahBgZExmb6bLvwVynwsBjcXSzfEwyjbKC-LM,685
-Aciembler-1.0.8.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
-Aciembler-1.0.8.dist-info/top_level.txt,sha256=6TpCZLFVDZWui9z9dVSA1WdBskuCwPDcB-qXFeBcYPI,15
-Aciembler-1.0.8.dist-info/RECORD,,
+Aciembler/data/Template.xlsx,sha256=USSyDCqjP_lrb5zUIibSM-KZX5ToAg-qLG1iuuL-lnE,10686
+Aciembler-1.0.9.dist-info/LICENSE.txt,sha256=38hGaAYWJOuEjGRNUyJtwqSjp0GODZZ9UWoMtBbhaG8,1091
+Aciembler-1.0.9.dist-info/METADATA,sha256=LlLUVSIN6lEANY-Wr3o6pBxZX_2lj_BntSr5z5d13-0,701
+Aciembler-1.0.9.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
+Aciembler-1.0.9.dist-info/top_level.txt,sha256=pxsIJ5iLkKlA9kUzML4tWwn-4XzsD0alCIx1d2IgBRk,10
+Aciembler-1.0.9.dist-info/RECORD,,
```

