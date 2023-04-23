# Comparing `tmp/tunein-0.0.2a3-py3-none-any.whl.zip` & `tmp/tunein-0.0.3a1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 8020 bytes, number of entries: 9
--rw-r--r--  2.0 unx     3166 b- defN 23-Feb-19 19:27 tunein/__init__.py
--rw-r--r--  2.0 unx     1972 b- defN 23-Feb-19 19:27 tunein/parse.py
--rw-r--r--  2.0 unx      114 b- defN 23-Feb-19 19:27 tunein/version.py
--rw-r--r--  2.0 unx     1683 b- defN 23-Feb-19 19:27 tunein/xml_helper.py
--rw-r--r--  2.0 unx    11431 b- defN 23-Feb-19 19:27 tunein-0.0.2a3.dist-info/LICENSE
--rw-r--r--  2.0 unx      270 b- defN 23-Feb-19 19:27 tunein-0.0.2a3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-19 19:27 tunein-0.0.2a3.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Feb-19 19:27 tunein-0.0.2a3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      687 b- defN 23-Feb-19 19:27 tunein-0.0.2a3.dist-info/RECORD
-9 files, 19422 bytes uncompressed, 6846 bytes compressed:  64.8%
+Zip file size: 8022 bytes, number of entries: 9
+-rw-r--r--  2.0 unx     3166 b- defN 23-Apr-23 18:42 tunein/__init__.py
+-rw-r--r--  2.0 unx     1972 b- defN 23-Apr-23 18:42 tunein/parse.py
+-rw-r--r--  2.0 unx      114 b- defN 23-Apr-23 18:42 tunein/version.py
+-rw-r--r--  2.0 unx     1683 b- defN 23-Apr-23 18:42 tunein/xml_helper.py
+-rw-r--r--  2.0 unx    11431 b- defN 23-Apr-23 18:42 tunein-0.0.3a1.dist-info/LICENSE
+-rw-r--r--  2.0 unx      270 b- defN 23-Apr-23 18:42 tunein-0.0.3a1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-23 18:42 tunein-0.0.3a1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Apr-23 18:42 tunein-0.0.3a1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      687 b- defN 23-Apr-23 18:42 tunein-0.0.3a1.dist-info/RECORD
+9 files, 19422 bytes uncompressed, 6848 bytes compressed:  64.7%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: tunein/version.py
 Comment: 
 
 Filename: tunein/xml_helper.py
 Comment: 
 
-Filename: tunein-0.0.2a3.dist-info/LICENSE
+Filename: tunein-0.0.3a1.dist-info/LICENSE
 Comment: 
 
-Filename: tunein-0.0.2a3.dist-info/METADATA
+Filename: tunein-0.0.3a1.dist-info/METADATA
 Comment: 
 
-Filename: tunein-0.0.2a3.dist-info/WHEEL
+Filename: tunein-0.0.3a1.dist-info/WHEEL
 Comment: 
 
-Filename: tunein-0.0.2a3.dist-info/top_level.txt
+Filename: tunein-0.0.3a1.dist-info/top_level.txt
 Comment: 
 
-Filename: tunein-0.0.2a3.dist-info/RECORD
+Filename: tunein-0.0.3a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tunein/version.py

```diff
@@ -1,6 +1,6 @@
 # START_VERSION_BLOCK
 VERSION_MAJOR = 0
 VERSION_MINOR = 0
-VERSION_BUILD = 2
-VERSION_ALPHA = 3
+VERSION_BUILD = 3
+VERSION_ALPHA = 1
 # END_VERSION_BLOCK
```

## Comparing `tunein-0.0.2a3.dist-info/LICENSE` & `tunein-0.0.3a1.dist-info/LICENSE`

 * *Files identical despite different names*

