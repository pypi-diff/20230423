# Comparing `tmp/empiric_network-1.5.1.tar.gz` & `tmp/empiric_network-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "empiric_network-1.5.1.tar", max compression
+gzip compressed data, was "empiric_network-1.5.2.tar", max compression
```

## Comparing `empiric_network-1.5.1.tar` & `empiric_network-1.5.2.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0      284 2023-04-23 14:16:06.417535 empiric_network-1.5.1/README.md
--rw-r--r--   0        0        0        0 2023-04-23 14:16:06.417535 empiric_network-1.5.1/empiric/__init__.py
--rw-r--r--   0        0        0      204 2023-04-23 14:16:06.417535 empiric_network-1.5.1/empiric/cli/.example.config copy.ini
--rw-r--r--   0        0        0      697 2023-04-23 14:16:06.417535 empiric_network-1.5.1/empiric/cli/README.md
--rw-r--r--   0        0        0      342 2023-04-23 14:16:06.417535 empiric_network-1.5.1/empiric/cli/__init__.py
--rw-r--r--   0        0        0      148 2023-04-23 14:16:06.417535 empiric_network-1.5.1/empiric/cli/__main__.py
--rw-r--r--   0        0        0     1628 2023-04-23 14:16:06.417535 empiric_network-1.5.1/empiric/cli/account.py
--rw-r--r--   0        0        0   544336 2023-04-23 14:16:06.417535 empiric_network-1.5.1/empiric/cli/compiled_account_contract.py
--rw-r--r--   0        0        0     2050 2023-04-23 14:16:06.417535 empiric_network-1.5.1/empiric/cli/config.py
--rw-r--r--   0        0        0     1118 2023-04-23 14:16:06.417535 empiric_network-1.5.1/empiric/cli/contracts/__init__.py
--rw-r--r--   0        0        0     8098 2023-04-23 14:16:06.417535 empiric_network-1.5.1/empiric/cli/contracts/oracle.py
--rw-r--r--   0        0        0     5217 2023-04-23 14:16:06.417535 empiric_network-1.5.1/empiric/cli/contracts/publisher_registry.py
--rw-r--r--   0        0        0     2638 2023-04-23 14:16:06.417535 empiric_network-1.5.1/empiric/cli/contracts/summary_stats.py
--rw-r--r--   0        0        0     3318 2023-04-23 14:16:06.417535 empiric_network-1.5.1/empiric/cli/contracts/utils.py
--rw-r--r--   0        0        0     4080 2023-04-23 14:16:06.417535 empiric_network-1.5.1/empiric/cli/empiric_cli.py
--rw-r--r--   0        0        0     2682 2023-04-23 14:16:06.417535 empiric_network-1.5.1/empiric/cli/net.py
--rw-r--r--   0        0        0     1420 2023-04-23 14:16:06.417535 empiric_network-1.5.1/empiric/cli/publisher/__init__.py
--rw-r--r--   0        0        0    12230 2023-04-23 14:16:06.417535 empiric_network-1.5.1/empiric/cli/randomness/__init__.py
--rw-r--r--   0        0        0    16306 2023-04-23 14:16:06.417535 empiric_network-1.5.1/empiric/cli/randomness/randomness_utils.py
--rw-r--r--   0        0        0     3682 2023-04-23 14:16:06.417535 empiric_network-1.5.1/empiric/cli/randomness/utils.py
--rw-r--r--   0        0        0      547 2023-04-23 14:16:06.417535 empiric_network-1.5.1/empiric/cli/sample_config/oracle_constructor_data.json
--rw-r--r--   0        0        0        0 2023-04-23 14:16:06.417535 empiric_network-1.5.1/empiric/cli/tests/__init__.py
--rw-r--r--   0        0        0      262 2023-04-23 14:16:06.417535 empiric_network-1.5.1/empiric/cli/tests/test_empiric_cli.py
--rw-r--r--   0        0        0      236 2023-04-23 14:16:06.417535 empiric_network-1.5.1/empiric/cli/utils.py
--rw-r--r--   0        0        0      193 2023-04-23 14:16:06.417535 empiric_network-1.5.1/empiric/core/__init__.py
--rw-r--r--   0        0        0      284 2023-04-23 14:16:06.417535 empiric_network-1.5.1/empiric/core/abis/__init__.py
--rw-r--r--   0        0        0    14135 2023-04-23 14:16:06.417535 empiric_network-1.5.1/empiric/core/abis/oracle.py
--rw-r--r--   0        0        0     1436 2023-04-23 14:16:06.417535 empiric_network-1.5.1/empiric/core/abis/proxy.py
--rw-r--r--   0        0        0     3896 2023-04-23 14:16:06.417535 empiric_network-1.5.1/empiric/core/abis/publisher_registry.py
--rw-r--r--   0        0        0     5912 2023-04-23 14:16:06.417535 empiric_network-1.5.1/empiric/core/abis/randomness.py
--rw-r--r--   0        0        0      868 2023-04-23 14:16:06.417535 empiric_network-1.5.1/empiric/core/abis/summary_stats.py
--rw-r--r--   0        0        0     4557 2023-04-23 14:16:06.417535 empiric_network-1.5.1/empiric/core/client.py
--rw-r--r--   0        0        0     2150 2023-04-23 14:16:06.417535 empiric_network-1.5.1/empiric/core/config.py
--rw-r--r--   0        0        0     3801 2023-04-23 14:16:06.417535 empiric_network-1.5.1/empiric/core/contract.py
--rw-r--r--   0        0        0     9972 2023-04-23 14:16:06.417535 empiric_network-1.5.1/empiric/core/entry.py
--rw-r--r--   0        0        0      387 2023-04-23 14:16:06.417535 empiric_network-1.5.1/empiric/core/logger.py
--rw-r--r--   0        0        0      295 2023-04-23 14:16:06.417535 empiric_network-1.5.1/empiric/core/mixins/__init__.py
--rw-r--r--   0        0        0    25235 2023-04-23 14:16:06.417535 empiric_network-1.5.1/empiric/core/mixins/evm.py
--rw-r--r--   0        0        0     3074 2023-04-23 14:16:06.417535 empiric_network-1.5.1/empiric/core/mixins/nonce.py
--rw-r--r--   0        0        0     8808 2023-04-23 14:16:06.417535 empiric_network-1.5.1/empiric/core/mixins/oracle.py
--rw-r--r--   0        0        0     2287 2023-04-23 14:16:06.417535 empiric_network-1.5.1/empiric/core/mixins/publisher_registry.py
--rw-r--r--   0        0        0     3065 2023-04-23 14:16:06.417535 empiric_network-1.5.1/empiric/core/mixins/randomness.py
--rw-r--r--   0        0        0      669 2023-04-23 14:16:06.417535 empiric_network-1.5.1/empiric/core/mixins/transactions.py
--rw-r--r--   0        0        0     3306 2023-04-23 14:16:06.421535 empiric_network-1.5.1/empiric/core/types.py
--rw-r--r--   0        0        0      880 2023-04-23 14:16:06.421535 empiric_network-1.5.1/empiric/core/utils.py
--rw-r--r--   0        0        0       82 2023-04-23 14:16:06.421535 empiric_network-1.5.1/empiric/publisher/__init__.py
--rw-r--r--   0        0        0     2716 2023-04-23 14:16:06.421535 empiric_network-1.5.1/empiric/publisher/assets.py
--rw-r--r--   0        0        0     2261 2023-04-23 14:16:06.421535 empiric_network-1.5.1/empiric/publisher/client.py
--rw-r--r--   0        0        0      354 2023-04-23 14:16:06.421535 empiric_network-1.5.1/empiric/publisher/fetchers/__init__.py
--rw-r--r--   0        0        0     3755 2023-04-23 14:16:06.421535 empiric_network-1.5.1/empiric/publisher/fetchers/ascendex.py
--rw-r--r--   0        0        0     3017 2023-04-23 14:16:06.421535 empiric_network-1.5.1/empiric/publisher/fetchers/bitstamp.py
--rw-r--r--   0        0        0     3380 2023-04-23 14:16:06.421535 empiric_network-1.5.1/empiric/publisher/fetchers/cex.py
--rw-r--r--   0        0        0     2953 2023-04-23 14:16:06.421535 empiric_network-1.5.1/empiric/publisher/fetchers/coinbase.py
--rw-r--r--   0        0        0     3980 2023-04-23 14:16:06.421535 empiric_network-1.5.1/empiric/publisher/fetchers/coingecko.py
--rw-r--r--   0        0        0     3826 2023-04-23 14:16:06.421535 empiric_network-1.5.1/empiric/publisher/fetchers/defillama.py
--rw-r--r--   0        0        0     3814 2023-04-23 14:16:06.421535 empiric_network-1.5.1/empiric/publisher/fetchers/gemini.py
--rw-r--r--   0        0        0     3754 2023-04-23 14:16:06.421535 empiric_network-1.5.1/empiric/publisher/fetchers/kaiko.py
--rw-r--r--   0        0        0     3631 2023-04-23 14:16:06.421535 empiric_network-1.5.1/empiric/publisher/fetchers/okx.py
--rw-r--r--   0        0        0     3762 2023-04-23 14:16:06.421535 empiric_network-1.5.1/empiric/publisher/fetchers/thegraph.py
--rw-r--r--   0        0        0      668 2023-04-23 14:16:06.421535 empiric_network-1.5.1/empiric/publisher/types.py
--rw-r--r--   0        0        0        0 2023-04-23 14:16:06.421535 empiric_network-1.5.1/empiric/test/__init__.py
--rw-r--r--   0        0        0     5965 2023-04-23 14:16:06.421535 empiric_network-1.5.1/empiric/test/interface_consistency.py
--rw-r--r--   0        0        0     1088 2023-04-23 14:16:06.421535 empiric_network-1.5.1/pyproject.toml
--rw-r--r--   0        0        0     1032 1970-01-01 00:00:00.000000 empiric_network-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0      284 2023-04-23 18:47:52.389966 empiric_network-1.5.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-23 18:47:52.389966 empiric_network-1.5.2/empiric/__init__.py
+-rw-r--r--   0        0        0      204 2023-04-23 18:47:52.389966 empiric_network-1.5.2/empiric/cli/.example.config copy.ini
+-rw-r--r--   0        0        0      697 2023-04-23 18:47:52.389966 empiric_network-1.5.2/empiric/cli/README.md
+-rw-r--r--   0        0        0      342 2023-04-23 18:47:52.389966 empiric_network-1.5.2/empiric/cli/__init__.py
+-rw-r--r--   0        0        0      148 2023-04-23 18:47:52.389966 empiric_network-1.5.2/empiric/cli/__main__.py
+-rw-r--r--   0        0        0     1628 2023-04-23 18:47:52.389966 empiric_network-1.5.2/empiric/cli/account.py
+-rw-r--r--   0        0        0   544336 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/cli/compiled_account_contract.py
+-rw-r--r--   0        0        0     2050 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/cli/config.py
+-rw-r--r--   0        0        0     1118 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/cli/contracts/__init__.py
+-rw-r--r--   0        0        0     8098 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/cli/contracts/oracle.py
+-rw-r--r--   0        0        0     5217 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/cli/contracts/publisher_registry.py
+-rw-r--r--   0        0        0     2638 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/cli/contracts/summary_stats.py
+-rw-r--r--   0        0        0     3318 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/cli/contracts/utils.py
+-rw-r--r--   0        0        0     4080 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/cli/empiric_cli.py
+-rw-r--r--   0        0        0     2682 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/cli/net.py
+-rw-r--r--   0        0        0     1420 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/cli/publisher/__init__.py
+-rw-r--r--   0        0        0    12230 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/cli/randomness/__init__.py
+-rw-r--r--   0        0        0    16306 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/cli/randomness/randomness_utils.py
+-rw-r--r--   0        0        0     3682 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/cli/randomness/utils.py
+-rw-r--r--   0        0        0      547 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/cli/sample_config/oracle_constructor_data.json
+-rw-r--r--   0        0        0        0 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/cli/tests/__init__.py
+-rw-r--r--   0        0        0      262 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/cli/tests/test_empiric_cli.py
+-rw-r--r--   0        0        0      236 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/cli/utils.py
+-rw-r--r--   0        0        0      193 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/core/__init__.py
+-rw-r--r--   0        0        0      284 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/core/abis/__init__.py
+-rw-r--r--   0        0        0    14135 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/core/abis/oracle.py
+-rw-r--r--   0        0        0     1436 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/core/abis/proxy.py
+-rw-r--r--   0        0        0     3896 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/core/abis/publisher_registry.py
+-rw-r--r--   0        0        0     5912 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/core/abis/randomness.py
+-rw-r--r--   0        0        0      868 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/core/abis/summary_stats.py
+-rw-r--r--   0        0        0     4557 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/core/client.py
+-rw-r--r--   0        0        0     2150 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/core/config.py
+-rw-r--r--   0        0        0     3801 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/core/contract.py
+-rw-r--r--   0        0        0     9972 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/core/entry.py
+-rw-r--r--   0        0        0      387 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/core/logger.py
+-rw-r--r--   0        0        0      295 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/core/mixins/__init__.py
+-rw-r--r--   0        0        0    25441 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/core/mixins/evm.py
+-rw-r--r--   0        0        0     3074 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/core/mixins/nonce.py
+-rw-r--r--   0        0        0     8808 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/core/mixins/oracle.py
+-rw-r--r--   0        0        0     2287 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/core/mixins/publisher_registry.py
+-rw-r--r--   0        0        0     3065 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/core/mixins/randomness.py
+-rw-r--r--   0        0        0      669 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/core/mixins/transactions.py
+-rw-r--r--   0        0        0     3306 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/core/types.py
+-rw-r--r--   0        0        0      880 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/core/utils.py
+-rw-r--r--   0        0        0       82 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/publisher/__init__.py
+-rw-r--r--   0        0        0     2716 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/publisher/assets.py
+-rw-r--r--   0        0        0     2261 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/publisher/client.py
+-rw-r--r--   0        0        0      354 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/publisher/fetchers/__init__.py
+-rw-r--r--   0        0        0     3755 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/publisher/fetchers/ascendex.py
+-rw-r--r--   0        0        0     3017 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/publisher/fetchers/bitstamp.py
+-rw-r--r--   0        0        0     3380 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/publisher/fetchers/cex.py
+-rw-r--r--   0        0        0     2953 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/publisher/fetchers/coinbase.py
+-rw-r--r--   0        0        0     3980 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/publisher/fetchers/coingecko.py
+-rw-r--r--   0        0        0     3826 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/publisher/fetchers/defillama.py
+-rw-r--r--   0        0        0     3814 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/publisher/fetchers/gemini.py
+-rw-r--r--   0        0        0     3754 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/publisher/fetchers/kaiko.py
+-rw-r--r--   0        0        0     3631 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/publisher/fetchers/okx.py
+-rw-r--r--   0        0        0     3762 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/publisher/fetchers/thegraph.py
+-rw-r--r--   0        0        0      668 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/publisher/types.py
+-rw-r--r--   0        0        0        0 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/test/__init__.py
+-rw-r--r--   0        0        0     5965 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/test/interface_consistency.py
+-rw-r--r--   0        0        0     1088 2023-04-23 18:47:52.393966 empiric_network-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0     1032 1970-01-01 00:00:00.000000 empiric_network-1.5.2/PKG-INFO
```

### Comparing `empiric_network-1.5.1/empiric/cli/README.md` & `empiric_network-1.5.2/empiric/cli/README.md`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.1/empiric/cli/account.py` & `empiric_network-1.5.2/empiric/cli/account.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.1/empiric/cli/compiled_account_contract.py` & `empiric_network-1.5.2/empiric/cli/compiled_account_contract.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.1/empiric/cli/config.py` & `empiric_network-1.5.2/empiric/cli/config.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.1/empiric/cli/contracts/__init__.py` & `empiric_network-1.5.2/empiric/cli/contracts/__init__.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.1/empiric/cli/contracts/oracle.py` & `empiric_network-1.5.2/empiric/cli/contracts/oracle.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.1/empiric/cli/contracts/publisher_registry.py` & `empiric_network-1.5.2/empiric/cli/contracts/publisher_registry.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.1/empiric/cli/contracts/summary_stats.py` & `empiric_network-1.5.2/empiric/cli/contracts/summary_stats.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.1/empiric/cli/contracts/utils.py` & `empiric_network-1.5.2/empiric/cli/contracts/utils.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.1/empiric/cli/empiric_cli.py` & `empiric_network-1.5.2/empiric/cli/empiric_cli.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.1/empiric/cli/net.py` & `empiric_network-1.5.2/empiric/cli/net.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.1/empiric/cli/publisher/__init__.py` & `empiric_network-1.5.2/empiric/cli/publisher/__init__.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.1/empiric/cli/randomness/__init__.py` & `empiric_network-1.5.2/empiric/cli/randomness/__init__.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.1/empiric/cli/randomness/randomness_utils.py` & `empiric_network-1.5.2/empiric/cli/randomness/randomness_utils.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.1/empiric/cli/randomness/utils.py` & `empiric_network-1.5.2/empiric/cli/randomness/utils.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.1/empiric/cli/sample_config/oracle_constructor_data.json` & `empiric_network-1.5.2/empiric/cli/sample_config/oracle_constructor_data.json`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.1/empiric/core/abis/oracle.py` & `empiric_network-1.5.2/empiric/core/abis/oracle.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.1/empiric/core/abis/proxy.py` & `empiric_network-1.5.2/empiric/core/abis/proxy.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.1/empiric/core/abis/publisher_registry.py` & `empiric_network-1.5.2/empiric/core/abis/publisher_registry.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.1/empiric/core/abis/randomness.py` & `empiric_network-1.5.2/empiric/core/abis/randomness.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.1/empiric/core/abis/summary_stats.py` & `empiric_network-1.5.2/empiric/core/abis/summary_stats.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.1/empiric/core/client.py` & `empiric_network-1.5.2/empiric/core/client.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.1/empiric/core/config.py` & `empiric_network-1.5.2/empiric/core/config.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.1/empiric/core/contract.py` & `empiric_network-1.5.2/empiric/core/contract.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.1/empiric/core/entry.py` & `empiric_network-1.5.2/empiric/core/entry.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.1/empiric/core/mixins/evm.py` & `empiric_network-1.5.2/empiric/core/mixins/evm.py`

 * *Files 1% similar despite different names*

```diff
@@ -636,15 +636,15 @@
         ],
         "stateMutability": "view",
         "type": "function",
     },
 ]
 
 ORACLE_ADDRESS = {
-    LINEA_TESTNET: "0x8A571d47fA7Ce97E8F6BDcEFAc1221585567C84b",
+    LINEA_TESTNET: "0xa2c8B12F06c27F235F1732A95cb86667476951Ac",
     SCROLL_TESTNET: "0xbb91Ed469258069Ff2590CA11E1800DE05Bf6Ec7",
     ERA_TESTNET: "0x807dEEA2a8BA552b13C418F1E9Ac8a12af77D1B1",
 }
 
 
 class EvmHelper:
     def __init__(
@@ -706,24 +706,32 @@
         self.w3.eth.sendRawTransaction(signed_txn.rawTransaction)
 
         return signed_txn.hash.hex()
 
     def publish_spot_entries(self, spot_entries: List[SpotEntry], gas_price=int(1e8), gas=int(1e6)):
         serialized_spot_entries = SpotEntry.serialize_entries_evm(spot_entries)
         nonce = self.w3.eth.get_transaction_count(self.sender)
-        transaction = self.oracle.functions.publishSpotEntries(
-            serialized_spot_entries
-        ).build_transaction(
-            {
+
+        # Transaction params
+        # If it's a legacy transaction, we need to set the gasPrice and gas
+        build_params = {
                 "nonce": nonce,
                 "chainId": self.chain_id,
                 "from": self.sender,
-                "gasPrice": gas_price,
-                "gas": gas,
-            }
+        }
+        if gas_price > 0:
+            build_params["gasPrice"] = gas_price
+        if gas > 0:
+            build_params["gas"] = gas
+
+        transaction = self.oracle.functions.publishSpotEntries(
+            serialized_spot_entries
+        ).build_transaction(
+            build_params
         )
+
         signed_tx = self.w3.eth.account.sign_transaction(transaction, self.private_key)
 
         txn_hash = self.w3.eth.send_raw_transaction(signed_tx.rawTransaction)
         txn_receipt = self.w3.eth.wait_for_transaction_receipt(txn_hash)
 
         return txn_hash.hex()
```

### Comparing `empiric_network-1.5.1/empiric/core/mixins/nonce.py` & `empiric_network-1.5.2/empiric/core/mixins/nonce.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.1/empiric/core/mixins/oracle.py` & `empiric_network-1.5.2/empiric/core/mixins/oracle.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.1/empiric/core/mixins/publisher_registry.py` & `empiric_network-1.5.2/empiric/core/mixins/publisher_registry.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.1/empiric/core/mixins/randomness.py` & `empiric_network-1.5.2/empiric/core/mixins/randomness.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.1/empiric/core/mixins/transactions.py` & `empiric_network-1.5.2/empiric/core/mixins/transactions.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.1/empiric/core/types.py` & `empiric_network-1.5.2/empiric/core/types.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.1/empiric/core/utils.py` & `empiric_network-1.5.2/empiric/core/utils.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.1/empiric/publisher/assets.py` & `empiric_network-1.5.2/empiric/publisher/assets.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.1/empiric/publisher/client.py` & `empiric_network-1.5.2/empiric/publisher/client.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.1/empiric/publisher/fetchers/ascendex.py` & `empiric_network-1.5.2/empiric/publisher/fetchers/ascendex.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.1/empiric/publisher/fetchers/bitstamp.py` & `empiric_network-1.5.2/empiric/publisher/fetchers/bitstamp.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.1/empiric/publisher/fetchers/cex.py` & `empiric_network-1.5.2/empiric/publisher/fetchers/cex.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.1/empiric/publisher/fetchers/coinbase.py` & `empiric_network-1.5.2/empiric/publisher/fetchers/coinbase.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.1/empiric/publisher/fetchers/coingecko.py` & `empiric_network-1.5.2/empiric/publisher/fetchers/coingecko.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.1/empiric/publisher/fetchers/defillama.py` & `empiric_network-1.5.2/empiric/publisher/fetchers/defillama.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.1/empiric/publisher/fetchers/gemini.py` & `empiric_network-1.5.2/empiric/publisher/fetchers/gemini.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.1/empiric/publisher/fetchers/kaiko.py` & `empiric_network-1.5.2/empiric/publisher/fetchers/kaiko.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.1/empiric/publisher/fetchers/okx.py` & `empiric_network-1.5.2/empiric/publisher/fetchers/okx.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.1/empiric/publisher/fetchers/thegraph.py` & `empiric_network-1.5.2/empiric/publisher/fetchers/thegraph.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.1/empiric/publisher/types.py` & `empiric_network-1.5.2/empiric/publisher/types.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.1/empiric/test/interface_consistency.py` & `empiric_network-1.5.2/empiric/test/interface_consistency.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.1/pyproject.toml` & `empiric_network-1.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
 
 [tool.poetry]
 name = "empiric-network"
-version = "1.5.1"
+version = "1.5.2"
 authors = ["Pragma <contact@pragmaoracle.com>"]
 description = "Core package for rollup-native Pragma Oracle"
 readme = "README.md"
 homepage = "https://pragmaoracle.com"
 repository = "https://github.com/Astraly-Labs/Pragma"
 documentation = "https://docs.pragmaoracle.com"
 classifiers = [
```

### Comparing `empiric_network-1.5.1/PKG-INFO` & `empiric_network-1.5.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: empiric-network
-Version: 1.5.1
+Version: 1.5.2
 Summary: Core package for rollup-native Pragma Oracle
 Home-page: https://pragmaoracle.com
 Author: Pragma
 Author-email: contact@pragmaoracle.com
 Requires-Python: >=3.9,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

