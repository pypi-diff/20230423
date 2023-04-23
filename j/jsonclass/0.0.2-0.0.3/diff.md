# Comparing `tmp/jsonclass-0.0.2.tar.gz` & `tmp/jsonclass-0.0.3.tar.gz`

## Comparing `jsonclass-0.0.2.tar` & `jsonclass-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 jsonclass-0.0.2/build.sh
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 jsonclass-0.0.2/src/jsonclass.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 jsonclass-0.0.2/tests/test.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 jsonclass-0.0.2/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 jsonclass-0.0.2/LICENSE
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 jsonclass-0.0.2/README.md
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 jsonclass-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 jsonclass-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 jsonclass-0.0.3/build.sh
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 jsonclass-0.0.3/src/jsonclass.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 jsonclass-0.0.3/tests/test.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 jsonclass-0.0.3/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 jsonclass-0.0.3/LICENSE
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 jsonclass-0.0.3/README.md
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 jsonclass-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 jsonclass-0.0.3/PKG-INFO
```

### Comparing `jsonclass-0.0.2/src/jsonclass.py` & `jsonclass-0.0.3/src/jsonclass.py`

 * *Files identical despite different names*

### Comparing `jsonclass-0.0.2/.gitignore` & `jsonclass-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `jsonclass-0.0.2/LICENSE` & `jsonclass-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonclass-0.0.2/pyproject.toml` & `jsonclass-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jsonclass"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="soundagain2", email="soundagain2@proton.me" },
 ]
 description = "Convert json to object and back in Python."
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

### Comparing `jsonclass-0.0.2/PKG-INFO` & `jsonclass-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonclass
-Version: 0.0.2
+Version: 0.0.3
 Summary: Convert json to object and back in Python.
 Project-URL: Homepage, https://github.com/soundagain2/jsonclass
 Project-URL: Bug Tracker, https://github.com/soundagain2/jsonclass/issues
 Author-email: soundagain2 <soundagain2@proton.me>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

