# Comparing `tmp/netin-1.0.5.6.tar.gz` & `tmp/netin-1.0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netin-1.0.5.6.tar", last modified: Sun Apr 23 08:34:31 2023, max compression
+gzip compressed data, was "netin-1.0.5.7.tar", last modified: Sun Apr 23 15:08:11 2023, max compression
```

## Comparing `netin-1.0.5.6.tar` & `netin-1.0.5.7.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 08:34:31.523171 netin-1.0.5.6/
--rw-r--r--   0 espinl    (1001) espinl    (1001)    20843 2023-04-06 14:10:28.000000 netin-1.0.5.6/LICENSE
--rw-r--r--   0 espinl    (1001) espinl    (1001)      457 2023-04-16 06:40:57.000000 netin-1.0.5.6/MANIFEST.in
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3774 2023-04-23 08:34:31.523171 netin-1.0.5.6/PKG-INFO
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2502 2023-04-23 08:16:29.000000 netin-1.0.5.6/README.rst
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 08:34:31.519170 netin-1.0.5.6/examples/
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 08:34:31.519170 netin-1.0.5.6/examples/directed/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      311 2023-04-15 01:00:38.000000 netin-1.0.5.6/examples/directed/dh.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      258 2023-04-07 18:39:19.000000 netin-1.0.5.6/examples/directed/dpa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      315 2023-04-15 01:15:07.000000 netin-1.0.5.6/examples/directed/dpah.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 08:34:31.519170 netin-1.0.5.6/examples/notebooks/
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2947 2023-04-19 11:08:57.000000 netin-1.0.5.6/examples/notebooks/deleteme.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 08:34:31.523171 netin-1.0.5.6/examples/undirected/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      196 2023-04-07 14:05:50.000000 netin-1.0.5.6/examples/undirected/pa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      251 2023-04-14 23:44:49.000000 netin-1.0.5.6/examples/undirected/pah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      220 2023-04-14 23:45:47.000000 netin-1.0.5.6/examples/undirected/patc.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      274 2023-04-07 22:28:52.000000 netin-1.0.5.6/examples/undirected/patch.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 08:34:31.523171 netin-1.0.5.6/netin/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      353 2023-04-23 08:24:34.000000 netin-1.0.5.6/netin/__init__.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 08:34:31.523171 netin-1.0.5.6/netin/algorithms/
--rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-06 13:44:46.000000 netin-1.0.5.6/netin/algorithms/__init__.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 08:34:31.523171 netin-1.0.5.6/netin/generators/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      406 2023-04-23 06:45:06.000000 netin-1.0.5.6/netin/generators/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     4078 2023-04-15 01:01:03.000000 netin-1.0.5.6/netin/generators/dh.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)    13133 2023-04-23 08:09:54.000000 netin-1.0.5.6/netin/generators/directed.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2385 2023-04-14 21:16:14.000000 netin-1.0.5.6/netin/generators/dpa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     5002 2023-04-23 07:49:19.000000 netin-1.0.5.6/netin/generators/dpah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)    21404 2023-04-23 08:10:40.000000 netin-1.0.5.6/netin/generators/graph.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     6332 2023-04-15 18:01:34.000000 netin-1.0.5.6/netin/generators/h.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1948 2023-04-14 21:16:41.000000 netin-1.0.5.6/netin/generators/pa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     6228 2023-04-23 07:46:08.000000 netin-1.0.5.6/netin/generators/pah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3676 2023-04-23 06:45:06.000000 netin-1.0.5.6/netin/generators/patc.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     5682 2023-04-23 07:29:26.000000 netin-1.0.5.6/netin/generators/patch.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     6438 2023-04-23 06:45:06.000000 netin-1.0.5.6/netin/generators/tc.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 08:34:31.523171 netin-1.0.5.6/netin/generators/tests/
--rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-15 10:40:52.000000 netin-1.0.5.6/netin/generators/tests/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3106 2023-04-14 21:24:51.000000 netin-1.0.5.6/netin/generators/tests/test_directed.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     4122 2023-04-15 01:17:44.000000 netin-1.0.5.6/netin/generators/tests/test_dpah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3241 2023-04-15 01:19:15.000000 netin-1.0.5.6/netin/generators/tests/test_patch.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3895 2023-04-15 01:22:06.000000 netin-1.0.5.6/netin/generators/tests/test_undirected.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     8697 2023-04-23 08:15:01.000000 netin-1.0.5.6/netin/generators/undirected.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 08:34:31.523171 netin-1.0.5.6/netin/stats/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      288 2023-04-15 18:06:03.000000 netin-1.0.5.6/netin/stats/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2271 2023-04-23 06:45:06.000000 netin-1.0.5.6/netin/stats/distributions.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2753 2023-04-15 22:08:18.000000 netin-1.0.5.6/netin/stats/ranking.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 08:34:31.523171 netin-1.0.5.6/netin/utils/
--rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-14 21:38:11.000000 netin-1.0.5.6/netin/utils/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1075 2023-04-15 18:01:34.000000 netin-1.0.5.6/netin/utils/constants.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1221 2023-04-13 15:18:30.000000 netin-1.0.5.6/netin/utils/validator.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 08:34:31.523171 netin-1.0.5.6/netin/viz/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      425 2023-04-17 12:53:55.000000 netin-1.0.5.6/netin/viz/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      466 2023-04-17 10:09:00.000000 netin-1.0.5.6/netin/viz/constants.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)    26872 2023-04-19 13:08:56.000000 netin-1.0.5.6/netin/viz/handlers.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 08:34:31.523171 netin-1.0.5.6/netin.egg-info/
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3774 2023-04-23 08:34:31.000000 netin-1.0.5.6/netin.egg-info/PKG-INFO
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1290 2023-04-23 08:34:31.000000 netin-1.0.5.6/netin.egg-info/SOURCES.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-23 08:34:31.000000 netin-1.0.5.6/netin.egg-info/dependency_links.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-16 07:00:51.000000 netin-1.0.5.6/netin.egg-info/not-zip-safe
--rw-r--r--   0 espinl    (1001) espinl    (1001)      418 2023-04-23 08:34:31.000000 netin-1.0.5.6/netin.egg-info/requires.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)        6 2023-04-23 08:34:31.000000 netin-1.0.5.6/netin.egg-info/top_level.txt
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 08:34:31.523171 netin-1.0.5.6/requirements/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      182 2023-04-16 07:05:49.000000 netin-1.0.5.6/requirements/default.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)       60 2023-04-23 06:45:06.000000 netin-1.0.5.6/requirements/docs.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)       32 2023-04-15 10:35:15.000000 netin-1.0.5.6/requirements/test.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)      104 2023-04-23 08:34:31.527171 netin-1.0.5.6/setup.cfg
--rw-r--r--   0 espinl    (1001) espinl    (1001)     4247 2023-04-16 07:47:09.000000 netin-1.0.5.6/setup.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 15:08:11.201018 netin-1.0.5.7/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)    20843 2023-04-06 14:10:28.000000 netin-1.0.5.7/LICENSE
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      457 2023-04-16 06:40:57.000000 netin-1.0.5.7/MANIFEST.in
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3774 2023-04-23 15:08:11.201018 netin-1.0.5.7/PKG-INFO
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2502 2023-04-23 08:16:29.000000 netin-1.0.5.7/README.rst
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 15:08:11.197018 netin-1.0.5.7/examples/
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 15:08:11.197018 netin-1.0.5.7/examples/directed/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      311 2023-04-15 01:00:38.000000 netin-1.0.5.7/examples/directed/dh.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      258 2023-04-07 18:39:19.000000 netin-1.0.5.7/examples/directed/dpa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      315 2023-04-15 01:15:07.000000 netin-1.0.5.7/examples/directed/dpah.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 15:08:11.197018 netin-1.0.5.7/examples/notebooks/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2947 2023-04-19 11:08:57.000000 netin-1.0.5.7/examples/notebooks/deleteme.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 15:08:11.197018 netin-1.0.5.7/examples/undirected/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      196 2023-04-07 14:05:50.000000 netin-1.0.5.7/examples/undirected/pa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      251 2023-04-14 23:44:49.000000 netin-1.0.5.7/examples/undirected/pah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      220 2023-04-14 23:45:47.000000 netin-1.0.5.7/examples/undirected/patc.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      274 2023-04-07 22:28:52.000000 netin-1.0.5.7/examples/undirected/patch.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 15:08:11.197018 netin-1.0.5.7/netin/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      353 2023-04-23 14:55:29.000000 netin-1.0.5.7/netin/__init__.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 15:08:11.197018 netin-1.0.5.7/netin/algorithms/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-06 13:44:46.000000 netin-1.0.5.7/netin/algorithms/__init__.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 15:08:11.201018 netin-1.0.5.7/netin/generators/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      440 2023-04-23 11:31:23.000000 netin-1.0.5.7/netin/generators/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     5060 2023-04-23 14:19:48.000000 netin-1.0.5.7/netin/generators/dh.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)    13472 2023-04-23 14:19:40.000000 netin-1.0.5.7/netin/generators/directed.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3074 2023-04-23 14:19:52.000000 netin-1.0.5.7/netin/generators/dpa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     4701 2023-04-23 14:19:44.000000 netin-1.0.5.7/netin/generators/dpah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)    21657 2023-04-23 14:52:02.000000 netin-1.0.5.7/netin/generators/graph.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     8232 2023-04-23 12:41:52.000000 netin-1.0.5.7/netin/generators/h.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2483 2023-04-23 14:23:52.000000 netin-1.0.5.7/netin/generators/pa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     5943 2023-04-23 14:23:15.000000 netin-1.0.5.7/netin/generators/pah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     6103 2023-04-23 14:24:14.000000 netin-1.0.5.7/netin/generators/patc.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     5818 2023-04-23 14:52:52.000000 netin-1.0.5.7/netin/generators/patch.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     8299 2023-04-23 12:35:51.000000 netin-1.0.5.7/netin/generators/tc.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 15:08:11.201018 netin-1.0.5.7/netin/generators/tests/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-15 10:40:52.000000 netin-1.0.5.7/netin/generators/tests/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3106 2023-04-14 21:24:51.000000 netin-1.0.5.7/netin/generators/tests/test_directed.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     4122 2023-04-15 01:17:44.000000 netin-1.0.5.7/netin/generators/tests/test_dpah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3241 2023-04-15 01:19:15.000000 netin-1.0.5.7/netin/generators/tests/test_patch.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3895 2023-04-15 01:22:06.000000 netin-1.0.5.7/netin/generators/tests/test_undirected.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     8828 2023-04-23 14:52:43.000000 netin-1.0.5.7/netin/generators/undirected.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 15:08:11.201018 netin-1.0.5.7/netin/stats/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      288 2023-04-15 18:06:03.000000 netin-1.0.5.7/netin/stats/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2271 2023-04-23 06:45:06.000000 netin-1.0.5.7/netin/stats/distributions.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2753 2023-04-15 22:08:18.000000 netin-1.0.5.7/netin/stats/ranking.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 15:08:11.201018 netin-1.0.5.7/netin/utils/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-14 21:38:11.000000 netin-1.0.5.7/netin/utils/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1075 2023-04-15 18:01:34.000000 netin-1.0.5.7/netin/utils/constants.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1221 2023-04-13 15:18:30.000000 netin-1.0.5.7/netin/utils/validator.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 15:08:11.201018 netin-1.0.5.7/netin/viz/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      425 2023-04-17 12:53:55.000000 netin-1.0.5.7/netin/viz/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      466 2023-04-17 10:09:00.000000 netin-1.0.5.7/netin/viz/constants.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)    26872 2023-04-19 13:08:56.000000 netin-1.0.5.7/netin/viz/handlers.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 15:08:11.197018 netin-1.0.5.7/netin.egg-info/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3774 2023-04-23 15:08:11.000000 netin-1.0.5.7/netin.egg-info/PKG-INFO
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1290 2023-04-23 15:08:11.000000 netin-1.0.5.7/netin.egg-info/SOURCES.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-23 15:08:11.000000 netin-1.0.5.7/netin.egg-info/dependency_links.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-16 07:00:51.000000 netin-1.0.5.7/netin.egg-info/not-zip-safe
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      418 2023-04-23 15:08:11.000000 netin-1.0.5.7/netin.egg-info/requires.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        6 2023-04-23 15:08:11.000000 netin-1.0.5.7/netin.egg-info/top_level.txt
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 15:08:11.201018 netin-1.0.5.7/requirements/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      182 2023-04-16 07:05:49.000000 netin-1.0.5.7/requirements/default.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)       60 2023-04-23 06:45:06.000000 netin-1.0.5.7/requirements/docs.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)       32 2023-04-15 10:35:15.000000 netin-1.0.5.7/requirements/test.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      104 2023-04-23 15:08:11.201018 netin-1.0.5.7/setup.cfg
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     4247 2023-04-16 07:47:09.000000 netin-1.0.5.7/setup.py
```

### Comparing `netin-1.0.5.6/LICENSE` & `netin-1.0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.6/PKG-INFO` & `netin-1.0.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netin
-Version: 1.0.5.6
+Version: 1.0.5.7
 Summary: Python package to study inequalities in social networks
 Home-page: https://github.com/CSHVienna/NetworkInequalities
 Author: Lisette Espín-Noboa
 Author-email: espin@csh.ac.at
 Maintainer: NetIn Developers
 Maintainer-email: netin-dev@googlegroups.com
 Keywords: Networks,Inequalities,Social Networks,Ranking,InferenceGraph Theory,Mathematics,network,undirected,discrete mathematics,math
