# Comparing `tmp/jsonrpc-py-3.0.1.tar.gz` & `tmp/jsonrpc-py-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonrpc-py-3.0.1.tar", last modified: Wed Apr 19 09:30:06 2023, max compression
+gzip compressed data, was "jsonrpc-py-3.0.2.tar", last modified: Sun Apr 23 01:27:52 2023, max compression
```

## Comparing `jsonrpc-py-3.0.1.tar` & `jsonrpc-py-3.0.2.tar`

### file list

```diff
@@ -1,36 +1,82 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:30:06.029232 jsonrpc-py-3.0.1/
--rw-rw-rw-   0 root         (0) root         (0)     1499 2023-04-19 09:29:54.000000 jsonrpc-py-3.0.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       43 2023-04-19 09:29:54.000000 jsonrpc-py-3.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2937 2023-04-19 09:30:06.030149 jsonrpc-py-3.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1453 2023-04-19 09:29:54.000000 jsonrpc-py-3.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:30:06.025565 jsonrpc-py-3.0.1/jsonrpc/
--rw-rw-rw-   0 root         (0) root         (0)      501 2023-04-19 09:29:54.000000 jsonrpc-py-3.0.1/jsonrpc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9198 2023-04-19 09:29:54.000000 jsonrpc-py-3.0.1/jsonrpc/asgi.py
--rw-rw-rw-   0 root         (0) root         (0)     4351 2023-04-19 09:29:54.000000 jsonrpc-py-3.0.1/jsonrpc/dispatcher.py
--rw-rw-rw-   0 root         (0) root         (0)     2219 2023-04-19 09:29:54.000000 jsonrpc-py-3.0.1/jsonrpc/errors.py
--rw-rw-rw-   0 root         (0) root         (0)       59 2023-04-19 09:29:54.000000 jsonrpc-py-3.0.1/jsonrpc/py.typed
--rw-rw-rw-   0 root         (0) root         (0)     5746 2023-04-19 09:29:54.000000 jsonrpc-py-3.0.1/jsonrpc/request.py
--rw-rw-rw-   0 root         (0) root         (0)     4055 2023-04-19 09:29:54.000000 jsonrpc-py-3.0.1/jsonrpc/response.py
--rw-rw-rw-   0 root         (0) root         (0)     1706 2023-04-19 09:29:54.000000 jsonrpc-py-3.0.1/jsonrpc/serializer.py
--rw-rw-rw-   0 root         (0) root         (0)     2877 2023-04-19 09:29:54.000000 jsonrpc-py-3.0.1/jsonrpc/typedefs.py
--rw-rw-rw-   0 root         (0) root         (0)     1951 2023-04-19 09:29:54.000000 jsonrpc-py-3.0.1/jsonrpc/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:30:06.027398 jsonrpc-py-3.0.1/jsonrpc_py.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2937 2023-04-19 09:30:05.000000 jsonrpc-py-3.0.1/jsonrpc_py.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      658 2023-04-19 09:30:05.000000 jsonrpc-py-3.0.1/jsonrpc_py.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 09:30:05.000000 jsonrpc-py-3.0.1/jsonrpc_py.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 09:30:05.000000 jsonrpc-py-3.0.1/jsonrpc_py.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      134 2023-04-19 09:30:05.000000 jsonrpc-py-3.0.1/jsonrpc_py.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-19 09:30:05.000000 jsonrpc-py-3.0.1/jsonrpc_py.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      389 2023-04-19 09:29:54.000000 jsonrpc-py-3.0.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      127 2023-04-19 09:29:54.000000 jsonrpc-py-3.0.1/requirements-dev.txt
--rw-rw-rw-   0 root         (0) root         (0)     1572 2023-04-19 09:30:06.030149 jsonrpc-py-3.0.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)       61 2023-04-19 09:29:54.000000 jsonrpc-py-3.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:30:06.029232 jsonrpc-py-3.0.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 09:29:54.000000 jsonrpc-py-3.0.1/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13845 2023-04-19 09:29:54.000000 jsonrpc-py-3.0.1/tests/test_asgi.py
--rw-rw-rw-   0 root         (0) root         (0)     3580 2023-04-19 09:29:54.000000 jsonrpc-py-3.0.1/tests/test_dispatcher.py
--rw-rw-rw-   0 root         (0) root         (0)     1917 2023-04-19 09:29:54.000000 jsonrpc-py-3.0.1/tests/test_errors.py
--rw-rw-rw-   0 root         (0) root         (0)     8121 2023-04-19 09:29:54.000000 jsonrpc-py-3.0.1/tests/test_request.py
--rw-rw-rw-   0 root         (0) root         (0)     5721 2023-04-19 09:29:54.000000 jsonrpc-py-3.0.1/tests/test_response.py
--rw-rw-rw-   0 root         (0) root         (0)     1164 2023-04-19 09:29:54.000000 jsonrpc-py-3.0.1/tests/test_serializer.py
--rw-rw-rw-   0 root         (0) root         (0)     2344 2023-04-19 09:29:54.000000 jsonrpc-py-3.0.1/tests/test_utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 01:27:52.947112 jsonrpc-py-3.0.2/
+-rw-rw-rw-   0 root         (0) root         (0)      286 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/.flake8
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/.gitattributes
+-rw-rw-rw-   0 root         (0) root         (0)      318 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1305 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1499 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)     1262 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/Makefile
+-rw-r--r--   0 root         (0) root         (0)     2852 2023-04-23 01:27:52.947112 jsonrpc-py-3.0.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1453 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 01:27:52.925110 jsonrpc-py-3.0.2/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 01:27:52.918109 jsonrpc-py-3.0.2/docs/changelog/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 01:27:52.928110 jsonrpc-py-3.0.2/docs/changelog/v1.x.x/
+-rw-rw-rw-   0 root         (0) root         (0)       98 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v1.x.x/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      156 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v1.x.x/v1.0.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      234 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v1.x.x/v1.0.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      346 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v1.x.x/v1.0.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)      433 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v1.x.x/v1.0.3.rst
+-rw-rw-rw-   0 root         (0) root         (0)      386 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v1.x.x/v1.0.4.rst
+-rw-rw-rw-   0 root         (0) root         (0)      567 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v1.x.x/v1.1.0.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 01:27:52.936111 jsonrpc-py-3.0.2/docs/changelog/v2.x.x/
+-rw-rw-rw-   0 root         (0) root         (0)      233 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v2.x.x/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      322 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v2.x.x/v2.0.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      539 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v2.x.x/v2.0.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      420 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v2.x.x/v2.0.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)      421 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v2.x.x/v2.1.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      368 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v2.x.x/v2.2.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      368 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v2.x.x/v2.2.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      182 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v2.x.x/v2.2.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)      397 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v2.x.x/v2.2.3.rst
+-rw-rw-rw-   0 root         (0) root         (0)      669 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v2.x.x/v2.3.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      466 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v2.x.x/v2.4.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      345 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v2.x.x/v2.4.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      263 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v2.x.x/v2.4.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)      314 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v2.x.x/v2.4.3.rst
+-rw-rw-rw-   0 root         (0) root         (0)      152 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v2.x.x/v2.4.4.rst
+-rw-rw-rw-   0 root         (0) root         (0)      320 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v2.x.x/v2.4.5.rst
+-rw-rw-rw-   0 root         (0) root         (0)      270 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v2.x.x/v2.4.6.rst
+-rw-rw-rw-   0 root         (0) root         (0)      289 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v2.x.x/v2.4.7.rst
+-rw-rw-rw-   0 root         (0) root         (0)      321 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v2.x.x/v2.4.8.rst
+-rw-rw-rw-   0 root         (0) root         (0)      154 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v2.x.x/v2.4.9.rst
+-rw-rw-rw-   0 root         (0) root         (0)      284 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v2.x.x/v2.5.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      265 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v2.x.x/v2.5.1.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 01:27:52.937111 jsonrpc-py-3.0.2/docs/changelog/v3.x.x/
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v3.x.x/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      720 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v3.x.x/v3.0.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      278 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v3.x.x/v3.0.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      211 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v3.x.x/v3.0.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)      696 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1612 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2623 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/deployment.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1752 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1861 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/quickstart.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1009 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/reference.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 01:27:52.941112 jsonrpc-py-3.0.2/jsonrpc/
+-rw-rw-rw-   0 root         (0) root         (0)      525 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/jsonrpc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9198 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/jsonrpc/asgi.py
+-rw-rw-rw-   0 root         (0) root         (0)     4351 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/jsonrpc/dispatcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     2219 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/jsonrpc/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)       59 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/jsonrpc/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     5734 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/jsonrpc/request.py
+-rw-rw-rw-   0 root         (0) root         (0)     4055 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/jsonrpc/response.py
+-rw-rw-rw-   0 root         (0) root         (0)     1706 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/jsonrpc/serializer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2877 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/jsonrpc/typedefs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1951 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/jsonrpc/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 01:27:52.943112 jsonrpc-py-3.0.2/jsonrpc_py.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2852 2023-04-23 01:27:52.000000 jsonrpc-py-3.0.2/jsonrpc_py.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1823 2023-04-23 01:27:52.000000 jsonrpc-py-3.0.2/jsonrpc_py.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 01:27:52.000000 jsonrpc-py-3.0.2/jsonrpc_py.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-23 01:27:52.000000 jsonrpc-py-3.0.2/jsonrpc_py.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1795 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      199 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/requirements-dev.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-23 01:27:52.947112 jsonrpc-py-3.0.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 01:27:52.946112 jsonrpc-py-3.0.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13845 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/tests/test_asgi.py
+-rw-rw-rw-   0 root         (0) root         (0)     3580 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/tests/test_dispatcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     1917 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/tests/test_errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     8121 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/tests/test_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     5721 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/tests/test_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     1164 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/tests/test_serializer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2344 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/tests/test_utilities.py
```

### Comparing `jsonrpc-py-3.0.1/LICENSE` & `jsonrpc-py-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.1/PKG-INFO` & `jsonrpc-py-3.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 Metadata-Version: 2.1
 Name: jsonrpc-py
