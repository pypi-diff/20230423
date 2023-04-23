# Comparing `tmp/common-test-29.9.20.tar.gz` & `tmp/common-test-29.9.20.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "common-test-29.9.20.tar", last modified: Fri Apr 14 00:31:46 2023, max compression
+gzip compressed data, was "common-test-29.9.20.1.tar", last modified: Sun Apr 23 07:19:04 2023, max compression
```

## Comparing `common-test-29.9.20.tar` & `common-test-29.9.20.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-14 00:31:46.475943 common-test-29.9.20/
--rw-r--r--   0 edz        (502) staff       (20)      623 2023-04-14 00:31:46.476146 common-test-29.9.20/PKG-INFO
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-14 00:31:46.451749 common-test-29.9.20/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:20.000000 common-test-29.9.20/common/__init__.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-14 00:31:46.453202 common-test-29.9.20/common/autotest/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:14.000000 common-test-29.9.20/common/autotest/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     5939 2023-04-14 00:29:21.000000 common-test-29.9.20/common/autotest/base_requests.py
--rw-r--r--   0 edz        (502) staff       (20)     6429 2023-03-22 09:11:35.000000 common-test-29.9.20/common/autotest/handle_allure.py
--rw-r--r--   0 edz        (502) staff       (20)    10703 2023-04-14 00:29:21.000000 common-test-29.9.20/common/autotest/handle_assert.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-14 00:31:46.455106 common-test-29.9.20/common/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:39.000000 common-test-29.9.20/common/common/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2050 2023-04-14 00:29:21.000000 common-test-29.9.20/common/common/api_driver.py
--rw-r--r--   0 edz        (502) staff       (20)     3462 2023-04-14 00:29:21.000000 common-test-29.9.20/common/common/constant.py
--rw-r--r--   0 edz        (502) staff       (20)     1763 2023-04-14 00:29:21.000000 common-test-29.9.20/common/common/test.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-14 00:31:46.455813 common-test-29.9.20/common/config/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:55.000000 common-test-29.9.20/common/config/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2429 2022-12-01 00:35:04.000000 common-test-29.9.20/common/config/config.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-14 00:31:46.457088 common-test-29.9.20/common/data/
--rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:37.000000 common-test-29.9.20/common/data/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    16494 2023-04-07 07:27:39.000000 common-test-29.9.20/common/data/data_process.py
--rw-r--r--   0 edz        (502) staff       (20)     8693 2023-04-14 00:29:21.000000 common-test-29.9.20/common/data/handle_common.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-14 00:31:46.460120 common-test-29.9.20/common/db/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:55.000000 common-test-29.9.20/common/db/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     3436 2023-04-14 00:29:21.000000 common-test-29.9.20/common/db/handle_db.py
--rw-r--r--   0 edz        (502) staff       (20)     1345 2022-12-13 01:35:27.000000 common-test-29.9.20/common/db/handle_db_batch.py
--rw-r--r--   0 edz        (502) staff       (20)     1223 2023-04-14 00:29:21.000000 common-test-29.9.20/common/db/handle_mysqldb.py
--rw-r--r--   0 edz        (502) staff       (20)     1533 2023-04-14 00:29:21.000000 common-test-29.9.20/common/db/handle_oracle.py
--rw-r--r--   0 edz        (502) staff       (20)     1665 2023-04-14 00:29:21.000000 common-test-29.9.20/common/db/handle_sqlserver.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-14 00:31:46.462478 common-test-29.9.20/common/file/
--rw-r--r--   0 edz        (502) staff       (20)     4508 2023-04-14 00:29:21.000000 common-test-29.9.20/common/file/ReadFile.py
--rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:53.000000 common-test-29.9.20/common/file/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    11639 2023-04-14 00:29:21.000000 common-test-29.9.20/common/file/handle_excel.py
--rw-r--r--   0 edz        (502) staff       (20)     2265 2023-04-14 00:29:21.000000 common-test-29.9.20/common/file/handle_file.py
--rw-r--r--   0 edz        (502) staff       (20)     1364 2023-04-14 00:29:21.000000 common-test-29.9.20/common/file/handle_reques.py
--rw-r--r--   0 edz        (502) staff       (20)     2201 2022-10-24 01:09:23.000000 common-test-29.9.20/common/file/handle_system.py
--rw-r--r--   0 edz        (502) staff       (20)     1000 2023-04-14 00:29:21.000000 common-test-29.9.20/common/file/handle_yaml.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-14 00:31:46.463028 common-test-29.9.20/common/mq/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:55.000000 common-test-29.9.20/common/mq/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2059 2023-04-14 00:29:21.000000 common-test-29.9.20/common/mq/handle_rabbit.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-14 00:31:46.465066 common-test-29.9.20/common/plat/
--rw-r--r--   0 edz        (502) staff       (20)    12849 2023-04-14 00:29:21.000000 common-test-29.9.20/common/plat/ATF_platform.py
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-04-16 11:02:13.000000 common-test-29.9.20/common/plat/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1384 2022-04-27 12:06:42.000000 common-test-29.9.20/common/plat/jenkin_platform.py
--rw-r--r--   0 edz        (502) staff       (20)    15697 2023-04-14 00:29:21.000000 common-test-29.9.20/common/plat/jira_platform.py
--rw-r--r--   0 edz        (502) staff       (20)    13513 2023-04-14 00:29:21.000000 common-test-29.9.20/common/plat/mysql_platform.py
--rw-r--r--   0 edz        (502) staff       (20)     1056 2023-04-14 00:29:21.000000 common-test-29.9.20/common/plat/service_platform.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-14 00:31:46.471472 common-test-29.9.20/common/plugin/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:42.000000 common-test-29.9.20/common/plugin/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1330 2023-01-16 07:33:57.000000 common-test-29.9.20/common/plugin/allure_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     2054 2022-07-28 02:48:03.000000 common-test-29.9.20/common/plugin/assert_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     7574 2023-04-14 00:29:21.000000 common-test-29.9.20/common/plugin/atf_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     5988 2023-04-14 00:29:21.000000 common-test-29.9.20/common/plugin/data_bus.py
--rw-r--r--   0 edz        (502) staff       (20)     3009 2023-04-14 00:29:21.000000 common-test-29.9.20/common/plugin/data_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     9624 2023-04-14 00:29:21.000000 common-test-29.9.20/common/plugin/file_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:18.000000 common-test-29.9.20/common/plugin/hooks_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    13093 2023-01-16 07:46:45.000000 common-test-29.9.20/common/plugin/pytest_playwright.py
--rw-r--r--   0 edz        (502) staff       (20)    15927 2023-04-14 00:29:21.000000 common-test-29.9.20/common/plugin/pytest_plugin.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-14 00:31:46.475414 common-test-29.9.20/common_test.egg-info/
--rw-r--r--   0 edz        (502) staff       (20)      623 2023-04-14 00:31:46.000000 common-test-29.9.20/common_test.egg-info/PKG-INFO
--rw-r--r--   0 edz        (502) staff       (20)     1475 2023-04-14 00:31:46.000000 common-test-29.9.20/common_test.egg-info/SOURCES.txt
--rw-r--r--   0 edz        (502) staff       (20)        1 2023-04-14 00:31:46.000000 common-test-29.9.20/common_test.egg-info/dependency_links.txt
--rw-r--r--   0 edz        (502) staff       (20)       57 2023-04-14 00:31:46.000000 common-test-29.9.20/common_test.egg-info/entry_points.txt
--rw-r--r--   0 edz        (502) staff       (20)      560 2023-04-14 00:31:46.000000 common-test-29.9.20/common_test.egg-info/requires.txt
--rw-r--r--   0 edz        (502) staff       (20)        7 2023-04-14 00:31:46.000000 common-test-29.9.20/common_test.egg-info/top_level.txt
--rw-r--r--   0 edz        (502) staff       (20)      440 2023-04-14 00:31:46.477186 common-test-29.9.20/setup.cfg
--rw-r--r--   0 edz        (502) staff       (20)     1621 2023-04-11 07:05:24.000000 common-test-29.9.20/setup.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-23 07:19:04.453598 common-test-29.9.20.1/
+-rw-r--r--   0 edz        (502) staff       (20)      625 2023-04-23 07:19:04.453748 common-test-29.9.20.1/PKG-INFO
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-23 07:19:04.405652 common-test-29.9.20.1/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:00.000000 common-test-29.9.20.1/common/__init__.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-23 07:19:04.407921 common-test-29.9.20.1/common/autotest/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:00.000000 common-test-29.9.20.1/common/autotest/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     5993 2023-04-23 00:57:35.000000 common-test-29.9.20.1/common/autotest/base_requests.py
+-rw-r--r--   0 edz        (502) staff       (20)     6429 2023-03-22 09:11:00.000000 common-test-29.9.20.1/common/autotest/handle_allure.py
+-rw-r--r--   0 edz        (502) staff       (20)    10703 2023-04-14 00:29:00.000000 common-test-29.9.20.1/common/autotest/handle_assert.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-23 07:19:04.414528 common-test-29.9.20.1/common/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:00.000000 common-test-29.9.20.1/common/common/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2126 2023-04-23 02:46:40.000000 common-test-29.9.20.1/common/common/api_driver.py
+-rw-r--r--   0 edz        (502) staff       (20)     3462 2023-04-14 00:29:00.000000 common-test-29.9.20.1/common/common/constant.py
+-rw-r--r--   0 edz        (502) staff       (20)     1763 2023-04-14 00:29:00.000000 common-test-29.9.20.1/common/common/test.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-23 07:19:04.415647 common-test-29.9.20.1/common/config/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 common-test-29.9.20.1/common/config/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2429 2022-12-01 00:35:00.000000 common-test-29.9.20.1/common/config/config.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-23 07:19:04.418222 common-test-29.9.20.1/common/data/
+-rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:00.000000 common-test-29.9.20.1/common/data/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    17483 2023-04-23 00:57:35.000000 common-test-29.9.20.1/common/data/data_process.py
+-rw-r--r--   0 edz        (502) staff       (20)     8693 2023-04-14 00:29:00.000000 common-test-29.9.20.1/common/data/handle_common.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-23 07:19:04.422169 common-test-29.9.20.1/common/db/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 common-test-29.9.20.1/common/db/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     3436 2023-04-14 00:29:00.000000 common-test-29.9.20.1/common/db/handle_db.py
+-rw-r--r--   0 edz        (502) staff       (20)     1345 2022-12-13 01:35:00.000000 common-test-29.9.20.1/common/db/handle_db_batch.py
+-rw-r--r--   0 edz        (502) staff       (20)     1223 2023-04-14 00:29:00.000000 common-test-29.9.20.1/common/db/handle_mysqldb.py
+-rw-r--r--   0 edz        (502) staff       (20)     1533 2023-04-14 00:29:00.000000 common-test-29.9.20.1/common/db/handle_oracle.py
+-rw-r--r--   0 edz        (502) staff       (20)     1665 2023-04-14 00:29:00.000000 common-test-29.9.20.1/common/db/handle_sqlserver.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-23 07:19:04.429230 common-test-29.9.20.1/common/file/
+-rw-r--r--   0 edz        (502) staff       (20)     4508 2023-04-14 00:29:00.000000 common-test-29.9.20.1/common/file/ReadFile.py
+-rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:00.000000 common-test-29.9.20.1/common/file/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    11703 2023-04-23 07:18:42.000000 common-test-29.9.20.1/common/file/handle_excel.py
+-rw-r--r--   0 edz        (502) staff       (20)     2265 2023-04-14 00:29:00.000000 common-test-29.9.20.1/common/file/handle_file.py
+-rw-r--r--   0 edz        (502) staff       (20)     1364 2023-04-14 00:29:00.000000 common-test-29.9.20.1/common/file/handle_reques.py
+-rw-r--r--   0 edz        (502) staff       (20)     2201 2022-10-24 01:09:00.000000 common-test-29.9.20.1/common/file/handle_system.py
+-rw-r--r--   0 edz        (502) staff       (20)     1000 2023-04-14 00:29:00.000000 common-test-29.9.20.1/common/file/handle_yaml.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-23 07:19:04.432721 common-test-29.9.20.1/common/mq/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 common-test-29.9.20.1/common/mq/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2059 2023-04-14 00:29:00.000000 common-test-29.9.20.1/common/mq/handle_rabbit.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-23 07:19:04.437549 common-test-29.9.20.1/common/plat/
+-rw-r--r--   0 edz        (502) staff       (20)    12849 2023-04-14 00:29:00.000000 common-test-29.9.20.1/common/plat/ATF_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-04-16 11:02:00.000000 common-test-29.9.20.1/common/plat/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1384 2022-04-27 12:06:00.000000 common-test-29.9.20.1/common/plat/jenkin_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)    15697 2023-04-14 00:29:00.000000 common-test-29.9.20.1/common/plat/jira_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)    13513 2023-04-14 00:29:00.000000 common-test-29.9.20.1/common/plat/mysql_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)     1056 2023-04-14 00:29:00.000000 common-test-29.9.20.1/common/plat/service_platform.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-23 07:19:04.449330 common-test-29.9.20.1/common/plugin/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:00.000000 common-test-29.9.20.1/common/plugin/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1330 2023-01-16 07:33:00.000000 common-test-29.9.20.1/common/plugin/allure_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     2054 2022-07-28 02:48:00.000000 common-test-29.9.20.1/common/plugin/assert_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     7574 2023-04-14 00:29:00.000000 common-test-29.9.20.1/common/plugin/atf_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     5988 2023-04-14 00:29:00.000000 common-test-29.9.20.1/common/plugin/data_bus.py
+-rw-r--r--   0 edz        (502) staff       (20)     3009 2023-04-14 00:29:00.000000 common-test-29.9.20.1/common/plugin/data_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     9773 2023-04-23 03:07:54.000000 common-test-29.9.20.1/common/plugin/file_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:00.000000 common-test-29.9.20.1/common/plugin/hooks_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    13093 2023-01-16 07:46:00.000000 common-test-29.9.20.1/common/plugin/pytest_playwright.py
+-rw-r--r--   0 edz        (502) staff       (20)    15927 2023-04-14 00:29:00.000000 common-test-29.9.20.1/common/plugin/pytest_plugin.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-23 07:19:04.453217 common-test-29.9.20.1/common_test.egg-info/
+-rw-r--r--   0 edz        (502) staff       (20)      625 2023-04-23 07:19:04.000000 common-test-29.9.20.1/common_test.egg-info/PKG-INFO
+-rw-r--r--   0 edz        (502) staff       (20)     1475 2023-04-23 07:19:04.000000 common-test-29.9.20.1/common_test.egg-info/SOURCES.txt
+-rw-r--r--   0 edz        (502) staff       (20)        1 2023-04-23 07:19:04.000000 common-test-29.9.20.1/common_test.egg-info/dependency_links.txt
+-rw-r--r--   0 edz        (502) staff       (20)       57 2023-04-23 07:19:04.000000 common-test-29.9.20.1/common_test.egg-info/entry_points.txt
+-rw-r--r--   0 edz        (502) staff       (20)      560 2023-04-23 07:19:04.000000 common-test-29.9.20.1/common_test.egg-info/requires.txt
+-rw-r--r--   0 edz        (502) staff       (20)        7 2023-04-23 07:19:04.000000 common-test-29.9.20.1/common_test.egg-info/top_level.txt
+-rw-r--r--   0 edz        (502) staff       (20)      442 2023-04-23 07:19:04.454640 common-test-29.9.20.1/setup.cfg
+-rw-r--r--   0 edz        (502) staff       (20)     1621 2023-04-23 00:59:38.000000 common-test-29.9.20.1/setup.py
```

### Comparing `common-test-29.9.20/PKG-INFO` & `common-test-29.9.20.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: common-test
-Version: 29.9.20
+Version: 29.9.20.1
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: shiqiang.ou
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `common-test-29.9.20/common/autotest/base_requests.py` & `common-test-29.9.20.1/common/autotest/base_requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
                 data = DataProcess.handle_data(data, False)
         except Exception as e:
             logger.info(f'测试数据：{data} 转换异常:' + repr(e))
         file = DataProcess.handler_files(file_obj)
         desc = f'测试接口详情:{url}'
         # 发送请求
         res = cls.http_request(url=url, method=method, parametric_key=parametric_key,
-                               header=header, data=data, file=file, desc=desc)
+                               header=DataProcess.setDictEncode(header), data=data, file=file, desc=desc)
         try:
             if DataProcess.isNotNull(get_system_key(Constant.RUN_TYPE)):
                 MysqlPlatForm.insert_api_data(url, method, header, data, res.elapsed.total_seconds(), res.status_code)
         except:
             logger.warning("保存请求数据异常")
         # 响应后操作
         if token == '写':
@@ -95,15 +95,15 @@
                 data = DataProcess.handle_data(data, False)
         except Exception as e:
             logger.info(f'测试数据：{data} 转换异常:' + repr(e))
         file_obj = DataProcess.handler_files(file)
         if step == '测试接口详情' and DataProcess.isNotNull(schemal_data['desc']):
             step = '测试接口详情:'+schemal_data['desc']
         res = cls.http_request(url=url, method=schemal_data['method'], parametric_key=schemal_data['datatype'],
-                               header=header, data=data, file=file_obj, cookie=cookie, desc=step)
+                               header=DataProcess.setDictEncode(header), data=data, file=file_obj, cookie=cookie, desc=step)
         try:
             if DataProcess.isNotNull(get_system_key(Constant.RUN_TYPE)):
                 MysqlPlatForm.insert_api_data(url, schemal_data['method'], header, data, res.elapsed.total_seconds(), res.status_code)
         except:
             logger.warning("保存请求数据异常")
         return res
```