```

### Comparing `netin-1.0.5.6/README.rst` & `netin-1.0.5.7/README.rst`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.6/examples/notebooks/deleteme.py` & `netin-1.0.5.7/examples/notebooks/deleteme.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.6/netin/generators/dh.py` & `netin-1.0.5.7/netin/generators/dpah.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,123 +1,144 @@
-from typing import Union, Set
+from typing import Union, Set, Tuple
 
 import numpy as np
 
-from netin.generators.directed import DiGraph
-from netin.generators.h import Homophily
 from netin.utils import constants as const
+from netin.generators.h import Homophily
+from .dpa import DPA
 
 
-class DH(DiGraph, Homophily):
-
-    ############################################################
-    # Constructor
-    ############################################################
+class DPAH(DPA, Homophily):
 
-    def __init__(self, n: int, d: float, f_m: float, plo_M: float, plo_m: float, h_MM: float, h_mm: float,
-                 seed: object = None):
-        """
+    """Creates a new DPAH instance. A directed graph with preferential attachment and homophily.
 
-        Parameters
-        ----------
-        n: int
-            number of nodes (minimum=2)
+    Parameters
+    ----------
+    n: int
+        number of nodes (minimum=2)
 
-        k: int
-            minimum degree of nodes (minimum=1)
+    d: float
+        edge density (minimum=0, maximum=1)
 
-        f_m: float
-            fraction of minorities (minimum=1/n, maximum=(n-1)/n)
+    f_m: float
+        fraction of minorities (minimum=1/n, maximum=(n-1)/n)
 
-        d: float
-            edge density (minimum=0, maximum=1)
+    plo_M: float
+        activity (out-degree power law exponent) majority group (minimum=1)
 
-        plo_M: float
-            activity (out-degree power law exponent) majority group (minimum=1)
+    plo_m: float
+        activity (out-degree power law exponent) minority group (minimum=1)
 
-        plo_m: float
-            activity (out-degree power law exponent) minority group (minimum=1)
+    h_MM: float
+        homophily within majority group (minimum=0, maximum=1)
 
-        h_MM: float
-            homophily within majority group (minimum=0, maximum=1)
+    h_mm: float
+        homophily within minority group (minimum=0, maximum=1)
 
-        h_mm: float
-            homophily within minority group (minimum=0, maximum=1)
+    seed: object
+        seed for random number generator
 
-        seed: object
-            seed for random number generator
+    Notes
+    -----
+    The initialization is a directed with n nodes where f_m are the minority.
+    Source nodes are selected based on their activity given by plo_M (if majority) or plo_m (if minority).
+    Target nodes are selected via preferential attachment (in-degree) an homophily (h**).
+    This model is based on [Espin-Noboa2022]_ which is the directed version of the "BA Homophily" model [Karimi2018]_.
+    """
 
-        Notes
-        -----
-        The initialization is a directed with n nodes and no edges.
-        Then, everytime a node is selected as source, it gets connected to k target nodes.
-        Target nodes are selected via preferential attachment (in-degree)
+    ############################################################
+    # Constructor
+    ############################################################
 
-        References
-        ----------
-        - [1] A. L. Barabasi and R. Albert "Emergence of scaling in random networks", Science 286, pp 509-512, 1999.
-        """
-        DiGraph.__init__(self, n=n, d=d, f_m=f_m, plo_M=plo_M, plo_m=plo_m, seed=seed)
+    def __init__(self, n: int, d: float, f_m: float, plo_M: float, plo_m: float, h_MM: float, h_mm: float,
+                 seed: object = None):
+        DPA.__init__(self, n=n, d=d, f_m=f_m, plo_M=plo_M, plo_m=plo_m, seed=seed)
         Homophily.__init__(self, n=n, f_m=f_m, h_MM=h_MM, h_mm=h_mm, seed=seed)
 
     ############################################################
     # Init
     ############################################################
 
     def _infer_model_name(self):
         """
         Infers the name of the model.
         """
-        return self.set_model_name(const.DH_MODEL_NAME)
+        return self.set_model_name(const.DPAH_MODEL_NAME)
 
     ############################################################
     # Generation
     ############################################################
 
     def _initialize(self, class_attribute: str = 'm', class_values: list = None, class_labels: list = None):
-        DiGraph._initialize(self, class_attribute, class_values, class_labels)
+        """
+        Initializes the model.
+
+        Parameters
+        ----------
+        class_attribute: str
+            name of the attribute that represents the class
+
+        class_values: list
+            values of the class attribute
+
+        class_labels: list
+            labels of the class attribute mapping the class_values.
+        """
+        DPA._initialize(self, class_attribute, class_values, class_labels)
         Homophily._initialize(self, class_attribute, class_values, class_labels)
 
-    def get_target_probabilities(self, source: Union[None, int], target_set: Union[None, Set[int], np.array],
+    def get_target_probabilities(self, source: Union[None, int], target_set: Union[None, Set[int]],
                                  special_targets: Union[None, object, iter] = None) -> np.array:
-        probs, ts = Homophily.get_target_probabilities(self, source, target_set, special_targets)
+        """
+        Returns the probabilities of selecting a target node from a set of nodes based on
+        preferential attachment and homophily, i.e., in-degree or target and homophily between source and target.
+
+        Parameters
+        ----------
+        source: int
+            source node
+
+        target_set: Set[int]
+            set of target nodes
+
+        special_targets: object
+            special targets
+
+        Returns
+        -------
+        np.array
+            probabilities of selecting a target node from a set of nodes
+        """
+        probs = np.array([self.get_homophily_between_source_and_target(source, target) *
+                          (self.get_in_degree(target) + const.EPSILON) for target in target_set])
+        probs /= probs.sum()
         return probs
 
     ############################################################
     # Calculations
     ############################################################
 
     def info_params(self):
-        DiGraph.info_params(self)
+        """
+        Shows the (input) parameters of the model.
+        """
+        DPA.info_params(self)
         Homophily.info_params(self)
 
     def info_computed(self):
+        """
+        Shows the (computed) properties of the graph.
+        """
+        DPA.info_computed(self)
         Homophily.info_computed(self)
 
-    def infer_homophily_values(self) -> (float, float):
-        from sympy import symbols
-        from sympy import Eq
-        from sympy import solve
-
-        f_m = self.calculate_fraction_of_minority()
-        f_M = 1 - f_m
-
-        e = self.count_edges_types()
-        e_MM = e['MM']
-        e_mm = e['mm']
-        e_Mm = e['Mm']
-        e_mM = e['mM']
-
-        p_MM = e_MM / (e_MM + e_Mm)
-        p_mm = e_mm / (e_mm + e_mM)
-
-        # equations
-        hmm, hMM, hmM, hMm = symbols('hmm hMM hmM hMm')
-        eq1 = Eq((f_m * hmm) / ((f_m * hmm) + (f_M * hmM)), p_mm)
-        eq2 = Eq(hmm + hmM, 1)
-
-        eq3 = Eq((f_M * hMM) / ((f_M * hMM) + (f_m * hMm)), p_MM)
-        eq4 = Eq(hMM + hMm, 1)
+    def infer_homophily_values(self) -> Tuple[float, float]:
+        """
+        Infers the level of homophily within the majority and minority groups analytically.
 
-        solution = solve((eq1, eq2, eq3, eq4), (hmm, hmM, hMM, hMm))
-        h_MM, h_mm = solution[hMM], solution[hmm]
+        Returns
+        -------
+        Tuple[float, float]
+            homophily within the majority and minority groups
+        """
+        h_MM, h_mm = None, None
         return h_MM, h_mm
```

