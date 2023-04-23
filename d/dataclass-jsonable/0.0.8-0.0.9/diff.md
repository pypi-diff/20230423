# Comparing `tmp/dataclass-jsonable-0.0.8.tar.gz` & `tmp/dataclass-jsonable-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataclass-jsonable-0.0.8.tar", last modified: Mon Aug 15 07:27:50 2022, max compression
+gzip compressed data, was "dataclass-jsonable-0.0.9.tar", last modified: Mon Aug 15 08:21:50 2022, max compression
```

## Comparing `dataclass-jsonable-0.0.8.tar` & `dataclass-jsonable-0.0.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 hit9       (501) staff       (20)        0 2022-08-15 07:27:50.864677 dataclass-jsonable-0.0.8/
--rw-r--r--   0 hit9       (501) staff       (20)     1539 2022-08-11 15:42:12.000000 dataclass-jsonable-0.0.8/LICENSE-BSD3
--rw-r--r--   0 hit9       (501) staff       (20)      600 2022-08-11 14:27:41.000000 dataclass-jsonable-0.0.8/MANIFEST.in
--rw-r--r--   0 hit9       (501) staff       (20)    11772 2022-08-15 07:27:50.864111 dataclass-jsonable-0.0.8/PKG-INFO
--rw-r--r--   0 hit9       (501) staff       (20)     8557 2022-08-15 06:59:36.000000 dataclass-jsonable-0.0.8/README.md
-drwxr-xr-x   0 hit9       (501) staff       (20)        0 2022-08-15 07:27:50.863126 dataclass-jsonable-0.0.8/dataclass_jsonable/
--rw-r--r--   0 hit9       (501) staff       (20)    14269 2022-08-15 07:26:43.000000 dataclass-jsonable-0.0.8/dataclass_jsonable/__init__.py
--rw-r--r--   0 hit9       (501) staff       (20)        0 2022-08-09 02:53:50.000000 dataclass-jsonable-0.0.8/dataclass_jsonable/py.typed
-drwxr-xr-x   0 hit9       (501) staff       (20)        0 2022-08-15 07:27:50.863388 dataclass-jsonable-0.0.8/dataclass_jsonable.egg-info/
--rw-r--r--   0 hit9       (501) staff       (20)      102 2022-08-15 07:27:50.000000 dataclass-jsonable-0.0.8/dataclass_jsonable.egg-info/SOURCES.txt
--rw-r--r--   0 hit9       (501) staff       (20)       38 2022-08-15 07:27:50.865116 dataclass-jsonable-0.0.8/setup.cfg
--rw-r--r--   0 hit9       (501) staff       (20)      590 2022-08-15 07:27:07.000000 dataclass-jsonable-0.0.8/setup.py
+drwxr-xr-x   0 hit9       (501) staff       (20)        0 2022-08-15 08:21:50.650889 dataclass-jsonable-0.0.9/
+-rw-r--r--   0 hit9       (501) staff       (20)     1539 2022-08-11 15:42:12.000000 dataclass-jsonable-0.0.9/LICENSE-BSD3
+-rw-r--r--   0 hit9       (501) staff       (20)      600 2022-08-11 14:27:41.000000 dataclass-jsonable-0.0.9/MANIFEST.in
+-rw-r--r--   0 hit9       (501) staff       (20)    12594 2022-08-15 08:21:50.650373 dataclass-jsonable-0.0.9/PKG-INFO
+-rw-r--r--   0 hit9       (501) staff       (20)     9203 2022-08-15 08:20:40.000000 dataclass-jsonable-0.0.9/README.md
+drwxr-xr-x   0 hit9       (501) staff       (20)        0 2022-08-15 08:21:50.648375 dataclass-jsonable-0.0.9/dataclass_jsonable/
+-rw-r--r--   0 hit9       (501) staff       (20)    15056 2022-08-15 08:12:26.000000 dataclass-jsonable-0.0.9/dataclass_jsonable/__init__.py
+-rw-r--r--   0 hit9       (501) staff       (20)        0 2022-08-09 02:53:50.000000 dataclass-jsonable-0.0.9/dataclass_jsonable/py.typed
+drwxr-xr-x   0 hit9       (501) staff       (20)        0 2022-08-15 08:21:50.649843 dataclass-jsonable-0.0.9/dataclass_jsonable.egg-info/
+-rw-r--r--   0 hit9       (501) staff       (20)      102 2022-08-15 08:21:50.000000 dataclass-jsonable-0.0.9/dataclass_jsonable.egg-info/SOURCES.txt
+-rw-r--r--   0 hit9       (501) staff       (20)       38 2022-08-15 08:21:50.651137 dataclass-jsonable-0.0.9/setup.cfg
+-rw-r--r--   0 hit9       (501) staff       (20)      590 2022-08-15 08:21:02.000000 dataclass-jsonable-0.0.9/setup.py
```

### Comparing `dataclass-jsonable-0.0.8/LICENSE-BSD3` & `dataclass-jsonable-0.0.9/LICENSE-BSD3`

 * *Files identical despite different names*

### Comparing `dataclass-jsonable-0.0.8/MANIFEST.in` & `dataclass-jsonable-0.0.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `dataclass-jsonable-0.0.8/PKG-INFO` & `dataclass-jsonable-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataclass-jsonable
-Version: 0.0.8
+Version: 0.0.9
 Summary: Simple and flexible conversions between dataclasses and jsonable dictionaries.
 Home-page: https://github.com/hit9/dataclass-jsonable
 Author: hit9
 Author-email: hit9@icloud.com
 License: BSD
 Description: # dataclass-jsonable
         
@@ -225,14 +225,24 @@
            ```python
            @dataclass
            class Person(J):
                attr: str = field(metadata={"j": json_options(name="new_attr")})
            Person(attr="value").json() # => {"new_attr": "value"}
            ```
         
+          And more, we can use a function to specific a custom dictionary key.
+          This may be convenient to work with class-level `__default_json_options__` attribute (check it below).
+        
+          ```python
+          @dataclass
+          class Obj(J):
+              simple_value: int = field(metadata={"j": json_options(name_converter=to_camel_case)})
+          Obj(simple_value=1).json()  # => {"simpleValue": 1}
+          ```
+        
         * Omit a field if its value is empty:
         
            ```python
            @dataclass
            class Book(J):
                name: str = field(metadata={"j": json_options(omitempty=True)})
            Book(name="").json() # => {}
