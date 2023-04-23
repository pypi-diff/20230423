# Comparing `tmp/ccpem_utils-0.0.1.dev8.tar.gz` & `tmp/ccpem_utils-0.0.1.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccpem_utils-0.0.1.dev8.tar", last modified: Thu Jan 19 21:00:16 2023, max compression
+gzip compressed data, was "ccpem_utils-0.0.1.dev9.tar", last modified: Sun Apr 23 08:51:02 2023, max compression
```

## Comparing `ccpem_utils-0.0.1.dev8.tar` & `ccpem_utils-0.0.1.dev9.tar`

### file list

```diff
@@ -1,56 +1,58 @@
-drwxr-xr-x   0 agnel      (501) staff       (20)        0 2023-01-19 21:00:16.720871 ccpem_utils-0.0.1.dev8/
--rw-r--r--   0 agnel      (501) staff       (20)        0 2022-12-05 12:36:33.000000 ccpem_utils-0.0.1.dev8/LICENSE
--rw-r--r--   0 agnel      (501) staff       (20)       37 2022-12-05 12:36:33.000000 ccpem_utils-0.0.1.dev8/MANIFEST.in
--rw-r--r--   0 agnel      (501) staff       (20)      592 2023-01-19 21:00:16.721360 ccpem_utils-0.0.1.dev8/PKG-INFO
--rw-r--r--   0 agnel      (501) staff       (20)      289 2022-12-05 15:28:21.000000 ccpem_utils-0.0.1.dev8/README.md
-drwxr-xr-x   0 agnel      (501) staff       (20)        0 2023-01-19 21:00:16.509414 ccpem_utils-0.0.1.dev8/ccpem_pyutils/
--rw-r--r--   0 agnel      (501) staff       (20)        0 2022-12-01 11:34:02.000000 ccpem_utils-0.0.1.dev8/ccpem_pyutils/__init__.py
-drwxr-xr-x   0 agnel      (501) staff       (20)        0 2023-01-19 21:00:16.510036 ccpem_utils-0.0.1.dev8/ccpem_pyutils/image/
--rw-r--r--   0 agnel      (501) staff       (20)        0 2022-12-01 11:34:02.000000 ccpem_utils-0.0.1.dev8/ccpem_pyutils/image/__init__.py
-drwxr-xr-x   0 agnel      (501) staff       (20)        0 2023-01-19 21:00:16.513531 ccpem_utils-0.0.1.dev8/ccpem_pyutils/map/
--rw-r--r--   0 agnel      (501) staff       (20)        0 2022-12-05 12:36:33.000000 ccpem_utils-0.0.1.dev8/ccpem_pyutils/map/__init__.py
--rw-r--r--   0 agnel      (501) staff       (20)    34249 2022-12-01 11:34:02.000000 ccpem_utils-0.0.1.dev8/ccpem_pyutils/map/array_utils.py
--rw-r--r--   0 agnel      (501) staff       (20)     1306 2022-12-01 11:34:02.000000 ccpem_utils-0.0.1.dev8/ccpem_pyutils/map/mrc_map_utils.py
--rw-r--r--   0 agnel      (501) staff       (20)    15062 2022-12-01 11:34:02.000000 ccpem_utils-0.0.1.dev8/ccpem_pyutils/map/parse_mrcmapobj.py
-drwxr-xr-x   0 agnel      (501) staff       (20)        0 2023-01-19 21:00:16.517845 ccpem_utils-0.0.1.dev8/ccpem_pyutils/model/
--rw-r--r--   0 agnel      (501) staff       (20)        0 2022-12-05 12:36:33.000000 ccpem_utils-0.0.1.dev8/ccpem_pyutils/model/__init__.py
--rw-r--r--   0 agnel      (501) staff       (20)     6818 2022-12-07 13:44:39.000000 ccpem_utils-0.0.1.dev8/ccpem_pyutils/model/coord_grid.py
--rw-r--r--   0 agnel      (501) staff       (20)    29502 2023-01-18 16:08:48.000000 ccpem_utils-0.0.1.dev8/ccpem_pyutils/model/gemmi_model_utils.py
--rw-r--r--   0 agnel      (501) staff       (20)    10602 2023-01-18 14:40:54.000000 ccpem_utils-0.0.1.dev8/ccpem_pyutils/model/model_utils.py
-drwxr-xr-x   0 agnel      (501) staff       (20)        0 2023-01-19 21:00:16.529389 ccpem_utils-0.0.1.dev8/ccpem_pyutils/other/
--rw-r--r--   0 agnel      (501) staff       (20)        0 2022-12-05 12:36:33.000000 ccpem_utils-0.0.1.dev8/ccpem_pyutils/other/__init__.py
--rw-r--r--   0 agnel      (501) staff       (20)     4427 2022-12-16 13:57:10.000000 ccpem_utils-0.0.1.dev8/ccpem_pyutils/other/calc.py
--rw-r--r--   0 agnel      (501) staff       (20)     4140 2022-12-22 20:11:01.000000 ccpem_utils-0.0.1.dev8/ccpem_pyutils/other/cluster.py
--rw-r--r--   0 agnel      (501) staff       (20)     1016 2022-12-08 22:28:38.000000 ccpem_utils-0.0.1.dev8/ccpem_pyutils/other/json_utils.py
--rw-r--r--   0 agnel      (501) staff       (20)      106 2023-01-05 15:49:26.000000 ccpem_utils-0.0.1.dev8/ccpem_pyutils/other/utils.py
-drwxr-xr-x   0 agnel      (501) staff       (20)        0 2023-01-19 21:00:16.534469 ccpem_utils-0.0.1.dev8/ccpem_pyutils/scripts/
--rw-r--r--   0 agnel      (501) staff       (20)        0 2022-12-12 15:45:59.000000 ccpem_utils-0.0.1.dev8/ccpem_pyutils/scripts/__init__.py
--rw-r--r--   0 agnel      (501) staff       (20)     3624 2023-01-17 13:57:12.000000 ccpem_utils-0.0.1.dev8/ccpem_pyutils/scripts/analyse_bfactors.py
--rw-r--r--   0 agnel      (501) staff       (20)      914 2022-12-01 11:34:02.000000 ccpem_utils-0.0.1.dev8/ccpem_pyutils/scripts/get_contacts.py
--rw-r--r--   0 agnel      (501) staff       (20)     2427 2022-12-05 14:13:01.000000 ccpem_utils-0.0.1.dev8/ccpem_pyutils/scripts/get_map_parameters.py
--rw-r--r--   0 agnel      (501) staff       (20)     2455 2022-12-01 11:34:02.000000 ccpem_utils-0.0.1.dev8/ccpem_pyutils/scripts/set_sigf_fom_columns.py
--rw-r--r--   0 agnel      (501) staff       (20)     1809 2022-12-07 13:55:53.000000 ccpem_utils-0.0.1.dev8/ccpem_pyutils/scripts/shift_map_model_origin_zero.py
-drwxr-xr-x   0 agnel      (501) staff       (20)        0 2023-01-19 21:00:16.535487 ccpem_utils-0.0.1.dev8/ccpem_pyutils/sequence/
--rw-r--r--   0 agnel      (501) staff       (20)        0 2022-12-01 11:34:02.000000 ccpem_utils-0.0.1.dev8/ccpem_pyutils/sequence/__init__.py
-drwxr-xr-x   0 agnel      (501) staff       (20)        0 2023-01-19 21:00:16.546093 ccpem_utils-0.0.1.dev8/ccpem_utils.egg-info/
--rw-r--r--   0 agnel      (501) staff       (20)      592 2023-01-19 21:00:16.000000 ccpem_utils-0.0.1.dev8/ccpem_utils.egg-info/PKG-INFO
--rw-r--r--   0 agnel      (501) staff       (20)     1375 2023-01-19 21:00:16.000000 ccpem_utils-0.0.1.dev8/ccpem_utils.egg-info/SOURCES.txt
--rw-r--r--   0 agnel      (501) staff       (20)        1 2023-01-19 21:00:16.000000 ccpem_utils-0.0.1.dev8/ccpem_utils.egg-info/dependency_links.txt
--rw-r--r--   0 agnel      (501) staff       (20)       68 2023-01-19 21:00:16.000000 ccpem_utils-0.0.1.dev8/ccpem_utils.egg-info/requires.txt
--rw-r--r--   0 agnel      (501) staff       (20)       38 2023-01-19 21:00:16.000000 ccpem_utils-0.0.1.dev8/ccpem_utils.egg-info/top_level.txt
-drwxr-xr-x   0 agnel      (501) staff       (20)        0 2023-01-19 21:00:16.558652 ccpem_utils-0.0.1.dev8/ccpem_utils_tests/
--rw-r--r--   0 agnel      (501) staff       (20)        0 2022-12-05 12:36:33.000000 ccpem_utils-0.0.1.dev8/ccpem_utils_tests/__init__.py
--rw-r--r--   0 agnel      (501) staff       (20)     5353 2022-12-16 13:56:57.000000 ccpem_utils-0.0.1.dev8/ccpem_utils_tests/test_cluster.py
--rw-r--r--   0 agnel      (501) staff       (20)     3869 2022-12-07 13:58:14.000000 ccpem_utils-0.0.1.dev8/ccpem_utils_tests/test_coord_grid.py
-drwxr-xr-x   0 agnel      (501) staff       (20)        0 2023-01-19 21:00:16.576419 ccpem_utils-0.0.1.dev8/ccpem_utils_tests/test_data/
--rw-r--r--   0 agnel      (501) staff       (20)   404838 2022-12-05 12:36:33.000000 ccpem_utils-0.0.1.dev8/ccpem_utils_tests/test_data/5me2.pdb
--rw-r--r--   0 agnel      (501) staff       (20)        0 2022-12-05 12:36:33.000000 ccpem_utils-0.0.1.dev8/ccpem_utils_tests/test_data/__init__.py
--rw-r--r--   0 agnel      (501) staff       (20)  4001024 2022-12-05 12:36:33.000000 ccpem_utils-0.0.1.dev8/ccpem_utils_tests/test_data/emd_3488.mrc
--rw-r--r--   0 agnel      (501) staff       (20)     3306 2022-12-12 10:23:12.000000 ccpem_utils-0.0.1.dev8/ccpem_utils_tests/test_gemmi_model_utils.py
--rw-r--r--   0 agnel      (501) staff       (20)     6013 2022-12-05 12:36:33.000000 ccpem_utils-0.0.1.dev8/ccpem_utils_tests/test_map_parse.py
--rw-r--r--   0 agnel      (501) staff       (20)     1719 2022-12-05 12:36:33.000000 ccpem_utils-0.0.1.dev8/ccpem_utils_tests/test_mrc_map_utils.py
--rw-r--r--   0 agnel      (501) staff       (20)      499 2022-12-05 12:36:33.000000 ccpem_utils-0.0.1.dev8/pyproject.toml
--rw-r--r--   0 agnel      (501) staff       (20)      550 2023-01-19 21:00:16.722833 ccpem_utils-0.0.1.dev8/setup.cfg
--rw-r--r--   0 agnel      (501) staff       (20)       92 2022-12-01 11:34:02.000000 ccpem_utils-0.0.1.dev8/setup.py
-drwxr-xr-x   0 agnel      (501) staff       (20)        0 2023-01-19 21:00:16.720487 ccpem_utils-0.0.1.dev8/tests/
--rw-r--r--   0 agnel      (501) staff       (20)        0 2022-12-05 12:36:33.000000 ccpem_utils-0.0.1.dev8/tests/__init__.py
+drwxr-xr-x   0 agnel      (501) staff       (20)        0 2023-04-23 08:51:02.480047 ccpem_utils-0.0.1.dev9/
+-rw-r--r--   0 agnel      (501) staff       (20)        0 2022-12-05 12:36:33.000000 ccpem_utils-0.0.1.dev9/LICENSE
+-rw-r--r--   0 agnel      (501) staff       (20)       37 2022-12-05 12:36:33.000000 ccpem_utils-0.0.1.dev9/MANIFEST.in
+-rw-r--r--   0 agnel      (501) staff       (20)      592 2023-04-23 08:51:02.480289 ccpem_utils-0.0.1.dev9/PKG-INFO
+-rw-r--r--   0 agnel      (501) staff       (20)      289 2022-12-05 15:28:21.000000 ccpem_utils-0.0.1.dev9/README.md
+drwxr-xr-x   0 agnel      (501) staff       (20)        0 2023-04-23 08:51:02.427222 ccpem_utils-0.0.1.dev9/ccpem_utils/
+-rw-r--r--   0 agnel      (501) staff       (20)        0 2023-04-22 22:57:13.000000 ccpem_utils-0.0.1.dev9/ccpem_utils/__init__.py
+drwxr-xr-x   0 agnel      (501) staff       (20)        0 2023-04-23 08:51:02.431243 ccpem_utils-0.0.1.dev9/ccpem_utils/image/
+-rw-r--r--   0 agnel      (501) staff       (20)        0 2023-04-22 22:57:13.000000 ccpem_utils-0.0.1.dev9/ccpem_utils/image/__init__.py
+drwxr-xr-x   0 agnel      (501) staff       (20)        0 2023-04-23 08:51:02.435278 ccpem_utils-0.0.1.dev9/ccpem_utils/map/
+-rw-r--r--   0 agnel      (501) staff       (20)        0 2023-04-22 22:57:13.000000 ccpem_utils-0.0.1.dev9/ccpem_utils/map/__init__.py
+-rw-r--r--   0 agnel      (501) staff       (20)    34249 2023-04-22 22:57:13.000000 ccpem_utils-0.0.1.dev9/ccpem_utils/map/array_utils.py
+-rw-r--r--   0 agnel      (501) staff       (20)     8708 2023-04-23 06:38:51.000000 ccpem_utils-0.0.1.dev9/ccpem_utils/map/mrc_map_utils.py
+-rw-r--r--   0 agnel      (501) staff       (20)     2672 2023-04-22 22:57:13.000000 ccpem_utils-0.0.1.dev9/ccpem_utils/map/mrcfile_utils.py
+-rw-r--r--   0 agnel      (501) staff       (20)    11354 2023-04-22 22:57:13.000000 ccpem_utils-0.0.1.dev9/ccpem_utils/map/parse_mrcmapobj.py
+drwxr-xr-x   0 agnel      (501) staff       (20)        0 2023-04-23 08:51:02.440368 ccpem_utils-0.0.1.dev9/ccpem_utils/model/
+-rw-r--r--   0 agnel      (501) staff       (20)        0 2023-04-22 22:57:13.000000 ccpem_utils-0.0.1.dev9/ccpem_utils/model/__init__.py
+-rw-r--r--   0 agnel      (501) staff       (20)     9267 2023-04-23 06:38:51.000000 ccpem_utils-0.0.1.dev9/ccpem_utils/model/coord_grid.py
+-rw-r--r--   0 agnel      (501) staff       (20)    29502 2023-04-23 06:38:51.000000 ccpem_utils-0.0.1.dev9/ccpem_utils/model/gemmi_model_utils.py
+-rw-r--r--   0 agnel      (501) staff       (20)    10602 2023-04-22 22:57:13.000000 ccpem_utils-0.0.1.dev9/ccpem_utils/model/model_utils.py
+drwxr-xr-x   0 agnel      (501) staff       (20)        0 2023-04-23 08:51:02.443744 ccpem_utils-0.0.1.dev9/ccpem_utils/other/
+-rw-r--r--   0 agnel      (501) staff       (20)        0 2023-04-22 22:57:13.000000 ccpem_utils-0.0.1.dev9/ccpem_utils/other/__init__.py
+-rw-r--r--   0 agnel      (501) staff       (20)     4427 2023-04-22 22:57:13.000000 ccpem_utils-0.0.1.dev9/ccpem_utils/other/calc.py
+-rw-r--r--   0 agnel      (501) staff       (20)     4140 2023-04-22 22:57:13.000000 ccpem_utils-0.0.1.dev9/ccpem_utils/other/cluster.py
+-rw-r--r--   0 agnel      (501) staff       (20)     1016 2023-04-22 22:57:13.000000 ccpem_utils-0.0.1.dev9/ccpem_utils/other/json_utils.py
+-rw-r--r--   0 agnel      (501) staff       (20)      106 2023-04-22 22:57:13.000000 ccpem_utils-0.0.1.dev9/ccpem_utils/other/utils.py
+drwxr-xr-x   0 agnel      (501) staff       (20)        0 2023-04-23 08:51:02.448069 ccpem_utils-0.0.1.dev9/ccpem_utils/scripts/
+-rw-r--r--   0 agnel      (501) staff       (20)        0 2023-04-22 22:57:13.000000 ccpem_utils-0.0.1.dev9/ccpem_utils/scripts/__init__.py
+-rw-r--r--   0 agnel      (501) staff       (20)     3622 2023-04-22 22:57:13.000000 ccpem_utils-0.0.1.dev9/ccpem_utils/scripts/analyse_bfactors.py
+-rw-r--r--   0 agnel      (501) staff       (20)      912 2023-04-22 22:57:13.000000 ccpem_utils-0.0.1.dev9/ccpem_utils/scripts/get_contacts.py
+-rw-r--r--   0 agnel      (501) staff       (20)     2427 2023-04-22 22:57:13.000000 ccpem_utils-0.0.1.dev9/ccpem_utils/scripts/get_map_parameters.py
+-rw-r--r--   0 agnel      (501) staff       (20)     2455 2023-04-22 22:57:13.000000 ccpem_utils-0.0.1.dev9/ccpem_utils/scripts/set_sigf_fom_columns.py
+-rw-r--r--   0 agnel      (501) staff       (20)     1805 2023-04-22 22:57:13.000000 ccpem_utils-0.0.1.dev9/ccpem_utils/scripts/shift_map_model_origin_zero.py
+drwxr-xr-x   0 agnel      (501) staff       (20)        0 2023-04-23 08:51:02.448943 ccpem_utils-0.0.1.dev9/ccpem_utils/sequence/
+-rw-r--r--   0 agnel      (501) staff       (20)        0 2023-04-22 22:57:13.000000 ccpem_utils-0.0.1.dev9/ccpem_utils/sequence/__init__.py
+drwxr-xr-x   0 agnel      (501) staff       (20)        0 2023-04-23 08:51:02.430541 ccpem_utils-0.0.1.dev9/ccpem_utils.egg-info/
+-rw-r--r--   0 agnel      (501) staff       (20)      592 2023-04-23 08:51:02.000000 ccpem_utils-0.0.1.dev9/ccpem_utils.egg-info/PKG-INFO
+-rw-r--r--   0 agnel      (501) staff       (20)     1404 2023-04-23 08:51:02.000000 ccpem_utils-0.0.1.dev9/ccpem_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 agnel      (501) staff       (20)        1 2023-04-23 08:51:02.000000 ccpem_utils-0.0.1.dev9/ccpem_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 agnel      (501) staff       (20)       68 2023-04-23 08:51:02.000000 ccpem_utils-0.0.1.dev9/ccpem_utils.egg-info/requires.txt
+-rw-r--r--   0 agnel      (501) staff       (20)       36 2023-04-23 08:51:02.000000 ccpem_utils-0.0.1.dev9/ccpem_utils.egg-info/top_level.txt
+drwxr-xr-x   0 agnel      (501) staff       (20)        0 2023-04-23 08:51:02.457453 ccpem_utils-0.0.1.dev9/ccpem_utils_tests/
+-rw-r--r--   0 agnel      (501) staff       (20)        0 2022-12-05 12:36:33.000000 ccpem_utils-0.0.1.dev9/ccpem_utils_tests/__init__.py
+-rw-r--r--   0 agnel      (501) staff       (20)     5349 2023-04-22 22:57:13.000000 ccpem_utils-0.0.1.dev9/ccpem_utils_tests/test_cluster.py
+-rw-r--r--   0 agnel      (501) staff       (20)     3906 2023-04-23 06:38:51.000000 ccpem_utils-0.0.1.dev9/ccpem_utils_tests/test_coord_grid.py
+drwxr-xr-x   0 agnel      (501) staff       (20)        0 2023-04-23 08:51:02.460808 ccpem_utils-0.0.1.dev9/ccpem_utils_tests/test_data/
+-rw-r--r--   0 agnel      (501) staff       (20)   404838 2022-12-05 12:36:33.000000 ccpem_utils-0.0.1.dev9/ccpem_utils_tests/test_data/5me2.pdb
+-rw-r--r--   0 agnel      (501) staff       (20)        0 2022-12-05 12:36:33.000000 ccpem_utils-0.0.1.dev9/ccpem_utils_tests/test_data/__init__.py
+-rw-r--r--   0 agnel      (501) staff       (20)  4001024 2022-12-05 12:36:33.000000 ccpem_utils-0.0.1.dev9/ccpem_utils_tests/test_data/emd_3488.mrc
+-rw-r--r--   0 agnel      (501) staff       (20)     3302 2023-04-22 22:57:13.000000 ccpem_utils-0.0.1.dev9/ccpem_utils_tests/test_gemmi_model_utils.py
+-rw-r--r--   0 agnel      (501) staff       (20)     3596 2023-04-23 08:47:15.000000 ccpem_utils-0.0.1.dev9/ccpem_utils_tests/test_map_parse.py
+-rw-r--r--   0 agnel      (501) staff       (20)     6212 2023-04-22 22:57:13.000000 ccpem_utils-0.0.1.dev9/ccpem_utils_tests/test_mrc_map_utils.py
+-rw-r--r--   0 agnel      (501) staff       (20)     3072 2023-04-22 22:57:13.000000 ccpem_utils-0.0.1.dev9/ccpem_utils_tests/test_mrcfile_utils.py
+-rw-r--r--   0 agnel      (501) staff       (20)      499 2022-12-05 12:36:33.000000 ccpem_utils-0.0.1.dev9/pyproject.toml
+-rw-r--r--   0 agnel      (501) staff       (20)      550 2023-04-23 08:51:02.481913 ccpem_utils-0.0.1.dev9/setup.cfg
+-rw-r--r--   0 agnel      (501) staff       (20)       92 2022-12-01 11:34:02.000000 ccpem_utils-0.0.1.dev9/setup.py
+drwxr-xr-x   0 agnel      (501) staff       (20)        0 2023-04-23 08:51:02.479553 ccpem_utils-0.0.1.dev9/tests/
+-rw-r--r--   0 agnel      (501) staff       (20)        0 2022-12-05 12:36:33.000000 ccpem_utils-0.0.1.dev9/tests/__init__.py
```

### Comparing `ccpem_utils-0.0.1.dev8/PKG-INFO` & `ccpem_utils-0.0.1.dev9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccpem_utils
-Version: 0.0.1.dev8
+Version: 0.0.1.dev9
 Summary: "Python utils for EM data processing (dev version)"
 Home-page: https://gitlab.com/ccpem/ccpem-utils
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ccpem_utils-0.0.1.dev8/ccpem_pyutils/map/array_utils.py` & `ccpem_utils-0.0.1.dev9/ccpem_utils/map/array_utils.py`

 * *Files identical despite different names*

### Comparing `ccpem_utils-0.0.1.dev8/ccpem_pyutils/model/gemmi_model_utils.py` & `ccpem_utils-0.0.1.dev9/ccpem_utils/model/gemmi_model_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,15 +168,15 @@
                     self.dict_resnames[model.name][chain.name][
                         str(residue.seqid.num)
                     ] = residue.name
 
     def get_avgbfact_deviation(
         self,
         calc_dev: bool = True,
-        dist_dev: float = 5.0,
+        dist_dev: float = 3.0,
         save_obj: bool = False,
         out_json: str = None,
         skip_nonpoly: bool = True,
     ):
         """
         Get average atomic B-factors, and stdev of atomic B-factors
         around each residue in the model
```

### Comparing `ccpem_utils-0.0.1.dev8/ccpem_pyutils/model/model_utils.py` & `ccpem_utils-0.0.1.dev9/ccpem_utils/model/model_utils.py`

 * *Files identical despite different names*

### Comparing `ccpem_utils-0.0.1.dev8/ccpem_pyutils/other/calc.py` & `ccpem_utils-0.0.1.dev9/ccpem_utils/other/calc.py`

 * *Files identical despite different names*

### Comparing `ccpem_utils-0.0.1.dev8/ccpem_pyutils/other/cluster.py` & `ccpem_utils-0.0.1.dev9/ccpem_utils/other/cluster.py`

 * *Files identical despite different names*

### Comparing `ccpem_utils-0.0.1.dev8/ccpem_pyutils/other/json_utils.py` & `ccpem_utils-0.0.1.dev9/ccpem_utils/other/json_utils.py`

 * *Files identical despite different names*

### Comparing `ccpem_utils-0.0.1.dev8/ccpem_pyutils/scripts/analyse_bfactors.py` & `ccpem_utils-0.0.1.dev9/ccpem_utils/scripts/analyse_bfactors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import argparse
 import os
 import json
-from ccpem_pyutils.model.gemmi_model_utils import (
+from ccpem_utils.model.gemmi_model_utils import (
     GemmiModelUtils,
     set_bfactor_attributes,
 )
 
 
 def parse_args():
     parser = argparse.ArgumentParser(description="CCP-EM analyse B-factors")
```

### Comparing `ccpem_utils-0.0.1.dev8/ccpem_pyutils/scripts/get_contacts.py` & `ccpem_utils-0.0.1.dev9/ccpem_utils/scripts/get_contacts.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #
 #     This code is distributed under the terms and conditions of the
 #     CCP-EM Program Suite Licence Agreement as a CCP-EM Application.
 #     A copy of the CCP-EM licence can be obtained by writing to the
 #     CCP-EM Secretary, RAL Laboratory, Harwell, OX11 0FA, UK.
 
 import argparse
-from ccpem_pyutils.model import gemmi_model_utils
+from ccpem_utils.model import gemmi_model_utils
 
 
 def parse_args():
     parser = argparse.ArgumentParser(description="CCP-EM model tools")
     parser.add_argument(
         "-m",
         "--model",
```

### Comparing `ccpem_utils-0.0.1.dev8/ccpem_pyutils/scripts/get_map_parameters.py` & `ccpem_utils-0.0.1.dev9/ccpem_utils/scripts/get_map_parameters.py`

 * *Files identical despite different names*

### Comparing `ccpem_utils-0.0.1.dev8/ccpem_pyutils/scripts/set_sigf_fom_columns.py` & `ccpem_utils-0.0.1.dev9/ccpem_utils/scripts/set_sigf_fom_columns.py`

 * *Files identical despite different names*

### Comparing `ccpem_utils-0.0.1.dev8/ccpem_pyutils/scripts/shift_map_model_origin_zero.py` & `ccpem_utils-0.0.1.dev9/ccpem_utils/scripts/shift_map_model_origin_zero.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 #
 #     This code is distributed under the terms and conditions of the
 #     CCP-EM Program Suite Licence Agreement as a CCP-EM Application.
 #     A copy of the CCP-EM licence can be obtained by writing to the
 #     CCP-EM Secretary, RAL Laboratory, Harwell, OX11 0FA, UK.
 
 import argparse
-from ccpem_pyutils.model import gemmi_model_utils
-from ccpem_pyutils.map.parse_mrcmapobj import MapObjHandle
+from ccpem_utils.model import gemmi_model_utils
+from ccpem_utils.map.parse_mrcmapobj import MapObjHandle
 import mrcfile
 import os
 
 
 def parse_args():
     parser = argparse.ArgumentParser(description="CCP-EM model tools")
     parser.add_argument(
```

### Comparing `ccpem_utils-0.0.1.dev8/ccpem_utils.egg-info/PKG-INFO` & `ccpem_utils-0.0.1.dev9/ccpem_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccpem-utils
-Version: 0.0.1.dev8
+Version: 0.0.1.dev9
 Summary: "Python utils for EM data processing (dev version)"
 Home-page: https://gitlab.com/ccpem/ccpem-utils
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ccpem_utils-0.0.1.dev8/ccpem_utils_tests/test_cluster.py` & `ccpem_utils-0.0.1.dev9/ccpem_utils_tests/test_cluster.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 
 import unittest
 import os
 import tempfile
 import shutil
 from ccpem_utils_tests import test_data
 import numpy as np
-from ccpem_pyutils.model.gemmi_model_utils import (
+from ccpem_utils.model.gemmi_model_utils import (
     GemmiModelUtils,
     get_residue_attribute,
     set_bfactor_attributes,
 )
-from ccpem_pyutils.other.cluster import (
+from ccpem_utils.other.cluster import (
     cluster_coord_features,
     generate_kdtree,
     pairs_kdtree,
 )
 import datetime
```

### Comparing `ccpem_utils-0.0.1.dev8/ccpem_utils_tests/test_coord_grid.py` & `ccpem_utils-0.0.1.dev9/ccpem_utils_tests/test_coord_grid.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 
 import unittest
 import os
 import shutil
 import tempfile
 import numpy as np
 from ccpem_utils_tests import test_data
-from ccpem_pyutils.model.coord_grid import (
+from ccpem_utils.model.coord_grid import (
     set_map_grid,
     set_cubic_map_grid,
     mapGridPositions,
 )
-from ccpem_pyutils.map.parse_mrcmapobj import MapObjHandle
-from ccpem_pyutils.scripts import shift_map_model_origin_zero
+from ccpem_utils.map.parse_mrcmapobj import MapObjHandle
+from ccpem_utils.scripts import shift_map_model_origin_zero
 import mrcfile
 import subprocess
 
 
 class MapParseTests(unittest.TestCase):
     def setUp(self):
         """
