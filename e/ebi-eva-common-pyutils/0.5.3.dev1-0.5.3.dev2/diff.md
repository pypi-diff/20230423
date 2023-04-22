# Comparing `tmp/ebi_eva_common_pyutils-0.5.3.dev1.tar.gz` & `tmp/ebi_eva_common_pyutils-0.5.3.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebi_eva_common_pyutils-0.5.3.dev1.tar", last modified: Fri Apr 21 23:21:21 2023, max compression
+gzip compressed data, was "ebi_eva_common_pyutils-0.5.3.dev2.tar", last modified: Sat Apr 22 22:41:43 2023, max compression
```

## Comparing `ebi_eva_common_pyutils-0.5.3.dev1.tar` & `ebi_eva_common_pyutils-0.5.3.dev2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-04-21 23:21:21.401457 ebi_eva_common_pyutils-0.5.3.dev1/
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     1492 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev1/CHANGELOG.md
--rw-r--r--   0 nkumar2   (9636) eva       (1254)    11357 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev1/LICENSE
--rw-r--r--   0 nkumar2   (9636) eva       (1254)       28 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev1/MANIFEST.in
--rw-r--r--   0 nkumar2   (9636) eva       (1254)      517 2023-04-21 23:21:21.401457 ebi_eva_common_pyutils-0.5.3.dev1/PKG-INFO
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     1434 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev1/README.md
-drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-04-21 23:21:21.401457 ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/
--rw-r--r--   0 nkumar2   (9636) eva       (1254)        0 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/__init__.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     4984 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/archive_directory.py
-drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-04-21 23:21:21.401457 ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/assembly/
--rw-r--r--   0 nkumar2   (9636) eva       (1254)       66 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/assembly/__init__.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)      673 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/assembly/assembly.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     2151 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/command_utils.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     1192 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/common_utils.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     2242 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/config.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     8342 2023-04-21 07:36:06.000000 ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/config_utils.py
-drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-04-21 23:21:21.401457 ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/contig_alias/
--rw-r--r--   0 nkumar2   (9636) eva       (1254)        0 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/contig_alias/__init__.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     3056 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/contig_alias/contig_alias.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     1452 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/ena_utils.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     1375 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/file_utils.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     4990 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/logger.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)    13489 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/metadata_utils.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     3589 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/mongo_utils.py
-drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-04-21 23:21:21.401457 ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/mongodb/
--rw-r--r--   0 nkumar2   (9636) eva       (1254)       72 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/mongodb/__init__.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     9676 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/mongodb/mongo_database.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     4965 2023-04-21 08:17:45.000000 ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/ncbi_utils.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     2285 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/network_utils.py
-drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-04-21 23:21:21.401457 ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/nextflow/
--rw-r--r--   0 nkumar2   (9636) eva       (1254)      120 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/nextflow/__init__.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)    10114 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/nextflow/nextflow_pipeline.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     4398 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/pg_utils.py
-drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-04-21 23:21:21.401457 ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/reference/
--rw-r--r--   0 nkumar2   (9636) eva       (1254)      134 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/reference/__init__.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)    12162 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/reference/assembly.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     3911 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/reference/sequence.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)    13457 2023-04-21 21:06:06.000000 ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/spring_properties.py
-drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-04-21 23:21:21.401457 ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/taxonomy/
--rw-r--r--   0 nkumar2   (9636) eva       (1254)        0 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/taxonomy/__init__.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     2259 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/taxonomy/taxonomy.py
-drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-04-21 23:21:21.401457 ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/variation/
--rw-r--r--   0 nkumar2   (9636) eva       (1254)        0 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/variation/__init__.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     3515 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/variation/assembly_utils.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     5230 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/variation/contig_utils.py
-drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-04-21 23:21:21.401457 ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils.egg-info/
--rw-r--r--   0 nkumar2   (9636) eva       (1254)      517 2023-04-21 23:21:21.000000 ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils.egg-info/PKG-INFO
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     1699 2023-04-21 23:21:21.000000 ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils.egg-info/SOURCES.txt
--rw-r--r--   0 nkumar2   (9636) eva       (1254)        1 2023-04-21 23:21:21.000000 ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils.egg-info/dependency_links.txt
--rw-r--r--   0 nkumar2   (9636) eva       (1254)       81 2023-04-21 23:21:21.000000 ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils.egg-info/requires.txt
--rw-r--r--   0 nkumar2   (9636) eva       (1254)       23 2023-04-21 23:21:21.000000 ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils.egg-info/top_level.txt
--rw-r--r--   0 nkumar2   (9636) eva       (1254)      225 2023-04-21 23:21:21.401457 ebi_eva_common_pyutils-0.5.3.dev1/setup.cfg
--rw-r--r--   0 nkumar2   (9636) eva       (1254)      912 2023-04-21 23:21:05.000000 ebi_eva_common_pyutils-0.5.3.dev1/setup.py
+drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-04-22 22:41:43.068881 ebi_eva_common_pyutils-0.5.3.dev2/
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     1492 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev2/CHANGELOG.md
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)    11357 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev2/LICENSE
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)       28 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev2/MANIFEST.in
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)      517 2023-04-22 22:41:43.068881 ebi_eva_common_pyutils-0.5.3.dev2/PKG-INFO
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     1434 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev2/README.md
+drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-04-22 22:41:43.064881 ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)        0 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/__init__.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     4984 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/archive_directory.py
+drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-04-22 22:41:43.064881 ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/assembly/
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)       66 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/assembly/__init__.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)      673 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/assembly/assembly.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     2151 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/command_utils.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     1192 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/common_utils.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     2242 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/config.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     8342 2023-04-21 07:36:06.000000 ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/config_utils.py
+drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-04-22 22:41:43.064881 ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/contig_alias/
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)        0 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/contig_alias/__init__.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     3056 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/contig_alias/contig_alias.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     1452 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/ena_utils.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     1375 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/file_utils.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     4990 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/logger.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)    13489 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/metadata_utils.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     3589 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/mongo_utils.py
+drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-04-22 22:41:43.064881 ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/mongodb/
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)       72 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/mongodb/__init__.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     9676 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/mongodb/mongo_database.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     4965 2023-04-21 08:17:45.000000 ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/ncbi_utils.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     2285 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/network_utils.py
+drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-04-22 22:41:43.064881 ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/nextflow/
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)      120 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/nextflow/__init__.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)    10114 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/nextflow/nextflow_pipeline.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     4398 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/pg_utils.py
+drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-04-22 22:41:43.064881 ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/reference/
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)      134 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/reference/__init__.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)    12162 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/reference/assembly.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     3911 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/reference/sequence.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)    14210 2023-04-22 22:24:07.000000 ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/spring_properties.py
+drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-04-22 22:41:43.068881 ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/taxonomy/
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)        0 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/taxonomy/__init__.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     2259 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/taxonomy/taxonomy.py
+drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-04-22 22:41:43.068881 ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/variation/
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)        0 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/variation/__init__.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     3515 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/variation/assembly_utils.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     5230 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/variation/contig_utils.py
+drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-04-22 22:41:43.064881 ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils.egg-info/
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)      517 2023-04-22 22:41:43.000000 ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils.egg-info/PKG-INFO
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     1699 2023-04-22 22:41:43.000000 ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils.egg-info/SOURCES.txt
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)        1 2023-04-22 22:41:43.000000 ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils.egg-info/dependency_links.txt
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)       81 2023-04-22 22:41:43.000000 ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils.egg-info/requires.txt
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)       23 2023-04-22 22:41:43.000000 ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils.egg-info/top_level.txt
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)      225 2023-04-22 22:41:43.068881 ebi_eva_common_pyutils-0.5.3.dev2/setup.cfg
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)      912 2023-04-22 22:41:04.000000 ebi_eva_common_pyutils-0.5.3.dev2/setup.py
```

### Comparing `ebi_eva_common_pyutils-0.5.3.dev1/CHANGELOG.md` & `ebi_eva_common_pyutils-0.5.3.dev2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev1/LICENSE` & `ebi_eva_common_pyutils-0.5.3.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev1/PKG-INFO` & `ebi_eva_common_pyutils-0.5.3.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebi_eva_common_pyutils
-Version: 0.5.3.dev1
+Version: 0.5.3.dev2
 Summary: EBI EVA - Common Python Utilities
 Home-page: https://github.com/EBIVariation/eva-common-pyutils
 License: Apache
 Keywords: EBI,EVA,PYTHON,UTILITIES
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `ebi_eva_common_pyutils-0.5.3.dev1/README.md` & `ebi_eva_common_pyutils-0.5.3.dev2/README.md`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/archive_directory.py` & `ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/archive_directory.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/assembly/assembly.py` & `ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/assembly/assembly.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/command_utils.py` & `ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/command_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/common_utils.py` & `ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/common_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/config.py` & `ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/config.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/config_utils.py` & `ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/config_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/contig_alias/contig_alias.py` & `ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/contig_alias/contig_alias.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/ena_utils.py` & `ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/ena_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/file_utils.py` & `ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/file_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/logger.py` & `ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/logger.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/metadata_utils.py` & `ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/metadata_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/mongo_utils.py` & `ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/mongo_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/mongodb/mongo_database.py` & `ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/mongodb/mongo_database.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/ncbi_utils.py` & `ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/ncbi_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/network_utils.py` & `ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/network_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/nextflow/nextflow_pipeline.py` & `ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/nextflow/nextflow_pipeline.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/pg_utils.py` & `ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/pg_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/reference/assembly.py` & `ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/reference/assembly.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/reference/sequence.py` & `ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/reference/sequence.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/spring_properties.py` & `ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/spring_properties.py`

 * *Files 6% similar despite different names*

```diff
@@ -119,72 +119,97 @@
                 'parameters.projectAccession': project_accession,
                 'parameters.taxonomyAccession': taxonomy_accession,
                 'parameters.vcfAggregation': aggregation,
                 'parameters.vcf': vcf_file,
                 'parameters.outputVcf': output_vcf
             },
         )
