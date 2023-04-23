# Comparing `tmp/iam_actions-1.2.20230422.tar.gz` & `tmp/iam_actions-1.2.20230423.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230422.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230423.tar", max compression
```

## Comparing `iam_actions-1.2.20230422.tar` & `iam_actions-1.2.20230423.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-04-22 02:26:17.093102 iam_actions-1.2.20230422/LICENSE
--rw-r--r--   0        0        0     2302 2023-04-22 02:26:17.093102 iam_actions-1.2.20230422/README.md
--rw-r--r--   0        0        0      228 2023-04-22 02:26:17.093102 iam_actions-1.2.20230422/iam_actions/__init__.py
--rw-r--r--   0        0        0  4220933 2023-04-22 02:28:09.830322 iam_actions-1.2.20230422/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-04-22 02:26:17.093102 iam_actions-1.2.20230422/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-04-22 02:26:17.093102 iam_actions-1.2.20230422/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-04-22 02:26:17.093102 iam_actions-1.2.20230422/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-04-22 02:26:17.093102 iam_actions-1.2.20230422/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-04-22 02:26:17.093102 iam_actions-1.2.20230422/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-04-22 02:26:17.093102 iam_actions-1.2.20230422/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-04-22 02:26:17.093102 iam_actions-1.2.20230422/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-04-22 02:26:17.093102 iam_actions-1.2.20230422/iam_actions/generate/services.py
--rw-r--r--   0        0        0   543343 2023-04-22 02:28:09.830322 iam_actions-1.2.20230422/iam_actions/policies.json
--rw-r--r--   0        0        0   190303 2023-04-22 02:28:09.830322 iam_actions-1.2.20230422/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   526934 2023-04-22 02:28:09.830322 iam_actions-1.2.20230422/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-04-22 02:28:10.598330 iam_actions-1.2.20230422/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230422/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230422/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-23 02:33:45.186350 iam_actions-1.2.20230423/LICENSE
+-rw-r--r--   0        0        0     2302 2023-04-23 02:33:45.186350 iam_actions-1.2.20230423/README.md
+-rw-r--r--   0        0        0      228 2023-04-23 02:33:45.186350 iam_actions-1.2.20230423/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4220933 2023-04-23 02:35:26.550562 iam_actions-1.2.20230423/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-04-23 02:33:45.186350 iam_actions-1.2.20230423/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-04-23 02:33:45.186350 iam_actions-1.2.20230423/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-04-23 02:33:45.186350 iam_actions-1.2.20230423/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-04-23 02:33:45.190350 iam_actions-1.2.20230423/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-04-23 02:33:45.190350 iam_actions-1.2.20230423/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-04-23 02:33:45.190350 iam_actions-1.2.20230423/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-04-23 02:33:45.190350 iam_actions-1.2.20230423/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-04-23 02:33:45.190350 iam_actions-1.2.20230423/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   543343 2023-04-23 02:35:26.550562 iam_actions-1.2.20230423/iam_actions/policies.json
+-rw-r--r--   0        0        0   190303 2023-04-23 02:35:26.550562 iam_actions-1.2.20230423/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   526934 2023-04-23 02:35:26.550562 iam_actions-1.2.20230423/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-04-23 02:35:27.310563 iam_actions-1.2.20230423/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230423/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230423/PKG-INFO
```

### Comparing `iam_actions-1.2.20230422/LICENSE` & `iam_actions-1.2.20230423/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230422/README.md` & `iam_actions-1.2.20230423/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230422/iam_actions/actions.json` & `iam_actions-1.2.20230423/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -16841,305 +16841,305 @@
             "condition_keys": [],
             "description": "Grants permission to validate an address to be used for 911 calls made with Amazon Chime Voice Connectors",
             "orphan": false,
             "resources": []
         }
     },
     "cleanrooms": {
-        "UpdateMembership": {
-            "access_level": "Undocumented",
-            "action": "UpdateMembership",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
-            "orphan": false,
-            "resources": []
-        },
-        "GetSchemaAnalysisRule": {
+        "DeleteCollaboration": {
             "access_level": "Undocumented",
-            "action": "GetSchemaAnalysisRule",
+            "action": "DeleteCollaboration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListCollaborations": {
+        "GetSchema": {
             "access_level": "Undocumented",
-            "action": "ListCollaborations",
+            "action": "GetSchema",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConfiguredTableAssociation": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "GetConfiguredTableAssociation",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConfiguredTableAnalysisRule": {
+        "ListMemberships": {
             "access_level": "Undocumented",
-            "action": "CreateConfiguredTableAnalysisRule",
+            "action": "ListMemberships",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateMembership": {
+        "UpdateCollaboration": {
             "access_level": "Undocumented",
-            "action": "CreateMembership",
+            "action": "UpdateCollaboration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListConfiguredTables": {
             "access_level": "Undocumented",
             "action": "ListConfiguredTables",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConfiguredTable": {
+        "UpdateConfiguredTable": {
             "access_level": "Undocumented",
-            "action": "DeleteConfiguredTable",
+            "action": "UpdateConfiguredTable",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMembers": {
+        "UpdateMembership": {
             "access_level": "Undocumented",
-            "action": "ListMembers",
+            "action": "UpdateMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "GetCollaboration": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "GetCollaboration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateConfiguredTable": {
+        "CreateMembership": {
             "access_level": "Undocumented",
-            "action": "UpdateConfiguredTable",
+            "action": "CreateMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConfiguredTableAssociation": {
+        "CreateConfiguredTable": {
             "access_level": "Undocumented",
-            "action": "DeleteConfiguredTableAssociation",
+            "action": "CreateConfiguredTable",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartProtectedQuery": {
+        "GetConfiguredTableAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "StartProtectedQuery",
+            "action": "GetConfiguredTableAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCollaboration": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "GetCollaboration",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSchemas": {
+        "DeleteConfiguredTableAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "ListSchemas",
+            "action": "DeleteConfiguredTableAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "UpdateConfiguredTableAssociation": {
             "access_level": "Undocumented",
             "action": "UpdateConfiguredTableAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConfiguredTable": {
+        "ListProtectedQueries": {
             "access_level": "Undocumented",
-            "action": "CreateConfiguredTable",
+            "action": "ListProtectedQueries",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "UpdateProtectedQuery": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "UpdateProtectedQuery",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchGetSchema": {
+        "ListSchemas": {
             "access_level": "Undocumented",
-            "action": "BatchGetSchema",
+            "action": "ListSchemas",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "UpdateConfiguredTableAnalysisRule": {
             "access_level": "Undocumented",
             "action": "UpdateConfiguredTableAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConfiguredTableAssociation": {
+        "StartProtectedQuery": {
             "access_level": "Undocumented",
-            "action": "CreateConfiguredTableAssociation",
+            "action": "StartProtectedQuery",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListConfiguredTableAssociations": {
+        "GetConfiguredTable": {
             "access_level": "Undocumented",
-            "action": "ListConfiguredTableAssociations",
+            "action": "GetConfiguredTable",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConfiguredTable": {
+        "DeleteMembership": {
             "access_level": "Undocumented",
-            "action": "GetConfiguredTable",
+            "action": "DeleteMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProtectedQueries": {
+        "BatchGetSchema": {
             "access_level": "Undocumented",
-            "action": "ListProtectedQueries",
+            "action": "BatchGetSchema",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConfiguredTableAnalysisRule": {
+        "GetSchemaAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "GetConfiguredTableAnalysisRule",
+            "action": "GetSchemaAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateCollaboration": {
+        "CreateConfiguredTableAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "CreateCollaboration",
+            "action": "CreateConfiguredTableAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteCollaboration": {
+        "ListMembers": {
             "access_level": "Undocumented",
-            "action": "DeleteCollaboration",
+            "action": "ListMembers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMembership": {
+        "GetConfiguredTableAssociation": {
             "access_level": "Undocumented",
-            "action": "GetMembership",
+            "action": "GetConfiguredTableAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSchema": {
+        "CreateCollaboration": {
             "access_level": "Undocumented",
-            "action": "GetSchema",
+            "action": "CreateCollaboration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteMembership": {
+        "GetProtectedQuery": {
             "access_level": "Undocumented",
-            "action": "DeleteMembership",
+            "action": "GetProtectedQuery",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteMember": {
+        "ListCollaborations": {
             "access_level": "Undocumented",
-            "action": "DeleteMember",
+            "action": "ListCollaborations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetProtectedQuery": {
+        "DeleteConfiguredTableAssociation": {
             "access_level": "Undocumented",
-            "action": "GetProtectedQuery",
+            "action": "DeleteConfiguredTableAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMemberships": {
+        "ListConfiguredTableAssociations": {
             "access_level": "Undocumented",
-            "action": "ListMemberships",
+            "action": "ListConfiguredTableAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateCollaboration": {
+        "CreateConfiguredTableAssociation": {
             "access_level": "Undocumented",
-            "action": "UpdateCollaboration",
+            "action": "CreateConfiguredTableAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConfiguredTableAnalysisRule": {
+        "GetMembership": {
             "access_level": "Undocumented",
-            "action": "DeleteConfiguredTableAnalysisRule",
+            "action": "GetMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateProtectedQuery": {
+        "DeleteConfiguredTable": {
             "access_level": "Undocumented",
-            "action": "UpdateProtectedQuery",
+            "action": "DeleteConfiguredTable",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DeleteMember": {
+            "access_level": "Undocumented",
+            "action": "DeleteMember",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "cloud9": {
@@ -24485,73 +24485,73 @@
             "orphan": false,
             "resources": [
                 "association"
             ]
         }
     },
     "codeguru-security": {
-        "DeleteScansByCategory": {
+        "CreateUploadUrl": {
             "access_level": "Undocumented",
-            "action": "DeleteScansByCategory",
+            "action": "CreateUploadUrl",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFindings": {
+        "ListScans": {
             "access_level": "Undocumented",
-            "action": "ListFindings",
+            "action": "ListScans",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateScan": {
+        "BatchGetFindings": {
             "access_level": "Undocumented",
-            "action": "CreateScan",
+            "action": "BatchGetFindings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetScan": {
             "access_level": "Undocumented",
             "action": "GetScan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListScans": {
+        "CreateScan": {
             "access_level": "Undocumented",
-            "action": "ListScans",
+            "action": "CreateScan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccountConfiguration": {
+        "ListFindings": {
             "access_level": "Undocumented",
-            "action": "UpdateAccountConfiguration",
+            "action": "ListFindings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateUploadUrl": {
+        "DeleteScansByCategory": {
             "access_level": "Undocumented",
-            "action": "CreateUploadUrl",
+            "action": "DeleteScansByCategory",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchGetFindings": {
+        "UpdateAccountConfiguration": {
             "access_level": "Undocumented",
-            "action": "BatchGetFindings",
+            "action": "UpdateAccountConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "codepipeline": {
@@ -31852,25 +31852,25 @@
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "consolidatedbilling": {
-        "GetAccountBillingRole": {
+        "ListLinkedAccounts": {
             "access_level": "Undocumented",
-            "action": "GetAccountBillingRole",
+            "action": "ListLinkedAccounts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListLinkedAccounts": {
+        "GetAccountBillingRole": {
             "access_level": "Undocumented",
-            "action": "ListLinkedAccounts",
+            "action": "GetAccountBillingRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "controltower": {
@@ -33796,283 +33796,283 @@
             "orphan": false,
             "resources": [
                 "taskexecution"
             ]
         }
     },
     "datazone": {
-        "GetProjectCredentials": {
+        "GetProjectConfiguration": {
             "access_level": "Undocumented",
-            "action": "GetProjectCredentials",
+            "action": "GetProjectConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetProject": {
             "access_level": "Undocumented",
             "action": "GetProject",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetProjectConfiguration": {
+        "ListUserProjects": {
             "access_level": "Undocumented",
-            "action": "GetProjectConfiguration",
+            "action": "ListUserProjects",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListProjects": {
             "access_level": "Undocumented",
             "action": "ListProjects",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListUserProjects": {
+        "GetProjectCredentials": {
             "access_level": "Undocumented",
-            "action": "ListUserProjects",
+            "action": "GetProjectCredentials",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "datazonecontrol": {
-        "CreateDataSource": {
+        "ListDataSources": {
             "access_level": "Undocumented",
-            "action": "CreateDataSource",
+            "action": "ListDataSources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMetadataCollectors": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "ListMetadataCollectors",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAccountAssociationInvitation": {
+        "GetDomain": {
             "access_level": "Undocumented",
-            "action": "CreateAccountAssociationInvitation",
+            "action": "GetDomain",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDataSource": {
+        "ListAccountAssociationInvitations": {
             "access_level": "Undocumented",
-            "action": "DeleteDataSource",
+            "action": "ListAccountAssociationInvitations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDomain": {
+        "DissociateAccount": {
             "access_level": "Undocumented",
-            "action": "GetDomain",
+            "action": "DissociateAccount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateEnvironment": {
             "access_level": "Undocumented",
             "action": "CreateEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAllAssociatedAccountsForEnvironment": {
+        "ListDomains": {
             "access_level": "Undocumented",
-            "action": "ListAllAssociatedAccountsForEnvironment",
+            "action": "ListDomains",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "DeleteDataSource": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "DeleteDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetAssociatedDomain": {
             "access_level": "Undocumented",
             "action": "GetAssociatedDomain",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteEnvironment": {
+        "GetMetadataCollector": {
             "access_level": "Undocumented",
-            "action": "DeleteEnvironment",
+            "action": "GetMetadataCollector",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMetadataCollectorRuns": {
+        "ListDataSourcesByEnvironment": {
             "access_level": "Undocumented",
-            "action": "ListMetadataCollectorRuns",
+            "action": "ListDataSourcesByEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAccountAssociationInvitations": {
+        "ListAllAssociatedAccountsForEnvironment": {
             "access_level": "Undocumented",
-            "action": "ListAccountAssociationInvitations",
+            "action": "ListAllAssociatedAccountsForEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDataSourcesByEnvironment": {
+        "GetEnvironment": {
             "access_level": "Undocumented",
-            "action": "ListDataSourcesByEnvironment",
+            "action": "GetEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccountAssociationDescription": {
+        "ListMetadataCollectorRuns": {
             "access_level": "Undocumented",
-            "action": "UpdateAccountAssociationDescription",
+            "action": "ListMetadataCollectorRuns",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEnvironment": {
+        "UpdateEnvironment": {
             "access_level": "Undocumented",
-            "action": "ListEnvironment",
+            "action": "UpdateEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ReviewAccountAssociationInvitation": {
+        "DeleteEnvironment": {
             "access_level": "Undocumented",
-            "action": "ReviewAccountAssociationInvitation",
+            "action": "DeleteEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DissociateAccount": {
+        "ListAssociatedEnvironments": {
             "access_level": "Undocumented",
-            "action": "DissociateAccount",
+            "action": "ListAssociatedEnvironments",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAssociatedEnvironments": {
+        "GetUserPortalLoginAuthCode": {
             "access_level": "Undocumented",
-            "action": "ListAssociatedEnvironments",
+            "action": "GetUserPortalLoginAuthCode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMetadataCollector": {
+        "UpdateDataSource": {
             "access_level": "Undocumented",
-            "action": "GetMetadataCollector",
+            "action": "UpdateDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDataSourceByEnvironment": {
+        "CreateAccountAssociationInvitation": {
             "access_level": "Undocumented",
-            "action": "GetDataSourceByEnvironment",
+            "action": "CreateAccountAssociationInvitation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDataSources": {
+        "UpdateAccountAssociationDescription": {
             "access_level": "Undocumented",
-            "action": "ListDataSources",
+            "action": "UpdateAccountAssociationDescription",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetUserPortalLoginAuthCode": {
+        "ListEnvironment": {
             "access_level": "Undocumented",
-            "action": "GetUserPortalLoginAuthCode",
+            "action": "ListEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateEnvironment": {
+        "ListMetadataCollectors": {
             "access_level": "Undocumented",
-            "action": "UpdateEnvironment",
+            "action": "ListMetadataCollectors",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEnvironment": {
+        "ReviewAccountAssociationInvitation": {
             "access_level": "Undocumented",
-            "action": "GetEnvironment",
+            "action": "ReviewAccountAssociationInvitation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProjects": {
+        "CreateDataSource": {
             "access_level": "Undocumented",
-            "action": "ListProjects",
+            "action": "CreateDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateDataSource": {
+        "GetDataSourceByEnvironment": {
             "access_level": "Undocumented",
-            "action": "UpdateDataSource",
+            "action": "GetDataSourceByEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDomains": {
+        "ListProjects": {
             "access_level": "Undocumented",
-            "action": "ListDomains",
+            "action": "ListProjects",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "dax": {
@@ -70150,737 +70150,737 @@
             "condition_keys": [],
             "description": "Grants permission to update an Amazon Honeycode team for your AWS Account",
             "orphan": false,
             "resources": []
         }
     },
     "iam": {
-        "GetLoginProfile": {
+        "ListInstanceProfiles": {
             "access_level": "Undocumented",
-            "action": "GetLoginProfile",
+            "action": "ListInstanceProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRoleTags": {
+        "DeleteServerCertificate": {
             "access_level": "Undocumented",
-            "action": "ListRoleTags",
+            "action": "DeleteServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateVirtualMFADevice": {
+        "ResetServiceSpecificCredential": {
             "access_level": "Undocumented",
-            "action": "CreateVirtualMFADevice",
+            "action": "ResetServiceSpecificCredential",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "AddUserToGroup": {
             "access_level": "Undocumented",
             "action": "AddUserToGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteUserPermissionsBoundary": {
+        "DeleteSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "DeleteUserPermissionsBoundary",
+            "action": "DeleteSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListUserTags": {
+        "DeleteSSHPublicKey": {
             "access_level": "Undocumented",
-            "action": "ListUserTags",
+            "action": "DeleteSSHPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGroupPolicies": {
+        "ListUserPolicies": {
             "access_level": "Undocumented",
-            "action": "ListGroupPolicies",
+            "action": "ListUserPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ResyncMFADevice": {
+        "GetAccountPasswordPolicy": {
             "access_level": "Undocumented",
-            "action": "ResyncMFADevice",
+            "action": "GetAccountPasswordPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagServerCertificate": {
+        "ChangePassword": {
             "access_level": "Undocumented",
-            "action": "UntagServerCertificate",
+            "action": "ChangePassword",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteUser": {
+        "GetInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "DeleteUser",
+            "action": "GetInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagSAMLProvider": {
+        "UpdateAccessKey": {
             "access_level": "Undocumented",
-            "action": "UntagSAMLProvider",
+            "action": "UpdateAccessKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "EnableMFADevice": {
+        "SimulateCustomPolicy": {
             "access_level": "Undocumented",
-            "action": "EnableMFADevice",
+            "action": "SimulateCustomPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetContextKeysForCustomPolicy": {
+        "DeletePolicyVersion": {
             "access_level": "Undocumented",
-            "action": "GetContextKeysForCustomPolicy",
+            "action": "DeletePolicyVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRolePolicies": {
+        "DeleteGroupPolicy": {
             "access_level": "Undocumented",
-            "action": "ListRolePolicies",
+            "action": "DeleteGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetSTSRegionalEndpointStatus": {
+        "UploadSSHPublicKey": {
             "access_level": "Undocumented",
-            "action": "SetSTSRegionalEndpointStatus",
+            "action": "UploadSSHPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServerCertificate": {
+        "GetAccountName": {
             "access_level": "Undocumented",
-            "action": "GetServerCertificate",
+            "action": "GetAccountName",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetOpenIDConnectProvider": {
+        "GetGroupPolicy": {
             "access_level": "Undocumented",
-            "action": "GetOpenIDConnectProvider",
+            "action": "GetGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeactivateMFADevice": {
+        "GetAccountSummary": {
             "access_level": "Undocumented",
-            "action": "DeactivateMFADevice",
+            "action": "GetAccountSummary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPoliciesGrantingServiceAccess": {
+        "PutUserPermissionsBoundary": {
             "access_level": "Undocumented",
-            "action": "ListPoliciesGrantingServiceAccess",
+            "action": "PutUserPermissionsBoundary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListUsers": {
+        "DeleteAccountAlias": {
             "access_level": "Undocumented",
-            "action": "ListUsers",
+            "action": "DeleteAccountAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCloudFrontPublicKey": {
+        "CreateServiceSpecificCredential": {
             "access_level": "Undocumented",
-            "action": "GetCloudFrontPublicKey",
+            "action": "CreateServiceSpecificCredential",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListInstanceProfilesForRole": {
+        "AttachRolePolicy": {
             "access_level": "Undocumented",
-            "action": "ListInstanceProfilesForRole",
+            "action": "AttachRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagSAMLProvider": {
+        "UntagRole": {
             "access_level": "Undocumented",
-            "action": "TagSAMLProvider",
+            "action": "UntagRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSSHPublicKey": {
+        "UntagOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "DeleteSSHPublicKey",
+            "action": "UntagOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveRoleFromInstanceProfile": {
+        "TagPolicy": {
             "access_level": "Undocumented",
-            "action": "RemoveRoleFromInstanceProfile",
+            "action": "TagPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicies": {
+        "TagServerCertificate": {
             "access_level": "Undocumented",
-            "action": "ListPolicies",
+            "action": "TagServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateCloudFrontPublicKey": {
+        "GetServiceLastAccessedDetails": {
             "access_level": "Undocumented",
-            "action": "UpdateCloudFrontPublicKey",
+            "action": "GetServiceLastAccessedDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetDefaultPolicyVersion": {
+        "GetUserPolicy": {
             "access_level": "Undocumented",
-            "action": "SetDefaultPolicyVersion",
+            "action": "GetUserPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagOpenIDConnectProvider": {
+        "ListRoleTags": {
             "access_level": "Undocumented",
-            "action": "TagOpenIDConnectProvider",
+            "action": "ListRoleTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRolePolicy": {
+        "CreatePolicy": {
             "access_level": "Undocumented",
-            "action": "GetRolePolicy",
+            "action": "CreatePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAccessKey": {
+        "DeleteAccountPasswordPolicy": {
             "access_level": "Undocumented",
-            "action": "CreateAccessKey",
+            "action": "DeleteAccountPasswordPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagRole": {
+        "TagRole": {
             "access_level": "Undocumented",
-            "action": "UntagRole",
+            "action": "TagRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSigningCertificates": {
+        "UploadSigningCertificate": {
             "access_level": "Undocumented",
-            "action": "ListSigningCertificates",
+            "action": "UploadSigningCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetContextKeysForPrincipalPolicy": {
+        "DeleteSigningCertificate": {
             "access_level": "Undocumented",
-            "action": "GetContextKeysForPrincipalPolicy",
+            "action": "DeleteSigningCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAttachedUserPolicies": {
+        "UntagServerCertificate": {
             "access_level": "Undocumented",
-            "action": "ListAttachedUserPolicies",
+            "action": "UntagServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagOpenIDConnectProvider": {
+        "DeleteRolePermissionsBoundary": {
             "access_level": "Undocumented",
-            "action": "UntagOpenIDConnectProvider",
+            "action": "DeleteRolePermissionsBoundary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UploadSSHPublicKey": {
+        "DeleteGroup": {
             "access_level": "Undocumented",
-            "action": "UploadSSHPublicKey",
+            "action": "DeleteGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRolePolicy": {
+        "DetachRolePolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteRolePolicy",
+            "action": "DetachRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagServerCertificate": {
+        "EnableMFADevice": {
             "access_level": "Undocumented",
-            "action": "TagServerCertificate",
+            "action": "EnableMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountEmailAddress": {
+        "GetPolicy": {
             "access_level": "Undocumented",
-            "action": "GetAccountEmailAddress",
+            "action": "GetPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateServerCertificate": {
+        "CreateServiceLinkedRole": {
             "access_level": "Undocumented",
-            "action": "UpdateServerCertificate",
+            "action": "CreateServiceLinkedRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UploadServerCertificate": {
+        "DeleteServiceLinkedRole": {
             "access_level": "Undocumented",
-            "action": "UploadServerCertificate",
+            "action": "DeleteServiceLinkedRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteOpenIDConnectProvider": {
+        "ListPolicyVersions": {
             "access_level": "Undocumented",
-            "action": "DeleteOpenIDConnectProvider",
+            "action": "ListPolicyVersions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AttachGroupPolicy": {
+        "ListGroupPolicies": {
             "access_level": "Undocumented",
-            "action": "AttachGroupPolicy",
+            "action": "ListGroupPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetUserPolicy": {
+        "PutGroupPolicy": {
             "access_level": "Undocumented",
-            "action": "GetUserPolicy",
+            "action": "PutGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountAuthorizationDetails": {
+        "DetachUserPolicy": {
             "access_level": "Undocumented",
-            "action": "GetAccountAuthorizationDetails",
+            "action": "DetachUserPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEntitiesForPolicy": {
+        "ListAccountAliases": {
             "access_level": "Undocumented",
-            "action": "ListEntitiesForPolicy",
+            "action": "ListAccountAliases",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAttachedGroupPolicies": {
+        "ListSigningCertificates": {
             "access_level": "Undocumented",
-            "action": "ListAttachedGroupPolicies",
+            "action": "ListSigningCertificates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutGroupPolicy": {
+        "ListEntitiesForPolicy": {
             "access_level": "Undocumented",
-            "action": "PutGroupPolicy",
+            "action": "ListEntitiesForPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagRole": {
+        "CreateLoginProfile": {
             "access_level": "Undocumented",
-            "action": "TagRole",
+            "action": "CreateLoginProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateRoleDescription": {
+        "CreateOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "UpdateRoleDescription",
+            "action": "CreateOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAccountAliases": {
+        "DeleteServiceSpecificCredential": {
             "access_level": "Undocumented",
-            "action": "ListAccountAliases",
+            "action": "DeleteServiceSpecificCredential",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListInstanceProfileTags": {
+        "TagInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "ListInstanceProfileTags",
+            "action": "TagInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateRole": {
+        "DetachGroupPolicy": {
             "access_level": "Undocumented",
-            "action": "UpdateRole",
+            "action": "DetachGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateRole": {
+        "UploadServerCertificate": {
             "access_level": "Undocumented",
-            "action": "CreateRole",
+            "action": "UploadServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveUserFromGroup": {
+        "ListSAMLProviders": {
             "access_level": "Undocumented",
-            "action": "RemoveUserFromGroup",
+            "action": "ListSAMLProviders",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateServiceSpecificCredential": {
+        "CreateGroup": {
             "access_level": "Undocumented",
-            "action": "CreateServiceSpecificCredential",
+            "action": "CreateGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteUserPolicy": {
+        "UpdateGroup": {
             "access_level": "Undocumented",
-            "action": "DeleteUserPolicy",
+            "action": "UpdateGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMFADevices": {
+        "GetLoginProfile": {
             "access_level": "Undocumented",
-            "action": "ListMFADevices",
+            "action": "GetLoginProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateGroup": {
+        "CreatePolicyVersion": {
             "access_level": "Undocumented",
-            "action": "CreateGroup",
+            "action": "CreatePolicyVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRoles": {
+        "GenerateServiceLastAccessedDetails": {
             "access_level": "Undocumented",
-            "action": "ListRoles",
+            "action": "GenerateServiceLastAccessedDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRole": {
+        "SetDefaultPolicyVersion": {
             "access_level": "Undocumented",
-            "action": "GetRole",
+            "action": "SetDefaultPolicyVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListUserPolicies": {
+        "GetUser": {
             "access_level": "Undocumented",
-            "action": "ListUserPolicies",
+            "action": "GetUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateGroup": {
+        "SetSecurityTokenServicePreferences": {
             "access_level": "Undocumented",
-            "action": "UpdateGroup",
+            "action": "SetSecurityTokenServicePreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddClientIDToOpenIDConnectProvider": {
+        "ListServiceSpecificCredentials": {
             "access_level": "Undocumented",
-            "action": "AddClientIDToOpenIDConnectProvider",
+            "action": "ListServiceSpecificCredentials",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAccessKeys": {
+        "GetRole": {
             "access_level": "Undocumented",
-            "action": "ListAccessKeys",
+            "action": "GetRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSSHPublicKey": {
+        "ListSTSRegionalEndpointsStatus": {
             "access_level": "Undocumented",
-            "action": "GetSSHPublicKey",
+            "action": "ListSTSRegionalEndpointsStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListOpenIDConnectProviderTags": {
+        "DeleteInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "ListOpenIDConnectProviderTags",
+            "action": "DeleteInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagUser": {
+        "AddRoleToInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "UntagUser",
+            "action": "AddRoleToInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AttachUserPolicy": {
+        "ListPolicyTags": {
             "access_level": "Undocumented",
-            "action": "AttachUserPolicy",
+            "action": "ListPolicyTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagPolicy": {
+        "GenerateOrganizationsAccessReport": {
             "access_level": "Undocumented",
-            "action": "TagPolicy",
+            "action": "GenerateOrganizationsAccessReport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSTSRegionalEndpointsStatus": {
+        "ListUserTags": {
             "access_level": "Undocumented",
-            "action": "ListSTSRegionalEndpointsStatus",
+            "action": "ListUserTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagMFADevice": {
+        "PutRolePolicy": {
             "access_level": "Undocumented",
-            "action": "UntagMFADevice",
+            "action": "PutRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateUser": {
             "access_level": "Undocumented",
             "action": "CreateUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateServiceLinkedRole": {
+        "ListPolicies": {
             "access_level": "Undocumented",
-            "action": "CreateServiceLinkedRole",
+            "action": "ListPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePolicy": {
+        "GenerateCredentialReport": {
             "access_level": "Undocumented",
-            "action": "CreatePolicy",
+            "action": "GenerateCredentialReport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceLinkedRoleDeletionStatus": {
+        "ListGroups": {
             "access_level": "Undocumented",
-            "action": "GetServiceLinkedRoleDeletionStatus",
+            "action": "ListGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DetachUserPolicy": {
+        "DeleteAccessKey": {
             "access_level": "Undocumented",
-            "action": "DetachUserPolicy",
+            "action": "DeleteAccessKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAccountPasswordPolicy": {
+        "TagMFADevice": {
             "access_level": "Undocumented",
-            "action": "DeleteAccountPasswordPolicy",
+            "action": "TagMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountSummary": {
+        "UntagMFADevice": {
             "access_level": "Undocumented",
-            "action": "GetAccountSummary",
+            "action": "UntagMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGroupPolicy": {
+        "GetGroup": {
             "access_level": "Undocumented",
-            "action": "GetGroupPolicy",
+            "action": "GetGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetOrganizationsAccessReport": {
+        "UpdateServiceSpecificCredential": {
             "access_level": "Undocumented",
-            "action": "GetOrganizationsAccessReport",
+            "action": "UpdateServiceSpecificCredential",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSSHPublicKeys": {
+        "GetServerCertificate": {
             "access_level": "Undocumented",
-            "action": "ListSSHPublicKeys",
+            "action": "GetServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSAMLProvider": {
+        "CreateInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "CreateSAMLProvider",
+            "action": "CreateInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteServiceSpecificCredential": {
+        "UntagInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "DeleteServiceSpecificCredential",
+            "action": "UntagInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SimulateCustomPolicy": {
+        "UpdateCloudFrontPublicKey": {
             "access_level": "Undocumented",
-            "action": "SimulateCustomPolicy",
+            "action": "UpdateCloudFrontPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAssumeRolePolicy": {
+        "UpdateSigningCertificate": {
             "access_level": "Undocumented",
-            "action": "UpdateAssumeRolePolicy",
+            "action": "UpdateSigningCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPolicy": {
+        "ListVirtualMFADevices": {
             "access_level": "Undocumented",
-            "action": "GetPolicy",
+            "action": "ListVirtualMFADevices",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PassRole": {
+        "PutRolePermissionsBoundary": {
             "access_level": "Undocumented",
-            "action": "PassRole",
+            "action": "PutRolePermissionsBoundary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutUserPolicy": {
+        "DeleteRolePolicy": {
             "access_level": "Undocumented",
-            "action": "PutUserPolicy",
+            "action": "DeleteRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateInstanceProfile": {
+        "GetAccountAuthorizationDetails": {
             "access_level": "Undocumented",
-            "action": "CreateInstanceProfile",
+            "action": "GetAccountAuthorizationDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListAttachedRolePolicies": {
             "access_level": "Undocumented",
@@ -70894,625 +70894,625 @@
             "access_level": "Undocumented",
             "action": "GetAccessKeyLastUsed",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSAMLProviders": {
+        "ListAccessKeys": {
             "access_level": "Undocumented",
-            "action": "ListSAMLProviders",
+            "action": "ListAccessKeys",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountPasswordPolicy": {
+        "UpdateAccountName": {
             "access_level": "Undocumented",
-            "action": "GetAccountPasswordPolicy",
+            "action": "UpdateAccountName",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAccountAlias": {
+        "SimulatePrincipalPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteAccountAlias",
+            "action": "SimulatePrincipalPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteInstanceProfile": {
+        "UntagUser": {
             "access_level": "Undocumented",
-            "action": "DeleteInstanceProfile",
+            "action": "UntagUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutRolePolicy": {
+        "UpdateLoginProfile": {
             "access_level": "Undocumented",
-            "action": "PutRolePolicy",
+            "action": "UpdateLoginProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagInstanceProfile": {
+        "CreateAccountAlias": {
             "access_level": "Undocumented",
-            "action": "UntagInstanceProfile",
+            "action": "CreateAccountAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAccessKey": {
+        "UpdateAccountEmailAddress": {
             "access_level": "Undocumented",
-            "action": "DeleteAccessKey",
+            "action": "UpdateAccountEmailAddress",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagInstanceProfile": {
+        "UpdateRoleDescription": {
             "access_level": "Undocumented",
-            "action": "TagInstanceProfile",
+            "action": "UpdateRoleDescription",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DetachGroupPolicy": {
+        "GetSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "DetachGroupPolicy",
+            "action": "GetSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMFADeviceTags": {
+        "RemoveUserFromGroup": {
             "access_level": "Undocumented",
-            "action": "ListMFADeviceTags",
+            "action": "RemoveUserFromGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCredentialReport": {
+        "ListMFADevices": {
             "access_level": "Undocumented",
-            "action": "GetCredentialReport",
+            "action": "ListMFADevices",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteVirtualMFADevice": {
+        "GetServiceLastAccessedDetailsWithEntities": {
             "access_level": "Undocumented",
-            "action": "DeleteVirtualMFADevice",
+            "action": "GetServiceLastAccessedDetailsWithEntities",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteGroupPolicy": {
+        "UpdateOpenIDConnectProviderThumbprint": {
             "access_level": "Undocumented",
-            "action": "DeleteGroupPolicy",
+            "action": "UpdateOpenIDConnectProviderThumbprint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccountPasswordPolicy": {
+        "CreateAccessKey": {
             "access_level": "Undocumented",
-            "action": "UpdateAccountPasswordPolicy",
+            "action": "CreateAccessKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListOpenIDConnectProviders": {
+        "AttachUserPolicy": {
             "access_level": "Undocumented",
-            "action": "ListOpenIDConnectProviders",
+            "action": "AttachUserPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateLoginProfile": {
+        "ListSSHPublicKeys": {
             "access_level": "Undocumented",
-            "action": "UpdateLoginProfile",
+            "action": "ListSSHPublicKeys",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GenerateOrganizationsAccessReport": {
+        "ResyncMFADevice": {
             "access_level": "Undocumented",
-            "action": "GenerateOrganizationsAccessReport",
+            "action": "ResyncMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateOpenIDConnectProviderThumbprint": {
+        "UpdateSSHPublicKey": {
             "access_level": "Undocumented",
-            "action": "UpdateOpenIDConnectProviderThumbprint",
+            "action": "UpdateSSHPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AttachRolePolicy": {
+        "CreateVirtualMFADevice": {
             "access_level": "Undocumented",
-            "action": "AttachRolePolicy",
+            "action": "CreateVirtualMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRolePermissionsBoundary": {
+        "DeleteRole": {
             "access_level": "Undocumented",
-            "action": "DeleteRolePermissionsBoundary",
+            "action": "DeleteRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteCloudFrontPublicKey": {
+        "ListRoles": {
             "access_level": "Undocumented",
-            "action": "DeleteCloudFrontPublicKey",
+            "action": "ListRoles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UploadSigningCertificate": {
+        "CreateSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "UploadSigningCertificate",
+            "action": "CreateSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListInstanceProfiles": {
+        "TagSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "ListInstanceProfiles",
+            "action": "TagSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicyTags": {
+        "SetSTSRegionalEndpointStatus": {
             "access_level": "Undocumented",
-            "action": "ListPolicyTags",
+            "action": "SetSTSRegionalEndpointStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetUser": {
+        "AddClientIDToOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "GetUser",
+            "action": "AddClientIDToOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetSecurityTokenServicePreferences": {
+        "RemoveRoleFromInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "SetSecurityTokenServicePreferences",
+            "action": "RemoveRoleFromInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutRolePermissionsBoundary": {
+        "ListServerCertificateTags": {
             "access_level": "Undocumented",
-            "action": "PutRolePermissionsBoundary",
+            "action": "ListServerCertificateTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRole": {
+        "PutUserPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteRole",
+            "action": "PutUserPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutUserPermissionsBoundary": {
+        "ListServerCertificates": {
             "access_level": "Undocumented",
-            "action": "PutUserPermissionsBoundary",
+            "action": "ListServerCertificates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicyVersions": {
+        "UpdateServerCertificate": {
             "access_level": "Undocumented",
-            "action": "ListPolicyVersions",
+            "action": "UpdateServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSAMLProvider": {
+        "TagOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "GetSAMLProvider",
+            "action": "TagOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagPolicy": {
+        "ListCloudFrontPublicKeys": {
             "access_level": "Undocumented",
-            "action": "UntagPolicy",
+            "action": "ListCloudFrontPublicKeys",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SimulatePrincipalPolicy": {
+        "UploadCloudFrontPublicKey": {
             "access_level": "Undocumented",
-            "action": "SimulatePrincipalPolicy",
+            "action": "UploadCloudFrontPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListVirtualMFADevices": {
+        "DeleteOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "ListVirtualMFADevices",
+            "action": "DeleteOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccessKey": {
+        "DeleteVirtualMFADevice": {
             "access_level": "Undocumented",
-            "action": "UpdateAccessKey",
+            "action": "DeleteVirtualMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListServerCertificateTags": {
+        "GetAccountEmailAddress": {
             "access_level": "Undocumented",
-            "action": "ListServerCertificateTags",
+            "action": "GetAccountEmailAddress",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateLoginProfile": {
+        "GetOrganizationsAccessReport": {
             "access_level": "Undocumented",
-            "action": "CreateLoginProfile",
+            "action": "GetOrganizationsAccessReport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ChangePassword": {
+        "GetPolicyVersion": {
             "access_level": "Undocumented",
-            "action": "ChangePassword",
+            "action": "GetPolicyVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceLastAccessedDetailsWithEntities": {
+        "GetServiceLinkedRoleDeletionStatus": {
             "access_level": "Undocumented",
-            "action": "GetServiceLastAccessedDetailsWithEntities",
+            "action": "GetServiceLinkedRoleDeletionStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccountName": {
+        "GetContextKeysForCustomPolicy": {
             "access_level": "Undocumented",
-            "action": "UpdateAccountName",
+            "action": "GetContextKeysForCustomPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListCloudFrontPublicKeys": {
+        "UpdateAccountPasswordPolicy": {
             "access_level": "Undocumented",
-            "action": "ListCloudFrontPublicKeys",
+            "action": "UpdateAccountPasswordPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccountEmailAddress": {
+        "GetContextKeysForPrincipalPolicy": {
             "access_level": "Undocumented",
-            "action": "UpdateAccountEmailAddress",
+            "action": "GetContextKeysForPrincipalPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePolicyVersion": {
+        "ListOpenIDConnectProviders": {
             "access_level": "Undocumented",
-            "action": "DeletePolicyVersion",
+            "action": "ListOpenIDConnectProviders",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagMFADevice": {
+        "ListPoliciesGrantingServiceAccess": {
             "access_level": "Undocumented",
-            "action": "TagMFADevice",
+            "action": "ListPoliciesGrantingServiceAccess",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteServiceLinkedRole": {
+        "ListSAMLProviderTags": {
             "access_level": "Undocumented",
-            "action": "DeleteServiceLinkedRole",
+            "action": "ListSAMLProviderTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSigningCertificate": {
+        "GetCredentialReport": {
             "access_level": "Undocumented",
-            "action": "UpdateSigningCertificate",
+            "action": "GetCredentialReport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePolicyVersion": {
+        "ListUsers": {
             "access_level": "Undocumented",
-            "action": "CreatePolicyVersion",
+            "action": "ListUsers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPolicyVersion": {
+        "TagUser": {
             "access_level": "Undocumented",
-            "action": "GetPolicyVersion",
+            "action": "TagUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateServiceSpecificCredential": {
+        "GetSSHPublicKey": {
             "access_level": "Undocumented",
-            "action": "UpdateServiceSpecificCredential",
+            "action": "GetSSHPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DetachRolePolicy": {
+        "ListInstanceProfilesForRole": {
             "access_level": "Undocumented",
-            "action": "DetachRolePolicy",
+            "action": "ListInstanceProfilesForRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteGroup": {
+        "UpdateSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "DeleteGroup",
+            "action": "UpdateSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSSHPublicKey": {
+        "UntagSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "UpdateSSHPublicKey",
+            "action": "UntagSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteServerCertificate": {
+        "DeleteUserPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteServerCertificate",
+            "action": "DeleteUserPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSigningCertificate": {
+        "DeleteLoginProfile": {
             "access_level": "Undocumented",
-            "action": "DeleteSigningCertificate",
+            "action": "DeleteLoginProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGroup": {
+        "DeletePolicy": {
             "access_level": "Undocumented",
-            "action": "GetGroup",
+            "action": "DeletePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSAMLProviderTags": {
+        "ListMFADeviceTags": {
             "access_level": "Undocumented",
-            "action": "ListSAMLProviderTags",
+            "action": "ListMFADeviceTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddRoleToInstanceProfile": {
+        "UpdateUser": {
             "access_level": "Undocumented",
-            "action": "AddRoleToInstanceProfile",
+            "action": "UpdateUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountName": {
+        "UpdateRole": {
             "access_level": "Undocumented",
-            "action": "GetAccountName",
+            "action": "UpdateRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListServerCertificates": {
+        "ListInstanceProfileTags": {
             "access_level": "Undocumented",
-            "action": "ListServerCertificates",
+            "action": "ListInstanceProfileTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagUser": {
+        "ListRolePolicies": {
             "access_level": "Undocumented",
-            "action": "TagUser",
+            "action": "ListRolePolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSAMLProvider": {
+        "PassRole": {
             "access_level": "Undocumented",
-            "action": "DeleteSAMLProvider",
+            "action": "PassRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSAMLProvider": {
+        "ListGroupsForUser": {
             "access_level": "Undocumented",
-            "action": "UpdateSAMLProvider",
+            "action": "ListGroupsForUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteLoginProfile": {
+        "UntagPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteLoginProfile",
+            "action": "UntagPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePolicy": {
+        "GetRolePolicy": {
             "access_level": "Undocumented",
-            "action": "DeletePolicy",
+            "action": "GetRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ResetServiceSpecificCredential": {
+        "GetCloudFrontPublicKey": {
             "access_level": "Undocumented",
-            "action": "ResetServiceSpecificCredential",
+            "action": "GetCloudFrontPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetInstanceProfile": {
+        "GetOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "GetInstanceProfile",
+            "action": "GetOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAccountAlias": {
+        "ListOpenIDConnectProviderTags": {
             "access_level": "Undocumented",
-            "action": "CreateAccountAlias",
+            "action": "ListOpenIDConnectProviderTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGroups": {
+        "CreateRole": {
             "access_level": "Undocumented",
-            "action": "ListGroups",
+            "action": "CreateRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGroupsForUser": {
+        "DeleteUserPermissionsBoundary": {
             "access_level": "Undocumented",
-            "action": "ListGroupsForUser",
+            "action": "DeleteUserPermissionsBoundary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateOpenIDConnectProvider": {
+        "RemoveClientIDFromOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "CreateOpenIDConnectProvider",
+            "action": "RemoveClientIDFromOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GenerateServiceLastAccessedDetails": {
+        "DeleteCloudFrontPublicKey": {
             "access_level": "Undocumented",
-            "action": "GenerateServiceLastAccessedDetails",
+            "action": "DeleteCloudFrontPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateUser": {
+        "DeleteUser": {
             "access_level": "Undocumented",
-            "action": "UpdateUser",
+            "action": "DeleteUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UploadCloudFrontPublicKey": {
+        "DeactivateMFADevice": {
             "access_level": "Undocumented",
-            "action": "UploadCloudFrontPublicKey",
+            "action": "DeactivateMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GenerateCredentialReport": {
+        "ListAttachedGroupPolicies": {
             "access_level": "Undocumented",
-            "action": "GenerateCredentialReport",
+            "action": "ListAttachedGroupPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceLastAccessedDetails": {
+        "ListAttachedUserPolicies": {
             "access_level": "Undocumented",
-            "action": "GetServiceLastAccessedDetails",
+            "action": "ListAttachedUserPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListServiceSpecificCredentials": {
+        "AttachGroupPolicy": {
             "access_level": "Undocumented",
-            "action": "ListServiceSpecificCredentials",
+            "action": "AttachGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveClientIDFromOpenIDConnectProvider": {
+        "UpdateAssumeRolePolicy": {
             "access_level": "Undocumented",
-            "action": "RemoveClientIDFromOpenIDConnectProvider",
+            "action": "UpdateAssumeRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "identity-sync": {
@@ -73280,41 +73280,41 @@
             "orphan": false,
             "resources": [
                 "Monitor"
             ]
         }
     },
     "invoicing": {
-        "GetInvoicePDF": {
+        "PutInvoiceEmailDeliveryPreferences": {
             "access_level": "Undocumented",
-            "action": "GetInvoicePDF",
+            "action": "PutInvoiceEmailDeliveryPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListInvoiceSummaries": {
+        "GetInvoicePDF": {
             "access_level": "Undocumented",
-            "action": "ListInvoiceSummaries",
+            "action": "GetInvoicePDF",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetInvoiceEmailDeliveryPreferences": {
+        "ListInvoiceSummaries": {
             "access_level": "Undocumented",
-            "action": "GetInvoiceEmailDeliveryPreferences",
+            "action": "ListInvoiceSummaries",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutInvoiceEmailDeliveryPreferences": {
+        "GetInvoiceEmailDeliveryPreferences": {
             "access_level": "Undocumented",
-            "action": "PutInvoiceEmailDeliveryPreferences",
+            "action": "GetInvoiceEmailDeliveryPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "iot": {
@@ -79094,889 +79094,889 @@
             "orphan": false,
             "resources": [
                 "workspace"
             ]
         }
     },
     "iotwireless": {
-        "GetResourceLogLevel": {
+        "CreateNetworkAnalyzerConfiguration": {
             "access_level": "Undocumented",
-            "action": "GetResourceLogLevel",
+            "action": "CreateNetworkAnalyzerConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteFuotaTask": {
+        "GetEventConfigurationByResourceTypes": {
             "access_level": "Undocumented",
-            "action": "DeleteFuotaTask",
+            "action": "GetEventConfigurationByResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDeviceProfile": {
+        "DeleteWirelessGatewayTaskDefinition": {
             "access_level": "Undocumented",
-            "action": "GetDeviceProfile",
+            "action": "DeleteWirelessGatewayTaskDefinition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWirelessGatewayTask": {
+        "UpdateLogLevelsByResourceTypes": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessGatewayTask",
+            "action": "UpdateLogLevelsByResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateWirelessGatewayFromThing": {
+        "StartBulkDisassociateWirelessDeviceFromMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessGatewayFromThing",
+            "action": "StartBulkDisassociateWirelessDeviceFromMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetLogLevelsByResourceTypes": {
+        "GetPositionEstimate": {
             "access_level": "Undocumented",
-            "action": "GetLogLevelsByResourceTypes",
+            "action": "GetPositionEstimate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessGatewayWithThing": {
+        "ListPositionConfigurations": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessGatewayWithThing",
+            "action": "ListPositionConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWirelessDevices": {
+        "StartFuotaTask": {
             "access_level": "Undocumented",
-            "action": "ListWirelessDevices",
+            "action": "StartFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWirelessGatewayTaskDefinitions": {
+        "DeleteDeviceProfile": {
             "access_level": "Undocumented",
-            "action": "ListWirelessGatewayTaskDefinitions",
+            "action": "DeleteDeviceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateDestination": {
+        "GetWirelessGatewayStatistics": {
             "access_level": "Undocumented",
-            "action": "UpdateDestination",
+            "action": "GetWirelessGatewayStatistics",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPositionConfigurations": {
+        "ResetResourceLogLevel": {
             "access_level": "Undocumented",
-            "action": "ListPositionConfigurations",
+            "action": "ResetResourceLogLevel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeregisterWirelessDevice": {
+        "GetWirelessGatewayCertificate": {
             "access_level": "Undocumented",
-            "action": "DeregisterWirelessDevice",
+            "action": "GetWirelessGatewayCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateResourcePosition": {
+        "DisassociateWirelessGatewayFromThing": {
             "access_level": "Undocumented",
-            "action": "UpdateResourcePosition",
+            "action": "DisassociateWirelessGatewayFromThing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWirelessDeviceImportTasks": {
+        "ListMulticastGroups": {
             "access_level": "Undocumented",
-            "action": "ListWirelessDeviceImportTasks",
+            "action": "ListMulticastGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPosition": {
+        "GetWirelessGateway": {
             "access_level": "Undocumented",
-            "action": "GetPosition",
+            "action": "GetWirelessGateway",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutResourceLogLevel": {
+        "DeleteWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "PutResourceLogLevel",
+            "action": "DeleteWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "DisassociateWirelessDeviceFromFuotaTask": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "DisassociateWirelessDeviceFromFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceEventConfiguration": {
+        "PutPositionConfiguration": {
             "access_level": "Undocumented",
-            "action": "GetResourceEventConfiguration",
+            "action": "PutPositionConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDestination": {
+        "UpdateFuotaTask": {
             "access_level": "Undocumented",
-            "action": "CreateDestination",
+            "action": "UpdateFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDestination": {
+        "DeleteFuotaTask": {
             "access_level": "Undocumented",
-            "action": "DeleteDestination",
+            "action": "DeleteFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartNetworkAnalyzerStream": {
+        "DeregisterWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "StartNetworkAnalyzerStream",
+            "action": "DeregisterWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMulticastGroupsByFuotaTask": {
+        "AssociateAwsAccountWithPartnerAccount": {
             "access_level": "Undocumented",
-            "action": "ListMulticastGroupsByFuotaTask",
+            "action": "AssociateAwsAccountWithPartnerAccount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessDeviceStatistics": {
+        "GetMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "GetWirelessDeviceStatistics",
+            "action": "GetMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateMulticastGroup": {
+        "ListPartnerAccounts": {
             "access_level": "Undocumented",
-            "action": "CreateMulticastGroup",
+            "action": "ListPartnerAccounts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateAwsAccountFromPartnerAccount": {
+        "AssociateWirelessDeviceWithThing": {
             "access_level": "Undocumented",
-            "action": "DisassociateAwsAccountFromPartnerAccount",
+            "action": "AssociateWirelessDeviceWithThing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateNetworkAnalyzerConfiguration": {
+        "GetDeviceProfile": {
             "access_level": "Undocumented",
-            "action": "UpdateNetworkAnalyzerConfiguration",
+            "action": "GetDeviceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateWirelessDeviceFromFuotaTask": {
+        "CreateWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessDeviceFromFuotaTask",
+            "action": "CreateWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetNetworkAnalyzerConfiguration": {
+        "ListDeviceProfiles": {
             "access_level": "Undocumented",
-            "action": "GetNetworkAnalyzerConfiguration",
+            "action": "ListDeviceProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessDevice": {
+        "ListWirelessDevices": {
             "access_level": "Undocumented",
-            "action": "GetWirelessDevice",
+            "action": "ListWirelessDevices",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TestWirelessDevice": {
+        "GetServiceProfile": {
             "access_level": "Undocumented",
-            "action": "TestWirelessDevice",
+            "action": "GetServiceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDestination": {
+        "UpdateWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "GetDestination",
+            "action": "UpdateWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateServiceProfile": {
+        "AssociateWirelessDeviceWithFuotaTask": {
             "access_level": "Undocumented",
-            "action": "CreateServiceProfile",
+            "action": "AssociateWirelessDeviceWithFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDestinations": {
+        "GetResourcePosition": {
             "access_level": "Undocumented",
-            "action": "ListDestinations",
+            "action": "GetResourcePosition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePosition": {
+        "UpdatePartnerAccount": {
             "access_level": "Undocumented",
-            "action": "UpdatePosition",
+            "action": "UpdatePartnerAccount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartBulkAssociateWirelessDeviceWithMulticastGroup": {
+        "DisassociateAwsAccountFromPartnerAccount": {
             "access_level": "Undocumented",
-            "action": "StartBulkAssociateWirelessDeviceWithMulticastGroup",
+            "action": "DisassociateAwsAccountFromPartnerAccount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPositionEstimate": {
+        "GetWirelessDeviceStatistics": {
             "access_level": "Undocumented",
-            "action": "GetPositionEstimate",
+            "action": "GetWirelessDeviceStatistics",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessDeviceWithFuotaTask": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessDeviceWithFuotaTask",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMulticastGroup": {
+        "GetResourceEventConfiguration": {
             "access_level": "Undocumented",
-            "action": "GetMulticastGroup",
+            "action": "GetResourceEventConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SendDataToWirelessDevice": {
+        "CreateWirelessGatewayTask": {
             "access_level": "Undocumented",
-            "action": "SendDataToWirelessDevice",
+            "action": "CreateWirelessGatewayTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGatewayCertificate": {
+        "UpdateResourcePosition": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGatewayCertificate",
+            "action": "UpdateResourcePosition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWirelessDeviceImportTask": {
+        "DeleteMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessDeviceImportTask",
+            "action": "DeleteMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFuotaTask": {
+        "GetWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "GetFuotaTask",
+            "action": "GetWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPositionConfiguration": {
+        "SendDataToWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "GetPositionConfiguration",
+            "action": "SendDataToWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWirelessGatewayTaskDefinition": {
+        "UpdateEventConfigurationByResourceTypes": {
             "access_level": "Undocumented",
-            "action": "CreateWirelessGatewayTaskDefinition",
+            "action": "UpdateEventConfigurationByResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateWirelessDeviceFromMulticastGroup": {
+        "UpdatePosition": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessDeviceFromMulticastGroup",
+            "action": "UpdatePosition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteMulticastGroup": {
+        "DisassociateMulticastGroupFromFuotaTask": {
             "access_level": "Undocumented",
-            "action": "DeleteMulticastGroup",
+            "action": "DisassociateMulticastGroupFromFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateWirelessDevice": {
+        "CreateFuotaTask": {
             "access_level": "Undocumented",
-            "action": "UpdateWirelessDevice",
+            "action": "CreateFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteQueuedMessages": {
+        "ListMulticastGroupsByFuotaTask": {
             "access_level": "Undocumented",
-            "action": "DeleteQueuedMessages",
+            "action": "ListMulticastGroupsByFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateWirelessDeviceFromThing": {
+        "GetMulticastGroupSession": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessDeviceFromThing",
+            "action": "GetMulticastGroupSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessGatewayWithCertificate": {
+        "ListNetworkAnalyzerConfigurations": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessGatewayWithCertificate",
+            "action": "ListNetworkAnalyzerConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFuotaTasks": {
+        "GetNetworkAnalyzerConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListFuotaTasks",
+            "action": "GetNetworkAnalyzerConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartSingleWirelessDeviceImportTask": {
+        "ListQueuedMessages": {
             "access_level": "Undocumented",
-            "action": "StartSingleWirelessDeviceImportTask",
+            "action": "ListQueuedMessages",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWirelessGatewayTask": {
+        "GetServiceEndpoint": {
             "access_level": "Undocumented",
-            "action": "CreateWirelessGatewayTask",
+            "action": "GetServiceEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateWirelessDeviceImportTask": {
+        "GetWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "UpdateWirelessDeviceImportTask",
+            "action": "GetWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessDeviceWithMulticastGroup": {
+        "GetPosition": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessDeviceWithMulticastGroup",
+            "action": "GetPosition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutPositionConfiguration": {
+        "DeleteWirelessGateway": {
             "access_level": "Undocumented",
-            "action": "PutPositionConfiguration",
+            "action": "DeleteWirelessGateway",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateNetworkAnalyzerConfiguration": {
+        "DeleteQueuedMessages": {
             "access_level": "Undocumented",
-            "action": "CreateNetworkAnalyzerConfiguration",
+            "action": "DeleteQueuedMessages",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteNetworkAnalyzerConfiguration": {
+        "ListDevicesForWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "DeleteNetworkAnalyzerConfiguration",
+            "action": "ListDevicesForWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPartnerAccount": {
+        "StartSingleWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "GetPartnerAccount",
+            "action": "StartSingleWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPartnerAccounts": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "ListPartnerAccounts",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWirelessGatewayTaskDefinition": {
+        "UpdateWirelessGateway": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessGatewayTaskDefinition",
+            "action": "UpdateWirelessGateway",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWirelessDevice": {
+        "DisassociateWirelessGatewayFromCertificate": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessDevice",
+            "action": "DisassociateWirelessGatewayFromCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGatewayTaskDefinition": {
+        "GetPositionConfiguration": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGatewayTaskDefinition",
+            "action": "GetPositionConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateFuotaTask": {
+        "CreateMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "CreateFuotaTask",
+            "action": "CreateMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWirelessGateway": {
+        "DisassociateWirelessDeviceFromThing": {
             "access_level": "Undocumented",
-            "action": "CreateWirelessGateway",
+            "action": "DisassociateWirelessDeviceFromThing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "GetLogLevelsByResourceTypes": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "GetLogLevelsByResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SendDataToMulticastGroup": {
+        "UpdateMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "SendDataToMulticastGroup",
+            "action": "UpdateMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEventConfigurationByResourceTypes": {
+        "GetWirelessGatewayTaskDefinition": {
             "access_level": "Undocumented",
-            "action": "GetEventConfigurationByResourceTypes",
+            "action": "GetWirelessGatewayTaskDefinition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMulticastGroupSession": {
+        "UpdateResourceEventConfiguration": {
             "access_level": "Undocumented",
-            "action": "GetMulticastGroupSession",
+            "action": "UpdateResourceEventConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListServiceProfiles": {
+        "UpdateNetworkAnalyzerConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListServiceProfiles",
+            "action": "UpdateNetworkAnalyzerConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateFuotaTask": {
+        "ListWirelessGatewayTaskDefinitions": {
             "access_level": "Undocumented",
-            "action": "UpdateFuotaTask",
+            "action": "ListWirelessGatewayTaskDefinitions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartBulkDisassociateWirelessDeviceFromMulticastGroup": {
+        "CreateServiceProfile": {
             "access_level": "Undocumented",
-            "action": "StartBulkDisassociateWirelessDeviceFromMulticastGroup",
+            "action": "CreateServiceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelMulticastGroupSession": {
+        "ListEventConfigurations": {
             "access_level": "Undocumented",
-            "action": "CancelMulticastGroupSession",
+            "action": "ListEventConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePartnerAccount": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "UpdatePartnerAccount",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWirelessDevice": {
+        "UpdateDestination": {
             "access_level": "Undocumented",
-            "action": "CreateWirelessDevice",
+            "action": "UpdateDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateEventConfigurationByResourceTypes": {
+        "AssociateMulticastGroupWithFuotaTask": {
             "access_level": "Undocumented",
-            "action": "UpdateEventConfigurationByResourceTypes",
+            "action": "AssociateMulticastGroupWithFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGatewayStatistics": {
+        "StartWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGatewayStatistics",
+            "action": "StartWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDevicesForWirelessDeviceImportTask": {
+        "CreateWirelessGateway": {
             "access_level": "Undocumented",
-            "action": "ListDevicesForWirelessDeviceImportTask",
+            "action": "CreateWirelessGateway",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDeviceProfile": {
+        "StartMulticastGroupSession": {
             "access_level": "Undocumented",
-            "action": "DeleteDeviceProfile",
+            "action": "StartMulticastGroupSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateMulticastGroupFromFuotaTask": {
+        "GetFuotaTask": {
             "access_level": "Undocumented",
-            "action": "DisassociateMulticastGroupFromFuotaTask",
+            "action": "GetFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceProfile": {
+        "ListWirelessDeviceImportTasks": {
             "access_level": "Undocumented",
-            "action": "GetServiceProfile",
+            "action": "ListWirelessDeviceImportTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateMulticastGroupWithFuotaTask": {
+        "AssociateWirelessDeviceWithMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "AssociateMulticastGroupWithFuotaTask",
+            "action": "AssociateWirelessDeviceWithMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEventConfigurations": {
+        "AssociateWirelessGatewayWithCertificate": {
             "access_level": "Undocumented",
-            "action": "ListEventConfigurations",
+            "action": "AssociateWirelessGatewayWithCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGateway": {
+        "PutResourceLogLevel": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGateway",
+            "action": "PutResourceLogLevel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateWirelessGatewayFromCertificate": {
+        "DeleteWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessGatewayFromCertificate",
+            "action": "DeleteWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ResetAllResourceLogLevels": {
+        "AssociateWirelessGatewayWithThing": {
             "access_level": "Undocumented",
-            "action": "ResetAllResourceLogLevels",
+            "action": "AssociateWirelessGatewayWithThing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessDeviceWithThing": {
+        "DisassociateWirelessDeviceFromMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessDeviceWithThing",
+            "action": "DisassociateWirelessDeviceFromMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGatewayFirmwareInformation": {
+        "GetPartnerAccount": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGatewayFirmwareInformation",
+            "action": "GetPartnerAccount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateResourceEventConfiguration": {
+        "UpdateWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "UpdateResourceEventConfiguration",
+            "action": "UpdateWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListQueuedMessages": {
+        "ListFuotaTasks": {
             "access_level": "Undocumented",
-            "action": "ListQueuedMessages",
+            "action": "ListFuotaTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartFuotaTask": {
+        "DeleteServiceProfile": {
             "access_level": "Undocumented",
-            "action": "StartFuotaTask",
+            "action": "DeleteServiceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWirelessGateways": {
+        "GetWirelessGatewayFirmwareInformation": {
             "access_level": "Undocumented",
-            "action": "ListWirelessGateways",
+            "action": "GetWirelessGatewayFirmwareInformation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateAwsAccountWithPartnerAccount": {
+        "CreateWirelessGatewayTaskDefinition": {
             "access_level": "Undocumented",
-            "action": "AssociateAwsAccountWithPartnerAccount",
+            "action": "CreateWirelessGatewayTaskDefinition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateLogLevelsByResourceTypes": {
+        "SendDataToMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "UpdateLogLevelsByResourceTypes",
+            "action": "SendDataToMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "StartNetworkAnalyzerStream": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "StartNetworkAnalyzerStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourcePosition": {
+        "GetDestination": {
             "access_level": "Undocumented",
-            "action": "GetResourcePosition",
+            "action": "GetDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateMulticastGroup": {
+        "ResetAllResourceLogLevels": {
             "access_level": "Undocumented",
-            "action": "UpdateMulticastGroup",
+            "action": "ResetAllResourceLogLevels",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ResetResourceLogLevel": {
+        "DeleteNetworkAnalyzerConfiguration": {
             "access_level": "Undocumented",
-            "action": "ResetResourceLogLevel",
+            "action": "DeleteNetworkAnalyzerConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWirelessGateway": {
+        "StartBulkAssociateWirelessDeviceWithMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessGateway",
+            "action": "StartBulkAssociateWirelessDeviceWithMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceEndpoint": {
+        "CancelMulticastGroupSession": {
             "access_level": "Undocumented",
-            "action": "GetServiceEndpoint",
+            "action": "CancelMulticastGroupSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListNetworkAnalyzerConfigurations": {
+        "GetWirelessGatewayTask": {
             "access_level": "Undocumented",
-            "action": "ListNetworkAnalyzerConfigurations",
+            "action": "GetWirelessGatewayTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartMulticastGroupSession": {
+        "DeleteDestination": {
             "access_level": "Undocumented",
-            "action": "StartMulticastGroupSession",
+            "action": "DeleteDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDeviceProfiles": {
+        "CreateDestination": {
             "access_level": "Undocumented",
-            "action": "ListDeviceProfiles",
+            "action": "CreateDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateWirelessGateway": {
+        "DeleteWirelessGatewayTask": {
             "access_level": "Undocumented",
-            "action": "UpdateWirelessGateway",
+            "action": "DeleteWirelessGatewayTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDeviceProfile": {
+        "ListWirelessGateways": {
             "access_level": "Undocumented",
-            "action": "CreateDeviceProfile",
+            "action": "ListWirelessGateways",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMulticastGroups": {
+        "CreateDeviceProfile": {
             "access_level": "Undocumented",
-            "action": "ListMulticastGroups",
+            "action": "CreateDeviceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessDeviceImportTask": {
+        "TestWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "GetWirelessDeviceImportTask",
+            "action": "TestWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGatewayTask": {
+        "GetResourceLogLevel": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGatewayTask",
+            "action": "GetResourceLogLevel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartWirelessDeviceImportTask": {
+        "ListServiceProfiles": {
             "access_level": "Undocumented",
-            "action": "StartWirelessDeviceImportTask",
+            "action": "ListServiceProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteServiceProfile": {
+        "ListDestinations": {
             "access_level": "Undocumented",
-            "action": "DeleteServiceProfile",
+            "action": "ListDestinations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "iq": {
@@ -82486,315 +82486,315 @@
             "resources": [
                 "index",
                 "thesaurus"
             ]
         }
     },
     "kendra-ranking": {
-        "ListRescoreExecutionPlans": {
+        "CreateRescoreExecutionPlan": {
             "access_level": "Undocumented",
-            "action": "ListRescoreExecutionPlans",
+            "action": "CreateRescoreExecutionPlan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeRescoreExecutionPlan": {
+        "ListRescoreExecutionPlans": {
             "access_level": "Undocumented",
-            "action": "DescribeRescoreExecutionPlan",
+            "action": "ListRescoreExecutionPlans",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateRescoreExecutionPlan": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "CreateRescoreExecutionPlan",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "Rescore": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "Rescore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "Rescore": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "Rescore",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeleteRescoreExecutionPlan": {
             "access_level": "Undocumented",
             "action": "DeleteRescoreExecutionPlan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "UpdateRescoreExecutionPlan": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "UpdateRescoreExecutionPlan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateRescoreExecutionPlan": {
+        "DescribeRescoreExecutionPlan": {
             "access_level": "Undocumented",
-            "action": "UpdateRescoreExecutionPlan",
+            "action": "DescribeRescoreExecutionPlan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "kinesis": {
-        "DescribeStream": {
+        "StartStreamEncryption": {
             "access_level": "Undocumented",
-            "action": "DescribeStream",
+            "action": "StartStreamEncryption",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeStreamConsumer": {
+        "AddTagsToStream": {
             "access_level": "Undocumented",
-            "action": "DescribeStreamConsumer",
+            "action": "AddTagsToStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "IncreaseStreamRetentionPeriod": {
+        "ListStreamConsumers": {
             "access_level": "Undocumented",
-            "action": "IncreaseStreamRetentionPeriod",
+            "action": "ListStreamConsumers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListShards": {
+        "StopStreamEncryption": {
             "access_level": "Undocumented",
-            "action": "ListShards",
+            "action": "StopStreamEncryption",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "RegisterStreamConsumer": {
             "access_level": "Undocumented",
             "action": "RegisterStreamConsumer",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopStreamEncryption": {
+        "SplitShard": {
             "access_level": "Undocumented",
-            "action": "StopStreamEncryption",
+            "action": "SplitShard",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRecords": {
+        "DescribeStream": {
             "access_level": "Undocumented",
-            "action": "GetRecords",
+            "action": "DescribeStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeregisterStreamConsumer": {
+        "GetRecords": {
             "access_level": "Undocumented",
-            "action": "DeregisterStreamConsumer",
+            "action": "GetRecords",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SubscribeToShard": {
+        "UpdateStreamMode": {
             "access_level": "Undocumented",
-            "action": "SubscribeToShard",
+            "action": "UpdateStreamMode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListStreamConsumers": {
+        "ListShards": {
             "access_level": "Undocumented",
-            "action": "ListStreamConsumers",
+            "action": "ListShards",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddTagsToStream": {
+        "IncreaseStreamRetentionPeriod": {
             "access_level": "Undocumented",
-            "action": "AddTagsToStream",
+            "action": "IncreaseStreamRetentionPeriod",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateShardCount": {
+        "GetShardIterator": {
             "access_level": "Undocumented",
-            "action": "UpdateShardCount",
+            "action": "GetShardIterator",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetShardIterator": {
+        "DescribeStreamConsumer": {
             "access_level": "Undocumented",
-            "action": "GetShardIterator",
+            "action": "DescribeStreamConsumer",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveTagsFromStream": {
+        "DecreaseStreamRetentionPeriod": {
             "access_level": "Undocumented",
-            "action": "RemoveTagsFromStream",
+            "action": "DecreaseStreamRetentionPeriod",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForStream": {
+        "EnableEnhancedMonitoring": {
             "access_level": "Undocumented",
-            "action": "ListTagsForStream",
+            "action": "EnableEnhancedMonitoring",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutRecords": {
+        "MergeShards": {
             "access_level": "Undocumented",
-            "action": "PutRecords",
+            "action": "MergeShards",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutRecord": {
+        "SubscribeToShard": {
             "access_level": "Undocumented",
-            "action": "PutRecord",
+            "action": "SubscribeToShard",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeStreamSummary": {
+        "DeleteStream": {
             "access_level": "Undocumented",
-            "action": "DescribeStreamSummary",
+            "action": "DeleteStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListStreams": {
             "access_level": "Undocumented",
             "action": "ListStreams",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisableEnhancedMonitoring": {
+        "ListTagsForStream": {
             "access_level": "Undocumented",
-            "action": "DisableEnhancedMonitoring",
+            "action": "ListTagsForStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "MergeShards": {
+        "PutRecords": {
             "access_level": "Undocumented",
-            "action": "MergeShards",
+            "action": "PutRecords",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateStreamMode": {
+        "DescribeStreamSummary": {
             "access_level": "Undocumented",
-            "action": "UpdateStreamMode",
+            "action": "DescribeStreamSummary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateStream": {
+        "DisableEnhancedMonitoring": {
             "access_level": "Undocumented",
-            "action": "CreateStream",
+            "action": "DisableEnhancedMonitoring",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DecreaseStreamRetentionPeriod": {
+        "UpdateShardCount": {
             "access_level": "Undocumented",
-            "action": "DecreaseStreamRetentionPeriod",
+            "action": "UpdateShardCount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteStream": {
+        "PutRecord": {
             "access_level": "Undocumented",
-            "action": "DeleteStream",
+            "action": "PutRecord",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeLimits": {
+        "RemoveTagsFromStream": {
             "access_level": "Undocumented",
-            "action": "DescribeLimits",
+            "action": "RemoveTagsFromStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "EnableEnhancedMonitoring": {
+        "CreateStream": {
             "access_level": "Undocumented",
-            "action": "EnableEnhancedMonitoring",
+            "action": "CreateStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartStreamEncryption": {
+        "DeregisterStreamConsumer": {
             "access_level": "Undocumented",
-            "action": "StartStreamEncryption",
+            "action": "DeregisterStreamConsumer",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SplitShard": {
+        "DescribeLimits": {
             "access_level": "Undocumented",
-            "action": "SplitShard",
+            "action": "DescribeLimits",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "kinesisanalytics": {
@@ -85361,73 +85361,73 @@
             "orphan": false,
             "resources": [
                 "function"
             ]
         }
     },
     "launchwizard": {
-        "GetResourceCostEstimate": {
+        "DescribeProvisionedApp": {
             "access_level": "Undocumented",
-            "action": "GetResourceCostEstimate",
+            "action": "DescribeProvisionedApp",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartProvisioning": {
+        "GetResourceCostEstimate": {
             "access_level": "Undocumented",
-            "action": "StartProvisioning",
+            "action": "GetResourceCostEstimate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProvisionedApps": {
+        "StartProvisioning": {
             "access_level": "Undocumented",
-            "action": "ListProvisionedApps",
+            "action": "StartProvisioning",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeProvisionedApp": {
+        "DeleteApp": {
             "access_level": "Undocumented",
-            "action": "DescribeProvisionedApp",
+            "action": "DeleteApp",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeProvisioningEvents": {
+        "GetInfrastructureSuggestion": {
             "access_level": "Undocumented",
-            "action": "DescribeProvisioningEvents",
+            "action": "GetInfrastructureSuggestion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteApp": {
+        "ListProvisionedApps": {
             "access_level": "Undocumented",
-            "action": "DeleteApp",
+            "action": "ListProvisionedApps",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetIpAddress": {
             "access_level": "Undocumented",
             "action": "GetIpAddress",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetInfrastructureSuggestion": {
+        "DescribeProvisioningEvents": {
             "access_level": "Undocumented",
-            "action": "GetInfrastructureSuggestion",
+            "action": "DescribeProvisioningEvents",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "lex": {
@@ -100885,251 +100885,251 @@
             "orphan": false,
             "resources": [
                 "studio-component"
             ]
         }
     },
     "notifications": {
-        "UpdateEventRule": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "UpdateEventRule",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEventRule": {
+        "ListChannels": {
             "access_level": "Undocumented",
-            "action": "GetEventRule",
+            "action": "ListChannels",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RegisterNotificationHub": {
+        "DisassociateChannel": {
             "access_level": "Undocumented",
-            "action": "RegisterNotificationHub",
+            "action": "DisassociateChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEventRules": {
+        "UpdateNotificationConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListEventRules",
+            "action": "UpdateNotificationConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateNotificationConfiguration": {
+        "AssociateChannel": {
             "access_level": "Undocumented",
-            "action": "CreateNotificationConfiguration",
+            "action": "AssociateChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListNotificationConfigurations": {
+        "DeregisterNotificationHub": {
             "access_level": "Undocumented",
-            "action": "ListNotificationConfigurations",
+            "action": "DeregisterNotificationHub",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "GetNotificationEvent": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "GetNotificationEvent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateChannel": {
+        "RegisterNotificationHub": {
             "access_level": "Undocumented",
-            "action": "DisassociateChannel",
+            "action": "RegisterNotificationHub",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListChannels": {
+        "DeleteEventRule": {
             "access_level": "Undocumented",
-            "action": "ListChannels",
+            "action": "DeleteEventRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListEventRules": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListEventRules",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetNotificationConfiguration": {
+        "ListNotificationHubs": {
             "access_level": "Undocumented",
-            "action": "GetNotificationConfiguration",
+            "action": "ListNotificationHubs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListNotificationEvents": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ListNotificationEvents",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListNotificationHubs": {
+        "GetEventRule": {
             "access_level": "Undocumented",
-            "action": "ListNotificationHubs",
+            "action": "GetEventRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetNotificationEvent": {
+        "DeleteNotificationConfiguration": {
             "access_level": "Undocumented",
-            "action": "GetNotificationEvent",
+            "action": "DeleteNotificationConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteNotificationConfiguration": {
+        "UpdateEventRule": {
             "access_level": "Undocumented",
-            "action": "DeleteNotificationConfiguration",
+            "action": "UpdateEventRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateNotificationConfiguration": {
+        "GetNotificationConfiguration": {
             "access_level": "Undocumented",
-            "action": "UpdateNotificationConfiguration",
+            "action": "GetNotificationConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateChannel": {
+        "ListNotificationConfigurations": {
             "access_level": "Undocumented",
-            "action": "AssociateChannel",
+            "action": "ListNotificationConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteEventRule": {
+        "CreateNotificationConfiguration": {
             "access_level": "Undocumented",
-            "action": "DeleteEventRule",
+            "action": "CreateNotificationConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateEventRule": {
             "access_level": "Undocumented",
             "action": "CreateEventRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeregisterNotificationHub": {
+        "ListNotificationEvents": {
             "access_level": "Undocumented",
-            "action": "DeregisterNotificationHub",
+            "action": "ListNotificationEvents",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "notifications-contacts": {
-        "GetEmailContact": {
+        "DeleteEmailContact": {
             "access_level": "Undocumented",
-            "action": "GetEmailContact",
+            "action": "DeleteEmailContact",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListEmailContacts": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListEmailContacts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SendActivationCode": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "SendActivationCode",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ActivateEmailContact": {
+        "SendActivationCode": {
             "access_level": "Undocumented",
-            "action": "ActivateEmailContact",
+            "action": "SendActivationCode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateEmailContact": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "CreateEmailContact",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "CreateEmailContact": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "CreateEmailContact",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEmailContacts": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListEmailContacts",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "GetEmailContact": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "GetEmailContact",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteEmailContact": {
+        "ActivateEmailContact": {
             "access_level": "Undocumented",
-            "action": "DeleteEmailContact",
+            "action": "ActivateEmailContact",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "oam": {
@@ -104040,65 +104040,65 @@
             "orphan": false,
             "resources": [
                 "device"
             ]
         }
     },
     "payments": {
-        "ListPaymentPreferences": {
+        "GetPaymentStatus": {
             "access_level": "Undocumented",
-            "action": "ListPaymentPreferences",
+            "action": "GetPaymentStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePaymentInstrument": {
+        "ListPaymentPreferences": {
             "access_level": "Undocumented",
-            "action": "CreatePaymentInstrument",
+            "action": "ListPaymentPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePaymentInstrument": {
+        "CreatePaymentInstrument": {
             "access_level": "Undocumented",
-            "action": "DeletePaymentInstrument",
+            "action": "CreatePaymentInstrument",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPaymentStatus": {
+        "MakePayment": {
             "access_level": "Undocumented",
-            "action": "GetPaymentStatus",
+            "action": "MakePayment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPaymentInstrument": {
+        "DeletePaymentInstrument": {
             "access_level": "Undocumented",
-            "action": "GetPaymentInstrument",
+            "action": "DeletePaymentInstrument",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "MakePayment": {
+        "UpdatePaymentPreferences": {
             "access_level": "Undocumented",
-            "action": "MakePayment",
+            "action": "UpdatePaymentPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePaymentPreferences": {
+        "GetPaymentInstrument": {
             "access_level": "Undocumented",
-            "action": "UpdatePaymentPreferences",
+            "action": "GetPaymentInstrument",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "personalize": {
@@ -109028,281 +109028,281 @@
             "orphan": false,
             "resources": [
                 "user"
             ]
         }
     },
     "ram": {
-        "PromotePermissionCreatedFromPolicy": {
+        "CreatePermissionVersion": {
             "access_level": "Undocumented",
-            "action": "PromotePermissionCreatedFromPolicy",
+            "action": "CreatePermissionVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateResourceShare": {
+        "CreatePermission": {
             "access_level": "Undocumented",
-            "action": "AssociateResourceShare",
+            "action": "CreatePermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListReplacePermissionAssociationsWork": {
+        "DisassociateResourceShare": {
             "access_level": "Undocumented",
-            "action": "ListReplacePermissionAssociationsWork",
+            "action": "DisassociateResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListResourceTypes": {
+        "ListPermissionVersions": {
             "access_level": "Undocumented",
-            "action": "ListResourceTypes",
+            "action": "ListPermissionVersions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteResourceShare": {
+        "ListResourceTypes": {
             "access_level": "Undocumented",
-            "action": "DeleteResourceShare",
+            "action": "ListResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePermissionVersion": {
+        "ListResources": {
             "access_level": "Undocumented",
-            "action": "DeletePermissionVersion",
+            "action": "ListResources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PromoteResourceShareCreatedFromPolicy": {
+        "ListPrincipals": {
             "access_level": "Undocumented",
-            "action": "PromoteResourceShareCreatedFromPolicy",
+            "action": "ListPrincipals",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AcceptResourceShareInvitation": {
+        "RejectResourceShareInvitation": {
             "access_level": "Undocumented",
-            "action": "AcceptResourceShareInvitation",
+            "action": "RejectResourceShareInvitation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPermission": {
+        "UpdateResourceShare": {
             "access_level": "Undocumented",
-            "action": "GetPermission",
+            "action": "UpdateResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "EnableSharingWithAwsOrganization": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "EnableSharingWithAwsOrganization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "EnableSharingWithAwsOrganization": {
+        "GetResourcePolicies": {
             "access_level": "Undocumented",
-            "action": "EnableSharingWithAwsOrganization",
+            "action": "GetResourcePolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPermissions": {
+        "AcceptResourceShareInvitation": {
             "access_level": "Undocumented",
-            "action": "ListPermissions",
+            "action": "AcceptResourceShareInvitation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListResources": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ListResources",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPrincipals": {
+        "ListPendingInvitationResources": {
             "access_level": "Undocumented",
-            "action": "ListPrincipals",
+            "action": "ListPendingInvitationResources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateResourceShare": {
+        "ListPermissionAssociations": {
             "access_level": "Undocumented",
-            "action": "DisassociateResourceShare",
+            "action": "ListPermissionAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPermissionAssociations": {
+        "ListReplacePermissionAssociationsWork": {
             "access_level": "Undocumented",
-            "action": "ListPermissionAssociations",
+            "action": "ListReplacePermissionAssociationsWork",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RejectResourceShareInvitation": {
+        "DisassociateResourceSharePermission": {
             "access_level": "Undocumented",
-            "action": "RejectResourceShareInvitation",
+            "action": "DisassociateResourceSharePermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceShares": {
+        "GetResourceShareInvitations": {
             "access_level": "Undocumented",
-            "action": "GetResourceShares",
+            "action": "GetResourceShareInvitations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateResourceShare": {
+        "PromoteResourceShareCreatedFromPolicy": {
             "access_level": "Undocumented",
-            "action": "UpdateResourceShare",
+            "action": "PromoteResourceShareCreatedFromPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetDefaultPermissionVersion": {
+        "GetPermission": {
             "access_level": "Undocumented",
-            "action": "SetDefaultPermissionVersion",
+            "action": "GetPermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateResourceShare": {
+        "ReplacePermissionAssociations": {
             "access_level": "Undocumented",
-            "action": "CreateResourceShare",
+            "action": "ReplacePermissionAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPermissionVersions": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListPermissionVersions",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ReplacePermissionAssociations": {
+        "AssociateResourceSharePermission": {
             "access_level": "Undocumented",
-            "action": "ReplacePermissionAssociations",
+            "action": "AssociateResourceSharePermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListResourceSharePermissions": {
+        "DeleteResourceShare": {
             "access_level": "Undocumented",
-            "action": "ListResourceSharePermissions",
+            "action": "DeleteResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePermissionVersion": {
+        "PromotePermissionCreatedFromPolicy": {
             "access_level": "Undocumented",
-            "action": "CreatePermissionVersion",
+            "action": "PromotePermissionCreatedFromPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "DeletePermissionVersion": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "DeletePermissionVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourcePolicies": {
+        "AssociateResourceShare": {
             "access_level": "Undocumented",
-            "action": "GetResourcePolicies",
+            "action": "AssociateResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceShareAssociations": {
+        "GetResourceShares": {
             "access_level": "Undocumented",
-            "action": "GetResourceShareAssociations",
+            "action": "GetResourceShares",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateResourceSharePermission": {
+        "ListPermissions": {
             "access_level": "Undocumented",
-            "action": "AssociateResourceSharePermission",
+            "action": "ListPermissions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePermission": {
+        "GetResourceShareAssociations": {
             "access_level": "Undocumented",
-            "action": "CreatePermission",
+            "action": "GetResourceShareAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceShareInvitations": {
+        "SetDefaultPermissionVersion": {
             "access_level": "Undocumented",
-            "action": "GetResourceShareInvitations",
+            "action": "SetDefaultPermissionVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPendingInvitationResources": {
+        "ListResourceSharePermissions": {
             "access_level": "Undocumented",
-            "action": "ListPendingInvitationResources",
+            "action": "ListResourceSharePermissions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePermission": {
+        "CreateResourceShare": {
             "access_level": "Undocumented",
-            "action": "DeletePermission",
+            "action": "CreateResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateResourceSharePermission": {
+        "DeletePermission": {
             "access_level": "Undocumented",
-            "action": "DisassociateResourceSharePermission",
+            "action": "DeletePermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "rbin": {
@@ -126752,113 +126752,113 @@
             "orphan": false,
             "resources": [
                 "schema"
             ]
         }
     },
     "scn": {
-        "CreateInstance": {
+        "AssignAdminPermissionsToUser": {
             "access_level": "Undocumented",
-            "action": "CreateInstance",
+            "action": "AssignAdminPermissionsToUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSSOApplication": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "CreateSSOApplication",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSSOApplication": {
+        "CreateInstance": {
             "access_level": "Undocumented",
-            "action": "DeleteSSOApplication",
+            "action": "CreateInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListAdminUsers": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListAdminUsers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssignAdminPermissionsToUser": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "AssignAdminPermissionsToUser",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteInstance": {
+        "DeleteSSOApplication": {
             "access_level": "Undocumented",
-            "action": "DeleteInstance",
+            "action": "DeleteSSOApplication",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveAdminPermissionsForUser": {
+        "DescribeInstance": {
             "access_level": "Undocumented",
-            "action": "RemoveAdminPermissionsForUser",
+            "action": "DescribeInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateInstance": {
+        "DeleteInstance": {
             "access_level": "Undocumented",
-            "action": "UpdateInstance",
+            "action": "DeleteInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListInstances": {
+        "RemoveAdminPermissionsForUser": {
             "access_level": "Undocumented",
-            "action": "ListInstances",
+            "action": "RemoveAdminPermissionsForUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeInstance": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "DescribeInstance",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "CreateSSOApplication": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "CreateSSOApplication",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListInstances": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListInstances",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAdminUsers": {
+        "UpdateInstance": {
             "access_level": "Undocumented",
-            "action": "ListAdminUsers",
+            "action": "UpdateInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "sdb": {
@@ -141568,273 +141568,273 @@
             "condition_keys": [],
             "description": "Grants permission to list accounts that might be useful in a new query",
             "orphan": false,
             "resources": []
         }
     },
     "tnb": {
-        "UpdateSolFunctionPackage": {
+        "GetSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "UpdateSolFunctionPackage",
+            "action": "GetSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolNetworkInstance": {
+        "CreateSolFunctionPackage": {
             "access_level": "Undocumented",
-            "action": "GetSolNetworkInstance",
+            "action": "CreateSolFunctionPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutSolFunctionPackageContent": {
+        "CreateSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "PutSolFunctionPackageContent",
+            "action": "CreateSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolNetworkPackage": {
+        "InstantiateSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "GetSolNetworkPackage",
+            "action": "InstantiateSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolNetworkPackageContent": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "GetSolNetworkPackageContent",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSolFunctionPackages": {
+        "GetSolFunctionPackageContent": {
             "access_level": "Undocumented",
-            "action": "ListSolFunctionPackages",
+            "action": "GetSolFunctionPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "CreateSolNetworkPackage": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "CreateSolNetworkPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolNetworkOperation": {
+        "GetSolNetworkPackageContent": {
             "access_level": "Undocumented",
-            "action": "GetSolNetworkOperation",
+            "action": "GetSolNetworkPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSolNetworkPackage": {
+        "UpdateSolFunctionPackage": {
             "access_level": "Undocumented",
-            "action": "UpdateSolNetworkPackage",
+            "action": "UpdateSolFunctionPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "GetSolNetworkPackage": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "GetSolNetworkPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSolNetworkOperations": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ListSolNetworkOperations",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolFunctionPackageDescriptor": {
+        "UpdateSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "GetSolFunctionPackageDescriptor",
+            "action": "UpdateSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSolFunctionPackage": {
+        "DeleteSolFunctionPackage": {
             "access_level": "Undocumented",
-            "action": "CreateSolFunctionPackage",
+            "action": "DeleteSolFunctionPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSolFunctionInstances": {
+        "DeleteSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "ListSolFunctionInstances",
+            "action": "DeleteSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolFunctionPackageContent": {
+        "GetSolNetworkPackageDescriptor": {
             "access_level": "Undocumented",
-            "action": "GetSolFunctionPackageContent",
+            "action": "GetSolNetworkPackageDescriptor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelSolNetworkOperation": {
+        "ListSolNetworkInstances": {
             "access_level": "Undocumented",
-            "action": "CancelSolNetworkOperation",
+            "action": "ListSolNetworkInstances",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "InstantiateSolNetworkInstance": {
+        "DeleteSolNetworkPackage": {
             "access_level": "Undocumented",
-            "action": "InstantiateSolNetworkInstance",
+            "action": "DeleteSolNetworkPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolFunctionPackage": {
+        "GetSolFunctionPackageDescriptor": {
             "access_level": "Undocumented",
-            "action": "GetSolFunctionPackage",
+            "action": "GetSolFunctionPackageDescriptor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSolNetworkInstances": {
+        "GetSolFunctionPackage": {
             "access_level": "Undocumented",
-            "action": "ListSolNetworkInstances",
+            "action": "GetSolFunctionPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TerminateSolNetworkInstance": {
+        "ListSolNetworkOperations": {
             "access_level": "Undocumented",
-            "action": "TerminateSolNetworkInstance",
+            "action": "ListSolNetworkOperations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutSolNetworkPackageContent": {
+        "ValidateSolNetworkPackageContent": {
             "access_level": "Undocumented",
-            "action": "PutSolNetworkPackageContent",
+            "action": "ValidateSolNetworkPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ValidateSolFunctionPackageContent": {
+        "ListSolNetworkPackages": {
             "access_level": "Undocumented",
-            "action": "ValidateSolFunctionPackageContent",
+            "action": "ListSolNetworkPackages",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ValidateSolNetworkPackageContent": {
+        "PutSolFunctionPackageContent": {
             "access_level": "Undocumented",
-            "action": "ValidateSolNetworkPackageContent",
+            "action": "PutSolFunctionPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSolNetworkPackage": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteSolNetworkPackage",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSolNetworkPackage": {
+        "UpdateSolNetworkPackage": {
             "access_level": "Undocumented",
-            "action": "CreateSolNetworkPackage",
+            "action": "UpdateSolNetworkPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "CancelSolNetworkOperation": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "CancelSolNetworkOperation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolNetworkPackageDescriptor": {
+        "GetSolNetworkOperation": {
             "access_level": "Undocumented",
-            "action": "GetSolNetworkPackageDescriptor",
+            "action": "GetSolNetworkOperation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSolNetworkInstance": {
+        "ValidateSolFunctionPackageContent": {
             "access_level": "Undocumented",
-            "action": "UpdateSolNetworkInstance",
+            "action": "ValidateSolFunctionPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSolNetworkInstance": {
+        "GetSolFunctionInstance": {
             "access_level": "Undocumented",
-            "action": "DeleteSolNetworkInstance",
+            "action": "GetSolFunctionInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolFunctionInstance": {
+        "ListSolFunctionPackages": {
             "access_level": "Undocumented",
-            "action": "GetSolFunctionInstance",
+            "action": "ListSolFunctionPackages",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSolFunctionPackage": {
+        "TerminateSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "DeleteSolFunctionPackage",
+            "action": "TerminateSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSolNetworkInstance": {
+        "ListSolFunctionInstances": {
             "access_level": "Undocumented",
-            "action": "CreateSolNetworkInstance",
+            "action": "ListSolFunctionInstances",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSolNetworkPackages": {
+        "PutSolNetworkPackageContent": {
             "access_level": "Undocumented",
-            "action": "ListSolNetworkPackages",
+            "action": "PutSolNetworkPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "transcribe": {
```

### Comparing `iam_actions-1.2.20230422/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230423/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230422/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230423/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230422/iam_actions/generate/generate.py` & `iam_actions-1.2.20230423/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230422/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230423/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230422/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230423/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230422/iam_actions/generate/services.py` & `iam_actions-1.2.20230423/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230422/iam_actions/policies.json` & `iam_actions-1.2.20230423/iam_actions/policies.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230422/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230423/iam_actions/resourcetypes.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230422/iam_actions/services.json` & `iam_actions-1.2.20230423/iam_actions/services.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230422/pyproject.toml` & `iam_actions-1.2.20230423/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230422"
+version = "1.2.20230423"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230422/setup.py` & `iam_actions-1.2.20230423/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230422',
+    'version': '1.2.20230423',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230422/PKG-INFO` & `iam_actions-1.2.20230423/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230422
+Version: 1.2.20230423
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

