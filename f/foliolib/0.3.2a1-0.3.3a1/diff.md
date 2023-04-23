# Comparing `tmp/foliolib-0.3.2a1.tar.gz` & `tmp/foliolib-0.3.3a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foliolib-0.3.2a1.tar", last modified: Sun Apr 16 05:35:39 2023, max compression
+gzip compressed data, was "foliolib-0.3.3a1.tar", last modified: Sun Apr 23 06:38:47 2023, max compression
```

## Comparing `foliolib-0.3.2a1.tar` & `foliolib-0.3.3a1.tar`

### file list

```diff
@@ -1,127 +1,128 @@
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-04-16 05:35:39.741968 foliolib-0.3.2a1/
--rw-r--r--   0 tobi      (1000) tobi      (1000)    35146 2020-10-11 07:41:52.000000 foliolib-0.3.2a1/COPYING
--rw-r--r--   0 tobi      (1000) tobi      (1000)       43 2020-11-07 12:13:21.000000 foliolib-0.3.2a1/MANIFEST.in
--rw-r--r--   0 tobi      (1000) tobi      (1000)     2357 2023-04-16 05:35:39.741968 foliolib-0.3.2a1/PKG-INFO
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1719 2023-02-21 11:23:02.000000 foliolib-0.3.2a1/README.rst
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-04-16 05:35:39.721968 foliolib-0.3.2a1/foliolib/
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1031 2023-03-24 13:25:47.000000 foliolib-0.3.2a1/foliolib/__init__.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      396 2023-04-16 05:35:39.000000 foliolib-0.3.2a1/foliolib/__version__.py
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-04-16 05:35:39.721968 foliolib-0.3.2a1/foliolib/apiBuilder/
--rw-r--r--   0 tobi      (1000) tobi      (1000)      351 2022-10-11 12:37:16.000000 foliolib-0.3.2a1/foliolib/apiBuilder/__init__.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1288 2022-03-13 04:11:25.000000 foliolib-0.3.2a1/foliolib/apiBuilder/build_api.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1586 2022-05-04 20:18:39.000000 foliolib-0.3.2a1/foliolib/apiBuilder/cli.py
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-04-16 05:35:39.725968 foliolib-0.3.2a1/foliolib/cli/
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3653 2023-03-30 06:15:34.000000 foliolib-0.3.2a1/foliolib/cli/__init__.py
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-04-16 05:35:39.725968 foliolib-0.3.2a1/foliolib/cli/folio/
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1461 2022-05-09 17:53:56.000000 foliolib-0.3.2a1/foliolib/cli/folio/__init__.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      229 2022-04-05 13:20:51.000000 foliolib-0.3.2a1/foliolib/cli/folio/inventory.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      634 2022-02-21 04:57:32.000000 foliolib-0.3.2a1/foliolib/cli/main.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      374 2022-02-21 04:57:41.000000 foliolib-0.3.2a1/foliolib/cli/main_err.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      895 2022-02-21 04:57:36.000000 foliolib-0.3.2a1/foliolib/cli/main_noauth.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     4591 2023-04-15 04:58:38.000000 foliolib-0.3.2a1/foliolib/cli/module.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3495 2023-04-01 07:43:09.000000 foliolib-0.3.2a1/foliolib/cli/okapi.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      446 2022-02-21 04:57:17.000000 foliolib-0.3.2a1/foliolib/cli/orderedGroup.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3680 2023-02-15 15:06:27.000000 foliolib-0.3.2a1/foliolib/cli/platform.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     2754 2023-04-01 07:33:03.000000 foliolib-0.3.2a1/foliolib/cli/server.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    12868 2022-10-06 05:29:03.000000 foliolib-0.3.2a1/foliolib/cli/tenant.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    11993 2023-04-01 07:33:58.000000 foliolib-0.3.2a1/foliolib/config.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      801 2022-05-09 17:52:49.000000 foliolib-0.3.2a1/foliolib/exceptions.py
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-04-16 05:35:39.725968 foliolib-0.3.2a1/foliolib/folio/
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1870 2022-10-06 05:35:01.000000 foliolib-0.3.2a1/foliolib/folio/__init__.py
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-04-16 05:35:39.737968 foliolib-0.3.2a1/foliolib/folio/api/
--rw-r--r--   0 tobi      (1000) tobi      (1000)        0 2021-11-15 08:23:39.000000 foliolib-0.3.2a1/foliolib/folio/api/__init__.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     9675 2023-02-10 14:45:38.000000 foliolib-0.3.2a1/foliolib/folio/api/audit.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      173 2023-02-10 14:45:38.000000 foliolib-0.3.2a1/foliolib/folio/api/calendar.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    39987 2023-02-10 14:45:38.000000 foliolib-0.3.2a1/foliolib/folio/api/circulation.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    73691 2023-02-10 14:45:38.000000 foliolib-0.3.2a1/foliolib/folio/api/circulationStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     6506 2023-02-10 14:45:38.000000 foliolib-0.3.2a1/foliolib/folio/api/configuration.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     4913 2023-02-10 14:45:38.000000 foliolib-0.3.2a1/foliolib/folio/api/copycat.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    54009 2023-02-10 14:45:38.000000 foliolib-0.3.2a1/foliolib/folio/api/courses.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    19883 2023-02-10 14:45:38.000000 foliolib-0.3.2a1/foliolib/folio/api/dataExport.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     6764 2023-02-10 14:45:38.000000 foliolib-0.3.2a1/foliolib/folio/api/dataExportSpring.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     5642 2023-02-10 14:45:38.000000 foliolib-0.3.2a1/foliolib/folio/api/dataExportWorker.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    13485 2023-02-10 14:45:38.000000 foliolib-0.3.2a1/foliolib/folio/api/dataImport.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    37645 2023-02-10 14:45:38.000000 foliolib-0.3.2a1/foliolib/folio/api/dataImportConverterStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     2268 2023-02-10 14:45:38.000000 foliolib-0.3.2a1/foliolib/folio/api/ebsconet.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     2208 2023-02-10 14:45:38.000000 foliolib-0.3.2a1/foliolib/folio/api/edgeCaiasoft.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     2779 2023-02-10 14:45:38.000000 foliolib-0.3.2a1/foliolib/folio/api/edgeDematic.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     2818 2023-02-10 14:45:38.000000 foliolib-0.3.2a1/foliolib/folio/api/edgeLtiCourses.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     7884 2023-02-10 14:45:38.000000 foliolib-0.3.2a1/foliolib/folio/api/email.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    25152 2023-02-10 14:45:38.000000 foliolib-0.3.2a1/foliolib/folio/api/ermUsage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     4482 2023-02-10 14:45:38.000000 foliolib-0.3.2a1/foliolib/folio/api/ermUsageHarvester.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     4273 2023-02-10 14:45:38.000000 foliolib-0.3.2a1/foliolib/folio/api/eventConfig.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    80620 2023-02-10 14:45:39.000000 foliolib-0.3.2a1/foliolib/folio/api/feesfines.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    69309 2023-02-10 14:45:39.000000 foliolib-0.3.2a1/foliolib/folio/api/finance.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    72036 2023-02-10 14:45:39.000000 foliolib-0.3.2a1/foliolib/folio/api/financeStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    51717 2023-02-10 14:45:39.000000 foliolib-0.3.2a1/foliolib/folio/api/fincConfig.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     7837 2023-02-10 14:45:40.000000 foliolib-0.3.2a1/foliolib/folio/api/gobi.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    76551 2023-02-10 14:45:41.000000 foliolib-0.3.2a1/foliolib/folio/api/innReach.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    22929 2023-02-10 14:45:41.000000 foliolib-0.3.2a1/foliolib/folio/api/inventory.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)   217400 2023-02-10 14:45:42.000000 foliolib-0.3.2a1/foliolib/folio/api/inventoryStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     6001 2023-02-10 14:45:42.000000 foliolib-0.3.2a1/foliolib/folio/api/inventoryUpdate.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    38864 2023-02-10 14:45:42.000000 foliolib-0.3.2a1/foliolib/folio/api/invoice.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    44099 2023-02-10 14:45:42.000000 foliolib-0.3.2a1/foliolib/folio/api/invoiceStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    54231 2023-02-10 14:45:43.000000 foliolib-0.3.2a1/foliolib/folio/api/kbEbscoJava.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3051 2023-02-10 14:45:43.000000 foliolib-0.3.2a1/foliolib/folio/api/ldp.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1332 2023-02-10 14:45:43.000000 foliolib-0.3.2a1/foliolib/folio/api/licenses.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     8538 2023-02-10 14:45:43.000000 foliolib-0.3.2a1/foliolib/folio/api/login.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     4260 2023-02-10 14:45:43.000000 foliolib-0.3.2a1/foliolib/folio/api/loginSaml.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    17932 2023-02-10 14:45:43.000000 foliolib-0.3.2a1/foliolib/folio/api/marccat.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    20392 2023-02-10 14:45:43.000000 foliolib-0.3.2a1/foliolib/folio/api/metaStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      171 2023-02-10 14:45:43.000000 foliolib-0.3.2a1/foliolib/folio/api/notes.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     8870 2023-02-10 14:45:43.000000 foliolib-0.3.2a1/foliolib/folio/api/notify.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    12105 2023-02-10 14:45:43.000000 foliolib-0.3.2a1/foliolib/folio/api/oaiPmh.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    57718 2023-02-10 14:45:43.000000 foliolib-0.3.2a1/foliolib/folio/api/orders.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    71436 2023-02-10 14:45:43.000000 foliolib-0.3.2a1/foliolib/folio/api/ordersStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     4489 2023-02-10 14:45:43.000000 foliolib-0.3.2a1/foliolib/folio/api/organizations.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    41381 2023-02-10 14:45:43.000000 foliolib-0.3.2a1/foliolib/folio/api/organizationsStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3678 2023-02-10 14:45:43.000000 foliolib-0.3.2a1/foliolib/folio/api/passwordValidator.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     5893 2023-02-10 14:45:43.000000 foliolib-0.3.2a1/foliolib/folio/api/patron.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    15601 2023-02-10 14:45:43.000000 foliolib-0.3.2a1/foliolib/folio/api/patronBlocks.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    14392 2023-02-10 14:45:43.000000 foliolib-0.3.2a1/foliolib/folio/api/permissions.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     9093 2023-02-10 14:45:43.000000 foliolib-0.3.2a1/foliolib/folio/api/pubsub.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     4445 2023-02-10 14:45:43.000000 foliolib-0.3.2a1/foliolib/folio/api/quickMarc.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    17286 2023-02-10 14:45:44.000000 foliolib-0.3.2a1/foliolib/folio/api/remoteStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1928 2023-02-10 14:45:44.000000 foliolib-0.3.2a1/foliolib/folio/api/rtac.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    17486 2023-02-10 14:45:44.000000 foliolib-0.3.2a1/foliolib/folio/api/search.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      732 2023-02-10 14:45:44.000000 foliolib-0.3.2a1/foliolib/folio/api/sender.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    11154 2023-02-10 14:45:44.000000 foliolib-0.3.2a1/foliolib/folio/api/sharedIndex.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    21352 2023-02-10 14:45:44.000000 foliolib-0.3.2a1/foliolib/folio/api/sourceRecordManager.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    24923 2023-02-10 14:45:44.000000 foliolib-0.3.2a1/foliolib/folio/api/sourceRecordStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      170 2023-02-10 14:45:44.000000 foliolib-0.3.2a1/foliolib/folio/api/tags.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     4091 2023-02-10 14:45:44.000000 foliolib-0.3.2a1/foliolib/folio/api/templateEngine.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      870 2023-02-10 14:45:44.000000 foliolib-0.3.2a1/foliolib/folio/api/userImport.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    22608 2023-02-10 14:45:44.000000 foliolib-0.3.2a1/foliolib/folio/api/users.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    11127 2023-02-10 14:45:44.000000 foliolib-0.3.2a1/foliolib/folio/api/usersBl.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     5803 2022-05-31 09:32:11.000000 foliolib-0.3.2a1/foliolib/folio/config.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     8495 2021-02-25 09:49:29.000000 foliolib-0.3.2a1/foliolib/folio/dataImport.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      436 2022-03-17 02:39:17.000000 foliolib-0.3.2a1/foliolib/folio/exceptions.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      945 2022-04-08 08:56:47.000000 foliolib-0.3.2a1/foliolib/folio/inventory.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    24056 2022-09-15 02:29:53.000000 foliolib-0.3.2a1/foliolib/folio/inventoryReferenceData.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     9488 2022-06-03 04:45:10.000000 foliolib-0.3.2a1/foliolib/folio/users.py
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-04-16 05:35:39.741968 foliolib-0.3.2a1/foliolib/helper/
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1205 2022-08-28 17:47:01.000000 foliolib-0.3.2a1/foliolib/helper/__init__.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     9307 2023-04-15 13:31:32.000000 foliolib-0.3.2a1/foliolib/helper/database.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3636 2022-10-11 03:50:00.000000 foliolib-0.3.2a1/foliolib/helper/folio.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3055 2023-02-09 19:10:16.000000 foliolib-0.3.2a1/foliolib/helper/modules.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3935 2023-04-01 06:20:04.000000 foliolib-0.3.2a1/foliolib/helper/okapi.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     5714 2023-02-18 17:54:00.000000 foliolib-0.3.2a1/foliolib/helper/platform.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1517 2022-10-11 03:48:54.000000 foliolib-0.3.2a1/foliolib/helper/tenant.py
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-04-16 05:35:39.741968 foliolib-0.3.2a1/foliolib/okapi/
--rw-r--r--   0 tobi      (1000) tobi      (1000)    14520 2022-10-13 08:48:51.000000 foliolib-0.3.2a1/foliolib/okapi/__init__.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     2399 2022-07-24 04:45:10.000000 foliolib-0.3.2a1/foliolib/okapi/exceptions.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    16265 2023-04-15 13:33:45.000000 foliolib-0.3.2a1/foliolib/okapi/kubeClient.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      542 2022-03-22 15:04:58.000000 foliolib-0.3.2a1/foliolib/okapi/misc.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    38795 2023-03-24 13:15:22.000000 foliolib-0.3.2a1/foliolib/okapi/okapiClient.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    10030 2023-02-02 10:53:21.000000 foliolib-0.3.2a1/foliolib/okapi/okapiModule.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    17119 2023-04-04 07:30:25.000000 foliolib-0.3.2a1/foliolib/okapi/okapiModuleKubernetes.py
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-04-16 05:35:39.721968 foliolib-0.3.2a1/foliolib.egg-info/
--rw-r--r--   0 tobi      (1000) tobi      (1000)     2357 2023-04-16 05:35:39.000000 foliolib-0.3.2a1/foliolib.egg-info/PKG-INFO
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3472 2023-04-16 05:35:39.000000 foliolib-0.3.2a1/foliolib.egg-info/SOURCES.txt
--rw-r--r--   0 tobi      (1000) tobi      (1000)        1 2023-04-16 05:35:39.000000 foliolib-0.3.2a1/foliolib.egg-info/dependency_links.txt
--rw-r--r--   0 tobi      (1000) tobi      (1000)       88 2023-04-16 05:35:39.000000 foliolib-0.3.2a1/foliolib.egg-info/entry_points.txt
--rw-r--r--   0 tobi      (1000) tobi      (1000)      130 2023-04-16 05:35:39.000000 foliolib-0.3.2a1/foliolib.egg-info/requires.txt
--rw-r--r--   0 tobi      (1000) tobi      (1000)      126 2023-04-16 05:35:39.000000 foliolib-0.3.2a1/foliolib.egg-info/top_level.txt
--rw-r--r--   0 tobi      (1000) tobi      (1000)      305 2023-02-21 08:41:56.000000 foliolib-0.3.2a1/requirements.txt
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1145 2023-04-16 05:35:39.741968 foliolib-0.3.2a1/setup.cfg
--rw-r--r--   0 tobi      (1000) tobi      (1000)      117 2022-10-11 12:39:31.000000 foliolib-0.3.2a1/setup.py
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-04-23 06:38:47.864991 foliolib-0.3.3a1/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    35146 2020-10-11 07:41:52.000000 foliolib-0.3.3a1/COPYING
+-rw-r--r--   0 tobi      (1000) tobi      (1000)       43 2020-11-07 12:13:21.000000 foliolib-0.3.3a1/MANIFEST.in
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     2357 2023-04-23 06:38:47.864991 foliolib-0.3.3a1/PKG-INFO
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1719 2023-02-21 11:23:02.000000 foliolib-0.3.3a1/README.rst
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-04-23 06:38:47.840991 foliolib-0.3.3a1/foliolib/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1031 2023-03-24 13:25:47.000000 foliolib-0.3.3a1/foliolib/__init__.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      396 2023-04-23 06:38:47.000000 foliolib-0.3.3a1/foliolib/__version__.py
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-04-23 06:38:47.840991 foliolib-0.3.3a1/foliolib/apiBuilder/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      351 2022-10-11 12:37:16.000000 foliolib-0.3.3a1/foliolib/apiBuilder/__init__.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1288 2022-03-13 04:11:25.000000 foliolib-0.3.3a1/foliolib/apiBuilder/build_api.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1586 2022-05-04 20:18:39.000000 foliolib-0.3.3a1/foliolib/apiBuilder/cli.py
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-04-23 06:38:47.844991 foliolib-0.3.3a1/foliolib/cli/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3821 2023-04-21 06:17:59.000000 foliolib-0.3.3a1/foliolib/cli/__init__.py
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-04-23 06:38:47.844991 foliolib-0.3.3a1/foliolib/cli/folio/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1461 2022-05-09 17:53:56.000000 foliolib-0.3.3a1/foliolib/cli/folio/__init__.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      229 2022-04-05 13:20:51.000000 foliolib-0.3.3a1/foliolib/cli/folio/inventory.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      634 2022-02-21 04:57:32.000000 foliolib-0.3.3a1/foliolib/cli/main.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      374 2022-02-21 04:57:41.000000 foliolib-0.3.3a1/foliolib/cli/main_err.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      895 2022-02-21 04:57:36.000000 foliolib-0.3.3a1/foliolib/cli/main_noauth.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     4591 2023-04-15 04:58:38.000000 foliolib-0.3.3a1/foliolib/cli/module.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3495 2023-04-01 07:43:09.000000 foliolib-0.3.3a1/foliolib/cli/okapi.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      446 2022-02-21 04:57:17.000000 foliolib-0.3.3a1/foliolib/cli/orderedGroup.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3680 2023-02-15 15:06:27.000000 foliolib-0.3.3a1/foliolib/cli/platform.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     2759 2023-04-21 05:25:46.000000 foliolib-0.3.3a1/foliolib/cli/server.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    12868 2022-10-06 05:29:03.000000 foliolib-0.3.3a1/foliolib/cli/tenant.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    12088 2023-04-21 06:26:30.000000 foliolib-0.3.3a1/foliolib/config.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      801 2022-05-09 17:52:49.000000 foliolib-0.3.3a1/foliolib/exceptions.py
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-04-23 06:38:47.844991 foliolib-0.3.3a1/foliolib/folio/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1870 2022-10-06 05:35:01.000000 foliolib-0.3.3a1/foliolib/folio/__init__.py
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-04-23 06:38:47.860991 foliolib-0.3.3a1/foliolib/folio/api/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)        0 2021-11-15 08:23:39.000000 foliolib-0.3.3a1/foliolib/folio/api/__init__.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     9675 2023-04-16 06:50:57.000000 foliolib-0.3.3a1/foliolib/folio/api/audit.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     6883 2023-04-16 06:50:57.000000 foliolib-0.3.3a1/foliolib/folio/api/bulkOperations.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      173 2023-04-16 06:50:57.000000 foliolib-0.3.3a1/foliolib/folio/api/calendar.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    40174 2023-04-16 06:50:57.000000 foliolib-0.3.3a1/foliolib/folio/api/circulation.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    73691 2023-04-16 06:50:57.000000 foliolib-0.3.3a1/foliolib/folio/api/circulationStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     6506 2023-04-16 06:50:57.000000 foliolib-0.3.3a1/foliolib/folio/api/configuration.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     4913 2023-04-16 06:50:57.000000 foliolib-0.3.3a1/foliolib/folio/api/copycat.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    54009 2023-04-16 06:50:58.000000 foliolib-0.3.3a1/foliolib/folio/api/courses.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    19883 2023-04-16 06:50:58.000000 foliolib-0.3.3a1/foliolib/folio/api/dataExport.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     6764 2023-04-16 06:50:58.000000 foliolib-0.3.3a1/foliolib/folio/api/dataExportSpring.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     5642 2023-04-16 06:50:58.000000 foliolib-0.3.3a1/foliolib/folio/api/dataExportWorker.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    13485 2023-04-16 06:50:58.000000 foliolib-0.3.3a1/foliolib/folio/api/dataImport.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    37645 2023-04-16 06:50:58.000000 foliolib-0.3.3a1/foliolib/folio/api/dataImportConverterStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     2268 2023-04-16 06:50:58.000000 foliolib-0.3.3a1/foliolib/folio/api/ebsconet.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     7884 2023-04-16 06:50:58.000000 foliolib-0.3.3a1/foliolib/folio/api/email.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     4399 2023-04-16 06:50:58.000000 foliolib-0.3.3a1/foliolib/folio/api/entitiesLinks.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    25152 2023-04-16 06:50:58.000000 foliolib-0.3.3a1/foliolib/folio/api/ermUsage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     4482 2023-04-16 06:50:58.000000 foliolib-0.3.3a1/foliolib/folio/api/ermUsageHarvester.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     4273 2023-04-16 06:50:58.000000 foliolib-0.3.3a1/foliolib/folio/api/eventConfig.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    80620 2023-04-16 06:50:59.000000 foliolib-0.3.3a1/foliolib/folio/api/feesfines.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    76479 2023-04-16 06:50:59.000000 foliolib-0.3.3a1/foliolib/folio/api/finance.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    79172 2023-04-16 06:50:59.000000 foliolib-0.3.3a1/foliolib/folio/api/financeStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    51717 2023-04-16 06:50:59.000000 foliolib-0.3.3a1/foliolib/folio/api/fincConfig.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     8283 2023-04-16 06:51:00.000000 foliolib-0.3.3a1/foliolib/folio/api/gobi.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    76551 2023-04-16 06:51:02.000000 foliolib-0.3.3a1/foliolib/folio/api/innReach.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    22929 2023-04-16 06:51:02.000000 foliolib-0.3.3a1/foliolib/folio/api/inventory.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)   217418 2023-04-16 06:51:03.000000 foliolib-0.3.3a1/foliolib/folio/api/inventoryStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     6001 2023-04-16 06:51:03.000000 foliolib-0.3.3a1/foliolib/folio/api/inventoryUpdate.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    45051 2023-04-16 06:51:03.000000 foliolib-0.3.3a1/foliolib/folio/api/invoice.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    47143 2023-04-16 06:51:03.000000 foliolib-0.3.3a1/foliolib/folio/api/invoiceStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    54294 2023-04-16 06:51:03.000000 foliolib-0.3.3a1/foliolib/folio/api/kbEbscoJava.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3051 2023-04-16 06:51:03.000000 foliolib-0.3.3a1/foliolib/folio/api/ldp.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1332 2023-04-16 06:51:03.000000 foliolib-0.3.3a1/foliolib/folio/api/licenses.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     8538 2023-04-16 06:51:03.000000 foliolib-0.3.3a1/foliolib/folio/api/login.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     4260 2023-04-16 06:51:03.000000 foliolib-0.3.3a1/foliolib/folio/api/loginSaml.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    17932 2023-04-16 06:51:03.000000 foliolib-0.3.3a1/foliolib/folio/api/marccat.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    20392 2023-04-16 06:51:04.000000 foliolib-0.3.3a1/foliolib/folio/api/metaStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      171 2023-04-16 06:51:04.000000 foliolib-0.3.3a1/foliolib/folio/api/notes.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     8870 2023-04-16 06:51:04.000000 foliolib-0.3.3a1/foliolib/folio/api/notify.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    12105 2023-04-16 06:51:04.000000 foliolib-0.3.3a1/foliolib/folio/api/oaiPmh.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    63105 2023-04-16 06:51:04.000000 foliolib-0.3.3a1/foliolib/folio/api/orders.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    78262 2023-04-16 06:51:04.000000 foliolib-0.3.3a1/foliolib/folio/api/ordersStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     4978 2023-04-16 06:51:04.000000 foliolib-0.3.3a1/foliolib/folio/api/organizations.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    45825 2023-04-16 06:51:04.000000 foliolib-0.3.3a1/foliolib/folio/api/organizationsStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3678 2023-04-16 06:51:04.000000 foliolib-0.3.3a1/foliolib/folio/api/passwordValidator.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     5893 2023-04-16 06:51:04.000000 foliolib-0.3.3a1/foliolib/folio/api/patron.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    15601 2023-04-16 06:51:04.000000 foliolib-0.3.3a1/foliolib/folio/api/patronBlocks.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    14392 2023-04-16 06:51:04.000000 foliolib-0.3.3a1/foliolib/folio/api/permissions.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     9093 2023-04-16 06:51:04.000000 foliolib-0.3.3a1/foliolib/folio/api/pubsub.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     4445 2023-04-16 06:51:05.000000 foliolib-0.3.3a1/foliolib/folio/api/quickMarc.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    17286 2023-04-16 06:51:05.000000 foliolib-0.3.3a1/foliolib/folio/api/remoteStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    21589 2023-04-16 06:51:05.000000 foliolib-0.3.3a1/foliolib/folio/api/reservoir.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1928 2023-04-16 06:51:05.000000 foliolib-0.3.3a1/foliolib/folio/api/rtac.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    17486 2023-04-16 06:51:05.000000 foliolib-0.3.3a1/foliolib/folio/api/search.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      732 2023-04-16 06:51:05.000000 foliolib-0.3.3a1/foliolib/folio/api/sender.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     5425 2023-04-16 06:51:05.000000 foliolib-0.3.3a1/foliolib/folio/api/settings.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    11154 2023-04-16 06:51:05.000000 foliolib-0.3.3a1/foliolib/folio/api/sharedIndex.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    21352 2023-04-16 06:51:05.000000 foliolib-0.3.3a1/foliolib/folio/api/sourceRecordManager.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    24923 2023-04-16 06:51:05.000000 foliolib-0.3.3a1/foliolib/folio/api/sourceRecordStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      170 2023-04-16 06:51:05.000000 foliolib-0.3.3a1/foliolib/folio/api/tags.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     4091 2023-04-16 06:51:05.000000 foliolib-0.3.3a1/foliolib/folio/api/templateEngine.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      870 2023-04-16 06:51:05.000000 foliolib-0.3.3a1/foliolib/folio/api/userImport.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    22806 2023-04-16 06:51:05.000000 foliolib-0.3.3a1/foliolib/folio/api/users.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    11127 2023-04-16 06:51:05.000000 foliolib-0.3.3a1/foliolib/folio/api/usersBl.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     5803 2022-05-31 09:32:11.000000 foliolib-0.3.3a1/foliolib/folio/config.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     8495 2021-02-25 09:49:29.000000 foliolib-0.3.3a1/foliolib/folio/dataImport.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      436 2022-03-17 02:39:17.000000 foliolib-0.3.3a1/foliolib/folio/exceptions.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      945 2022-04-08 08:56:47.000000 foliolib-0.3.3a1/foliolib/folio/inventory.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    24056 2022-09-15 02:29:53.000000 foliolib-0.3.3a1/foliolib/folio/inventoryReferenceData.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     9488 2022-06-03 04:45:10.000000 foliolib-0.3.3a1/foliolib/folio/users.py
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-04-23 06:38:47.860991 foliolib-0.3.3a1/foliolib/helper/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1207 2023-04-21 05:23:46.000000 foliolib-0.3.3a1/foliolib/helper/__init__.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     9311 2023-04-21 05:23:46.000000 foliolib-0.3.3a1/foliolib/helper/database.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3636 2022-10-11 03:50:00.000000 foliolib-0.3.3a1/foliolib/helper/folio.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3055 2023-02-09 19:10:16.000000 foliolib-0.3.3a1/foliolib/helper/modules.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3935 2023-04-01 06:20:04.000000 foliolib-0.3.3a1/foliolib/helper/okapi.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     5714 2023-02-18 17:54:00.000000 foliolib-0.3.3a1/foliolib/helper/platform.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1517 2022-10-11 03:48:54.000000 foliolib-0.3.3a1/foliolib/helper/tenant.py
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-04-23 06:38:47.864991 foliolib-0.3.3a1/foliolib/okapi/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    14520 2022-10-13 08:48:51.000000 foliolib-0.3.3a1/foliolib/okapi/__init__.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     2399 2022-07-24 04:45:10.000000 foliolib-0.3.3a1/foliolib/okapi/exceptions.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    16267 2023-04-21 05:23:46.000000 foliolib-0.3.3a1/foliolib/okapi/kubeClient.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      542 2022-03-22 15:04:58.000000 foliolib-0.3.3a1/foliolib/okapi/misc.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    38800 2023-04-21 05:23:46.000000 foliolib-0.3.3a1/foliolib/okapi/okapiClient.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    10030 2023-02-02 10:53:21.000000 foliolib-0.3.3a1/foliolib/okapi/okapiModule.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    17121 2023-04-21 05:23:46.000000 foliolib-0.3.3a1/foliolib/okapi/okapiModuleKubernetes.py
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-04-23 06:38:47.840991 foliolib-0.3.3a1/foliolib.egg-info/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     2357 2023-04-23 06:38:47.000000 foliolib-0.3.3a1/foliolib.egg-info/PKG-INFO
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3502 2023-04-23 06:38:47.000000 foliolib-0.3.3a1/foliolib.egg-info/SOURCES.txt
+-rw-r--r--   0 tobi      (1000) tobi      (1000)        1 2023-04-23 06:38:47.000000 foliolib-0.3.3a1/foliolib.egg-info/dependency_links.txt
+-rw-r--r--   0 tobi      (1000) tobi      (1000)       88 2023-04-23 06:38:47.000000 foliolib-0.3.3a1/foliolib.egg-info/entry_points.txt
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      130 2023-04-23 06:38:47.000000 foliolib-0.3.3a1/foliolib.egg-info/requires.txt
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      126 2023-04-23 06:38:47.000000 foliolib-0.3.3a1/foliolib.egg-info/top_level.txt
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      305 2023-02-21 08:41:56.000000 foliolib-0.3.3a1/requirements.txt
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1145 2023-04-23 06:38:47.864991 foliolib-0.3.3a1/setup.cfg
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      117 2022-10-11 12:39:31.000000 foliolib-0.3.3a1/setup.py
```

### Comparing `foliolib-0.3.2a1/COPYING` & `foliolib-0.3.3a1/COPYING`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.2a1/PKG-INFO` & `foliolib-0.3.3a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foliolib
-Version: 0.3.2a1
+Version: 0.3.3a1
 Summary: Okapi/Folio Manager and Library
 Home-page: https://github.com/tobi-weber/foliolib
 Author: Tobias Weber
 Author-email: tobi-weber@gmx.de
 License: GPL-3.0 License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `foliolib-0.3.2a1/README.rst` & `foliolib-0.3.3a1/README.rst`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.2a1/foliolib/__init__.py` & `foliolib-0.3.3a1/foliolib/__init__.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.2a1/foliolib/apiBuilder/build_api.py` & `foliolib-0.3.3a1/foliolib/apiBuilder/build_api.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.2a1/foliolib/apiBuilder/cli.py` & `foliolib-0.3.3a1/foliolib/apiBuilder/cli.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.2a1/foliolib/cli/__init__.py` & `foliolib-0.3.3a1/foliolib/cli/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,18 @@
     elif len(sys.argv) > 2 and sys.argv[1] == "server" and sys.argv[2] == "delete":
         return True
     elif "FOLIOLIB_SERVER" in os.environ:
         config.set_server(os.environ["FOLIOLIB_SERVER"])
     elif os.path.exists(fname):
         with open(fname) as f:
             config.set_server(f.read())
+        level = Config().servercfg().get("Cli", "loglevel", fallback="INFO")
+        if "FOLIOLIB_LOGLEVEL" in os.environ:
+            level = os.environ["FOLIOLIB_LOGLEVEL"]
+        set_logging(level, traceback=False)
     else:
         print("\nEnable a server config or create a new one!\n")
         return False
     return True
 
 
 def __check_okapi():
@@ -50,14 +54,16 @@
         return 11
     except OkapiFatalError as e:
         print(e)
         return 12
 
 
 def __confirmation():
+    if not Config().servercfg().getboolean("Cli", "confirm", fallback=False):
+        return True
     confirmFile = os.path.join(Config().get_confdir(), ".confirm")
     confirmServer = None
     if os.path.exists(confirmFile):
         with open(confirmFile, encoding="utf8") as f:
             confirmServer = f.read()
     if len(sys.argv) > 2:
         if confirmServer is not None:
@@ -93,18 +99,14 @@
 
 def __run_err_cli():
     from foliolib.cli.main_err import main
     main()
 
 
 def cli():
-    level = "INFO"
-    if "FOLIOLIB_LOGLEVEL" in os.environ:
-        level = os.environ["FOLIOLIB_LOGLEVEL"]
-    set_logging(level, traceback=False)
     if __load_config():
         if len(sys.argv) > 1 and sys.argv[1] == "server":
             __run_err_cli()
         check_okapi = __check_okapi()
         print(
             f"== Active server is {Config().get_server()} - {Config().get_url()}")
         if check_okapi == 1:
```

