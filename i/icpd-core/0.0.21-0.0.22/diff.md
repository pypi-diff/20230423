# Comparing `tmp/icpd_core-0.0.21-py3-none-any.whl.zip` & `tmp/icpd_core-0.0.22-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 474413 bytes, number of entries: 279
+Zip file size: 474676 bytes, number of entries: 279
 -rw-r--r--  2.0 unx    19236 b- defN 20-Feb-02 00:00 icpd_core/__init__.py
 -rw-r--r--  2.0 unx    24964 b- defN 20-Feb-02 00:00 icpd_core/api_client.py
 -rw-r--r--  2.0 unx     7812 b- defN 20-Feb-02 00:00 icpd_core/configuration.py
--rw-r--r--  2.0 unx    10590 b- defN 20-Feb-02 00:00 icpd_core/icpd_util.py
+-rw-r--r--  2.0 unx    11396 b- defN 20-Feb-02 00:00 icpd_core/icpd_util.py
 -rw-r--r--  2.0 unx    13157 b- defN 20-Feb-02 00:00 icpd_core/rest.py
 -rw-r--r--  2.0 unx     3136 b- defN 20-Feb-02 00:00 icpd_core/api/__init__.py
 -rw-r--r--  2.0 unx    46244 b- defN 20-Feb-02 00:00 icpd_core/api/access_management_api.py
 -rw-r--r--  2.0 unx    20988 b- defN 20-Feb-02 00:00 icpd_core/api/access_management_v3_api.py
 -rw-r--r--  2.0 unx    12690 b- defN 20-Feb-02 00:00 icpd_core/api/account_management_api.py
 -rw-r--r--  2.0 unx    35086 b- defN 20-Feb-02 00:00 icpd_core/api/add_on_manager_api.py
 -rw-r--r--  2.0 unx     4429 b- defN 20-Feb-02 00:00 icpd_core/api/authorization_api.py
@@ -270,12 +270,12 @@
 -rw-r--r--  2.0 unx     4189 b- defN 20-Feb-02 00:00 icpd_core/models/user_role.py
 -rw-r--r--  2.0 unx     3869 b- defN 20-Feb-02 00:00 icpd_core/models/vault_details_response.py
 -rw-r--r--  2.0 unx    15991 b- defN 20-Feb-02 00:00 icpd_core/models/vault_meta_data.py
 -rw-r--r--  2.0 unx     3149 b- defN 20-Feb-02 00:00 icpd_core/models/vault_response.py
 -rw-r--r--  2.0 unx     4134 b- defN 20-Feb-02 00:00 icpd_core/models/volume_object.py
 -rw-r--r--  2.0 unx     3652 b- defN 20-Feb-02 00:00 icpd_core/models/volumes_obj.py
 -rw-r--r--  2.0 unx     3509 b- defN 20-Feb-02 00:00 icpd_core/models/zen_service_instance_info.py
-?rw-r--r--  2.0 unx     5641 b- defN 20-Feb-02 00:00 icpd_core-0.0.21.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 icpd_core-0.0.21.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1073 b- defN 20-Feb-02 00:00 icpd_core-0.0.21.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx    27021 b- defN 20-Feb-02 00:00 icpd_core-0.0.21.dist-info/RECORD
-279 files, 2468114 bytes uncompressed, 430959 bytes compressed:  82.5%
+?rw-r--r--  2.0 unx     5641 b- defN 20-Feb-02 00:00 icpd_core-0.0.22.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 icpd_core-0.0.22.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1073 b- defN 20-Feb-02 00:00 icpd_core-0.0.22.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx    27021 b- defN 20-Feb-02 00:00 icpd_core-0.0.22.dist-info/RECORD
+279 files, 2468920 bytes uncompressed, 431222 bytes compressed:  82.6%
```

## zipnote {}

```diff
@@ -819,20 +819,20 @@
 
 Filename: icpd_core/models/volumes_obj.py
 Comment: 
 
 Filename: icpd_core/models/zen_service_instance_info.py
 Comment: 
 
-Filename: icpd_core-0.0.21.dist-info/METADATA
+Filename: icpd_core-0.0.22.dist-info/METADATA
 Comment: 
 
-Filename: icpd_core-0.0.21.dist-info/WHEEL
+Filename: icpd_core-0.0.22.dist-info/WHEEL
 Comment: 
 
-Filename: icpd_core-0.0.21.dist-info/licenses/LICENSE
+Filename: icpd_core-0.0.22.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: icpd_core-0.0.21.dist-info/RECORD
+Filename: icpd_core-0.0.22.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## icpd_core/icpd_util.py

```diff
@@ -6,25 +6,49 @@
 
 api_client = None
 amapi = None
 smapi = None
 conn_api = None
 
 icpd_token = ''
+zencoreapi_host = None
+
+# Using environment var RUNTIME_ENV_APSX_URL published by Jupyter environment extract controlplane namespace
+# after first period (.)
+def extract_controlplane_ns():
+    cplane_ns = None
+    ns_delimiter = '.'
+    # Getting internal ngix URL
+    int_nginx_url = os.environ.get('RUNTIME_ENV_APSX_URL')
+    if int_nginx_url is None:
+        return
+    fIndex = int_nginx_url.find(ns_delimiter)+1
+    if fIndex <= 0:
+        return
+    nIndex = int_nginx_url[fIndex:].find(ns_delimiter)
+    if nIndex <= 0:
+        return
+    cplane_ns = int_nginx_url[fIndex:fIndex+nIndex]
+    return cplane_ns
+
 
 def init_utils(host=None, token=None, verify_ssl=False):
     global api_client
     global amapi
     global smapi
     global conn_api
     global icpd_token
     global zencoreapi_host
-   
-    if zencoreapi_host is None:
+
+    # Update after v2/secrets are exposed through internal nginx configuration
+    cp_ns = extract_controlplane_ns()
+    if cp_ns is None:
         zencoreapi_host = 'https://zen-core-api-svc:4444'
+    else:
+        zencoreapi_host = 'https://zen-core-api-svc.' + cp_ns + '.svc:4444'
 
     configuration = icpd_core.Configuration()
 
     configuration.host = host
     if host is None:
         configuration.host = 'https://zen-core-api-svc:4444'
```

