# Comparing `tmp/pyhanko-certvalidator-0.21.2.tar.gz` & `tmp/pyhanko-certvalidator-0.22.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhanko-certvalidator-0.21.2.tar", last modified: Mon Apr 17 21:55:20 2023, max compression
+gzip compressed data, was "pyhanko-certvalidator-0.22.0.tar", last modified: Sun Apr 23 17:17:01 2023, max compression
```

## Comparing `pyhanko-certvalidator-0.21.2.tar` & `pyhanko-certvalidator-0.22.0.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 matthias   (501) staff       (20)        0 2023-04-17 21:55:20.102492 pyhanko-certvalidator-0.21.2/
--rw-r--r--   0 matthias   (501) staff       (20)     1138 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.2/LICENSE
--rw-r--r--   0 matthias   (501) staff       (20)     4817 2023-04-17 21:55:20.102348 pyhanko-certvalidator-0.21.2/PKG-INFO
--rw-r--r--   0 matthias   (501) staff       (20)     3864 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.2/README.md
-drwxr-xr-x   0 matthias   (501) staff       (20)        0 2023-04-17 21:55:20.096996 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/
--rw-r--r--   0 matthias   (501) staff       (20)    11707 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/__init__.py
--rw-r--r--   0 matthias   (501) staff       (20)     1141 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/_asyncio_compat.py
--rw-r--r--   0 matthias   (501) staff       (20)     2578 2023-04-01 15:28:48.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/_state.py
--rw-r--r--   0 matthias   (501) staff       (20)      481 2022-05-24 17:45:42.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/_types.py
--rw-r--r--   0 matthias   (501) staff       (20)     2909 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/asn1_types.py
--rw-r--r--   0 matthias   (501) staff       (20)     8798 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/authority.py
--rw-r--r--   0 matthias   (501) staff       (20)    24845 2023-02-21 22:28:44.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/context.py
--rw-r--r--   0 matthias   (501) staff       (20)     5209 2023-04-02 09:14:52.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/errors.py
-drwxr-xr-x   0 matthias   (501) staff       (20)        0 2023-04-17 21:55:20.097972 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/
--rw-r--r--   0 matthias   (501) staff       (20)      491 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/__init__.py
-drwxr-xr-x   0 matthias   (501) staff       (20)        0 2023-04-17 21:55:20.098594 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/aiohttp_fetchers/
--rw-r--r--   0 matthias   (501) staff       (20)     1257 2023-02-21 22:28:44.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/aiohttp_fetchers/__init__.py
--rw-r--r--   0 matthias   (501) staff       (20)     4955 2023-02-21 22:28:44.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/aiohttp_fetchers/cert_fetch_client.py
--rw-r--r--   0 matthias   (501) staff       (20)     3983 2023-02-21 22:28:44.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/aiohttp_fetchers/crl_client.py
--rw-r--r--   0 matthias   (501) staff       (20)     4424 2023-02-21 22:28:44.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/aiohttp_fetchers/ocsp_client.py
--rw-r--r--   0 matthias   (501) staff       (20)     1846 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/aiohttp_fetchers/util.py
--rw-r--r--   0 matthias   (501) staff       (20)     6622 2023-02-21 22:28:45.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/api.py
--rw-r--r--   0 matthias   (501) staff       (20)    10682 2023-02-21 22:28:44.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/common_utils.py
-drwxr-xr-x   0 matthias   (501) staff       (20)        0 2023-04-17 21:55:20.099275 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/requests_fetchers/
--rw-r--r--   0 matthias   (501) staff       (20)     1019 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/requests_fetchers/__init__.py
--rw-r--r--   0 matthias   (501) staff       (20)     4510 2023-04-17 21:02:32.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/requests_fetchers/cert_fetch_client.py
--rw-r--r--   0 matthias   (501) staff       (20)     2603 2023-02-21 22:28:44.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/requests_fetchers/crl_client.py
--rw-r--r--   0 matthias   (501) staff       (20)     3482 2023-02-21 22:28:44.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/requests_fetchers/ocsp_client.py
--rw-r--r--   0 matthias   (501) staff       (20)     2464 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/requests_fetchers/util.py
-drwxr-xr-x   0 matthias   (501) staff       (20)        0 2023-04-17 21:55:20.100149 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/ltv/
--rw-r--r--   0 matthias   (501) staff       (20)        0 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/ltv/__init__.py
--rw-r--r--   0 matthias   (501) staff       (20)     6053 2023-04-02 09:14:52.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/ltv/ades_past.py
--rw-r--r--   0 matthias   (501) staff       (20)      235 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/ltv/errors.py
--rw-r--r--   0 matthias   (501) staff       (20)     3280 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/ltv/poe.py
--rw-r--r--   0 matthias   (501) staff       (20)    16108 2023-03-21 22:12:59.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/ltv/time_slide.py
--rw-r--r--   0 matthias   (501) staff       (20)     1464 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/ltv/types.py
--rw-r--r--   0 matthias   (501) staff       (20)    13166 2023-02-21 22:28:45.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/name_trees.py
--rw-r--r--   0 matthias   (501) staff       (20)    12224 2023-02-21 22:28:44.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/path.py
--rw-r--r--   0 matthias   (501) staff       (20)    19124 2023-04-02 09:14:52.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/policy_decl.py
--rw-r--r--   0 matthias   (501) staff       (20)    10970 2023-02-21 22:28:45.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/policy_tree.py
--rw-r--r--   0 matthias   (501) staff       (20)        0 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/py.typed
--rw-r--r--   0 matthias   (501) staff       (20)    22057 2023-02-21 22:28:44.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/registry.py
-drwxr-xr-x   0 matthias   (501) staff       (20)        0 2023-04-17 21:55:20.100964 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/revinfo/
--rw-r--r--   0 matthias   (501) staff       (20)        0 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/revinfo/__init__.py
--rw-r--r--   0 matthias   (501) staff       (20)    13846 2023-04-17 21:02:32.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/revinfo/archival.py
--rw-r--r--   0 matthias   (501) staff       (20)      567 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/revinfo/constants.py
--rw-r--r--   0 matthias   (501) staff       (20)     8178 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/revinfo/manager.py
--rw-r--r--   0 matthias   (501) staff       (20)    47720 2023-02-21 22:28:44.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/revinfo/validate_crl.py
--rw-r--r--   0 matthias   (501) staff       (20)    23041 2023-02-21 22:28:44.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/revinfo/validate_ocsp.py
--rw-r--r--   0 matthias   (501) staff       (20)    10347 2023-04-01 15:33:21.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/util.py
--rw-r--r--   0 matthias   (501) staff       (20)    55273 2023-04-02 09:14:52.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/validate.py
--rw-r--r--   0 matthias   (501) staff       (20)       71 2023-04-17 21:53:26.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/version.py
-drwxr-xr-x   0 matthias   (501) staff       (20)        0 2023-04-17 21:55:20.097613 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator.egg-info/
--rw-r--r--   0 matthias   (501) staff       (20)     4817 2023-04-17 21:55:20.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator.egg-info/PKG-INFO
--rw-r--r--   0 matthias   (501) staff       (20)     2307 2023-04-17 21:55:20.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator.egg-info/SOURCES.txt
--rw-r--r--   0 matthias   (501) staff       (20)        1 2023-04-17 21:55:20.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator.egg-info/dependency_links.txt
--rw-r--r--   0 matthias   (501) staff       (20)      218 2023-04-17 21:55:20.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator.egg-info/requires.txt
--rw-r--r--   0 matthias   (501) staff       (20)       22 2023-04-17 21:55:20.000000 pyhanko-certvalidator-0.21.2/pyhanko_certvalidator.egg-info/top_level.txt
--rw-r--r--   0 matthias   (501) staff       (20)     2099 2023-03-08 19:43:30.000000 pyhanko-certvalidator-0.21.2/pyproject.toml
--rw-r--r--   0 matthias   (501) staff       (20)       38 2023-04-17 21:55:20.102534 pyhanko-certvalidator-0.21.2/setup.cfg
-drwxr-xr-x   0 matthias   (501) staff       (20)        0 2023-04-17 21:55:20.102123 pyhanko-certvalidator-0.21.2/tests/
--rw-r--r--   0 matthias   (501) staff       (20)    18398 2023-04-01 15:28:58.000000 pyhanko-certvalidator-0.21.2/tests/test_ac_validate.py
--rw-r--r--   0 matthias   (501) staff       (20)    12665 2023-02-21 22:28:44.000000 pyhanko-certvalidator-0.21.2/tests/test_ades_time_slide.py
--rw-r--r--   0 matthias   (501) staff       (20)     5291 2023-04-01 15:28:58.000000 pyhanko-certvalidator-0.21.2/tests/test_certificate_validator.py
--rw-r--r--   0 matthias   (501) staff       (20)     1247 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.2/tests/test_crl_client.py
--rw-r--r--   0 matthias   (501) staff       (20)     7376 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.2/tests/test_freshness.py
--rw-r--r--   0 matthias   (501) staff       (20)     3220 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.2/tests/test_ocsp_client.py
--rw-r--r--   0 matthias   (501) staff       (20)     7054 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.2/tests/test_policy_proc.py
--rw-r--r--   0 matthias   (501) staff       (20)     2042 2023-02-03 18:48:11.000000 pyhanko-certvalidator-0.21.2/tests/test_registry.py
--rw-r--r--   0 matthias   (501) staff       (20)    22461 2023-04-17 21:36:08.000000 pyhanko-certvalidator-0.21.2/tests/test_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:17:01.880287 pyhanko-certvalidator-0.22.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-04-23 17:17:01.880287 pyhanko-certvalidator-0.22.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:17:01.872284 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/
+-rw-r--r--   0 runner    (1001) docker     (123)    11707 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/_asyncio_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/asn1_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/authority.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24845 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:17:01.876286 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:17:01.876286 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/aiohttp_fetchers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/aiohttp_fetchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/aiohttp_fetchers/cert_fetch_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/aiohttp_fetchers/crl_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/aiohttp_fetchers/ocsp_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/aiohttp_fetchers/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10682 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/common_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:17:01.876286 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/requests_fetchers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/requests_fetchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/requests_fetchers/cert_fetch_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/requests_fetchers/crl_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/requests_fetchers/ocsp_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/requests_fetchers/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:17:01.876286 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/ltv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/ltv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/ltv/ades_past.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/ltv/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/ltv/poe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16108 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/ltv/time_slide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/ltv/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/name_trees.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12224 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19124 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/policy_decl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10970 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/policy_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22057 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:17:01.880287 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/revinfo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/revinfo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13846 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/revinfo/archival.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/revinfo/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8178 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/revinfo/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47720 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/revinfo/validate_crl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23041 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/revinfo/validate_ocsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10347 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55273 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:17:01.872284 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-04-23 17:17:01.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-23 17:17:01.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 17:17:01.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-23 17:17:01.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-23 17:17:01.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 17:17:01.880287 pyhanko-certvalidator-0.22.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:17:01.880287 pyhanko-certvalidator-0.22.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    18398 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/tests/test_ac_validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12665 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/tests/test_ades_time_slide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/tests/test_certificate_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/tests/test_crl_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/tests/test_freshness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/tests/test_ocsp_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/tests/test_policy_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22461 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/tests/test_validate.py
```

### Comparing `pyhanko-certvalidator-0.21.2/LICENSE` & `pyhanko-certvalidator-0.22.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.2/PKG-INFO` & `pyhanko-certvalidator-0.22.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhanko-certvalidator
-Version: 0.21.2
+Version: 0.22.0
 Summary: Validates X.509 certificates and paths; forked from wbond/certvalidator
 Author-email: Matthias Valvekens <dev@mvalvekens.be>
 License: MIT
 Project-URL: Homepage, https://github.com/MatthiasValvekens/certvalidator
 Keywords: crypto,pki,x509,certificate,crl,ocsp
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Security :: Cryptography
 Description-Content-Type: text/markdown