### Comparing `netin-1.0.5.6/netin/generators/directed.py` & `netin-1.0.5.7/netin/generators/directed.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 from netin.utils import constants as const
 from netin.utils import validator as val
 from .graph import Graph
 
 
 class DiGraph(nx.DiGraph, Graph):
-
     """Directed graph base model.
 
     Parameters
     ----------
     n: int
         number of nodes (minimum=2)
 
@@ -33,23 +32,26 @@
 
     seed: object
         seed for random number generator
 
     Notes
     -----
     The initialization is a directed with n nodes and no edges.
-    Source nodes are selected based on their activity given by plo_M (if majority) or plo_m (if minority), see [1].
-    Target nodes are selected depending on the chosen mechanism of edge formation:
-        - DPAH: preferential attachment (in-degree) and homophily (h**) [1]
-        - DPA: preferential attachment (in-degree)
-        - DH: homophily (h**)
+    Source nodes are selected based on their activity given by plo_M (if majority) or plo_m (if minority).
+    Target nodes are selected depending on the chosen mechanism of edge formation.
+
+    - DPAH: preferential attachment (in-degree) and homophily (h**), see :class:`netin.DPAH`
+    - DPA: preferential attachment (in-degree), see :class:`netin.DPA`
+    - DH: homophily (h**), see :class:`netin.DH`
 
     References
     ----------
-    [1] L. Espín-Noboa, C. Wagner, M. Strohmaier, & F. Karimi "Inequality and inequity in network-based ranking and recommendation algorithms" Scientific reports 12(1), 1-14, 2022.
+    .. [Espin-Noboa2022] L. Espín-Noboa, C. Wagner, M. Strohmaier, & F. Karimi "Inequality and inequity in network-based ranking and recommendation algorithms" Scientific reports 12(1), 1-14, 2022.
+    .. [Karimi2018] F. Karimi, M. Génois, C. Wagner, P. Singer, & M. Strohmaier, M "Homophily influences ranking of minorities in social networks", Scientific reports 8(1), 11077, 2018.
+    .. [BarabasiAlbert1999] A. L. Barabasi and R. Albert "Emergence of scaling in random networks", Science 286, pp 509-512, 1999.
     """
 
     ############################################################
     # Constructor
     ############################################################
 
     def __init__(self, n: int, f_m: float, d: float, plo_M: float, plo_m: float, seed: object = None):
@@ -118,15 +120,15 @@
         """
         self.expected_number_of_edges = int(round(self.d * self.n * (self.n - 1)))
         self.in_degrees = np.zeros(self.n)
         self.out_degrees = np.zeros(self.n)
 
     def _init_activity(self):
         """
-        Intializes the level of activity for each node based on the power law exponents (input param).
+        Initializes the level of activity for each node based on the power law exponents (input param).
         """
         act_M = powerlaw.Power_Law(parameters=[self.plo_M], discrete=True).generate_random(self.n_M)
         act_m = powerlaw.Power_Law(parameters=[self.plo_m], discrete=True).generate_random(self.n_m)
         self.activity = np.append(act_M, act_m)
         if np.inf in self.activity:
             self.activity[self.activity == np.inf] = 0.0
             self.activity += 1
@@ -182,24 +184,19 @@
         probs = self.get_target_probabilities(source, targets, **kwargs)
         return np.random.choice(a=targets, size=1, replace=False, p=probs)[0]
 
     def generate(self):
         """
         A directed graph of n nodes is grown by attaching new nodes.
         Source nodes are selected randomly with replacement based on their activity.
-        Each target node drawn based on the chosen mechanism of edge formation [1].
-
-        - DPA: A graph with h_mm = h_MM in [0.5, None] is a directed BA preferential attachment model.
-        - DH: A graph with h_mm not in [0.5, None] and h_MM not in [0.5, None] is a directed Erdos-Renyi with homophily.
-        - DPAH: A graph with h_mm not in [0.5, None] and h_MM not in [0.5, None] is a DPA model with homophily.
-
-        References
-        ----------
-        [1] L. Espín-Noboa, C. Wagner, M. Strohmaier, & F. Karimi "Inequality and inequity in network-based ranking and recommendation algorithms" Scientific reports 12(1), 1-14, 2022.
+        Each target node drawn based on the chosen mechanism of edge formation.
 
+        - DPA: A graph with h_mm = h_MM in [0.5, None] is a directed BA preferential attachment model, see :class:`netin.DPA`.
+        - DH: A graph with h_mm not in [0.5, None] and h_MM not in [0.5, None] is a directed Erdos-Renyi with homophily, see :class:`netin.DPH`.
+        - DPAH: A graph with h_mm not in [0.5, None] and h_MM not in [0.5, None] is a DPA model with homophily, see :class:`netin.DPAH`.
         """
         # 1. Init directed and nodes (assign class labels)
         Graph.generate(self)
 
         # 2. Iterate until reaching desired number of edges (edge density)
         tries = 0
         edge_list = defaultdict(list)
@@ -248,27 +245,30 @@
             fit_M, fit_m = self.fit_powerlaw(metric)
             print(f"- Powerlaw fit ({metric}):")
             print(f"- {self.get_majority_label()}: alpha={fit_M.power_law.alpha}, sigma={fit_M.power_law.sigma}, "
                   f"min={fit_M.power_law.xmin}, max={fit_M.power_law.xmax}")
             print(f"- {self.get_minority_label()}: alpha={fit_m.power_law.alpha}, sigma={fit_m.power_law.sigma}, "
                   f"min={fit_m.power_law.xmin}, max={fit_m.power_law.xmax}")
 
-    def fit_powerlaw(self, metric: str) -> powerlaw.Fit:
+    def fit_powerlaw(self, metric: str) -> Tuple[powerlaw.Fit, powerlaw.Fit]:
         """
         Fits a power law to the distribution given by 'metric' (the in- or out-degree of nodes in the graph).
 
         Parameters
         ----------
         metric: str
             metric to fit power law to
 
         Returns
         -------
         powerlaw.Fit
-            power law fit
+            power law fit of the majority class
+
+        powerlaw.Fit
+            power law fit of the minority class
         """
         # @TODO: validate if metric is not in_degree or out_degree
         vM = self.get_majority_value()
         dist_fnc = self.in_degree if metric == 'in_degree' else self.out_degree
         dM = [d for n, d in dist_fnc if self.nodes[n][self.class_attribute] == vM]
         dm = [d for n, d in dist_fnc if self.nodes[n][self.class_attribute] != vM]
```

### Comparing `netin-1.0.5.6/netin/generators/dpa.py` & `netin-1.0.5.7/netin/generators/dpa.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,55 +3,52 @@
 import numpy as np
 
 from netin.utils import constants as const
 from netin.generators.directed import DiGraph
 
 
 class DPA(DiGraph):
+    """Creates a new DPA instance. A directed graph with preferential attachment.
 
-    ############################################################
-    # Constructor
-    ############################################################
+    Parameters
+    ----------
+    n: int
+        number of nodes (minimum=2)
 
-    def __init__(self, n: int, d: float, f_m: float, plo_M: float, plo_m: float, seed: object = None):
-        """
+    d: float
+        edge density (minimum=0, maximum=1)
 
-        Parameters
-        ----------
-        n: int
-            number of nodes (minimum=2)
+    f_m: float
+        fraction of minorities (minimum=1/n, maximum=(n-1)/n)
 
-        k: int
-            minimum degree of nodes (minimum=1)
+    plo_M: float
+        activity (out-degree power law exponent) majority group (minimum=1)
 
-        f_m: float
-            fraction of minorities (minimum=1/n, maximum=(n-1)/n)
+    plo_m: float
+        activity (out-degree power law exponent) minority group (minimum=1)
 
-        d: float
-            edge density (minimum=0, maximum=1)
+    seed: object
+        seed for random number generator
 
-        plo_M: float
-            activity (out-degree power law exponent) majority group (minimum=1)
+    Notes
+    -----
+    The initialization is a directed with n nodes and no edges.
+    Source nodes are selected based on their activity given by plo_M (if majority) or plo_m (if minority) [Espin-Noboa2022]_.
+    Target nodes are selected via preferential attachment [BarabasiAlbert1999]_.
 
-        plo_m: float
-            activity (out-degree power law exponent) minority group (minimum=1)
+    References
+    ----------
 
-        seed: object
-            seed for random number generator
+    """
 
-        Notes
-        -----
-        The initialization is a directed with n nodes and no edges.
-        Then, everytime a node is selected as source, it gets connected to k target nodes.
-        Target nodes are selected via preferential attachment (in-degree)
+    ############################################################
+    # Constructor
+    ############################################################
 
