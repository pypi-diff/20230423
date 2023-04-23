# Comparing `tmp/pyram_mogus-0.0.1.tar.gz` & `tmp/pyram_mogus-0.0.2.tar.gz`

## Comparing `pyram_mogus-0.0.1.tar` & `pyram_mogus-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyram_mogus-0.0.1/src/pyram_mogus/__init__.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pyram_mogus-0.0.1/src/pyram_mogus/pyram.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pyram_mogus-0.0.1/LICENSE
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 pyram_mogus-0.0.1/README.md
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 pyram_mogus-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 pyram_mogus-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyram_mogus-0.0.2/src/pyram_mogus/__init__.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pyram_mogus-0.0.2/src/pyram_mogus/pyram.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pyram_mogus-0.0.2/LICENSE
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 pyram_mogus-0.0.2/README.md
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 pyram_mogus-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 pyram_mogus-0.0.2/PKG-INFO
```

### Comparing `pyram_mogus-0.0.1/LICENSE` & `pyram_mogus-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyram_mogus-0.0.1/pyproject.toml` & `pyram_mogus-0.0.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyram_mogus"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Example Author", email="author@example.com" },
 ]
-description = "A small example package to take up ram"
+description = "A small package to take up ram"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `pyram_mogus-0.0.1/PKG-INFO` & `pyram_mogus-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: pyram_mogus
-Version: 0.0.1
-Summary: A small example package to take up ram
+Version: 0.0.2
+Summary: A small package to take up ram
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Example Author <author@example.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 USAGE:
+
 var_name = pyram(value_in_gb)
 
+
 eg.:
+
 from pyram_mogus.pyram import pyram
 a = pyram(4)
```

