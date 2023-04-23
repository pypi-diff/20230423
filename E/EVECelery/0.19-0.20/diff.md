# Comparing `tmp/EVECelery-0.19.tar.gz` & `tmp/EVECelery-0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EVECelery-0.19.tar", last modified: Wed Mar 15 05:26:21 2023, max compression
+gzip compressed data, was "EVECelery-0.20.tar", last modified: Sun Apr 23 09:32:01 2023, max compression
```

## Comparing `EVECelery-0.19.tar` & `EVECelery-0.20.tar`

### file list

```diff
@@ -1,65 +1,602 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 05:26:21.743521 EVECelery-0.19/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 05:26:21.735521 EVECelery-0.19/EVECelery/
--rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-03-15 05:26:11.000000 EVECelery-0.19/EVECelery/CeleryApps.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-03-15 05:26:11.000000 EVECelery-0.19/EVECelery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-15 05:26:11.000000 EVECelery-0.19/EVECelery/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-03-15 05:26:11.000000 EVECelery-0.19/EVECelery/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-15 05:26:11.000000 EVECelery-0.19/EVECelery/celeryconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 05:26:21.739521 EVECelery-0.19/EVECelery/clients/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-03-15 05:26:11.000000 EVECelery-0.19/EVECelery/clients/BaseClient.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-03-15 05:26:11.000000 EVECelery-0.19/EVECelery/clients/ClientRabbitMQ.py
--rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-03-15 05:26:11.000000 EVECelery-0.19/EVECelery/clients/ClientRedis.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 05:26:11.000000 EVECelery-0.19/EVECelery/clients/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 05:26:21.739521 EVECelery-0.19/EVECelery/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 05:26:11.000000 EVECelery-0.19/EVECelery/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-15 05:26:11.000000 EVECelery-0.19/EVECelery/exceptions/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-15 05:26:11.000000 EVECelery-0.19/EVECelery/exceptions/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 05:26:21.739521 EVECelery-0.19/EVECelery/tasks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 05:26:21.739521 EVECelery-0.19/EVECelery/tasks/Alliance/
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-03-15 05:26:11.000000 EVECelery-0.19/EVECelery/tasks/Alliance/AllianceInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-15 05:26:11.000000 EVECelery-0.19/EVECelery/tasks/Alliance/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 05:26:21.739521 EVECelery-0.19/EVECelery/tasks/BaseTasks/
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-03-15 05:26:11.000000 EVECelery-0.19/EVECelery/tasks/BaseTasks/BaseTask.py
--rw-r--r--   0 runner    (1001) docker     (123)     9730 2023-03-15 05:26:11.000000 EVECelery-0.19/EVECelery/tasks/BaseTasks/ESIResqust.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 05:26:11.000000 EVECelery-0.19/EVECelery/tasks/BaseTasks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 05:26:21.739521 EVECelery-0.19/EVECelery/tasks/Character/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-03-15 05:26:11.000000 EVECelery-0.19/EVECelery/tasks/Character/CharacterPublicInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-15 05:26:11.000000 EVECelery-0.19/EVECelery/tasks/Character/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 05:26:21.739521 EVECelery-0.19/EVECelery/tasks/Corporation/
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-03-15 05:26:11.000000 EVECelery-0.19/EVECelery/tasks/Corporation/CorporationInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-15 05:26:11.000000 EVECelery-0.19/EVECelery/tasks/Corporation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 05:26:21.739521 EVECelery-0.19/EVECelery/tasks/Market/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-03-15 05:26:11.000000 EVECelery-0.19/EVECelery/tasks/Market/PricesList.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-15 05:26:11.000000 EVECelery-0.19/EVECelery/tasks/Market/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 05:26:21.739521 EVECelery-0.19/EVECelery/tasks/Routes/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-03-15 05:26:11.000000 EVECelery-0.19/EVECelery/tasks/Routes/Route.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-15 05:26:11.000000 EVECelery-0.19/EVECelery/tasks/Routes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 05:26:21.739521 EVECelery-0.19/EVECelery/tasks/Universe/
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-03-15 05:26:11.000000 EVECelery-0.19/EVECelery/tasks/Universe/CategoryInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-03-15 05:26:11.000000 EVECelery-0.19/EVECelery/tasks/Universe/ConstellationInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-03-15 05:26:11.000000 EVECelery-0.19/EVECelery/tasks/Universe/FactionsList.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-03-15 05:26:11.000000 EVECelery-0.19/EVECelery/tasks/Universe/GroupInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-03-15 05:26:11.000000 EVECelery-0.19/EVECelery/tasks/Universe/RegionInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-03-15 05:26:11.000000 EVECelery-0.19/EVECelery/tasks/Universe/SystemInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-03-15 05:26:11.000000 EVECelery-0.19/EVECelery/tasks/Universe/TypeInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-03-15 05:26:11.000000 EVECelery-0.19/EVECelery/tasks/Universe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 05:26:11.000000 EVECelery-0.19/EVECelery/tasks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 05:26:21.739521 EVECelery-0.19/EVECelery/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-03-15 05:26:11.000000 EVECelery-0.19/EVECelery/utils/ErrorLimiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-03-15 05:26:11.000000 EVECelery-0.19/EVECelery/utils/RequestHeaders.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 05:26:11.000000 EVECelery-0.19/EVECelery/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 05:26:21.739521 EVECelery-0.19/EVECelery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-03-15 05:26:21.000000 EVECelery-0.19/EVECelery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-03-15 05:26:21.000000 EVECelery-0.19/EVECelery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 05:26:21.000000 EVECelery-0.19/EVECelery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-15 05:26:21.000000 EVECelery-0.19/EVECelery.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-15 05:26:21.000000 EVECelery-0.19/EVECelery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-15 05:26:21.000000 EVECelery-0.19/EVECelery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-15 05:26:11.000000 EVECelery-0.19/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-03-15 05:26:21.739521 EVECelery-0.19/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-03-15 05:26:11.000000 EVECelery-0.19/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-15 05:26:11.000000 EVECelery-0.19/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-15 05:26:21.743521 EVECelery-0.19/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-03-15 05:26:11.000000 EVECelery-0.19/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 05:26:21.739521 EVECelery-0.19/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-03-15 05:26:11.000000 EVECelery-0.19/tests/test_CeleryApps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.355816 EVECelery-0.20/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.291816 EVECelery-0.20/EVECelery/
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/EVECeleryBeatScheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/EVECeleryWorker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.295816 EVECelery-0.20/EVECelery/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/clients/BaseClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/clients/ClientRabbitMQ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/clients/ClientRedis.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/clients/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.295816 EVECelery-0.20/EVECelery/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/exceptions/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/exceptions/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.295816 EVECelery-0.20/EVECelery/tasks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.295816 EVECelery-0.20/EVECelery/tasks/BaseTasks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.295816 EVECelery-0.20/EVECelery/tasks/BaseTasks/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/BaseTasks/Models/ModelsBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/BaseTasks/Models/ModelsCached.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/BaseTasks/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/BaseTasks/TaskBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/BaseTasks/TaskCached.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/BaseTasks/TaskESI.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/BaseTasks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.295816 EVECelery-0.20/EVECelery/tasks/ESI/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.295816 EVECelery-0.20/EVECelery/tasks/ESI/Alliance/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.295816 EVECelery-0.20/EVECelery/tasks/ESI/Alliance/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Alliance/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Alliance/Models/get_alliances_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Alliance/Models/get_alliances_alliance_id_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Alliance/Models/get_alliances_alliance_id_corporations_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Alliance/Models/get_alliances_alliance_id_icons_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Alliance/TaskDirectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Alliance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Alliance/get_alliances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Alliance/get_alliances_alliance_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Alliance/get_alliances_alliance_id_corporations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Alliance/get_alliances_alliance_id_icons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.299816 EVECelery-0.20/EVECelery/tasks/ESI/Assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.299816 EVECelery-0.20/EVECelery/tasks/ESI/Assets/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Assets/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Assets/Models/get_characters_character_id_assets_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Assets/Models/get_corporations_corporation_id_assets_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Assets/Models/post_characters_character_id_assets_locations_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Assets/Models/post_characters_character_id_assets_names_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Assets/Models/post_corporations_corporation_id_assets_locations_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Assets/Models/post_corporations_corporation_id_assets_names_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Assets/TaskDirectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Assets/get_characters_character_id_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Assets/get_corporations_corporation_id_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Assets/post_characters_character_id_assets_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Assets/post_characters_character_id_assets_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Assets/post_corporations_corporation_id_assets_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Assets/post_corporations_corporation_id_assets_names.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.299816 EVECelery-0.20/EVECelery/tasks/ESI/Bookmarks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.299816 EVECelery-0.20/EVECelery/tasks/ESI/Bookmarks/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Bookmarks/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5137 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Bookmarks/Models/get_characters_character_id_bookmarks_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Bookmarks/Models/get_characters_character_id_bookmarks_folders_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Bookmarks/Models/get_corporations_corporation_id_bookmarks_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Bookmarks/Models/get_corporations_corporation_id_bookmarks_folders_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Bookmarks/TaskDirectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Bookmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Bookmarks/get_characters_character_id_bookmarks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Bookmarks/get_characters_character_id_bookmarks_folders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Bookmarks/get_corporations_corporation_id_bookmarks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Bookmarks/get_corporations_corporation_id_bookmarks_folders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.299816 EVECelery-0.20/EVECelery/tasks/ESI/Calendar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.303816 EVECelery-0.20/EVECelery/tasks/ESI/Calendar/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Calendar/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Calendar/Models/get_characters_character_id_calendar_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Calendar/Models/get_characters_character_id_calendar_event_id_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Calendar/Models/get_characters_character_id_calendar_event_id_attendees_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Calendar/TaskDirectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Calendar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6613 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Calendar/get_characters_character_id_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Calendar/get_characters_character_id_calendar_event_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Calendar/get_characters_character_id_calendar_event_id_attendees.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.303816 EVECelery-0.20/EVECelery/tasks/ESI/Character/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.303816 EVECelery-0.20/EVECelery/tasks/ESI/Character/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Character/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Character/Models/get_characters_character_id_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Character/Models/get_characters_character_id_agents_research_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Character/Models/get_characters_character_id_blueprints_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Character/Models/get_characters_character_id_corporationhistory_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Character/Models/get_characters_character_id_fatigue_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Character/Models/get_characters_character_id_medals_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10497 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Character/Models/get_characters_character_id_notifications_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Character/Models/get_characters_character_id_notifications_contacts_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Character/Models/get_characters_character_id_portrait_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9479 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Character/Models/get_characters_character_id_roles_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Character/Models/get_characters_character_id_standings_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Character/Models/get_characters_character_id_titles_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Character/Models/post_characters_affiliation_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Character/Models/post_characters_character_id_cspa_201.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12596 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Character/TaskDirectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Character/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Character/get_characters_character_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Character/get_characters_character_id_agents_research.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Character/get_characters_character_id_blueprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Character/get_characters_character_id_corporationhistory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Character/get_characters_character_id_fatigue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Character/get_characters_character_id_medals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Character/get_characters_character_id_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Character/get_characters_character_id_notifications_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Character/get_characters_character_id_portrait.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Character/get_characters_character_id_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Character/get_characters_character_id_standings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Character/get_characters_character_id_titles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Character/post_characters_affiliation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Character/post_characters_character_id_cspa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.307816 EVECelery-0.20/EVECelery/tasks/ESI/Clones/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.307816 EVECelery-0.20/EVECelery/tasks/ESI/Clones/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Clones/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Clones/Models/get_characters_character_id_clones_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Clones/Models/get_characters_character_id_implants_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Clones/TaskDirectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Clones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Clones/get_characters_character_id_clones.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Clones/get_characters_character_id_implants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.307816 EVECelery-0.20/EVECelery/tasks/ESI/Contacts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.307816 EVECelery-0.20/EVECelery/tasks/ESI/Contacts/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Contacts/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Contacts/Models/delete_characters_character_id_contacts_204.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Contacts/Models/get_alliances_alliance_id_contacts_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Contacts/Models/get_alliances_alliance_id_contacts_labels_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Contacts/Models/get_characters_character_id_contacts_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Contacts/Models/get_characters_character_id_contacts_labels_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Contacts/Models/get_corporations_corporation_id_contacts_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Contacts/Models/get_corporations_corporation_id_contacts_labels_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Contacts/Models/post_characters_character_id_contacts_201.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Contacts/Models/put_characters_character_id_contacts_204.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8554 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Contacts/TaskDirectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Contacts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Contacts/delete_characters_character_id_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Contacts/get_alliances_alliance_id_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Contacts/get_alliances_alliance_id_contacts_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Contacts/get_characters_character_id_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Contacts/get_characters_character_id_contacts_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5860 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Contacts/get_corporations_corporation_id_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Contacts/get_corporations_corporation_id_contacts_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Contacts/post_characters_character_id_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Contacts/put_characters_character_id_contacts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.311816 EVECelery-0.20/EVECelery/tasks/ESI/Contracts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.311816 EVECelery-0.20/EVECelery/tasks/ESI/Contracts/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Contracts/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Contracts/Models/get_characters_character_id_contracts_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Contracts/Models/get_characters_character_id_contracts_contract_id_bids_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Contracts/Models/get_characters_character_id_contracts_contract_id_items_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Contracts/Models/get_contracts_public_bids_contract_id_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Contracts/Models/get_contracts_public_bids_contract_id_204.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Contracts/Models/get_contracts_public_items_contract_id_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Contracts/Models/get_contracts_public_items_contract_id_204.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5447 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Contracts/Models/get_contracts_public_region_id_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Contracts/Models/get_corporations_corporation_id_contracts_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Contracts/Models/get_corporations_corporation_id_contracts_contract_id_bids_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Contracts/Models/get_corporations_corporation_id_contracts_contract_id_items_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9236 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Contracts/TaskDirectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Contracts/get_characters_character_id_contracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Contracts/get_characters_character_id_contracts_contract_id_bids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Contracts/get_characters_character_id_contracts_contract_id_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Contracts/get_contracts_public_bids_contract_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5948 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Contracts/get_contracts_public_items_contract_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Contracts/get_contracts_public_region_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Contracts/get_corporations_corporation_id_contracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Contracts/get_corporations_corporation_id_contracts_contract_id_bids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Contracts/get_corporations_corporation_id_contracts_contract_id_items.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.315816 EVECelery-0.20/EVECelery/tasks/ESI/Corporation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.319816 EVECelery-0.20/EVECelery/tasks/ESI/Corporation/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Corporation/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Corporation/Models/get_corporations_corporation_id_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Corporation/Models/get_corporations_corporation_id_alliancehistory_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Corporation/Models/get_corporations_corporation_id_blueprints_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Corporation/Models/get_corporations_corporation_id_containers_logs_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Corporation/Models/get_corporations_corporation_id_divisions_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Corporation/Models/get_corporations_corporation_id_facilities_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Corporation/Models/get_corporations_corporation_id_icons_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Corporation/Models/get_corporations_corporation_id_medals_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Corporation/Models/get_corporations_corporation_id_medals_issued_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Corporation/Models/get_corporations_corporation_id_members_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Corporation/Models/get_corporations_corporation_id_members_limit_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Corporation/Models/get_corporations_corporation_id_members_titles_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Corporation/Models/get_corporations_corporation_id_membertracking_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17831 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Corporation/Models/get_corporations_corporation_id_roles_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6782 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Corporation/Models/get_corporations_corporation_id_roles_history_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Corporation/Models/get_corporations_corporation_id_shareholders_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Corporation/Models/get_corporations_corporation_id_standings_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Corporation/Models/get_corporations_corporation_id_starbases_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Corporation/Models/get_corporations_corporation_id_starbases_starbase_id_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6713 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Corporation/Models/get_corporations_corporation_id_structures_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18001 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Corporation/Models/get_corporations_corporation_id_titles_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Corporation/Models/get_corporations_npccorps_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21013 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Corporation/TaskDirectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Corporation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Corporation/get_corporations_corporation_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Corporation/get_corporations_corporation_id_alliancehistory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6097 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Corporation/get_corporations_corporation_id_blueprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Corporation/get_corporations_corporation_id_containers_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Corporation/get_corporations_corporation_id_divisions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5844 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Corporation/get_corporations_corporation_id_facilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5322 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Corporation/get_corporations_corporation_id_icons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Corporation/get_corporations_corporation_id_medals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Corporation/get_corporations_corporation_id_medals_issued.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Corporation/get_corporations_corporation_id_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Corporation/get_corporations_corporation_id_members_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5907 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Corporation/get_corporations_corporation_id_members_titles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Corporation/get_corporations_corporation_id_membertracking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Corporation/get_corporations_corporation_id_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Corporation/get_corporations_corporation_id_roles_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Corporation/get_corporations_corporation_id_shareholders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Corporation/get_corporations_corporation_id_standings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Corporation/get_corporations_corporation_id_starbases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Corporation/get_corporations_corporation_id_starbases_starbase_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Corporation/get_corporations_corporation_id_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Corporation/get_corporations_corporation_id_titles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Corporation/get_corporations_npccorps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.319816 EVECelery-0.20/EVECelery/tasks/ESI/Dogma/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.319816 EVECelery-0.20/EVECelery/tasks/ESI/Dogma/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Dogma/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Dogma/Models/get_dogma_attributes_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Dogma/Models/get_dogma_attributes_attribute_id_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Dogma/Models/get_dogma_dynamic_items_type_id_item_id_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Dogma/Models/get_dogma_effects_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Dogma/Models/get_dogma_effects_effect_id_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Dogma/TaskDirectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Dogma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Dogma/get_dogma_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Dogma/get_dogma_attributes_attribute_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Dogma/get_dogma_dynamic_items_type_id_item_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Dogma/get_dogma_effects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Dogma/get_dogma_effects_effect_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.319816 EVECelery-0.20/EVECelery/tasks/ESI/FactionWarfare/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.323816 EVECelery-0.20/EVECelery/tasks/ESI/FactionWarfare/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/FactionWarfare/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/FactionWarfare/Models/get_characters_character_id_fw_stats_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/FactionWarfare/Models/get_corporations_corporation_id_fw_stats_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/FactionWarfare/Models/get_fw_leaderboards_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/FactionWarfare/Models/get_fw_leaderboards_characters_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7830 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/FactionWarfare/Models/get_fw_leaderboards_corporations_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/FactionWarfare/Models/get_fw_stats_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/FactionWarfare/Models/get_fw_systems_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/FactionWarfare/Models/get_fw_wars_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6620 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/FactionWarfare/TaskDirectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/FactionWarfare/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/FactionWarfare/get_characters_character_id_fw_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/FactionWarfare/get_corporations_corporation_id_fw_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/FactionWarfare/get_fw_leaderboards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/FactionWarfare/get_fw_leaderboards_characters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/FactionWarfare/get_fw_leaderboards_corporations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/FactionWarfare/get_fw_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/FactionWarfare/get_fw_systems.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4897 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/FactionWarfare/get_fw_wars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.323816 EVECelery-0.20/EVECelery/tasks/ESI/Fittings/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.323816 EVECelery-0.20/EVECelery/tasks/ESI/Fittings/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Fittings/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Fittings/Models/delete_characters_character_id_fittings_fitting_id_204.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Fittings/Models/get_characters_character_id_fittings_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Fittings/TaskDirectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Fittings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6082 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Fittings/delete_characters_character_id_fittings_fitting_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Fittings/get_characters_character_id_fittings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.323816 EVECelery-0.20/EVECelery/tasks/ESI/Fleets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.323816 EVECelery-0.20/EVECelery/tasks/ESI/Fleets/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Fleets/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Fleets/Models/delete_fleets_fleet_id_members_member_id_204.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Fleets/Models/delete_fleets_fleet_id_squads_squad_id_204.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Fleets/Models/delete_fleets_fleet_id_wings_wing_id_204.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Fleets/Models/get_characters_character_id_fleet_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Fleets/Models/get_fleets_fleet_id_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Fleets/Models/get_fleets_fleet_id_members_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Fleets/Models/get_fleets_fleet_id_wings_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Fleets/Models/post_fleets_fleet_id_wings_201.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Fleets/Models/post_fleets_fleet_id_wings_wing_id_squads_201.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Fleets/TaskDirectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Fleets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Fleets/delete_fleets_fleet_id_members_member_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5860 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Fleets/delete_fleets_fleet_id_squads_squad_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Fleets/delete_fleets_fleet_id_wings_wing_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Fleets/get_characters_character_id_fleet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Fleets/get_fleets_fleet_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Fleets/get_fleets_fleet_id_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Fleets/get_fleets_fleet_id_wings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Fleets/post_fleets_fleet_id_wings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Fleets/post_fleets_fleet_id_wings_wing_id_squads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.327816 EVECelery-0.20/EVECelery/tasks/ESI/Incursions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.327816 EVECelery-0.20/EVECelery/tasks/ESI/Incursions/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Incursions/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Incursions/Models/get_incursions_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Incursions/TaskDirectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Incursions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Incursions/get_incursions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.327816 EVECelery-0.20/EVECelery/tasks/ESI/Industry/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.327816 EVECelery-0.20/EVECelery/tasks/ESI/Industry/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Industry/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Industry/Models/get_characters_character_id_industry_jobs_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Industry/Models/get_characters_character_id_mining_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Industry/Models/get_corporation_corporation_id_mining_extractions_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Industry/Models/get_corporation_corporation_id_mining_observers_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Industry/Models/get_corporation_corporation_id_mining_observers_observer_id_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Industry/Models/get_corporations_corporation_id_industry_jobs_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Industry/Models/get_industry_facilities_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Industry/Models/get_industry_systems_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Industry/TaskDirectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Industry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Industry/get_characters_character_id_industry_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Industry/get_characters_character_id_mining.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Industry/get_corporation_corporation_id_mining_extractions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Industry/get_corporation_corporation_id_mining_observers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Industry/get_corporation_corporation_id_mining_observers_observer_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Industry/get_corporations_corporation_id_industry_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Industry/get_industry_facilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Industry/get_industry_systems.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.327816 EVECelery-0.20/EVECelery/tasks/ESI/Insurance/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.327816 EVECelery-0.20/EVECelery/tasks/ESI/Insurance/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Insurance/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Insurance/Models/get_insurance_prices_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Insurance/TaskDirectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Insurance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Insurance/get_insurance_prices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.327816 EVECelery-0.20/EVECelery/tasks/ESI/Killmails/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.331816 EVECelery-0.20/EVECelery/tasks/ESI/Killmails/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Killmails/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Killmails/Models/get_characters_character_id_killmails_recent_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Killmails/Models/get_corporations_corporation_id_killmails_recent_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9678 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Killmails/Models/get_killmails_killmail_id_killmail_hash_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Killmails/TaskDirectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Killmails/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Killmails/get_characters_character_id_killmails_recent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Killmails/get_corporations_corporation_id_killmails_recent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Killmails/get_killmails_killmail_id_killmail_hash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.331816 EVECelery-0.20/EVECelery/tasks/ESI/Location/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.331816 EVECelery-0.20/EVECelery/tasks/ESI/Location/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Location/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Location/Models/get_characters_character_id_location_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Location/Models/get_characters_character_id_online_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Location/Models/get_characters_character_id_ship_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Location/TaskDirectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Location/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Location/get_characters_character_id_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Location/get_characters_character_id_online.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Location/get_characters_character_id_ship.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.331816 EVECelery-0.20/EVECelery/tasks/ESI/Loyalty/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.331816 EVECelery-0.20/EVECelery/tasks/ESI/Loyalty/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Loyalty/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Loyalty/Models/get_characters_character_id_loyalty_points_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Loyalty/Models/get_loyalty_stores_corporation_id_offers_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Loyalty/TaskDirectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Loyalty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5860 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Loyalty/get_characters_character_id_loyalty_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Loyalty/get_loyalty_stores_corporation_id_offers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.331816 EVECelery-0.20/EVECelery/tasks/ESI/Mail/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.335816 EVECelery-0.20/EVECelery/tasks/ESI/Mail/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Mail/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Mail/Models/delete_characters_character_id_mail_labels_label_id_204.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Mail/Models/delete_characters_character_id_mail_mail_id_204.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Mail/Models/get_characters_character_id_mail_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Mail/Models/get_characters_character_id_mail_labels_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Mail/Models/get_characters_character_id_mail_lists_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Mail/Models/get_characters_character_id_mail_mail_id_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Mail/TaskDirectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Mail/delete_characters_character_id_mail_labels_label_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Mail/delete_characters_character_id_mail_mail_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6608 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Mail/get_characters_character_id_mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Mail/get_characters_character_id_mail_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Mail/get_characters_character_id_mail_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Mail/get_characters_character_id_mail_mail_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.335816 EVECelery-0.20/EVECelery/tasks/ESI/Market/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.335816 EVECelery-0.20/EVECelery/tasks/ESI/Market/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Market/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Market/Models/get_characters_character_id_orders_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Market/Models/get_characters_character_id_orders_history_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Market/Models/get_corporations_corporation_id_orders_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Market/Models/get_corporations_corporation_id_orders_history_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Market/Models/get_markets_groups_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Market/Models/get_markets_groups_market_group_id_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Market/Models/get_markets_prices_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Market/Models/get_markets_region_id_history_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Market/Models/get_markets_region_id_orders_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Market/Models/get_markets_region_id_types_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Market/Models/get_markets_structures_structure_id_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9357 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Market/TaskDirectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Market/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Market/get_characters_character_id_orders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Market/get_characters_character_id_orders_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Market/get_corporations_corporation_id_orders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6310 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Market/get_corporations_corporation_id_orders_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Market/get_markets_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Market/get_markets_groups_market_group_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Market/get_markets_prices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Market/get_markets_region_id_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Market/get_markets_region_id_orders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Market/get_markets_region_id_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Market/get_markets_structures_structure_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.339816 EVECelery-0.20/EVECelery/tasks/ESI/Opportunities/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.339816 EVECelery-0.20/EVECelery/tasks/ESI/Opportunities/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Opportunities/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Opportunities/Models/get_characters_character_id_opportunities_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Opportunities/Models/get_opportunities_groups_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Opportunities/Models/get_opportunities_groups_group_id_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Opportunities/Models/get_opportunities_tasks_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Opportunities/Models/get_opportunities_tasks_task_id_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Opportunities/TaskDirectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Opportunities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Opportunities/get_characters_character_id_opportunities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Opportunities/get_opportunities_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Opportunities/get_opportunities_groups_group_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Opportunities/get_opportunities_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Opportunities/get_opportunities_tasks_task_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.339816 EVECelery-0.20/EVECelery/tasks/ESI/PlanetaryInteraction/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.339816 EVECelery-0.20/EVECelery/tasks/ESI/PlanetaryInteraction/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/PlanetaryInteraction/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/PlanetaryInteraction/Models/get_characters_character_id_planets_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/PlanetaryInteraction/Models/get_characters_character_id_planets_planet_id_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/PlanetaryInteraction/Models/get_corporations_corporation_id_customs_offices_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/PlanetaryInteraction/Models/get_universe_schematics_schematic_id_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/PlanetaryInteraction/TaskDirectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/PlanetaryInteraction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/PlanetaryInteraction/get_characters_character_id_planets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6288 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/PlanetaryInteraction/get_characters_character_id_planets_planet_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/PlanetaryInteraction/get_corporations_corporation_id_customs_offices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/PlanetaryInteraction/get_universe_schematics_schematic_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.339816 EVECelery-0.20/EVECelery/tasks/ESI/Routes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.339816 EVECelery-0.20/EVECelery/tasks/ESI/Routes/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Routes/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Routes/Models/get_route_origin_destination_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Routes/TaskDirectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Routes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Routes/get_route_origin_destination.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.339816 EVECelery-0.20/EVECelery/tasks/ESI/Search/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.339816 EVECelery-0.20/EVECelery/tasks/ESI/Search/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Search/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Search/Models/get_characters_character_id_search_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Search/TaskDirectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Search/get_characters_character_id_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.343816 EVECelery-0.20/EVECelery/tasks/ESI/Skills/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.343816 EVECelery-0.20/EVECelery/tasks/ESI/Skills/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Skills/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Skills/Models/get_characters_character_id_attributes_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Skills/Models/get_characters_character_id_skillqueue_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Skills/Models/get_characters_character_id_skills_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Skills/TaskDirectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Skills/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Skills/get_characters_character_id_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Skills/get_characters_character_id_skillqueue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Skills/get_characters_character_id_skills.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.343816 EVECelery-0.20/EVECelery/tasks/ESI/Sovereignty/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.343816 EVECelery-0.20/EVECelery/tasks/ESI/Sovereignty/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Sovereignty/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Sovereignty/Models/get_sovereignty_campaigns_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Sovereignty/Models/get_sovereignty_map_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Sovereignty/Models/get_sovereignty_structures_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Sovereignty/TaskDirectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Sovereignty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Sovereignty/get_sovereignty_campaigns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Sovereignty/get_sovereignty_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Sovereignty/get_sovereignty_structures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.343816 EVECelery-0.20/EVECelery/tasks/ESI/Status/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.343816 EVECelery-0.20/EVECelery/tasks/ESI/Status/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Status/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Status/Models/get_status_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Status/TaskDirectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Status/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Status/get_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11288 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/TaskDirectory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.347816 EVECelery-0.20/EVECelery/tasks/ESI/Universe/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.351816 EVECelery-0.20/EVECelery/tasks/ESI/Universe/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/Models/get_universe_ancestries_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/Models/get_universe_asteroid_belts_asteroid_belt_id_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/Models/get_universe_bloodlines_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/Models/get_universe_categories_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/Models/get_universe_categories_category_id_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/Models/get_universe_constellations_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/Models/get_universe_constellations_constellation_id_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/Models/get_universe_factions_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/Models/get_universe_graphics_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/Models/get_universe_graphics_graphic_id_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/Models/get_universe_groups_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/Models/get_universe_groups_group_id_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/Models/get_universe_moons_moon_id_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/Models/get_universe_planets_planet_id_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/Models/get_universe_races_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/Models/get_universe_regions_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/Models/get_universe_regions_region_id_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/Models/get_universe_stargates_stargate_id_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/Models/get_universe_stars_star_id_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/Models/get_universe_stations_station_id_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/Models/get_universe_structures_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/Models/get_universe_structures_structure_id_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/Models/get_universe_system_jumps_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/Models/get_universe_system_kills_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/Models/get_universe_systems_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/Models/get_universe_systems_system_id_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/Models/get_universe_types_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/Models/get_universe_types_type_id_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/Models/post_universe_ids_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/Models/post_universe_names_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22509 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/TaskDirectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/get_universe_ancestries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/get_universe_asteroid_belts_asteroid_belt_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/get_universe_bloodlines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/get_universe_categories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/get_universe_categories_category_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/get_universe_constellations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/get_universe_constellations_constellation_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/get_universe_factions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/get_universe_graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/get_universe_graphics_graphic_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/get_universe_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/get_universe_groups_group_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/get_universe_moons_moon_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/get_universe_planets_planet_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/get_universe_races.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/get_universe_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/get_universe_regions_region_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/get_universe_stargates_stargate_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/get_universe_stars_star_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/get_universe_stations_station_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/get_universe_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/get_universe_structures_structure_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/get_universe_system_jumps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5031 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/get_universe_system_kills.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/get_universe_systems.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/get_universe_systems_system_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/get_universe_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/get_universe_types_type_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/post_universe_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Universe/post_universe_names.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.351816 EVECelery-0.20/EVECelery/tasks/ESI/UserInterface/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.351816 EVECelery-0.20/EVECelery/tasks/ESI/UserInterface/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/UserInterface/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/UserInterface/Models/post_ui_autopilot_waypoint_204.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/UserInterface/Models/post_ui_openwindow_contract_204.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/UserInterface/Models/post_ui_openwindow_information_204.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/UserInterface/Models/post_ui_openwindow_marketdetails_204.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/UserInterface/TaskDirectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/UserInterface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6313 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/UserInterface/post_ui_autopilot_waypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/UserInterface/post_ui_openwindow_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/UserInterface/post_ui_openwindow_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/UserInterface/post_ui_openwindow_marketdetails.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.355816 EVECelery-0.20/EVECelery/tasks/ESI/Wallet/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.355816 EVECelery-0.20/EVECelery/tasks/ESI/Wallet/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Wallet/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Wallet/Models/get_characters_character_id_wallet_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10642 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Wallet/Models/get_characters_character_id_wallet_journal_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Wallet/Models/get_characters_character_id_wallet_transactions_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Wallet/Models/get_corporations_corporation_id_wallets_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11326 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Wallet/Models/get_corporations_corporation_id_wallets_division_journal_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Wallet/Models/get_corporations_corporation_id_wallets_division_transactions_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Wallet/TaskDirectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Wallet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5837 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Wallet/get_characters_character_id_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Wallet/get_characters_character_id_wallet_journal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6207 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Wallet/get_characters_character_id_wallet_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Wallet/get_corporations_corporation_id_wallets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Wallet/get_corporations_corporation_id_wallets_division_journal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Wallet/get_corporations_corporation_id_wallets_division_transactions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.355816 EVECelery-0.20/EVECelery/tasks/ESI/Wars/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.355816 EVECelery-0.20/EVECelery/tasks/ESI/Wars/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Wars/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Wars/Models/get_wars_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Wars/Models/get_wars_war_id_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Wars/Models/get_wars_war_id_killmails_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Wars/TaskDirectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Wars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Wars/get_wars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Wars/get_wars_war_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/Wars/get_wars_war_id_killmails.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/ESI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.355816 EVECelery-0.20/EVECelery/tasks/Samples/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/Samples/CachedAddTask.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/Samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/TaskDirectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/tasks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.355816 EVECelery-0.20/EVECelery/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/utils/ErrorLimiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/utils/RequestHeaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/utils/Singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:31:50.000000 EVECelery-0.20/EVECelery/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.295816 EVECelery-0.20/EVECelery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7077 2023-04-23 09:32:01.000000 EVECelery-0.20/EVECelery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    34237 2023-04-23 09:32:01.000000 EVECelery-0.20/EVECelery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 09:32:01.000000 EVECelery-0.20/EVECelery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-23 09:32:01.000000 EVECelery-0.20/EVECelery.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-23 09:32:01.000000 EVECelery-0.20/EVECelery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-23 09:32:01.000000 EVECelery-0.20/EVECelery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-23 09:31:50.000000 EVECelery-0.20/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7077 2023-04-23 09:32:01.355816 EVECelery-0.20/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-04-23 09:31:50.000000 EVECelery-0.20/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-23 09:31:50.000000 EVECelery-0.20/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 09:32:01.355816 EVECelery-0.20/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-04-23 09:31:50.000000 EVECelery-0.20/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:32:01.355816 EVECelery-0.20/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-23 09:31:50.000000 EVECelery-0.20/tests/test_CeleryApps.py
```

### Comparing `EVECelery-0.19/EVECelery/CeleryApps.py` & `EVECelery-0.20/EVECelery/EVECeleryWorker.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,107 +1,109 @@
 from celery import Celery, Task