-        References
-        ----------
-        - [1] A. L. Barabasi and R. Albert "Emergence of scaling in random networks", Science 286, pp 509-512, 1999.
-        """
+    def __init__(self, n: int, d: float, f_m: float, plo_M: float, plo_m: float, seed: object = None):
         super().__init__(n=n, d=d, f_m=f_m, plo_M=plo_M, plo_m=plo_m, seed=seed)
 
     ############################################################
     # Init
     ############################################################
 
     def _infer_model_name(self):
@@ -61,14 +58,49 @@
         return self.set_model_name(const.DPA_MODEL_NAME)
 
     ############################################################
     # Generation
     ############################################################
 
     def get_in_degree(self, n: int) -> int:
+        """
+        Returns the in-degree of node `n`.
+        This in-degree is not calculated, it is taken from the object `in_degrees` that is populated while
+        generating the graph.
+
+        Parameters
+        ----------
+        n: int
+            node id
+
+        Returns
+        -------
+        int
+            in-degree of node `n`
+        """
         return self.in_degrees[n]
 
     def get_target_probabilities(self, source: Union[None, int], target_set: Union[None, Set[int], np.array],
                                  special_targets: Union[None, object, iter] = None) -> np.array:
+        """
+        Returns the probabilities for each target node in `target_set` to be selected as target node
+        given source node `source`.
+
+        Parameters
+        ----------
+        source: int
+            source node id
+
+        target_set: Set[int]
+            set of target node ids
+
+        special_targets: object
+            special targets
+
+        Returns
+        -------
+        np.array
+            array of probabilities for each target node.
+        """
         probs = np.array([self.get_in_degree(n) + const.EPSILON for n in target_set])
         probs /= probs.sum()
         return probs
```

### Comparing `netin-1.0.5.6/netin/generators/dpah.py` & `netin-1.0.5.7/netin/generators/pah.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,77 +1,87 @@
 from typing import Union, Set, Tuple
 
 import numpy as np
+from sympy import symbols
+from sympy import Eq
+from sympy import solve
 
 from netin.utils import constants as const
 from netin.generators.h import Homophily
-from .dpa import DPA
+from .pa import PA
 
 
-class DPAH(DPA, Homophily):
-
-    """Creates a new DPAH instance.
+class PAH(PA, Homophily):
+    """Creates a new PAH instance. An undirected graph with preferential attachment and homophily.
 
     Parameters
     ----------
     n: int
         number of nodes (minimum=2)
 
-    d: float
-        edge density (minimum=0, maximum=1)
+    k: int
+        minimum degree of nodes (minimum=1)
 
     f_m: float
         fraction of minorities (minimum=1/n, maximum=(n-1)/n)
 
-    plo_M: float
-        activity (out-degree power law exponent) majority group (minimum=1)
-
-    plo_m: float
-        activity (out-degree power law exponent) minority group (minimum=1)
-
     h_MM: float
-        homophily within majority group (minimum=0, maximum=1)
+        homophily (similarity) between majority nodes (minimum=0, maximum=1.)
 
     h_mm: float
-        homophily within minority group (minimum=0, maximum=1)
+        homophily (similarity) between minority nodes (minimum=0, maximum=1.)
 
     seed: object
         seed for random number generator
 
     Notes
     -----
-    The initialization is a directed with n nodes where f_m are the minority.
-    Source nodes are selected based on their activity given by plo_M (if majority) or plo_m (if minority).
-    Target nodes are selected via preferential attachment (in-degree) an homophily (h**).
-    This model is based on [1] which is the directed version of the "BA Homophily" model [2].
-
-    References
-    ----------
-    [1] L. Espín-Noboa, C. Wagner, M. Strohmaier, & F. Karimi "Inequality and inequity in network-based ranking and recommendation algorithms" Scientific reports 12(1), 1-14, 2022.
-    [2] F. Karimi, M. Génois, C. Wagner, P. Singer, & M. Strohmaier, M "Homophily influences ranking of minorities in social networks", Scientific reports 8(1), 11077, 2018.
+    The initialization is an undirected with n nodes, where f_m are the minority.
+    Then, everytime a node is selected as source, it gets connected to k target nodes.
+    Target nodes are selected via preferential attachment (in-degree) and homophily (h_**).
+    This model is based on [Karimi2018]_ known as the "Barabasi model with homophily" or "BA Homophily".
     """
 
     ############################################################
     # Constructor
     ############################################################
 
-    def __init__(self, n: int, d: float, f_m: float, plo_M: float, plo_m: float, h_MM: float, h_mm: float,
-                 seed: object = None):
-        DPA.__init__(self, n=n, d=d, f_m=f_m, plo_M=plo_M, plo_m=plo_m, seed=seed)
+    def __init__(self, n: int, k: int, f_m: float, h_MM: float, h_mm: float, seed: object = None):
+        PA.__init__(self, n=n, k=k, f_m=f_m, seed=seed)
         Homophily.__init__(self, n=n, f_m=f_m, h_MM=h_MM, h_mm=h_mm, seed=seed)
 
     ############################################################
     # Init
     ############################################################
 
     def _infer_model_name(self):
         """
         Infers the name of the model.
         """
-        return self.set_model_name(const.DPAH_MODEL_NAME)
+        return self.set_model_name(const.PAH_MODEL_NAME)
+
+    def _validate_parameters(self):
+        """
+        Validates the parameters of the undirected.
+        """
+        PA._validate_parameters(self)
+        Homophily._validate_parameters(self)
+
+    def get_metadata_as_dict(self) -> dict:
+        """
+        Returns the metadata (parameters) of the model as a dictionary.
+
+        Returns
+        -------
+        dict
+            metadata of the model
+        """
+        obj = PA.get_metadata_as_dict(self)
+        obj.update(Homophily.get_metadata_as_dict(self))
+        return obj
 
     ############################################################
     # Generation
     ############################################################
 
     def _initialize(self, class_attribute: str = 'm', class_values: list = None, class_labels: list = None):
         """
@@ -84,66 +94,94 @@
 
         class_values: list
             values of the class attribute
 
         class_labels: list
             labels of the class attribute mapping the class_values.
         """
-        DPA._initialize(self, class_attribute, class_values, class_labels)
+        PA._initialize(self, class_attribute, class_values, class_labels)
         Homophily._initialize(self, class_attribute, class_values, class_labels)
 
     def get_target_probabilities(self, source: Union[None, int], target_set: Union[None, Set[int]],
-                                 special_targets: Union[None, object, iter] = None) -> np.array:
+                                 special_targets: Union[None, object, iter] = None) -> tuple[np.array, set[int]]:
         """
-        Returns the probabilities of selecting a target node from a set of nodes based on
-        preferential attachment and homophily,i.e., in-degree or target and homophily between source and target.
+        Returns the probabilities of selecting a target node from a set of nodes based on the preferential attachment
+        and homophily.
 
         Parameters
         ----------
         source: int
             source node
 
-        target_set: Set[int]
+        target_set: set[int]
             set of target nodes
 
         special_targets: object
             special targets
 
         Returns
         -------
-        np.array
-            probabilities of selecting a target node from a set of nodes
+        tuple[np.array, set[int]]
+            probabilities of selecting a target node from a set of nodes, and the set of target nodes
         """
         probs = np.array([self.get_homophily_between_source_and_target(source, target) *
-                          (self.get_in_degree(target) + const.EPSILON) for target in target_set])
+                          (self.degree(target) + const.EPSILON) for target in target_set])
         probs /= probs.sum()
-        return probs
+        return probs, target_set
 
     ############################################################
     # Calculations
     ############################################################
 
     def info_params(self):
         """
-        Shows the (input) parameters of the model.
+        Shows the parameters of the model.
         """
-        DPA.info_params(self)
+        PA.info_params(self)
         Homophily.info_params(self)
 
     def info_computed(self):
         """
-        Shows the (computed) properties of the graph.
+        Shows the computed properties of the graph.
         """
-        DPA.info_computed(self)
+        PA.info_computed(self)
         Homophily.info_computed(self)
 
     def infer_homophily_values(self) -> Tuple[float, float]:
         """
-        Infers the level of homophily within the majority and minority groups analytically.
+        Infers the level of homophily using the analytical solution of the model.
 
         Returns
         -------
-        Tuple[float, float]
-            homophily within the majority and minority groups
-        """
-        h_MM, h_mm = None, None
+        tuple[float, float]
+            homophily between majority nodes, and homophily between minority nodes
+
+        Notes
+        -----
+        See derivations in [Karimi2018]_.
+        """
+        f_m = self.calculate_fraction_of_minority()
+        f_M = 1 - f_m
+
+        e = self.count_edges_types()
+        e_MM = e['MM']
+        e_mm = e['mm']
+        M = e['MM'] + e['mm'] + e['Mm'] + e['mM']
+
+        p_MM = e_MM / M
+        p_mm = e_mm / M
+
+        pl_M, pl_m = self.calculate_degree_powerlaw_exponents()
+        b_M = -1 / (pl_M + 1)
+        b_m = -1 / (pl_m + 1)
+
+        # equations
+        hmm, hMM, hmM, hMm = symbols('hmm hMM hmM hMm')
+        eq1 = Eq((f_m * f_m * hmm * (1 - b_M)) / ((f_m * hmm * (1 - b_M)) + (f_M * hmM * (1 - b_m))), p_mm)
+        eq2 = Eq(hmm + hmM, 1)
+
+        eq3 = Eq((f_M * f_M * hMM * (1 - b_m)) / ((f_M * hMM * (1 - b_m)) + (f_m * hMm * (1 - b_M))), p_MM)
+        eq4 = Eq(hMM + hMm, 1)
+
+        solution = solve((eq1, eq2, eq3, eq4), (hmm, hmM, hMM, hMm))
+        h_MM, h_mm = solution[hMM], solution[hmm]
         return h_MM, h_mm
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `netin-1.0.5.6/netin/generators/graph.py` & `netin-1.0.5.7/netin/generators/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from pqdm.threads import pqdm
 
 from netin.utils import constants as const
 from netin.utils import validator as val
 
 
 class Graph(nx.Graph):
-    """Bi-populated network
+    """Bi-populated network (base graph model)
 
     Parameters
     ----------
     n: int
         number of nodes (minimum=2)
 
     f_m: float
@@ -28,30 +28,30 @@
     Notes
     -----
     The initialization is a graph with n nodes and fraction of minority f_m.
     Source nodes are selected one-by-one (if undirected) and based on their activity (if directed).
     Target nodes are selected depending on the chosen edge mechanism.
 
     Available target mechanisms for undirected networks:
-    - preferential attachment (pa), see PA [1].
-    - preferential attachment with homophily (h_**), see PAH [2].
-    - preferential attachment with triadic closure (tc), see PATC [3].
-    - preferential attachment with homophily and triadic closure (tc), see PATCH.
+    - preferential attachment (pa), see :class:`netin.PA` [1]_.
+    - preferential attachment with homophily (h_**), see :class:`netin.PAH` [2]_.
+    - preferential attachment with triadic closure (tc), see :class:`netin.PATC` [3]_.
+    - preferential attachment with homophily and triadic closure (tc), see :class:`netin.PATCH`.
 
     Available target mechanisms for directed networks:
-    - preferential attachment, see DPA [4]
-    - homophily, see DH [4]
-    - preferential attachment with homophily (h_**), see DPAH [4]
+    - preferential attachment, see :class:`netin.DPA` [4]_
+    - homophily, see :class:`netin.DH` [4]_
+    - preferential attachment with homophily (h_**), see :class:`netin.DPAH` [4]_
 
     References
     ----------
-    [1] A. L. Barabasi and R. Albert "Emergence of scaling in random networks", Science 286, pp 509-512, 1999.
-    [2] F. Karimi, M. Génois, C. Wagner, P. Singer, & M. Strohmaier, M "Homophily influences ranking of minorities in social networks", Scientific reports 8(1), 11077, 2018.
-    [3] P. Holme and B. J. Kim “Growing scale-free networks with tunable clustering” Phys. Rev. E 2002.
-    [4] L. Espín-Noboa, C. Wagner, M. Strohmaier, & F. Karimi "Inequality and inequity in network-based ranking and recommendation algorithms" Scientific reports 12(1), 1-14, 2022.
+    .. [BarabasiAlbert1999] A. L. Barabasi and R. Albert "Emergence of scaling in random networks", Science 286, pp 509-512, 1999.
+    .. [Karimi2018] F. Karimi, M. Génois, C. Wagner, P. Singer, & M. Strohmaier, M "Homophily influences ranking of minorities in social networks", Scientific reports 8(1), 11077, 2018.
+    .. [HolmeKim2002] P. Holme and B. J. Kim “Growing scale-free networks with tunable clustering” Phys. Rev. E 2002.
+    .. [Espin-Noboa2022] L. Espín-Noboa, C. Wagner, M. Strohmaier, & F. Karimi "Inequality and inequity in network-based ranking and recommendation algorithms" Scientific reports 12(1), 1-14, 2022.
     """
 
     ############################################################
     # Constructor
     ############################################################
 
     def __init__(self, n: int, f_m: float, seed: object = None):
