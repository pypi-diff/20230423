# Comparing `tmp/alaric-1.3.1.tar.gz` & `tmp/alaric-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alaric-1.3.1.tar", last modified: Mon Mar 27 04:02:59 2023, max compression
+gzip compressed data, was "alaric-1.3.2.tar", last modified: Sun Apr 23 07:15:09 2023, max compression
```

## Comparing `alaric-1.3.1.tar` & `alaric-1.3.2.tar`

### file list

```diff
@@ -1,58 +1,63 @@
-drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-03-27 04:02:59.864801 alaric-1.3.1/
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1662 2023-03-27 04:02:59.864801 alaric-1.3.1/PKG-INFO
-drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-03-27 04:02:59.856801 alaric-1.3.1/alaric/
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      599 2023-03-27 04:02:43.000000 alaric-1.3.1/alaric/__init__.py
-drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-03-27 04:02:59.860801 alaric-1.3.1/alaric/abc/
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      243 2022-06-27 05:34:52.000000 alaric-1.3.1/alaric/abc/__init__.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      248 2022-06-27 05:34:52.000000 alaric-1.3.1/alaric/abc/buildable.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      417 2022-06-01 19:52:25.000000 alaric-1.3.1/alaric/abc/comparison.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      301 2022-06-27 05:34:52.000000 alaric-1.3.1/alaric/abc/filterable.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      645 2022-06-01 19:52:25.000000 alaric-1.3.1/alaric/abc/logical.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      250 2022-06-27 05:34:52.000000 alaric-1.3.1/alaric/abc/saveable.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      899 2022-07-13 12:06:18.000000 alaric-1.3.1/alaric/advanced_query.py
-drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-03-27 04:02:59.860801 alaric-1.3.1/alaric/comparison/
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      247 2022-08-17 18:44:27.000000 alaric-1.3.1/alaric/comparison/__init__.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1247 2022-07-13 12:29:56.000000 alaric-1.3.1/alaric/comparison/comparison_eq.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      840 2022-08-17 18:44:27.000000 alaric-1.3.1/alaric/comparison/comparison_exists.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1097 2022-06-21 13:44:09.000000 alaric-1.3.1/alaric/comparison/comparison_greater_than.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1134 2022-07-13 07:58:10.000000 alaric-1.3.1/alaric/comparison/comparison_in.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1088 2022-06-21 13:44:09.000000 alaric-1.3.1/alaric/comparison/comparison_less_than.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)    10747 2023-03-11 04:36:14.000000 alaric-1.3.1/alaric/cursor.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)    17615 2023-03-11 04:36:14.000000 alaric-1.3.1/alaric/document.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)    18772 2023-03-11 04:36:14.000000 alaric-1.3.1/alaric/encrypted_document.py
-drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-03-27 04:02:59.864801 alaric-1.3.1/alaric/encryption/
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      281 2023-03-11 04:36:14.000000 alaric-1.3.1/alaric/encryption/__init__.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      891 2023-03-11 04:41:30.000000 alaric-1.3.1/alaric/encryption/automatic_hashed_fields.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      336 2023-03-11 04:36:14.000000 alaric-1.3.1/alaric/encryption/base.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      288 2023-03-11 04:36:14.000000 alaric-1.3.1/alaric/encryption/encrypted_fields.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      649 2023-03-11 04:36:14.000000 alaric-1.3.1/alaric/encryption/hashed_fields.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1021 2023-03-11 04:36:14.000000 alaric-1.3.1/alaric/encryption/hashed_query_field.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      132 2023-03-11 04:36:14.000000 alaric-1.3.1/alaric/encryption/ignore_fields.py
-drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-03-27 04:02:59.864801 alaric-1.3.1/alaric/logical/
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      117 2022-06-01 19:52:25.000000 alaric-1.3.1/alaric/logical/__init__.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1259 2022-08-23 15:35:35.000000 alaric-1.3.1/alaric/logical/logical_and.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1213 2022-08-23 15:35:35.000000 alaric-1.3.1/alaric/logical/logical_not.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1271 2022-08-23 15:35:47.000000 alaric-1.3.1/alaric/logical/logical_or.py
-drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-03-27 04:02:59.864801 alaric-1.3.1/alaric/meta/
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      103 2023-03-11 04:36:14.000000 alaric-1.3.1/alaric/meta/__init__.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      391 2023-03-11 04:36:14.000000 alaric-1.3.1/alaric/meta/all.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      211 2022-11-09 07:40:10.000000 alaric-1.3.1/alaric/meta/case_insensitive.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1962 2022-08-17 18:54:27.000000 alaric-1.3.1/alaric/meta/negate.py
-drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-03-27 04:02:59.864801 alaric-1.3.1/alaric/projections/
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      229 2022-08-17 18:47:02.000000 alaric-1.3.1/alaric/projections/__init__.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      326 2022-08-17 18:46:25.000000 alaric-1.3.1/alaric/projections/hide.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1066 2022-08-17 18:55:57.000000 alaric-1.3.1/alaric/projections/projections.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      326 2022-08-17 18:46:10.000000 alaric-1.3.1/alaric/projections/show.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      906 2023-03-11 04:36:14.000000 alaric-1.3.1/alaric/query_builder.py
-drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-03-27 04:02:59.864801 alaric-1.3.1/alaric/types/
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)       32 2022-07-13 07:52:24.000000 alaric-1.3.1/alaric/types/__init__.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      351 2022-07-13 07:54:13.000000 alaric-1.3.1/alaric/types/object_id.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      682 2023-03-11 04:40:45.000000 alaric-1.3.1/alaric/util.py
-drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-03-27 04:02:59.856801 alaric-1.3.1/alaric.egg-info/
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1662 2023-03-27 04:02:59.000000 alaric-1.3.1/alaric.egg-info/PKG-INFO
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1305 2023-03-27 04:02:59.000000 alaric-1.3.1/alaric.egg-info/SOURCES.txt
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)        1 2023-03-27 04:02:59.000000 alaric-1.3.1/alaric.egg-info/dependency_links.txt
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)       30 2023-03-27 04:02:59.000000 alaric-1.3.1/alaric.egg-info/requires.txt
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)        7 2023-03-27 04:02:59.000000 alaric-1.3.1/alaric.egg-info/top_level.txt
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)       38 2023-03-27 04:02:59.864801 alaric-1.3.1/setup.cfg
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1446 2022-06-21 13:44:09.000000 alaric-1.3.1/setup.py
+drwxr-xr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-04-23 07:15:09.564280 alaric-1.3.2/
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     1662 2023-04-23 07:15:09.564280 alaric-1.3.2/PKG-INFO
+drwxr-xr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-04-23 07:15:09.556280 alaric-1.3.2/alaric/
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)      599 2023-04-23 07:13:08.000000 alaric-1.3.2/alaric/__init__.py
+drwxr-xr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-04-23 07:15:09.560280 alaric-1.3.2/alaric/abc/
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)      243 2023-04-23 07:11:33.000000 alaric-1.3.2/alaric/abc/__init__.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)      248 2023-04-23 07:11:33.000000 alaric-1.3.2/alaric/abc/buildable.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)      417 2022-06-01 23:38:52.000000 alaric-1.3.2/alaric/abc/comparison.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)      301 2023-04-23 07:11:33.000000 alaric-1.3.2/alaric/abc/filterable.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)      645 2022-06-01 23:38:52.000000 alaric-1.3.2/alaric/abc/logical.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)      250 2023-04-23 07:11:33.000000 alaric-1.3.2/alaric/abc/saveable.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)      899 2023-04-23 07:11:33.000000 alaric-1.3.2/alaric/advanced_query.py
+drwxr-xr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-04-23 07:15:09.560280 alaric-1.3.2/alaric/comparison/
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)      247 2023-04-23 07:11:33.000000 alaric-1.3.2/alaric/comparison/__init__.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     1247 2023-04-23 07:11:33.000000 alaric-1.3.2/alaric/comparison/comparison_eq.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)      840 2023-04-23 07:11:33.000000 alaric-1.3.2/alaric/comparison/comparison_exists.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     1097 2023-04-23 07:11:33.000000 alaric-1.3.2/alaric/comparison/comparison_greater_than.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     1134 2023-04-23 07:11:33.000000 alaric-1.3.2/alaric/comparison/comparison_in.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     1088 2023-04-23 07:11:33.000000 alaric-1.3.2/alaric/comparison/comparison_less_than.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)    10747 2023-04-23 07:11:33.000000 alaric-1.3.2/alaric/cursor.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)    17615 2023-04-23 07:11:33.000000 alaric-1.3.2/alaric/document.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)    18772 2023-04-23 07:11:33.000000 alaric-1.3.2/alaric/encrypted_document.py
+drwxr-xr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-04-23 07:15:09.560280 alaric-1.3.2/alaric/encryption/
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)      281 2023-04-23 07:11:33.000000 alaric-1.3.2/alaric/encryption/__init__.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)      891 2023-04-23 07:11:33.000000 alaric-1.3.2/alaric/encryption/automatic_hashed_fields.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)      336 2023-04-23 07:11:33.000000 alaric-1.3.2/alaric/encryption/base.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)      288 2023-04-23 07:11:33.000000 alaric-1.3.2/alaric/encryption/encrypted_fields.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)      649 2023-04-23 07:11:33.000000 alaric-1.3.2/alaric/encryption/hashed_fields.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     1021 2023-04-23 07:11:33.000000 alaric-1.3.2/alaric/encryption/hashed_query_field.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)      132 2023-04-23 07:11:33.000000 alaric-1.3.2/alaric/encryption/ignore_fields.py
+drwxr-xr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-04-23 07:15:09.560280 alaric-1.3.2/alaric/logical/
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)      117 2022-06-01 23:38:52.000000 alaric-1.3.2/alaric/logical/__init__.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     1259 2023-04-23 07:11:33.000000 alaric-1.3.2/alaric/logical/logical_and.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     1213 2023-04-23 07:11:33.000000 alaric-1.3.2/alaric/logical/logical_not.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     1271 2023-04-23 07:11:33.000000 alaric-1.3.2/alaric/logical/logical_or.py
+drwxr-xr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-04-23 07:15:09.560280 alaric-1.3.2/alaric/meta/
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)      103 2023-04-23 07:11:33.000000 alaric-1.3.2/alaric/meta/__init__.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)      391 2023-04-23 07:11:33.000000 alaric-1.3.2/alaric/meta/all.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)      211 2022-06-01 23:38:52.000000 alaric-1.3.2/alaric/meta/case_insensitive.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     1962 2023-04-23 07:11:33.000000 alaric-1.3.2/alaric/meta/negate.py
+drwxr-xr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-04-23 07:15:09.564280 alaric-1.3.2/alaric/projections/
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)      229 2023-04-23 07:11:33.000000 alaric-1.3.2/alaric/projections/__init__.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)      326 2023-04-23 07:11:33.000000 alaric-1.3.2/alaric/projections/hide.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     1066 2023-04-23 07:11:33.000000 alaric-1.3.2/alaric/projections/projections.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)      326 2023-04-23 07:11:33.000000 alaric-1.3.2/alaric/projections/show.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)      906 2023-04-23 07:11:33.000000 alaric-1.3.2/alaric/query_builder.py
+drwxr-xr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-04-23 07:15:09.564280 alaric-1.3.2/alaric/types/
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)       32 2023-04-23 07:11:33.000000 alaric-1.3.2/alaric/types/__init__.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)      351 2023-04-23 07:11:33.000000 alaric-1.3.2/alaric/types/object_id.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)      682 2023-04-23 07:11:33.000000 alaric-1.3.2/alaric/util.py
+drwxr-xr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-04-23 07:15:09.560280 alaric-1.3.2/alaric.egg-info/
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     1662 2023-04-23 07:15:09.000000 alaric-1.3.2/alaric.egg-info/PKG-INFO
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     1401 2023-04-23 07:15:09.000000 alaric-1.3.2/alaric.egg-info/SOURCES.txt
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)        1 2023-04-23 07:15:09.000000 alaric-1.3.2/alaric.egg-info/dependency_links.txt
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)       30 2023-04-23 07:15:09.000000 alaric-1.3.2/alaric.egg-info/requires.txt
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)        7 2023-04-23 07:15:09.000000 alaric-1.3.2/alaric.egg-info/top_level.txt
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)       38 2023-04-23 07:15:09.564280 alaric-1.3.2/setup.cfg
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     1446 2023-04-23 07:12:58.000000 alaric-1.3.2/setup.py
+drwxr-xr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-04-23 07:15:09.564280 alaric-1.3.2/tests/
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)      234 2023-04-23 07:11:33.000000 alaric-1.3.2/tests/test_all.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     4342 2023-04-23 07:11:33.000000 alaric-1.3.2/tests/test_cursors.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     2950 2023-04-23 07:11:33.000000 alaric-1.3.2/tests/test_document.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     4339 2023-04-23 07:11:33.000000 alaric-1.3.2/tests/test_encrypted_document.py
```

### Comparing `alaric-1.3.1/PKG-INFO` & `alaric-1.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alaric
-Version: 1.3.1
+Version: 1.3.2
 Summary: A simplistic yet powerful asynchronous MongoDB query engine.
 Author: Skelmis
 Author-email: ethan@koldfusion.xyz
 Project-URL: Issue tracker, https://github.com/Skelmis/Alaric/issues
 Project-URL: Documentation, https://alaric.rtfd.io/
 Project-URL: Homepage, https://github.com/Skelmis/Alaric
 Classifier: Programming Language :: Python :: 3
