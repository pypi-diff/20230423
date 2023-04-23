# Comparing `tmp/jsonclass-0.0.3.tar.gz` & `tmp/jsonclass-0.0.5.tar.gz`

## Comparing `jsonclass-0.0.3.tar` & `jsonclass-0.0.5.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 jsonclass-0.0.3/build.sh
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 jsonclass-0.0.3/src/jsonclass.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 jsonclass-0.0.3/tests/test.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 jsonclass-0.0.3/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 jsonclass-0.0.3/LICENSE
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 jsonclass-0.0.3/README.md
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 jsonclass-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 jsonclass-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jsonclass-0.0.5/test.sh
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 jsonclass-0.0.5/test_upload.sh
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 jsonclass-0.0.5/upload.sh
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 jsonclass-0.0.5/src/jsonclass.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 jsonclass-0.0.5/tests/test.py
+-rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 jsonclass-0.0.5/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 jsonclass-0.0.5/LICENSE
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 jsonclass-0.0.5/README.md
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 jsonclass-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 jsonclass-0.0.5/PKG-INFO
```

### Comparing `jsonclass-0.0.3/src/jsonclass.py` & `jsonclass-0.0.5/src/jsonclass.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,16 +7,15 @@
     __json_data: Dict
 
     def __init_subclass__(cls):
         object.__init_subclass__()
         _json_classes[cls.__qualname__] = cls
 
     def __new__(cls, data: Dict[str, Any] = None):
-        __data = data or {}
-        __data["__json_class__"] = cls.__qualname__
+        __data = data or {"__json_class__": cls.__qualname__}
         __instance = object.__new__(_json_classes[__data["__json_class__"]])
         object.__setattr__(__instance, "__json_data", __data)
         return __instance
 
     def __getattr__(self, item):
         return object.__getattribute__(self, "__json_data")[item]
```

### Comparing `jsonclass-0.0.3/.gitignore` & `jsonclass-0.0.5/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+.idea/
+
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
```

### Comparing `jsonclass-0.0.3/LICENSE` & `jsonclass-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonclass-0.0.3/pyproject.toml` & `jsonclass-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jsonclass"
-version = "0.0.3"
+version = "0.0.5"
 authors = [
   { name="soundagain2", email="soundagain2@proton.me" },
 ]
 description = "Convert json to object and back in Python."
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

### Comparing `jsonclass-0.0.3/PKG-INFO` & `jsonclass-0.0.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonclass
-Version: 0.0.3
+Version: 0.0.5
 Summary: Convert json to object and back in Python.
 Project-URL: Homepage, https://github.com/soundagain2/jsonclass
 Project-URL: Bug Tracker, https://github.com/soundagain2/jsonclass/issues
 Author-email: soundagain2 <soundagain2@proton.me>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

