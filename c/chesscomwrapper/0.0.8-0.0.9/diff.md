# Comparing `tmp/chesscomwrapper-0.0.8.tar.gz` & `tmp/chesscomwrapper-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chesscomwrapper-0.0.8.tar", last modified: Sat Apr 22 17:26:33 2023, max compression
+gzip compressed data, was "chesscomwrapper-0.0.9.tar", last modified: Sun Apr 23 18:27:22 2023, max compression
```

## Comparing `chesscomwrapper-0.0.8.tar` & `chesscomwrapper-0.0.9.tar`

### file list

```diff
@@ -1,99 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:33.648776 chesscomwrapper-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-22 17:26:33.648776 chesscomwrapper-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:33.636775 chesscomwrapper-0.0.8/app/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:33.636775 chesscomwrapper-0.0.8/app/chesscomwrapper/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:33.640775 chesscomwrapper-0.0.8/app/chesscomwrapper/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/apimanager.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/chessclub.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/chesscountry.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/chessleaderboards.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/chessplayer.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/chessstreamer.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/chessteammatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/chesstournament.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/chesswrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/dailypuzzle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:33.640775 chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/chesscomhandler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:33.644775 chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/chesscomhandlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/chesscomhandlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/chesscomhandlers/archivehandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/chesscomhandlers/clubhandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/chesscomhandlers/countryhandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/chesscomhandlers/dailypuzzlehandler.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/chesscomhandlers/leaderboardshandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/chesscomhandlers/playerhandler.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/chesscomhandlers/roundhandler.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/chesscomhandlers/roundinfohandler.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/chesscomhandlers/streamerhandler.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/chesscomhandlers/teammatchboardhandler.py
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/chesscomhandlers/teammatchhandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/chesscomhandlers/tournamenthandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/errorhandler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:33.644775 chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/errorhandlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/errorhandlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/errorhandlers/noneerrorhandler.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/errorhandlers/raisererrorhandler.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/requesthandler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:33.644775 chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/requesthandlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/requesthandlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/requesthandlers/singletonrequesthandler.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/lazy_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:33.644775 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:33.644775 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/club/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/club/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/club/clubmember.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/club/clubprofile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:33.644775 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/country/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/country/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/country/countryinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:33.644775 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/leaderboards/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/leaderboards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/leaderboards/leaderboardsinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:33.644775 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/player/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/player/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/player/chessplayerprofile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/player/chessplayerstats.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/player/playerclub.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/player/playergames.py
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/player/playertournament.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/player/titledcategory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:33.644775 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/puzzle/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/puzzle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/puzzle/puzzleinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:33.644775 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/streamer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/streamer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/streamer/chessstreamerinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:33.648776 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/teammatch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/teammatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/teammatch/teammatchboardinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/teammatch/teammatchinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:33.648776 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/tournament/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/tournament/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/tournament/tournamentinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/tournament/tournamentplayer.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/tournament/tournamentroundgroupinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/tournament/tournamentroundplayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/tournament/tournamentsettings.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/tournament/tournamnetroundinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/playerarchive.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/teammatchboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/tournamentround.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/tournamentroundgroup.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:33.640775 chesscomwrapper-0.0.8/app/chesscomwrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-22 17:26:33.000000 chesscomwrapper-0.0.8/app/chesscomwrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-04-22 17:26:33.000000 chesscomwrapper-0.0.8/app/chesscomwrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 17:26:33.000000 chesscomwrapper-0.0.8/app/chesscomwrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-22 17:26:33.000000 chesscomwrapper-0.0.8/app/chesscomwrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-22 17:26:33.000000 chesscomwrapper-0.0.8/app/chesscomwrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 17:26:33.648776 chesscomwrapper-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:33.648776 chesscomwrapper-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    16478 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/tests/test_chesswrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:27:22.623250 chesscomwrapper-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-23 18:27:22.623250 chesscomwrapper-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:27:22.611250 chesscomwrapper-0.0.9/app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:27:22.611250 chesscomwrapper-0.0.9/app/chesscomwrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:27:22.615249 chesscomwrapper-0.0.9/app/chesscomwrapper/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/apimanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/chessclub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/chesscountry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/chessleaderboards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/chessplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/chessstreamer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/chessteammatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/chesstournament.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/chesswrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/dailypuzzle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:27:22.615249 chesscomwrapper-0.0.9/app/chesscomwrapper/src/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/handlers/chesscomhandler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:27:22.619250 chesscomwrapper-0.0.9/app/chesscomwrapper/src/handlers/chesscomhandlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/handlers/chesscomhandlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/handlers/chesscomhandlers/archivehandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/handlers/chesscomhandlers/clubhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/handlers/chesscomhandlers/countryhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/handlers/chesscomhandlers/dailypuzzlehandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/handlers/chesscomhandlers/leaderboardshandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/handlers/chesscomhandlers/playerhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/handlers/chesscomhandlers/roundhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/handlers/chesscomhandlers/roundinfohandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/handlers/chesscomhandlers/streamerhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/handlers/chesscomhandlers/teammatchboardhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/handlers/chesscomhandlers/teammatchhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/handlers/chesscomhandlers/tournamenthandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/handlers/errorhandler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:27:22.619250 chesscomwrapper-0.0.9/app/chesscomwrapper/src/handlers/errorhandlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/handlers/errorhandlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/handlers/errorhandlers/noneerrorhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/handlers/errorhandlers/raisererrorhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/handlers/requesthandler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:27:22.619250 chesscomwrapper-0.0.9/app/chesscomwrapper/src/handlers/requesthandlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/handlers/requesthandlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/handlers/requesthandlers/singletonrequesthandler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:27:22.619250 chesscomwrapper-0.0.9/app/chesscomwrapper/src/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:27:22.619250 chesscomwrapper-0.0.9/app/chesscomwrapper/src/models/club/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/models/club/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/models/club/clubmember.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/models/club/clubprofile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:27:22.619250 chesscomwrapper-0.0.9/app/chesscomwrapper/src/models/country/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/models/country/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/models/country/countryinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:27:22.619250 chesscomwrapper-0.0.9/app/chesscomwrapper/src/models/leaderboards/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/models/leaderboards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/models/leaderboards/leaderboardsinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:27:22.619250 chesscomwrapper-0.0.9/app/chesscomwrapper/src/models/player/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/models/player/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/models/player/chessplayerprofile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/models/player/chessplayerstats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/models/player/playerclub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/models/player/playergames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/models/player/playertournament.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/models/player/titledcategory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:27:22.619250 chesscomwrapper-0.0.9/app/chesscomwrapper/src/models/puzzle/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/models/puzzle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/models/puzzle/puzzleinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:27:22.619250 chesscomwrapper-0.0.9/app/chesscomwrapper/src/models/streamer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/models/streamer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/models/streamer/chessstreamerinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:27:22.623250 chesscomwrapper-0.0.9/app/chesscomwrapper/src/models/teammatch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/models/teammatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/models/teammatch/teammatchboardinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/models/teammatch/teammatchinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:27:22.623250 chesscomwrapper-0.0.9/app/chesscomwrapper/src/models/tournament/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/models/tournament/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/models/tournament/tournamentinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/models/tournament/tournamentplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/models/tournament/tournamentroundgroupinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/models/tournament/tournamentroundplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/models/tournament/tournamentsettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/models/tournament/tournamnetroundinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/playerarchive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/teammatchboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/tournamentround.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/src/tournamentroundgroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/app/chesscomwrapper/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:27:22.615249 chesscomwrapper-0.0.9/app/chesscomwrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-23 18:27:22.000000 chesscomwrapper-0.0.9/app/chesscomwrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-04-23 18:27:22.000000 chesscomwrapper-0.0.9/app/chesscomwrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 18:27:22.000000 chesscomwrapper-0.0.9/app/chesscomwrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-23 18:27:22.000000 chesscomwrapper-0.0.9/app/chesscomwrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-23 18:27:22.000000 chesscomwrapper-0.0.9/app/chesscomwrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 18:27:22.623250 chesscomwrapper-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:27:22.623250 chesscomwrapper-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    16106 2023-04-23 18:27:11.000000 chesscomwrapper-0.0.9/tests/test_chesswrapper.py
```

### Comparing `chesscomwrapper-0.0.8/LICENSE.txt` & `chesscomwrapper-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.8/app/chesscomwrapper/src/apimanager.py` & `chesscomwrapper-0.0.9/app/chesscomwrapper/src/apimanager.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.8/app/chesscomwrapper/src/chessclub.py` & `chesscomwrapper-0.0.9/app/chesscomwrapper/src/chessclub.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.8/app/chesscomwrapper/src/chesscountry.py` & `chesscomwrapper-0.0.9/app/chesscomwrapper/src/chesscountry.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Optional
+from .chessclub import Club
 from .handlers.chesscomhandlers.countryhandler import CountryHandler
 import functools
 
 
 class ChessCountry(object):
     def __init__(self, abbr, lazy = True) -> None:
         self.code = abbr
