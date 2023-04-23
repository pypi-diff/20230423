# Comparing `tmp/alchemiscale-0.1.1.tar.gz` & `tmp/alchemiscale-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alchemiscale-0.1.1.tar", last modified: Fri Apr 21 17:39:13 2023, max compression
+gzip compressed data, was "alchemiscale-0.1.2.tar", last modified: Sun Apr 23 04:25:24 2023, max compression
```

## Comparing `alchemiscale-0.1.1.tar` & `alchemiscale-0.1.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 david     (1001) david     (1001)        0 2023-04-21 17:39:13.510923 alchemiscale-0.1.1/
--rw-r--r--   0 david     (1001) david     (1001)     1084 2022-08-27 01:07:20.000000 alchemiscale-0.1.1/LICENSE
--rw-r--r--   0 david     (1001) david     (1001)       55 2023-02-07 08:08:11.000000 alchemiscale-0.1.1/MANIFEST.in
--rw-r--r--   0 david     (1001) david     (1001)     1195 2023-04-21 17:39:13.510923 alchemiscale-0.1.1/PKG-INFO
--rw-r--r--   0 david     (1001) david     (1001)      610 2023-03-17 00:52:31.000000 alchemiscale-0.1.1/README.md
-drwxr-xr-x   0 david     (1001) david     (1001)        0 2023-04-21 17:39:13.514256 alchemiscale-0.1.1/alchemiscale/
--rw-r--r--   0 david     (1001) david     (1001)      153 2023-02-07 08:08:11.000000 alchemiscale-0.1.1/alchemiscale/__init__.py
--rw-r--r--   0 david     (1001) david     (1001)      498 2023-04-21 17:39:13.514256 alchemiscale-0.1.1/alchemiscale/_version.py
-drwxr-xr-x   0 david     (1001) david     (1001)        0 2023-04-21 17:39:13.507589 alchemiscale-0.1.1/alchemiscale/base/
--rw-r--r--   0 david     (1001) david     (1001)        0 2023-04-21 17:35:54.000000 alchemiscale-0.1.1/alchemiscale/base/__init__.py
--rw-r--r--   0 david     (1001) david     (1001)     6804 2023-04-21 17:35:54.000000 alchemiscale-0.1.1/alchemiscale/base/api.py
--rw-r--r--   0 david     (1001) david     (1001)     8197 2023-04-21 17:35:54.000000 alchemiscale-0.1.1/alchemiscale/base/client.py
--rw-r--r--   0 david     (1001) david     (1001)    17195 2023-04-21 17:35:54.000000 alchemiscale-0.1.1/alchemiscale/cli.py
--rw-r--r--   0 david     (1001) david     (1001)      929 2023-04-21 17:35:54.000000 alchemiscale-0.1.1/alchemiscale/cli_utils.py
-drwxr-xr-x   0 david     (1001) david     (1001)        0 2023-04-21 17:39:13.510923 alchemiscale-0.1.1/alchemiscale/compute/
--rw-r--r--   0 david     (1001) david     (1001)       46 2023-02-07 08:08:11.000000 alchemiscale-0.1.1/alchemiscale/compute/__init__.py
--rw-r--r--   0 david     (1001) david     (1001)     7282 2023-04-21 17:35:58.000000 alchemiscale-0.1.1/alchemiscale/compute/api.py
--rw-r--r--   0 david     (1001) david     (1001)     3570 2023-04-21 17:35:58.000000 alchemiscale-0.1.1/alchemiscale/compute/client.py
--rw-r--r--   0 david     (1001) david     (1001)    16582 2023-04-21 17:35:58.000000 alchemiscale-0.1.1/alchemiscale/compute/service.py
-drwxr-xr-x   0 david     (1001) david     (1001)        0 2023-04-21 17:39:13.510923 alchemiscale-0.1.1/alchemiscale/interface/
--rw-r--r--   0 david     (1001) david     (1001)       39 2023-02-07 08:08:11.000000 alchemiscale-0.1.1/alchemiscale/interface/__init__.py
--rw-r--r--   0 david     (1001) david     (1001)    13870 2023-04-21 17:35:54.000000 alchemiscale-0.1.1/alchemiscale/interface/api.py
--rw-r--r--   0 david     (1001) david     (1001)    17778 2023-04-21 17:35:58.000000 alchemiscale-0.1.1/alchemiscale/interface/client.py
--rw-r--r--   0 david     (1001) david     (1001)     5712 2023-04-21 17:35:54.000000 alchemiscale-0.1.1/alchemiscale/models.py
-drwxr-xr-x   0 david     (1001) david     (1001)        0 2023-04-21 17:39:13.510923 alchemiscale-0.1.1/alchemiscale/security/
--rw-r--r--   0 david     (1001) david     (1001)        0 2023-04-16 23:09:10.000000 alchemiscale-0.1.1/alchemiscale/security/__init__.py
--rw-r--r--   0 david     (1001) david     (1001)     2036 2023-04-21 17:35:54.000000 alchemiscale-0.1.1/alchemiscale/security/auth.py
--rw-r--r--   0 david     (1001) david     (1001)     1565 2023-04-21 17:35:54.000000 alchemiscale-0.1.1/alchemiscale/security/models.py
--rw-r--r--   0 david     (1001) david     (1001)     2552 2023-04-21 17:35:54.000000 alchemiscale-0.1.1/alchemiscale/settings.py
-drwxr-xr-x   0 david     (1001) david     (1001)        0 2023-04-21 17:39:13.510923 alchemiscale-0.1.1/alchemiscale/storage/
--rw-r--r--   0 david     (1001) david     (1001)        0 2023-04-16 23:09:10.000000 alchemiscale-0.1.1/alchemiscale/storage/__init__.py
--rw-r--r--   0 david     (1001) david     (1001)     6893 2023-04-21 17:35:58.000000 alchemiscale-0.1.1/alchemiscale/storage/models.py
--rw-r--r--   0 david     (1001) david     (1001)     8843 2023-04-21 17:35:58.000000 alchemiscale-0.1.1/alchemiscale/storage/objectstore.py
--rw-r--r--   0 david     (1001) david     (1001)    69559 2023-04-21 17:35:54.000000 alchemiscale-0.1.1/alchemiscale/storage/statestore.py
-drwxr-xr-x   0 david     (1001) david     (1001)        0 2023-04-21 17:39:13.510923 alchemiscale-0.1.1/alchemiscale/strategies/
--rw-r--r--   0 david     (1001) david     (1001)       27 2023-02-07 08:08:11.000000 alchemiscale-0.1.1/alchemiscale/strategies/__init__.py
--rw-r--r--   0 david     (1001) david     (1001)      371 2023-04-21 17:35:54.000000 alchemiscale-0.1.1/alchemiscale/strategies/base.py
-drwxr-xr-x   0 david     (1001) david     (1001)        0 2023-04-21 17:39:13.510923 alchemiscale-0.1.1/alchemiscale/strategist/
--rw-r--r--   0 david     (1001) david     (1001)        0 2023-04-21 17:35:54.000000 alchemiscale-0.1.1/alchemiscale/strategist/__init__.py
--rw-r--r--   0 david     (1001) david     (1001)      213 2023-04-21 17:35:54.000000 alchemiscale-0.1.1/alchemiscale/strategist/service.py
-drwxr-xr-x   0 david     (1001) david     (1001)        0 2023-04-21 17:39:13.507589 alchemiscale-0.1.1/alchemiscale.egg-info/
--rw-r--r--   0 david     (1001) david     (1001)     1195 2023-04-21 17:39:13.000000 alchemiscale-0.1.1/alchemiscale.egg-info/PKG-INFO
--rw-r--r--   0 david     (1001) david     (1001)     1134 2023-04-21 17:39:13.000000 alchemiscale-0.1.1/alchemiscale.egg-info/SOURCES.txt
--rw-r--r--   0 david     (1001) david     (1001)        1 2023-04-21 17:39:13.000000 alchemiscale-0.1.1/alchemiscale.egg-info/dependency_links.txt
--rw-r--r--   0 david     (1001) david     (1001)       54 2023-04-21 17:39:13.000000 alchemiscale-0.1.1/alchemiscale.egg-info/entry_points.txt
--rw-r--r--   0 david     (1001) david     (1001)        1 2023-02-07 08:28:06.000000 alchemiscale-0.1.1/alchemiscale.egg-info/not-zip-safe
--rw-r--r--   0 david     (1001) david     (1001)       28 2023-04-21 17:39:13.000000 alchemiscale-0.1.1/alchemiscale.egg-info/requires.txt
--rw-r--r--   0 david     (1001) david     (1001)       13 2023-04-21 17:39:13.000000 alchemiscale-0.1.1/alchemiscale.egg-info/top_level.txt
--rw-r--r--   0 david     (1001) david     (1001)     1052 2023-04-21 17:39:13.514256 alchemiscale-0.1.1/setup.cfg
--rw-r--r--   0 david     (1001) david     (1001)      136 2022-08-27 01:07:20.000000 alchemiscale-0.1.1/setup.py
--rw-r--r--   0 david     (1001) david     (1001)    81180 2022-08-27 01:07:20.000000 alchemiscale-0.1.1/versioneer.py
+drwxr-xr-x   0 david     (1001) david     (1001)        0 2023-04-23 04:25:24.946013 alchemiscale-0.1.2/
+-rw-r--r--   0 david     (1001) david     (1001)     1084 2022-02-15 17:06:19.000000 alchemiscale-0.1.2/LICENSE
+-rw-r--r--   0 david     (1001) david     (1001)       55 2023-02-15 05:25:44.000000 alchemiscale-0.1.2/MANIFEST.in
+-rw-r--r--   0 david     (1001) david     (1001)     1195 2023-04-23 04:25:24.946013 alchemiscale-0.1.2/PKG-INFO
+-rw-r--r--   0 david     (1001) david     (1001)      610 2023-03-23 07:15:07.000000 alchemiscale-0.1.2/README.md
+drwxr-xr-x   0 david     (1001) david     (1001)        0 2023-04-23 04:25:24.946013 alchemiscale-0.1.2/alchemiscale/
+-rw-r--r--   0 david     (1001) david     (1001)      153 2023-02-15 05:25:44.000000 alchemiscale-0.1.2/alchemiscale/__init__.py
+-rw-r--r--   0 david     (1001) david     (1001)      498 2023-04-23 04:25:24.946013 alchemiscale-0.1.2/alchemiscale/_version.py
+drwxr-xr-x   0 david     (1001) david     (1001)        0 2023-04-23 04:25:24.939346 alchemiscale-0.1.2/alchemiscale/base/
+-rw-r--r--   0 david     (1001) david     (1001)        0 2023-04-18 06:27:03.000000 alchemiscale-0.1.2/alchemiscale/base/__init__.py
+-rw-r--r--   0 david     (1001) david     (1001)     6804 2023-04-17 19:03:58.000000 alchemiscale-0.1.2/alchemiscale/base/api.py
+-rw-r--r--   0 david     (1001) david     (1001)     8197 2023-04-17 19:03:58.000000 alchemiscale-0.1.2/alchemiscale/base/client.py
+-rw-r--r--   0 david     (1001) david     (1001)    17195 2023-04-17 19:03:58.000000 alchemiscale-0.1.2/alchemiscale/cli.py
+-rw-r--r--   0 david     (1001) david     (1001)      929 2023-04-17 19:03:58.000000 alchemiscale-0.1.2/alchemiscale/cli_utils.py
+drwxr-xr-x   0 david     (1001) david     (1001)        0 2023-04-23 04:25:24.939346 alchemiscale-0.1.2/alchemiscale/compute/
+-rw-r--r--   0 david     (1001) david     (1001)       46 2023-02-15 05:25:44.000000 alchemiscale-0.1.2/alchemiscale/compute/__init__.py
+-rw-r--r--   0 david     (1001) david     (1001)     7369 2023-04-19 19:27:01.000000 alchemiscale-0.1.2/alchemiscale/compute/api.py
+-rw-r--r--   0 david     (1001) david     (1001)     3699 2023-04-19 18:53:57.000000 alchemiscale-0.1.2/alchemiscale/compute/client.py
+-rw-r--r--   0 david     (1001) david     (1001)    16905 2023-04-22 03:05:51.000000 alchemiscale-0.1.2/alchemiscale/compute/service.py
+drwxr-xr-x   0 david     (1001) david     (1001)        0 2023-04-23 04:25:24.942679 alchemiscale-0.1.2/alchemiscale/interface/
+-rw-r--r--   0 david     (1001) david     (1001)       39 2023-02-15 05:25:44.000000 alchemiscale-0.1.2/alchemiscale/interface/__init__.py
+-rw-r--r--   0 david     (1001) david     (1001)    13870 2023-04-17 19:03:58.000000 alchemiscale-0.1.2/alchemiscale/interface/api.py
+-rw-r--r--   0 david     (1001) david     (1001)    18306 2023-04-19 20:37:27.000000 alchemiscale-0.1.2/alchemiscale/interface/client.py
+-rw-r--r--   0 david     (1001) david     (1001)     5712 2023-04-16 23:49:41.000000 alchemiscale-0.1.2/alchemiscale/models.py
+drwxr-xr-x   0 david     (1001) david     (1001)        0 2023-04-23 04:25:24.942679 alchemiscale-0.1.2/alchemiscale/security/
+-rw-r--r--   0 david     (1001) david     (1001)        0 2023-04-14 20:41:38.000000 alchemiscale-0.1.2/alchemiscale/security/__init__.py
+-rw-r--r--   0 david     (1001) david     (1001)     2036 2023-04-16 23:49:41.000000 alchemiscale-0.1.2/alchemiscale/security/auth.py
+-rw-r--r--   0 david     (1001) david     (1001)     1565 2023-04-16 23:49:41.000000 alchemiscale-0.1.2/alchemiscale/security/models.py
+-rw-r--r--   0 david     (1001) david     (1001)     2552 2023-04-16 23:49:41.000000 alchemiscale-0.1.2/alchemiscale/settings.py
+drwxr-xr-x   0 david     (1001) david     (1001)        0 2023-04-23 04:25:24.946013 alchemiscale-0.1.2/alchemiscale/storage/
+-rw-r--r--   0 david     (1001) david     (1001)        0 2023-04-14 20:41:38.000000 alchemiscale-0.1.2/alchemiscale/storage/__init__.py
+-rw-r--r--   0 david     (1001) david     (1001)     7000 2023-04-19 19:27:27.000000 alchemiscale-0.1.2/alchemiscale/storage/models.py
+-rw-r--r--   0 david     (1001) david     (1001)     8921 2023-04-19 19:26:45.000000 alchemiscale-0.1.2/alchemiscale/storage/objectstore.py
+-rw-r--r--   0 david     (1001) david     (1001)    69559 2023-04-17 00:02:33.000000 alchemiscale-0.1.2/alchemiscale/storage/statestore.py
+drwxr-xr-x   0 david     (1001) david     (1001)        0 2023-04-23 04:25:24.946013 alchemiscale-0.1.2/alchemiscale/strategies/
+-rw-r--r--   0 david     (1001) david     (1001)       27 2023-02-15 05:25:44.000000 alchemiscale-0.1.2/alchemiscale/strategies/__init__.py
+-rw-r--r--   0 david     (1001) david     (1001)      371 2023-04-16 23:49:41.000000 alchemiscale-0.1.2/alchemiscale/strategies/base.py
+drwxr-xr-x   0 david     (1001) david     (1001)        0 2023-04-23 04:25:24.946013 alchemiscale-0.1.2/alchemiscale/strategist/
+-rw-r--r--   0 david     (1001) david     (1001)        0 2023-04-18 06:27:53.000000 alchemiscale-0.1.2/alchemiscale/strategist/__init__.py
+-rw-r--r--   0 david     (1001) david     (1001)      213 2023-04-16 23:49:41.000000 alchemiscale-0.1.2/alchemiscale/strategist/service.py
+drwxr-xr-x   0 david     (1001) david     (1001)        0 2023-04-23 04:25:24.936013 alchemiscale-0.1.2/alchemiscale.egg-info/
+-rw-r--r--   0 david     (1001) david     (1001)     1195 2023-04-23 04:25:24.000000 alchemiscale-0.1.2/alchemiscale.egg-info/PKG-INFO
+-rw-r--r--   0 david     (1001) david     (1001)     1134 2023-04-23 04:25:24.000000 alchemiscale-0.1.2/alchemiscale.egg-info/SOURCES.txt
+-rw-r--r--   0 david     (1001) david     (1001)        1 2023-04-23 04:25:24.000000 alchemiscale-0.1.2/alchemiscale.egg-info/dependency_links.txt
+-rw-r--r--   0 david     (1001) david     (1001)       54 2023-04-23 04:25:24.000000 alchemiscale-0.1.2/alchemiscale.egg-info/entry_points.txt
+-rw-r--r--   0 david     (1001) david     (1001)        1 2023-04-23 04:25:24.000000 alchemiscale-0.1.2/alchemiscale.egg-info/not-zip-safe
+-rw-r--r--   0 david     (1001) david     (1001)       28 2023-04-23 04:25:24.000000 alchemiscale-0.1.2/alchemiscale.egg-info/requires.txt
+-rw-r--r--   0 david     (1001) david     (1001)       13 2023-04-23 04:25:24.000000 alchemiscale-0.1.2/alchemiscale.egg-info/top_level.txt
+-rw-r--r--   0 david     (1001) david     (1001)     1052 2023-04-23 04:25:24.946013 alchemiscale-0.1.2/setup.cfg
+-rw-r--r--   0 david     (1001) david     (1001)      136 2022-11-18 18:18:33.000000 alchemiscale-0.1.2/setup.py
+-rw-r--r--   0 david     (1001) david     (1001)    81180 2023-03-16 05:35:03.000000 alchemiscale-0.1.2/versioneer.py
```

### Comparing `alchemiscale-0.1.1/LICENSE` & `alchemiscale-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alchemiscale-0.1.1/PKG-INFO` & `alchemiscale-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alchemiscale
-Version: 0.1.1
+Version: 0.1.2
 Home-page: https://github.com/openforcefield/alchemiscale
 Author: OpenFE and OpenFF developers
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
```

### Comparing `alchemiscale-0.1.1/README.md` & `alchemiscale-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `alchemiscale-0.1.1/alchemiscale/base/api.py` & `alchemiscale-0.1.2/alchemiscale/base/api.py`

 * *Files identical despite different names*

