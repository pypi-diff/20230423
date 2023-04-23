# Comparing `tmp/tarina-0.3.0.tar.gz` & `tmp/tarina-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarina-0.3.0.tar", last modified: Mon Apr 17 05:31:24 2023, max compression
+gzip compressed data, was "tarina-0.3.1.tar", last modified: Sun Apr 23 14:34:17 2023, max compression
```

## Comparing `tarina-0.3.0.tar` & `tarina-0.3.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:31:24.729679 tarina-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-17 05:31:07.000000 tarina-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-17 05:31:07.000000 tarina-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-17 05:31:24.729679 tarina-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-17 05:31:07.000000 tarina-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-17 05:31:07.000000 tarina-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 05:31:24.729679 tarina-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-17 05:31:07.000000 tarina-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:31:24.725679 tarina-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:31:24.729679 tarina-0.3.0/src/tarina/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-17 05:31:07.000000 tarina-0.3.0/src/tarina/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23066 2023-04-17 05:31:07.000000 tarina-0.3.0/src/tarina/_lru_c.c
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-17 05:31:07.000000 tarina-0.3.0/src/tarina/_lru_c.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-04-17 05:31:07.000000 tarina-0.3.0/src/tarina/_lru_py.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-04-17 05:31:07.000000 tarina-0.3.0/src/tarina/_op.h
--rw-r--r--   0 runner    (1001) docker     (123)   200403 2023-04-17 05:31:16.000000 tarina-0.3.0/src/tarina/_string_c.c
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-17 05:31:07.000000 tarina-0.3.0/src/tarina/_string_c.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-04-17 05:31:07.000000 tarina-0.3.0/src/tarina/_string_c.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-17 05:31:07.000000 tarina-0.3.0/src/tarina/_string_py.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-17 05:31:07.000000 tarina-0.3.0/src/tarina/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-17 05:31:07.000000 tarina-0.3.0/src/tarina/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-04-17 05:31:07.000000 tarina-0.3.0/src/tarina/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-17 05:31:07.000000 tarina-0.3.0/src/tarina/guard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:31:24.729679 tarina-0.3.0/src/tarina/i18n/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-17 05:31:07.000000 tarina-0.3.0/src/tarina/i18n/.config.json
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-17 05:31:07.000000 tarina-0.3.0/src/tarina/i18n/en-US.json
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-17 05:31:07.000000 tarina-0.3.0/src/tarina/i18n/zh-CN.json
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-04-17 05:31:07.000000 tarina-0.3.0/src/tarina/lang.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-17 05:31:07.000000 tarina-0.3.0/src/tarina/lru.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-17 05:31:07.000000 tarina-0.3.0/src/tarina/lru.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-17 05:31:07.000000 tarina-0.3.0/src/tarina/signature.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-17 05:31:07.000000 tarina-0.3.0/src/tarina/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-17 05:31:07.000000 tarina-0.3.0/src/tarina/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:31:24.729679 tarina-0.3.0/src/tarina.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-17 05:31:24.000000 tarina-0.3.0/src/tarina.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-17 05:31:24.000000 tarina-0.3.0/src/tarina.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 05:31:24.000000 tarina-0.3.0/src/tarina.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-17 05:31:24.000000 tarina-0.3.0/src/tarina.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-17 05:31:24.000000 tarina-0.3.0/src/tarina.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:34:17.126438 tarina-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-23 14:33:58.000000 tarina-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-23 14:33:58.000000 tarina-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-23 14:34:17.126438 tarina-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-23 14:33:58.000000 tarina-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-23 14:33:58.000000 tarina-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 14:34:17.126438 tarina-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-23 14:33:58.000000 tarina-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:34:17.122438 tarina-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:34:17.126438 tarina-0.3.1/src/tarina/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-23 14:33:58.000000 tarina-0.3.1/src/tarina/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23066 2023-04-23 14:33:58.000000 tarina-0.3.1/src/tarina/_lru_c.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-23 14:33:58.000000 tarina-0.3.1/src/tarina/_lru_c.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-04-23 14:33:58.000000 tarina-0.3.1/src/tarina/_lru_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-04-23 14:33:58.000000 tarina-0.3.1/src/tarina/_op.h
+-rw-r--r--   0 runner    (1001) docker     (123)   193906 2023-04-23 14:34:08.000000 tarina-0.3.1/src/tarina/_string_c.c
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-23 14:33:58.000000 tarina-0.3.1/src/tarina/_string_c.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-04-23 14:33:58.000000 tarina-0.3.1/src/tarina/_string_c.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-23 14:33:58.000000 tarina-0.3.1/src/tarina/_string_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-23 14:33:58.000000 tarina-0.3.1/src/tarina/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-23 14:33:58.000000 tarina-0.3.1/src/tarina/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-04-23 14:33:58.000000 tarina-0.3.1/src/tarina/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-23 14:33:58.000000 tarina-0.3.1/src/tarina/guard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:34:17.126438 tarina-0.3.1/src/tarina/i18n/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-23 14:33:58.000000 tarina-0.3.1/src/tarina/i18n/.config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-23 14:33:58.000000 tarina-0.3.1/src/tarina/i18n/en-US.json
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-23 14:33:58.000000 tarina-0.3.1/src/tarina/i18n/zh-CN.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-04-23 14:33:58.000000 tarina-0.3.1/src/tarina/lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-23 14:33:58.000000 tarina-0.3.1/src/tarina/lru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-23 14:33:58.000000 tarina-0.3.1/src/tarina/lru.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-23 14:33:58.000000 tarina-0.3.1/src/tarina/signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-23 14:33:58.000000 tarina-0.3.1/src/tarina/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-23 14:33:58.000000 tarina-0.3.1/src/tarina/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:34:17.126438 tarina-0.3.1/src/tarina.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-23 14:34:17.000000 tarina-0.3.1/src/tarina.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-23 14:34:17.000000 tarina-0.3.1/src/tarina.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 14:34:17.000000 tarina-0.3.1/src/tarina.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-23 14:34:17.000000 tarina-0.3.1/src/tarina.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-23 14:34:17.000000 tarina-0.3.1/src/tarina.egg-info/top_level.txt
```

### Comparing `tarina-0.3.0/LICENSE` & `tarina-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tarina-0.3.0/PKG-INFO` & `tarina-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tarina
-Version: 0.3.0
+Version: 0.3.1
 Summary: A collection of common utils for Arclet
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `tarina-0.3.0/pyproject.toml` & `tarina-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tarina"
-version = "0.3.0"
+version = "0.3.1"
 description = "A collection of common utils for Arclet"
 authors = [
     {name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com"},
 ]
 dependencies = [
     "typing-extensions>=4.4.0",
 ]
```

### Comparing `tarina-0.3.0/setup.py` & `tarina-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `tarina-0.3.0/src/tarina/_lru_c.c` & `tarina-0.3.1/src/tarina/_lru_c.c`

 * *Files identical despite different names*

### Comparing `tarina-0.3.0/src/tarina/_lru_c.pyi` & `tarina-0.3.1/src/tarina/_lru_c.pyi`

 * *Files identical despite different names*

### Comparing `tarina-0.3.0/src/tarina/_lru_py.py` & `tarina-0.3.1/src/tarina/_lru_py.py`

 * *Files identical despite different names*

### Comparing `tarina-0.3.0/src/tarina/_op.h` & `tarina-0.3.1/src/tarina/_op.h`

 * *Files 12% similar despite different names*

```diff
@@ -5,21 +5,41 @@
 #ifndef LINEAR_PROBES
 #define LINEAR_PROBES 9
 #endif
 
 /* This must be >= 1 */
 #define PERTURB_SHIFT 5
 
+static inline Py_ssize_t tuplesize(PyObject *ob) {
+    PyVarObject *var_ob = (PyVarObject*)ob;
+    return var_ob->ob_size;
+}
 
-static PyObject * tupleitem(PyObject *a, Py_ssize_t i)
+static inline PyObject * tupleitem(PyObject *a, Py_ssize_t i)
 {
-    Py_INCREF(((PyTupleObject*)a)->ob_item[i]);
     return ((PyTupleObject*)a)->ob_item[i];
 }
 
+
+static int contains(PyObject *chs, Py_UCS4 ch) {
+    Py_ssize_t i = 0;
+    Py_ssize_t length = tuplesize(chs);
+    while (1) {
+        if (i >= length) {
+            return 0;
+        }
+        if (ch == PyUnicode_READ_CHAR(tupleitem(chs, i), 0)) {
+            return 1;
+        }
+        i++;
+    }
+    return 0;
+}
+
+
 static setentry *
 set_lookkey(PySetObject *so, PyObject *key, Py_hash_t hash)
 {
     setentry *table;
     setentry *entry;
     size_t perturb = hash;
     size_t mask = so->mask;
```

### Comparing `tarina-0.3.0/src/tarina/_string_c.c` & `tarina-0.3.1/src/tarina/_string_c.c`

 * *Files 1% similar despite different names*