### Comparing `foliolib-0.3.2a1/foliolib/cli/folio/__init__.py` & `foliolib-0.3.3a1/foliolib/cli/folio/__init__.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.2a1/foliolib/cli/main.py` & `foliolib-0.3.3a1/foliolib/cli/main.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.2a1/foliolib/cli/main_noauth.py` & `foliolib-0.3.3a1/foliolib/cli/main_noauth.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.2a1/foliolib/cli/module.py` & `foliolib-0.3.3a1/foliolib/cli/module.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.2a1/foliolib/cli/okapi.py` & `foliolib-0.3.3a1/foliolib/cli/okapi.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.2a1/foliolib/cli/platform.py` & `foliolib-0.3.3a1/foliolib/cli/platform.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.2a1/foliolib/cli/server.py` & `foliolib-0.3.3a1/foliolib/cli/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,16 +49,16 @@
     name = kwargs["name"]
     if name in Config().get_servers():
         print("Load configs for server %s." % name)
         config = Config()
         config.set_server(name)
         __save_current_server(name)
         print("Loaded config: %s - %s:%s" % (Config().get_server(),
-                                             Config().okapicfg().get("Okapi", "host"),
-                                             Config().okapicfg().get("Okapi", "port")))
+                                             Config().servercfg().get("Okapi", "host"),
+                                             Config().servercfg().get("Okapi", "port")))
     else:
         print("Config for server %s does not exist." % name)
 
 
 @server.command()
 @click.argument("name")
 @click.option("-H", "--host", default="localhost", help="okapi host", show_default=True)
