# Comparing `tmp/pysasl-1.0.1.tar.gz` & `tmp/pysasl-1.0.2.tar.gz`

## Comparing `pysasl-1.0.1.tar` & `pysasl-1.0.2.tar`

### file list

```diff
@@ -1,33 +1,32 @@
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 pysasl-1.0.1/.flake8
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 pysasl-1.0.1/importlib_metadata.pyi
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pysasl-1.0.1/requirements-all.txt
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pysasl-1.0.1/requirements-dev.txt
--rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 pysasl-1.0.1/pysasl/__init__.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pysasl-1.0.1/pysasl/config.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 pysasl-1.0.1/pysasl/exception.py
--rw-r--r--   0        0        0     8051 2020-02-02 00:00:00.000000 pysasl-1.0.1/pysasl/hashing.py
--rw-r--r--   0        0        0     4453 2020-02-02 00:00:00.000000 pysasl-1.0.1/pysasl/identity.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 pysasl-1.0.1/pysasl/prep.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pysasl-1.0.1/pysasl/py.typed
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 pysasl-1.0.1/pysasl/creds/__init__.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 pysasl-1.0.1/pysasl/creds/client.py
--rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 pysasl-1.0.1/pysasl/creds/external.py
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 pysasl-1.0.1/pysasl/creds/plain.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 pysasl-1.0.1/pysasl/creds/server.py
--rw-r--r--   0        0        0     4841 2020-02-02 00:00:00.000000 pysasl-1.0.1/pysasl/mechanism/__init__.py
--rw-r--r--   0        0        0     3904 2020-02-02 00:00:00.000000 pysasl-1.0.1/pysasl/mechanism/crammd5.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 pysasl-1.0.1/pysasl/mechanism/external.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 pysasl-1.0.1/pysasl/mechanism/login.py
--rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 pysasl-1.0.1/pysasl/mechanism/oauth.py
--rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 pysasl-1.0.1/pysasl/mechanism/plain.py
--rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 pysasl-1.0.1/test/test_crammd5.py
--rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 pysasl-1.0.1/test/test_creds.py
--rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 pysasl-1.0.1/test/test_external.py
--rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 pysasl-1.0.1/test/test_login.py
--rw-r--r--   0        0        0     3471 2020-02-02 00:00:00.000000 pysasl-1.0.1/test/test_oauth.py
--rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 pysasl-1.0.1/test/test_plain.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 pysasl-1.0.1/.gitignore
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 pysasl-1.0.1/LICENSE.md
--rw-r--r--   0        0        0     6198 2020-02-02 00:00:00.000000 pysasl-1.0.1/README.md
--rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 pysasl-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     8392 2020-02-02 00:00:00.000000 pysasl-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 pysasl-1.0.2/.flake8
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 pysasl-1.0.2/importlib_metadata.pyi
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pysasl-1.0.2/pysasl/__about__.py
+-rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 pysasl-1.0.2/pysasl/__init__.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pysasl-1.0.2/pysasl/config.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 pysasl-1.0.2/pysasl/exception.py
+-rw-r--r--   0        0        0     8051 2020-02-02 00:00:00.000000 pysasl-1.0.2/pysasl/hashing.py
+-rw-r--r--   0        0        0     4453 2020-02-02 00:00:00.000000 pysasl-1.0.2/pysasl/identity.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 pysasl-1.0.2/pysasl/prep.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pysasl-1.0.2/pysasl/py.typed
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 pysasl-1.0.2/pysasl/creds/__init__.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 pysasl-1.0.2/pysasl/creds/client.py
+-rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 pysasl-1.0.2/pysasl/creds/external.py
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 pysasl-1.0.2/pysasl/creds/plain.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 pysasl-1.0.2/pysasl/creds/server.py
+-rw-r--r--   0        0        0     4841 2020-02-02 00:00:00.000000 pysasl-1.0.2/pysasl/mechanism/__init__.py
+-rw-r--r--   0        0        0     3904 2020-02-02 00:00:00.000000 pysasl-1.0.2/pysasl/mechanism/crammd5.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 pysasl-1.0.2/pysasl/mechanism/external.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 pysasl-1.0.2/pysasl/mechanism/login.py
+-rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 pysasl-1.0.2/pysasl/mechanism/oauth.py
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 pysasl-1.0.2/pysasl/mechanism/plain.py
+-rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 pysasl-1.0.2/test/test_crammd5.py
+-rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 pysasl-1.0.2/test/test_creds.py
+-rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 pysasl-1.0.2/test/test_external.py
+-rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 pysasl-1.0.2/test/test_login.py
+-rw-r--r--   0        0        0     3471 2020-02-02 00:00:00.000000 pysasl-1.0.2/test/test_oauth.py
+-rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 pysasl-1.0.2/test/test_plain.py
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 pysasl-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 pysasl-1.0.2/LICENSE.md
+-rw-r--r--   0        0        0     6217 2020-02-02 00:00:00.000000 pysasl-1.0.2/README.md
+-rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 pysasl-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     8476 2020-02-02 00:00:00.000000 pysasl-1.0.2/PKG-INFO
```

