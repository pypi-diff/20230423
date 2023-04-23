# Comparing `tmp/mvclib-0.5.9.tar.gz` & `tmp/mvclib-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mvclib-0.5.9.tar", last modified: Thu Jan 19 17:14:47 2023, max compression
+gzip compressed data, was "mvclib-0.6.0.tar", last modified: Sun Apr 23 16:43:05 2023, max compression
```

## Comparing `mvclib-0.5.9.tar` & `mvclib-0.6.0.tar`

### file list

```diff
@@ -1,44 +1,56 @@
-drwxr-xr-x   0 aaron67    (501) staff       (20)        0 2023-01-19 17:14:47.151474 mvclib-0.5.9/
--rw-r--r--   0 aaron67    (501) staff       (20)     1069 2022-04-01 08:37:18.000000 mvclib-0.5.9/LICENSE
--rw-r--r--   0 aaron67    (501) staff       (20)     1449 2023-01-19 17:14:47.151572 mvclib-0.5.9/PKG-INFO
--rw-r--r--   0 aaron67    (501) staff       (20)      689 2022-04-13 14:06:28.000000 mvclib-0.5.9/README.md
-drwxr-xr-x   0 aaron67    (501) staff       (20)        0 2023-01-19 17:14:47.145138 mvclib-0.5.9/mvclib/
--rw-r--r--   0 aaron67    (501) staff       (20)      263 2023-01-19 17:13:52.000000 mvclib-0.5.9/mvclib/__init__.py
--rw-r--r--   0 aaron67    (501) staff       (20)      934 2022-01-20 12:33:26.000000 mvclib-0.5.9/mvclib/aes.py
--rw-r--r--   0 aaron67    (501) staff       (20)     1529 2022-02-05 05:13:48.000000 mvclib-0.5.9/mvclib/base58.py
--rw-r--r--   0 aaron67    (501) staff       (20)     6778 2022-11-19 19:16:03.000000 mvclib-0.5.9/mvclib/constants.py
--rw-r--r--   0 aaron67    (501) staff       (20)     2509 2022-01-28 20:24:48.000000 mvclib-0.5.9/mvclib/curve.py
--rw-r--r--   0 aaron67    (501) staff       (20)      371 2022-12-03 18:42:31.000000 mvclib-0.5.9/mvclib/hash.py
-drwxr-xr-x   0 aaron67    (501) staff       (20)        0 2023-01-19 17:14:47.147034 mvclib-0.5.9/mvclib/hd/
--rw-r--r--   0 aaron67    (501) staff       (20)      266 2022-11-12 13:31:42.000000 mvclib-0.5.9/mvclib/hd/__init__.py
--rw-r--r--   0 aaron67    (501) staff       (20)     7023 2022-11-25 14:59:02.000000 mvclib-0.5.9/mvclib/hd/bip32.py
--rw-r--r--   0 aaron67    (501) staff       (20)     4015 2022-11-17 13:39:56.000000 mvclib-0.5.9/mvclib/hd/bip39.py
--rw-r--r--   0 aaron67    (501) staff       (20)     1542 2022-11-17 13:40:23.000000 mvclib-0.5.9/mvclib/hd/bip44.py
-drwxr-xr-x   0 aaron67    (501) staff       (20)        0 2023-01-19 17:14:47.147744 mvclib-0.5.9/mvclib/hd/wordlist/
--rw-r--r--   0 aaron67    (501) staff       (20)     8192 2022-01-24 22:27:44.000000 mvclib-0.5.9/mvclib/hd/wordlist/chinese_simplified.txt
--rw-r--r--   0 aaron67    (501) staff       (20)    15164 2022-01-24 22:27:44.000000 mvclib-0.5.9/mvclib/hd/wordlist/english.txt
--rw-r--r--   0 aaron67    (501) staff       (20)    13780 2022-11-25 14:59:11.000000 mvclib-0.5.9/mvclib/keys.py
-drwxr-xr-x   0 aaron67    (501) staff       (20)        0 2023-01-19 17:14:47.148745 mvclib-0.5.9/mvclib/script/
--rw-r--r--   0 aaron67    (501) staff       (20)      152 2022-02-05 07:20:08.000000 mvclib-0.5.9/mvclib/script/__init__.py
--rw-r--r--   0 aaron67    (501) staff       (20)     1275 2022-11-25 14:59:16.000000 mvclib-0.5.9/mvclib/script/script.py
--rw-r--r--   0 aaron67    (501) staff       (20)     7307 2023-01-19 17:13:27.000000 mvclib-0.5.9/mvclib/script/type.py
-drwxr-xr-x   0 aaron67    (501) staff       (20)        0 2023-01-19 17:14:47.149709 mvclib-0.5.9/mvclib/service/
--rw-r--r--   0 aaron67    (501) staff       (20)      104 2022-09-30 15:54:30.000000 mvclib-0.5.9/mvclib/service/__init__.py
--rw-r--r--   0 aaron67    (501) staff       (20)     5594 2022-12-01 22:17:08.000000 mvclib-0.5.9/mvclib/service/metasv.py
--rw-r--r--   0 aaron67    (501) staff       (20)     2493 2022-11-19 19:28:50.000000 mvclib-0.5.9/mvclib/service/provider.py
--rw-r--r--   0 aaron67    (501) staff       (20)     1264 2022-11-22 07:40:49.000000 mvclib-0.5.9/mvclib/service/service.py
-drwxr-xr-x   0 aaron67    (501) staff       (20)        0 2023-01-19 17:14:47.151075 mvclib-0.5.9/mvclib/transaction/
--rw-r--r--   0 aaron67    (501) staff       (20)      124 2022-04-01 14:30:40.000000 mvclib-0.5.9/mvclib/transaction/__init__.py
--rw-r--r--   0 aaron67    (501) staff       (20)    20078 2023-01-19 17:02:30.000000 mvclib-0.5.9/mvclib/transaction/transaction.py
--rw-r--r--   0 aaron67    (501) staff       (20)     2802 2022-10-28 12:42:46.000000 mvclib-0.5.9/mvclib/transaction/unspent.py
--rw-r--r--   0 aaron67    (501) staff       (20)     9663 2022-12-05 23:08:59.000000 mvclib-0.5.9/mvclib/utils.py
--rw-r--r--   0 aaron67    (501) staff       (20)     8737 2022-11-22 07:40:49.000000 mvclib-0.5.9/mvclib/wallet.py
-drwxr-xr-x   0 aaron67    (501) staff       (20)        0 2023-01-19 17:14:47.145990 mvclib-0.5.9/mvclib.egg-info/
--rw-r--r--   0 aaron67    (501) staff       (20)     1449 2023-01-19 17:14:47.000000 mvclib-0.5.9/mvclib.egg-info/PKG-INFO
--rw-r--r--   0 aaron67    (501) staff       (20)      773 2023-01-19 17:14:47.000000 mvclib-0.5.9/mvclib.egg-info/SOURCES.txt
--rw-r--r--   0 aaron67    (501) staff       (20)        1 2023-01-19 17:14:47.000000 mvclib-0.5.9/mvclib.egg-info/dependency_links.txt
--rw-r--r--   0 aaron67    (501) staff       (20)       51 2023-01-19 17:14:47.000000 mvclib-0.5.9/mvclib.egg-info/requires.txt
--rw-r--r--   0 aaron67    (501) staff       (20)        7 2023-01-19 17:14:47.000000 mvclib-0.5.9/mvclib.egg-info/top_level.txt
--rw-r--r--   0 aaron67    (501) staff       (20)      104 2022-01-13 03:23:06.000000 mvclib-0.5.9/pyproject.toml
--rw-r--r--   0 aaron67    (501) staff       (20)      920 2023-01-19 17:14:47.152611 mvclib-0.5.9/setup.cfg
--rw-r--r--   0 aaron67    (501) staff       (20)      318 2022-04-01 08:19:30.000000 mvclib-0.5.9/setup.py
+drwxr-xr-x   0 aaron67    (501) staff       (20)        0 2023-04-23 16:43:05.763127 mvclib-0.6.0/
+-rw-r--r--   0 aaron67    (501) staff       (20)     1069 2022-04-01 08:37:18.000000 mvclib-0.6.0/LICENSE
+-rw-r--r--   0 aaron67    (501) staff       (20)     1449 2023-04-23 16:43:05.763214 mvclib-0.6.0/PKG-INFO
+-rw-r--r--   0 aaron67    (501) staff       (20)      689 2022-04-13 14:06:28.000000 mvclib-0.6.0/README.md
+drwxr-xr-x   0 aaron67    (501) staff       (20)        0 2023-04-23 16:43:05.754341 mvclib-0.6.0/mvclib/
+-rw-r--r--   0 aaron67    (501) staff       (20)      263 2023-04-23 16:42:03.000000 mvclib-0.6.0/mvclib/__init__.py
+-rw-r--r--   0 aaron67    (501) staff       (20)      934 2022-01-20 12:33:26.000000 mvclib-0.6.0/mvclib/aes.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     1529 2022-02-05 05:13:48.000000 mvclib-0.6.0/mvclib/base58.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     6777 2023-04-23 16:31:43.000000 mvclib-0.6.0/mvclib/constants.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     2509 2022-01-28 20:24:48.000000 mvclib-0.6.0/mvclib/curve.py
+-rw-r--r--   0 aaron67    (501) staff       (20)      371 2022-12-03 18:42:31.000000 mvclib-0.6.0/mvclib/hash.py
+drwxr-xr-x   0 aaron67    (501) staff       (20)        0 2023-04-23 16:43:05.756203 mvclib-0.6.0/mvclib/hd/
+-rw-r--r--   0 aaron67    (501) staff       (20)      266 2022-11-12 13:31:42.000000 mvclib-0.6.0/mvclib/hd/__init__.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     7023 2023-04-23 16:37:21.000000 mvclib-0.6.0/mvclib/hd/bip32.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     4015 2022-11-17 13:39:56.000000 mvclib-0.6.0/mvclib/hd/bip39.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     1542 2022-11-17 13:40:23.000000 mvclib-0.6.0/mvclib/hd/bip44.py
+drwxr-xr-x   0 aaron67    (501) staff       (20)        0 2023-04-23 16:43:05.756831 mvclib-0.6.0/mvclib/hd/wordlist/
+-rw-r--r--   0 aaron67    (501) staff       (20)     8192 2022-01-24 22:27:44.000000 mvclib-0.6.0/mvclib/hd/wordlist/chinese_simplified.txt
+-rw-r--r--   0 aaron67    (501) staff       (20)    15164 2022-01-24 22:27:44.000000 mvclib-0.6.0/mvclib/hd/wordlist/english.txt
+-rw-r--r--   0 aaron67    (501) staff       (20)    13780 2022-11-25 14:59:11.000000 mvclib-0.6.0/mvclib/keys.py
+drwxr-xr-x   0 aaron67    (501) staff       (20)        0 2023-04-23 16:43:05.757692 mvclib-0.6.0/mvclib/script/
+-rw-r--r--   0 aaron67    (501) staff       (20)      152 2022-02-05 07:20:08.000000 mvclib-0.6.0/mvclib/script/__init__.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     1275 2022-11-25 14:59:16.000000 mvclib-0.6.0/mvclib/script/script.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     7307 2023-01-19 20:10:34.000000 mvclib-0.6.0/mvclib/script/type.py
+drwxr-xr-x   0 aaron67    (501) staff       (20)        0 2023-04-23 16:43:05.758889 mvclib-0.6.0/mvclib/service/
+-rw-r--r--   0 aaron67    (501) staff       (20)      104 2023-04-23 16:29:27.000000 mvclib-0.6.0/mvclib/service/__init__.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     5643 2023-04-23 16:34:36.000000 mvclib-0.6.0/mvclib/service/mvcapi.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     2493 2022-11-19 19:28:50.000000 mvclib-0.6.0/mvclib/service/provider.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     1264 2023-04-23 16:29:27.000000 mvclib-0.6.0/mvclib/service/service.py
+drwxr-xr-x   0 aaron67    (501) staff       (20)        0 2023-04-23 16:43:05.759901 mvclib-0.6.0/mvclib/transaction/
+-rw-r--r--   0 aaron67    (501) staff       (20)      124 2022-04-01 14:30:40.000000 mvclib-0.6.0/mvclib/transaction/__init__.py
+-rw-r--r--   0 aaron67    (501) staff       (20)    20078 2023-01-19 17:02:30.000000 mvclib-0.6.0/mvclib/transaction/transaction.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     2802 2022-10-28 12:42:46.000000 mvclib-0.6.0/mvclib/transaction/unspent.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     9663 2022-12-05 23:08:59.000000 mvclib-0.6.0/mvclib/utils.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     8737 2023-04-23 16:29:27.000000 mvclib-0.6.0/mvclib/wallet.py
+drwxr-xr-x   0 aaron67    (501) staff       (20)        0 2023-04-23 16:43:05.755283 mvclib-0.6.0/mvclib.egg-info/
+-rw-r--r--   0 aaron67    (501) staff       (20)     1449 2023-04-23 16:43:05.000000 mvclib-0.6.0/mvclib.egg-info/PKG-INFO
+-rw-r--r--   0 aaron67    (501) staff       (20)      997 2023-04-23 16:43:05.000000 mvclib-0.6.0/mvclib.egg-info/SOURCES.txt
+-rw-r--r--   0 aaron67    (501) staff       (20)        1 2023-04-23 16:43:05.000000 mvclib-0.6.0/mvclib.egg-info/dependency_links.txt
+-rw-r--r--   0 aaron67    (501) staff       (20)       51 2023-04-23 16:43:05.000000 mvclib-0.6.0/mvclib.egg-info/requires.txt
+-rw-r--r--   0 aaron67    (501) staff       (20)        7 2023-04-23 16:43:05.000000 mvclib-0.6.0/mvclib.egg-info/top_level.txt
+-rw-r--r--   0 aaron67    (501) staff       (20)      104 2022-01-13 03:23:06.000000 mvclib-0.6.0/pyproject.toml
+-rw-r--r--   0 aaron67    (501) staff       (20)      920 2023-04-23 16:43:05.763620 mvclib-0.6.0/setup.cfg
+-rw-r--r--   0 aaron67    (501) staff       (20)      318 2022-04-01 08:19:30.000000 mvclib-0.6.0/setup.py
+drwxr-xr-x   0 aaron67    (501) staff       (20)        0 2023-04-23 16:43:05.762907 mvclib-0.6.0/tests/
+-rw-r--r--   0 aaron67    (501) staff       (20)     1411 2022-04-01 13:27:38.000000 mvclib-0.6.0/tests/test_aes.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     1166 2022-04-01 13:27:38.000000 mvclib-0.6.0/tests/test_base58.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     2328 2022-04-01 13:27:38.000000 mvclib-0.6.0/tests/test_curve.py
+-rw-r--r--   0 aaron67    (501) staff       (20)      532 2022-04-01 13:27:38.000000 mvclib-0.6.0/tests/test_hash.py
+-rw-r--r--   0 aaron67    (501) staff       (20)    10082 2022-11-17 13:44:20.000000 mvclib-0.6.0/tests/test_hd.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     7170 2022-04-01 13:27:38.000000 mvclib-0.6.0/tests/test_keys.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     3624 2022-12-05 23:08:59.000000 mvclib-0.6.0/tests/test_script.py
+-rw-r--r--   0 aaron67    (501) staff       (20)      442 2023-04-23 16:30:25.000000 mvclib-0.6.0/tests/test_service.py
+-rw-r--r--   0 aaron67    (501) staff       (20)    12015 2023-04-23 16:29:27.000000 mvclib-0.6.0/tests/test_transaction.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     9817 2022-12-05 23:08:59.000000 mvclib-0.6.0/tests/test_utils.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     1489 2023-04-23 16:29:27.000000 mvclib-0.6.0/tests/test_wallet.py
```

### Comparing `mvclib-0.5.9/LICENSE` & `mvclib-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mvclib-0.5.9/PKG-INFO` & `mvclib-0.6.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mvclib
-Version: 0.5.9
+Version: 0.6.0
 Home-page: https://github.com/MetaverseChain/mvc-lib-py
 Author: aaron67
 Author-email: aaron67@aaron67.cc
 Project-URL: Bug Tracker, https://github.com/MetaverseChain/mvc-lib-py/issues
 Keywords: cryptocurrency,payments,tools,wallet
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `mvclib-0.5.9/README.md` & `mvclib-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `mvclib-0.5.9/mvclib/aes.py` & `mvclib-0.6.0/mvclib/aes.py`

 * *Files identical despite different names*

### Comparing `mvclib-0.5.9/mvclib/base58.py` & `mvclib-0.6.0/mvclib/base58.py`

 * *Files identical despite different names*

### Comparing `mvclib-0.5.9/mvclib/constants.py` & `mvclib-0.6.0/mvclib/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 from typing import Dict, List, Optional
 
 TRANSACTION_SEQUENCE: int = int(os.getenv('MVCLIB_TRANSACTION_SEQUENCE') or 0xffffffff)
 TRANSACTION_VERSION: int = int(os.getenv('MVCLIB_TRANSACTION_VERSION') or 1)
 TRANSACTION_LOCKTIME: int = int(os.getenv('MVCLIB_TRANSACTION_LOCKTIME') or 0)
 TRANSACTION_FEE_RATE: float = float(os.getenv('MVCLIB_TRANSACTION_FEE_RATE') or 1)  # satoshi per byte
 P2PKH_DUST_LIMIT: int = int(os.getenv('MVCLIB_P2PKH_DUST_LIMIT') or 135)
