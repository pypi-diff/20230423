# Comparing `tmp/ossfs-2023.3.0.tar.gz` & `tmp/ossfs-2023.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ossfs-2023.3.0.tar", last modified: Thu Apr  6 01:42:35 2023, max compression
+gzip compressed data, was "ossfs-2023.4.0.tar", last modified: Sun Apr 23 06:18:12 2023, max compression
```

## Comparing `ossfs-2023.3.0.tar` & `ossfs-2023.4.0.tar`

### file list

```diff
@@ -1,47 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 01:42:35.650859 ossfs-2023.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-06 01:42:07.000000 ossfs-2023.3.0/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-06 01:42:07.000000 ossfs-2023.3.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 01:42:35.646859 ossfs-2023.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-06 01:42:07.000000 ossfs-2023.3.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 01:42:35.646859 ossfs-2023.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-06 01:42:07.000000 ossfs-2023.3.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-06 01:42:07.000000 ossfs-2023.3.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-06 01:42:07.000000 ossfs-2023.3.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-06 01:42:07.000000 ossfs-2023.3.0/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-06 01:42:07.000000 ossfs-2023.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-06 01:42:07.000000 ossfs-2023.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-04-06 01:42:07.000000 ossfs-2023.3.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-04-06 01:42:07.000000 ossfs-2023.3.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-04-06 01:42:07.000000 ossfs-2023.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-06 01:42:07.000000 ossfs-2023.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-04-06 01:42:35.650859 ossfs-2023.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-06 01:42:07.000000 ossfs-2023.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-06 01:42:07.000000 ossfs-2023.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 01:42:35.646859 ossfs-2023.3.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 01:42:35.650859 ossfs-2023.3.0/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-06 01:42:07.000000 ossfs-2023.3.0/docs/assets/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-06 01:42:07.000000 ossfs-2023.3.0/docs/gen_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-06 01:42:07.000000 ossfs-2023.3.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-06 01:42:07.000000 ossfs-2023.3.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-06 01:42:07.000000 ossfs-2023.3.0/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-06 01:42:07.000000 ossfs-2023.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-06 01:42:35.654859 ossfs-2023.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 01:42:35.642859 ossfs-2023.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 01:42:35.650859 ossfs-2023.3.0/src/ossfs/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-06 01:42:07.000000 ossfs-2023.3.0/src/ossfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25397 2023-04-06 01:42:07.000000 ossfs-2023.3.0/src/ossfs/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-06 01:42:07.000000 ossfs-2023.3.0/src/ossfs/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 01:42:35.650859 ossfs-2023.3.0/src/ossfs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-04-06 01:42:35.000000 ossfs-2023.3.0/src/ossfs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-06 01:42:35.000000 ossfs-2023.3.0/src/ossfs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 01:42:35.000000 ossfs-2023.3.0/src/ossfs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 01:42:35.000000 ossfs-2023.3.0/src/ossfs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-06 01:42:35.000000 ossfs-2023.3.0/src/ossfs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-06 01:42:35.000000 ossfs-2023.3.0/src/ossfs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 01:42:35.650859 ossfs-2023.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-06 01:42:07.000000 ossfs-2023.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-04-06 01:42:07.000000 ossfs-2023.3.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9028 2023-04-06 01:42:07.000000 ossfs-2023.3.0/tests/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-06 01:42:07.000000 ossfs-2023.3.0/tests/test_login.py
--rw-r--r--   0 runner    (1001) docker     (123)    15292 2023-04-06 01:42:07.000000 ossfs-2023.3.0/tests/test_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-04-06 01:42:07.000000 ossfs-2023.3.0/tests/test_ossfs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:18:12.401256 ossfs-2023.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-23 06:17:45.000000 ossfs-2023.4.0/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-23 06:17:45.000000 ossfs-2023.4.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:18:12.393256 ossfs-2023.4.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-23 06:17:45.000000 ossfs-2023.4.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:18:12.393256 ossfs-2023.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-23 06:17:45.000000 ossfs-2023.4.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-23 06:17:45.000000 ossfs-2023.4.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-23 06:17:45.000000 ossfs-2023.4.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-23 06:17:45.000000 ossfs-2023.4.0/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-23 06:17:45.000000 ossfs-2023.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-23 06:17:45.000000 ossfs-2023.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-04-23 06:17:45.000000 ossfs-2023.4.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-04-23 06:17:45.000000 ossfs-2023.4.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-04-23 06:17:45.000000 ossfs-2023.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-23 06:17:45.000000 ossfs-2023.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-04-23 06:18:12.401256 ossfs-2023.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-04-23 06:17:45.000000 ossfs-2023.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:18:12.393256 ossfs-2023.4.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:18:12.393256 ossfs-2023.4.0/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-23 06:17:45.000000 ossfs-2023.4.0/docs/assets/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-23 06:17:45.000000 ossfs-2023.4.0/docs/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-23 06:17:45.000000 ossfs-2023.4.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-23 06:17:45.000000 ossfs-2023.4.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-04-23 06:17:45.000000 ossfs-2023.4.0/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-23 06:17:45.000000 ossfs-2023.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-23 06:18:12.401256 ossfs-2023.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:18:12.389256 ossfs-2023.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:18:12.393256 ossfs-2023.4.0/src/ossfs/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-23 06:17:45.000000 ossfs-2023.4.0/src/ossfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23852 2023-04-23 06:17:45.000000 ossfs-2023.4.0/src/ossfs/async_oss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9608 2023-04-23 06:17:45.000000 ossfs-2023.4.0/src/ossfs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19735 2023-04-23 06:17:45.000000 ossfs-2023.4.0/src/ossfs/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-04-23 06:17:45.000000 ossfs-2023.4.0/src/ossfs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-23 06:17:45.000000 ossfs-2023.4.0/src/ossfs/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-04-23 06:17:45.000000 ossfs-2023.4.0/src/ossfs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:18:12.397256 ossfs-2023.4.0/src/ossfs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-04-23 06:18:12.000000 ossfs-2023.4.0/src/ossfs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-23 06:18:12.000000 ossfs-2023.4.0/src/ossfs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 06:18:12.000000 ossfs-2023.4.0/src/ossfs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 06:18:12.000000 ossfs-2023.4.0/src/ossfs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-23 06:18:12.000000 ossfs-2023.4.0/src/ossfs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 06:18:12.000000 ossfs-2023.4.0/src/ossfs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:18:12.401256 ossfs-2023.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-23 06:17:45.000000 ossfs-2023.4.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:18:12.401256 ossfs-2023.4.0/tests/bench/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:17:45.000000 ossfs-2023.4.0/tests/bench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-04-23 06:17:45.000000 ossfs-2023.4.0/tests/bench/test_put_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-04-23 06:17:45.000000 ossfs-2023.4.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:18:12.401256 ossfs-2023.4.0/tests/func/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:17:45.000000 ossfs-2023.4.0/tests/func/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-23 06:17:45.000000 ossfs-2023.4.0/tests/func/test_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13170 2023-04-23 06:17:45.000000 ossfs-2023.4.0/tests/func/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-04-23 06:17:45.000000 ossfs-2023.4.0/tests/func/test_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23431 2023-04-23 06:17:45.000000 ossfs-2023.4.0/tests/func/test_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-04-23 06:17:45.000000 ossfs-2023.4.0/tests/func/test_ossfs.py
```

### Comparing `ossfs-2023.3.0/.cruft.json` & `ossfs-2023.4.0/.cruft.json`

 * *Files identical despite different names*

### Comparing `ossfs-2023.3.0/.github/dependabot.yml` & `ossfs-2023.4.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ossfs-2023.3.0/.github/workflows/docs.yml` & `ossfs-2023.4.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `ossfs-2023.3.0/.github/workflows/release.yml` & `ossfs-2023.4.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ossfs-2023.3.0/.github/workflows/tests.yml` & `ossfs-2023.4.0/.github/workflows/tests.yml`

 * *Files 5% similar despite different names*