@@ -24,9 +26,9 @@
     
     def _getInfo(self) -> None:
         return CountryHandler().getInfo(self.code)
 
     def _getPlayers(self) -> None:
         return CountryHandler().getPlayers(self.code)
     
-    def _getClubs(self) -> None:
+    def _getClubs(self) -> Optional[list[Club]]:
         return CountryHandler().getClubs(self.code)
```

### Comparing `chesscomwrapper-0.0.8/app/chesscomwrapper/src/chessplayer.py` & `chesscomwrapper-0.0.9/app/chesscomwrapper/src/chessplayer.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.8/app/chesscomwrapper/src/chesswrapper.py` & `chesscomwrapper-0.0.9/app/chesscomwrapper/src/chesswrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from .chessplayer import ChessPlayer 
 from .chesstournament import Tournament
 from .chessteammatch import TeamMatch
 from .chesscountry import ChessCountry
 from .dailypuzzle import PuzzleFactory
 
 from .chessleaderboards import ChessLeaderboards
-class ChessWrapper(object):
+class ChesscomWrapper(object):
   """A class to wrap the chess.com API"""
   
   def __init__(self):
     pass
```

### Comparing `chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/chesscomhandler.py` & `chesscomwrapper-0.0.9/app/chesscomwrapper/src/handlers/chesscomhandler.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/chesscomhandlers/archivehandler.py` & `chesscomwrapper-0.0.9/app/chesscomwrapper/src/handlers/chesscomhandlers/archivehandler.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/chesscomhandlers/clubhandler.py` & `chesscomwrapper-0.0.9/app/chesscomwrapper/src/handlers/chesscomhandlers/clubhandler.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/chesscomhandlers/countryhandler.py` & `chesscomwrapper-0.0.9/app/chesscomwrapper/src/handlers/chesscomhandlers/countryhandler.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/chesscomhandlers/dailypuzzlehandler.py` & `chesscomwrapper-0.0.9/app/chesscomwrapper/src/handlers/chesscomhandlers/dailypuzzlehandler.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/chesscomhandlers/leaderboardshandler.py` & `chesscomwrapper-0.0.9/app/chesscomwrapper/src/handlers/chesscomhandlers/leaderboardshandler.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/chesscomhandlers/playerhandler.py` & `chesscomwrapper-0.0.9/app/chesscomwrapper/src/handlers/chesscomhandlers/playerhandler.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/chesscomhandlers/roundhandler.py` & `chesscomwrapper-0.0.9/app/chesscomwrapper/src/handlers/chesscomhandlers/roundhandler.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/chesscomhandlers/roundinfohandler.py` & `chesscomwrapper-0.0.9/app/chesscomwrapper/src/handlers/chesscomhandlers/roundinfohandler.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/chesscomhandlers/streamerhandler.py` & `chesscomwrapper-0.0.9/app/chesscomwrapper/src/handlers/chesscomhandlers/streamerhandler.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/chesscomhandlers/teammatchboardhandler.py` & `chesscomwrapper-0.0.9/app/chesscomwrapper/src/handlers/chesscomhandlers/teammatchboardhandler.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/chesscomhandlers/teammatchhandler.py` & `chesscomwrapper-0.0.9/app/chesscomwrapper/src/handlers/chesscomhandlers/teammatchhandler.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/chesscomhandlers/tournamenthandler.py` & `chesscomwrapper-0.0.9/app/chesscomwrapper/src/handlers/chesscomhandlers/tournamenthandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Optional
 from ...models.tournament.tournamnetroundinfo import TournamentRoundInfo
 from ...apimanager import API
 from ..chesscomhandler import ChesscomHandler
 from ..errorhandlers.noneerrorhandler import NoneErrorHandler
 from ..requesthandlers.singletonrequesthandler import SingletonRequestHandler
 from ...models.tournament.tournamentinfo import TournamentInfo
 
