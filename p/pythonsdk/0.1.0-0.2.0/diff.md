# Comparing `tmp/pythonsdk-0.1.0.tar.gz` & `tmp/pythonsdk-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonsdk-0.1.0.tar", last modified: Sun Apr 23 11:19:21 2023, max compression
+gzip compressed data, was "pythonsdk-0.2.0.tar", last modified: Sun Apr 23 12:38:42 2023, max compression
```

## Comparing `pythonsdk-0.1.0.tar` & `pythonsdk-0.2.0.tar`

### file list

```diff
@@ -1,71 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:19:21.671910 pythonsdk-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-23 11:18:50.000000 pythonsdk-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-23 11:19:21.671910 pythonsdk-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-23 11:18:50.000000 pythonsdk-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-23 11:18:50.000000 pythonsdk-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 11:19:21.671910 pythonsdk-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:19:21.663910 pythonsdk-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:19:21.663910 pythonsdk-0.1.0/src/python_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-23 11:18:50.000000 pythonsdk-0.1.0/src/python_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-23 11:18:50.000000 pythonsdk-0.1.0/src/python_sdk/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:19:21.663910 pythonsdk-0.1.0/src/python_sdk/bin/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-23 11:18:50.000000 pythonsdk-0.1.0/src/python_sdk/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-04-23 11:18:50.000000 pythonsdk-0.1.0/src/python_sdk/bin/_call.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:19:21.663910 pythonsdk-0.1.0/src/python_sdk/config/
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-23 11:18:50.000000 pythonsdk-0.1.0/src/python_sdk/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11782 2023-04-23 11:18:50.000000 pythonsdk-0.1.0/src/python_sdk/config/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 11:18:50.000000 pythonsdk-0.1.0/src/python_sdk/config/_config_documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-04-23 11:18:50.000000 pythonsdk-0.1.0/src/python_sdk/config/_config_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-04-23 11:18:50.000000 pythonsdk-0.1.0/src/python_sdk/config/_config_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-23 11:18:50.000000 pythonsdk-0.1.0/src/python_sdk/config/_config_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-23 11:18:50.000000 pythonsdk-0.1.0/src/python_sdk/config/_config_value_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-04-23 11:18:50.000000 pythonsdk-0.1.0/src/python_sdk/config/_config_value_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-23 11:18:50.000000 pythonsdk-0.1.0/src/python_sdk/config/_optional_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-04-23 11:18:50.000000 pythonsdk-0.1.0/src/python_sdk/config/_string_decoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:19:21.667910 pythonsdk-0.1.0/src/python_sdk/encoding/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-23 11:18:50.000000 pythonsdk-0.1.0/src/python_sdk/encoding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-23 11:18:50.000000 pythonsdk-0.1.0/src/python_sdk/encoding/_base64url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:19:21.667910 pythonsdk-0.1.0/src/python_sdk/log/
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-23 11:18:50.000000 pythonsdk-0.1.0/src/python_sdk/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-23 11:18:50.000000 pythonsdk-0.1.0/src/python_sdk/log/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-04-23 11:18:50.000000 pythonsdk-0.1.0/src/python_sdk/log/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-23 11:18:50.000000 pythonsdk-0.1.0/src/python_sdk/log/_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-04-23 11:18:50.000000 pythonsdk-0.1.0/src/python_sdk/log/_formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-04-23 11:18:50.000000 pythonsdk-0.1.0/src/python_sdk/log/_log.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-23 11:18:50.000000 pythonsdk-0.1.0/src/python_sdk/log/_log_levels.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 11:18:50.000000 pythonsdk-0.1.0/src/python_sdk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:19:21.667910 pythonsdk-0.1.0/src/python_sdk/secrets/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-23 11:18:50.000000 pythonsdk-0.1.0/src/python_sdk/secrets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-04-23 11:18:50.000000 pythonsdk-0.1.0/src/python_sdk/secrets/_aws_ps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-04-23 11:18:50.000000 pythonsdk-0.1.0/src/python_sdk/secrets/_aws_sm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-04-23 11:18:50.000000 pythonsdk-0.1.0/src/python_sdk/secrets/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-23 11:18:50.000000 pythonsdk-0.1.0/src/python_sdk/secrets/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-23 11:18:50.000000 pythonsdk-0.1.0/src/python_sdk/secrets/_get_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-23 11:18:50.000000 pythonsdk-0.1.0/src/python_sdk/secrets/_secrets_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:19:21.667910 pythonsdk-0.1.0/src/python_sdk/sentinel/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-23 11:18:50.000000 pythonsdk-0.1.0/src/python_sdk/sentinel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-04-23 11:18:50.000000 pythonsdk-0.1.0/src/python_sdk/sentinel/_sentinel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:19:21.667910 pythonsdk-0.1.0/src/python_sdk/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-23 11:18:50.000000 pythonsdk-0.1.0/src/python_sdk/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-04-23 11:18:50.000000 pythonsdk-0.1.0/src/python_sdk/testing/_prepackaged_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:19:21.671910 pythonsdk-0.1.0/src/python_sdk/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-23 11:18:50.000000 pythonsdk-0.1.0/src/python_sdk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-23 11:18:50.000000 pythonsdk-0.1.0/src/python_sdk/utils/_ansi.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-23 11:18:50.000000 pythonsdk-0.1.0/src/python_sdk/utils/_checksum.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-23 11:18:50.000000 pythonsdk-0.1.0/src/python_sdk/utils/_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-23 11:18:50.000000 pythonsdk-0.1.0/src/python_sdk/utils/_file_watcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-23 11:18:50.000000 pythonsdk-0.1.0/src/python_sdk/utils/_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-23 11:18:50.000000 pythonsdk-0.1.0/src/python_sdk/utils/_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-23 11:18:50.000000 pythonsdk-0.1.0/src/python_sdk/utils/_which.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-23 11:18:50.000000 pythonsdk-0.1.0/src/python_sdk/utils/_zipfile.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-23 11:19:15.000000 pythonsdk-0.1.0/src/python_sdk/version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:19:21.671910 pythonsdk-0.1.0/src/python_sdk/versioning/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-23 11:18:50.000000 pythonsdk-0.1.0/src/python_sdk/versioning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-04-23 11:18:50.000000 pythonsdk-0.1.0/src/python_sdk/versioning/_version_file_based.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:19:21.671910 pythonsdk-0.1.0/src/pythonsdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-23 11:19:21.000000 pythonsdk-0.1.0/src/pythonsdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-23 11:19:21.000000 pythonsdk-0.1.0/src/pythonsdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 11:19:21.000000 pythonsdk-0.1.0/src/pythonsdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-23 11:19:21.000000 pythonsdk-0.1.0/src/pythonsdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-23 11:19:21.000000 pythonsdk-0.1.0/src/pythonsdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-23 11:18:50.000000 pythonsdk-0.1.0/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:38:42.336500 pythonsdk-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-23 12:38:15.000000 pythonsdk-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-04-23 12:38:42.336500 pythonsdk-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-23 12:38:15.000000 pythonsdk-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-23 12:38:15.000000 pythonsdk-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 12:38:42.336500 pythonsdk-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:38:42.328500 pythonsdk-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:38:42.328500 pythonsdk-0.2.0/src/python_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-23 12:38:15.000000 pythonsdk-0.2.0/src/python_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-23 12:38:15.000000 pythonsdk-0.2.0/src/python_sdk/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:38:42.328500 pythonsdk-0.2.0/src/python_sdk/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-23 12:38:15.000000 pythonsdk-0.2.0/src/python_sdk/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-04-23 12:38:15.000000 pythonsdk-0.2.0/src/python_sdk/bin/_call.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:38:42.332500 pythonsdk-0.2.0/src/python_sdk/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-23 12:38:15.000000 pythonsdk-0.2.0/src/python_sdk/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11782 2023-04-23 12:38:15.000000 pythonsdk-0.2.0/src/python_sdk/config/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:38:15.000000 pythonsdk-0.2.0/src/python_sdk/config/_config_documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-04-23 12:38:15.000000 pythonsdk-0.2.0/src/python_sdk/config/_config_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-04-23 12:38:15.000000 pythonsdk-0.2.0/src/python_sdk/config/_config_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-23 12:38:15.000000 pythonsdk-0.2.0/src/python_sdk/config/_config_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-23 12:38:15.000000 pythonsdk-0.2.0/src/python_sdk/config/_config_value_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-04-23 12:38:15.000000 pythonsdk-0.2.0/src/python_sdk/config/_config_value_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-23 12:38:15.000000 pythonsdk-0.2.0/src/python_sdk/config/_optional_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-04-23 12:38:15.000000 pythonsdk-0.2.0/src/python_sdk/config/_string_decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:38:42.332500 pythonsdk-0.2.0/src/python_sdk/encoding/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-23 12:38:15.000000 pythonsdk-0.2.0/src/python_sdk/encoding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-23 12:38:15.000000 pythonsdk-0.2.0/src/python_sdk/encoding/_base64url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:38:42.332500 pythonsdk-0.2.0/src/python_sdk/log/
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-23 12:38:15.000000 pythonsdk-0.2.0/src/python_sdk/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-23 12:38:15.000000 pythonsdk-0.2.0/src/python_sdk/log/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-04-23 12:38:15.000000 pythonsdk-0.2.0/src/python_sdk/log/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-23 12:38:15.000000 pythonsdk-0.2.0/src/python_sdk/log/_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-04-23 12:38:15.000000 pythonsdk-0.2.0/src/python_sdk/log/_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-04-23 12:38:15.000000 pythonsdk-0.2.0/src/python_sdk/log/_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-23 12:38:15.000000 pythonsdk-0.2.0/src/python_sdk/log/_log_levels.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:38:15.000000 pythonsdk-0.2.0/src/python_sdk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:38:42.332500 pythonsdk-0.2.0/src/python_sdk/secrets/
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-23 12:38:15.000000 pythonsdk-0.2.0/src/python_sdk/secrets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-23 12:38:15.000000 pythonsdk-0.2.0/src/python_sdk/secrets/_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:38:42.332500 pythonsdk-0.2.0/src/python_sdk/secrets/_secrets_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-23 12:38:15.000000 pythonsdk-0.2.0/src/python_sdk/secrets/_secrets_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-23 12:38:15.000000 pythonsdk-0.2.0/src/python_sdk/secrets/_secrets_engine/_aws_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-04-23 12:38:15.000000 pythonsdk-0.2.0/src/python_sdk/secrets/_secrets_engine/_aws_secrets_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-23 12:38:15.000000 pythonsdk-0.2.0/src/python_sdk/secrets/_secrets_engine/_aws_systems_manager_parameter_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-23 12:38:15.000000 pythonsdk-0.2.0/src/python_sdk/secrets/_secrets_engine/_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-23 12:38:15.000000 pythonsdk-0.2.0/src/python_sdk/secrets/_secrets_engine/_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:38:42.332500 pythonsdk-0.2.0/src/python_sdk/sentinel/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-23 12:38:15.000000 pythonsdk-0.2.0/src/python_sdk/sentinel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-04-23 12:38:15.000000 pythonsdk-0.2.0/src/python_sdk/sentinel/_sentinel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:38:42.332500 pythonsdk-0.2.0/src/python_sdk/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-23 12:38:15.000000 pythonsdk-0.2.0/src/python_sdk/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-04-23 12:38:15.000000 pythonsdk-0.2.0/src/python_sdk/testing/_prepackaged_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:38:42.336500 pythonsdk-0.2.0/src/python_sdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-23 12:38:15.000000 pythonsdk-0.2.0/src/python_sdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-23 12:38:15.000000 pythonsdk-0.2.0/src/python_sdk/utils/_ansi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-23 12:38:15.000000 pythonsdk-0.2.0/src/python_sdk/utils/_checksum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-23 12:38:15.000000 pythonsdk-0.2.0/src/python_sdk/utils/_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-23 12:38:15.000000 pythonsdk-0.2.0/src/python_sdk/utils/_file_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-23 12:38:15.000000 pythonsdk-0.2.0/src/python_sdk/utils/_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-23 12:38:15.000000 pythonsdk-0.2.0/src/python_sdk/utils/_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-23 12:38:15.000000 pythonsdk-0.2.0/src/python_sdk/utils/_which.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-23 12:38:15.000000 pythonsdk-0.2.0/src/python_sdk/utils/_zipfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-23 12:38:36.000000 pythonsdk-0.2.0/src/python_sdk/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:38:42.336500 pythonsdk-0.2.0/src/python_sdk/versioning/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-23 12:38:15.000000 pythonsdk-0.2.0/src/python_sdk/versioning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-04-23 12:38:15.000000 pythonsdk-0.2.0/src/python_sdk/versioning/_version_file_based.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:38:42.336500 pythonsdk-0.2.0/src/pythonsdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-04-23 12:38:42.000000 pythonsdk-0.2.0/src/pythonsdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-23 12:38:42.000000 pythonsdk-0.2.0/src/pythonsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 12:38:42.000000 pythonsdk-0.2.0/src/pythonsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-23 12:38:42.000000 pythonsdk-0.2.0/src/pythonsdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-23 12:38:42.000000 pythonsdk-0.2.0/src/pythonsdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-23 12:38:15.000000 pythonsdk-0.2.0/version
```

### Comparing `pythonsdk-0.1.0/LICENSE` & `pythonsdk-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.1.0/PKG-INFO` & `pythonsdk-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythonsdk
-Version: 0.1.0
+Version: 0.2.0
 Summary: Python Software Dev Kit
 Author-email: lijok <lijok@pm.me>
 License: MIT License
         
         Copyright (c) 2022 Lijok
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -46,8 +46,17 @@
 Provides-Extra: dev
 Provides-Extra: aws
 Provides-Extra: testing
 License-File: LICENSE
 
 # python-sdk
 
