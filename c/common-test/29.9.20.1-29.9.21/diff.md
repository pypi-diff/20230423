# Comparing `tmp/common-test-29.9.20.1.tar.gz` & `tmp/common-test-29.9.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "common-test-29.9.20.1.tar", last modified: Sun Apr 23 07:19:04 2023, max compression
+gzip compressed data, was "common-test-29.9.21.tar", last modified: Sun Apr 23 08:06:17 2023, max compression
```

## Comparing `common-test-29.9.20.1.tar` & `common-test-29.9.21.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-23 07:19:04.453598 common-test-29.9.20.1/
--rw-r--r--   0 edz        (502) staff       (20)      625 2023-04-23 07:19:04.453748 common-test-29.9.20.1/PKG-INFO
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-23 07:19:04.405652 common-test-29.9.20.1/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:00.000000 common-test-29.9.20.1/common/__init__.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-23 07:19:04.407921 common-test-29.9.20.1/common/autotest/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:00.000000 common-test-29.9.20.1/common/autotest/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     5993 2023-04-23 00:57:35.000000 common-test-29.9.20.1/common/autotest/base_requests.py
--rw-r--r--   0 edz        (502) staff       (20)     6429 2023-03-22 09:11:00.000000 common-test-29.9.20.1/common/autotest/handle_allure.py
--rw-r--r--   0 edz        (502) staff       (20)    10703 2023-04-14 00:29:00.000000 common-test-29.9.20.1/common/autotest/handle_assert.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-23 07:19:04.414528 common-test-29.9.20.1/common/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:00.000000 common-test-29.9.20.1/common/common/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2126 2023-04-23 02:46:40.000000 common-test-29.9.20.1/common/common/api_driver.py
--rw-r--r--   0 edz        (502) staff       (20)     3462 2023-04-14 00:29:00.000000 common-test-29.9.20.1/common/common/constant.py
--rw-r--r--   0 edz        (502) staff       (20)     1763 2023-04-14 00:29:00.000000 common-test-29.9.20.1/common/common/test.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-23 07:19:04.415647 common-test-29.9.20.1/common/config/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 common-test-29.9.20.1/common/config/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2429 2022-12-01 00:35:00.000000 common-test-29.9.20.1/common/config/config.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-23 07:19:04.418222 common-test-29.9.20.1/common/data/
--rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:00.000000 common-test-29.9.20.1/common/data/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    17483 2023-04-23 00:57:35.000000 common-test-29.9.20.1/common/data/data_process.py
--rw-r--r--   0 edz        (502) staff       (20)     8693 2023-04-14 00:29:00.000000 common-test-29.9.20.1/common/data/handle_common.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-23 07:19:04.422169 common-test-29.9.20.1/common/db/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 common-test-29.9.20.1/common/db/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     3436 2023-04-14 00:29:00.000000 common-test-29.9.20.1/common/db/handle_db.py
--rw-r--r--   0 edz        (502) staff       (20)     1345 2022-12-13 01:35:00.000000 common-test-29.9.20.1/common/db/handle_db_batch.py
--rw-r--r--   0 edz        (502) staff       (20)     1223 2023-04-14 00:29:00.000000 common-test-29.9.20.1/common/db/handle_mysqldb.py
--rw-r--r--   0 edz        (502) staff       (20)     1533 2023-04-14 00:29:00.000000 common-test-29.9.20.1/common/db/handle_oracle.py
--rw-r--r--   0 edz        (502) staff       (20)     1665 2023-04-14 00:29:00.000000 common-test-29.9.20.1/common/db/handle_sqlserver.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-23 07:19:04.429230 common-test-29.9.20.1/common/file/
--rw-r--r--   0 edz        (502) staff       (20)     4508 2023-04-14 00:29:00.000000 common-test-29.9.20.1/common/file/ReadFile.py
--rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:00.000000 common-test-29.9.20.1/common/file/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    11703 2023-04-23 07:18:42.000000 common-test-29.9.20.1/common/file/handle_excel.py
--rw-r--r--   0 edz        (502) staff       (20)     2265 2023-04-14 00:29:00.000000 common-test-29.9.20.1/common/file/handle_file.py
--rw-r--r--   0 edz        (502) staff       (20)     1364 2023-04-14 00:29:00.000000 common-test-29.9.20.1/common/file/handle_reques.py
--rw-r--r--   0 edz        (502) staff       (20)     2201 2022-10-24 01:09:00.000000 common-test-29.9.20.1/common/file/handle_system.py
--rw-r--r--   0 edz        (502) staff       (20)     1000 2023-04-14 00:29:00.000000 common-test-29.9.20.1/common/file/handle_yaml.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-23 07:19:04.432721 common-test-29.9.20.1/common/mq/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 common-test-29.9.20.1/common/mq/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2059 2023-04-14 00:29:00.000000 common-test-29.9.20.1/common/mq/handle_rabbit.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-23 07:19:04.437549 common-test-29.9.20.1/common/plat/
--rw-r--r--   0 edz        (502) staff       (20)    12849 2023-04-14 00:29:00.000000 common-test-29.9.20.1/common/plat/ATF_platform.py
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-04-16 11:02:00.000000 common-test-29.9.20.1/common/plat/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1384 2022-04-27 12:06:00.000000 common-test-29.9.20.1/common/plat/jenkin_platform.py
--rw-r--r--   0 edz        (502) staff       (20)    15697 2023-04-14 00:29:00.000000 common-test-29.9.20.1/common/plat/jira_platform.py
--rw-r--r--   0 edz        (502) staff       (20)    13513 2023-04-14 00:29:00.000000 common-test-29.9.20.1/common/plat/mysql_platform.py
--rw-r--r--   0 edz        (502) staff       (20)     1056 2023-04-14 00:29:00.000000 common-test-29.9.20.1/common/plat/service_platform.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-23 07:19:04.449330 common-test-29.9.20.1/common/plugin/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:00.000000 common-test-29.9.20.1/common/plugin/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1330 2023-01-16 07:33:00.000000 common-test-29.9.20.1/common/plugin/allure_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     2054 2022-07-28 02:48:00.000000 common-test-29.9.20.1/common/plugin/assert_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     7574 2023-04-14 00:29:00.000000 common-test-29.9.20.1/common/plugin/atf_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     5988 2023-04-14 00:29:00.000000 common-test-29.9.20.1/common/plugin/data_bus.py
--rw-r--r--   0 edz        (502) staff       (20)     3009 2023-04-14 00:29:00.000000 common-test-29.9.20.1/common/plugin/data_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     9773 2023-04-23 03:07:54.000000 common-test-29.9.20.1/common/plugin/file_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:00.000000 common-test-29.9.20.1/common/plugin/hooks_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    13093 2023-01-16 07:46:00.000000 common-test-29.9.20.1/common/plugin/pytest_playwright.py
--rw-r--r--   0 edz        (502) staff       (20)    15927 2023-04-14 00:29:00.000000 common-test-29.9.20.1/common/plugin/pytest_plugin.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-23 07:19:04.453217 common-test-29.9.20.1/common_test.egg-info/
--rw-r--r--   0 edz        (502) staff       (20)      625 2023-04-23 07:19:04.000000 common-test-29.9.20.1/common_test.egg-info/PKG-INFO
--rw-r--r--   0 edz        (502) staff       (20)     1475 2023-04-23 07:19:04.000000 common-test-29.9.20.1/common_test.egg-info/SOURCES.txt
--rw-r--r--   0 edz        (502) staff       (20)        1 2023-04-23 07:19:04.000000 common-test-29.9.20.1/common_test.egg-info/dependency_links.txt
--rw-r--r--   0 edz        (502) staff       (20)       57 2023-04-23 07:19:04.000000 common-test-29.9.20.1/common_test.egg-info/entry_points.txt
--rw-r--r--   0 edz        (502) staff       (20)      560 2023-04-23 07:19:04.000000 common-test-29.9.20.1/common_test.egg-info/requires.txt
--rw-r--r--   0 edz        (502) staff       (20)        7 2023-04-23 07:19:04.000000 common-test-29.9.20.1/common_test.egg-info/top_level.txt
--rw-r--r--   0 edz        (502) staff       (20)      442 2023-04-23 07:19:04.454640 common-test-29.9.20.1/setup.cfg
--rw-r--r--   0 edz        (502) staff       (20)     1621 2023-04-23 00:59:38.000000 common-test-29.9.20.1/setup.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-23 08:06:17.573247 common-test-29.9.21/
+-rw-r--r--   0 edz        (502) staff       (20)      623 2023-04-23 08:06:17.573420 common-test-29.9.21/PKG-INFO
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-23 08:06:17.534266 common-test-29.9.21/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:00.000000 common-test-29.9.21/common/__init__.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-23 08:06:17.536518 common-test-29.9.21/common/autotest/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:00.000000 common-test-29.9.21/common/autotest/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     5993 2023-04-23 00:57:35.000000 common-test-29.9.21/common/autotest/base_requests.py
+-rw-r--r--   0 edz        (502) staff       (20)     6429 2023-03-22 09:11:00.000000 common-test-29.9.21/common/autotest/handle_allure.py
+-rw-r--r--   0 edz        (502) staff       (20)    10703 2023-04-14 00:29:00.000000 common-test-29.9.21/common/autotest/handle_assert.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-23 08:06:17.539092 common-test-29.9.21/common/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:00.000000 common-test-29.9.21/common/common/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2126 2023-04-23 02:46:40.000000 common-test-29.9.21/common/common/api_driver.py
+-rw-r--r--   0 edz        (502) staff       (20)     3462 2023-04-14 00:29:00.000000 common-test-29.9.21/common/common/constant.py
+-rw-r--r--   0 edz        (502) staff       (20)     1763 2023-04-14 00:29:00.000000 common-test-29.9.21/common/common/test.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-23 08:06:17.540220 common-test-29.9.21/common/config/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 common-test-29.9.21/common/config/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2429 2022-12-01 00:35:00.000000 common-test-29.9.21/common/config/config.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-23 08:06:17.542585 common-test-29.9.21/common/data/
+-rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:00.000000 common-test-29.9.21/common/data/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    17483 2023-04-23 00:57:35.000000 common-test-29.9.21/common/data/data_process.py
+-rw-r--r--   0 edz        (502) staff       (20)     8662 2023-04-23 07:58:21.000000 common-test-29.9.21/common/data/handle_common.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-23 08:06:17.546980 common-test-29.9.21/common/db/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 common-test-29.9.21/common/db/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     3436 2023-04-14 00:29:00.000000 common-test-29.9.21/common/db/handle_db.py
+-rw-r--r--   0 edz        (502) staff       (20)     1345 2022-12-13 01:35:00.000000 common-test-29.9.21/common/db/handle_db_batch.py
+-rw-r--r--   0 edz        (502) staff       (20)     1223 2023-04-14 00:29:00.000000 common-test-29.9.21/common/db/handle_mysqldb.py
+-rw-r--r--   0 edz        (502) staff       (20)     1533 2023-04-14 00:29:00.000000 common-test-29.9.21/common/db/handle_oracle.py
+-rw-r--r--   0 edz        (502) staff       (20)     1665 2023-04-14 00:29:00.000000 common-test-29.9.21/common/db/handle_sqlserver.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-23 08:06:17.551839 common-test-29.9.21/common/file/
+-rw-r--r--   0 edz        (502) staff       (20)     4508 2023-04-14 00:29:00.000000 common-test-29.9.21/common/file/ReadFile.py
+-rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:00.000000 common-test-29.9.21/common/file/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    11703 2023-04-23 07:18:42.000000 common-test-29.9.21/common/file/handle_excel.py
+-rw-r--r--   0 edz        (502) staff       (20)     2265 2023-04-14 00:29:00.000000 common-test-29.9.21/common/file/handle_file.py
+-rw-r--r--   0 edz        (502) staff       (20)     1364 2023-04-14 00:29:00.000000 common-test-29.9.21/common/file/handle_reques.py
+-rw-r--r--   0 edz        (502) staff       (20)     2201 2022-10-24 01:09:00.000000 common-test-29.9.21/common/file/handle_system.py
+-rw-r--r--   0 edz        (502) staff       (20)     1000 2023-04-14 00:29:00.000000 common-test-29.9.21/common/file/handle_yaml.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-23 08:06:17.552812 common-test-29.9.21/common/mq/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 common-test-29.9.21/common/mq/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2059 2023-04-14 00:29:00.000000 common-test-29.9.21/common/mq/handle_rabbit.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-23 08:06:17.557428 common-test-29.9.21/common/plat/
+-rw-r--r--   0 edz        (502) staff       (20)    12849 2023-04-14 00:29:00.000000 common-test-29.9.21/common/plat/ATF_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-04-16 11:02:00.000000 common-test-29.9.21/common/plat/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1384 2022-04-27 12:06:00.000000 common-test-29.9.21/common/plat/jenkin_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)    15697 2023-04-14 00:29:00.000000 common-test-29.9.21/common/plat/jira_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)    13513 2023-04-14 00:29:00.000000 common-test-29.9.21/common/plat/mysql_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)     1056 2023-04-14 00:29:00.000000 common-test-29.9.21/common/plat/service_platform.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-23 08:06:17.569582 common-test-29.9.21/common/plugin/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:00.000000 common-test-29.9.21/common/plugin/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1330 2023-01-16 07:33:00.000000 common-test-29.9.21/common/plugin/allure_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     2054 2022-07-28 02:48:00.000000 common-test-29.9.21/common/plugin/assert_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     7574 2023-04-14 00:29:00.000000 common-test-29.9.21/common/plugin/atf_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     5988 2023-04-14 00:29:00.000000 common-test-29.9.21/common/plugin/data_bus.py
+-rw-r--r--   0 edz        (502) staff       (20)     3908 2023-04-23 08:05:34.000000 common-test-29.9.21/common/plugin/data_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     9576 2023-04-23 07:58:21.000000 common-test-29.9.21/common/plugin/file_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:00.000000 common-test-29.9.21/common/plugin/hooks_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    13093 2023-01-16 07:46:00.000000 common-test-29.9.21/common/plugin/pytest_playwright.py
+-rw-r--r--   0 edz        (502) staff       (20)    15927 2023-04-14 00:29:00.000000 common-test-29.9.21/common/plugin/pytest_plugin.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-23 08:06:17.572880 common-test-29.9.21/common_test.egg-info/
+-rw-r--r--   0 edz        (502) staff       (20)      623 2023-04-23 08:06:17.000000 common-test-29.9.21/common_test.egg-info/PKG-INFO
+-rw-r--r--   0 edz        (502) staff       (20)     1475 2023-04-23 08:06:17.000000 common-test-29.9.21/common_test.egg-info/SOURCES.txt
+-rw-r--r--   0 edz        (502) staff       (20)        1 2023-04-23 08:06:17.000000 common-test-29.9.21/common_test.egg-info/dependency_links.txt
+-rw-r--r--   0 edz        (502) staff       (20)       57 2023-04-23 08:06:17.000000 common-test-29.9.21/common_test.egg-info/entry_points.txt
+-rw-r--r--   0 edz        (502) staff       (20)      571 2023-04-23 08:06:17.000000 common-test-29.9.21/common_test.egg-info/requires.txt
+-rw-r--r--   0 edz        (502) staff       (20)        7 2023-04-23 08:06:17.000000 common-test-29.9.21/common_test.egg-info/top_level.txt
+-rw-r--r--   0 edz        (502) staff       (20)      440 2023-04-23 08:06:17.574206 common-test-29.9.21/setup.cfg
+-rw-r--r--   0 edz        (502) staff       (20)     1670 2023-04-23 07:41:21.000000 common-test-29.9.21/setup.py
```

### Comparing `common-test-29.9.20.1/PKG-INFO` & `common-test-29.9.21/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: common-test
-Version: 29.9.20.1
+Version: 29.9.21
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: shiqiang.ou
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `common-test-29.9.20.1/common/autotest/base_requests.py` & `common-test-29.9.21/common/autotest/base_requests.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20.1/common/autotest/handle_allure.py` & `common-test-29.9.21/common/autotest/handle_allure.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20.1/common/autotest/handle_assert.py` & `common-test-29.9.21/common/autotest/handle_assert.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20.1/common/common/api_driver.py` & `common-test-29.9.21/common/common/api_driver.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20.1/common/common/constant.py` & `common-test-29.9.21/common/common/constant.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20.1/common/common/test.py` & `common-test-29.9.21/common/common/test.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20.1/common/config/config.py` & `common-test-29.9.21/common/config/config.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20.1/common/data/data_process.py` & `common-test-29.9.21/common/data/data_process.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20.1/common/data/handle_common.py` & `common-test-29.9.21/common/data/handle_common.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,14 @@
     :param data: 在该项目中一般为响应字典，从字典取值出来
     :param expr: 查找用的正则表达式
     return content： 替换表达式后的字符串
     """
     if isinstance(content, str):
         content = content.replace('\\', '')
     else:
-        content = str(content)
         content = str(content).replace('\\', '')
 
     for i in re.findall(expr, content):
         if i.find(".") >= 0:
             from common.plugin.data_bus import DataBus
             _content = DataBus.get_key(i)
```