### Comparing `alchemiscale-0.1.1/alchemiscale/base/client.py` & `alchemiscale-0.1.2/alchemiscale/base/client.py`

 * *Files identical despite different names*

### Comparing `alchemiscale-0.1.1/alchemiscale/cli.py` & `alchemiscale-0.1.2/alchemiscale/cli.py`

 * *Files identical despite different names*

### Comparing `alchemiscale-0.1.1/alchemiscale/cli_utils.py` & `alchemiscale-0.1.2/alchemiscale/cli_utils.py`

 * *Files identical despite different names*

### Comparing `alchemiscale-0.1.1/alchemiscale/compute/api.py` & `alchemiscale-0.1.2/alchemiscale/compute/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 AlchemiscaleComputeAPI --- :mod:`alchemiscale.compute.api`
 ==========================================================
 
 """
 
-from typing import Any, Dict, List
+from typing import Any, Dict, List, Optional
 import os
 import json
 from datetime import datetime, timedelta
 
 from fastapi import FastAPI, APIRouter, Body, Depends, HTTPException, status
 from gufe.tokenization import GufeTokenizable, JSON_HANDLER
 
@@ -218,28 +218,28 @@
 
 # TODO: support compression performed client-side
 @router.post("/tasks/{task_scoped_key}/results", response_model=ScopedKey)
 def set_task_result(
     task_scoped_key,
     *,
     protocoldagresult: str = Body(embed=True),
+    compute_service_id: Optional[str] = Body(embed=True),
     n4js: Neo4jStore = Depends(get_n4js_depends),
     s3os: S3ObjectStore = Depends(get_s3os_depends),
     token: TokenData = Depends(get_token_data_depends),
 ):
     task_sk = ScopedKey.from_str(task_scoped_key)
     validate_scopes(task_sk.scope, token)
 
     pdr = json.loads(protocoldagresult, cls=JSON_HANDLER.decoder)
     pdr = GufeTokenizable.from_dict(pdr)
 
     # push the ProtocolDAGResult to the object store
     protocoldagresultref: ProtocolDAGResultRef = s3os.push_protocoldagresult(
-        pdr,
-        scope=task_sk.scope,
+        pdr, scope=task_sk.scope, creator=compute_service_id
     )
 
     # push the reference to the state store
     result_sk: ScopedKey = n4js.set_task_result(
         task=task_sk, protocoldagresultref=protocoldagresultref
     )
```

### Comparing `alchemiscale-0.1.1/alchemiscale/compute/client.py` & `alchemiscale-0.1.2/alchemiscale/compute/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -89,18 +89,22 @@
 
         return (
             json_to_gufe(transformation),
             json_to_gufe(protocoldagresult) if protocoldagresult is not None else None,
         )
 
     def set_task_result(
-        self, task: ScopedKey, protocoldagresult: ProtocolDAGResult
+        self,
+        task: ScopedKey,
+        protocoldagresult: ProtocolDAGResult,
+        compute_service_id=Optional[ComputeServiceID],
     ) -> ScopedKey:
         data = dict(
             protocoldagresult=json.dumps(
                 protocoldagresult.to_dict(), cls=JSON_HANDLER.encoder
-            )
+            ),
+            compute_service_id=str(compute_service_id),
         )
 
         pdr_sk = self._post_resource(f"tasks/{task}/results", data)
 
         return ScopedKey.from_dict(pdr_sk)
```

### Comparing `alchemiscale-0.1.1/alchemiscale/compute/service.py` & `alchemiscale-0.1.2/alchemiscale/compute/service.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 AlchemiscaleComputeService --- :mod:`alchemiscale.compute.service`
 ==================================================================
 
 """
 
 import os
