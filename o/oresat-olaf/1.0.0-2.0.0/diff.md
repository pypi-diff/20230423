# Comparing `tmp/oresat-olaf-1.0.0.tar.gz` & `tmp/oresat-olaf-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oresat-olaf-1.0.0.tar", last modified: Sun Jan 29 20:01:38 2023, max compression
+gzip compressed data, was "oresat-olaf-2.0.0.tar", last modified: Sun Apr 23 21:15:41 2023, max compression
```

## Comparing `oresat-olaf-1.0.0.tar` & `oresat-olaf-2.0.0.tar`

### file list

```diff
@@ -1,79 +1,87 @@
-drwxr-xr-x   0 ryan      (1000) ryan      (1000)        0 2023-01-29 20:01:38.836729 oresat-olaf-1.0.0/
--rw-r--r--   0 ryan      (1000) ryan      (1000)    35149 2022-01-04 23:33:32.000000 oresat-olaf-1.0.0/LICENSE
--rw-r--r--   0 ryan      (1000) ryan      (1000)     2652 2023-01-29 20:01:38.836729 oresat-olaf-1.0.0/PKG-INFO
--rw-r--r--   0 ryan      (1000) ryan      (1000)     1649 2023-01-26 02:19:19.000000 oresat-olaf-1.0.0/README.rst
-drwxr-xr-x   0 ryan      (1000) ryan      (1000)        0 2023-01-29 20:01:38.830063 oresat-olaf-1.0.0/olaf/
--rw-r--r--   0 ryan      (1000) ryan      (1000)     1989 2023-01-26 02:19:19.000000 oresat-olaf-1.0.0/olaf/__init__.py
-drwxr-xr-x   0 ryan      (1000) ryan      (1000)        0 2023-01-29 20:01:38.830063 oresat-olaf-1.0.0/olaf/_internals/
--rw-r--r--   0 ryan      (1000) ryan      (1000)        0 2023-01-26 02:19:19.000000 oresat-olaf-1.0.0/olaf/_internals/__init__.py
--rw-r--r--   0 ryan      (1000) ryan      (1000)    12785 2023-01-26 02:19:19.000000 oresat-olaf-1.0.0/olaf/_internals/app.py
-drwxr-xr-x   0 ryan      (1000) ryan      (1000)        0 2023-01-29 20:01:38.830063 oresat-olaf-1.0.0/olaf/_internals/data/
--rw-r--r--   0 ryan      (1000) ryan      (1000)    81544 2023-01-26 02:19:19.000000 oresat-olaf-1.0.0/olaf/_internals/data/oresat_app.eds
-drwxr-xr-x   0 ryan      (1000) ryan      (1000)        0 2023-01-29 20:01:38.830063 oresat-olaf-1.0.0/olaf/_internals/resources/
--rw-r--r--   0 ryan      (1000) ryan      (1000)        0 2023-01-26 02:19:19.000000 oresat-olaf-1.0.0/olaf/_internals/resources/__init__.py
--rw-r--r--   0 ryan      (1000) ryan      (1000)     1475 2023-01-26 02:19:19.000000 oresat-olaf-1.0.0/olaf/_internals/resources/ecss.py
--rw-r--r--   0 ryan      (1000) ryan      (1000)     3112 2023-01-26 02:19:19.000000 oresat-olaf-1.0.0/olaf/_internals/resources/file_caches.py
--rw-r--r--   0 ryan      (1000) ryan      (1000)     2685 2023-01-26 02:19:19.000000 oresat-olaf-1.0.0/olaf/_internals/resources/fread.py
--rw-r--r--   0 ryan      (1000) ryan      (1000)     2095 2023-01-26 02:19:19.000000 oresat-olaf-1.0.0/olaf/_internals/resources/fwrite.py
--rw-r--r--   0 ryan      (1000) ryan      (1000)     1226 2023-01-26 02:19:19.000000 oresat-olaf-1.0.0/olaf/_internals/resources/logs.py
--rw-r--r--   0 ryan      (1000) ryan      (1000)     2934 2023-01-26 02:19:19.000000 oresat-olaf-1.0.0/olaf/_internals/resources/os_command.py
--rw-r--r--   0 ryan      (1000) ryan      (1000)     5111 2023-01-26 02:19:19.000000 oresat-olaf-1.0.0/olaf/_internals/resources/system_info.py
--rw-r--r--   0 ryan      (1000) ryan      (1000)     2201 2023-01-26 02:19:19.000000 oresat-olaf-1.0.0/olaf/_internals/resources/updater.py
-drwxr-xr-x   0 ryan      (1000) ryan      (1000)        0 2023-01-29 20:01:38.830063 oresat-olaf-1.0.0/olaf/_internals/rest_api/
--rw-r--r--   0 ryan      (1000) ryan      (1000)     2169 2023-01-26 02:19:19.000000 oresat-olaf-1.0.0/olaf/_internals/rest_api/__init__.py
--rw-r--r--   0 ryan      (1000) ryan      (1000)     5416 2023-01-26 02:19:19.000000 oresat-olaf-1.0.0/olaf/_internals/rest_api/blueprints.py
-drwxr-xr-x   0 ryan      (1000) ryan      (1000)        0 2023-01-29 20:01:38.830063 oresat-olaf-1.0.0/olaf/_internals/rest_api/static/
--rw-r--r--   0 ryan      (1000) ryan      (1000)    15406 2023-01-26 02:19:19.000000 oresat-olaf-1.0.0/olaf/_internals/rest_api/static/favicon.ico
-drwxr-xr-x   0 ryan      (1000) ryan      (1000)        0 2023-01-29 20:01:38.830063 oresat-olaf-1.0.0/olaf/_internals/rest_api/templates/
--rw-r--r--   0 ryan      (1000) ryan      (1000)     2645 2023-01-26 02:19:19.000000 oresat-olaf-1.0.0/olaf/_internals/rest_api/templates/base.html
--rw-r--r--   0 ryan      (1000) ryan      (1000)     2971 2023-01-26 02:19:19.000000 oresat-olaf-1.0.0/olaf/_internals/rest_api/templates/fread.html
--rw-r--r--   0 ryan      (1000) ryan      (1000)     1356 2023-01-26 02:19:19.000000 oresat-olaf-1.0.0/olaf/_internals/rest_api/templates/fwrite.html
--rw-r--r--   0 ryan      (1000) ryan      (1000)     4067 2023-01-26 02:19:19.000000 oresat-olaf-1.0.0/olaf/_internals/rest_api/templates/od.html
--rw-r--r--   0 ryan      (1000) ryan      (1000)     2034 2023-01-26 02:19:19.000000 oresat-olaf-1.0.0/olaf/_internals/rest_api/templates/os_command.html
--rw-r--r--   0 ryan      (1000) ryan      (1000)      338 2023-01-26 02:19:19.000000 oresat-olaf-1.0.0/olaf/_internals/rest_api/templates/root.html
--rw-r--r--   0 ryan      (1000) ryan      (1000)     3754 2023-01-26 02:19:19.000000 oresat-olaf-1.0.0/olaf/_internals/rest_api/templates/system_info.html
--rw-r--r--   0 ryan      (1000) ryan      (1000)     2357 2023-01-26 02:19:19.000000 oresat-olaf-1.0.0/olaf/_internals/rest_api/templates/updater.html
--rw-r--r--   0 ryan      (1000) ryan      (1000)    15246 2023-01-26 02:19:19.000000 oresat-olaf-1.0.0/olaf/_internals/updater.py
-drwxr-xr-x   0 ryan      (1000) ryan      (1000)        0 2023-01-29 20:01:38.833396 oresat-olaf-1.0.0/olaf/common/
--rw-r--r--   0 ryan      (1000) ryan      (1000)        0 2022-05-30 01:12:02.000000 oresat-olaf-1.0.0/olaf/common/__init__.py
--rw-r--r--   0 ryan      (1000) ryan      (1000)     2449 2023-01-26 02:19:19.000000 oresat-olaf-1.0.0/olaf/common/ecss.py
--rw-r--r--   0 ryan      (1000) ryan      (1000)     3081 2022-05-30 01:12:02.000000 oresat-olaf-1.0.0/olaf/common/oresat_file.py
--rw-r--r--   0 ryan      (1000) ryan      (1000)     6256 2023-01-26 02:19:19.000000 oresat-olaf-1.0.0/olaf/common/oresat_file_cache.py
--rw-r--r--   0 ryan      (1000) ryan      (1000)     5281 2023-01-26 02:19:19.000000 oresat-olaf-1.0.0/olaf/common/resource.py
--rw-r--r--   0 ryan      (1000) ryan      (1000)     3169 2023-01-26 02:19:19.000000 oresat-olaf-1.0.0/olaf/common/timer_loop.py
-drwxr-xr-x   0 ryan      (1000) ryan      (1000)        0 2023-01-29 20:01:38.833396 oresat-olaf-1.0.0/olaf/scripts/
--rw-r--r--   0 ryan      (1000) ryan      (1000)        0 2022-09-18 00:48:00.000000 oresat-olaf-1.0.0/olaf/scripts/__init__.py
--rwxr-xr-x   0 ryan      (1000) ryan      (1000)     2482 2023-01-26 02:19:19.000000 oresat-olaf-1.0.0/olaf/scripts/file_transfer.py
--rwxr-xr-x   0 ryan      (1000) ryan      (1000)     1832 2023-01-26 02:19:19.000000 oresat-olaf-1.0.0/olaf/scripts/new_eds.py
--rwxr-xr-x   0 ryan      (1000) ryan      (1000)     1212 2023-01-26 02:19:19.000000 oresat-olaf-1.0.0/olaf/scripts/os_command.py
--rwxr-xr-x   0 ryan      (1000) ryan      (1000)     4938 2022-06-01 03:03:30.000000 oresat-olaf-1.0.0/olaf/scripts/sdo_transfer.py
--rwxr-xr-x   0 ryan      (1000) ryan      (1000)     3541 2023-01-26 02:19:19.000000 oresat-olaf-1.0.0/olaf/scripts/system_info.py
-drwxr-xr-x   0 ryan      (1000) ryan      (1000)        0 2023-01-29 20:01:38.833396 oresat-olaf-1.0.0/oresat_olaf.egg-info/
--rw-r--r--   0 ryan      (1000) ryan      (1000)     2652 2023-01-29 20:01:38.000000 oresat-olaf-1.0.0/oresat_olaf.egg-info/PKG-INFO
--rw-r--r--   0 ryan      (1000) ryan      (1000)     2076 2023-01-29 20:01:38.000000 oresat-olaf-1.0.0/oresat_olaf.egg-info/SOURCES.txt
--rw-r--r--   0 ryan      (1000) ryan      (1000)        1 2023-01-29 20:01:38.000000 oresat-olaf-1.0.0/oresat_olaf.egg-info/dependency_links.txt
--rw-r--r--   0 ryan      (1000) ryan      (1000)      259 2023-01-29 20:01:38.000000 oresat-olaf-1.0.0/oresat_olaf.egg-info/entry_points.txt
--rw-r--r--   0 ryan      (1000) ryan      (1000)       36 2023-01-29 20:01:38.000000 oresat-olaf-1.0.0/oresat_olaf.egg-info/requires.txt
--rw-r--r--   0 ryan      (1000) ryan      (1000)       11 2023-01-29 20:01:38.000000 oresat-olaf-1.0.0/oresat_olaf.egg-info/top_level.txt
--rw-r--r--   0 ryan      (1000) ryan      (1000)       41 2023-01-29 20:01:09.000000 oresat-olaf-1.0.0/pyproject.toml
--rw-r--r--   0 ryan      (1000) ryan      (1000)     1474 2023-01-29 20:01:38.836729 oresat-olaf-1.0.0/setup.cfg
-drwxr-xr-x   0 ryan      (1000) ryan      (1000)        0 2023-01-29 20:01:38.833396 oresat-olaf-1.0.0/tests/
--rw-r--r--   0 ryan      (1000) ryan      (1000)        0 2022-05-30 00:49:37.000000 oresat-olaf-1.0.0/tests/__init__.py
-drwxr-xr-x   0 ryan      (1000) ryan      (1000)        0 2023-01-29 20:01:38.833396 oresat-olaf-1.0.0/tests/common/
--rw-r--r--   0 ryan      (1000) ryan      (1000)        0 2022-05-30 00:49:05.000000 oresat-olaf-1.0.0/tests/common/__init__.py
--rw-r--r--   0 ryan      (1000) ryan      (1000)      526 2022-05-30 01:12:02.000000 oresat-olaf-1.0.0/tests/common/test_ecss.py
--rw-r--r--   0 ryan      (1000) ryan      (1000)     2066 2022-05-30 01:12:02.000000 oresat-olaf-1.0.0/tests/common/test_oresat_file.py
--rw-r--r--   0 ryan      (1000) ryan      (1000)    10193 2023-01-26 02:19:19.000000 oresat-olaf-1.0.0/tests/common/test_oresat_file_cache.py
-drwxr-xr-x   0 ryan      (1000) ryan      (1000)        0 2023-01-29 20:01:38.833396 oresat-olaf-1.0.0/tests/internals/
--rw-r--r--   0 ryan      (1000) ryan      (1000)        0 2023-01-26 02:19:19.000000 oresat-olaf-1.0.0/tests/internals/__init__.py
-drwxr-xr-x   0 ryan      (1000) ryan      (1000)        0 2023-01-29 20:01:38.836729 oresat-olaf-1.0.0/tests/internals/resources/
--rw-r--r--   0 ryan      (1000) ryan      (1000)     1257 2023-01-26 02:27:05.000000 oresat-olaf-1.0.0/tests/internals/resources/__init__.py
--rw-r--r--   0 ryan      (1000) ryan      (1000)      480 2023-01-26 02:19:19.000000 oresat-olaf-1.0.0/tests/internals/resources/test_ecss.py
--rw-r--r--   0 ryan      (1000) ryan      (1000)     7228 2023-01-26 02:23:17.000000 oresat-olaf-1.0.0/tests/internals/resources/test_file_caches.py
--rw-r--r--   0 ryan      (1000) ryan      (1000)     2038 2023-01-26 02:19:19.000000 oresat-olaf-1.0.0/tests/internals/resources/test_fread.py
--rw-r--r--   0 ryan      (1000) ryan      (1000)     2293 2023-01-26 02:19:19.000000 oresat-olaf-1.0.0/tests/internals/resources/test_fwrite.py
--rw-r--r--   0 ryan      (1000) ryan      (1000)     1359 2023-01-26 02:23:04.000000 oresat-olaf-1.0.0/tests/internals/resources/test_os_command.py
--rw-r--r--   0 ryan      (1000) ryan      (1000)     2698 2023-01-26 02:37:00.000000 oresat-olaf-1.0.0/tests/internals/resources/test_system_info.py
-drwxr-xr-x   0 ryan      (1000) ryan      (1000)        0 2023-01-29 20:01:38.836729 oresat-olaf-1.0.0/tests/internals/updater/
--rw-r--r--   0 ryan      (1000) ryan      (1000)        0 2023-01-26 02:19:19.000000 oresat-olaf-1.0.0/tests/internals/updater/__init__.py
--rw-r--r--   0 ryan      (1000) ryan      (1000)     6556 2023-01-26 02:19:19.000000 oresat-olaf-1.0.0/tests/internals/updater/test_updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:15:41.569478 oresat-olaf-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-23 21:15:41.569478 oresat-olaf-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:15:41.557478 oresat-olaf-2.0.0/olaf/
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:15:41.557478 oresat-olaf-2.0.0/olaf/_internals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7033 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:15:41.557478 oresat-olaf-2.0.0/olaf/_internals/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    82085 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/data/oresat_app.eds
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/master_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16649 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:15:41.557478 oresat-olaf-2.0.0/olaf/_internals/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/resources/ecss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/resources/file_caches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/resources/fread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/resources/fwrite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/resources/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/resources/os_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/resources/power_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/resources/store_eds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/resources/system_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/resources/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:15:41.561478 oresat-olaf-2.0.0/olaf/_internals/rest_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/rest_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:15:41.561478 oresat-olaf-2.0.0/olaf/_internals/rest_api/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/rest_api/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:15:41.561478 oresat-olaf-2.0.0/olaf/_internals/rest_api/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/rest_api/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/rest_api/templates/fread.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/rest_api/templates/fwrite.html
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/rest_api/templates/logs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/rest_api/templates/od.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/rest_api/templates/os_command.html
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/rest_api/templates/power_control.html
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/rest_api/templates/root.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/rest_api/templates/system_info.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/rest_api/templates/updater.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15344 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:15:41.561478 oresat-olaf-2.0.0/olaf/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/common/cpufreq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/common/ecss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/common/gpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/common/oresat_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/common/oresat_file_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/common/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/common/timer_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:15:41.565478 oresat-olaf-2.0.0/olaf/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2482 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/scripts/file_transfer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1832 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/scripts/new_eds.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1212 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/scripts/os_command.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5444 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/scripts/sdo_transfer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      456 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/scripts/sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3541 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/scripts/system_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:15:41.565478 oresat-olaf-2.0.0/oresat_olaf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-23 21:15:41.000000 oresat-olaf-2.0.0/oresat_olaf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-04-23 21:15:41.000000 oresat-olaf-2.0.0/oresat_olaf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 21:15:41.000000 oresat-olaf-2.0.0/oresat_olaf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-23 21:15:41.000000 oresat-olaf-2.0.0/oresat_olaf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-23 21:15:41.000000 oresat-olaf-2.0.0/oresat_olaf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-23 21:15:41.000000 oresat-olaf-2.0.0/oresat_olaf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-23 21:15:41.569478 oresat-olaf-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:15:41.565478 oresat-olaf-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:15:41.565478 oresat-olaf-2.0.0/tests/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/tests/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/tests/common/test_ecss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/tests/common/test_oresat_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10193 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/tests/common/test_oresat_file_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:15:41.565478 oresat-olaf-2.0.0/tests/internals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/tests/internals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:15:41.569478 oresat-olaf-2.0.0/tests/internals/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/tests/internals/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/tests/internals/resources/test_ecss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/tests/internals/resources/test_file_caches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/tests/internals/resources/test_fread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/tests/internals/resources/test_fwrite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/tests/internals/resources/test_os_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/tests/internals/resources/test_system_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:15:41.569478 oresat-olaf-2.0.0/tests/internals/updater/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/tests/internals/updater/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/tests/internals/updater/test_updater.py
```

### Comparing `oresat-olaf-1.0.0/LICENSE` & `oresat-olaf-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oresat-olaf-1.0.0/PKG-INFO` & `oresat-olaf-2.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oresat-olaf
-Version: 1.0.0
+Version: 2.0.0
 Summary: Application framework for all OreSat Linux boards
 Home-page: https://github.com/oresat/oresat-olaf
 Author: PSAS
 Author-email: oresat@pdx.edu
 Maintainer: PSAS
 Maintainer-email: oresat@pdx.edu
 License: GPL-3.0