```diff
@@ -1019,64 +1019,14 @@
 #define __Pyx_DECREF_SET(r, v) do {\
         PyObject *tmp = (PyObject *) r;\
         r = v; __Pyx_DECREF(tmp);\
     } while (0)
 #define __Pyx_CLEAR(r)    do { PyObject* tmp = ((PyObject*)(r)); r = NULL; __Pyx_DECREF(tmp);} while(0)
 #define __Pyx_XCLEAR(r)   do { if((r) != NULL) {PyObject* tmp = ((PyObject*)(r)); r = NULL; __Pyx_DECREF(tmp);}} while(0)
 
-/* IncludeStringH.proto */
-#include <string.h>
-
-/* BytesEquals.proto */
-static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals);
-
-/* UnicodeEquals.proto */
-static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals);
-
-/* PyThreadStateGet.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_PyThreadState_declare  PyThreadState *__pyx_tstate;
-#define __Pyx_PyThreadState_assign  __pyx_tstate = __Pyx_PyThreadState_Current;
-#define __Pyx_PyErr_Occurred()  __pyx_tstate->curexc_type
-#else
-#define __Pyx_PyThreadState_declare
-#define __Pyx_PyThreadState_assign
-#define __Pyx_PyErr_Occurred()  PyErr_Occurred()
-#endif
-
-/* PyErrFetchRestore.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_PyErr_Clear() __Pyx_ErrRestore(NULL, NULL, NULL)
-#define __Pyx_ErrRestoreWithState(type, value, tb)  __Pyx_ErrRestoreInState(PyThreadState_GET(), type, value, tb)
-#define __Pyx_ErrFetchWithState(type, value, tb)    __Pyx_ErrFetchInState(PyThreadState_GET(), type, value, tb)
-#define __Pyx_ErrRestore(type, value, tb)  __Pyx_ErrRestoreInState(__pyx_tstate, type, value, tb)
-#define __Pyx_ErrFetch(type, value, tb)    __Pyx_ErrFetchInState(__pyx_tstate, type, value, tb)
-static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
-static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
-#if CYTHON_COMPILING_IN_CPYTHON
-#define __Pyx_PyErr_SetNone(exc) (Py_INCREF(exc), __Pyx_ErrRestore((exc), NULL, NULL))
-#else
-#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
-#endif
-#else
-#define __Pyx_PyErr_Clear() PyErr_Clear()
-#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
-#define __Pyx_ErrRestoreWithState(type, value, tb)  PyErr_Restore(type, value, tb)
-#define __Pyx_ErrFetchWithState(type, value, tb)  PyErr_Fetch(type, value, tb)
-#define __Pyx_ErrRestoreInState(tstate, type, value, tb)  PyErr_Restore(type, value, tb)
-#define __Pyx_ErrFetchInState(tstate, type, value, tb)  PyErr_Fetch(type, value, tb)
-#define __Pyx_ErrRestore(type, value, tb)  PyErr_Restore(type, value, tb)
-#define __Pyx_ErrFetch(type, value, tb)  PyErr_Fetch(type, value, tb)
-#endif
-
-/* WriteUnraisableException.proto */
-static void __Pyx_WriteUnraisable(const char *name, int clineno,
-                                  int lineno, const char *filename,
-                                  int full_traceback, int nogil);
-
 /* RaiseArgTupleInvalid.proto */
 static void __Pyx_RaiseArgtupleInvalid(const char* func_name, int exact,
     Py_ssize_t num_min, Py_ssize_t num_max, Py_ssize_t num_found);
 
 /* RaiseDoubleKeywords.proto */
 static void __Pyx_RaiseDoubleKeywordsError(const char* func_name, PyObject* kw_name);
 
@@ -1109,14 +1059,23 @@
     (PyErr_SetString(PyExc_IndexError, "tuple index out of range"), (PyObject*)NULL))
 static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
                                                               int wraparound, int boundscheck);
 static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j);
 static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i,
                                                      int is_list, int wraparound, int boundscheck);
 
+/* IncludeStringH.proto */
+#include <string.h>
+
+/* BytesEquals.proto */
+static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals);
+
+/* UnicodeEquals.proto */
+static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals);
+
 /* PyObjectCall.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
 #else
 #define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
 #endif
 
@@ -1201,14 +1160,50 @@
 static CYTHON_INLINE int __Pyx_object_dict_version_matches(PyObject* obj, PY_UINT64_T tp_dict_version, PY_UINT64_T obj_dict_version);
 #else
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
+/* PyThreadStateGet.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_PyThreadState_declare  PyThreadState *__pyx_tstate;
+#define __Pyx_PyThreadState_assign  __pyx_tstate = __Pyx_PyThreadState_Current;
+#define __Pyx_PyErr_Occurred()  __pyx_tstate->curexc_type
+#else
+#define __Pyx_PyThreadState_declare
+#define __Pyx_PyThreadState_assign
+#define __Pyx_PyErr_Occurred()  PyErr_Occurred()
+#endif
+
+/* PyErrFetchRestore.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_PyErr_Clear() __Pyx_ErrRestore(NULL, NULL, NULL)
+#define __Pyx_ErrRestoreWithState(type, value, tb)  __Pyx_ErrRestoreInState(PyThreadState_GET(), type, value, tb)
+#define __Pyx_ErrFetchWithState(type, value, tb)    __Pyx_ErrFetchInState(PyThreadState_GET(), type, value, tb)
+#define __Pyx_ErrRestore(type, value, tb)  __Pyx_ErrRestoreInState(__pyx_tstate, type, value, tb)
+#define __Pyx_ErrFetch(type, value, tb)    __Pyx_ErrFetchInState(__pyx_tstate, type, value, tb)
+static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
+static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+#if CYTHON_COMPILING_IN_CPYTHON
+#define __Pyx_PyErr_SetNone(exc) (Py_INCREF(exc), __Pyx_ErrRestore((exc), NULL, NULL))
+#else
+#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
+#endif
+#else
+#define __Pyx_PyErr_Clear() PyErr_Clear()
+#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
+#define __Pyx_ErrRestoreWithState(type, value, tb)  PyErr_Restore(type, value, tb)
+#define __Pyx_ErrFetchWithState(type, value, tb)  PyErr_Fetch(type, value, tb)
+#define __Pyx_ErrRestoreInState(tstate, type, value, tb)  PyErr_Restore(type, value, tb)
+#define __Pyx_ErrFetchInState(tstate, type, value, tb)  PyErr_Fetch(type, value, tb)
+#define __Pyx_ErrRestore(type, value, tb)  PyErr_Restore(type, value, tb)
+#define __Pyx_ErrFetch(type, value, tb)  PyErr_Fetch(type, value, tb)
+#endif
+
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
 #endif
 
@@ -1236,17 +1231,14 @@
 #define __Pyx_HAS_GCC_DIAGNOSTIC
 #endif
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE char __Pyx_PyInt_As_char(PyObject *);
 
 /* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
-
-/* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_char(char value);
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
@@ -1290,15 +1282,14 @@
 /* Module declarations from 'cpython.unicode' */
 
 /* Module declarations from 'cpython.list' */
 
 /* Module declarations from 'tarina._string_c' */
 static PyObject *__pyx_v_6tarina_9_string_c_QUOTES = 0;
 static PyObject *__pyx_v_6tarina_9_string_c_CRLF = 0;
-static CYTHON_INLINE int __pyx_f_6tarina_9_string_c_contains(PyObject *, Py_UCS4); /*proto*/
 #define __Pyx_MODULE_NAME "tarina._string_c"
 extern int __pyx_module_is_main_tarina___string_c;
 int __pyx_module_is_main_tarina___string_c = 0;
 
 /* Implementation of 'tarina._string_c' */
 static const char __pyx_k_[] = "\001";
 static const char __pyx_k_i[] = "i";
@@ -1359,136 +1350,15 @@
 static __Pyx_CachedCFunction __pyx_umethod_PyUnicode_Type_lstrip = {0, &__pyx_n_s_lstrip, 0, 0, 0};
 static PyObject *__pyx_tuple__7;
 static PyObject *__pyx_tuple__9;
 static PyObject *__pyx_codeobj__8;
 static PyObject *__pyx_codeobj__10;
 /* Late includes */
 
-/* "tarina/_string_c.pyx":16
- *     bint set_contains_key(object anyset, object key) except -1
- * 
- * cdef inline int contains(tuple chs, Py_UCS4 ch):             # <<<<<<<<<<<<<<
- *     cdef Py_ssize_t i = 0
- *     cdef Py_ssize_t length = Py_SIZE(chs)
- */
-
-static CYTHON_INLINE int __pyx_f_6tarina_9_string_c_contains(PyObject *__pyx_v_chs, Py_UCS4 __pyx_v_ch) {
-  Py_ssize_t __pyx_v_i;
-  Py_ssize_t __pyx_v_length;
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("contains", 0);
-
-  /* "tarina/_string_c.pyx":17
- * 
- * cdef inline int contains(tuple chs, Py_UCS4 ch):
- *     cdef Py_ssize_t i = 0             # <<<<<<<<<<<<<<
- *     cdef Py_ssize_t length = Py_SIZE(chs)
- *     while i < length:
- */
-  __pyx_v_i = 0;
-
-  /* "tarina/_string_c.pyx":18
- * cdef inline int contains(tuple chs, Py_UCS4 ch):
- *     cdef Py_ssize_t i = 0
- *     cdef Py_ssize_t length = Py_SIZE(chs)             # <<<<<<<<<<<<<<
- *     while i < length:
- *         if ch == <object>tupleitem(chs, i):
- */
-  __pyx_v_length = Py_SIZE(__pyx_v_chs);
-
-  /* "tarina/_string_c.pyx":19
- *     cdef Py_ssize_t i = 0
- *     cdef Py_ssize_t length = Py_SIZE(chs)
- *     while i < length:             # <<<<<<<<<<<<<<
- *         if ch == <object>tupleitem(chs, i):
- *             return 1
- */
-  while (1) {
-    __pyx_t_1 = ((__pyx_v_i < __pyx_v_length) != 0);
-    if (!__pyx_t_1) break;
-
-    /* "tarina/_string_c.pyx":20
- *     cdef Py_ssize_t length = Py_SIZE(chs)
- *     while i < length:
- *         if ch == <object>tupleitem(chs, i):             # <<<<<<<<<<<<<<
- *             return 1
- *         i += 1
- */
-    __pyx_t_2 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 20, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = tupleitem(__pyx_v_chs, __pyx_v_i);
-    __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_t_2, ((PyObject *)__pyx_t_3), Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 20, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (__pyx_t_1) {
-
-      /* "tarina/_string_c.pyx":21
- *     while i < length:
- *         if ch == <object>tupleitem(chs, i):
- *             return 1             # <<<<<<<<<<<<<<
- *         i += 1
- *     return 0
- */
-      __pyx_r = 1;
-      goto __pyx_L0;
-
-      /* "tarina/_string_c.pyx":20
- *     cdef Py_ssize_t length = Py_SIZE(chs)
- *     while i < length:
- *         if ch == <object>tupleitem(chs, i):             # <<<<<<<<<<<<<<
- *             return 1
- *         i += 1
- */
-    }
-
-    /* "tarina/_string_c.pyx":22
- *         if ch == <object>tupleitem(chs, i):
- *             return 1
- *         i += 1             # <<<<<<<<<<<<<<
- *     return 0
- * 
- */
-    __pyx_v_i = (__pyx_v_i + 1);
-  }
-
-  /* "tarina/_string_c.pyx":23
- *             return 1
- *         i += 1
- *     return 0             # <<<<<<<<<<<<<<
- * 
- * cdef set QUOTES = {'"', '\''}
- */
-  __pyx_r = 0;
-  goto __pyx_L0;
-
-  /* "tarina/_string_c.pyx":16
- *     bint set_contains_key(object anyset, object key) except -1
- * 
- * cdef inline int contains(tuple chs, Py_UCS4 ch):             # <<<<<<<<<<<<<<
- *     cdef Py_ssize_t i = 0
- *     cdef Py_ssize_t length = Py_SIZE(chs)
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_WriteUnraisable("tarina._string_c.contains", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "tarina/_string_c.pyx":28
+/* "tarina/_string_c.pyx":19
  * cdef set CRLF = {'\r', '\n'}
  * 
  * def split(str text, tuple separates, char crlf=True):             # <<<<<<<<<<<<<<
  *     """
  * 
  */
 
@@ -1527,54 +1397,54 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_text)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_separates)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("split", 0, 2, 3, 1); __PYX_ERR(0, 28, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("split", 0, 2, 3, 1); __PYX_ERR(0, 19, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_crlf);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "split") < 0)) __PYX_ERR(0, 28, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "split") < 0)) __PYX_ERR(0, 19, __pyx_L3_error)
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
     __pyx_v_text = ((PyObject*)values[0]);
     __pyx_v_separates = ((PyObject*)values[1]);
     if (values[2]) {
-      __pyx_v_crlf = __Pyx_PyInt_As_char(values[2]); if (unlikely((__pyx_v_crlf == (char)-1) && PyErr_Occurred())) __PYX_ERR(0, 28, __pyx_L3_error)
+      __pyx_v_crlf = __Pyx_PyInt_As_char(values[2]); if (unlikely((__pyx_v_crlf == (char)-1) && PyErr_Occurred())) __PYX_ERR(0, 19, __pyx_L3_error)
     } else {
       __pyx_v_crlf = ((char)1);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("split", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 28, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("split", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 19, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("tarina._string_c.split", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_text), (&PyUnicode_Type), 1, "text", 1))) __PYX_ERR(0, 28, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_separates), (&PyTuple_Type), 1, "separates", 1))) __PYX_ERR(0, 28, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_text), (&PyUnicode_Type), 1, "text", 1))) __PYX_ERR(0, 19, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_separates), (&PyTuple_Type), 1, "separates", 1))) __PYX_ERR(0, 19, __pyx_L1_error)
   __pyx_r = __pyx_pf_6tarina_9_string_c_split(__pyx_self, __pyx_v_text, __pyx_v_separates, __pyx_v_crlf);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -1598,444 +1468,444 @@
   int __pyx_t_5;
   int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("split", 0);
 
-  /* "tarina/_string_c.pyx":39
+  /* "tarina/_string_c.pyx":30
  *         List[str]: ,
  *     """
  *     cdef char escape = 0             # <<<<<<<<<<<<<<
  *     cdef list result = []
  *     cdef Py_UCS4 quotation = 0
  */
   __pyx_v_escape = 0;
 
-  /* "tarina/_string_c.pyx":40
+  /* "tarina/_string_c.pyx":31
  *     """
  *     cdef char escape = 0
  *     cdef list result = []             # <<<<<<<<<<<<<<
  *     cdef Py_UCS4 quotation = 0
  *     cdef Py_UCS4 ch = 0
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 40, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 31, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_result = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "tarina/_string_c.pyx":41
+  /* "tarina/_string_c.pyx":32
  *     cdef char escape = 0
  *     cdef list result = []
  *     cdef Py_UCS4 quotation = 0             # <<<<<<<<<<<<<<
  *     cdef Py_UCS4 ch = 0
  *     cdef Py_ssize_t i = 0
  */
   __pyx_v_quotation = 0;
 
-  /* "tarina/_string_c.pyx":42
+  /* "tarina/_string_c.pyx":33
  *     cdef list result = []
  *     cdef Py_UCS4 quotation = 0
  *     cdef Py_UCS4 ch = 0             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t i = 0
  *     cdef Py_ssize_t length = PyUnicode_GET_LENGTH(text)
  */
   __pyx_v_ch = 0;
 
-  /* "tarina/_string_c.pyx":43
+  /* "tarina/_string_c.pyx":34
  *     cdef Py_UCS4 quotation = 0
  *     cdef Py_UCS4 ch = 0
  *     cdef Py_ssize_t i = 0             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t length = PyUnicode_GET_LENGTH(text)
  * 
  */
   __pyx_v_i = 0;
 
-  /* "tarina/_string_c.pyx":44
+  /* "tarina/_string_c.pyx":35
  *     cdef Py_UCS4 ch = 0
  *     cdef Py_ssize_t i = 0
  *     cdef Py_ssize_t length = PyUnicode_GET_LENGTH(text)             # <<<<<<<<<<<<<<
  * 
  *     while i < length:
  */
   __pyx_v_length = PyUnicode_GET_LENGTH(__pyx_v_text);
 
-  /* "tarina/_string_c.pyx":46
+  /* "tarina/_string_c.pyx":37
  *     cdef Py_ssize_t length = PyUnicode_GET_LENGTH(text)
  * 
  *     while i < length:             # <<<<<<<<<<<<<<
  *         ch = PyUnicode_READ_CHAR(text, i)
  *         i += 1
  */
   while (1) {
     __pyx_t_2 = ((__pyx_v_i < __pyx_v_length) != 0);
     if (!__pyx_t_2) break;
 
-    /* "tarina/_string_c.pyx":47
+    /* "tarina/_string_c.pyx":38
  * 
  *     while i < length:
  *         ch = PyUnicode_READ_CHAR(text, i)             # <<<<<<<<<<<<<<
  *         i += 1
  *         if ch == 92:  # \\
  */
     __pyx_v_ch = PyUnicode_READ_CHAR(__pyx_v_text, __pyx_v_i);
 
-    /* "tarina/_string_c.pyx":48
+    /* "tarina/_string_c.pyx":39
  *     while i < length:
  *         ch = PyUnicode_READ_CHAR(text, i)
  *         i += 1             # <<<<<<<<<<<<<<
  *         if ch == 92:  # \\
  *             escape = 1
  */
     __pyx_v_i = (__pyx_v_i + 1);
 
-    /* "tarina/_string_c.pyx":49
+    /* "tarina/_string_c.pyx":40
  *         ch = PyUnicode_READ_CHAR(text, i)
  *         i += 1
  *         if ch == 92:  # \\             # <<<<<<<<<<<<<<
  *             escape = 1
  *             PyList_Append(result, ch)
  */
     __pyx_t_2 = ((__pyx_v_ch == 92) != 0);
     if (__pyx_t_2) {
 
-      /* "tarina/_string_c.pyx":50
+      /* "tarina/_string_c.pyx":41
  *         i += 1
  *         if ch == 92:  # \\
  *             escape = 1             # <<<<<<<<<<<<<<
  *             PyList_Append(result, ch)
  *         elif set_contains_key(QUOTES, ch):
  */
       __pyx_v_escape = 1;
 
-      /* "tarina/_string_c.pyx":51
+      /* "tarina/_string_c.pyx":42
  *         if ch == 92:  # \\
  *             escape = 1
  *             PyList_Append(result, ch)             # <<<<<<<<<<<<<<
  *         elif set_contains_key(QUOTES, ch):
  *             if quotation == 0:
  */
-      __pyx_t_1 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 51, __pyx_L1_error)
+      __pyx_t_1 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 42, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_3 = PyList_Append(__pyx_v_result, __pyx_t_1); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 51, __pyx_L1_error)
+      __pyx_t_3 = PyList_Append(__pyx_v_result, __pyx_t_1); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 42, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "tarina/_string_c.pyx":49
+      /* "tarina/_string_c.pyx":40
  *         ch = PyUnicode_READ_CHAR(text, i)
  *         i += 1
  *         if ch == 92:  # \\             # <<<<<<<<<<<<<<
  *             escape = 1
  *             PyList_Append(result, ch)
  */
       goto __pyx_L5;
     }
 
-    /* "tarina/_string_c.pyx":52
+    /* "tarina/_string_c.pyx":43
  *             escape = 1
  *             PyList_Append(result, ch)
  *         elif set_contains_key(QUOTES, ch):             # <<<<<<<<<<<<<<
  *             if quotation == 0:
  *                 quotation = ch
  */
     __pyx_t_1 = __pyx_v_6tarina_9_string_c_QUOTES;
     __Pyx_INCREF(__pyx_t_1);
-    __pyx_t_4 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 52, __pyx_L1_error)
+    __pyx_t_4 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 43, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_2 = set_contains_key(__pyx_t_1, __pyx_t_4); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 52, __pyx_L1_error)
+    __pyx_t_2 = set_contains_key(__pyx_t_1, __pyx_t_4); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 43, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_5 = (__pyx_t_2 != 0);
     if (__pyx_t_5) {
 
-      /* "tarina/_string_c.pyx":53
+      /* "tarina/_string_c.pyx":44
  *             PyList_Append(result, ch)
  *         elif set_contains_key(QUOTES, ch):
  *             if quotation == 0:             # <<<<<<<<<<<<<<
  *                 quotation = ch
  *             elif ch == quotation:
  */
       __pyx_t_5 = ((__pyx_v_quotation == 0) != 0);
       if (__pyx_t_5) {
 
-        /* "tarina/_string_c.pyx":54
+        /* "tarina/_string_c.pyx":45
  *         elif set_contains_key(QUOTES, ch):
  *             if quotation == 0:
  *                 quotation = ch             # <<<<<<<<<<<<<<
  *             elif ch == quotation:
  *                 quotation = 0
  */
         __pyx_v_quotation = __pyx_v_ch;
 
-        /* "tarina/_string_c.pyx":53
+        /* "tarina/_string_c.pyx":44
  *             PyList_Append(result, ch)
  *         elif set_contains_key(QUOTES, ch):
  *             if quotation == 0:             # <<<<<<<<<<<<<<
  *                 quotation = ch
  *             elif ch == quotation:
  */
         goto __pyx_L6;
       }
 
-      /* "tarina/_string_c.pyx":55
+      /* "tarina/_string_c.pyx":46
  *             if quotation == 0:
  *                 quotation = ch
  *             elif ch == quotation:             # <<<<<<<<<<<<<<
  *                 quotation = 0
  *             else:
  */
       __pyx_t_5 = ((__pyx_v_ch == __pyx_v_quotation) != 0);
       if (__pyx_t_5) {
 
-        /* "tarina/_string_c.pyx":56
+        /* "tarina/_string_c.pyx":47
  *                 quotation = ch
  *             elif ch == quotation:
  *                 quotation = 0             # <<<<<<<<<<<<<<
  *             else:
  *                 PyList_Append(result, ch)
  */
         __pyx_v_quotation = 0;
 
-        /* "tarina/_string_c.pyx":55
+        /* "tarina/_string_c.pyx":46
  *             if quotation == 0:
  *                 quotation = ch
  *             elif ch == quotation:             # <<<<<<<<<<<<<<
  *                 quotation = 0
  *             else:
  */
         goto __pyx_L6;
       }
 
-      /* "tarina/_string_c.pyx":58
+      /* "tarina/_string_c.pyx":49
  *                 quotation = 0
  *             else:
  *                 PyList_Append(result, ch)             # <<<<<<<<<<<<<<
  *                 continue
  *             if escape:
  */
       /*else*/ {
-        __pyx_t_4 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 58, __pyx_L1_error)
+        __pyx_t_4 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 49, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
-        __pyx_t_3 = PyList_Append(__pyx_v_result, __pyx_t_4); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 58, __pyx_L1_error)
+        __pyx_t_3 = PyList_Append(__pyx_v_result, __pyx_t_4); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 49, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-        /* "tarina/_string_c.pyx":59
+        /* "tarina/_string_c.pyx":50
  *             else:
  *                 PyList_Append(result, ch)
  *                 continue             # <<<<<<<<<<<<<<
  *             if escape:
  *                 PyList_SET_ITEM(result, Py_SIZE(result)-1 , ch)
  */
         goto __pyx_L3_continue;
       }
       __pyx_L6:;
 
-      /* "tarina/_string_c.pyx":60
+      /* "tarina/_string_c.pyx":51
  *                 PyList_Append(result, ch)
  *                 continue
  *             if escape:             # <<<<<<<<<<<<<<
  *                 PyList_SET_ITEM(result, Py_SIZE(result)-1 , ch)
  *         elif (quotation == 0 and contains(separates, ch)) or (crlf and set_contains_key(CRLF, ch)):
  */
       __pyx_t_5 = (__pyx_v_escape != 0);
       if (__pyx_t_5) {
 
-        /* "tarina/_string_c.pyx":61
+        /* "tarina/_string_c.pyx":52
  *                 continue
  *             if escape:
  *                 PyList_SET_ITEM(result, Py_SIZE(result)-1 , ch)             # <<<<<<<<<<<<<<
  *         elif (quotation == 0 and contains(separates, ch)) or (crlf and set_contains_key(CRLF, ch)):
  *             if result and result[-1] != '\1':
  */
-        __pyx_t_4 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 61, __pyx_L1_error)
+        __pyx_t_4 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 52, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         PyList_SET_ITEM(__pyx_v_result, (Py_SIZE(__pyx_v_result) - 1), __pyx_t_4);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-        /* "tarina/_string_c.pyx":60
+        /* "tarina/_string_c.pyx":51
  *                 PyList_Append(result, ch)
  *                 continue
  *             if escape:             # <<<<<<<<<<<<<<
  *                 PyList_SET_ITEM(result, Py_SIZE(result)-1 , ch)
  *         elif (quotation == 0 and contains(separates, ch)) or (crlf and set_contains_key(CRLF, ch)):
  */
       }
 
-      /* "tarina/_string_c.pyx":52
+      /* "tarina/_string_c.pyx":43
  *             escape = 1
  *             PyList_Append(result, ch)
  *         elif set_contains_key(QUOTES, ch):             # <<<<<<<<<<<<<<
  *             if quotation == 0:
  *                 quotation = ch
  */
       goto __pyx_L5;
     }
 
-    /* "tarina/_string_c.pyx":62
+    /* "tarina/_string_c.pyx":53
  *             if escape:
  *                 PyList_SET_ITEM(result, Py_SIZE(result)-1 , ch)
  *         elif (quotation == 0 and contains(separates, ch)) or (crlf and set_contains_key(CRLF, ch)):             # <<<<<<<<<<<<<<
  *             if result and result[-1] != '\1':
  *                 PyList_Append(result, '\1')
  */
     __pyx_t_2 = ((__pyx_v_quotation == 0) != 0);
     if (!__pyx_t_2) {
       goto __pyx_L9_next_or;
     } else {
     }
-    __pyx_t_2 = (__pyx_f_6tarina_9_string_c_contains(__pyx_v_separates, __pyx_v_ch) != 0);
+    __pyx_t_2 = (contains(__pyx_v_separates, __pyx_v_ch) != 0);
     if (!__pyx_t_2) {
     } else {
       __pyx_t_5 = __pyx_t_2;
       goto __pyx_L8_bool_binop_done;
     }
     __pyx_L9_next_or:;
     __pyx_t_2 = (__pyx_v_crlf != 0);
     if (__pyx_t_2) {
     } else {
       __pyx_t_5 = __pyx_t_2;
       goto __pyx_L8_bool_binop_done;
     }
     __pyx_t_4 = __pyx_v_6tarina_9_string_c_CRLF;
     __Pyx_INCREF(__pyx_t_4);
-    __pyx_t_1 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 62, __pyx_L1_error)
+    __pyx_t_1 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 53, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = set_contains_key(__pyx_t_4, __pyx_t_1); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 62, __pyx_L1_error)
+    __pyx_t_2 = set_contains_key(__pyx_t_4, __pyx_t_1); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 53, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_6 = (__pyx_t_2 != 0);
     __pyx_t_5 = __pyx_t_6;
     __pyx_L8_bool_binop_done:;
     if (__pyx_t_5) {
 
-      /* "tarina/_string_c.pyx":63
+      /* "tarina/_string_c.pyx":54
  *                 PyList_SET_ITEM(result, Py_SIZE(result)-1 , ch)
  *         elif (quotation == 0 and contains(separates, ch)) or (crlf and set_contains_key(CRLF, ch)):
  *             if result and result[-1] != '\1':             # <<<<<<<<<<<<<<
  *                 PyList_Append(result, '\1')
  *         else:
  */
       __pyx_t_6 = (PyList_GET_SIZE(__pyx_v_result) != 0);
       if (__pyx_t_6) {
       } else {
         __pyx_t_5 = __pyx_t_6;
         goto __pyx_L13_bool_binop_done;
       }
-      __pyx_t_1 = __Pyx_GetItemInt_List(__pyx_v_result, -1L, long, 1, __Pyx_PyInt_From_long, 1, 1, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 63, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_GetItemInt_List(__pyx_v_result, -1L, long, 1, __Pyx_PyInt_From_long, 1, 1, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 54, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_6 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_kp_u_, Py_NE)); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 63, __pyx_L1_error)
+      __pyx_t_6 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_kp_u_, Py_NE)); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 54, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_5 = __pyx_t_6;
       __pyx_L13_bool_binop_done:;
       if (__pyx_t_5) {
 
-        /* "tarina/_string_c.pyx":64
+        /* "tarina/_string_c.pyx":55
  *         elif (quotation == 0 and contains(separates, ch)) or (crlf and set_contains_key(CRLF, ch)):
  *             if result and result[-1] != '\1':
  *                 PyList_Append(result, '\1')             # <<<<<<<<<<<<<<
  *         else:
  *             PyList_Append(result, ch)
  */
-        __pyx_t_3 = PyList_Append(__pyx_v_result, __pyx_kp_u_); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 64, __pyx_L1_error)
+        __pyx_t_3 = PyList_Append(__pyx_v_result, __pyx_kp_u_); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 55, __pyx_L1_error)
 
-        /* "tarina/_string_c.pyx":63
+        /* "tarina/_string_c.pyx":54
  *                 PyList_SET_ITEM(result, Py_SIZE(result)-1 , ch)
  *         elif (quotation == 0 and contains(separates, ch)) or (crlf and set_contains_key(CRLF, ch)):
  *             if result and result[-1] != '\1':             # <<<<<<<<<<<<<<
  *                 PyList_Append(result, '\1')
  *         else:
  */
       }
 
-      /* "tarina/_string_c.pyx":62
+      /* "tarina/_string_c.pyx":53
  *             if escape:
  *                 PyList_SET_ITEM(result, Py_SIZE(result)-1 , ch)
  *         elif (quotation == 0 and contains(separates, ch)) or (crlf and set_contains_key(CRLF, ch)):             # <<<<<<<<<<<<<<
  *             if result and result[-1] != '\1':
  *                 PyList_Append(result, '\1')
  */
       goto __pyx_L5;
     }
 
-    /* "tarina/_string_c.pyx":66
+    /* "tarina/_string_c.pyx":57
  *                 PyList_Append(result, '\1')
  *         else:
  *             PyList_Append(result, ch)             # <<<<<<<<<<<<<<
  *             escape = 0
  *     if PyUnicode_GET_LENGTH(result) == 0:
  */
     /*else*/ {
-      __pyx_t_1 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 66, __pyx_L1_error)
+      __pyx_t_1 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 57, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_3 = PyList_Append(__pyx_v_result, __pyx_t_1); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 66, __pyx_L1_error)
+      __pyx_t_3 = PyList_Append(__pyx_v_result, __pyx_t_1); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 57, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "tarina/_string_c.pyx":67
+      /* "tarina/_string_c.pyx":58
  *         else:
  *             PyList_Append(result, ch)
  *             escape = 0             # <<<<<<<<<<<<<<
  *     if PyUnicode_GET_LENGTH(result) == 0:
  *         return []
  */
       __pyx_v_escape = 0;
     }
     __pyx_L5:;
     __pyx_L3_continue:;
   }
 
-  /* "tarina/_string_c.pyx":68
+  /* "tarina/_string_c.pyx":59
  *             PyList_Append(result, ch)
  *             escape = 0
  *     if PyUnicode_GET_LENGTH(result) == 0:             # <<<<<<<<<<<<<<
  *         return []
  *     return PyUnicode_Split(PyUnicode_Join('', result), '\1', -1)
  */
   __pyx_t_5 = ((PyUnicode_GET_LENGTH(__pyx_v_result) == 0) != 0);
   if (__pyx_t_5) {
 
-    /* "tarina/_string_c.pyx":69
+    /* "tarina/_string_c.pyx":60
  *             escape = 0
  *     if PyUnicode_GET_LENGTH(result) == 0:
  *         return []             # <<<<<<<<<<<<<<
  *     return PyUnicode_Split(PyUnicode_Join('', result), '\1', -1)
  * 
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 69, __pyx_L1_error)
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 60, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_r = __pyx_t_1;
     __pyx_t_1 = 0;
     goto __pyx_L0;
 
-    /* "tarina/_string_c.pyx":68
+    /* "tarina/_string_c.pyx":59
  *             PyList_Append(result, ch)
  *             escape = 0
  *     if PyUnicode_GET_LENGTH(result) == 0:             # <<<<<<<<<<<<<<
  *         return []
  *     return PyUnicode_Split(PyUnicode_Join('', result), '\1', -1)
  */
   }
 
-  /* "tarina/_string_c.pyx":70
+  /* "tarina/_string_c.pyx":61
  *     if PyUnicode_GET_LENGTH(result) == 0:
  *         return []
  *     return PyUnicode_Split(PyUnicode_Join('', result), '\1', -1)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyUnicode_Join(__pyx_kp_u__2, __pyx_v_result); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __pyx_t_1 = PyUnicode_Join(__pyx_kp_u__2, __pyx_v_result); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 61, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = PyUnicode_Split(__pyx_t_1, __pyx_kp_u_, -1L); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __pyx_t_4 = PyUnicode_Split(__pyx_t_1, __pyx_kp_u_, -1L); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 61, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "tarina/_string_c.pyx":28
+  /* "tarina/_string_c.pyx":19
  * cdef set CRLF = {'\r', '\n'}
  * 
  * def split(str text, tuple separates, char crlf=True):             # <<<<<<<<<<<<<<
  *     """
  * 
  */
 
@@ -2048,15 +1918,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "tarina/_string_c.pyx":73
+/* "tarina/_string_c.pyx":64
  * 
  * 
  * def split_once(str text, tuple separates, char crlf=True):             # <<<<<<<<<<<<<<
  *     text = text.lstrip()
  *     cdef Py_ssize_t index = 0
  */
 
@@ -2094,54 +1964,54 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_text)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_separates)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("split_once", 0, 2, 3, 1); __PYX_ERR(0, 73, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("split_once", 0, 2, 3, 1); __PYX_ERR(0, 64, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_crlf);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "split_once") < 0)) __PYX_ERR(0, 73, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "split_once") < 0)) __PYX_ERR(0, 64, __pyx_L3_error)
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
     __pyx_v_text = ((PyObject*)values[0]);
     __pyx_v_separates = ((PyObject*)values[1]);
     if (values[2]) {
-      __pyx_v_crlf = __Pyx_PyInt_As_char(values[2]); if (unlikely((__pyx_v_crlf == (char)-1) && PyErr_Occurred())) __PYX_ERR(0, 73, __pyx_L3_error)
+      __pyx_v_crlf = __Pyx_PyInt_As_char(values[2]); if (unlikely((__pyx_v_crlf == (char)-1) && PyErr_Occurred())) __PYX_ERR(0, 64, __pyx_L3_error)
     } else {
       __pyx_v_crlf = ((char)1);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("split_once", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 73, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("split_once", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 64, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("tarina._string_c.split_once", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_text), (&PyUnicode_Type), 1, "text", 1))) __PYX_ERR(0, 73, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_separates), (&PyTuple_Type), 1, "separates", 1))) __PYX_ERR(0, 73, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_text), (&PyUnicode_Type), 1, "text", 1))) __PYX_ERR(0, 64, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_separates), (&PyTuple_Type), 1, "separates", 1))) __PYX_ERR(0, 64, __pyx_L1_error)
   __pyx_r = __pyx_pf_6tarina_9_string_c_2split_once(__pyx_self, __pyx_v_text, __pyx_v_separates, __pyx_v_crlf);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -2168,457 +2038,457 @@
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("split_once", 0);
   __Pyx_INCREF(__pyx_v_text);
 
-  /* "tarina/_string_c.pyx":74
+  /* "tarina/_string_c.pyx":65
  * 
  * def split_once(str text, tuple separates, char crlf=True):
  *     text = text.lstrip()             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t index = 0
  *     cdef list out_text = []
  */
-  __pyx_t_1 = __Pyx_CallUnboundCMethod0(&__pyx_umethod_PyUnicode_Type_lstrip, __pyx_v_text); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 74, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CallUnboundCMethod0(&__pyx_umethod_PyUnicode_Type_lstrip, __pyx_v_text); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 74, __pyx_L1_error)
+  if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_DECREF_SET(__pyx_v_text, ((PyObject*)__pyx_t_1));
   __pyx_t_1 = 0;
 
-  /* "tarina/_string_c.pyx":75
+  /* "tarina/_string_c.pyx":66
  * def split_once(str text, tuple separates, char crlf=True):
  *     text = text.lstrip()
  *     cdef Py_ssize_t index = 0             # <<<<<<<<<<<<<<
  *     cdef list out_text = []
  *     cdef Py_UCS4 quotation = 0
  */
   __pyx_v_index = 0;
 
-  /* "tarina/_string_c.pyx":76
+  /* "tarina/_string_c.pyx":67
  *     text = text.lstrip()
  *     cdef Py_ssize_t index = 0
  *     cdef list out_text = []             # <<<<<<<<<<<<<<
  *     cdef Py_UCS4 quotation = 0
  *     cdef Py_UCS4 ch = 0
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 76, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_out_text = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "tarina/_string_c.pyx":77
+  /* "tarina/_string_c.pyx":68
  *     cdef Py_ssize_t index = 0
  *     cdef list out_text = []
  *     cdef Py_UCS4 quotation = 0             # <<<<<<<<<<<<<<
  *     cdef Py_UCS4 ch = 0
  *     cdef char escape = 0
  */
   __pyx_v_quotation = 0;
 
-  /* "tarina/_string_c.pyx":78
+  /* "tarina/_string_c.pyx":69
  *     cdef list out_text = []
  *     cdef Py_UCS4 quotation = 0
  *     cdef Py_UCS4 ch = 0             # <<<<<<<<<<<<<<
  *     cdef char escape = 0
  *     cdef char sep = 0
  */
   __pyx_v_ch = 0;
 
-  /* "tarina/_string_c.pyx":79
+  /* "tarina/_string_c.pyx":70
  *     cdef Py_UCS4 quotation = 0
  *     cdef Py_UCS4 ch = 0
  *     cdef char escape = 0             # <<<<<<<<<<<<<<
  *     cdef char sep = 0
  *     cdef Py_ssize_t length = PyUnicode_GET_LENGTH(text)
  */
   __pyx_v_escape = 0;
 
-  /* "tarina/_string_c.pyx":80
+  /* "tarina/_string_c.pyx":71
  *     cdef Py_UCS4 ch = 0
  *     cdef char escape = 0
  *     cdef char sep = 0             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t length = PyUnicode_GET_LENGTH(text)
  * 
  */
   __pyx_v_sep = 0;
 
-  /* "tarina/_string_c.pyx":81
+  /* "tarina/_string_c.pyx":72
  *     cdef char escape = 0
  *     cdef char sep = 0
  *     cdef Py_ssize_t length = PyUnicode_GET_LENGTH(text)             # <<<<<<<<<<<<<<
  * 
  *     while index < length:
  */
   __pyx_v_length = PyUnicode_GET_LENGTH(__pyx_v_text);
 
-  /* "tarina/_string_c.pyx":83
+  /* "tarina/_string_c.pyx":74
  *     cdef Py_ssize_t length = PyUnicode_GET_LENGTH(text)
  * 
  *     while index < length:             # <<<<<<<<<<<<<<
  *         ch = PyUnicode_READ_CHAR(text, index)
  *         index += 1
  */
   while (1) {
     __pyx_t_2 = ((__pyx_v_index < __pyx_v_length) != 0);
     if (!__pyx_t_2) break;
 
-    /* "tarina/_string_c.pyx":84
+    /* "tarina/_string_c.pyx":75
  * 
  *     while index < length:
  *         ch = PyUnicode_READ_CHAR(text, index)             # <<<<<<<<<<<<<<
  *         index += 1
  *         if quotation == 0 and (contains(separates, ch) or (crlf and set_contains_key(CRLF, ch))):
  */
     __pyx_v_ch = PyUnicode_READ_CHAR(__pyx_v_text, __pyx_v_index);
 
-    /* "tarina/_string_c.pyx":85
+    /* "tarina/_string_c.pyx":76
  *     while index < length:
  *         ch = PyUnicode_READ_CHAR(text, index)
  *         index += 1             # <<<<<<<<<<<<<<
  *         if quotation == 0 and (contains(separates, ch) or (crlf and set_contains_key(CRLF, ch))):
  *             sep = 1
  */
     __pyx_v_index = (__pyx_v_index + 1);
 
-    /* "tarina/_string_c.pyx":86
+    /* "tarina/_string_c.pyx":77
  *         ch = PyUnicode_READ_CHAR(text, index)
  *         index += 1
  *         if quotation == 0 and (contains(separates, ch) or (crlf and set_contains_key(CRLF, ch))):             # <<<<<<<<<<<<<<
  *             sep = 1
  *             continue
  */
     __pyx_t_3 = ((__pyx_v_quotation == 0) != 0);
     if (__pyx_t_3) {
     } else {
       __pyx_t_2 = __pyx_t_3;
       goto __pyx_L6_bool_binop_done;
     }
-    __pyx_t_3 = (__pyx_f_6tarina_9_string_c_contains(__pyx_v_separates, __pyx_v_ch) != 0);
+    __pyx_t_3 = (contains(__pyx_v_separates, __pyx_v_ch) != 0);
     if (!__pyx_t_3) {
     } else {
       __pyx_t_2 = __pyx_t_3;
       goto __pyx_L6_bool_binop_done;
     }
     __pyx_t_3 = (__pyx_v_crlf != 0);
     if (__pyx_t_3) {
     } else {
       __pyx_t_2 = __pyx_t_3;
       goto __pyx_L6_bool_binop_done;
     }
     __pyx_t_1 = __pyx_v_6tarina_9_string_c_CRLF;
     __Pyx_INCREF(__pyx_t_1);
-    __pyx_t_4 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 86, __pyx_L1_error)
+    __pyx_t_4 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 77, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_3 = set_contains_key(__pyx_t_1, __pyx_t_4); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 86, __pyx_L1_error)
+    __pyx_t_3 = set_contains_key(__pyx_t_1, __pyx_t_4); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 77, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_5 = (__pyx_t_3 != 0);
     __pyx_t_2 = __pyx_t_5;
     __pyx_L6_bool_binop_done:;
     if (__pyx_t_2) {
 
-      /* "tarina/_string_c.pyx":87
+      /* "tarina/_string_c.pyx":78
  *         index += 1
  *         if quotation == 0 and (contains(separates, ch) or (crlf and set_contains_key(CRLF, ch))):
  *             sep = 1             # <<<<<<<<<<<<<<
  *             continue
  *         if sep == 1:
  */
       __pyx_v_sep = 1;
 
-      /* "tarina/_string_c.pyx":88
+      /* "tarina/_string_c.pyx":79
  *         if quotation == 0 and (contains(separates, ch) or (crlf and set_contains_key(CRLF, ch))):
  *             sep = 1
  *             continue             # <<<<<<<<<<<<<<
  *         if sep == 1:
  *             index -= 1
  */
       goto __pyx_L3_continue;
 
-      /* "tarina/_string_c.pyx":86
+      /* "tarina/_string_c.pyx":77
  *         ch = PyUnicode_READ_CHAR(text, index)
  *         index += 1
  *         if quotation == 0 and (contains(separates, ch) or (crlf and set_contains_key(CRLF, ch))):             # <<<<<<<<<<<<<<
  *             sep = 1
  *             continue
  */
     }
 
-    /* "tarina/_string_c.pyx":89
+    /* "tarina/_string_c.pyx":80
  *             sep = 1
  *             continue
  *         if sep == 1:             # <<<<<<<<<<<<<<
  *             index -= 1
  *             break
  */
     __pyx_t_2 = ((__pyx_v_sep == 1) != 0);
     if (__pyx_t_2) {
 
-      /* "tarina/_string_c.pyx":90
+      /* "tarina/_string_c.pyx":81
  *             continue
  *         if sep == 1:
  *             index -= 1             # <<<<<<<<<<<<<<
  *             break
  *         if ch == 92:  # \\
  */
       __pyx_v_index = (__pyx_v_index - 1);
 
-      /* "tarina/_string_c.pyx":91
+      /* "tarina/_string_c.pyx":82
  *         if sep == 1:
  *             index -= 1
  *             break             # <<<<<<<<<<<<<<
  *         if ch == 92:  # \\
  *             escape = 1
  */
       goto __pyx_L4_break;
 
-      /* "tarina/_string_c.pyx":89
+      /* "tarina/_string_c.pyx":80
  *             sep = 1
  *             continue
  *         if sep == 1:             # <<<<<<<<<<<<<<
  *             index -= 1
  *             break
  */
     }
 
-    /* "tarina/_string_c.pyx":92
+    /* "tarina/_string_c.pyx":83
  *             index -= 1
  *             break
  *         if ch == 92:  # \\             # <<<<<<<<<<<<<<
  *             escape = 1
  *             PyList_Append(out_text, ch)
  */
     __pyx_t_2 = ((__pyx_v_ch == 92) != 0);
     if (__pyx_t_2) {
 
-      /* "tarina/_string_c.pyx":93
+      /* "tarina/_string_c.pyx":84
  *             break
  *         if ch == 92:  # \\
  *             escape = 1             # <<<<<<<<<<<<<<
  *             PyList_Append(out_text, ch)
  *         elif set_contains_key(QUOTES, ch):  #
  */
       __pyx_v_escape = 1;
 
-      /* "tarina/_string_c.pyx":94
+      /* "tarina/_string_c.pyx":85
  *         if ch == 92:  # \\
  *             escape = 1
  *             PyList_Append(out_text, ch)             # <<<<<<<<<<<<<<
  *         elif set_contains_key(QUOTES, ch):  #
  *             if quotation == 0:
  */
-      __pyx_t_4 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 94, __pyx_L1_error)
+      __pyx_t_4 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 85, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_6 = PyList_Append(__pyx_v_out_text, __pyx_t_4); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 94, __pyx_L1_error)
+      __pyx_t_6 = PyList_Append(__pyx_v_out_text, __pyx_t_4); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 85, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-      /* "tarina/_string_c.pyx":92
+      /* "tarina/_string_c.pyx":83
  *             index -= 1
  *             break
  *         if ch == 92:  # \\             # <<<<<<<<<<<<<<
  *             escape = 1
  *             PyList_Append(out_text, ch)
  */
       goto __pyx_L11;
     }
 
-    /* "tarina/_string_c.pyx":95
+    /* "tarina/_string_c.pyx":86
  *             escape = 1
  *             PyList_Append(out_text, ch)
  *         elif set_contains_key(QUOTES, ch):  #             # <<<<<<<<<<<<<<
  *             if quotation == 0:
  *                 quotation = ch
  */
     __pyx_t_4 = __pyx_v_6tarina_9_string_c_QUOTES;
     __Pyx_INCREF(__pyx_t_4);
-    __pyx_t_1 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 95, __pyx_L1_error)
+    __pyx_t_1 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 86, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = set_contains_key(__pyx_t_4, __pyx_t_1); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 95, __pyx_L1_error)
+    __pyx_t_2 = set_contains_key(__pyx_t_4, __pyx_t_1); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 86, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_5 = (__pyx_t_2 != 0);
     if (__pyx_t_5) {
 
-      /* "tarina/_string_c.pyx":96
+      /* "tarina/_string_c.pyx":87
  *             PyList_Append(out_text, ch)
  *         elif set_contains_key(QUOTES, ch):  #
  *             if quotation == 0:             # <<<<<<<<<<<<<<
  *                 quotation = ch
  *             elif ch == quotation:
  */
       __pyx_t_5 = ((__pyx_v_quotation == 0) != 0);
       if (__pyx_t_5) {
 
-        /* "tarina/_string_c.pyx":97
+        /* "tarina/_string_c.pyx":88
  *         elif set_contains_key(QUOTES, ch):  #
  *             if quotation == 0:
  *                 quotation = ch             # <<<<<<<<<<<<<<
  *             elif ch == quotation:
  *                 quotation = 0
  */
         __pyx_v_quotation = __pyx_v_ch;
 
-        /* "tarina/_string_c.pyx":96
+        /* "tarina/_string_c.pyx":87
  *             PyList_Append(out_text, ch)
  *         elif set_contains_key(QUOTES, ch):  #
  *             if quotation == 0:             # <<<<<<<<<<<<<<
  *                 quotation = ch
  *             elif ch == quotation:
  */
         goto __pyx_L12;
       }
 
-      /* "tarina/_string_c.pyx":98
+      /* "tarina/_string_c.pyx":89
  *             if quotation == 0:
  *                 quotation = ch
  *             elif ch == quotation:             # <<<<<<<<<<<<<<
  *                 quotation = 0
  *             else:
  */
       __pyx_t_5 = ((__pyx_v_ch == __pyx_v_quotation) != 0);
       if (__pyx_t_5) {
 
-        /* "tarina/_string_c.pyx":99
+        /* "tarina/_string_c.pyx":90
  *                 quotation = ch
  *             elif ch == quotation:
  *                 quotation = 0             # <<<<<<<<<<<<<<
  *             else:
  *                 PyList_Append(out_text, ch)
  */
         __pyx_v_quotation = 0;
 
-        /* "tarina/_string_c.pyx":98
+        /* "tarina/_string_c.pyx":89
  *             if quotation == 0:
  *                 quotation = ch
  *             elif ch == quotation:             # <<<<<<<<<<<<<<
  *                 quotation = 0
  *             else:
  */
         goto __pyx_L12;
       }
 
-      /* "tarina/_string_c.pyx":101
+      /* "tarina/_string_c.pyx":92
  *                 quotation = 0
  *             else:
  *                 PyList_Append(out_text, ch)             # <<<<<<<<<<<<<<
  *                 continue
  *             if escape:
  */
       /*else*/ {
-        __pyx_t_1 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 101, __pyx_L1_error)
+        __pyx_t_1 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 92, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_6 = PyList_Append(__pyx_v_out_text, __pyx_t_1); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 101, __pyx_L1_error)
+        __pyx_t_6 = PyList_Append(__pyx_v_out_text, __pyx_t_1); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 92, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-        /* "tarina/_string_c.pyx":102
+        /* "tarina/_string_c.pyx":93
  *             else:
  *                 PyList_Append(out_text, ch)
  *                 continue             # <<<<<<<<<<<<<<
  *             if escape:
  *                 PyList_SET_ITEM(out_text, Py_SIZE(out_text) - 1, ch)
  */
         goto __pyx_L3_continue;
       }
       __pyx_L12:;
 
-      /* "tarina/_string_c.pyx":103
+      /* "tarina/_string_c.pyx":94
  *                 PyList_Append(out_text, ch)
  *                 continue
  *             if escape:             # <<<<<<<<<<<<<<
  *                 PyList_SET_ITEM(out_text, Py_SIZE(out_text) - 1, ch)
  *         else:
  */
       __pyx_t_5 = (__pyx_v_escape != 0);
       if (__pyx_t_5) {
 
-        /* "tarina/_string_c.pyx":104
+        /* "tarina/_string_c.pyx":95
  *                 continue
  *             if escape:
  *                 PyList_SET_ITEM(out_text, Py_SIZE(out_text) - 1, ch)             # <<<<<<<<<<<<<<
  *         else:
  *             PyList_Append(out_text, ch)
  */
-        __pyx_t_1 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 104, __pyx_L1_error)
+        __pyx_t_1 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 95, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         PyList_SET_ITEM(__pyx_v_out_text, (Py_SIZE(__pyx_v_out_text) - 1), __pyx_t_1);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-        /* "tarina/_string_c.pyx":103
+        /* "tarina/_string_c.pyx":94
  *                 PyList_Append(out_text, ch)
  *                 continue
  *             if escape:             # <<<<<<<<<<<<<<
  *                 PyList_SET_ITEM(out_text, Py_SIZE(out_text) - 1, ch)
  *         else:
  */
       }
 
-      /* "tarina/_string_c.pyx":95
+      /* "tarina/_string_c.pyx":86
  *             escape = 1
  *             PyList_Append(out_text, ch)
  *         elif set_contains_key(QUOTES, ch):  #             # <<<<<<<<<<<<<<
  *             if quotation == 0:
  *                 quotation = ch
  */
       goto __pyx_L11;
     }
 
-    /* "tarina/_string_c.pyx":106
+    /* "tarina/_string_c.pyx":97
  *                 PyList_SET_ITEM(out_text, Py_SIZE(out_text) - 1, ch)
  *         else:
  *             PyList_Append(out_text, ch)             # <<<<<<<<<<<<<<
  *             escape = 0
  *     return PyUnicode_Join('', out_text), text[index:]
  */
     /*else*/ {
-      __pyx_t_1 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 106, __pyx_L1_error)
+      __pyx_t_1 = PyUnicode_FromOrdinal(__pyx_v_ch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 97, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_6 = PyList_Append(__pyx_v_out_text, __pyx_t_1); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 106, __pyx_L1_error)
+      __pyx_t_6 = PyList_Append(__pyx_v_out_text, __pyx_t_1); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 97, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "tarina/_string_c.pyx":107
+      /* "tarina/_string_c.pyx":98
  *         else:
  *             PyList_Append(out_text, ch)
  *             escape = 0             # <<<<<<<<<<<<<<
  *     return PyUnicode_Join('', out_text), text[index:]
  */
       __pyx_v_escape = 0;
     }
     __pyx_L11:;
     __pyx_L3_continue:;
   }
   __pyx_L4_break:;
 
-  /* "tarina/_string_c.pyx":108
+  /* "tarina/_string_c.pyx":99
  *             PyList_Append(out_text, ch)
  *             escape = 0
  *     return PyUnicode_Join('', out_text), text[index:]             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyUnicode_Join(__pyx_kp_u__2, __pyx_v_out_text); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 108, __pyx_L1_error)
+  __pyx_t_1 = PyUnicode_Join(__pyx_kp_u__2, __pyx_v_out_text); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 99, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (unlikely(__pyx_v_text == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 108, __pyx_L1_error)
+    __PYX_ERR(0, 99, __pyx_L1_error)
   }
-  __pyx_t_4 = __Pyx_PyUnicode_Substring(__pyx_v_text, __pyx_v_index, PY_SSIZE_T_MAX); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 108, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyUnicode_Substring(__pyx_v_text, __pyx_v_index, PY_SSIZE_T_MAX); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 99, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_7 = PyTuple_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 108, __pyx_L1_error)
+  __pyx_t_7 = PyTuple_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 99, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_t_4);
   __pyx_t_1 = 0;
   __pyx_t_4 = 0;
   __pyx_r = __pyx_t_7;
   __pyx_t_7 = 0;
   goto __pyx_L0;
 
-  /* "tarina/_string_c.pyx":73
+  /* "tarina/_string_c.pyx":64
  * 
  * 
  * def split_once(str text, tuple separates, char crlf=True):             # <<<<<<<<<<<<<<
  *     text = text.lstrip()
  *     cdef Py_ssize_t index = 0
  */
 
@@ -2716,37 +2586,37 @@
   return 0;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "tarina/_string_c.pyx":28
+  /* "tarina/_string_c.pyx":19
  * cdef set CRLF = {'\r', '\n'}
  * 
  * def split(str text, tuple separates, char crlf=True):             # <<<<<<<<<<<<<<
  *     """
  * 
  */
-  __pyx_tuple__7 = PyTuple_Pack(9, __pyx_n_s_text, __pyx_n_s_separates, __pyx_n_s_crlf, __pyx_n_s_escape, __pyx_n_s_result, __pyx_n_s_quotation, __pyx_n_s_ch, __pyx_n_s_i, __pyx_n_s_length); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_tuple__7 = PyTuple_Pack(9, __pyx_n_s_text, __pyx_n_s_separates, __pyx_n_s_crlf, __pyx_n_s_escape, __pyx_n_s_result, __pyx_n_s_quotation, __pyx_n_s_ch, __pyx_n_s_i, __pyx_n_s_length); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 19, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
-  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(3, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_tarina__string_c_pyx, __pyx_n_s_split, 28, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(3, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_tarina__string_c_pyx, __pyx_n_s_split, 19, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(0, 19, __pyx_L1_error)
 
-  /* "tarina/_string_c.pyx":73
+  /* "tarina/_string_c.pyx":64
  * 
  * 
  * def split_once(str text, tuple separates, char crlf=True):             # <<<<<<<<<<<<<<
  *     text = text.lstrip()
  *     cdef Py_ssize_t index = 0
  */
-  __pyx_tuple__9 = PyTuple_Pack(10, __pyx_n_s_text, __pyx_n_s_separates, __pyx_n_s_crlf, __pyx_n_s_index, __pyx_n_s_out_text, __pyx_n_s_quotation, __pyx_n_s_ch, __pyx_n_s_escape, __pyx_n_s_sep, __pyx_n_s_length); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 73, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(10, __pyx_n_s_text, __pyx_n_s_separates, __pyx_n_s_crlf, __pyx_n_s_index, __pyx_n_s_out_text, __pyx_n_s_quotation, __pyx_n_s_ch, __pyx_n_s_escape, __pyx_n_s_sep, __pyx_n_s_length); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
-  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(3, 0, 10, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_tarina__string_c_pyx, __pyx_n_s_split_once, 73, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(0, 73, __pyx_L1_error)
+  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(3, 0, 10, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_tarina__string_c_pyx, __pyx_n_s_split_once, 64, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -3039,68 +2909,68 @@
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
-  /* "tarina/_string_c.pyx":25
- *     return 0
+  /* "tarina/_string_c.pyx":16
+ *     bint set_contains_key(object anyset, object key) except -1
  * 
  * cdef set QUOTES = {'"', '\''}             # <<<<<<<<<<<<<<
  * cdef set CRLF = {'\r', '\n'}
  * 
  */
-  __pyx_t_1 = PySet_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 25, __pyx_L1_error)
+  __pyx_t_1 = PySet_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PySet_Add(__pyx_t_1, __pyx_kp_u__3) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
-  if (PySet_Add(__pyx_t_1, __pyx_kp_u__4) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
+  if (PySet_Add(__pyx_t_1, __pyx_kp_u__3) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
+  if (PySet_Add(__pyx_t_1, __pyx_kp_u__4) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_XGOTREF(__pyx_v_6tarina_9_string_c_QUOTES);
   __Pyx_DECREF_SET(__pyx_v_6tarina_9_string_c_QUOTES, ((PyObject*)__pyx_t_1));
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "tarina/_string_c.pyx":26
+  /* "tarina/_string_c.pyx":17
  * 
  * cdef set QUOTES = {'"', '\''}
  * cdef set CRLF = {'\r', '\n'}             # <<<<<<<<<<<<<<
  * 
  * def split(str text, tuple separates, char crlf=True):
  */
-  __pyx_t_1 = PySet_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __pyx_t_1 = PySet_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PySet_Add(__pyx_t_1, __pyx_kp_u__5) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
-  if (PySet_Add(__pyx_t_1, __pyx_kp_u__6) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
+  if (PySet_Add(__pyx_t_1, __pyx_kp_u__5) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
+  if (PySet_Add(__pyx_t_1, __pyx_kp_u__6) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_XGOTREF(__pyx_v_6tarina_9_string_c_CRLF);
   __Pyx_DECREF_SET(__pyx_v_6tarina_9_string_c_CRLF, ((PyObject*)__pyx_t_1));
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "tarina/_string_c.pyx":28
+  /* "tarina/_string_c.pyx":19
  * cdef set CRLF = {'\r', '\n'}
  * 
  * def split(str text, tuple separates, char crlf=True):             # <<<<<<<<<<<<<<
  *     """
  * 
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_6tarina_9_string_c_1split, NULL, __pyx_n_s_tarina__string_c); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_6tarina_9_string_c_1split, NULL, __pyx_n_s_tarina__string_c); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 19, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_split, __pyx_t_1) < 0) __PYX_ERR(0, 28, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_split, __pyx_t_1) < 0) __PYX_ERR(0, 19, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "tarina/_string_c.pyx":73
+  /* "tarina/_string_c.pyx":64
  * 
  * 
  * def split_once(str text, tuple separates, char crlf=True):             # <<<<<<<<<<<<<<
  *     text = text.lstrip()
  *     cdef Py_ssize_t index = 0
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_6tarina_9_string_c_3split_once, NULL, __pyx_n_s_tarina__string_c); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 73, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_6tarina_9_string_c_3split_once, NULL, __pyx_n_s_tarina__string_c); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_split_once, __pyx_t_1) < 0) __PYX_ERR(0, 73, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_split_once, __pyx_t_1) < 0) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "tarina/_string_c.pyx":1
  * # cython: boundscheck=False             # <<<<<<<<<<<<<<
  * # cython: cdivision=True
  * # cython: initializedcheck=False
  */
@@ -3147,227 +3017,14 @@
 end:
     Py_XDECREF(p);
     Py_XDECREF(m);
     return (__Pyx_RefNannyAPIStruct *)r;
 }
 #endif
 
-/* BytesEquals */
-static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals) {
-#if CYTHON_COMPILING_IN_PYPY
-    return PyObject_RichCompareBool(s1, s2, equals);
-#else
-    if (s1 == s2) {
-        return (equals == Py_EQ);
-    } else if (PyBytes_CheckExact(s1) & PyBytes_CheckExact(s2)) {
-        const char *ps1, *ps2;
-        Py_ssize_t length = PyBytes_GET_SIZE(s1);
-        if (length != PyBytes_GET_SIZE(s2))
-            return (equals == Py_NE);
-        ps1 = PyBytes_AS_STRING(s1);
-        ps2 = PyBytes_AS_STRING(s2);
-        if (ps1[0] != ps2[0]) {
-            return (equals == Py_NE);
-        } else if (length == 1) {
-            return (equals == Py_EQ);
-        } else {
-            int result;
-#if CYTHON_USE_UNICODE_INTERNALS && (PY_VERSION_HEX < 0x030B0000)
-            Py_hash_t hash1, hash2;
-            hash1 = ((PyBytesObject*)s1)->ob_shash;
-            hash2 = ((PyBytesObject*)s2)->ob_shash;
-            if (hash1 != hash2 && hash1 != -1 && hash2 != -1) {
-                return (equals == Py_NE);
-            }
-#endif
-            result = memcmp(ps1, ps2, (size_t)length);
-            return (equals == Py_EQ) ? (result == 0) : (result != 0);
-        }
-    } else if ((s1 == Py_None) & PyBytes_CheckExact(s2)) {
-        return (equals == Py_NE);
-    } else if ((s2 == Py_None) & PyBytes_CheckExact(s1)) {
-        return (equals == Py_NE);
-    } else {
-        int result;
-        PyObject* py_result = PyObject_RichCompare(s1, s2, equals);
-        if (!py_result)
-            return -1;
-        result = __Pyx_PyObject_IsTrue(py_result);
-        Py_DECREF(py_result);
-        return result;
-    }
-#endif
-}
-
-/* UnicodeEquals */
-static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals) {
-#if CYTHON_COMPILING_IN_PYPY
-    return PyObject_RichCompareBool(s1, s2, equals);
-#else
-#if PY_MAJOR_VERSION < 3
-    PyObject* owned_ref = NULL;
-#endif
-    int s1_is_unicode, s2_is_unicode;
-    if (s1 == s2) {
-        goto return_eq;
-    }
-    s1_is_unicode = PyUnicode_CheckExact(s1);
-    s2_is_unicode = PyUnicode_CheckExact(s2);
-#if PY_MAJOR_VERSION < 3
-    if ((s1_is_unicode & (!s2_is_unicode)) && PyString_CheckExact(s2)) {
-        owned_ref = PyUnicode_FromObject(s2);
-        if (unlikely(!owned_ref))
-            return -1;
-        s2 = owned_ref;
-        s2_is_unicode = 1;
-    } else if ((s2_is_unicode & (!s1_is_unicode)) && PyString_CheckExact(s1)) {
-        owned_ref = PyUnicode_FromObject(s1);
-        if (unlikely(!owned_ref))
-            return -1;
-        s1 = owned_ref;
-        s1_is_unicode = 1;
-    } else if (((!s2_is_unicode) & (!s1_is_unicode))) {
-        return __Pyx_PyBytes_Equals(s1, s2, equals);
-    }
-#endif
-    if (s1_is_unicode & s2_is_unicode) {
-        Py_ssize_t length;
-        int kind;
-        void *data1, *data2;
-        if (unlikely(__Pyx_PyUnicode_READY(s1) < 0) || unlikely(__Pyx_PyUnicode_READY(s2) < 0))
-            return -1;
-        length = __Pyx_PyUnicode_GET_LENGTH(s1);
-        if (length != __Pyx_PyUnicode_GET_LENGTH(s2)) {
-            goto return_ne;
-        }
-#if CYTHON_USE_UNICODE_INTERNALS
-        {
-            Py_hash_t hash1, hash2;
-        #if CYTHON_PEP393_ENABLED
-            hash1 = ((PyASCIIObject*)s1)->hash;
-            hash2 = ((PyASCIIObject*)s2)->hash;
-        #else
-            hash1 = ((PyUnicodeObject*)s1)->hash;
-            hash2 = ((PyUnicodeObject*)s2)->hash;
-        #endif
-            if (hash1 != hash2 && hash1 != -1 && hash2 != -1) {
-                goto return_ne;
-            }
-        }
-#endif
-        kind = __Pyx_PyUnicode_KIND(s1);
-        if (kind != __Pyx_PyUnicode_KIND(s2)) {
-            goto return_ne;
-        }
-        data1 = __Pyx_PyUnicode_DATA(s1);
-        data2 = __Pyx_PyUnicode_DATA(s2);
-        if (__Pyx_PyUnicode_READ(kind, data1, 0) != __Pyx_PyUnicode_READ(kind, data2, 0)) {
-            goto return_ne;
-        } else if (length == 1) {
-            goto return_eq;
-        } else {
-            int result = memcmp(data1, data2, (size_t)(length * kind));
-            #if PY_MAJOR_VERSION < 3
-            Py_XDECREF(owned_ref);
-            #endif
-            return (equals == Py_EQ) ? (result == 0) : (result != 0);
-        }
-    } else if ((s1 == Py_None) & s2_is_unicode) {
-        goto return_ne;
-    } else if ((s2 == Py_None) & s1_is_unicode) {
-        goto return_ne;
-    } else {
-        int result;
-        PyObject* py_result = PyObject_RichCompare(s1, s2, equals);
-        #if PY_MAJOR_VERSION < 3
-        Py_XDECREF(owned_ref);
-        #endif
-        if (!py_result)
-            return -1;
-        result = __Pyx_PyObject_IsTrue(py_result);
-        Py_DECREF(py_result);
-        return result;
-    }
-return_eq:
-    #if PY_MAJOR_VERSION < 3
-    Py_XDECREF(owned_ref);
-    #endif
-    return (equals == Py_EQ);
-return_ne:
-    #if PY_MAJOR_VERSION < 3
-    Py_XDECREF(owned_ref);
-    #endif
-    return (equals == Py_NE);
-#endif
-}
-
-/* PyErrFetchRestore */
-#if CYTHON_FAST_THREAD_STATE
-static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
-    PyObject *tmp_type, *tmp_value, *tmp_tb;
-    tmp_type = tstate->curexc_type;
-    tmp_value = tstate->curexc_value;
-    tmp_tb = tstate->curexc_traceback;
-    tstate->curexc_type = type;
-    tstate->curexc_value = value;
-    tstate->curexc_traceback = tb;
-    Py_XDECREF(tmp_type);
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(tmp_tb);
-}
-static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
-    *type = tstate->curexc_type;
-    *value = tstate->curexc_value;
-    *tb = tstate->curexc_traceback;
-    tstate->curexc_type = 0;
-    tstate->curexc_value = 0;
-    tstate->curexc_traceback = 0;
-}
-#endif
-
-/* WriteUnraisableException */
-static void __Pyx_WriteUnraisable(const char *name, CYTHON_UNUSED int clineno,
-                                  CYTHON_UNUSED int lineno, CYTHON_UNUSED const char *filename,
-                                  int full_traceback, CYTHON_UNUSED int nogil) {
-    PyObject *old_exc, *old_val, *old_tb;
-    PyObject *ctx;
-    __Pyx_PyThreadState_declare
-#ifdef WITH_THREAD
-    PyGILState_STATE state;
-    if (nogil)
-        state = PyGILState_Ensure();
-    else state = (PyGILState_STATE)0;
-#endif
-    __Pyx_PyThreadState_assign
-    __Pyx_ErrFetch(&old_exc, &old_val, &old_tb);
-    if (full_traceback) {
-        Py_XINCREF(old_exc);
-        Py_XINCREF(old_val);
-        Py_XINCREF(old_tb);
-        __Pyx_ErrRestore(old_exc, old_val, old_tb);
-        PyErr_PrintEx(1);
-    }
-    #if PY_MAJOR_VERSION < 3
-    ctx = PyString_FromString(name);
-    #else
-    ctx = PyUnicode_FromString(name);
-    #endif
-    __Pyx_ErrRestore(old_exc, old_val, old_tb);
-    if (!ctx) {
-        PyErr_WriteUnraisable(Py_None);
-    } else {
-        PyErr_WriteUnraisable(ctx);
-        Py_DECREF(ctx);
-    }
-#ifdef WITH_THREAD
-    if (nogil)
-        PyGILState_Release(state);
-#endif
-}
-
 /* RaiseArgTupleInvalid */
 static void __Pyx_RaiseArgtupleInvalid(
     const char* func_name,
     int exact,
     Py_ssize_t num_min,
     Py_ssize_t num_max,
     Py_ssize_t num_found)
@@ -3610,14 +3267,163 @@
     if (is_list || PySequence_Check(o)) {
         return PySequence_GetItem(o, i);
     }
 #endif
     return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
 }
 
+/* BytesEquals */
+static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals) {
+#if CYTHON_COMPILING_IN_PYPY
+    return PyObject_RichCompareBool(s1, s2, equals);
+#else
+    if (s1 == s2) {
+        return (equals == Py_EQ);
+    } else if (PyBytes_CheckExact(s1) & PyBytes_CheckExact(s2)) {
+        const char *ps1, *ps2;
+        Py_ssize_t length = PyBytes_GET_SIZE(s1);
+        if (length != PyBytes_GET_SIZE(s2))
+            return (equals == Py_NE);
+        ps1 = PyBytes_AS_STRING(s1);
+        ps2 = PyBytes_AS_STRING(s2);
+        if (ps1[0] != ps2[0]) {
+            return (equals == Py_NE);
+        } else if (length == 1) {
+            return (equals == Py_EQ);
+        } else {
+            int result;
+#if CYTHON_USE_UNICODE_INTERNALS && (PY_VERSION_HEX < 0x030B0000)
+            Py_hash_t hash1, hash2;
+            hash1 = ((PyBytesObject*)s1)->ob_shash;
+            hash2 = ((PyBytesObject*)s2)->ob_shash;
+            if (hash1 != hash2 && hash1 != -1 && hash2 != -1) {
+                return (equals == Py_NE);
+            }
+#endif
+            result = memcmp(ps1, ps2, (size_t)length);
+            return (equals == Py_EQ) ? (result == 0) : (result != 0);
+        }
+    } else if ((s1 == Py_None) & PyBytes_CheckExact(s2)) {
+        return (equals == Py_NE);
+    } else if ((s2 == Py_None) & PyBytes_CheckExact(s1)) {
+        return (equals == Py_NE);
+    } else {
+        int result;
+        PyObject* py_result = PyObject_RichCompare(s1, s2, equals);
+        if (!py_result)
+            return -1;
+        result = __Pyx_PyObject_IsTrue(py_result);
+        Py_DECREF(py_result);
+        return result;
+    }
+#endif
+}
+
+/* UnicodeEquals */
+static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals) {
+#if CYTHON_COMPILING_IN_PYPY
+    return PyObject_RichCompareBool(s1, s2, equals);
+#else
+#if PY_MAJOR_VERSION < 3
+    PyObject* owned_ref = NULL;
+#endif
+    int s1_is_unicode, s2_is_unicode;
+    if (s1 == s2) {
+        goto return_eq;
+    }
+    s1_is_unicode = PyUnicode_CheckExact(s1);
+    s2_is_unicode = PyUnicode_CheckExact(s2);
+#if PY_MAJOR_VERSION < 3
+    if ((s1_is_unicode & (!s2_is_unicode)) && PyString_CheckExact(s2)) {
+        owned_ref = PyUnicode_FromObject(s2);
+        if (unlikely(!owned_ref))
+            return -1;
+        s2 = owned_ref;
+        s2_is_unicode = 1;
+    } else if ((s2_is_unicode & (!s1_is_unicode)) && PyString_CheckExact(s1)) {
+        owned_ref = PyUnicode_FromObject(s1);
+        if (unlikely(!owned_ref))
+            return -1;
+        s1 = owned_ref;
+        s1_is_unicode = 1;
+    } else if (((!s2_is_unicode) & (!s1_is_unicode))) {
+        return __Pyx_PyBytes_Equals(s1, s2, equals);
+    }
+#endif
+    if (s1_is_unicode & s2_is_unicode) {
+        Py_ssize_t length;
+        int kind;
+        void *data1, *data2;
+        if (unlikely(__Pyx_PyUnicode_READY(s1) < 0) || unlikely(__Pyx_PyUnicode_READY(s2) < 0))
+            return -1;
+        length = __Pyx_PyUnicode_GET_LENGTH(s1);
+        if (length != __Pyx_PyUnicode_GET_LENGTH(s2)) {
+            goto return_ne;
+        }
+#if CYTHON_USE_UNICODE_INTERNALS
+        {
+            Py_hash_t hash1, hash2;
+        #if CYTHON_PEP393_ENABLED
+            hash1 = ((PyASCIIObject*)s1)->hash;
+            hash2 = ((PyASCIIObject*)s2)->hash;
+        #else
+            hash1 = ((PyUnicodeObject*)s1)->hash;
+            hash2 = ((PyUnicodeObject*)s2)->hash;
+        #endif
+            if (hash1 != hash2 && hash1 != -1 && hash2 != -1) {
+                goto return_ne;
+            }
+        }
+#endif
+        kind = __Pyx_PyUnicode_KIND(s1);
+        if (kind != __Pyx_PyUnicode_KIND(s2)) {
+            goto return_ne;
+        }
+        data1 = __Pyx_PyUnicode_DATA(s1);
+        data2 = __Pyx_PyUnicode_DATA(s2);
+        if (__Pyx_PyUnicode_READ(kind, data1, 0) != __Pyx_PyUnicode_READ(kind, data2, 0)) {
+            goto return_ne;
+        } else if (length == 1) {
+            goto return_eq;
+        } else {
+            int result = memcmp(data1, data2, (size_t)(length * kind));
+            #if PY_MAJOR_VERSION < 3
+            Py_XDECREF(owned_ref);
+            #endif
+            return (equals == Py_EQ) ? (result == 0) : (result != 0);
+        }
+    } else if ((s1 == Py_None) & s2_is_unicode) {
+        goto return_ne;
+    } else if ((s2 == Py_None) & s1_is_unicode) {
+        goto return_ne;
+    } else {
+        int result;
+        PyObject* py_result = PyObject_RichCompare(s1, s2, equals);
+        #if PY_MAJOR_VERSION < 3
+        Py_XDECREF(owned_ref);
+        #endif
+        if (!py_result)
+            return -1;
+        result = __Pyx_PyObject_IsTrue(py_result);
+        Py_DECREF(py_result);
+        return result;
+    }
+return_eq:
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(owned_ref);
+    #endif
+    return (equals == Py_EQ);
+return_ne:
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(owned_ref);
+    #endif
+    return (equals == Py_NE);
+#endif
+}
+
 /* PyObjectCall */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
     PyObject *result;
     ternaryfunc call = Py_TYPE(func)->tp_call;
     if (unlikely(!call))
         return PyObject_Call(func, arg, kw);
@@ -3813,14 +3619,38 @@
     PyObject *dict = Py_TYPE(obj)->tp_dict;
     if (unlikely(!dict) || unlikely(tp_dict_version != __PYX_GET_DICT_VERSION(dict)))
         return 0;
     return obj_dict_version == __Pyx_get_object_dict_version(obj);
 }
 #endif
 
+/* PyErrFetchRestore */
+#if CYTHON_FAST_THREAD_STATE
+static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+    tmp_type = tstate->curexc_type;
+    tmp_value = tstate->curexc_value;
+    tmp_tb = tstate->curexc_traceback;
+    tstate->curexc_type = type;
+    tstate->curexc_value = value;
+    tstate->curexc_traceback = tb;
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
+}
+static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
+    *type = tstate->curexc_type;
+    *value = tstate->curexc_value;
+    *tb = tstate->curexc_traceback;
+    tstate->curexc_type = 0;
+    tstate->curexc_value = 0;
+    tstate->curexc_traceback = 0;
+}
+#endif
+
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
 static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
@@ -4261,52 +4091,14 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to char");
     return (char) -1;
 }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const int neg_one = (int) -1, const_zero = (int) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(int) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(int) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(int) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(int),
-                                     little, !is_unsigned);
-    }
-}
-
-/* CIntToPy */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_char(char value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const char neg_one = (char) -1, const_zero = (char) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
```

