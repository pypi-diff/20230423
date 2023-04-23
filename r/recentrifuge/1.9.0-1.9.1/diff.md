# Comparing `tmp/recentrifuge-1.9.0.tar.gz` & `tmp/recentrifuge-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recentrifuge-1.9.0.tar", last modified: Thu Jun  9 08:21:58 2022, max compression
+gzip compressed data, was "recentrifuge-1.9.1.tar", last modified: Sat Jun 25 21:18:28 2022, max compression
```

## Comparing `recentrifuge-1.9.0.tar` & `recentrifuge-1.9.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 martijm    (501) staff       (20)        0 2022-06-09 08:21:58.161211 recentrifuge-1.9.0/
--rw-r--r--   0 martijm    (501) staff       (20)      110 2019-01-21 11:02:50.000000 recentrifuge-1.9.0/MANIFEST.in
--rw-r--r--   0 martijm    (501) staff       (20)     3664 2022-06-09 08:21:58.160887 recentrifuge-1.9.0/PKG-INFO
--rw-r--r--   0 martijm    (501) staff       (20)     5585 2022-06-09 07:55:41.000000 recentrifuge-1.9.0/README.md
--rwxr-xr-x   0 martijm    (501) staff       (20)    40416 2022-03-27 22:40:24.000000 recentrifuge-1.9.0/rcf
-drwxr-xr-x   0 martijm    (501) staff       (20)        0 2022-06-09 08:21:58.143055 recentrifuge-1.9.0/recentrifuge/
--rw-r--r--   0 martijm    (501) staff       (20)     2380 2022-06-09 07:54:15.000000 recentrifuge-1.9.0/recentrifuge/__init__.py
--rw-r--r--   0 martijm    (501) staff       (20)     9080 2022-03-09 20:13:24.000000 recentrifuge-1.9.0/recentrifuge/centrifuge.py
--rw-rw-rw-   0 martijm    (501) staff       (20)     3500 2021-02-10 23:33:54.000000 recentrifuge-1.9.0/recentrifuge/centrifuge_io.py
--rw-r--r--   0 martijm    (501) staff       (20)    10086 2022-03-09 20:13:24.000000 recentrifuge-1.9.0/recentrifuge/clark.py
--rw-r--r--   0 martijm    (501) staff       (20)     5403 2022-03-27 22:19:05.000000 recentrifuge-1.9.0/recentrifuge/config.py
--rw-r--r--   0 martijm    (501) staff       (20)    24115 2020-12-14 00:13:46.000000 recentrifuge-1.9.0/recentrifuge/core.py
--rw-r--r--   0 martijm    (501) staff       (20)     1940 2020-12-14 03:01:28.000000 recentrifuge-1.9.0/recentrifuge/fastq_io.py
--rw-r--r--   0 martijm    (501) staff       (20)    11908 2022-03-09 20:13:24.000000 recentrifuge-1.9.0/recentrifuge/generic.py
-drwxr-xr-x   0 martijm    (501) staff       (20)        0 2022-06-09 08:21:58.147333 recentrifuge-1.9.0/recentrifuge/img/
--rw-r--r--   0 martijm    (501) staff       (20)    10541 2017-08-01 22:12:03.000000 recentrifuge-1.9.0/recentrifuge/img/favicon.uri
--rw-r--r--   0 martijm    (501) staff       (20)      622 2017-08-01 22:12:03.000000 recentrifuge-1.9.0/recentrifuge/img/hidden.uri
--rw-r--r--   0 martijm    (501) staff       (20)      922 2017-08-01 22:12:03.000000 recentrifuge-1.9.0/recentrifuge/img/loading.uri
--rw-r--r--   0 martijm    (501) staff       (20)    12919 2018-06-27 06:19:40.000000 recentrifuge-1.9.0/recentrifuge/img/logo-rcf-mini.uri
--rw-r--r--   0 martijm    (501) staff       (20)     9924 2022-03-09 20:13:24.000000 recentrifuge-1.9.0/recentrifuge/kraken.py
--rw-r--r--   0 martijm    (501) staff       (20)   202031 2022-01-02 21:14:55.000000 recentrifuge-1.9.0/recentrifuge/krona.js
--rw-r--r--   0 martijm    (501) staff       (20)    15435 2022-03-09 20:13:24.000000 recentrifuge-1.9.0/recentrifuge/krona.py
--rw-r--r--   0 martijm    (501) staff       (20)     8497 2022-03-09 20:13:24.000000 recentrifuge-1.9.0/recentrifuge/lmat.py
--rw-r--r--   0 martijm    (501) staff       (20)     5590 2020-12-14 00:13:46.000000 recentrifuge-1.9.0/recentrifuge/lmat_io.py
--rw-r--r--   0 martijm    (501) staff       (20)     8090 2022-03-24 06:27:27.000000 recentrifuge-1.9.0/recentrifuge/mock.py
--rw-r--r--   0 martijm    (501) staff       (20)     1344 2019-01-21 11:02:50.000000 recentrifuge-1.9.0/recentrifuge/ontology.py
--rw-r--r--   0 martijm    (501) staff       (20)      714 2018-11-19 09:18:35.000000 recentrifuge-1.9.0/recentrifuge/params.py
--rw-r--r--   0 martijm    (501) staff       (20)     7431 2022-03-10 09:20:57.000000 recentrifuge-1.9.0/recentrifuge/rank.py
--rw-r--r--   0 martijm    (501) staff       (20)     3433 2019-01-21 11:02:50.000000 recentrifuge-1.9.0/recentrifuge/shared_counter.py
--rw-r--r--   0 martijm    (501) staff       (20)     7042 2020-12-14 00:13:36.000000 recentrifuge-1.9.0/recentrifuge/stats.py
--rw-r--r--   0 martijm    (501) staff       (20)     9039 2022-03-23 19:22:23.000000 recentrifuge-1.9.0/recentrifuge/taxclass.py
--rw-r--r--   0 martijm    (501) staff       (20)    11991 2022-03-21 19:35:40.000000 recentrifuge-1.9.0/recentrifuge/taxonomy.py
-drwxr-xr-x   0 martijm    (501) staff       (20)        0 2022-06-09 08:21:58.160239 recentrifuge-1.9.0/recentrifuge/test/
--rw-------   0 martijm    (501) staff       (20)   478749 2022-06-09 04:54:48.000000 recentrifuge-1.9.0/recentrifuge/test/TEST.rcf.xlsx
--rw-r--r--   0 martijm    (501) staff       (20)      330 2019-01-21 11:02:50.000000 recentrifuge-1.9.0/recentrifuge/test/ctrl1.mck
--rw-r--r--   0 martijm    (501) staff       (20)      324 2019-01-21 11:02:50.000000 recentrifuge-1.9.0/recentrifuge/test/ctrl2.mck
--rw-r--r--   0 martijm    (501) staff       (20)      352 2019-01-21 11:02:50.000000 recentrifuge-1.9.0/recentrifuge/test/ctrl3.mck
--rw-r--r--   0 martijm    (501) staff       (20)    40224 2022-03-08 23:53:47.000000 recentrifuge-1.9.0/recentrifuge/test/mock.xlsx
--rw-r--r--   0 martijm    (501) staff       (20)   361907 2019-03-06 17:25:16.000000 recentrifuge-1.9.0/recentrifuge/test/myTEST.rcf.xlsx
--rw-r--r--   0 martijm    (501) staff       (20)      357 2019-01-21 11:02:50.000000 recentrifuge-1.9.0/recentrifuge/test/smpl1.mck
--rw-r--r--   0 martijm    (501) staff       (20)      581 2019-01-21 11:02:50.000000 recentrifuge-1.9.0/recentrifuge/test/smpl2.mck
--rw-r--r--   0 martijm    (501) staff       (20)      560 2019-01-21 11:02:50.000000 recentrifuge-1.9.0/recentrifuge/test/smpl3.mck
--rw-r--r--   0 martijm    (501) staff       (20)    36452 2022-03-12 23:45:28.000000 recentrifuge-1.9.0/recentrifuge/trees.py
-drwxr-xr-x   0 martijm    (501) staff       (20)        0 2022-06-09 08:21:58.145316 recentrifuge-1.9.0/recentrifuge.egg-info/
--rw-r--r--   0 martijm    (501) staff       (20)     3664 2022-06-09 08:21:58.000000 recentrifuge-1.9.0/recentrifuge.egg-info/PKG-INFO
--rw-r--r--   0 martijm    (501) staff       (20)     1163 2022-06-09 08:21:58.000000 recentrifuge-1.9.0/recentrifuge.egg-info/SOURCES.txt
--rw-r--r--   0 martijm    (501) staff       (20)        1 2022-06-09 08:21:58.000000 recentrifuge-1.9.0/recentrifuge.egg-info/dependency_links.txt
--rw-r--r--   0 martijm    (501) staff       (20)       10 2022-06-09 08:21:58.000000 recentrifuge-1.9.0/recentrifuge.egg-info/requires.txt
--rw-r--r--   0 martijm    (501) staff       (20)       13 2022-06-09 08:21:58.000000 recentrifuge-1.9.0/recentrifuge.egg-info/top_level.txt
--rwxr-xr-x   0 martijm    (501) staff       (20)     6456 2022-06-09 07:54:15.000000 recentrifuge-1.9.0/refasplit
--rwxr-xr-x   0 martijm    (501) staff       (20)     5258 2022-03-23 22:08:54.000000 recentrifuge-1.9.0/remock
--rwxr-xr-x   0 martijm    (501) staff       (20)     4627 2022-01-02 21:14:55.000000 recentrifuge-1.9.0/retaxdump
--rwxr-xr-x   0 martijm    (501) staff       (20)    35077 2022-03-24 07:27:16.000000 recentrifuge-1.9.0/retest
--rwxr-xr-x   0 martijm    (501) staff       (20)    16729 2022-03-26 02:10:09.000000 recentrifuge-1.9.0/rextract
--rw-r--r--   0 martijm    (501) staff       (20)       38 2022-06-09 08:21:58.161312 recentrifuge-1.9.0/setup.cfg
--rw-r--r--   0 martijm    (501) staff       (20)     3855 2022-06-09 07:58:40.000000 recentrifuge-1.9.0/setup.py
+drwxr-xr-x   0 martijm    (501) staff       (20)        0 2022-06-25 21:18:28.036857 recentrifuge-1.9.1/
+-rw-r--r--   0 martijm    (501) staff       (20)      110 2019-01-21 11:02:50.000000 recentrifuge-1.9.1/MANIFEST.in
+-rw-r--r--   0 martijm    (501) staff       (20)     3664 2022-06-25 21:18:28.036555 recentrifuge-1.9.1/PKG-INFO
+-rw-r--r--   0 martijm    (501) staff       (20)     5585 2022-06-25 17:42:41.000000 recentrifuge-1.9.1/README.md
+-rwxr-xr-x   0 martijm    (501) staff       (20)    40416 2022-03-27 22:40:24.000000 recentrifuge-1.9.1/rcf
+drwxr-xr-x   0 martijm    (501) staff       (20)        0 2022-06-25 21:18:28.019870 recentrifuge-1.9.1/recentrifuge/
+-rw-r--r--   0 martijm    (501) staff       (20)     2380 2022-06-25 17:42:41.000000 recentrifuge-1.9.1/recentrifuge/__init__.py
+-rw-r--r--   0 martijm    (501) staff       (20)     9080 2022-03-09 20:13:24.000000 recentrifuge-1.9.1/recentrifuge/centrifuge.py
+-rw-rw-rw-   0 martijm    (501) staff       (20)     3500 2021-02-10 23:33:54.000000 recentrifuge-1.9.1/recentrifuge/centrifuge_io.py
+-rw-r--r--   0 martijm    (501) staff       (20)    10086 2022-03-09 20:13:24.000000 recentrifuge-1.9.1/recentrifuge/clark.py
+-rw-r--r--   0 martijm    (501) staff       (20)     5403 2022-03-27 22:19:05.000000 recentrifuge-1.9.1/recentrifuge/config.py
+-rw-r--r--   0 martijm    (501) staff       (20)    24115 2020-12-14 00:13:46.000000 recentrifuge-1.9.1/recentrifuge/core.py
+-rw-r--r--   0 martijm    (501) staff       (20)     1940 2020-12-14 03:01:28.000000 recentrifuge-1.9.1/recentrifuge/fastq_io.py
+-rw-r--r--   0 martijm    (501) staff       (20)    11908 2022-03-09 20:13:24.000000 recentrifuge-1.9.1/recentrifuge/generic.py
+drwxr-xr-x   0 martijm    (501) staff       (20)        0 2022-06-25 21:18:28.024373 recentrifuge-1.9.1/recentrifuge/img/
+-rw-r--r--   0 martijm    (501) staff       (20)    10541 2017-08-01 22:12:03.000000 recentrifuge-1.9.1/recentrifuge/img/favicon.uri
+-rw-r--r--   0 martijm    (501) staff       (20)      622 2017-08-01 22:12:03.000000 recentrifuge-1.9.1/recentrifuge/img/hidden.uri
+-rw-r--r--   0 martijm    (501) staff       (20)      922 2017-08-01 22:12:03.000000 recentrifuge-1.9.1/recentrifuge/img/loading.uri
+-rw-r--r--   0 martijm    (501) staff       (20)    12919 2018-06-27 06:19:40.000000 recentrifuge-1.9.1/recentrifuge/img/logo-rcf-mini.uri
+-rw-r--r--   0 martijm    (501) staff       (20)     9924 2022-03-09 20:13:24.000000 recentrifuge-1.9.1/recentrifuge/kraken.py
+-rw-r--r--   0 martijm    (501) staff       (20)   202031 2022-01-02 21:14:55.000000 recentrifuge-1.9.1/recentrifuge/krona.js
+-rw-r--r--   0 martijm    (501) staff       (20)    15435 2022-03-09 20:13:24.000000 recentrifuge-1.9.1/recentrifuge/krona.py
+-rw-r--r--   0 martijm    (501) staff       (20)     8497 2022-03-09 20:13:24.000000 recentrifuge-1.9.1/recentrifuge/lmat.py
+-rw-r--r--   0 martijm    (501) staff       (20)     5590 2020-12-14 00:13:46.000000 recentrifuge-1.9.1/recentrifuge/lmat_io.py
+-rw-r--r--   0 martijm    (501) staff       (20)     8090 2022-03-24 06:27:27.000000 recentrifuge-1.9.1/recentrifuge/mock.py
+-rw-r--r--   0 martijm    (501) staff       (20)     1344 2019-01-21 11:02:50.000000 recentrifuge-1.9.1/recentrifuge/ontology.py
+-rw-r--r--   0 martijm    (501) staff       (20)      714 2018-11-19 09:18:35.000000 recentrifuge-1.9.1/recentrifuge/params.py
+-rw-r--r--   0 martijm    (501) staff       (20)     7431 2022-03-10 09:20:57.000000 recentrifuge-1.9.1/recentrifuge/rank.py
+-rw-r--r--   0 martijm    (501) staff       (20)     3433 2019-01-21 11:02:50.000000 recentrifuge-1.9.1/recentrifuge/shared_counter.py
+-rw-r--r--   0 martijm    (501) staff       (20)     7042 2020-12-14 00:13:36.000000 recentrifuge-1.9.1/recentrifuge/stats.py
+-rw-r--r--   0 martijm    (501) staff       (20)     9039 2022-03-23 19:22:23.000000 recentrifuge-1.9.1/recentrifuge/taxclass.py
+-rw-r--r--   0 martijm    (501) staff       (20)    11991 2022-03-21 19:35:40.000000 recentrifuge-1.9.1/recentrifuge/taxonomy.py
+drwxr-xr-x   0 martijm    (501) staff       (20)        0 2022-06-25 21:18:28.035842 recentrifuge-1.9.1/recentrifuge/test/
+-rw-------   0 martijm    (501) staff       (20)   478749 2022-06-09 04:54:48.000000 recentrifuge-1.9.1/recentrifuge/test/TEST.rcf.xlsx
+-rw-r--r--   0 martijm    (501) staff       (20)      330 2019-01-21 11:02:50.000000 recentrifuge-1.9.1/recentrifuge/test/ctrl1.mck
+-rw-r--r--   0 martijm    (501) staff       (20)      324 2019-01-21 11:02:50.000000 recentrifuge-1.9.1/recentrifuge/test/ctrl2.mck
+-rw-r--r--   0 martijm    (501) staff       (20)      352 2019-01-21 11:02:50.000000 recentrifuge-1.9.1/recentrifuge/test/ctrl3.mck
+-rw-r--r--   0 martijm    (501) staff       (20)    40224 2022-03-08 23:53:47.000000 recentrifuge-1.9.1/recentrifuge/test/mock.xlsx
+-rw-r--r--   0 martijm    (501) staff       (20)   361907 2019-03-06 17:25:16.000000 recentrifuge-1.9.1/recentrifuge/test/myTEST.rcf.xlsx
+-rw-r--r--   0 martijm    (501) staff       (20)      357 2019-01-21 11:02:50.000000 recentrifuge-1.9.1/recentrifuge/test/smpl1.mck
+-rw-r--r--   0 martijm    (501) staff       (20)      581 2019-01-21 11:02:50.000000 recentrifuge-1.9.1/recentrifuge/test/smpl2.mck
+-rw-r--r--   0 martijm    (501) staff       (20)      560 2019-01-21 11:02:50.000000 recentrifuge-1.9.1/recentrifuge/test/smpl3.mck
+-rw-r--r--   0 martijm    (501) staff       (20)    36452 2022-03-12 23:45:28.000000 recentrifuge-1.9.1/recentrifuge/trees.py
+drwxr-xr-x   0 martijm    (501) staff       (20)        0 2022-06-25 21:18:28.022316 recentrifuge-1.9.1/recentrifuge.egg-info/
+-rw-r--r--   0 martijm    (501) staff       (20)     3664 2022-06-25 21:18:27.000000 recentrifuge-1.9.1/recentrifuge.egg-info/PKG-INFO
+-rw-r--r--   0 martijm    (501) staff       (20)     1163 2022-06-25 21:18:27.000000 recentrifuge-1.9.1/recentrifuge.egg-info/SOURCES.txt
+-rw-r--r--   0 martijm    (501) staff       (20)        1 2022-06-25 21:18:27.000000 recentrifuge-1.9.1/recentrifuge.egg-info/dependency_links.txt
+-rw-r--r--   0 martijm    (501) staff       (20)       10 2022-06-25 21:18:27.000000 recentrifuge-1.9.1/recentrifuge.egg-info/requires.txt
+-rw-r--r--   0 martijm    (501) staff       (20)       13 2022-06-25 21:18:27.000000 recentrifuge-1.9.1/recentrifuge.egg-info/top_level.txt
+-rwxr-xr-x   0 martijm    (501) staff       (20)     6453 2022-06-25 17:40:50.000000 recentrifuge-1.9.1/refasplit
+-rwxr-xr-x   0 martijm    (501) staff       (20)     5258 2022-03-23 22:08:54.000000 recentrifuge-1.9.1/remock
+-rwxr-xr-x   0 martijm    (501) staff       (20)     4627 2022-01-02 21:14:55.000000 recentrifuge-1.9.1/retaxdump
+-rwxr-xr-x   0 martijm    (501) staff       (20)    35077 2022-03-24 07:27:16.000000 recentrifuge-1.9.1/retest
+-rwxr-xr-x   0 martijm    (501) staff       (20)    16729 2022-03-26 02:10:09.000000 recentrifuge-1.9.1/rextract
+-rw-r--r--   0 martijm    (501) staff       (20)       38 2022-06-25 21:18:28.036949 recentrifuge-1.9.1/setup.cfg
+-rw-r--r--   0 martijm    (501) staff       (20)     3855 2022-06-25 17:42:41.000000 recentrifuge-1.9.1/setup.py
```

### Comparing `recentrifuge-1.9.0/PKG-INFO` & `recentrifuge-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recentrifuge
-Version: 1.9.0
+Version: 1.9.1
 Summary: Robust comparative analysis and contamination removal for metagenomics
 Home-page: http://www.recentrifuge.org
 Author: Jose Manuel Martí
 Author-email: jse.mnl@gmail.com
 License: AGPL except krona.js, with its own license by BNBI
 Project-URL: Documentation, https://github.com/khyox/recentrifuge/wiki
 Project-URL: Source, https://github.com/khyox/recentrifuge
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: recentrifuge Version: 1.9.0 Summary: Robust
+Metadata-Version: 2.1 Name: recentrifuge Version: 1.9.1 Summary: Robust
 comparative analysis and contamination removal for metagenomics Home-page:
 http://www.recentrifuge.org Author: Jose Manuel MartÃ­ Author-email:
 jse.mnl@gmail.com License: AGPL except krona.js, with its own license by BNBI
 Project-URL: Documentation, https://github.com/khyox/recentrifuge/wiki Project-
 URL: Source, https://github.com/khyox/recentrifuge Project-URL: Tracker, https:
 //github.com/khyox/recentrifuge/issues Description: **Robust comparative
 analysis and contamination removal for metagenomics** [![Retest](https://
```

### Comparing `recentrifuge-1.9.0/README.md` & `recentrifuge-1.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <p align="center"><a href="http://www.recentrifuge.org" target="_blank">
 <img src="https://raw.githubusercontent.com/khyox/rcf-aux/master/RCFheader.png" alt="Recentrifuge" width="900px"/></a></p><hr>
 <p align="center"><b>Robust comparative analysis and contamination removal for metagenomics</b>
 </p> 
 
 
 ____
-[![Retest](https://github.com/khyox/Recentrifuge/actions/workflows/retest.yaml/badge.svg?branch=v1.9.0)](https://github.com/khyox/recentrifuge/actions/workflows/retest.yaml)
+[![Retest](https://github.com/khyox/Recentrifuge/actions/workflows/retest.yaml/badge.svg?branch=v1.9.1)](https://github.com/khyox/recentrifuge/actions/workflows/retest.yaml)
 [![](https://img.shields.io/maintenance/yes/2022.svg)](http://www.recentrifuge.org)
 [![](https://img.shields.io/github/languages/top/khyox/recentrifuge.svg)](https://pypi.org/project/recentrifuge/)
 [![](https://img.shields.io/pypi/pyversions/recentrifuge.svg)](https://pypi.org/project/recentrifuge/)
 [![](https://img.shields.io/pypi/v/recentrifuge.svg)](https://pypi.org/project/recentrifuge/)
 [![](https://img.shields.io/pypi/wheel/recentrifuge.svg)](https://pypi.org/project/recentrifuge/)
 [![Anaconda-Server Badge](https://anaconda.org/bioconda/recentrifuge/badges/version.svg)](https://anaconda.org/bioconda/recentrifuge)
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
                                 [Recentrifuge]
 ===============================================================================
     Robust comparative analysis and contamination removal for metagenomics
 ____ [![Retest](https://github.com/khyox/Recentrifuge/actions/workflows/
-retest.yaml/badge.svg?branch=v1.9.0)](https://github.com/khyox/recentrifuge/
+retest.yaml/badge.svg?branch=v1.9.1)](https://github.com/khyox/recentrifuge/
 actions/workflows/retest.yaml) [![](https://img.shields.io/maintenance/yes/
 2022.svg)](http://www.recentrifuge.org) [![](https://img.shields.io/github/
 languages/top/khyox/recentrifuge.svg)](https://pypi.org/project/recentrifuge/)
 [![](https://img.shields.io/pypi/pyversions/recentrifuge.svg)](https://
 pypi.org/project/recentrifuge/) [![](https://img.shields.io/pypi/v/
 recentrifuge.svg)](https://pypi.org/project/recentrifuge/) [![](https://
 img.shields.io/pypi/wheel/recentrifuge.svg)](https://pypi.org/project/
```

### Comparing `recentrifuge-1.9.0/rcf` & `recentrifuge-1.9.1/rcf`

 * *Files identical despite different names*

### Comparing `recentrifuge-1.9.0/recentrifuge/__init__.py` & `recentrifuge-1.9.1/recentrifuge/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 __author__ = 'Jose Manuel Martí'
 __copyright__ = 'Copyright (C) 2017–2022 Jose Manuel Martí Martínez'
 __license__ = 'GNU Affero General Public License Version 3'
 __email__ = 'jse.mnl **AT** gmail.com'
 __maintainer__ = 'Jose Manuel Martí'
 __status__ = 'Production/Stable'
 __date__ = 'Jun 2022'
-__version__ = '1.9.0'
+__version__ = '1.9.1'
 
 import sys
 from Bio import SeqIO
 from . import lmat_io  # LMAT support
 from . import centrifuge_io  # Centrifuge support
 from . import fastq_io  # Quick FASTQ support
```

### Comparing `recentrifuge-1.9.0/recentrifuge/centrifuge.py` & `recentrifuge-1.9.1/recentrifuge/centrifuge.py`

 * *Files identical despite different names*

### Comparing `recentrifuge-1.9.0/recentrifuge/centrifuge_io.py` & `recentrifuge-1.9.1/recentrifuge/centrifuge_io.py`

 * *Files identical despite different names*

### Comparing `recentrifuge-1.9.0/recentrifuge/clark.py` & `recentrifuge-1.9.1/recentrifuge/clark.py`

 * *Files identical despite different names*

### Comparing `recentrifuge-1.9.0/recentrifuge/config.py` & `recentrifuge-1.9.1/recentrifuge/config.py`

 * *Files identical despite different names*

### Comparing `recentrifuge-1.9.0/recentrifuge/core.py` & `recentrifuge-1.9.1/recentrifuge/core.py`

 * *Files identical despite different names*

### Comparing `recentrifuge-1.9.0/recentrifuge/fastq_io.py` & `recentrifuge-1.9.1/recentrifuge/fastq_io.py`

 * *Files identical despite different names*

### Comparing `recentrifuge-1.9.0/recentrifuge/generic.py` & `recentrifuge-1.9.1/recentrifuge/generic.py`

 * *Files identical despite different names*

### Comparing `recentrifuge-1.9.0/recentrifuge/img/favicon.uri` & `recentrifuge-1.9.1/recentrifuge/img/favicon.uri`

 * *Files identical despite different names*

### Comparing `recentrifuge-1.9.0/recentrifuge/img/hidden.uri` & `recentrifuge-1.9.1/recentrifuge/img/hidden.uri`

 * *Files identical despite different names*

### Comparing `recentrifuge-1.9.0/recentrifuge/img/loading.uri` & `recentrifuge-1.9.1/recentrifuge/img/loading.uri`

 * *Files identical despite different names*

### Comparing `recentrifuge-1.9.0/recentrifuge/img/logo-rcf-mini.uri` & `recentrifuge-1.9.1/recentrifuge/img/logo-rcf-mini.uri`

 * *Files identical despite different names*

### Comparing `recentrifuge-1.9.0/recentrifuge/kraken.py` & `recentrifuge-1.9.1/recentrifuge/kraken.py`

 * *Files identical despite different names*

### Comparing `recentrifuge-1.9.0/recentrifuge/krona.js` & `recentrifuge-1.9.1/recentrifuge/krona.js`

 * *Files identical despite different names*

### Comparing `recentrifuge-1.9.0/recentrifuge/krona.py` & `recentrifuge-1.9.1/recentrifuge/krona.py`

 * *Files identical despite different names*

### Comparing `recentrifuge-1.9.0/recentrifuge/lmat.py` & `recentrifuge-1.9.1/recentrifuge/lmat.py`

 * *Files identical despite different names*

### Comparing `recentrifuge-1.9.0/recentrifuge/lmat_io.py` & `recentrifuge-1.9.1/recentrifuge/lmat_io.py`

 * *Files identical despite different names*

### Comparing `recentrifuge-1.9.0/recentrifuge/mock.py` & `recentrifuge-1.9.1/recentrifuge/mock.py`

 * *Files identical despite different names*

### Comparing `recentrifuge-1.9.0/recentrifuge/ontology.py` & `recentrifuge-1.9.1/recentrifuge/ontology.py`

 * *Files identical despite different names*

### Comparing `recentrifuge-1.9.0/recentrifuge/params.py` & `recentrifuge-1.9.1/recentrifuge/params.py`

 * *Files identical despite different names*

### Comparing `recentrifuge-1.9.0/recentrifuge/rank.py` & `recentrifuge-1.9.1/recentrifuge/rank.py`

 * *Files identical despite different names*

### Comparing `recentrifuge-1.9.0/recentrifuge/shared_counter.py` & `recentrifuge-1.9.1/recentrifuge/shared_counter.py`

 * *Files identical despite different names*

### Comparing `recentrifuge-1.9.0/recentrifuge/stats.py` & `recentrifuge-1.9.1/recentrifuge/stats.py`

 * *Files identical despite different names*

### Comparing `recentrifuge-1.9.0/recentrifuge/taxclass.py` & `recentrifuge-1.9.1/recentrifuge/taxclass.py`

 * *Files identical despite different names*

### Comparing `recentrifuge-1.9.0/recentrifuge/taxonomy.py` & `recentrifuge-1.9.1/recentrifuge/taxonomy.py`

 * *Files identical despite different names*

### Comparing `recentrifuge-1.9.0/recentrifuge/test/TEST.rcf.xlsx` & `recentrifuge-1.9.1/recentrifuge/test/TEST.rcf.xlsx`

 * *Files identical despite different names*

### Comparing `recentrifuge-1.9.0/recentrifuge/test/mock.xlsx` & `recentrifuge-1.9.1/recentrifuge/test/mock.xlsx`

 * *Files identical despite different names*

### Comparing `recentrifuge-1.9.0/recentrifuge/test/myTEST.rcf.xlsx` & `recentrifuge-1.9.1/recentrifuge/test/myTEST.rcf.xlsx`

 * *Files identical despite different names*

### Comparing `recentrifuge-1.9.0/recentrifuge/test/smpl2.mck` & `recentrifuge-1.9.1/recentrifuge/test/smpl2.mck`

 * *Files identical despite different names*

### Comparing `recentrifuge-1.9.0/recentrifuge/test/smpl3.mck` & `recentrifuge-1.9.1/recentrifuge/test/smpl3.mck`

 * *Files identical despite different names*

### Comparing `recentrifuge-1.9.0/recentrifuge/trees.py` & `recentrifuge-1.9.1/recentrifuge/trees.py`

 * *Files identical despite different names*

### Comparing `recentrifuge-1.9.0/recentrifuge.egg-info/PKG-INFO` & `recentrifuge-1.9.1/recentrifuge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recentrifuge
-Version: 1.9.0
+Version: 1.9.1
 Summary: Robust comparative analysis and contamination removal for metagenomics
 Home-page: http://www.recentrifuge.org
 Author: Jose Manuel Martí
 Author-email: jse.mnl@gmail.com
 License: AGPL except krona.js, with its own license by BNBI
 Project-URL: Documentation, https://github.com/khyox/recentrifuge/wiki
 Project-URL: Source, https://github.com/khyox/recentrifuge
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: recentrifuge Version: 1.9.0 Summary: Robust
+Metadata-Version: 2.1 Name: recentrifuge Version: 1.9.1 Summary: Robust
 comparative analysis and contamination removal for metagenomics Home-page:
 http://www.recentrifuge.org Author: Jose Manuel MartÃ­ Author-email:
 jse.mnl@gmail.com License: AGPL except krona.js, with its own license by BNBI
 Project-URL: Documentation, https://github.com/khyox/recentrifuge/wiki Project-
 URL: Source, https://github.com/khyox/recentrifuge Project-URL: Tracker, https:
 //github.com/khyox/recentrifuge/issues Description: **Robust comparative
 analysis and contamination removal for metagenomics** [![Retest](https://
```

### Comparing `recentrifuge-1.9.0/recentrifuge.egg-info/SOURCES.txt` & `recentrifuge-1.9.1/recentrifuge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `recentrifuge-1.9.0/refasplit` & `recentrifuge-1.9.1/refasplit`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,15 @@
     else:
         handler = open
     nts: Counter[int] = collections.Counter()
     in_handler: Dict[str, TextIO] = {}
     omag: str = ceil(log10(num_files))  # Get order of magnitude ceil
     for n in range(num_files):
         key: str = f'{n:0>{omag}}'
-        in_handler[key] = handler(Filename(out_root + str(n) + fext), 'wt')
+        in_handler[key] = handler(Filename(out_root + key + fext), 'wt')
         nts[key] = 0  # Initialize counter so that most_common will work
 
     # Main loop: split FASTA file
     i: int = 0
     print(gray('Splitting FASTA file'), f'{in_fasta}', gray('...\nMseqs: '),
           end='')
     sys.stdout.flush()
```

### Comparing `recentrifuge-1.9.0/remock` & `recentrifuge-1.9.1/remock`

 * *Files identical despite different names*

### Comparing `recentrifuge-1.9.0/retaxdump` & `recentrifuge-1.9.1/retaxdump`

 * *Files identical despite different names*

### Comparing `recentrifuge-1.9.0/retest` & `recentrifuge-1.9.1/retest`

 * *Files identical despite different names*

### Comparing `recentrifuge-1.9.0/rextract` & `recentrifuge-1.9.1/rextract`

 * *Files identical despite different names*

### Comparing `recentrifuge-1.9.0/setup.py` & `recentrifuge-1.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='recentrifuge',
-    version='1.9.0',
+    version='1.9.1',
     packages=['recentrifuge'],
     url='http://www.recentrifuge.org',
     license='AGPL except krona.js, with its own license by BNBI',
     author='Jose Manuel Martí',
     author_email='jse.mnl@gmail.com',
     description='Robust comparative analysis and contamination removal for metagenomics',
     long_description="""
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-from setuptools import setup setup( name='recentrifuge', version='1.9.0',
+from setuptools import setup setup( name='recentrifuge', version='1.9.1',
 packages=['recentrifuge'], url='http://www.recentrifuge.org', license='AGPL
 except krona.js, with its own license by BNBI', author='Jose Manuel MartÃ­',
 author_email='jse.mnl@gmail.com', description='Robust comparative analysis and
 contamination removal for metagenomics', long_description=""" **Robust
 comparative analysis and contamination removal for metagenomics** [![Retest]
 (https://github.com/khyox/Recentrifuge/actions/workflows/retest.yaml/
 badge.svg?branch=v1.9.0)](https://github.com/khyox/recentrifuge/actions/
```

