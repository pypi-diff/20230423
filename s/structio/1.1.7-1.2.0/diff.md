# Comparing `tmp/structio-1.1.7.tar.gz` & `tmp/structio-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "structio-1.1.7.tar", last modified: Thu Apr 20 00:24:59 2023, max compression
+gzip compressed data, was "structio-1.2.0.tar", last modified: Sun Apr 23 00:07:15 2023, max compression
```

## Comparing `structio-1.1.7.tar` & `structio-1.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:24:59.772009 structio-1.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)    13124 2023-04-20 00:24:59.772009 structio-1.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13225 2023-04-20 00:24:41.000000 structio-1.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-20 00:24:41.000000 structio-1.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 00:24:59.772009 structio-1.1.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:24:59.772009 structio-1.1.7/structio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13124 2023-04-20 00:24:59.000000 structio-1.1.7/structio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-20 00:24:59.000000 structio-1.1.7/structio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 00:24:59.000000 structio-1.1.7/structio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-20 00:24:59.000000 structio-1.1.7/structio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11814 2023-04-20 00:24:41.000000 structio-1.1.7/structio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:07:15.913372 structio-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    12866 2023-04-23 00:07:15.913372 structio-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12963 2023-04-23 00:06:41.000000 structio-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-23 00:06:41.000000 structio-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 00:07:15.913372 structio-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:07:15.913372 structio-1.2.0/structio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12866 2023-04-23 00:07:15.000000 structio-1.2.0/structio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-23 00:07:15.000000 structio-1.2.0/structio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 00:07:15.000000 structio-1.2.0/structio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-23 00:07:15.000000 structio-1.2.0/structio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11518 2023-04-23 00:06:41.000000 structio-1.2.0/structio.py
```

### Comparing `structio-1.1.7/PKG-INFO` & `structio-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structio
-Version: 1.1.7
+Version: 1.2.0
 Summary: A Library for unparsing, parsing, and editing binary files
 Project-URL: Homepage, https://github.com/lingeringwillx/StructIO
 Requires-Python: >=3.2
 Description-Content-Type: text/markdown
 
 A small Python library based on the BytesIO object from the standard library, designed to make parsing and editing binary files easier.
 
@@ -108,33 +108,33 @@
 
 Convert bytes object *b* into a string.
 
 **pack_str(string)**
 
 Converts *string* into a bytes object.
 
-**unpack_cstr(b, start=0, ret_len=False)**
+**unpack_cstr(b, start=0)**
 
-Convert bytes object *b* into a string up to the null termination. If *start* is specified, then the bytes object will be converted starting from position *start*. If *ret_len* is True, then a tuple is returned containing both the value and the length of the type.
+Convert bytes object *b* into a string up to the null termination. If *start* is specified, then the bytes object will be converted starting from position *start*. Returns a tuple containing both the value and the length of the type.
 
 **pack_cstr(string)**
 
 Converts *string* into a bytes object representing a null-terminated string.
 
-**unpack_pstr(b, numbytes, endian=None, start=0, ret_len=False)**
+**unpack_pstr(b, numbytes, endian=None, start=0)**
 
-Converts bytes object *b* into a Pascal string. *numbytes* is used to specify how many bytes are used for the string's length in the object. The endian of the length of the string is specified with the *endian* argument. *b* will only be converted up to the length specified in the bytes object. If *start* is specified, then the bytes object will be converted starting from position *start*. If *ret_len* is True, then a tuple is returned containing both the value and the length of the type.
+Converts bytes object *b* into a Pascal string. *numbytes* is used to specify how many bytes are used for the string's length in the object. The endian of the length of the string is specified with the *endian* argument. *b* will only be converted up to the length specified in the bytes object. If *start* is specified, then the bytes object will be converted starting from position *start*. Returns a tuple containing both the value and the length of the type.
 
 **pack_pstr(string, numbytes, endian=None)**
 
 Converts *string* into a bytes object in the Pascal string format. *numbytes* is used to specify how many bytes are used for the string's length. The endian of the length of the string is specified with the *endian* argument.
 
-**unpack_7bint(b, start=0, ret_len=False)**
+**unpack_7bint(b, start=0)**
 
