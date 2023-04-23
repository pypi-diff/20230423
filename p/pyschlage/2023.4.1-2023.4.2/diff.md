# Comparing `tmp/pyschlage-2023.4.1.tar.gz` & `tmp/pyschlage-2023.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyschlage-2023.4.1.tar", last modified: Tue Apr 11 01:06:10 2023, max compression
+gzip compressed data, was "pyschlage-2023.4.2.tar", last modified: Sun Apr 23 00:14:32 2023, max compression
```

## Comparing `pyschlage-2023.4.1.tar` & `pyschlage-2023.4.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:06:10.969962 pyschlage-2023.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/.devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:06:10.965962 pyschlage-2023.4.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:06:10.965962 pyschlage-2023.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/.github/workflows/build-and-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/.github/workflows/publish-python.yml
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:06:10.965962 pyschlage-2023.4.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-11 01:06:10.969962 pyschlage-2023.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:06:10.965962 pyschlage-2023.4.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:06:10.969962 pyschlage-2023.4.1/pyschlage/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/pyschlage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-11 01:06:10.000000 pyschlage-2023.4.1/pyschlage/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/pyschlage/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/pyschlage/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     8091 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/pyschlage/code.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/pyschlage/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/pyschlage/device.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/pyschlage/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/pyschlage/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/pyschlage/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/pyschlage/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:06:10.969962 pyschlage-2023.4.1/pyschlage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-11 01:06:10.000000 pyschlage-2023.4.1/pyschlage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-11 01:06:10.000000 pyschlage-2023.4.1/pyschlage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 01:06:10.000000 pyschlage-2023.4.1/pyschlage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-11 01:06:10.000000 pyschlage-2023.4.1/pyschlage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-11 01:06:10.000000 pyschlage-2023.4.1/pyschlage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 01:06:10.000000 pyschlage-2023.4.1/pyschlage.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:06:10.969962 pyschlage-2023.4.1/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      324 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/scripts/setup
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 01:06:10.969962 pyschlage-2023.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:06:10.969962 pyschlage-2023.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/tests/test_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/tests/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/tests/test_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/tests/test_user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:14:32.068046 pyschlage-2023.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/.devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:14:32.064046 pyschlage-2023.4.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:14:32.064046 pyschlage-2023.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/.github/workflows/build-and-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/.github/workflows/publish-python.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:14:32.064046 pyschlage-2023.4.2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-23 00:14:32.068046 pyschlage-2023.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:14:32.064046 pyschlage-2023.4.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:14:32.068046 pyschlage-2023.4.2/pyschlage/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/pyschlage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-23 00:14:31.000000 pyschlage-2023.4.2/pyschlage/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/pyschlage/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/pyschlage/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8091 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/pyschlage/code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/pyschlage/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/pyschlage/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/pyschlage/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/pyschlage/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/pyschlage/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/pyschlage/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:14:32.068046 pyschlage-2023.4.2/pyschlage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-23 00:14:32.000000 pyschlage-2023.4.2/pyschlage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-23 00:14:32.000000 pyschlage-2023.4.2/pyschlage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 00:14:32.000000 pyschlage-2023.4.2/pyschlage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-23 00:14:32.000000 pyschlage-2023.4.2/pyschlage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-23 00:14:32.000000 pyschlage-2023.4.2/pyschlage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 00:14:31.000000 pyschlage-2023.4.2/pyschlage.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:14:32.068046 pyschlage-2023.4.2/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      324 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/scripts/setup
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 00:14:32.068046 pyschlage-2023.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:14:32.068046 pyschlage-2023.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/tests/test_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/tests/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/tests/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-23 00:14:08.000000 pyschlage-2023.4.2/tests/test_user.py
```

### Comparing `pyschlage-2023.4.1/.devcontainer.json` & `pyschlage-2023.4.2/.devcontainer.json`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.1/.github/workflows/build-and-test.yml` & `pyschlage-2023.4.2/.github/workflows/build-and-test.yml`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.1/.github/workflows/publish-python.yml` & `pyschlage-2023.4.2/.github/workflows/publish-python.yml`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.1/.gitignore` & `pyschlage-2023.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.1/.pre-commit-config.yaml` & `pyschlage-2023.4.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.1/LICENSE` & `pyschlage-2023.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.1/PKG-INFO` & `pyschlage-2023.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyschlage
-Version: 2023.4.1
+Version: 2023.4.2
 Summary: Python API for interacting with Schlage WiFi locks.
 Author-email: David Knowles <dknowles2@gmail.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/dknowles2/pyschlage
 Project-URL: Source Code, https://github.com/dknowles2/pyschlage
 Project-URL: Bug Reports, https://github.com/dknowles2/pyschlage/issues
 Project-URL: Documentation, https://pyschlage.readthedocs.io
```

### Comparing `pyschlage-2023.4.1/README.md` & `pyschlage-2023.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.1/docs/Makefile` & `pyschlage-2023.4.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.1/docs/api.rst` & `pyschlage-2023.4.2/docs/api.rst`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.1/docs/index.rst` & `pyschlage-2023.4.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.1/docs/make.bat` & `pyschlage-2023.4.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.1/pyproject.toml` & `pyschlage-2023.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.1/pyschlage/api.py` & `pyschlage-2023.4.2/pyschlage/api.py`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.1/pyschlage/auth.py` & `pyschlage-2023.4.2/pyschlage/auth.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Authentication support for the Schlage WiFi cloud service."""
 
 from __future__ import annotations
 
 from functools import wraps
