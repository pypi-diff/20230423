# Comparing `tmp/netin-1.0.5.5.tar.gz` & `tmp/netin-1.0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netin-1.0.5.5.tar", last modified: Wed Apr 19 11:44:07 2023, max compression
+gzip compressed data, was "netin-1.0.5.6.tar", last modified: Sun Apr 23 08:34:31 2023, max compression
```

## Comparing `netin-1.0.5.5.tar` & `netin-1.0.5.6.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-19 11:44:07.288888 netin-1.0.5.5/
--rw-r--r--   0 espinl    (1001) espinl    (1001)    20843 2023-04-06 14:10:28.000000 netin-1.0.5.5/LICENSE
--rw-r--r--   0 espinl    (1001) espinl    (1001)      457 2023-04-16 06:40:57.000000 netin-1.0.5.5/MANIFEST.in
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3705 2023-04-19 11:44:07.288888 netin-1.0.5.5/PKG-INFO
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2433 2023-04-16 07:53:42.000000 netin-1.0.5.5/README.rst
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-19 11:44:07.284888 netin-1.0.5.5/examples/
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-19 11:44:07.284888 netin-1.0.5.5/examples/directed/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      311 2023-04-15 01:00:38.000000 netin-1.0.5.5/examples/directed/dh.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      258 2023-04-07 18:39:19.000000 netin-1.0.5.5/examples/directed/dpa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      315 2023-04-15 01:15:07.000000 netin-1.0.5.5/examples/directed/dpah.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-19 11:44:07.288888 netin-1.0.5.5/examples/notebooks/
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2947 2023-04-19 11:08:57.000000 netin-1.0.5.5/examples/notebooks/deleteme.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-19 11:44:07.288888 netin-1.0.5.5/examples/undirected/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      196 2023-04-07 14:05:50.000000 netin-1.0.5.5/examples/undirected/pa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      251 2023-04-14 23:44:49.000000 netin-1.0.5.5/examples/undirected/pah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      220 2023-04-14 23:45:47.000000 netin-1.0.5.5/examples/undirected/patc.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      274 2023-04-07 22:28:52.000000 netin-1.0.5.5/examples/undirected/patch.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-19 11:44:07.288888 netin-1.0.5.5/netin/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      353 2023-04-19 10:53:22.000000 netin-1.0.5.5/netin/__init__.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-19 11:44:07.288888 netin-1.0.5.5/netin/algorithms/
--rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-06 13:44:46.000000 netin-1.0.5.5/netin/algorithms/__init__.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-19 11:44:07.288888 netin-1.0.5.5/netin/generators/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      320 2023-04-14 21:19:23.000000 netin-1.0.5.5/netin/generators/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     4078 2023-04-15 01:01:03.000000 netin-1.0.5.5/netin/generators/dh.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     9214 2023-04-15 22:08:19.000000 netin-1.0.5.5/netin/generators/directed.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2385 2023-04-14 21:16:14.000000 netin-1.0.5.5/netin/generators/dpa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3448 2023-04-15 21:55:31.000000 netin-1.0.5.5/netin/generators/dpah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)    13362 2023-04-15 21:45:47.000000 netin-1.0.5.5/netin/generators/graph.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     6332 2023-04-15 18:01:34.000000 netin-1.0.5.5/netin/generators/h.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1948 2023-04-14 21:16:41.000000 netin-1.0.5.5/netin/generators/pa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     4363 2023-04-16 07:05:49.000000 netin-1.0.5.5/netin/generators/pah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3587 2023-04-14 21:16:55.000000 netin-1.0.5.5/netin/generators/patc.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3951 2023-04-15 22:08:18.000000 netin-1.0.5.5/netin/generators/patch.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     6339 2023-04-14 23:53:00.000000 netin-1.0.5.5/netin/generators/tc.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-19 11:44:07.288888 netin-1.0.5.5/netin/generators/tests/
--rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-15 10:40:52.000000 netin-1.0.5.5/netin/generators/tests/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3106 2023-04-14 21:24:51.000000 netin-1.0.5.5/netin/generators/tests/test_directed.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     4122 2023-04-15 01:17:44.000000 netin-1.0.5.5/netin/generators/tests/test_dpah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3241 2023-04-15 01:19:15.000000 netin-1.0.5.5/netin/generators/tests/test_patch.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3895 2023-04-15 01:22:06.000000 netin-1.0.5.5/netin/generators/tests/test_undirected.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     7000 2023-04-15 22:08:18.000000 netin-1.0.5.5/netin/generators/undirected.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-19 11:44:07.288888 netin-1.0.5.5/netin/stats/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      288 2023-04-15 18:06:03.000000 netin-1.0.5.5/netin/stats/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1854 2023-04-15 19:33:04.000000 netin-1.0.5.5/netin/stats/distributions.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2753 2023-04-15 22:08:18.000000 netin-1.0.5.5/netin/stats/ranking.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-19 11:44:07.288888 netin-1.0.5.5/netin/utils/
--rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-14 21:38:11.000000 netin-1.0.5.5/netin/utils/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1075 2023-04-15 18:01:34.000000 netin-1.0.5.5/netin/utils/constants.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1221 2023-04-13 15:18:30.000000 netin-1.0.5.5/netin/utils/validator.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-19 11:44:07.288888 netin-1.0.5.5/netin/viz/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      425 2023-04-17 12:53:55.000000 netin-1.0.5.5/netin/viz/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      466 2023-04-17 10:09:00.000000 netin-1.0.5.5/netin/viz/constants.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)    26851 2023-04-19 11:35:51.000000 netin-1.0.5.5/netin/viz/handlers.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-19 11:44:07.288888 netin-1.0.5.5/netin.egg-info/
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3705 2023-04-19 11:44:07.000000 netin-1.0.5.5/netin.egg-info/PKG-INFO
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1268 2023-04-19 11:44:07.000000 netin-1.0.5.5/netin.egg-info/SOURCES.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-19 11:44:07.000000 netin-1.0.5.5/netin.egg-info/dependency_links.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-16 07:00:51.000000 netin-1.0.5.5/netin.egg-info/not-zip-safe
--rw-r--r--   0 espinl    (1001) espinl    (1001)      418 2023-04-19 11:44:07.000000 netin-1.0.5.5/netin.egg-info/requires.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)        6 2023-04-19 11:44:07.000000 netin-1.0.5.5/netin.egg-info/top_level.txt
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-19 11:44:07.288888 netin-1.0.5.5/requirements/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      182 2023-04-16 07:05:49.000000 netin-1.0.5.5/requirements/default.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)       32 2023-04-15 10:35:15.000000 netin-1.0.5.5/requirements/test.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)      104 2023-04-19 11:44:07.288888 netin-1.0.5.5/setup.cfg
--rw-r--r--   0 espinl    (1001) espinl    (1001)     4247 2023-04-16 07:47:09.000000 netin-1.0.5.5/setup.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 08:34:31.523171 netin-1.0.5.6/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)    20843 2023-04-06 14:10:28.000000 netin-1.0.5.6/LICENSE
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      457 2023-04-16 06:40:57.000000 netin-1.0.5.6/MANIFEST.in
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3774 2023-04-23 08:34:31.523171 netin-1.0.5.6/PKG-INFO
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2502 2023-04-23 08:16:29.000000 netin-1.0.5.6/README.rst
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 08:34:31.519170 netin-1.0.5.6/examples/
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 08:34:31.519170 netin-1.0.5.6/examples/directed/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      311 2023-04-15 01:00:38.000000 netin-1.0.5.6/examples/directed/dh.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      258 2023-04-07 18:39:19.000000 netin-1.0.5.6/examples/directed/dpa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      315 2023-04-15 01:15:07.000000 netin-1.0.5.6/examples/directed/dpah.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 08:34:31.519170 netin-1.0.5.6/examples/notebooks/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2947 2023-04-19 11:08:57.000000 netin-1.0.5.6/examples/notebooks/deleteme.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 08:34:31.523171 netin-1.0.5.6/examples/undirected/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      196 2023-04-07 14:05:50.000000 netin-1.0.5.6/examples/undirected/pa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      251 2023-04-14 23:44:49.000000 netin-1.0.5.6/examples/undirected/pah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      220 2023-04-14 23:45:47.000000 netin-1.0.5.6/examples/undirected/patc.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      274 2023-04-07 22:28:52.000000 netin-1.0.5.6/examples/undirected/patch.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 08:34:31.523171 netin-1.0.5.6/netin/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      353 2023-04-23 08:24:34.000000 netin-1.0.5.6/netin/__init__.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 08:34:31.523171 netin-1.0.5.6/netin/algorithms/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-06 13:44:46.000000 netin-1.0.5.6/netin/algorithms/__init__.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 08:34:31.523171 netin-1.0.5.6/netin/generators/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      406 2023-04-23 06:45:06.000000 netin-1.0.5.6/netin/generators/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     4078 2023-04-15 01:01:03.000000 netin-1.0.5.6/netin/generators/dh.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)    13133 2023-04-23 08:09:54.000000 netin-1.0.5.6/netin/generators/directed.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2385 2023-04-14 21:16:14.000000 netin-1.0.5.6/netin/generators/dpa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     5002 2023-04-23 07:49:19.000000 netin-1.0.5.6/netin/generators/dpah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)    21404 2023-04-23 08:10:40.000000 netin-1.0.5.6/netin/generators/graph.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     6332 2023-04-15 18:01:34.000000 netin-1.0.5.6/netin/generators/h.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1948 2023-04-14 21:16:41.000000 netin-1.0.5.6/netin/generators/pa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     6228 2023-04-23 07:46:08.000000 netin-1.0.5.6/netin/generators/pah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3676 2023-04-23 06:45:06.000000 netin-1.0.5.6/netin/generators/patc.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     5682 2023-04-23 07:29:26.000000 netin-1.0.5.6/netin/generators/patch.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     6438 2023-04-23 06:45:06.000000 netin-1.0.5.6/netin/generators/tc.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 08:34:31.523171 netin-1.0.5.6/netin/generators/tests/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-15 10:40:52.000000 netin-1.0.5.6/netin/generators/tests/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3106 2023-04-14 21:24:51.000000 netin-1.0.5.6/netin/generators/tests/test_directed.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     4122 2023-04-15 01:17:44.000000 netin-1.0.5.6/netin/generators/tests/test_dpah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3241 2023-04-15 01:19:15.000000 netin-1.0.5.6/netin/generators/tests/test_patch.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3895 2023-04-15 01:22:06.000000 netin-1.0.5.6/netin/generators/tests/test_undirected.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     8697 2023-04-23 08:15:01.000000 netin-1.0.5.6/netin/generators/undirected.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 08:34:31.523171 netin-1.0.5.6/netin/stats/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      288 2023-04-15 18:06:03.000000 netin-1.0.5.6/netin/stats/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2271 2023-04-23 06:45:06.000000 netin-1.0.5.6/netin/stats/distributions.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2753 2023-04-15 22:08:18.000000 netin-1.0.5.6/netin/stats/ranking.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 08:34:31.523171 netin-1.0.5.6/netin/utils/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-14 21:38:11.000000 netin-1.0.5.6/netin/utils/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1075 2023-04-15 18:01:34.000000 netin-1.0.5.6/netin/utils/constants.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1221 2023-04-13 15:18:30.000000 netin-1.0.5.6/netin/utils/validator.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 08:34:31.523171 netin-1.0.5.6/netin/viz/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      425 2023-04-17 12:53:55.000000 netin-1.0.5.6/netin/viz/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      466 2023-04-17 10:09:00.000000 netin-1.0.5.6/netin/viz/constants.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)    26872 2023-04-19 13:08:56.000000 netin-1.0.5.6/netin/viz/handlers.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 08:34:31.523171 netin-1.0.5.6/netin.egg-info/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3774 2023-04-23 08:34:31.000000 netin-1.0.5.6/netin.egg-info/PKG-INFO
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1290 2023-04-23 08:34:31.000000 netin-1.0.5.6/netin.egg-info/SOURCES.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-23 08:34:31.000000 netin-1.0.5.6/netin.egg-info/dependency_links.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-16 07:00:51.000000 netin-1.0.5.6/netin.egg-info/not-zip-safe
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      418 2023-04-23 08:34:31.000000 netin-1.0.5.6/netin.egg-info/requires.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        6 2023-04-23 08:34:31.000000 netin-1.0.5.6/netin.egg-info/top_level.txt
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 08:34:31.523171 netin-1.0.5.6/requirements/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      182 2023-04-16 07:05:49.000000 netin-1.0.5.6/requirements/default.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)       60 2023-04-23 06:45:06.000000 netin-1.0.5.6/requirements/docs.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)       32 2023-04-15 10:35:15.000000 netin-1.0.5.6/requirements/test.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      104 2023-04-23 08:34:31.527171 netin-1.0.5.6/setup.cfg
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     4247 2023-04-16 07:47:09.000000 netin-1.0.5.6/setup.py
```

### Comparing `netin-1.0.5.5/LICENSE` & `netin-1.0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.5/PKG-INFO` & `netin-1.0.5.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netin
-Version: 1.0.5.5
+Version: 1.0.5.6
 Summary: Python package to study inequalities in social networks
 Home-page: https://github.com/CSHVienna/NetworkInequalities
 Author: Lisette Espín-Noboa
 Author-email: espin@csh.ac.at
 Maintainer: NetIn Developers
 Maintainer-email: netin-dev@googlegroups.com
 Keywords: Networks,Inequalities,Social Networks,Ranking,InferenceGraph Theory,Mathematics,network,undirected,discrete mathematics,math
