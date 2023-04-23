# Comparing `tmp/nitrado-1.0.7.tar.gz` & `tmp/nitrado-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nitrado-1.0.7.tar", last modified: Sun Apr 23 20:33:14 2023, max compression
+gzip compressed data, was "nitrado-1.0.8.tar", last modified: Sun Apr 23 21:52:04 2023, max compression
```

## Comparing `nitrado-1.0.7.tar` & `nitrado-1.0.8.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 20:33:14.854306 nitrado-1.0.7/
--rw-rw-rw-   0        0        0     1093 2023-03-25 00:21:47.000000 nitrado-1.0.7/LICENSE
--rw-rw-rw-   0        0        0     3526 2023-04-23 20:33:14.854306 nitrado-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2673 2023-04-23 03:27:46.000000 nitrado-1.0.7/README.md
--rw-rw-rw-   0        0        0      555 2023-04-16 01:48:34.000000 nitrado-1.0.7/pyproject.toml
--rw-rw-rw-   0        0        0     1176 2023-04-23 20:33:14.854306 nitrado-1.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-23 20:33:14.807431 nitrado-1.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-04-23 20:33:14.823054 nitrado-1.0.7/src/nitrado/
--rw-rw-rw-   0        0        0      332 2023-04-23 06:24:51.000000 nitrado-1.0.7/src/nitrado/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 20:33:14.823054 nitrado-1.0.7/src/nitrado/games/
--rw-rw-rw-   0        0        0       43 2023-04-23 05:14:54.000000 nitrado-1.0.7/src/nitrado/games/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 20:33:14.823054 nitrado-1.0.7/src/nitrado/games/ark/
--rw-rw-rw-   0        0        0       56 2023-04-23 04:53:42.000000 nitrado-1.0.7/src/nitrado/games/ark/__init__.py
--rw-rw-rw-   0        0        0     6398 2023-04-23 20:30:30.000000 nitrado-1.0.7/src/nitrado/games/ark/ark_survival.py
-drwxrwxrwx   0        0        0        0 2023-04-23 20:33:14.823054 nitrado-1.0.7/src/nitrado/games/ark/game_specific/
--rw-rw-rw-   0        0        0        0 2023-04-23 05:03:58.000000 nitrado-1.0.7/src/nitrado/games/ark/game_specific/__init__.py
--rw-rw-rw-   0        0        0     1770 2023-04-23 05:44:17.000000 nitrado-1.0.7/src/nitrado/games/ark/game_specific/game_features.py
--rw-rw-rw-   0        0        0     1353 2023-04-23 05:52:11.000000 nitrado-1.0.7/src/nitrado/games/ark/game_specific/game_specific.py
--rw-rw-rw-   0        0        0       98 2023-04-19 12:08:29.000000 nitrado-1.0.7/src/nitrado/games/ark/logs.py
--rw-rw-rw-   0        0        0      893 2023-04-23 04:53:42.000000 nitrado-1.0.7/src/nitrado/games/ark/query.py
-drwxrwxrwx   0        0        0        0 2023-04-23 20:33:14.838681 nitrado-1.0.7/src/nitrado/games/ark/settings/
--rw-rw-rw-   0        0        0        0 2023-04-23 05:03:30.000000 nitrado-1.0.7/src/nitrado/games/ark/settings/__init__.py
--rw-rw-rw-   0        0        0    11956 2023-04-23 05:44:17.000000 nitrado-1.0.7/src/nitrado/games/ark/settings/config.py
--rw-rw-rw-   0        0        0      493 2023-04-23 05:06:51.000000 nitrado-1.0.7/src/nitrado/games/ark/settings/feature_settings.py
--rw-rw-rw-   0        0        0    11429 2023-04-23 05:44:17.000000 nitrado-1.0.7/src/nitrado/games/ark/settings/game_ini.py
--rw-rw-rw-   0        0        0     2921 2023-04-23 05:44:17.000000 nitrado-1.0.7/src/nitrado/games/ark/settings/general.py
--rw-rw-rw-   0        0        0     1575 2023-04-23 05:52:11.000000 nitrado-1.0.7/src/nitrado/games/ark/settings/settings.py
--rw-rw-rw-   0        0        0     5798 2023-04-23 05:44:17.000000 nitrado-1.0.7/src/nitrado/games/ark/settings/start_param.py
-drwxrwxrwx   0        0        0        0 2023-04-23 20:33:14.838681 nitrado-1.0.7/src/nitrado/gameserver/
--rw-rw-rw-   0        0        0       36 2023-04-23 03:36:03.000000 nitrado-1.0.7/src/nitrado/gameserver/__init__.py
--rw-rw-rw-   0        0        0      511 2023-04-23 04:31:25.000000 nitrado-1.0.7/src/nitrado/gameserver/credentials.py
--rw-rw-rw-   0        0        0    19160 2023-04-23 07:18:43.000000 nitrado-1.0.7/src/nitrado/gameserver/gameserver.py
--rw-rw-rw-   0        0        0      877 2023-04-23 04:39:32.000000 nitrado-1.0.7/src/nitrado/gameserver/host_systems.py
--rw-rw-rw-   0        0        0      608 2023-04-23 04:25:36.000000 nitrado-1.0.7/src/nitrado/gameserver/operating_system.py
--rw-rw-rw-   0        0        0      946 2023-04-23 06:35:04.000000 nitrado-1.0.7/src/nitrado/gameserver/players.py
-drwxrwxrwx   0        0        0        0 2023-04-23 20:33:14.838681 nitrado-1.0.7/src/nitrado/globals/
--rw-rw-rw-   0        0        0       29 2023-04-23 04:53:42.000000 nitrado-1.0.7/src/nitrado/globals/__init__.py
--rw-rw-rw-   0        0        0     1272 2023-04-23 07:18:43.000000 nitrado-1.0.7/src/nitrado/globals/globals.py
--rw-rw-rw-   0        0        0      583 2023-04-23 00:50:25.000000 nitrado-1.0.7/src/nitrado/globals/maintenance.py
-drwxrwxrwx   0        0        0        0 2023-04-23 20:33:14.838681 nitrado-1.0.7/src/nitrado/lib/
--rw-rw-rw-   0        0        0       30 2023-04-23 03:36:03.000000 nitrado-1.0.7/src/nitrado/lib/__init__.py
--rw-rw-rw-   0        0        0     2430 2023-04-23 07:01:52.000000 nitrado-1.0.7/src/nitrado/lib/client.py
--rw-rw-rw-   0        0        0     1347 2023-04-16 03:40:10.000000 nitrado-1.0.7/src/nitrado/lib/errors.py
--rw-rw-rw-   0        0        0      549 2023-04-23 06:23:45.000000 nitrado-1.0.7/src/nitrado/nitrado.py
-drwxrwxrwx   0        0        0        0 2023-04-23 20:33:14.838681 nitrado-1.0.7/src/nitrado/oauth/
--rw-rw-rw-   0        0        0        0 2023-04-23 07:16:16.000000 nitrado-1.0.7/src/nitrado/oauth/__init__.py
--rw-rw-rw-   0        0        0        0 2023-03-25 00:21:47.000000 nitrado-1.0.7/src/nitrado/py.typed
-drwxrwxrwx   0        0        0        0 2023-04-23 20:33:14.854306 nitrado-1.0.7/src/nitrado/service/
--rw-rw-rw-   0        0        0       89 2023-04-23 03:36:03.000000 nitrado-1.0.7/src/nitrado/service/__init__.py
--rw-rw-rw-   0        0        0      474 2023-04-23 02:34:26.000000 nitrado-1.0.7/src/nitrado/service/action.py
--rw-rw-rw-   0        0        0      930 2023-04-23 02:34:26.000000 nitrado-1.0.7/src/nitrado/service/arguments.py
--rw-rw-rw-   0        0        0      910 2023-04-23 02:34:26.000000 nitrado-1.0.7/src/nitrado/service/details.py
--rw-rw-rw-   0        0        0      765 2023-04-23 03:22:07.000000 nitrado-1.0.7/src/nitrado/service/log.py
--rw-rw-rw-   0        0        0     1536 2023-04-23 03:17:31.000000 nitrado-1.0.7/src/nitrado/service/logs_page.py
--rw-rw-rw-   0        0        0     1517 2023-04-23 02:24:59.000000 nitrado-1.0.7/src/nitrado/service/notification.py
--rw-rw-rw-   0        0        0     4263 2023-04-23 03:39:31.000000 nitrado-1.0.7/src/nitrado/service/service.py
--rw-rw-rw-   0        0        0     2871 2023-04-23 02:34:26.000000 nitrado-1.0.7/src/nitrado/service/task.py
-drwxrwxrwx   0        0        0        0 2023-04-23 20:33:14.854306 nitrado-1.0.7/src/nitrado/tools/
--rw-rw-rw-   0        0        0        0 2023-04-23 00:21:40.000000 nitrado-1.0.7/src/nitrado/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 20:33:14.823054 nitrado-1.0.7/src/nitrado.egg-info/
--rw-rw-rw-   0        0        0     3526 2023-04-23 20:33:14.000000 nitrado-1.0.7/src/nitrado.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1728 2023-04-23 20:33:14.000000 nitrado-1.0.7/src/nitrado.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 20:33:14.000000 nitrado-1.0.7/src/nitrado.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       93 2023-04-23 20:33:14.000000 nitrado-1.0.7/src/nitrado.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-23 20:33:14.000000 nitrado-1.0.7/src/nitrado.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-23 20:33:14.854306 nitrado-1.0.7/tests/
--rw-rw-rw-   0        0        0     1998 2023-04-23 19:58:07.000000 nitrado-1.0.7/tests/test_connection.py
--rw-rw-rw-   0        0        0    19270 2023-04-23 20:12:30.000000 nitrado-1.0.7/tests/test_game_server.py
--rw-rw-rw-   0        0        0     1662 2023-04-23 20:13:19.000000 nitrado-1.0.7/tests/test_service.py
+drwxrwxrwx   0        0        0        0 2023-04-23 21:52:04.955841 nitrado-1.0.8/
+-rw-rw-rw-   0        0        0     1093 2023-03-25 00:21:47.000000 nitrado-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0     3857 2023-04-23 21:52:04.955841 nitrado-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3004 2023-04-23 21:51:39.000000 nitrado-1.0.8/README.md
+-rw-rw-rw-   0        0        0      555 2023-04-16 01:48:34.000000 nitrado-1.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0     1176 2023-04-23 21:52:04.956429 nitrado-1.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-23 21:52:04.902125 nitrado-1.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-04-23 21:52:04.918516 nitrado-1.0.8/src/nitrado/
+-rw-rw-rw-   0        0        0      332 2023-04-23 06:24:51.000000 nitrado-1.0.8/src/nitrado/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 21:52:04.920945 nitrado-1.0.8/src/nitrado/games/
+-rw-rw-rw-   0        0        0       43 2023-04-23 05:14:54.000000 nitrado-1.0.8/src/nitrado/games/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 21:52:04.920945 nitrado-1.0.8/src/nitrado/games/ark/
+-rw-rw-rw-   0        0        0       56 2023-04-23 04:53:42.000000 nitrado-1.0.8/src/nitrado/games/ark/__init__.py
+-rw-rw-rw-   0        0        0     6598 2023-04-23 21:50:27.000000 nitrado-1.0.8/src/nitrado/games/ark/ark_survival.py
+drwxrwxrwx   0        0        0        0 2023-04-23 21:52:04.920945 nitrado-1.0.8/src/nitrado/games/ark/game_specific/
+-rw-rw-rw-   0        0        0        0 2023-04-23 05:03:58.000000 nitrado-1.0.8/src/nitrado/games/ark/game_specific/__init__.py
+-rw-rw-rw-   0        0        0     1770 2023-04-23 05:44:17.000000 nitrado-1.0.8/src/nitrado/games/ark/game_specific/game_features.py
+-rw-rw-rw-   0        0        0     1353 2023-04-23 05:52:11.000000 nitrado-1.0.8/src/nitrado/games/ark/game_specific/game_specific.py
+-rw-rw-rw-   0        0        0       98 2023-04-19 12:08:29.000000 nitrado-1.0.8/src/nitrado/games/ark/logs.py
+-rw-rw-rw-   0        0        0      893 2023-04-23 04:53:42.000000 nitrado-1.0.8/src/nitrado/games/ark/query.py
+drwxrwxrwx   0        0        0        0 2023-04-23 21:52:04.920945 nitrado-1.0.8/src/nitrado/games/ark/settings/
+-rw-rw-rw-   0        0        0        0 2023-04-23 05:03:30.000000 nitrado-1.0.8/src/nitrado/games/ark/settings/__init__.py
+-rw-rw-rw-   0        0        0    11956 2023-04-23 05:44:17.000000 nitrado-1.0.8/src/nitrado/games/ark/settings/config.py
+-rw-rw-rw-   0        0        0      493 2023-04-23 05:06:51.000000 nitrado-1.0.8/src/nitrado/games/ark/settings/feature_settings.py
+-rw-rw-rw-   0        0        0    11429 2023-04-23 05:44:17.000000 nitrado-1.0.8/src/nitrado/games/ark/settings/game_ini.py
+-rw-rw-rw-   0        0        0     2921 2023-04-23 05:44:17.000000 nitrado-1.0.8/src/nitrado/games/ark/settings/general.py
+-rw-rw-rw-   0        0        0     1575 2023-04-23 05:52:11.000000 nitrado-1.0.8/src/nitrado/games/ark/settings/settings.py
+-rw-rw-rw-   0        0        0     5798 2023-04-23 05:44:17.000000 nitrado-1.0.8/src/nitrado/games/ark/settings/start_param.py
+drwxrwxrwx   0        0        0        0 2023-04-23 21:52:04.935605 nitrado-1.0.8/src/nitrado/gameserver/
+-rw-rw-rw-   0        0        0       36 2023-04-23 03:36:03.000000 nitrado-1.0.8/src/nitrado/gameserver/__init__.py
+-rw-rw-rw-   0        0        0      511 2023-04-23 04:31:25.000000 nitrado-1.0.8/src/nitrado/gameserver/credentials.py
+-rw-rw-rw-   0        0        0    19160 2023-04-23 07:18:43.000000 nitrado-1.0.8/src/nitrado/gameserver/gameserver.py
+-rw-rw-rw-   0        0        0      877 2023-04-23 04:39:32.000000 nitrado-1.0.8/src/nitrado/gameserver/host_systems.py
+-rw-rw-rw-   0        0        0      608 2023-04-23 04:25:36.000000 nitrado-1.0.8/src/nitrado/gameserver/operating_system.py
+-rw-rw-rw-   0        0        0      946 2023-04-23 06:35:04.000000 nitrado-1.0.8/src/nitrado/gameserver/players.py
+drwxrwxrwx   0        0        0        0 2023-04-23 21:52:04.935605 nitrado-1.0.8/src/nitrado/globals/
+-rw-rw-rw-   0        0        0       29 2023-04-23 04:53:42.000000 nitrado-1.0.8/src/nitrado/globals/__init__.py
+-rw-rw-rw-   0        0        0     1272 2023-04-23 07:18:43.000000 nitrado-1.0.8/src/nitrado/globals/globals.py
+-rw-rw-rw-   0        0        0      583 2023-04-23 00:50:25.000000 nitrado-1.0.8/src/nitrado/globals/maintenance.py
+drwxrwxrwx   0        0        0        0 2023-04-23 21:52:04.935605 nitrado-1.0.8/src/nitrado/lib/
+-rw-rw-rw-   0        0        0       30 2023-04-23 03:36:03.000000 nitrado-1.0.8/src/nitrado/lib/__init__.py
+-rw-rw-rw-   0        0        0     2430 2023-04-23 07:01:52.000000 nitrado-1.0.8/src/nitrado/lib/client.py
+-rw-rw-rw-   0        0        0     1347 2023-04-16 03:40:10.000000 nitrado-1.0.8/src/nitrado/lib/errors.py
+-rw-rw-rw-   0        0        0      549 2023-04-23 06:23:45.000000 nitrado-1.0.8/src/nitrado/nitrado.py
+drwxrwxrwx   0        0        0        0 2023-04-23 21:52:04.935605 nitrado-1.0.8/src/nitrado/oauth/
+-rw-rw-rw-   0        0        0        0 2023-04-23 07:16:16.000000 nitrado-1.0.8/src/nitrado/oauth/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-03-25 00:21:47.000000 nitrado-1.0.8/src/nitrado/py.typed
+drwxrwxrwx   0        0        0        0 2023-04-23 21:52:04.951835 nitrado-1.0.8/src/nitrado/service/
+-rw-rw-rw-   0        0        0       89 2023-04-23 03:36:03.000000 nitrado-1.0.8/src/nitrado/service/__init__.py
+-rw-rw-rw-   0        0        0      474 2023-04-23 02:34:26.000000 nitrado-1.0.8/src/nitrado/service/action.py
+-rw-rw-rw-   0        0        0      930 2023-04-23 02:34:26.000000 nitrado-1.0.8/src/nitrado/service/arguments.py
+-rw-rw-rw-   0        0        0      910 2023-04-23 02:34:26.000000 nitrado-1.0.8/src/nitrado/service/details.py
+-rw-rw-rw-   0        0        0      765 2023-04-23 03:22:07.000000 nitrado-1.0.8/src/nitrado/service/log.py
+-rw-rw-rw-   0        0        0     1536 2023-04-23 03:17:31.000000 nitrado-1.0.8/src/nitrado/service/logs_page.py
+-rw-rw-rw-   0        0        0     1517 2023-04-23 02:24:59.000000 nitrado-1.0.8/src/nitrado/service/notification.py
+-rw-rw-rw-   0        0        0     4263 2023-04-23 03:39:31.000000 nitrado-1.0.8/src/nitrado/service/service.py
+-rw-rw-rw-   0        0        0     2871 2023-04-23 02:34:26.000000 nitrado-1.0.8/src/nitrado/service/task.py
+drwxrwxrwx   0        0        0        0 2023-04-23 21:52:04.952843 nitrado-1.0.8/src/nitrado/tools/
+-rw-rw-rw-   0        0        0        0 2023-04-23 00:21:40.000000 nitrado-1.0.8/src/nitrado/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 21:52:04.920945 nitrado-1.0.8/src/nitrado.egg-info/
+-rw-rw-rw-   0        0        0     3857 2023-04-23 21:52:04.000000 nitrado-1.0.8/src/nitrado.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1728 2023-04-23 21:52:04.000000 nitrado-1.0.8/src/nitrado.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 21:52:04.000000 nitrado-1.0.8/src/nitrado.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       93 2023-04-23 21:52:04.000000 nitrado-1.0.8/src/nitrado.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-23 21:52:04.000000 nitrado-1.0.8/src/nitrado.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 21:52:04.954842 nitrado-1.0.8/tests/
+-rw-rw-rw-   0        0        0     1998 2023-04-23 19:58:07.000000 nitrado-1.0.8/tests/test_connection.py
+-rw-rw-rw-   0        0        0    19270 2023-04-23 20:12:30.000000 nitrado-1.0.8/tests/test_game_server.py
+-rw-rw-rw-   0        0        0     1662 2023-04-23 20:13:19.000000 nitrado-1.0.8/tests/test_service.py
```

### Comparing `nitrado-1.0.7/LICENSE` & `nitrado-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.7/PKG-INFO` & `nitrado-1.0.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nitrado
-Version: 1.0.7
+Version: 1.0.8
 Summary: This application accesses the Nitrado API.
 Home-page: https://github.com/mjlomeli/NitradoAPI
 Author: Mauricio
 Author-email: dev.mauricio.lomeli@gmail.com
 Project-URL: Bug Tracker, https://github.com/mjlomeli/NitradoAPI/issues
 Platform: unix
 Platform: linux
