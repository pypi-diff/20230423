# Comparing `tmp/PyMemoryEditor-1.4.8.tar.gz` & `tmp/PyMemoryEditor-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyMemoryEditor-1.4.8.tar", last modified: Mon Apr 10 04:50:35 2023, max compression
+gzip compressed data, was "PyMemoryEditor-1.4.9.tar", last modified: Mon Apr 10 17:02:42 2023, max compression
```

## Comparing `PyMemoryEditor-1.4.8.tar` & `PyMemoryEditor-1.4.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 04:50:35.264084 PyMemoryEditor-1.4.8/
--rw-rw-rw-   0        0        0     1110 2023-04-03 04:22:57.000000 PyMemoryEditor-1.4.8/LICENSE
--rw-rw-rw-   0        0        0     4341 2023-04-10 04:50:35.263014 PyMemoryEditor-1.4.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-10 04:50:35.240442 PyMemoryEditor-1.4.8/PyMemoryEditor/
--rw-rw-rw-   0        0        0      445 2023-04-10 04:29:19.000000 PyMemoryEditor-1.4.8/PyMemoryEditor/__init__.py
--rw-rw-rw-   0        0        0     5196 2023-04-10 03:54:13.000000 PyMemoryEditor-1.4.8/PyMemoryEditor/open_process.py
-drwxrwxrwx   0        0        0        0 2023-04-10 04:50:35.247505 PyMemoryEditor-1.4.8/PyMemoryEditor/process/
--rw-rw-rw-   0        0        0     1676 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.8/PyMemoryEditor/process/__init__.py
--rw-rw-rw-   0        0        0      717 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.8/PyMemoryEditor/process/errors.py
--rw-rw-rw-   0        0        0      746 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.8/PyMemoryEditor/process/util.py
-drwxrwxrwx   0        0        0        0 2023-04-10 04:50:35.247505 PyMemoryEditor-1.4.8/PyMemoryEditor/win32/
-drwxrwxrwx   0        0        0        0 2023-04-10 04:50:35.247505 PyMemoryEditor-1.4.8/PyMemoryEditor/win32/enums/
--rw-rw-rw-   0        0        0      320 2023-04-10 03:44:13.000000 PyMemoryEditor-1.4.8/PyMemoryEditor/win32/enums/__init__.py
--rw-rw-rw-   0        0        0     2449 2023-04-09 23:42:16.000000 PyMemoryEditor-1.4.8/PyMemoryEditor/win32/enums/memory_allocation_states.py
--rw-rw-rw-   0        0        0     6600 2023-04-09 23:42:16.000000 PyMemoryEditor-1.4.8/PyMemoryEditor/win32/enums/memory_protections.py
--rw-rw-rw-   0        0        0      537 2023-04-10 03:44:01.000000 PyMemoryEditor-1.4.8/PyMemoryEditor/win32/enums/memory_types.py
--rw-rw-rw-   0        0        0     2681 2023-04-09 23:42:46.000000 PyMemoryEditor-1.4.8/PyMemoryEditor/win32/enums/process_operations.py
--rw-rw-rw-   0        0        0      221 2023-04-10 03:51:01.000000 PyMemoryEditor-1.4.8/PyMemoryEditor/win32/enums/scan_types.py
--rw-rw-rw-   0        0        0      977 2023-04-09 23:41:45.000000 PyMemoryEditor-1.4.8/PyMemoryEditor/win32/enums/standard_access_rights.py
--rw-rw-rw-   0        0        0     7901 2023-04-10 04:29:04.000000 PyMemoryEditor-1.4.8/PyMemoryEditor/win32/functions.py
--rw-rw-rw-   0        0        0     1791 2023-04-09 16:56:11.000000 PyMemoryEditor-1.4.8/PyMemoryEditor/win32/types.py
--rw-rw-rw-   0        0        0      928 2023-04-09 16:07:32.000000 PyMemoryEditor-1.4.8/PyMemoryEditor/win32/util.py
-drwxrwxrwx   0        0        0        0 2023-04-10 04:50:35.247505 PyMemoryEditor-1.4.8/PyMemoryEditor.egg-info/
--rw-rw-rw-   0        0        0     4341 2023-04-10 04:50:35.000000 PyMemoryEditor-1.4.8/PyMemoryEditor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      794 2023-04-10 04:50:35.000000 PyMemoryEditor-1.4.8/PyMemoryEditor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 04:50:35.000000 PyMemoryEditor-1.4.8/PyMemoryEditor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-10 04:50:35.000000 PyMemoryEditor-1.4.8/PyMemoryEditor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-10 04:50:35.000000 PyMemoryEditor-1.4.8/PyMemoryEditor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3072 2023-04-10 04:50:08.000000 PyMemoryEditor-1.4.8/README.md
--rw-rw-rw-   0        0        0       42 2023-04-10 04:50:35.264084 PyMemoryEditor-1.4.8/setup.cfg
--rw-rw-rw-   0        0        0     1727 2023-04-10 01:35:30.000000 PyMemoryEditor-1.4.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 17:02:42.984199 PyMemoryEditor-1.4.9/
+-rw-rw-rw-   0        0        0     1110 2023-04-03 04:22:57.000000 PyMemoryEditor-1.4.9/LICENSE
+-rw-rw-rw-   0        0        0     4447 2023-04-10 17:02:42.984199 PyMemoryEditor-1.4.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-10 17:02:42.903949 PyMemoryEditor-1.4.9/PyMemoryEditor/
+-rw-rw-rw-   0        0        0      445 2023-04-10 13:36:41.000000 PyMemoryEditor-1.4.9/PyMemoryEditor/__init__.py
+-rw-rw-rw-   0        0        0     5196 2023-04-10 03:54:13.000000 PyMemoryEditor-1.4.9/PyMemoryEditor/open_process.py
+drwxrwxrwx   0        0        0        0 2023-04-10 17:02:42.935228 PyMemoryEditor-1.4.9/PyMemoryEditor/process/
+-rw-rw-rw-   0        0        0     1676 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.9/PyMemoryEditor/process/__init__.py
+-rw-rw-rw-   0        0        0      717 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.9/PyMemoryEditor/process/errors.py
+-rw-rw-rw-   0        0        0      746 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.9/PyMemoryEditor/process/util.py
+drwxrwxrwx   0        0        0        0 2023-04-10 17:02:42.942582 PyMemoryEditor-1.4.9/PyMemoryEditor/win32/
+drwxrwxrwx   0        0        0        0 2023-04-10 17:02:42.984199 PyMemoryEditor-1.4.9/PyMemoryEditor/win32/enums/
+-rw-rw-rw-   0        0        0      320 2023-04-10 03:44:13.000000 PyMemoryEditor-1.4.9/PyMemoryEditor/win32/enums/__init__.py
+-rw-rw-rw-   0        0        0     2449 2023-04-09 23:42:16.000000 PyMemoryEditor-1.4.9/PyMemoryEditor/win32/enums/memory_allocation_states.py
+-rw-rw-rw-   0        0        0     6600 2023-04-09 23:42:16.000000 PyMemoryEditor-1.4.9/PyMemoryEditor/win32/enums/memory_protections.py
+-rw-rw-rw-   0        0        0      537 2023-04-10 03:44:01.000000 PyMemoryEditor-1.4.9/PyMemoryEditor/win32/enums/memory_types.py
+-rw-rw-rw-   0        0        0     2681 2023-04-09 23:42:46.000000 PyMemoryEditor-1.4.9/PyMemoryEditor/win32/enums/process_operations.py
+-rw-rw-rw-   0        0        0      320 2023-04-10 17:00:43.000000 PyMemoryEditor-1.4.9/PyMemoryEditor/win32/enums/scan_types.py
+-rw-rw-rw-   0        0        0      977 2023-04-09 23:41:45.000000 PyMemoryEditor-1.4.9/PyMemoryEditor/win32/enums/standard_access_rights.py
+-rw-rw-rw-   0        0        0     8301 2023-04-10 17:00:43.000000 PyMemoryEditor-1.4.9/PyMemoryEditor/win32/functions.py
+-rw-rw-rw-   0        0        0     1791 2023-04-09 16:56:11.000000 PyMemoryEditor-1.4.9/PyMemoryEditor/win32/types.py
+-rw-rw-rw-   0        0        0      928 2023-04-09 16:07:32.000000 PyMemoryEditor-1.4.9/PyMemoryEditor/win32/util.py
+drwxrwxrwx   0        0        0        0 2023-04-10 17:02:42.919609 PyMemoryEditor-1.4.9/PyMemoryEditor.egg-info/
+-rw-rw-rw-   0        0        0     4447 2023-04-10 17:02:42.000000 PyMemoryEditor-1.4.9/PyMemoryEditor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      794 2023-04-10 17:02:42.000000 PyMemoryEditor-1.4.9/PyMemoryEditor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 17:02:42.000000 PyMemoryEditor-1.4.9/PyMemoryEditor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-10 17:02:42.000000 PyMemoryEditor-1.4.9/PyMemoryEditor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-10 17:02:42.000000 PyMemoryEditor-1.4.9/PyMemoryEditor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3178 2023-04-10 16:36:02.000000 PyMemoryEditor-1.4.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-10 17:02:42.984199 PyMemoryEditor-1.4.9/setup.cfg
+-rw-rw-rw-   0        0        0     1727 2023-04-10 01:35:30.000000 PyMemoryEditor-1.4.9/setup.py
```

### Comparing `PyMemoryEditor-1.4.8/LICENSE` & `PyMemoryEditor-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.8/PKG-INFO` & `PyMemoryEditor-1.4.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyMemoryEditor
-Version: 1.4.8
+Version: 1.4.9
 Summary: A Python library to edit and track memory of Windows processes (32 bits and 64 bits).
 Home-page: https://github.com/JeanExtreme002/PyMemoryEditor
 Author: Jean Loui Bernard Silva de Jesus
 License: MIT
 Keywords: memory virtual writer reader read write override address pointer edit editor process win32 api cheat scan scanner debug trainer
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
@@ -72,18 +72,15 @@
 You can look up a value in memory and get the address of all matches, like this:
 ```
 for address process.search_by_value(int, 4, target_value):
     print("Found address:", address)
 ```
 
 ## Choosing the comparison method used for scanning:
