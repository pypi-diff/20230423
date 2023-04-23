# Comparing `tmp/nendo-0.0.1.tar.gz` & `tmp/nendo-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nendo-0.0.1.tar", last modified: Mon Mar 27 21:35:50 2023, max compression
+gzip compressed data, was "nendo-0.0.2.tar", max compression
```

## Comparing `nendo-0.0.1.tar` & `nendo-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,9 @@
-drwxr-xr-x   0 sh8       (1000) sh8       (1000)        0 2023-03-27 21:35:50.136032 nendo-0.0.1/
--rw-r--r--   0 sh8       (1000) sh8       (1000)     1073 2023-03-27 21:33:18.000000 nendo-0.0.1/LICENSE
--rw-r--r--   0 sh8       (1000) sh8       (1000)      579 2023-03-27 21:35:50.135032 nendo-0.0.1/PKG-INFO
--rw-r--r--   0 sh8       (1000) sh8       (1000)       54 2023-03-27 21:33:51.000000 nendo-0.0.1/README.md
--rw-r--r--   0 sh8       (1000) sh8       (1000)      616 2023-03-27 21:33:18.000000 nendo-0.0.1/pyproject.toml
--rw-r--r--   0 sh8       (1000) sh8       (1000)       38 2023-03-27 21:35:50.136032 nendo-0.0.1/setup.cfg
-drwxr-xr-x   0 sh8       (1000) sh8       (1000)        0 2023-03-27 21:35:50.134032 nendo-0.0.1/src/
-drwxr-xr-x   0 sh8       (1000) sh8       (1000)        0 2023-03-27 21:35:50.135032 nendo-0.0.1/src/nendo/
--rw-r--r--   0 sh8       (1000) sh8       (1000)      118 2023-03-27 21:35:04.000000 nendo-0.0.1/src/nendo/__init__.py
--rw-r--r--   0 sh8       (1000) sh8       (1000)      284 2023-03-27 21:35:14.000000 nendo-0.0.1/src/nendo/core.py
-drwxr-xr-x   0 sh8       (1000) sh8       (1000)        0 2023-03-27 21:35:50.135032 nendo-0.0.1/src/nendo.egg-info/
--rw-r--r--   0 sh8       (1000) sh8       (1000)      579 2023-03-27 21:35:50.000000 nendo-0.0.1/src/nendo.egg-info/PKG-INFO
--rw-r--r--   0 sh8       (1000) sh8       (1000)      204 2023-03-27 21:35:50.000000 nendo-0.0.1/src/nendo.egg-info/SOURCES.txt
--rw-r--r--   0 sh8       (1000) sh8       (1000)        1 2023-03-27 21:35:50.000000 nendo-0.0.1/src/nendo.egg-info/dependency_links.txt
--rw-r--r--   0 sh8       (1000) sh8       (1000)        6 2023-03-27 21:35:50.000000 nendo-0.0.1/src/nendo.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1073 2023-03-27 20:51:34.595817 nendo-0.0.2/LICENSE
+-rw-r--r--   0        0        0     3160 2023-04-23 00:48:26.855126 nendo-0.0.2/README.md
+-rw-r--r--   0        0        0     1319 2023-04-23 10:18:55.315019 nendo-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      465 2023-04-23 00:06:26.661112 nendo-0.0.2/src/nendo/__init__.py
+-rw-r--r--   0        0        0      547 2023-04-22 23:11:10.596093 nendo-0.0.2/src/nendo/config.py
+-rw-r--r--   0        0        0     2130 2023-04-23 00:05:55.439112 nendo-0.0.2/src/nendo/core.py
+-rw-r--r--   0        0        0     6486 2023-04-23 10:05:12.928015 nendo-0.0.2/src/nendo/schema.py
+-rw-r--r--   0        0        0      209 2023-04-22 23:57:14.679109 nendo-0.0.2/src/nendo/utils.py
+-rw-r--r--   0        0        0     4382 1970-01-01 00:00:00.000000 nendo-0.0.2/PKG-INFO
```

### Comparing `nendo-0.0.1/LICENSE` & `nendo-0.0.2/LICENSE`

 * *Files identical despite different names*