@@ -439,35 +439,39 @@
         """
         return set([t for t in targets if t != source and t not in nx.neighbors(self, source)])
 
     def get_target_probabilities(self, source: Union[None, int], target_set: Union[None, Set[int]],
                                  special_targets: Union[None, object, iter] = None) -> tuple[np.array, set[int]]:
         """
         Returns the probability for each target node to be connected to the source node.
-        It follows an Erdos-Renyi model [1].
 
         Parameters
         ----------
         source:  int
             source node id (not used here)
 
         target_set: set
             set of target node ids
 
         special_targets:
             special targets to be considered (not used here)
 
+
+        Notes
+        -----
+        It follows an Erdos-Renyi model [ErdosRenyi1959]_.
+
         Returns
         -------
         tuple[np.array, set[int]]
             tuple of probabilities and target set
 
         References
         ----------
-        [1] P. Erdős and A. Rényi, On Random Graphs, Publ. Math. 6, 290 (1959).
+        .. [ErdosRenyi1959] P. Erdős and A. Rényi, On Random Graphs, Publ. Math. 6, 290 (1959).
         """
         # Random (erdos renyi)
         probs = np.ones(len(target_set))
         probs /= probs.sum()
         return probs, target_set
 
     def get_target(self, source: Union[None, int], targets: Union[None, Set[int]],
```

### Comparing `netin-1.0.5.6/netin/generators/h.py` & `netin-1.0.5.7/netin/generators/patch.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,184 +1,191 @@
-from collections import Counter
-from typing import Union, Set
+from typing import Union, Set, Tuple
 
 import numpy as np
 
 from netin.utils import constants as const
-from netin.utils import validator as val
-from .graph import Graph
+from netin.generators.tc import TriadicClosure
+from .pah import PAH
 
 
-class Homophily(Graph):
+class PATCH(PAH, TriadicClosure):
+    """Creates a new PATCH instance. An undirected graph with preferential attachment, homophily, and triadic closure.
 
-    ############################################################
-    # Constructor
-    ############################################################
+    Parameters
+    ----------
+    n: int
+        number of nodes (minimum=2)
 
-    def __init__(self, n: int, f_m: float, h_MM: float, h_mm: float, seed: object = None):
-        """
+    k: int
+        minimum degree of nodes (minimum=1)
 
-        Parameters
-        ----------
-        n: int
-            number of nodes (minimum=2)
+    f_m: float
+        fraction of minorities (minimum=1/n, maximum=(n-1)/n)
 
-        f_m: float
-            fraction of minorities (minimum=1/n, maximum=(n-1)/n)
+    h_MM: float
+        homophily (similarity) between majority nodes (minimum=0, maximum=1.)
 
-        h_MM: float
-            homophily (similarity) between majority nodes (minimum=0, maximum=1.)
+    h_mm: float
+        homophily (similarity) between minority nodes (minimum=0, maximum=1.)
 
-        h_mm: float
-            homophily (similarity) between minority nodes (minimum=0, maximum=1.)
+    tc: float
+        probability of a new edge to close a triad (minimum=0, maximum=1.)
 
-        attr: dict
-            attributes to add to graph as key=value pairs
+    Notes
+    -----
+    The initialization is an undirected with n nodes and no edges.
+    Then, everytime a node is selected as source, it gets connected to k target nodes.
+    Target nodes are selected via preferential attachment (in-degree) [BarabasiAlbert1999]_,
+    homophily (h_**; see :class:`netin.Homophily`) [Karimi2018]_,
+    and triadic closure (see :class:`netin.TriadicClosure`) [HolmeKim2002]_.
+    """
 
-        Notes
-        -----
-        The initialization is a graph with n nodes and no edges.
-        Then, everytime a node is selected as source, it gets connected to k target nodes.
-        Target nodes are selected via preferential attachment (in-degree), and homophily (h_**)
+    ############################################################
+    # Constructor
+    ############################################################
 
-        References
-        ----------
-        - [1] A. L. Barabasi and R. Albert "Emergence of scaling in random networks", Science 286, pp 509-512, 1999.
-        """
-        Graph.__init__(self, n=n, f_m=f_m, seed=seed)
-        self.h_MM = h_MM
-        self.h_mm = h_mm
-        self.mixing_matrix = None
+    def __init__(self, n: int, k: int, f_m: float, h_mm: float, h_MM: float, tc: float, seed: object = None):
+        PAH.__init__(self, n=n, k=k, f_m=f_m, h_MM=h_MM, h_mm=h_mm, seed=seed)
+        TriadicClosure.__init__(self, n=n, f_m=f_m, tc=tc, seed=seed)
 
     ############################################################
     # Init
     ############################################################
 
     def _infer_model_name(self):
         """
         Infers the name of the model.
         """
-        return self.set_model_name(const.H_MODEL_NAME)
+        return self.set_model_name(const.PATCH_MODEL_NAME)
 
     def _validate_parameters(self):
         """
         Validates the parameters of the undirected.
         """
-        Graph._validate_parameters(self)
-        val.validate_float(self.h_MM, minimum=0., maximum=1.)
-        val.validate_float(self.h_mm, minimum=0., maximum=1.)
+        PAH._validate_parameters(self)
+        TriadicClosure._validate_parameters(self)
 
     def get_metadata_as_dict(self) -> dict:
-        obj = Graph.get_metadata_as_dict(self)
-        obj.update({
-            'h_MM': self.h_MM,
-            'h_mm': self.h_mm,
-        })
-        return obj
+        """
+        Returns a dictionary with the metadata of the PATCH graph.
+
+        Returns
+        -------
+        dict
+            the graph  metadata as a dictionary
+        """
+        obj1 = PAH.get_metadata_as_dict(self)
+        obj2 = TriadicClosure.get_metadata_as_dict(self)
+        obj1.update(obj2)
+        return obj1
 
     ############################################################
-    # Getters & Setters
+    # Generation
     ############################################################
 
-    def set_homophily_majority(self, h_MM):
+    def get_target_probabilities(self, source: Union[None, int], target_set: Union[None, Set[int]],
+                                 special_targets: Union[None, object, iter] = None) -> Tuple[np.array, set[int]]:
         """
+        Returns the probabilities of nodes to be selected as target nodes.
+
         Parameters
         ----------
-        h_MM: float
-            homophily (similarity) between majority nodes (minimum=0, maximum=1.)
-        """
-        self.h_MM = h_MM
+        source: int
+            source node id
+
+        target_set: set
+            set of target node ids
+
+        special_targets: dict
+            dictionary of special target node ids to be considered
 
-    def get_homophily_majority(self):
-        """
         Returns
         -------
-        h_MM: float
-            homophily (similarity) between majority nodes (minimum=0, maximum=1.)
+        tuple
+            probabilities of nodes to be selected as target nodes, and set of target of nodes
+
         """
-        return self.h_MM
+        return TriadicClosure.get_target_probabilities(self, source, target_set, special_targets)
 
-    def set_homophily_minority(self, h_mm):
+    def get_target_probabilities_regular(self, source: Union[None, int], target_set: Union[None, Set[int]],
+                                         special_targets: Union[None, object, iter] = None) -> Tuple[
+        np.ndarray, set[int]]:
         """
+        Returns the probability of nodes to be selected as target nodes using the
+        preferential attachment with homophily mechanism.
+
         Parameters
         ----------
-        h_mm: float
-            homophily (similarity) between minority nodes (minimum=0, maximum=1.)
-        """
-        self.h_mm = h_mm
+        source: int
+            source node id
+
+        target_set: set
+            set of target node ids
+
+        special_targets: dict
+            dictionary of special target node ids to be considered
 
-    def get_homophily_minority(self):
-        """
         Returns
         -------
-        h_mm: float
-            homophily (similarity) between minority nodes (minimum=0, maximum=1.)
+        tuple
+            probabilities of nodes to be selected as target nodes, and set of target of nodes
         """
-        return self.h_mm
-
-    def get_homophily_between_source_and_target(self, source, target):
-        return self.mixing_matrix[self.node_labels[source], self.node_labels[target]]
+        return PAH.get_target_probabilities(self, source, target_set, special_targets)
 
-    ############################################################
-    # Generation
-    ############################################################
-
-    def _initialize(self, class_attribute: str = 'm', class_values: list = None, class_labels: list = None):
-        Graph._initialize(self, class_attribute, class_values, class_labels)
-        self.h_MM = val.calibrate_null_probabilities(self.h_MM)
-        self.h_mm = val.calibrate_null_probabilities(self.h_mm)
-        self.mixing_matrix = np.array([[self.h_MM, 1 - self.h_MM], [1 - self.h_mm, self.h_mm]])
-
-    def get_target_probabilities(self, source: Union[None, int], target_set: Union[None, Set[int], np.array],
-                                 special_targets: Union[None, object, iter] = None) -> tuple[np.array, set[int]]:
-        probs = np.array([self.get_homophily_between_source_and_target(source, target) for target in target_set])
-        probs /= probs.sum()
-        return probs, target_set
-
-    def get_target(self, source: Union[None, int], targets: Union[None, Set[int]],
-                   special_targets: Union[None, object, iter]) -> int:
+    def get_special_targets(self, source: int) -> object:
         """
