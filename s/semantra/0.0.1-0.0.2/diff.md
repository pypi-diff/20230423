# Comparing `tmp/semantra-0.0.1.tar.gz` & `tmp/semantra-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantra-0.0.1.tar", last modified: Sun Apr  9 15:53:27 2023, max compression
+gzip compressed data, was "semantra-0.0.2.tar", last modified: Sun Apr 23 04:17:17 2023, max compression
```

## Comparing `semantra-0.0.1.tar` & `semantra-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,17 @@
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-09 15:53:27.448400 semantra-0.0.1/
--rw-r--r--   0 freedmand   (501) staff       (20)     1071 2023-03-31 03:28:18.000000 semantra-0.0.1/LICENSE
--rw-r--r--   0 freedmand   (501) staff       (20)      267 2023-04-09 15:53:27.448261 semantra-0.0.1/PKG-INFO
--rw-r--r--   0 freedmand   (501) staff       (20)       53 2023-04-09 15:23:10.000000 semantra-0.0.1/README.md
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-09 15:53:27.448091 semantra-0.0.1/semantra.egg-info/
--rw-r--r--   0 freedmand   (501) staff       (20)      267 2023-04-09 15:53:27.000000 semantra-0.0.1/semantra.egg-info/PKG-INFO
--rw-r--r--   0 freedmand   (501) staff       (20)      154 2023-04-09 15:53:27.000000 semantra-0.0.1/semantra.egg-info/SOURCES.txt
--rw-r--r--   0 freedmand   (501) staff       (20)        1 2023-04-09 15:53:27.000000 semantra-0.0.1/semantra.egg-info/dependency_links.txt
--rw-r--r--   0 freedmand   (501) staff       (20)        1 2023-04-09 15:53:27.000000 semantra-0.0.1/semantra.egg-info/top_level.txt
--rw-r--r--   0 freedmand   (501) staff       (20)       38 2023-04-09 15:53:27.448440 semantra-0.0.1/setup.cfg
--rw-r--r--   0 freedmand   (501) staff       (20)      347 2023-04-09 15:52:08.000000 semantra-0.0.1/setup.py
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 04:17:17.223431 semantra-0.0.2/
+-rw-r--r--   0 freedmand   (501) staff       (20)     1071 2023-03-31 03:28:18.000000 semantra-0.0.2/LICENSE
+-rw-r--r--   0 freedmand   (501) staff       (20)       32 2023-04-23 04:14:55.000000 semantra-0.0.2/MANIFEST.in
+-rw-r--r--   0 freedmand   (501) staff       (20)     3488 2023-04-23 04:17:17.223287 semantra-0.0.2/PKG-INFO
+-rw-r--r--   0 freedmand   (501) staff       (20)     3102 2023-04-16 16:45:22.000000 semantra-0.0.2/README.md
+-rw-r--r--   0 freedmand   (501) staff       (20)        5 2023-04-23 04:16:46.000000 semantra-0.0.2/VERSION
+-rw-r--r--   0 freedmand   (501) staff       (20)      156 2023-04-23 03:03:00.000000 semantra-0.0.2/requirements.txt
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 04:17:17.223100 semantra-0.0.2/semantra.egg-info/
+-rw-r--r--   0 freedmand   (501) staff       (20)     3488 2023-04-23 04:17:17.000000 semantra-0.0.2/semantra.egg-info/PKG-INFO
+-rw-r--r--   0 freedmand   (501) staff       (20)      269 2023-04-23 04:17:17.000000 semantra-0.0.2/semantra.egg-info/SOURCES.txt
+-rw-r--r--   0 freedmand   (501) staff       (20)        1 2023-04-23 04:17:17.000000 semantra-0.0.2/semantra.egg-info/dependency_links.txt
+-rw-r--r--   0 freedmand   (501) staff       (20)       43 2023-04-23 04:17:17.000000 semantra-0.0.2/semantra.egg-info/entry_points.txt
+-rw-r--r--   0 freedmand   (501) staff       (20)      156 2023-04-23 04:17:17.000000 semantra-0.0.2/semantra.egg-info/requires.txt
+-rw-r--r--   0 freedmand   (501) staff       (20)        9 2023-04-23 04:17:17.000000 semantra-0.0.2/semantra.egg-info/top_level.txt
+-rw-r--r--   0 freedmand   (501) staff       (20)    28707 2023-04-23 04:15:34.000000 semantra-0.0.2/semantra.py
+-rw-r--r--   0 freedmand   (501) staff       (20)       38 2023-04-23 04:17:17.223478 semantra-0.0.2/setup.cfg
+-rw-r--r--   0 freedmand   (501) staff       (20)     1150 2023-04-23 04:15:11.000000 semantra-0.0.2/setup.py
```

### Comparing `semantra-0.0.1/LICENSE` & `semantra-0.0.2/LICENSE`

 * *Files identical despite different names*