```

### Comparing `oresat-olaf-1.0.0/README.rst` & `oresat-olaf-2.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `oresat-olaf-1.0.0/olaf/__init__.py` & `oresat-olaf-2.0.0/olaf/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,58 +1,86 @@
 import os
 import sys
 from logging.handlers import SysLogHandler
-from argparse import ArgumentParser
+from argparse import ArgumentParser, Namespace
 
 from loguru import logger
 
-from ._internals.app import app
-from ._internals.rest_api import rest_api
+from ._internals.app import app, App
+from ._internals.node import Node, NetworkError
+from ._internals.master_node import MasterNode
+from ._internals.rest_api import rest_api, RestAPI, render_olaf_template
 from .common.resource import Resource
 from .common.ecss import scet_int_from_time, scet_int_to_time, utc_int_from_time, utc_int_to_time
 from .common.oresat_file import OreSatFile, new_oresat_file
 from .common.oresat_file_cache import OreSatFileCache
 from .common.timer_loop import TimerLoop
+from .common.gpio import GPIO
 
-__version__ = '1.0.0'
+__version__ = '2.0.0'
 
 
-def olaf_run(eds_path: str = None):
-    '''Start the app and rest api.
+def olaf_setup(eds_path: str = None, master_node: bool = False) -> Namespace:
+    '''
+    Parse runtime args and setup the app and REST API.
 
     Parameters
     ----------
     eds_path: str
-        The path to the eds or dcf file
+        The path to the eds or dcf file.
+    master_node: bool
+        Run as master node.
+
+    Returns
+    -------
+    Namespace
+        The runtime args.
     '''
 
     parser = ArgumentParser(prog='OLAF')
     parser.add_argument('-b', '--bus', default='vcan0', help='CAN bus to use, defaults to vcan0')
     parser.add_argument('-n', '--node-id', type=str, default='0', metavar='ID',
                         help='set the node ID')
-    parser.add_argument('-v', '--verbose', action='store_true', help='verbose logging')
+    parser.add_argument('-v', '--verbose', action='store_true', help='enable verbose logging')
     parser.add_argument('-l', '--log', action='store_true', help='log to only journald')
-    parser.add_argument('-e', '--eds', metavar='FILE', help='EDS/DCF file to use')
-    parser.add_argument('-m', '--mock-hw', action='store_true', help='mock the hardware')
-    parser.add_argument('-a', '--address', default='localhost', help='rest api address')
-    parser.add_argument('-p', '--port', type=int, default=8000, help='rest api port number')
+    parser.add_argument('-e', '--eds', metavar='FILE', help='EDS / DCF file to use')
+    parser.add_argument('-m', '--mock-hw', nargs='*', metavar='HW', default=[],
+                        help='list the hardware to mock or just "all" to mock all hardware')
+    parser.add_argument('-a', '--address', default='localhost',
+                        help='rest api address, defaults to localhost')
+    parser.add_argument('-p', '--port', type=int, default=8000,
+                        help='rest api port number, defaults to 8000')
     args = parser.parse_args()
 
     if args.verbose:
         level = 'DEBUG'
+        backtrace = True
     else:
         level = 'INFO'
+        backtrace = False
 
     logger.remove()  # remove default logger
     if args.log:
-        logger.add(SysLogHandler(address='/dev/log'), level=level)
+        logger.add(SysLogHandler(address='/dev/log'), level=level, backtrace=backtrace)
     else:
-        logger.add(sys.stdout, level=level)
+        logger.add(sys.stdout, level=level, backtrace=backtrace)
+
+    olaf_boot_logs = '/tmp/olaf.log'
+    if os.path.isfile(olaf_boot_logs):
+        os.remove(olaf_boot_logs)
+    logger.add(olaf_boot_logs, level=level, backtrace=backtrace)
 
     if eds_path is None:
         eds_path = args.eds
 
-    app.setup(eds_path, args.bus, args.node_id, args.mock_hw)
+    app.setup(eds_path, args.bus, args.node_id, master_node=master_node)
+    rest_api.setup(address=args.address, port=args.port)
+
+    return args
+
+
+def olaf_run():
+    '''Start the app and REST API.'''
 
-    rest_api.start(address=args.address, port=args.port)
+    rest_api.start()
     app.run()
     rest_api.stop()
```

### Comparing `oresat-olaf-1.0.0/olaf/_internals/app.py` & `oresat-olaf-2.0.0/olaf/_internals/node.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,228 +1,181 @@
-import errno
 import struct
-import signal
 import subprocess
+from enum import IntEnum
 from os import geteuid
-from os.path import abspath, dirname
 from pathlib import Path
 from threading import Event
-from time import sleep
 
 import canopen
 import psutil
 from loguru import logger
 
-from ..common.resource import Resource
 from ..common.timer_loop import TimerLoop
 from ..common.oresat_file_cache import OreSatFileCache
-from .resources.os_command import OSCommandResource
-from .resources.system_info import SystemInfoResource
-from .resources.file_caches import FileCachesResource
-from .resources.fread import FreadResource
-from .resources.fwrite import FwriteResource
-from .resources.ecss import ECSSResource
-from .resources.updater import UpdaterResource
-from .resources.logs import LogsResource
 
 
-class App:
-    '''
-    The application class that manages the CAN bus and resources.
+class NodeStop(IntEnum):
 
-    Use the global ``olaf.app`` obect.
-    '''
+    SOFT_RESET = 1
+    '''Just stop the app and exit. Systemd will restart the app.'''
+    HARD_RESET = 2
+    '''Reboot system after app has stopped'''
+    FACTORY_RESET = 3
+    '''Clear all file cachces and reboot system after app has stopped'''
+    POWER_OFF = 4
+    '''Just power off the system.'''
 
-    _BACKUP_EDS = abspath(dirname(__file__)) + '/data/oresat_app.eds'
-    '''Internal eds file incase app's is misformatted or missing.'''
 
-    def __init__(self):
+class NetworkError(Exception):
+    '''Error with the CANopen network / bus'''
 
-        self._bus = None
-        self._event = Event()
-        self._res = []
-        self._network = None
-        self._mock_hw = False
-        self._name = 'OLAF'
-        self._node = None
-        self._node_id = 0
-
-        # setup event
-        for sig in ['SIGTERM', 'SIGHUP', 'SIGINT']:
-            signal.signal(getattr(signal, sig), self._quit)
-
-        if geteuid() == 0:  # running as root
-            self.work_base_dir = '/var/lib/oresat'
-            self.cache_base_dir = '/var/cache/oresat'
-        else:
-            self.work_base_dir = str(Path.home()) + '/.oresat'
-            self.cache_base_dir = str(Path.home()) + '/.cache/oresat'
-
-        fread_path = self.cache_base_dir + '/fread'
-        fwrite_path = self.cache_base_dir + '/fwrite'
-
-        self.fread_cache = OreSatFileCache(fread_path)
-        self.fwrite_cache = OreSatFileCache(fwrite_path)
-
-        # default resources
-        self.add_resource(OSCommandResource)
-        self.add_resource(ECSSResource)
-        self.add_resource(SystemInfoResource)
-        self.add_resource(FileCachesResource)
-        self.add_resource(FreadResource)
-        self.add_resource(FwriteResource)
-        self.add_resource(UpdaterResource)
-        self.add_resource(LogsResource)
-
-    def __del__(self):
-
-        self.stop()
-
-        if self._network:
-            try:
-                self._network.disconnect()
-            except Exception:
-                pass
-
-    def _load_node(self, node_id: int, eds: str):
 
-        dcf_node_id = canopen.import_od(eds).node_id
-        if node_id != 0:
-            self._node_id = node_id
-        elif dcf_node_id:
-            self._node_id = dcf_node_id
-        else:
-            self._node_id = 0x7C
-        self._node = canopen.LocalNode(self._node_id, eds)
-        self._node.object_dictionary.node_id = self._node_id
+class Node:
+    '''OreSat CANopen Node'''
 