### Comparing `tarina-0.3.0/src/tarina/_string_c.pyi` & `tarina-0.3.1/src/tarina/_string_c.pyi`

 * *Files identical despite different names*

### Comparing `tarina-0.3.0/src/tarina/_string_c.pyx` & `tarina-0.3.1/src/tarina/_string_c.pyx`

 * *Files 6% similar despite different names*

```diff
@@ -6,26 +6,17 @@
 from cpython.unicode cimport PyUnicode_Join, PyUnicode_Split, PyUnicode_GET_LENGTH
 from cpython.list cimport PyList_Append, PyList_SET_ITEM
 
 cdef extern from "Python.h":
     Py_UCS4 PyUnicode_READ_CHAR(object s, Py_ssize_t i)
 
 cdef extern from "_op.h":
-    PyObject* tupleitem(object a, Py_ssize_t i)
+    bint contains(object chs, Py_UCS4 ch)
     bint set_contains_key(object anyset, object key) except -1
 
-cdef inline int contains(tuple chs, Py_UCS4 ch):
-    cdef Py_ssize_t i = 0
-    cdef Py_ssize_t length = Py_SIZE(chs)
-    while i < length:
-        if ch == <object>tupleitem(chs, i):
-            return 1
-        i += 1
-    return 0
-
 cdef set QUOTES = {'"', '\''}
 cdef set CRLF = {'\r', '\n'}
 
 def split(str text, tuple separates, char crlf=True):
     """尊重引号与转义的字符串切分
 
     Args:
```

