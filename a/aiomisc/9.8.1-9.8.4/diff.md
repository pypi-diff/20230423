# Comparing `tmp/aiomisc-9.8.1.tar.gz` & `tmp/aiomisc-9.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aiomisc-9.8.1.tar", last modified: Thu May  7 23:56:10 2020, max compression
+gzip compressed data, was "dist/aiomisc-9.8.4.tar", last modified: Fri May  8 09:58:39 2020, max compression
```

## Comparing `aiomisc-9.8.1.tar` & `aiomisc-9.8.4.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 mosquito (610789169) staff       (20)        0 2020-05-07 23:56:10.000000 aiomisc-9.8.1/
--rw-r--r--   0 mosquito (610789169) staff       (20)       73 2018-08-23 10:32:24.000000 aiomisc-9.8.1/MANIFEST.in
--rw-r--r--   0 mosquito (610789169) staff       (20)    61680 2020-05-07 23:56:10.000000 aiomisc-9.8.1/PKG-INFO
--rw-r--r--   0 mosquito (610789169) staff       (20)    45355 2020-05-07 23:48:38.000000 aiomisc-9.8.1/README.rst
-drwxr-xr-x   0 mosquito (610789169) staff       (20)        0 2020-05-07 23:56:10.000000 aiomisc-9.8.1/aiomisc/
--rw-r--r--   0 mosquito (610789169) staff       (20)     1850 2020-05-07 17:20:00.000000 aiomisc-9.8.1/aiomisc/__init__.py
--rw-r--r--   0 mosquito (610789169) staff       (20)     2487 2020-05-07 17:20:00.000000 aiomisc-9.8.1/aiomisc/backoff.py
--rw-r--r--   0 mosquito (610789169) staff       (20)     1027 2020-05-07 17:20:00.000000 aiomisc-9.8.1/aiomisc/context.py
--rw-r--r--   0 mosquito (610789169) staff       (20)     4874 2020-05-07 17:20:00.000000 aiomisc-9.8.1/aiomisc/entrypoint.py
--rw-r--r--   0 mosquito (610789169) staff       (20)     4933 2020-05-07 17:20:00.000000 aiomisc-9.8.1/aiomisc/io.py
--rw-r--r--   0 mosquito (610789169) staff       (20)     3789 2020-05-07 17:20:00.000000 aiomisc-9.8.1/aiomisc/iterator_wrapper.py
--rw-r--r--   0 mosquito (610789169) staff       (20)     2343 2020-05-07 17:20:00.000000 aiomisc-9.8.1/aiomisc/log.py
--rw-r--r--   0 mosquito (610789169) staff       (20)     2641 2020-05-07 17:20:00.000000 aiomisc-9.8.1/aiomisc/periodic.py
--rw-r--r--   0 mosquito (610789169) staff       (20)     5049 2020-05-07 17:20:00.000000 aiomisc-9.8.1/aiomisc/pool.py
--rw-r--r--   0 mosquito (610789169) staff       (20)     1555 2020-02-06 16:48:43.000000 aiomisc-9.8.1/aiomisc/process_pool.py
-drwxr-xr-x   0 mosquito (610789169) staff       (20)        0 2020-05-07 23:56:10.000000 aiomisc-9.8.1/aiomisc/service/
--rw-r--r--   0 mosquito (610789169) staff       (20)      355 2020-05-07 17:20:00.000000 aiomisc-9.8.1/aiomisc/service/__init__.py
--rw-r--r--   0 mosquito (610789169) staff       (20)     2895 2020-05-07 17:25:21.000000 aiomisc-9.8.1/aiomisc/service/aiohttp.py
--rw-r--r--   0 mosquito (610789169) staff       (20)     2249 2020-05-07 19:39:42.000000 aiomisc-9.8.1/aiomisc/service/base.py
--rw-r--r--   0 mosquito (610789169) staff       (20)     1685 2020-05-07 17:20:00.000000 aiomisc-9.8.1/aiomisc/service/carbon.py
--rw-r--r--   0 mosquito (610789169) staff       (20)      979 2020-05-07 17:20:00.000000 aiomisc-9.8.1/aiomisc/service/periodic.py
--rw-r--r--   0 mosquito (610789169) staff       (20)     1551 2020-05-07 17:20:00.000000 aiomisc-9.8.1/aiomisc/service/profiler.py
--rw-r--r--   0 mosquito (610789169) staff       (20)     3402 2020-05-07 17:20:00.000000 aiomisc-9.8.1/aiomisc/service/raven.py
--rw-r--r--   0 mosquito (610789169) staff       (20)     1639 2020-05-07 19:39:42.000000 aiomisc-9.8.1/aiomisc/service/tcp.py
--rw-r--r--   0 mosquito (610789169) staff       (20)     2614 2020-05-07 19:39:42.000000 aiomisc-9.8.1/aiomisc/service/tls.py
--rw-r--r--   0 mosquito (610789169) staff       (20)     2604 2020-05-07 17:20:00.000000 aiomisc-9.8.1/aiomisc/service/tracer.py
--rw-r--r--   0 mosquito (610789169) staff       (20)     2182 2020-05-07 19:39:42.000000 aiomisc-9.8.1/aiomisc/service/udp.py
--rw-r--r--   0 mosquito (610789169) staff       (20)     1063 2020-05-07 17:20:00.000000 aiomisc-9.8.1/aiomisc/signal.py
--rw-r--r--   0 mosquito (610789169) staff       (20)     9088 2020-05-07 17:20:00.000000 aiomisc-9.8.1/aiomisc/thread_pool.py
--rw-r--r--   0 mosquito (610789169) staff       (20)      519 2020-05-07 17:20:00.000000 aiomisc-9.8.1/aiomisc/timeout.py
--rw-r--r--   0 mosquito (610789169) staff       (20)     6465 2020-05-07 17:25:21.000000 aiomisc-9.8.1/aiomisc/utils.py
--rw-r--r--   0 mosquito (610789169) staff       (20)      147 2020-05-07 23:56:10.000000 aiomisc-9.8.1/aiomisc/version.py
-drwxr-xr-x   0 mosquito (610789169) staff       (20)        0 2020-05-07 23:56:10.000000 aiomisc-9.8.1/aiomisc.egg-info/
--rw-r--r--   0 mosquito (610789169) staff       (20)    61680 2020-05-07 23:56:10.000000 aiomisc-9.8.1/aiomisc.egg-info/PKG-INFO
--rw-r--r--   0 mosquito (610789169) staff       (20)     1160 2020-05-07 23:56:10.000000 aiomisc-9.8.1/aiomisc.egg-info/SOURCES.txt
--rw-r--r--   0 mosquito (610789169) staff       (20)        1 2020-05-07 23:56:10.000000 aiomisc-9.8.1/aiomisc.egg-info/dependency_links.txt
--rw-r--r--   0 mosquito (610789169) staff       (20)       51 2020-05-07 23:56:10.000000 aiomisc-9.8.1/aiomisc.egg-info/entry_points.txt
--rw-r--r--   0 mosquito (610789169) staff       (20)      331 2020-05-07 23:56:10.000000 aiomisc-9.8.1/aiomisc.egg-info/requires.txt
--rw-r--r--   0 mosquito (610789169) staff       (20)       29 2020-05-07 23:56:10.000000 aiomisc-9.8.1/aiomisc.egg-info/top_level.txt
-drwxr-xr-x   0 mosquito (610789169) staff       (20)        0 2020-05-07 23:56:10.000000 aiomisc-9.8.1/aiomisc_pytest/
--rw-r--r--   0 mosquito (610789169) staff       (20)        0 2019-01-22 22:57:20.000000 aiomisc-9.8.1/aiomisc_pytest/__init__.py
--rw-r--r--   0 mosquito (610789169) staff       (20)    16992 2020-05-07 23:51:56.000000 aiomisc-9.8.1/aiomisc_pytest/pytest_plugin.py
--rw-r--r--   0 mosquito (610789169) staff       (20)      125 2020-05-07 19:39:42.000000 aiomisc-9.8.1/requirements.dev.txt
--rw-r--r--   0 mosquito (610789169) staff       (20)       26 2020-04-01 13:44:20.000000 aiomisc-9.8.1/requirements.txt
--rw-r--r--   0 mosquito (610789169) staff       (20)       38 2020-05-07 23:56:10.000000 aiomisc-9.8.1/setup.cfg
--rw-r--r--   0 mosquito (610789169) staff       (20)     2117 2020-02-11 13:47:46.000000 aiomisc-9.8.1/setup.py
-drwxr-xr-x   0 mosquito (610789169) staff       (20)        0 2020-05-07 23:56:10.000000 aiomisc-9.8.1/tests/
-drwxr-xr-x   0 mosquito (610789169) staff       (20)        0 2020-05-07 23:56:10.000000 aiomisc-9.8.1/tests/pytest_plugin/
--rw-r--r--   0 mosquito (610789169) staff       (20)        0 2019-02-28 22:19:47.000000 aiomisc-9.8.1/tests/pytest_plugin/__init__.py
--rw-r--r--   0 mosquito (610789169) staff       (20)       65 2019-10-30 15:35:55.000000 aiomisc-9.8.1/tests/pytest_plugin/conftest.py
--rw-r--r--   0 mosquito (610789169) staff       (20)     1044 2020-05-07 17:20:00.000000 aiomisc-9.8.1/tests/pytest_plugin/test_loop_fixture.py
--rw-r--r--   0 mosquito (610789169) staff       (20)     2674 2020-05-07 23:05:16.000000 aiomisc-9.8.1/tests/pytest_plugin/test_tcp_proxy.py
--rw-r--r--   0 mosquito (610789169) staff       (20)     2277 2020-05-07 23:48:38.000000 aiomisc-9.8.1/tests/pytest_plugin/test_tcp_proxy_example.py
--rw-r--r--   0 mosquito (610789169) staff       (20)      372 2020-05-07 17:20:00.000000 aiomisc-9.8.1/tests/pytest_plugin/yield_fixture.py
--rw-r--r--   0 mosquito (610789169) staff       (20)      362 2020-02-05 21:38:09.000000 aiomisc-9.8.1/tests/pytest_plugin/yield_fixture_native.py
+drwxr-xr-x   0 mosquito (610789169) staff       (20)        0 2020-05-08 09:58:39.000000 aiomisc-9.8.4/
+-rw-r--r--   0 mosquito (610789169) staff       (20)       73 2018-08-23 10:32:24.000000 aiomisc-9.8.4/MANIFEST.in
+-rw-r--r--   0 mosquito (610789169) staff       (20)    61680 2020-05-08 09:58:39.000000 aiomisc-9.8.4/PKG-INFO
+-rw-r--r--   0 mosquito (610789169) staff       (20)    45355 2020-05-07 23:48:38.000000 aiomisc-9.8.4/README.rst
+drwxr-xr-x   0 mosquito (610789169) staff       (20)        0 2020-05-08 09:58:39.000000 aiomisc-9.8.4/aiomisc/
+-rw-r--r--   0 mosquito (610789169) staff       (20)     1850 2020-05-07 17:20:00.000000 aiomisc-9.8.4/aiomisc/__init__.py
+-rw-r--r--   0 mosquito (610789169) staff       (20)     2487 2020-05-07 17:20:00.000000 aiomisc-9.8.4/aiomisc/backoff.py
+-rw-r--r--   0 mosquito (610789169) staff       (20)     1027 2020-05-07 17:20:00.000000 aiomisc-9.8.4/aiomisc/context.py
+-rw-r--r--   0 mosquito (610789169) staff       (20)     4874 2020-05-07 17:20:00.000000 aiomisc-9.8.4/aiomisc/entrypoint.py
+-rw-r--r--   0 mosquito (610789169) staff       (20)     4933 2020-05-07 17:20:00.000000 aiomisc-9.8.4/aiomisc/io.py
+-rw-r--r--   0 mosquito (610789169) staff       (20)     3789 2020-05-07 17:20:00.000000 aiomisc-9.8.4/aiomisc/iterator_wrapper.py
+-rw-r--r--   0 mosquito (610789169) staff       (20)     2343 2020-05-07 17:20:00.000000 aiomisc-9.8.4/aiomisc/log.py
+-rw-r--r--   0 mosquito (610789169) staff       (20)     2641 2020-05-07 17:20:00.000000 aiomisc-9.8.4/aiomisc/periodic.py
+-rw-r--r--   0 mosquito (610789169) staff       (20)     5049 2020-05-07 17:20:00.000000 aiomisc-9.8.4/aiomisc/pool.py
+-rw-r--r--   0 mosquito (610789169) staff       (20)     1555 2020-02-06 16:48:43.000000 aiomisc-9.8.4/aiomisc/process_pool.py
+drwxr-xr-x   0 mosquito (610789169) staff       (20)        0 2020-05-08 09:58:39.000000 aiomisc-9.8.4/aiomisc/service/
+-rw-r--r--   0 mosquito (610789169) staff       (20)      355 2020-05-07 17:20:00.000000 aiomisc-9.8.4/aiomisc/service/__init__.py
+-rw-r--r--   0 mosquito (610789169) staff       (20)     2895 2020-05-07 17:25:21.000000 aiomisc-9.8.4/aiomisc/service/aiohttp.py
+-rw-r--r--   0 mosquito (610789169) staff       (20)     2249 2020-05-07 19:39:42.000000 aiomisc-9.8.4/aiomisc/service/base.py
+-rw-r--r--   0 mosquito (610789169) staff       (20)     1685 2020-05-07 17:20:00.000000 aiomisc-9.8.4/aiomisc/service/carbon.py
+-rw-r--r--   0 mosquito (610789169) staff       (20)      979 2020-05-07 17:20:00.000000 aiomisc-9.8.4/aiomisc/service/periodic.py
+-rw-r--r--   0 mosquito (610789169) staff       (20)     1551 2020-05-07 17:20:00.000000 aiomisc-9.8.4/aiomisc/service/profiler.py
+-rw-r--r--   0 mosquito (610789169) staff       (20)     3402 2020-05-07 17:20:00.000000 aiomisc-9.8.4/aiomisc/service/raven.py
+-rw-r--r--   0 mosquito (610789169) staff       (20)     1639 2020-05-07 19:39:42.000000 aiomisc-9.8.4/aiomisc/service/tcp.py
+-rw-r--r--   0 mosquito (610789169) staff       (20)     2614 2020-05-07 19:39:42.000000 aiomisc-9.8.4/aiomisc/service/tls.py
+-rw-r--r--   0 mosquito (610789169) staff       (20)     2604 2020-05-07 17:20:00.000000 aiomisc-9.8.4/aiomisc/service/tracer.py
+-rw-r--r--   0 mosquito (610789169) staff       (20)     2182 2020-05-07 19:39:42.000000 aiomisc-9.8.4/aiomisc/service/udp.py
+-rw-r--r--   0 mosquito (610789169) staff       (20)     1063 2020-05-07 17:20:00.000000 aiomisc-9.8.4/aiomisc/signal.py
+-rw-r--r--   0 mosquito (610789169) staff       (20)     9088 2020-05-07 17:20:00.000000 aiomisc-9.8.4/aiomisc/thread_pool.py
+-rw-r--r--   0 mosquito (610789169) staff       (20)      519 2020-05-07 17:20:00.000000 aiomisc-9.8.4/aiomisc/timeout.py
+-rw-r--r--   0 mosquito (610789169) staff       (20)     6465 2020-05-07 17:25:21.000000 aiomisc-9.8.4/aiomisc/utils.py
+-rw-r--r--   0 mosquito (610789169) staff       (20)      147 2020-05-08 09:58:39.000000 aiomisc-9.8.4/aiomisc/version.py
+drwxr-xr-x   0 mosquito (610789169) staff       (20)        0 2020-05-08 09:58:39.000000 aiomisc-9.8.4/aiomisc.egg-info/
+-rw-r--r--   0 mosquito (610789169) staff       (20)    61680 2020-05-08 09:58:39.000000 aiomisc-9.8.4/aiomisc.egg-info/PKG-INFO
+-rw-r--r--   0 mosquito (610789169) staff       (20)     1160 2020-05-08 09:58:39.000000 aiomisc-9.8.4/aiomisc.egg-info/SOURCES.txt
+-rw-r--r--   0 mosquito (610789169) staff       (20)        1 2020-05-08 09:58:39.000000 aiomisc-9.8.4/aiomisc.egg-info/dependency_links.txt
+-rw-r--r--   0 mosquito (610789169) staff       (20)       51 2020-05-08 09:58:39.000000 aiomisc-9.8.4/aiomisc.egg-info/entry_points.txt
+-rw-r--r--   0 mosquito (610789169) staff       (20)      331 2020-05-08 09:58:39.000000 aiomisc-9.8.4/aiomisc.egg-info/requires.txt
+-rw-r--r--   0 mosquito (610789169) staff       (20)       29 2020-05-08 09:58:39.000000 aiomisc-9.8.4/aiomisc.egg-info/top_level.txt
+drwxr-xr-x   0 mosquito (610789169) staff       (20)        0 2020-05-08 09:58:39.000000 aiomisc-9.8.4/aiomisc_pytest/
+-rw-r--r--   0 mosquito (610789169) staff       (20)        0 2019-01-22 22:57:20.000000 aiomisc-9.8.4/aiomisc_pytest/__init__.py
+-rw-r--r--   0 mosquito (610789169) staff       (20)    18274 2020-05-08 09:58:02.000000 aiomisc-9.8.4/aiomisc_pytest/pytest_plugin.py
+-rw-r--r--   0 mosquito (610789169) staff       (20)      125 2020-05-07 19:39:42.000000 aiomisc-9.8.4/requirements.dev.txt
+-rw-r--r--   0 mosquito (610789169) staff       (20)       26 2020-04-01 13:44:20.000000 aiomisc-9.8.4/requirements.txt
+-rw-r--r--   0 mosquito (610789169) staff       (20)       38 2020-05-08 09:58:39.000000 aiomisc-9.8.4/setup.cfg
+-rw-r--r--   0 mosquito (610789169) staff       (20)     2117 2020-02-11 13:47:46.000000 aiomisc-9.8.4/setup.py
+drwxr-xr-x   0 mosquito (610789169) staff       (20)        0 2020-05-08 09:58:39.000000 aiomisc-9.8.4/tests/
+drwxr-xr-x   0 mosquito (610789169) staff       (20)        0 2020-05-08 09:58:39.000000 aiomisc-9.8.4/tests/pytest_plugin/
+-rw-r--r--   0 mosquito (610789169) staff       (20)        0 2019-02-28 22:19:47.000000 aiomisc-9.8.4/tests/pytest_plugin/__init__.py
+-rw-r--r--   0 mosquito (610789169) staff       (20)       65 2019-10-30 15:35:55.000000 aiomisc-9.8.4/tests/pytest_plugin/conftest.py
+-rw-r--r--   0 mosquito (610789169) staff       (20)     1044 2020-05-07 17:20:00.000000 aiomisc-9.8.4/tests/pytest_plugin/test_loop_fixture.py
+-rw-r--r--   0 mosquito (610789169) staff       (20)     2689 2020-05-08 00:18:18.000000 aiomisc-9.8.4/tests/pytest_plugin/test_tcp_proxy.py
+-rw-r--r--   0 mosquito (610789169) staff       (20)     2277 2020-05-07 23:48:38.000000 aiomisc-9.8.4/tests/pytest_plugin/test_tcp_proxy_example.py
+-rw-r--r--   0 mosquito (610789169) staff       (20)      372 2020-05-07 17:20:00.000000 aiomisc-9.8.4/tests/pytest_plugin/yield_fixture.py
+-rw-r--r--   0 mosquito (610789169) staff       (20)      362 2020-02-05 21:38:09.000000 aiomisc-9.8.4/tests/pytest_plugin/yield_fixture_native.py
```

### Comparing `aiomisc-9.8.1/PKG-INFO` & `aiomisc-9.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiomisc
-Version: 9.8.1
+Version: 9.8.4
 Summary: aiomisc - miscellaneous utils for asyncio
 Home-page: https://github.com/mosquito/aiomisc
 Author: Dmitry Orlov
 Author-email: me@mosquito.su
 License: MIT
 Description: aiomisc - miscellaneous utils for asyncio
         =========================================