@@ -45,14 +45,15 @@
 .. image:: https://img.shields.io/badge/NetworkX-3.1-blue.svg
     :target: https://networkx.org/
 
 .. image:: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg
     :target: https://creativecommons.org/licenses/by-nc-sa/4.0/
 
 - **Website:** https://www.networkinequality.com
+- **Documentation:** https://cshvienna.github.io/NetworkInequalities
 - **Source:** https://github.com/CSHVienna/NetworkInequalities
 - **Bug reports:** https://github.com/CSHVienna/NetworkInequalities/issues
 - **GitHub Discussions:** https://github.com/CSHVienna/NetworkInequalities/discussions
 - **Mailing list:** https://groups.google.com/forum/#!forum/netin-dev
 
 Simple examples
 ---------------
```

### Comparing `netin-1.0.5.5/README.rst` & `netin-1.0.5.6/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 .. image:: https://img.shields.io/badge/NetworkX-3.1-blue.svg
     :target: https://networkx.org/
 
 .. image:: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg
     :target: https://creativecommons.org/licenses/by-nc-sa/4.0/
 
 - **Website:** https://www.networkinequality.com
+- **Documentation:** https://cshvienna.github.io/NetworkInequalities
 - **Source:** https://github.com/CSHVienna/NetworkInequalities
 - **Bug reports:** https://github.com/CSHVienna/NetworkInequalities/issues
 - **GitHub Discussions:** https://github.com/CSHVienna/NetworkInequalities/discussions
 - **Mailing list:** https://groups.google.com/forum/#!forum/netin-dev
 
 Simple examples
 ---------------
```

### Comparing `netin-1.0.5.5/examples/notebooks/deleteme.py` & `netin-1.0.5.6/examples/notebooks/deleteme.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.5/netin/generators/dh.py` & `netin-1.0.5.6/netin/generators/dh.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.5/netin/generators/directed.py` & `netin-1.0.5.6/netin/generators/undirected.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,236 +1,230 @@
-from collections import defaultdict
-from typing import Union, Set
+from typing import Set
+from typing import Union
+from typing import Tuple
 
 import networkx as nx
 import numpy as np
 import powerlaw
 
-from netin.utils import constants as const
 from netin.utils import validator as val
 from .graph import Graph
 
 
-class DiGraph(nx.DiGraph, Graph):
+class UnDiGraph(Graph):
+    """Undirected graph base model.
+
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
+    Target nodes are selected depending on the chosen mechanism of edge formation:
+        - PA: Preferential attachment (in-degree) [1]
+        - PAH: Preferential attachment (in-degree) with homophily [2]
+        - PATC: Preferential attachment (in-degree) with triadic closure [3]
+        - PATCH: Preferential attachment (in-degree) with homophily and triadic closure
+
+    References
+    ----------
+    [1] A. L. Barabasi and R. Albert "Emergence of scaling in random networks", Science 286, pp 509-512, 1999.
+    [2] F. Karimi, M. Génois, C. Wagner, P. Singer, & M. Strohmaier, M "Homophily influences ranking of minorities in social networks", Scientific reports 8(1), 11077, 2018.
+    [3] P. Holme and B. J. Kim “Growing scale-free networks with tunable clustering” Phys. Rev. E 2002.
+    """
 
     ############################################################
     # Constructor
     ############################################################
 
-    def __init__(self, n: int, f_m: float, d: float, plo_M: float, plo_m: float, seed: object = None):
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
-        d: float
-            edge density (minimum=0, maximum=1)
-
-        plo_M: float
-            activity (out-degree power law exponent) majority group (minimum=1)
-
-        plo_m: float
-            activity (out-degree power law exponent) minority group (minimum=1)
-
-        seed: object
-            seed for random number generator
-
-        Notes
-        -----
-        The initialization is a directed with n nodes and no edges.
-        Then, everytime a node is selected as source, it gets connected to k target nodes.
-        Target nodes are selected via preferential attachment (in-degree), homophily (h_**),
-        and/or triadic closure (tc).
-
-        References
-        ----------
-        - [1] A. L. Barabasi and R. Albert "Emergence of scaling in random networks", Science 286, pp 509-512, 1999.
-        """
-        nx.DiGraph.__init__(self)
+    def __init__(self, n: int, k: int, f_m: float, seed: object = None):
         Graph.__init__(self, n=n, f_m=f_m, seed=seed)
-        self.d = d
-        self.plo_M = plo_M
-        self.plo_m = plo_m
-        self.in_degrees = None
-        self.out_degrees = None
-        self.activity = None
-        self.expected_number_of_edges = None
+        self.k = k
 
     ############################################################
     # Init
     ############################################################
 
     def _validate_parameters(self):
         """
