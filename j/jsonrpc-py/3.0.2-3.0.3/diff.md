# Comparing `tmp/jsonrpc-py-3.0.2.tar.gz` & `tmp/jsonrpc-py-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonrpc-py-3.0.2.tar", last modified: Sun Apr 23 01:27:52 2023, max compression
+gzip compressed data, was "jsonrpc-py-3.0.3.tar", last modified: Sun Apr 23 01:43:27 2023, max compression
```

## Comparing `jsonrpc-py-3.0.2.tar` & `jsonrpc-py-3.0.3.tar`

### file list

```diff
@@ -1,82 +1,83 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 01:27:52.947112 jsonrpc-py-3.0.2/
--rw-rw-rw-   0 root         (0) root         (0)      286 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/.flake8
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/.gitattributes
--rw-rw-rw-   0 root         (0) root         (0)      318 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1305 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1499 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)     1262 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/Makefile
--rw-r--r--   0 root         (0) root         (0)     2852 2023-04-23 01:27:52.947112 jsonrpc-py-3.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1453 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 01:27:52.925110 jsonrpc-py-3.0.2/docs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 01:27:52.918109 jsonrpc-py-3.0.2/docs/changelog/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 01:27:52.928110 jsonrpc-py-3.0.2/docs/changelog/v1.x.x/
--rw-rw-rw-   0 root         (0) root         (0)       98 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v1.x.x/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      156 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v1.x.x/v1.0.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      234 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v1.x.x/v1.0.1.rst
--rw-rw-rw-   0 root         (0) root         (0)      346 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v1.x.x/v1.0.2.rst
--rw-rw-rw-   0 root         (0) root         (0)      433 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v1.x.x/v1.0.3.rst
--rw-rw-rw-   0 root         (0) root         (0)      386 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v1.x.x/v1.0.4.rst
--rw-rw-rw-   0 root         (0) root         (0)      567 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v1.x.x/v1.1.0.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 01:27:52.936111 jsonrpc-py-3.0.2/docs/changelog/v2.x.x/
--rw-rw-rw-   0 root         (0) root         (0)      233 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v2.x.x/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      322 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v2.x.x/v2.0.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      539 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v2.x.x/v2.0.1.rst
--rw-rw-rw-   0 root         (0) root         (0)      420 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v2.x.x/v2.0.2.rst
--rw-rw-rw-   0 root         (0) root         (0)      421 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v2.x.x/v2.1.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      368 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v2.x.x/v2.2.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      368 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v2.x.x/v2.2.1.rst
--rw-rw-rw-   0 root         (0) root         (0)      182 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v2.x.x/v2.2.2.rst
--rw-rw-rw-   0 root         (0) root         (0)      397 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v2.x.x/v2.2.3.rst
--rw-rw-rw-   0 root         (0) root         (0)      669 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v2.x.x/v2.3.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      466 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v2.x.x/v2.4.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      345 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v2.x.x/v2.4.1.rst
--rw-rw-rw-   0 root         (0) root         (0)      263 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v2.x.x/v2.4.2.rst
--rw-rw-rw-   0 root         (0) root         (0)      314 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v2.x.x/v2.4.3.rst
--rw-rw-rw-   0 root         (0) root         (0)      152 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v2.x.x/v2.4.4.rst
--rw-rw-rw-   0 root         (0) root         (0)      320 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v2.x.x/v2.4.5.rst
--rw-rw-rw-   0 root         (0) root         (0)      270 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v2.x.x/v2.4.6.rst
--rw-rw-rw-   0 root         (0) root         (0)      289 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v2.x.x/v2.4.7.rst
--rw-rw-rw-   0 root         (0) root         (0)      321 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v2.x.x/v2.4.8.rst
--rw-rw-rw-   0 root         (0) root         (0)      154 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v2.x.x/v2.4.9.rst
--rw-rw-rw-   0 root         (0) root         (0)      284 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v2.x.x/v2.5.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      265 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v2.x.x/v2.5.1.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 01:27:52.937111 jsonrpc-py-3.0.2/docs/changelog/v3.x.x/
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v3.x.x/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      720 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v3.x.x/v3.0.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      278 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v3.x.x/v3.0.1.rst
--rw-rw-rw-   0 root         (0) root         (0)      211 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog/v3.x.x/v3.0.2.rst
--rw-rw-rw-   0 root         (0) root         (0)      696 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     1612 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     2623 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/deployment.rst
--rw-rw-rw-   0 root         (0) root         (0)     1752 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1861 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/quickstart.rst
--rw-rw-rw-   0 root         (0) root         (0)     1009 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/docs/reference.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 01:27:52.941112 jsonrpc-py-3.0.2/jsonrpc/
--rw-rw-rw-   0 root         (0) root         (0)      525 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/jsonrpc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9198 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/jsonrpc/asgi.py
--rw-rw-rw-   0 root         (0) root         (0)     4351 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/jsonrpc/dispatcher.py
--rw-rw-rw-   0 root         (0) root         (0)     2219 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/jsonrpc/errors.py
--rw-rw-rw-   0 root         (0) root         (0)       59 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/jsonrpc/py.typed
--rw-rw-rw-   0 root         (0) root         (0)     5734 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/jsonrpc/request.py
--rw-rw-rw-   0 root         (0) root         (0)     4055 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/jsonrpc/response.py
--rw-rw-rw-   0 root         (0) root         (0)     1706 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/jsonrpc/serializer.py
--rw-rw-rw-   0 root         (0) root         (0)     2877 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/jsonrpc/typedefs.py
--rw-rw-rw-   0 root         (0) root         (0)     1951 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/jsonrpc/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 01:27:52.943112 jsonrpc-py-3.0.2/jsonrpc_py.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2852 2023-04-23 01:27:52.000000 jsonrpc-py-3.0.2/jsonrpc_py.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1823 2023-04-23 01:27:52.000000 jsonrpc-py-3.0.2/jsonrpc_py.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 01:27:52.000000 jsonrpc-py-3.0.2/jsonrpc_py.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-23 01:27:52.000000 jsonrpc-py-3.0.2/jsonrpc_py.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1795 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      199 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/requirements-dev.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-23 01:27:52.947112 jsonrpc-py-3.0.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 01:27:52.946112 jsonrpc-py-3.0.2/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13845 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/tests/test_asgi.py
--rw-rw-rw-   0 root         (0) root         (0)     3580 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/tests/test_dispatcher.py
--rw-rw-rw-   0 root         (0) root         (0)     1917 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/tests/test_errors.py
--rw-rw-rw-   0 root         (0) root         (0)     8121 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/tests/test_request.py
--rw-rw-rw-   0 root         (0) root         (0)     5721 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/tests/test_response.py
--rw-rw-rw-   0 root         (0) root         (0)     1164 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/tests/test_serializer.py
--rw-rw-rw-   0 root         (0) root         (0)     2344 2023-04-23 01:27:30.000000 jsonrpc-py-3.0.2/tests/test_utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 01:43:27.436999 jsonrpc-py-3.0.3/
+-rw-rw-rw-   0 root         (0) root         (0)      286 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/.flake8
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/.gitattributes
+-rw-rw-rw-   0 root         (0) root         (0)      318 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1305 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1499 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)     1262 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/Makefile
+-rw-r--r--   0 root         (0) root         (0)     2852 2023-04-23 01:43:27.436999 jsonrpc-py-3.0.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1453 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 01:43:27.416000 jsonrpc-py-3.0.3/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 01:43:27.409000 jsonrpc-py-3.0.3/docs/changelog/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 01:43:27.419000 jsonrpc-py-3.0.3/docs/changelog/v1.x.x/
+-rw-rw-rw-   0 root         (0) root         (0)       98 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v1.x.x/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      156 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v1.x.x/v1.0.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      234 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v1.x.x/v1.0.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      346 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v1.x.x/v1.0.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)      433 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v1.x.x/v1.0.3.rst
+-rw-rw-rw-   0 root         (0) root         (0)      386 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v1.x.x/v1.0.4.rst
+-rw-rw-rw-   0 root         (0) root         (0)      567 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v1.x.x/v1.1.0.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 01:43:27.426999 jsonrpc-py-3.0.3/docs/changelog/v2.x.x/
+-rw-rw-rw-   0 root         (0) root         (0)      233 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v2.x.x/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      322 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v2.x.x/v2.0.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      539 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v2.x.x/v2.0.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      420 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v2.x.x/v2.0.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)      421 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v2.x.x/v2.1.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      368 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v2.x.x/v2.2.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      368 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v2.x.x/v2.2.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      182 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v2.x.x/v2.2.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)      397 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v2.x.x/v2.2.3.rst
+-rw-rw-rw-   0 root         (0) root         (0)      669 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v2.x.x/v2.3.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      466 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v2.x.x/v2.4.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      345 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v2.x.x/v2.4.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      263 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v2.x.x/v2.4.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)      314 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v2.x.x/v2.4.3.rst
+-rw-rw-rw-   0 root         (0) root         (0)      152 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v2.x.x/v2.4.4.rst
+-rw-rw-rw-   0 root         (0) root         (0)      320 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v2.x.x/v2.4.5.rst
+-rw-rw-rw-   0 root         (0) root         (0)      270 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v2.x.x/v2.4.6.rst
+-rw-rw-rw-   0 root         (0) root         (0)      289 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v2.x.x/v2.4.7.rst
+-rw-rw-rw-   0 root         (0) root         (0)      321 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v2.x.x/v2.4.8.rst
+-rw-rw-rw-   0 root         (0) root         (0)      154 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v2.x.x/v2.4.9.rst
+-rw-rw-rw-   0 root         (0) root         (0)      284 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v2.x.x/v2.5.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      265 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v2.x.x/v2.5.1.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 01:43:27.429000 jsonrpc-py-3.0.3/docs/changelog/v3.x.x/
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v3.x.x/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      720 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v3.x.x/v3.0.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      278 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v3.x.x/v3.0.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      211 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v3.x.x/v3.0.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)      206 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v3.x.x/v3.0.3.rst
+-rw-rw-rw-   0 root         (0) root         (0)      696 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1612 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2623 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/deployment.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1752 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1861 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/quickstart.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1009 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/reference.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 01:43:27.431999 jsonrpc-py-3.0.3/jsonrpc/
+-rw-rw-rw-   0 root         (0) root         (0)      525 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/jsonrpc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9198 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/jsonrpc/asgi.py
+-rw-rw-rw-   0 root         (0) root         (0)     4351 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/jsonrpc/dispatcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     2219 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/jsonrpc/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)       59 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/jsonrpc/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     5734 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/jsonrpc/request.py
+-rw-rw-rw-   0 root         (0) root         (0)     4055 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/jsonrpc/response.py
+-rw-rw-rw-   0 root         (0) root         (0)     1706 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/jsonrpc/serializer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2877 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/jsonrpc/typedefs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1951 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/jsonrpc/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 01:43:27.433999 jsonrpc-py-3.0.3/jsonrpc_py.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2852 2023-04-23 01:43:27.000000 jsonrpc-py-3.0.3/jsonrpc_py.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1856 2023-04-23 01:43:27.000000 jsonrpc-py-3.0.3/jsonrpc_py.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 01:43:27.000000 jsonrpc-py-3.0.3/jsonrpc_py.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-23 01:43:27.000000 jsonrpc-py-3.0.3/jsonrpc_py.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1795 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      199 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/requirements-dev.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-23 01:43:27.436999 jsonrpc-py-3.0.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 01:43:27.435999 jsonrpc-py-3.0.3/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13845 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/tests/test_asgi.py
+-rw-rw-rw-   0 root         (0) root         (0)     3580 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/tests/test_dispatcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     1917 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/tests/test_errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     8121 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/tests/test_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     5721 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/tests/test_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     1164 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/tests/test_serializer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2344 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/tests/test_utilities.py
```

### Comparing `jsonrpc-py-3.0.2/.gitlab-ci.yml` & `jsonrpc-py-3.0.3/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.2/LICENSE` & `jsonrpc-py-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.2/Makefile` & `jsonrpc-py-3.0.3/Makefile`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.2/PKG-INFO` & `jsonrpc-py-3.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonrpc-py
-Version: 3.0.2
+Version: 3.0.3
 Summary: Pure zero-dependency JSON-RPC 2.0 implementation
 Author-email: Andrew Malchuk <andrew.malchuk@yandex.ru>
 Maintainer-email: JSON-RPC Development Group <dev@jsonrpc.ru>
 License: BSD-3-Clause
 Project-URL: Source Code, https://gitlab.com/jsonrpc/jsonrpc-py
 Project-URL: Documentation, https://docs.jsonrpc.ru
 Project-URL: Change Log, https://docs.jsonrpc.ru/changelog.html
```