@@ -11,15 +12,15 @@
     def __init__(self):
         """Initializes a ArchiveHandler object"""
         self.errorHandler = NoneErrorHandler()
         self.requestHandler = SingletonRequestHandler()
         pass
 
     
-    def getInfo(self, tournamentId):
+    def getInfo(self, tournamentId) -> Optional[TournamentInfo]:
         """Returns player's monthly archives"""
         response = self.doRequest(tournamentId)
         if response is None:
             return None
         info = TournamentInfo(response.json())
         return info
```

### Comparing `chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/errorhandler.py` & `chesscomwrapper-0.0.9/app/chesscomwrapper/src/handlers/errorhandler.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/requesthandlers/singletonrequesthandler.py` & `chesscomwrapper-0.0.9/app/chesscomwrapper/src/handlers/requesthandlers/singletonrequesthandler.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/club/clubprofile.py` & `chesscomwrapper-0.0.9/app/chesscomwrapper/src/models/club/clubprofile.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/leaderboards/leaderboardsinfo.py` & `chesscomwrapper-0.0.9/app/chesscomwrapper/src/models/leaderboards/leaderboardsinfo.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/player/chessplayerprofile.py` & `chesscomwrapper-0.0.9/app/chesscomwrapper/src/models/player/chessplayerprofile.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/player/chessplayerstats.py` & `chesscomwrapper-0.0.9/app/chesscomwrapper/src/models/player/chessplayerstats.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/player/playergames.py` & `chesscomwrapper-0.0.9/app/chesscomwrapper/src/models/player/playergames.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/player/playertournament.py` & `chesscomwrapper-0.0.9/app/chesscomwrapper/src/models/player/playertournament.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/teammatch/teammatchinfo.py` & `chesscomwrapper-0.0.9/app/chesscomwrapper/src/models/teammatch/teammatchinfo.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/tournament/tournamentinfo.py` & `chesscomwrapper-0.0.9/app/chesscomwrapper/src/models/tournament/tournamentinfo.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/tournament/tournamentsettings.py` & `chesscomwrapper-0.0.9/app/chesscomwrapper/src/models/tournament/tournamentsettings.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.8/app/chesscomwrapper/src/playerarchive.py` & `chesscomwrapper-0.0.9/app/chesscomwrapper/src/playerarchive.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.8/app/chesscomwrapper.egg-info/SOURCES.txt` & `chesscomwrapper-0.0.9/app/chesscomwrapper.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 app/chesscomwrapper/src/chessleaderboards.py
 app/chesscomwrapper/src/chessplayer.py
 app/chesscomwrapper/src/chessstreamer.py
 app/chesscomwrapper/src/chessteammatch.py
 app/chesscomwrapper/src/chesstournament.py
 app/chesscomwrapper/src/chesswrapper.py
 app/chesscomwrapper/src/dailypuzzle.py