@@ -70,17 +70,17 @@
 
     NAME\tserver name.
     """
     name = kwargs["name"]
     if not name in Config().get_servers():
         print(f"Create configs for server %s." % name)
         Config().create_foliolib_conf()
-        Config().create_okapi_conf(name, okapi_host=kwargs["host"],
-                                   okapi_port=kwargs["port"],
-                                   ssl=kwargs["ssl"])
+        Config().create_server_conf(name, okapi_host=kwargs["host"],
+                                    okapi_port=kwargs["port"],
+                                    ssl=kwargs["ssl"])
         Config().set_server(name)
         __save_current_server(name)
     else:
         print("Config for server %s exist already." % kwargs["name"])
 
 
 @server.command()
```

### Comparing `foliolib-0.3.2a1/foliolib/cli/tenant.py` & `foliolib-0.3.3a1/foliolib/cli/tenant.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.2a1/foliolib/config.py` & `foliolib-0.3.3a1/foliolib/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             cls.__init__ = init_pass
 
         return cls._inst
 
     def __init__(self):
         self._server = None
         self.__foliolibcfg = None
-        self.__okapicfg = None
+        self.__servercfg = None
 
     def get_server(self):
         """Get current server name.
 
         Returns:
             str: Current server name.
         """
@@ -49,34 +49,34 @@
 
         Raises:
             ServerConfigNotFound: Server config not found.
         """
         if name in self.get_servers():
             self._server = name
             self.__foliolibcfg = configparser.ConfigParser()
-            self.__okapicfg = configparser.ConfigParser()
+            self.__servercfg = configparser.ConfigParser()
             self.__load()
         else:
             raise ServerConfigNotFound(name, self.get_servers())
 
     def foliolibcfg(self):
         """Get foliolib.conf ConfigParser object.
 
         Returns:
             ConfigParser: ConfigParser object of foliolib.conf
         """
         return self.__foliolibcfg
 