-    def setup(self, eds: str, bus: str, node_id=0, mock_hw=False):
+    def __init__(self, node: canopen.LocalNode, bus: str):
         '''
-        Setup the app. Must be called after all `self.add_resource` calls.
-
         Parameters
         ----------
-        eds: str
-            File path to EDS or DCF file.
+        node: canopen.LocalNode
+            The canopen node obj this class wraps around.
         bus: str
             Which CAN bus to use.
-        node_id: int, str
-            The node ID. If set to 0 and DCF was used for the eds arg, the value will be pulled
-            from the DCF, otherwise, it will be set to 0x7C.
-        mock_hw: bool
-            Flag to mock hardware. This will be pass to any resources added.
-
-        Raises
-        ------
-        ValueError
-            Invalid parameter(s)
         '''
 
+        self._node = node
         self._bus = bus
-        self._mock_hw = mock_hw
-
-        logger.debug(f'fread cache path {self.fread_cache.dir}')
-        logger.debug(f'fwrite cache path {self.fwrite_cache.dir}')
+        self._network = None
+        self._event = Event()
+        self._read_cbs = {}
+        self._write_cbs = {}
+        self._syncs = 0
+        self._reset = NodeStop.SOFT_RESET
 
-        if self._mock_hw:
-            logger.warning('mock hardware flag enabled')
+        if geteuid() == 0:  # running as root
+            self.work_base_dir = '/var/lib/oresat'
+            self.cache_base_dir = '/var/cache/oresat'
+        else:
+            self.work_base_dir = str(Path.home()) + '/.oresat'
+            self.cache_base_dir = str(Path.home()) + '/.cache/oresat'
 
-        if not psutil.net_if_stats().get(self._bus):
-            logger.error(f'{self._bus} does not exist, waiting for bus to appear')
-            while not psutil.net_if_stats().get(self._bus):
-                try:
-                    sleep(1)
-                except KeyboardInterrupt:
-                    exit(0)
-            logger.info(f'{self._bus} now exists')
-
-        if isinstance(node_id, str):
-            if node_id.startswith('0x'):
-                node_id = int(node_id, 16)
-            else:
-                node_id = int(node_id)
-        elif not isinstance(node_id, int):
-            raise ValueError('node_id is not a int/hex str or a int')
+        fread_path = self.cache_base_dir + '/fread'
+        fwrite_path = self.cache_base_dir + '/fwrite'
 
-        if eds is not None:
-            try:
-                self._load_node(node_id, eds)
-            except Exception as e:
-                logger.error(f'{e.__class__.__name__}: {e}')
-                logger.warning(f'failed to read in {eds}, using OLAF\'s internal eds as backup')
-                self._load_node(node_id, self._BACKUP_EDS)
-        else:
-            logger.warning('No eds or dcf was supplied, using OLAF\'s internal eds')
-            self._load_node(node_id, self._BACKUP_EDS)
+        self._fread_cache = OreSatFileCache(fread_path)
+        self._fwrite_cache = OreSatFileCache(fwrite_path)
 
-        self._name = self._node.object_dictionary.device_information.product_name
+        logger.debug(f'fread cache path {self._fread_cache.dir}')
+        logger.debug(f'fwrite cache path {self._fwrite_cache.dir}')
 
         # python canopen does not set the value to default for some reason
         for i in self.od:
             if not isinstance(self.od[i], canopen.objectdictionary.Variable):
                 for j in self.od[i]:
-                    self.od[i][j].value = self.od[i][j].default
+                    if self.od[i][j].data_type == canopen.objectdictionary.BOOLEAN:
+                        # fix bools to be bools
+                        self.od[i][j].default = bool(self.od[i][j].default)
+                        self.od[i][j].value = bool(self.od[i][j].default)
+                    else:
+                        self.od[i][j].value = self.od[i][j].default
+            elif self.od[i].data_type == canopen.objectdictionary.BOOLEAN:
+                # fix bools to be bools
+                self.od[i].default = bool(self.od[i].default)
+                self.od[i].value = bool(self.od[i].default)
             else:
                 self.od[i].value = self.od[i].default
 
+        if self._node.object_dictionary.node_id is None:
+            self._node.object_dictionary.node_id = 0x7C
+
+        node_id = self._node.object_dictionary.node_id
+
         default_rpdos = [
-            0x200 + self._node_id,
-            0x300 + self._node_id,
-            0x400 + self._node_id,
-            0x500 + self._node_id
+            0x200 + node_id,
+            0x300 + node_id,
+            0x400 + node_id,
+            0x500 + node_id
         ]
         default_tpdos = [
-            0x180 + self._node_id,
-            0x280 + self._node_id,
-            0x380 + self._node_id,
-            0x480 + self._node_id
+            0x180 + node_id,
+            0x280 + node_id,
+            0x380 + node_id,
+            0x480 + node_id
         ]
 
         # fix COB-IDs for invaild PDOs
         #
         # all oresat node RPDO COB-ID follow values of 0x[2345]00 + $NODEID
         # all oresat node TPDO COB-ID follow values of 0x[1234]80 + $NODEID
         # this fixes the values for all 16 RPDOs/TPDOs
         for i in range(len(self._node.rpdo)):
             cob_id = self.od[0x1400 + i][1].default & 0xFFF
             if cob_id in default_rpdos:
-                cob_id = 0x200 + 0x100 * (i % 4) + self._node_id + i // 4
+                cob_id = 0x200 + 0x100 * (i % 4) + node_id + i // 4
             else:
                 cob_id = self.od[0x1400 + i][1].default
             self.od[0x1400 + i][1].value = cob_id
         for i in range(len(self._node.tpdo)):
             cob_id = self.od[0x1800 + i][1].default & 0xFFF
             if cob_id in default_tpdos:
-                cob_id = 0x180 + 0x100 * (i % 4) + self._node_id + i // 4
+                cob_id = 0x180 + 0x100 * (i % 4) + node_id + i // 4
             else:
                 cob_id = self.od[0x1800 + i][1].default
             self.od[0x1800 + i][1].value = cob_id
 
-    def _quit(self, signo, _frame):
-        '''Called when signals are caught'''
+        self._node.add_read_callback(self._on_sdo_read)
+        self._node.add_write_callback(self._on_sdo_write)
+
+    def __del__(self):
 
-        logger.debug(f'signal {signal.Signals(signo).name} was caught')
         self.stop()
 
+        if self._network:
+            try:
+                self._network.disconnect()
+            except Exception:
+                pass
+
+    def _on_sync(self, cob_id: int, data: bytes, timestamp: float):
+        '''On SYNC message send TPDOs configured to be SYNC-based'''
+
+        self._syncs += 1
+        if self._syncs == 241:
+            self._syncs = 1
+
+        for i in range(len(self._node.tpdo)):
+            transmission_type = self.od[0x1800 + i][2].value
+            if self._syncs % transmission_type == 0:
+                self.send_tpdo(i)
+
     def send_tpdo(self, tpdo: int):
-        '''Send a TPDO. Will not be sent if not node is not in operational state.
+        '''
+        Send a TPDO. Will not be sent if not node is not in operational state.
 
         Parameters
         ----------
         tpdo: int
             TPDO number to send
+
+        Raises
+        ------
+        NetworkError
+            Cannot send a TPDO message when the network is down.
         '''
 
+        if self._network is None:
+            raise NetworkError('network is down cannot send an TPDO message')
+
         # PDOs can't be sent if CAN bus is down and PDOs should not be sent if CAN bus not in
         # 'OPERATIONAL' state
         can_bus = psutil.net_if_stats().get(self._bus)
-        if not can_bus or (can_bus.isup and self._node.nmt.state != 'OPERATIONAL'):
-            return
+        if can_bus is None or (can_bus.isup and self._node.nmt.state != 'OPERATIONAL'):
+            return True
 
-        cob_id = self.od[0x1800 + tpdo][1].value
+        cob_id = self.od[0x1800 + tpdo][1].value & 0x3F_FF_FF_FF
         maps = self.od[0x1A00 + tpdo][0].value
 
         data = b''
         for i in range(maps):
             pdo_map = self.od[0x1A00 + tpdo][i + 1].value
 
             if pdo_map == 0:
@@ -241,144 +194,311 @@
 
             # pack pdo with bytes
             data += value_bytes
 
         try:
             i = self._network.send_message(cob_id, data)
         except Exception as exc:
-            logger.debug(f'TPDO{tpdo} failed with: {exc}')
+            logger.error(f'TPDO{tpdo} failed with: {exc}')
 
-    def _send_tpdo_loop(self, tpdo: int) -> bool:
+    def _tpdo_timer_loop(self, tpdo: int) -> bool:
+        '''Send TPDO for TPDO loop. Can handle network errors.'''
 
-        self.send_tpdo(tpdo)
+        try:
+            self.send_tpdo(tpdo)
+        except NetworkError:
+            pass
 
-        # get event time
-        value = self.od[0x1800 + tpdo][5].value
+        return True
 
-        # milliseconds as int to seconds as a float
-        delay = float(value) / 1000
+    def _start_tpdo_timer_loops(self) -> list:
+        '''Start TPDO timer loops'''
 
-        self._event.wait(delay)
+        tpdo_timers = []
 
-        return True
+        for i in range(len(self._node.tpdo)):
+            transmission_type = self.od[0x1800 + i][2].default
+            event_time = self.od[0x1800 + i][5].default
+            if transmission_type in [0xFE, 0xFF] and event_time > 0:
+                t = TimerLoop(name=f'TPDO{i + 1}', loop_func=self._tpdo_timer_loop,
+                              delay=self.od[0x1800 + i][5], start_delay=self.od[0x1800 + i][3],
+                              args=(i,))
+                tpdo_timers.append(t)
+                t.start()
+
+        return tpdo_timers
+
+    def _on_rpdo_update_od(self, map: canopen.pdo.base.Map):
+        '''Handle parsering an RPDO'''
 
-    def add_resource(self, resource: Resource):
-        '''Add a resource for the app'''
+        for i in map.map_array:
+            if i == 0:
+                continue
 
-        self._res.append(resource)
+            value = map.map_array[i].raw
+            if value == 0:
+                break  # no more mapping
+
+            index, subindex, size = struct.unpack('>HBB', value.to_bytes(4, 'big'))
+            if isinstance(self.od[index], canopen.objectdictionary.Variable):
+                self._node.sdo[index].raw = map.map[i - 1].get_data()
+            else:
+                self._node.sdo[index][subindex].raw = map.map[i - 1].get_data()
 
     def _restart_bus(self):
-        '''Reset the can bus to up'''
+        '''Try to restart the CAN bus'''
 
-        if self.first_bus_error:
+        if self.first_bus_reset:
             logger.error(f'{self._bus} is down')
-            self.first_bus_error = False
+            self.first_bus_reset = False
 
         if geteuid() == 0:  # running as root
-            if self.first_bus_error:
+            if self.first_bus_reset:
                 logger.info(f'trying to restart CAN bus {self._bus}')
 
             out = subprocess.run(f'ip link set {self._bus} up', shell=True)
             if out.returncode != 0:
                 logger.error(out)
 
     def _restart_network(self):
-        '''Restart the canopen network'''
+        '''Restart the CANopen network'''
 
-        logger.debug('(re)starting CANopen network')
+        logger.info('(re)starting CANopen network')
 
         self._network = canopen.Network()
         self._network.connect(bustype='socketcan', channel=self._bus)
         self._network.add_node(self._node)
 
         try:
             self._node.nmt.state = 'PRE-OPERATIONAL'
             self._node.nmt.start_heartbeat(self.od[0x1017].default)
             self._node.nmt.state = 'OPERATIONAL'
-            logger.info('(re)started CANopen network')
         except Exception as exc:
             logger.error(f'failed to (re)start CANopen network with {exc}')
 
+        self._network.subscribe(0x80, self._on_sync)
+
+        # setup RPDOs callbacks
+        self._node.rpdo.read()
+        for i in self._node.rpdo:
+            if self._node.rpdo[i].enabled:
+                self._node.rpdo[i].add_callback(self._on_rpdo_update_od)
+
+    def _disable_network(self):
+        '''Disable the CANopen network'''
+
+        try:
+            if self._network:
+                self._network.disconnect()
+        except Exception:
+            self._network = None  # make sure the canopen network is down
+
+    def _monitor_can(self):
+        '''Monitor the CAN bus and CAN network'''
+
+        first_bus_down = True  # flag to only log error message on first error
+        self.first_bus_reset = True  # flag to only log error message on first error
+        logger.info(f'{self.name} app is running')
+        while not self._event.is_set():
+            bus = psutil.net_if_stats().get(self._bus)
+            if not bus:  # bus does not exist
+                self._disable_network()
+                if first_bus_down:
+                    logger.critical(f'{self._bus} does not exists, nothing OLAF can do')
+                    first_bus_down = False
+            elif not bus.isup:  # bus is down
+                first_bus_down = True  # reset flag
+                self._disable_network()
+                self._restart_bus()
+            elif not self._network:  # bus is up, network is down
+                first_bus_down = True  # reset flag
+                self._restart_network()
+            else:  # bus is up, network is up
+                self.first_bus_reset = True  # reset flag
+                first_bus_down = True  # reset flag
+
+            self._event.wait(1)
+
     def run(self) -> int:
-        '''Go into operational mode, start all the resources, start all the threads, and monitor
+        '''
+        Go into operational mode, start all the resources, start all the threads, and monitor
         everything in a loop.
 
         Returns
         -------
-        int
-            Errno value or 0 for on no error.
+        NodeStop
+            Reset / power off condition.
         '''
         tpdo_timers = []
-        resources = []
 
