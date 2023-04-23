# Comparing `tmp/OctoBot-Services-1.5.4.tar.gz` & `tmp/OctoBot-Services-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OctoBot-Services-1.5.4.tar", last modified: Fri Mar 31 16:56:57 2023, max compression
+gzip compressed data, was "OctoBot-Services-1.5.5.tar", last modified: Sun Apr 23 11:26:15 2023, max compression
```

## Comparing `OctoBot-Services-1.5.4.tar` & `OctoBot-Services-1.5.5.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:56:57.646321 OctoBot-Services-1.5.4/
--rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-03-31 16:55:56.000000 OctoBot-Services-1.5.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-03-31 16:55:56.000000 OctoBot-Services-1.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-03-31 16:55:56.000000 OctoBot-Services-1.5.4/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:56:57.638320 OctoBot-Services-1.5.4/OctoBot_Services.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-03-31 16:56:57.000000 OctoBot-Services-1.5.4/OctoBot_Services.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-03-31 16:56:57.000000 OctoBot-Services-1.5.4/OctoBot_Services.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 16:56:57.000000 OctoBot-Services-1.5.4/OctoBot_Services.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 16:56:57.000000 OctoBot-Services-1.5.4/OctoBot_Services.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-03-31 16:56:57.000000 OctoBot-Services-1.5.4/OctoBot_Services.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-31 16:56:57.000000 OctoBot-Services-1.5.4/OctoBot_Services.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-03-31 16:56:57.646321 OctoBot-Services-1.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-03-31 16:55:56.000000 OctoBot-Services-1.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:56:57.638320 OctoBot-Services-1.5.4/octobot_services/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-03-31 16:55:56.000000 OctoBot-Services-1.5.4/octobot_services/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-03-31 16:55:56.000000 OctoBot-Services-1.5.4/octobot_services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-03-31 16:55:56.000000 OctoBot-Services-1.5.4/octobot_services/abstract_service_user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:56:57.642320 OctoBot-Services-1.5.4/octobot_services/api/
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-03-31 16:55:56.000000 OctoBot-Services-1.5.4/octobot_services/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-03-31 16:55:56.000000 OctoBot-Services-1.5.4/octobot_services/api/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-03-31 16:55:56.000000 OctoBot-Services-1.5.4/octobot_services/api/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-03-31 16:55:56.000000 OctoBot-Services-1.5.4/octobot_services/api/service_feeds.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-03-31 16:55:56.000000 OctoBot-Services-1.5.4/octobot_services/api/services.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:56:57.642320 OctoBot-Services-1.5.4/octobot_services/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-03-31 16:55:56.000000 OctoBot-Services-1.5.4/octobot_services/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-03-31 16:55:56.000000 OctoBot-Services-1.5.4/octobot_services/channel/abstract_service_feed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-03-31 16:55:56.000000 OctoBot-Services-1.5.4/octobot_services/channel/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-03-31 16:55:56.000000 OctoBot-Services-1.5.4/octobot_services/channel/user_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-03-31 16:55:56.000000 OctoBot-Services-1.5.4/octobot_services/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-03-31 16:55:56.000000 OctoBot-Services-1.5.4/octobot_services/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-03-31 16:55:56.000000 OctoBot-Services-1.5.4/octobot_services/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:56:57.642320 OctoBot-Services-1.5.4/octobot_services/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-03-31 16:55:56.000000 OctoBot-Services-1.5.4/octobot_services/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-03-31 16:55:56.000000 OctoBot-Services-1.5.4/octobot_services/interfaces/abstract_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:56:57.642320 OctoBot-Services-1.5.4/octobot_services/interfaces/bots/
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-03-31 16:55:56.000000 OctoBot-Services-1.5.4/octobot_services/interfaces/bots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18545 2023-03-31 16:55:56.000000 OctoBot-Services-1.5.4/octobot_services/interfaces/bots/abstract_bot_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-03-31 16:55:56.000000 OctoBot-Services-1.5.4/octobot_services/interfaces/interface_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:56:57.642320 OctoBot-Services-1.5.4/octobot_services/interfaces/util/
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-03-31 16:55:56.000000 OctoBot-Services-1.5.4/octobot_services/interfaces/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-03-31 16:55:56.000000 OctoBot-Services-1.5.4/octobot_services/interfaces/util/bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-03-31 16:55:56.000000 OctoBot-Services-1.5.4/octobot_services/interfaces/util/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-03-31 16:55:56.000000 OctoBot-Services-1.5.4/octobot_services/interfaces/util/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-03-31 16:55:56.000000 OctoBot-Services-1.5.4/octobot_services/interfaces/util/position.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-03-31 16:55:56.000000 OctoBot-Services-1.5.4/octobot_services/interfaces/util/profitability.py
--rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-03-31 16:55:56.000000 OctoBot-Services-1.5.4/octobot_services/interfaces/util/trader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-03-31 16:55:56.000000 OctoBot-Services-1.5.4/octobot_services/interfaces/util/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:56:57.642320 OctoBot-Services-1.5.4/octobot_services/interfaces/web/
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-03-31 16:55:56.000000 OctoBot-Services-1.5.4/octobot_services/interfaces/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-03-31 16:55:56.000000 OctoBot-Services-1.5.4/octobot_services/interfaces/web/abstract_web_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:56:57.642320 OctoBot-Services-1.5.4/octobot_services/managers/
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-03-31 16:55:56.000000 OctoBot-Services-1.5.4/octobot_services/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-03-31 16:55:56.000000 OctoBot-Services-1.5.4/octobot_services/managers/interface_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-03-31 16:55:56.000000 OctoBot-Services-1.5.4/octobot_services/managers/service_feed_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-03-31 16:55:56.000000 OctoBot-Services-1.5.4/octobot_services/managers/service_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:56:57.646321 OctoBot-Services-1.5.4/octobot_services/notification/
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-03-31 16:55:56.000000 OctoBot-Services-1.5.4/octobot_services/notification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-03-31 16:55:56.000000 OctoBot-Services-1.5.4/octobot_services/notification/formated_notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-03-31 16:55:56.000000 OctoBot-Services-1.5.4/octobot_services/notification/notification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:56:57.646321 OctoBot-Services-1.5.4/octobot_services/notifier/
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-03-31 16:55:56.000000 OctoBot-Services-1.5.4/octobot_services/notifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9261 2023-03-31 16:55:56.000000 OctoBot-Services-1.5.4/octobot_services/notifier/abstract_notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-03-31 16:55:57.000000 OctoBot-Services-1.5.4/octobot_services/notifier/notifier_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-03-31 16:55:57.000000 OctoBot-Services-1.5.4/octobot_services/octobot_channel_consumer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:56:57.646321 OctoBot-Services-1.5.4/octobot_services/service_feeds/
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-03-31 16:55:57.000000 OctoBot-Services-1.5.4/octobot_services/service_feeds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-03-31 16:55:57.000000 OctoBot-Services-1.5.4/octobot_services/service_feeds/abstract_service_feed.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-03-31 16:55:57.000000 OctoBot-Services-1.5.4/octobot_services/service_feeds/service_feed_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-03-31 16:55:57.000000 OctoBot-Services-1.5.4/octobot_services/service_feeds/service_feed_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-03-31 16:55:57.000000 OctoBot-Services-1.5.4/octobot_services/service_feeds/service_feeds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:56:57.646321 OctoBot-Services-1.5.4/octobot_services/services/
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-03-31 16:55:57.000000 OctoBot-Services-1.5.4/octobot_services/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-03-31 16:55:57.000000 OctoBot-Services-1.5.4/octobot_services/services/abstract_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-03-31 16:55:57.000000 OctoBot-Services-1.5.4/octobot_services/services/service_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:56:57.646321 OctoBot-Services-1.5.4/octobot_services/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-03-31 16:55:57.000000 OctoBot-Services-1.5.4/octobot_services/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-03-31 16:55:57.000000 OctoBot-Services-1.5.4/octobot_services/util/exchange_watcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-03-31 16:55:57.000000 OctoBot-Services-1.5.4/octobot_services/util/initializable_with_post_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-03-31 16:55:57.000000 OctoBot-Services-1.5.4/octobot_services/util/returning_startable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-03-31 16:55:57.000000 OctoBot-Services-1.5.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 16:56:57.646321 OctoBot-Services-1.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-03-31 16:55:57.000000 OctoBot-Services-1.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:56:57.646321 OctoBot-Services-1.5.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-03-31 16:55:57.000000 OctoBot-Services-1.5.4/tests/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-03-31 16:55:57.000000 OctoBot-Services-1.5.4/tests/test_interface_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-03-31 16:55:57.000000 OctoBot-Services-1.5.4/tests/test_notification_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-03-31 16:55:57.000000 OctoBot-Services-1.5.4/tests/test_service_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:26:15.847124 OctoBot-Services-1.5.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:26:15.839123 OctoBot-Services-1.5.5/OctoBot_Services.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-23 11:26:15.000000 OctoBot-Services-1.5.5/OctoBot_Services.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-04-23 11:26:15.000000 OctoBot-Services-1.5.5/OctoBot_Services.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 11:26:15.000000 OctoBot-Services-1.5.5/OctoBot_Services.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 11:26:15.000000 OctoBot-Services-1.5.5/OctoBot_Services.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-23 11:26:15.000000 OctoBot-Services-1.5.5/OctoBot_Services.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-23 11:26:15.000000 OctoBot-Services-1.5.5/OctoBot_Services.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-23 11:26:15.847124 OctoBot-Services-1.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:26:15.839123 OctoBot-Services-1.5.5/octobot_services/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/octobot_services/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/octobot_services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/octobot_services/abstract_service_user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:26:15.839123 OctoBot-Services-1.5.5/octobot_services/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/octobot_services/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/octobot_services/api/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/octobot_services/api/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/octobot_services/api/service_feeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/octobot_services/api/services.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:26:15.839123 OctoBot-Services-1.5.5/octobot_services/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/octobot_services/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/octobot_services/channel/abstract_service_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/octobot_services/channel/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/octobot_services/channel/user_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/octobot_services/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/octobot_services/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/octobot_services/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:26:15.839123 OctoBot-Services-1.5.5/octobot_services/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/octobot_services/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/octobot_services/interfaces/abstract_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:26:15.839123 OctoBot-Services-1.5.5/octobot_services/interfaces/bots/
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/octobot_services/interfaces/bots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19047 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/octobot_services/interfaces/bots/abstract_bot_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/octobot_services/interfaces/interface_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:26:15.843124 OctoBot-Services-1.5.5/octobot_services/interfaces/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/octobot_services/interfaces/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/octobot_services/interfaces/util/bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/octobot_services/interfaces/util/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/octobot_services/interfaces/util/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/octobot_services/interfaces/util/position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/octobot_services/interfaces/util/profitability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/octobot_services/interfaces/util/trader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/octobot_services/interfaces/util/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:26:15.843124 OctoBot-Services-1.5.5/octobot_services/interfaces/web/
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/octobot_services/interfaces/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/octobot_services/interfaces/web/abstract_web_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:26:15.843124 OctoBot-Services-1.5.5/octobot_services/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/octobot_services/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/octobot_services/managers/interface_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/octobot_services/managers/service_feed_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/octobot_services/managers/service_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:26:15.843124 OctoBot-Services-1.5.5/octobot_services/notification/
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/octobot_services/notification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/octobot_services/notification/formated_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/octobot_services/notification/notification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:26:15.843124 OctoBot-Services-1.5.5/octobot_services/notifier/
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/octobot_services/notifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9261 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/octobot_services/notifier/abstract_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/octobot_services/notifier/notifier_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/octobot_services/octobot_channel_consumer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:26:15.843124 OctoBot-Services-1.5.5/octobot_services/service_feeds/
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/octobot_services/service_feeds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/octobot_services/service_feeds/abstract_service_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/octobot_services/service_feeds/service_feed_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/octobot_services/service_feeds/service_feed_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/octobot_services/service_feeds/service_feeds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:26:15.843124 OctoBot-Services-1.5.5/octobot_services/services/
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/octobot_services/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/octobot_services/services/abstract_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/octobot_services/services/service_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:26:15.843124 OctoBot-Services-1.5.5/octobot_services/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/octobot_services/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/octobot_services/util/exchange_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/octobot_services/util/initializable_with_post_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/octobot_services/util/returning_startable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 11:26:15.847124 OctoBot-Services-1.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:26:15.847124 OctoBot-Services-1.5.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/tests/test_interface_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/tests/test_notification_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-23 11:25:04.000000 OctoBot-Services-1.5.5/tests/test_service_api.py
```

### Comparing `OctoBot-Services-1.5.4/CHANGELOG.md` & `OctoBot-Services-1.5.5/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [1.5.5] - 2023-04-23
+### Updated
+- [BotInterface] set_risk command now updated edited config
+
 ## [1.5.4] - 2023-03-30
 ### Updated
 - [Orders] Order channel callback
 
 ## [1.5.3] - 2023-03-29
 ### Added
 - [Services] Add GPT requirements
