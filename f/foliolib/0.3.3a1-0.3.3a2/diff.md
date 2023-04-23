# Comparing `tmp/foliolib-0.3.3a1.tar.gz` & `tmp/foliolib-0.3.3a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foliolib-0.3.3a1.tar", last modified: Sun Apr 23 06:38:47 2023, max compression
+gzip compressed data, was "foliolib-0.3.3a2.tar", last modified: Sun Apr 23 06:42:51 2023, max compression
```

## Comparing `foliolib-0.3.3a1.tar` & `foliolib-0.3.3a2.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-04-23 06:38:47.864991 foliolib-0.3.3a1/
--rw-r--r--   0 tobi      (1000) tobi      (1000)    35146 2020-10-11 07:41:52.000000 foliolib-0.3.3a1/COPYING
--rw-r--r--   0 tobi      (1000) tobi      (1000)       43 2020-11-07 12:13:21.000000 foliolib-0.3.3a1/MANIFEST.in
--rw-r--r--   0 tobi      (1000) tobi      (1000)     2357 2023-04-23 06:38:47.864991 foliolib-0.3.3a1/PKG-INFO
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1719 2023-02-21 11:23:02.000000 foliolib-0.3.3a1/README.rst
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-04-23 06:38:47.840991 foliolib-0.3.3a1/foliolib/
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1031 2023-03-24 13:25:47.000000 foliolib-0.3.3a1/foliolib/__init__.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      396 2023-04-23 06:38:47.000000 foliolib-0.3.3a1/foliolib/__version__.py
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-04-23 06:38:47.840991 foliolib-0.3.3a1/foliolib/apiBuilder/
--rw-r--r--   0 tobi      (1000) tobi      (1000)      351 2022-10-11 12:37:16.000000 foliolib-0.3.3a1/foliolib/apiBuilder/__init__.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1288 2022-03-13 04:11:25.000000 foliolib-0.3.3a1/foliolib/apiBuilder/build_api.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1586 2022-05-04 20:18:39.000000 foliolib-0.3.3a1/foliolib/apiBuilder/cli.py
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-04-23 06:38:47.844991 foliolib-0.3.3a1/foliolib/cli/
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3821 2023-04-21 06:17:59.000000 foliolib-0.3.3a1/foliolib/cli/__init__.py
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-04-23 06:38:47.844991 foliolib-0.3.3a1/foliolib/cli/folio/
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1461 2022-05-09 17:53:56.000000 foliolib-0.3.3a1/foliolib/cli/folio/__init__.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      229 2022-04-05 13:20:51.000000 foliolib-0.3.3a1/foliolib/cli/folio/inventory.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      634 2022-02-21 04:57:32.000000 foliolib-0.3.3a1/foliolib/cli/main.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      374 2022-02-21 04:57:41.000000 foliolib-0.3.3a1/foliolib/cli/main_err.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      895 2022-02-21 04:57:36.000000 foliolib-0.3.3a1/foliolib/cli/main_noauth.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     4591 2023-04-15 04:58:38.000000 foliolib-0.3.3a1/foliolib/cli/module.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3495 2023-04-01 07:43:09.000000 foliolib-0.3.3a1/foliolib/cli/okapi.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      446 2022-02-21 04:57:17.000000 foliolib-0.3.3a1/foliolib/cli/orderedGroup.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3680 2023-02-15 15:06:27.000000 foliolib-0.3.3a1/foliolib/cli/platform.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     2759 2023-04-21 05:25:46.000000 foliolib-0.3.3a1/foliolib/cli/server.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    12868 2022-10-06 05:29:03.000000 foliolib-0.3.3a1/foliolib/cli/tenant.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    12088 2023-04-21 06:26:30.000000 foliolib-0.3.3a1/foliolib/config.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      801 2022-05-09 17:52:49.000000 foliolib-0.3.3a1/foliolib/exceptions.py
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-04-23 06:38:47.844991 foliolib-0.3.3a1/foliolib/folio/
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1870 2022-10-06 05:35:01.000000 foliolib-0.3.3a1/foliolib/folio/__init__.py
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-04-23 06:38:47.860991 foliolib-0.3.3a1/foliolib/folio/api/
--rw-r--r--   0 tobi      (1000) tobi      (1000)        0 2021-11-15 08:23:39.000000 foliolib-0.3.3a1/foliolib/folio/api/__init__.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     9675 2023-04-16 06:50:57.000000 foliolib-0.3.3a1/foliolib/folio/api/audit.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     6883 2023-04-16 06:50:57.000000 foliolib-0.3.3a1/foliolib/folio/api/bulkOperations.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      173 2023-04-16 06:50:57.000000 foliolib-0.3.3a1/foliolib/folio/api/calendar.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    40174 2023-04-16 06:50:57.000000 foliolib-0.3.3a1/foliolib/folio/api/circulation.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    73691 2023-04-16 06:50:57.000000 foliolib-0.3.3a1/foliolib/folio/api/circulationStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     6506 2023-04-16 06:50:57.000000 foliolib-0.3.3a1/foliolib/folio/api/configuration.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     4913 2023-04-16 06:50:57.000000 foliolib-0.3.3a1/foliolib/folio/api/copycat.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    54009 2023-04-16 06:50:58.000000 foliolib-0.3.3a1/foliolib/folio/api/courses.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    19883 2023-04-16 06:50:58.000000 foliolib-0.3.3a1/foliolib/folio/api/dataExport.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     6764 2023-04-16 06:50:58.000000 foliolib-0.3.3a1/foliolib/folio/api/dataExportSpring.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     5642 2023-04-16 06:50:58.000000 foliolib-0.3.3a1/foliolib/folio/api/dataExportWorker.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    13485 2023-04-16 06:50:58.000000 foliolib-0.3.3a1/foliolib/folio/api/dataImport.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    37645 2023-04-16 06:50:58.000000 foliolib-0.3.3a1/foliolib/folio/api/dataImportConverterStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     2268 2023-04-16 06:50:58.000000 foliolib-0.3.3a1/foliolib/folio/api/ebsconet.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     7884 2023-04-16 06:50:58.000000 foliolib-0.3.3a1/foliolib/folio/api/email.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     4399 2023-04-16 06:50:58.000000 foliolib-0.3.3a1/foliolib/folio/api/entitiesLinks.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    25152 2023-04-16 06:50:58.000000 foliolib-0.3.3a1/foliolib/folio/api/ermUsage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     4482 2023-04-16 06:50:58.000000 foliolib-0.3.3a1/foliolib/folio/api/ermUsageHarvester.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     4273 2023-04-16 06:50:58.000000 foliolib-0.3.3a1/foliolib/folio/api/eventConfig.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    80620 2023-04-16 06:50:59.000000 foliolib-0.3.3a1/foliolib/folio/api/feesfines.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    76479 2023-04-16 06:50:59.000000 foliolib-0.3.3a1/foliolib/folio/api/finance.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    79172 2023-04-16 06:50:59.000000 foliolib-0.3.3a1/foliolib/folio/api/financeStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    51717 2023-04-16 06:50:59.000000 foliolib-0.3.3a1/foliolib/folio/api/fincConfig.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     8283 2023-04-16 06:51:00.000000 foliolib-0.3.3a1/foliolib/folio/api/gobi.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    76551 2023-04-16 06:51:02.000000 foliolib-0.3.3a1/foliolib/folio/api/innReach.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    22929 2023-04-16 06:51:02.000000 foliolib-0.3.3a1/foliolib/folio/api/inventory.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)   217418 2023-04-16 06:51:03.000000 foliolib-0.3.3a1/foliolib/folio/api/inventoryStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     6001 2023-04-16 06:51:03.000000 foliolib-0.3.3a1/foliolib/folio/api/inventoryUpdate.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    45051 2023-04-16 06:51:03.000000 foliolib-0.3.3a1/foliolib/folio/api/invoice.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    47143 2023-04-16 06:51:03.000000 foliolib-0.3.3a1/foliolib/folio/api/invoiceStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    54294 2023-04-16 06:51:03.000000 foliolib-0.3.3a1/foliolib/folio/api/kbEbscoJava.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3051 2023-04-16 06:51:03.000000 foliolib-0.3.3a1/foliolib/folio/api/ldp.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1332 2023-04-16 06:51:03.000000 foliolib-0.3.3a1/foliolib/folio/api/licenses.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     8538 2023-04-16 06:51:03.000000 foliolib-0.3.3a1/foliolib/folio/api/login.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     4260 2023-04-16 06:51:03.000000 foliolib-0.3.3a1/foliolib/folio/api/loginSaml.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    17932 2023-04-16 06:51:03.000000 foliolib-0.3.3a1/foliolib/folio/api/marccat.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    20392 2023-04-16 06:51:04.000000 foliolib-0.3.3a1/foliolib/folio/api/metaStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      171 2023-04-16 06:51:04.000000 foliolib-0.3.3a1/foliolib/folio/api/notes.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     8870 2023-04-16 06:51:04.000000 foliolib-0.3.3a1/foliolib/folio/api/notify.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    12105 2023-04-16 06:51:04.000000 foliolib-0.3.3a1/foliolib/folio/api/oaiPmh.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    63105 2023-04-16 06:51:04.000000 foliolib-0.3.3a1/foliolib/folio/api/orders.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    78262 2023-04-16 06:51:04.000000 foliolib-0.3.3a1/foliolib/folio/api/ordersStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     4978 2023-04-16 06:51:04.000000 foliolib-0.3.3a1/foliolib/folio/api/organizations.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    45825 2023-04-16 06:51:04.000000 foliolib-0.3.3a1/foliolib/folio/api/organizationsStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3678 2023-04-16 06:51:04.000000 foliolib-0.3.3a1/foliolib/folio/api/passwordValidator.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     5893 2023-04-16 06:51:04.000000 foliolib-0.3.3a1/foliolib/folio/api/patron.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    15601 2023-04-16 06:51:04.000000 foliolib-0.3.3a1/foliolib/folio/api/patronBlocks.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    14392 2023-04-16 06:51:04.000000 foliolib-0.3.3a1/foliolib/folio/api/permissions.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     9093 2023-04-16 06:51:04.000000 foliolib-0.3.3a1/foliolib/folio/api/pubsub.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     4445 2023-04-16 06:51:05.000000 foliolib-0.3.3a1/foliolib/folio/api/quickMarc.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    17286 2023-04-16 06:51:05.000000 foliolib-0.3.3a1/foliolib/folio/api/remoteStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    21589 2023-04-16 06:51:05.000000 foliolib-0.3.3a1/foliolib/folio/api/reservoir.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1928 2023-04-16 06:51:05.000000 foliolib-0.3.3a1/foliolib/folio/api/rtac.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    17486 2023-04-16 06:51:05.000000 foliolib-0.3.3a1/foliolib/folio/api/search.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      732 2023-04-16 06:51:05.000000 foliolib-0.3.3a1/foliolib/folio/api/sender.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     5425 2023-04-16 06:51:05.000000 foliolib-0.3.3a1/foliolib/folio/api/settings.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    11154 2023-04-16 06:51:05.000000 foliolib-0.3.3a1/foliolib/folio/api/sharedIndex.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    21352 2023-04-16 06:51:05.000000 foliolib-0.3.3a1/foliolib/folio/api/sourceRecordManager.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    24923 2023-04-16 06:51:05.000000 foliolib-0.3.3a1/foliolib/folio/api/sourceRecordStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      170 2023-04-16 06:51:05.000000 foliolib-0.3.3a1/foliolib/folio/api/tags.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     4091 2023-04-16 06:51:05.000000 foliolib-0.3.3a1/foliolib/folio/api/templateEngine.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      870 2023-04-16 06:51:05.000000 foliolib-0.3.3a1/foliolib/folio/api/userImport.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    22806 2023-04-16 06:51:05.000000 foliolib-0.3.3a1/foliolib/folio/api/users.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    11127 2023-04-16 06:51:05.000000 foliolib-0.3.3a1/foliolib/folio/api/usersBl.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     5803 2022-05-31 09:32:11.000000 foliolib-0.3.3a1/foliolib/folio/config.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     8495 2021-02-25 09:49:29.000000 foliolib-0.3.3a1/foliolib/folio/dataImport.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      436 2022-03-17 02:39:17.000000 foliolib-0.3.3a1/foliolib/folio/exceptions.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      945 2022-04-08 08:56:47.000000 foliolib-0.3.3a1/foliolib/folio/inventory.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    24056 2022-09-15 02:29:53.000000 foliolib-0.3.3a1/foliolib/folio/inventoryReferenceData.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     9488 2022-06-03 04:45:10.000000 foliolib-0.3.3a1/foliolib/folio/users.py
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-04-23 06:38:47.860991 foliolib-0.3.3a1/foliolib/helper/
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1207 2023-04-21 05:23:46.000000 foliolib-0.3.3a1/foliolib/helper/__init__.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     9311 2023-04-21 05:23:46.000000 foliolib-0.3.3a1/foliolib/helper/database.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3636 2022-10-11 03:50:00.000000 foliolib-0.3.3a1/foliolib/helper/folio.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3055 2023-02-09 19:10:16.000000 foliolib-0.3.3a1/foliolib/helper/modules.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3935 2023-04-01 06:20:04.000000 foliolib-0.3.3a1/foliolib/helper/okapi.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     5714 2023-02-18 17:54:00.000000 foliolib-0.3.3a1/foliolib/helper/platform.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1517 2022-10-11 03:48:54.000000 foliolib-0.3.3a1/foliolib/helper/tenant.py
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-04-23 06:38:47.864991 foliolib-0.3.3a1/foliolib/okapi/
--rw-r--r--   0 tobi      (1000) tobi      (1000)    14520 2022-10-13 08:48:51.000000 foliolib-0.3.3a1/foliolib/okapi/__init__.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     2399 2022-07-24 04:45:10.000000 foliolib-0.3.3a1/foliolib/okapi/exceptions.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    16267 2023-04-21 05:23:46.000000 foliolib-0.3.3a1/foliolib/okapi/kubeClient.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      542 2022-03-22 15:04:58.000000 foliolib-0.3.3a1/foliolib/okapi/misc.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    38800 2023-04-21 05:23:46.000000 foliolib-0.3.3a1/foliolib/okapi/okapiClient.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    10030 2023-02-02 10:53:21.000000 foliolib-0.3.3a1/foliolib/okapi/okapiModule.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    17121 2023-04-21 05:23:46.000000 foliolib-0.3.3a1/foliolib/okapi/okapiModuleKubernetes.py
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-04-23 06:38:47.840991 foliolib-0.3.3a1/foliolib.egg-info/
--rw-r--r--   0 tobi      (1000) tobi      (1000)     2357 2023-04-23 06:38:47.000000 foliolib-0.3.3a1/foliolib.egg-info/PKG-INFO
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3502 2023-04-23 06:38:47.000000 foliolib-0.3.3a1/foliolib.egg-info/SOURCES.txt
--rw-r--r--   0 tobi      (1000) tobi      (1000)        1 2023-04-23 06:38:47.000000 foliolib-0.3.3a1/foliolib.egg-info/dependency_links.txt
--rw-r--r--   0 tobi      (1000) tobi      (1000)       88 2023-04-23 06:38:47.000000 foliolib-0.3.3a1/foliolib.egg-info/entry_points.txt
--rw-r--r--   0 tobi      (1000) tobi      (1000)      130 2023-04-23 06:38:47.000000 foliolib-0.3.3a1/foliolib.egg-info/requires.txt
--rw-r--r--   0 tobi      (1000) tobi      (1000)      126 2023-04-23 06:38:47.000000 foliolib-0.3.3a1/foliolib.egg-info/top_level.txt
--rw-r--r--   0 tobi      (1000) tobi      (1000)      305 2023-02-21 08:41:56.000000 foliolib-0.3.3a1/requirements.txt
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1145 2023-04-23 06:38:47.864991 foliolib-0.3.3a1/setup.cfg
--rw-r--r--   0 tobi      (1000) tobi      (1000)      117 2022-10-11 12:39:31.000000 foliolib-0.3.3a1/setup.py
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-04-23 06:42:51.256268 foliolib-0.3.3a2/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    35146 2020-10-11 07:41:52.000000 foliolib-0.3.3a2/COPYING
+-rw-r--r--   0 tobi      (1000) tobi      (1000)       43 2020-11-07 12:13:21.000000 foliolib-0.3.3a2/MANIFEST.in
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     2357 2023-04-23 06:42:51.256268 foliolib-0.3.3a2/PKG-INFO
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1719 2023-02-21 11:23:02.000000 foliolib-0.3.3a2/README.rst
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-04-23 06:42:51.248268 foliolib-0.3.3a2/foliolib/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1031 2023-03-24 13:25:47.000000 foliolib-0.3.3a2/foliolib/__init__.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      396 2023-04-23 06:42:50.000000 foliolib-0.3.3a2/foliolib/__version__.py
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-04-23 06:42:51.248268 foliolib-0.3.3a2/foliolib/apiBuilder/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      351 2022-10-11 12:37:16.000000 foliolib-0.3.3a2/foliolib/apiBuilder/__init__.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1288 2022-03-13 04:11:25.000000 foliolib-0.3.3a2/foliolib/apiBuilder/build_api.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1586 2022-05-04 20:18:39.000000 foliolib-0.3.3a2/foliolib/apiBuilder/cli.py
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-04-23 06:42:51.252268 foliolib-0.3.3a2/foliolib/cli/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3821 2023-04-21 06:17:59.000000 foliolib-0.3.3a2/foliolib/cli/__init__.py
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-04-23 06:42:51.252268 foliolib-0.3.3a2/foliolib/cli/folio/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1461 2022-05-09 17:53:56.000000 foliolib-0.3.3a2/foliolib/cli/folio/__init__.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      229 2022-04-05 13:20:51.000000 foliolib-0.3.3a2/foliolib/cli/folio/inventory.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      634 2022-02-21 04:57:32.000000 foliolib-0.3.3a2/foliolib/cli/main.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      374 2022-02-21 04:57:41.000000 foliolib-0.3.3a2/foliolib/cli/main_err.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      895 2022-02-21 04:57:36.000000 foliolib-0.3.3a2/foliolib/cli/main_noauth.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     4591 2023-04-15 04:58:38.000000 foliolib-0.3.3a2/foliolib/cli/module.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3495 2023-04-01 07:43:09.000000 foliolib-0.3.3a2/foliolib/cli/okapi.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      446 2022-02-21 04:57:17.000000 foliolib-0.3.3a2/foliolib/cli/orderedGroup.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3680 2023-02-15 15:06:27.000000 foliolib-0.3.3a2/foliolib/cli/platform.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     2759 2023-04-21 05:25:46.000000 foliolib-0.3.3a2/foliolib/cli/server.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    12868 2022-10-06 05:29:03.000000 foliolib-0.3.3a2/foliolib/cli/tenant.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    12088 2023-04-21 06:26:30.000000 foliolib-0.3.3a2/foliolib/config.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      801 2022-05-09 17:52:49.000000 foliolib-0.3.3a2/foliolib/exceptions.py
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-04-23 06:42:51.252268 foliolib-0.3.3a2/foliolib/folio/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1870 2022-10-06 05:35:01.000000 foliolib-0.3.3a2/foliolib/folio/__init__.py
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-04-23 06:42:51.256268 foliolib-0.3.3a2/foliolib/folio/api/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)        0 2021-11-15 08:23:39.000000 foliolib-0.3.3a2/foliolib/folio/api/__init__.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     9675 2023-04-16 06:50:57.000000 foliolib-0.3.3a2/foliolib/folio/api/audit.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     6883 2023-04-16 06:50:57.000000 foliolib-0.3.3a2/foliolib/folio/api/bulkOperations.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      173 2023-04-16 06:50:57.000000 foliolib-0.3.3a2/foliolib/folio/api/calendar.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    40174 2023-04-16 06:50:57.000000 foliolib-0.3.3a2/foliolib/folio/api/circulation.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    73691 2023-04-16 06:50:57.000000 foliolib-0.3.3a2/foliolib/folio/api/circulationStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     6506 2023-04-16 06:50:57.000000 foliolib-0.3.3a2/foliolib/folio/api/configuration.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     4913 2023-04-16 06:50:57.000000 foliolib-0.3.3a2/foliolib/folio/api/copycat.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    54009 2023-04-16 06:50:58.000000 foliolib-0.3.3a2/foliolib/folio/api/courses.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    19883 2023-04-16 06:50:58.000000 foliolib-0.3.3a2/foliolib/folio/api/dataExport.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     6764 2023-04-16 06:50:58.000000 foliolib-0.3.3a2/foliolib/folio/api/dataExportSpring.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     5642 2023-04-16 06:50:58.000000 foliolib-0.3.3a2/foliolib/folio/api/dataExportWorker.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    13485 2023-04-16 06:50:58.000000 foliolib-0.3.3a2/foliolib/folio/api/dataImport.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    37645 2023-04-16 06:50:58.000000 foliolib-0.3.3a2/foliolib/folio/api/dataImportConverterStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     2268 2023-04-16 06:50:58.000000 foliolib-0.3.3a2/foliolib/folio/api/ebsconet.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     7884 2023-04-16 06:50:58.000000 foliolib-0.3.3a2/foliolib/folio/api/email.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     4399 2023-04-16 06:50:58.000000 foliolib-0.3.3a2/foliolib/folio/api/entitiesLinks.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    25152 2023-04-16 06:50:58.000000 foliolib-0.3.3a2/foliolib/folio/api/ermUsage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     4482 2023-04-16 06:50:58.000000 foliolib-0.3.3a2/foliolib/folio/api/ermUsageHarvester.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     4273 2023-04-16 06:50:58.000000 foliolib-0.3.3a2/foliolib/folio/api/eventConfig.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    80620 2023-04-16 06:50:59.000000 foliolib-0.3.3a2/foliolib/folio/api/feesfines.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    76479 2023-04-16 06:50:59.000000 foliolib-0.3.3a2/foliolib/folio/api/finance.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    79172 2023-04-16 06:50:59.000000 foliolib-0.3.3a2/foliolib/folio/api/financeStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    51717 2023-04-16 06:50:59.000000 foliolib-0.3.3a2/foliolib/folio/api/fincConfig.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     8283 2023-04-16 06:51:00.000000 foliolib-0.3.3a2/foliolib/folio/api/gobi.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    76551 2023-04-16 06:51:02.000000 foliolib-0.3.3a2/foliolib/folio/api/innReach.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    22929 2023-04-16 06:51:02.000000 foliolib-0.3.3a2/foliolib/folio/api/inventory.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)   217418 2023-04-16 06:51:03.000000 foliolib-0.3.3a2/foliolib/folio/api/inventoryStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     6001 2023-04-16 06:51:03.000000 foliolib-0.3.3a2/foliolib/folio/api/inventoryUpdate.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    45051 2023-04-16 06:51:03.000000 foliolib-0.3.3a2/foliolib/folio/api/invoice.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    47143 2023-04-16 06:51:03.000000 foliolib-0.3.3a2/foliolib/folio/api/invoiceStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    54294 2023-04-16 06:51:03.000000 foliolib-0.3.3a2/foliolib/folio/api/kbEbscoJava.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3051 2023-04-16 06:51:03.000000 foliolib-0.3.3a2/foliolib/folio/api/ldp.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1332 2023-04-16 06:51:03.000000 foliolib-0.3.3a2/foliolib/folio/api/licenses.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     8538 2023-04-16 06:51:03.000000 foliolib-0.3.3a2/foliolib/folio/api/login.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     4260 2023-04-16 06:51:03.000000 foliolib-0.3.3a2/foliolib/folio/api/loginSaml.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    17932 2023-04-16 06:51:03.000000 foliolib-0.3.3a2/foliolib/folio/api/marccat.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    20392 2023-04-16 06:51:04.000000 foliolib-0.3.3a2/foliolib/folio/api/metaStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      171 2023-04-16 06:51:04.000000 foliolib-0.3.3a2/foliolib/folio/api/notes.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     8870 2023-04-16 06:51:04.000000 foliolib-0.3.3a2/foliolib/folio/api/notify.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    12105 2023-04-16 06:51:04.000000 foliolib-0.3.3a2/foliolib/folio/api/oaiPmh.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    63105 2023-04-16 06:51:04.000000 foliolib-0.3.3a2/foliolib/folio/api/orders.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    78262 2023-04-16 06:51:04.000000 foliolib-0.3.3a2/foliolib/folio/api/ordersStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     4978 2023-04-16 06:51:04.000000 foliolib-0.3.3a2/foliolib/folio/api/organizations.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    45825 2023-04-16 06:51:04.000000 foliolib-0.3.3a2/foliolib/folio/api/organizationsStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3678 2023-04-16 06:51:04.000000 foliolib-0.3.3a2/foliolib/folio/api/passwordValidator.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     5893 2023-04-16 06:51:04.000000 foliolib-0.3.3a2/foliolib/folio/api/patron.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    15601 2023-04-16 06:51:04.000000 foliolib-0.3.3a2/foliolib/folio/api/patronBlocks.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    14392 2023-04-16 06:51:04.000000 foliolib-0.3.3a2/foliolib/folio/api/permissions.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     9093 2023-04-16 06:51:04.000000 foliolib-0.3.3a2/foliolib/folio/api/pubsub.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     4445 2023-04-16 06:51:05.000000 foliolib-0.3.3a2/foliolib/folio/api/quickMarc.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    17286 2023-04-16 06:51:05.000000 foliolib-0.3.3a2/foliolib/folio/api/remoteStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    21589 2023-04-16 06:51:05.000000 foliolib-0.3.3a2/foliolib/folio/api/reservoir.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1928 2023-04-16 06:51:05.000000 foliolib-0.3.3a2/foliolib/folio/api/rtac.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    17486 2023-04-16 06:51:05.000000 foliolib-0.3.3a2/foliolib/folio/api/search.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      732 2023-04-16 06:51:05.000000 foliolib-0.3.3a2/foliolib/folio/api/sender.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     5425 2023-04-16 06:51:05.000000 foliolib-0.3.3a2/foliolib/folio/api/settings.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    11154 2023-04-16 06:51:05.000000 foliolib-0.3.3a2/foliolib/folio/api/sharedIndex.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    21352 2023-04-16 06:51:05.000000 foliolib-0.3.3a2/foliolib/folio/api/sourceRecordManager.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    24923 2023-04-16 06:51:05.000000 foliolib-0.3.3a2/foliolib/folio/api/sourceRecordStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      170 2023-04-16 06:51:05.000000 foliolib-0.3.3a2/foliolib/folio/api/tags.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     4091 2023-04-16 06:51:05.000000 foliolib-0.3.3a2/foliolib/folio/api/templateEngine.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      870 2023-04-16 06:51:05.000000 foliolib-0.3.3a2/foliolib/folio/api/userImport.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    22806 2023-04-16 06:51:05.000000 foliolib-0.3.3a2/foliolib/folio/api/users.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    11127 2023-04-16 06:51:05.000000 foliolib-0.3.3a2/foliolib/folio/api/usersBl.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     5803 2022-05-31 09:32:11.000000 foliolib-0.3.3a2/foliolib/folio/config.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     8495 2021-02-25 09:49:29.000000 foliolib-0.3.3a2/foliolib/folio/dataImport.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      436 2022-03-17 02:39:17.000000 foliolib-0.3.3a2/foliolib/folio/exceptions.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      945 2022-04-08 08:56:47.000000 foliolib-0.3.3a2/foliolib/folio/inventory.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    24056 2022-09-15 02:29:53.000000 foliolib-0.3.3a2/foliolib/folio/inventoryReferenceData.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     9488 2022-06-03 04:45:10.000000 foliolib-0.3.3a2/foliolib/folio/users.py
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-04-23 06:42:51.256268 foliolib-0.3.3a2/foliolib/helper/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1207 2023-04-21 05:23:46.000000 foliolib-0.3.3a2/foliolib/helper/__init__.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     9311 2023-04-21 05:23:46.000000 foliolib-0.3.3a2/foliolib/helper/database.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3636 2022-10-11 03:50:00.000000 foliolib-0.3.3a2/foliolib/helper/folio.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3055 2023-02-09 19:10:16.000000 foliolib-0.3.3a2/foliolib/helper/modules.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3935 2023-04-01 06:20:04.000000 foliolib-0.3.3a2/foliolib/helper/okapi.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     5714 2023-02-18 17:54:00.000000 foliolib-0.3.3a2/foliolib/helper/platform.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1517 2022-10-11 03:48:54.000000 foliolib-0.3.3a2/foliolib/helper/tenant.py
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-04-23 06:42:51.256268 foliolib-0.3.3a2/foliolib/okapi/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    14520 2022-10-13 08:48:51.000000 foliolib-0.3.3a2/foliolib/okapi/__init__.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     2399 2022-07-24 04:45:10.000000 foliolib-0.3.3a2/foliolib/okapi/exceptions.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    16267 2023-04-21 05:23:46.000000 foliolib-0.3.3a2/foliolib/okapi/kubeClient.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      542 2022-03-22 15:04:58.000000 foliolib-0.3.3a2/foliolib/okapi/misc.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    38800 2023-04-21 05:23:46.000000 foliolib-0.3.3a2/foliolib/okapi/okapiClient.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    10030 2023-02-02 10:53:21.000000 foliolib-0.3.3a2/foliolib/okapi/okapiModule.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    17121 2023-04-21 05:23:46.000000 foliolib-0.3.3a2/foliolib/okapi/okapiModuleKubernetes.py
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-04-23 06:42:51.248268 foliolib-0.3.3a2/foliolib.egg-info/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     2357 2023-04-23 06:42:51.000000 foliolib-0.3.3a2/foliolib.egg-info/PKG-INFO
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3502 2023-04-23 06:42:51.000000 foliolib-0.3.3a2/foliolib.egg-info/SOURCES.txt
+-rw-r--r--   0 tobi      (1000) tobi      (1000)        1 2023-04-23 06:42:51.000000 foliolib-0.3.3a2/foliolib.egg-info/dependency_links.txt
+-rw-r--r--   0 tobi      (1000) tobi      (1000)       88 2023-04-23 06:42:51.000000 foliolib-0.3.3a2/foliolib.egg-info/entry_points.txt
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      130 2023-04-23 06:42:51.000000 foliolib-0.3.3a2/foliolib.egg-info/requires.txt
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      126 2023-04-23 06:42:51.000000 foliolib-0.3.3a2/foliolib.egg-info/top_level.txt
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      305 2023-02-21 08:41:56.000000 foliolib-0.3.3a2/requirements.txt
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1145 2023-04-23 06:42:51.260268 foliolib-0.3.3a2/setup.cfg
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      117 2022-10-11 12:39:31.000000 foliolib-0.3.3a2/setup.py
```

### Comparing `foliolib-0.3.3a1/COPYING` & `foliolib-0.3.3a2/COPYING`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/PKG-INFO` & `foliolib-0.3.3a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foliolib
-Version: 0.3.3a1
+Version: 0.3.3a2
 Summary: Okapi/Folio Manager and Library
 Home-page: https://github.com/tobi-weber/foliolib
 Author: Tobias Weber
 Author-email: tobi-weber@gmx.de
 License: GPL-3.0 License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `foliolib-0.3.3a1/README.rst` & `foliolib-0.3.3a2/README.rst`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/__init__.py` & `foliolib-0.3.3a2/foliolib/__init__.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/apiBuilder/build_api.py` & `foliolib-0.3.3a2/foliolib/apiBuilder/build_api.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/apiBuilder/cli.py` & `foliolib-0.3.3a2/foliolib/apiBuilder/cli.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/cli/__init__.py` & `foliolib-0.3.3a2/foliolib/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/cli/folio/__init__.py` & `foliolib-0.3.3a2/foliolib/cli/folio/__init__.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/cli/main.py` & `foliolib-0.3.3a2/foliolib/cli/main.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/cli/main_noauth.py` & `foliolib-0.3.3a2/foliolib/cli/main_noauth.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/cli/module.py` & `foliolib-0.3.3a2/foliolib/cli/module.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/cli/okapi.py` & `foliolib-0.3.3a2/foliolib/cli/okapi.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/cli/platform.py` & `foliolib-0.3.3a2/foliolib/cli/platform.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/cli/server.py` & `foliolib-0.3.3a2/foliolib/cli/server.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/cli/tenant.py` & `foliolib-0.3.3a2/foliolib/cli/tenant.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/config.py` & `foliolib-0.3.3a2/foliolib/config.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/exceptions.py` & `foliolib-0.3.3a2/foliolib/exceptions.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/__init__.py` & `foliolib-0.3.3a2/foliolib/folio/__init__.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/audit.py` & `foliolib-0.3.3a2/foliolib/folio/api/audit.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/bulkOperations.py` & `foliolib-0.3.3a2/foliolib/folio/api/bulkOperations.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/circulation.py` & `foliolib-0.3.3a2/foliolib/folio/api/circulation.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/circulationStorage.py` & `foliolib-0.3.3a2/foliolib/folio/api/circulationStorage.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/configuration.py` & `foliolib-0.3.3a2/foliolib/folio/api/configuration.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/copycat.py` & `foliolib-0.3.3a2/foliolib/folio/api/copycat.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/courses.py` & `foliolib-0.3.3a2/foliolib/folio/api/courses.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/dataExport.py` & `foliolib-0.3.3a2/foliolib/folio/api/dataExport.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/dataExportSpring.py` & `foliolib-0.3.3a2/foliolib/folio/api/dataExportSpring.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/dataExportWorker.py` & `foliolib-0.3.3a2/foliolib/folio/api/dataExportWorker.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/dataImport.py` & `foliolib-0.3.3a2/foliolib/folio/api/dataImport.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/dataImportConverterStorage.py` & `foliolib-0.3.3a2/foliolib/folio/api/dataImportConverterStorage.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/ebsconet.py` & `foliolib-0.3.3a2/foliolib/folio/api/ebsconet.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/email.py` & `foliolib-0.3.3a2/foliolib/folio/api/email.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/entitiesLinks.py` & `foliolib-0.3.3a2/foliolib/folio/api/entitiesLinks.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/ermUsage.py` & `foliolib-0.3.3a2/foliolib/folio/api/ermUsage.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/ermUsageHarvester.py` & `foliolib-0.3.3a2/foliolib/folio/api/ermUsageHarvester.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/eventConfig.py` & `foliolib-0.3.3a2/foliolib/folio/api/eventConfig.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/feesfines.py` & `foliolib-0.3.3a2/foliolib/folio/api/feesfines.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/finance.py` & `foliolib-0.3.3a2/foliolib/folio/api/finance.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/financeStorage.py` & `foliolib-0.3.3a2/foliolib/folio/api/financeStorage.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/fincConfig.py` & `foliolib-0.3.3a2/foliolib/folio/api/fincConfig.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/gobi.py` & `foliolib-0.3.3a2/foliolib/folio/api/gobi.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/innReach.py` & `foliolib-0.3.3a2/foliolib/folio/api/innReach.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/inventory.py` & `foliolib-0.3.3a2/foliolib/folio/api/inventory.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/inventoryStorage.py` & `foliolib-0.3.3a2/foliolib/folio/api/inventoryStorage.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/inventoryUpdate.py` & `foliolib-0.3.3a2/foliolib/folio/api/inventoryUpdate.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/invoice.py` & `foliolib-0.3.3a2/foliolib/folio/api/invoice.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/invoiceStorage.py` & `foliolib-0.3.3a2/foliolib/folio/api/invoiceStorage.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/kbEbscoJava.py` & `foliolib-0.3.3a2/foliolib/folio/api/kbEbscoJava.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/ldp.py` & `foliolib-0.3.3a2/foliolib/folio/api/ldp.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/licenses.py` & `foliolib-0.3.3a2/foliolib/folio/api/licenses.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/login.py` & `foliolib-0.3.3a2/foliolib/folio/api/login.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/loginSaml.py` & `foliolib-0.3.3a2/foliolib/folio/api/loginSaml.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/marccat.py` & `foliolib-0.3.3a2/foliolib/folio/api/marccat.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/metaStorage.py` & `foliolib-0.3.3a2/foliolib/folio/api/metaStorage.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/notify.py` & `foliolib-0.3.3a2/foliolib/folio/api/notify.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/oaiPmh.py` & `foliolib-0.3.3a2/foliolib/folio/api/oaiPmh.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/orders.py` & `foliolib-0.3.3a2/foliolib/folio/api/orders.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/ordersStorage.py` & `foliolib-0.3.3a2/foliolib/folio/api/ordersStorage.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/organizations.py` & `foliolib-0.3.3a2/foliolib/folio/api/organizations.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/organizationsStorage.py` & `foliolib-0.3.3a2/foliolib/folio/api/organizationsStorage.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/passwordValidator.py` & `foliolib-0.3.3a2/foliolib/folio/api/passwordValidator.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/patron.py` & `foliolib-0.3.3a2/foliolib/folio/api/patron.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/patronBlocks.py` & `foliolib-0.3.3a2/foliolib/folio/api/patronBlocks.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/permissions.py` & `foliolib-0.3.3a2/foliolib/folio/api/permissions.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/pubsub.py` & `foliolib-0.3.3a2/foliolib/folio/api/pubsub.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/quickMarc.py` & `foliolib-0.3.3a2/foliolib/folio/api/quickMarc.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/remoteStorage.py` & `foliolib-0.3.3a2/foliolib/folio/api/remoteStorage.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/reservoir.py` & `foliolib-0.3.3a2/foliolib/folio/api/reservoir.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/rtac.py` & `foliolib-0.3.3a2/foliolib/folio/api/rtac.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/search.py` & `foliolib-0.3.3a2/foliolib/folio/api/search.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/sender.py` & `foliolib-0.3.3a2/foliolib/folio/api/sender.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/settings.py` & `foliolib-0.3.3a2/foliolib/folio/api/settings.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/sharedIndex.py` & `foliolib-0.3.3a2/foliolib/folio/api/sharedIndex.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/sourceRecordManager.py` & `foliolib-0.3.3a2/foliolib/folio/api/sourceRecordManager.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/sourceRecordStorage.py` & `foliolib-0.3.3a2/foliolib/folio/api/sourceRecordStorage.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/templateEngine.py` & `foliolib-0.3.3a2/foliolib/folio/api/templateEngine.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/userImport.py` & `foliolib-0.3.3a2/foliolib/folio/api/userImport.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/users.py` & `foliolib-0.3.3a2/foliolib/folio/api/users.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/api/usersBl.py` & `foliolib-0.3.3a2/foliolib/folio/api/usersBl.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/config.py` & `foliolib-0.3.3a2/foliolib/folio/config.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/dataImport.py` & `foliolib-0.3.3a2/foliolib/folio/dataImport.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/inventory.py` & `foliolib-0.3.3a2/foliolib/folio/inventory.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/inventoryReferenceData.py` & `foliolib-0.3.3a2/foliolib/folio/inventoryReferenceData.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/folio/users.py` & `foliolib-0.3.3a2/foliolib/folio/users.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/helper/__init__.py` & `foliolib-0.3.3a2/foliolib/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/helper/database.py` & `foliolib-0.3.3a2/foliolib/helper/database.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/helper/folio.py` & `foliolib-0.3.3a2/foliolib/helper/folio.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/helper/modules.py` & `foliolib-0.3.3a2/foliolib/helper/modules.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/helper/okapi.py` & `foliolib-0.3.3a2/foliolib/helper/okapi.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/helper/platform.py` & `foliolib-0.3.3a2/foliolib/helper/platform.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/helper/tenant.py` & `foliolib-0.3.3a2/foliolib/helper/tenant.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/okapi/__init__.py` & `foliolib-0.3.3a2/foliolib/okapi/__init__.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/okapi/exceptions.py` & `foliolib-0.3.3a2/foliolib/okapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/okapi/kubeClient.py` & `foliolib-0.3.3a2/foliolib/okapi/kubeClient.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/okapi/misc.py` & `foliolib-0.3.3a2/foliolib/okapi/misc.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/okapi/okapiClient.py` & `foliolib-0.3.3a2/foliolib/okapi/okapiClient.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/okapi/okapiModule.py` & `foliolib-0.3.3a2/foliolib/okapi/okapiModule.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib/okapi/okapiModuleKubernetes.py` & `foliolib-0.3.3a2/foliolib/okapi/okapiModuleKubernetes.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/foliolib.egg-info/PKG-INFO` & `foliolib-0.3.3a2/foliolib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foliolib
-Version: 0.3.3a1
+Version: 0.3.3a2
 Summary: Okapi/Folio Manager and Library
 Home-page: https://github.com/tobi-weber/foliolib
 Author: Tobias Weber
 Author-email: tobi-weber@gmx.de
 License: GPL-3.0 License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `foliolib-0.3.3a1/foliolib.egg-info/SOURCES.txt` & `foliolib-0.3.3a2/foliolib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.3a1/setup.cfg` & `foliolib-0.3.3a2/setup.cfg`

 * *Files identical despite different names*

