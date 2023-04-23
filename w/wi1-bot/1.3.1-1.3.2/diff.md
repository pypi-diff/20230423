# Comparing `tmp/wi1-bot-1.3.1.tar.gz` & `tmp/wi1-bot-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wi1-bot-1.3.1.tar", last modified: Mon Apr  3 04:57:40 2023, max compression
+gzip compressed data, was "wi1-bot-1.3.2.tar", last modified: Sun Apr 23 07:42:26 2023, max compression
```

## Comparing `wi1-bot-1.3.1.tar` & `wi1-bot-1.3.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 04:57:40.677039 wi1-bot-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-03 04:57:28.000000 wi1-bot-1.3.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 04:57:40.673039 wi1-bot-1.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 04:57:40.677039 wi1-bot-1.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-03 04:57:28.000000 wi1-bot-1.3.1/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-03 04:57:28.000000 wi1-bot-1.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-03 04:57:28.000000 wi1-bot-1.3.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-03 04:57:28.000000 wi1-bot-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-04-03 04:57:40.677039 wi1-bot-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-04-03 04:57:28.000000 wi1-bot-1.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-03 04:57:28.000000 wi1-bot-1.3.1/config.yaml.template
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-03 04:57:28.000000 wi1-bot-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 04:57:40.677039 wi1-bot-1.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 04:57:40.677039 wi1-bot-1.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-03 04:57:28.000000 wi1-bot-1.3.1/tests/movie_downloaded.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 04:57:40.677039 wi1-bot-1.3.1/wi1_bot/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-03 04:57:28.000000 wi1-bot-1.3.1/wi1_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-03 04:57:39.000000 wi1-bot-1.3.1/wi1_bot/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 04:57:40.677039 wi1-bot-1.3.1/wi1_bot/arr/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-03 04:57:28.000000 wi1-bot-1.3.1/wi1_bot/arr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-03 04:57:28.000000 wi1-bot-1.3.1/wi1_bot/arr/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-03 04:57:28.000000 wi1-bot-1.3.1/wi1_bot/arr/episode.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-03 04:57:28.000000 wi1-bot-1.3.1/wi1_bot/arr/movie.py
--rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-04-03 04:57:28.000000 wi1-bot-1.3.1/wi1_bot/arr/radarr.py
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-04-03 04:57:28.000000 wi1-bot-1.3.1/wi1_bot/arr/sonarr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-03 04:57:28.000000 wi1-bot-1.3.1/wi1_bot/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 04:57:40.677039 wi1-bot-1.3.1/wi1_bot/discord/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 04:57:28.000000 wi1-bot-1.3.1/wi1_bot/discord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-04-03 04:57:28.000000 wi1-bot-1.3.1/wi1_bot/discord/bot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 04:57:40.677039 wi1-bot-1.3.1/wi1_bot/discord/cogs/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-03 04:57:28.000000 wi1-bot-1.3.1/wi1_bot/discord/cogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-04-03 04:57:28.000000 wi1-bot-1.3.1/wi1_bot/discord/cogs/movie.py
--rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-04-03 04:57:28.000000 wi1-bot-1.3.1/wi1_bot/discord/cogs/series.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-03 04:57:28.000000 wi1-bot-1.3.1/wi1_bot/discord/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-03 04:57:28.000000 wi1-bot-1.3.1/wi1_bot/push.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 04:57:40.677039 wi1-bot-1.3.1/wi1_bot/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 04:57:28.000000 wi1-bot-1.3.1/wi1_bot/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-04-03 04:57:28.000000 wi1-bot-1.3.1/wi1_bot/scripts/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-03 04:57:28.000000 wi1-bot-1.3.1/wi1_bot/scripts/transcode_item.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 04:57:40.677039 wi1-bot-1.3.1/wi1_bot/transcoder/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-03 04:57:28.000000 wi1-bot-1.3.1/wi1_bot/transcoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-03 04:57:28.000000 wi1-bot-1.3.1/wi1_bot/transcoder/transcode_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-04-03 04:57:28.000000 wi1-bot-1.3.1/wi1_bot/transcoder/transcoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-04-03 04:57:28.000000 wi1-bot-1.3.1/wi1_bot/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 04:57:40.677039 wi1-bot-1.3.1/wi1_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-04-03 04:57:40.000000 wi1-bot-1.3.1/wi1_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-03 04:57:40.000000 wi1-bot-1.3.1/wi1_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 04:57:40.000000 wi1-bot-1.3.1/wi1_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-03 04:57:40.000000 wi1-bot-1.3.1/wi1_bot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-03 04:57:40.000000 wi1-bot-1.3.1/wi1_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-03 04:57:40.000000 wi1-bot-1.3.1/wi1_bot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 07:42:26.139047 wi1-bot-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 07:42:26.135047 wi1-bot-1.3.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 07:42:26.139047 wi1-bot-1.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-04-23 07:42:26.139047 wi1-bot-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/config.yaml.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 07:42:26.143047 wi1-bot-1.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 07:42:26.139047 wi1-bot-1.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/tests/movie_downloaded.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 07:42:26.139047 wi1-bot-1.3.2/wi1_bot/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/wi1_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-23 07:42:25.000000 wi1-bot-1.3.2/wi1_bot/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 07:42:26.139047 wi1-bot-1.3.2/wi1_bot/arr/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/wi1_bot/arr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/wi1_bot/arr/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/wi1_bot/arr/episode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/wi1_bot/arr/movie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/wi1_bot/arr/radarr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/wi1_bot/arr/sonarr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/wi1_bot/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 07:42:26.139047 wi1-bot-1.3.2/wi1_bot/discord/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/wi1_bot/discord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/wi1_bot/discord/bot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 07:42:26.139047 wi1-bot-1.3.2/wi1_bot/discord/cogs/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/wi1_bot/discord/cogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/wi1_bot/discord/cogs/movie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/wi1_bot/discord/cogs/series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/wi1_bot/discord/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/wi1_bot/push.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 07:42:26.139047 wi1-bot-1.3.2/wi1_bot/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/wi1_bot/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/wi1_bot/scripts/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/wi1_bot/scripts/transcode_item.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 07:42:26.139047 wi1-bot-1.3.2/wi1_bot/transcoder/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/wi1_bot/transcoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/wi1_bot/transcoder/transcode_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/wi1_bot/transcoder/transcoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-04-23 07:42:12.000000 wi1-bot-1.3.2/wi1_bot/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 07:42:26.139047 wi1-bot-1.3.2/wi1_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-04-23 07:42:25.000000 wi1-bot-1.3.2/wi1_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-23 07:42:26.000000 wi1-bot-1.3.2/wi1_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 07:42:25.000000 wi1-bot-1.3.2/wi1_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-23 07:42:25.000000 wi1-bot-1.3.2/wi1_bot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-23 07:42:25.000000 wi1-bot-1.3.2/wi1_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-23 07:42:26.000000 wi1-bot-1.3.2/wi1_bot.egg-info/top_level.txt
```

### Comparing `wi1-bot-1.3.1/.github/workflows/pypi-publish.yml` & `wi1-bot-1.3.2/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.1/.pre-commit-config.yaml` & `wi1-bot-1.3.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.1/LICENSE` & `wi1-bot-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.1/PKG-INFO` & `wi1-bot-1.3.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wi1-bot
-Version: 1.3.1
+Version: 1.3.2
 Summary: Discord bot for Radarr/Sonarr integration
 Home-page: https://github.com/wthueb/wi1-bot
 Author-email: William Huebner <wilhueb@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 William Huebner
         