```diff
@@ -46,16 +46,17 @@
     - name: Run tests
       env:
         OSS_ACCESS_KEY_ID: ${{ secrets.OSS_ACCESS_KEY_ID}}
         OSS_SECRET_ACCESS_KEY: ${{ secrets.OSS_SECRET_ACCESS_KEY}}
         OSS_TEST_STS_ID: ${{ secrets.OSS_TEST_STS_ID}}
         OSS_TEST_STS_KEY: ${{ secrets.OSS_TEST_STS_KEY}}
         OSS_TEST_STS_ARN: ${{ secrets.OSS_TEST_STS_ARN}}
-        OSS_ENDPOINT: ${{ secrets.OSS_ENDPOINT}}
-        OSS_TEST_BUCKET_NAME: ${{ secrets.OSS_TEST_BUCKET_NAME}}
+        OSS_ENDPOINT: ${{ vars.OSS_ENDPOINT}}
+        OSS_TEST_BUCKET_NAME: ${{ vars.OSS_TEST_BUCKET_NAME}}
+        OSS_TEST_ANONYMOUS_BUCKET_NAME: ${{ vars.OSS_TEST_ANONYMOUS_BUCKET_NAME}}
       run: nox -s tests-${{ matrix.nox_pyv || matrix.pyv }} -- --cov-report=xml
 
     - name: Upload coverage report
       uses: codecov/codecov-action@v3.1.1
 
     - name: Build package
       run: nox -s build
```

### Comparing `ossfs-2023.3.0/.gitignore` & `ossfs-2023.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ossfs-2023.3.0/.pre-commit-config.yaml` & `ossfs-2023.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ossfs-2023.3.0/CODE_OF_CONDUCT.rst` & `ossfs-2023.4.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `ossfs-2023.3.0/CONTRIBUTING.rst` & `ossfs-2023.4.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ossfs-2023.3.0/LICENSE` & `ossfs-2023.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ossfs-2023.3.0/docs/assets/logo.svg` & `ossfs-2023.4.0/docs/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `ossfs-2023.3.0/docs/gen_ref_pages.py` & `ossfs-2023.4.0/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `ossfs-2023.3.0/mkdocs.yml` & `ossfs-2023.4.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ossfs-2023.3.0/noxfile.py` & `ossfs-2023.4.0/noxfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 
 
 @nox.session(python=["3.8", "3.9", "3.10", "3.11", "pypy3.8", "pypy3.9"])
 def tests(session: nox.Session) -> None:
     session.install(".[tests]")
     session.run(
         "pytest",
+        "tests/func",
         "--cov",
         "--cov-config=pyproject.toml",
-        "--durations",
-        "100",
+        "--durations=100",
         *session.posargs,
         env={"COVERAGE_FILE": f".coverage.{session.python}"},
     )
 
 
 @nox.session
 def lint(session: nox.Session) -> None:
