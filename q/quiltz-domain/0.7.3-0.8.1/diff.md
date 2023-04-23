# Comparing `tmp/quiltz-domain-0.7.3.tar.gz` & `tmp/quiltz-domain-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quiltz-domain-0.7.3.tar", last modified: Sun Jan  8 13:18:34 2023, max compression
+gzip compressed data, was "quiltz-domain-0.8.1.tar", last modified: Sun Apr 23 09:59:20 2023, max compression
```

## Comparing `quiltz-domain-0.7.3.tar` & `quiltz-domain-0.8.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 13:18:34.525253 quiltz-domain-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-01-08 13:18:18.000000 quiltz-domain-0.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-01-08 13:18:34.525253 quiltz-domain-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-01-08 13:18:18.000000 quiltz-domain-0.7.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-08 13:18:34.525253 quiltz-domain-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-01-08 13:18:18.000000 quiltz-domain-0.7.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 13:18:34.525253 quiltz-domain-0.7.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 13:18:34.525253 quiltz-domain-0.7.3/src/quiltz/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-01-08 13:18:18.000000 quiltz-domain-0.7.3/src/quiltz/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 13:18:34.525253 quiltz-domain-0.7.3/src/quiltz/domain/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-01-08 13:18:18.000000 quiltz-domain-0.7.3/src/quiltz/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-01-08 13:18:18.000000 quiltz-domain-0.7.3/src/quiltz/domain/anonymizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-01-08 13:18:18.000000 quiltz-domain-0.7.3/src/quiltz/domain/email.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 13:18:34.525253 quiltz-domain-0.7.3/src/quiltz/domain/id/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-01-08 13:18:18.000000 quiltz-domain-0.7.3/src/quiltz/domain/id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-01-08 13:18:18.000000 quiltz-domain-0.7.3/src/quiltz/domain/id/id.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-01-08 13:18:18.000000 quiltz-domain-0.7.3/src/quiltz/domain/id/testbuilders.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-01-08 13:18:18.000000 quiltz-domain-0.7.3/src/quiltz/domain/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-01-08 13:18:18.000000 quiltz-domain-0.7.3/src/quiltz/domain/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-01-08 13:18:18.000000 quiltz-domain-0.7.3/src/quiltz/domain/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-01-08 13:18:18.000000 quiltz-domain-0.7.3/src/quiltz/domain/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 13:18:34.525253 quiltz-domain-0.7.3/src/quiltz_domain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-01-08 13:18:34.000000 quiltz-domain-0.7.3/src/quiltz_domain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-01-08 13:18:34.000000 quiltz-domain-0.7.3/src/quiltz_domain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-08 13:18:34.000000 quiltz-domain-0.7.3/src/quiltz_domain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-08 13:18:34.000000 quiltz-domain-0.7.3/src/quiltz_domain.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:59:20.888149 quiltz-domain-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-23 09:59:00.000000 quiltz-domain-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-23 09:59:20.888149 quiltz-domain-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-23 09:59:00.000000 quiltz-domain-0.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 09:59:20.888149 quiltz-domain-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-23 09:59:00.000000 quiltz-domain-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:59:20.884149 quiltz-domain-0.8.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:59:20.884149 quiltz-domain-0.8.1/src/quiltz/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-23 09:59:00.000000 quiltz-domain-0.8.1/src/quiltz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:59:20.888149 quiltz-domain-0.8.1/src/quiltz/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-23 09:59:00.000000 quiltz-domain-0.8.1/src/quiltz/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-23 09:59:00.000000 quiltz-domain-0.8.1/src/quiltz/domain/anonymizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-23 09:59:00.000000 quiltz-domain-0.8.1/src/quiltz/domain/email.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:59:20.888149 quiltz-domain-0.8.1/src/quiltz/domain/id/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-23 09:59:00.000000 quiltz-domain-0.8.1/src/quiltz/domain/id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-23 09:59:00.000000 quiltz-domain-0.8.1/src/quiltz/domain/id/id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-23 09:59:00.000000 quiltz-domain-0.8.1/src/quiltz/domain/id/testbuilders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-23 09:59:00.000000 quiltz-domain-0.8.1/src/quiltz/domain/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-23 09:59:00.000000 quiltz-domain-0.8.1/src/quiltz/domain/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-04-23 09:59:00.000000 quiltz-domain-0.8.1/src/quiltz/domain/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-23 09:59:00.000000 quiltz-domain-0.8.1/src/quiltz/domain/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:59:20.888149 quiltz-domain-0.8.1/src/quiltz_domain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-23 09:59:20.000000 quiltz-domain-0.8.1/src/quiltz_domain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-23 09:59:20.000000 quiltz-domain-0.8.1/src/quiltz_domain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 09:59:20.000000 quiltz-domain-0.8.1/src/quiltz_domain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-23 09:59:20.000000 quiltz-domain-0.8.1/src/quiltz_domain.egg-info/top_level.txt
```

### Comparing `quiltz-domain-0.7.3/LICENSE` & `quiltz-domain-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `quiltz-domain-0.7.3/PKG-INFO` & `quiltz-domain-0.8.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quiltz-domain
-Version: 0.7.3
+Version: 0.8.1
 Summary: A domain utility module for python
 Home-page: https://github.com/qwaneu/quiltz-domain
 Author: Rob Westgeest
 Author-email: rob@qwan.eu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `quiltz-domain-0.7.3/README.md` & `quiltz-domain-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `quiltz-domain-0.7.3/setup.py` & `quiltz-domain-0.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `quiltz-domain-0.7.3/src/quiltz/domain/id/id.py` & `quiltz-domain-0.8.1/src/quiltz/domain/id/id.py`

 * *Files identical despite different names*

### Comparing `quiltz-domain-0.7.3/src/quiltz/domain/parsers.py` & `quiltz-domain-0.8.1/src/quiltz/domain/parsers.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,16 @@
             return Success(**{success_attribute: date.fromisoformat(date_string)})
         except ValueError as e:
             return Failure(message=f'{success_attribute}: {e}')
 
 
 class StringToIntParser:
     def parse_from(self, int_string, success_attribute='int_val'):
+        if not int_string:
+            return Failure(message=f"{success_attribute} is missing")
         try:
             return Success(**{success_attribute: int(int_string)})
         except ValueError as e:
             return Failure(message="'{}' is not a valid integer".format(int_string))
 
 
 date_from_iso = StringToDateParser()
```

### Comparing `quiltz-domain-0.7.3/src/quiltz/domain/results.py` & `quiltz-domain-0.8.1/src/quiltz/domain/results.py`

 * *Files identical despite different names*

### Comparing `quiltz-domain-0.7.3/src/quiltz/domain/validator.py` & `quiltz-domain-0.8.1/src/quiltz/domain/validator.py`

 * *Files identical despite different names*

### Comparing `quiltz-domain-0.7.3/src/quiltz_domain.egg-info/PKG-INFO` & `quiltz-domain-0.8.1/src/quiltz_domain.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quiltz-domain
-Version: 0.7.3
+Version: 0.8.1
 Summary: A domain utility module for python
 Home-page: https://github.com/qwaneu/quiltz-domain
 Author: Rob Westgeest
 Author-email: rob@qwan.eu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `quiltz-domain-0.7.3/src/quiltz_domain.egg-info/SOURCES.txt` & `quiltz-domain-0.8.1/src/quiltz_domain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

