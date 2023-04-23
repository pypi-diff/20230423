# Comparing `tmp/lib-dzne-tsv-0.1.5.tar.gz` & `tmp/lib-dzne-tsv-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib-dzne-tsv-0.1.5.tar", last modified: Fri Apr 21 21:04:12 2023, max compression
+gzip compressed data, was "lib-dzne-tsv-0.1.6.tar", last modified: Sun Apr 23 18:22:45 2023, max compression
```

## Comparing `lib-dzne-tsv-0.1.5.tar` & `lib-dzne-tsv-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-04-21 21:04:12.142330 lib-dzne-tsv-0.1.5/
--rw-r--r--   0 base      (1001) base      (1001)     1066 2023-03-01 20:28:52.000000 lib-dzne-tsv-0.1.5/LICENSE
--rw-rw-r--   0 base      (1001) base      (1001)     1472 2023-04-21 21:04:12.142330 lib-dzne-tsv-0.1.5/PKG-INFO
--rw-rw-r--   0 base      (1001) base      (1001)      522 2023-04-21 21:00:03.000000 lib-dzne-tsv-0.1.5/pyproject.toml
--rw-r--r--   0 base      (1001) base      (1001)       38 2023-04-21 21:04:12.142330 lib-dzne-tsv-0.1.5/setup.cfg
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-04-21 21:04:12.142330 lib-dzne-tsv-0.1.5/src/
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-04-21 21:04:12.142330 lib-dzne-tsv-0.1.5/src/lib_dzne_tsv/
--rw-rw-r--   0 base      (1001) base      (1001)     5436 2023-04-21 20:50:00.000000 lib-dzne-tsv-0.1.5/src/lib_dzne_tsv/__init__.py
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-04-21 21:04:12.142330 lib-dzne-tsv-0.1.5/src/lib_dzne_tsv.egg-info/
--rw-rw-r--   0 base      (1001) base      (1001)     1472 2023-04-21 21:04:12.000000 lib-dzne-tsv-0.1.5/src/lib_dzne_tsv.egg-info/PKG-INFO
--rw-rw-r--   0 base      (1001) base      (1001)      260 2023-04-21 21:04:12.000000 lib-dzne-tsv-0.1.5/src/lib_dzne_tsv.egg-info/SOURCES.txt
--rw-rw-r--   0 base      (1001) base      (1001)        1 2023-04-21 21:04:12.000000 lib-dzne-tsv-0.1.5/src/lib_dzne_tsv.egg-info/dependency_links.txt
--rw-rw-r--   0 base      (1001) base      (1001)       14 2023-04-21 21:04:12.000000 lib-dzne-tsv-0.1.5/src/lib_dzne_tsv.egg-info/requires.txt
--rw-rw-r--   0 base      (1001) base      (1001)       13 2023-04-21 21:04:12.000000 lib-dzne-tsv-0.1.5/src/lib_dzne_tsv.egg-info/top_level.txt
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-04-23 18:22:45.518881 lib-dzne-tsv-0.1.6/
+-rw-r--r--   0 base      (1001) base      (1001)     1066 2023-03-01 20:28:52.000000 lib-dzne-tsv-0.1.6/LICENSE
+-rw-rw-r--   0 base      (1001) base      (1001)     1472 2023-04-23 18:22:45.518881 lib-dzne-tsv-0.1.6/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)      522 2023-04-23 18:21:46.000000 lib-dzne-tsv-0.1.6/pyproject.toml
+-rw-r--r--   0 base      (1001) base      (1001)       38 2023-04-23 18:22:45.518881 lib-dzne-tsv-0.1.6/setup.cfg
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-04-23 18:22:45.518881 lib-dzne-tsv-0.1.6/src/
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-04-23 18:22:45.518881 lib-dzne-tsv-0.1.6/src/lib_dzne_tsv/
+-rw-rw-r--   0 base      (1001) base      (1001)     5570 2023-04-23 18:17:57.000000 lib-dzne-tsv-0.1.6/src/lib_dzne_tsv/__init__.py
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-04-23 18:22:45.518881 lib-dzne-tsv-0.1.6/src/lib_dzne_tsv.egg-info/
+-rw-rw-r--   0 base      (1001) base      (1001)     1472 2023-04-23 18:22:45.000000 lib-dzne-tsv-0.1.6/src/lib_dzne_tsv.egg-info/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)      260 2023-04-23 18:22:45.000000 lib-dzne-tsv-0.1.6/src/lib_dzne_tsv.egg-info/SOURCES.txt
+-rw-rw-r--   0 base      (1001) base      (1001)        1 2023-04-23 18:22:45.000000 lib-dzne-tsv-0.1.6/src/lib_dzne_tsv.egg-info/dependency_links.txt
+-rw-rw-r--   0 base      (1001) base      (1001)       14 2023-04-23 18:22:45.000000 lib-dzne-tsv-0.1.6/src/lib_dzne_tsv.egg-info/requires.txt
+-rw-rw-r--   0 base      (1001) base      (1001)       13 2023-04-23 18:22:45.000000 lib-dzne-tsv-0.1.6/src/lib_dzne_tsv.egg-info/top_level.txt
```

### Comparing `lib-dzne-tsv-0.1.5/LICENSE` & `lib-dzne-tsv-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lib-dzne-tsv-0.1.5/PKG-INFO` & `lib-dzne-tsv-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-tsv
-Version: 0.1.5
+Version: 0.1.6
 Summary: Libary for handling tsv-data. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `lib-dzne-tsv-0.1.5/pyproject.toml` & `lib-dzne-tsv-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "lib-dzne-tsv"
-version = "0.1.5"
+version = "0.1.6"
 description = "Libary for handling tsv-data. "
 license = { file = "LICENSE" }
 authors = [{ name = "Johannes Horler", email = "johannes.horler@dzne.de" }]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `lib-dzne-tsv-0.1.5/src/lib_dzne_tsv/__init__.py` & `lib-dzne-tsv-0.1.6/src/lib_dzne_tsv/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,18 +38,24 @@
     @classmethod
     def from_handler(cls, handler, **kwargs):
         return cls(handler, **kwargs)
     @classmethod
     def from_stream(cls, stream, **kwargs):
         return cls(cls._handler(stream), **kwargs)
     @_contextlib.contextmanager