### Comparing `jsonrpc-py-3.0.2/README.md` & `jsonrpc-py-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.2/docs/changelog/v1.x.x/v1.1.0.rst` & `jsonrpc-py-3.0.3/docs/changelog/v1.x.x/v1.1.0.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.2/docs/changelog/v2.x.x/v2.0.1.rst` & `jsonrpc-py-3.0.3/docs/changelog/v2.x.x/v2.0.1.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.2/docs/changelog/v2.x.x/v2.3.0.rst` & `jsonrpc-py-3.0.3/docs/changelog/v2.x.x/v2.3.0.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.2/docs/changelog/v3.x.x/v3.0.0.rst` & `jsonrpc-py-3.0.3/docs/changelog/v3.x.x/v3.0.0.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.2/docs/changelog.rst` & `jsonrpc-py-3.0.3/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.2/docs/conf.py` & `jsonrpc-py-3.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.2/docs/deployment.rst` & `jsonrpc-py-3.0.3/docs/deployment.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.2/docs/index.rst` & `jsonrpc-py-3.0.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.2/docs/quickstart.rst` & `jsonrpc-py-3.0.3/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.2/docs/reference.rst` & `jsonrpc-py-3.0.3/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.2/jsonrpc/__init__.py` & `jsonrpc-py-3.0.3/jsonrpc/__init__.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.2/jsonrpc/asgi.py` & `jsonrpc-py-3.0.3/jsonrpc/asgi.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.2/jsonrpc/dispatcher.py` & `jsonrpc-py-3.0.3/jsonrpc/dispatcher.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.2/jsonrpc/errors.py` & `jsonrpc-py-3.0.3/jsonrpc/errors.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.2/jsonrpc/request.py` & `jsonrpc-py-3.0.3/jsonrpc/request.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.2/jsonrpc/response.py` & `jsonrpc-py-3.0.3/jsonrpc/response.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.2/jsonrpc/serializer.py` & `jsonrpc-py-3.0.3/jsonrpc/serializer.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.2/jsonrpc/typedefs.py` & `jsonrpc-py-3.0.3/jsonrpc/typedefs.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.2/jsonrpc/utilities.py` & `jsonrpc-py-3.0.3/jsonrpc/utilities.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.2/jsonrpc_py.egg-info/PKG-INFO` & `jsonrpc-py-3.0.3/jsonrpc_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonrpc-py
-Version: 3.0.2
+Version: 3.0.3
 Summary: Pure zero-dependency JSON-RPC 2.0 implementation
 Author-email: Andrew Malchuk <andrew.malchuk@yandex.ru>
 Maintainer-email: JSON-RPC Development Group <dev@jsonrpc.ru>
 License: BSD-3-Clause
 Project-URL: Source Code, https://gitlab.com/jsonrpc/jsonrpc-py
 Project-URL: Documentation, https://docs.jsonrpc.ru
 Project-URL: Change Log, https://docs.jsonrpc.ru/changelog.html