-HTTP_REQUEST_TIMEOUT: int = int(os.getenv('MVCLIB_HTTP_REQUEST_TIMEOUT') or 30)
+HTTP_REQUEST_TIMEOUT: int = int(os.getenv('MVCLIB_HTTP_REQUEST_TIMEOUT') or 3)
 THREAD_POOL_MAX_EXECUTORS: int = int(os.getenv('MVCLIB_THREAD_POOL_MAX_EXECUTORS') or 10)
 BIP39_ENTROPY_BIT_LENGTH: int = int(os.getenv('MVCLIB_BIP39_ENTROPY_BIT_LENGTH') or 128)
 BIP44_DERIVATION_PATH = os.getenv('MVCLIB_BIP44_DERIVATION_PATH') or "m/44'/10001'/0'"
-METASV_TOKEN: Optional[str] = os.getenv('MVCLIB_METASV_TOKEN') or os.getenv('METASV_TOKEN')
-METASV_CLIENT_KEY: Optional[str] = os.getenv('MVCLIB_METASV_CLIENT_KEY') or os.getenv('METASV_CLIENT_KEY')
+MVCAPI_TOKEN: Optional[str] = os.getenv('MVCLIB_MVCAPI_TOKEN') or os.getenv('MVCAPI_TOKEN')
+MVCAPI_CLIENT_KEY: Optional[str] = os.getenv('MVCLIB_MVCAPI_CLIENT_KEY') or os.getenv('MVCAPI_CLIENT_KEY')
 
 
 class Chain(str, Enum):
     MAIN = 'main'
     TEST = 'test'