### Comparing `tarina-0.3.0/src/tarina/_string_py.py` & `tarina-0.3.1/src/tarina/_string_py.py`

 * *Files identical despite different names*

### Comparing `tarina-0.3.0/src/tarina/context.py` & `tarina-0.3.1/src/tarina/context.py`

 * *Files identical despite different names*

### Comparing `tarina-0.3.0/src/tarina/generic.py` & `tarina-0.3.1/src/tarina/generic.py`

 * *Files identical despite different names*

### Comparing `tarina-0.3.0/src/tarina/guard.py` & `tarina-0.3.1/src/tarina/guard.py`

 * *Files identical despite different names*

### Comparing `tarina-0.3.0/src/tarina/lang.py` & `tarina-0.3.1/src/tarina/lang.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,129 +5,181 @@
 import json
 
 root_dir: Final[Path] = Path(__file__).parent / "i18n"
 
 
 def _get_config(root: Path) -> dict[str, Any]:
     if not (root / ".config.json").exists():
-        raise FileNotFoundError("Config file not found")
+        return {}
     with (root / ".config.json").open("r", encoding="utf-8") as f:
         return json.load(f)
 
 
-def _get_types(root: Path) -> list[str]:
-    return [i.stem for i in root.iterdir() if i.is_file() and not i.name.startswith(".")]
+def _get_scopes(root: Path) -> list[str]:
+    return [
+        i.stem for i in root.iterdir() if i.is_file() and not i.name.startswith(".")
+    ]
 
 
 def _get_lang(root: Path, _type: str) -> dict[str, dict[str, str]]:
     with (root / f"{_type}.json").open("r", encoding="utf-8") as f:
         return json.load(f)
 
 
 def merge(source: dict, target: dict, ignore: list[str] | None = None) -> dict:
     ignore = ignore or []
     for key, value in source.items():
