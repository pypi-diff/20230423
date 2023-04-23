# Comparing `tmp/bitmex_websocket-0.3.2.tar.gz` & `tmp/bitmex_websocket-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitmex_websocket-0.3.2.tar", last modified: Sun Apr 23 00:08:21 2023, max compression
+gzip compressed data, was "bitmex_websocket-0.3.5.tar", last modified: Sun Apr 23 00:34:22 2023, max compression
```

## Comparing `bitmex_websocket-0.3.2.tar` & `bitmex_websocket-0.3.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 joliveros  (1000) joliveros  (1000)        0 2023-04-23 00:08:21.474701 bitmex_websocket-0.3.2/
--rw-rw-r--   0 joliveros  (1000) joliveros  (1000)        5 2023-04-22 23:17:52.000000 bitmex_websocket-0.3.2/.version
--rw-r--r--   0 joliveros  (1000) joliveros  (1000)     1076 2020-04-20 15:54:16.000000 bitmex_websocket-0.3.2/LICENSE
--rw-r--r--   0 joliveros  (1000) joliveros  (1000)       31 2020-04-20 15:54:16.000000 bitmex_websocket-0.3.2/MANIFEST.in
--rw-rw-r--   0 joliveros  (1000) joliveros  (1000)     3205 2023-04-23 00:08:21.474701 bitmex_websocket-0.3.2/PKG-INFO
--rw-rw-r--   0 joliveros  (1000) joliveros  (1000)     1299 2023-04-22 23:05:56.000000 bitmex_websocket-0.3.2/README.rst
-drwxrwxr-x   0 joliveros  (1000) joliveros  (1000)        0 2023-04-23 00:08:21.470701 bitmex_websocket-0.3.2/bitmex_websocket/
--rw-rw-r--   0 joliveros  (1000) joliveros  (1000)      124 2023-04-22 23:05:56.000000 bitmex_websocket-0.3.2/bitmex_websocket/__init__.py
--rw-rw-r--   0 joliveros  (1000) joliveros  (1000)     4296 2023-04-22 23:10:42.000000 bitmex_websocket-0.3.2/bitmex_websocket/_bitmex_websocket.py
--rwxrwxr-x   0 joliveros  (1000) joliveros  (1000)     1989 2023-04-22 23:05:56.000000 bitmex_websocket-0.3.2/bitmex_websocket/_instrument.py
--rw-rw-r--   0 joliveros  (1000) joliveros  (1000)      481 2023-04-22 23:05:56.000000 bitmex_websocket-0.3.2/bitmex_websocket/_settings_base.py
-drwxrwxr-x   0 joliveros  (1000) joliveros  (1000)        0 2023-04-23 00:08:21.470701 bitmex_websocket-0.3.2/bitmex_websocket/auth/
--rw-rw-r--   0 joliveros  (1000) joliveros  (1000)       61 2023-04-22 23:05:56.000000 bitmex_websocket-0.3.2/bitmex_websocket/auth/__init__.py
--rw-rw-r--   0 joliveros  (1000) joliveros  (1000)     2082 2023-04-22 23:05:56.000000 bitmex_websocket-0.3.2/bitmex_websocket/auth/api_key_auth.py
--rw-rw-r--   0 joliveros  (1000) joliveros  (1000)     1902 2023-04-22 23:05:56.000000 bitmex_websocket-0.3.2/bitmex_websocket/constants.py
--rw-rw-r--   0 joliveros  (1000) joliveros  (1000)       80 2023-04-22 23:05:56.000000 bitmex_websocket-0.3.2/bitmex_websocket/settings.py
-drwxrwxr-x   0 joliveros  (1000) joliveros  (1000)        0 2023-04-23 00:08:21.470701 bitmex_websocket-0.3.2/bitmex_websocket.egg-info/
--rw-rw-r--   0 joliveros  (1000) joliveros  (1000)     3205 2023-04-23 00:08:21.000000 bitmex_websocket-0.3.2/bitmex_websocket.egg-info/PKG-INFO
--rw-rw-r--   0 joliveros  (1000) joliveros  (1000)      660 2023-04-23 00:08:21.000000 bitmex_websocket-0.3.2/bitmex_websocket.egg-info/SOURCES.txt
--rw-rw-r--   0 joliveros  (1000) joliveros  (1000)        1 2023-04-23 00:08:21.000000 bitmex_websocket-0.3.2/bitmex_websocket.egg-info/dependency_links.txt
--rw-rw-r--   0 joliveros  (1000) joliveros  (1000)      731 2023-04-23 00:08:21.000000 bitmex_websocket-0.3.2/bitmex_websocket.egg-info/requires.txt
--rw-rw-r--   0 joliveros  (1000) joliveros  (1000)       17 2023-04-23 00:08:21.000000 bitmex_websocket-0.3.2/bitmex_websocket.egg-info/top_level.txt
--rw-rw-r--   0 joliveros  (1000) joliveros  (1000)        1 2023-04-22 23:28:45.000000 bitmex_websocket-0.3.2/bitmex_websocket.egg-info/zip-safe
--rw-rw-r--   0 joliveros  (1000) joliveros  (1000)      717 2023-04-23 00:07:32.000000 bitmex_websocket-0.3.2/pyproject.toml
--rw-r--r--   0 joliveros  (1000) joliveros  (1000)       41 2020-04-20 15:54:16.000000 bitmex_websocket-0.3.2/requirements-test.txt
--rw-rw-r--   0 joliveros  (1000) joliveros  (1000)      731 2023-04-23 00:07:04.000000 bitmex_websocket-0.3.2/requirements.txt
--rw-r--r--   0 joliveros  (1000) joliveros  (1000)       67 2023-04-23 00:08:21.474701 bitmex_websocket-0.3.2/setup.cfg
--rwxrwxr-x   0 joliveros  (1000) joliveros  (1000)     1167 2023-04-22 23:58:26.000000 bitmex_websocket-0.3.2/setup.py
-drwxrwxr-x   0 joliveros  (1000) joliveros  (1000)        0 2023-04-23 00:08:21.474701 bitmex_websocket-0.3.2/tests/
--rw-r--r--   0 joliveros  (1000) joliveros  (1000)     2865 2020-04-20 15:54:16.000000 bitmex_websocket-0.3.2/tests/test_instrument.py
--rw-rw-r--   0 joliveros  (1000) joliveros  (1000)     2728 2023-04-22 23:05:56.000000 bitmex_websocket-0.3.2/tests/test_websocket.py
+drwxrwxr-x   0 joliveros  (1000) joliveros  (1000)        0 2023-04-23 00:34:22.489159 bitmex_websocket-0.3.5/
+-rw-rw-r--   0 joliveros  (1000) joliveros  (1000)        5 2023-04-22 23:17:52.000000 bitmex_websocket-0.3.5/.version
+-rw-r--r--   0 joliveros  (1000) joliveros  (1000)     1076 2020-04-20 15:54:16.000000 bitmex_websocket-0.3.5/LICENSE
+-rw-r--r--   0 joliveros  (1000) joliveros  (1000)       31 2020-04-20 15:54:16.000000 bitmex_websocket-0.3.5/MANIFEST.in
+-rw-rw-r--   0 joliveros  (1000) joliveros  (1000)     3349 2023-04-23 00:34:22.489159 bitmex_websocket-0.3.5/PKG-INFO
+-rw-rw-r--   0 joliveros  (1000) joliveros  (1000)     1443 2023-04-23 00:34:08.000000 bitmex_websocket-0.3.5/README.rst
+drwxrwxr-x   0 joliveros  (1000) joliveros  (1000)        0 2023-04-23 00:34:22.485159 bitmex_websocket-0.3.5/bitmex_websocket/
+-rw-rw-r--   0 joliveros  (1000) joliveros  (1000)      124 2023-04-22 23:05:56.000000 bitmex_websocket-0.3.5/bitmex_websocket/__init__.py
+-rw-rw-r--   0 joliveros  (1000) joliveros  (1000)     4296 2023-04-22 23:10:42.000000 bitmex_websocket-0.3.5/bitmex_websocket/_bitmex_websocket.py
+-rwxrwxr-x   0 joliveros  (1000) joliveros  (1000)     1989 2023-04-22 23:05:56.000000 bitmex_websocket-0.3.5/bitmex_websocket/_instrument.py
+-rw-rw-r--   0 joliveros  (1000) joliveros  (1000)      517 2023-04-23 00:28:30.000000 bitmex_websocket-0.3.5/bitmex_websocket/_settings_base.py
+drwxrwxr-x   0 joliveros  (1000) joliveros  (1000)        0 2023-04-23 00:34:22.489159 bitmex_websocket-0.3.5/bitmex_websocket/auth/
+-rw-rw-r--   0 joliveros  (1000) joliveros  (1000)       61 2023-04-22 23:05:56.000000 bitmex_websocket-0.3.5/bitmex_websocket/auth/__init__.py
+-rw-rw-r--   0 joliveros  (1000) joliveros  (1000)     2082 2023-04-22 23:05:56.000000 bitmex_websocket-0.3.5/bitmex_websocket/auth/api_key_auth.py
+-rw-rw-r--   0 joliveros  (1000) joliveros  (1000)     1902 2023-04-22 23:05:56.000000 bitmex_websocket-0.3.5/bitmex_websocket/constants.py
+-rw-rw-r--   0 joliveros  (1000) joliveros  (1000)       80 2023-04-22 23:05:56.000000 bitmex_websocket-0.3.5/bitmex_websocket/settings.py
+drwxrwxr-x   0 joliveros  (1000) joliveros  (1000)        0 2023-04-23 00:34:22.485159 bitmex_websocket-0.3.5/bitmex_websocket.egg-info/
+-rw-rw-r--   0 joliveros  (1000) joliveros  (1000)     3349 2023-04-23 00:34:22.000000 bitmex_websocket-0.3.5/bitmex_websocket.egg-info/PKG-INFO
+-rw-rw-r--   0 joliveros  (1000) joliveros  (1000)      660 2023-04-23 00:34:22.000000 bitmex_websocket-0.3.5/bitmex_websocket.egg-info/SOURCES.txt
+-rw-rw-r--   0 joliveros  (1000) joliveros  (1000)        1 2023-04-23 00:34:22.000000 bitmex_websocket-0.3.5/bitmex_websocket.egg-info/dependency_links.txt
+-rw-rw-r--   0 joliveros  (1000) joliveros  (1000)      695 2023-04-23 00:34:22.000000 bitmex_websocket-0.3.5/bitmex_websocket.egg-info/requires.txt
+-rw-rw-r--   0 joliveros  (1000) joliveros  (1000)       17 2023-04-23 00:34:22.000000 bitmex_websocket-0.3.5/bitmex_websocket.egg-info/top_level.txt
+-rw-rw-r--   0 joliveros  (1000) joliveros  (1000)        1 2023-04-22 23:28:45.000000 bitmex_websocket-0.3.5/bitmex_websocket.egg-info/zip-safe
+-rw-rw-r--   0 joliveros  (1000) joliveros  (1000)      717 2023-04-23 00:34:03.000000 bitmex_websocket-0.3.5/pyproject.toml
+-rw-r--r--   0 joliveros  (1000) joliveros  (1000)       41 2020-04-20 15:54:16.000000 bitmex_websocket-0.3.5/requirements-test.txt
+-rw-rw-r--   0 joliveros  (1000) joliveros  (1000)      695 2023-04-23 00:29:10.000000 bitmex_websocket-0.3.5/requirements.txt
+-rw-r--r--   0 joliveros  (1000) joliveros  (1000)       67 2023-04-23 00:34:22.489159 bitmex_websocket-0.3.5/setup.cfg
+-rwxrwxr-x   0 joliveros  (1000) joliveros  (1000)     1167 2023-04-22 23:58:26.000000 bitmex_websocket-0.3.5/setup.py
+drwxrwxr-x   0 joliveros  (1000) joliveros  (1000)        0 2023-04-23 00:34:22.489159 bitmex_websocket-0.3.5/tests/
+-rw-r--r--   0 joliveros  (1000) joliveros  (1000)     2865 2020-04-20 15:54:16.000000 bitmex_websocket-0.3.5/tests/test_instrument.py
+-rw-rw-r--   0 joliveros  (1000) joliveros  (1000)     2728 2023-04-22 23:05:56.000000 bitmex_websocket-0.3.5/tests/test_websocket.py
```

### Comparing `bitmex_websocket-0.3.2/LICENSE` & `bitmex_websocket-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bitmex_websocket-0.3.2/PKG-INFO` & `bitmex_websocket-0.3.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitmex_websocket
-Version: 0.3.2
+Version: 0.3.5
 Summary: Bitmex websocket API
 Home-page: https://github.com/joliveros/bitmex-websocket
 Author: José Oliveros
 Author-email: Jose Oliveros <jose.oliveros.1983@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2019 joliveros
