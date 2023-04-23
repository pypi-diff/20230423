# Comparing `tmp/wwpdb.apps.chem_ref_data-0.19.tar.gz` & `tmp/wwpdb.apps.chem_ref_data-0.20.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.apps.chem_ref_data-0.19.tar", last modified: Fri Mar 17 20:26:54 2023, max compression
+gzip compressed data, was "wwpdb.apps.chem_ref_data-0.20.dev1.tar", last modified: Sun Apr 23 20:18:27 2023, max compression
```

## Comparing `wwpdb.apps.chem_ref_data-0.19.tar` & `wwpdb.apps.chem_ref_data-0.20.dev1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:26:54.986534 wwpdb.apps.chem_ref_data-0.19/
--rw-r--r--   0 vsts      (1001) docker     (123)      749 2023-03-17 20:26:54.986534 wwpdb.apps.chem_ref_data-0.19/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)       92 2023-03-17 20:25:44.000000 wwpdb.apps.chem_ref_data-0.19/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-03-17 20:26:54.986534 wwpdb.apps.chem_ref_data-0.19/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (123)     2528 2023-03-17 20:25:44.000000 wwpdb.apps.chem_ref_data-0.19/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:26:54.982534 wwpdb.apps.chem_ref_data-0.19/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-03-17 20:25:44.000000 wwpdb.apps.chem_ref_data-0.19/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:26:54.982534 wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-03-17 20:25:44.000000 wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:26:54.982534 wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/
--rw-r--r--   0 vsts      (1001) docker     (123)       57 2023-03-17 20:25:44.000000 wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)      150 2023-03-17 20:25:44.000000 wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:26:54.982534 wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/depict/
--rw-r--r--   0 vsts      (1001) docker     (123)     8619 2023-03-17 20:25:44.000000 wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/depict/ChemRefDataDepict.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4349 2023-03-17 20:25:44.000000 wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/depict/ChemRefDataDepictBootstrap.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-03-17 20:25:44.000000 wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/depict/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:26:54.982534 wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/io/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-03-17 20:25:44.000000 wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/io/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:26:54.982534 wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/report/
--rw-r--r--   0 vsts      (1001) docker     (123)     8147 2023-03-17 20:25:44.000000 wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/report/BirdReport.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5517 2023-03-17 20:25:44.000000 wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/report/ChemCompReport.py
--rw-r--r--   0 vsts      (1001) docker     (123)    26735 2023-03-17 20:25:44.000000 wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/report/ChemRefReportDepictBootstrap.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3626 2023-03-17 20:25:44.000000 wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/report/ReportUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-03-17 20:25:44.000000 wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/report/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:26:54.986534 wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/search/
--rw-r--r--   0 vsts      (1001) docker     (123)    19631 2023-03-17 20:25:44.000000 wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/search/ChemCompSearchIndexUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)      672 2023-03-17 20:25:44.000000 wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/search/ChemRefSearch.py
--rw-r--r--   0 vsts      (1001) docker     (123)    26652 2023-03-17 20:25:44.000000 wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/search/ChemRefSearchBase.py
--rw-r--r--   0 vsts      (1001) docker     (123)    27353 2023-03-17 20:25:44.000000 wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/search/ChemRefSearchDef.py
--rw-r--r--   0 vsts      (1001) docker     (123)    19563 2023-03-17 20:25:44.000000 wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/search/ChemRefSearchDepictBootstrap.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7816 2023-03-17 20:25:44.000000 wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/search/ChemRefSearchDuplicates.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2485 2023-03-17 20:25:44.000000 wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/search/MiscUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-03-17 20:25:44.000000 wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/search/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:26:54.986534 wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/utils/
--rw-r--r--   0 vsts      (1001) docker     (123)    18045 2023-03-17 20:25:44.000000 wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/utils/ChemRefDataCvsUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11314 2023-03-17 20:25:44.000000 wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/utils/ChemRefDataDbExec.py
--rw-r--r--   0 vsts      (1001) docker     (123)    16029 2023-03-17 20:25:44.000000 wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/utils/ChemRefDataDbUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    26207 2023-03-17 20:25:44.000000 wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/utils/ChemRefDataMiscUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3671 2023-03-17 20:25:44.000000 wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/utils/DownloadUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1111 2023-03-17 20:25:44.000000 wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/utils/OSVersion.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-03-17 20:25:44.000000 wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:26:54.986534 wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/webapp/
--rw-r--r--   0 vsts      (1001) docker     (123)    48578 2023-03-17 20:25:44.000000 wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/webapp/ChemRefDataWebApp.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-03-17 20:25:44.000000 wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/webapp/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:26:54.982534 wwpdb.apps.chem_ref_data-0.19/wwpdb.apps.chem_ref_data.egg-info/
--rw-rw-rw-   0 vsts      (1001) docker     (123)      749 2023-03-17 20:26:54.000000 wwpdb.apps.chem_ref_data-0.19/wwpdb.apps.chem_ref_data.egg-info/PKG-INFO
--rw-rw-rw-   0 vsts      (1001) docker     (123)     1749 2023-03-17 20:26:54.000000 wwpdb.apps.chem_ref_data-0.19/wwpdb.apps.chem_ref_data.egg-info/SOURCES.txt
--rw-rw-rw-   0 vsts      (1001) docker     (123)        1 2023-03-17 20:26:54.000000 wwpdb.apps.chem_ref_data-0.19/wwpdb.apps.chem_ref_data.egg-info/dependency_links.txt
--rw-rw-rw-   0 vsts      (1001) docker     (123)        1 2023-03-17 20:26:42.000000 wwpdb.apps.chem_ref_data-0.19/wwpdb.apps.chem_ref_data.egg-info/not-zip-safe
--rw-rw-rw-   0 vsts      (1001) docker     (123)      336 2023-03-17 20:26:54.000000 wwpdb.apps.chem_ref_data-0.19/wwpdb.apps.chem_ref_data.egg-info/requires.txt
--rw-rw-rw-   0 vsts      (1001) docker     (123)        6 2023-03-17 20:26:54.000000 wwpdb.apps.chem_ref_data-0.19/wwpdb.apps.chem_ref_data.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-23 20:18:27.749084 wwpdb.apps.chem_ref_data-0.20.dev1/
+-rw-r--r--   0 vsts      (1001) docker     (123)      754 2023-04-23 20:18:27.749084 wwpdb.apps.chem_ref_data-0.20.dev1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)       92 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-04-23 20:18:27.749084 wwpdb.apps.chem_ref_data-0.20.dev1/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     2528 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-23 20:18:27.741084 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-23 20:18:27.741084 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-23 20:18:27.741084 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/
+-rw-r--r--   0 vsts      (1001) docker     (123)       57 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)      155 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-23 20:18:27.741084 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/depict/
+-rw-r--r--   0 vsts      (1001) docker     (123)     8619 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/depict/ChemRefDataDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4349 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/depict/ChemRefDataDepictBootstrap.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/depict/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-23 20:18:27.741084 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/io/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/io/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-23 20:18:27.745084 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/report/
+-rw-r--r--   0 vsts      (1001) docker     (123)     8147 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/report/BirdReport.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5517 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/report/ChemCompReport.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    26735 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/report/ChemRefReportDepictBootstrap.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3626 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/report/ReportUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/report/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-23 20:18:27.745084 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/search/
+-rw-r--r--   0 vsts      (1001) docker     (123)    19650 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/search/ChemCompSearchIndexUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      672 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/search/ChemRefSearch.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    26652 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/search/ChemRefSearchBase.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    27353 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/search/ChemRefSearchDef.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    19563 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/search/ChemRefSearchDepictBootstrap.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7816 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/search/ChemRefSearchDuplicates.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2485 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/search/MiscUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/search/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-23 20:18:27.745084 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/utils/
+-rw-r--r--   0 vsts      (1001) docker     (123)    18237 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/utils/ChemRefDataCvsUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11314 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/utils/ChemRefDataDbExec.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    16203 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/utils/ChemRefDataDbUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    28016 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/utils/ChemRefDataMiscUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3671 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/utils/DownloadUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1111 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/utils/OSVersion.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-23 20:18:27.749084 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/webapp/
+-rw-r--r--   0 vsts      (1001) docker     (123)    48578 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/webapp/ChemRefDataWebApp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/webapp/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-23 20:18:27.741084 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb.apps.chem_ref_data.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      754 2023-04-23 20:18:27.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb.apps.chem_ref_data.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     1749 2023-04-23 20:18:27.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb.apps.chem_ref_data.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-23 20:18:27.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb.apps.chem_ref_data.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-23 20:18:09.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb.apps.chem_ref_data.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)      336 2023-04-23 20:18:27.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb.apps.chem_ref_data.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-04-23 20:18:27.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb.apps.chem_ref_data.egg-info/top_level.txt
```

### Comparing `wwpdb.apps.chem_ref_data-0.19/PKG-INFO` & `wwpdb.apps.chem_ref_data-0.20.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.chem_ref_data
-Version: 0.19
+Version: 0.20.dev1
 Summary: wwPDB chemical reference admin application
 Home-page: https://github.com/rcsb/py-wwpdb_apps_chem_ref_data
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.apps.chem_ref_data-0.19/setup.py` & `wwpdb.apps.chem_ref_data-0.20.dev1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,18 +38,18 @@
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
     ],
     #
     install_requires=[
-        "wwpdb.utils.config ~= 0.24",
+        "wwpdb.utils.config ~= 0.34",
         "wwpdb.utils.db ~= 0.26",
         "wwpdb.utils.session ~= 0.4",
-        "wwpdb.io ~= 0.25",
+        "wwpdb.io ~= 0.26",
         "mmcif.utils ~= 0.18",
         "wwpdb.utils.oe_util",
         "jellyfish ~= 0.6.1; python_version < '3'",
         "jellyfish; python_version >= '3'",
         "wwpdb.utils.cc_dict_util",
         "wwpdb.utils.dp ~= 0.19",
         "rcsb.utils.multiproc",
```

### Comparing `wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/depict/ChemRefDataDepict.py` & `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/depict/ChemRefDataDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/depict/ChemRefDataDepictBootstrap.py` & `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/depict/ChemRefDataDepictBootstrap.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/report/BirdReport.py` & `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/report/BirdReport.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/report/ChemCompReport.py` & `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/report/ChemCompReport.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/report/ChemRefReportDepictBootstrap.py` & `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/report/ChemRefReportDepictBootstrap.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/report/ReportUtils.py` & `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/report/ReportUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/search/ChemCompSearchIndexUtils.py` & `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/search/ChemCompSearchIndexUtils.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,29 +15,29 @@
 import sys
 import time
 
 import jellyfish
 from operator import itemgetter
 
 from wwpdb.utils.cc_dict_util.persist.PdbxChemCompDictIndex import PdbxChemCompDictIndex
-from wwpdb.utils.config.ConfigInfoApp import ConfigInfoAppCommon
+from wwpdb.utils.config.ConfigInfoApp import ConfigInfoAppCc
 
 import logging
 
 logger = logging.getLogger(__name__)
 
 
 class ChemCompSearchIndexUtils(object):
     def __init__(self, siteId, verbose=True, log=sys.stderr):
         self.__verbose = verbose
         self.__debug = False
         self.__lfh = log
         self.__siteId = siteId
-        self.__cICommon = ConfigInfoAppCommon(self.__siteId)
-        self.__pathCCIndex = self.__cICommon.get_cc_index()
+        self.__cIAppCc = ConfigInfoAppCc(self.__siteId)
+        self.__pathCCIndex = self.__cIAppCc.get_cc_index()
         logger.debug("ChemCompSearchIndexUtils index path %r", self.__pathCCIndex)
         #
         dIndx = PdbxChemCompDictIndex(verbose=self.__verbose, log=self.__lfh)
         self.__ccIndx = dIndx.readIndex(indexPath=self.__pathCCIndex)
 
     def getValue(self, ccId, key):
         try:
@@ -451,15 +451,15 @@
     def __editDistanceNormJF(self, s1, s2):
         """
         Compute the Normalized Damerau-Levenshtein distance between two given
         strings (s1 and s2)
         """
         try:
             maxLen = max(len(s1), len(s2))
-            ed = jellyfish.damerau_levenshtein_distance(s1, s2)
+            ed = jellyfish.damerau_levenshtein_distance(s1, s2)  # pylint: disable=no-member
             edN = float(maxLen - ed) / float(maxLen)
             # logging.debug("s1 %r s2 %r maxLen %r ed %f edN %f " % (s1, s2, maxLen, ed, edN))
             return edN
         except Exception as e:
             logger.exception("Edit distance norm s1 %r s2 %r %r", s1, s2, str(e))
         return 0
```

### Comparing `wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/search/ChemRefSearch.py` & `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/search/ChemRefSearch.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/search/ChemRefSearchBase.py` & `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/search/ChemRefSearchBase.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/search/ChemRefSearchDef.py` & `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/search/ChemRefSearchDef.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/search/ChemRefSearchDepictBootstrap.py` & `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/search/ChemRefSearchDepictBootstrap.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/search/ChemRefSearchDuplicates.py` & `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/search/ChemRefSearchDuplicates.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/search/MiscUtils.py` & `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/search/MiscUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/utils/ChemRefDataCvsUtils.py` & `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/utils/ChemRefDataCvsUtils.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,16 +55,16 @@
         self.__sObj = self.__reqObj.getSessionObj()
         self.__sessionPath = self.__sObj.getPath()
         # self.__sessionRelativePath = self.__sObj.getRelativePath()
         # self.__sessionId           = self.__sObj.getId()
         #
         self.__siteId = self.__reqObj.getValue("WWPDB_SITE_ID")
         self.__cI = ConfigInfo(self.__siteId)
-        self.__cICommonCc = ConfigInfoAppCc(self.__siteId)
-        self.__sbTopPath = self.__cICommonCc.get_site_refdata_top_cvs_sb_path()
+        self.__cIAppCc = ConfigInfoAppCc(self.__siteId)
+        self.__sbTopPath = self.__cIAppCc.get_site_refdata_top_cvs_sb_path()
         self.__pI = ChemRefPathInfo(siteId=self.__siteId, verbose=self.__verbose, log=self.__lfh)
         #
         self.__vc, self.__vcAd = self.__setupCvs()
         #
 
     def __setupCvs(self):
         #  Assign site specific chemical reference data CVS repository details --
@@ -184,14 +184,20 @@
         """Update the CVS repositories related to the chemical component dicitonary."""
         #
         startTime = time.time()
         #
         cvsProjectName = self.__pI.assignCvsProjectName(repType="CC")
         dataS = "ABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789"
         dataList = [(cvsProjectName, a, True) for a in dataS]
+
+        # Extended CCD support
+        ext_ccd = self.__cIAppCc.get_extended_ccd_supp()
+        if ext_ccd:
+            dataList += [("cvsProjectName", a + b, True) for a in dataS for b in dataS]
+
         #
         mpu = MultiProcUtil(verbose=self.__debug)
         mpu.set(workerObj=self.__vc, workerMethod="updateList")
         ok, failList, _resultList, diagList = mpu.runMulti(dataList=dataList, numProc=numProc)
         endTime = time.time()
         if self.__verbose:
             logger.info("+ChemRefDataCvsUtils(syncChemComp) CVS %s update status is: %r in %.2f seconds", cvsProjectName, ok, endTime - startTime)
```

### Comparing `wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/utils/ChemRefDataDbExec.py` & `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/utils/ChemRefDataDbExec.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/utils/ChemRefDataDbUtils.py` & `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/utils/ChemRefDataDbUtils.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 # try:
 #    from itertools import zip_longest
 # except ImportError:
 #    from itertools import izip_longest as zip_longest
 
 from wwpdb.utils.config.ConfigInfo import ConfigInfo
-from wwpdb.utils.config.ConfigInfoApp import ConfigInfoAppCommon
+from wwpdb.utils.config.ConfigInfoApp import ConfigInfoAppCc
 from wwpdb.utils.db.MyDbSqlGen import MyDbAdminSqlGen
 from wwpdb.utils.db.SchemaDefLoader import SchemaDefLoader
 from wwpdb.utils.db.MyDbUtil import MyDbQuery
 
 from rcsb.utils.multiproc.MultiProcPoolUtil import MultiProcPoolUtil
 from rcsb.utils.multiproc.MultiProcUtil import MultiProcUtil
 
@@ -86,28 +86,28 @@
         # self.__sessionId = self.__sObj.getId()
         #
 
         self.__ioObj = IoAdapterCore(verbose=self.__verbose, log=self.__lfh)
         #
         self.__siteId = self.__reqObj.getValue("WWPDB_SITE_ID")
         self.__cI = ConfigInfo(self.__siteId)
-        self.__cICommon = ConfigInfoAppCommon(self.__siteId)
-        self.__sbTopPath = self.__cICommon.get_site_refdata_top_cvs_sb_path()
+        self.__cIAppCc = ConfigInfoAppCc(self.__siteId)
+        self.__sbTopPath = self.__cIAppCc.get_site_refdata_top_cvs_sb_path()
         self.__projName = self.__cI.get("SITE_REFDATA_PROJ_NAME_CC")
 
     def loadBird(self):
         """Load database containing BIRD PRD and PRD Family data.  Materialized some sequence
         details prior to load.
         """
         startTime = time.time()
         logger.info("+ChemRefDataLoad(loadBird) Starting at %s", time.strftime("%Y %m %d %H:%M:%S", time.localtime()))
         try:
-            birdCachePath = self.__cICommon.get_site_prd_cvs_path()
-            birdCcCachePath = self.__cICommon.get_site_prdcc_cvs_path()
-            birdFamilyCachePath = self.__cICommon.get_site_family_cvs_path()
+            birdCachePath = self.__cIAppCc.get_site_prd_cvs_path()
+            birdCcCachePath = self.__cIAppCc.get_site_prdcc_cvs_path()
+            birdFamilyCachePath = self.__cIAppCc.get_site_family_cvs_path()
             #
             #
             prd = PdbxPrdIo(verbose=self.__verbose, log=self.__lfh)
             prd.setCachePath(birdCachePath)
             pathList = prd.makeDefinitionPathList()
             #
             for pth in pathList:
@@ -174,15 +174,15 @@
         logger.info("+ChemRefDataLoad(loadBird) Completed at %s (%.4f seconds)", time.strftime("%Y %m %d %H:%M:%S", time.localtime()), endTime - startTime)
         return ok
 
     def loadChemComp(self):
         startTime = time.time()
         logger.info("+ChemRefDataDbUtils(loadChemComp) Starting at %s", time.strftime("%Y %m %d %H:%M:%S", time.localtime()))
         try:
-            chemCompCachePath = self.__cICommon.get_site_cc_cvs_path()
+            chemCompCachePath = self.__cIAppCc.get_site_cc_cvs_path()
             #
             cc = PdbxChemCompIo(verbose=self.__verbose, log=self.__lfh)
             cc.setCachePath(chemCompCachePath)
             pathList = cc.makeComponentPathList()
             #
             for pth in pathList:
                 cc.setFilePath(pth)
@@ -273,14 +273,20 @@
         """Create batch load files for all chemical component definition data files - (multiprocessing for file generation only)"""
         if self.__verbose:
             logger.info("Starting")
         startTime = time.time()
         try:
             dataS = "ABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789"
             dataList = [a for a in dataS]
+
+            # Extended CCD support
+            ext_ccd = self.__cIAppCc.get_extended_ccd_supp()
+            if ext_ccd:
+                dataList += [a + b for a in dataS for b in dataS]
+
             if OSVersion().IsRhel8Like() is False:
                 mpu = MultiProcUtil(verbose=True)
                 mpu.set(workerObj=self, workerMethod="makeComponentPathListMulti")
                 ok, _failList, retLists, _diagList = mpu.runMulti(dataList=dataList, numProc=numProc, numResults=1)
             else:
                 mppu = MultiProcPoolUtil(verbose=True)
                 mppu.set(workerObj=self, workerMethod="makeComponentPathListMulti")
```

### Comparing `wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/utils/ChemRefDataMiscUtils.py` & `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/utils/ChemRefDataMiscUtils.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import time
 import scandir
 import filecmp
 import fnmatch
 import logging
 
 from wwpdb.utils.config.ConfigInfo import ConfigInfo
-from wwpdb.utils.config.ConfigInfoApp import ConfigInfoAppCommon
+from wwpdb.utils.config.ConfigInfoApp import ConfigInfoAppCc
 
 from rcsb.utils.multiproc.MultiProcUtil import MultiProcUtil
 
 from mmcif_utils.bird.PdbxPrdIo import PdbxPrdIo
 from mmcif_utils.bird.PdbxPrdCcIo import PdbxPrdCcIo
 from mmcif_utils.bird.PdbxFamilyIo import PdbxFamilyIo
 
@@ -64,57 +64,57 @@
         #
         self.__sObj = self.__reqObj.getSessionObj()
         self.__sessionPath = self.__sObj.getPath()
         #
 
         self.__siteId = self.__reqObj.getValue("WWPDB_SITE_ID")
         self.__cI = ConfigInfo(self.__siteId)
-        self.__cICommon = ConfigInfoAppCommon(self.__siteId)
-        self.__sbTopPath = self.__cICommon.get_site_refdata_top_cvs_sb_path()
+        self.__cIConfigInfoCc = ConfigInfoAppCc(self.__siteId)
+        self.__sbTopPath = self.__cIConfigInfoCc.get_site_refdata_top_cvs_sb_path()
         self.__projName = self.__cI.get("SITE_REFDATA_PROJ_NAME_CC")
-        self.__ccDictPath = self.__cICommon.get_site_cc_dict_path()
+        self.__ccDictPath = self.__cIConfigInfoCc.get_site_cc_dict_path()
         #
-        self.__pathCCDict = self.__cICommon.get_cc_dict()
-        self.__pathCCPathList = self.__cICommon.get_cc_path_list()
-        self.__pathCCIdList = self.__cICommon.get_cc_id_list()
-        self.__pathCCDictSerial = self.__cICommon.get_cc_dict_serial()
-        self.__pathCCDictIdx = self.__cICommon.get_cc_dict_idx()
+        self.__pathCCDict = self.__cIConfigInfoCc.get_cc_dict()
+        self.__pathCCPathList = self.__cIConfigInfoCc.get_cc_path_list()
+        self.__pathCCIdList = self.__cIConfigInfoCc.get_cc_id_list()
+        self.__pathCCDictSerial = self.__cIConfigInfoCc.get_cc_dict_serial()
+        self.__pathCCDictIdx = self.__cIConfigInfoCc.get_cc_dict_idx()
         #
         if sys.version_info[0] > 2:
-            self.__pathCCDb = self.__cICommon.get_cc_db()
+            self.__pathCCDb = self.__cIConfigInfoCc.get_cc_db()
         else:
             self.__pathCCDb = os.path.join(self.__ccDictPath, "chemcomp.db")
-        self.__pathCCIndex = self.__cICommon.get_cc_index()
-        self.__pathCCParentIndex = self.__cICommon.get_cc_parent_index()
+        self.__pathCCIndex = self.__cIConfigInfoCc.get_cc_index()
+        self.__pathCCParentIndex = self.__cIConfigInfoCc.get_cc_parent_index()
 
-        self.__pathPrdChemCompCVS = self.__cICommon.get_site_prdcc_cvs_path()
-        self.__pathPrdDictRef = self.__cICommon.get_site_prd_dict_path()
-        self.__pathPrdDictFile = self.__cICommon.get_prd_dict_file()
-        self.__pathPrdDictSerial = self.__cICommon.get_prd_dict_serial()
-        self.__pathPrdCcFile = self.__cICommon.get_prd_cc_file()
-        self.__pathPrdCcSerial = self.__cICommon.get_prd_cc_serial()
-        self.__pathPrdSummary = self.__cICommon.get_prd_summary_cif()
-        self.__pathPrdSummarySerial = self.__cICommon.get_prd_summary_sdb()
-        self.__pathPrdFamilyMapping = self.__cICommon.get_prd_family_mapping()
+        self.__pathPrdChemCompCVS = self.__cIConfigInfoCc.get_site_prdcc_cvs_path()
+        self.__pathPrdDictRef = self.__cIConfigInfoCc.get_site_prd_dict_path()
+        self.__pathPrdDictFile = self.__cIConfigInfoCc.get_prd_dict_file()
+        self.__pathPrdDictSerial = self.__cIConfigInfoCc.get_prd_dict_serial()
+        self.__pathPrdCcFile = self.__cIConfigInfoCc.get_prd_cc_file()
+        self.__pathPrdCcSerial = self.__cIConfigInfoCc.get_prd_cc_serial()
+        self.__pathPrdSummary = self.__cIConfigInfoCc.get_prd_summary_cif()
+        self.__pathPrdSummarySerial = self.__cIConfigInfoCc.get_prd_summary_sdb()
+        self.__pathPrdFamilyMapping = self.__cIConfigInfoCc.get_prd_family_mapping()
         #
         self.__makeTopPaths()
 
     def __makeTopPaths(self):
         for top_path in (self.__ccDictPath, self.__pathPrdDictRef, self.__pathPrdChemCompCVS):
             if not os.path.exists(top_path):
                 os.makedirs(top_path)
 
     def getBirdPathList(self):
         """Get pathlist for BIRD PRD and PRD Family data."""
         logger.info("+ChemRefDataLoad(getBirdPathList) Starting at %s", time.strftime("%Y %m %d %H:%M:%S", time.localtime()))
         try:
             #
-            birdCachePath = self.__cICommon.get_site_prd_cvs_path()
-            birdFamilyCachePath = self.__cICommon.get_site_family_cvs_path()
-            birdCcCachePath = self.__cICommon.get_site_prdcc_cvs_path()
+            birdCachePath = self.__cIConfigInfoCc.get_site_prd_cvs_path()
+            birdFamilyCachePath = self.__cIConfigInfoCc.get_site_family_cvs_path()
+            birdCcCachePath = self.__cIConfigInfoCc.get_site_prdcc_cvs_path()
             #
             #
             prd = PdbxPrdIo(verbose=self.__verbose, log=self.__lfh)
             prd.setCachePath(birdCachePath)
             pathList = prd.makeDefinitionPathList()
             #
             prdFam = PdbxFamilyIo(verbose=self.__verbose, log=self.__lfh)
@@ -128,14 +128,35 @@
             return pathList, familyPathList, prdCcPathList
         except:  # noqa: E722 pylint: disable=bare-except
             logger.exception("In getBirdPathList")
 
         logger.info("+ChemRefDataLoad(getBirdPathList) Completed at %s", time.strftime("%Y %m %d %H:%M:%S", time.localtime()))
         return [], [], []
 
+    def __atomicRename(self, srcPath, dstPath, suffix=".old"):
+        """Performs an atomic rename - while keeping the old file open to handle race conditions.
+        On NFS, if you have a file open on server B, and server A moves (atomically) a new file onto another, the
+        old file is unlinked by server.  Server B wlll then have a stale file handle for the already open file.
+
+        The solution here is to hardlink the old file to a tempoerary, and then atomically move new to old -- the old
+        inode is still valid until removed
+
+        srcPath and dstPath must be on the same filesyetem.
+        """
+
+        tempPath = dstPath + suffix
+
+        # Remove from previous round
+        if os.path.exists(tempPath):
+            os.remove(tempPath)
+
+        os.link(dstPath, tempPath)
+
+        os.rename(srcPath, dstPath)
+
     def __makeTempPath(self, inpPath):
         try:
             pid = str(os.getpid())
             return inpPath + pid
         except:  # noqa: E722 pylint: disable=bare-except
             return inpPath
 
@@ -215,16 +236,23 @@
     def updateChemCompPySupportFiles(self):
         """Create BSD DB of full chemical component dictionary, PRD CC files, index and parent index pickle files."""
         ok = False
         startTime = time.time()
         logger.info("Starting at %s", time.strftime("%Y %m %d %H:%M:%S", time.localtime()))
         try:
             dU = PdbxChemCompDictUtil(verbose=self.__verbose, log=self.__lfh)
+            logger.info("Starting full load at %s", time.strftime("%Y %m %d %H:%M:%S", time.localtime()))
+
             ok = dU.makeStoreFromFile(dictPath=self.__pathCCDict, storePath=self.__pathCCDb)
-            ok = self.updatePrdCCFiles()
+            logger.info("Finished full load at %s", time.strftime("%Y %m %d %H:%M:%S", time.localtime()))
+
+            # We skip the next - as it incrementally loads the CC definitions into database which is good for low memory machines
+            # but terribly slow
+            # ok = self.updatePrdCCFiles()
+            ok = True
             if ok:
                 dIndx = PdbxChemCompDictIndex(verbose=self.__verbose, log=self.__lfh)
                 dIndx.makeIndex(storePath=self.__pathCCDb, indexPath=self.__pathCCIndex)
                 _pD, _cD = dIndx.makeParentComponentIndex(storePath=self.__pathCCDb, indexPath=self.__pathCCParentIndex)
                 ok = True
             else:
                 ok = False
@@ -277,15 +305,17 @@
         logger.info("Starting at %s", time.strftime("%Y %m %d %H:%M:%S", time.localtime()))
         try:
             ccPathList = self.__getPathList(topPath=self.__pathPrdChemCompCVS, pattern="*.cif", excludeDirs=["CVS", "REMOVED", "FULL"])
             if self.__verbose:
                 logger.info("PRD CC pathlist length is %d", len(ccPathList))
             #
             dUtil = PdbxChemCompDictUtil(verbose=self.__verbose, log=self.__lfh)
+            logger.info("Starting incremental load at %s", time.strftime("%Y %m %d %H:%M:%S", time.localtime()))
             dUtil.updateStoreByFile(pathList=ccPathList, storePath=self.__pathCCDb)
+            logger.info("Finished incremental load at %s", time.strftime("%Y %m %d %H:%M:%S", time.localtime()))
             ok = True
             #
         except:  # noqa: E722 pylint: disable=bare-except
             logger.exception("updatePrdCCFiles")
 
         endTime = time.time()
         logger.info("Completed at %s (%d seconds)", time.strftime("%Y %m %d %H:%M:%S", time.localtime()), endTime - startTime)
@@ -305,15 +335,15 @@
             dp.imp(inpPath)
             dp.op("chem-comp-dict-makeindex")
             dp.expLog(logPath)
             dp.exp(outPathTmp)
             fSize = dp.expSize()
             if fSize > minSize:
                 os.chmod(outPathTmp, 0o664)
-                shutil.move(outPathTmp, self.__pathCCDictIdx)
+                self.__atomicRename(outPathTmp, self.__pathCCDictIdx)
                 os.chmod(self.__pathCCDictIdx, 0o664)
                 ok = True
             else:
                 ok = False
             if not self.__debug:
                 dp.cleanup()
             endTime0 = time.time()
@@ -322,15 +352,15 @@
             return ok
         except:  # noqa: E722 pylint: disable=bare-except
             logger.exception("Failure in __indexDictOp")
         return False
 
     def __serializeDictOp(self, minSize=10):
         """Serialize chemical component dictionary from concatenated dictionary text."""
-        logger.info("Starting %s %s")
+        logger.info("Starting")
         startTime = time.time()
         try:
             outPathTmp = self.__makeTempPath(self.__pathCCDictSerial)
             inpPath = self.__pathCCDict
             logPath = os.path.join(self.__ccDictPath, "chem-comp-dict-serialize.log")
             dp = RcsbDpUtility(tmpPath=self.__sessionPath, siteId=self.__siteId, verbose=self.__verbose)
             #
@@ -338,15 +368,15 @@
             dp.imp(inpPath)
             dp.op("chem-comp-dict-serialize")
             dp.expLog(logPath)
             dp.exp(outPathTmp)
             fSize = dp.expSize()
             if fSize > minSize:
                 os.chmod(outPathTmp, 0o664)
-                shutil.move(outPathTmp, self.__pathCCDictSerial)
+                self.__atomicRename(outPathTmp, self.__pathCCDictSerial)
                 os.chmod(self.__pathCCDictSerial, 0o664)
                 ok = True
             else:
                 ok = False
             if not self.__debug:
                 dp.cleanup()
             endTime0 = time.time()
@@ -357,15 +387,15 @@
             logger.exception("Failure in __serializeDictOp")
         return False
 
     def getChemCompPathList(self):
         startTime = time.time()
         logger.info("+ChemRefDataDbUtils(getChemCompPathList) Starting at %s", time.strftime("%Y %m %d %H:%M:%S", time.localtime()))
         try:
-            chemCompCachePath = self.__cICommon.get_site_cc_cvs_path()
+            chemCompCachePath = self.__cIConfigInfoCc.get_site_cc_cvs_path()
             #
             #
             cc = PdbxChemCompIo(verbose=self.__verbose, log=self.__lfh)
             cc.setCachePath(chemCompCachePath)
             pathList = cc.makeComponentPathList()
             endTime0 = time.time()
             if self.__verbose:
@@ -396,14 +426,20 @@
         """Return path list for all chemical component definition data files - (multiprocessing version)"""
         if self.__verbose:
             logger.info("Starting")
         startTime = time.time()
         try:
             dataS = "ABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789"
             dataList = [a for a in dataS]
+
+            # Extended CCD support
+            ext_ccd = self.__cIConfigInfoCc.get_extended_ccd_supp()
+            if ext_ccd:
+                dataList += [(a + b) for a in dataS for b in dataS]
+
             mpu = MultiProcUtil(verbose=True)
             mpu.set(workerObj=self, workerMethod="_makeComponentPathListMulti")
             _ok, _failList, retLists, _diagList = mpu.runMulti(dataList=dataList, numProc=numProc, numResults=1)
             pathList = retLists[0]
             endTime0 = time.time()
             if self.__verbose:
                 logger.info("Path list length %d  in %.2f seconds", len(pathList), endTime0 - startTime)
```

### Comparing `wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/utils/DownloadUtils.py` & `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/utils/DownloadUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/utils/OSVersion.py` & `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/utils/OSVersion.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.19/wwpdb/apps/chem_ref_data/webapp/ChemRefDataWebApp.py` & `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/webapp/ChemRefDataWebApp.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.19/wwpdb.apps.chem_ref_data.egg-info/SOURCES.txt` & `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb.apps.chem_ref_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

