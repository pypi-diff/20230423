# Comparing `tmp/nitrado-1.0.6.tar.gz` & `tmp/nitrado-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nitrado-1.0.6.tar", last modified: Wed Apr 19 12:38:59 2023, max compression
+gzip compressed data, was "nitrado-1.0.7.tar", last modified: Sun Apr 23 20:33:14 2023, max compression
```

## Comparing `nitrado-1.0.6.tar` & `nitrado-1.0.7.tar`

### file list

```diff
@@ -1,36 +1,69 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 12:38:59.382990 nitrado-1.0.6/
--rw-rw-rw-   0        0        0     1093 2023-03-25 00:21:47.000000 nitrado-1.0.6/LICENSE
--rw-rw-rw-   0        0        0     3435 2023-04-19 12:38:59.382990 nitrado-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2634 2023-04-16 09:41:48.000000 nitrado-1.0.6/README.md
--rw-rw-rw-   0        0        0      555 2023-04-16 01:48:34.000000 nitrado-1.0.6/pyproject.toml
--rw-rw-rw-   0        0        0     1135 2023-04-19 12:38:59.384990 nitrado-1.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-19 12:38:59.348462 nitrado-1.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-04-19 12:38:59.356711 nitrado-1.0.6/src/nitrado/
--rw-rw-rw-   0        0        0      236 2023-03-25 08:45:32.000000 nitrado-1.0.6/src/nitrado/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 12:38:59.370735 nitrado-1.0.6/src/nitrado/games/
--rw-rw-rw-   0        0        0        0 2023-04-16 22:12:29.000000 nitrado-1.0.6/src/nitrado/games/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 12:38:59.372893 nitrado-1.0.6/src/nitrado/games/ark/
--rw-rw-rw-   0        0        0       62 2023-04-19 03:43:26.000000 nitrado-1.0.6/src/nitrado/games/ark/__init__.py
--rw-rw-rw-   0        0        0     3732 2023-04-19 12:32:51.000000 nitrado-1.0.6/src/nitrado/games/ark/ark_survival.py
--rw-rw-rw-   0        0        0       98 2023-04-19 12:08:29.000000 nitrado-1.0.6/src/nitrado/games/ark/logs.py
-drwxrwxrwx   0        0        0        0 2023-04-19 12:38:59.376894 nitrado-1.0.6/src/nitrado/lib/
--rw-rw-rw-   0        0        0       91 2023-03-25 00:51:09.000000 nitrado-1.0.6/src/nitrado/lib/__init__.py
--rw-rw-rw-   0        0        0     1347 2023-04-16 03:40:10.000000 nitrado-1.0.6/src/nitrado/lib/errors.py
--rw-rw-rw-   0        0        0    22391 2023-04-17 02:38:37.000000 nitrado-1.0.6/src/nitrado/lib/game_server.py
--rw-rw-rw-   0        0        0     3889 2023-04-17 00:46:43.000000 nitrado-1.0.6/src/nitrado/lib/service.py
--rw-rw-rw-   0        0        0     3165 2023-04-19 03:43:26.000000 nitrado-1.0.6/src/nitrado/nitrado_api.py
--rw-rw-rw-   0        0        0        0 2023-03-25 00:21:47.000000 nitrado-1.0.6/src/nitrado/py.typed
-drwxrwxrwx   0        0        0        0 2023-04-19 12:38:59.378894 nitrado-1.0.6/src/nitrado/tools/
--rw-rw-rw-   0        0        0       43 2023-03-25 00:37:24.000000 nitrado-1.0.6/src/nitrado/tools/__init__.py
--rw-rw-rw-   0        0        0     1564 2023-04-16 05:08:15.000000 nitrado-1.0.6/src/nitrado/tools/client.py
-drwxrwxrwx   0        0        0        0 2023-04-19 12:38:59.369737 nitrado-1.0.6/src/nitrado.egg-info/
--rw-rw-rw-   0        0        0     3435 2023-04-19 12:38:59.000000 nitrado-1.0.6/src/nitrado.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      689 2023-04-19 12:38:59.000000 nitrado-1.0.6/src/nitrado.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 12:38:59.000000 nitrado-1.0.6/src/nitrado.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       93 2023-04-19 12:38:59.000000 nitrado-1.0.6/src/nitrado.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-19 12:38:59.000000 nitrado-1.0.6/src/nitrado.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-19 12:38:59.381988 nitrado-1.0.6/tests/
--rw-rw-rw-   0        0        0     2251 2023-04-16 05:41:31.000000 nitrado-1.0.6/tests/test_connection.py
--rw-rw-rw-   0        0        0    19592 2023-04-16 09:33:34.000000 nitrado-1.0.6/tests/test_game_server.py
--rw-rw-rw-   0        0        0      106 2023-03-25 08:45:33.000000 nitrado-1.0.6/tests/test_nitrado_api.py
--rw-rw-rw-   0        0        0     2511 2023-03-25 08:45:33.000000 nitrado-1.0.6/tests/test_service.py
+drwxrwxrwx   0        0        0        0 2023-04-23 20:33:14.854306 nitrado-1.0.7/
+-rw-rw-rw-   0        0        0     1093 2023-03-25 00:21:47.000000 nitrado-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0     3526 2023-04-23 20:33:14.854306 nitrado-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2673 2023-04-23 03:27:46.000000 nitrado-1.0.7/README.md
+-rw-rw-rw-   0        0        0      555 2023-04-16 01:48:34.000000 nitrado-1.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0     1176 2023-04-23 20:33:14.854306 nitrado-1.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-23 20:33:14.807431 nitrado-1.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-04-23 20:33:14.823054 nitrado-1.0.7/src/nitrado/
+-rw-rw-rw-   0        0        0      332 2023-04-23 06:24:51.000000 nitrado-1.0.7/src/nitrado/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 20:33:14.823054 nitrado-1.0.7/src/nitrado/games/
+-rw-rw-rw-   0        0        0       43 2023-04-23 05:14:54.000000 nitrado-1.0.7/src/nitrado/games/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 20:33:14.823054 nitrado-1.0.7/src/nitrado/games/ark/
+-rw-rw-rw-   0        0        0       56 2023-04-23 04:53:42.000000 nitrado-1.0.7/src/nitrado/games/ark/__init__.py
+-rw-rw-rw-   0        0        0     6398 2023-04-23 20:30:30.000000 nitrado-1.0.7/src/nitrado/games/ark/ark_survival.py
+drwxrwxrwx   0        0        0        0 2023-04-23 20:33:14.823054 nitrado-1.0.7/src/nitrado/games/ark/game_specific/
+-rw-rw-rw-   0        0        0        0 2023-04-23 05:03:58.000000 nitrado-1.0.7/src/nitrado/games/ark/game_specific/__init__.py
+-rw-rw-rw-   0        0        0     1770 2023-04-23 05:44:17.000000 nitrado-1.0.7/src/nitrado/games/ark/game_specific/game_features.py
+-rw-rw-rw-   0        0        0     1353 2023-04-23 05:52:11.000000 nitrado-1.0.7/src/nitrado/games/ark/game_specific/game_specific.py
+-rw-rw-rw-   0        0        0       98 2023-04-19 12:08:29.000000 nitrado-1.0.7/src/nitrado/games/ark/logs.py
+-rw-rw-rw-   0        0        0      893 2023-04-23 04:53:42.000000 nitrado-1.0.7/src/nitrado/games/ark/query.py
+drwxrwxrwx   0        0        0        0 2023-04-23 20:33:14.838681 nitrado-1.0.7/src/nitrado/games/ark/settings/
+-rw-rw-rw-   0        0        0        0 2023-04-23 05:03:30.000000 nitrado-1.0.7/src/nitrado/games/ark/settings/__init__.py
+-rw-rw-rw-   0        0        0    11956 2023-04-23 05:44:17.000000 nitrado-1.0.7/src/nitrado/games/ark/settings/config.py
+-rw-rw-rw-   0        0        0      493 2023-04-23 05:06:51.000000 nitrado-1.0.7/src/nitrado/games/ark/settings/feature_settings.py
+-rw-rw-rw-   0        0        0    11429 2023-04-23 05:44:17.000000 nitrado-1.0.7/src/nitrado/games/ark/settings/game_ini.py
+-rw-rw-rw-   0        0        0     2921 2023-04-23 05:44:17.000000 nitrado-1.0.7/src/nitrado/games/ark/settings/general.py
+-rw-rw-rw-   0        0        0     1575 2023-04-23 05:52:11.000000 nitrado-1.0.7/src/nitrado/games/ark/settings/settings.py
+-rw-rw-rw-   0        0        0     5798 2023-04-23 05:44:17.000000 nitrado-1.0.7/src/nitrado/games/ark/settings/start_param.py
+drwxrwxrwx   0        0        0        0 2023-04-23 20:33:14.838681 nitrado-1.0.7/src/nitrado/gameserver/
+-rw-rw-rw-   0        0        0       36 2023-04-23 03:36:03.000000 nitrado-1.0.7/src/nitrado/gameserver/__init__.py
+-rw-rw-rw-   0        0        0      511 2023-04-23 04:31:25.000000 nitrado-1.0.7/src/nitrado/gameserver/credentials.py
+-rw-rw-rw-   0        0        0    19160 2023-04-23 07:18:43.000000 nitrado-1.0.7/src/nitrado/gameserver/gameserver.py
+-rw-rw-rw-   0        0        0      877 2023-04-23 04:39:32.000000 nitrado-1.0.7/src/nitrado/gameserver/host_systems.py
+-rw-rw-rw-   0        0        0      608 2023-04-23 04:25:36.000000 nitrado-1.0.7/src/nitrado/gameserver/operating_system.py
+-rw-rw-rw-   0        0        0      946 2023-04-23 06:35:04.000000 nitrado-1.0.7/src/nitrado/gameserver/players.py
+drwxrwxrwx   0        0        0        0 2023-04-23 20:33:14.838681 nitrado-1.0.7/src/nitrado/globals/
+-rw-rw-rw-   0        0        0       29 2023-04-23 04:53:42.000000 nitrado-1.0.7/src/nitrado/globals/__init__.py
+-rw-rw-rw-   0        0        0     1272 2023-04-23 07:18:43.000000 nitrado-1.0.7/src/nitrado/globals/globals.py
+-rw-rw-rw-   0        0        0      583 2023-04-23 00:50:25.000000 nitrado-1.0.7/src/nitrado/globals/maintenance.py
+drwxrwxrwx   0        0        0        0 2023-04-23 20:33:14.838681 nitrado-1.0.7/src/nitrado/lib/
+-rw-rw-rw-   0        0        0       30 2023-04-23 03:36:03.000000 nitrado-1.0.7/src/nitrado/lib/__init__.py
+-rw-rw-rw-   0        0        0     2430 2023-04-23 07:01:52.000000 nitrado-1.0.7/src/nitrado/lib/client.py
+-rw-rw-rw-   0        0        0     1347 2023-04-16 03:40:10.000000 nitrado-1.0.7/src/nitrado/lib/errors.py
+-rw-rw-rw-   0        0        0      549 2023-04-23 06:23:45.000000 nitrado-1.0.7/src/nitrado/nitrado.py
+drwxrwxrwx   0        0        0        0 2023-04-23 20:33:14.838681 nitrado-1.0.7/src/nitrado/oauth/
+-rw-rw-rw-   0        0        0        0 2023-04-23 07:16:16.000000 nitrado-1.0.7/src/nitrado/oauth/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-03-25 00:21:47.000000 nitrado-1.0.7/src/nitrado/py.typed
+drwxrwxrwx   0        0        0        0 2023-04-23 20:33:14.854306 nitrado-1.0.7/src/nitrado/service/
+-rw-rw-rw-   0        0        0       89 2023-04-23 03:36:03.000000 nitrado-1.0.7/src/nitrado/service/__init__.py
+-rw-rw-rw-   0        0        0      474 2023-04-23 02:34:26.000000 nitrado-1.0.7/src/nitrado/service/action.py
+-rw-rw-rw-   0        0        0      930 2023-04-23 02:34:26.000000 nitrado-1.0.7/src/nitrado/service/arguments.py
+-rw-rw-rw-   0        0        0      910 2023-04-23 02:34:26.000000 nitrado-1.0.7/src/nitrado/service/details.py
+-rw-rw-rw-   0        0        0      765 2023-04-23 03:22:07.000000 nitrado-1.0.7/src/nitrado/service/log.py
+-rw-rw-rw-   0        0        0     1536 2023-04-23 03:17:31.000000 nitrado-1.0.7/src/nitrado/service/logs_page.py
+-rw-rw-rw-   0        0        0     1517 2023-04-23 02:24:59.000000 nitrado-1.0.7/src/nitrado/service/notification.py
+-rw-rw-rw-   0        0        0     4263 2023-04-23 03:39:31.000000 nitrado-1.0.7/src/nitrado/service/service.py
+-rw-rw-rw-   0        0        0     2871 2023-04-23 02:34:26.000000 nitrado-1.0.7/src/nitrado/service/task.py
+drwxrwxrwx   0        0        0        0 2023-04-23 20:33:14.854306 nitrado-1.0.7/src/nitrado/tools/
+-rw-rw-rw-   0        0        0        0 2023-04-23 00:21:40.000000 nitrado-1.0.7/src/nitrado/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 20:33:14.823054 nitrado-1.0.7/src/nitrado.egg-info/
+-rw-rw-rw-   0        0        0     3526 2023-04-23 20:33:14.000000 nitrado-1.0.7/src/nitrado.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1728 2023-04-23 20:33:14.000000 nitrado-1.0.7/src/nitrado.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 20:33:14.000000 nitrado-1.0.7/src/nitrado.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       93 2023-04-23 20:33:14.000000 nitrado-1.0.7/src/nitrado.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-23 20:33:14.000000 nitrado-1.0.7/src/nitrado.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 20:33:14.854306 nitrado-1.0.7/tests/
+-rw-rw-rw-   0        0        0     1998 2023-04-23 19:58:07.000000 nitrado-1.0.7/tests/test_connection.py
+-rw-rw-rw-   0        0        0    19270 2023-04-23 20:12:30.000000 nitrado-1.0.7/tests/test_game_server.py
+-rw-rw-rw-   0        0        0     1662 2023-04-23 20:13:19.000000 nitrado-1.0.7/tests/test_service.py
```

### Comparing `nitrado-1.0.6/LICENSE` & `nitrado-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.6/PKG-INFO` & `nitrado-1.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,46 @@
 Metadata-Version: 2.1
 Name: nitrado
