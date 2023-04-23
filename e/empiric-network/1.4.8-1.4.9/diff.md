# Comparing `tmp/empiric_network-1.4.8.tar.gz` & `tmp/empiric_network-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "empiric_network-1.4.8.tar", max compression
+gzip compressed data, was "empiric_network-1.4.9.tar", max compression
```

## Comparing `empiric_network-1.4.8.tar` & `empiric_network-1.4.9.tar`

### file list

```diff
@@ -1,61 +1,62 @@
--rw-r--r--   0        0        0      284 2023-01-25 21:43:54.197892 empiric_network-1.4.8/README.md
--rw-r--r--   0        0        0      204 2023-01-25 21:43:54.197892 empiric_network-1.4.8/empiric/cli/.example.config copy.ini
--rw-r--r--   0        0        0      697 2023-01-25 21:43:54.197892 empiric_network-1.4.8/empiric/cli/README.md
--rw-r--r--   0        0        0      342 2023-01-25 21:43:54.197892 empiric_network-1.4.8/empiric/cli/__init__.py
--rw-r--r--   0        0        0      148 2023-01-25 21:43:54.197892 empiric_network-1.4.8/empiric/cli/__main__.py
--rw-r--r--   0        0        0     1628 2023-01-25 21:43:54.197892 empiric_network-1.4.8/empiric/cli/account.py
--rw-r--r--   0        0        0   544336 2023-01-25 21:43:54.197892 empiric_network-1.4.8/empiric/cli/compiled_account_contract.py
--rw-r--r--   0        0        0     2050 2023-01-25 21:43:54.197892 empiric_network-1.4.8/empiric/cli/config.py
--rw-r--r--   0        0        0     1118 2023-01-25 21:43:54.197892 empiric_network-1.4.8/empiric/cli/contracts/__init__.py
--rw-r--r--   0        0        0     8098 2023-01-25 21:43:54.197892 empiric_network-1.4.8/empiric/cli/contracts/oracle.py
--rw-r--r--   0        0        0     5217 2023-01-25 21:43:54.197892 empiric_network-1.4.8/empiric/cli/contracts/publisher_registry.py
--rw-r--r--   0        0        0     2638 2023-01-25 21:43:54.197892 empiric_network-1.4.8/empiric/cli/contracts/summary_stats.py
--rw-r--r--   0        0        0     3318 2023-01-25 21:43:54.197892 empiric_network-1.4.8/empiric/cli/contracts/utils.py
--rw-r--r--   0        0        0     4080 2023-01-25 21:43:54.197892 empiric_network-1.4.8/empiric/cli/empiric_cli.py
--rw-r--r--   0        0        0     2682 2023-01-25 21:43:54.197892 empiric_network-1.4.8/empiric/cli/net.py
--rw-r--r--   0        0        0     1420 2023-01-25 21:43:54.197892 empiric_network-1.4.8/empiric/cli/publisher/__init__.py
--rw-r--r--   0        0        0    12230 2023-01-25 21:43:54.197892 empiric_network-1.4.8/empiric/cli/randomness/__init__.py
--rw-r--r--   0        0        0    16306 2023-01-25 21:43:54.197892 empiric_network-1.4.8/empiric/cli/randomness/randomness_utils.py
--rw-r--r--   0        0        0     3682 2023-01-25 21:43:54.197892 empiric_network-1.4.8/empiric/cli/randomness/utils.py
--rw-r--r--   0        0        0      547 2023-01-25 21:43:54.197892 empiric_network-1.4.8/empiric/cli/sample_config/oracle_constructor_data.json
--rw-r--r--   0        0        0        0 2023-01-25 21:43:54.197892 empiric_network-1.4.8/empiric/cli/tests/__init__.py
--rw-r--r--   0        0        0      262 2023-01-25 21:43:54.197892 empiric_network-1.4.8/empiric/cli/tests/test_empiric_cli.py
--rw-r--r--   0        0        0      236 2023-01-25 21:43:54.197892 empiric_network-1.4.8/empiric/cli/utils.py
--rw-r--r--   0        0        0      193 2023-01-25 21:43:54.197892 empiric_network-1.4.8/empiric/core/__init__.py
--rw-r--r--   0        0        0      284 2023-01-25 21:43:54.197892 empiric_network-1.4.8/empiric/core/abis/__init__.py
--rw-r--r--   0        0        0    14135 2023-01-25 21:43:54.201892 empiric_network-1.4.8/empiric/core/abis/oracle.py
--rw-r--r--   0        0        0     1436 2023-01-25 21:43:54.201892 empiric_network-1.4.8/empiric/core/abis/proxy.py
--rw-r--r--   0        0        0     3896 2023-01-25 21:43:54.201892 empiric_network-1.4.8/empiric/core/abis/publisher_registry.py
--rw-r--r--   0        0        0     5912 2023-01-25 21:43:54.201892 empiric_network-1.4.8/empiric/core/abis/randomness.py
--rw-r--r--   0        0        0      868 2023-01-25 21:43:54.201892 empiric_network-1.4.8/empiric/core/abis/summary_stats.py
--rw-r--r--   0        0        0     4557 2023-01-25 21:43:54.201892 empiric_network-1.4.8/empiric/core/client.py
--rw-r--r--   0        0        0     2150 2023-01-25 21:43:54.201892 empiric_network-1.4.8/empiric/core/config.py
--rw-r--r--   0        0        0     3801 2023-01-25 21:43:54.201892 empiric_network-1.4.8/empiric/core/contract.py
--rw-r--r--   0        0        0     8936 2023-01-25 21:43:54.201892 empiric_network-1.4.8/empiric/core/entry.py
--rw-r--r--   0        0        0      387 2023-01-25 21:43:54.201892 empiric_network-1.4.8/empiric/core/logger.py
--rw-r--r--   0        0        0      295 2023-01-25 21:43:54.201892 empiric_network-1.4.8/empiric/core/mixins/__init__.py
--rw-r--r--   0        0        0     5546 2023-01-25 21:43:54.201892 empiric_network-1.4.8/empiric/core/mixins/evm.py
--rw-r--r--   0        0        0     3074 2023-01-25 21:43:54.201892 empiric_network-1.4.8/empiric/core/mixins/nonce.py
--rw-r--r--   0        0        0     8808 2023-01-25 21:43:54.201892 empiric_network-1.4.8/empiric/core/mixins/oracle.py
--rw-r--r--   0        0        0     2287 2023-01-25 21:43:54.201892 empiric_network-1.4.8/empiric/core/mixins/publisher_registry.py
--rw-r--r--   0        0        0     3065 2023-01-25 21:43:54.201892 empiric_network-1.4.8/empiric/core/mixins/randomness.py
--rw-r--r--   0        0        0      669 2023-01-25 21:43:54.201892 empiric_network-1.4.8/empiric/core/mixins/transactions.py
--rw-r--r--   0        0        0     2913 2023-01-25 21:43:54.201892 empiric_network-1.4.8/empiric/core/types.py
--rw-r--r--   0        0        0      880 2023-01-25 21:43:54.201892 empiric_network-1.4.8/empiric/core/utils.py
--rw-r--r--   0        0        0       82 2023-01-25 21:43:54.201892 empiric_network-1.4.8/empiric/publisher/__init__.py
--rw-r--r--   0        0        0     2716 2023-01-25 21:43:54.201892 empiric_network-1.4.8/empiric/publisher/assets.py
--rw-r--r--   0        0        0     2261 2023-01-25 21:43:54.201892 empiric_network-1.4.8/empiric/publisher/client.py
--rw-r--r--   0        0        0      282 2023-01-25 21:43:54.201892 empiric_network-1.4.8/empiric/publisher/fetchers/__init__.py
--rw-r--r--   0        0        0     3747 2023-01-25 21:43:54.201892 empiric_network-1.4.8/empiric/publisher/fetchers/ascendex.py
--rw-r--r--   0        0        0     3017 2023-01-25 21:43:54.201892 empiric_network-1.4.8/empiric/publisher/fetchers/bitstamp.py
--rw-r--r--   0        0        0     3380 2023-01-25 21:43:54.201892 empiric_network-1.4.8/empiric/publisher/fetchers/cex.py
--rw-r--r--   0        0        0     2953 2023-01-25 21:43:54.201892 empiric_network-1.4.8/empiric/publisher/fetchers/coinbase.py
--rw-r--r--   0        0        0     3980 2023-01-25 21:43:54.201892 empiric_network-1.4.8/empiric/publisher/fetchers/coingecko.py
--rw-r--r--   0        0        0     3814 2023-01-25 21:43:54.201892 empiric_network-1.4.8/empiric/publisher/fetchers/gemini.py
--rw-r--r--   0        0        0     3631 2023-01-25 21:43:54.201892 empiric_network-1.4.8/empiric/publisher/fetchers/okx.py
--rw-r--r--   0        0        0     3762 2023-01-25 21:43:54.201892 empiric_network-1.4.8/empiric/publisher/fetchers/thegraph.py
--rw-r--r--   0        0        0      668 2023-01-25 21:43:54.201892 empiric_network-1.4.8/empiric/publisher/types.py
--rw-r--r--   0        0        0     5965 2023-01-25 21:43:54.201892 empiric_network-1.4.8/empiric/test/interface_consistency.py
--rw-r--r--   0        0        0     1000 2023-01-25 21:43:54.201892 empiric_network-1.4.8/pyproject.toml
--rw-r--r--   0        0        0     1545 1970-01-01 00:00:00.000000 empiric_network-1.4.8/setup.py
--rw-r--r--   0        0        0      981 1970-01-01 00:00:00.000000 empiric_network-1.4.8/PKG-INFO
+-rw-r--r--   0        0        0      284 2023-01-29 19:05:27.756261 empiric_network-1.4.9/README.md
+-rw-r--r--   0        0        0      204 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/cli/.example.config copy.ini
+-rw-r--r--   0        0        0      697 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/cli/README.md
+-rw-r--r--   0        0        0      342 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/cli/__init__.py
+-rw-r--r--   0        0        0      148 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/cli/__main__.py
+-rw-r--r--   0        0        0     1628 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/cli/account.py
+-rw-r--r--   0        0        0   544336 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/cli/compiled_account_contract.py
+-rw-r--r--   0        0        0     2050 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/cli/config.py
+-rw-r--r--   0        0        0     1118 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/cli/contracts/__init__.py
+-rw-r--r--   0        0        0     8098 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/cli/contracts/oracle.py
+-rw-r--r--   0        0        0     5217 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/cli/contracts/publisher_registry.py
+-rw-r--r--   0        0        0     2638 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/cli/contracts/summary_stats.py
+-rw-r--r--   0        0        0     3318 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/cli/contracts/utils.py
+-rw-r--r--   0        0        0     4080 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/cli/empiric_cli.py
+-rw-r--r--   0        0        0     2682 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/cli/net.py
+-rw-r--r--   0        0        0     1420 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/cli/publisher/__init__.py
+-rw-r--r--   0        0        0    12230 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/cli/randomness/__init__.py
+-rw-r--r--   0        0        0    16306 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/cli/randomness/randomness_utils.py
+-rw-r--r--   0        0        0     3682 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/cli/randomness/utils.py
+-rw-r--r--   0        0        0      547 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/cli/sample_config/oracle_constructor_data.json
+-rw-r--r--   0        0        0        0 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/cli/tests/__init__.py
+-rw-r--r--   0        0        0      262 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/cli/tests/test_empiric_cli.py
+-rw-r--r--   0        0        0      236 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/cli/utils.py
+-rw-r--r--   0        0        0      193 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/core/__init__.py
+-rw-r--r--   0        0        0      284 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/core/abis/__init__.py
+-rw-r--r--   0        0        0    14135 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/core/abis/oracle.py
+-rw-r--r--   0        0        0     1436 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/core/abis/proxy.py
+-rw-r--r--   0        0        0     3896 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/core/abis/publisher_registry.py
+-rw-r--r--   0        0        0     5912 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/core/abis/randomness.py
+-rw-r--r--   0        0        0      868 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/core/abis/summary_stats.py
+-rw-r--r--   0        0        0     4557 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/core/client.py
+-rw-r--r--   0        0        0     2150 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/core/config.py
+-rw-r--r--   0        0        0     3801 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/core/contract.py
+-rw-r--r--   0        0        0     8936 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/core/entry.py
+-rw-r--r--   0        0        0      387 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/core/logger.py
+-rw-r--r--   0        0        0      295 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/core/mixins/__init__.py
+-rw-r--r--   0        0        0     5546 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/core/mixins/evm.py
+-rw-r--r--   0        0        0     3074 2023-01-29 19:05:27.760261 empiric_network-1.4.9/empiric/core/mixins/nonce.py
+-rw-r--r--   0        0        0     8808 2023-01-29 19:05:27.760261 empiric_network-1.4.9/empiric/core/mixins/oracle.py
+-rw-r--r--   0        0        0     2287 2023-01-29 19:05:27.760261 empiric_network-1.4.9/empiric/core/mixins/publisher_registry.py
+-rw-r--r--   0        0        0     3065 2023-01-29 19:05:27.760261 empiric_network-1.4.9/empiric/core/mixins/randomness.py
+-rw-r--r--   0        0        0      669 2023-01-29 19:05:27.760261 empiric_network-1.4.9/empiric/core/mixins/transactions.py
+-rw-r--r--   0        0        0     2913 2023-01-29 19:05:27.760261 empiric_network-1.4.9/empiric/core/types.py
+-rw-r--r--   0        0        0      880 2023-01-29 19:05:27.760261 empiric_network-1.4.9/empiric/core/utils.py
+-rw-r--r--   0        0        0       82 2023-01-29 19:05:27.760261 empiric_network-1.4.9/empiric/publisher/__init__.py
+-rw-r--r--   0        0        0     2716 2023-01-29 19:05:27.760261 empiric_network-1.4.9/empiric/publisher/assets.py
+-rw-r--r--   0        0        0     2261 2023-01-29 19:05:27.760261 empiric_network-1.4.9/empiric/publisher/client.py
+-rw-r--r--   0        0        0      282 2023-01-29 19:05:27.760261 empiric_network-1.4.9/empiric/publisher/fetchers/__init__.py
+-rw-r--r--   0        0        0     3747 2023-01-29 19:05:27.760261 empiric_network-1.4.9/empiric/publisher/fetchers/ascendex.py
+-rw-r--r--   0        0        0     3017 2023-01-29 19:05:27.760261 empiric_network-1.4.9/empiric/publisher/fetchers/bitstamp.py
+-rw-r--r--   0        0        0     3380 2023-01-29 19:05:27.760261 empiric_network-1.4.9/empiric/publisher/fetchers/cex.py
+-rw-r--r--   0        0        0     2953 2023-01-29 19:05:27.760261 empiric_network-1.4.9/empiric/publisher/fetchers/coinbase.py
+-rw-r--r--   0        0        0     3980 2023-01-29 19:05:27.760261 empiric_network-1.4.9/empiric/publisher/fetchers/coingecko.py
+-rw-r--r--   0        0        0     3814 2023-01-29 19:05:27.760261 empiric_network-1.4.9/empiric/publisher/fetchers/gemini.py
+-rw-r--r--   0        0        0     3631 2023-01-29 19:05:27.760261 empiric_network-1.4.9/empiric/publisher/fetchers/okx.py
+-rw-r--r--   0        0        0     3762 2023-01-29 19:05:27.760261 empiric_network-1.4.9/empiric/publisher/fetchers/thegraph.py
+-rw-r--r--   0        0        0      668 2023-01-29 19:05:27.760261 empiric_network-1.4.9/empiric/publisher/types.py
+-rw-r--r--   0        0        0        0 2023-01-29 19:05:27.760261 empiric_network-1.4.9/empiric/test/__init__.py
+-rw-r--r--   0        0        0     5965 2023-01-29 19:05:27.760261 empiric_network-1.4.9/empiric/test/interface_consistency.py
+-rw-r--r--   0        0        0     1000 2023-01-29 19:05:27.760261 empiric_network-1.4.9/pyproject.toml
+-rw-r--r--   0        0        0     1545 1970-01-01 00:00:00.000000 empiric_network-1.4.9/setup.py
+-rw-r--r--   0        0        0      981 1970-01-01 00:00:00.000000 empiric_network-1.4.9/PKG-INFO
```

### Comparing `empiric_network-1.4.8/empiric/cli/README.md` & `empiric_network-1.4.9/empiric/cli/README.md`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.8/empiric/cli/account.py` & `empiric_network-1.4.9/empiric/cli/account.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.8/empiric/cli/compiled_account_contract.py` & `empiric_network-1.4.9/empiric/cli/compiled_account_contract.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.8/empiric/cli/config.py` & `empiric_network-1.4.9/empiric/cli/config.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.8/empiric/cli/contracts/__init__.py` & `empiric_network-1.4.9/empiric/cli/contracts/__init__.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.8/empiric/cli/contracts/oracle.py` & `empiric_network-1.4.9/empiric/cli/contracts/oracle.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.8/empiric/cli/contracts/publisher_registry.py` & `empiric_network-1.4.9/empiric/cli/contracts/publisher_registry.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.8/empiric/cli/contracts/summary_stats.py` & `empiric_network-1.4.9/empiric/cli/contracts/summary_stats.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.8/empiric/cli/contracts/utils.py` & `empiric_network-1.4.9/empiric/cli/contracts/utils.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.8/empiric/cli/empiric_cli.py` & `empiric_network-1.4.9/empiric/cli/empiric_cli.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.8/empiric/cli/net.py` & `empiric_network-1.4.9/empiric/cli/net.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.8/empiric/cli/publisher/__init__.py` & `empiric_network-1.4.9/empiric/cli/publisher/__init__.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.8/empiric/cli/randomness/__init__.py` & `empiric_network-1.4.9/empiric/cli/randomness/__init__.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.8/empiric/cli/randomness/randomness_utils.py` & `empiric_network-1.4.9/empiric/cli/randomness/randomness_utils.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.8/empiric/cli/randomness/utils.py` & `empiric_network-1.4.9/empiric/cli/randomness/utils.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.8/empiric/cli/sample_config/oracle_constructor_data.json` & `empiric_network-1.4.9/empiric/cli/sample_config/oracle_constructor_data.json`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.8/empiric/core/abis/oracle.py` & `empiric_network-1.4.9/empiric/core/abis/oracle.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.8/empiric/core/abis/proxy.py` & `empiric_network-1.4.9/empiric/core/abis/proxy.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.8/empiric/core/abis/publisher_registry.py` & `empiric_network-1.4.9/empiric/core/abis/publisher_registry.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.8/empiric/core/abis/randomness.py` & `empiric_network-1.4.9/empiric/core/abis/randomness.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.8/empiric/core/abis/summary_stats.py` & `empiric_network-1.4.9/empiric/core/abis/summary_stats.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.8/empiric/core/client.py` & `empiric_network-1.4.9/empiric/core/client.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.8/empiric/core/config.py` & `empiric_network-1.4.9/empiric/core/config.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.8/empiric/core/contract.py` & `empiric_network-1.4.9/empiric/core/contract.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.8/empiric/core/entry.py` & `empiric_network-1.4.9/empiric/core/entry.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.8/empiric/core/mixins/evm.py` & `empiric_network-1.4.9/empiric/core/mixins/evm.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.8/empiric/core/mixins/nonce.py` & `empiric_network-1.4.9/empiric/core/mixins/nonce.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.8/empiric/core/mixins/oracle.py` & `empiric_network-1.4.9/empiric/core/mixins/oracle.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.8/empiric/core/mixins/publisher_registry.py` & `empiric_network-1.4.9/empiric/core/mixins/publisher_registry.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.8/empiric/core/mixins/randomness.py` & `empiric_network-1.4.9/empiric/core/mixins/randomness.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.8/empiric/core/mixins/transactions.py` & `empiric_network-1.4.9/empiric/core/mixins/transactions.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.8/empiric/core/types.py` & `empiric_network-1.4.9/empiric/core/types.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.8/empiric/core/utils.py` & `empiric_network-1.4.9/empiric/core/utils.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.8/empiric/publisher/assets.py` & `empiric_network-1.4.9/empiric/publisher/assets.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.8/empiric/publisher/client.py` & `empiric_network-1.4.9/empiric/publisher/client.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.8/empiric/publisher/fetchers/ascendex.py` & `empiric_network-1.4.9/empiric/publisher/fetchers/ascendex.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.8/empiric/publisher/fetchers/bitstamp.py` & `empiric_network-1.4.9/empiric/publisher/fetchers/bitstamp.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.8/empiric/publisher/fetchers/cex.py` & `empiric_network-1.4.9/empiric/publisher/fetchers/cex.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.8/empiric/publisher/fetchers/coinbase.py` & `empiric_network-1.4.9/empiric/publisher/fetchers/coinbase.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.8/empiric/publisher/fetchers/coingecko.py` & `empiric_network-1.4.9/empiric/publisher/fetchers/coingecko.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.8/empiric/publisher/fetchers/gemini.py` & `empiric_network-1.4.9/empiric/publisher/fetchers/gemini.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.8/empiric/publisher/fetchers/okx.py` & `empiric_network-1.4.9/empiric/publisher/fetchers/okx.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.8/empiric/publisher/fetchers/thegraph.py` & `empiric_network-1.4.9/empiric/publisher/fetchers/thegraph.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.8/empiric/publisher/types.py` & `empiric_network-1.4.9/empiric/publisher/types.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.8/empiric/test/interface_consistency.py` & `empiric_network-1.4.9/empiric/test/interface_consistency.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.8/pyproject.toml` & `empiric_network-1.4.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
 
 [tool.poetry]
 name = "empiric-network"