+import gc
 import asyncio
 import sched
 import time
 import logging
 from uuid import uuid4
 import random
 import threading
@@ -208,15 +209,15 @@
     def _deregister(self):
         """Deregister this compute service with the compute API."""
         self.client.deregister(self.compute_service_id)
 
     def beat(self):
         """Deliver a heartbeat to the compute API, indicating this service is still alive."""
         self.client.heartbeat(self.compute_service_id)
-        self.logger.info("Updated heartbeat")
+        self.logger.debug("Updated heartbeat")
 
     def heartbeat(self):
         """Start up the heartbeat, sleeping for `self.heartbeat_interval`"""
         while True:
             if self._stop:
                 break
             self.beat()
@@ -289,28 +290,35 @@
     ) -> ScopedKey:
         # TODO: this method should postprocess any paths,
         # leaf nodes in DAG for blob results that should go to object store
 
         # TODO: ship paths to object store
 
         # finally, push ProtocolDAGResult
-        sk: ScopedKey = self.client.set_task_result(task, protocoldagresult)
+        sk: ScopedKey = self.client.set_task_result(
+            task, protocoldagresult, self.compute_service_id
+        )
 
         return sk
 
     def execute(self, task: ScopedKey) -> ScopedKey:
         """Executes given Task.
 
         Returns ScopedKey of ProtocolDAGResultRef following push to database.
 
         """
         # obtain a ProtocolDAG from the task