+        if key in target and key in ignore:
+            continue
         if isinstance(value, dict):
             target[key] = merge(value, target.get(key, {}))
         elif isinstance(value, list):
             target[key] = value + target.get(key, [])
-        elif key in ignore:
-            continue
         else:
             target[key] = value
     return target
 
 
 @final
 class _LangConfig:
-
     def __init__(self):
         __config = _get_config(root_dir)
         self.__scope: str = __config["default"]
-        self.__immutable: list[str] = __config["immutable"]
-        self.__types = _get_types(root_dir)
-        self.__langs = {t: _get_lang(root_dir, t) for t in self.__types}
+        self.__frozen: list[str] = __config["frozen"]
+        self.__require: list[str] = __config["require"]
+        self.__scopes = _get_scopes(root_dir)
+        self.__langs = {t: _get_lang(root_dir, t) for t in self.__scopes}
 
     @property
-    def types(self):
-        return self.__types
+    def scopes(self):
+        return self.__scopes
 
     def scope(self, item: str) -> Self:
         if item not in self.__langs:
-            raise ValueError(
-                self.__langs[self.__scope]["lang"]["scope_error"].format(target=item)
-            )
+            raise ValueError(self.require("lang", "scope_error").format(target=item))
         self.__scope = item
         return self
 