@@ -1934,13 +1934,13 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Provides-Extra: carbon
-Provides-Extra: contextvars
 Provides-Extra: raven
-Provides-Extra: develop
 Provides-Extra: aiohttp
+Provides-Extra: contextvars
+Provides-Extra: develop
+Provides-Extra: carbon
 Provides-Extra: uvloop
```

### Comparing `aiomisc-9.8.1/README.rst` & `aiomisc-9.8.4/README.rst`

 * *Files identical despite different names*

### Comparing `aiomisc-9.8.1/aiomisc/__init__.py` & `aiomisc-9.8.4/aiomisc/__init__.py`

 * *Files identical despite different names*

### Comparing `aiomisc-9.8.1/aiomisc/backoff.py` & `aiomisc-9.8.4/aiomisc/backoff.py`

 * *Files identical despite different names*

### Comparing `aiomisc-9.8.1/aiomisc/context.py` & `aiomisc-9.8.4/aiomisc/context.py`

 * *Files identical despite different names*

### Comparing `aiomisc-9.8.1/aiomisc/entrypoint.py` & `aiomisc-9.8.4/aiomisc/entrypoint.py`

 * *Files identical despite different names*

### Comparing `aiomisc-9.8.1/aiomisc/io.py` & `aiomisc-9.8.4/aiomisc/io.py`

 * *Files identical despite different names*

### Comparing `aiomisc-9.8.1/aiomisc/iterator_wrapper.py` & `aiomisc-9.8.4/aiomisc/iterator_wrapper.py`

 * *Files identical despite different names*

### Comparing `aiomisc-9.8.1/aiomisc/log.py` & `aiomisc-9.8.4/aiomisc/log.py`

 * *Files identical despite different names*

### Comparing `aiomisc-9.8.1/aiomisc/periodic.py` & `aiomisc-9.8.4/aiomisc/periodic.py`

 * *Files identical despite different names*

### Comparing `aiomisc-9.8.1/aiomisc/pool.py` & `aiomisc-9.8.4/aiomisc/pool.py`

 * *Files identical despite different names*

### Comparing `aiomisc-9.8.1/aiomisc/process_pool.py` & `aiomisc-9.8.4/aiomisc/process_pool.py`

 * *Files identical despite different names*

### Comparing `aiomisc-9.8.1/aiomisc/service/aiohttp.py` & `aiomisc-9.8.4/aiomisc/service/aiohttp.py`

 * *Files identical despite different names*

### Comparing `aiomisc-9.8.1/aiomisc/service/base.py` & `aiomisc-9.8.4/aiomisc/service/base.py`

 * *Files identical despite different names*

### Comparing `aiomisc-9.8.1/aiomisc/service/carbon.py` & `aiomisc-9.8.4/aiomisc/service/carbon.py`

 * *Files identical despite different names*

### Comparing `aiomisc-9.8.1/aiomisc/service/periodic.py` & `aiomisc-9.8.4/aiomisc/service/periodic.py`

 * *Files identical despite different names*

### Comparing `aiomisc-9.8.1/aiomisc/service/profiler.py` & `aiomisc-9.8.4/aiomisc/service/profiler.py`

 * *Files identical despite different names*

### Comparing `aiomisc-9.8.1/aiomisc/service/raven.py` & `aiomisc-9.8.4/aiomisc/service/raven.py`

 * *Files identical despite different names*

### Comparing `aiomisc-9.8.1/aiomisc/service/tcp.py` & `aiomisc-9.8.4/aiomisc/service/tcp.py`

 * *Files identical despite different names*

### Comparing `aiomisc-9.8.1/aiomisc/service/tls.py` & `aiomisc-9.8.4/aiomisc/service/tls.py`

 * *Files identical despite different names*

### Comparing `aiomisc-9.8.1/aiomisc/service/tracer.py` & `aiomisc-9.8.4/aiomisc/service/tracer.py`

 * *Files identical despite different names*

### Comparing `aiomisc-9.8.1/aiomisc/service/udp.py` & `aiomisc-9.8.4/aiomisc/service/udp.py`

 * *Files identical despite different names*

### Comparing `aiomisc-9.8.1/aiomisc/signal.py` & `aiomisc-9.8.4/aiomisc/signal.py`

 * *Files identical despite different names*

### Comparing `aiomisc-9.8.1/aiomisc/thread_pool.py` & `aiomisc-9.8.4/aiomisc/thread_pool.py`

 * *Files identical despite different names*

### Comparing `aiomisc-9.8.1/aiomisc/timeout.py` & `aiomisc-9.8.4/aiomisc/timeout.py`

 * *Files identical despite different names*

### Comparing `aiomisc-9.8.1/aiomisc/utils.py` & `aiomisc-9.8.4/aiomisc/utils.py`

 * *Files identical despite different names*

### Comparing `aiomisc-9.8.1/aiomisc.egg-info/PKG-INFO` & `aiomisc-9.8.4/aiomisc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiomisc
-Version: 9.8.1
+Version: 9.8.4
 Summary: aiomisc - miscellaneous utils for asyncio
 Home-page: https://github.com/mosquito/aiomisc
 Author: Dmitry Orlov
 Author-email: me@mosquito.su
 License: MIT
 Description: aiomisc - miscellaneous utils for asyncio
         =========================================
