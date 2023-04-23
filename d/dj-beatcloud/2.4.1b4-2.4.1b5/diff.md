# Comparing `tmp/dj_beatcloud-2.4.1b4.tar.gz` & `tmp/dj_beatcloud-2.4.1b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj_beatcloud-2.4.1b4.tar", last modified: Thu Apr 13 17:08:19 2023, max compression
+gzip compressed data, was "dj_beatcloud-2.4.1b5.tar", last modified: Sun Apr 23 15:10:39 2023, max compression
```

## Comparing `dj_beatcloud-2.4.1b4.tar` & `dj_beatcloud-2.4.1b5.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-13 17:08:19.237205 dj_beatcloud-2.4.1b4/
--rw-r--r--   0 alrichards   (502) staff       (20)    35148 2022-06-16 01:40:44.000000 dj_beatcloud-2.4.1b4/LICENSE
--rw-r--r--   0 alrichards   (502) staff       (20)       64 2022-06-16 01:40:44.000000 dj_beatcloud-2.4.1b4/MANIFEST.in
--rw-r--r--   0 alrichards   (502) staff       (20)    29508 2023-04-13 17:08:19.237333 dj_beatcloud-2.4.1b4/PKG-INFO
--rw-r--r--   0 alrichards   (502) staff       (20)    28223 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/README.md
--rw-r--r--   0 alrichards   (502) staff       (20)      225 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/pyproject.toml
--rw-r--r--   0 alrichards   (502) staff       (20)      164 2023-04-13 17:08:19.237628 dj_beatcloud-2.4.1b4/setup.cfg
--rw-r--r--   0 alrichards   (502) staff       (20)     2225 2023-04-13 15:48:53.000000 dj_beatcloud-2.4.1b4/setup.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-13 17:08:19.220504 dj_beatcloud-2.4.1b4/src/
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-13 17:08:19.222709 dj_beatcloud-2.4.1b4/src/dj_beatcloud.egg-info/
--rw-r--r--   0 alrichards   (502) staff       (20)    29508 2023-04-13 17:08:19.000000 dj_beatcloud-2.4.1b4/src/dj_beatcloud.egg-info/PKG-INFO
--rw-r--r--   0 alrichards   (502) staff       (20)     2193 2023-04-13 17:08:19.000000 dj_beatcloud-2.4.1b4/src/dj_beatcloud.egg-info/SOURCES.txt
--rw-r--r--   0 alrichards   (502) staff       (20)        1 2023-04-13 17:08:19.000000 dj_beatcloud-2.4.1b4/src/dj_beatcloud.egg-info/dependency_links.txt
--rw-r--r--   0 alrichards   (502) staff       (20)       50 2023-04-13 17:08:19.000000 dj_beatcloud-2.4.1b4/src/dj_beatcloud.egg-info/entry_points.txt
--rw-r--r--   0 alrichards   (502) staff       (20)      332 2023-04-13 17:08:19.000000 dj_beatcloud-2.4.1b4/src/dj_beatcloud.egg-info/requires.txt
--rw-r--r--   0 alrichards   (502) staff       (20)       18 2023-04-13 17:08:19.000000 dj_beatcloud-2.4.1b4/src/dj_beatcloud.egg-info/top_level.txt
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-13 17:08:19.224135 dj_beatcloud-2.4.1b4/src/djtools/
--rw-r--r--   0 alrichards   (502) staff       (20)      966 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b4/src/djtools/__init__.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-13 17:08:19.227567 dj_beatcloud-2.4.1b4/src/djtools/configs/
--rw-r--r--   0 alrichards   (502) staff       (20)     6148 2023-03-09 22:06:36.000000 dj_beatcloud-2.4.1b4/src/djtools/configs/.DS_Store
--rw-r--r--   0 alrichards   (502) staff       (20)     4258 2023-03-09 22:06:36.000000 dj_beatcloud-2.4.1b4/src/djtools/configs/README.md
--rw-r--r--   0 alrichards   (502) staff       (20)      496 2023-03-09 22:06:36.000000 dj_beatcloud-2.4.1b4/src/djtools/configs/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3103 2023-04-13 16:23:56.000000 dj_beatcloud-2.4.1b4/src/djtools/configs/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1223 2023-03-09 22:09:23.000000 dj_beatcloud-2.4.1b4/src/djtools/configs/config.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)    13418 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/djtools/configs/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)      484 2023-03-09 22:06:36.000000 dj_beatcloud-2.4.1b4/src/djtools/configs/logging.conf
--rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-04-13 16:51:43.000000 dj_beatcloud-2.4.1b4/src/djtools/configs/registered_users.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)      878 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/djtools/configs/rekordbox_playlists.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-03-09 22:09:23.000000 dj_beatcloud-2.4.1b4/src/djtools/configs/spotify_playlists.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)     2305 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/djtools/configs/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4478 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/djtools/configs/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1721 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b4/src/djtools/dj_tools.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-13 17:08:19.227754 dj_beatcloud-2.4.1b4/src/djtools/logs/
--rw-r--r--   0 alrichards   (502) staff       (20)        0 2022-06-16 01:40:44.000000 dj_beatcloud-2.4.1b4/src/djtools/logs/empty.txt
--rw-r--r--   0 alrichards   (502) staff       (20)     1649 2023-03-16 00:56:47.000000 dj_beatcloud-2.4.1b4/src/djtools/main.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-13 17:08:19.231027 dj_beatcloud-2.4.1b4/src/djtools/rekordbox/
--rw-r--r--   0 alrichards   (502) staff       (20)     1360 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b4/src/djtools/rekordbox/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1794 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/djtools/rekordbox/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4123 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/djtools/rekordbox/copy_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4521 2023-04-12 23:23:56.000000 dj_beatcloud-2.4.1b4/src/djtools/rekordbox/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)    18868 2023-04-12 23:23:56.000000 dj_beatcloud-2.4.1b4/src/djtools/rekordbox/playlist_builder.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2859 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/djtools/rekordbox/randomize_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)    13303 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/djtools/rekordbox/tag_parsers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1225 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/djtools/rekordbox/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1390 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/djtools/rekordbox/test_copy_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2807 2023-04-12 23:23:56.000000 dj_beatcloud-2.4.1b4/src/djtools/rekordbox/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     5142 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/djtools/rekordbox/test_playlist_builder.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1477 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/djtools/rekordbox/test_randomize_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3975 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/djtools/rekordbox/test_tag_parsers.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-13 17:08:19.232927 dj_beatcloud-2.4.1b4/src/djtools/spotify/
--rw-r--r--   0 alrichards   (502) staff       (20)      718 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b4/src/djtools/spotify/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3229 2023-03-09 18:55:21.000000 dj_beatcloud-2.4.1b4/src/djtools/spotify/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)    15361 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/djtools/spotify/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     6155 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/djtools/spotify/playlist_builder.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1958 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b4/src/djtools/spotify/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)    17499 2023-03-17 15:21:16.000000 dj_beatcloud-2.4.1b4/src/djtools/spotify/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     6153 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/djtools/spotify/test_playlist_builder.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-13 17:08:19.234632 dj_beatcloud-2.4.1b4/src/djtools/sync/
--rw-r--r--   0 alrichards   (502) staff       (20)      772 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b4/src/djtools/sync/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4706 2023-04-13 16:50:12.000000 dj_beatcloud-2.4.1b4/src/djtools/sync/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     8237 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/djtools/sync/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4605 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/djtools/sync/sync_operations.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4038 2023-04-13 16:51:38.000000 dj_beatcloud-2.4.1b4/src/djtools/sync/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     7496 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/djtools/sync/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4520 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/djtools/sync/test_sync_operations.py
--rw-r--r--   0 alrichards   (502) staff       (20)      830 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/djtools/test_main.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-13 17:08:19.236600 dj_beatcloud-2.4.1b4/src/djtools/utils/
--rw-r--r--   0 alrichards   (502) staff       (20)      821 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b4/src/djtools/utils/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3488 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/djtools/utils/check_tracks.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1093 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/djtools/utils/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     7904 2023-04-13 15:40:43.000000 dj_beatcloud-2.4.1b4/src/djtools/utils/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3227 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/djtools/utils/test_check_tracks.py
--rw-r--r--   0 alrichards   (502) staff       (20)      397 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b4/src/djtools/utils/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     8533 2023-04-13 15:45:33.000000 dj_beatcloud-2.4.1b4/src/djtools/utils/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1580 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/djtools/utils/test_url_download.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1641 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/djtools/utils/url_download.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-13 17:08:19.237029 dj_beatcloud-2.4.1b4/src/test_data/
--rw-r--r--   0 alrichards   (502) staff       (20)      138 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/test_data/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3547 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/test_data/conftest.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-23 15:10:39.607978 dj_beatcloud-2.4.1b5/
+-rw-r--r--   0 alrichards   (502) staff       (20)    35148 2022-06-16 01:40:44.000000 dj_beatcloud-2.4.1b5/LICENSE
+-rw-r--r--   0 alrichards   (502) staff       (20)       64 2022-06-16 01:40:44.000000 dj_beatcloud-2.4.1b5/MANIFEST.in
+-rw-r--r--   0 alrichards   (502) staff       (20)    29508 2023-04-23 15:10:39.608108 dj_beatcloud-2.4.1b5/PKG-INFO
+-rw-r--r--   0 alrichards   (502) staff       (20)    28223 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/README.md
+-rw-r--r--   0 alrichards   (502) staff       (20)      225 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/pyproject.toml
+-rw-r--r--   0 alrichards   (502) staff       (20)      164 2023-04-23 15:10:39.608472 dj_beatcloud-2.4.1b5/setup.cfg
+-rw-r--r--   0 alrichards   (502) staff       (20)     2225 2023-04-23 15:10:29.000000 dj_beatcloud-2.4.1b5/setup.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-23 15:10:39.591810 dj_beatcloud-2.4.1b5/src/
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-23 15:10:39.595153 dj_beatcloud-2.4.1b5/src/dj_beatcloud.egg-info/
+-rw-r--r--   0 alrichards   (502) staff       (20)    29508 2023-04-23 15:10:39.000000 dj_beatcloud-2.4.1b5/src/dj_beatcloud.egg-info/PKG-INFO
+-rw-r--r--   0 alrichards   (502) staff       (20)     2193 2023-04-23 15:10:39.000000 dj_beatcloud-2.4.1b5/src/dj_beatcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)        1 2023-04-23 15:10:39.000000 dj_beatcloud-2.4.1b5/src/dj_beatcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)       50 2023-04-23 15:10:39.000000 dj_beatcloud-2.4.1b5/src/dj_beatcloud.egg-info/entry_points.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)      332 2023-04-23 15:10:39.000000 dj_beatcloud-2.4.1b5/src/dj_beatcloud.egg-info/requires.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)       18 2023-04-23 15:10:39.000000 dj_beatcloud-2.4.1b5/src/dj_beatcloud.egg-info/top_level.txt
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-23 15:10:39.596075 dj_beatcloud-2.4.1b5/src/djtools/
+-rw-r--r--   0 alrichards   (502) staff       (20)      966 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b5/src/djtools/__init__.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-23 15:10:39.598811 dj_beatcloud-2.4.1b5/src/djtools/configs/
+-rw-r--r--   0 alrichards   (502) staff       (20)     6148 2023-03-09 22:06:36.000000 dj_beatcloud-2.4.1b5/src/djtools/configs/.DS_Store
+-rw-r--r--   0 alrichards   (502) staff       (20)     4258 2023-03-09 22:06:36.000000 dj_beatcloud-2.4.1b5/src/djtools/configs/README.md
+-rw-r--r--   0 alrichards   (502) staff       (20)      496 2023-03-09 22:06:36.000000 dj_beatcloud-2.4.1b5/src/djtools/configs/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3103 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/configs/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1223 2023-03-09 22:09:23.000000 dj_beatcloud-2.4.1b5/src/djtools/configs/config.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)    13418 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/configs/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      484 2023-03-09 22:06:36.000000 dj_beatcloud-2.4.1b5/src/djtools/configs/logging.conf
+-rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-04-13 16:51:43.000000 dj_beatcloud-2.4.1b5/src/djtools/configs/registered_users.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)      878 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/configs/rekordbox_playlists.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-03-09 22:09:23.000000 dj_beatcloud-2.4.1b5/src/djtools/configs/spotify_playlists.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)     2305 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/configs/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4641 2023-04-23 15:09:12.000000 dj_beatcloud-2.4.1b5/src/djtools/configs/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1721 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b5/src/djtools/dj_tools.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-23 15:10:39.598976 dj_beatcloud-2.4.1b5/src/djtools/logs/
+-rw-r--r--   0 alrichards   (502) staff       (20)        0 2022-06-16 01:40:44.000000 dj_beatcloud-2.4.1b5/src/djtools/logs/empty.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)     1649 2023-03-16 00:56:47.000000 dj_beatcloud-2.4.1b5/src/djtools/main.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-23 15:10:39.602038 dj_beatcloud-2.4.1b5/src/djtools/rekordbox/
+-rw-r--r--   0 alrichards   (502) staff       (20)     1360 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b5/src/djtools/rekordbox/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1794 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/rekordbox/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4123 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/rekordbox/copy_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4521 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/rekordbox/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    18868 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/rekordbox/playlist_builder.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2859 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/rekordbox/randomize_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    13303 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/rekordbox/tag_parsers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1225 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/rekordbox/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1390 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/rekordbox/test_copy_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3013 2023-04-23 15:09:12.000000 dj_beatcloud-2.4.1b5/src/djtools/rekordbox/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     5142 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/rekordbox/test_playlist_builder.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1477 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/rekordbox/test_randomize_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3975 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/rekordbox/test_tag_parsers.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-23 15:10:39.603408 dj_beatcloud-2.4.1b5/src/djtools/spotify/
+-rw-r--r--   0 alrichards   (502) staff       (20)      718 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b5/src/djtools/spotify/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3229 2023-03-09 18:55:21.000000 dj_beatcloud-2.4.1b5/src/djtools/spotify/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    15361 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/spotify/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     6155 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/spotify/playlist_builder.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1958 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b5/src/djtools/spotify/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    17499 2023-03-17 15:21:16.000000 dj_beatcloud-2.4.1b5/src/djtools/spotify/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     6153 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/spotify/test_playlist_builder.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-23 15:10:39.605593 dj_beatcloud-2.4.1b5/src/djtools/sync/
+-rw-r--r--   0 alrichards   (502) staff       (20)      772 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b5/src/djtools/sync/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4706 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/sync/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     8237 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/sync/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4605 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/sync/sync_operations.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4038 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/sync/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     8185 2023-04-23 15:09:12.000000 dj_beatcloud-2.4.1b5/src/djtools/sync/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4713 2023-04-23 15:09:12.000000 dj_beatcloud-2.4.1b5/src/djtools/sync/test_sync_operations.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      830 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/test_main.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-23 15:10:39.607334 dj_beatcloud-2.4.1b5/src/djtools/utils/
+-rw-r--r--   0 alrichards   (502) staff       (20)      821 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b5/src/djtools/utils/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3488 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/utils/check_tracks.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1093 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/utils/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     7970 2023-04-23 15:09:12.000000 dj_beatcloud-2.4.1b5/src/djtools/utils/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3227 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/utils/test_check_tracks.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      397 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b5/src/djtools/utils/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     8533 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/utils/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1580 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/utils/test_url_download.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1641 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/utils/url_download.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-23 15:10:39.607786 dj_beatcloud-2.4.1b5/src/test_data/
+-rw-r--r--   0 alrichards   (502) staff       (20)      138 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/test_data/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3547 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/test_data/conftest.py
```

### Comparing `dj_beatcloud-2.4.1b4/LICENSE` & `dj_beatcloud-2.4.1b5/LICENSE`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b4/PKG-INFO` & `dj_beatcloud-2.4.1b5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj_beatcloud
-Version: 2.4.1b4
+Version: 2.4.1b5
 Summary: DJ Tools is a library for managing a collection of music and Rekordbox XML files.
 Home-page: https://github.com/a-rich/DJ-tools
 Author: Alex Richards
 Author-email: alex.richards006@gmail.com
 License: GNU GPLv3
 Keywords: MP3 Rekordbox XML spotify reddit aws s3
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dj_beatcloud-2.4.1b4/README.md` & `dj_beatcloud-2.4.1b5/README.md`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b4/setup.py` & `dj_beatcloud-2.4.1b5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 EXTRAS = {
         'levenshtein': ['python-Levenshtein==0.12.2']
 }
 
 setup(
     name='dj_beatcloud',
-    version='2.4.1-b4',
+    version='2.4.1-b5',
     description=(
         'DJ Tools is a library for managing a collection of music and '
         'Rekordbox XML files.'
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url='https://github.com/a-rich/DJ-tools',
```

### Comparing `dj_beatcloud-2.4.1b4/src/dj_beatcloud.egg-info/PKG-INFO` & `dj_beatcloud-2.4.1b5/src/dj_beatcloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-beatcloud
-Version: 2.4.1b4
+Version: 2.4.1b5
 Summary: DJ Tools is a library for managing a collection of music and Rekordbox XML files.
 Home-page: https://github.com/a-rich/DJ-tools
 Author: Alex Richards
 Author-email: alex.richards006@gmail.com
 License: GNU GPLv3
 Keywords: MP3 Rekordbox XML spotify reddit aws s3
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dj_beatcloud-2.4.1b4/src/dj_beatcloud.egg-info/SOURCES.txt` & `dj_beatcloud-2.4.1b5/src/dj_beatcloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b4/src/djtools/__init__.py` & `dj_beatcloud-2.4.1b5/src/djtools/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b4/src/djtools/configs/.DS_Store` & `dj_beatcloud-2.4.1b5/src/djtools/configs/.DS_Store`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b4/src/djtools/configs/README.md` & `dj_beatcloud-2.4.1b5/src/djtools/configs/README.md`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b4/src/djtools/configs/config.py` & `dj_beatcloud-2.4.1b5/src/djtools/configs/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b4/src/djtools/configs/config.yaml` & `dj_beatcloud-2.4.1b5/src/djtools/configs/config.yaml`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b4/src/djtools/configs/helpers.py` & `dj_beatcloud-2.4.1b5/src/djtools/configs/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b4/src/djtools/configs/rekordbox_playlists.yaml` & `dj_beatcloud-2.4.1b5/src/djtools/configs/rekordbox_playlists.yaml`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b4/src/djtools/configs/test_config.py` & `dj_beatcloud-2.4.1b5/src/djtools/configs/test_config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b4/src/djtools/configs/test_helpers.py` & `dj_beatcloud-2.4.1b5/src/djtools/configs/test_helpers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from argparse import Namespace
 from pathlib import Path
+import re
 from typing import List
 from unittest import mock
 
 import pytest
 
 from djtools.configs.config import BaseConfig
 from djtools.configs.helpers import (
@@ -37,15 +38,19 @@
 def test_arg_parse_links_configs_dir_does_not_exist(mock_parse_args, tmpdir):
     link_path = str(tmpdir)
     mock_parse_args.return_value = Namespace(
         link_configs=link_path, log_level="INFO"
     )
     with pytest.raises(
         ValueError,
-        match=f'{link_path} must be a directory that does not already exist',
+        # NOTE(a-rich): WindowsPath needs to be escaped for `\` characters to
+        # appear in the `match` argument.
+        match=re.escape(
+            f'{link_path} must be a directory that does not already exist'
+        ),
     ):
         args = arg_parse()
 
 
 @mock.patch("djtools.spotify.helpers.get_spotify_client")
 @mock.patch(
     "builtins.open",
```

### Comparing `dj_beatcloud-2.4.1b4/src/djtools/dj_tools.py` & `dj_beatcloud-2.4.1b5/src/djtools/dj_tools.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b4/src/djtools/main.py` & `dj_beatcloud-2.4.1b5/src/djtools/main.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b4/src/djtools/rekordbox/__init__.py` & `dj_beatcloud-2.4.1b5/src/djtools/rekordbox/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b4/src/djtools/rekordbox/config.py` & `dj_beatcloud-2.4.1b5/src/djtools/rekordbox/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b4/src/djtools/rekordbox/copy_playlists.py` & `dj_beatcloud-2.4.1b5/src/djtools/rekordbox/copy_playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b4/src/djtools/rekordbox/helpers.py` & `dj_beatcloud-2.4.1b5/src/djtools/rekordbox/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b4/src/djtools/rekordbox/playlist_builder.py` & `dj_beatcloud-2.4.1b5/src/djtools/rekordbox/playlist_builder.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b4/src/djtools/rekordbox/randomize_playlists.py` & `dj_beatcloud-2.4.1b5/src/djtools/rekordbox/randomize_playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b4/src/djtools/rekordbox/tag_parsers.py` & `dj_beatcloud-2.4.1b5/src/djtools/rekordbox/tag_parsers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b4/src/djtools/rekordbox/test_config.py` & `dj_beatcloud-2.4.1b5/src/djtools/rekordbox/test_config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b4/src/djtools/rekordbox/test_copy_playlists.py` & `dj_beatcloud-2.4.1b5/src/djtools/rekordbox/test_copy_playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b4/src/djtools/rekordbox/test_helpers.py` & `dj_beatcloud-2.4.1b5/src/djtools/rekordbox/test_helpers.py`

 * *Files 17% similar despite different names*

```diff
@@ -73,15 +73,18 @@
     old_track_loc = Path(test_track["Location"])
     copy_file(track=test_track, destination=dest_dir)
     new_track_loc = unquote(test_track["Location"])
     loc_prefix = inspect.signature(
         copy_file
     ).parameters.get("loc_prefix").default
     new_file_path = dest_dir / old_track_loc.name
-    assert new_track_loc == f"{loc_prefix}{new_file_path}"
+    # NOTE(a-rich): `Location` attributes in the XML's `TRACK` tags always
+    # have unix-style paths so comparisons made with paths created in Windows
+    # must be interpretted `.as_posix()`.
+    assert new_track_loc == f"{loc_prefix}{new_file_path.as_posix()}"
     assert new_file_path.exists()
 
 
 def test_get_playlist_track_locations(xml):
     playlist = "Hip Hop"
     seen_tracks = set()
     ret = get_playlist_track_locations(xml, playlist, seen_tracks)
```

### Comparing `dj_beatcloud-2.4.1b4/src/djtools/rekordbox/test_playlist_builder.py` & `dj_beatcloud-2.4.1b5/src/djtools/rekordbox/test_playlist_builder.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b4/src/djtools/rekordbox/test_randomize_playlists.py` & `dj_beatcloud-2.4.1b5/src/djtools/rekordbox/test_randomize_playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b4/src/djtools/rekordbox/test_tag_parsers.py` & `dj_beatcloud-2.4.1b5/src/djtools/rekordbox/test_tag_parsers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b4/src/djtools/spotify/__init__.py` & `dj_beatcloud-2.4.1b5/src/djtools/spotify/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b4/src/djtools/spotify/config.py` & `dj_beatcloud-2.4.1b5/src/djtools/spotify/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b4/src/djtools/spotify/helpers.py` & `dj_beatcloud-2.4.1b5/src/djtools/spotify/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b4/src/djtools/spotify/playlist_builder.py` & `dj_beatcloud-2.4.1b5/src/djtools/spotify/playlist_builder.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b4/src/djtools/spotify/test_config.py` & `dj_beatcloud-2.4.1b5/src/djtools/spotify/test_config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b4/src/djtools/spotify/test_helpers.py` & `dj_beatcloud-2.4.1b5/src/djtools/spotify/test_helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b4/src/djtools/spotify/test_playlist_builder.py` & `dj_beatcloud-2.4.1b5/src/djtools/spotify/test_playlist_builder.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b4/src/djtools/sync/__init__.py` & `dj_beatcloud-2.4.1b5/src/djtools/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b4/src/djtools/sync/config.py` & `dj_beatcloud-2.4.1b5/src/djtools/sync/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b4/src/djtools/sync/helpers.py` & `dj_beatcloud-2.4.1b5/src/djtools/sync/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b4/src/djtools/sync/sync_operations.py` & `dj_beatcloud-2.4.1b5/src/djtools/sync/sync_operations.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b4/src/djtools/sync/test_config.py` & `dj_beatcloud-2.4.1b5/src/djtools/sync/test_config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b4/src/djtools/sync/test_helpers.py` & `dj_beatcloud-2.4.1b5/src/djtools/sync/test_helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,18 +85,21 @@
     test_config.XML_PATH = test_xml
     other_users_xml = Path(test_xml).parent / f"{other_user}_rekordbox.xml"
     other_users_xml.write_text(Path(test_xml).read_text())
 
     for track in xml.find_all("TRACK"):
         if not track.get("Location"):
             continue
+        # NOTE(a-rich): `Location` attributes in the XML's `TRACK` tags always
+        # have unix-style paths so paths created in Windows must be
+        # interpretted `.as_posix()`.
         track["Location"] = (
             Path(track["Location"]).parent / user_b_path.strip("/") /
             Path(track["Location"]).name
-        )
+        ).as_posix()
     
     with open(
         other_users_xml, mode="wb", encoding=xml.orignal_encoding
     ) as _file:
         _file.write(xml.prettify("utf-8"))
         
     rewrite_xml(test_config)
@@ -123,17 +126,22 @@
             "- other artist.mp3 to s3://dj.beatcloud.com/dj/music/Bass/"
             "2O22-12-21/other track - other artist.mp3\n"
         "upload: ../../Volumes/AWEEEEZY/DJ Music/Techno/2022-12-22/last track "
             "- last artist.mp3 to s3://dj.beatcloud.com/dj/music/Techno/"
             "2022-12-22/last track - last artist.mp3"
         "\nirrelevant line"
     )
-    tmp_file = tempfile.NamedTemporaryFile(mode="w")
+    # NOTE(a-rich): Windows does not allow opening a temporary file after it's
+    # been created. The WAR is to initialize a `NamedTemporaryFile` with the
+    # `delete` argument set to `False` and explicitly `.close()` the object
+    # before calling `open()` on it.
+    tmp_file = tempfile.NamedTemporaryFile(mode="w", delete=False)
     tmp_file.write(sync_output)
     tmp_file.seek(0)
+    tmp_file.close()
     tmp_file = open(tmp_file.name)
     process = mock_popen.return_value.__enter__.return_value
     process.stdout = tmp_file
     process.wait.return_value = 0
     ret = run_sync(cmd)
     expected = (
         "Bass/2022-12-21: 1\n\ttrack - artist.mp3\nBass/2O22-12-21: 1\n\tother"
@@ -142,18 +150,27 @@
     )
     assert ret == expected
 
 
 @mock.patch("djtools.sync.helpers.Popen")
 def test_run_sync_handles_return_code(mock_popen, tmpdir, caplog):
     caplog.set_level("CRITICAL")
-    cmd = ["aws", "s3", "sync", str(tmpdir), "s3://dj.beatcloud.com/dj/music/"]
-    tmp_file = tempfile.NamedTemporaryFile(mode="w")
+    # NOTE(a-rich): subprocess calls to `awscli` need to have unix-style path
+    # arguments.
+    cmd = [
+        "aws",
+        "s3",
+        "sync",
+        Path(tmpdir).as_posix(),
+        "s3://dj.beatcloud.com/dj/music/",
+    ]
+    tmp_file = tempfile.NamedTemporaryFile(mode="w", delete=False)
     tmp_file.write("")
     tmp_file.seek(0)
+    tmp_file.close()
     tmp_file = open(tmp_file.name)
     process = mock_popen.return_value.__enter__.return_value
     process.stdout = tmp_file
     process.wait.return_value = 1
     msg = (
         f"Failure while syncing: Command '{' '.join(cmd)}' returned "
         f"non-zero exit status {process.wait.return_value}."
```

### Comparing `dj_beatcloud-2.4.1b4/src/djtools/sync/test_sync_operations.py` & `dj_beatcloud-2.4.1b5/src/djtools/sync/test_sync_operations.py`

 * *Files 14% similar despite different names*

```diff
@@ -77,15 +77,18 @@
     test_config.XML_PATH = test_xml
     download_xml(test_config)
     cmd = [
         "aws",
         "s3",
         "cp",
         f's3://dj.beatcloud.com/dj/xml/{other_user}/rekordbox.xml',
-        new_xml.as_posix(),
+        # NOTE(a-rich): since we could be passing a `test_xml` formatted as a
+        # WindowsPath, the comparison needs to be made with `str(new_xml)`
+        # (rather than `new_xml.as_posix()`).
+        str(new_xml),
     ] 
     assert caplog.records[0].message == "Syncing remote rekordbox.xml..."
     assert caplog.records[1].message == " ".join(cmd)
     mock_rewrite_xml.assert_called_once()
 
 
 @pytest.mark.parametrize(
```

### Comparing `dj_beatcloud-2.4.1b4/src/djtools/test_main.py` & `dj_beatcloud-2.4.1b5/src/djtools/test_main.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b4/src/djtools/utils/__init__.py` & `dj_beatcloud-2.4.1b5/src/djtools/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b4/src/djtools/utils/check_tracks.py` & `dj_beatcloud-2.4.1b5/src/djtools/utils/check_tracks.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b4/src/djtools/utils/config.py` & `dj_beatcloud-2.4.1b5/src/djtools/utils/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b4/src/djtools/utils/helpers.py` & `dj_beatcloud-2.4.1b5/src/djtools/utils/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,15 +162,15 @@
     for _dir in config.CHECK_TRACKS_LOCAL_DIRS:
         if not _dir.exists():
             logger.warning(
                 f"{_dir} does not exist; will not be able to check its "
                 "contents against the beatcloud"
             )
             continue
-        files = (_dir / "**" / "*.*").rglob("*")
+        files = _dir.rglob("**/*.*")
         local_dir_tracks[_dir] = [_file.stem for _file in files]
 
     return local_dir_tracks
 
 
 def get_playlist_tracks(
     spotify: spotipy.Spotify, playlist_id: str
@@ -245,12 +245,13 @@
     log_file = (
         Path(__file__).parent.parent / "logs" /
         f'{datetime.now().strftime("%Y-%m-%d")}.log'
     )
     log_conf = Path(__file__).parent.parent / "configs" / "logging.conf"
     logging.config.fileConfig(
         fname=log_conf,
-        defaults={"logfilename": log_file},
+        # NOTE(a-rich): the `logfilename` needs a unix-style path.
+        defaults={"logfilename": log_file.as_posix()},
         disable_existing_loggers=False,
     )
 
     return logging.getLogger(__name__), log_file
```

### Comparing `dj_beatcloud-2.4.1b4/src/djtools/utils/test_check_tracks.py` & `dj_beatcloud-2.4.1b5/src/djtools/utils/test_check_tracks.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b4/src/djtools/utils/test_helpers.py` & `dj_beatcloud-2.4.1b5/src/djtools/utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b4/src/djtools/utils/test_url_download.py` & `dj_beatcloud-2.4.1b5/src/djtools/utils/test_url_download.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b4/src/djtools/utils/url_download.py` & `dj_beatcloud-2.4.1b5/src/djtools/utils/url_download.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b4/src/test_data/conftest.py` & `dj_beatcloud-2.4.1b5/src/test_data/conftest.py`

 * *Files identical despite different names*

