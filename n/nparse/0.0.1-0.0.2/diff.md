# Comparing `tmp/nparse-0.0.1.tar.gz` & `tmp/nparse-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nparse-0.0.1.tar", last modified: Sat Apr 22 07:57:21 2023, max compression
+gzip compressed data, was "nparse-0.0.2.tar", last modified: Sat Apr 22 08:16:17 2023, max compression
```

## Comparing `nparse-0.0.1.tar` & `nparse-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 mknzm      (501) staff       (20)        0 2023-04-22 07:57:21.709229 nparse-0.0.1/
--rw-r--r--   0 mknzm      (501) staff       (20)      213 2023-04-22 07:57:21.705569 nparse-0.0.1/PKG-INFO
-drwxr-xr-x   0 mknzm      (501) staff       (20)        0 2023-04-22 07:57:21.704408 nparse-0.0.1/nparse.egg-info/
--rw-r--r--   0 mknzm      (501) staff       (20)      213 2023-04-22 07:57:21.000000 nparse-0.0.1/nparse.egg-info/PKG-INFO
--rw-r--r--   0 mknzm      (501) staff       (20)      190 2023-04-22 07:57:21.000000 nparse-0.0.1/nparse.egg-info/SOURCES.txt
--rw-r--r--   0 mknzm      (501) staff       (20)        1 2023-04-22 07:57:21.000000 nparse-0.0.1/nparse.egg-info/dependency_links.txt
--rw-r--r--   0 mknzm      (501) staff       (20)       44 2023-04-22 07:57:21.000000 nparse-0.0.1/nparse.egg-info/entry_points.txt
--rw-r--r--   0 mknzm      (501) staff       (20)        9 2023-04-22 07:57:21.000000 nparse-0.0.1/nparse.egg-info/requires.txt
--rw-r--r--   0 mknzm      (501) staff       (20)        1 2023-04-22 07:57:21.000000 nparse-0.0.1/nparse.egg-info/top_level.txt
--rw-r--r--   0 mknzm      (501) staff       (20)       38 2023-04-22 07:57:21.710035 nparse-0.0.1/setup.cfg
--rw-r--r--   0 mknzm      (501) staff       (20)      455 2023-04-22 07:44:08.000000 nparse-0.0.1/setup.py
+drwxr-xr-x   0 mknzm      (501) staff       (20)        0 2023-04-22 08:16:17.096728 nparse-0.0.2/
+-rw-r--r--   0 mknzm      (501) staff       (20)     1099 2023-04-22 08:16:17.096190 nparse-0.0.2/PKG-INFO
+drwxr-xr-x   0 mknzm      (501) staff       (20)        0 2023-04-22 08:16:17.091571 nparse-0.0.2/nparse.egg-info/
+-rw-r--r--   0 mknzm      (501) staff       (20)     1099 2023-04-22 08:16:16.000000 nparse-0.0.2/nparse.egg-info/PKG-INFO
+-rw-r--r--   0 mknzm      (501) staff       (20)      190 2023-04-22 08:16:16.000000 nparse-0.0.2/nparse.egg-info/SOURCES.txt
+-rw-r--r--   0 mknzm      (501) staff       (20)        1 2023-04-22 08:16:16.000000 nparse-0.0.2/nparse.egg-info/dependency_links.txt
+-rw-r--r--   0 mknzm      (501) staff       (20)       44 2023-04-22 08:16:16.000000 nparse-0.0.2/nparse.egg-info/entry_points.txt
+-rw-r--r--   0 mknzm      (501) staff       (20)        9 2023-04-22 08:16:16.000000 nparse-0.0.2/nparse.egg-info/requires.txt
+-rw-r--r--   0 mknzm      (501) staff       (20)        1 2023-04-22 08:16:16.000000 nparse-0.0.2/nparse.egg-info/top_level.txt
+-rw-r--r--   0 mknzm      (501) staff       (20)       38 2023-04-22 08:16:17.096867 nparse-0.0.2/setup.cfg
+-rw-r--r--   0 mknzm      (501) staff       (20)      622 2023-04-22 08:15:58.000000 nparse-0.0.2/setup.py
```