+    def _open_file(*, cls, file, **kwargs):
+        with open(file=file, mode=cls._handler.__name__[0]) as stream:
+            yield cls.from_stream(stream, **kwargs)
     @classmethod
     def open_file(cls, file, **kwargs):
-        with open(file=file, mode=cls._mode) as stream:
-            yield cls.from_stream(stream, **kwargs)
+        return cls._open_file(
+            cls=cls,
+            file=file,
+            **kwargs,
+        )
     def __init__(self, handler, *, fieldnames=None):
         cls = type(self)
         if not hasattr(cls, cls._handler_function):
             setattr(cls, cls._handler_function, cls.handle)
         if not hasattr(cls, cls._handler.__name__):
             setattr(cls, cls._handler.__name__, property(cls._get_handler))
             #setattr(cls, cls._handler.__name__, property(cls._get_handler))
@@ -107,15 +113,14 @@
 
 
 
 
 class DictReader(_DictHandler):
     _handler = reader
     _handler_function = '__next__'
-    _mode = 'r'
     def __iter__(self):
         return self
     @property
     def fieldnames(self):
         if (self._fieldnames is None) or (type(self._fieldnames) is int):
             self.fieldnames = self.use_handler()
         return self._fieldnames
@@ -131,15 +136,14 @@
 
 
 
 
 class DictWriter(_DictHandler):
     _handler = writer
     _handler_function = 'writerow'
-    _mode = 'w'
     @property
     def fieldnames(self):
         return self._fieldnames
     @fieldnames.setter
     def fieldnames(self, value):
         self._set_fieldnames(value)
         if type(self._fieldnames) is tuple:
```

### Comparing `lib-dzne-tsv-0.1.5/src/lib_dzne_tsv.egg-info/PKG-INFO` & `lib-dzne-tsv-0.1.6/src/lib_dzne_tsv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-tsv
-Version: 0.1.5
+Version: 0.1.6
 Summary: Libary for handling tsv-data. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

