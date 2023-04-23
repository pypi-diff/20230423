# Comparing `tmp/stigg-api-client-0.3.0.tar.gz` & `tmp/stigg_api_client-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stigg-api-client-0.3.0.tar", max compression
+gzip compressed data, was "stigg_api_client-0.4.0.tar", max compression
```

## Comparing `stigg-api-client-0.3.0.tar` & `stigg_api_client-0.4.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     2479 2023-03-05 12:25:06.526402 stigg-api-client-0.3.0/README.md
--rw-r--r--   0        0        0      396 2023-04-11 10:26:38.527477 stigg-api-client-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       44 2023-03-05 12:25:06.527501 stigg-api-client-0.3.0/stigg/__init__.py
--rw-r--r--   0        0        0      997 2023-03-05 12:25:06.527623 stigg-api-client-0.3.0/stigg/client.py
--rw-r--r--   0        0        0        0 2023-03-05 12:25:06.527730 stigg-api-client-0.3.0/stigg/generated/__init__.py
--rw-r--r--   0        0        0    43935 2023-04-11 10:24:57.366059 stigg-api-client-0.3.0/stigg/generated/operations.py
--rw-r--r--   0        0        0   432273 2023-04-11 10:24:57.216151 stigg-api-client-0.3.0/stigg/generated/schema.py
--rw-r--r--   0        0        0     3287 1970-01-01 00:00:00.000000 stigg-api-client-0.3.0/setup.py
--rw-r--r--   0        0        0     3108 1970-01-01 00:00:00.000000 stigg-api-client-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     2479 2023-03-05 12:25:06.526402 stigg_api_client-0.4.0/README.md
+-rw-r--r--   0        0        0      396 2023-04-23 10:58:44.895101 stigg_api_client-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-04-23 10:33:15.442973 stigg_api_client-0.4.0/stigg/__init__.py
+-rw-r--r--   0        0        0     1141 2023-04-23 10:31:23.415609 stigg_api_client-0.4.0/stigg/client.py
+-rw-r--r--   0        0        0        0 2023-03-05 12:25:06.527730 stigg_api_client-0.4.0/stigg/generated/__init__.py
+-rw-r--r--   0        0        0    43935 2023-04-12 14:11:36.612247 stigg_api_client-0.4.0/stigg/generated/operations.py
+-rw-r--r--   0        0        0   432273 2023-04-12 14:11:36.614988 stigg_api_client-0.4.0/stigg/generated/schema.py
+-rw-r--r--   0        0        0     3159 1970-01-01 00:00:00.000000 stigg_api_client-0.4.0/PKG-INFO
```

### Comparing `stigg-api-client-0.3.0/README.md` & `stigg_api_client-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `stigg-api-client-0.3.0/stigg/client.py` & `stigg_api_client-0.4.0/stigg/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,14 +8,20 @@
     def __init__(self, endpoint: RequestsEndpoint):
         self._endpoint: RequestsEndpoint = endpoint
 
     def request(self, operation: Operation, variables: dict, raw_response=False):
         data = self._endpoint(operation, variables)
         if raw_response:
             return data
+
+        # clean up data to so an exepction will be raised
+        errors = data.get('errors')
+        if errors:
+            data.pop('data')
+
         # interpret results into native Python objects
         return operation + data
 
 
 class Stigg(Operations):
     @staticmethod
     def create_client(api_key: str,
```

### Comparing `stigg-api-client-0.3.0/stigg/generated/operations.py` & `stigg_api_client-0.4.0/stigg/generated/operations.py`

 * *Files identical despite different names*

### Comparing `stigg-api-client-0.3.0/stigg/generated/schema.py` & `stigg_api_client-0.4.0/stigg/generated/schema.py`

 * *Files identical despite different names*

