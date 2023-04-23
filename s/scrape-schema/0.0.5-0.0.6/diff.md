# Comparing `tmp/scrape_schema-0.0.5.tar.gz` & `tmp/scrape_schema-0.0.6.tar.gz`

## Comparing `scrape_schema-0.0.5.tar` & `scrape_schema-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 scrape_schema-0.0.5/scrape_schema/__init__.py
--rw-r--r--   0        0        0    18686 2020-02-02 00:00:00.000000 scrape_schema-0.0.5/scrape_schema/base.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 scrape_schema-0.0.5/scrape_schema/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scrape_schema-0.0.5/scrape_schema/callbacks/__init__.py
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 scrape_schema-0.0.5/scrape_schema/callbacks/slax.py
--rw-r--r--   0        0        0     5184 2020-02-02 00:00:00.000000 scrape_schema-0.0.5/scrape_schema/callbacks/soup.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 scrape_schema-0.0.5/scrape_schema/factory/__init__.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 scrape_schema-0.0.5/scrape_schema/fields/__init__.py
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 scrape_schema-0.0.5/scrape_schema/fields/nested.py
--rw-r--r--   0        0        0     6111 2020-02-02 00:00:00.000000 scrape_schema-0.0.5/scrape_schema/fields/regex.py
--rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 scrape_schema-0.0.5/scrape_schema/fields/slax.py
--rw-r--r--   0        0        0     5020 2020-02-02 00:00:00.000000 scrape_schema-0.0.5/scrape_schema/fields/soup.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 scrape_schema-0.0.5/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 scrape_schema-0.0.5/LICENSE
--rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 scrape_schema-0.0.5/README.md
--rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 scrape_schema-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     5166 2020-02-02 00:00:00.000000 scrape_schema-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 scrape_schema-0.0.6/scrape_schema/__init__.py
+-rw-r--r--   0        0        0    19602 2020-02-02 00:00:00.000000 scrape_schema-0.0.6/scrape_schema/base.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 scrape_schema-0.0.6/scrape_schema/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scrape_schema-0.0.6/scrape_schema/callbacks/__init__.py
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 scrape_schema-0.0.6/scrape_schema/callbacks/slax.py
+-rw-r--r--   0        0        0     5184 2020-02-02 00:00:00.000000 scrape_schema-0.0.6/scrape_schema/callbacks/soup.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 scrape_schema-0.0.6/scrape_schema/factory/__init__.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 scrape_schema-0.0.6/scrape_schema/fields/__init__.py
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 scrape_schema-0.0.6/scrape_schema/fields/nested.py
+-rw-r--r--   0        0        0     6111 2020-02-02 00:00:00.000000 scrape_schema-0.0.6/scrape_schema/fields/regex.py
+-rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 scrape_schema-0.0.6/scrape_schema/fields/slax.py
+-rw-r--r--   0        0        0     5020 2020-02-02 00:00:00.000000 scrape_schema-0.0.6/scrape_schema/fields/soup.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 scrape_schema-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 scrape_schema-0.0.6/LICENSE
+-rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 scrape_schema-0.0.6/README.md
+-rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 scrape_schema-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     5166 2020-02-02 00:00:00.000000 scrape_schema-0.0.6/PKG-INFO
```

### Comparing `scrape_schema-0.0.5/scrape_schema/base.py` & `scrape_schema-0.0.6/scrape_schema/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -205,23 +205,49 @@
         """first parser entrypoint
 
         :param markup: parser class object or string. this value can be config in Config class
         :return: first parsed value
         """
         ...
 
+    def extract(self, markup: MARKUP_TYPE, *, type_: Optional[Type] = None) -> Any:
+        """parse markup without BaseSchema Instance
+
+        :param markup: string target
+        :param type_: optional type for type-casting
+        """
+        # TODO add logging
+        if self.Config.parser and not isinstance(markup, self.Config.parser):
+            raise TypeError(
+                f"markup in `{self.__class__.__name__}` "
+                f"should be `{self.Config.parser.__class__.__name__}`,"
+                f"not {type(markup).__name__}"
+            )
+        value = self._parse(markup)
+        if not value:
+            value = self.default
+        if self._is_iterable_and_not_string_value(value):
+            value = self._filter(value)
+        if self.callback:
+            value = self._callback(value)
+        if self.factory:
+            value = self._factory(value)
+        elif type_:
+            value = self._cast_type(type_, value)
+        return value
+
     def __call__(self, instance: BaseSchema, name: str, markup: MARKUP_TYPE) -> Any:
         logger.info(
             "`%s.%s[%s]`. Field attrs: factory=%s, callback=%s, filter_=%s, default=%s",
             instance.__class__.__name__,
             name,
             self.Config.parser or "str",
-            getattr(self.factory, "__name__", None),
-            getattr(self.callback, "__name__", None),
-            getattr(self.filter_, "__name__", None),
+            repr(self.factory),
+            repr(self.callback),
+            repr(self.filter_),
             self.default,
         )
         value = self._parse(markup)
         if not value:
             logger.debug(
                 "`%s.%s` value not found, set default `%s` value",
                 instance.__class__.__name__,
```

### Comparing `scrape_schema-0.0.5/scrape_schema/callbacks/slax.py` & `scrape_schema-0.0.6/scrape_schema/callbacks/slax.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.0.5/scrape_schema/callbacks/soup.py` & `scrape_schema-0.0.6/scrape_schema/callbacks/soup.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.0.5/scrape_schema/fields/nested.py` & `scrape_schema-0.0.6/scrape_schema/fields/nested.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.0.5/scrape_schema/fields/regex.py` & `scrape_schema-0.0.6/scrape_schema/fields/regex.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.0.5/scrape_schema/fields/slax.py` & `scrape_schema-0.0.6/scrape_schema/fields/slax.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.0.5/scrape_schema/fields/soup.py` & `scrape_schema-0.0.6/scrape_schema/fields/soup.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.0.5/.gitignore` & `scrape_schema-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.0.5/LICENSE` & `scrape_schema-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.0.5/README.md` & `scrape_schema-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.0.5/pyproject.toml` & `scrape_schema-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.0.5/PKG-INFO` & `scrape_schema-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrape-schema
-Version: 0.0.5
+Version: 0.0.6
 Summary: A library for converting any text (xml, html, plain text, stdout, etc) to python datatypes
 Project-URL: Documentation, https://github.com/vypivshiy/scrape-schema#readme
 Project-URL: Issues, https://github.com/vypivshiy/scrape-schema/issues
 Project-URL: Source, https://github.com/vypivshiy/scrape-schema
 Project-URL: Examples, https://github.com/vypivshiy/scrape-schema/examples
 Author: vypivshiy
 License-Expression: MIT
```

