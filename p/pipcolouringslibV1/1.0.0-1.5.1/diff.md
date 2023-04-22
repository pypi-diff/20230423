# Comparing `tmp/pipcolouringslibV1-1.0.0.tar.gz` & `tmp/pipcolouringslibV1-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipcolouringslibV1-1.0.0.tar", last modified: Fri Apr 21 16:58:13 2023, max compression
+gzip compressed data, was "pipcolouringslibV1-1.5.1.tar", last modified: Sat Apr 22 22:54:29 2023, max compression
```

## Comparing `pipcolouringslibV1-1.0.0.tar` & `pipcolouringslibV1-1.5.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:58:13.532674 pipcolouringslibV1-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      326 2023-04-21 16:58:13.532674 pipcolouringslibV1-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:58:13.532674 pipcolouringslibV1-1.0.0/pipcolouringslibV1/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-21 16:58:13.000000 pipcolouringslibV1-1.0.0/pipcolouringslibV1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:58:13.532674 pipcolouringslibV1-1.0.0/pipcolouringslibV1.egg-info/
--rw-r--r--   0 root         (0) root         (0)      326 2023-04-21 16:58:13.000000 pipcolouringslibV1-1.0.0/pipcolouringslibV1.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      207 2023-04-21 16:58:13.000000 pipcolouringslibV1-1.0.0/pipcolouringslibV1.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 16:58:13.000000 pipcolouringslibV1-1.0.0/pipcolouringslibV1.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-04-21 16:58:13.000000 pipcolouringslibV1-1.0.0/pipcolouringslibV1.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-21 16:58:13.532674 pipcolouringslibV1-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      539 2023-04-21 16:58:12.000000 pipcolouringslibV1-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 22:54:29.246111 pipcolouringslibV1-1.5.1/
+-rw-r--r--   0 root         (0) root         (0)      392 2023-04-22 22:54:29.246111 pipcolouringslibV1-1.5.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 22:54:29.246111 pipcolouringslibV1-1.5.1/pipcolouringslibV1/
+-rw-r--r--   0 root         (0) root         (0)    70957 2023-04-22 22:54:28.000000 pipcolouringslibV1-1.5.1/pipcolouringslibV1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 22:54:29.246111 pipcolouringslibV1-1.5.1/pipcolouringslibV1.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      392 2023-04-22 22:54:29.000000 pipcolouringslibV1-1.5.1/pipcolouringslibV1.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      207 2023-04-22 22:54:29.000000 pipcolouringslibV1-1.5.1/pipcolouringslibV1.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-22 22:54:29.000000 pipcolouringslibV1-1.5.1/pipcolouringslibV1.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-04-22 22:54:29.000000 pipcolouringslibV1-1.5.1/pipcolouringslibV1.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-22 22:54:29.246111 pipcolouringslibV1-1.5.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      605 2023-04-22 22:54:28.000000 pipcolouringslibV1-1.5.1/setup.py
```