```

### Comparing `ossfs-2023.3.0/pyproject.toml` & `ossfs-2023.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ossfs-2023.3.0/setup.cfg` & `ossfs-2023.4.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -21,16 +21,17 @@
 [options]
 python_requires = >=3.8
 zip_safe = False
 package_dir = 
 	=src
 packages = find:
 install_requires = 
-	fsspec==2023.3.0
+	fsspec==2023.4.0
 	oss2==2.17.0
+	aiooss2==0.2.5
 
 [options.extras_require]
 docs = 
 	mkdocs==1.3.1
 	mkdocs-gen-files==0.3.5
 	mkdocs-material==8.4.1
 	mkdocs-section-index==0.3.4
```

### Comparing `ossfs-2023.3.0/src/ossfs/core.py` & `ossfs-2023.4.0/src/ossfs/core.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,108 +1,58 @@
 """
-Code of OSSFileSystem and OSSFile
+Code of OSSFileSystem
 """
+# pylint:disable=missing-function-docstring
 import copy
 import logging
 import os
-import re
 from datetime import datetime
 from hashlib import sha256
-from typing import Dict, List, Optional, Tuple, Union
+from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Union
 
 import oss2
-from fsspec.spec import AbstractBufferedFile, AbstractFileSystem
-from fsspec.utils import stringify_path
+from oss2.auth import AnonymousAuth
+from oss2.models import PartInfo
 
-from ossfs.exceptions import translate_boto_error
+from .base import DEFAULT_BLOCK_SIZE, SIMPLE_TRANSFER_THRESHOLD, BaseOSSFileSystem
+from .exceptions import translate_oss_error
+from .utils import as_progress_handler, prettify_info_result
+
+if TYPE_CHECKING:
+    from oss2.models import (
+        GetObjectResult,
+        InitMultipartUploadResult,
+        PutObjectResult,
+        SimplifiedObjectInfo,
+    )
 
-logger = logging.getLogger("ossfs")
-logging.getLogger("oss2").setLevel(logging.CRITICAL)
-logging.getLogger("urllib3").setLevel(logging.WARNING)
-
-
-def _as_progress_handler(callback):
-    if callback is None:
-        return None
-
-    sent_total = False
-
-    def progress_handler(absolute_progress, total_size):
-        nonlocal sent_total
-        if not sent_total:
-            callback.set_size(total_size)
-            sent_total = True
 
-        callback.absolute_update(absolute_progress)
-
-    return progress_handler
+logger = logging.getLogger("ossfs")
 
 
-class OSSFileSystem(AbstractFileSystem):  # pylint:disable=too-many-public-methods
+class OSSFileSystem(BaseOSSFileSystem):  # pylint:disable=too-many-public-methods
     # pylint:disable=no-value-for-parameter
     """
     A pythonic file-systems interface to OSS (Object Storage Service)
-    """
 
