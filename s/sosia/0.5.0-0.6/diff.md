# Comparing `tmp/sosia-0.5.0.tar.gz` & `tmp/sosia-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sosia-0.5.0.tar", last modified: Thu Jan 20 15:23:08 2022, max compression
+gzip compressed data, was "sosia-0.6.tar", last modified: Sun Apr 23 18:24:25 2023, max compression
```

## Comparing `sosia-0.5.0.tar` & `sosia-0.6.tar`

### file list

```diff
@@ -1,89 +1,87 @@
-drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2022-01-20 15:23:08.318081 sosia-0.5.0/
--rw-r--r--   0 panther   (1000) panther   (1000)     2684 2020-01-10 15:47:30.000000 sosia-0.5.0/CONTRIBUTING.rst
--rw-r--r--   0 panther   (1000) panther   (1000)     1066 2020-01-10 15:47:30.000000 sosia-0.5.0/LICENSE
--rw-rw-r--   0 panther   (1000) panther   (1000)     4467 2022-01-20 15:23:08.318081 sosia-0.5.0/PKG-INFO
--rw-r--r--   0 panther   (1000) panther   (1000)     2839 2021-01-04 13:54:25.000000 sosia-0.5.0/README.rst
-drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2022-01-20 15:23:08.302080 sosia-0.5.0/docs/
--rw-r--r--   0 panther   (1000) panther   (1000)      580 2020-01-10 15:47:30.000000 sosia-0.5.0/docs/Makefile
--rw-r--r--   0 panther   (1000) panther   (1000)       33 2020-04-17 08:59:49.000000 sosia-0.5.0/docs/authors.rst
--rw-r--r--   0 panther   (1000) panther   (1000)       33 2020-04-17 08:59:49.000000 sosia-0.5.0/docs/changelog.rst
--rw-r--r--   0 panther   (1000) panther   (1000)     6112 2020-01-10 15:47:30.000000 sosia-0.5.0/docs/conf.py
--rw-r--r--   0 panther   (1000) panther   (1000)       33 2020-01-10 15:47:30.000000 sosia-0.5.0/docs/contributing.rst
--rw-r--r--   0 panther   (1000) panther   (1000)     1592 2020-04-30 13:44:25.000000 sosia-0.5.0/docs/functioning.rst
--rw-r--r--   0 panther   (1000) panther   (1000)     1956 2020-12-08 13:01:49.000000 sosia-0.5.0/docs/index.rst
--rw-r--r--   0 panther   (1000) panther   (1000)      787 2020-01-10 15:47:30.000000 sosia-0.5.0/docs/make.bat
-drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2022-01-20 15:23:08.302080 sosia-0.5.0/docs/reference/
--rw-r--r--   0 panther   (1000) panther   (1000)      117 2020-01-10 15:47:30.000000 sosia-0.5.0/docs/reference/sosia.Original.rst
--rw-r--r--   0 panther   (1000) panther   (1000)      149 2020-01-10 15:47:30.000000 sosia-0.5.0/docs/reference.rst
-drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2022-01-20 15:23:08.306080 sosia-0.5.0/docs/tutorial/
--rw-r--r--   0 panther   (1000) panther   (1000)      473 2020-11-18 19:42:01.000000 sosia-0.5.0/docs/tutorial/installation.rst
--rw-r--r--   0 panther   (1000) panther   (1000)     3215 2020-11-18 20:45:50.000000 sosia-0.5.0/docs/tutorial/refining.rst
--rw-r--r--   0 panther   (1000) panther   (1000)      783 2020-11-18 19:42:02.000000 sosia-0.5.0/docs/tutorial/setup.rst
--rw-r--r--   0 panther   (1000) panther   (1000)    17069 2022-01-20 12:47:12.000000 sosia-0.5.0/docs/tutorial/usage.rst
--rw-r--r--   0 panther   (1000) panther   (1000)      166 2020-11-18 18:17:54.000000 sosia-0.5.0/docs/tutorial.rst
-drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2022-01-20 15:23:08.306080 sosia-0.5.0/meta/
--rw-r--r--   0 panther   (1000) panther   (1000)      277 2020-04-17 08:59:49.000000 sosia-0.5.0/meta/AUTHORS.rst
--rw-r--r--   0 panther   (1000) panther   (1000)     5871 2022-01-20 15:18:06.000000 sosia-0.5.0/meta/CHANGES.rst
--rw-r--r--   0 panther   (1000) panther   (1000)       59 2022-01-20 11:37:56.000000 sosia-0.5.0/requirements.txt
--rw-r--r--   0 panther   (1000) panther   (1000)      888 2022-01-20 15:23:08.318081 sosia-0.5.0/setup.cfg
--rw-r--r--   0 panther   (1000) panther   (1000)       93 2020-01-10 15:47:30.000000 sosia-0.5.0/setup.py
-drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2022-01-20 15:23:08.306080 sosia-0.5.0/sosia/
--rw-r--r--   0 panther   (1000) panther   (1000)      405 2020-04-17 08:59:49.000000 sosia-0.5.0/sosia/README.md
--rw-r--r--   0 panther   (1000) panther   (1000)      493 2020-12-04 16:21:58.000000 sosia-0.5.0/sosia/__init__.py
-drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2022-01-20 15:23:08.310080 sosia-0.5.0/sosia/classes/
--rw-r--r--   0 panther   (1000) panther   (1000)       75 2020-04-17 08:59:49.000000 sosia-0.5.0/sosia/classes/__init__.py
--rw-rw-r--   0 panther   (1000) panther   (1000)    16075 2022-01-20 11:11:03.000000 sosia-0.5.0/sosia/classes/original.py
--rw-rw-r--   0 panther   (1000) panther   (1000)    12392 2022-01-17 08:15:39.000000 sosia-0.5.0/sosia/classes/scientist.py
-drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2022-01-20 15:23:08.310080 sosia-0.5.0/sosia/classes/tests/
--rw-r--r--   0 panther   (1000) panther   (1000)        0 2020-01-10 15:47:30.000000 sosia-0.5.0/sosia/classes/tests/__init__.py
--rw-r--r--   0 panther   (1000) panther   (1000)     5989 2022-01-20 11:30:33.000000 sosia-0.5.0/sosia/classes/tests/test_Original.py
--rw-r--r--   0 panther   (1000) panther   (1000)     8451 2022-01-17 08:16:03.000000 sosia-0.5.0/sosia/classes/tests/test_Scientist.py
-drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2022-01-20 15:23:08.310080 sosia-0.5.0/sosia/establishing/
--rw-r--r--   0 panther   (1000) panther   (1000)      173 2020-04-17 08:59:49.000000 sosia-0.5.0/sosia/establishing/__init__.py
--rw-r--r--   0 panther   (1000) panther   (1000)      867 2020-12-06 21:24:40.000000 sosia-0.5.0/sosia/establishing/config.py
--rw-r--r--   0 panther   (1000) panther   (1000)     1515 2020-11-09 14:05:27.000000 sosia-0.5.0/sosia/establishing/constants.py
--rw-r--r--   0 panther   (1000) panther   (1000)     1378 2020-08-24 21:43:30.000000 sosia-0.5.0/sosia/establishing/database.py
--rw-r--r--   0 panther   (1000) panther   (1000)      899 2020-10-18 21:34:00.000000 sosia-0.5.0/sosia/establishing/fields_sources.py
-drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2022-01-20 15:23:08.310080 sosia-0.5.0/sosia/establishing/tests/
--rw-r--r--   0 panther   (1000) panther   (1000)        0 2020-04-17 08:59:49.000000 sosia-0.5.0/sosia/establishing/tests/__init__.py
--rw-r--r--   0 panther   (1000) panther   (1000)      344 2020-04-19 18:34:21.000000 sosia-0.5.0/sosia/establishing/tests/test_database.py
--rw-r--r--   0 panther   (1000) panther   (1000)     1066 2020-10-18 21:26:18.000000 sosia-0.5.0/sosia/establishing/tests/test_fields_sources.py
-drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2022-01-20 15:23:08.314081 sosia-0.5.0/sosia/processing/
--rw-r--r--   0 panther   (1000) panther   (1000)      323 2022-01-20 14:08:57.000000 sosia-0.5.0/sosia/processing/__init__.py
-drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2022-01-20 15:23:08.314081 sosia-0.5.0/sosia/processing/caching/
--rw-r--r--   0 panther   (1000) panther   (1000)      144 2020-04-17 08:59:49.000000 sosia-0.5.0/sosia/processing/caching/__init__.py
--rw-r--r--   0 panther   (1000) panther   (1000)     3627 2022-01-17 12:51:42.000000 sosia-0.5.0/sosia/processing/caching/inserting.py
--rw-r--r--   0 panther   (1000) panther   (1000)     3633 2022-01-17 11:25:53.000000 sosia-0.5.0/sosia/processing/caching/retrieving.py
-drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2022-01-20 15:23:08.314081 sosia-0.5.0/sosia/processing/caching/tests/
--rw-r--r--   0 panther   (1000) panther   (1000)        0 2020-04-17 08:59:49.000000 sosia-0.5.0/sosia/processing/caching/tests/__init__.py
--rw-r--r--   0 panther   (1000) panther   (1000)     5838 2020-11-16 15:55:50.000000 sosia-0.5.0/sosia/processing/caching/tests/test_retrieving.py
--rw-r--r--   0 panther   (1000) panther   (1000)      947 2020-11-09 16:12:49.000000 sosia-0.5.0/sosia/processing/caching/utils.py
--rw-r--r--   0 panther   (1000) panther   (1000)      433 2020-10-12 09:57:30.000000 sosia-0.5.0/sosia/processing/constants.py
--rw-r--r--   0 panther   (1000) panther   (1000)     9294 2022-01-20 14:11:05.000000 sosia-0.5.0/sosia/processing/extracting.py
--rw-r--r--   0 panther   (1000) panther   (1000)     6675 2022-01-17 08:48:33.000000 sosia-0.5.0/sosia/processing/filtering.py
--rw-r--r--   0 panther   (1000) panther   (1000)    10530 2022-01-17 13:49:43.000000 sosia-0.5.0/sosia/processing/finding.py
--rw-r--r--   0 panther   (1000) panther   (1000)     3974 2022-01-17 11:18:32.000000 sosia-0.5.0/sosia/processing/getting.py
--rw-r--r--   0 panther   (1000) panther   (1000)     1112 2020-04-17 08:59:49.000000 sosia-0.5.0/sosia/processing/initializing.py
--rw-r--r--   0 panther   (1000) panther   (1000)     9033 2022-01-16 20:20:17.000000 sosia-0.5.0/sosia/processing/querying.py
-drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2022-01-20 15:23:08.318081 sosia-0.5.0/sosia/processing/tests/
--rw-r--r--   0 panther   (1000) panther   (1000)        0 2020-01-10 15:47:30.000000 sosia-0.5.0/sosia/processing/tests/__init__.py
--rw-r--r--   0 panther   (1000) panther   (1000)     2166 2022-01-20 14:06:46.000000 sosia-0.5.0/sosia/processing/tests/test_extracting.py
--rw-r--r--   0 panther   (1000) panther   (1000)     1610 2022-01-16 21:10:22.000000 sosia-0.5.0/sosia/processing/tests/test_filtering.py
--rw-r--r--   0 panther   (1000) panther   (1000)      952 2020-09-02 09:27:16.000000 sosia-0.5.0/sosia/processing/tests/test_getting.py
--rw-r--r--   0 panther   (1000) panther   (1000)      795 2022-01-16 21:13:54.000000 sosia-0.5.0/sosia/processing/tests/test_initializing.py
--rw-rw-r--   0 panther   (1000) panther   (1000)     5321 2022-01-16 11:48:07.000000 sosia-0.5.0/sosia/processing/tests/test_querying.py
--rw-r--r--   0 panther   (1000) panther   (1000)     1529 2022-01-20 14:10:41.000000 sosia-0.5.0/sosia/processing/tests/test_utils.py
--rw-r--r--   0 panther   (1000) panther   (1000)     4101 2022-01-20 14:08:46.000000 sosia-0.5.0/sosia/processing/utils.py
-drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2022-01-20 15:23:08.318081 sosia-0.5.0/sosia/utils/
--rw-r--r--   0 panther   (1000) panther   (1000)      106 2020-04-17 08:59:49.000000 sosia-0.5.0/sosia/utils/__init__.py
--rw-r--r--   0 panther   (1000) panther   (1000)      829 2020-04-17 08:59:49.000000 sosia-0.5.0/sosia/utils/decorators.py
--rw-r--r--   0 panther   (1000) panther   (1000)      126 2020-10-12 09:57:30.000000 sosia-0.5.0/sosia/utils/defaults.py
--rw-r--r--   0 panther   (1000) panther   (1000)      790 2020-04-17 08:59:49.000000 sosia-0.5.0/sosia/utils/helpers.py
-drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2022-01-20 15:23:08.306080 sosia-0.5.0/sosia.egg-info/
--rw-r--r--   0 panther   (1000) panther   (1000)     4467 2022-01-20 15:23:07.000000 sosia-0.5.0/sosia.egg-info/PKG-INFO
--rw-r--r--   0 panther   (1000) panther   (1000)     2000 2022-01-20 15:23:08.000000 sosia-0.5.0/sosia.egg-info/SOURCES.txt
--rw-r--r--   0 panther   (1000) panther   (1000)        1 2022-01-20 15:23:07.000000 sosia-0.5.0/sosia.egg-info/dependency_links.txt
--rw-r--r--   0 panther   (1000) panther   (1000)        1 2020-03-17 12:54:59.000000 sosia-0.5.0/sosia.egg-info/not-zip-safe
--rw-r--r--   0 panther   (1000) panther   (1000)       47 2020-12-08 13:04:33.000000 sosia-0.5.0/sosia.egg-info/pbr.json
--rw-r--r--   0 panther   (1000) panther   (1000)       59 2022-01-20 15:23:07.000000 sosia-0.5.0/sosia.egg-info/requires.txt
--rw-r--r--   0 panther   (1000) panther   (1000)        6 2022-01-20 15:23:07.000000 sosia-0.5.0/sosia.egg-info/top_level.txt
+drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-04-23 18:24:25.610866 sosia-0.6/
+-rw-r--r--   0 panther   (1000) panther   (1000)     1203 2020-01-10 15:47:30.000000 sosia-0.6/.gitignore
+-rw-r--r--   0 panther   (1000) panther   (1000)     2684 2020-01-10 15:47:30.000000 sosia-0.6/CONTRIBUTING.rst
+-rw-r--r--   0 panther   (1000) panther   (1000)     1066 2020-01-10 15:47:30.000000 sosia-0.6/LICENSE
+-rw-rw-r--   0 panther   (1000) panther   (1000)     4060 2023-04-23 18:24:25.610866 sosia-0.6/PKG-INFO
+-rw-r--r--   0 panther   (1000) panther   (1000)     2839 2021-01-04 13:54:25.000000 sosia-0.6/README.rst
+drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-04-23 18:24:25.590866 sosia-0.6/docs/
+-rw-rw-r--   0 panther   (1000) panther   (1000)      168 2023-04-22 18:31:07.000000 sosia-0.6/docs/.readthedocs.yaml
+-rw-r--r--   0 panther   (1000) panther   (1000)      580 2020-01-10 15:47:30.000000 sosia-0.6/docs/Makefile
+-rw-r--r--   0 panther   (1000) panther   (1000)       33 2020-04-17 08:59:49.000000 sosia-0.6/docs/authors.rst
+-rw-r--r--   0 panther   (1000) panther   (1000)       33 2020-04-17 08:59:49.000000 sosia-0.6/docs/changelog.rst
+-rw-rw-r--   0 panther   (1000) panther   (1000)     2778 2023-04-22 18:29:52.000000 sosia-0.6/docs/conf.py
+-rw-r--r--   0 panther   (1000) panther   (1000)       33 2020-01-10 15:47:30.000000 sosia-0.6/docs/contributing.rst
+-rw-r--r--   0 panther   (1000) panther   (1000)     1592 2020-04-30 13:44:25.000000 sosia-0.6/docs/functioning.rst
+-rw-r--r--   0 panther   (1000) panther   (1000)     1956 2020-12-08 13:01:49.000000 sosia-0.6/docs/index.rst
+-rw-r--r--   0 panther   (1000) panther   (1000)      787 2020-01-10 15:47:30.000000 sosia-0.6/docs/make.bat
+drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-04-23 18:24:25.590866 sosia-0.6/docs/reference/
+-rw-r--r--   0 panther   (1000) panther   (1000)      117 2020-01-10 15:47:30.000000 sosia-0.6/docs/reference/sosia.Original.rst
+-rw-r--r--   0 panther   (1000) panther   (1000)      149 2020-01-10 15:47:30.000000 sosia-0.6/docs/reference.rst
+-rw-rw-r--   0 panther   (1000) panther   (1000)       19 2023-04-23 15:41:30.000000 sosia-0.6/docs/requirements.txt
+drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-04-23 18:24:25.594866 sosia-0.6/docs/tutorial/
+-rw-r--r--   0 panther   (1000) panther   (1000)      473 2020-11-18 19:42:01.000000 sosia-0.6/docs/tutorial/installation.rst
+-rw-r--r--   0 panther   (1000) panther   (1000)     3215 2020-11-18 20:45:50.000000 sosia-0.6/docs/tutorial/refining.rst
+-rw-r--r--   0 panther   (1000) panther   (1000)     1193 2023-04-23 06:57:31.000000 sosia-0.6/docs/tutorial/setup.rst
+-rw-r--r--   0 panther   (1000) panther   (1000)    17013 2023-04-23 06:57:49.000000 sosia-0.6/docs/tutorial/usage.rst
+-rw-r--r--   0 panther   (1000) panther   (1000)      166 2020-11-18 18:17:54.000000 sosia-0.6/docs/tutorial.rst
+drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-04-23 18:24:25.594866 sosia-0.6/meta/
+-rw-r--r--   0 panther   (1000) panther   (1000)      277 2020-04-17 08:59:49.000000 sosia-0.6/meta/AUTHORS.rst
+-rw-r--r--   0 panther   (1000) panther   (1000)     6570 2023-04-23 18:23:34.000000 sosia-0.6/meta/CHANGES.rst
+-rw-rw-r--   0 panther   (1000) panther   (1000)     1586 2023-04-22 18:31:07.000000 sosia-0.6/pyproject.toml
+-rw-rw-r--   0 panther   (1000) panther   (1000)       38 2023-04-23 18:24:25.610866 sosia-0.6/setup.cfg
+drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-04-23 18:24:25.594866 sosia-0.6/sosia/
+-rw-r--r--   0 panther   (1000) panther   (1000)      441 2023-04-23 10:11:23.000000 sosia-0.6/sosia/README.md
+-rw-rw-r--   0 panther   (1000) panther   (1000)      486 2023-04-22 18:31:07.000000 sosia-0.6/sosia/__init__.py
+drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-04-23 18:24:25.598866 sosia-0.6/sosia/classes/
+-rw-r--r--   0 panther   (1000) panther   (1000)       75 2020-04-17 08:59:49.000000 sosia-0.6/sosia/classes/__init__.py
+-rw-rw-r--   0 panther   (1000) panther   (1000)    15957 2022-02-13 12:29:50.000000 sosia-0.6/sosia/classes/original.py
+-rw-rw-r--   0 panther   (1000) panther   (1000)    12918 2023-04-23 07:15:38.000000 sosia-0.6/sosia/classes/scientist.py
+drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-04-23 18:24:25.598866 sosia-0.6/sosia/classes/tests/
+-rw-r--r--   0 panther   (1000) panther   (1000)        0 2020-01-10 15:47:30.000000 sosia-0.6/sosia/classes/tests/__init__.py
+-rw-r--r--   0 panther   (1000) panther   (1000)     6171 2023-04-23 16:17:09.000000 sosia-0.6/sosia/classes/tests/test_Original.py
+-rw-rw-r--   0 panther   (1000) panther   (1000)     8824 2023-04-23 16:52:50.000000 sosia-0.6/sosia/classes/tests/test_Scientist.py
+drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-04-23 18:24:25.598866 sosia-0.6/sosia/establishing/
+-rw-r--r--   0 panther   (1000) panther   (1000)      133 2023-04-23 06:51:26.000000 sosia-0.6/sosia/establishing/__init__.py
+-rw-r--r--   0 panther   (1000) panther   (1000)     1528 2023-04-23 06:45:36.000000 sosia-0.6/sosia/establishing/constants.py
+-rw-r--r--   0 panther   (1000) panther   (1000)     1322 2023-04-23 07:10:09.000000 sosia-0.6/sosia/establishing/database.py
+-rw-r--r--   0 panther   (1000) panther   (1000)     1079 2023-04-23 06:42:09.000000 sosia-0.6/sosia/establishing/fields_sources.py
+drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-04-23 18:24:25.602866 sosia-0.6/sosia/establishing/tests/
+-rw-r--r--   0 panther   (1000) panther   (1000)        0 2020-04-17 08:59:49.000000 sosia-0.6/sosia/establishing/tests/__init__.py
+-rw-r--r--   0 panther   (1000) panther   (1000)      445 2023-04-23 16:17:04.000000 sosia-0.6/sosia/establishing/tests/test_database.py
+-rw-r--r--   0 panther   (1000) panther   (1000)      964 2023-04-23 16:17:19.000000 sosia-0.6/sosia/establishing/tests/test_fields_sources.py
+drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-04-23 18:24:25.602866 sosia-0.6/sosia/processing/
+-rw-r--r--   0 panther   (1000) panther   (1000)      323 2022-01-20 14:08:57.000000 sosia-0.6/sosia/processing/__init__.py
+drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-04-23 18:24:25.606866 sosia-0.6/sosia/processing/caching/
+-rw-r--r--   0 panther   (1000) panther   (1000)      144 2020-04-17 08:59:49.000000 sosia-0.6/sosia/processing/caching/__init__.py
+-rw-r--r--   0 panther   (1000) panther   (1000)     3627 2022-01-17 12:51:42.000000 sosia-0.6/sosia/processing/caching/inserting.py
+-rw-r--r--   0 panther   (1000) panther   (1000)     3633 2022-01-17 11:25:53.000000 sosia-0.6/sosia/processing/caching/retrieving.py
+drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-04-23 18:24:25.606866 sosia-0.6/sosia/processing/caching/tests/
+-rw-r--r--   0 panther   (1000) panther   (1000)        0 2020-04-17 08:59:49.000000 sosia-0.6/sosia/processing/caching/tests/__init__.py
+-rw-r--r--   0 panther   (1000) panther   (1000)     5864 2023-04-23 18:18:34.000000 sosia-0.6/sosia/processing/caching/tests/test_retrieving.py
+-rw-r--r--   0 panther   (1000) panther   (1000)      947 2020-11-09 16:12:49.000000 sosia-0.6/sosia/processing/caching/utils.py
+-rw-r--r--   0 panther   (1000) panther   (1000)      433 2020-10-12 09:57:30.000000 sosia-0.6/sosia/processing/constants.py
+-rw-rw-r--   0 panther   (1000) panther   (1000)     8805 2022-02-07 12:07:34.000000 sosia-0.6/sosia/processing/extracting.py
+-rw-r--r--   0 panther   (1000) panther   (1000)     6675 2022-01-17 08:48:33.000000 sosia-0.6/sosia/processing/filtering.py
+-rw-r--r--   0 panther   (1000) panther   (1000)    10575 2022-02-07 12:37:14.000000 sosia-0.6/sosia/processing/finding.py
+-rw-r--r--   0 panther   (1000) panther   (1000)     3992 2022-02-07 12:36:01.000000 sosia-0.6/sosia/processing/getting.py
+-rw-r--r--   0 panther   (1000) panther   (1000)     1112 2020-04-17 08:59:49.000000 sosia-0.6/sosia/processing/initializing.py
+-rw-rw-r--   0 panther   (1000) panther   (1000)     9033 2022-02-01 21:33:14.000000 sosia-0.6/sosia/processing/querying.py
+drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-04-23 18:24:25.610866 sosia-0.6/sosia/processing/tests/
+-rw-r--r--   0 panther   (1000) panther   (1000)        0 2020-01-10 15:47:30.000000 sosia-0.6/sosia/processing/tests/__init__.py
+-rw-rw-r--   0 panther   (1000) panther   (1000)     1983 2023-04-23 16:52:35.000000 sosia-0.6/sosia/processing/tests/test_extracting.py
+-rw-r--r--   0 panther   (1000) panther   (1000)     1730 2023-04-23 16:52:23.000000 sosia-0.6/sosia/processing/tests/test_filtering.py
+-rw-r--r--   0 panther   (1000) panther   (1000)      945 2023-04-23 16:52:19.000000 sosia-0.6/sosia/processing/tests/test_getting.py
+-rw-r--r--   0 panther   (1000) panther   (1000)      916 2023-04-23 16:52:42.000000 sosia-0.6/sosia/processing/tests/test_initializing.py
+-rw-rw-r--   0 panther   (1000) panther   (1000)     5129 2023-04-23 16:52:28.000000 sosia-0.6/sosia/processing/tests/test_querying.py
+-rw-r--r--   0 panther   (1000) panther   (1000)     1505 2023-04-23 16:52:08.000000 sosia-0.6/sosia/processing/tests/test_utils.py
+-rw-r--r--   0 panther   (1000) panther   (1000)     3976 2022-02-08 21:29:28.000000 sosia-0.6/sosia/processing/utils.py
+drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-04-23 18:24:25.610866 sosia-0.6/sosia/utils/
+-rw-r--r--   0 panther   (1000) panther   (1000)       71 2023-04-23 06:45:44.000000 sosia-0.6/sosia/utils/__init__.py
+-rw-r--r--   0 panther   (1000) panther   (1000)      829 2020-04-17 08:59:49.000000 sosia-0.6/sosia/utils/decorators.py
+-rw-r--r--   0 panther   (1000) panther   (1000)      790 2020-04-17 08:59:49.000000 sosia-0.6/sosia/utils/helpers.py
+drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-04-23 18:24:25.594866 sosia-0.6/sosia.egg-info/
+-rw-rw-r--   0 panther   (1000) panther   (1000)     4060 2023-04-23 18:24:25.000000 sosia-0.6/sosia.egg-info/PKG-INFO
+-rw-rw-r--   0 panther   (1000) panther   (1000)     1930 2023-04-23 18:24:25.000000 sosia-0.6/sosia.egg-info/SOURCES.txt
+-rw-rw-r--   0 panther   (1000) panther   (1000)        1 2023-04-23 18:24:25.000000 sosia-0.6/sosia.egg-info/dependency_links.txt
+-rw-rw-r--   0 panther   (1000) panther   (1000)       52 2023-04-23 18:24:25.000000 sosia-0.6/sosia.egg-info/requires.txt
+-rw-rw-r--   0 panther   (1000) panther   (1000)        6 2023-04-23 18:24:25.000000 sosia-0.6/sosia.egg-info/top_level.txt
```

### Comparing `sosia-0.5.0/CONTRIBUTING.rst` & `sosia-0.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `sosia-0.5.0/LICENSE` & `sosia-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sosia-0.5.0/PKG-INFO` & `sosia-0.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,112 +1,113 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: sosia
-Version: 0.5.0
+Version: 0.6
 Summary: Find control groups for academics in Scopus
-Home-page: UNKNOWN
-Author: Stefano H. Barruffaldi and Michael E. Rose
-Author-email: Michael.Ernst.Rose@gmail.com
-Maintainer: Michael E. Rose
-Maintainer-email: Michael.Ernst.Rose@gmail.com
+Author-email: "Michael E. Rose and Stefano H. Baruffaldi" <Michael.Ernst.Rose@gmail.com>
+Maintainer-email: "Michael E. Rose" <Michael.Ernst.Rose@gmail.com>
 License: MIT
-Description: sosia
-        =====
-        
-        Match authors automatically in Scopus on-line
-        
-        Documentation: https://sosia.readthedocs.io
-        
-        Development: https://github.com/sosia-dev/sosia
-        
-        .. image:: https://badge.fury.io/py/sosia.svg
-            :target: https://badge.fury.io/py/sosia
-        
-        .. image:: https://readthedocs.org/projects/sosia/badge/?version=latest
-            :target: https://readthedocs.org/projects/sosia/badge/?version=latest
-        
-        .. image:: https://img.shields.io/pypi/pyversions/sosia.svg
-            :target: https://img.shields.io/pypi/pyversions/sosia.svg
-        
-        .. image:: https://img.shields.io/pypi/l/sosia.svg
-            :target: https://img.shields.io/pypi/l/sosia.svg
-        
-        .. image:: https://api.codeclimate.com/v1/badges/3e10a47fefae831b973a/maintainability
-           :target: https://codeclimate.com/github/sosia-dev/sosia/maintainability
-        
-        Installation
-        ============
-        
-        Install stable version from PyPI:
-        
-        .. code:: bash
-        
-            pip install sosia
-        
-        or development version from GitHub repository:
-        
-        .. code:: bash
-        
-            pip install git+https://github.com/sosia-dev/sosia
-        
-        Functioning
-        ===========
-        
-        sosia performs a series of queries in the Scopus database using the `pybliometrics package 
-        <http://pybliometrics.readthedocs.io/>`_.  After configuring your local pybliometrics (providing access credentials and eventually setting cache directories), you can use sosia:
-        
-        .. inclusion-marker-start
-        .. code-block:: python
-        
-            >>> import sosia
-            >>> 
-            >>> sosia.create_fields_sources_list()  # Necessary only once
-            >>> sosia.make_database()  # Necessary only once
-            >>> 
-            >>> stefano = sosia.Original(55208373700, 2019)  # Scopus ID and year
-            >>> stefano.define_search_sources()  # Sources similiar to scientist
-            >>> stefano.define_search_group()  # Authors publishing in similar sources
-            >>> stefano.find_matches()  # Find matches satisfying all criteria
-            >>> print(stefano.matches)
-            >>> ['55022752500', '55810688700', '55824607400']
-            >>> stefano.inform_matches()  # Optional step to provide additional information
-            >>> print(stefano.matches[0])
-            Match(ID='55022752500', name='Van der Borgh, Michel', first_name='Michel',
-            surname='Van der Borgh', first_year=2012, num_coauthors=6, num_publications=5,
-            num_citations=33, num_coauthors_period=6, num_publications_period=5,
-            num_citations_period=33, subjects=['BUSI', 'COMP', 'SOCI'], country='Netherlands',
-            affiliation_id='60032882', affiliation='Eindhoven University of Technology,
-            Department of Industrial Engineering & Innovation Sciences', language='eng',
-            reference_sim=0.0, abstract_sim=0.1217)
-        
-        
-        .. inclusion-marker-end
-        
-        Change log
-        ==========
-        
-        Please see `CHANGES.rst <./meta/CHANGES.rst>`_.
-        
-        Contributing
-        ============
-        
-        Please see `CONTRIBUTING.rst <CONTRIBUTING.rst>`_.  For the list of contributors see
-        `AUTHORS.rst <./meta/AUTHORS.rst>`_.
-        
-        License
-        =======
-        
-        MIT License; see `LICENSE <LICENSE>`_.
-        
-        
-Keywords: sosia
-Platform: UNKNOWN
+Project-URL: Homepage, https://github.com/sosia-dev/sosia
+Project-URL: Bug Tracker, https://github.com/sosia-dev/sosia/issues
+Project-URL: Documentation (stable), https://sosia.readthedocs.io/en/stable/
+Project-URL: Documentation (latest), https://sosia.readthedocs.io/en/latest/
+Keywords: sosia,control groups,research
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+sosia
+=====
+
+Match authors automatically in Scopus on-line
+
+Documentation: https://sosia.readthedocs.io
+
+Development: https://github.com/sosia-dev/sosia
+
+.. image:: https://badge.fury.io/py/sosia.svg
+    :target: https://badge.fury.io/py/sosia
+
+.. image:: https://readthedocs.org/projects/sosia/badge/?version=latest
+    :target: https://readthedocs.org/projects/sosia/badge/?version=latest
+
+.. image:: https://img.shields.io/pypi/pyversions/sosia.svg
+    :target: https://img.shields.io/pypi/pyversions/sosia.svg
+
+.. image:: https://img.shields.io/pypi/l/sosia.svg
+    :target: https://img.shields.io/pypi/l/sosia.svg
+
+.. image:: https://api.codeclimate.com/v1/badges/3e10a47fefae831b973a/maintainability
+   :target: https://codeclimate.com/github/sosia-dev/sosia/maintainability
+
+Installation
+============
+
+Install stable version from PyPI:
+
+.. code:: bash
+
+    pip install sosia
+
+or development version from GitHub repository:
+
+.. code:: bash
+
+    pip install git+https://github.com/sosia-dev/sosia
+
+Functioning
+===========
+
+sosia performs a series of queries in the Scopus database using the `pybliometrics package 
+<http://pybliometrics.readthedocs.io/>`_.  After configuring your local pybliometrics (providing access credentials and eventually setting cache directories), you can use sosia:
+
+.. inclusion-marker-start
+.. code-block:: python
+
+    >>> import sosia
+    >>> 
+    >>> sosia.create_fields_sources_list()  # Necessary only once
+    >>> sosia.make_database()  # Necessary only once
+    >>> 
+    >>> stefano = sosia.Original(55208373700, 2019)  # Scopus ID and year
+    >>> stefano.define_search_sources()  # Sources similiar to scientist
+    >>> stefano.define_search_group()  # Authors publishing in similar sources
+    >>> stefano.find_matches()  # Find matches satisfying all criteria
+    >>> print(stefano.matches)
+    >>> ['55022752500', '55810688700', '55824607400']
+    >>> stefano.inform_matches()  # Optional step to provide additional information
+    >>> print(stefano.matches[0])
+    Match(ID='55022752500', name='Van der Borgh, Michel', first_name='Michel',
+    surname='Van der Borgh', first_year=2012, num_coauthors=6, num_publications=5,
+    num_citations=33, num_coauthors_period=6, num_publications_period=5,
+    num_citations_period=33, subjects=['BUSI', 'COMP', 'SOCI'], country='Netherlands',
+    affiliation_id='60032882', affiliation='Eindhoven University of Technology,
+    Department of Industrial Engineering & Innovation Sciences', language='eng',
+    reference_sim=0.0, abstract_sim=0.1217)
+
+
+.. inclusion-marker-end
+
+Change log
+==========
+
+Please see `CHANGES.rst <./meta/CHANGES.rst>`_.
+
+Contributing
+============
+
+Please see `CONTRIBUTING.rst <CONTRIBUTING.rst>`_.  For the list of contributors see
+`AUTHORS.rst <./meta/AUTHORS.rst>`_.
+
+License
+=======
+
+MIT License; see `LICENSE <LICENSE>`_.
```

### Comparing `sosia-0.5.0/README.rst` & `sosia-0.6/README.rst`

 * *Files identical despite different names*

### Comparing `sosia-0.5.0/docs/Makefile` & `sosia-0.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sosia-0.5.0/docs/functioning.rst` & `sosia-0.6/docs/functioning.rst`

 * *Files identical despite different names*

### Comparing `sosia-0.5.0/docs/index.rst` & `sosia-0.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `sosia-0.5.0/docs/make.bat` & `sosia-0.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sosia-0.5.0/docs/tutorial/refining.rst` & `sosia-0.6/docs/tutorial/refining.rst`

 * *Files identical despite different names*