-app/chesscomwrapper/src/lazy_decorator.py
 app/chesscomwrapper/src/playerarchive.py
 app/chesscomwrapper/src/teammatchboard.py
 app/chesscomwrapper/src/tournamentround.py
 app/chesscomwrapper/src/tournamentroundgroup.py
 app/chesscomwrapper/src/handlers/__init__.py
 app/chesscomwrapper/src/handlers/chesscomhandler.py
 app/chesscomwrapper/src/handlers/errorhandler.py
```

### Comparing `chesscomwrapper-0.0.8/setup.py` & `chesscomwrapper-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.8/tests/test_chesswrapper.py` & `chesscomwrapper-0.0.9/tests/test_chesswrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,24 +37,24 @@
 from app.chesscomwrapper.src.models.leaderboards.leaderboardsinfo import LeaderboardsInfo
 
 
 class PlayerTest(unittest.TestCase):
     def test_player_profile(self):
         """Tests an API call to get a player's info"""
 
-        chess_instance = chesswrapper.ChessWrapper()
+        chess_instance = chesswrapper.ChesscomWrapper()
         player = chess_instance.getPlayer("nicolapanozzo")
 
         "Player should be a ChessPlayer object"
         assert isinstance(player.profile, ChessPlayerProfile ), "Player should be a ChessPlayer object"
         assert player.profile.name == "Nicola Panozzo", "Username should be Nicola Panozzo, not {}".format(player.profile.name)
     
     def test_rate_limit(self):
         """Tests the rate limit"""