```

### Comparing `mvclib-0.5.9/mvclib/curve.py` & `mvclib-0.6.0/mvclib/curve.py`

 * *Files identical despite different names*

### Comparing `mvclib-0.5.9/mvclib/hd/bip32.py` & `mvclib-0.6.0/mvclib/hd/bip32.py`

 * *Files identical despite different names*

### Comparing `mvclib-0.5.9/mvclib/hd/bip39.py` & `mvclib-0.6.0/mvclib/hd/bip39.py`

 * *Files identical despite different names*

### Comparing `mvclib-0.5.9/mvclib/hd/bip44.py` & `mvclib-0.6.0/mvclib/hd/bip44.py`

 * *Files identical despite different names*

### Comparing `mvclib-0.5.9/mvclib/hd/wordlist/chinese_simplified.txt` & `mvclib-0.6.0/mvclib/hd/wordlist/chinese_simplified.txt`

 * *Files identical despite different names*

### Comparing `mvclib-0.5.9/mvclib/hd/wordlist/english.txt` & `mvclib-0.6.0/mvclib/hd/wordlist/english.txt`

 * *Files identical despite different names*

### Comparing `mvclib-0.5.9/mvclib/keys.py` & `mvclib-0.6.0/mvclib/keys.py`

 * *Files identical despite different names*

### Comparing `mvclib-0.5.9/mvclib/script/script.py` & `mvclib-0.6.0/mvclib/script/script.py`

 * *Files identical despite different names*

### Comparing `mvclib-0.5.9/mvclib/script/type.py` & `mvclib-0.6.0/mvclib/script/type.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,11 +185,11 @@
         script: bytes = OP.OP_0
         for signature in signatures:
             script += encode_pushdata(signature + sighash.to_bytes(1, 'little'))
         return Script(script)
 
     @classmethod
     def estimated_unlocking_byte_length(cls, **kwargs) -> int:  # pragma: no cover