-        logger.info(f'{self._name} app is starting')
+        logger.info(f'{self.name} app is starting')
         if geteuid() != 0:  # running as root
             logger.warning('not running as root, cannot restart CAN bus if it goes down')
 
-        if not psutil.net_if_stats().get(self._bus):
-            logger.critical(f'{self._bus} does not exist, nothing OLAF can do, exiting')
-            return errno.ENETUNREACH
-
-        # start the CANopen network
-        self._restart_network()
-
-        for resource in self._res:
-            res = resource(self.fread_cache, self.fwrite_cache, self._mock_hw, self.send_tpdo)
-            resources.append(res)
-            res.start(self._node)
-
-        for i in range(len(self._node.tpdo)):
-            transmission_type = self.od[0x1800 + i][2].default
-            event_time = self.od[0x1800 + i][5].default
-
-            if transmission_type in [0xFE, 0xFF] and event_time and event_time > 0:
-                t = TimerLoop(f'TPDO{i + 1}', self._send_tpdo_loop, 0, args=(i,))
-                t.start()
-                tpdo_timers.append(t)
-
-        self.first_bus_error = True  # flag to only log error message on first error
-        logger.info(f'{self._name} app is running')
-        while not self._event.is_set():
-            if not psutil.net_if_stats().get(self._bus):  # bus does not exist
-                logger.critical(f'{self._bus} no longer exists, nothing OLAF can do, exiting')
-                self._event.set()
-                break
-            elif not psutil.net_if_stats().get(self._bus).isup:  # bus is down
-                self._network = None  # make sure the canopen network is down
-                self._restart_bus()
-            else:  # bus is up
-                if not self._network:  # network is down
-                    self._restart_network()
-                else:
-                    self.first_bus_error = True  # reset flag
-
-            self._event.wait(1)
+        tpdo_timers = self._start_tpdo_timer_loops()
 
-        for res in resources:
-            res.end()
+        try:
+            self._monitor_can()
+        except Exception as e:
+            logger.critical(e)
 
         for t in tpdo_timers:
             t.stop()
 
-        logger.info(f'{self._name} app has ended')
-        return 0
+        logger.info(f'{self.name} app has ended')
+        return self._reset
 
-    def stop(self):
+    def stop(self, reset: NodeStop = NodeStop.SOFT_RESET):
         '''End the run loop'''
 
+        self._reset = reset
         self._event.set()
 
+    def add_sdo_read_callback(self, index: int, sdo_cb):
+        '''
+        Add an SDO read callback
+
+        Parameters
+        ----------
+        index: int
+            The index to call the callback on.
+        sdo_cb
+            The SDO read callback. Must take index and subindex args and return a valid value or
+            None to use the value from the OD.
+        '''
+
+        if index not in self._read_cbs:
+            self._read_cbs[index] = [sdo_cb]
+        else:
+            self._read_cbs[index].append(sdo_cb)
+
+    def add_sdo_write_callback(self, index: int, sdo_cb):
+        '''
+        Add an SDO write callback
+
+        Parameters
+        ----------
+        index: int
+            The index to call the callback on.
+        sdo_cb
+            The SDO read callback. Must take index, subindex, value args.
+        '''
+
+        if index not in self._write_cbs:
+            self._write_cbs[index] = [sdo_cb]
+        else:
+            self._write_cbs[index].append(sdo_cb)
+
+    def send_emcy(self, code: int, register: int = 0, data: bytes = b''):
+        '''
+        Send a EMCY message. Wrapper on canopen's `EmcyProducer.send`.
+
+        Parameters
+        ----------
+        code: int
+            The EMCY code.
+        register: int
+            Optional error register value in EMCY message (uint8). See Object 1001 def for bit
+            field.
+        manufacturer_code: bytes
+            Optional manufacturer error code (up to 5 bytes).
+
+        Raises
+        ------
+        NetworkError
+            Cannot send a EMCY message when the network is down.
+        '''
+
+        if self._network is None:
+            raise NetworkError('network is down cannot send an EMCY message')
+
+        self._node.emcy.send(code, register, data)
+
+    def _on_sdo_read(self, index: int, subindex: int, od: canopen.objectdictionary.Variable):
+        '''
+        SDO read callback function. Allows overriding the data being sent on a SDO read. Return
+        valid datatype for object, if overriding read data, or :py:data:`None` to use the the value
+        on object dictionary.
+
+        Parameters
+        ----------
+        index: int
+            The index the SDO is reading to.
+        subindex: int
+            The subindex the SDO is reading to.
+        od: canopen.objectdictionary.Variable
+            The variable object being read tp. Badly named.
+
+        Returns
+        -------
+        Any
+            The value to return for that index / subindex. Return :py:data:`None` if invalid index
+            / subindex.
+        '''
+
+        ret = None
+
+        if index in self._read_cbs:
+            for cb_func in self._read_cbs[index]:
+                try:
+                    ret = cb_func(index, subindex)
+                except Exception as e:
+                    logger.error(f'sdo read cb for 0x{index:04X} 0x{subindex:02X} raised: {e}')
+
+        return ret
+
+    def _on_sdo_write(self, index: int, subindex: int, od: canopen.objectdictionary.Variable,
+                      data: bytes):
+        '''SDO write callback function. Gives access to the data being received on a SDO write.
+
+        *Note:* data is still written to object dictionary before call.
+
+        Parameters
+        ----------
+        index: int
+            The index the SDO being written to.
+        subindex: int
+            The subindex the SDO being written to.
+        od: canopen.objectdictionary.Variable
+            The variable object being written to. Badly named.
+        data: bytes
+            The raw data being written.
+        '''
+
+        if index in self._write_cbs:
+            value = od.decode_raw(data)
+            for cb_func in self._write_cbs[index]:
+                try:
+                    cb_func(index, subindex, value)
+                except Exception as e:
+                    logger.error(f'sdo write cb for 0x{index:04X} 0x{subindex:02X} raised: {e}')
+
+    @property
+    def name(self) -> str:
+        '''str: The nodes name.'''
+
+        if self._node:
+            return self._node.object_dictionary.device_information.product_name
+
     @property
-    def od(self):
-        '''For convenience. Access to the object dictionary.'''
+    def od(self) -> canopen.ObjectDictionary:
+        '''canopen.ObjectDictionary: Access to the object dictionary.'''
 
         return self._node.object_dictionary
 
     @property
-    def node(self):
-        '''For convenience. Access to the CANopen node.'''
+    def fread_cache(self) -> OreSatFileCache:
+        '''OreSatFile: Cache the CANopen master node can read to.'''
 
-        return self._node
+        return self._fread_cache
 
+    @property
+    def fwrite_cache(self) -> OreSatFileCache:
+        '''OreSatFile: Cache the CANopen master node can write to.'''
+
+        return self._fwrite_cache
+
+    @property
+    def is_running(self) -> bool:
+        '''bool: is the node loop running'''
 
