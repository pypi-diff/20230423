# Comparing `tmp/varya-0.0.5a1-py3-none-any.whl.zip` & `tmp/varya-0.0.6a1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 4278 bytes, number of entries: 9
--rw-r--r--  2.0 unx      206 b- defN 23-Mar-11 21:43 varya/__init__.py
+Zip file size: 4314 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      206 b- defN 23-Mar-12 11:02 varya/__init__.py
 -rw-r--r--  2.0 unx     2140 b- defN 23-Mar-11 04:33 varya/compose/__compose.py
 -rw-r--r--  2.0 unx       44 b- defN 23-Mar-11 05:45 varya/compose/__init__.py
--rw-r--r--  2.0 unx     2993 b- defN 23-Mar-11 21:43 varya/compose/core.py
--rw-r--r--  2.0 unx     1519 b- defN 23-Mar-11 21:43 varya-0.0.5a1.dist-info/LICENSE
--rw-r--r--  2.0 unx      558 b- defN 23-Mar-11 21:43 varya-0.0.5a1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-11 21:43 varya-0.0.5a1.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Mar-11 21:43 varya-0.0.5a1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      698 b- defN 23-Mar-11 21:43 varya-0.0.5a1.dist-info/RECORD
-9 files, 8257 bytes uncompressed, 3076 bytes compressed:  62.7%
+-rw-r--r--  2.0 unx     3227 b- defN 23-Mar-12 11:02 varya/compose/core.py
+-rw-r--r--  2.0 unx     1519 b- defN 23-Mar-12 11:02 varya-0.0.6a1.dist-info/LICENSE
+-rw-r--r--  2.0 unx      558 b- defN 23-Mar-12 11:02 varya-0.0.6a1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Mar-12 11:02 varya-0.0.6a1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Mar-12 11:02 varya-0.0.6a1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      698 b- defN 23-Mar-12 11:02 varya-0.0.6a1.dist-info/RECORD
+9 files, 8491 bytes uncompressed, 3112 bytes compressed:  63.3%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: varya/compose/__init__.py
 Comment: 
 
 Filename: varya/compose/core.py
 Comment: 
 
-Filename: varya-0.0.5a1.dist-info/LICENSE
+Filename: varya-0.0.6a1.dist-info/LICENSE
 Comment: 
 
-Filename: varya-0.0.5a1.dist-info/METADATA
+Filename: varya-0.0.6a1.dist-info/METADATA
 Comment: 
 
-Filename: varya-0.0.5a1.dist-info/WHEEL
+Filename: varya-0.0.6a1.dist-info/WHEEL
 Comment: 
 
-Filename: varya-0.0.5a1.dist-info/top_level.txt
+Filename: varya-0.0.6a1.dist-info/top_level.txt
 Comment: 
 
-Filename: varya-0.0.5a1.dist-info/RECORD
+Filename: varya-0.0.6a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## varya/__init__.py

```diff
@@ -1,6 +1,6 @@
-__version__ = '0.0.5a1'
+__version__ = '0.0.6a1'
 __author__ = 'Kritik Seth'
 __maintainer__ = __author__
 __license__ = 'BSD 3-Clause License'
 __url__ = 'https://github.com/varya-ml/varya'
 __connect__ = 'https://www.kritikseth.com/'
```

## varya/compose/core.py

```diff
@@ -67,14 +67,26 @@
         
         elif isinstance(target, (pandas.core.frame.DataFrame, pandas.core.series.Series,
                                  numpy.ndarray,
                                  torch.Tensor)):
             self._target = target
             if isinstance(target, (pandas.core.frame.DataFrame, pandas.core.series.Series)):
                 self.target_name = target.name
+    
+    @property
+    def rows(self):
+        return self.data.shape[0]
+    
+    @property
+    def columns(self):
+        return self.data.shape[1]
+    
+    @property
+    def shape(self):
+        return (self.rows(), self.columns())
 
     def _recast(self, datum):
 
         if isinstance(datum, (pandas.core.frame.DataFrame, pandas.core.series.Series)):
             return torch.from_numpy(datum.values)
         
         if isinstance(datum, numpy.ndarray):
```

## Comparing `varya-0.0.5a1.dist-info/LICENSE` & `varya-0.0.6a1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `varya-0.0.5a1.dist-info/METADATA` & `varya-0.0.6a1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: varya
-Version: 0.0.5a1
+Version: 0.0.6a1
 Summary: Machine Learning Tools
 Home-page: https://github.com/varya-ml/varya
 Author: Kritik Seth
 Author-email: sethkritik@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

## Comparing `varya-0.0.5a1.dist-info/RECORD` & `varya-0.0.6a1.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-varya/__init__.py,sha256=mSGRJA8unoLUGk3QTHn94KjDBy_JDTInlQT1qGa6iD0,206
+varya/__init__.py,sha256=E16DH6iNcQ5oFxqlAAcENk_QhW1ROmigqBzw4uEsboM,206
 varya/compose/__compose.py,sha256=ioCqukxIiaWk3LSJQW6ct4V8RJcm5LmQLmjX7bXifrc,2140
 varya/compose/__init__.py,sha256=-Fzc0Cmpu2jpN3R5GfP9hC_L23wTl_dy_yu1zURVUGw,44
-varya/compose/core.py,sha256=udXqrj7r6JixEYzmqga3j5r0anpzRPqRr11adZgJj0U,2993
-varya-0.0.5a1.dist-info/LICENSE,sha256=EFNCHlXvsrMcrrVHTK6Na8ysDWp6yU-7SmMcZWiSAVk,1519
-varya-0.0.5a1.dist-info/METADATA,sha256=vsno-GDJ5xBc7OULQ0rFqS1p9RD0s0bAFVBsMjptFig,558
-varya-0.0.5a1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-varya-0.0.5a1.dist-info/top_level.txt,sha256=1CZBh5KXfjOyndV2X6niNupUsYS0vcstKJvukU_2Vi4,7
-varya-0.0.5a1.dist-info/RECORD,,
+varya/compose/core.py,sha256=FATu4lrDIogq3l-koktPaF_3EDinTbU5okZn1dsmUxM,3227
+varya-0.0.6a1.dist-info/LICENSE,sha256=EFNCHlXvsrMcrrVHTK6Na8ysDWp6yU-7SmMcZWiSAVk,1519
+varya-0.0.6a1.dist-info/METADATA,sha256=KsZBZusSzBFvE0I2uR8vNRhh7ewKX-1ncdS-6cCdw2s,558
+varya-0.0.6a1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+varya-0.0.6a1.dist-info/top_level.txt,sha256=1CZBh5KXfjOyndV2X6niNupUsYS0vcstKJvukU_2Vi4,7
+varya-0.0.6a1.dist-info/RECORD,,
```