@@ -53,16 +53,15 @@
 3. `pip install -e .[dev]`
 4. `pre-commit install`
 
 Requires Python >=3.10.
 
 ### TODO
 
-- Use `mypy --strict`
-- Use Discord slash commands instead of normal text commands
+- Use Discord slash commands instead of normal text commands (difficult: can't have "conversation" with slash commands)
 - Web dashboard for seeing transcode queue, transcode progress, quotas
 - Enforce quotas
 - !linktmdb
     - !rate / !ratings (https://developers.themoviedb.org/3/movies/rate-movie)
     - !movierec based off of ratings and similar-to-user ratings?
         - https://towardsdatascience.com/the-4-recommendation-engines-that-can-predict-your-movie-tastes-109dc4e10c52
         - or just use TMDB's API to get recommendations (if that's possible?)
```

### Comparing `wi1-bot-1.3.1/README.md` & `wi1-bot-1.3.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -15,16 +15,15 @@
 3. `pip install -e .[dev]`
 4. `pre-commit install`
 
 Requires Python >=3.10.
 
 ### TODO
 
-- Use `mypy --strict`
-- Use Discord slash commands instead of normal text commands
+- Use Discord slash commands instead of normal text commands (difficult: can't have "conversation" with slash commands)
 - Web dashboard for seeing transcode queue, transcode progress, quotas
 - Enforce quotas
 - !linktmdb
     - !rate / !ratings (https://developers.themoviedb.org/3/movies/rate-movie)
     - !movierec based off of ratings and similar-to-user ratings?
         - https://towardsdatascience.com/the-4-recommendation-engines-that-can-predict-your-movie-tastes-109dc4e10c52
         - or just use TMDB's API to get recommendations (if that's possible?)
```

### Comparing `wi1-bot-1.3.1/config.yaml.template` & `wi1-bot-1.3.2/config.yaml.template`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 ---
+general:
+  # log file directory, optional
+  log_dir: /var/log/wi1-bot
+
 radarr:
   # radarr url you use to get to the dashboard
   url: http://localhost:7878
   # radarr api key (Settings->General->Security->API Key)
   api_key: XXX
   # radarr root folder (absolute path)
   root_folder: /full/path/movies
```

### Comparing `wi1-bot-1.3.1/pyproject.toml` & `wi1-bot-1.3.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -12,34 +12,32 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.10"
 ]
 dynamic = ["version"]
 requires-python = ">=3.10"
 dependencies = [
-    "discord.py==2.1.0",
-    "Flask==2.1.2",
-    "mongoengine==0.24.1",
+    "discord.py==2.2.2",
+    "Flask==2.2.3",
+    "mongoengine==0.27.0",
     "pyarr==3.1.3",
     "python-pushover==0.4",
     "PyYAML==6.0"
 ]
 
 [project.optional-dependencies]
 dev = [
-    "black==22.12.0",
+    "black==23.3.0",
     "flake8==6.0.0",
     "isort==5.12.0",
     "mongo-types==0.15.1",
-    "mypy==0.991",
-    "pre-commit==3.0.2",
+    "mypy==1.2.0",
+    "pre-commit==3.2.2",
     "requests==2.28.2",
-    "types-flask==1.1.6",
-    "types-PyYAML==6.0.12.3",
-    "types-requests==2.28.11.8"
+    "types-PyYAML==6.0.12.9",
 ]
 
 [project.urls]
 Homepage = "https://github.com/wthueb/wi1-bot"
 
 [project.scripts]
 wi1-bot = "wi1_bot.scripts.start:main"
```

### Comparing `wi1-bot-1.3.1/wi1_bot/arr/download.py` & `wi1-bot-1.3.2/wi1_bot/arr/download.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.1/wi1_bot/arr/episode.py` & `wi1-bot-1.3.2/wi1_bot/arr/episode.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.1/wi1_bot/arr/movie.py` & `wi1-bot-1.3.2/wi1_bot/arr/movie.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.1/wi1_bot/arr/radarr.py` & `wi1-bot-1.3.2/wi1_bot/arr/radarr.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.1/wi1_bot/arr/sonarr.py` & `wi1-bot-1.3.2/wi1_bot/arr/sonarr.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.1/wi1_bot/config.py` & `wi1-bot-1.3.2/wi1_bot/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -92,15 +92,24 @@
     hwaccel: str  # optional
 
 
 class TranscodingConfig(TranscodingConfigOptional):
     profiles: dict[str, TranscodingProfile]
 
 
+class GeneralConfigOptional(TypedDict, total=False):
+    log_dir: str
+
+
+class GeneralConfig(GeneralConfigOptional):
+    pass
+
+
 class ConfigOptional(TypedDict, total=False):
+    general: GeneralConfig  # optional
     pushover: PushoverConfig  # optional
     transcoding: TranscodingConfig  # optional
 
 
 class Config(ConfigOptional):
     radarr: ArrConfig
     sonarr: ArrConfig
```

### Comparing `wi1-bot-1.3.1/wi1_bot/discord/bot.py` & `wi1-bot-1.3.2/wi1_bot/discord/bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,20 +59,20 @@
         await bot.change_presence(
             activity=discord.Activity(
                 type=discord.ActivityType.watching,
                 name=config["discord"]["bot_presence"],
             )
         )
 
-    logger.debug("bot is ready")
+    logger.info("bot is ready")
 
 
 @bot.before_invoke
 async def before_invoke(ctx: commands.Context[Any]) -> None:
-    logger.debug(f"got command from {ctx.message.author}: {ctx.message.content}")
+    logger.info(f"got command from {ctx.message.author}: {ctx.message.content}")
 
 
 @commands.cooldown(1, 10)  # type: ignore
 @bot.command(
     name="downloads", aliases=["queue", "q"], help="see the status of movie downloads"
 )
 async def downloads_cmd(ctx: commands.Context[Any]) -> None:
@@ -157,15 +157,15 @@
     radarr.create_tag(tag)
     sonarr.create_tag(tag)
 
     await reply(ctx.message, f"tag `{tag}` added for {user.display_name}")
 
 
 async def run() -> None:
-    logger.debug("starting bot")
+    logger.info("starting bot")
 
     async with bot:
         await bot.add_cog(MovieCog(bot))
         await bot.add_cog(SeriesCog(bot))
 
         await bot.start(config["discord"]["bot_token"])
```

### Comparing `wi1-bot-1.3.1/wi1_bot/discord/cogs/movie.py` & `wi1-bot-1.3.2/wi1_bot/discord/cogs/movie.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.1/wi1_bot/discord/cogs/series.py` & `wi1-bot-1.3.2/wi1_bot/discord/cogs/series.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.1/wi1_bot/discord/helpers.py` & `wi1-bot-1.3.2/wi1_bot/discord/helpers.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.1/wi1_bot/push.py` & `wi1-bot-1.3.2/wi1_bot/push.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.1/wi1_bot/scripts/start.py` & `wi1-bot-1.3.2/wi1_bot/scripts/start.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import asyncio
 import logging
 import logging.config
+import pathlib
+from typing import Any
 
 from wi1_bot import webhook
+from wi1_bot.config import config
 from wi1_bot.discord import bot
 from wi1_bot.transcoder import Transcoder
 
 
 def main() -> None:
-    logging_config = {
+    logging_config: dict[str, Any] = {
         "version": 1,
         "disable_existing_loggers": True,
         "formatters": {
             "basic": {
                 "class": "logging.Formatter",
                 "format": "[%(asctime)s] %(levelname)s %(message)s",
                 "datefmt": "%Y-%m-%d %H:%M:%S",
@@ -28,37 +31,44 @@
         "handlers": {
             "console": {
                 "class": "logging.StreamHandler",
                 "stream": "ext://sys.stdout",
                 "level": "DEBUG",
                 "formatter": "detailed",
             },
-            # "file": {
-            #     "class": "logging.handlers.RotatingFileHandler",
-            #     "filename": "logs/wi1-bot.log",
-            #     "maxBytes": 1024**2 * 10,  # 10 MB
-            #     "backupCount": 20,
-            #     "level": "INFO",
-            #     "formatter": "basic",
-            # },
-            # "file_debug": {
-            #     "class": "logging.handlers.RotatingFileHandler",
-            #     "filename": "logs/wi1-bot.debug.log",
-            #     "maxBytes": 1024**2 * 10,  # 10 MB
-            #     "backupCount": 20,
-            #     "level": "DEBUG",
-            #     "formatter": "detailed",
-            # },
         },
         "loggers": {
             "": {"level": "DEBUG", "handlers": ["console"]},
             "wi1_bot": {"level": "DEBUG", "handlers": [], "propagate": True},
         },
     }
 
+    if "general" in config and "log_dir" in config["general"]:
+        log_dir = pathlib.Path(config["general"]["log_dir"]).resolve()
+
+        logging_config["handlers"]["file"] = {
+            "class": "logging.handlers.RotatingFileHandler",
+            "filename": str(log_dir / "wi1-bot.log"),
+            "maxBytes": 1024**2 * 10,  # 10 MB
+            "backupCount": 20,
+            "level": "INFO",
+            "formatter": "basic",
+        }
+
+        logging_config["handlers"]["file_debug"] = {
+            "class": "logging.handlers.RotatingFileHandler",
+            "filename": str(log_dir / "wi1-bot.debug.log"),
+            "maxBytes": 1024**2 * 10,  # 10 MB
+            "backupCount": 20,
+            "level": "DEBUG",
+            "formatter": "detailed",
+        }
+
+        logging_config["loggers"][""]["handlers"].extend(["file", "file_debug"])
+
     logging.config.dictConfig(logging_config)
 
     webhook.start()
 
     t = Transcoder()
     t.start()
```

### Comparing `wi1-bot-1.3.1/wi1_bot/scripts/transcode_item.py` & `wi1-bot-1.3.2/wi1_bot/scripts/transcode_item.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.1/wi1_bot/transcoder/transcode_queue.py` & `wi1-bot-1.3.2/wi1_bot/transcoder/transcode_queue.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.1/wi1_bot/transcoder/transcoder.py` & `wi1-bot-1.3.2/wi1_bot/transcoder/transcoder.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.1/wi1_bot/webhook.py` & `wi1-bot-1.3.2/wi1_bot/webhook.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.1/wi1_bot.egg-info/PKG-INFO` & `wi1-bot-1.3.2/wi1_bot.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wi1-bot
-Version: 1.3.1
+Version: 1.3.2
 Summary: Discord bot for Radarr/Sonarr integration
 Home-page: https://github.com/wthueb/wi1-bot
 Author-email: William Huebner <wilhueb@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 William Huebner
         
@@ -53,16 +53,15 @@
 3. `pip install -e .[dev]`
 4. `pre-commit install`
 
 Requires Python >=3.10.
 
 ### TODO
 
-- Use `mypy --strict`
-- Use Discord slash commands instead of normal text commands
+- Use Discord slash commands instead of normal text commands (difficult: can't have "conversation" with slash commands)
 - Web dashboard for seeing transcode queue, transcode progress, quotas
 - Enforce quotas
 - !linktmdb
     - !rate / !ratings (https://developers.themoviedb.org/3/movies/rate-movie)
     - !movierec based off of ratings and similar-to-user ratings?
         - https://towardsdatascience.com/the-4-recommendation-engines-that-can-predict-your-movie-tastes-109dc4e10c52
         - or just use TMDB's API to get recommendations (if that's possible?)
```

### Comparing `wi1-bot-1.3.1/wi1_bot.egg-info/SOURCES.txt` & `wi1-bot-1.3.2/wi1_bot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