### Comparing `sosia-0.5.0/docs/tutorial/usage.rst` & `sosia-0.6/docs/tutorial/usage.rst`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 --------------------------------
 
 The only class to interact with is :doc:`Original() <../reference/sosia.Original>`.  It represents the scientist for whom you'd like to find matches.  You initiate it with the Scopus Author ID and the year of treatment.
 
 .. code-block:: python
    
     >>> from sosia import Original
-    >>> stefano = Original(55208373700, 2017)
+    >>> stefano = Original(55208373700, 2017, sql_fname=DB_NAME)
 
 All properties and the control group are based on the publications associated with the profile and published before the treatment year.
 
 Upon initation, `pybliometrics` performs queries on the Scopus database under the hood.  The information is valid in the year of treatment and used to find similarities:
 
 .. code-block:: python
 
-    >>> stefano.country
+    >>> stefano.affiliation_country
     'Switzerland'
     >>> stefano.coauthors
     {57217825601, 54930777900, 36617057700, 54929867200, 55875219200,
      24464562500, 24781156100}
     >>> stefano.fields
     [2300, 3300, 2002, 1405, 1400, 1405, 1408, 1803, 2200, 2002, 1405, 1400,
      3300, 2300, 1405, 1803, 1408]
@@ -34,16 +34,16 @@
     >>> stefano.main_field
     (1405, 'BUSI')
 
 Additionally, `stefano.publications` is a list of namedtuples storing information about the indexed publications.  Each property can be manually overriden:
 
 .. code-block:: python
 