-
-    def get_variant_load_properties(self,  project_accession, study_name, output_dir, annotation_dir, stats_dir,
-                                    vep_cache_path, read_preference='secondaryPreferred'):
+    def _common_eva_pipeline_properties(self, opencga_path, read_preference='se'):
         mongo_host, mongo_user, mongo_pass = get_primary_mongo_creds_for_profile(
             self.maven_profile, self.private_settings_file)
         counts_url, counts_username, counts_password = get_count_service_creds_for_profile(
             self.maven_profile, self.private_settings_file)
-        variant_url, variant_user, variant_pass = get_variant_pg_creds_for_profile(self.maven_profile, self.private_settings_file)
-        files_collection = get_properties_from_xml_file(
-            self.maven_profile, self.private_settings_file)['eva.mongo.collections.files']
-        variants_collection = get_properties_from_xml_file(
-            self.maven_profile, self.private_settings_file)['eva.mongo.collections.variants']
-        annotation_metadata_collection = get_properties_from_xml_file(
-            self.maven_profile, self.private_settings_file)['eva.mongo.collections.annotation-metadata']
-        annotation_collection = get_properties_from_xml_file(
-            self.maven_profile, self.private_settings_file)['eva.mongo.collections.annotations']
+        variant_url, variant_user, variant_pass = get_variant_pg_creds_for_profile(self.maven_profile,
+                                                                                   self.private_settings_file)
 
