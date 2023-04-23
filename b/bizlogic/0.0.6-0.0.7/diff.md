# Comparing `tmp/bizlogic-0.0.6.tar.gz` & `tmp/bizlogic-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bizlogic-0.0.6.tar", max compression
+gzip compressed data, was "bizlogic-0.0.7.tar", max compression
```

## Comparing `bizlogic-0.0.6.tar` & `bizlogic-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0     1211 2023-04-20 00:41:45.427991 bizlogic-0.0.6/LICENSE
--rw-r--r--   0        0        0     2000 2023-04-23 01:27:25.257694 bizlogic-0.0.6/README.md
--rw-r--r--   0        0        0      438 2023-04-23 15:29:01.054669 bizlogic-0.0.6/bizlogic/__init__.py
--rw-r--r--   0        0        0     2501 2023-04-23 01:28:29.489913 bizlogic-0.0.6/bizlogic/application.py
--rw-r--r--   0        0        0       31 2023-04-23 15:26:55.029602 bizlogic-0.0.6/bizlogic/loan/__init__.py
--rw-r--r--   0        0        0     2103 2023-04-23 01:28:11.757761 bizlogic-0.0.6/bizlogic/loan/reader.py
--rw-r--r--   0        0        0     1596 2023-04-23 01:29:03.050820 bizlogic-0.0.6/bizlogic/loan/repayment.py
--rw-r--r--   0        0        0     1070 2023-04-23 01:29:08.919190 bizlogic-0.0.6/bizlogic/loan/status.py
--rw-r--r--   0        0        0     3231 2023-04-23 01:29:12.085631 bizlogic-0.0.6/bizlogic/loan/writer.py
--rw-r--r--   0        0        0       15 2023-04-23 15:26:57.521945 bizlogic-0.0.6/bizlogic/protoc/__init__.py
--rw-r--r--   0        0        0     1053 2023-04-21 18:43:51.632790 bizlogic-0.0.6/bizlogic/protoc/loan_application_pb2.py
--rw-r--r--   0        0        0     1263 2023-04-21 01:34:03.254693 bizlogic-0.0.6/bizlogic/protoc/loan_payment_pb2.py
--rw-r--r--   0        0        0     1709 2023-04-21 18:43:51.632965 bizlogic-0.0.6/bizlogic/protoc/loan_pb2.py
--rw-r--r--   0        0        0      942 2023-04-21 18:43:51.633978 bizlogic-0.0.6/bizlogic/protoc/vouch_pb2.py
--rw-r--r--   0        0        0     2080 2023-04-23 01:28:57.982128 bizlogic-0.0.6/bizlogic/vouch.py
--rw-r--r--   0        0        0      451 2023-04-23 15:29:18.558269 bizlogic-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2533 1970-01-01 00:00:00.000000 bizlogic-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-04-20 00:41:45.427991 bizlogic-0.0.7/LICENSE
+-rw-r--r--   0        0        0     2000 2023-04-23 01:27:25.257694 bizlogic-0.0.7/README.md
+-rw-r--r--   0        0        0      393 2023-04-23 15:39:26.408950 bizlogic-0.0.7/bizlogic/__init__.py
+-rw-r--r--   0        0        0     2501 2023-04-23 01:28:29.489913 bizlogic-0.0.7/bizlogic/application.py
+-rw-r--r--   0        0        0       61 2023-04-23 15:36:06.068712 bizlogic-0.0.7/bizlogic/loan/__init__.py
+-rw-r--r--   0        0        0     2134 2023-04-23 15:40:44.613829 bizlogic-0.0.7/bizlogic/loan/reader.py
+-rw-r--r--   0        0        0     1600 2023-04-23 15:41:28.932012 bizlogic-0.0.7/bizlogic/loan/repayment.py
+-rw-r--r--   0        0        0     1074 2023-04-23 15:39:56.859849 bizlogic-0.0.7/bizlogic/loan/status.py
+-rw-r--r--   0        0        0     3231 2023-04-23 01:29:12.085631 bizlogic-0.0.7/bizlogic/loan/writer.py
+-rw-r--r--   0        0        0       48 2023-04-23 15:35:52.968443 bizlogic-0.0.7/bizlogic/protoc/__init__.py
+-rw-r--r--   0        0        0     1053 2023-04-23 15:31:58.337652 bizlogic-0.0.7/bizlogic/protoc/loan_application_pb2.py
+-rw-r--r--   0        0        0     1709 2023-04-23 15:31:58.338431 bizlogic-0.0.7/bizlogic/protoc/loan_pb2.py
+-rw-r--r--   0        0        0      942 2023-04-23 15:31:58.338641 bizlogic-0.0.7/bizlogic/protoc/vouch_pb2.py
+-rw-r--r--   0        0        0     2080 2023-04-23 01:28:57.982128 bizlogic-0.0.7/bizlogic/vouch.py
+-rw-r--r--   0        0        0      451 2023-04-23 15:39:36.514038 bizlogic-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2533 1970-01-01 00:00:00.000000 bizlogic-0.0.7/PKG-INFO
```

### Comparing `bizlogic-0.0.6/LICENSE` & `bizlogic-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bizlogic-0.0.6/README.md` & `bizlogic-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `bizlogic-0.0.6/bizlogic/application.py` & `bizlogic-0.0.7/bizlogic/application.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.0.6/bizlogic/loan/reader.py` & `bizlogic-0.0.7/bizlogic/loan/reader.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from ipfsclient.ipfs import Ipfs
 from typing import Self
 from bizlogic.loan import PREFIX
 from bizlogic.loan.status import LoanStatus, LoanStatusType
-from ipfskvs import Index, Store
+from ipfskvs.index import Index
+from ipfskvs.store import Store
 
 from bizlogic.protoc.loan_pb2 import Loan
 
 class LoanReader():
     ipfsclient: Ipfs
 
     def __init__(self: Self, ipfsclient: Ipfs):
```