@@ -75,27 +75,36 @@
         InstrumentChannels.quote,
         InstrumentChannels.trade,
         InstrumentChannels.orderBookL2
     ]
 
     XBTUSD = Instrument(symbol='XBTUSD',
                         channels=channels)
-    XBTUSD.on('action', lambda msg: print(message))
+    XBTUSD.on('action', lambda msg: print(msg))
 
     XBTUSD.run_forever()
 
+TestNet
+--------
+
+You may change the `BASE_URL` by setting the `BITMEX_BASE_URL` environment variable to:
+`https://testnet.bitmex.com/api/v1/`.
+
+
+
 Examples
 --------
 
 Run example scripts:
 
 .. code-block:: sh
 
     $ ./examples/example.py
 
+
 Tests
 -----
 
 Testing is set up using `pytest <http://pytest.org>` and coverage is handled
 with the pytest-cov plugin.
 
 Run your tests with `pytest` in the root directory.
```

### Comparing `bitmex_websocket-0.3.2/README.rst` & `bitmex_websocket-0.3.5/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -36,27 +36,36 @@
         InstrumentChannels.quote,
         InstrumentChannels.trade,
         InstrumentChannels.orderBookL2
     ]
 
     XBTUSD = Instrument(symbol='XBTUSD',
                         channels=channels)