-        chess_instance = chesswrapper.ChessWrapper()
+        chess_instance = chesswrapper.ChesscomWrapper()
         player = chess_instance.getPlayer("nicolapanozzo")
         
         
         threadPool = []
         for i in range(0, 100):
             playert = chess_instance.getPlayer("nicolapanozzo{}".format(i*random.randint(1,1000)))
             threadPool.append(threading.Thread(target=playert.profile))
@@ -66,244 +66,235 @@
             thread.join()
 
         assert threadPool[60].is_alive() == False, "Thread should be dead"
 
     def test_player_stats(self):
         """Tests an API call to get a player's stats"""
 
-        chess_instance = chesswrapper.ChessWrapper()
+        chess_instance = chesswrapper.ChesscomWrapper()
         player = chess_instance.getPlayer("nicolapanozzo")
 
         "Player.stats should be a ChessPlayerStats object"
         assert isinstance(player.stats, ChessPlayerStats ), "Player should be a ChessPlayer object"
         assert player.stats.tactics.highest.rating == 2593, "Games should be 2539, not {}".format(player.stats.tactics.highest.rating)
     
     def test_player_games(self):
         """Tests an API call to get a player's games"""
 
-        chess_instance = chesswrapper.ChessWrapper()
+        chess_instance = chesswrapper.ChesscomWrapper()
         player = chess_instance.getPlayer("erik")
         
         "Player.games should be a list of ChesscomGame objects"
         assert isinstance(player.games[0], ChesscomGame), "Game[0] should be a ChesscomGame object"
         assert player.games[0].black == "erik", "Game result should be *, not {}".format(player.games[0].black)
 
     def test_player_games_to_move(self):
         """Tests an API call to get a player's games"""
 
-        chess_instance = chesswrapper.ChessWrapper()
+        chess_instance = chesswrapper.ChesscomWrapper()
         player = chess_instance.getPlayer("erik")
 
         "Player.games should be a list of ChesscomGame objects"
         assert isinstance(player.gamesToMove[0], ChesscomGameToMove),  "Game[0] should be a ChesscomGame object"
         assert len(player.gamesToMove) == 2
 
     def test_player_archives(self):
         """Tests an API call to get a player's archives"""
 
-        chess_instance = chesswrapper.ChessWrapper()
+        chess_instance = chesswrapper.ChesscomWrapper()
         player = chess_instance.getPlayer("erik")
 
         "Player.archives should be a list of ChesscomGame objects"
         assert isinstance(player.archives[0], PlayerArchive),  "Game[0] should be a ChesscomGame object"
         assert len(player.archives) == 190 , "Archives should be 189, not {}".format(len(player.archives))
 
     def test_player_archived_games(self):
         """Tests an API call to get a player's archives"""
 
-        chess_instance = chesswrapper.ChessWrapper()
+        chess_instance = chesswrapper.ChesscomWrapper()
         player = chess_instance.getPlayer("erik")
         "Player.archives should be a list of ChesscomGame objects"
         assert isinstance(player.archives[0].games[0], ChesscomGameArchived),  "Archive.games should be a list(ChesscomGame) object"
         assert player.archives[0].games[0].rated == True , "In the first game of the first archive should be rated == True, not {}".format(player.archives[0].games[0].rated)
     
     def test_player_clubs(self):
         """Tests an API call to get a player's clubs"""
 
