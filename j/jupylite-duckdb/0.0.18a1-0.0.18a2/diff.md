# Comparing `tmp/jupylite_duckdb-0.0.18a1-py3-none-any.whl.zip` & `tmp/jupylite_duckdb-0.0.18a2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 7302 bytes, number of entries: 10
+Zip file size: 7346 bytes, number of entries: 10
 -rw-rw-rw-  2.0 fat      128 b- defN 23-Apr-21 01:44 jupylite_duckdb/__init__.py
--rw-rw-rw-  2.0 fat       23 b- defN 23-Apr-22 23:18 jupylite_duckdb/_version.py
+-rw-rw-rw-  2.0 fat       23 b- defN 23-Apr-22 23:21 jupylite_duckdb/_version.py
 -rw-rw-rw-  2.0 fat     9216 b- defN 23-Apr-22 17:53 jupylite_duckdb/jdw.py
 -rw-rw-rw-  2.0 fat     2149 b- defN 23-Apr-22 23:17 jupylite_duckdb/jdw_magic.py
 -rw-rw-rw-  2.0 fat      979 b- defN 23-Apr-22 14:33 jupylite_duckdb/magic.py
--rw-rw-rw-  2.0 fat     1495 b- defN 23-Apr-22 23:18 jupylite_duckdb-0.0.18a1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2467 b- defN 23-Apr-22 23:18 jupylite_duckdb-0.0.18a1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-22 23:18 jupylite_duckdb-0.0.18a1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       16 b- defN 23-Apr-22 23:18 jupylite_duckdb-0.0.18a1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      850 b- defN 23-Apr-22 23:18 jupylite_duckdb-0.0.18a1.dist-info/RECORD
-10 files, 17415 bytes uncompressed, 5836 bytes compressed:  66.5%
+-rw-rw-rw-  2.0 fat     1495 b- defN 23-Apr-22 23:21 jupylite_duckdb-0.0.18a2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2559 b- defN 23-Apr-22 23:21 jupylite_duckdb-0.0.18a2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-22 23:21 jupylite_duckdb-0.0.18a2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       16 b- defN 23-Apr-22 23:21 jupylite_duckdb-0.0.18a2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      850 b- defN 23-Apr-22 23:21 jupylite_duckdb-0.0.18a2.dist-info/RECORD
+10 files, 17507 bytes uncompressed, 5880 bytes compressed:  66.4%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: jupylite_duckdb/jdw_magic.py
 Comment: 
 
 Filename: jupylite_duckdb/magic.py
 Comment: 
 
-Filename: jupylite_duckdb-0.0.18a1.dist-info/LICENSE
+Filename: jupylite_duckdb-0.0.18a2.dist-info/LICENSE
 Comment: 
 
-Filename: jupylite_duckdb-0.0.18a1.dist-info/METADATA
+Filename: jupylite_duckdb-0.0.18a2.dist-info/METADATA
 Comment: 
 
-Filename: jupylite_duckdb-0.0.18a1.dist-info/WHEEL
+Filename: jupylite_duckdb-0.0.18a2.dist-info/WHEEL
 Comment: 
 
-Filename: jupylite_duckdb-0.0.18a1.dist-info/top_level.txt
+Filename: jupylite_duckdb-0.0.18a2.dist-info/top_level.txt
 Comment: 
 
-Filename: jupylite_duckdb-0.0.18a1.dist-info/RECORD
+Filename: jupylite_duckdb-0.0.18a2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jupylite_duckdb/_version.py

```diff
@@ -1 +1 @@
-__version__="0.0.18a1"
+__version__="0.0.18a2"
```

## Comparing `jupylite_duckdb-0.0.18a1.dist-info/LICENSE` & `jupylite_duckdb-0.0.18a2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `jupylite_duckdb-0.0.18a1.dist-info/METADATA` & `jupylite_duckdb-0.0.18a2.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupylite-duckdb
-Version: 0.0.18a1
+Version: 0.0.18a2
 Summary: Testing
 Home-page: https://github.com/iqmo-org/
 Author: iqmo
 Author-email: info@iqmo.com
 Keywords: jupyterlite duckdb wasm
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -44,8 +44,8 @@
 
 
 ## Some development notes
 - There's some (well known) CORS considerations when trying to load data from other sites. Examples here are all using public sites, there's some limits that to address with your own jupyterlite deployment 
 - If you're adding local .py files, use [importlib.invalidate_caches()](https://pyodide.org/en/stable/usage/faq.html#why-can-t-i-import-a-file-i-just-wrote-to-the-file-system). Even then, it was flaky to import.
 - Careful with caching... %pip install will pull from browser cache. I had to clear frequently within dev tools
 - To clear local storage, which is annoyingly persistent, https://superuser.com/questions/519628/clear-html5-local-storage-on-a-specific-page
-- %autoawait is part of why this works in notebooks, which is enabled by default: https://ipython.readthedocs.io/en/stable/interactive/autoawait.html
+- %autoawait is part of why this works in notebooks, which is enabled by default. The %%dql cell magic patches transform-cell to push an await into the cell transformation.: https://ipython.readthedocs.io/en/stable/interactive/autoawait.html
```

## Comparing `jupylite_duckdb-0.0.18a1.dist-info/RECORD` & `jupylite_duckdb-0.0.18a2.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 jupylite_duckdb/__init__.py,sha256=-Z_P6KBbWKDsMsnvKal14k3bbGljgWmFQPEvz7zrLVU,128
-jupylite_duckdb/_version.py,sha256=bnGb1xseM2J6mXvI8BV0FJtYzRxYAhmJ11S9NxczMas,23
+jupylite_duckdb/_version.py,sha256=8kjh-5-0HwdjXERHb01s3MfdAh7atVwueZwVp9JKo_g,23
 jupylite_duckdb/jdw.py,sha256=LzIoBx4_3j3iUlp5lviHuISdCClNdHEKb9_O8X1-cpg,9216
 jupylite_duckdb/jdw_magic.py,sha256=EBbz8IhYUc4Wubrfjb5jQcxsHblPj-BdwerktkUWxBo,2149
 jupylite_duckdb/magic.py,sha256=okWgdHbcu0ul2BOYNdu9NHwRSoyAG_0m6RiGnw2Bj_k,979
-jupylite_duckdb-0.0.18a1.dist-info/LICENSE,sha256=WJMtiY9u9JD8FJ18a6_psLMXvrOIA7F-mYphCuyGFvw,1495
-jupylite_duckdb-0.0.18a1.dist-info/METADATA,sha256=O6zIm7mROG8kgkKpB2TDEDXdwQ1pvebr-P5A3oQWoIw,2467
-jupylite_duckdb-0.0.18a1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-jupylite_duckdb-0.0.18a1.dist-info/top_level.txt,sha256=y1GybQE7FyRTQPGLf2lE9dStC--h8ZozxhgXQRxz490,16
-jupylite_duckdb-0.0.18a1.dist-info/RECORD,,
+jupylite_duckdb-0.0.18a2.dist-info/LICENSE,sha256=WJMtiY9u9JD8FJ18a6_psLMXvrOIA7F-mYphCuyGFvw,1495
+jupylite_duckdb-0.0.18a2.dist-info/METADATA,sha256=GiT31739aHPaVigBw0mvlsTALlZCXtvjR88Qzm6GiVQ,2559
+jupylite_duckdb-0.0.18a2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+jupylite_duckdb-0.0.18a2.dist-info/top_level.txt,sha256=y1GybQE7FyRTQPGLf2lE9dStC--h8ZozxhgXQRxz490,16
+jupylite_duckdb-0.0.18a2.dist-info/RECORD,,
```