-Version: 1.0.6
+Version: 1.0.7
 Summary: This application accesses the Nitrado API.
 Home-page: https://github.com/mjlomeli/NitradoAPI
 Author: Mauricio
 Author-email: dev.mauricio.lomeli@gmail.com
 Project-URL: Bug Tracker, https://github.com/mjlomeli/NitradoAPI/issues
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
 Platform: win32
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
 # Python Nitrado SDK
 
 [![Testing](https://github.com/mjlomeli/NitradoAPI/actions/workflows/tests.yml/badge.svg)](#) tests need a Nitrado subscription account 
 
 
 A Python based SDK for the [Nitrado RESTful API](https://doc.nitrado.net/) published at [PyPI](https://pypi.org/project/nitrado/).
 
+# Installation
+In your terminal install the nitrado package with pip.
+
+```shell
+pip install nitrado
+```
+
 
 # Overview
 
 To have access to this application you must have an account created at [Nitrado](https://server.nitrado.net/)
 and create an API key.
 
 # [Wiki - Full documentation](https://github.com/mjlomeli/NitradoAPI/wiki)
@@ -44,23 +52,14 @@
 #### 3. [Services](https://github.com/mjlomeli/NitradoAPI/wiki/Services)
    > Data provided outside of the game server. Like server status, user id, and auto extension plan.
 #### 4. [GameServer](https://github.com/mjlomeli/NitradoAPI/wiki/GameServer)
    > Data directly related to the game server. This includes the player list, game settings, etc.
 
 <br />
 
-# Installation
-In your terminal install the nitrado package with pip.
-
-```shell
-pip install nitrado
-```
-
-<br />
-
 # Examples
 
 ### Connect to Client
 To begin using the API the Client must first be connected to your Nitrado account.
 Once connected to the client, you should have access to any of the API calls.
 
 
@@ -74,15 +73,16 @@
 This example highlights how to get the service.
 
 ```python
 from nitrado import NitradoAPI
 
 api = NitradoAPI("your-api-key")
 
-api.services()
+services = api.services()
+print(services)
 ```
 ```python
 [
     <Service(id=1011111, status='active', type_human='Publicserver 10 slots', suspend_date='2023-05-07T01:21:11')>,
     <Service(id=1022222, status='active', type_human='Publicserver 20 slots', suspend_date='2023-07-07T02:11:01')>,
     <Service(id=1033333, status='active', type_human='Publicserver 30 slots', suspend_date='2023-09-07T06:51:41')>
 ]
@@ -92,15 +92,16 @@
 This example highlights how to get the gameserver.
 
 ```python
 from nitrado import NitradoAPI
 
 api = NitradoAPI("your-api-key")
 
-gameserver = api.game_servers()
+gameservers = api.game_servers()
+print(gameservers)
 ```
 ```python
 [
     <GameServer(service_id=11111111, location='US', slots=10, ip='1.2.3.4', game_human='ARK: Survival Evolved (Xbox One)')>,
     <GameServer(service_id=22222222, location='US', slots=70, ip='11.22.33.44', game_human='ARK: Survival Evolved (Xbox One)')>
 ]
 ```
```

### Comparing `nitrado-1.0.6/README.md` & `nitrado-1.0.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 # Python Nitrado SDK
 
 [![Testing](https://github.com/mjlomeli/NitradoAPI/actions/workflows/tests.yml/badge.svg)](#) tests need a Nitrado subscription account 
 
 
 A Python based SDK for the [Nitrado RESTful API](https://doc.nitrado.net/) published at [PyPI](https://pypi.org/project/nitrado/).
 
+# Installation
+In your terminal install the nitrado package with pip.
+
+```shell
+pip install nitrado
+```
+
 
 # Overview
 
 To have access to this application you must have an account created at [Nitrado](https://server.nitrado.net/)
 and create an API key.
 
 # [Wiki - Full documentation](https://github.com/mjlomeli/NitradoAPI/wiki)
@@ -20,23 +27,14 @@
 #### 3. [Services](https://github.com/mjlomeli/NitradoAPI/wiki/Services)
    > Data provided outside of the game server. Like server status, user id, and auto extension plan.
 #### 4. [GameServer](https://github.com/mjlomeli/NitradoAPI/wiki/GameServer)
    > Data directly related to the game server. This includes the player list, game settings, etc.
 
 <br />
 
-# Installation
-In your terminal install the nitrado package with pip.
-
-```shell
-pip install nitrado
-```
-
-<br />
-
 # Examples
 
 ### Connect to Client
 To begin using the API the Client must first be connected to your Nitrado account.
 Once connected to the client, you should have access to any of the API calls.
 
 
@@ -50,15 +48,16 @@
 This example highlights how to get the service.
 
 ```python
 from nitrado import NitradoAPI
 
 api = NitradoAPI("your-api-key")
 
-api.services()
+services = api.services()
+print(services)
 ```
 ```python
 [
     <Service(id=1011111, status='active', type_human='Publicserver 10 slots', suspend_date='2023-05-07T01:21:11')>,
     <Service(id=1022222, status='active', type_human='Publicserver 20 slots', suspend_date='2023-07-07T02:11:01')>,
     <Service(id=1033333, status='active', type_human='Publicserver 30 slots', suspend_date='2023-09-07T06:51:41')>
 ]
@@ -68,15 +67,16 @@
 This example highlights how to get the gameserver.
 
 ```python
 from nitrado import NitradoAPI
 
 api = NitradoAPI("your-api-key")
 
-gameserver = api.game_servers()
+gameservers = api.game_servers()
+print(gameservers)
 ```
 ```python
 [
     <GameServer(service_id=11111111, location='US', slots=10, ip='1.2.3.4', game_human='ARK: Survival Evolved (Xbox One)')>,
     <GameServer(service_id=22222222, location='US', slots=70, ip='11.22.33.44', game_human='ARK: Survival Evolved (Xbox One)')>
 ]
 ```
```

### Comparing `nitrado-1.0.6/pyproject.toml` & `nitrado-1.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.6/setup.cfg` & `nitrado-1.0.7/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206e 6974 7261 646f 0d0a 7665 7273   = nitrado..vers
-00000020: 696f 6e20 3d20 312e 302e 360d 0a74 6573  ion = 1.0.6..tes
+00000020: 696f 6e20 3d20 312e 302e 370d 0a74 6573  ion = 1.0.7..tes
 00000030: 745f 7665 7273 696f 6e20 3d20 312e 302e  t_version = 1.0.
-00000040: 360d 0a70 726f 6475 6374 696f 6e5f 7665  6..production_ve
-00000050: 7273 696f 6e20 3d20 312e 302e 360d 0a61  rsion = 1.0.6..a
+00000040: 370d 0a70 726f 6475 6374 696f 6e5f 7665  7..production_ve
+00000050: 7273 696f 6e20 3d20 312e 302e 370d 0a61  rsion = 1.0.7..a
 00000060: 7574 686f 7220 3d20 4d61 7572 6963 696f  uthor = Mauricio
 00000070: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000080: 2064 6576 2e6d 6175 7269 6369 6f2e 6c6f   dev.mauricio.lo
 00000090: 6d65 6c69 4067 6d61 696c 2e63 6f6d 0d0a  meli@gmail.com..
 000000a0: 6465 7363 7269 7074 696f 6e20 3d20 5468  description = Th
 000000b0: 6973 2061 7070 6c69 6361 7469 6f6e 2061  is application a
 000000c0: 6363 6573 7365 7320 7468 6520 4e69 7472  ccesses the Nitr
@@ -34,38 +34,41 @@
 00000210: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
 00000220: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
 00000230: 3320 3a3a 204f 6e6c 790d 0a09 5072 6f67  3 :: Only...Prog
 00000240: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
 00000250: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
 00000260: 390d 0a09 5072 6f67 7261 6d6d 696e 6720  9...Programming 
 00000270: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000280: 6f6e 203a 3a20 332e 3130 0d0a 090d 0a09  on :: 3.10......
-00000290: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
-000002a0: 7070 726f 7665 6420 3a3a 204d 4954 204c  pproved :: MIT L
-000002b0: 6963 656e 7365 0d0a 094f 7065 7261 7469  icense...Operati
-000002c0: 6e67 2053 7973 7465 6d20 3a3a 204f 5320  ng System :: OS 
-000002d0: 496e 6465 7065 6e64 656e 740d 0a0d 0a5b  Independent....[
-000002e0: 6f70 7469 6f6e 735d 0d0a 7061 636b 6167  options]..packag
-000002f0: 655f 6469 7220 3d20 0d0a 093d 2073 7263  e_dir = ...= src
-00000300: 0d0a 7061 636b 6167 6573 203d 2066 696e  ..packages = fin
-00000310: 643a 0d0a 7079 7468 6f6e 5f72 6571 7569  d:..python_requi
-00000320: 7265 7320 3d20 3e3d 332e 390d 0a69 6e73  res = >=3.9..ins
-00000330: 7461 6c6c 5f72 6571 7569 7265 7320 3d20  tall_requires = 
-00000340: 0d0a 0977 6865 656c 0d0a 0972 6571 7565  ...wheel...reque
-00000350: 7374 733d 3d32 2e2a 0d0a 0d0a 5b6f 7074  sts==2.*....[opt
-00000360: 696f 6e73 2e70 6163 6b61 6765 732e 6669  ions.packages.fi
-00000370: 6e64 5d0d 0a77 6865 7265 203d 2073 7263  nd]..where = src
-00000380: 0d0a 0d0a 5b6f 7074 696f 6e73 2e65 7874  ....[options.ext
-00000390: 7261 735f 7265 7175 6972 655d 0d0a 7465  ras_require]..te
-000003a0: 7374 696e 6720 3d20 0d0a 0970 7974 6573  sting = ...pytes
-000003b0: 743e 3d36 2e30 0d0a 0970 7974 6573 742d  t>=6.0...pytest-
-000003c0: 636f 763e 3d32 2e30 0d0a 096d 7970 793e  cov>=2.0...mypy>
-000003d0: 3d30 2e39 3130 0d0a 0966 6c61 6b65 383e  =0.910...flake8>
-000003e0: 3d33 2e39 0d0a 0974 6f78 3e3d 332e 3234  =3.9...tox>=3.24
-000003f0: 0d0a 0d0a 5b6f 7074 696f 6e73 2e70 6163  ....[options.pac
-00000400: 6b61 6765 5f64 6174 615d 0d0a 6e69 7472  kage_data]..nitr
-00000410: 6164 6f20 3d20 7079 2e74 7970 6564 0d0a  ado = py.typed..
-00000420: 0d0a 5b66 6c61 6b65 385d 0d0a 6d61 782d  ..[flake8]..max-
-00000430: 6c69 6e65 2d6c 656e 6774 6820 3d20 3136  line-length = 16
-00000440: 300d 0a0d 0a5b 6567 675f 696e 666f 5d0d  0....[egg_info].
-00000450: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
-00000460: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
+00000280: 6f6e 203a 3a20 332e 3130 0d0a 0950 726f  on :: 3.10...Pro
+00000290: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+000002a0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+000002b0: 2e31 310d 0a09 0d0a 094c 6963 656e 7365  .11......License
+000002c0: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
+000002d0: 203a 3a20 4d49 5420 4c69 6365 6e73 650d   :: MIT License.
+000002e0: 0a09 4f70 6572 6174 696e 6720 5379 7374  ..Operating Syst
+000002f0: 656d 203a 3a20 4f53 2049 6e64 6570 656e  em :: OS Indepen
+00000300: 6465 6e74 0d0a 0d0a 5b6f 7074 696f 6e73  dent....[options
+00000310: 5d0d 0a70 6163 6b61 6765 5f64 6972 203d  ]..package_dir =
+00000320: 200d 0a09 3d20 7372 630d 0a70 6163 6b61   ...= src..packa
+00000330: 6765 7320 3d20 6669 6e64 3a0d 0a70 7974  ges = find:..pyt
+00000340: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
+00000350: 3d33 2e39 0d0a 696e 7374 616c 6c5f 7265  =3.9..install_re
+00000360: 7175 6972 6573 203d 200d 0a09 7768 6565  quires = ...whee
+00000370: 6c0d 0a09 7265 7175 6573 7473 3d3d 322e  l...requests==2.
+00000380: 2a0d 0a0d 0a5b 6f70 7469 6f6e 732e 7061  *....[options.pa
+00000390: 636b 6167 6573 2e66 696e 645d 0d0a 7768  ckages.find]..wh
+000003a0: 6572 6520 3d20 7372 630d 0a0d 0a5b 6f70  ere = src....[op
+000003b0: 7469 6f6e 732e 6578 7472 6173 5f72 6571  tions.extras_req
+000003c0: 7569 7265 5d0d 0a74 6573 7469 6e67 203d  uire]..testing =
+000003d0: 200d 0a09 7079 7465 7374 3e3d 362e 300d   ...pytest>=6.0.
+000003e0: 0a09 7079 7465 7374 2d63 6f76 3e3d 322e  ..pytest-cov>=2.
+000003f0: 300d 0a09 6d79 7079 3e3d 302e 3931 300d  0...mypy>=0.910.
+00000400: 0a09 666c 616b 6538 3e3d 332e 390d 0a09  ..flake8>=3.9...
+00000410: 746f 783e 3d33 2e32 340d 0a0d 0a5b 6f70  tox>=3.24....[op
+00000420: 7469 6f6e 732e 7061 636b 6167 655f 6461  tions.package_da
+00000430: 7461 5d0d 0a6e 6974 7261 646f 203d 2070  ta]..nitrado = p
+00000440: 792e 7479 7065 640d 0a0d 0a5b 666c 616b  y.typed....[flak
+00000450: 6538 5d0d 0a6d 6178 2d6c 696e 652d 6c65  e8]..max-line-le
+00000460: 6e67 7468 203d 2031 3630 0d0a 0d0a 5b65  ngth = 160....[e
+00000470: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
+00000480: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
+00000490: 203d 2030 0d0a 0d0a                       = 0....
```

### Comparing `nitrado-1.0.6/src/nitrado/lib/errors.py` & `nitrado-1.0.7/src/nitrado/lib/errors.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.6/src/nitrado/lib/game_server.py` & `nitrado-1.0.7/src/nitrado/gameserver/gameserver.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,496 +1,439 @@
-from nitrado.lib.errors import assert_response_is_ok
-from nitrado.lib.service import Service
-from nitrado.tools import Client
-import requests
-from pathlib import Path
-import json
+from __future__ import annotations
+from ..lib.client import Client
+from ..service.service import Service
+from .host_systems import HostSystem
+from .operating_system import OperatingSystem
+from .credentials import Credentials
+from .players import Players
 
 
 class GameServer:
-    def __init__(self, client: Client, data: dict):
-        self.__client = client
-        self.__data = data
-
-        self.status = None
-        self.last_status_change = None
-        self.must_be_started = None
-        self.websocket_token = None
-        self.hostsystems = None
-        self.username = None
-        self.user_id = None
-        self.service_id = None
-        self.location_id = None
-        self.minecraft_mode = None
-        self.ip = None
-        self.ipv6 = None
-        self.port = None
-        self.query_port = None
-        self.rcon_port = None
-        self.label = None
-        self.type = None
-        self.memory = None
-        self.memory_mb = None
-        self.game = None
-        self.game_human = None
-        self.game_specific = None
-        self.modpacks = None
-        self.slots = None
-        self.location = None
-        self.credentials = None
-        self.settings = None
-        self.quota = None
-        self.query = None
-        for k, v in data.items():
+    @classmethod
+    def find_by_id(cls, service_id: int) -> GameServer:
+        response = Client.get(path=f'/services/{service_id}/gameservers')
+        data: dict = response.json()['data']['gameserver']
+        data['hostsystems'] = HostSystem(service_id, **{
+            name: OperatingSystem(service_id, **values)
+            for name, values in data['hostsystems'].items()
+        })
+        data['credentials'] = Credentials(service_id, **data['credentials'])
+        return GameServer(**data)
+
+    @classmethod
+    def all(cls) -> list[GameServer]:
+        game_servers = []
+        for service in Service.all():
+            game_server = cls.find_by_id(service.id)
+            game_servers.append(game_server)
+        return game_servers
+
+    def __init__(
+            self,
+            status: str = None,
+            last_status_change: int = None,
+            must_be_started: bool = None,
+            websocket_token: str = None,
+            hostsystems: dict = None,
+            username: str = None,
+            user_id: int = None,
+            service_id: int = None,
+            location_id: int = None,
+            minecraft_mode: bool = None,
+            ip: str = None,
+            ipv6: str = None,
+            port: int = None,
+            query_port: int = None,
+            rcon_port: int = None,
+            label: str = None,
+            type: str = None,
+            memory: str = None,
+            memory_mb: int = None,
+            game: str = None,
+            game_human: str = None,
+            game_specific: dict = None,
+            modpacks: dict = None,
+            slots: int = None,
+            location: str = None,
+            credentials: dict = None,
+            settings: dict = None,
+            quota: str = None,
+            query: dict = None,
+            **kwargs
+    ):
+        self.status = status
+        self.last_status_change = last_status_change
+        self.must_be_started = must_be_started
+        self.websocket_token = websocket_token
+        self.hostsystems = hostsystems
+        self.username = username
+        self.user_id = user_id
+        self.service_id = service_id
+        self.location_id = location_id
+        self.minecraft_mode = minecraft_mode
+        self.ip = ip
+        self.ipv6 = ipv6
+        self.port = port
+        self.query_port = query_port
+        self.rcon_port = rcon_port
+        self.label = label
+        self.type = type
+        self.memory = memory
+        self.memory_mb = memory_mb
+        self.game = game
+        self.game_human = game_human
+        self.game_specific = game_specific
+        self.modpacks = modpacks
+        self.slots = slots
+        self.location = location
+        self.credentials = credentials
+        self.settings = settings
+        self.quota = quota
+        self.query = query
+        for k, v in kwargs.items():
             self.__dict__[k] = v
 
-    def service(self) -> Service:
-        response = self.__client.get(path=f'/services/{self.service_id}')
-        data: dict = response.json()['data']
-        return Service(self.__client, data['service'])
-
-    def cluster_id(self) -> str:
-        path = f'/services/{self.service_id}/gameservers/games/arkse/gen_cluster_id'
-        response = self.__client.get(path=path)
-        data: dict = response.json()['data']
-        return data['clusterid']
-
-    def logs_shooter_game(self) -> str:
-        """ Refreshes about every 15+/- minutes """
-        path = f'/services/{self.service_id}/gameservers/file_server/download'
-        params = {'file': f"/games/{self.username}/noftp/arkxb/ShooterGame/Saved/Logs/ShooterGame.log"}
-        response = self.__client.get(path=path, params=params)
-        data: dict = response.json()['data']
-        url = data['token']['url']
-        log_response = requests.get(url)
-        assert_response_is_ok(log_response)
-        return log_response.text.replace("\r\n", "\n")
-
-    def logs_restart(self) -> str:
-        """ Refreshes about every 15+/- minutes """
-        path = f'/services/{self.service_id}/gameservers/file_server/download'
-        params = {'file': f"/games/{self.username}/ftproot/restart.log"}
-        response = self.__client.get(path=path, params=params)
-        data: dict = response.json()['data']
-        url = data['token']['url']
-        log_response = requests.get(url)
-        assert_response_is_ok(log_response)
-        return log_response.text.replace("\r\n", "\n")
-
-    def logs_shooter_game_last(self) -> str:
-        """ Refreshes about every 15+/- minutes """
-        path = f'/services/{self.service_id}/gameservers/file_server/download'
-        params = {'file': f"/games/{self.username}/noftp/arkxb/ShooterGame/Saved/Logs/ShooterGame_Last.log"}
-        response = self.__client.get(path=path, params=params)
+    def players(self) -> list[Players]:
+        path = f'/services/{self.service_id}/gameservers/games/players'
+        response = Client.get(path=path)
         data: dict = response.json()['data']
-        url = data['token']['url']
-        log_response = requests.get(url)
-        assert_response_is_ok(log_response)
-        return log_response.text.replace("\r\n", "\n")
-
-    def logs_download(self, directory: str = None) -> None:
-        location = Path(directory or Path.cwd())
-        if not location.is_dir():
-            raise NotADirectoryError(f"Directory does not exist: {directory}")
-        with open(location / Path('shooter_games.txt'), 'w') as w:
-            w.write(self.logs_shooter_game())
-        with open(location / Path('shooter_games_last.txt'), 'w') as w:
-            w.write(self.logs_shooter_game_last())
-        with open(location / Path('restart.txt'), 'w') as w:
-            w.write(self.logs_restart())
-
-    def start(self, game: str) -> bool:
-        """ :param game: Provide the Folder Short of the specific game. """
-        path = f'/services/{self.service_id}/gameservers/games/start'
-        params = {'game': game}
-        response = self.__client.post(path=path, params=params)
-        data: dict = response.json()
-        return response.ok and data['status'] == 'success'
+        return [Players(self.service_id, **player) for player in data['players']]
 
     def is_gameserver_restorable(self, folder, backup_id) -> bool:
         path = f'/services/{self.service_id}/gameservers/backups/restore_possible'
         params = {'folder': folder, 'backup': backup_id}
-        response = self.__client.post(path=path, params=params)
+        response = Client.post(path=path, params=params)
         data: dict = response.json()
         return response.ok and data['status'] == 'success'
 
     def gameserver_restore(self, folder, backup_id) -> bool:
         path = f'/services/{self.service_id}/gameservers/backups/gameserver'
         params = {'folder': folder, 'backup': backup_id}
-        response = self.__client.post(path=path, params=params)
+        response = Client.post(path=path, params=params)
         data: dict = response.json()
         return response.ok and data['status'] == 'success'
 
-    def download_file(self, file_path) -> dict:
-        path = f'/services/{self.service_id}/gameservers/file_server/download'
-        params = {'file': file_path}
-        response = self.__client.get(path=path, params=params)
-        data: dict = response.json()['data']
-        return data
-
-    def rename_file(self, file_path, target_path, target_name) -> bool:
-        path = f'/services/{self.service_id}/gameservers/file_server/move'
-        params = {'source_path': file_path, 'target_path': target_path, 'target_filename': target_name}
-        response = self.__client.post(path=path, params=params)
-        data:dict = response.json()
-        return response.ok and data['status'] == 'success'
-
-    # def rename_file(self, file_path, new_name):
-    #     path = f'/services/{self.service_id}/gameservers/file_server/move'
-    #     target_path = '/'.join(file_path.split("/")[:-1])
-    #     params = {'source_path': file_path, 'target_path': target_path, 'target_filename': new_name}
-    #     return self._client.post(path=path, params=params)
-
-    def donation_history(self, page=0) -> dict:
-        path = f'/services/{self.service_id}/gameservers/boost/history'
-        params = {'page': page}
-        response = self.__client.get(path=path, params=params)
-        data: dict = response.json()['data']
-        return data
-
-    def donation_settings(self) -> dict:
-        path = f'/services/{self.service_id}/gameservers/boost'
-        response = self.__client.get(path=path)
-        data: dict = response.json()['data']
-        return data['boosting']
-
-    def update_donation_settings(self, enable=True, message=None, welcome_message=None) -> dict:
-        path = f'/services/{self.service_id}/gameservers/boost'
-        params = {'enable': enable, 'message': message, 'welcome_message': welcome_message}
-        response = self.__client.put(path=path, params=params)
-        data: dict = response.json()
-        return data['boosting']
-
-    def players(self) -> list:
-        path = f'/services/{self.service_id}/gameservers/games/players'
-        response = self.__client.get(path=path)
-        data: dict = response.json()['data']
-        return data['players']
-
     def white_list_player(self, gamertag: str) -> bool:
         """
         Player_Management - Add Player to Whitelist
         :param gamertag: Player unique identifier.
         """
-        params = {"identifer": gamertag}
+        params = {"identifier": gamertag}
         path = f'/services/{self.service_id}/gameservers/games/whitelist'
-        response = self.__client.put(path=path, params=params)
+        response = Client.post(path=path, params=params)
         data: dict = response.json()
         return response.ok and data['status'] == 'success'
 
     def admin_list(self) -> list:
         path = f'/services/{self.service_id}/gameservers/games/adminlist'
-        response = self.__client.post(path=path)
+        response = Client.get(path=path)
         data: dict = response.json()['data']
         return data['adminlist']
 
-    def admin_make(self, gamertag):
+    def make_admin(self, gamertag: str) -> bool:
         """ Must whitelist the player first """
-        path = f'/services/{self.service_id}/gameservers/adminlist'
+        if not self.white_list_player(gamertag):
+            return False
+        path = f'/services/{self.service_id}/gameservers/games/adminlist'
         params = {'identifier': gamertag}
-        return self.__client.post(path=path, params=params)
+        response = Client.post(path=path, params=params)
+        data: dict = response.json()
+        return response.ok and data['status'] == 'success'
 
     def details(self) -> dict:
         path = f'/services/{self.service_id}/gameservers'
-        response = self.__client.get(path=path)
+        response = Client.get(path=path)
         data: dict = response.json()['data']
         return data['gameserver']
 
-    def restart(self, restart_message: str = None, log_message: str = None) -> bool:
-        path = f'/services/{self.service_id}/gameservers/restart'
-        params = {"restart_message": restart_message, "message": log_message}
-        response = self.__client.post(path=path, params=params)
+    def download_file(self, file_path) -> dict:
+        path = f'/services/{self.service_id}/gameservers/file_server/download'
+        params = {'file': file_path}
+        response = Client.get(path=path, params=params)
+        data: dict = response.json()['data']
+        return data
+
+    def rename_file(self, file_path, target_path, target_name) -> bool:
+        path = f'/services/{self.service_id}/gameservers/file_server/move'
+        params = {'source_path': file_path, 'target_path': target_path, 'target_filename': target_name}
+        response = Client.post(path=path, params=params)
+        data:dict = response.json()
+        return response.ok and data['status'] == 'success'
+
+    def start_game(self, game: str) -> bool:
+        path = f'/services/{self.service_id}/gameservers/games/start'
+        params = {'game': game}
+        response = Client.post(path=path, params=params)
         data: dict = response.json()
         return response.ok and data['status'] == 'success'
 
-    def stop(self, message=None, stop_message=None) -> bool:
+    def stop_game(self, message=None, stop_message=None) -> bool:
         path = f'/services/{self.service_id}/gameservers/stop'
         params = {'message': message, 'stop_message': stop_message}
-        response = self.__client.post(path=path, params=params)
+        response = Client.post(path=path, params=params)
+        data: dict = response.json()
+        return response.ok and data['status'] == 'success'
+
+    def restart_game(self, restart_message: str = None, log_message: str = None) -> bool:
+        path = f'/services/{self.service_id}/gameservers/restart'
+        params = {"restart_message": restart_message, "message": log_message}
+        response = Client.post(path=path, params=params)
+        data: dict = response.json()
+        return response.ok and data['status'] == 'success'
+
+    def install_game(self, game: str, modpack: str = None) -> bool:
+        path = f'/services/{self.service_id}/gameservers/games/install'
+        params = {'game': game, 'modpack': modpack}
+        response = Client.post(path=path, params=params)
+        data: dict = response.json()
+        return response.ok and data['status'] == 'success'
+
+    def uninstall_game(self, game: str) -> bool:
+        path = f'/services/{self.service_id}/gameservers/games/uninstall'
+        params = {'game': game}
+        response = Client.delete(path=path, params=params)
         data: dict = response.json()
         return response.ok and data['status'] == 'success'
 
     def backups_list(self) -> dict:
         path = f'/services/{self.service_id}/gameservers/backups'
-        response = self.__client.get(path=path)
+        response = Client.get(path=path)
         data: dict = response.json()['data']
         return data['backups']
 
     def command(self, command) -> bool:
         path = f'/services/{self.service_id}/gameservers/app_server/command'
         params = {'command': command}
-        response = self.__client.post(path=path, params=params)
+        response = Client.post(path=path, params=params)
         data: dict = response.json()
         return response.ok and data['status'] == 'success'
 
     def ping(self, command) -> bool:
         path = f'/services/{self.service_id}/gameservers/app_server'
-        response = self.__client.get(path=path, params={'command': command})
+        response = Client.get(path=path, params={'command': command})
         data: dict = response.json()
         return response.ok and data['status'] == 'success'
 
     def restore_database(self, database: str, timestamp: str) -> bool:
         path = f'/services/{self.service_id}/gameservers/backups/database'
         params = {'database': database, 'timestamp': timestamp}
-        response = self.__client.post(path=path, params=params)
+        response = Client.post(path=path, params=params)
         data: dict = response.json()
         return response.ok and data['status'] == 'success'
 
     def ftp_change_password(self, password: str) -> bool:
         path = f'/services/{self.service_id}/gameservers/ftp/password'
         params = {'password': password}
-        response = self.__client.post(path=path, params=params)
+        response = Client.post(path=path, params=params)
         data:dict = response.json()
         return response.ok and data['status'] == 'success'
 
     def bookmarks(self) -> list:
         path = f'/services/{self.service_id}/gameservers/file_server/bookmarks'
-        response = self.__client.get(path=path)
+        response = Client.get(path=path)
         data: dict = response.json()['data']
         return data['bookmarks']
 
     def file_copy(self, source_path: str, target_path: str, target_name: str) -> bool:
         path = f'/services/{self.service_id}/gameservers/file_server/copy'
         params = {'source_path': source_path, 'target_path': target_path, 'target_name': target_name}
-        response = self.__client.post(path=path, params=params)
+        response = Client.post(path=path, params=params)
         data: dict = response.json()
         return response.ok and data['status'] == 'success'
 
     def create_directory(self, dir_path, name) -> bool:
         path = f'/services/{self.service_id}/gameservers/file_server/mkdir'
         params = {'path': dir_path, 'name': name}
-        response = self.__client.post(path=path, params=params)
+        response = Client.post(path=path, params=params)
         data: dict = response.json()
         return response.ok and data['status'] == 'success'
 
     def file_delete(self, file_path) -> bool:
         path = f'/services/{self.service_id}/gameservers/file_server/delete'
         params = {'path': file_path}
-        response = self.__client.delete(path=path, params=params)
+        response = Client.delete(path=path, params=params)
         data: dict = response.json()
         return response.ok and data['status'] == 'success'
 
     def files_list(self, dir_path=None, search: str = None) -> list:
         path = f'/services/{self.service_id}/gameservers/file_server/list'
         params = {'dir': dir_path, 'search': search}
-        response = self.__client.get(path=path, params=params)
+        response = Client.get(path=path, params=params)
         data: dict = response.json()['data']
         return data['entries']
 
     def file_move(self, source_path: str, target_path: str) -> bool:
         path = f'/services/{self.service_id}/gameservers/file_server/move'
         name = source_path.split('/')[-1]
         params = {'source_path': source_path, 'target_path': target_path, 'target_file_name': name}
-        response = self.__client.post(path=path, params=params)
+        response = Client.post(path=path, params=params)
         data: dict = response.json()
         return response.ok and data['status'] == 'success'
 
     def file_seek(self, file_path: str, offset: int, length: int, mode: str = None) -> dict:
         path = f'/services/{self.service_id}/gameservers/file_server/seek'
         params = {'file': file_path, 'offset': offset, 'length': length, 'mode': mode}
-        response = self.__client.get(path=path, params=params)
+        response = Client.get(path=path, params=params)
         data: dict = response.json()['data']
         return data
 
     def file_size(self, file_path) -> int:
         path = f'/services/{self.service_id}/gameservers/file_server/size'
         params = {'file': file_path}
-        response = self.__client.get(path=path, params=params)
+        response = Client.get(path=path, params=params)
         data: dict = response.json()['data']
         return data['size']
 
-    def file_copy(self, source_path, target_path, target_name) -> bool:
-        path = f'/services/{self.service_id}/gameservers/file_server/copy'
-        params = {'source_path': source_path, 'target_path': target_path, 'target_name': target_name}
-        response = self.__client.post(path=path, params=params)
-        data: dict = response.json()
-        return response.ok and data['status'] == 'success'
-
     def files_stat(self, files_paths: list) -> list:
         path = f'/services/{self.service_id}/gameservers/file_server/stat'
         params = {'files': files_paths}
-        response = self.__client.get(path=path, params=params)
+        response = Client.get(path=path, params=params)
         data: dict = response.json()['data']
         return data['entries']
 
     def file_download(self, file_path) -> dict:
         path = f'/services/{self.service_id}/gameservers/file_server/download'
         params = {'file': file_path}
-        response = self.__client.get(path=path, params=params)
+        response = Client.get(path=path, params=params)
         data: dict = response.json()['data']
         return data
 
     def file_upload(self, target_dir: str, file_name: str) -> dict:
         path = f'/services/{self.service_id}/gameservers/file_server/upload'
         params = {'path': target_dir, 'file': file_name}
-        response = self.__client.post(path=path, params=params)
+        response = Client.post(path=path, params=params)
         data: dict = response.json()['data']
         return data
 
-    def full_game_list(self) -> dict:
-        path = '/gameserver/games'
-        response = self.__client.get(path=path)
-        data: dict = response.json()['data']
-        return data['games']
-
-    def install_game(self, game: str, modpack: str = None) -> bool:
-        path = f'/services/{self.service_id}/gameservers/games/install'
-        params = {'game': game, 'modpack': modpack}
-        response = self.__client.post(path=path, params=params)
-        data: dict = response.json()
-        return response.ok and data['status'] == 'success'
-
     def list_games(self) -> list:
         path = f'/services/{self.service_id}/gameservers/games'
-        response = self.__client.get(path=path)
+        response = Client.get(path=path)
         data: dict = response.json()['data']
         return data['games']
 
-    def start_game(self, game: str) -> bool:
-        path = f'/services/{self.service_id}/gameservers/games/start'
-        params = {'game': game}
-        response = self.__client.post(path=path, params=params)
-        data: dict = response.json()
-        return response.ok and data['status'] == 'success'
-
-    def uninstall_game(self, game: str) -> bool:
-        path = f'/services/{self.service_id}/gameservers/games/uninstall'
-        params = {'game': game}
-        response = self.__client.delete(path=path, params=params)
-        data: dict = response.json()
-        return response.ok and data['status'] == 'success'
-
     def change_mysql_password(self, password: str) -> bool:
         path = f'/services/{self.service_id}/gameservers/mysql/password'
         params = {'password': password}
-        response = self.__client.post(path=path, params=params)
+        response = Client.post(path=path, params=params)
         data: dict = response.json()
         return response.ok and data['status'] == 'success'
 
     def reset_mysql_database(self, password: str) -> bool:
         path = f'/services/{self.service_id}/gameservers/mysql/reset'
         params = {'password': password}
-        response = self.__client.post(path=path, params=params)
+        response = Client.post(path=path, params=params)
         data: dict = response.json()
         return response.ok and data['status'] == 'success'
 
     def package_install(self, package: str, version: str = None) -> dict:
         path = f'/services/{self.service_id}/gameservers/packages/install'
         params = {'package': package, 'version': version}
-        response = self.__client.post(path=path, params=params)
+        response = Client.post(path=path, params=params)
         data: dict = response.json()
         return data
 
     def packages_list(self) -> dict:
         path = f'/services/{self.service_id}/gameservers/packages'
-        response = self.__client.get(path=path)
+        response = Client.get(path=path)
         data: dict = response.json()
         return data['packages']
 
     def package_reinstall(self, package: str, version: str = None) -> dict:
         path = f'/services/{self.service_id}/gameservers/packages/reinstall'
         params = {'package': package, 'version': version}
-        response = self.__client.put(path=path, params=params)
+        response = Client.put(path=path, params=params)
         data: dict = response.json()
         return data
 
     def package_uninstall(self, package: str) -> dict:
         path = f'/services/{self.service_id}/gameservers/packages/uninstall'
         params = {'package': package}
-        response = self.__client.delete(path=path, params=params)
+        response = Client.delete(path=path, params=params)
         data: dict = response.json()
         return data
 
     def resource_usage(self, hours: int = None) -> dict:
         path = f'/services/{self.service_id}/gameservers/stats'
         params = {'hours': hours}
-        response = self.__client.get(path=path, params=params)
+        response = Client.get(path=path, params=params)
         data: dict = response.json()['data']
         return data['stats']
 
     def settings_sets_create(self, name: str = None) -> bool:
         path = f'/services/{self.service_id}/gameservers/settings/sets'
         params = {'name': name}
-        response = self.__client.post(path=path, params=params)
+        response = Client.post(path=path, params=params)
         data: dict = response.json()
         return response.ok and data['status'] == 'success'
 
     def settings_sets_delete(self, set_id: int) -> bool:
         path = f'/services/{self.service_id}/gameservers/settings/sets/{set_id}'
-        response = self.__client.delete(path=path)
+        response = Client.delete(path=path)
         data: dict = response.json()
         return response.ok and data['success'] == 'success'
 
     def settings_sets(self) -> list:
         path = f'/services/{self.service_id}/gameservers/settings/sets'
-        response = self.__client.get(path=path)
+        response = Client.get(path=path)
         data:dict = response.json()['data']
         return data['sets']
 
     def settings_sets_restore(self, set_id: int) -> bool:
         path = f'/services/{self.service_id}/gameservers/settings/sets/{set_id}/restore'
-        response = self.__client.post(path=path)
+        response = Client.post(path=path)
         data: dict = response.json()
         return response.ok and data['status'] == 'success'
 
     def default_settings(self) -> dict:
         path = f'/services/{self.service_id}/gameservers/settings/defaults'
-        response = self.__client.get(path=path)
+        response = Client.get(path=path)
         data: dict = response.json()['data']
-        return data
+        return data['settings']
 
     def reset_settings(self) -> bool:
         path = f'/services/{self.service_id}/gameservers/settings'
-        response = self.__client.delete(path=path)
+        response = Client.delete(path=path)
         data: dict = response.json()
         return response.ok and data['status'] == "success"
 
     def update_settings(self, category: str = None, key: str = None, value: str = None) -> dict:
         path = f'/services/{self.service_id}/gameservers/settings'
         params = {'category': category, 'key': key, 'value': value}
-        response = self.__client.post(path=path, params=params)
+        response = Client.post(path=path, params=params)
         data: dict = response.json()['data']
         return data['settings']
 
     def boost_history(self, page: int = 1) -> dict:
         path = f'/services/{self.service_id}/gameservers/boost/history'
         params = {'page': page}
-        response = self.__client.get(path=path, params=params)
+        response = Client.get(path=path, params=params)
         data: dict = response.json()['data']
         return data
 
     def boost_settings(self) -> dict:
         path = f'/services/{self.service_id}/gameservers/boost'
-        response = self.__client.get(path=path)
-        data: dict = response.json()
+        response = Client.get(path=path)
+        data: dict = response.json()['data']
         return data['boosting']
 
     def boost_settings_update(self, enable: bool = True, message: str = None, welcome_message: str = None) -> dict:
         path = f'/services/{self.service_id}/gameservers/boost'
         params = {'enable': enable, 'message': message, 'welcome_message': welcome_message}
-        response = self.__client.put(path=path, params=params)
-        data: dict = response.json()
+        response = Client.put(path=path, params=params)
+        data: dict = response.json()['data']
         return data['boosting']
 
-    def __contains__(self, item):
-        return item in self.__data
-
     def __getitem__(self, item):
-        return self.__data[item]
+        return self.__dict__[item]
 
     def keys(self):
-        return self.__data.keys()
-
-    def __iter__(self):
-        return iter(self.__data)
+        return self.__dict__.keys()
 
     def __repr__(self):
         service_id = f"service_id={repr(self.service_id)}"
-        location = f"location={repr(self.location)}"
+        status = f"status={repr(self.status)}"
         slots = f"slots={repr(self.slots)}"
+        memory_mb = f"memory_mb={repr(self.memory_mb)}"
         game_human = f"game_human={repr(self.game_human)}"
-        ip = f"ip={repr(self.ip)}"
-        params = ", ".join([service_id, location, slots, ip, game_human])
-        return f"<GameServer({params})>"
+        params = [s for s in [service_id, status, slots, memory_mb, game_human]]
+        return f"<{self.__class__.__name__}({', '.join(params)}, ...)>"
 
-    def __str__(self):
-        return json.dumps(self.__data, indent=3)
```

### Comparing `nitrado-1.0.6/src/nitrado.egg-info/PKG-INFO` & `nitrado-1.0.7/src/nitrado.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,46 @@
 Metadata-Version: 2.1
 Name: nitrado
-Version: 1.0.6
+Version: 1.0.7
 Summary: This application accesses the Nitrado API.
 Home-page: https://github.com/mjlomeli/NitradoAPI
 Author: Mauricio
 Author-email: dev.mauricio.lomeli@gmail.com
 Project-URL: Bug Tracker, https://github.com/mjlomeli/NitradoAPI/issues
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
 Platform: win32
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
 # Python Nitrado SDK
 
 [![Testing](https://github.com/mjlomeli/NitradoAPI/actions/workflows/tests.yml/badge.svg)](#) tests need a Nitrado subscription account 
 
 
 A Python based SDK for the [Nitrado RESTful API](https://doc.nitrado.net/) published at [PyPI](https://pypi.org/project/nitrado/).
 
+# Installation
+In your terminal install the nitrado package with pip.
+
+```shell
+pip install nitrado
+```
+
 
 # Overview
 
 To have access to this application you must have an account created at [Nitrado](https://server.nitrado.net/)
 and create an API key.
 
 # [Wiki - Full documentation](https://github.com/mjlomeli/NitradoAPI/wiki)
@@ -44,23 +52,14 @@
 #### 3. [Services](https://github.com/mjlomeli/NitradoAPI/wiki/Services)
    > Data provided outside of the game server. Like server status, user id, and auto extension plan.
 #### 4. [GameServer](https://github.com/mjlomeli/NitradoAPI/wiki/GameServer)
    > Data directly related to the game server. This includes the player list, game settings, etc.
 
 <br />
 
-# Installation
-In your terminal install the nitrado package with pip.
-
-```shell
-pip install nitrado
-```
-
-<br />
-
 # Examples
 
 ### Connect to Client
 To begin using the API the Client must first be connected to your Nitrado account.
 Once connected to the client, you should have access to any of the API calls.
 
 
@@ -74,15 +73,16 @@
 This example highlights how to get the service.
 
 ```python
 from nitrado import NitradoAPI
 
 api = NitradoAPI("your-api-key")
 
-api.services()
+services = api.services()
+print(services)
 ```
 ```python
 [
     <Service(id=1011111, status='active', type_human='Publicserver 10 slots', suspend_date='2023-05-07T01:21:11')>,
     <Service(id=1022222, status='active', type_human='Publicserver 20 slots', suspend_date='2023-07-07T02:11:01')>,
     <Service(id=1033333, status='active', type_human='Publicserver 30 slots', suspend_date='2023-09-07T06:51:41')>
 ]
@@ -92,15 +92,16 @@
 This example highlights how to get the gameserver.
 
 ```python
 from nitrado import NitradoAPI
 
 api = NitradoAPI("your-api-key")
 
-gameserver = api.game_servers()
+gameservers = api.game_servers()
+print(gameservers)
 ```
 ```python
 [
     <GameServer(service_id=11111111, location='US', slots=10, ip='1.2.3.4', game_human='ARK: Survival Evolved (Xbox One)')>,
     <GameServer(service_id=22222222, location='US', slots=70, ip='11.22.33.44', game_human='ARK: Survival Evolved (Xbox One)')>
 ]
 ```
```

### Comparing `nitrado-1.0.6/tests/test_game_server.py` & `nitrado-1.0.7/tests/test_game_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,12 @@
 from nitrado import GameServer
 from tests.mocked_client import MockedClient
 
 
-def get_client() -> MockedClient:
-    url = "https://api.nitrado.net/"
-    return MockedClient(url)
-
-
 def get_a_game_server() -> GameServer:
-    client = get_client()
     data = {
         "status": "started",
         "last_status_change": 1679636808,
         "must_be_started": True,
         "websocket_token": "415511975144cabef35bbf49eaf0e4b1157677d2",
         "hostsystems": {
             "linux": {
@@ -364,26 +358,18 @@
             "map": "TheIsland",
             "version": "959.4",
             "player_current": 0,
             "player_max": 20,
             "players": []
         }
     }
-    return GameServer(client, data)
+    return GameServer(**data)
 
 
 def test_game_server():
     game_server = get_a_game_server()
     assert game_server.service_id == 1
     assert game_server.status == 'started'
     assert game_server.user_id == 123456
     assert game_server.slots == 20
     assert game_server.query['server_name'] == '[US]- EPIX ARK -Isl1-20x/6Man/FRESHWIPE/MaxWild150/CusDrop?'
 
-
-def test_list_backups():
-    gameserver = get_a_game_server()
-    backups_json = gameserver.backups_list()
-    assert type(backups_json) == dict
-
-
-# TODO: add more test cases
```

### Comparing `nitrado-1.0.6/tests/test_service.py` & `nitrado-1.0.7/tests/test_service.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 from nitrado import Service
-from tests.mocked_client import MockedClient
+from tests.mocked_client import MockedClient as Client
 
 
-def get_client():
-    url = "https://api.nitrado.net/"
-    return MockedClient(url)
 
 
 def get_a_service():
-    client = get_client()
     data = {
         "id": 1,
         "location_id": 3,
         "status": "active",
         "websocket_token": "41e4b1157551195144ceaf0677d2",
         "user_id": 1234567,
         "comment": None,
@@ -37,44 +33,22 @@
         "deleting_in": 1371077,
         "username": "ni1234567_1",
         "roles": [
             "ROLE_OWNER"
         ]
     }
     try:
-        return Service(client, data)
+        return Service(**data)
     except Exception:
         raise Exception(f"Service could not be constructed with data: {data}")
 
 
 def test_services():
     services = get_a_service()
     assert services.id == 1
     assert services.type == "gameserver"
-    assert services.start_date == "2023-01-02T21:18:43"
-    assert services.suspend_date == "2023-04-03T05:21:17"
-    assert services.delete_date == "2023-04-10T05:21:17"
+    assert str(services.start_date) == "2023-01-02 21:18:43"
+    assert str(services.suspend_date) == "2023-04-03 05:21:17"
+    assert str(services.delete_date) == "2023-04-10 05:21:17"
     assert services.username == "ni1234567_1"
 
 
-def test_logs():
-    service = get_a_service()
-    logs = service.logs()
-    assert type(logs) == list
-    assert len(logs) == 40
-
-
-def test_tasks():
-    service = get_a_service()
-    tasks = service.tasks()
-    assert type(tasks) == list
-    assert tasks == [{'id': 8394912, 'status': 'error', 'minute': '5', 'hour': '3', 'day': '*', 'month': '*', 'weekday': '*', 'next_run': '2023-03-11T03:05:00', 'last_run': '2023-03-10T03:05:16', 'timezone': 'America/Los_Angeles', 'action_method': 'game_server_restart', 'action_data': None}]
-
-
-def test_notifications():
-    service = get_a_service()
-    notifications = service.notifications()
-    assert type(notifications) == list
-    assert notifications == []
-
-
-# TODO: Create more tests
```