-        Picks a random target node based on the homophily/preferential attachment dynamic.
+        Returns an empty dictionary (source node ids)
 
         Parameters
         ----------
-        source: int
+        source : int
             Newly added node
 
-        targets: Set[int]
-            Potential target nodes in the graph
-
         Returns
         -------
-            int: Target node that an edge should be added to
+        Dict
+            Empty dictionary
         """
-        # Collect probabilities to connect to each node in target_list
-        target_set = self.get_potential_nodes_to_connect(source, targets)
-        probs = self.get_target_probabilities(source, target_set, special_targets)
-        return np.random.choice(a=target_set, size=1, replace=False, p=probs)[0]
+        return TriadicClosure.get_special_targets(self, source)
 
     ############################################################
     # Calculations
     ############################################################
 
     def info_params(self):
-        print('h_MM: {}'.format(self.h_MM))
-        print('h_mm: {}'.format(self.h_mm))
-        print('mixing matrix: \n{}'.format(self.mixing_matrix))
+        """
+        Shows the (input) parameters of the graph.
+        """
+        PAH.info_params(self)
+        TriadicClosure.info_params(self)
 
     def info_computed(self):
-        inferred_h_MM, inferred_h_mm = self.infer_homophily_values()
-        print("- Empirical homophily within majority: {}".format(inferred_h_MM))
-        print("- Empirical homophily within minority: {}".format(inferred_h_mm))
-
-    def infer_homophily_values(self) -> (float, float):
-        print('H', self.is_directed())
-        e = self.count_edges_types()
-
-        if self.is_directed():
-            h_MM = e['MM'] / (e['MM'] + e['Mm'])
-            h_mm = e['mm'] / (e['mm'] + e['mM'])
-        else:
-            h_MM = e['MM'] / (e['MM'] + e['Mm'] + e['mM'])
-            h_mm = e['mm'] / (e['mm'] + e['mM'] + e['Mm'])
+        """
+        Shows the (computed) properties of the graph.
+        """
+        PAH.info_computed(self)
+        TriadicClosure.info_computed(self)
+
+    def infer_homophily_values(self) -> Tuple[float, float]:
+        """
+        Infers analytically the homophily values of the graph.
 
+        Returns
+        -------
+        tuple
+            homophily values of the graph (majority, minority)
+        """
+        h_MM = None
+        h_mm = None
         return h_MM, h_mm
+
+    def infer_triadic_closure(self) -> float:
+        """
+        Infers analytically the triadic closure value of the graph.
+
+        Returns
+        -------
+        float
+            triadic closure probability of the graph
+        """
+        tc = None
+        return tc
```

### Comparing `netin-1.0.5.6/netin/generators/pa.py` & `netin-1.0.5.7/netin/generators/pa.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,43 +4,41 @@
 import numpy as np
 
 from netin.utils import constants as const
 from netin.generators.undirected import UnDiGraph
 
 
 class PA(UnDiGraph):
+    """Creates a new PA instance. An undirected graph with preferential attachment.
 
+    Parameters
+    ----------
+    n: int
+        number of nodes (minimum=2)
+
+    k: int
+        minimum degree of nodes (minimum=1)
+
+    f_m: float
+        fraction of minorities (minimum=1/n, maximum=(n-1)/n)
+
+    seed: object
+        seed for random number generator
+
+    Notes
+    -----
+    The initialization is an undirected graph with n nodes and no edges.
+    Then, everytime a node is selected as source, it gets connected to k target nodes.
+    Target nodes are selected via preferential attachment (in-degree), see [BarabasiAlbert1999]_.
+    """
     ############################################################
     # Constructor
     ############################################################
 
     def __init__(self, n: int, k: int, f_m: float, seed: object = None):
-        """
-
-        Parameters
-        ----------
-        n: int
-            number of nodes (minimum=2)
-
-        k: int
-            minimum degree of nodes (minimum=1)
-
-        f_m: float
-            fraction of minorities (minimum=1/n, maximum=(n-1)/n)
-
-        Notes
-        -----
-        The initialization is a undirected with n nodes and no edges.
-        Then, everytime a node is selected as source, it gets connected to k target nodes.
-        Target nodes are selected via preferential attachment (in-degree)
-
-        References
-        ----------
-        - [1] A. L. Barabasi and R. Albert "Emergence of scaling in random networks", Science 286, pp 509-512, 1999.
-        """
         super().__init__(n, k, f_m, seed)
 
     ############################################################
     # Init
     ############################################################
 
     def _infer_model_name(self):
@@ -51,10 +49,33 @@
 
     ############################################################
     # Generation
     ############################################################
 
     def get_target_probabilities(self, source: Union[None, int], target_set: Union[None, Set[int]],
                                  special_targets: Union[None, object, iter] = None) -> tuple[np.array, set[int]]:
+        """
+        Returns the probabilities of the target nodes to be selected given a source node.
+        This probability is proportional to the degree of the target node.
+
+        Parameters
+        ----------
+        source: int
+            source node (id)
+
+        target_set: set
+            set of target nodes (ids)
+
+        special_targets: object
+            special targets
+
+        Returns
+        -------
+        probs: np.array
+            probabilities of the target nodes to be selected
+
+        target_set: set
+            set of target nodes (ids)
+        """
         probs = np.array([(self.degree(target) + const.EPSILON) for target in target_set])
         probs /= probs.sum()
         return probs, target_set
```

### Comparing `netin-1.0.5.6/netin/generators/pah.py` & `netin-1.0.5.7/netin/generators/dh.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,91 +1,70 @@
 from typing import Union, Set, Tuple
 
 import numpy as np
-from sympy import symbols
-from sympy import Eq
-from sympy import solve
 
-from netin.utils import constants as const
+from netin.generators.directed import DiGraph
 from netin.generators.h import Homophily
-from .pa import PA
+from netin.utils import constants as const
 
 
-class PAH(PA, Homophily):
-    """Creates a new PAH instance.
+class DH(DiGraph, Homophily):
+    """ Creates a new DH instance. A directed graph with homophily.
 
     Parameters
     ----------
     n: int
         number of nodes (minimum=2)
 
-    k: int
-        minimum degree of nodes (minimum=1)
+    d: float
+        edge density (minimum=0, maximum=1)
 
     f_m: float
         fraction of minorities (minimum=1/n, maximum=(n-1)/n)
 
+    plo_M: float
+        activity (out-degree power law exponent) majority group (minimum=1)
+
+    plo_m: float
+        activity (out-degree power law exponent) minority group (minimum=1)
+
     h_MM: float
-        homophily (similarity) between majority nodes (minimum=0, maximum=1.)
+        homophily within majority group (minimum=0, maximum=1)
 
     h_mm: float
-        homophily (similarity) between minority nodes (minimum=0, maximum=1.)
+        homophily within minority group (minimum=0, maximum=1)
 
     seed: object
         seed for random number generator
 
     Notes
     -----
-    The initialization is an undirected with n nodes, where f_m are the minority.
-    Then, everytime a node is selected as source, it gets connected to k target nodes.
-    Target nodes are selected via preferential attachment (in-degree) and homophily (h_**).
-    This model is based on [1] known as the "Barabasi model with homophily" or "BA Homophily".
-
-    References
-    ----------
-    [1] F. Karimi, M. Génois, C. Wagner, P. Singer, & M. Strohmaier, M "Homophily influences ranking of minorities in social networks", Scientific reports 8(1), 11077, 2018.
+    The initialization is a directed with n nodes and no edges.
+    Source nodes are selected based on their activity given by plo_M (if majority) or plo_m (if minority).
+    Target nodes are selected via homophily, see [Espin-Noboa2022]_.
     """
 
     ############################################################
     # Constructor
     ############################################################
 
-    def __init__(self, n: int, k: int, f_m: float, h_MM: float, h_mm: float, seed: object = None):
-        PA.__init__(self, n=n, k=k, f_m=f_m, seed=seed)
+    def __init__(self, n: int, d: float, f_m: float, plo_M: float, plo_m: float, h_MM: float, h_mm: float,
+                 seed: object = None):
+        DiGraph.__init__(self, n=n, d=d, f_m=f_m, plo_M=plo_M, plo_m=plo_m, seed=seed)
         Homophily.__init__(self, n=n, f_m=f_m, h_MM=h_MM, h_mm=h_mm, seed=seed)
 
     ############################################################
     # Init
     ############################################################
 
     def _infer_model_name(self):
         """
         Infers the name of the model.
         """
-        return self.set_model_name(const.PAH_MODEL_NAME)
-
-    def _validate_parameters(self):
-        """
-        Validates the parameters of the undirected.
-        """
-        PA._validate_parameters(self)
-        Homophily._validate_parameters(self)
-
-    def get_metadata_as_dict(self) -> dict:
-        """
-        Returns the metadata (parameters) of the model as a dictionary.
-
-        Returns
-        -------
-        dict
-            metadata of the model
-        """
-        obj = PA.get_metadata_as_dict(self)
-        obj.update(Homophily.get_metadata_as_dict(self))
-        return obj
+        return self.set_model_name(const.DH_MODEL_NAME)
 
     ############################################################
     # Generation
     ############################################################
 
     def _initialize(self, class_attribute: str = 'm', class_values: list = None, class_labels: list = None):
         """
@@ -98,95 +77,91 @@
 
         class_values: list
             values of the class attribute
 
         class_labels: list
             labels of the class attribute mapping the class_values.
         """
-        PA._initialize(self, class_attribute, class_values, class_labels)
+        DiGraph._initialize(self, class_attribute, class_values, class_labels)
         Homophily._initialize(self, class_attribute, class_values, class_labels)
 