-from EVECelery.__version__ import __version__, __url__, __license__
-from EVECelery.tasks.Alliance import *
-from EVECelery.tasks.Character import *
-from EVECelery.tasks.Corporation import *
-from EVECelery.tasks.Market import *
-from EVECelery.tasks.Routes import *
-from EVECelery.tasks.Universe import *
+from .__version__ import __version__, __url__, __license__
+from EVECelery.tasks.BaseTasks.TaskBase import TaskBase
+from EVECelery.tasks import TaskDirectory
 from EVECelery.clients.ClientRabbitMQ import ClientRabbitMQ
 from EVECelery.clients.ClientRedis import ClientRedisResultBackend
 import os
 from typing import Optional
+from EVECelery.utils.Singleton import Singleton
+import random
 
 
-class CeleryWorker(object):
+class EVECeleryWorker(metaclass=Singleton):
     """Celery worker server wrapper.
     Creating an instance of this class creates a celery app and registers the default tasks.
 
     :param broker_user: RabbitMQ user
     :param broker_password: RabbitMQ password
     :param broker_host: RabbitMQ hostname
     :param broker_port: RabbitMQ port - normally 5672
     :param broker_vhost: RabbitMQ vhost - namespace for all EVECelery queues
     :param result_user: Redis user - normally "default" if not explicitly configured
     :param result_password: Redis password
     :param result_host: Redis hostname
     :param result_port: Redis port - normally 6379
     :param result_db: Redis db - normally 0 for the default db
-    :param config_object: Custom config object to overwrite the default EVECelery.celeryconfig - optional
-    :param esi_queue_prefix: Prefix to add to all generated ESI queue names
+    :param queue_prefix: Prefix to add to all generated ESI queue names
+    :param worker_log_level: The Celery worker log level for console output
     """
 
     def __init__(self, broker_user: Optional[str] = None, broker_password: Optional[str] = None,
                  broker_host: Optional[str] = None, broker_port: Optional[int] = None,
                  broker_vhost: Optional[str] = None,
                  result_user: Optional[str] = None, result_password: Optional[str] = None,
                  result_host: Optional[str] = None, result_port: Optional[int] = None, result_db: Optional[int] = None,
-                 config_object: str = "EVECelery.celeryconfig", esi_queue_prefix: str = "ESI-",
+                 queue_prefix: str = "EVECelery.", worker_log_level: Optional[str] = 'ERROR',
                  connection_check: bool = False):
         self.broker = ClientRabbitMQ(user=broker_user, password=broker_password, host=broker_host, port=broker_port,
                                      vhost=broker_vhost)
         self.result_backend = ClientRedisResultBackend(user=result_user, password=result_password, host=result_host,
                                                        port=result_port, db=result_db)
 
         if connection_check:
             self.result_backend.check_connection()