-    >>> stefano.country = 'Germany'
-    >>> stefano.country
+    >>> stefano.affiliation_country = 'Germany'
+    >>> stefano.affiliation_country
     'Germany'
     >>> stefano.main_field = (1406, 'ECON')
     >>> stefano.main_field
     (1406, 'ECON')
 
 
 Similarity parameters
@@ -53,26 +53,25 @@
 
 By default (i.e., if not specified), the margins for the first year of publication is 2, for the number of co-author, the number of publication, and for the number of citations it is 20%.  Margins work in either direction.  You can override these paramters.  `sosia` interprets integer values as absolute deviation, and float values as relative deviation:
 
 .. code-block:: python
    
     >>> stefano = Original(55208373700, 2017, first_year_margin=2,
                            coauth_margin=0.2, pub_margin=0.2,
-                           cits_margin=0.2)
+                           cits_margin=0.2, sql_fname=DB_NAME)
 
 This will find matches who started publishing the year of the scientist's first publication plus or minus 2 years, who in the year of treatment have the same number of coauthors plus or minus 20% of that number (at least 1), and who in the year of treatment have the same number of publications plus or minus 20% of that number (at least 1).
 
 
 Defining search sources
 -----------------------
 The first step is to define a list of sources similar (in type and area) to the sources the scientist published until the year of treatment.  `sosia` uses these source to define an intial search group.  A source is similar if (i) it is associated to the scientist's main field, (ii) is of the same type(s) of the scientist's sources and (iii) is not associated to fields alien to the scientist.  Here type of source refers to journal, conference proceeding, book, etc.  You define the list of search sources with a method to the class and access the results using a property:
 
 .. code-block:: python
 
