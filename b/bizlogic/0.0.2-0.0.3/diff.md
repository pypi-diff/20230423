# Comparing `tmp/bizlogic-0.0.2.tar.gz` & `tmp/bizlogic-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bizlogic-0.0.2.tar", max compression
+gzip compressed data, was "bizlogic-0.0.3.tar", max compression
```

## Comparing `bizlogic-0.0.2.tar` & `bizlogic-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1211 2023-04-20 00:41:45.427991 bizlogic-0.0.2/LICENSE
--rw-r--r--   0        0        0     1991 2023-04-20 22:21:31.358991 bizlogic-0.0.2/README.md
--rw-r--r--   0        0        0       58 2023-04-22 18:31:37.985161 bizlogic-0.0.2/bizlogic/__init__.py
--rw-r--r--   0        0        0     2492 2023-04-22 16:52:44.739841 bizlogic-0.0.2/bizlogic/application.py
--rw-r--r--   0        0        0       16 2023-04-22 17:58:44.167371 bizlogic-0.0.2/bizlogic/loan/__init__.py
--rw-r--r--   0        0        0     2089 2023-04-22 18:15:32.612007 bizlogic-0.0.2/bizlogic/loan/reader.py
--rw-r--r--   0        0        0     1587 2023-04-22 18:45:00.284766 bizlogic-0.0.2/bizlogic/loan/repayment.py
--rw-r--r--   0        0        0     1061 2023-04-22 18:21:43.913408 bizlogic-0.0.2/bizlogic/loan/status.py
--rw-r--r--   0        0        0     3222 2023-04-22 18:21:59.201132 bizlogic-0.0.2/bizlogic/loan/writer.py
--rw-r--r--   0        0        0     2071 2023-04-22 16:57:44.718847 bizlogic-0.0.2/bizlogic/vouch.py
--rw-r--r--   0        0        0      451 2023-04-22 18:31:16.788313 bizlogic-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2524 1970-01-01 00:00:00.000000 bizlogic-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-04-20 00:41:45.427991 bizlogic-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1991 2023-04-20 22:21:31.358991 bizlogic-0.0.3/README.md
+-rw-r--r--   0        0        0       58 2023-04-23 01:25:06.361195 bizlogic-0.0.3/bizlogic/__init__.py
+-rw-r--r--   0        0        0     2492 2023-04-22 16:52:44.739841 bizlogic-0.0.3/bizlogic/application.py
+-rw-r--r--   0        0        0       16 2023-04-22 17:58:44.167371 bizlogic-0.0.3/bizlogic/loan/__init__.py
+-rw-r--r--   0        0        0     2094 2023-04-23 01:24:32.178438 bizlogic-0.0.3/bizlogic/loan/reader.py
+-rw-r--r--   0        0        0     1587 2023-04-22 18:45:00.284766 bizlogic-0.0.3/bizlogic/loan/repayment.py
+-rw-r--r--   0        0        0     1061 2023-04-22 18:21:43.913408 bizlogic-0.0.3/bizlogic/loan/status.py
+-rw-r--r--   0        0        0     3222 2023-04-22 18:21:59.201132 bizlogic-0.0.3/bizlogic/loan/writer.py
+-rw-r--r--   0        0        0     2071 2023-04-22 16:57:44.718847 bizlogic-0.0.3/bizlogic/vouch.py
+-rw-r--r--   0        0        0      451 2023-04-23 01:24:59.916074 bizlogic-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2524 1970-01-01 00:00:00.000000 bizlogic-0.0.3/PKG-INFO
```

### Comparing `bizlogic-0.0.2/LICENSE` & `bizlogic-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bizlogic-0.0.2/README.md` & `bizlogic-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `bizlogic-0.0.2/bizlogic/application.py` & `bizlogic-0.0.3/bizlogic/application.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.0.2/bizlogic/loan/reader.py` & `bizlogic-0.0.3/bizlogic/loan/reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ipfsclient import Ipfs
+from ipfsclient.ipfs import Ipfs
 from typing import Self
 from bizlogic.loan import PREFIX
 from bizlogic.loan.status import LoanStatus, LoanStatusType
 from ipfskvs import Index, Store
 
 from protoc.loan_pb2 import Loan
```

### Comparing `bizlogic-0.0.2/bizlogic/loan/repayment.py` & `bizlogic-0.0.3/bizlogic/loan/repayment.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.0.2/bizlogic/loan/status.py` & `bizlogic-0.0.3/bizlogic/loan/status.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.0.2/bizlogic/loan/writer.py` & `bizlogic-0.0.3/bizlogic/loan/writer.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.0.2/bizlogic/vouch.py` & `bizlogic-0.0.3/bizlogic/vouch.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.0.2/PKG-INFO` & `bizlogic-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bizlogic
-Version: 0.0.2
+Version: 0.0.3
 Summary: web3 lending platform business logic
 Author: Nate Schultz
 Author-email: nate.schultz@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ipfsclient (==0.0.7)
```