-Converts bytes representing a 7 bit integer (Variable Length Quantity) into an integer.  If *start* is specified, then the bytes object will be converted starting from position *start*. If *ret_len* is True, then a tuple is returned containing both the value and the length of the type.
+Converts bytes representing a 7 bit integer (Variable Length Quantity) into an integer.  If *start* is specified, then the bytes object will be converted starting from position *start*. Returns a tuple containing both the value and the length of the type.
 
 **pack_7bint(number)**
 
 Converts *number* into a 7 bit integer.
 
 -----
 
@@ -323,26 +323,22 @@
 You can add your own types by inheriting from the two base objects:
 
 ```python
 from structio import Struct, StructIO
 
 class ExtendedStruct(Struct):
     def _get_7bstr_len(self, b, start=0):
-        str_len, int_len = self.unpack_7bint(b, start, ret_len=True)
+        str_len, int_len = self.unpack_7bint(b, start)
         return int_len + str_len
         
-    def unpack_7bstr(self, b, start=0, ret_len=False):
-        str_len, int_len = self.unpack_7bint(b, start, ret_len=True)
+    def unpack_7bstr(self, b, start=0):
+        str_len, int_len = self.unpack_7bint(b, start)
         string = self.unpack_str(b[(start + int_len):(start + int_len + str_len)])
+        return string, int_len + str_len
         
-        if ret_len:
-            return string, int_len + str_len
-        else:
-            return string
-            
     def pack_7bstr(self, string):
         b = self.pack_str(string)
         return self.pack_7bint(len(b)) + b
         
 class ExtendedStructIO(StructIO):
     def __init__(self, b=b'', endian='little', struct=ExtendedStruct):
         super().__init__(b, endian, struct=struct)
```

### Comparing `structio-1.1.7/README.md` & `structio-1.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -100,33 +100,33 @@
 
 Convert bytes object *b* into a string.
 
 **pack_str(string)**
 
 Converts *string* into a bytes object.
 
-**unpack_cstr(b, start=0, ret_len=False)**
+**unpack_cstr(b, start=0)**
 
-Convert bytes object *b* into a string up to the null termination. If *start* is specified, then the bytes object will be converted starting from position *start*. If *ret_len* is True, then a tuple is returned containing both the value and the length of the type.
+Convert bytes object *b* into a string up to the null termination. If *start* is specified, then the bytes object will be converted starting from position *start*. Returns a tuple containing both the value and the length of the type.
 
 **pack_cstr(string)**
 
 Converts *string* into a bytes object representing a null-terminated string.
 
-**unpack_pstr(b, numbytes, endian=None, start=0, ret_len=False)**
+**unpack_pstr(b, numbytes, endian=None, start=0)**
 
-Converts bytes object *b* into a Pascal string. *numbytes* is used to specify how many bytes are used for the string's length in the object. The endian of the length of the string is specified with the *endian* argument. *b* will only be converted up to the length specified in the bytes object. If *start* is specified, then the bytes object will be converted starting from position *start*. If *ret_len* is True, then a tuple is returned containing both the value and the length of the type.
+Converts bytes object *b* into a Pascal string. *numbytes* is used to specify how many bytes are used for the string's length in the object. The endian of the length of the string is specified with the *endian* argument. *b* will only be converted up to the length specified in the bytes object. If *start* is specified, then the bytes object will be converted starting from position *start*. Returns a tuple containing both the value and the length of the type.
 
 **pack_pstr(string, numbytes, endian=None)**
 
 Converts *string* into a bytes object in the Pascal string format. *numbytes* is used to specify how many bytes are used for the string's length. The endian of the length of the string is specified with the *endian* argument.
 
-**unpack_7bint(b, start=0, ret_len=False)**
+**unpack_7bint(b, start=0)**
 
-Converts bytes representing a 7 bit integer (Variable Length Quantity) into an integer.  If *start* is specified, then the bytes object will be converted starting from position *start*. If *ret_len* is True, then a tuple is returned containing both the value and the length of the type.
+Converts bytes representing a 7 bit integer (Variable Length Quantity) into an integer.  If *start* is specified, then the bytes object will be converted starting from position *start*. Returns a tuple containing both the value and the length of the type.
 
 **pack_7bint(number)**
 
 Converts *number* into a 7 bit integer.
 
 -----
 