-        Validates the parameters of the directed.
+        Validates the parameters of the undirected.
         """
-        Graph._validate_parameters(self)
-        val.validate_float(self.d, minimum=1. / (self.n * (self.n - 1)), maximum=1.)
-        val.validate_float(self.plo_M, minimum=1. + const.EPSILON)
-        val.validate_float(self.plo_m, minimum=1. + const.EPSILON)
+        super()._validate_parameters()
+        val.validate_int(self.k, minimum=1)
 
     def get_metadata_as_dict(self) -> dict:
         """
-        Returns metadata for a directed.
+        Returns metadata for a undirected.
         """
         obj = super().get_metadata_as_dict()
         obj.update({
-            'd': self.d,
-            'plo_M': self.plo_M,
-            'plo_m': self.plo_m,
+            'k': self.k,
         })
         return obj
 
     ############################################################
     # Generation
     ############################################################
 
-    def _initialize(self, class_attribute: str = 'm', class_values: list = None, class_labels: list = None):
-        Graph._initialize(self, class_attribute, class_values, class_labels)
-        self._init_edges()
-        self._init_activity()
-
-    def _init_edges(self):
-        self.expected_number_of_edges = int(round(self.d * self.n * (self.n - 1)))
-        self.in_degrees = np.zeros(self.n)
-        self.out_degrees = np.zeros(self.n)
-
-    def _init_activity(self):
-        act_M = powerlaw.Power_Law(parameters=[self.plo_M], discrete=True).generate_random(self.n_M)
-        act_m = powerlaw.Power_Law(parameters=[self.plo_m], discrete=True).generate_random(self.n_m)
-        self.activity = np.append(act_M, act_m)
-        if np.inf in self.activity:
-            self.activity[self.activity == np.inf] = 0.0
-            self.activity += 1
-        self.activity /= self.activity.sum()
-
-    def get_sources(self) -> np.array:
-        return np.random.choice(a=np.arange(self.n), size=self.expected_number_of_edges, replace=True, p=self.activity)
-
-    def get_target_probabilities(self, source: Union[None, int], target_set: Union[None, Set[int], np.array],
-                                 special_targets: Union[None, object, iter] = None) -> np.array:
-        pass
-
-    def get_target(self, source: int, edge_list: dict, **kwargs) -> Union[None, int]:
-        one_percent = self.n * 1 / 100.
-        if np.count_nonzero(self.out_degrees) > one_percent:
-            targets = [n for n in np.arange(self.n) if n not in edge_list[source]]
-        else:
-            targets = np.arange(self.n)
-        targets = np.delete(targets, np.where(targets == source))
+    def get_target(self, source: Union[None, int], targets: Union[None, Set[int]],
+                   special_targets: Union[None, object, iter]) -> int:
+        """
+        Picks a random target node based on preferential attachment.
 
-        if targets.shape[0] == 0:
-            return None
+        Parameters
+        ----------
+        special_targets : object
+            Special targets to be considered
+
+        source: int
+            Newly added node
+
+        targets: Set[int]
+            Potential target nodes in the undirected based on preferential attachment
 
-        probs = self.get_target_probabilities(source, targets, **kwargs)
-        return np.random.choice(a=targets, size=1, replace=False, p=probs)[0]
+        Returns
+        -------
+            int: Target node that an edge should be added to
+        """
+        # Collect probabilities to connect to each node in target_list
+        target_set = set([t for t in targets if t != source and t not in nx.neighbors(self, source)])
+        probs, target_set = self.get_target_probabilities(source, target_set, special_targets)
+        return np.random.choice(a=list(target_set), size=1, replace=False, p=probs)[0]
 
     def generate(self):
         """
-        A directed graph of n nodes is grown by attaching new nodes.
-        Each edge is either drawn by preferential attachment, homophily, or both
+        An undirected graph of n nodes is grown by attaching new nodes each with k edges.
+        Each edge is either drawn by preferential attachment, homophily, and/or triadic closure.
+
+        For triadic closure, a candidate is chosen uniformly at random from all triad-closing edges (of the new node).
+        Otherwise, or if there are no triads to close, edges are connected via preferential attachment and/or homophily.
 
         Homophily varies ranges from 0 (heterophilic) to 1 (homophilic), where 0.5 is neutral.
         Similarly, triadic closure varies from 0 (no triadic closure) to 1 (full triadic closure).
 
-        . DPA: A graph with h_mm = h_MM in [0.5, None] is a directed BA preferential attachment model.
-        . DH: A graph with h_mm not in [0.5, None] and h_MM not in [0.5, None] is a directed Erdos-Renyi with homophily.
-        . DPAH: A graph with h_mm not in [0.5, None] and h_MM not in [0.5, None] is a DPA model with homophily.
-
-        """
-        # 1. Init directed and nodes (assign class labels)
-        Graph.generate(self)
-
-        # 2. Iterate until reaching desired number of edges (edge density)
-        tries = 0
-        edge_list = defaultdict(list)
-        while self.number_of_edges() < self.expected_number_of_edges:
-            tries += 1
-            for source in self.get_sources():
-                target = self.get_target(source, edge_list)
-
-                if target is None:
-                    continue
-
-                if not self.has_edge(source, target):
-                    self.add_edge(source, target)
-                    self.in_degrees[target] += 1
-                    self.out_degrees[source] += 1
-                    edge_list[source].append(target)
-
-                if self.number_of_edges() >= self.expected_number_of_edges:
-                    break
-
-            # if no more edges can be added, break
-            if tries > const.MAX_TRIES_EDGE and self.number_of_edges() < self.expected_number_of_edges:
-                print(f">> Edge density ({nx.density(self)}) might differ from {self.d:.5f} (n={self.n}, f_m={self.f_m}"
-                      f"seed={self.seed}, plo_M={self.plo_M}, plo_m={self.plo_m}")
-                break
+        . PA:    An undirected graph with h_mm = h_MM in [0.5, None] and tc = 0 is a BA preferential attachment model.
+        . PAH:   An undirected graph with h_mm not in [0.5, None] and h_MM not in [0.5, None] and tc = 0 is a PA model
+                 with homophily.
+        . PATC:  An undirected graph with h_mm = h_MM in [0.5, None] and tc > 0 is a PA model with triadic closure.
+        . PATCH: An undirected graph with h_mm not in [0.5, None] and h_MM not in [0.5, None] and tc > 0 is a PA model
+                 with homophily and triadic closure.
+
+        """
+        # 1. Init an undirected graph and nodes (assign class labels)
+        super().generate()
+
+        # 2. Iterate until n nodes are added (starts with k pre-existing, unconnected nodes)
+        for source in self.node_list[self.k:]:
+            targets = set(range(source))  # targets via preferential attachment
+            special_targets = self.get_special_targets(source)
+
+            for idx_target in range(self.k):
+                # Choose next target
+                target = self.get_target(source, targets, special_targets)
+
+                special_targets = self.update_special_targets(idx_target, source, target, targets, special_targets)
+
+                # Finally add edge to undirected
+                self.add_edge(source, target)
+
+                # Call event handlers if present
+                self.on_edge_added(source, target)
 
         self._terminate()
 
     ############################################################
-    # Calculations
+    # Getters and Setters
     ############################################################
 
-    def info_params(self):
-        print(f'd: {self.d} (expected edges: {self.expected_number_of_edges})')
-        print(f'plo_M: {self.plo_M}')
-        print(f'plo_m: {self.plo_m}')
-
-    def info_computed(self):
-        for metric in ['in_degree', 'out_degree']:
-            fit_M, fit_m = self.fit_powerlaw(metric)
-            print(f"- Powerlaw fit ({metric}):")
-            print(f"- {self.get_majority_label()}: alpha={fit_M.power_law.alpha}, sigma={fit_M.power_law.sigma}, "
-                  f"min={fit_M.power_law.xmin}, max={fit_M.power_law.xmax}")
-            print(f"- {self.get_minority_label()}: alpha={fit_m.power_law.alpha}, sigma={fit_m.power_law.sigma}, "
-                  f"min={fit_m.power_law.xmin}, max={fit_m.power_law.xmax}")
+    def get_expected_number_of_edges(self) -> int:
+        """
+        Computes and returns the expected number of edges based on minimum degree `k` and number of nodes `n`
 
-    def fit_powerlaw(self, metric: str) -> powerlaw.Fit:
-        vM = self.get_majority_value()
-        dist_fnc = self.in_degree if metric == 'in_degree' else self.out_degree
-        dM = [d for n, d in dist_fnc if self.nodes[n][self.class_attribute] == vM]
-        dm = [d for n, d in dist_fnc if self.nodes[n][self.class_attribute] != vM]
+        Returns
+        -------
+            int
+                Expected number of edges
+        """
+        return (self.get_expected_number_of_nodes() * self.get_expected_minimum_degree()) - \
+            (self.get_expected_minimum_degree() ** self.get_expected_minimum_degree())
 
-        fit_M = powerlaw.Fit(data=dM, discrete=True, xmin=min(dM), xmax=max(dM), verbose=False)
-        fit_m = powerlaw.Fit(data=dm, discrete=True, xmin=min(dm), xmax=max(dm), verbose=False)
-        return fit_M, fit_m
+    def get_expected_minimum_degree(self) -> int:
+        """
+        Returns the expected minimum degree of the graph (`k`, the input parameter)
 
-    def calculate_in_degree_powerlaw_exponents(self) -> (float, float):
-        fit_M, fit_m = self.fit_powerlaw(metric='in_degree')
-        pl_M = fit_M.power_law.alpha
-        pl_m = fit_m.power_law.alpha
-        return pl_M, pl_m
+        Returns
+        -------
+            int
+                Expected minimum degree
+        """
 