-    def save(self):
-        config = _get_config(root_dir)
+    def save(self, root: Path | None = None):
+        _root = root or root_dir
+        config = _get_config(_root)
         config["default"] = self.__scope
-        with (root_dir / ".config.json").open("w", encoding="utf-8") as f:
+        with (_root / ".config.json").open("w+", encoding="utf-8") as f:
             json.dump(config, f, ensure_ascii=False, indent=2)
 
     def __getattr__(self, item: str):
         _lang = self.__langs[self.__scope]
         if item not in _lang:
             raise ValueError(
-                _lang["lang"]["type_error"].format(target=item)
+                _lang["lang"]["type_error"].format(target=item, scope=self.__scope)
             )
 
         class _getter:
-            def __init__(self, prefix: str):
-                self.prefix = prefix
+            def __init__(_self, prefix: str):
+                _self.prefix = prefix
 
         def __getattr__(_self, _item: str):
             _config = _lang[_self.prefix]
             if not _config.get(_item):
-                raise AttributeError(_lang["lang"]["name_error"].format(target=_item))
+                raise AttributeError(
+                    _lang["lang"]["name_error"].format(
+                        target=_item, scope=self.__scope, type=_self.prefix
+                    )
+                )
             return _config[_item]
 
-        return type(f"{self.__scope}_{item}_getter", (_getter,), {"__getattr__": __getattr__})(item)
+        return type(
+            f"{self.__scope}_{item}_getter", (_getter,), {"__getattr__": __getattr__}
+        )(item)
+
+    def load_file(self, filepath: Path):
+        _type = filepath.stem
+        if _type in self.__scopes:
+            self.__langs[_type] = merge(
+                _get_lang(filepath.parent, _type), self.__langs[_type], self.__frozen
+            )
+        else:
+            self.__scopes.append(_type)
+            self.__langs[_type] = _get_lang(filepath.parent, _type)
+        for key in self.__require:
+            t, n = key.split(".", 1)
+            if t not in self.__langs[_type]:
+                raise KeyError(
+                    self.require("lang", "miss_require_type", _type).format(
+                        scope=_type, target=t
+                    )
+                )
+            if n and n not in self.__langs[_type][t]:
+                raise KeyError(
+                    self.require("lang", "miss_require_name", _type).format(
+                        scope=_type, type=t, target=n
+                    )
+                )
 
     def load(self, root: Path):
         config = _get_config(root)