-        chess_instance = chesswrapper.ChessWrapper()
+        chess_instance = chesswrapper.ChesscomWrapper()
         player = chess_instance.getPlayer("nicolapanozzo")
         "Player.archives should be a list of ChesscomGame objects"
         assert isinstance(player.clubs[1], PlayerClub),  "Archive.games should be a list(ChesscomGame) object"
         assert player.clubs[1].name == "Bonobo" , "In the first game of the first archive should be rated == True, not {}".format(player.archives[0].games[0].rated)
 
     def test_player_tournaments(self):
         """Tests an API call to get a player's tournaments"""
 
-        chess_instance = chesswrapper.ChessWrapper()
+        chess_instance = chesswrapper.ChesscomWrapper()
         player = chess_instance.getPlayer("nicolapanozzo")
         player.tournaments
         "Player.archives should be a list of ChesscomGame objects"
         assert isinstance(player.tournaments, PlayerTournaments),  "player.tournaments should be a PlayerTournaments object"
         assert len(player.tournaments.finished) == 1 , "the number of finished tournaments should be 1, not {}".format(len(player.tournaments.finished))
 
     def test_titled_players(self):
         """Tests an API call to get all the titled players"""
 
-        chess_instance = chesswrapper.ChessWrapper()
+        chess_instance = chesswrapper.ChesscomWrapper()
         titled_players = chess_instance.getTitledPlayers(chesswrapper.TitledCategory.GM)
         "Player.archives should be a list of ChesscomGame objects"
         assert isinstance(titled_players[0], ChessPlayer),  "Archive.games should be a list(ChesscomGame) object"
         # assert titled_players[0].name == "Magnus Carlsen" , "In the first game of the first archive should be rated == True, not {}".format(player.archives[0].games[0].rated)
 
 class ClubTest(unittest.TestCase):
     def test_club_info(self):
         """Tests an API call to get a club's info"""
 
-        chess_instance = chesswrapper.ChessWrapper()
+        chess_instance = chesswrapper.ChesscomWrapper()
         club = chess_instance.getClub("bonobo")
         "Club.info should be a ClubInfo object"
         assert isinstance(club.profile, ClubProfile),  "Club.info should be a ClubInfo object"
         assert club.profile.name == "Bonobo" , "Club name should be Bonobo, not {}".format(club.profile.name)
         assert club.profile.average_daily_rating == 793, "Club average_daily_rating should be 794, not {}".format(club.profile.average_daily_rating)
 
     def test_club_members(self):
         """Tests an API call to get a club's members"""
 
-        chess_instance = chesswrapper.ChessWrapper()
+        chess_instance = chesswrapper.ChesscomWrapper()
         club = chess_instance.getClub("bonobo")
 
         "Club.members should be a list of ChessPlayer objects"
         assert isinstance(club.members[0].player, ChessPlayer),  "Club.members should be a list of ChessPlayer objects"
         assert club.members[0].player.username == "capitanoorsoblu" , "Club member should be capitanoorsoblu, not {}".format(club.members[0].player.username)
 
 
 
 class TournamentTest(unittest.TestCase):
     def test_tournament_info(self):
         """Tests an API call to get a tournament's info"""
 
-        chess_instance = chesswrapper.ChessWrapper()
+        chess_instance = chesswrapper.ChesscomWrapper()
         tournament = chess_instance.getTournament("https://api.chess.com/pub/tournament/-33rd-chesscom-quick-knockouts-1401-1600")
-        tournament.getInfo()
+        print(tournament.info)
         "Club.info should be a ClubInfo object"
         assert isinstance(tournament.info, TournamentInfo),  "Tournament.info should be a TournamentInfo object"
         assert tournament.info.creator == "Patzer24" , "Tournament creator should be Patzer24, not {}".format(tournament.info.creator)
         assert len(tournament.info.players) == 399, "Tournament parecipants numeber should be 399, not {}".format(len(tournament.info.players))
 
     def test_tournament_round_info(self):
         # """Tests an API call to get a tournament's round info"""