@@ -1934,13 +1934,13 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Provides-Extra: carbon
-Provides-Extra: contextvars
 Provides-Extra: raven
-Provides-Extra: develop
 Provides-Extra: aiohttp
+Provides-Extra: contextvars
+Provides-Extra: develop
+Provides-Extra: carbon
 Provides-Extra: uvloop
```

### Comparing `aiomisc-9.8.1/aiomisc.egg-info/SOURCES.txt` & `aiomisc-9.8.4/aiomisc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiomisc-9.8.1/aiomisc_pytest/pytest_plugin.py` & `aiomisc-9.8.4/aiomisc_pytest/pytest_plugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from unittest.mock import MagicMock
 
 import pytest
 
 import aiomisc
 
 
-log = logging.getLogger(__name__)
+log = logging.getLogger("aiomisc_pytest")
 asyncio.get_event_loop = MagicMock(asyncio.get_event_loop)
 asyncio.get_event_loop.side_effect = get_event_loop
 
 
 try:
     import uvloop
 except ImportError:
@@ -88,24 +88,25 @@
 class TCPProxyClient:
     __slots__ = (
         "client_reader", "client_writer",
         "server_reader", "server_writer",
         "chunk_size", "tasks", "loop",
         "read_delay", "write_delay", "closing",
         "__processors", "__client_repr", "__server_repr",
+        "buffered",
     )
 
     @staticmethod
     async def _blank_processor(body: bytes) -> bytes:
         return body
 
     def __init__(
         self, client_reader: asyncio.StreamReader,
         client_writer: asyncio.StreamWriter,
-        chunk_size: int = 64 * 1024,
+        chunk_size: int = 64 * 1024, buffered: bool=False,
     ):
 
         self.loop = asyncio.get_event_loop()
         self.client_reader = client_reader  # type: asyncio.StreamReader
         self.client_writer = client_writer  # type: asyncio.StreamWriter
 
         self.server_reader = None  # type: t.Optional[asyncio.StreamReader]