-There are three options to scan the memory:
-- EXACT_VALUE
-- BIGGER_THAN
-- SMALLER_THAN
+There are many options to scan the memory. Check all available options in [`ScanTypesEnum`](https://github.com/JeanExtreme002/PyMemoryEditor/blob/master/PyMemoryEditor/win32/enums/scan_types.py).
 
 The default option is `EXACT_VALUE`, but you can change it at `scan_type` parameter:
 ```
 for address process.search_by_value(int, 4, target_value, scan_type = ScanTypesEnum.BIGGER_THAN):
     print("Found address:", address)
 ```
```

### Comparing `PyMemoryEditor-1.4.8/PyMemoryEditor/open_process.py` & `PyMemoryEditor-1.4.9/PyMemoryEditor/open_process.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.8/PyMemoryEditor/process/__init__.py` & `PyMemoryEditor-1.4.9/PyMemoryEditor/process/__init__.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.8/PyMemoryEditor/process/errors.py` & `PyMemoryEditor-1.4.9/PyMemoryEditor/process/errors.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.8/PyMemoryEditor/process/util.py` & `PyMemoryEditor-1.4.9/PyMemoryEditor/process/util.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.8/PyMemoryEditor/win32/enums/memory_allocation_states.py` & `PyMemoryEditor-1.4.9/PyMemoryEditor/win32/enums/memory_allocation_states.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.8/PyMemoryEditor/win32/enums/memory_protections.py` & `PyMemoryEditor-1.4.9/PyMemoryEditor/win32/enums/memory_protections.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.8/PyMemoryEditor/win32/enums/memory_types.py` & `PyMemoryEditor-1.4.9/PyMemoryEditor/win32/enums/memory_types.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.8/PyMemoryEditor/win32/enums/process_operations.py` & `PyMemoryEditor-1.4.9/PyMemoryEditor/win32/enums/process_operations.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.8/PyMemoryEditor/win32/enums/standard_access_rights.py` & `PyMemoryEditor-1.4.9/PyMemoryEditor/win32/enums/standard_access_rights.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.8/PyMemoryEditor/win32/functions.py` & `PyMemoryEditor-1.4.9/PyMemoryEditor/win32/functions.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from .enums import MemoryAllocationStatesEnum, MemoryProtectionsEnum, MemoryTypesEnum, ScanTypesEnum
 from .types import MEMORY_BASIC_INFORMATION, SYSTEM_INFO, WNDENUMPROC
 from .util import get_c_type_of
 from typing import Generator, Optional, Tuple, Type, TypeVar, Union
 
 import ctypes
 import ctypes.wintypes
+import sys
 
 # Load the libraries.
 kernel32 = ctypes.windll.LoadLibrary("kernel32.dll")
 user32 = ctypes.windll.LoadLibrary("user32.dll")
 
 # Set the argtypes to prevent ArgumentError.
 kernel32.VirtualQueryEx.argtypes = (
@@ -143,15 +144,15 @@
         raise ValueError("The type must be bool, int, float, str or bytes.")
 
     # Get the target value as bytes.
     target_value = get_c_type_of(pytype, bufflength)
     target_value.value = value
 
     target_value_bytes = ctypes.cast(ctypes.byref(target_value), ctypes.POINTER(ctypes.c_byte * bufflength))
-    target_value_bytes = bytes(target_value_bytes.contents)
+    target_value_bytes = int.from_bytes(bytes(target_value_bytes.contents), sys.byteorder)
 
     regions = list()
     memory_total = 0
 
     # Get the memory regions, computing the space size.
     for region in GetMemoryRegions(process_handle):
 
@@ -172,20 +173,23 @@
 
         # Get data from the region.
         kernel32.ReadProcessMemory(process_handle, ctypes.c_void_p(address), ctypes.byref(region_data), size, None)
 
         # Walk by the returned bytes, searching for the target value.
         for index in range(size - bufflength):
             data = region_data[index: index + bufflength]
-            data = bytes((ctypes.c_byte * bufflength)(*data))
+            data = int.from_bytes(bytes((ctypes.c_byte * bufflength)(*data)), sys.byteorder)
 
             # Compare the values.
             if scan_type is ScanTypesEnum.EXACT_VALUE and data != target_value_bytes: continue
+            elif scan_type is ScanTypesEnum.DIFFERENT_THAN and data == target_value_bytes: continue
             elif scan_type is ScanTypesEnum.BIGGER_THAN and data <= target_value_bytes: continue
             elif scan_type is ScanTypesEnum.SMALLER_THAN and data >= target_value_bytes: continue
+            elif scan_type is ScanTypesEnum.BIGGER_THAN_OR_EXACT_VALUE and data < target_value_bytes: continue
+            elif scan_type is ScanTypesEnum.SMALLER_THAN_OR_EXACT_VALUE and data > target_value_bytes: continue
 
             found_address = address + index
 
             extra_information = {
                 "memory_total": memory_total,
                 "progress": (checked_memory_size + index) / memory_total,
             }
```

### Comparing `PyMemoryEditor-1.4.8/PyMemoryEditor/win32/types.py` & `PyMemoryEditor-1.4.9/PyMemoryEditor/win32/types.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.8/PyMemoryEditor/win32/util.py` & `PyMemoryEditor-1.4.9/PyMemoryEditor/win32/util.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.8/PyMemoryEditor.egg-info/PKG-INFO` & `PyMemoryEditor-1.4.9/PyMemoryEditor.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyMemoryEditor
-Version: 1.4.8
+Version: 1.4.9
 Summary: A Python library to edit and track memory of Windows processes (32 bits and 64 bits).
 Home-page: https://github.com/JeanExtreme002/PyMemoryEditor
 Author: Jean Loui Bernard Silva de Jesus
 License: MIT
 Keywords: memory virtual writer reader read write override address pointer edit editor process win32 api cheat scan scanner debug trainer
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
@@ -72,18 +72,15 @@
 You can look up a value in memory and get the address of all matches, like this:
 ```
 for address process.search_by_value(int, 4, target_value):
     print("Found address:", address)
 ```
 
 ## Choosing the comparison method used for scanning:
-There are three options to scan the memory:
-- EXACT_VALUE
-- BIGGER_THAN
-- SMALLER_THAN
+There are many options to scan the memory. Check all available options in [`ScanTypesEnum`](https://github.com/JeanExtreme002/PyMemoryEditor/blob/master/PyMemoryEditor/win32/enums/scan_types.py).
 
 The default option is `EXACT_VALUE`, but you can change it at `scan_type` parameter:
 ```
 for address process.search_by_value(int, 4, target_value, scan_type = ScanTypesEnum.BIGGER_THAN):
     print("Found address:", address)
 ```
```

### Comparing `PyMemoryEditor-1.4.8/PyMemoryEditor.egg-info/SOURCES.txt` & `PyMemoryEditor-1.4.9/PyMemoryEditor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.8/README.md` & `PyMemoryEditor-1.4.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -45,18 +45,15 @@
 You can look up a value in memory and get the address of all matches, like this:
 ```
 for address process.search_by_value(int, 4, target_value):
     print("Found address:", address)
 ```
 
 ## Choosing the comparison method used for scanning:
-There are three options to scan the memory:
-- EXACT_VALUE
-- BIGGER_THAN
-- SMALLER_THAN
+There are many options to scan the memory. Check all available options in [`ScanTypesEnum`](https://github.com/JeanExtreme002/PyMemoryEditor/blob/master/PyMemoryEditor/win32/enums/scan_types.py).
 
 The default option is `EXACT_VALUE`, but you can change it at `scan_type` parameter:
 ```
 for address process.search_by_value(int, 4, target_value, scan_type = ScanTypesEnum.BIGGER_THAN):
     print("Found address:", address)
 ```
```

### Comparing `PyMemoryEditor-1.4.8/setup.py` & `PyMemoryEditor-1.4.9/setup.py`

 * *Files identical despite different names*