+from typing import Any, Callable, Union
 
 from botocore.exceptions import ClientError
 import pycognito
 from pycognito import utils
 import requests
 
 from .exceptions import NotAuthorizedError, UnknownError
@@ -23,15 +24,19 @@
 BASE_URL = "https://api.allegion.yonomi.cloud/v1"
 CLIENT_ID = "t5836cptp2s1il0u9lki03j5"
 CLIENT_SECRET = "1kfmt18bgaig51in4j4v1j3jbe7ioqtjhle5o6knqc5dat0tpuvo"
 USER_POOL_REGION = "us-west-2"
 USER_POOL_ID = USER_POOL_REGION + "_2zhrVs9d4"
 
 
-def translate_errors(fn):
+def _translate_auth_errors(
+    # pylint: disable=invalid-name
+    fn: Callable[..., Union[requests.Request, requests.Response]]
+    # pylint: enable=invalid-name
+) -> Callable[..., Union[requests.Request, requests.Response]]:
     @wraps(fn)
     def wrapper(*args, **kwargs):
         try:
             return fn(*args, **kwargs)
         except ClientError as ex:
             resp_err = ex.response.get("Error", {})
             if resp_err.get("Code") in _NOT_AUTHORIZED_ERRORS:
@@ -39,14 +44,38 @@
                     resp_err.get("Message", "Not authorized")
                 ) from ex
             raise UnknownError(str(ex)) from ex
 
     return wrapper
 
 
+def _translate_http_errors(
+    # pylint: disable=invalid-name
+    fn: Callable[..., requests.Response]
+    # pylint: enable=invalid-name
+) -> Callable[..., requests.Response]:
+    @wraps(fn)
+    def wrapper(*args, **kwargs):
+        resp: requests.Response = fn(*args, **kwargs)
+        try:
+            resp.raise_for_status()
+            return resp
+        except requests.HTTPError as ex:
+            try:
+                message = resp.json().get("message", resp.reason)
+            except requests.JSONDecodeError:
+                message = resp.reason
+
+            if resp.status_code == 401:
+                raise NotAuthorizedError(message) from ex
+            raise UnknownError(message) from ex
+
+    return wrapper
+
+
 class Auth:
     """Handles authentication for the Schlage WiFi cloud service."""
 
     def __init__(self, username: str, password: str) -> None:
         """Initializes an Auth object.
 
         :param username: The username associated with the Schlage account.
@@ -63,15 +92,15 @@
         )
         self.auth = utils.RequestsSrpAuth(
             password=password,
             cognito=self.cognito,
         )
         self._user_id: str | None = None
 
-    @translate_errors
+    @_translate_auth_errors
     def authenticate(self):
         """Performs authentication with AWS.
 
         :raise pyschlage.exceptions.NotAuthorizedError: When authentication fails.
         :raise pyschlage.exceptions.UnknownError: On other errors.
         """
         self.auth(requests.Request())
@@ -83,21 +112,23 @@
             self._user_id = self._get_user_id()
         return self._user_id
 
     def _get_user_id(self) -> str:
         resp = self.request("get", "users/@me")
         return resp.json()["identityId"]
 
-    @translate_errors
+    @_translate_http_errors
+    @_translate_auth_errors
     def request(
         self, method: str, path: str, base_url: str = BASE_URL, **kwargs
     ) -> requests.Response:
         """Performs a request against the Schlage WiFi cloud service.
 
         :meta private:
         """
         kwargs["auth"] = self.auth
         if "headers" not in kwargs:
             kwargs["headers"] = {}
         kwargs["headers"]["X-Api-Key"] = API_KEY
         kwargs.setdefault("timeout", _DEFAULT_TIMEOUT)
+        # pylint: disable=missing-timeout
         return requests.request(method, f"{base_url}/{path.lstrip('/')}", **kwargs)
```

### Comparing `pyschlage-2023.4.1/pyschlage/code.py` & `pyschlage-2023.4.2/pyschlage/code.py`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.1/pyschlage/common.py` & `pyschlage-2023.4.2/pyschlage/common.py`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.1/pyschlage/device.py` & `pyschlage-2023.4.2/pyschlage/device.py`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.1/pyschlage/lock.py` & `pyschlage-2023.4.2/pyschlage/lock.py`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.1/pyschlage/log.py` & `pyschlage-2023.4.2/pyschlage/log.py`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.1/pyschlage/user.py` & `pyschlage-2023.4.2/pyschlage/user.py`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.1/pyschlage.egg-info/PKG-INFO` & `pyschlage-2023.4.2/pyschlage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyschlage
-Version: 2023.4.1
+Version: 2023.4.2
 Summary: Python API for interacting with Schlage WiFi locks.
 Author-email: David Knowles <dknowles2@gmail.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/dknowles2/pyschlage
 Project-URL: Source Code, https://github.com/dknowles2/pyschlage
 Project-URL: Bug Reports, https://github.com/dknowles2/pyschlage/issues
 Project-URL: Documentation, https://pyschlage.readthedocs.io
```

### Comparing `pyschlage-2023.4.1/pyschlage.egg-info/SOURCES.txt` & `pyschlage-2023.4.2/pyschlage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.1/tests/conftest.py` & `pyschlage-2023.4.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.1/tests/test_code.py` & `pyschlage-2023.4.2/tests/test_code.py`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.1/tests/test_lock.py` & `pyschlage-2023.4.2/tests/test_lock.py`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.1/tests/test_log.py` & `pyschlage-2023.4.2/tests/test_log.py`

 * *Files identical despite different names*