@@ -118,14 +119,16 @@
 
         self.closing = self.loop.create_future()  # type: asyncio.Future
         self.__processors = {
             "read": self._blank_processor,
             "write": self._blank_processor,
         }  # type: t.Dict[str, t.Callable[[], ProxyProcessorType]]
 
+        self.buffered = bool(buffered)
+
         self.__client_repr = None
         self.__server_repr = None
 
     @property
     def read_processor(self) -> t.Callable[[], ProxyProcessorType]:
         return self.__processors["read"]
 
@@ -145,16 +148,17 @@
     def write_processor(self, value: t.Optional[ProxyProcessorType]) -> None:
         if value is None:
             self.__processors["write"] = self._blank_processor
             return
         self.__processors["write"] = aiomisc.awaitable(value)
 
     def __repr__(self):
-        return "<%s: %s => %s>" % (
-            self.__class__.__name__, self.__client_repr, self.__server_repr,
+        return "<%s[%x]: %s => %s>" % (
+            self.__class__.__name__, id(self),
+            self.__client_repr, self.__server_repr,
         )
 
     async def pipe(
         self, reader: asyncio.StreamReader,
         writer: asyncio.StreamWriter,
         processor: str,
         delay: Delay,
@@ -168,20 +172,24 @@
                         "%r sleeping %.3f seconds on %s",
                         self, delay.timeout, processor,
                     )
 
                 await delay.wait()
 
                 writer.write(await self.__processors[processor](chunk))
-                await writer.drain()
+
+                if not self.buffered:
+                    await writer.drain()
         finally:
             writer.close()
             await writer.wait_closed()
 
     async def connect(self, target_host: str, target_port: int) -> None:
+        log.debug("Establishing connection for %r", self)
+
         self.server_reader, self.server_writer = await asyncio.open_connection(
             host=target_host, port=target_port,
         )
 
         self.__client_repr = ":".join(
             map(str, self.client_writer.get_extra_info("peername")[:2]),
         )
@@ -205,62 +213,75 @@
                     "read",
                     self.read_delay,
                 ),
             ),
         )
 
     async def close(self):