### Comparing `common-test-29.9.20.1/common/db/handle_db.py` & `common-test-29.9.21/common/db/handle_db.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20.1/common/db/handle_db_batch.py` & `common-test-29.9.21/common/db/handle_db_batch.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20.1/common/db/handle_mysqldb.py` & `common-test-29.9.21/common/db/handle_mysqldb.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20.1/common/db/handle_oracle.py` & `common-test-29.9.21/common/db/handle_oracle.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20.1/common/db/handle_sqlserver.py` & `common-test-29.9.21/common/db/handle_sqlserver.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20.1/common/file/ReadFile.py` & `common-test-29.9.21/common/file/ReadFile.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20.1/common/file/handle_excel.py` & `common-test-29.9.21/common/file/handle_excel.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20.1/common/file/handle_file.py` & `common-test-29.9.21/common/file/handle_file.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20.1/common/file/handle_reques.py` & `common-test-29.9.21/common/file/handle_reques.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20.1/common/file/handle_system.py` & `common-test-29.9.21/common/file/handle_system.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20.1/common/file/handle_yaml.py` & `common-test-29.9.21/common/file/handle_yaml.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20.1/common/mq/handle_rabbit.py` & `common-test-29.9.21/common/mq/handle_rabbit.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20.1/common/plat/ATF_platform.py` & `common-test-29.9.21/common/plat/ATF_platform.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20.1/common/plat/jenkin_platform.py` & `common-test-29.9.21/common/plat/jenkin_platform.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20.1/common/plat/jira_platform.py` & `common-test-29.9.21/common/plat/jira_platform.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20.1/common/plat/mysql_platform.py` & `common-test-29.9.21/common/plat/mysql_platform.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20.1/common/plat/service_platform.py` & `common-test-29.9.21/common/plat/service_platform.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20.1/common/plugin/allure_plugin.py` & `common-test-29.9.21/common/plugin/allure_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20.1/common/plugin/assert_plugin.py` & `common-test-29.9.21/common/plugin/assert_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20.1/common/plugin/atf_plugin.py` & `common-test-29.9.21/common/plugin/atf_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20.1/common/plugin/data_bus.py` & `common-test-29.9.21/common/plugin/data_bus.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20.1/common/plugin/file_plugin.py` & `common-test-29.9.21/common/plugin/file_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -260,17 +260,15 @@
             if _dict[Constant.CASE_TITLE] in _mark:
                 _flag = True
             else:
                 _flag = False
         return _flag
 
 