```

### Comparing `jsonrpc-py-3.0.2/jsonrpc_py.egg-info/SOURCES.txt` & `jsonrpc-py-3.0.3/jsonrpc_py.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 docs/changelog/v2.x.x/v2.4.9.rst
 docs/changelog/v2.x.x/v2.5.0.rst
 docs/changelog/v2.x.x/v2.5.1.rst
 docs/changelog/v3.x.x/index.rst
 docs/changelog/v3.x.x/v3.0.0.rst
 docs/changelog/v3.x.x/v3.0.1.rst
 docs/changelog/v3.x.x/v3.0.2.rst
+docs/changelog/v3.x.x/v3.0.3.rst
 jsonrpc/__init__.py
 jsonrpc/asgi.py
 jsonrpc/dispatcher.py
 jsonrpc/errors.py
 jsonrpc/py.typed
 jsonrpc/request.py
 jsonrpc/response.py
```

### Comparing `jsonrpc-py-3.0.2/pyproject.toml` & `jsonrpc-py-3.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.2/tests/test_asgi.py` & `jsonrpc-py-3.0.3/tests/test_asgi.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.2/tests/test_dispatcher.py` & `jsonrpc-py-3.0.3/tests/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.2/tests/test_errors.py` & `jsonrpc-py-3.0.3/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.2/tests/test_request.py` & `jsonrpc-py-3.0.3/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.2/tests/test_response.py` & `jsonrpc-py-3.0.3/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.2/tests/test_serializer.py` & `jsonrpc-py-3.0.3/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.2/tests/test_utilities.py` & `jsonrpc-py-3.0.3/tests/test_utilities.py`

 * *Files identical despite different names*