@@ -54,53 +54,61 @@
 #### 4. [GameServer](https://github.com/mjlomeli/NitradoAPI/wiki/GameServer)
    > Data directly related to the game server. This includes the player list, game settings, etc.
 
 <br />
 
 # Examples
 
-### Connect to Client
-To begin using the API the Client must first be connected to your Nitrado account.
-Once connected to the client, you should have access to any of the API calls.
+### Connect the Client
+To begin using the API you must have the API key saved as an environment variable.
+The identifer must be labeled as `NITRADO_API_KEY`.
 
+```text
+NITRADO_API_KEY=123456789abcdefghijklmnop
+```
+
+### Saving your API key
+If you don't know how to save your API key as an environment variable, run this 
+to save it in a `.env` file locally. 
+
+If you already have a `.env` file, this will append the key to the file.
+
+An important rule of thumb is to never save this file publicly. Add it to your 
+`.gitignore` file before attempting to upload changes to your repository.
 
 ```python
-from nitrado import NitradoAPI
+from nitrado import initialize
 
-api = NitradoAPI("your-api-key")
+initialize("your-api-key")
 ```
 
 ### Services
 This example highlights how to get the service.
 
 ```python
-from nitrado import NitradoAPI
-
-api = NitradoAPI("your-api-key")
+from nitrado import Service
 
-services = api.services()
+services = Services.all()
 print(services)
 ```
 ```python
 [
     <Service(id=1011111, status='active', type_human='Publicserver 10 slots', suspend_date='2023-05-07T01:21:11')>,
     <Service(id=1022222, status='active', type_human='Publicserver 20 slots', suspend_date='2023-07-07T02:11:01')>,
     <Service(id=1033333, status='active', type_human='Publicserver 30 slots', suspend_date='2023-09-07T06:51:41')>
 ]
 ``` 
 
 #### GameServer
 This example highlights how to get the gameserver.
 
 ```python
-from nitrado import NitradoAPI
-
-api = NitradoAPI("your-api-key")
+from nitrado import GameServer
 
-gameservers = api.game_servers()
+gameservers = GameServer.all()
 print(gameservers)
 ```
 ```python
 [
     <GameServer(service_id=11111111, location='US', slots=10, ip='1.2.3.4', game_human='ARK: Survival Evolved (Xbox One)')>,
     <GameServer(service_id=22222222, location='US', slots=70, ip='11.22.33.44', game_human='ARK: Survival Evolved (Xbox One)')>
 ]
```