-        if not kwargs.get('group_size') and not kwargs.get('private_keys'):
-            raise ValueError(f"can't estimate unlocking byte length without group size")
-        group_size = kwargs.get('group_size') if kwargs.get('group_size') else len(kwargs.get('private_keys'))
-        return 1 + 73 * group_size
+        if not kwargs.get('threshold') and not kwargs.get('private_keys'):
+            raise ValueError(f"can't estimate unlocking byte length without threshold value")
+        threshold = kwargs.get('threshold') if kwargs.get('threshold') else len(kwargs.get('private_keys'))
+        return 1 + 73 * threshold
```

### Comparing `mvclib-0.5.9/mvclib/service/metasv.py` & `mvclib-0.6.0/mvclib/service/mvcapi.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,29 +4,32 @@
 import time
 from contextlib import suppress
 from typing import Optional, List, Dict, Union, Tuple
 
 import requests
 
 from .provider import Provider, BroadcastResult
-from ..constants import Chain, METASV_TOKEN, METASV_CLIENT_KEY
+from ..constants import Chain, MVCAPI_TOKEN, MVCAPI_CLIENT_KEY
 from ..hash import sha256
 from ..hd import Xprv, Xpub
 from ..keys import Key
 
 
-class MetaSV(Provider):  # pragma: no cover
+class MvcApi(Provider):  # pragma: no cover
 
     def __init__(self, chain: Chain = Chain.MAIN, url: Optional[str] = None, headers: Optional[Dict] = None,
                  timeout: Optional[int] = None, token: Optional[str] = None, client_key: Optional[str] = None):
