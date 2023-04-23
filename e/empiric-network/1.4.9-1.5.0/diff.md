# Comparing `tmp/empiric_network-1.4.9.tar.gz` & `tmp/empiric_network-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "empiric_network-1.4.9.tar", max compression
+gzip compressed data, was "empiric_network-1.5.0.tar", max compression
```

## Comparing `empiric_network-1.4.9.tar` & `empiric_network-1.5.0.tar`

### file list

```diff
@@ -1,62 +1,64 @@
--rw-r--r--   0        0        0      284 2023-01-29 19:05:27.756261 empiric_network-1.4.9/README.md
--rw-r--r--   0        0        0      204 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/cli/.example.config copy.ini
--rw-r--r--   0        0        0      697 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/cli/README.md
--rw-r--r--   0        0        0      342 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/cli/__init__.py
--rw-r--r--   0        0        0      148 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/cli/__main__.py
--rw-r--r--   0        0        0     1628 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/cli/account.py
--rw-r--r--   0        0        0   544336 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/cli/compiled_account_contract.py
--rw-r--r--   0        0        0     2050 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/cli/config.py
--rw-r--r--   0        0        0     1118 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/cli/contracts/__init__.py
--rw-r--r--   0        0        0     8098 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/cli/contracts/oracle.py
--rw-r--r--   0        0        0     5217 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/cli/contracts/publisher_registry.py
--rw-r--r--   0        0        0     2638 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/cli/contracts/summary_stats.py
--rw-r--r--   0        0        0     3318 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/cli/contracts/utils.py
--rw-r--r--   0        0        0     4080 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/cli/empiric_cli.py
--rw-r--r--   0        0        0     2682 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/cli/net.py
--rw-r--r--   0        0        0     1420 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/cli/publisher/__init__.py
--rw-r--r--   0        0        0    12230 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/cli/randomness/__init__.py
--rw-r--r--   0        0        0    16306 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/cli/randomness/randomness_utils.py
--rw-r--r--   0        0        0     3682 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/cli/randomness/utils.py
--rw-r--r--   0        0        0      547 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/cli/sample_config/oracle_constructor_data.json
--rw-r--r--   0        0        0        0 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/cli/tests/__init__.py
--rw-r--r--   0        0        0      262 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/cli/tests/test_empiric_cli.py
--rw-r--r--   0        0        0      236 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/cli/utils.py
--rw-r--r--   0        0        0      193 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/core/__init__.py
--rw-r--r--   0        0        0      284 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/core/abis/__init__.py
--rw-r--r--   0        0        0    14135 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/core/abis/oracle.py
--rw-r--r--   0        0        0     1436 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/core/abis/proxy.py
--rw-r--r--   0        0        0     3896 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/core/abis/publisher_registry.py
--rw-r--r--   0        0        0     5912 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/core/abis/randomness.py
--rw-r--r--   0        0        0      868 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/core/abis/summary_stats.py
--rw-r--r--   0        0        0     4557 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/core/client.py
--rw-r--r--   0        0        0     2150 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/core/config.py
--rw-r--r--   0        0        0     3801 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/core/contract.py
--rw-r--r--   0        0        0     8936 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/core/entry.py
--rw-r--r--   0        0        0      387 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/core/logger.py
--rw-r--r--   0        0        0      295 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/core/mixins/__init__.py
--rw-r--r--   0        0        0     5546 2023-01-29 19:05:27.756261 empiric_network-1.4.9/empiric/core/mixins/evm.py
--rw-r--r--   0        0        0     3074 2023-01-29 19:05:27.760261 empiric_network-1.4.9/empiric/core/mixins/nonce.py
--rw-r--r--   0        0        0     8808 2023-01-29 19:05:27.760261 empiric_network-1.4.9/empiric/core/mixins/oracle.py
--rw-r--r--   0        0        0     2287 2023-01-29 19:05:27.760261 empiric_network-1.4.9/empiric/core/mixins/publisher_registry.py
--rw-r--r--   0        0        0     3065 2023-01-29 19:05:27.760261 empiric_network-1.4.9/empiric/core/mixins/randomness.py
--rw-r--r--   0        0        0      669 2023-01-29 19:05:27.760261 empiric_network-1.4.9/empiric/core/mixins/transactions.py
--rw-r--r--   0        0        0     2913 2023-01-29 19:05:27.760261 empiric_network-1.4.9/empiric/core/types.py
--rw-r--r--   0        0        0      880 2023-01-29 19:05:27.760261 empiric_network-1.4.9/empiric/core/utils.py
--rw-r--r--   0        0        0       82 2023-01-29 19:05:27.760261 empiric_network-1.4.9/empiric/publisher/__init__.py
--rw-r--r--   0        0        0     2716 2023-01-29 19:05:27.760261 empiric_network-1.4.9/empiric/publisher/assets.py
--rw-r--r--   0        0        0     2261 2023-01-29 19:05:27.760261 empiric_network-1.4.9/empiric/publisher/client.py
--rw-r--r--   0        0        0      282 2023-01-29 19:05:27.760261 empiric_network-1.4.9/empiric/publisher/fetchers/__init__.py
--rw-r--r--   0        0        0     3747 2023-01-29 19:05:27.760261 empiric_network-1.4.9/empiric/publisher/fetchers/ascendex.py
--rw-r--r--   0        0        0     3017 2023-01-29 19:05:27.760261 empiric_network-1.4.9/empiric/publisher/fetchers/bitstamp.py
--rw-r--r--   0        0        0     3380 2023-01-29 19:05:27.760261 empiric_network-1.4.9/empiric/publisher/fetchers/cex.py
--rw-r--r--   0        0        0     2953 2023-01-29 19:05:27.760261 empiric_network-1.4.9/empiric/publisher/fetchers/coinbase.py
--rw-r--r--   0        0        0     3980 2023-01-29 19:05:27.760261 empiric_network-1.4.9/empiric/publisher/fetchers/coingecko.py
--rw-r--r--   0        0        0     3814 2023-01-29 19:05:27.760261 empiric_network-1.4.9/empiric/publisher/fetchers/gemini.py
--rw-r--r--   0        0        0     3631 2023-01-29 19:05:27.760261 empiric_network-1.4.9/empiric/publisher/fetchers/okx.py
--rw-r--r--   0        0        0     3762 2023-01-29 19:05:27.760261 empiric_network-1.4.9/empiric/publisher/fetchers/thegraph.py
--rw-r--r--   0        0        0      668 2023-01-29 19:05:27.760261 empiric_network-1.4.9/empiric/publisher/types.py
--rw-r--r--   0        0        0        0 2023-01-29 19:05:27.760261 empiric_network-1.4.9/empiric/test/__init__.py
--rw-r--r--   0        0        0     5965 2023-01-29 19:05:27.760261 empiric_network-1.4.9/empiric/test/interface_consistency.py
--rw-r--r--   0        0        0     1000 2023-01-29 19:05:27.760261 empiric_network-1.4.9/pyproject.toml
--rw-r--r--   0        0        0     1545 1970-01-01 00:00:00.000000 empiric_network-1.4.9/setup.py
--rw-r--r--   0        0        0      981 1970-01-01 00:00:00.000000 empiric_network-1.4.9/PKG-INFO
+-rw-r--r--   0        0        0      284 2023-04-23 14:08:16.898318 empiric_network-1.5.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-23 14:08:16.898318 empiric_network-1.5.0/empiric/__init__.py
+-rw-r--r--   0        0        0      204 2023-04-23 14:08:16.898318 empiric_network-1.5.0/empiric/cli/.example.config copy.ini
+-rw-r--r--   0        0        0      697 2023-04-23 14:08:16.898318 empiric_network-1.5.0/empiric/cli/README.md
+-rw-r--r--   0        0        0      342 2023-04-23 14:08:16.898318 empiric_network-1.5.0/empiric/cli/__init__.py
+-rw-r--r--   0        0        0      148 2023-04-23 14:08:16.898318 empiric_network-1.5.0/empiric/cli/__main__.py
+-rw-r--r--   0        0        0     1628 2023-04-23 14:08:16.898318 empiric_network-1.5.0/empiric/cli/account.py
+-rw-r--r--   0        0        0   544336 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/cli/compiled_account_contract.py
+-rw-r--r--   0        0        0     2050 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/cli/config.py
+-rw-r--r--   0        0        0     1118 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/cli/contracts/__init__.py
+-rw-r--r--   0        0        0     8098 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/cli/contracts/oracle.py
+-rw-r--r--   0        0        0     5217 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/cli/contracts/publisher_registry.py
+-rw-r--r--   0        0        0     2638 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/cli/contracts/summary_stats.py
+-rw-r--r--   0        0        0     3318 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/cli/contracts/utils.py
+-rw-r--r--   0        0        0     4080 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/cli/empiric_cli.py
+-rw-r--r--   0        0        0     2682 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/cli/net.py
+-rw-r--r--   0        0        0     1420 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/cli/publisher/__init__.py
+-rw-r--r--   0        0        0    12230 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/cli/randomness/__init__.py
+-rw-r--r--   0        0        0    16306 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/cli/randomness/randomness_utils.py
+-rw-r--r--   0        0        0     3682 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/cli/randomness/utils.py
+-rw-r--r--   0        0        0      547 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/cli/sample_config/oracle_constructor_data.json
+-rw-r--r--   0        0        0        0 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/cli/tests/__init__.py
+-rw-r--r--   0        0        0      262 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/cli/tests/test_empiric_cli.py
+-rw-r--r--   0        0        0      236 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/cli/utils.py
+-rw-r--r--   0        0        0      193 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/core/__init__.py
+-rw-r--r--   0        0        0      284 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/core/abis/__init__.py
+-rw-r--r--   0        0        0    14135 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/core/abis/oracle.py
+-rw-r--r--   0        0        0     1436 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/core/abis/proxy.py
+-rw-r--r--   0        0        0     3896 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/core/abis/publisher_registry.py
+-rw-r--r--   0        0        0     5912 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/core/abis/randomness.py
+-rw-r--r--   0        0        0      868 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/core/abis/summary_stats.py
+-rw-r--r--   0        0        0     4557 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/core/client.py
+-rw-r--r--   0        0        0     2150 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/core/config.py
+-rw-r--r--   0        0        0     3801 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/core/contract.py
+-rw-r--r--   0        0        0     9972 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/core/entry.py
+-rw-r--r--   0        0        0      387 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/core/logger.py
+-rw-r--r--   0        0        0      295 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/core/mixins/__init__.py
+-rw-r--r--   0        0        0    25171 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/core/mixins/evm.py
+-rw-r--r--   0        0        0     3074 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/core/mixins/nonce.py
+-rw-r--r--   0        0        0     8808 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/core/mixins/oracle.py
+-rw-r--r--   0        0        0     2287 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/core/mixins/publisher_registry.py
+-rw-r--r--   0        0        0     3065 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/core/mixins/randomness.py
+-rw-r--r--   0        0        0      669 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/core/mixins/transactions.py
+-rw-r--r--   0        0        0     3306 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/core/types.py
+-rw-r--r--   0        0        0      880 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/core/utils.py
+-rw-r--r--   0        0        0       82 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/publisher/__init__.py
+-rw-r--r--   0        0        0     2716 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/publisher/assets.py
+-rw-r--r--   0        0        0     2261 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/publisher/client.py
+-rw-r--r--   0        0        0      354 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/publisher/fetchers/__init__.py
+-rw-r--r--   0        0        0     3755 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/publisher/fetchers/ascendex.py
+-rw-r--r--   0        0        0     3017 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/publisher/fetchers/bitstamp.py
+-rw-r--r--   0        0        0     3380 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/publisher/fetchers/cex.py
+-rw-r--r--   0        0        0     2953 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/publisher/fetchers/coinbase.py
+-rw-r--r--   0        0        0     3980 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/publisher/fetchers/coingecko.py
+-rw-r--r--   0        0        0     3826 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/publisher/fetchers/defillama.py
+-rw-r--r--   0        0        0     3814 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/publisher/fetchers/gemini.py
+-rw-r--r--   0        0        0     3754 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/publisher/fetchers/kaiko.py
+-rw-r--r--   0        0        0     3631 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/publisher/fetchers/okx.py
+-rw-r--r--   0        0        0     3762 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/publisher/fetchers/thegraph.py
+-rw-r--r--   0        0        0      668 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/publisher/types.py
+-rw-r--r--   0        0        0        0 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/test/__init__.py
+-rw-r--r--   0        0        0     5965 2023-04-23 14:08:16.902318 empiric_network-1.5.0/empiric/test/interface_consistency.py
+-rw-r--r--   0        0        0     1088 2023-04-23 14:08:16.902318 empiric_network-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1032 1970-01-01 00:00:00.000000 empiric_network-1.5.0/PKG-INFO
```

### Comparing `empiric_network-1.4.9/empiric/cli/README.md` & `empiric_network-1.5.0/empiric/cli/README.md`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.9/empiric/cli/account.py` & `empiric_network-1.5.0/empiric/cli/account.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.9/empiric/cli/compiled_account_contract.py` & `empiric_network-1.5.0/empiric/cli/compiled_account_contract.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.9/empiric/cli/config.py` & `empiric_network-1.5.0/empiric/cli/config.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.9/empiric/cli/contracts/__init__.py` & `empiric_network-1.5.0/empiric/cli/contracts/__init__.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.9/empiric/cli/contracts/oracle.py` & `empiric_network-1.5.0/empiric/cli/contracts/oracle.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.9/empiric/cli/contracts/publisher_registry.py` & `empiric_network-1.5.0/empiric/cli/contracts/publisher_registry.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.9/empiric/cli/contracts/summary_stats.py` & `empiric_network-1.5.0/empiric/cli/contracts/summary_stats.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.9/empiric/cli/contracts/utils.py` & `empiric_network-1.5.0/empiric/cli/contracts/utils.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.9/empiric/cli/empiric_cli.py` & `empiric_network-1.5.0/empiric/cli/empiric_cli.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.9/empiric/cli/net.py` & `empiric_network-1.5.0/empiric/cli/net.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.9/empiric/cli/publisher/__init__.py` & `empiric_network-1.5.0/empiric/cli/publisher/__init__.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.9/empiric/cli/randomness/__init__.py` & `empiric_network-1.5.0/empiric/cli/randomness/__init__.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.9/empiric/cli/randomness/randomness_utils.py` & `empiric_network-1.5.0/empiric/cli/randomness/randomness_utils.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.9/empiric/cli/randomness/utils.py` & `empiric_network-1.5.0/empiric/cli/randomness/utils.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.9/empiric/cli/sample_config/oracle_constructor_data.json` & `empiric_network-1.5.0/empiric/cli/sample_config/oracle_constructor_data.json`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.9/empiric/core/abis/oracle.py` & `empiric_network-1.5.0/empiric/core/abis/oracle.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.9/empiric/core/abis/proxy.py` & `empiric_network-1.5.0/empiric/core/abis/proxy.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.9/empiric/core/abis/publisher_registry.py` & `empiric_network-1.5.0/empiric/core/abis/publisher_registry.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.9/empiric/core/abis/randomness.py` & `empiric_network-1.5.0/empiric/core/abis/randomness.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.9/empiric/core/abis/summary_stats.py` & `empiric_network-1.5.0/empiric/core/abis/summary_stats.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.9/empiric/core/client.py` & `empiric_network-1.5.0/empiric/core/client.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.9/empiric/core/config.py` & `empiric_network-1.5.0/empiric/core/config.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.9/empiric/core/contract.py` & `empiric_network-1.5.0/empiric/core/contract.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.9/empiric/core/entry.py` & `empiric_network-1.5.0/empiric/core/entry.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import abc
 from typing import Dict, List, Optional, Tuple, Union
 
 from empiric.core.utils import felt_to_str, str_to_felt