-    protocol = "oss"
-    SIMPLE_TRANSFER_THRESHOLD = oss2.defaults.multiget_threshold
+    Examples
+    --------
+    >>> ossfs = OSSFileSystem(anon=False)
+    >>> ossfs.ls('my-bucket/')
+    ['my-file.txt']
+
+    >>> with ossfs.open('my-bucket/my-file.txt', mode='rb') as f:
+    ...     print(f.read())
+    b'Hello, world!'
+    """
 
-    def __init__(
-        self,
-        endpoint: str,
-        key: Optional[str] = None,
-        secret: Optional[str] = None,
-        token: Optional[str] = None,
-        default_cache_type: Optional[str] = "readahead",
-        **kwargs,  # pylint: disable=too-many-arguments
-    ):
-        """
-        Parameters
-        ----------
-        key : string (None)
-            If not anonymous, use this access key ID, if specified
-        secret : string (None)
-            If not anonymous, use this secret access key, if specified
-        token : string (None)
-            If not anonymous, use this security token, if specified
-        endpoint : string (None)
-            Default endpoints of the fs
-            Endpoints are the adderss where OSS locate
-            like: http://oss-cn-hangzhou.aliyuncs.com or
-                        https://oss-me-east-1.aliyuncs.com
-        """
+    def __init__(self, **kwargs):
         super().__init__(**kwargs)
-        if token:
-            self._auth = oss2.StsAuth(key, secret, token)
-        elif key:
-            self._auth = oss2.Auth(key, secret)
-        else:
-            self._auth = oss2.AnonymousAuth()
-        self._endpoint = endpoint or os.getenv("OSS_ENDPOINT")
-        if self._endpoint is None:
-            logger.warning(
-                "OSS endpoint is not set, OSSFS could not work properly"
-                "without a endpoint, please set it manually with "
-                "`ossfs.set_endpoint` later"
-            )
-        self._default_cache_type = default_cache_type
         self._session = oss2.Session()
 
-    def set_endpoint(self, endpoint: str):
-        """
-        Reset the endpoint for ossfs
-        endpoint : string (None)
-            Default endpoints of the fs
-            Endpoints are the adderss where OSS locate
-            like: http://oss-cn-hangzhou.aliyuncs.com or
-        """
-        if not endpoint:
-            raise ValueError("Not a valid endpoint")
-        self._endpoint = endpoint
-
     def _get_bucket(
         self, bucket_name: str, connect_timeout: Optional[int] = None
     ) -> oss2.Bucket:
         """
         get the new bucket instance
         """
         if not self._endpoint:
@@ -150,307 +100,175 @@
             except oss2.exceptions.RequestError as err:
                 logger.debug("Retryable error: %s, try %s times", err, count + 1)
                 error = err
             except oss2.exceptions.OssError as err:
                 logger.debug("Nonretryable error: %s", err)
                 error = err
                 break
-        raise translate_boto_error(error)
-
-    def split_path(self, path: str) -> Tuple[str, str]:
-        """
-        Normalise object path string into bucket and key.
-        Parameters
-        ----------
-        path : string
-            Input path, like `/mybucket/path/to/file`
-        Examples
-        --------
-        >>> split_path("/mybucket/path/to/file")
-        ['mybucket', 'path/to/file' ]
-        >>> split_path("
-        /mybucket/path/to/versioned_file?versionId=some_version_id
-        ")
-        ['mybucket', 'path/to/versioned_file', 'some_version_id']
-        """
-        path = self._strip_protocol(path)
-        path = path.lstrip("/")
-        if "/" not in path:
-            return path, ""
-        bucket_name, obj_name = path.split("/", 1)
-        return bucket_name, obj_name
-
-    def _open(
-        self,
-        path,
-        mode="rb",
-        block_size=None,
-        autocommit=True,
-        cache_options=None,
-        **kwargs,  # pylint: disable=too-many-arguments
-    ):
-        """
-        Open a file for reading or writing.
-        Parameters
-        ----------
-        path: str
-            File location
-        mode: str
-            'rb', 'wb', etc.
-        autocommit: bool
-            If False, writes to temporary file that only gets put in final
-            location upon commit
-        kwargs
-        Returns
-        -------
-        OSSFile instance
-        """
-        cache_type = kwargs.pop("cache_type", self._default_cache_type)
-        return OSSFile(
-            self,
-            path,
-            mode,
-            block_size,
-            autocommit,
-            cache_options=cache_options,
-            cache_type=cache_type,
-            **kwargs,
-        )
-
-    @classmethod
-    def _strip_protocol(cls, path: Union[str, List[str]]):
-        """Turn path from fully-qualified to file-system-specifi
-        Parameters
-        ----------
-        path : string
-            Input path, like
-            `http://oss-cn-hangzhou.aliyuncs.com/mybucket/myobject`
-            `oss://mybucket/myobject`
-        Examples
-        --------
-        >>> _strip_protocol(
-            "http://oss-cn-hangzhou.aliyuncs.com/mybucket/myobject"
-            )
-        ('/mybucket/myobject')
-        >>> _strip_protocol(
-            "oss://mybucket/myobject"
-            )
-        ('/mybucket/myobject')
-        """
-        if isinstance(path, list):
-            return [cls._strip_protocol(p) for p in path]
-        path_string: str = stringify_path(path)
-        if path_string.startswith("oss://"):
-            path_string = path_string[5:]
-
-        parser_re = r"https?://(?P<endpoint>oss.+aliyuncs\.com)(?P<path>/.+)"
-        matcher = re.compile(parser_re).match(path_string)
-        if matcher:
-            path_string = matcher["path"]
-        return path_string or cls.root_marker
+        raise translate_oss_error(error) from error
 
-    def _ls_bucket(self, connect_timeout) -> List[Dict]:
-        result = []
-        for bucket in self._call_oss("BucketIterator", timeout=connect_timeout):
-            result.append(
-                {
-                    "name": bucket.name,
-                    "Key": bucket.name,
-                    "type": "directory",
-                    "size": 0,
-                    "Size": 0,
-                    "StorageClass": "BUCKET",
-                    "CreateTime": bucket.creation_date,
-                }
-            )
-        return result
-
-    def _ls_object(self, path: str, connect_timeout) -> List[Dict]:
-        bucket_name, obj_name = self.split_path(path)
-        if not obj_name or not bucket_name:
-            return []
-        if not self._call_oss(
-            "object_exists",
-            obj_name,
-            bucket=bucket_name,
-            timeout=connect_timeout,
-        ):
-            return []
-        simplifiedmeta = self._call_oss(
-            "get_object_meta",
-            obj_name,
-            bucket=bucket_name,
-            timeout=connect_timeout,
-        )
-        info = {
-            "name": path,
-            "Key": path,
-            "type": "file",
-            "size": int(simplifiedmeta.headers["Content-Length"]),
-            "Size": int(simplifiedmeta.headers["Content-Length"]),
-            "StorageClass": "OBJECT",
-        }
-        if "Last-Modified" in simplifiedmeta.headers:
-            info["LastModified"] = int(
-                datetime.strptime(
-                    simplifiedmeta.headers["Last-Modified"],
-                    "%a, %d %b %Y %H:%M:%S %Z",
-                ).timestamp()
-            )
-        return [info]
+    def _ls_bucket(self, connect_timeout: Optional[int]) -> List[Dict[str, Any]]:
+        if "" not in self.dircache:
+            results: List[Dict[str, Any]] = []
+            if isinstance(self._auth, AnonymousAuth):
+                logging.warning("cannot list buckets if not logged in")
+                return []
+            try:
+                for bucket in self._call_oss("BucketIterator", timeout=connect_timeout):
+                    result = {
+                        "name": bucket.name,
+                        "type": "directory",
+                        "size": 0,
+                        "CreateTime": bucket.creation_date,
+                    }
+                    results.append(result)
+            except oss2.exceptions.ClientError:
+                pass
+            self.dircache[""] = copy.deepcopy(results)
+        else:
+            results = self.dircache[""]
+        return results
 
     def _get_object_info_list(
         self,
         bucket_name: str,
         prefix: str,
         delimiter: str,
         connect_timeout: Optional[int],
     ):
         """
         Wrap oss2.ObjectIterator return values into a
         fsspec form of file info
         """
         result = []
+        obj: "SimplifiedObjectInfo"
         for obj in self._call_oss(
             "ObjectIterator",
             prefix=prefix,
             delimiter=delimiter,
             bucket=bucket_name,
             timeout=connect_timeout,
         ):
-            data = {
-                "name": f"{bucket_name}/{obj.key}",
-                "Key": f"{bucket_name}/{obj.key}",
-                "type": "file",
-                "size": obj.size,
-                "Size": obj.size,
-                "StorageClass": "OBJECT",
-            }
-            if obj.last_modified:
-                data["LastModified"] = obj.last_modified
-            if obj.is_prefix():
-                data["type"] = "directory"
-                data["size"] = 0
-                data["Size"] = 0
+            data = self._transfer_object_info_to_dict(bucket_name, obj)
             result.append(data)
         return result
 
     def _ls_dir(
         self,
         path: str,
         delimiter: str = "/",
-        prefix: Optional[str] = None,
-        connect_timeout: int = None,
+        refresh: bool = False,
+        prefix: str = "",
+        connect_timeout: Optional[int] = None,
+        **kwargs,  # pylint: disable=too-many-arguments
     ) -> List[Dict]:
         norm_path = path.strip("/")
-        bucket_name, key = self.split_path(norm_path)
-        if not prefix:
-            prefix = ""
+        if norm_path in self.dircache and not refresh and not prefix and delimiter:
+            return self.dircache[norm_path]
 
+        logger.debug("Get directory listing page for %s", norm_path)
+        bucket_name, key = self.split_path(norm_path)
         if not delimiter or prefix:
             if key:
                 prefix = f"{key}/{prefix}"
-            infos = self._get_object_info_list(
-                bucket_name, prefix, delimiter, connect_timeout
-            )
         else:
+            if norm_path in self.dircache and not refresh:
+                return self.dircache[norm_path]
             if key:
                 prefix = f"{key}/"
-            if norm_path not in self.dircache:
-                self.dircache[norm_path] = self._get_object_info_list(
-                    bucket_name, prefix, delimiter, connect_timeout
-                )
-            infos = copy.deepcopy(self.dircache[norm_path])
-        if path.startswith("/"):
-            for info in infos:
-                info["name"] = f'/{info["name"]}'
-                info["Key"] = f'/{info["Key"]}'
-        return infos
 
-    def ls(self, path, detail=True, **kwargs):
+        try:
+            self.dircache[norm_path] = self._get_object_info_list(
+                bucket_name, prefix, delimiter, connect_timeout
+            )
+            return self.dircache[norm_path]
+        except oss2.exceptions.AccessDenied:
+            return []
+
+    @prettify_info_result
+    def ls(self, path: str, detail: bool = True, **kwargs):
         connect_timeout = kwargs.pop("connect_timeout", 60)
-        bucket_name, _ = self.split_path(path)
-        if bucket_name:
-            try:
-                infos = self._ls_dir(path, connect_timeout=connect_timeout)
-            except oss2.exceptions.AccessDenied:
-                infos = []
-            if not infos:
-                infos = self._ls_object(path, connect_timeout)
-        else:
-            infos = self._ls_bucket(connect_timeout)
+        norm_path = self._strip_protocol(path).strip("/")
+        if norm_path == "":
+            return self._ls_bucket(connect_timeout)
+        files = self._ls_dir(path, connect_timeout=connect_timeout)
+        if not files and "/" in norm_path:
+            files = self._ls_dir(self._parent(path), connect_timeout=connect_timeout)
+            files = [
+                file
+                for file in files
+                if file["type"] != "directory" and file["name"].strip("/") == norm_path
+            ]
 
-        if not infos:
-            return infos
-        if detail:
-            return sorted(infos, key=lambda i: i["name"])
-        return sorted(info["name"] for info in infos)
+        return files
 
-    def find(self, path, maxdepth=None, withdirs=False, detail=False, **kwargs):
+    @prettify_info_result
+    def find(
+        self,
+        path: str,
+        maxdepth: Optional[int] = None,
+        withdirs: bool = False,
+        detail: bool = False,
+        **kwargs,
+    ):
         """List all files below path.
 
         Like posix ``find`` command without conditions
 
         Parameters
         ----------
         path : str
         maxdepth: int or None
             If not None, the maximum number of levels to descend
         withdirs: bool
             Whether to include directory paths in the output. This is True
             when used by glob, but users usually only want files.
         kwargs are passed to ``ls``.
         """
-        path = self._strip_protocol(path)
         out = {}
-        prefix = kwargs.pop("prefix", None)
-        if (withdirs or maxdepth) and prefix:
-            raise ValueError(
-                "Can not specify 'prefix' option alongside "
-                "'withdirs'/'maxdepth' options."
-            )
+        prefix = kwargs.pop("prefix", "")
+        path = self._verify_find_arguments(path, maxdepth, withdirs, prefix)
         if prefix:
             connect_timeout = kwargs.get("connect_timeout", None)
             for info in self._ls_dir(
-                path,
-                delimiter="",
-                prefix=prefix,
-                connect_timeout=connect_timeout,
+                path, delimiter="", prefix=prefix, connect_timeout=connect_timeout
             ):
                 out.update({info["name"]: info})
         else:
             for _, dirs, files in self.walk(path, maxdepth, detail=True, **kwargs):
                 if withdirs:
                     files.update(dirs)
                 out.update({info["name"]: info for name, info in files.items()})
             if self.isfile(path) and path not in out:
                 # walk works on directories, but find should also return [path]
                 # when path happens to be a file
                 out[path] = {}
         names = sorted(out)
-        if not detail:
-            return names
         return {name: out[name] for name in names}
 
     def _directory_exists(self, dirname: str, **kwargs):
         connect_timeout = kwargs.pop("connect_timeout", None)
         ls_result = self._ls_dir(dirname, connect_timeout=connect_timeout)
         return bool(ls_result)
 
-    def _bucket_exist(self, bucket_name):
+    def _bucket_exist(self, bucket_name: str):
         if not bucket_name:
             return False
         try:
             self._call_oss("get_bucket_info", bucket=bucket_name)
-        except oss2.exceptions.OssError:
+        except (oss2.exceptions.OssError, PermissionError):
             return False
         return True
 
-    def exists(self, path, **kwargs):
+    def exists(self, path: str, **kwargs) -> bool:
         """Is there a file at the given path"""
+        norm_path = self._strip_protocol(path).lstrip("/")
+        if norm_path == "":
+            return True
+
         bucket_name, obj_name = self.split_path(path)
 
         if not self._bucket_exist(bucket_name):
             return False
 
         connect_timeout = kwargs.get("connect_timeout", None)
         if not obj_name:
@@ -462,42 +280,43 @@
             bucket=bucket_name,
             timeout=connect_timeout,
         ):
             return True
 
         return self._directory_exists(path, **kwargs)
 
-    def ukey(self, path):
+    def ukey(self, path: str):
         """Hash of file properties, to tell if it has changed"""
         bucket_name, obj_name = self.split_path(path)
         obj_stream = self._call_oss("get_object", obj_name, bucket=bucket_name)
         return obj_stream.server_crc
 
-    def checksum(self, path):
+    def checksum(self, path: str):
         """Unique value for current version of file
 
         If the checksum is the same from one moment to another, the contents
         are guaranteed to be the same. If the checksum changes, the contents
         *might* have changed.
 
         This should normally be overridden; default will probably capture
         creation/modification timestamp (which would be good) or maybe
         access timestamp (which would be bad)
         """
         return sha256(
             (str(self.ukey(path)) + str(self.info(path))).encode()
         ).hexdigest()
 
-    def cp_file(self, path1, path2, **kwargs):
+    def cp_file(self, path1: str, path2: str, **kwargs):
         """
         Copy within two locations in the filesystem
         # todo: big file optimization
         """
         bucket_name1, obj_name1 = self.split_path(path1)
         bucket_name2, obj_name2 = self.split_path(path2)
+        self.invalidate_cache(self._parent(path2))
         if bucket_name1 != bucket_name2:
             tempdir = "." + self.ukey(path1)
             self.get_file(path1, tempdir, **kwargs)
             self.put_file(tempdir, path2, **kwargs)
             os.remove(tempdir)
         else:
             connect_timeout = kwargs.pop("connect_timeout", None)
@@ -505,31 +324,45 @@
                 "copy_object",
                 bucket_name1,
                 obj_name1,
                 obj_name2,
                 bucket=bucket_name1,
                 timeout=connect_timeout,
             )
-        self.invalidate_cache(self._parent(path2))
 
     def _rm(self, path: Union[str, List[str]]):
         """Delete files.
 
         Parameters
         ----------
         path: str or list of str
             File(s) to delete.
         """
         if isinstance(path, list):
             for file in path:
                 self._rm(file)
             return
         bucket_name, obj_name = self.split_path(path)
-        self._call_oss("delete_object", obj_name, bucket=bucket_name)
         self.invalidate_cache(self._parent(path))
+        self._call_oss("delete_object", obj_name, bucket=bucket_name)
+
+    def _bulk_delete(self, pathlist, **kwargs):
+        """
+        Remove multiple keys with one call
+
+        Parameters
+        ----------
+        pathlist : list(str)
+            The keys to remove, must all be in the same bucket.
+            Must have 0 < len <= 1000
+        """
+        if not pathlist:
+            return
+        bucket, key_list = self._get_batch_delete_key_list(pathlist)
+        self._call_oss("batch_delete_objects", key_list, bucket=bucket)
 
     def rm(self, path: Union[str, List[str]], recursive=False, maxdepth=None):
         """Delete files.
 
         Parameters
         ----------
         path: str or list of str
@@ -544,97 +377,96 @@
         """
 
         if isinstance(path, list):
             for file in path:
                 self.rm(file)
             return
 
-        bucket_name, _ = self.split_path(path)
         path_expand = self.expand_path(path, recursive=recursive, maxdepth=maxdepth)
-        path_expand = [self.split_path(file)[1] for file in path_expand]
 
         def chunks(lst: list, num: int):
             for i in range(0, len(lst), num):
                 yield lst[i : i + num]
 
         for files in chunks(path_expand, 1000):
-            self._call_oss("batch_delete_objects", files, bucket=bucket_name)
-
-        self.invalidate_cache(self._parent(path))
+            self._bulk_delete(files)
 
-    def get_path(self, rpath, lpath, **kwargs):
+    def get_path(self, rpath: str, lpath: str, **kwargs):
         """
         Copy single remote path to local
         """
         if self.isdir(rpath):
             os.makedirs(lpath, exist_ok=True)
         else:
             self.get_file(rpath, lpath, **kwargs)
 
     def get_file(
-        self, rpath, lpath, callback=None, **kwargs
+        self, rpath: str, lpath: str, callback: Optional[Callable] = None, **kwargs
     ):  # pylint: disable=arguments-differ
         """
         Copy single remote file to local
         """
-        kwargs.setdefault("progress_callback", _as_progress_handler(callback))
+        bucket_name, obj_name = self.split_path(rpath)
+        kwargs.setdefault("progress_callback", as_progress_handler(callback))
         if self.isdir(rpath):
             os.makedirs(lpath, exist_ok=True)
+            return
+        connect_timeout = kwargs.pop("connect_timeout", None)
+        bucket = self._get_bucket(bucket_name, connect_timeout)
+        if self.size(rpath) >= SIMPLE_TRANSFER_THRESHOLD:
+            oss2.resumable_download(bucket, obj_name, lpath, **kwargs)
         else:
-            bucket_name, obj_name = self.split_path(rpath)
-            connect_timeout = kwargs.pop("connect_timeout", None)
-            bucket = self._get_bucket(bucket_name, connect_timeout)
-            if self.size(rpath) >= self.SIMPLE_TRANSFER_THRESHOLD:
-                oss2.resumable_download(bucket, obj_name, lpath, **kwargs)
-            else:
-                self._call_oss(
-                    "get_object_to_file",
-                    obj_name,
-                    lpath,
-                    bucket=bucket_name,
-                    timeout=connect_timeout,
-                    **kwargs,
-                )
+            self._call_oss(
+                "get_object_to_file",
+                obj_name,
+                lpath,
+                bucket=bucket_name,
+                timeout=connect_timeout,
+                **kwargs,
+            )
 
     def put_file(
-        self, lpath, rpath, callback=None, **kwargs
+        self, lpath: str, rpath: str, callback: Optional[Callable] = None, **kwargs
     ):  # pylint: disable=arguments-differ
         """
         Copy single file to remote
         """
-        kwargs.setdefault("progress_callback", _as_progress_handler(callback))
+        kwargs.setdefault("progress_callback", as_progress_handler(callback))
+        bucket_name, obj_name = self.split_path(rpath)
         if os.path.isdir(lpath):
-            self.makedirs(rpath, exist_ok=True)
+            if obj_name:
+                # don't make remote "directory"
+                return
+            self.mkdir(lpath)
         else:
-            bucket_name, obj_name = self.split_path(rpath)
             connect_timeout = kwargs.pop("connect_timeout", None)
             bucket = self._get_bucket(bucket_name, connect_timeout)
-            if os.path.getsize(lpath) >= self.SIMPLE_TRANSFER_THRESHOLD:
+            if os.path.getsize(lpath) >= SIMPLE_TRANSFER_THRESHOLD:
                 oss2.resumable_upload(bucket, obj_name, lpath, **kwargs)
             else:
                 self._call_oss(
                     "put_object_from_file",
                     obj_name,
                     lpath,
                     bucket=bucket_name,
                     timeout=connect_timeout,
                     **kwargs,
                 )
         self.invalidate_cache(self._parent(rpath))
 
-    def created(self, path):
+    def created(self, path: str):
         """Return the created timestamp of a file as a datetime.datetime"""
         bucket_name, obj_name = self.split_path(path)
         if obj_name:
             raise NotImplementedError("OSS has no created timestamp")
         bucket_info = self._call_oss("get_bucket_info", bucket=bucket_name)
         timestamp = bucket_info.creation_date
         return datetime.fromtimestamp(timestamp)
 
-    def modified(self, path):
+    def modified(self, path: str):
         """Return the modified timestamp of a file as a datetime.datetime"""
         bucket_name, obj_name = self.split_path(path)
         if not obj_name or self.isdir(path):
             raise NotImplementedError("bucket has no modified timestamp")
         simplifiedmeta = self._call_oss("get_object_meta", obj_name, bucket=bucket_name)
         return int(
             datetime.strptime(
@@ -671,85 +503,74 @@
                 byte_range=(start, end),
                 headers=headers,
             )
         except oss2.exceptions.ServerError as err:
             raise err
         return object_stream.read()
 
-    def sign(self, path, expiration=100, **kwargs):
+    def sign(self, path: str, expiration: int = 100, **kwargs):
         raise NotImplementedError("Sign is not implemented for this filesystem")
 
-    def touch(self, path, truncate=True, **kwargs):
-        """Create empty file, or update timestamp
-
-        Parameters
-        ----------
-        path: str
-            file location
-        truncate: bool
-            If True, always set file size to 0; if False, update timestamp and
-            leave file unchanged, if backend allows this
-        """
-        if truncate or not self.exists(path):
-            with self.open(path, "wb", **kwargs):
-                pass
-            self.invalidate_cache(self._parent(path))
-
-    def pipe_file(self, path, value, **kwargs):
+    def pipe_file(self, path: str, value: str, **kwargs):
         """Set the bytes of given file"""
-        bucket_name, obj_name = self.split_path(path)
-        self._call_oss("put_object", obj_name, value, bucket=bucket_name, **kwargs)
-        bucket = self._get_bucket(bucket_name)
-        bucket.put_object(obj_name, value, **kwargs)
-        self.invalidate_cache(self._parent(path))
+        bucket, key = self.split_path(path)
+        block_size = kwargs.get("block_size", DEFAULT_BLOCK_SIZE)
+        # 5 GB is the limit for an OSS PUT
+        self.invalidate_cache(path)
+        if len(value) < min(5 * 2**30, 2 * block_size):
+            self._call_oss("put_object", key, value, bucket=bucket, **kwargs)
+            return
+        mpu: "InitMultipartUploadResult" = self._call_oss(
+            "init_multipart_upload", key, bucket=bucket, **kwargs
+        )
+        parts: List["PartInfo"] = []
+        for i, off in enumerate(range(0, len(value), block_size)):
+            data = value[off : off + block_size]
+            part_number = i + 1
+            out: "PutObjectResult" = self._call_oss(
+                "upload_part",
+                key,
+                mpu.upload_id,
+                part_number,
+                data,
+                bucket=bucket,
+            )
+            parts.append(
+                PartInfo(
+                    part_number,
+                    out.etag,
+                    size=len(data),
+                    part_crc=out.crc,
+                )
+            )
+        self._call_oss(
+            "complete_multipart_upload",
+            key,
+            mpu.upload_id,
+            parts,
+            bucket=bucket,
+        )
 
-    def invalidate_cache(self, path=None):
-        if path is None:
-            self.dircache.clear()
+    @prettify_info_result
+    def info(self, path, **kwargs):
+        norm_path = self._strip_protocol(path).lstrip("/")
+        if norm_path == "":
+            result = {"name": path, "size": 0, "type": "directory"}
         else:
-            path = self._strip_protocol(path)
-            path = path.lstrip("/")
-            self.dircache.pop(path, None)
-            while path:
-                self.dircache.pop(path, None)
-                path = self._parent(path)
-
-
-class OSSFile(AbstractBufferedFile):
-    """A file living in OSSFileSystem"""
-
-    def _upload_chunk(self, final=False):
-        """Write one part of a multi-block file upload
-        Parameters
-        ==========
-        final: bool
-            This is the last block, so should complete file, if
-            self.autocommit is True.
-        """
-        self.loc = self.fs.append_object(self.path, self.loc, self.buffer.getvalue())
-        return True
+            result = super().info(path, **kwargs)
+        if "StorageClass" in result:
+            del result["StorageClass"]
+        if "CreateTime" in result:
+            del result["CreateTime"]
+        return result
 
-    def _initiate_upload(self):
-        """Create remote file/upload"""
-        if "a" in self.mode:
-            self.loc = 0
-            if self.fs.exists(self.path):
-                self.loc = self.fs.info(self.path)["size"]
-        elif "w" in self.mode:
-            # create empty file to append to
-            self.loc = 0
-            if self.fs.exists(self.path):
-                self.fs.rm_file(self.path)
+    def cat_file(self, path: str, start: int = None, end: int = None, **kwargs):
+        bucket, object_name = self.split_path(path)
+        object_stream: "GetObjectResult" = self._call_oss(
+            "get_object",
+            bucket=bucket,
+            key=object_name,
+            byte_range=(start, end),
+            **kwargs,
+        )
 
-    def _fetch_range(self, start, end):
-        """
-        Get the specified set of bytes from remote
-        Parameters
-        ==========
-        start: int
-        end: int
-        """
-        start = max(start, 0)
-        end = min(self.size, end)
-        if start >= end or start >= self.size:
-            return b""
-        return self.fs.get_object(self.path, start, end)
+        return object_stream.read()
```

### Comparing `ossfs-2023.3.0/src/ossfs/exceptions.py` & `ossfs-2023.4.0/src/ossfs/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,21 +6,22 @@
 import errno
 
 from oss2.exceptions import OssError
 
 ERROR_CODE_TO_EXCEPTION = {
     "NoSuchBucket": FileNotFoundError,
     "NoSuchKey": FileNotFoundError,
+    "NotFound": FileNotFoundError,
     "AccessDenied": PermissionError,
 }
 
 
-def translate_boto_error(
+def translate_oss_error(
     error: OssError, *args, message=None, set_cause=True, **kwargs
-):
+) -> BaseException:
     """Convert a ClientError exception into a Python one.
     Parameters
     ----------
     error : oss2.exceptions.OssError
         The exception returned by the OSS Server.
     message : str
         An error message to use for the returned exception. If not given, the
@@ -36,16 +37,15 @@
     -------
     An instantiated exception ready to be thrown. If the error code isn't
     recognized, an IOError with the original error message is returned.
     """
     if not isinstance(error, OssError):
         # not a oss error:
         return error
-    code = error.code
-    print("error code", code)
+    code = error.__class__.__name__
     constructor = ERROR_CODE_TO_EXCEPTION.get(code)
     if constructor:
         if not message:
             message = error.message
         custom_exc = constructor(message, *args, **kwargs)
     else:
         # No match found, wrap this in an IOError with the appropriate message.
```

### Comparing `ossfs-2023.3.0/src/ossfs.egg-info/requires.txt` & `ossfs-2023.4.0/src/ossfs.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-fsspec==2023.3.0
+fsspec==2023.4.0
 oss2==2.17.0
+aiooss2==0.2.5
 
 [dev]
 pytest==7.2.0
 pytest-sugar==0.9.5
 pytest-cov==3.0.0
 pytest-mock==3.8.2
 pylint==2.15.0
```