+        log.debug("Closing %r", self)
         if self.closing.done():
             return
 
         await aiomisc.cancel_tasks(self.tasks)
         self.loop.call_soon(self.closing.set_result, True)
         await self.closing
 
 
 class TCPProxy:
     DEFAULT_TIMEOUT = 30
 
     __slots__ = (
         "proxy_port", "clients", "server", "proxy_host",
         "target_port", "target_host", "listen_host", "read_delay",
-        "write_delay", "read_processor", "write_processor",
+        "write_delay", "read_processor", "write_processor", "buffered",
     )
 
     def __init__(
         self, target_host: str, target_port: int,
-        listen_host: str = "127.0.0.1",
+        listen_host: str = "127.0.0.1", buffered: bool = True,
     ):
         self.target_port = target_port
         self.target_host = target_host
         self.proxy_host = listen_host
         self.proxy_port = get_unused_port()
         self.read_delay = 0
         self.write_delay = 0
+        self.buffered = buffered
 
         self.clients = set()  # type: t.Set[TCPProxyClient]
         self.server = None  # type: t.Optional[asyncio.AbstractServer]
 
         self.read_processor = None  # type: t.Optional[ProxyProcessorType]
         self.write_processor = None  # type: t.Optional[ProxyProcessorType]
 
+    def __repr__(self):
+        return "<%s[%x]: tcp://%s:%s => tcp://%s:%s>" % (
+            self.__class__.__name__, id(self),
+            self.proxy_host, self.proxy_port,
+            self.target_host, self.target_port,
+        )
+
     async def start(self, timeout=None) -> asyncio.AbstractServer:
+        log.debug("Starting %r", self)
         self.server = await asyncio.wait_for(
             asyncio.start_server(
                 self._handle_client,
                 host=self.proxy_host,
                 port=self.proxy_port,
             ), timeout=timeout,
         )
         return self.server
 
     ClientType = t.Tuple[asyncio.StreamReader, asyncio.StreamWriter]
 
     async def create_client(self) -> ClientType:
-        return await asyncio.open_connection(self.proxy_host, self.proxy_port)
+        log.debug("Creating client for %r", self)
+        return await asyncio.open_connection(
+            self.proxy_host, self.proxy_port,
+        )
 
     async def __aenter__(self):
         if self.server is None:
             await self.start(timeout=self.DEFAULT_TIMEOUT)
         return self
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
@@ -270,44 +291,62 @@
         async def close():
             await self.disconnect_all()
             self.server.close()
             await self.server.wait_closed()
         await asyncio.wait_for(close(), timeout=timeout)
 
     def set_delay(self, read_delay: DelayType, write_delay: DelayType = 0):
+        log.debug("Setting delay [R/W %f %f]", read_delay, write_delay)
+
         for client in self.clients:
+            log.debug(
+                "Applying delays [R/W: %f %f] for %r",
+                read_delay, write_delay, client,
+            )
             client.read_delay.timeout = read_delay
             client.write_delay.timeout = write_delay