```

### Comparing `OctoBot-Services-1.5.4/LICENSE` & `OctoBot-Services-1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/OctoBot_Services.egg-info/PKG-INFO` & `OctoBot-Services-1.5.5/OctoBot_Services.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OctoBot-Services
-Version: 1.5.4
+Version: 1.5.5
 Summary: OctoBot project services package
 Home-page: https://github.com/Drakkar-Software/OctoBot-Services
 Author: Drakkar-Software
 Author-email: drakkar-software@protonmail.com
 License: LGPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
@@ -12,13 +12,13 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
 License-File: LICENSE
 
-# OctoBot-Services [1.5.4](https://github.com/Drakkar-Software/OctoBot-Services/tree/master/docs/CHANGELOG.md)
+# OctoBot-Services [1.5.5](https://github.com/Drakkar-Software/OctoBot-Services/tree/master/docs/CHANGELOG.md)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/31a1caa6e5384d80bf890dba5c9b5e4b)](https://app.codacy.com/gh/Drakkar-Software/OctoBot-Services?utm_source=github.com&utm_medium=referral&utm_content=Drakkar-Software/OctoBot-Services&utm_campaign=Badge_Grade_Dashboard)
 [![PyPI](https://img.shields.io/pypi/v/OctoBot-Services.svg)](https://pypi.python.org/pypi/OctoBot-Services/)
 [![Github-Action-CI](https://github.com/Drakkar-Software/OctoBot-Services/workflows/OctoBot-Services-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot-Services/actions)
 
 OctoBot services package.
```

### Comparing `OctoBot-Services-1.5.4/OctoBot_Services.egg-info/SOURCES.txt` & `OctoBot-Services-1.5.5/OctoBot_Services.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/PKG-INFO` & `OctoBot-Services-1.5.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OctoBot-Services
-Version: 1.5.4
+Version: 1.5.5
 Summary: OctoBot project services package
 Home-page: https://github.com/Drakkar-Software/OctoBot-Services
 Author: Drakkar-Software
 Author-email: drakkar-software@protonmail.com
 License: LGPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
@@ -12,13 +12,13 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
 License-File: LICENSE
 
-# OctoBot-Services [1.5.4](https://github.com/Drakkar-Software/OctoBot-Services/tree/master/docs/CHANGELOG.md)
+# OctoBot-Services [1.5.5](https://github.com/Drakkar-Software/OctoBot-Services/tree/master/docs/CHANGELOG.md)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/31a1caa6e5384d80bf890dba5c9b5e4b)](https://app.codacy.com/gh/Drakkar-Software/OctoBot-Services?utm_source=github.com&utm_medium=referral&utm_content=Drakkar-Software/OctoBot-Services&utm_campaign=Badge_Grade_Dashboard)
 [![PyPI](https://img.shields.io/pypi/v/OctoBot-Services.svg)](https://pypi.python.org/pypi/OctoBot-Services/)
 [![Github-Action-CI](https://github.com/Drakkar-Software/OctoBot-Services/workflows/OctoBot-Services-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot-Services/actions)
 
 OctoBot services package.
```

### Comparing `OctoBot-Services-1.5.4/README.md` & `OctoBot-Services-1.5.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,6 +1,6 @@
-# OctoBot-Services [1.5.4](https://github.com/Drakkar-Software/OctoBot-Services/tree/master/docs/CHANGELOG.md)
+# OctoBot-Services [1.5.5](https://github.com/Drakkar-Software/OctoBot-Services/tree/master/docs/CHANGELOG.md)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/31a1caa6e5384d80bf890dba5c9b5e4b)](https://app.codacy.com/gh/Drakkar-Software/OctoBot-Services?utm_source=github.com&utm_medium=referral&utm_content=Drakkar-Software/OctoBot-Services&utm_campaign=Badge_Grade_Dashboard)
 [![PyPI](https://img.shields.io/pypi/v/OctoBot-Services.svg)](https://pypi.python.org/pypi/OctoBot-Services/)
 [![Github-Action-CI](https://github.com/Drakkar-Software/OctoBot-Services/workflows/OctoBot-Services-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot-Services/actions)
 
 OctoBot services package.
```

### Comparing `OctoBot-Services-1.5.4/octobot_services/__init__.pxd` & `OctoBot-Services-1.5.5/octobot_services/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/octobot_services/__init__.py` & `OctoBot-Services-1.5.5/octobot_services/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 
 PROJECT_NAME = "OctoBot-Services"
-VERSION = "1.5.4"  # major.minor.revision
+VERSION = "1.5.5"  # major.minor.revision
```

### Comparing `OctoBot-Services-1.5.4/octobot_services/abstract_service_user.py` & `OctoBot-Services-1.5.5/octobot_services/abstract_service_user.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/octobot_services/api/__init__.py` & `OctoBot-Services-1.5.5/octobot_services/api/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/octobot_services/api/interfaces.py` & `OctoBot-Services-1.5.5/octobot_services/api/interfaces.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/octobot_services/api/notification.py` & `OctoBot-Services-1.5.5/octobot_services/api/notification.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/octobot_services/api/service_feeds.py` & `OctoBot-Services-1.5.5/octobot_services/api/service_feeds.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/octobot_services/api/services.py` & `OctoBot-Services-1.5.5/octobot_services/api/services.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/octobot_services/channel/__init__.py` & `OctoBot-Services-1.5.5/octobot_services/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/octobot_services/channel/abstract_service_feed.py` & `OctoBot-Services-1.5.5/octobot_services/channel/abstract_service_feed.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/octobot_services/channel/notifications.py` & `OctoBot-Services-1.5.5/octobot_services/channel/notifications.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/octobot_services/channel/user_commands.py` & `OctoBot-Services-1.5.5/octobot_services/channel/user_commands.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/octobot_services/constants.py` & `OctoBot-Services-1.5.5/octobot_services/constants.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/octobot_services/enums.py` & `OctoBot-Services-1.5.5/octobot_services/enums.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/octobot_services/errors.py` & `OctoBot-Services-1.5.5/octobot_services/errors.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/octobot_services/interfaces/__init__.py` & `OctoBot-Services-1.5.5/octobot_services/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/octobot_services/interfaces/abstract_interface.py` & `OctoBot-Services-1.5.5/octobot_services/interfaces/abstract_interface.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/octobot_services/interfaces/bots/__init__.py` & `OctoBot-Services-1.5.5/octobot_services/interfaces/bots/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/octobot_services/interfaces/bots/abstract_bot_interface.py` & `OctoBot-Services-1.5.5/octobot_services/interfaces/bots/abstract_bot_interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 import abc
-from octobot_commons import number_util
 
 import octobot_commons.constants as common_constants
 import octobot_commons.pretty_printer as pretty_printer
 import octobot_commons.timestamp_util as timestamp_util
+import octobot_commons.dict_util as dict_util
 
 import octobot_trading.api as trading_api
 import octobot_trading.constants as trading_constants
 
 import octobot_services.interfaces as interfaces
 import octobot_services.constants as constants
 import octobot_commons.constants as commons_constants
@@ -339,15 +339,22 @@
 
     @staticmethod
     def set_command_portfolios_refresh():
         return interfaces.trigger_portfolios_refresh()
 
     @staticmethod
     def set_command_risk(new_risk):
-        return interfaces.set_risk(new_risk)
+        updated_risk = interfaces.set_risk(new_risk)
+        risk_config = {
+            commons_constants.CONFIG_TRADING: {
+                commons_constants.CONFIG_RISK: float(updated_risk)
+            }
+        }
+        AbstractBotInterface._update_edited_config(risk_config)
+        return updated_risk
 
     @staticmethod
     def set_command_stop():
         interfaces.get_bot_api().stop_bot()
 
     def set_command_pause(self):
         interfaces.cancel_all_open_orders()
@@ -379,7 +386,13 @@
                 remaining = message[end_index + 1:]
                 return messages_list + AbstractBotInterface._split_messages_if_too_long(remaining, max_length,
                                                                                         preferred_separator)
             else:
                 return messages_list
         else:
             return [message]
+
+    @staticmethod
+    def _update_edited_config(partial_config_update):
+        config = interfaces.get_edited_config(dict_only=False)
+        dict_util.nested_update_dict(config.config, partial_config_update)
+        config.save()
```

### Comparing `OctoBot-Services-1.5.4/octobot_services/interfaces/interface_factory.py` & `OctoBot-Services-1.5.5/octobot_services/interfaces/interface_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/octobot_services/interfaces/util/__init__.py` & `OctoBot-Services-1.5.5/octobot_services/interfaces/util/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/octobot_services/interfaces/util/bot.py` & `OctoBot-Services-1.5.5/octobot_services/interfaces/util/bot.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/octobot_services/interfaces/util/order.py` & `OctoBot-Services-1.5.5/octobot_services/interfaces/util/order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/octobot_services/interfaces/util/portfolio.py` & `OctoBot-Services-1.5.5/octobot_services/interfaces/util/portfolio.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/octobot_services/interfaces/util/position.py` & `OctoBot-Services-1.5.5/octobot_services/interfaces/util/position.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/octobot_services/interfaces/util/profitability.py` & `OctoBot-Services-1.5.5/octobot_services/interfaces/util/profitability.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/octobot_services/interfaces/util/trader.py` & `OctoBot-Services-1.5.5/octobot_services/interfaces/util/trader.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/octobot_services/interfaces/util/util.py` & `OctoBot-Services-1.5.5/octobot_services/interfaces/util/util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/octobot_services/interfaces/web/__init__.py` & `OctoBot-Services-1.5.5/octobot_services/interfaces/web/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/octobot_services/interfaces/web/abstract_web_interface.py` & `OctoBot-Services-1.5.5/octobot_services/interfaces/web/abstract_web_interface.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/octobot_services/managers/__init__.py` & `OctoBot-Services-1.5.5/octobot_services/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/octobot_services/managers/interface_manager.py` & `OctoBot-Services-1.5.5/octobot_services/managers/interface_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/octobot_services/managers/service_feed_manager.py` & `OctoBot-Services-1.5.5/octobot_services/managers/service_feed_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/octobot_services/managers/service_manager.py` & `OctoBot-Services-1.5.5/octobot_services/managers/service_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/octobot_services/notification/__init__.py` & `OctoBot-Services-1.5.5/octobot_services/notification/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/octobot_services/notification/formated_notifications.py` & `OctoBot-Services-1.5.5/octobot_services/notification/formated_notifications.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/octobot_services/notification/notification.py` & `OctoBot-Services-1.5.5/octobot_services/notification/notification.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/octobot_services/notifier/__init__.py` & `OctoBot-Services-1.5.5/octobot_services/notifier/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/octobot_services/notifier/abstract_notifier.py` & `OctoBot-Services-1.5.5/octobot_services/notifier/abstract_notifier.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/octobot_services/notifier/notifier_factory.py` & `OctoBot-Services-1.5.5/octobot_services/notifier/notifier_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/octobot_services/octobot_channel_consumer.py` & `OctoBot-Services-1.5.5/octobot_services/octobot_channel_consumer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/octobot_services/service_feeds/__init__.py` & `OctoBot-Services-1.5.5/octobot_services/service_feeds/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/octobot_services/service_feeds/abstract_service_feed.py` & `OctoBot-Services-1.5.5/octobot_services/service_feeds/abstract_service_feed.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/octobot_services/service_feeds/service_feed_exception.py` & `OctoBot-Services-1.5.5/octobot_services/service_feeds/service_feed_exception.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/octobot_services/service_feeds/service_feed_factory.py` & `OctoBot-Services-1.5.5/octobot_services/service_feeds/service_feed_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/octobot_services/service_feeds/service_feeds.py` & `OctoBot-Services-1.5.5/octobot_services/service_feeds/service_feeds.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/octobot_services/services/__init__.py` & `OctoBot-Services-1.5.5/octobot_services/services/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/octobot_services/services/abstract_service.py` & `OctoBot-Services-1.5.5/octobot_services/services/abstract_service.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/octobot_services/services/service_factory.py` & `OctoBot-Services-1.5.5/octobot_services/services/service_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/octobot_services/util/__init__.py` & `OctoBot-Services-1.5.5/octobot_services/util/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/octobot_services/util/exchange_watcher.py` & `OctoBot-Services-1.5.5/octobot_services/util/exchange_watcher.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/octobot_services/util/initializable_with_post_actions.py` & `OctoBot-Services-1.5.5/octobot_services/util/initializable_with_post_actions.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/octobot_services/util/returning_startable.py` & `OctoBot-Services-1.5.5/octobot_services/util/returning_startable.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/requirements.txt` & `OctoBot-Services-1.5.5/requirements.txt`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/setup.py` & `OctoBot-Services-1.5.5/setup.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/tests/test_imports.py` & `OctoBot-Services-1.5.5/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/tests/test_interface_api.py` & `OctoBot-Services-1.5.5/tests/test_interface_api.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/tests/test_notification_api.py` & `OctoBot-Services-1.5.5/tests/test_notification_api.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Services-1.5.4/tests/test_service_api.py` & `OctoBot-Services-1.5.5/tests/test_service_api.py`

 * *Files identical despite different names*