-        chess_instance = chesswrapper.ChessWrapper()
+        chess_instance = chesswrapper.ChesscomWrapper()
         tournament = chess_instance.getTournament("https://api.chess.com/pub/tournament/-33rd-chesscom-quick-knockouts-1401-1600")
-        tournament.getInfo()
+
         print(tournament.info.rounds)
-        tournament.info.rounds[0].getInfo()
+
         print(tournament.info.rounds[0].info)
         assert isinstance(tournament.info.rounds[0].info, TournamentRoundInfo),  "Round.info should be a TournamentRoundInfo object"
         assert len(tournament.info.rounds[0].info.groups) == 67, "Tournament groups number should be 67, not {}".format(len(tournament.info.rounds[0].info.groups))
         
 
 
     def test_tournament_round_group(self):
         # """Tests an API call to get a tournament's round group info"""
-        chess_instance = chesswrapper.ChessWrapper()
+        chess_instance = chesswrapper.ChesscomWrapper()
         tournament = chess_instance.getTournament("https://api.chess.com/pub/tournament/-33rd-chesscom-quick-knockouts-1401-1600")
-        tournament.getInfo()
-        print(tournament.info.rounds)
-        tournament.info.rounds[0].getInfo()
-        # print(tournament.info.rounds[0].info.groupsUrls)
-        tournament.info.rounds[0].info.groups[0].getInfo()
-        
+
+        print(tournament.info)
 
         assert isinstance(tournament.info.rounds[0].info, TournamentRoundInfo),  "Round.info should be a TournamentRoundInfo object"
         assert isinstance(tournament.info.rounds[0].info.groups[0], TournamentRoundGroup),  "Round.info.groups[0] should be a TournamentRoundGroup object"
         assert isinstance(tournament.info.rounds[0].info.groups[0].info, TournamentRoundGroupInfo),  "Round.info.groups[0].info should be a TournamentRoundGroupInfo object"
         assert tournament.info.rounds[0].info.groups[0].info.games[0].white.username == "Rockaround" , "The first player with white in the first game of the first group of the first round Rockaround, not {}".format(tournament.info.rounds[0].info.groups[0].info.games[0].white.username)
 
 class TeamMatchTest(unittest.TestCase):
     def test_team_match_info(self):
         """Tests an API call to get a team match's info"""
 
-        chess_instance = chesswrapper.ChessWrapper()
+        chess_instance = chesswrapper.ChesscomWrapper()
         team_match = chess_instance.getTeamMatch("https://api.chess.com/pub/match/53")
-        team_match.getInfo()
         "TeamMatch.info should be a TeamMatchInfo object"
         assert isinstance(team_match.info, TeamMatchInfo),  "TeamMatch.info should be a TeamMatchInfo object"
         assert team_match.info.teams.team1.name == "International Flagbearers" , "TeamMatch team1 should be International Flagbearers, not {}".format(team_match.info.teams.team1.name)
         assert team_match.info.teams.team2.name == "Team Italia" , "TeamMatch team2 should be Team Italia, not {}".format(team_match.info.teams.team2.name)
     
     def test_team_match_board_info(self):
         """Tests an API call to get a team match's info"""
 
-        chess_instance = chesswrapper.ChessWrapper()
+        chess_instance = chesswrapper.ChesscomWrapper()
         team_match = chess_instance.getTeamMatch("https://api.chess.com/pub/match/53")
-        team_match.getInfo()
-        team_match.info.boards[0].getInfo()
         
         assert isinstance(team_match.info.boards[0].info, TeamMatchBoardInfo),  "TeamMatch.info.boards[0].info should be a TeamMatchBoardInfo object"
         assert team_match.info.boards[0].info.board_scores.result == "0.5-1.5" , "The result should be 0.5-1.5, not {}".format(team_match.info.boards[0].info.board_scores.result)
 
 class CountryTest(unittest.TestCase):
     def test_country_info(self):
         """Tests an API call to get a country's info"""
 
