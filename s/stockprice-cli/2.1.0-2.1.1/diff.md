# Comparing `tmp/stockprice_cli-2.1.0-py3-none-any.whl.zip` & `tmp/stockprice_cli-2.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3291 bytes, number of entries: 8
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-22 16:59 stockprice/__init__.py
--rw-r--r--  2.0 unx     2552 b- defN 23-Apr-22 16:59 stockprice/calculate_price_movement.py
--rw-r--r--  2.0 unx      974 b- defN 23-Apr-22 16:59 stockprice/main.py
--rw-r--r--  2.0 unx      612 b- defN 23-Apr-22 16:59 stockprice_cli-2.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-22 16:59 stockprice_cli-2.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       53 b- defN 23-Apr-22 16:59 stockprice_cli-2.1.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 23-Apr-22 16:59 stockprice_cli-2.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      672 b- defN 23-Apr-22 16:59 stockprice_cli-2.1.0.dist-info/RECORD
-8 files, 4966 bytes uncompressed, 2099 bytes compressed:  57.7%
+Zip file size: 3367 bytes, number of entries: 8
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-23 10:49 stockprice/__init__.py
+-rw-r--r--  2.0 unx     2552 b- defN 23-Apr-23 10:49 stockprice/calculate_price_movement.py
+-rw-r--r--  2.0 unx     1146 b- defN 23-Apr-23 10:49 stockprice/main.py
+-rw-r--r--  2.0 unx      612 b- defN 23-Apr-23 10:49 stockprice_cli-2.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-23 10:49 stockprice_cli-2.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 23-Apr-23 10:49 stockprice_cli-2.1.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 23-Apr-23 10:49 stockprice_cli-2.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      673 b- defN 23-Apr-23 10:49 stockprice_cli-2.1.1.dist-info/RECORD
+8 files, 5139 bytes uncompressed, 2175 bytes compressed:  57.7%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: stockprice/calculate_price_movement.py
 Comment: 
 
 Filename: stockprice/main.py
 Comment: 
 
-Filename: stockprice_cli-2.1.0.dist-info/METADATA
+Filename: stockprice_cli-2.1.1.dist-info/METADATA
 Comment: 
 
-Filename: stockprice_cli-2.1.0.dist-info/WHEEL
+Filename: stockprice_cli-2.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: stockprice_cli-2.1.0.dist-info/entry_points.txt
+Filename: stockprice_cli-2.1.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: stockprice_cli-2.1.0.dist-info/top_level.txt
+Filename: stockprice_cli-2.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: stockprice_cli-2.1.0.dist-info/RECORD
+Filename: stockprice_cli-2.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## stockprice/main.py

```diff
@@ -1,13 +1,17 @@
 import sys
 
 from stockprice.calculate_price_movement import calculate_price_movement
 
 
 def main(args: list = sys.argv) -> None:
+    if len(args) == 1 and args[0] == "stockprice":
+        print("Please provide at least one stock ticker.")
+        print("Example: stockprice tsla,aapl")
+        return
     raw_inputs = args[1:]
     stock_tickers = []
     for input in raw_inputs:
         input = input.upper()
         if input[-1] == ",":
             input = input[:-1]
```

## Comparing `stockprice_cli-2.1.0.dist-info/METADATA` & `stockprice_cli-2.1.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stockprice-cli
-Version: 2.1.0
+Version: 2.1.1
 Summary: UNKNOWN
 Home-page: https://github.com/Thomas-mcinally/stockprice
 Author: Thomas Mcinally
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

## Comparing `stockprice_cli-2.1.0.dist-info/RECORD` & `stockprice_cli-2.1.1.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 stockprice/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 stockprice/calculate_price_movement.py,sha256=5HTpYyA7p2tfo0AzC-xq1J6QCSOJ4OmqbGSmo1F98xE,2552
-stockprice/main.py,sha256=J3LN9QYpYlPPF8YSd52uxSqBXyn1Ky1zBplg4gWISmA,974
-stockprice_cli-2.1.0.dist-info/METADATA,sha256=OiI3L6uRVjHIEXx2zyKAK9iH1TfRxtRT9gOzFSfBF2s,612
-stockprice_cli-2.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-stockprice_cli-2.1.0.dist-info/entry_points.txt,sha256=BbbvxzL6AWVnrrEHkXLFL8NaKwhZ0NsKnzHKibL587M,53
-stockprice_cli-2.1.0.dist-info/top_level.txt,sha256=KeT6ClRPQ5zQdkU0Ela_rRQ2aR7Dy7SjyOcfhcPy6kw,11
-stockprice_cli-2.1.0.dist-info/RECORD,,
+stockprice/main.py,sha256=PkEZ0hPyXG6ZYNw7sBCpQeyGkMT0yszffy1Bv85WYFk,1146
+stockprice_cli-2.1.1.dist-info/METADATA,sha256=4pOPXR-7A50_tLPc2U0HkKL-Gm7oveB6InKlBjMnyO0,612
+stockprice_cli-2.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+stockprice_cli-2.1.1.dist-info/entry_points.txt,sha256=BbbvxzL6AWVnrrEHkXLFL8NaKwhZ0NsKnzHKibL587M,53
+stockprice_cli-2.1.1.dist-info/top_level.txt,sha256=KeT6ClRPQ5zQdkU0Ela_rRQ2aR7Dy7SjyOcfhcPy6kw,11
+stockprice_cli-2.1.1.dist-info/RECORD,,
```

