# Comparing `tmp/findmyorder-0.0.8.tar.gz` & `tmp/findmyorder-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findmyorder-0.0.8.tar", max compression
+gzip compressed data, was "findmyorder-0.0.9.tar", max compression
```

## Comparing `findmyorder-0.0.8.tar` & `findmyorder-0.0.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-04-23 13:51:27.929402 findmyorder-0.0.8/LICENSE
--rw-r--r--   0        0        0     1426 2023-04-23 13:51:27.929402 findmyorder-0.0.8/README.md
--rw-r--r--   0        0        0      103 2023-04-23 13:51:28.581399 findmyorder-0.0.8/findmyorder/__init__.py
--rw-r--r--   0        0        0      219 2023-04-23 13:51:27.929402 findmyorder-0.0.8/findmyorder/config.py
--rw-r--r--   0        0        0      231 2023-04-23 13:51:27.929402 findmyorder-0.0.8/findmyorder/core.toml
--rw-r--r--   0        0        0     2592 2023-04-23 13:51:27.929402 findmyorder-0.0.8/findmyorder/main.py
--rw-r--r--   0        0        0      962 2023-04-23 13:51:28.581399 findmyorder-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2199 1970-01-01 00:00:00.000000 findmyorder-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-23 14:03:54.167185 findmyorder-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1426 2023-04-23 14:03:54.167185 findmyorder-0.0.9/README.md
+-rw-r--r--   0        0        0      103 2023-04-23 14:03:54.923196 findmyorder-0.0.9/findmyorder/__init__.py
+-rw-r--r--   0        0        0      219 2023-04-23 14:03:54.167185 findmyorder-0.0.9/findmyorder/config.py
+-rw-r--r--   0        0        0      206 2023-04-23 14:03:54.167185 findmyorder-0.0.9/findmyorder/core.toml
+-rw-r--r--   0        0        0     2578 2023-04-23 14:03:54.167185 findmyorder-0.0.9/findmyorder/main.py
+-rw-r--r--   0        0        0      962 2023-04-23 14:03:54.923196 findmyorder-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2199 1970-01-01 00:00:00.000000 findmyorder-0.0.9/PKG-INFO
```

### Comparing `findmyorder-0.0.8/LICENSE` & `findmyorder-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `findmyorder-0.0.8/README.md` & `findmyorder-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `findmyorder-0.0.8/findmyorder/main.py` & `findmyorder-0.0.9/findmyorder/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import asyncio, logging, re
 from datetime import datetime
 
 
 
 from findmyorder import __version__
-from findmyorder.config import settings
+from config import settings
 
 # import pyparsing as pp
 
 # from translate import Translator
 # translator = Translator(to_lang="en")
 
 
@@ -20,26 +20,26 @@
         #self.logger.debug(f"find my order Logger:  {self.logger} on {__name__} version: {__version__}")
        # translation = translator.translate("ACHETER")
         
     def search(self,
                message_to_parse: str = None,
                ):
       try:
-        print(settings.fmo_identifier)
-        myDict = settings.fmo_identifier
+        print(settings.FMO_IDENTIFIER)
+        myDict = settings.FMO_IDENTIFIER
 
         for word in myDict:
             self.logger.debug(f"Loop check {word}")
             if re.search(word, message_to_parse):
               self.logger.debug(f"found {word} in {message_to_parse}")
               return True
         self.logger.debug(f"no word identified in {message_to_parse}")
         return False
       except Exception as e:
-        self.logger.debug(f"error identify {e}")
+        self.logger.debug(f"error search {e}")
         return False
 
     # def identify(self,
     #            mystring: str = None,
     #            ):
     #     order_format = self.identify_order_format(mystring)
     #     order_data = self.identify_order_element(mystring)
```

### Comparing `findmyorder-0.0.8/pyproject.toml` & `findmyorder-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "findmyorder"
-version = "0.0.8"
+version = "0.0.9"
 description = "A python package to identify and parse order for trade execution."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["trading", "order", "trade","buy","sell"]
```

### Comparing `findmyorder-0.0.8/PKG-INFO` & `findmyorder-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findmyorder
-Version: 0.0.8
+Version: 0.0.9
 Summary: A python package to identify and parse order for trade execution.
 License: MIT
 Keywords: trading,order,trade,buy,sell
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

