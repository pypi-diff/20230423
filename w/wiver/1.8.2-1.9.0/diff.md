# Comparing `tmp/wiver-1.8.2.tar.gz` & `tmp/wiver-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiver-1.8.2.tar", last modified: Sun Dec  5 17:04:59 2021, max compression
+gzip compressed data, was "wiver-1.9.0.tar", last modified: Sun Apr 23 20:01:31 2023, max compression
```

## Comparing `wiver-1.8.2.tar` & `wiver-1.9.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2021-12-05 17:04:59.973352 wiver-1.8.2/
--rw-rw-rw-   0        0        0       65 2021-12-05 16:56:22.000000 wiver-1.8.2/MANIFEST.in
--rw-rw-rw-   0        0        0      181 2021-12-05 17:04:59.957727 wiver-1.8.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2021-12-05 17:04:59.973352 wiver-1.8.2/setup.cfg
--rw-rw-rw-   0        0        0      849 2021-12-05 16:56:22.000000 wiver-1.8.2/setup.py
-drwxrwxrwx   0        0        0        0 2021-12-05 17:04:59.957727 wiver-1.8.2/src/
-drwxrwxrwx   0        0        0        0 2021-12-05 17:04:59.957727 wiver-1.8.2/src/wiver/
--rw-rw-rw-   0        0        0      279 2021-12-05 16:56:22.000000 wiver-1.8.2/src/wiver/__init__.py
--rw-rw-rw-   0        0        0       22 2021-12-05 16:56:22.000000 wiver-1.8.2/src/wiver/_version.py
--rw-rw-rw-   0        0        0    11895 2021-12-05 16:56:22.000000 wiver-1.8.2/src/wiver/run_wiver.py
-drwxrwxrwx   0        0        0        0 2021-12-05 17:04:59.957727 wiver-1.8.2/src/wiver/tests/
--rw-rw-rw-   0        0        0      244 2021-12-05 16:56:22.000000 wiver-1.8.2/src/wiver/tests/__init__.py
--rw-rw-rw-   0        0        0    28831 2021-12-05 16:56:22.000000 wiver-1.8.2/src/wiver/tests/test_wiver.py
--rw-rw-rw-   0        0        0     3309 2021-12-05 16:56:22.000000 wiver-1.8.2/src/wiver/tests/test_wiver_benchmark.py
--rw-rw-rw-   0        0        0  1651912 2021-12-05 17:04:56.000000 wiver-1.8.2/src/wiver/wiver_cython.c
--rw-rw-rw-   0        0        0     3709 2021-12-05 16:56:22.000000 wiver-1.8.2/src/wiver/wiver_cython.pxd
--rw-rw-rw-   0        0        0    19320 2021-12-05 16:56:22.000000 wiver-1.8.2/src/wiver/wiver_cython.pyx
--rw-rw-rw-   0        0        0      189 2021-12-05 16:56:22.000000 wiver-1.8.2/src/wiver/wiver_cython.pyxbld
--rw-rw-rw-   0        0        0    26113 2021-12-05 16:56:22.000000 wiver-1.8.2/src/wiver/wiver_python.py
-drwxrwxrwx   0        0        0        0 2021-12-05 17:04:59.957727 wiver-1.8.2/src/wiver.egg-info/
--rw-rw-rw-   0        0        0      181 2021-12-05 17:04:56.000000 wiver-1.8.2/src/wiver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      516 2021-12-05 17:04:56.000000 wiver-1.8.2/src/wiver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-12-05 17:04:56.000000 wiver-1.8.2/src/wiver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-12-05 17:04:56.000000 wiver-1.8.2/src/wiver.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       30 2021-12-05 17:04:56.000000 wiver-1.8.2/src/wiver.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2021-12-05 17:04:56.000000 wiver-1.8.2/src/wiver.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 20:01:31.360986 wiver-1.9.0/
+-rw-rw-rw-   0        0        0       65 2023-04-23 19:38:33.000000 wiver-1.9.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      111 2023-04-23 20:01:31.360986 wiver-1.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-23 20:01:31.360986 wiver-1.9.0/setup.cfg
+-rw-rw-rw-   0        0        0      849 2023-04-23 19:38:33.000000 wiver-1.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 20:01:31.345361 wiver-1.9.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-23 20:01:31.345361 wiver-1.9.0/src/wiver/
+-rw-rw-rw-   0        0        0       34 2023-04-23 19:38:33.000000 wiver-1.9.0/src/wiver/__init__.py
+-rw-rw-rw-   0        0        0       22 2023-04-23 19:38:33.000000 wiver-1.9.0/src/wiver/_version.py
+-rw-rw-rw-   0        0        0    12367 2023-04-23 19:38:33.000000 wiver-1.9.0/src/wiver/run_wiver.py
+drwxrwxrwx   0        0        0        0 2023-04-23 20:01:31.360986 wiver-1.9.0/src/wiver/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-23 19:38:33.000000 wiver-1.9.0/src/wiver/tests/__init__.py
+-rw-rw-rw-   0        0        0    28824 2023-04-23 19:38:33.000000 wiver-1.9.0/src/wiver/tests/test_wiver.py
+-rw-rw-rw-   0        0        0     3309 2023-04-23 19:38:33.000000 wiver-1.9.0/src/wiver/tests/test_wiver_benchmark.py
+-rw-rw-rw-   0        0        0  1668098 2023-04-23 20:01:28.000000 wiver-1.9.0/src/wiver/wiver_cython.c
+-rw-rw-rw-   0        0        0     3709 2023-04-23 19:38:33.000000 wiver-1.9.0/src/wiver/wiver_cython.pxd
+-rw-rw-rw-   0        0        0    19320 2023-04-23 19:38:33.000000 wiver-1.9.0/src/wiver/wiver_cython.pyx
+-rw-rw-rw-   0        0        0      189 2023-04-23 19:38:33.000000 wiver-1.9.0/src/wiver/wiver_cython.pyxbld
+-rw-rw-rw-   0        0        0    26113 2023-04-23 19:38:33.000000 wiver-1.9.0/src/wiver/wiver_python.py
+drwxrwxrwx   0        0        0        0 2023-04-23 20:01:31.345361 wiver-1.9.0/src/wiver.egg-info/
+-rw-rw-rw-   0        0        0      111 2023-04-23 20:01:28.000000 wiver-1.9.0/src/wiver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      516 2023-04-23 20:01:28.000000 wiver-1.9.0/src/wiver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 20:01:28.000000 wiver-1.9.0/src/wiver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-23 20:01:28.000000 wiver-1.9.0/src/wiver.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       30 2023-04-23 20:01:28.000000 wiver-1.9.0/src/wiver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-23 20:01:28.000000 wiver-1.9.0/src/wiver.egg-info/top_level.txt
```

### Comparing `wiver-1.8.2/setup.py` & `wiver-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `wiver-1.8.2/src/wiver/run_wiver.py` & `wiver-1.9.0/src/wiver/run_wiver.py`

 * *Files 6% similar despite different names*

```diff
@@ -405,28 +405,47 @@
     connection:
         An open Database Connection
     """
     fn = wiver_files['results']
     wiver.read_data('results', fn)
     df = wiver.calc_starting_and_ending_trips()
     df.to_sql(name='wiver', con=connection, if_exists='replace')
+    connection.close()
 
     sheetname = 'data'
-    # write to existing excel-file
-    if os.path.isfile(starting_ending_trips_file):
-        book = load_workbook(starting_ending_trips_file)
-        with pd.ExcelWriter(starting_ending_trips_file, engine='openpyxl') as writer:
-            writer.book = book
-            #  overwrite the sheet if exists
-            if sheetname in book.sheetnames:
-                writer.book.remove(writer.book[sheetname])
-            df.to_excel(writer, sheet_name=sheetname)
-    # otherwise create a new xlsx-file
-    else:
-        df.to_excel(starting_ending_trips_file, sheet_name=sheetname)
+    #check if filepath is writable or if there is an opened file
+    i = 0
+    fn0, ext = os.path.splitext(starting_ending_trips_file)
+    while True:
+        if os.path.exists(starting_ending_trips_file):
+            try:
+                with open(starting_ending_trips_file, 'a') as f:
+                    assert f.writable()
+            except (PermissionError, AssertionError):
+                # file exist but is not writable
+                i += 1
+                starting_ending_trips_file = f'{fn0}_{i}{ext}'
+            else:
+                # file exist bus is writable
+                mode = 'a'
+                break
+        else:
+            # file does not exist yet
+            mode = 'w'
+            break
+
+    kwargs = {}
+    if mode == 'a':
+        kwargs['if_sheet_exists'] = 'replace'
+    with pd.ExcelWriter(starting_ending_trips_file,
+                        engine='openpyxl',
+                        mode=mode,
+                        **kwargs) as writer:
+
+        df.to_excel(writer, sheet_name=sheetname)
 
 
 if __name__ == '__main__':
     parser = ArgumentParser(description="Commercial Trip Model Wiver")
     parser.add_argument('-f', '--folder', dest='project_folder',
                         help='Project folder',
                         required=True)
```

### Comparing `wiver-1.8.2/src/wiver/tests/test_wiver.py` & `wiver-1.9.0/src/wiver/tests/test_wiver.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from typing import Dict
 
 import numpy as np
 import orca
 from wiver.wiver_python import (WIVER, InvalidWiverInputData,
                                 DestinationChoiceError, DataConsistencyError)
 import wiver.run_wiver
-from netCDF4 import __hdf5libversion__
+from h5py.version import hdf5_version
 
 
 @pytest.fixture(scope='class', params=range(2))
 def group(request) -> int:
     """
     different values for groups
     """
@@ -57,15 +57,15 @@
     """return a tempdir managed by pytest"""
     return tmpdir_factory.mktemp('Wiver').strpath
 
 
 @pytest.fixture(scope='module',
                 params=['Wiver',
                         pytest.param('ÄÖÜß', marks=pytest.mark.xfail(
-                                     __hdf5libversion__ < '1.12',
+                                     hdf5_version < '1.16',
                             reason='Bug in HDF5'))])
 def result_folder(request, folder: str) -> str:
     """Temp folder to store the results"""
     result_folder = os.path.join(folder, f'results_{request.param}')
     os.makedirs(result_folder, exist_ok=True)
     return result_folder
```

### Comparing `wiver-1.8.2/src/wiver/tests/test_wiver_benchmark.py` & `wiver-1.9.0/src/wiver/tests/test_wiver_benchmark.py`

 * *Files identical despite different names*

### Comparing `wiver-1.8.2/src/wiver/wiver_cython.c` & `wiver-1.9.0/src/wiver/wiver_cython.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-/* Generated by Cython 0.29.24 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "C:\\Miniconda37-x64\\envs\\test-environment\\lib\\site-packages\\numpy\\core\\include\\numpy\\arrayobject.h",
-            "C:\\Miniconda37-x64\\envs\\test-environment\\lib\\site-packages\\numpy\\core\\include\\numpy\\arrayscalars.h",
-            "C:\\Miniconda37-x64\\envs\\test-environment\\lib\\site-packages\\numpy\\core\\include\\numpy\\ndarrayobject.h",
-            "C:\\Miniconda37-x64\\envs\\test-environment\\lib\\site-packages\\numpy\\core\\include\\numpy\\ndarraytypes.h",
-            "C:\\Miniconda37-x64\\envs\\test-environment\\lib\\site-packages\\numpy\\core\\include\\numpy\\ufuncobject.h"
+            "C:\\Miniconda37-x64\\envs\\test-environment\\Lib\\site-packages\\numpy\\core\\include\\numpy\\arrayobject.h",
+            "C:\\Miniconda37-x64\\envs\\test-environment\\Lib\\site-packages\\numpy\\core\\include\\numpy\\arrayscalars.h",
+            "C:\\Miniconda37-x64\\envs\\test-environment\\Lib\\site-packages\\numpy\\core\\include\\numpy\\ndarrayobject.h",
+            "C:\\Miniconda37-x64\\envs\\test-environment\\Lib\\site-packages\\numpy\\core\\include\\numpy\\ndarraytypes.h",
+            "C:\\Miniconda37-x64\\envs\\test-environment\\Lib\\site-packages\\numpy\\core\\include\\numpy\\ufuncobject.h"
         ],
         "extra_compile_args": [
             "/openmp"
         ],
         "include_dirs": [
-            "C:\\Miniconda37-x64\\envs\\test-environment\\lib\\site-packages\\numpy\\core\\include"
+            "C:\\Miniconda37-x64\\envs\\test-environment\\Lib\\site-packages\\numpy\\core\\include"
         ],
         "name": "wiver.wiver_cython",
         "sources": [
             "src\\wiver\\wiver_cython.pyx"
         ]
     },
     "module_name": "wiver.wiver_cython"
@@ -30,16 +30,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_24"
-#define CYTHON_HEX_VERSION 0x001D18F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -70,14 +70,15 @@
 #ifndef Py_HUGE_VAL
   #define Py_HUGE_VAL HUGE_VAL
 #endif
 #ifdef PYPY_VERSION
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
   #define CYTHON_USE_TYPE_SLOTS 0
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #if PY_VERSION_HEX < 0x03050000
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
@@ -106,18 +107,22 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #undef CYTHON_USE_ASYNC_SLOTS
   #define CYTHON_USE_ASYNC_SLOTS 0
@@ -147,18 +152,67 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
+#elif defined(PY_NOGIL)
+  #define CYTHON_COMPILING_IN_PYPY 0
+  #define CYTHON_COMPILING_IN_PYSTON 0
+  #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 1
+  #ifndef CYTHON_USE_TYPE_SLOTS
+    #define CYTHON_USE_TYPE_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYTYPE_LOOKUP
+  #define CYTHON_USE_PYTYPE_LOOKUP 0
+  #ifndef CYTHON_USE_ASYNC_SLOTS
+    #define CYTHON_USE_ASYNC_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYLIST_INTERNALS
+  #define CYTHON_USE_PYLIST_INTERNALS 0
+  #ifndef CYTHON_USE_UNICODE_INTERNALS
+    #define CYTHON_USE_UNICODE_INTERNALS 1
+  #endif
+  #undef CYTHON_USE_UNICODE_WRITER
+  #define CYTHON_USE_UNICODE_WRITER 0
+  #undef CYTHON_USE_PYLONG_INTERNALS
+  #define CYTHON_USE_PYLONG_INTERNALS 0
+  #ifndef CYTHON_AVOID_BORROWED_REFS
+    #define CYTHON_AVOID_BORROWED_REFS 0
+  #endif
+  #ifndef CYTHON_ASSUME_SAFE_MACROS
+    #define CYTHON_ASSUME_SAFE_MACROS 1
+  #endif
+  #ifndef CYTHON_UNPACK_METHODS
+    #define CYTHON_UNPACK_METHODS 1
+  #endif
+  #undef CYTHON_FAST_THREAD_STATE
+  #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_PYCALL
+  #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
+  #ifndef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 1
+  #endif
+  #undef CYTHON_USE_DICT_VERSIONS
+  #define CYTHON_USE_DICT_VERSIONS 0
+  #undef CYTHON_USE_EXC_INFO_STACK
+  #define CYTHON_USE_EXC_INFO_STACK 0
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYTYPE_LOOKUP
     #define CYTHON_USE_PYTYPE_LOOKUP 0
   #elif !defined(CYTHON_USE_PYTYPE_LOOKUP)
@@ -170,61 +224,72 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
-  #if PY_VERSION_HEX < 0x030300F0
+  #if PY_VERSION_HEX < 0x030300F0 || PY_VERSION_HEX >= 0x030B00A2
     #undef CYTHON_USE_UNICODE_WRITER
     #define CYTHON_USE_UNICODE_WRITER 0
   #elif !defined(CYTHON_USE_UNICODE_WRITER)
     #define CYTHON_USE_UNICODE_WRITER 1
   #endif
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
-  #ifndef CYTHON_FAST_THREAD_STATE
+  #if PY_VERSION_HEX >= 0x030B00A4
+    #undef CYTHON_FAST_THREAD_STATE
+    #define CYTHON_FAST_THREAD_STATE 0
+  #elif !defined(CYTHON_FAST_THREAD_STATE)
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
   #ifndef CYTHON_FAST_PYCALL
-    #define CYTHON_FAST_PYCALL 1
+    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030A0000)
   #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
-  #ifndef CYTHON_USE_EXC_INFO_STACK
+  #if PY_VERSION_HEX >= 0x030B00A4
+    #undef CYTHON_USE_EXC_INFO_STACK
+    #define CYTHON_USE_EXC_INFO_STACK 0
+  #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if CYTHON_USE_PYLONG_INTERNALS
-  #include "longintrepr.h"
+  #if PY_MAJOR_VERSION < 3
+    #include "longintrepr.h"
+  #endif
   #undef SHIFT
   #undef BASE
   #undef MASK
   #ifdef SIZEOF_VOID_P
     enum { __pyx_check_sizeof_voidp = 1 / (int)(SIZEOF_VOID_P == sizeof(void*)) };
   #endif
 #endif
@@ -333,17 +398,76 @@
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
 #else
   #define __Pyx_BUILTIN_MODULE_NAME "builtins"
-#if PY_VERSION_HEX >= 0x030800A4 && PY_VERSION_HEX < 0x030800B2
-  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
-          PyCode_New(a, 0, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
+  #define __Pyx_DefaultClassType PyType_Type
+#if PY_VERSION_HEX >= 0x030B00A1
+    static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int k, int l, int s, int f,
+                                                    PyObject *code, PyObject *c, PyObject* n, PyObject *v,
+                                                    PyObject *fv, PyObject *cell, PyObject* fn,
+                                                    PyObject *name, int fline, PyObject *lnos) {
+        PyObject *kwds=NULL, *argcount=NULL, *posonlyargcount=NULL, *kwonlyargcount=NULL;
+        PyObject *nlocals=NULL, *stacksize=NULL, *flags=NULL, *replace=NULL, *call_result=NULL, *empty=NULL;
+        const char *fn_cstr=NULL;
+        const char *name_cstr=NULL;
+        PyCodeObject* co=NULL;
+        PyObject *type, *value, *traceback;
+        PyErr_Fetch(&type, &value, &traceback);
+        if (!(kwds=PyDict_New())) goto end;
+        if (!(argcount=PyLong_FromLong(a))) goto end;
+        if (PyDict_SetItemString(kwds, "co_argcount", argcount) != 0) goto end;
+        if (!(posonlyargcount=PyLong_FromLong(0))) goto end;
+        if (PyDict_SetItemString(kwds, "co_posonlyargcount", posonlyargcount) != 0) goto end;
+        if (!(kwonlyargcount=PyLong_FromLong(k))) goto end;
+        if (PyDict_SetItemString(kwds, "co_kwonlyargcount", kwonlyargcount) != 0) goto end;
+        if (!(nlocals=PyLong_FromLong(l))) goto end;
+        if (PyDict_SetItemString(kwds, "co_nlocals", nlocals) != 0) goto end;
+        if (!(stacksize=PyLong_FromLong(s))) goto end;
+        if (PyDict_SetItemString(kwds, "co_stacksize", stacksize) != 0) goto end;
+        if (!(flags=PyLong_FromLong(f))) goto end;
+        if (PyDict_SetItemString(kwds, "co_flags", flags) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_code", code) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_consts", c) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_names", n) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_varnames", v) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_freevars", fv) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_cellvars", cell) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_linetable", lnos) != 0) goto end;
+        if (!(fn_cstr=PyUnicode_AsUTF8AndSize(fn, NULL))) goto end;
+        if (!(name_cstr=PyUnicode_AsUTF8AndSize(name, NULL))) goto end;
+        if (!(co = PyCode_NewEmpty(fn_cstr, name_cstr, fline))) goto end;
+        if (!(replace = PyObject_GetAttrString((PyObject*)co, "replace"))) goto cleanup_code_too;
+        if (!(empty = PyTuple_New(0))) goto cleanup_code_too; // unfortunately __pyx_empty_tuple isn't available here
+        if (!(call_result = PyObject_Call(replace, empty, kwds))) goto cleanup_code_too;
+        Py_XDECREF((PyObject*)co);
+        co = (PyCodeObject*)call_result;
+        call_result = NULL;
+        if (0) {
+            cleanup_code_too:
+            Py_XDECREF((PyObject*)co);
+            co = NULL;
+        }
+        end:
+        Py_XDECREF(kwds);
+        Py_XDECREF(argcount);
+        Py_XDECREF(posonlyargcount);
+        Py_XDECREF(kwonlyargcount);
+        Py_XDECREF(nlocals);
+        Py_XDECREF(stacksize);
+        Py_XDECREF(replace);
+        Py_XDECREF(call_result);
+        Py_XDECREF(empty);
+        if (type) {
+            PyErr_Restore(type, value, traceback);
+        }
+        return co;
+    }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
 #ifndef Py_TPFLAGS_CHECKTYPES
@@ -449,35 +573,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -573,18 +697,18 @@
   #ifndef PyUnicode_InternFromString
     #define PyUnicode_InternFromString(s) PyUnicode_FromString(s)
   #endif
 #endif
 #if PY_VERSION_HEX < 0x030200A4
   typedef long Py_hash_t;
   #define __Pyx_PyInt_FromHash_t PyInt_FromLong
-  #define __Pyx_PyInt_AsHash_t   PyInt_AsLong
+  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsHash_t
 #else
   #define __Pyx_PyInt_FromHash_t PyInt_FromSsize_t
-  #define __Pyx_PyInt_AsHash_t   PyInt_AsSsize_t
+  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsSsize_t
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define __Pyx_PyMethod_New(func, self, klass) ((self) ? ((void)(klass), PyMethod_New(func, self)) : __Pyx_NewRef(func))
 #else
   #define __Pyx_PyMethod_New(func, self, klass) PyMethod_New(func, self, klass)
 #endif
 #if CYTHON_USE_ASYNC_SLOTS
@@ -601,16 +725,18 @@
     typedef struct {
         unaryfunc am_await;
         unaryfunc am_aiter;
         unaryfunc am_anext;
     } __Pyx_PyAsyncMethodsStruct;
 #endif
 
-#if defined(WIN32) || defined(MS_WINDOWS)
-  #define _USE_MATH_DEFINES
+#if defined(_WIN32) || defined(WIN32) || defined(MS_WINDOWS)
+  #if !defined(_USE_MATH_DEFINES)
+    #define _USE_MATH_DEFINES
+  #endif
 #endif
 #include <math.h>
 #ifdef NAN
 #define __PYX_NAN() ((float) NAN)
 #else
 static CYTHON_INLINE float __PYX_NAN() {
   float value;
@@ -747,14 +873,15 @@
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
 #define __Pyx_PySequence_Tuple(obj)\
     (likely(PyTuple_CheckExact(obj)) ? __Pyx_NewRef(obj) : PySequence_Tuple(obj))
 static CYTHON_INLINE Py_ssize_t __Pyx_PyIndex_AsSsize_t(PyObject*);
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t);
+static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject*);
 #if CYTHON_ASSUME_SAFE_MACROS
 #define __pyx_PyFloat_AsDouble(x) (PyFloat_CheckExact(x) ? PyFloat_AS_DOUBLE(x) : PyFloat_AsDouble(x))
 #else
 #define __pyx_PyFloat_AsDouble(x) PyFloat_AsDouble(x)
 #endif
 #define __pyx_PyFloat_AsFloat(x) ((float) __pyx_PyFloat_AsDouble(x))
 #if PY_MAJOR_VERSION >= 3
@@ -915,51 +1042,47 @@
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* Atomics.proto */
 #include <pythread.h>
 #ifndef CYTHON_ATOMICS
     #define CYTHON_ATOMICS 1
 #endif
+#define __PYX_CYTHON_ATOMICS_ENABLED() CYTHON_ATOMICS
 #define __pyx_atomic_int_type int
-#if CYTHON_ATOMICS && __GNUC__ >= 4 && (__GNUC_MINOR__ > 1 ||\
-                    (__GNUC_MINOR__ == 1 && __GNUC_PATCHLEVEL >= 2)) &&\
-                    !defined(__i386__)
-    #define __pyx_atomic_incr_aligned(value, lock) __sync_fetch_and_add(value, 1)
-    #define __pyx_atomic_decr_aligned(value, lock) __sync_fetch_and_sub(value, 1)
+#if CYTHON_ATOMICS && (__GNUC__ >= 5 || (__GNUC__ == 4 &&\
+                    (__GNUC_MINOR__ > 1 ||\
+                    (__GNUC_MINOR__ == 1 && __GNUC_PATCHLEVEL__ >= 2))))
+    #define __pyx_atomic_incr_aligned(value) __sync_fetch_and_add(value, 1)
+    #define __pyx_atomic_decr_aligned(value) __sync_fetch_and_sub(value, 1)
     #ifdef __PYX_DEBUG_ATOMICS
         #warning "Using GNU atomics"
     #endif
-#elif CYTHON_ATOMICS && defined(_MSC_VER) && 0
-    #include <Windows.h>
+#elif CYTHON_ATOMICS && defined(_MSC_VER) && CYTHON_COMPILING_IN_NOGIL
+    #include <intrin.h>
     #undef __pyx_atomic_int_type
-    #define __pyx_atomic_int_type LONG
-    #define __pyx_atomic_incr_aligned(value, lock) InterlockedIncrement(value)
-    #define __pyx_atomic_decr_aligned(value, lock) InterlockedDecrement(value)
+    #define __pyx_atomic_int_type long
+    #pragma intrinsic (_InterlockedExchangeAdd)
+    #define __pyx_atomic_incr_aligned(value) _InterlockedExchangeAdd(value, 1)
+    #define __pyx_atomic_decr_aligned(value) _InterlockedExchangeAdd(value, -1)
     #ifdef __PYX_DEBUG_ATOMICS
         #pragma message ("Using MSVC atomics")
     #endif
-#elif CYTHON_ATOMICS && (defined(__ICC) || defined(__INTEL_COMPILER)) && 0
-    #define __pyx_atomic_incr_aligned(value, lock) _InterlockedIncrement(value)
-    #define __pyx_atomic_decr_aligned(value, lock) _InterlockedDecrement(value)
-    #ifdef __PYX_DEBUG_ATOMICS
-        #warning "Using Intel atomics"
-    #endif
 #else
     #undef CYTHON_ATOMICS
     #define CYTHON_ATOMICS 0
     #ifdef __PYX_DEBUG_ATOMICS
         #warning "Not using atomics"
     #endif
 #endif
 typedef volatile __pyx_atomic_int_type __pyx_atomic_int;
 #if CYTHON_ATOMICS
     #define __pyx_add_acquisition_count(memview)\
-             __pyx_atomic_incr_aligned(__pyx_get_slice_count_pointer(memview), memview->lock)
+             __pyx_atomic_incr_aligned(__pyx_get_slice_count_pointer(memview))
     #define __pyx_sub_acquisition_count(memview)\
-            __pyx_atomic_decr_aligned(__pyx_get_slice_count_pointer(memview), memview->lock)
+            __pyx_atomic_decr_aligned(__pyx_get_slice_count_pointer(memview))
 #else
     #define __pyx_add_acquisition_count(memview)\
             __pyx_add_acquisition_count_locked(__pyx_get_slice_count_pointer(memview), memview->lock)
     #define __pyx_sub_acquisition_count(memview)\
             __pyx_sub_acquisition_count_locked(__pyx_get_slice_count_pointer(memview), memview->lock)
 #endif
 
@@ -996,195 +1119,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":690
+/* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":691
+/* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":692
+/* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":693
+/* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":697
+/* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":698
+/* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":699
+/* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":700
+/* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":704
+/* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":705
+/* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":714
+/* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":715
+/* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":716
+/* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":718
+/* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":719
+/* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":720
+/* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":722
+/* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":723
+/* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":725
+/* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":726
+/* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":727
+/* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1343,42 +1466,42 @@
 struct __pyx_obj_12cythonarrays_12array_shapes_ArrayShapes;
 struct __pyx_obj_5wiver_12wiver_cython__WIVER;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":729
+/* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":730
+/* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":731
+/* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":733
+/* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1814,15 +1937,15 @@
   __pyx_t_12cythonarrays_11numpy_types_ARRAY_3D_d _trips_mij;
   __pyx_t_12cythonarrays_11numpy_types_ARRAY_4D_d _trips_msij;
   __pyx_t_12cythonarrays_11numpy_types_ARRAY_2D_d _p_destination_tj;
   __pyx_t_12cythonarrays_11numpy_types_ARRAY_3D_d _p_links_tij;
 };
 
 
-/* "View.MemoryView":105
+/* "View.MemoryView":106
  * 
  * @cname("__pyx_array")
  * cdef class array:             # <<<<<<<<<<<<<<
  * 
  *     cdef:
  */
 struct __pyx_array_obj {
@@ -1839,28 +1962,28 @@
   PyObject *_format;
   void (*callback_free_data)(void *);
   int free_data;
   int dtype_is_object;
 };
 
 
-/* "View.MemoryView":279
+/* "View.MemoryView":280
  * 
  * @cname('__pyx_MemviewEnum')
  * cdef class Enum(object):             # <<<<<<<<<<<<<<
  *     cdef object name
  *     def __init__(self, name):
  */
 struct __pyx_MemviewEnum_obj {
   PyObject_HEAD
   PyObject *name;
 };
 
 
-/* "View.MemoryView":330
+/* "View.MemoryView":331
  * 
  * @cname('__pyx_memoryview')
  * cdef class memoryview(object):             # <<<<<<<<<<<<<<
  * 
  *     cdef object obj
  */
 struct __pyx_memoryview_obj {
@@ -1875,15 +1998,15 @@
   Py_buffer view;
   int flags;
   int dtype_is_object;
   __Pyx_TypeInfo *typeinfo;
 };
 
 
-/* "View.MemoryView":965
+/* "View.MemoryView":967
  * 
  * @cname('__pyx_memoryviewslice')
  * cdef class _memoryviewslice(memoryview):             # <<<<<<<<<<<<<<
  *     "Internal class for passing memoryview slices to Python"
  * 
  */
 struct __pyx_memoryviewslice_obj {
@@ -1936,29 +2059,29 @@
   PyObject *(*aggregate_to_modes)(struct __pyx_obj_5wiver_12wiver_cython__WIVER *, int __pyx_skip_dispatch);
   PyObject *(*calc_mean_distance)(struct __pyx_obj_5wiver_12wiver_cython__WIVER *, int __pyx_skip_dispatch);
   PyObject *(*calc_mean_distance_mode)(struct __pyx_obj_5wiver_12wiver_cython__WIVER *, int __pyx_skip_dispatch);
 };
 static struct __pyx_vtabstruct_5wiver_12wiver_cython__WIVER *__pyx_vtabptr_5wiver_12wiver_cython__WIVER;
 
 
-/* "View.MemoryView":105
+/* "View.MemoryView":106
  * 
  * @cname("__pyx_array")
  * cdef class array:             # <<<<<<<<<<<<<<
  * 
  *     cdef:
  */
 
 struct __pyx_vtabstruct_array {
   PyObject *(*get_memview)(struct __pyx_array_obj *);
 };
 static struct __pyx_vtabstruct_array *__pyx_vtabptr_array;
 
 
-/* "View.MemoryView":330
+/* "View.MemoryView":331
  * 
  * @cname('__pyx_memoryview')
  * cdef class memoryview(object):             # <<<<<<<<<<<<<<
  * 
  *     cdef object obj
  */
 
@@ -1970,15 +2093,15 @@
   PyObject *(*setitem_indexed)(struct __pyx_memoryview_obj *, PyObject *, PyObject *);
   PyObject *(*convert_item_to_object)(struct __pyx_memoryview_obj *, char *);
   PyObject *(*assign_item_from_object)(struct __pyx_memoryview_obj *, char *, PyObject *);
 };
 static struct __pyx_vtabstruct_memoryview *__pyx_vtabptr_memoryview;
 
 
-/* "View.MemoryView":965
+/* "View.MemoryView":967
  * 
  * @cname('__pyx_memoryviewslice')
  * cdef class _memoryviewslice(memoryview):             # <<<<<<<<<<<<<<
  *     "Internal class for passing memoryview slices to Python"
  * 
  */
 
@@ -2121,41 +2244,66 @@
 #ifndef CYTHON_PROFILE_REUSE_FRAME
   #define CYTHON_PROFILE_REUSE_FRAME 0
 #endif
 #if CYTHON_PROFILE || CYTHON_TRACE
   #include "compile.h"
   #include "frameobject.h"
   #include "traceback.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
   #if CYTHON_PROFILE_REUSE_FRAME
     #define CYTHON_FRAME_MODIFIER static
     #define CYTHON_FRAME_DEL(frame)
   #else
     #define CYTHON_FRAME_MODIFIER
     #define CYTHON_FRAME_DEL(frame) Py_CLEAR(frame)
   #endif
   #define __Pyx_TraceDeclarations\
       static PyCodeObject *__pyx_frame_code = NULL;\
       CYTHON_FRAME_MODIFIER PyFrameObject *__pyx_frame = NULL;\
       int __Pyx_use_tracing = 0;
   #define __Pyx_TraceFrameInit(codeobj)\
       if (codeobj) __pyx_frame_code = (PyCodeObject*) codeobj;
-#if PY_VERSION_HEX >= 0x030a00b1
+#if PY_VERSION_HEX >= 0x030b00a2
   #define __Pyx_IsTracing(tstate, check_tracing, check_funcs)\
      (unlikely((tstate)->cframe->use_tracing) &&\
          (!(check_tracing) || !(tstate)->tracing) &&\
          (!(check_funcs) || (tstate)->c_profilefunc || (CYTHON_TRACE && (tstate)->c_tracefunc)))
-  #define __Pyx_SetTracing(tstate, enable)\
-      (tstate)->cframe->use_tracing = (enable)
+  #define __Pyx_EnterTracing(tstate) PyThreadState_EnterTracing(tstate)
+  #define __Pyx_LeaveTracing(tstate) PyThreadState_LeaveTracing(tstate)
+#elif PY_VERSION_HEX >= 0x030a00b1
+  #define __Pyx_IsTracing(tstate, check_tracing, check_funcs)\
+     (unlikely((tstate)->cframe->use_tracing) &&\
+         (!(check_tracing) || !(tstate)->tracing) &&\
+         (!(check_funcs) || (tstate)->c_profilefunc || (CYTHON_TRACE && (tstate)->c_tracefunc)))
+  #define __Pyx_EnterTracing(tstate)\
+      do { tstate->tracing++; tstate->cframe->use_tracing = 0; } while (0)
+  #define __Pyx_LeaveTracing(tstate)\
+      do {\
+          tstate->tracing--;\
+          tstate->cframe->use_tracing = ((CYTHON_TRACE && tstate->c_tracefunc != NULL)\
+                                 || tstate->c_profilefunc != NULL);\
+      } while (0)
 #else
   #define __Pyx_IsTracing(tstate, check_tracing, check_funcs)\
      (unlikely((tstate)->use_tracing) &&\
          (!(check_tracing) || !(tstate)->tracing) &&\
          (!(check_funcs) || (tstate)->c_profilefunc || (CYTHON_TRACE && (tstate)->c_tracefunc)))
-  #define __Pyx_SetTracing(tstate, enable)\
-      (tstate)->use_tracing = (enable)
+  #define __Pyx_EnterTracing(tstate)\
+      do { tstate->tracing++; tstate->use_tracing = 0; } while (0)
+  #define __Pyx_LeaveTracing(tstate)\
+      do {\
+          tstate->tracing--;\
+          tstate->use_tracing = ((CYTHON_TRACE && tstate->c_tracefunc != NULL)\
+                                         || tstate->c_profilefunc != NULL);\
+      } while (0)
 #endif
   #ifdef WITH_THREAD
   #define __Pyx_TraceCall(funcname, srcfile, firstlineno, nogil, goto_error)\
   if (nogil) {\
       if (CYTHON_TRACE_NOGIL) {\
           PyThreadState *tstate;\
           PyGILState_STATE state = PyGILState_Ensure();\
@@ -2182,41 +2330,37 @@
       }\
   }
   #endif
   #define __Pyx_TraceException()\
   if (likely(!__Pyx_use_tracing)); else {\
       PyThreadState* tstate = __Pyx_PyThreadState_Current;\
       if (__Pyx_IsTracing(tstate, 0, 1)) {\
-          tstate->tracing++;\
-          __Pyx_SetTracing(tstate, 0);\
+          __Pyx_EnterTracing(tstate);\
           PyObject *exc_info = __Pyx_GetExceptionTuple(tstate);\
           if (exc_info) {\
               if (CYTHON_TRACE && tstate->c_tracefunc)\
                   tstate->c_tracefunc(\
                       tstate->c_traceobj, __pyx_frame, PyTrace_EXCEPTION, exc_info);\
               tstate->c_profilefunc(\
                   tstate->c_profileobj, __pyx_frame, PyTrace_EXCEPTION, exc_info);\
               Py_DECREF(exc_info);\
           }\
-          __Pyx_SetTracing(tstate, 1);\
-          tstate->tracing--;\
+          __Pyx_LeaveTracing(tstate);\
       }\
   }
   static void __Pyx_call_return_trace_func(PyThreadState *tstate, PyFrameObject *frame, PyObject *result) {
       PyObject *type, *value, *traceback;
       __Pyx_ErrFetchInState(tstate, &type, &value, &traceback);
-      tstate->tracing++;
-      __Pyx_SetTracing(tstate, 0);
+      __Pyx_EnterTracing(tstate);
       if (CYTHON_TRACE && tstate->c_tracefunc)
           tstate->c_tracefunc(tstate->c_traceobj, frame, PyTrace_RETURN, result);
       if (tstate->c_profilefunc)
           tstate->c_profilefunc(tstate->c_profileobj, frame, PyTrace_RETURN, result);
       CYTHON_FRAME_DEL(frame);
-      __Pyx_SetTracing(tstate, 1);
-      tstate->tracing--;
+      __Pyx_LeaveTracing(tstate);
       __Pyx_ErrRestoreInState(tstate, type, value, traceback);
   }
   #ifdef WITH_THREAD
   #define __Pyx_TraceReturn(result, nogil)\
   if (likely(!__Pyx_use_tracing)); else {\
       if (nogil) {\
           if (CYTHON_TRACE_NOGIL) {\
@@ -2255,19 +2399,17 @@
 #endif
 #if CYTHON_TRACE
   static int __Pyx_call_line_trace_func(PyThreadState *tstate, PyFrameObject *frame, int lineno) {
       int ret;
       PyObject *type, *value, *traceback;
       __Pyx_ErrFetchInState(tstate, &type, &value, &traceback);
       __Pyx_PyFrame_SetLineNumber(frame, lineno);
-      tstate->tracing++;
-      __Pyx_SetTracing(tstate, 0);
+      __Pyx_EnterTracing(tstate);
       ret = tstate->c_tracefunc(tstate->c_traceobj, frame, PyTrace_LINE, NULL);
-      __Pyx_SetTracing(tstate, 1);
-      tstate->tracing--;
+      __Pyx_LeaveTracing(tstate);
       if (likely(!ret)) {
           __Pyx_ErrRestoreInState(tstate, type, value, traceback);
       } else {
           Py_XDECREF(type);
           Py_XDECREF(value);
           Py_XDECREF(traceback);
       }
@@ -2353,21 +2495,29 @@
 #define __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs) _PyFunction_FastCallDict(func, args, nargs, kwargs)
 #endif
 #define __Pyx_BUILD_ASSERT_EXPR(cond)\
     (sizeof(char [1 - 2*!(cond)]) - 1)
 #ifndef Py_MEMBER_SIZE
 #define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
 #endif
+#if CYTHON_FAST_PYCALL
   static size_t __pyx_pyframe_localsplus_offset = 0;
   #include "frameobject.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
   #define __Pxy_PyFrame_Initialize_Offsets()\
     ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
      (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
   #define __Pyx_PyFrame_GetLocalsplus(frame)\
     (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
+#endif // CYTHON_FAST_PYCALL
 #endif
 
 /* PyObjectCall.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
 #else
 #define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
@@ -2477,26 +2627,26 @@
 /* ParseKeywords.proto */
 static int __Pyx_ParseOptionalKeywords(PyObject *kwds, PyObject **argnames[],\
     PyObject *kwds2, PyObject *values[], Py_ssize_t num_pos_args,\
     const char* function_name);
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -2553,14 +2703,20 @@
 #else
 #define __Pyx_PyErr_ExceptionMatches(err)  PyErr_ExceptionMatches(err)
 #endif
 
 /* GetAttr3.proto */
 static CYTHON_INLINE PyObject *__Pyx_GetAttr3(PyObject *, PyObject *, PyObject *);
 
+/* PySequenceContains.proto */
+static CYTHON_INLINE int __Pyx_PySequence_ContainsTF(PyObject* item, PyObject* seq, int eq) {
+    int result = PySequence_Contains(seq, item);
+    return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
+}
+
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
 
 /* HasAttr.proto */
@@ -2734,20 +2890,28 @@
 #else
 #define __Pyx_PyObject_GenericGetAttr PyObject_GenericGetAttr
 #endif
 
 /* TypeImport.proto */
 #ifndef __PYX_HAVE_RT_ImportType_proto
 #define __PYX_HAVE_RT_ImportType_proto
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#endif
 enum __Pyx_ImportType_CheckSize {
    __Pyx_ImportType_CheckSize_Error = 0,
    __Pyx_ImportType_CheckSize_Warn = 1,
    __Pyx_ImportType_CheckSize_Ignore = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
 #endif
 
 /* GetVTable.proto */
 static void* __Pyx_GetVtable(PyObject *dict);
 
 /* SetVTable.proto */
 static int __Pyx_SetVtable(PyObject *dict, void *vtable);
@@ -3332,29 +3496,29 @@
 static const char __pyx_k_mean_distance_of_group_n_15_g_3[] = "mean distance of group {n:15} ({g:3}): {d:5.2f} km, {t:7.0f} trips, {td:7.0f} vkm. HomeBased: {dh:5.2f} km, {th:7.0f} trips, {tdh:7.0f} vkm. LinkingTrips: {dl:5.2f} km, {tl:7.0f} trips, {tdl:7.0f} vkm. ";
 static const char __pyx_k_numpy_core_multiarray_failed_to[] = "numpy.core.multiarray failed to import";
 static const char __pyx_k_Buffer_view_does_not_expose_stri[] = "Buffer view does not expose strides";
 static const char __pyx_k_Can_only_create_a_buffer_that_is[] = "Can only create a buffer that is contiguous in memory.";
 static const char __pyx_k_Cannot_assign_to_read_only_memor[] = "Cannot assign to read-only memoryview";
 static const char __pyx_k_Cannot_create_writable_memory_vi[] = "Cannot create writable memory view from read-only memoryview";
 static const char __pyx_k_Empty_shape_tuple_for_cython_arr[] = "Empty shape tuple for cython.array";
-static const char __pyx_k_Incompatible_checksums_s_vs_0xb0[] = "Incompatible checksums (%s vs 0xb068931 = (name))";
-static const char __pyx_k_Incompatible_checksums_s_vs_0xb9[] = "Incompatible checksums (%s vs 0xb9d7a6d = (INF_d, INF_f, NAN_d, NAN_f, NINF_d, NINF_f, _active_g, _balancing_factor_gj, _converged_g, _home_based_trips_gij, _km_ij, _linking_trips_gij, _mean_distance_g, _mean_distance_m, _mode_g, _p_destination_tj, _p_links_tij, _param_dist_g, _return_trips_gij, _savings_param_g, _sector_g, _sink_potential_gj, _source_potential_gh, _stops_per_tour_g, _time_series_ending_trips_gs, _time_series_linking_trips_gs, _time_series_starting_trips_gs, _tour_rates_g, _travel_time_mij, _trips_gij, _trips_gsij, _trips_mij, _trips_msij, _trips_to_destination_gj, _zone_no, n_groups, n_modes, n_sectors, n_threads, n_time_slices, n_zones))";
+static const char __pyx_k_Incompatible_checksums_0x_x_vs_0[] = "Incompatible checksums (0x%x vs (0xb9d7a6d, 0x31b4ce0, 0xa09edd1) = (INF_d, INF_f, NAN_d, NAN_f, NINF_d, NINF_f, _active_g, _balancing_factor_gj, _converged_g, _home_based_trips_gij, _km_ij, _linking_trips_gij, _mean_distance_g, _mean_distance_m, _mode_g, _p_destination_tj, _p_links_tij, _param_dist_g, _return_trips_gij, _savings_param_g, _sector_g, _sink_potential_gj, _source_potential_gh, _stops_per_tour_g, _time_series_ending_trips_gs, _time_series_linking_trips_gs, _time_series_starting_trips_gs, _tour_rates_g, _travel_time_mij, _trips_gij, _trips_gsij, _trips_mij, _trips_msij, _trips_to_destination_gj, _zone_no, n_groups, n_modes, n_sectors, n_threads, n_time_slices, n_zones))";
 static const char __pyx_k_Indirect_dimensions_not_supporte[] = "Indirect dimensions not supported";
 static const char __pyx_k_Invalid_mode_expected_c_or_fortr[] = "Invalid mode, expected 'c' or 'fortran', got %s";
 static const char __pyx_k_No_accessible_destinations_found[] = "No accessible destinations found for group {g} and home zone {h}";
 static const char __pyx_k_No_destinations_cannot_be_linked[] = "No destinations cannot be linked for group {g} and home zone {h} because they is no accessibility between the destinations";
 static const char __pyx_k_Out_of_bounds_on_buffer_access_a[] = "Out of bounds on buffer access (axis %d)";
 static const char __pyx_k_Unable_to_convert_item_to_object[] = "Unable to convert item to object";
 static const char __pyx_k_array_v_should_only_contain_valu[] = "array {v} should only contain values v with 0 <= v < {d}={n},\nbut contains the following invalid values at pos {pos}:\n{val}";
 static const char __pyx_k_assert_data_consistency_of_array[] = "assert_data_consistency_of_array";
 static const char __pyx_k_got_differing_extents_in_dimensi[] = "got differing extents in dimension %d (got %d and %d)";
 static const char __pyx_k_mean_distance_of_mode_m_n_d_0_2f[] = "mean distance of mode {m} ({n}): {d:0.2f}";
 static const char __pyx_k_no_default___reduce___due_to_non[] = "no default __reduce__ due to non-trivial __cinit__";
 static const char __pyx_k_numpy_core_umath_failed_to_impor[] = "numpy.core.umath failed to import";
 static const char __pyx_k_unable_to_allocate_shape_and_str[] = "unable to allocate shape and strides.";
+static const char __pyx_k_Incompatible_checksums_0x_x_vs_0_2[] = "Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))";
 static PyObject *__pyx_n_u_;
 static PyObject *__pyx_n_s_ASCII;
 static PyObject *__pyx_n_s_ArrayProperties;
 static PyObject *__pyx_n_s_ArrayShapes;
 static PyObject *__pyx_kp_s_Buffer_view_does_not_expose_stri;
 static PyObject *__pyx_kp_s_Can_only_create_a_buffer_that_is;
 static PyObject *__pyx_kp_s_Cannot_assign_to_read_only_memor;
@@ -3364,16 +3528,16 @@
 static PyObject *__pyx_kp_s_Data_is_not_consistent_and_coul;
 static PyObject *__pyx_n_s_DestinationChoiceError;
 static PyObject *__pyx_n_s_Ellipsis;
 static PyObject *__pyx_kp_s_Empty_shape_tuple_for_cython_arr;
 static PyObject *__pyx_kp_s_Error_in_destination_choice_mod;
 static PyObject *__pyx_kp_u_Group;
 static PyObject *__pyx_n_s_ImportError;
-static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0xb0;
-static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0xb9;
+static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0;
+static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_2;
 static PyObject *__pyx_n_s_IndexError;
 static PyObject *__pyx_kp_s_Indirect_dimensions_not_supporte;
 static PyObject *__pyx_kp_s_Invalid_mode_expected_c_or_fortr;
 static PyObject *__pyx_kp_s_Invalid_shape_in_axis_d_d;
 static PyObject *__pyx_n_s_MemoryError;
 static PyObject *__pyx_kp_s_MemoryView_of_r_at_0x_x;
 static PyObject *__pyx_kp_s_MemoryView_of_r_object;
@@ -3667,14 +3831,18 @@
 static PyObject *__pyx_tp_new_5wiver_12wiver_cython__WIVER(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_array(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_Enum(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_int_0;
 static PyObject *__pyx_int_1;
+static PyObject *__pyx_int_52120800;
+static PyObject *__pyx_int_112105877;
+static PyObject *__pyx_int_136983863;
+static PyObject *__pyx_int_168422865;
 static PyObject *__pyx_int_184977713;
 static PyObject *__pyx_int_194869869;
 static PyObject *__pyx_int_neg_1;
 static PyObject *__pyx_slice__5;
 static PyObject *__pyx_tuple__6;
 static PyObject *__pyx_tuple__7;
 static PyObject *__pyx_tuple__9;
@@ -3692,25 +3860,27 @@
 static PyObject *__pyx_tuple__21;
 static PyObject *__pyx_tuple__22;
 static PyObject *__pyx_tuple__23;
 static PyObject *__pyx_tuple__24;
 static PyObject *__pyx_tuple__25;
 static PyObject *__pyx_tuple__26;
 static PyObject *__pyx_tuple__27;
-static PyObject *__pyx_tuple__29;
+static PyObject *__pyx_tuple__28;
 static PyObject *__pyx_tuple__30;
 static PyObject *__pyx_tuple__31;
 static PyObject *__pyx_tuple__32;
 static PyObject *__pyx_tuple__33;
 static PyObject *__pyx_tuple__34;
 static PyObject *__pyx_tuple__35;
 static PyObject *__pyx_tuple__36;
 static PyObject *__pyx_tuple__37;
+static PyObject *__pyx_tuple__38;
+static PyObject *__pyx_tuple__39;
 static PyObject *__pyx_codeobj__8;
-static PyObject *__pyx_codeobj__28;
+static PyObject *__pyx_codeobj__29;
 /* Late includes */
 
 /* "wiver/wiver_cython.pyx":40
  * 
  *     @cython.initializedcheck(False)
  *     cpdef char calc_daily_trips(self, long32 g) except -1:             # <<<<<<<<<<<<<<
  *         """
@@ -14527,15 +14697,15 @@
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle__WIVER, (type(self), 0xb9d7a6d, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle__WIVER__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
   __Pyx_TraceLine(17,0,__PYX_ERR(2, 17, __pyx_L1_error))
-  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(2, 17, __pyx_L1_error)
+  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(2, 17, __pyx_L1_error)
   __pyx_t_1 = __pyx_f_5wiver_12wiver_cython___pyx_unpickle__WIVER__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle__WIVER, (type(self), 0xb9d7a6d, state)
@@ -14642,159 +14812,163 @@
 
 static PyObject *__pyx_pf_5wiver_12wiver_cython___pyx_unpickle__WIVER(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_TraceFrameInit(__pyx_codeobj__8)
   __Pyx_RefNannySetupContext("__pyx_unpickle__WIVER", 0);
   __Pyx_TraceCall("__pyx_unpickle__WIVER", __pyx_f[2], 1, 0, __PYX_ERR(2, 1, __pyx_L1_error));
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xb9d7a6d:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xb9d7a6d, 0x31b4ce0, 0xa09edd1):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb9d7a6d = (INF_d, INF_f, NAN_d, NAN_f, NINF_d, NINF_f, _active_g, _balancing_factor_gj, _converged_g, _home_based_trips_gij, _km_ij, _linking_trips_gij, _mean_distance_g, _mean_distance_m, _mode_g, _p_destination_tj, _p_links_tij, _param_dist_g, _return_trips_gij, _savings_param_g, _sector_g, _sink_potential_gj, _source_potential_gh, _stops_per_tour_g, _time_series_ending_trips_gs, _time_series_linking_trips_gs, _time_series_starting_trips_gs, _tour_rates_g, _travel_time_mij, _trips_gij, _trips_gsij, _trips_mij, _trips_msij, _trips_to_destination_gj, _zone_no, n_groups, n_modes, n_sectors, n_threads, n_time_slices, n_zones))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb9d7a6d, 0x31b4ce0, 0xa09edd1) = (INF_d, INF_f, NAN_d, NAN_f, NINF_d, NINF_f, _active_g, _balancing_factor_gj, _converged_g, _home_based_trips_gij, _km_ij, _linking_trips_gij, _mean_distance_g, _mean_distance_m, _mode_g, _p_destination_tj, _p_links_tij, _param_dist_g, _return_trips_gij, _savings_param_g, _sector_g, _sink_potential_gj, _source_potential_gh, _stops_per_tour_g, _time_series_ending_trips_gs, _time_series_linking_trips_gs, _time_series_starting_trips_gs, _tour_rates_g, _travel_time_mij, _trips_gij, _trips_gsij, _trips_mij, _trips_msij, _trips_to_destination_gj, _zone_no, n_groups, n_modes, n_sectors, n_threads, n_time_slices, n_zones))" % __pyx_checksum)
  */
   __Pyx_TraceLine(4,0,__PYX_ERR(2, 4, __pyx_L1_error))
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0xb9d7a6d) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__9, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xb9d7a6d:
+ *     if __pyx_checksum not in (0xb9d7a6d, 0x31b4ce0, 0xa09edd1):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb9d7a6d = (INF_d, INF_f, NAN_d, NAN_f, NINF_d, NINF_f, _active_g, _balancing_factor_gj, _converged_g, _home_based_trips_gij, _km_ij, _linking_trips_gij, _mean_distance_g, _mean_distance_m, _mode_g, _p_destination_tj, _p_links_tij, _param_dist_g, _return_trips_gij, _savings_param_g, _sector_g, _sink_potential_gj, _source_potential_gh, _stops_per_tour_g, _time_series_ending_trips_gs, _time_series_linking_trips_gs, _time_series_starting_trips_gs, _tour_rates_g, _travel_time_mij, _trips_gij, _trips_gsij, _trips_mij, _trips_msij, _trips_to_destination_gj, _zone_no, n_groups, n_modes, n_sectors, n_threads, n_time_slices, n_zones))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb9d7a6d, 0x31b4ce0, 0xa09edd1) = (INF_d, INF_f, NAN_d, NAN_f, NINF_d, NINF_f, _active_g, _balancing_factor_gj, _converged_g, _home_based_trips_gij, _km_ij, _linking_trips_gij, _mean_distance_g, _mean_distance_m, _mode_g, _p_destination_tj, _p_links_tij, _param_dist_g, _return_trips_gij, _savings_param_g, _sector_g, _sink_potential_gj, _source_potential_gh, _stops_per_tour_g, _time_series_ending_trips_gs, _time_series_linking_trips_gs, _time_series_starting_trips_gs, _tour_rates_g, _travel_time_mij, _trips_gij, _trips_gsij, _trips_mij, _trips_msij, _trips_to_destination_gj, _zone_no, n_groups, n_modes, n_sectors, n_threads, n_time_slices, n_zones))" % __pyx_checksum)
  *     __pyx_result = _WIVER.__new__(__pyx_type)
  */
     __Pyx_TraceLine(5,0,__PYX_ERR(2, 5, __pyx_L1_error))
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0xb9d7a6d:
+ *     if __pyx_checksum not in (0xb9d7a6d, 0x31b4ce0, 0xa09edd1):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb9d7a6d = (INF_d, INF_f, NAN_d, NAN_f, NINF_d, NINF_f, _active_g, _balancing_factor_gj, _converged_g, _home_based_trips_gij, _km_ij, _linking_trips_gij, _mean_distance_g, _mean_distance_m, _mode_g, _p_destination_tj, _p_links_tij, _param_dist_g, _return_trips_gij, _savings_param_g, _sector_g, _sink_potential_gj, _source_potential_gh, _stops_per_tour_g, _time_series_ending_trips_gs, _time_series_linking_trips_gs, _time_series_starting_trips_gs, _tour_rates_g, _travel_time_mij, _trips_gij, _trips_gsij, _trips_mij, _trips_msij, _trips_to_destination_gj, _zone_no, n_groups, n_modes, n_sectors, n_threads, n_time_slices, n_zones))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb9d7a6d, 0x31b4ce0, 0xa09edd1) = (INF_d, INF_f, NAN_d, NAN_f, NINF_d, NINF_f, _active_g, _balancing_factor_gj, _converged_g, _home_based_trips_gij, _km_ij, _linking_trips_gij, _mean_distance_g, _mean_distance_m, _mode_g, _p_destination_tj, _p_links_tij, _param_dist_g, _return_trips_gij, _savings_param_g, _sector_g, _sink_potential_gj, _source_potential_gh, _stops_per_tour_g, _time_series_ending_trips_gs, _time_series_linking_trips_gs, _time_series_starting_trips_gs, _tour_rates_g, _travel_time_mij, _trips_gij, _trips_gsij, _trips_mij, _trips_msij, _trips_to_destination_gj, _zone_no, n_groups, n_modes, n_sectors, n_threads, n_time_slices, n_zones))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = _WIVER.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
     __Pyx_TraceLine(6,0,__PYX_ERR(2, 6, __pyx_L1_error))
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0xb9, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(2, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xb9d7a6d:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xb9d7a6d, 0x31b4ce0, 0xa09edd1):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb9d7a6d = (INF_d, INF_f, NAN_d, NAN_f, NINF_d, NINF_f, _active_g, _balancing_factor_gj, _converged_g, _home_based_trips_gij, _km_ij, _linking_trips_gij, _mean_distance_g, _mean_distance_m, _mode_g, _p_destination_tj, _p_links_tij, _param_dist_g, _return_trips_gij, _savings_param_g, _sector_g, _sink_potential_gj, _source_potential_gh, _stops_per_tour_g, _time_series_ending_trips_gs, _time_series_linking_trips_gs, _time_series_starting_trips_gs, _tour_rates_g, _travel_time_mij, _trips_gij, _trips_gsij, _trips_mij, _trips_msij, _trips_to_destination_gj, _zone_no, n_groups, n_modes, n_sectors, n_threads, n_time_slices, n_zones))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb9d7a6d, 0x31b4ce0, 0xa09edd1) = (INF_d, INF_f, NAN_d, NAN_f, NINF_d, NINF_f, _active_g, _balancing_factor_gj, _converged_g, _home_based_trips_gij, _km_ij, _linking_trips_gij, _mean_distance_g, _mean_distance_m, _mode_g, _p_destination_tj, _p_links_tij, _param_dist_g, _return_trips_gij, _savings_param_g, _sector_g, _sink_potential_gj, _source_potential_gh, _stops_per_tour_g, _time_series_ending_trips_gs, _time_series_linking_trips_gs, _time_series_starting_trips_gs, _tour_rates_g, _travel_time_mij, _trips_gij, _trips_gsij, _trips_mij, _trips_msij, _trips_to_destination_gj, _zone_no, n_groups, n_modes, n_sectors, n_threads, n_time_slices, n_zones))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb9d7a6d = (INF_d, INF_f, NAN_d, NAN_f, NINF_d, NINF_f, _active_g, _balancing_factor_gj, _converged_g, _home_based_trips_gij, _km_ij, _linking_trips_gij, _mean_distance_g, _mean_distance_m, _mode_g, _p_destination_tj, _p_links_tij, _param_dist_g, _return_trips_gij, _savings_param_g, _sector_g, _sink_potential_gj, _source_potential_gh, _stops_per_tour_g, _time_series_ending_trips_gs, _time_series_linking_trips_gs, _time_series_starting_trips_gs, _tour_rates_g, _travel_time_mij, _trips_gij, _trips_gsij, _trips_mij, _trips_msij, _trips_to_destination_gj, _zone_no, n_groups, n_modes, n_sectors, n_threads, n_time_slices, n_zones))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb9d7a6d, 0x31b4ce0, 0xa09edd1) = (INF_d, INF_f, NAN_d, NAN_f, NINF_d, NINF_f, _active_g, _balancing_factor_gj, _converged_g, _home_based_trips_gij, _km_ij, _linking_trips_gij, _mean_distance_g, _mean_distance_m, _mode_g, _p_destination_tj, _p_links_tij, _param_dist_g, _return_trips_gij, _savings_param_g, _sector_g, _sink_potential_gj, _source_potential_gh, _stops_per_tour_g, _time_series_ending_trips_gs, _time_series_linking_trips_gs, _time_series_starting_trips_gs, _tour_rates_g, _travel_time_mij, _trips_gij, _trips_gsij, _trips_mij, _trips_msij, _trips_to_destination_gj, _zone_no, n_groups, n_modes, n_sectors, n_threads, n_time_slices, n_zones))" % __pyx_checksum)
  *     __pyx_result = _WIVER.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle__WIVER__set_state(<_WIVER> __pyx_result, __pyx_state)
  */
   __Pyx_TraceLine(7,0,__PYX_ERR(2, 7, __pyx_L1_error))
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_5wiver_12wiver_cython__WIVER), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_5wiver_12wiver_cython__WIVER), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb9d7a6d = (INF_d, INF_f, NAN_d, NAN_f, NINF_d, NINF_f, _active_g, _balancing_factor_gj, _converged_g, _home_based_trips_gij, _km_ij, _linking_trips_gij, _mean_distance_g, _mean_distance_m, _mode_g, _p_destination_tj, _p_links_tij, _param_dist_g, _return_trips_gij, _savings_param_g, _sector_g, _sink_potential_gj, _source_potential_gh, _stops_per_tour_g, _time_series_ending_trips_gs, _time_series_linking_trips_gs, _time_series_starting_trips_gs, _tour_rates_g, _travel_time_mij, _trips_gij, _trips_gsij, _trips_mij, _trips_msij, _trips_to_destination_gj, _zone_no, n_groups, n_modes, n_sectors, n_threads, n_time_slices, n_zones))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb9d7a6d, 0x31b4ce0, 0xa09edd1) = (INF_d, INF_f, NAN_d, NAN_f, NINF_d, NINF_f, _active_g, _balancing_factor_gj, _converged_g, _home_based_trips_gij, _km_ij, _linking_trips_gij, _mean_distance_g, _mean_distance_m, _mode_g, _p_destination_tj, _p_links_tij, _param_dist_g, _return_trips_gij, _savings_param_g, _sector_g, _sink_potential_gj, _source_potential_gh, _stops_per_tour_g, _time_series_ending_trips_gs, _time_series_linking_trips_gs, _time_series_starting_trips_gs, _tour_rates_g, _travel_time_mij, _trips_gij, _trips_gsij, _trips_mij, _trips_msij, _trips_to_destination_gj, _zone_no, n_groups, n_modes, n_sectors, n_threads, n_time_slices, n_zones))" % __pyx_checksum)
  *     __pyx_result = _WIVER.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle__WIVER__set_state(<_WIVER> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   __Pyx_TraceLine(8,0,__PYX_ERR(2, 8, __pyx_L1_error))
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = _WIVER.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle__WIVER__set_state(<_WIVER> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle__WIVER__set_state(_WIVER __pyx_result, tuple __pyx_state):
  */
     __Pyx_TraceLine(9,0,__PYX_ERR(2, 9, __pyx_L1_error))
-    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(2, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_5wiver_12wiver_cython___pyx_unpickle__WIVER__set_state(((struct __pyx_obj_5wiver_12wiver_cython__WIVER *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(2, 9, __pyx_L1_error)
+    __pyx_t_4 = __pyx_f_5wiver_12wiver_cython___pyx_unpickle__WIVER__set_state(((struct __pyx_obj_5wiver_12wiver_cython__WIVER *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb9d7a6d = (INF_d, INF_f, NAN_d, NAN_f, NINF_d, NINF_f, _active_g, _balancing_factor_gj, _converged_g, _home_based_trips_gij, _km_ij, _linking_trips_gij, _mean_distance_g, _mean_distance_m, _mode_g, _p_destination_tj, _p_links_tij, _param_dist_g, _return_trips_gij, _savings_param_g, _sector_g, _sink_potential_gj, _source_potential_gh, _stops_per_tour_g, _time_series_ending_trips_gs, _time_series_linking_trips_gs, _time_series_starting_trips_gs, _tour_rates_g, _travel_time_mij, _trips_gij, _trips_gsij, _trips_mij, _trips_msij, _trips_to_destination_gj, _zone_no, n_groups, n_modes, n_sectors, n_threads, n_time_slices, n_zones))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb9d7a6d, 0x31b4ce0, 0xa09edd1) = (INF_d, INF_f, NAN_d, NAN_f, NINF_d, NINF_f, _active_g, _balancing_factor_gj, _converged_g, _home_based_trips_gij, _km_ij, _linking_trips_gij, _mean_distance_g, _mean_distance_m, _mode_g, _p_destination_tj, _p_links_tij, _param_dist_g, _return_trips_gij, _savings_param_g, _sector_g, _sink_potential_gj, _source_potential_gh, _stops_per_tour_g, _time_series_ending_trips_gs, _time_series_linking_trips_gs, _time_series_starting_trips_gs, _tour_rates_g, _travel_time_mij, _trips_gij, _trips_gsij, _trips_mij, _trips_msij, _trips_to_destination_gj, _zone_no, n_groups, n_modes, n_sectors, n_threads, n_time_slices, n_zones))" % __pyx_checksum)
  *     __pyx_result = _WIVER.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle__WIVER__set_state(<_WIVER> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -14815,18 +14989,18 @@
  * def __pyx_unpickle__WIVER(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("wiver.wiver_cython.__pyx_unpickle__WIVER", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
@@ -15303,15 +15477,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":735
+/* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -15320,32 +15494,32 @@
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
-  __Pyx_TraceCall("PyArray_MultiIterNew1", __pyx_f[3], 735, 0, __PYX_ERR(3, 735, __pyx_L1_error));
+  __Pyx_TraceCall("PyArray_MultiIterNew1", __pyx_f[3], 734, 0, __PYX_ERR(3, 734, __pyx_L1_error));
 
-  /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":736
+  /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
-  __Pyx_TraceLine(736,0,__PYX_ERR(3, 736, __pyx_L1_error))
+  __Pyx_TraceLine(735,0,__PYX_ERR(3, 735, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 736, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":735
+  /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -15357,15 +15531,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":738
+/* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -15374,32 +15548,32 @@
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
-  __Pyx_TraceCall("PyArray_MultiIterNew2", __pyx_f[3], 738, 0, __PYX_ERR(3, 738, __pyx_L1_error));
+  __Pyx_TraceCall("PyArray_MultiIterNew2", __pyx_f[3], 737, 0, __PYX_ERR(3, 737, __pyx_L1_error));
 
-  /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":739
+  /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
-  __Pyx_TraceLine(739,0,__PYX_ERR(3, 739, __pyx_L1_error))
+  __Pyx_TraceLine(738,0,__PYX_ERR(3, 738, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 739, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":738
+  /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -15411,15 +15585,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":741
+/* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -15428,32 +15602,32 @@
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
-  __Pyx_TraceCall("PyArray_MultiIterNew3", __pyx_f[3], 741, 0, __PYX_ERR(3, 741, __pyx_L1_error));
+  __Pyx_TraceCall("PyArray_MultiIterNew3", __pyx_f[3], 740, 0, __PYX_ERR(3, 740, __pyx_L1_error));
 
-  /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":742
+  /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
-  __Pyx_TraceLine(742,0,__PYX_ERR(3, 742, __pyx_L1_error))
+  __Pyx_TraceLine(741,0,__PYX_ERR(3, 741, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 742, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":741
+  /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -15465,15 +15639,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":744
+/* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -15482,32 +15656,32 @@
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
-  __Pyx_TraceCall("PyArray_MultiIterNew4", __pyx_f[3], 744, 0, __PYX_ERR(3, 744, __pyx_L1_error));
+  __Pyx_TraceCall("PyArray_MultiIterNew4", __pyx_f[3], 743, 0, __PYX_ERR(3, 743, __pyx_L1_error));
 
-  /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":745
+  /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
-  __Pyx_TraceLine(745,0,__PYX_ERR(3, 745, __pyx_L1_error))
+  __Pyx_TraceLine(744,0,__PYX_ERR(3, 744, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 745, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":744
+  /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -15519,15 +15693,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":747
+/* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -15536,32 +15710,32 @@
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
-  __Pyx_TraceCall("PyArray_MultiIterNew5", __pyx_f[3], 747, 0, __PYX_ERR(3, 747, __pyx_L1_error));
+  __Pyx_TraceCall("PyArray_MultiIterNew5", __pyx_f[3], 746, 0, __PYX_ERR(3, 746, __pyx_L1_error));
 
-  /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":748
+  /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
-  __Pyx_TraceLine(748,0,__PYX_ERR(3, 748, __pyx_L1_error))
+  __Pyx_TraceLine(747,0,__PYX_ERR(3, 747, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 748, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":747
+  /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -15573,15 +15747,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":750
+/* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
@@ -15590,65 +15764,65 @@
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
-  __Pyx_TraceCall("PyDataType_SHAPE", __pyx_f[3], 750, 0, __PYX_ERR(3, 750, __pyx_L1_error));
+  __Pyx_TraceCall("PyDataType_SHAPE", __pyx_f[3], 749, 0, __PYX_ERR(3, 749, __pyx_L1_error));
 
-  /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":751
+  /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
-  __Pyx_TraceLine(751,0,__PYX_ERR(3, 751, __pyx_L1_error))
+  __Pyx_TraceLine(750,0,__PYX_ERR(3, 750, __pyx_L1_error))
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":752
+    /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
-    __Pyx_TraceLine(752,0,__PYX_ERR(3, 752, __pyx_L1_error))
+    __Pyx_TraceLine(751,0,__PYX_ERR(3, 751, __pyx_L1_error))
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":751
+    /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":754
+  /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_TraceLine(754,0,__PYX_ERR(3, 754, __pyx_L1_error))
+  __Pyx_TraceLine(753,0,__PYX_ERR(3, 753, __pyx_L1_error))
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":750
+  /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
@@ -15659,52 +15833,52 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":929
+/* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
-  __Pyx_TraceCall("set_array_base", __pyx_f[3], 929, 0, __PYX_ERR(3, 929, __pyx_L1_error));
+  __Pyx_TraceCall("set_array_base", __pyx_f[3], 928, 0, __PYX_ERR(3, 928, __pyx_L1_error));
 
-  /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":930
+  /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
-  __Pyx_TraceLine(930,0,__PYX_ERR(3, 930, __pyx_L1_error))
+  __Pyx_TraceLine(929,0,__PYX_ERR(3, 929, __pyx_L1_error))
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":931
+  /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
-  __Pyx_TraceLine(931,0,__PYX_ERR(3, 931, __pyx_L1_error))
+  __Pyx_TraceLine(930,0,__PYX_ERR(3, 930, __pyx_L1_error))
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":929
+  /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -15713,15 +15887,15 @@
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":933
+/* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
@@ -15731,72 +15905,72 @@
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_array_base", 0);
-  __Pyx_TraceCall("get_array_base", __pyx_f[3], 933, 0, __PYX_ERR(3, 933, __pyx_L1_error));
+  __Pyx_TraceCall("get_array_base", __pyx_f[3], 932, 0, __PYX_ERR(3, 932, __pyx_L1_error));
 
-  /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":934
+  /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
-  __Pyx_TraceLine(934,0,__PYX_ERR(3, 934, __pyx_L1_error))
+  __Pyx_TraceLine(933,0,__PYX_ERR(3, 933, __pyx_L1_error))
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":935
+  /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
-  __Pyx_TraceLine(935,0,__PYX_ERR(3, 935, __pyx_L1_error))
+  __Pyx_TraceLine(934,0,__PYX_ERR(3, 934, __pyx_L1_error))
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":936
+    /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
-    __Pyx_TraceLine(936,0,__PYX_ERR(3, 936, __pyx_L1_error))
+    __Pyx_TraceLine(935,0,__PYX_ERR(3, 935, __pyx_L1_error))
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":935
+    /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":937
+  /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
-  __Pyx_TraceLine(937,0,__PYX_ERR(3, 937, __pyx_L1_error))
+  __Pyx_TraceLine(936,0,__PYX_ERR(3, 936, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":933
+  /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
@@ -15807,15 +15981,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":941
+/* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -15831,106 +16005,106 @@
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
-  __Pyx_TraceCall("import_array", __pyx_f[3], 941, 0, __PYX_ERR(3, 941, __pyx_L1_error));
+  __Pyx_TraceCall("import_array", __pyx_f[3], 940, 0, __PYX_ERR(3, 940, __pyx_L1_error));
 
-  /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":942
+  /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
-  __Pyx_TraceLine(942,0,__PYX_ERR(3, 942, __pyx_L1_error))
+  __Pyx_TraceLine(941,0,__PYX_ERR(3, 941, __pyx_L1_error))
   {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":943
+      /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __Pyx_TraceLine(943,0,__PYX_ERR(3, 943, __pyx_L3_error))
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 943, __pyx_L3_error)
+      __Pyx_TraceLine(942,0,__PYX_ERR(3, 942, __pyx_L3_error))
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 942, __pyx_L3_error)
 
-      /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":942
+      /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":944
+    /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
-    __Pyx_TraceLine(944,0,__PYX_ERR(3, 944, __pyx_L5_except_error))
+    __Pyx_TraceLine(943,0,__PYX_ERR(3, 943, __pyx_L5_except_error))
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 944, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":945
+      /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __Pyx_TraceLine(945,0,__PYX_ERR(3, 945, __pyx_L5_except_error))
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 945, __pyx_L5_except_error)
+      __Pyx_TraceLine(944,0,__PYX_ERR(3, 944, __pyx_L5_except_error))
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 944, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(3, 945, __pyx_L5_except_error)
+      __PYX_ERR(3, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":942
+    /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":941
+  /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -15946,15 +16120,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":947
+/* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -15970,106 +16144,106 @@
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
-  __Pyx_TraceCall("import_umath", __pyx_f[3], 947, 0, __PYX_ERR(3, 947, __pyx_L1_error));
+  __Pyx_TraceCall("import_umath", __pyx_f[3], 946, 0, __PYX_ERR(3, 946, __pyx_L1_error));
 
-  /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":948
+  /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
-  __Pyx_TraceLine(948,0,__PYX_ERR(3, 948, __pyx_L1_error))
+  __Pyx_TraceLine(947,0,__PYX_ERR(3, 947, __pyx_L1_error))
   {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":949
+      /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __Pyx_TraceLine(949,0,__PYX_ERR(3, 949, __pyx_L3_error))
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 949, __pyx_L3_error)
+      __Pyx_TraceLine(948,0,__PYX_ERR(3, 948, __pyx_L3_error))
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 948, __pyx_L3_error)
 
-      /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":948
+      /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":950
+    /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
-    __Pyx_TraceLine(950,0,__PYX_ERR(3, 950, __pyx_L5_except_error))
+    __Pyx_TraceLine(949,0,__PYX_ERR(3, 949, __pyx_L5_except_error))
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 950, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":951
+      /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __Pyx_TraceLine(951,0,__PYX_ERR(3, 951, __pyx_L5_except_error))
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 951, __pyx_L5_except_error)
+      __Pyx_TraceLine(950,0,__PYX_ERR(3, 950, __pyx_L5_except_error))
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 950, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(3, 951, __pyx_L5_except_error)
+      __PYX_ERR(3, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":948
+    /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":947
+  /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -16085,15 +16259,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":953
+/* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -16109,106 +16283,106 @@
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
-  __Pyx_TraceCall("import_ufunc", __pyx_f[3], 953, 0, __PYX_ERR(3, 953, __pyx_L1_error));
+  __Pyx_TraceCall("import_ufunc", __pyx_f[3], 952, 0, __PYX_ERR(3, 952, __pyx_L1_error));
 
-  /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":954
+  /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
-  __Pyx_TraceLine(954,0,__PYX_ERR(3, 954, __pyx_L1_error))
+  __Pyx_TraceLine(953,0,__PYX_ERR(3, 953, __pyx_L1_error))
   {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":955
+      /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __Pyx_TraceLine(955,0,__PYX_ERR(3, 955, __pyx_L3_error))
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 955, __pyx_L3_error)
+      __Pyx_TraceLine(954,0,__PYX_ERR(3, 954, __pyx_L3_error))
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 954, __pyx_L3_error)
 
-      /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":954
+      /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":956
+    /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
-    __Pyx_TraceLine(956,0,__PYX_ERR(3, 956, __pyx_L5_except_error))
+    __Pyx_TraceLine(955,0,__PYX_ERR(3, 955, __pyx_L5_except_error))
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 956, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":957
+      /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
-      __Pyx_TraceLine(957,0,__PYX_ERR(3, 957, __pyx_L5_except_error))
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 957, __pyx_L5_except_error)
+      __Pyx_TraceLine(956,0,__PYX_ERR(3, 956, __pyx_L5_except_error))
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 956, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(3, 957, __pyx_L5_except_error)
+      __PYX_ERR(3, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":954
+    /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":953
+  /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -16224,15 +16398,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":967
+/* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
@@ -16240,28 +16414,28 @@
   int __pyx_r;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
-  __Pyx_TraceCall("is_timedelta64_object", __pyx_f[3], 967, 0, __PYX_ERR(3, 967, __pyx_L1_error));
+  __Pyx_TraceCall("is_timedelta64_object", __pyx_f[3], 966, 0, __PYX_ERR(3, 966, __pyx_L1_error));
 
-  /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":979
+  /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_TraceLine(979,0,__PYX_ERR(3, 979, __pyx_L1_error))
+  __Pyx_TraceLine(978,0,__PYX_ERR(3, 978, __pyx_L1_error))
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":967
+  /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
@@ -16271,15 +16445,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":982
+/* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
@@ -16287,28 +16461,28 @@
   int __pyx_r;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
-  __Pyx_TraceCall("is_datetime64_object", __pyx_f[3], 982, 0, __PYX_ERR(3, 982, __pyx_L1_error));
+  __Pyx_TraceCall("is_datetime64_object", __pyx_f[3], 981, 0, __PYX_ERR(3, 981, __pyx_L1_error));
 
-  /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":994
+  /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_TraceLine(994,0,__PYX_ERR(3, 994, __pyx_L1_error))
+  __Pyx_TraceLine(993,0,__PYX_ERR(3, 993, __pyx_L1_error))
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":982
+  /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
@@ -16318,42 +16492,42 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":997
+/* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
   __Pyx_TraceDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_TraceCall("get_datetime64_value", __pyx_f[3], 997, 1, __PYX_ERR(3, 997, __pyx_L1_error));
+  __Pyx_TraceCall("get_datetime64_value", __pyx_f[3], 996, 1, __PYX_ERR(3, 996, __pyx_L1_error));
 
-  /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":1004
+  /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_TraceLine(1004,1,__PYX_ERR(3, 1004, __pyx_L1_error))
+  __Pyx_TraceLine(1003,1,__PYX_ERR(3, 1003, __pyx_L1_error))
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":997
+  /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
@@ -16362,42 +16536,42 @@
   __Pyx_WriteUnraisable("numpy.get_datetime64_value", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 1);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
   return __pyx_r;
 }
 
-/* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":1007
+/* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
   __Pyx_TraceDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_TraceCall("get_timedelta64_value", __pyx_f[3], 1007, 1, __PYX_ERR(3, 1007, __pyx_L1_error));
+  __Pyx_TraceCall("get_timedelta64_value", __pyx_f[3], 1006, 1, __PYX_ERR(3, 1006, __pyx_L1_error));
 
-  /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":1011
+  /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_TraceLine(1011,1,__PYX_ERR(3, 1011, __pyx_L1_error))
+  __Pyx_TraceLine(1010,1,__PYX_ERR(3, 1010, __pyx_L1_error))
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":1007
+  /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
@@ -16406,40 +16580,40 @@
   __Pyx_WriteUnraisable("numpy.get_timedelta64_value", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 1);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
   return __pyx_r;
 }
 
-/* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":1014
+/* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
   __Pyx_TraceDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_TraceCall("get_datetime64_unit", __pyx_f[3], 1014, 1, __PYX_ERR(3, 1014, __pyx_L1_error));
+  __Pyx_TraceCall("get_datetime64_unit", __pyx_f[3], 1013, 1, __PYX_ERR(3, 1013, __pyx_L1_error));
 
-  /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":1018
+  /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
-  __Pyx_TraceLine(1018,1,__PYX_ERR(3, 1018, __pyx_L1_error))
+  __Pyx_TraceLine(1017,1,__PYX_ERR(3, 1017, __pyx_L1_error))
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":1014
+  /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -16448,15 +16622,15 @@
   __Pyx_WriteUnraisable("numpy.get_datetime64_unit", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 1);
   __pyx_r = (NPY_DATETIMEUNIT) 0;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
   return __pyx_r;
 }
 
-/* "View.MemoryView":122
+/* "View.MemoryView":123
  *         cdef bint dtype_is_object
  * 
  *     def __cinit__(array self, tuple shape, Py_ssize_t itemsize, format not None,             # <<<<<<<<<<<<<<
  *                   mode="c", bint allocate_buffer=True):
  * 
  */
 
@@ -16500,21 +16674,21 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_shape)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_itemsize)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 3, 5, 1); __PYX_ERR(2, 122, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 3, 5, 1); __PYX_ERR(2, 123, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_format)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 3, 5, 2); __PYX_ERR(2, 122, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 3, 5, 2); __PYX_ERR(2, 123, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_mode);
           if (value) { values[3] = value; kw_args--; }
         }
@@ -16522,15 +16696,15 @@
         case  4:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_allocate_buffer);
           if (value) { values[4] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(2, 122, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(2, 123, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
@@ -16538,46 +16712,46 @@
         values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_shape = ((PyObject*)values[0]);
-    __pyx_v_itemsize = __Pyx_PyIndex_AsSsize_t(values[1]); if (unlikely((__pyx_v_itemsize == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(2, 122, __pyx_L3_error)
+    __pyx_v_itemsize = __Pyx_PyIndex_AsSsize_t(values[1]); if (unlikely((__pyx_v_itemsize == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(2, 123, __pyx_L3_error)
     __pyx_v_format = values[2];
     __pyx_v_mode = values[3];
     if (values[4]) {
-      __pyx_v_allocate_buffer = __Pyx_PyObject_IsTrue(values[4]); if (unlikely((__pyx_v_allocate_buffer == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 123, __pyx_L3_error)
+      __pyx_v_allocate_buffer = __Pyx_PyObject_IsTrue(values[4]); if (unlikely((__pyx_v_allocate_buffer == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 124, __pyx_L3_error)
     } else {
 
-      /* "View.MemoryView":123
+      /* "View.MemoryView":124
  * 
  *     def __cinit__(array self, tuple shape, Py_ssize_t itemsize, format not None,
  *                   mode="c", bint allocate_buffer=True):             # <<<<<<<<<<<<<<
  * 
  *         cdef int idx
  */
       __pyx_v_allocate_buffer = ((int)1);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 3, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(2, 122, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 3, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(2, 123, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("View.MemoryView.array.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_shape), (&PyTuple_Type), 1, "shape", 1))) __PYX_ERR(2, 122, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_shape), (&PyTuple_Type), 1, "shape", 1))) __PYX_ERR(2, 123, __pyx_L1_error)
   if (unlikely(((PyObject *)__pyx_v_format) == Py_None)) {
-    PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "format"); __PYX_ERR(2, 122, __pyx_L1_error)
+    PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "format"); __PYX_ERR(2, 123, __pyx_L1_error)
   }
   __pyx_r = __pyx_array___pyx_pf_15View_dot_MemoryView_5array___cinit__(((struct __pyx_array_obj *)__pyx_v_self), __pyx_v_shape, __pyx_v_itemsize, __pyx_v_format, __pyx_v_mode, __pyx_v_allocate_buffer);
 
-  /* "View.MemoryView":122
+  /* "View.MemoryView":123
  *         cdef bint dtype_is_object
  * 
  *     def __cinit__(array self, tuple shape, Py_ssize_t itemsize, format not None,             # <<<<<<<<<<<<<<
  *                   mode="c", bint allocate_buffer=True):
  * 
  */
 
@@ -16610,620 +16784,620 @@
   Py_ssize_t __pyx_t_9;
   PyObject *__pyx_t_10 = NULL;
   Py_ssize_t __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
-  __Pyx_TraceCall("__cinit__", __pyx_f[2], 122, 0, __PYX_ERR(2, 122, __pyx_L1_error));
+  __Pyx_TraceCall("__cinit__", __pyx_f[2], 123, 0, __PYX_ERR(2, 123, __pyx_L1_error));
   __Pyx_INCREF(__pyx_v_format);
 
-  /* "View.MemoryView":129
+  /* "View.MemoryView":130
  *         cdef PyObject **p
  * 
  *         self.ndim = <int> len(shape)             # <<<<<<<<<<<<<<
  *         self.itemsize = itemsize
  * 
  */
-  __Pyx_TraceLine(129,0,__PYX_ERR(2, 129, __pyx_L1_error))
+  __Pyx_TraceLine(130,0,__PYX_ERR(2, 130, __pyx_L1_error))
   if (unlikely(__pyx_v_shape == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(2, 129, __pyx_L1_error)
+    __PYX_ERR(2, 130, __pyx_L1_error)
   }
-  __pyx_t_1 = PyTuple_GET_SIZE(__pyx_v_shape); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(2, 129, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_GET_SIZE(__pyx_v_shape); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(2, 130, __pyx_L1_error)
   __pyx_v_self->ndim = ((int)__pyx_t_1);
 
-  /* "View.MemoryView":130
+  /* "View.MemoryView":131
  * 
  *         self.ndim = <int> len(shape)
  *         self.itemsize = itemsize             # <<<<<<<<<<<<<<
  * 
  *         if not self.ndim:
  */
-  __Pyx_TraceLine(130,0,__PYX_ERR(2, 130, __pyx_L1_error))
+  __Pyx_TraceLine(131,0,__PYX_ERR(2, 131, __pyx_L1_error))
   __pyx_v_self->itemsize = __pyx_v_itemsize;
 
-  /* "View.MemoryView":132
+  /* "View.MemoryView":133
  *         self.itemsize = itemsize
  * 
  *         if not self.ndim:             # <<<<<<<<<<<<<<
  *             raise ValueError("Empty shape tuple for cython.array")
  * 
  */
-  __Pyx_TraceLine(132,0,__PYX_ERR(2, 132, __pyx_L1_error))
+  __Pyx_TraceLine(133,0,__PYX_ERR(2, 133, __pyx_L1_error))
   __pyx_t_2 = ((!(__pyx_v_self->ndim != 0)) != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "View.MemoryView":133
+    /* "View.MemoryView":134
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if itemsize <= 0:
  */
-    __Pyx_TraceLine(133,0,__PYX_ERR(2, 133, __pyx_L1_error))
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 133, __pyx_L1_error)
+    __Pyx_TraceLine(134,0,__PYX_ERR(2, 134, __pyx_L1_error))
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 134, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(2, 133, __pyx_L1_error)
+    __PYX_ERR(2, 134, __pyx_L1_error)
 
-    /* "View.MemoryView":132
+    /* "View.MemoryView":133
  *         self.itemsize = itemsize
  * 
  *         if not self.ndim:             # <<<<<<<<<<<<<<
  *             raise ValueError("Empty shape tuple for cython.array")
  * 
  */
   }
 
-  /* "View.MemoryView":135
+  /* "View.MemoryView":136
  *             raise ValueError("Empty shape tuple for cython.array")
  * 
  *         if itemsize <= 0:             # <<<<<<<<<<<<<<
  *             raise ValueError("itemsize <= 0 for cython.array")
  * 
  */
-  __Pyx_TraceLine(135,0,__PYX_ERR(2, 135, __pyx_L1_error))
+  __Pyx_TraceLine(136,0,__PYX_ERR(2, 136, __pyx_L1_error))
   __pyx_t_2 = ((__pyx_v_itemsize <= 0) != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "View.MemoryView":136
+    /* "View.MemoryView":137
  * 
  *         if itemsize <= 0:
  *             raise ValueError("itemsize <= 0 for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if not isinstance(format, bytes):
  */
-    __Pyx_TraceLine(136,0,__PYX_ERR(2, 136, __pyx_L1_error))
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 136, __pyx_L1_error)
+    __Pyx_TraceLine(137,0,__PYX_ERR(2, 137, __pyx_L1_error))
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 137, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(2, 136, __pyx_L1_error)
+    __PYX_ERR(2, 137, __pyx_L1_error)
 
-    /* "View.MemoryView":135
+    /* "View.MemoryView":136
  *             raise ValueError("Empty shape tuple for cython.array")
  * 
  *         if itemsize <= 0:             # <<<<<<<<<<<<<<
  *             raise ValueError("itemsize <= 0 for cython.array")
  * 
  */
   }
 
-  /* "View.MemoryView":138
+  /* "View.MemoryView":139
  *             raise ValueError("itemsize <= 0 for cython.array")
  * 
  *         if not isinstance(format, bytes):             # <<<<<<<<<<<<<<
  *             format = format.encode('ASCII')
  *         self._format = format  # keep a reference to the byte string
  */
-  __Pyx_TraceLine(138,0,__PYX_ERR(2, 138, __pyx_L1_error))
+  __Pyx_TraceLine(139,0,__PYX_ERR(2, 139, __pyx_L1_error))
   __pyx_t_2 = PyBytes_Check(__pyx_v_format); 
   __pyx_t_4 = ((!(__pyx_t_2 != 0)) != 0);
   if (__pyx_t_4) {
 
-    /* "View.MemoryView":139
+    /* "View.MemoryView":140
  * 
  *         if not isinstance(format, bytes):
  *             format = format.encode('ASCII')             # <<<<<<<<<<<<<<
  *         self._format = format  # keep a reference to the byte string
  *         self.format = self._format
  */
-    __Pyx_TraceLine(139,0,__PYX_ERR(2, 139, __pyx_L1_error))
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_format, __pyx_n_s_encode); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 139, __pyx_L1_error)
+    __Pyx_TraceLine(140,0,__PYX_ERR(2, 140, __pyx_L1_error))
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_format, __pyx_n_s_encode); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 140, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_6 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
       }
     }
     __pyx_t_3 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_6, __pyx_n_s_ASCII) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_n_s_ASCII);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 139, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 140, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF_SET(__pyx_v_format, __pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "View.MemoryView":138
+    /* "View.MemoryView":139
  *             raise ValueError("itemsize <= 0 for cython.array")
  * 
  *         if not isinstance(format, bytes):             # <<<<<<<<<<<<<<
  *             format = format.encode('ASCII')
  *         self._format = format  # keep a reference to the byte string
  */
   }
 
-  /* "View.MemoryView":140
+  /* "View.MemoryView":141
  *         if not isinstance(format, bytes):
  *             format = format.encode('ASCII')
  *         self._format = format  # keep a reference to the byte string             # <<<<<<<<<<<<<<
  *         self.format = self._format
  * 
  */
-  __Pyx_TraceLine(140,0,__PYX_ERR(2, 140, __pyx_L1_error))
-  if (!(likely(PyBytes_CheckExact(__pyx_v_format))||((__pyx_v_format) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_v_format)->tp_name), 0))) __PYX_ERR(2, 140, __pyx_L1_error)
+  __Pyx_TraceLine(141,0,__PYX_ERR(2, 141, __pyx_L1_error))
+  if (!(likely(PyBytes_CheckExact(__pyx_v_format))||((__pyx_v_format) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_v_format)->tp_name), 0))) __PYX_ERR(2, 141, __pyx_L1_error)
   __pyx_t_3 = __pyx_v_format;
   __Pyx_INCREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_3);
   __Pyx_GOTREF(__pyx_v_self->_format);
   __Pyx_DECREF(__pyx_v_self->_format);
   __pyx_v_self->_format = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "View.MemoryView":141
+  /* "View.MemoryView":142
  *             format = format.encode('ASCII')
  *         self._format = format  # keep a reference to the byte string
  *         self.format = self._format             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_TraceLine(141,0,__PYX_ERR(2, 141, __pyx_L1_error))
+  __Pyx_TraceLine(142,0,__PYX_ERR(2, 142, __pyx_L1_error))
   if (unlikely(__pyx_v_self->_format == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
-    __PYX_ERR(2, 141, __pyx_L1_error)
+    __PYX_ERR(2, 142, __pyx_L1_error)
   }
-  __pyx_t_7 = __Pyx_PyBytes_AsWritableString(__pyx_v_self->_format); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(2, 141, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyBytes_AsWritableString(__pyx_v_self->_format); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(2, 142, __pyx_L1_error)
   __pyx_v_self->format = __pyx_t_7;
 
-  /* "View.MemoryView":144
+  /* "View.MemoryView":145
  * 
  * 
  *         self._shape = <Py_ssize_t *> PyObject_Malloc(sizeof(Py_ssize_t)*self.ndim*2)             # <<<<<<<<<<<<<<
  *         self._strides = self._shape + self.ndim
  * 
  */
-  __Pyx_TraceLine(144,0,__PYX_ERR(2, 144, __pyx_L1_error))
+  __Pyx_TraceLine(145,0,__PYX_ERR(2, 145, __pyx_L1_error))
   __pyx_v_self->_shape = ((Py_ssize_t *)PyObject_Malloc((((sizeof(Py_ssize_t)) * __pyx_v_self->ndim) * 2)));
 
-  /* "View.MemoryView":145
+  /* "View.MemoryView":146
  * 
  *         self._shape = <Py_ssize_t *> PyObject_Malloc(sizeof(Py_ssize_t)*self.ndim*2)
  *         self._strides = self._shape + self.ndim             # <<<<<<<<<<<<<<
  * 
  *         if not self._shape:
  */
-  __Pyx_TraceLine(145,0,__PYX_ERR(2, 145, __pyx_L1_error))
+  __Pyx_TraceLine(146,0,__PYX_ERR(2, 146, __pyx_L1_error))
   __pyx_v_self->_strides = (__pyx_v_self->_shape + __pyx_v_self->ndim);
 
-  /* "View.MemoryView":147
+  /* "View.MemoryView":148
  *         self._strides = self._shape + self.ndim
  * 
  *         if not self._shape:             # <<<<<<<<<<<<<<
  *             raise MemoryError("unable to allocate shape and strides.")
  * 
  */
-  __Pyx_TraceLine(147,0,__PYX_ERR(2, 147, __pyx_L1_error))
+  __Pyx_TraceLine(148,0,__PYX_ERR(2, 148, __pyx_L1_error))
   __pyx_t_4 = ((!(__pyx_v_self->_shape != 0)) != 0);
   if (unlikely(__pyx_t_4)) {
 
-    /* "View.MemoryView":148
+    /* "View.MemoryView":149
  * 
  *         if not self._shape:
  *             raise MemoryError("unable to allocate shape and strides.")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __Pyx_TraceLine(148,0,__PYX_ERR(2, 148, __pyx_L1_error))
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 148, __pyx_L1_error)
+    __Pyx_TraceLine(149,0,__PYX_ERR(2, 149, __pyx_L1_error))
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__14, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 149, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(2, 148, __pyx_L1_error)
+    __PYX_ERR(2, 149, __pyx_L1_error)
 
-    /* "View.MemoryView":147
+    /* "View.MemoryView":148
  *         self._strides = self._shape + self.ndim
  * 
  *         if not self._shape:             # <<<<<<<<<<<<<<
  *             raise MemoryError("unable to allocate shape and strides.")
  * 
  */
   }
 
-  /* "View.MemoryView":151
+  /* "View.MemoryView":152
  * 
  * 
  *         for idx, dim in enumerate(shape):             # <<<<<<<<<<<<<<
  *             if dim <= 0:
  *                 raise ValueError("Invalid shape in axis %d: %d." % (idx, dim))
  */
-  __Pyx_TraceLine(151,0,__PYX_ERR(2, 151, __pyx_L1_error))
+  __Pyx_TraceLine(152,0,__PYX_ERR(2, 152, __pyx_L1_error))
   __pyx_t_8 = 0;
   __pyx_t_3 = __pyx_v_shape; __Pyx_INCREF(__pyx_t_3); __pyx_t_1 = 0;
   for (;;) {
     if (__pyx_t_1 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_5); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(2, 151, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_5); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(2, 152, __pyx_L1_error)
     #else
-    __pyx_t_5 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 151, __pyx_L1_error)
+    __pyx_t_5 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 152, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     #endif
-    __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_5); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(2, 151, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_5); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(2, 152, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_v_dim = __pyx_t_9;
     __pyx_v_idx = __pyx_t_8;
     __pyx_t_8 = (__pyx_t_8 + 1);
 
-    /* "View.MemoryView":152
+    /* "View.MemoryView":153
  * 
  *         for idx, dim in enumerate(shape):
  *             if dim <= 0:             # <<<<<<<<<<<<<<
  *                 raise ValueError("Invalid shape in axis %d: %d." % (idx, dim))
  *             self._shape[idx] = dim
  */
-    __Pyx_TraceLine(152,0,__PYX_ERR(2, 152, __pyx_L1_error))
+    __Pyx_TraceLine(153,0,__PYX_ERR(2, 153, __pyx_L1_error))
     __pyx_t_4 = ((__pyx_v_dim <= 0) != 0);
     if (unlikely(__pyx_t_4)) {
 
-      /* "View.MemoryView":153
+      /* "View.MemoryView":154
  *         for idx, dim in enumerate(shape):
  *             if dim <= 0:
  *                 raise ValueError("Invalid shape in axis %d: %d." % (idx, dim))             # <<<<<<<<<<<<<<
  *             self._shape[idx] = dim
  * 
  */
-      __Pyx_TraceLine(153,0,__PYX_ERR(2, 153, __pyx_L1_error))
-      __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_idx); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 153, __pyx_L1_error)
+      __Pyx_TraceLine(154,0,__PYX_ERR(2, 154, __pyx_L1_error))
+      __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_idx); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 154, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_6 = PyInt_FromSsize_t(__pyx_v_dim); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 153, __pyx_L1_error)
+      __pyx_t_6 = PyInt_FromSsize_t(__pyx_v_dim); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 154, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_10 = PyTuple_New(2); if (unlikely(!__pyx_t_10)) __PYX_ERR(2, 153, __pyx_L1_error)
+      __pyx_t_10 = PyTuple_New(2); if (unlikely(!__pyx_t_10)) __PYX_ERR(2, 154, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_GIVEREF(__pyx_t_5);
       PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_5);
       __Pyx_GIVEREF(__pyx_t_6);
       PyTuple_SET_ITEM(__pyx_t_10, 1, __pyx_t_6);
       __pyx_t_5 = 0;
       __pyx_t_6 = 0;
-      __pyx_t_6 = __Pyx_PyString_Format(__pyx_kp_s_Invalid_shape_in_axis_d_d, __pyx_t_10); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 153, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyString_Format(__pyx_kp_s_Invalid_shape_in_axis_d_d, __pyx_t_10); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 154, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-      __pyx_t_10 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_6); if (unlikely(!__pyx_t_10)) __PYX_ERR(2, 153, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_6); if (unlikely(!__pyx_t_10)) __PYX_ERR(2, 154, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_Raise(__pyx_t_10, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-      __PYX_ERR(2, 153, __pyx_L1_error)
+      __PYX_ERR(2, 154, __pyx_L1_error)
 
-      /* "View.MemoryView":152
+      /* "View.MemoryView":153
  * 
  *         for idx, dim in enumerate(shape):
  *             if dim <= 0:             # <<<<<<<<<<<<<<
  *                 raise ValueError("Invalid shape in axis %d: %d." % (idx, dim))
  *             self._shape[idx] = dim
  */
     }
 
-    /* "View.MemoryView":154
+    /* "View.MemoryView":155
  *             if dim <= 0:
  *                 raise ValueError("Invalid shape in axis %d: %d." % (idx, dim))
  *             self._shape[idx] = dim             # <<<<<<<<<<<<<<
  * 
  *         cdef char order
  */
-    __Pyx_TraceLine(154,0,__PYX_ERR(2, 154, __pyx_L1_error))
+    __Pyx_TraceLine(155,0,__PYX_ERR(2, 155, __pyx_L1_error))
     (__pyx_v_self->_shape[__pyx_v_idx]) = __pyx_v_dim;
 
-    /* "View.MemoryView":151
+    /* "View.MemoryView":152
  * 
  * 
  *         for idx, dim in enumerate(shape):             # <<<<<<<<<<<<<<
  *             if dim <= 0:
  *                 raise ValueError("Invalid shape in axis %d: %d." % (idx, dim))
  */
-    __Pyx_TraceLine(151,0,__PYX_ERR(2, 151, __pyx_L1_error))
+    __Pyx_TraceLine(152,0,__PYX_ERR(2, 152, __pyx_L1_error))
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "View.MemoryView":157
+  /* "View.MemoryView":158
  * 
  *         cdef char order
  *         if mode == 'fortran':             # <<<<<<<<<<<<<<
  *             order = b'F'
  *             self.mode = u'fortran'
  */
-  __Pyx_TraceLine(157,0,__PYX_ERR(2, 157, __pyx_L1_error))
-  __pyx_t_4 = (__Pyx_PyString_Equals(__pyx_v_mode, __pyx_n_s_fortran, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(2, 157, __pyx_L1_error)
+  __Pyx_TraceLine(158,0,__PYX_ERR(2, 158, __pyx_L1_error))
+  __pyx_t_4 = (__Pyx_PyString_Equals(__pyx_v_mode, __pyx_n_s_fortran, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(2, 158, __pyx_L1_error)
   if (__pyx_t_4) {
 
-    /* "View.MemoryView":158
+    /* "View.MemoryView":159
  *         cdef char order
  *         if mode == 'fortran':
  *             order = b'F'             # <<<<<<<<<<<<<<
  *             self.mode = u'fortran'
  *         elif mode == 'c':
  */
-    __Pyx_TraceLine(158,0,__PYX_ERR(2, 158, __pyx_L1_error))
+    __Pyx_TraceLine(159,0,__PYX_ERR(2, 159, __pyx_L1_error))
     __pyx_v_order = 'F';
 
-    /* "View.MemoryView":159
+    /* "View.MemoryView":160
  *         if mode == 'fortran':
  *             order = b'F'
  *             self.mode = u'fortran'             # <<<<<<<<<<<<<<
  *         elif mode == 'c':
  *             order = b'C'
  */
-    __Pyx_TraceLine(159,0,__PYX_ERR(2, 159, __pyx_L1_error))
+    __Pyx_TraceLine(160,0,__PYX_ERR(2, 160, __pyx_L1_error))
     __Pyx_INCREF(__pyx_n_u_fortran);
     __Pyx_GIVEREF(__pyx_n_u_fortran);
     __Pyx_GOTREF(__pyx_v_self->mode);
     __Pyx_DECREF(__pyx_v_self->mode);
     __pyx_v_self->mode = __pyx_n_u_fortran;
 
-    /* "View.MemoryView":157
+    /* "View.MemoryView":158
  * 
  *         cdef char order
  *         if mode == 'fortran':             # <<<<<<<<<<<<<<
  *             order = b'F'
  *             self.mode = u'fortran'
  */
     goto __pyx_L10;
   }
 
-  /* "View.MemoryView":160
+  /* "View.MemoryView":161
  *             order = b'F'
  *             self.mode = u'fortran'
  *         elif mode == 'c':             # <<<<<<<<<<<<<<
  *             order = b'C'
  *             self.mode = u'c'
  */
-  __Pyx_TraceLine(160,0,__PYX_ERR(2, 160, __pyx_L1_error))
-  __pyx_t_4 = (__Pyx_PyString_Equals(__pyx_v_mode, __pyx_n_s_c, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(2, 160, __pyx_L1_error)
+  __Pyx_TraceLine(161,0,__PYX_ERR(2, 161, __pyx_L1_error))
+  __pyx_t_4 = (__Pyx_PyString_Equals(__pyx_v_mode, __pyx_n_s_c, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(2, 161, __pyx_L1_error)
   if (likely(__pyx_t_4)) {
 
-    /* "View.MemoryView":161
+    /* "View.MemoryView":162
  *             self.mode = u'fortran'
  *         elif mode == 'c':
  *             order = b'C'             # <<<<<<<<<<<<<<
  *             self.mode = u'c'
  *         else:
  */
-    __Pyx_TraceLine(161,0,__PYX_ERR(2, 161, __pyx_L1_error))
+    __Pyx_TraceLine(162,0,__PYX_ERR(2, 162, __pyx_L1_error))
     __pyx_v_order = 'C';
 
-    /* "View.MemoryView":162
+    /* "View.MemoryView":163
  *         elif mode == 'c':
  *             order = b'C'
  *             self.mode = u'c'             # <<<<<<<<<<<<<<
  *         else:
  *             raise ValueError("Invalid mode, expected 'c' or 'fortran', got %s" % mode)
  */
-    __Pyx_TraceLine(162,0,__PYX_ERR(2, 162, __pyx_L1_error))
+    __Pyx_TraceLine(163,0,__PYX_ERR(2, 163, __pyx_L1_error))
     __Pyx_INCREF(__pyx_n_u_c);
     __Pyx_GIVEREF(__pyx_n_u_c);
     __Pyx_GOTREF(__pyx_v_self->mode);
     __Pyx_DECREF(__pyx_v_self->mode);
     __pyx_v_self->mode = __pyx_n_u_c;
 
-    /* "View.MemoryView":160
+    /* "View.MemoryView":161
  *             order = b'F'
  *             self.mode = u'fortran'
  *         elif mode == 'c':             # <<<<<<<<<<<<<<
  *             order = b'C'
  *             self.mode = u'c'
  */
     goto __pyx_L10;
   }
 
-  /* "View.MemoryView":164
+  /* "View.MemoryView":165
  *             self.mode = u'c'
  *         else:
  *             raise ValueError("Invalid mode, expected 'c' or 'fortran', got %s" % mode)             # <<<<<<<<<<<<<<
  * 
  *         self.len = fill_contig_strides_array(self._shape, self._strides,
  */
-  __Pyx_TraceLine(164,0,__PYX_ERR(2, 164, __pyx_L1_error))
+  __Pyx_TraceLine(165,0,__PYX_ERR(2, 165, __pyx_L1_error))
   /*else*/ {
-    __pyx_t_3 = __Pyx_PyString_FormatSafe(__pyx_kp_s_Invalid_mode_expected_c_or_fortr, __pyx_v_mode); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 164, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyString_FormatSafe(__pyx_kp_s_Invalid_mode_expected_c_or_fortr, __pyx_v_mode); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 165, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_10 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_10)) __PYX_ERR(2, 164, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_10)) __PYX_ERR(2, 165, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_Raise(__pyx_t_10, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-    __PYX_ERR(2, 164, __pyx_L1_error)
+    __PYX_ERR(2, 165, __pyx_L1_error)
   }
   __pyx_L10:;
 
-  /* "View.MemoryView":166
+  /* "View.MemoryView":167
  *             raise ValueError("Invalid mode, expected 'c' or 'fortran', got %s" % mode)
  * 
  *         self.len = fill_contig_strides_array(self._shape, self._strides,             # <<<<<<<<<<<<<<
  *                                              itemsize, self.ndim, order)
  * 
  */
-  __Pyx_TraceLine(166,0,__PYX_ERR(2, 166, __pyx_L1_error))
+  __Pyx_TraceLine(167,0,__PYX_ERR(2, 167, __pyx_L1_error))
   __pyx_v_self->len = __pyx_fill_contig_strides_array(__pyx_v_self->_shape, __pyx_v_self->_strides, __pyx_v_itemsize, __pyx_v_self->ndim, __pyx_v_order);
 
-  /* "View.MemoryView":169
+  /* "View.MemoryView":170
  *                                              itemsize, self.ndim, order)
  * 
  *         self.free_data = allocate_buffer             # <<<<<<<<<<<<<<
  *         self.dtype_is_object = format == b'O'
  *         if allocate_buffer:
  */
-  __Pyx_TraceLine(169,0,__PYX_ERR(2, 169, __pyx_L1_error))
+  __Pyx_TraceLine(170,0,__PYX_ERR(2, 170, __pyx_L1_error))
   __pyx_v_self->free_data = __pyx_v_allocate_buffer;
 
-  /* "View.MemoryView":170
+  /* "View.MemoryView":171
  * 
  *         self.free_data = allocate_buffer
  *         self.dtype_is_object = format == b'O'             # <<<<<<<<<<<<<<
  *         if allocate_buffer:
  * 
  */
-  __Pyx_TraceLine(170,0,__PYX_ERR(2, 170, __pyx_L1_error))
-  __pyx_t_10 = PyObject_RichCompare(__pyx_v_format, __pyx_n_b_O, Py_EQ); __Pyx_XGOTREF(__pyx_t_10); if (unlikely(!__pyx_t_10)) __PYX_ERR(2, 170, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_10); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 170, __pyx_L1_error)
+  __Pyx_TraceLine(171,0,__PYX_ERR(2, 171, __pyx_L1_error))
+  __pyx_t_10 = PyObject_RichCompare(__pyx_v_format, __pyx_n_b_O, Py_EQ); __Pyx_XGOTREF(__pyx_t_10); if (unlikely(!__pyx_t_10)) __PYX_ERR(2, 171, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_10); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 171, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
   __pyx_v_self->dtype_is_object = __pyx_t_4;
 
-  /* "View.MemoryView":171
+  /* "View.MemoryView":172
  *         self.free_data = allocate_buffer
  *         self.dtype_is_object = format == b'O'
  *         if allocate_buffer:             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_TraceLine(171,0,__PYX_ERR(2, 171, __pyx_L1_error))
+  __Pyx_TraceLine(172,0,__PYX_ERR(2, 172, __pyx_L1_error))
   __pyx_t_4 = (__pyx_v_allocate_buffer != 0);
   if (__pyx_t_4) {
 
-    /* "View.MemoryView":174
+    /* "View.MemoryView":175
  * 
  * 
  *             self.data = <char *>malloc(self.len)             # <<<<<<<<<<<<<<
  *             if not self.data:
  *                 raise MemoryError("unable to allocate array data.")
  */
-    __Pyx_TraceLine(174,0,__PYX_ERR(2, 174, __pyx_L1_error))
+    __Pyx_TraceLine(175,0,__PYX_ERR(2, 175, __pyx_L1_error))
     __pyx_v_self->data = ((char *)malloc(__pyx_v_self->len));
 
-    /* "View.MemoryView":175
+    /* "View.MemoryView":176
  * 
  *             self.data = <char *>malloc(self.len)
  *             if not self.data:             # <<<<<<<<<<<<<<
  *                 raise MemoryError("unable to allocate array data.")
  * 
  */
-    __Pyx_TraceLine(175,0,__PYX_ERR(2, 175, __pyx_L1_error))
+    __Pyx_TraceLine(176,0,__PYX_ERR(2, 176, __pyx_L1_error))
     __pyx_t_4 = ((!(__pyx_v_self->data != 0)) != 0);
     if (unlikely(__pyx_t_4)) {
 
-      /* "View.MemoryView":176
+      /* "View.MemoryView":177
  *             self.data = <char *>malloc(self.len)
  *             if not self.data:
  *                 raise MemoryError("unable to allocate array data.")             # <<<<<<<<<<<<<<
  * 
  *             if self.dtype_is_object:
  */
-      __Pyx_TraceLine(176,0,__PYX_ERR(2, 176, __pyx_L1_error))
-      __pyx_t_10 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__14, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(2, 176, __pyx_L1_error)
+      __Pyx_TraceLine(177,0,__PYX_ERR(2, 177, __pyx_L1_error))
+      __pyx_t_10 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__15, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(2, 177, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_Raise(__pyx_t_10, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-      __PYX_ERR(2, 176, __pyx_L1_error)
+      __PYX_ERR(2, 177, __pyx_L1_error)
 
-      /* "View.MemoryView":175
+      /* "View.MemoryView":176
  * 
  *             self.data = <char *>malloc(self.len)
  *             if not self.data:             # <<<<<<<<<<<<<<
  *                 raise MemoryError("unable to allocate array data.")
  * 
  */
     }
 
-    /* "View.MemoryView":178
+    /* "View.MemoryView":179
  *                 raise MemoryError("unable to allocate array data.")
  * 
  *             if self.dtype_is_object:             # <<<<<<<<<<<<<<
  *                 p = <PyObject **> self.data
  *                 for i in range(self.len / itemsize):
  */
-    __Pyx_TraceLine(178,0,__PYX_ERR(2, 178, __pyx_L1_error))
+    __Pyx_TraceLine(179,0,__PYX_ERR(2, 179, __pyx_L1_error))
     __pyx_t_4 = (__pyx_v_self->dtype_is_object != 0);
     if (__pyx_t_4) {
 
-      /* "View.MemoryView":179
+      /* "View.MemoryView":180
  * 
  *             if self.dtype_is_object:
  *                 p = <PyObject **> self.data             # <<<<<<<<<<<<<<
  *                 for i in range(self.len / itemsize):
  *                     p[i] = Py_None
  */
-      __Pyx_TraceLine(179,0,__PYX_ERR(2, 179, __pyx_L1_error))
+      __Pyx_TraceLine(180,0,__PYX_ERR(2, 180, __pyx_L1_error))
       __pyx_v_p = ((PyObject **)__pyx_v_self->data);
 
-      /* "View.MemoryView":180
+      /* "View.MemoryView":181
  *             if self.dtype_is_object:
  *                 p = <PyObject **> self.data
  *                 for i in range(self.len / itemsize):             # <<<<<<<<<<<<<<
  *                     p[i] = Py_None
  *                     Py_INCREF(Py_None)
  */
-      __Pyx_TraceLine(180,0,__PYX_ERR(2, 180, __pyx_L1_error))
+      __Pyx_TraceLine(181,0,__PYX_ERR(2, 181, __pyx_L1_error))
       if (unlikely(__pyx_v_itemsize == 0)) {
         PyErr_SetString(PyExc_ZeroDivisionError, "integer division or modulo by zero");
-        __PYX_ERR(2, 180, __pyx_L1_error)
+        __PYX_ERR(2, 181, __pyx_L1_error)
       }
       else if (sizeof(Py_ssize_t) == sizeof(long) && (!(((Py_ssize_t)-1) > 0)) && unlikely(__pyx_v_itemsize == (Py_ssize_t)-1)  && unlikely(UNARY_NEG_WOULD_OVERFLOW(__pyx_v_self->len))) {
         PyErr_SetString(PyExc_OverflowError, "value too large to perform division");
-        __PYX_ERR(2, 180, __pyx_L1_error)
+        __PYX_ERR(2, 181, __pyx_L1_error)
       }
       __pyx_t_1 = (__pyx_v_self->len / __pyx_v_itemsize);
       __pyx_t_9 = __pyx_t_1;
       for (__pyx_t_11 = 0; __pyx_t_11 < __pyx_t_9; __pyx_t_11+=1) {
         __pyx_v_i = __pyx_t_11;
 
-        /* "View.MemoryView":181
+        /* "View.MemoryView":182
  *                 p = <PyObject **> self.data
  *                 for i in range(self.len / itemsize):
  *                     p[i] = Py_None             # <<<<<<<<<<<<<<
  *                     Py_INCREF(Py_None)
  * 
  */
-        __Pyx_TraceLine(181,0,__PYX_ERR(2, 181, __pyx_L1_error))
+        __Pyx_TraceLine(182,0,__PYX_ERR(2, 182, __pyx_L1_error))
         (__pyx_v_p[__pyx_v_i]) = Py_None;
 
-        /* "View.MemoryView":182
+        /* "View.MemoryView":183
  *                 for i in range(self.len / itemsize):
  *                     p[i] = Py_None
  *                     Py_INCREF(Py_None)             # <<<<<<<<<<<<<<
  * 
  *     @cname('getbuffer')
  */
-        __Pyx_TraceLine(182,0,__PYX_ERR(2, 182, __pyx_L1_error))
+        __Pyx_TraceLine(183,0,__PYX_ERR(2, 183, __pyx_L1_error))
         Py_INCREF(Py_None);
       }
 
-      /* "View.MemoryView":178
+      /* "View.MemoryView":179
  *                 raise MemoryError("unable to allocate array data.")
  * 
  *             if self.dtype_is_object:             # <<<<<<<<<<<<<<
  *                 p = <PyObject **> self.data
  *                 for i in range(self.len / itemsize):
  */
     }
 
-    /* "View.MemoryView":171
+    /* "View.MemoryView":172
  *         self.free_data = allocate_buffer
  *         self.dtype_is_object = format == b'O'
  *         if allocate_buffer:             # <<<<<<<<<<<<<<
  * 
  * 
  */
   }
 
-  /* "View.MemoryView":122
+  /* "View.MemoryView":123
  *         cdef bint dtype_is_object
  * 
  *     def __cinit__(array self, tuple shape, Py_ssize_t itemsize, format not None,             # <<<<<<<<<<<<<<
  *                   mode="c", bint allocate_buffer=True):
  * 
  */
 
@@ -17240,15 +17414,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_format);
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":185
+/* "View.MemoryView":186
  * 
  *     @cname('getbuffer')
  *     def __getbuffer__(self, Py_buffer *info, int flags):             # <<<<<<<<<<<<<<
  *         cdef int bufmode = -1
  *         if self.mode == u"c":
  */
 
@@ -17283,270 +17457,270 @@
   if (__pyx_v_info == NULL) {
     PyErr_SetString(PyExc_BufferError, "PyObject_GetBuffer: view==NULL argument is obsolete");
     return -1;
   }
   __Pyx_RefNannySetupContext("__getbuffer__", 0);
   __pyx_v_info->obj = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(__pyx_v_info->obj);
-  __Pyx_TraceCall("__getbuffer__", __pyx_f[2], 185, 0, __PYX_ERR(2, 185, __pyx_L1_error));
+  __Pyx_TraceCall("__getbuffer__", __pyx_f[2], 186, 0, __PYX_ERR(2, 186, __pyx_L1_error));
 
-  /* "View.MemoryView":186
+  /* "View.MemoryView":187
  *     @cname('getbuffer')
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         cdef int bufmode = -1             # <<<<<<<<<<<<<<
  *         if self.mode == u"c":
  *             bufmode = PyBUF_C_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  */
-  __Pyx_TraceLine(186,0,__PYX_ERR(2, 186, __pyx_L1_error))
+  __Pyx_TraceLine(187,0,__PYX_ERR(2, 187, __pyx_L1_error))
   __pyx_v_bufmode = -1;
 
-  /* "View.MemoryView":187
+  /* "View.MemoryView":188
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         cdef int bufmode = -1
  *         if self.mode == u"c":             # <<<<<<<<<<<<<<
  *             bufmode = PyBUF_C_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         elif self.mode == u"fortran":
  */
-  __Pyx_TraceLine(187,0,__PYX_ERR(2, 187, __pyx_L1_error))
-  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_self->mode, __pyx_n_u_c, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(2, 187, __pyx_L1_error)
+  __Pyx_TraceLine(188,0,__PYX_ERR(2, 188, __pyx_L1_error))
+  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_self->mode, __pyx_n_u_c, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(2, 188, __pyx_L1_error)
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":188
+    /* "View.MemoryView":189
  *         cdef int bufmode = -1
  *         if self.mode == u"c":
  *             bufmode = PyBUF_C_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS             # <<<<<<<<<<<<<<
  *         elif self.mode == u"fortran":
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  */
-    __Pyx_TraceLine(188,0,__PYX_ERR(2, 188, __pyx_L1_error))
+    __Pyx_TraceLine(189,0,__PYX_ERR(2, 189, __pyx_L1_error))
     __pyx_v_bufmode = (PyBUF_C_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS);
 
-    /* "View.MemoryView":187
+    /* "View.MemoryView":188
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         cdef int bufmode = -1
  *         if self.mode == u"c":             # <<<<<<<<<<<<<<
  *             bufmode = PyBUF_C_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         elif self.mode == u"fortran":
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":189
+  /* "View.MemoryView":190
  *         if self.mode == u"c":
  *             bufmode = PyBUF_C_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         elif self.mode == u"fortran":             # <<<<<<<<<<<<<<
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         if not (flags & bufmode):
  */
-  __Pyx_TraceLine(189,0,__PYX_ERR(2, 189, __pyx_L1_error))
-  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_self->mode, __pyx_n_u_fortran, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(2, 189, __pyx_L1_error)
+  __Pyx_TraceLine(190,0,__PYX_ERR(2, 190, __pyx_L1_error))
+  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_self->mode, __pyx_n_u_fortran, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(2, 190, __pyx_L1_error)
   __pyx_t_1 = (__pyx_t_2 != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":190
+    /* "View.MemoryView":191
  *             bufmode = PyBUF_C_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         elif self.mode == u"fortran":
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS             # <<<<<<<<<<<<<<
  *         if not (flags & bufmode):
  *             raise ValueError("Can only create a buffer that is contiguous in memory.")
  */
-    __Pyx_TraceLine(190,0,__PYX_ERR(2, 190, __pyx_L1_error))
+    __Pyx_TraceLine(191,0,__PYX_ERR(2, 191, __pyx_L1_error))
     __pyx_v_bufmode = (PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS);
 
-    /* "View.MemoryView":189
+    /* "View.MemoryView":190
  *         if self.mode == u"c":
  *             bufmode = PyBUF_C_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         elif self.mode == u"fortran":             # <<<<<<<<<<<<<<
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         if not (flags & bufmode):
  */
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":191
+  /* "View.MemoryView":192
  *         elif self.mode == u"fortran":
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         if not (flags & bufmode):             # <<<<<<<<<<<<<<
  *             raise ValueError("Can only create a buffer that is contiguous in memory.")
  *         info.buf = self.data
  */
-  __Pyx_TraceLine(191,0,__PYX_ERR(2, 191, __pyx_L1_error))
+  __Pyx_TraceLine(192,0,__PYX_ERR(2, 192, __pyx_L1_error))
   __pyx_t_1 = ((!((__pyx_v_flags & __pyx_v_bufmode) != 0)) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "View.MemoryView":192
+    /* "View.MemoryView":193
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         if not (flags & bufmode):
  *             raise ValueError("Can only create a buffer that is contiguous in memory.")             # <<<<<<<<<<<<<<
  *         info.buf = self.data
  *         info.len = self.len
  */
-    __Pyx_TraceLine(192,0,__PYX_ERR(2, 192, __pyx_L1_error))
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__15, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 192, __pyx_L1_error)
+    __Pyx_TraceLine(193,0,__PYX_ERR(2, 193, __pyx_L1_error))
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 193, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(2, 192, __pyx_L1_error)
+    __PYX_ERR(2, 193, __pyx_L1_error)
 
-    /* "View.MemoryView":191
+    /* "View.MemoryView":192
  *         elif self.mode == u"fortran":
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         if not (flags & bufmode):             # <<<<<<<<<<<<<<
  *             raise ValueError("Can only create a buffer that is contiguous in memory.")
  *         info.buf = self.data
  */
   }
 
-  /* "View.MemoryView":193
+  /* "View.MemoryView":194
  *         if not (flags & bufmode):
  *             raise ValueError("Can only create a buffer that is contiguous in memory.")
  *         info.buf = self.data             # <<<<<<<<<<<<<<
  *         info.len = self.len
  *         info.ndim = self.ndim
  */
-  __Pyx_TraceLine(193,0,__PYX_ERR(2, 193, __pyx_L1_error))
+  __Pyx_TraceLine(194,0,__PYX_ERR(2, 194, __pyx_L1_error))
   __pyx_t_4 = __pyx_v_self->data;
   __pyx_v_info->buf = __pyx_t_4;
 
-  /* "View.MemoryView":194
+  /* "View.MemoryView":195
  *             raise ValueError("Can only create a buffer that is contiguous in memory.")
  *         info.buf = self.data
  *         info.len = self.len             # <<<<<<<<<<<<<<
  *         info.ndim = self.ndim
  *         info.shape = self._shape
  */
-  __Pyx_TraceLine(194,0,__PYX_ERR(2, 194, __pyx_L1_error))
+  __Pyx_TraceLine(195,0,__PYX_ERR(2, 195, __pyx_L1_error))
   __pyx_t_5 = __pyx_v_self->len;
   __pyx_v_info->len = __pyx_t_5;
 
-  /* "View.MemoryView":195
+  /* "View.MemoryView":196
  *         info.buf = self.data
  *         info.len = self.len
  *         info.ndim = self.ndim             # <<<<<<<<<<<<<<
  *         info.shape = self._shape
  *         info.strides = self._strides
  */
-  __Pyx_TraceLine(195,0,__PYX_ERR(2, 195, __pyx_L1_error))
+  __Pyx_TraceLine(196,0,__PYX_ERR(2, 196, __pyx_L1_error))
   __pyx_t_6 = __pyx_v_self->ndim;
   __pyx_v_info->ndim = __pyx_t_6;
 
-  /* "View.MemoryView":196
+  /* "View.MemoryView":197
  *         info.len = self.len
  *         info.ndim = self.ndim
  *         info.shape = self._shape             # <<<<<<<<<<<<<<
  *         info.strides = self._strides
  *         info.suboffsets = NULL
  */
-  __Pyx_TraceLine(196,0,__PYX_ERR(2, 196, __pyx_L1_error))
+  __Pyx_TraceLine(197,0,__PYX_ERR(2, 197, __pyx_L1_error))
   __pyx_t_7 = __pyx_v_self->_shape;
   __pyx_v_info->shape = __pyx_t_7;
 
-  /* "View.MemoryView":197
+  /* "View.MemoryView":198
  *         info.ndim = self.ndim
  *         info.shape = self._shape
  *         info.strides = self._strides             # <<<<<<<<<<<<<<
  *         info.suboffsets = NULL
  *         info.itemsize = self.itemsize
  */
-  __Pyx_TraceLine(197,0,__PYX_ERR(2, 197, __pyx_L1_error))
+  __Pyx_TraceLine(198,0,__PYX_ERR(2, 198, __pyx_L1_error))
   __pyx_t_7 = __pyx_v_self->_strides;
   __pyx_v_info->strides = __pyx_t_7;
 
-  /* "View.MemoryView":198
+  /* "View.MemoryView":199
  *         info.shape = self._shape
  *         info.strides = self._strides
  *         info.suboffsets = NULL             # <<<<<<<<<<<<<<
  *         info.itemsize = self.itemsize
  *         info.readonly = 0
  */
-  __Pyx_TraceLine(198,0,__PYX_ERR(2, 198, __pyx_L1_error))
+  __Pyx_TraceLine(199,0,__PYX_ERR(2, 199, __pyx_L1_error))
   __pyx_v_info->suboffsets = NULL;
 
-  /* "View.MemoryView":199
+  /* "View.MemoryView":200
  *         info.strides = self._strides
  *         info.suboffsets = NULL
  *         info.itemsize = self.itemsize             # <<<<<<<<<<<<<<
  *         info.readonly = 0
  * 
  */
-  __Pyx_TraceLine(199,0,__PYX_ERR(2, 199, __pyx_L1_error))
+  __Pyx_TraceLine(200,0,__PYX_ERR(2, 200, __pyx_L1_error))
   __pyx_t_5 = __pyx_v_self->itemsize;
   __pyx_v_info->itemsize = __pyx_t_5;
 
-  /* "View.MemoryView":200
+  /* "View.MemoryView":201
  *         info.suboffsets = NULL
  *         info.itemsize = self.itemsize
  *         info.readonly = 0             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_FORMAT:
  */
-  __Pyx_TraceLine(200,0,__PYX_ERR(2, 200, __pyx_L1_error))
+  __Pyx_TraceLine(201,0,__PYX_ERR(2, 201, __pyx_L1_error))
   __pyx_v_info->readonly = 0;
 
-  /* "View.MemoryView":202
+  /* "View.MemoryView":203
  *         info.readonly = 0
  * 
  *         if flags & PyBUF_FORMAT:             # <<<<<<<<<<<<<<
  *             info.format = self.format
  *         else:
  */
-  __Pyx_TraceLine(202,0,__PYX_ERR(2, 202, __pyx_L1_error))
+  __Pyx_TraceLine(203,0,__PYX_ERR(2, 203, __pyx_L1_error))
   __pyx_t_1 = ((__pyx_v_flags & PyBUF_FORMAT) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":203
+    /* "View.MemoryView":204
  * 
  *         if flags & PyBUF_FORMAT:
  *             info.format = self.format             # <<<<<<<<<<<<<<
  *         else:
  *             info.format = NULL
  */
-    __Pyx_TraceLine(203,0,__PYX_ERR(2, 203, __pyx_L1_error))
+    __Pyx_TraceLine(204,0,__PYX_ERR(2, 204, __pyx_L1_error))
     __pyx_t_4 = __pyx_v_self->format;
     __pyx_v_info->format = __pyx_t_4;
 
-    /* "View.MemoryView":202
+    /* "View.MemoryView":203
  *         info.readonly = 0
  * 
  *         if flags & PyBUF_FORMAT:             # <<<<<<<<<<<<<<
  *             info.format = self.format
  *         else:
  */
     goto __pyx_L5;
   }
 
-  /* "View.MemoryView":205
+  /* "View.MemoryView":206
  *             info.format = self.format
  *         else:
  *             info.format = NULL             # <<<<<<<<<<<<<<
  * 
  *         info.obj = self
  */
-  __Pyx_TraceLine(205,0,__PYX_ERR(2, 205, __pyx_L1_error))
+  __Pyx_TraceLine(206,0,__PYX_ERR(2, 206, __pyx_L1_error))
   /*else*/ {
     __pyx_v_info->format = NULL;
   }
   __pyx_L5:;
 
-  /* "View.MemoryView":207
+  /* "View.MemoryView":208
  *             info.format = NULL
  * 
  *         info.obj = self             # <<<<<<<<<<<<<<
  * 
  *     __pyx_getbuffer = capsule(<void *> &__pyx_array_getbuffer, "getbuffer(obj, view, flags)")
  */
-  __Pyx_TraceLine(207,0,__PYX_ERR(2, 207, __pyx_L1_error))
+  __Pyx_TraceLine(208,0,__PYX_ERR(2, 208, __pyx_L1_error))
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_self));
   __Pyx_GOTREF(__pyx_v_info->obj);
   __Pyx_DECREF(__pyx_v_info->obj);
   __pyx_v_info->obj = ((PyObject *)__pyx_v_self);
 
-  /* "View.MemoryView":185
+  /* "View.MemoryView":186
  * 
  *     @cname('getbuffer')
  *     def __getbuffer__(self, Py_buffer *info, int flags):             # <<<<<<<<<<<<<<
  *         cdef int bufmode = -1
  *         if self.mode == u"c":
  */
 
@@ -17569,15 +17743,15 @@
   }
   __pyx_L2:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":211
+/* "View.MemoryView":212
  *     __pyx_getbuffer = capsule(<void *> &__pyx_array_getbuffer, "getbuffer(obj, view, flags)")
  * 
  *     def __dealloc__(array self):             # <<<<<<<<<<<<<<
  *         if self.callback_free_data != NULL:
  *             self.callback_free_data(self.data)
  */
 
@@ -17596,119 +17770,119 @@
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__dealloc__", 0);
-  __Pyx_TraceCall("__dealloc__", __pyx_f[2], 211, 0, __PYX_ERR(2, 211, __pyx_L1_error));
+  __Pyx_TraceCall("__dealloc__", __pyx_f[2], 212, 0, __PYX_ERR(2, 212, __pyx_L1_error));
 
-  /* "View.MemoryView":212
+  /* "View.MemoryView":213
  * 
  *     def __dealloc__(array self):
  *         if self.callback_free_data != NULL:             # <<<<<<<<<<<<<<
  *             self.callback_free_data(self.data)
  *         elif self.free_data:
  */
-  __Pyx_TraceLine(212,0,__PYX_ERR(2, 212, __pyx_L1_error))
+  __Pyx_TraceLine(213,0,__PYX_ERR(2, 213, __pyx_L1_error))
   __pyx_t_1 = ((__pyx_v_self->callback_free_data != NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":213
+    /* "View.MemoryView":214
  *     def __dealloc__(array self):
  *         if self.callback_free_data != NULL:
  *             self.callback_free_data(self.data)             # <<<<<<<<<<<<<<
  *         elif self.free_data:
  *             if self.dtype_is_object:
  */
-    __Pyx_TraceLine(213,0,__PYX_ERR(2, 213, __pyx_L1_error))
+    __Pyx_TraceLine(214,0,__PYX_ERR(2, 214, __pyx_L1_error))
     __pyx_v_self->callback_free_data(__pyx_v_self->data);
 
-    /* "View.MemoryView":212
+    /* "View.MemoryView":213
  * 
  *     def __dealloc__(array self):
  *         if self.callback_free_data != NULL:             # <<<<<<<<<<<<<<
  *             self.callback_free_data(self.data)
  *         elif self.free_data:
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":214
+  /* "View.MemoryView":215
  *         if self.callback_free_data != NULL:
  *             self.callback_free_data(self.data)
  *         elif self.free_data:             # <<<<<<<<<<<<<<
  *             if self.dtype_is_object:
  *                 refcount_objects_in_slice(self.data, self._shape,
  */
-  __Pyx_TraceLine(214,0,__PYX_ERR(2, 214, __pyx_L1_error))
+  __Pyx_TraceLine(215,0,__PYX_ERR(2, 215, __pyx_L1_error))
   __pyx_t_1 = (__pyx_v_self->free_data != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":215
+    /* "View.MemoryView":216
  *             self.callback_free_data(self.data)
  *         elif self.free_data:
  *             if self.dtype_is_object:             # <<<<<<<<<<<<<<
  *                 refcount_objects_in_slice(self.data, self._shape,
  *                                           self._strides, self.ndim, False)
  */
-    __Pyx_TraceLine(215,0,__PYX_ERR(2, 215, __pyx_L1_error))
+    __Pyx_TraceLine(216,0,__PYX_ERR(2, 216, __pyx_L1_error))
     __pyx_t_1 = (__pyx_v_self->dtype_is_object != 0);
     if (__pyx_t_1) {
 
-      /* "View.MemoryView":216
+      /* "View.MemoryView":217
  *         elif self.free_data:
  *             if self.dtype_is_object:
  *                 refcount_objects_in_slice(self.data, self._shape,             # <<<<<<<<<<<<<<
  *                                           self._strides, self.ndim, False)
  *             free(self.data)
  */
-      __Pyx_TraceLine(216,0,__PYX_ERR(2, 216, __pyx_L1_error))
+      __Pyx_TraceLine(217,0,__PYX_ERR(2, 217, __pyx_L1_error))
       __pyx_memoryview_refcount_objects_in_slice(__pyx_v_self->data, __pyx_v_self->_shape, __pyx_v_self->_strides, __pyx_v_self->ndim, 0);
 
-      /* "View.MemoryView":215
+      /* "View.MemoryView":216
  *             self.callback_free_data(self.data)
  *         elif self.free_data:
  *             if self.dtype_is_object:             # <<<<<<<<<<<<<<
  *                 refcount_objects_in_slice(self.data, self._shape,
  *                                           self._strides, self.ndim, False)
  */
     }
 
-    /* "View.MemoryView":218
+    /* "View.MemoryView":219
  *                 refcount_objects_in_slice(self.data, self._shape,
  *                                           self._strides, self.ndim, False)
  *             free(self.data)             # <<<<<<<<<<<<<<
  *         PyObject_Free(self._shape)
  * 
  */
-    __Pyx_TraceLine(218,0,__PYX_ERR(2, 218, __pyx_L1_error))
+    __Pyx_TraceLine(219,0,__PYX_ERR(2, 219, __pyx_L1_error))
     free(__pyx_v_self->data);
 
-    /* "View.MemoryView":214
+    /* "View.MemoryView":215
  *         if self.callback_free_data != NULL:
  *             self.callback_free_data(self.data)
  *         elif self.free_data:             # <<<<<<<<<<<<<<
  *             if self.dtype_is_object:
  *                 refcount_objects_in_slice(self.data, self._shape,
  */
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":219
+  /* "View.MemoryView":220
  *                                           self._strides, self.ndim, False)
  *             free(self.data)
  *         PyObject_Free(self._shape)             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
-  __Pyx_TraceLine(219,0,__PYX_ERR(2, 219, __pyx_L1_error))
+  __Pyx_TraceLine(220,0,__PYX_ERR(2, 220, __pyx_L1_error))
   PyObject_Free(__pyx_v_self->_shape);
 
-  /* "View.MemoryView":211
+  /* "View.MemoryView":212
  *     __pyx_getbuffer = capsule(<void *> &__pyx_array_getbuffer, "getbuffer(obj, view, flags)")
  * 
  *     def __dealloc__(array self):             # <<<<<<<<<<<<<<
  *         if self.callback_free_data != NULL:
  *             self.callback_free_data(self.data)
  */
 
@@ -17717,15 +17891,15 @@
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("View.MemoryView.array.__dealloc__", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
 }
 
-/* "View.MemoryView":222
+/* "View.MemoryView":223
  * 
  *     @property
  *     def memview(self):             # <<<<<<<<<<<<<<
  *         return self.get_memview()
  * 
  */
 
@@ -17747,32 +17921,32 @@
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
-  __Pyx_TraceCall("__get__", __pyx_f[2], 222, 0, __PYX_ERR(2, 222, __pyx_L1_error));
+  __Pyx_TraceCall("__get__", __pyx_f[2], 223, 0, __PYX_ERR(2, 223, __pyx_L1_error));
 
-  /* "View.MemoryView":223
+  /* "View.MemoryView":224
  *     @property
  *     def memview(self):
  *         return self.get_memview()             # <<<<<<<<<<<<<<
  * 
  *     @cname('get_memview')
  */
-  __Pyx_TraceLine(223,0,__PYX_ERR(2, 223, __pyx_L1_error))
+  __Pyx_TraceLine(224,0,__PYX_ERR(2, 224, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = ((struct __pyx_vtabstruct_array *)__pyx_v_self->__pyx_vtab)->get_memview(__pyx_v_self); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 223, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_array *)__pyx_v_self->__pyx_vtab)->get_memview(__pyx_v_self); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 224, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":222
+  /* "View.MemoryView":223
  * 
  *     @property
  *     def memview(self):             # <<<<<<<<<<<<<<
  *         return self.get_memview()
  * 
  */
 
@@ -17784,15 +17958,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":226
+/* "View.MemoryView":227
  * 
  *     @cname('get_memview')
  *     cdef get_memview(self):             # <<<<<<<<<<<<<<
  *         flags =  PyBUF_ANY_CONTIGUOUS|PyBUF_FORMAT|PyBUF_WRITABLE
  *         return  memoryview(self, flags, self.dtype_is_object)
  */
 
@@ -17804,58 +17978,58 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_memview", 0);
-  __Pyx_TraceCall("get_memview", __pyx_f[2], 226, 0, __PYX_ERR(2, 226, __pyx_L1_error));
+  __Pyx_TraceCall("get_memview", __pyx_f[2], 227, 0, __PYX_ERR(2, 227, __pyx_L1_error));
 
-  /* "View.MemoryView":227
+  /* "View.MemoryView":228
  *     @cname('get_memview')
  *     cdef get_memview(self):
  *         flags =  PyBUF_ANY_CONTIGUOUS|PyBUF_FORMAT|PyBUF_WRITABLE             # <<<<<<<<<<<<<<
  *         return  memoryview(self, flags, self.dtype_is_object)
  * 
  */
-  __Pyx_TraceLine(227,0,__PYX_ERR(2, 227, __pyx_L1_error))
+  __Pyx_TraceLine(228,0,__PYX_ERR(2, 228, __pyx_L1_error))
   __pyx_v_flags = ((PyBUF_ANY_CONTIGUOUS | PyBUF_FORMAT) | PyBUF_WRITABLE);
 
-  /* "View.MemoryView":228
+  /* "View.MemoryView":229
  *     cdef get_memview(self):
  *         flags =  PyBUF_ANY_CONTIGUOUS|PyBUF_FORMAT|PyBUF_WRITABLE
  *         return  memoryview(self, flags, self.dtype_is_object)             # <<<<<<<<<<<<<<
  * 
  *     def __len__(self):
  */
-  __Pyx_TraceLine(228,0,__PYX_ERR(2, 228, __pyx_L1_error))
+  __Pyx_TraceLine(229,0,__PYX_ERR(2, 229, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_flags); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 228, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_flags); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 229, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_v_self->dtype_is_object); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 228, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_v_self->dtype_is_object); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 229, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 228, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 229, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_self));
   PyTuple_SET_ITEM(__pyx_t_3, 0, ((PyObject *)__pyx_v_self));
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_t_2);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_memoryview_type), __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 228, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_memoryview_type), __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 229, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":226
+  /* "View.MemoryView":227
  * 
  *     @cname('get_memview')
  *     cdef get_memview(self):             # <<<<<<<<<<<<<<
  *         flags =  PyBUF_ANY_CONTIGUOUS|PyBUF_FORMAT|PyBUF_WRITABLE
  *         return  memoryview(self, flags, self.dtype_is_object)
  */
 
@@ -17869,15 +18043,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":230
+/* "View.MemoryView":231
  *         return  memoryview(self, flags, self.dtype_is_object)
  * 
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         return self._shape[0]
  * 
  */
 
@@ -17898,28 +18072,28 @@
   Py_ssize_t __pyx_r;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__len__", 0);
-  __Pyx_TraceCall("__len__", __pyx_f[2], 230, 0, __PYX_ERR(2, 230, __pyx_L1_error));
+  __Pyx_TraceCall("__len__", __pyx_f[2], 231, 0, __PYX_ERR(2, 231, __pyx_L1_error));
 
-  /* "View.MemoryView":231
+  /* "View.MemoryView":232
  * 
  *     def __len__(self):
  *         return self._shape[0]             # <<<<<<<<<<<<<<
  * 
  *     def __getattr__(self, attr):
  */
-  __Pyx_TraceLine(231,0,__PYX_ERR(2, 231, __pyx_L1_error))
+  __Pyx_TraceLine(232,0,__PYX_ERR(2, 232, __pyx_L1_error))
   __pyx_r = (__pyx_v_self->_shape[0]);
   goto __pyx_L0;
 
-  /* "View.MemoryView":230
+  /* "View.MemoryView":231
  *         return  memoryview(self, flags, self.dtype_is_object)
  * 
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         return self._shape[0]
  * 
  */
 
@@ -17929,15 +18103,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":233
+/* "View.MemoryView":234
  *         return self._shape[0]
  * 
  *     def __getattr__(self, attr):             # <<<<<<<<<<<<<<
  *         return getattr(self.memview, attr)
  * 
  */
 
@@ -17960,35 +18134,35 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__getattr__", 0);
-  __Pyx_TraceCall("__getattr__", __pyx_f[2], 233, 0, __PYX_ERR(2, 233, __pyx_L1_error));
+  __Pyx_TraceCall("__getattr__", __pyx_f[2], 234, 0, __PYX_ERR(2, 234, __pyx_L1_error));
 
-  /* "View.MemoryView":234
+  /* "View.MemoryView":235
  * 
  *     def __getattr__(self, attr):
  *         return getattr(self.memview, attr)             # <<<<<<<<<<<<<<
  * 
  *     def __getitem__(self, item):
  */
-  __Pyx_TraceLine(234,0,__PYX_ERR(2, 234, __pyx_L1_error))
+  __Pyx_TraceLine(235,0,__PYX_ERR(2, 235, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_memview); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 234, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_memview); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 235, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_GetAttr(__pyx_t_1, __pyx_v_attr); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 234, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetAttr(__pyx_t_1, __pyx_v_attr); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 235, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":233
+  /* "View.MemoryView":234
  *         return self._shape[0]
  * 
  *     def __getattr__(self, attr):             # <<<<<<<<<<<<<<
  *         return getattr(self.memview, attr)
  * 
  */
 
@@ -18001,15 +18175,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":236
+/* "View.MemoryView":237
  *         return getattr(self.memview, attr)
  * 
  *     def __getitem__(self, item):             # <<<<<<<<<<<<<<
  *         return self.memview[item]
  * 
  */
 
@@ -18032,35 +18206,35 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__getitem__", 0);
-  __Pyx_TraceCall("__getitem__", __pyx_f[2], 236, 0, __PYX_ERR(2, 236, __pyx_L1_error));
+  __Pyx_TraceCall("__getitem__", __pyx_f[2], 237, 0, __PYX_ERR(2, 237, __pyx_L1_error));
 
-  /* "View.MemoryView":237
+  /* "View.MemoryView":238
  * 
  *     def __getitem__(self, item):
  *         return self.memview[item]             # <<<<<<<<<<<<<<
  * 
  *     def __setitem__(self, item, value):
  */
-  __Pyx_TraceLine(237,0,__PYX_ERR(2, 237, __pyx_L1_error))
+  __Pyx_TraceLine(238,0,__PYX_ERR(2, 238, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_memview); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 237, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_memview); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 238, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_v_item); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 237, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_v_item); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 238, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":236
+  /* "View.MemoryView":237
  *         return getattr(self.memview, attr)
  * 
  *     def __getitem__(self, item):             # <<<<<<<<<<<<<<
  *         return self.memview[item]
  * 
  */
 
@@ -18073,15 +18247,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":239
+/* "View.MemoryView":240
  *         return self.memview[item]
  * 
  *     def __setitem__(self, item, value):             # <<<<<<<<<<<<<<
  *         self.memview[item] = value
  * 
  */
 
@@ -18103,30 +18277,30 @@
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setitem__", 0);
-  __Pyx_TraceCall("__setitem__", __pyx_f[2], 239, 0, __PYX_ERR(2, 239, __pyx_L1_error));
+  __Pyx_TraceCall("__setitem__", __pyx_f[2], 240, 0, __PYX_ERR(2, 240, __pyx_L1_error));
 
-  /* "View.MemoryView":240
+  /* "View.MemoryView":241
  * 
  *     def __setitem__(self, item, value):
  *         self.memview[item] = value             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_TraceLine(240,0,__PYX_ERR(2, 240, __pyx_L1_error))
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_memview); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 240, __pyx_L1_error)
+  __Pyx_TraceLine(241,0,__PYX_ERR(2, 241, __pyx_L1_error))
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_memview); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 241, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (unlikely(PyObject_SetItem(__pyx_t_1, __pyx_v_item, __pyx_v_value) < 0)) __PYX_ERR(2, 240, __pyx_L1_error)
+  if (unlikely(PyObject_SetItem(__pyx_t_1, __pyx_v_item, __pyx_v_value) < 0)) __PYX_ERR(2, 241, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "View.MemoryView":239
+  /* "View.MemoryView":240
  *         return self.memview[item]
  * 
  *     def __setitem__(self, item, value):             # <<<<<<<<<<<<<<
  *         self.memview[item] = value
  * 
  */
 
@@ -18176,15 +18350,15 @@
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
   __Pyx_TraceLine(2,0,__PYX_ERR(2, 2, __pyx_L1_error))
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__17, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(2, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
@@ -18236,15 +18410,15 @@
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __Pyx_TraceLine(4,0,__PYX_ERR(2, 4, __pyx_L1_error))
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__17, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__18, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(2, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
@@ -18260,15 +18434,15 @@
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":244
+/* "View.MemoryView":245
  * 
  * @cname("__pyx_array_new")
  * cdef array array_cwrapper(tuple shape, Py_ssize_t itemsize, char *format,             # <<<<<<<<<<<<<<
  *                           char *mode, char *buf):
  *     cdef array result
  */
 
@@ -18282,154 +18456,154 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("array_cwrapper", 0);
-  __Pyx_TraceCall("array_cwrapper", __pyx_f[2], 244, 0, __PYX_ERR(2, 244, __pyx_L1_error));
+  __Pyx_TraceCall("array_cwrapper", __pyx_f[2], 245, 0, __PYX_ERR(2, 245, __pyx_L1_error));
 
-  /* "View.MemoryView":248
+  /* "View.MemoryView":249
  *     cdef array result
  * 
  *     if buf == NULL:             # <<<<<<<<<<<<<<
  *         result = array(shape, itemsize, format, mode.decode('ASCII'))
  *     else:
  */
-  __Pyx_TraceLine(248,0,__PYX_ERR(2, 248, __pyx_L1_error))
+  __Pyx_TraceLine(249,0,__PYX_ERR(2, 249, __pyx_L1_error))
   __pyx_t_1 = ((__pyx_v_buf == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":249
+    /* "View.MemoryView":250
  * 
  *     if buf == NULL:
  *         result = array(shape, itemsize, format, mode.decode('ASCII'))             # <<<<<<<<<<<<<<
  *     else:
  *         result = array(shape, itemsize, format, mode.decode('ASCII'),
  */
-    __Pyx_TraceLine(249,0,__PYX_ERR(2, 249, __pyx_L1_error))
-    __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_itemsize); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 249, __pyx_L1_error)
+    __Pyx_TraceLine(250,0,__PYX_ERR(2, 250, __pyx_L1_error))
+    __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_itemsize); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 250, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyBytes_FromString(__pyx_v_format); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 249, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyBytes_FromString(__pyx_v_format); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 250, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_decode_c_string(__pyx_v_mode, 0, strlen(__pyx_v_mode), NULL, NULL, PyUnicode_DecodeASCII); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 249, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_decode_c_string(__pyx_v_mode, 0, strlen(__pyx_v_mode), NULL, NULL, PyUnicode_DecodeASCII); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 250, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = PyTuple_New(4); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 249, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(4); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 250, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_INCREF(__pyx_v_shape);
     __Pyx_GIVEREF(__pyx_v_shape);
     PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_shape);
     __Pyx_GIVEREF(__pyx_t_2);
     PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_5, 3, __pyx_t_4);
     __pyx_t_2 = 0;
     __pyx_t_3 = 0;
     __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_array_type), __pyx_t_5, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 249, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_array_type), __pyx_t_5, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 250, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_v_result = ((struct __pyx_array_obj *)__pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "View.MemoryView":248
+    /* "View.MemoryView":249
  *     cdef array result
  * 
  *     if buf == NULL:             # <<<<<<<<<<<<<<
  *         result = array(shape, itemsize, format, mode.decode('ASCII'))
  *     else:
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":251
+  /* "View.MemoryView":252
  *         result = array(shape, itemsize, format, mode.decode('ASCII'))
  *     else:
  *         result = array(shape, itemsize, format, mode.decode('ASCII'),             # <<<<<<<<<<<<<<
  *                        allocate_buffer=False)
  *         result.data = buf
  */
-  __Pyx_TraceLine(251,0,__PYX_ERR(2, 251, __pyx_L1_error))
+  __Pyx_TraceLine(252,0,__PYX_ERR(2, 252, __pyx_L1_error))
   /*else*/ {
-    __pyx_t_4 = PyInt_FromSsize_t(__pyx_v_itemsize); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 251, __pyx_L1_error)
+    __pyx_t_4 = PyInt_FromSsize_t(__pyx_v_itemsize); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 252, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyBytes_FromString(__pyx_v_format); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 251, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyBytes_FromString(__pyx_v_format); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 252, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_3 = __Pyx_decode_c_string(__pyx_v_mode, 0, strlen(__pyx_v_mode), NULL, NULL, PyUnicode_DecodeASCII); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 251, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_decode_c_string(__pyx_v_mode, 0, strlen(__pyx_v_mode), NULL, NULL, PyUnicode_DecodeASCII); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 252, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_2 = PyTuple_New(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 251, __pyx_L1_error)
+    __pyx_t_2 = PyTuple_New(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 252, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_INCREF(__pyx_v_shape);
     __Pyx_GIVEREF(__pyx_v_shape);
     PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_shape);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_2, 2, __pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_2, 3, __pyx_t_3);
     __pyx_t_4 = 0;
     __pyx_t_5 = 0;
     __pyx_t_3 = 0;
 
-    /* "View.MemoryView":252
+    /* "View.MemoryView":253
  *     else:
  *         result = array(shape, itemsize, format, mode.decode('ASCII'),
  *                        allocate_buffer=False)             # <<<<<<<<<<<<<<
  *         result.data = buf
  * 
  */
-    __Pyx_TraceLine(252,0,__PYX_ERR(2, 252, __pyx_L1_error))
-    __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 252, __pyx_L1_error)
+    __Pyx_TraceLine(253,0,__PYX_ERR(2, 253, __pyx_L1_error))
+    __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 253, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_allocate_buffer, Py_False) < 0) __PYX_ERR(2, 252, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_allocate_buffer, Py_False) < 0) __PYX_ERR(2, 253, __pyx_L1_error)
 
-    /* "View.MemoryView":251
+    /* "View.MemoryView":252
  *         result = array(shape, itemsize, format, mode.decode('ASCII'))
  *     else:
  *         result = array(shape, itemsize, format, mode.decode('ASCII'),             # <<<<<<<<<<<<<<
  *                        allocate_buffer=False)
  *         result.data = buf
  */
-    __Pyx_TraceLine(251,0,__PYX_ERR(2, 251, __pyx_L1_error))
-    __pyx_t_5 = __Pyx_PyObject_Call(((PyObject *)__pyx_array_type), __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 251, __pyx_L1_error)
+    __Pyx_TraceLine(252,0,__PYX_ERR(2, 252, __pyx_L1_error))
+    __pyx_t_5 = __Pyx_PyObject_Call(((PyObject *)__pyx_array_type), __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 252, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_result = ((struct __pyx_array_obj *)__pyx_t_5);
     __pyx_t_5 = 0;
 
-    /* "View.MemoryView":253
+    /* "View.MemoryView":254
  *         result = array(shape, itemsize, format, mode.decode('ASCII'),
  *                        allocate_buffer=False)
  *         result.data = buf             # <<<<<<<<<<<<<<
  * 
  *     return result
  */
-    __Pyx_TraceLine(253,0,__PYX_ERR(2, 253, __pyx_L1_error))
+    __Pyx_TraceLine(254,0,__PYX_ERR(2, 254, __pyx_L1_error))
     __pyx_v_result->data = __pyx_v_buf;
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":255
+  /* "View.MemoryView":256
  *         result.data = buf
  * 
  *     return result             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_TraceLine(255,0,__PYX_ERR(2, 255, __pyx_L1_error))
+  __Pyx_TraceLine(256,0,__PYX_ERR(2, 256, __pyx_L1_error))
   __Pyx_XDECREF(((PyObject *)__pyx_r));
   __Pyx_INCREF(((PyObject *)__pyx_v_result));
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "View.MemoryView":244
+  /* "View.MemoryView":245
  * 
  * @cname("__pyx_array_new")
  * cdef array array_cwrapper(tuple shape, Py_ssize_t itemsize, char *format,             # <<<<<<<<<<<<<<
  *                           char *mode, char *buf):
  *     cdef array result
  */
 
@@ -18445,15 +18619,15 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_result);
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":281
+/* "View.MemoryView":282
  * cdef class Enum(object):
  *     cdef object name
  *     def __init__(self, name):             # <<<<<<<<<<<<<<
  *         self.name = name
  *     def __repr__(self):
  */
 
@@ -18482,26 +18656,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_name)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(2, 281, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(2, 282, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_name = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(2, 281, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(2, 282, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("View.MemoryView.Enum.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_MemviewEnum___pyx_pf_15View_dot_MemoryView_4Enum___init__(((struct __pyx_MemviewEnum_obj *)__pyx_v_self), __pyx_v_name);
 
@@ -18514,31 +18688,31 @@
   int __pyx_r;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
-  __Pyx_TraceCall("__init__", __pyx_f[2], 281, 0, __PYX_ERR(2, 281, __pyx_L1_error));
+  __Pyx_TraceCall("__init__", __pyx_f[2], 282, 0, __PYX_ERR(2, 282, __pyx_L1_error));
 
-  /* "View.MemoryView":282
+  /* "View.MemoryView":283
  *     cdef object name
  *     def __init__(self, name):
  *         self.name = name             # <<<<<<<<<<<<<<
  *     def __repr__(self):
  *         return self.name
  */
-  __Pyx_TraceLine(282,0,__PYX_ERR(2, 282, __pyx_L1_error))
+  __Pyx_TraceLine(283,0,__PYX_ERR(2, 283, __pyx_L1_error))
   __Pyx_INCREF(__pyx_v_name);
   __Pyx_GIVEREF(__pyx_v_name);
   __Pyx_GOTREF(__pyx_v_self->name);
   __Pyx_DECREF(__pyx_v_self->name);
   __pyx_v_self->name = __pyx_v_name;
 
-  /* "View.MemoryView":281
+  /* "View.MemoryView":282
  * cdef class Enum(object):
  *     cdef object name
  *     def __init__(self, name):             # <<<<<<<<<<<<<<
  *         self.name = name
  *     def __repr__(self):
  */
 
@@ -18550,15 +18724,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":283
+/* "View.MemoryView":284
  *     def __init__(self, name):
  *         self.name = name
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return self.name
  * 
  */
 
@@ -18579,30 +18753,30 @@
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__repr__", 0);
-  __Pyx_TraceCall("__repr__", __pyx_f[2], 283, 0, __PYX_ERR(2, 283, __pyx_L1_error));
+  __Pyx_TraceCall("__repr__", __pyx_f[2], 284, 0, __PYX_ERR(2, 284, __pyx_L1_error));
 
-  /* "View.MemoryView":284
+  /* "View.MemoryView":285
  *         self.name = name
  *     def __repr__(self):
  *         return self.name             # <<<<<<<<<<<<<<
  * 
  * cdef generic = Enum("<strided and direct or indirect>")
  */
-  __Pyx_TraceLine(284,0,__PYX_ERR(2, 284, __pyx_L1_error))
+  __Pyx_TraceLine(285,0,__PYX_ERR(2, 285, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_self->name);
   __pyx_r = __pyx_v_self->name;
   goto __pyx_L0;
 
-  /* "View.MemoryView":283
+  /* "View.MemoryView":284
  *     def __init__(self, name):
  *         self.name = name
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return self.name
  * 
  */
 
@@ -18896,15 +19070,15 @@
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_Enum, (type(self), 0xb068931, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_Enum__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
   __Pyx_TraceLine(17,0,__PYX_ERR(2, 17, __pyx_L1_error))
-  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(2, 17, __pyx_L1_error)
+  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(2, 17, __pyx_L1_error)
   __pyx_t_1 = __pyx_unpickle_Enum__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_Enum, (type(self), 0xb068931, state)
@@ -18922,15 +19096,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":298
+/* "View.MemoryView":299
  * 
  * @cname('__pyx_align_pointer')
  * cdef void *align_pointer(void *memory, size_t alignment) nogil:             # <<<<<<<<<<<<<<
  *     "Align pointer memory on a given boundary"
  *     cdef Py_intptr_t aligned_p = <Py_intptr_t> memory
  */
 
@@ -18939,77 +19113,77 @@
   size_t __pyx_v_offset;
   void *__pyx_r;
   __Pyx_TraceDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_TraceCall("align_pointer", __pyx_f[2], 298, 1, __PYX_ERR(2, 298, __pyx_L1_error));
+  __Pyx_TraceCall("align_pointer", __pyx_f[2], 299, 1, __PYX_ERR(2, 299, __pyx_L1_error));
 
-  /* "View.MemoryView":300
+  /* "View.MemoryView":301
  * cdef void *align_pointer(void *memory, size_t alignment) nogil:
  *     "Align pointer memory on a given boundary"
  *     cdef Py_intptr_t aligned_p = <Py_intptr_t> memory             # <<<<<<<<<<<<<<
  *     cdef size_t offset
  * 
  */
-  __Pyx_TraceLine(300,1,__PYX_ERR(2, 300, __pyx_L1_error))
+  __Pyx_TraceLine(301,1,__PYX_ERR(2, 301, __pyx_L1_error))
   __pyx_v_aligned_p = ((Py_intptr_t)__pyx_v_memory);
 
-  /* "View.MemoryView":304
+  /* "View.MemoryView":305
  * 
  *     with cython.cdivision(True):
  *         offset = aligned_p % alignment             # <<<<<<<<<<<<<<
  * 
  *     if offset > 0:
  */
   __pyx_v_offset = (__pyx_v_aligned_p % __pyx_v_alignment);
 
-  /* "View.MemoryView":306
+  /* "View.MemoryView":307
  *         offset = aligned_p % alignment
  * 
  *     if offset > 0:             # <<<<<<<<<<<<<<
  *         aligned_p += alignment - offset
  * 
  */
-  __Pyx_TraceLine(306,1,__PYX_ERR(2, 306, __pyx_L1_error))
+  __Pyx_TraceLine(307,1,__PYX_ERR(2, 307, __pyx_L1_error))
   __pyx_t_1 = ((__pyx_v_offset > 0) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":307
+    /* "View.MemoryView":308
  * 
  *     if offset > 0:
  *         aligned_p += alignment - offset             # <<<<<<<<<<<<<<
  * 
  *     return <void *> aligned_p
  */
-    __Pyx_TraceLine(307,1,__PYX_ERR(2, 307, __pyx_L1_error))
+    __Pyx_TraceLine(308,1,__PYX_ERR(2, 308, __pyx_L1_error))
     __pyx_v_aligned_p = (__pyx_v_aligned_p + (__pyx_v_alignment - __pyx_v_offset));
 
-    /* "View.MemoryView":306
+    /* "View.MemoryView":307
  *         offset = aligned_p % alignment
  * 
  *     if offset > 0:             # <<<<<<<<<<<<<<
  *         aligned_p += alignment - offset
  * 
  */
   }
 
-  /* "View.MemoryView":309
+  /* "View.MemoryView":310
  *         aligned_p += alignment - offset
  * 
  *     return <void *> aligned_p             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_TraceLine(309,1,__PYX_ERR(2, 309, __pyx_L1_error))
+  __Pyx_TraceLine(310,1,__PYX_ERR(2, 310, __pyx_L1_error))
   __pyx_r = ((void *)__pyx_v_aligned_p);
   goto __pyx_L0;
 
-  /* "View.MemoryView":298
+  /* "View.MemoryView":299
  * 
  * @cname('__pyx_align_pointer')
  * cdef void *align_pointer(void *memory, size_t alignment) nogil:             # <<<<<<<<<<<<<<
  *     "Align pointer memory on a given boundary"
  *     cdef Py_intptr_t aligned_p = <Py_intptr_t> memory
  */
 
@@ -19018,15 +19192,15 @@
   __Pyx_WriteUnraisable("View.MemoryView.align_pointer", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 1);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
   return __pyx_r;
 }
 
-/* "View.MemoryView":345
+/* "View.MemoryView":346
  *     cdef __Pyx_TypeInfo *typeinfo
  * 
  *     def __cinit__(memoryview self, object obj, int flags, bint dtype_is_object=False):             # <<<<<<<<<<<<<<
  *         self.obj = obj
  *         self.flags = flags
  */
 
@@ -19063,47 +19237,47 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_obj)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_flags)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 2, 3, 1); __PYX_ERR(2, 345, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 2, 3, 1); __PYX_ERR(2, 346, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_dtype_is_object);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(2, 345, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(2, 346, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_obj = values[0];
-    __pyx_v_flags = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_flags == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 345, __pyx_L3_error)
+    __pyx_v_flags = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_flags == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 346, __pyx_L3_error)
     if (values[2]) {
-      __pyx_v_dtype_is_object = __Pyx_PyObject_IsTrue(values[2]); if (unlikely((__pyx_v_dtype_is_object == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 345, __pyx_L3_error)
+      __pyx_v_dtype_is_object = __Pyx_PyObject_IsTrue(values[2]); if (unlikely((__pyx_v_dtype_is_object == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 346, __pyx_L3_error)
     } else {
       __pyx_v_dtype_is_object = ((int)0);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(2, 345, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(2, 346, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("View.MemoryView.memoryview.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview___cinit__(((struct __pyx_memoryview_obj *)__pyx_v_self), __pyx_v_obj, __pyx_v_flags, __pyx_v_dtype_is_object);
 
@@ -19120,294 +19294,314 @@
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
-  __Pyx_TraceCall("__cinit__", __pyx_f[2], 345, 0, __PYX_ERR(2, 345, __pyx_L1_error));
+  __Pyx_TraceCall("__cinit__", __pyx_f[2], 346, 0, __PYX_ERR(2, 346, __pyx_L1_error));
 
-  /* "View.MemoryView":346
+  /* "View.MemoryView":347
  * 
  *     def __cinit__(memoryview self, object obj, int flags, bint dtype_is_object=False):
  *         self.obj = obj             # <<<<<<<<<<<<<<
  *         self.flags = flags
  *         if type(self) is memoryview or obj is not None:
  */
-  __Pyx_TraceLine(346,0,__PYX_ERR(2, 346, __pyx_L1_error))
+  __Pyx_TraceLine(347,0,__PYX_ERR(2, 347, __pyx_L1_error))
   __Pyx_INCREF(__pyx_v_obj);
   __Pyx_GIVEREF(__pyx_v_obj);
   __Pyx_GOTREF(__pyx_v_self->obj);
   __Pyx_DECREF(__pyx_v_self->obj);
   __pyx_v_self->obj = __pyx_v_obj;
 
-  /* "View.MemoryView":347
+  /* "View.MemoryView":348
  *     def __cinit__(memoryview self, object obj, int flags, bint dtype_is_object=False):
  *         self.obj = obj
  *         self.flags = flags             # <<<<<<<<<<<<<<
  *         if type(self) is memoryview or obj is not None:
  *             __Pyx_GetBuffer(obj, &self.view, flags)
  */
-  __Pyx_TraceLine(347,0,__PYX_ERR(2, 347, __pyx_L1_error))
+  __Pyx_TraceLine(348,0,__PYX_ERR(2, 348, __pyx_L1_error))
   __pyx_v_self->flags = __pyx_v_flags;
 
-  /* "View.MemoryView":348
+  /* "View.MemoryView":349
  *         self.obj = obj
  *         self.flags = flags
  *         if type(self) is memoryview or obj is not None:             # <<<<<<<<<<<<<<
  *             __Pyx_GetBuffer(obj, &self.view, flags)
  *             if <PyObject *> self.view.obj == NULL:
  */
-  __Pyx_TraceLine(348,0,__PYX_ERR(2, 348, __pyx_L1_error))
+  __Pyx_TraceLine(349,0,__PYX_ERR(2, 349, __pyx_L1_error))
   __pyx_t_2 = (((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))) == ((PyObject *)__pyx_memoryview_type));
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (!__pyx_t_3) {
   } else {
     __pyx_t_1 = __pyx_t_3;
     goto __pyx_L4_bool_binop_done;
   }
   __pyx_t_3 = (__pyx_v_obj != Py_None);
   __pyx_t_2 = (__pyx_t_3 != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":349
+    /* "View.MemoryView":350
  *         self.flags = flags
  *         if type(self) is memoryview or obj is not None:
  *             __Pyx_GetBuffer(obj, &self.view, flags)             # <<<<<<<<<<<<<<
  *             if <PyObject *> self.view.obj == NULL:
  *                 (<__pyx_buffer *> &self.view).obj = Py_None
  */
-    __Pyx_TraceLine(349,0,__PYX_ERR(2, 349, __pyx_L1_error))
-    __pyx_t_4 = __Pyx_GetBuffer(__pyx_v_obj, (&__pyx_v_self->view), __pyx_v_flags); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 349, __pyx_L1_error)
+    __Pyx_TraceLine(350,0,__PYX_ERR(2, 350, __pyx_L1_error))
+    __pyx_t_4 = __Pyx_GetBuffer(__pyx_v_obj, (&__pyx_v_self->view), __pyx_v_flags); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 350, __pyx_L1_error)
 
-    /* "View.MemoryView":350
+    /* "View.MemoryView":351
  *         if type(self) is memoryview or obj is not None:
  *             __Pyx_GetBuffer(obj, &self.view, flags)
  *             if <PyObject *> self.view.obj == NULL:             # <<<<<<<<<<<<<<
  *                 (<__pyx_buffer *> &self.view).obj = Py_None
  *                 Py_INCREF(Py_None)
  */
-    __Pyx_TraceLine(350,0,__PYX_ERR(2, 350, __pyx_L1_error))
+    __Pyx_TraceLine(351,0,__PYX_ERR(2, 351, __pyx_L1_error))
     __pyx_t_1 = ((((PyObject *)__pyx_v_self->view.obj) == NULL) != 0);
     if (__pyx_t_1) {
 
-      /* "View.MemoryView":351
+      /* "View.MemoryView":352
  *             __Pyx_GetBuffer(obj, &self.view, flags)
  *             if <PyObject *> self.view.obj == NULL:
  *                 (<__pyx_buffer *> &self.view).obj = Py_None             # <<<<<<<<<<<<<<
  *                 Py_INCREF(Py_None)
  * 
  */
-      __Pyx_TraceLine(351,0,__PYX_ERR(2, 351, __pyx_L1_error))
+      __Pyx_TraceLine(352,0,__PYX_ERR(2, 352, __pyx_L1_error))
       ((Py_buffer *)(&__pyx_v_self->view))->obj = Py_None;
 
-      /* "View.MemoryView":352
+      /* "View.MemoryView":353
  *             if <PyObject *> self.view.obj == NULL:
  *                 (<__pyx_buffer *> &self.view).obj = Py_None
  *                 Py_INCREF(Py_None)             # <<<<<<<<<<<<<<
  * 
- *         global __pyx_memoryview_thread_locks_used
+ *         if not __PYX_CYTHON_ATOMICS_ENABLED():
  */
-      __Pyx_TraceLine(352,0,__PYX_ERR(2, 352, __pyx_L1_error))
+      __Pyx_TraceLine(353,0,__PYX_ERR(2, 353, __pyx_L1_error))
       Py_INCREF(Py_None);
 
-      /* "View.MemoryView":350
+      /* "View.MemoryView":351
  *         if type(self) is memoryview or obj is not None:
  *             __Pyx_GetBuffer(obj, &self.view, flags)
  *             if <PyObject *> self.view.obj == NULL:             # <<<<<<<<<<<<<<
  *                 (<__pyx_buffer *> &self.view).obj = Py_None
  *                 Py_INCREF(Py_None)
  */
     }
 
-    /* "View.MemoryView":348
+    /* "View.MemoryView":349
  *         self.obj = obj
  *         self.flags = flags
  *         if type(self) is memoryview or obj is not None:             # <<<<<<<<<<<<<<
  *             __Pyx_GetBuffer(obj, &self.view, flags)
  *             if <PyObject *> self.view.obj == NULL:
  */
   }
 
   /* "View.MemoryView":355
+ *                 Py_INCREF(Py_None)
  * 
- *         global __pyx_memoryview_thread_locks_used
- *         if __pyx_memoryview_thread_locks_used < THREAD_LOCKS_PREALLOCATED:             # <<<<<<<<<<<<<<
- *             self.lock = __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]
- *             __pyx_memoryview_thread_locks_used += 1
+ *         if not __PYX_CYTHON_ATOMICS_ENABLED():             # <<<<<<<<<<<<<<
+ *             global __pyx_memoryview_thread_locks_used
+ *             if __pyx_memoryview_thread_locks_used < THREAD_LOCKS_PREALLOCATED:
  */
   __Pyx_TraceLine(355,0,__PYX_ERR(2, 355, __pyx_L1_error))
-  __pyx_t_1 = ((__pyx_memoryview_thread_locks_used < 8) != 0);
+  __pyx_t_1 = ((!(__PYX_CYTHON_ATOMICS_ENABLED() != 0)) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":356
- *         global __pyx_memoryview_thread_locks_used
- *         if __pyx_memoryview_thread_locks_used < THREAD_LOCKS_PREALLOCATED:
- *             self.lock = __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]             # <<<<<<<<<<<<<<
- *             __pyx_memoryview_thread_locks_used += 1
- *         if self.lock is NULL:
- */
-    __Pyx_TraceLine(356,0,__PYX_ERR(2, 356, __pyx_L1_error))
-    __pyx_v_self->lock = (__pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]);
-
     /* "View.MemoryView":357
- *         if __pyx_memoryview_thread_locks_used < THREAD_LOCKS_PREALLOCATED:
- *             self.lock = __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]
- *             __pyx_memoryview_thread_locks_used += 1             # <<<<<<<<<<<<<<
- *         if self.lock is NULL:
- *             self.lock = PyThread_allocate_lock()
+ *         if not __PYX_CYTHON_ATOMICS_ENABLED():
+ *             global __pyx_memoryview_thread_locks_used
+ *             if __pyx_memoryview_thread_locks_used < THREAD_LOCKS_PREALLOCATED:             # <<<<<<<<<<<<<<
+ *                 self.lock = __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]
+ *                 __pyx_memoryview_thread_locks_used += 1
  */
     __Pyx_TraceLine(357,0,__PYX_ERR(2, 357, __pyx_L1_error))
-    __pyx_memoryview_thread_locks_used = (__pyx_memoryview_thread_locks_used + 1);
+    __pyx_t_1 = ((__pyx_memoryview_thread_locks_used < 8) != 0);
+    if (__pyx_t_1) {
 
-    /* "View.MemoryView":355
- * 
- *         global __pyx_memoryview_thread_locks_used
- *         if __pyx_memoryview_thread_locks_used < THREAD_LOCKS_PREALLOCATED:             # <<<<<<<<<<<<<<
- *             self.lock = __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]
- *             __pyx_memoryview_thread_locks_used += 1
+      /* "View.MemoryView":358
+ *             global __pyx_memoryview_thread_locks_used
+ *             if __pyx_memoryview_thread_locks_used < THREAD_LOCKS_PREALLOCATED:
+ *                 self.lock = __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]             # <<<<<<<<<<<<<<
+ *                 __pyx_memoryview_thread_locks_used += 1
+ *             if self.lock is NULL:
  */
-  }
+      __Pyx_TraceLine(358,0,__PYX_ERR(2, 358, __pyx_L1_error))
+      __pyx_v_self->lock = (__pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]);
 
-  /* "View.MemoryView":358
- *             self.lock = __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]
- *             __pyx_memoryview_thread_locks_used += 1
- *         if self.lock is NULL:             # <<<<<<<<<<<<<<
- *             self.lock = PyThread_allocate_lock()
+      /* "View.MemoryView":359
+ *             if __pyx_memoryview_thread_locks_used < THREAD_LOCKS_PREALLOCATED:
+ *                 self.lock = __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]
+ *                 __pyx_memoryview_thread_locks_used += 1             # <<<<<<<<<<<<<<
  *             if self.lock is NULL:
+ *                 self.lock = PyThread_allocate_lock()
  */
-  __Pyx_TraceLine(358,0,__PYX_ERR(2, 358, __pyx_L1_error))
-  __pyx_t_1 = ((__pyx_v_self->lock == NULL) != 0);
-  if (__pyx_t_1) {
+      __Pyx_TraceLine(359,0,__PYX_ERR(2, 359, __pyx_L1_error))
+      __pyx_memoryview_thread_locks_used = (__pyx_memoryview_thread_locks_used + 1);
 
-    /* "View.MemoryView":359
- *             __pyx_memoryview_thread_locks_used += 1
- *         if self.lock is NULL:
- *             self.lock = PyThread_allocate_lock()             # <<<<<<<<<<<<<<
- *             if self.lock is NULL:
- *                 raise MemoryError
+      /* "View.MemoryView":357
+ *         if not __PYX_CYTHON_ATOMICS_ENABLED():
+ *             global __pyx_memoryview_thread_locks_used
+ *             if __pyx_memoryview_thread_locks_used < THREAD_LOCKS_PREALLOCATED:             # <<<<<<<<<<<<<<
+ *                 self.lock = __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]
+ *                 __pyx_memoryview_thread_locks_used += 1
  */
-    __Pyx_TraceLine(359,0,__PYX_ERR(2, 359, __pyx_L1_error))
-    __pyx_v_self->lock = PyThread_allocate_lock();
+    }
 
     /* "View.MemoryView":360
- *         if self.lock is NULL:
- *             self.lock = PyThread_allocate_lock()
+ *                 self.lock = __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]
+ *                 __pyx_memoryview_thread_locks_used += 1
  *             if self.lock is NULL:             # <<<<<<<<<<<<<<
- *                 raise MemoryError
- * 
+ *                 self.lock = PyThread_allocate_lock()
+ *                 if self.lock is NULL:
  */
     __Pyx_TraceLine(360,0,__PYX_ERR(2, 360, __pyx_L1_error))
     __pyx_t_1 = ((__pyx_v_self->lock == NULL) != 0);
-    if (unlikely(__pyx_t_1)) {
+    if (__pyx_t_1) {
 
       /* "View.MemoryView":361
- *             self.lock = PyThread_allocate_lock()
+ *                 __pyx_memoryview_thread_locks_used += 1
  *             if self.lock is NULL:
- *                 raise MemoryError             # <<<<<<<<<<<<<<
+ *                 self.lock = PyThread_allocate_lock()             # <<<<<<<<<<<<<<
+ *                 if self.lock is NULL:
+ *                     raise MemoryError
+ */
+      __Pyx_TraceLine(361,0,__PYX_ERR(2, 361, __pyx_L1_error))
+      __pyx_v_self->lock = PyThread_allocate_lock();
+
+      /* "View.MemoryView":362
+ *             if self.lock is NULL:
+ *                 self.lock = PyThread_allocate_lock()
+ *                 if self.lock is NULL:             # <<<<<<<<<<<<<<
+ *                     raise MemoryError
+ * 
+ */
+      __Pyx_TraceLine(362,0,__PYX_ERR(2, 362, __pyx_L1_error))
+      __pyx_t_1 = ((__pyx_v_self->lock == NULL) != 0);
+      if (unlikely(__pyx_t_1)) {
+
+        /* "View.MemoryView":363
+ *                 self.lock = PyThread_allocate_lock()
+ *                 if self.lock is NULL:
+ *                     raise MemoryError             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_FORMAT:
  */
-      __Pyx_TraceLine(361,0,__PYX_ERR(2, 361, __pyx_L1_error))
-      PyErr_NoMemory(); __PYX_ERR(2, 361, __pyx_L1_error)
+        __Pyx_TraceLine(363,0,__PYX_ERR(2, 363, __pyx_L1_error))
+        PyErr_NoMemory(); __PYX_ERR(2, 363, __pyx_L1_error)
+
+        /* "View.MemoryView":362
+ *             if self.lock is NULL:
+ *                 self.lock = PyThread_allocate_lock()
+ *                 if self.lock is NULL:             # <<<<<<<<<<<<<<
+ *                     raise MemoryError
+ * 
+ */
+      }
 
       /* "View.MemoryView":360
- *         if self.lock is NULL:
- *             self.lock = PyThread_allocate_lock()
+ *                 self.lock = __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]
+ *                 __pyx_memoryview_thread_locks_used += 1
  *             if self.lock is NULL:             # <<<<<<<<<<<<<<
- *                 raise MemoryError
- * 
+ *                 self.lock = PyThread_allocate_lock()
+ *                 if self.lock is NULL:
  */
     }
 
-    /* "View.MemoryView":358
- *             self.lock = __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]
- *             __pyx_memoryview_thread_locks_used += 1
- *         if self.lock is NULL:             # <<<<<<<<<<<<<<
- *             self.lock = PyThread_allocate_lock()
- *             if self.lock is NULL:
+    /* "View.MemoryView":355
+ *                 Py_INCREF(Py_None)
+ * 
+ *         if not __PYX_CYTHON_ATOMICS_ENABLED():             # <<<<<<<<<<<<<<
+ *             global __pyx_memoryview_thread_locks_used
+ *             if __pyx_memoryview_thread_locks_used < THREAD_LOCKS_PREALLOCATED:
  */
   }
 
-  /* "View.MemoryView":363
- *                 raise MemoryError
+  /* "View.MemoryView":365
+ *                     raise MemoryError
  * 
  *         if flags & PyBUF_FORMAT:             # <<<<<<<<<<<<<<
  *             self.dtype_is_object = (self.view.format[0] == b'O' and self.view.format[1] == b'\0')
  *         else:
  */
-  __Pyx_TraceLine(363,0,__PYX_ERR(2, 363, __pyx_L1_error))
+  __Pyx_TraceLine(365,0,__PYX_ERR(2, 365, __pyx_L1_error))
   __pyx_t_1 = ((__pyx_v_flags & PyBUF_FORMAT) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":364
+    /* "View.MemoryView":366
  * 
  *         if flags & PyBUF_FORMAT:
  *             self.dtype_is_object = (self.view.format[0] == b'O' and self.view.format[1] == b'\0')             # <<<<<<<<<<<<<<
  *         else:
  *             self.dtype_is_object = dtype_is_object
  */
-    __Pyx_TraceLine(364,0,__PYX_ERR(2, 364, __pyx_L1_error))
+    __Pyx_TraceLine(366,0,__PYX_ERR(2, 366, __pyx_L1_error))
     __pyx_t_2 = (((__pyx_v_self->view.format[0]) == 'O') != 0);
     if (__pyx_t_2) {
     } else {
       __pyx_t_1 = __pyx_t_2;
-      goto __pyx_L11_bool_binop_done;
+      goto __pyx_L12_bool_binop_done;
     }
     __pyx_t_2 = (((__pyx_v_self->view.format[1]) == '\x00') != 0);
     __pyx_t_1 = __pyx_t_2;
-    __pyx_L11_bool_binop_done:;
+    __pyx_L12_bool_binop_done:;
     __pyx_v_self->dtype_is_object = __pyx_t_1;
 
-    /* "View.MemoryView":363
- *                 raise MemoryError
+    /* "View.MemoryView":365
+ *                     raise MemoryError
  * 
  *         if flags & PyBUF_FORMAT:             # <<<<<<<<<<<<<<
  *             self.dtype_is_object = (self.view.format[0] == b'O' and self.view.format[1] == b'\0')
  *         else:
  */
-    goto __pyx_L10;
+    goto __pyx_L11;
   }
 
-  /* "View.MemoryView":366
+  /* "View.MemoryView":368
  *             self.dtype_is_object = (self.view.format[0] == b'O' and self.view.format[1] == b'\0')
  *         else:
  *             self.dtype_is_object = dtype_is_object             # <<<<<<<<<<<<<<
  * 
  *         self.acquisition_count_aligned_p = <__pyx_atomic_int *> align_pointer(
  */
-  __Pyx_TraceLine(366,0,__PYX_ERR(2, 366, __pyx_L1_error))
+  __Pyx_TraceLine(368,0,__PYX_ERR(2, 368, __pyx_L1_error))
   /*else*/ {
     __pyx_v_self->dtype_is_object = __pyx_v_dtype_is_object;
   }
-  __pyx_L10:;
+  __pyx_L11:;
 
-  /* "View.MemoryView":368
+  /* "View.MemoryView":370
  *             self.dtype_is_object = dtype_is_object
  * 
  *         self.acquisition_count_aligned_p = <__pyx_atomic_int *> align_pointer(             # <<<<<<<<<<<<<<
  *                   <void *> &self.acquisition_count[0], sizeof(__pyx_atomic_int))
  *         self.typeinfo = NULL
  */
-  __Pyx_TraceLine(368,0,__PYX_ERR(2, 368, __pyx_L1_error))
+  __Pyx_TraceLine(370,0,__PYX_ERR(2, 370, __pyx_L1_error))
   __pyx_v_self->acquisition_count_aligned_p = ((__pyx_atomic_int *)__pyx_align_pointer(((void *)(&(__pyx_v_self->acquisition_count[0]))), (sizeof(__pyx_atomic_int))));
 
-  /* "View.MemoryView":370
+  /* "View.MemoryView":372
  *         self.acquisition_count_aligned_p = <__pyx_atomic_int *> align_pointer(
  *                   <void *> &self.acquisition_count[0], sizeof(__pyx_atomic_int))
  *         self.typeinfo = NULL             # <<<<<<<<<<<<<<
  * 
  *     def __dealloc__(memoryview self):
  */
-  __Pyx_TraceLine(370,0,__PYX_ERR(2, 370, __pyx_L1_error))
+  __Pyx_TraceLine(372,0,__PYX_ERR(2, 372, __pyx_L1_error))
   __pyx_v_self->typeinfo = NULL;
 
-  /* "View.MemoryView":345
+  /* "View.MemoryView":346
  *     cdef __Pyx_TypeInfo *typeinfo
  * 
  *     def __cinit__(memoryview self, object obj, int flags, bint dtype_is_object=False):             # <<<<<<<<<<<<<<
  *         self.obj = obj
  *         self.flags = flags
  */
 
@@ -19419,15 +19613,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":372
+/* "View.MemoryView":374
  *         self.typeinfo = NULL
  * 
  *     def __dealloc__(memoryview self):             # <<<<<<<<<<<<<<
  *         if self.obj is not None:
  *             __Pyx_ReleaseBuffer(&self.view)
  */
 
@@ -19453,219 +19647,219 @@
   int __pyx_t_5;
   PyThread_type_lock __pyx_t_6;
   PyThread_type_lock __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__dealloc__", 0);
-  __Pyx_TraceCall("__dealloc__", __pyx_f[2], 372, 0, __PYX_ERR(2, 372, __pyx_L1_error));
+  __Pyx_TraceCall("__dealloc__", __pyx_f[2], 374, 0, __PYX_ERR(2, 374, __pyx_L1_error));
 
-  /* "View.MemoryView":373
+  /* "View.MemoryView":375
  * 
  *     def __dealloc__(memoryview self):
  *         if self.obj is not None:             # <<<<<<<<<<<<<<
  *             __Pyx_ReleaseBuffer(&self.view)
  *         elif (<__pyx_buffer *> &self.view).obj == Py_None:
  */
-  __Pyx_TraceLine(373,0,__PYX_ERR(2, 373, __pyx_L1_error))
+  __Pyx_TraceLine(375,0,__PYX_ERR(2, 375, __pyx_L1_error))
   __pyx_t_1 = (__pyx_v_self->obj != Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":374
+    /* "View.MemoryView":376
  *     def __dealloc__(memoryview self):
  *         if self.obj is not None:
  *             __Pyx_ReleaseBuffer(&self.view)             # <<<<<<<<<<<<<<
  *         elif (<__pyx_buffer *> &self.view).obj == Py_None:
  * 
  */
-    __Pyx_TraceLine(374,0,__PYX_ERR(2, 374, __pyx_L1_error))
+    __Pyx_TraceLine(376,0,__PYX_ERR(2, 376, __pyx_L1_error))
     __Pyx_ReleaseBuffer((&__pyx_v_self->view));
 
-    /* "View.MemoryView":373
+    /* "View.MemoryView":375
  * 
  *     def __dealloc__(memoryview self):
  *         if self.obj is not None:             # <<<<<<<<<<<<<<
  *             __Pyx_ReleaseBuffer(&self.view)
  *         elif (<__pyx_buffer *> &self.view).obj == Py_None:
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":375
+  /* "View.MemoryView":377
  *         if self.obj is not None:
  *             __Pyx_ReleaseBuffer(&self.view)
  *         elif (<__pyx_buffer *> &self.view).obj == Py_None:             # <<<<<<<<<<<<<<
  * 
  *             (<__pyx_buffer *> &self.view).obj = NULL
  */
-  __Pyx_TraceLine(375,0,__PYX_ERR(2, 375, __pyx_L1_error))
+  __Pyx_TraceLine(377,0,__PYX_ERR(2, 377, __pyx_L1_error))
   __pyx_t_2 = ((((Py_buffer *)(&__pyx_v_self->view))->obj == Py_None) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":377
+    /* "View.MemoryView":379
  *         elif (<__pyx_buffer *> &self.view).obj == Py_None:
  * 
  *             (<__pyx_buffer *> &self.view).obj = NULL             # <<<<<<<<<<<<<<
  *             Py_DECREF(Py_None)
  * 
  */
-    __Pyx_TraceLine(377,0,__PYX_ERR(2, 377, __pyx_L1_error))
+    __Pyx_TraceLine(379,0,__PYX_ERR(2, 379, __pyx_L1_error))
     ((Py_buffer *)(&__pyx_v_self->view))->obj = NULL;
 
-    /* "View.MemoryView":378
+    /* "View.MemoryView":380
  * 
  *             (<__pyx_buffer *> &self.view).obj = NULL
  *             Py_DECREF(Py_None)             # <<<<<<<<<<<<<<
  * 
  *         cdef int i
  */
-    __Pyx_TraceLine(378,0,__PYX_ERR(2, 378, __pyx_L1_error))
+    __Pyx_TraceLine(380,0,__PYX_ERR(2, 380, __pyx_L1_error))
     Py_DECREF(Py_None);
 
-    /* "View.MemoryView":375
+    /* "View.MemoryView":377
  *         if self.obj is not None:
  *             __Pyx_ReleaseBuffer(&self.view)
  *         elif (<__pyx_buffer *> &self.view).obj == Py_None:             # <<<<<<<<<<<<<<
  * 
  *             (<__pyx_buffer *> &self.view).obj = NULL
  */
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":382
+  /* "View.MemoryView":384
  *         cdef int i
  *         global __pyx_memoryview_thread_locks_used
  *         if self.lock != NULL:             # <<<<<<<<<<<<<<
  *             for i in range(__pyx_memoryview_thread_locks_used):
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:
  */
-  __Pyx_TraceLine(382,0,__PYX_ERR(2, 382, __pyx_L1_error))
+  __Pyx_TraceLine(384,0,__PYX_ERR(2, 384, __pyx_L1_error))
   __pyx_t_2 = ((__pyx_v_self->lock != NULL) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":383
+    /* "View.MemoryView":385
  *         global __pyx_memoryview_thread_locks_used
  *         if self.lock != NULL:
  *             for i in range(__pyx_memoryview_thread_locks_used):             # <<<<<<<<<<<<<<
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:
  *                     __pyx_memoryview_thread_locks_used -= 1
  */
-    __Pyx_TraceLine(383,0,__PYX_ERR(2, 383, __pyx_L1_error))
+    __Pyx_TraceLine(385,0,__PYX_ERR(2, 385, __pyx_L1_error))
     __pyx_t_3 = __pyx_memoryview_thread_locks_used;
     __pyx_t_4 = __pyx_t_3;
     for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_4; __pyx_t_5+=1) {
       __pyx_v_i = __pyx_t_5;
 
-      /* "View.MemoryView":384
+      /* "View.MemoryView":386
  *         if self.lock != NULL:
  *             for i in range(__pyx_memoryview_thread_locks_used):
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:             # <<<<<<<<<<<<<<
  *                     __pyx_memoryview_thread_locks_used -= 1
  *                     if i != __pyx_memoryview_thread_locks_used:
  */
-      __Pyx_TraceLine(384,0,__PYX_ERR(2, 384, __pyx_L1_error))
+      __Pyx_TraceLine(386,0,__PYX_ERR(2, 386, __pyx_L1_error))
       __pyx_t_2 = (((__pyx_memoryview_thread_locks[__pyx_v_i]) == __pyx_v_self->lock) != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":385
+        /* "View.MemoryView":387
  *             for i in range(__pyx_memoryview_thread_locks_used):
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:
  *                     __pyx_memoryview_thread_locks_used -= 1             # <<<<<<<<<<<<<<
  *                     if i != __pyx_memoryview_thread_locks_used:
  *                         __pyx_memoryview_thread_locks[i], __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used] = (
  */
-        __Pyx_TraceLine(385,0,__PYX_ERR(2, 385, __pyx_L1_error))
+        __Pyx_TraceLine(387,0,__PYX_ERR(2, 387, __pyx_L1_error))
         __pyx_memoryview_thread_locks_used = (__pyx_memoryview_thread_locks_used - 1);
 
-        /* "View.MemoryView":386
+        /* "View.MemoryView":388
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:
  *                     __pyx_memoryview_thread_locks_used -= 1
  *                     if i != __pyx_memoryview_thread_locks_used:             # <<<<<<<<<<<<<<
  *                         __pyx_memoryview_thread_locks[i], __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used] = (
  *                             __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used], __pyx_memoryview_thread_locks[i])
  */
-        __Pyx_TraceLine(386,0,__PYX_ERR(2, 386, __pyx_L1_error))
+        __Pyx_TraceLine(388,0,__PYX_ERR(2, 388, __pyx_L1_error))
         __pyx_t_2 = ((__pyx_v_i != __pyx_memoryview_thread_locks_used) != 0);
         if (__pyx_t_2) {
 
-          /* "View.MemoryView":388
+          /* "View.MemoryView":390
  *                     if i != __pyx_memoryview_thread_locks_used:
  *                         __pyx_memoryview_thread_locks[i], __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used] = (
  *                             __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used], __pyx_memoryview_thread_locks[i])             # <<<<<<<<<<<<<<
  *                     break
  *             else:
  */
-          __Pyx_TraceLine(388,0,__PYX_ERR(2, 388, __pyx_L1_error))
+          __Pyx_TraceLine(390,0,__PYX_ERR(2, 390, __pyx_L1_error))
           __pyx_t_6 = (__pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]);
           __pyx_t_7 = (__pyx_memoryview_thread_locks[__pyx_v_i]);
 
-          /* "View.MemoryView":387
+          /* "View.MemoryView":389
  *                     __pyx_memoryview_thread_locks_used -= 1
  *                     if i != __pyx_memoryview_thread_locks_used:
  *                         __pyx_memoryview_thread_locks[i], __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used] = (             # <<<<<<<<<<<<<<
  *                             __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used], __pyx_memoryview_thread_locks[i])
  *                     break
  */
-          __Pyx_TraceLine(387,0,__PYX_ERR(2, 387, __pyx_L1_error))
+          __Pyx_TraceLine(389,0,__PYX_ERR(2, 389, __pyx_L1_error))
           (__pyx_memoryview_thread_locks[__pyx_v_i]) = __pyx_t_6;
           (__pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]) = __pyx_t_7;
 
-          /* "View.MemoryView":386
+          /* "View.MemoryView":388
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:
  *                     __pyx_memoryview_thread_locks_used -= 1
  *                     if i != __pyx_memoryview_thread_locks_used:             # <<<<<<<<<<<<<<
  *                         __pyx_memoryview_thread_locks[i], __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used] = (
  *                             __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used], __pyx_memoryview_thread_locks[i])
  */
         }
 
-        /* "View.MemoryView":389
+        /* "View.MemoryView":391
  *                         __pyx_memoryview_thread_locks[i], __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used] = (
  *                             __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used], __pyx_memoryview_thread_locks[i])
  *                     break             # <<<<<<<<<<<<<<
  *             else:
  *                 PyThread_free_lock(self.lock)
  */
-        __Pyx_TraceLine(389,0,__PYX_ERR(2, 389, __pyx_L1_error))
+        __Pyx_TraceLine(391,0,__PYX_ERR(2, 391, __pyx_L1_error))
         goto __pyx_L6_break;
 
-        /* "View.MemoryView":384
+        /* "View.MemoryView":386
  *         if self.lock != NULL:
  *             for i in range(__pyx_memoryview_thread_locks_used):
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:             # <<<<<<<<<<<<<<
  *                     __pyx_memoryview_thread_locks_used -= 1
  *                     if i != __pyx_memoryview_thread_locks_used:
  */
       }
     }
     /*else*/ {
 
-      /* "View.MemoryView":391
+      /* "View.MemoryView":393
  *                     break
  *             else:
  *                 PyThread_free_lock(self.lock)             # <<<<<<<<<<<<<<
  * 
  *     cdef char *get_item_pointer(memoryview self, object index) except NULL:
  */
-      __Pyx_TraceLine(391,0,__PYX_ERR(2, 391, __pyx_L1_error))
+      __Pyx_TraceLine(393,0,__PYX_ERR(2, 393, __pyx_L1_error))
       PyThread_free_lock(__pyx_v_self->lock);
     }
     __pyx_L6_break:;
 
-    /* "View.MemoryView":382
+    /* "View.MemoryView":384
  *         cdef int i
  *         global __pyx_memoryview_thread_locks_used
  *         if self.lock != NULL:             # <<<<<<<<<<<<<<
  *             for i in range(__pyx_memoryview_thread_locks_used):
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:
  */
   }
 
-  /* "View.MemoryView":372
+  /* "View.MemoryView":374
  *         self.typeinfo = NULL
  * 
  *     def __dealloc__(memoryview self):             # <<<<<<<<<<<<<<
  *         if self.obj is not None:
  *             __Pyx_ReleaseBuffer(&self.view)
  */
 
@@ -19674,15 +19868,15 @@
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("View.MemoryView.memoryview.__dealloc__", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
 }
 
-/* "View.MemoryView":393
+/* "View.MemoryView":395
  *                 PyThread_free_lock(self.lock)
  * 
  *     cdef char *get_item_pointer(memoryview self, object index) except NULL:             # <<<<<<<<<<<<<<
  *         cdef Py_ssize_t dim
  *         cdef char *itemp = <char *> self.view.buf
  */
 
@@ -19700,114 +19894,114 @@
   PyObject *__pyx_t_5 = NULL;
   Py_ssize_t __pyx_t_6;
   char *__pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_item_pointer", 0);
-  __Pyx_TraceCall("get_item_pointer", __pyx_f[2], 393, 0, __PYX_ERR(2, 393, __pyx_L1_error));
+  __Pyx_TraceCall("get_item_pointer", __pyx_f[2], 395, 0, __PYX_ERR(2, 395, __pyx_L1_error));
 
-  /* "View.MemoryView":395
+  /* "View.MemoryView":397
  *     cdef char *get_item_pointer(memoryview self, object index) except NULL:
  *         cdef Py_ssize_t dim
  *         cdef char *itemp = <char *> self.view.buf             # <<<<<<<<<<<<<<
  * 
  *         for dim, idx in enumerate(index):
  */
-  __Pyx_TraceLine(395,0,__PYX_ERR(2, 395, __pyx_L1_error))
+  __Pyx_TraceLine(397,0,__PYX_ERR(2, 397, __pyx_L1_error))
   __pyx_v_itemp = ((char *)__pyx_v_self->view.buf);
 
-  /* "View.MemoryView":397
+  /* "View.MemoryView":399
  *         cdef char *itemp = <char *> self.view.buf
  * 
  *         for dim, idx in enumerate(index):             # <<<<<<<<<<<<<<
  *             itemp = pybuffer_index(&self.view, itemp, idx, dim)
  * 
  */
-  __Pyx_TraceLine(397,0,__PYX_ERR(2, 397, __pyx_L1_error))
+  __Pyx_TraceLine(399,0,__PYX_ERR(2, 399, __pyx_L1_error))
   __pyx_t_1 = 0;
   if (likely(PyList_CheckExact(__pyx_v_index)) || PyTuple_CheckExact(__pyx_v_index)) {
     __pyx_t_2 = __pyx_v_index; __Pyx_INCREF(__pyx_t_2); __pyx_t_3 = 0;
     __pyx_t_4 = NULL;
   } else {
-    __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 397, __pyx_L1_error)
+    __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 399, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 397, __pyx_L1_error)
+    __pyx_t_4 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 399, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_4)) {
       if (likely(PyList_CheckExact(__pyx_t_2))) {
         if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(2, 397, __pyx_L1_error)
+        __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(2, 399, __pyx_L1_error)
         #else
-        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 397, __pyx_L1_error)
+        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 399, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         #endif
       } else {
         if (__pyx_t_3 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(2, 397, __pyx_L1_error)
+        __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(2, 399, __pyx_L1_error)
         #else
-        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 397, __pyx_L1_error)
+        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 399, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         #endif
       }
     } else {
       __pyx_t_5 = __pyx_t_4(__pyx_t_2);
       if (unlikely(!__pyx_t_5)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(2, 397, __pyx_L1_error)
+          else __PYX_ERR(2, 399, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_5);
     }
     __Pyx_XDECREF_SET(__pyx_v_idx, __pyx_t_5);
     __pyx_t_5 = 0;
     __pyx_v_dim = __pyx_t_1;
     __pyx_t_1 = (__pyx_t_1 + 1);
 
-    /* "View.MemoryView":398
+    /* "View.MemoryView":400
  * 
  *         for dim, idx in enumerate(index):
  *             itemp = pybuffer_index(&self.view, itemp, idx, dim)             # <<<<<<<<<<<<<<
  * 
  *         return itemp
  */
-    __Pyx_TraceLine(398,0,__PYX_ERR(2, 398, __pyx_L1_error))
-    __pyx_t_6 = __Pyx_PyIndex_AsSsize_t(__pyx_v_idx); if (unlikely((__pyx_t_6 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(2, 398, __pyx_L1_error)
-    __pyx_t_7 = __pyx_pybuffer_index((&__pyx_v_self->view), __pyx_v_itemp, __pyx_t_6, __pyx_v_dim); if (unlikely(__pyx_t_7 == ((char *)NULL))) __PYX_ERR(2, 398, __pyx_L1_error)
+    __Pyx_TraceLine(400,0,__PYX_ERR(2, 400, __pyx_L1_error))
+    __pyx_t_6 = __Pyx_PyIndex_AsSsize_t(__pyx_v_idx); if (unlikely((__pyx_t_6 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(2, 400, __pyx_L1_error)
+    __pyx_t_7 = __pyx_pybuffer_index((&__pyx_v_self->view), __pyx_v_itemp, __pyx_t_6, __pyx_v_dim); if (unlikely(__pyx_t_7 == ((char *)NULL))) __PYX_ERR(2, 400, __pyx_L1_error)
     __pyx_v_itemp = __pyx_t_7;
 
-    /* "View.MemoryView":397
+    /* "View.MemoryView":399
  *         cdef char *itemp = <char *> self.view.buf
  * 
  *         for dim, idx in enumerate(index):             # <<<<<<<<<<<<<<
  *             itemp = pybuffer_index(&self.view, itemp, idx, dim)
  * 
  */
-    __Pyx_TraceLine(397,0,__PYX_ERR(2, 397, __pyx_L1_error))
+    __Pyx_TraceLine(399,0,__PYX_ERR(2, 399, __pyx_L1_error))
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "View.MemoryView":400
+  /* "View.MemoryView":402
  *             itemp = pybuffer_index(&self.view, itemp, idx, dim)
  * 
  *         return itemp             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_TraceLine(400,0,__PYX_ERR(2, 400, __pyx_L1_error))
+  __Pyx_TraceLine(402,0,__PYX_ERR(2, 402, __pyx_L1_error))
   __pyx_r = __pyx_v_itemp;
   goto __pyx_L0;
 
-  /* "View.MemoryView":393
+  /* "View.MemoryView":395
  *                 PyThread_free_lock(self.lock)
  * 
  *     cdef char *get_item_pointer(memoryview self, object index) except NULL:             # <<<<<<<<<<<<<<
  *         cdef Py_ssize_t dim
  *         cdef char *itemp = <char *> self.view.buf
  */
 
@@ -19820,15 +20014,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_idx);
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":403
+/* "View.MemoryView":405
  * 
  * 
  *     def __getitem__(memoryview self, object index):             # <<<<<<<<<<<<<<
  *         if index is Ellipsis:
  *             return self
  */
 
@@ -19858,152 +20052,152 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   char *__pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__getitem__", 0);
-  __Pyx_TraceCall("__getitem__", __pyx_f[2], 403, 0, __PYX_ERR(2, 403, __pyx_L1_error));
+  __Pyx_TraceCall("__getitem__", __pyx_f[2], 405, 0, __PYX_ERR(2, 405, __pyx_L1_error));
 
-  /* "View.MemoryView":404
+  /* "View.MemoryView":406
  * 
  *     def __getitem__(memoryview self, object index):
  *         if index is Ellipsis:             # <<<<<<<<<<<<<<
  *             return self
  * 
  */
-  __Pyx_TraceLine(404,0,__PYX_ERR(2, 404, __pyx_L1_error))
+  __Pyx_TraceLine(406,0,__PYX_ERR(2, 406, __pyx_L1_error))
   __pyx_t_1 = (__pyx_v_index == __pyx_builtin_Ellipsis);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":405
+    /* "View.MemoryView":407
  *     def __getitem__(memoryview self, object index):
  *         if index is Ellipsis:
  *             return self             # <<<<<<<<<<<<<<
  * 
  *         have_slices, indices = _unellipsify(index, self.view.ndim)
  */
-    __Pyx_TraceLine(405,0,__PYX_ERR(2, 405, __pyx_L1_error))
+    __Pyx_TraceLine(407,0,__PYX_ERR(2, 407, __pyx_L1_error))
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject *)__pyx_v_self));
     __pyx_r = ((PyObject *)__pyx_v_self);
     goto __pyx_L0;
 
-    /* "View.MemoryView":404
+    /* "View.MemoryView":406
  * 
  *     def __getitem__(memoryview self, object index):
  *         if index is Ellipsis:             # <<<<<<<<<<<<<<
  *             return self
  * 
  */
   }
 
-  /* "View.MemoryView":407
+  /* "View.MemoryView":409
  *             return self
  * 
  *         have_slices, indices = _unellipsify(index, self.view.ndim)             # <<<<<<<<<<<<<<
  * 
  *         cdef char *itemp
  */
-  __Pyx_TraceLine(407,0,__PYX_ERR(2, 407, __pyx_L1_error))
-  __pyx_t_3 = _unellipsify(__pyx_v_index, __pyx_v_self->view.ndim); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 407, __pyx_L1_error)
+  __Pyx_TraceLine(409,0,__PYX_ERR(2, 409, __pyx_L1_error))
+  __pyx_t_3 = _unellipsify(__pyx_v_index, __pyx_v_self->view.ndim); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 409, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (likely(__pyx_t_3 != Py_None)) {
     PyObject* sequence = __pyx_t_3;
     Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
     if (unlikely(size != 2)) {
       if (size > 2) __Pyx_RaiseTooManyValuesError(2);
       else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-      __PYX_ERR(2, 407, __pyx_L1_error)
+      __PYX_ERR(2, 409, __pyx_L1_error)
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     __pyx_t_4 = PyTuple_GET_ITEM(sequence, 0); 
     __pyx_t_5 = PyTuple_GET_ITEM(sequence, 1); 
     __Pyx_INCREF(__pyx_t_4);
     __Pyx_INCREF(__pyx_t_5);
     #else
-    __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 407, __pyx_L1_error)
+    __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 409, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 407, __pyx_L1_error)
+    __pyx_t_5 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 409, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     #endif
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else {
-    __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(2, 407, __pyx_L1_error)
+    __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(2, 409, __pyx_L1_error)
   }
   __pyx_v_have_slices = __pyx_t_4;
   __pyx_t_4 = 0;
   __pyx_v_indices = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "View.MemoryView":410
+  /* "View.MemoryView":412
  * 
  *         cdef char *itemp
  *         if have_slices:             # <<<<<<<<<<<<<<
  *             return memview_slice(self, indices)
  *         else:
  */
-  __Pyx_TraceLine(410,0,__PYX_ERR(2, 410, __pyx_L1_error))
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_have_slices); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(2, 410, __pyx_L1_error)
+  __Pyx_TraceLine(412,0,__PYX_ERR(2, 412, __pyx_L1_error))
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_have_slices); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(2, 412, __pyx_L1_error)
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":411
+    /* "View.MemoryView":413
  *         cdef char *itemp
  *         if have_slices:
  *             return memview_slice(self, indices)             # <<<<<<<<<<<<<<
  *         else:
  *             itemp = self.get_item_pointer(indices)
  */
-    __Pyx_TraceLine(411,0,__PYX_ERR(2, 411, __pyx_L1_error))
+    __Pyx_TraceLine(413,0,__PYX_ERR(2, 413, __pyx_L1_error))
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = ((PyObject *)__pyx_memview_slice(__pyx_v_self, __pyx_v_indices)); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 411, __pyx_L1_error)
+    __pyx_t_3 = ((PyObject *)__pyx_memview_slice(__pyx_v_self, __pyx_v_indices)); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 413, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "View.MemoryView":410
+    /* "View.MemoryView":412
  * 
  *         cdef char *itemp
  *         if have_slices:             # <<<<<<<<<<<<<<
  *             return memview_slice(self, indices)
  *         else:
  */
   }
 
-  /* "View.MemoryView":413
+  /* "View.MemoryView":415
  *             return memview_slice(self, indices)
  *         else:
  *             itemp = self.get_item_pointer(indices)             # <<<<<<<<<<<<<<
  *             return self.convert_item_to_object(itemp)
  * 
  */
-  __Pyx_TraceLine(413,0,__PYX_ERR(2, 413, __pyx_L1_error))
+  __Pyx_TraceLine(415,0,__PYX_ERR(2, 415, __pyx_L1_error))
   /*else*/ {
-    __pyx_t_6 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->get_item_pointer(__pyx_v_self, __pyx_v_indices); if (unlikely(__pyx_t_6 == ((char *)NULL))) __PYX_ERR(2, 413, __pyx_L1_error)
+    __pyx_t_6 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->get_item_pointer(__pyx_v_self, __pyx_v_indices); if (unlikely(__pyx_t_6 == ((char *)NULL))) __PYX_ERR(2, 415, __pyx_L1_error)
     __pyx_v_itemp = __pyx_t_6;
 
-    /* "View.MemoryView":414
+    /* "View.MemoryView":416
  *         else:
  *             itemp = self.get_item_pointer(indices)
  *             return self.convert_item_to_object(itemp)             # <<<<<<<<<<<<<<
  * 
  *     def __setitem__(memoryview self, object index, object value):
  */
-    __Pyx_TraceLine(414,0,__PYX_ERR(2, 414, __pyx_L1_error))
+    __Pyx_TraceLine(416,0,__PYX_ERR(2, 416, __pyx_L1_error))
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->convert_item_to_object(__pyx_v_self, __pyx_v_itemp); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 414, __pyx_L1_error)
+    __pyx_t_3 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->convert_item_to_object(__pyx_v_self, __pyx_v_itemp); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 416, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
   }
 
-  /* "View.MemoryView":403
+  /* "View.MemoryView":405
  * 
  * 
  *     def __getitem__(memoryview self, object index):             # <<<<<<<<<<<<<<
  *         if index is Ellipsis:
  *             return self
  */
 
@@ -20019,15 +20213,15 @@
   __Pyx_XDECREF(__pyx_v_indices);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":416
+/* "View.MemoryView":418
  *             return self.convert_item_to_object(itemp)
  * 
  *     def __setitem__(memoryview self, object index, object value):             # <<<<<<<<<<<<<<
  *         if self.view.readonly:
  *             raise TypeError("Cannot assign to read-only memoryview")
  */
 
@@ -20054,194 +20248,194 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setitem__", 0);
-  __Pyx_TraceCall("__setitem__", __pyx_f[2], 416, 0, __PYX_ERR(2, 416, __pyx_L1_error));
+  __Pyx_TraceCall("__setitem__", __pyx_f[2], 418, 0, __PYX_ERR(2, 418, __pyx_L1_error));
   __Pyx_INCREF(__pyx_v_index);
 
-  /* "View.MemoryView":417
+  /* "View.MemoryView":419
  * 
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:             # <<<<<<<<<<<<<<
  *             raise TypeError("Cannot assign to read-only memoryview")
  * 
  */
-  __Pyx_TraceLine(417,0,__PYX_ERR(2, 417, __pyx_L1_error))
+  __Pyx_TraceLine(419,0,__PYX_ERR(2, 419, __pyx_L1_error))
   __pyx_t_1 = (__pyx_v_self->view.readonly != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "View.MemoryView":418
+    /* "View.MemoryView":420
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:
  *             raise TypeError("Cannot assign to read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         have_slices, index = _unellipsify(index, self.view.ndim)
  */
-    __Pyx_TraceLine(418,0,__PYX_ERR(2, 418, __pyx_L1_error))
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__18, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 418, __pyx_L1_error)
+    __Pyx_TraceLine(420,0,__PYX_ERR(2, 420, __pyx_L1_error))
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__19, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 420, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(2, 418, __pyx_L1_error)
+    __PYX_ERR(2, 420, __pyx_L1_error)
 
-    /* "View.MemoryView":417
+    /* "View.MemoryView":419
  * 
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:             # <<<<<<<<<<<<<<
  *             raise TypeError("Cannot assign to read-only memoryview")
  * 
  */
   }
 
-  /* "View.MemoryView":420
+  /* "View.MemoryView":422
  *             raise TypeError("Cannot assign to read-only memoryview")
  * 
  *         have_slices, index = _unellipsify(index, self.view.ndim)             # <<<<<<<<<<<<<<
  * 
  *         if have_slices:
  */
-  __Pyx_TraceLine(420,0,__PYX_ERR(2, 420, __pyx_L1_error))
-  __pyx_t_2 = _unellipsify(__pyx_v_index, __pyx_v_self->view.ndim); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 420, __pyx_L1_error)
+  __Pyx_TraceLine(422,0,__PYX_ERR(2, 422, __pyx_L1_error))
+  __pyx_t_2 = _unellipsify(__pyx_v_index, __pyx_v_self->view.ndim); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 422, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (likely(__pyx_t_2 != Py_None)) {
     PyObject* sequence = __pyx_t_2;
     Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
     if (unlikely(size != 2)) {
       if (size > 2) __Pyx_RaiseTooManyValuesError(2);
       else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-      __PYX_ERR(2, 420, __pyx_L1_error)
+      __PYX_ERR(2, 422, __pyx_L1_error)
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     __pyx_t_3 = PyTuple_GET_ITEM(sequence, 0); 
     __pyx_t_4 = PyTuple_GET_ITEM(sequence, 1); 
     __Pyx_INCREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_t_4);
     #else
-    __pyx_t_3 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 420, __pyx_L1_error)
+    __pyx_t_3 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 422, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 420, __pyx_L1_error)
+    __pyx_t_4 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 422, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     #endif
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   } else {
-    __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(2, 420, __pyx_L1_error)
+    __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(2, 422, __pyx_L1_error)
   }
   __pyx_v_have_slices = __pyx_t_3;
   __pyx_t_3 = 0;
   __Pyx_DECREF_SET(__pyx_v_index, __pyx_t_4);
   __pyx_t_4 = 0;
 
-  /* "View.MemoryView":422
+  /* "View.MemoryView":424
  *         have_slices, index = _unellipsify(index, self.view.ndim)
  * 
  *         if have_slices:             # <<<<<<<<<<<<<<
  *             obj = self.is_slice(value)
  *             if obj:
  */
-  __Pyx_TraceLine(422,0,__PYX_ERR(2, 422, __pyx_L1_error))
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_have_slices); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(2, 422, __pyx_L1_error)
+  __Pyx_TraceLine(424,0,__PYX_ERR(2, 424, __pyx_L1_error))
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_have_slices); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(2, 424, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":423
+    /* "View.MemoryView":425
  * 
  *         if have_slices:
  *             obj = self.is_slice(value)             # <<<<<<<<<<<<<<
  *             if obj:
  *                 self.setitem_slice_assignment(self[index], obj)
  */
-    __Pyx_TraceLine(423,0,__PYX_ERR(2, 423, __pyx_L1_error))
-    __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->is_slice(__pyx_v_self, __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 423, __pyx_L1_error)
+    __Pyx_TraceLine(425,0,__PYX_ERR(2, 425, __pyx_L1_error))
+    __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->is_slice(__pyx_v_self, __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 425, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_v_obj = __pyx_t_2;
     __pyx_t_2 = 0;
 
-    /* "View.MemoryView":424
+    /* "View.MemoryView":426
  *         if have_slices:
  *             obj = self.is_slice(value)
  *             if obj:             # <<<<<<<<<<<<<<
  *                 self.setitem_slice_assignment(self[index], obj)
  *             else:
  */
-    __Pyx_TraceLine(424,0,__PYX_ERR(2, 424, __pyx_L1_error))
-    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_obj); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(2, 424, __pyx_L1_error)
+    __Pyx_TraceLine(426,0,__PYX_ERR(2, 426, __pyx_L1_error))
+    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_obj); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(2, 426, __pyx_L1_error)
     if (__pyx_t_1) {
 
-      /* "View.MemoryView":425
+      /* "View.MemoryView":427
  *             obj = self.is_slice(value)
  *             if obj:
  *                 self.setitem_slice_assignment(self[index], obj)             # <<<<<<<<<<<<<<
  *             else:
  *                 self.setitem_slice_assign_scalar(self[index], value)
  */
-      __Pyx_TraceLine(425,0,__PYX_ERR(2, 425, __pyx_L1_error))
-      __pyx_t_2 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_v_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 425, __pyx_L1_error)
+      __Pyx_TraceLine(427,0,__PYX_ERR(2, 427, __pyx_L1_error))
+      __pyx_t_2 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_v_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 427, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_4 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->setitem_slice_assignment(__pyx_v_self, __pyx_t_2, __pyx_v_obj); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 425, __pyx_L1_error)
+      __pyx_t_4 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->setitem_slice_assignment(__pyx_v_self, __pyx_t_2, __pyx_v_obj); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 427, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-      /* "View.MemoryView":424
+      /* "View.MemoryView":426
  *         if have_slices:
  *             obj = self.is_slice(value)
  *             if obj:             # <<<<<<<<<<<<<<
  *                 self.setitem_slice_assignment(self[index], obj)
  *             else:
  */
       goto __pyx_L5;
     }
 
-    /* "View.MemoryView":427
+    /* "View.MemoryView":429
  *                 self.setitem_slice_assignment(self[index], obj)
  *             else:
  *                 self.setitem_slice_assign_scalar(self[index], value)             # <<<<<<<<<<<<<<
  *         else:
  *             self.setitem_indexed(index, value)
  */
-    __Pyx_TraceLine(427,0,__PYX_ERR(2, 427, __pyx_L1_error))
+    __Pyx_TraceLine(429,0,__PYX_ERR(2, 429, __pyx_L1_error))
     /*else*/ {
-      __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_v_index); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 427, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_v_index); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 429, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_memoryview_type))))) __PYX_ERR(2, 427, __pyx_L1_error)
-      __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->setitem_slice_assign_scalar(__pyx_v_self, ((struct __pyx_memoryview_obj *)__pyx_t_4), __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 427, __pyx_L1_error)
+      if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_memoryview_type))))) __PYX_ERR(2, 429, __pyx_L1_error)
+      __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->setitem_slice_assign_scalar(__pyx_v_self, ((struct __pyx_memoryview_obj *)__pyx_t_4), __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 429, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
     __pyx_L5:;
 
-    /* "View.MemoryView":422
+    /* "View.MemoryView":424
  *         have_slices, index = _unellipsify(index, self.view.ndim)
  * 
  *         if have_slices:             # <<<<<<<<<<<<<<
  *             obj = self.is_slice(value)
  *             if obj:
  */
     goto __pyx_L4;
   }
 
-  /* "View.MemoryView":429
+  /* "View.MemoryView":431
  *                 self.setitem_slice_assign_scalar(self[index], value)
  *         else:
  *             self.setitem_indexed(index, value)             # <<<<<<<<<<<<<<
  * 
  *     cdef is_slice(self, obj):
  */
-  __Pyx_TraceLine(429,0,__PYX_ERR(2, 429, __pyx_L1_error))
+  __Pyx_TraceLine(431,0,__PYX_ERR(2, 431, __pyx_L1_error))
   /*else*/ {
-    __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->setitem_indexed(__pyx_v_self, __pyx_v_index, __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 429, __pyx_L1_error)
+    __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->setitem_indexed(__pyx_v_self, __pyx_v_index, __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 431, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_L4:;
 
-  /* "View.MemoryView":416
+  /* "View.MemoryView":418
  *             return self.convert_item_to_object(itemp)
  * 
  *     def __setitem__(memoryview self, object index, object value):             # <<<<<<<<<<<<<<
  *         if self.view.readonly:
  *             raise TypeError("Cannot assign to read-only memoryview")
  */
 
@@ -20259,15 +20453,15 @@
   __Pyx_XDECREF(__pyx_v_obj);
   __Pyx_XDECREF(__pyx_v_index);
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":431
+/* "View.MemoryView":433
  *             self.setitem_indexed(index, value)
  * 
  *     cdef is_slice(self, obj):             # <<<<<<<<<<<<<<
  *         if not isinstance(obj, memoryview):
  *             try:
  */
 
@@ -20284,94 +20478,94 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_slice", 0);
-  __Pyx_TraceCall("is_slice", __pyx_f[2], 431, 0, __PYX_ERR(2, 431, __pyx_L1_error));
+  __Pyx_TraceCall("is_slice", __pyx_f[2], 433, 0, __PYX_ERR(2, 433, __pyx_L1_error));
   __Pyx_INCREF(__pyx_v_obj);
 
-  /* "View.MemoryView":432
+  /* "View.MemoryView":434
  * 
  *     cdef is_slice(self, obj):
  *         if not isinstance(obj, memoryview):             # <<<<<<<<<<<<<<
  *             try:
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,
  */
-  __Pyx_TraceLine(432,0,__PYX_ERR(2, 432, __pyx_L1_error))
+  __Pyx_TraceLine(434,0,__PYX_ERR(2, 434, __pyx_L1_error))
   __pyx_t_1 = __Pyx_TypeCheck(__pyx_v_obj, __pyx_memoryview_type); 
   __pyx_t_2 = ((!(__pyx_t_1 != 0)) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":433
+    /* "View.MemoryView":435
  *     cdef is_slice(self, obj):
  *         if not isinstance(obj, memoryview):
  *             try:             # <<<<<<<<<<<<<<
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,
  *                                  self.dtype_is_object)
  */
-    __Pyx_TraceLine(433,0,__PYX_ERR(2, 433, __pyx_L1_error))
+    __Pyx_TraceLine(435,0,__PYX_ERR(2, 435, __pyx_L1_error))
     {
       __Pyx_PyThreadState_declare
       __Pyx_PyThreadState_assign
       __Pyx_ExceptionSave(&__pyx_t_3, &__pyx_t_4, &__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_3);
       __Pyx_XGOTREF(__pyx_t_4);
       __Pyx_XGOTREF(__pyx_t_5);
       /*try:*/ {
 
-        /* "View.MemoryView":434
+        /* "View.MemoryView":436
  *         if not isinstance(obj, memoryview):
  *             try:
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,             # <<<<<<<<<<<<<<
  *                                  self.dtype_is_object)
  *             except TypeError:
  */
-        __Pyx_TraceLine(434,0,__PYX_ERR(2, 434, __pyx_L4_error))
-        __pyx_t_6 = __Pyx_PyInt_From_int(((__pyx_v_self->flags & (~PyBUF_WRITABLE)) | PyBUF_ANY_CONTIGUOUS)); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 434, __pyx_L4_error)
+        __Pyx_TraceLine(436,0,__PYX_ERR(2, 436, __pyx_L4_error))
+        __pyx_t_6 = __Pyx_PyInt_From_int(((__pyx_v_self->flags & (~PyBUF_WRITABLE)) | PyBUF_ANY_CONTIGUOUS)); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 436, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_6);
 
-        /* "View.MemoryView":435
+        /* "View.MemoryView":437
  *             try:
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,
  *                                  self.dtype_is_object)             # <<<<<<<<<<<<<<
  *             except TypeError:
  *                 return None
  */
-        __Pyx_TraceLine(435,0,__PYX_ERR(2, 435, __pyx_L4_error))
-        __pyx_t_7 = __Pyx_PyBool_FromLong(__pyx_v_self->dtype_is_object); if (unlikely(!__pyx_t_7)) __PYX_ERR(2, 435, __pyx_L4_error)
+        __Pyx_TraceLine(437,0,__PYX_ERR(2, 437, __pyx_L4_error))
+        __pyx_t_7 = __Pyx_PyBool_FromLong(__pyx_v_self->dtype_is_object); if (unlikely(!__pyx_t_7)) __PYX_ERR(2, 437, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_7);
 
-        /* "View.MemoryView":434
+        /* "View.MemoryView":436
  *         if not isinstance(obj, memoryview):
  *             try:
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,             # <<<<<<<<<<<<<<
  *                                  self.dtype_is_object)
  *             except TypeError:
  */
-        __Pyx_TraceLine(434,0,__PYX_ERR(2, 434, __pyx_L4_error))
-        __pyx_t_8 = PyTuple_New(3); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 434, __pyx_L4_error)
+        __Pyx_TraceLine(436,0,__PYX_ERR(2, 436, __pyx_L4_error))
+        __pyx_t_8 = PyTuple_New(3); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 436, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_8);
         __Pyx_INCREF(__pyx_v_obj);
         __Pyx_GIVEREF(__pyx_v_obj);
         PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_v_obj);
         __Pyx_GIVEREF(__pyx_t_6);
         PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_t_6);
         __Pyx_GIVEREF(__pyx_t_7);
         PyTuple_SET_ITEM(__pyx_t_8, 2, __pyx_t_7);
         __pyx_t_6 = 0;
         __pyx_t_7 = 0;
-        __pyx_t_7 = __Pyx_PyObject_Call(((PyObject *)__pyx_memoryview_type), __pyx_t_8, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(2, 434, __pyx_L4_error)
+        __pyx_t_7 = __Pyx_PyObject_Call(((PyObject *)__pyx_memoryview_type), __pyx_t_8, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(2, 436, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         __Pyx_DECREF_SET(__pyx_v_obj, __pyx_t_7);
         __pyx_t_7 = 0;
 
-        /* "View.MemoryView":433
+        /* "View.MemoryView":435
  *     cdef is_slice(self, obj):
  *         if not isinstance(obj, memoryview):
  *             try:             # <<<<<<<<<<<<<<
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,
  *                                  self.dtype_is_object)
  */
       }
@@ -20380,49 +20574,49 @@
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       goto __pyx_L9_try_end;
       __pyx_L4_error:;
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-      /* "View.MemoryView":436
+      /* "View.MemoryView":438
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,
  *                                  self.dtype_is_object)
  *             except TypeError:             # <<<<<<<<<<<<<<
  *                 return None
  * 
  */
-      __Pyx_TraceLine(436,0,__PYX_ERR(2, 436, __pyx_L6_except_error))
+      __Pyx_TraceLine(438,0,__PYX_ERR(2, 438, __pyx_L6_except_error))
       __pyx_t_9 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_TypeError);
       if (__pyx_t_9) {
         __Pyx_AddTraceback("View.MemoryView.memoryview.is_slice", __pyx_clineno, __pyx_lineno, __pyx_filename);
-        if (__Pyx_GetException(&__pyx_t_7, &__pyx_t_8, &__pyx_t_6) < 0) __PYX_ERR(2, 436, __pyx_L6_except_error)
+        if (__Pyx_GetException(&__pyx_t_7, &__pyx_t_8, &__pyx_t_6) < 0) __PYX_ERR(2, 438, __pyx_L6_except_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_GOTREF(__pyx_t_8);
         __Pyx_GOTREF(__pyx_t_6);
 
-        /* "View.MemoryView":437
+        /* "View.MemoryView":439
  *                                  self.dtype_is_object)
  *             except TypeError:
  *                 return None             # <<<<<<<<<<<<<<
  * 
  *         return obj
  */
-        __Pyx_TraceLine(437,0,__PYX_ERR(2, 437, __pyx_L6_except_error))
+        __Pyx_TraceLine(439,0,__PYX_ERR(2, 439, __pyx_L6_except_error))
         __Pyx_XDECREF(__pyx_r);
         __pyx_r = Py_None; __Pyx_INCREF(Py_None);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         goto __pyx_L7_except_return;
       }
       goto __pyx_L6_except_error;
       __pyx_L6_except_error:;
 
-      /* "View.MemoryView":433
+      /* "View.MemoryView":435
  *     cdef is_slice(self, obj):
  *         if not isinstance(obj, memoryview):
  *             try:             # <<<<<<<<<<<<<<
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,
  *                                  self.dtype_is_object)
  */
       __Pyx_XGIVEREF(__pyx_t_3);
@@ -20435,37 +20629,37 @@
       __Pyx_XGIVEREF(__pyx_t_4);
       __Pyx_XGIVEREF(__pyx_t_5);
       __Pyx_ExceptionReset(__pyx_t_3, __pyx_t_4, __pyx_t_5);
       goto __pyx_L0;
       __pyx_L9_try_end:;
     }
 
-    /* "View.MemoryView":432
+    /* "View.MemoryView":434
  * 
  *     cdef is_slice(self, obj):
  *         if not isinstance(obj, memoryview):             # <<<<<<<<<<<<<<
  *             try:
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,
  */
   }
 
-  /* "View.MemoryView":439
+  /* "View.MemoryView":441
  *                 return None
  * 
  *         return obj             # <<<<<<<<<<<<<<
  * 
  *     cdef setitem_slice_assignment(self, dst, src):
  */
-  __Pyx_TraceLine(439,0,__PYX_ERR(2, 439, __pyx_L1_error))
+  __Pyx_TraceLine(441,0,__PYX_ERR(2, 441, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_obj);
   __pyx_r = __pyx_v_obj;
   goto __pyx_L0;
 
-  /* "View.MemoryView":431
+  /* "View.MemoryView":433
  *             self.setitem_indexed(index, value)
  * 
  *     cdef is_slice(self, obj):             # <<<<<<<<<<<<<<
  *         if not isinstance(obj, memoryview):
  *             try:
  */
 
@@ -20480,15 +20674,15 @@
   __Pyx_XDECREF(__pyx_v_obj);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":441
+/* "View.MemoryView":443
  *         return obj
  * 
  *     cdef setitem_slice_assignment(self, dst, src):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice dst_slice
  *         cdef __Pyx_memviewslice src_slice
  */
 
@@ -20504,66 +20698,66 @@
   int __pyx_t_4;
   int __pyx_t_5;
   int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("setitem_slice_assignment", 0);
-  __Pyx_TraceCall("setitem_slice_assignment", __pyx_f[2], 441, 0, __PYX_ERR(2, 441, __pyx_L1_error));
+  __Pyx_TraceCall("setitem_slice_assignment", __pyx_f[2], 443, 0, __PYX_ERR(2, 443, __pyx_L1_error));
 
-  /* "View.MemoryView":445
+  /* "View.MemoryView":447
  *         cdef __Pyx_memviewslice src_slice
  * 
  *         memoryview_copy_contents(get_slice_from_memview(src, &src_slice)[0],             # <<<<<<<<<<<<<<
  *                                  get_slice_from_memview(dst, &dst_slice)[0],
  *                                  src.ndim, dst.ndim, self.dtype_is_object)
  */
-  __Pyx_TraceLine(445,0,__PYX_ERR(2, 445, __pyx_L1_error))
-  if (!(likely(((__pyx_v_src) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_src, __pyx_memoryview_type))))) __PYX_ERR(2, 445, __pyx_L1_error)
-  __pyx_t_1 = __pyx_memoryview_get_slice_from_memoryview(((struct __pyx_memoryview_obj *)__pyx_v_src), (&__pyx_v_src_slice)); if (unlikely(__pyx_t_1 == ((__Pyx_memviewslice *)NULL))) __PYX_ERR(2, 445, __pyx_L1_error)
+  __Pyx_TraceLine(447,0,__PYX_ERR(2, 447, __pyx_L1_error))
+  if (!(likely(((__pyx_v_src) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_src, __pyx_memoryview_type))))) __PYX_ERR(2, 447, __pyx_L1_error)
+  __pyx_t_1 = __pyx_memoryview_get_slice_from_memoryview(((struct __pyx_memoryview_obj *)__pyx_v_src), (&__pyx_v_src_slice)); if (unlikely(__pyx_t_1 == ((__Pyx_memviewslice *)NULL))) __PYX_ERR(2, 447, __pyx_L1_error)
 
-  /* "View.MemoryView":446
+  /* "View.MemoryView":448
  * 
  *         memoryview_copy_contents(get_slice_from_memview(src, &src_slice)[0],
  *                                  get_slice_from_memview(dst, &dst_slice)[0],             # <<<<<<<<<<<<<<
  *                                  src.ndim, dst.ndim, self.dtype_is_object)
  * 
  */
-  __Pyx_TraceLine(446,0,__PYX_ERR(2, 446, __pyx_L1_error))
-  if (!(likely(((__pyx_v_dst) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_dst, __pyx_memoryview_type))))) __PYX_ERR(2, 446, __pyx_L1_error)
-  __pyx_t_2 = __pyx_memoryview_get_slice_from_memoryview(((struct __pyx_memoryview_obj *)__pyx_v_dst), (&__pyx_v_dst_slice)); if (unlikely(__pyx_t_2 == ((__Pyx_memviewslice *)NULL))) __PYX_ERR(2, 446, __pyx_L1_error)
+  __Pyx_TraceLine(448,0,__PYX_ERR(2, 448, __pyx_L1_error))
+  if (!(likely(((__pyx_v_dst) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_dst, __pyx_memoryview_type))))) __PYX_ERR(2, 448, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memoryview_get_slice_from_memoryview(((struct __pyx_memoryview_obj *)__pyx_v_dst), (&__pyx_v_dst_slice)); if (unlikely(__pyx_t_2 == ((__Pyx_memviewslice *)NULL))) __PYX_ERR(2, 448, __pyx_L1_error)
 
-  /* "View.MemoryView":447
+  /* "View.MemoryView":449
  *         memoryview_copy_contents(get_slice_from_memview(src, &src_slice)[0],
  *                                  get_slice_from_memview(dst, &dst_slice)[0],
  *                                  src.ndim, dst.ndim, self.dtype_is_object)             # <<<<<<<<<<<<<<
  * 
  *     cdef setitem_slice_assign_scalar(self, memoryview dst, value):
  */
-  __Pyx_TraceLine(447,0,__PYX_ERR(2, 447, __pyx_L1_error))
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_src, __pyx_n_s_ndim); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 447, __pyx_L1_error)
+  __Pyx_TraceLine(449,0,__PYX_ERR(2, 449, __pyx_L1_error))
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_src, __pyx_n_s_ndim); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 449, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 447, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 449, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_dst, __pyx_n_s_ndim); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 447, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_dst, __pyx_n_s_ndim); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 449, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 447, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 449, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "View.MemoryView":445
+  /* "View.MemoryView":447
  *         cdef __Pyx_memviewslice src_slice
  * 
  *         memoryview_copy_contents(get_slice_from_memview(src, &src_slice)[0],             # <<<<<<<<<<<<<<
  *                                  get_slice_from_memview(dst, &dst_slice)[0],
  *                                  src.ndim, dst.ndim, self.dtype_is_object)
  */
-  __Pyx_TraceLine(445,0,__PYX_ERR(2, 445, __pyx_L1_error))
-  __pyx_t_6 = __pyx_memoryview_copy_contents((__pyx_t_1[0]), (__pyx_t_2[0]), __pyx_t_4, __pyx_t_5, __pyx_v_self->dtype_is_object); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(2, 445, __pyx_L1_error)
+  __Pyx_TraceLine(447,0,__PYX_ERR(2, 447, __pyx_L1_error))
+  __pyx_t_6 = __pyx_memoryview_copy_contents((__pyx_t_1[0]), (__pyx_t_2[0]), __pyx_t_4, __pyx_t_5, __pyx_v_self->dtype_is_object); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(2, 447, __pyx_L1_error)
 
-  /* "View.MemoryView":441
+  /* "View.MemoryView":443
  *         return obj
  * 
  *     cdef setitem_slice_assignment(self, dst, src):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice dst_slice
  *         cdef __Pyx_memviewslice src_slice
  */
 
@@ -20577,15 +20771,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":449
+/* "View.MemoryView":451
  *                                  src.ndim, dst.ndim, self.dtype_is_object)
  * 
  *     cdef setitem_slice_assign_scalar(self, memoryview dst, value):             # <<<<<<<<<<<<<<
  *         cdef int array[128]
  *         cdef void *tmp = NULL
  */
 
@@ -20610,228 +20804,228 @@
   PyObject *__pyx_t_10 = NULL;
   PyObject *__pyx_t_11 = NULL;
   PyObject *__pyx_t_12 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("setitem_slice_assign_scalar", 0);
-  __Pyx_TraceCall("setitem_slice_assign_scalar", __pyx_f[2], 449, 0, __PYX_ERR(2, 449, __pyx_L1_error));
+  __Pyx_TraceCall("setitem_slice_assign_scalar", __pyx_f[2], 451, 0, __PYX_ERR(2, 451, __pyx_L1_error));
 
-  /* "View.MemoryView":451
+  /* "View.MemoryView":453
  *     cdef setitem_slice_assign_scalar(self, memoryview dst, value):
  *         cdef int array[128]
  *         cdef void *tmp = NULL             # <<<<<<<<<<<<<<
  *         cdef void *item
  * 
  */
-  __Pyx_TraceLine(451,0,__PYX_ERR(2, 451, __pyx_L1_error))
+  __Pyx_TraceLine(453,0,__PYX_ERR(2, 453, __pyx_L1_error))
   __pyx_v_tmp = NULL;
 
-  /* "View.MemoryView":456
+  /* "View.MemoryView":458
  *         cdef __Pyx_memviewslice *dst_slice
  *         cdef __Pyx_memviewslice tmp_slice
  *         dst_slice = get_slice_from_memview(dst, &tmp_slice)             # <<<<<<<<<<<<<<
  * 
  *         if <size_t>self.view.itemsize > sizeof(array):
  */
-  __Pyx_TraceLine(456,0,__PYX_ERR(2, 456, __pyx_L1_error))
-  __pyx_t_1 = __pyx_memoryview_get_slice_from_memoryview(__pyx_v_dst, (&__pyx_v_tmp_slice)); if (unlikely(__pyx_t_1 == ((__Pyx_memviewslice *)NULL))) __PYX_ERR(2, 456, __pyx_L1_error)
+  __Pyx_TraceLine(458,0,__PYX_ERR(2, 458, __pyx_L1_error))
+  __pyx_t_1 = __pyx_memoryview_get_slice_from_memoryview(__pyx_v_dst, (&__pyx_v_tmp_slice)); if (unlikely(__pyx_t_1 == ((__Pyx_memviewslice *)NULL))) __PYX_ERR(2, 458, __pyx_L1_error)
   __pyx_v_dst_slice = __pyx_t_1;
 
-  /* "View.MemoryView":458
+  /* "View.MemoryView":460
  *         dst_slice = get_slice_from_memview(dst, &tmp_slice)
  * 
  *         if <size_t>self.view.itemsize > sizeof(array):             # <<<<<<<<<<<<<<
  *             tmp = PyMem_Malloc(self.view.itemsize)
  *             if tmp == NULL:
  */
-  __Pyx_TraceLine(458,0,__PYX_ERR(2, 458, __pyx_L1_error))
+  __Pyx_TraceLine(460,0,__PYX_ERR(2, 460, __pyx_L1_error))
   __pyx_t_2 = ((((size_t)__pyx_v_self->view.itemsize) > (sizeof(__pyx_v_array))) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":459
+    /* "View.MemoryView":461
  * 
  *         if <size_t>self.view.itemsize > sizeof(array):
  *             tmp = PyMem_Malloc(self.view.itemsize)             # <<<<<<<<<<<<<<
  *             if tmp == NULL:
  *                 raise MemoryError
  */
-    __Pyx_TraceLine(459,0,__PYX_ERR(2, 459, __pyx_L1_error))
+    __Pyx_TraceLine(461,0,__PYX_ERR(2, 461, __pyx_L1_error))
     __pyx_v_tmp = PyMem_Malloc(__pyx_v_self->view.itemsize);
 
-    /* "View.MemoryView":460
+    /* "View.MemoryView":462
  *         if <size_t>self.view.itemsize > sizeof(array):
  *             tmp = PyMem_Malloc(self.view.itemsize)
  *             if tmp == NULL:             # <<<<<<<<<<<<<<
  *                 raise MemoryError
  *             item = tmp
  */
-    __Pyx_TraceLine(460,0,__PYX_ERR(2, 460, __pyx_L1_error))
+    __Pyx_TraceLine(462,0,__PYX_ERR(2, 462, __pyx_L1_error))
     __pyx_t_2 = ((__pyx_v_tmp == NULL) != 0);
     if (unlikely(__pyx_t_2)) {
 
-      /* "View.MemoryView":461
+      /* "View.MemoryView":463
  *             tmp = PyMem_Malloc(self.view.itemsize)
  *             if tmp == NULL:
  *                 raise MemoryError             # <<<<<<<<<<<<<<
  *             item = tmp
  *         else:
  */
-      __Pyx_TraceLine(461,0,__PYX_ERR(2, 461, __pyx_L1_error))
-      PyErr_NoMemory(); __PYX_ERR(2, 461, __pyx_L1_error)
+      __Pyx_TraceLine(463,0,__PYX_ERR(2, 463, __pyx_L1_error))
+      PyErr_NoMemory(); __PYX_ERR(2, 463, __pyx_L1_error)
 
-      /* "View.MemoryView":460
+      /* "View.MemoryView":462
  *         if <size_t>self.view.itemsize > sizeof(array):
  *             tmp = PyMem_Malloc(self.view.itemsize)
  *             if tmp == NULL:             # <<<<<<<<<<<<<<
  *                 raise MemoryError
  *             item = tmp
  */
     }
 
-    /* "View.MemoryView":462
+    /* "View.MemoryView":464
  *             if tmp == NULL:
  *                 raise MemoryError
  *             item = tmp             # <<<<<<<<<<<<<<
  *         else:
  *             item = <void *> array
  */
-    __Pyx_TraceLine(462,0,__PYX_ERR(2, 462, __pyx_L1_error))
+    __Pyx_TraceLine(464,0,__PYX_ERR(2, 464, __pyx_L1_error))
     __pyx_v_item = __pyx_v_tmp;
 
-    /* "View.MemoryView":458
+    /* "View.MemoryView":460
  *         dst_slice = get_slice_from_memview(dst, &tmp_slice)
  * 
  *         if <size_t>self.view.itemsize > sizeof(array):             # <<<<<<<<<<<<<<
  *             tmp = PyMem_Malloc(self.view.itemsize)
  *             if tmp == NULL:
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":464
+  /* "View.MemoryView":466
  *             item = tmp
  *         else:
  *             item = <void *> array             # <<<<<<<<<<<<<<
  * 
  *         try:
  */
-  __Pyx_TraceLine(464,0,__PYX_ERR(2, 464, __pyx_L1_error))
+  __Pyx_TraceLine(466,0,__PYX_ERR(2, 466, __pyx_L1_error))
   /*else*/ {
     __pyx_v_item = ((void *)__pyx_v_array);
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":466
+  /* "View.MemoryView":468
  *             item = <void *> array
  * 
  *         try:             # <<<<<<<<<<<<<<
  *             if self.dtype_is_object:
  *                 (<PyObject **> item)[0] = <PyObject *> value
  */
-  __Pyx_TraceLine(466,0,__PYX_ERR(2, 466, __pyx_L1_error))
+  __Pyx_TraceLine(468,0,__PYX_ERR(2, 468, __pyx_L1_error))
   /*try:*/ {
 
-    /* "View.MemoryView":467
+    /* "View.MemoryView":469
  * 
  *         try:
  *             if self.dtype_is_object:             # <<<<<<<<<<<<<<
  *                 (<PyObject **> item)[0] = <PyObject *> value
  *             else:
  */
-    __Pyx_TraceLine(467,0,__PYX_ERR(2, 467, __pyx_L6_error))
+    __Pyx_TraceLine(469,0,__PYX_ERR(2, 469, __pyx_L6_error))
     __pyx_t_2 = (__pyx_v_self->dtype_is_object != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":468
+      /* "View.MemoryView":470
  *         try:
  *             if self.dtype_is_object:
  *                 (<PyObject **> item)[0] = <PyObject *> value             # <<<<<<<<<<<<<<
  *             else:
  *                 self.assign_item_from_object(<char *> item, value)
  */
-      __Pyx_TraceLine(468,0,__PYX_ERR(2, 468, __pyx_L6_error))
+      __Pyx_TraceLine(470,0,__PYX_ERR(2, 470, __pyx_L6_error))
       (((PyObject **)__pyx_v_item)[0]) = ((PyObject *)__pyx_v_value);
 
-      /* "View.MemoryView":467
+      /* "View.MemoryView":469
  * 
  *         try:
  *             if self.dtype_is_object:             # <<<<<<<<<<<<<<
  *                 (<PyObject **> item)[0] = <PyObject *> value
  *             else:
  */
       goto __pyx_L8;
     }
 
-    /* "View.MemoryView":470
+    /* "View.MemoryView":472
  *                 (<PyObject **> item)[0] = <PyObject *> value
  *             else:
  *                 self.assign_item_from_object(<char *> item, value)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __Pyx_TraceLine(470,0,__PYX_ERR(2, 470, __pyx_L6_error))
+    __Pyx_TraceLine(472,0,__PYX_ERR(2, 472, __pyx_L6_error))
     /*else*/ {
-      __pyx_t_3 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->assign_item_from_object(__pyx_v_self, ((char *)__pyx_v_item), __pyx_v_value); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 470, __pyx_L6_error)
+      __pyx_t_3 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->assign_item_from_object(__pyx_v_self, ((char *)__pyx_v_item), __pyx_v_value); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 472, __pyx_L6_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
     __pyx_L8:;
 
-    /* "View.MemoryView":474
+    /* "View.MemoryView":476
  * 
  * 
  *             if self.view.suboffsets != NULL:             # <<<<<<<<<<<<<<
  *                 assert_direct_dimensions(self.view.suboffsets, self.view.ndim)
  *             slice_assign_scalar(dst_slice, dst.view.ndim, self.view.itemsize,
  */
-    __Pyx_TraceLine(474,0,__PYX_ERR(2, 474, __pyx_L6_error))
+    __Pyx_TraceLine(476,0,__PYX_ERR(2, 476, __pyx_L6_error))
     __pyx_t_2 = ((__pyx_v_self->view.suboffsets != NULL) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":475
+      /* "View.MemoryView":477
  * 
  *             if self.view.suboffsets != NULL:
  *                 assert_direct_dimensions(self.view.suboffsets, self.view.ndim)             # <<<<<<<<<<<<<<
  *             slice_assign_scalar(dst_slice, dst.view.ndim, self.view.itemsize,
  *                                 item, self.dtype_is_object)
  */
-      __Pyx_TraceLine(475,0,__PYX_ERR(2, 475, __pyx_L6_error))
-      __pyx_t_3 = assert_direct_dimensions(__pyx_v_self->view.suboffsets, __pyx_v_self->view.ndim); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 475, __pyx_L6_error)
+      __Pyx_TraceLine(477,0,__PYX_ERR(2, 477, __pyx_L6_error))
+      __pyx_t_3 = assert_direct_dimensions(__pyx_v_self->view.suboffsets, __pyx_v_self->view.ndim); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 477, __pyx_L6_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-      /* "View.MemoryView":474
+      /* "View.MemoryView":476
  * 
  * 
  *             if self.view.suboffsets != NULL:             # <<<<<<<<<<<<<<
  *                 assert_direct_dimensions(self.view.suboffsets, self.view.ndim)
  *             slice_assign_scalar(dst_slice, dst.view.ndim, self.view.itemsize,
  */
     }
 
-    /* "View.MemoryView":476
+    /* "View.MemoryView":478
  *             if self.view.suboffsets != NULL:
  *                 assert_direct_dimensions(self.view.suboffsets, self.view.ndim)
  *             slice_assign_scalar(dst_slice, dst.view.ndim, self.view.itemsize,             # <<<<<<<<<<<<<<
  *                                 item, self.dtype_is_object)
  *         finally:
  */
-    __Pyx_TraceLine(476,0,__PYX_ERR(2, 476, __pyx_L6_error))
+    __Pyx_TraceLine(478,0,__PYX_ERR(2, 478, __pyx_L6_error))
     __pyx_memoryview_slice_assign_scalar(__pyx_v_dst_slice, __pyx_v_dst->view.ndim, __pyx_v_self->view.itemsize, __pyx_v_item, __pyx_v_self->dtype_is_object);
   }
 
-  /* "View.MemoryView":479
+  /* "View.MemoryView":481
  *                                 item, self.dtype_is_object)
  *         finally:
  *             PyMem_Free(tmp)             # <<<<<<<<<<<<<<
  * 
  *     cdef setitem_indexed(self, index, value):
  */
-  __Pyx_TraceLine(479,0,__PYX_ERR(2, 479, __pyx_L6_error))
+  __Pyx_TraceLine(481,0,__PYX_ERR(2, 481, __pyx_L6_error))
   /*finally:*/ {
     /*normal exit:*/{
       PyMem_Free(__pyx_v_tmp);
       goto __pyx_L7;
     }
     __pyx_L6_error:;
     /*exception exit:*/{
@@ -20864,15 +21058,15 @@
       __pyx_t_7 = 0; __pyx_t_8 = 0; __pyx_t_9 = 0; __pyx_t_10 = 0; __pyx_t_11 = 0; __pyx_t_12 = 0;
       __pyx_lineno = __pyx_t_4; __pyx_clineno = __pyx_t_5; __pyx_filename = __pyx_t_6;
       goto __pyx_L1_error;
     }
     __pyx_L7:;
   }
 
-  /* "View.MemoryView":449
+  /* "View.MemoryView":451
  *                                  src.ndim, dst.ndim, self.dtype_is_object)
  * 
  *     cdef setitem_slice_assign_scalar(self, memoryview dst, value):             # <<<<<<<<<<<<<<
  *         cdef int array[128]
  *         cdef void *tmp = NULL
  */
 
@@ -20886,15 +21080,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":481
+/* "View.MemoryView":483
  *             PyMem_Free(tmp)
  * 
  *     cdef setitem_indexed(self, index, value):             # <<<<<<<<<<<<<<
  *         cdef char *itemp = self.get_item_pointer(index)
  *         self.assign_item_from_object(itemp, value)
  */
 
@@ -20905,40 +21099,40 @@
   __Pyx_RefNannyDeclarations
   char *__pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("setitem_indexed", 0);
-  __Pyx_TraceCall("setitem_indexed", __pyx_f[2], 481, 0, __PYX_ERR(2, 481, __pyx_L1_error));
+  __Pyx_TraceCall("setitem_indexed", __pyx_f[2], 483, 0, __PYX_ERR(2, 483, __pyx_L1_error));
 
-  /* "View.MemoryView":482
+  /* "View.MemoryView":484
  * 
  *     cdef setitem_indexed(self, index, value):
  *         cdef char *itemp = self.get_item_pointer(index)             # <<<<<<<<<<<<<<
  *         self.assign_item_from_object(itemp, value)
  * 
  */
-  __Pyx_TraceLine(482,0,__PYX_ERR(2, 482, __pyx_L1_error))
-  __pyx_t_1 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->get_item_pointer(__pyx_v_self, __pyx_v_index); if (unlikely(__pyx_t_1 == ((char *)NULL))) __PYX_ERR(2, 482, __pyx_L1_error)
+  __Pyx_TraceLine(484,0,__PYX_ERR(2, 484, __pyx_L1_error))
+  __pyx_t_1 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->get_item_pointer(__pyx_v_self, __pyx_v_index); if (unlikely(__pyx_t_1 == ((char *)NULL))) __PYX_ERR(2, 484, __pyx_L1_error)
   __pyx_v_itemp = __pyx_t_1;
 
-  /* "View.MemoryView":483
+  /* "View.MemoryView":485
  *     cdef setitem_indexed(self, index, value):
  *         cdef char *itemp = self.get_item_pointer(index)
  *         self.assign_item_from_object(itemp, value)             # <<<<<<<<<<<<<<
  * 
  *     cdef convert_item_to_object(self, char *itemp):
  */
-  __Pyx_TraceLine(483,0,__PYX_ERR(2, 483, __pyx_L1_error))
-  __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->assign_item_from_object(__pyx_v_self, __pyx_v_itemp, __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 483, __pyx_L1_error)
+  __Pyx_TraceLine(485,0,__PYX_ERR(2, 485, __pyx_L1_error))
+  __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->assign_item_from_object(__pyx_v_self, __pyx_v_itemp, __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 485, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "View.MemoryView":481
+  /* "View.MemoryView":483
  *             PyMem_Free(tmp)
  * 
  *     cdef setitem_indexed(self, index, value):             # <<<<<<<<<<<<<<
  *         cdef char *itemp = self.get_item_pointer(index)
  *         self.assign_item_from_object(itemp, value)
  */
 
@@ -20952,15 +21146,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":485
+/* "View.MemoryView":487
  *         self.assign_item_from_object(itemp, value)
  * 
  *     cdef convert_item_to_object(self, char *itemp):             # <<<<<<<<<<<<<<
  *         """Only used if instantiated manually by the user, or if Cython doesn't
  *         know how to convert the type"""
  */
 
@@ -20982,70 +21176,70 @@
   PyObject *__pyx_t_9 = NULL;
   size_t __pyx_t_10;
   int __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("convert_item_to_object", 0);
-  __Pyx_TraceCall("convert_item_to_object", __pyx_f[2], 485, 0, __PYX_ERR(2, 485, __pyx_L1_error));
+  __Pyx_TraceCall("convert_item_to_object", __pyx_f[2], 487, 0, __PYX_ERR(2, 487, __pyx_L1_error));
 
-  /* "View.MemoryView":488
+  /* "View.MemoryView":490
  *         """Only used if instantiated manually by the user, or if Cython doesn't
  *         know how to convert the type"""
  *         import struct             # <<<<<<<<<<<<<<
  *         cdef bytes bytesitem
  * 
  */
-  __Pyx_TraceLine(488,0,__PYX_ERR(2, 488, __pyx_L1_error))
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_struct, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 488, __pyx_L1_error)
+  __Pyx_TraceLine(490,0,__PYX_ERR(2, 490, __pyx_L1_error))
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_struct, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 490, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_struct = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "View.MemoryView":491
+  /* "View.MemoryView":493
  *         cdef bytes bytesitem
  * 
  *         bytesitem = itemp[:self.view.itemsize]             # <<<<<<<<<<<<<<
  *         try:
  *             result = struct.unpack(self.view.format, bytesitem)
  */
-  __Pyx_TraceLine(491,0,__PYX_ERR(2, 491, __pyx_L1_error))
-  __pyx_t_1 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_itemp + 0, __pyx_v_self->view.itemsize - 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 491, __pyx_L1_error)
+  __Pyx_TraceLine(493,0,__PYX_ERR(2, 493, __pyx_L1_error))
+  __pyx_t_1 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_itemp + 0, __pyx_v_self->view.itemsize - 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 493, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_bytesitem = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "View.MemoryView":492
+  /* "View.MemoryView":494
  * 
  *         bytesitem = itemp[:self.view.itemsize]
  *         try:             # <<<<<<<<<<<<<<
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  */
-  __Pyx_TraceLine(492,0,__PYX_ERR(2, 492, __pyx_L1_error))
+  __Pyx_TraceLine(494,0,__PYX_ERR(2, 494, __pyx_L1_error))
   {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_2, &__pyx_t_3, &__pyx_t_4);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_4);
     /*try:*/ {
 
-      /* "View.MemoryView":493
+      /* "View.MemoryView":495
  *         bytesitem = itemp[:self.view.itemsize]
  *         try:
  *             result = struct.unpack(self.view.format, bytesitem)             # <<<<<<<<<<<<<<
  *         except struct.error:
  *             raise ValueError("Unable to convert item to object")
  */
-      __Pyx_TraceLine(493,0,__PYX_ERR(2, 493, __pyx_L3_error))
-      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_unpack); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 493, __pyx_L3_error)
+      __Pyx_TraceLine(495,0,__PYX_ERR(2, 495, __pyx_L3_error))
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_unpack); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 495, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_6 = __Pyx_PyBytes_FromString(__pyx_v_self->view.format); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 493, __pyx_L3_error)
+      __pyx_t_6 = __Pyx_PyBytes_FromString(__pyx_v_self->view.format); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 495, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_6);
       __pyx_t_7 = NULL;
       __pyx_t_8 = 0;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
         __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_5);
         if (likely(__pyx_t_7)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
@@ -21054,155 +21248,155 @@
           __Pyx_DECREF_SET(__pyx_t_5, function);
           __pyx_t_8 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_5)) {
         PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_t_6, __pyx_v_bytesitem};
-        __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 493, __pyx_L3_error)
+        __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 495, __pyx_L3_error)
         __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_5)) {
         PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_t_6, __pyx_v_bytesitem};
-        __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 493, __pyx_L3_error)
+        __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 495, __pyx_L3_error)
         __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       } else
       #endif
       {
-        __pyx_t_9 = PyTuple_New(2+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 493, __pyx_L3_error)
+        __pyx_t_9 = PyTuple_New(2+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 495, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_9);
         if (__pyx_t_7) {
           __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_7); __pyx_t_7 = NULL;
         }
         __Pyx_GIVEREF(__pyx_t_6);
         PyTuple_SET_ITEM(__pyx_t_9, 0+__pyx_t_8, __pyx_t_6);
         __Pyx_INCREF(__pyx_v_bytesitem);
         __Pyx_GIVEREF(__pyx_v_bytesitem);
         PyTuple_SET_ITEM(__pyx_t_9, 1+__pyx_t_8, __pyx_v_bytesitem);
         __pyx_t_6 = 0;
-        __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 493, __pyx_L3_error)
+        __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 495, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       }
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __pyx_v_result = __pyx_t_1;
       __pyx_t_1 = 0;
 
-      /* "View.MemoryView":492
+      /* "View.MemoryView":494
  * 
  *         bytesitem = itemp[:self.view.itemsize]
  *         try:             # <<<<<<<<<<<<<<
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  */
     }
 
-    /* "View.MemoryView":497
+    /* "View.MemoryView":499
  *             raise ValueError("Unable to convert item to object")
  *         else:
  *             if len(self.view.format) == 1:             # <<<<<<<<<<<<<<
  *                 return result[0]
  *             return result
  */
-    __Pyx_TraceLine(497,0,__PYX_ERR(2, 497, __pyx_L5_except_error))
+    __Pyx_TraceLine(499,0,__PYX_ERR(2, 499, __pyx_L5_except_error))
     /*else:*/ {
       __pyx_t_10 = strlen(__pyx_v_self->view.format); 
       __pyx_t_11 = ((__pyx_t_10 == 1) != 0);
       if (__pyx_t_11) {
 
-        /* "View.MemoryView":498
+        /* "View.MemoryView":500
  *         else:
  *             if len(self.view.format) == 1:
  *                 return result[0]             # <<<<<<<<<<<<<<
  *             return result
  * 
  */
-        __Pyx_TraceLine(498,0,__PYX_ERR(2, 498, __pyx_L5_except_error))
+        __Pyx_TraceLine(500,0,__PYX_ERR(2, 500, __pyx_L5_except_error))
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_result, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 498, __pyx_L5_except_error)
+        __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_result, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 500, __pyx_L5_except_error)
         __Pyx_GOTREF(__pyx_t_1);
         __pyx_r = __pyx_t_1;
         __pyx_t_1 = 0;
         goto __pyx_L6_except_return;
 
-        /* "View.MemoryView":497
+        /* "View.MemoryView":499
  *             raise ValueError("Unable to convert item to object")
  *         else:
  *             if len(self.view.format) == 1:             # <<<<<<<<<<<<<<
  *                 return result[0]
  *             return result
  */
       }
 
-      /* "View.MemoryView":499
+      /* "View.MemoryView":501
  *             if len(self.view.format) == 1:
  *                 return result[0]
  *             return result             # <<<<<<<<<<<<<<
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):
  */
-      __Pyx_TraceLine(499,0,__PYX_ERR(2, 499, __pyx_L5_except_error))
+      __Pyx_TraceLine(501,0,__PYX_ERR(2, 501, __pyx_L5_except_error))
       __Pyx_XDECREF(__pyx_r);
       __Pyx_INCREF(__pyx_v_result);
       __pyx_r = __pyx_v_result;
       goto __pyx_L6_except_return;
     }
     __pyx_L3_error:;
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-    /* "View.MemoryView":494
+    /* "View.MemoryView":496
  *         try:
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:             # <<<<<<<<<<<<<<
  *             raise ValueError("Unable to convert item to object")
  *         else:
  */
-    __Pyx_TraceLine(494,0,__PYX_ERR(2, 494, __pyx_L5_except_error))
+    __Pyx_TraceLine(496,0,__PYX_ERR(2, 496, __pyx_L5_except_error))
     __Pyx_ErrFetch(&__pyx_t_1, &__pyx_t_5, &__pyx_t_9);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_error); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 494, __pyx_L5_except_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_error); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 496, __pyx_L5_except_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_8 = __Pyx_PyErr_GivenExceptionMatches(__pyx_t_1, __pyx_t_6);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_ErrRestore(__pyx_t_1, __pyx_t_5, __pyx_t_9);
     __pyx_t_1 = 0; __pyx_t_5 = 0; __pyx_t_9 = 0;
     if (__pyx_t_8) {
       __Pyx_AddTraceback("View.MemoryView.memoryview.convert_item_to_object", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_9, &__pyx_t_5, &__pyx_t_1) < 0) __PYX_ERR(2, 494, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_9, &__pyx_t_5, &__pyx_t_1) < 0) __PYX_ERR(2, 496, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_9);
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_1);
 
-      /* "View.MemoryView":495
+      /* "View.MemoryView":497
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  *             raise ValueError("Unable to convert item to object")             # <<<<<<<<<<<<<<
  *         else:
  *             if len(self.view.format) == 1:
  */
-      __Pyx_TraceLine(495,0,__PYX_ERR(2, 495, __pyx_L5_except_error))
-      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__19, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 495, __pyx_L5_except_error)
+      __Pyx_TraceLine(497,0,__PYX_ERR(2, 497, __pyx_L5_except_error))
+      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__20, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 497, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_Raise(__pyx_t_6, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __PYX_ERR(2, 495, __pyx_L5_except_error)
+      __PYX_ERR(2, 497, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "View.MemoryView":492
+    /* "View.MemoryView":494
  * 
  *         bytesitem = itemp[:self.view.itemsize]
  *         try:             # <<<<<<<<<<<<<<
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  */
     __Pyx_XGIVEREF(__pyx_t_2);
@@ -21214,15 +21408,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_XGIVEREF(__pyx_t_4);
     __Pyx_ExceptionReset(__pyx_t_2, __pyx_t_3, __pyx_t_4);
     goto __pyx_L0;
   }
 
-  /* "View.MemoryView":485
+  /* "View.MemoryView":487
  *         self.assign_item_from_object(itemp, value)
  * 
  *     cdef convert_item_to_object(self, char *itemp):             # <<<<<<<<<<<<<<
  *         """Only used if instantiated manually by the user, or if Cython doesn't
  *         know how to convert the type"""
  */
 
@@ -21241,15 +21435,15 @@
   __Pyx_XDECREF(__pyx_v_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":501
+/* "View.MemoryView":503
  *             return result
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):             # <<<<<<<<<<<<<<
  *         """Only used if instantiated manually by the user, or if Cython doesn't
  *         know how to convert the type"""
  */
 
@@ -21275,94 +21469,94 @@
   char *__pyx_t_12;
   char *__pyx_t_13;
   char *__pyx_t_14;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("assign_item_from_object", 0);
-  __Pyx_TraceCall("assign_item_from_object", __pyx_f[2], 501, 0, __PYX_ERR(2, 501, __pyx_L1_error));
+  __Pyx_TraceCall("assign_item_from_object", __pyx_f[2], 503, 0, __PYX_ERR(2, 503, __pyx_L1_error));
 
-  /* "View.MemoryView":504
+  /* "View.MemoryView":506
  *         """Only used if instantiated manually by the user, or if Cython doesn't
  *         know how to convert the type"""
  *         import struct             # <<<<<<<<<<<<<<
  *         cdef char c
  *         cdef bytes bytesvalue
  */
-  __Pyx_TraceLine(504,0,__PYX_ERR(2, 504, __pyx_L1_error))
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_struct, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 504, __pyx_L1_error)
+  __Pyx_TraceLine(506,0,__PYX_ERR(2, 506, __pyx_L1_error))
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_struct, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 506, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_struct = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "View.MemoryView":509
+  /* "View.MemoryView":511
  *         cdef Py_ssize_t i
  * 
  *         if isinstance(value, tuple):             # <<<<<<<<<<<<<<
  *             bytesvalue = struct.pack(self.view.format, *value)
  *         else:
  */
-  __Pyx_TraceLine(509,0,__PYX_ERR(2, 509, __pyx_L1_error))
+  __Pyx_TraceLine(511,0,__PYX_ERR(2, 511, __pyx_L1_error))
   __pyx_t_2 = PyTuple_Check(__pyx_v_value); 
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
-    /* "View.MemoryView":510
+    /* "View.MemoryView":512
  * 
  *         if isinstance(value, tuple):
  *             bytesvalue = struct.pack(self.view.format, *value)             # <<<<<<<<<<<<<<
  *         else:
  *             bytesvalue = struct.pack(self.view.format, value)
  */
-    __Pyx_TraceLine(510,0,__PYX_ERR(2, 510, __pyx_L1_error))
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_pack); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 510, __pyx_L1_error)
+    __Pyx_TraceLine(512,0,__PYX_ERR(2, 512, __pyx_L1_error))
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_pack); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 512, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = __Pyx_PyBytes_FromString(__pyx_v_self->view.format); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 510, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyBytes_FromString(__pyx_v_self->view.format); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 512, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 510, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 512, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_4);
     __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PySequence_Tuple(__pyx_v_value); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 510, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PySequence_Tuple(__pyx_v_value); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 512, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_6 = PyNumber_Add(__pyx_t_5, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 510, __pyx_L1_error)
+    __pyx_t_6 = PyNumber_Add(__pyx_t_5, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 512, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_6, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 510, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_6, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 512, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(2, 510, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(2, 512, __pyx_L1_error)
     __pyx_v_bytesvalue = ((PyObject*)__pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "View.MemoryView":509
+    /* "View.MemoryView":511
  *         cdef Py_ssize_t i
  * 
  *         if isinstance(value, tuple):             # <<<<<<<<<<<<<<
  *             bytesvalue = struct.pack(self.view.format, *value)
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":512
+  /* "View.MemoryView":514
  *             bytesvalue = struct.pack(self.view.format, *value)
  *         else:
  *             bytesvalue = struct.pack(self.view.format, value)             # <<<<<<<<<<<<<<
  * 
  *         for i, c in enumerate(bytesvalue):
  */
-  __Pyx_TraceLine(512,0,__PYX_ERR(2, 512, __pyx_L1_error))
+  __Pyx_TraceLine(514,0,__PYX_ERR(2, 514, __pyx_L1_error))
   /*else*/ {
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_pack); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 512, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_pack); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 514, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_1 = __Pyx_PyBytes_FromString(__pyx_v_self->view.format); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 512, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyBytes_FromString(__pyx_v_self->view.format); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 514, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_5 = NULL;
     __pyx_t_7 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_6);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
@@ -21371,106 +21565,106 @@
         __Pyx_DECREF_SET(__pyx_t_6, function);
         __pyx_t_7 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_6)) {
       PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_t_1, __pyx_v_value};
-      __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 512, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 514, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_6)) {
       PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_t_1, __pyx_v_value};
-      __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 512, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 514, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     } else
     #endif
     {
-      __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 512, __pyx_L1_error)
+      __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 514, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       if (__pyx_t_5) {
         __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_5); __pyx_t_5 = NULL;
       }
       __Pyx_GIVEREF(__pyx_t_1);
       PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_t_1);
       __Pyx_INCREF(__pyx_v_value);
       __Pyx_GIVEREF(__pyx_v_value);
       PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_v_value);
       __pyx_t_1 = 0;
-      __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_8, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 512, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_8, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 514, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     }
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(2, 512, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(2, 514, __pyx_L1_error)
     __pyx_v_bytesvalue = ((PyObject*)__pyx_t_4);
     __pyx_t_4 = 0;
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":514
+  /* "View.MemoryView":516
  *             bytesvalue = struct.pack(self.view.format, value)
  * 
  *         for i, c in enumerate(bytesvalue):             # <<<<<<<<<<<<<<
  *             itemp[i] = c
  * 
  */
-  __Pyx_TraceLine(514,0,__PYX_ERR(2, 514, __pyx_L1_error))
+  __Pyx_TraceLine(516,0,__PYX_ERR(2, 516, __pyx_L1_error))
   __pyx_t_9 = 0;
   if (unlikely(__pyx_v_bytesvalue == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' is not iterable");
-    __PYX_ERR(2, 514, __pyx_L1_error)
+    __PYX_ERR(2, 516, __pyx_L1_error)
   }
   __Pyx_INCREF(__pyx_v_bytesvalue);
   __pyx_t_10 = __pyx_v_bytesvalue;
   __pyx_t_12 = PyBytes_AS_STRING(__pyx_t_10);
   __pyx_t_13 = (__pyx_t_12 + PyBytes_GET_SIZE(__pyx_t_10));
   for (__pyx_t_14 = __pyx_t_12; __pyx_t_14 < __pyx_t_13; __pyx_t_14++) {
     __pyx_t_11 = __pyx_t_14;
     __pyx_v_c = (__pyx_t_11[0]);
 
-    /* "View.MemoryView":515
+    /* "View.MemoryView":517
  * 
  *         for i, c in enumerate(bytesvalue):
  *             itemp[i] = c             # <<<<<<<<<<<<<<
  * 
  *     @cname('getbuffer')
  */
-    __Pyx_TraceLine(515,0,__PYX_ERR(2, 515, __pyx_L1_error))
+    __Pyx_TraceLine(517,0,__PYX_ERR(2, 517, __pyx_L1_error))
     __pyx_v_i = __pyx_t_9;
 
-    /* "View.MemoryView":514
+    /* "View.MemoryView":516
  *             bytesvalue = struct.pack(self.view.format, value)
  * 
  *         for i, c in enumerate(bytesvalue):             # <<<<<<<<<<<<<<
  *             itemp[i] = c
  * 
  */
-    __Pyx_TraceLine(514,0,__PYX_ERR(2, 514, __pyx_L1_error))
+    __Pyx_TraceLine(516,0,__PYX_ERR(2, 516, __pyx_L1_error))
     __pyx_t_9 = (__pyx_t_9 + 1);
 
-    /* "View.MemoryView":515
+    /* "View.MemoryView":517
  * 
  *         for i, c in enumerate(bytesvalue):
  *             itemp[i] = c             # <<<<<<<<<<<<<<
  * 
  *     @cname('getbuffer')
  */
-    __Pyx_TraceLine(515,0,__PYX_ERR(2, 515, __pyx_L1_error))
+    __Pyx_TraceLine(517,0,__PYX_ERR(2, 517, __pyx_L1_error))
     (__pyx_v_itemp[__pyx_v_i]) = __pyx_v_c;
   }
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-  /* "View.MemoryView":501
+  /* "View.MemoryView":503
  *             return result
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):             # <<<<<<<<<<<<<<
  *         """Only used if instantiated manually by the user, or if Cython doesn't
  *         know how to convert the type"""
  */
 
@@ -21491,15 +21685,15 @@
   __Pyx_XDECREF(__pyx_v_bytesvalue);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":518
+/* "View.MemoryView":520
  * 
  *     @cname('getbuffer')
  *     def __getbuffer__(self, Py_buffer *info, int flags):             # <<<<<<<<<<<<<<
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")
  */
 
@@ -21534,308 +21728,308 @@
   if (__pyx_v_info == NULL) {
     PyErr_SetString(PyExc_BufferError, "PyObject_GetBuffer: view==NULL argument is obsolete");
     return -1;
   }
   __Pyx_RefNannySetupContext("__getbuffer__", 0);
   __pyx_v_info->obj = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(__pyx_v_info->obj);
-  __Pyx_TraceCall("__getbuffer__", __pyx_f[2], 518, 0, __PYX_ERR(2, 518, __pyx_L1_error));
+  __Pyx_TraceCall("__getbuffer__", __pyx_f[2], 520, 0, __PYX_ERR(2, 520, __pyx_L1_error));
 
-  /* "View.MemoryView":519
+  /* "View.MemoryView":521
  *     @cname('getbuffer')
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:             # <<<<<<<<<<<<<<
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")
  * 
  */
-  __Pyx_TraceLine(519,0,__PYX_ERR(2, 519, __pyx_L1_error))
+  __Pyx_TraceLine(521,0,__PYX_ERR(2, 521, __pyx_L1_error))
   __pyx_t_2 = ((__pyx_v_flags & PyBUF_WRITABLE) != 0);
   if (__pyx_t_2) {
   } else {
     __pyx_t_1 = __pyx_t_2;
     goto __pyx_L4_bool_binop_done;
   }
   __pyx_t_2 = (__pyx_v_self->view.readonly != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L4_bool_binop_done:;
   if (unlikely(__pyx_t_1)) {
 
-    /* "View.MemoryView":520
+    /* "View.MemoryView":522
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_ND:
  */
-    __Pyx_TraceLine(520,0,__PYX_ERR(2, 520, __pyx_L1_error))
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__20, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 520, __pyx_L1_error)
+    __Pyx_TraceLine(522,0,__PYX_ERR(2, 522, __pyx_L1_error))
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__21, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 522, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(2, 520, __pyx_L1_error)
+    __PYX_ERR(2, 522, __pyx_L1_error)
 
-    /* "View.MemoryView":519
+    /* "View.MemoryView":521
  *     @cname('getbuffer')
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:             # <<<<<<<<<<<<<<
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")
  * 
  */
   }
 
-  /* "View.MemoryView":522
+  /* "View.MemoryView":524
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")
  * 
  *         if flags & PyBUF_ND:             # <<<<<<<<<<<<<<
  *             info.shape = self.view.shape
  *         else:
  */
-  __Pyx_TraceLine(522,0,__PYX_ERR(2, 522, __pyx_L1_error))
+  __Pyx_TraceLine(524,0,__PYX_ERR(2, 524, __pyx_L1_error))
   __pyx_t_1 = ((__pyx_v_flags & PyBUF_ND) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":523
+    /* "View.MemoryView":525
  * 
  *         if flags & PyBUF_ND:
  *             info.shape = self.view.shape             # <<<<<<<<<<<<<<
  *         else:
  *             info.shape = NULL
  */
-    __Pyx_TraceLine(523,0,__PYX_ERR(2, 523, __pyx_L1_error))
+    __Pyx_TraceLine(525,0,__PYX_ERR(2, 525, __pyx_L1_error))
     __pyx_t_4 = __pyx_v_self->view.shape;
     __pyx_v_info->shape = __pyx_t_4;
 
-    /* "View.MemoryView":522
+    /* "View.MemoryView":524
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")
  * 
  *         if flags & PyBUF_ND:             # <<<<<<<<<<<<<<
  *             info.shape = self.view.shape
  *         else:
  */
     goto __pyx_L6;
   }
 
-  /* "View.MemoryView":525
+  /* "View.MemoryView":527
  *             info.shape = self.view.shape
  *         else:
  *             info.shape = NULL             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_STRIDES:
  */
-  __Pyx_TraceLine(525,0,__PYX_ERR(2, 525, __pyx_L1_error))
+  __Pyx_TraceLine(527,0,__PYX_ERR(2, 527, __pyx_L1_error))
   /*else*/ {
     __pyx_v_info->shape = NULL;
   }
   __pyx_L6:;
 
-  /* "View.MemoryView":527
+  /* "View.MemoryView":529
  *             info.shape = NULL
  * 
  *         if flags & PyBUF_STRIDES:             # <<<<<<<<<<<<<<
  *             info.strides = self.view.strides
  *         else:
  */
-  __Pyx_TraceLine(527,0,__PYX_ERR(2, 527, __pyx_L1_error))
+  __Pyx_TraceLine(529,0,__PYX_ERR(2, 529, __pyx_L1_error))
   __pyx_t_1 = ((__pyx_v_flags & PyBUF_STRIDES) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":528
+    /* "View.MemoryView":530
  * 
  *         if flags & PyBUF_STRIDES:
  *             info.strides = self.view.strides             # <<<<<<<<<<<<<<
  *         else:
  *             info.strides = NULL
  */
-    __Pyx_TraceLine(528,0,__PYX_ERR(2, 528, __pyx_L1_error))
+    __Pyx_TraceLine(530,0,__PYX_ERR(2, 530, __pyx_L1_error))
     __pyx_t_4 = __pyx_v_self->view.strides;
     __pyx_v_info->strides = __pyx_t_4;
 
-    /* "View.MemoryView":527
+    /* "View.MemoryView":529
  *             info.shape = NULL
  * 
  *         if flags & PyBUF_STRIDES:             # <<<<<<<<<<<<<<
  *             info.strides = self.view.strides
  *         else:
  */
     goto __pyx_L7;
   }
 
-  /* "View.MemoryView":530
+  /* "View.MemoryView":532
  *             info.strides = self.view.strides
  *         else:
  *             info.strides = NULL             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_INDIRECT:
  */
-  __Pyx_TraceLine(530,0,__PYX_ERR(2, 530, __pyx_L1_error))
+  __Pyx_TraceLine(532,0,__PYX_ERR(2, 532, __pyx_L1_error))
   /*else*/ {
     __pyx_v_info->strides = NULL;
   }
   __pyx_L7:;
 
-  /* "View.MemoryView":532
+  /* "View.MemoryView":534
  *             info.strides = NULL
  * 
  *         if flags & PyBUF_INDIRECT:             # <<<<<<<<<<<<<<
  *             info.suboffsets = self.view.suboffsets
  *         else:
  */
-  __Pyx_TraceLine(532,0,__PYX_ERR(2, 532, __pyx_L1_error))
+  __Pyx_TraceLine(534,0,__PYX_ERR(2, 534, __pyx_L1_error))
   __pyx_t_1 = ((__pyx_v_flags & PyBUF_INDIRECT) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":533
+    /* "View.MemoryView":535
  * 
  *         if flags & PyBUF_INDIRECT:
  *             info.suboffsets = self.view.suboffsets             # <<<<<<<<<<<<<<
  *         else:
  *             info.suboffsets = NULL
  */
-    __Pyx_TraceLine(533,0,__PYX_ERR(2, 533, __pyx_L1_error))
+    __Pyx_TraceLine(535,0,__PYX_ERR(2, 535, __pyx_L1_error))
     __pyx_t_4 = __pyx_v_self->view.suboffsets;
     __pyx_v_info->suboffsets = __pyx_t_4;
 
-    /* "View.MemoryView":532
+    /* "View.MemoryView":534
  *             info.strides = NULL
  * 
  *         if flags & PyBUF_INDIRECT:             # <<<<<<<<<<<<<<
  *             info.suboffsets = self.view.suboffsets
  *         else:
  */
     goto __pyx_L8;
   }
 
-  /* "View.MemoryView":535
+  /* "View.MemoryView":537
  *             info.suboffsets = self.view.suboffsets
  *         else:
  *             info.suboffsets = NULL             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_FORMAT:
  */
-  __Pyx_TraceLine(535,0,__PYX_ERR(2, 535, __pyx_L1_error))
+  __Pyx_TraceLine(537,0,__PYX_ERR(2, 537, __pyx_L1_error))
   /*else*/ {
     __pyx_v_info->suboffsets = NULL;
   }
   __pyx_L8:;
 
-  /* "View.MemoryView":537
+  /* "View.MemoryView":539
  *             info.suboffsets = NULL
  * 
  *         if flags & PyBUF_FORMAT:             # <<<<<<<<<<<<<<
  *             info.format = self.view.format
  *         else:
  */
-  __Pyx_TraceLine(537,0,__PYX_ERR(2, 537, __pyx_L1_error))
+  __Pyx_TraceLine(539,0,__PYX_ERR(2, 539, __pyx_L1_error))
   __pyx_t_1 = ((__pyx_v_flags & PyBUF_FORMAT) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":538
+    /* "View.MemoryView":540
  * 
  *         if flags & PyBUF_FORMAT:
  *             info.format = self.view.format             # <<<<<<<<<<<<<<
  *         else:
  *             info.format = NULL
  */
-    __Pyx_TraceLine(538,0,__PYX_ERR(2, 538, __pyx_L1_error))
+    __Pyx_TraceLine(540,0,__PYX_ERR(2, 540, __pyx_L1_error))
     __pyx_t_5 = __pyx_v_self->view.format;
     __pyx_v_info->format = __pyx_t_5;
 
-    /* "View.MemoryView":537
+    /* "View.MemoryView":539
  *             info.suboffsets = NULL
  * 
  *         if flags & PyBUF_FORMAT:             # <<<<<<<<<<<<<<
  *             info.format = self.view.format
  *         else:
  */
     goto __pyx_L9;
   }
 
-  /* "View.MemoryView":540
+  /* "View.MemoryView":542
  *             info.format = self.view.format
  *         else:
  *             info.format = NULL             # <<<<<<<<<<<<<<
  * 
  *         info.buf = self.view.buf
  */
-  __Pyx_TraceLine(540,0,__PYX_ERR(2, 540, __pyx_L1_error))
+  __Pyx_TraceLine(542,0,__PYX_ERR(2, 542, __pyx_L1_error))
   /*else*/ {
     __pyx_v_info->format = NULL;
   }
   __pyx_L9:;
 
-  /* "View.MemoryView":542
+  /* "View.MemoryView":544
  *             info.format = NULL
  * 
  *         info.buf = self.view.buf             # <<<<<<<<<<<<<<
  *         info.ndim = self.view.ndim
  *         info.itemsize = self.view.itemsize
  */
-  __Pyx_TraceLine(542,0,__PYX_ERR(2, 542, __pyx_L1_error))
+  __Pyx_TraceLine(544,0,__PYX_ERR(2, 544, __pyx_L1_error))
   __pyx_t_6 = __pyx_v_self->view.buf;
   __pyx_v_info->buf = __pyx_t_6;
 
-  /* "View.MemoryView":543
+  /* "View.MemoryView":545
  * 
  *         info.buf = self.view.buf
  *         info.ndim = self.view.ndim             # <<<<<<<<<<<<<<
  *         info.itemsize = self.view.itemsize
  *         info.len = self.view.len
  */
-  __Pyx_TraceLine(543,0,__PYX_ERR(2, 543, __pyx_L1_error))
+  __Pyx_TraceLine(545,0,__PYX_ERR(2, 545, __pyx_L1_error))
   __pyx_t_7 = __pyx_v_self->view.ndim;
   __pyx_v_info->ndim = __pyx_t_7;
 
-  /* "View.MemoryView":544
+  /* "View.MemoryView":546
  *         info.buf = self.view.buf
  *         info.ndim = self.view.ndim
  *         info.itemsize = self.view.itemsize             # <<<<<<<<<<<<<<
  *         info.len = self.view.len
  *         info.readonly = self.view.readonly
  */
-  __Pyx_TraceLine(544,0,__PYX_ERR(2, 544, __pyx_L1_error))
+  __Pyx_TraceLine(546,0,__PYX_ERR(2, 546, __pyx_L1_error))
   __pyx_t_8 = __pyx_v_self->view.itemsize;
   __pyx_v_info->itemsize = __pyx_t_8;
 
-  /* "View.MemoryView":545
+  /* "View.MemoryView":547
  *         info.ndim = self.view.ndim
  *         info.itemsize = self.view.itemsize
  *         info.len = self.view.len             # <<<<<<<<<<<<<<
  *         info.readonly = self.view.readonly
  *         info.obj = self
  */
-  __Pyx_TraceLine(545,0,__PYX_ERR(2, 545, __pyx_L1_error))
+  __Pyx_TraceLine(547,0,__PYX_ERR(2, 547, __pyx_L1_error))
   __pyx_t_8 = __pyx_v_self->view.len;
   __pyx_v_info->len = __pyx_t_8;
 
-  /* "View.MemoryView":546
+  /* "View.MemoryView":548
  *         info.itemsize = self.view.itemsize
  *         info.len = self.view.len
  *         info.readonly = self.view.readonly             # <<<<<<<<<<<<<<
  *         info.obj = self
  * 
  */
-  __Pyx_TraceLine(546,0,__PYX_ERR(2, 546, __pyx_L1_error))
+  __Pyx_TraceLine(548,0,__PYX_ERR(2, 548, __pyx_L1_error))
   __pyx_t_1 = __pyx_v_self->view.readonly;
   __pyx_v_info->readonly = __pyx_t_1;
 
-  /* "View.MemoryView":547
+  /* "View.MemoryView":549
  *         info.len = self.view.len
  *         info.readonly = self.view.readonly
  *         info.obj = self             # <<<<<<<<<<<<<<
  * 
  *     __pyx_getbuffer = capsule(<void *> &__pyx_memoryview_getbuffer, "getbuffer(obj, view, flags)")
  */
-  __Pyx_TraceLine(547,0,__PYX_ERR(2, 547, __pyx_L1_error))
+  __Pyx_TraceLine(549,0,__PYX_ERR(2, 549, __pyx_L1_error))
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_self));
   __Pyx_GOTREF(__pyx_v_info->obj);
   __Pyx_DECREF(__pyx_v_info->obj);
   __pyx_v_info->obj = ((PyObject *)__pyx_v_self);
 
-  /* "View.MemoryView":518
+  /* "View.MemoryView":520
  * 
  *     @cname('getbuffer')
  *     def __getbuffer__(self, Py_buffer *info, int flags):             # <<<<<<<<<<<<<<
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")
  */
 
@@ -21858,15 +22052,15 @@
   }
   __pyx_L2:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":553
+/* "View.MemoryView":555
  * 
  *     @property
  *     def T(self):             # <<<<<<<<<<<<<<
  *         cdef _memoryviewslice result = memoryview_copy(self)
  *         transpose_memslice(&result.from_slice)
  */
 
@@ -21890,54 +22084,54 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
-  __Pyx_TraceCall("__get__", __pyx_f[2], 553, 0, __PYX_ERR(2, 553, __pyx_L1_error));
+  __Pyx_TraceCall("__get__", __pyx_f[2], 555, 0, __PYX_ERR(2, 555, __pyx_L1_error));
 
-  /* "View.MemoryView":554
+  /* "View.MemoryView":556
  *     @property
  *     def T(self):
  *         cdef _memoryviewslice result = memoryview_copy(self)             # <<<<<<<<<<<<<<
  *         transpose_memslice(&result.from_slice)
  *         return result
  */
-  __Pyx_TraceLine(554,0,__PYX_ERR(2, 554, __pyx_L1_error))
-  __pyx_t_1 = __pyx_memoryview_copy_object(__pyx_v_self); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 554, __pyx_L1_error)
+  __Pyx_TraceLine(556,0,__PYX_ERR(2, 556, __pyx_L1_error))
+  __pyx_t_1 = __pyx_memoryview_copy_object(__pyx_v_self); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 556, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_memoryviewslice_type))))) __PYX_ERR(2, 554, __pyx_L1_error)
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_memoryviewslice_type))))) __PYX_ERR(2, 556, __pyx_L1_error)
   __pyx_v_result = ((struct __pyx_memoryviewslice_obj *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "View.MemoryView":555
+  /* "View.MemoryView":557
  *     def T(self):
  *         cdef _memoryviewslice result = memoryview_copy(self)
  *         transpose_memslice(&result.from_slice)             # <<<<<<<<<<<<<<
  *         return result
  * 
  */
-  __Pyx_TraceLine(555,0,__PYX_ERR(2, 555, __pyx_L1_error))
-  __pyx_t_2 = __pyx_memslice_transpose((&__pyx_v_result->from_slice)); if (unlikely(__pyx_t_2 == ((int)0))) __PYX_ERR(2, 555, __pyx_L1_error)
+  __Pyx_TraceLine(557,0,__PYX_ERR(2, 557, __pyx_L1_error))
+  __pyx_t_2 = __pyx_memslice_transpose((&__pyx_v_result->from_slice)); if (unlikely(__pyx_t_2 == ((int)0))) __PYX_ERR(2, 557, __pyx_L1_error)
 
-  /* "View.MemoryView":556
+  /* "View.MemoryView":558
  *         cdef _memoryviewslice result = memoryview_copy(self)
  *         transpose_memslice(&result.from_slice)
  *         return result             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
-  __Pyx_TraceLine(556,0,__PYX_ERR(2, 556, __pyx_L1_error))
+  __Pyx_TraceLine(558,0,__PYX_ERR(2, 558, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_result));
   __pyx_r = ((PyObject *)__pyx_v_result);
   goto __pyx_L0;
 
-  /* "View.MemoryView":553
+  /* "View.MemoryView":555
  * 
  *     @property
  *     def T(self):             # <<<<<<<<<<<<<<
  *         cdef _memoryviewslice result = memoryview_copy(self)
  *         transpose_memslice(&result.from_slice)
  */
 
@@ -21950,15 +22144,15 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":559
+/* "View.MemoryView":561
  * 
  *     @property
  *     def base(self):             # <<<<<<<<<<<<<<
  *         return self.obj
  * 
  */
 
@@ -21979,30 +22173,30 @@
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
-  __Pyx_TraceCall("__get__", __pyx_f[2], 559, 0, __PYX_ERR(2, 559, __pyx_L1_error));
+  __Pyx_TraceCall("__get__", __pyx_f[2], 561, 0, __PYX_ERR(2, 561, __pyx_L1_error));
 
-  /* "View.MemoryView":560
+  /* "View.MemoryView":562
  *     @property
  *     def base(self):
  *         return self.obj             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
-  __Pyx_TraceLine(560,0,__PYX_ERR(2, 560, __pyx_L1_error))
+  __Pyx_TraceLine(562,0,__PYX_ERR(2, 562, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_self->obj);
   __pyx_r = __pyx_v_self->obj;
   goto __pyx_L0;
 
-  /* "View.MemoryView":559
+  /* "View.MemoryView":561
  * 
  *     @property
  *     def base(self):             # <<<<<<<<<<<<<<
  *         return self.obj
  * 
  */
 
@@ -22013,15 +22207,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":563
+/* "View.MemoryView":565
  * 
  *     @property
  *     def shape(self):             # <<<<<<<<<<<<<<
  *         return tuple([length for length in self.view.shape[:self.view.ndim]])
  * 
  */
 
@@ -22048,44 +22242,44 @@
   Py_ssize_t *__pyx_t_3;
   Py_ssize_t *__pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
-  __Pyx_TraceCall("__get__", __pyx_f[2], 563, 0, __PYX_ERR(2, 563, __pyx_L1_error));
+  __Pyx_TraceCall("__get__", __pyx_f[2], 565, 0, __PYX_ERR(2, 565, __pyx_L1_error));
 
-  /* "View.MemoryView":564
+  /* "View.MemoryView":566
  *     @property
  *     def shape(self):
  *         return tuple([length for length in self.view.shape[:self.view.ndim]])             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
-  __Pyx_TraceLine(564,0,__PYX_ERR(2, 564, __pyx_L1_error))
+  __Pyx_TraceLine(566,0,__PYX_ERR(2, 566, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 564, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 566, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_3 = (__pyx_v_self->view.shape + __pyx_v_self->view.ndim);
   for (__pyx_t_4 = __pyx_v_self->view.shape; __pyx_t_4 < __pyx_t_3; __pyx_t_4++) {
     __pyx_t_2 = __pyx_t_4;
     __pyx_v_length = (__pyx_t_2[0]);
-    __pyx_t_5 = PyInt_FromSsize_t(__pyx_v_length); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 564, __pyx_L1_error)
+    __pyx_t_5 = PyInt_FromSsize_t(__pyx_v_length); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 566, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_5))) __PYX_ERR(2, 564, __pyx_L1_error)
+    if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_5))) __PYX_ERR(2, 566, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
-  __pyx_t_5 = PyList_AsTuple(((PyObject*)__pyx_t_1)); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 564, __pyx_L1_error)
+  __pyx_t_5 = PyList_AsTuple(((PyObject*)__pyx_t_1)); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 566, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_5;
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":563
+  /* "View.MemoryView":565
  * 
  *     @property
  *     def shape(self):             # <<<<<<<<<<<<<<
  *         return tuple([length for length in self.view.shape[:self.view.ndim]])
  * 
  */
 
@@ -22098,15 +22292,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":567
+/* "View.MemoryView":569
  * 
  *     @property
  *     def strides(self):             # <<<<<<<<<<<<<<
  *         if self.view.strides == NULL:
  * 
  */
 
@@ -22134,78 +22328,78 @@
   Py_ssize_t *__pyx_t_4;
   Py_ssize_t *__pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
-  __Pyx_TraceCall("__get__", __pyx_f[2], 567, 0, __PYX_ERR(2, 567, __pyx_L1_error));
+  __Pyx_TraceCall("__get__", __pyx_f[2], 569, 0, __PYX_ERR(2, 569, __pyx_L1_error));
 
-  /* "View.MemoryView":568
+  /* "View.MemoryView":570
  *     @property
  *     def strides(self):
  *         if self.view.strides == NULL:             # <<<<<<<<<<<<<<
  * 
  *             raise ValueError("Buffer view does not expose strides")
  */
-  __Pyx_TraceLine(568,0,__PYX_ERR(2, 568, __pyx_L1_error))
+  __Pyx_TraceLine(570,0,__PYX_ERR(2, 570, __pyx_L1_error))
   __pyx_t_1 = ((__pyx_v_self->view.strides == NULL) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "View.MemoryView":570
+    /* "View.MemoryView":572
  *         if self.view.strides == NULL:
  * 
  *             raise ValueError("Buffer view does not expose strides")             # <<<<<<<<<<<<<<
  * 
  *         return tuple([stride for stride in self.view.strides[:self.view.ndim]])
  */
-    __Pyx_TraceLine(570,0,__PYX_ERR(2, 570, __pyx_L1_error))
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__21, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 570, __pyx_L1_error)
+    __Pyx_TraceLine(572,0,__PYX_ERR(2, 572, __pyx_L1_error))
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__22, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 572, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(2, 570, __pyx_L1_error)
+    __PYX_ERR(2, 572, __pyx_L1_error)
 
-    /* "View.MemoryView":568
+    /* "View.MemoryView":570
  *     @property
  *     def strides(self):
  *         if self.view.strides == NULL:             # <<<<<<<<<<<<<<
  * 
  *             raise ValueError("Buffer view does not expose strides")
  */
   }
 
-  /* "View.MemoryView":572
+  /* "View.MemoryView":574
  *             raise ValueError("Buffer view does not expose strides")
  * 
  *         return tuple([stride for stride in self.view.strides[:self.view.ndim]])             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
-  __Pyx_TraceLine(572,0,__PYX_ERR(2, 572, __pyx_L1_error))
+  __Pyx_TraceLine(574,0,__PYX_ERR(2, 574, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 572, __pyx_L1_error)
+  __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 574, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = (__pyx_v_self->view.strides + __pyx_v_self->view.ndim);
   for (__pyx_t_5 = __pyx_v_self->view.strides; __pyx_t_5 < __pyx_t_4; __pyx_t_5++) {
     __pyx_t_3 = __pyx_t_5;
     __pyx_v_stride = (__pyx_t_3[0]);
-    __pyx_t_6 = PyInt_FromSsize_t(__pyx_v_stride); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 572, __pyx_L1_error)
+    __pyx_t_6 = PyInt_FromSsize_t(__pyx_v_stride); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 574, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_6))) __PYX_ERR(2, 572, __pyx_L1_error)
+    if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_6))) __PYX_ERR(2, 574, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
-  __pyx_t_6 = PyList_AsTuple(((PyObject*)__pyx_t_2)); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 572, __pyx_L1_error)
+  __pyx_t_6 = PyList_AsTuple(((PyObject*)__pyx_t_2)); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 574, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_6;
   __pyx_t_6 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":567
+  /* "View.MemoryView":569
  * 
  *     @property
  *     def strides(self):             # <<<<<<<<<<<<<<
  *         if self.view.strides == NULL:
  * 
  */
 
@@ -22218,15 +22412,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":575
+/* "View.MemoryView":577
  * 
  *     @property
  *     def suboffsets(self):             # <<<<<<<<<<<<<<
  *         if self.view.suboffsets == NULL:
  *             return (-1,) * self.view.ndim
  */
 
@@ -22254,82 +22448,82 @@
   Py_ssize_t *__pyx_t_4;
   Py_ssize_t *__pyx_t_5;
   Py_ssize_t *__pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
-  __Pyx_TraceCall("__get__", __pyx_f[2], 575, 0, __PYX_ERR(2, 575, __pyx_L1_error));
+  __Pyx_TraceCall("__get__", __pyx_f[2], 577, 0, __PYX_ERR(2, 577, __pyx_L1_error));
 
-  /* "View.MemoryView":576
+  /* "View.MemoryView":578
  *     @property
  *     def suboffsets(self):
  *         if self.view.suboffsets == NULL:             # <<<<<<<<<<<<<<
  *             return (-1,) * self.view.ndim
  * 
  */
-  __Pyx_TraceLine(576,0,__PYX_ERR(2, 576, __pyx_L1_error))
+  __Pyx_TraceLine(578,0,__PYX_ERR(2, 578, __pyx_L1_error))
   __pyx_t_1 = ((__pyx_v_self->view.suboffsets == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":577
+    /* "View.MemoryView":579
  *     def suboffsets(self):
  *         if self.view.suboffsets == NULL:
  *             return (-1,) * self.view.ndim             # <<<<<<<<<<<<<<
  * 
  *         return tuple([suboffset for suboffset in self.view.suboffsets[:self.view.ndim]])
  */
-    __Pyx_TraceLine(577,0,__PYX_ERR(2, 577, __pyx_L1_error))
+    __Pyx_TraceLine(579,0,__PYX_ERR(2, 579, __pyx_L1_error))
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->view.ndim); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 577, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->view.ndim); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 579, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PyNumber_Multiply(__pyx_tuple__22, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 577, __pyx_L1_error)
+    __pyx_t_3 = PyNumber_Multiply(__pyx_tuple__23, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 579, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "View.MemoryView":576
+    /* "View.MemoryView":578
  *     @property
  *     def suboffsets(self):
  *         if self.view.suboffsets == NULL:             # <<<<<<<<<<<<<<
  *             return (-1,) * self.view.ndim
  * 
  */
   }
 
-  /* "View.MemoryView":579
+  /* "View.MemoryView":581
  *             return (-1,) * self.view.ndim
  * 
  *         return tuple([suboffset for suboffset in self.view.suboffsets[:self.view.ndim]])             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
-  __Pyx_TraceLine(579,0,__PYX_ERR(2, 579, __pyx_L1_error))
+  __Pyx_TraceLine(581,0,__PYX_ERR(2, 581, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 579, __pyx_L1_error)
+  __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 581, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_5 = (__pyx_v_self->view.suboffsets + __pyx_v_self->view.ndim);
   for (__pyx_t_6 = __pyx_v_self->view.suboffsets; __pyx_t_6 < __pyx_t_5; __pyx_t_6++) {
     __pyx_t_4 = __pyx_t_6;
     __pyx_v_suboffset = (__pyx_t_4[0]);
-    __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_suboffset); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 579, __pyx_L1_error)
+    __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_suboffset); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 581, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    if (unlikely(__Pyx_ListComp_Append(__pyx_t_3, (PyObject*)__pyx_t_2))) __PYX_ERR(2, 579, __pyx_L1_error)
+    if (unlikely(__Pyx_ListComp_Append(__pyx_t_3, (PyObject*)__pyx_t_2))) __PYX_ERR(2, 581, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
-  __pyx_t_2 = PyList_AsTuple(((PyObject*)__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 579, __pyx_L1_error)
+  __pyx_t_2 = PyList_AsTuple(((PyObject*)__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 581, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":575
+  /* "View.MemoryView":577
  * 
  *     @property
  *     def suboffsets(self):             # <<<<<<<<<<<<<<
  *         if self.view.suboffsets == NULL:
  *             return (-1,) * self.view.ndim
  */
 
@@ -22342,15 +22536,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":582
+/* "View.MemoryView":584
  * 
  *     @property
  *     def ndim(self):             # <<<<<<<<<<<<<<
  *         return self.view.ndim
  * 
  */
 
@@ -22372,32 +22566,32 @@
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
-  __Pyx_TraceCall("__get__", __pyx_f[2], 582, 0, __PYX_ERR(2, 582, __pyx_L1_error));
+  __Pyx_TraceCall("__get__", __pyx_f[2], 584, 0, __PYX_ERR(2, 584, __pyx_L1_error));
 
-  /* "View.MemoryView":583
+  /* "View.MemoryView":585
  *     @property
  *     def ndim(self):
  *         return self.view.ndim             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
-  __Pyx_TraceLine(583,0,__PYX_ERR(2, 583, __pyx_L1_error))
+  __Pyx_TraceLine(585,0,__PYX_ERR(2, 585, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->view.ndim); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 583, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->view.ndim); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 585, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":582
+  /* "View.MemoryView":584
  * 
  *     @property
  *     def ndim(self):             # <<<<<<<<<<<<<<
  *         return self.view.ndim
  * 
  */
 
@@ -22409,15 +22603,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":586
+/* "View.MemoryView":588
  * 
  *     @property
  *     def itemsize(self):             # <<<<<<<<<<<<<<
  *         return self.view.itemsize
  * 
  */
 
@@ -22439,32 +22633,32 @@
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
-  __Pyx_TraceCall("__get__", __pyx_f[2], 586, 0, __PYX_ERR(2, 586, __pyx_L1_error));
+  __Pyx_TraceCall("__get__", __pyx_f[2], 588, 0, __PYX_ERR(2, 588, __pyx_L1_error));
 
-  /* "View.MemoryView":587
+  /* "View.MemoryView":589
  *     @property
  *     def itemsize(self):
  *         return self.view.itemsize             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
-  __Pyx_TraceLine(587,0,__PYX_ERR(2, 587, __pyx_L1_error))
+  __Pyx_TraceLine(589,0,__PYX_ERR(2, 589, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyInt_FromSsize_t(__pyx_v_self->view.itemsize); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 587, __pyx_L1_error)
+  __pyx_t_1 = PyInt_FromSsize_t(__pyx_v_self->view.itemsize); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 589, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":586
+  /* "View.MemoryView":588
  * 
  *     @property
  *     def itemsize(self):             # <<<<<<<<<<<<<<
  *         return self.view.itemsize
  * 
  */
 
@@ -22476,15 +22670,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":590
+/* "View.MemoryView":592
  * 
  *     @property
  *     def nbytes(self):             # <<<<<<<<<<<<<<
  *         return self.size * self.view.itemsize
  * 
  */
 
@@ -22508,38 +22702,38 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
-  __Pyx_TraceCall("__get__", __pyx_f[2], 590, 0, __PYX_ERR(2, 590, __pyx_L1_error));
+  __Pyx_TraceCall("__get__", __pyx_f[2], 592, 0, __PYX_ERR(2, 592, __pyx_L1_error));
 
-  /* "View.MemoryView":591
+  /* "View.MemoryView":593
  *     @property
  *     def nbytes(self):
  *         return self.size * self.view.itemsize             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
-  __Pyx_TraceLine(591,0,__PYX_ERR(2, 591, __pyx_L1_error))
+  __Pyx_TraceLine(593,0,__PYX_ERR(2, 593, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 591, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 593, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_self->view.itemsize); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 591, __pyx_L1_error)
+  __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_self->view.itemsize); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 593, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyNumber_Multiply(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 591, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Multiply(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 593, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":590
+  /* "View.MemoryView":592
  * 
  *     @property
  *     def nbytes(self):             # <<<<<<<<<<<<<<
  *         return self.size * self.view.itemsize
  * 
  */
 
@@ -22553,15 +22747,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":594
+/* "View.MemoryView":596
  * 
  *     @property
  *     def size(self):             # <<<<<<<<<<<<<<
  *         if self._size is None:
  *             result = 1
  */
 
@@ -22590,106 +22784,106 @@
   Py_ssize_t *__pyx_t_4;
   Py_ssize_t *__pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
-  __Pyx_TraceCall("__get__", __pyx_f[2], 594, 0, __PYX_ERR(2, 594, __pyx_L1_error));
+  __Pyx_TraceCall("__get__", __pyx_f[2], 596, 0, __PYX_ERR(2, 596, __pyx_L1_error));
 
-  /* "View.MemoryView":595
+  /* "View.MemoryView":597
  *     @property
  *     def size(self):
  *         if self._size is None:             # <<<<<<<<<<<<<<
  *             result = 1
  * 
  */
-  __Pyx_TraceLine(595,0,__PYX_ERR(2, 595, __pyx_L1_error))
+  __Pyx_TraceLine(597,0,__PYX_ERR(2, 597, __pyx_L1_error))
   __pyx_t_1 = (__pyx_v_self->_size == Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":596
+    /* "View.MemoryView":598
  *     def size(self):
  *         if self._size is None:
  *             result = 1             # <<<<<<<<<<<<<<
  * 
  *             for length in self.view.shape[:self.view.ndim]:
  */
-    __Pyx_TraceLine(596,0,__PYX_ERR(2, 596, __pyx_L1_error))
+    __Pyx_TraceLine(598,0,__PYX_ERR(2, 598, __pyx_L1_error))
     __Pyx_INCREF(__pyx_int_1);
     __pyx_v_result = __pyx_int_1;
 
-    /* "View.MemoryView":598
+    /* "View.MemoryView":600
  *             result = 1
  * 
  *             for length in self.view.shape[:self.view.ndim]:             # <<<<<<<<<<<<<<
  *                 result *= length
  * 
  */
-    __Pyx_TraceLine(598,0,__PYX_ERR(2, 598, __pyx_L1_error))
+    __Pyx_TraceLine(600,0,__PYX_ERR(2, 600, __pyx_L1_error))
     __pyx_t_4 = (__pyx_v_self->view.shape + __pyx_v_self->view.ndim);
     for (__pyx_t_5 = __pyx_v_self->view.shape; __pyx_t_5 < __pyx_t_4; __pyx_t_5++) {
       __pyx_t_3 = __pyx_t_5;
-      __pyx_t_6 = PyInt_FromSsize_t((__pyx_t_3[0])); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 598, __pyx_L1_error)
+      __pyx_t_6 = PyInt_FromSsize_t((__pyx_t_3[0])); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 600, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_XDECREF_SET(__pyx_v_length, __pyx_t_6);
       __pyx_t_6 = 0;
 
-      /* "View.MemoryView":599
+      /* "View.MemoryView":601
  * 
  *             for length in self.view.shape[:self.view.ndim]:
  *                 result *= length             # <<<<<<<<<<<<<<
  * 
  *             self._size = result
  */
-      __Pyx_TraceLine(599,0,__PYX_ERR(2, 599, __pyx_L1_error))
-      __pyx_t_6 = PyNumber_InPlaceMultiply(__pyx_v_result, __pyx_v_length); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 599, __pyx_L1_error)
+      __Pyx_TraceLine(601,0,__PYX_ERR(2, 601, __pyx_L1_error))
+      __pyx_t_6 = PyNumber_InPlaceMultiply(__pyx_v_result, __pyx_v_length); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 601, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF_SET(__pyx_v_result, __pyx_t_6);
       __pyx_t_6 = 0;
     }
 
-    /* "View.MemoryView":601
+    /* "View.MemoryView":603
  *                 result *= length
  * 
  *             self._size = result             # <<<<<<<<<<<<<<
  * 
  *         return self._size
  */
-    __Pyx_TraceLine(601,0,__PYX_ERR(2, 601, __pyx_L1_error))
+    __Pyx_TraceLine(603,0,__PYX_ERR(2, 603, __pyx_L1_error))
     __Pyx_INCREF(__pyx_v_result);
     __Pyx_GIVEREF(__pyx_v_result);
     __Pyx_GOTREF(__pyx_v_self->_size);
     __Pyx_DECREF(__pyx_v_self->_size);
     __pyx_v_self->_size = __pyx_v_result;
 
-    /* "View.MemoryView":595
+    /* "View.MemoryView":597
  *     @property
  *     def size(self):
  *         if self._size is None:             # <<<<<<<<<<<<<<
  *             result = 1
  * 
  */
   }
 
-  /* "View.MemoryView":603
+  /* "View.MemoryView":605
  *             self._size = result
  * 
  *         return self._size             # <<<<<<<<<<<<<<
  * 
  *     def __len__(self):
  */
-  __Pyx_TraceLine(603,0,__PYX_ERR(2, 603, __pyx_L1_error))
+  __Pyx_TraceLine(605,0,__PYX_ERR(2, 605, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_self->_size);
   __pyx_r = __pyx_v_self->_size;
   goto __pyx_L0;
 
-  /* "View.MemoryView":594
+  /* "View.MemoryView":596
  * 
  *     @property
  *     def size(self):             # <<<<<<<<<<<<<<
  *         if self._size is None:
  *             result = 1
  */
 
@@ -22703,15 +22897,15 @@
   __Pyx_XDECREF(__pyx_v_length);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":605
+/* "View.MemoryView":607
  *         return self._size
  * 
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         if self.view.ndim >= 1:
  *             return self.view.shape[0]
  */
 
@@ -22733,59 +22927,59 @@
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__len__", 0);
-  __Pyx_TraceCall("__len__", __pyx_f[2], 605, 0, __PYX_ERR(2, 605, __pyx_L1_error));
+  __Pyx_TraceCall("__len__", __pyx_f[2], 607, 0, __PYX_ERR(2, 607, __pyx_L1_error));
 
-  /* "View.MemoryView":606
+  /* "View.MemoryView":608
  * 
  *     def __len__(self):
  *         if self.view.ndim >= 1:             # <<<<<<<<<<<<<<
  *             return self.view.shape[0]
  * 
  */
-  __Pyx_TraceLine(606,0,__PYX_ERR(2, 606, __pyx_L1_error))
+  __Pyx_TraceLine(608,0,__PYX_ERR(2, 608, __pyx_L1_error))
   __pyx_t_1 = ((__pyx_v_self->view.ndim >= 1) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":607
+    /* "View.MemoryView":609
  *     def __len__(self):
  *         if self.view.ndim >= 1:
  *             return self.view.shape[0]             # <<<<<<<<<<<<<<
  * 
  *         return 0
  */
-    __Pyx_TraceLine(607,0,__PYX_ERR(2, 607, __pyx_L1_error))
+    __Pyx_TraceLine(609,0,__PYX_ERR(2, 609, __pyx_L1_error))
     __pyx_r = (__pyx_v_self->view.shape[0]);
     goto __pyx_L0;
 
-    /* "View.MemoryView":606
+    /* "View.MemoryView":608
  * 
  *     def __len__(self):
  *         if self.view.ndim >= 1:             # <<<<<<<<<<<<<<
  *             return self.view.shape[0]
  * 
  */
   }
 
-  /* "View.MemoryView":609
+  /* "View.MemoryView":611
  *             return self.view.shape[0]
  * 
  *         return 0             # <<<<<<<<<<<<<<
  * 
  *     def __repr__(self):
  */
-  __Pyx_TraceLine(609,0,__PYX_ERR(2, 609, __pyx_L1_error))
+  __Pyx_TraceLine(611,0,__PYX_ERR(2, 611, __pyx_L1_error))
   __pyx_r = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":605
+  /* "View.MemoryView":607
  *         return self._size
  * 
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         if self.view.ndim >= 1:
  *             return self.view.shape[0]
  */
 
@@ -22795,15 +22989,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":611
+/* "View.MemoryView":613
  *         return 0
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return "<MemoryView of %r at 0x%x>" % (self.base.__class__.__name__,
  *                                                id(self))
  */
 
@@ -22827,69 +23021,69 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__repr__", 0);
-  __Pyx_TraceCall("__repr__", __pyx_f[2], 611, 0, __PYX_ERR(2, 611, __pyx_L1_error));
+  __Pyx_TraceCall("__repr__", __pyx_f[2], 613, 0, __PYX_ERR(2, 613, __pyx_L1_error));
 
-  /* "View.MemoryView":612
+  /* "View.MemoryView":614
  * 
  *     def __repr__(self):
  *         return "<MemoryView of %r at 0x%x>" % (self.base.__class__.__name__,             # <<<<<<<<<<<<<<
  *                                                id(self))
  * 
  */
-  __Pyx_TraceLine(612,0,__PYX_ERR(2, 612, __pyx_L1_error))
+  __Pyx_TraceLine(614,0,__PYX_ERR(2, 614, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_base); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 612, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_base); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 614, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_class); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 612, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_class); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 614, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_name_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 612, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_name_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 614, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "View.MemoryView":613
+  /* "View.MemoryView":615
  *     def __repr__(self):
  *         return "<MemoryView of %r at 0x%x>" % (self.base.__class__.__name__,
  *                                                id(self))             # <<<<<<<<<<<<<<
  * 
  *     def __str__(self):
  */
-  __Pyx_TraceLine(613,0,__PYX_ERR(2, 613, __pyx_L1_error))
-  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_id, ((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 613, __pyx_L1_error)
+  __Pyx_TraceLine(615,0,__PYX_ERR(2, 615, __pyx_L1_error))
+  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_id, ((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 615, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
 
-  /* "View.MemoryView":612
+  /* "View.MemoryView":614
  * 
  *     def __repr__(self):
  *         return "<MemoryView of %r at 0x%x>" % (self.base.__class__.__name__,             # <<<<<<<<<<<<<<
  *                                                id(self))
  * 
  */
-  __Pyx_TraceLine(612,0,__PYX_ERR(2, 612, __pyx_L1_error))
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 612, __pyx_L1_error)
+  __Pyx_TraceLine(614,0,__PYX_ERR(2, 614, __pyx_L1_error))
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 614, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_2);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyString_Format(__pyx_kp_s_MemoryView_of_r_at_0x_x, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 612, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyString_Format(__pyx_kp_s_MemoryView_of_r_at_0x_x, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 614, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":611
+  /* "View.MemoryView":613
  *         return 0
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return "<MemoryView of %r at 0x%x>" % (self.base.__class__.__name__,
  *                                                id(self))
  */
 
@@ -22903,15 +23097,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":615
+/* "View.MemoryView":617
  *                                                id(self))
  * 
  *     def __str__(self):             # <<<<<<<<<<<<<<
  *         return "<MemoryView of %r object>" % (self.base.__class__.__name__,)
  * 
  */
 
@@ -22934,46 +23128,46 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__str__", 0);
-  __Pyx_TraceCall("__str__", __pyx_f[2], 615, 0, __PYX_ERR(2, 615, __pyx_L1_error));
+  __Pyx_TraceCall("__str__", __pyx_f[2], 617, 0, __PYX_ERR(2, 617, __pyx_L1_error));
 
-  /* "View.MemoryView":616
+  /* "View.MemoryView":618
  * 
  *     def __str__(self):
  *         return "<MemoryView of %r object>" % (self.base.__class__.__name__,)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_TraceLine(616,0,__PYX_ERR(2, 616, __pyx_L1_error))
+  __Pyx_TraceLine(618,0,__PYX_ERR(2, 618, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_base); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 616, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_base); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 618, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_class); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 616, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_class); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 618, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_name_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 616, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_name_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 618, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 616, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 618, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyString_Format(__pyx_kp_s_MemoryView_of_r_object, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 616, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyString_Format(__pyx_kp_s_MemoryView_of_r_object, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 618, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":615
+  /* "View.MemoryView":617
  *                                                id(self))
  * 
  *     def __str__(self):             # <<<<<<<<<<<<<<
  *         return "<MemoryView of %r object>" % (self.base.__class__.__name__,)
  * 
  */
 
@@ -22986,15 +23180,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":619
+/* "View.MemoryView":621
  * 
  * 
  *     def is_c_contig(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice *mslice
  *         cdef __Pyx_memviewslice tmp
  */
 
@@ -23019,43 +23213,43 @@
   __Pyx_RefNannyDeclarations
   __Pyx_memviewslice *__pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_c_contig", 0);
-  __Pyx_TraceCall("is_c_contig", __pyx_f[2], 619, 0, __PYX_ERR(2, 619, __pyx_L1_error));
+  __Pyx_TraceCall("is_c_contig", __pyx_f[2], 621, 0, __PYX_ERR(2, 621, __pyx_L1_error));
 
-  /* "View.MemoryView":622
+  /* "View.MemoryView":624
  *         cdef __Pyx_memviewslice *mslice
  *         cdef __Pyx_memviewslice tmp
  *         mslice = get_slice_from_memview(self, &tmp)             # <<<<<<<<<<<<<<
  *         return slice_is_contig(mslice[0], 'C', self.view.ndim)
  * 
  */
-  __Pyx_TraceLine(622,0,__PYX_ERR(2, 622, __pyx_L1_error))
-  __pyx_t_1 = __pyx_memoryview_get_slice_from_memoryview(__pyx_v_self, (&__pyx_v_tmp)); if (unlikely(__pyx_t_1 == ((__Pyx_memviewslice *)NULL))) __PYX_ERR(2, 622, __pyx_L1_error)
+  __Pyx_TraceLine(624,0,__PYX_ERR(2, 624, __pyx_L1_error))
+  __pyx_t_1 = __pyx_memoryview_get_slice_from_memoryview(__pyx_v_self, (&__pyx_v_tmp)); if (unlikely(__pyx_t_1 == ((__Pyx_memviewslice *)NULL))) __PYX_ERR(2, 624, __pyx_L1_error)
   __pyx_v_mslice = __pyx_t_1;
 
-  /* "View.MemoryView":623
+  /* "View.MemoryView":625
  *         cdef __Pyx_memviewslice tmp
  *         mslice = get_slice_from_memview(self, &tmp)
  *         return slice_is_contig(mslice[0], 'C', self.view.ndim)             # <<<<<<<<<<<<<<
  * 
  *     def is_f_contig(self):
  */
-  __Pyx_TraceLine(623,0,__PYX_ERR(2, 623, __pyx_L1_error))
+  __Pyx_TraceLine(625,0,__PYX_ERR(2, 625, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_memviewslice_is_contig((__pyx_v_mslice[0]), 'C', __pyx_v_self->view.ndim)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 623, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_memviewslice_is_contig((__pyx_v_mslice[0]), 'C', __pyx_v_self->view.ndim)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 625, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":619
+  /* "View.MemoryView":621
  * 
  * 
  *     def is_c_contig(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice *mslice
  *         cdef __Pyx_memviewslice tmp
  */
 
@@ -23067,15 +23261,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":625
+/* "View.MemoryView":627
  *         return slice_is_contig(mslice[0], 'C', self.view.ndim)
  * 
  *     def is_f_contig(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice *mslice
  *         cdef __Pyx_memviewslice tmp
  */
 
@@ -23100,43 +23294,43 @@
   __Pyx_RefNannyDeclarations
   __Pyx_memviewslice *__pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_f_contig", 0);
-  __Pyx_TraceCall("is_f_contig", __pyx_f[2], 625, 0, __PYX_ERR(2, 625, __pyx_L1_error));
+  __Pyx_TraceCall("is_f_contig", __pyx_f[2], 627, 0, __PYX_ERR(2, 627, __pyx_L1_error));
 
-  /* "View.MemoryView":628
+  /* "View.MemoryView":630
  *         cdef __Pyx_memviewslice *mslice
  *         cdef __Pyx_memviewslice tmp
  *         mslice = get_slice_from_memview(self, &tmp)             # <<<<<<<<<<<<<<
  *         return slice_is_contig(mslice[0], 'F', self.view.ndim)
  * 
  */
-  __Pyx_TraceLine(628,0,__PYX_ERR(2, 628, __pyx_L1_error))
-  __pyx_t_1 = __pyx_memoryview_get_slice_from_memoryview(__pyx_v_self, (&__pyx_v_tmp)); if (unlikely(__pyx_t_1 == ((__Pyx_memviewslice *)NULL))) __PYX_ERR(2, 628, __pyx_L1_error)
+  __Pyx_TraceLine(630,0,__PYX_ERR(2, 630, __pyx_L1_error))
+  __pyx_t_1 = __pyx_memoryview_get_slice_from_memoryview(__pyx_v_self, (&__pyx_v_tmp)); if (unlikely(__pyx_t_1 == ((__Pyx_memviewslice *)NULL))) __PYX_ERR(2, 630, __pyx_L1_error)
   __pyx_v_mslice = __pyx_t_1;
 
-  /* "View.MemoryView":629
+  /* "View.MemoryView":631
  *         cdef __Pyx_memviewslice tmp
  *         mslice = get_slice_from_memview(self, &tmp)
  *         return slice_is_contig(mslice[0], 'F', self.view.ndim)             # <<<<<<<<<<<<<<
  * 
  *     def copy(self):
  */
-  __Pyx_TraceLine(629,0,__PYX_ERR(2, 629, __pyx_L1_error))
+  __Pyx_TraceLine(631,0,__PYX_ERR(2, 631, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_memviewslice_is_contig((__pyx_v_mslice[0]), 'F', __pyx_v_self->view.ndim)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 629, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_memviewslice_is_contig((__pyx_v_mslice[0]), 'F', __pyx_v_self->view.ndim)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 631, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":625
+  /* "View.MemoryView":627
  *         return slice_is_contig(mslice[0], 'C', self.view.ndim)
  * 
  *     def is_f_contig(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice *mslice
  *         cdef __Pyx_memviewslice tmp
  */
 
@@ -23148,15 +23342,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":631
+/* "View.MemoryView":633
  *         return slice_is_contig(mslice[0], 'F', self.view.ndim)
  * 
  *     def copy(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice mslice
  *         cdef int flags = self.flags & ~PyBUF_F_CONTIGUOUS
  */
 
@@ -23181,63 +23375,63 @@
   __Pyx_RefNannyDeclarations
   __Pyx_memviewslice __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("copy", 0);
-  __Pyx_TraceCall("copy", __pyx_f[2], 631, 0, __PYX_ERR(2, 631, __pyx_L1_error));
+  __Pyx_TraceCall("copy", __pyx_f[2], 633, 0, __PYX_ERR(2, 633, __pyx_L1_error));
 
-  /* "View.MemoryView":633
+  /* "View.MemoryView":635
  *     def copy(self):
  *         cdef __Pyx_memviewslice mslice
  *         cdef int flags = self.flags & ~PyBUF_F_CONTIGUOUS             # <<<<<<<<<<<<<<
  * 
  *         slice_copy(self, &mslice)
  */
-  __Pyx_TraceLine(633,0,__PYX_ERR(2, 633, __pyx_L1_error))
+  __Pyx_TraceLine(635,0,__PYX_ERR(2, 635, __pyx_L1_error))
   __pyx_v_flags = (__pyx_v_self->flags & (~PyBUF_F_CONTIGUOUS));
 
-  /* "View.MemoryView":635
+  /* "View.MemoryView":637
  *         cdef int flags = self.flags & ~PyBUF_F_CONTIGUOUS
  * 
  *         slice_copy(self, &mslice)             # <<<<<<<<<<<<<<
  *         mslice = slice_copy_contig(&mslice, "c", self.view.ndim,
  *                                    self.view.itemsize,
  */
-  __Pyx_TraceLine(635,0,__PYX_ERR(2, 635, __pyx_L1_error))
+  __Pyx_TraceLine(637,0,__PYX_ERR(2, 637, __pyx_L1_error))
   __pyx_memoryview_slice_copy(__pyx_v_self, (&__pyx_v_mslice));
 
-  /* "View.MemoryView":636
+  /* "View.MemoryView":638
  * 
  *         slice_copy(self, &mslice)
  *         mslice = slice_copy_contig(&mslice, "c", self.view.ndim,             # <<<<<<<<<<<<<<
  *                                    self.view.itemsize,
  *                                    flags|PyBUF_C_CONTIGUOUS,
  */
-  __Pyx_TraceLine(636,0,__PYX_ERR(2, 636, __pyx_L1_error))
-  __pyx_t_1 = __pyx_memoryview_copy_new_contig((&__pyx_v_mslice), ((char *)"c"), __pyx_v_self->view.ndim, __pyx_v_self->view.itemsize, (__pyx_v_flags | PyBUF_C_CONTIGUOUS), __pyx_v_self->dtype_is_object); if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 636, __pyx_L1_error)
+  __Pyx_TraceLine(638,0,__PYX_ERR(2, 638, __pyx_L1_error))
+  __pyx_t_1 = __pyx_memoryview_copy_new_contig((&__pyx_v_mslice), ((char *)"c"), __pyx_v_self->view.ndim, __pyx_v_self->view.itemsize, (__pyx_v_flags | PyBUF_C_CONTIGUOUS), __pyx_v_self->dtype_is_object); if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 638, __pyx_L1_error)
   __pyx_v_mslice = __pyx_t_1;
 
-  /* "View.MemoryView":641
+  /* "View.MemoryView":643
  *                                    self.dtype_is_object)
  * 
  *         return memoryview_copy_from_slice(self, &mslice)             # <<<<<<<<<<<<<<
  * 
  *     def copy_fortran(self):
  */
-  __Pyx_TraceLine(641,0,__PYX_ERR(2, 641, __pyx_L1_error))
+  __Pyx_TraceLine(643,0,__PYX_ERR(2, 643, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __pyx_memoryview_copy_object_from_slice(__pyx_v_self, (&__pyx_v_mslice)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 641, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memoryview_copy_object_from_slice(__pyx_v_self, (&__pyx_v_mslice)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 643, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":631
+  /* "View.MemoryView":633
  *         return slice_is_contig(mslice[0], 'F', self.view.ndim)
  * 
  *     def copy(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice mslice
  *         cdef int flags = self.flags & ~PyBUF_F_CONTIGUOUS
  */
 
@@ -23249,15 +23443,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":643
+/* "View.MemoryView":645
  *         return memoryview_copy_from_slice(self, &mslice)
  * 
  *     def copy_fortran(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice src, dst
  *         cdef int flags = self.flags & ~PyBUF_C_CONTIGUOUS
  */
 
@@ -23283,63 +23477,63 @@
   __Pyx_RefNannyDeclarations
   __Pyx_memviewslice __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("copy_fortran", 0);
-  __Pyx_TraceCall("copy_fortran", __pyx_f[2], 643, 0, __PYX_ERR(2, 643, __pyx_L1_error));
+  __Pyx_TraceCall("copy_fortran", __pyx_f[2], 645, 0, __PYX_ERR(2, 645, __pyx_L1_error));
 
-  /* "View.MemoryView":645
+  /* "View.MemoryView":647
  *     def copy_fortran(self):
  *         cdef __Pyx_memviewslice src, dst
  *         cdef int flags = self.flags & ~PyBUF_C_CONTIGUOUS             # <<<<<<<<<<<<<<
  * 
  *         slice_copy(self, &src)
  */
-  __Pyx_TraceLine(645,0,__PYX_ERR(2, 645, __pyx_L1_error))
+  __Pyx_TraceLine(647,0,__PYX_ERR(2, 647, __pyx_L1_error))
   __pyx_v_flags = (__pyx_v_self->flags & (~PyBUF_C_CONTIGUOUS));
 
-  /* "View.MemoryView":647
+  /* "View.MemoryView":649
  *         cdef int flags = self.flags & ~PyBUF_C_CONTIGUOUS
  * 
  *         slice_copy(self, &src)             # <<<<<<<<<<<<<<
  *         dst = slice_copy_contig(&src, "fortran", self.view.ndim,
  *                                 self.view.itemsize,
  */
-  __Pyx_TraceLine(647,0,__PYX_ERR(2, 647, __pyx_L1_error))
+  __Pyx_TraceLine(649,0,__PYX_ERR(2, 649, __pyx_L1_error))
   __pyx_memoryview_slice_copy(__pyx_v_self, (&__pyx_v_src));
 
-  /* "View.MemoryView":648
+  /* "View.MemoryView":650
  * 
  *         slice_copy(self, &src)
  *         dst = slice_copy_contig(&src, "fortran", self.view.ndim,             # <<<<<<<<<<<<<<
  *                                 self.view.itemsize,
  *                                 flags|PyBUF_F_CONTIGUOUS,
  */
-  __Pyx_TraceLine(648,0,__PYX_ERR(2, 648, __pyx_L1_error))
-  __pyx_t_1 = __pyx_memoryview_copy_new_contig((&__pyx_v_src), ((char *)"fortran"), __pyx_v_self->view.ndim, __pyx_v_self->view.itemsize, (__pyx_v_flags | PyBUF_F_CONTIGUOUS), __pyx_v_self->dtype_is_object); if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 648, __pyx_L1_error)
+  __Pyx_TraceLine(650,0,__PYX_ERR(2, 650, __pyx_L1_error))
+  __pyx_t_1 = __pyx_memoryview_copy_new_contig((&__pyx_v_src), ((char *)"fortran"), __pyx_v_self->view.ndim, __pyx_v_self->view.itemsize, (__pyx_v_flags | PyBUF_F_CONTIGUOUS), __pyx_v_self->dtype_is_object); if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 650, __pyx_L1_error)
   __pyx_v_dst = __pyx_t_1;
 
-  /* "View.MemoryView":653
+  /* "View.MemoryView":655
  *                                 self.dtype_is_object)
  * 
  *         return memoryview_copy_from_slice(self, &dst)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_TraceLine(653,0,__PYX_ERR(2, 653, __pyx_L1_error))
+  __Pyx_TraceLine(655,0,__PYX_ERR(2, 655, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __pyx_memoryview_copy_object_from_slice(__pyx_v_self, (&__pyx_v_dst)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 653, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memoryview_copy_object_from_slice(__pyx_v_self, (&__pyx_v_dst)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 655, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":643
+  /* "View.MemoryView":645
  *         return memoryview_copy_from_slice(self, &mslice)
  * 
  *     def copy_fortran(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice src, dst
  *         cdef int flags = self.flags & ~PyBUF_C_CONTIGUOUS
  */
 
@@ -23388,15 +23582,15 @@
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
   __Pyx_TraceLine(2,0,__PYX_ERR(2, 2, __pyx_L1_error))
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__23, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__24, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(2, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
@@ -23448,15 +23642,15 @@
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __Pyx_TraceLine(4,0,__PYX_ERR(2, 4, __pyx_L1_error))
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__24, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__25, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(2, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
@@ -23472,15 +23666,15 @@
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":657
+/* "View.MemoryView":659
  * 
  * @cname('__pyx_memoryview_new')
  * cdef memoryview_cwrapper(object o, int flags, bint dtype_is_object, __Pyx_TypeInfo *typeinfo):             # <<<<<<<<<<<<<<
  *     cdef memoryview result = memoryview(o, flags, dtype_is_object)
  *     result.typeinfo = typeinfo
  */
 
@@ -23492,69 +23686,69 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("memoryview_cwrapper", 0);
-  __Pyx_TraceCall("memoryview_cwrapper", __pyx_f[2], 657, 0, __PYX_ERR(2, 657, __pyx_L1_error));
+  __Pyx_TraceCall("memoryview_cwrapper", __pyx_f[2], 659, 0, __PYX_ERR(2, 659, __pyx_L1_error));
 
-  /* "View.MemoryView":658
+  /* "View.MemoryView":660
  * @cname('__pyx_memoryview_new')
  * cdef memoryview_cwrapper(object o, int flags, bint dtype_is_object, __Pyx_TypeInfo *typeinfo):
  *     cdef memoryview result = memoryview(o, flags, dtype_is_object)             # <<<<<<<<<<<<<<
  *     result.typeinfo = typeinfo
  *     return result
  */
-  __Pyx_TraceLine(658,0,__PYX_ERR(2, 658, __pyx_L1_error))
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_flags); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 658, __pyx_L1_error)
+  __Pyx_TraceLine(660,0,__PYX_ERR(2, 660, __pyx_L1_error))
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_flags); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 660, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_v_dtype_is_object); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 658, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_v_dtype_is_object); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 660, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 658, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 660, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_v_o);
   __Pyx_GIVEREF(__pyx_v_o);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_o);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_t_2);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_memoryview_type), __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 658, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_memoryview_type), __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 660, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_result = ((struct __pyx_memoryview_obj *)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "View.MemoryView":659
+  /* "View.MemoryView":661
  * cdef memoryview_cwrapper(object o, int flags, bint dtype_is_object, __Pyx_TypeInfo *typeinfo):
  *     cdef memoryview result = memoryview(o, flags, dtype_is_object)
  *     result.typeinfo = typeinfo             # <<<<<<<<<<<<<<
  *     return result
  * 
  */
-  __Pyx_TraceLine(659,0,__PYX_ERR(2, 659, __pyx_L1_error))
+  __Pyx_TraceLine(661,0,__PYX_ERR(2, 661, __pyx_L1_error))
   __pyx_v_result->typeinfo = __pyx_v_typeinfo;
 
-  /* "View.MemoryView":660
+  /* "View.MemoryView":662
  *     cdef memoryview result = memoryview(o, flags, dtype_is_object)
  *     result.typeinfo = typeinfo
  *     return result             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_check')
  */
-  __Pyx_TraceLine(660,0,__PYX_ERR(2, 660, __pyx_L1_error))
+  __Pyx_TraceLine(662,0,__PYX_ERR(2, 662, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_result));
   __pyx_r = ((PyObject *)__pyx_v_result);
   goto __pyx_L0;
 
-  /* "View.MemoryView":657
+  /* "View.MemoryView":659
  * 
  * @cname('__pyx_memoryview_new')
  * cdef memoryview_cwrapper(object o, int flags, bint dtype_is_object, __Pyx_TypeInfo *typeinfo):             # <<<<<<<<<<<<<<
  *     cdef memoryview result = memoryview(o, flags, dtype_is_object)
  *     result.typeinfo = typeinfo
  */
 
@@ -23569,15 +23763,15 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":663
+/* "View.MemoryView":665
  * 
  * @cname('__pyx_memoryview_check')
  * cdef inline bint memoryview_check(object o):             # <<<<<<<<<<<<<<
  *     return isinstance(o, memoryview)
  * 
  */
 
@@ -23586,29 +23780,29 @@
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("memoryview_check", 0);
-  __Pyx_TraceCall("memoryview_check", __pyx_f[2], 663, 0, __PYX_ERR(2, 663, __pyx_L1_error));
+  __Pyx_TraceCall("memoryview_check", __pyx_f[2], 665, 0, __PYX_ERR(2, 665, __pyx_L1_error));
 
-  /* "View.MemoryView":664
+  /* "View.MemoryView":666
  * @cname('__pyx_memoryview_check')
  * cdef inline bint memoryview_check(object o):
  *     return isinstance(o, memoryview)             # <<<<<<<<<<<<<<
  * 
  * cdef tuple _unellipsify(object index, int ndim):
  */
-  __Pyx_TraceLine(664,0,__PYX_ERR(2, 664, __pyx_L1_error))
+  __Pyx_TraceLine(666,0,__PYX_ERR(2, 666, __pyx_L1_error))
   __pyx_t_1 = __Pyx_TypeCheck(__pyx_v_o, __pyx_memoryview_type); 
   __pyx_r = __pyx_t_1;
   goto __pyx_L0;
 
-  /* "View.MemoryView":663
+  /* "View.MemoryView":665
  * 
  * @cname('__pyx_memoryview_check')
  * cdef inline bint memoryview_check(object o):             # <<<<<<<<<<<<<<
  *     return isinstance(o, memoryview)
  * 
  */
 
@@ -23618,15 +23812,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":666
+/* "View.MemoryView":668
  *     return isinstance(o, memoryview)
  * 
  * cdef tuple _unellipsify(object index, int ndim):             # <<<<<<<<<<<<<<
  *     """
  *     Replace all ellipses with full slices and fill incomplete indices with
  */
 
@@ -23652,436 +23846,436 @@
   int __pyx_t_9;
   int __pyx_t_10;
   PyObject *__pyx_t_11 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_unellipsify", 0);
-  __Pyx_TraceCall("_unellipsify", __pyx_f[2], 666, 0, __PYX_ERR(2, 666, __pyx_L1_error));
+  __Pyx_TraceCall("_unellipsify", __pyx_f[2], 668, 0, __PYX_ERR(2, 668, __pyx_L1_error));
 
-  /* "View.MemoryView":671
+  /* "View.MemoryView":673
  *     full slices.
  *     """
  *     if not isinstance(index, tuple):             # <<<<<<<<<<<<<<
  *         tup = (index,)
  *     else:
  */
-  __Pyx_TraceLine(671,0,__PYX_ERR(2, 671, __pyx_L1_error))
+  __Pyx_TraceLine(673,0,__PYX_ERR(2, 673, __pyx_L1_error))
   __pyx_t_1 = PyTuple_Check(__pyx_v_index); 
   __pyx_t_2 = ((!(__pyx_t_1 != 0)) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":672
+    /* "View.MemoryView":674
  *     """
  *     if not isinstance(index, tuple):
  *         tup = (index,)             # <<<<<<<<<<<<<<
  *     else:
  *         tup = index
  */
-    __Pyx_TraceLine(672,0,__PYX_ERR(2, 672, __pyx_L1_error))
-    __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 672, __pyx_L1_error)
+    __Pyx_TraceLine(674,0,__PYX_ERR(2, 674, __pyx_L1_error))
+    __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 674, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_v_index);
     __Pyx_GIVEREF(__pyx_v_index);
     PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_index);
     __pyx_v_tup = __pyx_t_3;
     __pyx_t_3 = 0;
 
-    /* "View.MemoryView":671
+    /* "View.MemoryView":673
  *     full slices.
  *     """
  *     if not isinstance(index, tuple):             # <<<<<<<<<<<<<<
  *         tup = (index,)
  *     else:
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":674
+  /* "View.MemoryView":676
  *         tup = (index,)
  *     else:
  *         tup = index             # <<<<<<<<<<<<<<
  * 
  *     result = []
  */
-  __Pyx_TraceLine(674,0,__PYX_ERR(2, 674, __pyx_L1_error))
+  __Pyx_TraceLine(676,0,__PYX_ERR(2, 676, __pyx_L1_error))
   /*else*/ {
     __Pyx_INCREF(__pyx_v_index);
     __pyx_v_tup = __pyx_v_index;
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":676
+  /* "View.MemoryView":678
  *         tup = index
  * 
  *     result = []             # <<<<<<<<<<<<<<
  *     have_slices = False
  *     seen_ellipsis = False
  */
-  __Pyx_TraceLine(676,0,__PYX_ERR(2, 676, __pyx_L1_error))
-  __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 676, __pyx_L1_error)
+  __Pyx_TraceLine(678,0,__PYX_ERR(2, 678, __pyx_L1_error))
+  __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 678, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_v_result = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "View.MemoryView":677
+  /* "View.MemoryView":679
  * 
  *     result = []
  *     have_slices = False             # <<<<<<<<<<<<<<
  *     seen_ellipsis = False
  *     for idx, item in enumerate(tup):
  */
-  __Pyx_TraceLine(677,0,__PYX_ERR(2, 677, __pyx_L1_error))
+  __Pyx_TraceLine(679,0,__PYX_ERR(2, 679, __pyx_L1_error))
   __pyx_v_have_slices = 0;
 
-  /* "View.MemoryView":678
+  /* "View.MemoryView":680
  *     result = []
  *     have_slices = False
  *     seen_ellipsis = False             # <<<<<<<<<<<<<<
  *     for idx, item in enumerate(tup):
  *         if item is Ellipsis:
  */
-  __Pyx_TraceLine(678,0,__PYX_ERR(2, 678, __pyx_L1_error))
+  __Pyx_TraceLine(680,0,__PYX_ERR(2, 680, __pyx_L1_error))
   __pyx_v_seen_ellipsis = 0;
 
-  /* "View.MemoryView":679
+  /* "View.MemoryView":681
  *     have_slices = False
  *     seen_ellipsis = False
  *     for idx, item in enumerate(tup):             # <<<<<<<<<<<<<<
  *         if item is Ellipsis:
  *             if not seen_ellipsis:
  */
-  __Pyx_TraceLine(679,0,__PYX_ERR(2, 679, __pyx_L1_error))
+  __Pyx_TraceLine(681,0,__PYX_ERR(2, 681, __pyx_L1_error))
   __Pyx_INCREF(__pyx_int_0);
   __pyx_t_3 = __pyx_int_0;
   if (likely(PyList_CheckExact(__pyx_v_tup)) || PyTuple_CheckExact(__pyx_v_tup)) {
     __pyx_t_4 = __pyx_v_tup; __Pyx_INCREF(__pyx_t_4); __pyx_t_5 = 0;
     __pyx_t_6 = NULL;
   } else {
-    __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_tup); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 679, __pyx_L1_error)
+    __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_tup); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 681, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 679, __pyx_L1_error)
+    __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 681, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_6)) {
       if (likely(PyList_CheckExact(__pyx_t_4))) {
         if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_4)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_7 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(2, 679, __pyx_L1_error)
+        __pyx_t_7 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(2, 681, __pyx_L1_error)
         #else
-        __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(2, 679, __pyx_L1_error)
+        __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(2, 681, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         #endif
       } else {
         if (__pyx_t_5 >= PyTuple_GET_SIZE(__pyx_t_4)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(2, 679, __pyx_L1_error)
+        __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(2, 681, __pyx_L1_error)
         #else
-        __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(2, 679, __pyx_L1_error)
+        __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(2, 681, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         #endif
       }
     } else {
       __pyx_t_7 = __pyx_t_6(__pyx_t_4);
       if (unlikely(!__pyx_t_7)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(2, 679, __pyx_L1_error)
+          else __PYX_ERR(2, 681, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_7);
     }
     __Pyx_XDECREF_SET(__pyx_v_item, __pyx_t_7);
     __pyx_t_7 = 0;
     __Pyx_INCREF(__pyx_t_3);
     __Pyx_XDECREF_SET(__pyx_v_idx, __pyx_t_3);
-    __pyx_t_7 = __Pyx_PyInt_AddObjC(__pyx_t_3, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(2, 679, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyInt_AddObjC(__pyx_t_3, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(2, 681, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_3);
     __pyx_t_3 = __pyx_t_7;
     __pyx_t_7 = 0;
 
-    /* "View.MemoryView":680
+    /* "View.MemoryView":682
  *     seen_ellipsis = False
  *     for idx, item in enumerate(tup):
  *         if item is Ellipsis:             # <<<<<<<<<<<<<<
  *             if not seen_ellipsis:
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))
  */
-    __Pyx_TraceLine(680,0,__PYX_ERR(2, 680, __pyx_L1_error))
+    __Pyx_TraceLine(682,0,__PYX_ERR(2, 682, __pyx_L1_error))
     __pyx_t_2 = (__pyx_v_item == __pyx_builtin_Ellipsis);
     __pyx_t_1 = (__pyx_t_2 != 0);
     if (__pyx_t_1) {
 
-      /* "View.MemoryView":681
+      /* "View.MemoryView":683
  *     for idx, item in enumerate(tup):
  *         if item is Ellipsis:
  *             if not seen_ellipsis:             # <<<<<<<<<<<<<<
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))
  *                 seen_ellipsis = True
  */
-      __Pyx_TraceLine(681,0,__PYX_ERR(2, 681, __pyx_L1_error))
+      __Pyx_TraceLine(683,0,__PYX_ERR(2, 683, __pyx_L1_error))
       __pyx_t_1 = ((!(__pyx_v_seen_ellipsis != 0)) != 0);
       if (__pyx_t_1) {
 
-        /* "View.MemoryView":682
+        /* "View.MemoryView":684
  *         if item is Ellipsis:
  *             if not seen_ellipsis:
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))             # <<<<<<<<<<<<<<
  *                 seen_ellipsis = True
  *             else:
  */
-        __Pyx_TraceLine(682,0,__PYX_ERR(2, 682, __pyx_L1_error))
-        __pyx_t_8 = PyObject_Length(__pyx_v_tup); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(2, 682, __pyx_L1_error)
-        __pyx_t_7 = PyList_New(1 * ((((__pyx_v_ndim - __pyx_t_8) + 1)<0) ? 0:((__pyx_v_ndim - __pyx_t_8) + 1))); if (unlikely(!__pyx_t_7)) __PYX_ERR(2, 682, __pyx_L1_error)
+        __Pyx_TraceLine(684,0,__PYX_ERR(2, 684, __pyx_L1_error))
+        __pyx_t_8 = PyObject_Length(__pyx_v_tup); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(2, 684, __pyx_L1_error)
+        __pyx_t_7 = PyList_New(1 * ((((__pyx_v_ndim - __pyx_t_8) + 1)<0) ? 0:((__pyx_v_ndim - __pyx_t_8) + 1))); if (unlikely(!__pyx_t_7)) __PYX_ERR(2, 684, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         { Py_ssize_t __pyx_temp;
           for (__pyx_temp=0; __pyx_temp < ((__pyx_v_ndim - __pyx_t_8) + 1); __pyx_temp++) {
             __Pyx_INCREF(__pyx_slice__5);
             __Pyx_GIVEREF(__pyx_slice__5);
             PyList_SET_ITEM(__pyx_t_7, __pyx_temp, __pyx_slice__5);
           }
         }
-        __pyx_t_9 = __Pyx_PyList_Extend(__pyx_v_result, __pyx_t_7); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(2, 682, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyList_Extend(__pyx_v_result, __pyx_t_7); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(2, 684, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-        /* "View.MemoryView":683
+        /* "View.MemoryView":685
  *             if not seen_ellipsis:
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))
  *                 seen_ellipsis = True             # <<<<<<<<<<<<<<
  *             else:
  *                 result.append(slice(None))
  */
-        __Pyx_TraceLine(683,0,__PYX_ERR(2, 683, __pyx_L1_error))
+        __Pyx_TraceLine(685,0,__PYX_ERR(2, 685, __pyx_L1_error))
         __pyx_v_seen_ellipsis = 1;
 
-        /* "View.MemoryView":681
+        /* "View.MemoryView":683
  *     for idx, item in enumerate(tup):
  *         if item is Ellipsis:
  *             if not seen_ellipsis:             # <<<<<<<<<<<<<<
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))
  *                 seen_ellipsis = True
  */
         goto __pyx_L7;
       }
 
-      /* "View.MemoryView":685
+      /* "View.MemoryView":687
  *                 seen_ellipsis = True
  *             else:
  *                 result.append(slice(None))             # <<<<<<<<<<<<<<
  *             have_slices = True
  *         else:
  */
-      __Pyx_TraceLine(685,0,__PYX_ERR(2, 685, __pyx_L1_error))
+      __Pyx_TraceLine(687,0,__PYX_ERR(2, 687, __pyx_L1_error))
       /*else*/ {
-        __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_result, __pyx_slice__5); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(2, 685, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_result, __pyx_slice__5); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(2, 687, __pyx_L1_error)
       }
       __pyx_L7:;
 
-      /* "View.MemoryView":686
+      /* "View.MemoryView":688
  *             else:
  *                 result.append(slice(None))
  *             have_slices = True             # <<<<<<<<<<<<<<
  *         else:
  *             if not isinstance(item, slice) and not PyIndex_Check(item):
  */
-      __Pyx_TraceLine(686,0,__PYX_ERR(2, 686, __pyx_L1_error))
+      __Pyx_TraceLine(688,0,__PYX_ERR(2, 688, __pyx_L1_error))
       __pyx_v_have_slices = 1;
 
-      /* "View.MemoryView":680
+      /* "View.MemoryView":682
  *     seen_ellipsis = False
  *     for idx, item in enumerate(tup):
  *         if item is Ellipsis:             # <<<<<<<<<<<<<<
  *             if not seen_ellipsis:
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))
  */
       goto __pyx_L6;
     }
 
-    /* "View.MemoryView":688
+    /* "View.MemoryView":690
  *             have_slices = True
  *         else:
  *             if not isinstance(item, slice) and not PyIndex_Check(item):             # <<<<<<<<<<<<<<
  *                 raise TypeError("Cannot index with type '%s'" % type(item))
  * 
  */
-    __Pyx_TraceLine(688,0,__PYX_ERR(2, 688, __pyx_L1_error))
+    __Pyx_TraceLine(690,0,__PYX_ERR(2, 690, __pyx_L1_error))
     /*else*/ {
       __pyx_t_2 = PySlice_Check(__pyx_v_item); 
       __pyx_t_10 = ((!(__pyx_t_2 != 0)) != 0);
       if (__pyx_t_10) {
       } else {
         __pyx_t_1 = __pyx_t_10;
         goto __pyx_L9_bool_binop_done;
       }
       __pyx_t_10 = ((!(PyIndex_Check(__pyx_v_item) != 0)) != 0);
       __pyx_t_1 = __pyx_t_10;
       __pyx_L9_bool_binop_done:;
       if (unlikely(__pyx_t_1)) {
 
-        /* "View.MemoryView":689
+        /* "View.MemoryView":691
  *         else:
  *             if not isinstance(item, slice) and not PyIndex_Check(item):
  *                 raise TypeError("Cannot index with type '%s'" % type(item))             # <<<<<<<<<<<<<<
  * 
  *             have_slices = have_slices or isinstance(item, slice)
  */
-        __Pyx_TraceLine(689,0,__PYX_ERR(2, 689, __pyx_L1_error))
-        __pyx_t_7 = __Pyx_PyString_FormatSafe(__pyx_kp_s_Cannot_index_with_type_s, ((PyObject *)Py_TYPE(__pyx_v_item))); if (unlikely(!__pyx_t_7)) __PYX_ERR(2, 689, __pyx_L1_error)
+        __Pyx_TraceLine(691,0,__PYX_ERR(2, 691, __pyx_L1_error))
+        __pyx_t_7 = __Pyx_PyString_FormatSafe(__pyx_kp_s_Cannot_index_with_type_s, ((PyObject *)Py_TYPE(__pyx_v_item))); if (unlikely(!__pyx_t_7)) __PYX_ERR(2, 691, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
-        __pyx_t_11 = __Pyx_PyObject_CallOneArg(__pyx_builtin_TypeError, __pyx_t_7); if (unlikely(!__pyx_t_11)) __PYX_ERR(2, 689, __pyx_L1_error)
+        __pyx_t_11 = __Pyx_PyObject_CallOneArg(__pyx_builtin_TypeError, __pyx_t_7); if (unlikely(!__pyx_t_11)) __PYX_ERR(2, 691, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_11);
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_Raise(__pyx_t_11, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-        __PYX_ERR(2, 689, __pyx_L1_error)
+        __PYX_ERR(2, 691, __pyx_L1_error)
 
-        /* "View.MemoryView":688
+        /* "View.MemoryView":690
  *             have_slices = True
  *         else:
  *             if not isinstance(item, slice) and not PyIndex_Check(item):             # <<<<<<<<<<<<<<
  *                 raise TypeError("Cannot index with type '%s'" % type(item))
  * 
  */
       }
 
-      /* "View.MemoryView":691
+      /* "View.MemoryView":693
  *                 raise TypeError("Cannot index with type '%s'" % type(item))
  * 
  *             have_slices = have_slices or isinstance(item, slice)             # <<<<<<<<<<<<<<
  *             result.append(item)
  * 
  */
-      __Pyx_TraceLine(691,0,__PYX_ERR(2, 691, __pyx_L1_error))
+      __Pyx_TraceLine(693,0,__PYX_ERR(2, 693, __pyx_L1_error))
       __pyx_t_10 = (__pyx_v_have_slices != 0);
       if (!__pyx_t_10) {
       } else {
         __pyx_t_1 = __pyx_t_10;
         goto __pyx_L11_bool_binop_done;
       }
       __pyx_t_10 = PySlice_Check(__pyx_v_item); 
       __pyx_t_2 = (__pyx_t_10 != 0);
       __pyx_t_1 = __pyx_t_2;
       __pyx_L11_bool_binop_done:;
       __pyx_v_have_slices = __pyx_t_1;
 
-      /* "View.MemoryView":692
+      /* "View.MemoryView":694
  * 
  *             have_slices = have_slices or isinstance(item, slice)
  *             result.append(item)             # <<<<<<<<<<<<<<
  * 
  *     nslices = ndim - len(result)
  */
-      __Pyx_TraceLine(692,0,__PYX_ERR(2, 692, __pyx_L1_error))
-      __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_result, __pyx_v_item); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(2, 692, __pyx_L1_error)
+      __Pyx_TraceLine(694,0,__PYX_ERR(2, 694, __pyx_L1_error))
+      __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_result, __pyx_v_item); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(2, 694, __pyx_L1_error)
     }
     __pyx_L6:;
 
-    /* "View.MemoryView":679
+    /* "View.MemoryView":681
  *     have_slices = False
  *     seen_ellipsis = False
  *     for idx, item in enumerate(tup):             # <<<<<<<<<<<<<<
  *         if item is Ellipsis:
  *             if not seen_ellipsis:
  */
-    __Pyx_TraceLine(679,0,__PYX_ERR(2, 679, __pyx_L1_error))
+    __Pyx_TraceLine(681,0,__PYX_ERR(2, 681, __pyx_L1_error))
   }
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "View.MemoryView":694
+  /* "View.MemoryView":696
  *             result.append(item)
  * 
  *     nslices = ndim - len(result)             # <<<<<<<<<<<<<<
  *     if nslices:
  *         result.extend([slice(None)] * nslices)
  */
-  __Pyx_TraceLine(694,0,__PYX_ERR(2, 694, __pyx_L1_error))
-  __pyx_t_5 = PyList_GET_SIZE(__pyx_v_result); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(2, 694, __pyx_L1_error)
+  __Pyx_TraceLine(696,0,__PYX_ERR(2, 696, __pyx_L1_error))
+  __pyx_t_5 = PyList_GET_SIZE(__pyx_v_result); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(2, 696, __pyx_L1_error)
   __pyx_v_nslices = (__pyx_v_ndim - __pyx_t_5);
 
-  /* "View.MemoryView":695
+  /* "View.MemoryView":697
  * 
  *     nslices = ndim - len(result)
  *     if nslices:             # <<<<<<<<<<<<<<
  *         result.extend([slice(None)] * nslices)
  * 
  */
-  __Pyx_TraceLine(695,0,__PYX_ERR(2, 695, __pyx_L1_error))
+  __Pyx_TraceLine(697,0,__PYX_ERR(2, 697, __pyx_L1_error))
   __pyx_t_1 = (__pyx_v_nslices != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":696
+    /* "View.MemoryView":698
  *     nslices = ndim - len(result)
  *     if nslices:
  *         result.extend([slice(None)] * nslices)             # <<<<<<<<<<<<<<
  * 
  *     return have_slices or nslices, tuple(result)
  */
-    __Pyx_TraceLine(696,0,__PYX_ERR(2, 696, __pyx_L1_error))
-    __pyx_t_3 = PyList_New(1 * ((__pyx_v_nslices<0) ? 0:__pyx_v_nslices)); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 696, __pyx_L1_error)
+    __Pyx_TraceLine(698,0,__PYX_ERR(2, 698, __pyx_L1_error))
+    __pyx_t_3 = PyList_New(1 * ((__pyx_v_nslices<0) ? 0:__pyx_v_nslices)); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 698, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     { Py_ssize_t __pyx_temp;
       for (__pyx_temp=0; __pyx_temp < __pyx_v_nslices; __pyx_temp++) {
         __Pyx_INCREF(__pyx_slice__5);
         __Pyx_GIVEREF(__pyx_slice__5);
         PyList_SET_ITEM(__pyx_t_3, __pyx_temp, __pyx_slice__5);
       }
     }
-    __pyx_t_9 = __Pyx_PyList_Extend(__pyx_v_result, __pyx_t_3); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(2, 696, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyList_Extend(__pyx_v_result, __pyx_t_3); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(2, 698, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "View.MemoryView":695
+    /* "View.MemoryView":697
  * 
  *     nslices = ndim - len(result)
  *     if nslices:             # <<<<<<<<<<<<<<
  *         result.extend([slice(None)] * nslices)
  * 
  */
   }
 
-  /* "View.MemoryView":698
+  /* "View.MemoryView":700
  *         result.extend([slice(None)] * nslices)
  * 
  *     return have_slices or nslices, tuple(result)             # <<<<<<<<<<<<<<
  * 
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):
  */
-  __Pyx_TraceLine(698,0,__PYX_ERR(2, 698, __pyx_L1_error))
+  __Pyx_TraceLine(700,0,__PYX_ERR(2, 700, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
   if (!__pyx_v_have_slices) {
   } else {
-    __pyx_t_4 = __Pyx_PyBool_FromLong(__pyx_v_have_slices); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 698, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyBool_FromLong(__pyx_v_have_slices); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 700, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_3 = __pyx_t_4;
     __pyx_t_4 = 0;
     goto __pyx_L14_bool_binop_done;
   }
-  __pyx_t_4 = PyInt_FromSsize_t(__pyx_v_nslices); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 698, __pyx_L1_error)
+  __pyx_t_4 = PyInt_FromSsize_t(__pyx_v_nslices); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 700, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_3 = __pyx_t_4;
   __pyx_t_4 = 0;
   __pyx_L14_bool_binop_done:;
-  __pyx_t_4 = PyList_AsTuple(__pyx_v_result); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 698, __pyx_L1_error)
+  __pyx_t_4 = PyList_AsTuple(__pyx_v_result); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 700, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_11 = PyTuple_New(2); if (unlikely(!__pyx_t_11)) __PYX_ERR(2, 698, __pyx_L1_error)
+  __pyx_t_11 = PyTuple_New(2); if (unlikely(!__pyx_t_11)) __PYX_ERR(2, 700, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_11, 1, __pyx_t_4);
   __pyx_t_3 = 0;
   __pyx_t_4 = 0;
   __pyx_r = ((PyObject*)__pyx_t_11);
   __pyx_t_11 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":666
+  /* "View.MemoryView":668
  *     return isinstance(o, memoryview)
  * 
  * cdef tuple _unellipsify(object index, int ndim):             # <<<<<<<<<<<<<<
  *     """
  *     Replace all ellipses with full slices and fill incomplete indices with
  */
 
@@ -24100,15 +24294,15 @@
   __Pyx_XDECREF(__pyx_v_item);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":700
+/* "View.MemoryView":702
  *     return have_slices or nslices, tuple(result)
  * 
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):             # <<<<<<<<<<<<<<
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  */
 
@@ -24122,65 +24316,65 @@
   Py_ssize_t *__pyx_t_3;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("assert_direct_dimensions", 0);
-  __Pyx_TraceCall("assert_direct_dimensions", __pyx_f[2], 700, 0, __PYX_ERR(2, 700, __pyx_L1_error));
+  __Pyx_TraceCall("assert_direct_dimensions", __pyx_f[2], 702, 0, __PYX_ERR(2, 702, __pyx_L1_error));
 
-  /* "View.MemoryView":701
+  /* "View.MemoryView":703
  * 
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):
  *     for suboffset in suboffsets[:ndim]:             # <<<<<<<<<<<<<<
  *         if suboffset >= 0:
  *             raise ValueError("Indirect dimensions not supported")
  */
-  __Pyx_TraceLine(701,0,__PYX_ERR(2, 701, __pyx_L1_error))
+  __Pyx_TraceLine(703,0,__PYX_ERR(2, 703, __pyx_L1_error))
   __pyx_t_2 = (__pyx_v_suboffsets + __pyx_v_ndim);
   for (__pyx_t_3 = __pyx_v_suboffsets; __pyx_t_3 < __pyx_t_2; __pyx_t_3++) {
     __pyx_t_1 = __pyx_t_3;
     __pyx_v_suboffset = (__pyx_t_1[0]);
 
-    /* "View.MemoryView":702
+    /* "View.MemoryView":704
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:             # <<<<<<<<<<<<<<
  *             raise ValueError("Indirect dimensions not supported")
  * 
  */
-    __Pyx_TraceLine(702,0,__PYX_ERR(2, 702, __pyx_L1_error))
+    __Pyx_TraceLine(704,0,__PYX_ERR(2, 704, __pyx_L1_error))
     __pyx_t_4 = ((__pyx_v_suboffset >= 0) != 0);
     if (unlikely(__pyx_t_4)) {
 
-      /* "View.MemoryView":703
+      /* "View.MemoryView":705
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  *             raise ValueError("Indirect dimensions not supported")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-      __Pyx_TraceLine(703,0,__PYX_ERR(2, 703, __pyx_L1_error))
-      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__25, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 703, __pyx_L1_error)
+      __Pyx_TraceLine(705,0,__PYX_ERR(2, 705, __pyx_L1_error))
+      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__26, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 705, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_Raise(__pyx_t_5, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __PYX_ERR(2, 703, __pyx_L1_error)
+      __PYX_ERR(2, 705, __pyx_L1_error)
 
-      /* "View.MemoryView":702
+      /* "View.MemoryView":704
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:             # <<<<<<<<<<<<<<
  *             raise ValueError("Indirect dimensions not supported")
  * 
  */
     }
   }
 
-  /* "View.MemoryView":700
+  /* "View.MemoryView":702
  *     return have_slices or nslices, tuple(result)
  * 
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):             # <<<<<<<<<<<<<<
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  */
 
@@ -24194,15 +24388,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":710
+/* "View.MemoryView":712
  * 
  * @cname('__pyx_memview_slice')
  * cdef memoryview memview_slice(memoryview memview, object indices):             # <<<<<<<<<<<<<<
  *     cdef int new_ndim = 0, suboffset_dim = -1, dim
  *     cdef bint negative_step
  */
 
@@ -24238,569 +24432,569 @@
   Py_ssize_t __pyx_t_10;
   int __pyx_t_11;
   Py_ssize_t __pyx_t_12;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("memview_slice", 0);
-  __Pyx_TraceCall("memview_slice", __pyx_f[2], 710, 0, __PYX_ERR(2, 710, __pyx_L1_error));
+  __Pyx_TraceCall("memview_slice", __pyx_f[2], 712, 0, __PYX_ERR(2, 712, __pyx_L1_error));
 
-  /* "View.MemoryView":711
+  /* "View.MemoryView":713
  * @cname('__pyx_memview_slice')
  * cdef memoryview memview_slice(memoryview memview, object indices):
  *     cdef int new_ndim = 0, suboffset_dim = -1, dim             # <<<<<<<<<<<<<<
  *     cdef bint negative_step
  *     cdef __Pyx_memviewslice src, dst
  */
-  __Pyx_TraceLine(711,0,__PYX_ERR(2, 711, __pyx_L1_error))
+  __Pyx_TraceLine(713,0,__PYX_ERR(2, 713, __pyx_L1_error))
   __pyx_v_new_ndim = 0;
   __pyx_v_suboffset_dim = -1;
 
-  /* "View.MemoryView":718
+  /* "View.MemoryView":720
  * 
  * 
  *     memset(&dst, 0, sizeof(dst))             # <<<<<<<<<<<<<<
  * 
  *     cdef _memoryviewslice memviewsliceobj
  */
-  __Pyx_TraceLine(718,0,__PYX_ERR(2, 718, __pyx_L1_error))
+  __Pyx_TraceLine(720,0,__PYX_ERR(2, 720, __pyx_L1_error))
   (void)(memset((&__pyx_v_dst), 0, (sizeof(__pyx_v_dst))));
 
-  /* "View.MemoryView":722
+  /* "View.MemoryView":724
  *     cdef _memoryviewslice memviewsliceobj
  * 
  *     assert memview.view.ndim > 0             # <<<<<<<<<<<<<<
  * 
  *     if isinstance(memview, _memoryviewslice):
  */
-  __Pyx_TraceLine(722,0,__PYX_ERR(2, 722, __pyx_L1_error))
+  __Pyx_TraceLine(724,0,__PYX_ERR(2, 724, __pyx_L1_error))
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(!Py_OptimizeFlag)) {
     if (unlikely(!((__pyx_v_memview->view.ndim > 0) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(2, 722, __pyx_L1_error)
+      __PYX_ERR(2, 724, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "View.MemoryView":724
+  /* "View.MemoryView":726
  *     assert memview.view.ndim > 0
  * 
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         memviewsliceobj = memview
  *         p_src = &memviewsliceobj.from_slice
  */
-  __Pyx_TraceLine(724,0,__PYX_ERR(2, 724, __pyx_L1_error))
+  __Pyx_TraceLine(726,0,__PYX_ERR(2, 726, __pyx_L1_error))
   __pyx_t_1 = __Pyx_TypeCheck(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":725
+    /* "View.MemoryView":727
  * 
  *     if isinstance(memview, _memoryviewslice):
  *         memviewsliceobj = memview             # <<<<<<<<<<<<<<
  *         p_src = &memviewsliceobj.from_slice
  *     else:
  */
-    __Pyx_TraceLine(725,0,__PYX_ERR(2, 725, __pyx_L1_error))
-    if (!(likely(((((PyObject *)__pyx_v_memview)) == Py_None) || likely(__Pyx_TypeTest(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type))))) __PYX_ERR(2, 725, __pyx_L1_error)
+    __Pyx_TraceLine(727,0,__PYX_ERR(2, 727, __pyx_L1_error))
+    if (!(likely(((((PyObject *)__pyx_v_memview)) == Py_None) || likely(__Pyx_TypeTest(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type))))) __PYX_ERR(2, 727, __pyx_L1_error)
     __pyx_t_3 = ((PyObject *)__pyx_v_memview);
     __Pyx_INCREF(__pyx_t_3);
     __pyx_v_memviewsliceobj = ((struct __pyx_memoryviewslice_obj *)__pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "View.MemoryView":726
+    /* "View.MemoryView":728
  *     if isinstance(memview, _memoryviewslice):
  *         memviewsliceobj = memview
  *         p_src = &memviewsliceobj.from_slice             # <<<<<<<<<<<<<<
  *     else:
  *         slice_copy(memview, &src)
  */
-    __Pyx_TraceLine(726,0,__PYX_ERR(2, 726, __pyx_L1_error))
+    __Pyx_TraceLine(728,0,__PYX_ERR(2, 728, __pyx_L1_error))
     __pyx_v_p_src = (&__pyx_v_memviewsliceobj->from_slice);
 
-    /* "View.MemoryView":724
+    /* "View.MemoryView":726
  *     assert memview.view.ndim > 0
  * 
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         memviewsliceobj = memview
  *         p_src = &memviewsliceobj.from_slice
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":728
+  /* "View.MemoryView":730
  *         p_src = &memviewsliceobj.from_slice
  *     else:
  *         slice_copy(memview, &src)             # <<<<<<<<<<<<<<
  *         p_src = &src
  * 
  */
-  __Pyx_TraceLine(728,0,__PYX_ERR(2, 728, __pyx_L1_error))
+  __Pyx_TraceLine(730,0,__PYX_ERR(2, 730, __pyx_L1_error))
   /*else*/ {
     __pyx_memoryview_slice_copy(__pyx_v_memview, (&__pyx_v_src));
 
-    /* "View.MemoryView":729
+    /* "View.MemoryView":731
  *     else:
  *         slice_copy(memview, &src)
  *         p_src = &src             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __Pyx_TraceLine(729,0,__PYX_ERR(2, 729, __pyx_L1_error))
+    __Pyx_TraceLine(731,0,__PYX_ERR(2, 731, __pyx_L1_error))
     __pyx_v_p_src = (&__pyx_v_src);
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":735
+  /* "View.MemoryView":737
  * 
  * 
  *     dst.memview = p_src.memview             # <<<<<<<<<<<<<<
  *     dst.data = p_src.data
  * 
  */
-  __Pyx_TraceLine(735,0,__PYX_ERR(2, 735, __pyx_L1_error))
+  __Pyx_TraceLine(737,0,__PYX_ERR(2, 737, __pyx_L1_error))
   __pyx_t_4 = __pyx_v_p_src->memview;
   __pyx_v_dst.memview = __pyx_t_4;
 
-  /* "View.MemoryView":736
+  /* "View.MemoryView":738
  * 
  *     dst.memview = p_src.memview
  *     dst.data = p_src.data             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_TraceLine(736,0,__PYX_ERR(2, 736, __pyx_L1_error))
+  __Pyx_TraceLine(738,0,__PYX_ERR(2, 738, __pyx_L1_error))
   __pyx_t_5 = __pyx_v_p_src->data;
   __pyx_v_dst.data = __pyx_t_5;
 
-  /* "View.MemoryView":741
+  /* "View.MemoryView":743
  * 
  * 
  *     cdef __Pyx_memviewslice *p_dst = &dst             # <<<<<<<<<<<<<<
  *     cdef int *p_suboffset_dim = &suboffset_dim
  *     cdef Py_ssize_t start, stop, step
  */
-  __Pyx_TraceLine(741,0,__PYX_ERR(2, 741, __pyx_L1_error))
+  __Pyx_TraceLine(743,0,__PYX_ERR(2, 743, __pyx_L1_error))
   __pyx_v_p_dst = (&__pyx_v_dst);
 
-  /* "View.MemoryView":742
+  /* "View.MemoryView":744
  * 
  *     cdef __Pyx_memviewslice *p_dst = &dst
  *     cdef int *p_suboffset_dim = &suboffset_dim             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t start, stop, step
  *     cdef bint have_start, have_stop, have_step
  */
-  __Pyx_TraceLine(742,0,__PYX_ERR(2, 742, __pyx_L1_error))
+  __Pyx_TraceLine(744,0,__PYX_ERR(2, 744, __pyx_L1_error))
   __pyx_v_p_suboffset_dim = (&__pyx_v_suboffset_dim);
 
-  /* "View.MemoryView":746
+  /* "View.MemoryView":748
  *     cdef bint have_start, have_stop, have_step
  * 
  *     for dim, index in enumerate(indices):             # <<<<<<<<<<<<<<
  *         if PyIndex_Check(index):
  *             slice_memviewslice(
  */
-  __Pyx_TraceLine(746,0,__PYX_ERR(2, 746, __pyx_L1_error))
+  __Pyx_TraceLine(748,0,__PYX_ERR(2, 748, __pyx_L1_error))
   __pyx_t_6 = 0;
   if (likely(PyList_CheckExact(__pyx_v_indices)) || PyTuple_CheckExact(__pyx_v_indices)) {
     __pyx_t_3 = __pyx_v_indices; __Pyx_INCREF(__pyx_t_3); __pyx_t_7 = 0;
     __pyx_t_8 = NULL;
   } else {
-    __pyx_t_7 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_indices); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 746, __pyx_L1_error)
+    __pyx_t_7 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_indices); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 748, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_8 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 746, __pyx_L1_error)
+    __pyx_t_8 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 748, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_8)) {
       if (likely(PyList_CheckExact(__pyx_t_3))) {
         if (__pyx_t_7 >= PyList_GET_SIZE(__pyx_t_3)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_9 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_7); __Pyx_INCREF(__pyx_t_9); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(2, 746, __pyx_L1_error)
+        __pyx_t_9 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_7); __Pyx_INCREF(__pyx_t_9); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(2, 748, __pyx_L1_error)
         #else
-        __pyx_t_9 = PySequence_ITEM(__pyx_t_3, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 746, __pyx_L1_error)
+        __pyx_t_9 = PySequence_ITEM(__pyx_t_3, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 748, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_9);
         #endif
       } else {
         if (__pyx_t_7 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_9 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_7); __Pyx_INCREF(__pyx_t_9); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(2, 746, __pyx_L1_error)
+        __pyx_t_9 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_7); __Pyx_INCREF(__pyx_t_9); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(2, 748, __pyx_L1_error)
         #else
-        __pyx_t_9 = PySequence_ITEM(__pyx_t_3, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 746, __pyx_L1_error)
+        __pyx_t_9 = PySequence_ITEM(__pyx_t_3, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 748, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_9);
         #endif
       }
     } else {
       __pyx_t_9 = __pyx_t_8(__pyx_t_3);
       if (unlikely(!__pyx_t_9)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(2, 746, __pyx_L1_error)
+          else __PYX_ERR(2, 748, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_9);
     }
     __Pyx_XDECREF_SET(__pyx_v_index, __pyx_t_9);
     __pyx_t_9 = 0;
     __pyx_v_dim = __pyx_t_6;
     __pyx_t_6 = (__pyx_t_6 + 1);
 
-    /* "View.MemoryView":747
+    /* "View.MemoryView":749
  * 
  *     for dim, index in enumerate(indices):
  *         if PyIndex_Check(index):             # <<<<<<<<<<<<<<
  *             slice_memviewslice(
  *                 p_dst, p_src.shape[dim], p_src.strides[dim], p_src.suboffsets[dim],
  */
-    __Pyx_TraceLine(747,0,__PYX_ERR(2, 747, __pyx_L1_error))
+    __Pyx_TraceLine(749,0,__PYX_ERR(2, 749, __pyx_L1_error))
     __pyx_t_2 = (PyIndex_Check(__pyx_v_index) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":751
+      /* "View.MemoryView":753
  *                 p_dst, p_src.shape[dim], p_src.strides[dim], p_src.suboffsets[dim],
  *                 dim, new_ndim, p_suboffset_dim,
  *                 index, 0, 0, # start, stop, step             # <<<<<<<<<<<<<<
  *                 0, 0, 0, # have_{start,stop,step}
  *                 False)
  */
-      __Pyx_TraceLine(751,0,__PYX_ERR(2, 751, __pyx_L1_error))
-      __pyx_t_10 = __Pyx_PyIndex_AsSsize_t(__pyx_v_index); if (unlikely((__pyx_t_10 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(2, 751, __pyx_L1_error)
+      __Pyx_TraceLine(753,0,__PYX_ERR(2, 753, __pyx_L1_error))
+      __pyx_t_10 = __Pyx_PyIndex_AsSsize_t(__pyx_v_index); if (unlikely((__pyx_t_10 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(2, 753, __pyx_L1_error)
 
-      /* "View.MemoryView":748
+      /* "View.MemoryView":750
  *     for dim, index in enumerate(indices):
  *         if PyIndex_Check(index):
  *             slice_memviewslice(             # <<<<<<<<<<<<<<
  *                 p_dst, p_src.shape[dim], p_src.strides[dim], p_src.suboffsets[dim],
  *                 dim, new_ndim, p_suboffset_dim,
  */
-      __Pyx_TraceLine(748,0,__PYX_ERR(2, 748, __pyx_L1_error))
-      __pyx_t_11 = __pyx_memoryview_slice_memviewslice(__pyx_v_p_dst, (__pyx_v_p_src->shape[__pyx_v_dim]), (__pyx_v_p_src->strides[__pyx_v_dim]), (__pyx_v_p_src->suboffsets[__pyx_v_dim]), __pyx_v_dim, __pyx_v_new_ndim, __pyx_v_p_suboffset_dim, __pyx_t_10, 0, 0, 0, 0, 0, 0); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(2, 748, __pyx_L1_error)
+      __Pyx_TraceLine(750,0,__PYX_ERR(2, 750, __pyx_L1_error))
+      __pyx_t_11 = __pyx_memoryview_slice_memviewslice(__pyx_v_p_dst, (__pyx_v_p_src->shape[__pyx_v_dim]), (__pyx_v_p_src->strides[__pyx_v_dim]), (__pyx_v_p_src->suboffsets[__pyx_v_dim]), __pyx_v_dim, __pyx_v_new_ndim, __pyx_v_p_suboffset_dim, __pyx_t_10, 0, 0, 0, 0, 0, 0); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(2, 750, __pyx_L1_error)
 
-      /* "View.MemoryView":747
+      /* "View.MemoryView":749
  * 
  *     for dim, index in enumerate(indices):
  *         if PyIndex_Check(index):             # <<<<<<<<<<<<<<
  *             slice_memviewslice(
  *                 p_dst, p_src.shape[dim], p_src.strides[dim], p_src.suboffsets[dim],
  */
       goto __pyx_L6;
     }
 
-    /* "View.MemoryView":754
+    /* "View.MemoryView":756
  *                 0, 0, 0, # have_{start,stop,step}
  *                 False)
  *         elif index is None:             # <<<<<<<<<<<<<<
  *             p_dst.shape[new_ndim] = 1
  *             p_dst.strides[new_ndim] = 0
  */
-    __Pyx_TraceLine(754,0,__PYX_ERR(2, 754, __pyx_L1_error))
+    __Pyx_TraceLine(756,0,__PYX_ERR(2, 756, __pyx_L1_error))
     __pyx_t_2 = (__pyx_v_index == Py_None);
     __pyx_t_1 = (__pyx_t_2 != 0);
     if (__pyx_t_1) {
 
-      /* "View.MemoryView":755
+      /* "View.MemoryView":757
  *                 False)
  *         elif index is None:
  *             p_dst.shape[new_ndim] = 1             # <<<<<<<<<<<<<<
  *             p_dst.strides[new_ndim] = 0
  *             p_dst.suboffsets[new_ndim] = -1
  */
-      __Pyx_TraceLine(755,0,__PYX_ERR(2, 755, __pyx_L1_error))
+      __Pyx_TraceLine(757,0,__PYX_ERR(2, 757, __pyx_L1_error))
       (__pyx_v_p_dst->shape[__pyx_v_new_ndim]) = 1;
 
-      /* "View.MemoryView":756
+      /* "View.MemoryView":758
  *         elif index is None:
  *             p_dst.shape[new_ndim] = 1
  *             p_dst.strides[new_ndim] = 0             # <<<<<<<<<<<<<<
  *             p_dst.suboffsets[new_ndim] = -1
  *             new_ndim += 1
  */
-      __Pyx_TraceLine(756,0,__PYX_ERR(2, 756, __pyx_L1_error))
+      __Pyx_TraceLine(758,0,__PYX_ERR(2, 758, __pyx_L1_error))
       (__pyx_v_p_dst->strides[__pyx_v_new_ndim]) = 0;
 
-      /* "View.MemoryView":757
+      /* "View.MemoryView":759
  *             p_dst.shape[new_ndim] = 1
  *             p_dst.strides[new_ndim] = 0
  *             p_dst.suboffsets[new_ndim] = -1             # <<<<<<<<<<<<<<
  *             new_ndim += 1
  *         else:
  */
-      __Pyx_TraceLine(757,0,__PYX_ERR(2, 757, __pyx_L1_error))
+      __Pyx_TraceLine(759,0,__PYX_ERR(2, 759, __pyx_L1_error))
       (__pyx_v_p_dst->suboffsets[__pyx_v_new_ndim]) = -1L;
 
-      /* "View.MemoryView":758
+      /* "View.MemoryView":760
  *             p_dst.strides[new_ndim] = 0
  *             p_dst.suboffsets[new_ndim] = -1
  *             new_ndim += 1             # <<<<<<<<<<<<<<
  *         else:
  *             start = index.start or 0
  */
-      __Pyx_TraceLine(758,0,__PYX_ERR(2, 758, __pyx_L1_error))
+      __Pyx_TraceLine(760,0,__PYX_ERR(2, 760, __pyx_L1_error))
       __pyx_v_new_ndim = (__pyx_v_new_ndim + 1);
 
-      /* "View.MemoryView":754
+      /* "View.MemoryView":756
  *                 0, 0, 0, # have_{start,stop,step}
  *                 False)
  *         elif index is None:             # <<<<<<<<<<<<<<
  *             p_dst.shape[new_ndim] = 1
  *             p_dst.strides[new_ndim] = 0
  */
       goto __pyx_L6;
     }
 
-    /* "View.MemoryView":760
+    /* "View.MemoryView":762
  *             new_ndim += 1
  *         else:
  *             start = index.start or 0             # <<<<<<<<<<<<<<
  *             stop = index.stop or 0
  *             step = index.step or 0
  */
-    __Pyx_TraceLine(760,0,__PYX_ERR(2, 760, __pyx_L1_error))
+    __Pyx_TraceLine(762,0,__PYX_ERR(2, 762, __pyx_L1_error))
     /*else*/ {
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_start); if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 760, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_start); if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 762, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
-      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(2, 760, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(2, 762, __pyx_L1_error)
       if (!__pyx_t_1) {
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       } else {
-        __pyx_t_12 = __Pyx_PyIndex_AsSsize_t(__pyx_t_9); if (unlikely((__pyx_t_12 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(2, 760, __pyx_L1_error)
+        __pyx_t_12 = __Pyx_PyIndex_AsSsize_t(__pyx_t_9); if (unlikely((__pyx_t_12 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(2, 762, __pyx_L1_error)
         __pyx_t_10 = __pyx_t_12;
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         goto __pyx_L7_bool_binop_done;
       }
       __pyx_t_10 = 0;
       __pyx_L7_bool_binop_done:;
       __pyx_v_start = __pyx_t_10;
 
-      /* "View.MemoryView":761
+      /* "View.MemoryView":763
  *         else:
  *             start = index.start or 0
  *             stop = index.stop or 0             # <<<<<<<<<<<<<<
  *             step = index.step or 0
  * 
  */
-      __Pyx_TraceLine(761,0,__PYX_ERR(2, 761, __pyx_L1_error))
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_stop); if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 761, __pyx_L1_error)
+      __Pyx_TraceLine(763,0,__PYX_ERR(2, 763, __pyx_L1_error))
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_stop); if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 763, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
-      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(2, 761, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(2, 763, __pyx_L1_error)
       if (!__pyx_t_1) {
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       } else {
-        __pyx_t_12 = __Pyx_PyIndex_AsSsize_t(__pyx_t_9); if (unlikely((__pyx_t_12 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(2, 761, __pyx_L1_error)
+        __pyx_t_12 = __Pyx_PyIndex_AsSsize_t(__pyx_t_9); if (unlikely((__pyx_t_12 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(2, 763, __pyx_L1_error)
         __pyx_t_10 = __pyx_t_12;
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         goto __pyx_L9_bool_binop_done;
       }
       __pyx_t_10 = 0;
       __pyx_L9_bool_binop_done:;
       __pyx_v_stop = __pyx_t_10;
 
-      /* "View.MemoryView":762
+      /* "View.MemoryView":764
  *             start = index.start or 0
  *             stop = index.stop or 0
  *             step = index.step or 0             # <<<<<<<<<<<<<<
  * 
  *             have_start = index.start is not None
  */
-      __Pyx_TraceLine(762,0,__PYX_ERR(2, 762, __pyx_L1_error))
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_step); if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 762, __pyx_L1_error)
+      __Pyx_TraceLine(764,0,__PYX_ERR(2, 764, __pyx_L1_error))
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_step); if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 764, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
-      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(2, 762, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(2, 764, __pyx_L1_error)
       if (!__pyx_t_1) {
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       } else {
-        __pyx_t_12 = __Pyx_PyIndex_AsSsize_t(__pyx_t_9); if (unlikely((__pyx_t_12 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(2, 762, __pyx_L1_error)
+        __pyx_t_12 = __Pyx_PyIndex_AsSsize_t(__pyx_t_9); if (unlikely((__pyx_t_12 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(2, 764, __pyx_L1_error)
         __pyx_t_10 = __pyx_t_12;
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         goto __pyx_L11_bool_binop_done;
       }
       __pyx_t_10 = 0;
       __pyx_L11_bool_binop_done:;
       __pyx_v_step = __pyx_t_10;
 
-      /* "View.MemoryView":764
+      /* "View.MemoryView":766
  *             step = index.step or 0
  * 
  *             have_start = index.start is not None             # <<<<<<<<<<<<<<
  *             have_stop = index.stop is not None
  *             have_step = index.step is not None
  */
-      __Pyx_TraceLine(764,0,__PYX_ERR(2, 764, __pyx_L1_error))
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_start); if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 764, __pyx_L1_error)
+      __Pyx_TraceLine(766,0,__PYX_ERR(2, 766, __pyx_L1_error))
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_start); if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 766, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __pyx_t_1 = (__pyx_t_9 != Py_None);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __pyx_v_have_start = __pyx_t_1;
 
-      /* "View.MemoryView":765
+      /* "View.MemoryView":767
  * 
  *             have_start = index.start is not None
  *             have_stop = index.stop is not None             # <<<<<<<<<<<<<<
  *             have_step = index.step is not None
  * 
  */
-      __Pyx_TraceLine(765,0,__PYX_ERR(2, 765, __pyx_L1_error))
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_stop); if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 765, __pyx_L1_error)
+      __Pyx_TraceLine(767,0,__PYX_ERR(2, 767, __pyx_L1_error))
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_stop); if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 767, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __pyx_t_1 = (__pyx_t_9 != Py_None);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __pyx_v_have_stop = __pyx_t_1;
 
-      /* "View.MemoryView":766
+      /* "View.MemoryView":768
  *             have_start = index.start is not None
  *             have_stop = index.stop is not None
  *             have_step = index.step is not None             # <<<<<<<<<<<<<<
  * 
  *             slice_memviewslice(
  */
-      __Pyx_TraceLine(766,0,__PYX_ERR(2, 766, __pyx_L1_error))
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_step); if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 766, __pyx_L1_error)
+      __Pyx_TraceLine(768,0,__PYX_ERR(2, 768, __pyx_L1_error))
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_step); if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 768, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __pyx_t_1 = (__pyx_t_9 != Py_None);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __pyx_v_have_step = __pyx_t_1;
 
-      /* "View.MemoryView":768
+      /* "View.MemoryView":770
  *             have_step = index.step is not None
  * 
  *             slice_memviewslice(             # <<<<<<<<<<<<<<
  *                 p_dst, p_src.shape[dim], p_src.strides[dim], p_src.suboffsets[dim],
  *                 dim, new_ndim, p_suboffset_dim,
  */
-      __Pyx_TraceLine(768,0,__PYX_ERR(2, 768, __pyx_L1_error))
-      __pyx_t_11 = __pyx_memoryview_slice_memviewslice(__pyx_v_p_dst, (__pyx_v_p_src->shape[__pyx_v_dim]), (__pyx_v_p_src->strides[__pyx_v_dim]), (__pyx_v_p_src->suboffsets[__pyx_v_dim]), __pyx_v_dim, __pyx_v_new_ndim, __pyx_v_p_suboffset_dim, __pyx_v_start, __pyx_v_stop, __pyx_v_step, __pyx_v_have_start, __pyx_v_have_stop, __pyx_v_have_step, 1); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(2, 768, __pyx_L1_error)
+      __Pyx_TraceLine(770,0,__PYX_ERR(2, 770, __pyx_L1_error))
+      __pyx_t_11 = __pyx_memoryview_slice_memviewslice(__pyx_v_p_dst, (__pyx_v_p_src->shape[__pyx_v_dim]), (__pyx_v_p_src->strides[__pyx_v_dim]), (__pyx_v_p_src->suboffsets[__pyx_v_dim]), __pyx_v_dim, __pyx_v_new_ndim, __pyx_v_p_suboffset_dim, __pyx_v_start, __pyx_v_stop, __pyx_v_step, __pyx_v_have_start, __pyx_v_have_stop, __pyx_v_have_step, 1); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(2, 770, __pyx_L1_error)
 
-      /* "View.MemoryView":774
+      /* "View.MemoryView":776
  *                 have_start, have_stop, have_step,
  *                 True)
  *             new_ndim += 1             # <<<<<<<<<<<<<<
  * 
  *     if isinstance(memview, _memoryviewslice):
  */
-      __Pyx_TraceLine(774,0,__PYX_ERR(2, 774, __pyx_L1_error))
+      __Pyx_TraceLine(776,0,__PYX_ERR(2, 776, __pyx_L1_error))
       __pyx_v_new_ndim = (__pyx_v_new_ndim + 1);
     }
     __pyx_L6:;
 
-    /* "View.MemoryView":746
+    /* "View.MemoryView":748
  *     cdef bint have_start, have_stop, have_step
  * 
  *     for dim, index in enumerate(indices):             # <<<<<<<<<<<<<<
  *         if PyIndex_Check(index):
  *             slice_memviewslice(
  */
-    __Pyx_TraceLine(746,0,__PYX_ERR(2, 746, __pyx_L1_error))
+    __Pyx_TraceLine(748,0,__PYX_ERR(2, 748, __pyx_L1_error))
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "View.MemoryView":776
+  /* "View.MemoryView":778
  *             new_ndim += 1
  * 
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         return memoryview_fromslice(dst, new_ndim,
  *                                     memviewsliceobj.to_object_func,
  */
-  __Pyx_TraceLine(776,0,__PYX_ERR(2, 776, __pyx_L1_error))
+  __Pyx_TraceLine(778,0,__PYX_ERR(2, 778, __pyx_L1_error))
   __pyx_t_1 = __Pyx_TypeCheck(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":777
+    /* "View.MemoryView":779
  * 
  *     if isinstance(memview, _memoryviewslice):
  *         return memoryview_fromslice(dst, new_ndim,             # <<<<<<<<<<<<<<
  *                                     memviewsliceobj.to_object_func,
  *                                     memviewsliceobj.to_dtype_func,
  */
-    __Pyx_TraceLine(777,0,__PYX_ERR(2, 777, __pyx_L1_error))
+    __Pyx_TraceLine(779,0,__PYX_ERR(2, 779, __pyx_L1_error))
     __Pyx_XDECREF(((PyObject *)__pyx_r));
 
-    /* "View.MemoryView":778
+    /* "View.MemoryView":780
  *     if isinstance(memview, _memoryviewslice):
  *         return memoryview_fromslice(dst, new_ndim,
  *                                     memviewsliceobj.to_object_func,             # <<<<<<<<<<<<<<
  *                                     memviewsliceobj.to_dtype_func,
  *                                     memview.dtype_is_object)
  */
-    __Pyx_TraceLine(778,0,__PYX_ERR(2, 778, __pyx_L1_error))
-    if (unlikely(!__pyx_v_memviewsliceobj)) { __Pyx_RaiseUnboundLocalError("memviewsliceobj"); __PYX_ERR(2, 778, __pyx_L1_error) }
+    __Pyx_TraceLine(780,0,__PYX_ERR(2, 780, __pyx_L1_error))
+    if (unlikely(!__pyx_v_memviewsliceobj)) { __Pyx_RaiseUnboundLocalError("memviewsliceobj"); __PYX_ERR(2, 780, __pyx_L1_error) }
 
-    /* "View.MemoryView":779
+    /* "View.MemoryView":781
  *         return memoryview_fromslice(dst, new_ndim,
  *                                     memviewsliceobj.to_object_func,
  *                                     memviewsliceobj.to_dtype_func,             # <<<<<<<<<<<<<<
  *                                     memview.dtype_is_object)
  *     else:
  */
-    __Pyx_TraceLine(779,0,__PYX_ERR(2, 779, __pyx_L1_error))
-    if (unlikely(!__pyx_v_memviewsliceobj)) { __Pyx_RaiseUnboundLocalError("memviewsliceobj"); __PYX_ERR(2, 779, __pyx_L1_error) }
+    __Pyx_TraceLine(781,0,__PYX_ERR(2, 781, __pyx_L1_error))
+    if (unlikely(!__pyx_v_memviewsliceobj)) { __Pyx_RaiseUnboundLocalError("memviewsliceobj"); __PYX_ERR(2, 781, __pyx_L1_error) }
 
-    /* "View.MemoryView":777
+    /* "View.MemoryView":779
  * 
  *     if isinstance(memview, _memoryviewslice):
  *         return memoryview_fromslice(dst, new_ndim,             # <<<<<<<<<<<<<<
  *                                     memviewsliceobj.to_object_func,
  *                                     memviewsliceobj.to_dtype_func,
  */
-    __Pyx_TraceLine(777,0,__PYX_ERR(2, 777, __pyx_L1_error))
-    __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_dst, __pyx_v_new_ndim, __pyx_v_memviewsliceobj->to_object_func, __pyx_v_memviewsliceobj->to_dtype_func, __pyx_v_memview->dtype_is_object); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 777, __pyx_L1_error)
+    __Pyx_TraceLine(779,0,__PYX_ERR(2, 779, __pyx_L1_error))
+    __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_dst, __pyx_v_new_ndim, __pyx_v_memviewsliceobj->to_object_func, __pyx_v_memviewsliceobj->to_dtype_func, __pyx_v_memview->dtype_is_object); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 779, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_memoryview_type))))) __PYX_ERR(2, 777, __pyx_L1_error)
+    if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_memoryview_type))))) __PYX_ERR(2, 779, __pyx_L1_error)
     __pyx_r = ((struct __pyx_memoryview_obj *)__pyx_t_3);
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "View.MemoryView":776
+    /* "View.MemoryView":778
  *             new_ndim += 1
  * 
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         return memoryview_fromslice(dst, new_ndim,
  *                                     memviewsliceobj.to_object_func,
  */
   }
 
-  /* "View.MemoryView":782
+  /* "View.MemoryView":784
  *                                     memview.dtype_is_object)
  *     else:
  *         return memoryview_fromslice(dst, new_ndim, NULL, NULL,             # <<<<<<<<<<<<<<
  *                                     memview.dtype_is_object)
  * 
  */
-  __Pyx_TraceLine(782,0,__PYX_ERR(2, 782, __pyx_L1_error))
+  __Pyx_TraceLine(784,0,__PYX_ERR(2, 784, __pyx_L1_error))
   /*else*/ {
     __Pyx_XDECREF(((PyObject *)__pyx_r));
 
-    /* "View.MemoryView":783
+    /* "View.MemoryView":785
  *     else:
  *         return memoryview_fromslice(dst, new_ndim, NULL, NULL,
  *                                     memview.dtype_is_object)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __Pyx_TraceLine(783,0,__PYX_ERR(2, 783, __pyx_L1_error))
-    __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_dst, __pyx_v_new_ndim, NULL, NULL, __pyx_v_memview->dtype_is_object); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 782, __pyx_L1_error)
+    __Pyx_TraceLine(785,0,__PYX_ERR(2, 785, __pyx_L1_error))
+    __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_dst, __pyx_v_new_ndim, NULL, NULL, __pyx_v_memview->dtype_is_object); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 784, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
 
-    /* "View.MemoryView":782
+    /* "View.MemoryView":784
  *                                     memview.dtype_is_object)
  *     else:
  *         return memoryview_fromslice(dst, new_ndim, NULL, NULL,             # <<<<<<<<<<<<<<
  *                                     memview.dtype_is_object)
  * 
  */
-    __Pyx_TraceLine(782,0,__PYX_ERR(2, 782, __pyx_L1_error))
-    if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_memoryview_type))))) __PYX_ERR(2, 782, __pyx_L1_error)
+    __Pyx_TraceLine(784,0,__PYX_ERR(2, 784, __pyx_L1_error))
+    if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_memoryview_type))))) __PYX_ERR(2, 784, __pyx_L1_error)
     __pyx_r = ((struct __pyx_memoryview_obj *)__pyx_t_3);
     __pyx_t_3 = 0;
     goto __pyx_L0;
   }
 
-  /* "View.MemoryView":710
+  /* "View.MemoryView":712
  * 
  * @cname('__pyx_memview_slice')
  * cdef memoryview memview_slice(memoryview memview, object indices):             # <<<<<<<<<<<<<<
  *     cdef int new_ndim = 0, suboffset_dim = -1, dim
  *     cdef bint negative_step
  */
 
@@ -24815,15 +25009,15 @@
   __Pyx_XDECREF(__pyx_v_index);
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":807
+/* "View.MemoryView":809
  * 
  * @cname('__pyx_memoryview_slice_memviewslice')
  * cdef int slice_memviewslice(             # <<<<<<<<<<<<<<
  *         __Pyx_memviewslice *dst,
  *         Py_ssize_t shape, Py_ssize_t stride, Py_ssize_t suboffset,
  */
 
@@ -24834,806 +25028,806 @@
   __Pyx_TraceDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_TraceCall("slice_memviewslice", __pyx_f[2], 807, 1, __PYX_ERR(2, 807, __pyx_L1_error));
+  __Pyx_TraceCall("slice_memviewslice", __pyx_f[2], 809, 1, __PYX_ERR(2, 809, __pyx_L1_error));
 
-  /* "View.MemoryView":827
+  /* "View.MemoryView":829
  *     cdef bint negative_step
  * 
  *     if not is_slice:             # <<<<<<<<<<<<<<
  * 
  *         if start < 0:
  */
-  __Pyx_TraceLine(827,1,__PYX_ERR(2, 827, __pyx_L1_error))
+  __Pyx_TraceLine(829,1,__PYX_ERR(2, 829, __pyx_L1_error))
   __pyx_t_1 = ((!(__pyx_v_is_slice != 0)) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":829
+    /* "View.MemoryView":831
  *     if not is_slice:
  * 
  *         if start < 0:             # <<<<<<<<<<<<<<
  *             start += shape
  *         if not 0 <= start < shape:
  */
-    __Pyx_TraceLine(829,1,__PYX_ERR(2, 829, __pyx_L1_error))
+    __Pyx_TraceLine(831,1,__PYX_ERR(2, 831, __pyx_L1_error))
     __pyx_t_1 = ((__pyx_v_start < 0) != 0);
     if (__pyx_t_1) {
 
-      /* "View.MemoryView":830
+      /* "View.MemoryView":832
  * 
  *         if start < 0:
  *             start += shape             # <<<<<<<<<<<<<<
  *         if not 0 <= start < shape:
  *             _err_dim(IndexError, "Index out of bounds (axis %d)", dim)
  */
-      __Pyx_TraceLine(830,1,__PYX_ERR(2, 830, __pyx_L1_error))
+      __Pyx_TraceLine(832,1,__PYX_ERR(2, 832, __pyx_L1_error))
       __pyx_v_start = (__pyx_v_start + __pyx_v_shape);
 
-      /* "View.MemoryView":829
+      /* "View.MemoryView":831
  *     if not is_slice:
  * 
  *         if start < 0:             # <<<<<<<<<<<<<<
  *             start += shape
  *         if not 0 <= start < shape:
  */
     }
 
-    /* "View.MemoryView":831
+    /* "View.MemoryView":833
  *         if start < 0:
  *             start += shape
  *         if not 0 <= start < shape:             # <<<<<<<<<<<<<<
  *             _err_dim(IndexError, "Index out of bounds (axis %d)", dim)
  *     else:
  */
-    __Pyx_TraceLine(831,1,__PYX_ERR(2, 831, __pyx_L1_error))
+    __Pyx_TraceLine(833,1,__PYX_ERR(2, 833, __pyx_L1_error))
     __pyx_t_1 = (0 <= __pyx_v_start);
     if (__pyx_t_1) {
       __pyx_t_1 = (__pyx_v_start < __pyx_v_shape);
     }
     __pyx_t_2 = ((!(__pyx_t_1 != 0)) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":832
+      /* "View.MemoryView":834
  *             start += shape
  *         if not 0 <= start < shape:
  *             _err_dim(IndexError, "Index out of bounds (axis %d)", dim)             # <<<<<<<<<<<<<<
  *     else:
  * 
  */
-      __Pyx_TraceLine(832,1,__PYX_ERR(2, 832, __pyx_L1_error))
-      __pyx_t_3 = __pyx_memoryview_err_dim(__pyx_builtin_IndexError, ((char *)"Index out of bounds (axis %d)"), __pyx_v_dim); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(2, 832, __pyx_L1_error)
+      __Pyx_TraceLine(834,1,__PYX_ERR(2, 834, __pyx_L1_error))
+      __pyx_t_3 = __pyx_memoryview_err_dim(__pyx_builtin_IndexError, ((char *)"Index out of bounds (axis %d)"), __pyx_v_dim); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(2, 834, __pyx_L1_error)
 
-      /* "View.MemoryView":831
+      /* "View.MemoryView":833
  *         if start < 0:
  *             start += shape
  *         if not 0 <= start < shape:             # <<<<<<<<<<<<<<
  *             _err_dim(IndexError, "Index out of bounds (axis %d)", dim)
  *     else:
  */
     }
 
-    /* "View.MemoryView":827
+    /* "View.MemoryView":829
  *     cdef bint negative_step
  * 
  *     if not is_slice:             # <<<<<<<<<<<<<<
  * 
  *         if start < 0:
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":835
+  /* "View.MemoryView":837
  *     else:
  * 
  *         negative_step = have_step != 0 and step < 0             # <<<<<<<<<<<<<<
  * 
  *         if have_step and step == 0:
  */
-  __Pyx_TraceLine(835,1,__PYX_ERR(2, 835, __pyx_L1_error))
+  __Pyx_TraceLine(837,1,__PYX_ERR(2, 837, __pyx_L1_error))
   /*else*/ {
     __pyx_t_1 = ((__pyx_v_have_step != 0) != 0);
     if (__pyx_t_1) {
     } else {
       __pyx_t_2 = __pyx_t_1;
       goto __pyx_L6_bool_binop_done;
     }
     __pyx_t_1 = ((__pyx_v_step < 0) != 0);
     __pyx_t_2 = __pyx_t_1;
     __pyx_L6_bool_binop_done:;
     __pyx_v_negative_step = __pyx_t_2;
 
-    /* "View.MemoryView":837
+    /* "View.MemoryView":839
  *         negative_step = have_step != 0 and step < 0
  * 
  *         if have_step and step == 0:             # <<<<<<<<<<<<<<
  *             _err_dim(ValueError, "Step may not be zero (axis %d)", dim)
  * 
  */
-    __Pyx_TraceLine(837,1,__PYX_ERR(2, 837, __pyx_L1_error))
+    __Pyx_TraceLine(839,1,__PYX_ERR(2, 839, __pyx_L1_error))
     __pyx_t_1 = (__pyx_v_have_step != 0);
     if (__pyx_t_1) {
     } else {
       __pyx_t_2 = __pyx_t_1;
       goto __pyx_L9_bool_binop_done;
     }
     __pyx_t_1 = ((__pyx_v_step == 0) != 0);
     __pyx_t_2 = __pyx_t_1;
     __pyx_L9_bool_binop_done:;
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":838
+      /* "View.MemoryView":840
  * 
  *         if have_step and step == 0:
  *             _err_dim(ValueError, "Step may not be zero (axis %d)", dim)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-      __Pyx_TraceLine(838,1,__PYX_ERR(2, 838, __pyx_L1_error))
-      __pyx_t_3 = __pyx_memoryview_err_dim(__pyx_builtin_ValueError, ((char *)"Step may not be zero (axis %d)"), __pyx_v_dim); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(2, 838, __pyx_L1_error)
+      __Pyx_TraceLine(840,1,__PYX_ERR(2, 840, __pyx_L1_error))
+      __pyx_t_3 = __pyx_memoryview_err_dim(__pyx_builtin_ValueError, ((char *)"Step may not be zero (axis %d)"), __pyx_v_dim); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(2, 840, __pyx_L1_error)
 
-      /* "View.MemoryView":837
+      /* "View.MemoryView":839
  *         negative_step = have_step != 0 and step < 0
  * 
  *         if have_step and step == 0:             # <<<<<<<<<<<<<<
  *             _err_dim(ValueError, "Step may not be zero (axis %d)", dim)
  * 
  */
     }
 
-    /* "View.MemoryView":841
+    /* "View.MemoryView":843
  * 
  * 
  *         if have_start:             # <<<<<<<<<<<<<<
  *             if start < 0:
  *                 start += shape
  */
-    __Pyx_TraceLine(841,1,__PYX_ERR(2, 841, __pyx_L1_error))
+    __Pyx_TraceLine(843,1,__PYX_ERR(2, 843, __pyx_L1_error))
     __pyx_t_2 = (__pyx_v_have_start != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":842
+      /* "View.MemoryView":844
  * 
  *         if have_start:
  *             if start < 0:             # <<<<<<<<<<<<<<
  *                 start += shape
  *                 if start < 0:
  */
-      __Pyx_TraceLine(842,1,__PYX_ERR(2, 842, __pyx_L1_error))
+      __Pyx_TraceLine(844,1,__PYX_ERR(2, 844, __pyx_L1_error))
       __pyx_t_2 = ((__pyx_v_start < 0) != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":843
+        /* "View.MemoryView":845
  *         if have_start:
  *             if start < 0:
  *                 start += shape             # <<<<<<<<<<<<<<
  *                 if start < 0:
  *                     start = 0
  */
-        __Pyx_TraceLine(843,1,__PYX_ERR(2, 843, __pyx_L1_error))
+        __Pyx_TraceLine(845,1,__PYX_ERR(2, 845, __pyx_L1_error))
         __pyx_v_start = (__pyx_v_start + __pyx_v_shape);
 
-        /* "View.MemoryView":844
+        /* "View.MemoryView":846
  *             if start < 0:
  *                 start += shape
  *                 if start < 0:             # <<<<<<<<<<<<<<
  *                     start = 0
  *             elif start >= shape:
  */
-        __Pyx_TraceLine(844,1,__PYX_ERR(2, 844, __pyx_L1_error))
+        __Pyx_TraceLine(846,1,__PYX_ERR(2, 846, __pyx_L1_error))
         __pyx_t_2 = ((__pyx_v_start < 0) != 0);
         if (__pyx_t_2) {
 
-          /* "View.MemoryView":845
+          /* "View.MemoryView":847
  *                 start += shape
  *                 if start < 0:
  *                     start = 0             # <<<<<<<<<<<<<<
  *             elif start >= shape:
  *                 if negative_step:
  */
-          __Pyx_TraceLine(845,1,__PYX_ERR(2, 845, __pyx_L1_error))
+          __Pyx_TraceLine(847,1,__PYX_ERR(2, 847, __pyx_L1_error))
           __pyx_v_start = 0;
 
-          /* "View.MemoryView":844
+          /* "View.MemoryView":846
  *             if start < 0:
  *                 start += shape
  *                 if start < 0:             # <<<<<<<<<<<<<<
  *                     start = 0
  *             elif start >= shape:
  */
         }
 
-        /* "View.MemoryView":842
+        /* "View.MemoryView":844
  * 
  *         if have_start:
  *             if start < 0:             # <<<<<<<<<<<<<<
  *                 start += shape
  *                 if start < 0:
  */
         goto __pyx_L12;
       }
 
-      /* "View.MemoryView":846
+      /* "View.MemoryView":848
  *                 if start < 0:
  *                     start = 0
  *             elif start >= shape:             # <<<<<<<<<<<<<<
  *                 if negative_step:
  *                     start = shape - 1
  */
-      __Pyx_TraceLine(846,1,__PYX_ERR(2, 846, __pyx_L1_error))
+      __Pyx_TraceLine(848,1,__PYX_ERR(2, 848, __pyx_L1_error))
       __pyx_t_2 = ((__pyx_v_start >= __pyx_v_shape) != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":847
+        /* "View.MemoryView":849
  *                     start = 0
  *             elif start >= shape:
  *                 if negative_step:             # <<<<<<<<<<<<<<
  *                     start = shape - 1
  *                 else:
  */
-        __Pyx_TraceLine(847,1,__PYX_ERR(2, 847, __pyx_L1_error))
+        __Pyx_TraceLine(849,1,__PYX_ERR(2, 849, __pyx_L1_error))
         __pyx_t_2 = (__pyx_v_negative_step != 0);
         if (__pyx_t_2) {
 
-          /* "View.MemoryView":848
+          /* "View.MemoryView":850
  *             elif start >= shape:
  *                 if negative_step:
  *                     start = shape - 1             # <<<<<<<<<<<<<<
  *                 else:
  *                     start = shape
  */
-          __Pyx_TraceLine(848,1,__PYX_ERR(2, 848, __pyx_L1_error))
+          __Pyx_TraceLine(850,1,__PYX_ERR(2, 850, __pyx_L1_error))
           __pyx_v_start = (__pyx_v_shape - 1);
 
-          /* "View.MemoryView":847
+          /* "View.MemoryView":849
  *                     start = 0
  *             elif start >= shape:
  *                 if negative_step:             # <<<<<<<<<<<<<<
  *                     start = shape - 1
  *                 else:
  */
           goto __pyx_L14;
         }
 
-        /* "View.MemoryView":850
+        /* "View.MemoryView":852
  *                     start = shape - 1
  *                 else:
  *                     start = shape             # <<<<<<<<<<<<<<
  *         else:
  *             if negative_step:
  */
-        __Pyx_TraceLine(850,1,__PYX_ERR(2, 850, __pyx_L1_error))
+        __Pyx_TraceLine(852,1,__PYX_ERR(2, 852, __pyx_L1_error))
         /*else*/ {
           __pyx_v_start = __pyx_v_shape;
         }
         __pyx_L14:;
 
-        /* "View.MemoryView":846
+        /* "View.MemoryView":848
  *                 if start < 0:
  *                     start = 0
  *             elif start >= shape:             # <<<<<<<<<<<<<<
  *                 if negative_step:
  *                     start = shape - 1
  */
       }
       __pyx_L12:;
 
-      /* "View.MemoryView":841
+      /* "View.MemoryView":843
  * 
  * 
  *         if have_start:             # <<<<<<<<<<<<<<
  *             if start < 0:
  *                 start += shape
  */
       goto __pyx_L11;
     }
 
-    /* "View.MemoryView":852
+    /* "View.MemoryView":854
  *                     start = shape
  *         else:
  *             if negative_step:             # <<<<<<<<<<<<<<
  *                 start = shape - 1
  *             else:
  */
-    __Pyx_TraceLine(852,1,__PYX_ERR(2, 852, __pyx_L1_error))
+    __Pyx_TraceLine(854,1,__PYX_ERR(2, 854, __pyx_L1_error))
     /*else*/ {
       __pyx_t_2 = (__pyx_v_negative_step != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":853
+        /* "View.MemoryView":855
  *         else:
  *             if negative_step:
  *                 start = shape - 1             # <<<<<<<<<<<<<<
  *             else:
  *                 start = 0
  */
-        __Pyx_TraceLine(853,1,__PYX_ERR(2, 853, __pyx_L1_error))
+        __Pyx_TraceLine(855,1,__PYX_ERR(2, 855, __pyx_L1_error))
         __pyx_v_start = (__pyx_v_shape - 1);
 
-        /* "View.MemoryView":852
+        /* "View.MemoryView":854
  *                     start = shape
  *         else:
  *             if negative_step:             # <<<<<<<<<<<<<<
  *                 start = shape - 1
  *             else:
  */
         goto __pyx_L15;
       }
 
-      /* "View.MemoryView":855
+      /* "View.MemoryView":857
  *                 start = shape - 1
  *             else:
  *                 start = 0             # <<<<<<<<<<<<<<
  * 
  *         if have_stop:
  */
-      __Pyx_TraceLine(855,1,__PYX_ERR(2, 855, __pyx_L1_error))
+      __Pyx_TraceLine(857,1,__PYX_ERR(2, 857, __pyx_L1_error))
       /*else*/ {
         __pyx_v_start = 0;
       }
       __pyx_L15:;
     }
     __pyx_L11:;
 
-    /* "View.MemoryView":857
+    /* "View.MemoryView":859
  *                 start = 0
  * 
  *         if have_stop:             # <<<<<<<<<<<<<<
  *             if stop < 0:
  *                 stop += shape
  */
-    __Pyx_TraceLine(857,1,__PYX_ERR(2, 857, __pyx_L1_error))
+    __Pyx_TraceLine(859,1,__PYX_ERR(2, 859, __pyx_L1_error))
     __pyx_t_2 = (__pyx_v_have_stop != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":858
+      /* "View.MemoryView":860
  * 
  *         if have_stop:
  *             if stop < 0:             # <<<<<<<<<<<<<<
  *                 stop += shape
  *                 if stop < 0:
  */
-      __Pyx_TraceLine(858,1,__PYX_ERR(2, 858, __pyx_L1_error))
+      __Pyx_TraceLine(860,1,__PYX_ERR(2, 860, __pyx_L1_error))
       __pyx_t_2 = ((__pyx_v_stop < 0) != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":859
+        /* "View.MemoryView":861
  *         if have_stop:
  *             if stop < 0:
  *                 stop += shape             # <<<<<<<<<<<<<<
  *                 if stop < 0:
  *                     stop = 0
  */
-        __Pyx_TraceLine(859,1,__PYX_ERR(2, 859, __pyx_L1_error))
+        __Pyx_TraceLine(861,1,__PYX_ERR(2, 861, __pyx_L1_error))
         __pyx_v_stop = (__pyx_v_stop + __pyx_v_shape);
 
-        /* "View.MemoryView":860
+        /* "View.MemoryView":862
  *             if stop < 0:
  *                 stop += shape
  *                 if stop < 0:             # <<<<<<<<<<<<<<
  *                     stop = 0
  *             elif stop > shape:
  */
-        __Pyx_TraceLine(860,1,__PYX_ERR(2, 860, __pyx_L1_error))
+        __Pyx_TraceLine(862,1,__PYX_ERR(2, 862, __pyx_L1_error))
         __pyx_t_2 = ((__pyx_v_stop < 0) != 0);
         if (__pyx_t_2) {
 
-          /* "View.MemoryView":861
+          /* "View.MemoryView":863
  *                 stop += shape
  *                 if stop < 0:
  *                     stop = 0             # <<<<<<<<<<<<<<
  *             elif stop > shape:
  *                 stop = shape
  */
-          __Pyx_TraceLine(861,1,__PYX_ERR(2, 861, __pyx_L1_error))
+          __Pyx_TraceLine(863,1,__PYX_ERR(2, 863, __pyx_L1_error))
           __pyx_v_stop = 0;
 
-          /* "View.MemoryView":860
+          /* "View.MemoryView":862
  *             if stop < 0:
  *                 stop += shape
  *                 if stop < 0:             # <<<<<<<<<<<<<<
  *                     stop = 0
  *             elif stop > shape:
  */
         }
 
-        /* "View.MemoryView":858
+        /* "View.MemoryView":860
  * 
  *         if have_stop:
  *             if stop < 0:             # <<<<<<<<<<<<<<
  *                 stop += shape
  *                 if stop < 0:
  */
         goto __pyx_L17;
       }
 
-      /* "View.MemoryView":862
+      /* "View.MemoryView":864
  *                 if stop < 0:
  *                     stop = 0
  *             elif stop > shape:             # <<<<<<<<<<<<<<
  *                 stop = shape
  *         else:
  */
-      __Pyx_TraceLine(862,1,__PYX_ERR(2, 862, __pyx_L1_error))
+      __Pyx_TraceLine(864,1,__PYX_ERR(2, 864, __pyx_L1_error))
       __pyx_t_2 = ((__pyx_v_stop > __pyx_v_shape) != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":863
+        /* "View.MemoryView":865
  *                     stop = 0
  *             elif stop > shape:
  *                 stop = shape             # <<<<<<<<<<<<<<
  *         else:
  *             if negative_step:
  */
-        __Pyx_TraceLine(863,1,__PYX_ERR(2, 863, __pyx_L1_error))
+        __Pyx_TraceLine(865,1,__PYX_ERR(2, 865, __pyx_L1_error))
         __pyx_v_stop = __pyx_v_shape;
 
-        /* "View.MemoryView":862
+        /* "View.MemoryView":864
  *                 if stop < 0:
  *                     stop = 0
  *             elif stop > shape:             # <<<<<<<<<<<<<<
  *                 stop = shape
  *         else:
  */
       }
       __pyx_L17:;
 
-      /* "View.MemoryView":857
+      /* "View.MemoryView":859
  *                 start = 0
  * 
  *         if have_stop:             # <<<<<<<<<<<<<<
  *             if stop < 0:
  *                 stop += shape
  */
       goto __pyx_L16;
     }
 
-    /* "View.MemoryView":865
+    /* "View.MemoryView":867
  *                 stop = shape
  *         else:
  *             if negative_step:             # <<<<<<<<<<<<<<
  *                 stop = -1
  *             else:
  */
-    __Pyx_TraceLine(865,1,__PYX_ERR(2, 865, __pyx_L1_error))
+    __Pyx_TraceLine(867,1,__PYX_ERR(2, 867, __pyx_L1_error))
     /*else*/ {
       __pyx_t_2 = (__pyx_v_negative_step != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":866
+        /* "View.MemoryView":868
  *         else:
  *             if negative_step:
  *                 stop = -1             # <<<<<<<<<<<<<<
  *             else:
  *                 stop = shape
  */
-        __Pyx_TraceLine(866,1,__PYX_ERR(2, 866, __pyx_L1_error))
+        __Pyx_TraceLine(868,1,__PYX_ERR(2, 868, __pyx_L1_error))
         __pyx_v_stop = -1L;
 
-        /* "View.MemoryView":865
+        /* "View.MemoryView":867
  *                 stop = shape
  *         else:
  *             if negative_step:             # <<<<<<<<<<<<<<
  *                 stop = -1
  *             else:
  */
         goto __pyx_L19;
       }
 
-      /* "View.MemoryView":868
+      /* "View.MemoryView":870
  *                 stop = -1
  *             else:
  *                 stop = shape             # <<<<<<<<<<<<<<
  * 
  *         if not have_step:
  */
-      __Pyx_TraceLine(868,1,__PYX_ERR(2, 868, __pyx_L1_error))
+      __Pyx_TraceLine(870,1,__PYX_ERR(2, 870, __pyx_L1_error))
       /*else*/ {
         __pyx_v_stop = __pyx_v_shape;
       }
       __pyx_L19:;
     }
     __pyx_L16:;
 
-    /* "View.MemoryView":870
+    /* "View.MemoryView":872
  *                 stop = shape
  * 
  *         if not have_step:             # <<<<<<<<<<<<<<
  *             step = 1
  * 
  */
-    __Pyx_TraceLine(870,1,__PYX_ERR(2, 870, __pyx_L1_error))
+    __Pyx_TraceLine(872,1,__PYX_ERR(2, 872, __pyx_L1_error))
     __pyx_t_2 = ((!(__pyx_v_have_step != 0)) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":871
+      /* "View.MemoryView":873
  * 
  *         if not have_step:
  *             step = 1             # <<<<<<<<<<<<<<
  * 
  * 
  */
-      __Pyx_TraceLine(871,1,__PYX_ERR(2, 871, __pyx_L1_error))
+      __Pyx_TraceLine(873,1,__PYX_ERR(2, 873, __pyx_L1_error))
       __pyx_v_step = 1;
 
-      /* "View.MemoryView":870
+      /* "View.MemoryView":872
  *                 stop = shape
  * 
  *         if not have_step:             # <<<<<<<<<<<<<<
  *             step = 1
  * 
  */
     }
 
-    /* "View.MemoryView":875
+    /* "View.MemoryView":877
  * 
  *         with cython.cdivision(True):
  *             new_shape = (stop - start) // step             # <<<<<<<<<<<<<<
  * 
  *             if (stop - start) - step * new_shape:
  */
     __pyx_v_new_shape = ((__pyx_v_stop - __pyx_v_start) / __pyx_v_step);
 
-    /* "View.MemoryView":877
+    /* "View.MemoryView":879
  *             new_shape = (stop - start) // step
  * 
  *             if (stop - start) - step * new_shape:             # <<<<<<<<<<<<<<
  *                 new_shape += 1
  * 
  */
     __pyx_t_2 = (((__pyx_v_stop - __pyx_v_start) - (__pyx_v_step * __pyx_v_new_shape)) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":878
+      /* "View.MemoryView":880
  * 
  *             if (stop - start) - step * new_shape:
  *                 new_shape += 1             # <<<<<<<<<<<<<<
  * 
  *         if new_shape < 0:
  */
       __pyx_v_new_shape = (__pyx_v_new_shape + 1);
 
-      /* "View.MemoryView":877
+      /* "View.MemoryView":879
  *             new_shape = (stop - start) // step
  * 
  *             if (stop - start) - step * new_shape:             # <<<<<<<<<<<<<<
  *                 new_shape += 1
  * 
  */
     }
 
-    /* "View.MemoryView":880
+    /* "View.MemoryView":882
  *                 new_shape += 1
  * 
  *         if new_shape < 0:             # <<<<<<<<<<<<<<
  *             new_shape = 0
  * 
  */
-    __Pyx_TraceLine(880,1,__PYX_ERR(2, 880, __pyx_L1_error))
+    __Pyx_TraceLine(882,1,__PYX_ERR(2, 882, __pyx_L1_error))
     __pyx_t_2 = ((__pyx_v_new_shape < 0) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":881
+      /* "View.MemoryView":883
  * 
  *         if new_shape < 0:
  *             new_shape = 0             # <<<<<<<<<<<<<<
  * 
  * 
  */
-      __Pyx_TraceLine(881,1,__PYX_ERR(2, 881, __pyx_L1_error))
+      __Pyx_TraceLine(883,1,__PYX_ERR(2, 883, __pyx_L1_error))
       __pyx_v_new_shape = 0;
 
-      /* "View.MemoryView":880
+      /* "View.MemoryView":882
  *                 new_shape += 1
  * 
  *         if new_shape < 0:             # <<<<<<<<<<<<<<
  *             new_shape = 0
  * 
  */
     }
 
-    /* "View.MemoryView":884
+    /* "View.MemoryView":886
  * 
  * 
  *         dst.strides[new_ndim] = stride * step             # <<<<<<<<<<<<<<
  *         dst.shape[new_ndim] = new_shape
  *         dst.suboffsets[new_ndim] = suboffset
  */
-    __Pyx_TraceLine(884,1,__PYX_ERR(2, 884, __pyx_L1_error))
+    __Pyx_TraceLine(886,1,__PYX_ERR(2, 886, __pyx_L1_error))
     (__pyx_v_dst->strides[__pyx_v_new_ndim]) = (__pyx_v_stride * __pyx_v_step);
 
-    /* "View.MemoryView":885
+    /* "View.MemoryView":887
  * 
  *         dst.strides[new_ndim] = stride * step
  *         dst.shape[new_ndim] = new_shape             # <<<<<<<<<<<<<<
  *         dst.suboffsets[new_ndim] = suboffset
  * 
  */
-    __Pyx_TraceLine(885,1,__PYX_ERR(2, 885, __pyx_L1_error))
+    __Pyx_TraceLine(887,1,__PYX_ERR(2, 887, __pyx_L1_error))
     (__pyx_v_dst->shape[__pyx_v_new_ndim]) = __pyx_v_new_shape;
 
-    /* "View.MemoryView":886
+    /* "View.MemoryView":888
  *         dst.strides[new_ndim] = stride * step
  *         dst.shape[new_ndim] = new_shape
  *         dst.suboffsets[new_ndim] = suboffset             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __Pyx_TraceLine(886,1,__PYX_ERR(2, 886, __pyx_L1_error))
+    __Pyx_TraceLine(888,1,__PYX_ERR(2, 888, __pyx_L1_error))
     (__pyx_v_dst->suboffsets[__pyx_v_new_ndim]) = __pyx_v_suboffset;
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":889
+  /* "View.MemoryView":891
  * 
  * 
  *     if suboffset_dim[0] < 0:             # <<<<<<<<<<<<<<
  *         dst.data += start * stride
  *     else:
  */
-  __Pyx_TraceLine(889,1,__PYX_ERR(2, 889, __pyx_L1_error))
+  __Pyx_TraceLine(891,1,__PYX_ERR(2, 891, __pyx_L1_error))
   __pyx_t_2 = (((__pyx_v_suboffset_dim[0]) < 0) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":890
+    /* "View.MemoryView":892
  * 
  *     if suboffset_dim[0] < 0:
  *         dst.data += start * stride             # <<<<<<<<<<<<<<
  *     else:
  *         dst.suboffsets[suboffset_dim[0]] += start * stride
  */
-    __Pyx_TraceLine(890,1,__PYX_ERR(2, 890, __pyx_L1_error))
+    __Pyx_TraceLine(892,1,__PYX_ERR(2, 892, __pyx_L1_error))
     __pyx_v_dst->data = (__pyx_v_dst->data + (__pyx_v_start * __pyx_v_stride));
 
-    /* "View.MemoryView":889
+    /* "View.MemoryView":891
  * 
  * 
  *     if suboffset_dim[0] < 0:             # <<<<<<<<<<<<<<
  *         dst.data += start * stride
  *     else:
  */
     goto __pyx_L23;
   }
 
-  /* "View.MemoryView":892
+  /* "View.MemoryView":894
  *         dst.data += start * stride
  *     else:
  *         dst.suboffsets[suboffset_dim[0]] += start * stride             # <<<<<<<<<<<<<<
  * 
  *     if suboffset >= 0:
  */
-  __Pyx_TraceLine(892,1,__PYX_ERR(2, 892, __pyx_L1_error))
+  __Pyx_TraceLine(894,1,__PYX_ERR(2, 894, __pyx_L1_error))
   /*else*/ {
     __pyx_t_3 = (__pyx_v_suboffset_dim[0]);
     (__pyx_v_dst->suboffsets[__pyx_t_3]) = ((__pyx_v_dst->suboffsets[__pyx_t_3]) + (__pyx_v_start * __pyx_v_stride));
   }
   __pyx_L23:;
 
-  /* "View.MemoryView":894
+  /* "View.MemoryView":896
  *         dst.suboffsets[suboffset_dim[0]] += start * stride
  * 
  *     if suboffset >= 0:             # <<<<<<<<<<<<<<
  *         if not is_slice:
  *             if new_ndim == 0:
  */
-  __Pyx_TraceLine(894,1,__PYX_ERR(2, 894, __pyx_L1_error))
+  __Pyx_TraceLine(896,1,__PYX_ERR(2, 896, __pyx_L1_error))
   __pyx_t_2 = ((__pyx_v_suboffset >= 0) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":895
+    /* "View.MemoryView":897
  * 
  *     if suboffset >= 0:
  *         if not is_slice:             # <<<<<<<<<<<<<<
  *             if new_ndim == 0:
  *                 dst.data = (<char **> dst.data)[0] + suboffset
  */
-    __Pyx_TraceLine(895,1,__PYX_ERR(2, 895, __pyx_L1_error))
+    __Pyx_TraceLine(897,1,__PYX_ERR(2, 897, __pyx_L1_error))
     __pyx_t_2 = ((!(__pyx_v_is_slice != 0)) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":896
+      /* "View.MemoryView":898
  *     if suboffset >= 0:
  *         if not is_slice:
  *             if new_ndim == 0:             # <<<<<<<<<<<<<<
  *                 dst.data = (<char **> dst.data)[0] + suboffset
  *             else:
  */
-      __Pyx_TraceLine(896,1,__PYX_ERR(2, 896, __pyx_L1_error))
+      __Pyx_TraceLine(898,1,__PYX_ERR(2, 898, __pyx_L1_error))
       __pyx_t_2 = ((__pyx_v_new_ndim == 0) != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":897
+        /* "View.MemoryView":899
  *         if not is_slice:
  *             if new_ndim == 0:
  *                 dst.data = (<char **> dst.data)[0] + suboffset             # <<<<<<<<<<<<<<
  *             else:
  *                 _err_dim(IndexError, "All dimensions preceding dimension %d "
  */
-        __Pyx_TraceLine(897,1,__PYX_ERR(2, 897, __pyx_L1_error))
+        __Pyx_TraceLine(899,1,__PYX_ERR(2, 899, __pyx_L1_error))
         __pyx_v_dst->data = ((((char **)__pyx_v_dst->data)[0]) + __pyx_v_suboffset);
 
-        /* "View.MemoryView":896
+        /* "View.MemoryView":898
  *     if suboffset >= 0:
  *         if not is_slice:
  *             if new_ndim == 0:             # <<<<<<<<<<<<<<
  *                 dst.data = (<char **> dst.data)[0] + suboffset
  *             else:
  */
         goto __pyx_L26;
       }
 
-      /* "View.MemoryView":899
+      /* "View.MemoryView":901
  *                 dst.data = (<char **> dst.data)[0] + suboffset
  *             else:
  *                 _err_dim(IndexError, "All dimensions preceding dimension %d "             # <<<<<<<<<<<<<<
  *                                      "must be indexed and not sliced", dim)
  *         else:
  */
-      __Pyx_TraceLine(899,1,__PYX_ERR(2, 899, __pyx_L1_error))
+      __Pyx_TraceLine(901,1,__PYX_ERR(2, 901, __pyx_L1_error))
       /*else*/ {
 
-        /* "View.MemoryView":900
+        /* "View.MemoryView":902
  *             else:
  *                 _err_dim(IndexError, "All dimensions preceding dimension %d "
  *                                      "must be indexed and not sliced", dim)             # <<<<<<<<<<<<<<
  *         else:
  *             suboffset_dim[0] = new_ndim
  */
-        __Pyx_TraceLine(900,1,__PYX_ERR(2, 900, __pyx_L1_error))
-        __pyx_t_3 = __pyx_memoryview_err_dim(__pyx_builtin_IndexError, ((char *)"All dimensions preceding dimension %d must be indexed and not sliced"), __pyx_v_dim); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(2, 899, __pyx_L1_error)
+        __Pyx_TraceLine(902,1,__PYX_ERR(2, 902, __pyx_L1_error))
+        __pyx_t_3 = __pyx_memoryview_err_dim(__pyx_builtin_IndexError, ((char *)"All dimensions preceding dimension %d must be indexed and not sliced"), __pyx_v_dim); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(2, 901, __pyx_L1_error)
       }
       __pyx_L26:;
 
-      /* "View.MemoryView":895
+      /* "View.MemoryView":897
  * 
  *     if suboffset >= 0:
  *         if not is_slice:             # <<<<<<<<<<<<<<
  *             if new_ndim == 0:
  *                 dst.data = (<char **> dst.data)[0] + suboffset
  */
       goto __pyx_L25;
     }
 
-    /* "View.MemoryView":902
+    /* "View.MemoryView":904
  *                                      "must be indexed and not sliced", dim)
  *         else:
  *             suboffset_dim[0] = new_ndim             # <<<<<<<<<<<<<<
  * 
  *     return 0
  */
-    __Pyx_TraceLine(902,1,__PYX_ERR(2, 902, __pyx_L1_error))
+    __Pyx_TraceLine(904,1,__PYX_ERR(2, 904, __pyx_L1_error))
     /*else*/ {
       (__pyx_v_suboffset_dim[0]) = __pyx_v_new_ndim;
     }
     __pyx_L25:;
 
-    /* "View.MemoryView":894
+    /* "View.MemoryView":896
  *         dst.suboffsets[suboffset_dim[0]] += start * stride
  * 
  *     if suboffset >= 0:             # <<<<<<<<<<<<<<
  *         if not is_slice:
  *             if new_ndim == 0:
  */
   }
 
-  /* "View.MemoryView":904
+  /* "View.MemoryView":906
  *             suboffset_dim[0] = new_ndim
  * 
  *     return 0             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_TraceLine(904,1,__PYX_ERR(2, 904, __pyx_L1_error))
+  __Pyx_TraceLine(906,1,__PYX_ERR(2, 906, __pyx_L1_error))
   __pyx_r = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":807
+  /* "View.MemoryView":809
  * 
  * @cname('__pyx_memoryview_slice_memviewslice')
  * cdef int slice_memviewslice(             # <<<<<<<<<<<<<<
  *         __Pyx_memviewslice *dst,
  *         Py_ssize_t shape, Py_ssize_t stride, Py_ssize_t suboffset,
  */
 
@@ -25650,15 +25844,15 @@
   }
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
   return __pyx_r;
 }
 
-/* "View.MemoryView":910
+/* "View.MemoryView":912
  * 
  * @cname('__pyx_pybuffer_index')
  * cdef char *pybuffer_index(Py_buffer *view, char *bufp, Py_ssize_t index,             # <<<<<<<<<<<<<<
  *                           Py_ssize_t dim) except NULL:
  *     cdef Py_ssize_t shape, stride, suboffset = -1
  */
 
@@ -25675,301 +25869,301 @@
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("pybuffer_index", 0);
-  __Pyx_TraceCall("pybuffer_index", __pyx_f[2], 910, 0, __PYX_ERR(2, 910, __pyx_L1_error));
+  __Pyx_TraceCall("pybuffer_index", __pyx_f[2], 912, 0, __PYX_ERR(2, 912, __pyx_L1_error));
 
-  /* "View.MemoryView":912
+  /* "View.MemoryView":914
  * cdef char *pybuffer_index(Py_buffer *view, char *bufp, Py_ssize_t index,
  *                           Py_ssize_t dim) except NULL:
  *     cdef Py_ssize_t shape, stride, suboffset = -1             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t itemsize = view.itemsize
  *     cdef char *resultp
  */
-  __Pyx_TraceLine(912,0,__PYX_ERR(2, 912, __pyx_L1_error))
+  __Pyx_TraceLine(914,0,__PYX_ERR(2, 914, __pyx_L1_error))
   __pyx_v_suboffset = -1L;
 
-  /* "View.MemoryView":913
+  /* "View.MemoryView":915
  *                           Py_ssize_t dim) except NULL:
  *     cdef Py_ssize_t shape, stride, suboffset = -1
  *     cdef Py_ssize_t itemsize = view.itemsize             # <<<<<<<<<<<<<<
  *     cdef char *resultp
  * 
  */
-  __Pyx_TraceLine(913,0,__PYX_ERR(2, 913, __pyx_L1_error))
+  __Pyx_TraceLine(915,0,__PYX_ERR(2, 915, __pyx_L1_error))
   __pyx_t_1 = __pyx_v_view->itemsize;
   __pyx_v_itemsize = __pyx_t_1;
 
-  /* "View.MemoryView":916
+  /* "View.MemoryView":918
  *     cdef char *resultp
  * 
  *     if view.ndim == 0:             # <<<<<<<<<<<<<<
  *         shape = view.len / itemsize
  *         stride = itemsize
  */
-  __Pyx_TraceLine(916,0,__PYX_ERR(2, 916, __pyx_L1_error))
+  __Pyx_TraceLine(918,0,__PYX_ERR(2, 918, __pyx_L1_error))
   __pyx_t_2 = ((__pyx_v_view->ndim == 0) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":917
+    /* "View.MemoryView":919
  * 
  *     if view.ndim == 0:
  *         shape = view.len / itemsize             # <<<<<<<<<<<<<<
  *         stride = itemsize
  *     else:
  */
-    __Pyx_TraceLine(917,0,__PYX_ERR(2, 917, __pyx_L1_error))
+    __Pyx_TraceLine(919,0,__PYX_ERR(2, 919, __pyx_L1_error))
     if (unlikely(__pyx_v_itemsize == 0)) {
       PyErr_SetString(PyExc_ZeroDivisionError, "integer division or modulo by zero");
-      __PYX_ERR(2, 917, __pyx_L1_error)
+      __PYX_ERR(2, 919, __pyx_L1_error)
     }
     else if (sizeof(Py_ssize_t) == sizeof(long) && (!(((Py_ssize_t)-1) > 0)) && unlikely(__pyx_v_itemsize == (Py_ssize_t)-1)  && unlikely(UNARY_NEG_WOULD_OVERFLOW(__pyx_v_view->len))) {
       PyErr_SetString(PyExc_OverflowError, "value too large to perform division");
-      __PYX_ERR(2, 917, __pyx_L1_error)
+      __PYX_ERR(2, 919, __pyx_L1_error)
     }
     __pyx_v_shape = (__pyx_v_view->len / __pyx_v_itemsize);
 
-    /* "View.MemoryView":918
+    /* "View.MemoryView":920
  *     if view.ndim == 0:
  *         shape = view.len / itemsize
  *         stride = itemsize             # <<<<<<<<<<<<<<
  *     else:
  *         shape = view.shape[dim]
  */
-    __Pyx_TraceLine(918,0,__PYX_ERR(2, 918, __pyx_L1_error))
+    __Pyx_TraceLine(920,0,__PYX_ERR(2, 920, __pyx_L1_error))
     __pyx_v_stride = __pyx_v_itemsize;
 
-    /* "View.MemoryView":916
+    /* "View.MemoryView":918
  *     cdef char *resultp
  * 
  *     if view.ndim == 0:             # <<<<<<<<<<<<<<
  *         shape = view.len / itemsize
  *         stride = itemsize
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":920
+  /* "View.MemoryView":922
  *         stride = itemsize
  *     else:
  *         shape = view.shape[dim]             # <<<<<<<<<<<<<<
  *         stride = view.strides[dim]
  *         if view.suboffsets != NULL:
  */
-  __Pyx_TraceLine(920,0,__PYX_ERR(2, 920, __pyx_L1_error))
+  __Pyx_TraceLine(922,0,__PYX_ERR(2, 922, __pyx_L1_error))
   /*else*/ {
     __pyx_v_shape = (__pyx_v_view->shape[__pyx_v_dim]);
 
-    /* "View.MemoryView":921
+    /* "View.MemoryView":923
  *     else:
  *         shape = view.shape[dim]
  *         stride = view.strides[dim]             # <<<<<<<<<<<<<<
  *         if view.suboffsets != NULL:
  *             suboffset = view.suboffsets[dim]
  */
-    __Pyx_TraceLine(921,0,__PYX_ERR(2, 921, __pyx_L1_error))
+    __Pyx_TraceLine(923,0,__PYX_ERR(2, 923, __pyx_L1_error))
     __pyx_v_stride = (__pyx_v_view->strides[__pyx_v_dim]);
 
-    /* "View.MemoryView":922
+    /* "View.MemoryView":924
  *         shape = view.shape[dim]
  *         stride = view.strides[dim]
  *         if view.suboffsets != NULL:             # <<<<<<<<<<<<<<
  *             suboffset = view.suboffsets[dim]
  * 
  */
-    __Pyx_TraceLine(922,0,__PYX_ERR(2, 922, __pyx_L1_error))
+    __Pyx_TraceLine(924,0,__PYX_ERR(2, 924, __pyx_L1_error))
     __pyx_t_2 = ((__pyx_v_view->suboffsets != NULL) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":923
+      /* "View.MemoryView":925
  *         stride = view.strides[dim]
  *         if view.suboffsets != NULL:
  *             suboffset = view.suboffsets[dim]             # <<<<<<<<<<<<<<
  * 
  *     if index < 0:
  */
-      __Pyx_TraceLine(923,0,__PYX_ERR(2, 923, __pyx_L1_error))
+      __Pyx_TraceLine(925,0,__PYX_ERR(2, 925, __pyx_L1_error))
       __pyx_v_suboffset = (__pyx_v_view->suboffsets[__pyx_v_dim]);
 
-      /* "View.MemoryView":922
+      /* "View.MemoryView":924
  *         shape = view.shape[dim]
  *         stride = view.strides[dim]
  *         if view.suboffsets != NULL:             # <<<<<<<<<<<<<<
  *             suboffset = view.suboffsets[dim]
  * 
  */
     }
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":925
+  /* "View.MemoryView":927
  *             suboffset = view.suboffsets[dim]
  * 
  *     if index < 0:             # <<<<<<<<<<<<<<
  *         index += view.shape[dim]
  *         if index < 0:
  */
-  __Pyx_TraceLine(925,0,__PYX_ERR(2, 925, __pyx_L1_error))
+  __Pyx_TraceLine(927,0,__PYX_ERR(2, 927, __pyx_L1_error))
   __pyx_t_2 = ((__pyx_v_index < 0) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":926
+    /* "View.MemoryView":928
  * 
  *     if index < 0:
  *         index += view.shape[dim]             # <<<<<<<<<<<<<<
  *         if index < 0:
  *             raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  */
-    __Pyx_TraceLine(926,0,__PYX_ERR(2, 926, __pyx_L1_error))
+    __Pyx_TraceLine(928,0,__PYX_ERR(2, 928, __pyx_L1_error))
     __pyx_v_index = (__pyx_v_index + (__pyx_v_view->shape[__pyx_v_dim]));
 
-    /* "View.MemoryView":927
+    /* "View.MemoryView":929
  *     if index < 0:
  *         index += view.shape[dim]
  *         if index < 0:             # <<<<<<<<<<<<<<
  *             raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  * 
  */
-    __Pyx_TraceLine(927,0,__PYX_ERR(2, 927, __pyx_L1_error))
+    __Pyx_TraceLine(929,0,__PYX_ERR(2, 929, __pyx_L1_error))
     __pyx_t_2 = ((__pyx_v_index < 0) != 0);
     if (unlikely(__pyx_t_2)) {
 
-      /* "View.MemoryView":928
+      /* "View.MemoryView":930
  *         index += view.shape[dim]
  *         if index < 0:
  *             raise IndexError("Out of bounds on buffer access (axis %d)" % dim)             # <<<<<<<<<<<<<<
  * 
  *     if index >= shape:
  */
-      __Pyx_TraceLine(928,0,__PYX_ERR(2, 928, __pyx_L1_error))
-      __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_dim); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 928, __pyx_L1_error)
+      __Pyx_TraceLine(930,0,__PYX_ERR(2, 930, __pyx_L1_error))
+      __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_dim); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 930, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Out_of_bounds_on_buffer_access_a, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 928, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Out_of_bounds_on_buffer_access_a, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 930, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_IndexError, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 928, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_IndexError, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 930, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_Raise(__pyx_t_3, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __PYX_ERR(2, 928, __pyx_L1_error)
+      __PYX_ERR(2, 930, __pyx_L1_error)
 
-      /* "View.MemoryView":927
+      /* "View.MemoryView":929
  *     if index < 0:
  *         index += view.shape[dim]
  *         if index < 0:             # <<<<<<<<<<<<<<
  *             raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  * 
  */
     }
 
-    /* "View.MemoryView":925
+    /* "View.MemoryView":927
  *             suboffset = view.suboffsets[dim]
  * 
  *     if index < 0:             # <<<<<<<<<<<<<<
  *         index += view.shape[dim]
  *         if index < 0:
  */
   }
 
-  /* "View.MemoryView":930
+  /* "View.MemoryView":932
  *             raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  * 
  *     if index >= shape:             # <<<<<<<<<<<<<<
  *         raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  * 
  */
-  __Pyx_TraceLine(930,0,__PYX_ERR(2, 930, __pyx_L1_error))
+  __Pyx_TraceLine(932,0,__PYX_ERR(2, 932, __pyx_L1_error))
   __pyx_t_2 = ((__pyx_v_index >= __pyx_v_shape) != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "View.MemoryView":931
+    /* "View.MemoryView":933
  * 
  *     if index >= shape:
  *         raise IndexError("Out of bounds on buffer access (axis %d)" % dim)             # <<<<<<<<<<<<<<
  * 
  *     resultp = bufp + index * stride
  */
-    __Pyx_TraceLine(931,0,__PYX_ERR(2, 931, __pyx_L1_error))
-    __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_dim); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 931, __pyx_L1_error)
+    __Pyx_TraceLine(933,0,__PYX_ERR(2, 933, __pyx_L1_error))
+    __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_dim); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 933, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Out_of_bounds_on_buffer_access_a, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 931, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Out_of_bounds_on_buffer_access_a, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 933, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_IndexError, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 931, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_IndexError, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 933, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(2, 931, __pyx_L1_error)
+    __PYX_ERR(2, 933, __pyx_L1_error)
 
-    /* "View.MemoryView":930
+    /* "View.MemoryView":932
  *             raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  * 
  *     if index >= shape:             # <<<<<<<<<<<<<<
  *         raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  * 
  */
   }
 
-  /* "View.MemoryView":933
+  /* "View.MemoryView":935
  *         raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  * 
  *     resultp = bufp + index * stride             # <<<<<<<<<<<<<<
  *     if suboffset >= 0:
  *         resultp = (<char **> resultp)[0] + suboffset
  */
-  __Pyx_TraceLine(933,0,__PYX_ERR(2, 933, __pyx_L1_error))
+  __Pyx_TraceLine(935,0,__PYX_ERR(2, 935, __pyx_L1_error))
   __pyx_v_resultp = (__pyx_v_bufp + (__pyx_v_index * __pyx_v_stride));
 
-  /* "View.MemoryView":934
+  /* "View.MemoryView":936
  * 
  *     resultp = bufp + index * stride
  *     if suboffset >= 0:             # <<<<<<<<<<<<<<
  *         resultp = (<char **> resultp)[0] + suboffset
  * 
  */
-  __Pyx_TraceLine(934,0,__PYX_ERR(2, 934, __pyx_L1_error))
+  __Pyx_TraceLine(936,0,__PYX_ERR(2, 936, __pyx_L1_error))
   __pyx_t_2 = ((__pyx_v_suboffset >= 0) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":935
+    /* "View.MemoryView":937
  *     resultp = bufp + index * stride
  *     if suboffset >= 0:
  *         resultp = (<char **> resultp)[0] + suboffset             # <<<<<<<<<<<<<<
  * 
  *     return resultp
  */
-    __Pyx_TraceLine(935,0,__PYX_ERR(2, 935, __pyx_L1_error))
+    __Pyx_TraceLine(937,0,__PYX_ERR(2, 937, __pyx_L1_error))
     __pyx_v_resultp = ((((char **)__pyx_v_resultp)[0]) + __pyx_v_suboffset);
 
-    /* "View.MemoryView":934
+    /* "View.MemoryView":936
  * 
  *     resultp = bufp + index * stride
  *     if suboffset >= 0:             # <<<<<<<<<<<<<<
  *         resultp = (<char **> resultp)[0] + suboffset
  * 
  */
   }
 
-  /* "View.MemoryView":937
+  /* "View.MemoryView":939
  *         resultp = (<char **> resultp)[0] + suboffset
  * 
  *     return resultp             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_TraceLine(937,0,__PYX_ERR(2, 937, __pyx_L1_error))
+  __Pyx_TraceLine(939,0,__PYX_ERR(2, 939, __pyx_L1_error))
   __pyx_r = __pyx_v_resultp;
   goto __pyx_L0;
 
-  /* "View.MemoryView":910
+  /* "View.MemoryView":912
  * 
  * @cname('__pyx_pybuffer_index')
  * cdef char *pybuffer_index(Py_buffer *view, char *bufp, Py_ssize_t index,             # <<<<<<<<<<<<<<
  *                           Py_ssize_t dim) except NULL:
  *     cdef Py_ssize_t shape, stride, suboffset = -1
  */
 
@@ -25981,15 +26175,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":943
+/* "View.MemoryView":945
  * 
  * @cname('__pyx_memslice_transpose')
  * cdef int transpose_memslice(__Pyx_memviewslice *memslice) nogil except 0:             # <<<<<<<<<<<<<<
  *     cdef int ndim = memslice.memview.view.ndim
  * 
  */
 
@@ -26009,149 +26203,149 @@
   Py_ssize_t __pyx_t_6;
   int __pyx_t_7;
   int __pyx_t_8;
   int __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_TraceCall("transpose_memslice", __pyx_f[2], 943, 1, __PYX_ERR(2, 943, __pyx_L1_error));
+  __Pyx_TraceCall("transpose_memslice", __pyx_f[2], 945, 1, __PYX_ERR(2, 945, __pyx_L1_error));
 
-  /* "View.MemoryView":944
+  /* "View.MemoryView":946
  * @cname('__pyx_memslice_transpose')
  * cdef int transpose_memslice(__Pyx_memviewslice *memslice) nogil except 0:
  *     cdef int ndim = memslice.memview.view.ndim             # <<<<<<<<<<<<<<
  * 
  *     cdef Py_ssize_t *shape = memslice.shape
  */
-  __Pyx_TraceLine(944,1,__PYX_ERR(2, 944, __pyx_L1_error))
+  __Pyx_TraceLine(946,1,__PYX_ERR(2, 946, __pyx_L1_error))
   __pyx_t_1 = __pyx_v_memslice->memview->view.ndim;
   __pyx_v_ndim = __pyx_t_1;
 
-  /* "View.MemoryView":946
+  /* "View.MemoryView":948
  *     cdef int ndim = memslice.memview.view.ndim
  * 
  *     cdef Py_ssize_t *shape = memslice.shape             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t *strides = memslice.strides
  * 
  */
-  __Pyx_TraceLine(946,1,__PYX_ERR(2, 946, __pyx_L1_error))
+  __Pyx_TraceLine(948,1,__PYX_ERR(2, 948, __pyx_L1_error))
   __pyx_t_2 = __pyx_v_memslice->shape;
   __pyx_v_shape = __pyx_t_2;
 
-  /* "View.MemoryView":947
+  /* "View.MemoryView":949
  * 
  *     cdef Py_ssize_t *shape = memslice.shape
  *     cdef Py_ssize_t *strides = memslice.strides             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_TraceLine(947,1,__PYX_ERR(2, 947, __pyx_L1_error))
+  __Pyx_TraceLine(949,1,__PYX_ERR(2, 949, __pyx_L1_error))
   __pyx_t_2 = __pyx_v_memslice->strides;
   __pyx_v_strides = __pyx_t_2;
 
-  /* "View.MemoryView":951
+  /* "View.MemoryView":953
  * 
  *     cdef int i, j
  *     for i in range(ndim / 2):             # <<<<<<<<<<<<<<
  *         j = ndim - 1 - i
  *         strides[i], strides[j] = strides[j], strides[i]
  */
-  __Pyx_TraceLine(951,1,__PYX_ERR(2, 951, __pyx_L1_error))
+  __Pyx_TraceLine(953,1,__PYX_ERR(2, 953, __pyx_L1_error))
   __pyx_t_3 = (__pyx_v_ndim / 2);
   __pyx_t_4 = __pyx_t_3;
   for (__pyx_t_1 = 0; __pyx_t_1 < __pyx_t_4; __pyx_t_1+=1) {
     __pyx_v_i = __pyx_t_1;
 
-    /* "View.MemoryView":952
+    /* "View.MemoryView":954
  *     cdef int i, j
  *     for i in range(ndim / 2):
  *         j = ndim - 1 - i             # <<<<<<<<<<<<<<
  *         strides[i], strides[j] = strides[j], strides[i]
  *         shape[i], shape[j] = shape[j], shape[i]
  */
-    __Pyx_TraceLine(952,1,__PYX_ERR(2, 952, __pyx_L1_error))
+    __Pyx_TraceLine(954,1,__PYX_ERR(2, 954, __pyx_L1_error))
     __pyx_v_j = ((__pyx_v_ndim - 1) - __pyx_v_i);
 
-    /* "View.MemoryView":953
+    /* "View.MemoryView":955
  *     for i in range(ndim / 2):
  *         j = ndim - 1 - i
  *         strides[i], strides[j] = strides[j], strides[i]             # <<<<<<<<<<<<<<
  *         shape[i], shape[j] = shape[j], shape[i]
  * 
  */
-    __Pyx_TraceLine(953,1,__PYX_ERR(2, 953, __pyx_L1_error))
+    __Pyx_TraceLine(955,1,__PYX_ERR(2, 955, __pyx_L1_error))
     __pyx_t_5 = (__pyx_v_strides[__pyx_v_j]);
     __pyx_t_6 = (__pyx_v_strides[__pyx_v_i]);
     (__pyx_v_strides[__pyx_v_i]) = __pyx_t_5;
     (__pyx_v_strides[__pyx_v_j]) = __pyx_t_6;
 
-    /* "View.MemoryView":954
+    /* "View.MemoryView":956
  *         j = ndim - 1 - i
  *         strides[i], strides[j] = strides[j], strides[i]
  *         shape[i], shape[j] = shape[j], shape[i]             # <<<<<<<<<<<<<<
  * 
  *         if memslice.suboffsets[i] >= 0 or memslice.suboffsets[j] >= 0:
  */
-    __Pyx_TraceLine(954,1,__PYX_ERR(2, 954, __pyx_L1_error))
+    __Pyx_TraceLine(956,1,__PYX_ERR(2, 956, __pyx_L1_error))
     __pyx_t_6 = (__pyx_v_shape[__pyx_v_j]);
     __pyx_t_5 = (__pyx_v_shape[__pyx_v_i]);
     (__pyx_v_shape[__pyx_v_i]) = __pyx_t_6;
     (__pyx_v_shape[__pyx_v_j]) = __pyx_t_5;
 
-    /* "View.MemoryView":956
+    /* "View.MemoryView":958
  *         shape[i], shape[j] = shape[j], shape[i]
  * 
  *         if memslice.suboffsets[i] >= 0 or memslice.suboffsets[j] >= 0:             # <<<<<<<<<<<<<<
  *             _err(ValueError, "Cannot transpose memoryview with indirect dimensions")
  * 
  */
-    __Pyx_TraceLine(956,1,__PYX_ERR(2, 956, __pyx_L1_error))
+    __Pyx_TraceLine(958,1,__PYX_ERR(2, 958, __pyx_L1_error))
     __pyx_t_8 = (((__pyx_v_memslice->suboffsets[__pyx_v_i]) >= 0) != 0);
     if (!__pyx_t_8) {
     } else {
       __pyx_t_7 = __pyx_t_8;
       goto __pyx_L6_bool_binop_done;
     }
     __pyx_t_8 = (((__pyx_v_memslice->suboffsets[__pyx_v_j]) >= 0) != 0);
     __pyx_t_7 = __pyx_t_8;
     __pyx_L6_bool_binop_done:;
     if (__pyx_t_7) {
 
-      /* "View.MemoryView":957
+      /* "View.MemoryView":959
  * 
  *         if memslice.suboffsets[i] >= 0 or memslice.suboffsets[j] >= 0:
  *             _err(ValueError, "Cannot transpose memoryview with indirect dimensions")             # <<<<<<<<<<<<<<
  * 
  *     return 1
  */
-      __Pyx_TraceLine(957,1,__PYX_ERR(2, 957, __pyx_L1_error))
-      __pyx_t_9 = __pyx_memoryview_err(__pyx_builtin_ValueError, ((char *)"Cannot transpose memoryview with indirect dimensions")); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(2, 957, __pyx_L1_error)
+      __Pyx_TraceLine(959,1,__PYX_ERR(2, 959, __pyx_L1_error))
+      __pyx_t_9 = __pyx_memoryview_err(__pyx_builtin_ValueError, ((char *)"Cannot transpose memoryview with indirect dimensions")); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(2, 959, __pyx_L1_error)
 
-      /* "View.MemoryView":956
+      /* "View.MemoryView":958
  *         shape[i], shape[j] = shape[j], shape[i]
  * 
  *         if memslice.suboffsets[i] >= 0 or memslice.suboffsets[j] >= 0:             # <<<<<<<<<<<<<<
  *             _err(ValueError, "Cannot transpose memoryview with indirect dimensions")
  * 
  */
     }
   }
 
-  /* "View.MemoryView":959
+  /* "View.MemoryView":961
  *             _err(ValueError, "Cannot transpose memoryview with indirect dimensions")
  * 
  *     return 1             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_TraceLine(959,1,__PYX_ERR(2, 959, __pyx_L1_error))
+  __Pyx_TraceLine(961,1,__PYX_ERR(2, 961, __pyx_L1_error))
   __pyx_r = 1;
   goto __pyx_L0;
 
-  /* "View.MemoryView":943
+  /* "View.MemoryView":945
  * 
  * @cname('__pyx_memslice_transpose')
  * cdef int transpose_memslice(__Pyx_memviewslice *memslice) nogil except 0:             # <<<<<<<<<<<<<<
  *     cdef int ndim = memslice.memview.view.ndim
  * 
  */
 
@@ -26168,15 +26362,15 @@
   }
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
   return __pyx_r;
 }
 
-/* "View.MemoryView":976
+/* "View.MemoryView":978
  *     cdef int (*to_dtype_func)(char *, object) except 0
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         __PYX_XDEC_MEMVIEW(&self.from_slice, 1)
  * 
  */
 
@@ -26194,27 +26388,27 @@
 static void __pyx_memoryviewslice___pyx_pf_15View_dot_MemoryView_16_memoryviewslice___dealloc__(struct __pyx_memoryviewslice_obj *__pyx_v_self) {
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__dealloc__", 0);
-  __Pyx_TraceCall("__dealloc__", __pyx_f[2], 976, 0, __PYX_ERR(2, 976, __pyx_L1_error));
+  __Pyx_TraceCall("__dealloc__", __pyx_f[2], 978, 0, __PYX_ERR(2, 978, __pyx_L1_error));
 
-  /* "View.MemoryView":977
+  /* "View.MemoryView":979
  * 
  *     def __dealloc__(self):
  *         __PYX_XDEC_MEMVIEW(&self.from_slice, 1)             # <<<<<<<<<<<<<<
  * 
  *     cdef convert_item_to_object(self, char *itemp):
  */
-  __Pyx_TraceLine(977,0,__PYX_ERR(2, 977, __pyx_L1_error))
+  __Pyx_TraceLine(979,0,__PYX_ERR(2, 979, __pyx_L1_error))
   __PYX_XDEC_MEMVIEW((&__pyx_v_self->from_slice), 1);
 
-  /* "View.MemoryView":976
+  /* "View.MemoryView":978
  *     cdef int (*to_dtype_func)(char *, object) except 0
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         __PYX_XDEC_MEMVIEW(&self.from_slice, 1)
  * 
  */
 
@@ -26223,15 +26417,15 @@
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("View.MemoryView._memoryviewslice.__dealloc__", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
 }
 
-/* "View.MemoryView":979
+/* "View.MemoryView":981
  *         __PYX_XDEC_MEMVIEW(&self.from_slice, 1)
  * 
  *     cdef convert_item_to_object(self, char *itemp):             # <<<<<<<<<<<<<<
  *         if self.to_object_func != NULL:
  *             return self.to_object_func(itemp)
  */
 
@@ -26241,69 +26435,69 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("convert_item_to_object", 0);
-  __Pyx_TraceCall("convert_item_to_object", __pyx_f[2], 979, 0, __PYX_ERR(2, 979, __pyx_L1_error));
+  __Pyx_TraceCall("convert_item_to_object", __pyx_f[2], 981, 0, __PYX_ERR(2, 981, __pyx_L1_error));
 
-  /* "View.MemoryView":980
+  /* "View.MemoryView":982
  * 
  *     cdef convert_item_to_object(self, char *itemp):
  *         if self.to_object_func != NULL:             # <<<<<<<<<<<<<<
  *             return self.to_object_func(itemp)
  *         else:
  */
-  __Pyx_TraceLine(980,0,__PYX_ERR(2, 980, __pyx_L1_error))
+  __Pyx_TraceLine(982,0,__PYX_ERR(2, 982, __pyx_L1_error))
   __pyx_t_1 = ((__pyx_v_self->to_object_func != NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":981
+    /* "View.MemoryView":983
  *     cdef convert_item_to_object(self, char *itemp):
  *         if self.to_object_func != NULL:
  *             return self.to_object_func(itemp)             # <<<<<<<<<<<<<<
  *         else:
  *             return memoryview.convert_item_to_object(self, itemp)
  */
-    __Pyx_TraceLine(981,0,__PYX_ERR(2, 981, __pyx_L1_error))
+    __Pyx_TraceLine(983,0,__PYX_ERR(2, 983, __pyx_L1_error))
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_2 = __pyx_v_self->to_object_func(__pyx_v_itemp); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 981, __pyx_L1_error)
+    __pyx_t_2 = __pyx_v_self->to_object_func(__pyx_v_itemp); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 983, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
 
-    /* "View.MemoryView":980
+    /* "View.MemoryView":982
  * 
  *     cdef convert_item_to_object(self, char *itemp):
  *         if self.to_object_func != NULL:             # <<<<<<<<<<<<<<
  *             return self.to_object_func(itemp)
  *         else:
  */
   }
 
-  /* "View.MemoryView":983
+  /* "View.MemoryView":985
  *             return self.to_object_func(itemp)
  *         else:
  *             return memoryview.convert_item_to_object(self, itemp)             # <<<<<<<<<<<<<<
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):
  */
-  __Pyx_TraceLine(983,0,__PYX_ERR(2, 983, __pyx_L1_error))
+  __Pyx_TraceLine(985,0,__PYX_ERR(2, 985, __pyx_L1_error))
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_2 = __pyx_memoryview_convert_item_to_object(((struct __pyx_memoryview_obj *)__pyx_v_self), __pyx_v_itemp); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 983, __pyx_L1_error)
+    __pyx_t_2 = __pyx_memoryview_convert_item_to_object(((struct __pyx_memoryview_obj *)__pyx_v_self), __pyx_v_itemp); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 985, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
   }
 
-  /* "View.MemoryView":979
+  /* "View.MemoryView":981
  *         __PYX_XDEC_MEMVIEW(&self.from_slice, 1)
  * 
  *     cdef convert_item_to_object(self, char *itemp):             # <<<<<<<<<<<<<<
  *         if self.to_object_func != NULL:
  *             return self.to_object_func(itemp)
  */
 
@@ -26315,15 +26509,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":985
+/* "View.MemoryView":987
  *             return memoryview.convert_item_to_object(self, itemp)
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):             # <<<<<<<<<<<<<<
  *         if self.to_dtype_func != NULL:
  *             self.to_dtype_func(itemp, value)
  */
 
@@ -26334,63 +26528,63 @@
   int __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("assign_item_from_object", 0);
-  __Pyx_TraceCall("assign_item_from_object", __pyx_f[2], 985, 0, __PYX_ERR(2, 985, __pyx_L1_error));
+  __Pyx_TraceCall("assign_item_from_object", __pyx_f[2], 987, 0, __PYX_ERR(2, 987, __pyx_L1_error));
 
-  /* "View.MemoryView":986
+  /* "View.MemoryView":988
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):
  *         if self.to_dtype_func != NULL:             # <<<<<<<<<<<<<<
  *             self.to_dtype_func(itemp, value)
  *         else:
  */
-  __Pyx_TraceLine(986,0,__PYX_ERR(2, 986, __pyx_L1_error))
+  __Pyx_TraceLine(988,0,__PYX_ERR(2, 988, __pyx_L1_error))
   __pyx_t_1 = ((__pyx_v_self->to_dtype_func != NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":987
+    /* "View.MemoryView":989
  *     cdef assign_item_from_object(self, char *itemp, object value):
  *         if self.to_dtype_func != NULL:
  *             self.to_dtype_func(itemp, value)             # <<<<<<<<<<<<<<
  *         else:
  *             memoryview.assign_item_from_object(self, itemp, value)
  */
-    __Pyx_TraceLine(987,0,__PYX_ERR(2, 987, __pyx_L1_error))
-    __pyx_t_2 = __pyx_v_self->to_dtype_func(__pyx_v_itemp, __pyx_v_value); if (unlikely(__pyx_t_2 == ((int)0))) __PYX_ERR(2, 987, __pyx_L1_error)
+    __Pyx_TraceLine(989,0,__PYX_ERR(2, 989, __pyx_L1_error))
+    __pyx_t_2 = __pyx_v_self->to_dtype_func(__pyx_v_itemp, __pyx_v_value); if (unlikely(__pyx_t_2 == ((int)0))) __PYX_ERR(2, 989, __pyx_L1_error)
 
-    /* "View.MemoryView":986
+    /* "View.MemoryView":988
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):
  *         if self.to_dtype_func != NULL:             # <<<<<<<<<<<<<<
  *             self.to_dtype_func(itemp, value)
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":989
+  /* "View.MemoryView":991
  *             self.to_dtype_func(itemp, value)
  *         else:
  *             memoryview.assign_item_from_object(self, itemp, value)             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
-  __Pyx_TraceLine(989,0,__PYX_ERR(2, 989, __pyx_L1_error))
+  __Pyx_TraceLine(991,0,__PYX_ERR(2, 991, __pyx_L1_error))
   /*else*/ {
-    __pyx_t_3 = __pyx_memoryview_assign_item_from_object(((struct __pyx_memoryview_obj *)__pyx_v_self), __pyx_v_itemp, __pyx_v_value); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 989, __pyx_L1_error)
+    __pyx_t_3 = __pyx_memoryview_assign_item_from_object(((struct __pyx_memoryview_obj *)__pyx_v_self), __pyx_v_itemp, __pyx_v_value); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 991, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":985
+  /* "View.MemoryView":987
  *             return memoryview.convert_item_to_object(self, itemp)
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):             # <<<<<<<<<<<<<<
  *         if self.to_dtype_func != NULL:
  *             self.to_dtype_func(itemp, value)
  */
 
@@ -26404,15 +26598,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":992
+/* "View.MemoryView":994
  * 
  *     @property
  *     def base(self):             # <<<<<<<<<<<<<<
  *         return self.from_object
  * 
  */
 
@@ -26433,30 +26627,30 @@
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
-  __Pyx_TraceCall("__get__", __pyx_f[2], 992, 0, __PYX_ERR(2, 992, __pyx_L1_error));
+  __Pyx_TraceCall("__get__", __pyx_f[2], 994, 0, __PYX_ERR(2, 994, __pyx_L1_error));
 
-  /* "View.MemoryView":993
+  /* "View.MemoryView":995
  *     @property
  *     def base(self):
  *         return self.from_object             # <<<<<<<<<<<<<<
  * 
  *     __pyx_getbuffer = capsule(<void *> &__pyx_memoryview_getbuffer, "getbuffer(obj, view, flags)")
  */
-  __Pyx_TraceLine(993,0,__PYX_ERR(2, 993, __pyx_L1_error))
+  __Pyx_TraceLine(995,0,__PYX_ERR(2, 995, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_self->from_object);
   __pyx_r = __pyx_v_self->from_object;
   goto __pyx_L0;
 
-  /* "View.MemoryView":992
+  /* "View.MemoryView":994
  * 
  *     @property
  *     def base(self):             # <<<<<<<<<<<<<<
  *         return self.from_object
  * 
  */
 
@@ -26504,15 +26698,15 @@
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
   __Pyx_TraceLine(2,0,__PYX_ERR(2, 2, __pyx_L1_error))
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__26, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__27, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(2, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
@@ -26564,15 +26758,15 @@
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __Pyx_TraceLine(4,0,__PYX_ERR(2, 4, __pyx_L1_error))
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__27, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__28, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(2, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
@@ -26588,15 +26782,15 @@
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":999
+/* "View.MemoryView":1001
  * 
  * @cname('__pyx_memoryview_fromslice')
  * cdef memoryview_fromslice(__Pyx_memviewslice memviewslice,             # <<<<<<<<<<<<<<
  *                           int ndim,
  *                           object (*to_object_func)(char *),
  */
 
@@ -26616,381 +26810,381 @@
   Py_ssize_t *__pyx_t_7;
   Py_ssize_t *__pyx_t_8;
   Py_ssize_t __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("memoryview_fromslice", 0);
-  __Pyx_TraceCall("memoryview_fromslice", __pyx_f[2], 999, 0, __PYX_ERR(2, 999, __pyx_L1_error));
+  __Pyx_TraceCall("memoryview_fromslice", __pyx_f[2], 1001, 0, __PYX_ERR(2, 1001, __pyx_L1_error));
 
-  /* "View.MemoryView":1007
+  /* "View.MemoryView":1009
  *     cdef _memoryviewslice result
  * 
  *     if <PyObject *> memviewslice.memview == Py_None:             # <<<<<<<<<<<<<<
  *         return None
  * 
  */
-  __Pyx_TraceLine(1007,0,__PYX_ERR(2, 1007, __pyx_L1_error))
+  __Pyx_TraceLine(1009,0,__PYX_ERR(2, 1009, __pyx_L1_error))
   __pyx_t_1 = ((((PyObject *)__pyx_v_memviewslice.memview) == Py_None) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":1008
+    /* "View.MemoryView":1010
  * 
  *     if <PyObject *> memviewslice.memview == Py_None:
  *         return None             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __Pyx_TraceLine(1008,0,__PYX_ERR(2, 1008, __pyx_L1_error))
+    __Pyx_TraceLine(1010,0,__PYX_ERR(2, 1010, __pyx_L1_error))
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "View.MemoryView":1007
+    /* "View.MemoryView":1009
  *     cdef _memoryviewslice result
  * 
  *     if <PyObject *> memviewslice.memview == Py_None:             # <<<<<<<<<<<<<<
  *         return None
  * 
  */
   }
 
-  /* "View.MemoryView":1013
+  /* "View.MemoryView":1015
  * 
  * 
  *     result = _memoryviewslice(None, 0, dtype_is_object)             # <<<<<<<<<<<<<<
  * 
  *     result.from_slice = memviewslice
  */
-  __Pyx_TraceLine(1013,0,__PYX_ERR(2, 1013, __pyx_L1_error))
-  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_v_dtype_is_object); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1013, __pyx_L1_error)
+  __Pyx_TraceLine(1015,0,__PYX_ERR(2, 1015, __pyx_L1_error))
+  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_v_dtype_is_object); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1015, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 1013, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 1015, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   PyTuple_SET_ITEM(__pyx_t_3, 0, Py_None);
   __Pyx_INCREF(__pyx_int_0);
   __Pyx_GIVEREF(__pyx_int_0);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_int_0);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_t_2);
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_memoryviewslice_type), __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1013, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_memoryviewslice_type), __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1015, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_result = ((struct __pyx_memoryviewslice_obj *)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "View.MemoryView":1015
+  /* "View.MemoryView":1017
  *     result = _memoryviewslice(None, 0, dtype_is_object)
  * 
  *     result.from_slice = memviewslice             # <<<<<<<<<<<<<<
  *     __PYX_INC_MEMVIEW(&memviewslice, 1)
  * 
  */
-  __Pyx_TraceLine(1015,0,__PYX_ERR(2, 1015, __pyx_L1_error))
+  __Pyx_TraceLine(1017,0,__PYX_ERR(2, 1017, __pyx_L1_error))
   __pyx_v_result->from_slice = __pyx_v_memviewslice;
 
-  /* "View.MemoryView":1016
+  /* "View.MemoryView":1018
  * 
  *     result.from_slice = memviewslice
  *     __PYX_INC_MEMVIEW(&memviewslice, 1)             # <<<<<<<<<<<<<<
  * 
  *     result.from_object = (<memoryview> memviewslice.memview).base
  */
-  __Pyx_TraceLine(1016,0,__PYX_ERR(2, 1016, __pyx_L1_error))
+  __Pyx_TraceLine(1018,0,__PYX_ERR(2, 1018, __pyx_L1_error))
   __PYX_INC_MEMVIEW((&__pyx_v_memviewslice), 1);
 
-  /* "View.MemoryView":1018
+  /* "View.MemoryView":1020
  *     __PYX_INC_MEMVIEW(&memviewslice, 1)
  * 
  *     result.from_object = (<memoryview> memviewslice.memview).base             # <<<<<<<<<<<<<<
  *     result.typeinfo = memviewslice.memview.typeinfo
  * 
  */
-  __Pyx_TraceLine(1018,0,__PYX_ERR(2, 1018, __pyx_L1_error))
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_memviewslice.memview), __pyx_n_s_base); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1018, __pyx_L1_error)
+  __Pyx_TraceLine(1020,0,__PYX_ERR(2, 1020, __pyx_L1_error))
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_memviewslice.memview), __pyx_n_s_base); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1020, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   __Pyx_GOTREF(__pyx_v_result->from_object);
   __Pyx_DECREF(__pyx_v_result->from_object);
   __pyx_v_result->from_object = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "View.MemoryView":1019
+  /* "View.MemoryView":1021
  * 
  *     result.from_object = (<memoryview> memviewslice.memview).base
  *     result.typeinfo = memviewslice.memview.typeinfo             # <<<<<<<<<<<<<<
  * 
  *     result.view = memviewslice.memview.view
  */
-  __Pyx_TraceLine(1019,0,__PYX_ERR(2, 1019, __pyx_L1_error))
+  __Pyx_TraceLine(1021,0,__PYX_ERR(2, 1021, __pyx_L1_error))
   __pyx_t_4 = __pyx_v_memviewslice.memview->typeinfo;
   __pyx_v_result->__pyx_base.typeinfo = __pyx_t_4;
 
-  /* "View.MemoryView":1021
+  /* "View.MemoryView":1023
  *     result.typeinfo = memviewslice.memview.typeinfo
  * 
  *     result.view = memviewslice.memview.view             # <<<<<<<<<<<<<<
  *     result.view.buf = <void *> memviewslice.data
  *     result.view.ndim = ndim
  */
-  __Pyx_TraceLine(1021,0,__PYX_ERR(2, 1021, __pyx_L1_error))
+  __Pyx_TraceLine(1023,0,__PYX_ERR(2, 1023, __pyx_L1_error))
   __pyx_t_5 = __pyx_v_memviewslice.memview->view;
   __pyx_v_result->__pyx_base.view = __pyx_t_5;
 
-  /* "View.MemoryView":1022
+  /* "View.MemoryView":1024
  * 
  *     result.view = memviewslice.memview.view
  *     result.view.buf = <void *> memviewslice.data             # <<<<<<<<<<<<<<
  *     result.view.ndim = ndim
  *     (<__pyx_buffer *> &result.view).obj = Py_None
  */
-  __Pyx_TraceLine(1022,0,__PYX_ERR(2, 1022, __pyx_L1_error))
+  __Pyx_TraceLine(1024,0,__PYX_ERR(2, 1024, __pyx_L1_error))
   __pyx_v_result->__pyx_base.view.buf = ((void *)__pyx_v_memviewslice.data);
 
-  /* "View.MemoryView":1023
+  /* "View.MemoryView":1025
  *     result.view = memviewslice.memview.view
  *     result.view.buf = <void *> memviewslice.data
  *     result.view.ndim = ndim             # <<<<<<<<<<<<<<
  *     (<__pyx_buffer *> &result.view).obj = Py_None
  *     Py_INCREF(Py_None)
  */
-  __Pyx_TraceLine(1023,0,__PYX_ERR(2, 1023, __pyx_L1_error))
+  __Pyx_TraceLine(1025,0,__PYX_ERR(2, 1025, __pyx_L1_error))
   __pyx_v_result->__pyx_base.view.ndim = __pyx_v_ndim;
 
-  /* "View.MemoryView":1024
+  /* "View.MemoryView":1026
  *     result.view.buf = <void *> memviewslice.data
  *     result.view.ndim = ndim
  *     (<__pyx_buffer *> &result.view).obj = Py_None             # <<<<<<<<<<<<<<
  *     Py_INCREF(Py_None)
  * 
  */
-  __Pyx_TraceLine(1024,0,__PYX_ERR(2, 1024, __pyx_L1_error))
+  __Pyx_TraceLine(1026,0,__PYX_ERR(2, 1026, __pyx_L1_error))
   ((Py_buffer *)(&__pyx_v_result->__pyx_base.view))->obj = Py_None;
 
-  /* "View.MemoryView":1025
+  /* "View.MemoryView":1027
  *     result.view.ndim = ndim
  *     (<__pyx_buffer *> &result.view).obj = Py_None
  *     Py_INCREF(Py_None)             # <<<<<<<<<<<<<<
  * 
  *     if (<memoryview>memviewslice.memview).flags & PyBUF_WRITABLE:
  */
-  __Pyx_TraceLine(1025,0,__PYX_ERR(2, 1025, __pyx_L1_error))
+  __Pyx_TraceLine(1027,0,__PYX_ERR(2, 1027, __pyx_L1_error))
   Py_INCREF(Py_None);
 
-  /* "View.MemoryView":1027
+  /* "View.MemoryView":1029
  *     Py_INCREF(Py_None)
  * 
  *     if (<memoryview>memviewslice.memview).flags & PyBUF_WRITABLE:             # <<<<<<<<<<<<<<
  *         result.flags = PyBUF_RECORDS
  *     else:
  */
-  __Pyx_TraceLine(1027,0,__PYX_ERR(2, 1027, __pyx_L1_error))
+  __Pyx_TraceLine(1029,0,__PYX_ERR(2, 1029, __pyx_L1_error))
   __pyx_t_1 = ((((struct __pyx_memoryview_obj *)__pyx_v_memviewslice.memview)->flags & PyBUF_WRITABLE) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":1028
+    /* "View.MemoryView":1030
  * 
  *     if (<memoryview>memviewslice.memview).flags & PyBUF_WRITABLE:
  *         result.flags = PyBUF_RECORDS             # <<<<<<<<<<<<<<
  *     else:
  *         result.flags = PyBUF_RECORDS_RO
  */
-    __Pyx_TraceLine(1028,0,__PYX_ERR(2, 1028, __pyx_L1_error))
+    __Pyx_TraceLine(1030,0,__PYX_ERR(2, 1030, __pyx_L1_error))
     __pyx_v_result->__pyx_base.flags = PyBUF_RECORDS;
 
-    /* "View.MemoryView":1027
+    /* "View.MemoryView":1029
  *     Py_INCREF(Py_None)
  * 
  *     if (<memoryview>memviewslice.memview).flags & PyBUF_WRITABLE:             # <<<<<<<<<<<<<<
  *         result.flags = PyBUF_RECORDS
  *     else:
  */
     goto __pyx_L4;
   }
 
-  /* "View.MemoryView":1030
+  /* "View.MemoryView":1032
  *         result.flags = PyBUF_RECORDS
  *     else:
  *         result.flags = PyBUF_RECORDS_RO             # <<<<<<<<<<<<<<
  * 
  *     result.view.shape = <Py_ssize_t *> result.from_slice.shape
  */
-  __Pyx_TraceLine(1030,0,__PYX_ERR(2, 1030, __pyx_L1_error))
+  __Pyx_TraceLine(1032,0,__PYX_ERR(2, 1032, __pyx_L1_error))
   /*else*/ {
     __pyx_v_result->__pyx_base.flags = PyBUF_RECORDS_RO;
   }
   __pyx_L4:;
 
-  /* "View.MemoryView":1032
+  /* "View.MemoryView":1034
  *         result.flags = PyBUF_RECORDS_RO
  * 
  *     result.view.shape = <Py_ssize_t *> result.from_slice.shape             # <<<<<<<<<<<<<<
  *     result.view.strides = <Py_ssize_t *> result.from_slice.strides
  * 
  */
-  __Pyx_TraceLine(1032,0,__PYX_ERR(2, 1032, __pyx_L1_error))
+  __Pyx_TraceLine(1034,0,__PYX_ERR(2, 1034, __pyx_L1_error))
   __pyx_v_result->__pyx_base.view.shape = ((Py_ssize_t *)__pyx_v_result->from_slice.shape);
 
-  /* "View.MemoryView":1033
+  /* "View.MemoryView":1035
  * 
  *     result.view.shape = <Py_ssize_t *> result.from_slice.shape
  *     result.view.strides = <Py_ssize_t *> result.from_slice.strides             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_TraceLine(1033,0,__PYX_ERR(2, 1033, __pyx_L1_error))
+  __Pyx_TraceLine(1035,0,__PYX_ERR(2, 1035, __pyx_L1_error))
   __pyx_v_result->__pyx_base.view.strides = ((Py_ssize_t *)__pyx_v_result->from_slice.strides);
 
-  /* "View.MemoryView":1036
+  /* "View.MemoryView":1038
  * 
  * 
  *     result.view.suboffsets = NULL             # <<<<<<<<<<<<<<
  *     for suboffset in result.from_slice.suboffsets[:ndim]:
  *         if suboffset >= 0:
  */
-  __Pyx_TraceLine(1036,0,__PYX_ERR(2, 1036, __pyx_L1_error))
+  __Pyx_TraceLine(1038,0,__PYX_ERR(2, 1038, __pyx_L1_error))
   __pyx_v_result->__pyx_base.view.suboffsets = NULL;
 
-  /* "View.MemoryView":1037
+  /* "View.MemoryView":1039
  * 
  *     result.view.suboffsets = NULL
  *     for suboffset in result.from_slice.suboffsets[:ndim]:             # <<<<<<<<<<<<<<
  *         if suboffset >= 0:
  *             result.view.suboffsets = <Py_ssize_t *> result.from_slice.suboffsets
  */
-  __Pyx_TraceLine(1037,0,__PYX_ERR(2, 1037, __pyx_L1_error))
+  __Pyx_TraceLine(1039,0,__PYX_ERR(2, 1039, __pyx_L1_error))
   __pyx_t_7 = (__pyx_v_result->from_slice.suboffsets + __pyx_v_ndim);
   for (__pyx_t_8 = __pyx_v_result->from_slice.suboffsets; __pyx_t_8 < __pyx_t_7; __pyx_t_8++) {
     __pyx_t_6 = __pyx_t_8;
     __pyx_v_suboffset = (__pyx_t_6[0]);
 
-    /* "View.MemoryView":1038
+    /* "View.MemoryView":1040
  *     result.view.suboffsets = NULL
  *     for suboffset in result.from_slice.suboffsets[:ndim]:
  *         if suboffset >= 0:             # <<<<<<<<<<<<<<
  *             result.view.suboffsets = <Py_ssize_t *> result.from_slice.suboffsets
  *             break
  */
-    __Pyx_TraceLine(1038,0,__PYX_ERR(2, 1038, __pyx_L1_error))
+    __Pyx_TraceLine(1040,0,__PYX_ERR(2, 1040, __pyx_L1_error))
     __pyx_t_1 = ((__pyx_v_suboffset >= 0) != 0);
     if (__pyx_t_1) {
 
-      /* "View.MemoryView":1039
+      /* "View.MemoryView":1041
  *     for suboffset in result.from_slice.suboffsets[:ndim]:
  *         if suboffset >= 0:
  *             result.view.suboffsets = <Py_ssize_t *> result.from_slice.suboffsets             # <<<<<<<<<<<<<<
  *             break
  * 
  */
-      __Pyx_TraceLine(1039,0,__PYX_ERR(2, 1039, __pyx_L1_error))
+      __Pyx_TraceLine(1041,0,__PYX_ERR(2, 1041, __pyx_L1_error))
       __pyx_v_result->__pyx_base.view.suboffsets = ((Py_ssize_t *)__pyx_v_result->from_slice.suboffsets);
 
-      /* "View.MemoryView":1040
+      /* "View.MemoryView":1042
  *         if suboffset >= 0:
  *             result.view.suboffsets = <Py_ssize_t *> result.from_slice.suboffsets
  *             break             # <<<<<<<<<<<<<<
  * 
  *     result.view.len = result.view.itemsize
  */
-      __Pyx_TraceLine(1040,0,__PYX_ERR(2, 1040, __pyx_L1_error))
+      __Pyx_TraceLine(1042,0,__PYX_ERR(2, 1042, __pyx_L1_error))
       goto __pyx_L6_break;
 
-      /* "View.MemoryView":1038
+      /* "View.MemoryView":1040
  *     result.view.suboffsets = NULL
  *     for suboffset in result.from_slice.suboffsets[:ndim]:
  *         if suboffset >= 0:             # <<<<<<<<<<<<<<
  *             result.view.suboffsets = <Py_ssize_t *> result.from_slice.suboffsets
  *             break
  */
     }
   }
   __pyx_L6_break:;
 
-  /* "View.MemoryView":1042
+  /* "View.MemoryView":1044
  *             break
  * 
  *     result.view.len = result.view.itemsize             # <<<<<<<<<<<<<<
  *     for length in result.view.shape[:ndim]:
  *         result.view.len *= length
  */
-  __Pyx_TraceLine(1042,0,__PYX_ERR(2, 1042, __pyx_L1_error))
+  __Pyx_TraceLine(1044,0,__PYX_ERR(2, 1044, __pyx_L1_error))
   __pyx_t_9 = __pyx_v_result->__pyx_base.view.itemsize;
   __pyx_v_result->__pyx_base.view.len = __pyx_t_9;
 
-  /* "View.MemoryView":1043
+  /* "View.MemoryView":1045
  * 
  *     result.view.len = result.view.itemsize
  *     for length in result.view.shape[:ndim]:             # <<<<<<<<<<<<<<
  *         result.view.len *= length
  * 
  */
-  __Pyx_TraceLine(1043,0,__PYX_ERR(2, 1043, __pyx_L1_error))
+  __Pyx_TraceLine(1045,0,__PYX_ERR(2, 1045, __pyx_L1_error))
   __pyx_t_7 = (__pyx_v_result->__pyx_base.view.shape + __pyx_v_ndim);
   for (__pyx_t_8 = __pyx_v_result->__pyx_base.view.shape; __pyx_t_8 < __pyx_t_7; __pyx_t_8++) {
     __pyx_t_6 = __pyx_t_8;
-    __pyx_t_2 = PyInt_FromSsize_t((__pyx_t_6[0])); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1043, __pyx_L1_error)
+    __pyx_t_2 = PyInt_FromSsize_t((__pyx_t_6[0])); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1045, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_XDECREF_SET(__pyx_v_length, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "View.MemoryView":1044
+    /* "View.MemoryView":1046
  *     result.view.len = result.view.itemsize
  *     for length in result.view.shape[:ndim]:
  *         result.view.len *= length             # <<<<<<<<<<<<<<
  * 
  *     result.to_object_func = to_object_func
  */
-    __Pyx_TraceLine(1044,0,__PYX_ERR(2, 1044, __pyx_L1_error))
-    __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_result->__pyx_base.view.len); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1044, __pyx_L1_error)
+    __Pyx_TraceLine(1046,0,__PYX_ERR(2, 1046, __pyx_L1_error))
+    __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_result->__pyx_base.view.len); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1046, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PyNumber_InPlaceMultiply(__pyx_t_2, __pyx_v_length); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 1044, __pyx_L1_error)
+    __pyx_t_3 = PyNumber_InPlaceMultiply(__pyx_t_2, __pyx_v_length); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 1046, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_3); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(2, 1044, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_3); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(2, 1046, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_result->__pyx_base.view.len = __pyx_t_9;
   }
 
-  /* "View.MemoryView":1046
+  /* "View.MemoryView":1048
  *         result.view.len *= length
  * 
  *     result.to_object_func = to_object_func             # <<<<<<<<<<<<<<
  *     result.to_dtype_func = to_dtype_func
  * 
  */
-  __Pyx_TraceLine(1046,0,__PYX_ERR(2, 1046, __pyx_L1_error))
+  __Pyx_TraceLine(1048,0,__PYX_ERR(2, 1048, __pyx_L1_error))
   __pyx_v_result->to_object_func = __pyx_v_to_object_func;
 
-  /* "View.MemoryView":1047
+  /* "View.MemoryView":1049
  * 
  *     result.to_object_func = to_object_func
  *     result.to_dtype_func = to_dtype_func             # <<<<<<<<<<<<<<
  * 
  *     return result
  */
-  __Pyx_TraceLine(1047,0,__PYX_ERR(2, 1047, __pyx_L1_error))
+  __Pyx_TraceLine(1049,0,__PYX_ERR(2, 1049, __pyx_L1_error))
   __pyx_v_result->to_dtype_func = __pyx_v_to_dtype_func;
 
-  /* "View.MemoryView":1049
+  /* "View.MemoryView":1051
  *     result.to_dtype_func = to_dtype_func
  * 
  *     return result             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_get_slice_from_memoryview')
  */
-  __Pyx_TraceLine(1049,0,__PYX_ERR(2, 1049, __pyx_L1_error))
+  __Pyx_TraceLine(1051,0,__PYX_ERR(2, 1051, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_result));
   __pyx_r = ((PyObject *)__pyx_v_result);
   goto __pyx_L0;
 
-  /* "View.MemoryView":999
+  /* "View.MemoryView":1001
  * 
  * @cname('__pyx_memoryview_fromslice')
  * cdef memoryview_fromslice(__Pyx_memviewslice memviewslice,             # <<<<<<<<<<<<<<
  *                           int ndim,
  *                           object (*to_object_func)(char *),
  */
 
@@ -27005,15 +27199,15 @@
   __Pyx_XDECREF(__pyx_v_length);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":1052
+/* "View.MemoryView":1054
  * 
  * @cname('__pyx_memoryview_get_slice_from_memoryview')
  * cdef __Pyx_memviewslice *get_slice_from_memview(memoryview memview,             # <<<<<<<<<<<<<<
  *                                                    __Pyx_memviewslice *mslice) except NULL:
  *     cdef _memoryviewslice obj
  */
 
@@ -27025,86 +27219,86 @@
   int __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_slice_from_memview", 0);
-  __Pyx_TraceCall("get_slice_from_memview", __pyx_f[2], 1052, 0, __PYX_ERR(2, 1052, __pyx_L1_error));
+  __Pyx_TraceCall("get_slice_from_memview", __pyx_f[2], 1054, 0, __PYX_ERR(2, 1054, __pyx_L1_error));
 
-  /* "View.MemoryView":1055
+  /* "View.MemoryView":1057
  *                                                    __Pyx_memviewslice *mslice) except NULL:
  *     cdef _memoryviewslice obj
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         obj = memview
  *         return &obj.from_slice
  */
-  __Pyx_TraceLine(1055,0,__PYX_ERR(2, 1055, __pyx_L1_error))
+  __Pyx_TraceLine(1057,0,__PYX_ERR(2, 1057, __pyx_L1_error))
   __pyx_t_1 = __Pyx_TypeCheck(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1056
+    /* "View.MemoryView":1058
  *     cdef _memoryviewslice obj
  *     if isinstance(memview, _memoryviewslice):
  *         obj = memview             # <<<<<<<<<<<<<<
  *         return &obj.from_slice
  *     else:
  */
-    __Pyx_TraceLine(1056,0,__PYX_ERR(2, 1056, __pyx_L1_error))
-    if (!(likely(((((PyObject *)__pyx_v_memview)) == Py_None) || likely(__Pyx_TypeTest(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type))))) __PYX_ERR(2, 1056, __pyx_L1_error)
+    __Pyx_TraceLine(1058,0,__PYX_ERR(2, 1058, __pyx_L1_error))
+    if (!(likely(((((PyObject *)__pyx_v_memview)) == Py_None) || likely(__Pyx_TypeTest(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type))))) __PYX_ERR(2, 1058, __pyx_L1_error)
     __pyx_t_3 = ((PyObject *)__pyx_v_memview);
     __Pyx_INCREF(__pyx_t_3);
     __pyx_v_obj = ((struct __pyx_memoryviewslice_obj *)__pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "View.MemoryView":1057
+    /* "View.MemoryView":1059
  *     if isinstance(memview, _memoryviewslice):
  *         obj = memview
  *         return &obj.from_slice             # <<<<<<<<<<<<<<
  *     else:
  *         slice_copy(memview, mslice)
  */
-    __Pyx_TraceLine(1057,0,__PYX_ERR(2, 1057, __pyx_L1_error))
+    __Pyx_TraceLine(1059,0,__PYX_ERR(2, 1059, __pyx_L1_error))
     __pyx_r = (&__pyx_v_obj->from_slice);
     goto __pyx_L0;
 
-    /* "View.MemoryView":1055
+    /* "View.MemoryView":1057
  *                                                    __Pyx_memviewslice *mslice) except NULL:
  *     cdef _memoryviewslice obj
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         obj = memview
  *         return &obj.from_slice
  */
   }
 
-  /* "View.MemoryView":1059
+  /* "View.MemoryView":1061
  *         return &obj.from_slice
  *     else:
  *         slice_copy(memview, mslice)             # <<<<<<<<<<<<<<
  *         return mslice
  * 
  */
-  __Pyx_TraceLine(1059,0,__PYX_ERR(2, 1059, __pyx_L1_error))
+  __Pyx_TraceLine(1061,0,__PYX_ERR(2, 1061, __pyx_L1_error))
   /*else*/ {
     __pyx_memoryview_slice_copy(__pyx_v_memview, __pyx_v_mslice);
 
-    /* "View.MemoryView":1060
+    /* "View.MemoryView":1062
  *     else:
  *         slice_copy(memview, mslice)
  *         return mslice             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_slice_copy')
  */
-    __Pyx_TraceLine(1060,0,__PYX_ERR(2, 1060, __pyx_L1_error))
+    __Pyx_TraceLine(1062,0,__PYX_ERR(2, 1062, __pyx_L1_error))
     __pyx_r = __pyx_v_mslice;
     goto __pyx_L0;
   }
 
-  /* "View.MemoryView":1052
+  /* "View.MemoryView":1054
  * 
  * @cname('__pyx_memoryview_get_slice_from_memoryview')
  * cdef __Pyx_memviewslice *get_slice_from_memview(memoryview memview,             # <<<<<<<<<<<<<<
  *                                                    __Pyx_memviewslice *mslice) except NULL:
  *     cdef _memoryviewslice obj
  */
 
@@ -27116,15 +27310,15 @@
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_obj);
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":1063
+/* "View.MemoryView":1065
  * 
  * @cname('__pyx_memoryview_slice_copy')
  * cdef void slice_copy(memoryview memview, __Pyx_memviewslice *dst):             # <<<<<<<<<<<<<<
  *     cdef int dim
  *     cdef (Py_ssize_t*) shape, strides, suboffsets
  */
 
@@ -27140,119 +27334,119 @@
   int __pyx_t_3;
   int __pyx_t_4;
   Py_ssize_t __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("slice_copy", 0);
-  __Pyx_TraceCall("slice_copy", __pyx_f[2], 1063, 0, __PYX_ERR(2, 1063, __pyx_L1_error));
+  __Pyx_TraceCall("slice_copy", __pyx_f[2], 1065, 0, __PYX_ERR(2, 1065, __pyx_L1_error));
 
-  /* "View.MemoryView":1067
+  /* "View.MemoryView":1069
  *     cdef (Py_ssize_t*) shape, strides, suboffsets
  * 
  *     shape = memview.view.shape             # <<<<<<<<<<<<<<
  *     strides = memview.view.strides
  *     suboffsets = memview.view.suboffsets
  */
-  __Pyx_TraceLine(1067,0,__PYX_ERR(2, 1067, __pyx_L1_error))
+  __Pyx_TraceLine(1069,0,__PYX_ERR(2, 1069, __pyx_L1_error))
   __pyx_t_1 = __pyx_v_memview->view.shape;
   __pyx_v_shape = __pyx_t_1;
 
-  /* "View.MemoryView":1068
+  /* "View.MemoryView":1070
  * 
  *     shape = memview.view.shape
  *     strides = memview.view.strides             # <<<<<<<<<<<<<<
  *     suboffsets = memview.view.suboffsets
  * 
  */
-  __Pyx_TraceLine(1068,0,__PYX_ERR(2, 1068, __pyx_L1_error))
+  __Pyx_TraceLine(1070,0,__PYX_ERR(2, 1070, __pyx_L1_error))
   __pyx_t_1 = __pyx_v_memview->view.strides;
   __pyx_v_strides = __pyx_t_1;
 
-  /* "View.MemoryView":1069
+  /* "View.MemoryView":1071
  *     shape = memview.view.shape
  *     strides = memview.view.strides
  *     suboffsets = memview.view.suboffsets             # <<<<<<<<<<<<<<
  * 
  *     dst.memview = <__pyx_memoryview *> memview
  */
-  __Pyx_TraceLine(1069,0,__PYX_ERR(2, 1069, __pyx_L1_error))
+  __Pyx_TraceLine(1071,0,__PYX_ERR(2, 1071, __pyx_L1_error))
   __pyx_t_1 = __pyx_v_memview->view.suboffsets;
   __pyx_v_suboffsets = __pyx_t_1;
 
-  /* "View.MemoryView":1071
+  /* "View.MemoryView":1073
  *     suboffsets = memview.view.suboffsets
  * 
  *     dst.memview = <__pyx_memoryview *> memview             # <<<<<<<<<<<<<<
  *     dst.data = <char *> memview.view.buf
  * 
  */
-  __Pyx_TraceLine(1071,0,__PYX_ERR(2, 1071, __pyx_L1_error))
+  __Pyx_TraceLine(1073,0,__PYX_ERR(2, 1073, __pyx_L1_error))
   __pyx_v_dst->memview = ((struct __pyx_memoryview_obj *)__pyx_v_memview);
 
-  /* "View.MemoryView":1072
+  /* "View.MemoryView":1074
  * 
  *     dst.memview = <__pyx_memoryview *> memview
  *     dst.data = <char *> memview.view.buf             # <<<<<<<<<<<<<<
  * 
  *     for dim in range(memview.view.ndim):
  */
-  __Pyx_TraceLine(1072,0,__PYX_ERR(2, 1072, __pyx_L1_error))
+  __Pyx_TraceLine(1074,0,__PYX_ERR(2, 1074, __pyx_L1_error))
   __pyx_v_dst->data = ((char *)__pyx_v_memview->view.buf);
 
-  /* "View.MemoryView":1074
+  /* "View.MemoryView":1076
  *     dst.data = <char *> memview.view.buf
  * 
  *     for dim in range(memview.view.ndim):             # <<<<<<<<<<<<<<
  *         dst.shape[dim] = shape[dim]
  *         dst.strides[dim] = strides[dim]
  */
-  __Pyx_TraceLine(1074,0,__PYX_ERR(2, 1074, __pyx_L1_error))
+  __Pyx_TraceLine(1076,0,__PYX_ERR(2, 1076, __pyx_L1_error))
   __pyx_t_2 = __pyx_v_memview->view.ndim;
   __pyx_t_3 = __pyx_t_2;
   for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
     __pyx_v_dim = __pyx_t_4;
 
-    /* "View.MemoryView":1075
+    /* "View.MemoryView":1077
  * 
  *     for dim in range(memview.view.ndim):
  *         dst.shape[dim] = shape[dim]             # <<<<<<<<<<<<<<
  *         dst.strides[dim] = strides[dim]
  *         dst.suboffsets[dim] = suboffsets[dim] if suboffsets else -1
  */
-    __Pyx_TraceLine(1075,0,__PYX_ERR(2, 1075, __pyx_L1_error))
+    __Pyx_TraceLine(1077,0,__PYX_ERR(2, 1077, __pyx_L1_error))
     (__pyx_v_dst->shape[__pyx_v_dim]) = (__pyx_v_shape[__pyx_v_dim]);
 
-    /* "View.MemoryView":1076
+    /* "View.MemoryView":1078
  *     for dim in range(memview.view.ndim):
  *         dst.shape[dim] = shape[dim]
  *         dst.strides[dim] = strides[dim]             # <<<<<<<<<<<<<<
  *         dst.suboffsets[dim] = suboffsets[dim] if suboffsets else -1
  * 
  */
-    __Pyx_TraceLine(1076,0,__PYX_ERR(2, 1076, __pyx_L1_error))
+    __Pyx_TraceLine(1078,0,__PYX_ERR(2, 1078, __pyx_L1_error))
     (__pyx_v_dst->strides[__pyx_v_dim]) = (__pyx_v_strides[__pyx_v_dim]);
 
-    /* "View.MemoryView":1077
+    /* "View.MemoryView":1079
  *         dst.shape[dim] = shape[dim]
  *         dst.strides[dim] = strides[dim]
  *         dst.suboffsets[dim] = suboffsets[dim] if suboffsets else -1             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_copy_object')
  */
-    __Pyx_TraceLine(1077,0,__PYX_ERR(2, 1077, __pyx_L1_error))
+    __Pyx_TraceLine(1079,0,__PYX_ERR(2, 1079, __pyx_L1_error))
     if ((__pyx_v_suboffsets != 0)) {
       __pyx_t_5 = (__pyx_v_suboffsets[__pyx_v_dim]);
     } else {
       __pyx_t_5 = -1L;
     }
     (__pyx_v_dst->suboffsets[__pyx_v_dim]) = __pyx_t_5;
   }
 
-  /* "View.MemoryView":1063
+  /* "View.MemoryView":1065
  * 
  * @cname('__pyx_memoryview_slice_copy')
  * cdef void slice_copy(memoryview memview, __Pyx_memviewslice *dst):             # <<<<<<<<<<<<<<
  *     cdef int dim
  *     cdef (Py_ssize_t*) shape, strides, suboffsets
  */
 
@@ -27261,15 +27455,15 @@
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("View.MemoryView.slice_copy", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
 }
 
-/* "View.MemoryView":1080
+/* "View.MemoryView":1082
  * 
  * @cname('__pyx_memoryview_copy_object')
  * cdef memoryview_copy(memoryview memview):             # <<<<<<<<<<<<<<
  *     "Create a new memoryview object"
  *     cdef __Pyx_memviewslice memviewslice
  */
 
@@ -27279,42 +27473,42 @@
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("memoryview_copy", 0);
-  __Pyx_TraceCall("memoryview_copy", __pyx_f[2], 1080, 0, __PYX_ERR(2, 1080, __pyx_L1_error));
+  __Pyx_TraceCall("memoryview_copy", __pyx_f[2], 1082, 0, __PYX_ERR(2, 1082, __pyx_L1_error));
 
-  /* "View.MemoryView":1083
+  /* "View.MemoryView":1085
  *     "Create a new memoryview object"
  *     cdef __Pyx_memviewslice memviewslice
  *     slice_copy(memview, &memviewslice)             # <<<<<<<<<<<<<<
  *     return memoryview_copy_from_slice(memview, &memviewslice)
  * 
  */
-  __Pyx_TraceLine(1083,0,__PYX_ERR(2, 1083, __pyx_L1_error))
+  __Pyx_TraceLine(1085,0,__PYX_ERR(2, 1085, __pyx_L1_error))
   __pyx_memoryview_slice_copy(__pyx_v_memview, (&__pyx_v_memviewslice));
 
-  /* "View.MemoryView":1084
+  /* "View.MemoryView":1086
  *     cdef __Pyx_memviewslice memviewslice
  *     slice_copy(memview, &memviewslice)
  *     return memoryview_copy_from_slice(memview, &memviewslice)             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_copy_object_from_slice')
  */
-  __Pyx_TraceLine(1084,0,__PYX_ERR(2, 1084, __pyx_L1_error))
+  __Pyx_TraceLine(1086,0,__PYX_ERR(2, 1086, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_memoryview_copy_object_from_slice(__pyx_v_memview, (&__pyx_v_memviewslice)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 1084, __pyx_L1_error)
+  __pyx_t_1 = __pyx_memoryview_copy_object_from_slice(__pyx_v_memview, (&__pyx_v_memviewslice)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 1086, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":1080
+  /* "View.MemoryView":1082
  * 
  * @cname('__pyx_memoryview_copy_object')
  * cdef memoryview_copy(memoryview memview):             # <<<<<<<<<<<<<<
  *     "Create a new memoryview object"
  *     cdef __Pyx_memviewslice memviewslice
  */
 
@@ -27326,15 +27520,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":1087
+/* "View.MemoryView":1089
  * 
  * @cname('__pyx_memoryview_copy_object_from_slice')
  * cdef memoryview_copy_from_slice(memoryview memview, __Pyx_memviewslice *memviewslice):             # <<<<<<<<<<<<<<
  *     """
  *     Create a new memoryview object from a given memoryview object and slice.
  */
 
@@ -27349,108 +27543,108 @@
   PyObject *(*__pyx_t_3)(char *);
   int (*__pyx_t_4)(char *, PyObject *);
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("memoryview_copy_from_slice", 0);
-  __Pyx_TraceCall("memoryview_copy_from_slice", __pyx_f[2], 1087, 0, __PYX_ERR(2, 1087, __pyx_L1_error));
+  __Pyx_TraceCall("memoryview_copy_from_slice", __pyx_f[2], 1089, 0, __PYX_ERR(2, 1089, __pyx_L1_error));
 
-  /* "View.MemoryView":1094
+  /* "View.MemoryView":1096
  *     cdef int (*to_dtype_func)(char *, object) except 0
  * 
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         to_object_func = (<_memoryviewslice> memview).to_object_func
  *         to_dtype_func = (<_memoryviewslice> memview).to_dtype_func
  */
-  __Pyx_TraceLine(1094,0,__PYX_ERR(2, 1094, __pyx_L1_error))
+  __Pyx_TraceLine(1096,0,__PYX_ERR(2, 1096, __pyx_L1_error))
   __pyx_t_1 = __Pyx_TypeCheck(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1095
+    /* "View.MemoryView":1097
  * 
  *     if isinstance(memview, _memoryviewslice):
  *         to_object_func = (<_memoryviewslice> memview).to_object_func             # <<<<<<<<<<<<<<
  *         to_dtype_func = (<_memoryviewslice> memview).to_dtype_func
  *     else:
  */
-    __Pyx_TraceLine(1095,0,__PYX_ERR(2, 1095, __pyx_L1_error))
+    __Pyx_TraceLine(1097,0,__PYX_ERR(2, 1097, __pyx_L1_error))
     __pyx_t_3 = ((struct __pyx_memoryviewslice_obj *)__pyx_v_memview)->to_object_func;
     __pyx_v_to_object_func = __pyx_t_3;
 
-    /* "View.MemoryView":1096
+    /* "View.MemoryView":1098
  *     if isinstance(memview, _memoryviewslice):
  *         to_object_func = (<_memoryviewslice> memview).to_object_func
  *         to_dtype_func = (<_memoryviewslice> memview).to_dtype_func             # <<<<<<<<<<<<<<
  *     else:
  *         to_object_func = NULL
  */
-    __Pyx_TraceLine(1096,0,__PYX_ERR(2, 1096, __pyx_L1_error))
+    __Pyx_TraceLine(1098,0,__PYX_ERR(2, 1098, __pyx_L1_error))
     __pyx_t_4 = ((struct __pyx_memoryviewslice_obj *)__pyx_v_memview)->to_dtype_func;
     __pyx_v_to_dtype_func = __pyx_t_4;
 
-    /* "View.MemoryView":1094
+    /* "View.MemoryView":1096
  *     cdef int (*to_dtype_func)(char *, object) except 0
  * 
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         to_object_func = (<_memoryviewslice> memview).to_object_func
  *         to_dtype_func = (<_memoryviewslice> memview).to_dtype_func
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":1098
+  /* "View.MemoryView":1100
  *         to_dtype_func = (<_memoryviewslice> memview).to_dtype_func
  *     else:
  *         to_object_func = NULL             # <<<<<<<<<<<<<<
  *         to_dtype_func = NULL
  * 
  */
-  __Pyx_TraceLine(1098,0,__PYX_ERR(2, 1098, __pyx_L1_error))
+  __Pyx_TraceLine(1100,0,__PYX_ERR(2, 1100, __pyx_L1_error))
   /*else*/ {
     __pyx_v_to_object_func = NULL;
 
-    /* "View.MemoryView":1099
+    /* "View.MemoryView":1101
  *     else:
  *         to_object_func = NULL
  *         to_dtype_func = NULL             # <<<<<<<<<<<<<<
  * 
  *     return memoryview_fromslice(memviewslice[0], memview.view.ndim,
  */
-    __Pyx_TraceLine(1099,0,__PYX_ERR(2, 1099, __pyx_L1_error))
+    __Pyx_TraceLine(1101,0,__PYX_ERR(2, 1101, __pyx_L1_error))
     __pyx_v_to_dtype_func = NULL;
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":1101
+  /* "View.MemoryView":1103
  *         to_dtype_func = NULL
  * 
  *     return memoryview_fromslice(memviewslice[0], memview.view.ndim,             # <<<<<<<<<<<<<<
  *                                 to_object_func, to_dtype_func,
  *                                 memview.dtype_is_object)
  */
-  __Pyx_TraceLine(1101,0,__PYX_ERR(2, 1101, __pyx_L1_error))
+  __Pyx_TraceLine(1103,0,__PYX_ERR(2, 1103, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
 
-  /* "View.MemoryView":1103
+  /* "View.MemoryView":1105
  *     return memoryview_fromslice(memviewslice[0], memview.view.ndim,
  *                                 to_object_func, to_dtype_func,
  *                                 memview.dtype_is_object)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_TraceLine(1103,0,__PYX_ERR(2, 1103, __pyx_L1_error))
-  __pyx_t_5 = __pyx_memoryview_fromslice((__pyx_v_memviewslice[0]), __pyx_v_memview->view.ndim, __pyx_v_to_object_func, __pyx_v_to_dtype_func, __pyx_v_memview->dtype_is_object); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 1101, __pyx_L1_error)
+  __Pyx_TraceLine(1105,0,__PYX_ERR(2, 1105, __pyx_L1_error))
+  __pyx_t_5 = __pyx_memoryview_fromslice((__pyx_v_memviewslice[0]), __pyx_v_memview->view.ndim, __pyx_v_to_object_func, __pyx_v_to_dtype_func, __pyx_v_memview->dtype_is_object); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 1103, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_r = __pyx_t_5;
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":1087
+  /* "View.MemoryView":1089
  * 
  * @cname('__pyx_memoryview_copy_object_from_slice')
  * cdef memoryview_copy_from_slice(memoryview memview, __Pyx_memviewslice *memviewslice):             # <<<<<<<<<<<<<<
  *     """
  *     Create a new memoryview object from a given memoryview object and slice.
  */
 
@@ -27462,76 +27656,76 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":1109
+/* "View.MemoryView":1111
  * 
  * 
  * cdef Py_ssize_t abs_py_ssize_t(Py_ssize_t arg) nogil:             # <<<<<<<<<<<<<<
  *     if arg < 0:
  *         return -arg
  */
 
 static Py_ssize_t abs_py_ssize_t(Py_ssize_t __pyx_v_arg) {
   Py_ssize_t __pyx_r;
   __Pyx_TraceDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_TraceCall("abs_py_ssize_t", __pyx_f[2], 1109, 1, __PYX_ERR(2, 1109, __pyx_L1_error));
+  __Pyx_TraceCall("abs_py_ssize_t", __pyx_f[2], 1111, 1, __PYX_ERR(2, 1111, __pyx_L1_error));
 
-  /* "View.MemoryView":1110
+  /* "View.MemoryView":1112
  * 
  * cdef Py_ssize_t abs_py_ssize_t(Py_ssize_t arg) nogil:
  *     if arg < 0:             # <<<<<<<<<<<<<<
  *         return -arg
  *     else:
  */
-  __Pyx_TraceLine(1110,1,__PYX_ERR(2, 1110, __pyx_L1_error))
+  __Pyx_TraceLine(1112,1,__PYX_ERR(2, 1112, __pyx_L1_error))
   __pyx_t_1 = ((__pyx_v_arg < 0) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":1111
+    /* "View.MemoryView":1113
  * cdef Py_ssize_t abs_py_ssize_t(Py_ssize_t arg) nogil:
  *     if arg < 0:
  *         return -arg             # <<<<<<<<<<<<<<
  *     else:
  *         return arg
  */
-    __Pyx_TraceLine(1111,1,__PYX_ERR(2, 1111, __pyx_L1_error))
+    __Pyx_TraceLine(1113,1,__PYX_ERR(2, 1113, __pyx_L1_error))
     __pyx_r = (-__pyx_v_arg);
     goto __pyx_L0;
 
-    /* "View.MemoryView":1110
+    /* "View.MemoryView":1112
  * 
  * cdef Py_ssize_t abs_py_ssize_t(Py_ssize_t arg) nogil:
  *     if arg < 0:             # <<<<<<<<<<<<<<
  *         return -arg
  *     else:
  */
   }
 
-  /* "View.MemoryView":1113
+  /* "View.MemoryView":1115
  *         return -arg
  *     else:
  *         return arg             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_get_best_slice_order')
  */
-  __Pyx_TraceLine(1113,1,__PYX_ERR(2, 1113, __pyx_L1_error))
+  __Pyx_TraceLine(1115,1,__PYX_ERR(2, 1115, __pyx_L1_error))
   /*else*/ {
     __pyx_r = __pyx_v_arg;
     goto __pyx_L0;
   }
 
-  /* "View.MemoryView":1109
+  /* "View.MemoryView":1111
  * 
  * 
  * cdef Py_ssize_t abs_py_ssize_t(Py_ssize_t arg) nogil:             # <<<<<<<<<<<<<<
  *     if arg < 0:
  *         return -arg
  */
 
@@ -27540,15 +27734,15 @@
   __Pyx_WriteUnraisable("View.MemoryView.abs_py_ssize_t", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 1);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
   return __pyx_r;
 }
 
-/* "View.MemoryView":1116
+/* "View.MemoryView":1118
  * 
  * @cname('__pyx_get_best_slice_order')
  * cdef char get_best_order(__Pyx_memviewslice *mslice, int ndim) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     Figure out the best memory access order for a given slice.
  */
 
@@ -27561,189 +27755,189 @@
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_TraceCall("get_best_order", __pyx_f[2], 1116, 1, __PYX_ERR(2, 1116, __pyx_L1_error));
+  __Pyx_TraceCall("get_best_order", __pyx_f[2], 1118, 1, __PYX_ERR(2, 1118, __pyx_L1_error));
 
-  /* "View.MemoryView":1121
+  /* "View.MemoryView":1123
  *     """
  *     cdef int i
  *     cdef Py_ssize_t c_stride = 0             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t f_stride = 0
  * 
  */
-  __Pyx_TraceLine(1121,1,__PYX_ERR(2, 1121, __pyx_L1_error))
+  __Pyx_TraceLine(1123,1,__PYX_ERR(2, 1123, __pyx_L1_error))
   __pyx_v_c_stride = 0;
 
-  /* "View.MemoryView":1122
+  /* "View.MemoryView":1124
  *     cdef int i
  *     cdef Py_ssize_t c_stride = 0
  *     cdef Py_ssize_t f_stride = 0             # <<<<<<<<<<<<<<
  * 
  *     for i in range(ndim - 1, -1, -1):
  */
-  __Pyx_TraceLine(1122,1,__PYX_ERR(2, 1122, __pyx_L1_error))
+  __Pyx_TraceLine(1124,1,__PYX_ERR(2, 1124, __pyx_L1_error))
   __pyx_v_f_stride = 0;
 
-  /* "View.MemoryView":1124
+  /* "View.MemoryView":1126
  *     cdef Py_ssize_t f_stride = 0
  * 
  *     for i in range(ndim - 1, -1, -1):             # <<<<<<<<<<<<<<
  *         if mslice.shape[i] > 1:
  *             c_stride = mslice.strides[i]
  */
-  __Pyx_TraceLine(1124,1,__PYX_ERR(2, 1124, __pyx_L1_error))
+  __Pyx_TraceLine(1126,1,__PYX_ERR(2, 1126, __pyx_L1_error))
   for (__pyx_t_1 = (__pyx_v_ndim - 1); __pyx_t_1 > -1; __pyx_t_1-=1) {
     __pyx_v_i = __pyx_t_1;
 
-    /* "View.MemoryView":1125
+    /* "View.MemoryView":1127
  * 
  *     for i in range(ndim - 1, -1, -1):
  *         if mslice.shape[i] > 1:             # <<<<<<<<<<<<<<
  *             c_stride = mslice.strides[i]
  *             break
  */
-    __Pyx_TraceLine(1125,1,__PYX_ERR(2, 1125, __pyx_L1_error))
+    __Pyx_TraceLine(1127,1,__PYX_ERR(2, 1127, __pyx_L1_error))
     __pyx_t_2 = (((__pyx_v_mslice->shape[__pyx_v_i]) > 1) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1126
+      /* "View.MemoryView":1128
  *     for i in range(ndim - 1, -1, -1):
  *         if mslice.shape[i] > 1:
  *             c_stride = mslice.strides[i]             # <<<<<<<<<<<<<<
  *             break
  * 
  */
-      __Pyx_TraceLine(1126,1,__PYX_ERR(2, 1126, __pyx_L1_error))
+      __Pyx_TraceLine(1128,1,__PYX_ERR(2, 1128, __pyx_L1_error))
       __pyx_v_c_stride = (__pyx_v_mslice->strides[__pyx_v_i]);
 
-      /* "View.MemoryView":1127
+      /* "View.MemoryView":1129
  *         if mslice.shape[i] > 1:
  *             c_stride = mslice.strides[i]
  *             break             # <<<<<<<<<<<<<<
  * 
  *     for i in range(ndim):
  */
-      __Pyx_TraceLine(1127,1,__PYX_ERR(2, 1127, __pyx_L1_error))
+      __Pyx_TraceLine(1129,1,__PYX_ERR(2, 1129, __pyx_L1_error))
       goto __pyx_L4_break;
 
-      /* "View.MemoryView":1125
+      /* "View.MemoryView":1127
  * 
  *     for i in range(ndim - 1, -1, -1):
  *         if mslice.shape[i] > 1:             # <<<<<<<<<<<<<<
  *             c_stride = mslice.strides[i]
  *             break
  */
     }
   }
   __pyx_L4_break:;
 
-  /* "View.MemoryView":1129
+  /* "View.MemoryView":1131
  *             break
  * 
  *     for i in range(ndim):             # <<<<<<<<<<<<<<
  *         if mslice.shape[i] > 1:
  *             f_stride = mslice.strides[i]
  */
-  __Pyx_TraceLine(1129,1,__PYX_ERR(2, 1129, __pyx_L1_error))
+  __Pyx_TraceLine(1131,1,__PYX_ERR(2, 1131, __pyx_L1_error))
   __pyx_t_1 = __pyx_v_ndim;
   __pyx_t_3 = __pyx_t_1;
   for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
     __pyx_v_i = __pyx_t_4;
 
-    /* "View.MemoryView":1130
+    /* "View.MemoryView":1132
  * 
  *     for i in range(ndim):
  *         if mslice.shape[i] > 1:             # <<<<<<<<<<<<<<
  *             f_stride = mslice.strides[i]
  *             break
  */
-    __Pyx_TraceLine(1130,1,__PYX_ERR(2, 1130, __pyx_L1_error))
+    __Pyx_TraceLine(1132,1,__PYX_ERR(2, 1132, __pyx_L1_error))
     __pyx_t_2 = (((__pyx_v_mslice->shape[__pyx_v_i]) > 1) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1131
+      /* "View.MemoryView":1133
  *     for i in range(ndim):
  *         if mslice.shape[i] > 1:
  *             f_stride = mslice.strides[i]             # <<<<<<<<<<<<<<
  *             break
  * 
  */
-      __Pyx_TraceLine(1131,1,__PYX_ERR(2, 1131, __pyx_L1_error))
+      __Pyx_TraceLine(1133,1,__PYX_ERR(2, 1133, __pyx_L1_error))
       __pyx_v_f_stride = (__pyx_v_mslice->strides[__pyx_v_i]);
 
-      /* "View.MemoryView":1132
+      /* "View.MemoryView":1134
  *         if mslice.shape[i] > 1:
  *             f_stride = mslice.strides[i]
  *             break             # <<<<<<<<<<<<<<
  * 
  *     if abs_py_ssize_t(c_stride) <= abs_py_ssize_t(f_stride):
  */
-      __Pyx_TraceLine(1132,1,__PYX_ERR(2, 1132, __pyx_L1_error))
+      __Pyx_TraceLine(1134,1,__PYX_ERR(2, 1134, __pyx_L1_error))
       goto __pyx_L7_break;
 
-      /* "View.MemoryView":1130
+      /* "View.MemoryView":1132
  * 
  *     for i in range(ndim):
  *         if mslice.shape[i] > 1:             # <<<<<<<<<<<<<<
  *             f_stride = mslice.strides[i]
  *             break
  */
     }
   }
   __pyx_L7_break:;
 
-  /* "View.MemoryView":1134
+  /* "View.MemoryView":1136
  *             break
  * 
  *     if abs_py_ssize_t(c_stride) <= abs_py_ssize_t(f_stride):             # <<<<<<<<<<<<<<
  *         return 'C'
  *     else:
  */
-  __Pyx_TraceLine(1134,1,__PYX_ERR(2, 1134, __pyx_L1_error))
+  __Pyx_TraceLine(1136,1,__PYX_ERR(2, 1136, __pyx_L1_error))
   __pyx_t_2 = ((abs_py_ssize_t(__pyx_v_c_stride) <= abs_py_ssize_t(__pyx_v_f_stride)) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1135
+    /* "View.MemoryView":1137
  * 
  *     if abs_py_ssize_t(c_stride) <= abs_py_ssize_t(f_stride):
  *         return 'C'             # <<<<<<<<<<<<<<
  *     else:
  *         return 'F'
  */
-    __Pyx_TraceLine(1135,1,__PYX_ERR(2, 1135, __pyx_L1_error))
+    __Pyx_TraceLine(1137,1,__PYX_ERR(2, 1137, __pyx_L1_error))
     __pyx_r = 'C';
     goto __pyx_L0;
 
-    /* "View.MemoryView":1134
+    /* "View.MemoryView":1136
  *             break
  * 
  *     if abs_py_ssize_t(c_stride) <= abs_py_ssize_t(f_stride):             # <<<<<<<<<<<<<<
  *         return 'C'
  *     else:
  */
   }
 
-  /* "View.MemoryView":1137
+  /* "View.MemoryView":1139
  *         return 'C'
  *     else:
  *         return 'F'             # <<<<<<<<<<<<<<
  * 
  * @cython.cdivision(True)
  */
-  __Pyx_TraceLine(1137,1,__PYX_ERR(2, 1137, __pyx_L1_error))
+  __Pyx_TraceLine(1139,1,__PYX_ERR(2, 1139, __pyx_L1_error))
   /*else*/ {
     __pyx_r = 'F';
     goto __pyx_L0;
   }
 
-  /* "View.MemoryView":1116
+  /* "View.MemoryView":1118
  * 
  * @cname('__pyx_get_best_slice_order')
  * cdef char get_best_order(__Pyx_memviewslice *mslice, int ndim) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     Figure out the best memory access order for a given slice.
  */
 
@@ -27752,15 +27946,15 @@
   __Pyx_WriteUnraisable("View.MemoryView.get_best_order", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 1);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
   return __pyx_r;
 }
 
-/* "View.MemoryView":1140
+/* "View.MemoryView":1142
  * 
  * @cython.cdivision(True)
  * cdef void _copy_strided_to_strided(char *src_data, Py_ssize_t *src_strides,             # <<<<<<<<<<<<<<
  *                                    char *dst_data, Py_ssize_t *dst_strides,
  *                                    Py_ssize_t *src_shape, Py_ssize_t *dst_shape,
  */
 
@@ -27773,61 +27967,61 @@
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   Py_ssize_t __pyx_t_4;
   Py_ssize_t __pyx_t_5;
   Py_ssize_t __pyx_t_6;
 
-  /* "View.MemoryView":1147
+  /* "View.MemoryView":1149
  * 
  *     cdef Py_ssize_t i
  *     cdef Py_ssize_t src_extent = src_shape[0]             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t dst_extent = dst_shape[0]
  *     cdef Py_ssize_t src_stride = src_strides[0]
  */
   __pyx_v_src_extent = (__pyx_v_src_shape[0]);
 
-  /* "View.MemoryView":1148
+  /* "View.MemoryView":1150
  *     cdef Py_ssize_t i
  *     cdef Py_ssize_t src_extent = src_shape[0]
  *     cdef Py_ssize_t dst_extent = dst_shape[0]             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t src_stride = src_strides[0]
  *     cdef Py_ssize_t dst_stride = dst_strides[0]
  */
   __pyx_v_dst_extent = (__pyx_v_dst_shape[0]);
 
-  /* "View.MemoryView":1149
+  /* "View.MemoryView":1151
  *     cdef Py_ssize_t src_extent = src_shape[0]
  *     cdef Py_ssize_t dst_extent = dst_shape[0]
  *     cdef Py_ssize_t src_stride = src_strides[0]             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t dst_stride = dst_strides[0]
  * 
  */
   __pyx_v_src_stride = (__pyx_v_src_strides[0]);
 
-  /* "View.MemoryView":1150
+  /* "View.MemoryView":1152
  *     cdef Py_ssize_t dst_extent = dst_shape[0]
  *     cdef Py_ssize_t src_stride = src_strides[0]
  *     cdef Py_ssize_t dst_stride = dst_strides[0]             # <<<<<<<<<<<<<<
  * 
  *     if ndim == 1:
  */
   __pyx_v_dst_stride = (__pyx_v_dst_strides[0]);
 
-  /* "View.MemoryView":1152
+  /* "View.MemoryView":1154
  *     cdef Py_ssize_t dst_stride = dst_strides[0]
  * 
  *     if ndim == 1:             # <<<<<<<<<<<<<<
  *        if (src_stride > 0 and dst_stride > 0 and
  *            <size_t> src_stride == itemsize == <size_t> dst_stride):
  */
   __pyx_t_1 = ((__pyx_v_ndim == 1) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":1153
+    /* "View.MemoryView":1155
  * 
  *     if ndim == 1:
  *        if (src_stride > 0 and dst_stride > 0 and             # <<<<<<<<<<<<<<
  *            <size_t> src_stride == itemsize == <size_t> dst_stride):
  *            memcpy(dst_data, src_data, itemsize * dst_extent)
  */
     __pyx_t_2 = ((__pyx_v_src_stride > 0) != 0);
@@ -27839,190 +28033,190 @@
     __pyx_t_2 = ((__pyx_v_dst_stride > 0) != 0);
     if (__pyx_t_2) {
     } else {
       __pyx_t_1 = __pyx_t_2;
       goto __pyx_L5_bool_binop_done;
     }
 
-    /* "View.MemoryView":1154
+    /* "View.MemoryView":1156
  *     if ndim == 1:
  *        if (src_stride > 0 and dst_stride > 0 and
  *            <size_t> src_stride == itemsize == <size_t> dst_stride):             # <<<<<<<<<<<<<<
  *            memcpy(dst_data, src_data, itemsize * dst_extent)
  *        else:
  */
     __pyx_t_2 = (((size_t)__pyx_v_src_stride) == __pyx_v_itemsize);
     if (__pyx_t_2) {
       __pyx_t_2 = (__pyx_v_itemsize == ((size_t)__pyx_v_dst_stride));
     }
     __pyx_t_3 = (__pyx_t_2 != 0);
     __pyx_t_1 = __pyx_t_3;
     __pyx_L5_bool_binop_done:;
 
-    /* "View.MemoryView":1153
+    /* "View.MemoryView":1155
  * 
  *     if ndim == 1:
  *        if (src_stride > 0 and dst_stride > 0 and             # <<<<<<<<<<<<<<
  *            <size_t> src_stride == itemsize == <size_t> dst_stride):
  *            memcpy(dst_data, src_data, itemsize * dst_extent)
  */
     if (__pyx_t_1) {
 
-      /* "View.MemoryView":1155
+      /* "View.MemoryView":1157
  *        if (src_stride > 0 and dst_stride > 0 and
  *            <size_t> src_stride == itemsize == <size_t> dst_stride):
  *            memcpy(dst_data, src_data, itemsize * dst_extent)             # <<<<<<<<<<<<<<
  *        else:
  *            for i in range(dst_extent):
  */
       (void)(memcpy(__pyx_v_dst_data, __pyx_v_src_data, (__pyx_v_itemsize * __pyx_v_dst_extent)));
 
-      /* "View.MemoryView":1153
+      /* "View.MemoryView":1155
  * 
  *     if ndim == 1:
  *        if (src_stride > 0 and dst_stride > 0 and             # <<<<<<<<<<<<<<
  *            <size_t> src_stride == itemsize == <size_t> dst_stride):
  *            memcpy(dst_data, src_data, itemsize * dst_extent)
  */
       goto __pyx_L4;
     }
 
-    /* "View.MemoryView":1157
+    /* "View.MemoryView":1159
  *            memcpy(dst_data, src_data, itemsize * dst_extent)
  *        else:
  *            for i in range(dst_extent):             # <<<<<<<<<<<<<<
  *                memcpy(dst_data, src_data, itemsize)
  *                src_data += src_stride
  */
     /*else*/ {
       __pyx_t_4 = __pyx_v_dst_extent;
       __pyx_t_5 = __pyx_t_4;
       for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
         __pyx_v_i = __pyx_t_6;
 
-        /* "View.MemoryView":1158
+        /* "View.MemoryView":1160
  *        else:
  *            for i in range(dst_extent):
  *                memcpy(dst_data, src_data, itemsize)             # <<<<<<<<<<<<<<
  *                src_data += src_stride
  *                dst_data += dst_stride
  */
         (void)(memcpy(__pyx_v_dst_data, __pyx_v_src_data, __pyx_v_itemsize));
 
-        /* "View.MemoryView":1159
+        /* "View.MemoryView":1161
  *            for i in range(dst_extent):
  *                memcpy(dst_data, src_data, itemsize)
  *                src_data += src_stride             # <<<<<<<<<<<<<<
  *                dst_data += dst_stride
  *     else:
  */
         __pyx_v_src_data = (__pyx_v_src_data + __pyx_v_src_stride);
 
-        /* "View.MemoryView":1160
+        /* "View.MemoryView":1162
  *                memcpy(dst_data, src_data, itemsize)
  *                src_data += src_stride
  *                dst_data += dst_stride             # <<<<<<<<<<<<<<
  *     else:
  *         for i in range(dst_extent):
  */
         __pyx_v_dst_data = (__pyx_v_dst_data + __pyx_v_dst_stride);
       }
     }
     __pyx_L4:;
 
-    /* "View.MemoryView":1152
+    /* "View.MemoryView":1154
  *     cdef Py_ssize_t dst_stride = dst_strides[0]
  * 
  *     if ndim == 1:             # <<<<<<<<<<<<<<
  *        if (src_stride > 0 and dst_stride > 0 and
  *            <size_t> src_stride == itemsize == <size_t> dst_stride):
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":1162
+  /* "View.MemoryView":1164
  *                dst_data += dst_stride
  *     else:
  *         for i in range(dst_extent):             # <<<<<<<<<<<<<<
  *             _copy_strided_to_strided(src_data, src_strides + 1,
  *                                      dst_data, dst_strides + 1,
  */
   /*else*/ {
     __pyx_t_4 = __pyx_v_dst_extent;
     __pyx_t_5 = __pyx_t_4;
     for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
       __pyx_v_i = __pyx_t_6;
 
-      /* "View.MemoryView":1163
+      /* "View.MemoryView":1165
  *     else:
  *         for i in range(dst_extent):
  *             _copy_strided_to_strided(src_data, src_strides + 1,             # <<<<<<<<<<<<<<
  *                                      dst_data, dst_strides + 1,
  *                                      src_shape + 1, dst_shape + 1,
  */
       _copy_strided_to_strided(__pyx_v_src_data, (__pyx_v_src_strides + 1), __pyx_v_dst_data, (__pyx_v_dst_strides + 1), (__pyx_v_src_shape + 1), (__pyx_v_dst_shape + 1), (__pyx_v_ndim - 1), __pyx_v_itemsize);
 
-      /* "View.MemoryView":1167
+      /* "View.MemoryView":1169
  *                                      src_shape + 1, dst_shape + 1,
  *                                      ndim - 1, itemsize)
  *             src_data += src_stride             # <<<<<<<<<<<<<<
  *             dst_data += dst_stride
  * 
  */
       __pyx_v_src_data = (__pyx_v_src_data + __pyx_v_src_stride);
 
-      /* "View.MemoryView":1168
+      /* "View.MemoryView":1170
  *                                      ndim - 1, itemsize)
  *             src_data += src_stride
  *             dst_data += dst_stride             # <<<<<<<<<<<<<<
  * 
  * cdef void copy_strided_to_strided(__Pyx_memviewslice *src,
  */
       __pyx_v_dst_data = (__pyx_v_dst_data + __pyx_v_dst_stride);
     }
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":1140
+  /* "View.MemoryView":1142
  * 
  * @cython.cdivision(True)
  * cdef void _copy_strided_to_strided(char *src_data, Py_ssize_t *src_strides,             # <<<<<<<<<<<<<<
  *                                    char *dst_data, Py_ssize_t *dst_strides,
  *                                    Py_ssize_t *src_shape, Py_ssize_t *dst_shape,
  */
 
   /* function exit code */
 }
 
-/* "View.MemoryView":1170
+/* "View.MemoryView":1172
  *             dst_data += dst_stride
  * 
  * cdef void copy_strided_to_strided(__Pyx_memviewslice *src,             # <<<<<<<<<<<<<<
  *                                   __Pyx_memviewslice *dst,
  *                                   int ndim, size_t itemsize) nogil:
  */
 
 static void copy_strided_to_strided(__Pyx_memviewslice *__pyx_v_src, __Pyx_memviewslice *__pyx_v_dst, int __pyx_v_ndim, size_t __pyx_v_itemsize) {
   __Pyx_TraceDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_TraceCall("copy_strided_to_strided", __pyx_f[2], 1170, 1, __PYX_ERR(2, 1170, __pyx_L1_error));
+  __Pyx_TraceCall("copy_strided_to_strided", __pyx_f[2], 1172, 1, __PYX_ERR(2, 1172, __pyx_L1_error));
 
-  /* "View.MemoryView":1173
+  /* "View.MemoryView":1175
  *                                   __Pyx_memviewslice *dst,
  *                                   int ndim, size_t itemsize) nogil:
  *     _copy_strided_to_strided(src.data, src.strides, dst.data, dst.strides,             # <<<<<<<<<<<<<<
  *                              src.shape, dst.shape, ndim, itemsize)
  * 
  */
-  __Pyx_TraceLine(1173,1,__PYX_ERR(2, 1173, __pyx_L1_error))
+  __Pyx_TraceLine(1175,1,__PYX_ERR(2, 1175, __pyx_L1_error))
   _copy_strided_to_strided(__pyx_v_src->data, __pyx_v_src->strides, __pyx_v_dst->data, __pyx_v_dst->strides, __pyx_v_src->shape, __pyx_v_dst->shape, __pyx_v_ndim, __pyx_v_itemsize);
 
-  /* "View.MemoryView":1170
+  /* "View.MemoryView":1172
  *             dst_data += dst_stride
  * 
  * cdef void copy_strided_to_strided(__Pyx_memviewslice *src,             # <<<<<<<<<<<<<<
  *                                   __Pyx_memviewslice *dst,
  *                                   int ndim, size_t itemsize) nogil:
  */
 
@@ -28030,15 +28224,15 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("View.MemoryView.copy_strided_to_strided", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 1);
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
 }
 
-/* "View.MemoryView":1177
+/* "View.MemoryView":1179
  * 
  * @cname('__pyx_memoryview_slice_get_size')
  * cdef Py_ssize_t slice_get_size(__Pyx_memviewslice *src, int ndim) nogil:             # <<<<<<<<<<<<<<
  *     "Return the size of the memory occupied by the slice in number of bytes"
  *     cdef Py_ssize_t shape, size = src.memview.view.itemsize
  */
 
@@ -28050,63 +28244,63 @@
   Py_ssize_t __pyx_t_1;
   Py_ssize_t *__pyx_t_2;
   Py_ssize_t *__pyx_t_3;
   Py_ssize_t *__pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_TraceCall("slice_get_size", __pyx_f[2], 1177, 1, __PYX_ERR(2, 1177, __pyx_L1_error));
+  __Pyx_TraceCall("slice_get_size", __pyx_f[2], 1179, 1, __PYX_ERR(2, 1179, __pyx_L1_error));
 
-  /* "View.MemoryView":1179
+  /* "View.MemoryView":1181
  * cdef Py_ssize_t slice_get_size(__Pyx_memviewslice *src, int ndim) nogil:
  *     "Return the size of the memory occupied by the slice in number of bytes"
  *     cdef Py_ssize_t shape, size = src.memview.view.itemsize             # <<<<<<<<<<<<<<
  * 
  *     for shape in src.shape[:ndim]:
  */
-  __Pyx_TraceLine(1179,1,__PYX_ERR(2, 1179, __pyx_L1_error))
+  __Pyx_TraceLine(1181,1,__PYX_ERR(2, 1181, __pyx_L1_error))
   __pyx_t_1 = __pyx_v_src->memview->view.itemsize;
   __pyx_v_size = __pyx_t_1;
 
-  /* "View.MemoryView":1181
+  /* "View.MemoryView":1183
  *     cdef Py_ssize_t shape, size = src.memview.view.itemsize
  * 
  *     for shape in src.shape[:ndim]:             # <<<<<<<<<<<<<<
  *         size *= shape
  * 
  */
-  __Pyx_TraceLine(1181,1,__PYX_ERR(2, 1181, __pyx_L1_error))
+  __Pyx_TraceLine(1183,1,__PYX_ERR(2, 1183, __pyx_L1_error))
   __pyx_t_3 = (__pyx_v_src->shape + __pyx_v_ndim);
   for (__pyx_t_4 = __pyx_v_src->shape; __pyx_t_4 < __pyx_t_3; __pyx_t_4++) {
     __pyx_t_2 = __pyx_t_4;
     __pyx_v_shape = (__pyx_t_2[0]);
 
-    /* "View.MemoryView":1182
+    /* "View.MemoryView":1184
  * 
  *     for shape in src.shape[:ndim]:
  *         size *= shape             # <<<<<<<<<<<<<<
  * 
  *     return size
  */
-    __Pyx_TraceLine(1182,1,__PYX_ERR(2, 1182, __pyx_L1_error))
+    __Pyx_TraceLine(1184,1,__PYX_ERR(2, 1184, __pyx_L1_error))
     __pyx_v_size = (__pyx_v_size * __pyx_v_shape);
   }
 
-  /* "View.MemoryView":1184
+  /* "View.MemoryView":1186
  *         size *= shape
  * 
  *     return size             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_fill_contig_strides_array')
  */
-  __Pyx_TraceLine(1184,1,__PYX_ERR(2, 1184, __pyx_L1_error))
+  __Pyx_TraceLine(1186,1,__PYX_ERR(2, 1186, __pyx_L1_error))
   __pyx_r = __pyx_v_size;
   goto __pyx_L0;
 
-  /* "View.MemoryView":1177
+  /* "View.MemoryView":1179
  * 
  * @cname('__pyx_memoryview_slice_get_size')
  * cdef Py_ssize_t slice_get_size(__Pyx_memviewslice *src, int ndim) nogil:             # <<<<<<<<<<<<<<
  *     "Return the size of the memory occupied by the slice in number of bytes"
  *     cdef Py_ssize_t shape, size = src.memview.view.itemsize
  */
 
@@ -28115,15 +28309,15 @@
   __Pyx_WriteUnraisable("View.MemoryView.slice_get_size", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 1);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
   return __pyx_r;
 }
 
-/* "View.MemoryView":1187
+/* "View.MemoryView":1189
  * 
  * @cname('__pyx_fill_contig_strides_array')
  * cdef Py_ssize_t fill_contig_strides_array(             # <<<<<<<<<<<<<<
  *                 Py_ssize_t *shape, Py_ssize_t *strides, Py_ssize_t stride,
  *                 int ndim, char order) nogil:
  */
 
@@ -28134,118 +28328,118 @@
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_TraceCall("fill_contig_strides_array", __pyx_f[2], 1187, 1, __PYX_ERR(2, 1187, __pyx_L1_error));
+  __Pyx_TraceCall("fill_contig_strides_array", __pyx_f[2], 1189, 1, __PYX_ERR(2, 1189, __pyx_L1_error));
 
-  /* "View.MemoryView":1196
+  /* "View.MemoryView":1198
  *     cdef int idx
  * 
  *     if order == 'F':             # <<<<<<<<<<<<<<
  *         for idx in range(ndim):
  *             strides[idx] = stride
  */
-  __Pyx_TraceLine(1196,1,__PYX_ERR(2, 1196, __pyx_L1_error))
+  __Pyx_TraceLine(1198,1,__PYX_ERR(2, 1198, __pyx_L1_error))
   __pyx_t_1 = ((__pyx_v_order == 'F') != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":1197
+    /* "View.MemoryView":1199
  * 
  *     if order == 'F':
  *         for idx in range(ndim):             # <<<<<<<<<<<<<<
  *             strides[idx] = stride
  *             stride *= shape[idx]
  */
-    __Pyx_TraceLine(1197,1,__PYX_ERR(2, 1197, __pyx_L1_error))
+    __Pyx_TraceLine(1199,1,__PYX_ERR(2, 1199, __pyx_L1_error))
     __pyx_t_2 = __pyx_v_ndim;
     __pyx_t_3 = __pyx_t_2;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_v_idx = __pyx_t_4;
 
-      /* "View.MemoryView":1198
+      /* "View.MemoryView":1200
  *     if order == 'F':
  *         for idx in range(ndim):
  *             strides[idx] = stride             # <<<<<<<<<<<<<<
  *             stride *= shape[idx]
  *     else:
  */
-      __Pyx_TraceLine(1198,1,__PYX_ERR(2, 1198, __pyx_L1_error))
+      __Pyx_TraceLine(1200,1,__PYX_ERR(2, 1200, __pyx_L1_error))
       (__pyx_v_strides[__pyx_v_idx]) = __pyx_v_stride;
 
-      /* "View.MemoryView":1199
+      /* "View.MemoryView":1201
  *         for idx in range(ndim):
  *             strides[idx] = stride
  *             stride *= shape[idx]             # <<<<<<<<<<<<<<
  *     else:
  *         for idx in range(ndim - 1, -1, -1):
  */
-      __Pyx_TraceLine(1199,1,__PYX_ERR(2, 1199, __pyx_L1_error))
+      __Pyx_TraceLine(1201,1,__PYX_ERR(2, 1201, __pyx_L1_error))
       __pyx_v_stride = (__pyx_v_stride * (__pyx_v_shape[__pyx_v_idx]));
     }
 
-    /* "View.MemoryView":1196
+    /* "View.MemoryView":1198
  *     cdef int idx
  * 
  *     if order == 'F':             # <<<<<<<<<<<<<<
  *         for idx in range(ndim):
  *             strides[idx] = stride
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":1201
+  /* "View.MemoryView":1203
  *             stride *= shape[idx]
  *     else:
  *         for idx in range(ndim - 1, -1, -1):             # <<<<<<<<<<<<<<
  *             strides[idx] = stride
  *             stride *= shape[idx]
  */
-  __Pyx_TraceLine(1201,1,__PYX_ERR(2, 1201, __pyx_L1_error))
+  __Pyx_TraceLine(1203,1,__PYX_ERR(2, 1203, __pyx_L1_error))
   /*else*/ {
     for (__pyx_t_2 = (__pyx_v_ndim - 1); __pyx_t_2 > -1; __pyx_t_2-=1) {
       __pyx_v_idx = __pyx_t_2;
 
-      /* "View.MemoryView":1202
+      /* "View.MemoryView":1204
  *     else:
  *         for idx in range(ndim - 1, -1, -1):
  *             strides[idx] = stride             # <<<<<<<<<<<<<<
  *             stride *= shape[idx]
  * 
  */
-      __Pyx_TraceLine(1202,1,__PYX_ERR(2, 1202, __pyx_L1_error))
+      __Pyx_TraceLine(1204,1,__PYX_ERR(2, 1204, __pyx_L1_error))
       (__pyx_v_strides[__pyx_v_idx]) = __pyx_v_stride;
 
-      /* "View.MemoryView":1203
+      /* "View.MemoryView":1205
  *         for idx in range(ndim - 1, -1, -1):
  *             strides[idx] = stride
  *             stride *= shape[idx]             # <<<<<<<<<<<<<<
  * 
  *     return stride
  */
-      __Pyx_TraceLine(1203,1,__PYX_ERR(2, 1203, __pyx_L1_error))
+      __Pyx_TraceLine(1205,1,__PYX_ERR(2, 1205, __pyx_L1_error))
       __pyx_v_stride = (__pyx_v_stride * (__pyx_v_shape[__pyx_v_idx]));
     }
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":1205
+  /* "View.MemoryView":1207
  *             stride *= shape[idx]
  * 
  *     return stride             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_copy_data_to_temp')
  */
-  __Pyx_TraceLine(1205,1,__PYX_ERR(2, 1205, __pyx_L1_error))
+  __Pyx_TraceLine(1207,1,__PYX_ERR(2, 1207, __pyx_L1_error))
   __pyx_r = __pyx_v_stride;
   goto __pyx_L0;
 
-  /* "View.MemoryView":1187
+  /* "View.MemoryView":1189
  * 
  * @cname('__pyx_fill_contig_strides_array')
  * cdef Py_ssize_t fill_contig_strides_array(             # <<<<<<<<<<<<<<
  *                 Py_ssize_t *shape, Py_ssize_t *strides, Py_ssize_t stride,
  *                 int ndim, char order) nogil:
  */
 
@@ -28254,15 +28448,15 @@
   __Pyx_WriteUnraisable("View.MemoryView.fill_contig_strides_array", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 1);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
   return __pyx_r;
 }
 
-/* "View.MemoryView":1208
+/* "View.MemoryView":1210
  * 
  * @cname('__pyx_memoryview_copy_data_to_temp')
  * cdef void *copy_data_to_temp(__Pyx_memviewslice *src,             # <<<<<<<<<<<<<<
  *                              __Pyx_memviewslice *tmpslice,
  *                              char order,
  */
 
@@ -28278,242 +28472,242 @@
   int __pyx_t_3;
   struct __pyx_memoryview_obj *__pyx_t_4;
   int __pyx_t_5;
   int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_TraceCall("copy_data_to_temp", __pyx_f[2], 1208, 1, __PYX_ERR(2, 1208, __pyx_L1_error));
+  __Pyx_TraceCall("copy_data_to_temp", __pyx_f[2], 1210, 1, __PYX_ERR(2, 1210, __pyx_L1_error));
 
-  /* "View.MemoryView":1219
+  /* "View.MemoryView":1221
  *     cdef void *result
  * 
  *     cdef size_t itemsize = src.memview.view.itemsize             # <<<<<<<<<<<<<<
  *     cdef size_t size = slice_get_size(src, ndim)
  * 
  */
-  __Pyx_TraceLine(1219,1,__PYX_ERR(2, 1219, __pyx_L1_error))
+  __Pyx_TraceLine(1221,1,__PYX_ERR(2, 1221, __pyx_L1_error))
   __pyx_t_1 = __pyx_v_src->memview->view.itemsize;
   __pyx_v_itemsize = __pyx_t_1;
 
-  /* "View.MemoryView":1220
+  /* "View.MemoryView":1222
  * 
  *     cdef size_t itemsize = src.memview.view.itemsize
  *     cdef size_t size = slice_get_size(src, ndim)             # <<<<<<<<<<<<<<
  * 
  *     result = malloc(size)
  */
-  __Pyx_TraceLine(1220,1,__PYX_ERR(2, 1220, __pyx_L1_error))
+  __Pyx_TraceLine(1222,1,__PYX_ERR(2, 1222, __pyx_L1_error))
   __pyx_v_size = __pyx_memoryview_slice_get_size(__pyx_v_src, __pyx_v_ndim);
 
-  /* "View.MemoryView":1222
+  /* "View.MemoryView":1224
  *     cdef size_t size = slice_get_size(src, ndim)
  * 
  *     result = malloc(size)             # <<<<<<<<<<<<<<
  *     if not result:
  *         _err(MemoryError, NULL)
  */
-  __Pyx_TraceLine(1222,1,__PYX_ERR(2, 1222, __pyx_L1_error))
+  __Pyx_TraceLine(1224,1,__PYX_ERR(2, 1224, __pyx_L1_error))
   __pyx_v_result = malloc(__pyx_v_size);
 
-  /* "View.MemoryView":1223
+  /* "View.MemoryView":1225
  * 
  *     result = malloc(size)
  *     if not result:             # <<<<<<<<<<<<<<
  *         _err(MemoryError, NULL)
  * 
  */
-  __Pyx_TraceLine(1223,1,__PYX_ERR(2, 1223, __pyx_L1_error))
+  __Pyx_TraceLine(1225,1,__PYX_ERR(2, 1225, __pyx_L1_error))
   __pyx_t_2 = ((!(__pyx_v_result != 0)) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1224
+    /* "View.MemoryView":1226
  *     result = malloc(size)
  *     if not result:
  *         _err(MemoryError, NULL)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __Pyx_TraceLine(1224,1,__PYX_ERR(2, 1224, __pyx_L1_error))
-    __pyx_t_3 = __pyx_memoryview_err(__pyx_builtin_MemoryError, NULL); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(2, 1224, __pyx_L1_error)
+    __Pyx_TraceLine(1226,1,__PYX_ERR(2, 1226, __pyx_L1_error))
+    __pyx_t_3 = __pyx_memoryview_err(__pyx_builtin_MemoryError, NULL); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(2, 1226, __pyx_L1_error)
 
-    /* "View.MemoryView":1223
+    /* "View.MemoryView":1225
  * 
  *     result = malloc(size)
  *     if not result:             # <<<<<<<<<<<<<<
  *         _err(MemoryError, NULL)
  * 
  */
   }
 
-  /* "View.MemoryView":1227
+  /* "View.MemoryView":1229
  * 
  * 
  *     tmpslice.data = <char *> result             # <<<<<<<<<<<<<<
  *     tmpslice.memview = src.memview
  *     for i in range(ndim):
  */
-  __Pyx_TraceLine(1227,1,__PYX_ERR(2, 1227, __pyx_L1_error))
+  __Pyx_TraceLine(1229,1,__PYX_ERR(2, 1229, __pyx_L1_error))
   __pyx_v_tmpslice->data = ((char *)__pyx_v_result);
 
-  /* "View.MemoryView":1228
+  /* "View.MemoryView":1230
  * 
  *     tmpslice.data = <char *> result
  *     tmpslice.memview = src.memview             # <<<<<<<<<<<<<<
  *     for i in range(ndim):
  *         tmpslice.shape[i] = src.shape[i]
  */
-  __Pyx_TraceLine(1228,1,__PYX_ERR(2, 1228, __pyx_L1_error))
+  __Pyx_TraceLine(1230,1,__PYX_ERR(2, 1230, __pyx_L1_error))
   __pyx_t_4 = __pyx_v_src->memview;
   __pyx_v_tmpslice->memview = __pyx_t_4;
 
-  /* "View.MemoryView":1229
+  /* "View.MemoryView":1231
  *     tmpslice.data = <char *> result
  *     tmpslice.memview = src.memview
  *     for i in range(ndim):             # <<<<<<<<<<<<<<
  *         tmpslice.shape[i] = src.shape[i]
  *         tmpslice.suboffsets[i] = -1
  */
-  __Pyx_TraceLine(1229,1,__PYX_ERR(2, 1229, __pyx_L1_error))
+  __Pyx_TraceLine(1231,1,__PYX_ERR(2, 1231, __pyx_L1_error))
   __pyx_t_3 = __pyx_v_ndim;
   __pyx_t_5 = __pyx_t_3;
   for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
     __pyx_v_i = __pyx_t_6;
 
-    /* "View.MemoryView":1230
+    /* "View.MemoryView":1232
  *     tmpslice.memview = src.memview
  *     for i in range(ndim):
  *         tmpslice.shape[i] = src.shape[i]             # <<<<<<<<<<<<<<
  *         tmpslice.suboffsets[i] = -1
  * 
  */
-    __Pyx_TraceLine(1230,1,__PYX_ERR(2, 1230, __pyx_L1_error))
+    __Pyx_TraceLine(1232,1,__PYX_ERR(2, 1232, __pyx_L1_error))
     (__pyx_v_tmpslice->shape[__pyx_v_i]) = (__pyx_v_src->shape[__pyx_v_i]);
 
-    /* "View.MemoryView":1231
+    /* "View.MemoryView":1233
  *     for i in range(ndim):
  *         tmpslice.shape[i] = src.shape[i]
  *         tmpslice.suboffsets[i] = -1             # <<<<<<<<<<<<<<
  * 
  *     fill_contig_strides_array(&tmpslice.shape[0], &tmpslice.strides[0], itemsize,
  */
-    __Pyx_TraceLine(1231,1,__PYX_ERR(2, 1231, __pyx_L1_error))
+    __Pyx_TraceLine(1233,1,__PYX_ERR(2, 1233, __pyx_L1_error))
     (__pyx_v_tmpslice->suboffsets[__pyx_v_i]) = -1L;
   }
 
-  /* "View.MemoryView":1233
+  /* "View.MemoryView":1235
  *         tmpslice.suboffsets[i] = -1
  * 
  *     fill_contig_strides_array(&tmpslice.shape[0], &tmpslice.strides[0], itemsize,             # <<<<<<<<<<<<<<
  *                               ndim, order)
  * 
  */
-  __Pyx_TraceLine(1233,1,__PYX_ERR(2, 1233, __pyx_L1_error))
+  __Pyx_TraceLine(1235,1,__PYX_ERR(2, 1235, __pyx_L1_error))
   (void)(__pyx_fill_contig_strides_array((&(__pyx_v_tmpslice->shape[0])), (&(__pyx_v_tmpslice->strides[0])), __pyx_v_itemsize, __pyx_v_ndim, __pyx_v_order));
 
-  /* "View.MemoryView":1237
+  /* "View.MemoryView":1239
  * 
  * 
  *     for i in range(ndim):             # <<<<<<<<<<<<<<
  *         if tmpslice.shape[i] == 1:
  *             tmpslice.strides[i] = 0
  */
-  __Pyx_TraceLine(1237,1,__PYX_ERR(2, 1237, __pyx_L1_error))
+  __Pyx_TraceLine(1239,1,__PYX_ERR(2, 1239, __pyx_L1_error))
   __pyx_t_3 = __pyx_v_ndim;
   __pyx_t_5 = __pyx_t_3;
   for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
     __pyx_v_i = __pyx_t_6;
 
-    /* "View.MemoryView":1238
+    /* "View.MemoryView":1240
  * 
  *     for i in range(ndim):
  *         if tmpslice.shape[i] == 1:             # <<<<<<<<<<<<<<
  *             tmpslice.strides[i] = 0
  * 
  */
-    __Pyx_TraceLine(1238,1,__PYX_ERR(2, 1238, __pyx_L1_error))
+    __Pyx_TraceLine(1240,1,__PYX_ERR(2, 1240, __pyx_L1_error))
     __pyx_t_2 = (((__pyx_v_tmpslice->shape[__pyx_v_i]) == 1) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1239
+      /* "View.MemoryView":1241
  *     for i in range(ndim):
  *         if tmpslice.shape[i] == 1:
  *             tmpslice.strides[i] = 0             # <<<<<<<<<<<<<<
  * 
  *     if slice_is_contig(src[0], order, ndim):
  */
-      __Pyx_TraceLine(1239,1,__PYX_ERR(2, 1239, __pyx_L1_error))
+      __Pyx_TraceLine(1241,1,__PYX_ERR(2, 1241, __pyx_L1_error))
       (__pyx_v_tmpslice->strides[__pyx_v_i]) = 0;
 
-      /* "View.MemoryView":1238
+      /* "View.MemoryView":1240
  * 
  *     for i in range(ndim):
  *         if tmpslice.shape[i] == 1:             # <<<<<<<<<<<<<<
  *             tmpslice.strides[i] = 0
  * 
  */
     }
   }
 
-  /* "View.MemoryView":1241
+  /* "View.MemoryView":1243
  *             tmpslice.strides[i] = 0
  * 
  *     if slice_is_contig(src[0], order, ndim):             # <<<<<<<<<<<<<<
  *         memcpy(result, src.data, size)
  *     else:
  */
-  __Pyx_TraceLine(1241,1,__PYX_ERR(2, 1241, __pyx_L1_error))
+  __Pyx_TraceLine(1243,1,__PYX_ERR(2, 1243, __pyx_L1_error))
   __pyx_t_2 = (__pyx_memviewslice_is_contig((__pyx_v_src[0]), __pyx_v_order, __pyx_v_ndim) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1242
+    /* "View.MemoryView":1244
  * 
  *     if slice_is_contig(src[0], order, ndim):
  *         memcpy(result, src.data, size)             # <<<<<<<<<<<<<<
  *     else:
  *         copy_strided_to_strided(src, tmpslice, ndim, itemsize)
  */
-    __Pyx_TraceLine(1242,1,__PYX_ERR(2, 1242, __pyx_L1_error))
+    __Pyx_TraceLine(1244,1,__PYX_ERR(2, 1244, __pyx_L1_error))
     (void)(memcpy(__pyx_v_result, __pyx_v_src->data, __pyx_v_size));
 
-    /* "View.MemoryView":1241
+    /* "View.MemoryView":1243
  *             tmpslice.strides[i] = 0
  * 
  *     if slice_is_contig(src[0], order, ndim):             # <<<<<<<<<<<<<<
  *         memcpy(result, src.data, size)
  *     else:
  */
     goto __pyx_L9;
   }
 
-  /* "View.MemoryView":1244
+  /* "View.MemoryView":1246
  *         memcpy(result, src.data, size)
  *     else:
  *         copy_strided_to_strided(src, tmpslice, ndim, itemsize)             # <<<<<<<<<<<<<<
  * 
  *     return result
  */
-  __Pyx_TraceLine(1244,1,__PYX_ERR(2, 1244, __pyx_L1_error))
+  __Pyx_TraceLine(1246,1,__PYX_ERR(2, 1246, __pyx_L1_error))
   /*else*/ {
     copy_strided_to_strided(__pyx_v_src, __pyx_v_tmpslice, __pyx_v_ndim, __pyx_v_itemsize);
   }
   __pyx_L9:;
 
-  /* "View.MemoryView":1246
+  /* "View.MemoryView":1248
  *         copy_strided_to_strided(src, tmpslice, ndim, itemsize)
  * 
  *     return result             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_TraceLine(1246,1,__PYX_ERR(2, 1246, __pyx_L1_error))
+  __Pyx_TraceLine(1248,1,__PYX_ERR(2, 1248, __pyx_L1_error))
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "View.MemoryView":1208
+  /* "View.MemoryView":1210
  * 
  * @cname('__pyx_memoryview_copy_data_to_temp')
  * cdef void *copy_data_to_temp(__Pyx_memviewslice *src,             # <<<<<<<<<<<<<<
  *                              __Pyx_memviewslice *tmpslice,
  *                              char order,
  */
 
@@ -28530,15 +28724,15 @@
   }
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
   return __pyx_r;
 }
 
-/* "View.MemoryView":1251
+/* "View.MemoryView":1253
  * 
  * @cname('__pyx_memoryview_err_extents')
  * cdef int _err_extents(int i, Py_ssize_t extent1,             # <<<<<<<<<<<<<<
  *                              Py_ssize_t extent2) except -1 with gil:
  *     raise ValueError("got differing extents in dimension %d (got %d and %d)" %
  */
 
@@ -28553,61 +28747,61 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("_err_extents", 0);
-  __Pyx_TraceCall("_err_extents", __pyx_f[2], 1251, 0, __PYX_ERR(2, 1251, __pyx_L1_error));
+  __Pyx_TraceCall("_err_extents", __pyx_f[2], 1253, 0, __PYX_ERR(2, 1253, __pyx_L1_error));
 
-  /* "View.MemoryView":1254
+  /* "View.MemoryView":1256
  *                              Py_ssize_t extent2) except -1 with gil:
  *     raise ValueError("got differing extents in dimension %d (got %d and %d)" %
  *                                                         (i, extent1, extent2))             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_err_dim')
  */
-  __Pyx_TraceLine(1254,0,__PYX_ERR(2, 1254, __pyx_L1_error))
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 1254, __pyx_L1_error)
+  __Pyx_TraceLine(1256,0,__PYX_ERR(2, 1256, __pyx_L1_error))
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 1256, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_extent1); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1254, __pyx_L1_error)
+  __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_extent1); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1256, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_extent2); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 1254, __pyx_L1_error)
+  __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_extent2); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 1256, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 1254, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 1256, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_t_3);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
   __pyx_t_3 = 0;
 
-  /* "View.MemoryView":1253
+  /* "View.MemoryView":1255
  * cdef int _err_extents(int i, Py_ssize_t extent1,
  *                              Py_ssize_t extent2) except -1 with gil:
  *     raise ValueError("got differing extents in dimension %d (got %d and %d)" %             # <<<<<<<<<<<<<<
  *                                                         (i, extent1, extent2))
  * 
  */
-  __Pyx_TraceLine(1253,0,__PYX_ERR(2, 1253, __pyx_L1_error))
-  __pyx_t_3 = __Pyx_PyString_Format(__pyx_kp_s_got_differing_extents_in_dimensi, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 1253, __pyx_L1_error)
+  __Pyx_TraceLine(1255,0,__PYX_ERR(2, 1255, __pyx_L1_error))
+  __pyx_t_3 = __Pyx_PyString_Format(__pyx_kp_s_got_differing_extents_in_dimensi, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 1255, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 1253, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 1255, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_Raise(__pyx_t_4, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __PYX_ERR(2, 1253, __pyx_L1_error)
+  __PYX_ERR(2, 1255, __pyx_L1_error)
 
-  /* "View.MemoryView":1251
+  /* "View.MemoryView":1253
  * 
  * @cname('__pyx_memoryview_err_extents')
  * cdef int _err_extents(int i, Py_ssize_t extent1,             # <<<<<<<<<<<<<<
  *                              Py_ssize_t extent2) except -1 with gil:
  *     raise ValueError("got differing extents in dimension %d (got %d and %d)" %
  */
 
@@ -28623,15 +28817,15 @@
   __Pyx_RefNannyFinishContext();
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   return __pyx_r;
 }
 
-/* "View.MemoryView":1257
+/* "View.MemoryView":1259
  * 
  * @cname('__pyx_memoryview_err_dim')
  * cdef int _err_dim(object error, char *msg, int dim) except -1 with gil:             # <<<<<<<<<<<<<<
  *     raise error(msg.decode('ascii') % dim)
  * 
  */
 
@@ -28646,30 +28840,30 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("_err_dim", 0);
-  __Pyx_TraceCall("_err_dim", __pyx_f[2], 1257, 0, __PYX_ERR(2, 1257, __pyx_L1_error));
+  __Pyx_TraceCall("_err_dim", __pyx_f[2], 1259, 0, __PYX_ERR(2, 1259, __pyx_L1_error));
   __Pyx_INCREF(__pyx_v_error);
 
-  /* "View.MemoryView":1258
+  /* "View.MemoryView":1260
  * @cname('__pyx_memoryview_err_dim')
  * cdef int _err_dim(object error, char *msg, int dim) except -1 with gil:
  *     raise error(msg.decode('ascii') % dim)             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_err')
  */
-  __Pyx_TraceLine(1258,0,__PYX_ERR(2, 1258, __pyx_L1_error))
-  __pyx_t_2 = __Pyx_decode_c_string(__pyx_v_msg, 0, strlen(__pyx_v_msg), NULL, NULL, PyUnicode_DecodeASCII); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1258, __pyx_L1_error)
+  __Pyx_TraceLine(1260,0,__PYX_ERR(2, 1260, __pyx_L1_error))
+  __pyx_t_2 = __Pyx_decode_c_string(__pyx_v_msg, 0, strlen(__pyx_v_msg), NULL, NULL, PyUnicode_DecodeASCII); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1260, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_dim); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 1258, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_dim); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 1260, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyUnicode_Format(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 1258, __pyx_L1_error)
+  __pyx_t_4 = PyUnicode_Format(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 1260, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_INCREF(__pyx_v_error);
   __pyx_t_3 = __pyx_v_error; __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
@@ -28679,22 +28873,22 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 1258, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 1260, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __PYX_ERR(2, 1258, __pyx_L1_error)
+  __PYX_ERR(2, 1260, __pyx_L1_error)
 
-  /* "View.MemoryView":1257
+  /* "View.MemoryView":1259
  * 
  * @cname('__pyx_memoryview_err_dim')
  * cdef int _err_dim(object error, char *msg, int dim) except -1 with gil:             # <<<<<<<<<<<<<<
  *     raise error(msg.decode('ascii') % dim)
  * 
  */
 
@@ -28711,15 +28905,15 @@
   __Pyx_RefNannyFinishContext();
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   return __pyx_r;
 }
 
-/* "View.MemoryView":1261
+/* "View.MemoryView":1263
  * 
  * @cname('__pyx_memoryview_err')
  * cdef int _err(object error, char *msg) except -1 with gil:             # <<<<<<<<<<<<<<
  *     if msg != NULL:
  *         raise error(msg.decode('ascii'))
  */
 
@@ -28735,37 +28929,37 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("_err", 0);
-  __Pyx_TraceCall("_err", __pyx_f[2], 1261, 0, __PYX_ERR(2, 1261, __pyx_L1_error));
+  __Pyx_TraceCall("_err", __pyx_f[2], 1263, 0, __PYX_ERR(2, 1263, __pyx_L1_error));
   __Pyx_INCREF(__pyx_v_error);
 
-  /* "View.MemoryView":1262
+  /* "View.MemoryView":1264
  * @cname('__pyx_memoryview_err')
  * cdef int _err(object error, char *msg) except -1 with gil:
  *     if msg != NULL:             # <<<<<<<<<<<<<<
  *         raise error(msg.decode('ascii'))
  *     else:
  */
-  __Pyx_TraceLine(1262,0,__PYX_ERR(2, 1262, __pyx_L1_error))
+  __Pyx_TraceLine(1264,0,__PYX_ERR(2, 1264, __pyx_L1_error))
   __pyx_t_1 = ((__pyx_v_msg != NULL) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "View.MemoryView":1263
+    /* "View.MemoryView":1265
  * cdef int _err(object error, char *msg) except -1 with gil:
  *     if msg != NULL:
  *         raise error(msg.decode('ascii'))             # <<<<<<<<<<<<<<
  *     else:
  *         raise error
  */
-    __Pyx_TraceLine(1263,0,__PYX_ERR(2, 1263, __pyx_L1_error))
-    __pyx_t_3 = __Pyx_decode_c_string(__pyx_v_msg, 0, strlen(__pyx_v_msg), NULL, NULL, PyUnicode_DecodeASCII); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 1263, __pyx_L1_error)
+    __Pyx_TraceLine(1265,0,__PYX_ERR(2, 1265, __pyx_L1_error))
+    __pyx_t_3 = __Pyx_decode_c_string(__pyx_v_msg, 0, strlen(__pyx_v_msg), NULL, NULL, PyUnicode_DecodeASCII); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 1265, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_v_error);
     __pyx_t_4 = __pyx_v_error; __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -28773,44 +28967,44 @@
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_3);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1263, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1265, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(2, 1263, __pyx_L1_error)
+    __PYX_ERR(2, 1265, __pyx_L1_error)
 
-    /* "View.MemoryView":1262
+    /* "View.MemoryView":1264
  * @cname('__pyx_memoryview_err')
  * cdef int _err(object error, char *msg) except -1 with gil:
  *     if msg != NULL:             # <<<<<<<<<<<<<<
  *         raise error(msg.decode('ascii'))
  *     else:
  */
   }
 
-  /* "View.MemoryView":1265
+  /* "View.MemoryView":1267
  *         raise error(msg.decode('ascii'))
  *     else:
  *         raise error             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_copy_contents')
  */
-  __Pyx_TraceLine(1265,0,__PYX_ERR(2, 1265, __pyx_L1_error))
+  __Pyx_TraceLine(1267,0,__PYX_ERR(2, 1267, __pyx_L1_error))
   /*else*/ {
     __Pyx_Raise(__pyx_v_error, 0, 0, 0);
-    __PYX_ERR(2, 1265, __pyx_L1_error)
+    __PYX_ERR(2, 1267, __pyx_L1_error)
   }
 
-  /* "View.MemoryView":1261
+  /* "View.MemoryView":1263
  * 
  * @cname('__pyx_memoryview_err')
  * cdef int _err(object error, char *msg) except -1 with gil:             # <<<<<<<<<<<<<<
  *     if msg != NULL:
  *         raise error(msg.decode('ascii'))
  */
 
@@ -28827,15 +29021,15 @@
   __Pyx_RefNannyFinishContext();
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   return __pyx_r;
 }
 
-/* "View.MemoryView":1268
+/* "View.MemoryView":1270
  * 
  * @cname('__pyx_memoryview_copy_contents')
  * cdef int memoryview_copy_contents(__Pyx_memviewslice src,             # <<<<<<<<<<<<<<
  *                                   __Pyx_memviewslice dst,
  *                                   int src_ndim, int dst_ndim,
  */
 
@@ -28857,584 +29051,584 @@
   int __pyx_t_5;
   int __pyx_t_6;
   void *__pyx_t_7;
   int __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_TraceCall("memoryview_copy_contents", __pyx_f[2], 1268, 1, __PYX_ERR(2, 1268, __pyx_L1_error));
+  __Pyx_TraceCall("memoryview_copy_contents", __pyx_f[2], 1270, 1, __PYX_ERR(2, 1270, __pyx_L1_error));
 
-  /* "View.MemoryView":1276
+  /* "View.MemoryView":1278
  *     Check for overlapping memory and verify the shapes.
  *     """
  *     cdef void *tmpdata = NULL             # <<<<<<<<<<<<<<
  *     cdef size_t itemsize = src.memview.view.itemsize
  *     cdef int i
  */
-  __Pyx_TraceLine(1276,1,__PYX_ERR(2, 1276, __pyx_L1_error))
+  __Pyx_TraceLine(1278,1,__PYX_ERR(2, 1278, __pyx_L1_error))
   __pyx_v_tmpdata = NULL;
 
-  /* "View.MemoryView":1277
+  /* "View.MemoryView":1279
  *     """
  *     cdef void *tmpdata = NULL
  *     cdef size_t itemsize = src.memview.view.itemsize             # <<<<<<<<<<<<<<
  *     cdef int i
  *     cdef char order = get_best_order(&src, src_ndim)
  */
-  __Pyx_TraceLine(1277,1,__PYX_ERR(2, 1277, __pyx_L1_error))
+  __Pyx_TraceLine(1279,1,__PYX_ERR(2, 1279, __pyx_L1_error))
   __pyx_t_1 = __pyx_v_src.memview->view.itemsize;
   __pyx_v_itemsize = __pyx_t_1;
 
-  /* "View.MemoryView":1279
+  /* "View.MemoryView":1281
  *     cdef size_t itemsize = src.memview.view.itemsize
  *     cdef int i
  *     cdef char order = get_best_order(&src, src_ndim)             # <<<<<<<<<<<<<<
  *     cdef bint broadcasting = False
  *     cdef bint direct_copy = False
  */
-  __Pyx_TraceLine(1279,1,__PYX_ERR(2, 1279, __pyx_L1_error))
+  __Pyx_TraceLine(1281,1,__PYX_ERR(2, 1281, __pyx_L1_error))
   __pyx_v_order = __pyx_get_best_slice_order((&__pyx_v_src), __pyx_v_src_ndim);
 
-  /* "View.MemoryView":1280
+  /* "View.MemoryView":1282
  *     cdef int i
  *     cdef char order = get_best_order(&src, src_ndim)
  *     cdef bint broadcasting = False             # <<<<<<<<<<<<<<
  *     cdef bint direct_copy = False
  *     cdef __Pyx_memviewslice tmp
  */
-  __Pyx_TraceLine(1280,1,__PYX_ERR(2, 1280, __pyx_L1_error))
+  __Pyx_TraceLine(1282,1,__PYX_ERR(2, 1282, __pyx_L1_error))
   __pyx_v_broadcasting = 0;
 
-  /* "View.MemoryView":1281
+  /* "View.MemoryView":1283
  *     cdef char order = get_best_order(&src, src_ndim)
  *     cdef bint broadcasting = False
  *     cdef bint direct_copy = False             # <<<<<<<<<<<<<<
  *     cdef __Pyx_memviewslice tmp
  * 
  */
-  __Pyx_TraceLine(1281,1,__PYX_ERR(2, 1281, __pyx_L1_error))
+  __Pyx_TraceLine(1283,1,__PYX_ERR(2, 1283, __pyx_L1_error))
   __pyx_v_direct_copy = 0;
 
-  /* "View.MemoryView":1284
+  /* "View.MemoryView":1286
  *     cdef __Pyx_memviewslice tmp
  * 
  *     if src_ndim < dst_ndim:             # <<<<<<<<<<<<<<
  *         broadcast_leading(&src, src_ndim, dst_ndim)
  *     elif dst_ndim < src_ndim:
  */
-  __Pyx_TraceLine(1284,1,__PYX_ERR(2, 1284, __pyx_L1_error))
+  __Pyx_TraceLine(1286,1,__PYX_ERR(2, 1286, __pyx_L1_error))
   __pyx_t_2 = ((__pyx_v_src_ndim < __pyx_v_dst_ndim) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1285
+    /* "View.MemoryView":1287
  * 
  *     if src_ndim < dst_ndim:
  *         broadcast_leading(&src, src_ndim, dst_ndim)             # <<<<<<<<<<<<<<
  *     elif dst_ndim < src_ndim:
  *         broadcast_leading(&dst, dst_ndim, src_ndim)
  */
-    __Pyx_TraceLine(1285,1,__PYX_ERR(2, 1285, __pyx_L1_error))
+    __Pyx_TraceLine(1287,1,__PYX_ERR(2, 1287, __pyx_L1_error))
     __pyx_memoryview_broadcast_leading((&__pyx_v_src), __pyx_v_src_ndim, __pyx_v_dst_ndim);
 
-    /* "View.MemoryView":1284
+    /* "View.MemoryView":1286
  *     cdef __Pyx_memviewslice tmp
  * 
  *     if src_ndim < dst_ndim:             # <<<<<<<<<<<<<<
  *         broadcast_leading(&src, src_ndim, dst_ndim)
  *     elif dst_ndim < src_ndim:
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":1286
+  /* "View.MemoryView":1288
  *     if src_ndim < dst_ndim:
  *         broadcast_leading(&src, src_ndim, dst_ndim)
  *     elif dst_ndim < src_ndim:             # <<<<<<<<<<<<<<
  *         broadcast_leading(&dst, dst_ndim, src_ndim)
  * 
  */
-  __Pyx_TraceLine(1286,1,__PYX_ERR(2, 1286, __pyx_L1_error))
+  __Pyx_TraceLine(1288,1,__PYX_ERR(2, 1288, __pyx_L1_error))
   __pyx_t_2 = ((__pyx_v_dst_ndim < __pyx_v_src_ndim) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1287
+    /* "View.MemoryView":1289
  *         broadcast_leading(&src, src_ndim, dst_ndim)
  *     elif dst_ndim < src_ndim:
  *         broadcast_leading(&dst, dst_ndim, src_ndim)             # <<<<<<<<<<<<<<
  * 
  *     cdef int ndim = max(src_ndim, dst_ndim)
  */
-    __Pyx_TraceLine(1287,1,__PYX_ERR(2, 1287, __pyx_L1_error))
+    __Pyx_TraceLine(1289,1,__PYX_ERR(2, 1289, __pyx_L1_error))
     __pyx_memoryview_broadcast_leading((&__pyx_v_dst), __pyx_v_dst_ndim, __pyx_v_src_ndim);
 
-    /* "View.MemoryView":1286
+    /* "View.MemoryView":1288
  *     if src_ndim < dst_ndim:
  *         broadcast_leading(&src, src_ndim, dst_ndim)
  *     elif dst_ndim < src_ndim:             # <<<<<<<<<<<<<<
  *         broadcast_leading(&dst, dst_ndim, src_ndim)
  * 
  */
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":1289
+  /* "View.MemoryView":1291
  *         broadcast_leading(&dst, dst_ndim, src_ndim)
  * 
  *     cdef int ndim = max(src_ndim, dst_ndim)             # <<<<<<<<<<<<<<
  * 
  *     for i in range(ndim):
  */
-  __Pyx_TraceLine(1289,1,__PYX_ERR(2, 1289, __pyx_L1_error))
+  __Pyx_TraceLine(1291,1,__PYX_ERR(2, 1291, __pyx_L1_error))
   __pyx_t_3 = __pyx_v_dst_ndim;
   __pyx_t_4 = __pyx_v_src_ndim;
   if (((__pyx_t_3 > __pyx_t_4) != 0)) {
     __pyx_t_5 = __pyx_t_3;
   } else {
     __pyx_t_5 = __pyx_t_4;
   }
   __pyx_v_ndim = __pyx_t_5;
 
-  /* "View.MemoryView":1291
+  /* "View.MemoryView":1293
  *     cdef int ndim = max(src_ndim, dst_ndim)
  * 
  *     for i in range(ndim):             # <<<<<<<<<<<<<<
  *         if src.shape[i] != dst.shape[i]:
  *             if src.shape[i] == 1:
  */
-  __Pyx_TraceLine(1291,1,__PYX_ERR(2, 1291, __pyx_L1_error))
+  __Pyx_TraceLine(1293,1,__PYX_ERR(2, 1293, __pyx_L1_error))
   __pyx_t_5 = __pyx_v_ndim;
   __pyx_t_3 = __pyx_t_5;
   for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
     __pyx_v_i = __pyx_t_4;
 
-    /* "View.MemoryView":1292
+    /* "View.MemoryView":1294
  * 
  *     for i in range(ndim):
  *         if src.shape[i] != dst.shape[i]:             # <<<<<<<<<<<<<<
  *             if src.shape[i] == 1:
  *                 broadcasting = True
  */
-    __Pyx_TraceLine(1292,1,__PYX_ERR(2, 1292, __pyx_L1_error))
+    __Pyx_TraceLine(1294,1,__PYX_ERR(2, 1294, __pyx_L1_error))
     __pyx_t_2 = (((__pyx_v_src.shape[__pyx_v_i]) != (__pyx_v_dst.shape[__pyx_v_i])) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1293
+      /* "View.MemoryView":1295
  *     for i in range(ndim):
  *         if src.shape[i] != dst.shape[i]:
  *             if src.shape[i] == 1:             # <<<<<<<<<<<<<<
  *                 broadcasting = True
  *                 src.strides[i] = 0
  */
-      __Pyx_TraceLine(1293,1,__PYX_ERR(2, 1293, __pyx_L1_error))
+      __Pyx_TraceLine(1295,1,__PYX_ERR(2, 1295, __pyx_L1_error))
       __pyx_t_2 = (((__pyx_v_src.shape[__pyx_v_i]) == 1) != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":1294
+        /* "View.MemoryView":1296
  *         if src.shape[i] != dst.shape[i]:
  *             if src.shape[i] == 1:
  *                 broadcasting = True             # <<<<<<<<<<<<<<
  *                 src.strides[i] = 0
  *             else:
  */
-        __Pyx_TraceLine(1294,1,__PYX_ERR(2, 1294, __pyx_L1_error))
+        __Pyx_TraceLine(1296,1,__PYX_ERR(2, 1296, __pyx_L1_error))
         __pyx_v_broadcasting = 1;
 
-        /* "View.MemoryView":1295
+        /* "View.MemoryView":1297
  *             if src.shape[i] == 1:
  *                 broadcasting = True
  *                 src.strides[i] = 0             # <<<<<<<<<<<<<<
  *             else:
  *                 _err_extents(i, dst.shape[i], src.shape[i])
  */
-        __Pyx_TraceLine(1295,1,__PYX_ERR(2, 1295, __pyx_L1_error))
+        __Pyx_TraceLine(1297,1,__PYX_ERR(2, 1297, __pyx_L1_error))
         (__pyx_v_src.strides[__pyx_v_i]) = 0;
 
-        /* "View.MemoryView":1293
+        /* "View.MemoryView":1295
  *     for i in range(ndim):
  *         if src.shape[i] != dst.shape[i]:
  *             if src.shape[i] == 1:             # <<<<<<<<<<<<<<
  *                 broadcasting = True
  *                 src.strides[i] = 0
  */
         goto __pyx_L7;
       }
 
-      /* "View.MemoryView":1297
+      /* "View.MemoryView":1299
  *                 src.strides[i] = 0
  *             else:
  *                 _err_extents(i, dst.shape[i], src.shape[i])             # <<<<<<<<<<<<<<
  * 
  *         if src.suboffsets[i] >= 0:
  */
-      __Pyx_TraceLine(1297,1,__PYX_ERR(2, 1297, __pyx_L1_error))
+      __Pyx_TraceLine(1299,1,__PYX_ERR(2, 1299, __pyx_L1_error))
       /*else*/ {
-        __pyx_t_6 = __pyx_memoryview_err_extents(__pyx_v_i, (__pyx_v_dst.shape[__pyx_v_i]), (__pyx_v_src.shape[__pyx_v_i])); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(2, 1297, __pyx_L1_error)
+        __pyx_t_6 = __pyx_memoryview_err_extents(__pyx_v_i, (__pyx_v_dst.shape[__pyx_v_i]), (__pyx_v_src.shape[__pyx_v_i])); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(2, 1299, __pyx_L1_error)
       }
       __pyx_L7:;
 
-      /* "View.MemoryView":1292
+      /* "View.MemoryView":1294
  * 
  *     for i in range(ndim):
  *         if src.shape[i] != dst.shape[i]:             # <<<<<<<<<<<<<<
  *             if src.shape[i] == 1:
  *                 broadcasting = True
  */
     }
 
-    /* "View.MemoryView":1299
+    /* "View.MemoryView":1301
  *                 _err_extents(i, dst.shape[i], src.shape[i])
  * 
  *         if src.suboffsets[i] >= 0:             # <<<<<<<<<<<<<<
  *             _err_dim(ValueError, "Dimension %d is not direct", i)
  * 
  */
-    __Pyx_TraceLine(1299,1,__PYX_ERR(2, 1299, __pyx_L1_error))
+    __Pyx_TraceLine(1301,1,__PYX_ERR(2, 1301, __pyx_L1_error))
     __pyx_t_2 = (((__pyx_v_src.suboffsets[__pyx_v_i]) >= 0) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1300
+      /* "View.MemoryView":1302
  * 
  *         if src.suboffsets[i] >= 0:
  *             _err_dim(ValueError, "Dimension %d is not direct", i)             # <<<<<<<<<<<<<<
  * 
  *     if slices_overlap(&src, &dst, ndim, itemsize):
  */
-      __Pyx_TraceLine(1300,1,__PYX_ERR(2, 1300, __pyx_L1_error))
-      __pyx_t_6 = __pyx_memoryview_err_dim(__pyx_builtin_ValueError, ((char *)"Dimension %d is not direct"), __pyx_v_i); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(2, 1300, __pyx_L1_error)
+      __Pyx_TraceLine(1302,1,__PYX_ERR(2, 1302, __pyx_L1_error))
+      __pyx_t_6 = __pyx_memoryview_err_dim(__pyx_builtin_ValueError, ((char *)"Dimension %d is not direct"), __pyx_v_i); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(2, 1302, __pyx_L1_error)
 
-      /* "View.MemoryView":1299
+      /* "View.MemoryView":1301
  *                 _err_extents(i, dst.shape[i], src.shape[i])
  * 
  *         if src.suboffsets[i] >= 0:             # <<<<<<<<<<<<<<
  *             _err_dim(ValueError, "Dimension %d is not direct", i)
  * 
  */
     }
   }
 
-  /* "View.MemoryView":1302
+  /* "View.MemoryView":1304
  *             _err_dim(ValueError, "Dimension %d is not direct", i)
  * 
  *     if slices_overlap(&src, &dst, ndim, itemsize):             # <<<<<<<<<<<<<<
  * 
  *         if not slice_is_contig(src, order, ndim):
  */
-  __Pyx_TraceLine(1302,1,__PYX_ERR(2, 1302, __pyx_L1_error))
+  __Pyx_TraceLine(1304,1,__PYX_ERR(2, 1304, __pyx_L1_error))
   __pyx_t_2 = (__pyx_slices_overlap((&__pyx_v_src), (&__pyx_v_dst), __pyx_v_ndim, __pyx_v_itemsize) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1304
+    /* "View.MemoryView":1306
  *     if slices_overlap(&src, &dst, ndim, itemsize):
  * 
  *         if not slice_is_contig(src, order, ndim):             # <<<<<<<<<<<<<<
  *             order = get_best_order(&dst, ndim)
  * 
  */
-    __Pyx_TraceLine(1304,1,__PYX_ERR(2, 1304, __pyx_L1_error))
+    __Pyx_TraceLine(1306,1,__PYX_ERR(2, 1306, __pyx_L1_error))
     __pyx_t_2 = ((!(__pyx_memviewslice_is_contig(__pyx_v_src, __pyx_v_order, __pyx_v_ndim) != 0)) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1305
+      /* "View.MemoryView":1307
  * 
  *         if not slice_is_contig(src, order, ndim):
  *             order = get_best_order(&dst, ndim)             # <<<<<<<<<<<<<<
  * 
  *         tmpdata = copy_data_to_temp(&src, &tmp, order, ndim)
  */
-      __Pyx_TraceLine(1305,1,__PYX_ERR(2, 1305, __pyx_L1_error))
+      __Pyx_TraceLine(1307,1,__PYX_ERR(2, 1307, __pyx_L1_error))
       __pyx_v_order = __pyx_get_best_slice_order((&__pyx_v_dst), __pyx_v_ndim);
 
-      /* "View.MemoryView":1304
+      /* "View.MemoryView":1306
  *     if slices_overlap(&src, &dst, ndim, itemsize):
  * 
  *         if not slice_is_contig(src, order, ndim):             # <<<<<<<<<<<<<<
  *             order = get_best_order(&dst, ndim)
  * 
  */
     }
 
-    /* "View.MemoryView":1307
+    /* "View.MemoryView":1309
  *             order = get_best_order(&dst, ndim)
  * 
  *         tmpdata = copy_data_to_temp(&src, &tmp, order, ndim)             # <<<<<<<<<<<<<<
  *         src = tmp
  * 
  */
-    __Pyx_TraceLine(1307,1,__PYX_ERR(2, 1307, __pyx_L1_error))
-    __pyx_t_7 = __pyx_memoryview_copy_data_to_temp((&__pyx_v_src), (&__pyx_v_tmp), __pyx_v_order, __pyx_v_ndim); if (unlikely(__pyx_t_7 == ((void *)NULL))) __PYX_ERR(2, 1307, __pyx_L1_error)
+    __Pyx_TraceLine(1309,1,__PYX_ERR(2, 1309, __pyx_L1_error))
+    __pyx_t_7 = __pyx_memoryview_copy_data_to_temp((&__pyx_v_src), (&__pyx_v_tmp), __pyx_v_order, __pyx_v_ndim); if (unlikely(__pyx_t_7 == ((void *)NULL))) __PYX_ERR(2, 1309, __pyx_L1_error)
     __pyx_v_tmpdata = __pyx_t_7;
 
-    /* "View.MemoryView":1308
+    /* "View.MemoryView":1310
  * 
  *         tmpdata = copy_data_to_temp(&src, &tmp, order, ndim)
  *         src = tmp             # <<<<<<<<<<<<<<
  * 
  *     if not broadcasting:
  */
-    __Pyx_TraceLine(1308,1,__PYX_ERR(2, 1308, __pyx_L1_error))
+    __Pyx_TraceLine(1310,1,__PYX_ERR(2, 1310, __pyx_L1_error))
     __pyx_v_src = __pyx_v_tmp;
 
-    /* "View.MemoryView":1302
+    /* "View.MemoryView":1304
  *             _err_dim(ValueError, "Dimension %d is not direct", i)
  * 
  *     if slices_overlap(&src, &dst, ndim, itemsize):             # <<<<<<<<<<<<<<
  * 
  *         if not slice_is_contig(src, order, ndim):
  */
   }
 
-  /* "View.MemoryView":1310
+  /* "View.MemoryView":1312
  *         src = tmp
  * 
  *     if not broadcasting:             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_TraceLine(1310,1,__PYX_ERR(2, 1310, __pyx_L1_error))
+  __Pyx_TraceLine(1312,1,__PYX_ERR(2, 1312, __pyx_L1_error))
   __pyx_t_2 = ((!(__pyx_v_broadcasting != 0)) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1313
+    /* "View.MemoryView":1315
  * 
  * 
  *         if slice_is_contig(src, 'C', ndim):             # <<<<<<<<<<<<<<
  *             direct_copy = slice_is_contig(dst, 'C', ndim)
  *         elif slice_is_contig(src, 'F', ndim):
  */
-    __Pyx_TraceLine(1313,1,__PYX_ERR(2, 1313, __pyx_L1_error))
+    __Pyx_TraceLine(1315,1,__PYX_ERR(2, 1315, __pyx_L1_error))
     __pyx_t_2 = (__pyx_memviewslice_is_contig(__pyx_v_src, 'C', __pyx_v_ndim) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1314
+      /* "View.MemoryView":1316
  * 
  *         if slice_is_contig(src, 'C', ndim):
  *             direct_copy = slice_is_contig(dst, 'C', ndim)             # <<<<<<<<<<<<<<
  *         elif slice_is_contig(src, 'F', ndim):
  *             direct_copy = slice_is_contig(dst, 'F', ndim)
  */
-      __Pyx_TraceLine(1314,1,__PYX_ERR(2, 1314, __pyx_L1_error))
+      __Pyx_TraceLine(1316,1,__PYX_ERR(2, 1316, __pyx_L1_error))
       __pyx_v_direct_copy = __pyx_memviewslice_is_contig(__pyx_v_dst, 'C', __pyx_v_ndim);
 
-      /* "View.MemoryView":1313
+      /* "View.MemoryView":1315
  * 
  * 
  *         if slice_is_contig(src, 'C', ndim):             # <<<<<<<<<<<<<<
  *             direct_copy = slice_is_contig(dst, 'C', ndim)
  *         elif slice_is_contig(src, 'F', ndim):
  */
       goto __pyx_L12;
     }
 
-    /* "View.MemoryView":1315
+    /* "View.MemoryView":1317
  *         if slice_is_contig(src, 'C', ndim):
  *             direct_copy = slice_is_contig(dst, 'C', ndim)
  *         elif slice_is_contig(src, 'F', ndim):             # <<<<<<<<<<<<<<
  *             direct_copy = slice_is_contig(dst, 'F', ndim)
  * 
  */
-    __Pyx_TraceLine(1315,1,__PYX_ERR(2, 1315, __pyx_L1_error))
+    __Pyx_TraceLine(1317,1,__PYX_ERR(2, 1317, __pyx_L1_error))
     __pyx_t_2 = (__pyx_memviewslice_is_contig(__pyx_v_src, 'F', __pyx_v_ndim) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1316
+      /* "View.MemoryView":1318
  *             direct_copy = slice_is_contig(dst, 'C', ndim)
  *         elif slice_is_contig(src, 'F', ndim):
  *             direct_copy = slice_is_contig(dst, 'F', ndim)             # <<<<<<<<<<<<<<
  * 
  *         if direct_copy:
  */
-      __Pyx_TraceLine(1316,1,__PYX_ERR(2, 1316, __pyx_L1_error))
+      __Pyx_TraceLine(1318,1,__PYX_ERR(2, 1318, __pyx_L1_error))
       __pyx_v_direct_copy = __pyx_memviewslice_is_contig(__pyx_v_dst, 'F', __pyx_v_ndim);
 
-      /* "View.MemoryView":1315
+      /* "View.MemoryView":1317
  *         if slice_is_contig(src, 'C', ndim):
  *             direct_copy = slice_is_contig(dst, 'C', ndim)
  *         elif slice_is_contig(src, 'F', ndim):             # <<<<<<<<<<<<<<
  *             direct_copy = slice_is_contig(dst, 'F', ndim)
  * 
  */
     }
     __pyx_L12:;
 
-    /* "View.MemoryView":1318
+    /* "View.MemoryView":1320
  *             direct_copy = slice_is_contig(dst, 'F', ndim)
  * 
  *         if direct_copy:             # <<<<<<<<<<<<<<
  * 
  *             refcount_copying(&dst, dtype_is_object, ndim, False)
  */
-    __Pyx_TraceLine(1318,1,__PYX_ERR(2, 1318, __pyx_L1_error))
+    __Pyx_TraceLine(1320,1,__PYX_ERR(2, 1320, __pyx_L1_error))
     __pyx_t_2 = (__pyx_v_direct_copy != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1320
+      /* "View.MemoryView":1322
  *         if direct_copy:
  * 
  *             refcount_copying(&dst, dtype_is_object, ndim, False)             # <<<<<<<<<<<<<<
  *             memcpy(dst.data, src.data, slice_get_size(&src, ndim))
  *             refcount_copying(&dst, dtype_is_object, ndim, True)
  */
-      __Pyx_TraceLine(1320,1,__PYX_ERR(2, 1320, __pyx_L1_error))
+      __Pyx_TraceLine(1322,1,__PYX_ERR(2, 1322, __pyx_L1_error))
       __pyx_memoryview_refcount_copying((&__pyx_v_dst), __pyx_v_dtype_is_object, __pyx_v_ndim, 0);
 
-      /* "View.MemoryView":1321
+      /* "View.MemoryView":1323
  * 
  *             refcount_copying(&dst, dtype_is_object, ndim, False)
  *             memcpy(dst.data, src.data, slice_get_size(&src, ndim))             # <<<<<<<<<<<<<<
  *             refcount_copying(&dst, dtype_is_object, ndim, True)
  *             free(tmpdata)
  */
-      __Pyx_TraceLine(1321,1,__PYX_ERR(2, 1321, __pyx_L1_error))
+      __Pyx_TraceLine(1323,1,__PYX_ERR(2, 1323, __pyx_L1_error))
       (void)(memcpy(__pyx_v_dst.data, __pyx_v_src.data, __pyx_memoryview_slice_get_size((&__pyx_v_src), __pyx_v_ndim)));
 
-      /* "View.MemoryView":1322
+      /* "View.MemoryView":1324
  *             refcount_copying(&dst, dtype_is_object, ndim, False)
  *             memcpy(dst.data, src.data, slice_get_size(&src, ndim))
  *             refcount_copying(&dst, dtype_is_object, ndim, True)             # <<<<<<<<<<<<<<
  *             free(tmpdata)
  *             return 0
  */
-      __Pyx_TraceLine(1322,1,__PYX_ERR(2, 1322, __pyx_L1_error))
+      __Pyx_TraceLine(1324,1,__PYX_ERR(2, 1324, __pyx_L1_error))
       __pyx_memoryview_refcount_copying((&__pyx_v_dst), __pyx_v_dtype_is_object, __pyx_v_ndim, 1);
 
-      /* "View.MemoryView":1323
+      /* "View.MemoryView":1325
  *             memcpy(dst.data, src.data, slice_get_size(&src, ndim))
  *             refcount_copying(&dst, dtype_is_object, ndim, True)
  *             free(tmpdata)             # <<<<<<<<<<<<<<
  *             return 0
  * 
  */
-      __Pyx_TraceLine(1323,1,__PYX_ERR(2, 1323, __pyx_L1_error))
+      __Pyx_TraceLine(1325,1,__PYX_ERR(2, 1325, __pyx_L1_error))
       free(__pyx_v_tmpdata);
 
-      /* "View.MemoryView":1324
+      /* "View.MemoryView":1326
  *             refcount_copying(&dst, dtype_is_object, ndim, True)
  *             free(tmpdata)
  *             return 0             # <<<<<<<<<<<<<<
  * 
  *     if order == 'F' == get_best_order(&dst, ndim):
  */
-      __Pyx_TraceLine(1324,1,__PYX_ERR(2, 1324, __pyx_L1_error))
+      __Pyx_TraceLine(1326,1,__PYX_ERR(2, 1326, __pyx_L1_error))
       __pyx_r = 0;
       goto __pyx_L0;
 
-      /* "View.MemoryView":1318
+      /* "View.MemoryView":1320
  *             direct_copy = slice_is_contig(dst, 'F', ndim)
  * 
  *         if direct_copy:             # <<<<<<<<<<<<<<
  * 
  *             refcount_copying(&dst, dtype_is_object, ndim, False)
  */
     }
 
-    /* "View.MemoryView":1310
+    /* "View.MemoryView":1312
  *         src = tmp
  * 
  *     if not broadcasting:             # <<<<<<<<<<<<<<
  * 
  * 
  */
   }
 
-  /* "View.MemoryView":1326
+  /* "View.MemoryView":1328
  *             return 0
  * 
  *     if order == 'F' == get_best_order(&dst, ndim):             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_TraceLine(1326,1,__PYX_ERR(2, 1326, __pyx_L1_error))
+  __Pyx_TraceLine(1328,1,__PYX_ERR(2, 1328, __pyx_L1_error))
   __pyx_t_2 = (__pyx_v_order == 'F');
   if (__pyx_t_2) {
     __pyx_t_2 = ('F' == __pyx_get_best_slice_order((&__pyx_v_dst), __pyx_v_ndim));
   }
   __pyx_t_8 = (__pyx_t_2 != 0);
   if (__pyx_t_8) {
 
-    /* "View.MemoryView":1329
+    /* "View.MemoryView":1331
  * 
  * 
  *         transpose_memslice(&src)             # <<<<<<<<<<<<<<
  *         transpose_memslice(&dst)
  * 
  */
-    __Pyx_TraceLine(1329,1,__PYX_ERR(2, 1329, __pyx_L1_error))
-    __pyx_t_5 = __pyx_memslice_transpose((&__pyx_v_src)); if (unlikely(__pyx_t_5 == ((int)0))) __PYX_ERR(2, 1329, __pyx_L1_error)
+    __Pyx_TraceLine(1331,1,__PYX_ERR(2, 1331, __pyx_L1_error))
+    __pyx_t_5 = __pyx_memslice_transpose((&__pyx_v_src)); if (unlikely(__pyx_t_5 == ((int)0))) __PYX_ERR(2, 1331, __pyx_L1_error)
 
-    /* "View.MemoryView":1330
+    /* "View.MemoryView":1332
  * 
  *         transpose_memslice(&src)
  *         transpose_memslice(&dst)             # <<<<<<<<<<<<<<
  * 
  *     refcount_copying(&dst, dtype_is_object, ndim, False)
  */
-    __Pyx_TraceLine(1330,1,__PYX_ERR(2, 1330, __pyx_L1_error))
-    __pyx_t_5 = __pyx_memslice_transpose((&__pyx_v_dst)); if (unlikely(__pyx_t_5 == ((int)0))) __PYX_ERR(2, 1330, __pyx_L1_error)
+    __Pyx_TraceLine(1332,1,__PYX_ERR(2, 1332, __pyx_L1_error))
+    __pyx_t_5 = __pyx_memslice_transpose((&__pyx_v_dst)); if (unlikely(__pyx_t_5 == ((int)0))) __PYX_ERR(2, 1332, __pyx_L1_error)
 
-    /* "View.MemoryView":1326
+    /* "View.MemoryView":1328
  *             return 0
  * 
  *     if order == 'F' == get_best_order(&dst, ndim):             # <<<<<<<<<<<<<<
  * 
  * 
  */
   }
 
-  /* "View.MemoryView":1332
+  /* "View.MemoryView":1334
  *         transpose_memslice(&dst)
  * 
  *     refcount_copying(&dst, dtype_is_object, ndim, False)             # <<<<<<<<<<<<<<
  *     copy_strided_to_strided(&src, &dst, ndim, itemsize)
  *     refcount_copying(&dst, dtype_is_object, ndim, True)
  */
-  __Pyx_TraceLine(1332,1,__PYX_ERR(2, 1332, __pyx_L1_error))
+  __Pyx_TraceLine(1334,1,__PYX_ERR(2, 1334, __pyx_L1_error))
   __pyx_memoryview_refcount_copying((&__pyx_v_dst), __pyx_v_dtype_is_object, __pyx_v_ndim, 0);
 
-  /* "View.MemoryView":1333
+  /* "View.MemoryView":1335
  * 
  *     refcount_copying(&dst, dtype_is_object, ndim, False)
  *     copy_strided_to_strided(&src, &dst, ndim, itemsize)             # <<<<<<<<<<<<<<
  *     refcount_copying(&dst, dtype_is_object, ndim, True)
  * 
  */
-  __Pyx_TraceLine(1333,1,__PYX_ERR(2, 1333, __pyx_L1_error))
+  __Pyx_TraceLine(1335,1,__PYX_ERR(2, 1335, __pyx_L1_error))
   copy_strided_to_strided((&__pyx_v_src), (&__pyx_v_dst), __pyx_v_ndim, __pyx_v_itemsize);
 
-  /* "View.MemoryView":1334
+  /* "View.MemoryView":1336
  *     refcount_copying(&dst, dtype_is_object, ndim, False)
  *     copy_strided_to_strided(&src, &dst, ndim, itemsize)
  *     refcount_copying(&dst, dtype_is_object, ndim, True)             # <<<<<<<<<<<<<<
  * 
  *     free(tmpdata)
  */
-  __Pyx_TraceLine(1334,1,__PYX_ERR(2, 1334, __pyx_L1_error))
+  __Pyx_TraceLine(1336,1,__PYX_ERR(2, 1336, __pyx_L1_error))
   __pyx_memoryview_refcount_copying((&__pyx_v_dst), __pyx_v_dtype_is_object, __pyx_v_ndim, 1);
 
-  /* "View.MemoryView":1336
+  /* "View.MemoryView":1338
  *     refcount_copying(&dst, dtype_is_object, ndim, True)
  * 
  *     free(tmpdata)             # <<<<<<<<<<<<<<
  *     return 0
  * 
  */
-  __Pyx_TraceLine(1336,1,__PYX_ERR(2, 1336, __pyx_L1_error))
+  __Pyx_TraceLine(1338,1,__PYX_ERR(2, 1338, __pyx_L1_error))
   free(__pyx_v_tmpdata);
 
-  /* "View.MemoryView":1337
+  /* "View.MemoryView":1339
  * 
  *     free(tmpdata)
  *     return 0             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_broadcast_leading')
  */
-  __Pyx_TraceLine(1337,1,__PYX_ERR(2, 1337, __pyx_L1_error))
+  __Pyx_TraceLine(1339,1,__PYX_ERR(2, 1339, __pyx_L1_error))
   __pyx_r = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":1268
+  /* "View.MemoryView":1270
  * 
  * @cname('__pyx_memoryview_copy_contents')
  * cdef int memoryview_copy_contents(__Pyx_memviewslice src,             # <<<<<<<<<<<<<<
  *                                   __Pyx_memviewslice dst,
  *                                   int src_ndim, int dst_ndim,
  */
 
@@ -29451,15 +29645,15 @@
   }
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
   return __pyx_r;
 }
 
-/* "View.MemoryView":1340
+/* "View.MemoryView":1342
  * 
  * @cname('__pyx_memoryview_broadcast_leading')
  * cdef void broadcast_leading(__Pyx_memviewslice *mslice,             # <<<<<<<<<<<<<<
  *                             int ndim,
  *                             int ndim_other) nogil:
  */
 
@@ -29469,113 +29663,113 @@
   __Pyx_TraceDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_TraceCall("broadcast_leading", __pyx_f[2], 1340, 1, __PYX_ERR(2, 1340, __pyx_L1_error));
+  __Pyx_TraceCall("broadcast_leading", __pyx_f[2], 1342, 1, __PYX_ERR(2, 1342, __pyx_L1_error));
 
-  /* "View.MemoryView":1344
+  /* "View.MemoryView":1346
  *                             int ndim_other) nogil:
  *     cdef int i
  *     cdef int offset = ndim_other - ndim             # <<<<<<<<<<<<<<
  * 
  *     for i in range(ndim - 1, -1, -1):
  */
-  __Pyx_TraceLine(1344,1,__PYX_ERR(2, 1344, __pyx_L1_error))
+  __Pyx_TraceLine(1346,1,__PYX_ERR(2, 1346, __pyx_L1_error))
   __pyx_v_offset = (__pyx_v_ndim_other - __pyx_v_ndim);
 
-  /* "View.MemoryView":1346
+  /* "View.MemoryView":1348
  *     cdef int offset = ndim_other - ndim
  * 
  *     for i in range(ndim - 1, -1, -1):             # <<<<<<<<<<<<<<
  *         mslice.shape[i + offset] = mslice.shape[i]
  *         mslice.strides[i + offset] = mslice.strides[i]
  */
-  __Pyx_TraceLine(1346,1,__PYX_ERR(2, 1346, __pyx_L1_error))
+  __Pyx_TraceLine(1348,1,__PYX_ERR(2, 1348, __pyx_L1_error))
   for (__pyx_t_1 = (__pyx_v_ndim - 1); __pyx_t_1 > -1; __pyx_t_1-=1) {
     __pyx_v_i = __pyx_t_1;
 
-    /* "View.MemoryView":1347
+    /* "View.MemoryView":1349
  * 
  *     for i in range(ndim - 1, -1, -1):
  *         mslice.shape[i + offset] = mslice.shape[i]             # <<<<<<<<<<<<<<
  *         mslice.strides[i + offset] = mslice.strides[i]
  *         mslice.suboffsets[i + offset] = mslice.suboffsets[i]
  */
-    __Pyx_TraceLine(1347,1,__PYX_ERR(2, 1347, __pyx_L1_error))
+    __Pyx_TraceLine(1349,1,__PYX_ERR(2, 1349, __pyx_L1_error))
     (__pyx_v_mslice->shape[(__pyx_v_i + __pyx_v_offset)]) = (__pyx_v_mslice->shape[__pyx_v_i]);
 
-    /* "View.MemoryView":1348
+    /* "View.MemoryView":1350
  *     for i in range(ndim - 1, -1, -1):
  *         mslice.shape[i + offset] = mslice.shape[i]
  *         mslice.strides[i + offset] = mslice.strides[i]             # <<<<<<<<<<<<<<
  *         mslice.suboffsets[i + offset] = mslice.suboffsets[i]
  * 
  */
-    __Pyx_TraceLine(1348,1,__PYX_ERR(2, 1348, __pyx_L1_error))
+    __Pyx_TraceLine(1350,1,__PYX_ERR(2, 1350, __pyx_L1_error))
     (__pyx_v_mslice->strides[(__pyx_v_i + __pyx_v_offset)]) = (__pyx_v_mslice->strides[__pyx_v_i]);
 
-    /* "View.MemoryView":1349
+    /* "View.MemoryView":1351
  *         mslice.shape[i + offset] = mslice.shape[i]
  *         mslice.strides[i + offset] = mslice.strides[i]
  *         mslice.suboffsets[i + offset] = mslice.suboffsets[i]             # <<<<<<<<<<<<<<
  * 
  *     for i in range(offset):
  */
-    __Pyx_TraceLine(1349,1,__PYX_ERR(2, 1349, __pyx_L1_error))
+    __Pyx_TraceLine(1351,1,__PYX_ERR(2, 1351, __pyx_L1_error))
     (__pyx_v_mslice->suboffsets[(__pyx_v_i + __pyx_v_offset)]) = (__pyx_v_mslice->suboffsets[__pyx_v_i]);
   }
 
-  /* "View.MemoryView":1351
+  /* "View.MemoryView":1353
  *         mslice.suboffsets[i + offset] = mslice.suboffsets[i]
  * 
  *     for i in range(offset):             # <<<<<<<<<<<<<<
  *         mslice.shape[i] = 1
  *         mslice.strides[i] = mslice.strides[0]
  */
-  __Pyx_TraceLine(1351,1,__PYX_ERR(2, 1351, __pyx_L1_error))
+  __Pyx_TraceLine(1353,1,__PYX_ERR(2, 1353, __pyx_L1_error))
   __pyx_t_1 = __pyx_v_offset;
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     __pyx_v_i = __pyx_t_3;
 
-    /* "View.MemoryView":1352
+    /* "View.MemoryView":1354
  * 
  *     for i in range(offset):
  *         mslice.shape[i] = 1             # <<<<<<<<<<<<<<
  *         mslice.strides[i] = mslice.strides[0]
  *         mslice.suboffsets[i] = -1
  */
-    __Pyx_TraceLine(1352,1,__PYX_ERR(2, 1352, __pyx_L1_error))
+    __Pyx_TraceLine(1354,1,__PYX_ERR(2, 1354, __pyx_L1_error))
     (__pyx_v_mslice->shape[__pyx_v_i]) = 1;
 
-    /* "View.MemoryView":1353
+    /* "View.MemoryView":1355
  *     for i in range(offset):
  *         mslice.shape[i] = 1
  *         mslice.strides[i] = mslice.strides[0]             # <<<<<<<<<<<<<<
  *         mslice.suboffsets[i] = -1
  * 
  */
-    __Pyx_TraceLine(1353,1,__PYX_ERR(2, 1353, __pyx_L1_error))
+    __Pyx_TraceLine(1355,1,__PYX_ERR(2, 1355, __pyx_L1_error))
     (__pyx_v_mslice->strides[__pyx_v_i]) = (__pyx_v_mslice->strides[0]);
 
-    /* "View.MemoryView":1354
+    /* "View.MemoryView":1356
  *         mslice.shape[i] = 1
  *         mslice.strides[i] = mslice.strides[0]
  *         mslice.suboffsets[i] = -1             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __Pyx_TraceLine(1354,1,__PYX_ERR(2, 1354, __pyx_L1_error))
+    __Pyx_TraceLine(1356,1,__PYX_ERR(2, 1356, __pyx_L1_error))
     (__pyx_v_mslice->suboffsets[__pyx_v_i]) = -1L;
   }
 
-  /* "View.MemoryView":1340
+  /* "View.MemoryView":1342
  * 
  * @cname('__pyx_memoryview_broadcast_leading')
  * cdef void broadcast_leading(__Pyx_memviewslice *mslice,             # <<<<<<<<<<<<<<
  *                             int ndim,
  *                             int ndim_other) nogil:
  */
 
@@ -29583,61 +29777,61 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("View.MemoryView.broadcast_leading", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 1);
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
 }
 
-/* "View.MemoryView":1362
+/* "View.MemoryView":1364
  * 
  * @cname('__pyx_memoryview_refcount_copying')
  * cdef void refcount_copying(__Pyx_memviewslice *dst, bint dtype_is_object,             # <<<<<<<<<<<<<<
  *                            int ndim, bint inc) nogil:
  * 
  */
 
 static void __pyx_memoryview_refcount_copying(__Pyx_memviewslice *__pyx_v_dst, int __pyx_v_dtype_is_object, int __pyx_v_ndim, int __pyx_v_inc) {
   __Pyx_TraceDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_TraceCall("refcount_copying", __pyx_f[2], 1362, 1, __PYX_ERR(2, 1362, __pyx_L1_error));
+  __Pyx_TraceCall("refcount_copying", __pyx_f[2], 1364, 1, __PYX_ERR(2, 1364, __pyx_L1_error));
 
-  /* "View.MemoryView":1366
+  /* "View.MemoryView":1368
  * 
  * 
  *     if dtype_is_object:             # <<<<<<<<<<<<<<
  *         refcount_objects_in_slice_with_gil(dst.data, dst.shape,
  *                                            dst.strides, ndim, inc)
  */
-  __Pyx_TraceLine(1366,1,__PYX_ERR(2, 1366, __pyx_L1_error))
+  __Pyx_TraceLine(1368,1,__PYX_ERR(2, 1368, __pyx_L1_error))
   __pyx_t_1 = (__pyx_v_dtype_is_object != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":1367
+    /* "View.MemoryView":1369
  * 
  *     if dtype_is_object:
  *         refcount_objects_in_slice_with_gil(dst.data, dst.shape,             # <<<<<<<<<<<<<<
  *                                            dst.strides, ndim, inc)
  * 
  */
-    __Pyx_TraceLine(1367,1,__PYX_ERR(2, 1367, __pyx_L1_error))
+    __Pyx_TraceLine(1369,1,__PYX_ERR(2, 1369, __pyx_L1_error))
     __pyx_memoryview_refcount_objects_in_slice_with_gil(__pyx_v_dst->data, __pyx_v_dst->shape, __pyx_v_dst->strides, __pyx_v_ndim, __pyx_v_inc);
 
-    /* "View.MemoryView":1366
+    /* "View.MemoryView":1368
  * 
  * 
  *     if dtype_is_object:             # <<<<<<<<<<<<<<
  *         refcount_objects_in_slice_with_gil(dst.data, dst.shape,
  *                                            dst.strides, ndim, inc)
  */
   }
 
-  /* "View.MemoryView":1362
+  /* "View.MemoryView":1364
  * 
  * @cname('__pyx_memoryview_refcount_copying')
  * cdef void refcount_copying(__Pyx_memviewslice *dst, bint dtype_is_object,             # <<<<<<<<<<<<<<
  *                            int ndim, bint inc) nogil:
  * 
  */
 
@@ -29645,15 +29839,15 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("View.MemoryView.refcount_copying", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 1);
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
 }
 
-/* "View.MemoryView":1371
+/* "View.MemoryView":1373
  * 
  * @cname('__pyx_memoryview_refcount_objects_in_slice_with_gil')
  * cdef void refcount_objects_in_slice_with_gil(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                                              Py_ssize_t *strides, int ndim,
  *                                              bint inc) with gil:
  */
 
@@ -29663,27 +29857,27 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("refcount_objects_in_slice_with_gil", 0);
-  __Pyx_TraceCall("refcount_objects_in_slice_with_gil", __pyx_f[2], 1371, 0, __PYX_ERR(2, 1371, __pyx_L1_error));
+  __Pyx_TraceCall("refcount_objects_in_slice_with_gil", __pyx_f[2], 1373, 0, __PYX_ERR(2, 1373, __pyx_L1_error));
 
-  /* "View.MemoryView":1374
+  /* "View.MemoryView":1376
  *                                              Py_ssize_t *strides, int ndim,
  *                                              bint inc) with gil:
  *     refcount_objects_in_slice(data, shape, strides, ndim, inc)             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_refcount_objects_in_slice')
  */
-  __Pyx_TraceLine(1374,0,__PYX_ERR(2, 1374, __pyx_L1_error))
+  __Pyx_TraceLine(1376,0,__PYX_ERR(2, 1376, __pyx_L1_error))
   __pyx_memoryview_refcount_objects_in_slice(__pyx_v_data, __pyx_v_shape, __pyx_v_strides, __pyx_v_ndim, __pyx_v_inc);
 
-  /* "View.MemoryView":1371
+  /* "View.MemoryView":1373
  * 
  * @cname('__pyx_memoryview_refcount_objects_in_slice_with_gil')
  * cdef void refcount_objects_in_slice_with_gil(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                                              Py_ssize_t *strides, int ndim,
  *                                              bint inc) with gil:
  */
 
@@ -29695,15 +29889,15 @@
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
 }
 
-/* "View.MemoryView":1377
+/* "View.MemoryView":1379
  * 
  * @cname('__pyx_memoryview_refcount_objects_in_slice')
  * cdef void refcount_objects_in_slice(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                                     Py_ssize_t *strides, int ndim, bint inc):
  *     cdef Py_ssize_t i
  */
 
@@ -29715,128 +29909,128 @@
   Py_ssize_t __pyx_t_2;
   Py_ssize_t __pyx_t_3;
   int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("refcount_objects_in_slice", 0);
-  __Pyx_TraceCall("refcount_objects_in_slice", __pyx_f[2], 1377, 0, __PYX_ERR(2, 1377, __pyx_L1_error));
+  __Pyx_TraceCall("refcount_objects_in_slice", __pyx_f[2], 1379, 0, __PYX_ERR(2, 1379, __pyx_L1_error));
 
-  /* "View.MemoryView":1381
+  /* "View.MemoryView":1383
  *     cdef Py_ssize_t i
  * 
  *     for i in range(shape[0]):             # <<<<<<<<<<<<<<
  *         if ndim == 1:
  *             if inc:
  */
-  __Pyx_TraceLine(1381,0,__PYX_ERR(2, 1381, __pyx_L1_error))
+  __Pyx_TraceLine(1383,0,__PYX_ERR(2, 1383, __pyx_L1_error))
   __pyx_t_1 = (__pyx_v_shape[0]);
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     __pyx_v_i = __pyx_t_3;
 
-    /* "View.MemoryView":1382
+    /* "View.MemoryView":1384
  * 
  *     for i in range(shape[0]):
  *         if ndim == 1:             # <<<<<<<<<<<<<<
  *             if inc:
  *                 Py_INCREF((<PyObject **> data)[0])
  */
-    __Pyx_TraceLine(1382,0,__PYX_ERR(2, 1382, __pyx_L1_error))
+    __Pyx_TraceLine(1384,0,__PYX_ERR(2, 1384, __pyx_L1_error))
     __pyx_t_4 = ((__pyx_v_ndim == 1) != 0);
     if (__pyx_t_4) {
 
-      /* "View.MemoryView":1383
+      /* "View.MemoryView":1385
  *     for i in range(shape[0]):
  *         if ndim == 1:
  *             if inc:             # <<<<<<<<<<<<<<
  *                 Py_INCREF((<PyObject **> data)[0])
  *             else:
  */
-      __Pyx_TraceLine(1383,0,__PYX_ERR(2, 1383, __pyx_L1_error))
+      __Pyx_TraceLine(1385,0,__PYX_ERR(2, 1385, __pyx_L1_error))
       __pyx_t_4 = (__pyx_v_inc != 0);
       if (__pyx_t_4) {
 
-        /* "View.MemoryView":1384
+        /* "View.MemoryView":1386
  *         if ndim == 1:
  *             if inc:
  *                 Py_INCREF((<PyObject **> data)[0])             # <<<<<<<<<<<<<<
  *             else:
  *                 Py_DECREF((<PyObject **> data)[0])
  */
-        __Pyx_TraceLine(1384,0,__PYX_ERR(2, 1384, __pyx_L1_error))
+        __Pyx_TraceLine(1386,0,__PYX_ERR(2, 1386, __pyx_L1_error))
         Py_INCREF((((PyObject **)__pyx_v_data)[0]));
 
-        /* "View.MemoryView":1383
+        /* "View.MemoryView":1385
  *     for i in range(shape[0]):
  *         if ndim == 1:
  *             if inc:             # <<<<<<<<<<<<<<
  *                 Py_INCREF((<PyObject **> data)[0])
  *             else:
  */
         goto __pyx_L6;
       }
 
-      /* "View.MemoryView":1386
+      /* "View.MemoryView":1388
  *                 Py_INCREF((<PyObject **> data)[0])
  *             else:
  *                 Py_DECREF((<PyObject **> data)[0])             # <<<<<<<<<<<<<<
  *         else:
  *             refcount_objects_in_slice(data, shape + 1, strides + 1,
  */
-      __Pyx_TraceLine(1386,0,__PYX_ERR(2, 1386, __pyx_L1_error))
+      __Pyx_TraceLine(1388,0,__PYX_ERR(2, 1388, __pyx_L1_error))
       /*else*/ {
         Py_DECREF((((PyObject **)__pyx_v_data)[0]));
       }
       __pyx_L6:;
 
-      /* "View.MemoryView":1382
+      /* "View.MemoryView":1384
  * 
  *     for i in range(shape[0]):
  *         if ndim == 1:             # <<<<<<<<<<<<<<
  *             if inc:
  *                 Py_INCREF((<PyObject **> data)[0])
  */
       goto __pyx_L5;
     }
 
-    /* "View.MemoryView":1388
+    /* "View.MemoryView":1390
  *                 Py_DECREF((<PyObject **> data)[0])
  *         else:
  *             refcount_objects_in_slice(data, shape + 1, strides + 1,             # <<<<<<<<<<<<<<
  *                                       ndim - 1, inc)
  * 
  */
-    __Pyx_TraceLine(1388,0,__PYX_ERR(2, 1388, __pyx_L1_error))
+    __Pyx_TraceLine(1390,0,__PYX_ERR(2, 1390, __pyx_L1_error))
     /*else*/ {
 
-      /* "View.MemoryView":1389
+      /* "View.MemoryView":1391
  *         else:
  *             refcount_objects_in_slice(data, shape + 1, strides + 1,
  *                                       ndim - 1, inc)             # <<<<<<<<<<<<<<
  * 
  *         data += strides[0]
  */
-      __Pyx_TraceLine(1389,0,__PYX_ERR(2, 1389, __pyx_L1_error))
+      __Pyx_TraceLine(1391,0,__PYX_ERR(2, 1391, __pyx_L1_error))
       __pyx_memoryview_refcount_objects_in_slice(__pyx_v_data, (__pyx_v_shape + 1), (__pyx_v_strides + 1), (__pyx_v_ndim - 1), __pyx_v_inc);
     }
     __pyx_L5:;
 
-    /* "View.MemoryView":1391
+    /* "View.MemoryView":1393
  *                                       ndim - 1, inc)
  * 
  *         data += strides[0]             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __Pyx_TraceLine(1391,0,__PYX_ERR(2, 1391, __pyx_L1_error))
+    __Pyx_TraceLine(1393,0,__PYX_ERR(2, 1393, __pyx_L1_error))
     __pyx_v_data = (__pyx_v_data + (__pyx_v_strides[0]));
   }
 
-  /* "View.MemoryView":1377
+  /* "View.MemoryView":1379
  * 
  * @cname('__pyx_memoryview_refcount_objects_in_slice')
  * cdef void refcount_objects_in_slice(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                                     Py_ssize_t *strides, int ndim, bint inc):
  *     cdef Py_ssize_t i
  */
 
@@ -29845,60 +30039,60 @@
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("View.MemoryView.refcount_objects_in_slice", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
 }
 
-/* "View.MemoryView":1397
+/* "View.MemoryView":1399
  * 
  * @cname('__pyx_memoryview_slice_assign_scalar')
  * cdef void slice_assign_scalar(__Pyx_memviewslice *dst, int ndim,             # <<<<<<<<<<<<<<
  *                               size_t itemsize, void *item,
  *                               bint dtype_is_object) nogil:
  */
 
 static void __pyx_memoryview_slice_assign_scalar(__Pyx_memviewslice *__pyx_v_dst, int __pyx_v_ndim, size_t __pyx_v_itemsize, void *__pyx_v_item, int __pyx_v_dtype_is_object) {
   __Pyx_TraceDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_TraceCall("slice_assign_scalar", __pyx_f[2], 1397, 1, __PYX_ERR(2, 1397, __pyx_L1_error));
+  __Pyx_TraceCall("slice_assign_scalar", __pyx_f[2], 1399, 1, __PYX_ERR(2, 1399, __pyx_L1_error));
 
-  /* "View.MemoryView":1400
+  /* "View.MemoryView":1402
  *                               size_t itemsize, void *item,
  *                               bint dtype_is_object) nogil:
  *     refcount_copying(dst, dtype_is_object, ndim, False)             # <<<<<<<<<<<<<<
  *     _slice_assign_scalar(dst.data, dst.shape, dst.strides, ndim,
  *                          itemsize, item)
  */
-  __Pyx_TraceLine(1400,1,__PYX_ERR(2, 1400, __pyx_L1_error))
+  __Pyx_TraceLine(1402,1,__PYX_ERR(2, 1402, __pyx_L1_error))
   __pyx_memoryview_refcount_copying(__pyx_v_dst, __pyx_v_dtype_is_object, __pyx_v_ndim, 0);
 
-  /* "View.MemoryView":1401
+  /* "View.MemoryView":1403
  *                               bint dtype_is_object) nogil:
  *     refcount_copying(dst, dtype_is_object, ndim, False)
  *     _slice_assign_scalar(dst.data, dst.shape, dst.strides, ndim,             # <<<<<<<<<<<<<<
  *                          itemsize, item)
  *     refcount_copying(dst, dtype_is_object, ndim, True)
  */
-  __Pyx_TraceLine(1401,1,__PYX_ERR(2, 1401, __pyx_L1_error))
+  __Pyx_TraceLine(1403,1,__PYX_ERR(2, 1403, __pyx_L1_error))
   __pyx_memoryview__slice_assign_scalar(__pyx_v_dst->data, __pyx_v_dst->shape, __pyx_v_dst->strides, __pyx_v_ndim, __pyx_v_itemsize, __pyx_v_item);
 
-  /* "View.MemoryView":1403
+  /* "View.MemoryView":1405
  *     _slice_assign_scalar(dst.data, dst.shape, dst.strides, ndim,
  *                          itemsize, item)
  *     refcount_copying(dst, dtype_is_object, ndim, True)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_TraceLine(1403,1,__PYX_ERR(2, 1403, __pyx_L1_error))
+  __Pyx_TraceLine(1405,1,__PYX_ERR(2, 1405, __pyx_L1_error))
   __pyx_memoryview_refcount_copying(__pyx_v_dst, __pyx_v_dtype_is_object, __pyx_v_ndim, 1);
 
-  /* "View.MemoryView":1397
+  /* "View.MemoryView":1399
  * 
  * @cname('__pyx_memoryview_slice_assign_scalar')
  * cdef void slice_assign_scalar(__Pyx_memviewslice *dst, int ndim,             # <<<<<<<<<<<<<<
  *                               size_t itemsize, void *item,
  *                               bint dtype_is_object) nogil:
  */
 
@@ -29906,15 +30100,15 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("View.MemoryView.slice_assign_scalar", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 1);
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
 }
 
-/* "View.MemoryView":1407
+/* "View.MemoryView":1409
  * 
  * @cname('__pyx_memoryview__slice_assign_scalar')
  * cdef void _slice_assign_scalar(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                               Py_ssize_t *strides, int ndim,
  *                               size_t itemsize, void *item) nogil:
  */
 
@@ -29926,129 +30120,129 @@
   int __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   Py_ssize_t __pyx_t_3;
   Py_ssize_t __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_TraceCall("_slice_assign_scalar", __pyx_f[2], 1407, 1, __PYX_ERR(2, 1407, __pyx_L1_error));
+  __Pyx_TraceCall("_slice_assign_scalar", __pyx_f[2], 1409, 1, __PYX_ERR(2, 1409, __pyx_L1_error));
 
-  /* "View.MemoryView":1411
+  /* "View.MemoryView":1413
  *                               size_t itemsize, void *item) nogil:
  *     cdef Py_ssize_t i
  *     cdef Py_ssize_t stride = strides[0]             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t extent = shape[0]
  * 
  */
-  __Pyx_TraceLine(1411,1,__PYX_ERR(2, 1411, __pyx_L1_error))
+  __Pyx_TraceLine(1413,1,__PYX_ERR(2, 1413, __pyx_L1_error))
   __pyx_v_stride = (__pyx_v_strides[0]);
 
-  /* "View.MemoryView":1412
+  /* "View.MemoryView":1414
  *     cdef Py_ssize_t i
  *     cdef Py_ssize_t stride = strides[0]
  *     cdef Py_ssize_t extent = shape[0]             # <<<<<<<<<<<<<<
  * 
  *     if ndim == 1:
  */
-  __Pyx_TraceLine(1412,1,__PYX_ERR(2, 1412, __pyx_L1_error))
+  __Pyx_TraceLine(1414,1,__PYX_ERR(2, 1414, __pyx_L1_error))
   __pyx_v_extent = (__pyx_v_shape[0]);
 
-  /* "View.MemoryView":1414
+  /* "View.MemoryView":1416
  *     cdef Py_ssize_t extent = shape[0]
  * 
  *     if ndim == 1:             # <<<<<<<<<<<<<<
  *         for i in range(extent):
  *             memcpy(data, item, itemsize)
  */
-  __Pyx_TraceLine(1414,1,__PYX_ERR(2, 1414, __pyx_L1_error))
+  __Pyx_TraceLine(1416,1,__PYX_ERR(2, 1416, __pyx_L1_error))
   __pyx_t_1 = ((__pyx_v_ndim == 1) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":1415
+    /* "View.MemoryView":1417
  * 
  *     if ndim == 1:
  *         for i in range(extent):             # <<<<<<<<<<<<<<
  *             memcpy(data, item, itemsize)
  *             data += stride
  */
-    __Pyx_TraceLine(1415,1,__PYX_ERR(2, 1415, __pyx_L1_error))
+    __Pyx_TraceLine(1417,1,__PYX_ERR(2, 1417, __pyx_L1_error))
     __pyx_t_2 = __pyx_v_extent;
     __pyx_t_3 = __pyx_t_2;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_v_i = __pyx_t_4;
 
-      /* "View.MemoryView":1416
+      /* "View.MemoryView":1418
  *     if ndim == 1:
  *         for i in range(extent):
  *             memcpy(data, item, itemsize)             # <<<<<<<<<<<<<<
  *             data += stride
  *     else:
  */
-      __Pyx_TraceLine(1416,1,__PYX_ERR(2, 1416, __pyx_L1_error))
+      __Pyx_TraceLine(1418,1,__PYX_ERR(2, 1418, __pyx_L1_error))
       (void)(memcpy(__pyx_v_data, __pyx_v_item, __pyx_v_itemsize));
 
-      /* "View.MemoryView":1417
+      /* "View.MemoryView":1419
  *         for i in range(extent):
  *             memcpy(data, item, itemsize)
  *             data += stride             # <<<<<<<<<<<<<<
  *     else:
  *         for i in range(extent):
  */
-      __Pyx_TraceLine(1417,1,__PYX_ERR(2, 1417, __pyx_L1_error))
+      __Pyx_TraceLine(1419,1,__PYX_ERR(2, 1419, __pyx_L1_error))
       __pyx_v_data = (__pyx_v_data + __pyx_v_stride);
     }
 
-    /* "View.MemoryView":1414
+    /* "View.MemoryView":1416
  *     cdef Py_ssize_t extent = shape[0]
  * 
  *     if ndim == 1:             # <<<<<<<<<<<<<<
  *         for i in range(extent):
  *             memcpy(data, item, itemsize)
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":1419
+  /* "View.MemoryView":1421
  *             data += stride
  *     else:
  *         for i in range(extent):             # <<<<<<<<<<<<<<
  *             _slice_assign_scalar(data, shape + 1, strides + 1,
  *                                 ndim - 1, itemsize, item)
  */
-  __Pyx_TraceLine(1419,1,__PYX_ERR(2, 1419, __pyx_L1_error))
+  __Pyx_TraceLine(1421,1,__PYX_ERR(2, 1421, __pyx_L1_error))
   /*else*/ {
     __pyx_t_2 = __pyx_v_extent;
     __pyx_t_3 = __pyx_t_2;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_v_i = __pyx_t_4;
 
-      /* "View.MemoryView":1420
+      /* "View.MemoryView":1422
  *     else:
  *         for i in range(extent):
  *             _slice_assign_scalar(data, shape + 1, strides + 1,             # <<<<<<<<<<<<<<
  *                                 ndim - 1, itemsize, item)
  *             data += stride
  */
-      __Pyx_TraceLine(1420,1,__PYX_ERR(2, 1420, __pyx_L1_error))
+      __Pyx_TraceLine(1422,1,__PYX_ERR(2, 1422, __pyx_L1_error))
       __pyx_memoryview__slice_assign_scalar(__pyx_v_data, (__pyx_v_shape + 1), (__pyx_v_strides + 1), (__pyx_v_ndim - 1), __pyx_v_itemsize, __pyx_v_item);
 
-      /* "View.MemoryView":1422
+      /* "View.MemoryView":1424
  *             _slice_assign_scalar(data, shape + 1, strides + 1,
  *                                 ndim - 1, itemsize, item)
  *             data += stride             # <<<<<<<<<<<<<<
  * 
  * 
  */
-      __Pyx_TraceLine(1422,1,__PYX_ERR(2, 1422, __pyx_L1_error))
+      __Pyx_TraceLine(1424,1,__PYX_ERR(2, 1424, __pyx_L1_error))
       __pyx_v_data = (__pyx_v_data + __pyx_v_stride);
     }
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":1407
+  /* "View.MemoryView":1409
  * 
  * @cname('__pyx_memoryview__slice_assign_scalar')
  * cdef void _slice_assign_scalar(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                               Py_ssize_t *strides, int ndim,
  *                               size_t itemsize, void *item) nogil:
  */
 
@@ -30144,159 +30338,163 @@
 
 static PyObject *__pyx_pf_15View_dot_MemoryView___pyx_unpickle_Enum(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_TraceFrameInit(__pyx_codeobj__28)
+  __Pyx_TraceFrameInit(__pyx_codeobj__29)
   __Pyx_RefNannySetupContext("__pyx_unpickle_Enum", 0);
   __Pyx_TraceCall("__pyx_unpickle_Enum", __pyx_f[2], 1, 0, __PYX_ERR(2, 1, __pyx_L1_error));
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xb068931:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xb068931, 0x82a3537, 0x6ae9995):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb068931 = (name))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))" % __pyx_checksum)
  */
   __Pyx_TraceLine(4,0,__PYX_ERR(2, 4, __pyx_L1_error))
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0xb068931) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__30, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xb068931:
+ *     if __pyx_checksum not in (0xb068931, 0x82a3537, 0x6ae9995):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb068931 = (name))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))" % __pyx_checksum)
  *     __pyx_result = Enum.__new__(__pyx_type)
  */
     __Pyx_TraceLine(5,0,__PYX_ERR(2, 5, __pyx_L1_error))
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0xb068931:
+ *     if __pyx_checksum not in (0xb068931, 0x82a3537, 0x6ae9995):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb068931 = (name))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = Enum.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
     __Pyx_TraceLine(6,0,__PYX_ERR(2, 6, __pyx_L1_error))
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0xb0, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_2, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(2, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xb068931:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xb068931, 0x82a3537, 0x6ae9995):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb068931 = (name))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb068931 = (name))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))" % __pyx_checksum)
  *     __pyx_result = Enum.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_Enum__set_state(<Enum> __pyx_result, __pyx_state)
  */
   __Pyx_TraceLine(7,0,__PYX_ERR(2, 7, __pyx_L1_error))
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_MemviewEnum_type), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_MemviewEnum_type), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb068931 = (name))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))" % __pyx_checksum)
  *     __pyx_result = Enum.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_Enum__set_state(<Enum> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   __Pyx_TraceLine(8,0,__PYX_ERR(2, 8, __pyx_L1_error))
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = Enum.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_Enum__set_state(<Enum> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_Enum__set_state(Enum __pyx_result, tuple __pyx_state):
  */
     __Pyx_TraceLine(9,0,__PYX_ERR(2, 9, __pyx_L1_error))
-    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(2, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_unpickle_Enum__set_state(((struct __pyx_MemviewEnum_obj *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(2, 9, __pyx_L1_error)
+    __pyx_t_4 = __pyx_unpickle_Enum__set_state(((struct __pyx_MemviewEnum_obj *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb068931 = (name))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))" % __pyx_checksum)
  *     __pyx_result = Enum.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_Enum__set_state(<Enum> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -30317,18 +30515,18 @@
  * def __pyx_unpickle_Enum(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("View.MemoryView.__pyx_unpickle_Enum", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
@@ -31192,20 +31390,23 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  0, /*tp_pypy_flags*/
+  #endif
 };
 static struct __pyx_vtabstruct_array __pyx_vtable_array;
 
 static PyObject *__pyx_tp_new_array(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_array_obj *p;
   PyObject *o;
   if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
@@ -31381,20 +31582,23 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  0, /*tp_pypy_flags*/
+  #endif
 };
 
 static PyObject *__pyx_tp_new_Enum(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_MemviewEnum_obj *p;
   PyObject *o;
   if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
     o = (*t->tp_alloc)(t, 0);
@@ -31500,20 +31704,23 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  0, /*tp_pypy_flags*/
+  #endif
 };
 static struct __pyx_vtabstruct_memoryview __pyx_vtable_memoryview;
 
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryview_obj *p;
   PyObject *o;
   if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
@@ -31761,20 +31968,23 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  0, /*tp_pypy_flags*/
+  #endif
 };
 static struct __pyx_vtabstruct__memoryviewslice __pyx_vtable__memoryviewslice;
 
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryviewslice_obj *p;
   PyObject *o = __pyx_tp_new_memoryview(t, a, k);
   if (unlikely(!o)) return 0;
@@ -31907,20 +32117,23 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  0, /*tp_pypy_flags*/
+  #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
 
 #if PY_MAJOR_VERSION >= 3
@@ -31978,16 +32191,16 @@
   {&__pyx_kp_s_Data_is_not_consistent_and_coul, __pyx_k_Data_is_not_consistent_and_coul, sizeof(__pyx_k_Data_is_not_consistent_and_coul), 0, 0, 1, 0},
   {&__pyx_n_s_DestinationChoiceError, __pyx_k_DestinationChoiceError, sizeof(__pyx_k_DestinationChoiceError), 0, 0, 1, 1},
   {&__pyx_n_s_Ellipsis, __pyx_k_Ellipsis, sizeof(__pyx_k_Ellipsis), 0, 0, 1, 1},
   {&__pyx_kp_s_Empty_shape_tuple_for_cython_arr, __pyx_k_Empty_shape_tuple_for_cython_arr, sizeof(__pyx_k_Empty_shape_tuple_for_cython_arr), 0, 0, 1, 0},
   {&__pyx_kp_s_Error_in_destination_choice_mod, __pyx_k_Error_in_destination_choice_mod, sizeof(__pyx_k_Error_in_destination_choice_mod), 0, 0, 1, 0},
   {&__pyx_kp_u_Group, __pyx_k_Group, sizeof(__pyx_k_Group), 0, 1, 0, 0},
   {&__pyx_n_s_ImportError, __pyx_k_ImportError, sizeof(__pyx_k_ImportError), 0, 0, 1, 1},
-  {&__pyx_kp_s_Incompatible_checksums_s_vs_0xb0, __pyx_k_Incompatible_checksums_s_vs_0xb0, sizeof(__pyx_k_Incompatible_checksums_s_vs_0xb0), 0, 0, 1, 0},
-  {&__pyx_kp_s_Incompatible_checksums_s_vs_0xb9, __pyx_k_Incompatible_checksums_s_vs_0xb9, sizeof(__pyx_k_Incompatible_checksums_s_vs_0xb9), 0, 0, 1, 0},
+  {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_k_Incompatible_checksums_0x_x_vs_0, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0), 0, 0, 1, 0},
+  {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_2, __pyx_k_Incompatible_checksums_0x_x_vs_0_2, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0_2), 0, 0, 1, 0},
   {&__pyx_n_s_IndexError, __pyx_k_IndexError, sizeof(__pyx_k_IndexError), 0, 0, 1, 1},
   {&__pyx_kp_s_Indirect_dimensions_not_supporte, __pyx_k_Indirect_dimensions_not_supporte, sizeof(__pyx_k_Indirect_dimensions_not_supporte), 0, 0, 1, 0},
   {&__pyx_kp_s_Invalid_mode_expected_c_or_fortr, __pyx_k_Invalid_mode_expected_c_or_fortr, sizeof(__pyx_k_Invalid_mode_expected_c_or_fortr), 0, 0, 1, 0},
   {&__pyx_kp_s_Invalid_shape_in_axis_d_d, __pyx_k_Invalid_shape_in_axis_d_d, sizeof(__pyx_k_Invalid_shape_in_axis_d_d), 0, 0, 1, 0},
   {&__pyx_n_s_MemoryError, __pyx_k_MemoryError, sizeof(__pyx_k_MemoryError), 0, 0, 1, 1},
   {&__pyx_kp_s_MemoryView_of_r_at_0x_x, __pyx_k_MemoryView_of_r_at_0x_x, sizeof(__pyx_k_MemoryView_of_r_at_0x_x), 0, 0, 1, 0},
   {&__pyx_kp_s_MemoryView_of_r_object, __pyx_k_MemoryView_of_r_object, sizeof(__pyx_k_MemoryView_of_r_object), 0, 0, 1, 0},
@@ -32146,20 +32359,20 @@
   {&__pyx_n_s_wiver_wiver_cython, __pyx_k_wiver_wiver_cython, sizeof(__pyx_k_wiver_wiver_cython), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 21, __pyx_L1_error)
   __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(0, 27, __pyx_L1_error)
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 123, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(3, 945, __pyx_L1_error)
-  __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(2, 148, __pyx_L1_error)
-  __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(2, 151, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(3, 944, __pyx_L1_error)
+  __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(2, 149, __pyx_L1_error)
+  __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(2, 152, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(2, 2, __pyx_L1_error)
-  __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(2, 404, __pyx_L1_error)
-  __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(2, 613, __pyx_L1_error)
+  __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(2, 406, __pyx_L1_error)
+  __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(2, 615, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
@@ -32194,313 +32407,327 @@
  * 
  *     def assert_data_consistency_of_array(self, str attrname, str dim):
  */
   __pyx_tuple__7 = PyTuple_Pack(2, __pyx_n_u_sector_g, __pyx_n_u_n_sectors); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 488, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
 
-  /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":945
+  /* "(tree fragment)":4
+ *     cdef object __pyx_PickleError
+ *     cdef object __pyx_result
+ *     if __pyx_checksum not in (0xb9d7a6d, 0x31b4ce0, 0xa09edd1):             # <<<<<<<<<<<<<<
+ *         from pickle import PickleError as __pyx_PickleError
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb9d7a6d, 0x31b4ce0, 0xa09edd1) = (INF_d, INF_f, NAN_d, NAN_f, NINF_d, NINF_f, _active_g, _balancing_factor_gj, _converged_g, _home_based_trips_gij, _km_ij, _linking_trips_gij, _mean_distance_g, _mean_distance_m, _mode_g, _p_destination_tj, _p_links_tij, _param_dist_g, _return_trips_gij, _savings_param_g, _sector_g, _sink_potential_gj, _source_potential_gh, _stops_per_tour_g, _time_series_ending_trips_gs, _time_series_linking_trips_gs, _time_series_starting_trips_gs, _tour_rates_g, _travel_time_mij, _trips_gij, _trips_gsij, _trips_mij, _trips_msij, _trips_to_destination_gj, _zone_no, n_groups, n_modes, n_sectors, n_threads, n_time_slices, n_zones))" % __pyx_checksum)
+ */
+  __pyx_tuple__9 = PyTuple_Pack(3, __pyx_int_194869869, __pyx_int_52120800, __pyx_int_168422865); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__9);
+  __Pyx_GIVEREF(__pyx_tuple__9);
+
+  /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(3, 945, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__9);
-  __Pyx_GIVEREF(__pyx_tuple__9);
+  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(3, 944, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__10);
+  __Pyx_GIVEREF(__pyx_tuple__10);
 
-  /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":951
+  /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(3, 951, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__10);
-  __Pyx_GIVEREF(__pyx_tuple__10);
+  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(3, 950, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__11);
+  __Pyx_GIVEREF(__pyx_tuple__11);
 
-  /* "View.MemoryView":133
+  /* "View.MemoryView":134
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if itemsize <= 0:
  */
-  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_s_Empty_shape_tuple_for_cython_arr); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(2, 133, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__11);
-  __Pyx_GIVEREF(__pyx_tuple__11);
+  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_s_Empty_shape_tuple_for_cython_arr); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(2, 134, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__12);
+  __Pyx_GIVEREF(__pyx_tuple__12);
 
-  /* "View.MemoryView":136
+  /* "View.MemoryView":137
  * 
  *         if itemsize <= 0:
  *             raise ValueError("itemsize <= 0 for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if not isinstance(format, bytes):
  */
-  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_s_itemsize_0_for_cython_array); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(2, 136, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__12);
-  __Pyx_GIVEREF(__pyx_tuple__12);
+  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_s_itemsize_0_for_cython_array); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(2, 137, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__13);
+  __Pyx_GIVEREF(__pyx_tuple__13);
 
-  /* "View.MemoryView":148
+  /* "View.MemoryView":149
  * 
  *         if not self._shape:
  *             raise MemoryError("unable to allocate shape and strides.")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_shape_and_str); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(2, 148, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__13);
-  __Pyx_GIVEREF(__pyx_tuple__13);
+  __pyx_tuple__14 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_shape_and_str); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(2, 149, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__14);
+  __Pyx_GIVEREF(__pyx_tuple__14);
 
-  /* "View.MemoryView":176
+  /* "View.MemoryView":177
  *             self.data = <char *>malloc(self.len)
  *             if not self.data:
  *                 raise MemoryError("unable to allocate array data.")             # <<<<<<<<<<<<<<
  * 
  *             if self.dtype_is_object:
  */
-  __pyx_tuple__14 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_array_data); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(2, 176, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__14);
-  __Pyx_GIVEREF(__pyx_tuple__14);
+  __pyx_tuple__15 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_array_data); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(2, 177, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__15);
+  __Pyx_GIVEREF(__pyx_tuple__15);
 
-  /* "View.MemoryView":192
+  /* "View.MemoryView":193
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         if not (flags & bufmode):
  *             raise ValueError("Can only create a buffer that is contiguous in memory.")             # <<<<<<<<<<<<<<
  *         info.buf = self.data
  *         info.len = self.len
  */
-  __pyx_tuple__15 = PyTuple_Pack(1, __pyx_kp_s_Can_only_create_a_buffer_that_is); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(2, 192, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__15);
-  __Pyx_GIVEREF(__pyx_tuple__15);
+  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_s_Can_only_create_a_buffer_that_is); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(2, 193, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__16);
+  __Pyx_GIVEREF(__pyx_tuple__16);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(2, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__16);
-  __Pyx_GIVEREF(__pyx_tuple__16);
+  __pyx_tuple__17 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(2, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__17);
+  __Pyx_GIVEREF(__pyx_tuple__17);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__17 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(2, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__17);
-  __Pyx_GIVEREF(__pyx_tuple__17);
+  __pyx_tuple__18 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__18);
+  __Pyx_GIVEREF(__pyx_tuple__18);
 
-  /* "View.MemoryView":418
+  /* "View.MemoryView":420
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:
  *             raise TypeError("Cannot assign to read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         have_slices, index = _unellipsify(index, self.view.ndim)
  */
-  __pyx_tuple__18 = PyTuple_Pack(1, __pyx_kp_s_Cannot_assign_to_read_only_memor); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(2, 418, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__18);
-  __Pyx_GIVEREF(__pyx_tuple__18);
+  __pyx_tuple__19 = PyTuple_Pack(1, __pyx_kp_s_Cannot_assign_to_read_only_memor); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(2, 420, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__19);
+  __Pyx_GIVEREF(__pyx_tuple__19);
 
-  /* "View.MemoryView":495
+  /* "View.MemoryView":497
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  *             raise ValueError("Unable to convert item to object")             # <<<<<<<<<<<<<<
  *         else:
  *             if len(self.view.format) == 1:
  */
-  __pyx_tuple__19 = PyTuple_Pack(1, __pyx_kp_s_Unable_to_convert_item_to_object); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(2, 495, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__19);
-  __Pyx_GIVEREF(__pyx_tuple__19);
+  __pyx_tuple__20 = PyTuple_Pack(1, __pyx_kp_s_Unable_to_convert_item_to_object); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(2, 497, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__20);
+  __Pyx_GIVEREF(__pyx_tuple__20);
 
-  /* "View.MemoryView":520
+  /* "View.MemoryView":522
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_ND:
  */
-  __pyx_tuple__20 = PyTuple_Pack(1, __pyx_kp_s_Cannot_create_writable_memory_vi); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(2, 520, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__20);
-  __Pyx_GIVEREF(__pyx_tuple__20);
+  __pyx_tuple__21 = PyTuple_Pack(1, __pyx_kp_s_Cannot_create_writable_memory_vi); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(2, 522, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__21);
+  __Pyx_GIVEREF(__pyx_tuple__21);
 
-  /* "View.MemoryView":570
+  /* "View.MemoryView":572
  *         if self.view.strides == NULL:
  * 
  *             raise ValueError("Buffer view does not expose strides")             # <<<<<<<<<<<<<<
  * 
  *         return tuple([stride for stride in self.view.strides[:self.view.ndim]])
  */
-  __pyx_tuple__21 = PyTuple_Pack(1, __pyx_kp_s_Buffer_view_does_not_expose_stri); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(2, 570, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__21);
-  __Pyx_GIVEREF(__pyx_tuple__21);
+  __pyx_tuple__22 = PyTuple_Pack(1, __pyx_kp_s_Buffer_view_does_not_expose_stri); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(2, 572, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__22);
+  __Pyx_GIVEREF(__pyx_tuple__22);
 
-  /* "View.MemoryView":577
+  /* "View.MemoryView":579
  *     def suboffsets(self):
  *         if self.view.suboffsets == NULL:
  *             return (-1,) * self.view.ndim             # <<<<<<<<<<<<<<
  * 
  *         return tuple([suboffset for suboffset in self.view.suboffsets[:self.view.ndim]])
  */
-  __pyx_tuple__22 = PyTuple_New(1); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(2, 577, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__22);
+  __pyx_tuple__23 = PyTuple_New(1); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(2, 579, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__23);
   __Pyx_INCREF(__pyx_int_neg_1);
   __Pyx_GIVEREF(__pyx_int_neg_1);
-  PyTuple_SET_ITEM(__pyx_tuple__22, 0, __pyx_int_neg_1);
-  __Pyx_GIVEREF(__pyx_tuple__22);
+  PyTuple_SET_ITEM(__pyx_tuple__23, 0, __pyx_int_neg_1);
+  __Pyx_GIVEREF(__pyx_tuple__23);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_tuple__23 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(2, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__23);
-  __Pyx_GIVEREF(__pyx_tuple__23);
+  __pyx_tuple__24 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(2, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__24);
+  __Pyx_GIVEREF(__pyx_tuple__24);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__24 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(2, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__24);
-  __Pyx_GIVEREF(__pyx_tuple__24);
+  __pyx_tuple__25 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__25);
+  __Pyx_GIVEREF(__pyx_tuple__25);
 
-  /* "View.MemoryView":703
+  /* "View.MemoryView":705
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  *             raise ValueError("Indirect dimensions not supported")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__25 = PyTuple_Pack(1, __pyx_kp_s_Indirect_dimensions_not_supporte); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(2, 703, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__25);
-  __Pyx_GIVEREF(__pyx_tuple__25);
+  __pyx_tuple__26 = PyTuple_Pack(1, __pyx_kp_s_Indirect_dimensions_not_supporte); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(2, 705, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__26);
+  __Pyx_GIVEREF(__pyx_tuple__26);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_tuple__26 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(2, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__26);
-  __Pyx_GIVEREF(__pyx_tuple__26);
+  __pyx_tuple__27 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(2, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__27);
+  __Pyx_GIVEREF(__pyx_tuple__27);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__27 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(2, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__27);
-  __Pyx_GIVEREF(__pyx_tuple__27);
+  __pyx_tuple__28 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__28);
+  __Pyx_GIVEREF(__pyx_tuple__28);
+  __pyx_tuple__30 = PyTuple_Pack(3, __pyx_int_184977713, __pyx_int_136983863, __pyx_int_112105877); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__30);
+  __Pyx_GIVEREF(__pyx_tuple__30);
 
   /* "wiver/wiver_cython.pyx":21
  * 
  * 
  * class DestinationChoiceError(ValueError):             # <<<<<<<<<<<<<<
  *     """
  *     Error in destination choice model,
  */
-  __pyx_tuple__29 = PyTuple_Pack(1, __pyx_builtin_ValueError); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(0, 21, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__29);
-  __Pyx_GIVEREF(__pyx_tuple__29);
+  __pyx_tuple__31 = PyTuple_Pack(1, __pyx_builtin_ValueError); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(0, 21, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__31);
+  __Pyx_GIVEREF(__pyx_tuple__31);
 
   /* "wiver/wiver_cython.pyx":27
  *     """
  * 
  * class DataConsistencyError(IndexError):             # <<<<<<<<<<<<<<
  *     """
  *     Data is not consistent and could lead to IndexErrors when running the model
  */
-  __pyx_tuple__30 = PyTuple_Pack(1, __pyx_builtin_IndexError); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(0, 27, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__30);
-  __Pyx_GIVEREF(__pyx_tuple__30);
+  __pyx_tuple__32 = PyTuple_Pack(1, __pyx_builtin_IndexError); if (unlikely(!__pyx_tuple__32)) __PYX_ERR(0, 27, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__32);
+  __Pyx_GIVEREF(__pyx_tuple__32);
 
   /* "(tree fragment)":1
  * def __pyx_unpickle__WIVER(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_tuple__31 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(2, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__31);
-  __Pyx_GIVEREF(__pyx_tuple__31);
-  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__31, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle__WIVER, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __pyx_tuple__33 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__33);
+  __Pyx_GIVEREF(__pyx_tuple__33);
+  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__33, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle__WIVER, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(2, 1, __pyx_L1_error)
 
-  /* "View.MemoryView":286
+  /* "View.MemoryView":287
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
  */
-  __pyx_tuple__32 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct_or_indirect); if (unlikely(!__pyx_tuple__32)) __PYX_ERR(2, 286, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__32);
-  __Pyx_GIVEREF(__pyx_tuple__32);
+  __pyx_tuple__34 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct_or_indirect); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(2, 287, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__34);
+  __Pyx_GIVEREF(__pyx_tuple__34);
 
-  /* "View.MemoryView":287
+  /* "View.MemoryView":288
  * 
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default             # <<<<<<<<<<<<<<
  * cdef indirect = Enum("<strided and indirect>")
  * 
  */
-  __pyx_tuple__33 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(2, 287, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__33);
-  __Pyx_GIVEREF(__pyx_tuple__33);
+  __pyx_tuple__35 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(2, 288, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__35);
+  __Pyx_GIVEREF(__pyx_tuple__35);
 
-  /* "View.MemoryView":288
+  /* "View.MemoryView":289
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__34 = PyTuple_Pack(1, __pyx_kp_s_strided_and_indirect); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(2, 288, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__34);
-  __Pyx_GIVEREF(__pyx_tuple__34);
+  __pyx_tuple__36 = PyTuple_Pack(1, __pyx_kp_s_strided_and_indirect); if (unlikely(!__pyx_tuple__36)) __PYX_ERR(2, 289, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__36);
+  __Pyx_GIVEREF(__pyx_tuple__36);
 
-  /* "View.MemoryView":291
+  /* "View.MemoryView":292
  * 
  * 
  * cdef contiguous = Enum("<contiguous and direct>")             # <<<<<<<<<<<<<<
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")
  * 
  */
-  __pyx_tuple__35 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_direct); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(2, 291, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__35);
-  __Pyx_GIVEREF(__pyx_tuple__35);
+  __pyx_tuple__37 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_direct); if (unlikely(!__pyx_tuple__37)) __PYX_ERR(2, 292, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__37);
+  __Pyx_GIVEREF(__pyx_tuple__37);
 
-  /* "View.MemoryView":292
+  /* "View.MemoryView":293
  * 
  * cdef contiguous = Enum("<contiguous and direct>")
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__36 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_indirect); if (unlikely(!__pyx_tuple__36)) __PYX_ERR(2, 292, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__36);
-  __Pyx_GIVEREF(__pyx_tuple__36);
+  __pyx_tuple__38 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_indirect); if (unlikely(!__pyx_tuple__38)) __PYX_ERR(2, 293, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__38);
+  __Pyx_GIVEREF(__pyx_tuple__38);
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_Enum(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_tuple__37 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__37)) __PYX_ERR(2, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__37);
-  __Pyx_GIVEREF(__pyx_tuple__37);
-  __pyx_codeobj__28 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__37, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Enum, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__28)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __pyx_tuple__39 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__39)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__39);
+  __Pyx_GIVEREF(__pyx_tuple__39);
+  __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__39, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Enum, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(2, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -32508,17 +32735,21 @@
   /* InitThreads.init */
   #if defined(WITH_THREAD) && PY_VERSION_HEX < 0x030700F0
 PyEval_InitThreads();
 #endif
 
 if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1, __pyx_L1_error)
 
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_52120800 = PyInt_FromLong(52120800L); if (unlikely(!__pyx_int_52120800)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_112105877 = PyInt_FromLong(112105877L); if (unlikely(!__pyx_int_112105877)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_136983863 = PyInt_FromLong(136983863L); if (unlikely(!__pyx_int_136983863)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_168422865 = PyInt_FromLong(168422865L); if (unlikely(!__pyx_int_168422865)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_184977713 = PyInt_FromLong(184977713L); if (unlikely(!__pyx_int_184977713)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_194869869 = PyInt_FromLong(194869869L); if (unlikely(!__pyx_int_194869869)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_neg_1 = PyInt_FromLong(-1); if (unlikely(!__pyx_int_neg_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
@@ -32566,15 +32797,16 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
   __pyx_t_1 = PyImport_ImportModule("cythonarrays.array_shapes"); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_12cythonarrays_12array_shapes_ArrayShapes = __Pyx_ImportType(__pyx_t_1, "cythonarrays.array_shapes", "ArrayShapes", sizeof(struct __pyx_obj_12cythonarrays_12array_shapes_ArrayShapes), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_12cythonarrays_12array_shapes_ArrayShapes = __Pyx_ImportType(__pyx_t_1, "cythonarrays.array_shapes", "ArrayShapes", sizeof(struct __pyx_obj_12cythonarrays_12array_shapes_ArrayShapes), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_12cythonarrays_12array_shapes_ArrayShapes),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_12cythonarrays_12array_shapes_ArrayShapes) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_vtabptr_12cythonarrays_12array_shapes_ArrayShapes = (struct __pyx_vtabstruct_12cythonarrays_12array_shapes_ArrayShapes*)__Pyx_GetVtable(__pyx_ptype_12cythonarrays_12array_shapes_ArrayShapes->tp_dict); if (unlikely(!__pyx_vtabptr_12cythonarrays_12array_shapes_ArrayShapes)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_vtabptr_5wiver_12wiver_cython__WIVER = &__pyx_vtable_5wiver_12wiver_cython__WIVER;
   __pyx_vtable_5wiver_12wiver_cython__WIVER.__pyx_base = *__pyx_vtabptr_12cythonarrays_12array_shapes_ArrayShapes;
   __pyx_vtable_5wiver_12wiver_cython__WIVER.calc_daily_trips = (char (*)(struct __pyx_obj_5wiver_12wiver_cython__WIVER *, __pyx_t_12cythonarrays_11numpy_types_long32, int __pyx_skip_dispatch))__pyx_f_5wiver_12wiver_cython_6_WIVER_calc_daily_trips;
   __pyx_vtable_5wiver_12wiver_cython__WIVER._calc_tours = (double (*)(struct __pyx_obj_5wiver_12wiver_cython__WIVER *, __pyx_t_12cythonarrays_11numpy_types_long32, __pyx_t_12cythonarrays_11numpy_types_long32))__pyx_f_5wiver_12wiver_cython_6_WIVER__calc_tours;
   __pyx_vtable_5wiver_12wiver_cython__WIVER._calc_linking_trips = (double (*)(struct __pyx_obj_5wiver_12wiver_cython__WIVER *, __pyx_t_12cythonarrays_11numpy_types_long32, double))__pyx_f_5wiver_12wiver_cython_6_WIVER__calc_linking_trips;
@@ -32599,62 +32831,62 @@
   }
   if (__Pyx_SetVtable(__pyx_type_5wiver_12wiver_cython__WIVER.tp_dict, __pyx_vtabptr_5wiver_12wiver_cython__WIVER) < 0) __PYX_ERR(0, 34, __pyx_L1_error)
   if (PyObject_SetAttr(__pyx_m, __pyx_n_s_WIVER, (PyObject *)&__pyx_type_5wiver_12wiver_cython__WIVER) < 0) __PYX_ERR(0, 34, __pyx_L1_error)
   if (__Pyx_setup_reduce((PyObject*)&__pyx_type_5wiver_12wiver_cython__WIVER) < 0) __PYX_ERR(0, 34, __pyx_L1_error)
   __pyx_ptype_5wiver_12wiver_cython__WIVER = &__pyx_type_5wiver_12wiver_cython__WIVER;
   __pyx_vtabptr_array = &__pyx_vtable_array;
   __pyx_vtable_array.get_memview = (PyObject *(*)(struct __pyx_array_obj *))__pyx_array_get_memview;
-  if (PyType_Ready(&__pyx_type___pyx_array) < 0) __PYX_ERR(2, 105, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type___pyx_array) < 0) __PYX_ERR(2, 106, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type___pyx_array.tp_print = 0;
   #endif
-  if (__Pyx_SetVtable(__pyx_type___pyx_array.tp_dict, __pyx_vtabptr_array) < 0) __PYX_ERR(2, 105, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type___pyx_array) < 0) __PYX_ERR(2, 105, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type___pyx_array.tp_dict, __pyx_vtabptr_array) < 0) __PYX_ERR(2, 106, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type___pyx_array) < 0) __PYX_ERR(2, 106, __pyx_L1_error)
   __pyx_array_type = &__pyx_type___pyx_array;
-  if (PyType_Ready(&__pyx_type___pyx_MemviewEnum) < 0) __PYX_ERR(2, 279, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type___pyx_MemviewEnum) < 0) __PYX_ERR(2, 280, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type___pyx_MemviewEnum.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type___pyx_MemviewEnum.tp_dictoffset && __pyx_type___pyx_MemviewEnum.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type___pyx_MemviewEnum.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type___pyx_MemviewEnum) < 0) __PYX_ERR(2, 279, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type___pyx_MemviewEnum) < 0) __PYX_ERR(2, 280, __pyx_L1_error)
   __pyx_MemviewEnum_type = &__pyx_type___pyx_MemviewEnum;
   __pyx_vtabptr_memoryview = &__pyx_vtable_memoryview;
   __pyx_vtable_memoryview.get_item_pointer = (char *(*)(struct __pyx_memoryview_obj *, PyObject *))__pyx_memoryview_get_item_pointer;
   __pyx_vtable_memoryview.is_slice = (PyObject *(*)(struct __pyx_memoryview_obj *, PyObject *))__pyx_memoryview_is_slice;
   __pyx_vtable_memoryview.setitem_slice_assignment = (PyObject *(*)(struct __pyx_memoryview_obj *, PyObject *, PyObject *))__pyx_memoryview_setitem_slice_assignment;
   __pyx_vtable_memoryview.setitem_slice_assign_scalar = (PyObject *(*)(struct __pyx_memoryview_obj *, struct __pyx_memoryview_obj *, PyObject *))__pyx_memoryview_setitem_slice_assign_scalar;
   __pyx_vtable_memoryview.setitem_indexed = (PyObject *(*)(struct __pyx_memoryview_obj *, PyObject *, PyObject *))__pyx_memoryview_setitem_indexed;
   __pyx_vtable_memoryview.convert_item_to_object = (PyObject *(*)(struct __pyx_memoryview_obj *, char *))__pyx_memoryview_convert_item_to_object;
   __pyx_vtable_memoryview.assign_item_from_object = (PyObject *(*)(struct __pyx_memoryview_obj *, char *, PyObject *))__pyx_memoryview_assign_item_from_object;
-  if (PyType_Ready(&__pyx_type___pyx_memoryview) < 0) __PYX_ERR(2, 330, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type___pyx_memoryview) < 0) __PYX_ERR(2, 331, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type___pyx_memoryview.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type___pyx_memoryview.tp_dictoffset && __pyx_type___pyx_memoryview.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type___pyx_memoryview.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type___pyx_memoryview.tp_dict, __pyx_vtabptr_memoryview) < 0) __PYX_ERR(2, 330, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type___pyx_memoryview) < 0) __PYX_ERR(2, 330, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type___pyx_memoryview.tp_dict, __pyx_vtabptr_memoryview) < 0) __PYX_ERR(2, 331, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type___pyx_memoryview) < 0) __PYX_ERR(2, 331, __pyx_L1_error)
   __pyx_memoryview_type = &__pyx_type___pyx_memoryview;
   __pyx_vtabptr__memoryviewslice = &__pyx_vtable__memoryviewslice;
   __pyx_vtable__memoryviewslice.__pyx_base = *__pyx_vtabptr_memoryview;
   __pyx_vtable__memoryviewslice.__pyx_base.convert_item_to_object = (PyObject *(*)(struct __pyx_memoryview_obj *, char *))__pyx_memoryviewslice_convert_item_to_object;
   __pyx_vtable__memoryviewslice.__pyx_base.assign_item_from_object = (PyObject *(*)(struct __pyx_memoryview_obj *, char *, PyObject *))__pyx_memoryviewslice_assign_item_from_object;
   __pyx_type___pyx_memoryviewslice.tp_base = __pyx_memoryview_type;
-  if (PyType_Ready(&__pyx_type___pyx_memoryviewslice) < 0) __PYX_ERR(2, 965, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type___pyx_memoryviewslice) < 0) __PYX_ERR(2, 967, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type___pyx_memoryviewslice.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type___pyx_memoryviewslice.tp_dictoffset && __pyx_type___pyx_memoryviewslice.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type___pyx_memoryviewslice.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type___pyx_memoryviewslice.tp_dict, __pyx_vtabptr__memoryviewslice) < 0) __PYX_ERR(2, 965, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type___pyx_memoryviewslice) < 0) __PYX_ERR(2, 965, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type___pyx_memoryviewslice.tp_dict, __pyx_vtabptr__memoryviewslice) < 0) __PYX_ERR(2, 967, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type___pyx_memoryviewslice) < 0) __PYX_ERR(2, 967, __pyx_L1_error)
   __pyx_memoryviewslice_type = &__pyx_type___pyx_memoryviewslice;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -32669,53 +32901,68 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 200, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(3, 200, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(3, 223, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(3, 227, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(3, 239, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(3, 771, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_number) __PYX_ERR(3, 773, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(3, 775, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(3, 777, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(3, 779, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(3, 781, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(3, 783, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(3, 785, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(3, 787, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_character) __PYX_ERR(3, 789, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(3, 827, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT(PyArray_Descr),
+  __Pyx_ImportType_CheckSize_Ignore);
+   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(3, 199, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
+   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(3, 222, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayMultiIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
+   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(3, 226, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayObject),
+  __Pyx_ImportType_CheckSize_Ignore);
+   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(3, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(3, 770, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_number) __PYX_ERR(3, 772, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(3, 774, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(3, 776, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(3, 778, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(3, 780, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(3, 782, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(3, 784, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(3, 786, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_character) __PYX_ERR(3, 788, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT(PyUFuncObject),
+  __Pyx_ImportType_CheckSize_Ignore);
+   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(3, 826, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -32903,15 +33150,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_wiver__wiver_cython) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name_2, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -32999,38 +33246,38 @@
  * 
  * 
  * class DestinationChoiceError(ValueError):             # <<<<<<<<<<<<<<
  *     """
  *     Error in destination choice model,
  */
   __Pyx_TraceLine(21,0,__PYX_ERR(0, 21, __pyx_L1_error))
-  __pyx_t_1 = __Pyx_CalculateMetaclass(NULL, __pyx_tuple__29); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 21, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CalculateMetaclass(NULL, __pyx_tuple__31); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 21, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_Py3MetaclassPrepare(__pyx_t_1, __pyx_tuple__29, __pyx_n_s_DestinationChoiceError, __pyx_n_s_DestinationChoiceError, (PyObject *) NULL, __pyx_n_s_wiver_wiver_cython, __pyx_kp_s_Error_in_destination_choice_mod); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 21, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Py3MetaclassPrepare(__pyx_t_1, __pyx_tuple__31, __pyx_n_s_DestinationChoiceError, __pyx_n_s_DestinationChoiceError, (PyObject *) NULL, __pyx_n_s_wiver_wiver_cython, __pyx_kp_s_Error_in_destination_choice_mod); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 21, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_Py3ClassCreate(__pyx_t_1, __pyx_n_s_DestinationChoiceError, __pyx_tuple__29, __pyx_t_2, NULL, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 21, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_Py3ClassCreate(__pyx_t_1, __pyx_n_s_DestinationChoiceError, __pyx_tuple__31, __pyx_t_2, NULL, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 21, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_DestinationChoiceError, __pyx_t_3) < 0) __PYX_ERR(0, 21, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "wiver/wiver_cython.pyx":27
  *     """
  * 
  * class DataConsistencyError(IndexError):             # <<<<<<<<<<<<<<
  *     """
  *     Data is not consistent and could lead to IndexErrors when running the model
  */
   __Pyx_TraceLine(27,0,__PYX_ERR(0, 27, __pyx_L1_error))
-  __pyx_t_1 = __Pyx_CalculateMetaclass(NULL, __pyx_tuple__30); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 27, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CalculateMetaclass(NULL, __pyx_tuple__32); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 27, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_Py3MetaclassPrepare(__pyx_t_1, __pyx_tuple__30, __pyx_n_s_DataConsistencyError, __pyx_n_s_DataConsistencyError, (PyObject *) NULL, __pyx_n_s_wiver_wiver_cython, __pyx_kp_s_Data_is_not_consistent_and_coul); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 27, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Py3MetaclassPrepare(__pyx_t_1, __pyx_tuple__32, __pyx_n_s_DataConsistencyError, __pyx_n_s_DataConsistencyError, (PyObject *) NULL, __pyx_n_s_wiver_wiver_cython, __pyx_kp_s_Data_is_not_consistent_and_coul); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 27, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_Py3ClassCreate(__pyx_t_1, __pyx_n_s_DataConsistencyError, __pyx_tuple__30, __pyx_t_2, NULL, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 27, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_Py3ClassCreate(__pyx_t_1, __pyx_n_s_DataConsistencyError, __pyx_tuple__32, __pyx_t_2, NULL, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 27, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_DataConsistencyError, __pyx_t_3) < 0) __PYX_ERR(0, 27, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "wiver/wiver_cython.pyx":40
@@ -33201,727 +33448,727 @@
  */
   __Pyx_TraceLine(1,0,__PYX_ERR(0, 1, __pyx_L1_error))
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":735
+  /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
-  __Pyx_TraceLine(735,0,__PYX_ERR(3, 735, __pyx_L1_error))
+  __Pyx_TraceLine(734,0,__PYX_ERR(3, 734, __pyx_L1_error))
 
 
-  /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":738
+  /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
-  __Pyx_TraceLine(738,0,__PYX_ERR(3, 738, __pyx_L1_error))
+  __Pyx_TraceLine(737,0,__PYX_ERR(3, 737, __pyx_L1_error))
 
 
-  /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":741
+  /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
-  __Pyx_TraceLine(741,0,__PYX_ERR(3, 741, __pyx_L1_error))
+  __Pyx_TraceLine(740,0,__PYX_ERR(3, 740, __pyx_L1_error))
 
 
-  /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":744
+  /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
-  __Pyx_TraceLine(744,0,__PYX_ERR(3, 744, __pyx_L1_error))
+  __Pyx_TraceLine(743,0,__PYX_ERR(3, 743, __pyx_L1_error))
 
 
-  /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":747
+  /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
-  __Pyx_TraceLine(747,0,__PYX_ERR(3, 747, __pyx_L1_error))
+  __Pyx_TraceLine(746,0,__PYX_ERR(3, 746, __pyx_L1_error))
 
 
-  /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":750
+  /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
-  __Pyx_TraceLine(750,0,__PYX_ERR(3, 750, __pyx_L1_error))
+  __Pyx_TraceLine(749,0,__PYX_ERR(3, 749, __pyx_L1_error))
 
 
-  /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":929
+  /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
-  __Pyx_TraceLine(929,0,__PYX_ERR(3, 929, __pyx_L1_error))
+  __Pyx_TraceLine(928,0,__PYX_ERR(3, 928, __pyx_L1_error))
 
 
-  /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":933
+  /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
-  __Pyx_TraceLine(933,0,__PYX_ERR(3, 933, __pyx_L1_error))
+  __Pyx_TraceLine(932,0,__PYX_ERR(3, 932, __pyx_L1_error))
 
 
-  /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":941
+  /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
-  __Pyx_TraceLine(941,0,__PYX_ERR(3, 941, __pyx_L1_error))
+  __Pyx_TraceLine(940,0,__PYX_ERR(3, 940, __pyx_L1_error))
 
 
-  /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":947
+  /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
-  __Pyx_TraceLine(947,0,__PYX_ERR(3, 947, __pyx_L1_error))
+  __Pyx_TraceLine(946,0,__PYX_ERR(3, 946, __pyx_L1_error))
 
 
-  /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":953
+  /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
-  __Pyx_TraceLine(953,0,__PYX_ERR(3, 953, __pyx_L1_error))
+  __Pyx_TraceLine(952,0,__PYX_ERR(3, 952, __pyx_L1_error))
 
 
-  /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":967
+  /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
-  __Pyx_TraceLine(967,0,__PYX_ERR(3, 967, __pyx_L1_error))
+  __Pyx_TraceLine(966,0,__PYX_ERR(3, 966, __pyx_L1_error))
 
 
-  /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":982
+  /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
-  __Pyx_TraceLine(982,0,__PYX_ERR(3, 982, __pyx_L1_error))
+  __Pyx_TraceLine(981,0,__PYX_ERR(3, 981, __pyx_L1_error))
 
 
-  /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":997
+  /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
-  __Pyx_TraceLine(997,0,__PYX_ERR(3, 997, __pyx_L1_error))
+  __Pyx_TraceLine(996,0,__PYX_ERR(3, 996, __pyx_L1_error))
 
 
-  /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":1007
+  /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
-  __Pyx_TraceLine(1007,0,__PYX_ERR(3, 1007, __pyx_L1_error))
+  __Pyx_TraceLine(1006,0,__PYX_ERR(3, 1006, __pyx_L1_error))
 
 
-  /* "../../../Miniconda37-x64/envs/test-environment/lib/site-packages/numpy/__init__.pxd":1014
+  /* "../../../Miniconda37-x64/envs/test-environment/Lib/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
-  __Pyx_TraceLine(1014,0,__PYX_ERR(3, 1014, __pyx_L1_error))
+  __Pyx_TraceLine(1013,0,__PYX_ERR(3, 1013, __pyx_L1_error))
 
 
-  /* "View.MemoryView":209
+  /* "View.MemoryView":210
  *         info.obj = self
  * 
  *     __pyx_getbuffer = capsule(<void *> &__pyx_array_getbuffer, "getbuffer(obj, view, flags)")             # <<<<<<<<<<<<<<
  * 
  *     def __dealloc__(array self):
  */
-  __Pyx_TraceLine(209,0,__PYX_ERR(2, 209, __pyx_L1_error))
-  __pyx_t_1 = __pyx_capsule_create(((void *)(&__pyx_array_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 209, __pyx_L1_error)
+  __Pyx_TraceLine(210,0,__PYX_ERR(2, 210, __pyx_L1_error))
+  __pyx_t_1 = __pyx_capsule_create(((void *)(&__pyx_array_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 210, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem((PyObject *)__pyx_array_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_1) < 0) __PYX_ERR(2, 209, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_array_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_1) < 0) __PYX_ERR(2, 210, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   PyType_Modified(__pyx_array_type);
 
-  /* "View.MemoryView":226
+  /* "View.MemoryView":227
  * 
  *     @cname('get_memview')
  *     cdef get_memview(self):             # <<<<<<<<<<<<<<
  *         flags =  PyBUF_ANY_CONTIGUOUS|PyBUF_FORMAT|PyBUF_WRITABLE
  *         return  memoryview(self, flags, self.dtype_is_object)
  */
-  __Pyx_TraceLine(226,0,__PYX_ERR(2, 226, __pyx_L1_error))
+  __Pyx_TraceLine(227,0,__PYX_ERR(2, 227, __pyx_L1_error))
 
 
-  /* "View.MemoryView":244
+  /* "View.MemoryView":245
  * 
  * @cname("__pyx_array_new")
  * cdef array array_cwrapper(tuple shape, Py_ssize_t itemsize, char *format,             # <<<<<<<<<<<<<<
  *                           char *mode, char *buf):
  *     cdef array result
  */
-  __Pyx_TraceLine(244,0,__PYX_ERR(2, 244, __pyx_L1_error))
+  __Pyx_TraceLine(245,0,__PYX_ERR(2, 245, __pyx_L1_error))
 
 
-  /* "View.MemoryView":286
+  /* "View.MemoryView":287
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
  */
-  __Pyx_TraceLine(286,0,__PYX_ERR(2, 286, __pyx_L1_error))
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__32, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 286, __pyx_L1_error)
+  __Pyx_TraceLine(287,0,__PYX_ERR(2, 287, __pyx_L1_error))
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__34, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 287, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(generic);
   __Pyx_DECREF_SET(generic, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "View.MemoryView":287
+  /* "View.MemoryView":288
  * 
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default             # <<<<<<<<<<<<<<
  * cdef indirect = Enum("<strided and indirect>")
  * 
  */
-  __Pyx_TraceLine(287,0,__PYX_ERR(2, 287, __pyx_L1_error))
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__33, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 287, __pyx_L1_error)
+  __Pyx_TraceLine(288,0,__PYX_ERR(2, 288, __pyx_L1_error))
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__35, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 288, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(strided);
   __Pyx_DECREF_SET(strided, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "View.MemoryView":288
+  /* "View.MemoryView":289
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_TraceLine(288,0,__PYX_ERR(2, 288, __pyx_L1_error))
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__34, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 288, __pyx_L1_error)
+  __Pyx_TraceLine(289,0,__PYX_ERR(2, 289, __pyx_L1_error))
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__36, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 289, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(indirect);
   __Pyx_DECREF_SET(indirect, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "View.MemoryView":291
+  /* "View.MemoryView":292
  * 
  * 
  * cdef contiguous = Enum("<contiguous and direct>")             # <<<<<<<<<<<<<<
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")
  * 
  */
-  __Pyx_TraceLine(291,0,__PYX_ERR(2, 291, __pyx_L1_error))
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__35, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 291, __pyx_L1_error)
+  __Pyx_TraceLine(292,0,__PYX_ERR(2, 292, __pyx_L1_error))
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__37, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 292, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(contiguous);
   __Pyx_DECREF_SET(contiguous, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "View.MemoryView":292
+  /* "View.MemoryView":293
  * 
  * cdef contiguous = Enum("<contiguous and direct>")
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_TraceLine(292,0,__PYX_ERR(2, 292, __pyx_L1_error))
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__36, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 292, __pyx_L1_error)
+  __Pyx_TraceLine(293,0,__PYX_ERR(2, 293, __pyx_L1_error))
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__38, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 293, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(indirect_contiguous);
   __Pyx_DECREF_SET(indirect_contiguous, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "View.MemoryView":298
+  /* "View.MemoryView":299
  * 
  * @cname('__pyx_align_pointer')
  * cdef void *align_pointer(void *memory, size_t alignment) nogil:             # <<<<<<<<<<<<<<
  *     "Align pointer memory on a given boundary"
  *     cdef Py_intptr_t aligned_p = <Py_intptr_t> memory
  */
-  __Pyx_TraceLine(298,0,__PYX_ERR(2, 298, __pyx_L1_error))
+  __Pyx_TraceLine(299,0,__PYX_ERR(2, 299, __pyx_L1_error))
 
 
-  /* "View.MemoryView":316
+  /* "View.MemoryView":317
  * 
  * DEF THREAD_LOCKS_PREALLOCATED = 8
  * cdef int __pyx_memoryview_thread_locks_used = 0             # <<<<<<<<<<<<<<
  * cdef PyThread_type_lock[THREAD_LOCKS_PREALLOCATED] __pyx_memoryview_thread_locks = [
  *     PyThread_allocate_lock(),
  */
-  __Pyx_TraceLine(316,0,__PYX_ERR(2, 316, __pyx_L1_error))
+  __Pyx_TraceLine(317,0,__PYX_ERR(2, 317, __pyx_L1_error))
   __pyx_memoryview_thread_locks_used = 0;
 
-  /* "View.MemoryView":317
+  /* "View.MemoryView":318
  * DEF THREAD_LOCKS_PREALLOCATED = 8
  * cdef int __pyx_memoryview_thread_locks_used = 0
  * cdef PyThread_type_lock[THREAD_LOCKS_PREALLOCATED] __pyx_memoryview_thread_locks = [             # <<<<<<<<<<<<<<
  *     PyThread_allocate_lock(),
  *     PyThread_allocate_lock(),
  */
-  __Pyx_TraceLine(317,0,__PYX_ERR(2, 317, __pyx_L1_error))
+  __Pyx_TraceLine(318,0,__PYX_ERR(2, 318, __pyx_L1_error))
   __pyx_t_4[0] = PyThread_allocate_lock();
   __pyx_t_4[1] = PyThread_allocate_lock();
   __pyx_t_4[2] = PyThread_allocate_lock();
   __pyx_t_4[3] = PyThread_allocate_lock();
   __pyx_t_4[4] = PyThread_allocate_lock();
   __pyx_t_4[5] = PyThread_allocate_lock();
   __pyx_t_4[6] = PyThread_allocate_lock();
   __pyx_t_4[7] = PyThread_allocate_lock();
   memcpy(&(__pyx_memoryview_thread_locks[0]), __pyx_t_4, sizeof(__pyx_memoryview_thread_locks[0]) * (8));
 
-  /* "View.MemoryView":393
+  /* "View.MemoryView":395
  *                 PyThread_free_lock(self.lock)
  * 
  *     cdef char *get_item_pointer(memoryview self, object index) except NULL:             # <<<<<<<<<<<<<<
  *         cdef Py_ssize_t dim
  *         cdef char *itemp = <char *> self.view.buf
  */
-  __Pyx_TraceLine(393,0,__PYX_ERR(2, 393, __pyx_L1_error))
+  __Pyx_TraceLine(395,0,__PYX_ERR(2, 395, __pyx_L1_error))
 
 
-  /* "View.MemoryView":431
+  /* "View.MemoryView":433
  *             self.setitem_indexed(index, value)
  * 
  *     cdef is_slice(self, obj):             # <<<<<<<<<<<<<<
  *         if not isinstance(obj, memoryview):
  *             try:
  */
-  __Pyx_TraceLine(431,0,__PYX_ERR(2, 431, __pyx_L1_error))
+  __Pyx_TraceLine(433,0,__PYX_ERR(2, 433, __pyx_L1_error))
 
 
-  /* "View.MemoryView":441
+  /* "View.MemoryView":443
  *         return obj
  * 
  *     cdef setitem_slice_assignment(self, dst, src):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice dst_slice
  *         cdef __Pyx_memviewslice src_slice
  */
-  __Pyx_TraceLine(441,0,__PYX_ERR(2, 441, __pyx_L1_error))
+  __Pyx_TraceLine(443,0,__PYX_ERR(2, 443, __pyx_L1_error))
 
 
-  /* "View.MemoryView":449
+  /* "View.MemoryView":451
  *                                  src.ndim, dst.ndim, self.dtype_is_object)
  * 
  *     cdef setitem_slice_assign_scalar(self, memoryview dst, value):             # <<<<<<<<<<<<<<
  *         cdef int array[128]
  *         cdef void *tmp = NULL
  */
-  __Pyx_TraceLine(449,0,__PYX_ERR(2, 449, __pyx_L1_error))
+  __Pyx_TraceLine(451,0,__PYX_ERR(2, 451, __pyx_L1_error))
 
 
-  /* "View.MemoryView":481
+  /* "View.MemoryView":483
  *             PyMem_Free(tmp)
  * 
  *     cdef setitem_indexed(self, index, value):             # <<<<<<<<<<<<<<
  *         cdef char *itemp = self.get_item_pointer(index)
  *         self.assign_item_from_object(itemp, value)
  */
-  __Pyx_TraceLine(481,0,__PYX_ERR(2, 481, __pyx_L1_error))
+  __Pyx_TraceLine(483,0,__PYX_ERR(2, 483, __pyx_L1_error))
 
 
-  /* "View.MemoryView":485
+  /* "View.MemoryView":487
  *         self.assign_item_from_object(itemp, value)
  * 
  *     cdef convert_item_to_object(self, char *itemp):             # <<<<<<<<<<<<<<
  *         """Only used if instantiated manually by the user, or if Cython doesn't
  *         know how to convert the type"""
  */
-  __Pyx_TraceLine(485,0,__PYX_ERR(2, 485, __pyx_L1_error))
+  __Pyx_TraceLine(487,0,__PYX_ERR(2, 487, __pyx_L1_error))
 
 
-  /* "View.MemoryView":501
+  /* "View.MemoryView":503
  *             return result
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):             # <<<<<<<<<<<<<<
  *         """Only used if instantiated manually by the user, or if Cython doesn't
  *         know how to convert the type"""
  */
-  __Pyx_TraceLine(501,0,__PYX_ERR(2, 501, __pyx_L1_error))
+  __Pyx_TraceLine(503,0,__PYX_ERR(2, 503, __pyx_L1_error))
 
 
-  /* "View.MemoryView":549
+  /* "View.MemoryView":551
  *         info.obj = self
  * 
  *     __pyx_getbuffer = capsule(<void *> &__pyx_memoryview_getbuffer, "getbuffer(obj, view, flags)")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_TraceLine(549,0,__PYX_ERR(2, 549, __pyx_L1_error))
-  __pyx_t_1 = __pyx_capsule_create(((void *)(&__pyx_memoryview_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 549, __pyx_L1_error)
+  __Pyx_TraceLine(551,0,__PYX_ERR(2, 551, __pyx_L1_error))
+  __pyx_t_1 = __pyx_capsule_create(((void *)(&__pyx_memoryview_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 551, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem((PyObject *)__pyx_memoryview_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_1) < 0) __PYX_ERR(2, 549, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_memoryview_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_1) < 0) __PYX_ERR(2, 551, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   PyType_Modified(__pyx_memoryview_type);
 
-  /* "View.MemoryView":657
+  /* "View.MemoryView":659
  * 
  * @cname('__pyx_memoryview_new')
  * cdef memoryview_cwrapper(object o, int flags, bint dtype_is_object, __Pyx_TypeInfo *typeinfo):             # <<<<<<<<<<<<<<
  *     cdef memoryview result = memoryview(o, flags, dtype_is_object)
  *     result.typeinfo = typeinfo
  */
-  __Pyx_TraceLine(657,0,__PYX_ERR(2, 657, __pyx_L1_error))
+  __Pyx_TraceLine(659,0,__PYX_ERR(2, 659, __pyx_L1_error))
 
 
-  /* "View.MemoryView":663
+  /* "View.MemoryView":665
  * 
  * @cname('__pyx_memoryview_check')
  * cdef inline bint memoryview_check(object o):             # <<<<<<<<<<<<<<
  *     return isinstance(o, memoryview)
  * 
  */
-  __Pyx_TraceLine(663,0,__PYX_ERR(2, 663, __pyx_L1_error))
+  __Pyx_TraceLine(665,0,__PYX_ERR(2, 665, __pyx_L1_error))
 
 
-  /* "View.MemoryView":666
+  /* "View.MemoryView":668
  *     return isinstance(o, memoryview)
  * 
  * cdef tuple _unellipsify(object index, int ndim):             # <<<<<<<<<<<<<<
  *     """
  *     Replace all ellipses with full slices and fill incomplete indices with
  */
-  __Pyx_TraceLine(666,0,__PYX_ERR(2, 666, __pyx_L1_error))
+  __Pyx_TraceLine(668,0,__PYX_ERR(2, 668, __pyx_L1_error))
 
 
-  /* "View.MemoryView":700
+  /* "View.MemoryView":702
  *     return have_slices or nslices, tuple(result)
  * 
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):             # <<<<<<<<<<<<<<
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  */
-  __Pyx_TraceLine(700,0,__PYX_ERR(2, 700, __pyx_L1_error))
+  __Pyx_TraceLine(702,0,__PYX_ERR(2, 702, __pyx_L1_error))
 
 
-  /* "View.MemoryView":710
+  /* "View.MemoryView":712
  * 
  * @cname('__pyx_memview_slice')
  * cdef memoryview memview_slice(memoryview memview, object indices):             # <<<<<<<<<<<<<<
  *     cdef int new_ndim = 0, suboffset_dim = -1, dim
  *     cdef bint negative_step
  */
-  __Pyx_TraceLine(710,0,__PYX_ERR(2, 710, __pyx_L1_error))
+  __Pyx_TraceLine(712,0,__PYX_ERR(2, 712, __pyx_L1_error))
 
 
-  /* "View.MemoryView":807
+  /* "View.MemoryView":809
  * 
  * @cname('__pyx_memoryview_slice_memviewslice')
  * cdef int slice_memviewslice(             # <<<<<<<<<<<<<<
  *         __Pyx_memviewslice *dst,
  *         Py_ssize_t shape, Py_ssize_t stride, Py_ssize_t suboffset,
  */
-  __Pyx_TraceLine(807,0,__PYX_ERR(2, 807, __pyx_L1_error))
+  __Pyx_TraceLine(809,0,__PYX_ERR(2, 809, __pyx_L1_error))
 
 
-  /* "View.MemoryView":910
+  /* "View.MemoryView":912
  * 
  * @cname('__pyx_pybuffer_index')
  * cdef char *pybuffer_index(Py_buffer *view, char *bufp, Py_ssize_t index,             # <<<<<<<<<<<<<<
  *                           Py_ssize_t dim) except NULL:
  *     cdef Py_ssize_t shape, stride, suboffset = -1
  */
-  __Pyx_TraceLine(910,0,__PYX_ERR(2, 910, __pyx_L1_error))
+  __Pyx_TraceLine(912,0,__PYX_ERR(2, 912, __pyx_L1_error))
 
 
-  /* "View.MemoryView":943
+  /* "View.MemoryView":945
  * 
  * @cname('__pyx_memslice_transpose')
  * cdef int transpose_memslice(__Pyx_memviewslice *memslice) nogil except 0:             # <<<<<<<<<<<<<<
  *     cdef int ndim = memslice.memview.view.ndim
  * 
  */
-  __Pyx_TraceLine(943,0,__PYX_ERR(2, 943, __pyx_L1_error))
+  __Pyx_TraceLine(945,0,__PYX_ERR(2, 945, __pyx_L1_error))
 
 
-  /* "View.MemoryView":979
+  /* "View.MemoryView":981
  *         __PYX_XDEC_MEMVIEW(&self.from_slice, 1)
  * 
  *     cdef convert_item_to_object(self, char *itemp):             # <<<<<<<<<<<<<<
  *         if self.to_object_func != NULL:
  *             return self.to_object_func(itemp)
  */
-  __Pyx_TraceLine(979,0,__PYX_ERR(2, 979, __pyx_L1_error))
+  __Pyx_TraceLine(981,0,__PYX_ERR(2, 981, __pyx_L1_error))
 
 
-  /* "View.MemoryView":985
+  /* "View.MemoryView":987
  *             return memoryview.convert_item_to_object(self, itemp)
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):             # <<<<<<<<<<<<<<
  *         if self.to_dtype_func != NULL:
  *             self.to_dtype_func(itemp, value)
  */
-  __Pyx_TraceLine(985,0,__PYX_ERR(2, 985, __pyx_L1_error))
+  __Pyx_TraceLine(987,0,__PYX_ERR(2, 987, __pyx_L1_error))
 
 
-  /* "View.MemoryView":995
+  /* "View.MemoryView":997
  *         return self.from_object
  * 
  *     __pyx_getbuffer = capsule(<void *> &__pyx_memoryview_getbuffer, "getbuffer(obj, view, flags)")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_TraceLine(995,0,__PYX_ERR(2, 995, __pyx_L1_error))
-  __pyx_t_1 = __pyx_capsule_create(((void *)(&__pyx_memoryview_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 995, __pyx_L1_error)
+  __Pyx_TraceLine(997,0,__PYX_ERR(2, 997, __pyx_L1_error))
+  __pyx_t_1 = __pyx_capsule_create(((void *)(&__pyx_memoryview_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 997, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem((PyObject *)__pyx_memoryviewslice_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_1) < 0) __PYX_ERR(2, 995, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_memoryviewslice_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_1) < 0) __PYX_ERR(2, 997, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   PyType_Modified(__pyx_memoryviewslice_type);
 
-  /* "View.MemoryView":999
+  /* "View.MemoryView":1001
  * 
  * @cname('__pyx_memoryview_fromslice')
  * cdef memoryview_fromslice(__Pyx_memviewslice memviewslice,             # <<<<<<<<<<<<<<
  *                           int ndim,
  *                           object (*to_object_func)(char *),
  */
-  __Pyx_TraceLine(999,0,__PYX_ERR(2, 999, __pyx_L1_error))
+  __Pyx_TraceLine(1001,0,__PYX_ERR(2, 1001, __pyx_L1_error))
 
 
-  /* "View.MemoryView":1052
+  /* "View.MemoryView":1054
  * 
  * @cname('__pyx_memoryview_get_slice_from_memoryview')
  * cdef __Pyx_memviewslice *get_slice_from_memview(memoryview memview,             # <<<<<<<<<<<<<<
  *                                                    __Pyx_memviewslice *mslice) except NULL:
  *     cdef _memoryviewslice obj
  */
-  __Pyx_TraceLine(1052,0,__PYX_ERR(2, 1052, __pyx_L1_error))
+  __Pyx_TraceLine(1054,0,__PYX_ERR(2, 1054, __pyx_L1_error))
 
 
-  /* "View.MemoryView":1063
+  /* "View.MemoryView":1065
  * 
  * @cname('__pyx_memoryview_slice_copy')
  * cdef void slice_copy(memoryview memview, __Pyx_memviewslice *dst):             # <<<<<<<<<<<<<<
  *     cdef int dim
  *     cdef (Py_ssize_t*) shape, strides, suboffsets
  */
-  __Pyx_TraceLine(1063,0,__PYX_ERR(2, 1063, __pyx_L1_error))
+  __Pyx_TraceLine(1065,0,__PYX_ERR(2, 1065, __pyx_L1_error))
 
 
-  /* "View.MemoryView":1080
+  /* "View.MemoryView":1082
  * 
  * @cname('__pyx_memoryview_copy_object')
  * cdef memoryview_copy(memoryview memview):             # <<<<<<<<<<<<<<
  *     "Create a new memoryview object"
  *     cdef __Pyx_memviewslice memviewslice
  */
-  __Pyx_TraceLine(1080,0,__PYX_ERR(2, 1080, __pyx_L1_error))
+  __Pyx_TraceLine(1082,0,__PYX_ERR(2, 1082, __pyx_L1_error))
 
 
-  /* "View.MemoryView":1087
+  /* "View.MemoryView":1089
  * 
  * @cname('__pyx_memoryview_copy_object_from_slice')
  * cdef memoryview_copy_from_slice(memoryview memview, __Pyx_memviewslice *memviewslice):             # <<<<<<<<<<<<<<
  *     """
  *     Create a new memoryview object from a given memoryview object and slice.
  */
-  __Pyx_TraceLine(1087,0,__PYX_ERR(2, 1087, __pyx_L1_error))
+  __Pyx_TraceLine(1089,0,__PYX_ERR(2, 1089, __pyx_L1_error))
 
 
-  /* "View.MemoryView":1109
+  /* "View.MemoryView":1111
  * 
  * 
  * cdef Py_ssize_t abs_py_ssize_t(Py_ssize_t arg) nogil:             # <<<<<<<<<<<<<<
  *     if arg < 0:
  *         return -arg
  */
-  __Pyx_TraceLine(1109,0,__PYX_ERR(2, 1109, __pyx_L1_error))
+  __Pyx_TraceLine(1111,0,__PYX_ERR(2, 1111, __pyx_L1_error))
 
 
-  /* "View.MemoryView":1116
+  /* "View.MemoryView":1118
  * 
  * @cname('__pyx_get_best_slice_order')
  * cdef char get_best_order(__Pyx_memviewslice *mslice, int ndim) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     Figure out the best memory access order for a given slice.
  */
-  __Pyx_TraceLine(1116,0,__PYX_ERR(2, 1116, __pyx_L1_error))
+  __Pyx_TraceLine(1118,0,__PYX_ERR(2, 1118, __pyx_L1_error))
 
 
-  /* "View.MemoryView":1170
+  /* "View.MemoryView":1172
  *             dst_data += dst_stride
  * 
  * cdef void copy_strided_to_strided(__Pyx_memviewslice *src,             # <<<<<<<<<<<<<<
  *                                   __Pyx_memviewslice *dst,
  *                                   int ndim, size_t itemsize) nogil:
  */
-  __Pyx_TraceLine(1170,0,__PYX_ERR(2, 1170, __pyx_L1_error))
+  __Pyx_TraceLine(1172,0,__PYX_ERR(2, 1172, __pyx_L1_error))
 
 
-  /* "View.MemoryView":1177
+  /* "View.MemoryView":1179
  * 
  * @cname('__pyx_memoryview_slice_get_size')
  * cdef Py_ssize_t slice_get_size(__Pyx_memviewslice *src, int ndim) nogil:             # <<<<<<<<<<<<<<
  *     "Return the size of the memory occupied by the slice in number of bytes"
  *     cdef Py_ssize_t shape, size = src.memview.view.itemsize
  */
-  __Pyx_TraceLine(1177,0,__PYX_ERR(2, 1177, __pyx_L1_error))
+  __Pyx_TraceLine(1179,0,__PYX_ERR(2, 1179, __pyx_L1_error))
 
 
-  /* "View.MemoryView":1187
+  /* "View.MemoryView":1189
  * 
  * @cname('__pyx_fill_contig_strides_array')
  * cdef Py_ssize_t fill_contig_strides_array(             # <<<<<<<<<<<<<<
  *                 Py_ssize_t *shape, Py_ssize_t *strides, Py_ssize_t stride,
  *                 int ndim, char order) nogil:
  */
-  __Pyx_TraceLine(1187,0,__PYX_ERR(2, 1187, __pyx_L1_error))
+  __Pyx_TraceLine(1189,0,__PYX_ERR(2, 1189, __pyx_L1_error))
 
 
-  /* "View.MemoryView":1208
+  /* "View.MemoryView":1210
  * 
  * @cname('__pyx_memoryview_copy_data_to_temp')
  * cdef void *copy_data_to_temp(__Pyx_memviewslice *src,             # <<<<<<<<<<<<<<
  *                              __Pyx_memviewslice *tmpslice,
  *                              char order,
  */
-  __Pyx_TraceLine(1208,0,__PYX_ERR(2, 1208, __pyx_L1_error))
+  __Pyx_TraceLine(1210,0,__PYX_ERR(2, 1210, __pyx_L1_error))
 
 
-  /* "View.MemoryView":1251
+  /* "View.MemoryView":1253
  * 
  * @cname('__pyx_memoryview_err_extents')
  * cdef int _err_extents(int i, Py_ssize_t extent1,             # <<<<<<<<<<<<<<
  *                              Py_ssize_t extent2) except -1 with gil:
  *     raise ValueError("got differing extents in dimension %d (got %d and %d)" %
  */
-  __Pyx_TraceLine(1251,0,__PYX_ERR(2, 1251, __pyx_L1_error))
+  __Pyx_TraceLine(1253,0,__PYX_ERR(2, 1253, __pyx_L1_error))
 
 
-  /* "View.MemoryView":1257
+  /* "View.MemoryView":1259
  * 
  * @cname('__pyx_memoryview_err_dim')
  * cdef int _err_dim(object error, char *msg, int dim) except -1 with gil:             # <<<<<<<<<<<<<<
  *     raise error(msg.decode('ascii') % dim)
  * 
  */
-  __Pyx_TraceLine(1257,0,__PYX_ERR(2, 1257, __pyx_L1_error))
+  __Pyx_TraceLine(1259,0,__PYX_ERR(2, 1259, __pyx_L1_error))
 
 
-  /* "View.MemoryView":1261
+  /* "View.MemoryView":1263
  * 
  * @cname('__pyx_memoryview_err')
  * cdef int _err(object error, char *msg) except -1 with gil:             # <<<<<<<<<<<<<<
  *     if msg != NULL:
  *         raise error(msg.decode('ascii'))
  */
-  __Pyx_TraceLine(1261,0,__PYX_ERR(2, 1261, __pyx_L1_error))
+  __Pyx_TraceLine(1263,0,__PYX_ERR(2, 1263, __pyx_L1_error))
 
 
-  /* "View.MemoryView":1268
+  /* "View.MemoryView":1270
  * 
  * @cname('__pyx_memoryview_copy_contents')
  * cdef int memoryview_copy_contents(__Pyx_memviewslice src,             # <<<<<<<<<<<<<<
  *                                   __Pyx_memviewslice dst,
  *                                   int src_ndim, int dst_ndim,
  */
-  __Pyx_TraceLine(1268,0,__PYX_ERR(2, 1268, __pyx_L1_error))
+  __Pyx_TraceLine(1270,0,__PYX_ERR(2, 1270, __pyx_L1_error))
 
 
-  /* "View.MemoryView":1340
+  /* "View.MemoryView":1342
  * 
  * @cname('__pyx_memoryview_broadcast_leading')
  * cdef void broadcast_leading(__Pyx_memviewslice *mslice,             # <<<<<<<<<<<<<<
  *                             int ndim,
  *                             int ndim_other) nogil:
  */
-  __Pyx_TraceLine(1340,0,__PYX_ERR(2, 1340, __pyx_L1_error))
+  __Pyx_TraceLine(1342,0,__PYX_ERR(2, 1342, __pyx_L1_error))
 
 
-  /* "View.MemoryView":1362
+  /* "View.MemoryView":1364
  * 
  * @cname('__pyx_memoryview_refcount_copying')
  * cdef void refcount_copying(__Pyx_memviewslice *dst, bint dtype_is_object,             # <<<<<<<<<<<<<<
  *                            int ndim, bint inc) nogil:
  * 
  */
-  __Pyx_TraceLine(1362,0,__PYX_ERR(2, 1362, __pyx_L1_error))
+  __Pyx_TraceLine(1364,0,__PYX_ERR(2, 1364, __pyx_L1_error))
 
 
-  /* "View.MemoryView":1371
+  /* "View.MemoryView":1373
  * 
  * @cname('__pyx_memoryview_refcount_objects_in_slice_with_gil')
  * cdef void refcount_objects_in_slice_with_gil(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                                              Py_ssize_t *strides, int ndim,
  *                                              bint inc) with gil:
  */
-  __Pyx_TraceLine(1371,0,__PYX_ERR(2, 1371, __pyx_L1_error))
+  __Pyx_TraceLine(1373,0,__PYX_ERR(2, 1373, __pyx_L1_error))
 
 
-  /* "View.MemoryView":1377
+  /* "View.MemoryView":1379
  * 
  * @cname('__pyx_memoryview_refcount_objects_in_slice')
  * cdef void refcount_objects_in_slice(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                                     Py_ssize_t *strides, int ndim, bint inc):
  *     cdef Py_ssize_t i
  */
-  __Pyx_TraceLine(1377,0,__PYX_ERR(2, 1377, __pyx_L1_error))
+  __Pyx_TraceLine(1379,0,__PYX_ERR(2, 1379, __pyx_L1_error))
 
 
-  /* "View.MemoryView":1397
+  /* "View.MemoryView":1399
  * 
  * @cname('__pyx_memoryview_slice_assign_scalar')
  * cdef void slice_assign_scalar(__Pyx_memviewslice *dst, int ndim,             # <<<<<<<<<<<<<<
  *                               size_t itemsize, void *item,
  *                               bint dtype_is_object) nogil:
  */
-  __Pyx_TraceLine(1397,0,__PYX_ERR(2, 1397, __pyx_L1_error))
+  __Pyx_TraceLine(1399,0,__PYX_ERR(2, 1399, __pyx_L1_error))
 
 
-  /* "View.MemoryView":1407
+  /* "View.MemoryView":1409
  * 
  * @cname('__pyx_memoryview__slice_assign_scalar')
  * cdef void _slice_assign_scalar(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                               Py_ssize_t *strides, int ndim,
  *                               size_t itemsize, void *item) nogil:
  */
-  __Pyx_TraceLine(1407,0,__PYX_ERR(2, 1407, __pyx_L1_error))
+  __Pyx_TraceLine(1409,0,__PYX_ERR(2, 1409, __pyx_L1_error))
 
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_Enum(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
@@ -34067,25 +34314,23 @@
 #if PY_VERSION_HEX < 0x030400B1
     } else {
         (*frame)->f_tstate = tstate;
 #endif
     }
     __Pyx_PyFrame_SetLineNumber(*frame, firstlineno);
     retval = 1;
-    tstate->tracing++;
-    __Pyx_SetTracing(tstate, 0);
+    __Pyx_EnterTracing(tstate);
     __Pyx_ErrFetchInState(tstate, &type, &value, &traceback);
     #if CYTHON_TRACE
     if (tstate->c_tracefunc)
         retval = tstate->c_tracefunc(tstate->c_traceobj, *frame, PyTrace_CALL, NULL) == 0;
     if (retval && tstate->c_profilefunc)
     #endif
         retval = tstate->c_profilefunc(tstate->c_profileobj, *frame, PyTrace_CALL, NULL) == 0;
-    __Pyx_SetTracing(tstate, (tstate->c_profilefunc || (CYTHON_TRACE && tstate->c_tracefunc)));
-    tstate->tracing--;
+    __Pyx_LeaveTracing(tstate);
     if (retval) {
         __Pyx_ErrRestoreInState(tstate, type, value, traceback);
         return __Pyx_IsTracing(tstate, 0, 0) && retval;
     } else {
         Py_XDECREF(type);
         Py_XDECREF(value);
         Py_XDECREF(traceback);
@@ -34542,15 +34787,15 @@
 #endif
     return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
 }
 
 /* ObjectGetItem */
 #if CYTHON_USE_TYPE_SLOTS
 static PyObject *__Pyx_PyObject_GetIndex(PyObject *obj, PyObject* index) {
-    PyObject *runerr;
+    PyObject *runerr = NULL;
     Py_ssize_t key_value;
     PySequenceMethods *m = Py_TYPE(obj)->tp_as_sequence;
     if (unlikely(!(m && m->sq_item))) {
         PyErr_Format(PyExc_TypeError, "'%.200s' object is not subscriptable", Py_TYPE(obj)->tp_name);
         return NULL;
     }
     key_value = __Pyx_PyIndex_AsSsize_t(index);
@@ -34638,15 +34883,15 @@
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
 #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(func)) {
         return __Pyx_PyFunction_FastCall(func, NULL, 0);
     }
 #endif
-#ifdef __Pyx_CyFunction_USED
+#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
     if (likely(PyCFunction_Check(func) || __Pyx_CyFunction_Check(func)))
 #else
     if (likely(PyCFunction_Check(func)))
 #endif
     {
         if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
             return __Pyx_PyObject_CallMethO(func, NULL);
@@ -35090,28 +35335,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -35123,17 +35368,15 @@
     PyObject *old_exc, *old_val, *old_tb;
     PyObject *ctx;
     __Pyx_PyThreadState_declare
 #ifdef WITH_THREAD
     PyGILState_STATE state;
     if (nogil)
         state = PyGILState_Ensure();
-#ifdef _MSC_VER
-    else state = (PyGILState_STATE)-1;
-#endif
+    else state = (PyGILState_STATE)0;
 #endif
     __Pyx_PyThreadState_assign
     __Pyx_ErrFetch(&old_exc, &old_val, &old_tb);
     if (full_traceback) {
         Py_XINCREF(old_exc);
         Py_XINCREF(old_val);
         Py_XINCREF(old_tb);
@@ -35257,15 +35500,15 @@
 }
 #ifndef Py_NO_RETURN
 #define Py_NO_RETURN
 #endif
 static void __pyx_fatalerror(const char *fmt, ...) Py_NO_RETURN {
     va_list vargs;
     char msg[200];
-#ifdef HAVE_STDARG_PROTOTYPES
+#if PY_VERSION_HEX >= 0x030A0000 || defined(HAVE_STDARG_PROTOTYPES)
     va_start(vargs, fmt);
 #else
     va_start(vargs);
 #endif
     vsnprintf(msg, 200, fmt, vargs);
     va_end(vargs);
     Py_FatalError(msg);
@@ -35620,15 +35863,15 @@
         ps2 = PyBytes_AS_STRING(s2);
         if (ps1[0] != ps2[0]) {
             return (equals == Py_NE);
         } else if (length == 1) {
             return (equals == Py_EQ);
         } else {
             int result;
-#if CYTHON_USE_UNICODE_INTERNALS
+#if CYTHON_USE_UNICODE_INTERNALS && (PY_VERSION_HEX < 0x030B0000)
             Py_hash_t hash1, hash2;
             hash1 = ((PyBytesObject*)s1)->ob_shash;
             hash2 = ((PyBytesObject*)s2)->ob_shash;
             if (hash1 != hash2 && hash1 != -1 && hash2 != -1) {
                 return (equals == Py_NE);
             }
 #endif
@@ -36129,44 +36372,62 @@
 }
 #endif
 
 /* TypeImport */
 #ifndef __PYX_HAVE_RT_ImportType
 #define __PYX_HAVE_RT_ImportType
 static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
     if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
@@ -36266,25 +36527,43 @@
   }
   Py_XDECREF(name_attr);
   return ret;
 }
 static int __Pyx_setup_reduce(PyObject* type_obj) {
     int ret = 0;
     PyObject *object_reduce = NULL;
+    PyObject *object_getstate = NULL;
     PyObject *object_reduce_ex = NULL;
     PyObject *reduce = NULL;
     PyObject *reduce_ex = NULL;
     PyObject *reduce_cython = NULL;
     PyObject *setstate = NULL;
     PyObject *setstate_cython = NULL;
+    PyObject *getstate = NULL;
+#if CYTHON_USE_PYTYPE_LOOKUP
+    getstate = _PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate);
+#else
+    getstate = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_getstate);
+    if (!getstate && PyErr_Occurred()) {
+        goto __PYX_BAD;
+    }
+#endif
+    if (getstate) {
 #if CYTHON_USE_PYTYPE_LOOKUP
-    if (_PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate)) goto __PYX_GOOD;
+        object_getstate = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_getstate);
 #else
-    if (PyObject_HasAttr(type_obj, __pyx_n_s_getstate)) goto __PYX_GOOD;
+        object_getstate = __Pyx_PyObject_GetAttrStrNoError((PyObject*)&PyBaseObject_Type, __pyx_n_s_getstate);
+        if (!object_getstate && PyErr_Occurred()) {
+            goto __PYX_BAD;
+        }
 #endif
+        if (object_getstate != getstate) {
+            goto __PYX_GOOD;
+        }
+    }
 #if CYTHON_USE_PYTYPE_LOOKUP
     object_reduce_ex = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
 #else
     object_reduce_ex = __Pyx_PyObject_GetAttrStr((PyObject*)&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
 #endif
     reduce_ex = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce_ex); if (unlikely(!reduce_ex)) goto __PYX_BAD;
     if (reduce_ex == object_reduce_ex) {
@@ -36321,14 +36600,16 @@
     if (!PyErr_Occurred())
         PyErr_Format(PyExc_RuntimeError, "Unable to initialize pickling for %s", ((PyTypeObject*)type_obj)->tp_name);
     ret = -1;
 __PYX_GOOD:
 #if !CYTHON_USE_PYTYPE_LOOKUP
     Py_XDECREF(object_reduce);
     Py_XDECREF(object_reduce_ex);
+    Py_XDECREF(object_getstate);
+    Py_XDECREF(getstate);
 #endif
     Py_XDECREF(reduce);
     Py_XDECREF(reduce_ex);
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
@@ -36438,15 +36719,15 @@
     }
     Py_XDECREF(owned_metaclass);
     return result;
 }
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -36468,15 +36749,15 @@
       } else {
         PyErr_Clear();
         use_cline = NULL;
       }
     }
     if (!use_cline) {
         c_line = 0;
-        PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
+        (void) PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
     }
     else if (use_cline == Py_False || (use_cline != Py_True && PyObject_Not(use_cline) != 0)) {
         c_line = 0;
     }
     __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
     return c_line;
 }
@@ -36562,41 +36843,48 @@
     Py_INCREF(code_object);
 }
 
 /* AddTraceback */
 #include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
 static PyCodeObject* __Pyx_CreateCodeObjectForTraceback(
             const char *funcname, int c_line,
             int py_line, const char *filename) {
-    PyCodeObject *py_code = 0;
-    PyObject *py_srcfile = 0;
-    PyObject *py_funcname = 0;
+    PyCodeObject *py_code = NULL;
+    PyObject *py_funcname = NULL;
     #if PY_MAJOR_VERSION < 3
+    PyObject *py_srcfile = NULL;
     py_srcfile = PyString_FromString(filename);
-    #else
-    py_srcfile = PyUnicode_FromString(filename);
-    #endif
     if (!py_srcfile) goto bad;
+    #endif
     if (c_line) {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
+        if (!py_funcname) goto bad;
         #else
         py_funcname = PyUnicode_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
+        if (!py_funcname) goto bad;
+        funcname = PyUnicode_AsUTF8(py_funcname);
+        if (!funcname) goto bad;
         #endif
     }
     else {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromString(funcname);
-        #else
-        py_funcname = PyUnicode_FromString(funcname);
+        if (!py_funcname) goto bad;
         #endif
     }
-    if (!py_funcname) goto bad;
+    #if PY_MAJOR_VERSION < 3
     py_code = __Pyx_PyCode_New(
         0,
         0,
         0,
         0,
         0,
         __pyx_empty_bytes, /*PyObject *code,*/
@@ -36607,34 +36895,49 @@
         __pyx_empty_tuple, /*PyObject *cellvars,*/
         py_srcfile,   /*PyObject *filename,*/
         py_funcname,  /*PyObject *name,*/
         py_line,
         __pyx_empty_bytes  /*PyObject *lnotab*/
     );
     Py_DECREF(py_srcfile);
-    Py_DECREF(py_funcname);
+    #else
+    py_code = PyCode_NewEmpty(filename, funcname, py_line);
+    #endif
+    Py_XDECREF(py_funcname);  // XDECREF since it's only set on Py3 if cline
     return py_code;
 bad:
-    Py_XDECREF(py_srcfile);
     Py_XDECREF(py_funcname);
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(py_srcfile);
+    #endif
     return NULL;
 }
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
     PyCodeObject *py_code = 0;
     PyFrameObject *py_frame = 0;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
+    PyObject *ptype, *pvalue, *ptraceback;
     if (c_line) {
         c_line = __Pyx_CLineForTraceback(tstate, c_line);
     }
     py_code = __pyx_find_code_object(c_line ? -c_line : py_line);
     if (!py_code) {
+        __Pyx_ErrFetchInState(tstate, &ptype, &pvalue, &ptraceback);
         py_code = __Pyx_CreateCodeObjectForTraceback(
             funcname, c_line, py_line, filename);
-        if (!py_code) goto bad;
+        if (!py_code) {
+            /* If the code object creation fails, then we should clear the
+               fetched exception references and propagate the new exception */
+            Py_XDECREF(ptype);
+            Py_XDECREF(pvalue);
+            Py_XDECREF(ptraceback);
+            goto bad;
+        }
+        __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
         __pyx_insert_code_object(c_line ? -c_line : py_line, py_code);
     }
     py_frame = PyFrame_New(
         tstate,            /*PyThreadState *tstate,*/
         py_code,           /*PyCodeObject *code,*/
         __pyx_d,    /*PyObject *globals,*/
         0                  /*PyObject *locals*/
@@ -37831,15 +38134,15 @@
                         z = __Pyx_c_prod_float(a, a);
                         return __Pyx_c_prod_float(z, z);
                 }
             }
             if (a.imag == 0) {
                 if (a.real == 0) {
                     return a;
-                } else if (b.imag == 0) {
+                } else if ((b.imag == 0) && (a.real >= 0)) {
                     z.real = powf(a.real, b.real);
                     z.imag = 0;
                     return z;
                 } else if (a.real > 0) {
                     r = a.real;
                     theta = 0;
                 } else {
@@ -37985,15 +38288,15 @@
                         z = __Pyx_c_prod_double(a, a);
                         return __Pyx_c_prod_double(z, z);
                 }
             }
             if (a.imag == 0) {
                 if (a.real == 0) {
                     return a;
-                } else if (b.imag == 0) {
+                } else if ((b.imag == 0) && (a.real >= 0)) {
                     z.real = pow(a.real, b.real);
                     z.imag = 0;
                     return z;
                 } else if (a.real > 0) {
                     r = a.real;
                     theta = 0;
                 } else {
@@ -39249,19 +39552,41 @@
         return _PyLong_FromByteArray(bytes, sizeof(long),
                                      little, !is_unsigned);
     }
 }
 
 /* CheckBinaryVersion */
   static int __Pyx_check_binary_version(void) {
-    char ctversion[4], rtversion[4];
-    PyOS_snprintf(ctversion, 4, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    PyOS_snprintf(rtversion, 4, "%s", Py_GetVersion());
-    if (ctversion[0] != rtversion[0] || ctversion[2] != rtversion[2]) {
+    char ctversion[5];
+    int same=1, i, found_dot;
+    const char* rt_from_call = Py_GetVersion();
+    PyOS_snprintf(ctversion, 5, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
+    found_dot = 0;
+    for (i = 0; i < 4; i++) {
+        if (!ctversion[i]) {
+            same = (rt_from_call[i] < '0' || rt_from_call[i] > '9');
+            break;
+        }
+        if (rt_from_call[i] != ctversion[i]) {
+            same = 0;
+            break;
+        }
+    }
+    if (!same) {
+        char rtversion[5] = {'\0'};
         char message[200];
+        for (i=0; i<4; ++i) {
+            if (rt_from_call[i] == '.') {
+                if (found_dot) break;
+                found_dot = 1;
+            } else if (rt_from_call[i] < '0' || rt_from_call[i] > '9') {
+                break;
+            }
+            rtversion[i] = rt_from_call[i];
+        }
         PyOS_snprintf(message, sizeof(message),
                       "compiletime version %s of module '%.100s' "
                       "does not match runtime version %s",
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
@@ -39511,14 +39836,31 @@
   }
   x = PyNumber_Index(b);
   if (!x) return -1;
   ival = PyInt_AsSsize_t(x);
   Py_DECREF(x);
   return ival;
 }
+static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject* o) {
+  if (sizeof(Py_hash_t) == sizeof(Py_ssize_t)) {
+    return (Py_hash_t) __Pyx_PyIndex_AsSsize_t(o);
+#if PY_MAJOR_VERSION < 3
+  } else if (likely(PyInt_CheckExact(o))) {
+    return PyInt_AS_LONG(o);
+#endif
+  } else {
+    Py_ssize_t ival;
+    PyObject *x;
+    x = PyNumber_Index(o);
+    if (!x) return -1;
+    ival = PyInt_AsLong(x);
+    Py_DECREF(x);
+    return ival;
+  }
+}
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b) {
   return b ? __Pyx_NewRef(Py_True) : __Pyx_NewRef(Py_False);
 }
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t ival) {
     return PyInt_FromSize_t(ival);
 }
```

### Comparing `wiver-1.8.2/src/wiver/wiver_cython.pxd` & `wiver-1.9.0/src/wiver/wiver_cython.pxd`

 * *Files identical despite different names*

### Comparing `wiver-1.8.2/src/wiver/wiver_cython.pyx` & `wiver-1.9.0/src/wiver/wiver_cython.pyx`

 * *Files identical despite different names*

### Comparing `wiver-1.8.2/src/wiver/wiver_python.py` & `wiver-1.9.0/src/wiver/wiver_python.py`

 * *Files identical despite different names*

### Comparing `wiver-1.8.2/src/wiver.egg-info/SOURCES.txt` & `wiver-1.9.0/src/wiver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