-        assert chain == Chain.TEST, 'MetaSV service now only supports Chain.TEST'
-        self.url = url or 'https://api-mvc-testnet.metasv.com'
+        if chain == Chain.MAIN:
+            default_url = 'https://mainnet.mvcapi.com'
+        else:
+            default_url = 'https://testnet.mvcapi.com'
+        self.url = url or default_url
         super().__init__(chain, headers, timeout)
-        self.token = token or METASV_TOKEN
-        self.client_key = client_key or METASV_CLIENT_KEY
+        self.token = token or MVCAPI_TOKEN
+        self.client_key = client_key or MVCAPI_CLIENT_KEY
 
     def _get_unspents(self, address: str, flag: Optional[str] = None) -> Union[Dict, List[Dict]]:
         with suppress(Exception):
             params = {}
             if flag:
                 params['flag'] = flag
             return self.get(url=f'{self.url}/address/{address}/utxo', params=params)
@@ -101,17 +104,17 @@
         try to parse out (xpub, xprv) from kwargs
         """
         xprv: Xprv = kwargs.get('xprv') or None
         xpub: Xpub = kwargs.get('xpub') or (xprv.xpub() if xprv else None)
         return xpub, xprv
 
     def get_xpub_unspents(self, **kwargs) -> List[Dict]:
-        assert self.token or self.client_key, 'MetaSV service requires a token or a client key'
+        assert self.token or self.client_key, 'MVCAPI service requires a token or a client key'
         try:
-            xpub, xprv = MetaSV._parse_xkey(**kwargs)
+            xpub, xprv = MvcApi._parse_xkey(**kwargs)
             path = f'/xpubLite/{xpub}/utxo'
             r: Dict = self.get(url=f'{self.url}{path}', headers=self.parse_headers(path))
             unspents: List[Dict] = []
             for item in r:
                 unspent = {'vout': item['txIndex'], 'satoshi': item['value']}
                 if xprv:
                     # update private key
@@ -120,17 +123,17 @@
             return unspents
         except Exception as e:
             if kwargs.get('throw'):
                 raise e
         return []
 
     def get_xpub_balance(self, **kwargs) -> int:
-        assert self.token or self.client_key, 'MetaSV service requires a token or a client key'
+        assert self.token or self.client_key, 'MVCAPI service requires a token or a client key'
         try:
-            xpub, xprv = MetaSV._parse_xkey(**kwargs)
+            xpub, xprv = MvcApi._parse_xkey(**kwargs)
             path = f'/xpubLite/{xpub}/balance'
             r: Dict = self.get(url=f'{self.url}{path}', headers=self.parse_headers(path))
             return r.get('balance')
         except Exception as e:
             if kwargs.get('throw'):
                 raise e
         return 0
```

### Comparing `mvclib-0.5.9/mvclib/service/provider.py` & `mvclib-0.6.0/mvclib/service/provider.py`

 * *Files identical despite different names*

### Comparing `mvclib-0.5.9/mvclib/service/service.py` & `mvclib-0.6.0/mvclib/service/service.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from typing import List, Dict, Optional
 
-from .metasv import MetaSV
+from .mvcapi import MvcApi
 from .provider import Provider, BroadcastResult
 from ..constants import Chain
 
 
 class Service:
 
     def __init__(self, chain: Optional[Chain] = None, provider: Optional[Provider] = None):
         if provider:
             self.provider = provider
         else:
             chain = chain or Chain.MAIN
-            self.provider = MetaSV(chain=chain)
+            self.provider = MvcApi(chain=chain)
         self.chain = self.provider.chain
 
     def get_unspents(self, **kwargs) -> List[Dict]:
         """kwargs will pass the following at least
         {
             'private_keys': List[mvclib.keys.PrivateKey],
         }