-    >>> stefano = Original(55208373700, 2017, cits_margin=200)
     >>> stefano.define_search_sources()
     >>> stefano.search_sources
     [(14726, 'Technovation'), (15143, 'Regional Studies'),
     (16680, 'Engineering Science and Education Journal'),
     (17047, 'Chronicle of Higher Education'), (18769, 'Applied Economics Letters'),
     # 57 more sources omitted
     (21100889873, 'International Journal of Recent Technology and Engineering'),
@@ -109,15 +108,15 @@
     Progress: |██████████████████████████████████████████████████| 100.00% complete
     ... parsing Scopus information for 2012...
     Progress: |██████████████████████████████████████████████████| 100.00% complete
     ... parsing Scopus information for 2013...
     Progress: |██████████████████████████████████████████████████| 100.00% complete
     ... parsing Scopus information for 2014...
     Progress: |██████████████████████████████████████████████████| 100.00% complete
-    Found 846 authors for search_group
+    Found 863 authors for search_group
 
 
 You can inspect the search group using `stefano.search_group`, which you can also override, pre-define or edit.
 
 An alternative search process will try to minimize the number of queries.  The downside is that the resulting query, which pybliometrics caches under the hood, cannot be reused for other searches (of other scientists).  Activate this setting with `stacked=True`:
 
 .. code-block:: python
@@ -134,39 +133,39 @@
     Progress: |██████████████████████████████████████████████████| 100.00% complete
     ... parsing Scopus information for 2012...
     Progress: |██████████████████████████████████████████████████| 100.00% complete
     ... parsing Scopus information for 2013...
     Progress: |██████████████████████████████████████████████████| 100.00% complete
     ... parsing Scopus information for 2014...
     Progress: |██████████████████████████████████████████████████| 100.00% complete
-    Found 846 authors for search_group
+    Found 863 authors for search_group
 
 
 Finding matches
 ---------------
 
 The final step is to search within this search group for authors that fulfill criteria 5 through 6.  Matches are accessible through property `.matches`:
 
 .. code-block:: python
 
     >>> stefano.find_matches(verbose=True)
-    Searching through characteristics of 846 authors...
+    Searching through characteristics of 863 authors...
     Pre-filtering...
     Progress: |██████████████████████████████████████████████████| 100.00% complete
-    Left with 503 authors with sufficient number of publications and same main field
-    Obtaining information for 503 authors without sufficient information in database...
+    Left with 516 authors with sufficient number of publications and same main field
+    Obtaining information for 516 authors without sufficient information in database...
     Progress: |██████████████████████████████████████████████████| 100.00% complete
     Left with 97 authors based on publication information before 2009
     Counting publications of 97 authors before 2018...
     Progress: |██████████████████████████████████████████████████| 100.00% complete
-    Left with 35 researchers
-    Counting citations of 35 authors...
+    Left with 34 researchers
+    Counting citations of 34 authors...
     Progress: |██████████████████████████████████████████████████| 100.00% complete
     Filtering based on count of citations...
-    Left with 5 authors
+    Left with 6 authors
     Filtering based on coauthor count...
     Progress: |██████████████████████████████████████████████████| 100.00% complete
     Found 3 author(s) matching all criteria
     Find matches...
     Searching through characteristics of 846 authors...
     Left with 503 authors with sufficient number of publications and same main field
     Left with 35 researchers
@@ -182,41 +181,43 @@
 -----------------------------
 
 You might need additional information to both assess match quality and select matches.  Method `.inform_matches()` adds certain specified information to each match.  Attribute `stefano.matches` then becomes a list of `namedtuples <https://docs.python.org/3/library/collections.html#collections.namedtuple>`_:
 
 .. code-block:: python
 
     >>> stefano.inform_matches(verbose=True)
-    Providing additional information...
+    Providing information for 3 matches...
     Progress: |██████████████████████████████████████████████████| 100.00% complete
-    Match 55071051800: 0 reference list(s) out of 8 document(s) missing
-    Match 55317901900: 0 reference list(s) out of 7 document(s) missing
-    Match 55804519400: 0 reference list(s) out of 8 document(s) missing
+    Match 55022752500: 0 reference list(s) out of 5 documents missing
+    Match 55810688700: 0 reference list(s) out of 6 documents missing
+    Match 55824607400: 0 reference list(s) out of 7 documents missing
     Original 55208373700: 1 reference list(s) out of 7 documents missing
     >>> print(stefano.matches[0])
     Match(ID=55022752500, name='Van der Borgh, Michel', first_name='Michel',
     surname='Van der Borgh', first_year=2012, num_coauthors=6, num_publications=5,
-    num_citations=33, num_coauthors_period=6, num_publications_period=5, num_citations_period=33,
-    subjects=['BUSI', 'COMP', 'SOCI'], country='Netherlands', affiliation_id='60032882',
-    affiliation='Eindhoven University of Technology, Department of Industrial Engineering &
-    Innovation Sciences', language='eng', num_cited_refs=0)
+    num_citations=33, num_coauthors_period=6, num_publications_period=5,
+    num_citations_period=33, subjects=['BUSI', 'COMP', 'SOCI'],
+    affiliation_country='Netherlands', affiliation_id='60032882',
+    affiliation_name='Eindhoven University of Technology, Department of Industrial Engineering & Innovation Sciences',
+    affiliation_type="univ", language='eng', num_cited_refs=0)
 
 By default, `sosia` provides the following information:
 
 * `first_year`: The year of the first recorded publication
 * `num_coauthors`: The number of coauthors (Scopus Author profiles) up to the year of treatment
 * `num_publications`: The number of indexed publications up to the year of treatment
 * `num_citations`: The number of citations up until up to year of treatment
 * `num_coauthors_period`: The number of coauthors (Scopus Author profiles) within the `period` desired (if not provided, equal to num_coauthors)
 * `num_publications_period`: The number of indexed publications within the `period` desired (if not provided, equal to num_publications)
 * `num_citations_period`: The number of citations within the `period` desired  (if not provided, equal to num_citations)
-* `country`: The most frequent country of all affiliations listed on publications most recent to the year of treatment
 * `subjects`: List of research subjects in which the matched author has published up to the year of treatment
+* `affiliation_country`: The current country of the affiliation belonging to "affiliation_id"
 * `affiliation_id`: The most frequent Scopus Affiliation ID of all affiliations listed on publications most recent to the year of treatment
-* `affiliation`: The most frequent affiliation of all affiliations listed on publications most recent to the year of treatment
+* `affiliation_name`: The current name of the affiliation belonging to "affiliation_id"
+* `affiliation_type`: The current type of the affiliation belonging to "affiliation_id"
 * `language`: The language(s) of the published documents of an author up until the year of treatment
 * `num_cited_refs`: The number of jointly cited references as per publications up until the year of treatment (reference lists may be missing)
 
 Alternatively, you can provide a list of above keywords to only obtain information on these keywords.  This is helpful as some information takes time to gather.
 
 It is easy to work with namedtuples.  For example, using `pandas <https://pandas.pydata.org/>`_ you easily turn the list into a pandas DataFrame:
 
@@ -231,41 +232,35 @@
     ID                                                                          
     55022752500  Van der Borgh, Michel      Michel  Van der Borgh        2012   
     55810688700     Zapkau, Florian B.  Florian B.         Zapkau        2014   
     55824607400   Pellegrino, Gabriele    Gabriele     Pellegrino        2011   
 
                  num_coauthors  num_publications  num_citations  \
     ID                                                            
-    55022752500              6                 5             33   
-    55810688700              8                 6             32   
-    55824607400              5                 7             34   
-
-                 num_coauthors_period  num_publications_period  \
-    ID                                                           
-    55022752500                     6                        5   
-    55810688700                     8                        6   
-    55824607400                     5                        7   
-
-                 num_citations_period            subjects             country  \
-    ID                                                                          
-    55022752500                    33  [BUSI, COMP, SOCI]         Netherlands   
-    55810688700                    32        [BUSI, ECON]             Germany   
-    55824607400                    34  [BUSI, ECON, DECI]  Spain; Switzerland   
-
-                               affiliation_id  \
-    ID                                          
-    55022752500                      60032882   
-    55810688700                      60025310   
-    55824607400  60001576; 60028186; 60121786   
-
-                                                       affiliation language  \
-    ID                                                                        
-    55022752500  Eindhoven University of Technology, Department...      eng   
-    55810688700                           University of Düsseldorf      eng   
-    55824607400  Barcelona Institute of Economics, University o...      eng   
-
-                 num_cited_refs
-    ID                                        
-    55022752500         0
-    55810688700         0
-    55824607400         5
+    55022752500              6                 5             34   
+    55810688700              8                 6             33   
+    55824607400              5                 7             32   
+
+                num_coauthors_period num_publications_period num_citations_period  \
+    ID                                                                              
+    55022752500                 None                    None                 None   
+    55810688700                 None                    None                 None   
+    55824607400                 None                    None                 None   
+
+                           subjects affiliation_country affiliation_id  \
+    ID                                                                   
+    55022752500  [BUSI, ECON, COMP]         Netherlands       60032882   
+    55810688700        [BUSI, ECON]             Germany       60025310   
+    55824607400  [BUSI, ECON, DECI]         Switzerland       60028186   
+
+                                         affiliation_name affiliation_type  \
+    ID                                                                       
+    55022752500         Technische Universiteit Eindhoven             univ   
+    55810688700                Heinrich Heine Universitat             univ   
+    55824607400  Ecole Polytechnique Fédérale de Lausanne             univ   
+
+                language  num_cited_refs  
+    ID                                    
+    55022752500      eng               0  
+    55810688700      eng               0  
+    55824607400      eng               5
```

### Comparing `sosia-0.5.0/meta/CHANGES.rst` & `sosia-0.6/meta/CHANGES.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,27 @@
 Change Log
 ----------
 
 .. toctree::
 
+0.6
+~~~
+
+2023-04-23
+
+* Drop usage of configuration file and recommend project-specific databases.
+* In class `Scientist(), rename properties: `.country` -> `.affiliation_country`, `.affiliation` -> `.affiliation_name`.
+* In class `Scientist(), create property `.affiliation_type`.
+* In `.create_fields_sources_list()`, make use of parameter "verbose".
+* Make retrieval of affiliation related information robust to missing information (404 error).
+* Pass on "refresh" parameter from `inform_matches()`.
+* Use pyproject.toml for packaging, drop `pbr` (PEP 621).
+* Use XDG compliant file storage for support files in `~/.cache/sosia/`.
+* Improve various methods and functions for stability and speed.
+
 0.5
 ~~~
 
 2022-01-20
 
 * In `.inform_matches()`, remove abstract similarity and reference list similarity computation and corresponding keywords "abstract_sim" and "reference_sim"; do not require `nltk` and `scikit-learn` anymore.
 * In `.inform_matches()`, add "num_cited_refs" as number of jointly cited references up until provided year.
```

### Comparing `sosia-0.5.0/sosia/classes/original.py` & `sosia-0.6/sosia/classes/original.py`

 * *Files 4% similar despite different names*

```diff
@@ -186,15 +186,15 @@
     def define_search_group(self, stacked=False, verbose=False, refresh=False):
         """Define search_group.
 
         Parameters
         ----------
         stacked : bool (optional, default=False)
             Whether to combine searches in few queries or not.  Cached
-            files with most likely not be reusable.  Set to True if you
+            files will most likely not be reusable.  Set to True if you
             query in distinct fields or you want to minimize API key usage.
 
         verbose : bool (optional, default=False)
             Whether to report on the progress of the process.
 
         refresh : bool (optional, default=False)
             Whether to refresh cached results (if they exist) or not.
@@ -304,66 +304,63 @@
 
         # Find matches
         matches = find_matches(self, stacked, verbose, refresh)
         text = f"Found {len(matches):,} author(s) matching all criteria"
         custom_print(text, verbose)
         self._matches = sorted([auth_id for auth_id in matches])
 
-    def inform_matches(self, fields=None, verbose=False, refresh=False,
-                       **tfidf_kwds):
+    def inform_matches(self, fields=None, verbose=False, refresh=False):
         """Add information to matches to aid in selection process.
 
         Parameters
         ----------
         fields : iterable (optional, default=None)
-            Which information to provide. Allowed values are "first_year",
-            "num_coauthors", "num_publications", "num_citations", "country",
+            Which information to provide.  Allowed values are "first_name",
+            "surname", "first_year", "num_coauthors", "num_publications",
+            "num_citations", "num_coauthors_period", "num_publications_period",
+            "num_citations_period", "subjects", "affiliation_country",
+            "affiliation_id", "affiliation_name", "affiliation_type",
             "language", "num_cited_refs".  If None, will use all
             available fields.
 
         verbose : bool (optional, default=False)
             Whether to report on the progress of the process.
 
         refresh : bool (optional, default=False)
             Whether to refresh cached results (if they exist) or not. If int
             is passed and stacked=False, results will be refreshed if they are
             older than that value in number of days.
 
-        tfidf_kwds : keywords
-            Parameters to pass to TfidfVectorizer from the sklearn package
-            for reference vectorization.  Not used when `information=False` or
-            or when "num_cited_refs" is not in `information`.  See
-            https://scikit-learn.org/stable/modules/generated/sklearn.feature_extraction.text.TfidfVectorizer.html
-            for possible values.
-
         Notes
         -----
         Matches including corresponding information are available through
         property `.matches`.
 
         Raises
         ------
-        fields
-            If fields contains invalid keywords.
+        ValueError
+            If `fields` contains invalid keywords.
         """
         # Checks
         if not self._matches:
             text = "No matches defined.  Please run .find_matches() first."
             raise Exception(text)
         allowed_fields = ["first_name", "surname", "first_year",
                           "num_coauthors", "num_publications", "num_citations",
                           "num_coauthors_period", "num_publications_period",
-                          "num_citations_period", "subjects", "country",
-                          "affiliation_id", "affiliation", "language",
+                          "num_citations_period", "subjects",
+                          "affiliation_country", "affiliation_id",
+                          "affiliation_name", "affiliation_type", "language",
                           "num_cited_refs"]
         if fields:
             invalid = [x for x in fields if x not in allowed_fields]
             if invalid:
                 text = "Parameter fields contains invalid keywords: " +\
                        ", ".join(invalid)
                 raise ValueError(text)
         else:
             fields = allowed_fields
 
-        custom_print("Providing additional information...", verbose)
-        matches = inform_matches(self, fields, verbose, refresh, **tfidf_kwds)
+        text = f"Providing information for {len(self._matches):,} matches..."
+        custom_print(text, verbose)
+        matches = inform_matches(self, fields, verbose, refresh)
         self._matches = matches
```

### Comparing `sosia-0.5.0/sosia/classes/scientist.py` & `sosia-0.6/sosia/classes/scientist.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Author:   Michael E. Rose <michael.ernst.rose@gmail.com>
 """Super class to represent a scientist."""
 
 from warnings import warn
 
-from pybliometrics.scopus import AbstractRetrieval
+from pybliometrics.scopus import AbstractRetrieval, AffiliationRetrieval
+from pybliometrics.scopus.exception import Scopus404Error
 
-from sosia.establishing import config, connect_database
+from sosia.establishing import connect_database, DEFAULT_DATABASE
 from sosia.processing import add_source_names, base_query, count_citations,\
-    extract_authors, find_location, get_authors, get_main_field,\
+    extract_authors, find_main_affiliation, get_authors, get_main_field,\
     maybe_add_source_names, read_fields_sources_list
 from sosia.utils import accepts
 
 
 class Scientist(object):
     @property
     def active_year(self):
@@ -24,26 +25,56 @@
 
     @active_year.setter
     @accepts(int)
     def active_year(self, val):
         self._active_year = val
 
     @property
+    def affiliation_country(self):
+        """The current country of the affiliation defined in affiliation_id."""
+        return self._affiliation_country
+
+    @affiliation_country.setter
+    @accepts(str)
+    def affiliation_country(self, val):
+        self._affiliation_country = val
+
+    @property
     def affiliation_id(self):
         """The affiliation ID (as string) of the scientist's most frequent
         affiliation in or before the active year.
         """
         return self._affiliation_id
 
     @affiliation_id.setter
     @accepts(str)
     def affiliation_id(self, val):
         self._affiliation_id = val
 
     @property
+    def affiliation_name(self):
+        """The current name of the affiliation defined in affiliation_id."""
+        return self._affiliation_name
+
+    @affiliation_name.setter
+    @accepts(str)
+    def affiliation_name(self, val):
+        self._affiliation_name = val
+
+    @property
+    def affiliation_type(self):
+        """The current type of the affiliation defined in affiliation_id."""
+        return self._affiliation_type
+
+    @affiliation_type.setter
+    @accepts(str)
+    def affiliation_type(self, val):
+        self.affiliation_type = val
+
+    @property
     def citations(self):
         """The citations of the scientist until the provided year."""
         return self._citations
 
     @citations.setter
     @accepts(int)
     def citations(self, val):
@@ -56,25 +87,14 @@
 
     @citations_period.setter
     @accepts(int)
     def citations_period(self, val):
         self._citations_period = val
 
     @property
-    def country(self):
-        """Country belonging to the affiliation defined in affiliation_id.
-        """
-        return self._country
-
-    @country.setter
-    @accepts(str)
-    def country(self, val):
-        self._country = val
-
-    @property
     def coauthors(self):
         """Set of coauthors of the scientist on all publications until the
         provided year.
         """
         return self._coauthors
 
     @coauthors.setter
@@ -161,24 +181,14 @@
 
     @language.setter
     @accepts(str)
     def language(self, val):
         self._language = val
 
     @property
-    def organization(self):
-        """The name belonging to the affiliation defined in affiliation_id."""
-        return self._organization
-
-    @organization.setter
-    @accepts(str)
-    def organization(self, val):
-        self._organization = val
-
-    @property
     def publications(self):
         """List of the scientists' publications."""
         return self._publications
 
     @publications.setter
     @accepts((set, list, tuple))
     def publications(self, val):
@@ -252,28 +262,28 @@
             the Scopus Author ID(s).
 
         period: int (optional, default=None)
             In additional starting x years prior to the treatment year,
             which is also used to compute characteristics in the treatment
             year.
 
-        sql_fname : str (optional, default=None)
-            The path of the SQLite database to connect to.  If None, will use
-            the path specified in config.ini.
+        sql_fname : str (optional or pathlib.Path(), default=None)
+            The path of the SQLite database to connect to.  If None will
+            default to `~/.cache/sosia/main.sqlite`.
 
         Raises
         ------
         Exception
             When there are no publications for the author until the
             provided year.
         """
         self.identifier = identifier
         self.year = int(year)
         if not sql_fname:
-            sql_fname = config.get('Filepaths', 'Database')
+            sql_fname = DEFAULT_DATABASE
         self.sql_conn = connect_database(sql_fname)
 
         # Read mapping of fields to sources
         df, names = read_fields_sources_list()
         self.field_source = df
         self.source_names = names.set_index("source_id")["title"].to_dict()
 
@@ -335,19 +345,25 @@
         self._main_field = get_main_field(self._fields)
         if not self._main_field[0]:
             text = "Not possible to determine research field(s) of "\
                    "researcher.  Functionality is reduced."
             warn(text, UserWarning)
 
         # Most recent geolocation
-        ctry, afid, org = find_location(identifier, self._publications,
-                                        year, refresh=refresh)
-        self._country = ctry
+        afid = find_main_affiliation(identifier, self._publications, year)
         self._affiliation_id = afid
-        self._organization = org
+        try:
+            aff = AffiliationRetrieval(afid, refresh=refresh)
+            self._affiliation_country = aff.country
+            self._affiliation_name = aff.affiliation_name
+            self._affiliation_type = aff.org_type
+        except (Scopus404Error, ValueError):
+            self._affiliation_country = None
+            self._affiliation_name = None
+            self._affiliation_type = None
         self._language = None
 
         # Author name from profile with most documents
         df = get_authors(self.identifier, self.sql_conn,
                          refresh=refresh, verbose=False)
         au = df.sort_values("documents", ascending=False).iloc[0]
         self._subjects = [a.split(" ")[0] for a in au.areas.split("; ")]
@@ -356,20 +372,16 @@
         name = ", ".join([self._surname or "", au.givenname or ""])
         if name == ", ":
             name = None
         self._name = name
 
     def get_publication_languages(self, refresh=False):
         """Parse languages of published documents."""
-        from json import JSONDecodeError
-        from pybliometrics.scopus.exception import Scopus404Error
         langs = set()
         for eid in self._eids:
             try:
                 ab = AbstractRetrieval(eid, view="FULL", refresh=refresh)
-            except JSONDecodeError:
-                ab = AbstractRetrieval(eid, view="FULL", refresh=True)
             except Scopus404Error:
                 continue
             langs.add(ab.language)
         self._language = "; ".join(sorted(filter(None, langs)))
         return self
```

### Comparing `sosia-0.5.0/sosia/classes/tests/test_Original.py` & `sosia-0.6/sosia/classes/tests/test_Original.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-# -*- coding: utf-8 -*-
 """Tests for class `Original`."""
 
 import warnings
 from collections import namedtuple
-from os.path import expanduser
+from pathlib import Path
 
 import pandas as pd
 from nose.tools import assert_equal, assert_true
 
 from sosia.classes import Original
+from sosia.establishing import make_database
 
 warnings.filterwarnings("ignore")
 
-test_cache = expanduser("~/.sosia/test.sqlite")
+test_cache = Path.home()/".cache/sosia/test.sqlite"
+test_cache.unlink(missing_ok=True)
+make_database(test_cache)
 refresh = False
 test_params = {"refresh": refresh, "sql_fname": test_cache}
 
 # Test objects
 # Normal values
 scientist1 = Original(55208373700, 2017, cits_margin=200, first_year_margin=1,
                       pub_margin=0.1, coauth_margin=0.1, **test_params)
@@ -33,66 +35,66 @@
 scientist4 = Original(55208373700, 2017, cits_margin=1, pub_margin=1,
                       coauth_margin=1, first_year_margin=1, period=3,
                       first_year_search="name", affiliations=affs,
                       **test_params)
 
 # Expected matches
 fields = "ID name first_year num_coauthors num_publications num_citations "\
-         "country language num_cited_refs"
+         "affiliation_country language num_cited_refs"
 Match = namedtuple("Match", fields)
 MATCHES = [
     Match(
         ID=53164702100,
         name='Sapprasert, Koson',
         first_year=2011,
         num_coauthors=7,
         num_publications=6,
         num_citations=190,
-        country='Norway',
+        affiliation_country='Norway',
         language='eng',
         num_cited_refs=4),
     Match(
         ID=55071051800,
         name='Doldor, Elena',
         first_year=2013,
         num_coauthors=6,
         num_publications=8,
         num_citations=19,
-        country='United Kingdom',
+        affiliation_country='United Kingdom',
         language='eng',
         num_cited_refs=0),
     Match(
         ID=55317901900,
         name='Siepel, Josh',
         first_year=2013,
         num_coauthors=8,
         num_publications=7,
         num_citations=52,
-        country='United Kingdom',
+        affiliation_country='United Kingdom',
         language='eng',
         num_cited_refs=7),
     Match(
         ID=55804519400,
         name='González, Miguel Domingo',
         first_year=2013,
         num_coauthors=7,
         num_publications=8,
         num_citations=1,
-        country='Peru',
+        affiliation_country='Peru',
         language='eng; spa',
         num_cited_refs=0)]
 
 
 def test_search_sources():
     scientists_list = [scientist1, scientist2, scientist3, scientist4]
     for s in scientists_list:
         s.define_search_sources()
         search_sources = s.search_sources
         assert_equal(len(search_sources), 65)
-        assert_true((14726, "Technovation") in search_sources)
+        assert_true((20206, "Academy of Management Review") in search_sources)
         assert_true((15143, "Regional Studies") in search_sources)
 
 
 def test_search_sources_change():
     backup = scientist1.search_sources
     expected = [(14351, "Brain Research Reviews"),
                 (18632, "Progress in Brain Research")]
@@ -153,29 +155,30 @@
     scientist1.find_matches(stacked=True, refresh=refresh)
     expected = [m.ID for m in MATCHES]
     assert_equal(scientist1.matches, expected)
 
 
 def test_find_matches_stacked_affiliations():
     scientist3.find_matches(stacked=True, refresh=refresh)
-    expected = [m.ID for m in MATCHES if m.ID != 55804519400]
+    expected = [m.ID for m in MATCHES if m.ID != 53164702100]
     assert_equal(scientist3.matches, expected)
 
 
 def test_find_matches_stacked_period_affiliations():
     scientist4.find_matches(stacked=True, refresh=refresh)
-    expected_ids = [57188695848, 57188709931]
+    expected_ids = [56049973600, 57188695848, 57188709931]
     assert_equal(scientist4.matches, expected_ids)
 
 
 def test_inform_matches():
     scientist1.inform_matches(refresh=refresh)
     recieved = scientist1.matches
     assert_equal(len(recieved), len(MATCHES))
     assert_true(isinstance(recieved, list))
     cols = ["ID", "name", "first_year", "num_coauthors", "num_publications",
-            "country", "num_cited_refs"]
+            "affiliation_country", "num_cited_refs"]
     df_r = pd.DataFrame(recieved)
     df_r["num_cited_refs"] = df_r["num_cited_refs"].round(3)
     df_m = pd.DataFrame(MATCHES)
     df_m["num_cited_refs"] = df_m["num_cited_refs"].round(3)
     pd.testing.assert_frame_equal(df_r[cols], df_m[cols])
+
```

### Comparing `sosia-0.5.0/sosia/classes/tests/test_Scientist.py` & `sosia-0.6/sosia/classes/tests/test_Scientist.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,60 +1,70 @@
-# -*- coding: utf-8 -*-
 """Tests for class `Scientist`."""
 
 from collections import namedtuple
+from pathlib import Path
+
 from nose.tools import assert_equal, assert_true, assert_false
 
 from sosia.classes import Scientist
+from sosia.establishing import make_database
 
-refresh = 30
-scientist1 = Scientist([6701809842], 2001, refresh=refresh)
-scientist2 = Scientist([55208373700, 55208373700], 2017, refresh=refresh)
-eids = ["2-s2.0-84959420483", "2-s2.0-84949113230"]
-scientist3 = Scientist([55208373700], 2017, eids=eids, refresh=refresh)
-scientist4 = Scientist([55208373700], 2015, refresh=refresh)
-scientist5 = Scientist([55208373700], 2018, period=2, refresh=refresh)
-
-
-def test_affiliation():
-    org = 'Universität München'
-    assert_equal(scientist1.organization, org)
-    org = 'École Polytechnique Fédérale de Lausanne (EPFL)'
-    assert_equal(scientist2.organization, org)
-    org = 'Department of Economics and Management of Innovation, '\
-          'École Polytechnique Fédérale de Lausanne'
-    assert_equal(scientist3.organization, org)
-    org = 'École Polytechnique Fédérale de Lausanne, CEMI, CDM MTEI-GE'
-    assert_equal(scientist4.organization, org)
-    org = 'Max Planck Institute for Innovation and Competition'
-    assert_equal(scientist5.organization, org)
-
+test_cache = Path.home()/".cache/sosia/test.sqlite"
+refresh = False
+test_params = {"refresh": refresh, "sql_fname": test_cache}
 
-def test_affiliation_id():
-    assert_equal(scientist1.affiliation_id, '60028717')
-    assert_equal(scientist2.affiliation_id, '60028186')
-    assert_equal(scientist3.affiliation_id, '60028186')
-    assert_equal(scientist4.affiliation_id, '60028186')
-    assert_equal(scientist5.affiliation_id, '60105007')
+scientist1 = Scientist([6701809842], 2001, **test_params)
+scientist2 = Scientist([55208373700, 55208373700], 2017, **test_params)
+eids = ["2-s2.0-84959420483", "2-s2.0-84949113230"]
+scientist3 = Scientist([55208373700], 2017, eids=eids, **test_params)
+scientist4 = Scientist([55208373700], 2015, **test_params)
+scientist5 = Scientist([55208373700], 2018, period=2, **test_params)
 
 
 def test_active_year():
     assert_equal(scientist1.active_year, 2001)
     assert_equal(scientist2.active_year, 2017)
     assert_equal(scientist3.active_year, 2016)
     assert_equal(scientist4.active_year, 2012)
     assert_equal(scientist5.active_year, 2018)
 
 
-def test_country():
-    assert_equal(scientist1.country, "Germany")
-    assert_equal(scientist2.country, "Switzerland")
-    assert_equal(scientist3.country, "Switzerland")
-    assert_equal(scientist4.country, "Switzerland")
-    assert_equal(scientist5.country, "Germany")
+def test_affiliation_country():
+    assert_equal(scientist1.affiliation_country, "Germany")
+    assert_equal(scientist2.affiliation_country, "Switzerland")
+    assert_equal(scientist3.affiliation_country, "Switzerland")
+    assert_equal(scientist4.affiliation_country, "Switzerland")
+    assert_equal(scientist5.affiliation_country, "Germany")
+
+
+def test_affiliation_id():
+    assert_equal(scientist1.affiliation_id, '60028717')
+    assert_equal(scientist2.affiliation_id, '60028186')
+    assert_equal(scientist3.affiliation_id, '60028186')
+    assert_equal(scientist4.affiliation_id, '60028186')
+    assert_equal(scientist5.affiliation_id, '60105007')
+
+
+def test_affiliation_name():
+    assert_equal(scientist1.affiliation_name,
+                 'Ludwig-Maximilians-Universität München')
+    epfl = 'Ecole Polytechnique Fédérale de Lausanne'
+    assert_equal(scientist2.affiliation_name, epfl)
+    assert_equal(scientist3.affiliation_name, epfl)
+    assert_equal(scientist4.affiliation_name, epfl)
+    assert_equal(scientist5.affiliation_name,
+                 'Max Planck Institute for Innovation and Competition')
+
+
+def test_affiliation_type():
+    assert_equal(scientist1.affiliation_type, 'univ')
+    assert_equal(scientist2.affiliation_type, 'univ')
+    assert_equal(scientist3.affiliation_type, 'univ')
+    assert_equal(scientist4.affiliation_type, 'univ')
+    assert_equal(scientist5.affiliation_type, 'resi')
 
 
 def test_citations():
     assert_true(scientist1.citations >= 47)
     assert_true(scientist2.citations >= 28)
     assert_true(scientist3.citations >= 2)
     assert_true(scientist4.citations >= 19)
```

### Comparing `sosia-0.5.0/sosia/establishing/constants.py` & `sosia-0.6/sosia/establishing/constants.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-from os.path import expanduser
+from pathlib import Path
 
 DATA_REPO_URL = "https://raw.githubusercontent.com/sosia-dev/sosia-data/"
-FIELDS_SOURCES_LIST = expanduser("~/.sosia/") + "field_sources_list.csv"
-SOURCES_NAMES_LIST = expanduser("~/.sosia/") + "sources_names.csv"
-CONFIG_FILE = expanduser("~/.sosia/config.ini")
+_cache_folder = Path.home()/".cache/sosia/"
+FIELDS_SOURCES_LIST = _cache_folder/"field_sources_list.csv"
+SOURCES_NAMES_LIST = _cache_folder/"sources_names.csv"
+DEFAULT_DATABASE = _cache_folder/'main.sqlite'
 
 DB_TABLES = {
     "author_ncits":
         {"columns": (("auth_id", "int"), ("year", "int"), ("n_cits", "int")),
          "primary": ("auth_id", "year")},
     "author_pubs":
         {"columns": (("auth_id", "int"), ("year", "int"), ("n_pubs", "int")),
```

### Comparing `sosia-0.5.0/sosia/establishing/database.py` & `sosia-0.6/sosia/establishing/database.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,25 +17,25 @@
 
 def make_database(fname=None, drop=False):
     """Make SQLite database with predefined tables and keys.
 
     Parameters
     ----------
     fname : str (optional, default=None)
-        The path of the SQLite database to connect to.  If None will use
-        the path provided in `~/.sosia/config.ini`.
+        The path of the SQLite database to connect to.  If None will default
+        to `~/.cache/sosia/main.sqlite`.
 
     drop : boolean (optional, default=False)
         If True, deletes and recreates all tables in cache (irreversible).
     """
-    from sosia.establishing.constants import DB_TABLES
-    from sosia.establishing.config import config
+    from sosia.establishing.constants import DB_TABLES, DEFAULT_DATABASE
 
     if not fname:
-        fname = config.get('Filepaths', 'Database')
+        fname = DEFAULT_DATABASE
+
     conn = sqlite3.connect(fname)
     cursor = conn.cursor()
     for table, variables in DB_TABLES.items():
         if drop:
             cursor.execute(f"DROP TABLE IF EXISTS {table}")
         columns = ", ".join(" ".join(v) for v in variables["columns"])
         q = f"CREATE TABLE IF NOT EXISTS {table} "\
```

### Comparing `sosia-0.5.0/sosia/establishing/tests/test_fields_sources.py` & `sosia-0.6/sosia/establishing/tests/test_fields_sources.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,17 @@
-# -*- coding: utf-8 -*-
 """Tests for establishing.fields_sources module."""
 
-from os import remove
-
 import pandas as pd
 from nose.tools import assert_equal, assert_true
 
 from sosia.establishing.constants import FIELDS_SOURCES_LIST, SOURCES_NAMES_LIST
 from sosia.establishing.fields_sources import create_fields_sources_list
 
-try:
-    remove(FIELDS_SOURCES_LIST)
-except FileNotFoundError:
-    pass
-try:
-    remove(SOURCES_NAMES_LIST)
-except FileNotFoundError:
-    pass
+FIELDS_SOURCES_LIST.unlink(missing_ok=True)
+FIELDS_SOURCES_LIST.unlink(missing_ok=True)
 create_fields_sources_list()
 
 
 def test_fields_sources_list():
     df = pd.read_csv(FIELDS_SOURCES_LIST)
     assert_true(isinstance(df, pd.DataFrame))
     assert_equal(list(df.columns), ["asjc", "source_id", "type"])
```

### Comparing `sosia-0.5.0/sosia/processing/caching/inserting.py` & `sosia-0.6/sosia/processing/caching/inserting.py`

 * *Files identical despite different names*

### Comparing `sosia-0.5.0/sosia/processing/caching/retrieving.py` & `sosia-0.6/sosia/processing/caching/retrieving.py`

 * *Files identical despite different names*

### Comparing `sosia-0.5.0/sosia/processing/caching/tests/test_retrieving.py` & `sosia-0.6/sosia/processing/caching/tests/test_retrieving.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-# -*- coding: utf-8 -*-
 """Tests for processing.caching.retrieving module."""
 
 from itertools import product
-from nose.tools import assert_equal, assert_true
-import numpy as np
-from os.path import expanduser
+from pathlib import Path
 
+import numpy as np
 import pandas as pd
-from pybliometrics.scopus import ScopusSearch, AuthorSearch
+from nose.tools import assert_equal, assert_true
 from pandas.testing import assert_frame_equal
+from pybliometrics.scopus import ScopusSearch, AuthorSearch
 
 from sosia.establishing import connect_database, make_database
 from sosia.processing import build_dict, insert_data, retrieve_authors,\
     retrieve_author_info, retrieve_authors_from_sourceyear, robust_join,\
     query_pubs_by_sourceyear
 
-test_cache = expanduser("~/.sosia/test.sqlite")
+test_cache = Path.home()/".cache/sosia/test.sqlite"
 refresh = 30
 
 
 def test_retrieve_authors():
     make_database(test_cache, drop=True)
     conn = connect_database(test_cache)
     # Variables
@@ -42,21 +41,22 @@
     expected_auth = [53164702100, 57197093438]
     search_auth = [55317901900]
     expected_cols = ['auth_id', 'eid', 'surname', 'initials', 'givenname',
                      'affiliation', 'documents', 'affiliation_id', 'city',
                      'country', 'areas']
     # Insert data
     q = f"AU-ID({robust_join(expected_auth, sep=') OR AU-ID(')})"
-    res = pd.DataFrame(AuthorSearch(q, refresh=refresh).authors, dtype="int64")
-    res["auth_id"] = res["eid"].str.split("-").str[-1]
+    res = pd.DataFrame(AuthorSearch(q, refresh=refresh).authors)
+    res["auth_id"] = res["eid"].str.split("-").str[-1].astype("uint64")
+    res["affiliation_id"] = res["affiliation_id"].astype(float)
     res = res[expected_cols]
     insert_data(res, conn, table="authors")
     # Retrieve data
     df = pd.DataFrame(expected_auth + search_auth, columns=["auth_id"],
-                      dtype="int64")
+                      dtype="uint64")
     incache, missing = retrieve_authors(df, conn)
     assert_equal(incache.shape[0], 2)
     assert_equal(missing, [55317901900])
 
 
 def test_retrieve_author_info_authorpubs():
     make_database(test_cache, drop=True)
@@ -104,15 +104,15 @@
     df2 = pd.DataFrame(expected_auth + search_auth,
                        columns=["auth_id"], dtype="int64")
     df2["year"] = year
     # Insert data
     fill = robust_join(expected_auth, sep=') OR AU-ID(')
     q = f"(AU-ID({fill})) AND PUBYEAR BEF {year+1}"
     d = build_dict(ScopusSearch(q, refresh=refresh).results, expected_auth)
-    expected = pd.DataFrame.from_dict(d, orient="index", dtype="int64")
+    expected = pd.DataFrame.from_dict(d, orient="index")
     expected = expected.sort_index().rename_axis('auth_id').reset_index()
     expected["year"] = year
     expected = expected[['auth_id', 'year', 'first_year', 'n_pubs', 'n_coauth']]
     insert_data(expected, conn, table=table)
     # Retrieve data
     incache, missing = retrieve_author_info(df2, conn, table)
     assert_frame_equal(incache, expected)
```

### Comparing `sosia-0.5.0/sosia/processing/caching/utils.py` & `sosia-0.6/sosia/processing/caching/utils.py`

 * *Files identical despite different names*

### Comparing `sosia-0.5.0/sosia/processing/extracting.py` & `sosia-0.6/sosia/processing/extracting.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,64 +11,62 @@
     """Get list of author IDs from a list of namedtuples representing
     publications.
     """
     l = [x.author_ids.split(";") for x in pubs if isinstance(x.author_ids, str)]
     return [int(au) for sl in l for au in sl]
 
 
-def find_location(auth_ids, pubs, year, refresh):
-    """Find the most common country, affiliation ID, and affiliation name
-    of a scientist using her most recent publications with valid information.
+def find_main_affiliation(auth_ids, pubs, year):
+    """Find the most common affiliation ID of a scientist on publications
+    with valid information of the most recent year.
 
     Parameters
     ----------
     auth_ids : list of str
         A list of Scopus Author Profile IDs for which the affiliation should
         be searched for.
 
     pubs : list of namedtuple
         The publications associated with the Author IDs as returned from a
         scopus query.
 
     year : int
         The year for which we would like to have the country.
 
-    refresh : bool
-        Whether to refresh all cached files or not.
-
     Returns
     -------
-    country, affiliation_id, organization : str or None
-        The country, city, affiliation ID, and affiliation name of the
-        scientist in the year closest to the treatment year, given that the
-        publications list valid information for each output. Equals None when
-        no valid publications are found.
+    affiliation_id : str or None
+        The most common affiliation_id of the scientist in the year closest
+        to the treatment year, given that the publications list valid
+        information for each output.  Equals None when no valid
+        publications are found.
     """
-    from operator import attrgetter
-    # Available papers of most recent year with publications
-    papers = [p for p in pubs if int(p.coverDate[:4]) <= year]
-    papers = sorted(papers, key=attrgetter("coverDate"), reverse=True)
-    params = {"view": "FULL", "refresh": refresh}
-    # Return most recent complete information
-    for p in papers:
-        try:
-            authgroup = AbstractRetrieval(p.eid, **params).authorgroup or []
-        except Scopus404Error:
+    from collections import defaultdict, Counter
+    pubs = [p for p in pubs if p.author_ids and p.author_afids]
+    # Find affiliation ID of all available publications
+    affs = defaultdict(lambda: Counter())
+    for p in pubs:
+        cur_year = int(p.coverDate[:4])
+        if cur_year > year:
             continue
-        authgroup = [a for a in authgroup if a.auid in auth_ids
-                     and a.country and a.affiliation_id and a.organization]
-        countries = "; ".join(sorted(set([a.country for a in authgroup])))
-        aff_ids = [str(a.affiliation_id) for a in authgroup if a]
-        aff_ids = "; ".join(sorted(set(aff_ids)))
-        orgs = "; ".join(sorted(set([a.organization for a in authgroup])))
-        if not countries and not aff_ids and not orgs:
+        authors = [int(a) for a in p.author_ids.split(";")]
+        for focal in set(auth_ids).intersection(authors):
+            idx = authors.index(focal)
+        try:
+            aff_ids = p.author_afids.split(";")[idx].split("-")
+        except (IndexError, UnboundLocalError):
             continue
-        return countries, aff_ids, orgs
-    # Return None-triple if all else fails
-    return countries, aff_ids, orgs
+        affs[cur_year].update(Counter([a for a in aff_ids if a]))
+    # Use only most recent publications
+    try:
+        max_year = max(affs.keys())
+        main_aff = affs[max_year].most_common()[0][0]
+    except (IndexError, ValueError):
+        main_aff = None
+    return main_aff
 
 
 def get_main_field(fields):
     """Get main 4-digit ASJC field (code) and main 2-digit ASJC field (name).
 
     Parameters
     ----------
@@ -115,25 +113,28 @@
     c = Counter([str(f)[:2] for f in fields])
     main_2 = int(c.most_common(1)[0][0])
     name = ASJC_2D[main_2]
 
     return main_4, name
 
 
-def inform_match(profile, keywords):
+def inform_match(profile, keywords, refresh):
     """Create namedtuple adding information to matches.
 
     Parameters
     ----------
     profile : sosia.Scientist()
         A Scientist() object representing a match.
 
     keywords : iterable of strings
         Which information to add to the match.
 
+    refresh : bool
+        Whether to refresh all cached files or not.
+
     Returns
     -------
     match_info : dict
         Information corresponding to provided keywords.
     """
     from sosia.classes import Scientist
 
@@ -146,50 +147,44 @@
         "num_coauthors": len(profile.coauthors),
         "num_publications": len(profile.publications),
         "num_citations": profile.citations,
         "num_coauthors_period": len(profile.coauthors_period or "") or None,
         "num_publications_period": len(profile.publications_period or "") or None,
         "num_citations_period": profile.citations_period,
         "subjects": profile.subjects,
-        "country": profile.country,
+        "affiliation_country": profile.affiliation_country,
         "affiliation_id": profile.affiliation_id,
-        "affiliation": profile.organization
+        "affiliation_name": profile.affiliation_name,
+        "affiliation_type": profile.affiliation_type,
     }
     match_info = {k: v for k, v in info.items() if k in keywords + ["ID", "name"]}
     if "language" in keywords:
-        try:
-            match_info["language"] = profile.get_publication_languages().language
-        except Scopus404Error:  # Refresh profile
-            profile = Scientist(profile.identifier, profile.year, refresh=True)
-            match_info["language"] = profile.get_publication_languages().language
+        lang = profile.get_publication_languages(refresh=refresh).language
+        match_info["language"] = lang
     return match_info
 
 
-def inform_matches(self, keywords, verbose, refresh, **kwds):
+def inform_matches(self, keywords, verbose, refresh):
     """Add match-specific information to all matches.
 
     Parameters
     ----------
     self : sosia.Original()
-        Object whose matches should received additional information
+        Object whose matches should receive additional information.
 
     keywords : iterable of strings
         Which information to add to matches.
 
     verbose : bool
         Whether to report on the progress of the process and the completeness
         of document information.
 
     refresh : bool
         Whether to refresh all cached files or not.
 
-    kwds : keywords
-        Parameters to pass to sklearn.feature_extraction.text.TfidfVectorizer
-        for reference vectorization.
-
     Returns
     -------
     out : list of namedtuples
         A list of namedtuples representing matches.  Provided information
         depend on provided keywords.
     """
     from sosia.classes import Scientist
@@ -209,22 +204,22 @@
     completeness = {}
     total = len(self.matches)
     print_progress(0, total, verbose)
     for idx, auth_id in enumerate(self.matches):
         period = self.year + 1 - self._period_year
         p = Scientist([auth_id], self.year, period=period, refresh=refresh,
                       sql_fname=self.sql_fname)
-        match_info = inform_match(p, keywords)
+        match_info = inform_match(p, keywords, refresh=refresh)
         # Abstract and reference similarity is performed jointly
         if doc_parse:
             eids = [d.eid for d in p.publications]
             refs, refs_n = parse_docs(eids, refresh)
             completeness[auth_id] = (refs_n, len(eids))
             if "num_cited_refs" in keywords:
-                ref_cos = compute_overlap(refs, focal_refs, **kwds)
+                ref_cos = compute_overlap(refs, focal_refs)
                 match_info["num_cited_refs"] = ref_cos
         out.append(m(**match_info))
         print_progress(idx+1, total, verbose)
 
     # Eventually print information on missing information
     if verbose and doc_parse:
         for auth_id, completeness in completeness.items():
```

### Comparing `sosia-0.5.0/sosia/processing/filtering.py` & `sosia-0.6/sosia/processing/filtering.py`

 * *Files identical despite different names*

### Comparing `sosia-0.5.0/sosia/processing/finding.py` & `sosia-0.6/sosia/processing/finding.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from itertools import product
 from string import Template
 
-from pandas import DataFrame
+import pandas as pd
 
 from sosia.processing.caching import insert_data, retrieve_author_info
 from sosia.processing.extracting import extract_authors
 from sosia.processing.filtering import filter_pub_counts, same_affiliation
 from sosia.processing.getting import get_authors_from_sourceyear, get_authors
 from sosia.processing.querying import base_query, count_citations, stacked_query
 from sosia.processing.utils import build_dict, flat_set_from_df, margin_range
@@ -74,15 +74,15 @@
         params.update({"npapers": [1, _max_papers], "yfrom": None,
                        "group": group})
         group, _, _ = filter_pub_counts(**params)
     text = f"Left with {len(group):,} researchers"
     custom_print(text, verbose)
 
     # Third round of filtering: citations (in the FULL period)
-    authors = DataFrame({"auth_id": group, "year": original.year})
+    authors = pd.DataFrame({"auth_id": group, "year": original.year})
     auth_cits, missing = retrieve_author_info(authors, conn, "author_ncits")
     if not missing.empty:
         total = missing.shape[0]
         text = f"Counting citations of {total:,} authors..."
         custom_print(text, verbose)
         missing['n_cits'] = 0
         print_progress(0, total, verbose)
@@ -90,41 +90,42 @@
         for i, au in missing.iterrows():
             n_cits = count_citations([str(au['auth_id'])], original.year+1)
             missing.at[i, 'n_cits'] = n_cits
             print_progress(i + 1, total, verbose)
             if i % 100 == 0 or i == len(missing) - 1:
                 insert_data(missing.iloc[start:i+1], conn, table="author_ncits")
                 start = i
-    auth_cits = auth_cits.append(missing)
+    auth_cits = pd.concat([auth_cits, missing])
     auth_cits['auth_id'] = auth_cits['auth_id'].astype("uint64")
     # Keep if citations are in range
     custom_print("Filtering based on count of citations...", verbose)
     mask = auth_cits["n_cits"].between(min(_ncits), _max_cits)
     group = auth_cits[mask]['auth_id'].tolist()
 
     # Fourth round of filtering: Download publications, verify coauthors
     # (in the FULL period) and first year
     text = f"Left with {len(group):,} authors\nFiltering based on "\
            "coauthor count..."
     custom_print(text, verbose)
-    authors = DataFrame({"auth_id": group, "year": original.year}, dtype="uint64")
+    authors = pd.DataFrame({"auth_id": group, "year": original.year},
+                           dtype="uint64")
     _, author_year_search = retrieve_author_info(authors, conn, "author_year")
     matches = []
 
     if not author_year_search.empty:
         q = Template(f"AU-ID($fill) AND PUBYEAR BEF {original.year + 1}")
         auth_year_group = author_year_search["auth_id"].tolist()
         params = {"group": auth_year_group, "template": q, "refresh": refresh,
                   "joiner": ") OR AU-ID(", "q_type": "docs",
                   "verbose": verbose, "stacked": stacked}
         res = stacked_query(**params)
         res = build_dict(res, auth_year_group)
         if res:
             # res can become empty after build_dict if a au_id is old
-            res = DataFrame.from_dict(res, orient="index")
+            res = pd.DataFrame.from_dict(res, orient="index")
             res["year"] = original.year
             res = res[["year", "first_year", "n_pubs", "n_coauth"]]
             res.index.name = "auth_id"
             res = res.reset_index()
             insert_data(res, original.sql_conn, table="author_year")
     authors_year, _ = retrieve_author_info(authors, conn, "author_year")
     # Check for number of coauthors within margin
@@ -192,31 +193,31 @@
     """
     # Define variables
     search_sources, _ = zip(*original.search_sources)
     text = f"Defining 'search_group' using up to {len(search_sources):,} sources..."
     custom_print(text, verbose)
 
     # Retrieve author list for today
-    sources_today = DataFrame(product(search_sources, [original.active_year]),
-                              columns=["source_id", "year"])
+    sources_today = pd.DataFrame(product(search_sources, [original.active_year]),
+                                 columns=["source_id", "year"])
     auth_today = get_authors_from_sourceyear(sources_today, original.sql_conn,
         refresh=refresh, stacked=stacked, verbose=verbose)
     mask = None
     if original.search_affiliations:
         mask = auth_today["afid"].isin(original.search_affiliations)
     today = flat_set_from_df(auth_today, "auids", condition=mask)
 
     # Authors active around year of first publication
     min_year = original.first_year - original.first_year_margin
     max_year = original.first_year + original.first_year_margin
     then_years = [min_year-1]
     if not original.first_year_name_search:
         then_years.extend(range(min_year, max_year+1))
-    sources_then = DataFrame(product(search_sources, then_years),
-                             columns=["source_id", "year"])
+    sources_then = pd.DataFrame(product(search_sources, then_years),
+                                columns=["source_id", "year"])
     auth_then = get_authors_from_sourceyear(sources_then, original.sql_conn,
         refresh=refresh, stacked=stacked, verbose=verbose)
     mask = auth_then["year"].between(min_year, max_year)
     then = flat_set_from_df(auth_then, "auids", condition=mask)
 
     # Remove authors active before
     mask = auth_then["year"] < min_year
```

### Comparing `sosia-0.5.0/sosia/processing/getting.py` & `sosia-0.6/sosia/processing/getting.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,24 +87,24 @@
     for year in missing["year"].unique():
         subset = missing[missing["year"] == year]
         sources = subset["source_id"].unique()
         new = query_pubs_by_sourceyear(sources, year, refresh=refresh,
                                        stacked=stacked, verbose=verbose)
         no_info = set(sources) - set(new["source_id"].unique())
         empty.extend([(s, year) for s in no_info])
-        to_add = to_add.append(new)
+        to_add = pd.concat([to_add, new])
 
     # Format useful information
-    data = data.append(to_add)
+    data = pd.concat([data, to_add])
     data = data[data["auids"] != ""]
     data["auids"] = data["auids"].str.replace(";", ",").str.split(",")
 
     # Insert new information and information on missing data
     if empty:
         sources, years = list(zip(*empty))
         d = {"source_id": sources, "year": years, "auids": [""]*len(sources),
              "afid": [""]*len(sources)}
-        to_add = to_add.append(pd.DataFrame(d))
+        to_add = pd.concat([to_add, pd.DataFrame(d)])
     if not to_add.empty:
         to_add["auids"] = to_add["auids"].str.replace(";", ",").str.split(",")
         insert_data(to_add, conn, table="sources_afids")
     return data
```

### Comparing `sosia-0.5.0/sosia/processing/initializing.py` & `sosia-0.6/sosia/processing/initializing.py`

 * *Files identical despite different names*

### Comparing `sosia-0.5.0/sosia/processing/querying.py` & `sosia-0.6/sosia/processing/querying.py`

 * *Files identical despite different names*

### Comparing `sosia-0.5.0/sosia/processing/tests/test_extracting.py` & `sosia-0.6/sosia/processing/tests/test_extracting.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,22 @@
-# -*- coding: utf-8 -*-
 """Tests for processing.extracting module."""
 
-from os.path import expanduser
-
 from nose.tools import assert_equal
 from pybliometrics.scopus import ScopusSearch
 
-from sosia.processing import find_location, parse_docs, get_main_field
+from sosia.processing import find_main_affiliation, get_main_field, parse_docs
 
 refresh = 30
-test_cache = expanduser("~/.sosia/") + "test.sqlite"
 test_id = 6701809842
 
 
-def test_find_location():
+def test_find_main_affiliation():
     pubs = ScopusSearch(f"AU-ID({test_id})", refresh=refresh).results
-    ctry, aid, aff = find_location([test_id], pubs, 2000, refresh=30)
-    assert_equal(ctry, "Germany")
-    assert_equal(aid, "60028717")
-    assert_equal(aff, "Universität München")
+    aff_id = find_main_affiliation([test_id], pubs, 2000)
+    assert_equal(aff_id, "60028717")
 
 
 def test_get_main_field():
     fields = [1000, 1000, 2000, 2000, 2020, 2020]
     received = get_main_field(fields)
     expected = (2020, "ECON")
     assert_equal(received, expected)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `sosia-0.5.0/sosia/processing/tests/test_filtering.py` & `sosia-0.6/sosia/processing/tests/test_filtering.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,35 @@
-# -*- coding: utf-8 -*-
 """Tests for processing.filtering module."""
 
-from os.path import expanduser
+from pathlib import Path
 
 from nose.tools import assert_equal, assert_false, assert_true
 
 from sosia.classes import Original
-from sosia.establishing import connect_database
+from sosia.establishing import make_database, connect_database
 from sosia.processing.filtering import filter_pub_counts, same_affiliation
 
-test_cache = expanduser("~/.sosia/test.sqlite")
-test_conn = connect_database(test_cache)
+test_cache = Path.home()/".cache/sosia/test.sqlite"
 
 
 def test_filter_pub_counts():
+    make_database(test_cache, drop=True)
+    test_conn = connect_database(test_cache)
     group = [6701809842, 16319073600, 54984906100, 56148489300, 57131011400,
              57194816659, 35097480000, 56055501900, 20434039300, 6602070937]
     npapers = range(2, 60)
     g, pubs, older = filter_pub_counts(group, test_conn, 1993, 2005, npapers)
     assert_equal(sorted(g), [6602070937, 6701809842, 35097480000])
     assert_equal(sorted(pubs), [3, 15, 17])
     assert_equal(sorted(older), [20434039300, 54984906100, 56148489300])
 
 
 def test_filter_pub_counts_period():
+    make_database(test_cache, drop=True)
+    test_conn = connect_database(test_cache)
     group = [6701809842, 16319073600, 54984906100, 56148489300, 57131011400,
              57194816659, 35097480000, 56055501900, 20434039300, 6602070937]
     npapers = range(2, 60)
     g, pubs, older = filter_pub_counts(group, test_conn, 1993, 2005, npapers, yfrom=2005)
     assert_equal(sorted(g), [6602070937])
     assert_equal(sorted(pubs), [2])
     assert_equal(sorted(older), [20434039300, 54984906100, 56148489300])
```

### Comparing `sosia-0.5.0/sosia/processing/tests/test_getting.py` & `sosia-0.6/sosia/processing/tests/test_getting.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-# -*- coding: utf-8 -*-
 """Tests for processing.getting module."""
 
-from os.path import expanduser
+from pathlib import Path
 
 from nose.tools import assert_equal, assert_true
 from pandas import DataFrame
 
-from sosia.establishing import connect_database
+from sosia.establishing import connect_database, make_database
 from sosia.processing.getting import get_authors
 
-test_cache = expanduser("~/.sosia/test.sqlite")
-test_conn = connect_database(test_cache)
+test_cache = Path.home()/".cache/sosia/test.sqlite"
 refresh = 30
 
 
 def test_query_authors():
     auth_list = [6701809842, 55208373700]
+    test_conn = connect_database(test_cache)
     auth_data = get_authors(auth_list, test_conn, refresh=refresh)
     assert_true(isinstance(auth_data,  DataFrame))
     expected_cols = ["auth_id", "eid", "surname", "initials", "givenname",
                      "affiliation", "documents", "affiliation_id", "city",
                      "country", "areas"]
     assert_equal(auth_data.columns.tolist(), expected_cols)
     assert_equal(auth_data["auth_id"].tolist(), auth_list)
```

### Comparing `sosia-0.5.0/sosia/processing/tests/test_initializing.py` & `sosia-0.6/sosia/processing/tests/test_initializing.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,23 @@
-# -*- coding: utf-8 -*-
 """Tests for processing.initializing module."""
 
+from pathlib import Path
+
 import pandas as pd
 from nose.tools import assert_equal
 
 from sosia.classes import Scientist
+from sosia.establishing import make_database
 from sosia.processing.initializing import add_source_names,\
     read_fields_sources_list
 
+test_cache = Path.home()/".cache/sosia/test.sqlite"
 
 def test_add_source_names():
-    s = Scientist([55208373700], 2017)
+    s = Scientist([55208373700], 2017, sql_fname=test_cache)
     expected = [(14351, "Brain Research Reviews"),
                 (18632, "Progress in Brain Research")]
     ids, names = zip(*expected)
     received = add_source_names(ids, s.source_names)
     assert_equal(received, expected)
```

### Comparing `sosia-0.5.0/sosia/processing/tests/test_querying.py` & `sosia-0.6/sosia/processing/tests/test_querying.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,16 @@
-# -*- coding: utf-8 -*-
 """Tests for processing.querying module."""
 
-from os.path import expanduser
+from string import Template
 
 from nose.tools import assert_equal, assert_true
-from string import Template
 
-from sosia.establishing import connect_database
 from sosia.processing import base_query, count_citations, create_queries,\
     query_pubs_by_sourceyear, stacked_query
 
-test_cache = expanduser("~/.sosia/test.sqlite")
-test_conn = connect_database(test_cache)
 test_id = 53164702100
 year = 2017
 refresh = 30
 
 
 def test_base_query():
     q = f"AU-ID({test_id}) AND PUBYEAR BEF {year}"
@@ -28,15 +23,15 @@
     size = base_query("author", query, size_only=True)
     assert_equal(size, 1)
 
 
 def test_count_citations():
     identifier = ["55208373700", "55208373700"]
     count1 = count_citations(identifier, 2017)
-    assert_equal(count1, 22)
+    assert_equal(count1, 24)
     eids = ["2-s2.0-84959420483", "2-s2.0-84949113230"]
     count2 = count_citations(eids, 2017, exclusion_ids=identifier)
     assert_equal(count2, 1)
     eids_long = eids * 100
     count3 = count_citations(eids_long, 2017, exclusion_ids=identifier)
     assert_equal(count3, 1)
```

### Comparing `sosia-0.5.0/sosia/processing/tests/test_utils.py` & `sosia-0.6/sosia/processing/tests/test_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """Tests for processing.utils module."""
 
 import pandas as pd
 from nose.tools import assert_equal, assert_true
 from pybliometrics.scopus import ScopusSearch
 
 from sosia.processing import compute_overlap, expand_affiliation,\
```

### Comparing `sosia-0.5.0/sosia/processing/utils.py` & `sosia-0.6/sosia/processing/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,24 +43,21 @@
 
 
 def expand_affiliation(df):
     """Auxiliary function to expand the information about the affiliation
     in publications from ScopusSearch.
     """
     from pandas import Series
-    res = df[["source_id", "author_ids", "afid"]].copy()
-    res['afid'] = res["afid"].str.split(';')
-    res = (res["afid"].apply(Series)
-              .merge(res, right_index=True, left_index=True)
-              .drop(["afid"], axis=1)
-              .melt(id_vars=['source_id', 'author_ids'], value_name="afid")
-              .drop("variable", axis=1)
-              .dropna())
-    res['afid'] = res['afid'].astype(float)
-    return res
+    temp = df.set_index(["source_id", "author_ids"])[["afid"]]
+    temp = (temp["afid"].str.split(";", expand=True)
+                .stack().dropna().reset_index()
+                .drop("level_2", axis=1)
+                .rename(columns={0: "afid"}))
+    temp['afid'] = temp['afid'].astype(float)
+    return temp
 
 
 def flat_set_from_df(df, col, condition=None):
     """Flatten Series from DataFrame which contains lists and
     return as set, optionally after filtering the DataFrame.
     """
     if condition is not None:
```

### Comparing `sosia-0.5.0/sosia/utils/decorators.py` & `sosia-0.6/sosia/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `sosia-0.5.0/sosia/utils/helpers.py` & `sosia-0.6/sosia/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `sosia-0.5.0/sosia.egg-info/PKG-INFO` & `sosia-0.6/sosia.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,112 +1,113 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: sosia
-Version: 0.5.0
+Version: 0.6
 Summary: Find control groups for academics in Scopus
-Home-page: UNKNOWN
-Author: Stefano H. Barruffaldi and Michael E. Rose
-Author-email: Michael.Ernst.Rose@gmail.com
-Maintainer: Michael E. Rose
-Maintainer-email: Michael.Ernst.Rose@gmail.com
+Author-email: "Michael E. Rose and Stefano H. Baruffaldi" <Michael.Ernst.Rose@gmail.com>
+Maintainer-email: "Michael E. Rose" <Michael.Ernst.Rose@gmail.com>
 License: MIT
-Description: sosia
-        =====
-        
-        Match authors automatically in Scopus on-line
-        
-        Documentation: https://sosia.readthedocs.io
-        
-        Development: https://github.com/sosia-dev/sosia
-        
-        .. image:: https://badge.fury.io/py/sosia.svg
-            :target: https://badge.fury.io/py/sosia
-        
-        .. image:: https://readthedocs.org/projects/sosia/badge/?version=latest
-            :target: https://readthedocs.org/projects/sosia/badge/?version=latest
-        
-        .. image:: https://img.shields.io/pypi/pyversions/sosia.svg
-            :target: https://img.shields.io/pypi/pyversions/sosia.svg
-        
-        .. image:: https://img.shields.io/pypi/l/sosia.svg
-            :target: https://img.shields.io/pypi/l/sosia.svg
-        
-        .. image:: https://api.codeclimate.com/v1/badges/3e10a47fefae831b973a/maintainability
-           :target: https://codeclimate.com/github/sosia-dev/sosia/maintainability
-        
-        Installation
-        ============
-        
-        Install stable version from PyPI:
-        
-        .. code:: bash
-        
-            pip install sosia
-        
-        or development version from GitHub repository:
-        
-        .. code:: bash
-        
-            pip install git+https://github.com/sosia-dev/sosia
-        
-        Functioning
-        ===========
-        
-        sosia performs a series of queries in the Scopus database using the `pybliometrics package 
-        <http://pybliometrics.readthedocs.io/>`_.  After configuring your local pybliometrics (providing access credentials and eventually setting cache directories), you can use sosia:
-        
-        .. inclusion-marker-start
-        .. code-block:: python
-        
-            >>> import sosia
-            >>> 
-            >>> sosia.create_fields_sources_list()  # Necessary only once
-            >>> sosia.make_database()  # Necessary only once
-            >>> 
-            >>> stefano = sosia.Original(55208373700, 2019)  # Scopus ID and year
-            >>> stefano.define_search_sources()  # Sources similiar to scientist
-            >>> stefano.define_search_group()  # Authors publishing in similar sources
-            >>> stefano.find_matches()  # Find matches satisfying all criteria
-            >>> print(stefano.matches)
-            >>> ['55022752500', '55810688700', '55824607400']
-            >>> stefano.inform_matches()  # Optional step to provide additional information
-            >>> print(stefano.matches[0])
-            Match(ID='55022752500', name='Van der Borgh, Michel', first_name='Michel',
-            surname='Van der Borgh', first_year=2012, num_coauthors=6, num_publications=5,
-            num_citations=33, num_coauthors_period=6, num_publications_period=5,
-            num_citations_period=33, subjects=['BUSI', 'COMP', 'SOCI'], country='Netherlands',
-            affiliation_id='60032882', affiliation='Eindhoven University of Technology,
-            Department of Industrial Engineering & Innovation Sciences', language='eng',
-            reference_sim=0.0, abstract_sim=0.1217)
-        
-        
-        .. inclusion-marker-end
-        
-        Change log
-        ==========
-        
-        Please see `CHANGES.rst <./meta/CHANGES.rst>`_.
-        
-        Contributing
-        ============
-        
-        Please see `CONTRIBUTING.rst <CONTRIBUTING.rst>`_.  For the list of contributors see
-        `AUTHORS.rst <./meta/AUTHORS.rst>`_.
-        
-        License
-        =======
-        
-        MIT License; see `LICENSE <LICENSE>`_.
-        
-        
-Keywords: sosia
-Platform: UNKNOWN
+Project-URL: Homepage, https://github.com/sosia-dev/sosia
+Project-URL: Bug Tracker, https://github.com/sosia-dev/sosia/issues
+Project-URL: Documentation (stable), https://sosia.readthedocs.io/en/stable/
+Project-URL: Documentation (latest), https://sosia.readthedocs.io/en/latest/
+Keywords: sosia,control groups,research
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+sosia
+=====
+
+Match authors automatically in Scopus on-line
+
+Documentation: https://sosia.readthedocs.io
+
+Development: https://github.com/sosia-dev/sosia
+
+.. image:: https://badge.fury.io/py/sosia.svg
+    :target: https://badge.fury.io/py/sosia
+
+.. image:: https://readthedocs.org/projects/sosia/badge/?version=latest
+    :target: https://readthedocs.org/projects/sosia/badge/?version=latest
+
+.. image:: https://img.shields.io/pypi/pyversions/sosia.svg
+    :target: https://img.shields.io/pypi/pyversions/sosia.svg
+
+.. image:: https://img.shields.io/pypi/l/sosia.svg
+    :target: https://img.shields.io/pypi/l/sosia.svg
+
+.. image:: https://api.codeclimate.com/v1/badges/3e10a47fefae831b973a/maintainability
+   :target: https://codeclimate.com/github/sosia-dev/sosia/maintainability
+
+Installation
+============
+
+Install stable version from PyPI:
+
+.. code:: bash
+
+    pip install sosia
+
+or development version from GitHub repository:
+
+.. code:: bash
+
+    pip install git+https://github.com/sosia-dev/sosia
+
+Functioning
+===========
+
+sosia performs a series of queries in the Scopus database using the `pybliometrics package 
+<http://pybliometrics.readthedocs.io/>`_.  After configuring your local pybliometrics (providing access credentials and eventually setting cache directories), you can use sosia:
+
+.. inclusion-marker-start
+.. code-block:: python
+
+    >>> import sosia
+    >>> 
+    >>> sosia.create_fields_sources_list()  # Necessary only once
+    >>> sosia.make_database()  # Necessary only once
+    >>> 
+    >>> stefano = sosia.Original(55208373700, 2019)  # Scopus ID and year
+    >>> stefano.define_search_sources()  # Sources similiar to scientist
+    >>> stefano.define_search_group()  # Authors publishing in similar sources
+    >>> stefano.find_matches()  # Find matches satisfying all criteria
+    >>> print(stefano.matches)
+    >>> ['55022752500', '55810688700', '55824607400']
+    >>> stefano.inform_matches()  # Optional step to provide additional information
+    >>> print(stefano.matches[0])
+    Match(ID='55022752500', name='Van der Borgh, Michel', first_name='Michel',
+    surname='Van der Borgh', first_year=2012, num_coauthors=6, num_publications=5,
+    num_citations=33, num_coauthors_period=6, num_publications_period=5,
+    num_citations_period=33, subjects=['BUSI', 'COMP', 'SOCI'], country='Netherlands',
+    affiliation_id='60032882', affiliation='Eindhoven University of Technology,
+    Department of Industrial Engineering & Innovation Sciences', language='eng',
+    reference_sim=0.0, abstract_sim=0.1217)
+
+
+.. inclusion-marker-end
+
+Change log
+==========
+
+Please see `CHANGES.rst <./meta/CHANGES.rst>`_.
+
+Contributing
+============
+
+Please see `CONTRIBUTING.rst <CONTRIBUTING.rst>`_.  For the list of contributors see
+`AUTHORS.rst <./meta/AUTHORS.rst>`_.
+
+License
+=======
+
+MIT License; see `LICENSE <LICENSE>`_.
```

### Comparing `sosia-0.5.0/sosia.egg-info/SOURCES.txt` & `sosia-0.6/sosia.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,47 +1,45 @@
+.gitignore
 CONTRIBUTING.rst
 LICENSE
 README.rst
-requirements.txt
-setup.cfg
-setup.py
+pyproject.toml
+docs/.readthedocs.yaml
 docs/Makefile
 docs/authors.rst
 docs/changelog.rst
 docs/conf.py
 docs/contributing.rst
 docs/functioning.rst
 docs/index.rst
 docs/make.bat
 docs/reference.rst
+docs/requirements.txt
 docs/tutorial.rst
 docs/reference/sosia.Original.rst
 docs/tutorial/installation.rst
 docs/tutorial/refining.rst
 docs/tutorial/setup.rst
 docs/tutorial/usage.rst
 meta/AUTHORS.rst
 meta/CHANGES.rst
 sosia/README.md
 sosia/__init__.py
 sosia.egg-info/PKG-INFO
 sosia.egg-info/SOURCES.txt
 sosia.egg-info/dependency_links.txt
-sosia.egg-info/not-zip-safe
-sosia.egg-info/pbr.json
 sosia.egg-info/requires.txt
 sosia.egg-info/top_level.txt
 sosia/classes/__init__.py
 sosia/classes/original.py
 sosia/classes/scientist.py
 sosia/classes/tests/__init__.py
 sosia/classes/tests/test_Original.py
 sosia/classes/tests/test_Scientist.py
 sosia/establishing/__init__.py
-sosia/establishing/config.py
 sosia/establishing/constants.py
 sosia/establishing/database.py
 sosia/establishing/fields_sources.py
 sosia/establishing/tests/__init__.py
 sosia/establishing/tests/test_database.py
 sosia/establishing/tests/test_fields_sources.py
 sosia/processing/__init__.py
@@ -64,9 +62,8 @@
 sosia/processing/tests/test_filtering.py
 sosia/processing/tests/test_getting.py
 sosia/processing/tests/test_initializing.py
 sosia/processing/tests/test_querying.py
 sosia/processing/tests/test_utils.py
 sosia/utils/__init__.py
 sosia/utils/decorators.py
-sosia/utils/defaults.py
 sosia/utils/helpers.py
```