```

### Comparing `alaric-1.3.1/alaric/__init__.py` & `alaric-1.3.2/alaric/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,11 +14,11 @@
     "Document",
     "Ascending",
     "Descending",
     "Cursor",
     "EncryptedDocument",
     "util",
 )
-__version__ = "1.3.1"
+__version__ = "1.3.2"
 VersionInfo = namedtuple("VersionInfo", "major minor micro releaselevel serial")
-version_info = VersionInfo(major=1, minor=3, micro=1, releaselevel="final", serial=0)
+version_info = VersionInfo(major=1, minor=3, micro=2, releaselevel="final", serial=0)
 logging.getLogger(__name__).addHandler(logging.NullHandler())
```

### Comparing `alaric-1.3.1/alaric/abc/logical.py` & `alaric-1.3.2/alaric/abc/logical.py`

 * *Files identical despite different names*

### Comparing `alaric-1.3.1/alaric/advanced_query.py` & `alaric-1.3.2/alaric/advanced_query.py`

 * *Files identical despite different names*

### Comparing `alaric-1.3.1/alaric/comparison/comparison_eq.py` & `alaric-1.3.2/alaric/comparison/comparison_eq.py`

 * *Files identical despite different names*

### Comparing `alaric-1.3.1/alaric/comparison/comparison_exists.py` & `alaric-1.3.2/alaric/comparison/comparison_exists.py`

 * *Files identical despite different names*

### Comparing `alaric-1.3.1/alaric/comparison/comparison_greater_than.py` & `alaric-1.3.2/alaric/comparison/comparison_greater_than.py`

 * *Files identical despite different names*

### Comparing `alaric-1.3.1/alaric/comparison/comparison_in.py` & `alaric-1.3.2/alaric/comparison/comparison_in.py`

 * *Files identical despite different names*

### Comparing `alaric-1.3.1/alaric/comparison/comparison_less_than.py` & `alaric-1.3.2/alaric/comparison/comparison_less_than.py`

 * *Files identical despite different names*

### Comparing `alaric-1.3.1/alaric/cursor.py` & `alaric-1.3.2/alaric/cursor.py`

 * *Files identical despite different names*

### Comparing `alaric-1.3.1/alaric/document.py` & `alaric-1.3.2/alaric/document.py`

 * *Files identical despite different names*

### Comparing `alaric-1.3.1/alaric/encrypted_document.py` & `alaric-1.3.2/alaric/encrypted_document.py`

 * *Files identical despite different names*

### Comparing `alaric-1.3.1/alaric/encryption/automatic_hashed_fields.py` & `alaric-1.3.2/alaric/encryption/automatic_hashed_fields.py`

 * *Files identical despite different names*

### Comparing `alaric-1.3.1/alaric/encryption/hashed_fields.py` & `alaric-1.3.2/alaric/encryption/hashed_fields.py`

 * *Files identical despite different names*

### Comparing `alaric-1.3.1/alaric/encryption/hashed_query_field.py` & `alaric-1.3.2/alaric/encryption/hashed_query_field.py`

 * *Files identical despite different names*

### Comparing `alaric-1.3.1/alaric/logical/logical_and.py` & `alaric-1.3.2/alaric/logical/logical_and.py`

 * *Files identical despite different names*

### Comparing `alaric-1.3.1/alaric/logical/logical_not.py` & `alaric-1.3.2/alaric/logical/logical_not.py`

 * *Files identical despite different names*

### Comparing `alaric-1.3.1/alaric/logical/logical_or.py` & `alaric-1.3.2/alaric/logical/logical_or.py`

 * *Files identical despite different names*

### Comparing `alaric-1.3.1/alaric/meta/negate.py` & `alaric-1.3.2/alaric/meta/negate.py`

 * *Files identical despite different names*

### Comparing `alaric-1.3.1/alaric/projections/projections.py` & `alaric-1.3.2/alaric/projections/projections.py`

 * *Files identical despite different names*

### Comparing `alaric-1.3.1/alaric/query_builder.py` & `alaric-1.3.2/alaric/query_builder.py`

 * *Files identical despite different names*

### Comparing `alaric-1.3.1/alaric/util.py` & `alaric-1.3.2/alaric/util.py`

 * *Files identical despite different names*

### Comparing `alaric-1.3.1/alaric.egg-info/PKG-INFO` & `alaric-1.3.2/alaric.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alaric
-Version: 1.3.1
+Version: 1.3.2
 Summary: A simplistic yet powerful asynchronous MongoDB query engine.
 Author: Skelmis
 Author-email: ethan@koldfusion.xyz
 Project-URL: Issue tracker, https://github.com/Skelmis/Alaric/issues
 Project-URL: Documentation, https://alaric.rtfd.io/
 Project-URL: Homepage, https://github.com/Skelmis/Alaric
 Classifier: Programming Language :: Python :: 3
```

### Comparing `alaric-1.3.1/alaric.egg-info/SOURCES.txt` & `alaric-1.3.2/alaric.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -39,8 +39,12 @@
 alaric/meta/case_insensitive.py
 alaric/meta/negate.py
 alaric/projections/__init__.py
 alaric/projections/hide.py
 alaric/projections/projections.py
 alaric/projections/show.py
 alaric/types/__init__.py
-alaric/types/object_id.py
+alaric/types/object_id.py
+tests/test_all.py
+tests/test_cursors.py
+tests/test_document.py
+tests/test_encrypted_document.py
```

### Comparing `alaric-1.3.1/setup.py` & `alaric-1.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     long_description_content_type="text/markdown",
     project_urls={
         "Issue tracker": "https://github.com/Skelmis/Alaric/issues",
         "Documentation": "https://alaric.rtfd.io/",
         "Homepage": "https://github.com/Skelmis/Alaric",
     },
     packages=find_packages(include=("alaric", "alaric.*")),
-    install_requires=["dnspython==2.2.1", "motor==3.0.0"],
+    install_requires=["dnspython>=2.2.1", "motor>=3.0.0"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.8",
 )
```

