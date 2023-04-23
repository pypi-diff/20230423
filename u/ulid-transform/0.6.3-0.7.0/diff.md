# Comparing `tmp/ulid_transform-0.6.3.tar.gz` & `tmp/ulid_transform-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ulid_transform-0.6.3.tar", max compression
+gzip compressed data, was "ulid_transform-0.7.0.tar", max compression
```

## Comparing `ulid_transform-0.6.3.tar` & `ulid_transform-0.7.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1072 2023-04-10 04:05:29.903306 ulid_transform-0.6.3/LICENSE
--rw-r--r--   0        0        0     4043 2023-04-10 04:05:29.907306 ulid_transform-0.6.3/README.md
--rw-r--r--   0        0        0     1298 2023-04-10 04:05:29.907306 ulid_transform-0.6.3/build_ext.py
--rw-r--r--   0        0        0     2050 2023-04-10 04:05:30.799316 ulid_transform-0.6.3/pyproject.toml
--rw-r--r--   0        0        0      195 2023-04-10 04:05:30.775316 ulid_transform-0.6.3/src/ulid_transform/__init__.py
--rw-r--r--   0        0        0      613 2023-04-10 04:05:29.907306 ulid_transform-0.6.3/src/ulid_transform/_ulid_impl.pyx
--rw-r--r--   0        0        0        0 2023-04-10 04:05:29.907306 ulid_transform-0.6.3/src/ulid_transform/py.typed
--rw-r--r--   0        0        0      295 2023-04-10 04:05:29.907306 ulid_transform-0.6.3/src/ulid_transform/ulid.hh
--rw-r--r--   0        0        0     9473 2023-04-10 04:05:29.907306 ulid_transform-0.6.3/src/ulid_transform/ulid_impl.py
--rw-r--r--   0        0        0    19309 2023-04-10 04:05:29.907306 ulid_transform-0.6.3/src/ulid_transform/ulid_struct.hh
--rw-r--r--   0        0        0    14815 2023-04-10 04:05:29.907306 ulid_transform-0.6.3/src/ulid_transform/ulid_uint128.hh
--rw-r--r--   0        0        0      696 2023-04-10 04:05:29.907306 ulid_transform-0.6.3/src/ulid_transform/ulid_wrapper.cpp
--rw-r--r--   0        0        0      205 2023-04-10 04:05:29.907306 ulid_transform-0.6.3/src/ulid_transform/ulid_wrapper.h
--rw-r--r--   0        0        0     4831 1970-01-01 00:00:00.000000 ulid_transform-0.6.3/setup.py
--rw-r--r--   0        0        0     4989 1970-01-01 00:00:00.000000 ulid_transform-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-23 05:38:01.960281 ulid_transform-0.7.0/LICENSE
+-rw-r--r--   0        0        0     4043 2023-04-23 05:38:01.960281 ulid_transform-0.7.0/README.md
+-rw-r--r--   0        0        0     1298 2023-04-23 05:38:01.960281 ulid_transform-0.7.0/build_ext.py
+-rw-r--r--   0        0        0     2050 2023-04-23 05:38:02.732291 ulid_transform-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      195 2023-04-23 05:38:02.692290 ulid_transform-0.7.0/src/ulid_transform/__init__.py
+-rw-r--r--   0        0        0      847 2023-04-23 05:38:01.964281 ulid_transform-0.7.0/src/ulid_transform/_ulid_impl.pyx
+-rw-r--r--   0        0        0        0 2023-04-23 05:38:01.964281 ulid_transform-0.7.0/src/ulid_transform/py.typed
+-rw-r--r--   0        0        0      295 2023-04-23 05:38:01.964281 ulid_transform-0.7.0/src/ulid_transform/ulid.hh
+-rw-r--r--   0        0        0     9594 2023-04-23 05:38:01.964281 ulid_transform-0.7.0/src/ulid_transform/ulid_impl.py
+-rw-r--r--   0        0        0    19309 2023-04-23 05:38:01.964281 ulid_transform-0.7.0/src/ulid_transform/ulid_struct.hh
+-rw-r--r--   0        0        0    14815 2023-04-23 05:38:01.964281 ulid_transform-0.7.0/src/ulid_transform/ulid_uint128.hh
+-rw-r--r--   0        0        0      908 2023-04-23 05:38:01.964281 ulid_transform-0.7.0/src/ulid_transform/ulid_wrapper.cpp
+-rw-r--r--   0        0        0      263 2023-04-23 05:38:01.964281 ulid_transform-0.7.0/src/ulid_transform/ulid_wrapper.h
+-rw-r--r--   0        0        0     4831 1970-01-01 00:00:00.000000 ulid_transform-0.7.0/setup.py
+-rw-r--r--   0        0        0     4989 1970-01-01 00:00:00.000000 ulid_transform-0.7.0/PKG-INFO
```

### Comparing `ulid_transform-0.6.3/LICENSE` & `ulid_transform-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ulid_transform-0.6.3/README.md` & `ulid_transform-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `ulid_transform-0.6.3/build_ext.py` & `ulid_transform-0.7.0/build_ext.py`

 * *Files identical despite different names*

