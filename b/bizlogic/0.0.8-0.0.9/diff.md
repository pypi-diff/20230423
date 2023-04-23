# Comparing `tmp/bizlogic-0.0.8.tar.gz` & `tmp/bizlogic-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bizlogic-0.0.8.tar", max compression
+gzip compressed data, was "bizlogic-0.0.9.tar", max compression
```

## Comparing `bizlogic-0.0.8.tar` & `bizlogic-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1211 2023-04-20 00:41:45.427991 bizlogic-0.0.8/LICENSE
--rw-r--r--   0        0        0     2000 2023-04-23 01:27:25.257694 bizlogic-0.0.8/README.md
--rw-r--r--   0        0        0      393 2023-04-23 16:14:44.553019 bizlogic-0.0.8/bizlogic/__init__.py
--rw-r--r--   0        0        0     3385 2023-04-23 16:13:06.454470 bizlogic-0.0.8/bizlogic/application.py
--rw-r--r--   0        0        0       61 2023-04-23 15:36:06.068712 bizlogic-0.0.8/bizlogic/loan/__init__.py
--rw-r--r--   0        0        0     2134 2023-04-23 15:40:44.613829 bizlogic-0.0.8/bizlogic/loan/reader.py
--rw-r--r--   0        0        0     1600 2023-04-23 15:41:28.932012 bizlogic-0.0.8/bizlogic/loan/repayment.py
--rw-r--r--   0        0        0     1074 2023-04-23 15:39:56.859849 bizlogic-0.0.8/bizlogic/loan/status.py
--rw-r--r--   0        0        0     3231 2023-04-23 01:29:12.085631 bizlogic-0.0.8/bizlogic/loan/writer.py
--rw-r--r--   0        0        0       48 2023-04-23 15:35:52.968443 bizlogic-0.0.8/bizlogic/protoc/__init__.py
--rw-r--r--   0        0        0     1053 2023-04-23 15:31:58.337652 bizlogic-0.0.8/bizlogic/protoc/loan_application_pb2.py
--rw-r--r--   0        0        0     1709 2023-04-23 15:31:58.338431 bizlogic-0.0.8/bizlogic/protoc/loan_pb2.py
--rw-r--r--   0        0        0      942 2023-04-23 15:31:58.338641 bizlogic-0.0.8/bizlogic/protoc/vouch_pb2.py
--rw-r--r--   0        0        0     2080 2023-04-23 01:28:57.982128 bizlogic-0.0.8/bizlogic/vouch.py
--rw-r--r--   0        0        0      451 2023-04-23 16:14:37.153999 bizlogic-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2533 1970-01-01 00:00:00.000000 bizlogic-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-04-20 00:41:45.427991 bizlogic-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2000 2023-04-23 01:27:25.257694 bizlogic-0.0.9/README.md
+-rw-r--r--   0        0        0      393 2023-04-23 19:20:59.434581 bizlogic-0.0.9/bizlogic/__init__.py
+-rw-r--r--   0        0        0     3433 2023-04-23 19:19:35.197027 bizlogic-0.0.9/bizlogic/application.py
+-rw-r--r--   0        0        0       61 2023-04-23 15:36:06.068712 bizlogic-0.0.9/bizlogic/loan/__init__.py
+-rw-r--r--   0        0        0     2230 2023-04-23 19:20:38.910227 bizlogic-0.0.9/bizlogic/loan/reader.py
+-rw-r--r--   0        0        0     1600 2023-04-23 15:41:28.932012 bizlogic-0.0.9/bizlogic/loan/repayment.py
+-rw-r--r--   0        0        0     1074 2023-04-23 15:39:56.859849 bizlogic-0.0.9/bizlogic/loan/status.py
+-rw-r--r--   0        0        0     3231 2023-04-23 01:29:12.085631 bizlogic-0.0.9/bizlogic/loan/writer.py
+-rw-r--r--   0        0        0       48 2023-04-23 15:35:52.968443 bizlogic-0.0.9/bizlogic/protoc/__init__.py
+-rw-r--r--   0        0        0     1053 2023-04-23 15:31:58.337652 bizlogic-0.0.9/bizlogic/protoc/loan_application_pb2.py
+-rw-r--r--   0        0        0     1709 2023-04-23 15:31:58.338431 bizlogic-0.0.9/bizlogic/protoc/loan_pb2.py
+-rw-r--r--   0        0        0      942 2023-04-23 15:31:58.338641 bizlogic-0.0.9/bizlogic/protoc/vouch_pb2.py
+-rw-r--r--   0        0        0     2128 2023-04-23 19:20:08.408812 bizlogic-0.0.9/bizlogic/vouch.py
+-rw-r--r--   0        0        0      451 2023-04-23 19:20:51.434045 bizlogic-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2533 1970-01-01 00:00:00.000000 bizlogic-0.0.9/PKG-INFO
```

### Comparing `bizlogic-0.0.8/LICENSE` & `bizlogic-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bizlogic-0.0.8/README.md` & `bizlogic-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `bizlogic-0.0.8/bizlogic/application.py` & `bizlogic-0.0.9/bizlogic/application.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,24 +98,26 @@
     
     def get_loan_applications_for_borrower(self: Self, borrower: str) -> List[LoanApplication]:
         return Store.query(
             query_index=Index(
                 prefix=PREFIX,
                 index={
                     "borrower": borrower
-                }
+                },
+                size=2
             ),
             ipfs=self.ipfsclient,
             reader=LoanApplication()
         )
 
     def get_loan_application(self: Self, application_id: str) -> LoanApplication:
         return Store.query(
             query_index=Index(
                 prefix=PREFIX,
                 index={
                     "application": application_id
-                }
+                },
+                size=2
             ),
             ipfs=self.ipfsclient,
             reader=LoanApplication()
         )
```

