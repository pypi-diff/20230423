# Comparing `tmp/sui_brownie-0.31.3-py3-none-any.whl.zip` & `tmp/sui_brownie-0.31.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 27597 bytes, number of entries: 16
+Zip file size: 27601 bytes, number of entries: 16
 -rw-r--r--  2.0 unx       10 b- defN 22-Dec-02 09:41 sui_brownie/MANIFEST.in
 -rw-r--r--  2.0 unx      878 b- defN 23-Apr-01 13:03 sui_brownie/README.md
 -rw-r--r--  2.0 unx       38 b- defN 23-Apr-11 02:45 sui_brownie/__init__.py
 -rw-r--r--  2.0 unx     2514 b- defN 23-Apr-01 12:52 sui_brownie/account.py
--rw-r--r--  2.0 unx    12144 b- defN 23-Apr-01 10:43 sui_brownie/bcs.py
+-rw-r--r--  2.0 unx    12144 b- defN 23-Apr-21 09:58 sui_brownie/bcs.py
 -rw-r--r--  2.0 unx     4326 b- defN 23-Apr-01 12:53 sui_brownie/ed25519.py
 -rw-r--r--  2.0 unx    10047 b- defN 22-Dec-02 09:41 sui_brownie/parallelism.py
--rw-r--r--  2.0 unx    91115 b- defN 23-Apr-21 09:48 sui_brownie/sui_brownie.py
+-rw-r--r--  2.0 unx    91352 b- defN 23-Apr-23 09:38 sui_brownie/sui_brownie.py
 -rw-r--r--  2.0 unx    32439 b- defN 23-Apr-19 08:03 sui_brownie/sui_client.py
 -rw-r--r--  2.0 unx      140 b- defN 22-Dec-02 09:41 sui_brownie/sui_config.template.yaml
 -rw-r--r--  2.0 unx       19 b- defN 22-Dec-02 09:41 sui_brownie/sui_keystore.template.keystore
 -rw-r--r--  2.0 unx      866 b- defN 23-Apr-11 02:45 sui_brownie/utils.py
--rw-r--r--  2.0 unx      983 b- defN 23-Apr-21 09:52 sui_brownie-0.31.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-21 09:52 sui_brownie-0.31.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Apr-21 09:52 sui_brownie-0.31.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1300 b- defN 23-Apr-21 09:52 sui_brownie-0.31.3.dist-info/RECORD
-16 files, 156923 bytes uncompressed, 25455 bytes compressed:  83.8%
+-rw-r--r--  2.0 unx      983 b- defN 23-Apr-23 09:39 sui_brownie-0.31.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-23 09:39 sui_brownie-0.31.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Apr-23 09:39 sui_brownie-0.31.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1300 b- defN 23-Apr-23 09:39 sui_brownie-0.31.4.dist-info/RECORD
+16 files, 157160 bytes uncompressed, 25459 bytes compressed:  83.8%
```

## zipnote {}

```diff
@@ -30,20 +30,20 @@
 
 Filename: sui_brownie/sui_keystore.template.keystore
 Comment: 
 
 Filename: sui_brownie/utils.py
 Comment: 
 
-Filename: sui_brownie-0.31.3.dist-info/METADATA
+Filename: sui_brownie-0.31.4.dist-info/METADATA
 Comment: 
 
-Filename: sui_brownie-0.31.3.dist-info/WHEEL
+Filename: sui_brownie-0.31.4.dist-info/WHEEL
 Comment: 
 
-Filename: sui_brownie-0.31.3.dist-info/top_level.txt
+Filename: sui_brownie-0.31.4.dist-info/top_level.txt
 Comment: 
 
-Filename: sui_brownie-0.31.3.dist-info/RECORD
+Filename: sui_brownie-0.31.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sui_brownie/sui_brownie.py

```diff
@@ -1424,15 +1424,20 @@
             view = f"Upgrade {self.package_name}"
             print("\n" + "-" * 50 + view + "-" * 50)
             result = self.project.upgrade(self.package_id, move_modules, dep_ids,
                                           upgrade_capability,
                                           upgrade_policy, digest,
                                           gas_price, gas_budget,
                                           )
-            self.update_abi()
+            for d in result.get("objectChanges", []):
+                if d["type"] == "published":
+                    self.package_id = d["packageId"]
+                    self.project.add_package(self)
+                    self.update_abi()
+                    break
             result = self.format_result(result)
             pprint(result)
             assert self.package_id is not None, f"Package id not found"
             print("-" * (100 + len(view)))
             print("\n")
             for k in replace_tomls:
                 replace_tomls[k].restore()
```

## Comparing `sui_brownie-0.31.3.dist-info/METADATA` & `sui_brownie-0.31.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sui-brownie
-Version: 0.31.3
+Version: 0.31.4
 Summary: Sui Package Tool
 Home-page: https://github.com/OmniBTC/DolaProtocol/blob/main/utils
 Author: DaiWei
 Author-email: dw1253464613@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