-        self.logger.info("Creating ProtocolDAG from task '%s'...", task)
+        self.logger.info("Creating ProtocolDAG from '%s'...", task)
         protocoldag, transformation, extends = self.task_to_protocoldag(task)
-        self.logger.info("Created '%s' from task '%s'", protocoldag, task)
+        self.logger.info(
+            "Created '%s' from '%s' performing '%s'",
+            protocoldag,
+            task,
+            transformation.protocol,
+        )
 
         # execute the task; this looks the same whether the ProtocolDAG is a
         # success or failure
 
         shared = self.shared_basedir / str(protocoldag.key)
         shared.mkdir()
         scratch = self.scratch_basedir / str(protocoldag.key)
@@ -328,20 +336,21 @@
         finally:
             if not self.keep_shared:
                 shutil.rmtree(shared)
 
             if not self.keep_scratch:
                 shutil.rmtree(scratch)
 
-        if protocoldagresult.ok:
-            self.logger.info("'%s' : SUCCESS", protocoldagresult)
+        if protocoldagresult.ok():
+            self.logger.info("'%s' -> '%s' : SUCCESS", protocoldag, protocoldagresult)
         else:
             for failure in protocoldagresult.protocol_unit_failures:
                 self.logger.info(
-                    "'%s' : FAILURE : '%s' : %s",
+                    "'%s' -> '%s' : FAILURE :: '%s' : %s",
+                    protocoldag,
                     protocoldagresult,
                     failure,
                     failure.exception,
                 )
 
         # push the result (or failure) back to the compute API
         result_sk = self.push_result(task, protocoldagresult)
