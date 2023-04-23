# Comparing `tmp/dank_mids-4.20.8.tar.gz` & `tmp/dank_mids-4.20.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dank_mids-4.20.8.tar", last modified: Mon Oct 17 11:35:36 2022, max compression
+gzip compressed data, was "dank_mids-4.20.9.tar", last modified: Wed Oct 19 17:56:40 2022, max compression
```

## Comparing `dank_mids-4.20.8.tar` & `dank_mids-4.20.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 11:35:36.032503 dank_mids-4.20.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 11:35:36.028503 dank_mids-4.20.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 11:35:36.032503 dank_mids-4.20.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      545 2022-10-17 11:35:22.000000 dank_mids-4.20.8/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1217 2022-10-17 11:35:22.000000 dank_mids-4.20.8/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      609 2022-10-17 11:35:22.000000 dank_mids-4.20.8/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-10-17 11:35:22.000000 dank_mids-4.20.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      263 2022-10-17 11:35:36.032503 dank_mids-4.20.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1158 2022-10-17 11:35:22.000000 dank_mids-4.20.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 11:35:36.032503 dank_mids-4.20.8/dank_mids/
--rw-r--r--   0 runner    (1001) docker     (121)      162 2022-10-17 11:35:22.000000 dank_mids-4.20.8/dank_mids/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      560 2022-10-17 11:35:22.000000 dank_mids-4.20.8/dank_mids/_config.py
--rw-r--r--   0 runner    (1001) docker     (121)      331 2022-10-17 11:35:22.000000 dank_mids-4.20.8/dank_mids/_demo_mode.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 11:35:36.032503 dank_mids-4.20.8/dank_mids/brownie_patch/
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-10-17 11:35:22.000000 dank_mids-4.20.8/dank_mids/brownie_patch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3016 2022-10-17 11:35:22.000000 dank_mids-4.20.8/dank_mids/brownie_patch/call.py
--rw-r--r--   0 runner    (1001) docker     (121)      981 2022-10-17 11:35:22.000000 dank_mids-4.20.8/dank_mids/brownie_patch/contract.py
--rw-r--r--   0 runner    (1001) docker     (121)     1186 2022-10-17 11:35:22.000000 dank_mids-4.20.8/dank_mids/brownie_patch/overloaded.py
--rw-r--r--   0 runner    (1001) docker     (121)     4784 2022-10-17 11:35:22.000000 dank_mids-4.20.8/dank_mids/call.py
--rw-r--r--   0 runner    (1001) docker     (121)     2971 2022-10-17 11:35:22.000000 dank_mids-4.20.8/dank_mids/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     4685 2022-10-17 11:35:22.000000 dank_mids-4.20.8/dank_mids/controller.py
--rw-r--r--   0 runner    (1001) docker     (121)      793 2022-10-17 11:35:22.000000 dank_mids-4.20.8/dank_mids/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)      237 2022-10-17 11:35:22.000000 dank_mids-4.20.8/dank_mids/loggers.py
--rw-r--r--   0 runner    (1001) docker     (121)      615 2022-10-17 11:35:22.000000 dank_mids-4.20.8/dank_mids/middleware.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-17 11:35:22.000000 dank_mids-4.20.8/dank_mids/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)      995 2022-10-17 11:35:22.000000 dank_mids-4.20.8/dank_mids/types.py
--rw-r--r--   0 runner    (1001) docker     (121)      465 2022-10-17 11:35:22.000000 dank_mids-4.20.8/dank_mids/uid.py
--rw-r--r--   0 runner    (1001) docker     (121)    11199 2022-10-17 11:35:22.000000 dank_mids-4.20.8/dank_mids/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 11:35:36.032503 dank_mids-4.20.8/dank_mids.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      263 2022-10-17 11:35:35.000000 dank_mids-4.20.8/dank_mids.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      874 2022-10-17 11:35:35.000000 dank_mids-4.20.8/dank_mids.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-17 11:35:35.000000 dank_mids-4.20.8/dank_mids.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-10-17 11:35:35.000000 dank_mids-4.20.8/dank_mids.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-10-17 11:35:35.000000 dank_mids-4.20.8/dank_mids.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-10-17 11:35:22.000000 dank_mids-4.20.8/license
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-10-17 11:35:22.000000 dank_mids-4.20.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-10-17 11:35:22.000000 dank_mids-4.20.8/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-10-17 11:35:22.000000 dank_mids-4.20.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-10-17 11:35:36.032503 dank_mids-4.20.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      827 2022-10-17 11:35:22.000000 dank_mids-4.20.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 11:35:36.032503 dank_mids-4.20.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-17 11:35:22.000000 dank_mids-4.20.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      175 2022-10-17 11:35:22.000000 dank_mids-4.20.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)      113 2022-10-17 11:35:22.000000 dank_mids-4.20.8/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (121)     1453 2022-10-17 11:35:22.000000 dank_mids-4.20.8/tests/test_brownie_patch.py
--rw-r--r--   0 runner    (1001) docker     (121)     2821 2022-10-17 11:35:22.000000 dank_mids-4.20.8/tests/test_dank_mids.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 17:56:40.680519 dank_mids-4.20.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 17:56:40.676519 dank_mids-4.20.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 17:56:40.676519 dank_mids-4.20.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)      545 2022-10-19 17:56:26.000000 dank_mids-4.20.9/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1217 2022-10-19 17:56:26.000000 dank_mids-4.20.9/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      609 2022-10-19 17:56:26.000000 dank_mids-4.20.9/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)       89 2022-10-19 17:56:26.000000 dank_mids-4.20.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      263 2022-10-19 17:56:40.680519 dank_mids-4.20.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1158 2022-10-19 17:56:26.000000 dank_mids-4.20.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 17:56:40.680519 dank_mids-4.20.9/dank_mids/
+-rw-r--r--   0 runner    (1001) docker     (121)      162 2022-10-19 17:56:26.000000 dank_mids-4.20.9/dank_mids/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      560 2022-10-19 17:56:26.000000 dank_mids-4.20.9/dank_mids/_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)      331 2022-10-19 17:56:26.000000 dank_mids-4.20.9/dank_mids/_demo_mode.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 17:56:40.680519 dank_mids-4.20.9/dank_mids/brownie_patch/
+-rw-r--r--   0 runner    (1001) docker     (121)       61 2022-10-19 17:56:26.000000 dank_mids-4.20.9/dank_mids/brownie_patch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3016 2022-10-19 17:56:26.000000 dank_mids-4.20.9/dank_mids/brownie_patch/call.py
+-rw-r--r--   0 runner    (1001) docker     (121)      981 2022-10-19 17:56:26.000000 dank_mids-4.20.9/dank_mids/brownie_patch/contract.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1186 2022-10-19 17:56:26.000000 dank_mids-4.20.9/dank_mids/brownie_patch/overloaded.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4784 2022-10-19 17:56:26.000000 dank_mids-4.20.9/dank_mids/call.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2971 2022-10-19 17:56:26.000000 dank_mids-4.20.9/dank_mids/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4685 2022-10-19 17:56:26.000000 dank_mids-4.20.9/dank_mids/controller.py
+-rw-r--r--   0 runner    (1001) docker     (121)      793 2022-10-19 17:56:26.000000 dank_mids-4.20.9/dank_mids/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)      237 2022-10-19 17:56:26.000000 dank_mids-4.20.9/dank_mids/loggers.py
+-rw-r--r--   0 runner    (1001) docker     (121)      615 2022-10-19 17:56:26.000000 dank_mids-4.20.9/dank_mids/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 17:56:26.000000 dank_mids-4.20.9/dank_mids/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)      995 2022-10-19 17:56:26.000000 dank_mids-4.20.9/dank_mids/types.py
+-rw-r--r--   0 runner    (1001) docker     (121)      465 2022-10-19 17:56:26.000000 dank_mids-4.20.9/dank_mids/uid.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11199 2022-10-19 17:56:26.000000 dank_mids-4.20.9/dank_mids/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 17:56:40.680519 dank_mids-4.20.9/dank_mids.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      263 2022-10-19 17:56:40.000000 dank_mids-4.20.9/dank_mids.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      874 2022-10-19 17:56:40.000000 dank_mids-4.20.9/dank_mids.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-19 17:56:40.000000 dank_mids-4.20.9/dank_mids.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       60 2022-10-19 17:56:40.000000 dank_mids-4.20.9/dank_mids.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-10-19 17:56:40.000000 dank_mids-4.20.9/dank_mids.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-10-19 17:56:26.000000 dank_mids-4.20.9/license
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2022-10-19 17:56:26.000000 dank_mids-4.20.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-10-19 17:56:26.000000 dank_mids-4.20.9/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-10-19 17:56:26.000000 dank_mids-4.20.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2022-10-19 17:56:40.680519 dank_mids-4.20.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      778 2022-10-19 17:56:26.000000 dank_mids-4.20.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 17:56:40.680519 dank_mids-4.20.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 17:56:26.000000 dank_mids-4.20.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      175 2022-10-19 17:56:26.000000 dank_mids-4.20.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      113 2022-10-19 17:56:26.000000 dank_mids-4.20.9/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1453 2022-10-19 17:56:26.000000 dank_mids-4.20.9/tests/test_brownie_patch.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2310 2022-10-19 17:56:26.000000 dank_mids-4.20.9/tests/test_dank_mids.py
```

### Comparing `dank_mids-4.20.8/.github/workflows/mypy.yaml` & `dank_mids-4.20.9/.github/workflows/mypy.yaml`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.8/.github/workflows/pytest.yaml` & `dank_mids-4.20.9/.github/workflows/pytest.yaml`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.8/.github/workflows/release.yaml` & `dank_mids-4.20.9/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.8/README.md` & `dank_mids-4.20.9/README.md`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.8/dank_mids/_config.py` & `dank_mids-4.20.9/dank_mids/_config.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.8/dank_mids/brownie_patch/call.py` & `dank_mids-4.20.9/dank_mids/brownie_patch/call.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.8/dank_mids/brownie_patch/contract.py` & `dank_mids-4.20.9/dank_mids/brownie_patch/contract.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.8/dank_mids/brownie_patch/overloaded.py` & `dank_mids-4.20.9/dank_mids/brownie_patch/overloaded.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.8/dank_mids/call.py` & `dank_mids-4.20.9/dank_mids/call.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.8/dank_mids/constants.py` & `dank_mids-4.20.9/dank_mids/constants.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.8/dank_mids/controller.py` & `dank_mids-4.20.9/dank_mids/controller.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.8/dank_mids/helpers.py` & `dank_mids-4.20.9/dank_mids/helpers.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.8/dank_mids/middleware.py` & `dank_mids-4.20.9/dank_mids/middleware.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.8/dank_mids/types.py` & `dank_mids-4.20.9/dank_mids/types.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.8/dank_mids/worker.py` & `dank_mids-4.20.9/dank_mids/worker.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.8/dank_mids.egg-info/SOURCES.txt` & `dank_mids-4.20.9/dank_mids.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.8/license` & `dank_mids-4.20.9/license`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.8/tests/test_brownie_patch.py` & `dank_mids-4.20.9/tests/test_brownie_patch.py`

 * *Files identical despite different names*