-
+from web3 import Web3
 
 class Entry(abc.ABC):
     @abc.abstractmethod
     def serialize(self) -> Dict[str, str]:
         ...
 
     @abc.abstractmethod
@@ -109,14 +109,15 @@
         pair_id: Union[str, int],
         price: int,
         timestamp: int,
         source: Union[str, int],
         publisher: Union[str, int],
         volume: Optional[int] = 0,
     ) -> None:
+        # TODO: This should be network agnostic
         if type(pair_id) == str:
             pair_id = str_to_felt(pair_id)
 
         if type(publisher) == str:
             publisher = str_to_felt(publisher)
 
         if type(source) == str:
@@ -168,14 +169,26 @@
                 "publisher": self.base.publisher,
             },
             "pair_id": self.pair_id,
             "price": self.price,
             "volume": self.volume,
         }
 
+    def serialize_evm(self) -> Dict[str, str]:
+        return {
+            "base": {
+                "timestamp": self.base.timestamp,
+                "source": Web3.toBytes(text=felt_to_str(self.base.source)),
+                "publisher": Web3.toBytes(text=felt_to_str(self.base.publisher)),
+            },
+            "pairId": Web3.toBytes(text=felt_to_str(self.pair_id)),
+            "price": self.price,
+            "volume": self.volume,
+        }
+
     @staticmethod
     def from_dict(entry_dict: Dict[str, str]) -> "SpotEntry":
         return SpotEntry(
             entry_dict["base"]["pair_id"],
             entry_dict["price"],
             entry_dict["timestamp"],
             entry_dict["base"]["source"],
@@ -190,14 +203,26 @@
             entry.serialize()
             for entry in entries
             # TODO (rlkelly): This needs to be much more resilient to publish errors
             if isinstance(entry, SpotEntry)
         ]
         return list(filter(lambda item: item is not None, serialized_entries))
 