@@ -352,14 +362,26 @@
         
               a: Optional[int] = None
               b: Optional[str] = None
         
           Obj(b="b").json() # => {'b': 'b'}
           ````
         
+          ```python
+          @dataclass
+          class Obj(J):
+              __default_json_options__ = json_options(name_converter=to_camel_case)
+        
+              status_code: int
+              simple_value: str
+        
+          Obj2(status_code=1, simple_value="simple").json()
+          # => {"statusCode": 1, "simpleValue": "simple"}
+          ```
+        
         ## License
         
         BSD.
         
 Keywords: dataclasses,json,jsonable
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `dataclass-jsonable-0.0.8/README.md` & `dataclass-jsonable-0.0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -217,14 +217,24 @@
    ```python
    @dataclass
    class Person(J):
        attr: str = field(metadata={"j": json_options(name="new_attr")})
    Person(attr="value").json() # => {"new_attr": "value"}
    ```
 
+  And more, we can use a function to specific a custom dictionary key.
+  This may be convenient to work with class-level `__default_json_options__` attribute (check it below).
+
+  ```python
+  @dataclass
+  class Obj(J):
+      simple_value: int = field(metadata={"j": json_options(name_converter=to_camel_case)})
+  Obj(simple_value=1).json()  # => {"simpleValue": 1}
+  ```
+
 * Omit a field if its value is empty:
 
    ```python
    @dataclass
    class Book(J):
        name: str = field(metadata={"j": json_options(omitempty=True)})
    Book(name="").json() # => {}
@@ -344,10 +354,22 @@
 
       a: Optional[int] = None
       b: Optional[str] = None
 
   Obj(b="b").json() # => {'b': 'b'}
   ````
 