@@ -448,14 +457,17 @@
                     self.heartbeat_thread = threading.Thread(
                         target=self.heartbeat, daemon=True
                     )
                     self.heartbeat_thread.start()
 
                 # perform main loop cycle
                 self.cycle(max_tasks, max_time)
+
+                # force a garbage collection to avoid consuming too much memory
+                gc.collect()
         except KeyboardInterrupt:
             self.logger.info("Caught SIGINT/Keyboard interrupt.")
         except SleepInterrupted:
             self.logger.info("Service stopping.")
         finally:
             # remove ComputeServiceRegistration, drop all claims
             self._deregister()
```

### Comparing `alchemiscale-0.1.1/alchemiscale/interface/api.py` & `alchemiscale-0.1.2/alchemiscale/interface/api.py`

 * *Files identical despite different names*

### Comparing `alchemiscale-0.1.1/alchemiscale/interface/client.py` & `alchemiscale-0.1.2/alchemiscale/interface/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -417,17 +417,26 @@
 
         return pdrs
 
     def get_transformation_results(
         self,
         transformation: ScopedKey,
         return_protocoldagresults: bool = False,
-    ) -> Union[ProtocolResult, List[ProtocolDAGResult]]:
+    ) -> Union[Optional[ProtocolResult], List[ProtocolDAGResult]]:
         """Get a `ProtocolResult` for the given `Transformation`.
 
+        A `ProtocolResult` object corresponding to the `Protocol` used for this
+        `Transformation`. This is constructed from the available
+        `ProtocolDAGResult`\s for this `Transformation`. If no
+        `ProtocolDAGResult`\s exist for this `Transformation`, ``None`` is
+        returned.
+
+        If `return_protocoldagresults` is ``True``, then a list of the
+        `ProtocolDAGResult`\s themselves are returned instead.
+
         Parameters
         ----------
         transformation
             The `ScopedKey` of the `Transformation` to retrieve results for.
         return_protocoldagresults
             If `True`, return the raw `ProtocolDAGResult`s instead of returning
             a processed `ProtocolResult`. Only successful `ProtocolDAGResult`\s
@@ -447,15 +456,18 @@
         pdrs = self._get_prototocoldagresults(
             protocoldagresultrefs, transformation, ok=True
         )
 
         if return_protocoldagresults:
             return pdrs
         else:
-            return tf.gather(pdrs)
+            if len(pdrs) != 0:
+                return tf.gather(pdrs)
+            else:
+                return None
 
     def get_transformation_failures(
         self,
         transformation: ScopedKey,
     ) -> Union[ProtocolResult, List[ProtocolDAGResult]]:
         """Get failed `ProtocolDAGResult`\s for the given `Transformation`.