### Comparing `nitrado-1.0.7/README.md` & `nitrado-1.0.8/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -29,53 +29,61 @@
 #### 4. [GameServer](https://github.com/mjlomeli/NitradoAPI/wiki/GameServer)
    > Data directly related to the game server. This includes the player list, game settings, etc.
 
 <br />
 
 # Examples
 
-### Connect to Client
-To begin using the API the Client must first be connected to your Nitrado account.
-Once connected to the client, you should have access to any of the API calls.
+### Connect the Client
+To begin using the API you must have the API key saved as an environment variable.
+The identifer must be labeled as `NITRADO_API_KEY`.
 
+```text
+NITRADO_API_KEY=123456789abcdefghijklmnop
+```
+
+### Saving your API key
+If you don't know how to save your API key as an environment variable, run this 
+to save it in a `.env` file locally. 
+
+If you already have a `.env` file, this will append the key to the file.
+
+An important rule of thumb is to never save this file publicly. Add it to your 
+`.gitignore` file before attempting to upload changes to your repository.
 
 ```python
-from nitrado import NitradoAPI
+from nitrado import initialize
 
-api = NitradoAPI("your-api-key")
+initialize("your-api-key")
 ```
 
 ### Services
 This example highlights how to get the service.
 
 ```python
-from nitrado import NitradoAPI
-
-api = NitradoAPI("your-api-key")
+from nitrado import Service
 
-services = api.services()
+services = Services.all()
 print(services)
 ```
 ```python
 [
     <Service(id=1011111, status='active', type_human='Publicserver 10 slots', suspend_date='2023-05-07T01:21:11')>,
     <Service(id=1022222, status='active', type_human='Publicserver 20 slots', suspend_date='2023-07-07T02:11:01')>,
     <Service(id=1033333, status='active', type_human='Publicserver 30 slots', suspend_date='2023-09-07T06:51:41')>
 ]
 ``` 
 
 #### GameServer
 This example highlights how to get the gameserver.
 
 ```python
-from nitrado import NitradoAPI
-
-api = NitradoAPI("your-api-key")
+from nitrado import GameServer
 
-gameservers = api.game_servers()
+gameservers = GameServer.all()
 print(gameservers)
 ```
 ```python
 [
     <GameServer(service_id=11111111, location='US', slots=10, ip='1.2.3.4', game_human='ARK: Survival Evolved (Xbox One)')>,
     <GameServer(service_id=22222222, location='US', slots=70, ip='11.22.33.44', game_human='ARK: Survival Evolved (Xbox One)')>
 ]
```

