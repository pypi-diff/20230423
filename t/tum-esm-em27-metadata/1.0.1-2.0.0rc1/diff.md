# Comparing `tmp/tum_esm_em27_metadata-1.0.1.tar.gz` & `tmp/tum_esm_em27_metadata-2.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tum_esm_em27_metadata-1.0.1.tar", max compression
+gzip compressed data, was "tum_esm_em27_metadata-2.0.0rc1.tar", max compression
```

## Comparing `tum_esm_em27_metadata-1.0.1.tar` & `tum_esm_em27_metadata-2.0.0rc1.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     4711 2023-03-19 15:44:15.943536 tum_esm_em27_metadata-1.0.1/README.md
--rw-r--r--   0        0        0      909 2023-03-19 21:38:16.077297 tum_esm_em27_metadata-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      121 2023-03-19 15:31:01.993849 tum_esm_em27_metadata-1.0.1/tum_esm_em27_metadata/__init__.py
--rw-r--r--   0        0        0     8547 2023-03-19 15:34:34.340807 tum_esm_em27_metadata-1.0.1/tum_esm_em27_metadata/interfaces.py
--rw-r--r--   0        0        0        0 2023-03-13 14:21:55.850518 tum_esm_em27_metadata-1.0.1/tum_esm_em27_metadata/py.typed
--rw-r--r--   0        0        0     4277 2023-03-19 15:29:15.342522 tum_esm_em27_metadata-1.0.1/tum_esm_em27_metadata/types.py
--rw-r--r--   0        0        0     5672 1970-01-01 00:00:00.000000 tum_esm_em27_metadata-1.0.1/setup.py
--rw-r--r--   0        0        0     5382 1970-01-01 00:00:00.000000 tum_esm_em27_metadata-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2826 2023-04-23 11:30:01.572048 tum_esm_em27_metadata-2.0.0rc1/README.md
+-rw-r--r--   0        0        0     1107 2023-04-19 12:07:55.915913 tum_esm_em27_metadata-2.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0      126 2023-04-23 10:28:10.736200 tum_esm_em27_metadata-2.0.0rc1/tum_esm_em27_metadata/__init__.py
+-rw-r--r--   0        0        0     6385 2023-04-23 11:11:29.637459 tum_esm_em27_metadata-2.0.0rc1/tum_esm_em27_metadata/interfaces.py
+-rw-r--r--   0        0        0     2112 2023-04-23 11:12:48.008464 tum_esm_em27_metadata-2.0.0rc1/tum_esm_em27_metadata/loader.py
+-rw-r--r--   0        0        0        0 2023-04-19 09:38:48.570525 tum_esm_em27_metadata-2.0.0rc1/tum_esm_em27_metadata/py.typed
+-rw-r--r--   0        0        0     3910 2023-04-23 11:09:58.388668 tum_esm_em27_metadata-2.0.0rc1/tum_esm_em27_metadata/types.py
+-rw-r--r--   0        0        0     3759 1970-01-01 00:00:00.000000 tum_esm_em27_metadata-2.0.0rc1/setup.py
+-rw-r--r--   0        0        0     3541 1970-01-01 00:00:00.000000 tum_esm_em27_metadata-2.0.0rc1/PKG-INFO
```

### Comparing `tum_esm_em27_metadata-1.0.1/pyproject.toml` & `tum_esm_em27_metadata-2.0.0rc1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "tum_esm_em27_metadata"
-version = "1.0.1"
-description = "single source of truth for ESM's EM27 measurement logistics"
+version = "2.0.0-rc.1"
+description = "Single source of truth for ESM's EM27 measurement logistics"
 readme = "README.md"
 authors = [
     "Moritz Makowski <moritz.makowski@tum.de>",
     "Marlon Mueller <marlon.mueller@tum.de>"
 ]
 packages = [
     {include = "tum_esm_em27_metadata"},
@@ -13,29 +13,37 @@
 ]
 repository = "https://github.com/tum-esm/em27-metadata"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pydantic = "^1.10.4"
 tum-esm-utils = "^1.0.0"
+pendulum = "^2.1.2"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
-mypy = "^0.991"
 pytest = "^7.2.1"
 black = "^22.12.0"
 python-dotenv = "^0.21.1"
+mypy = "^1.2.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length=100
 
 [tool.mypy]
 strict = true
 implicit_reexport = true
 no_warn_unused_ignores = true
 plugins = ["pydantic.mypy"]
+
+[tool.pytest.ini_options]
+markers = [
+    "ci: can be run in GitHub CI",
+    "action: can be run when using this repo as a GitHub Action",
+    "local: can be run locally"
+]
```

