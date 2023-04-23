# Comparing `tmp/cnd_vault-0.1.0-py3-none-any.whl.zip` & `tmp/cnd_vault-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 3633 bytes, number of entries: 11
--rw-rw-rw-  2.0 unx        5 b- defN 23-Apr-23 19:18 vault/VERSION
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-23 19:18 vault/__init__.py
--rw-r--r--  2.0 unx      114 b- defN 23-Apr-23 19:18 vault/__version__.py
--rw-r--r--  2.0 unx      396 b- defN 23-Apr-23 19:18 vault/v1.py
--rw-r--r--  2.0 unx     1095 b- defN 23-Apr-23 19:18 vault/v2.py
--rw-r--r--  2.0 unx     1500 b- defN 23-Apr-23 19:18 vault/vault.py
--rw-r--r--  2.0 unx      771 b- defN 23-Apr-23 19:18 vault/vault_base.py
--rw-r--r--  2.0 unx      528 b- defN 23-Apr-23 19:19 cnd_vault-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-23 19:19 cnd_vault-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Apr-23 19:19 cnd_vault-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      800 b- defN 23-Apr-23 19:19 cnd_vault-0.1.0.dist-info/RECORD
-11 files, 5399 bytes uncompressed, 2293 bytes compressed:  57.5%
+Zip file size: 3695 bytes, number of entries: 11
+-rw-rw-rw-  2.0 unx        5 b- defN 23-Apr-23 19:25 vault/VERSION
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-23 19:25 vault/__init__.py
+-rw-r--r--  2.0 unx      114 b- defN 23-Apr-23 19:25 vault/__version__.py
+-rw-r--r--  2.0 unx      396 b- defN 23-Apr-23 19:25 vault/v1.py
+-rw-r--r--  2.0 unx     1095 b- defN 23-Apr-23 19:25 vault/v2.py
+-rw-r--r--  2.0 unx     1500 b- defN 23-Apr-23 19:25 vault/vault.py
+-rw-r--r--  2.0 unx      771 b- defN 23-Apr-23 19:25 vault/vault_base.py
+-rw-r--r--  2.0 unx      741 b- defN 23-Apr-23 19:26 cnd_vault-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-23 19:26 cnd_vault-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-Apr-23 19:26 cnd_vault-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      800 b- defN 23-Apr-23 19:26 cnd_vault-0.1.1.dist-info/RECORD
+11 files, 5612 bytes uncompressed, 2355 bytes compressed:  58.0%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: vault/vault.py
 Comment: 
 
 Filename: vault/vault_base.py
 Comment: 
 
-Filename: cnd_vault-0.1.0.dist-info/METADATA
+Filename: cnd_vault-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: cnd_vault-0.1.0.dist-info/WHEEL
+Filename: cnd_vault-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: cnd_vault-0.1.0.dist-info/top_level.txt
+Filename: cnd_vault-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: cnd_vault-0.1.0.dist-info/RECORD
+Filename: cnd_vault-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vault/VERSION

```diff
@@ -1 +1 @@
-0.1.0
+0.1.1
```

## Comparing `cnd_vault-0.1.0.dist-info/METADATA` & `cnd_vault-0.1.1.dist-info/METADATA`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,25 @@
 Metadata-Version: 2.1
 Name: cnd-vault
-Version: 0.1.0
+Version: 0.1.1
 Summary: Tools to read/write secret
 Home-page: https://gitlab.com/changendevops/cnd-vault
 Author: Denis FABIEN
 Author-email: denis.fabien@changendevops.com
 License: MIT/X11
 Project-URL: Documentation, https://changendevops.com
 Project-URL: Source, https://gitlab.com/changendevops/cnd-vault
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Requires-Dist: clint
-Requires-Dist: coverage
+Requires-Dist: mockito
+Requires-Dist: mamba
+Requires-Dist: expects
+Requires-Dist: cndprint
+Requires-Dist: pyyaml
+Requires-Dist: requests
+Requires-Dist: twine
+Requires-Dist: CndIO
+Requires-Dist: cnd-scaffold (>=2.2.1)
+Requires-Dist: CndIo
+Requires-Dist: hvac
```