### Comparing `bizlogic-0.0.8/bizlogic/loan/reader.py` & `bizlogic-0.0.9/bizlogic/loan/reader.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,15 +16,16 @@
     def get_open_loan_offers(self: Self, borrower: str):
         return self.query_for_status(
             status=LoanStatus.PENDING_ACCEPTANCE,
             index=Index(
                 prefix=PREFIX,
                 index={
                     "borrower": borrower
-                }
+                },
+                size=3
             ),
         )
 
     def query_for_status(self: Self, status: LoanStatusType, index: dict = {}):
         # get all applications from ipfs
         loans = Store.query(
             query_index=Index(
@@ -44,36 +45,39 @@
 
     def query_for_borrower(self: Self, borrower: str):
         return Store.query(
             query_index=Index(
                 prefix=PREFIX,
                 index={
                     "borrower": borrower
-                }
+                },
+                size=3
             ),
             ipfs=self.ipfsclient,
             reader=Loan()
         )
 
     def query_for_lender(self: Self, lender: str):
         return Store.query(
             query_index=Index(
                 prefix=PREFIX,
                 index={
                     "lender": lender
-                }
+                },
+                size=3
             ),
             ipfs=self.ipfsclient,
             reader=Loan()
         )
 
     def query_for_loan(self: Self, loan_id: str):
         return Store.query(
             query_index=Index(
                 prefix=PREFIX,
                 index={
                     "loan": loan_id
-                }
+                },
+                size=3
             ),
             ipfs=self.ipfsclient,
             reader=Loan()
         )
```

### Comparing `bizlogic-0.0.8/bizlogic/loan/repayment.py` & `bizlogic-0.0.9/bizlogic/loan/repayment.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.0.8/bizlogic/loan/status.py` & `bizlogic-0.0.9/bizlogic/loan/status.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.0.8/bizlogic/loan/writer.py` & `bizlogic-0.0.9/bizlogic/loan/writer.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.0.8/bizlogic/protoc/loan_application_pb2.py` & `bizlogic-0.0.9/bizlogic/protoc/loan_application_pb2.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.0.8/bizlogic/protoc/loan_pb2.py` & `bizlogic-0.0.9/bizlogic/protoc/loan_pb2.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.0.8/bizlogic/protoc/vouch_pb2.py` & `bizlogic-0.0.9/bizlogic/protoc/vouch_pb2.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.0.8/bizlogic/vouch.py` & `bizlogic-0.0.9/bizlogic/vouch.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,24 +65,26 @@
 
     def get_vouchers_for_borrower(self: Self, borrower: str):
         return Store.query(
             query_index=Index(
                 prefix=PREFIX,
                 index={
                     "voucher": borrower
-                }
+                },
+                size=2
             ),
             ipfs=self.ipfsclient,
             reader=Vouch()
         )
 
     def get_vouchees_for_borrower(self: Self, borrower: str):
         return Store.query(
             query_index=Index(
                 prefix=PREFIX,
                 index={
                     "vouchee": borrower
-                }
+                },
+                size=2
             ),
             ipfs=self.ipfsclient,
             reader=Vouch()
         )
```

### Comparing `bizlogic-0.0.8/PKG-INFO` & `bizlogic-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bizlogic
-Version: 0.0.8
+Version: 0.0.9
 Summary: web3 lending platform business logic
 Author: Nate Schultz
 Author-email: nate.schultz@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ipfsclient (==0.0.7)
```