@@ -68,14 +68,15 @@
         wrapped_mapobj.crop_map_grid(new_dim=(71, 73, 58))
         # write
         with mrcfile.new("emd_3488_cropped.mrc", overwrite=True) as mrc:
             wrapped_mapobj.update_newmap_data_header(mrc)
             list_grid_points = mapGridPositions(
                 wrapped_mapobj, atom_coord=(61.197, 39.327, 61.266), res_map=3.2
             )[:]
+        assert len(list_grid_points) == 22
         ox, oy, oz = wrapped_mapobj.origin
         wrapped_mapobj.close()
         model_input = os.path.join(self.test_data, "5me2.pdb")
         subprocess.call(
             [
                 "python3 "
                 + os.path.realpath(shift_map_model_origin_zero.__file__)
```

### Comparing `ccpem_utils-0.0.1.dev8/ccpem_utils_tests/test_data/5me2.pdb` & `ccpem_utils-0.0.1.dev9/ccpem_utils_tests/test_data/5me2.pdb`

 * *Files identical despite different names*

### Comparing `ccpem_utils-0.0.1.dev8/ccpem_utils_tests/test_data/emd_3488.mrc` & `ccpem_utils-0.0.1.dev9/ccpem_utils_tests/test_data/emd_3488.mrc`

 * *Files identical despite different names*

### Comparing `ccpem_utils-0.0.1.dev8/ccpem_utils_tests/test_gemmi_model_utils.py` & `ccpem_utils-0.0.1.dev9/ccpem_utils_tests/test_gemmi_model_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 
 import unittest
 import os
 import math
 import tempfile
 import shutil
 from ccpem_utils_tests import test_data
-from ccpem_pyutils.model.gemmi_model_utils import (
+from ccpem_utils.model.gemmi_model_utils import (
     GemmiModelUtils,
     set_bfactor_attributes,
 )
-from ccpem_pyutils.scripts import analyse_bfactors
+from ccpem_utils.scripts import analyse_bfactors
 import subprocess
 
 
 class GemmiModelUtilsTest(unittest.TestCase):
     def setUp(self):
         """
         Setup test data and output directories.
```

### Comparing `ccpem_utils-0.0.1.dev8/ccpem_utils_tests/test_map_parse.py` & `ccpem_utils-0.0.1.dev9/ccpem_utils_tests/test_mrc_map_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,24 +5,29 @@
 #     CCP-EM Program Suite Licence Agreement as a CCP-EM Application.
 #     A copy of the CCP-EM licence can be obtained by writing to the
 #     CCP-EM Secretary, RAL Laboratory, Harwell, OX11 0FA, UK.
 #
 
 import unittest
 import os
-import shutil
 import tempfile
 import math
+import shutil
 from ccpem_utils_tests import test_data
 import subprocess
-from ccpem_pyutils.scripts import get_map_parameters
-from ccpem_pyutils.map.parse_mrcmapobj import MapObjHandle
-from ccpem_pyutils.model.coord_grid import mapGridPositions
-from ccpem_pyutils.other.calc import get_ccc
+from ccpem_utils.scripts import get_map_parameters
+from ccpem_utils.map.parse_mrcmapobj import MapObjHandle
+from ccpem_utils.map.mrc_map_utils import (
+    crop_map_grid,
+    pad_map_grid,
+    interpolate_to_grid,
+    downsample_apix,
+)
 import mrcfile
+from ccpem_utils.other.calc import get_ccc
 
 
 class MapParseTests(unittest.TestCase):
     def setUp(self):
         """
         Setup test data and output directories.
         """
@@ -30,62 +35,38 @@
         self.test_dir = tempfile.mkdtemp(prefix="map_parse")
         # Change to test directory
         self._orig_dir = os.getcwd()
         os.chdir(self.test_dir)
 
     def tearDown(self):
         os.chdir(self._orig_dir)
+        # print(self.test_dir)
         if os.path.exists(self.test_dir):
             shutil.rmtree(self.test_dir)
 
-    def test_map_parse(self):
-        # read
-        map_input = os.path.join(self.test_data, "emd_3488.mrc")
-        with mrcfile.open(map_input, mode="r", permissive=True) as mrc:
-            wrapped_mapobj = MapObjHandle(mrc)
-        # process
-        wrapped_mapobj.shift_origin((1.0, 1.0, 1.0))
-        with mrcfile.new("emd_3488_shifted.mrc", overwrite=True) as mrc:
-            wrapped_mapobj.update_newmap_data_header(mrc)
-        wrapped_mapobj.close()
-        # write
-        with mrcfile.open("emd_3488_shifted.mrc", mode="r") as mrc:
-            wrapped_mapobj = MapObjHandle(mrc)
-            assert wrapped_mapobj.origin == (1.0, 1.0, 1.0)
-
-    def test_map_fix_origin(self):
-        # read
-        map_input = os.path.join(self.test_data, "emd_3488.mrc")
-        with mrcfile.open(map_input, mode="r", permissive=True) as mrc:
-            wrapped_mapobj = MapObjHandle(mrc)
-        # process
-        wrapped_mapobj.shift_nstart((1, 1, 1))
-        wrapped_mapobj.fix_origin()
-        assert tuple([round(o, 5) for o in wrapped_mapobj.origin]) == (1.05, 1.05, 1.05)
-
     def test_map_crop(self):
         # read
         map_input = os.path.join(self.test_data, "emd_3488.mrc")
         with mrcfile.open(map_input, mode="r", permissive=True) as mrc:
             wrapped_mapobj = MapObjHandle(mrc)
         # copy
         wrapped_mapobj_copy = wrapped_mapobj.copy()
         # process1
-        wrapped_mapobj.crop_map_grid(new_dim=(71, 73, 58))
+        crop_map_grid(wrapped_mapobj, new_dim=(71, 73, 58))
         # write1
         with mrcfile.new("emd_3488_cropped1.mrc", overwrite=True) as mrc:
             wrapped_mapobj.update_newmap_data_header(mrc)
         wrapped_mapobj.close()
         # check1
         with mrcfile.open("emd_3488_cropped1.mrc", mode="r") as mrc:
             wrapped_mapobj1 = MapObjHandle(mrc)
             assert wrapped_mapobj1.data.shape == (58, 73, 71)
         # process2
-        wrapped_mapobj2 = wrapped_mapobj_copy.crop_map_grid(
-            contour=0.125, ext=3, inplace=False
+        wrapped_mapobj2 = crop_map_grid(
+            wrapped_mapobj_copy, contour=0.125, ext=3, inplace=False
         )
         # write
         with mrcfile.new("emd_3488_cropped2.mrc", overwrite=True) as mrc:
             wrapped_mapobj2.update_newmap_data_header(mrc)
         # check
         with mrcfile.open("emd_3488_cropped2.mrc", mode="r") as mrc:
             wrapped_mapobj2 = MapObjHandle(mrc)
@@ -93,51 +74,82 @@
         assert (
             get_ccc(
                 wrapped_mapobj1.data,
                 wrapped_mapobj2.data,
             )
             == 1.0
         )
-        wrapped_mapobj_copy.crop_map_grid(contour=0.125, ext=3, cubic=True)
+        crop_map_grid(wrapped_mapobj_copy, contour=0.125, ext=3, cubic=True)
         assert wrapped_mapobj_copy.data.shape == (73, 73, 73)
 
     def test_map_pad(self):
         # read
         map_input = os.path.join(self.test_data, "emd_3488.mrc")
         with mrcfile.open(map_input, mode="r", permissive=True) as mrc:
             wrapped_mapobj = MapObjHandle(mrc)
         # process
-        wrapped_mapobj.pad_map_grid(ext_dim=(10, 10, 10))
+        pad_map_grid(wrapped_mapobj, ext_dim=(10, 10, 10))
         min_map = wrapped_mapobj.data.min()
         # write
         with mrcfile.new("emd_3488_padded.mrc", overwrite=True) as mrc:
             wrapped_mapobj.update_newmap_data_header(mrc)
         wrapped_mapobj.close()
         # check1
         with mrcfile.open("emd_3488_padded.mrc", mode="r") as mrc:
             wrapped_mapobj = MapObjHandle(mrc)
             assert wrapped_mapobj.data.shape == (110, 110, 110)
         min_padded_map = wrapped_mapobj.data.min()
         assert min_map == min_padded_map  # padding filled with min
 
-    def test_map_coordinate_search(self):
+    def test_interpolate_downsample(self):
         map_input = os.path.join(self.test_data, "emd_3488.mrc")
         with mrcfile.open(map_input, mode="r", permissive=True) as mrc:
             wrapped_mapobj = MapObjHandle(mrc)
-            list_grid_points = mapGridPositions(
-                wrapped_mapobj, atom_coord=(61.197, 39.327, 61.266), res_map=3.2
+        # copy
+        wrapped_mapobj_copy = wrapped_mapobj.copy()
+        # interpolate
+        interpolate_to_grid(
+            wrapped_mapobj, (50, 50, 50), (2.1, 2.1, 2.1), (0.0, 0.0, 0.0)
+        )
+        # write
+        with mrcfile.new("emd_3488_interpolated.mrc", overwrite=True) as mrc:
+            wrapped_mapobj.update_newmap_data_header(mrc)
+        wrapped_mapobj.close()
+        # check1
+        with mrcfile.open("emd_3488_interpolated.mrc", mode="r") as mrc:
+            interpolated_mapobj = MapObjHandle(mrc)
+            assert interpolated_mapobj.data.shape == (50, 50, 50)
+            assert interpolated_mapobj.origin == (0.0, 0.0, 0.0)
+            assert math.isclose(
+                interpolated_mapobj.apix[0],
+                2.1,
+                rel_tol=0.00001,
             )
-            assert len(list_grid_points) == 27
-            list_grid_points = mapGridPositions(
-                wrapped_mapobj,
-                atom_coord=(61.197, 39.327, 61.266),
-                res_map=3.2,
-                gauss=False,
+        # downsample
+        downsample_apix(wrapped_mapobj_copy, (2.1, 2.1, 2.1))
+        # write
+        with mrcfile.new("emd_3488_downsampled.mrc", overwrite=True) as mrc:
+            wrapped_mapobj_copy.update_newmap_data_header(mrc)
+        # check2
+        with mrcfile.open("emd_3488_downsampled.mrc", mode="r") as mrc:
+            downsampled_mapobj = MapObjHandle(mrc)
+            assert downsampled_mapobj.data.shape == (50, 50, 50)
+            assert downsampled_mapobj.origin == (0.0, 0.0, 0.0)
+            assert math.isclose(
+                downsampled_mapobj.apix[0],
+                2.1,
+                rel_tol=0.00001,
             )
-            assert len(list_grid_points) == 1
+        assert (
+            get_ccc(
+                interpolated_mapobj.data,
+                downsampled_mapobj.data,
+            )
+            == 1.0
+        )
 
     def test_run_subprocess_get_map_parameters(self):
         map_input = os.path.join(self.test_data, "emd_3488.mrc")
         subprocess.call(
             [
                 "python3 "
                 + os.path.realpath(get_map_parameters.__file__)
```