+
         self.read_delay = read_delay
         self.write_delay = write_delay
 
     def set_content_processors(
         self, read: t.Optional[ProxyProcessorType],
         write: t.Optional[ProxyProcessorType],
     ):
+        log.debug(
+            "Setting content processors for %r: read=%r write=%r",
+            self, read, write,
+        )
         for client in self.clients:
+            log.debug(
+                "Applying context processors for %r: read=%r write=%r",
+                client, read, write,
+            )
             client.read_processor = read
             client.write_processor = write
 
         self.read_processor = read
         self.write_processor = write
 
     def disconnect_all(self) -> asyncio.Future:
+        log.debug(
+            "Disconnecting %s clients of %r", len(self.clients), self,
+        )
         return asyncio.ensure_future(
             asyncio.gather(
                 *[client.close() for client in self.clients],
                 return_exceptions=True
             ),
         )
 
     async def _handle_client(
         self, reader: asyncio.StreamReader,
         writer: asyncio.StreamWriter
     ):
-        client = TCPProxyClient(reader, writer)
+        client = TCPProxyClient(reader, writer, buffered=self.buffered)
         self.clients.add(client)
 
         client.read_delay.timeout = self.read_delay
         client.write_delay.timeout = self.write_delay
         client.read_processor = self.read_processor
         client.write_processor = self.write_processor
```

### Comparing `aiomisc-9.8.1/setup.py` & `aiomisc-9.8.4/setup.py`

 * *Files identical despite different names*

### Comparing `aiomisc-9.8.1/tests/pytest_plugin/test_loop_fixture.py` & `aiomisc-9.8.4/tests/pytest_plugin/test_loop_fixture.py`

 * *Files identical despite different names*

### Comparing `aiomisc-9.8.1/tests/pytest_plugin/test_tcp_proxy.py` & `aiomisc-9.8.4/tests/pytest_plugin/test_tcp_proxy.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 def services(service: HashServer):
     return [service]
 
 
 @pytest.fixture()
 @async_generator
 async def proxy(tcp_proxy, localhost, server_port):
-    async with tcp_proxy(localhost, server_port) as proxy:
+    async with tcp_proxy(localhost, server_port, buffered=True) as proxy:
         await yield_(proxy)
 
 
 async def test_proxy_client(proxy):
     reader, writer = await proxy.create_client()
     payload = b"Hello world"
```

### Comparing `aiomisc-9.8.1/tests/pytest_plugin/test_tcp_proxy_example.py` & `aiomisc-9.8.4/tests/pytest_plugin/test_tcp_proxy_example.py`

 * *Files identical despite different names*