+    @staticmethod
+    def serialize_entries_evm(entries: List[SpotEntry]) -> List[Dict[str, int]]:
+        """serialize entries to a List of dictionaries"""
+        # TODO (rlkelly): log errors
+        serialized_entries = [
+            entry.serialize_evm()
+            for entry in entries
+            # TODO (rlkelly): This needs to be much more resilient to publish errors
+            if isinstance(entry, SpotEntry)
+        ]
+        return list(filter(lambda item: item is not None, serialized_entries))
+
     def __repr__(self):
         return f'SpotEntry(pair_id="{felt_to_str(self.pair_id)}", price={self.price}, timestamp={self.base.timestamp}, source="{felt_to_str(self.base.source)}", publisher="{felt_to_str(self.base.publisher)}, volume={self.volume})")'
 
 
 class FutureEntry(Entry):
     timestamp: int
     source: int
```

### Comparing `empiric_network-1.4.9/empiric/core/mixins/nonce.py` & `empiric_network-1.5.0/empiric/core/mixins/nonce.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.9/empiric/core/mixins/oracle.py` & `empiric_network-1.5.0/empiric/core/mixins/oracle.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.9/empiric/core/mixins/publisher_registry.py` & `empiric_network-1.5.0/empiric/core/mixins/publisher_registry.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.9/empiric/core/mixins/randomness.py` & `empiric_network-1.5.0/empiric/core/mixins/randomness.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.9/empiric/core/mixins/transactions.py` & `empiric_network-1.5.0/empiric/core/mixins/transactions.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.9/empiric/core/types.py` & `empiric_network-1.5.0/empiric/core/types.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,27 +7,36 @@
 HEX_STR = str
 
 # Network Types
 STAGING = "staging"
 TESTNET = "testnet"
 INTEGRATION = "integration"
 MAINNET = "mainnet"
