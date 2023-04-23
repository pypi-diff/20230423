# Comparing `tmp/findmyorder-0.0.4.tar.gz` & `tmp/findmyorder-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findmyorder-0.0.4.tar", max compression
+gzip compressed data, was "findmyorder-0.0.5.tar", max compression
```

## Comparing `findmyorder-0.0.4.tar` & `findmyorder-0.0.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-04-23 10:52:17.587076 findmyorder-0.0.4/LICENSE
--rw-r--r--   0        0        0     1426 2023-04-23 10:52:17.587076 findmyorder-0.0.4/README.md
--rw-r--r--   0        0        0      103 2023-04-23 10:52:18.295086 findmyorder-0.0.4/findmyorder/__init__.py
--rw-r--r--   0        0        0      218 2023-04-23 10:52:17.587076 findmyorder-0.0.4/findmyorder/config.py
--rw-r--r--   0        0        0     2596 2023-04-23 10:52:17.587076 findmyorder-0.0.4/findmyorder/main.py
--rw-r--r--   0        0        0      199 2023-04-23 10:52:17.587076 findmyorder-0.0.4/findmyorder/settings.toml
--rw-r--r--   0        0        0      962 2023-04-23 10:52:18.291086 findmyorder-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2199 1970-01-01 00:00:00.000000 findmyorder-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-23 12:36:36.034577 findmyorder-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1426 2023-04-23 12:36:36.034577 findmyorder-0.0.5/README.md
+-rw-r--r--   0        0        0      103 2023-04-23 12:36:36.766582 findmyorder-0.0.5/findmyorder/__init__.py
+-rw-r--r--   0        0        0      218 2023-04-23 12:36:36.034577 findmyorder-0.0.5/findmyorder/config.py
+-rw-r--r--   0        0        0     2596 2023-04-23 12:36:36.034577 findmyorder-0.0.5/findmyorder/main.py
+-rw-r--r--   0        0        0      199 2023-04-23 12:36:36.034577 findmyorder-0.0.5/findmyorder/settings.toml
+-rw-r--r--   0        0        0      962 2023-04-23 12:36:36.766582 findmyorder-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2199 1970-01-01 00:00:00.000000 findmyorder-0.0.5/PKG-INFO
```

### Comparing `findmyorder-0.0.4/LICENSE` & `findmyorder-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `findmyorder-0.0.4/README.md` & `findmyorder-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `findmyorder-0.0.4/findmyorder/main.py` & `findmyorder-0.0.5/findmyorder/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     def identify(self,
                mystring: str = None,
                ):
       try:
         self.logger.debug(f"identify_order_element for {order_string}")
         if (self.search(mystring)):
             order_raw = mystring.split()
-            self.logger.info(msg=f"Order identified: {order raw}")
+            self.logger.info(msg=f"Order identified: {order_raw}")
             order = {}
             order['direction'] = 'BUY'
             order['symbol'] = 'EURUSD'
             order['quantity'] = 10
             order['amount'] = 100
             order['stoploss'] = 1000
             order['comments'] = 'default comment'
```

### Comparing `findmyorder-0.0.4/pyproject.toml` & `findmyorder-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "findmyorder"
-version = "0.0.4"
+version = "0.0.5"
 description = "A python package to identify and parse order for trade execution."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["trading", "order", "trade","buy","sell"]
```

### Comparing `findmyorder-0.0.4/PKG-INFO` & `findmyorder-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findmyorder
-Version: 0.0.4
+Version: 0.0.5
 Summary: A python package to identify and parse order for trade execution.
 License: MIT
 Keywords: trading,order,trade,buy,sell
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