+            self.broker.check_connection()
 
-        self.max_concurrency = int(os.environ.get('EVECelery_MaxConcurrency', 4))
+        self.max_concurrency = int(os.environ.get('EVECelery_MaxConcurrency', 10))
+        self.worker_log_level = os.environ.get('EVECelery_LogLevel', worker_log_level)
 
-        self.esi_queue_prefix = esi_queue_prefix
+        self.queue_prefix = queue_prefix
+        self.default_queue = f"{self.queue_prefix}Default"
+
+        self.worker_name = f"EVECeleryWorker{random.randint(1000000, 9999999)}"
         self.app = Celery("EVECelery")
-        self.app.config_from_object(config_object)
-        self.app.conf.update(broker_url=self.broker.connection_str)
-        self.app.conf.update(result_backend=self.result_backend.connection_str)
-        self.app.conf.update(task_default_queue=f"{self.esi_queue_prefix}Default")
+        self.app.conf.update(**self.celery_config())
+
+        self.queues = set()
+        self.queues.add(self.default_queue)
 
-        self.queues = [f"{self.esi_queue_prefix}Default"]
         self.task_routes = {}
         self.beat_schedule = {}
-        self._register_defaults()
+        self._register_all_tasks()
 
-    def esi_tasks(self):
-        """Default ESI tasks
-
-        :return: ESI task instances registered by default
-        """
-        yield AllianceInfo()
-        yield CharacterPublicInfo()
-        yield CorporationInfo()
-        yield PricesList()
-        yield CategoryInfo()
-        yield ConstellationInfo()
-        yield FactionsList()
-        yield GroupInfo()
-        yield RegionInfo()
-        yield Route()
-        yield SystemInfo()
-        yield TypeInfo()
-
-    def tasks_to_register(self):
-        """Yields tuple pairs of (task, queue name) to register with the Celery app
-
-        :return: yields tuple consisting of (task instance, queue name)
-        """
-        for t in self.esi_tasks():
-            yield (t, f"{self.esi_queue_prefix}{t.name}")
-
-    def _register_defaults(self):
-        for t in self.tasks_to_register():
-            self.register_task(t[0])
-            self.register_additional_queue(t[1])
-            self.register_task_route(t[0].name, t[1])
+    def celery_config(self) -> dict:
+        return {
+            'task_serializer': 'json',
+            'result_serializer': 'json',
+            'accept_content': ['json'],
+            'enable_utc': True,
+            'broker_url': self.broker.connection_str,
+            'result_backend': self.result_backend.connection_str,
+            'task_default_queue': self.default_queue,
+            'result_expires': 5400  # default
+        }
+
+    @property
+    def tasks(self) -> TaskDirectory:
+        return TaskDirectory()
+
+    def _register_all_tasks(self):
+        """
+        Register all subtasks that inherit from BaseTask
+
+        This method will register and initialize all subtasks that inherit from BaseTask.
+        """
+        for t in TaskBase.get_all_subtasks():
+            task = t()
+            self.app.register_task(task)
+            if hasattr(task, 'queue_assignment') and task.queue_assignment is not None:
+                q = f'{self.queue_prefix}{task.queue_assignment}'
+                self.register_additional_queue(q)
+                self.register_task_route(task.name, q)
+            else:
+                self.register_task_route(task.name, self.default_queue)
 
     def register_additional_queue(self, queue: str):
         """Register an additional queue that this Celery app should process.
 
         :param queue: Name of the queue
         :return: None
         """