### Comparing `common-test-29.9.20/common/autotest/handle_allure.py` & `common-test-29.9.20.1/common/autotest/handle_allure.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/autotest/handle_assert.py` & `common-test-29.9.20.1/common/autotest/handle_assert.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/common/api_driver.py` & `common-test-29.9.20.1/common/common/api_driver.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,15 @@
         """
         :param method: 请求方法
         :param url: 请求url
         :param parametric_key: 入参关键字， params(查询参数类型，明文传输，一般在url?参数名=参数值), data(一般用于form表单类型参数)
         json(一般用于json类型请求参数)
         :param data: 参数数据，默认等于None
         :param file: 文件对象
+        :param desc: 自动化测试过程请求描述：打印到Report中
         :param header: 请求头
         :return: 返回res对象
         """
         session = cls.get_session()
         if parametric_key is None:
             res = session.request(method=method, url=url, headers=header, cookies=cookie, auth=_auth)
             allure_api_step(desc, url, method, header, '', '', res)
```

### Comparing `common-test-29.9.20/common/common/constant.py` & `common-test-29.9.20.1/common/common/constant.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/common/test.py` & `common-test-29.9.20.1/common/common/test.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/config/config.py` & `common-test-29.9.20.1/common/config/config.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/data/data_process.py` & `common-test-29.9.20.1/common/data/data_process.py`

 * *Files 7% similar despite different names*

```diff
@@ -385,14 +385,46 @@
                     scriptmethod = scrtpArr[0]
             scriptname = get_system_key(Constant.CURRENT_PATH) + os.sep + caseArr[0]
             return testname,gitname,scripturl, scriptclass, scriptmethod, scriptname
         except Exception as e:
             logger.info(f'解析用例脚本路径URL：用例名称:{testname} 脚本路径:{caseurl} 异常信息：{e}')
             return testname, "", "", "", "",""
 