-Version: 3.0.1
+Version: 3.0.2
 Summary: Pure zero-dependency JSON-RPC 2.0 implementation
-Home-page: https://docs.jsonrpc.ru
-Author: Andrew Malchuk
-Author-email: andrew.malchuk@yandex.ru
-Maintainer: JSON-RPC Development Group
-Maintainer-email: dev@jsonrpc.ru
+Author-email: Andrew Malchuk <andrew.malchuk@yandex.ru>
+Maintainer-email: JSON-RPC Development Group <dev@jsonrpc.ru>
 License: BSD-3-Clause
 Project-URL: Source Code, https://gitlab.com/jsonrpc/jsonrpc-py
 Project-URL: Documentation, https://docs.jsonrpc.ru
 Project-URL: Change Log, https://docs.jsonrpc.ru/changelog.html
-Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -27,15 +23,14 @@
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
 
 JSON-RPC Python
 ===============
 [![pipeline status][pipeline]][homepage]
 [![coverage report][coverage]][homepage]
 [![latest release][version]][pypi]
```

### Comparing `jsonrpc-py-3.0.1/README.md` & `jsonrpc-py-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.1/jsonrpc/asgi.py` & `jsonrpc-py-3.0.2/jsonrpc/asgi.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.1/jsonrpc/dispatcher.py` & `jsonrpc-py-3.0.2/jsonrpc/dispatcher.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.1/jsonrpc/errors.py` & `jsonrpc-py-3.0.2/jsonrpc/errors.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.1/jsonrpc/request.py` & `jsonrpc-py-3.0.2/jsonrpc/request.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     """
 
     #: The :py:class:`str` object containing the name of the method.
     method: str
     #: The object of type :py:class:`list` or :py:class:`dict` that holds the parameter values
     #: to be used during the invocation of the method.
     #: May be omitted if provided method has no parameters for example.
-    params: list[object] | dict[str, object] | UndefinedType = Undefined
+    params: list[Any] | dict[str, Any] | UndefinedType = Undefined
     #: The :py:class:`str` object or any type of :py:class:`numbers.Number` object which represents an identifier
     #: of the request instance. May be omitted. If its value omitted, the request assumed to be a notification.
     request_id: str | float | UndefinedType = Undefined
 
     def __post_init__(self) -> None:
         self._validate_method()
         self._validate_params()
@@ -56,22 +56,22 @@
         if not isinstance(self.request_id, str | Number | UndefinedType):
             raise Error(
                 code=ErrorEnum.INVALID_REQUEST,
                 message=f"Request id must be an optional string or number, not a {type(self.request_id).__name__!r}",
             )
 
     @property
-    def args(self) -> tuple[object, ...]:
+    def args(self) -> tuple[Any, ...]:
         """
         Returns the :py:class:`tuple` object containing positional arguments of the method.
         """
         return tuple(params) if isinstance(params := self.params, MutableSequence) else ()
 
     @property
-    def kwargs(self) -> dict[str, object]:
+    def kwargs(self) -> dict[str, Any]:
         """
         Returns the :py:class:`dict` object containing keyword arguments of the method.
         """
         return params if isinstance(params := self.params, MutableMapping) else {}
 
     @property
     def is_notification(self) -> bool:
```

### Comparing `jsonrpc-py-3.0.1/jsonrpc/response.py` & `jsonrpc-py-3.0.2/jsonrpc/response.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.1/jsonrpc/serializer.py` & `jsonrpc-py-3.0.2/jsonrpc/serializer.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.1/jsonrpc/typedefs.py` & `jsonrpc-py-3.0.2/jsonrpc/typedefs.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.1/jsonrpc/utilities.py` & `jsonrpc-py-3.0.2/jsonrpc/utilities.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.1/jsonrpc_py.egg-info/PKG-INFO` & `jsonrpc-py-3.0.2/jsonrpc_py.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 Metadata-Version: 2.1
 Name: jsonrpc-py
-Version: 3.0.1
+Version: 3.0.2
 Summary: Pure zero-dependency JSON-RPC 2.0 implementation
-Home-page: https://docs.jsonrpc.ru
-Author: Andrew Malchuk
-Author-email: andrew.malchuk@yandex.ru
-Maintainer: JSON-RPC Development Group
-Maintainer-email: dev@jsonrpc.ru
+Author-email: Andrew Malchuk <andrew.malchuk@yandex.ru>
+Maintainer-email: JSON-RPC Development Group <dev@jsonrpc.ru>
 License: BSD-3-Clause
 Project-URL: Source Code, https://gitlab.com/jsonrpc/jsonrpc-py
 Project-URL: Documentation, https://docs.jsonrpc.ru
 Project-URL: Change Log, https://docs.jsonrpc.ru/changelog.html
-Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -27,15 +23,14 @@
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
 
 JSON-RPC Python
 ===============
 [![pipeline status][pipeline]][homepage]
 [![coverage report][coverage]][homepage]
 [![latest release][version]][pypi]
```

### Comparing `jsonrpc-py-3.0.1/tests/test_asgi.py` & `jsonrpc-py-3.0.2/tests/test_asgi.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.1/tests/test_dispatcher.py` & `jsonrpc-py-3.0.2/tests/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.1/tests/test_errors.py` & `jsonrpc-py-3.0.2/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.1/tests/test_request.py` & `jsonrpc-py-3.0.2/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.1/tests/test_response.py` & `jsonrpc-py-3.0.2/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.1/tests/test_serializer.py` & `jsonrpc-py-3.0.2/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.1/tests/test_utilities.py` & `jsonrpc-py-3.0.2/tests/test_utilities.py`

 * *Files identical despite different names*