@@ -315,26 +315,22 @@
 You can add your own types by inheriting from the two base objects:
 
 ```python
 from structio import Struct, StructIO
 
 class ExtendedStruct(Struct):
     def _get_7bstr_len(self, b, start=0):
-        str_len, int_len = self.unpack_7bint(b, start, ret_len=True)
+        str_len, int_len = self.unpack_7bint(b, start)
         return int_len + str_len
         
-    def unpack_7bstr(self, b, start=0, ret_len=False):
-        str_len, int_len = self.unpack_7bint(b, start, ret_len=True)
+    def unpack_7bstr(self, b, start=0):
+        str_len, int_len = self.unpack_7bint(b, start)
         string = self.unpack_str(b[(start + int_len):(start + int_len + str_len)])
+        return string, int_len + str_len
         
-        if ret_len:
-            return string, int_len + str_len
-        else:
-            return string
-            
     def pack_7bstr(self, string):
         b = self.pack_str(string)
         return self.pack_7bint(len(b)) + b
         
 class ExtendedStructIO(StructIO):
     def __init__(self, b=b'', endian='little', struct=ExtendedStruct):
         super().__init__(b, endian, struct=struct)
```

### Comparing `structio-1.1.7/structio.egg-info/PKG-INFO` & `structio-1.2.0/structio.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structio
-Version: 1.1.7
+Version: 1.2.0
 Summary: A Library for unparsing, parsing, and editing binary files
 Project-URL: Homepage, https://github.com/lingeringwillx/StructIO
 Requires-Python: >=3.2
 Description-Content-Type: text/markdown
 
 A small Python library based on the BytesIO object from the standard library, designed to make parsing and editing binary files easier.
 
@@ -108,33 +108,33 @@
 
 Convert bytes object *b* into a string.
 
 **pack_str(string)**
 
 Converts *string* into a bytes object.
 
-**unpack_cstr(b, start=0, ret_len=False)**
+**unpack_cstr(b, start=0)**
 
-Convert bytes object *b* into a string up to the null termination. If *start* is specified, then the bytes object will be converted starting from position *start*. If *ret_len* is True, then a tuple is returned containing both the value and the length of the type.
+Convert bytes object *b* into a string up to the null termination. If *start* is specified, then the bytes object will be converted starting from position *start*. Returns a tuple containing both the value and the length of the type.
 
 **pack_cstr(string)**
 
 Converts *string* into a bytes object representing a null-terminated string.
 
-**unpack_pstr(b, numbytes, endian=None, start=0, ret_len=False)**
+**unpack_pstr(b, numbytes, endian=None, start=0)**
 
-Converts bytes object *b* into a Pascal string. *numbytes* is used to specify how many bytes are used for the string's length in the object. The endian of the length of the string is specified with the *endian* argument. *b* will only be converted up to the length specified in the bytes object. If *start* is specified, then the bytes object will be converted starting from position *start*. If *ret_len* is True, then a tuple is returned containing both the value and the length of the type.
+Converts bytes object *b* into a Pascal string. *numbytes* is used to specify how many bytes are used for the string's length in the object. The endian of the length of the string is specified with the *endian* argument. *b* will only be converted up to the length specified in the bytes object. If *start* is specified, then the bytes object will be converted starting from position *start*. Returns a tuple containing both the value and the length of the type.
 
 **pack_pstr(string, numbytes, endian=None)**
 
 Converts *string* into a bytes object in the Pascal string format. *numbytes* is used to specify how many bytes are used for the string's length. The endian of the length of the string is specified with the *endian* argument.
 
-**unpack_7bint(b, start=0, ret_len=False)**
+**unpack_7bint(b, start=0)**
 
-Converts bytes representing a 7 bit integer (Variable Length Quantity) into an integer.  If *start* is specified, then the bytes object will be converted starting from position *start*. If *ret_len* is True, then a tuple is returned containing both the value and the length of the type.
+Converts bytes representing a 7 bit integer (Variable Length Quantity) into an integer.  If *start* is specified, then the bytes object will be converted starting from position *start*. Returns a tuple containing both the value and the length of the type.
 
 **pack_7bint(number)**
 
 Converts *number* into a 7 bit integer.
 
 -----
 