-    def okapicfg(self):
-        """Get okapi.conf ConfigParser object.
+    def servercfg(self):
+        """Get server.conf ConfigParser object.
 
         Returns:
-            ConfigParser: ConfigParser object of okapi.conf of the current server setted.
+            ConfigParser: ConfigParser object of server.conf of the current server setted.
         """
-        return self.__okapicfg
+        return self.__servercfg
 
     def modulescfg(self, modId):
         """Get ConfigParser object of a module config file.
 
         Returns:
             ConfigParser: ConfigParser object of $MODULENAME.conf for a specific module.
         """
@@ -98,15 +98,15 @@
 
     def is_kubernetes(self):
         """Is Kubernetes enabled?
 
         Returns:
             bool: Wether kubernets is enabled.
         """
-        return self.__okapicfg.get("Kubernetes", "enable", fallback=False)
+        return self.__servercfg.get("Kubernetes", "enable", fallback=False)
 
     def get_kube_config(self):
         kube_config = os.path.join(self.get_confdir(),
                                    self.get_server(), "kube_config")
         if os.path.exists(kube_config):
             return kube_config
         else:
@@ -116,148 +116,146 @@
         """Get all available server configs.
 
         Returns:
             List: List of available servers.
         """
         servers = []
         for f in os.listdir(self.get_confdir()):
-            if os.path.exists(os.path.join(self.get_confdir(), f, "okapi.conf")):
+            if os.path.exists(os.path.join(self.get_confdir(), f, "server.conf")):
                 servers.append(f)
         return servers
 
     def get_url(self):
-        host = self.okapicfg().get("Okapi", "host")
-        port = self.okapicfg().get("Okapi", "port")
-        ssl = self.okapicfg().getboolean("Okapi", "ssl", fallback=False)
+        host = self.servercfg().get("Okapi", "host")
+        port = self.servercfg().get("Okapi", "port")
+        ssl = self.servercfg().getboolean("Okapi", "ssl", fallback=False)
         if ssl:
             url = f"https://{host}:{port}"
         else:
             url = f"http://{host}:{port}"
 
         return url
 
-    def set_okapicfg(self, section: str, option: str, value: str):
-        """Set a value in okapi.conf
+    def set_servercfg(self, section: str, option: str, value: str):
+        """Set a value in server.conf
 
         Args:
             section (str): Section
             option (str): Option
             value (any): Value
         """
         fname = os.path.join(self.get_confdir(),
                              self.get_server(),
-                             "okapi.conf")
-        if not section in self.__okapicfg:
-            self.__okapicfg[section] = {}
-        self.__okapicfg.set(section, option, value)
+                             "server.conf")
+        if not section in self.__servercfg:
+            self.__servercfg[section] = {}
+        self.__servercfg.set(section, option, value)
         with open(fname, "w") as f:
-            self.__okapicfg.write(f)
+            self.__servercfg.write(f)
 
-    def remove_okapicfg(self, section: str, option: str):
-        """Remove a option in okapi.conf
+    def remove_servercfg(self, section: str, option: str):
+        """Remove a option in server.conf
 
         Args:
             section (str): Section
             option (str): Option
             value (any): Value
         """
         fname = os.path.join(self.get_confdir(),
                              self.get_server(),
-                             "okapi.conf")
-        self.__okapicfg.remove_option(section, option)
+                             "server.conf")
+        self.__servercfg.remove_option(section, option)
         with open(fname, "w") as f:
-            self.__okapicfg.write(f)
+            self.__servercfg.write(f)
 
     def set_foliolibcfg(self, section: str, option: str, value: str):
         """Set a value in foliolib.conf
 
         Args:
             section (str): Section
             option (str): Option
             value (any): Value
         """
         fname = os.path.join(self.get_confdir(),
                              "foliolib.conf")
-        if not section in self.__okapicfg:
+        if not section in self.__servercfg:
             self.__foliolibcfg[section] = {}
         self.__foliolibcfg.set(section, option, value)
         with open(fname, "w") as f:
             self.__foliolibcfg.write(f)
 
     def get_token(self, tenantid: str):
         """Get token for a tenant
 
         Args:
             tenantid (str): tenant id
         """
-        return self.__okapicfg.get("Tokens", tenantid, fallback=None)
+        return self.__servercfg.get("Tokens", tenantid, fallback=None)
 
     def set_token(self, tenantid: str, token: str):
         """Set token for a tenant
 
         Args:
             tenantid (str): tenant id
             token (str): token
         """
         log.debug("Set token for %s", tenantid)
-        self.set_okapicfg("Tokens", tenantid, token)
+        self.set_servercfg("Tokens", tenantid, token)
 
     def del_token(self, tenantid: str):
         """Delete token for a tenant
 
         Args:
             tenantid (str): tenant id
             token (str): token
         """
         if self.has_token(tenantid):
             log.debug("Remove token for %s", tenantid)
-            self.__okapicfg.remove_option("Tokens", tenantid)
+            self.__servercfg.remove_option("Tokens", tenantid)
 
     def has_token(self, tenantid: str):
         """Delete token for a tenant
 
         Args:
             tenantid (str): tenant id
             token (str): token
         """
-        return self.__okapicfg.has_option("Tokens", tenantid)
+        return self.__servercfg.has_option("Tokens", tenantid)
 
     def is_foliolib_env(self):
         """Is global env handled by foliolib?
 
         Returns:
             bool: Wether foliolib env is enabled.
         """
-        is_foliolib_env = self.__okapicfg.get(
+        is_foliolib_env = self.__servercfg.get(
             "Okapi", "foliolibEnv", fallback=False)
-        # if is_foliolib_env and not self.__okapicfg.has_section("Env"):
-        #    self.__okapicfg.add_section("Env")
 
         return is_foliolib_env
 
     def get_env(self, as_dict=False):
         if self.is_foliolib_env():
             if as_dict:
-                return {k: v for k, v in self.__okapicfg["Env"].items()}
+                return {k: v for k, v in self.__servercfg["Env"].items()}
             else:
                 return [{"name": k, "value": v}
-                        for k, v in self.__okapicfg["Env"].items()]
+                        for k, v in self.__servercfg["Env"].items()]
         else:
             if as_dict:
                 return {}
             else:
                 return []
 
     def set_env(self, key, value):
         if self.is_foliolib_env():
-            self.set_okapicfg("Env", key, value)
+            self.set_servercfg("Env", key, value)
 
     def delete_env(self, key):
         if self.is_foliolib_env():
-            self.remove_okapicfg("Env", key)
+            self.remove_servercfg("Env", key)
 
     def get_confdir(self):
         """Get the configuration directory
 
         Returns:
             str: Path to configuration directory
         """
@@ -287,68 +285,71 @@
             self.__foliolibcfg["GitHub"] = {}
             self.__foliolibcfg["GitHub"]["access-token"] = ""
             with open(fpath, "w") as f:
                 self.__foliolibcfg.write(f)
         else:
             log.debug("%s already exists.", fpath)
 
-    def create_okapi_conf(self, name: str, okapi_host: str = "localhost",
-                          okapi_port: str = "9130", ssl=False):
-        """Create okapi.conf for given server config name.
+    def create_server_conf(self, name: str, okapi_host: str = "localhost",
+                           okapi_port: str = "9130", ssl=False):
+        """Create server.conf for given server config name.
 
         Args:
             name (str): Server name.
             okapi_host (str, optional): Okapi host. Defaults to "localhost".
             okapi_port (str, optional): Okapi port. Defaults to "9130".
             ssl (bool, optional): SSL. Defaults to False.
         """
-        self.__okapicfg = configparser.ConfigParser()
+        self.__servercfg = configparser.ConfigParser()
         sdir = os.path.join(self.get_confdir(), name)
-        fpath = os.path.join(sdir, "okapi.conf")
+        fpath = os.path.join(sdir, "server.conf")
         if not os.path.exists(fpath):
             os.mkdir(sdir)
             os.mkdir(os.path.join(sdir, "modules"))
             log.debug("Write new config %s", fpath)
-            self.__okapicfg["Okapi"] = {}
-            self.__okapicfg["Okapi"]["host"] = okapi_host
-            self.__okapicfg["Okapi"]["port"] = okapi_port
-            self.__okapicfg["Okapi"]["ssl"] = str(ssl)
-            self.__okapicfg["Okapi"]["foliolibenv"] = str(True)
-            self.__okapicfg["Env"] = {}
-            self.__okapicfg["Env"]["db_host"] = okapi_host
-            self.__okapicfg["Env"]["db_port"] = "default"
-            self.__okapicfg["Env"]["db_username"] = "okapi"
-            self.__okapicfg["Env"]["db_password"] = "okapi25"
-            self.__okapicfg["Env"]["db_database"] = "okapi"
-            self.__okapicfg["Env"]["db_querytimeout"] = "120000"
-            self.__okapicfg["Env"]["db_charset"] = "UTF-8"
-            self.__okapicfg["Env"]["kafka_host"] = okapi_host
-            self.__okapicfg["Env"]["kafka_port"] = "9092"
-            self.__okapicfg["Env"]["okapi_url"] = f"http://{okapi_host}:{okapi_port}"
-            self.__okapicfg["Env"]["replication_factor"] = "1"
+            self.__servercfg["Okapi"] = {}
+            self.__servercfg["Okapi"]["host"] = okapi_host
+            self.__servercfg["Okapi"]["port"] = okapi_port
+            self.__servercfg["Okapi"]["ssl"] = str(ssl)
+            self.__servercfg["Okapi"]["foliolibenv"] = str(True)
+            self.__servercfg["Cli"] = {}
+            self.__servercfg["Cli"]["confirm"] = str(True)
+            self.__servercfg["Cli"]["loglevel"] = "INFO"
+            self.__servercfg["Env"] = {}
+            self.__servercfg["Env"]["db_host"] = okapi_host
+            self.__servercfg["Env"]["db_port"] = "default"
+            self.__servercfg["Env"]["db_username"] = "okapi"
+            self.__servercfg["Env"]["db_password"] = "okapi25"
+            self.__servercfg["Env"]["db_database"] = "okapi"
+            self.__servercfg["Env"]["db_querytimeout"] = "120000"
+            self.__servercfg["Env"]["db_charset"] = "UTF-8"
+            self.__servercfg["Env"]["kafka_host"] = okapi_host
+            self.__servercfg["Env"]["kafka_port"] = "9092"
+            self.__servercfg["Env"]["okapi_url"] = f"http://{okapi_host}:{okapi_port}"
+            self.__servercfg["Env"]["replication_factor"] = "1"
             with open(fpath, "w") as f:
-                self.__okapicfg.write(f)
+                self.__servercfg.write(f)
             if not os.path.exists(os.path.join(sdir, "modules")):
                 os.mkdir(os.path.join(sdir, "modules"))
         else:
             log.debug("%s already exists.", fpath)
 
     def __load(self):
         # Load foliolib.conf
         fpath = os.path.join(self.get_confdir(), "foliolib.conf")
         log.debug("Load config from %s", fpath)
         self.__foliolibcfg.read(fpath)
         if not os.path.exists(self.__foliolibcfg["Cache"]["descriptors"]):
             os.makedirs(self.__foliolibcfg["Cache"]
                         ["descriptors"], exist_ok=True)
-        # Load okapi.conf
+        # Load server.conf
         sdir = os.path.join(self.get_confdir(), self.get_server())
-        fpath = os.path.join(sdir, "okapi.conf")
+        fpath = os.path.join(sdir, "server.conf")
         log.debug("Load config from %s", fpath)
-        self.__okapicfg.read(fpath)
+        self.__servercfg.read(fpath)
 
 
 def server(name, logging_level="INFO"):
     from foliolib import set_logging
     set_logging(level=logging_level)
     Config().set_server(name)
     print("Server is %s" % name)
```

### Comparing `foliolib-0.3.2a1/foliolib/exceptions.py` & `foliolib-0.3.3a1/foliolib/exceptions.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.2a1/foliolib/folio/__init__.py` & `foliolib-0.3.3a1/foliolib/folio/__init__.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/audit.py` & `foliolib-0.3.3a1/foliolib/folio/api/audit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.audit")
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/circulation.py` & `foliolib-0.3.3a1/foliolib/folio/api/circulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.circulation")
 
@@ -96,15 +96,15 @@
 class LoanAnonymization(FolioApi):
     """Loan Anonymization API
 
     **Loan Anonymization API**
     """
 
     def set_byUser(self, userId: str):