-    def calculate_out_degree_powerlaw_exponents(self) -> (float, float):
-        fit_M, fit_m = self.fit_powerlaw(metric='out_degree')
-        pl_M = fit_M.power_law.alpha
-        pl_m = fit_m.power_law.alpha
-        return pl_M, pl_m
+        return self.k
 
     ############################################################
-    # Getters and setters
+    # Calculations
     ############################################################
 
-    def get_expected_number_of_edges(self) -> int:
-        return self.expected_number_of_edges
+    def info_params(self):
+        """
+        Shows the parameters of the model.
+        """
+        print('k: {}'.format(self.k))
 
-    def get_expected_density(self) -> float:
-        return self.d
+    def info_computed(self):
+        """
+        Shows the computed properties of the graph.
+        """
+        fit_M, fit_m = self.fit_degree_powerlaw()
+        print(f"- Powerlaw fit (degree):")
+        print(f"- {self.get_majority_label()}: alpha={fit_M.power_law.alpha}, "
+              f"sigma={fit_M.power_law.sigma}, "
+              f"min={fit_M.power_law.xmin}, max={fit_M.power_law.xmax}")
+        print(f"- {self.get_minority_label()}: alpha={fit_m.power_law.alpha}, "
+              f"sigma={fit_m.power_law.sigma}, "
+              f"min={fit_m.power_law.xmin}, max={fit_m.power_law.xmax}")
+
+    def fit_degree_powerlaw(self) -> Tuple[powerlaw.Fit,powerlaw.Fit]:
+        """
+        Returns the powerlaw fit of the degree distribution to a powerlaw for the majority and minority class.
+
+        Returns
+        -------
+        fit_M : powerlaw.Fit
+            Powerlaw fit for the majority class
+        fit_m: powerlaw.Fit
+            Powerlaw fit for the minority class
+        """
+        vM = self.get_majority_value()
+        dM = [d for n, d in self.degree() if self.nodes[n][self.class_attribute] == vM]
+        dm = [d for n, d in self.degree() if self.nodes[n][self.class_attribute] != vM]
 
-    def get_expected_powerlaw_out_degree_majority(self):
-        return self.plo_M
+        fit_M = powerlaw.Fit(data=dM, discrete=True, xmin=min(dM), xmax=max(dM))
+        fit_m = powerlaw.Fit(data=dm, discrete=True, xmin=min(dm), xmax=max(dm))
+        return fit_M, fit_m
 
