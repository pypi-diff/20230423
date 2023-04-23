# Comparing `tmp/triade-0.1.tar.gz` & `tmp/triade-0.1.1.tar.gz`

## Comparing `triade-0.1.tar` & `triade-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 triade-0.1/CHANGELOG.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 triade-0.1/triade/__init__.py
--rwxr-xr-x   0        0        0     2109 2020-02-02 00:00:00.000000 triade-0.1/triade/cli.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 triade-0.1/triade/lib.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 triade-0.1/.gitignore
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 triade-0.1/README.md
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 triade-0.1/pyproject.toml
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 triade-0.1/PKG-INFO
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 triade-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 triade-0.1.1/triade/__init__.py
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 triade-0.1.1/triade/cli.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 triade-0.1.1/triade/lib.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 triade-0.1.1/.gitignore
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 triade-0.1.1/README.md
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 triade-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 triade-0.1.1/PKG-INFO
```

### Comparing `triade-0.1/triade/cli.py` & `triade-0.1.1/triade/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-#!/usr/bin/env python3
 import sys
 import argparse
 
-from lib import parse, write
+from triade.lib import parse, write
 
 
 FORMAT_LIST = ["json", "yaml", "toml"]
 
 
 def main():
     parser = argparse.ArgumentParser()
@@ -51,19 +50,16 @@
 
     input_data = input_file.read()
 
     if output_format is None:
         output_data = parse(input_data, input_format)
     elif output_ext is not None and output_format not in FORMAT_LIST:
         output_data = parse(input_data, input_format)
-        print("Warning")
+        print("Warning: the output file's format is not recognized. Defaulting to object as standard format.",
+              file=sys.stderr)
     else:
         parsed_data = parse(input_data, input_format)
         output_data = write(parsed_data, output_format)
 
     print(output_data, file=output_file)
 
     return 0
-
-
-if __name__ == "__main__":
-    sys.exit(main())
```

### Comparing `triade-0.1/triade/lib.py` & `triade-0.1.1/triade/lib.py`

 * *Files identical despite different names*

### Comparing `triade-0.1/pyproject.toml` & `triade-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "Makefile",
     "dev_requirements.txt",
     ".?*",
 ]
 
 [project]
 name = "triade"
-version = "0.1"
+version = "0.1.1"
 authors = [
   { name="Lucas L. S. Haine", email="lucaslshaine@gmail.com" },
 ]
 description = ""
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `triade-0.1/PKG-INFO` & `triade-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: triade
-Version: 0.1
+Version: 0.1.1
 Project-URL: Homepage, https://github.com/llucasls/triade
 Author-email: "Lucas L. S. Haine" <lucaslshaine@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: pyyaml
```