-        """
+        """Note that a 422 error with haveAssociatedFeesAndFines message and key loanIds has a value that is not a JSON array but a JSON string that contains a serialized JSON array of the loan ids.
 
         ``POST /loan-anonymization/by-user/{userId}``
 
         Args:
             userId (str)
 
         Returns:
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/circulationStorage.py` & `foliolib-0.3.3a1/foliolib/folio/api/circulationStorage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.circulationStorage")
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/configuration.py` & `foliolib-0.3.3a1/foliolib/folio/api/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.configuration")
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/copycat.py` & `foliolib-0.3.3a1/foliolib/folio/api/copycat.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.copycat")
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/courses.py` & `foliolib-0.3.3a1/foliolib/folio/api/courses.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.courses")
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/dataExport.py` & `foliolib-0.3.3a1/foliolib/folio/api/dataExport.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.dataExport")
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/dataExportSpring.py` & `foliolib-0.3.3a1/foliolib/folio/api/dataExportSpring.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("foliolib.folio.api.dataExportSpring")
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/dataExportWorker.py` & `foliolib-0.3.3a1/foliolib/folio/api/dataExportWorker.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("foliolib.folio.api.dataExportWorker")
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/dataImport.py` & `foliolib-0.3.3a1/foliolib/folio/api/dataImport.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.dataImport")
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/dataImportConverterStorage.py` & `foliolib-0.3.3a1/foliolib/folio/api/dataImportConverterStorage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.dataImportConverterStorage")
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/ebsconet.py` & `foliolib-0.3.3a1/foliolib/folio/api/ebsconet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("foliolib.folio.api.ebsconet")
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/email.py` & `foliolib-0.3.3a1/foliolib/folio/api/email.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.email")
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/ermUsage.py` & `foliolib-0.3.3a1/foliolib/folio/api/ermUsage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.ermUsage")
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/ermUsageHarvester.py` & `foliolib-0.3.3a1/foliolib/folio/api/ermUsageHarvester.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.ermUsageHarvester")
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/eventConfig.py` & `foliolib-0.3.3a1/foliolib/folio/api/eventConfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.eventConfig")
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/feesfines.py` & `foliolib-0.3.3a1/foliolib/folio/api/feesfines.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.feesfines")
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/finance.py` & `foliolib-0.3.3a1/foliolib/folio/api/finance.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.finance")
 
@@ -33,14 +33,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - ["code", "MEDGRANT", "="]
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -128,14 +133,19 @@
 
         ``GET /finance/fund-codes-expense-classes``
 
         Args:
             **kwargs (properties): Keyword Arguments
 
         Keyword Args:
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -169,14 +179,19 @@
 
         ``GET /finance/expense-classes``
 
         Args:
             **kwargs (properties): Keyword Arguments
 
         Keyword Args:
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -305,14 +320,19 @@
 
         ``GET /finance/fiscal-years``
 
         Args:
             **kwargs (properties): Keyword Arguments
 
         Keyword Args:
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -432,34 +452,29 @@
 
 class ReleaseEncumbrance(FolioApi):
     """Release encumbrance API
 
     This documents the API calls that release any remaining money encumbered back to the budget's available pool
     """
 
-    def set_releaseEncumbrance(self, releaseEncumbranceId: str, **kwargs):
+    def set_releaseEncumbrance(self, releaseEncumbranceId: str):
         """Release encumbrance
 
         ``POST /finance/release-encumbrance/{releaseEncumbranceId}``
 
         Args:
             releaseEncumbranceId (str)
-            **kwargs (properties): Keyword Arguments
-
-        Keyword Args:
-            lang (str): (default=en) Requested language. Optional. [lang=en]
-                    
 
         Raises:
             OkapiRequestError: Bad Request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Server Error
             OkapiRequestUnprocessableEntity: Unprocessable Entity
         """
-        return self.call("POST", f"/finance/release-encumbrance/{releaseEncumbranceId}", query=kwargs)
+        return self.call("POST", f"/finance/release-encumbrance/{releaseEncumbranceId}")
 
 
 class ExchangeRate(FolioApi):
     """Exchange rate API
 
     This documents the API calls that can be made to get exchange rates
     """
@@ -479,16 +494,14 @@
                     
                      - USD
             to (currency_code):  To currency code
                     
                     Example:
                     
                      - EUR
-            lang (str): (default=en) Requested language. Optional. [lang=en]
-                    
 
         Returns:
             dict: See Schema below
 
         Raises:
             OkapiRequestError: Bad Request
             OkapiRequestNotFound: Not Found
@@ -526,14 +539,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - ["code", "MEDGRANT", "="]
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -542,23 +560,62 @@
                      - 10
 
         Returns:
             dict: See Schema below
 
         Raises:
             OkapiRequestError: Bad Request
+            OkapiRequestUnauthorized: Authentication is required
             OkapiFatalError: Server Error
             OkapiRequestError: Bad Request
 
         Schema:
 
             .. literalinclude:: ../files/LedgerRolloverErrors_get_ledgerRolloversErrors_return.schema 
         """
         return self.call("GET", "/finance/ledger-rollovers-errors", query=kwargs)
 
+    def set_ledgerRolloversError(self, ledgerRolloversError: dict):
+        """Create a new ledgerRolloversError item.
+
+        ``POST /finance/ledger-rollovers-errors``
+
+        Args:
+            ledgerRolloversError (dict): See Schema below
+
+        Raises:
+            OkapiRequestError: Bad Request
+            OkapiRequestUnauthorized: Authentication is required
+            OkapiFatalError: Server Error
+
+        Headers:
+            - **Location** - URI to the created ledgerRolloversError item
+
+        Schema:
+
+            .. literalinclude:: ../files/LedgerRolloverErrors_set_ledgerRolloversError_request.schema
+        """
+        return self.call("POST", "/finance/ledger-rollovers-errors", data=ledgerRolloversError)
+
+    def delete_ledgerRolloversError(self, ledgerRolloversErrorsId: str):
+        """Delete a ledger rollover error
+
+        ``DELETE /finance/ledger-rollovers-errors/{ledgerRolloversErrorsId}``
+
+        Args:
+            ledgerRolloversErrorsId (str)
+
+        Raises:
+            OkapiRequestNotFound: Not Found
+            OkapiRequestError: Bad Request
+            OkapiFatalError: Server Error
+            OkapiRequestUnprocessableEntity: Unprocessable Entity
+        """
+        return self.call("DELETE", f"/finance/ledger-rollovers-errors/{ledgerRolloversErrorsId}")
+
 
 class GroupFundFiscalYear(FolioApi):
     """Group Fund Fiscal Year API
 
     This documents the API calls that can be made to manage group-fund-fiscal-years
     """
 
@@ -567,14 +624,19 @@
 
         ``GET /finance/group-fund-fiscal-years``
 
         Args:
             **kwargs (properties): Keyword Arguments
 
         Keyword Args:
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -629,34 +691,29 @@
 
         Schema:
 
             .. literalinclude:: ../files/GroupFundFiscalYear_set_groupFundFiscalYear_request.schema
         """
         return self.call("POST", "/finance/group-fund-fiscal-years", data=groupFundFiscalYear)
 
-    def delete_groupFundFiscalYear(self, groupFundFiscalYearsId: str, **kwargs):
+    def delete_groupFundFiscalYear(self, groupFundFiscalYearsId: str):
         """Delete a group fund fiscal year
 
         ``DELETE /finance/group-fund-fiscal-years/{groupFundFiscalYearsId}``
 
         Args:
             groupFundFiscalYearsId (str)
-            **kwargs (properties): Keyword Arguments
-
-        Keyword Args:
-            lang (str): (default=en) Requested language. Optional. [lang=en]
-                    
 
         Raises:
             OkapiRequestNotFound: Not Found
             OkapiRequestError: Bad Request
             OkapiFatalError: Server Error
             OkapiRequestUnprocessableEntity: Unprocessable Entity
         """
-        return self.call("DELETE", f"/finance/group-fund-fiscal-years/{groupFundFiscalYearsId}", query=kwargs)
+        return self.call("DELETE", f"/finance/group-fund-fiscal-years/{groupFundFiscalYearsId}")
 
 
 class Groups(FolioApi):
     """Group API
 
     This documents the API calls that can be made to manage groups
     """
@@ -666,14 +723,19 @@
 
         ``GET /finance/groups``
 
         Args:
             **kwargs (properties): Keyword Arguments
 
         Keyword Args:
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -825,14 +887,19 @@
 
         ``GET /finance/ledgers``
 
         Args:
             **kwargs (properties): Keyword Arguments
 
         Keyword Args:
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -997,14 +1064,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - ["ledgerRolloverType", "Commit", "="]
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -1061,14 +1133,19 @@
 
         ``GET /finance/fund-types``
 
         Args:
             **kwargs (properties): Keyword Arguments
 
         Keyword Args:
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -1211,14 +1288,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - ["code", "MEDGRANT", "="]
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -1350,51 +1432,41 @@
 
         Schema:
 
             .. literalinclude:: ../files/Transaction_set_encumbrance_request.schema
         """
         return self.call("POST", "/finance/encumbrances", data=encumbrance)
 
-    def modify_encumbrance(self, encumbrancesId: str, encumbrance: dict, **kwargs):
+    def modify_encumbrance(self, encumbrancesId: str, encumbrance: dict):
         """Update a Transaction instance
 
         ``PUT /finance/encumbrances/{encumbrancesId}``
 
         Args:
             encumbrancesId (str)
-            encumbrance (dict)
-            **kwargs (properties): Keyword Arguments: See Schema below
-
-        Keyword Args:
-            lang (str): (default=en) Requested language. Optional. [lang=en]
-                    
+            encumbrance (dict): See Schema below
 
         Schema:
 
             .. literalinclude:: ../files/Transaction_modify_encumbrance_request.schema
         """
-        return self.call("PUT", f"/finance/encumbrances/{encumbrancesId}", data=encumbrance, query=kwargs)
+        return self.call("PUT", f"/finance/encumbrances/{encumbrancesId}", data=encumbrance)
 
-    def delete_encumbrance(self, encumbrancesId: str, **kwargs):
+    def delete_encumbrance(self, encumbrancesId: str):
         """Delete an encumbrance with given transactionId
 
         ``DELETE /finance/encumbrances/{encumbrancesId}``
 
         Args:
             encumbrancesId (str)
-            **kwargs (properties): Keyword Arguments
-
-        Keyword Args:
-            lang (str): (default=en) Requested language. Optional. [lang=en]
-                    
 
         Raises:
             OkapiRequestUnprocessableEntity: Unprocessable Entity
         """
-        return self.call("DELETE", f"/finance/encumbrances/{encumbrancesId}", query=kwargs)
+        return self.call("DELETE", f"/finance/encumbrances/{encumbrancesId}")
 
     def set_payment(self, payment: dict):
         """Create a payment by transaction
 
         ``POST /finance/payments``
 
         Args:
@@ -1534,14 +1606,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - currency=USD
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -1700,14 +1777,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - ["budgetStatus", "Active", "="]
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -1810,14 +1892,19 @@
 
         ``GET /finance/budgets``
 
         Args:
             **kwargs (properties): Keyword Arguments
 
         Keyword Args:
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -1969,14 +2056,19 @@
 
         ``GET /finance/funds``
 
         Args:
             **kwargs (properties): Keyword Arguments
 
         Keyword Args:
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/financeStorage.py` & `foliolib-0.3.3a1/foliolib/folio/api/financeStorage.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.financeStorage")
 
@@ -33,14 +33,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - ["code", "MEDGRANT", "="]
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -167,14 +172,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - ["ledgerRolloverType", "Commit", "="]
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -245,14 +255,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - ["errorType", "Orders", "="]
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -379,14 +394,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - ["name", "MEDGRANT", "="]
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -513,14 +533,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - ["code", "MEDGRANT", "="]
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -647,14 +672,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - ["code", "MEDGRANT", "="]
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -781,14 +811,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - ["code", "MEDGRANT", "="]
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -915,14 +950,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - ["code", "MEDGRANT", "="]
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -1216,14 +1256,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - ["code", "MEDGRANT", "="]
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -1350,14 +1395,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - ["name", "Electronic", "="]
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -1484,14 +1534,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - ["name", "Electronic", "="]
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -1618,14 +1673,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - ["budgetStatus", "Active", "="]
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -1696,14 +1756,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - ["code", "MEDGRANT", "="]
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -1830,14 +1895,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - group.name == History and and fund.fundStatus == Active and fiscalYear.periodEnd < 2020-01-01 and fundType.name == Monographs and ledger.name == One-time
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -1964,14 +2034,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - ["code", "MEDGRANT", "="]
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -2020,14 +2095,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - status==Active sortBy name
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/fincConfig.py` & `foliolib-0.3.3a1/foliolib/folio/api/fincConfig.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.fincConfig")
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/gobi.py` & `foliolib-0.3.3a1/foliolib/folio/api/gobi.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.gobi")
 