-        self.queues.append(queue)
+        self.queues.add(queue)
 
     def register_task_route(self, task_name: str, queue_name: str):
         """Register a task to a specific queue using a Celery task route.
 
         :param task_name: The name of the task
         :param queue_name: Name of the queue to route tasks to.
         :return: None
@@ -123,32 +125,10 @@
 
     def start(self):
         """Starts the Celery app and beings processing messages in the queues.
 
         :return: None
         """
         self.print_header()
-        self.app.start(argv=["worker", "-l", "WARNING", f"--autoscale={self.max_concurrency},1",
+        self.app.start(argv=["worker", "-l", self.worker_log_level, f"-n{self.worker_name}@%h",
+                             f"--autoscale={self.max_concurrency},1",
                              "-Q", ",".join(self.queues)])
-
-
-class CeleryBeat(CeleryWorker):
-    """Celery beat scheduler for periodic tasks.
-
-    """
-
-    def schedule_task(self, schedule_name: str, schedule_config: dict):
-        """Schedule a task to run at intervals. The passed in schedule object is a dictionary following the
-        format and fields described here:
-        https://docs.celeryproject.org/en/stable/userguide/periodic-tasks.html#available-fields
-
-        :param schedule_name: Name of the scheduled job. This must be unique.
-        :param schedule_config: The scheduled job config as specified at
-            https://docs.celeryproject.org/en/stable/userguide/periodic-tasks.html#available-fields
-        :return: None
-        """
-        self.beat_schedule[schedule_name] = schedule_config
-        self.app.conf.update(beat_schedule=self.beat_schedule)
-
-    def start(self):
-        self.print_header()
-        self.app.start(argv=["beat"])
```

### Comparing `EVECelery-0.19/EVECelery/clients/ClientRabbitMQ.py` & `EVECelery-0.20/EVECelery/clients/ClientRabbitMQ.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 import os
 import sys
 from typing import Optional
 from pydantic import BaseModel
 import traceback
 from .BaseClient import BaseClient
+from EVECelery.utils.Singleton import Singleton
+import pika
 
 
 class ConfigRabbitMQ(BaseModel):
     user: str
     password: str
     host: str
     port: int
     vhost: str
 
 
-class ClientRabbitMQ(BaseClient):
+class ClientRabbitMQ(BaseClient, metaclass=Singleton):
     """