-THIS IS WIP
+## Requirements
+Python 3.10+
+
+## Installation
+```console
+pip install pythonsdk
+
+# If using AWS functionality
+pip install pythonsdk[aws]
+```
```

### Comparing `pythonsdk-0.1.0/pyproject.toml` & `pythonsdk-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.1.0/src/python_sdk/bin/_call.py` & `pythonsdk-0.2.0/src/python_sdk/bin/_call.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.1.0/src/python_sdk/config/__init__.py` & `pythonsdk-0.2.0/src/python_sdk/config/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.1.0/src/python_sdk/config/_config.py` & `pythonsdk-0.2.0/src/python_sdk/config/_config.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.1.0/src/python_sdk/config/_config_option.py` & `pythonsdk-0.2.0/src/python_sdk/config/_config_option.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.1.0/src/python_sdk/config/_config_sources.py` & `pythonsdk-0.2.0/src/python_sdk/config/_config_sources.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.1.0/src/python_sdk/config/_config_value_types.py` & `pythonsdk-0.2.0/src/python_sdk/config/_config_value_types.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.1.0/src/python_sdk/config/_config_value_validators.py` & `pythonsdk-0.2.0/src/python_sdk/config/_config_value_validators.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.1.0/src/python_sdk/config/_string_decoder.py` & `pythonsdk-0.2.0/src/python_sdk/config/_string_decoder.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.1.0/src/python_sdk/encoding/_base64url.py` & `pythonsdk-0.2.0/src/python_sdk/encoding/_base64url.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.1.0/src/python_sdk/log/__init__.py` & `pythonsdk-0.2.0/src/python_sdk/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.1.0/src/python_sdk/log/_base.py` & `pythonsdk-0.2.0/src/python_sdk/log/_base.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.1.0/src/python_sdk/log/_config.py` & `pythonsdk-0.2.0/src/python_sdk/log/_config.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.1.0/src/python_sdk/log/_context.py` & `pythonsdk-0.2.0/src/python_sdk/log/_context.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.1.0/src/python_sdk/log/_formatters.py` & `pythonsdk-0.2.0/src/python_sdk/log/_formatters.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.1.0/src/python_sdk/log/_log.py` & `pythonsdk-0.2.0/src/python_sdk/log/_log.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.1.0/src/python_sdk/secrets/_aws_sm.py` & `pythonsdk-0.2.0/src/python_sdk/secrets/_secrets_engine/_aws_systems_manager_parameter_store.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,69 +1,60 @@
-import json
+import io
 import logging
 import typing
 