-    XBTUSD.on('action', lambda msg: print(message))
+    XBTUSD.on('action', lambda msg: print(msg))
 
     XBTUSD.run_forever()
 
+TestNet
+--------
+
+You may change the `BASE_URL` by setting the `BITMEX_BASE_URL` environment variable to:
+`https://testnet.bitmex.com/api/v1/`.
+
+
+
 Examples
 --------
 
 Run example scripts:
 
 .. code-block:: sh
 
     $ ./examples/example.py
 
+
 Tests
 -----
 
 Testing is set up using `pytest <http://pytest.org>` and coverage is handled
 with the pytest-cov plugin.
 
 Run your tests with `pytest` in the root directory.
```

### Comparing `bitmex_websocket-0.3.2/bitmex_websocket/_bitmex_websocket.py` & `bitmex_websocket-0.3.5/bitmex_websocket/_bitmex_websocket.py`

 * *Files identical despite different names*

### Comparing `bitmex_websocket-0.3.2/bitmex_websocket/_instrument.py` & `bitmex_websocket-0.3.5/bitmex_websocket/_instrument.py`

 * *Files identical despite different names*

### Comparing `bitmex_websocket-0.3.2/bitmex_websocket/auth/api_key_auth.py` & `bitmex_websocket-0.3.5/bitmex_websocket/auth/api_key_auth.py`

 * *Files identical despite different names*

### Comparing `bitmex_websocket-0.3.2/bitmex_websocket/constants.py` & `bitmex_websocket-0.3.5/bitmex_websocket/constants.py`

 * *Files identical despite different names*

### Comparing `bitmex_websocket-0.3.2/bitmex_websocket.egg-info/PKG-INFO` & `bitmex_websocket-0.3.5/bitmex_websocket.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitmex-websocket
-Version: 0.3.2
+Version: 0.3.5
 Summary: Bitmex websocket API
 Home-page: https://github.com/joliveros/bitmex-websocket
 Author: José Oliveros
 Author-email: Jose Oliveros <jose.oliveros.1983@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2019 joliveros