+    The RabbitMQ client wrapper used as the Celery broker service.
 
     :param user: RabbitMQ user
     :param password: RabbitMQ password
     :param host: RabbitMQ hostname
     :param port: RabbitMQ port - normally 5672
     :param vhost: RabbitMQ vhost - namespace for all queues
     """
@@ -40,10 +43,20 @@
         except KeyError as ex:
             traceback.print_exc()
             print(f'The environmental variable is not set for {ex}. '
                   f'Please set this env var or pass it as an argument to initialize ClientRabbitMQ.')
             sys.exit(1)
         self.config = ConfigRabbitMQ(user=user, password=password, host=host, port=port, vhost=vhost)
 
+    def check_connection(self) -> bool:
+        credentials = pika.PlainCredentials(username=self.config.user, password=self.config.password,
+                                            erase_on_connect=True)
+        c = pika.BlockingConnection(pika.ConnectionParameters(host=self.config.host, port=self.config.port,
+                                                              virtual_host=self.config.vhost, credentials=credentials,
+                                                              blocked_connection_timeout=10, socket_timeout=10))
+        c.close()
+        return True
+
+
     @property
     def connection_str(self):
         return f"amqp://{self.config.user}:{self.config.password}@{self.config.host}:{self.config.port}/{self.config.vhost}"
```

### Comparing `EVECelery-0.19/EVECelery/utils/ErrorLimiter.py` & `EVECelery-0.20/EVECelery/utils/ErrorLimiter.py`

 * *Files identical despite different names*

### Comparing `EVECelery-0.19/EVECelery/utils/RequestHeaders.py` & `EVECelery-0.20/EVECelery/utils/RequestHeaders.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 class RequestHeaders(object):
     @classmethod
     def get_email(cls):
         email = os.environ.get('EVECelery_Email')
         if email is None:
-            raise MissingHeaderEmail("Missing 'header_email' variable. "
+            raise MissingHeaderEmail("Missing 'EVECelery_Email' variable. "
                                      "Please set this variable to your email address so ESI and ZK APIs "
                                      "can contact you if there are problems. "
                                      "Requests to ESI or ZK will not occur until this field is set.")
         else:
             return email
 
     @classmethod
```

### Comparing `EVECelery-0.19/EVECelery.egg-info/PKG-INFO` & `EVECelery-0.20/EVECelery.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EVECelery
-Version: 0.19
+Version: 0.20
 Summary: Task queue framework for building tools that interact with the EVE Online ESI API using Celery, RabbitMQ, and Redis.
 Home-page: https://github.com/NullsecSpace/EVECelery
 Author-email: maintainers@nullsec.space
 License: MIT License
 Project-URL: Documentation, https://EVECelery.nullsec.space
 Project-URL: Source, https://github.com/NullsecSpace/EVECelery
 Project-URL: Tracker, https://github.com/NullsecSpace/EVECelery/issues
@@ -14,96 +14,150 @@
 Classifier: Topic :: Games/Entertainment
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # EVECelery
+
 [![PyPI](https://img.shields.io/pypi/v/EVECelery)](https://pypi.org/project/EVECelery)
 [![Documentation Status](https://readthedocs.org/projects/evecelery/badge/?version=latest)](https://evecelery.nullsec.space/en/latest/?badge=latest)
 [![EVECelery](https://github.com/NullsecSpace/EVECelery/actions/workflows/github-actions.yml/badge.svg)](https://github.com/NullsecSpace/EVECelery/actions/workflows/github-actions.yml)
 [![GitHub](https://img.shields.io/github/license/NullsecSpace/EVECelery)](https://github.com/NullsecSpace/EVECelery/blob/main/LICENSE)
 
-EVECelery is a distributed task queue framework for building tools that interact with the [EVE Online ESI API](https://esi.evetech.net/ui) using Celery, RabbitMQ, and Redis.
+EVECelery is a distributed task queue framework for building tools that interact with
+the [EVE Online ESI API](https://esi.evetech.net/ui) using Celery, RabbitMQ, and Redis.
 
-With EVECelery you can easily distribute ESI calls across task queues built on top of [Celery](https://docs.celeryq.dev/) with a fleet of worker nodes.
-You can build on top of EVECelery to create your own tools defining custom tasks and scheduled jobs.
+With EVECelery you can easily distribute ESI calls and tasks across a fleet of worker nodes built using [Celery](https://docs.celeryq.dev/).
+You can create your own tasks on top of EVECelery defining custom functions and scheduled jobs that run alongside the included tasks.
 
 NOTE: This software is in development and may rapidly change or have breaking bugs until the v1.0 release is ready.
 Ensure you use version pinning in your ```requirements.txt```.
 
-# Installation
+- :books: Documentation: https://evecelery.nullsec.space
+- :bulb: Examples: https://evecelery.nullsec.space/en/latest/examples/index.html
+
+## Features
+* Built with [Celery](https://docs.celeryq.dev/) to distribute ESI calls and tasks across a fleet of worker nodes
+* Distributed locking system with Redis ensures stateless workers won't make duplicate API calls if multiple clients run tasks with matching parameters at the same time
+* Cache integration with Redis that caches ESI responses
+* Easily define your own Celery tasks to register with the EVECelery worker nodes
+* Client support for obtaining results synchronously or asynchronously. See [Celery calling tasks](https://docs.celeryq.dev/) for docs on calling tasks.
+* Automated task retry and distributed error rate control limiting across the worker fleet
+* ESI task API designed to mirror the [ESI Swagger Spec](https://esi.evetech.net/ui/) with the same parameter names, responses, and documentation for easy development and code completion
+* Support for periodic scheduled tasks making use of the [Celery beat scheduler](https://docs.celeryq.dev/en/stable/userguide/periodic-tasks.html)
+
+## Installation
+
 ```
 pip install EVECelery
 ```
 
-# Requirements
-EVECelery requires RabbitMQ for the message broker service and Redis for distributed locks, cache, and Celery's result backend (fetching the result of completed tasks).
+## Requirements
+
+EVECelery requires RabbitMQ for the message broker service and Redis for distributed locks, cache, and Celery's result
+backend (fetching the result of completed tasks).
 
-Deploying these two servers through the official Docker images for [RabbitMQ](https://hub.docker.com/_/rabbitmq) and [Redis](https://hub.docker.com/_/redis) is recommended.
+Deploying these two servers through the official Docker images for [RabbitMQ](https://hub.docker.com/_/rabbitmq)
+and [Redis](https://hub.docker.com/_/redis) is recommended.
 
-# Quickstart and Usage
+## Quickstart and Usage
 EVECelery has two components:
 * Celery Worker - The Celery worker server that processes tasks from the message broker and makes requests to ESI on behalf of the client applications 
 * Task api - Collection of Celery tasks to make ESI requests from your client application
 
 You can deploy multiple worker servers that process tasks in the message queues. These worker nodes share locks, error limiting info, and cache requests for clients.
 From your application you make requests using the task api.
 
 
-## Starting the Celery Worker
+### Starting the Celery Worker
 You can start the worker server from either the CLI or your own Python script.
 It is recommended to use the CLI unless you plan on registering your own tasks to the celery worker.
 
-### From CLI
+#### From CLI
 
 Ensure the following environmental variables are set and run the application via bash:
 * EVECelery_RabbitMQ_User
 * EVECelery_RabbitMQ_Password
 * EVECelery_RabbitMQ_Host
 * EVECelery_RabbitMQ_Port
 * EVECelery_RabbitMQ_Vhost
 * EVECelery_Redis_ResultBackend_User
 * EVECelery_Redis_ResultBackend_Password
 * EVECelery_Redis_ResultBackend_Host
 * EVECelery_Redis_ResultBackend_Port
 * EVECelery_Redis_ResultBackend_DB
+* EVECelery_Email
 
 ```shell
 $ eve-celery
 ```
 
-### From your code
+#### From your code
 You can also start the worker from a Python script if you don't want to set environmental variables.
 
 ```python
-from EVECelery.CeleryApps import CeleryWorker
+from EVECelery import EVECeleryWorker
 
-c = CeleryWorker(broker_user="user", broker_password="pass", broker_host="host", broker_port=5672, broker_vhost="esi",
-                 result_user="user", result_password="pass", result_host="host", result_port=6379, result_db=0)
+c = EVECeleryWorker(broker_user="user", broker_password="pass", broker_host="host", broker_port=5672,
+                    broker_vhost="esi",
+                    result_user="user", result_password="pass", result_host="host", result_port=6379, result_db=0)
 
 c.start()
 ```
 
-## Using the task API from your code
+### Using the task API from your code
 From another Python script you can send tasks to the queues and receive results:
 
 ```python
-from EVECelery.CeleryApps import CeleryWorker
-from EVECelery.tasks.Universe import SystemInfo
+from EVECelery import EVECeleryWorker, TaskDirectory
+import json
 
 # only need to make one CeleryWorker in our code to init the tasks and setup connections to RabbitMQ and Redis
 # by not passing connection params to CeleryWorker() the connection info will be read from environmental variables
-c = CeleryWorker()
+c = EVECeleryWorker()
 
 # note we don't call c.start() here as this is not a worker node script.
 # we are calling the task api to submit requests to the message queue which run on the Celery worker nodes
 
-r = SystemInfo().get_sync(timeout=5, system_id=30000142)
-# r is a response dictionary containing system info obtained from ESI.
-# subsequent calls for the same system ID will return results from the cache regardless of requesting client
+r = TaskDirectory.ESI.Universe.get_universe_regions_region_id.get_sync(region_id=10000053)
+# r is the response containing data obtained from ESI
+# subsequent calls with the same parameters return results from the cache regardless of requesting client
+print(json.dumps(r.dict(), indent=2, default=str))
+{
+  "pydantic_model": "Response200_get_universe_regions_region_id",
+  "cache": {
+    "hit": true,
+    "key": "Cache.ESI.Universe.get_universe_regions_region_id.cd252dea2970194b46260124270444f07f4bf449a5fe37ef31f163005fcb50e7",
+    "ttl": 8940
+  },
+  "headers": {
+    "Cache_Control": "public",
+    "Content_Language": "en",
+    "ETag": null,
+    "Expires": "Sun, 23 Apr 2023 11:05:00 GMT",
+    "Last_Modified": "Sat, 22 Apr 2023 11:01:05 GMT"
+  },
+  "body": {
+    "constellations": [
+      20000609,
+      20000610,
+      20000611,
+      20000612,
+      20000613,
+      20000614,
+      20000615,
+      20000616,
+      20000617,
+      20000618
+    ],
+    "description": "A natural destination for explorers and adventurers of all kinds, Cobalt Edge...",
+    "name": "Cobalt Edge",
+    "region_id": 10000053
+  }
+}
 ```
 
-# Copyright Notice
+## Copyright Notice
 
 See [CCP.md](https://github.com/NullsecSpace/EVECelery/blob/main/CCP.md)
```

### Comparing `EVECelery-0.19/LICENSE` & `EVECelery-0.20/LICENSE`

 * *Files identical despite different names*

### Comparing `EVECelery-0.19/PKG-INFO` & `EVECelery-0.20/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EVECelery
-Version: 0.19
+Version: 0.20
 Summary: Task queue framework for building tools that interact with the EVE Online ESI API using Celery, RabbitMQ, and Redis.
 Home-page: https://github.com/NullsecSpace/EVECelery
 Author-email: maintainers@nullsec.space
 License: MIT License
 Project-URL: Documentation, https://EVECelery.nullsec.space
 Project-URL: Source, https://github.com/NullsecSpace/EVECelery
 Project-URL: Tracker, https://github.com/NullsecSpace/EVECelery/issues
@@ -14,96 +14,150 @@
 Classifier: Topic :: Games/Entertainment
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # EVECelery
+
 [![PyPI](https://img.shields.io/pypi/v/EVECelery)](https://pypi.org/project/EVECelery)
 [![Documentation Status](https://readthedocs.org/projects/evecelery/badge/?version=latest)](https://evecelery.nullsec.space/en/latest/?badge=latest)
 [![EVECelery](https://github.com/NullsecSpace/EVECelery/actions/workflows/github-actions.yml/badge.svg)](https://github.com/NullsecSpace/EVECelery/actions/workflows/github-actions.yml)
 [![GitHub](https://img.shields.io/github/license/NullsecSpace/EVECelery)](https://github.com/NullsecSpace/EVECelery/blob/main/LICENSE)
 
-EVECelery is a distributed task queue framework for building tools that interact with the [EVE Online ESI API](https://esi.evetech.net/ui) using Celery, RabbitMQ, and Redis.
+EVECelery is a distributed task queue framework for building tools that interact with
+the [EVE Online ESI API](https://esi.evetech.net/ui) using Celery, RabbitMQ, and Redis.
 
-With EVECelery you can easily distribute ESI calls across task queues built on top of [Celery](https://docs.celeryq.dev/) with a fleet of worker nodes.
-You can build on top of EVECelery to create your own tools defining custom tasks and scheduled jobs.
+With EVECelery you can easily distribute ESI calls and tasks across a fleet of worker nodes built using [Celery](https://docs.celeryq.dev/).
+You can create your own tasks on top of EVECelery defining custom functions and scheduled jobs that run alongside the included tasks.
 
 NOTE: This software is in development and may rapidly change or have breaking bugs until the v1.0 release is ready.
 Ensure you use version pinning in your ```requirements.txt```.
 
-# Installation
+- :books: Documentation: https://evecelery.nullsec.space
+- :bulb: Examples: https://evecelery.nullsec.space/en/latest/examples/index.html
+
+## Features
+* Built with [Celery](https://docs.celeryq.dev/) to distribute ESI calls and tasks across a fleet of worker nodes
+* Distributed locking system with Redis ensures stateless workers won't make duplicate API calls if multiple clients run tasks with matching parameters at the same time
+* Cache integration with Redis that caches ESI responses
+* Easily define your own Celery tasks to register with the EVECelery worker nodes
+* Client support for obtaining results synchronously or asynchronously. See [Celery calling tasks](https://docs.celeryq.dev/) for docs on calling tasks.
+* Automated task retry and distributed error rate control limiting across the worker fleet
+* ESI task API designed to mirror the [ESI Swagger Spec](https://esi.evetech.net/ui/) with the same parameter names, responses, and documentation for easy development and code completion
+* Support for periodic scheduled tasks making use of the [Celery beat scheduler](https://docs.celeryq.dev/en/stable/userguide/periodic-tasks.html)
+
+## Installation
+
 ```
 pip install EVECelery
 ```
 
-# Requirements
-EVECelery requires RabbitMQ for the message broker service and Redis for distributed locks, cache, and Celery's result backend (fetching the result of completed tasks).
+## Requirements
+
+EVECelery requires RabbitMQ for the message broker service and Redis for distributed locks, cache, and Celery's result
+backend (fetching the result of completed tasks).
 
-Deploying these two servers through the official Docker images for [RabbitMQ](https://hub.docker.com/_/rabbitmq) and [Redis](https://hub.docker.com/_/redis) is recommended.
+Deploying these two servers through the official Docker images for [RabbitMQ](https://hub.docker.com/_/rabbitmq)
+and [Redis](https://hub.docker.com/_/redis) is recommended.
 
-# Quickstart and Usage
+## Quickstart and Usage
 EVECelery has two components:
 * Celery Worker - The Celery worker server that processes tasks from the message broker and makes requests to ESI on behalf of the client applications 
 * Task api - Collection of Celery tasks to make ESI requests from your client application
 
 You can deploy multiple worker servers that process tasks in the message queues. These worker nodes share locks, error limiting info, and cache requests for clients.
 From your application you make requests using the task api.
 
 
-## Starting the Celery Worker
+### Starting the Celery Worker
 You can start the worker server from either the CLI or your own Python script.
 It is recommended to use the CLI unless you plan on registering your own tasks to the celery worker.
 
-### From CLI
+#### From CLI
 
 Ensure the following environmental variables are set and run the application via bash:
 * EVECelery_RabbitMQ_User
 * EVECelery_RabbitMQ_Password
 * EVECelery_RabbitMQ_Host
 * EVECelery_RabbitMQ_Port
 * EVECelery_RabbitMQ_Vhost
 * EVECelery_Redis_ResultBackend_User
 * EVECelery_Redis_ResultBackend_Password
 * EVECelery_Redis_ResultBackend_Host
 * EVECelery_Redis_ResultBackend_Port
 * EVECelery_Redis_ResultBackend_DB
+* EVECelery_Email
 
 ```shell
 $ eve-celery
 ```
 
-### From your code
+#### From your code
 You can also start the worker from a Python script if you don't want to set environmental variables.
 
 ```python
-from EVECelery.CeleryApps import CeleryWorker
+from EVECelery import EVECeleryWorker
 
-c = CeleryWorker(broker_user="user", broker_password="pass", broker_host="host", broker_port=5672, broker_vhost="esi",
-                 result_user="user", result_password="pass", result_host="host", result_port=6379, result_db=0)
+c = EVECeleryWorker(broker_user="user", broker_password="pass", broker_host="host", broker_port=5672,
+                    broker_vhost="esi",
+                    result_user="user", result_password="pass", result_host="host", result_port=6379, result_db=0)
 
 c.start()
 ```
 
-## Using the task API from your code
+### Using the task API from your code
 From another Python script you can send tasks to the queues and receive results:
 
 ```python
-from EVECelery.CeleryApps import CeleryWorker
-from EVECelery.tasks.Universe import SystemInfo
+from EVECelery import EVECeleryWorker, TaskDirectory
+import json
 
 # only need to make one CeleryWorker in our code to init the tasks and setup connections to RabbitMQ and Redis
 # by not passing connection params to CeleryWorker() the connection info will be read from environmental variables
-c = CeleryWorker()
+c = EVECeleryWorker()
 
 # note we don't call c.start() here as this is not a worker node script.
 # we are calling the task api to submit requests to the message queue which run on the Celery worker nodes
 
-r = SystemInfo().get_sync(timeout=5, system_id=30000142)
-# r is a response dictionary containing system info obtained from ESI.
-# subsequent calls for the same system ID will return results from the cache regardless of requesting client
+r = TaskDirectory.ESI.Universe.get_universe_regions_region_id.get_sync(region_id=10000053)
+# r is the response containing data obtained from ESI
+# subsequent calls with the same parameters return results from the cache regardless of requesting client
+print(json.dumps(r.dict(), indent=2, default=str))
+{
+  "pydantic_model": "Response200_get_universe_regions_region_id",
+  "cache": {
+    "hit": true,
+    "key": "Cache.ESI.Universe.get_universe_regions_region_id.cd252dea2970194b46260124270444f07f4bf449a5fe37ef31f163005fcb50e7",
+    "ttl": 8940
+  },
+  "headers": {
+    "Cache_Control": "public",
+    "Content_Language": "en",
+    "ETag": null,
+    "Expires": "Sun, 23 Apr 2023 11:05:00 GMT",
+    "Last_Modified": "Sat, 22 Apr 2023 11:01:05 GMT"
+  },
+  "body": {
+    "constellations": [
+      20000609,
+      20000610,
+      20000611,
+      20000612,
+      20000613,
+      20000614,
+      20000615,
+      20000616,
+      20000617,
+      20000618
+    ],
+    "description": "A natural destination for explorers and adventurers of all kinds, Cobalt Edge...",
+    "name": "Cobalt Edge",
+    "region_id": 10000053
+  }
+}
 ```
 
-# Copyright Notice
+## Copyright Notice
 
 See [CCP.md](https://github.com/NullsecSpace/EVECelery/blob/main/CCP.md)
```

### Comparing `EVECelery-0.19/setup.py` & `EVECelery-0.20/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
                      'redis~=4.1',
                      'requests~=2.27',
                      'pydantic~=1.10'
                  ],
                  python_requires=">=3.7",
                  entry_points={
                      'console_scripts': [
-                         'eve-celery = EVECelery:main'
+                         'eve-celery = EVECelery.__main__:main'
                      ]
                  },
                  classifiers=[
                      'Development Status :: 2 - Pre-Alpha',
                      'Programming Language :: Python :: 3.10',
                      'Topic :: Games/Entertainment',
                      'License :: OSI Approved :: MIT License',
```

### Comparing `EVECelery-0.19/tests/test_CeleryApps.py` & `EVECelery-0.20/tests/test_CeleryApps.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from tests.TestUtils import *
 import pytest
-from EVECelery.CeleryApps import CeleryWorker
+from EVECelery import EVECeleryWorker
 from redis.exceptions import ConnectionError
 from redis.exceptions import AuthenticationError
 
 
 class TestCeleryWorker:
     def test_init_no_running_servers(self, mock_env_no_servers):
         """test responses on init when no servers are running"""
         with pytest.raises(ConnectionError):
-            CeleryWorker(connection_check=True)
+            EVECeleryWorker(connection_check=True)
 
-        CeleryWorker()  # should not raise an exception since connection_check is by default false
+        EVECeleryWorker()  # should not raise an exception since connection_check is by default false
 
     def test_init_running_servers(self, mock_env_rabbitmq_redis):
         """test responses on init when servers are running"""
-        CeleryWorker(connection_check=True)  # should not raise an exception
+        EVECeleryWorker(connection_check=True)  # should not raise an exception
 
     def test_init_running_servers_redis_bad_auth(self, mock_env_rabbitmq_redis, monkeypatch):
         """test bad auth to redis"""
         monkeypatch.setenv('EVECelery_Redis_ResultBackend_Password', 'WrongPass')
         with pytest.raises(AuthenticationError):
-            CeleryWorker(connection_check=True)  # should raise auth error
+            EVECeleryWorker(connection_check=True)  # should raise auth error
```

