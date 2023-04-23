# Comparing `tmp/cwsearch_utils-0.1.8-py3-none-any.whl.zip` & `tmp/cwsearch_utils-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 5632 bytes, number of entries: 8
+Zip file size: 5582 bytes, number of entries: 8
 -rw-rw-r--  2.0 unx        0 b- defN 23-Apr-09 04:52 cwsearch_utils/__init__.py
--rw-rw-r--  2.0 unx     7836 b- defN 23-Apr-20 04:42 cwsearch_utils/aggregate.py
+-rw-rw-r--  2.0 unx     7265 b- defN 23-Apr-20 05:19 cwsearch_utils/aggregate.py
 -rw-rw-r--  2.0 unx      210 b- defN 23-Apr-19 17:07 cwsearch_utils/infinstor_dbutils.py
--rw-rw-r--  2.0 unx     4780 b- defN 23-Apr-18 00:21 cwsearch_utils/infinstor_lock.py
--rw-rw-r--  2.0 unx      570 b- defN 23-Apr-20 04:43 cwsearch_utils-0.1.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-20 04:43 cwsearch_utils-0.1.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       15 b- defN 23-Apr-20 04:43 cwsearch_utils-0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      669 b- defN 23-Apr-20 04:43 cwsearch_utils-0.1.8.dist-info/RECORD
-8 files, 14172 bytes uncompressed, 4450 bytes compressed:  68.6%
+-rw-rw-r--  2.0 unx     4959 b- defN 23-Apr-20 05:20 cwsearch_utils/infinstor_lock.py
+-rw-rw-r--  2.0 unx      570 b- defN 23-Apr-20 05:20 cwsearch_utils-0.1.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-20 05:20 cwsearch_utils-0.1.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       15 b- defN 23-Apr-20 05:20 cwsearch_utils-0.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      669 b- defN 23-Apr-20 05:20 cwsearch_utils-0.1.9.dist-info/RECORD
+8 files, 13780 bytes uncompressed, 4400 bytes compressed:  68.1%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: cwsearch_utils/infinstor_dbutils.py
 Comment: 
 
 Filename: cwsearch_utils/infinstor_lock.py
 Comment: 
 
-Filename: cwsearch_utils-0.1.8.dist-info/METADATA
+Filename: cwsearch_utils-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: cwsearch_utils-0.1.8.dist-info/WHEEL
+Filename: cwsearch_utils-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: cwsearch_utils-0.1.8.dist-info/top_level.txt
+Filename: cwsearch_utils-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: cwsearch_utils-0.1.8.dist-info/RECORD
+Filename: cwsearch_utils-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cwsearch_utils/aggregate.py

```diff
@@ -33,25 +33,20 @@
         else:
             resp = s3client.list_objects_v2(Bucket=bucket, Delimiter='/', Prefix=prefix)
         if 'Contents' in resp:
             for one in resp['Contents']:
                 nm = one['Key']
                 if not nm[-1] == '/':
                     if resources:
-                        print(f"resources specified. evaluating file {nm} of sz {one['Size']} last_mod {one['LastModified']}", flush=True)
                         for res in resources:
                             arn = arnparse(res)
                             munged_resource_id = arn.resource.replace('/', '_')
                             if munged_resource_id in nm:
-                                print(f"Add: {nm}, size {one['Size']}, last_mod {one['LastModified']}. res_id={munged_resource_id}", flush=True)
                                 rv.append([nm, one['Size'], one['LastModified']])
-                            else:
-                                print(f"Skip: {nm}, size {one['Size']}, last_mod {one['LastModified']}. res_id={munged_resource_id}", flush=True)
                     else:
-                        print(f"Add: {nm} of sz {one['Size']} last_mod {one['LastModified']}", flush=True)
                         rv.append([nm, one['Size'], one['LastModified']])
         if not resp['IsTruncated']:
             break
         else:
             nextContinuationToken = resp['NextContinuationToken']
 
 def resources_for_tag(s3client, bucket, prefix, tag):
```

## cwsearch_utils/infinstor_lock.py

```diff
@@ -55,15 +55,20 @@
     return rv
 
 # returns 'NotPresent'|'Creating'|'Ready'|'CreationFailed', names|None
 def get_cache_entry(bucket, prefix, infinstor_time_spec, tag, head_only):
     import boto3
     import botocore
     s3client = boto3.client('s3')
-    object_name = f"{prefix}/index/{infinstor_time_spec}/names.db"
+    if tag:
+        object_name = f"{prefix}/index/{infinstor_time_spec}/names-{tag}.db"
+    else:
+        object_name = f"{prefix}/index/{infinstor_time_spec}/names.db"
+
+    print(f'get_cache_entry: object={object_name}, head_only={head_only}')
 
     if head_only:
         try:
             metadata = s3client.head_object(Bucket=bucket, Key=object_name)
             return 'Ready', {}
         except botocore.exceptions.ClientError as e:
             if e.response['Error']['Code'] == "404":
```

## Comparing `cwsearch_utils-0.1.8.dist-info/METADATA` & `cwsearch_utils-0.1.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cwsearch-utils
-Version: 0.1.8
+Version: 0.1.9
 Summary: InfinStor InfinLogs CloudWatch Search Utilities
 Home-page: https://infinstor.com/
 Author: InfinStor, Inc.
 Author-email: support@infinstor.com
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

## Comparing `cwsearch_utils-0.1.8.dist-info/RECORD` & `cwsearch_utils-0.1.9.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 cwsearch_utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-cwsearch_utils/aggregate.py,sha256=XwzClBWwSwEWFetylgHMS_S_ZaLnaLNs2rvZZD_wfOc,7836
+cwsearch_utils/aggregate.py,sha256=mUewsBxSaI24ak_Z7TgrI6AlIu3wfLWW52MxZvuvoBU,7265
 cwsearch_utils/infinstor_dbutils.py,sha256=kC2AgOEON5kIz64TSgGpkdzWuzJUW84rlwosrMRN9cg,210
-cwsearch_utils/infinstor_lock.py,sha256=kxY_afhPD8K50s1C-bxzs0DX3I28HLsayM-fn8H0Sw8,4780
-cwsearch_utils-0.1.8.dist-info/METADATA,sha256=cciOILblx4txKHIWWi57GQOYda3prcg3sNir2GSHjnI,570
-cwsearch_utils-0.1.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-cwsearch_utils-0.1.8.dist-info/top_level.txt,sha256=OGqL3fU8yTeTOI4vTn4QZa2PZY145LPKbmtLSjWi9kY,15
-cwsearch_utils-0.1.8.dist-info/RECORD,,
+cwsearch_utils/infinstor_lock.py,sha256=SjQLs6ozO2ZRX7tT93WICvGF8ESAmrKvcnN9Z7pUbiY,4959
+cwsearch_utils-0.1.9.dist-info/METADATA,sha256=XdK9QFDjy8voIiHeR8kY4zhiDBm_jm5bDNThgFCtgj4,570
+cwsearch_utils-0.1.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+cwsearch_utils-0.1.9.dist-info/top_level.txt,sha256=OGqL3fU8yTeTOI4vTn4QZa2PZY145LPKbmtLSjWi9kY,15
+cwsearch_utils-0.1.9.dist-info/RECORD,,
```