-        return self._format({
+        return {
             'spring.profiles.active': 'production,mongo',
             'spring.profiles.include': 'variant-writer-mongo,variant-annotation-mongo',
 
             'spring.data.mongodb.authentication-database': 'admin',
             'spring.data.mongodb.host': mongo_host,
             'spring.data.mongodb.password': mongo_pass,
             'spring.data.mongodb.port': 27017,
             'spring.data.mongodb.username': mongo_user,
             'spring.data.mongodb.authentication-mechanism': 'SCRAM-SHA-1',
+
             'job.repository.driverClassName': 'org.postgresql.Driver',
             'job.repository.url': variant_url,
             'job.repository.username': variant_user,
             'job.repository.password': variant_pass,
+
             'eva.count-stats.url': counts_url,
             'eva.count-stats.username': counts_username,
             'eva.count-stats.password': counts_password,
 
-            'app.opencga.path': '/nfs/production/keane/eva/software/opencga/',
-            'app.vep.cache.path': vep_cache_path,
+            'app.opencga.path': opencga_path,
+            'config.restartability.allow': 'false',
+            'config.db.read-preference': read_preference,
+
+            'logging.level.embl.ebi.variation.eva': 'DEBUG',
+            'logging.level.org.opencb.opencga': 'DEBUG',
+            'logging.level.org.springframework': 'INFO',
+
+            'spring.main.allow-bean-definition-overriding': 'true',
+            }
+
+    def get_accession_import_properties(self, opencga_path, read_preference='secondaryPreferred'):
+        variants_collection = get_properties_from_xml_file(
+            self.maven_profile, self.private_settings_file)['eva.mongo.collections.variants']
+
+        return self._format(
+            self._common_eva_pipeline_properties(opencga_path, read_preference),
+            {
+                'db.collections.variants.name': variants_collection,
+            },
+        )
 
+    def get_variant_load_properties(self,  project_accession, study_name, output_dir, annotation_dir, stats_dir,
+                                    vep_cache_path, opencga_path, read_preference='secondaryPreferred'):
+        variants_collection = get_properties_from_xml_file(
+            self.maven_profile, self.private_settings_file)['eva.mongo.collections.variants']
+        files_collection = get_properties_from_xml_file(
+            self.maven_profile, self.private_settings_file)['eva.mongo.collections.files']
+        annotation_metadata_collection = get_properties_from_xml_file(
+            self.maven_profile, self.private_settings_file)['eva.mongo.collections.annotation-metadata']
+        annotation_collection = get_properties_from_xml_file(
+            self.maven_profile, self.private_settings_file)['eva.mongo.collections.annotations']
+
+        return self._format(
+            self._common_eva_pipeline_properties(opencga_path, read_preference),
+            {
             'annotation.overwrite': False,
+            'app.vep.cache.path': vep_cache_path,
             'app.vep.num-forks': 4,
             'app.vep.timeout': 500,
             'config.chunk.size': 200,
-            'config.restartability.allow': 'false',
-            'config.db.read-preference': read_preference,
-            'db.collections.files.name': files_collection,
+
             'db.collections.variants.name': variants_collection,
+            'db.collections.files.name': files_collection,
             'db.collections.annotation-metadata.name': annotation_metadata_collection,
             'db.collections.annotations.name': annotation_collection,
+
             'input.study.id': project_accession,
             'input.study.name': study_name,
             'input.study.type': 'COLLECTION',
-            'logging.level.embl.ebi.variation.eva': 'DEBUG',
-            'logging.level.org.opencb.opencga': 'DEBUG',
-            'logging.level.org.springframework': 'INFO',
+
             'output.dir': str(output_dir),
             'output.dir.annotation': str(annotation_dir),
             'output.dir.statistics': str(stats_dir),
-            'spring.main.allow-bean-definition-overriding': 'true',
+
             'spring.jpa.database-platform': 'org.hibernate.dialect.PostgreSQL9Dialect',
             'spring.jpa.properties.hibernate.jdbc.lob.non_contextual_creation': True,
             'spring.jpa.properties.hibernate.temp.use_jdbc_metadata_defaults': False,
             'statistics.skip': False
         },
     )
```

### Comparing `ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/taxonomy/taxonomy.py` & `ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/taxonomy/taxonomy.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/variation/assembly_utils.py` & `ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/variation/assembly_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils/variation/contig_utils.py` & `ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils/variation/contig_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils.egg-info/PKG-INFO` & `ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebi-eva-common-pyutils
-Version: 0.5.3.dev1
+Version: 0.5.3.dev2
 Summary: EBI EVA - Common Python Utilities
 Home-page: https://github.com/EBIVariation/eva-common-pyutils
 License: Apache
 Keywords: EBI,EVA,PYTHON,UTILITIES
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `ebi_eva_common_pyutils-0.5.3.dev1/ebi_eva_common_pyutils.egg-info/SOURCES.txt` & `ebi_eva_common_pyutils-0.5.3.dev2/ebi_eva_common_pyutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev1/setup.py` & `ebi_eva_common_pyutils-0.5.3.dev2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from setuptools import find_packages
 
 setup(
     name='ebi_eva_common_pyutils',
     scripts=[os.path.join(os.path.dirname(__file__), 'ebi_eva_common_pyutils', 'archive_directory.py')],
     packages=find_packages(),
-    version='0.5.3-dev1',
+    version='0.5.3-dev2',
     license='Apache',
     description='EBI EVA - Common Python Utilities',
     url='https://github.com/EBIVariation/eva-common-pyutils',
     keywords=['EBI', 'EVA', 'PYTHON', 'UTILITIES'],
     install_requires=['psycopg2-binary', 'requests', 'pymongo', 'lxml', 'pyyaml', 'cached-property', 'retry',
                       'networkx<=2.5'],
     classifiers=[
```