### Comparing `stigg-api-client-0.3.0/setup.py` & `stigg_api_client-0.4.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,124 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: stigg-api-client
+Version: 0.4.0
+Summary: 
+Author: Stigg
+Author-email: support@stigg.io
+Requires-Python: >=3.7,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: black (>=22.8.0,<23.0.0)
+Requires-Dist: flake8 (>=5.0.4,<6.0.0)
+Requires-Dist: graphql-core (==3.1.6)
+Requires-Dist: requests (>=2.28.1,<3.0.0)
+Requires-Dist: sgqlc (>=16.0,<17.0)
+Description-Content-Type: text/markdown
+
+# stigg-api-client
+
+This library provides a Python wrapper to [Stigg's GraphQL API](https://docs.stigg.io/docs/graphql-api) based on 
+the operations that are in use by the [Stigg's Node.js SDK](https://docs.stigg.io/docs/nodejs-sdk).
+
+It leverages the [sgqlc](https://github.com/profusion/sgqlc) library to generate Python classes for GraphQL types, and
+utilizes the `sgqlc.endpoint.requests.RequestsEndpoint` class to send the API requests. The responses are being
+automatically converted into native Python types.
+
+## Documentation
+
+See https://docs.stigg.io/docs/python-sdk
+
+## Installation
+
+    pip install stigg-api-client
+
+## Usage
+
+Initialize the client:
+
+```python
+
+import os
+from stigg import Stigg
+
+api_key = os.environ.get("STIGG_SERVER_API_KEY")
+
+stigg_client = Stigg.create_client(api_key)
+
+```
+
+Provision a customer
+
+```python
+
+import os
+from stigg import Stigg
+
+api_key = os.environ.get("STIGG_SERVER_API_KEY")
+
+client = Stigg.create_client(api_key)
+
+data = client.request(Stigg.mutation.provision_customer, {
+    "input": {
+        "refId": "customer-id",
+        "name": "Acme",
+        "email": "hello@acme.com",
+        "couponRefId": "coupon-id",
+        "billingInformation": {
+            "language": "en",
+            "timezone": "America/New_York",
+            "billingAddress": {
+                "country": "US",
+                "city": "New York",
+                "state": "NY",
+                "addressLine1": "123 Main Street",
+                "addressLine2": "Apt. 1",
+                "phoneNumber": "+1 212-499-5321",
+                "postalCode": "10164"
+            },
+            "shippingAddress": {
+                "country": "US",
+                "city": "New York",
+                "state": "NY",
+                "addressLine1": "123 Main Street",
+                "addressLine2": "Apt. 1",
+                "phoneNumber": "+1 212-499-5321",
+                "postalCode": "10164"
+            }
+        },
+        "additionalMetaData": {
+            "key": "value"
+        },
+        "subscriptionParams": {
+            "planId": "plan-revvenu-basic"
+        }
+    }
+})
+
+print(data.provision_customer.customer.name)
+
+```
+
+Get a customer by ID
+
+```python
+
+import os
+from stigg import Stigg
+
+api_key = os.environ.get("STIGG_SERVER_API_KEY")
+
+client = Stigg.create_client(api_key)
+
+data = client.request(Stigg.query.get_customer_by_id, {
+  "input": {"customerId": "customer-id"}
+})
 
-packages = \
-['stigg', 'stigg.generated']
+customer = data.get_customer_by_ref_id
+print(customer.name)
 
-package_data = \
-{'': ['*']}
+```
 
-install_requires = \
-['black>=22.8.0,<23.0.0',
- 'flake8>=5.0.4,<6.0.0',
- 'graphql-core==3.1.6',
- 'requests>=2.28.1,<3.0.0',
- 'sgqlc>=16.0,<17.0']
-
-setup_kwargs = {
-    'name': 'stigg-api-client',
-    'version': '0.3.0',
-    'description': '',
-    'long_description': '# stigg-api-client\n\nThis library provides a Python wrapper to [Stigg\'s GraphQL API](https://docs.stigg.io/docs/graphql-api) based on \nthe operations that are in use by the [Stigg\'s Node.js SDK](https://docs.stigg.io/docs/nodejs-sdk).\n\nIt leverages the [sgqlc](https://github.com/profusion/sgqlc) library to generate Python classes for GraphQL types, and\nutilizes the `sgqlc.endpoint.requests.RequestsEndpoint` class to send the API requests. The responses are being\nautomatically converted into native Python types.\n\n## Documentation\n\nSee https://docs.stigg.io/docs/python-sdk\n\n## Installation\n\n    pip install stigg-api-client\n\n## Usage\n\nInitialize the client:\n\n```python\n\nimport os\nfrom stigg import Stigg\n\napi_key = os.environ.get("STIGG_SERVER_API_KEY")\n\nstigg_client = Stigg.create_client(api_key)\n\n```\n\nProvision a customer\n\n```python\n\nimport os\nfrom stigg import Stigg\n\napi_key = os.environ.get("STIGG_SERVER_API_KEY")\n\nclient = Stigg.create_client(api_key)\n\ndata = client.request(Stigg.mutation.provision_customer, {\n    "input": {\n        "refId": "customer-id",\n        "name": "Acme",\n        "email": "hello@acme.com",\n        "couponRefId": "coupon-id",\n        "billingInformation": {\n            "language": "en",\n            "timezone": "America/New_York",\n            "billingAddress": {\n                "country": "US",\n                "city": "New York",\n                "state": "NY",\n                "addressLine1": "123 Main Street",\n                "addressLine2": "Apt. 1",\n                "phoneNumber": "+1 212-499-5321",\n                "postalCode": "10164"\n            },\n            "shippingAddress": {\n                "country": "US",\n                "city": "New York",\n                "state": "NY",\n                "addressLine1": "123 Main Street",\n                "addressLine2": "Apt. 1",\n                "phoneNumber": "+1 212-499-5321",\n                "postalCode": "10164"\n            }\n        },\n        "additionalMetaData": {\n            "key": "value"\n        },\n        "subscriptionParams": {\n            "planId": "plan-revvenu-basic"\n        }\n    }\n})\n\nprint(data.provision_customer.customer.name)\n\n```\n\nGet a customer by ID\n\n```python\n\nimport os\nfrom stigg import Stigg\n\napi_key = os.environ.get("STIGG_SERVER_API_KEY")\n\nclient = Stigg.create_client(api_key)\n\ndata = client.request(Stigg.query.get_customer_by_id, {\n  "input": {"customerId": "customer-id"}\n})\n\ncustomer = data.get_customer_by_ref_id\nprint(customer.name)\n\n```\n',
-    'author': 'Stigg',
-    'author_email': 'support@stigg.io',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