```

### Comparing `alchemiscale-0.1.1/alchemiscale/models.py` & `alchemiscale-0.1.2/alchemiscale/models.py`

 * *Files identical despite different names*

### Comparing `alchemiscale-0.1.1/alchemiscale/security/auth.py` & `alchemiscale-0.1.2/alchemiscale/security/auth.py`

 * *Files identical despite different names*

### Comparing `alchemiscale-0.1.1/alchemiscale/security/models.py` & `alchemiscale-0.1.2/alchemiscale/security/models.py`

 * *Files identical despite different names*

### Comparing `alchemiscale-0.1.1/alchemiscale/settings.py` & `alchemiscale-0.1.2/alchemiscale/settings.py`

 * *Files identical despite different names*

### Comparing `alchemiscale-0.1.1/alchemiscale/storage/models.py` & `alchemiscale-0.1.2/alchemiscale/storage/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -241,30 +241,33 @@
         self,
         *,
         location: Optional[str] = None,
         obj_key: GufeKey,
         scope: Scope,
         ok: bool,
         datetime_created: Optional[datetime] = None,
+        creator: Optional[str] = None,
     ):
         self.location = location
         self.obj_key = GufeKey(obj_key)
         self.scope = scope
         self.ok = ok
         self.datetime_created = datetime_created