+  ```python
+  @dataclass
+  class Obj(J):
+      __default_json_options__ = json_options(name_converter=to_camel_case)
+
+      status_code: int
+      simple_value: str
+
+  Obj2(status_code=1, simple_value="simple").json()
+  # => {"statusCode": 1, "simpleValue": "simple"}
+  ```
+
 ## License
 
 BSD.
```

### Comparing `dataclass-jsonable-0.0.8/dataclass_jsonable/__init__.py` & `dataclass-jsonable-0.0.9/dataclass_jsonable/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 """
 
 from dataclasses import dataclass
 from datetime import datetime, timedelta
 from decimal import Decimal
 from enum import Enum
 from types import MappingProxyType
-from typing import Any, Callable, Dict, Optional, TypeVar, Union, get_type_hints
+from typing import Any, Callable, Dict, Optional, Tuple, TypeVar, Union, get_type_hints
 
 __all__ = ("json_options", "JSONAble", "JSON", "J")
 
 # Any value, in short.
 V = Any
 
 # Jsonable dataclasses, bound to JSONAble.
@@ -32,25 +32,33 @@
 # Function that tests a value.
 # Returns a bool and accepts a given argument.
 Tester = Callable[[V], bool]
 
 # Jsonable dictionary.
 JSON = Dict[str, V]
 
+# Function that converts a field's name.
+NameConverter = Callable[[str], str]
+
 
 @dataclass(frozen=True)
 class json_options:
     """Field-level options to override the default conversion behavior.
     For each option, leaving `None` means not-set.
     """
 
     # Custom key to be mapping in the dictionary.
     # Uses the name of this field by default.
     name: Optional[str] = None
 
+    # A function that returns a custom key to be mapping in the dictionary.
+    # This option is similar to option `name`, but it's a function rather than a string.
+    # If the option `name` is set the same time, prefers `name` over `name_converter`.
+    name_converter: Optional[NameConverter] = None
+
     # Omit this field if it has an empty value, defaults to False.
     # This option is only about encoding.
     omitempty: Optional[bool] = None
 
     # Function to test whether a value can be called "empty".
     # Defaults to `lambda x: not x`.
     omitempty_tester: Optional[Tester] = None
@@ -280,15 +288,15 @@
 
             if options.omitempty:
                 omitempty_tester = options.omitempty_tester or _default_omitempty_tester
                 if omitempty_tester(v):
                     continue
 
             # Key in dictionary `d`.
-            k = options.name or name
+            k = _util_get_field_key(name, options)
 
             # Encode.
             encoder = options.encoder or self.get_encoder(t)
             d[k] = encoder(v)
 
         return d
 
@@ -301,15 +309,15 @@
 
         for name, f in cls.__dataclass_fields__.items():
             t = cls._get_typing_hint_by_field(f)
 
             options = cls._get_json_options(f)
 
             # Key in dictionary.
-            k = options.name or name
+            k = _util_get_field_key(name, options)
 
             if options.skip:
                 continue
 
             v = None
 
             if k not in d:
@@ -388,7 +396,19 @@
 
 
 def _replace_mapping_proxy(m: MappingProxyType, kwds) -> MappingProxyType:
     """Copy a MappingProxyType `m`, and update it with `kwds`."""
     d = dict(m)
     d.update(**kwds)
     return MappingProxyType(d)
+
+
+def _util_get_field_key(name: str, options: json_options) -> str:
+    """A util function returns the `key` in target dictionary.
+    :param name: the field's name.
+    :param options: the json_options for this field.
+    """
+    if options.name:
+        return options.name
+    elif options.name_converter:
+        return options.name_converter(name)
+    return name
```

### Comparing `dataclass-jsonable-0.0.8/setup.py` & `dataclass-jsonable-0.0.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup  # type: ignore
 
 setup(
     name="dataclass-jsonable",
-    version="0.0.8",
+    version="0.0.9",
     author="hit9",
     author_email="hit9@icloud.com",
     description="Simple and flexible conversions between dataclasses and jsonable dictionaries.",
     license="BSD",
     keywords="dataclasses,json,jsonable",
     url="https://github.com/hit9/dataclass-jsonable",
     packages=["dataclass_jsonable"],
```

