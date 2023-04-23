# Comparing `tmp/dead_simple_framework-1.3.2.tar.gz` & `tmp/dead_simple_framework-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dead_simple_framework-1.3.2.tar", last modified: Sun Feb 27 01:41:12 2022, max compression
+gzip compressed data, was "dead_simple_framework-1.3.3.tar", last modified: Sun Apr 23 02:51:27 2023, max compression
```

## Comparing `dead_simple_framework-1.3.2.tar` & `dead_simple_framework-1.3.3.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2022-02-27 01:41:12.201654 dead_simple_framework-1.3.2/
--rw-r--r--   0 pswanson   (502) staff       (20)     6373 2022-02-27 01:41:12.200867 dead_simple_framework-1.3.2/PKG-INFO
--rw-r--r--   0 pswanson   (502) staff       (20)     4847 2022-02-27 01:41:11.000000 dead_simple_framework-1.3.2/README.md
-drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2022-02-27 01:41:12.154963 dead_simple_framework-1.3.2/dead_simple_framework/
--rw-r--r--   0 pswanson   (502) staff       (20)      433 2022-02-27 01:41:11.000000 dead_simple_framework-1.3.2/dead_simple_framework/__init__.py
-drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2022-02-27 01:41:12.164311 dead_simple_framework-1.3.2/dead_simple_framework/api/
--rw-r--r--   0 pswanson   (502) staff       (20)      139 2022-02-27 01:41:11.000000 dead_simple_framework-1.3.2/dead_simple_framework/api/__init__.py
--rw-r--r--   0 pswanson   (502) staff       (20)     4144 2022-02-27 01:41:11.000000 dead_simple_framework-1.3.2/dead_simple_framework/api/client.py
--rw-r--r--   0 pswanson   (502) staff       (20)     1146 2022-02-27 01:41:11.000000 dead_simple_framework-1.3.2/dead_simple_framework/api/errors.py
--rw-r--r--   0 pswanson   (502) staff       (20)    15252 2022-02-27 01:41:11.000000 dead_simple_framework-1.3.2/dead_simple_framework/api/main.py
--rw-r--r--   0 pswanson   (502) staff       (20)    10066 2022-02-27 01:41:11.000000 dead_simple_framework-1.3.2/dead_simple_framework/api/utils.py
-drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2022-02-27 01:41:12.165408 dead_simple_framework-1.3.2/dead_simple_framework/cache/
--rw-r--r--   0 pswanson   (502) staff       (20)       23 2022-02-27 01:41:11.000000 dead_simple_framework-1.3.2/dead_simple_framework/cache/__init__.py
--rw-r--r--   0 pswanson   (502) staff       (20)     3670 2022-02-27 01:41:11.000000 dead_simple_framework-1.3.2/dead_simple_framework/cache/main.py
-drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2022-02-27 01:41:12.173668 dead_simple_framework-1.3.2/dead_simple_framework/config/
--rw-r--r--   0 pswanson   (502) staff       (20)      422 2022-02-27 01:41:11.000000 dead_simple_framework-1.3.2/dead_simple_framework/config/__init__.py
--rw-r--r--   0 pswanson   (502) staff       (20)     1949 2022-02-27 01:41:11.000000 dead_simple_framework-1.3.2/dead_simple_framework/config/config.py
--rw-r--r--   0 pswanson   (502) staff       (20)     1743 2022-02-27 01:41:11.000000 dead_simple_framework-1.3.2/dead_simple_framework/config/route.py
--rw-r--r--   0 pswanson   (502) staff       (20)     3611 2022-02-27 01:41:11.000000 dead_simple_framework-1.3.2/dead_simple_framework/config/schema.py
-drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2022-02-27 01:41:12.182903 dead_simple_framework-1.3.2/dead_simple_framework/config/settings/
--rw-r--r--   0 pswanson   (502) staff       (20)      305 2022-02-27 01:41:11.000000 dead_simple_framework-1.3.2/dead_simple_framework/config/settings/__init__.py
--rw-r--r--   0 pswanson   (502) staff       (20)     1865 2022-02-27 01:41:11.000000 dead_simple_framework-1.3.2/dead_simple_framework/config/settings/app_settings.py
--rw-r--r--   0 pswanson   (502) staff       (20)     1831 2022-02-27 01:41:11.000000 dead_simple_framework-1.3.2/dead_simple_framework/config/settings/jwt_settings.py
--rw-r--r--   0 pswanson   (502) staff       (20)     2385 2022-02-27 01:41:11.000000 dead_simple_framework-1.3.2/dead_simple_framework/config/settings/main.py
--rw-r--r--   0 pswanson   (502) staff       (20)     6280 2022-02-27 01:41:11.000000 dead_simple_framework-1.3.2/dead_simple_framework/config/settings/mongodb_settings.py
--rw-r--r--   0 pswanson   (502) staff       (20)     4085 2022-02-27 01:41:11.000000 dead_simple_framework-1.3.2/dead_simple_framework/config/settings/rabbitmq_settings.py
--rw-r--r--   0 pswanson   (502) staff       (20)     3048 2022-02-27 01:41:11.000000 dead_simple_framework-1.3.2/dead_simple_framework/config/settings/redis_settings.py
--rw-r--r--   0 pswanson   (502) staff       (20)     1587 2022-02-27 01:41:11.000000 dead_simple_framework-1.3.2/dead_simple_framework/config/settings/sentry_settings.py
--rw-r--r--   0 pswanson   (502) staff       (20)      558 2022-02-27 01:41:11.000000 dead_simple_framework-1.3.2/dead_simple_framework/config/settings/setting.py
--rw-r--r--   0 pswanson   (502) staff       (20)     1400 2022-02-27 01:41:11.000000 dead_simple_framework-1.3.2/dead_simple_framework/config/settings/slack_settings.py
--rw-r--r--   0 pswanson   (502) staff       (20)     1947 2022-02-27 01:41:11.000000 dead_simple_framework-1.3.2/dead_simple_framework/config/task.py
-drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2022-02-27 01:41:12.191502 dead_simple_framework-1.3.2/dead_simple_framework/database/
--rw-r--r--   0 pswanson   (502) staff       (20)       91 2022-02-27 01:41:11.000000 dead_simple_framework-1.3.2/dead_simple_framework/database/__init__.py
--rw-r--r--   0 pswanson   (502) staff       (20)     1756 2022-02-27 01:41:11.000000 dead_simple_framework-1.3.2/dead_simple_framework/database/fixtures.py
--rw-r--r--   0 pswanson   (502) staff       (20)     3708 2022-02-27 01:41:11.000000 dead_simple_framework-1.3.2/dead_simple_framework/database/index.py
--rw-r--r--   0 pswanson   (502) staff       (20)     4295 2022-02-27 01:41:11.000000 dead_simple_framework-1.3.2/dead_simple_framework/database/main.py
--rw-r--r--   0 pswanson   (502) staff       (20)      568 2022-02-27 01:41:11.000000 dead_simple_framework-1.3.2/dead_simple_framework/database/utils.py
--rw-r--r--   0 pswanson   (502) staff       (20)      598 2022-02-27 01:41:11.000000 dead_simple_framework-1.3.2/dead_simple_framework/encoder.py
-drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2022-02-27 01:41:12.195481 dead_simple_framework-1.3.2/dead_simple_framework/handlers/
--rw-r--r--   0 pswanson   (502) staff       (20)      288 2022-02-27 01:41:11.000000 dead_simple_framework-1.3.2/dead_simple_framework/handlers/__init__.py
--rw-r--r--   0 pswanson   (502) staff       (20)     1969 2022-02-27 01:41:11.000000 dead_simple_framework-1.3.2/dead_simple_framework/handlers/default.py
--rw-r--r--   0 pswanson   (502) staff       (20)     4775 2022-02-27 01:41:11.000000 dead_simple_framework-1.3.2/dead_simple_framework/handlers/login.py
--rw-r--r--   0 pswanson   (502) staff       (20)     3514 2022-02-27 01:41:11.000000 dead_simple_framework-1.3.2/dead_simple_framework/handlers/permissions.py
--rw-r--r--   0 pswanson   (502) staff       (20)     4483 2022-02-27 01:41:11.000000 dead_simple_framework-1.3.2/dead_simple_framework/handlers/users.py
--rw-r--r--   0 pswanson   (502) staff       (20)       61 2022-02-27 01:41:11.000000 dead_simple_framework-1.3.2/dead_simple_framework/jwt.py
--rw-r--r--   0 pswanson   (502) staff       (20)     4083 2022-02-27 01:41:11.000000 dead_simple_framework-1.3.2/dead_simple_framework/main.py
--rw-r--r--   0 pswanson   (502) staff       (20)     2685 2022-02-27 01:41:11.000000 dead_simple_framework-1.3.2/dead_simple_framework/router.py
--rw-r--r--   0 pswanson   (502) staff       (20)     4511 2022-02-27 01:41:11.000000 dead_simple_framework-1.3.2/dead_simple_framework/slack.py
-drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2022-02-27 01:41:12.198917 dead_simple_framework-1.3.2/dead_simple_framework/tasks/
--rw-r--r--   0 pswanson   (502) staff       (20)       30 2022-02-27 01:41:11.000000 dead_simple_framework-1.3.2/dead_simple_framework/tasks/__init__.py
--rw-r--r--   0 pswanson   (502) staff       (20)    12468 2022-02-27 01:41:11.000000 dead_simple_framework-1.3.2/dead_simple_framework/tasks/main.py
--rw-r--r--   0 pswanson   (502) staff       (20)     3454 2022-02-27 01:41:11.000000 dead_simple_framework-1.3.2/dead_simple_framework/tasks/task.py
--rw-r--r--   0 pswanson   (502) staff       (20)     1306 2022-02-27 01:41:11.000000 dead_simple_framework-1.3.2/dead_simple_framework/tasks/utils.py
-drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2022-02-27 01:41:12.160189 dead_simple_framework-1.3.2/dead_simple_framework.egg-info/
--rw-r--r--   0 pswanson   (502) staff       (20)     6373 2022-02-27 01:41:11.000000 dead_simple_framework-1.3.2/dead_simple_framework.egg-info/PKG-INFO
--rw-r--r--   0 pswanson   (502) staff       (20)     1984 2022-02-27 01:41:11.000000 dead_simple_framework-1.3.2/dead_simple_framework.egg-info/SOURCES.txt
--rw-r--r--   0 pswanson   (502) staff       (20)        1 2022-02-27 01:41:11.000000 dead_simple_framework-1.3.2/dead_simple_framework.egg-info/dependency_links.txt
--rw-r--r--   0 pswanson   (502) staff       (20)      146 2022-02-27 01:41:11.000000 dead_simple_framework-1.3.2/dead_simple_framework.egg-info/requires.txt
--rw-r--r--   0 pswanson   (502) staff       (20)       22 2022-02-27 01:41:11.000000 dead_simple_framework-1.3.2/dead_simple_framework.egg-info/top_level.txt
--rw-r--r--   0 pswanson   (502) staff       (20)       38 2022-02-27 01:41:12.202041 dead_simple_framework-1.3.2/setup.cfg
--rw-r--r--   0 pswanson   (502) staff       (20)      824 2022-02-27 01:40:35.000000 dead_simple_framework-1.3.2/setup.py
+drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2023-04-23 02:51:27.164383 dead_simple_framework-1.3.3/
+-rw-r--r--   0 pswanson   (502) staff       (20)     5206 2023-04-23 02:51:27.163915 dead_simple_framework-1.3.3/PKG-INFO
+-rw-r--r--   0 pswanson   (502) staff       (20)     4847 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/README.md
+drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2023-04-23 02:51:27.123235 dead_simple_framework-1.3.3/dead_simple_framework/
+-rw-r--r--   0 pswanson   (502) staff       (20)      433 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/__init__.py
+drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2023-04-23 02:51:27.129879 dead_simple_framework-1.3.3/dead_simple_framework/api/
+-rw-r--r--   0 pswanson   (502) staff       (20)      139 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/api/__init__.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     4144 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/api/client.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     1146 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/api/errors.py
+-rw-r--r--   0 pswanson   (502) staff       (20)    15354 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/api/main.py
+-rw-r--r--   0 pswanson   (502) staff       (20)    10066 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/api/utils.py
+drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2023-04-23 02:51:27.131079 dead_simple_framework-1.3.3/dead_simple_framework/cache/
+-rw-r--r--   0 pswanson   (502) staff       (20)       23 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/cache/__init__.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     3670 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/cache/main.py
+drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2023-04-23 02:51:27.133445 dead_simple_framework-1.3.3/dead_simple_framework/config/
+-rw-r--r--   0 pswanson   (502) staff       (20)      422 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/config/__init__.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     1949 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/config/config.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     1743 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/config/route.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     3611 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/config/schema.py
+drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2023-04-23 02:51:27.140115 dead_simple_framework-1.3.3/dead_simple_framework/config/settings/
+-rw-r--r--   0 pswanson   (502) staff       (20)      305 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/config/settings/__init__.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     1865 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/config/settings/app_settings.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     1831 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/config/settings/jwt_settings.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     2385 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/config/settings/main.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     6280 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/config/settings/mongodb_settings.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     4085 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/config/settings/rabbitmq_settings.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     3048 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/config/settings/redis_settings.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     1587 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/config/settings/sentry_settings.py
+-rw-r--r--   0 pswanson   (502) staff       (20)      558 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/config/settings/setting.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     1400 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/config/settings/slack_settings.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     1947 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/config/task.py
+drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2023-04-23 02:51:27.152370 dead_simple_framework-1.3.3/dead_simple_framework/database/
+-rw-r--r--   0 pswanson   (502) staff       (20)       91 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/database/__init__.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     1756 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/database/fixtures.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     3708 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/database/index.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     4295 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/database/main.py
+-rw-r--r--   0 pswanson   (502) staff       (20)      568 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/database/utils.py
+-rw-r--r--   0 pswanson   (502) staff       (20)      598 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/encoder.py
+drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2023-04-23 02:51:27.158166 dead_simple_framework-1.3.3/dead_simple_framework/handlers/
+-rw-r--r--   0 pswanson   (502) staff       (20)      288 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/handlers/__init__.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     1969 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/handlers/default.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     4775 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/handlers/login.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     3514 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/handlers/permissions.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     4483 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/handlers/users.py
+-rw-r--r--   0 pswanson   (502) staff       (20)       61 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/jwt.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     4083 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/main.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     2685 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/router.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     4511 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/slack.py
+drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2023-04-23 02:51:27.159889 dead_simple_framework-1.3.3/dead_simple_framework/tasks/
+-rw-r--r--   0 pswanson   (502) staff       (20)       30 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/tasks/__init__.py
+-rw-r--r--   0 pswanson   (502) staff       (20)    12468 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/tasks/main.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     3454 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/tasks/task.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     1306 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/tasks/utils.py
+drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2023-04-23 02:51:27.126947 dead_simple_framework-1.3.3/dead_simple_framework.egg-info/
+-rw-r--r--   0 pswanson   (502) staff       (20)     5206 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework.egg-info/PKG-INFO
+-rw-r--r--   0 pswanson   (502) staff       (20)     1984 2023-04-23 02:51:27.000000 dead_simple_framework-1.3.3/dead_simple_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 pswanson   (502) staff       (20)        1 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 pswanson   (502) staff       (20)      146 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework.egg-info/requires.txt
+-rw-r--r--   0 pswanson   (502) staff       (20)       22 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework.egg-info/top_level.txt
+-rw-r--r--   0 pswanson   (502) staff       (20)       38 2023-04-23 02:51:27.164532 dead_simple_framework-1.3.3/setup.cfg
+-rw-r--r--   0 pswanson   (502) staff       (20)      824 2023-04-23 02:49:25.000000 dead_simple_framework-1.3.3/setup.py
```

### Comparing `dead_simple_framework-1.3.2/PKG-INFO` & `dead_simple_framework-1.3.3/dead_simple_framework.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,154 +1,153 @@
 Metadata-Version: 2.1