+        self.creator = creator
 
     def _to_dict(self):
         return {
             "location": self.location,
             "obj_key": str(self.obj_key),
             "scope": str(self.scope),
             "ok": self.ok,
             "datetime_created": self.datetime_created.isoformat()
             if self.datetime_created is not None
             else None,
+            "creator": self.creator,
         }
 
     @classmethod
     def _from_dict(cls, d):
         d_ = copy(d)
         d_["datetime_created"] = (
             datetime.fromisoformat(d["datetime_created"])
```

### Comparing `alchemiscale-0.1.1/alchemiscale/storage/objectstore.py` & `alchemiscale-0.1.2/alchemiscale/storage/objectstore.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 """
 
 import os
 import io
 import json
 from datetime import datetime
-from typing import Union
+from typing import Union, Optional
 from boto3.session import Session
 from functools import lru_cache
 
 from gufe.protocols import ProtocolDAGResult
 from gufe.tokenization import JSON_HANDLER, GufeTokenizable
 
 from ..models import ScopedKey, Scope
@@ -192,14 +192,15 @@
 
         return url
 
     def push_protocoldagresult(
         self,
         protocoldagresult: ProtocolDAGResult,
         scope: Scope,
+        creator: Optional[str] = None,
     ) -> ProtocolDAGResultRef:
         """Push given `ProtocolDAGResult` to this `ObjectStore`.
 
         Parameters
         ----------
         protocoldagresult
             ProtocolDAGResult to store.
@@ -233,14 +234,15 @@
 
         return ProtocolDAGResultRef(
             location=location,
             obj_key=protocoldagresult.key,
             scope=scope,
             ok=ok,
             datetime_created=datetime.utcnow(),
+            creator=creator,
         )
 
     def pull_protocoldagresult(
         self,
         protocoldagresult: ScopedKey,
         transformation: ScopedKey,
         return_as="gufe",
```

### Comparing `alchemiscale-0.1.1/alchemiscale/storage/statestore.py` & `alchemiscale-0.1.2/alchemiscale/storage/statestore.py`

 * *Files identical despite different names*

### Comparing `alchemiscale-0.1.1/alchemiscale.egg-info/PKG-INFO` & `alchemiscale-0.1.2/alchemiscale.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alchemiscale
-Version: 0.1.1
+Version: 0.1.2
 Home-page: https://github.com/openforcefield/alchemiscale
 Author: OpenFE and OpenFF developers
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
```

### Comparing `alchemiscale-0.1.1/alchemiscale.egg-info/SOURCES.txt` & `alchemiscale-0.1.2/alchemiscale.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alchemiscale-0.1.1/setup.cfg` & `alchemiscale-0.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `alchemiscale-0.1.1/versioneer.py` & `alchemiscale-0.1.2/versioneer.py`

 * *Files identical despite different names*