### Comparing `nitrado-1.0.7/pyproject.toml` & `nitrado-1.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.7/setup.cfg` & `nitrado-1.0.8/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206e 6974 7261 646f 0d0a 7665 7273   = nitrado..vers
-00000020: 696f 6e20 3d20 312e 302e 370d 0a74 6573  ion = 1.0.7..tes
+00000020: 696f 6e20 3d20 312e 302e 380d 0a74 6573  ion = 1.0.8..tes
 00000030: 745f 7665 7273 696f 6e20 3d20 312e 302e  t_version = 1.0.
 00000040: 370d 0a70 726f 6475 6374 696f 6e5f 7665  7..production_ve
-00000050: 7273 696f 6e20 3d20 312e 302e 370d 0a61  rsion = 1.0.7..a
+00000050: 7273 696f 6e20 3d20 312e 302e 380d 0a61  rsion = 1.0.8..a
 00000060: 7574 686f 7220 3d20 4d61 7572 6963 696f  uthor = Mauricio
 00000070: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000080: 2064 6576 2e6d 6175 7269 6369 6f2e 6c6f   dev.mauricio.lo
 00000090: 6d65 6c69 4067 6d61 696c 2e63 6f6d 0d0a  meli@gmail.com..
 000000a0: 6465 7363 7269 7074 696f 6e20 3d20 5468  description = Th
 000000b0: 6973 2061 7070 6c69 6361 7469 6f6e 2061  is application a
 000000c0: 6363 6573 7365 7320 7468 6520 4e69 7472  ccesses the Nitr
