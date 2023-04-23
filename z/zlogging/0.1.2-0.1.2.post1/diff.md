# Comparing `tmp/zlogging-0.1.2.tar.gz` & `tmp/zlogging-0.1.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zlogging-0.1.2.tar", last modified: Sat Jul 16 19:31:20 2022, max compression
+gzip compressed data, was "zlogging-0.1.2.post1.tar", last modified: Sun Apr 23 07:35:24 2023, max compression
```

## Comparing `zlogging-0.1.2.tar` & `zlogging-0.1.2.post1.tar`

### file list

```diff
@@ -1,73 +1,41 @@
-drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2022-07-16 19:31:20.485273 zlogging-0.1.2/
--rw-r--r--   0 jarryshaw   (501) staff       (20)     1523 2021-01-25 12:08:01.000000 zlogging-0.1.2/LICENSE
--rw-r--r--   0 jarryshaw   (501) staff       (20)      136 2020-02-10 12:53:21.000000 zlogging-0.1.2/MANIFEST.in
--rw-r--r--   0 jarryshaw   (501) staff       (20)    14926 2022-07-16 19:31:20.485687 zlogging-0.1.2/PKG-INFO
--rw-r--r--   0 jarryshaw   (501) staff       (20)    14088 2020-02-11 04:01:06.000000 zlogging-0.1.2/README.rst
-drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2022-07-16 19:31:20.403432 zlogging-0.1.2/archive/
--rw-r--r--   0 jarryshaw   (501) staff       (20)    30794 2020-02-08 08:03:00.000000 zlogging-0.1.2/archive/blogging.py
--rw-r--r--   0 jarryshaw   (501) staff       (20)     5718 2020-02-08 08:02:54.000000 zlogging-0.1.2/archive/logparser.py
--rw-r--r--   0 jarryshaw   (501) staff       (20)      494 2021-01-24 14:00:50.000000 zlogging-0.1.2/archive/test.py
-drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2022-07-16 19:31:20.398054 zlogging-0.1.2/docs/
-drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2022-07-16 19:31:20.403818 zlogging-0.1.2/docs/source/
--rw-r--r--   0 jarryshaw   (501) staff       (20)     4676 2022-07-16 06:25:06.000000 zlogging-0.1.2/docs/source/conf.py
-drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2022-07-16 19:31:20.404598 zlogging-0.1.2/gen/
--rw-r--r--   0 jarryshaw   (501) staff       (20)      980 2021-01-18 00:17:09.000000 zlogging-0.1.2/gen/fetch.py
--rw-r--r--   0 jarryshaw   (501) staff       (20)     8265 2022-07-15 22:52:19.000000 zlogging-0.1.2/gen/make.py
--rw-r--r--   0 jarryshaw   (501) staff       (20)      100 2020-10-07 16:57:02.000000 zlogging-0.1.2/pyproject.toml
--rw-r--r--   0 jarryshaw   (501) staff       (20)      256 2022-07-16 19:31:20.488066 zlogging-0.1.2/setup.cfg
--rw-r--r--   0 jarryshaw   (501) staff       (20)     2510 2022-07-16 19:16:27.000000 zlogging-0.1.2/setup.py
-drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2022-07-16 19:31:20.405342 zlogging-0.1.2/temp/
--rw-r--r--   0 jarryshaw   (501) staff       (20)      339 2021-01-16 12:33:15.000000 zlogging-0.1.2/temp/temp.py
--rw-r--r--   0 jarryshaw   (501) staff       (20)      595 2020-02-09 12:29:01.000000 zlogging-0.1.2/temp/test.py
-drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2022-07-16 19:31:20.406100 zlogging-0.1.2/tests/
--rw-r--r--   0 jarryshaw   (501) staff       (20)       24 2021-01-24 13:26:02.000000 zlogging-0.1.2/tests/__init__.py
--rw-r--r--   0 jarryshaw   (501) staff       (20)    28119 2022-07-16 19:24:24.000000 zlogging-0.1.2/tests/test_types.py
-drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2022-07-16 19:31:20.412839 zlogging-0.1.2/zlogging/
--rw-r--r--   0 jarryshaw   (501) staff       (20)      730 2021-01-31 14:11:31.000000 zlogging-0.1.2/zlogging/__init__.py
--rw-r--r--   0 jarryshaw   (501) staff       (20)    12381 2022-07-16 05:25:46.000000 zlogging-0.1.2/zlogging/_aux.py
--rw-r--r--   0 jarryshaw   (501) staff       (20)     3488 2021-01-31 13:43:01.000000 zlogging-0.1.2/zlogging/_compat.py
--rw-r--r--   0 jarryshaw   (501) staff       (20)     2790 2022-07-16 00:25:04.000000 zlogging-0.1.2/zlogging/_data.py
--rw-r--r--   0 jarryshaw   (501) staff       (20)     4732 2022-07-16 00:30:47.000000 zlogging-0.1.2/zlogging/_exc.py
--rw-r--r--   0 jarryshaw   (501) staff       (20)      564 2022-07-16 19:28:40.000000 zlogging-0.1.2/zlogging/_typing.py
--rw-r--r--   0 jarryshaw   (501) staff       (20)    25373 2022-07-16 05:25:46.000000 zlogging-0.1.2/zlogging/dumper.py
-drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2022-07-16 19:31:20.484168 zlogging-0.1.2/zlogging/enum/
--rw-r--r--   0 jarryshaw   (501) staff       (20)     5156 2022-07-09 19:11:38.000000 zlogging-0.1.2/zlogging/enum/Broker.py
--rw-r--r--   0 jarryshaw   (501) staff       (20)     1257 2022-07-09 19:11:39.000000 zlogging-0.1.2/zlogging/enum/Cluster.py
--rw-r--r--   0 jarryshaw   (501) staff       (20)     1688 2022-07-09 19:11:18.000000 zlogging-0.1.2/zlogging/enum/DCE_RPC.py
--rw-r--r--   0 jarryshaw   (501) staff       (20)     1092 2022-07-09 19:12:09.000000 zlogging-0.1.2/zlogging/enum/HTTP.py
--rw-r--r--   0 jarryshaw   (501) staff       (20)     1761 2022-07-09 19:11:41.000000 zlogging-0.1.2/zlogging/enum/Input.py
--rw-r--r--   0 jarryshaw   (501) staff       (20)     5661 2022-07-09 19:11:42.000000 zlogging-0.1.2/zlogging/enum/Intel.py
--rw-r--r--   0 jarryshaw   (501) staff       (20)     1011 2022-07-09 19:11:55.000000 zlogging-0.1.2/zlogging/enum/JSON.py
--rw-r--r--   0 jarryshaw   (501) staff       (20)      558 2022-07-09 19:12:37.000000 zlogging-0.1.2/zlogging/enum/Known.py
--rw-r--r--   0 jarryshaw   (501) staff       (20)      584 2022-07-09 19:12:34.000000 zlogging-0.1.2/zlogging/enum/LoadBalancing.py
--rw-r--r--   0 jarryshaw   (501) staff       (20)     9520 2022-07-09 19:11:43.000000 zlogging-0.1.2/zlogging/enum/Log.py
--rw-r--r--   0 jarryshaw   (501) staff       (20)     1691 2022-07-09 19:11:35.000000 zlogging-0.1.2/zlogging/enum/MOUNT3.py
--rw-r--r--   0 jarryshaw   (501) staff       (20)      474 2022-07-09 19:12:37.000000 zlogging-0.1.2/zlogging/enum/MQTT.py
--rw-r--r--   0 jarryshaw   (501) staff       (20)     4077 2022-07-09 19:11:35.000000 zlogging-0.1.2/zlogging/enum/NFS3.py
--rw-r--r--   0 jarryshaw   (501) staff       (20)     5824 2022-07-09 19:12:32.000000 zlogging-0.1.2/zlogging/enum/NetControl.py
--rw-r--r--   0 jarryshaw   (501) staff       (20)    16520 2022-07-09 19:11:46.000000 zlogging-0.1.2/zlogging/enum/Notice.py
--rw-r--r--   0 jarryshaw   (501) staff       (20)     3658 2022-07-09 19:11:48.000000 zlogging-0.1.2/zlogging/enum/OpenFlow.py
--rw-r--r--   0 jarryshaw   (501) staff       (20)      553 2022-07-09 19:12:25.000000 zlogging-0.1.2/zlogging/enum/ProtocolDetector.py
--rw-r--r--   0 jarryshaw   (501) staff       (20)      471 2022-07-09 19:11:35.000000 zlogging-0.1.2/zlogging/enum/Reporter.py
--rw-r--r--   0 jarryshaw   (501) staff       (20)      899 2022-07-09 19:12:16.000000 zlogging-0.1.2/zlogging/enum/SMB.py
--rw-r--r--   0 jarryshaw   (501) staff       (20)      521 2022-07-09 19:12:17.000000 zlogging-0.1.2/zlogging/enum/SOCKS.py
--rw-r--r--   0 jarryshaw   (501) staff       (20)      885 2022-07-09 19:12:40.000000 zlogging-0.1.2/zlogging/enum/SSL.py
--rw-r--r--   0 jarryshaw   (501) staff       (20)     1647 2022-07-09 19:11:49.000000 zlogging-0.1.2/zlogging/enum/Signatures.py
--rw-r--r--   0 jarryshaw   (501) staff       (20)     3450 2022-07-09 19:11:49.000000 zlogging-0.1.2/zlogging/enum/Software.py
--rw-r--r--   0 jarryshaw   (501) staff       (20)     2249 2022-07-09 19:11:49.000000 zlogging-0.1.2/zlogging/enum/SumStats.py
--rw-r--r--   0 jarryshaw   (501) staff       (20)      656 2022-07-09 19:11:51.000000 zlogging-0.1.2/zlogging/enum/Supervisor.py
--rw-r--r--   0 jarryshaw   (501) staff       (20)     1269 2022-07-09 19:11:52.000000 zlogging-0.1.2/zlogging/enum/Tunnel.py
--rw-r--r--   0 jarryshaw   (501) staff       (20)     1475 2022-07-09 19:11:46.000000 zlogging-0.1.2/zlogging/enum/Weird.py
--rw-r--r--   0 jarryshaw   (501) staff       (20)      891 2022-07-09 19:12:41.000000 zlogging-0.1.2/zlogging/enum/ZeekygenExample.py
--rw-r--r--   0 jarryshaw   (501) staff       (20)    38089 2022-07-15 22:52:06.000000 zlogging-0.1.2/zlogging/enum/__init__.py
--rw-r--r--   0 jarryshaw   (501) staff       (20)     6473 2022-07-09 19:12:21.000000 zlogging-0.1.2/zlogging/enum/zeek.py
--rw-r--r--   0 jarryshaw   (501) staff       (20)    22370 2022-07-16 19:29:44.000000 zlogging-0.1.2/zlogging/loader.py
--rw-r--r--   0 jarryshaw   (501) staff       (20)    10950 2022-07-15 22:02:31.000000 zlogging-0.1.2/zlogging/model.py
--rw-r--r--   0 jarryshaw   (501) staff       (20)    53151 2022-07-16 19:22:47.000000 zlogging-0.1.2/zlogging/types.py
--rw-r--r--   0 jarryshaw   (501) staff       (20)     6729 2022-07-16 06:17:09.000000 zlogging-0.1.2/zlogging/typing.py
-drwxr-xr-x   0 jarryshaw   (501) staff       (20)        0 2022-07-16 19:31:20.416149 zlogging-0.1.2/zlogging.egg-info/
--rw-r--r--   0 jarryshaw   (501) staff       (20)    14926 2022-07-16 19:31:18.000000 zlogging-0.1.2/zlogging.egg-info/PKG-INFO
--rw-r--r--   0 jarryshaw   (501) staff       (20)     1341 2022-07-16 19:31:20.000000 zlogging-0.1.2/zlogging.egg-info/SOURCES.txt
--rw-r--r--   0 jarryshaw   (501) staff       (20)        1 2022-07-16 19:31:18.000000 zlogging-0.1.2/zlogging.egg-info/dependency_links.txt
--rw-r--r--   0 jarryshaw   (501) staff       (20)       78 2022-07-16 19:31:18.000000 zlogging-0.1.2/zlogging.egg-info/requires.txt
--rw-r--r--   0 jarryshaw   (501) staff       (20)        9 2022-07-16 19:31:18.000000 zlogging-0.1.2/zlogging.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 07:35:24.882061 zlogging-0.1.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-23 07:35:10.000000 zlogging-0.1.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-23 07:35:10.000000 zlogging-0.1.2.post1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15054 2023-04-23 07:35:24.882061 zlogging-0.1.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14088 2023-04-23 07:35:10.000000 zlogging-0.1.2.post1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 07:35:24.882061 zlogging-0.1.2.post1/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)    30794 2023-04-23 07:35:10.000000 zlogging-0.1.2.post1/archive/blogging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-04-23 07:35:10.000000 zlogging-0.1.2.post1/archive/logparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-23 07:35:10.000000 zlogging-0.1.2.post1/archive/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 07:35:24.882061 zlogging-0.1.2.post1/gen/
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-23 07:35:10.000000 zlogging-0.1.2.post1/gen/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-04-23 07:35:10.000000 zlogging-0.1.2.post1/gen/make.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-04-23 07:35:10.000000 zlogging-0.1.2.post1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 07:35:24.882061 zlogging-0.1.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-23 07:35:10.000000 zlogging-0.1.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 07:35:24.882061 zlogging-0.1.2.post1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-23 07:35:10.000000 zlogging-0.1.2.post1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28119 2023-04-23 07:35:10.000000 zlogging-0.1.2.post1/tests/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 07:35:24.882061 zlogging-0.1.2.post1/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-04-23 07:35:10.000000 zlogging-0.1.2.post1/util/bump_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 07:35:24.882061 zlogging-0.1.2.post1/zlogging/
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-23 07:35:10.000000 zlogging-0.1.2.post1/zlogging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12381 2023-04-23 07:35:10.000000 zlogging-0.1.2.post1/zlogging/_aux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-04-23 07:35:10.000000 zlogging-0.1.2.post1/zlogging/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-23 07:35:10.000000 zlogging-0.1.2.post1/zlogging/_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-04-23 07:35:10.000000 zlogging-0.1.2.post1/zlogging/_exc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-23 07:35:10.000000 zlogging-0.1.2.post1/zlogging/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25373 2023-04-23 07:35:10.000000 zlogging-0.1.2.post1/zlogging/dumper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 07:35:24.882061 zlogging-0.1.2.post1/zlogging/enum/
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-23 07:35:10.000000 zlogging-0.1.2.post1/zlogging/enum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22370 2023-04-23 07:35:10.000000 zlogging-0.1.2.post1/zlogging/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10950 2023-04-23 07:35:10.000000 zlogging-0.1.2.post1/zlogging/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53151 2023-04-23 07:35:10.000000 zlogging-0.1.2.post1/zlogging/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-04-23 07:35:10.000000 zlogging-0.1.2.post1/zlogging/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 07:35:24.882061 zlogging-0.1.2.post1/zlogging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15054 2023-04-23 07:35:24.000000 zlogging-0.1.2.post1/zlogging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-23 07:35:24.000000 zlogging-0.1.2.post1/zlogging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 07:35:24.000000 zlogging-0.1.2.post1/zlogging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 07:35:24.000000 zlogging-0.1.2.post1/zlogging.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-23 07:35:24.000000 zlogging-0.1.2.post1/zlogging.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-23 07:35:24.000000 zlogging-0.1.2.post1/zlogging.egg-info/top_level.txt
```

### Comparing `zlogging-0.1.2/LICENSE` & `zlogging-0.1.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2/PKG-INFO` & `zlogging-0.1.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: zlogging
-Version: 0.1.2
-Summary: Bro/Zeek logging framework for Python.
-Home-page: https://github.com/JarryShaw/zlogging
-Download-URL: https://github.com/JarryShaw/zlogging/archive/v0.1.2.tar.gz
-Author: Jarry Shaw
-Author-email: jarryshaw@icloud.com
+Version: 0.1.2.post1
+Summary: zlogging: Bro/Zeek logging framework for Python.
+Author-email: Jarry Shaw <jarryshaw@icloud.com>
 Maintainer: Jarry Shaw