### Comparing `pysasl-1.0.1/pysasl/__init__.py` & `pysasl-1.0.2/pysasl/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 
 import sys
 from collections import OrderedDict
 from typing import Iterable, Optional, Sequence
 from typing_extensions import Final, Self
 
 if sys.version_info >= (3, 10):  # pragma: no cover
-    from importlib.metadata import distribution, entry_points
+    from importlib.metadata import entry_points
 else:  # pragma: no cover
-    from importlib_metadata import distribution, entry_points
+    from importlib_metadata import entry_points
 
 from . import mechanism
+from .__about__ import __version__
 from .config import default_config, SASLConfig
 from .mechanism import Mechanism, ServerMechanism, ClientMechanism
 
 __all__ = ['__version__', 'SASLAuth']
 
-#: The pysasl package version.
-__version__: str = distribution(__package__).version
-
 
 class SASLAuth(SASLConfig):
     """Manages the mechanisms available for authentication attempts.
 
     Args:
         mechanisms: List of available SASL mechanism objects.
         config: The configuration object.
```

### Comparing `pysasl-1.0.1/pysasl/config.py` & `pysasl-1.0.2/pysasl/config.py`

 * *Files identical despite different names*

### Comparing `pysasl-1.0.1/pysasl/exception.py` & `pysasl-1.0.2/pysasl/exception.py`

 * *Files identical despite different names*

### Comparing `pysasl-1.0.1/pysasl/hashing.py` & `pysasl-1.0.2/pysasl/hashing.py`

 * *Files identical despite different names*

### Comparing `pysasl-1.0.1/pysasl/identity.py` & `pysasl-1.0.2/pysasl/identity.py`

 * *Files identical despite different names*

### Comparing `pysasl-1.0.1/pysasl/prep.py` & `pysasl-1.0.2/pysasl/prep.py`

 * *Files identical despite different names*

### Comparing `pysasl-1.0.1/pysasl/creds/__init__.py` & `pysasl-1.0.2/pysasl/creds/__init__.py`

 * *Files identical despite different names*

### Comparing `pysasl-1.0.1/pysasl/creds/client.py` & `pysasl-1.0.2/pysasl/creds/client.py`

 * *Files identical despite different names*

### Comparing `pysasl-1.0.1/pysasl/creds/external.py` & `pysasl-1.0.2/pysasl/creds/external.py`

 * *Files identical despite different names*

### Comparing `pysasl-1.0.1/pysasl/creds/plain.py` & `pysasl-1.0.2/pysasl/creds/plain.py`

 * *Files identical despite different names*

### Comparing `pysasl-1.0.1/pysasl/creds/server.py` & `pysasl-1.0.2/pysasl/creds/server.py`

 * *Files identical despite different names*

### Comparing `pysasl-1.0.1/pysasl/mechanism/__init__.py` & `pysasl-1.0.2/pysasl/mechanism/__init__.py`

 * *Files identical despite different names*

### Comparing `pysasl-1.0.1/pysasl/mechanism/crammd5.py` & `pysasl-1.0.2/pysasl/mechanism/crammd5.py`

 * *Files identical despite different names*

### Comparing `pysasl-1.0.1/pysasl/mechanism/external.py` & `pysasl-1.0.2/pysasl/mechanism/external.py`

 * *Files identical despite different names*

### Comparing `pysasl-1.0.1/pysasl/mechanism/login.py` & `pysasl-1.0.2/pysasl/mechanism/login.py`

 * *Files identical despite different names*

### Comparing `pysasl-1.0.1/pysasl/mechanism/oauth.py` & `pysasl-1.0.2/pysasl/mechanism/oauth.py`

 * *Files identical despite different names*

### Comparing `pysasl-1.0.1/pysasl/mechanism/plain.py` & `pysasl-1.0.2/pysasl/mechanism/plain.py`

 * *Files identical despite different names*

### Comparing `pysasl-1.0.1/test/test_crammd5.py` & `pysasl-1.0.2/test/test_crammd5.py`

 * *Files identical despite different names*

### Comparing `pysasl-1.0.1/test/test_creds.py` & `pysasl-1.0.2/test/test_creds.py`

 * *Files identical despite different names*

### Comparing `pysasl-1.0.1/test/test_external.py` & `pysasl-1.0.2/test/test_external.py`

 * *Files identical despite different names*

### Comparing `pysasl-1.0.1/test/test_login.py` & `pysasl-1.0.2/test/test_login.py`

 * *Files identical despite different names*

### Comparing `pysasl-1.0.1/test/test_oauth.py` & `pysasl-1.0.2/test/test_oauth.py`

 * *Files identical despite different names*

### Comparing `pysasl-1.0.1/test/test_plain.py` & `pysasl-1.0.2/test/test_plain.py`

 * *Files identical despite different names*

### Comparing `pysasl-1.0.1/.gitignore` & `pysasl-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pysasl-1.0.1/LICENSE.md` & `pysasl-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pysasl-1.0.1/README.md` & `pysasl-1.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -21,33 +21,26 @@
 #### [API Documentation](https://icgood.github.io/pysasl/)
 
 Installation
 ============
 
 Available in [PyPi](https://pypi.python.org/):
 
-```
-pip install pysasl
+```console
+$ pip install pysasl
 ```
 
 ### Running Tests
 
-Install into a virtual environment:
-
-```
-python3 -m venv .venv
-source .venv/bin/activate
-
-pip install -r requirements-dev.txt
-```
+First, install [Hatch][0]. To run the build checks:
 
-Run the tests and report coverage metrics:
+```console
+$ hatch run check
 
-```
-invoke
+$ hatch run all:check  # to run against all supported Python versions
 ```
 
 Usage
 =====
 
 ## Server-side
 
@@ -194,11 +187,12 @@
 ```
 
 And for client-side, just call `resp = mech.client_attempt(creds, [])`
 to get the initial response before starting the transmission. All
 mechanisms should either return an initial response or an empty string
 when given an empty list for the second argument.
 
+[0]: https://hatch.pypa.io/latest/install/
 [1]: https://icgood.github.io/pysasl/pysasl.html#pysasl.SASLAuth
 [2]: https://icgood.github.io/pysasl/pysasl.creds.html#pysasl.creds.server.ServerCredentials
 [3]: https://tools.ietf.org/html/rfc4954
 [4]: https://tools.ietf.org/html/rfc3501#section-6.2.2
```

### Comparing `pysasl-1.0.1/pyproject.toml` & `pysasl-1.0.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 [build-system]
 requires = ['hatchling']
 build-backend = 'hatchling.build'
 
 [project]
 name = 'pysasl'
-version = '1.0.1'
+dynamic = ['version']
 authors = [
     { name = 'Ian Good', email = 'ian@icgood.net' },
 ]
 description = 'Pure Python SASL client and server library.'
 license = { file = 'LICENSE.md' }
 readme = { file = 'README.md', content-type = 'text/markdown' }
 requires-python = '~=3.7'
@@ -50,41 +50,85 @@
     'importlib-metadata; python_version < "3.10"',
 ]
 
 [project.optional-dependencies]
 hashing = ['passlib']
 
 [project.urls]
-homepage = 'https://github.com/icgood/pysasl/'
+'Homepage' = 'https://github.com/icgood/pysasl/'
+'API Documentation' = 'https://icgood.github.io/pysasl/'
 
 [project.entry-points.'pysasl.mechanism']
 CRAM-MD5 = 'pysasl.mechanism.crammd5:CramMD5Mechanism'
 EXTERNAL = 'pysasl.mechanism.external:ExternalMechanism'
 LOGIN = 'pysasl.mechanism.login:LoginMechanism'
 PLAIN = 'pysasl.mechanism.plain:PlainMechanism'
 XOAUTH2 = 'pysasl.mechanism.oauth:OAuth2Mechanism'
 
+[tool.hatch.version]
+path = 'pysasl/__about__.py'
+
 [tool.hatch.build]
-exclude = ['/tasks', '/doc', '/.github']
+exclude = ['/doc', '/.github']
+
+[tool.hatch.build.targets.wheel]
+packages = ['pysasl']
 
 [tool.mypy]
 strict = true
 files = ['pysasl', 'test']
 
 [[tool.mypy.overrides]]
 module = 'importlib_metadata.*'
 ignore_missing_imports = true
 
 [tool.bandit]
 skips = ['B101']
 
 [tool.pytest.ini_options]
+testpaths = 'test'
 norecursedirs = 'doc'
 
 [tool.coverage.report]
 fail_under = 100
 exclude_lines = [
     'pragma: no cover',
     'NotImplemented',
     '^\s*...\s*$',
     'def __repr__',
 ]
+
+[tool.hatch.envs.default]
+dependencies = [
+    'mypy',
+    'pyright',
+    'pytest',
+    'pytest-cov',
+    'flake8',
+    'flake8-annotations',
+    'flake8-bugbear',
+    'bandit[toml]',
+    'types-passlib',
+]
+features = ['hashing']
+
+[tool.hatch.envs.default.scripts]
+run-pytest = 'py.test --cov-report=term-missing --cov=pysasl'
+run-mypy = 'mypy pysasl test'
+run-pyright = 'pyright pysasl test'
+run-flake8 = 'flake8 pysasl test'
+run-bandit = 'bandit -c pyproject.toml -qr pysasl'
+check = ['run-pytest', 'run-mypy', 'run-pyright', 'run-flake8', 'run-bandit']
+
+[[tool.hatch.envs.all.matrix]]
+python = ['3.7', '3.8', '3.9', '3.10', '3.11']
+
+[tool.hatch.envs.doc]
+dependencies = [
+    'sphinx',
+    'sphinx-autodoc-typehints',
+    'cloud_sptheme',
+]
+
+[tool.hatch.envs.doc.scripts]
+build = 'make -C doc html'
+browse = ['build', 'open doc/build/html/index.html']
```

### Comparing `pysasl-1.0.1/PKG-INFO` & `pysasl-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: pysasl
-Version: 1.0.1
+Version: 1.0.2
 Summary: Pure Python SASL client and server library.
-Project-URL: homepage, https://github.com/icgood/pysasl/
+Project-URL: Homepage, https://github.com/icgood/pysasl/
+Project-URL: API Documentation, https://icgood.github.io/pysasl/
 Author-email: Ian Good <ian@icgood.net>
 License: ## The MIT License (MIT)
         
         Copyright (c) 2022 Ian Good
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -67,33 +68,26 @@
 #### [API Documentation](https://icgood.github.io/pysasl/)
 
 Installation
 ============
 
 Available in [PyPi](https://pypi.python.org/):
 
-```
-pip install pysasl
+```console
+$ pip install pysasl
 ```
 
 ### Running Tests
 
-Install into a virtual environment:
-
-```
-python3 -m venv .venv
-source .venv/bin/activate
-
-pip install -r requirements-dev.txt
-```
+First, install [Hatch][0]. To run the build checks:
 
-Run the tests and report coverage metrics:
+```console
+$ hatch run check
 
-```
-invoke
+$ hatch run all:check  # to run against all supported Python versions
 ```
 
 Usage
 =====
 
 ## Server-side
 
@@ -240,11 +234,12 @@
 ```
 
 And for client-side, just call `resp = mech.client_attempt(creds, [])`
 to get the initial response before starting the transmission. All
 mechanisms should either return an initial response or an empty string
 when given an empty list for the second argument.
 
+[0]: https://hatch.pypa.io/latest/install/
 [1]: https://icgood.github.io/pysasl/pysasl.html#pysasl.SASLAuth
 [2]: https://icgood.github.io/pysasl/pysasl.creds.html#pysasl.creds.server.ServerCredentials
 [3]: https://tools.ietf.org/html/rfc4954
 [4]: https://tools.ietf.org/html/rfc3501#section-6.2.2
```