-if __name__ == '__main__':
-    DataBus.set_key('883434','9999999')
-    print(FilePlugin.load_file('aa.json', _dict={'ticketNo':'883334','registrationNo':'733','subFrom':DataBus.get_key('883434')}))
+
```

### Comparing `common-test-29.9.20.1/common/plugin/hooks_plugin.py` & `common-test-29.9.21/common/plugin/hooks_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20.1/common/plugin/pytest_playwright.py` & `common-test-29.9.21/common/plugin/pytest_playwright.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20.1/common/plugin/pytest_plugin.py` & `common-test-29.9.21/common/plugin/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20.1/common_test.egg-info/PKG-INFO` & `common-test-29.9.21/common_test.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: common-test
-Version: 29.9.20.1
+Version: 29.9.21
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: shiqiang.ou
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `common-test-29.9.20.1/common_test.egg-info/SOURCES.txt` & `common-test-29.9.21/common_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20.1/common_test.egg-info/requires.txt` & `common-test-29.9.21/common_test.egg-info/requires.txt`

 * *Files 23% similar despite different names*

```diff
@@ -25,7 +25,8 @@
 deepdiff==5.8.1
 dnspython==2.2.1
 jsonschema==4.17.0
 xmlschema==1.0.14
 pymongo==3.5.1
 redis-py-cluster==2.1.3
 redis==3.5.3
+bs4==0.0.1
```

### Comparing `common-test-29.9.20.1/setup.py` & `common-test-29.9.21/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,17 @@
         "assertpy==1.1",
         "deepdiff==5.8.1",
         "dnspython==2.2.1",
         "jsonschema==4.17.0",
         "xmlschema==1.0.14",
         "pymongo==3.5.1",
         "redis-py-cluster==2.1.3",
-        "redis==3.5.3"
+        "redis==3.5.3",
+        #"ddddocr==1.4.7",
+        "bs4==0.0.1"
         # "selenium==4.6.0",
     ],
     entry_points={"pytest11": ["playwright = common.plugin.pytest_playwright"]},
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
```