-Maintainer-email: jarryshaw@icloud.com
-License: BSD License
+License: BSD 3-Clause License
+Project-URL: homepage, https://jarryshaw.github.io/zlogging/
+Project-URL: documentation, https://jarryshaw.github.io/zlogging/
+Project-URL: repository, https://github.com/JarryShaw/zlogging
+Project-URL: changelog, https://github.com/JarryShaw/zlogging/releases
 Keywords: bro,zeek,logging
-Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6
+Requires-Python: <4,>=3.6
 Description-Content-Type: text/x-rst
+Provides-Extra: docs
 License-File: LICENSE
 
 ================================================
 ZLogging - Bro/Zeek logging framework for Python
 ================================================
 
     Online documentation is available at https://zlogging.readthedocs.io/
```

### Comparing `zlogging-0.1.2/README.rst` & `zlogging-0.1.2.post1/README.rst`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2/archive/blogging.py` & `zlogging-0.1.2.post1/archive/blogging.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2/archive/logparser.py` & `zlogging-0.1.2.post1/archive/logparser.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2/gen/fetch.py` & `zlogging-0.1.2.post1/gen/fetch.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2/gen/make.py` & `zlogging-0.1.2.post1/gen/make.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2/tests/test_types.py` & `zlogging-0.1.2.post1/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2/zlogging/__init__.py` & `zlogging-0.1.2.post1/zlogging/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,7 +14,10 @@
 
     'Model', 'new_model',
 
     'AddrType', 'BoolType', 'CountType', 'DoubleType', 'EnumType',
     'IntervalType', 'IntType', 'PortType', 'RecordType', 'SetType',
     'StringType', 'SubnetType', 'TimeType', 'VectorType',
 ]
+
+# version string
+__version__ = '0.1.2.post1'
```