-    def get_target_probabilities(self, source: Union[None, int], target_set: Union[None, Set[int]],
-                                 special_targets: Union[None, object, iter] = None) -> tuple[np.array, set[int]]:
+    def get_target_probabilities(self, source: Union[None, int], target_set: Union[None, Set[int], np.array],
+                                 special_targets: Union[None, object, iter] = None) -> np.array:
         """
-        Returns the probabilities of selecting a target node from a set of nodes based on the preferential attachment
-        and homophily.
+        Returns the probabilities of the target nodes to be selected given a source node.
 
         Parameters
         ----------
         source: int
-            source node
+            source node (id)
 
-        target_set: set[int]
-            set of target nodes
+        target_set: set
+            set of target nodes (ids)
 
         special_targets: object
             special targets
 
         Returns
         -------
-        tuple[np.array, set[int]]
-            probabilities of selecting a target node from a set of nodes, and the set of target nodes
+        probs: np.array
+            probabilities of the target nodes to be selected
+
         """
-        probs = np.array([self.get_homophily_between_source_and_target(source, target) *
-                          (self.degree(target) + const.EPSILON) for target in target_set])
-        probs /= probs.sum()
-        return probs, target_set
+        probs, ts = Homophily.get_target_probabilities(self, source, target_set, special_targets)
+        return probs
 
     ############################################################
     # Calculations
     ############################################################
 
     def info_params(self):
         """
         Shows the parameters of the model.
         """
-        PA.info_params(self)
+        DiGraph.info_params(self)
         Homophily.info_params(self)
 
     def info_computed(self):
         """
         Shows the computed properties of the graph.
         """
-        PA.info_computed(self)
         Homophily.info_computed(self)
 
     def infer_homophily_values(self) -> Tuple[float, float]:
         """
-        Infers the level of homopolily using the analutical solution of the model [1].
+        Infers analytically the homophily values for the majority and minority classes.
 
         Returns
         -------
-        tuple[float, float]
-            homophily between majority nodes, and homophily between minority nodes
-
-        References
-        ----------
-        [1] F. Karimi, M. Génois, C. Wagner, P. Singer, & M. Strohmaier, M "Homophily influences ranking of minorities in social networks", Scientific reports 8(1), 11077, 2018.
+        h_MM: float
+            homophily within majority group
 
+        h_mm: float
+            homophily within minority group
         """
+        from sympy import symbols
+        from sympy import Eq
+        from sympy import solve
+
         f_m = self.calculate_fraction_of_minority()
         f_M = 1 - f_m
 
         e = self.count_edges_types()
         e_MM = e['MM']
         e_mm = e['mm']
-        M = e['MM'] + e['mm'] + e['Mm'] + e['mM']
-
-        p_MM = e_MM / M
-        p_mm = e_mm / M
+        e_Mm = e['Mm']
+        e_mM = e['mM']
 
-        pl_M, pl_m = self.calculate_degree_powerlaw_exponents()
-        b_M = -1 / (pl_M + 1)
-        b_m = -1 / (pl_m + 1)
+        p_MM = e_MM / (e_MM + e_Mm)
+        p_mm = e_mm / (e_mm + e_mM)
 
         # equations
         hmm, hMM, hmM, hMm = symbols('hmm hMM hmM hMm')
-        eq1 = Eq((f_m * f_m * hmm * (1 - b_M)) / ((f_m * hmm * (1 - b_M)) + (f_M * hmM * (1 - b_m))), p_mm)
+        eq1 = Eq((f_m * hmm) / ((f_m * hmm) + (f_M * hmM)), p_mm)
         eq2 = Eq(hmm + hmM, 1)
 
-        eq3 = Eq((f_M * f_M * hMM * (1 - b_m)) / ((f_M * hMM * (1 - b_m)) + (f_m * hMm * (1 - b_M))), p_MM)
+        eq3 = Eq((f_M * hMM) / ((f_M * hMM) + (f_m * hMm)), p_MM)
         eq4 = Eq(hMM + hMm, 1)
 
         solution = solve((eq1, eq2, eq3, eq4), (hmm, hmM, hMM, hMm))
         h_MM, h_mm = solution[hMM], solution[hmm]
         return h_MM, h_mm
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `netin-1.0.5.6/netin/generators/tc.py` & `netin-1.0.5.7/netin/generators/tc.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,46 +5,40 @@
 
 from netin.utils import constants as const
 from netin.utils import validator as val
 from .graph import Graph
 
 
 class TriadicClosure(Graph):
+    """Class to model triadic closure as a mechanism of edge formation given a source and a target node.
+
+    Parameters
+    ----------
+    n: int
+        number of nodes (minimum=2)
+
+    f_m: float
+        fraction of minorities (minimum=1/n, maximum=(n-1)/n)
+
+    tc: float
+        triadic closure probability (minimum=0, maximum=1)
+
+    seed: object
+        seed for random number generator
+
+    Notes
+    -----
+    This class does not generate a graph.
+    """
 
     ############################################################
     # Constructor
     ############################################################
 
     def __init__(self, n: int, f_m: float, tc: float, seed: object = None):
-        """
-
-        Parameters
-        ----------
-        n: int
-            number of nodes (minimum=2)
-
-        f_m: float
-            fraction of minorities (minimum=1/n, maximum=(n-1)/n)
-
-        tc: float
-            triadic closure probability (minimum=0, maximum=1)
-
-        seed: object
-            seed for random number generator
-
-        Notes
-        -----
-        The initialization is a graph with n nodes and no edges.
-        Then, everytime a node is selected as source, it gets connected to k target nodes.
-        Target nodes are selected via preferential attachment (in-degree), and homophily (h_**)
-
-        References
-        ----------
-        - [1] A. L. Barabasi and R. Albert "Emergence of scaling in random networks", Science 286, pp 509-512, 1999.
-        """
         Graph.__init__(self, n=n, f_m=f_m, seed=seed)
         self.tc = tc
 
     ############################################################
     # Init
     ############################################################
 
@@ -58,108 +52,188 @@
         """
         Validates the parameters of the undirected.
         """
         Graph._validate_parameters(self)
         val.validate_float(self.tc, minimum=0., maximum=1.)
 
     def get_metadata_as_dict(self) -> dict:
+        """
+        Returns the metadata (parameters) of the model as a dictionary.
+
+        Returns
+        -------
+        dict
+            metadata of the model
+        """
         obj = Graph.get_metadata_as_dict(self)
         obj.update({
             'tc': self.tc,
         })
         return obj
 
     ############################################################
     # Getters & Setters
     ############################################################
 
     def set_triadic_closure(self, tc):
         """
+        Sets the triadic closure probability `tc`.
+
         Parameters
         ----------
         tc: float
             triadic closure probability (minimum=0, maximum=1)
         """
         self.tc = tc
 
-    def get_triadic_closure(self):
+    def get_triadic_closure(self) -> float:
         """
+        Returns the triadic closure probability `tc`.
+
         Returns
         -------
         tc: float
             triadic closure probability (minimum=0, maximum=1)
         """
         return self.tc
 
     ############################################################
     # Generation
     ############################################################
 
     def _initialize(self, class_attribute: str = 'm', class_values: list = None, class_labels: list = None):
+        """
+        Initializes the model.
+
+        Parameters
+        ----------
+        class_attribute: str
+            name of the attribute that represents the class
+
+        class_values: list
+            values of the class attribute
+
+        class_labels: list
+            labels of the class attribute mapping the class_values.
+        """
         Graph._initialize(self, class_attribute, class_values, class_labels)
 
     def get_special_targets(self, source: int) -> object:
-        """ Return an empty dictionary (source node ids)
+        """
+        Returns an empty dictionary (source node ids)
 
         Parameters
         ----------
         source : int
             Newly added node
 
         Returns
         -------
         object
             Return an empty dictionary (source node ids)
         """
         return defaultdict(int)
 
-    def get_target_probabilities_regular(self, source: Union[None, int], target_set: Union[None, Set[int]],
-                                         special_targets: Union[None, object, iter] = None) -> tuple[
-        np.array, set[int]]:
+    def get_target_probabilities_regular(self, source: Union[None, int],
+                                         target_set: Union[None, Set[int]],
+                                         special_targets: Union[None, object, iter] = None) -> \
+            tuple[np.array, set[int]]:
         # return Graph.get_target_probabilities(self, source, target_set, special_targets)
         pass
 
     def get_target_probabilities(self, source: Union[None, int], target_set: Union[None, Set[int]],
                                  special_targets: Union[None, object, iter] = None) -> tuple[np.array, set[int]]:
+        """
+        Returns the probabilities of selecting a target node from a set of nodes based on triadic closure,
+        or a regular mechanism.
+
+        Parameters
+        ----------
+        source: int
+            source node
+
+        target_set: set[int]
+            set of target nodes
+
+        special_targets: object
+            special targets
+
+        Returns
+        -------
+        tuple[np.array, set[int]]
+            probabilities of selecting a target node from a set of nodes, and the set of target nodes`
+        """
         tc_prob = np.random.random()
 
         if tc_prob < self.tc and len(special_targets) > 0:
             target_set, probs = zip(*[(t, w) for t, w in special_targets.items()])
             probs = np.array(probs).astype(np.float32)
             probs /= probs.sum()
             target_set = set(target_set)
             return probs, target_set
 
         # Pick a target
         return self.get_target_probabilities_regular(source, target_set, special_targets)
 
-    def get_target(self, source: Union[None, int], targets: Union[None, Set[int]],
+    def get_target(self, source: Union[None, int],
+                   targets: Union[None, Set[int]],
                    special_targets: Union[None, object, iter]) -> int:
         """
         Picks a random target node based on the homophily/preferential attachment dynamic.
 
         Parameters
         ----------
         source: int
             Newly added node
 
         targets: Set[int]
             Potential target nodes in the graph
 
+        special_targets: object
+            Special target nodes
+
         Returns
         -------