-    def get_expected_powerlaw_out_degree_minority(self):
-        return self.plo_m
+    def calculate_degree_powerlaw_exponents(self) -> Tuple[float, float]:
+        """
+        Returns the powerlaw exponents for the majority and minority class.
 
-    def get_activity_distribution(self):
-        return self.activity
+        Returns
+        -------
+        pl_M : float
+            Powerlaw exponent for the majority class
+        pl_m: float
+            Powerlaw exponent for the minority class
+        """
+        fit_M, fit_m = self.fit_degree_powerlaw()
+        pl_M = fit_M.power_law.alpha
+        pl_m = fit_m.power_law.alpha
+        return pl_M, pl_m
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `netin-1.0.5.5/netin/generators/dpa.py` & `netin-1.0.5.6/netin/generators/dpa.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.5/netin/generators/graph.py` & `netin-1.0.5.6/netin/generators/directed.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,375 +1,366 @@
-import time
-from collections import Counter
-from typing import Union, Set
+from collections import defaultdict
+from typing import Union, Set, Tuple
 
 import networkx as nx
 import numpy as np
-import pandas as pd
-from pqdm.threads import pqdm
+import powerlaw
 
 from netin.utils import constants as const
 from netin.utils import validator as val
+from .graph import Graph
 
 
-class Graph(nx.Graph):
+class DiGraph(nx.DiGraph, Graph):
 
-    ############################################################
-    # Constructor
-    ############################################################
+    """Directed graph base model.
 
-    def __init__(self, n: int, f_m: float, seed: object = None):
-        """
-        Bi-populated network
+    Parameters
+    ----------
+    n: int
+        number of nodes (minimum=2)
 
-        Parameters
-        ----------
-        n: int
-            number of nodes (minimum=2)
+    d: float
+        edge density (minimum=0, maximum=1)
 
-        f_m: float
-            fraction of minorities (minimum=1/n, maximum=(n-1)/n)
+    f_m: float
+        fraction of minorities (minimum=1/n, maximum=(n-1)/n)
 
-        seed: object
-            seed for random number generator
+    plo_M: float
+        activity (out-degree power law exponent) majority group (minimum=1)
 
-        attr: dict
-            attributes to add to graph as key=value pairs
-
-        Notes
-        -----
-        The initialization is a graph with n nodes: f_m are minorities and (1-f_m) are majority.
-        Source nodes are selected one-by-one (if undirected) and based on their activity (if directed).
-        Target nodes are selected via preferential attachment (in-degree) [1].
-        Other target mechanisms:
-        - homophily (h_**),
-        - triadic closure (tc).
+    plo_m: float
+        activity (out-degree power law exponent) minority group (minimum=1)
 
-        References
-        ----------
-        - [1] A. L. Barabasi and R. Albert "Emergence of scaling in random networks", Science 286, pp 509-512, 1999.
-        """
-        nx.Graph.__init__(self)
-        self.n = n
-        self.f_m = f_m
-        self.seed = seed
-        self.n_m = 0
-        self.n_M = 0
-        self.model_name = None
-        self.class_attribute = None
-        self.class_values = None
-        self.class_labels = None
-        self.node_list = None
-        self.node_labels = None
-        self._gen_start_time = None
-        self._gen_duration = None
+    seed: object
+        seed for random number generator
+
+    Notes
+    -----
+    The initialization is a directed with n nodes and no edges.
+    Source nodes are selected based on their activity given by plo_M (if majority) or plo_m (if minority), see [1].
+    Target nodes are selected depending on the chosen mechanism of edge formation:
+        - DPAH: preferential attachment (in-degree) and homophily (h**) [1]
+        - DPA: preferential attachment (in-degree)
+        - DH: homophily (h**)
+
+    References
+    ----------
+    [1] L. Espín-Noboa, C. Wagner, M. Strohmaier, & F. Karimi "Inequality and inequity in network-based ranking and recommendation algorithms" Scientific reports 12(1), 1-14, 2022.
+    """
 
     ############################################################
-    # Init
+    # Constructor
     ############################################################
 
-    def _infer_model_name(self):
-        pass
+    def __init__(self, n: int, f_m: float, d: float, plo_M: float, plo_m: float, seed: object = None):
+        nx.DiGraph.__init__(self)
+        Graph.__init__(self, n=n, f_m=f_m, seed=seed)
+        self.d = d
+        self.plo_M = plo_M
+        self.plo_m = plo_m
+        self.in_degrees = None
+        self.out_degrees = None
+        self.activity = None
+        self.expected_number_of_edges = None
+
+    ############################################################
+    # Init
+    ############################################################
 
     def _validate_parameters(self):
         """
-        Validates the parameters of the graph.
+        Validates the parameters of the directed.
         """
-        val.validate_int(self.n, minimum=2)
-        val.validate_float(self.f_m, minimum=1 / self.n, maximum=(self.n - 1) / self.n)
-        self.seed = self.seed if self.seed is not None else np.random.randint(0, 2 ** 32)
-
-    def _set_class_info(self, class_attribute: str = 'm', class_values=None, class_labels=None):
-        if class_labels is None:
-            class_labels = [const.MAJORITY_LABEL, const.MINORITY_LABEL]
-        if class_values is None:
-            class_values = [0, 1]
-        self.set_class_attribute(class_attribute)
-        self.set_class_values(class_values)
-        self.set_class_labels(class_labels)
+        Graph._validate_parameters(self)
+        val.validate_float(self.d, minimum=1. / (self.n * (self.n - 1)), maximum=1.)
+        val.validate_float(self.plo_M, minimum=1. + const.EPSILON)
+        val.validate_float(self.plo_m, minimum=1. + const.EPSILON)
 
     def get_metadata_as_dict(self) -> dict:
         """
-        Returns metadata for a graph.
+        Returns metadata for a directed.
         """
-        obj = {'model': self.get_model_name(),
-               'class_attribute': self.get_class_attribute(),
-               'class_values': self.get_class_values(),
-               'class_labels': self.get_class_labels(),
-               'n': self.n,
-               'f_m': self.f_m,
-               'seed': self.seed}
+        obj = super().get_metadata_as_dict()
+        obj.update({
+            'd': self.d,
+            'plo_M': self.plo_M,
+            'plo_m': self.plo_m,
+        })
         return obj
 
     ############################################################
-    # Getters & Setters
+    # Generation
     ############################################################
 
-    def set_expected_number_of_nodes(self, n):
-        self.n = n
+    def _initialize(self, class_attribute: str = 'm', class_values: list = None, class_labels: list = None):
+        """
+        Initializes the model.
 
-    def get_expected_number_of_nodes(self):
-        return self.n
+        Parameters
+        ----------
+        class_attribute: str
+            name of the attribute that represents the class
 
-    def get_expected_number_of_edges(self):
-        pass
+        class_values: list
+            values of the class attribute
 
-    def set_expected_fraction_of_minorities(self, f_m):
-        self.f_m = f_m
+        class_labels: list
+            labels of the class attribute mapping the class_values.
+        """
+        Graph._initialize(self, class_attribute, class_values, class_labels)
+        self._init_edges()
+        self._init_activity()
 
-    def get_expected_fraction_of_minorities(self):
-        return self.f_m
+    def _init_edges(self):
+        """
+        Initializes the expected number of edges based on the number of nodes and density of the graph (input param).
+        It also initializes the in- and out-degrees of the nodes.
+        """
+        self.expected_number_of_edges = int(round(self.d * self.n * (self.n - 1)))
+        self.in_degrees = np.zeros(self.n)
+        self.out_degrees = np.zeros(self.n)
 
-    def set_seed(self, seed):
-        self.seed = seed
+    def _init_activity(self):
+        """
+        Intializes the level of activity for each node based on the power law exponents (input param).
+        """
+        act_M = powerlaw.Power_Law(parameters=[self.plo_M], discrete=True).generate_random(self.n_M)
+        act_m = powerlaw.Power_Law(parameters=[self.plo_m], discrete=True).generate_random(self.n_m)
+        self.activity = np.append(act_M, act_m)
+        if np.inf in self.activity:
+            self.activity[self.activity == np.inf] = 0.0
+            self.activity += 1
+        self.activity /= self.activity.sum()
 
-    def get_seed(self):
-        return self.seed
+    def get_sources(self) -> np.array:
+        """
+        Returns a random sample with replacement of nodes to be used as source nodes.
+        The sample has the length of the expected number of edges, and the probability of each node to be selected is
+        based on its activity.
 
-    def set_model_name(self, model_name):
-        self.model_name = model_name
+        Returns
+        -------
+        np.array
+            array of source nodes
+        """
+        return np.random.choice(a=np.arange(self.n), size=self.expected_number_of_edges, replace=True, p=self.activity)
 
-    def get_model_name(self):
-        return self.model_name
+    def get_target_probabilities(self, source: Union[None, int], target_set: Union[None, Set[int], np.array],
+                                 special_targets: Union[None, object, iter] = None) -> np.array:
+        pass
 
-    def set_class_attribute(self, class_attribute):
-        self.class_attribute = class_attribute
+    def get_target(self, source: int, edge_list: dict, **kwargs) -> Union[None, int]:
+        """
+        Returns a target node for a given source node.
 
-    def get_class_attribute(self):
-        return self.class_attribute
+        Parameters
+        ----------
+        source: int
+            source node
 
-    def set_class_values(self, class_values):
-        self.class_values = class_values
+        edge_list: dict
+            dictionary of edges
 
-    def get_class_values(self):
-        return self.class_values
+        kwargs: dict
+            additional parameters
 
-    def set_class_labels(self, class_labels):
-        self.class_labels = class_labels
+        Returns
+        -------
+        Union[None, int]
+            target node
+        """
+        one_percent = self.n * 1 / 100.
+        if np.count_nonzero(self.out_degrees) > one_percent:
+            targets = [n for n in np.arange(self.n) if n not in edge_list[source]]
+        else:
+            targets = np.arange(self.n)
+        targets = np.delete(targets, np.where(targets == source))
 
-    def get_class_labels(self):
-        return self.class_labels
+        if targets.shape[0] == 0:
+            return None
 
-    def get_class_value(self, node):
-        return self.nodes[node][self.class_attribute]
+        probs = self.get_target_probabilities(source, targets, **kwargs)
+        return np.random.choice(a=targets, size=1, replace=False, p=probs)[0]
 
-    def get_class_label(self, node):
-        idx = self.class_values.index(self.nodes[node][self.class_attribute])
-        return self.class_labels[idx]
+    def generate(self):
+        """
+        A directed graph of n nodes is grown by attaching new nodes.
+        Source nodes are selected randomly with replacement based on their activity.
+        Each target node drawn based on the chosen mechanism of edge formation [1].
+
+        - DPA: A graph with h_mm = h_MM in [0.5, None] is a directed BA preferential attachment model.
+        - DH: A graph with h_mm not in [0.5, None] and h_MM not in [0.5, None] is a directed Erdos-Renyi with homophily.
+        - DPAH: A graph with h_mm not in [0.5, None] and h_MM not in [0.5, None] is a DPA model with homophily.
 
-    def get_majority_value(self) -> int:
-        return const.MAJORITY_VALUE
+        References
+        ----------
+        [1] L. Espín-Noboa, C. Wagner, M. Strohmaier, & F. Karimi "Inequality and inequity in network-based ranking and recommendation algorithms" Scientific reports 12(1), 1-14, 2022.
 
-    def get_minority_value(self) -> int:
-        return const.MINORITY_VALUE
+        """
+        # 1. Init directed and nodes (assign class labels)
+        Graph.generate(self)
 
-    def get_majority_label(self) -> int:
-        return const.MAJORITY_LABEL
+        # 2. Iterate until reaching desired number of edges (edge density)
+        tries = 0
+        edge_list = defaultdict(list)
+        while self.number_of_edges() < self.expected_number_of_edges:
+            tries += 1
+            for source in self.get_sources():
+                target = self.get_target(source, edge_list)
+
+                if target is None:
+                    continue
+
+                if not self.has_edge(source, target):
+                    self.add_edge(source, target)
+                    self.in_degrees[target] += 1
+                    self.out_degrees[source] += 1
+                    edge_list[source].append(target)
+
+                if self.number_of_edges() >= self.expected_number_of_edges:
+                    break
+
+            # if no more edges can be added, break
+            if tries > const.MAX_TRIES_EDGE and self.number_of_edges() < self.expected_number_of_edges:
+                print(f">> Edge density ({nx.density(self)}) might differ from {self.d:.5f} (n={self.n}, f_m={self.f_m}"
+                      f"seed={self.seed}, plo_M={self.plo_M}, plo_m={self.plo_m}")
+                break
 
-    def get_minority_label(self) -> int:
-        return const.MINORITY_LABEL
+        self._terminate()
 
     ############################################################
-    # Generation
+    # Calculations
     ############################################################
 
-    def _initialize(self, class_attribute: str = 'm', class_values: list = None, class_labels: list = None):
+    def info_params(self):
         """
-        Initializes the random seed and the graph metadata.
+        Shows the (input) parameters of the graph.
         """
-        np.random.seed(self.seed)
-        self._validate_parameters()
-        self._init_graph(class_attribute, class_values, class_labels)
-        self._init_nodes()
+        print(f'd: {self.d} (expected edges: {self.expected_number_of_edges})')
+        print(f'plo_M: {self.plo_M}')
+        print(f'plo_m: {self.plo_m}')
 
-    def _init_graph(self, class_attribute: str = 'm', class_values: list = None, class_labels: list = None):
+    def info_computed(self):
+        """
+        Shows the computer properties of the graph.
         """
-        Sets the name of the model, class information, and the graph metadata.
+        for metric in ['in_degree', 'out_degree']:
+            fit_M, fit_m = self.fit_powerlaw(metric)
+            print(f"- Powerlaw fit ({metric}):")
+            print(f"- {self.get_majority_label()}: alpha={fit_M.power_law.alpha}, sigma={fit_M.power_law.sigma}, "
+                  f"min={fit_M.power_law.xmin}, max={fit_M.power_law.xmax}")
+            print(f"- {self.get_minority_label()}: alpha={fit_m.power_law.alpha}, sigma={fit_m.power_law.sigma}, "
+                  f"min={fit_m.power_law.xmin}, max={fit_m.power_law.xmax}")
+
+    def fit_powerlaw(self, metric: str) -> powerlaw.Fit:
+        """
+        Fits a power law to the distribution given by 'metric' (the in- or out-degree of nodes in the graph).
 
         Parameters
         ----------
-        class_attribute: str
-            name of the class attribute
+        metric: str
+            metric to fit power law to
 
-        class_values: list
-            list of class values
-
-        class_labels: list
-            list of class labels
+        Returns
+        -------
+        powerlaw.Fit
+            power law fit
         """
-        self._infer_model_name()
-        self._set_class_info(class_attribute, class_values, class_labels)
-        self.graph = self.get_metadata_as_dict()
+        # @TODO: validate if metric is not in_degree or out_degree
+        vM = self.get_majority_value()
+        dist_fnc = self.in_degree if metric == 'in_degree' else self.out_degree
+        dM = [d for n, d in dist_fnc if self.nodes[n][self.class_attribute] == vM]
+        dm = [d for n, d in dist_fnc if self.nodes[n][self.class_attribute] != vM]
+
+        fit_M = powerlaw.Fit(data=dM, discrete=True, xmin=min(dM), xmax=max(dM), verbose=False)
+        fit_m = powerlaw.Fit(data=dm, discrete=True, xmin=min(dm), xmax=max(dm), verbose=False)
+        return fit_M, fit_m
 
-    def _init_nodes(self):
-        """
-        Initializes the list of nodes with their respective labels.
+    def calculate_in_degree_powerlaw_exponents(self) -> Tuple[float, float]:
         """
-        self.node_list = np.arange(self.n)
-        self.n_M = int(round(self.n * (1 - self.f_m)))
-        self.n_m = self.n - self.n_M
-        minorities = np.random.choice(self.node_list, self.n_m, replace=False)
-        self.node_labels = {n: int(n in minorities) for n in self.node_list}
-
-    def get_special_targets(self, source: int) -> object:
-        pass
+        Returns the power law exponents for the in-degree distribution of the majority and minority class.
 
-    def get_potential_nodes_to_connect(self, source: int, targets: Set[int]) -> Set[int]:
-        return set([t for t in targets if t != source and t not in nx.neighbors(self, source)])
-
-    def get_target_probabilities(self, source: Union[None, int], target_set: Union[None, Set[int]],
-                                 special_targets: Union[None, object, iter] = None) -> tuple[np.array, set[int]]:
-        # Random (erdos renyi)
-        probs = np.ones(len(target_set))
-        probs /= probs.sum()
-        return probs, target_set
-
-    def get_target(self, source: Union[None, int], targets: Union[None, Set[int]],
-                   special_targets: Union[None, object, iter]) -> int:
-        pass
-
-    def update_special_targets(self, idx_target: int, source: int, target: int, targets: Set[int],
-                               special_targets: Union[None, object, iter]):
-        pass
-
-    def on_edge_added(self, source: int, target: int):
-        pass
-
-    def generate(self):
-        self._gen_start_time = time.time()
-
-        # init graph and nodes
-        self._initialize()
-        self.add_nodes_from(self.node_list)
-        nx.set_node_attributes(self, self.node_labels, self.class_attribute)
+        Returns
+        -------
+        Tuple[float, float]
+            power law exponents for the in-degree distribution of the majority and minority class
+        """
+        fit_M, fit_m = self.fit_powerlaw(metric='in_degree')
+        pl_M = fit_M.power_law.alpha
+        pl_m = fit_m.power_law.alpha
+        return pl_M, pl_m
 
-        # iterate
-        # for each source_node, get target (based on specific mechanisms), then add edge, update special targets
+    def calculate_out_degree_powerlaw_exponents(self) -> Tuple[float, float]:
+        """
+        Returns the power law exponents for the out-degree distribution of the majority and minority class.
 
-    def _terminate(self):
-        self._gen_duration = time.time() - self._gen_start_time
+        Returns
+        -------
+        Tuple[float, float]
+            power law exponents for the out-degree distribution of the majority and minority class
+        """
+        fit_M, fit_m = self.fit_powerlaw(metric='out_degree')
+        pl_M = fit_M.power_law.alpha
+        pl_m = fit_m.power_law.alpha
+        return pl_M, pl_m
 
     ############################################################
-    # Calculations
+    # Getters and setters
     ############################################################
 
-    def info_params(self):
-        pass
+    def get_expected_number_of_edges(self) -> int:
+        """
+        Returns the expected number of edges based on number of nodes and edge density.
 
-    def info_computed(self):
-        pass
+        Returns
+        -------
+        int
+            expected number of edges
+        """
+        return self.expected_number_of_edges
 
-    def info(self, **kwargs):
+    def get_expected_density(self) -> float:
         """
+        Returns the expected edge density (d, the input parameter).
 
         Returns
         -------
-        object
+        float
+            expected edge density
         """
-        print("=== Params ===")
-        print('n: {}'.format(self.n))
-        print('f_m: {}'.format(self.f_m))
-        self.info_params()
-        print('seed: {}'.format(self.seed))
-
-        print("=== Model ===")
-        print('Model: {}'.format(self.get_model_name()))
-        print('Class attribute: {}'.format(self.get_class_attribute()))
-        print('Class values: {}'.format(self.get_class_values()))
-        print('Class labels: {}'.format(self.get_class_labels()))
-        print('Generation time: {} (secs)'.format(self._gen_duration))
-
-        print("=== Computed ===")
-        print(f'- is directed: {self.is_directed()}')
-        print(f'- number of nodes: {self.number_of_nodes()}')
-        print(f'- number of edges: {self.number_of_edges()}')
-        print(f'- minimum degree: {self.calculate_minimum_degree()}')
-        print(f'- fraction of minority: {self.calculate_fraction_of_minority()}')
-        print(f'- edge-type counts: {self.count_edges_types()}')
-        print(f"- density: {nx.density(self)}")
-        try:
-            print(f"- diameter: {nx.diameter(self)}")
-        except Exception as ex:
-            print(f"- diameter: <{ex}>")
-        try:
-            print(f"- average shortest path length: {nx.average_shortest_path_length(self)}")
-        except Exception as ex:
-            print(f"- average shortest path length: <{ex}>")
-        print(f"- average degree: {sum([d for n, d in self.degree]) / self.number_of_nodes()}")
-        print(f"- degree assortativity: {nx.degree_assortativity_coefficient(self)}")
-        print(f"- attribute assortativity ({self.class_attribute}): "
-              f"{nx.attribute_assortativity_coefficient(self, self.class_attribute)}")
-        print(f"- transitivity: {nx.transitivity(self)}")
-        print(f"- average clustering: {nx.average_clustering(self)}")
-        self.info_computed()
-
-    def calculate_minimum_degree(self):
-        return min([d for n, d in self.degree])
-
-    def calculate_fraction_of_minority(self):
-        return sum([1 for n, obj in self.nodes(data=True) if obj[self.class_attribute] == self.class_values[
-            self.class_labels.index(const.MINORITY_LABEL)]]) / self.number_of_nodes()
-
-    def count_edges_types(self):
-        return Counter([f"{self.class_labels[self.nodes[e[0]][self.class_attribute]]}"
-                        f"{self.class_labels[self.nodes[e[1]][self.class_attribute]]}"
-                        for e in self.edges])
+        return self.d
 
-    ############################################################
-    # Metadata
-    ############################################################
+    def get_expected_powerlaw_out_degree_majority(self) -> float:
+        """
+        Returns the expected power law exponent for the out-degree distribution of the majority class
+        (plo_M, the input parameter).
 
-    def compute_node_stats(self, metric, **kwargs):
-        values = None
+        Returns
+        -------
+        float
+            expected power law exponent for the out-degree distribution of the majority class
+        """
+        return self.plo_M
 
-        # list of tuples (node, value)
-        if metric == 'degree':
-            values = self.degree(self.node_list, **kwargs) if not self.is_directed() else None
-        if metric == 'in_degree':
-            values = self.in_degree(self.node_list, **kwargs) if self.is_directed() else None
-        if metric == 'out_degree':
-            values = self.out_degree(self.node_list, **kwargs) if self.is_directed() else None
-        if metric == 'eigenvector':
-            values = nx.eigenvector_centrality_numpy(self, **kwargs)
-
-        # dict of node -> value
-        if metric == 'clustering':
-            values = nx.clustering(self, self.node_list, **kwargs)
-        if metric == 'betweenness':
-            values = nx.betweenness_centrality(self, **kwargs)
-        if metric == 'closeness':
-            if isinstance(self, nx.DiGraph):
-                values = nx.closeness_centrality(nx.DiGraph(self), **kwargs)
-            else:
-                values = nx.closeness_centrality(self, **kwargs)
-        if metric == 'pagerank':
-            values = nx.pagerank(self, **kwargs)
-
-        return [values[n] for n in self.node_list] if values is not None else np.nan
-
-    def get_node_metadata_as_dataframe(self, include_graph_metadata=False, n_jobs=1):
-        cols = ['node', 'class_label']
-        obj = {'node': self.node_list,
-               'class_label': [self.get_class_label(n) for n in self.node_list]}
-
-        # include graph metadata
-        if include_graph_metadata:
-            n = self.number_of_nodes()
-            newcols = [c for c in self.graph.keys() if c not in ['class_attribute', 'class_values', 'class_labels']]
-            obj.update({c: self.graph[c] for c in newcols})
-            cols.extend(newcols)
-
-        # include metrics
-        column_values = pqdm(const.VALID_METRICS, self.compute_node_stats, n_jobs=n_jobs)
-        obj.update({col: values for col, values in zip(const.VALID_METRICS, column_values)})
-        cols.extend(const.VALID_METRICS)
-
-        # create dataframe
-        df = pd.DataFrame(obj, columns=cols, index=self.node_list)
-        df.name = self.get_model_name()
-
-        # add ranking values
-        for metric in const.VALID_METRICS:
-            ncol = f'{metric}_rank'
-            df.loc[:, ncol] = df.loc[:, metric].rank(ascending=False, pct=True, method='dense')
+    def get_expected_powerlaw_out_degree_minority(self):
+        """
+        Returns the expected power law exponent for the out-degree distribution of the minority class
+        (plo_m, the input parameter).
 
-        return df
+        Returns
+        -------
+        float
+            expected power law exponent for the out-degree distribution of the minority class
+        """
+        return self.plo_m
+
+    def get_activity_distribution(self) -> np.array:
+        """
+        Returns the activity distribution of all the nodes in the graph.
+
+        Returns
+        -------
+        np.array
+            activity distribution of all the nodes in the graph
+        """
+        return self.activity
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `netin-1.0.5.5/netin/generators/h.py` & `netin-1.0.5.6/netin/generators/h.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.5/netin/generators/pa.py` & `netin-1.0.5.6/netin/generators/pa.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.5/netin/generators/pah.py` & `netin-1.0.5.6/netin/generators/pah.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,55 +1,59 @@
-from typing import Union, Set
+from typing import Union, Set, Tuple
 
 import numpy as np
 from sympy import symbols
 from sympy import Eq
 from sympy import solve
 
 from netin.utils import constants as const
 from netin.generators.h import Homophily
 from .pa import PA
 
 
 class PAH(PA, Homophily):