+SCROLL_TESTNET = "scroll_testnet"
+LINEA_TESTNET = "linea_testnet"
+ERA_TESTNET = "era_testnet"
 
 Network = Literal["staging", "testnet", "integration", "mainnet"]
 
 CHAIN_IDS = {
     INTEGRATION: 1536727068981429685321,
     TESTNET: 1536727068981429685321,
     MAINNET: 23448594291968334,
+    SCROLL_TESTNET: 534353,
+    LINEA_TESTNET: 59140,
+    ERA_TESTNET: 280
 }
 
 GATEWAY_URLS = {
     TESTNET: "https://alpha4.starknet.io",
     INTEGRATION: "https://external.integration.starknet.io",
     MAINNET: "https://alpha-mainnet.starknet.io",
+    SCROLL_TESTNET: "https://scroll-alphanet.public.blastapi.io",
+    LINEA_TESTNET: "https://consensys-zkevm-goerli-prealpha.infura.io/v3/ef9b71db32e242f39c6cf0691c8b521a",
+    ERA_TESTNET: "https://testnet.era.zksync.dev"
 }
 
 
 # aggregation mode enum
 @unique
 class AggregationMode(IntEnum):
     MEDIAN = 84959893733710  # str_to_felt("MEDIAN")
```

### Comparing `empiric_network-1.4.9/empiric/core/utils.py` & `empiric_network-1.5.0/empiric/core/utils.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.9/empiric/publisher/assets.py` & `empiric_network-1.5.0/empiric/publisher/assets.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.9/empiric/publisher/client.py` & `empiric_network-1.5.0/empiric/publisher/client.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.9/empiric/publisher/fetchers/ascendex.py` & `empiric_network-1.5.0/empiric/publisher/fetchers/ascendex.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
         async with session.get(url) as resp:
             if resp.status == 404:
                 return PublisherFetchError(
                     f"No data found for {'/'.join(pair)} from Ascendex"
                 )
             result = await resp.json(content_type="application/json")