+    @classmethod
+    def is_contain_chinese(self, check_str):
+        """
+        判断字符串中是否包含中文
+        :param check_str: {str} 需要检测的字符串
+        :return: {bool} 包含返回True， 不包含返回False
+        """
+        for ch in check_str:
+            if u'\u4e00' <= ch <= u'\u9fff':
+                return True
+        return False
+
+    @classmethod
+    def setDictEncode(self, dict):
+        """
+        处理header中的特殊字符串 空格、int、float、中文
+        :param dict:
+        :return:
+        """
+        for key, value in dict.items():
+            if value == " ":
+                dict[key] = ""
+            if type(value) == type(1):
+                dict[key] = str(value)
+                continue
+            if type(value) == type(1.2):
+                dict[key] = str(value)
+                continue
+            if self.is_contain_chinese(value):
+                dict[key] = value.encode('UTF-8')
+        return dict
+
 
 if __name__ == '__main__':
     aa="cell388334_cell"
     print(aa.find('cell'))
     print(aa)
```

### Comparing `common-test-29.9.20/common/data/handle_common.py` & `common-test-29.9.20.1/common/data/handle_common.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/db/handle_db.py` & `common-test-29.9.20.1/common/db/handle_db.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/db/handle_db_batch.py` & `common-test-29.9.20.1/common/db/handle_db_batch.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/db/handle_mysqldb.py` & `common-test-29.9.20.1/common/db/handle_mysqldb.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/db/handle_oracle.py` & `common-test-29.9.20.1/common/db/handle_oracle.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/db/handle_sqlserver.py` & `common-test-29.9.20.1/common/db/handle_sqlserver.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/file/ReadFile.py` & `common-test-29.9.20.1/common/file/ReadFile.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/file/handle_excel.py` & `common-test-29.9.20.1/common/file/handle_excel.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,35 +213,37 @@
     # 跳过标题行，从第二行开始取数据
     _mysql = None
     if DataProcess.isNotNull(get_system_key(Constant.TEST_SRTCYCLE_ID)):
         _config = {'key': 'traffic', 'env': 'test'}
         _mysql = MysqlDB(_config)
     for row in range(_index, sh.nrows):
         d = dict()