+    """Creates a new PAH instance.
+
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
+    h_MM: float
+        homophily (similarity) between majority nodes (minimum=0, maximum=1.)
+
+    h_mm: float
+        homophily (similarity) between minority nodes (minimum=0, maximum=1.)
+
+    seed: object
+        seed for random number generator
+
+    Notes
+    -----
+    The initialization is an undirected with n nodes, where f_m are the minority.
+    Then, everytime a node is selected as source, it gets connected to k target nodes.
+    Target nodes are selected via preferential attachment (in-degree) and homophily (h_**).
+    This model is based on [1] known as the "Barabasi model with homophily" or "BA Homophily".
+
+    References
+    ----------
+    [1] F. Karimi, M. Génois, C. Wagner, P. Singer, & M. Strohmaier, M "Homophily influences ranking of minorities in social networks", Scientific reports 8(1), 11077, 2018.
+    """
 
     ############################################################
     # Constructor
     ############################################################
 
     def __init__(self, n: int, k: int, f_m: float, h_MM: float, h_mm: float, seed: object = None):
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
-        h_MM: float
-            homophily (similarity) between majority nodes (minimum=0, maximum=1.)
-
-        h_mm: float
-            homophily (similarity) between minority nodes (minimum=0, maximum=1.)
-
-        Notes
-        -----
-        The initialization is a undirected with n nodes and no edges.
-        Then, everytime a node is selected as source, it gets connected to k target nodes.
-        Target nodes are selected via preferential attachment (in-degree), and homophily (h_**)
-
-        References
-        ----------
-        - [1] A. L. Barabasi and R. Albert "Emergence of scaling in random networks", Science 286, pp 509-512, 1999.
-        """
         PA.__init__(self, n=n, k=k, f_m=f_m, seed=seed)
         Homophily.__init__(self, n=n, f_m=f_m, h_MM=h_MM, h_mm=h_mm, seed=seed)
 
     ############################################################
     # Init
     ############################################################
 
@@ -63,46 +67,107 @@
         """
         Validates the parameters of the undirected.
         """
         PA._validate_parameters(self)
         Homophily._validate_parameters(self)
 
     def get_metadata_as_dict(self) -> dict:
+        """
+        Returns the metadata (parameters) of the model as a dictionary.
+
+        Returns
+        -------
+        dict
+            metadata of the model
+        """
         obj = PA.get_metadata_as_dict(self)
         obj.update(Homophily.get_metadata_as_dict(self))
         return obj
 
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
         PA._initialize(self, class_attribute, class_values, class_labels)
         Homophily._initialize(self, class_attribute, class_values, class_labels)
 
     def get_target_probabilities(self, source: Union[None, int], target_set: Union[None, Set[int]],
                                  special_targets: Union[None, object, iter] = None) -> tuple[np.array, set[int]]:
+        """
+        Returns the probabilities of selecting a target node from a set of nodes based on the preferential attachment
+        and homophily.
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
+            probabilities of selecting a target node from a set of nodes, and the set of target nodes
+        """
         probs = np.array([self.get_homophily_between_source_and_target(source, target) *
                           (self.degree(target) + const.EPSILON) for target in target_set])
         probs /= probs.sum()
         return probs, target_set
 
     ############################################################
     # Calculations
     ############################################################
 
     def info_params(self):
+        """
+        Shows the parameters of the model.
+        """
         PA.info_params(self)
         Homophily.info_params(self)
 
     def info_computed(self):
+        """
+        Shows the computed properties of the graph.
+        """
         PA.info_computed(self)
         Homophily.info_computed(self)
 
-    def infer_homophily_values(self) -> (float, float):
+    def infer_homophily_values(self) -> Tuple[float, float]:
+        """
+        Infers the level of homopolily using the analutical solution of the model [1].
+
+        Returns
+        -------
+        tuple[float, float]
+            homophily between majority nodes, and homophily between minority nodes
+
+        References
+        ----------
+        [1] F. Karimi, M. Génois, C. Wagner, P. Singer, & M. Strohmaier, M "Homophily influences ranking of minorities in social networks", Scientific reports 8(1), 11077, 2018.
+
+        """
         f_m = self.calculate_fraction_of_minority()
         f_M = 1 - f_m
 
         e = self.count_edges_types()
         e_MM = e['MM']
         e_mm = e['mm']
         M = e['MM'] + e['mm'] + e['Mm'] + e['mM']
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `netin-1.0.5.5/netin/generators/patc.py` & `netin-1.0.5.6/netin/generators/patc.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,20 +74,25 @@
     ############################################################
 
     def info_params(self):
         PA.info_params(self)
         TriadicClosure.info_params(self)
 
     def get_special_targets(self, source: int) -> object:
-        """
-        Return an empty dictionary (source node ids)
+        """Return an empty dictionary (source node ids)
+
         Parameters
         ----------
-        source: int
-            Newly added node
+        source : int
+             Newly added node
+
+        Returns
+        -------
+        object
+            Empty dictionary (source node ids)
         """
         return TriadicClosure.get_special_targets(self, source)
 
     def get_target_probabilities(self, source: Union[None, int], target_set: Union[None, Set[int]],
                                  special_targets: Union[None, object, iter] = None) -> tuple[np.array, set[int]]:
         return TriadicClosure.get_target_probabilities(self, source, target_set, special_targets)
