# Comparing `tmp/torch_max_mem-0.0.4.tar.gz` & `tmp/torch_max_mem-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_max_mem-0.0.4.tar", last modified: Thu Aug 18 09:02:13 2022, max compression
+gzip compressed data, was "torch_max_mem-0.0.5.tar", last modified: Sun Apr 23 19:05:12 2023, max compression
```

## Comparing `torch_max_mem-0.0.4.tar` & `torch_max_mem-0.0.5.tar`

### file list

```diff
@@ -1,28 +1,36 @@
-drwx------   0 berrendorf (30035) dbs      (12000)        0 2022-08-18 09:02:13.432176 torch_max_mem-0.0.4/
--rw-------   0 berrendorf (30035) dbs      (12000)     1071 2022-02-01 17:25:58.000000 torch_max_mem-0.0.4/LICENSE
--rw-------   0 berrendorf (30035) dbs      (12000)      346 2022-02-01 17:25:58.000000 torch_max_mem-0.0.4/MANIFEST.in
--rw-------   0 berrendorf (30035) dbs      (12000)     6825 2022-08-18 09:02:13.432176 torch_max_mem-0.0.4/PKG-INFO
--rw-r--r--   0 berrendorf (30035) dbs      (12000)     5569 2022-05-12 15:52:59.000000 torch_max_mem-0.0.4/README.md
-drwx------   0 berrendorf (30035) dbs      (12000)        0 2022-08-18 09:02:13.408176 torch_max_mem-0.0.4/docs/
-drwx------   0 berrendorf (30035) dbs      (12000)        0 2022-08-18 09:02:13.432176 torch_max_mem-0.0.4/docs/source/
--rw-------   0 berrendorf (30035) dbs      (12000)     7031 2022-08-18 09:02:10.000000 torch_max_mem-0.0.4/docs/source/conf.py
--rw-------   0 berrendorf (30035) dbs      (12000)      431 2022-05-06 17:09:13.000000 torch_max_mem-0.0.4/docs/source/index.rst
--rw-------   0 berrendorf (30035) dbs      (12000)      532 2022-02-01 17:25:58.000000 torch_max_mem-0.0.4/docs/source/installation.rst
--rw-------   0 berrendorf (30035) dbs      (12000)       60 2022-02-01 17:25:58.000000 torch_max_mem-0.0.4/docs/source/usage.rst
--rw-------   0 berrendorf (30035) dbs      (12000)      367 2022-02-01 17:25:58.000000 torch_max_mem-0.0.4/pyproject.toml
--rw-r--r--   0 berrendorf (30035) dbs      (12000)     1869 2022-08-18 09:02:13.436176 torch_max_mem-0.0.4/setup.cfg
-drwx------   0 berrendorf (30035) dbs      (12000)        0 2022-08-18 09:02:13.408176 torch_max_mem-0.0.4/src/
-drwx------   0 berrendorf (30035) dbs      (12000)        0 2022-08-18 09:02:13.432176 torch_max_mem-0.0.4/src/torch_max_mem/
--rw-------   0 berrendorf (30035) dbs      (12000)      230 2022-05-06 16:54:41.000000 torch_max_mem-0.0.4/src/torch_max_mem/__init__.py
--rw-r--r--   0 berrendorf (30035) dbs      (12000)     9923 2022-08-18 08:59:58.000000 torch_max_mem-0.0.4/src/torch_max_mem/api.py
--rw-r--r--   0 berrendorf (30035) dbs      (12000)     1028 2022-08-18 09:02:10.000000 torch_max_mem-0.0.4/src/torch_max_mem/version.py
-drwx------   0 berrendorf (30035) dbs      (12000)        0 2022-08-18 09:02:13.432176 torch_max_mem-0.0.4/src/torch_max_mem.egg-info/
--rw-------   0 berrendorf (30035) dbs      (12000)     6825 2022-08-18 09:02:12.000000 torch_max_mem-0.0.4/src/torch_max_mem.egg-info/PKG-INFO
--rw-------   0 berrendorf (30035) dbs      (12000)      517 2022-08-18 09:02:13.000000 torch_max_mem-0.0.4/src/torch_max_mem.egg-info/SOURCES.txt
--rw-------   0 berrendorf (30035) dbs      (12000)        1 2022-08-18 09:02:12.000000 torch_max_mem-0.0.4/src/torch_max_mem.egg-info/dependency_links.txt
--rw-------   0 berrendorf (30035) dbs      (12000)        1 2022-02-01 17:26:17.000000 torch_max_mem-0.0.4/src/torch_max_mem.egg-info/not-zip-safe
--rw-------   0 berrendorf (30035) dbs      (12000)      125 2022-08-18 09:02:13.000000 torch_max_mem-0.0.4/src/torch_max_mem.egg-info/requires.txt
--rw-------   0 berrendorf (30035) dbs      (12000)       14 2022-08-18 09:02:13.000000 torch_max_mem-0.0.4/src/torch_max_mem.egg-info/top_level.txt
-drwx------   0 berrendorf (30035) dbs      (12000)        0 2022-08-18 09:02:13.432176 torch_max_mem-0.0.4/tests/
--rw-------   0 berrendorf (30035) dbs      (12000)       63 2022-02-01 17:25:58.000000 torch_max_mem-0.0.4/tests/__init__.py
--rw-r--r--   0 berrendorf (30035) dbs      (12000)     3163 2022-08-18 08:58:41.000000 torch_max_mem-0.0.4/tests/test_decorator.py
+drwxrwxrwx   0        0        0        0 2023-04-23 19:05:12.730299 torch_max_mem-0.0.5/
+-rw-rw-rw-   0        0        0     1071 2023-04-23 16:49:58.000000 torch_max_mem-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      346 2023-04-23 16:49:58.000000 torch_max_mem-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     7054 2023-04-23 19:05:12.730299 torch_max_mem-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5569 2023-04-23 16:49:58.000000 torch_max_mem-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 19:05:12.693590 torch_max_mem-0.0.5/docs/
+drwxrwxrwx   0        0        0        0 2023-04-23 19:05:12.703430 torch_max_mem-0.0.5/docs/source/
+-rw-rw-rw-   0        0        0     7031 2023-04-23 19:03:30.000000 torch_max_mem-0.0.5/docs/source/conf.py
+-rw-rw-rw-   0        0        0      431 2023-04-23 16:49:58.000000 torch_max_mem-0.0.5/docs/source/index.rst
+-rw-rw-rw-   0        0        0      532 2023-04-23 16:49:58.000000 torch_max_mem-0.0.5/docs/source/installation.rst
+-rw-rw-rw-   0        0        0       60 2023-04-23 16:49:58.000000 torch_max_mem-0.0.5/docs/source/usage.rst
+-rw-rw-rw-   0        0        0      367 2023-04-23 16:49:58.000000 torch_max_mem-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0     2004 2023-04-23 19:05:12.736831 torch_max_mem-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-23 19:05:12.695575 torch_max_mem-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-04-23 19:05:12.705943 torch_max_mem-0.0.5/src/torch_max_mem/
+-rw-rw-rw-   0        0        0      230 2023-04-23 16:49:58.000000 torch_max_mem-0.0.5/src/torch_max_mem/__init__.py
+-rw-rw-rw-   0        0        0     8944 2023-04-23 19:02:21.000000 torch_max_mem-0.0.5/src/torch_max_mem/api.py
+-rw-rw-rw-   0        0        0     1028 2023-04-23 19:03:30.000000 torch_max_mem-0.0.5/src/torch_max_mem/version.py
+drwxrwxrwx   0        0        0        0 2023-04-23 19:05:12.723036 torch_max_mem-0.0.5/src/torch_max_mem.egg-info/
+-rw-rw-rw-   0        0        0     7054 2023-04-23 19:05:12.000000 torch_max_mem-0.0.5/src/torch_max_mem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      684 2023-04-23 19:05:12.000000 torch_max_mem-0.0.5/src/torch_max_mem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 19:05:12.000000 torch_max_mem-0.0.5/src/torch_max_mem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-23 16:53:42.000000 torch_max_mem-0.0.5/src/torch_max_mem.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      130 2023-04-23 19:05:12.000000 torch_max_mem-0.0.5/src/torch_max_mem.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-23 19:05:12.000000 torch_max_mem-0.0.5/src/torch_max_mem.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 19:05:12.725031 torch_max_mem-0.0.5/tests/
+drwxrwxrwx   0        0        0        0 2023-04-23 19:05:12.728301 torch_max_mem-0.0.5/tests/.pytest_cache/
+-rw-rw-rw-   0        0        0       39 2023-04-23 17:37:47.000000 torch_max_mem-0.0.5/tests/.pytest_cache/.gitignore
+-rw-rw-rw-   0        0        0      191 2023-04-23 17:37:47.000000 torch_max_mem-0.0.5/tests/.pytest_cache/CACHEDIR.TAG
+-rw-rw-rw-   0        0        0      310 2023-04-23 17:37:47.000000 torch_max_mem-0.0.5/tests/.pytest_cache/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 19:05:12.696523 torch_max_mem-0.0.5/tests/.pytest_cache/v/
+drwxrwxrwx   0        0        0        0 2023-04-23 19:05:12.729299 torch_max_mem-0.0.5/tests/.pytest_cache/v/cache/
+-rw-rw-rw-   0        0        0       46 2023-04-23 17:37:47.000000 torch_max_mem-0.0.5/tests/.pytest_cache/v/cache/nodeids
+-rw-rw-rw-   0        0        0        2 2023-04-23 17:37:47.000000 torch_max_mem-0.0.5/tests/.pytest_cache/v/cache/stepwise
+-rw-rw-rw-   0        0        0       63 2023-04-23 16:49:58.000000 torch_max_mem-0.0.5/tests/__init__.py
+-rw-rw-rw-   0        0        0     3082 2023-04-23 19:02:21.000000 torch_max_mem-0.0.5/tests/test_decorator.py
```

### Comparing `torch_max_mem-0.0.4/LICENSE` & `torch_max_mem-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_max_mem-0.0.4/PKG-INFO` & `torch_max_mem-0.0.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,204 +1,202 @@
-Metadata-Version: 2.1
-Name: torch_max_mem
-Version: 0.0.4
-Summary: Maximize memory utilization with PyTorch.
-Home-page: https://github.com/mberr/torch-max-mem
-Download-URL: https://github.com/mberr/torch-max-mem/releases
-Author: Max Berrendorf
-Author-email: max.berrendorf@gmail.com
-Maintainer: Max Berrendorf
-Maintainer-email: max.berrendorf@gmail.com
-License: MIT
-Project-URL: Bug Tracker, https://github.com/mberr/torch-max-mem/issues
-Project-URL: Source Code, https://github.com/mberr/torch-max-mem
-Keywords: snekpack,cookiecutter,torch
-Platform: UNKNOWN
-Classifier: Development Status :: 1 - Planning
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Framework :: Pytest
-Classifier: Framework :: tox
-Classifier: Framework :: Sphinx
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: tests
-Provides-Extra: docs
-License-File: LICENSE
-
-<!--
-<p align="center">
-  <img src="https://github.com/mberr/torch-max-mem/raw/main/docs/source/logo.png" height="150">
-</p>
--->
-
-<h1 align="center">
-  torch-max-mem
-</h1>
-
-<p align="center">
-    <a href="https://github.com/mberr/torch-max-mem/actions?query=workflow%3ATests">
-        <img alt="Tests" src="https://github.com/mberr/torch-max-mem/workflows/Tests/badge.svg" />
-    </a>
-    <a href="https://github.com/cthoyt/cookiecutter-python-package">
-        <img alt="Cookiecutter template from @cthoyt" src="https://img.shields.io/badge/Cookiecutter-snekpack-blue" /> 
-    </a>
-    <a href="https://pypi.org/project/torch_max_mem">
-        <img alt="PyPI" src="https://img.shields.io/pypi/v/torch_max_mem" />
-    </a>
-    <a href="https://pypi.org/project/torch_max_mem">
-        <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/torch_max_mem" />
-    </a>
-    <a href="https://github.com/mberr/torch-max-mem/blob/main/LICENSE">
-        <img alt="PyPI - License" src="https://img.shields.io/pypi/l/torch_max_mem" />
-    </a>
-    <a href='https://torch_max_mem.readthedocs.io/en/latest/?badge=latest'>
-        <img src='https://readthedocs.org/projects/torch_max_mem/badge/?version=latest' alt='Documentation Status' />
-    </a>
-    <a href='https://github.com/psf/black'>
-        <img src='https://img.shields.io/badge/code%20style-black-000000.svg' alt='Code style: black' />
-    </a>
-</p>
-
-This package provides decorators for memory utilization maximization with PyTorch and CUDA by starting with a maximum parameter size and applying successive halving until no more out-of-memory exception occurs.
-
-## 💪 Getting Started
-
-Assume you have a function for batched computation of nearest neighbors using brute-force distance calculation.
-
-```python
-import torch
-
-def knn(x, y, batch_size, k: int = 3):
-    return torch.cat(
-        [
-            torch.cdist(x[start : start + batch_size], y).topk(k=k, dim=1, largest=False).indices
-            for start in range(0, x.shape[0], batch_size)
-        ],
-        dim=0,
-    )
-```
-
-With `torch_max_mem` you can decorate this function to reduce the batch size until no more out-of-memory error occurs.
-
-```python
-import torch
-from torch_max_mem import maximize_memory_utilization
-
-
-@maximize_memory_utilization()
-def knn(x, y, batch_size, k: int = 3):
-    return torch.cat(
-        [
-            torch.cdist(x[start : start + batch_size], y).topk(k=k, dim=0, largest=False).indices
-            for start in range(0, x.shape[0], batch_size)
-        ],
-        dim=0,
-    )
-```
-
-In the code, you can now always pass the largest sensible batch size, e.g.,
-
-```python
-x = torch.rand(100, 100, device="cuda")
-y = torch.rand(200, 100, device="cuda")
-knn(x, y, batch_size=x.shape[0])
-```
-
-## 🚀 Installation
-
-The most recent release can be installed from
-[PyPI](https://pypi.org/project/torch_max_mem/) with:
-
-```bash
-$ pip install torch_max_mem
-```
-
-The most recent code and data can be installed directly from GitHub with:
-
-```bash
-$ pip install git+https://github.com/mberr/torch-max-mem.git
-```
-
-To install in development mode, use the following:
-
-```bash
-$ git clone git+https://github.com/mberr/torch-max-mem.git
-$ cd torch-max-mem
-$ pip install -e .
-```
-
-## 👐 Contributing
-
-Contributions, whether filing an issue, making a pull request, or forking, are appreciated. See
-[CONTRIBUTING.md](https://github.com/mberr/torch-max-mem/blob/master/CONTRIBUTING.md) for more information on getting involved.
-
-## 👋 Attribution
-
-Parts of the logic have been developed with [Laurent Vermue](https://github.com/lvermue) for [PyKEEN](https://github.com/pykeen/pykeen).
-
-
-### ⚖️ License
-
-The code in this package is licensed under the MIT License.
-
-### 🍪 Cookiecutter
-
-This package was created with [@audreyfeldroy](https://github.com/audreyfeldroy)'s
-[cookiecutter](https://github.com/cookiecutter/cookiecutter) package using [@cthoyt](https://github.com/cthoyt)'s
-[cookiecutter-snekpack](https://github.com/cthoyt/cookiecutter-snekpack) template.
-
-## 🛠️ For Developers
-
-<details>
-  <summary>See developer instrutions</summary>
-
-  
-The final section of the README is for if you want to get involved by making a code contribution.
-
-### 🥼 Testing
-
-After cloning the repository and installing `tox` with `pip install tox`, the unit tests in the `tests/` folder can be
-run reproducibly with:
-
-```shell
-$ tox
-```
-
-Additionally, these tests are automatically re-run with each commit in a [GitHub Action](https://github.com/mberr/torch-max-mem/actions?query=workflow%3ATests).
-
-### 📖 Building the Documentation
-
-```shell
-$ tox -e docs
-``` 
-
-### 📦 Making a Release
-
-After installing the package in development mode and installing
-`tox` with `pip install tox`, the commands for making a new release are contained within the `finish` environment
-in `tox.ini`. Run the following from the shell:
-
-```shell
-$ tox -e finish
-```
-
-This script does the following:
-
-1. Uses [Bump2Version](https://github.com/c4urself/bump2version) to switch the version number in the `setup.cfg` and
-   `src/torch_max_mem/version.py` to not have the `-dev` suffix
-2. Packages the code in both a tar archive and a wheel
-3. Uploads to PyPI using `twine`. Be sure to have a `.pypirc` file configured to avoid the need for manual input at this
-   step
-4. Push to GitHub. You'll need to make a release going with the commit where the version was bumped.
-5. Bump the version to the next patch. If you made big changes and want to bump the version by minor, you can
-   use `tox -e bumpversion minor` after.
-</details>
-
-
+Metadata-Version: 2.1
+Name: torch_max_mem
+Version: 0.0.5
+Summary: Maximize memory utilization with PyTorch.
+Home-page: https://github.com/mberr/torch-max-mem
+Download-URL: https://github.com/mberr/torch-max-mem/releases
+Author: Max Berrendorf
+Author-email: max.berrendorf@gmail.com
+Maintainer: Max Berrendorf
+Maintainer-email: max.berrendorf@gmail.com
+License: MIT
+Project-URL: Bug Tracker, https://github.com/mberr/torch-max-mem/issues
+Project-URL: Source Code, https://github.com/mberr/torch-max-mem
+Keywords: snekpack,cookiecutter,torch
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Framework :: Pytest
+Classifier: Framework :: tox
+Classifier: Framework :: Sphinx
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: tests
+Provides-Extra: docs
+License-File: LICENSE
+
+<!--
+<p align="center">
+  <img src="https://github.com/mberr/torch-max-mem/raw/main/docs/source/logo.png" height="150">
+</p>
+-->
+
+<h1 align="center">
+  torch-max-mem
+</h1>
+
+<p align="center">
+    <a href="https://github.com/mberr/torch-max-mem/actions?query=workflow%3ATests">
+        <img alt="Tests" src="https://github.com/mberr/torch-max-mem/workflows/Tests/badge.svg" />
+    </a>
+    <a href="https://github.com/cthoyt/cookiecutter-python-package">
+        <img alt="Cookiecutter template from @cthoyt" src="https://img.shields.io/badge/Cookiecutter-snekpack-blue" /> 
+    </a>
+    <a href="https://pypi.org/project/torch_max_mem">
+        <img alt="PyPI" src="https://img.shields.io/pypi/v/torch_max_mem" />
+    </a>
+    <a href="https://pypi.org/project/torch_max_mem">
+        <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/torch_max_mem" />
+    </a>
+    <a href="https://github.com/mberr/torch-max-mem/blob/main/LICENSE">
+        <img alt="PyPI - License" src="https://img.shields.io/pypi/l/torch_max_mem" />
+    </a>
+    <a href='https://torch_max_mem.readthedocs.io/en/latest/?badge=latest'>
+        <img src='https://readthedocs.org/projects/torch_max_mem/badge/?version=latest' alt='Documentation Status' />
+    </a>
+    <a href='https://github.com/psf/black'>
+        <img src='https://img.shields.io/badge/code%20style-black-000000.svg' alt='Code style: black' />
+    </a>
+</p>
+
+This package provides decorators for memory utilization maximization with PyTorch and CUDA by starting with a maximum parameter size and applying successive halving until no more out-of-memory exception occurs.
+
+## 💪 Getting Started
+
+Assume you have a function for batched computation of nearest neighbors using brute-force distance calculation.
+
+```python
+import torch
+
+def knn(x, y, batch_size, k: int = 3):
+    return torch.cat(
+        [
+            torch.cdist(x[start : start + batch_size], y).topk(k=k, dim=1, largest=False).indices
+            for start in range(0, x.shape[0], batch_size)
+        ],
+        dim=0,
+    )
+```
+
+With `torch_max_mem` you can decorate this function to reduce the batch size until no more out-of-memory error occurs.
+
+```python
+import torch
+from torch_max_mem import maximize_memory_utilization
+
+
+@maximize_memory_utilization()
+def knn(x, y, batch_size, k: int = 3):
+    return torch.cat(
+        [
+            torch.cdist(x[start : start + batch_size], y).topk(k=k, dim=0, largest=False).indices
+            for start in range(0, x.shape[0], batch_size)
+        ],
+        dim=0,
+    )
+```
+
+In the code, you can now always pass the largest sensible batch size, e.g.,
+
+```python
+x = torch.rand(100, 100, device="cuda")
+y = torch.rand(200, 100, device="cuda")
+knn(x, y, batch_size=x.shape[0])
+```
+
+## 🚀 Installation
+
+The most recent release can be installed from
+[PyPI](https://pypi.org/project/torch_max_mem/) with:
+
+```bash
+$ pip install torch_max_mem
+```
+
+The most recent code and data can be installed directly from GitHub with:
+
+```bash
+$ pip install git+https://github.com/mberr/torch-max-mem.git
+```
+
+To install in development mode, use the following:
+
+```bash
+$ git clone git+https://github.com/mberr/torch-max-mem.git
+$ cd torch-max-mem
+$ pip install -e .
+```
+
+## 👐 Contributing
+
+Contributions, whether filing an issue, making a pull request, or forking, are appreciated. See
+[CONTRIBUTING.md](https://github.com/mberr/torch-max-mem/blob/master/CONTRIBUTING.md) for more information on getting involved.
+
+## 👋 Attribution
+
+Parts of the logic have been developed with [Laurent Vermue](https://github.com/lvermue) for [PyKEEN](https://github.com/pykeen/pykeen).
+
+
+### ⚖️ License
+
+The code in this package is licensed under the MIT License.
+
+### 🍪 Cookiecutter
+
+This package was created with [@audreyfeldroy](https://github.com/audreyfeldroy)'s
+[cookiecutter](https://github.com/cookiecutter/cookiecutter) package using [@cthoyt](https://github.com/cthoyt)'s
+[cookiecutter-snekpack](https://github.com/cthoyt/cookiecutter-snekpack) template.
+
+## 🛠️ For Developers
+
+<details>
+  <summary>See developer instrutions</summary>
+
+  
+The final section of the README is for if you want to get involved by making a code contribution.
+
+### 🥼 Testing
+
+After cloning the repository and installing `tox` with `pip install tox`, the unit tests in the `tests/` folder can be
+run reproducibly with:
+
+```shell
+$ tox
+```
+
+Additionally, these tests are automatically re-run with each commit in a [GitHub Action](https://github.com/mberr/torch-max-mem/actions?query=workflow%3ATests).
+
+### 📖 Building the Documentation
+
+```shell
+$ tox -e docs
+``` 
+
+### 📦 Making a Release
+
+After installing the package in development mode and installing
+`tox` with `pip install tox`, the commands for making a new release are contained within the `finish` environment
+in `tox.ini`. Run the following from the shell:
+
+```shell
+$ tox -e finish
+```
+
+This script does the following:
+
+1. Uses [Bump2Version](https://github.com/c4urself/bump2version) to switch the version number in the `setup.cfg` and
+   `src/torch_max_mem/version.py` to not have the `-dev` suffix
+2. Packages the code in both a tar archive and a wheel
+3. Uploads to PyPI using `twine`. Be sure to have a `.pypirc` file configured to avoid the need for manual input at this
+   step
+4. Push to GitHub. You'll need to make a release going with the commit where the version was bumped.
+5. Bump the version to the next patch. If you made big changes and want to bump the version by minor, you can
+   use `tox -e bumpversion minor` after.
+</details>
```

#### html2text {}

```diff
@@ -1,24 +1,25 @@
-Metadata-Version: 2.1 Name: torch_max_mem Version: 0.0.4 Summary: Maximize
+Metadata-Version: 2.1 Name: torch_max_mem Version: 0.0.5 Summary: Maximize
 memory utilization with PyTorch. Home-page: https://github.com/mberr/torch-max-
 mem Download-URL: https://github.com/mberr/torch-max-mem/releases Author: Max
 Berrendorf Author-email: max.berrendorf@gmail.com Maintainer: Max Berrendorf
 Maintainer-email: max.berrendorf@gmail.com License: MIT Project-URL: Bug
 Tracker, https://github.com/mberr/torch-max-mem/issues Project-URL: Source
 Code, https://github.com/mberr/torch-max-mem Keywords:
-snekpack,cookiecutter,torch Platform: UNKNOWN Classifier: Development Status ::
-1 - Planning Classifier: Environment :: Console Classifier: Intended Audience
-:: Developers Classifier: License :: OSI Approved :: MIT License Classifier:
-Operating System :: OS Independent Classifier: Framework :: Pytest Classifier:
-Framework :: tox Classifier: Framework :: Sphinx Classifier: Programming
-Language :: Python Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3 ::
-Only Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-
-Extra: tests Provides-Extra: docs License-File: LICENSE
+snekpack,cookiecutter,torch Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
+:: OS Independent Classifier: Framework :: Pytest Classifier: Framework :: tox
+Classifier: Framework :: Sphinx Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3 :: Only Requires-Python: >=3.8 Description-Content-
+Type: text/markdown Provides-Extra: tests Provides-Extra: docs License-File:
+LICENSE
                           ****** torch-max-mem ******
  [Tests] [Cookiecutter_template_from_@cthoyt] [PyPI] [PyPI_-_Python_Version]
           [PyPI_-_License] [Documentation_Status] [Code_style:_black]
 This package provides decorators for memory utilization maximization with
 PyTorch and CUDA by starting with a maximum parameter size and applying
 successive halving until no more out-of-memory exception occurs. ## ðª
 Getting Started Assume you have a function for batched computation of nearest
```

### Comparing `torch_max_mem-0.0.4/README.md` & `torch_max_mem-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `torch_max_mem-0.0.4/docs/source/conf.py` & `torch_max_mem-0.0.5/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # -- Project information -----------------------------------------------------
 
 project = 'torch_max_mem'
 copyright = f'{date.today().year}, Max Berrendorf'
 author = 'Max Berrendorf'
 
 # The full version, including alpha/beta/rc tags.
-release = '0.0.4'
+release = '0.0.5'
 
 # The short X.Y version.
 parsed_version = re.match(
     '(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?:-(?P<release>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?(?:\+(?P<build>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?',
     release,
 )
 version = parsed_version.expand('\g<major>.\g<minor>.\g<patch>')
```

### Comparing `torch_max_mem-0.0.4/docs/source/installation.rst` & `torch_max_mem-0.0.5/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `torch_max_mem-0.0.4/setup.cfg` & `torch_max_mem-0.0.5/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -1,117 +1,126 @@
-00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
-00000010: 3d20 746f 7263 685f 6d61 785f 6d65 6d0a  = torch_max_mem.
-00000020: 7665 7273 696f 6e20 3d20 302e 302e 340a  version = 0.0.4.
-00000030: 6465 7363 7269 7074 696f 6e20 3d20 4d61  description = Ma
-00000040: 7869 6d69 7a65 206d 656d 6f72 7920 7574  ximize memory ut
-00000050: 696c 697a 6174 696f 6e20 7769 7468 2050  ilization with P
-00000060: 7954 6f72 6368 2e0a 6c6f 6e67 5f64 6573  yTorch..long_des
-00000070: 6372 6970 7469 6f6e 203d 2066 696c 653a  cription = file:
-00000080: 2052 4541 444d 452e 6d64 0a6c 6f6e 675f   README.md.long_
-00000090: 6465 7363 7269 7074 696f 6e5f 636f 6e74  description_cont
-000000a0: 656e 745f 7479 7065 203d 2074 6578 742f  ent_type = text/
-000000b0: 6d61 726b 646f 776e 0a75 726c 203d 2068  markdown.url = h
-000000c0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000000d0: 6d2f 6d62 6572 722f 746f 7263 682d 6d61  m/mberr/torch-ma
-000000e0: 782d 6d65 6d0a 646f 776e 6c6f 6164 5f75  x-mem.download_u
-000000f0: 726c 203d 2068 7474 7073 3a2f 2f67 6974  rl = https://git
-00000100: 6875 622e 636f 6d2f 6d62 6572 722f 746f  hub.com/mberr/to
-00000110: 7263 682d 6d61 782d 6d65 6d2f 7265 6c65  rch-max-mem/rele
-00000120: 6173 6573 0a70 726f 6a65 6374 5f75 726c  ases.project_url
-00000130: 7320 3d20 0a09 4275 6720 5472 6163 6b65  s = ..Bug Tracke
-00000140: 7220 3d20 6874 7470 733a 2f2f 6769 7468  r = https://gith
-00000150: 7562 2e63 6f6d 2f6d 6265 7272 2f74 6f72  ub.com/mberr/tor
-00000160: 6368 2d6d 6178 2d6d 656d 2f69 7373 7565  ch-max-mem/issue
-00000170: 730a 0953 6f75 7263 6520 436f 6465 203d  s..Source Code =
-00000180: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00000190: 636f 6d2f 6d62 6572 722f 746f 7263 682d  com/mberr/torch-
-000001a0: 6d61 782d 6d65 6d0a 6175 7468 6f72 203d  max-mem.author =
-000001b0: 204d 6178 2042 6572 7265 6e64 6f72 660a   Max Berrendorf.
-000001c0: 6175 7468 6f72 5f65 6d61 696c 203d 206d  author_email = m
-000001d0: 6178 2e62 6572 7265 6e64 6f72 6640 676d  ax.berrendorf@gm
-000001e0: 6169 6c2e 636f 6d0a 6d61 696e 7461 696e  ail.com.maintain
-000001f0: 6572 203d 204d 6178 2042 6572 7265 6e64  er = Max Berrend
-00000200: 6f72 660a 6d61 696e 7461 696e 6572 5f65  orf.maintainer_e
-00000210: 6d61 696c 203d 206d 6178 2e62 6572 7265  mail = max.berre
-00000220: 6e64 6f72 6640 676d 6169 6c2e 636f 6d0a  ndorf@gmail.com.
-00000230: 6c69 6365 6e73 6520 3d20 4d49 540a 6c69  license = MIT.li
-00000240: 6365 6e73 655f 6669 6c65 203d 204c 4943  cense_file = LIC
-00000250: 454e 5345 0a63 6c61 7373 6966 6965 7273  ENSE.classifiers
-00000260: 203d 200a 0944 6576 656c 6f70 6d65 6e74   = ..Development
-00000270: 2053 7461 7475 7320 3a3a 2031 202d 2050   Status :: 1 - P
-00000280: 6c61 6e6e 696e 670a 0945 6e76 6972 6f6e  lanning..Environ
-00000290: 6d65 6e74 203a 3a20 436f 6e73 6f6c 650a  ment :: Console.
-000002a0: 0949 6e74 656e 6465 6420 4175 6469 656e  .Intended Audien
-000002b0: 6365 203a 3a20 4465 7665 6c6f 7065 7273  ce :: Developers
-000002c0: 0a09 4c69 6365 6e73 6520 3a3a 204f 5349  ..License :: OSI
-000002d0: 2041 7070 726f 7665 6420 3a3a 204d 4954   Approved :: MIT
-000002e0: 204c 6963 656e 7365 0a09 4f70 6572 6174   License..Operat
-000002f0: 696e 6720 5379 7374 656d 203a 3a20 4f53  ing System :: OS
-00000300: 2049 6e64 6570 656e 6465 6e74 0a09 4672   Independent..Fr
-00000310: 616d 6577 6f72 6b20 3a3a 2050 7974 6573  amework :: Pytes
-00000320: 740a 0946 7261 6d65 776f 726b 203a 3a20  t..Framework :: 
-00000330: 746f 780a 0946 7261 6d65 776f 726b 203a  tox..Framework :
-00000340: 3a20 5370 6869 6e78 0a09 5072 6f67 7261  : Sphinx..Progra
-00000350: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000360: 3a20 5079 7468 6f6e 0a09 5072 6f67 7261  : Python..Progra
-00000370: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000380: 3a20 5079 7468 6f6e 203a 3a20 332e 380a  : Python :: 3.8.
-00000390: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
-000003a0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-000003b0: 3a3a 2033 2e39 0a09 5072 6f67 7261 6d6d  :: 3.9..Programm
-000003c0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-000003d0: 5079 7468 6f6e 203a 3a20 332e 3130 0a09  Python :: 3.10..
-000003e0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-000003f0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000400: 3a20 3320 3a3a 204f 6e6c 790a 6b65 7977  : 3 :: Only.keyw
-00000410: 6f72 6473 203d 200a 0973 6e65 6b70 6163  ords = ..snekpac
-00000420: 6b0a 0963 6f6f 6b69 6563 7574 7465 720a  k..cookiecutter.
-00000430: 0974 6f72 6368 0a0a 5b6f 7074 696f 6e73  .torch..[options
-00000440: 5d0a 696e 7374 616c 6c5f 7265 7175 6972  ].install_requir
-00000450: 6573 203d 200a 096e 756d 7079 0a09 746f  es = ..numpy..to
-00000460: 7263 680a 7a69 705f 7361 6665 203d 2066  rch.zip_safe = f
-00000470: 616c 7365 0a69 6e63 6c75 6465 5f70 6163  alse.include_pac
-00000480: 6b61 6765 5f64 6174 6120 3d20 5472 7565  kage_data = True
-00000490: 0a70 7974 686f 6e5f 7265 7175 6972 6573  .python_requires
-000004a0: 203d 203e 3d33 2e38 0a70 6163 6b61 6765   = >=3.8.package
-000004b0: 7320 3d20 6669 6e64 3a0a 7061 636b 6167  s = find:.packag
-000004c0: 655f 6469 7220 3d20 0a09 3d20 7372 630a  e_dir = ..= src.
-000004d0: 0a5b 6f70 7469 6f6e 732e 7061 636b 6167  .[options.packag
-000004e0: 6573 2e66 696e 645d 0a77 6865 7265 203d  es.find].where =
-000004f0: 2073 7263 0a0a 5b6f 7074 696f 6e73 2e65   src..[options.e
-00000500: 7874 7261 735f 7265 7175 6972 655d 0a74  xtras_require].t
-00000510: 6573 7473 203d 200a 0970 7974 6573 740a  ests = ..pytest.
-00000520: 0963 6f76 6572 6167 650a 646f 6373 203d  .coverage.docs =
-00000530: 200a 0973 7068 696e 780a 0973 7068 696e   ..sphinx..sphin
-00000540: 782d 7274 642d 7468 656d 650a 0973 7068  x-rtd-theme..sph
-00000550: 696e 782d 636c 6963 6b0a 0973 7068 696e  inx-click..sphin
-00000560: 782d 6175 746f 646f 632d 7479 7065 6869  x-autodoc-typehi
-00000570: 6e74 730a 0973 7068 696e 785f 6175 746f  nts..sphinx_auto
-00000580: 6d6f 6461 7069 0a0a 5b64 6f63 385d 0a6d  modapi..[doc8].m
-00000590: 6178 2d6c 696e 652d 6c65 6e67 7468 203d  ax-line-length =
-000005a0: 2031 3230 0a0a 5b63 6f76 6572 6167 653a   120..[coverage:
-000005b0: 7275 6e5d 0a62 7261 6e63 6820 3d20 5472  run].branch = Tr
-000005c0: 7565 0a73 6f75 7263 6520 3d20 746f 7263  ue.source = torc
-000005d0: 685f 6d61 785f 6d65 6d0a 6f6d 6974 203d  h_max_mem.omit =
-000005e0: 200a 0974 6573 7473 2f2a 0a09 646f 6373   ..tests/*..docs
-000005f0: 2f2a 0a0a 5b63 6f76 6572 6167 653a 7061  /*..[coverage:pa
-00000600: 7468 735d 0a73 6f75 7263 6520 3d20 0a09  ths].source = ..
-00000610: 7372 632f 746f 7263 685f 6d61 785f 6d65  src/torch_max_me
-00000620: 6d0a 092e 746f 782f 2a2f 6c69 622f 7079  m...tox/*/lib/py
-00000630: 7468 6f6e 2a2f 7369 7465 2d70 6163 6b61  thon*/site-packa
-00000640: 6765 732f 746f 7263 685f 6d61 785f 6d65  ges/torch_max_me
-00000650: 6d0a 0a5b 636f 7665 7261 6765 3a72 6570  m..[coverage:rep
-00000660: 6f72 745d 0a73 686f 775f 6d69 7373 696e  ort].show_missin
-00000670: 6720 3d20 5472 7565 0a65 7863 6c75 6465  g = True.exclude
-00000680: 5f6c 696e 6573 203d 200a 0970 7261 676d  _lines = ..pragm
-00000690: 613a 206e 6f20 636f 7665 720a 0972 6169  a: no cover..rai
-000006a0: 7365 204e 6f74 496d 706c 656d 656e 7465  se NotImplemente
-000006b0: 6445 7272 6f72 0a09 6966 205f 5f6e 616d  dError..if __nam
-000006c0: 655f 5f20 3d3d 202e 5f5f 6d61 696e 5f5f  e__ == .__main__
-000006d0: 2e3a 0a09 6465 6620 5f5f 7374 725f 5f0a  .:..def __str__.
-000006e0: 0964 6566 205f 5f72 6570 725f 5f0a 0a5b  .def __repr__..[
-000006f0: 6461 7267 6c69 6e74 5d0a 646f 6373 7472  darglint].docstr
-00000700: 696e 675f 7374 796c 6520 3d20 7370 6869  ing_style = sphi
-00000710: 6e78 0a73 7472 6963 746e 6573 7320 3d20  nx.strictness = 
-00000720: 7368 6f72 740a 0a5b 6567 675f 696e 666f  short..[egg_info
-00000730: 5d0a 7461 675f 6275 696c 6420 3d20 0a74  ].tag_build = .t
-00000740: 6167 5f64 6174 6520 3d20 300a 0a         ag_date = 0..
+00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
+00000010: 203d 2074 6f72 6368 5f6d 6178 5f6d 656d   = torch_max_mem
+00000020: 0d0a 7665 7273 696f 6e20 3d20 302e 302e  ..version = 0.0.
+00000030: 350d 0a64 6573 6372 6970 7469 6f6e 203d  5..description =
+00000040: 204d 6178 696d 697a 6520 6d65 6d6f 7279   Maximize memory
+00000050: 2075 7469 6c69 7a61 7469 6f6e 2077 6974   utilization wit
+00000060: 6820 5079 546f 7263 682e 0d0a 6c6f 6e67  h PyTorch...long
+00000070: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
+00000080: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
+00000090: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
+000000a0: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
+000000b0: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a75  text/markdown..u
+000000c0: 726c 203d 2068 7474 7073 3a2f 2f67 6974  rl = https://git
+000000d0: 6875 622e 636f 6d2f 6d62 6572 722f 746f  hub.com/mberr/to
+000000e0: 7263 682d 6d61 782d 6d65 6d0d 0a64 6f77  rch-max-mem..dow
+000000f0: 6e6c 6f61 645f 7572 6c20 3d20 6874 7470  nload_url = http
+00000100: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6d  s://github.com/m
+00000110: 6265 7272 2f74 6f72 6368 2d6d 6178 2d6d  berr/torch-max-m
+00000120: 656d 2f72 656c 6561 7365 730d 0a70 726f  em/releases..pro
+00000130: 6a65 6374 5f75 726c 7320 3d20 0d0a 0942  ject_urls = ...B
+00000140: 7567 2054 7261 636b 6572 203d 2068 7474  ug Tracker = htt
+00000150: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000160: 6d62 6572 722f 746f 7263 682d 6d61 782d  mberr/torch-max-
+00000170: 6d65 6d2f 6973 7375 6573 0d0a 0953 6f75  mem/issues...Sou
+00000180: 7263 6520 436f 6465 203d 2068 7474 7073  rce Code = https
+00000190: 3a2f 2f67 6974 6875 622e 636f 6d2f 6d62  ://github.com/mb
+000001a0: 6572 722f 746f 7263 682d 6d61 782d 6d65  err/torch-max-me
+000001b0: 6d0d 0a61 7574 686f 7220 3d20 4d61 7820  m..author = Max 
+000001c0: 4265 7272 656e 646f 7266 0d0a 6175 7468  Berrendorf..auth
+000001d0: 6f72 5f65 6d61 696c 203d 206d 6178 2e62  or_email = max.b
+000001e0: 6572 7265 6e64 6f72 6640 676d 6169 6c2e  errendorf@gmail.
+000001f0: 636f 6d0d 0a6d 6169 6e74 6169 6e65 7220  com..maintainer 
+00000200: 3d20 4d61 7820 4265 7272 656e 646f 7266  = Max Berrendorf
+00000210: 0d0a 6d61 696e 7461 696e 6572 5f65 6d61  ..maintainer_ema
+00000220: 696c 203d 206d 6178 2e62 6572 7265 6e64  il = max.berrend
+00000230: 6f72 6640 676d 6169 6c2e 636f 6d0d 0a6c  orf@gmail.com..l
+00000240: 6963 656e 7365 203d 204d 4954 0d0a 6c69  icense = MIT..li
+00000250: 6365 6e73 655f 6669 6c65 203d 204c 4943  cense_file = LIC
+00000260: 454e 5345 0d0a 636c 6173 7369 6669 6572  ENSE..classifier
+00000270: 7320 3d20 0d0a 0944 6576 656c 6f70 6d65  s = ...Developme
+00000280: 6e74 2053 7461 7475 7320 3a3a 2034 202d  nt Status :: 4 -
+00000290: 2042 6574 610d 0a09 456e 7669 726f 6e6d   Beta...Environm
+000002a0: 656e 7420 3a3a 2043 6f6e 736f 6c65 0d0a  ent :: Console..
+000002b0: 0949 6e74 656e 6465 6420 4175 6469 656e  .Intended Audien
+000002c0: 6365 203a 3a20 4465 7665 6c6f 7065 7273  ce :: Developers
+000002d0: 0d0a 094c 6963 656e 7365 203a 3a20 4f53  ...License :: OS
+000002e0: 4920 4170 7072 6f76 6564 203a 3a20 4d49  I Approved :: MI
+000002f0: 5420 4c69 6365 6e73 650d 0a09 4f70 6572  T License...Oper
+00000300: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
+00000310: 4f53 2049 6e64 6570 656e 6465 6e74 0d0a  OS Independent..
+00000320: 0946 7261 6d65 776f 726b 203a 3a20 5079  .Framework :: Py
+00000330: 7465 7374 0d0a 0946 7261 6d65 776f 726b  test...Framework
+00000340: 203a 3a20 746f 780d 0a09 4672 616d 6577   :: tox...Framew
+00000350: 6f72 6b20 3a3a 2053 7068 696e 780d 0a09  ork :: Sphinx...
+00000360: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000370: 7561 6765 203a 3a20 5079 7468 6f6e 0d0a  uage :: Python..
+00000380: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
+00000390: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+000003a0: 3a3a 2033 2e38 0d0a 0950 726f 6772 616d  :: 3.8...Program
+000003b0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+000003c0: 2050 7974 686f 6e20 3a3a 2033 2e39 0d0a   Python :: 3.9..
+000003d0: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
+000003e0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+000003f0: 3a3a 2033 2e31 300d 0a09 5072 6f67 7261  :: 3.10...Progra
+00000400: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000410: 3a20 5079 7468 6f6e 203a 3a20 332e 3131  : Python :: 3.11
+00000420: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
+00000430: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000440: 6e20 3a3a 2033 203a 3a20 4f6e 6c79 0d0a  n :: 3 :: Only..
+00000450: 6b65 7977 6f72 6473 203d 200d 0a09 736e  keywords = ...sn
+00000460: 656b 7061 636b 0d0a 0963 6f6f 6b69 6563  ekpack...cookiec
+00000470: 7574 7465 720d 0a09 746f 7263 680d 0a0d  utter...torch...
+00000480: 0a5b 6f70 7469 6f6e 735d 0d0a 696e 7374  .[options]..inst
+00000490: 616c 6c5f 7265 7175 6972 6573 203d 200d  all_requires = .
+000004a0: 0a09 6e75 6d70 790d 0a09 746f 7263 683e  ..numpy...torch>
+000004b0: 3d32 2e30 0d0a 7a69 705f 7361 6665 203d  =2.0..zip_safe =
+000004c0: 2066 616c 7365 0d0a 696e 636c 7564 655f   false..include_
+000004d0: 7061 636b 6167 655f 6461 7461 203d 2054  package_data = T
+000004e0: 7275 650d 0a70 7974 686f 6e5f 7265 7175  rue..python_requ
+000004f0: 6972 6573 203d 203e 3d33 2e38 0d0a 7061  ires = >=3.8..pa
+00000500: 636b 6167 6573 203d 2066 696e 643a 0d0a  ckages = find:..
+00000510: 7061 636b 6167 655f 6469 7220 3d20 0d0a  package_dir = ..
+00000520: 093d 2073 7263 0d0a 0d0a 5b6f 7074 696f  .= src....[optio
+00000530: 6e73 2e70 6163 6b61 6765 732e 6669 6e64  ns.packages.find
+00000540: 5d0d 0a77 6865 7265 203d 2073 7263 0d0a  ]..where = src..
+00000550: 0d0a 5b6f 7074 696f 6e73 2e65 7874 7261  ..[options.extra
+00000560: 735f 7265 7175 6972 655d 0d0a 7465 7374  s_require]..test
+00000570: 7320 3d20 0d0a 0970 7974 6573 740d 0a09  s = ...pytest...
+00000580: 636f 7665 7261 6765 0d0a 646f 6373 203d  coverage..docs =
+00000590: 200d 0a09 7370 6869 6e78 0d0a 0973 7068   ...sphinx...sph
+000005a0: 696e 782d 7274 642d 7468 656d 650d 0a09  inx-rtd-theme...
+000005b0: 7370 6869 6e78 2d63 6c69 636b 0d0a 0973  sphinx-click...s
+000005c0: 7068 696e 782d 6175 746f 646f 632d 7479  phinx-autodoc-ty
+000005d0: 7065 6869 6e74 730d 0a09 7370 6869 6e78  pehints...sphinx
+000005e0: 5f61 7574 6f6d 6f64 6170 690d 0a0d 0a5b  _automodapi....[
+000005f0: 646f 6338 5d0d 0a6d 6178 2d6c 696e 652d  doc8]..max-line-
+00000600: 6c65 6e67 7468 203d 2031 3230 0d0a 0d0a  length = 120....
+00000610: 5b63 6f76 6572 6167 653a 7275 6e5d 0d0a  [coverage:run]..
+00000620: 6272 616e 6368 203d 2054 7275 650d 0a73  branch = True..s
+00000630: 6f75 7263 6520 3d20 746f 7263 685f 6d61  ource = torch_ma
+00000640: 785f 6d65 6d0d 0a6f 6d69 7420 3d20 0d0a  x_mem..omit = ..
+00000650: 0974 6573 7473 2f2a 0d0a 0964 6f63 732f  .tests/*...docs/
+00000660: 2a0d 0a0d 0a5b 636f 7665 7261 6765 3a70  *....[coverage:p
+00000670: 6174 6873 5d0d 0a73 6f75 7263 6520 3d20  aths]..source = 
+00000680: 0d0a 0973 7263 2f74 6f72 6368 5f6d 6178  ...src/torch_max
+00000690: 5f6d 656d 0d0a 092e 746f 782f 2a2f 6c69  _mem....tox/*/li
+000006a0: 622f 7079 7468 6f6e 2a2f 7369 7465 2d70  b/python*/site-p
+000006b0: 6163 6b61 6765 732f 746f 7263 685f 6d61  ackages/torch_ma
+000006c0: 785f 6d65 6d0d 0a0d 0a5b 636f 7665 7261  x_mem....[covera
+000006d0: 6765 3a72 6570 6f72 745d 0d0a 7368 6f77  ge:report]..show
+000006e0: 5f6d 6973 7369 6e67 203d 2054 7275 650d  _missing = True.
+000006f0: 0a65 7863 6c75 6465 5f6c 696e 6573 203d  .exclude_lines =
+00000700: 200d 0a09 7072 6167 6d61 3a20 6e6f 2063   ...pragma: no c
+00000710: 6f76 6572 0d0a 0972 6169 7365 204e 6f74  over...raise Not
+00000720: 496d 706c 656d 656e 7465 6445 7272 6f72  ImplementedError
+00000730: 0d0a 0969 6620 5f5f 6e61 6d65 5f5f 203d  ...if __name__ =
+00000740: 3d20 2e5f 5f6d 6169 6e5f 5f2e 3a0d 0a09  = .__main__.:...
+00000750: 6465 6620 5f5f 7374 725f 5f0d 0a09 6465  def __str__...de
+00000760: 6620 5f5f 7265 7072 5f5f 0d0a 0d0a 5b64  f __repr__....[d
+00000770: 6172 676c 696e 745d 0d0a 646f 6373 7472  arglint]..docstr
+00000780: 696e 675f 7374 796c 6520 3d20 7370 6869  ing_style = sphi
+00000790: 6e78 0d0a 7374 7269 6374 6e65 7373 203d  nx..strictness =
+000007a0: 2073 686f 7274 0d0a 0d0a 5b65 6767 5f69   short....[egg_i
+000007b0: 6e66 6f5d 0d0a 7461 675f 6275 696c 6420  nfo]..tag_build 
+000007c0: 3d20 0d0a 7461 675f 6461 7465 203d 2030  = ..tag_date = 0
+000007d0: 0d0a 0d0a                                ....
```

### Comparing `torch_max_mem-0.0.4/src/torch_max_mem/api.py` & `torch_max_mem-0.0.5/src/torch_max_mem/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -60,38 +60,14 @@
 __all__ = [
     "maximize_memory_utilization",
 ]
 
 R = TypeVar("R")
 
 
-def is_oom_error(error: RuntimeError) -> bool:
-    """Check whether a runtime error was caused by insufficient memory."""
-    if not error.args:
-        logger.debug(f"Cannot check empty error message for {error}.")
-        return False
-
-    message = error.args[0]
-    logger.debug(f"Checking error for OOM: {message}")
-
-    # CUDA out of memory
-    if "CUDA out of memory." in message:
-        return True
-
-    # CUDA error (dimension was larger than int limit)
-    if "RuntimeError: CUDA error: invalid configuration argument" in message:
-        return True
-
-    # CPU out of memory
-    if "DefaultCPUAllocator: can't allocate memory:" in message:
-        return True
-
-    return False
-
-
 def maximize_memory_utilization_decorator(
     parameter_name: str = "batch_size",
     q: int = 32,
     cpu_warning: bool = True,
 ) -> Callable[[Callable[..., R]], Callable[..., Tuple[R, int]]]:
     """
     Create decorators to create methods for memory utilization maximization.
@@ -163,20 +139,18 @@
                 The positional arguments.
             :param kwargs:
                 The key-word based arguments.
 
             :return:
                 A tuple (result, max_value).
 
-            :raises RuntimeError:
-                any runtime error which was not caused by (CUDA) OOM.
             :raises MemoryError:
                 if the execution did not even succeed with the smallest parameter value
             :raises ValueError:
-                if an invalid  (or no) maximum parameter value is found
+                if an invalid (or no) maximum parameter value is found
             """
             check_for_cpu_tensors(*args, **kwargs)
             bound_arguments = signature.bind(*args, **kwargs)
             bound_arguments.apply_defaults()
             max_value = bound_arguments.arguments.pop(parameter_name, default_max_value)
             if max_value is None:
                 raise ValueError(
@@ -189,22 +163,17 @@
                     parameter_name: max_value,
                 }
                 try:
                     return (
                         func(*bound_arguments.args, **p_kwargs, **bound_arguments.kwargs),
                         max_value,
                     )
-                except RuntimeError as runtime_error:
+                except torch.cuda.OutOfMemoryError:
                     # clear cache
                     torch.cuda.empty_cache()
-
-                    # check whether the error is an out-of-memory error
-                    if not is_oom_error(error=runtime_error):
-                        raise runtime_error
-
                     logger.info(f"Execution failed with {parameter_name}={max_value}")
                     max_value //= 2
                     if max_value > q:
                         max_value = max_value // q * q
             raise MemoryError(f"Execution did not even succeed with {parameter_name}=1.")
 
         return wrapper_maximize_memory_utilization
```

### Comparing `torch_max_mem-0.0.4/src/torch_max_mem/version.py` & `torch_max_mem-0.0.5/src/torch_max_mem/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 __all__ = [
     "VERSION",
     "get_version",
     "get_git_hash",
 ]
 
-VERSION = "0.0.4"
+VERSION = "0.0.5"
 
 
 def get_git_hash() -> str:
     """Get the :mod:`torch_max_mem` git hash."""
     with open(os.devnull, "w") as devnull:
         try:
             ret = check_output(  # noqa: S603,S607
```

### Comparing `torch_max_mem-0.0.4/src/torch_max_mem.egg-info/PKG-INFO` & `torch_max_mem-0.0.5/src/torch_max_mem.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,204 +1,202 @@
-Metadata-Version: 2.1
-Name: torch-max-mem
-Version: 0.0.4
-Summary: Maximize memory utilization with PyTorch.
-Home-page: https://github.com/mberr/torch-max-mem
-Download-URL: https://github.com/mberr/torch-max-mem/releases
-Author: Max Berrendorf
-Author-email: max.berrendorf@gmail.com
-Maintainer: Max Berrendorf
-Maintainer-email: max.berrendorf@gmail.com
-License: MIT
-Project-URL: Bug Tracker, https://github.com/mberr/torch-max-mem/issues
-Project-URL: Source Code, https://github.com/mberr/torch-max-mem
-Keywords: snekpack,cookiecutter,torch
-Platform: UNKNOWN
-Classifier: Development Status :: 1 - Planning
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Framework :: Pytest
-Classifier: Framework :: tox
-Classifier: Framework :: Sphinx
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: tests
-Provides-Extra: docs
-License-File: LICENSE
-
-<!--
-<p align="center">
-  <img src="https://github.com/mberr/torch-max-mem/raw/main/docs/source/logo.png" height="150">
-</p>
--->
-
-<h1 align="center">
-  torch-max-mem
-</h1>
-
-<p align="center">
-    <a href="https://github.com/mberr/torch-max-mem/actions?query=workflow%3ATests">
-        <img alt="Tests" src="https://github.com/mberr/torch-max-mem/workflows/Tests/badge.svg" />
-    </a>
-    <a href="https://github.com/cthoyt/cookiecutter-python-package">
-        <img alt="Cookiecutter template from @cthoyt" src="https://img.shields.io/badge/Cookiecutter-snekpack-blue" /> 
-    </a>
-    <a href="https://pypi.org/project/torch_max_mem">
-        <img alt="PyPI" src="https://img.shields.io/pypi/v/torch_max_mem" />
-    </a>
-    <a href="https://pypi.org/project/torch_max_mem">
-        <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/torch_max_mem" />
-    </a>
-    <a href="https://github.com/mberr/torch-max-mem/blob/main/LICENSE">
-        <img alt="PyPI - License" src="https://img.shields.io/pypi/l/torch_max_mem" />
-    </a>
-    <a href='https://torch_max_mem.readthedocs.io/en/latest/?badge=latest'>
-        <img src='https://readthedocs.org/projects/torch_max_mem/badge/?version=latest' alt='Documentation Status' />
-    </a>
-    <a href='https://github.com/psf/black'>
-        <img src='https://img.shields.io/badge/code%20style-black-000000.svg' alt='Code style: black' />
-    </a>
-</p>
-
-This package provides decorators for memory utilization maximization with PyTorch and CUDA by starting with a maximum parameter size and applying successive halving until no more out-of-memory exception occurs.
-
-## 💪 Getting Started
-
-Assume you have a function for batched computation of nearest neighbors using brute-force distance calculation.
-
-```python
-import torch
-
-def knn(x, y, batch_size, k: int = 3):
-    return torch.cat(
-        [
-            torch.cdist(x[start : start + batch_size], y).topk(k=k, dim=1, largest=False).indices
-            for start in range(0, x.shape[0], batch_size)
-        ],
-        dim=0,
-    )
-```
-
-With `torch_max_mem` you can decorate this function to reduce the batch size until no more out-of-memory error occurs.
-
-```python
-import torch
-from torch_max_mem import maximize_memory_utilization
-
-
-@maximize_memory_utilization()
-def knn(x, y, batch_size, k: int = 3):
-    return torch.cat(
-        [
-            torch.cdist(x[start : start + batch_size], y).topk(k=k, dim=0, largest=False).indices
-            for start in range(0, x.shape[0], batch_size)
-        ],
-        dim=0,
-    )
-```
-
-In the code, you can now always pass the largest sensible batch size, e.g.,
-
-```python
-x = torch.rand(100, 100, device="cuda")
-y = torch.rand(200, 100, device="cuda")
-knn(x, y, batch_size=x.shape[0])
-```
-
-## 🚀 Installation
-
-The most recent release can be installed from
-[PyPI](https://pypi.org/project/torch_max_mem/) with:
-
-```bash
-$ pip install torch_max_mem
-```
-
-The most recent code and data can be installed directly from GitHub with:
-
-```bash
-$ pip install git+https://github.com/mberr/torch-max-mem.git
-```
-
-To install in development mode, use the following:
-
-```bash
-$ git clone git+https://github.com/mberr/torch-max-mem.git
-$ cd torch-max-mem
-$ pip install -e .
-```
-
-## 👐 Contributing
-
-Contributions, whether filing an issue, making a pull request, or forking, are appreciated. See
-[CONTRIBUTING.md](https://github.com/mberr/torch-max-mem/blob/master/CONTRIBUTING.md) for more information on getting involved.
-
-## 👋 Attribution
-
-Parts of the logic have been developed with [Laurent Vermue](https://github.com/lvermue) for [PyKEEN](https://github.com/pykeen/pykeen).
-
-
-### ⚖️ License
-
-The code in this package is licensed under the MIT License.
-
-### 🍪 Cookiecutter
-
-This package was created with [@audreyfeldroy](https://github.com/audreyfeldroy)'s
-[cookiecutter](https://github.com/cookiecutter/cookiecutter) package using [@cthoyt](https://github.com/cthoyt)'s
-[cookiecutter-snekpack](https://github.com/cthoyt/cookiecutter-snekpack) template.
-
-## 🛠️ For Developers
-
-<details>
-  <summary>See developer instrutions</summary>
-
-  
-The final section of the README is for if you want to get involved by making a code contribution.
-
-### 🥼 Testing
-
-After cloning the repository and installing `tox` with `pip install tox`, the unit tests in the `tests/` folder can be
-run reproducibly with:
-
-```shell
-$ tox
-```
-
-Additionally, these tests are automatically re-run with each commit in a [GitHub Action](https://github.com/mberr/torch-max-mem/actions?query=workflow%3ATests).
-
-### 📖 Building the Documentation
-
-```shell
-$ tox -e docs
-``` 
-
-### 📦 Making a Release
-
-After installing the package in development mode and installing
-`tox` with `pip install tox`, the commands for making a new release are contained within the `finish` environment
-in `tox.ini`. Run the following from the shell:
-
-```shell
-$ tox -e finish
-```
-
-This script does the following:
-
-1. Uses [Bump2Version](https://github.com/c4urself/bump2version) to switch the version number in the `setup.cfg` and
-   `src/torch_max_mem/version.py` to not have the `-dev` suffix
-2. Packages the code in both a tar archive and a wheel
-3. Uploads to PyPI using `twine`. Be sure to have a `.pypirc` file configured to avoid the need for manual input at this
-   step
-4. Push to GitHub. You'll need to make a release going with the commit where the version was bumped.
-5. Bump the version to the next patch. If you made big changes and want to bump the version by minor, you can
-   use `tox -e bumpversion minor` after.
-</details>
-
-
+Metadata-Version: 2.1
+Name: torch-max-mem
+Version: 0.0.5
+Summary: Maximize memory utilization with PyTorch.
+Home-page: https://github.com/mberr/torch-max-mem
+Download-URL: https://github.com/mberr/torch-max-mem/releases
+Author: Max Berrendorf
+Author-email: max.berrendorf@gmail.com
+Maintainer: Max Berrendorf
+Maintainer-email: max.berrendorf@gmail.com
+License: MIT
+Project-URL: Bug Tracker, https://github.com/mberr/torch-max-mem/issues
+Project-URL: Source Code, https://github.com/mberr/torch-max-mem
+Keywords: snekpack,cookiecutter,torch
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Framework :: Pytest
+Classifier: Framework :: tox
+Classifier: Framework :: Sphinx
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: tests
+Provides-Extra: docs
+License-File: LICENSE
+
+<!--
+<p align="center">
+  <img src="https://github.com/mberr/torch-max-mem/raw/main/docs/source/logo.png" height="150">
+</p>
+-->
+
+<h1 align="center">
+  torch-max-mem
+</h1>
+
+<p align="center">
+    <a href="https://github.com/mberr/torch-max-mem/actions?query=workflow%3ATests">
+        <img alt="Tests" src="https://github.com/mberr/torch-max-mem/workflows/Tests/badge.svg" />
+    </a>
+    <a href="https://github.com/cthoyt/cookiecutter-python-package">
+        <img alt="Cookiecutter template from @cthoyt" src="https://img.shields.io/badge/Cookiecutter-snekpack-blue" /> 
+    </a>
+    <a href="https://pypi.org/project/torch_max_mem">
+        <img alt="PyPI" src="https://img.shields.io/pypi/v/torch_max_mem" />
+    </a>
+    <a href="https://pypi.org/project/torch_max_mem">
+        <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/torch_max_mem" />
+    </a>
+    <a href="https://github.com/mberr/torch-max-mem/blob/main/LICENSE">
+        <img alt="PyPI - License" src="https://img.shields.io/pypi/l/torch_max_mem" />
+    </a>
+    <a href='https://torch_max_mem.readthedocs.io/en/latest/?badge=latest'>
+        <img src='https://readthedocs.org/projects/torch_max_mem/badge/?version=latest' alt='Documentation Status' />
+    </a>
+    <a href='https://github.com/psf/black'>
+        <img src='https://img.shields.io/badge/code%20style-black-000000.svg' alt='Code style: black' />
+    </a>
+</p>
+
+This package provides decorators for memory utilization maximization with PyTorch and CUDA by starting with a maximum parameter size and applying successive halving until no more out-of-memory exception occurs.
+
+## 💪 Getting Started
+
+Assume you have a function for batched computation of nearest neighbors using brute-force distance calculation.
+
+```python
+import torch
+
+def knn(x, y, batch_size, k: int = 3):
+    return torch.cat(
+        [
+            torch.cdist(x[start : start + batch_size], y).topk(k=k, dim=1, largest=False).indices
+            for start in range(0, x.shape[0], batch_size)
+        ],
+        dim=0,
+    )
+```
+
+With `torch_max_mem` you can decorate this function to reduce the batch size until no more out-of-memory error occurs.
+
+```python
+import torch
+from torch_max_mem import maximize_memory_utilization
+
+
+@maximize_memory_utilization()
+def knn(x, y, batch_size, k: int = 3):
+    return torch.cat(
+        [
+            torch.cdist(x[start : start + batch_size], y).topk(k=k, dim=0, largest=False).indices
+            for start in range(0, x.shape[0], batch_size)
+        ],
+        dim=0,
+    )
+```
+
+In the code, you can now always pass the largest sensible batch size, e.g.,
+
+```python
+x = torch.rand(100, 100, device="cuda")
+y = torch.rand(200, 100, device="cuda")
+knn(x, y, batch_size=x.shape[0])
+```
+
+## 🚀 Installation
+
+The most recent release can be installed from
+[PyPI](https://pypi.org/project/torch_max_mem/) with:
+
+```bash
+$ pip install torch_max_mem
+```
+
+The most recent code and data can be installed directly from GitHub with:
+
+```bash
+$ pip install git+https://github.com/mberr/torch-max-mem.git
+```
+
+To install in development mode, use the following:
+
+```bash
+$ git clone git+https://github.com/mberr/torch-max-mem.git
+$ cd torch-max-mem
+$ pip install -e .
+```
+
+## 👐 Contributing
+
+Contributions, whether filing an issue, making a pull request, or forking, are appreciated. See
+[CONTRIBUTING.md](https://github.com/mberr/torch-max-mem/blob/master/CONTRIBUTING.md) for more information on getting involved.
+
+## 👋 Attribution
+
+Parts of the logic have been developed with [Laurent Vermue](https://github.com/lvermue) for [PyKEEN](https://github.com/pykeen/pykeen).
+
+
+### ⚖️ License
+
+The code in this package is licensed under the MIT License.
+
+### 🍪 Cookiecutter
+
+This package was created with [@audreyfeldroy](https://github.com/audreyfeldroy)'s
+[cookiecutter](https://github.com/cookiecutter/cookiecutter) package using [@cthoyt](https://github.com/cthoyt)'s
+[cookiecutter-snekpack](https://github.com/cthoyt/cookiecutter-snekpack) template.
+
+## 🛠️ For Developers
+
+<details>
+  <summary>See developer instrutions</summary>
+
+  
+The final section of the README is for if you want to get involved by making a code contribution.
+
+### 🥼 Testing
+
+After cloning the repository and installing `tox` with `pip install tox`, the unit tests in the `tests/` folder can be
+run reproducibly with:
+
+```shell
+$ tox
+```
+
+Additionally, these tests are automatically re-run with each commit in a [GitHub Action](https://github.com/mberr/torch-max-mem/actions?query=workflow%3ATests).
+
+### 📖 Building the Documentation
+
+```shell
+$ tox -e docs
+``` 
+
+### 📦 Making a Release
+
+After installing the package in development mode and installing
+`tox` with `pip install tox`, the commands for making a new release are contained within the `finish` environment
+in `tox.ini`. Run the following from the shell:
+
+```shell
+$ tox -e finish
+```
+
+This script does the following:
+
+1. Uses [Bump2Version](https://github.com/c4urself/bump2version) to switch the version number in the `setup.cfg` and
+   `src/torch_max_mem/version.py` to not have the `-dev` suffix
+2. Packages the code in both a tar archive and a wheel
+3. Uploads to PyPI using `twine`. Be sure to have a `.pypirc` file configured to avoid the need for manual input at this
+   step
+4. Push to GitHub. You'll need to make a release going with the commit where the version was bumped.
+5. Bump the version to the next patch. If you made big changes and want to bump the version by minor, you can
+   use `tox -e bumpversion minor` after.
+</details>
```

#### html2text {}

```diff
@@ -1,24 +1,25 @@
-Metadata-Version: 2.1 Name: torch-max-mem Version: 0.0.4 Summary: Maximize
+Metadata-Version: 2.1 Name: torch-max-mem Version: 0.0.5 Summary: Maximize
 memory utilization with PyTorch. Home-page: https://github.com/mberr/torch-max-
 mem Download-URL: https://github.com/mberr/torch-max-mem/releases Author: Max
 Berrendorf Author-email: max.berrendorf@gmail.com Maintainer: Max Berrendorf
 Maintainer-email: max.berrendorf@gmail.com License: MIT Project-URL: Bug
 Tracker, https://github.com/mberr/torch-max-mem/issues Project-URL: Source
 Code, https://github.com/mberr/torch-max-mem Keywords:
-snekpack,cookiecutter,torch Platform: UNKNOWN Classifier: Development Status ::
-1 - Planning Classifier: Environment :: Console Classifier: Intended Audience
-:: Developers Classifier: License :: OSI Approved :: MIT License Classifier:
-Operating System :: OS Independent Classifier: Framework :: Pytest Classifier:
-Framework :: tox Classifier: Framework :: Sphinx Classifier: Programming
-Language :: Python Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3 ::
-Only Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-
-Extra: tests Provides-Extra: docs License-File: LICENSE
+snekpack,cookiecutter,torch Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
+:: OS Independent Classifier: Framework :: Pytest Classifier: Framework :: tox
+Classifier: Framework :: Sphinx Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3 :: Only Requires-Python: >=3.8 Description-Content-
+Type: text/markdown Provides-Extra: tests Provides-Extra: docs License-File:
+LICENSE
                           ****** torch-max-mem ******
  [Tests] [Cookiecutter_template_from_@cthoyt] [PyPI] [PyPI_-_Python_Version]
           [PyPI_-_License] [Documentation_Status] [Code_style:_black]
 This package provides decorators for memory utilization maximization with
 PyTorch and CUDA by starting with a maximum parameter size and applying
 successive halving until no more out-of-memory exception occurs. ## ðª
 Getting Started Assume you have a function for batched computation of nearest
```

### Comparing `torch_max_mem-0.0.4/tests/test_decorator.py` & `torch_max_mem-0.0.5/tests/test_decorator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # -*- coding: utf-8 -*-
 
 """Tests."""
 
 import unittest
 from typing import Optional, Tuple
-from unittest import mock
 
 import numpy.testing
 import pytest
 import torch
 
 from torch_max_mem import maximize_memory_utilization
 from torch_max_mem.api import maximize_memory_utilization_decorator
@@ -89,16 +88,15 @@
     # call with no arg
     func()
 
 
 def test_optimization():
     """Test optimization."""
 
-    @mock.patch("torch_max_mem.api.is_oom_error", lambda error: True)
     @maximize_memory_utilization()
     def func(batch_size: int = 8):
         """Test function."""
         if batch_size > 2:
-            raise RuntimeError()
+            raise torch.cuda.OutOfMemoryError()
         return batch_size
 
     assert func() == 2
```

