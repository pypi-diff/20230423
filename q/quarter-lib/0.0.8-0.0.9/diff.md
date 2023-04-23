# Comparing `tmp/quarter_lib-0.0.8.tar.gz` & `tmp/quarter_lib-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quarter_lib-0.0.8.tar", last modified: Sun Apr 23 15:15:29 2023, max compression
+gzip compressed data, was "quarter_lib-0.0.9.tar", last modified: Sun Apr 23 15:25:17 2023, max compression
```

## Comparing `quarter_lib-0.0.8.tar` & `quarter_lib-0.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:15:29.417152 quarter_lib-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:15:29.417152 quarter_lib-0.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:15:29.417152 quarter_lib-0.0.8/.github/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1448 2023-04-23 15:15:21.000000 quarter_lib-0.0.8/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:15:29.417152 quarter_lib-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-23 15:15:21.000000 quarter_lib-0.0.8/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-23 15:15:21.000000 quarter_lib-0.0.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-23 15:15:21.000000 quarter_lib-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 15:15:21.000000 quarter_lib-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-23 15:15:29.417152 quarter_lib-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-23 15:15:21.000000 quarter_lib-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-23 15:15:21.000000 quarter_lib-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-23 15:15:29.417152 quarter_lib-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:15:29.417152 quarter_lib-0.0.8/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 15:15:21.000000 quarter_lib-0.0.8/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:15:29.417152 quarter_lib-0.0.8/src/quarter_lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 15:15:21.000000 quarter_lib-0.0.8/src/quarter_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:15:29.417152 quarter_lib-0.0.8/src/quarter_lib/akeyless/
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-23 15:15:21.000000 quarter_lib-0.0.8/src/quarter_lib/akeyless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-23 15:15:21.000000 quarter_lib-0.0.8/src/quarter_lib/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:15:29.417152 quarter_lib-0.0.8/src/quarter_lib/google/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-23 15:15:21.000000 quarter_lib-0.0.8/src/quarter_lib/google/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:15:29.417152 quarter_lib-0.0.8/src/quarter_lib/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-23 15:15:21.000000 quarter_lib-0.0.8/src/quarter_lib/logging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:15:29.417152 quarter_lib-0.0.8/src/quarter_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-23 15:15:29.000000 quarter_lib-0.0.8/src/quarter_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-23 15:15:29.000000 quarter_lib-0.0.8/src/quarter_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 15:15:29.000000 quarter_lib-0.0.8/src/quarter_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-23 15:15:29.000000 quarter_lib-0.0.8/src/quarter_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:25:17.274319 quarter_lib-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:25:17.274319 quarter_lib-0.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:25:17.274319 quarter_lib-0.0.9/.github/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1448 2023-04-23 15:25:07.000000 quarter_lib-0.0.9/.github/scripts/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:25:17.274319 quarter_lib-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-23 15:25:07.000000 quarter_lib-0.0.9/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-23 15:25:07.000000 quarter_lib-0.0.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-23 15:25:07.000000 quarter_lib-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 15:25:07.000000 quarter_lib-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-23 15:25:17.278319 quarter_lib-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-23 15:25:07.000000 quarter_lib-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-23 15:25:07.000000 quarter_lib-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-23 15:25:17.278319 quarter_lib-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:25:17.274319 quarter_lib-0.0.9/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 15:25:07.000000 quarter_lib-0.0.9/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:25:17.274319 quarter_lib-0.0.9/src/quarter_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 15:25:07.000000 quarter_lib-0.0.9/src/quarter_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:25:17.274319 quarter_lib-0.0.9/src/quarter_lib/akeyless/
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-04-23 15:25:07.000000 quarter_lib-0.0.9/src/quarter_lib/akeyless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-23 15:25:07.000000 quarter_lib-0.0.9/src/quarter_lib/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:25:17.274319 quarter_lib-0.0.9/src/quarter_lib/google/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-23 15:25:07.000000 quarter_lib-0.0.9/src/quarter_lib/google/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:25:17.274319 quarter_lib-0.0.9/src/quarter_lib/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-23 15:25:07.000000 quarter_lib-0.0.9/src/quarter_lib/logging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:25:17.274319 quarter_lib-0.0.9/src/quarter_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-23 15:25:17.000000 quarter_lib-0.0.9/src/quarter_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-23 15:25:17.000000 quarter_lib-0.0.9/src/quarter_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 15:25:17.000000 quarter_lib-0.0.9/src/quarter_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-23 15:25:17.000000 quarter_lib-0.0.9/src/quarter_lib.egg-info/top_level.txt
```

### Comparing `quarter_lib-0.0.8/.github/scripts/release.py` & `quarter_lib-0.0.9/.github/scripts/release.py`

 * *Files identical despite different names*

### Comparing `quarter_lib-0.0.8/.gitignore` & `quarter_lib-0.0.9/.gitignore`

 * *Files identical despite different names*