```

### Comparing `mvclib-0.5.9/mvclib/transaction/transaction.py` & `mvclib-0.6.0/mvclib/transaction/transaction.py`

 * *Files identical despite different names*

### Comparing `mvclib-0.5.9/mvclib/transaction/unspent.py` & `mvclib-0.6.0/mvclib/transaction/unspent.py`

 * *Files identical despite different names*

### Comparing `mvclib-0.5.9/mvclib/utils.py` & `mvclib-0.6.0/mvclib/utils.py`

 * *Files identical despite different names*

### Comparing `mvclib-0.5.9/mvclib/wallet.py` & `mvclib-0.6.0/mvclib/wallet.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from itertools import repeat
 from typing import Optional, List, Tuple, Union, Dict, Any
 
 from .constants import Chain, THREAD_POOL_MAX_EXECUTORS
 from .hd import Xprv
 from .keys import PrivateKey
 from .service.provider import Provider
-from .service.service import Service, MetaSV
+from .service.service import Service, MvcApi
 from .transaction.transaction import Transaction, TxOutput, InsufficientFunds
 from .transaction.unspent import Unspent
 
 
 def get_unspents_wrapper(chain: Chain, provider: Provider, d: Dict) -> List['Unspent']:
     return Unspent.get_unspents(chain, provider, **d)
 