-        chess_instance = chesswrapper.ChessWrapper()
+        chess_instance = chesswrapper.ChesscomWrapper()
         country = chess_instance.getCountry("IT")
         
         "Country.info should be a CountryInfo object"
         assert isinstance(country.info, CountryInfo),  "Country.info should be a CountryInfo object"
         assert country.info.name == "Italy" , "Country name should be Italy, not {}".format(country.info.name)
     
     def test_country_players(self):
         """Tests an API call to get a country's players"""
 
-        chess_instance = chesswrapper.ChessWrapper()
+        chess_instance = chesswrapper.ChesscomWrapper()
         country = chess_instance.getCountry("IT")
         country._getPlayers()
 
         "Country.players should be a list of ChessPlayer objects"
         assert isinstance(country.players[0], ChessPlayer),  "Country.players should be a list of ChessPlayer objects"
         assert country.players[0].username == "--hugo--" , "Country player should be --hugo--, not {}".format(country.players[0].username)
 
     def test_country_clubs(self):
         """Tests an API call to get a country's players"""
 
-        chess_instance = chesswrapper.ChessWrapper()
+        chess_instance = chesswrapper.ChesscomWrapper()
         country = chess_instance.getCountry("IT")
-        country._getClubs()
-        country.clubs[0]._getProfile()
 
         print(country.clubs[0].profile.name)
         "Country.players should be a list of ChessPlayer objects"
         assert isinstance(country.clubs[0], Club),  "country.clubs[0] should be a Club"
         assert country.clubs[0].id == "italys-finest" , "Country club id should be italys-finest, not {}".format(country.clubs[0].id)
 
 class PuzzleTest(unittest.TestCase):
     def test_daily_puzzle(self):
         """Tests an API call to get a puzzle's info"""
 
-        chess_instance = chesswrapper.ChessWrapper()
+        chess_instance = chesswrapper.ChesscomWrapper()
         puzzle = chess_instance.getDailyPuzzle()
         "Puzzle.info should be a PuzzleInfo object"
         assert isinstance(puzzle.info, PuzzleInfo),  "Puzzle.info should be a PuzzleInfo object"
         assert puzzle.info.title == "Loose Piece Yo-Yo" , "Puzzle id should be 'Loose Piece Yo-Yo', not {}".format(puzzle.info.title)
 
     def test_random_puzzle(self):
         """Tests an API call to get a puzzle's info"""
 
-        chess_instance = chesswrapper.ChessWrapper()
+        chess_instance = chesswrapper.ChesscomWrapper()
         puzzle = chess_instance.getRandomPuzzle()
         print(puzzle.info.title)
         "Puzzle.info should be a PuzzleInfo object"
         assert isinstance(puzzle.info, PuzzleInfo),  "Puzzle.info should be a PuzzleInfo object"
         # assert puzzle.info.title == "Loose Piece Yo-Yo" , "Puzzle id should be 'Loose Piece Yo-Yo', not {}".format(puzzle.info.title)
 
 class StreamerTest(unittest.TestCase):
     def test_streamers(self):
         """Tests an API call to get streamers' info"""
 
-        chess_instance = chesswrapper.ChessWrapper()
+        chess_instance = chesswrapper.ChesscomWrapper()
         streamers = chess_instance.getStreamersInfo()
         print(streamers[0].username)
         "Streamers should be a list of Streamer objects"
         assert isinstance(streamers[0], ChessStreamerInfo),  "Streamers should be a list of ChessStreamerInfo objects"
         assert streamers[0].username == "LileKoridze" , "Streamer should be lularobs, not {}".format(streamers[0].username)
 
 class LeaderboardsTest(unittest.TestCase):
     def test_leaderboard(self):
         """Tests an API call to get a leaderboard's info"""
             
-        chess_instance = chesswrapper.ChessWrapper()
+        chess_instance = chesswrapper.ChesscomWrapper()
         leaderboards = chess_instance.getLeaderboards()
         
         "Leaderboard.info should be a LeaderboardInfo object"
         assert isinstance(leaderboards, LeaderboardsInfo),  "Leaderboard.info should be a LeaderboardInfo object"
         assert leaderboards.daily[0].rank == 1 , "Leaderboard rank of first player should be 1, not {}".format(leaderboards.info.daily[0].rank)
```

