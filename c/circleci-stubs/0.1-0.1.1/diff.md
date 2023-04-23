# Comparing `tmp/circleci-stubs-0.1.tar.gz` & `tmp/circleci-stubs-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circleci-stubs-0.1.tar", last modified: Sun Apr 23 18:01:16 2023, max compression
+gzip compressed data, was "circleci-stubs-0.1.1.tar", last modified: Sun Apr 23 18:53:03 2023, max compression
```

## Comparing `circleci-stubs-0.1.tar` & `circleci-stubs-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 johnclyde   (501) staff       (20)        0 2023-04-23 18:01:16.721094 circleci-stubs-0.1/
--rw-r--r--   0 johnclyde   (501) staff       (20)     1067 2023-04-23 15:43:18.000000 circleci-stubs-0.1/LICENSE
--rw-r--r--   0 johnclyde   (501) staff       (20)      111 2023-04-23 18:01:16.720963 circleci-stubs-0.1/PKG-INFO
--rw-r--r--   0 johnclyde   (501) staff       (20)     1341 2023-04-23 15:43:51.000000 circleci-stubs-0.1/README.md
-drwxr-xr-x   0 johnclyde   (501) staff       (20)        0 2023-04-23 18:01:16.720779 circleci-stubs-0.1/circleci_stubs.egg-info/
--rw-r--r--   0 johnclyde   (501) staff       (20)      111 2023-04-23 18:01:16.000000 circleci-stubs-0.1/circleci_stubs.egg-info/PKG-INFO
--rw-r--r--   0 johnclyde   (501) staff       (20)      215 2023-04-23 18:01:16.000000 circleci-stubs-0.1/circleci_stubs.egg-info/SOURCES.txt
--rw-r--r--   0 johnclyde   (501) staff       (20)        1 2023-04-23 18:01:16.000000 circleci-stubs-0.1/circleci_stubs.egg-info/dependency_links.txt
--rw-r--r--   0 johnclyde   (501) staff       (20)       16 2023-04-23 18:01:16.000000 circleci-stubs-0.1/circleci_stubs.egg-info/requires.txt
--rw-r--r--   0 johnclyde   (501) staff       (20)        1 2023-04-23 18:01:16.000000 circleci-stubs-0.1/circleci_stubs.egg-info/top_level.txt
--rw-r--r--   0 johnclyde   (501) staff       (20)       38 2023-04-23 18:01:16.721130 circleci-stubs-0.1/setup.cfg
--rw-r--r--   0 johnclyde   (501) staff       (20)      268 2023-04-23 17:59:28.000000 circleci-stubs-0.1/setup.py
+drwxr-xr-x   0 johnclyde   (501) staff       (20)        0 2023-04-23 18:53:03.568145 circleci-stubs-0.1.1/
+-rw-r--r--   0 johnclyde   (501) staff       (20)     1067 2023-04-23 15:43:18.000000 circleci-stubs-0.1.1/LICENSE
+-rw-r--r--   0 johnclyde   (501) staff       (20)      113 2023-04-23 18:53:03.567988 circleci-stubs-0.1.1/PKG-INFO
+-rw-r--r--   0 johnclyde   (501) staff       (20)     1341 2023-04-23 15:43:51.000000 circleci-stubs-0.1.1/README.md
+drwxr-xr-x   0 johnclyde   (501) staff       (20)        0 2023-04-23 18:53:03.567765 circleci-stubs-0.1.1/circleci_stubs.egg-info/
+-rw-r--r--   0 johnclyde   (501) staff       (20)      113 2023-04-23 18:53:03.000000 circleci-stubs-0.1.1/circleci_stubs.egg-info/PKG-INFO
+-rw-r--r--   0 johnclyde   (501) staff       (20)      215 2023-04-23 18:53:03.000000 circleci-stubs-0.1.1/circleci_stubs.egg-info/SOURCES.txt
+-rw-r--r--   0 johnclyde   (501) staff       (20)        1 2023-04-23 18:53:03.000000 circleci-stubs-0.1.1/circleci_stubs.egg-info/dependency_links.txt
+-rw-r--r--   0 johnclyde   (501) staff       (20)       16 2023-04-23 18:53:03.000000 circleci-stubs-0.1.1/circleci_stubs.egg-info/requires.txt
+-rw-r--r--   0 johnclyde   (501) staff       (20)        1 2023-04-23 18:53:03.000000 circleci-stubs-0.1.1/circleci_stubs.egg-info/top_level.txt
+-rw-r--r--   0 johnclyde   (501) staff       (20)       38 2023-04-23 18:53:03.568189 circleci-stubs-0.1.1/setup.cfg
+-rw-r--r--   0 johnclyde   (501) staff       (20)      511 2023-04-23 18:52:42.000000 circleci-stubs-0.1.1/setup.py
```

### Comparing `circleci-stubs-0.1/LICENSE` & `circleci-stubs-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `circleci-stubs-0.1/README.md` & `circleci-stubs-0.1.1/README.md`

 * *Files identical despite different names*