-Name: dead_simple_framework
-Version: 1.3.2
+Name: dead-simple-framework
+Version: 1.3.3
 Summary: RESTful Flask framework with builtin MongoDB, Redis, Celery, Sentry and Slack integrations
 Home-page: https://github.com/Topazoo/dead_simple_framework
 Author: Peter Swanson
 Author-email: pswanson@ucdavis.edu
 License: MIT
-Description: # 🙈 Dead Simple Web Framework 🙉
-        
-        [![Python](https://img.shields.io/badge/Python-3.5.7+-blue.svg)](https://www.python.org/downloads/)
-        [![Flask](https://img.shields.io/badge/Flask-1.1.1-yellow.svg)](https://flask.palletsprojects.com/en/1.1.x/)
-        [![MongoDB/Pymongo](https://img.shields.io/badge/MongoDB-4.2-green.svg)](https://docs.mongodb.com/drivers/pymongo)
-        [![PyPi](https://img.shields.io/badge/View%20On-PyPi-orange.svg)](https://pypi.org/project/dead-simple-framework/)
-        
-        
-        ## Overview:
-        
-        A RESTful Flask framework with MongoDB, Redis, Celery, Slack and Sentry integrations:
-        
-        Backend:
-        
-        - Flask [Framework]
-        - MongoDB [Database]
-        - Redis [Cache]
-        - Celery + RabbitMQ [Async Tasks]
-        - Slack + Sentry [Logging]
-        
-        ## Installing:
-        
-        ```sh
-        $ pip install dead-simple-framework
-        ```
-        
-        
-        ## Configuration:
-        
-        TODO - DOCS
-        
-        ## Example Application (`demo.py`):
-        
-        
-        ```python
-        from dead_simple_framework import Route, RouteHandler, Application
-        from dead_simple_framework.handlers import UserRouteHandler, LoginRouteHandler, Permissions, DefaultPermissionsRouteHandler
-        from dead_simple_framework.database import Indices
-        from dead_simple_framework.api.errors import API_Error
-        from dead_simple_framework.api.utils import JsonError
-        
-        # Method that throws a sample error
-        def throw(msg): raise API_Error(msg, 400)
-        
-        # App config for a simple blog application with user accounts
-        sample_config = {
-            'routes': {
-                # Users
-                'users': Route(
-                    # Route with a built-in handler for creating, updating, fetching and deleting users
-                    # Only authenticated users can perform certain operations.
-                    # Adding a `verifier` to the class will let you allow only a specific user to update 
-                    # their data or delete their account.
-                    url = '/api/users',
-                    handler=UserRouteHandler(permissions=Permissions(
-                        PUT='USER', PATCH='USER', GET='USER', DELETE='USER'
-                    )),
-                    # The schema controls what data can be passed to the endpoint
-                    # In this case, a user ObjectId is required and the only property
-                    # supported. 
-                    schema={
-                        'GET': {
-                            'type': 'object',
-                            'properties': {
-                                '_id': {'type': 'string'}
-                            },
-                            'required': ['_id']
-                        }
+Requires-Python: >=3.5
+Description-Content-Type: text/markdown
+
+# 🙈 Dead Simple Web Framework 🙉
+
+[![Python](https://img.shields.io/badge/Python-3.5.7+-blue.svg)](https://www.python.org/downloads/)
+[![Flask](https://img.shields.io/badge/Flask-1.1.1-yellow.svg)](https://flask.palletsprojects.com/en/1.1.x/)
+[![MongoDB/Pymongo](https://img.shields.io/badge/MongoDB-4.2-green.svg)](https://docs.mongodb.com/drivers/pymongo)
+[![PyPi](https://img.shields.io/badge/View%20On-PyPi-orange.svg)](https://pypi.org/project/dead-simple-framework/)
+
+
+## Overview:
+
+A RESTful Flask framework with MongoDB, Redis, Celery, Slack and Sentry integrations:
+
+Backend:
+
+- Flask [Framework]
+- MongoDB [Database]
+- Redis [Cache]
+- Celery + RabbitMQ [Async Tasks]
+- Slack + Sentry [Logging]
+
+## Installing:
+
+```sh
+$ pip install dead-simple-framework
+```
+
+
+## Configuration:
+
+TODO - DOCS
+
+## Example Application (`demo.py`):
+
+
+```python
+from dead_simple_framework import Route, RouteHandler, Application
+from dead_simple_framework.handlers import UserRouteHandler, LoginRouteHandler, Permissions, DefaultPermissionsRouteHandler
+from dead_simple_framework.database import Indices
+from dead_simple_framework.api.errors import API_Error
+from dead_simple_framework.api.utils import JsonError
+
+# Method that throws a sample error
+def throw(msg): raise API_Error(msg, 400)
+
+# App config for a simple blog application with user accounts
+sample_config = {
+    'routes': {
+        # Users
+        'users': Route(
+            # Route with a built-in handler for creating, updating, fetching and deleting users
+            # Only authenticated users can perform certain operations.
+            # Adding a `verifier` to the class will let you allow only a specific user to update 
+            # their data or delete their account.
+            url = '/api/users',
+            handler=UserRouteHandler(permissions=Permissions(
+                PUT='USER', PATCH='USER', GET='USER', DELETE='USER'
+            )),
+            # The schema controls what data can be passed to the endpoint
+            # In this case, a user ObjectId is required and the only property
+            # supported. 
+            schema={
+                'GET': {
+                    'type': 'object',
+                    'properties': {
+                        '_id': {'type': 'string'}
                     },
-                    # The MongoDB collection where data for this route should be stored
-                    # It is passed to any overloaded method handlers (e.g. a custom GET method)
-                    collection='users'
-                ),
-        
-                # Authentication
-                'authentication': Route(
-                    # Route with a built-in handler for authenticating users and issuing a JSON Web Token
-                    url='/api/authenticate', 
-                    handler=LoginRouteHandler(),
-                    # It relies on the same collection as the core `users` route
-                    collection='users'
-                ),
-        
-                # Posts
-                'posts': Route(
-                    # Route with a builtin generic CRUD handler for creating, updating, fetching and deleting posts
-                    # Only authenticated users can perform certain operations.
-                    url='/api/posts',
-                    handler=DefaultPermissionsRouteHandler(permissions=Permissions(POST=['USER'], PUT=['USER'], PATCH=['USER'], DELETE=['USER'])),
-                    collection='posts'
-                ),
-        
-                # Sample Error
-                'error': Route(
-                    # Route that demonstrates built-in error handling
-                    url='/error',
-                    handler=RouteHandler(
-                        # Custom handlers allow a POST request or a GET request to create different errors
-                        POST=lambda request, payload: throw(f'POST - Error from payload {payload}'),
-                        GET=lambda request, payload: JsonError('This is a GET error', code=500),
-                    )
-                ),
-            },
-        
-            # Application settings
-            'settings': {
-                # JWT Settings determine if the app uses JWT, what the token lifespan will be and more
-                'jwt_settings': {
-                    'app_use_jwt': True,
-                    'app_jwt_lifespan': 600,
-                    'app_permissions': ['USER', 'ADMIN'],
+                    'required': ['_id']
                 }
             },
-        
-            # MongoDB indices for each collection used by the application
-            'indices': Indices({
-                'users': {
-                    'username': {
-                        'order': -1
-                    },
-                    'password': {
-                        'order': 1,
-                        'compound_with': 'username'
-                    }
-                },
-            })
+            # The MongoDB collection where data for this route should be stored
+            # It is passed to any overloaded method handlers (e.g. a custom GET method)
+            collection='users'
+        ),
+
+        # Authentication
+        'authentication': Route(
+            # Route with a built-in handler for authenticating users and issuing a JSON Web Token
+            url='/api/authenticate', 
+            handler=LoginRouteHandler(),
+            # It relies on the same collection as the core `users` route
+            collection='users'
+        ),
+
+        # Posts
+        'posts': Route(
+            # Route with a builtin generic CRUD handler for creating, updating, fetching and deleting posts
+            # Only authenticated users can perform certain operations.
+            url='/api/posts',
+            handler=DefaultPermissionsRouteHandler(permissions=Permissions(POST=['USER'], PUT=['USER'], PATCH=['USER'], DELETE=['USER'])),
+            collection='posts'
+        ),
+
+        # Sample Error
+        'error': Route(
+            # Route that demonstrates built-in error handling
+            url='/error',
+            handler=RouteHandler(
+                # Custom handlers allow a POST request or a GET request to create different errors
+                POST=lambda request, payload: throw(f'POST - Error from payload {payload}'),
+                GET=lambda request, payload: JsonError('This is a GET error', code=500),
+            )
+        ),
+    },
+
+    # Application settings
+    'settings': {
+        # JWT Settings determine if the app uses JWT, what the token lifespan will be and more
+        'jwt_settings': {
+            'app_use_jwt': True,
+            'app_jwt_lifespan': 600,
+            'app_permissions': ['USER', 'ADMIN'],
         }
-        
-        if __name__ == '__main__':
-            Application(sample_config).run()
-        ```
-        
-        - Starts a local server at http://0.0.0.0:5000/
-        
-        - Serves CRUD operations for MongoDB users collection `users` at endpoint `/api/users`
-        
-        - Issues JWT tokents for created users at endpoint `/api/authenticate`
-        
-        - Serves CRUD operations for MongoDB collection `posts` at endpoint `/api/posts`
-        
-        - Demos errors at endpoint `/error`
-        
-        
-Platform: UNKNOWN
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
+    },
+
+    # MongoDB indices for each collection used by the application
+    'indices': Indices({
+        'users': {
+            'username': {
+                'order': -1
+            },
+            'password': {
+                'order': 1,
+                'compound_with': 'username'
+            }
+        },
+    })
+}
+
+if __name__ == '__main__':
+    Application(sample_config).run()
+```
+
+- Starts a local server at http://0.0.0.0:5000/
+
+- Serves CRUD operations for MongoDB users collection `users` at endpoint `/api/users`
+
+- Issues JWT tokents for created users at endpoint `/api/authenticate`
+
+- Serves CRUD operations for MongoDB collection `posts` at endpoint `/api/posts`
+
+- Demos errors at endpoint `/error`
+
```

### Comparing `dead_simple_framework-1.3.2/README.md` & `dead_simple_framework-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.2/dead_simple_framework/api/client.py` & `dead_simple_framework-1.3.3/dead_simple_framework/api/client.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.2/dead_simple_framework/api/errors.py` & `dead_simple_framework-1.3.3/dead_simple_framework/api/errors.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.2/dead_simple_framework/api/main.py` & `dead_simple_framework-1.3.3/dead_simple_framework/api/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -265,15 +265,15 @@
         if collection is not None and num_parameters < 3:
             raise API_Error(f'Handler [{logic_func.__name__}] for route [{route_name}] supports [{num_parameters}] arguments. Must support 3 (request, payload, collection)', 500)
         elif num_parameters < 2:
             raise API_Error(f'Handler [{logic_func.__name__}] for route [{route_name}] supports [{num_parameters}] arguments. Must support 2 (request, payload)', 500)
         
 
     @classmethod
-    def main(cls) -> Response:
+    def main(cls, **kwargs) -> Response:
         ''' Called when the speciied endpoint is sent an HTTP request. Delegates 
             to the appropriate handler based on the request method or returns a JSON
             formatted error if the method is not supported.
             --> request : The HTTP request sent to the server.
             <-- JSON containing the HTTP status code signifying the request's success or failure and
                 all other data returned from the server.
         '''
@@ -287,14 +287,17 @@
 
             # Normalize query params
             if str(request.method) == 'GET':
                 payload = parse_query_string(request.query_string.decode()) if request.query_string.decode() else {}
             else:
                 payload = request.get_json(force=True) if request.data else dict(request.form)
 
+            # Add URL params over query params
+            payload = {**payload, **kwargs}
+
             # Ensure user defined logic can accept required arguments or throw a warning
             cls._check_logic(route.name, logic, route.collection)
 
             # Ensure the payload passes schema validation
             validation_error = route.schema_handler.validate_request(request.url_rule, request.method, payload)
             if validation_error:
                 return JsonResponse(validation_error, 400)
```

### Comparing `dead_simple_framework-1.3.2/dead_simple_framework/api/utils.py` & `dead_simple_framework-1.3.3/dead_simple_framework/api/utils.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.2/dead_simple_framework/cache/main.py` & `dead_simple_framework-1.3.3/dead_simple_framework/cache/main.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.2/dead_simple_framework/config/config.py` & `dead_simple_framework-1.3.3/dead_simple_framework/config/config.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.2/dead_simple_framework/config/route.py` & `dead_simple_framework-1.3.3/dead_simple_framework/config/route.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.2/dead_simple_framework/config/schema.py` & `dead_simple_framework-1.3.3/dead_simple_framework/config/schema.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.2/dead_simple_framework/config/settings/app_settings.py` & `dead_simple_framework-1.3.3/dead_simple_framework/config/settings/app_settings.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.2/dead_simple_framework/config/settings/jwt_settings.py` & `dead_simple_framework-1.3.3/dead_simple_framework/config/settings/jwt_settings.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.2/dead_simple_framework/config/settings/main.py` & `dead_simple_framework-1.3.3/dead_simple_framework/config/settings/main.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.2/dead_simple_framework/config/settings/mongodb_settings.py` & `dead_simple_framework-1.3.3/dead_simple_framework/config/settings/mongodb_settings.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.2/dead_simple_framework/config/settings/rabbitmq_settings.py` & `dead_simple_framework-1.3.3/dead_simple_framework/config/settings/rabbitmq_settings.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.2/dead_simple_framework/config/settings/redis_settings.py` & `dead_simple_framework-1.3.3/dead_simple_framework/config/settings/redis_settings.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.2/dead_simple_framework/config/settings/sentry_settings.py` & `dead_simple_framework-1.3.3/dead_simple_framework/config/settings/sentry_settings.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.2/dead_simple_framework/config/settings/setting.py` & `dead_simple_framework-1.3.3/dead_simple_framework/config/settings/setting.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.2/dead_simple_framework/config/settings/slack_settings.py` & `dead_simple_framework-1.3.3/dead_simple_framework/config/settings/slack_settings.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.2/dead_simple_framework/config/task.py` & `dead_simple_framework-1.3.3/dead_simple_framework/config/task.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.2/dead_simple_framework/database/fixtures.py` & `dead_simple_framework-1.3.3/dead_simple_framework/database/fixtures.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.2/dead_simple_framework/database/index.py` & `dead_simple_framework-1.3.3/dead_simple_framework/database/index.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.2/dead_simple_framework/database/main.py` & `dead_simple_framework-1.3.3/dead_simple_framework/database/main.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.2/dead_simple_framework/database/utils.py` & `dead_simple_framework-1.3.3/dead_simple_framework/database/utils.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.2/dead_simple_framework/encoder.py` & `dead_simple_framework-1.3.3/dead_simple_framework/encoder.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.2/dead_simple_framework/handlers/default.py` & `dead_simple_framework-1.3.3/dead_simple_framework/handlers/default.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.2/dead_simple_framework/handlers/login.py` & `dead_simple_framework-1.3.3/dead_simple_framework/handlers/login.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.2/dead_simple_framework/handlers/permissions.py` & `dead_simple_framework-1.3.3/dead_simple_framework/handlers/permissions.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.2/dead_simple_framework/handlers/users.py` & `dead_simple_framework-1.3.3/dead_simple_framework/handlers/users.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.2/dead_simple_framework/main.py` & `dead_simple_framework-1.3.3/dead_simple_framework/main.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.2/dead_simple_framework/router.py` & `dead_simple_framework-1.3.3/dead_simple_framework/router.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.2/dead_simple_framework/slack.py` & `dead_simple_framework-1.3.3/dead_simple_framework/slack.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.2/dead_simple_framework/tasks/main.py` & `dead_simple_framework-1.3.3/dead_simple_framework/tasks/main.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.2/dead_simple_framework/tasks/task.py` & `dead_simple_framework-1.3.3/dead_simple_framework/tasks/task.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.2/dead_simple_framework/tasks/utils.py` & `dead_simple_framework-1.3.3/dead_simple_framework/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.2/dead_simple_framework.egg-info/PKG-INFO` & `dead_simple_framework-1.3.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,154 +1,153 @@
 Metadata-Version: 2.1
-Name: dead-simple-framework
-Version: 1.3.2
+Name: dead_simple_framework
+Version: 1.3.3
 Summary: RESTful Flask framework with builtin MongoDB, Redis, Celery, Sentry and Slack integrations
 Home-page: https://github.com/Topazoo/dead_simple_framework
 Author: Peter Swanson
 Author-email: pswanson@ucdavis.edu
 License: MIT
-Description: # 🙈 Dead Simple Web Framework 🙉
-        
-        [![Python](https://img.shields.io/badge/Python-3.5.7+-blue.svg)](https://www.python.org/downloads/)
-        [![Flask](https://img.shields.io/badge/Flask-1.1.1-yellow.svg)](https://flask.palletsprojects.com/en/1.1.x/)
-        [![MongoDB/Pymongo](https://img.shields.io/badge/MongoDB-4.2-green.svg)](https://docs.mongodb.com/drivers/pymongo)
-        [![PyPi](https://img.shields.io/badge/View%20On-PyPi-orange.svg)](https://pypi.org/project/dead-simple-framework/)
-        
-        
-        ## Overview:
-        
-        A RESTful Flask framework with MongoDB, Redis, Celery, Slack and Sentry integrations:
-        
-        Backend:
-        
-        - Flask [Framework]
-        - MongoDB [Database]
-        - Redis [Cache]
-        - Celery + RabbitMQ [Async Tasks]
-        - Slack + Sentry [Logging]
-        
-        ## Installing:
-        
-        ```sh
-        $ pip install dead-simple-framework
-        ```
-        
-        
-        ## Configuration:
-        
-        TODO - DOCS
-        
-        ## Example Application (`demo.py`):
-        
-        
-        ```python
-        from dead_simple_framework import Route, RouteHandler, Application
-        from dead_simple_framework.handlers import UserRouteHandler, LoginRouteHandler, Permissions, DefaultPermissionsRouteHandler
-        from dead_simple_framework.database import Indices
-        from dead_simple_framework.api.errors import API_Error
-        from dead_simple_framework.api.utils import JsonError
-        
-        # Method that throws a sample error
-        def throw(msg): raise API_Error(msg, 400)
-        
-        # App config for a simple blog application with user accounts
-        sample_config = {
-            'routes': {
-                # Users
-                'users': Route(
-                    # Route with a built-in handler for creating, updating, fetching and deleting users
-                    # Only authenticated users can perform certain operations.
-                    # Adding a `verifier` to the class will let you allow only a specific user to update 
-                    # their data or delete their account.
-                    url = '/api/users',
-                    handler=UserRouteHandler(permissions=Permissions(
-                        PUT='USER', PATCH='USER', GET='USER', DELETE='USER'
-                    )),
-                    # The schema controls what data can be passed to the endpoint
-                    # In this case, a user ObjectId is required and the only property
-                    # supported. 
-                    schema={
-                        'GET': {
-                            'type': 'object',
-                            'properties': {
-                                '_id': {'type': 'string'}
-                            },
-                            'required': ['_id']
-                        }
+Requires-Python: >=3.5
+Description-Content-Type: text/markdown
+
+# 🙈 Dead Simple Web Framework 🙉
+
+[![Python](https://img.shields.io/badge/Python-3.5.7+-blue.svg)](https://www.python.org/downloads/)
+[![Flask](https://img.shields.io/badge/Flask-1.1.1-yellow.svg)](https://flask.palletsprojects.com/en/1.1.x/)
+[![MongoDB/Pymongo](https://img.shields.io/badge/MongoDB-4.2-green.svg)](https://docs.mongodb.com/drivers/pymongo)
+[![PyPi](https://img.shields.io/badge/View%20On-PyPi-orange.svg)](https://pypi.org/project/dead-simple-framework/)
+
+
+## Overview:
+
+A RESTful Flask framework with MongoDB, Redis, Celery, Slack and Sentry integrations:
+
+Backend:
+
+- Flask [Framework]
+- MongoDB [Database]
+- Redis [Cache]
+- Celery + RabbitMQ [Async Tasks]
+- Slack + Sentry [Logging]
+
+## Installing:
+
+```sh
+$ pip install dead-simple-framework
+```
+
+
+## Configuration:
+
+TODO - DOCS
+
+## Example Application (`demo.py`):
+
+
+```python
+from dead_simple_framework import Route, RouteHandler, Application
+from dead_simple_framework.handlers import UserRouteHandler, LoginRouteHandler, Permissions, DefaultPermissionsRouteHandler
+from dead_simple_framework.database import Indices
+from dead_simple_framework.api.errors import API_Error
+from dead_simple_framework.api.utils import JsonError
+
+# Method that throws a sample error
+def throw(msg): raise API_Error(msg, 400)
+
+# App config for a simple blog application with user accounts
+sample_config = {
+    'routes': {
+        # Users
+        'users': Route(
+            # Route with a built-in handler for creating, updating, fetching and deleting users
+            # Only authenticated users can perform certain operations.
+            # Adding a `verifier` to the class will let you allow only a specific user to update 
+            # their data or delete their account.
+            url = '/api/users',
+            handler=UserRouteHandler(permissions=Permissions(
+                PUT='USER', PATCH='USER', GET='USER', DELETE='USER'
+            )),
+            # The schema controls what data can be passed to the endpoint
+            # In this case, a user ObjectId is required and the only property
+            # supported. 
+            schema={
+                'GET': {
+                    'type': 'object',
+                    'properties': {
+                        '_id': {'type': 'string'}
                     },
-                    # The MongoDB collection where data for this route should be stored
-                    # It is passed to any overloaded method handlers (e.g. a custom GET method)
-                    collection='users'
-                ),
-        
-                # Authentication
-                'authentication': Route(
-                    # Route with a built-in handler for authenticating users and issuing a JSON Web Token
-                    url='/api/authenticate', 
-                    handler=LoginRouteHandler(),
-                    # It relies on the same collection as the core `users` route
-                    collection='users'
-                ),
-        
-                # Posts
-                'posts': Route(
-                    # Route with a builtin generic CRUD handler for creating, updating, fetching and deleting posts
-                    # Only authenticated users can perform certain operations.
-                    url='/api/posts',
-                    handler=DefaultPermissionsRouteHandler(permissions=Permissions(POST=['USER'], PUT=['USER'], PATCH=['USER'], DELETE=['USER'])),
-                    collection='posts'
-                ),
-        
-                # Sample Error
-                'error': Route(
-                    # Route that demonstrates built-in error handling
-                    url='/error',
-                    handler=RouteHandler(
-                        # Custom handlers allow a POST request or a GET request to create different errors
-                        POST=lambda request, payload: throw(f'POST - Error from payload {payload}'),
-                        GET=lambda request, payload: JsonError('This is a GET error', code=500),
-                    )
-                ),
-            },
-        
-            # Application settings
-            'settings': {
-                # JWT Settings determine if the app uses JWT, what the token lifespan will be and more
-                'jwt_settings': {
-                    'app_use_jwt': True,
-                    'app_jwt_lifespan': 600,
-                    'app_permissions': ['USER', 'ADMIN'],
+                    'required': ['_id']
                 }
             },
-        
-            # MongoDB indices for each collection used by the application
-            'indices': Indices({
-                'users': {
-                    'username': {
-                        'order': -1
-                    },
-                    'password': {
-                        'order': 1,
-                        'compound_with': 'username'
-                    }
-                },
-            })
+            # The MongoDB collection where data for this route should be stored
+            # It is passed to any overloaded method handlers (e.g. a custom GET method)
+            collection='users'
+        ),
+
+        # Authentication
+        'authentication': Route(
+            # Route with a built-in handler for authenticating users and issuing a JSON Web Token
+            url='/api/authenticate', 
+            handler=LoginRouteHandler(),
+            # It relies on the same collection as the core `users` route
+            collection='users'
+        ),
+
+        # Posts
+        'posts': Route(
+            # Route with a builtin generic CRUD handler for creating, updating, fetching and deleting posts
+            # Only authenticated users can perform certain operations.
+            url='/api/posts',
+            handler=DefaultPermissionsRouteHandler(permissions=Permissions(POST=['USER'], PUT=['USER'], PATCH=['USER'], DELETE=['USER'])),
+            collection='posts'
+        ),
+
+        # Sample Error
+        'error': Route(
+            # Route that demonstrates built-in error handling
+            url='/error',
+            handler=RouteHandler(
+                # Custom handlers allow a POST request or a GET request to create different errors
+                POST=lambda request, payload: throw(f'POST - Error from payload {payload}'),
+                GET=lambda request, payload: JsonError('This is a GET error', code=500),
+            )
+        ),
+    },
+
+    # Application settings
+    'settings': {
+        # JWT Settings determine if the app uses JWT, what the token lifespan will be and more
+        'jwt_settings': {
+            'app_use_jwt': True,
+            'app_jwt_lifespan': 600,
+            'app_permissions': ['USER', 'ADMIN'],
         }
-        
-        if __name__ == '__main__':
-            Application(sample_config).run()
-        ```
-        
-        - Starts a local server at http://0.0.0.0:5000/
-        
-        - Serves CRUD operations for MongoDB users collection `users` at endpoint `/api/users`
-        
-        - Issues JWT tokents for created users at endpoint `/api/authenticate`
-        
-        - Serves CRUD operations for MongoDB collection `posts` at endpoint `/api/posts`
-        
-        - Demos errors at endpoint `/error`
-        
-        
-Platform: UNKNOWN
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
+    },
+
+    # MongoDB indices for each collection used by the application
+    'indices': Indices({
+        'users': {
+            'username': {
+                'order': -1
+            },
+            'password': {
+                'order': 1,
+                'compound_with': 'username'
+            }
+        },
+    })
+}
+
+if __name__ == '__main__':
+    Application(sample_config).run()
+```
+
+- Starts a local server at http://0.0.0.0:5000/
+
+- Serves CRUD operations for MongoDB users collection `users` at endpoint `/api/users`
+
+- Issues JWT tokents for created users at endpoint `/api/authenticate`
+
+- Serves CRUD operations for MongoDB collection `posts` at endpoint `/api/posts`
+
+- Demos errors at endpoint `/error`
+
```

### Comparing `dead_simple_framework-1.3.2/dead_simple_framework.egg-info/SOURCES.txt` & `dead_simple_framework-1.3.3/dead_simple_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.2/setup.py` & `dead_simple_framework-1.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 setuptools.setup(
     author="Peter Swanson",
     author_email="pswanson@ucdavis.edu",
     name='dead_simple_framework',
     license="MIT",
     description='RESTful Flask framework with builtin MongoDB, Redis, Celery, Sentry and Slack integrations',
-    version='v1.3.2',
+    version='v1.3.3',
     long_description=README,
     url='https://github.com/Topazoo/dead_simple_framework',
     packages=setuptools.find_packages(),
     python_requires=">=3.5",
     install_requires=['flask', 'pymongo', 'celery', 'flask-cors', 'requests', 'redis', 'eventlet', 'pyOpenSSL', 'Flask-JWT-Extended', 'passlib', 'jsonschema', 'sentry-sdk[flask]', 'slack-sdk', 'Flask-PyMongo'],
     long_description_content_type='text/markdown',
     classifiers=[]
```

