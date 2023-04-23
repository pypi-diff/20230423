# Comparing `tmp/py-sls-lambda-toolkit-0.0.2.tar.gz` & `tmp/py-sls-lambda-toolkit-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-sls-lambda-toolkit-0.0.2.tar", last modified: Sun Apr 23 18:15:01 2023, max compression
+gzip compressed data, was "py-sls-lambda-toolkit-0.0.3.tar", last modified: Sun Apr 23 18:26:19 2023, max compression
```

## Comparing `py-sls-lambda-toolkit-0.0.2.tar` & `py-sls-lambda-toolkit-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 julio     (1000) julio     (1000)        0 2023-04-23 18:15:01.537016 py-sls-lambda-toolkit-0.0.2/
--rw-rw-r--   0 julio     (1000) julio     (1000)     1069 2023-04-23 17:34:15.000000 py-sls-lambda-toolkit-0.0.2/LICENSE
--rw-rw-r--   0 julio     (1000) julio     (1000)       34 2023-04-23 18:05:48.000000 py-sls-lambda-toolkit-0.0.2/MANIFEST.in
--rw-rw-r--   0 julio     (1000) julio     (1000)      762 2023-04-23 18:15:01.537016 py-sls-lambda-toolkit-0.0.2/PKG-INFO
-drwxrwxr-x   0 julio     (1000) julio     (1000)        0 2023-04-23 18:15:01.533016 py-sls-lambda-toolkit-0.0.2/py_sls_lambda_toolkit/
--rw-rw-r--   0 julio     (1000) julio     (1000)        0 2023-04-23 17:11:35.000000 py-sls-lambda-toolkit-0.0.2/py_sls_lambda_toolkit/__init__.py
--rw-rw-r--   0 julio     (1000) julio     (1000)     1370 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.0.2/py_sls_lambda_toolkit/dynamodb_shortcuts.py
--rw-rw-r--   0 julio     (1000) julio     (1000)     1651 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.0.2/py_sls_lambda_toolkit/http_event.py
--rw-rw-r--   0 julio     (1000) julio     (1000)     1222 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.0.2/py_sls_lambda_toolkit/http_response.py
--rw-rw-r--   0 julio     (1000) julio     (1000)      112 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.0.2/py_sls_lambda_toolkit/logger.py
--rw-rw-r--   0 julio     (1000) julio     (1000)      757 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.0.2/py_sls_lambda_toolkit/parsers.py
--rw-rw-r--   0 julio     (1000) julio     (1000)     3350 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.0.2/py_sls_lambda_toolkit/scan_filter_builder.py
--rw-rw-r--   0 julio     (1000) julio     (1000)     1255 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.0.2/py_sls_lambda_toolkit/status_code.py
--rw-rw-r--   0 julio     (1000) julio     (1000)      863 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.0.2/py_sls_lambda_toolkit/validators.py
-drwxrwxr-x   0 julio     (1000) julio     (1000)        0 2023-04-23 18:15:01.537016 py-sls-lambda-toolkit-0.0.2/py_sls_lambda_toolkit.egg-info/
--rw-rw-r--   0 julio     (1000) julio     (1000)      762 2023-04-23 18:15:01.000000 py-sls-lambda-toolkit-0.0.2/py_sls_lambda_toolkit.egg-info/PKG-INFO
--rw-rw-r--   0 julio     (1000) julio     (1000)      604 2023-04-23 18:15:01.000000 py-sls-lambda-toolkit-0.0.2/py_sls_lambda_toolkit.egg-info/SOURCES.txt
--rw-rw-r--   0 julio     (1000) julio     (1000)        1 2023-04-23 18:15:01.000000 py-sls-lambda-toolkit-0.0.2/py_sls_lambda_toolkit.egg-info/dependency_links.txt
--rw-rw-r--   0 julio     (1000) julio     (1000)       33 2023-04-23 18:15:01.000000 py-sls-lambda-toolkit-0.0.2/py_sls_lambda_toolkit.egg-info/requires.txt
--rw-rw-r--   0 julio     (1000) julio     (1000)       22 2023-04-23 18:15:01.000000 py-sls-lambda-toolkit-0.0.2/py_sls_lambda_toolkit.egg-info/top_level.txt
--rw-rw-r--   0 julio     (1000) julio     (1000)       94 2023-04-23 17:31:48.000000 py-sls-lambda-toolkit-0.0.2/pyproject.toml
--rw-rw-r--   0 julio     (1000) julio     (1000)      927 2023-04-23 18:15:01.537016 py-sls-lambda-toolkit-0.0.2/setup.cfg
+drwxrwxr-x   0 julio     (1000) julio     (1000)        0 2023-04-23 18:26:19.318116 py-sls-lambda-toolkit-0.0.3/
+-rw-rw-r--   0 julio     (1000) julio     (1000)     1069 2023-04-23 17:34:15.000000 py-sls-lambda-toolkit-0.0.3/LICENSE
+-rw-rw-r--   0 julio     (1000) julio     (1000)       34 2023-04-23 18:05:48.000000 py-sls-lambda-toolkit-0.0.3/MANIFEST.in
+-rw-rw-r--   0 julio     (1000) julio     (1000)      762 2023-04-23 18:26:19.318116 py-sls-lambda-toolkit-0.0.3/PKG-INFO
+drwxrwxr-x   0 julio     (1000) julio     (1000)        0 2023-04-23 18:26:19.318116 py-sls-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/
+-rw-rw-r--   0 julio     (1000) julio     (1000)        0 2023-04-23 17:11:35.000000 py-sls-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/__init__.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)     1370 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/dynamodb_shortcuts.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)     1651 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/http_event.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)     1222 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/http_response.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)      112 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/logger.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)      757 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/parsers.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)     3350 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/scan_filter_builder.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)     1255 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/status_code.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)      863 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/validators.py
+drwxrwxr-x   0 julio     (1000) julio     (1000)        0 2023-04-23 18:26:19.318116 py-sls-lambda-toolkit-0.0.3/py_sls_lambda_toolkit.egg-info/
+-rw-rw-r--   0 julio     (1000) julio     (1000)      762 2023-04-23 18:26:19.000000 py-sls-lambda-toolkit-0.0.3/py_sls_lambda_toolkit.egg-info/PKG-INFO
+-rw-rw-r--   0 julio     (1000) julio     (1000)      604 2023-04-23 18:26:19.000000 py-sls-lambda-toolkit-0.0.3/py_sls_lambda_toolkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 julio     (1000) julio     (1000)        1 2023-04-23 18:26:19.000000 py-sls-lambda-toolkit-0.0.3/py_sls_lambda_toolkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 julio     (1000) julio     (1000)       33 2023-04-23 18:26:19.000000 py-sls-lambda-toolkit-0.0.3/py_sls_lambda_toolkit.egg-info/requires.txt
+-rw-rw-r--   0 julio     (1000) julio     (1000)       22 2023-04-23 18:26:19.000000 py-sls-lambda-toolkit-0.0.3/py_sls_lambda_toolkit.egg-info/top_level.txt
+-rw-rw-r--   0 julio     (1000) julio     (1000)       94 2023-04-23 17:31:48.000000 py-sls-lambda-toolkit-0.0.3/pyproject.toml
+-rw-rw-r--   0 julio     (1000) julio     (1000)      927 2023-04-23 18:26:19.318116 py-sls-lambda-toolkit-0.0.3/setup.cfg
```

### Comparing `py-sls-lambda-toolkit-0.0.2/LICENSE` & `py-sls-lambda-toolkit-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `py-sls-lambda-toolkit-0.0.2/PKG-INFO` & `py-sls-lambda-toolkit-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-sls-lambda-toolkit
-Version: 0.0.2
+Version: 0.0.3
 Summary: A toolkit for serverless and AWS, with a focus on AWS Lambda and dynamodb.
 Home-page: https://github.com/0riion/py-sls-lambda-toolkit
 Author: Julio Flores
 Author-email: juliocesarflores12@gmail.com
 License: MIT
 Keywords: aws,serverless,lambda,dynamodb,toolkit
 Classifier: Development Status :: 1 - Planning
```