-        d['_excelPath'] = data_file
-        d['_sheetName'] = sheet
+
         # 将标题和每行数据组装成字典
         for col in range(0, sh.ncols):
             # 获取指定单元格数据(行，列)
             cell_data = sh.cell_value(row, col)
             ctype = sh.cell(row, col).ctype
             if ctype == 2 and cell_data % 1 == 0.0:
                 cell_data = int(cell_data)
             if ctype == 3:
                 date = datetime(*xldate_as_tuple(cell_data, 0))
                 cell_data = date.strftime('%Y-%m-%d')
             col_title = sh.cell_value(0, col).strip()
             d[col_title] = cell_data
             d[col_title+'_cell'] = {"row": row, "col": col}
-        #d = dict(zip(header, sh.row_values(i)))
         if check_excel_data(d, _mysql, _filter):
             if _replace:
                 temp = DataBus.get_data(d)
+                temp['_excelPath'] = data_file
+                temp['_sheetName'] = sheet
             else:
                 temp = d
+                temp['_excelPath'] = data_file
+                temp['_sheetName'] = sheet
             print_info(f'添加单个参数化用例数据: {temp}')
             data_list.append(temp)
     if DataProcess.isNotNull(get_system_key(Constant.TEST_SRTCYCLE_ID)):
         _mysql.close()
     print_info(f'用例参数化数据: {data_list}')
     return data_list