@@ -88,14 +88,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - ["value", "Purchase At Vendor System", "="]
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/innReach.py` & `foliolib-0.3.3a1/foliolib/folio/api/innReach.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("foliolib.folio.api.innReach")
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/inventory.py` & `foliolib-0.3.3a1/foliolib/folio/api/inventory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.inventory")
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/inventoryStorage.py` & `foliolib-0.3.3a1/foliolib/folio/api/inventoryStorage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.inventoryStorage")
 
@@ -5288,15 +5288,15 @@
         Schema:
 
             .. literalinclude:: ../files/BoundWithPart_modify_boundWithPart_request.schema
         """
         return self.call("PUT", f"/inventory-storage/bound-with-parts/{boundWithPartsId}", data=boundWithPart)
 
     def modify_boundWith(self, boundWith: dict):
-        """Manage all parts (holdings references) of a bound-with item
+        """Manage the collective set of parts (holdings references) of a bound-with item
 
         ``PUT /inventory-storage/bound-withs``
 
         Args:
             boundWith (dict): See Schema below
 
         Raises:
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/inventoryUpdate.py` & `foliolib-0.3.3a1/foliolib/folio/api/inventoryUpdate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.inventoryUpdate")
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/invoice.py` & `foliolib-0.3.3a1/foliolib/folio/api/invoice.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.invoice")
 
@@ -19,14 +19,19 @@
 
         ``GET /batch-groups``
 
         Args:
             **kwargs (properties): Keyword Arguments
 
         Keyword Args:
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -156,14 +161,19 @@
 
         ``GET /invoice/invoices``
 
         Args:
             **kwargs (properties): Keyword Arguments
 
         Keyword Args:
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -287,14 +297,19 @@
         ``GET /invoice/invoices/{invoicesId}/documents``
 
         Args:
             invoicesId (str)
             **kwargs (properties): Keyword Arguments
 
         Keyword Args:
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -374,23 +389,91 @@
         Raises:
             OkapiRequestError: Bad Request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Server Error
         """
         return self.call("DELETE", f"/invoice/invoices/{invoicesId}/documents/{documentId}")
 
+    def get_fiscalYears(self, invoicesId: str, **kwargs):
+        """Get a list of fiscal years to approve or pay the invoice
+
+        ``GET /invoice/invoices/{invoicesId}/fiscal-years``
+
+        Args:
+            invoicesId (str)
+            **kwargs (properties): Keyword Arguments
+
+        Keyword Args:
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
+            offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
+                    
+                    Example:
+                    
+                     - 0
+            limit (int): (default=10) Limit the number of elements returned in the response
+                    
+                    Example:
+                    
+                     - 10
+            query (str):  A query expressed as a CQL string
+                    (see [dev.folio.org/reference/glossary#cql](https://dev.folio.org/reference/glossary#cql))
+                    using valid searchable fields.
+                    The first example below shows the general form of a full CQL query,
+                    but those fields might not be relevant in this context.
+                    
+                    with valid searchable fields: for example metadata.createdDate
+                    
+                    
+                    Example:
+                    
+                     - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
+                    
+                     - metadata.createdDate > '2018-07-19T00:00:00.000+0000'
+
+        Returns:
+            dict: See Schema below
+
+        Raises:
+            OkapiRequestError: Bad Request
+            OkapiFatalError: Server Error
+
+        Schema:
+
+            .. literalinclude:: ../files/Invoice_get_fiscalYears_return.schema 
+        """
+        return self.call("GET", f"/invoice/invoices/{invoicesId}/fiscal-years", query=kwargs)
+
+    def set_fiscalYear(self, invoicesId: str):
+        """
+
+        ``POST /invoice/invoices/{invoicesId}/fiscal-years``
+
+        Args:
+            invoicesId (str)
+        """
+        return self.call("POST", f"/invoice/invoices/{invoicesId}/fiscal-years")
+
     def get_invoiceLines(self, **kwargs):
         """Retrieve a list of invoiceLine items.
 
         ``GET /invoice/invoice-lines``
 
         Args:
             **kwargs (properties): Keyword Arguments
 
         Keyword Args:
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -563,14 +646,19 @@
 
         ``GET /batch-voucher/export-configurations``
 
         Args:
             **kwargs (properties): Keyword Arguments
 
         Keyword Args:
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -778,14 +866,19 @@
 
         ``GET /batch-voucher/batch-voucher-exports``
 
         Args:
             **kwargs (properties): Keyword Arguments
 
         Keyword Args:
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -974,14 +1067,19 @@
 
         ``GET /voucher/vouchers``
 
         Args:
             **kwargs (properties): Keyword Arguments
 
         Keyword Args:
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -1075,14 +1173,19 @@
         ``GET /voucher/voucher-lines/{voucherLinesId}``
 
         Args:
             voucherLinesId (str)
             **kwargs (properties): Keyword Arguments
 
         Keyword Args:
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/invoiceStorage.py` & `foliolib-0.3.3a1/foliolib/folio/api/invoiceStorage.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,39 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.invoiceStorage")
 
 
 class VoucherNumber(FolioApi):
     """Voucher Number
 
     **API used to manage voucher number.**
     """
 
-    def get_voucherNumbers(self, **kwargs):
+    def get_voucherNumbers(self):
         """Get generated voucher number
 
         ``GET /voucher-storage/voucher-number``
 
-        Args:
-            **kwargs (properties): Keyword Arguments
-
-        Keyword Args:
-            lang (str): (default=en) Requested language. Optional. [lang=en]
-                    
-
         Returns:
             dict: See Schema below
 
         Raises:
             OkapiFatalError: Server Error
 
         Schema:
 
             .. literalinclude:: ../files/VoucherNumber_get_voucherNumbers_return.schema 
         """
-        return self.call("GET", "/voucher-storage/voucher-number", query=kwargs)
+        return self.call("GET", "/voucher-storage/voucher-number")
 
     def get_starts(self):
         """Get voucher number start
 
         ``GET /voucher-storage/voucher-number/start``
 
         Returns:
@@ -81,14 +74,19 @@
 
         ``GET /batch-group-storage/batch-groups``
 
         Args:
             **kwargs (properties): Keyword Arguments
 
         Keyword Args:
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -215,14 +213,19 @@
 
         ``GET /invoice-storage/invoices``
 
         Args:
             **kwargs (properties): Keyword Arguments
 
         Keyword Args:
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -343,14 +346,19 @@
         ``GET /invoice-storage/invoices/{invoicesId}/documents``
 
         Args:
             invoicesId (str)
             **kwargs (properties): Keyword Arguments
 
         Keyword Args:
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -453,14 +461,19 @@
 
         ``GET /invoice-storage/invoice-lines``
 
         Args:
             **kwargs (properties): Keyword Arguments
 
         Keyword Args:
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -579,37 +592,30 @@
 
 class InvoiceNumber(FolioApi):
     """Invoice Number
 
     **API used to manage invoice number.**
     """
 
-    def get_invoiceNumbers(self, **kwargs):
+    def get_invoiceNumbers(self):
         """Get generated invoice number
 
         ``GET /invoice-storage/invoice-number``
 
-        Args:
-            **kwargs (properties): Keyword Arguments
-
-        Keyword Args:
-            lang (str): (default=en) Requested language. Optional. [lang=en]
-                    
-
         Returns:
             dict: See Schema below
 
         Raises:
             OkapiFatalError: Server Error
 
         Schema:
 
             .. literalinclude:: ../files/InvoiceNumber_get_invoiceNumbers_return.schema 
         """
-        return self.call("GET", "/invoice-storage/invoice-number", query=kwargs)
+        return self.call("GET", "/invoice-storage/invoice-number")
 
 
 class BatchVoucherExportConfiguration(FolioApi):
     """Batch voucher export configurations CRUD API
 
     This documents the API calls that can be made to manage batch voucher export configurations; This API is intended for internal use only
     """
@@ -619,14 +625,19 @@
 
         ``GET /batch-voucher-storage/export-configurations``
 
         Args:
             **kwargs (properties): Keyword Arguments
 
         Keyword Args:
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -830,14 +841,19 @@
 
         ``GET /batch-voucher-storage/batch-voucher-exports``
 
         Args:
             **kwargs (properties): Keyword Arguments
 
         Keyword Args:
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -1041,14 +1057,19 @@
 
         ``GET /voucher-storage/vouchers``
 
         Args:
             **kwargs (properties): Keyword Arguments
 
         Keyword Args:
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -1168,14 +1189,19 @@
 
         ``GET /voucher-storage/voucher-lines``
 
         Args:
             **kwargs (properties): Keyword Arguments
 
         Keyword Args:
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -1308,16 +1334,14 @@
 
         Keyword Args:
             invoiceId (uuid):  The UUID of a invoice
                     
                     Example:
                     
                      - 8ad4b87b-9b47-4199-b0c3-5480745c6b41
-            lang (str): (default=en) Requested language. Optional. [lang=en]
-                    
 
         Returns:
             dict: See Schema below
 
         Raises:
             OkapiRequestError: Bad Request
             OkapiFatalError: Server Error
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/kbEbscoJava.py` & `foliolib-0.3.3a1/foliolib/folio/api/kbEbscoJava.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.kbEbscoJava")
 
@@ -1567,14 +1567,15 @@
                     
                      - history
             filter[publisher] (str):  String to search publishers to get a collection of titles
                     
                     Example:
                     
                      - academic
+            filter[packageIds] (list):  Search by package ids.
             include (str):  Include related resource objects, each representing a partnering of this title with a package.
                     Any bogus value, like `include=deciduousTrees`, will be silently ignored.
                     
                     
                     Example:
                     
                      - resources
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/ldp.py` & `foliolib-0.3.3a1/foliolib/folio/api/ldp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.ldp")
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/licenses.py` & `foliolib-0.3.3a1/foliolib/folio/api/licenses.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.licenses")
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/login.py` & `foliolib-0.3.3a1/foliolib/folio/api/login.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.login")
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/loginSaml.py` & `foliolib-0.3.3a1/foliolib/folio/api/loginSaml.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.loginSaml")
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/marccat.py` & `foliolib-0.3.3a1/foliolib/folio/api/marccat.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.marccat")
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/metaStorage.py` & `foliolib-0.3.3a1/foliolib/folio/api/metaStorage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("foliolib.folio.api.metaStorage")
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/notify.py` & `foliolib-0.3.3a1/foliolib/folio/api/notify.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.notify")
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/oaiPmh.py` & `foliolib-0.3.3a1/foliolib/folio/api/oaiPmh.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.oaiPmh")
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/orders.py` & `foliolib-0.3.3a1/foliolib/folio/api/orders.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.orders")
 
@@ -33,14 +33,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - ["protectRead", "false"]
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -162,14 +167,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - ["acquisitionsUnitId", "57c35c88-625d-4f0e-bc79-d22818d84d1c"]
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -326,14 +336,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - ["reasonForClosure", "Denied", "="]
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -455,14 +470,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - ["prefix", "Prx", "="]
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -584,14 +604,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - ["code", "Sfx", "="]
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -706,14 +731,19 @@
 
         ``GET /orders/order-lines``
 
         Args:
             **kwargs (properties): Keyword Arguments
 
         Keyword Args:
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -856,14 +886,19 @@
 
         ``GET /orders/pieces``
 
         Args:
             **kwargs (properties): Keyword Arguments
 
         Keyword Args:
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -989,14 +1024,19 @@
 
         ``GET /orders/receiving-history``
 
         Args:
             **kwargs (properties): Keyword Arguments
 
         Keyword Args:
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -1129,14 +1169,19 @@
 
         ``GET /orders/composite-orders``
 
         Args:
             **kwargs (properties): Keyword Arguments
 
         Keyword Args:
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -1279,14 +1324,19 @@
 
         ``GET /orders/export-history``
 
         Args:
             **kwargs (properties): Keyword Arguments
 
         Keyword Args:
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -1349,14 +1399,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - ["templateCode", "Amazon", "="]
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -1484,14 +1539,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - ["value", "Purchase At Vendor System", "="]
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -1595,61 +1655,49 @@
 
 class PoNumber(FolioApi):
     """Orders Business Logic API
 
     **API for managing PO numbers**
     """
 
