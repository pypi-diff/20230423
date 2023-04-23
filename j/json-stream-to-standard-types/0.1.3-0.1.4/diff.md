# Comparing `tmp/json_stream_to_standard_types-0.1.3.tar.gz` & `tmp/json_stream_to_standard_types-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json_stream_to_standard_types-0.1.3.tar", max compression
+gzip compressed data, was "json_stream_to_standard_types-0.1.4.tar", max compression
```

## Comparing `json_stream_to_standard_types-0.1.3.tar` & `json_stream_to_standard_types-0.1.4.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1041 2023-03-16 17:56:07.162864 json_stream_to_standard_types-0.1.3/README.md
--rw-r--r--   0        0        0     2758 2023-03-16 17:56:07.162864 json_stream_to_standard_types-0.1.3/json_stream_to_standard_types.py
--rw-r--r--   0        0        0      502 2023-03-16 17:56:07.162864 json_stream_to_standard_types-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1654 1970-01-01 00:00:00.000000 json_stream_to_standard_types-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1041 2023-04-23 21:33:12.709740 json_stream_to_standard_types-0.1.4/README.md
+-rw-r--r--   0        0        0     2071 2023-04-23 21:33:12.709740 json_stream_to_standard_types-0.1.4/json_stream_to_standard_types.py
+-rw-r--r--   0        0        0      502 2023-04-23 21:33:12.709740 json_stream_to_standard_types-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1654 1970-01-01 00:00:00.000000 json_stream_to_standard_types-0.1.4/PKG-INFO
```

### Comparing `json_stream_to_standard_types-0.1.3/README.md` & `json_stream_to_standard_types-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `json_stream_to_standard_types-0.1.3/json_stream_to_standard_types.py` & `json_stream_to_standard_types-0.1.4/json_stream_to_standard_types.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,39 +3,14 @@
 from json_stream.base import StreamingJSONList, StreamingJSONObject
 
 
 class Context:
     LIST = 1
     DICT = 2
 
-def to_standard_types1(x):
-    if isinstance(x, StreamingJSONList):
-        return [ to_standard_types(y) for y in x ]
-    elif isinstance(x, StreamingJSONObject):
-        return { k: to_standard_types(v) for k, v in x.items() }
-    else:
-        return x
-
-class UnlimitedRecursor(ABC):
-    def __call__(self):
-        pass
-
-    @abstractmethod
-    def run(self, *args, **kwargs):
-        pass
-
-
-class ToStandardTypes(UnlimitedRecursor):
-    def run(self, x):
-        if isinstance(x, StreamingJSONList):
-            return [ self(y) for y in x ]
-        elif isinstance(x, StreamingJSONObject):
-            return { k: self(v) for k, v in x.items() }
-        else:
-            return x
 
 def to_standard_types(x):
     in_stack, out_stack = deque(), deque()
     if isinstance(x, StreamingJSONList):
         in_stack.append((Context.LIST, iter(x)))
         output = []
     elif isinstance(x, StreamingJSONObject):
```

### Comparing `json_stream_to_standard_types-0.1.3/PKG-INFO` & `json_stream_to_standard_types-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-stream-to-standard-types
-Version: 0.1.3
+Version: 0.1.4
 Summary: Convert json-stream objects to standard Python dicts and lists
 Author: smheidrich
 Author-email: smheidrich@weltenfunktion.de
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