@@ -75,27 +75,36 @@
         InstrumentChannels.quote,
         InstrumentChannels.trade,
         InstrumentChannels.orderBookL2
     ]
 
     XBTUSD = Instrument(symbol='XBTUSD',
                         channels=channels)
-    XBTUSD.on('action', lambda msg: print(message))
+    XBTUSD.on('action', lambda msg: print(msg))
 
     XBTUSD.run_forever()
 
+TestNet
+--------
+
+You may change the `BASE_URL` by setting the `BITMEX_BASE_URL` environment variable to:
+`https://testnet.bitmex.com/api/v1/`.
+
+
+
 Examples
 --------
 
 Run example scripts:
 
 .. code-block:: sh
 
     $ ./examples/example.py
 
+
 Tests
 -----
 
 Testing is set up using `pytest <http://pytest.org>` and coverage is handled
 with the pytest-cov plugin.
 
 Run your tests with `pytest` in the root directory.
```

### Comparing `bitmex_websocket-0.3.2/bitmex_websocket.egg-info/SOURCES.txt` & `bitmex_websocket-0.3.5/bitmex_websocket.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bitmex_websocket-0.3.2/bitmex_websocket.egg-info/requires.txt` & `bitmex_websocket-0.3.5/bitmex_websocket.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 alog==1.2.0
-bitmex-websocket==0.3.1
 bleach==6.0.0
 build==0.10.0
 certifi==2022.12.7
 cffi==1.15.1
 charset-normalizer==3.1.0
 click==8.1.3
 cryptography==40.0.2