-    def get_poNumbers(self, **kwargs):
+    def get_poNumbers(self):
         """Get generated PO number
 
         ``GET /orders/po-number``
 
-        Args:
-            **kwargs (properties): Keyword Arguments
-
-        Keyword Args:
-            lang (str): (default=en) Requested language. Optional. [lang=en]
-                    
-
         Returns:
             dict: See Schema below
 
         Raises:
             OkapiRequestUnprocessableEntity: Unprocessable Entity
 
         Schema:
 
             .. literalinclude:: ../files/PoNumber_get_poNumbers_return.schema 
         """
-        return self.call("GET", "/orders/po-number", query=kwargs)
+        return self.call("GET", "/orders/po-number")
 
-    def set_validate(self, validate: dict, **kwargs):
+    def set_validate(self, validate: dict):
         """validate if the PO Number is unique and matches the pattern specified
 
         ``POST /orders/po-number/validate``
 
         Args:
-            validate (dict)
-            **kwargs (properties): Keyword Arguments: See Schema below
-
-        Keyword Args:
-            lang (str): (default=en) Requested language. Optional. [lang=en]
-                    
+            validate (dict): See Schema below
 
         Raises:
             OkapiRequestError: Bad Request
             OkapiFatalError: Server Error
             OkapiRequestUnprocessableEntity: Unprocessable Entity
 
         Schema:
 
             .. literalinclude:: ../files/PoNumber_set_validate_request.schema
         """
-        return self.call("POST", "/orders/po-number/validate", data=validate, query=kwargs)
+        return self.call("POST", "/orders/po-number/validate", data=validate)
 
 
 class Titles(FolioApi):
     """Titles
 
     **CRUD API to manage Titles.**
     """
@@ -1673,14 +1721,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - ["title", "TITLE", "="]
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/ordersStorage.py` & `foliolib-0.3.3a1/foliolib/folio/api/ordersStorage.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.ordersStorage")
 
@@ -33,14 +33,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - ["code", "MEDGRANT", "="]
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -167,14 +172,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - ["code", "MEDGRANT", "="]
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -301,14 +311,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - ["reasonForClosure", "Denied", "="]
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -430,14 +445,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - ["prefix", "Prx", "="]
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -559,14 +579,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - ["code", "Sfx", "="]
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -695,14 +720,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - ["code", "MEDGRANT", "="]
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -829,14 +859,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - ["code", "MEDGRANT", "="]
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -963,14 +998,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - ["code", "MEDGRANT", "="]
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -1005,14 +1045,19 @@
 
         ``GET /orders-storage/export-history``
 
         Args:
             **kwargs (properties): Keyword Arguments
 
         Keyword Args:
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -1153,14 +1198,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - ["templateCode", "Amazon", "="]
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -1275,26 +1325,24 @@
 
         ``GET /orders-storage/po-line-number``
 
         Args:
             **kwargs (properties): Keyword Arguments
 
         Keyword Args:
-            purchaseOrderId (str):  Purchase Order Id
+            purchaseOrderId (uuid):  Purchase Order Id
                     
                     Example:
                     
                      - 8ad4b87b-9b47-4199-b0c3-5480745c6b41
             poLineNumbers (int): (default=1) Quantity of the PO line numbers
                     
                     Example:
                     
                      - 1
-            lang (str): (default=en) Requested language. Optional. [lang=en]
-                    
 
         Returns:
             dict: See Schema below
 
         Raises:
             OkapiRequestError: Bad Request
             OkapiFatalError: Server Error
@@ -1331,14 +1379,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - ["protectRead", "false"]
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -1460,14 +1513,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - ["acquisitionUnitId", "0ebb1f7d-983f-3026-8a4c-5318e0ebc041"]
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -1596,14 +1654,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - ["purchaseOrderId", "55b97a4a-6601-4488-84e1-8b0d47a3f523"]
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -1744,14 +1807,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - ["value", "Purchase At Vendor System", "="]
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -1855,38 +1923,31 @@
 
 class PoNumber(FolioApi):
     """Purchase Order Number
 
     **API used to manage PO number.  This API is intended for internal use only.  Please use the /orders/po-number API provided by mod-orders instead.**
     """
 
-    def get_poNumbers(self, **kwargs):
+    def get_poNumbers(self):
         """Get generated purchase order number
 
         ``GET /orders-storage/po-number``
 
-        Args:
-            **kwargs (properties): Keyword Arguments
-
-        Keyword Args:
-            lang (str): (default=en) Requested language. Optional. [lang=en]
-                    
-
         Returns:
             dict: See Schema below
 
         Raises:
             OkapiRequestError: Bad Request
             OkapiFatalError: Server Error
 
         Schema:
 
             .. literalinclude:: ../files/PoNumber_get_poNumbers_return.schema 
         """
-        return self.call("GET", "/orders-storage/po-number", query=kwargs)
+        return self.call("GET", "/orders-storage/po-number")
 
 
 class ReportingCode(FolioApi):
     """Reporting Code
 
     **CRUD APIs used to manage reporting codes.**
     """
@@ -1910,14 +1971,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - ["code", "MEDGRANT", "="]
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -2044,14 +2110,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - ["title", "TITLE", "="]
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/organizations.py` & `foliolib-0.3.3a1/foliolib/folio/api/organizations.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.organizations")
 
@@ -33,14 +33,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - status=="Active"
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -128,14 +133,15 @@
         Args:
             organizationsId (str)
             organization (dict): See Schema below
 
         Raises:
             OkapiRequestNotFound: Not Found
             OkapiRequestError: Bad Request
+            OkapiRequestConflict: Conflict
             OkapiFatalError: Server Error
 
         Schema:
 
             .. literalinclude:: ../files/Organizations_modify_organization_request.schema
         """
         return self.call("PUT", f"/organizations/organizations/{organizationsId}", data=organization)
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/organizationsStorage.py` & `foliolib-0.3.3a1/foliolib/folio/api/organizationsStorage.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.organizationsStorage")
 
@@ -33,14 +33,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - ["code", "MEDGRANT", "="]
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -128,14 +133,15 @@
         Args:
             organizationsId (str)
             organization (dict): See Schema below
 
         Raises:
             OkapiRequestNotFound: Not Found
             OkapiRequestError: Bad Request
+            OkapiRequestConflict: Conflict
             OkapiFatalError: Server Error
 
         Schema:
 
             .. literalinclude:: ../files/Organization_modify_organization_request.schema
         """
         return self.call("PUT", f"/organizations-storage/organizations/{organizationsId}", data=organization)
@@ -166,14 +172,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - ["code", "MEDGRANT", "="]
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -261,14 +272,15 @@
         Args:
             categoriesId (str)
             category (dict): See Schema below
 
         Raises:
             OkapiRequestNotFound: Not Found
             OkapiRequestError: Bad Request
+            OkapiRequestConflict: Conflict
             OkapiFatalError: Server Error
 
         Schema:
 
             .. literalinclude:: ../files/Category_modify_category_request.schema
         """
         return self.call("PUT", f"/organizations-storage/categories/{categoriesId}", data=category)
@@ -299,14 +311,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - ["code", "MEDGRANT", "="]
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -394,14 +411,15 @@
         Args:
             interfacesId (str)
             interface (dict): See Schema below
 
         Raises:
             OkapiRequestNotFound: Not Found
             OkapiRequestError: Bad Request
+            OkapiRequestConflict: Conflict
             OkapiFatalError: Server Error
 
         Schema:
 
             .. literalinclude:: ../files/Interface_modify_interface_request.schema
         """
         return self.call("PUT", f"/organizations-storage/interfaces/{interfacesId}", data=interface)
@@ -460,14 +478,15 @@
         Args:
             interfacesId (str)
             credential (dict): See Schema below
 
         Raises:
             OkapiRequestNotFound: Not Found
             OkapiRequestError: Bad Request
+            OkapiRequestConflict: Conflict
             OkapiFatalError: Server Error
 
         Schema:
 
             .. literalinclude:: ../files/Interface_modify_credential_request.schema
         """
         return self.call("PUT", f"/organizations-storage/interfaces/{interfacesId}/credentials", data=credential)
@@ -508,14 +527,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - ["code", "MEDGRANT", "="]
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -603,14 +627,15 @@
         Args:
             contactsId (str)
             contact (dict): See Schema below
 
         Raises:
             OkapiRequestNotFound: Not Found
             OkapiRequestError: Bad Request
+            OkapiRequestConflict: Conflict
             OkapiFatalError: Server Error
 
         Schema:
 
             .. literalinclude:: ../files/Contact_modify_contact_request.schema
         """
         return self.call("PUT", f"/organizations-storage/contacts/{contactsId}", data=contact)
@@ -642,14 +667,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - ["code", "MEDGRANT", "="]
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -737,14 +767,15 @@
         Args:
             emailsId (str)
             email (dict): See Schema below
 
         Raises:
             OkapiRequestNotFound: Not Found
             OkapiRequestError: Bad Request
+            OkapiRequestConflict: Conflict
             OkapiFatalError: Server Error
 
         Schema:
 
             .. literalinclude:: ../files/Email_modify_email_request.schema
         """
         return self.call("PUT", f"/organizations-storage/emails/{emailsId}", data=email)
@@ -776,14 +807,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - ["code", "MEDGRANT", "="]
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -871,14 +907,15 @@
         Args:
             urlsId (str)
             url (dict): See Schema below
 
         Raises:
             OkapiRequestNotFound: Not Found
             OkapiRequestError: Bad Request
+            OkapiRequestConflict: Conflict
             OkapiFatalError: Server Error
 
         Schema:
 
             .. literalinclude:: ../files/Url_modify_url_request.schema
         """
         return self.call("PUT", f"/organizations-storage/urls/{urlsId}", data=url)
@@ -910,14 +947,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - ["code", "MEDGRANT", "="]
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -1005,14 +1047,15 @@
         Args:
             addressesId (str)
             address (dict): See Schema below
 
         Raises:
             OkapiRequestNotFound: Not Found
             OkapiRequestError: Bad Request
+            OkapiRequestConflict: Conflict
             OkapiFatalError: Server Error
 
         Schema:
 
             .. literalinclude:: ../files/Address_modify_address_request.schema
         """
         return self.call("PUT", f"/organizations-storage/addresses/{addressesId}", data=address)
@@ -1043,14 +1086,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - status=Active
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -1140,14 +1188,15 @@
         Args:
             organizationTypesId (str)
             organizationType (dict): See Schema below
 
         Raises:
             OkapiRequestNotFound: Not Found
             OkapiRequestError: Bad Request
+            OkapiRequestConflict: Conflict
             OkapiFatalError: Server Error
             OkapiRequestUnprocessableEntity: Unprocessable Entity
 
         Schema:
 
             .. literalinclude:: ../files/OrganizationType_modify_organizationType_request.schema
         """
@@ -1180,14 +1229,19 @@
                     
                     
                     Example:
                     
                      - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
                     
                      - ["code", "MEDGRANT", "="]
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -1275,14 +1329,15 @@
         Args:
             phoneNumbersId (str)
             phoneNumber (dict): See Schema below
 
         Raises:
             OkapiRequestNotFound: Not Found
             OkapiRequestError: Bad Request