## Comparing `icpd_core-0.0.21.dist-info/METADATA` & `icpd_core-0.0.22.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icpd_core
-Version: 0.0.21
+Version: 0.0.22
 Summary: IBM CPD Core Python Client
 Project-URL: Homepage, https://www.ibm.com/docs/en/cloud-paks/cp-data/4.6.x?topic=2-managing-secrets-vaults
 Author-email: IBM <rahul.shinge@us.ibm.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

## Comparing `icpd_core-0.0.21.dist-info/licenses/LICENSE` & `icpd_core-0.0.22.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `icpd_core-0.0.21.dist-info/RECORD` & `icpd_core-0.0.22.dist-info/RECORD`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 icpd_core/__init__.py,sha256=IwuwZAK8TotL75RdkaFD2lshv6r9kcgVyP_hup5_rzs,19236
 icpd_core/api_client.py,sha256=WU1uZBcAVZ_d_QzZjJYEOCor2MNeRFjylFJiuW7j9C4,24964
 icpd_core/configuration.py,sha256=xpvMI12tvjvLRpuHtljOT5-A0R_wGDHXsil1ol9a9X8,7812
-icpd_core/icpd_util.py,sha256=rNNhNjLAnOeTyvw3hR_1o6AGMsMngME7BUQl9FGE96M,10590
+icpd_core/icpd_util.py,sha256=jvqHyPC3Q17-caHMoSzwELQOZiJY3C3_AhfkYnQ_YyM,11396
 icpd_core/rest.py,sha256=nGMqsuP_2YvN-IGGwQaH4j3H1gJb0wPGjOPWHstFSuo,13157
 icpd_core/api/__init__.py,sha256=Ghf656D7Q6EBaQPhmXJWeqeScftkrAR_zT_7ZnuOihQ,3136
 icpd_core/api/access_management_api.py,sha256=iMfAJ37l8Zrgr4iCtteA_0CgxLg3TXyOcryGXNdiVT4,46244
 icpd_core/api/access_management_v3_api.py,sha256=r-0paovW1Kbqc955irAwnJ6S59re_Rr9T9Bxz3Fq4ko,20988
 icpd_core/api/account_management_api.py,sha256=FmFfL9-GxUhT1bMRlnrOaFSYttF-yfDf9bgjH_S685o,12690
 icpd_core/api/add_on_manager_api.py,sha256=dLpBOUydIA_djlj6khde6P-jLVwiQnLOMCyd4WBj1Ic,35086
 icpd_core/api/authorization_api.py,sha256=k94-ZzabdBu0URZ4TRPONGXxOc0fu5AvYj5UZVzhbnk,4429
@@ -269,11 +269,11 @@
 icpd_core/models/user_role.py,sha256=DzIu3y8eeqCYLhpGx2ASp6qLTw03EvzxdwAazAZZ6cY,4189
 icpd_core/models/vault_details_response.py,sha256=u4_u0-XPgVfclPvsfn6wPmDmfYmEpb2CtlA53u97qNU,3869
 icpd_core/models/vault_meta_data.py,sha256=uhHrrCaJpuMhSGzt64Sd65aCMR2Tlmu2yrlHdMnx-mE,15991
 icpd_core/models/vault_response.py,sha256=BfkZetV-2nhRVVrCo1MUzZsaPP76-jJLFuBQMGT5aNs,3149
 icpd_core/models/volume_object.py,sha256=hMTXFBaCPKGAcBJVBW69tcnHF6nfu6GF8E42Ik5K_rg,4134
 icpd_core/models/volumes_obj.py,sha256=DEGLHN4J0tyDlscZF54V2Hr-i3yjzTNeH3OxqUm_k0g,3652
 icpd_core/models/zen_service_instance_info.py,sha256=MtJf0FQpKDG_TeAfBs3cDCdvwxM7FXC0gDDrm5qAY0k,3509
-icpd_core-0.0.21.dist-info/METADATA,sha256=6G5aVyhqYueGP1-tITZ6IHd1pfzxhKyrAgebu6rBybw,5641
-icpd_core-0.0.21.dist-info/WHEEL,sha256=EI2JsGydwUL5GP9t6kzZv7G3HDPi7FuZDDf9In6amRM,87
-icpd_core-0.0.21.dist-info/licenses/LICENSE,sha256=2bm9uFabQZ3Ykb_SaSU_uUbAj2-htc6WJQmS_65qD00,1073
-icpd_core-0.0.21.dist-info/RECORD,,
+icpd_core-0.0.22.dist-info/METADATA,sha256=GCmAmkVc65Hyz_gw5brI7BvwWnQ6MECw5KwYXR3h3Ak,5641
+icpd_core-0.0.22.dist-info/WHEEL,sha256=EI2JsGydwUL5GP9t6kzZv7G3HDPi7FuZDDf9In6amRM,87
+icpd_core-0.0.22.dist-info/licenses/LICENSE,sha256=2bm9uFabQZ3Ykb_SaSU_uUbAj2-htc6WJQmS_65qD00,1073
+icpd_core-0.0.22.dist-info/RECORD,,
```