@@ -13,29 +12,28 @@
 jaraco.classes==3.2.3
 jeepney==0.8.0
 keyring==23.13.1
 markdown-it-py==2.2.0
 mdurl==0.1.2
 more-itertools==9.1.0
 packaging==23.1
-pip==22.3.1
 pipfreeze==2.0.3
 pkginfo==1.9.6
 pycparser==2.21
 pyee==9.0.4
 Pygments==2.15.1
 pyproject_hooks==1.0.0
 readme-renderer==37.3
 requests==2.28.2
 requests-toolbelt==0.10.1
 rfc3986==2.0.0
 rich==13.3.4
 SecretStorage==3.3.3
 semver==3.0.0
-setuptools==65.5.0
+setuptools==65.5.1
 six==1.16.0
 twine==4.0.2
 typing_extensions==4.5.0
 urllib3==1.26.15
 webencodings==0.5.1
 websocket-client==1.5.1
 wheel==0.40.0
```

### Comparing `bitmex_websocket-0.3.2/pyproject.toml` & `bitmex_websocket-0.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bitmex_websocket"
-version = "0.3.2"
+version = "0.3.5"
 authors = [
   { name="Jose Oliveros", email="jose.oliveros.1983@gmail.com" },
 ]
 description = "Bitmex websocket API"
 readme = "README.rst"
 requires-python = ">=3.7"
 dynamic=["dependencies"]
```

### Comparing `bitmex_websocket-0.3.2/requirements.txt` & `bitmex_websocket-0.3.5/requirements.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 alog==1.2.0
-bitmex-websocket==0.3.1
 bleach==6.0.0
 build==0.10.0
 certifi==2022.12.7
 cffi==1.15.1
 charset-normalizer==3.1.0
 click==8.1.3
 cryptography==40.0.2
@@ -13,29 +12,28 @@
 jaraco.classes==3.2.3
 jeepney==0.8.0
 keyring==23.13.1
 markdown-it-py==2.2.0
 mdurl==0.1.2
 more-itertools==9.1.0
 packaging==23.1
-pip==22.3.1
 pipfreeze==2.0.3
 pkginfo==1.9.6
 pycparser==2.21
 pyee==9.0.4
 Pygments==2.15.1
 pyproject_hooks==1.0.0
 readme-renderer==37.3
 requests==2.28.2
 requests-toolbelt==0.10.1
 rfc3986==2.0.0
 rich==13.3.4
 SecretStorage==3.3.3
 semver==3.0.0
-setuptools==65.5.0
+setuptools==65.5.1
 six==1.16.0
 twine==4.0.2
 typing_extensions==4.5.0
 urllib3==1.26.15
 webencodings==0.5.1
 websocket-client==1.5.1
 wheel==0.40.0
```

### Comparing `bitmex_websocket-0.3.2/setup.py` & `bitmex_websocket-0.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `bitmex_websocket-0.3.2/tests/test_instrument.py` & `bitmex_websocket-0.3.5/tests/test_instrument.py`

 * *Files identical despite different names*

### Comparing `bitmex_websocket-0.3.2/tests/test_websocket.py` & `bitmex_websocket-0.3.5/tests/test_websocket.py`

 * *Files identical despite different names*