-Provides-Extra: async_http
+Provides-Extra: async-http
 Provides-Extra: testing
 Provides-Extra: mypy
 License-File: LICENSE
 
 # certvalidator
 
 This library started as a fork of [wbond/certvalidator](https://github.com/wbond/certvalidator) with patches for [pyHanko](https://github.com/MatthiasValvekens/pyHanko), but has since diverged considerably from its parent repository.
```

### Comparing `pyhanko-certvalidator-0.21.2/README.md` & `pyhanko-certvalidator-0.22.0/README.md`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/__init__.py` & `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/__init__.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/_asyncio_compat.py` & `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/_asyncio_compat.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/_state.py` & `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/_state.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/asn1_types.py` & `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/asn1_types.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/authority.py` & `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/authority.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/context.py` & `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/context.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/errors.py` & `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/errors.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/aiohttp_fetchers/__init__.py` & `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/aiohttp_fetchers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/aiohttp_fetchers/cert_fetch_client.py` & `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/aiohttp_fetchers/cert_fetch_client.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/aiohttp_fetchers/crl_client.py` & `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/aiohttp_fetchers/crl_client.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/aiohttp_fetchers/ocsp_client.py` & `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/aiohttp_fetchers/ocsp_client.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/aiohttp_fetchers/util.py` & `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/aiohttp_fetchers/util.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/api.py` & `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/api.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/common_utils.py` & `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/common_utils.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/requests_fetchers/__init__.py` & `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/requests_fetchers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/requests_fetchers/cert_fetch_client.py` & `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/requests_fetchers/cert_fetch_client.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/requests_fetchers/crl_client.py` & `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/requests_fetchers/crl_client.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/requests_fetchers/ocsp_client.py` & `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/requests_fetchers/ocsp_client.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/fetchers/requests_fetchers/util.py` & `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/requests_fetchers/util.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/ltv/ades_past.py` & `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/ltv/ades_past.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/ltv/poe.py` & `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/ltv/poe.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/ltv/time_slide.py` & `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/ltv/time_slide.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/ltv/types.py` & `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/ltv/types.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/name_trees.py` & `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/name_trees.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/path.py` & `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/path.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/policy_decl.py` & `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/policy_decl.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/policy_tree.py` & `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/policy_tree.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/registry.py` & `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/registry.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/revinfo/archival.py` & `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/revinfo/archival.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/revinfo/constants.py` & `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/revinfo/constants.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/revinfo/manager.py` & `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/revinfo/manager.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/revinfo/validate_crl.py` & `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/revinfo/validate_crl.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/revinfo/validate_ocsp.py` & `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/revinfo/validate_ocsp.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/util.py` & `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/util.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator/validate.py` & `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/validate.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator.egg-info/PKG-INFO` & `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhanko-certvalidator
-Version: 0.21.2
+Version: 0.22.0
 Summary: Validates X.509 certificates and paths; forked from wbond/certvalidator
 Author-email: Matthias Valvekens <dev@mvalvekens.be>
 License: MIT
 Project-URL: Homepage, https://github.com/MatthiasValvekens/certvalidator
 Keywords: crypto,pki,x509,certificate,crl,ocsp
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Security :: Cryptography
 Description-Content-Type: text/markdown
-Provides-Extra: async_http
+Provides-Extra: async-http
 Provides-Extra: testing
 Provides-Extra: mypy
 License-File: LICENSE
 
 # certvalidator
 
 This library started as a fork of [wbond/certvalidator](https://github.com/wbond/certvalidator) with patches for [pyHanko](https://github.com/MatthiasValvekens/pyHanko), but has since diverged considerably from its parent repository.
```

### Comparing `pyhanko-certvalidator-0.21.2/pyhanko_certvalidator.egg-info/SOURCES.txt` & `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.2/pyproject.toml` & `pyhanko-certvalidator-0.22.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -44,23 +44,26 @@
 file = "README.md"
 content-type = "text/markdown"
 
 [project.urls]
 Homepage = "https://github.com/MatthiasValvekens/certvalidator"
 
 [project.optional-dependencies]
-async_http = ["aiohttp~=3.8.0"]
+async-http = ["aiohttp~=3.8.0"]
 testing = [
     "pytest>=6.1.1",
+    "pytest-cov~=4.0.0",
     "freezegun>=1.1.0",
     "aiohttp~=3.8.0",
     "pytest-aiohttp~=1.0.4",
+    "pyhanko-certvalidator[async-http]",
 ]
 mypy = [
     "types-requests",
+    "pyhanko-certvalidator[testing]",
 ]
 
 [tool.setuptools]
 include-package-data = false
 
 [tool.setuptools.dynamic]
 version = {attr = "pyhanko_certvalidator.version.__version__"}
```

### Comparing `pyhanko-certvalidator-0.21.2/tests/test_ac_validate.py` & `pyhanko-certvalidator-0.22.0/tests/test_ac_validate.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.2/tests/test_ades_time_slide.py` & `pyhanko-certvalidator-0.22.0/tests/test_ades_time_slide.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.2/tests/test_certificate_validator.py` & `pyhanko-certvalidator-0.22.0/tests/test_certificate_validator.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.2/tests/test_crl_client.py` & `pyhanko-certvalidator-0.22.0/tests/test_crl_client.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.2/tests/test_freshness.py` & `pyhanko-certvalidator-0.22.0/tests/test_freshness.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.2/tests/test_ocsp_client.py` & `pyhanko-certvalidator-0.22.0/tests/test_ocsp_client.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.2/tests/test_policy_proc.py` & `pyhanko-certvalidator-0.22.0/tests/test_policy_proc.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.2/tests/test_registry.py` & `pyhanko-certvalidator-0.22.0/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.21.2/tests/test_validate.py` & `pyhanko-certvalidator-0.22.0/tests/test_validate.py`

 * *Files identical despite different names*