```

### Comparing `common-test-29.9.20/common/file/handle_file.py` & `common-test-29.9.20.1/common/file/handle_file.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/file/handle_reques.py` & `common-test-29.9.20.1/common/file/handle_reques.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/file/handle_system.py` & `common-test-29.9.20.1/common/file/handle_system.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/file/handle_yaml.py` & `common-test-29.9.20.1/common/file/handle_yaml.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/mq/handle_rabbit.py` & `common-test-29.9.20.1/common/mq/handle_rabbit.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/plat/ATF_platform.py` & `common-test-29.9.20.1/common/plat/ATF_platform.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/plat/jenkin_platform.py` & `common-test-29.9.20.1/common/plat/jenkin_platform.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/plat/jira_platform.py` & `common-test-29.9.20.1/common/plat/jira_platform.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/plat/mysql_platform.py` & `common-test-29.9.20.1/common/plat/mysql_platform.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/plat/service_platform.py` & `common-test-29.9.20.1/common/plat/service_platform.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/plugin/allure_plugin.py` & `common-test-29.9.20.1/common/plugin/allure_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/plugin/assert_plugin.py` & `common-test-29.9.20.1/common/plugin/assert_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/plugin/atf_plugin.py` & `common-test-29.9.20.1/common/plugin/atf_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/plugin/data_bus.py` & `common-test-29.9.20.1/common/plugin/data_bus.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/plugin/data_plugin.py` & `common-test-29.9.20.1/common/plugin/data_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/plugin/file_plugin.py` & `common-test-29.9.20.1/common/plugin/file_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -261,15 +261,16 @@
                 _flag = True
             else:
                 _flag = False
         return _flag
 
 
 if __name__ == '__main__':
-    str="['aa','bb']"
+    DataBus.set_key('883434','9999999')
+    print(FilePlugin.load_file('aa.json', _dict={'ticketNo':'883334','registrationNo':'733','subFrom':DataBus.get_key('883434')}))
```

### Comparing `common-test-29.9.20/common/plugin/hooks_plugin.py` & `common-test-29.9.20.1/common/plugin/hooks_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/plugin/pytest_playwright.py` & `common-test-29.9.20.1/common/plugin/pytest_playwright.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/plugin/pytest_plugin.py` & `common-test-29.9.20.1/common/plugin/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common_test.egg-info/PKG-INFO` & `common-test-29.9.20.1/common_test.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: common-test
-Version: 29.9.20
+Version: 29.9.20.1
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: shiqiang.ou
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `common-test-29.9.20/common_test.egg-info/SOURCES.txt` & `common-test-29.9.20.1/common_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common_test.egg-info/requires.txt` & `common-test-29.9.20.1/common_test.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/setup.py` & `common-test-29.9.20.1/setup.py`

 * *Files identical despite different names*

