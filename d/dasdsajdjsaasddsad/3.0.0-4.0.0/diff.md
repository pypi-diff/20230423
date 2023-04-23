# Comparing `tmp/dasdsajdjsaasddsad-3.0.0.tar.gz` & `tmp/dasdsajdjsaasddsad-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dasdsajdjsaasddsad-3.0.0.tar", last modified: Sun Apr 23 20:58:17 2023, max compression
+gzip compressed data, was "dasdsajdjsaasddsad-4.0.0.tar", last modified: Sun Apr 23 20:59:42 2023, max compression
```

## Comparing `dasdsajdjsaasddsad-3.0.0.tar` & `dasdsajdjsaasddsad-4.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 20:58:17.886539 dasdsajdjsaasddsad-3.0.0/
--rw-rw-rw-   0        0        0      260 2023-04-23 20:58:17.886539 dasdsajdjsaasddsad-3.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       16 2023-04-04 20:52:05.000000 dasdsajdjsaasddsad-3.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 20:58:17.868534 dasdsajdjsaasddsad-3.0.0/dasdsajdjsaasddsad/
--rw-rw-rw-   0        0        0   296896 2023-04-23 18:56:28.000000 dasdsajdjsaasddsad-3.0.0/dasdsajdjsaasddsad/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 20:58:17.885538 dasdsajdjsaasddsad-3.0.0/dasdsajdjsaasddsad.egg-info/
--rw-rw-rw-   0        0        0      260 2023-04-23 20:58:17.000000 dasdsajdjsaasddsad-3.0.0/dasdsajdjsaasddsad.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2023-04-23 20:58:17.000000 dasdsajdjsaasddsad-3.0.0/dasdsajdjsaasddsad.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 20:58:17.000000 dasdsajdjsaasddsad-3.0.0/dasdsajdjsaasddsad.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-04-23 20:58:17.000000 dasdsajdjsaasddsad-3.0.0/dasdsajdjsaasddsad.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-23 20:58:17.000000 dasdsajdjsaasddsad-3.0.0/dasdsajdjsaasddsad.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      415 2023-04-23 20:58:17.887538 dasdsajdjsaasddsad-3.0.0/setup.cfg
--rw-rw-rw-   0        0        0      354 2023-04-23 20:58:05.000000 dasdsajdjsaasddsad-3.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 20:59:42.326170 dasdsajdjsaasddsad-4.0.0/
+-rw-rw-rw-   0        0        0      260 2023-04-23 20:59:42.326170 dasdsajdjsaasddsad-4.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0       16 2023-04-04 20:52:05.000000 dasdsajdjsaasddsad-4.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 20:59:42.308166 dasdsajdjsaasddsad-4.0.0/dasdsajdjsaasddsad/
+-rw-rw-rw-   0        0        0   296896 2023-04-23 18:56:28.000000 dasdsajdjsaasddsad-4.0.0/dasdsajdjsaasddsad/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 20:59:42.325170 dasdsajdjsaasddsad-4.0.0/dasdsajdjsaasddsad.egg-info/
+-rw-rw-rw-   0        0        0      260 2023-04-23 20:59:42.000000 dasdsajdjsaasddsad-4.0.0/dasdsajdjsaasddsad.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2023-04-23 20:59:42.000000 dasdsajdjsaasddsad-4.0.0/dasdsajdjsaasddsad.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 20:59:42.000000 dasdsajdjsaasddsad-4.0.0/dasdsajdjsaasddsad.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-04-23 20:59:42.000000 dasdsajdjsaasddsad-4.0.0/dasdsajdjsaasddsad.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-23 20:59:42.000000 dasdsajdjsaasddsad-4.0.0/dasdsajdjsaasddsad.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      415 2023-04-23 20:59:42.328171 dasdsajdjsaasddsad-4.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      354 2023-04-23 20:59:38.000000 dasdsajdjsaasddsad-4.0.0/setup.py
```

### Comparing `dasdsajdjsaasddsad-3.0.0/dasdsajdjsaasddsad/__init__.py` & `dasdsajdjsaasddsad-4.0.0/dasdsajdjsaasddsad/__init__.py`

 * *Files identical despite different names*