```

### Comparing `netin-1.0.5.5/netin/generators/patch.py` & `netin-1.0.5.6/netin/generators/patch.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-from typing import Union, Set
+from typing import Union, Set, Tuple
 
 import numpy as np
 
 from netin.utils import constants as const
 from netin.generators.tc import TriadicClosure
 from .pah import PAH
 
 
 class PATCH(PAH, TriadicClosure):
+    """Creates a new PATCH instance.
+
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
+    h_MM: float
+        homophily (similarity) between majority nodes (minimum=0, maximum=1.)
+
+    h_mm: float
+        homophily (similarity) between minority nodes (minimum=0, maximum=1.)
+
+    tc: float
+        probability of a new edge to close a triad (minimum=0, maximum=1.)
+
+    Notes
+    -----
+    The initialization is a undirected with n nodes and no edges.
+    Then, everytime a node is selected as source, it gets connected to k target nodes.
+    Target nodes are selected via preferential attachment (in-degree),homophily (h_**; see :class:`netin.Homophily`), and triadic closure (see :class:`netin.TriadicClosure`).
+
+    References
+    ----------
+    [1] A. L. Barabasi and R. Albert "Emergence of scaling in random networks", Science 286, pp 509-512, 1999.
+    """
 
     ############################################################
     # Constructor
     ############################################################
 
     def __init__(self, n: int, k: int, f_m: float, h_mm: float, h_MM: float, tc: float, seed: object = None):
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
-        h_MM: float
-            homophily (similarity) between majority nodes (minimum=0, maximum=1.)
-
-        h_mm: float
-            homophily (similarity) between minority nodes (minimum=0, maximum=1.)
-
-        tc: float
-            probability of a new edge to close a triad (minimum=0, maximum=1.)
-
-        Notes
-        -----
-        The initialization is a undirected with n nodes and no edges.
-        Then, everytime a node is selected as source, it gets connected to k target nodes.
-        Target nodes are selected via preferential attachment (in-degree), and homophily (h_**)
-
-        References
-        ----------
-        - [1] A. L. Barabasi and R. Albert "Emergence of scaling in random networks", Science 286, pp 509-512, 1999.
-        """
         PAH.__init__(self, n=n, k=k, f_m=f_m, h_MM=h_MM, h_mm=h_mm, seed=seed)
         TriadicClosure.__init__(self, n=n, f_m=f_m, tc=tc, seed=seed)
 
     ############################################################
     # Init
     ############################################################
 
@@ -63,55 +63,129 @@
         """
         Validates the parameters of the undirected.
         """
         PAH._validate_parameters(self)
         TriadicClosure._validate_parameters(self)
 
     def get_metadata_as_dict(self) -> dict:
+        """
+        Returns a dictionary with the metadata of the PATCH graph.
+
+        Returns
+        -------
+        dict
+            the graph  metadata as a dictionary
+        """
         obj1 = PAH.get_metadata_as_dict(self)
         obj2 = TriadicClosure.get_metadata_as_dict(self)
         obj1.update(obj2)
         return obj1
 
     ############################################################
     # Generation
     ############################################################
 
     def get_target_probabilities(self, source: Union[None, int], target_set: Union[None, Set[int]],
-                                 special_targets: Union[None, object, iter] = None) -> tuple[np.array, set[int]]:
+                                 special_targets: Union[None, object, iter] = None) -> Tuple[np.array, set[int]]:
+        """
+        Returns the probabilities of nodes to be selected as target nodes.
+
+        Parameters
+        ----------
+        source: int
+            source node id
+
+        target_set: set
+            set of target node ids
+
+        special_targets: dict
+            dictionary of special target node ids to be considered
+
+        Returns
+        -------
+        tuple
+            probabilities of nodes to be selected as target nodes, and set of target of nodes
+
+        """
         return TriadicClosure.get_target_probabilities(self, source, target_set, special_targets)
 
     def get_target_probabilities_regular(self, source: Union[None, int], target_set: Union[None, Set[int]],
-                                         special_targets: Union[None, object, iter] = None) -> tuple[
+                                         special_targets: Union[None, object, iter] = None) -> Tuple[
         np.ndarray, set[int]]:
+        """
+        Returns the probability of nodes to be selected as target nodes using the
+        preferential attachment with homophily mechanism.
+
+        Parameters
+        ----------
+        source: int
+            source node id
+
+        target_set: set
+            set of target node ids
+
+        special_targets: dict
+            dictionary of special target node ids to be considered
+
+        Returns
+        -------
+        tuple
+            probabilities of nodes to be selected as target nodes, and set of target of nodes
+        """
         return PAH.get_target_probabilities(self, source, target_set, special_targets)
 
     def get_special_targets(self, source: int) -> object:
         """