-version = "1.4.8"
+version = "1.4.9"
 authors = ["Astraly Labs <contact@astraly.xyz>"]
 description = "Core package for rollup-native Empiric Network"
 readme = "README.md"
 homepage = "https://empiric.network"
 repository = "https://github.com/Astraly-Labs/Empiric"
 documentation = "https://docs.empiric.network"
 classifiers = [
```

### Comparing `empiric_network-1.4.8/setup.py` & `empiric_network-1.4.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 ['cairo-lang==0.10.3', 'starknet.py==0.13.0a0', 'typer==0.6.1']
 
 entry_points = \
 {'console_scripts': ['empiric = empiric.cli:main']}
 
 setup_kwargs = {
     'name': 'empiric-network',
-    'version': '1.4.8',
+    'version': '1.4.9',
     'description': 'Core package for rollup-native Empiric Network',
     'long_description': "# Empiric Network\n\n## About\n\nFor more information, see the [project's repository](https://github.com/Astraly-Labs/Empiric), [documentation overview](https://docs.empiric.network/) and [documentation on how to publish data](https://docs.empiric.network/using-empiric/publishing-data).\n",
     'author': 'Astraly Labs',
     'author_email': 'contact@astraly.xyz',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://empiric.network',
```

### Comparing `empiric_network-1.4.8/PKG-INFO` & `empiric_network-1.4.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: empiric-network
-Version: 1.4.8
+Version: 1.4.9
 Summary: Core package for rollup-native Empiric Network
 Home-page: https://empiric.network
 Author: Astraly Labs
 Author-email: contact@astraly.xyz
 Requires-Python: ==3.9.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