@@ -132,15 +132,15 @@
 
 
 class WalletLite:  # pragma: no cover
     def __init__(self, xprv: Union[Xprv, str, bytes], **kwargs):
         self.xprv = xprv if type(xprv) is Xprv else Xprv(xprv)
         assert self.xprv, 'bad xprv'
         self.chain: Chain = self.xprv.chain
-        self.provider: MetaSV = MetaSV(chain=self.chain, **kwargs)
+        self.provider: MvcApi = MvcApi(chain=self.chain, **kwargs)
         self.unspents: List[Unspent] = []
         self.kwargs: Dict[str, Any] = dict(**kwargs) or {}
 
     def get_unspents(self, refresh: bool = False, **kwargs) -> List[Unspent]:
         if refresh:
             unspents = self.provider.get_xpub_unspents(xprv=self.xprv, **{**self.kwargs, **kwargs})
             self.unspents = [Unspent(**unspent) for unspent in unspents]
```

### Comparing `mvclib-0.5.9/mvclib.egg-info/PKG-INFO` & `mvclib-0.6.0/mvclib.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mvclib
-Version: 0.5.9
+Version: 0.6.0
 Home-page: https://github.com/MetaverseChain/mvc-lib-py
 Author: aaron67
 Author-email: aaron67@aaron67.cc
 Project-URL: Bug Tracker, https://github.com/MetaverseChain/mvc-lib-py/issues
 Keywords: cryptocurrency,payments,tools,wallet
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `mvclib-0.5.9/setup.cfg` & `mvclib-0.6.0/setup.cfg`

 * *Files identical despite different names*