### Comparing `py-sls-lambda-toolkit-0.0.2/py_sls_lambda_toolkit/dynamodb_shortcuts.py` & `py-sls-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/dynamodb_shortcuts.py`

 * *Files identical despite different names*

### Comparing `py-sls-lambda-toolkit-0.0.2/py_sls_lambda_toolkit/http_event.py` & `py-sls-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/http_event.py`

 * *Files identical despite different names*

### Comparing `py-sls-lambda-toolkit-0.0.2/py_sls_lambda_toolkit/http_response.py` & `py-sls-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/http_response.py`

 * *Files identical despite different names*

### Comparing `py-sls-lambda-toolkit-0.0.2/py_sls_lambda_toolkit/parsers.py` & `py-sls-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/parsers.py`

 * *Files identical despite different names*

### Comparing `py-sls-lambda-toolkit-0.0.2/py_sls_lambda_toolkit/scan_filter_builder.py` & `py-sls-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/scan_filter_builder.py`

 * *Files identical despite different names*

### Comparing `py-sls-lambda-toolkit-0.0.2/py_sls_lambda_toolkit/status_code.py` & `py-sls-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/status_code.py`

 * *Files identical despite different names*

### Comparing `py-sls-lambda-toolkit-0.0.2/py_sls_lambda_toolkit/validators.py` & `py-sls-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/validators.py`

 * *Files identical despite different names*

### Comparing `py-sls-lambda-toolkit-0.0.2/py_sls_lambda_toolkit.egg-info/PKG-INFO` & `py-sls-lambda-toolkit-0.0.3/py_sls_lambda_toolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-sls-lambda-toolkit
-Version: 0.0.2
+Version: 0.0.3
 Summary: A toolkit for serverless and AWS, with a focus on AWS Lambda and dynamodb.
 Home-page: https://github.com/0riion/py-sls-lambda-toolkit
 Author: Julio Flores
 Author-email: juliocesarflores12@gmail.com
 License: MIT
 Keywords: aws,serverless,lambda,dynamodb,toolkit
 Classifier: Development Status :: 1 - Planning
```

### Comparing `py-sls-lambda-toolkit-0.0.2/py_sls_lambda_toolkit.egg-info/SOURCES.txt` & `py-sls-lambda-toolkit-0.0.3/py_sls_lambda_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-sls-lambda-toolkit-0.0.2/setup.cfg` & `py-sls-lambda-toolkit-0.0.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = py-sls-lambda-toolkit
-version = 0.0.2
+version = 0.0.3
 author = Julio Flores
 author_email = juliocesarflores12@gmail.com
 author_url = juliofloresdev.com
 description = A toolkit for serverless and AWS, with a focus on AWS Lambda and dynamodb.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/0riion/py-sls-lambda-toolkit
@@ -27,14 +27,14 @@
 
 [options]
 packages = find:
 python_requires = >=3.8
 install_requires = 
 	boto3
 	jsonschema
-	camel-converter
+	camel_converter
 include_package_data = True
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

