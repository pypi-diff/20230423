# Comparing `tmp/findmyorder-0.0.7.tar.gz` & `tmp/findmyorder-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findmyorder-0.0.7.tar", max compression
+gzip compressed data, was "findmyorder-0.0.8.tar", max compression
```

## Comparing `findmyorder-0.0.7.tar` & `findmyorder-0.0.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-04-23 13:38:26.794031 findmyorder-0.0.7/LICENSE
--rw-r--r--   0        0        0     1426 2023-04-23 13:38:26.794031 findmyorder-0.0.7/README.md
--rw-r--r--   0        0        0      103 2023-04-23 13:38:27.530042 findmyorder-0.0.7/findmyorder/__init__.py
--rw-r--r--   0        0        0      219 2023-04-23 13:38:26.794031 findmyorder-0.0.7/findmyorder/config.py
--rw-r--r--   0        0        0      204 2023-04-23 13:38:26.794031 findmyorder-0.0.7/findmyorder/core.toml
--rw-r--r--   0        0        0     2592 2023-04-23 13:38:26.794031 findmyorder-0.0.7/findmyorder/main.py
--rw-r--r--   0        0        0      962 2023-04-23 13:38:27.530042 findmyorder-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     2199 1970-01-01 00:00:00.000000 findmyorder-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-23 13:51:27.929402 findmyorder-0.0.8/LICENSE
+-rw-r--r--   0        0        0     1426 2023-04-23 13:51:27.929402 findmyorder-0.0.8/README.md
+-rw-r--r--   0        0        0      103 2023-04-23 13:51:28.581399 findmyorder-0.0.8/findmyorder/__init__.py
+-rw-r--r--   0        0        0      219 2023-04-23 13:51:27.929402 findmyorder-0.0.8/findmyorder/config.py
+-rw-r--r--   0        0        0      231 2023-04-23 13:51:27.929402 findmyorder-0.0.8/findmyorder/core.toml
+-rw-r--r--   0        0        0     2592 2023-04-23 13:51:27.929402 findmyorder-0.0.8/findmyorder/main.py
+-rw-r--r--   0        0        0      962 2023-04-23 13:51:28.581399 findmyorder-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2199 1970-01-01 00:00:00.000000 findmyorder-0.0.8/PKG-INFO
```

### Comparing `findmyorder-0.0.7/LICENSE` & `findmyorder-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `findmyorder-0.0.7/README.md` & `findmyorder-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `findmyorder-0.0.7/findmyorder/main.py` & `findmyorder-0.0.8/findmyorder/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,16 +20,16 @@
         #self.logger.debug(f"find my order Logger:  {self.logger} on {__name__} version: {__version__}")
        # translation = translator.translate("ACHETER")
         
     def search(self,
                message_to_parse: str = None,
                ):
       try:
-        print(settings.FMO_IDENTIFIER)
-        myDict = settings.FMO_IDENTIFIER
+        print(settings.fmo_identifier)
+        myDict = settings.fmo_identifier
 
         for word in myDict:
             self.logger.debug(f"Loop check {word}")
             if re.search(word, message_to_parse):
               self.logger.debug(f"found {word} in {message_to_parse}")
               return True
         self.logger.debug(f"no word identified in {message_to_parse}")
```

### Comparing `findmyorder-0.0.7/pyproject.toml` & `findmyorder-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "findmyorder"
-version = "0.0.7"
+version = "0.0.8"
 description = "A python package to identify and parse order for trade execution."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["trading", "order", "trade","buy","sell"]
```

### Comparing `findmyorder-0.0.7/PKG-INFO` & `findmyorder-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findmyorder
-Version: 0.0.7
+Version: 0.0.8
 Summary: A python package to identify and parse order for trade execution.
 License: MIT
 Keywords: trading,order,trade,buy,sell
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