-app = App()
-'''The global instance of the OLAF app.'''
+        return not self._event.is_set()
```

### Comparing `oresat-olaf-1.0.0/olaf/_internals/data/oresat_app.eds` & `oresat-olaf-2.0.0/olaf/_internals/data/oresat_app.eds`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 ParameterName=Serial number
 ObjectType=0x07
 DataType=0x0007
 AccessType=ro
 DefaultValue=0x00000000
 
 [OptionalObjects]
-SupportedObjects=83
+SupportedObjects=85
 1=0x1002
 2=0x1003
 3=0x1005
 4=0x1006
 5=0x1007
 6=0x1008
 7=0x1009
@@ -122,82 +122,84 @@
 9=0x1010
 10=0x1011
 11=0x1014
 12=0x1015
 13=0x1016
 14=0x1017
 15=0x1019
-16=0x1023
-17=0x1029
-18=0x1200
-19=0x1400
-20=0x1401
-21=0x1402
-22=0x1403
-23=0x1404
-24=0x1405
-25=0x1406
-26=0x1407
-27=0x1408
-28=0x1409
-29=0x140A
-30=0x140B
-31=0x140C
-32=0x140D
-33=0x140E
-34=0x140F
-35=0x1600
-36=0x1601
-37=0x1602
-38=0x1603
-39=0x1604
-40=0x1605
-41=0x1606
-42=0x1607
-43=0x1608
-44=0x1609
-45=0x160A
-46=0x160B
-47=0x160C
-48=0x160D
-49=0x160E
-50=0x160F
-51=0x1800
-52=0x1801
-53=0x1802
-54=0x1803
-55=0x1804
-56=0x1805
-57=0x1806
-58=0x1807
-59=0x1808
-60=0x1809
-61=0x180A
-62=0x180B
-63=0x180C
-64=0x180D
-65=0x180E
-66=0x180F
-67=0x1A00
-68=0x1A01
-69=0x1A02
-70=0x1A03
-71=0x1A04
-72=0x1A05
-73=0x1A06
-74=0x1A07
-75=0x1A08
-76=0x1A09
-77=0x1A0A
-78=0x1A0B
-79=0x1A0C
-80=0x1A0D
-81=0x1A0E
-82=0x1A0F
-83=0x1F80
+16=0x1021
+17=0x1022
+18=0x1023
+19=0x1029
+20=0x1200
+21=0x1400
+22=0x1401
+23=0x1402
+24=0x1403
+25=0x1404
+26=0x1405
+27=0x1406
+28=0x1407
+29=0x1408
+30=0x1409
+31=0x140A
+32=0x140B
+33=0x140C
+34=0x140D
+35=0x140E
+36=0x140F
+37=0x1600
+38=0x1601
+39=0x1602
+40=0x1603
+41=0x1604
+42=0x1605
+43=0x1606
+44=0x1607
+45=0x1608
+46=0x1609
+47=0x160A
+48=0x160B
+49=0x160C
+50=0x160D
+51=0x160E
+52=0x160F
+53=0x1800
+54=0x1801
+55=0x1802
+56=0x1803
+57=0x1804
+58=0x1805
+59=0x1806
+60=0x1807
+61=0x1808
+62=0x1809
+63=0x180A
+64=0x180B
+65=0x180C
+66=0x180D
+67=0x180E
+68=0x180F
+69=0x1A00
+70=0x1A01
+71=0x1A02
+72=0x1A03
+73=0x1A04
+74=0x1A05
+75=0x1A06
+76=0x1A07
+77=0x1A08
+78=0x1A09
+79=0x1A0A
+80=0x1A0B
+81=0x1A0C
+82=0x1A0D
+83=0x1A0E
+84=0x1A0F
+85=0x1F80
 
 [1002]
 ParameterName=Manufacturer status register
 ObjectType=0x07
 DataType=0x0007
 AccessType=ro
 DefaultValue=0
@@ -485,14 +487,30 @@
 [1019]
 ParameterName=Synchronous counter overflow value
 ObjectType=0x07
 DataType=0x0005
 AccessType=rw
 DefaultValue=0
 
+;A master node can read this for a copy of the node's EDS file
+[1021]
+ParameterName=Store EDS
+ObjectType=0x07
+DataType=0x000F
+AccessType=ro
+DefaultValue=0
+
+;Indicate the format of the Store EDS
+[1022]
+ParameterName=Store format
+ObjectType=0x07
+DataType=0x0005
+AccessType=ro
+DefaultValue=0
+
 [1023]
 ParameterName=OS command
 ObjectType=0x09
 SubNumber=4
 
 [1023sub0]
 ParameterName=Highest sub-index supported
@@ -502,27 +520,29 @@
 DefaultValue=0x03
 
 [1023sub1]
 ParameterName=Command
 ObjectType=0x07
 DataType=0x000F
 AccessType=rw
+DefaultValue=0
 
 [1023sub2]
 ParameterName=Status
 ObjectType=0x07
 DataType=0x0005
 AccessType=ro
 DefaultValue=0
 
 [1023sub3]
 ParameterName=Reply
 ObjectType=0x07
 DataType=0x000F
 AccessType=ro
+DefaultValue=0
 
 [1029]
 ParameterName=Error behavior
 ObjectType=0x08
 SubNumber=3
 
 [1029sub0]
@@ -587,15 +607,15 @@
 SubNumber=4
 
 [1400sub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x03
+DefaultValue=0x05
 
 [1400sub1]
 ParameterName=COB-ID used by RPDO
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
 DefaultValue=0x00000181
@@ -620,15 +640,15 @@
 SubNumber=4
 
 [1401sub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x03
+DefaultValue=0x05
 
 [1401sub1]
 ParameterName=COB-ID used by RPDO
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
 DefaultValue=0x80000300+$NODEID
@@ -653,15 +673,15 @@
 SubNumber=4
 
 [1402sub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x03
+DefaultValue=0x05
 
 [1402sub1]
 ParameterName=COB-ID used by RPDO
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
 DefaultValue=0x80000400+$NODEID
@@ -686,15 +706,15 @@
 SubNumber=4
 
 [1403sub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x03
+DefaultValue=0x05
 
 [1403sub1]
 ParameterName=COB-ID used by RPDO
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
 DefaultValue=0x80000500+$NODEID
@@ -719,15 +739,15 @@
 SubNumber=4
 
 [1404sub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x03
+DefaultValue=0x05
 
 [1404sub1]
 ParameterName=COB-ID used by RPDO
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
 DefaultValue=0x80000200+$NODEID
@@ -752,15 +772,15 @@
 SubNumber=4
 
 [1405sub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x03
+DefaultValue=0x05
 
 [1405sub1]
 ParameterName=COB-ID used by RPDO
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
 DefaultValue=0x80000300+$NODEID
@@ -785,15 +805,15 @@
 SubNumber=4
 
 [1406sub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x03
+DefaultValue=0x05
 
 [1406sub1]
 ParameterName=COB-ID used by RPDO
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
 DefaultValue=0x80000400+$NODEID
@@ -818,15 +838,15 @@
 SubNumber=4
 
 [1407sub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x03
+DefaultValue=0x05
 
 [1407sub1]
 ParameterName=COB-ID used by RPDO
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
 DefaultValue=0x80000500+$NODEID
@@ -851,15 +871,15 @@
 SubNumber=4
 
 [1408sub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x03
+DefaultValue=0x05
 
 [1408sub1]
 ParameterName=COB-ID used by RPDO
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
 DefaultValue=0x80000200+$NODEID
@@ -884,15 +904,15 @@
 SubNumber=4
 
 [1409sub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x03
+DefaultValue=0x05
 
 [1409sub1]
 ParameterName=COB-ID used by RPDO
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
 DefaultValue=0x80000300+$NODEID
@@ -917,15 +937,15 @@
 SubNumber=4
 
 [140Asub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x03
+DefaultValue=0x05
 
 [140Asub1]
 ParameterName=COB-ID used by RPDO
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
 DefaultValue=0x80000400+$NODEID
@@ -950,15 +970,15 @@
 SubNumber=4
 
 [140Bsub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x03
+DefaultValue=0x05
 
 [140Bsub1]
 ParameterName=COB-ID used by RPDO
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
 DefaultValue=0x80000500+$NODEID
@@ -983,15 +1003,15 @@
 SubNumber=4
 
 [140Csub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x03
+DefaultValue=0x05
 
 [140Csub1]
 ParameterName=COB-ID used by RPDO
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
 DefaultValue=0x80000200+$NODEID
@@ -1016,15 +1036,15 @@
 SubNumber=4
 
 [140Dsub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x03
+DefaultValue=0x05
 
 [140Dsub1]
 ParameterName=COB-ID used by RPDO
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
 DefaultValue=0x80000300+$NODEID
@@ -1049,15 +1069,15 @@
 SubNumber=4
 
 [140Esub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x03
+DefaultValue=0x05
 
 [140Esub1]
 ParameterName=COB-ID used by RPDO
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
 DefaultValue=0x80000400+$NODEID
@@ -1082,15 +1102,15 @@
 SubNumber=4
 
 [140Fsub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x03
+DefaultValue=0x05
 
 [140Fsub1]
 ParameterName=COB-ID used by RPDO
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
 DefaultValue=0x80000500+$NODEID
@@ -3012,15 +3032,15 @@
 ObjectType=0x09
 SubNumber=7
 
 [180Fsub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
-AccessType=ro
+AccessType=const
 DefaultValue=0x06
 
 [180Fsub1]
 ParameterName=COB-ID used by TPDO
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
@@ -4018,15 +4038,15 @@
 ObjectType=0x09
 SubNumber=9
 
 [1A0Esub0]
 ParameterName=Number of mapped application objects in PDO
 ObjectType=0x07
 DataType=0x0005
-AccessType=rw
+AccessType=const
 DefaultValue=0x08
 
 [1A0Esub1]
 ParameterName=Mapping object 1
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
@@ -4177,15 +4197,15 @@
 ObjectType=0x09
 SubNumber=5
 
 [2000sub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
-AccessType=ro
+AccessType=const
 DefaultValue=0x04
 
 ;Bdefault specifies the bus to be considered active after a node power-on, node hardware reset.
 [2000sub1]
 ParameterName=Bdefault
 ObjectType=0x07
 DataType=0x0005
@@ -4301,59 +4321,47 @@
 ;Manufacturer specific errors:
 ;Manufacturer may define its own constants up to index 0xFF. Of course, they must then define large enough buffer for error status bits (up to 32 bytes).
 [2100]
 ParameterName=Error status bits
 ObjectType=0x07
 DataType=0x000A
 AccessType=ro
-DefaultValue=00000000000000000000
+DefaultValue=00 00 00 00 00 00 00 00 00 00
 
 [3000]
-ParameterName=OLAF app control
+ParameterName=Power control
 ObjectType=0x09
-SubNumber=5
+SubNumber=3
 
 [3000sub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x04
+DefaultValue=0x02
 
-;Write true to restart the board
+;Write true to poweroff the system
 [3000sub1]
-ParameterName=Reboot Board
+ParameterName=Poweroff
 ObjectType=0x07
 DataType=0x0001
 AccessType=wo
 DefaultValue=0
 
-;Write true to poweroff the board
+;1 for a soft reset (restart daemon)
+;2 for hard reset (reboot the board)
+;3 to do a factory reset (clear all caches and reboot)
 [3000sub2]
-ParameterName=Poweroff Board
+ParameterName=Reset
 ObjectType=0x07
-DataType=0x0001
-AccessType=wo
-DefaultValue=0
-
-;Write true to have the OLAF app exit
-[3000sub3]
-ParameterName=Quit
-ObjectType=0x07
-DataType=0x0001
+DataType=0x0005
 AccessType=wo
 DefaultValue=0
-
-;Allow OLAF to control the board CPU frequency
-[3000sub4]
-ParameterName=CPU frequency
-ObjectType=0x07
-DataType=0x0001
-AccessType=rw
-DefaultValue=0
+LowLimit=0
+HighLimit=3
 
 [3001]
 ParameterName=System info
 ObjectType=0x09
 SubNumber=29
 
 [3001sub0]
@@ -4705,14 +4713,15 @@
 
 ;Data of the file selected in subindex 1
 [3003sub2]
 ParameterName=File data
 ObjectType=0x07
 DataType=0x000F
 AccessType=ro
+DefaultValue=0
 
 ;Gets the CRC32 of the file
 [3003sub3]
 ParameterName=CRC32
 ObjectType=0x07
 DataType=0x0007
 AccessType=ro
@@ -4747,14 +4756,15 @@
 
 ;File data for the new file written. Must set subindex 1 before writing to this subindex.
 [3004sub2]
 ParameterName=File data
 ObjectType=0x07
 DataType=0x000F
 AccessType=wo
+DefaultValue=0
 
 [3005]
 ParameterName=App manager
 ObjectType=0x09
 SubNumber=7
 
 [3005sub0]
@@ -4804,32 +4814,51 @@
 [3005sub6]
 ParameterName=Daemon state
 ObjectType=0x07
 DataType=0x0005
 AccessType=rw
 DefaultValue=0
 
-;Write any non-zero number to get system logs. Log will be place in fread cache.
 [3006]
-ParameterName=Get log
+ParameterName=New Record
+ObjectType=0x09
+SubNumber=3
+
+[3006sub0]
+ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
-AccessType=rw
+AccessType=const
+DefaultValue=0x02
+
+;This will make a compress tar archive of the full system logs. It will be add to the cache.
+[3006sub1]
+ParameterName=Make logs file
+ObjectType=0x07
+DataType=0x0001
+AccessType=wo
 DefaultValue=0
 
+;Get the logs since boot as a string.
+[3006sub2]
+ParameterName=Get logs
+ObjectType=0x07
+DataType=0x0009
+AccessType=ro
+
 [3100]
 ParameterName=Updater
 ObjectType=0x09
 SubNumber=6
 
 [3100sub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
-AccessType=ro
+AccessType=const
 DefaultValue=0x05
 
 ;Get the status of updater
 ;
 ;States:
 ; * update-succesful: 0x00
 ; * pre-update-failed: 0x01
```

### Comparing `oresat-olaf-1.0.0/olaf/_internals/resources/ecss.py` & `oresat-olaf-2.0.0/olaf/_internals/resources/ecss.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,44 +6,45 @@
 from ...common.resource import Resource
 from ...common.ecss import scet_int_from_time, utc_int_from_time, scet_int_to_time, utc_int_to_time
 
 
 class ECSSResource(Resource):
     '''Resource for ECSS CANBus Extended Protocal standards'''
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+    def __init__(self):
+        super().__init__()
 
         self.scet_index = 0x2010
         self.utc_index = 0x2011
 
     def on_start(self):
-        self.scet_obj = self.od[self.scet_index]
-        self.utc_obj = self.od[self.utc_index]
 
-    def on_read(self, index, subindex, od):
+        self.node.add_sdo_read_callback(self.scet_index, self.on_scet_read)
+        self.node.add_sdo_write_callback(self.scet_index, self.on_scet_write)
+        self.node.add_sdo_read_callback(self.utc_index, self.on_utc_read)
+        self.node.add_sdo_write_callback(self.utc_index, self.on_utc_write)
 
-        ret = None
+    def on_scet_read(self, index: int, subindex: int):
 
-        if index == self.scet_index:
-            ret = scet_int_from_time(time())
-        elif index == self.utc_index:
-            ret = utc_int_from_time(time())
+        return scet_int_from_time(time())
 
-        return ret
+    def on_scet_write(self, index: int, subindex: int, value):
 
-    def on_write(self, index, subindex, od, data):
+        ts = scet_int_to_time(value)
+        self._set_time(ts)
 
-        if index == self.scet_index:
-            raw = self.scet_obj.decode_raw(data)
-            ts = scet_int_to_time(raw)
-        elif index == self.utc_index:
-            raw = self.utc_index.decode_raw(data)
-            ts = utc_int_to_time(raw)
-        else:
-            return  # write is not for these indexes
+    def on_utc_read(self, index: int, subindex: int):
+
+        return utc_int_from_time(time())
+
+    def on_utc_write(self, index: int, subinde: int, value):
+
+        ts = utc_int_to_time(value)
+        self._set_time(ts)
 
+    def _set_time(self, ts: float):
         if geteuid() == 0:
             clock_settime(CLOCK_REALTIME, ts)
-            logger.info(f'{self.name} resource has set system time')
+            logger.info(f'{self.__class__.__name__} resource has set system time')
         else:
-            logger.error(f'{self.name} resource cannot set time, not running as root')
+            logger.error(f'{self.__class__.__name__} resource cannot set system time, not running '
+                         'as root')
```

### Comparing `oresat-olaf-1.0.0/olaf/_internals/resources/file_caches.py` & `oresat-olaf-2.0.0/olaf/_internals/resources/file_caches.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,37 +17,40 @@
     FILE_SIZE = auto()
     DELETE_FILE = auto()
 
 
 class FileCachesResource(Resource):
     '''Resource for interacting with the fread and fwrite caches'''
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+    def __init__(self):
+        super().__init__()
 
-        self.index = 0x3002
-        self.file_caches = [self.fread_cache, self.fwrite_cache]
-
-        # defaults
         self.selector = 0
         self.iter = 0
         self.filter = ''
+        self.index = 0x3002
+
+    def on_start(self):
+
+        self.file_caches = [self.node.fread_cache, self.node.fwrite_cache]
+        self.node.add_sdo_read_callback(self.index, self.on_read)
+        self.node.add_sdo_write_callback(self.index, self.on_write)
 
-    def on_read(self, index, subindex, od):
+    def on_read(self, index, subindex):
 
         ret = None
 
         if index != self.index:
             return ret
 
         try:
             if subindex == Subindex.FREAD_LEN:
-                ret = len(self.fread_cache)
+                ret = len(self.node.fread_cache)
             elif subindex == Subindex.FWRITE_LEN:
-                ret = len(self.fwrite_cache)
+                ret = len(self.node.fwrite_cache)
             elif subindex == Subindex.CACHE_SELECTOR:
                 ret = self.selector
             elif subindex == Subindex.FILTER:
                 ret = self.filter
             elif subindex == Subindex.CACHE_LENGTH:
                 ret = len(self.file_caches[self.selector].files(self.filter))
             elif subindex == Subindex.ITER:
@@ -60,31 +63,31 @@
                 file_path = f'{dir_name}/{file_name}'
                 ret = getsize(file_path)
         except Exception as exc:
             logger.error(exc)
 
         return ret
 
-    def on_write(self, index, subindex, od, data):
+    def on_write(self, index, subindex, value):
 
         if index != self.index:
             return
 
         try:
             if subindex == Subindex.CACHE_SELECTOR:
-                if self.od[index][subindex].decode_raw(data) in [0, 1]:  # check for invalid input
-                    self.selector = self.od[index][subindex].decode_raw(data)
+                if value in [0, 1]:  # check for invalid input
+                    self.selector = value
             elif subindex == Subindex.FILTER:
-                if data == b'\x00':  # just NULL terminator mean no filter
+                if value == '':  # aka no filter
                     self.filter = ''
                     logger.debug('file cache filter clear')
                 else:
-                    self.filter = data.decode()
+                    self.filter = value
                     logger.debug(f'file cache filter now "{self.filter}"')
             elif subindex == Subindex.ITER:
-                self.iter = self.od[index][subindex].decode_raw(data)
+                self.iter = value
             elif subindex == Subindex.DELETE_FILE:
                 file_name = self.file_caches[self.selector].files(self.filter)[self.iter].name
                 self.file_caches[self.selector].remove(file_name)
                 logger.info(f'deleted {file_name}')
         except Exception as exc:
             logger.error(exc)
```

### Comparing `oresat-olaf-1.0.0/olaf/_internals/resources/fread.py` & `oresat-olaf-2.0.0/olaf/_internals/resources/fread.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,28 +15,32 @@
     CRC32 = auto()
     DELETE_FILE = auto()
 
 
 class FreadResource(Resource):
     '''Resource for readings file over the CAN bus'''
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+    def __init__(self):
+        super().__init__()
+
+        self.index = 0x3003
+        self.file_path = ''
 
         self.tmp_dir = '/tmp/oresat/fread'
         Path(self.tmp_dir).mkdir(parents=True, exist_ok=True)
         logger.debug(f'fread tmp dir is {self.tmp_dir}')
         for i in listdir(self.tmp_dir):
             remove(f'{self.tmp_dir}/{i}')
 