### Comparing `bizlogic-0.0.6/bizlogic/loan/repayment.py` & `bizlogic-0.0.7/bizlogic/loan/repayment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime
 from typing import List
 from google.protobuf.timestamp_pb2 import Timestamp
 import uuid
 
-from bizlogic.protoc.loan import LoanPayment
+from bizlogic.protoc.loan_pb2 import LoanPayment
 
 
 class PaymentSchedule():
 
     @staticmethod
     @staticmethod
     def create_payment_schedule(
```

### Comparing `bizlogic-0.0.6/bizlogic/loan/status.py` & `bizlogic-0.0.7/bizlogic/loan/status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from google.protobuf.timestamp_pb2 import Timestamp
 from enum import Enum
 from datetime import datetime, timedelta
 
-from bizlogic.protoc.loan import Loan
+from bizlogic.protoc.loan_pb2 import Loan
 
 
 class LoanStatusType(Enum):
     PENDING_ACCEPTANCE = 1
     EXPIRED_UNACCEPTED = 2
     ACCEPTED = 3
```

### Comparing `bizlogic-0.0.6/bizlogic/loan/writer.py` & `bizlogic-0.0.7/bizlogic/loan/writer.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.0.6/bizlogic/protoc/loan_application_pb2.py` & `bizlogic-0.0.7/bizlogic/protoc/loan_application_pb2.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.0.6/bizlogic/protoc/loan_payment_pb2.py` & `bizlogic-0.0.7/bizlogic/protoc/loan_pb2.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: loan_payment.proto
+# source: loan.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12loan_payment.proto\x12\x10nanoswap.message\x1a\x1fgoogle/protobuf/timestamp.proto\"y\n\x0bLoanPayment\x12\x12\n\namount_due\x18\x01 \x01(\x03\x12,\n\x08\x64ue_date\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x0btransaction\x18\x03 \x01(\tH\x00\x88\x01\x01\x42\x0e\n\x0c_transactionb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\nloan.proto\x12\x10nanoswap.message\x1a\x1fgoogle/protobuf/timestamp.proto\"\x8d\x01\n\x0bLoanPayment\x12\x12\n\npayment_id\x18\x01 \x01(\t\x12\x12\n\namount_due\x18\x02 \x01(\x03\x12,\n\x08\x64ue_date\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x0btransaction\x18\x04 \x01(\tH\x00\x88\x01\x01\x42\x0e\n\x0c_transaction\"\xc9\x01\n\x04Loan\x12\x18\n\x10principal_amount\x18\x01 \x01(\x03\x12\x39\n\x12repayment_schedule\x18\x02 \x03(\x0b\x32\x1d.nanoswap.message.LoanPayment\x12\x30\n\x0coffer_expiry\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x0btransaction\x18\x04 \x01(\tH\x00\x88\x01\x01\x12\x10\n\x08\x61\x63\x63\x65pted\x18\x05 \x01(\x08\x42\x0e\n\x0c_transactionb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'loan_payment_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'loan_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  _LOANPAYMENT._serialized_start=73
-  _LOANPAYMENT._serialized_end=194
+  _LOANPAYMENT._serialized_start=66
+  _LOANPAYMENT._serialized_end=207
+  _LOAN._serialized_start=210
+  _LOAN._serialized_end=411
 # @@protoc_insertion_point(module_scope)
```

### Comparing `bizlogic-0.0.6/bizlogic/protoc/vouch_pb2.py` & `bizlogic-0.0.7/bizlogic/protoc/vouch_pb2.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.0.6/bizlogic/vouch.py` & `bizlogic-0.0.7/bizlogic/vouch.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.0.6/PKG-INFO` & `bizlogic-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bizlogic
-Version: 0.0.6
+Version: 0.0.7
 Summary: web3 lending platform business logic
 Author: Nate Schultz
 Author-email: nate.schultz@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ipfsclient (==0.0.7)
```