-        self.__scope = config["default"]
-        self.__immutable.extend(config.get("immutable", []))
-        _types = _get_types(root)
-        for t in _types:
-            if t in self.__types:
-                self.__langs[t] = merge(_get_lang(root, t), self.__langs[t], self.__immutable)
-            else:
-                self.__types.append(t)
-                self.__langs[t] = _get_lang(root, t)
+        self.__scope = config.get("default", self.__scope)
+        self.__frozen.extend(config.get("frozen", []))
+        self.__require.extend(config.get("require", []))
+        for i in root.iterdir():
+            if i.is_file() and not i.name.startswith("."):
+                continue
+            self.load_file(i)
 
     def require(self, _type: str, _name: str, scope: str | None = None) -> str:
         scope = scope or self.__scope
         if scope not in self.__langs:
-            raise ValueError(self.__langs[self.__scope]["lang"]["scope_error"].format(target=scope))
-        if _type not in self.__langs[scope]:
-            raise ValueError(self.__langs[scope]["lang"]["type_error"].format(target=_type))
-        if not self.__langs[scope][_type].get(_name):
-            raise ValueError(self.__langs[scope]["lang"]["name_error"].format(target=_name))
-        return self.__langs[scope][_type][_name]
+            raise ValueError(
+                self.__langs[self.__scope]["lang"]["scope_error"].format(target=scope)
+            )
+        if _type in self.__langs[scope]:
+            _types = self.__langs[scope][_type]
+        elif _type in self.__langs[self.__scope]:
+            _types = self.__langs[self.__scope][_type]
+        else:
+            raise ValueError(
+                self.__langs[scope]["lang"]["type_error"].format(
+                    target=_type, scope=scope
+                )
+            )
+        if _name in _types:
+            return _types[_name]
+        elif _name in self.__langs[self.__scope][_type]:
+            return self.__langs[self.__scope][_type][_name]
+        else:
+            raise ValueError(
+                self.__langs[scope]["lang"]["name_error"].format(
+                    target=_name, scope=scope, type=_type
+                )
+            )
 
     def set(self, _type: str, _name: str, content: str, scope: str | None = None):
         scope = scope or self.__scope
         if scope not in self.__langs:
-            raise ValueError(self.__langs[self.__scope]["lang"]["scope_error"].format(target=scope))
-        if _type in self.__immutable:
-            raise ValueError(self.__langs[scope]["lang"]["type_error"].format(target=_type))
+            raise ValueError(
+                self.__langs[self.__scope]["lang"]["scope_error"].format(target=scope)
+            )
+        if _type in self.__frozen:
+            raise ValueError(
+                self.__langs[scope]["lang"]["type_error"].format(
+                    target=_type, scope=scope
+                )
+            )
         self.__langs[scope].setdefault(_type, {})[_name] = content
 
     def __repr__(self):
         return f"<LangConfig: {self.__scope}>"
 
 
 lang: _LangConfig = _LangConfig()
 
 __all__ = ["lang"]
 
-if __name__ == '__main__':
-    print(lang.types)
+if __name__ == "__main__":
+    print(lang.scopes)
     print(lang.lang.name_error)
     print(lang.require("lang", "name_error"))
     print(lang.require("lang", "name_error", "en-US"))
     print(lang.scope("en-US"))
     print(lang.lang.name_error)
     print(lang.lang.type_error)
     print(lang.lang.scope_error)
```

### Comparing `tarina-0.3.0/src/tarina/lru.pyi` & `tarina-0.3.1/src/tarina/lru.pyi`

 * *Files identical despite different names*

### Comparing `tarina-0.3.0/src/tarina/signature.py` & `tarina-0.3.1/src/tarina/signature.py`

 * *Files identical despite different names*

### Comparing `tarina-0.3.0/src/tarina/string.py` & `tarina-0.3.1/src/tarina/string.py`

 * *Files identical despite different names*

### Comparing `tarina-0.3.0/src/tarina/tools.py` & `tarina-0.3.1/src/tarina/tools.py`

 * *Files identical despite different names*

### Comparing `tarina-0.3.0/src/tarina.egg-info/PKG-INFO` & `tarina-0.3.1/src/tarina.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tarina
-Version: 0.3.0
+Version: 0.3.1
 Summary: A collection of common utils for Arclet
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `tarina-0.3.0/src/tarina.egg-info/SOURCES.txt` & `tarina-0.3.1/src/tarina.egg-info/SOURCES.txt`

 * *Files identical despite different names*