### Comparing `ulid_transform-0.6.3/pyproject.toml` & `ulid_transform-0.7.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ulid-transform"
-version = "0.6.3"
+version = "0.7.0"
 description = "Create and transform ULIDs"
 authors = ["J. Nick Koston <nick@koston.org>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bdraco/ulid-transform"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
```

### Comparing `ulid_transform-0.6.3/src/ulid_transform/ulid_impl.py` & `ulid_transform-0.7.0/src/ulid_transform/ulid_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -408,14 +408,17 @@
     if len(value) != 16:
         raise ValueError(f"ULID bytes must be 16 bytes: {value!r}")
     return _encode(value)
 
 
 try:
     from ._ulid_impl import (  # type: ignore[no-redef] # noqa: F811 F401
+        _bytes_to_ulid as bytes_to_ulid,
+    )
+    from ._ulid_impl import (  # type: ignore[no-redef] # noqa: F811 F401
         _ulid_at_time as ulid_at_time,
     )
     from ._ulid_impl import (  # type: ignore[no-redef] # noqa: F811 F401
         _ulid_now as ulid_now,
     )
     from ._ulid_impl import (  # type: ignore[no-redef] # noqa: F811 F401
         _ulid_to_bytes as ulid_to_bytes,
```

### Comparing `ulid_transform-0.6.3/src/ulid_transform/ulid_struct.hh` & `ulid_transform-0.7.0/src/ulid_transform/ulid_struct.hh`

 * *Files identical despite different names*

### Comparing `ulid_transform-0.6.3/src/ulid_transform/ulid_uint128.hh` & `ulid_transform-0.7.0/src/ulid_transform/ulid_uint128.hh`

 * *Files identical despite different names*

### Comparing `ulid_transform-0.6.3/src/ulid_transform/ulid_wrapper.cpp` & `ulid_transform-0.7.0/src/ulid_transform/ulid_wrapper.cpp`

 * *Files 23% similar despite different names*

```diff
@@ -20,7 +20,13 @@
 std::string _cpp_ulid_to_bytes(std::string ulid_string) {
   ulid::ULID ulid;
   ulid::UnmarshalFrom(ulid_string.c_str(), ulid);
   std::vector<uint8_t> data = ulid::MarshalBinary(ulid);
   std::string str(reinterpret_cast<char *>(data.data()), data.size());
   return str;
 }
+
+std::string _cpp_bytes_to_ulid(std::string bytes_string) {
+  std::vector<uint8_t> data(bytes_string.begin(), bytes_string.end());
+  ulid::ULID ulid = ulid::UnmarshalBinary(data);
+  return ulid::Marshal(ulid);
+}
```

### Comparing `ulid_transform-0.6.3/setup.py` & `ulid_transform-0.7.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ['ulid_transform']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'ulid-transform',
-    'version': '0.6.3',
+    'version': '0.7.0',
     'description': 'Create and transform ULIDs',
     'long_description': '# Fast ULID transformations\n\n<p align="center">\n  <a href="https://github.com/bdraco/ulid-transform/actions/workflows/ci.yml?query=branch%3Amain">\n    <img src="https://img.shields.io/github/actions/workflow/status/bdraco/ulid-transform/ci.yml?branch=main&label=CI&logo=github&style=flat-square" alt="CI Status" >\n  </a>\n  <a href="https://codecov.io/gh/bdraco/ulid-transform">\n    <img src="https://img.shields.io/codecov/c/github/bdraco/ulid-transform.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage percentage">\n  </a>\n</p>\n<p align="center">\n  <a href="https://python-poetry.org/">\n    <img src="https://img.shields.io/badge/packaging-poetry-299bd7?style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAASCAYAAABrXO8xAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAJJSURBVHgBfZLPa1NBEMe/s7tNXoxW1KJQKaUHkXhQvHgW6UHQQ09CBS/6V3hKc/AP8CqCrUcpmop3Cx48eDB4yEECjVQrlZb80CRN8t6OM/teagVxYZi38+Yz853dJbzoMV3MM8cJUcLMSUKIE8AzQ2PieZzFxEJOHMOgMQQ+dUgSAckNXhapU/NMhDSWLs1B24A8sO1xrN4NECkcAC9ASkiIJc6k5TRiUDPhnyMMdhKc+Zx19l6SgyeW76BEONY9exVQMzKExGKwwPsCzza7KGSSWRWEQhyEaDXp6ZHEr416ygbiKYOd7TEWvvcQIeusHYMJGhTwF9y7sGnSwaWyFAiyoxzqW0PM/RjghPxF2pWReAowTEXnDh0xgcLs8l2YQmOrj3N7ByiqEoH0cARs4u78WgAVkoEDIDoOi3AkcLOHU60RIg5wC4ZuTC7FaHKQm8Hq1fQuSOBvX/sodmNJSB5geaF5CPIkUeecdMxieoRO5jz9bheL6/tXjrwCyX/UYBUcjCaWHljx1xiX6z9xEjkYAzbGVnB8pvLmyXm9ep+W8CmsSHQQY77Zx1zboxAV0w7ybMhQmfqdmmw3nEp1I0Z+FGO6M8LZdoyZnuzzBdjISicKRnpxzI9fPb+0oYXsNdyi+d3h9bm9MWYHFtPeIZfLwzmFDKy1ai3p+PDls1Llz4yyFpferxjnyjJDSEy9CaCx5m2cJPerq6Xm34eTrZt3PqxYO1XOwDYZrFlH1fWnpU38Y9HRze3lj0vOujZcXKuuXm3jP+s3KbZVra7y2EAAAAAASUVORK5CYII=" alt="Poetry">\n  </a>\n  <a href="https://github.com/ambv/black">\n    <img src="https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square" alt="black">\n  </a>\n  <a href="https://github.com/pre-commit/pre-commit">\n    <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=flat-square" alt="pre-commit">\n  </a>\n</p>\n<p align="center">\n  <a href="https://pypi.org/project/ulid-transform/">\n    <img src="https://img.shields.io/pypi/v/ulid-transform.svg?logo=python&logoColor=fff&style=flat-square" alt="PyPI Version">\n  </a>\n  <img src="https://img.shields.io/pypi/pyversions/ulid-transform.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">\n  <img src="https://img.shields.io/pypi/l/ulid-transform.svg?style=flat-square" alt="License">\n</p>\n\nCreate and transform ULIDs\n\nThis library will use the CPP implementation from https://github.com/suyash/ulid if cython is available, and will fallback to pure python if it is not.\n\n## Example\n\n```python\n>>> import ulid_transform\n>>> ulid_transform.ulid_hex()\n\'01869a2ea5fb0b43aa056293e47c0a35\'\n>>> ulid_transform.ulid_now()\n\'0001HZX0NW00GW0X476W5TVBFE\'\n>>> ulid_transform.ulid_at_time(1234)\n\'000000016JC62D620DGYNG2R8H\'\n>>> ulid_transform.ulid_to_bytes(\'0001HZX0NW00GW0X476W5TVBFE\')\nb\'\\x00\\x00c\\xfe\\x82\\xbc\\x00!\\xc0t\\x877\\x0b\\xad\\xad\\xee\'\n>> ulid_transform.bytes_to_ulid(b"\\x01\\x86\\x99?\\xe8\\xf3\\x11\\xbc\\xed\\xef\\x86U.9\\x03z")\n\'01GTCKZT7K26YEVVW6AMQ3J0VT\'\n```\n\n## Installation\n\nInstall this via pip (or your favourite package manager):\n\n`pip install ulid-transform`\n\n## Contributors ✨\n\nThanks to https://github.com/suyash/ulid which provides the cython implementation guts.\n\nThanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):\n\n<!-- prettier-ignore-start -->\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- markdownlint-disable -->\n<!-- markdownlint-enable -->\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n<!-- prettier-ignore-end -->\n\nThis project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!\n\n## Credits\n\nThis package was created with\n[Copier](https://copier.readthedocs.io/) and the\n[browniebroke/pypackage-template](https://github.com/browniebroke/pypackage-template)\nproject template.\n',
     'author': 'J. Nick Koston',
     'author_email': 'nick@koston.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/bdraco/ulid-transform',
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['ulid_transform'] package_data = \ {'': ['*']}
-setup_kwargs = { 'name': 'ulid-transform', 'version': '0.6.3', 'description':
+setup_kwargs = { 'name': 'ulid-transform', 'version': '0.7.0', 'description':
 'Create and transform ULIDs', 'long_description': '# Fast ULID
 transformations\n\n
             \n \n_[CI_Status]\n\n \n_[Test_coverage_percentage]\n\n
 \n
              \n \n_[Poetry]\n\n \n_[black]\n\n \n_[pre-commit]\n\n
 \n
       \n \n_[PyPI_Version]\n\n [Supported Python versions]\n [License]\n
```

### Comparing `ulid_transform-0.6.3/PKG-INFO` & `ulid_transform-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ulid-transform
-Version: 0.6.3
+Version: 0.7.0
 Summary: Create and transform ULIDs
 Home-page: https://github.com/bdraco/ulid-transform
 License: MIT
 Author: J. Nick Koston
 Author-email: nick@koston.org
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ulid-transform Version: 0.6.3 Summary: Create and
+Metadata-Version: 2.1 Name: ulid-transform Version: 0.7.0 Summary: Create and
 transform ULIDs Home-page: https://github.com/bdraco/ulid-transform License:
 MIT Author: J. Nick Koston Author-email: nick@koston.org Requires-Python:
 >=3.10,<4.0 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

