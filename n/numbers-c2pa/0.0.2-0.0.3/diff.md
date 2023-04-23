# Comparing `tmp/numbers-c2pa-0.0.2.tar.gz` & `tmp/numbers-c2pa-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/numbers-c2pa/numbers-c2pa/dist/.tmp-n5lvkac2/numbers-c2pa-0.0.2.tar", last modified: Fri Apr 21 13:26:03 2023, max compression
+gzip compressed data, was "/home/runner/work/numbers-c2pa/numbers-c2pa/dist/.tmp-5xsw33ey/numbers-c2pa-0.0.3.tar", last modified: Sun Apr 23 18:23:09 2023, max compression
```

## Comparing `numbers-c2pa-0.0.2.tar` & `numbers-c2pa-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:26:03.000000 numbers-c2pa-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-21 13:25:51.000000 numbers-c2pa-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-04-21 13:26:03.000000 numbers-c2pa-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-04-21 13:25:51.000000 numbers-c2pa-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-21 13:25:51.000000 numbers-c2pa-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-21 13:26:03.000000 numbers-c2pa-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-21 13:25:51.000000 numbers-c2pa-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:26:03.000000 numbers-c2pa-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:26:03.000000 numbers-c2pa-0.0.2/src/numbers_c2pa/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-21 13:25:51.000000 numbers-c2pa-0.0.2/src/numbers_c2pa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-04-21 13:25:51.000000 numbers-c2pa-0.0.2/src/numbers_c2pa/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-21 13:25:51.000000 numbers-c2pa-0.0.2/src/numbers_c2pa/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:26:03.000000 numbers-c2pa-0.0.2/src/numbers_c2pa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-04-21 13:26:03.000000 numbers-c2pa-0.0.2/src/numbers_c2pa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-21 13:26:03.000000 numbers-c2pa-0.0.2/src/numbers_c2pa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 13:26:03.000000 numbers-c2pa-0.0.2/src/numbers_c2pa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-21 13:26:03.000000 numbers-c2pa-0.0.2/src/numbers_c2pa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-21 13:26:03.000000 numbers-c2pa-0.0.2/src/numbers_c2pa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 13:26:02.000000 numbers-c2pa-0.0.2/src/numbers_c2pa.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:26:03.000000 numbers-c2pa-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-21 13:25:51.000000 numbers-c2pa-0.0.2/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:23:09.000000 numbers-c2pa-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-23 18:22:57.000000 numbers-c2pa-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-04-23 18:23:09.000000 numbers-c2pa-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-04-23 18:22:57.000000 numbers-c2pa-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-23 18:22:57.000000 numbers-c2pa-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-23 18:23:09.000000 numbers-c2pa-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-23 18:22:57.000000 numbers-c2pa-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:23:09.000000 numbers-c2pa-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:23:09.000000 numbers-c2pa-0.0.3/src/numbers_c2pa/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-23 18:22:57.000000 numbers-c2pa-0.0.3/src/numbers_c2pa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-04-23 18:22:57.000000 numbers-c2pa-0.0.3/src/numbers_c2pa/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-23 18:22:57.000000 numbers-c2pa-0.0.3/src/numbers_c2pa/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:23:09.000000 numbers-c2pa-0.0.3/src/numbers_c2pa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-04-23 18:23:09.000000 numbers-c2pa-0.0.3/src/numbers_c2pa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-23 18:23:09.000000 numbers-c2pa-0.0.3/src/numbers_c2pa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 18:23:09.000000 numbers-c2pa-0.0.3/src/numbers_c2pa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-23 18:23:09.000000 numbers-c2pa-0.0.3/src/numbers_c2pa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-23 18:23:09.000000 numbers-c2pa-0.0.3/src/numbers_c2pa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 18:23:08.000000 numbers-c2pa-0.0.3/src/numbers_c2pa.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:23:09.000000 numbers-c2pa-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-23 18:22:57.000000 numbers-c2pa-0.0.3/tests/test_core.py
```

### Comparing `numbers-c2pa-0.0.2/LICENSE` & `numbers-c2pa-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `numbers-c2pa-0.0.2/PKG-INFO` & `numbers-c2pa-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numbers-c2pa
-Version: 0.0.2
+Version: 0.0.3
 Summary: Numbers C2PA tool
 Home-page: https://github.com/numbersprotocol/numbers-c2pa
 Author: Numbers Co., Inc
 Author-email: dev@numbersprotocol.io
 Keywords: authenticity
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `numbers-c2pa-0.0.2/README.md` & `numbers-c2pa-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `numbers-c2pa-0.0.2/setup.cfg` & `numbers-c2pa-0.0.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = numbers-c2pa
-version = 0.0.2
+version = 0.0.3
 author = Numbers Co., Inc
 author_email = dev@numbersprotocol.io
 description = Numbers C2PA tool
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = authenticity
 url = https://github.com/numbersprotocol/numbers-c2pa
```

### Comparing `numbers-c2pa-0.0.2/src/numbers_c2pa/core.py` & `numbers-c2pa-0.0.3/src/numbers_c2pa/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
         manifest_temp_file.flush()
 
         env_vars = os.environ.copy()
         if private_key:
             env_vars['C2PA_PRIVATE_KEY'] = private_key
         if sign_cert:
             env_vars['C2PA_SIGN_CERT'] = sign_cert
-        command = f'c2patool {asset_file} -m {manifest_temp_file} -o {c2pa_output_file}'
+        command = f'c2patool {asset_file} -m {manifest_temp_file.name} -o {c2pa_output_file}'
         if force_overwrite:
             command += ' -f'
         subprocess.run(
             command,
             shell=True,
             env=env_vars,
             check=True,
```

### Comparing `numbers-c2pa-0.0.2/src/numbers_c2pa/utils.py` & `numbers-c2pa-0.0.3/src/numbers_c2pa/utils.py`

 * *Files identical despite different names*

### Comparing `numbers-c2pa-0.0.2/src/numbers_c2pa.egg-info/PKG-INFO` & `numbers-c2pa-0.0.3/src/numbers_c2pa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numbers-c2pa
-Version: 0.0.2
+Version: 0.0.3
 Summary: Numbers C2PA tool
 Home-page: https://github.com/numbersprotocol/numbers-c2pa
 Author: Numbers Co., Inc
 Author-email: dev@numbersprotocol.io
 Keywords: authenticity
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