-            if result["code"] == "100002" or result["reason"] == "DATA_NOT_AVAILABLE":
+            if result["code"] == "100002" and result["reason"] == "DATA_NOT_AVAILABLE":
                 return PublisherFetchError(
                     f"No data found for {'/'.join(pair)} from Ascendex"
                 )
 
             return self._construct(asset, result)
 
     def _fetch_pair_sync(
@@ -50,15 +50,15 @@
 
         resp = requests.get(url)
         if resp.status_code == 404:
             return PublisherFetchError(
                 f"No data found for {'/'.join(pair)} from Ascendex"
             )
         result = resp.json(content_type="application/json")
-        if result["code"] == "100002" or result["reason"] == "DATA_NOT_AVAILABLE":
+        if result["code"] == "100002" and result["reason"] == "DATA_NOT_AVAILABLE":
             return PublisherFetchError(
                 f"No data found for {'/'.join(pair)} from Ascendex"
             )
 
         return self._construct(asset, result)
 
     async def fetch(
@@ -80,22 +80,21 @@
                 continue
             entries.append(self._fetch_pair_sync(asset))
         return entries
 
     def _construct(self, asset, result) -> SpotEntry:
         pair = asset["pair"]
         data = result["data"]
-
         timestamp = int(time.time())
         ask = float(data["ask"][0])
         bid = float(data["bid"][0])
         price = (float(data["ask"][0]) + float(data["bid"][0])) / 2.0
         price_int = int(price * (10 ** asset["decimals"]))
         pair_id = currency_pair_to_pair_id(*pair)
-        volume = int(data["volume"])
+        volume = int(float(data["volume"]))
 
         logger.info(f"Fetched price {price} for {'/'.join(pair)} from Ascendex")
 
         return SpotEntry(
             pair_id=pair_id,
             price=price_int,
             volume=volume,
```

### Comparing `empiric_network-1.4.9/empiric/publisher/fetchers/bitstamp.py` & `empiric_network-1.5.0/empiric/publisher/fetchers/bitstamp.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.9/empiric/publisher/fetchers/cex.py` & `empiric_network-1.5.0/empiric/publisher/fetchers/cex.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.9/empiric/publisher/fetchers/coinbase.py` & `empiric_network-1.5.0/empiric/publisher/fetchers/coinbase.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.9/empiric/publisher/fetchers/coingecko.py` & `empiric_network-1.5.0/empiric/publisher/fetchers/coingecko.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.9/empiric/publisher/fetchers/gemini.py` & `empiric_network-1.5.0/empiric/publisher/fetchers/gemini.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.9/empiric/publisher/fetchers/okx.py` & `empiric_network-1.5.0/empiric/publisher/fetchers/okx.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.9/empiric/publisher/fetchers/thegraph.py` & `empiric_network-1.5.0/empiric/publisher/fetchers/thegraph.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.9/empiric/publisher/types.py` & `empiric_network-1.5.0/empiric/publisher/types.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.9/empiric/test/interface_consistency.py` & `empiric_network-1.5.0/empiric/test/interface_consistency.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.4.9/pyproject.toml` & `empiric_network-1.5.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -3,38 +3,40 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
 
 [tool.poetry]
 name = "empiric-network"
-version = "1.4.9"
-authors = ["Astraly Labs <contact@astraly.xyz>"]
-description = "Core package for rollup-native Empiric Network"
+version = "1.5.0"
+authors = ["Pragma <contact@pragmaoracle.com>"]
+description = "Core package for rollup-native Pragma Oracle"
 readme = "README.md"
-homepage = "https://empiric.network"
-repository = "https://github.com/Astraly-Labs/Empiric"
-documentation = "https://docs.empiric.network"
+homepage = "https://pragmaoracle.com"
+repository = "https://github.com/Astraly-Labs/Pragma"
+documentation = "https://docs.pragmaoracle.com"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 packages = [
+  {include = "empiric"},
   {include = "cli", from = "empiric"},
   {include = "core", from = "empiric"},
   {include = "publisher", from = "empiric"},
   {include = "test", from = "empiric"},
 ]
 
 [tool.poetry.dependencies]
-python = "3.9.13"
-"starknet.py" = "0.13.0a0"
+python = ">=3.9,<3.10"
+"starknet.py" = "0.14.0a0"
 cairo-lang = "0.10.3"
 typer = "0.6.1"
 
 [tool.poetry.dev-dependencies]
 black = "*"
 flake8 = "*"
 
 [tool.poetry.scripts]
 empiric = "empiric.cli:main"
+interface-check = "empiric.test.interface_consistency:main"
```

### Comparing `empiric_network-1.4.9/PKG-INFO` & `empiric_network-1.5.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: empiric-network
-Version: 1.4.9
-Summary: Core package for rollup-native Empiric Network
-Home-page: https://empiric.network
-Author: Astraly Labs
-Author-email: contact@astraly.xyz
-Requires-Python: ==3.9.13
+Version: 1.5.0
+Summary: Core package for rollup-native Pragma Oracle
+Home-page: https://pragmaoracle.com
+Author: Pragma
+Author-email: contact@pragmaoracle.com
+Requires-Python: >=3.9,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: cairo-lang (==0.10.3)
-Requires-Dist: starknet.py (==0.13.0a0)
+Requires-Dist: starknet.py (==0.14.0a0)
 Requires-Dist: typer (==0.6.1)
-Project-URL: Documentation, https://docs.empiric.network
-Project-URL: Repository, https://github.com/Astraly-Labs/Empiric
+Project-URL: Documentation, https://docs.pragmaoracle.com
+Project-URL: Repository, https://github.com/Astraly-Labs/Pragma
 Description-Content-Type: text/markdown
 
 # Empiric Network
 
 ## About
 
 For more information, see the [project's repository](https://github.com/Astraly-Labs/Empiric), [documentation overview](https://docs.empiric.network/) and [documentation on how to publish data](https://docs.empiric.network/using-empiric/publishing-data).
```