-import boto3  # type: ignore
-import botocore.exceptions  # type: ignore
+from python_sdk.secrets._config import AWSSecretsEngineConfig
+from python_sdk.secrets._secrets_engine import _protocol
 
-from python_sdk.secrets import _exceptions
-from python_sdk.secrets import _secrets_engine
 
+class AWSSystemsManagerParameterStore:
+    TYPE: str = "AWS_SYSTEMS_MANAGER_PARAMETER_STORE"
 
-# Boto3 does not have types, so we have to make our own.
-class AWSSecretsManagerClient(typing.Protocol):
-    def get_secret_value(self, **kwargs: typing.Any) -> dict[str, typing.Any]:
-        ...
-
-
-class AWSSecretsManager(_secrets_engine.SecretsEngine):
-    client: AWSSecretsManagerClient
-
-    def __init__(
-        self,
-        secret_key_id: str | None = None,
-        secret_access_key: str | None = None,
-        session_token: str | None = None,
-        region_name: str | None = None,
-        api_version: str | None = None,
-        use_ssl: bool = True,
-        verify: bool = True,
-        endpoint_url: str | None = None,
-        botocore_config: dict[str, str] | None = None,
-    ) -> None:
-        self.client = boto3.client(
-            service_name="secretsmanager",
-            aws_access_key_id=secret_key_id,
-            aws_secret_access_key=secret_access_key,
-            aws_session_token=session_token,
-            region_name=region_name,
-            api_version=api_version,
-            use_ssl=use_ssl,
-            verify=verify,
-            endpoint_url=endpoint_url,
-            config=botocore_config,
+    def __init__(self) -> None:
+        import boto3  # type: ignore
+        import botocore.client  # type: ignore
+
+        self.client: botocore.client.BaseClient = boto3.Session().client(
+            service_name="ssm",
+            aws_access_key_id=AWSSecretsEngineConfig.ACCESS_KEY_ID,
+            aws_secret_access_key=AWSSecretsEngineConfig.SECRET_ACCESS_KEY,
+            aws_session_token=AWSSecretsEngineConfig.SESSION_TOKEN,
+            region_name=AWSSecretsEngineConfig.REGION_NAME,
+            api_version=AWSSecretsEngineConfig.API_VERSION,
+            use_ssl=AWSSecretsEngineConfig.USE_SSL,
+            verify=AWSSecretsEngineConfig.VERIFY,
+            endpoint_url=AWSSecretsEngineConfig.ENDPOINT_URL,
+            config=AWSSecretsEngineConfig.BOTOCORE_CONFIG,
         )
 
-    def get_secret(self, secret_name: str) -> _secrets_engine.SecretValue:
-        logging.debug(f"Getting secret. {secret_name=}")
+    def _processed_key(self, key: str) -> str:
+        return "/" + key.removeprefix("/")  # ensure prefixed with /
+
+    def autocomplete_key(self, key: str) -> list[str]:
+        return [
+            parameter["Name"]
+            for parameter in self.client.get_paginator("describe_parameters")
+            .paginate()
+            .build_full_result()["Parameters"]
+            if parameter["Name"].startswith(self._processed_key(key=key))
+        ]
+
+    def get_secret_value(self, key: str) -> typing.IO[bytes]:
+        import botocore.exceptions
+
+        logging.debug(f"Getting secret. {key=}")
         try:
-            response = self.client.get_secret_value(SecretId=secret_name)
+            response = self.client.get_parameter(Name=self._processed_key(key=key), WithDecryption=True)
         except botocore.exceptions.ClientError as e:
-            if e.response["Error"]["Code"] == "ResourceNotFoundException":
-                raise _exceptions.SecretDoesNotExist(e.response["Error"]["Message"]) from e
+            if e.response["Error"]["Code"] == "ParameterNotFound":
+                raise _protocol.DoesNotExist(e.response["Error"]["Message"]) from e
             elif e.response["Error"]["Code"] == "NotAuthorizedException":
-                raise _exceptions.Unauthorized(e.response["Error"]["Message"]) from e
+                raise _protocol.Unauthorized(e.response["Error"]["Message"]) from e
             raise
 
-        unprocessed_secret: str
-        if "SecretBinary" in response:
-            unprocessed_secret = response["SecretBinary"].decode("utf-8")
-        else:
-            unprocessed_secret = response["SecretString"]
-
-        secret: _secrets_engine.SecretValue
-        try:
-            secret = json.loads(unprocessed_secret)
-        except json.JSONDecodeError:
-            secret = unprocessed_secret
+        value: typing.IO[bytes] = io.BytesIO()
+        value.write(response["Parameter"]["Value"].encode("utf-8"))
+        value.seek(0)
+        return value
 
-        return secret
+    def set_secret_value(self, key: str, value: typing.IO[bytes]) -> None:
+        self.client.put_parameter(Name=self._processed_key(key=key), Value=value.read().decode("utf-8"), Overwrite=True)
```

### Comparing `pythonsdk-0.1.0/src/python_sdk/sentinel/_sentinel.py` & `pythonsdk-0.2.0/src/python_sdk/sentinel/_sentinel.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.1.0/src/python_sdk/testing/_prepackaged_tests.py` & `pythonsdk-0.2.0/src/python_sdk/testing/_prepackaged_tests.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.1.0/src/python_sdk/utils/__init__.py` & `pythonsdk-0.2.0/src/python_sdk/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.1.0/src/python_sdk/utils/_file_watcher.py` & `pythonsdk-0.2.0/src/python_sdk/utils/_file_watcher.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.1.0/src/python_sdk/utils/_zipfile.py` & `pythonsdk-0.2.0/src/python_sdk/utils/_zipfile.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.1.0/src/python_sdk/versioning/_version_file_based.py` & `pythonsdk-0.2.0/src/python_sdk/versioning/_version_file_based.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.1.0/src/pythonsdk.egg-info/PKG-INFO` & `pythonsdk-0.2.0/src/pythonsdk.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythonsdk
-Version: 0.1.0
+Version: 0.2.0
 Summary: Python Software Dev Kit
 Author-email: lijok <lijok@pm.me>
 License: MIT License
         
         Copyright (c) 2022 Lijok
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -46,8 +46,17 @@
 Provides-Extra: dev
 Provides-Extra: aws
 Provides-Extra: testing
 License-File: LICENSE
 
 # python-sdk
 
-THIS IS WIP
+## Requirements
+Python 3.10+
+
+## Installation
+```console
+pip install pythonsdk
+
+# If using AWS functionality
+pip install pythonsdk[aws]
+```
```

### Comparing `pythonsdk-0.1.0/src/pythonsdk.egg-info/SOURCES.txt` & `pythonsdk-0.2.0/src/pythonsdk.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -24,20 +24,21 @@
 src/python_sdk/log/_base.py
 src/python_sdk/log/_config.py
 src/python_sdk/log/_context.py
 src/python_sdk/log/_formatters.py
 src/python_sdk/log/_log.py
 src/python_sdk/log/_log_levels.py
 src/python_sdk/secrets/__init__.py
-src/python_sdk/secrets/_aws_ps.py
-src/python_sdk/secrets/_aws_sm.py
 src/python_sdk/secrets/_config.py
-src/python_sdk/secrets/_exceptions.py
-src/python_sdk/secrets/_get_secret.py
-src/python_sdk/secrets/_secrets_engine.py
+src/python_sdk/secrets/_secrets_engine/__init__.py
+src/python_sdk/secrets/_secrets_engine/_aws_s3.py
+src/python_sdk/secrets/_secrets_engine/_aws_secrets_manager.py
+src/python_sdk/secrets/_secrets_engine/_aws_systems_manager_parameter_store.py
+src/python_sdk/secrets/_secrets_engine/_factory.py
+src/python_sdk/secrets/_secrets_engine/_protocol.py
 src/python_sdk/sentinel/__init__.py
 src/python_sdk/sentinel/_sentinel.py
 src/python_sdk/testing/__init__.py
 src/python_sdk/testing/_prepackaged_tests.py
 src/python_sdk/utils/__init__.py
 src/python_sdk/utils/_ansi.py
 src/python_sdk/utils/_checksum.py
```