-        Return an empty dictionary (source node ids)
+        Returns an empty dictionary (source node ids)
+
         Parameters
         ----------
-        source: int
+        source : int
             Newly added node
+
+        Returns
+        -------
+        Dict
+            Empty dictionary
         """
         return TriadicClosure.get_special_targets(self, source)
 
     ############################################################
     # Calculations
     ############################################################
 
     def info_params(self):
+        """
+        Shows the (input) parameters of the graph.
+        """
         PAH.info_params(self)
         TriadicClosure.info_params(self)
 
     def info_computed(self):
+        """
+        Shows the (computed) properties of the graph.
+        """
         PAH.info_computed(self)
         TriadicClosure.info_computed(self)
 
-    def infer_homophily_values(self) -> (float, float):
+    def infer_homophily_values(self) -> Tuple[float, float]:
+        """
+        Infers analytically the homophily values of the graph.
+
+        Returns
+        -------
+        tuple
+            homophily values of the graph (majority, minority)
+        """
         h_MM = None
         h_mm = None
         return h_MM, h_mm
 
     def infer_triadic_closure(self) -> float:
+        """
+
+        Returns
+        -------
+
+        """
         tc = None
         return tc
```

### Comparing `netin-1.0.5.5/netin/generators/tc.py` & `netin-1.0.5.6/netin/generators/tc.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,20 +94,25 @@
     # Generation
     ############################################################
 
     def _initialize(self, class_attribute: str = 'm', class_values: list = None, class_labels: list = None):
         Graph._initialize(self, class_attribute, class_values, class_labels)
 
     def get_special_targets(self, source: int) -> object:
-        """
-        Return an empty dictionary (source node ids)
+        """ Return an empty dictionary (source node ids)
+
         Parameters
         ----------
-        source: int
+        source : int
             Newly added node
+
+        Returns
+        -------
+        object
+            Return an empty dictionary (source node ids)
         """
         return defaultdict(int)
 
     def get_target_probabilities_regular(self, source: Union[None, int], target_set: Union[None, Set[int]],
                                          special_targets: Union[None, object, iter] = None) -> tuple[
         np.array, set[int]]:
         # return Graph.get_target_probabilities(self, source, target_set, special_targets)
```

### Comparing `netin-1.0.5.5/netin/generators/tests/test_directed.py` & `netin-1.0.5.6/netin/generators/tests/test_directed.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.5/netin/generators/tests/test_dpah.py` & `netin-1.0.5.6/netin/generators/tests/test_dpah.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.5/netin/generators/tests/test_patch.py` & `netin-1.0.5.6/netin/generators/tests/test_patch.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.5/netin/generators/tests/test_undirected.py` & `netin-1.0.5.6/netin/generators/tests/test_undirected.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.5/netin/stats/distributions.py` & `netin-1.0.5.6/netin/stats/distributions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,31 @@
-from typing import Union, Set, List
+from typing import Union, Set, List, Tuple
 
 import numpy as np
 import pandas as pd
 import powerlaw
 
 
-def get_pdf(df: pd.DataFrame, x: str, total: float) -> (np.ndarray, np.ndarray):
+def get_pdf(df: pd.DataFrame, x: str, total: float) -> Tuple[np.ndarray, np.ndarray]:
+    """Compute the probability density of the input data.
+
+    Parameters
+    ----------
+    df : pd.DataFrame
+        DataFrame that contains the data.
+    x : str
+        The column name of the data.
+    total : float
+        The total amount by which to normalize the data.
+
+    Returns
+    -------
+    Tuple[np.ndarray, np.ndarray]
+        Two arrays holding the values and their probability.
+    """
     values = df.groupby(x).size()
     xs = values.index.values
     ys = values.values / total
     return xs, ys
 
 
 def get_cdf(df: pd.DataFrame, x: str, total: float = None) -> (np.ndarray, np.ndarray):
```

### Comparing `netin-1.0.5.5/netin/stats/ranking.py` & `netin-1.0.5.6/netin/stats/ranking.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.5/netin/utils/constants.py` & `netin-1.0.5.6/netin/utils/constants.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.5/netin/utils/validator.py` & `netin-1.0.5.6/netin/utils/validator.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.5/netin/viz/handlers.py` & `netin-1.0.5.6/netin/viz/handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -461,15 +461,15 @@
 
 
 def _show_beta(axline, data):
     axline(const.INEQUITY_BETA, ls='--', color='grey', alpha=0.5)
     axline(-const.INEQUITY_BETA, ls='--', color='grey', alpha=0.5)
 
 
-def plot_disparity(data: Union[pd.DataFrame, List[pd.DataFrame]], col_name: Union[str, List], fn=None, **kwargs):
+def plot_disparity(data: Union[pd.DataFrame, List[pd.DataFrame]], col_name: Union[str, List], fn: str = None, **kwargs):
     """
     Plots the disparity of the ranking of the minority group.
 
     Parameters
     ----------
     data: pd.DataFrame or List[pd.DataFrame]
         Metadata of nodes (each column is a property, e.g., degree)
@@ -497,15 +497,15 @@
     plot_distribution(data,
                       col_name=col_name,
                       get_x_y_from_df_fnc=get_disparity,
                       fn=fn, **kwargs)
 
 
 def plot_gini_coefficient(data: Union[pd.DataFrame, List[pd.DataFrame]], col_name: Union[str, List],
-                          fn=None, **kwargs):
+                          fn: str = None, **kwargs):
     """
     Plots the Gini coefficient of the ranking of the minority group.
 
     Parameters
     ----------
     data: pd.DataFrame or List[pd.DataFrame]
         Metadata of nodes (each column is a property, e.g., degree)
@@ -556,15 +556,15 @@
     plot_distribution(data,
                       col_name=col_name,
                       get_x_y_from_df_fnc=get_gini_coefficient,
                       fn=fn, **kwargs)
 
 
 def plot_fraction_of_minority(data: Union[pd.DataFrame, List[pd.DataFrame]], col_name: Union[str, List],
-                              fn=None, **kwargs):
+                              fn: str = None, **kwargs):
     """
     Plots the fraction of minority nodes in each top-k of the rank.
 
     Parameters
     ----------
     data: pd.DataFrame or List[pd.DataFrame]
         Metadata of nodes (each column is a property, e.g., degree)
```

### Comparing `netin-1.0.5.5/netin.egg-info/PKG-INFO` & `netin-1.0.5.6/netin.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netin
-Version: 1.0.5.5
+Version: 1.0.5.6
 Summary: Python package to study inequalities in social networks
 Home-page: https://github.com/CSHVienna/NetworkInequalities
 Author: Lisette Espín-Noboa
 Author-email: espin@csh.ac.at
 Maintainer: NetIn Developers
 Maintainer-email: netin-dev@googlegroups.com
 Keywords: Networks,Inequalities,Social Networks,Ranking,InferenceGraph Theory,Mathematics,network,undirected,discrete mathematics,math
@@ -45,14 +45,15 @@
 .. image:: https://img.shields.io/badge/NetworkX-3.1-blue.svg
     :target: https://networkx.org/
 
 .. image:: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg
     :target: https://creativecommons.org/licenses/by-nc-sa/4.0/
 
 - **Website:** https://www.networkinequality.com
+- **Documentation:** https://cshvienna.github.io/NetworkInequalities
 - **Source:** https://github.com/CSHVienna/NetworkInequalities
 - **Bug reports:** https://github.com/CSHVienna/NetworkInequalities/issues
 - **GitHub Discussions:** https://github.com/CSHVienna/NetworkInequalities/discussions
 - **Mailing list:** https://groups.google.com/forum/#!forum/netin-dev
 
 Simple examples
 ---------------
```

### Comparing `netin-1.0.5.5/netin.egg-info/SOURCES.txt` & `netin-1.0.5.6/netin.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -43,8 +43,9 @@
 netin/utils/__init__.py
 netin/utils/constants.py
 netin/utils/validator.py
 netin/viz/__init__.py
 netin/viz/constants.py
 netin/viz/handlers.py
 requirements/default.txt
+requirements/docs.txt
 requirements/test.txt
```

### Comparing `netin-1.0.5.5/setup.py` & `netin-1.0.5.6/setup.py`

 * *Files identical despite different names*