```

### Comparing `nitrado-1.0.7/src/nitrado/games/ark/ark_survival.py` & `nitrado-1.0.8/src/nitrado/games/ark/ark_survival.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 from ...lib.client import Client
 from ...gameserver import GameServer
+from ...gameserver.players import Players
 from .query import Query
 from .settings.settings import Settings
 from .game_specific.game_specific import GameSpecific
 from ...lib.errors import assert_response_is_ok
 from ...lib.errors import assert_response_is_json
 import requests
 
@@ -39,14 +40,16 @@
         data['game_specific'] = GameSpecific.from_data(service_id, **data['game_specific'])
         return ArkSurvival(gameserver, **data)
 
     @classmethod
     def all(cls) -> list[ArkSurvival]:
         gameservers = []
         for gameserver in GameServer.all():
+            if gameserver.game != 'arkxb':
+                continue
             data: dict = dict(gameserver)
             data['query'] = Query(gameserver.service_id, **data['query'])
             data['settings'] = Settings.from_data(gameserver.service_id, **data['settings'])
             data['game_specific'] = GameSpecific.from_data(gameserver.service_id, **data['game_specific'])
             gameservers.append(ArkSurvival(gameserver, **data))
         return gameservers
 
@@ -131,14 +134,17 @@
 
     def cluster_id(self) -> str:
         path = f'/services/{self.service_id}/gameservers/games/arkse/gen_cluster_id'
         response = Client.get(path=path)
         data: dict = response.json()['data']
         return data['clusterid']
 
