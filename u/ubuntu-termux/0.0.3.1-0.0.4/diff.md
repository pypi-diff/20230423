# Comparing `tmp/ubuntu_termux-0.0.3.1-py3-none-any.whl.zip` & `tmp/ubuntu_termux-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 15122 bytes, number of entries: 9
--rw-rw----  2.0 unx        0 b- defN 23-Jan-02 01:36 ubuntu_termux/__init__.py
--rw-rw----  2.0 unx     1099 b- defN 23-Jan-02 01:58 ubuntu_termux/install.py
--rw-rw----  2.0 unx      324 b- defN 23-Jan-02 01:36 ubuntu_termux/start.py
--rw-rw----  2.0 unx    35149 b- defN 23-Jan-02 02:05 ubuntu_termux-0.0.3.1.dist-info/LICENSE
--rw-rw----  2.0 unx      426 b- defN 23-Jan-02 02:05 ubuntu_termux-0.0.3.1.dist-info/METADATA
--rw-rw----  2.0 unx       92 b- defN 23-Jan-02 02:05 ubuntu_termux-0.0.3.1.dist-info/WHEEL
--rw-rw----  2.0 unx       66 b- defN 23-Jan-02 02:05 ubuntu_termux-0.0.3.1.dist-info/entry_points.txt
--rw-rw----  2.0 unx       14 b- defN 23-Jan-02 02:05 ubuntu_termux-0.0.3.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      767 b- defN 23-Jan-02 02:05 ubuntu_termux-0.0.3.1.dist-info/RECORD
-9 files, 37937 bytes uncompressed, 13780 bytes compressed:  63.7%
+Zip file size: 15077 bytes, number of entries: 9
+-rw-rw----  2.0 unx        0 b- defN 23-Apr-21 13:33 ubuntu_termux/__init__.py
+-rw-rw----  2.0 unx     1099 b- defN 23-Apr-21 13:33 ubuntu_termux/install.py
+-rw-rw----  2.0 unx      324 b- defN 23-Apr-21 13:33 ubuntu_termux/start.py
+-rw-rw----  2.0 unx    35149 b- defN 23-Apr-22 22:31 ubuntu_termux-0.0.4.dist-info/LICENSE
+-rw-rw----  2.0 unx      404 b- defN 23-Apr-22 22:31 ubuntu_termux-0.0.4.dist-info/METADATA
+-rw-rw----  2.0 unx       92 b- defN 23-Apr-22 22:31 ubuntu_termux-0.0.4.dist-info/WHEEL
+-rw-rw----  2.0 unx       65 b- defN 23-Apr-22 22:31 ubuntu_termux-0.0.4.dist-info/entry_points.txt
+-rw-rw----  2.0 unx       14 b- defN 23-Apr-22 22:31 ubuntu_termux-0.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      755 b- defN 23-Apr-22 22:31 ubuntu_termux-0.0.4.dist-info/RECORD
+9 files, 37902 bytes uncompressed, 13759 bytes compressed:  63.7%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: ubuntu_termux/install.py
 Comment: 
 
 Filename: ubuntu_termux/start.py
 Comment: 
 
-Filename: ubuntu_termux-0.0.3.1.dist-info/LICENSE
+Filename: ubuntu_termux-0.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: ubuntu_termux-0.0.3.1.dist-info/METADATA
+Filename: ubuntu_termux-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: ubuntu_termux-0.0.3.1.dist-info/WHEEL
+Filename: ubuntu_termux-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: ubuntu_termux-0.0.3.1.dist-info/entry_points.txt
+Filename: ubuntu_termux-0.0.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: ubuntu_termux-0.0.3.1.dist-info/top_level.txt
+Filename: ubuntu_termux-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: ubuntu_termux-0.0.3.1.dist-info/RECORD
+Filename: ubuntu_termux-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `ubuntu_termux-0.0.3.1.dist-info/LICENSE` & `ubuntu_termux-0.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ubuntu_termux-0.0.3.1.dist-info/RECORD` & `ubuntu_termux-0.0.4.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ubuntu_termux/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ubuntu_termux/install.py,sha256=teuVq3vP4OAYrHDxQi3r5LtVt1BzKHU6gtU_TKrR2BI,1099
 ubuntu_termux/start.py,sha256=rXGvSDhbHjHzLXCChkmUCpcThyhZ9QpV6UiIbW_ED8g,324
-ubuntu_termux-0.0.3.1.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-ubuntu_termux-0.0.3.1.dist-info/METADATA,sha256=G01oiYhLbFgBnv0eyi2UQfW2YEvWfD4xDdjOSWgQyJM,426
-ubuntu_termux-0.0.3.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-ubuntu_termux-0.0.3.1.dist-info/entry_points.txt,sha256=zY0otA7EoWtlSdA36Y2AbYCbFGEcDDvs4iq1MiJP8U0,66
-ubuntu_termux-0.0.3.1.dist-info/top_level.txt,sha256=QfzseQYrbV8VQtm2GSbrPl9VrO1-yPR8WxtyzxGN0iI,14
-ubuntu_termux-0.0.3.1.dist-info/RECORD,,
+ubuntu_termux-0.0.4.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+ubuntu_termux-0.0.4.dist-info/METADATA,sha256=eQbig0RhgziKNwii5Os0Laatfv18uZXMnFuFYCv97_c,404
+ubuntu_termux-0.0.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+ubuntu_termux-0.0.4.dist-info/entry_points.txt,sha256=QXX1Ji4FoI5La0GyHxweGCvR8Zz3UDdmF1gz0sMG_qA,65
+ubuntu_termux-0.0.4.dist-info/top_level.txt,sha256=QfzseQYrbV8VQtm2GSbrPl9VrO1-yPR8WxtyzxGN0iI,14
+ubuntu_termux-0.0.4.dist-info/RECORD,,
```