@@ -323,26 +323,22 @@
 You can add your own types by inheriting from the two base objects:
 
 ```python
 from structio import Struct, StructIO
 
 class ExtendedStruct(Struct):
     def _get_7bstr_len(self, b, start=0):
-        str_len, int_len = self.unpack_7bint(b, start, ret_len=True)
+        str_len, int_len = self.unpack_7bint(b, start)
         return int_len + str_len
         
-    def unpack_7bstr(self, b, start=0, ret_len=False):
-        str_len, int_len = self.unpack_7bint(b, start, ret_len=True)
+    def unpack_7bstr(self, b, start=0):
+        str_len, int_len = self.unpack_7bint(b, start)
         string = self.unpack_str(b[(start + int_len):(start + int_len + str_len)])
+        return string, int_len + str_len
         
-        if ret_len:
-            return string, int_len + str_len
-        else:
-            return string
-            
     def pack_7bstr(self, string):
         b = self.pack_str(string)
         return self.pack_7bint(len(b)) + b
         
 class ExtendedStructIO(StructIO):
     def __init__(self, b=b'', endian='little', struct=ExtendedStruct):
         super().__init__(b, endian, struct=struct)
```

### Comparing `structio-1.1.7/structio.py` & `structio-1.2.0/structio.py`

 * *Files 5% similar despite different names*

```diff
@@ -79,68 +79,57 @@
         end = b.find(b'\x00', start)
         
         if end == -1:
             raise ValueError('null termination not found')
             
         return end - start + 1
         
-    def unpack_cstr(self, b, start=0, ret_len=False):
+    def unpack_cstr(self, b, start=0):
         length = self._get_cstr_len(b, start)
         string = self.unpack_str(b[start:(start + length - 1)])
+        return string, length
         
-        if ret_len:
-            return string, length
-        else:
-            return string
-            
     def pack_cstr(self, string):
         return self.pack_str(string) + b'\x00'
         
     def _get_pstr_len(self, b, numbytes, endian=None, start=0):
         return numbytes + self.unpack_int(b[start:(start + numbytes)], endian)
         
-    def unpack_pstr(self, b, numbytes, endian=None, start=0, ret_len=False):
+    def unpack_pstr(self, b, numbytes, endian=None, start=0):
         length = self._get_pstr_len(b, numbytes, endian, start)
         string = self.unpack_str(b[(start + numbytes):(start + length)])
+        return string, length
         
-        if ret_len:
-            return string, length
-        else:
-            return string
-            
     def pack_pstr(self, string, numbytes, endian=None):
         b = self.pack_str(string)
         return self.pack_int(len(b), numbytes, endian) + b
         
     def _get_7bint_len(self, b, start=0):
         i = 0
         while b[start + i] > 127:
             i += 1
             
         return i + 1
         
-    def unpack_7bint(self, b, start=0, ret_len=False):
+    def unpack_7bint(self, b, start=0):
         number = 0
         i = 0
         
-        byte = b[start + i]
+        byte = b[start]
         while byte > 127:
             number |= (byte & 0b01111111) << (7 * i)
             i += 1
             
             byte = b[start + i]
             
         number |= byte << (7 * i)
         length = i + 1
         
-        if ret_len:
-            return number, length
-        else:
-            return number
-            
+        return number, length
+        
     def pack_7bint(self, number):
         b = bytearray()
         
         while number > 127:
             b += self.pack_int(number & 0b01111111 | 0b10000000, 1) 
             number >>= 7
             
@@ -254,15 +243,15 @@
         
         if end == -1:
             raise ValueError('{} not found'.format(bytes_sequence))
             
         return end
         
     def _read(self, unpack_func, unpack_args):
-        value, length = unpack_func(self.getvalue(), *unpack_args, start=self.tell(), ret_len=True)
+        value, length = unpack_func(self.getvalue(), *unpack_args, start=self.tell())
         self.seek(length, 1)
         return value
         
     def _overwrite(self, len_func, len_args, pack_func, pack_args):
         start = self.tell()
         length = len_func(self.getvalue(), *len_args, start=start)
         return self.overwrite(start, start + length, pack_func(*pack_args))
```