+    def players(self) -> list[Players]:
+        return self.__gameserver.players()
+
     def start(self) -> bool:
         return self.__gameserver.start_game('arkxb')
 
     def restart(self, restart_message: str = None, log_message: str = None) -> bool:
         return self.__gameserver.restart_game(restart_message=restart_message, log_message=log_message)
 
     def reinstall(self) -> bool:
```

### Comparing `nitrado-1.0.7/src/nitrado/games/ark/game_specific/game_features.py` & `nitrado-1.0.8/src/nitrado/games/ark/game_specific/game_features.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.7/src/nitrado/games/ark/game_specific/game_specific.py` & `nitrado-1.0.8/src/nitrado/games/ark/game_specific/game_specific.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.7/src/nitrado/games/ark/query.py` & `nitrado-1.0.8/src/nitrado/games/ark/query.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.7/src/nitrado/games/ark/settings/config.py` & `nitrado-1.0.8/src/nitrado/games/ark/settings/config.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.7/src/nitrado/games/ark/settings/game_ini.py` & `nitrado-1.0.8/src/nitrado/games/ark/settings/game_ini.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.7/src/nitrado/games/ark/settings/general.py` & `nitrado-1.0.8/src/nitrado/games/ark/settings/general.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.7/src/nitrado/games/ark/settings/settings.py` & `nitrado-1.0.8/src/nitrado/games/ark/settings/settings.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.7/src/nitrado/games/ark/settings/start_param.py` & `nitrado-1.0.8/src/nitrado/games/ark/settings/start_param.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.7/src/nitrado/gameserver/gameserver.py` & `nitrado-1.0.8/src/nitrado/gameserver/gameserver.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.7/src/nitrado/gameserver/host_systems.py` & `nitrado-1.0.8/src/nitrado/gameserver/host_systems.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.7/src/nitrado/gameserver/operating_system.py` & `nitrado-1.0.8/src/nitrado/gameserver/operating_system.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.7/src/nitrado/gameserver/players.py` & `nitrado-1.0.8/src/nitrado/gameserver/players.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.7/src/nitrado/globals/globals.py` & `nitrado-1.0.8/src/nitrado/globals/globals.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.7/src/nitrado/globals/maintenance.py` & `nitrado-1.0.8/src/nitrado/globals/maintenance.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.7/src/nitrado/lib/client.py` & `nitrado-1.0.8/src/nitrado/lib/client.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.7/src/nitrado/lib/errors.py` & `nitrado-1.0.8/src/nitrado/lib/errors.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.7/src/nitrado/nitrado.py` & `nitrado-1.0.8/src/nitrado/nitrado.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.7/src/nitrado/service/arguments.py` & `nitrado-1.0.8/src/nitrado/service/arguments.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.7/src/nitrado/service/details.py` & `nitrado-1.0.8/src/nitrado/service/details.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.7/src/nitrado/service/log.py` & `nitrado-1.0.8/src/nitrado/service/log.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.7/src/nitrado/service/logs_page.py` & `nitrado-1.0.8/src/nitrado/service/logs_page.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.7/src/nitrado/service/notification.py` & `nitrado-1.0.8/src/nitrado/service/notification.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.7/src/nitrado/service/service.py` & `nitrado-1.0.8/src/nitrado/service/service.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.7/src/nitrado/service/task.py` & `nitrado-1.0.8/src/nitrado/service/task.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.7/src/nitrado.egg-info/PKG-INFO` & `nitrado-1.0.8/src/nitrado.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nitrado
-Version: 1.0.7
+Version: 1.0.8
 Summary: This application accesses the Nitrado API.
 Home-page: https://github.com/mjlomeli/NitradoAPI
 Author: Mauricio
 Author-email: dev.mauricio.lomeli@gmail.com
 Project-URL: Bug Tracker, https://github.com/mjlomeli/NitradoAPI/issues
 Platform: unix
 Platform: linux
