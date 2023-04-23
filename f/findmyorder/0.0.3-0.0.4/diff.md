# Comparing `tmp/findmyorder-0.0.3.tar.gz` & `tmp/findmyorder-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findmyorder-0.0.3.tar", max compression
+gzip compressed data, was "findmyorder-0.0.4.tar", max compression
```

## Comparing `findmyorder-0.0.3.tar` & `findmyorder-0.0.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-04-23 07:02:22.127779 findmyorder-0.0.3/LICENSE
--rw-r--r--   0        0        0     1426 2023-04-23 07:02:22.127779 findmyorder-0.0.3/README.md
--rw-r--r--   0        0        0      103 2023-04-23 07:02:22.799793 findmyorder-0.0.3/findmyorder/__init__.py
--rw-r--r--   0        0        0      146 2023-04-23 07:02:22.127779 findmyorder-0.0.3/findmyorder/config.py
--rw-r--r--   0        0        0     2119 2023-04-23 07:02:22.127779 findmyorder-0.0.3/findmyorder/main.py
--rw-r--r--   0        0        0       77 2023-04-23 07:02:22.127779 findmyorder-0.0.3/findmyorder/settings.toml
--rw-r--r--   0        0        0      995 2023-04-23 07:02:22.795793 findmyorder-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2249 1970-01-01 00:00:00.000000 findmyorder-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-23 10:52:17.587076 findmyorder-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1426 2023-04-23 10:52:17.587076 findmyorder-0.0.4/README.md
+-rw-r--r--   0        0        0      103 2023-04-23 10:52:18.295086 findmyorder-0.0.4/findmyorder/__init__.py
+-rw-r--r--   0        0        0      218 2023-04-23 10:52:17.587076 findmyorder-0.0.4/findmyorder/config.py
+-rw-r--r--   0        0        0     2596 2023-04-23 10:52:17.587076 findmyorder-0.0.4/findmyorder/main.py
+-rw-r--r--   0        0        0      199 2023-04-23 10:52:17.587076 findmyorder-0.0.4/findmyorder/settings.toml
+-rw-r--r--   0        0        0      962 2023-04-23 10:52:18.291086 findmyorder-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2199 1970-01-01 00:00:00.000000 findmyorder-0.0.4/PKG-INFO
```

### Comparing `findmyorder-0.0.3/LICENSE` & `findmyorder-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `findmyorder-0.0.3/README.md` & `findmyorder-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `findmyorder-0.0.3/findmyorder/main.py` & `findmyorder-0.0.4/findmyorder/main.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import asyncio, logging, re
+from datetime import datetime
+
 
 from findmyorder.config import settings
 from findmyorder import __version__
 
 # import pyparsing as pp
 
 # from translate import Translator
@@ -19,51 +21,71 @@
         
        # translation = translator.translate("ACHETER")
         
     def search(self,
                message_to_parse: str = None,
                ):
       try:
-        myDict = settings.DIRECTION
+        myDict = settings.IDENTIFIER
 
         for word in myDict:
             self.logger.debug(f"Loop check {word}")
             if re.search(word, message_to_parse):
               self.logger.debug(f"found {word} in {message_to_parse}")
               return True
         self.logger.debug(f"no word identified in {message_to_parse}")
         return False
       except Exception as e:
         self.logger.debug(f"error identify {e}")
         return False
 
+    # def identify(self,
+    #            mystring: str = None,
+    #            ):
+    #     order_format = self.identify_order_format(mystring)
+    #     order_data = self.identify_order_element(mystring)
+
+    # def identify_order_format(self,
+    #            mystring: str = None,
+    #            ):
+    #   return
+
+
+
     def identify(self,
-               order_string: str = None,
+               mystring: str = None,
                ):
       try:
-        self.logger.debug(f"identify order for {order_string}")
-        if (self.search(order_string)):
-            order = order_string.split()
-          # self.logger.info(msg=f"Order parsing: {order}")
-          # direction = wordlist[0].upper()
-          # stoploss = 100
-          # takeprofit = 100
-          # quantity = 10
-          # # self.direction
-          # # self.symbol
-          # # self.amount
-          # # self.quantity
-          # # self.stoploss
-          # # self.takeprofit
-          # # self.comment
-          # # self.exchange
-          # if wordlistsize > 2:
-          #     stoploss = wordlist[2][3:]
-          #     takeprofit = wordlist[3][3:]
-          #     quantity = wordlist[4][2:-1]
-          # symbol = wordlist[1]
-          # order=[direction,symbol,stoploss,takeprofit,quantity]
+        self.logger.debug(f"identify_order_element for {order_string}")
+        if (self.search(mystring)):
+            order_raw = mystring.split()
+            self.logger.info(msg=f"Order identified: {order raw}")
+            order = {}
+            order['direction'] = 'BUY'
+            order['symbol'] = 'EURUSD'
+            order['quantity'] = 10
+            order['amount'] = 100
+            order['stoploss'] = 1000
+            order['comments'] = 'default comment'
+            order['market'] = 'Any'
+            order['exchange'] = 'Any'
+            order['timestamp'] = datetime.utcnow()
+            order['leverage'] = 1
+            order['takeprofit'] = {'tp1':1, 'tp2':10, 'tp3':100, 'tp4':1000, 'tp5':1000}
+
+            # if order_raw
+            #   order['direction'] = 'BUY'
             return order
 
       except Exception as e:
-          self.logger.debug(f"error identify {e}")
+          self.logger.debug(f"error identify_order_element {e}")
           return
+
+
+
+
+# class order:
+
+#      def __init__(self,
+#                  ):
+#           self.direction = 'buy'
+#           self.symbol = 'EURUSD'
```

### Comparing `findmyorder-0.0.3/pyproject.toml` & `findmyorder-0.0.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "findmyorder"
-version = "0.0.3"
+version = "0.0.4"
 description = "A python package to identify and parse order for trade execution."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["trading", "order", "trade","buy","sell"]
 
 
@@ -12,17 +12,14 @@
 "Changelog" =  "https://github.com/mraniki/findmyorder/blob/dev/CHANGELOG.rst"
 "Support" =  "https://github.com/mraniki/findmyorder/discussions"
 "Issues" =  "https://github.com/mraniki/findmyorder/issues"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.11"
 asyncio = "*"
-pyparsing = "*"
-translate = "*"
-
 
 [tool.poetry.dev-dependencies]
 python-semantic-release = "*"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `findmyorder-0.0.3/PKG-INFO` & `findmyorder-0.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: findmyorder
-Version: 0.0.3
+Version: 0.0.4
 Summary: A python package to identify and parse order for trade execution.
 License: MIT
 Keywords: trading,order,trade,buy,sell
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: asyncio
-Requires-Dist: pyparsing
-Requires-Dist: translate
 Project-URL: Changelog, https://github.com/mraniki/findmyorder/blob/dev/CHANGELOG.rst
 Project-URL: Issues, https://github.com/mraniki/findmyorder/issues
 Project-URL: Support, https://github.com/mraniki/findmyorder/discussions
 Description-Content-Type: text/markdown
 
 # Find my order.
```