### Comparing `zlogging-0.1.2/zlogging/_aux.py` & `zlogging-0.1.2.post1/zlogging/_aux.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2/zlogging/_compat.py` & `zlogging-0.1.2.post1/zlogging/_compat.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2/zlogging/_data.py` & `zlogging-0.1.2.post1/zlogging/_data.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2/zlogging/_exc.py` & `zlogging-0.1.2.post1/zlogging/_exc.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2/zlogging/_typing.py` & `zlogging-0.1.2.post1/zlogging/_typing.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2/zlogging/dumper.py` & `zlogging-0.1.2.post1/zlogging/dumper.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2/zlogging/loader.py` & `zlogging-0.1.2.post1/zlogging/loader.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2/zlogging/model.py` & `zlogging-0.1.2.post1/zlogging/model.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2/zlogging/types.py` & `zlogging-0.1.2.post1/zlogging/types.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2/zlogging/typing.py` & `zlogging-0.1.2.post1/zlogging/typing.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2/zlogging.egg-info/PKG-INFO` & `zlogging-0.1.2.post1/zlogging.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: zlogging
-Version: 0.1.2
-Summary: Bro/Zeek logging framework for Python.
-Home-page: https://github.com/JarryShaw/zlogging
-Download-URL: https://github.com/JarryShaw/zlogging/archive/v0.1.2.tar.gz
-Author: Jarry Shaw
-Author-email: jarryshaw@icloud.com
+Version: 0.1.2.post1
+Summary: zlogging: Bro/Zeek logging framework for Python.
+Author-email: Jarry Shaw <jarryshaw@icloud.com>
 Maintainer: Jarry Shaw
-Maintainer-email: jarryshaw@icloud.com
-License: BSD License
+License: BSD 3-Clause License
+Project-URL: homepage, https://jarryshaw.github.io/zlogging/
+Project-URL: documentation, https://jarryshaw.github.io/zlogging/
+Project-URL: repository, https://github.com/JarryShaw/zlogging
+Project-URL: changelog, https://github.com/JarryShaw/zlogging/releases
 Keywords: bro,zeek,logging
-Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6
+Requires-Python: <4,>=3.6
 Description-Content-Type: text/x-rst
+Provides-Extra: docs
 License-File: LICENSE
 
 ================================================
 ZLogging - Bro/Zeek logging framework for Python
 ================================================
 
     Online documentation is available at https://zlogging.readthedocs.io/
```

