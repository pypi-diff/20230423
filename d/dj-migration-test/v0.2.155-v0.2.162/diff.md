# Comparing `tmp/dj-migration-test-v0.2.155.tar.gz` & `tmp/dj-migration-test-v0.2.162.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dj-migration-test-v0.2.155.tar", last modified: Tue Sep 17 09:31:00 2019, max compression
+gzip compressed data, was "dist/dj-migration-test-v0.2.162.tar", last modified: Tue Sep 17 09:33:04 2019, max compression
```

## Comparing `dj-migration-test-v0.2.155.tar` & `dj-migration-test-v0.2.162.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-09-17 09:31:00.000000 dj-migration-test-v0.2.155/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1413 2019-09-17 09:31:00.000000 dj-migration-test-v0.2.155/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      468 2019-09-17 09:30:58.000000 dj-migration-test-v0.2.155/README
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-09-17 09:31:00.000000 dj-migration-test-v0.2.155/dj_migration_test/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      114 2019-09-17 09:30:58.000000 dj-migration-test-v0.2.155/dj_migration_test/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       97 2019-09-17 09:30:58.000000 dj-migration-test-v0.2.155/dj_migration_test/exceptions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2794 2019-09-17 09:30:58.000000 dj-migration-test-v0.2.155/dj_migration_test/test_clients.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       37 2019-09-17 09:30:58.000000 dj-migration-test-v0.2.155/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1181 2019-09-17 09:30:58.000000 dj-migration-test-v0.2.155/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-09-17 09:33:04.000000 dj-migration-test-v0.2.162/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1413 2019-09-17 09:33:04.000000 dj-migration-test-v0.2.162/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      468 2019-09-17 09:33:03.000000 dj-migration-test-v0.2.162/README
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-09-17 09:33:04.000000 dj-migration-test-v0.2.162/dj_migration_test/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      114 2019-09-17 09:33:03.000000 dj-migration-test-v0.2.162/dj_migration_test/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       97 2019-09-17 09:33:03.000000 dj-migration-test-v0.2.162/dj_migration_test/exceptions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2794 2019-09-17 09:33:03.000000 dj-migration-test-v0.2.162/dj_migration_test/test_clients.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       37 2019-09-17 09:33:03.000000 dj-migration-test-v0.2.162/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1181 2019-09-17 09:33:03.000000 dj-migration-test-v0.2.162/setup.py
```

### Comparing `dj-migration-test-v0.2.155/PKG-INFO` & `dj-migration-test-v0.2.162/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dj-migration-test
-Version: v0.2.155
+Version: v0.2.162
 Summary: Django migration test module
 Home-page: https://github.com/philsupertramp/dj-migration-test
 Author: Philipp Zettl
 Author-email: philipp.zettl@godesteem.de
 License: MIT
 Download-URL: https://github.com/philsupertramp/dj-migration-test/archive/v0.1.tar.gz
 Description: ## dj-migration-test [![CircleCI](https://circleci.com/gh/philsupertramp/dj-migration-test/tree/master.svg?style=svg)](https://circleci.com/gh/philsupertramp/dj-migration-test/tree/master)
```

### Comparing `dj-migration-test-v0.2.155/dj_migration_test/test_clients.py` & `dj-migration-test-v0.2.162/dj_migration_test/test_clients.py`

 * *Files identical despite different names*

### Comparing `dj-migration-test-v0.2.155/setup.py` & `dj-migration-test-v0.2.162/setup.py`

 * *Files identical despite different names*