-        self.index = 0x3003
+    def on_start(self):
 
-        self.file_path = ''
+        self.node.add_sdo_read_callback(self.index, self.on_read)
+        self.node.add_sdo_write_callback(self.index, self.on_write)
 
-    def on_read(self, index, subindex, od):
+    def on_read(self, index, subindex):
 
         ret = None
 
         if index != self.index:
             return ret
 
         if subindex == Subindex.FILE_NAME:
@@ -56,33 +60,27 @@
                 with open(self.file_path, 'rb') as f:
                     ret = f.read()
             except FileNotFoundError as exc:
                 logger.error(exc)
 
         return ret
 
-    def on_write(self, index, subindex, od, data):
+    def on_write(self, index, subindex, value):
 
         if index != self.index:
             return
 
         if subindex == Subindex.FILE_NAME:
-            # delete old file if it exist
-            if self.file_path:
-                remove(self.file_path)
-                self.file_path = ''
-
-            file_name = data.decode()
             try:
-                self.file_path = self.fread_cache.get(file_name, self.tmp_dir, True)
+                self.file_path = self.node.fread_cache.get(value, self.tmp_dir, True)
             except FileNotFoundError:
-                logger.error(f'file {file_name} not in fread cache')
+                logger.error(f'file {value} not in fread cache')
                 self.file_path = ''
         elif subindex == Subindex.DELETE_FILE:
             if self.file_path:
                 # delete file from cache and tmp dir
-                self.fread_cache.remove(basename(self.file_path))
+                self.node.fread_cache.remove(basename(self.file_path))
                 remove(self.file_path)
                 self.file_path = ''
                 logger.info(f'{basename(self.file_path)} was deleted from fread cache')
             else:
                 logger.error('fread file path was not set before trying to delete file')
```

### Comparing `oresat-olaf-1.0.0/olaf/_internals/resources/fwrite.py` & `oresat-olaf-2.0.0/olaf/_internals/resources/fwrite.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,61 +13,63 @@
     FILE_NAME = auto()
     FILE_DATA = auto()
 
 
 class FwriteResource(Resource):
     '''Resource for writing files over the CAN bus'''
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+    def __init__(self):
+        super().__init__()
+
+        self.index = 0x3004
+        self.file_path = ''
 
         self.tmp_dir = '/tmp/oresat/fwrite'
         Path(self.tmp_dir).mkdir(parents=True, exist_ok=True)
         logger.debug(f'fread tmp dir is {self.tmp_dir}')
         for i in listdir(self.tmp_dir):
             remove(f'{self.tmp_dir}/{i}')
 
-        self.index = 0x3004
+    def on_start(self):
 
-        self.file_path = ''
+        self.node.add_sdo_read_callback(self.index, self.on_read)
+        self.node.add_sdo_write_callback(self.index, self.on_write)
 
-    def on_read(self, index, subindex, od):
+    def on_read(self, index, subindex, value):
 
         ret = None
 
         if index == self.index and subindex == Subindex.FILE_NAME:
             ret = basename(self.file_path)
 
         return ret
 
-    def on_write(self, index, subindex, od, data):
+    def on_write(self, index, subindex, value):
 
         if index != self.index:
             return
 
         if subindex == Subindex.FILE_NAME:
-            file_name = data.decode()
-
             try:
-                OreSatFile(file_name)  # valiate file name format
-                self.file_path = self.tmp_dir + '/' + file_name
+                OreSatFile(value)  # valiate file name format
+                self.file_path = self.tmp_dir + '/' + value
             except ValueError:
-                logger.error(f'{file_name} is not a valid file name format')
+                logger.error(f'{value} is not a valid file name format')
                 self.file_path = ''
 
         elif subindex == Subindex.FILE_DATA:
             if not self.file_path:
                 logger.error('fwrite file path was not set before file data was sent')
                 return
 
             try:
                 with open(self.file_path, 'wb') as f:
-                    f.write(data)
+                    f.write(value)
                 logger.info(f'receive new file: {basename(self.file_path)}')
-                self.fwrite_cache.add(self.file_path, consume=True)
+                self.node.fwrite_cache.add(self.file_path, consume=True)
             except Exception as exc:
                 logger.error(exc)
 
             self.file_path = ''
 
             # clear buffers to not waste memory
-            self.od[index][subindex].value = ''
+            self.node.od[index][subindex].value = ''
```

### Comparing `oresat-olaf-1.0.0/olaf/_internals/resources/logs.py` & `oresat-olaf-2.0.0/olaf/_internals/resources/logs.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,42 +7,54 @@
 from ...common.oresat_file import new_oresat_file
 from ...common.timer_loop import TimerLoop
 
 
 class LogsResource(Resource):
     '''Resource for getting logs'''
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+    def __init__(self):
+        super().__init__()
 
         self.index = 0x3006
         self.logs_dir_path = '/var/log/journal/'
 
-        self.timer_loop = TimerLoop('logs resource', self._loop, 0.5)
+        self.timer_loop = TimerLoop('logs resource', self._loop, 500)
         self.failed = True
 
+    def on_start(self):
+
+        self.make_logs_obj = self.node.od[self.index][1]
+        self.make_logs_obj.value = False  # make sure this is False by default
+
+        self.node.add_sdo_read_callback(self.index, self.on_read)
+
+        self.timer_loop.start()
+
+    def on_end(self):
+
+        self.timer_loop.stop()
+
     def _loop(self):
 
-        if self.obj.value:
+        if self.make_logs_obj.value:
             logger.info('Making a copy of logs')
 
             tar_file_path = '/tmp/' + new_oresat_file('logs', ext='.tar.xz')
 
             with tarfile.open(tar_file_path, 'w:xz') as t:
                 for i in listdir(self.logs_dir_path):
                     t.add(self.logs_dir_path + '/' + i, arcname=i)
 
-            self.fread_cache.add(tar_file_path, consume=True)
-            self.obj.value = False
+            self.node.fread_cache.add(tar_file_path, consume=True)
+            self.make_logs_obj.value = False
 
         return True
 
-    def on_start(self):
+    def on_read(self, index: int, subindex: int):
 
-        self.obj = self.od[self.index]
-        self.obj.value = False  # make sure this is False by default
+        if index != self.index and subindex != 2:
+            return
 
-        self.timer_loop.start()
+        with open('/tmp/olaf.log', 'r') as f:
+            ret = ''.join(reversed(f.readlines()[:250]))
 
-    def on_end(self):
-
-        self.timer_loop.stop()
+        return ret
```

### Comparing `oresat-olaf-1.0.0/olaf/_internals/resources/os_command.py` & `oresat-olaf-2.0.0/olaf/_internals/resources/os_command.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,30 +14,40 @@
     ERROR_REPLY = 0x03
     EXECUTING = 0xFF
 
 
 class OSCommandResource(Resource):
     '''Resource for running OS (bash) commands over CAN bus as defined by CiA 301 specs'''
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+    def __init__(self):
+        super().__init__()
 
         self.index = 0x1023
         self.sub_command = 0x01
         self.sub_state = 0x02
         self.sub_reply = 0x03
 
         self.command = ''
         self.state = OSCommandState.NO_ERROR_NO_REPLY
         self.reply = ''
         self.reply_max_len = 10000
+        self.failed = False
 