-            int: Target node that an edge should be added to
+            int
+                Target node that an edge should be created from `source`
         """
         # Collect probabilities to connect to each node in target_list
         target_set = self.get_potential_nodes_to_connect(source, targets)
         probs = self.get_target_probabilities(source, target_set, special_targets)
         return np.random.choice(a=target_set, size=1, replace=False, p=probs)[0]
 
     def update_special_targets(self, idx_target: int, source: int, target: int, targets: Set[int],
                                special_targets: object) -> object:
+        """
+        Updates the set of special targets based on the triadic closure mechanism.
+        When an edge is created, multiple potential triadic closures emerge (i.e., two-hop neighbors that are not yet
+        directly connected). These are added to the set of special targets.
+
+        Parameters
+        ----------
+        idx_target: int
+            index of the target node
+
+        source: int
+            source node
+
+        target: int
+            target node
+
+        targets: Set[int]
+            set of target nodes
+
+        special_targets: object
+            special targets
+
+        Returns
+        -------
+        object
+            updated special targets
+        """
         if idx_target < self.k - 1:
             # Remove target candidates of source
             targets.discard(target)
             if target in special_targets:
                 del special_targets[target]  # Remove target from TC candidates
 
             # Incr. occurrence counter for friends of new friend
@@ -172,17 +246,23 @@
         return special_targets
 
     ############################################################
     # Calculations
     ############################################################
 
     def info_params(self):
+        """
+        Shows the parameters of the model.
+        """
         print('tc: {}'.format(self.tc))
 
     def info_computed(self):
+        """
+        Shows the computed properties of the graph.
+        """
         inferred_tc = self.infer_triadic_closure()
         print("- Empirical triadic closure: {}".format(inferred_tc))
 
     def infer_triadic_closure(self) -> float:
         # @TODO: To be implemented
         tc = None
         return tc
```

### Comparing `netin-1.0.5.6/netin/generators/tests/test_directed.py` & `netin-1.0.5.7/netin/generators/tests/test_directed.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.6/netin/generators/tests/test_dpah.py` & `netin-1.0.5.7/netin/generators/tests/test_dpah.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.6/netin/generators/tests/test_patch.py` & `netin-1.0.5.7/netin/generators/tests/test_patch.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.6/netin/generators/tests/test_undirected.py` & `netin-1.0.5.7/netin/generators/tests/test_undirected.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.6/netin/generators/undirected.py` & `netin-1.0.5.7/netin/generators/undirected.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Set
-from typing import Union
 from typing import Tuple
+from typing import Union
 
 import networkx as nx
 import numpy as np
 import powerlaw
 
 from netin.utils import validator as val
 from .graph import Graph
@@ -28,24 +28,25 @@
         seed for random number generator
 
     Notes
     -----
     The initialization is an undirected graph with n nodes and no edges.
     Then, everytime a node is selected as source, it gets connected to k target nodes.
     Target nodes are selected depending on the chosen mechanism of edge formation:
-        - PA: Preferential attachment (in-degree) [1]
-        - PAH: Preferential attachment (in-degree) with homophily [2]
-        - PATC: Preferential attachment (in-degree) with triadic closure [3]
-        - PATCH: Preferential attachment (in-degree) with homophily and triadic closure
+
+    - PA: Preferential attachment (in-degree), see :class:`netin.PA` [BarabasiAlbert1999]_
+    - PAH: Preferential attachment (in-degree) with homophily, see :class:`netin.PAH` [Karimi2018]_
+    - PATC: Preferential attachment (in-degree) with triadic closure, see :class:`netin.PATC` [HolmeKim2002]_
+    - PATCH: Preferential attachment (in-degree) with homophily and triadic closure, see :class:`netin.PATCH`
 
     References
     ----------
-    [1] A. L. Barabasi and R. Albert "Emergence of scaling in random networks", Science 286, pp 509-512, 1999.
-    [2] F. Karimi, M. Génois, C. Wagner, P. Singer, & M. Strohmaier, M "Homophily influences ranking of minorities in social networks", Scientific reports 8(1), 11077, 2018.
-    [3] P. Holme and B. J. Kim “Growing scale-free networks with tunable clustering” Phys. Rev. E 2002.
+    .. [BarabasiAlbert1999] A. L. Barabasi and R. Albert "Emergence of scaling in random networks", Science 286, pp 509-512, 1999.
+    .. [Karimi2018] F. Karimi, M. Génois, C. Wagner, P. Singer, & M. Strohmaier, M "Homophily influences ranking of minorities in social networks", Scientific reports 8(1), 11077, 2018.
+    .. [HolmeKim2002] P. Holme and B. J. Kim “Growing scale-free networks with tunable clustering” Phys. Rev. E 2002.
     """
 
     ############################################################
     # Constructor
     ############################################################
 
     def __init__(self, n: int, k: int, f_m: float, seed: object = None):
@@ -91,15 +92,16 @@
             Newly added node
 
         targets: Set[int]
             Potential target nodes in the undirected based on preferential attachment
 
         Returns
         -------
-            int: Target node that an edge should be added to
+            int
+                Target node that an edge should be added to
         """
         # Collect probabilities to connect to each node in target_list
         target_set = set([t for t in targets if t != source and t not in nx.neighbors(self, source)])
         probs, target_set = self.get_target_probabilities(source, target_set, special_targets)
         return np.random.choice(a=list(target_set), size=1, replace=False, p=probs)[0]
 
     def generate(self):
@@ -109,20 +111,18 @@
 
         For triadic closure, a candidate is chosen uniformly at random from all triad-closing edges (of the new node).
         Otherwise, or if there are no triads to close, edges are connected via preferential attachment and/or homophily.
 
         Homophily varies ranges from 0 (heterophilic) to 1 (homophilic), where 0.5 is neutral.
         Similarly, triadic closure varies from 0 (no triadic closure) to 1 (full triadic closure).
 
-        . PA:    An undirected graph with h_mm = h_MM in [0.5, None] and tc = 0 is a BA preferential attachment model.
-        . PAH:   An undirected graph with h_mm not in [0.5, None] and h_MM not in [0.5, None] and tc = 0 is a PA model
-                 with homophily.
-        . PATC:  An undirected graph with h_mm = h_MM in [0.5, None] and tc > 0 is a PA model with triadic closure.
-        . PATCH: An undirected graph with h_mm not in [0.5, None] and h_MM not in [0.5, None] and tc > 0 is a PA model
-                 with homophily and triadic closure.
+        - PA: An undirected graph with h_mm = h_MM in [0.5, None] and tc = 0 is a BA preferential attachment model.
+        - PAH: An undirected graph with h_mm not in [0.5, None] and h_MM not in [0.5, None] and tc = 0 is a PA model with homophily.
+        - PATC: An undirected graph with h_mm = h_MM in [0.5, None] and tc > 0 is a PA model with triadic closure.
+        - PATCH: An undirected graph with h_mm not in [0.5, None] and h_MM not in [0.5, None] and tc > 0 is a PA model with homophily and triadic closure.
 
         """
         # 1. Init an undirected graph and nodes (assign class labels)
         super().generate()
 
         # 2. Iterate until n nodes are added (starts with k pre-existing, unconnected nodes)
         for source in self.node_list[self.k:]:
@@ -149,28 +149,28 @@
 
     def get_expected_number_of_edges(self) -> int:
         """
         Computes and returns the expected number of edges based on minimum degree `k` and number of nodes `n`
 
         Returns
         -------
-            int
-                Expected number of edges
+        int
+            Expected number of edges
         """
         return (self.get_expected_number_of_nodes() * self.get_expected_minimum_degree()) - \
             (self.get_expected_minimum_degree() ** self.get_expected_minimum_degree())
 
     def get_expected_minimum_degree(self) -> int:
         """
         Returns the expected minimum degree of the graph (`k`, the input parameter)
 
         Returns
         -------
-            int
-                Expected minimum degree
+        int
+            Expected minimum degree
         """
 
         return self.k
 
     ############################################################
     # Calculations
     ############################################################
@@ -190,22 +190,23 @@
         print(f"- {self.get_majority_label()}: alpha={fit_M.power_law.alpha}, "
               f"sigma={fit_M.power_law.sigma}, "
               f"min={fit_M.power_law.xmin}, max={fit_M.power_law.xmax}")
         print(f"- {self.get_minority_label()}: alpha={fit_m.power_law.alpha}, "
               f"sigma={fit_m.power_law.sigma}, "
               f"min={fit_m.power_law.xmin}, max={fit_m.power_law.xmax}")
 
-    def fit_degree_powerlaw(self) -> Tuple[powerlaw.Fit,powerlaw.Fit]:
+    def fit_degree_powerlaw(self) -> Tuple[powerlaw.Fit, powerlaw.Fit]:
         """
         Returns the powerlaw fit of the degree distribution to a powerlaw for the majority and minority class.
 
         Returns
         -------
         fit_M : powerlaw.Fit
             Powerlaw fit for the majority class
+
         fit_m: powerlaw.Fit
             Powerlaw fit for the minority class
         """
         vM = self.get_majority_value()
         dM = [d for n, d in self.degree() if self.nodes[n][self.class_attribute] == vM]
         dm = [d for n, d in self.degree() if self.nodes[n][self.class_attribute] != vM]
 
@@ -217,14 +218,15 @@
         """
         Returns the powerlaw exponents for the majority and minority class.
 
         Returns
         -------
         pl_M : float
             Powerlaw exponent for the majority class
+
         pl_m: float
             Powerlaw exponent for the minority class
         """
         fit_M, fit_m = self.fit_degree_powerlaw()
         pl_M = fit_M.power_law.alpha
         pl_m = fit_m.power_law.alpha
         return pl_M, pl_m
```

### Comparing `netin-1.0.5.6/netin/stats/distributions.py` & `netin-1.0.5.7/netin/stats/distributions.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.6/netin/stats/ranking.py` & `netin-1.0.5.7/netin/stats/ranking.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.6/netin/utils/constants.py` & `netin-1.0.5.7/netin/utils/constants.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.6/netin/utils/validator.py` & `netin-1.0.5.7/netin/utils/validator.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.6/netin/viz/handlers.py` & `netin-1.0.5.7/netin/viz/handlers.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.6/netin.egg-info/PKG-INFO` & `netin-1.0.5.7/netin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netin
-Version: 1.0.5.6
+Version: 1.0.5.7
 Summary: Python package to study inequalities in social networks
 Home-page: https://github.com/CSHVienna/NetworkInequalities
 Author: Lisette Espín-Noboa
 Author-email: espin@csh.ac.at
 Maintainer: NetIn Developers
 Maintainer-email: netin-dev@googlegroups.com
 Keywords: Networks,Inequalities,Social Networks,Ranking,InferenceGraph Theory,Mathematics,network,undirected,discrete mathematics,math
```

### Comparing `netin-1.0.5.6/netin.egg-info/SOURCES.txt` & `netin-1.0.5.7/netin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.6/setup.py` & `netin-1.0.5.7/setup.py`

 * *Files identical despite different names*

