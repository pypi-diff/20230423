# Comparing `tmp/bizlogic-0.0.4.tar.gz` & `tmp/bizlogic-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bizlogic-0.0.4.tar", max compression
+gzip compressed data, was "bizlogic-0.0.5.tar", max compression
```

## Comparing `bizlogic-0.0.4.tar` & `bizlogic-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     1211 2023-04-20 00:41:45.427991 bizlogic-0.0.4/LICENSE
--rw-r--r--   0        0        0     2000 2023-04-23 01:27:25.257694 bizlogic-0.0.4/README.md
--rw-r--r--   0        0        0       58 2023-04-23 01:31:53.055116 bizlogic-0.0.4/bizlogic/__init__.py
--rw-r--r--   0        0        0     2501 2023-04-23 01:28:29.489913 bizlogic-0.0.4/bizlogic/application.py
--rw-r--r--   0        0        0       16 2023-04-22 17:58:44.167371 bizlogic-0.0.4/bizlogic/loan/__init__.py
--rw-r--r--   0        0        0     2103 2023-04-23 01:28:11.757761 bizlogic-0.0.4/bizlogic/loan/reader.py
--rw-r--r--   0        0        0     1596 2023-04-23 01:29:03.050820 bizlogic-0.0.4/bizlogic/loan/repayment.py
--rw-r--r--   0        0        0     1070 2023-04-23 01:29:08.919190 bizlogic-0.0.4/bizlogic/loan/status.py
--rw-r--r--   0        0        0     3231 2023-04-23 01:29:12.085631 bizlogic-0.0.4/bizlogic/loan/writer.py
--rw-r--r--   0        0        0     1053 2023-04-21 18:43:51.632790 bizlogic-0.0.4/bizlogic/protoc/loan_application_pb2.py
--rw-r--r--   0        0        0     1263 2023-04-21 01:34:03.254693 bizlogic-0.0.4/bizlogic/protoc/loan_payment_pb2.py
--rw-r--r--   0        0        0     1709 2023-04-21 18:43:51.632965 bizlogic-0.0.4/bizlogic/protoc/loan_pb2.py
--rw-r--r--   0        0        0      942 2023-04-21 18:43:51.633978 bizlogic-0.0.4/bizlogic/protoc/vouch_pb2.py
--rw-r--r--   0        0        0     2080 2023-04-23 01:28:57.982128 bizlogic-0.0.4/bizlogic/vouch.py
--rw-r--r--   0        0        0      451 2023-04-23 01:30:12.626067 bizlogic-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2533 1970-01-01 00:00:00.000000 bizlogic-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-04-20 00:41:45.427991 bizlogic-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2000 2023-04-23 01:27:25.257694 bizlogic-0.0.5/README.md
+-rw-r--r--   0        0        0       58 2023-04-23 01:33:26.387031 bizlogic-0.0.5/bizlogic/__init__.py
+-rw-r--r--   0        0        0     2501 2023-04-23 01:28:29.489913 bizlogic-0.0.5/bizlogic/application.py
+-rw-r--r--   0        0        0       16 2023-04-22 17:58:44.167371 bizlogic-0.0.5/bizlogic/loan/__init__.py
+-rw-r--r--   0        0        0     2103 2023-04-23 01:28:11.757761 bizlogic-0.0.5/bizlogic/loan/reader.py
+-rw-r--r--   0        0        0     1596 2023-04-23 01:29:03.050820 bizlogic-0.0.5/bizlogic/loan/repayment.py
+-rw-r--r--   0        0        0     1070 2023-04-23 01:29:08.919190 bizlogic-0.0.5/bizlogic/loan/status.py
+-rw-r--r--   0        0        0     3231 2023-04-23 01:29:12.085631 bizlogic-0.0.5/bizlogic/loan/writer.py
+-rw-r--r--   0        0        0        0 2023-04-23 01:33:10.539027 bizlogic-0.0.5/bizlogic/protoc/__init__.py
+-rw-r--r--   0        0        0     1053 2023-04-21 18:43:51.632790 bizlogic-0.0.5/bizlogic/protoc/loan_application_pb2.py
+-rw-r--r--   0        0        0     1263 2023-04-21 01:34:03.254693 bizlogic-0.0.5/bizlogic/protoc/loan_payment_pb2.py
+-rw-r--r--   0        0        0     1709 2023-04-21 18:43:51.632965 bizlogic-0.0.5/bizlogic/protoc/loan_pb2.py
+-rw-r--r--   0        0        0      942 2023-04-21 18:43:51.633978 bizlogic-0.0.5/bizlogic/protoc/vouch_pb2.py
+-rw-r--r--   0        0        0     2080 2023-04-23 01:28:57.982128 bizlogic-0.0.5/bizlogic/vouch.py
+-rw-r--r--   0        0        0      451 2023-04-23 01:33:22.321198 bizlogic-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2533 1970-01-01 00:00:00.000000 bizlogic-0.0.5/PKG-INFO
```

### Comparing `bizlogic-0.0.4/LICENSE` & `bizlogic-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bizlogic-0.0.4/README.md` & `bizlogic-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `bizlogic-0.0.4/bizlogic/application.py` & `bizlogic-0.0.5/bizlogic/application.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.0.4/bizlogic/loan/reader.py` & `bizlogic-0.0.5/bizlogic/loan/reader.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.0.4/bizlogic/loan/repayment.py` & `bizlogic-0.0.5/bizlogic/loan/repayment.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.0.4/bizlogic/loan/status.py` & `bizlogic-0.0.5/bizlogic/loan/status.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.0.4/bizlogic/loan/writer.py` & `bizlogic-0.0.5/bizlogic/loan/writer.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.0.4/bizlogic/protoc/loan_application_pb2.py` & `bizlogic-0.0.5/bizlogic/protoc/loan_application_pb2.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.0.4/bizlogic/protoc/loan_payment_pb2.py` & `bizlogic-0.0.5/bizlogic/protoc/loan_payment_pb2.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.0.4/bizlogic/protoc/loan_pb2.py` & `bizlogic-0.0.5/bizlogic/protoc/loan_pb2.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.0.4/bizlogic/protoc/vouch_pb2.py` & `bizlogic-0.0.5/bizlogic/protoc/vouch_pb2.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.0.4/bizlogic/vouch.py` & `bizlogic-0.0.5/bizlogic/vouch.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.0.4/PKG-INFO` & `bizlogic-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bizlogic
-Version: 0.0.4
+Version: 0.0.5
 Summary: web3 lending platform business logic
 Author: Nate Schultz
 Author-email: nate.schultz@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ipfsclient (==0.0.7)
```

