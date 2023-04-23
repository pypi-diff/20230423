# Comparing `tmp/zeroconf-0.57.0.tar.gz` & `tmp/zeroconf-0.58.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeroconf-0.57.0.tar", max compression
+gzip compressed data, was "zeroconf-0.58.0.tar", max compression
```

## Comparing `zeroconf-0.57.0.tar` & `zeroconf-0.58.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0    49096 2023-04-23 18:49:10.747447 zeroconf-0.57.0/CHANGELOG.md
--rw-r--r--   0        0        0    24380 2023-04-23 18:49:09.971442 zeroconf-0.57.0/COPYING
--rw-r--r--   0        0        0     4407 2023-04-23 18:49:09.971442 zeroconf-0.57.0/README.rst
--rw-r--r--   0        0        0     1060 2023-04-23 18:49:09.971442 zeroconf-0.57.0/build_ext.py
--rw-r--r--   0        0        0     6770 2023-04-23 18:49:09.971442 zeroconf-0.57.0/docs/Makefile
--rw-r--r--   0        0        0      234 2023-04-23 18:49:09.971442 zeroconf-0.57.0/docs/api.rst
--rw-r--r--   0        0        0     8145 2023-04-23 18:49:09.971442 zeroconf-0.57.0/docs/conf.py
--rw-r--r--   0        0        0      991 2023-04-23 18:49:09.971442 zeroconf-0.57.0/docs/index.rst
--rw-r--r--   0        0        0     3995 2023-04-23 18:49:10.823448 zeroconf-0.57.0/pyproject.toml
--rw-r--r--   0        0        0     3868 2023-04-23 18:49:10.759447 zeroconf-0.57.0/src/zeroconf/__init__.py
--rw-r--r--   0        0        0      511 2023-04-23 18:49:09.971442 zeroconf-0.57.0/src/zeroconf/_cache.pxd
--rw-r--r--   0        0        0     8493 2023-04-23 18:49:09.971442 zeroconf-0.57.0/src/zeroconf/_cache.py
--rw-r--r--   0        0        0    39043 2023-04-23 18:49:09.971442 zeroconf-0.57.0/src/zeroconf/_core.py
--rw-r--r--   0        0        0     2061 2023-04-23 18:49:09.971442 zeroconf-0.57.0/src/zeroconf/_dns.pxd
--rw-r--r--   0        0        0    18218 2023-04-23 18:49:09.971442 zeroconf-0.57.0/src/zeroconf/_dns.py
--rw-r--r--   0        0        0     2167 2023-04-23 18:49:09.971442 zeroconf-0.57.0/src/zeroconf/_exceptions.py
--rw-r--r--   0        0        0    25863 2023-04-23 18:49:09.971442 zeroconf-0.57.0/src/zeroconf/_handlers.py
--rw-r--r--   0        0        0     2916 2023-04-23 18:49:09.971442 zeroconf-0.57.0/src/zeroconf/_history.py
--rw-r--r--   0        0        0     2980 2023-04-23 18:49:09.971442 zeroconf-0.57.0/src/zeroconf/_logger.py
--rw-r--r--   0        0        0      971 2023-04-23 18:49:09.975442 zeroconf-0.57.0/src/zeroconf/_protocol/__init__.py
--rw-r--r--   0        0        0     2154 2023-04-23 18:49:09.975442 zeroconf-0.57.0/src/zeroconf/_protocol/incoming.pxd
--rw-r--r--   0        0        0    13655 2023-04-23 18:49:09.975442 zeroconf-0.57.0/src/zeroconf/_protocol/incoming.py
--rw-r--r--   0        0        0     1950 2023-04-23 18:49:09.975442 zeroconf-0.57.0/src/zeroconf/_protocol/outgoing.pxd
--rw-r--r--   0        0        0    17758 2023-04-23 18:49:09.975442 zeroconf-0.57.0/src/zeroconf/_protocol/outgoing.py
--rw-r--r--   0        0        0     2355 2023-04-23 18:49:09.975442 zeroconf-0.57.0/src/zeroconf/_services/__init__.py
--rw-r--r--   0        0        0    22174 2023-04-23 18:49:09.975442 zeroconf-0.57.0/src/zeroconf/_services/browser.py
--rw-r--r--   0        0        0    25364 2023-04-23 18:49:09.975442 zeroconf-0.57.0/src/zeroconf/_services/info.py
--rw-r--r--   0        0        0     3964 2023-04-23 18:49:09.975442 zeroconf-0.57.0/src/zeroconf/_services/registry.py
--rw-r--r--   0        0        0     3003 2023-04-23 18:49:09.975442 zeroconf-0.57.0/src/zeroconf/_services/types.py
--rw-r--r--   0        0        0     2909 2023-04-23 18:49:09.975442 zeroconf-0.57.0/src/zeroconf/_updates.py
--rw-r--r--   0        0        0      971 2023-04-23 18:49:09.975442 zeroconf-0.57.0/src/zeroconf/_utils/__init__.py
--rw-r--r--   0        0        0     4144 2023-04-23 18:49:09.975442 zeroconf-0.57.0/src/zeroconf/_utils/asyncio.py
--rw-r--r--   0        0        0     6904 2023-04-23 18:49:09.975442 zeroconf-0.57.0/src/zeroconf/_utils/name.py
--rw-r--r--   0        0        0    15252 2023-04-23 18:49:09.975442 zeroconf-0.57.0/src/zeroconf/_utils/net.py
--rw-r--r--   0        0        0     1308 2023-04-23 18:49:09.975442 zeroconf-0.57.0/src/zeroconf/_utils/time.py
--rw-r--r--   0        0        0    11084 2023-04-23 18:49:09.975442 zeroconf-0.57.0/src/zeroconf/asyncio.py
--rw-r--r--   0        0        0     4469 2023-04-23 18:49:09.975442 zeroconf-0.57.0/src/zeroconf/const.py
--rw-r--r--   0        0        0        0 2023-04-23 18:49:09.975442 zeroconf-0.57.0/src/zeroconf/py.typed
--rw-r--r--   0        0        0     2416 2023-04-23 18:49:09.975442 zeroconf-0.57.0/tests/__init__.py
--rw-r--r--   0        0        0      668 2023-04-23 18:49:09.975442 zeroconf-0.57.0/tests/conftest.py
--rw-r--r--   0        0        0      971 2023-04-23 18:49:09.975442 zeroconf-0.57.0/tests/services/__init__.py
--rw-r--r--   0        0        0    42950 2023-04-23 18:49:09.975442 zeroconf-0.57.0/tests/services/test_browser.py
--rw-r--r--   0        0        0    45244 2023-04-23 18:49:09.975442 zeroconf-0.57.0/tests/services/test_info.py
--rw-r--r--   0        0        0     4923 2023-04-23 18:49:09.975442 zeroconf-0.57.0/tests/services/test_registry.py
--rw-r--r--   0        0        0     6273 2023-04-23 18:49:09.975442 zeroconf-0.57.0/tests/services/test_types.py
--rw-r--r--   0        0        0    41883 2023-04-23 18:49:09.975442 zeroconf-0.57.0/tests/test_asyncio.py
--rw-r--r--   0        0        0     8830 2023-04-23 18:49:09.975442 zeroconf-0.57.0/tests/test_cache.py
--rw-r--r--   0        0        0    29468 2023-04-23 18:49:09.975442 zeroconf-0.57.0/tests/test_core.py
--rw-r--r--   0        0        0    14686 2023-04-23 18:49:09.975442 zeroconf-0.57.0/tests/test_dns.py
--rw-r--r--   0        0        0     5022 2023-04-23 18:49:09.975442 zeroconf-0.57.0/tests/test_exceptions.py
--rw-r--r--   0        0        0    63127 2023-04-23 18:49:09.975442 zeroconf-0.57.0/tests/test_handlers.py
--rw-r--r--   0        0        0     2580 2023-04-23 18:49:09.975442 zeroconf-0.57.0/tests/test_history.py
--rw-r--r--   0        0        0     6640 2023-04-23 18:49:09.975442 zeroconf-0.57.0/tests/test_init.py
--rw-r--r--   0        0        0     3396 2023-04-23 18:49:09.975442 zeroconf-0.57.0/tests/test_logger.py
--rw-r--r--   0        0        0    41672 2023-04-23 18:49:09.975442 zeroconf-0.57.0/tests/test_protocol.py
--rw-r--r--   0        0        0     9477 2023-04-23 18:49:09.975442 zeroconf-0.57.0/tests/test_services.py
--rw-r--r--   0        0        0     2240 2023-04-23 18:49:09.975442 zeroconf-0.57.0/tests/test_updates.py
--rw-r--r--   0        0        0      971 2023-04-23 18:49:09.979442 zeroconf-0.57.0/tests/utils/__init__.py
--rw-r--r--   0        0        0     5101 2023-04-23 18:49:09.979442 zeroconf-0.57.0/tests/utils/test_asyncio.py
--rw-r--r--   0        0        0     2045 2023-04-23 18:49:09.979442 zeroconf-0.57.0/tests/utils/test_name.py
--rw-r--r--   0        0        0     9413 2023-04-23 18:49:09.979442 zeroconf-0.57.0/tests/utils/test_net.py
--rw-r--r--   0        0        0     5527 1970-01-01 00:00:00.000000 zeroconf-0.57.0/setup.py
--rw-r--r--   0        0        0     6297 1970-01-01 00:00:00.000000 zeroconf-0.57.0/PKG-INFO
+-rw-r--r--   0        0        0    49348 2023-04-23 20:04:25.622252 zeroconf-0.58.0/CHANGELOG.md
+-rw-r--r--   0        0        0    24380 2023-04-23 20:04:24.778237 zeroconf-0.58.0/COPYING
+-rw-r--r--   0        0        0     4407 2023-04-23 20:04:24.782237 zeroconf-0.58.0/README.rst
+-rw-r--r--   0        0        0     1060 2023-04-23 20:04:24.782237 zeroconf-0.58.0/build_ext.py
+-rw-r--r--   0        0        0     6770 2023-04-23 20:04:24.782237 zeroconf-0.58.0/docs/Makefile
+-rw-r--r--   0        0        0      234 2023-04-23 20:04:24.782237 zeroconf-0.58.0/docs/api.rst
+-rw-r--r--   0        0        0     8145 2023-04-23 20:04:24.782237 zeroconf-0.58.0/docs/conf.py
+-rw-r--r--   0        0        0      991 2023-04-23 20:04:24.782237 zeroconf-0.58.0/docs/index.rst
+-rw-r--r--   0        0        0     3995 2023-04-23 20:04:25.698253 zeroconf-0.58.0/pyproject.toml
+-rw-r--r--   0        0        0     3868 2023-04-23 20:04:25.630252 zeroconf-0.58.0/src/zeroconf/__init__.py
+-rw-r--r--   0        0        0      511 2023-04-23 20:04:24.782237 zeroconf-0.58.0/src/zeroconf/_cache.pxd
+-rw-r--r--   0        0        0     8493 2023-04-23 20:04:24.782237 zeroconf-0.58.0/src/zeroconf/_cache.py
+-rw-r--r--   0        0        0    39043 2023-04-23 20:04:24.782237 zeroconf-0.58.0/src/zeroconf/_core.py
+-rw-r--r--   0        0        0     2061 2023-04-23 20:04:24.782237 zeroconf-0.58.0/src/zeroconf/_dns.pxd
+-rw-r--r--   0        0        0    18218 2023-04-23 20:04:24.782237 zeroconf-0.58.0/src/zeroconf/_dns.py
+-rw-r--r--   0        0        0     2167 2023-04-23 20:04:24.782237 zeroconf-0.58.0/src/zeroconf/_exceptions.py
+-rw-r--r--   0        0        0    25863 2023-04-23 20:04:24.782237 zeroconf-0.58.0/src/zeroconf/_handlers.py
+-rw-r--r--   0        0        0     2916 2023-04-23 20:04:24.782237 zeroconf-0.58.0/src/zeroconf/_history.py
+-rw-r--r--   0        0        0     2980 2023-04-23 20:04:24.782237 zeroconf-0.58.0/src/zeroconf/_logger.py
+-rw-r--r--   0        0        0      971 2023-04-23 20:04:24.782237 zeroconf-0.58.0/src/zeroconf/_protocol/__init__.py
+-rw-r--r--   0        0        0     2385 2023-04-23 20:04:24.782237 zeroconf-0.58.0/src/zeroconf/_protocol/incoming.pxd
+-rw-r--r--   0        0        0    13655 2023-04-23 20:04:24.782237 zeroconf-0.58.0/src/zeroconf/_protocol/incoming.py
+-rw-r--r--   0        0        0     1950 2023-04-23 20:04:24.782237 zeroconf-0.58.0/src/zeroconf/_protocol/outgoing.pxd
+-rw-r--r--   0        0        0    17758 2023-04-23 20:04:24.782237 zeroconf-0.58.0/src/zeroconf/_protocol/outgoing.py
+-rw-r--r--   0        0        0     2355 2023-04-23 20:04:24.782237 zeroconf-0.58.0/src/zeroconf/_services/__init__.py
+-rw-r--r--   0        0        0    22174 2023-04-23 20:04:24.786237 zeroconf-0.58.0/src/zeroconf/_services/browser.py
+-rw-r--r--   0        0        0    25364 2023-04-23 20:04:24.786237 zeroconf-0.58.0/src/zeroconf/_services/info.py
+-rw-r--r--   0        0        0     3964 2023-04-23 20:04:24.786237 zeroconf-0.58.0/src/zeroconf/_services/registry.py
+-rw-r--r--   0        0        0     3003 2023-04-23 20:04:24.786237 zeroconf-0.58.0/src/zeroconf/_services/types.py
+-rw-r--r--   0        0        0     2909 2023-04-23 20:04:24.786237 zeroconf-0.58.0/src/zeroconf/_updates.py
+-rw-r--r--   0        0        0      971 2023-04-23 20:04:24.786237 zeroconf-0.58.0/src/zeroconf/_utils/__init__.py
+-rw-r--r--   0        0        0     4144 2023-04-23 20:04:24.786237 zeroconf-0.58.0/src/zeroconf/_utils/asyncio.py
+-rw-r--r--   0        0        0     6904 2023-04-23 20:04:24.786237 zeroconf-0.58.0/src/zeroconf/_utils/name.py
+-rw-r--r--   0        0        0    15252 2023-04-23 20:04:24.786237 zeroconf-0.58.0/src/zeroconf/_utils/net.py
+-rw-r--r--   0        0        0     1308 2023-04-23 20:04:24.786237 zeroconf-0.58.0/src/zeroconf/_utils/time.py
+-rw-r--r--   0        0        0    11084 2023-04-23 20:04:24.786237 zeroconf-0.58.0/src/zeroconf/asyncio.py
+-rw-r--r--   0        0        0     4469 2023-04-23 20:04:24.786237 zeroconf-0.58.0/src/zeroconf/const.py
+-rw-r--r--   0        0        0        0 2023-04-23 20:04:24.786237 zeroconf-0.58.0/src/zeroconf/py.typed
+-rw-r--r--   0        0        0     2416 2023-04-23 20:04:24.786237 zeroconf-0.58.0/tests/__init__.py
+-rw-r--r--   0        0        0      668 2023-04-23 20:04:24.786237 zeroconf-0.58.0/tests/conftest.py
+-rw-r--r--   0        0        0      971 2023-04-23 20:04:24.786237 zeroconf-0.58.0/tests/services/__init__.py
+-rw-r--r--   0        0        0    42950 2023-04-23 20:04:24.786237 zeroconf-0.58.0/tests/services/test_browser.py
+-rw-r--r--   0        0        0    45244 2023-04-23 20:04:24.786237 zeroconf-0.58.0/tests/services/test_info.py
+-rw-r--r--   0        0        0     4923 2023-04-23 20:04:24.786237 zeroconf-0.58.0/tests/services/test_registry.py
+-rw-r--r--   0        0        0     6273 2023-04-23 20:04:24.786237 zeroconf-0.58.0/tests/services/test_types.py
+-rw-r--r--   0        0        0    41883 2023-04-23 20:04:24.786237 zeroconf-0.58.0/tests/test_asyncio.py
+-rw-r--r--   0        0        0     8830 2023-04-23 20:04:24.786237 zeroconf-0.58.0/tests/test_cache.py
+-rw-r--r--   0        0        0    29468 2023-04-23 20:04:24.786237 zeroconf-0.58.0/tests/test_core.py
+-rw-r--r--   0        0        0    14686 2023-04-23 20:04:24.786237 zeroconf-0.58.0/tests/test_dns.py
+-rw-r--r--   0        0        0     5022 2023-04-23 20:04:24.786237 zeroconf-0.58.0/tests/test_exceptions.py
+-rw-r--r--   0        0        0    63127 2023-04-23 20:04:24.786237 zeroconf-0.58.0/tests/test_handlers.py
+-rw-r--r--   0        0        0     2580 2023-04-23 20:04:24.786237 zeroconf-0.58.0/tests/test_history.py
+-rw-r--r--   0        0        0     6640 2023-04-23 20:04:24.786237 zeroconf-0.58.0/tests/test_init.py
+-rw-r--r--   0        0        0     3396 2023-04-23 20:04:24.786237 zeroconf-0.58.0/tests/test_logger.py
+-rw-r--r--   0        0        0    41672 2023-04-23 20:04:24.786237 zeroconf-0.58.0/tests/test_protocol.py
+-rw-r--r--   0        0        0     9477 2023-04-23 20:04:24.786237 zeroconf-0.58.0/tests/test_services.py
+-rw-r--r--   0        0        0     2240 2023-04-23 20:04:24.786237 zeroconf-0.58.0/tests/test_updates.py
+-rw-r--r--   0        0        0      971 2023-04-23 20:04:24.786237 zeroconf-0.58.0/tests/utils/__init__.py
+-rw-r--r--   0        0        0     5101 2023-04-23 20:04:24.786237 zeroconf-0.58.0/tests/utils/test_asyncio.py
+-rw-r--r--   0        0        0     2045 2023-04-23 20:04:24.786237 zeroconf-0.58.0/tests/utils/test_name.py
+-rw-r--r--   0        0        0     9413 2023-04-23 20:04:24.786237 zeroconf-0.58.0/tests/utils/test_net.py
+-rw-r--r--   0        0        0     5527 1970-01-01 00:00:00.000000 zeroconf-0.58.0/setup.py
+-rw-r--r--   0        0        0     6297 1970-01-01 00:00:00.000000 zeroconf-0.58.0/PKG-INFO
```

### Comparing `zeroconf-0.57.0/CHANGELOG.md` & `zeroconf-0.58.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.58.0 (2023-04-23)
+### Feature
+* Speed up incoming parser ([#1163](https://github.com/python-zeroconf/python-zeroconf/issues/1163)) ([`4626399`](https://github.com/python-zeroconf/python-zeroconf/commit/46263999c0c7ea5176885f1eadd2c8498834b70e))
+
 ## v0.57.0 (2023-04-23)
 ### Feature
 * Speed up incoming data parser ([#1161](https://github.com/python-zeroconf/python-zeroconf/issues/1161)) ([`cb4c3b2`](https://github.com/python-zeroconf/python-zeroconf/commit/cb4c3b2b80ca3b88b8de6e87062a45e03e8805a6))
 
 ## v0.56.0 (2023-04-07)
 ### Feature
 * Reduce denial of service protection overhead ([#1157](https://github.com/python-zeroconf/python-zeroconf/issues/1157)) ([`2c2f26a`](https://github.com/python-zeroconf/python-zeroconf/commit/2c2f26a87d0aac81a77205b06bc9ba499caa2321))
```

### Comparing `zeroconf-0.57.0/COPYING` & `zeroconf-0.58.0/COPYING`

 * *Files identical despite different names*

### Comparing `zeroconf-0.57.0/README.rst` & `zeroconf-0.58.0/README.rst`

 * *Files identical despite different names*

### Comparing `zeroconf-0.57.0/build_ext.py` & `zeroconf-0.58.0/build_ext.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.57.0/docs/Makefile` & `zeroconf-0.58.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zeroconf-0.57.0/docs/conf.py` & `zeroconf-0.58.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.57.0/docs/index.rst` & `zeroconf-0.58.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `zeroconf-0.57.0/pyproject.toml` & `zeroconf-0.58.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zeroconf"
-version = "0.57.0"
+version = "0.58.0"
 description = "A pure python implementation of multicast DNS service discovery"
 authors = ["Paul Scott-Murphy", "William McBrine", "Jakub Stasiak", "J. Nick Koston"]
 license = "LGPL"
 readme = "README.rst"
 repository = "https://github.com/python-zeroconf/python-zeroconf"
 documentation = "https://python-zeroconf.readthedocs.io"
 classifiers=[
```

### Comparing `zeroconf-0.57.0/src/zeroconf/__init__.py` & `zeroconf-0.58.0/src/zeroconf/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 from ._utils.time import (  # noqa # import needed for backwards compat
     current_time_millis,
     millis_to_seconds,
 )
 
 __author__ = 'Paul Scott-Murphy, William McBrine'
 __maintainer__ = 'Jakub Stasiak <jakub@stasiak.at>'
-__version__ = '0.57.0'
+__version__ = '0.58.0'
 __license__ = 'LGPL'
 
 
 __all__ = [
     "__version__",
     "Zeroconf",
     "ServiceInfo",
```

### Comparing `zeroconf-0.57.0/src/zeroconf/_cache.py` & `zeroconf-0.58.0/src/zeroconf/_cache.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.57.0/src/zeroconf/_core.py` & `zeroconf-0.58.0/src/zeroconf/_core.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.57.0/src/zeroconf/_dns.pxd` & `zeroconf-0.58.0/src/zeroconf/_dns.pxd`

 * *Files identical despite different names*

### Comparing `zeroconf-0.57.0/src/zeroconf/_dns.py` & `zeroconf-0.58.0/src/zeroconf/_dns.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.57.0/src/zeroconf/_exceptions.py` & `zeroconf-0.58.0/src/zeroconf/_exceptions.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.57.0/src/zeroconf/_handlers.py` & `zeroconf-0.58.0/src/zeroconf/_handlers.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.57.0/src/zeroconf/_history.py` & `zeroconf-0.58.0/src/zeroconf/_history.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.57.0/src/zeroconf/_logger.py` & `zeroconf-0.58.0/src/zeroconf/_logger.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.57.0/src/zeroconf/_protocol/__init__.py` & `zeroconf-0.58.0/src/zeroconf/_protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.57.0/src/zeroconf/_protocol/incoming.pxd` & `zeroconf-0.58.0/src/zeroconf/_protocol/incoming.pxd`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 
 cdef cython.uint DNS_COMPRESSION_HEADER_LEN
 cdef cython.uint MAX_DNS_LABELS
 cdef cython.uint DNS_COMPRESSION_POINTER_LEN
 cdef cython.uint MAX_NAME_LENGTH
 
+cdef object current_time_millis
 
 cdef cython.uint _TYPE_A
 cdef cython.uint _TYPE_CNAME
 cdef cython.uint _TYPE_PTR
 cdef cython.uint _TYPE_TXT
 cdef cython.uint _TYPE_SRV
 cdef cython.uint _TYPE_HINFO
@@ -27,14 +28,26 @@
 cdef object UNPACK_HH
 cdef object UNPACK_HHiH
 
 cdef object DECODE_EXCEPTIONS
 
 cdef object IncomingDecodeError
 
+from .._dns cimport (
+    DNSAddress,
+    DNSEntry,
+    DNSHinfo,
+    DNSNsec,
+    DNSPointer,
+    DNSRecord,
+    DNSService,
+    DNSText,
+)
+
+
 cdef class DNSIncoming:
 
     cdef bint _did_read_others
     cdef public unsigned int flags
     cdef object offset
     cdef public bytes data
     cdef unsigned int _data_len
@@ -60,14 +73,16 @@
     )
     cdef _decode_labels_at_offset(self, unsigned int off, cython.list labels, cython.set seen_pointers)
 
     cdef _read_header(self)
 
     cdef _initial_parse(self)
 
+    cdef _unpack(self, object unpacker, object length)
+
     @cython.locals(
         end=cython.uint,
         length=cython.uint
     )
     cdef _read_others(self)
 
     cdef _read_questions(self)
```

### Comparing `zeroconf-0.57.0/src/zeroconf/_protocol/incoming.py` & `zeroconf-0.58.0/src/zeroconf/_protocol/incoming.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.57.0/src/zeroconf/_protocol/outgoing.pxd` & `zeroconf-0.58.0/src/zeroconf/_protocol/outgoing.pxd`

 * *Files identical despite different names*

### Comparing `zeroconf-0.57.0/src/zeroconf/_protocol/outgoing.py` & `zeroconf-0.58.0/src/zeroconf/_protocol/outgoing.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.57.0/src/zeroconf/_services/__init__.py` & `zeroconf-0.58.0/src/zeroconf/_services/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.57.0/src/zeroconf/_services/browser.py` & `zeroconf-0.58.0/src/zeroconf/_services/browser.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.57.0/src/zeroconf/_services/info.py` & `zeroconf-0.58.0/src/zeroconf/_services/info.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.57.0/src/zeroconf/_services/registry.py` & `zeroconf-0.58.0/src/zeroconf/_services/registry.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.57.0/src/zeroconf/_services/types.py` & `zeroconf-0.58.0/src/zeroconf/_services/types.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.57.0/src/zeroconf/_updates.py` & `zeroconf-0.58.0/src/zeroconf/_updates.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.57.0/src/zeroconf/_utils/__init__.py` & `zeroconf-0.58.0/src/zeroconf/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.57.0/src/zeroconf/_utils/asyncio.py` & `zeroconf-0.58.0/src/zeroconf/_utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.57.0/src/zeroconf/_utils/name.py` & `zeroconf-0.58.0/src/zeroconf/_utils/name.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.57.0/src/zeroconf/_utils/net.py` & `zeroconf-0.58.0/src/zeroconf/_utils/net.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.57.0/src/zeroconf/_utils/time.py` & `zeroconf-0.58.0/src/zeroconf/_utils/time.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.57.0/src/zeroconf/asyncio.py` & `zeroconf-0.58.0/src/zeroconf/asyncio.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.57.0/src/zeroconf/const.py` & `zeroconf-0.58.0/src/zeroconf/const.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.57.0/tests/__init__.py` & `zeroconf-0.58.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.57.0/tests/conftest.py` & `zeroconf-0.58.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.57.0/tests/services/__init__.py` & `zeroconf-0.58.0/tests/services/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.57.0/tests/services/test_browser.py` & `zeroconf-0.58.0/tests/services/test_browser.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.57.0/tests/services/test_info.py` & `zeroconf-0.58.0/tests/services/test_info.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.57.0/tests/services/test_registry.py` & `zeroconf-0.58.0/tests/services/test_registry.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.57.0/tests/services/test_types.py` & `zeroconf-0.58.0/tests/services/test_types.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.57.0/tests/test_asyncio.py` & `zeroconf-0.58.0/tests/test_asyncio.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.57.0/tests/test_cache.py` & `zeroconf-0.58.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.57.0/tests/test_core.py` & `zeroconf-0.58.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.57.0/tests/test_dns.py` & `zeroconf-0.58.0/tests/test_dns.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.57.0/tests/test_exceptions.py` & `zeroconf-0.58.0/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.57.0/tests/test_handlers.py` & `zeroconf-0.58.0/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.57.0/tests/test_history.py` & `zeroconf-0.58.0/tests/test_history.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.57.0/tests/test_init.py` & `zeroconf-0.58.0/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.57.0/tests/test_logger.py` & `zeroconf-0.58.0/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.57.0/tests/test_protocol.py` & `zeroconf-0.58.0/tests/test_protocol.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.57.0/tests/test_services.py` & `zeroconf-0.58.0/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.57.0/tests/test_updates.py` & `zeroconf-0.58.0/tests/test_updates.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.57.0/tests/utils/__init__.py` & `zeroconf-0.58.0/tests/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.57.0/tests/utils/test_asyncio.py` & `zeroconf-0.58.0/tests/utils/test_asyncio.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.57.0/tests/utils/test_name.py` & `zeroconf-0.58.0/tests/utils/test_name.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.57.0/tests/utils/test_net.py` & `zeroconf-0.58.0/tests/utils/test_net.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.57.0/setup.py` & `zeroconf-0.58.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ['ifaddr>=0.1.7']
 
 extras_require = \
 {':python_version < "3.11"': ['async-timeout>=3.0.0']}
 
 setup_kwargs = {
     'name': 'zeroconf',
-    'version': '0.57.0',
+    'version': '0.58.0',
     'description': 'A pure python implementation of multicast DNS service discovery',
     'long_description': 'python-zeroconf\n===============\n\n.. image:: https://github.com/python-zeroconf/python-zeroconf/workflows/CI/badge.svg\n   :target: https://github.com/python-zeroconf/python-zeroconf?query=workflow%3ACI+branch%3Amaster\n\n.. image:: https://img.shields.io/pypi/v/zeroconf.svg\n    :target: https://pypi.python.org/pypi/zeroconf\n\n.. image:: https://codecov.io/gh/python-zeroconf/python-zeroconf/branch/master/graph/badge.svg\n   :target: https://codecov.io/gh/python-zeroconf/python-zeroconf\n\n`Documentation <https://python-zeroconf.readthedocs.io/en/latest/>`_.\n\nThis is fork of pyzeroconf, Multicast DNS Service Discovery for Python,\noriginally by Paul Scott-Murphy (https://github.com/paulsm/pyzeroconf),\nmodified by William McBrine (https://github.com/wmcbrine/pyzeroconf).\n\nThe original William McBrine\'s fork note::\n\n    This fork is used in all of my TiVo-related projects: HME for Python\n    (and therefore HME/VLC), Network Remote, Remote Proxy, and pyTivo.\n    Before this, I was tracking the changes for zeroconf.py in three\n    separate repos. I figured I should have an authoritative source.\n\n    Although I make changes based on my experience with TiVos, I expect that\n    they\'re generally applicable. This version also includes patches found\n    on the now-defunct (?) Launchpad repo of pyzeroconf, and elsewhere\n    around the net -- not always well-documented, sorry.\n\nCompatible with:\n\n* Bonjour\n* Avahi\n\nCompared to some other Zeroconf/Bonjour/Avahi Python packages, python-zeroconf:\n\n* isn\'t tied to Bonjour or Avahi\n* doesn\'t use D-Bus\n* doesn\'t force you to use particular event loop or Twisted (asyncio is used under the hood but not required)\n* is pip-installable\n* has PyPI distribution\n* has an optional cython extension for performance (pure python is supported as well)\n\nPython compatibility\n--------------------\n\n* CPython 3.7+\n* PyPy3.7 7.3+\n\nVersioning\n----------\n\nThis project uses semantic versioning.\n\nStatus\n------\n\nThis project is actively maintained.\n\nTraffic Reduction\n-----------------\n\nBefore version 0.32, most traffic reduction techniques described in https://datatracker.ietf.org/doc/html/rfc6762#section-7\nwhere not implemented which could lead to excessive network traffic.  It is highly recommended that version 0.32 or later\nis used if this is a concern.\n\nIPv6 support\n------------\n\nIPv6 support is relatively new and currently limited, specifically:\n\n* `InterfaceChoice.All` is an alias for `InterfaceChoice.Default` on non-POSIX\n  systems.\n* Dual-stack IPv6 sockets are used, which may not be supported everywhere (some\n  BSD variants do not have them).\n* Listening on localhost (`::1`) does not work. Help with understanding why is\n  appreciated.\n\nHow to get python-zeroconf?\n===========================\n\n* PyPI page https://pypi.org/project/zeroconf/\n* GitHub project https://github.com/python-zeroconf/python-zeroconf\n\nThe easiest way to install python-zeroconf is using pip::\n\n    pip install zeroconf\n\n\n\nHow do I use it?\n================\n\nHere\'s an example of browsing for a service:\n\n.. code-block:: python\n\n    from zeroconf import ServiceBrowser, ServiceListener, Zeroconf\n\n\n    class MyListener(ServiceListener):\n\n        def update_service(self, zc: Zeroconf, type_: str, name: str) -> None:\n            print(f"Service {name} updated")\n\n        def remove_service(self, zc: Zeroconf, type_: str, name: str) -> None:\n            print(f"Service {name} removed")\n\n        def add_service(self, zc: Zeroconf, type_: str, name: str) -> None:\n            info = zc.get_service_info(type_, name)\n            print(f"Service {name} added, service info: {info}")\n\n\n    zeroconf = Zeroconf()\n    listener = MyListener()\n    browser = ServiceBrowser(zeroconf, "_http._tcp.local.", listener)\n    try:\n        input("Press enter to exit...\\n\\n")\n    finally:\n        zeroconf.close()\n\n.. note::\n\n    Discovery and service registration use *all* available network interfaces by default.\n    If you want to customize that you need to specify ``interfaces`` argument when\n    constructing ``Zeroconf`` object (see the code for details).\n\nIf you don\'t know the name of the service you need to browse for, try:\n\n.. code-block:: python\n\n    from zeroconf import ZeroconfServiceTypes\n    print(\'\\n\'.join(ZeroconfServiceTypes.find()))\n\nSee examples directory for more.\n\nChangelog\n=========\n\n`Changelog <CHANGELOG.md>`_\n\nLicense\n=======\n\nLGPL, see COPYING file for details.\n',
     'author': 'Paul Scott-Murphy',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/python-zeroconf/python-zeroconf',
```

### Comparing `zeroconf-0.57.0/PKG-INFO` & `zeroconf-0.58.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeroconf
-Version: 0.57.0
+Version: 0.58.0
 Summary: A pure python implementation of multicast DNS service discovery
 Home-page: https://github.com/python-zeroconf/python-zeroconf
 License: LGPL
 Author: Paul Scott-Murphy
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