+            OkapiRequestConflict: Conflict
             OkapiFatalError: Server Error
 
         Schema:
 
             .. literalinclude:: ../files/PhoneNumber_modify_phoneNumber_request.schema
         """
         return self.call("PUT", f"/organizations-storage/phone-numbers/{phoneNumbersId}", data=phoneNumber)
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/passwordValidator.py` & `foliolib-0.3.3a1/foliolib/folio/api/passwordValidator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("foliolib.folio.api.passwordValidator")
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/patron.py` & `foliolib-0.3.3a1/foliolib/folio/api/patron.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.patron")
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/patronBlocks.py` & `foliolib-0.3.3a1/foliolib/folio/api/patronBlocks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.patronBlocks")
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/permissions.py` & `foliolib-0.3.3a1/foliolib/folio/api/permissions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.permissions")
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/pubsub.py` & `foliolib-0.3.3a1/foliolib/folio/api/pubsub.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.pubsub")
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/quickMarc.py` & `foliolib-0.3.3a1/foliolib/folio/api/quickMarc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("foliolib.folio.api.quickMarc")
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/remoteStorage.py` & `foliolib-0.3.3a1/foliolib/folio/api/remoteStorage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("foliolib.folio.api.remoteStorage")
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/rtac.py` & `foliolib-0.3.3a1/foliolib/folio/api/rtac.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.rtac")
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/search.py` & `foliolib-0.3.3a1/foliolib/folio/api/search.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("foliolib.folio.api.search")
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/sender.py` & `foliolib-0.3.3a1/foliolib/folio/api/sender.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.sender")
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/sharedIndex.py` & `foliolib-0.3.3a1/foliolib/folio/api/sharedIndex.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("foliolib.folio.api.sharedIndex")
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/sourceRecordManager.py` & `foliolib-0.3.3a1/foliolib/folio/api/sourceRecordManager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.sourceRecordManager")
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/sourceRecordStorage.py` & `foliolib-0.3.3a1/foliolib/folio/api/sourceRecordStorage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.sourceRecordStorage")
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/templateEngine.py` & `foliolib-0.3.3a1/foliolib/folio/api/templateEngine.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.templateEngine")
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/userImport.py` & `foliolib-0.3.3a1/foliolib/folio/api/userImport.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.userImport")
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/users.py` & `foliolib-0.3.3a1/foliolib/folio/api/users.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.users")
 
@@ -561,14 +561,21 @@
 
         Raises:
             OkapiRequestError: Bad Request
             OkapiFatalError: Server Error
         """
         return self.call("POST", "/users/expire/timer")
 
+    def set_process(self):
+        """Read audit events from DB and send them to Kafka
+
+        ``POST /users/outbox/process``
+        """
+        return self.call("POST", "/users/outbox/process")
+
 
 class Groups(FolioApi):
     """mod-users Groups API
 
     This documents the API calls that can be made to query and manage user groups of the system
     """
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/api/usersBl.py` & `foliolib-0.3.3a1/foliolib/folio/api/usersBl.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-02-10
+# Generated at 2023-04-16
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.usersBl")
```

### Comparing `foliolib-0.3.2a1/foliolib/folio/config.py` & `foliolib-0.3.3a1/foliolib/folio/config.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.2a1/foliolib/folio/dataImport.py` & `foliolib-0.3.3a1/foliolib/folio/dataImport.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.2a1/foliolib/folio/inventory.py` & `foliolib-0.3.3a1/foliolib/folio/inventory.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.2a1/foliolib/folio/inventoryReferenceData.py` & `foliolib-0.3.3a1/foliolib/folio/inventoryReferenceData.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.2a1/foliolib/folio/users.py` & `foliolib-0.3.3a1/foliolib/folio/users.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.2a1/foliolib/helper/__init__.py` & `foliolib-0.3.3a1/foliolib/helper/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 def get_node():
     from foliolib.okapi.okapiClient import OkapiClient
     try:
         nodes = OkapiClient().get_nodes()
     except:
         nodes = []
     try:
-        host = Config().okapicfg().get("Okapi", "host")
+        host = Config().servercfg().get("Okapi", "host")
     except:
         host = "localhost"
     try:
-        port = Config().okapicfg().get("Okapi", "port")
+        port = Config().servercfg().get("Okapi", "port")
     except:
         port = "9130"
     # If Okapi role is clustered
     for node in nodes:
         if "nodeName" in node:
             if f"{host}:{port}" in node["url"]:
                 return node["nodeName"]
```

### Comparing `foliolib-0.3.2a1/foliolib/helper/database.py` & `foliolib-0.3.3a1/foliolib/helper/database.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,21 +20,21 @@
 
     with Postgres(databas="okapi_modules") as pg:
         print(pg.get_schemas)
     """
 
     def __init__(self, user: str = None, password: str = None, database: str = "postgres",
                  host: str = None, port: str = None) -> None:
-        self._host = host or Config().okapicfg().get(
+        self._host = host or Config().servercfg().get(
             "Postgres", "host", fallback="localhost")
-        self._port = port or Config().okapicfg().get(
+        self._port = port or Config().servercfg().get(
             "Postgres", "port", fallback="5432")
-        self._user = user or Config().okapicfg().get(
+        self._user = user or Config().servercfg().get(
             "Postgres", "user", fallback="postgres")
-        self._password = password or Config().okapicfg().get(
+        self._password = password or Config().servercfg().get(
             "Postgres", "password", fallback="postgres")
         self._database = database
         self._con = None
 
     def open(self):
         try:
             log.info("Open postgres database %s on %s:%s with user %s:%s",
```

### Comparing `foliolib-0.3.2a1/foliolib/helper/folio.py` & `foliolib-0.3.3a1/foliolib/helper/folio.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.2a1/foliolib/helper/modules.py` & `foliolib-0.3.3a1/foliolib/helper/modules.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.2a1/foliolib/helper/okapi.py` & `foliolib-0.3.3a1/foliolib/helper/okapi.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.2a1/foliolib/helper/platform.py` & `foliolib-0.3.3a1/foliolib/helper/platform.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.2a1/foliolib/helper/tenant.py` & `foliolib-0.3.3a1/foliolib/helper/tenant.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.2a1/foliolib/okapi/__init__.py` & `foliolib-0.3.3a1/foliolib/okapi/__init__.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.2a1/foliolib/okapi/exceptions.py` & `foliolib-0.3.3a1/foliolib/okapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.2a1/foliolib/okapi/kubeClient.py` & `foliolib-0.3.3a1/foliolib/okapi/kubeClient.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,17 +28,17 @@
             kube_config (str)): Path to kube config. Defaults to None.
         """
         kube_config = kube_config or Config().get_kube_config()
         try:
             config.load_kube_config(config_file=kube_config)
         except ConfigException as e:
             log.error("Failed to load kube config %s", kube_config)
-        self._namespace = Config().okapicfg().get(
+        self._namespace = Config().servercfg().get(
             "Kubernetes", "namespace", fallback="default")
-        self._deploy_timeout = Config().okapicfg().getint(
+        self._deploy_timeout = Config().servercfg().getint(
             "Kubernetes", "deployTimeout", fallback=3600)
 
     def deploy(self, modId: str):
         """Deploy a Folio module
 
         Args:
             modId (str): Module id, e.g. mod-users-1.8.0
```

### Comparing `foliolib-0.3.2a1/foliolib/okapi/misc.py` & `foliolib-0.3.3a1/foliolib/okapi/misc.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.2a1/foliolib/okapi/okapiClient.py` & `foliolib-0.3.3a1/foliolib/okapi/okapiClient.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,19 +49,19 @@
 
     def __init__(self, host: str = None, port: str = None, path: str = None, ssl: bool = False) -> None:
         """
         Args:
             host (str, optional): IP or Hostame of the Okapi server. Defaults from foliolib.conf.
             port (str, optional):. Defaults from foliolib.conf.
         """
-        host = host or Config().okapicfg().get("Okapi", "host")
-        port = port or Config().okapicfg().get("Okapi", "port")
-        self._okapi_path = path or Config().okapicfg().get("Okapi", "path", fallback=None)
-        ssl = ssl or Config().okapicfg().getboolean("Okapi", "ssl", fallback=False)
-        self._verify_ssl = Config().okapicfg().getboolean(
+        host = host or Config().servercfg().get("Okapi", "host")
+        port = port or Config().servercfg().get("Okapi", "port")
+        self._okapi_path = path or Config().servercfg().get("Okapi", "path", fallback=None)
+        ssl = ssl or Config().servercfg().getboolean("Okapi", "ssl", fallback=False)
+        self._verify_ssl = Config().servercfg().getboolean(
             "Okapi", "verify_ssl", fallback=True)
 
         if ssl:
             self._host = f"https://{host}:{port}"
         else:
             self._host = f"http://{host}:{port}"
```

### Comparing `foliolib-0.3.2a1/foliolib/okapi/okapiModule.py` & `foliolib-0.3.3a1/foliolib/okapi/okapiModule.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.2a1/foliolib/okapi/okapiModuleKubernetes.py` & `foliolib-0.3.3a1/foliolib/okapi/okapiModuleKubernetes.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         self._memory = docker_args["memory"]
         self._port = docker_args["port"]
         self._protocol = docker_args["protocol"]
         self._env = module.get_env()
         self.healthCheck = True
         self.podAntiAffinity = True
         modcfg = Config().modulescfg(modId)
-        okapicfg = Config().okapicfg()
+        okapicfg = Config().servercfg()
         self._namespace = okapicfg.get(
             "Kubernetes", "namespace", fallback="default")
         self.imagePullSecret = okapicfg.get(
             "Kubernetes", "imagePullSecret", fallback=None)
 
         self._replicas = okapicfg.getint("Kubernetes", "replicas", fallback=1)
 
@@ -285,15 +285,15 @@
     def resources(self):
         conf = Config().modulescfg(self._modId)
         module = OkapiModule(self._modId)
         min_cpu = "10m"
         max_cpu = 0
         memory = module.get_docker_args()["memory"]
         if memory is not None:
-            memoryRequestPercentage = Config().okapicfg().getint(
+            memoryRequestPercentage = Config().servercfg().getint(
                 "Kubernetes", "memoryRequestPercentage", fallback=100)
             mk = math.ceil(memory/1024)
             min_mem = "%iKi" % ((mk * memoryRequestPercentage) / 100)
             max_mem = "%iKi" % mk
         else:
             log.warning(
                 "ModuleDescriptor for %s has no memory defined", self._modId)
```

### Comparing `foliolib-0.3.2a1/foliolib.egg-info/PKG-INFO` & `foliolib-0.3.3a1/foliolib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foliolib
-Version: 0.3.2a1
+Version: 0.3.3a1
 Summary: Okapi/Folio Manager and Library
 Home-page: https://github.com/tobi-weber/foliolib
 Author: Tobias Weber
 Author-email: tobi-weber@gmx.de
 License: GPL-3.0 License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `foliolib-0.3.2a1/foliolib.egg-info/SOURCES.txt` & `foliolib-0.3.3a1/foliolib.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -34,30 +34,29 @@
 foliolib/folio/dataImport.py
 foliolib/folio/exceptions.py
 foliolib/folio/inventory.py
 foliolib/folio/inventoryReferenceData.py
 foliolib/folio/users.py
 foliolib/folio/api/__init__.py
 foliolib/folio/api/audit.py
+foliolib/folio/api/bulkOperations.py
 foliolib/folio/api/calendar.py
 foliolib/folio/api/circulation.py
 foliolib/folio/api/circulationStorage.py
 foliolib/folio/api/configuration.py
 foliolib/folio/api/copycat.py
 foliolib/folio/api/courses.py
 foliolib/folio/api/dataExport.py
 foliolib/folio/api/dataExportSpring.py
 foliolib/folio/api/dataExportWorker.py
 foliolib/folio/api/dataImport.py
 foliolib/folio/api/dataImportConverterStorage.py
 foliolib/folio/api/ebsconet.py
-foliolib/folio/api/edgeCaiasoft.py
-foliolib/folio/api/edgeDematic.py
-foliolib/folio/api/edgeLtiCourses.py
 foliolib/folio/api/email.py
+foliolib/folio/api/entitiesLinks.py
 foliolib/folio/api/ermUsage.py
 foliolib/folio/api/ermUsageHarvester.py
 foliolib/folio/api/eventConfig.py
 foliolib/folio/api/feesfines.py
 foliolib/folio/api/finance.py
 foliolib/folio/api/financeStorage.py
 foliolib/folio/api/fincConfig.py
@@ -85,17 +84,19 @@
 foliolib/folio/api/passwordValidator.py
 foliolib/folio/api/patron.py
 foliolib/folio/api/patronBlocks.py
 foliolib/folio/api/permissions.py
 foliolib/folio/api/pubsub.py
 foliolib/folio/api/quickMarc.py
 foliolib/folio/api/remoteStorage.py
+foliolib/folio/api/reservoir.py
 foliolib/folio/api/rtac.py
 foliolib/folio/api/search.py
 foliolib/folio/api/sender.py
+foliolib/folio/api/settings.py
 foliolib/folio/api/sharedIndex.py
 foliolib/folio/api/sourceRecordManager.py
 foliolib/folio/api/sourceRecordStorage.py
 foliolib/folio/api/tags.py
 foliolib/folio/api/templateEngine.py
 foliolib/folio/api/userImport.py
 foliolib/folio/api/users.py
```

### Comparing `foliolib-0.3.2a1/setup.cfg` & `foliolib-0.3.3a1/setup.cfg`

 * *Files identical despite different names*

