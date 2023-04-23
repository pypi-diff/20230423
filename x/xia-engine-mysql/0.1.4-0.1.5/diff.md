# Comparing `tmp/xia_engine_mysql-0.1.4-cp39-none-win_amd64.whl.zip` & `tmp/xia_engine_mysql-0.1.5-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 138468 bytes, number of entries: 7
--rw-r--r--  2.0 unx      144 b- defN 23-Mar-07 20:06 xia_engine_mysql/__init__.py
--rw-r--r--  2.0 unx   338944 b- defN 23-Mar-07 20:09 xia_engine_mysql/engine.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      152 b- defN 23-Mar-07 20:09 xia_engine_mysql-0.1.4.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      715 b- defN 23-Mar-07 20:09 xia_engine_mysql-0.1.4.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Mar-07 20:09 xia_engine_mysql-0.1.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Mar-07 20:09 xia_engine_mysql-0.1.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      618 b- defN 23-Mar-07 20:09 xia_engine_mysql-0.1.4.dist-info/RECORD
-7 files, 340689 bytes uncompressed, 137358 bytes compressed:  59.7%
+Zip file size: 138427 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      144 b- defN 23-Apr-23 11:18 xia_engine_mysql/__init__.py
+-rw-r--r--  2.0 unx   337920 b- defN 23-Apr-23 11:21 xia_engine_mysql/engine.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-23 11:21 xia_engine_mysql-0.1.5.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      715 b- defN 23-Apr-23 11:21 xia_engine_mysql-0.1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Apr-23 11:21 xia_engine_mysql-0.1.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Apr-23 11:21 xia_engine_mysql-0.1.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      618 b- defN 23-Apr-23 11:21 xia_engine_mysql-0.1.5.dist-info/RECORD
+7 files, 339665 bytes uncompressed, 137317 bytes compressed:  59.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_engine_mysql/__init__.py
 Comment: 
 
 Filename: xia_engine_mysql/engine.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_engine_mysql-0.1.4.dist-info/LICENSE.txt
+Filename: xia_engine_mysql-0.1.5.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_engine_mysql-0.1.4.dist-info/METADATA
+Filename: xia_engine_mysql-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: xia_engine_mysql-0.1.4.dist-info/WHEEL
+Filename: xia_engine_mysql-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: xia_engine_mysql-0.1.4.dist-info/top_level.txt
+Filename: xia_engine_mysql-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_engine_mysql-0.1.4.dist-info/RECORD
+Filename: xia_engine_mysql-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_engine_mysql/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_engine_mysql.engine import MysqlEngine, MysqlConnectParam
 
 __all__ = [
     "MysqlEngine", "MysqlConnectParam"
 ]
 
-__version__ = "0.1.4"
+__version__ = "0.1.5"
```

## Comparing `xia_engine_mysql-0.1.4.dist-info/METADATA` & `xia_engine_mysql-0.1.5.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-engine-mysql
-Version: 0.1.4
+Version: 0.1.5
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-engine-mysql/0.1.4/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-engine-mysql/0.1.5/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_engine_mysql-0.1.4.dist-info/RECORD` & `xia_engine_mysql-0.1.5.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_engine_mysql/__init__.py,sha256=YoWy1ac1Rag9UMgLhOSmPnILVYAd8mf6mRv3GDLYZuU,144
-xia_engine_mysql/engine.cp39-win_amd64.pyd,sha256=8fxoI9nORhu_ngUFoshPHv1YCFuc51NGb9Ng6voJxEQ,338944
-xia_engine_mysql-0.1.4.dist-info/LICENSE.txt,sha256=evtniHLykwblDbV3lZzaD98uMkurAme7DE6rndxMK5Q,152
-xia_engine_mysql-0.1.4.dist-info/METADATA,sha256=JJNP2aZUHcz9TTv446U8NcmCxJmrpY9BH-kmiZa_-mM,715
-xia_engine_mysql-0.1.4.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
-xia_engine_mysql-0.1.4.dist-info/top_level.txt,sha256=iEabOz01n8HLyWdyjMLZMYHeuLxpVhBNWV3Rh6M4n1c,17
-xia_engine_mysql-0.1.4.dist-info/RECORD,,
+xia_engine_mysql/__init__.py,sha256=rq_rDbMmtXozsG4h_GghOWMpnGc-_4g-Kmyp7tux6U8,144
+xia_engine_mysql/engine.cp39-win_amd64.pyd,sha256=DMF7rtVsjyzxGNWtZEFir_IM2RuoloVez1VlcOOlBPA,337920
+xia_engine_mysql-0.1.5.dist-info/LICENSE.txt,sha256=30wWxpufZqbxK7WdwZRoX8iA_veQA4gbl5oih3j5vFs,152
+xia_engine_mysql-0.1.5.dist-info/METADATA,sha256=rOkmuCSLkice6qf0ncyWkaGL7F5pFiwvbUqAi0kbQmM,715
+xia_engine_mysql-0.1.5.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
+xia_engine_mysql-0.1.5.dist-info/top_level.txt,sha256=iEabOz01n8HLyWdyjMLZMYHeuLxpVhBNWV3Rh6M4n1c,17
+xia_engine_mysql-0.1.5.dist-info/RECORD,,
```