-        self.timer_loop = TimerLoop('os command resource', self._loop, 0.5,
+        self.timer_loop = TimerLoop('os command resource', self._loop, 500,
                                     exc_func=self._loop_error)
-        self.failed = False
+
+    def on_start(self):
+
+        self.node.add_sdo_read_callback(self.index, self.on_read)
+        self.node.add_sdo_write_callback(self.index, self.on_write)
+        self.timer_loop.start()
+
+    def on_end(self):
+
+        self.timer_loop.stop()
 
     def _loop(self):
 
         if self.state == OSCommandState.EXECUTING:
             logger.info('Running OS command: ' + self.command)
 
             out = subprocess.run(self.command, capture_output=True, shell=True)
@@ -61,39 +71,31 @@
     def _loop_error(self, exc: Exception):
 
         self.failed = True
         self.command = ''
         self.state = OSCommandState.ERROR_NO_REPLY
         self.reply = ''
 
-    def on_start(self):
-
-        self.timer_loop.start()
-
-    def on_end(self):
-
-        self.timer_loop.stop()
-
-    def on_read(self, index, subindex, od):
+    def on_read(self, index, subindex):
 
         ret = None
 
         if index == self.index and not self.failed:
             if subindex == self.sub_command:
                 ret = self.command.encode()
             elif subindex == self.sub_state:
                 ret = self.state.value
             elif subindex == self.sub_reply:
                 ret = self.reply.encode()
 
         return ret
 
-    def on_write(self, index, subindex, od, data):
+    def on_write(self, index, subindex, value):
 
         if index == self.index and subindex == self.sub_command:
             if self.state == OSCommandState.EXECUTING or self.failed:
                 logger.eror('cannot start another os command when one is running')
                 return
 
             self.reply = ''
-            self.command = data.decode()
+            self.command = value.decode()
             self.state = OSCommandState.EXECUTING  # run os command
```

### Comparing `oresat-olaf-1.0.0/olaf/_internals/resources/system_info.py` & `oresat-olaf-2.0.0/olaf/_internals/resources/system_info.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import platform
 from time import time
 from enum import IntEnum, auto
 
 import psutil
 
 from ...common.resource import Resource
+from ...common.cpufreq import get_cpufreq, get_cpufreq_gov
 
 _B_TO_MB = 1024 * 1024
 
 
 class Subindex(IntEnum):
     OS_NAME = auto()
     OS_DISTRO = auto()
@@ -40,100 +41,99 @@
     ROOT_PART_FREE = auto()
     ROOT_PART_PERCENT = auto()
 
 
 class SystemInfoResource(Resource):
     '''Resource for getting local system infomation'''
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+    def __init__(self):
+        super().__init__()
 
         self.index = 0x3001
         self.rprocs = 0
         self.rproc_iter = 0
 
     def on_start(self):
 
         with open('/etc/os-release', 'r') as f:
             os_release = f.readlines()
 
-        si_record = self.od[self.index]
+        si_record = self.node.od[self.index]
         si_record[Subindex.OS_NAME.value].value = platform.system()
         si_record[Subindex.OS_DISTRO.value].value = os_release[1].split('"')[1]
         si_record[Subindex.OS_KERNEL_VER.value].value = platform.release()
         si_record[Subindex.HOSTNAME.value].value = platform.node()
         si_record[Subindex.NUM_OF_CPUS.value].value = psutil.cpu_count()
         si_record[Subindex.CPU_ARCH.value].value = platform.machine()
         si_record[Subindex.RAM_TOTAL.value].value = psutil.virtual_memory().total // _B_TO_MB
         si_record[Subindex.SWAP_TOTAL.value].value = psutil.swap_memory().total // _B_TO_MB
         si_record[Subindex.ROOT_PART_TOTAL.value].value = psutil.disk_usage('/').total // _B_TO_MB
         if os.path.isdir('/sys/class/remoteproc'):
-            self.rprocs = len(os.listdir('/sys/class/remoteproc'))
-            # save for `on_read`
+            self.rprocs = len(os.listdir('/sys/class/remoteproc'))  # save for `on_read`
         si_record[Subindex.NUM_OF_RPROCS.value].value = self.rprocs
 
-    def on_read(self, index, subindex, od):
+        self.node.add_sdo_read_callback(self.index, self.on_read)
+        self.node.add_sdo_write_callback(self.index, self.on_write)
+
+    def on_read(self, index: int, subindex: int):
 
         if index != self.index:
             return
 
         ret = None
 
-        if subindex == Subindex.UPTIME.value:
+        if subindex == Subindex.UPTIME:
             ret = int(time() - psutil.boot_time())
-        elif subindex == Subindex.CPU_GOV.value:
-            file_path = '/sys/devices/system/cpu/cpu0/cpufreq/scaling_governor'
-            if os.path.exists(file_path):
-                with open(file_path, 'r') as f:
-                    ret = f.read().strip()
-        elif subindex == Subindex.CPU_FREQ.value:
-            # there was MHz vs GHz bug with psutil v5.9.0
-            ret = int(psutil.cpu_freq().current)
-            if ret < 10:  # value was in GHz, not MHz
-                ret = int(psutil.cpu_freq().current * 1000)
-        elif subindex == Subindex.RPROC_ITER.value:
+        elif subindex == Subindex.CPU_GOV:
+            ret = get_cpufreq_gov()
+        elif subindex == Subindex.CPU_FREQ:
+            ret = get_cpufreq()
+        elif subindex == Subindex.RPROC_ITER:
             ret = self.rproc_iter
-        elif subindex == Subindex.RPROC_NAME.value:
+        elif subindex == Subindex.RPROC_NAME:
             file_path = f'/sys/class/remoteproc/remoteproc{self.rprocs}/state'
             if os.path.exists(file_path):
                 with open(file_path, 'r') as f:
                     ret = f.read()
-        elif subindex == Subindex.RPROC_STATE.value:
+            else:
+                return ''
+        elif subindex == Subindex.RPROC_STATE:
             file_path = f'/sys/class/remoteproc/remoteproc{self.rprocs}/state'
             if os.path.exists(file_path):
                 with open(file_path, 'r') as f:
                     ret = f.read()
-        elif subindex == Subindex.LOAD_AVG_1MIN.value:
+            else:
+                return ''
+        elif subindex == Subindex.LOAD_AVG_1MIN:
             ret = int(psutil.getloadavg()[0] * 100)
-        elif subindex == Subindex.LOAD_AVG_5MIN.value:
+        elif subindex == Subindex.LOAD_AVG_5MIN:
             ret = int(psutil.getloadavg()[1] * 100)
-        elif subindex == Subindex.LOAD_AVG_15MIN.value:
+        elif subindex == Subindex.LOAD_AVG_15MIN:
             ret = int(psutil.getloadavg()[2] * 100)
-        elif subindex == Subindex.RAM_FREE.value:
+        elif subindex == Subindex.RAM_FREE:
             ret = psutil.virtual_memory().free // _B_TO_MB
-        elif subindex == Subindex.RAM_SHARED.value:
+        elif subindex == Subindex.RAM_SHARED:
             ret = psutil.virtual_memory().shared // _B_TO_MB
-        elif subindex == Subindex.RAM_BUFFERED.value:
+        elif subindex == Subindex.RAM_BUFFERED:
             ret = psutil.virtual_memory().buffers // _B_TO_MB
-        elif subindex == Subindex.RAM_PERCENT.value:
+        elif subindex == Subindex.RAM_PERCENT:
             ret = psutil.virtual_memory().percent
-        elif subindex == Subindex.SWAP_FREE.value:
+        elif subindex == Subindex.SWAP_FREE:
             ret = psutil.swap_memory().free // _B_TO_MB
-        elif subindex == Subindex.SWAP_PERCENT.value:
+        elif subindex == Subindex.SWAP_PERCENT:
             ret = psutil.swap_memory().percent
-        elif subindex == Subindex.PROCS.value:
+        elif subindex == Subindex.PROCS:
             ret = len(psutil.pids())
-        elif subindex == Subindex.ROOT_PART_FREE.value:
+        elif subindex == Subindex.ROOT_PART_FREE:
             ret = psutil.disk_usage('/').free // _B_TO_MB
-        elif subindex == Subindex.ROOT_PART_PERCENT.value:
+        elif subindex == Subindex.ROOT_PART_PERCENT:
             ret = psutil.disk_usage('/').percent
 
         return ret
 
-    def on_write(self, index, subindex, od, data):
+    def on_write(self, index: int, subindex: int, value):
 
-        if index != self.index or subindex != Subindex.RPROC_ITER.value:
+        if index != self.index or subindex != Subindex.RPROC_ITER:
             return
 
-        temp = od.decode_raw(data)
-        if temp < self.rprocs:
-            self.rproc_iter = temp
+        if value < self.rprocs:
+            self.rproc_iter = value
```

### Comparing `oresat-olaf-1.0.0/olaf/_internals/resources/updater.py` & `oresat-olaf-2.0.0/olaf/_internals/resources/updater.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from pathlib import Path
 from enum import IntEnum, auto
 
 from loguru import logger
 
 from ...common.resource import Resource
 from ...common.timer_loop import TimerLoop
 from ..updater import Updater, UpdaterError
@@ -15,58 +14,61 @@
     UPDATE = auto()
     MAKE_STATUS_FILE = auto()
 
 
 class UpdaterResource(Resource):
     '''Resource for interacting with the updater'''
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-        self._updater = Updater('/tmp/updater', f'{Path.home()}/.cache/oresat/updates')
+    def __init__(self, updater: Updater):
+        super().__init__()
 
+        self._updater = updater
         self.index = 0x3100
+        self.timer_loop = TimerLoop('updater resource', self._loop, 500)
+
+    def on_start(self):
+
+        record = self.node.od[self.index]
+        self.update_obj = record[Subindex.UPDATE.value]
+        self.make_status_obj = record[Subindex.MAKE_STATUS_FILE.value]
+        self.timer_loop.start()
 
-        self.timer_loop = TimerLoop('updater resource', self._loop, 0.5)
+        # make sure defaults are set correctly (override the values from eds/dcf)
+        self.update_obj.value = False
+        self.make_status_obj.value = False
+
+        self.node.add_sdo_read_callback(self.index, self.on_read)
+
+    def on_end(self):
+
+        self.timer_loop.stop()
 
     def _loop(self):
 
-        for i in self.fwrite_cache.files('update'):
-            self._updater.add_update(self.fwrite_cache.dir + '/' + i)
+        # check for update files in fwrite cache
+        for i in self.node.fwrite_cache.files('update'):
+            self._updater.add_update(self.node.fwrite_cache.dir + '/' + i)
 
+        # check for flag to start a update
         if self.update_obj.value:
             try:
                 self._updater.update()
             except UpdaterError as exc:
                 logger.critical(exc)
             self.update_obj.value = False
 
+        # check for flag to make a status archive
         if self.make_status_obj.value:
             status_archive_file_path = self._updater.make_status_archive()
-            self.fread_cache.add(status_archive_file_path, consume=True)
+            self.node.fread_cache.add(status_archive_file_path, consume=True)
             self.make_status_obj.value = False
 
         return True
 
-    def on_start(self):
-
-        record = self.od[self.index]
-        self.update_obj = record[Subindex.UPDATE.value]
-        self.make_status_obj = record[Subindex.MAKE_STATUS_FILE.value]
-        self.timer_loop.start()
-
-        # make sure defaults are set correctly (override the values from eds/dcf)
-        self.update_obj.value = False
-        self.make_status_obj.value = False
-
-    def on_end(self):
-
-        self.timer_loop.stop()
-
-    def on_read(self, index, subindex, od):
+    def on_read(self, index: int, subindex: int):
 
         ret = None
 
         if index == self.index:
             if subindex == Subindex.STATUS:
                 ret = self._updater.status.value
             elif subindex == Subindex.UPDATES_CACHED:
```

### Comparing `oresat-olaf-1.0.0/olaf/_internals/rest_api/static/favicon.ico` & `oresat-olaf-2.0.0/olaf/_internals/rest_api/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `oresat-olaf-1.0.0/olaf/_internals/rest_api/templates/base.html` & `oresat-olaf-2.0.0/olaf/_internals/rest_api/templates/base.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,29 @@
 <!DOCTYPE html>
 <html lang='en'>
 <head>
   <title>{{title}}</title>
   <style>
-    #header {
+    #headerGrid {
+      display: grid;
+      grid-template-columns: 25% 50% 25%;
+    }
+    #headerCenter {
       text-align: center;
     }
   </style>
-  <div id='header'>
-    <h2>{{name}}</h2>
+  <div id='headerGrid'>
+    <div id='headerLeft'>
+       <a href='/'>home</a>
+    </div>
+    <div id='headerCenter'>
+      <h2>{{name}}</h2>
+    </div>
+    <div id='headerRight'>
+    </div>
   </div>
 </head>
 <body>
   <style>
     #content {
       text-align: center;
     }
@@ -25,15 +36,15 @@
      * @param {String} subindex The eubndex of the object to write to. Set to
      * null if subindex is not needed. 
      *
      * @return {Object} The object from the OD.
      */
     async function readValue(index, subindex) {
       let url = `http://${window.location.host}/od/${index}`;
-      if (subindex !== null || subindex !== '') {
+      if (subindex !== null && subindex !== '') {
         url = `http://${window.location.host}/od/${index}/${subindex}`;
       }
 
       return await fetch(url)
         .then(response => response.json())
         .then(data => { return data; });
     }
```

#### html2text {}

```diff
@@ -1,2 +1,3 @@
+home
 ***** {{name}} *****
 {% block content %}{% endblock %}
```

### Comparing `oresat-olaf-1.0.0/olaf/_internals/rest_api/templates/fread.html` & `oresat-olaf-2.0.0/olaf/_internals/rest_api/templates/fread.html`

 * *Files identical despite different names*

### Comparing `oresat-olaf-1.0.0/olaf/_internals/rest_api/templates/fwrite.html` & `oresat-olaf-2.0.0/olaf/_internals/rest_api/templates/fwrite.html`

 * *Files identical despite different names*

### Comparing `oresat-olaf-1.0.0/olaf/_internals/rest_api/templates/od.html` & `oresat-olaf-2.0.0/olaf/_internals/rest_api/templates/od.html`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
       margin-right: auto;
     }
     td, th {
       border: 1px solid #dddddd;
       text-align: left;
       padding: 8px;
     }
-    a, label {
+    label {
       font-weight: bold;
     }
     #variableObj, #arrayRecordObj, #varNewValueInput {
       display: none;
     }
   </style>
   <label for='objIndex'>Index:</label>
@@ -90,31 +90,31 @@
         document.getElementById('arrayRecordObj').style.display = 'none';
 
         alert(obj['error']);
       } else if (obj['object_type'] === 'VARIABLE') {
         document.getElementById('variableObj').style.display = 'inline';
         document.getElementById('arrayRecordObj').style.display = 'none';
 
-        document.getElementById('varName').textContent = obj['name'];
-        document.getElementById('varDataType').textContent = obj['data_type'];
-        document.getElementById('varAccessType').textContent = obj['access_type'];
-        document.getElementById('varValue').textContent = obj['value'];
+        document.getElementById('varName').textContent = obj.name;
+        document.getElementById('varDataType').textContent = obj.data_type;
+        document.getElementById('varAccessType').textContent = obj.access_type;
+        document.getElementById('varValue').textContent = obj.value;
 
-        if (obj['access_type'] === 'ro' || obj['access_type'] === 'const') {
+        if (obj.access_type === 'ro' || obj.access_type === 'const') {
           document.getElementById('varNewValueInput').style.display = 'none';
         } else {
           document.getElementById('varNewValueInput').style.display = 'inline';
         }
       } else {
         document.getElementById('variableObj').style.display = 'none';
         document.getElementById('arrayRecordObj').style.display = 'inline';
 
-        document.getElementById('objType').textContent = obj['object_type'];
-        document.getElementById('objName').textContent = obj['name'];
-        document.getElementById('objSubindexes').textContent = obj['subindexes'];
+        document.getElementById('objType').textContent = obj.object_type;
+        document.getElementById('objName').textContent = obj.name;
+        document.getElementById('objSubindexes').textContent = Object.keys(obj.subindexes).length;
       }
     }
 
     function getObjectInfo() {
       updateData();
     }
```

### Comparing `oresat-olaf-1.0.0/olaf/_internals/rest_api/templates/os_command.html` & `oresat-olaf-2.0.0/olaf/_internals/rest_api/templates/os_command.html`

 * *Files 3% similar despite different names*

```diff
@@ -6,37 +6,37 @@
       justify-content: center;
       display: flex;
     }
     #abc {
       width: 50%;
       text-align: left;
     }
-    a, label {
+    label, .boldText {
       font-weight: bold;
     }
     #command {
-      width: 95%;
+      width: 94%;
     }
     textarea {
       resize: none;
       width: 100%;
     }
   </style>
   <div id='page'>
     <div id='abc'>
-      <a>Status: </a><span id='status'></span>
+      <a class='boldText'>Status: </a><span id='status'></span>
       <br/>
       <br/>
       <label for='command'>Bash Command:</label>
       <br/>
       <input type='text' id='command' name='command'/>
       <button onclick='runCommand()'>Run</button>
       <br/>
       <br/>
-      <a>Reply:</a>
+      <a class='boldText'>Reply:</a>
       <br/>
       <textarea id='reply' rows=30 disabled></textarea>
     </div>
   </div>
   <script>
     const states = {
         0: 'NO_ERROR_NO_REPLY',
@@ -64,15 +64,15 @@
       const statusObj = await readValue('0x1023', '0x02');
       const status = document.getElementById('status');
       const newStatus = states[statusObj['value']];
 
       // state has change to a new state with a reply, display reply
       if (status.textContent === 'EXECUTING' && reply_states.includes(newStatus)) {
         const replyObj = await readValue('0x1023', '0x03');
-        document.getElementById('reply').value = atob(replyObj['value']);
+        document.getElementById('reply').value = atob(replyObj.value);
       }
 
       status.textContent = newStatus;
     }
 
     runCommand();
     updateStatus();
```

### Comparing `oresat-olaf-1.0.0/olaf/_internals/rest_api/templates/system_info.html` & `oresat-olaf-2.0.0/olaf/_internals/rest_api/templates/system_info.html`

 * *Files 13% similar despite different names*

```diff
@@ -108,52 +108,53 @@
       <td><span id='rootPartTotal'></span> MB</td>
     </tr>
     <tr>
       <td>Root Partition Free</td>
       <td><span id='rootPartFree'></span> MB</td>
     </tr>
     <tr>
-        <td>Root Partition Percent</td>
-        <td><span id='rootPartPercent'></span> %</td>
-      </tr>
-    </table>
-  </div>
+      <td>Root Partition Percent</td>
+      <td><span id='rootPartPercent'></span> %</td>
+    </tr>
+  </table>
   <script>
-    const indexNames = {
-      '0x01': 'osName',
-      '0x02': 'osDistro',
-      '0x03': 'osKernelVersion',
-      '0x04': 'hostname',
-      '0x05': 'uptime',
-      '0x06': 'cpuNum',
-      '0x07': 'cpuArch',
-      '0x08': 'cpuGov',
-      '0x09': 'cpuFreq',
-      '0x0A': 'remoteProcNum',
-      '0x0E': 'load1Min',
-      '0x0F': 'load5Min',
-      '0x10': 'load15Min',
-      '0x11': 'ramTotal',
-      '0x12': 'ramFree',
-      '0x13': 'ramShared',
-      '0x14': 'ramBuffered',
-      '0x15': 'ramPercent',
-      '0x16': 'swapTotal',
-      '0x17': 'swapFree',
-      '0x18': 'swapPercent',
-      '0x19': 'procs',
-      '0x1A': 'rootPartTotal',
-      '0x1B': 'rootPartFree',
-      '0x1C': 'rootPartPercent',
-    }
+    const subindexNames = {
+      0x01: 'osName',
+      0x02: 'osDistro',
+      0x03: 'osKernelVersion',
+      0x04: 'hostname',
+      0x05: 'uptime',
+      0x06: 'cpuNum',
+      0x07: 'cpuArch',
+      0x08: 'cpuGov',
+      0x09: 'cpuFreq',
+      0x0A: 'remoteProcNum',
+      0x0E: 'load1Min',
+      0x0F: 'load5Min',
+      0x10: 'load15Min',
+      0x11: 'ramTotal',
+      0x12: 'ramFree',
+      0x13: 'ramShared',
+      0x14: 'ramBuffered',
+      0x15: 'ramPercent',
+      0x16: 'swapTotal',
+      0x17: 'swapFree',
+      0x18: 'swapPercent',
+      0x19: 'procs',
+      0x1A: 'rootPartTotal',
+      0x1B: 'rootPartFree',
+      0x1C: 'rootPartPercent',
+    };
 
     async  function updateAll() {
-      for (const index in indexNames) {
-        const obj = await readValue('0x3001', index)
-        document.getElementById(indexNames[index]).textContent = obj['value'];
+      let tmp;
+      const obj = await readValue('0x3001', null);
+      for (const subindex in subindexNames) {
+        tmp = document.getElementById(subindexNames[subindex]);
+        tmp.textContent = obj.subindexes[subindex].value;
       }
     }
 
     updateAll();
 
     const interval = setInterval(function() {
       updateAll()
```

### Comparing `oresat-olaf-1.0.0/olaf/_internals/rest_api/templates/updater.html` & `oresat-olaf-2.0.0/olaf/_internals/rest_api/templates/updater.html`

 * *Files 1% similar despite different names*

```diff
@@ -33,25 +33,25 @@
       1: 'PRE_UPDATE_FAILED',
       2: 'UPDATE_FAILED',
       255: 'UPDATING',
     }
 
     async function updaterInfo() {
       const statusObj = await readValue('0x3100', '0x01');
-      const newState = STATES[statusObj['value']];
+      const newState = STATES[statusObj.value];
       document.getElementById('status').textContent = newState;
 
       const updatesObj = await readValue('0x3100', '0x02');
-      document.getElementById('updatesAvailable').textContent = updatesObj['value'];
+      document.getElementById('updatesAvailable').textContent = updatesObj.value;
 
       if (newState === 'UPDATING') {
         document.getElementById('startUpdateButton').disabled = true;
         document.getElementById('makeStatusFileButton').disabled = true;
       } else {
-        if (updatesObj['value'] === 0) {
+        if (updatesObj.value === 0) {
           document.getElementById('startUpdateButton').disabled = true;
           document.getElementById('makeStatusFileButton').disabled = false;
         } else {
           document.getElementById('startUpdateButton').disabled = false;
           document.getElementById('makeStatusFileButton').disabled = false;
         }
       }
```

### Comparing `oresat-olaf-1.0.0/olaf/_internals/updater.py` & `oresat-olaf-2.0.0/olaf/_internals/updater.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 defines the order instructions are ran in and how it is ran.'''
 
 INSTRUCTIONS = {
     'BASH_SCRIPT': 'bash',
     'DPKG_INSTALL': 'dpkg -i',
     'DPKG_REMOVE': 'dpkg -r',
     'DPKG_PURGE': 'dpkg -P',
-    'PIP_INSTALL': 'python -m pip install',
-    'PIP_UNINSTALL': 'python -m pip uninstall',
+    'PIP_INSTALL': 'python3 -m pip install',
+    'PIP_UNINSTALL': 'python3 -m pip uninstall',
 }
 '''All the valid instruction. Values are the commands.'''
 
 INSTRUCTIONS_WITH_FILES = [
     'BASH_SCRIPT',
     'DPKG_INSTALL',
     'PIP_INSTALL',
@@ -397,17 +397,23 @@
                 else:
                     logger.error(f'could not find {dpkg_status_file}')
 
         remove(olu_file)
 
         return olu_tar
 
+    def clear_cache(self):
+        '''Clear the update cache.'''
+
+        self._cache.clear()
+
     @property
     def has_dpkg(self) -> bool:
         '''bool: system has dpkg or not'''
+
         return self._has_dpkg
 
     @property
     def status(self) -> UpdaterState:
         '''UpdaterState: The current state.'''
 
         return self._state
```

### Comparing `oresat-olaf-1.0.0/olaf/common/ecss.py` & `oresat-olaf-2.0.0/olaf/common/ecss.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-1.0.0/olaf/common/oresat_file.py` & `oresat-olaf-2.0.0/olaf/common/oresat_file.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-1.0.0/olaf/common/oresat_file_cache.py` & `oresat-olaf-2.0.0/olaf/common/oresat_file_cache.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-1.0.0/olaf/scripts/file_transfer.py` & `oresat-olaf-2.0.0/olaf/scripts/file_transfer.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-1.0.0/olaf/scripts/new_eds.py` & `oresat-olaf-2.0.0/olaf/scripts/new_eds.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-1.0.0/olaf/scripts/os_command.py` & `oresat-olaf-2.0.0/olaf/scripts/os_command.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-1.0.0/olaf/scripts/system_info.py` & `oresat-olaf-2.0.0/olaf/scripts/system_info.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-1.0.0/oresat_olaf.egg-info/PKG-INFO` & `oresat-olaf-2.0.0/oresat_olaf.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oresat-olaf
-Version: 1.0.0
+Version: 2.0.0
 Summary: Application framework for all OreSat Linux boards
 Home-page: https://github.com/oresat/oresat-olaf
 Author: PSAS
 Author-email: oresat@pdx.edu
 Maintainer: PSAS
 Maintainer-email: oresat@pdx.edu
 License: GPL-3.0
```

### Comparing `oresat-olaf-1.0.0/oresat_olaf.egg-info/SOURCES.txt` & `oresat-olaf-2.0.0/oresat_olaf.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,55 @@
 LICENSE
 README.rst
 pyproject.toml
 setup.cfg
 olaf/__init__.py
 olaf/_internals/__init__.py
 olaf/_internals/app.py
+olaf/_internals/master_node.py
+olaf/_internals/node.py
 olaf/_internals/updater.py
 olaf/_internals/data/oresat_app.eds
 olaf/_internals/resources/__init__.py
 olaf/_internals/resources/ecss.py
 olaf/_internals/resources/file_caches.py
 olaf/_internals/resources/fread.py
 olaf/_internals/resources/fwrite.py
 olaf/_internals/resources/logs.py
 olaf/_internals/resources/os_command.py
+olaf/_internals/resources/power_control.py
+olaf/_internals/resources/store_eds.py
 olaf/_internals/resources/system_info.py
 olaf/_internals/resources/updater.py
 olaf/_internals/rest_api/__init__.py
-olaf/_internals/rest_api/blueprints.py
 olaf/_internals/rest_api/static/favicon.ico
 olaf/_internals/rest_api/templates/base.html
 olaf/_internals/rest_api/templates/fread.html
 olaf/_internals/rest_api/templates/fwrite.html
+olaf/_internals/rest_api/templates/logs.html
 olaf/_internals/rest_api/templates/od.html
 olaf/_internals/rest_api/templates/os_command.html
+olaf/_internals/rest_api/templates/power_control.html
 olaf/_internals/rest_api/templates/root.html
 olaf/_internals/rest_api/templates/system_info.html
 olaf/_internals/rest_api/templates/updater.html
 olaf/common/__init__.py
+olaf/common/cpufreq.py
 olaf/common/ecss.py
+olaf/common/gpio.py
 olaf/common/oresat_file.py
 olaf/common/oresat_file_cache.py
 olaf/common/resource.py
 olaf/common/timer_loop.py
 olaf/scripts/__init__.py
 olaf/scripts/file_transfer.py
 olaf/scripts/new_eds.py
 olaf/scripts/os_command.py
 olaf/scripts/sdo_transfer.py
+olaf/scripts/sync.py
 olaf/scripts/system_info.py
 oresat_olaf.egg-info/PKG-INFO
 oresat_olaf.egg-info/SOURCES.txt
 oresat_olaf.egg-info/dependency_links.txt
 oresat_olaf.egg-info/entry_points.txt
 oresat_olaf.egg-info/requires.txt
 oresat_olaf.egg-info/top_level.txt
```

### Comparing `oresat-olaf-1.0.0/setup.cfg` & `oresat-olaf-2.0.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -44,12 +44,13 @@
 [options.entry_points]
 console_scripts = 
 	olaf-sdo-transfer = olaf.scripts.sdo_transfer:main
 	olaf-file-transfer = olaf.scripts.file_transfer:main
 	olaf-os-command = olaf.scripts.os_command:main
 	olaf-system-info = olaf.scripts.system_info:main
 	olaf-new-eds = olaf.scripts.new_eds:main
+	olaf-sync = olaf.scripts.sync:main
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `oresat-olaf-1.0.0/tests/common/test_ecss.py` & `oresat-olaf-2.0.0/tests/common/test_ecss.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-1.0.0/tests/common/test_oresat_file.py` & `oresat-olaf-2.0.0/tests/common/test_oresat_file.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-1.0.0/tests/common/test_oresat_file_cache.py` & `oresat-olaf-2.0.0/tests/common/test_oresat_file_cache.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-1.0.0/tests/internals/resources/test_fwrite.py` & `oresat-olaf-2.0.0/tests/internals/resources/test_fwrite.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,57 +7,61 @@
 from olaf import new_oresat_file
 from olaf._internals.resources.fwrite import FwriteResource, Subindex
 
 from . import MockApp
 
 
 class TestFwriteResource(unittest.TestCase):
+
     def setUp(self):
+
         self.app = MockApp()
-        self.node = self.app.node
-        self.app.add_resource(FwriteResource)
+        self.app.add_resource(FwriteResource())
         self.app.start()
-        self.fwrite_sdo = self.node.sdo[self.app.resource.index]
 
     def tearDown(self):
+
         self.app.stop()
 
     def test_write(self):
-        self.assertEqual(len(self.app.fwrite_cache), 0)
+
+        index = self.app.resource.index
+
+        self.assertEqual(len(self.app.node.fwrite_cache), 0)
 
         # add a file to the cache
         file_name = new_oresat_file('test')
         file_path = '/tmp/' + file_name
         file_data = ''.join(random.choice(string.ascii_letters) for i in range(100))
         with open(file_path, 'w') as f:
             f.write(file_data)
 
         # test sdo trasfer of a file
-        self.fwrite_sdo[Subindex.FILE_NAME.value].phys = basename(file_name)
-        self.assertEqual(self.fwrite_sdo[Subindex.FILE_NAME.value].phys, file_name)
-        self.fwrite_sdo[Subindex.FILE_DATA.value].phys = file_data.encode()
-        self.assertEqual(len(self.app.fwrite_cache), 1)
+        self.app.sdo_write(index, Subindex.FILE_NAME.value, basename(file_name))
+        self.assertEqual(self.app.sdo_read(index, Subindex.FILE_NAME.value), file_name)
+        self.app.sdo_write(index, Subindex.FILE_DATA.value, file_data.encode())
+        self.assertEqual(len(self.app.node.fwrite_cache), 1)
 
         # test sdo trasfer of a file to over write
-        self.fwrite_sdo[Subindex.FILE_NAME.value].phys = basename(file_name)
-        self.assertEqual(self.fwrite_sdo[Subindex.FILE_NAME.value].phys, file_name)
-        self.fwrite_sdo[Subindex.FILE_DATA.value].phys = file_data.encode()
-        self.assertEqual(len(self.app.fwrite_cache), 1)
+        self.app.sdo_write(index, Subindex.FILE_NAME.value, basename(file_name))
+        self.assertEqual(self.app.sdo_read(index, Subindex.FILE_NAME.value), file_name)
+        self.app.sdo_write(index, Subindex.FILE_DATA.value, file_data.encode())
+        self.assertEqual(len(self.app.node.fwrite_cache), 1)
 
         # remove test file
         remove(file_path)
 
         # add another file to the cache
         file_name = new_oresat_file('test2')
         file_path = '/tmp/' + file_name
         file_data = ''.join(random.choice(string.ascii_letters) for i in range(100))
         with open(file_path, 'w') as f:
             f.write(file_data)
 
         # test sdo trasfer of a file
-        self.fwrite_sdo[Subindex.FILE_NAME.value].phys = basename(file_name)
-        self.assertEqual(self.fwrite_sdo[Subindex.FILE_NAME.value].phys, file_name)
-        self.fwrite_sdo[Subindex.FILE_DATA.value].phys = file_data.encode()
-        self.assertEqual(len(self.app.fwrite_cache), 2)
+        self.app.sdo_write(index, Subindex.FILE_NAME.value, basename(file_name))
+        self.assertEqual(self.app.sdo_read(index, Subindex.FILE_NAME.value), file_name)
+        self.app.sdo_write(index, Subindex.FILE_DATA.value, file_data.encode())
+        self.assertEqual(len(self.app.node.fwrite_cache), 2)
 
         # remove test file
         remove(file_path)
```

### Comparing `oresat-olaf-1.0.0/tests/internals/updater/test_updater.py` & `oresat-olaf-2.0.0/tests/internals/updater/test_updater.py`

 * *Files identical despite different names*