@@ -54,53 +54,61 @@
 #### 4. [GameServer](https://github.com/mjlomeli/NitradoAPI/wiki/GameServer)
    > Data directly related to the game server. This includes the player list, game settings, etc.
 
 <br />
 
 # Examples
 
-### Connect to Client
-To begin using the API the Client must first be connected to your Nitrado account.
-Once connected to the client, you should have access to any of the API calls.
+### Connect the Client
+To begin using the API you must have the API key saved as an environment variable.
+The identifer must be labeled as `NITRADO_API_KEY`.
 
+```text
+NITRADO_API_KEY=123456789abcdefghijklmnop
+```
+
+### Saving your API key
+If you don't know how to save your API key as an environment variable, run this 
+to save it in a `.env` file locally. 
+
+If you already have a `.env` file, this will append the key to the file.
+
+An important rule of thumb is to never save this file publicly. Add it to your 
+`.gitignore` file before attempting to upload changes to your repository.
 
 ```python
-from nitrado import NitradoAPI
+from nitrado import initialize
 
-api = NitradoAPI("your-api-key")
+initialize("your-api-key")
 ```
 
 ### Services
 This example highlights how to get the service.
 
 ```python
-from nitrado import NitradoAPI
-
-api = NitradoAPI("your-api-key")
+from nitrado import Service
 
-services = api.services()
+services = Services.all()
 print(services)
 ```
 ```python
 [
     <Service(id=1011111, status='active', type_human='Publicserver 10 slots', suspend_date='2023-05-07T01:21:11')>,
     <Service(id=1022222, status='active', type_human='Publicserver 20 slots', suspend_date='2023-07-07T02:11:01')>,
     <Service(id=1033333, status='active', type_human='Publicserver 30 slots', suspend_date='2023-09-07T06:51:41')>
 ]
 ``` 
 
 #### GameServer
 This example highlights how to get the gameserver.
 
 ```python
-from nitrado import NitradoAPI
-
-api = NitradoAPI("your-api-key")
+from nitrado import GameServer
 
-gameservers = api.game_servers()
+gameservers = GameServer.all()
 print(gameservers)
 ```
 ```python
 [
     <GameServer(service_id=11111111, location='US', slots=10, ip='1.2.3.4', game_human='ARK: Survival Evolved (Xbox One)')>,
     <GameServer(service_id=22222222, location='US', slots=70, ip='11.22.33.44', game_human='ARK: Survival Evolved (Xbox One)')>
 ]
```

### Comparing `nitrado-1.0.7/src/nitrado.egg-info/SOURCES.txt` & `nitrado-1.0.8/src/nitrado.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.7/tests/test_connection.py` & `nitrado-1.0.8/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.7/tests/test_game_server.py` & `nitrado-1.0.8/tests/test_game_server.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.7/tests/test_service.py` & `nitrado-1.0.8/tests/test_service.py`

 * *Files identical despite different names*

